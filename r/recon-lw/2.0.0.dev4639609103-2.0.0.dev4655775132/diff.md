# Comparing `tmp/recon_lw-2.0.0.dev4639609103.tar.gz` & `tmp/recon_lw-2.0.0.dev4655775132.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev4639609103.tar", last modified: Fri Apr  7 16:13:24 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev4655775132.tar", last modified: Mon Apr 10 08:12:23 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev4639609103.tar` & `recon_lw-2.0.0.dev4655775132.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 16:13:24.000000 recon_lw-2.0.0.dev4639609103/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-04-07 16:13:07.000000 recon_lw-2.0.0.dev4639609103/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-07 16:13:24.000000 recon_lw-2.0.0.dev4639609103/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-07 16:13:07.000000 recon_lw-2.0.0.dev4639609103/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-04-07 16:13:13.000000 recon_lw-2.0.0.dev4639609103/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 16:13:24.000000 recon_lw-2.0.0.dev4639609103/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-04-07 16:13:07.000000 recon_lw-2.0.0.dev4639609103/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12849 2023-04-07 16:13:07.000000 recon_lw-2.0.0.dev4639609103/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    12172 2023-04-07 16:13:07.000000 recon_lw-2.0.0.dev4639609103/recon_lw/recon_ob.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 16:13:24.000000 recon_lw-2.0.0.dev4639609103/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-07 16:13:24.000000 recon_lw-2.0.0.dev4639609103/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      287 2023-04-07 16:13:24.000000 recon_lw-2.0.0.dev4639609103/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-07 16:13:24.000000 recon_lw-2.0.0.dev4639609103/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-04-07 16:13:24.000000 recon_lw-2.0.0.dev4639609103/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-07 16:13:24.000000 recon_lw-2.0.0.dev4639609103/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-07 16:13:07.000000 recon_lw-2.0.0.dev4639609103/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-07 16:13:24.000000 recon_lw-2.0.0.dev4639609103/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-04-07 16:13:07.000000 recon_lw-2.0.0.dev4639609103/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 08:12:23.000000 recon_lw-2.0.0.dev4655775132/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-04-10 08:11:47.000000 recon_lw-2.0.0.dev4655775132/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-10 08:12:23.000000 recon_lw-2.0.0.dev4655775132/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-10 08:11:47.000000 recon_lw-2.0.0.dev4655775132/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-04-10 08:12:11.000000 recon_lw-2.0.0.dev4655775132/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 08:12:23.000000 recon_lw-2.0.0.dev4655775132/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-04-10 08:11:47.000000 recon_lw-2.0.0.dev4655775132/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12849 2023-04-10 08:11:47.000000 recon_lw-2.0.0.dev4655775132/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12936 2023-04-10 08:11:47.000000 recon_lw-2.0.0.dev4655775132/recon_lw/recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 08:12:23.000000 recon_lw-2.0.0.dev4655775132/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-10 08:12:23.000000 recon_lw-2.0.0.dev4655775132/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      287 2023-04-10 08:12:23.000000 recon_lw-2.0.0.dev4655775132/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-10 08:12:23.000000 recon_lw-2.0.0.dev4655775132/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-04-10 08:12:23.000000 recon_lw-2.0.0.dev4655775132/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-10 08:12:23.000000 recon_lw-2.0.0.dev4655775132/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-10 08:11:47.000000 recon_lw-2.0.0.dev4655775132/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-10 08:12:23.000000 recon_lw-2.0.0.dev4655775132/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-04-10 08:11:47.000000 recon_lw-2.0.0.dev4655775132/setup.py
```

### Comparing `recon_lw-2.0.0.dev4639609103/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev4655775132/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4639609103/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev4655775132/recon_lw/recon_ob.py`

 * *Files 18% similar despite different names*

```diff
@@ -284,20 +284,38 @@
         return result_body
 
     order_book[side_key].pop(del_index)
 
     return {}
 
 
-def ob_aggr_update_level(side, level, price, qty, num_orders, impl_qty, iml_num_orders, order_book):
+def ob_aggr_update_level(side, level, price, real_qty, real_num_orders, impl_qty, iml_num_orders, order_book):
     result_body = {}
     max_levels = order_book["aggr_max_levels"]
     side_key = side+"_aggr"
     update_index = level - 1
     if not 0 <= update_index < len(order_book[side_key]):
         result_body["error"] = "Unexpected level {0}, against existing {1}".format(level, len(order_book[side_key]))
         return result_body
 
-    upd_level = {"price": price, "qty": qty, "num_orders": num_orders, "impl_qty" : impl_qty, "impl_num_orders": iml_num_orders}
+    upd_level = {"price": price, "real_qty": real_qty, "real_num_orders": real_num_orders, 
+                 "impl_qty" : impl_qty, "impl_num_orders": iml_num_orders}
     order_book[side_key][update_index].update(upd_level)
 
     return {}
+
+
+def ob_top_update(ask_price, ask_real_qty, ask_impl_qty, ask_real_n_orders, ask_impl_n_orders,
+                  bid_price, bid_real_qty, bid_impl_qty, bid_real_n_orders, bid_impl_n_orders,
+                  order_book):
+    order_book["ask_price"] = ask_price
+    order_book["ask_real_qty"] = ask_real_qty
+    order_book["ask_impl_qty"] = ask_impl_qty
+    order_book["ask_real_n_orders"] = ask_real_n_orders
+    order_book["ask_impl_n_orders"] = ask_impl_n_orders
+    order_book["bid_price"] = bid_price
+    order_book["bid_real_qty"] = bid_real_qty
+    order_book["bid_impl_qty"] = bid_impl_qty
+    order_book["bid_real_n_orders"] = bid_real_n_orders
+    order_book["bid_impl_n_orders"] = bid_impl_n_orders
+
+
```

### Comparing `recon_lw-2.0.0.dev4639609103/setup.py` & `recon_lw-2.0.0.dev4655775132/setup.py`

 * *Files identical despite different names*

