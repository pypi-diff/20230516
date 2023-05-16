# Comparing `tmp/aiorobonect-0.1.4.tar.gz` & `tmp/aiorobonect-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiorobonect-0.1.4.tar", last modified: Mon May 15 22:34:55 2023, max compression
+gzip compressed data, was "aiorobonect-0.1.5.tar", last modified: Tue May 16 08:49:03 2023, max compression
```

## Comparing `aiorobonect-0.1.4.tar` & `aiorobonect-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:34:55.764088 aiorobonect-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-15 22:34:35.000000 aiorobonect-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-15 22:34:55.764088 aiorobonect-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-15 22:34:35.000000 aiorobonect-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:34:55.764088 aiorobonect-0.1.4/aiorobonect/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-15 22:34:35.000000 aiorobonect-0.1.4/aiorobonect/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1257 2023-05-15 22:34:35.000000 aiorobonect-0.1.4/aiorobonect/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-15 22:34:35.000000 aiorobonect-0.1.4/aiorobonect/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-05-15 22:34:35.000000 aiorobonect-0.1.4/aiorobonect/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-15 22:34:35.000000 aiorobonect-0.1.4/aiorobonect/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:34:55.764088 aiorobonect-0.1.4/aiorobonect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-15 22:34:55.000000 aiorobonect-0.1.4/aiorobonect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-15 22:34:55.000000 aiorobonect-0.1.4/aiorobonect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 22:34:55.000000 aiorobonect-0.1.4/aiorobonect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 22:34:55.000000 aiorobonect-0.1.4/aiorobonect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-15 22:34:55.000000 aiorobonect-0.1.4/aiorobonect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 22:34:55.764088 aiorobonect-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-15 22:34:38.000000 aiorobonect-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:49:03.113573 aiorobonect-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-16 08:48:37.000000 aiorobonect-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-16 08:49:03.113573 aiorobonect-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-16 08:48:37.000000 aiorobonect-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:49:03.113573 aiorobonect-0.1.5/aiorobonect/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-16 08:48:37.000000 aiorobonect-0.1.5/aiorobonect/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1257 2023-05-16 08:48:37.000000 aiorobonect-0.1.5/aiorobonect/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-16 08:48:37.000000 aiorobonect-0.1.5/aiorobonect/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-05-16 08:48:37.000000 aiorobonect-0.1.5/aiorobonect/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-16 08:48:37.000000 aiorobonect-0.1.5/aiorobonect/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:49:03.113573 aiorobonect-0.1.5/aiorobonect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-16 08:49:03.000000 aiorobonect-0.1.5/aiorobonect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-16 08:49:03.000000 aiorobonect-0.1.5/aiorobonect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 08:49:03.000000 aiorobonect-0.1.5/aiorobonect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 08:49:03.000000 aiorobonect-0.1.5/aiorobonect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 08:49:03.000000 aiorobonect-0.1.5/aiorobonect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 08:49:03.113573 aiorobonect-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-16 08:48:40.000000 aiorobonect-0.1.5/setup.py
```

### Comparing `aiorobonect-0.1.4/LICENSE` & `aiorobonect-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aiorobonect-0.1.4/PKG-INFO` & `aiorobonect-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiorobonect
-Version: 0.1.4
+Version: 0.1.5
 Summary: Module to communicate to the Robonect API
 Home-page: https://github.com/geertmeersman/aiorobonect
 Author: Geert Meersman
 Author-email: geertmeersman@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `aiorobonect-0.1.4/README.md` & `aiorobonect-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `aiorobonect-0.1.4/aiorobonect/cli.py` & `aiorobonect-0.1.5/aiorobonect/cli.py`

 * *Files identical despite different names*

### Comparing `aiorobonect-0.1.4/aiorobonect/rest.py` & `aiorobonect-0.1.5/aiorobonect/rest.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         ) as response:
             result = await response.json()
             _LOGGER.debug("Response mower data: %s", response)
             if response.status == 200:
                 result = await response.json()
                 _LOGGER.debug("Result mower data: %s", result)
             if response.status >= 400:
-                self.session_close()
+                await self.session_close()
                 response.raise_for_status()
         if self.transform_json:
             return transform_json_to_single_depth(result)
         return result
 
     async def async_cmds(self, commands=None) -> list[dict]:
         """Send command to mower."""
```

### Comparing `aiorobonect-0.1.4/aiorobonect.egg-info/PKG-INFO` & `aiorobonect-0.1.5/aiorobonect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiorobonect
-Version: 0.1.4
+Version: 0.1.5
 Summary: Module to communicate to the Robonect API
 Home-page: https://github.com/geertmeersman/aiorobonect
 Author: Geert Meersman
 Author-email: geertmeersman@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `aiorobonect-0.1.4/setup.py` & `aiorobonect-0.1.5/setup.py`

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
-    version="v0.1.4",
+    version="v0.1.5",
 )
```

