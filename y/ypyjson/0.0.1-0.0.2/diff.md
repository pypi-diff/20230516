# Comparing `tmp/ypyjson-0.0.1.tar.gz` & `tmp/ypyjson-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ypyjson-0.0.1.tar", last modified: Sun May 14 21:31:42 2023, max compression
+gzip compressed data, was "ypyjson-0.0.2.tar", last modified: Mon May 15 22:12:04 2023, max compression
```

## Comparing `ypyjson-0.0.1.tar` & `ypyjson-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 21:31:42.355104 ypyjson-0.0.1/
--rw-rw-rw-   0        0        0     1233 2023-04-29 20:24:32.000000 ypyjson-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     3444 2023-05-14 21:31:42.335039 ypyjson-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3033 2023-05-14 21:18:27.000000 ypyjson-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-14 21:31:42.355104 ypyjson-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1695 2023-05-14 21:30:34.000000 ypyjson-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-14 21:31:42.285038 ypyjson-0.0.1/ypyjson/
--rw-rw-rw-   0        0        0      130 2023-04-29 20:59:59.000000 ypyjson-0.0.1/ypyjson/__init__.py
--rw-rw-rw-   0        0        0   436438 2023-04-29 20:57:20.000000 ypyjson-0.0.1/ypyjson/reader.c
--rw-rw-rw-   0        0        0      801 2023-04-29 19:51:53.000000 ypyjson-0.0.1/ypyjson/reader.pxd
--rw-rw-rw-   0        0        0     3488 2023-04-29 19:50:35.000000 ypyjson-0.0.1/ypyjson/reader.pyi
--rw-rw-rw-   0        0        0    11724 2023-04-29 20:53:50.000000 ypyjson-0.0.1/ypyjson/reader.pyx
--rw-rw-rw-   0        0        0     2607 2023-04-29 19:58:16.000000 ypyjson-0.0.1/ypyjson/ypyflags.py
-drwxrwxrwx   0        0        0        0 2023-05-14 21:31:42.330038 ypyjson-0.0.1/ypyjson/yyjson/
--rw-rw-rw-   0        0        0   322938 2023-04-08 04:44:19.000000 ypyjson-0.0.1/ypyjson/yyjson/yyjson.c
--rw-rw-rw-   0        0        0   243960 2023-04-17 20:29:41.000000 ypyjson-0.0.1/ypyjson/yyjson/yyjson.h
--rw-rw-rw-   0        0        0     3426 2023-04-29 20:52:46.000000 ypyjson-0.0.1/ypyjson/yyr.pxi
-drwxrwxrwx   0        0        0        0 2023-05-14 21:31:42.310038 ypyjson-0.0.1/ypyjson.egg-info/
--rw-rw-rw-   0        0        0     3444 2023-05-14 21:31:40.000000 ypyjson-0.0.1/ypyjson.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2023-05-14 21:31:41.000000 ypyjson-0.0.1/ypyjson.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 21:31:40.000000 ypyjson-0.0.1/ypyjson.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-14 21:31:40.000000 ypyjson-0.0.1/ypyjson.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-15 22:12:04.018081 ypyjson-0.0.2/
+-rw-rw-rw-   0        0        0     1233 2023-04-29 20:24:32.000000 ypyjson-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     3444 2023-05-15 22:12:04.018081 ypyjson-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3033 2023-05-14 21:18:27.000000 ypyjson-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-15 22:12:04.018081 ypyjson-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1651 2023-05-15 22:11:21.000000 ypyjson-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 22:12:03.908080 ypyjson-0.0.2/ypyjson/
+-rw-rw-rw-   0        0        0      130 2023-04-29 20:59:59.000000 ypyjson-0.0.2/ypyjson/__init__.py
+-rw-rw-rw-   0        0        0   436438 2023-04-29 20:57:20.000000 ypyjson-0.0.2/ypyjson/reader.c
+-rw-rw-rw-   0        0        0      801 2023-04-29 19:51:53.000000 ypyjson-0.0.2/ypyjson/reader.pxd
+-rw-rw-rw-   0        0        0     3488 2023-04-29 19:50:35.000000 ypyjson-0.0.2/ypyjson/reader.pyi
+-rw-rw-rw-   0        0        0    11724 2023-04-29 20:53:50.000000 ypyjson-0.0.2/ypyjson/reader.pyx
+-rw-rw-rw-   0        0        0     2607 2023-04-29 19:58:16.000000 ypyjson-0.0.2/ypyjson/ypyflags.py
+drwxrwxrwx   0        0        0        0 2023-05-15 22:12:03.988082 ypyjson-0.0.2/ypyjson/yyjson/
+-rw-rw-rw-   0        0        0   322938 2023-04-08 04:44:19.000000 ypyjson-0.0.2/ypyjson/yyjson/yyjson.c
+-rw-rw-rw-   0        0        0   243960 2023-04-17 20:29:41.000000 ypyjson-0.0.2/ypyjson/yyjson/yyjson.h
+-rw-rw-rw-   0        0        0     3426 2023-04-29 20:52:46.000000 ypyjson-0.0.2/ypyjson/yyr.pxi
+drwxrwxrwx   0        0        0        0 2023-05-15 22:12:03.968081 ypyjson-0.0.2/ypyjson.egg-info/
+-rw-rw-rw-   0        0        0     3444 2023-05-15 22:12:02.000000 ypyjson-0.0.2/ypyjson.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2023-05-15 22:12:03.000000 ypyjson-0.0.2/ypyjson.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 22:12:02.000000 ypyjson-0.0.2/ypyjson.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-15 22:12:02.000000 ypyjson-0.0.2/ypyjson.egg-info/top_level.txt
```

### Comparing `ypyjson-0.0.1/LICENSE.txt` & `ypyjson-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ypyjson-0.0.1/PKG-INFO` & `ypyjson-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ypyjson
-Version: 0.0.1
+Version: 0.0.2
 Summary: yet another python json library using yyjson
 Author: Vizonex
 License: Unlicense
 Keywords: yyjson,ypyjson,json,cython
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `ypyjson-0.0.1/README.md` & `ypyjson-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ypyjson-0.0.1/setup.py` & `ypyjson-0.0.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, Extension, find_packages
 import pathlib
 
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 
 HERE = pathlib.Path("ypyjson")
 long_description = open('README.md').read()
 
 # with open("readme.md","r",encoding="utf-8") as r:
 #     LONG_DESC = r.read()
 
@@ -29,26 +29,23 @@
         author="Vizonex", 
         description="""yet another python json library using yyjson""",
         long_description_content_type='text/markdown',
         long_description=long_description,
         ext_modules = extensions,
         license="Unlicense",
         packages=find_packages(
-            include=['ypyjson'],
-            exclude=['reader.cp39-win_amd64.pyd']
+            include=['ypyjson',"ypyjson/yyjson/yyjson.c","ypyjson/yyjson/yyjson.h"],
+            exclude=['ypyjson/reader.cp39-win_amd64.pyd']
             ),
         # Include cython packages , stub files and yyjson's header file
-        data_files=["ypyjson/reader.pyi",
-                    "ypyjson/yyr.pxi",
-                    "ypyjson/reader.pxd",
-                    "ypyjson/reader.pyx",
-                    "ypyjson/yyjson/yyjson.h"],
+        package_data = {".": ["*.pyi","*.pxi","*.pxd","*.pyx","*.c","*.h"]},
         keywords=["yyjson", "ypyjson", "json", "cython"],
         classifiers=[
             'Programming Language :: Python :: 3.9',
             'Programming Language :: Python :: 3.10',
             'Programming Language :: Python :: 3.11'
-        ]
+        ],
+        include_package_data=True
     )
 
 if __name__ == "__main__":
     main()
```

### Comparing `ypyjson-0.0.1/ypyjson/reader.c` & `ypyjson-0.0.2/ypyjson/reader.c`

 * *Files identical despite different names*

### Comparing `ypyjson-0.0.1/ypyjson/reader.pxd` & `ypyjson-0.0.2/ypyjson/reader.pxd`

 * *Files identical despite different names*

### Comparing `ypyjson-0.0.1/ypyjson/reader.pyi` & `ypyjson-0.0.2/ypyjson/reader.pyi`

 * *Files identical despite different names*

### Comparing `ypyjson-0.0.1/ypyjson/reader.pyx` & `ypyjson-0.0.2/ypyjson/reader.pyx`

 * *Files identical despite different names*

### Comparing `ypyjson-0.0.1/ypyjson/ypyflags.py` & `ypyjson-0.0.2/ypyjson/ypyflags.py`

 * *Files identical despite different names*

### Comparing `ypyjson-0.0.1/ypyjson/yyjson/yyjson.c` & `ypyjson-0.0.2/ypyjson/yyjson/yyjson.c`

 * *Files identical despite different names*

### Comparing `ypyjson-0.0.1/ypyjson/yyjson/yyjson.h` & `ypyjson-0.0.2/ypyjson/yyjson/yyjson.h`

 * *Files identical despite different names*

### Comparing `ypyjson-0.0.1/ypyjson/yyr.pxi` & `ypyjson-0.0.2/ypyjson/yyr.pxi`

 * *Files identical despite different names*

### Comparing `ypyjson-0.0.1/ypyjson.egg-info/PKG-INFO` & `ypyjson-0.0.2/ypyjson.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ypyjson
-Version: 0.0.1
+Version: 0.0.2
 Summary: yet another python json library using yyjson
 Author: Vizonex
 License: Unlicense
 Keywords: yyjson,ypyjson,json,cython
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

