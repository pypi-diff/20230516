# Comparing `tmp/recon_lw-2.0.0.dev4991603720.tar.gz` & `tmp/recon_lw-2.0.0.dev4992831728.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev4991603720.tar", last modified: Tue May 16 12:04:47 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev4992831728.tar", last modified: Tue May 16 13:58:36 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev4991603720.tar` & `recon_lw-2.0.0.dev4992831728.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 12:04:47.000000 recon_lw-2.0.0.dev4991603720/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-16 12:04:21.000000 recon_lw-2.0.0.dev4991603720/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-16 12:04:47.000000 recon_lw-2.0.0.dev4991603720/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-16 12:04:21.000000 recon_lw-2.0.0.dev4991603720/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-16 12:04:27.000000 recon_lw-2.0.0.dev4991603720/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 12:04:47.000000 recon_lw-2.0.0.dev4991603720/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-05-16 12:04:21.000000 recon_lw-2.0.0.dev4991603720/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-05-16 12:04:21.000000 recon_lw-2.0.0.dev4991603720/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     2773 2023-05-16 12:04:21.000000 recon_lw-2.0.0.dev4991603720/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-16 12:04:21.000000 recon_lw-2.0.0.dev4991603720/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-05-16 12:04:21.000000 recon_lw-2.0.0.dev4991603720/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    27755 2023-05-16 12:04:21.000000 recon_lw-2.0.0.dev4991603720/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    15433 2023-05-16 12:04:21.000000 recon_lw-2.0.0.dev4991603720/recon_lw/recon_ob_cross_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 12:04:47.000000 recon_lw-2.0.0.dev4991603720/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-16 12:04:47.000000 recon_lw-2.0.0.dev4991603720/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      425 2023-05-16 12:04:47.000000 recon_lw-2.0.0.dev4991603720/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-16 12:04:47.000000 recon_lw-2.0.0.dev4991603720/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-16 12:04:47.000000 recon_lw-2.0.0.dev4991603720/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-16 12:04:47.000000 recon_lw-2.0.0.dev4991603720/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-16 12:04:21.000000 recon_lw-2.0.0.dev4991603720/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-16 12:04:47.000000 recon_lw-2.0.0.dev4991603720/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-16 12:04:21.000000 recon_lw-2.0.0.dev4991603720/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 12:04:47.000000 recon_lw-2.0.0.dev4991603720/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-05-16 12:04:21.000000 recon_lw-2.0.0.dev4991603720/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 13:58:36.000000 recon_lw-2.0.0.dev4992831728/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-16 13:58:05.000000 recon_lw-2.0.0.dev4992831728/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-16 13:58:36.000000 recon_lw-2.0.0.dev4992831728/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-16 13:58:05.000000 recon_lw-2.0.0.dev4992831728/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-16 13:58:14.000000 recon_lw-2.0.0.dev4992831728/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 13:58:36.000000 recon_lw-2.0.0.dev4992831728/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-05-16 13:58:05.000000 recon_lw-2.0.0.dev4992831728/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-05-16 13:58:05.000000 recon_lw-2.0.0.dev4992831728/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2773 2023-05-16 13:58:05.000000 recon_lw-2.0.0.dev4992831728/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-16 13:58:05.000000 recon_lw-2.0.0.dev4992831728/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-05-16 13:58:05.000000 recon_lw-2.0.0.dev4992831728/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27755 2023-05-16 13:58:05.000000 recon_lw-2.0.0.dev4992831728/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15427 2023-05-16 13:58:05.000000 recon_lw-2.0.0.dev4992831728/recon_lw/recon_ob_cross_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 13:58:36.000000 recon_lw-2.0.0.dev4992831728/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-16 13:58:36.000000 recon_lw-2.0.0.dev4992831728/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      425 2023-05-16 13:58:36.000000 recon_lw-2.0.0.dev4992831728/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-16 13:58:36.000000 recon_lw-2.0.0.dev4992831728/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-16 13:58:36.000000 recon_lw-2.0.0.dev4992831728/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-16 13:58:36.000000 recon_lw-2.0.0.dev4992831728/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-16 13:58:05.000000 recon_lw-2.0.0.dev4992831728/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-16 13:58:36.000000 recon_lw-2.0.0.dev4992831728/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-16 13:58:05.000000 recon_lw-2.0.0.dev4992831728/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 13:58:36.000000 recon_lw-2.0.0.dev4992831728/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-05-16 13:58:05.000000 recon_lw-2.0.0.dev4992831728/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev4991603720/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev4992831728/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4991603720/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev4992831728/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4991603720/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev4992831728/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4991603720/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev4992831728/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4991603720/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev4992831728/recon_lw/recon_ob.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4991603720/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev4992831728/recon_lw/recon_ob_cross_stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     problems = []
     if len(full_book["ask"]) > 0:
         if top_book["ask_real_qty"] == 0 and top_book["ask_impl_qty"] == 0:
             problems.append({"synopsys": "top_miss_level", "side": "ask"})
         else:
             top_p = min(full_book["ask"].keys())
             price_condition = top_p == top_book["ask_price"]
-            num_orders_condition = len(full_book["ask"][top_p]) == \
+            num_orders_condition = (full_book["ask"][top_p]) == \
                                    (top_book["ask_impl_n_orders"] + top_book["ask_real_n_orders"])
             size_condition = sum(full_book["ask"][top_p].values()) == (
                     top_book["ask_real_qty"] + top_book["ask_impl_qty"])
             if not (price_condition and num_orders_condition and size_condition):
                 problems.append({"synopsys": synopsys(price_condition, num_orders_condition, size_condition),
                                  "side": "ask"})
     else:
@@ -69,15 +69,15 @@
 
     if len(full_book["bid"]) > 0:
         if top_book["bid_real_qty"] == 0 and top_book["bid_impl_qty"] == 0:
             problems.append({"synopsys": "top_miss_level", "side": "bid"})
         else:
             top_p = max(full_book["bid"].keys())
             price_condition = top_p == top_book["bid_price"]
-            num_orders_condition = len(full_book["bid"][top_p]) == \
+            num_orders_condition = (full_book["bid"][top_p]) == \
                                    (top_book["bid_impl_n_orders"] + top_book["bid_real_n_orders"])
             size_condition = sum(full_book["bid"][top_p].values()) == (
                     top_book["bid_real_qty"] + top_book["bid_impl_qty"])
             if not (price_condition and num_orders_condition and size_condition):
                 problems.append({"synopsys": synopsys(price_condition, num_orders_condition, size_condition),
                                  "side": "bid"})
     else:
```

### Comparing `recon_lw-2.0.0.dev4991603720/setup.py` & `recon_lw-2.0.0.dev4992831728/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4991603720/test/test_recon_ob.py` & `recon_lw-2.0.0.dev4992831728/test/test_recon_ob.py`

 * *Files identical despite different names*

