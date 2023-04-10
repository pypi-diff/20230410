# Comparing `tmp/damo-1.7.5.tar.gz` & `tmp/damo-1.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "damo-1.7.5.tar", last modified: Mon Apr  3 23:11:38 2023, max compression
+gzip compressed data, was "damo-1.7.6.tar", last modified: Mon Apr 10 17:35:57 2023, max compression
```

## Comparing `damo-1.7.5.tar` & `damo-1.7.6.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-04-03 23:11:38.438166 damo-1.7.5/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5906 2023-04-03 23:11:38.438166 damo-1.7.5/PKG-INFO
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5385 2023-04-03 23:11:34.000000 damo-1.7.5/README.md
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      104 2023-04-03 23:11:34.000000 damo-1.7.5/pyproject.toml
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       38 2023-04-03 23:11:38.438166 damo-1.7.5/setup.cfg
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      959 2023-04-03 23:11:34.000000 damo-1.7.5/setup.py
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-04-03 23:11:38.422166 damo-1.7.5/src/
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-04-03 23:11:38.434166 damo-1.7.5/src/damo/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        0 2023-04-03 23:11:34.000000 damo-1.7.5/src/damo/__init__.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      643 2023-04-03 23:11:34.000000 damo-1.7.5/src/damo/_damo_dist.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     9367 2023-04-03 23:11:34.000000 damo-1.7.5/src/damo/_damo_fmt_str.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3018 2023-04-03 23:11:34.000000 damo-1.7.5/src/damo/_damo_fs.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5368 2023-04-03 23:11:34.000000 damo-1.7.5/src/damo/_damo_paddr_layout.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      916 2023-04-03 23:11:34.000000 damo-1.7.5/src/damo/_damo_python2_support.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      762 2023-04-03 23:11:34.000000 damo-1.7.5/src/damo/_damo_subcmds.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    34357 2023-04-03 23:11:34.000000 damo-1.7.5/src/damo/_damon.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     9926 2023-04-03 23:11:34.000000 damo-1.7.5/src/damo/_damon_args.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7947 2023-04-03 23:11:34.000000 damo-1.7.5/src/damo/_damon_args_schemes.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    17741 2023-04-03 23:11:34.000000 damo-1.7.5/src/damo/_damon_dbgfs.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    17021 2023-04-03 23:11:34.000000 damo-1.7.5/src/damo/_damon_result.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    20452 2023-04-03 23:11:34.000000 damo-1.7.5/src/damo/_damon_sysfs.py
--rwxrwxr-x   0 sjpark    (1000) sjpark    (1000)     3454 2023-04-03 23:11:34.000000 damo-1.7.5/src/damo/damo.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1849 2023-04-03 23:11:34.000000 damo-1.7.5/src/damo/damo_adjust.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1170 2023-04-03 23:11:34.000000 damo-1.7.5/src/damo/damo_features.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      746 2023-04-03 23:11:34.000000 damo-1.7.5/src/damo/damo_fmt_json.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    13288 2023-04-03 23:11:34.000000 damo-1.7.5/src/damo/damo_heats.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4691 2023-04-03 23:11:34.000000 damo-1.7.5/src/damo/damo_lru_sort.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3613 2023-04-03 23:11:34.000000 damo-1.7.5/src/damo/damo_monitor.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2772 2023-04-03 23:11:34.000000 damo-1.7.5/src/damo/damo_nr_regions.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4481 2023-04-03 23:11:34.000000 damo-1.7.5/src/damo/damo_reclaim.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5034 2023-04-03 23:11:34.000000 damo-1.7.5/src/damo/damo_record.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1196 2023-04-03 23:11:34.000000 damo-1.7.5/src/damo/damo_report.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2900 2023-04-03 23:11:34.000000 damo-1.7.5/src/damo/damo_report_raw.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1599 2023-04-03 23:11:34.000000 damo-1.7.5/src/damo/damo_schemes.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      565 2023-04-03 23:11:34.000000 damo-1.7.5/src/damo/damo_start.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2406 2023-04-03 23:11:34.000000 damo-1.7.5/src/damo/damo_stat.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1530 2023-04-03 23:11:34.000000 damo-1.7.5/src/damo/damo_stat_kdamonds.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3097 2023-04-03 23:11:34.000000 damo-1.7.5/src/damo/damo_stat_regions.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2733 2023-04-03 23:11:34.000000 damo-1.7.5/src/damo/damo_stat_schemes.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      681 2023-04-03 23:11:34.000000 damo-1.7.5/src/damo/damo_stop.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      651 2023-04-03 23:11:34.000000 damo-1.7.5/src/damo/damo_tune.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3958 2023-04-03 23:11:34.000000 damo-1.7.5/src/damo/damo_validate.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        6 2023-04-03 23:11:34.000000 damo-1.7.5/src/damo/damo_version.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5483 2023-04-03 23:11:34.000000 damo-1.7.5/src/damo/damo_wss.py
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-04-03 23:11:38.438166 damo-1.7.5/src/damo.egg-info/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5906 2023-04-03 23:11:38.000000 damo-1.7.5/src/damo.egg-info/PKG-INFO
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1102 2023-04-03 23:11:38.000000 damo-1.7.5/src/damo.egg-info/SOURCES.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        1 2023-04-03 23:11:38.000000 damo-1.7.5/src/damo.egg-info/dependency_links.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       40 2023-04-03 23:11:38.000000 damo-1.7.5/src/damo.egg-info/entry_points.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        5 2023-04-03 23:11:38.000000 damo-1.7.5/src/damo.egg-info/top_level.txt
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-04-10 17:35:57.323521 damo-1.7.6/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     6519 2023-04-10 17:35:57.323521 damo-1.7.6/PKG-INFO
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5998 2023-04-10 17:35:53.000000 damo-1.7.6/README.md
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      104 2023-04-10 17:35:53.000000 damo-1.7.6/pyproject.toml
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       38 2023-04-10 17:35:57.323521 damo-1.7.6/setup.cfg
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      959 2023-04-10 17:35:53.000000 damo-1.7.6/setup.py
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-04-10 17:35:57.307522 damo-1.7.6/src/
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-04-10 17:35:57.323521 damo-1.7.6/src/damo/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        0 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/__init__.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      643 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/_damo_dist.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     9696 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/_damo_fmt_str.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3018 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/_damo_fs.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5368 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/_damo_paddr_layout.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      916 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/_damo_python2_support.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      762 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/_damo_subcmds.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    34437 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/_damon.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     9979 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/_damon_args.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8196 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/_damon_args_schemes.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    17741 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/_damon_dbgfs.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    17021 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/_damon_result.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    20452 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/_damon_sysfs.py
+-rwxrwxr-x   0 sjpark    (1000) sjpark    (1000)     3643 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1849 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo_adjust.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1170 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo_features.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      746 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo_fmt_json.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    13288 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo_heats.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4691 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo_lru_sort.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3613 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo_monitor.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2772 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo_nr_regions.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4481 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo_reclaim.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5108 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo_record.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1196 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo_report.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2900 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo_report_raw.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1599 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo_schemes.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      565 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo_start.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2406 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo_stat.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1530 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo_stat_kdamonds.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3097 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo_stat_regions.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2733 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo_stat_schemes.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      681 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo_stop.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      727 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo_translate_damos.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      651 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo_tune.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3958 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo_validate.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        6 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo_version.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5568 2023-04-10 17:35:53.000000 damo-1.7.6/src/damo/damo_wss.py
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-04-10 17:35:57.323521 damo-1.7.6/src/damo.egg-info/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     6519 2023-04-10 17:35:57.000000 damo-1.7.6/src/damo.egg-info/PKG-INFO
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1135 2023-04-10 17:35:57.000000 damo-1.7.6/src/damo.egg-info/SOURCES.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        1 2023-04-10 17:35:57.000000 damo-1.7.6/src/damo.egg-info/dependency_links.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       40 2023-04-10 17:35:57.000000 damo-1.7.6/src/damo.egg-info/entry_points.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        5 2023-04-10 17:35:57.000000 damo-1.7.6/src/damo.egg-info/top_level.txt
```

### Comparing `damo-1.7.5/PKG-INFO` & `damo-1.7.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damo
-Version: 1.7.5
+Version: 1.7.6
 Summary: DAMON user-space tool
 Home-page: https://github.com/awslabs/damo
 Author: SeongJae Park
 Author-email: sj@kernel.org
 Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
 Project-URL: DAMON, https://damonitor.github.io
 Classifier: Programming Language :: Python :: 3
@@ -42,16 +42,16 @@
     $ # ensure your kernel is built with CONFIG_DAMON_*=y
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.5/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.5/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.6/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.6/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -59,15 +59,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.7.5/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.7.6/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -87,14 +87,28 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
+I show --rbuf option from `damo record` is removed.  What happened?
+-------------------------------------------------------------------
+
+The option is deprecated.  Please report your usecase to sj@kernel.org,
+damon@lists.linux.dev and linux-mm@kvack.org if you depend on those.
+
+
+damo suddenly exit with `You're using unsupported DAMOS format` message.  Why?
+-----------------------------------------------------------------------------
+
+Because the DAMOS input you're using is no more supported.  Please report your
+usecase to sj@kernel.org, damon@lists.linux.dev and linux-mm@kvack.org if you
+depend on those.
+
 
 Recording Data Access Patterns
 ==============================
 
 Below commands record memory access patterns of a program and save the
 monitoring results in `damon.data` file.
```

### Comparing `damo-1.7.5/README.md` & `damo-1.7.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -27,16 +27,16 @@
     $ # ensure your kernel is built with CONFIG_DAMON_*=y
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.5/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.5/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.6/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.6/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -44,15 +44,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.7.5/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.7.6/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -72,14 +72,28 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
+I show --rbuf option from `damo record` is removed.  What happened?
+-------------------------------------------------------------------
+
+The option is deprecated.  Please report your usecase to sj@kernel.org,
+damon@lists.linux.dev and linux-mm@kvack.org if you depend on those.
+
+
+damo suddenly exit with `You're using unsupported DAMOS format` message.  Why?
+-----------------------------------------------------------------------------
+
+Because the DAMOS input you're using is no more supported.  Please report your
+usecase to sj@kernel.org, damon@lists.linux.dev and linux-mm@kvack.org if you
+depend on those.
+
 
 Recording Data Access Patterns
 ==============================
 
 Below commands record memory access patterns of a program and save the
 monitoring results in `damon.data` file.
```

### Comparing `damo-1.7.5/setup.py` & `damo-1.7.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="damo",
-    version="1.7.5",
+    version="1.7.6",
     author="SeongJae Park",
     author_email="sj@kernel.org",
     description="DAMON user-space tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/awslabs/damo",
     project_urls={
```

### Comparing `damo-1.7.5/src/damo/_damo_dist.py` & `damo-1.7.6/src/damo/_damo_dist.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.5/src/damo/_damo_fmt_str.py` & `damo-1.7.6/src/damo/_damo_fmt_str.py`

 * *Files 8% similar despite different names*

```diff
@@ -181,18 +181,21 @@
     pass
 
 uint_max = 2**32 - 1
 ulong_max = 2**64 - 1
 if platform.architecture()[0] != '64bit':
     ulong_max = 2**32 - 1
 
-unit_to_bytes = {'B': 1, 'K': 1 << 10, 'KiB': 1 << 10,
-        'M': 1 << 20, 'MiB': 1 << 20, 'G': 1 << 30, 'GiB': 1 << 30,
-        'T': 1 << 40, 'TiB': 1 << 40, 'P': 1 << 50, 'PiB': 1 << 50,
-        'E': 1 << 60, 'EiB': 1 << 60}
+unit_to_bytes = {'B': 1,
+        'K': 1 << 10, 'KB': 1 << 10, 'KiB': 1 << 10,
+        'M': 1 << 20, 'MB': 1 << 20, 'MiB': 1 << 20,
+        'G': 1 << 30, 'GB': 1 << 30, 'GiB': 1 << 30,
+        'T': 1 << 40, 'TB': 1 << 40, 'TiB': 1 << 40,
+        'P': 1 << 50, 'PB': 1 << 50, 'PiB': 1 << 50,
+        'E': 1 << 60, 'EB': 1 << 60, 'EiB': 1 << 60}
 
 def text_to_nr(txt):
     if type(txt) in number_types:
         return txt
 
     new_txt = ''.join([c for c in txt if c != ','])
     try:
@@ -223,14 +226,22 @@
         unit = txt[len(txt) - 3:]
         if unit in unit_to_bytes:
             number = text_to_nr(txt[:-3])
         else:
             unit = None
 
     if unit == None:
+        if len(txt) > 2:
+            unit = txt[len(txt) - 2:]
+            if unit in unit_to_bytes:
+                number = text_to_nr(txt[:-2])
+            else:
+                unit = None
+
+    if unit == None:
         if txt[-1] in unit_to_bytes:
             unit = txt[-1]
             number = text_to_nr(txt[:-1])
         else:
             unit = 'B'
             number  = text_to_nr(txt)
```

### Comparing `damo-1.7.5/src/damo/_damo_fs.py` & `damo-1.7.6/src/damo/_damo_fs.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.5/src/damo/_damo_paddr_layout.py` & `damo-1.7.6/src/damo/_damo_paddr_layout.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.5/src/damo/_damo_python2_support.py` & `damo-1.7.6/src/damo/_damo_python2_support.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.5/src/damo/_damo_subcmds.py` & `damo-1.7.6/src/damo/_damo_subcmds.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.5/src/damo/_damon.py` & `damo-1.7.6/src/damo/_damon.py`

 * *Files 1% similar despite different names*

```diff
@@ -601,28 +601,31 @@
             for region in self.tried_regions:
                 lines.append(_damo_fmt_str.indent_lines(region.to_str(raw), 4))
         return '\n'.join(lines)
 
     def __str__(self):
         return self.to_str(False)
 
+    def __repr__(self):
+        return self.__str__()
+
     def __eq__(self, other):
         return (type(self) == type(other) and self.name == other.name and
                 self.access_pattern == other.access_pattern and
                 self.action == other.action and self.quotas == other.quotas and
                 self.watermarks == other.watermarks and
                 self.filters == other.filters)
 
     @classmethod
     def from_kvpairs(cls, kv):
         filters = []
         if 'filters' in kv:
             for damos_filter_kv in kv['filters']:
                 filters.append(DamosFilter.from_kvpairs(damos_filter_kv))
-        return Damos(kv['name'],
+        return Damos(kv['name'] if 'name' in kv else '0',
                 DamosAccessPattern.from_kvpairs(kv['access_pattern'])
                     if 'access_pattern' in kv else DamosAccessPattern(),
                 kv['action'] if 'action' in kv else damos_action_stat,
                 DamosQuotas.from_kvpairs(kv['quotas'])
                     if 'quotas' in kv else DamosQuotas(),
                 DamosWatermarks.from_kvpairs(kv['watermarks'])
                     if 'watermarks' in kv else DamosWatermarks(),
```

### Comparing `damo-1.7.5/src/damo/_damon_args.py` & `damo-1.7.6/src/damo/_damon_args.py`

 * *Files 1% similar despite different names*

```diff
@@ -259,13 +259,14 @@
 	    help='data access monitoring-based operation schemes')
     parser.add_argument('--kdamonds', metavar='<json string or file>',
             help='json format kdamonds specification to run DAMON for')
     parser.add_argument('deducible_target', type=str,
             metavar='<deducible target>', nargs='?',
             help='the target (command, pid, or special keywords) to monitor')
     if add_record_options:
-        parser.add_argument('-l', '--rbuf', metavar='<len>', type=int,
-                help='length of record result buffer (!! DEPRECATED)')
+        # Uncomment if some dependant user found
+        # parser.add_argument('-l', '--rbuf', metavar='<len>', type=int,
+        #         help='length of record result buffer (!! DEPRECATED)')
         parser.add_argument('-o', '--out', metavar='<file path>', type=str,
                 default='damon.data', help='output file path')
     set_common_argparser(parser)
     return parser
```

### Comparing `damo-1.7.5/src/damo/_damon_args_schemes.py` & `damo-1.7.6/src/damo/_damon_args_schemes.py`

 * *Files 4% similar despite different names*

```diff
@@ -131,28 +131,38 @@
     scheme.watermarks.interval_us = _damo_fmt_str.text_to_us(
             fields[14])
     scheme.watermarks.high_permil = int(fields[15])
     scheme.watermarks.mid_permil = int(fields[16])
     scheme.watermarks.low_permil = int(fields[17])
     return scheme
 
-def damo_single_line_scheme_to_damos(line, name):
+avoid_crashing_v1_v3_schemes_for_testing = False
+def damo_single_line_scheme_to_damos(line):
     '''Returns Damos object and err'''
 
     sys.stderr.write('''
 WARNING: single line per-scheme scheme input is deprecated.  The support will
 be removed by 2023-Q2.  Please use json format or --damos_* commandline options
 instead.
 
 Please report your usecase to sj@kernel.org, damon@liss.linux.dev
 and linux-mm@kvack.org if you depend on it.
 
 ''')
 
     fields = line.split()
+
+    # Remove below if someone depends on the v1-v3  DAMOS input is found.
+    if not avoid_crashing_v1_v3_schemes_for_testing:
+        if len(fields) in [9, 12, 17]:
+            sys.stderr.write('''
+You're using unsupported DAMOS format (%s)
+    ''' % ' '.join(fields))
+            exit(1)
+
     try:
         if len(fields) == 7:
             return fields_to_v0_scheme(fields), None
         elif len(fields) == 9:
             return fields_to_v1_scheme(fields), None
         elif len(fields) == 12:
             return fields_to_v2_scheme(fields), None
@@ -163,42 +173,38 @@
         else:
             return None, 'expected %s fields, but \'%s\'' % (
                     [7, 9, 12, 17, 18], line)
     except:
         return None, 'wrong input field'
     return None, 'unsupported version of single line scheme'
 
-def damo_schemes_lines_except_comments(txt):
-    return [l for l in txt.strip().split('\n')
-            if not l.strip().startswith('#')]
-
-def damo_schemes_to_damos(damo_schemes):
-    if os.path.isfile(damo_schemes):
-        with open(damo_schemes, 'r') as f:
-            damo_schemes = f.read()
+def schemes_option_to_damos(schemes):
+    if os.path.isfile(schemes):
+        with open(schemes, 'r') as f:
+            schemes = f.read()
 
     try:
-        kvpairs = json.loads(damo_schemes)
+        kvpairs = json.loads(schemes)
         return [_damon.Damos.from_kvpairs(kv) for kv in kvpairs], None
     except Exception as json_err:
         # The input is not json file
         pass
 
-    damo_schemes_lines = damo_schemes_lines_except_comments(damo_schemes)
+    # remove comments, empty lines, and unnecessary white spaces
+    damo_schemes_lines = [l.strip() for l in schemes.strip().split('\n')
+            if not l.strip().startswith('#') and l.strip() != '']
 
     damos_list = []
-    for idx, line in enumerate(damo_schemes_lines):
-        line = line.strip()
-        if line == '':
-            continue
-        damos, err = damo_single_line_scheme_to_damos(line, '%d' % idx)
+    for line in damo_schemes_lines:
+        damos, err = damo_single_line_scheme_to_damos(line)
         if err != None:
             return None, ('invalid input: ' +
                     'neither json (%s), nor per-line scheme (%s)'
                     % (json_err, err))
+        damos.name = '%d' % len(damos_list)
         damos_list.append(damos)
     return damos_list, None
 
 def options_to_scheme(args):
     try:
         return _damon.Damos(
                 access_pattern=_damon.DamosAccessPattern(
@@ -214,11 +220,11 @@
         if err != None:
             return None, err
         return [damos], None
 
     if not 'schemes' in args or args.schemes == None:
         return [], None
 
-    schemes, err = damo_schemes_to_damos(args.schemes)
+    schemes, err = schemes_option_to_damos(args.schemes)
     if err:
         return None, 'failed damo schemes arguents parsing (%s)' % err
     return schemes, None
```

### Comparing `damo-1.7.5/src/damo/_damon_dbgfs.py` & `damo-1.7.6/src/damo/_damon_dbgfs.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.5/src/damo/_damon_result.py` & `damo-1.7.6/src/damo/_damon_result.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.5/src/damo/_damon_sysfs.py` & `damo-1.7.6/src/damo/_damon_sysfs.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.5/src/damo/damo.py` & `damo-1.7.6/src/damo/damo.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import damo_report
 import damo_schemes
 import damo_start
 import damo_stat
 import damo_stop
 import damo_tune
 import damo_validate
+import damo_translate_damos
 
 import _damo_subcmds
 
 def pr_damo_version(args_not_use):
     bindir = os.path.dirname(os.path.abspath(__file__))
     with open(os.path.join(bindir, 'damo_version.py'), 'r') as f:
         print(f.read().strip())
@@ -59,14 +60,17 @@
         _damo_subcmds.DamoSubCmd(name='tune', module=damo_tune,
             msg='update input parameters of ongoing DAMON'),
         _damo_subcmds.DamoSubCmd(name='fmt_json', module=damo_fmt_json,
             msg='convert damo-start cmdline option to DAMON json input'),
         _damo_subcmds.DamoSubCmd(name='version',
             module=_damo_subcmds.DamoSubCmdModule(None, pr_damo_version),
             msg='print the version number'),
+        _damo_subcmds.DamoSubCmd(name='translate_damos',
+            module=damo_translate_damos,
+            msg='translate old .damos to the new json format')
         ]
 
 class SubCmdHelpFormatter(argparse.RawDescriptionHelpFormatter):
     def _format_action(self, action):
         parts = super(argparse.RawDescriptionHelpFormatter,
                 self)._format_action(action)
         # skip sub parsers help
```

### Comparing `damo-1.7.5/src/damo/damo_adjust.py` & `damo-1.7.6/src/damo/damo_adjust.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.5/src/damo/damo_features.py` & `damo-1.7.6/src/damo/damo_features.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.5/src/damo/damo_fmt_json.py` & `damo-1.7.6/src/damo/damo_fmt_json.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.5/src/damo/damo_heats.py` & `damo-1.7.6/src/damo/damo_heats.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.5/src/damo/damo_lru_sort.py` & `damo-1.7.6/src/damo/damo_lru_sort.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.5/src/damo/damo_monitor.py` & `damo-1.7.6/src/damo/damo_monitor.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.5/src/damo/damo_nr_regions.py` & `damo-1.7.6/src/damo/damo_nr_regions.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.5/src/damo/damo_reclaim.py` & `damo-1.7.6/src/damo/damo_reclaim.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.5/src/damo/damo_record.py` & `damo-1.7.6/src/damo/damo_record.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,14 +55,17 @@
 def set_data_for_cleanup(data_for_cleanup, args, output_permission):
     data_for_cleanup.rfile_format = args.output_type
     data_for_cleanup.rfile_path = args.out
     data_for_cleanup.rfile_permission = output_permission
     data_for_cleanup.orig_kdamonds = _damon.current_kdamonds()
 
 def chk_handle_record_feature_support(args):
+    # Comment below line if --rbuf dependent user found
+    return False
+
     damon_record_supported = _damon.feature_supported('record')
     if not damon_record_supported:
         if args.rbuf:
             print('# \'--rbuf\' will be ignored')
 
     if damon_record_supported or args.rbuf:
         sys.stderr.write('''
```

### Comparing `damo-1.7.5/src/damo/damo_report.py` & `damo-1.7.6/src/damo/damo_report.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.5/src/damo/damo_report_raw.py` & `damo-1.7.6/src/damo/damo_report_raw.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.5/src/damo/damo_schemes.py` & `damo-1.7.6/src/damo/damo_schemes.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.5/src/damo/damo_start.py` & `damo-1.7.6/src/damo/damo_start.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.5/src/damo/damo_stat.py` & `damo-1.7.6/src/damo/damo_stat.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.5/src/damo/damo_stat_kdamonds.py` & `damo-1.7.6/src/damo/damo_stat_kdamonds.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.5/src/damo/damo_stat_regions.py` & `damo-1.7.6/src/damo/damo_stat_regions.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.5/src/damo/damo_stat_schemes.py` & `damo-1.7.6/src/damo/damo_stat_schemes.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.5/src/damo/damo_stop.py` & `damo-1.7.6/src/damo/damo_stop.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.5/src/damo/damo_tune.py` & `damo-1.7.6/src/damo/damo_tune.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.5/src/damo/damo_validate.py` & `damo-1.7.6/src/damo/damo_validate.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.5/src/damo/damo_wss.py` & `damo-1.7.6/src/damo/damo_wss.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,17 @@
         wss_dists[record.target_id] = wss_dist
     return wss_dists
 
 def pr_wss_dists(wss_dists, percentiles, raw_number, nr_cols_bar, pr_all_wss):
     print('# <percentile> <wss>')
     for tid, wss_dist in wss_dists.items():
         print('# target_id\t%s' % tid)
+        if len(wss_dist) == 0:
+            print('# no snapshot')
+            return
         print('# avr:\t%s' % _damo_fmt_str.format_sz(
             sum(wss_dist) / len(wss_dist), raw_number))
 
         if pr_all_wss:
             for idx, wss in enumerate(wss_dist):
                 print('%s %s' % (idx, _damo_fmt_str.format_sz(wss, raw_number)))
             return
```

### Comparing `damo-1.7.5/src/damo.egg-info/PKG-INFO` & `damo-1.7.6/src/damo.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damo
-Version: 1.7.5
+Version: 1.7.6
 Summary: DAMON user-space tool
 Home-page: https://github.com/awslabs/damo
 Author: SeongJae Park
 Author-email: sj@kernel.org
 Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
 Project-URL: DAMON, https://damonitor.github.io
 Classifier: Programming Language :: Python :: 3
@@ -42,16 +42,16 @@
     $ # ensure your kernel is built with CONFIG_DAMON_*=y
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.5/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.5/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.6/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.6/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -59,15 +59,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.7.5/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.7.6/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -87,14 +87,28 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
+I show --rbuf option from `damo record` is removed.  What happened?
+-------------------------------------------------------------------
+
+The option is deprecated.  Please report your usecase to sj@kernel.org,
+damon@lists.linux.dev and linux-mm@kvack.org if you depend on those.
+
+
+damo suddenly exit with `You're using unsupported DAMOS format` message.  Why?
+-----------------------------------------------------------------------------
+
+Because the DAMOS input you're using is no more supported.  Please report your
+usecase to sj@kernel.org, damon@lists.linux.dev and linux-mm@kvack.org if you
+depend on those.
+
 
 Recording Data Access Patterns
 ==============================
 
 Below commands record memory access patterns of a program and save the
 monitoring results in `damon.data` file.
```

### Comparing `damo-1.7.5/src/damo.egg-info/SOURCES.txt` & `damo-1.7.6/src/damo.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 src/damo/damo_schemes.py
 src/damo/damo_start.py
 src/damo/damo_stat.py
 src/damo/damo_stat_kdamonds.py
 src/damo/damo_stat_regions.py
 src/damo/damo_stat_schemes.py
 src/damo/damo_stop.py
+src/damo/damo_translate_damos.py
 src/damo/damo_tune.py
 src/damo/damo_validate.py
 src/damo/damo_version.py
 src/damo/damo_wss.py
 src/damo.egg-info/PKG-INFO
 src/damo.egg-info/SOURCES.txt
 src/damo.egg-info/dependency_links.txt
```

