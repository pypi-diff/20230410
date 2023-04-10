# Comparing `tmp/LRphase-1.1.0.tar.gz` & `tmp/LRphase-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LRphase-1.1.0.tar", last modified: Fri Dec 16 20:04:02 2022, max compression
+gzip compressed data, was "LRphase-1.1.1.tar", last modified: Mon Apr 10 20:03:28 2023, max compression
```

## Comparing `LRphase-1.1.0.tar` & `LRphase-1.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 adadiehl (201766) boyle-lab (2294145)        0 2022-12-16 20:04:02.363971 LRphase-1.1.0/
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)     1071 2022-12-13 14:14:17.000000 LRphase-1.1.0/LICENSE
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)     2031 2022-12-13 14:13:07.000000 LRphase-1.1.0/MANIFEST.in
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)     8101 2022-12-16 20:04:02.363971 LRphase-1.1.0/PKG-INFO
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)     5933 2022-12-16 20:01:09.000000 LRphase-1.1.0/README.md
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)       91 2022-12-13 14:13:07.000000 LRphase-1.1.0/pyproject.toml
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)      338 2022-12-16 20:04:02.367971 LRphase-1.1.0/setup.cfg
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)     3304 2022-12-16 20:04:01.000000 LRphase-1.1.0/setup.py
-drwxr-xr-x   0 adadiehl (201766) boyle-lab (2294145)        0 2022-12-16 20:04:02.359971 LRphase-1.1.0/src/
-drwxr-xr-x   0 adadiehl (201766) boyle-lab (2294145)        0 2022-12-16 20:04:02.363971 LRphase-1.1.0/src/LRphase/
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)    21497 2022-12-13 14:13:07.000000 LRphase-1.1.0/src/LRphase/HeterozygousSites.py
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)    57539 2022-12-15 19:50:52.000000 LRphase-1.1.0/src/LRphase/InputData.py
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)    14568 2022-12-15 19:29:13.000000 LRphase-1.1.0/src/LRphase/PhasableSample.py
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)    38006 2022-12-16 19:47:16.000000 LRphase-1.1.0/src/LRphase/PhaseSet.py
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)    48344 2022-12-13 14:13:07.000000 LRphase-1.1.0/src/LRphase/PhasedRead.py
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)    23153 2022-12-13 14:13:07.000000 LRphase-1.1.0/src/LRphase/SimulatePhasedData.py
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)      202 2022-12-16 20:04:01.000000 LRphase-1.1.0/src/LRphase/__init__.py
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)      364 2022-12-13 14:13:07.000000 LRphase-1.1.0/src/LRphase/__main__.py
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)    64502 2022-12-16 20:04:01.000000 LRphase-1.1.0/src/LRphase/cli.py
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)     4391 2022-12-13 14:13:07.000000 LRphase-1.1.0/src/LRphase/urls.py
-drwxr-xr-x   0 adadiehl (201766) boyle-lab (2294145)        0 2022-12-16 20:04:02.363971 LRphase-1.1.0/src/LRphase.egg-info/
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)     8101 2022-12-16 20:04:02.000000 LRphase-1.1.0/src/LRphase.egg-info/PKG-INFO
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)      608 2022-12-16 20:04:02.000000 LRphase-1.1.0/src/LRphase.egg-info/SOURCES.txt
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)        1 2022-12-16 20:04:02.000000 LRphase-1.1.0/src/LRphase.egg-info/dependency_links.txt
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)       46 2022-12-16 20:04:02.000000 LRphase-1.1.0/src/LRphase.egg-info/entry_points.txt
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)        1 2022-12-16 20:01:48.000000 LRphase-1.1.0/src/LRphase.egg-info/not-zip-safe
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)      109 2022-12-16 20:04:02.000000 LRphase-1.1.0/src/LRphase.egg-info/requires.txt
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)      117 2022-12-16 20:04:02.000000 LRphase-1.1.0/src/LRphase.egg-info/top_level.txt
-drwxr-xr-x   0 adadiehl (201766) boyle-lab (2294145)        0 2022-12-16 20:04:02.363971 LRphase-1.1.0/tests/
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)        0 2022-12-13 14:13:07.000000 LRphase-1.1.0/tests/__init__.py
--rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)      163 2022-12-13 14:13:07.000000 LRphase-1.1.0/tests/test_LRphase.py
+drwxr-xr-x   0 adadiehl (201766) boyle-lab (2294145)        0 2023-04-10 20:03:28.442864 LRphase-1.1.1/
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)     1071 2022-12-13 14:14:17.000000 LRphase-1.1.1/LICENSE
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)     2031 2022-12-13 14:13:07.000000 LRphase-1.1.1/MANIFEST.in
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)     8101 2023-04-10 20:03:28.442864 LRphase-1.1.1/PKG-INFO
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)     5933 2023-03-07 19:40:55.000000 LRphase-1.1.1/README.md
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)       91 2022-12-13 14:13:07.000000 LRphase-1.1.1/pyproject.toml
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)      338 2023-04-10 20:03:28.442864 LRphase-1.1.1/setup.cfg
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)     3304 2023-04-10 20:03:27.000000 LRphase-1.1.1/setup.py
+drwxr-xr-x   0 adadiehl (201766) boyle-lab (2294145)        0 2023-04-10 20:03:28.438864 LRphase-1.1.1/src/
+drwxr-xr-x   0 adadiehl (201766) boyle-lab (2294145)        0 2023-04-10 20:03:28.442864 LRphase-1.1.1/src/LRphase/
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)    21497 2022-12-13 14:13:07.000000 LRphase-1.1.1/src/LRphase/HeterozygousSites.py
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)    57539 2023-03-10 18:22:15.000000 LRphase-1.1.1/src/LRphase/InputData.py
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)    14614 2023-04-05 16:27:32.000000 LRphase-1.1.1/src/LRphase/PhasableSample.py
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)    38006 2023-03-07 19:40:55.000000 LRphase-1.1.1/src/LRphase/PhaseSet.py
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)    48416 2023-03-07 19:40:55.000000 LRphase-1.1.1/src/LRphase/PhasedRead.py
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)    23245 2023-04-05 16:41:44.000000 LRphase-1.1.1/src/LRphase/SimulatePhasedData.py
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)      202 2023-04-10 20:03:27.000000 LRphase-1.1.1/src/LRphase/__init__.py
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)      364 2022-12-13 14:13:07.000000 LRphase-1.1.1/src/LRphase/__main__.py
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)    64753 2023-04-10 20:03:27.000000 LRphase-1.1.1/src/LRphase/cli.py
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)     4391 2022-12-13 14:13:07.000000 LRphase-1.1.1/src/LRphase/urls.py
+drwxr-xr-x   0 adadiehl (201766) boyle-lab (2294145)        0 2023-04-10 20:03:28.442864 LRphase-1.1.1/src/LRphase.egg-info/
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)     8101 2023-04-10 20:03:28.000000 LRphase-1.1.1/src/LRphase.egg-info/PKG-INFO
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)      608 2023-04-10 20:03:28.000000 LRphase-1.1.1/src/LRphase.egg-info/SOURCES.txt
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)        1 2023-04-10 20:03:28.000000 LRphase-1.1.1/src/LRphase.egg-info/dependency_links.txt
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)       46 2023-04-10 20:03:28.000000 LRphase-1.1.1/src/LRphase.egg-info/entry_points.txt
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)        1 2022-12-16 20:01:48.000000 LRphase-1.1.1/src/LRphase.egg-info/not-zip-safe
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)      109 2023-04-10 20:03:28.000000 LRphase-1.1.1/src/LRphase.egg-info/requires.txt
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)      117 2023-04-10 20:03:28.000000 LRphase-1.1.1/src/LRphase.egg-info/top_level.txt
+drwxr-xr-x   0 adadiehl (201766) boyle-lab (2294145)        0 2023-04-10 20:03:28.442864 LRphase-1.1.1/tests/
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)        0 2022-12-13 14:13:07.000000 LRphase-1.1.1/tests/__init__.py
+-rw-r--r--   0 adadiehl (201766) boyle-lab (2294145)      163 2022-12-13 14:13:07.000000 LRphase-1.1.1/tests/test_LRphase.py
```

### Comparing `LRphase-1.1.0/LICENSE` & `LRphase-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `LRphase-1.1.0/MANIFEST.in` & `LRphase-1.1.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `LRphase-1.1.0/PKG-INFO` & `LRphase-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LRphase
-Version: 1.1.0
+Version: 1.1.1
 Summary: Phasing individual long reads using known haplotype information.
 Home-page: https://github.com/Boyle-Lab/LRphase.git
 Author: Greg Farnum
 Author-email: gregfar@umich.edu
 License: MIT
 Project-URL: Issue Tracker, https://github.com/Boyle-Lab/LRphase/issues
 Description: # LRphase
```

### Comparing `LRphase-1.1.0/README.md` & `LRphase-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `LRphase-1.1.0/setup.py` & `LRphase-1.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             return md.read()
 
 
 def main():
 
     metadata = dict(
         name = 'LRphase',
-        version = '1.1.0',
+        version = '1.1.1',
         license = 'MIT',
         description = 'Phasing individual long reads using known haplotype information.',
         description_content_type = 'text/plain',
         long_description = readme(),
         long_description_content_type = 'text/markdown',
         author = 'Greg Farnum',
         author_email = 'gregfar@umich.edu',
```

### Comparing `LRphase-1.1.0/src/LRphase/HeterozygousSites.py` & `LRphase-1.1.1/src/LRphase/HeterozygousSites.py`

 * *Files identical despite different names*

### Comparing `LRphase-1.1.0/src/LRphase/InputData.py` & `LRphase-1.1.1/src/LRphase/InputData.py`

 * *Files identical despite different names*

### Comparing `LRphase-1.1.0/src/LRphase/PhasableSample.py` & `LRphase-1.1.1/src/LRphase/PhasableSample.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import time
 from typing import Any, Iterator
 import sys, os
 import pysam
 from LRphase import SimulatePhasedData
 import pyliftover
 
-
 class PhasableSample:
     """
 
     """
     #RG_ID_dict: object 
     
     def __init__(
@@ -40,33 +39,34 @@
         self.vcf_file_path = vcf_file_path
         self.ignore_phase_sets = ignore_phase_sets
         
         self.alignment_file_paths = []
         self.RG_ID_dict = RG_ID_dict
         self.use_RG_tag = {}
         
-        #sys.stderr.write("%s\n" %(alignment_file_paths))        
         for alignment_file_path in alignment_file_paths:
             self.alignment_file_paths.append(str(alignment_file_path))
             self.use_RG_tag[str(alignment_file_path)] = alignment_file_paths[str(alignment_file_path)]
 
         if bam_header:
             self.bam_header = bam_header
         else:
-            # Take the header from an alignment file.
+            # Take the header from an alignment file, if possible.
             success = False
             for i in range(len(self.alignment_file_paths)):
+                #sys.stderr.write("%s\n" % (pysam.AlignmentFile(self.alignment_file_paths[i], 'rb').header))
                 try:
                     self.bam_header = pysam.AlignmentFile(self.alignment_file_paths[i], 'rb').header
                 except:
                     continue
                 success = True
                 break
             if not success:
-                raise Exception("ERROR: None of the bam files contain a header and none given. Exiting!")
+                # Use an empty header.
+                self.bam_header = { 'HD': {'VN': '1.0'} }
 
         self.reference_sequence_names = reference_sequence_names
         self.reference_sequence_paths = reference_sequence_paths
         self.reference_sequences_in_VCF = list(self.vcf_file.index)
         self.only_autosomal = only_autosomal
         self.regions = regions
         self.ploidy = ploidy
```

### Comparing `LRphase-1.1.0/src/LRphase/PhaseSet.py` & `LRphase-1.1.1/src/LRphase/PhaseSet.py`

 * *Files identical despite different names*

### Comparing `LRphase-1.1.0/src/LRphase/PhasedRead.py` & `LRphase-1.1.1/src/LRphase/PhasedRead.py`

 * *Files 0% similar despite different names*

```diff
@@ -841,25 +841,26 @@
         elif self.PhaseSet_max.phase == 'Nonphasable':
             return 'Nonphasable'
         else:
             return self.PhaseSet_max.phase_set
     
     @property
     def phasing_error_rate(self):
-        if self.phase == 'Nonphasable':
+        if self.phase in ['Nonphasable', 'nonphasable']:
             return 0.50
         if self.log_likelihood_ratio > 0:
             p = self.powlaw_modified(self.log_likelihood_ratio,
                                      a = self.powlaw_alpha,
                                      xmin = self.powlaw_xmin)
             pl = 1 - (1 / float(self.ploidy_phase_set))
             if p <= pl:
                 return p
             else:
                 return pl
+        return 0.5 # Default is to assume random guess
     
     def powlaw_modified(self, x, a = 4.5, xmin = 2):
         return ((a - 1) / xmin) * math.pow(x / xmin, -1 * a)
     
     @property
     def log_likelihood_ratio(self):
         '''
```

### Comparing `LRphase-1.1.0/src/LRphase/SimulatePhasedData.py` & `LRphase-1.1.1/src/LRphase/SimulatePhasedData.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 def simulate_reads_pbsim2(
         reference_sequence: str, path_to_pbsim: str = 'pbsim', depth: int = 1,
         simulation_mode: str = 'pbsim2/data/R103.model',
         difference_ratio: str = '23:31:46', length_mean: int = 20000,
         length_max: int = 1000000, length_min: int = 100,
         length_sd: int = 15000, accuracy_min: float = 0.01,
-        accuracy_max: float = 1.00, accuracy_mean: float = 0.80,
+        accuracy_max: float = 1.00, accuracy_mean: float = 0.98,
         prefix: str = None, id_prefix: str = 'S', output_directory: str = None, sample: str = None,
         haplotype: int = None, quiet = False, silent = False, no_sim = False
         ) -> str:
     """
     Args:
         reference_sequence (str):
             reference sequence template to simulate reads from
@@ -102,14 +102,16 @@
                    f'--accuracy-mean', str(accuracy_mean),
                    f'--accuracy-min', str(accuracy_min),
                    '--accuracy-max', str(accuracy_max),
                    f'--prefix', str(prefix),
                    '--id-prefix', str(id_prefix),
                    str(reference_genome_path)]
 
+    sys.stderr.write("pbsim2 command: %s\n" % (' ' .join(pbsim2_args)))
+    
     if silent:
         subprocess.run(pbsim2_args, check = True, stdout = subprocess.DEVNULL, stderr = subprocess.DEVNULL)
     elif quiet:
         subprocess.run(pbsim2_args, check = True, stdout = subprocess.DEVNULL)
     else:
         subprocess.run(pbsim2_args, check = True)
 
@@ -168,15 +170,15 @@
         for rec in maf_file:
             line = rec.strip('\n').split()
             if len(line) == 0:
                 continue
             elif state == 0 and line[0] == 'a':
                 state = 1
             elif state == 1 and line[0] == 's':
-                reg = [line[2], line[2]+line[3]]
+                reg = [line[2], str(int(line[2])+int(line[3]))]
                 state = 2
             elif state == 2 and line[0] == 's':
                 m = re.match('^S\d+_\d+', line[1])
                 if not m:
                     sys.stderr.write("Failed to parse read name from record: %s. Skipping...\n" % " ".join(line[0:5]))
                     state = 0
                     continue
```

### Comparing `LRphase-1.1.0/src/LRphase/cli.py` & `LRphase-1.1.1/src/LRphase/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from pysam import AlignmentFile, VariantFile
 import numpy as np
 from scipy.stats import nbinom
 import powerlaw
 import time
 from LRphase.PhaseSet import powlaw_modified, _estimate_prior_probabilities
 
-__version__ = "1.1.0"
+__version__ = "1.1.1"
 
 # TO-DO:
 ## The main phasing function should be a wrapper that loops over samples
 # in the input VCF. Content of the current function should be moved out
 # and called once per sample in the VCF, unless args.one_sample is given.
 #@profile
 def phasing(args):
@@ -140,26 +140,28 @@
 
 
 def trim_phased_reads_to_fdr_neg_binom(phased_reads_list, FDR_threshold, output_streams, args):
     """
     Given a list of phased reads, control FDR at the given level
     by calculating the expected number of phasing errors based on
     a negative binomial model. Phasing decisions can be considered 
-    Bernoulli trials with Psuccess = 1-(𝜀/2). Thus, the error 
+    Bernoulli trials with Psuccess = 1-(𝜀/3). Thus, the error 
     distribution may be modeled as negative binomial with N = the 
     number of phaseable reads. To control the error rate at any 
     given FDR, we use the mean of this distribution, N𝜀, as the 
     expected number of phasing errors, and reassign the N𝜀* (1-FDR)
     lowest-scoring reads as “unphased.”
     """
-    p = 1 - (get_average_seq_error_rate(phased_reads_list) / 2)
+    r = get_average_seq_error_rate(phased_reads_list)
+    p = 1 - (r / 3)
     n = len(phased_reads_list)
     E = get_expected_error_count_neg_binom(n, p)
     e = round(E * (1-FDR_threshold))
     #sys.stderr.write('p: %.5f, n: %d, E: %d, e: %d, FDR: %.5f\n' % (p, n, E, e, FDR_threshold))
+    sys.stderr.write('Negative-binomial error distribution params:\nAvg. Seq. Error Rate: %.5f, Neg. Binom. p: %.5f, phased read count: %d, estimated error count: %d, FDR: %.5f\n' % (r, p, n, e, FDR_threshold))
     sorted_reads_list = sort_reads_list(phased_reads_list)
     sys.stderr.write('Reassigning %d phased reads with the lowest log-likelihood ratios as Unphased to control FDR at %.2f...\n' % (e, FDR_threshold)) 
     for i, phased_read in enumerate(sorted_reads_list):
         if i < e:
             # Relabel the first e observations as Unphased.
             phased_read.PhaseSet_max.phase = 'Unphased'
             phased_read.aligned_segment.set_tag(tag = 'HP', value = "Unphased", value_type='Z', replace=True)
@@ -933,29 +935,32 @@
         help=argparse.SUPPRESS,
         dest = 'error_model',
         type = int
     )
 
     # Options related to the powerlaw error rate approximation are hidden with
     # defaults set to disable filtering of results based on powerlaw error rate
-    # estimates. -E 1 stipulates that no predictions will be tossed out based on
+    # estimates. -E 1.0 stipulates that no predictions will be tossed out based on
     # empirical error rates, which should not exceed 0.5.
     phasing_parser_stats_error.add_argument(
         '-E', '--error_rate_threshold',
         type = float,
         required = False,
         #default = 0.01,
-        default = 1,
+        default = 1.0,
         #help = 'Error rate threshold on phasing results. This threshold equates to the estimated phasing error rate for an experiment, such that a threshold of 0.05 should be equivalent to a 5%% false-discovery rate. This rate is estimated based on a fitted power-law distribution with alpha and xmin parameters supplied with the --powlaw_alpha and --powlaw_xmin options. These parameters may be estimated by running the LRphase error_analysis mode.',
         help=argparse.SUPPRESS,
         dest = 'error_rate_threshold', metavar = '<MAX_ERROR_RATE>'
     )
 
     phasing_parser_stats_error.add_argument(
-        '--log_likelihood_threshold', type = float, required = False, default = -1,
+        '--log_likelihood_threshold',
+        type = float,
+        required = False,
+        default = -1.0,
         help = 'Use a hard threshold on log-likelihood ratios when phasing reads. Results will only be printed for predicted phasings with log-likelihood ratios equal to or greater than this threshold. Setting this to zero will cause all reads to be assigned to the phase to which they share the greatest number matches. Log-likelihood ratios will still be reported in the output in this case, but are not used for phasing decisions.',
         metavar = '<MIN_LIKELIHOOD_RATIO>'
     )
 
     phasing_parser_stats_error.add_argument(
         #This option is permanently disabled!
         #When using sequencing error models other than the default (shared error rate
```

### Comparing `LRphase-1.1.0/src/LRphase/urls.py` & `LRphase-1.1.1/src/LRphase/urls.py`

 * *Files identical despite different names*

### Comparing `LRphase-1.1.0/src/LRphase.egg-info/PKG-INFO` & `LRphase-1.1.1/src/LRphase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LRphase
-Version: 1.1.0
+Version: 1.1.1
 Summary: Phasing individual long reads using known haplotype information.
 Home-page: https://github.com/Boyle-Lab/LRphase.git
 Author: Greg Farnum
 Author-email: gregfar@umich.edu
 License: MIT
 Project-URL: Issue Tracker, https://github.com/Boyle-Lab/LRphase/issues
 Description: # LRphase
```

### Comparing `LRphase-1.1.0/src/LRphase.egg-info/SOURCES.txt` & `LRphase-1.1.1/src/LRphase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

