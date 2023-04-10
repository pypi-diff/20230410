# Comparing `tmp/molmass-2022.12.9.tar.gz` & `tmp/molmass-2023.4.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molmass-2022.12.9.tar", last modified: Fri Dec  9 00:20:15 2022, max compression
+gzip compressed data, was "molmass-2023.4.10.tar", last modified: Mon Apr 10 02:43:46 2023, max compression
```

## Comparing `molmass-2022.12.9.tar` & `molmass-2023.4.10.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2022-12-09 00:20:15.739705 molmass-2022.12.9/
--rw-rw-rw-   0        0        0     1559 2022-12-09 00:20:13.000000 molmass-2022.12.9/LICENSE
--rw-rw-rw-   0        0        0      277 2022-12-09 00:10:38.000000 molmass-2022.12.9/MANIFEST.in
--rw-rw-rw-   0        0        0     6393 2022-12-09 00:20:15.739705 molmass-2022.12.9/PKG-INFO
--rw-rw-rw-   0        0        0     5446 2022-12-09 00:20:13.000000 molmass-2022.12.9/README.rst
-drwxrwxrwx   0        0        0        0 2022-12-09 00:20:15.730804 molmass-2022.12.9/molmass/
--rw-rw-rw-   0        0        0      206 2022-10-18 17:06:47.000000 molmass-2022.12.9/molmass/__init__.py
--rw-rw-rw-   0        0        0      132 2020-01-01 02:11:19.000000 molmass-2022.12.9/molmass/__main__.py
--rw-rw-rw-   0        0        0    81328 2022-12-08 23:45:38.000000 molmass-2022.12.9/molmass/elements.py
--rw-rw-rw-   0        0        0    44876 2022-10-18 03:17:47.000000 molmass-2022.12.9/molmass/elements_descriptions.py
--rw-rw-rw-   0        0        0    39072 2022-10-18 02:53:39.000000 molmass-2022.12.9/molmass/elements_gui.py
--rw-rw-rw-   0        0        0      355 2010-03-08 22:00:45.000000 molmass-2022.12.9/molmass/icon.png
--rw-rw-rw-   0        0        0    72707 2022-12-09 00:20:03.000000 molmass-2022.12.9/molmass/molmass.py
--rw-rw-rw-   0        0        0    19538 2022-12-08 20:52:02.000000 molmass-2022.12.9/molmass/web.py
-drwxrwxrwx   0        0        0        0 2022-12-09 00:20:15.739705 molmass-2022.12.9/molmass.egg-info/
--rw-rw-rw-   0        0        0     6393 2022-12-09 00:20:14.000000 molmass-2022.12.9/molmass.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      395 2022-12-09 00:20:15.000000 molmass-2022.12.9/molmass.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-09 00:20:14.000000 molmass-2022.12.9/molmass.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      136 2022-12-09 00:20:14.000000 molmass-2022.12.9/molmass.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       41 2022-12-09 00:20:14.000000 molmass-2022.12.9/molmass.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-12-09 00:20:14.000000 molmass-2022.12.9/molmass.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-09 00:20:15.739705 molmass-2022.12.9/setup.cfg
--rw-rw-rw-   0        0        0     2573 2022-10-17 17:53:47.000000 molmass-2022.12.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 02:43:46.161915 molmass-2023.4.10/
+-rw-rw-rw-   0        0        0     1559 2023-04-10 02:43:43.000000 molmass-2023.4.10/LICENSE
+-rw-rw-rw-   0        0        0      277 2022-12-09 00:10:38.000000 molmass-2023.4.10/MANIFEST.in
+-rw-rw-rw-   0        0        0     6595 2023-04-10 02:43:46.161915 molmass-2023.4.10/PKG-INFO
+-rw-rw-rw-   0        0        0     5648 2023-04-10 02:43:43.000000 molmass-2023.4.10/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-10 02:43:46.161915 molmass-2023.4.10/molmass/
+-rw-rw-rw-   0        0        0      206 2022-10-18 17:06:47.000000 molmass-2023.4.10/molmass/__init__.py
+-rw-rw-rw-   0        0        0      132 2020-01-01 02:11:19.000000 molmass-2023.4.10/molmass/__main__.py
+-rw-rw-rw-   0        0        0    81328 2023-03-08 22:26:52.000000 molmass-2023.4.10/molmass/elements.py
+-rw-rw-rw-   0        0        0    44874 2023-03-08 23:01:23.000000 molmass-2023.4.10/molmass/elements_descriptions.py
+-rw-rw-rw-   0        0        0    39072 2023-04-09 04:46:58.000000 molmass-2023.4.10/molmass/elements_gui.py
+-rw-rw-rw-   0        0        0      355 2010-03-08 22:00:45.000000 molmass-2023.4.10/molmass/icon.png
+-rw-rw-rw-   0        0        0    74302 2023-04-10 02:37:52.000000 molmass-2023.4.10/molmass/molmass.py
+-rw-rw-rw-   0        0        0    19552 2023-04-09 04:11:15.000000 molmass-2023.4.10/molmass/web.py
+drwxrwxrwx   0        0        0        0 2023-04-10 02:43:46.161915 molmass-2023.4.10/molmass.egg-info/
+-rw-rw-rw-   0        0        0     6595 2023-04-10 02:43:45.000000 molmass-2023.4.10/molmass.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      395 2023-04-10 02:43:45.000000 molmass-2023.4.10/molmass.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 02:43:45.000000 molmass-2023.4.10/molmass.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      136 2023-04-10 02:43:45.000000 molmass-2023.4.10/molmass.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       41 2023-04-10 02:43:45.000000 molmass-2023.4.10/molmass.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-10 02:43:45.000000 molmass-2023.4.10/molmass.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 02:43:46.161915 molmass-2023.4.10/setup.cfg
+-rw-rw-rw-   0        0        0     2573 2022-10-17 17:53:47.000000 molmass-2023.4.10/setup.py
```

### Comparing `molmass-2022.12.9/LICENSE` & `molmass-2023.4.10/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 1990-2022, Christoph Gohlke
+Copyright (c) 1990-2023, Christoph Gohlke
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice,
    this list of conditions and the following disclaimer.
```

### Comparing `molmass-2022.12.9/PKG-INFO` & `molmass-2023.4.10/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molmass
-Version: 2022.12.9
+Version: 2023.4.10
 Summary: Molecular mass calculations
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/molmass/issues
 Project-URL: Source Code, https://github.com/cgohlke/molmass
@@ -36,22 +36,22 @@
 deficiency due to chemical bonding is not taken into account.
 
 The library includes a database of physicochemical and descriptive properties
 of the chemical elements.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2022.12.9
-:DOI: 10.5281/zenodo.7135495
+:Version: 2023.4.10
+:DOI: `10.5281/zenodo.7135495 <https://doi.org/10.5281/zenodo.7135495>`_
 
 Quickstart
 ----------
 
 Install the molmass package and all dependencies from the
-Python Package Index::
+`Python Package Index <https://pypi.org/project/molmass/>`_::
 
     python -m pip install -U molmass[all]
 
 Print the console script usage::
 
     python -m molmass --help
 
@@ -65,25 +65,30 @@
 
 Source code and support are available on
 `GitHub <https://github.com/cgohlke/molmass>`_.
 
 Requirements
 ------------
 
-This release has been tested with the following requirements and dependencies
+This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython 3.8.10, 3.9.13, 3.10.9, 3.11.1 <https://www.python.org>`_
-- `Flask 2.2.2 <https://pypi.org/project/Flask/>`_ (optional)
-- `Pandas 1.5.2 <https://pypi.org/project/pandas/>`_ (optional)
-- `wxPython 4.2.0 <https://pypi.org/project/wxPython/>`_ (optional)
+- `CPython <https://www.python.org>`_ 3.8.10, 3.9.13, 3.10.11, 3.11.3
+- `Flask <https://pypi.org/project/Flask/>`_ 2.2.3 (optional)
+- `Pandas <https://pypi.org/project/pandas/>`_ 1.5.3 (optional)
+- `wxPython <https://pypi.org/project/wxPython/>`_ 4.2.0 (optional)
 
 Revisions
 ---------
 
+2023.4.10
+
+- Support rdkit-style ionic charges (#11, #12).
+- Enable multiplication without addition in from_string.
+
 2022.12.9
 
 - Fix split_charge formula with trailing ]] (#11).
 
 2022.10.18
 
 - Several breaking changes.
```

### Comparing `molmass-2022.12.9/README.rst` & `molmass-2023.4.10/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 deficiency due to chemical bonding is not taken into account.
 
 The library includes a database of physicochemical and descriptive properties
 of the chemical elements.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2022.12.9
-:DOI: 10.5281/zenodo.7135495
+:Version: 2023.4.10
+:DOI: `10.5281/zenodo.7135495 <https://doi.org/10.5281/zenodo.7135495>`_
 
 Quickstart
 ----------
 
 Install the molmass package and all dependencies from the
-Python Package Index::
+`Python Package Index <https://pypi.org/project/molmass/>`_::
 
     python -m pip install -U molmass[all]
 
 Print the console script usage::
 
     python -m molmass --help
 
@@ -39,25 +39,30 @@
 
 Source code and support are available on
 `GitHub <https://github.com/cgohlke/molmass>`_.
 
 Requirements
 ------------
 
-This release has been tested with the following requirements and dependencies
+This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython 3.8.10, 3.9.13, 3.10.9, 3.11.1 <https://www.python.org>`_
-- `Flask 2.2.2 <https://pypi.org/project/Flask/>`_ (optional)
-- `Pandas 1.5.2 <https://pypi.org/project/pandas/>`_ (optional)
-- `wxPython 4.2.0 <https://pypi.org/project/wxPython/>`_ (optional)
+- `CPython <https://www.python.org>`_ 3.8.10, 3.9.13, 3.10.11, 3.11.3
+- `Flask <https://pypi.org/project/Flask/>`_ 2.2.3 (optional)
+- `Pandas <https://pypi.org/project/pandas/>`_ 1.5.3 (optional)
+- `wxPython <https://pypi.org/project/wxPython/>`_ 4.2.0 (optional)
 
 Revisions
 ---------
 
+2023.4.10
+
+- Support rdkit-style ionic charges (#11, #12).
+- Enable multiplication without addition in from_string.
+
 2022.12.9
 
 - Fix split_charge formula with trailing ]] (#11).
 
 2022.10.18
 
 - Several breaking changes.
```

### Comparing `molmass-2022.12.9/molmass/elements.py` & `molmass-2023.4.10/molmass/elements.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # molmass/elements.py
 
-# Copyright (c) 2005-2022, Christoph Gohlke
+# Copyright (c) 2005-2023, Christoph Gohlke
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
```

### Comparing `molmass-2022.12.9/molmass/elements_descriptions.py` & `molmass-2023.4.10/molmass/elements_descriptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -809,15 +809,14 @@
     "demonstrated that fusion techniques could indeed be used to make new, "
     "heavy nuclei. Made and identified by physicists of the Heavy Ion "
     "Research Laboratory, Darmstadt, West Germany in 1982. Named in honor "
     "of Lise Meitner, the Austrian physicist."
 )
 
 if __name__ == '__main__':
-
     try:
         from .elements import word_wrap
     except ImportError:
         from elements import word_wrap  # type: ignore
 
     for ele in ELEMENTS:
         descr = word_wrap(
```

### Comparing `molmass-2022.12.9/molmass/elements_gui.py` & `molmass-2023.4.10/molmass/elements_gui.py`

 * *Files identical despite different names*

### Comparing `molmass-2022.12.9/molmass/molmass.py` & `molmass-2023.4.10/molmass/molmass.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # molmass.py
 
-# Copyright (c) 1990-2022, Christoph Gohlke
+# Copyright (c) 1990-2023, Christoph Gohlke
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
@@ -40,22 +40,22 @@
 deficiency due to chemical bonding is not taken into account.
 
 The library includes a database of physicochemical and descriptive properties
 of the chemical elements.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2022.12.9
-:DOI: 10.5281/zenodo.7135495
+:Version: 2023.4.10
+:DOI: `10.5281/zenodo.7135495 <https://doi.org/10.5281/zenodo.7135495>`_
 
 Quickstart
 ----------
 
 Install the molmass package and all dependencies from the
-Python Package Index::
+`Python Package Index <https://pypi.org/project/molmass/>`_::
 
     python -m pip install -U molmass[all]
 
 Print the console script usage::
 
     python -m molmass --help
 
@@ -69,25 +69,30 @@
 
 Source code and support are available on
 `GitHub <https://github.com/cgohlke/molmass>`_.
 
 Requirements
 ------------
 
-This release has been tested with the following requirements and dependencies
+This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython 3.8.10, 3.9.13, 3.10.9, 3.11.1 <https://www.python.org>`_
-- `Flask 2.2.2 <https://pypi.org/project/Flask/>`_ (optional)
-- `Pandas 1.5.2 <https://pypi.org/project/pandas/>`_ (optional)
-- `wxPython 4.2.0 <https://pypi.org/project/wxPython/>`_ (optional)
+- `CPython <https://www.python.org>`_ 3.8.10, 3.9.13, 3.10.11, 3.11.3
+- `Flask <https://pypi.org/project/Flask/>`_ 2.2.3 (optional)
+- `Pandas <https://pypi.org/project/pandas/>`_ 1.5.3 (optional)
+- `wxPython <https://pypi.org/project/wxPython/>`_ 4.2.0 (optional)
 
 Revisions
 ---------
 
+2023.4.10
+
+- Support rdkit-style ionic charges (#11, #12).
+- Enable multiplication without addition in from_string.
+
 2022.12.9
 
 - Fix split_charge formula with trailing ]] (#11).
 
 2022.10.18
 
 - Several breaking changes.
@@ -229,15 +234,15 @@
 ...     e.validate()
 ...     e = eval(repr(e))
 
 """
 
 from __future__ import annotations
 
-__version__ = '2022.12.9'
+__version__ = '2023.4.10'
 
 __all__ = [
     'Composition',
     'CompositionItem',
     'Formula',
     'FormulaError',
     'Spectrum',
@@ -291,14 +296,15 @@
 ) -> str:
     """Return analysis of chemical formula as string.
 
     Parameters:
         formula: Chemical formula.
         maxatoms: Number of atoms below which to calculate spectrum.
         min_intensity: Minimum intensity to include in spectrum.
+        debug: If True, raise exceptions, else print error message.
 
     Examples:
         >>> print(analyze('C8H10N4O2', min_intensity=0.01))
         Formula: C8H10N4O2
         Empirical formula: C4H5N2O
         <BLANKLINE>
         Nominal mass: 194
@@ -404,14 +410,17 @@
         Formula('[30Si]3O2')
 
         Ion charges:
 
         >>> Formula('[AsO4]3-')
         Formula('[AsO4]3-')
 
+        >>> Formula('O2-2')
+        Formula('[O2]2-')
+
         Abbreviations of chemical groups:
 
         >>> Formula('EtOH')
         Formula('(C2H5)OH')
 
         Simple arithmetic:
 
@@ -914,15 +923,15 @@
         """Return formula repeated number times.
 
         >>> Formula('HO-') * 2
         Formula('[(HO)2]2-')
 
         """
         if not isinstance(number, int) or number < 1:
-            raise TypeError('can only multipy with positive number')
+            raise TypeError('can only multiply with positive number')
         return Formula(
             join_charge(
                 f'({self._formula_nocharge}){number}', self._charge * number
             )
         )
 
     def __rmul__(self, number: int, /) -> Formula:
@@ -1332,15 +1341,15 @@
         molmass.molmass.FormulaError: unexpected character 'a'
         abc
         ^
 
         >>> Formula('(H2O)2-H2O').formula
         Traceback (most recent call last):
          ...
-        molmass.molmass.FormulaError: unexpected character '-'
+        molmass.molmass.FormulaError: subtraction not allowed
         (H2O)2-H2O
         ......^
 
         >>> Formula('[11C]').formula
         Traceback (most recent call last):
          ...
         molmass.molmass.FormulaError: unknown isotope '11C'
@@ -1402,14 +1411,18 @@
         'O2[30Si]3'
         >>> from_string('PhNH2.HCl')
         '(C6H5)NH2HCl'
         >>> from_string('CuSO4.5H2O')
         'CuSO4(H2O)5'
         >>> from_string('CuSO4+5*H2O')
         'CuSO4(H2O)5'
+        >>> from_string('5*H2O')
+        '(H2O)5'
+        >>> from_string('O2+12C')  # not [12C]O2
+        'O2(C)12'
         >>> from_string('ssdna(AC)')
         '((C10H12N5O5P)(C9H12N3O6P)H2O)'
         >>> from_string('peptide(GG)')
         '((C2H3NO)2H2O)'
 
     """
     try:
@@ -1454,22 +1467,30 @@
     formula = re.sub('(D)(?![a-z])', '[2H]', formula)
 
     # charge
     formula, charge = split_charge(formula)
 
     # arithmetic
     formula = formula.replace('.', '+')
-    if '+' in formula:
+    if '+' in formula or '*' in formula:
+        # TODO: document O2+12C is C12O2, not [12C]O2
         for match in re.findall(
             r'(?:\+|^)((\d+)\*?(.*?))(?:(?=\+)|$)', formula
         ):
             formula = formula.replace(match[0], f'({match[2]}){match[1]}')
+        m = re.search(r'(\+[a-z])', formula)
+        if m:
+            raise FormulaError(
+                'invalid symbol', formula, formula.index(m[0]) + 1
+            )
         formula = formula.replace('+', '')
     if '-' in formula:
-        FormulaError('subtraction not allowed', formula, formula.index('-'))
+        raise FormulaError(
+            'subtraction not allowed', formula, formula.index('-')
+        )
 
     if charge != 0:
         formula = f'[{formula}]{format_charge(charge)}'
     return formula
 
 
 def from_elements(
@@ -1795,24 +1816,32 @@
         Chemical formula without charge, and charge number.
 
     Examples:
         >>> split_charge('Formula')
         ('Formula', 0)
         >>> split_charge('Formula+')
         ('Formula', 1)
+        >>> split_charge('Formula+1')
+        ('Formula', 1)
         >>> split_charge('Formula++')
         ('Formula', 2)
         >>> split_charge('[Formula]2+')
         ('Formula', 2)
+        >>> split_charge('Formula+2')
+        ('Formula', 2)
         >>> split_charge('[[Formula]]2-')
         ('[Formula]', -2)
+        >>> split_charge('[Formula]-2')
+        ('Formula', -2)
         >>> split_charge('[Formula]_2-')
         ('Formula', -2)
         >>> split_charge('Formula_2-')
         ('Formula', -2)
+        >>> split_charge('Formula-2')
+        ('Formula', -2)
         >>> split_charge('Formula_+')
         ('Formula', 1)
         >>> split_charge('Formula+-')
         ('Formula', 0)
         >>> split_charge('Formul+a+')
         ('Formul+a', 1)
 
@@ -1822,30 +1851,38 @@
     if m:
         m_delim, m_count, m_sign = m.groups()
         if m_count == '':
             charge = int(f'{m_sign}1')
         else:
             charge = int(f'{m_sign}{m_count}')
     else:
-        m = re.search(r'([\]_]?)([+-]{1,})$', formula)
-        charge = 0
+        m = re.search(r'([+-]{1})([0-9]{1,})$', formula)
         if m:
-            m_delim, m_sign = m.groups()
-            for char in m_sign:
-                if char == '+':
-                    charge += 1
-                elif char == '-':
-                    charge -= 1
+            m_sign, m_count = m.groups()
+            m_delim = f'{m_sign}{m_count}'
+            charge = int(m_delim)
+        else:
+            m = re.search(r'([\]_]?)([+-]{1,})$', formula)
+            charge = 0
+            if m:
+                m_delim, m_sign = m.groups()
+                for char in m_sign:
+                    if char == '+':
+                        charge += 1
+                    elif char == '-':
+                        charge -= 1
     if m:
         if m_delim == '_':
             formula = formula.rsplit('_', 1)[0]
         elif m_delim == '':
             formula = formula.strip(m_sign)
         elif m_delim == ']':
             formula = formula.rsplit(']', 1)[0] + ']'
+        else:
+            formula = formula.rsplit(m_delim, 1)[0]
         if formula.startswith('[') and formula.endswith(']'):
             formula = formula[1:-1]
     return formula, charge
 
 
 def join_charge(formula: str, charge: int, separator: str = '', /) -> str:
     """Return formula with charge appended.
@@ -1874,15 +1911,15 @@
         if separator:
             formula = f'{formula}{separator}{format_charge(charge, "")}'
         else:
             formula = f'[{formula}]{format_charge(charge, "")}'
     return formula
 
 
-def format_charge(charge: int, prefix='', /) -> str:
+def format_charge(charge: int, prefix: str = '', /) -> str:
     """Return string representation of charge.
 
     Parameters:
         charge: Charge number.
         prefix: Character placed in front of charge in case ``abs(charge)>1``.
 
     Examples:
@@ -2159,14 +2196,15 @@
     for formula, empirical, mass in [
         (''.join(e.symbol for e in ELEMENTS), '', 14693.181589000998),
         ('12C', '[12C]', 12.0),
         ('12CC', 'C[12C]', 24.0107),
         ('SO4_2-', '[O4S]2-', 96.06351715981813),
         ('[CHNOP[13C]]2-', '[C[13C]HNOP]2-', 87.003),
         ('[CHNOP[13C]]_2-', '[C[13C]HNOP]2-', 87.003),
+        ('CHNOP[13C]-2', '[C[13C]HNOP]2-', 87.003),
         ('Co(Bpy)(CO)4', '', 327.16),
         ('CH3CH2Cl', 'C2H5Cl', 64.5147),
         ('C1000H1000', 'CH', 13018.68),
         ('Ru2(CO)8', 'C4O4Ru', 426.2232),
         ('RuClH(CO)(PPh3)3', 'C55H46ClOP3Ru', 952.41392),
         ('PhSiMe3', 'C9H14Si', 150.29566),
         ('Ph(CO)C(CH3)3', 'C11H14O', 162.23156),
@@ -2177,14 +2215,16 @@
         ('CDCl3', 'C[2H]Cl3', 120.384),
         ('[13C]Cl4', '[13C]Cl4', 154.8153),
         ('C5(PhBu(EtCHBr)2)3', 'C53H78Br6', 1194.626),
         ('AgCuRu4(H)2[CO]12{PPh3}2', 'C48H32AgCuO12P2Ru4', 1438.4022),
         ('PhNH2.HCl', 'C6H8ClN', 129.5892),
         ('NH3.BF3', 'BF3H3N', 84.8357),
         ('CuSO4.5H2O', 'CuH10O9S', 249.68),
+        ('5*H2O+CuSO4', 'CuH10O9S', 249.68),
+        ('5*H2O', 'H2O', 90.076435),
         (
             'HCysp(Trt)Tyrp(Tbu)IleGlnp(Trt)Asnp(Trt)ProLeuGlyNH2',
             'C101H113N11O11S',
             1689.13532,
         ),
     ]:
         if verbose:
@@ -2229,14 +2269,16 @@
         '[11C]',
         'H0',
         '()0',
         '(H)0C',
         'Ox: 0.26, 30Si: 0.74',
         'H^++',
         '[CHNOP[13C]]__2-',
+        'O2_-2',
+        'C+a',
     ]:
         if verbose:
             print(f'Trying Formula({formula!r}) ...', end='')
         try:
             empirical = Formula(formula).empirical
         except FormulaError as exc:
             if verbose:
@@ -2260,16 +2302,21 @@
 
     """
     if argv is None:
         argv = sys.argv
 
     import optparse
 
-    def search_doc(r, d):
-        return re.search(r, __doc__).group(1) if __doc__ else d
+    def search_doc(r: str, d: str) -> str:
+        if not __doc__:
+            return d
+        match = re.search(r, __doc__)
+        if match is None:
+            return d
+        return match.group(1)
 
     parser = optparse.OptionParser(
         usage='usage: %prog [options] formula',
         description=search_doc('\n\n([^|]*?)\n\n', ''),
         version='%prog {}'.format(search_doc(':Version: (.*)', 'Unknown')),
         prog='molmass',
     )
```

### Comparing `molmass-2022.12.9/molmass/web.py` & `molmass-2023.4.10/molmass/web.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 # molmass/web.py
 
-# Copyright (c) 2005-2022, Christoph Gohlke
+# Copyright (c) 2005-2023, Christoph Gohlke
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
@@ -512,19 +512,18 @@
 
     if os.getenv('SERVER_NAME'):
         print('Content-type: text/html\n\n')
         request = cgi.FieldStorage()
         request.get = request.getfirst  # type: ignore
         print(response(request, url))
     else:
-
         from urllib.parse import urlparse
         from http.server import HTTPServer, CGIHTTPRequestHandler
 
-        def is_cgi(self):
+        def is_cgi(self) -> bool:
             # monkey patch for CGIHTTPRequestHandler.is_cgi
             if filename in self.path:
                 self.cgi_info = '', self.path[1:]
                 return True
             return False
 
         CGIHTTPRequestHandler.is_cgi = is_cgi  # type: ignore
@@ -574,15 +573,15 @@
     urlp = urlparse(url)
     if urlp.hostname is None or urlp.port is None:
         raise ValueError(f'invalid URL {url!r}')
 
     app = Flask(__name__)
 
     @app.route('/', methods=['GET'])
-    def root():
+    def root() -> str:
         nonlocal form
         r = response(
             request.args if form is None else form, url=request.base_url
         )
         form = None
         return r
```

### Comparing `molmass-2022.12.9/molmass.egg-info/PKG-INFO` & `molmass-2023.4.10/molmass.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molmass
-Version: 2022.12.9
+Version: 2023.4.10
 Summary: Molecular mass calculations
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/molmass/issues
 Project-URL: Source Code, https://github.com/cgohlke/molmass
@@ -36,22 +36,22 @@
 deficiency due to chemical bonding is not taken into account.
 
 The library includes a database of physicochemical and descriptive properties
 of the chemical elements.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2022.12.9
-:DOI: 10.5281/zenodo.7135495
+:Version: 2023.4.10
+:DOI: `10.5281/zenodo.7135495 <https://doi.org/10.5281/zenodo.7135495>`_
 
 Quickstart
 ----------
 
 Install the molmass package and all dependencies from the
-Python Package Index::
+`Python Package Index <https://pypi.org/project/molmass/>`_::
 
     python -m pip install -U molmass[all]
 
 Print the console script usage::
 
     python -m molmass --help
 
@@ -65,25 +65,30 @@
 
 Source code and support are available on
 `GitHub <https://github.com/cgohlke/molmass>`_.
 
 Requirements
 ------------
 
-This release has been tested with the following requirements and dependencies
+This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython 3.8.10, 3.9.13, 3.10.9, 3.11.1 <https://www.python.org>`_
-- `Flask 2.2.2 <https://pypi.org/project/Flask/>`_ (optional)
-- `Pandas 1.5.2 <https://pypi.org/project/pandas/>`_ (optional)
-- `wxPython 4.2.0 <https://pypi.org/project/wxPython/>`_ (optional)
+- `CPython <https://www.python.org>`_ 3.8.10, 3.9.13, 3.10.11, 3.11.3
+- `Flask <https://pypi.org/project/Flask/>`_ 2.2.3 (optional)
+- `Pandas <https://pypi.org/project/pandas/>`_ 1.5.3 (optional)
+- `wxPython <https://pypi.org/project/wxPython/>`_ 4.2.0 (optional)
 
 Revisions
 ---------
 
+2023.4.10
+
+- Support rdkit-style ionic charges (#11, #12).
+- Enable multiplication without addition in from_string.
+
 2022.12.9
 
 - Fix split_charge formula with trailing ]] (#11).
 
 2022.10.18
 
 - Several breaking changes.
```

### Comparing `molmass-2022.12.9/setup.py` & `molmass-2023.4.10/setup.py`

 * *Files identical despite different names*

