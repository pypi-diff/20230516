# Comparing `tmp/djungle-rulesengine-client-0.3.3.tar.gz` & `tmp/djungle-rulesengine-client-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djungle-rulesengine-client-0.3.3.tar", last modified: Thu May 11 09:45:56 2023, max compression
+gzip compressed data, was "djungle-rulesengine-client-0.4.0.tar", last modified: Tue May 16 09:02:05 2023, max compression
```

## Comparing `djungle-rulesengine-client-0.3.3.tar` & `djungle-rulesengine-client-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:45:56.400789 djungle-rulesengine-client-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-11 09:45:43.000000 djungle-rulesengine-client-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-11 09:45:56.400789 djungle-rulesengine-client-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-11 09:45:43.000000 djungle-rulesengine-client-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-11 09:45:43.000000 djungle-rulesengine-client-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-11 09:45:56.400789 djungle-rulesengine-client-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 09:45:43.000000 djungle-rulesengine-client-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:45:56.396789 djungle-rulesengine-client-0.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:45:56.396789 djungle-rulesengine-client-0.3.3/src/djungle_rulesengine_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-11 09:45:56.000000 djungle-rulesengine-client-0.3.3/src/djungle_rulesengine_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-11 09:45:56.000000 djungle-rulesengine-client-0.3.3/src/djungle_rulesengine_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 09:45:56.000000 djungle-rulesengine-client-0.3.3/src/djungle_rulesengine_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 09:45:56.000000 djungle-rulesengine-client-0.3.3/src/djungle_rulesengine_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-11 09:45:56.000000 djungle-rulesengine-client-0.3.3/src/djungle_rulesengine_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-11 09:45:56.000000 djungle-rulesengine-client-0.3.3/src/djungle_rulesengine_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:45:56.400789 djungle-rulesengine-client-0.3.3/src/rulesengine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 09:45:43.000000 djungle-rulesengine-client-0.3.3/src/rulesengine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-11 09:45:43.000000 djungle-rulesengine-client-0.3.3/src/rulesengine/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:45:56.400789 djungle-rulesengine-client-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9251 2023-05-11 09:45:43.000000 djungle-rulesengine-client-0.3.3/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:02:05.900365 djungle-rulesengine-client-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-16 09:01:57.000000 djungle-rulesengine-client-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-16 09:02:05.900365 djungle-rulesengine-client-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-16 09:01:57.000000 djungle-rulesengine-client-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-16 09:01:57.000000 djungle-rulesengine-client-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-16 09:02:05.900365 djungle-rulesengine-client-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 09:01:57.000000 djungle-rulesengine-client-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:02:05.900365 djungle-rulesengine-client-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:02:05.900365 djungle-rulesengine-client-0.4.0/src/djungle_rulesengine_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-16 09:02:05.000000 djungle-rulesengine-client-0.4.0/src/djungle_rulesengine_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-16 09:02:05.000000 djungle-rulesengine-client-0.4.0/src/djungle_rulesengine_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 09:02:05.000000 djungle-rulesengine-client-0.4.0/src/djungle_rulesengine_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 09:02:05.000000 djungle-rulesengine-client-0.4.0/src/djungle_rulesengine_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-16 09:02:05.000000 djungle-rulesengine-client-0.4.0/src/djungle_rulesengine_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 09:02:05.000000 djungle-rulesengine-client-0.4.0/src/djungle_rulesengine_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:02:05.900365 djungle-rulesengine-client-0.4.0/src/rulesengine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 09:01:57.000000 djungle-rulesengine-client-0.4.0/src/rulesengine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-05-16 09:01:57.000000 djungle-rulesengine-client-0.4.0/src/rulesengine/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-16 09:01:57.000000 djungle-rulesengine-client-0.4.0/src/rulesengine/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:02:05.900365 djungle-rulesengine-client-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9119 2023-05-16 09:01:57.000000 djungle-rulesengine-client-0.4.0/tests/test_async_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9251 2023-05-16 09:01:57.000000 djungle-rulesengine-client-0.4.0/tests/test_client.py
```

### Comparing `djungle-rulesengine-client-0.3.3/LICENSE` & `djungle-rulesengine-client-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `djungle-rulesengine-client-0.3.3/PKG-INFO` & `djungle-rulesengine-client-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djungle-rulesengine-client
-Version: 0.3.3
+Version: 0.4.0
 Summary: A client to Djungle Studio rulesengine API
 Home-page: https://github.com/djungle-io/djungle-rulesengine-client
 Author: Djungle s.r.l.
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -28,28 +28,34 @@
 your `~/.pypirc` file.
 
 Alternatively, push a tag to the `main` branch to make a release
 using GitHub Actions.
 
 ## Usage examples
 ```python
+from rulesengine.async_client import AsyncEngineClient
 from rulesengine.client import EngineClient
 
 engine = EngineClient(base_url="https://example.com", token="abcde")
 
 # To push an action to the engine:
 engine.push_action(subject_id="sys-1", action="my-action", payload={"key": "value"})
 
 # To get a pluggable prop from the engine
 prop_value = engine.get_pluggable_props(subject_id="sys-1", props="my-prop")
 
 # To make a "direct" call to the engine
 return_value = engine.direct_post(
     subject_id="sys-1", path="/my/path/", params={"key": "value"}, data={"my": "payload"}
 )
+
+# To push an action to the engine (async client):
+async_engine = AsyncEngineClient(base_url="https://example.com", token="abcde")
+
+await async_engine.push_action(subject_id="sys-1", action="my-action", payload={"key": "value"})
 ```
 
 MIT License
 
 Copyright (c) 2023 Djungle s.r.l.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `djungle-rulesengine-client-0.3.3/README.md` & `djungle-rulesengine-client-0.4.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -12,22 +12,28 @@
 your `~/.pypirc` file.
 
 Alternatively, push a tag to the `main` branch to make a release
 using GitHub Actions.
 
 ## Usage examples
 ```python
+from rulesengine.async_client import AsyncEngineClient
 from rulesengine.client import EngineClient
 
 engine = EngineClient(base_url="https://example.com", token="abcde")
 
 # To push an action to the engine:
 engine.push_action(subject_id="sys-1", action="my-action", payload={"key": "value"})
 
 # To get a pluggable prop from the engine
 prop_value = engine.get_pluggable_props(subject_id="sys-1", props="my-prop")
 
 # To make a "direct" call to the engine
 return_value = engine.direct_post(
     subject_id="sys-1", path="/my/path/", params={"key": "value"}, data={"my": "payload"}
 )
+
+# To push an action to the engine (async client):
+async_engine = AsyncEngineClient(base_url="https://example.com", token="abcde")
+
+await async_engine.push_action(subject_id="sys-1", action="my-action", payload={"key": "value"})
 ```
```

### Comparing `djungle-rulesengine-client-0.3.3/setup.cfg` & `djungle-rulesengine-client-0.4.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = djungle-rulesengine-client
-version = 0.3.3
+version = 0.4.0
 description = A client to Djungle Studio rulesengine API
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 license = MIT
 license_files = LICENSE
 author = Djungle s.r.l.
 url = https://github.com/djungle-io/djungle-rulesengine-client
@@ -15,14 +15,15 @@
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3 :: Only
 
 [options]
 install_requires = 
 	requests>=2.30.0
+	httpx>=0.24.0
 package_dir = 
 	=src
 packages = find:
 zip_safe = False
 
 [options.packages.find]
 where = src
```

### Comparing `djungle-rulesengine-client-0.3.3/src/djungle_rulesengine_client.egg-info/PKG-INFO` & `djungle-rulesengine-client-0.4.0/src/djungle_rulesengine_client.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djungle-rulesengine-client
-Version: 0.3.3
+Version: 0.4.0
 Summary: A client to Djungle Studio rulesengine API
 Home-page: https://github.com/djungle-io/djungle-rulesengine-client
 Author: Djungle s.r.l.
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -28,28 +28,34 @@
 your `~/.pypirc` file.
 
 Alternatively, push a tag to the `main` branch to make a release
 using GitHub Actions.
 
 ## Usage examples
 ```python
+from rulesengine.async_client import AsyncEngineClient
 from rulesengine.client import EngineClient
 
 engine = EngineClient(base_url="https://example.com", token="abcde")
 
 # To push an action to the engine:
 engine.push_action(subject_id="sys-1", action="my-action", payload={"key": "value"})
 
 # To get a pluggable prop from the engine
 prop_value = engine.get_pluggable_props(subject_id="sys-1", props="my-prop")
 
 # To make a "direct" call to the engine
 return_value = engine.direct_post(
     subject_id="sys-1", path="/my/path/", params={"key": "value"}, data={"my": "payload"}
 )
+
+# To push an action to the engine (async client):
+async_engine = AsyncEngineClient(base_url="https://example.com", token="abcde")
+
+await async_engine.push_action(subject_id="sys-1", action="my-action", payload={"key": "value"})
 ```
 
 MIT License
 
 Copyright (c) 2023 Djungle s.r.l.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `djungle-rulesengine-client-0.3.3/src/rulesengine/client.py` & `djungle-rulesengine-client-0.4.0/src/rulesengine/client.py`

 * *Files identical despite different names*

### Comparing `djungle-rulesengine-client-0.3.3/tests/test_client.py` & `djungle-rulesengine-client-0.4.0/tests/test_client.py`

 * *Files identical despite different names*

