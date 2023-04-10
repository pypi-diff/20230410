# Comparing `tmp/manga2pdf-0.0.3.tar.gz` & `tmp/manga2pdf-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manga2pdf-0.0.3.tar", last modified: Thu Apr  6 01:08:55 2023, max compression
+gzip compressed data, was "manga2pdf-0.0.4.tar", last modified: Mon Apr 10 12:18:27 2023, max compression
```

## Comparing `manga2pdf-0.0.3.tar` & `manga2pdf-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 shun       (501) staff       (20)        0 2023-04-06 01:08:55.381782 manga2pdf-0.0.3/
--rw-r--r--   0 shun       (501) staff       (20)     1063 2023-03-12 05:13:58.000000 manga2pdf-0.0.3/LICENSE
--rw-r--r--   0 shun       (501) staff       (20)     5624 2023-04-06 01:08:55.381630 manga2pdf-0.0.3/PKG-INFO
--rw-r--r--   0 shun       (501) staff       (20)     5080 2023-04-01 11:10:27.000000 manga2pdf-0.0.3/README.md
--rw-r--r--   0 shun       (501) staff       (20)       38 2023-04-06 01:08:55.381820 manga2pdf-0.0.3/setup.cfg
--rw-r--r--   0 shun       (501) staff       (20)     1035 2023-04-06 00:39:28.000000 manga2pdf-0.0.3/setup.py
-drwxr-xr-x   0 shun       (501) staff       (20)        0 2023-04-06 01:08:55.380291 manga2pdf-0.0.3/src/
-drwxr-xr-x   0 shun       (501) staff       (20)        0 2023-04-06 01:08:55.381464 manga2pdf-0.0.3/src/manga2pdf.egg-info/
--rw-r--r--   0 shun       (501) staff       (20)     5624 2023-04-06 01:08:55.000000 manga2pdf-0.0.3/src/manga2pdf.egg-info/PKG-INFO
--rw-r--r--   0 shun       (501) staff       (20)      267 2023-04-06 01:08:55.000000 manga2pdf-0.0.3/src/manga2pdf.egg-info/SOURCES.txt
--rw-r--r--   0 shun       (501) staff       (20)        1 2023-04-06 01:08:55.000000 manga2pdf-0.0.3/src/manga2pdf.egg-info/dependency_links.txt
--rw-r--r--   0 shun       (501) staff       (20)       45 2023-04-06 01:08:55.000000 manga2pdf-0.0.3/src/manga2pdf.egg-info/entry_points.txt
--rw-r--r--   0 shun       (501) staff       (20)       46 2023-04-06 01:08:55.000000 manga2pdf-0.0.3/src/manga2pdf.egg-info/requires.txt
--rw-r--r--   0 shun       (501) staff       (20)       10 2023-04-06 01:08:55.000000 manga2pdf-0.0.3/src/manga2pdf.egg-info/top_level.txt
--rw-r--r--   0 shun       (501) staff       (20)    17304 2023-04-06 00:39:01.000000 manga2pdf-0.0.3/src/manga2pdf.py
+drwxr-xr-x   0 shun       (501) staff       (20)        0 2023-04-10 12:18:27.381574 manga2pdf-0.0.4/
+-rw-r--r--   0 shun       (501) staff       (20)     1063 2023-03-12 05:13:58.000000 manga2pdf-0.0.4/LICENSE
+-rw-r--r--   0 shun       (501) staff       (20)     5624 2023-04-10 12:18:27.381455 manga2pdf-0.0.4/PKG-INFO
+-rw-r--r--   0 shun       (501) staff       (20)     5080 2023-04-01 11:10:27.000000 manga2pdf-0.0.4/README.md
+-rw-r--r--   0 shun       (501) staff       (20)       38 2023-04-10 12:18:27.381604 manga2pdf-0.0.4/setup.cfg
+-rw-r--r--   0 shun       (501) staff       (20)     1035 2023-04-10 10:22:02.000000 manga2pdf-0.0.4/setup.py
+drwxr-xr-x   0 shun       (501) staff       (20)        0 2023-04-10 12:18:27.380649 manga2pdf-0.0.4/src/
+drwxr-xr-x   0 shun       (501) staff       (20)        0 2023-04-10 12:18:27.381298 manga2pdf-0.0.4/src/manga2pdf.egg-info/
+-rw-r--r--   0 shun       (501) staff       (20)     5624 2023-04-10 12:18:27.000000 manga2pdf-0.0.4/src/manga2pdf.egg-info/PKG-INFO
+-rw-r--r--   0 shun       (501) staff       (20)      267 2023-04-10 12:18:27.000000 manga2pdf-0.0.4/src/manga2pdf.egg-info/SOURCES.txt
+-rw-r--r--   0 shun       (501) staff       (20)        1 2023-04-10 12:18:27.000000 manga2pdf-0.0.4/src/manga2pdf.egg-info/dependency_links.txt
+-rw-r--r--   0 shun       (501) staff       (20)       45 2023-04-10 12:18:27.000000 manga2pdf-0.0.4/src/manga2pdf.egg-info/entry_points.txt
+-rw-r--r--   0 shun       (501) staff       (20)       46 2023-04-10 12:18:27.000000 manga2pdf-0.0.4/src/manga2pdf.egg-info/requires.txt
+-rw-r--r--   0 shun       (501) staff       (20)       10 2023-04-10 12:18:27.000000 manga2pdf-0.0.4/src/manga2pdf.egg-info/top_level.txt
+-rw-r--r--   0 shun       (501) staff       (20)    17429 2023-04-10 10:18:41.000000 manga2pdf-0.0.4/src/manga2pdf.py
```

### Comparing `manga2pdf-0.0.3/LICENSE` & `manga2pdf-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `manga2pdf-0.0.3/PKG-INFO` & `manga2pdf-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manga2pdf
-Version: 0.0.3
+Version: 0.0.4
 Summary: Convert manga/comic files(zip, epub, etc.) or directory containing image files (jpg, png, etc.) to PDF.
 Home-page: https://github.com/mashu3/manga2pdf
 Author: mashu3
 License: MIT
 Keywords: manga comic pdf converter
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `manga2pdf-0.0.3/README.md` & `manga2pdf-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `manga2pdf-0.0.3/setup.py` & `manga2pdf-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.3"
+VERSION = "0.0.4"
 
 INSTALL_REQUIRES = (
     "img2pdf",
     "Pillow",
     "pikepdf",
     "rarfile",
     "beautifulsoup4"
```

### Comparing `manga2pdf-0.0.3/src/manga2pdf.egg-info/PKG-INFO` & `manga2pdf-0.0.4/src/manga2pdf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manga2pdf
-Version: 0.0.3
+Version: 0.0.4
 Summary: Convert manga/comic files(zip, epub, etc.) or directory containing image files (jpg, png, etc.) to PDF.
 Home-page: https://github.com/mashu3/manga2pdf
 Author: mashu3
 License: MIT
 Keywords: manga comic pdf converter
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `manga2pdf-0.0.3/src/manga2pdf.py` & `manga2pdf-0.0.4/src/manga2pdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,15 +194,15 @@
                     img_tags = xhtml_soup.find_all('img')
                 for img_tag in img_tags:
                     try:
                         img_link = img_tag['xlink:href']
                     except KeyError:
                         img_link = img_tag['src']
                     image_href = os.path.abspath(os.path.join(os.path.dirname(nav_text), img_link))
-                    image_href = os.path.relpath(image_href, os.getcwd())
+                    image_href = os.path.relpath(image_href, os.getcwd()).replace(os.sep, '/')
                     index_number = page_names.index(image_href)
                     page_index.append([nav_label, index_number])
             else:
                 index_number = page_names.index(nav_text)
                 page_index.append([nav_label, index_number])
         return page_index
     
@@ -288,20 +288,22 @@
                     pdf.Root.ViewerPreferences = pikepdf.Dictionary()
                 if not hasattr(pdf.Root.ViewerPreferences, 'Direction') \
                     or pdf.Root.ViewerPreferences.Direction != '/' + self.direction:
                         pdf.Root.ViewerPreferences.Direction = pikepdf.Name('/' + self.direction)
             if self.output_path is None:
                 if os.path.isdir(self.input_path):
                     pdf_filename = os.path.basename(self.input_path) + '.pdf'
-                    output_path = os.path.join(self.input_path, pdf_filename)
+                    output_path = os.path.join(self.input_path, pdf_filename).replace(os.sep, '/')
                 else:
                     pdf_filename, _ = os.path.splitext(self.input_path)
                     output_path = f"{pdf_filename}.pdf"
             else:
                 output_path = self.output_path
+            if os.path.exists(output_path):
+                os.remove(output_path)
             pdf.save(output_path, linearize=True)
         return None
 
 class HelpFormatter(argparse.HelpFormatter):
     def __init__(self, prog, indent_increment=2, max_help_position=6, width=None):
         super().__init__(prog, indent_increment, max_help_position, width)
     def _split_lines(self, text, _):
```

