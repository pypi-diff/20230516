# Comparing `tmp/aiorobonect-0.1.2.tar.gz` & `tmp/aiorobonect-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiorobonect-0.1.2.tar", last modified: Mon May 15 20:29:22 2023, max compression
+gzip compressed data, was "aiorobonect-0.1.3.tar", last modified: Mon May 15 21:35:06 2023, max compression
```

## Comparing `aiorobonect-0.1.2.tar` & `aiorobonect-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:29:22.739138 aiorobonect-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-15 20:29:03.000000 aiorobonect-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-15 20:29:22.739138 aiorobonect-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-15 20:29:03.000000 aiorobonect-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:29:22.739138 aiorobonect-0.1.2/aiorobonect/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-15 20:29:03.000000 aiorobonect-0.1.2/aiorobonect/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1257 2023-05-15 20:29:03.000000 aiorobonect-0.1.2/aiorobonect/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-15 20:29:03.000000 aiorobonect-0.1.2/aiorobonect/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-15 20:29:03.000000 aiorobonect-0.1.2/aiorobonect/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-15 20:29:03.000000 aiorobonect-0.1.2/aiorobonect/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:29:22.739138 aiorobonect-0.1.2/aiorobonect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-15 20:29:22.000000 aiorobonect-0.1.2/aiorobonect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-15 20:29:22.000000 aiorobonect-0.1.2/aiorobonect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 20:29:22.000000 aiorobonect-0.1.2/aiorobonect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 20:29:22.000000 aiorobonect-0.1.2/aiorobonect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-15 20:29:22.000000 aiorobonect-0.1.2/aiorobonect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 20:29:22.739138 aiorobonect-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-15 20:29:06.000000 aiorobonect-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:35:06.435088 aiorobonect-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-15 21:34:42.000000 aiorobonect-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-15 21:35:06.435088 aiorobonect-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-15 21:34:42.000000 aiorobonect-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:35:06.435088 aiorobonect-0.1.3/aiorobonect/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-15 21:34:42.000000 aiorobonect-0.1.3/aiorobonect/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1257 2023-05-15 21:34:42.000000 aiorobonect-0.1.3/aiorobonect/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-15 21:34:42.000000 aiorobonect-0.1.3/aiorobonect/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-05-15 21:34:42.000000 aiorobonect-0.1.3/aiorobonect/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-15 21:34:42.000000 aiorobonect-0.1.3/aiorobonect/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:35:06.435088 aiorobonect-0.1.3/aiorobonect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-15 21:35:06.000000 aiorobonect-0.1.3/aiorobonect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-15 21:35:06.000000 aiorobonect-0.1.3/aiorobonect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 21:35:06.000000 aiorobonect-0.1.3/aiorobonect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 21:35:06.000000 aiorobonect-0.1.3/aiorobonect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-15 21:35:06.000000 aiorobonect-0.1.3/aiorobonect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 21:35:06.435088 aiorobonect-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-15 21:34:45.000000 aiorobonect-0.1.3/setup.py
```

### Comparing `aiorobonect-0.1.2/LICENSE` & `aiorobonect-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aiorobonect-0.1.2/PKG-INFO` & `aiorobonect-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiorobonect
-Version: 0.1.2
+Version: 0.1.3
 Summary: Module to communicate to the Robonect API
 Home-page: https://github.com/geertmeersman/aiorobonect
 Author: Geert Meersman
 Author-email: geertmeersman@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `aiorobonect-0.1.2/README.md` & `aiorobonect-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `aiorobonect-0.1.2/aiorobonect/cli.py` & `aiorobonect-0.1.3/aiorobonect/cli.py`

 * *Files identical despite different names*

### Comparing `aiorobonect-0.1.2/aiorobonect/rest.py` & `aiorobonect-0.1.3/aiorobonect/rest.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,37 +13,52 @@
 
 
 class RobonectClient:
     """Class to communicate with the Robonect API."""
 
     def __init__(self, host, username, password, transform_json=False) -> None:
         """Initialize the Communication API to get data."""
-        auth = None
+        self.auth = None
         self.host = host
+        self.username = username
+        self.password = password
         self.session = None
         self.transform_json = transform_json
         if username is not None and password is not None:
-            auth = aiohttp.BasicAuth(login=username, password=password)
+            self.auth = aiohttp.BasicAuth(login=username, password=password)
             self.session = aiohttp.ClientSession(
-                read_timeout=TIMEOUT, raise_for_status=True, auth=auth
+                read_timeout=TIMEOUT, raise_for_status=True, auth=self.auth
             )
 
+    def session_start(self):
+        """Start the aiohttp session."""
+        if self.session:
+            return True
+        if self.username is not None and self.password is not None:
+            self.session = aiohttp.ClientSession(
+                read_timeout=TIMEOUT, raise_for_status=True, auth=self.auth
+            )
+            return True
+        return False
+
     async def session_close(self):
         """Close the session."""
         await self.session.close()
+        self.session = None
 
     async def async_cmd(self, command=None, params={}) -> list[dict]:
         """Send command to mower."""
         if command is None:
             return False
         params = urllib.parse.urlencode(params)
         if command == "job":
             _LOGGER.debug(f"Job params: {params}")
             return
 
+        self.session_start()
         async with self.session.get(
             f"http://{self.host}/json?cmd={command}&{params}"
         ) as response:
             result = await response.json()
             _LOGGER.debug("Response mower data: %s", response)
             if response.status == 200:
                 result = await response.json()
@@ -52,12 +67,20 @@
                 response.raise_for_status()
         if self.transform_json:
             return transform_json_to_single_depth(result)
         return result
 
     async def async_cmds(self, commands=None) -> list[dict]:
         """Send command to mower."""
+        self.session_start()
         result = []
         for cmd in commands:
             result.append({cmd: await self.async_cmd(cmd)})
         await self.session_close()
         return result
+
+    async def state(self) -> list[dict]:
+        """Send status command to mower."""
+        self.session_start()
+        result = await self.async_cmd("status")
+        await self.session_close()
+        return result
```

### Comparing `aiorobonect-0.1.2/aiorobonect.egg-info/PKG-INFO` & `aiorobonect-0.1.3/aiorobonect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiorobonect
-Version: 0.1.2
+Version: 0.1.3
 Summary: Module to communicate to the Robonect API
 Home-page: https://github.com/geertmeersman/aiorobonect
 Author: Geert Meersman
 Author-email: geertmeersman@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `aiorobonect-0.1.2/setup.py` & `aiorobonect-0.1.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,9 +16,9 @@
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     install_requires=[val.strip() for val in open("requirements.txt")],
-    version="v0.1.2",
+    version="v0.1.3",
 )
```

