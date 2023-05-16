# Comparing `tmp/recon_lw-2.0.0.dev4989950411.tar.gz` & `tmp/recon_lw-2.0.0.dev4990931200.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev4989950411.tar", last modified: Tue May 16 09:03:45 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev4990931200.tar", last modified: Tue May 16 10:46:40 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev4989950411.tar` & `recon_lw-2.0.0.dev4990931200.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 09:03:45.000000 recon_lw-2.0.0.dev4989950411/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-16 09:03:19.000000 recon_lw-2.0.0.dev4989950411/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-16 09:03:45.000000 recon_lw-2.0.0.dev4989950411/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-16 09:03:19.000000 recon_lw-2.0.0.dev4989950411/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-16 09:03:25.000000 recon_lw-2.0.0.dev4989950411/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 09:03:45.000000 recon_lw-2.0.0.dev4989950411/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-05-16 09:03:19.000000 recon_lw-2.0.0.dev4989950411/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-05-16 09:03:19.000000 recon_lw-2.0.0.dev4989950411/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     2773 2023-05-16 09:03:19.000000 recon_lw-2.0.0.dev4989950411/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-16 09:03:19.000000 recon_lw-2.0.0.dev4989950411/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-05-16 09:03:19.000000 recon_lw-2.0.0.dev4989950411/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    27699 2023-05-16 09:03:19.000000 recon_lw-2.0.0.dev4989950411/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    15433 2023-05-16 09:03:19.000000 recon_lw-2.0.0.dev4989950411/recon_lw/recon_ob_cross_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 09:03:45.000000 recon_lw-2.0.0.dev4989950411/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-16 09:03:45.000000 recon_lw-2.0.0.dev4989950411/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      425 2023-05-16 09:03:45.000000 recon_lw-2.0.0.dev4989950411/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-16 09:03:45.000000 recon_lw-2.0.0.dev4989950411/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-16 09:03:45.000000 recon_lw-2.0.0.dev4989950411/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-16 09:03:45.000000 recon_lw-2.0.0.dev4989950411/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-16 09:03:19.000000 recon_lw-2.0.0.dev4989950411/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-16 09:03:45.000000 recon_lw-2.0.0.dev4989950411/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-16 09:03:19.000000 recon_lw-2.0.0.dev4989950411/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 09:03:45.000000 recon_lw-2.0.0.dev4989950411/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-05-16 09:03:19.000000 recon_lw-2.0.0.dev4989950411/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 10:46:40.000000 recon_lw-2.0.0.dev4990931200/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-16 10:46:07.000000 recon_lw-2.0.0.dev4990931200/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-16 10:46:40.000000 recon_lw-2.0.0.dev4990931200/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-16 10:46:07.000000 recon_lw-2.0.0.dev4990931200/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-16 10:46:15.000000 recon_lw-2.0.0.dev4990931200/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 10:46:40.000000 recon_lw-2.0.0.dev4990931200/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-05-16 10:46:07.000000 recon_lw-2.0.0.dev4990931200/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-05-16 10:46:07.000000 recon_lw-2.0.0.dev4990931200/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2773 2023-05-16 10:46:07.000000 recon_lw-2.0.0.dev4990931200/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-16 10:46:07.000000 recon_lw-2.0.0.dev4990931200/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-05-16 10:46:07.000000 recon_lw-2.0.0.dev4990931200/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27696 2023-05-16 10:46:07.000000 recon_lw-2.0.0.dev4990931200/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15433 2023-05-16 10:46:07.000000 recon_lw-2.0.0.dev4990931200/recon_lw/recon_ob_cross_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 10:46:40.000000 recon_lw-2.0.0.dev4990931200/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-16 10:46:40.000000 recon_lw-2.0.0.dev4990931200/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      425 2023-05-16 10:46:40.000000 recon_lw-2.0.0.dev4990931200/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-16 10:46:40.000000 recon_lw-2.0.0.dev4990931200/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-16 10:46:40.000000 recon_lw-2.0.0.dev4990931200/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-16 10:46:40.000000 recon_lw-2.0.0.dev4990931200/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-16 10:46:07.000000 recon_lw-2.0.0.dev4990931200/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-16 10:46:40.000000 recon_lw-2.0.0.dev4990931200/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-16 10:46:07.000000 recon_lw-2.0.0.dev4990931200/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 10:46:40.000000 recon_lw-2.0.0.dev4990931200/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-05-16 10:46:07.000000 recon_lw-2.0.0.dev4990931200/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev4989950411/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev4990931200/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4989950411/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev4990931200/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4989950411/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev4990931200/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4989950411/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev4990931200/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4989950411/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev4990931200/recon_lw/recon_ob.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,40 +144,37 @@
     if len(obs) > 1 and aggregate_batch_updates:
         same_side = all(
             obs[i]["body"]["aggr_seq"]["affected_side"] == obs[0]["body"]["aggr_seq"]["affected_side"] for i in
             range(1, len(obs)))
         same_level = all(
             obs[i]["body"]["aggr_seq"]["affected_level"] == obs[0]["body"]["aggr_seq"]["affected_level"] for i in
             range(1, len(obs)))
-        obs[0]["body"]["debug_batch_updates"] = len(obs)
-        obs[0]["body"]["debug_same_side"] = same_side
-        obs[0]["body"]["debug_same_level"] = same_level
 
-        if same_side:
+        if same_side and obs[0]["body"]["aggr_seq"]["affected_side"] != "na":
             skip_top = 0
             skip_aggr = 0
             for i in range(len(obs) - 1):
                 if obs[i]["body"]["aggr_seq"]["top_delta"] == 1:
                     skip_top += 1
                 obs[i]["body"]["aggr_seq"]["top_delta"] = 0
                 obs[i]["body"]["aggr_seq"]["top_v"] = -1
                 obs[i]["body"]["aggr_seq"]["top_v2"] = -1
 
-                if same_level:
+                if same_level and obs[0]["body"]["aggr_seq"]["affected_side"] != -1:
                     if obs[i]["body"]["aggr_seq"]["limit_delta"] == 1:
                         skip_aggr += 1
                     obs[i]["body"]["aggr_seq"]["limit_delta"] = 0
                     obs[i]["body"]["aggr_seq"]["limit_v"] = -1
                     obs[i]["body"]["aggr_seq"]["limit_v2"] = -1
 
             obs[-1]["body"]["aggr_seq"]["top_delta"] = 1
             obs[-1]["body"]["aggr_seq"]["top_v"] -= skip_top
             obs[-1]["body"]["aggr_seq"]["top_v2"] -= skip_top
 
-            if same_level:
+            if same_level and obs[0]["body"]["aggr_seq"]["affected_side"] != -1:
                 obs[-1]["body"]["aggr_seq"]["limit_delta"] = 1
                 obs[-1]["body"]["aggr_seq"]["limit_v"] -= skip_aggr
                 obs[-1]["body"]["aggr_seq"]["limit_v2"] -= skip_aggr
 
     events.extend(obs)
```

### Comparing `recon_lw-2.0.0.dev4989950411/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev4990931200/recon_lw/recon_ob_cross_stream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4989950411/setup.py` & `recon_lw-2.0.0.dev4990931200/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4989950411/test/test_recon_ob.py` & `recon_lw-2.0.0.dev4990931200/test/test_recon_ob.py`

 * *Files identical despite different names*

