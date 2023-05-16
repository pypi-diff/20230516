# Comparing `tmp/aiorobonect-0.1.5.tar.gz` & `tmp/aiorobonect-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiorobonect-0.1.5.tar", last modified: Tue May 16 08:49:03 2023, max compression
+gzip compressed data, was "aiorobonect-0.1.6.tar", last modified: Tue May 16 09:07:34 2023, max compression
```

## Comparing `aiorobonect-0.1.5.tar` & `aiorobonect-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:49:03.113573 aiorobonect-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-16 08:48:37.000000 aiorobonect-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-16 08:49:03.113573 aiorobonect-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-16 08:48:37.000000 aiorobonect-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:49:03.113573 aiorobonect-0.1.5/aiorobonect/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-16 08:48:37.000000 aiorobonect-0.1.5/aiorobonect/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1257 2023-05-16 08:48:37.000000 aiorobonect-0.1.5/aiorobonect/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-16 08:48:37.000000 aiorobonect-0.1.5/aiorobonect/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-05-16 08:48:37.000000 aiorobonect-0.1.5/aiorobonect/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-16 08:48:37.000000 aiorobonect-0.1.5/aiorobonect/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:49:03.113573 aiorobonect-0.1.5/aiorobonect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-16 08:49:03.000000 aiorobonect-0.1.5/aiorobonect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-16 08:49:03.000000 aiorobonect-0.1.5/aiorobonect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 08:49:03.000000 aiorobonect-0.1.5/aiorobonect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 08:49:03.000000 aiorobonect-0.1.5/aiorobonect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 08:49:03.000000 aiorobonect-0.1.5/aiorobonect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 08:49:03.113573 aiorobonect-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-16 08:48:40.000000 aiorobonect-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:07:34.648746 aiorobonect-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-16 09:07:12.000000 aiorobonect-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-16 09:07:34.648746 aiorobonect-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-16 09:07:12.000000 aiorobonect-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:07:34.648746 aiorobonect-0.1.6/aiorobonect/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-16 09:07:12.000000 aiorobonect-0.1.6/aiorobonect/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1257 2023-05-16 09:07:12.000000 aiorobonect-0.1.6/aiorobonect/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-16 09:07:12.000000 aiorobonect-0.1.6/aiorobonect/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-05-16 09:07:12.000000 aiorobonect-0.1.6/aiorobonect/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-16 09:07:12.000000 aiorobonect-0.1.6/aiorobonect/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:07:34.648746 aiorobonect-0.1.6/aiorobonect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-16 09:07:34.000000 aiorobonect-0.1.6/aiorobonect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-16 09:07:34.000000 aiorobonect-0.1.6/aiorobonect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 09:07:34.000000 aiorobonect-0.1.6/aiorobonect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 09:07:34.000000 aiorobonect-0.1.6/aiorobonect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 09:07:34.000000 aiorobonect-0.1.6/aiorobonect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 09:07:34.648746 aiorobonect-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-16 09:07:15.000000 aiorobonect-0.1.6/setup.py
```

### Comparing `aiorobonect-0.1.5/LICENSE` & `aiorobonect-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aiorobonect-0.1.5/PKG-INFO` & `aiorobonect-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiorobonect
-Version: 0.1.5
+Version: 0.1.6
 Summary: Module to communicate to the Robonect API
 Home-page: https://github.com/geertmeersman/aiorobonect
 Author: Geert Meersman
 Author-email: geertmeersman@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `aiorobonect-0.1.5/README.md` & `aiorobonect-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `aiorobonect-0.1.5/aiorobonect/cli.py` & `aiorobonect-0.1.6/aiorobonect/cli.py`

 * *Files identical despite different names*

### Comparing `aiorobonect-0.1.5/aiorobonect/rest.py` & `aiorobonect-0.1.6/aiorobonect/rest.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,26 +21,21 @@
         self.host = host
         self.username = username
         self.password = password
         self.session = None
         self.transform_json = transform_json
         if username is not None and password is not None:
             self.auth = aiohttp.BasicAuth(login=username, password=password)
-            self.session = aiohttp.ClientSession(
-                read_timeout=TIMEOUT, raise_for_status=True, auth=self.auth
-            )
 
     def session_start(self):
         """Start the aiohttp session."""
         if self.session:
             return True
         if self.username is not None and self.password is not None:
-            self.session = aiohttp.ClientSession(
-                read_timeout=TIMEOUT, raise_for_status=True, auth=self.auth
-            )
+            self.session = aiohttp.ClientSession(read_timeout=TIMEOUT, auth=self.auth)
             return True
         return False
 
     async def session_close(self):
         """Close the session."""
         await self.session.close()
         self.session = None
```

### Comparing `aiorobonect-0.1.5/aiorobonect.egg-info/PKG-INFO` & `aiorobonect-0.1.6/aiorobonect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiorobonect
-Version: 0.1.5
+Version: 0.1.6
 Summary: Module to communicate to the Robonect API
 Home-page: https://github.com/geertmeersman/aiorobonect
 Author: Geert Meersman
 Author-email: geertmeersman@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

