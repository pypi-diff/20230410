# Comparing `tmp/recon_lw-2.0.0.dev4658240612.tar.gz` & `tmp/recon_lw-2.0.0.dev4658666204.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev4658240612.tar", last modified: Mon Apr 10 14:19:48 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev4658666204.tar", last modified: Mon Apr 10 15:14:54 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev4658240612.tar` & `recon_lw-2.0.0.dev4658666204.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 14:19:48.000000 recon_lw-2.0.0.dev4658240612/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-04-10 14:19:14.000000 recon_lw-2.0.0.dev4658240612/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-10 14:19:48.000000 recon_lw-2.0.0.dev4658240612/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-10 14:19:14.000000 recon_lw-2.0.0.dev4658240612/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-04-10 14:19:37.000000 recon_lw-2.0.0.dev4658240612/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 14:19:48.000000 recon_lw-2.0.0.dev4658240612/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-04-10 14:19:14.000000 recon_lw-2.0.0.dev4658240612/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12849 2023-04-10 14:19:14.000000 recon_lw-2.0.0.dev4658240612/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    13155 2023-04-10 14:19:14.000000 recon_lw-2.0.0.dev4658240612/recon_lw/recon_ob.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 14:19:48.000000 recon_lw-2.0.0.dev4658240612/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-10 14:19:48.000000 recon_lw-2.0.0.dev4658240612/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      287 2023-04-10 14:19:48.000000 recon_lw-2.0.0.dev4658240612/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-10 14:19:48.000000 recon_lw-2.0.0.dev4658240612/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-04-10 14:19:48.000000 recon_lw-2.0.0.dev4658240612/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-10 14:19:48.000000 recon_lw-2.0.0.dev4658240612/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-10 14:19:14.000000 recon_lw-2.0.0.dev4658240612/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-10 14:19:48.000000 recon_lw-2.0.0.dev4658240612/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-04-10 14:19:14.000000 recon_lw-2.0.0.dev4658240612/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:14:54.000000 recon_lw-2.0.0.dev4658666204/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-04-10 15:14:20.000000 recon_lw-2.0.0.dev4658666204/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-10 15:14:54.000000 recon_lw-2.0.0.dev4658666204/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-10 15:14:20.000000 recon_lw-2.0.0.dev4658666204/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-04-10 15:14:41.000000 recon_lw-2.0.0.dev4658666204/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:14:54.000000 recon_lw-2.0.0.dev4658666204/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-04-10 15:14:20.000000 recon_lw-2.0.0.dev4658666204/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12849 2023-04-10 15:14:20.000000 recon_lw-2.0.0.dev4658666204/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13157 2023-04-10 15:14:20.000000 recon_lw-2.0.0.dev4658666204/recon_lw/recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:14:54.000000 recon_lw-2.0.0.dev4658666204/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-10 15:14:54.000000 recon_lw-2.0.0.dev4658666204/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      287 2023-04-10 15:14:54.000000 recon_lw-2.0.0.dev4658666204/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-10 15:14:54.000000 recon_lw-2.0.0.dev4658666204/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-04-10 15:14:54.000000 recon_lw-2.0.0.dev4658666204/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-10 15:14:54.000000 recon_lw-2.0.0.dev4658666204/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-10 15:14:20.000000 recon_lw-2.0.0.dev4658666204/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-10 15:14:54.000000 recon_lw-2.0.0.dev4658666204/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-04-10 15:14:20.000000 recon_lw-2.0.0.dev4658666204/setup.py
```

### Comparing `recon_lw-2.0.0.dev4658240612/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev4658666204/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4658240612/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev4658666204/recon_lw/recon_ob.py`

 * *Files 0% similar despite different names*

```diff
@@ -286,25 +286,25 @@
         return result_body
 
     order_book[side_key].pop(del_index)
 
     return {}
 
 
-def ob_aggr_update_level(side, level, price, real_qty, real_num_orders, impl_qty, iml_num_orders, order_book):
+def ob_aggr_update_level(side, level, price, real_qty, real_num_orders, impl_qty, impl_num_orders, order_book):
     result_body = {}
     max_levels = order_book["aggr_max_levels"]
     side_key = side+"_aggr"
     update_index = level - 1
     if not 0 <= update_index < len(order_book[side_key]):
         result_body["error"] = "Unexpected level {0}, against existing {1}".format(level, len(order_book[side_key]))
         return result_body
 
     upd_level = {"price": price, "real_qty": real_qty, "real_num_orders": real_num_orders, 
-                 "impl_qty" : impl_qty, "impl_num_orders": iml_num_orders}
+                 "impl_qty" : impl_qty, "impl_num_orders": impl_num_orders}
     order_book[side_key][update_index].update(upd_level)
 
     return {}
 
 
 def ob_top_update(ask_price, ask_real_qty, ask_impl_qty, ask_real_n_orders, ask_impl_n_orders,
                   bid_price, bid_real_qty, bid_impl_qty, bid_real_n_orders, bid_impl_n_orders,
```

### Comparing `recon_lw-2.0.0.dev4658240612/setup.py` & `recon_lw-2.0.0.dev4658666204/setup.py`

 * *Files identical despite different names*

