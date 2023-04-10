# Comparing `tmp/pygedcom-0.1.3.tar.gz` & `tmp/pygedcom-0.1.4.tar.gz`

## Comparing `pygedcom-0.1.3.tar` & `pygedcom-0.1.4.tar`

### file list

```diff
@@ -1,56 +1,55 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.3/__init__.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 pygedcom-0.1.3/main.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 pygedcom-0.1.3/requirements.txt
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 pygedcom-0.1.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 pygedcom-0.1.3/.github/workflows/test_and_doc.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pygedcom-0.1.3/docs/Makefile
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 pygedcom-0.1.3/docs/conf.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 pygedcom-0.1.3/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 pygedcom-0.1.3/docs/make.bat
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 pygedcom-0.1.3/docs/sources/export.rst
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pygedcom-0.1.3/docs/sources/gedcomElement.rst
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 pygedcom-0.1.3/docs/sources/gedcomParser.rst
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 pygedcom-0.1.3/docs/sources/gedcomRootElement.rst
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 pygedcom-0.1.3/docs/sources/gedcomSubElement.rst
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 pygedcom-0.1.3/docs/sources/getting_started.rst
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 pygedcom-0.1.3/docs/sources/parsing.rst
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 pygedcom-0.1.3/src/pygedcom/Exception.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pygedcom-0.1.3/src/pygedcom/__init__.py
--rw-r--r--   0        0        0    20308 2020-02-02 00:00:00.000000 pygedcom-0.1.3/src/pygedcom/gedcom_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.3/src/pygedcom/elements/__init__.py
--rw-r--r--   0        0        0     6883 2020-02-02 00:00:00.000000 pygedcom-0.1.3/src/pygedcom/elements/element.py
--rw-r--r--   0        0        0    70880 2020-02-02 00:00:00.000000 pygedcom-0.1.3/src/pygedcom/elements/mapping.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.3/src/pygedcom/elements/rootElements/__init__.py
--rw-r--r--   0        0        0     5502 2020-02-02 00:00:00.000000 pygedcom-0.1.3/src/pygedcom/elements/rootElements/family.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 pygedcom-0.1.3/src/pygedcom/elements/rootElements/head.py
--rw-r--r--   0        0        0     6113 2020-02-02 00:00:00.000000 pygedcom-0.1.3/src/pygedcom/elements/rootElements/individual.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 pygedcom-0.1.3/src/pygedcom/elements/rootElements/note.py
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 pygedcom-0.1.3/src/pygedcom/elements/rootElements/object.py
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 pygedcom-0.1.3/src/pygedcom/elements/rootElements/repository.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 pygedcom-0.1.3/src/pygedcom/elements/rootElements/rootElement.py
--rw-r--r--   0        0        0     4858 2020-02-02 00:00:00.000000 pygedcom-0.1.3/src/pygedcom/elements/rootElements/source.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 pygedcom-0.1.3/src/pygedcom/elements/rootElements/submitter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.3/src/pygedcom/elements/subElements/__init__.py
--rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 pygedcom-0.1.3/src/pygedcom/elements/subElements/commonEvent.py
--rw-r--r--   0        0        0     6363 2020-02-02 00:00:00.000000 pygedcom-0.1.3/src/pygedcom/elements/subElements/date.py
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 pygedcom-0.1.3/src/pygedcom/elements/subElements/map.py
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 pygedcom-0.1.3/src/pygedcom/elements/subElements/place.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.3/test/__init__.py
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 pygedcom-0.1.3/test/test_add_elements.py
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 pygedcom-0.1.3/test/test_export.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 pygedcom-0.1.3/test/test_parse.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 pygedcom-0.1.3/test/test_remove_element.py
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 pygedcom-0.1.3/test/test_verify.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pygedcom-0.1.3/test/samples/00_simple_individual_record.ged
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pygedcom-0.1.3/test/samples/01_simple_family_record.ged
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 pygedcom-0.1.3/test/samples/02_simple_source_record.ged
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 pygedcom-0.1.3/test/samples/03_simple_repository_record.ged
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pygedcom-0.1.3/test/samples/04_simple_date_formats.ged
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pygedcom-0.1.3/test/samples/05_all_date_modifiers.ged
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pygedcom-0.1.3/test/samples/10_invalid_level.ged
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 pygedcom-0.1.3/test/samples/20_complex_sample.ged
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 pygedcom-0.1.3/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pygedcom-0.1.3/LICENSE
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 pygedcom-0.1.3/README.md
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 pygedcom-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 pygedcom-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.4/__init__.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 pygedcom-0.1.4/main.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 pygedcom-0.1.4/requirements.txt
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 pygedcom-0.1.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 pygedcom-0.1.4/.github/workflows/test_and_doc.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pygedcom-0.1.4/docs/Makefile
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 pygedcom-0.1.4/docs/conf.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 pygedcom-0.1.4/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 pygedcom-0.1.4/docs/make.bat
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 pygedcom-0.1.4/docs/sources/export.rst
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pygedcom-0.1.4/docs/sources/gedcomElement.rst
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 pygedcom-0.1.4/docs/sources/gedcomParser.rst
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 pygedcom-0.1.4/docs/sources/gedcomRootElement.rst
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 pygedcom-0.1.4/docs/sources/gedcomSubElement.rst
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 pygedcom-0.1.4/docs/sources/getting_started.rst
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 pygedcom-0.1.4/docs/sources/parsing.rst
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pygedcom-0.1.4/src/pygedcom/__init__.py
+-rw-r--r--   0        0        0    20052 2020-02-02 00:00:00.000000 pygedcom-0.1.4/src/pygedcom/gedcom_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.4/src/pygedcom/elements/__init__.py
+-rw-r--r--   0        0        0     6883 2020-02-02 00:00:00.000000 pygedcom-0.1.4/src/pygedcom/elements/element.py
+-rw-r--r--   0        0        0    70880 2020-02-02 00:00:00.000000 pygedcom-0.1.4/src/pygedcom/elements/mapping.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.4/src/pygedcom/elements/rootElements/__init__.py
+-rw-r--r--   0        0        0     5502 2020-02-02 00:00:00.000000 pygedcom-0.1.4/src/pygedcom/elements/rootElements/family.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 pygedcom-0.1.4/src/pygedcom/elements/rootElements/head.py
+-rw-r--r--   0        0        0     6113 2020-02-02 00:00:00.000000 pygedcom-0.1.4/src/pygedcom/elements/rootElements/individual.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 pygedcom-0.1.4/src/pygedcom/elements/rootElements/note.py
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 pygedcom-0.1.4/src/pygedcom/elements/rootElements/object.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 pygedcom-0.1.4/src/pygedcom/elements/rootElements/repository.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 pygedcom-0.1.4/src/pygedcom/elements/rootElements/rootElement.py
+-rw-r--r--   0        0        0     4858 2020-02-02 00:00:00.000000 pygedcom-0.1.4/src/pygedcom/elements/rootElements/source.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 pygedcom-0.1.4/src/pygedcom/elements/rootElements/submitter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.4/src/pygedcom/elements/subElements/__init__.py
+-rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 pygedcom-0.1.4/src/pygedcom/elements/subElements/commonEvent.py
+-rw-r--r--   0        0        0     6363 2020-02-02 00:00:00.000000 pygedcom-0.1.4/src/pygedcom/elements/subElements/date.py
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 pygedcom-0.1.4/src/pygedcom/elements/subElements/map.py
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 pygedcom-0.1.4/src/pygedcom/elements/subElements/place.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.1.4/test/__init__.py
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 pygedcom-0.1.4/test/test_add_elements.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 pygedcom-0.1.4/test/test_export.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 pygedcom-0.1.4/test/test_parse.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 pygedcom-0.1.4/test/test_remove_element.py
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 pygedcom-0.1.4/test/test_verify.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pygedcom-0.1.4/test/samples/00_simple_individual_record.ged
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pygedcom-0.1.4/test/samples/01_simple_family_record.ged
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 pygedcom-0.1.4/test/samples/02_simple_source_record.ged
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 pygedcom-0.1.4/test/samples/03_simple_repository_record.ged
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pygedcom-0.1.4/test/samples/04_simple_date_formats.ged
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pygedcom-0.1.4/test/samples/05_all_date_modifiers.ged
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pygedcom-0.1.4/test/samples/10_invalid_level.ged
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 pygedcom-0.1.4/test/samples/20_complex_sample.ged
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 pygedcom-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pygedcom-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 pygedcom-0.1.4/README.md
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 pygedcom-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 pygedcom-0.1.4/PKG-INFO
```

### Comparing `pygedcom-0.1.3/requirements.txt` & `pygedcom-0.1.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.3/.github/workflows/test_and_doc.yml` & `pygedcom-0.1.4/.github/workflows/test_and_doc.yml`

 * *Files 11% similar despite different names*

```diff
@@ -20,15 +20,15 @@
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install -r requirements.txt
 
       - name: Run tests
         run: |
-          pytest --html=build/tests/index.html --self-contained-html
+          pytest --html=build/tests/index.html --self-contained-html -vv
 
       - name: Generate documentation
         run: |
           cd docs/
           make html
           cd ..
```

### Comparing `pygedcom-0.1.3/docs/Makefile` & `pygedcom-0.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.3/docs/conf.py` & `pygedcom-0.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.3/docs/index.rst` & `pygedcom-0.1.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.3/docs/make.bat` & `pygedcom-0.1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.3/docs/sources/export.rst` & `pygedcom-0.1.4/docs/sources/export.rst`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.3/docs/sources/gedcomRootElement.rst` & `pygedcom-0.1.4/docs/sources/gedcomRootElement.rst`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.3/docs/sources/gedcomSubElement.rst` & `pygedcom-0.1.4/docs/sources/gedcomSubElement.rst`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.3/docs/sources/getting_started.rst` & `pygedcom-0.1.4/docs/sources/getting_started.rst`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.3/docs/sources/parsing.rst` & `pygedcom-0.1.4/docs/sources/parsing.rst`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.3/src/pygedcom/gedcom_parser.py` & `pygedcom-0.1.4/src/pygedcom/gedcom_parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from .elements.rootElements.individual import GedcomIndividual
 from .elements.rootElements.object import GedcomObject
 from .elements.rootElements.repository import GedcomRepository
 from .elements.rootElements.source import GedcomSource
 from .elements.rootElements.submitter import GedcomSubmitter
 from .elements.rootElements.note import GedcomNote
 from .elements.element import GedcomElement
-from .Exception import FormatException, DuplicateException, NotFoundException
 
 
 class GedcomParser:
     """The GEDCOM parser main class.
 
     Use this class to initialize the parsing of a GEDCOM file.
     You can then verify, parse, access the elements and export the data.
@@ -224,17 +223,18 @@
 
         :param format: The format to export to. Default is "json".
         :type format: str
         :param empty_fields: If True, empty fields will be exported. Default is True.
         :type empty_fields: bool
         :return: The exported file's content.
         :rtype: str
+        :raises ValueError: If the format is not supported.
         """
         if format not in ["json", "gedcom"]:
-            raise FormatException("Format " + format + " is not supported.")
+            raise ValueError("Format " + format + " is not supported.")
         if format == "json":
             export = {}
             if empty_fields or self.head:
                 export["head"] = (
                     self.head.export(empty_fields=empty_fields) if self.head else ""
                 )
             if empty_fields or self.submitters:
@@ -342,15 +342,15 @@
         :type xref: str
         :return: The element if found, None otherwise.
         :rtype: GedcomElement
         """
         for element in collection:
             if element.get_xref() == xref:
                 return element
-        raise NotFoundException("Element with xref " + xref + " not found.")
+        raise KeyError("Element with xref " + xref + " not found.")
 
     def find_individual(self, xref: str) -> GedcomIndividual:
         """Find an individual by its xref.
 
         :param xref: The xref to search for.
         :type xref: str
         :return: The individual if found, None otherwise.
@@ -401,139 +401,139 @@
     def __add_root_element(self, collection: list, element: GedcomRootElement):
         """Add an element to a collection.
 
         :param collection: The collection to add the element to.
         :type collection: list
         :param element: The element to add.
         :type element: GedcomRootElement
-        :raises DuplicateException: If the element already exists.
+        :raises KeyError: If the element already exists.
         """
         try:
             self.__find_root_element(collection, element.get_xref())
-        except NotFoundException:
+        except KeyError:
             collection.append(element)
         else:
-            raise DuplicateException(
+            raise KeyError(
                 "Element with xref " + element.get_xref() + " already exists."
             )
 
     def add_individual(self, individual: GedcomIndividual):
         """Add an individual to the collection.
 
         :param individual: The individual to add.
         :type individual: GedcomIndividual
-        :raises DuplicateException: If the individual already exists.
+        :raises KeyError: If the individual already exists.
         :raises TypeError: If the individual is not of type GedcomIndividual.
         """
         if not isinstance(individual, GedcomIndividual):
             raise TypeError("Individual must be of type GedcomIndividual.")
         try:
             self.__add_root_element(self.individuals, individual)
-        except DuplicateException:
-            raise DuplicateException(
+        except KeyError:
+            raise KeyError(
                 "Individual with xref " + individual.get_xref() + " already exists."
             )
 
     def add_family(self, family: GedcomFamily):
         """Add a family to the collection.
 
         :param family: The family to add.
         :type family: GedcomFamily
-        :raises DuplicateException: If the family already exists.
+        :raises KeyError: If the family already exists.
         :raises TypeError: If the family is not of type GedcomFamily.
         """
         if not isinstance(family, GedcomFamily):
             raise TypeError("Family must be of type GedcomFamily.")
         try:
             self.__add_root_element(self.families, family)
-        except DuplicateException:
-            raise DuplicateException(
+        except KeyError:
+            raise KeyError(
                 "Family with xref " + family.get_xref() + " already exists."
             )
         self.families.append(family)
 
     def add_source(self, source: GedcomSource):
         """Add a source to the collection.
 
         :param source: The source to add.
         :type source: GedcomSource
-        :raises DuplicateException: If the source already exists.
+        :raises KeyError: If the source already exists.
         :raises TypeError: If the source is not of type GedcomSource.
         """
         if not isinstance(source, GedcomSource):
             raise TypeError("Source must be of type GedcomSource.")
         try:
             self.__add_root_element(self.sources, source)
-        except DuplicateException:
-            raise DuplicateException(
+        except KeyError:
+            raise KeyError(
                 "Source with xref " + source.get_xref() + " already exists."
             )
         self.sources.append(source)
 
     def add_object(self, object: GedcomObject):
         """Add an object to the collection.
 
         :param object: The object to add.
         :type object: GedcomObject
-        :raises DuplicateException: If the object already exists.
+        :raises KeyError: If the object already exists.
         :raises TypeError: If the object is not of type GedcomObject.
         """
         if not isinstance(object, GedcomObject):
             raise TypeError("Object must be of type GedcomObject.")
         try:
             self.__add_root_element(self.objects, object)
-        except DuplicateException:
-            raise DuplicateException(
+        except KeyError:
+            raise KeyError(
                 "Object with xref " + object.get_xref() + " already exists."
             )
         self.objects.append(object)
 
     def add_repository(self, repository: GedcomRepository):
         """Add a repository to the collection.
 
         :param repository: The repository to add.
         :type repository: GedcomRepository
-        :raises DuplicateException: If the repository already exists.
+        :raises KeyError: If the repository already exists.
         :raises TypeError: If the repository is not of type GedcomRepository.
         """
         if not isinstance(repository, GedcomRepository):
             raise TypeError("Repository must be of type GedcomRepository.")
         try:
             self.__add_root_element(self.repositories, repository)
-        except DuplicateException:
-            raise DuplicateException(
+        except KeyError:
+            raise KeyError(
                 "Repository with xref " + repository.get_xref() + " already exists."
             )
         self.repositories.append(repository)
 
     def __remove_root_element(self, collection: list, xref: str):
         """Remove an element from a collection.
 
         :param collection: The collection to remove the element from.
         :type collection: list
         :param xref: The xref of the element to remove.
         :type xref: str
-        :raises NotFoundException: If the element does not exist.
+        :raises KeyError: If the element does not exist.
         """
         element = self.__find_root_element(collection, xref)
         if not element:
-            raise NotFoundException()
+            raise KeyError()
         collection.remove(element)
 
     def remove_individual(self, xref: str):
         """Remove an individual from the collection.
 
         :param xref: The xref of the individual to remove.
         :type xref: str
-        :raises NotFoundException: If the individual does not exist.
+        :raises KeyError: If the individual does not exist.
         """
         try:
             individual = self.find_individual(xref)
-        except NotFoundException:
-            raise NotFoundException("Individual with xref " + xref + " does not exist.")
+        except KeyError:
+            raise KeyError("Individual with xref " + xref + " does not exist.")
 
         xref = individual.get_xref()
 
         for family in self.families:
             family.remove_parent(xref)
             family.remove_child(xref)
```

### Comparing `pygedcom-0.1.3/src/pygedcom/elements/element.py` & `pygedcom-0.1.4/src/pygedcom/elements/element.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.3/src/pygedcom/elements/mapping.json` & `pygedcom-0.1.4/src/pygedcom/elements/mapping.json`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.3/src/pygedcom/elements/rootElements/family.py` & `pygedcom-0.1.4/src/pygedcom/elements/rootElements/family.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.3/src/pygedcom/elements/rootElements/head.py` & `pygedcom-0.1.4/src/pygedcom/elements/rootElements/head.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.3/src/pygedcom/elements/rootElements/individual.py` & `pygedcom-0.1.4/src/pygedcom/elements/rootElements/individual.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.3/src/pygedcom/elements/rootElements/note.py` & `pygedcom-0.1.4/src/pygedcom/elements/rootElements/note.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.3/src/pygedcom/elements/rootElements/object.py` & `pygedcom-0.1.4/src/pygedcom/elements/rootElements/object.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.3/src/pygedcom/elements/rootElements/repository.py` & `pygedcom-0.1.4/src/pygedcom/elements/rootElements/repository.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.3/src/pygedcom/elements/rootElements/rootElement.py` & `pygedcom-0.1.4/src/pygedcom/elements/rootElements/rootElement.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.3/src/pygedcom/elements/rootElements/source.py` & `pygedcom-0.1.4/src/pygedcom/elements/rootElements/source.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.3/src/pygedcom/elements/rootElements/submitter.py` & `pygedcom-0.1.4/src/pygedcom/elements/rootElements/submitter.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.3/src/pygedcom/elements/subElements/commonEvent.py` & `pygedcom-0.1.4/src/pygedcom/elements/subElements/commonEvent.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.3/src/pygedcom/elements/subElements/date.py` & `pygedcom-0.1.4/src/pygedcom/elements/subElements/date.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.3/src/pygedcom/elements/subElements/map.py` & `pygedcom-0.1.4/src/pygedcom/elements/subElements/map.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.3/src/pygedcom/elements/subElements/place.py` & `pygedcom-0.1.4/src/pygedcom/elements/subElements/place.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.3/test/test_add_elements.py` & `pygedcom-0.1.4/test/test_add_elements.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.3/test/test_export.py` & `pygedcom-0.1.4/test/test_export.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.3/test/test_parse.py` & `pygedcom-0.1.4/test/test_parse.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.3/test/test_remove_element.py` & `pygedcom-0.1.4/test/test_remove_element.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.3/test/test_verify.py` & `pygedcom-0.1.4/test/test_verify.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.3/test/samples/20_complex_sample.ged` & `pygedcom-0.1.4/test/samples/20_complex_sample.ged`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.3/.gitignore` & `pygedcom-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.3/LICENSE` & `pygedcom-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.3/README.md` & `pygedcom-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pygedcom-0.1.3/pyproject.toml` & `pygedcom-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pygedcom"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
     { name="Theo Petit", email="theo.p83@gmail.com" },
 ]
 description = "A gedcom utility library"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pygedcom-0.1.3/PKG-INFO` & `pygedcom-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygedcom
-Version: 0.1.3
+Version: 0.1.4
 Summary: A gedcom utility library
 Project-URL: Homepage, https://github.com/topetit/pygedcom
 Project-URL: Bug Tracker, https://github.com/topetit/pygedcom/issues
 Author-email: Theo Petit <theo.p83@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

