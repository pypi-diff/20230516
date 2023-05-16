# Comparing `tmp/recon_lw-2.0.0.dev4989419599.tar.gz` & `tmp/recon_lw-2.0.0.dev4989843192.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev4989419599.tar", last modified: Tue May 16 08:08:27 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev4989843192.tar", last modified: Tue May 16 08:52:43 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev4989419599.tar` & `recon_lw-2.0.0.dev4989843192.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 08:08:27.000000 recon_lw-2.0.0.dev4989419599/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-16 08:07:54.000000 recon_lw-2.0.0.dev4989419599/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-16 08:08:27.000000 recon_lw-2.0.0.dev4989419599/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-16 08:07:54.000000 recon_lw-2.0.0.dev4989419599/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-16 08:08:02.000000 recon_lw-2.0.0.dev4989419599/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 08:08:27.000000 recon_lw-2.0.0.dev4989419599/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-05-16 08:07:54.000000 recon_lw-2.0.0.dev4989419599/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-05-16 08:07:54.000000 recon_lw-2.0.0.dev4989419599/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     2773 2023-05-16 08:07:54.000000 recon_lw-2.0.0.dev4989419599/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-16 08:07:54.000000 recon_lw-2.0.0.dev4989419599/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-05-16 08:07:54.000000 recon_lw-2.0.0.dev4989419599/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    27644 2023-05-16 08:07:54.000000 recon_lw-2.0.0.dev4989419599/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    15433 2023-05-16 08:07:54.000000 recon_lw-2.0.0.dev4989419599/recon_lw/recon_ob_cross_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 08:08:27.000000 recon_lw-2.0.0.dev4989419599/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-16 08:08:27.000000 recon_lw-2.0.0.dev4989419599/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      425 2023-05-16 08:08:27.000000 recon_lw-2.0.0.dev4989419599/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-16 08:08:27.000000 recon_lw-2.0.0.dev4989419599/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-16 08:08:27.000000 recon_lw-2.0.0.dev4989419599/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-16 08:08:27.000000 recon_lw-2.0.0.dev4989419599/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-16 08:07:54.000000 recon_lw-2.0.0.dev4989419599/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-16 08:08:27.000000 recon_lw-2.0.0.dev4989419599/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-16 08:07:54.000000 recon_lw-2.0.0.dev4989419599/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 08:08:27.000000 recon_lw-2.0.0.dev4989419599/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-05-16 08:07:54.000000 recon_lw-2.0.0.dev4989419599/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 08:52:43.000000 recon_lw-2.0.0.dev4989843192/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-16 08:52:11.000000 recon_lw-2.0.0.dev4989843192/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-16 08:52:43.000000 recon_lw-2.0.0.dev4989843192/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-16 08:52:11.000000 recon_lw-2.0.0.dev4989843192/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-16 08:52:19.000000 recon_lw-2.0.0.dev4989843192/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 08:52:43.000000 recon_lw-2.0.0.dev4989843192/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-05-16 08:52:11.000000 recon_lw-2.0.0.dev4989843192/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-05-16 08:52:11.000000 recon_lw-2.0.0.dev4989843192/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2773 2023-05-16 08:52:11.000000 recon_lw-2.0.0.dev4989843192/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-16 08:52:11.000000 recon_lw-2.0.0.dev4989843192/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-05-16 08:52:11.000000 recon_lw-2.0.0.dev4989843192/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27654 2023-05-16 08:52:11.000000 recon_lw-2.0.0.dev4989843192/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15433 2023-05-16 08:52:11.000000 recon_lw-2.0.0.dev4989843192/recon_lw/recon_ob_cross_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 08:52:43.000000 recon_lw-2.0.0.dev4989843192/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-16 08:52:43.000000 recon_lw-2.0.0.dev4989843192/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      425 2023-05-16 08:52:43.000000 recon_lw-2.0.0.dev4989843192/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-16 08:52:43.000000 recon_lw-2.0.0.dev4989843192/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-16 08:52:43.000000 recon_lw-2.0.0.dev4989843192/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-16 08:52:43.000000 recon_lw-2.0.0.dev4989843192/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-16 08:52:11.000000 recon_lw-2.0.0.dev4989843192/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-16 08:52:43.000000 recon_lw-2.0.0.dev4989843192/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-16 08:52:11.000000 recon_lw-2.0.0.dev4989843192/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 08:52:43.000000 recon_lw-2.0.0.dev4989843192/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-05-16 08:52:11.000000 recon_lw-2.0.0.dev4989843192/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev4989419599/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev4989843192/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4989419599/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev4989843192/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4989419599/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev4989843192/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4989419599/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev4989843192/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4989419599/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev4989843192/recon_lw/recon_ob.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,16 @@
                                       event_sequence,
                                       ok=True,
                                       body={"operations": [(op[0], op[2]["messageId"]) for op in operations_batch],
                                             "len(batch)": len(operations_batch),
                                             "len(obs)": len(obs),
                                             "book_id": book_id},
                                       parentId=parent_event["eventId"])
-    dbg_event["attachedMessageIds"] = list({mess["messageId"] for mess in operations_batch})
+    for tupl in operations_batch:
+        dbg_event["attachedMessageIds"].append(tupl[2]["messageId"])
     events.append(dbg_event)
 
     if len(obs) > 1 and aggregate_batch_updates:
         same_side = all(
             obs[i]["body"]["aggr_seq"]["affected_side"] == obs[0]["body"]["aggr_seq"]["affected_side"] for i in
             range(1, len(obs)))
         same_level = all(
```

### Comparing `recon_lw-2.0.0.dev4989419599/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev4989843192/recon_lw/recon_ob_cross_stream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4989419599/setup.py` & `recon_lw-2.0.0.dev4989843192/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4989419599/test/test_recon_ob.py` & `recon_lw-2.0.0.dev4989843192/test/test_recon_ob.py`

 * *Files identical despite different names*

