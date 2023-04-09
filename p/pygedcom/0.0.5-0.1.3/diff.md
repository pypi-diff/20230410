# Comparing `tmp/pygedcom-0.0.5.tar.gz` & `tmp/pygedcom-0.1.3.tar.gz`

## Comparing `pygedcom-0.0.5.tar` & `pygedcom-0.1.3.tar`

### file list

```diff
@@ -1,52 +1,56 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.0.5/__init__.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 pygedcom-0.0.5/main.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 pygedcom-0.0.5/requirements.txt
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 pygedcom-0.0.5/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 pygedcom-0.0.5/.github/workflows/test_and_doc.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pygedcom-0.0.5/docs/Makefile
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 pygedcom-0.0.5/docs/conf.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 pygedcom-0.0.5/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 pygedcom-0.0.5/docs/make.bat
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 pygedcom-0.0.5/docs/sources/export.rst
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pygedcom-0.0.5/docs/sources/gedcomElement.rst
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 pygedcom-0.0.5/docs/sources/gedcomParser.rst
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 pygedcom-0.0.5/docs/sources/gedcomRootElement.rst
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 pygedcom-0.0.5/docs/sources/gedcomSubElement.rst
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 pygedcom-0.0.5/docs/sources/getting_started.rst
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 pygedcom-0.0.5/docs/sources/parsing.rst
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pygedcom-0.0.5/src/pygedcom/FormatException.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pygedcom-0.0.5/src/pygedcom/__init__.py
--rw-r--r--   0        0        0    12986 2020-02-02 00:00:00.000000 pygedcom-0.0.5/src/pygedcom/gedcom_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.0.5/src/pygedcom/elements/__init__.py
--rw-r--r--   0        0        0     6047 2020-02-02 00:00:00.000000 pygedcom-0.0.5/src/pygedcom/elements/element.py
--rw-r--r--   0        0        0    70880 2020-02-02 00:00:00.000000 pygedcom-0.0.5/src/pygedcom/elements/mapping.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.0.5/src/pygedcom/elements/rootElements/__init__.py
--rw-r--r--   0        0        0     4416 2020-02-02 00:00:00.000000 pygedcom-0.0.5/src/pygedcom/elements/rootElements/family.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 pygedcom-0.0.5/src/pygedcom/elements/rootElements/head.py
--rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 pygedcom-0.0.5/src/pygedcom/elements/rootElements/individual.py
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 pygedcom-0.0.5/src/pygedcom/elements/rootElements/object.py
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 pygedcom-0.0.5/src/pygedcom/elements/rootElements/repository.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 pygedcom-0.0.5/src/pygedcom/elements/rootElements/rootElement.py
--rw-r--r--   0        0        0     4858 2020-02-02 00:00:00.000000 pygedcom-0.0.5/src/pygedcom/elements/rootElements/source.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.0.5/src/pygedcom/elements/subElements/__init__.py
--rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 pygedcom-0.0.5/src/pygedcom/elements/subElements/commonEvent.py
--rw-r--r--   0        0        0     6363 2020-02-02 00:00:00.000000 pygedcom-0.0.5/src/pygedcom/elements/subElements/date.py
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 pygedcom-0.0.5/src/pygedcom/elements/subElements/map.py
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 pygedcom-0.0.5/src/pygedcom/elements/subElements/place.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.0.5/test/__init__.py
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 pygedcom-0.0.5/test/test_export.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 pygedcom-0.0.5/test/test_parse.py
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 pygedcom-0.0.5/test/test_verify.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pygedcom-0.0.5/test/samples/00_simple_individual_record.ged
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pygedcom-0.0.5/test/samples/01_simple_family_record.ged
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 pygedcom-0.0.5/test/samples/02_simple_source_record.ged
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 pygedcom-0.0.5/test/samples/03_simple_repository_record.ged
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pygedcom-0.0.5/test/samples/04_simple_date_formats.ged
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pygedcom-0.0.5/test/samples/05_all_date_modifiers.ged
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pygedcom-0.0.5/test/samples/10_invalid_level.ged
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 pygedcom-0.0.5/test/samples/20_complex_sample.ged
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 pygedcom-0.0.5/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pygedcom-0.0.5/LICENSE
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 pygedcom-0.0.5/README.md
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 pygedcom-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 pygedcom-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.3/__init__.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 pygedcom-0.1.3/main.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 pygedcom-0.1.3/requirements.txt
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 pygedcom-0.1.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 pygedcom-0.1.3/.github/workflows/test_and_doc.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pygedcom-0.1.3/docs/Makefile
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 pygedcom-0.1.3/docs/conf.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 pygedcom-0.1.3/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 pygedcom-0.1.3/docs/make.bat
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 pygedcom-0.1.3/docs/sources/export.rst
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pygedcom-0.1.3/docs/sources/gedcomElement.rst
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 pygedcom-0.1.3/docs/sources/gedcomParser.rst
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 pygedcom-0.1.3/docs/sources/gedcomRootElement.rst
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 pygedcom-0.1.3/docs/sources/gedcomSubElement.rst
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 pygedcom-0.1.3/docs/sources/getting_started.rst
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 pygedcom-0.1.3/docs/sources/parsing.rst
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 pygedcom-0.1.3/src/pygedcom/Exception.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pygedcom-0.1.3/src/pygedcom/__init__.py
+-rw-r--r--   0        0        0    20308 2020-02-02 00:00:00.000000 pygedcom-0.1.3/src/pygedcom/gedcom_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.3/src/pygedcom/elements/__init__.py
+-rw-r--r--   0        0        0     6883 2020-02-02 00:00:00.000000 pygedcom-0.1.3/src/pygedcom/elements/element.py
+-rw-r--r--   0        0        0    70880 2020-02-02 00:00:00.000000 pygedcom-0.1.3/src/pygedcom/elements/mapping.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.3/src/pygedcom/elements/rootElements/__init__.py
+-rw-r--r--   0        0        0     5502 2020-02-02 00:00:00.000000 pygedcom-0.1.3/src/pygedcom/elements/rootElements/family.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 pygedcom-0.1.3/src/pygedcom/elements/rootElements/head.py
+-rw-r--r--   0        0        0     6113 2020-02-02 00:00:00.000000 pygedcom-0.1.3/src/pygedcom/elements/rootElements/individual.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 pygedcom-0.1.3/src/pygedcom/elements/rootElements/note.py
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 pygedcom-0.1.3/src/pygedcom/elements/rootElements/object.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 pygedcom-0.1.3/src/pygedcom/elements/rootElements/repository.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 pygedcom-0.1.3/src/pygedcom/elements/rootElements/rootElement.py
+-rw-r--r--   0        0        0     4858 2020-02-02 00:00:00.000000 pygedcom-0.1.3/src/pygedcom/elements/rootElements/source.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 pygedcom-0.1.3/src/pygedcom/elements/rootElements/submitter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.3/src/pygedcom/elements/subElements/__init__.py
+-rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 pygedcom-0.1.3/src/pygedcom/elements/subElements/commonEvent.py
+-rw-r--r--   0        0        0     6363 2020-02-02 00:00:00.000000 pygedcom-0.1.3/src/pygedcom/elements/subElements/date.py
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 pygedcom-0.1.3/src/pygedcom/elements/subElements/map.py
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 pygedcom-0.1.3/src/pygedcom/elements/subElements/place.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.3/test/__init__.py
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 pygedcom-0.1.3/test/test_add_elements.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 pygedcom-0.1.3/test/test_export.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 pygedcom-0.1.3/test/test_parse.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 pygedcom-0.1.3/test/test_remove_element.py
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 pygedcom-0.1.3/test/test_verify.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pygedcom-0.1.3/test/samples/00_simple_individual_record.ged
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pygedcom-0.1.3/test/samples/01_simple_family_record.ged
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 pygedcom-0.1.3/test/samples/02_simple_source_record.ged
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 pygedcom-0.1.3/test/samples/03_simple_repository_record.ged
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pygedcom-0.1.3/test/samples/04_simple_date_formats.ged
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pygedcom-0.1.3/test/samples/05_all_date_modifiers.ged
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pygedcom-0.1.3/test/samples/10_invalid_level.ged
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 pygedcom-0.1.3/test/samples/20_complex_sample.ged
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 pygedcom-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pygedcom-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 pygedcom-0.1.3/README.md
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 pygedcom-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 pygedcom-0.1.3/PKG-INFO
```

### Comparing `pygedcom-0.0.5/requirements.txt` & `pygedcom-0.1.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `pygedcom-0.0.5/.github/workflows/python-publish.yml` & `pygedcom-0.1.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pygedcom-0.0.5/.github/workflows/test_and_doc.yml` & `pygedcom-0.1.3/.github/workflows/test_and_doc.yml`

 * *Files identical despite different names*

### Comparing `pygedcom-0.0.5/docs/Makefile` & `pygedcom-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pygedcom-0.0.5/docs/conf.py` & `pygedcom-0.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.0.5/docs/index.rst` & `pygedcom-0.1.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pygedcom-0.0.5/docs/make.bat` & `pygedcom-0.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pygedcom-0.0.5/docs/sources/export.rst` & `pygedcom-0.1.3/docs/sources/export.rst`

 * *Files identical despite different names*

### Comparing `pygedcom-0.0.5/docs/sources/gedcomRootElement.rst` & `pygedcom-0.1.3/docs/sources/gedcomRootElement.rst`

 * *Files identical despite different names*

### Comparing `pygedcom-0.0.5/docs/sources/gedcomSubElement.rst` & `pygedcom-0.1.3/docs/sources/gedcomSubElement.rst`

 * *Files identical despite different names*

### Comparing `pygedcom-0.0.5/docs/sources/getting_started.rst` & `pygedcom-0.1.3/docs/sources/getting_started.rst`

 * *Files identical despite different names*

### Comparing `pygedcom-0.0.5/docs/sources/parsing.rst` & `pygedcom-0.1.3/docs/sources/parsing.rst`

 * *Files identical despite different names*

### Comparing `pygedcom-0.0.5/src/pygedcom/elements/mapping.json` & `pygedcom-0.1.3/src/pygedcom/elements/mapping.json`

 * *Files identical despite different names*

### Comparing `pygedcom-0.0.5/src/pygedcom/elements/rootElements/family.py` & `pygedcom-0.1.3/src/pygedcom/elements/rootElements/family.py`

 * *Files 18% similar despite different names*

```diff
@@ -120,15 +120,15 @@
 
     def get_parents(self) -> list:
         """Get the parents of the family.
 
         :return: The parents of the family.
         :rtype: list
         """
-        return [self.__export_husband, self.__wife]
+        return [self.__export_husband, self.__export_wife]
 
     def get_married(self) -> bool:
         """Get if the family is married.
 
         :return: True if the family is married, False otherwise.
         :rtype: bool
         """
@@ -145,7 +145,35 @@
     def get_media(self) -> list:
         """Get the media of the family.
 
         :return: The media of the family.
         :rtype: list
         """
         return self.__export_media
+
+    def remove_child(self, child_xref: str):
+        """Remove a child from the family.
+
+        :param child_xref: The xref of the child to remove.
+        :type child_xref: str
+        """
+        for child in self.find_sub_element("CHIL"):
+            if child.get_value() == child_xref:
+                self.remove_sub_element(child)
+        self.__export_children.remove(
+            child_xref
+        ) if child_xref in self.__export_children else None
+
+    def remove_parent(self, parent_xref: str):
+        """Remove a parent from the family.
+
+        :param parent_xref: The xref of the parent to remove.
+        :type parent_xref: str
+        """
+        for parent in ["HUSB", "WIFE"]:
+            if self.find_sub_element(parent) != []:
+                if self.find_sub_element(parent)[0].get_value() == parent_xref:
+                    self.remove_sub_element(self.find_sub_element(parent)[0])
+        if self.__export_husband == parent_xref:
+            self.__export_husband = ""
+        if self.__export_wife == parent_xref:
+            self.__export_wife = ""
```

### Comparing `pygedcom-0.0.5/src/pygedcom/elements/rootElements/head.py` & `pygedcom-0.1.3/src/pygedcom/elements/rootElements/head.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from .rootElement import GedcomRootElement
 
+
 class GedcomHead(GedcomRootElement):
     """Class for the HEAD element.
 
     :param level: The level of the HEAD element.
     :type level: int
     :param tag: The tag of the HEAD element.
     :type tag: str
```

### Comparing `pygedcom-0.0.5/src/pygedcom/elements/rootElements/individual.py` & `pygedcom-0.1.3/src/pygedcom/elements/rootElements/individual.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from ...elements.element import GedcomElement
 from ..subElements.commonEvent import GedcomCommonEvent
 from .rootElement import GedcomRootElement
 
 
 class GedcomIndividual(GedcomRootElement):
     """This class represents an individual in the gedcom file.
 
@@ -49,15 +50,15 @@
 
     def __find_last_name(self):
         """Find the last name of the individual.
 
         :return: The last name of the individual.
         :rtype: str
         """
-        return self.__export_name.split("/")[-2].strip()
+        return self.__export_name.split("/")[-2].strip() if self.__export_name else ""
 
     def __init_birth(self) -> GedcomCommonEvent:
         """Initialize the birth of the individual.
 
         :return: The birth of the individual.
         :rtype: GedcomCommonEvent
         """
@@ -155,14 +156,42 @@
         """Get the media of the individual.
 
         :return: The media of the individual
         :rtype: list
         """
         return self.__export_media
 
+    def set_first_name(self, first_name: str):
+        """Set the first name of the individual.
+
+        :param first_name: The first name of the individual.
+        :type first_name: str
+        """
+        self.__export_first_name = first_name
+        self.__export_name = f"{first_name} /{self.__export_last_name}/"
+        name_element = self.find_sub_element("NAME")
+        if name_element != []:
+            name_element[0].set_value(self.__export_name)
+        else:
+            self.add_sub_element(2, "NAME", [], value=self.__export_name)
+
+    def set_last_name(self, last_name: str):
+        """Set the last name of the individual.
+
+        :param last_name: The last name of the individual.
+        :type last_name: str
+        """
+        self.__export_last_name = last_name
+        self.__export_name = f"{self.__export_first_name} /{last_name}/"
+        name_element = self.find_sub_element("NAME")
+        if name_element != []:
+            name_element[0].set_value(self.__export_name)
+        else:
+            self.add_sub_element(2, "NAME", [], value=self.__export_name)
+
     def __str__(self):
         """Get the string representation of the individual.
 
         :return: The string representation of the individual.
         :rtype: str
         """
         return self.__export_first_name + " " + self.__export_last_name
```

### Comparing `pygedcom-0.0.5/src/pygedcom/elements/rootElements/object.py` & `pygedcom-0.1.3/src/pygedcom/elements/rootElements/object.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from .rootElement import GedcomRootElement
 
+
 class GedcomObject(GedcomRootElement):
     """This class represents an object in the gedcom file.
 
     :param level: The level of the Gedcom object.
     :type level: int
     :param xref: The xref of the Gedcom object.
     :type xref: str
```

### Comparing `pygedcom-0.0.5/src/pygedcom/elements/rootElements/repository.py` & `pygedcom-0.1.3/src/pygedcom/elements/rootElements/repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from .rootElement import GedcomRootElement
 
+
 class GedcomRepository(GedcomRootElement):
     """This class represents a repository in the gedcom file.
 
     :param level: The level of the Gedcom repository.
     :type level: int
     :param xref: The xref of the Gedcom repository.
     :type xref: str
```

### Comparing `pygedcom-0.0.5/src/pygedcom/elements/rootElements/rootElement.py` & `pygedcom-0.1.3/src/pygedcom/elements/rootElements/rootElement.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.0.5/src/pygedcom/elements/rootElements/source.py` & `pygedcom-0.1.3/src/pygedcom/elements/rootElements/source.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.0.5/src/pygedcom/elements/subElements/commonEvent.py` & `pygedcom-0.1.3/src/pygedcom/elements/subElements/commonEvent.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.0.5/src/pygedcom/elements/subElements/date.py` & `pygedcom-0.1.3/src/pygedcom/elements/subElements/date.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.0.5/src/pygedcom/elements/subElements/map.py` & `pygedcom-0.1.3/src/pygedcom/elements/subElements/map.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.0.5/src/pygedcom/elements/subElements/place.py` & `pygedcom-0.1.3/src/pygedcom/elements/subElements/place.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.0.5/test/test_export.py` & `pygedcom-0.1.3/test/test_add_elements.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,29 @@
 import json
 from ..src.pygedcom import gedcom_parser
+from ..src.pygedcom.elements.rootElements.individual import GedcomIndividual
 
 
-def test_export_00():
+def test_add_individual():
     parser = gedcom_parser.GedcomParser("test/samples/00_simple_individual_record.ged")
     parser.parse()
+    newIndividual = GedcomIndividual(0, "@I2@", "INDI", [])
+    newIndividual.set_first_name("John")
+    newIndividual.set_last_name("Wick")
+    parser.add_individual(newIndividual)
+    assert len(parser.individuals) == 2
+    assert parser.individuals[1].get_xref() == "@I2@"
+    assert parser.individuals[1].get_first_name() == "John"
+    assert parser.individuals[1].get_last_name() == "Wick"
     result = json.loads(parser.export())
     assert result["individuals"]["@I1@"]["name"] == "John /Doe/"
     assert result["individuals"]["@I1@"]["first_name"] == "John"
     assert result["individuals"]["@I1@"]["last_name"] == "Doe"
     assert result["individuals"]["@I1@"]["birth"]["date"]["day"] == "01"
     assert result["individuals"]["@I1@"]["birth"]["date"]["month"] == "JAN"
     assert result["individuals"]["@I1@"]["birth"]["date"]["year"] == "1900"
     assert result["individuals"]["@I1@"]["death"]["date"]["day"] == "01"
     assert result["individuals"]["@I1@"]["death"]["date"]["month"] == "JAN"
     assert result["individuals"]["@I1@"]["death"]["date"]["year"] == "1970"
-
-
-def test_export_01():
-    parser = gedcom_parser.GedcomParser("test/samples/01_simple_family_record.ged")
-    parser.parse()
-    result = json.loads(parser.export())
-    assert result["families"]["@F1@"]["husband"] == "@I1@"
-    assert result["families"]["@F1@"]["wife"] == "@I2@"
-    assert result["families"]["@F1@"]["children"] == ["@I3@"]
-    assert result["families"]["@F1@"]["marriage"]["date"]["day"] == "01"
-    assert result["families"]["@F1@"]["marriage"]["date"]["month"] == "JAN"
-    assert result["families"]["@F1@"]["marriage"]["date"]["year"] == "1925"
-
-
-def test_export_20():
-    parser = gedcom_parser.GedcomParser("test/samples/20_complex_sample.ged")
-    parser.parse()
-    result = json.loads(parser.export())
-    assert result["individuals"]["@1@"]["name"] == "Robert Eugene/Williams/"
-    assert result["individuals"]["@1@"]["birth"]["date"]["day"] == "02"
-    assert result["individuals"]["@1@"]["birth"]["date"]["month"] == "OCT"
-    assert result["individuals"]["@1@"]["birth"]["date"]["year"] == "1822"
-    assert result["individuals"]["@1@"]["sex"] == "M"
-    assert result["individuals"]["@1@"]["death"]["date"]["day"] == "14"
-    assert result["individuals"]["@1@"]["death"]["date"]["month"] == "APR"
-    assert result["individuals"]["@1@"]["death"]["date"]["year"] == "1905"
+    assert result["individuals"]["@I2@"]["name"] == "John /Wick/"
+    assert result["individuals"]["@I2@"]["first_name"] == "John"
+    assert result["individuals"]["@I2@"]["last_name"] == "Wick"
```

### Comparing `pygedcom-0.0.5/test/test_parse.py` & `pygedcom-0.1.3/test/test_parse.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.0.5/test/test_verify.py` & `pygedcom-0.1.3/test/test_verify.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.0.5/.gitignore` & `pygedcom-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pygedcom-0.0.5/LICENSE` & `pygedcom-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pygedcom-0.0.5/README.md` & `pygedcom-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pygedcom-0.0.5/pyproject.toml` & `pygedcom-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pygedcom"
-version = "0.0.5"
+version = "0.1.3"
 authors = [
     { name="Theo Petit", email="theo.p83@gmail.com" },
 ]
 description = "A gedcom utility library"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pygedcom-0.0.5/PKG-INFO` & `pygedcom-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygedcom
-Version: 0.0.5
+Version: 0.1.3
 Summary: A gedcom utility library
 Project-URL: Homepage, https://github.com/topetit/pygedcom
 Project-URL: Bug Tracker, https://github.com/topetit/pygedcom/issues
 Author-email: Theo Petit <theo.p83@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

