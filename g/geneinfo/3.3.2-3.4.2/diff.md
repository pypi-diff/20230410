# Comparing `tmp/geneinfo-3.3.2.tar.gz` & `tmp/geneinfo-3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geneinfo-3.3.2.tar", last modified: Tue Apr  4 10:08:12 2023, max compression
+gzip compressed data, was "geneinfo-3.4.2.tar", last modified: Mon Apr 10 18:15:11 2023, max compression
```

## Comparing `geneinfo-3.3.2.tar` & `geneinfo-3.4.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwsr-x   0 kmt       (6358) xy-drive (50749)        0 2023-04-04 10:08:12.000000 geneinfo-3.3.2/
--rw-rw-r--   0 kmt       (6358) xy-drive (50749)     1069 2023-03-29 19:39:27.000000 geneinfo-3.3.2/LICENSE
--rw-rw-r--   0 kmt       (6358) xy-drive (50749)      491 2023-04-04 10:08:12.000000 geneinfo-3.3.2/PKG-INFO
--rw-rw-r--   0 kmt       (6358) xy-drive (50749)      174 2023-03-29 19:39:27.000000 geneinfo-3.3.2/README.md
-drwxrwsr-x   0 kmt       (6358) xy-drive (50749)        0 2023-04-04 10:08:12.000000 geneinfo-3.3.2/geneinfo/
--rw-rw-r--   0 kmt       (6358) xy-drive (50749)    52120 2023-04-04 10:00:38.000000 geneinfo-3.3.2/geneinfo/__init__.py
--rw-rw-r--   0 kmt       (6358) xy-drive (50749)     3385 2023-03-29 19:39:28.000000 geneinfo-3.3.2/geneinfo/intervals.py
-drwxrwsr-x   0 kmt       (6358) xy-drive (50749)        0 2023-04-04 10:08:12.000000 geneinfo-3.3.2/geneinfo.egg-info/
--rw-rw-r--   0 kmt       (6358) xy-drive (50749)      491 2023-04-04 10:08:11.000000 geneinfo-3.3.2/geneinfo.egg-info/PKG-INFO
--rw-rw-r--   0 kmt       (6358) xy-drive (50749)      228 2023-04-04 10:08:11.000000 geneinfo-3.3.2/geneinfo.egg-info/SOURCES.txt
--rw-rw-r--   0 kmt       (6358) xy-drive (50749)        1 2023-04-04 10:08:11.000000 geneinfo-3.3.2/geneinfo.egg-info/dependency_links.txt
--rw-rw-r--   0 kmt       (6358) xy-drive (50749)       68 2023-04-04 10:08:11.000000 geneinfo-3.3.2/geneinfo.egg-info/requires.txt
--rw-rw-r--   0 kmt       (6358) xy-drive (50749)        9 2023-04-04 10:08:11.000000 geneinfo-3.3.2/geneinfo.egg-info/top_level.txt
--rw-rw-r--   0 kmt       (6358) xy-drive (50749)       38 2023-04-04 10:08:12.000000 geneinfo-3.3.2/setup.cfg
--rw-rw-r--   0 kmt       (6358) xy-drive (50749)      862 2023-04-04 10:07:10.000000 geneinfo-3.3.2/setup.py
+drwxrwxr-x   0 kmt       (6358) kmt       (6358)        0 2023-04-10 18:15:11.124297 geneinfo-3.4.2/
+-rw-rw-r--   0 kmt       (6358) kmt       (6358)     1069 2023-04-10 18:12:55.000000 geneinfo-3.4.2/LICENSE
+-rw-rw-r--   0 kmt       (6358) kmt       (6358)      491 2023-04-10 18:15:11.113297 geneinfo-3.4.2/PKG-INFO
+-rw-rw-r--   0 kmt       (6358) kmt       (6358)      174 2023-04-10 18:12:55.000000 geneinfo-3.4.2/README.md
+drwxrwxr-x   0 kmt       (6358) kmt       (6358)        0 2023-04-10 18:15:10.529286 geneinfo-3.4.2/geneinfo/
+-rw-rw-r--   0 kmt       (6358) kmt       (6358)    52344 2023-04-10 18:13:17.000000 geneinfo-3.4.2/geneinfo/__init__.py
+-rw-rw-r--   0 kmt       (6358) kmt       (6358)     3385 2023-04-10 18:12:56.000000 geneinfo-3.4.2/geneinfo/intervals.py
+drwxrwxr-x   0 kmt       (6358) kmt       (6358)        0 2023-04-10 18:15:11.019295 geneinfo-3.4.2/geneinfo.egg-info/
+-rw-rw-r--   0 kmt       (6358) kmt       (6358)      491 2023-04-10 18:15:09.000000 geneinfo-3.4.2/geneinfo.egg-info/PKG-INFO
+-rw-rw-r--   0 kmt       (6358) kmt       (6358)      228 2023-04-10 18:15:10.000000 geneinfo-3.4.2/geneinfo.egg-info/SOURCES.txt
+-rw-rw-r--   0 kmt       (6358) kmt       (6358)        1 2023-04-10 18:15:09.000000 geneinfo-3.4.2/geneinfo.egg-info/dependency_links.txt
+-rw-rw-r--   0 kmt       (6358) kmt       (6358)       68 2023-04-10 18:15:09.000000 geneinfo-3.4.2/geneinfo.egg-info/requires.txt
+-rw-rw-r--   0 kmt       (6358) kmt       (6358)        9 2023-04-10 18:15:09.000000 geneinfo-3.4.2/geneinfo.egg-info/top_level.txt
+-rw-rw-r--   0 kmt       (6358) kmt       (6358)       38 2023-04-10 18:15:11.147297 geneinfo-3.4.2/setup.cfg
+-rw-rw-r--   0 kmt       (6358) kmt       (6358)      862 2023-04-10 18:13:45.000000 geneinfo-3.4.2/setup.py
```

### Comparing `geneinfo-3.3.2/LICENSE` & `geneinfo-3.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `geneinfo-3.3.2/geneinfo/__init__.py` & `geneinfo-3.4.2/geneinfo/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -279,21 +279,21 @@
     else:
         ax.text(txstart, offset-.5, name, horizontalalignment='right', verticalalignment='center', 
             fontsize=font_size, color=color, clip_on=clip_on)
 
 
 def gene_plot(chrom, start, end, assembly, highlight=[], db='ncbiRefSeq', 
                 collapse_splice_var=True, hard_limits=False, exact_exons=False, 
-                figsize=None, aspect=1, despine=False, clip_on=True):
+                figsize=None, aspect=1, despine=False, clip_on=True, gene_density=60, font_size=None, return_axes=1):
     
     global CACHE
 
-    fig, (ax1, ax2) = plt.subplots(2, 1, figsize=figsize, sharex='col', 
-                                    sharey='row', gridspec_kw={'height_ratios': [1, aspect]})
-    plt.subplots_adjust(wspace=0, hspace=0.05)
+    fig, axes = plt.subplots(return_axes+1, 1, figsize=figsize, sharex='col', 
+                                    sharey='row', gridspec_kw={'height_ratios': [1/return_axes]*return_axes + [aspect]})
+    plt.subplots_adjust(wspace=0, hspace=0.15)
 
     if (chrom, start, end, assembly) in CACHE:
         genes = CACHE[(chrom, start, end, assembly)]
     else:
         genes = list(get_genes_region(chrom, start, end, assembly, db))
         CACHE[(chrom, start, end, assembly)] = genes
 
@@ -304,16 +304,17 @@
                 d[name] = [name, txstart, txend, strand, set(exons)]
             else:
                 d[name][-1].update(exons)
         genes = d.values()
 
 
     line_width = max(6, int(50 / log10(end - start)))-2
-    font_size = max(6, int(50 / log10(end - start)))
-    label_width = font_size * (end - start) / 60
+    if font_size is None:
+        font_size = max(6, int(50 / log10(end - start)))
+    label_width = font_size * (end - start) / gene_density
     if exact_exons:
         min_visible_exon_width = 0
     else:
         min_visible_exon_width = (end - start) / 1000
         
     plotted_intervals = defaultdict(list)
     for name, txstart, txend, strand, exons in genes:
@@ -340,41 +341,42 @@
             hl = highlight[name]
         else:
             hl = None
 
         _plot_gene(name, txstart, txend, strand, exons, 
                   offset, line_width, min_visible_exon_width, font_size, 
                   highlight=hl,
-                  ax=ax2, clip_on=clip_on)
+                  ax=axes[-1], clip_on=clip_on)
 
     if plotted_intervals:
         offset = max(plotted_intervals.keys())
     else:
         offset = 1
 
     if hard_limits:
-        ax2.set_xlim(start, end)
+        axex[-1].set_xlim(start, end)
     else:
-        s, e = ax2.get_xlim()
-        ax2.set_xlim(min(s-label_width/2, start), max(e, end))
+        s, e = axes[-1].get_xlim()
+        axes[-1].set_xlim(min(s-label_width/2, start), max(e, end))
 
-    ax2.set_ylim(-2, offset+2)
-    ax2.get_yaxis().set_visible(False)
-    ax2.invert_yaxis()
-    ax2.spines['top'].set_visible(False)
-    ax2.spines['right'].set_visible(False)
-    ax2.spines['left'].set_visible(False)
-
-    ax1.set_xlim(ax2.get_xlim())
-
-    if despine:
-        ax1.spines['top'].set_visible(False)
-        ax1.spines['right'].set_visible(False)
-
-    return ax1
+    axes[-1].set_ylim(-2, offset+2)
+    axes[-1].get_yaxis().set_visible(False)
+    axes[-1].invert_yaxis()
+    axes[-1].spines['top'].set_visible(False)
+    axes[-1].spines['right'].set_visible(False)
+    axes[-1].spines['left'].set_visible(False)
+
+    for ax in axes[:-1]:
+        ax.set_xlim(axes[-1].get_xlim())
+
+        if despine:
+            ax.spines['top'].set_visible(False)
+            ax.spines['right'].set_visible(False)
+    
+    return axes[:-1]
 
 
 ##################################################################################
 # Map between assembly coordinates
 ##################################################################################
 
 def map_interval(chrom, start, end, strand, map_from, map_to, species='homo_sapiens'):
```

### Comparing `geneinfo-3.3.2/geneinfo/intervals.py` & `geneinfo-3.4.2/geneinfo/intervals.py`

 * *Files identical despite different names*

### Comparing `geneinfo-3.3.2/setup.py` & `geneinfo-3.4.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="geneinfo",
-    version="3.3.2",
+    version="3.4.2",
     author="Kasper Munch",
     author_email="kaspermunch@birc.au.dk",
     description="Functions for showing gene information in jupyter notebooks.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kaspermunch/geneinfo",
     packages=setuptools.find_packages(),
```

