# Comparing `tmp/pypack-template-1.0.0.tar.gz` & `tmp/pypack-template-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypack-template-1.0.0.tar", last modified: Tue May 16 04:18:11 2023, max compression
+gzip compressed data, was "pypack-template-1.0.1.tar", last modified: Tue May 16 08:20:09 2023, max compression
```

## Comparing `pypack-template-1.0.0.tar` & `pypack-template-1.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 dy         (501) staff       (20)        0 2023-05-16 04:18:11.730751 pypack-template-1.0.0/
--rw-rw-r--   0 dy         (501) staff       (20)     2182 2023-04-19 14:32:12.000000 pypack-template-1.0.0/LICENSE
--rw-r--r--   0 dy         (501) staff       (20)       29 2023-05-16 04:17:50.000000 pypack-template-1.0.0/MANIFEST.in
--rw-r--r--   0 dy         (501) staff       (20)     4394 2023-05-16 04:18:11.730614 pypack-template-1.0.0/PKG-INFO
--rw-rw-r--   0 dy         (501) staff       (20)     1664 2023-05-16 04:14:15.000000 pypack-template-1.0.0/README.md
--rw-rw-r--   0 dy         (501) staff       (20)      507 2023-05-16 03:11:21.000000 pypack-template-1.0.0/pyproject.toml
--rw-r--r--   0 dy         (501) staff       (20)       38 2023-05-16 04:18:11.730795 pypack-template-1.0.0/setup.cfg
--rw-rw-r--   0 dy         (501) staff       (20)      980 2023-05-16 04:11:36.000000 pypack-template-1.0.0/setup.py
-drwxr-xr-x   0 dy         (501) staff       (20)        0 2023-05-16 04:18:11.728070 pypack-template-1.0.0/src/
-drwxr-xr-x   0 dy         (501) staff       (20)        0 2023-05-16 04:18:11.729068 pypack-template-1.0.0/src/pypack/
--rw-r--r--   0 dy         (501) staff       (20)       90 2023-05-16 02:34:01.000000 pypack-template-1.0.0/src/pypack/__init__.py
--rw-r--r--   0 dy         (501) staff       (20)        0 2023-05-15 08:30:45.000000 pypack-template-1.0.0/src/pypack/__main__.py
-drwxr-xr-x   0 dy         (501) staff       (20)        0 2023-05-16 04:18:11.729515 pypack-template-1.0.0/src/pypack/c/
--rw-r--r--   0 dy         (501) staff       (20)     2874 2023-05-15 05:03:42.000000 pypack-template-1.0.0/src/pypack/c/fft.h
--rw-rw-r--   0 dy         (501) staff       (20)      871 2023-05-16 04:02:50.000000 pypack-template-1.0.0/src/pypack/c/main.cpp
--rw-r--r--   0 dy         (501) staff       (20)        0 2023-05-15 08:49:41.000000 pypack-template-1.0.0/src/pypack/convolution.py
-drwxr-xr-x   0 dy         (501) staff       (20)        0 2023-05-16 04:18:11.730285 pypack-template-1.0.0/src/pypack_template.egg-info/
--rw-r--r--   0 dy         (501) staff       (20)     4394 2023-05-16 04:18:11.000000 pypack-template-1.0.0/src/pypack_template.egg-info/PKG-INFO
--rw-r--r--   0 dy         (501) staff       (20)      440 2023-05-16 04:18:11.000000 pypack-template-1.0.0/src/pypack_template.egg-info/SOURCES.txt
--rw-r--r--   0 dy         (501) staff       (20)        1 2023-05-16 04:18:11.000000 pypack-template-1.0.0/src/pypack_template.egg-info/dependency_links.txt
--rw-r--r--   0 dy         (501) staff       (20)       52 2023-05-16 04:18:11.000000 pypack-template-1.0.0/src/pypack_template.egg-info/entry_points.txt
--rw-r--r--   0 dy         (501) staff       (20)       20 2023-05-16 04:18:11.000000 pypack-template-1.0.0/src/pypack_template.egg-info/requires.txt
--rw-r--r--   0 dy         (501) staff       (20)        7 2023-05-16 04:18:11.000000 pypack-template-1.0.0/src/pypack_template.egg-info/top_level.txt
-drwxr-xr-x   0 dy         (501) staff       (20)        0 2023-05-16 04:18:11.730422 pypack-template-1.0.0/tests/
--rw-rw-r--   0 dy         (501) staff       (20)      114 2023-04-19 14:32:12.000000 pypack-template-1.0.0/tests/test.py
+drwxr-xr-x   0 dy         (501) staff       (20)        0 2023-05-16 08:20:09.239153 pypack-template-1.0.1/
+-rw-rw-r--   0 dy         (501) staff       (20)        0 2023-05-16 05:25:27.000000 pypack-template-1.0.1/LICENSE
+-rw-r--r--   0 dy         (501) staff       (20)       29 2023-05-16 04:17:50.000000 pypack-template-1.0.1/MANIFEST.in
+-rw-r--r--   0 dy         (501) staff       (20)      826 2023-05-16 08:20:09.238994 pypack-template-1.0.1/PKG-INFO
+-rw-rw-r--   0 dy         (501) staff       (20)      576 2023-05-16 08:12:30.000000 pypack-template-1.0.1/README.md
+-rw-rw-r--   0 dy         (501) staff       (20)      550 2023-05-16 08:19:32.000000 pypack-template-1.0.1/pyproject.toml
+-rw-r--r--   0 dy         (501) staff       (20)       38 2023-05-16 08:20:09.239204 pypack-template-1.0.1/setup.cfg
+-rw-rw-r--   0 dy         (501) staff       (20)      966 2023-05-16 04:48:25.000000 pypack-template-1.0.1/setup.py
+drwxr-xr-x   0 dy         (501) staff       (20)        0 2023-05-16 08:20:09.236109 pypack-template-1.0.1/src/
+drwxr-xr-x   0 dy         (501) staff       (20)        0 2023-05-16 08:20:09.237225 pypack-template-1.0.1/src/pypack/
+-rw-r--r--   0 dy         (501) staff       (20)       90 2023-05-16 02:34:01.000000 pypack-template-1.0.1/src/pypack/__init__.py
+-rw-r--r--   0 dy         (501) staff       (20)        0 2023-05-15 08:30:45.000000 pypack-template-1.0.1/src/pypack/__main__.py
+drwxr-xr-x   0 dy         (501) staff       (20)        0 2023-05-16 08:20:09.237700 pypack-template-1.0.1/src/pypack/c/
+-rw-r--r--   0 dy         (501) staff       (20)     2874 2023-05-15 05:03:42.000000 pypack-template-1.0.1/src/pypack/c/fft.h
+-rw-rw-r--   0 dy         (501) staff       (20)      871 2023-05-16 04:02:50.000000 pypack-template-1.0.1/src/pypack/c/main.cpp
+-rw-r--r--   0 dy         (501) staff       (20)        0 2023-05-15 08:49:41.000000 pypack-template-1.0.1/src/pypack/convolution.py
+drwxr-xr-x   0 dy         (501) staff       (20)        0 2023-05-16 08:20:09.238545 pypack-template-1.0.1/src/pypack_template.egg-info/
+-rw-r--r--   0 dy         (501) staff       (20)      826 2023-05-16 08:20:09.000000 pypack-template-1.0.1/src/pypack_template.egg-info/PKG-INFO
+-rw-r--r--   0 dy         (501) staff       (20)      440 2023-05-16 08:20:09.000000 pypack-template-1.0.1/src/pypack_template.egg-info/SOURCES.txt
+-rw-r--r--   0 dy         (501) staff       (20)        1 2023-05-16 08:20:09.000000 pypack-template-1.0.1/src/pypack_template.egg-info/dependency_links.txt
+-rw-r--r--   0 dy         (501) staff       (20)       52 2023-05-16 08:20:09.000000 pypack-template-1.0.1/src/pypack_template.egg-info/entry_points.txt
+-rw-r--r--   0 dy         (501) staff       (20)       51 2023-05-16 08:20:09.000000 pypack-template-1.0.1/src/pypack_template.egg-info/requires.txt
+-rw-r--r--   0 dy         (501) staff       (20)        7 2023-05-16 08:20:09.000000 pypack-template-1.0.1/src/pypack_template.egg-info/top_level.txt
+drwxr-xr-x   0 dy         (501) staff       (20)        0 2023-05-16 08:20:09.238672 pypack-template-1.0.1/tests/
+-rw-rw-r--   0 dy         (501) staff       (20)      106 2023-05-16 05:47:15.000000 pypack-template-1.0.1/tests/test.py
```

### Comparing `pypack-template-1.0.0/setup.py` & `pypack-template-1.0.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 package_name = "pypack"
 ext_modules = [
     Pybind11Extension(f"{package_name}.c",
         sorted(glob(f"src/{package_name}/c/*.cpp")),
         # Example: passing in the version to the compiled code
         define_macros = [('VERSION_INFO', 1)],
-        include_dirs = [f"{os.getcwd()}/src/{package_name}/c"],
+        include_dirs = [f"src/{package_name}/c"],
         language = "c++",
         ),
 ]
 setup(
     ext_modules=ext_modules,
     cmdclass={"build_ext": build_ext},
 )
```

### Comparing `pypack-template-1.0.0/src/pypack/c/fft.h` & `pypack-template-1.0.1/src/pypack/c/fft.h`

 * *Files identical despite different names*

### Comparing `pypack-template-1.0.0/src/pypack/c/main.cpp` & `pypack-template-1.0.1/src/pypack/c/main.cpp`

 * *Files identical despite different names*

