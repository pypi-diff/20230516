# Comparing `tmp/pydivsufsort-0.0.8.tar.gz` & `tmp/pydivsufsort-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydivsufsort-0.0.8.tar", last modified: Sat May 13 15:53:25 2023, max compression
+gzip compressed data, was "pydivsufsort-0.0.9.tar", last modified: Mon May 15 17:23:13 2023, max compression
```

## Comparing `pydivsufsort-0.0.8.tar` & `pydivsufsort-0.0.9.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 15:53:25.403771 pydivsufsort-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-13 15:53:08.000000 pydivsufsort-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-13 15:53:08.000000 pydivsufsort-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-05-13 15:53:25.403771 pydivsufsort-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-05-13 15:53:08.000000 pydivsufsort-0.0.8/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      807 2023-05-13 15:53:08.000000 pydivsufsort-0.0.8/build.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 15:53:25.395771 pydivsufsort-0.0.8/libdivsufsort/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 15:53:08.000000 pydivsufsort-0.0.8/libdivsufsort/.git
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-13 15:53:08.000000 pydivsufsort-0.0.8/libdivsufsort/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-13 15:53:08.000000 pydivsufsort-0.0.8/libdivsufsort/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-05-13 15:53:08.000000 pydivsufsort-0.0.8/libdivsufsort/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 15:53:25.395771 pydivsufsort-0.0.8/libdivsufsort/CMakeModules/
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-13 15:53:08.000000 pydivsufsort-0.0.8/libdivsufsort/CMakeModules/AppendCompilerFlags.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-13 15:53:08.000000 pydivsufsort-0.0.8/libdivsufsort/CMakeModules/CheckFunctionKeywords.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-05-13 15:53:08.000000 pydivsufsort-0.0.8/libdivsufsort/CMakeModules/CheckLFS.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-05-13 15:53:08.000000 pydivsufsort-0.0.8/libdivsufsort/CMakeModules/ProjectCPack.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-13 15:53:08.000000 pydivsufsort-0.0.8/libdivsufsort/CMakeModules/cmake_uninstall.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-13 15:53:08.000000 pydivsufsort-0.0.8/libdivsufsort/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-05-13 15:53:08.000000 pydivsufsort-0.0.8/libdivsufsort/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-13 15:53:08.000000 pydivsufsort-0.0.8/libdivsufsort/VERSION.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 15:53:25.395771 pydivsufsort-0.0.8/libdivsufsort/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-13 15:53:08.000000 pydivsufsort-0.0.8/libdivsufsort/examples/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-05-13 15:53:08.000000 pydivsufsort-0.0.8/libdivsufsort/examples/bwt.c
--rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-05-13 15:53:08.000000 pydivsufsort-0.0.8/libdivsufsort/examples/mksary.c
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-05-13 15:53:08.000000 pydivsufsort-0.0.8/libdivsufsort/examples/sasearch.c
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-05-13 15:53:08.000000 pydivsufsort-0.0.8/libdivsufsort/examples/suftest.c
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-05-13 15:53:08.000000 pydivsufsort-0.0.8/libdivsufsort/examples/unbwt.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 15:53:25.395771 pydivsufsort-0.0.8/libdivsufsort/include/
--rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-05-13 15:53:08.000000 pydivsufsort-0.0.8/libdivsufsort/include/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-13 15:53:08.000000 pydivsufsort-0.0.8/libdivsufsort/include/config.h.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-05-13 15:53:08.000000 pydivsufsort-0.0.8/libdivsufsort/include/divsufsort.h.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-05-13 15:53:08.000000 pydivsufsort-0.0.8/libdivsufsort/include/divsufsort_private.h
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-13 15:53:08.000000 pydivsufsort-0.0.8/libdivsufsort/include/lfs.h.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 15:53:25.399771 pydivsufsort-0.0.8/libdivsufsort/lib/
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-13 15:53:08.000000 pydivsufsort-0.0.8/libdivsufsort/lib/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11728 2023-05-13 15:53:08.000000 pydivsufsort-0.0.8/libdivsufsort/lib/divsufsort.c
--rw-r--r--   0 runner    (1001) docker     (123)    24117 2023-05-13 15:53:08.000000 pydivsufsort-0.0.8/libdivsufsort/lib/sssort.c
--rw-r--r--   0 runner    (1001) docker     (123)    17794 2023-05-13 15:53:08.000000 pydivsufsort-0.0.8/libdivsufsort/lib/trsort.c
--rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-05-13 15:53:08.000000 pydivsufsort-0.0.8/libdivsufsort/lib/utils.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 15:53:25.399771 pydivsufsort-0.0.8/libdivsufsort/pkgconfig/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-13 15:53:08.000000 pydivsufsort-0.0.8/libdivsufsort/pkgconfig/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-13 15:53:08.000000 pydivsufsort-0.0.8/libdivsufsort/pkgconfig/libdivsufsort.pc.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 15:53:25.399771 pydivsufsort-0.0.8/pydivsufsort/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-13 15:53:08.000000 pydivsufsort-0.0.8/pydivsufsort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-05-13 15:53:08.000000 pydivsufsort-0.0.8/pydivsufsort/divsufsort.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-13 15:53:08.000000 pydivsufsort-0.0.8/pydivsufsort/dll.py
--rw-r--r--   0 runner    (1001) docker     (123)  2317232 2023-05-13 15:53:24.000000 pydivsufsort-0.0.8/pydivsufsort/stringalg.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-05-13 15:53:08.000000 pydivsufsort-0.0.8/pydivsufsort/stringalg.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-05-13 15:53:08.000000 pydivsufsort-0.0.8/pydivsufsort/wonderstring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 15:53:25.403771 pydivsufsort-0.0.8/pydivsufsort.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-05-13 15:53:25.000000 pydivsufsort-0.0.8/pydivsufsort.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-13 15:53:25.000000 pydivsufsort-0.0.8/pydivsufsort.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 15:53:25.000000 pydivsufsort-0.0.8/pydivsufsort.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-13 15:53:25.000000 pydivsufsort-0.0.8/pydivsufsort.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-13 15:53:25.000000 pydivsufsort-0.0.8/pydivsufsort.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-13 15:53:08.000000 pydivsufsort-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 15:53:25.403771 pydivsufsort-0.0.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2879 2023-05-13 15:53:08.000000 pydivsufsort-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 15:53:25.403771 pydivsufsort-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-05-13 15:53:08.000000 pydivsufsort-0.0.8/tests/test_correct.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-13 15:53:08.000000 pydivsufsort-0.0.8/tests/test_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:23:13.311941 pydivsufsort-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-15 17:22:56.000000 pydivsufsort-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-15 17:22:56.000000 pydivsufsort-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-05-15 17:23:13.311941 pydivsufsort-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-05-15 17:22:56.000000 pydivsufsort-0.0.9/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      807 2023-05-15 17:22:56.000000 pydivsufsort-0.0.9/build.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:23:13.307942 pydivsufsort-0.0.9/libdivsufsort/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 17:22:56.000000 pydivsufsort-0.0.9/libdivsufsort/.git
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-15 17:22:56.000000 pydivsufsort-0.0.9/libdivsufsort/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-15 17:22:56.000000 pydivsufsort-0.0.9/libdivsufsort/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-05-15 17:22:56.000000 pydivsufsort-0.0.9/libdivsufsort/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:23:13.307942 pydivsufsort-0.0.9/libdivsufsort/CMakeModules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-15 17:22:56.000000 pydivsufsort-0.0.9/libdivsufsort/CMakeModules/AppendCompilerFlags.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-15 17:22:56.000000 pydivsufsort-0.0.9/libdivsufsort/CMakeModules/CheckFunctionKeywords.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-05-15 17:22:56.000000 pydivsufsort-0.0.9/libdivsufsort/CMakeModules/CheckLFS.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-05-15 17:22:56.000000 pydivsufsort-0.0.9/libdivsufsort/CMakeModules/ProjectCPack.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-15 17:22:56.000000 pydivsufsort-0.0.9/libdivsufsort/CMakeModules/cmake_uninstall.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-15 17:22:56.000000 pydivsufsort-0.0.9/libdivsufsort/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-05-15 17:22:56.000000 pydivsufsort-0.0.9/libdivsufsort/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-15 17:22:56.000000 pydivsufsort-0.0.9/libdivsufsort/VERSION.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:23:13.307942 pydivsufsort-0.0.9/libdivsufsort/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-15 17:22:56.000000 pydivsufsort-0.0.9/libdivsufsort/examples/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-05-15 17:22:56.000000 pydivsufsort-0.0.9/libdivsufsort/examples/bwt.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-05-15 17:22:56.000000 pydivsufsort-0.0.9/libdivsufsort/examples/mksary.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-05-15 17:22:56.000000 pydivsufsort-0.0.9/libdivsufsort/examples/sasearch.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-05-15 17:22:56.000000 pydivsufsort-0.0.9/libdivsufsort/examples/suftest.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-05-15 17:22:56.000000 pydivsufsort-0.0.9/libdivsufsort/examples/unbwt.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:23:13.307942 pydivsufsort-0.0.9/libdivsufsort/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-05-15 17:22:56.000000 pydivsufsort-0.0.9/libdivsufsort/include/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-15 17:22:56.000000 pydivsufsort-0.0.9/libdivsufsort/include/config.h.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-05-15 17:22:56.000000 pydivsufsort-0.0.9/libdivsufsort/include/divsufsort.h.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-05-15 17:22:56.000000 pydivsufsort-0.0.9/libdivsufsort/include/divsufsort_private.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-15 17:22:56.000000 pydivsufsort-0.0.9/libdivsufsort/include/lfs.h.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:23:13.307942 pydivsufsort-0.0.9/libdivsufsort/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-15 17:22:56.000000 pydivsufsort-0.0.9/libdivsufsort/lib/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11728 2023-05-15 17:22:56.000000 pydivsufsort-0.0.9/libdivsufsort/lib/divsufsort.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24117 2023-05-15 17:22:56.000000 pydivsufsort-0.0.9/libdivsufsort/lib/sssort.c
+-rw-r--r--   0 runner    (1001) docker     (123)    17794 2023-05-15 17:22:56.000000 pydivsufsort-0.0.9/libdivsufsort/lib/trsort.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-05-15 17:22:56.000000 pydivsufsort-0.0.9/libdivsufsort/lib/utils.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:23:13.307942 pydivsufsort-0.0.9/libdivsufsort/pkgconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-15 17:22:56.000000 pydivsufsort-0.0.9/libdivsufsort/pkgconfig/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-15 17:22:56.000000 pydivsufsort-0.0.9/libdivsufsort/pkgconfig/libdivsufsort.pc.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:23:13.311941 pydivsufsort-0.0.9/pydivsufsort/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-15 17:22:56.000000 pydivsufsort-0.0.9/pydivsufsort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-05-15 17:22:56.000000 pydivsufsort-0.0.9/pydivsufsort/divsufsort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-15 17:22:56.000000 pydivsufsort-0.0.9/pydivsufsort/dll.py
+-rw-r--r--   0 runner    (1001) docker     (123)  2324817 2023-05-15 17:23:12.000000 pydivsufsort-0.0.9/pydivsufsort/stringalg.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10453 2023-05-15 17:22:56.000000 pydivsufsort-0.0.9/pydivsufsort/stringalg.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-05-15 17:22:56.000000 pydivsufsort-0.0.9/pydivsufsort/wonderstring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:23:13.311941 pydivsufsort-0.0.9/pydivsufsort.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-05-15 17:23:13.000000 pydivsufsort-0.0.9/pydivsufsort.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-15 17:23:13.000000 pydivsufsort-0.0.9/pydivsufsort.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 17:23:13.000000 pydivsufsort-0.0.9/pydivsufsort.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-15 17:23:13.000000 pydivsufsort-0.0.9/pydivsufsort.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-15 17:23:13.000000 pydivsufsort-0.0.9/pydivsufsort.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-15 17:22:56.000000 pydivsufsort-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 17:23:13.311941 pydivsufsort-0.0.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2879 2023-05-15 17:22:56.000000 pydivsufsort-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:23:13.311941 pydivsufsort-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-05-15 17:22:56.000000 pydivsufsort-0.0.9/tests/test_correct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-15 17:22:56.000000 pydivsufsort-0.0.9/tests/test_interface.py
```

### Comparing `pydivsufsort-0.0.8/LICENSE` & `pydivsufsort-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pydivsufsort-0.0.8/PKG-INFO` & `pydivsufsort-0.0.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydivsufsort
-Version: 0.0.8
+Version: 0.0.9
 Summary: String algorithms
 Home-page: https://github.com/louisabraham/pydivsufsort
 Author: Louis Abraham
 Author-email: louis.abraham@yahoo.fr
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -12,76 +12,79 @@
 
 [![PyPI
 version](https://badge.fury.io/py/pydivsufsort.svg)](https://badge.fury.io/py/pydivsufsort) [![Downloads](https://pepy.tech/badge/pydivsufsort)](https://pepy.tech/project/pydivsufsort) [![Test](https://github.com/louisabraham/pydivsufsort/actions/workflows/test.yml/badge.svg)](https://github.com/louisabraham/pydivsufsort/actions/workflows/test.yml) [![Build and upload](https://github.com/louisabraham/pydivsufsort/actions/workflows/build-and-upload.yml/badge.svg)](https://github.com/louisabraham/pydivsufsort/actions/workflows/build-and-upload.yml) [![codecov](https://codecov.io/gh/louisabraham/pydivsufsort/branch/master/graph/badge.svg?token=A1BM9U1OLV)](https://codecov.io/gh/louisabraham/pydivsufsort) [![DOI](https://zenodo.org/badge/241137939.svg)](https://zenodo.org/badge/latestdoi/241137939)
 
 # `pydivsufsort`: bindings to libdivsufsort
 
 `pydivsufsort` prebuilds `libdivsufsort` as a shared library and
-includes it in a Python package with bindings.
+includes it in a Python package with bindings. Wheels are built for Linux, macOS and Windows (32 and 64 bits) using `cibuildwheel` and GitHub Actions. Basically, you should be able to install it with `pip install pydivsufsort` on any system and it should work out of the box. If it doesn't, please create an issue.
 
 **Features**:
 
 - bindings to `divsufsort` that return numpy arrays
-- handle almost any integer data type (e.g. `int64`) and not only `char`
-- additional string algorithms
+- handle string, bytes and almost any integer data type (e.g. `int64`) and not only `char`
+- algorithms work even for non char inputs
+- additional string algorithms coded in Cython
 
 ## Installation
 
 On Linux, macOS and Windows:
 
 ```
 python -m pip install pydivsufsort
 ```
 
 We provide precompiled wheels for common systems using `cibuildwheel`, and a source distribution for Unix systems. Manual compilation on Windows might require some tweaking, please create an issue.
 
-## Usage
+## Features
 
-### Using String Inputs
+All methods support string, bytes and numpy array inputs, including datatypes greater than `uint8_t` (e.g. `uint64_t`). Below are the signatures of all methods exposed by `pydivsufsort`. To import a method, just do `from pydivsufsort import method_name`. All methods are documented in the docstrings. You can display them with `help(method_name)`.
+
+A nicer interface to reuse computations lazily is provided in WonderString but currently undocumented. Please create an issue if you are interested.
+
+### Methods exposed from libdivsufsort
+
+- `divsufsort(string)`: suffix array
+- `bw_transform(string)`: Burrows-Wheeler transform
+- `inverse_bw_transform(idx, string)`: inverse Burrows-Wheeler transform
+- `sa_search(string, suffix_array, pattern)`: search for a pattern in a suffix array
+
+
+### Additional string algorithms
+
+- `kasai(string, suffix_array=None)`: LCP array computation (lazily computes the suffix array if not provided)
+- `lcp_segtree(string, suffix_array=None, lcp=None)`: build a segment tree for LCP queries (lazily computes the suffix array and LCP array if not provided)
+- `lcp_query(segtree, queries)`: query a segment tree for LCP queries. Queries are pairs of indices.
+- `levenshtein(string1, string2)`: Levenshtein distance
+- `most_frequent_substrings(lcp, length, limit=0, minimum_count=1)`: most frequent substrings. See the docstring for details.
+- `common_substrings(string1, string2, limit=25)`: common substrings between two strings.
+
+
+### Example usage
 
 ```python
-import numpy as np
 from pydivsufsort import divsufsort, kasai
 
 string_inp = "banana$"
 string_suffix_array = divsufsort(string_inp)
 string_lcp_array = kasai(string_inp, string_suffix_array)
 print(string_suffix_array, string_lcp_array)
 # [6 5 3 1 0 4 2] [0 1 3 0 0 2 0]
-```
 
-### Using Integer Inputs
+# You can also convert the string input to integers first
 
-```python
 import numpy as np
-from pydivsufsort import divsufsort, kasai
-
-string_inp = "banana$"
 
-# Convert the string input to integers first
 int_inp = np.unique(np.array(list(string_inp)), return_inverse=True)[1]
 int_suffix_array = divsufsort(int_inp)
 int_lcp_array = kasai(int_inp, int_suffix_array)
 print(int_suffix_array, int_lcp_array)
 # [6 5 3 1 0 4 2] [0 1 3 0 0 2 0]
 ```
 
-### Using Multiple Sentinel Characters Witin A String
-
-```python
-import numpy as np
-from pydivsufsort import divsufsort, kasai
-
-sentinel_inp = "a$banana#and@a*bandana+"
-sentinel_suffix_array = divsufsort(sentinel_inp)
-sentinel_lcp_array = kasai(sentinel_inp, sentinel_suffix_array)
-print(sentinel_suffix_array, sentinel_lcp_array)
-# [ 8  1 14 22 12  7  0 13 21  5 19  3  9 16  2 15 11 18  6 20  4 10 17] [0 0 0 0 0 1 1 1 1 3 3 2 3 0 3 0 1 0 2 2 1 2 0]
-```
-
 
 ## Development
 
 You can install locally with
 
 ```
 pip install -e .
```

### Comparing `pydivsufsort-0.0.8/README.md` & `pydivsufsort-0.0.9/pydivsufsort.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,329 +1,425 @@
-00000000: 5b21 5b50 7950 490a 7665 7273 696f 6e5d  [![PyPI.version]
-00000010: 2868 7474 7073 3a2f 2f62 6164 6765 2e66  (https://badge.f
-00000020: 7572 792e 696f 2f70 792f 7079 6469 7673  ury.io/py/pydivs
-00000030: 7566 736f 7274 2e73 7667 295d 2868 7474  ufsort.svg)](htt
-00000040: 7073 3a2f 2f62 6164 6765 2e66 7572 792e  ps://badge.fury.
-00000050: 696f 2f70 792f 7079 6469 7673 7566 736f  io/py/pydivsufso
-00000060: 7274 2920 5b21 5b44 6f77 6e6c 6f61 6473  rt) [![Downloads
-00000070: 5d28 6874 7470 733a 2f2f 7065 7079 2e74  ](https://pepy.t
-00000080: 6563 682f 6261 6467 652f 7079 6469 7673  ech/badge/pydivs
-00000090: 7566 736f 7274 295d 2868 7474 7073 3a2f  ufsort)](https:/
-000000a0: 2f70 6570 792e 7465 6368 2f70 726f 6a65  /pepy.tech/proje
-000000b0: 6374 2f70 7964 6976 7375 6673 6f72 7429  ct/pydivsufsort)
-000000c0: 205b 215b 5465 7374 5d28 6874 7470 733a   [![Test](https:
-000000d0: 2f2f 6769 7468 7562 2e63 6f6d 2f6c 6f75  //github.com/lou
-000000e0: 6973 6162 7261 6861 6d2f 7079 6469 7673  isabraham/pydivs
-000000f0: 7566 736f 7274 2f61 6374 696f 6e73 2f77  ufsort/actions/w
-00000100: 6f72 6b66 6c6f 7773 2f74 6573 742e 796d  orkflows/test.ym
-00000110: 6c2f 6261 6467 652e 7376 6729 5d28 6874  l/badge.svg)](ht
-00000120: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000130: 2f6c 6f75 6973 6162 7261 6861 6d2f 7079  /louisabraham/py
-00000140: 6469 7673 7566 736f 7274 2f61 6374 696f  divsufsort/actio
-00000150: 6e73 2f77 6f72 6b66 6c6f 7773 2f74 6573  ns/workflows/tes
-00000160: 742e 796d 6c29 205b 215b 4275 696c 6420  t.yml) [![Build 
-00000170: 616e 6420 7570 6c6f 6164 5d28 6874 7470  and upload](http
-00000180: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6c  s://github.com/l
-00000190: 6f75 6973 6162 7261 6861 6d2f 7079 6469  ouisabraham/pydi
-000001a0: 7673 7566 736f 7274 2f61 6374 696f 6e73  vsufsort/actions
-000001b0: 2f77 6f72 6b66 6c6f 7773 2f62 7569 6c64  /workflows/build
-000001c0: 2d61 6e64 2d75 706c 6f61 642e 796d 6c2f  -and-upload.yml/
-000001d0: 6261 6467 652e 7376 6729 5d28 6874 7470  badge.svg)](http
-000001e0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6c  s://github.com/l
-000001f0: 6f75 6973 6162 7261 6861 6d2f 7079 6469  ouisabraham/pydi
-00000200: 7673 7566 736f 7274 2f61 6374 696f 6e73  vsufsort/actions
-00000210: 2f77 6f72 6b66 6c6f 7773 2f62 7569 6c64  /workflows/build
-00000220: 2d61 6e64 2d75 706c 6f61 642e 796d 6c29  -and-upload.yml)
-00000230: 205b 215b 636f 6465 636f 765d 2868 7474   [![codecov](htt
-00000240: 7073 3a2f 2f63 6f64 6563 6f76 2e69 6f2f  ps://codecov.io/
-00000250: 6768 2f6c 6f75 6973 6162 7261 6861 6d2f  gh/louisabraham/
-00000260: 7079 6469 7673 7566 736f 7274 2f62 7261  pydivsufsort/bra
-00000270: 6e63 682f 6d61 7374 6572 2f67 7261 7068  nch/master/graph
-00000280: 2f62 6164 6765 2e73 7667 3f74 6f6b 656e  /badge.svg?token
-00000290: 3d41 3142 4d39 5531 4f4c 5629 5d28 6874  =A1BM9U1OLV)](ht
-000002a0: 7470 733a 2f2f 636f 6465 636f 762e 696f  tps://codecov.io
-000002b0: 2f67 682f 6c6f 7569 7361 6272 6168 616d  /gh/louisabraham
-000002c0: 2f70 7964 6976 7375 6673 6f72 7429 205b  /pydivsufsort) [
-000002d0: 215b 444f 495d 2868 7474 7073 3a2f 2f7a  ![DOI](https://z
-000002e0: 656e 6f64 6f2e 6f72 672f 6261 6467 652f  enodo.org/badge/
-000002f0: 3234 3131 3337 3933 392e 7376 6729 5d28  241137939.svg)](
-00000300: 6874 7470 733a 2f2f 7a65 6e6f 646f 2e6f  https://zenodo.o
-00000310: 7267 2f62 6164 6765 2f6c 6174 6573 7464  rg/badge/latestd
-00000320: 6f69 2f32 3431 3133 3739 3339 290a 0a23  oi/241137939)..#
-00000330: 2060 7079 6469 7673 7566 736f 7274 603a   `pydivsufsort`:
-00000340: 2062 696e 6469 6e67 7320 746f 206c 6962   bindings to lib
-00000350: 6469 7673 7566 736f 7274 0a0a 6070 7964  divsufsort..`pyd
-00000360: 6976 7375 6673 6f72 7460 2070 7265 6275  ivsufsort` prebu
-00000370: 696c 6473 2060 6c69 6264 6976 7375 6673  ilds `libdivsufs
-00000380: 6f72 7460 2061 7320 6120 7368 6172 6564  ort` as a shared
-00000390: 206c 6962 7261 7279 2061 6e64 0a69 6e63   library and.inc
-000003a0: 6c75 6465 7320 6974 2069 6e20 6120 5079  ludes it in a Py
-000003b0: 7468 6f6e 2070 6163 6b61 6765 2077 6974  thon package wit
-000003c0: 6820 6269 6e64 696e 6773 2e0a 0a2a 2a46  h bindings...**F
-000003d0: 6561 7475 7265 732a 2a3a 0a0a 2d20 6269  eatures**:..- bi
-000003e0: 6e64 696e 6773 2074 6f20 6064 6976 7375  ndings to `divsu
-000003f0: 6673 6f72 7460 2074 6861 7420 7265 7475  fsort` that retu
-00000400: 726e 206e 756d 7079 2061 7272 6179 730a  rn numpy arrays.
-00000410: 2d20 6861 6e64 6c65 2061 6c6d 6f73 7420  - handle almost 
-00000420: 616e 7920 696e 7465 6765 7220 6461 7461  any integer data
-00000430: 2074 7970 6520 2865 2e67 2e20 6069 6e74   type (e.g. `int
-00000440: 3634 6029 2061 6e64 206e 6f74 206f 6e6c  64`) and not onl
-00000450: 7920 6063 6861 7260 0a2d 2061 6464 6974  y `char`.- addit
-00000460: 696f 6e61 6c20 7374 7269 6e67 2061 6c67  ional string alg
-00000470: 6f72 6974 686d 730a 0a23 2320 496e 7374  orithms..## Inst
-00000480: 616c 6c61 7469 6f6e 0a0a 4f6e 204c 696e  allation..On Lin
-00000490: 7578 2c20 6d61 634f 5320 616e 6420 5769  ux, macOS and Wi
-000004a0: 6e64 6f77 733a 0a0a 6060 600a 7079 7468  ndows:..```.pyth
-000004b0: 6f6e 202d 6d20 7069 7020 696e 7374 616c  on -m pip instal
-000004c0: 6c20 7079 6469 7673 7566 736f 7274 0a60  l pydivsufsort.`
-000004d0: 6060 0a0a 5765 2070 726f 7669 6465 2070  ``..We provide p
-000004e0: 7265 636f 6d70 696c 6564 2077 6865 656c  recompiled wheel
-000004f0: 7320 666f 7220 636f 6d6d 6f6e 2073 7973  s for common sys
-00000500: 7465 6d73 2075 7369 6e67 2060 6369 6275  tems using `cibu
-00000510: 696c 6477 6865 656c 602c 2061 6e64 2061  ildwheel`, and a
-00000520: 2073 6f75 7263 6520 6469 7374 7269 6275   source distribu
-00000530: 7469 6f6e 2066 6f72 2055 6e69 7820 7379  tion for Unix sy
-00000540: 7374 656d 732e 204d 616e 7561 6c20 636f  stems. Manual co
-00000550: 6d70 696c 6174 696f 6e20 6f6e 2057 696e  mpilation on Win
-00000560: 646f 7773 206d 6967 6874 2072 6571 7569  dows might requi
-00000570: 7265 2073 6f6d 6520 7477 6561 6b69 6e67  re some tweaking
-00000580: 2c20 706c 6561 7365 2063 7265 6174 6520  , please create 
-00000590: 616e 2069 7373 7565 2e0a 0a23 2320 5573  an issue...## Us
-000005a0: 6167 650a 0a23 2323 2055 7369 6e67 2053  age..### Using S
-000005b0: 7472 696e 6720 496e 7075 7473 0a0a 6060  tring Inputs..``
-000005c0: 6070 7974 686f 6e0a 696d 706f 7274 206e  `python.import n
-000005d0: 756d 7079 2061 7320 6e70 0a66 726f 6d20  umpy as np.from 
-000005e0: 7079 6469 7673 7566 736f 7274 2069 6d70  pydivsufsort imp
-000005f0: 6f72 7420 6469 7673 7566 736f 7274 2c20  ort divsufsort, 
-00000600: 6b61 7361 690a 0a73 7472 696e 675f 696e  kasai..string_in
-00000610: 7020 3d20 2262 616e 616e 6124 220a 7374  p = "banana$".st
-00000620: 7269 6e67 5f73 7566 6669 785f 6172 7261  ring_suffix_arra
-00000630: 7920 3d20 6469 7673 7566 736f 7274 2873  y = divsufsort(s
-00000640: 7472 696e 675f 696e 7029 0a73 7472 696e  tring_inp).strin
-00000650: 675f 6c63 705f 6172 7261 7920 3d20 6b61  g_lcp_array = ka
-00000660: 7361 6928 7374 7269 6e67 5f69 6e70 2c20  sai(string_inp, 
-00000670: 7374 7269 6e67 5f73 7566 6669 785f 6172  string_suffix_ar
-00000680: 7261 7929 0a70 7269 6e74 2873 7472 696e  ray).print(strin
-00000690: 675f 7375 6666 6978 5f61 7272 6179 2c20  g_suffix_array, 
-000006a0: 7374 7269 6e67 5f6c 6370 5f61 7272 6179  string_lcp_array
-000006b0: 290a 2320 5b36 2035 2033 2031 2030 2034  ).# [6 5 3 1 0 4
-000006c0: 2032 5d20 5b30 2031 2033 2030 2030 2032   2] [0 1 3 0 0 2
-000006d0: 2030 5d0a 6060 600a 0a23 2323 2055 7369   0].```..### Usi
-000006e0: 6e67 2049 6e74 6567 6572 2049 6e70 7574  ng Integer Input
-000006f0: 730a 0a60 6060 7079 7468 6f6e 0a69 6d70  s..```python.imp
-00000700: 6f72 7420 6e75 6d70 7920 6173 206e 700a  ort numpy as np.
-00000710: 6672 6f6d 2070 7964 6976 7375 6673 6f72  from pydivsufsor
-00000720: 7420 696d 706f 7274 2064 6976 7375 6673  t import divsufs
-00000730: 6f72 742c 206b 6173 6169 0a0a 7374 7269  ort, kasai..stri
-00000740: 6e67 5f69 6e70 203d 2022 6261 6e61 6e61  ng_inp = "banana
-00000750: 2422 0a0a 2320 436f 6e76 6572 7420 7468  $"..# Convert th
-00000760: 6520 7374 7269 6e67 2069 6e70 7574 2074  e string input t
-00000770: 6f20 696e 7465 6765 7273 2066 6972 7374  o integers first
-00000780: 0a69 6e74 5f69 6e70 203d 206e 702e 756e  .int_inp = np.un
-00000790: 6971 7565 286e 702e 6172 7261 7928 6c69  ique(np.array(li
-000007a0: 7374 2873 7472 696e 675f 696e 7029 292c  st(string_inp)),
-000007b0: 2072 6574 7572 6e5f 696e 7665 7273 653d   return_inverse=
-000007c0: 5472 7565 295b 315d 0a69 6e74 5f73 7566  True)[1].int_suf
-000007d0: 6669 785f 6172 7261 7920 3d20 6469 7673  fix_array = divs
-000007e0: 7566 736f 7274 2869 6e74 5f69 6e70 290a  ufsort(int_inp).
-000007f0: 696e 745f 6c63 705f 6172 7261 7920 3d20  int_lcp_array = 
-00000800: 6b61 7361 6928 696e 745f 696e 702c 2069  kasai(int_inp, i
-00000810: 6e74 5f73 7566 6669 785f 6172 7261 7929  nt_suffix_array)
-00000820: 0a70 7269 6e74 2869 6e74 5f73 7566 6669  .print(int_suffi
-00000830: 785f 6172 7261 792c 2069 6e74 5f6c 6370  x_array, int_lcp
-00000840: 5f61 7272 6179 290a 2320 5b36 2035 2033  _array).# [6 5 3
-00000850: 2031 2030 2034 2032 5d20 5b30 2031 2033   1 0 4 2] [0 1 3
-00000860: 2030 2030 2032 2030 5d0a 6060 600a 0a23   0 0 2 0].```..#
-00000870: 2323 2055 7369 6e67 204d 756c 7469 706c  ## Using Multipl
-00000880: 6520 5365 6e74 696e 656c 2043 6861 7261  e Sentinel Chara
-00000890: 6374 6572 7320 5769 7469 6e20 4120 5374  cters Witin A St
-000008a0: 7269 6e67 0a0a 6060 6070 7974 686f 6e0a  ring..```python.
-000008b0: 696d 706f 7274 206e 756d 7079 2061 7320  import numpy as 
-000008c0: 6e70 0a66 726f 6d20 7079 6469 7673 7566  np.from pydivsuf
-000008d0: 736f 7274 2069 6d70 6f72 7420 6469 7673  sort import divs
-000008e0: 7566 736f 7274 2c20 6b61 7361 690a 0a73  ufsort, kasai..s
-000008f0: 656e 7469 6e65 6c5f 696e 7020 3d20 2261  entinel_inp = "a
-00000900: 2462 616e 616e 6123 616e 6440 612a 6261  $banana#and@a*ba
-00000910: 6e64 616e 612b 220a 7365 6e74 696e 656c  ndana+".sentinel
-00000920: 5f73 7566 6669 785f 6172 7261 7920 3d20  _suffix_array = 
-00000930: 6469 7673 7566 736f 7274 2873 656e 7469  divsufsort(senti
-00000940: 6e65 6c5f 696e 7029 0a73 656e 7469 6e65  nel_inp).sentine
-00000950: 6c5f 6c63 705f 6172 7261 7920 3d20 6b61  l_lcp_array = ka
-00000960: 7361 6928 7365 6e74 696e 656c 5f69 6e70  sai(sentinel_inp
-00000970: 2c20 7365 6e74 696e 656c 5f73 7566 6669  , sentinel_suffi
-00000980: 785f 6172 7261 7929 0a70 7269 6e74 2873  x_array).print(s
-00000990: 656e 7469 6e65 6c5f 7375 6666 6978 5f61  entinel_suffix_a
-000009a0: 7272 6179 2c20 7365 6e74 696e 656c 5f6c  rray, sentinel_l
-000009b0: 6370 5f61 7272 6179 290a 2320 5b20 3820  cp_array).# [ 8 
-000009c0: 2031 2031 3420 3232 2031 3220 2037 2020   1 14 22 12  7  
-000009d0: 3020 3133 2032 3120 2035 2031 3920 2033  0 13 21  5 19  3
-000009e0: 2020 3920 3136 2020 3220 3135 2031 3120    9 16  2 15 11 
-000009f0: 3138 2020 3620 3230 2020 3420 3130 2031  18  6 20  4 10 1
-00000a00: 375d 205b 3020 3020 3020 3020 3020 3120  7] [0 0 0 0 0 1 
-00000a10: 3120 3120 3120 3320 3320 3220 3320 3020  1 1 1 3 3 2 3 0 
-00000a20: 3320 3020 3120 3020 3220 3220 3120 3220  3 0 1 0 2 2 1 2 
-00000a30: 305d 0a60 6060 0a0a 0a23 2320 4465 7665  0].```...## Deve
-00000a40: 6c6f 706d 656e 740a 0a59 6f75 2063 616e  lopment..You can
-00000a50: 2069 6e73 7461 6c6c 206c 6f63 616c 6c79   install locally
-00000a60: 2077 6974 680a 0a60 6060 0a70 6970 2069   with..```.pip i
-00000a70: 6e73 7461 6c6c 202d 6520 2e0a 6060 600a  nstall -e ..```.
-00000a80: 0a41 2075 7365 6675 6c20 636f 6d6d 616e  .A useful comman
-00000a90: 6420 746f 2069 7465 7261 7465 2071 7569  d to iterate qui
-00000aa0: 636b 6c79 2077 6865 6e20 6368 616e 6769  ckly when changi
-00000ab0: 6e67 2043 7974 686f 6e20 636f 6465 2069  ng Cython code i
-00000ac0: 730a 0a60 6060 0a70 7974 686f 6e20 7365  s..```.python se
-00000ad0: 7475 702e 7079 2062 7569 6c64 5f65 7874  tup.py build_ext
-00000ae0: 202d 2d69 6e70 6c61 6365 2026 2620 7079   --inplace && py
-00000af0: 7465 7374 202d 730a 6060 600a 0a23 2323  test -s.```..###
-00000b00: 2050 726f 6669 6c69 6e67 0a0a 5072 6f66   Profiling..Prof
-00000b10: 696c 696e 6720 6361 6e20 6265 2061 6374  iling can be act
-00000b20: 6976 6174 6564 2077 6974 6820 7468 6520  ivated with the 
-00000b30: 656e 7669 726f 6e6d 656e 7420 7661 7269  environment vari
-00000b40: 6162 6c65 2060 5052 4f46 494c 4560 3a0a  able `PROFILE`:.
-00000b50: 0a60 6060 0a50 524f 4649 4c45 3d31 2070  .```.PROFILE=1 p
-00000b60: 7974 686f 6e20 7365 7475 702e 7079 2062  ython setup.py b
-00000b70: 7569 6c64 5f65 7874 202d 2d69 6e70 6c61  uild_ext --inpla
-00000b80: 6365 2026 2620 7079 7465 7374 202d 730a  ce && pytest -s.
-00000b90: 6060 600a 0a48 6572 6520 6973 2061 6e20  ```..Here is an 
-00000ba0: 6578 616d 706c 6520 7769 7468 206c 696e  example with lin
-00000bb0: 655f 7072 6f66 696c 6572 2028 7265 7175  e_profiler (requ
-00000bc0: 6972 6573 2060 7069 7020 696e 7374 616c  ires `pip instal
-00000bd0: 6c20 226c 696e 655f 7072 6f66 696c 6572  l "line_profiler
-00000be0: 3c34 2260 293a 0a0a 6060 600a 696d 706f  <4"`):..```.impo
-00000bf0: 7274 206c 696e 655f 7072 6f66 696c 6572  rt line_profiler
-00000c00: 0a66 726f 6d20 7079 6469 7673 7566 736f  .from pydivsufso
-00000c10: 7274 2069 6d70 6f72 7420 636f 6d6d 6f6e  rt import common
-00000c20: 5f73 7562 7374 7269 6e67 730a 6672 6f6d  _substrings.from
-00000c30: 2070 7964 6976 7375 6673 6f72 742e 7374   pydivsufsort.st
-00000c40: 7269 6e67 616c 6720 696d 706f 7274 2028  ringalg import (
-00000c50: 0a20 2020 205f 636f 6d6d 6f6e 5f73 7562  .    _common_sub
-00000c60: 7374 7269 6e67 732c 0a20 2020 2072 6570  strings,.    rep
-00000c70: 6561 7465 645f 7375 6273 7472 696e 6773  eated_substrings
-00000c80: 2c0a 290a 0a73 3120 3d20 2262 616e 616e  ,.)..s1 = "banan
-00000c90: 6122 202a 2031 3030 3030 0a73 3220 3d20  a" * 10000.s2 = 
-00000ca0: 2261 6e61 6e61 7322 202a 2031 3030 3030  "ananas" * 10000
-00000cb0: 0a0a 6675 6e63 203d 2063 6f6d 6d6f 6e5f  ..func = common_
-00000cc0: 7375 6273 7472 696e 6773 0a70 726f 6669  substrings.profi
-00000cd0: 6c65 203d 206c 696e 655f 7072 6f66 696c  le = line_profil
-00000ce0: 6572 2e4c 696e 6550 726f 6669 6c65 7228  er.LineProfiler(
-00000cf0: 6675 6e63 290a 7072 6f66 696c 652e 6164  func).profile.ad
-00000d00: 645f 6675 6e63 7469 6f6e 285f 636f 6d6d  d_function(_comm
-00000d10: 6f6e 5f73 7562 7374 7269 6e67 7329 0a70  on_substrings).p
-00000d20: 726f 6669 6c65 2e61 6464 5f66 756e 6374  rofile.add_funct
-00000d30: 696f 6e28 7265 7065 6174 6564 5f73 7562  ion(repeated_sub
-00000d40: 7374 7269 6e67 7329 0a70 726f 6669 6c65  strings).profile
-00000d50: 2e72 756e 6361 6c6c 2866 756e 632c 2073  .runcall(func, s
-00000d60: 312c 2073 322c 206c 696d 6974 3d31 3529  1, s2, limit=15)
-00000d70: 0a70 726f 6669 6c65 2e70 7269 6e74 5f73  .profile.print_s
-00000d80: 7461 7473 2829 0a60 6060 0a0a 2323 2054  tats().```..## T
-00000d90: 6573 7469 6e67 0a0a 6060 600a 7079 7465  esting..```.pyte
-00000da0: 7374 0a60 6060 0a0a 2323 2054 6563 686e  st.```..## Techn
-00000db0: 6963 616c 2064 6574 6169 6c73 2028 666f  ical details (fo
-00000dc0: 7220 7065 7266 6f72 6d61 6e63 6520 7477  r performance tw
-00000dd0: 6561 6b73 290a 0a60 6c69 6264 6976 7375  eaks)..`libdivsu
-00000de0: 6673 6f72 7460 2069 7320 636f 6d70 696c  fsort` is compil
-00000df0: 6564 2069 6e20 626f 7468 2033 3220 616e  ed in both 32 an
-00000e00: 6420 3634 2062 6974 732c 2061 7320 5b74  d 64 bits, as [t
-00000e10: 6865 2033 3220 6269 7473 2076 6572 7369  he 32 bits versi
-00000e20: 6f6e 2069 7320 6661 7374 6572 5d28 6874  on is faster](ht
-00000e30: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000e40: 2f79 2d32 3536 2f6c 6962 6469 7673 7566  /y-256/libdivsuf
-00000e50: 736f 7274 2f69 7373 7565 732f 3231 292e  sort/issues/21).
-00000e60: 2060 7079 6469 7673 7566 736f 7274 6020   `pydivsufsort` 
-00000e70: 6175 746f 6d61 7469 6361 6c6c 7920 6368  automatically ch
-00000e80: 6f6f 7365 7320 746f 2075 7365 2074 6865  ooses to use the
-00000e90: 2033 3220 6269 7473 2076 6572 7369 6f6e   32 bits version
-00000ea0: 2077 6865 6e20 706f 7373 6962 6c65 2028   when possible (
-00000eb0: 616b 6120 7768 656e 2074 6865 2069 6e70  aka when the inp
-00000ec0: 7574 2073 697a 6520 6973 206c 6573 7320  ut size is less 
-00000ed0: 7468 616e 2060 322a 2a33 312d 3160 292e  than `2**31-1`).
-00000ee0: 0a0a 466f 7220 6265 7374 2070 6572 666f  ..For best perfo
-00000ef0: 726d 616e 6365 2c20 7573 6520 636f 6e74  rmance, use cont
-00000f00: 6967 756f 7573 2061 7272 6179 732e 2049  iguous arrays. I
-00000f10: 6620 796f 7520 6861 7665 2061 2073 6c69  f you have a sli
-00000f20: 6365 6420 6172 7261 792c 2070 7964 6976  ced array, pydiv
-00000f30: 7375 6673 6f72 7420 636f 6e76 6572 7473  sufsort converts
-00000f40: 2069 7420 6175 746f 6d61 7469 6361 6c6c   it automaticall
-00000f50: 7920 7769 7468 205b 606e 756d 7079 2e61  y with [`numpy.a
-00000f60: 7363 6f6e 7469 6775 6f75 7361 7272 6179  scontiguousarray
-00000f70: 605d 2868 7474 7073 3a2f 2f64 6f63 732e  `](https://docs.
-00000f80: 7363 6970 792e 6f72 672f 646f 632f 6e75  scipy.org/doc/nu
-00000f90: 6d70 792f 7265 6665 7265 6e63 652f 6765  mpy/reference/ge
-00000fa0: 6e65 7261 7465 642f 6e75 6d70 792e 6173  nerated/numpy.as
-00000fb0: 636f 6e74 6967 756f 7573 6172 7261 792e  contiguousarray.
-00000fc0: 6874 6d6c 292e 0a0a 5468 6520 7072 6563  html)...The prec
-00000fd0: 6f6d 7069 6c65 6420 6c69 6272 6172 6965  ompiled librarie
-00000fe0: 7320 7573 6520 4f70 656e 4d50 2e20 596f  s use OpenMP. Yo
-00000ff0: 7520 6361 6e20 6469 7361 626c 6520 6974  u can disable it
-00001000: 2062 7920 7365 7474 696e 6720 7468 6520   by setting the 
-00001010: 656e 7620 7661 7269 6162 6c65 2060 4f4d  env variable `OM
-00001020: 505f 4e55 4d5f 5448 5245 4144 533d 3160  P_NUM_THREADS=1`
-00001030: 2c20 616e 6420 6974 2077 696c 6c20 7969  , and it will yi
-00001040: 656c 6420 7468 6520 7361 6d65 2070 6572  eld the same per
-00001050: 666f 726d 616e 6365 2061 7320 7468 6520  formance as the 
-00001060: 7665 7273 696f 6e20 636f 6d70 696c 6564  version compiled
-00001070: 2077 6974 686f 7574 204f 7065 6e4d 500a   without OpenMP.
-00001080: 0a54 6865 206f 7269 6769 6e61 6c20 606c  .The original `l
-00001090: 6962 6469 7673 7566 736f 7274 6020 6f6e  ibdivsufsort` on
-000010a0: 6c79 2073 7570 706f 7274 7320 6368 6172  ly supports char
-000010b0: 2061 7320 7468 6520 6261 7365 2074 7970   as the base typ
-000010c0: 652e 2060 7079 6469 7673 7566 736f 7274  e. `pydivsufsort
-000010d0: 6020 6361 6e20 6861 6e64 6c65 2061 7272  ` can handle arr
-000010e0: 6179 7320 6f66 2061 6e79 2069 6e74 6567  ays of any integ
-000010f0: 6572 2074 7970 6520 2865 7665 6e20 7369  er type (even si
-00001100: 676e 6564 292c 2062 7920 656e 636f 6469  gned), by encodi
-00001110: 6e67 2065 6163 6820 656c 656d 656e 7420  ng each element 
-00001120: 6173 206d 756c 7469 706c 6520 6368 6172  as multiple char
-00001130: 732c 2077 6869 6368 206d 616b 6573 2074  s, which makes t
-00001140: 6865 2063 6f6d 7075 7461 7469 6f6e 2073  he computation s
-00001150: 6c6f 7765 722e 2049 6620 796f 7572 2076  lower. If your v
-00001160: 616c 7565 7320 7573 6520 616e 2069 6e74  alues use an int
-00001170: 6567 6572 2074 7970 6520 7468 6174 2069  eger type that i
-00001180: 7320 6269 6767 6572 2074 6861 6e20 7265  s bigger than re
-00001190: 7175 6972 6564 2c20 6275 7420 7468 6579  quired, but they
-000011a0: 2073 7061 6e20 6f76 6572 2061 2073 6d61   span over a sma
-000011b0: 6c6c 2063 6f6e 7469 6775 6f75 7320 7261  ll contiguous ra
-000011c0: 6e67 652c 2060 7079 6469 7673 7566 736f  nge, `pydivsufso
-000011d0: 7274 6020 7769 6c6c 2061 7574 6f6d 6174  rt` will automat
-000011e0: 6963 616c 6c79 2063 6861 6e67 6520 7468  ically change th
-000011f0: 6569 7220 7479 7065 2028 7365 6520 5b23  eir type (see [#
-00001200: 365d 2868 7474 7073 3a2f 2f67 6974 6875  6](https://githu
-00001210: 622e 636f 6d2f 6c6f 7569 7361 6272 6168  b.com/louisabrah
-00001220: 616d 2f70 7964 6976 7375 6673 6f72 742f  am/pydivsufsort/
-00001230: 6973 7375 6573 2f36 2929 2e0a 0a23 2320  issues/6))...## 
-00001240: 4163 6b6e 6f77 6c65 6467 656d 656e 7473  Acknowledgements
-00001250: 0a0a 2d20 5b59 7574 6120 4d6f 7269 5d28  ..- [Yuta Mori](
-00001260: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001270: 6f6d 2f79 2d32 3536 2920 666f 7220 7772  om/y-256) for wr
-00001280: 6974 696e 6720 5b6c 6962 6469 7673 7566  iting [libdivsuf
-00001290: 736f 7274 5d28 6874 7470 733a 2f2f 6769  sort](https://gi
-000012a0: 7468 7562 2e63 6f6d 2f79 2d32 3536 2f6c  thub.com/y-256/l
-000012b0: 6962 6469 7673 7566 736f 7274 290a 2d20  ibdivsufsort).- 
-000012c0: 5b53 6561 6e20 4c61 775d 2868 7474 703a  [Sean Law](http:
-000012d0: 2f2f 7365 616e 6c61 772e 6769 7468 7562  //seanlaw.github
-000012e0: 2e69 6f2f 2920 666f 7220 696e 6974 6961  .io/) for initia
-000012f0: 7469 6e67 2074 6869 7320 7072 6f6a 6563  ting this projec
-00001300: 7420 616e 6420 636f 6e74 7269 6275 7469  t and contributi
-00001310: 6e67 0a0a 2323 2043 6974 696e 670a 0a49  ng..## Citing..I
-00001320: 6620 796f 7520 6861 7665 2075 7365 6420  f you have used 
-00001330: 7468 6973 2073 6f66 7477 6172 6520 696e  this software in
-00001340: 2061 2073 6369 656e 7469 6669 6320 7075   a scientific pu
-00001350: 626c 6963 6174 696f 6e2c 2070 6c65 6173  blication, pleas
-00001360: 6520 6369 7465 2069 7420 7573 696e 6720  e cite it using 
-00001370: 7468 6520 666f 6c6c 6f77 696e 6720 4269  the following Bi
-00001380: 624c 6154 6558 2063 6f64 653a 0a0a 6060  bLaTeX code:..``
-00001390: 600a 4073 6f66 7477 6172 657b 7079 6469  `.@software{pydi
-000013a0: 7673 7566 736f 7274 2c0a 2020 6175 7468  vsufsort,.  auth
-000013b0: 6f72 2020 2020 2020 203d 207b 4c6f 7569  or       = {Loui
-000013c0: 7320 4162 7261 6861 6d7d 2c0a 2020 7469  s Abraham},.  ti
-000013d0: 746c 6520 2020 2020 2020 203d 207b 7079  tle        = {py
-000013e0: 6469 7673 7566 736f 7274 7d2c 0a20 2079  divsufsort},.  y
-000013f0: 6561 7220 2020 2020 2020 2020 3d20 3230  ear         = 20
-00001400: 3233 2c0a 2020 7075 626c 6973 6865 7220  23,.  publisher 
-00001410: 2020 203d 207b 5a65 6e6f 646f 7d2c 0a20     = {Zenodo},. 
-00001420: 2064 6f69 2020 2020 2020 2020 2020 3d20   doi          = 
-00001430: 7b31 302e 3532 3831 2f7a 656e 6f64 6f2e  {10.5281/zenodo.
-00001440: 3739 3332 3435 387d 2c0a 2020 7572 6c20  7932458},.  url 
-00001450: 2020 2020 2020 2020 203d 207b 6874 7470           = {http
-00001460: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6c  s://github.com/l
-00001470: 6f75 6973 6162 7261 6861 6d2f 7079 6469  ouisabraham/pydi
-00001480: 7673 7566 736f 7274 7d0a 7d0a 6060 60    vsufsort}.}.```
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 7079 6469  : 2.1.Name: pydi
+00000020: 7673 7566 736f 7274 0a56 6572 7369 6f6e  vsufsort.Version
+00000030: 3a20 302e 302e 390a 5375 6d6d 6172 793a  : 0.0.9.Summary:
+00000040: 2053 7472 696e 6720 616c 676f 7269 7468   String algorith
+00000050: 6d73 0a48 6f6d 652d 7061 6765 3a20 6874  ms.Home-page: ht
+00000060: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000070: 2f6c 6f75 6973 6162 7261 6861 6d2f 7079  /louisabraham/py
+00000080: 6469 7673 7566 736f 7274 0a41 7574 686f  divsufsort.Autho
+00000090: 723a 204c 6f75 6973 2041 6272 6168 616d  r: Louis Abraham
+000000a0: 0a41 7574 686f 722d 656d 6169 6c3a 206c  .Author-email: l
+000000b0: 6f75 6973 2e61 6272 6168 616d 4079 6168  ouis.abraham@yah
+000000c0: 6f6f 2e66 720a 4c69 6365 6e73 653a 204d  oo.fr.License: M
+000000d0: 4954 0a52 6571 7569 7265 732d 5079 7468  IT.Requires-Pyth
+000000e0: 6f6e 3a20 3e3d 332e 360a 4465 7363 7269  on: >=3.6.Descri
+000000f0: 7074 696f 6e2d 436f 6e74 656e 742d 5479  ption-Content-Ty
+00000100: 7065 3a20 7465 7874 2f6d 6172 6b64 6f77  pe: text/markdow
+00000110: 6e0a 4c69 6365 6e73 652d 4669 6c65 3a20  n.License-File: 
+00000120: 4c49 4345 4e53 450a 0a5b 215b 5079 5049  LICENSE..[![PyPI
+00000130: 0a76 6572 7369 6f6e 5d28 6874 7470 733a  .version](https:
+00000140: 2f2f 6261 6467 652e 6675 7279 2e69 6f2f  //badge.fury.io/
+00000150: 7079 2f70 7964 6976 7375 6673 6f72 742e  py/pydivsufsort.
+00000160: 7376 6729 5d28 6874 7470 733a 2f2f 6261  svg)](https://ba
+00000170: 6467 652e 6675 7279 2e69 6f2f 7079 2f70  dge.fury.io/py/p
+00000180: 7964 6976 7375 6673 6f72 7429 205b 215b  ydivsufsort) [![
+00000190: 446f 776e 6c6f 6164 735d 2868 7474 7073  Downloads](https
+000001a0: 3a2f 2f70 6570 792e 7465 6368 2f62 6164  ://pepy.tech/bad
+000001b0: 6765 2f70 7964 6976 7375 6673 6f72 7429  ge/pydivsufsort)
+000001c0: 5d28 6874 7470 733a 2f2f 7065 7079 2e74  ](https://pepy.t
+000001d0: 6563 682f 7072 6f6a 6563 742f 7079 6469  ech/project/pydi
+000001e0: 7673 7566 736f 7274 2920 5b21 5b54 6573  vsufsort) [![Tes
+000001f0: 745d 2868 7474 7073 3a2f 2f67 6974 6875  t](https://githu
+00000200: 622e 636f 6d2f 6c6f 7569 7361 6272 6168  b.com/louisabrah
+00000210: 616d 2f70 7964 6976 7375 6673 6f72 742f  am/pydivsufsort/
+00000220: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
+00000230: 732f 7465 7374 2e79 6d6c 2f62 6164 6765  s/test.yml/badge
+00000240: 2e73 7667 295d 2868 7474 7073 3a2f 2f67  .svg)](https://g
+00000250: 6974 6875 622e 636f 6d2f 6c6f 7569 7361  ithub.com/louisa
+00000260: 6272 6168 616d 2f70 7964 6976 7375 6673  braham/pydivsufs
+00000270: 6f72 742f 6163 7469 6f6e 732f 776f 726b  ort/actions/work
+00000280: 666c 6f77 732f 7465 7374 2e79 6d6c 2920  flows/test.yml) 
+00000290: 5b21 5b42 7569 6c64 2061 6e64 2075 706c  [![Build and upl
+000002a0: 6f61 645d 2868 7474 7073 3a2f 2f67 6974  oad](https://git
+000002b0: 6875 622e 636f 6d2f 6c6f 7569 7361 6272  hub.com/louisabr
+000002c0: 6168 616d 2f70 7964 6976 7375 6673 6f72  aham/pydivsufsor
+000002d0: 742f 6163 7469 6f6e 732f 776f 726b 666c  t/actions/workfl
+000002e0: 6f77 732f 6275 696c 642d 616e 642d 7570  ows/build-and-up
+000002f0: 6c6f 6164 2e79 6d6c 2f62 6164 6765 2e73  load.yml/badge.s
+00000300: 7667 295d 2868 7474 7073 3a2f 2f67 6974  vg)](https://git
+00000310: 6875 622e 636f 6d2f 6c6f 7569 7361 6272  hub.com/louisabr
+00000320: 6168 616d 2f70 7964 6976 7375 6673 6f72  aham/pydivsufsor
+00000330: 742f 6163 7469 6f6e 732f 776f 726b 666c  t/actions/workfl
+00000340: 6f77 732f 6275 696c 642d 616e 642d 7570  ows/build-and-up
+00000350: 6c6f 6164 2e79 6d6c 2920 5b21 5b63 6f64  load.yml) [![cod
+00000360: 6563 6f76 5d28 6874 7470 733a 2f2f 636f  ecov](https://co
+00000370: 6465 636f 762e 696f 2f67 682f 6c6f 7569  decov.io/gh/loui
+00000380: 7361 6272 6168 616d 2f70 7964 6976 7375  sabraham/pydivsu
+00000390: 6673 6f72 742f 6272 616e 6368 2f6d 6173  fsort/branch/mas
+000003a0: 7465 722f 6772 6170 682f 6261 6467 652e  ter/graph/badge.
+000003b0: 7376 673f 746f 6b65 6e3d 4131 424d 3955  svg?token=A1BM9U
+000003c0: 314f 4c56 295d 2868 7474 7073 3a2f 2f63  1OLV)](https://c
+000003d0: 6f64 6563 6f76 2e69 6f2f 6768 2f6c 6f75  odecov.io/gh/lou
+000003e0: 6973 6162 7261 6861 6d2f 7079 6469 7673  isabraham/pydivs
+000003f0: 7566 736f 7274 2920 5b21 5b44 4f49 5d28  ufsort) [![DOI](
+00000400: 6874 7470 733a 2f2f 7a65 6e6f 646f 2e6f  https://zenodo.o
+00000410: 7267 2f62 6164 6765 2f32 3431 3133 3739  rg/badge/2411379
+00000420: 3339 2e73 7667 295d 2868 7474 7073 3a2f  39.svg)](https:/
+00000430: 2f7a 656e 6f64 6f2e 6f72 672f 6261 6467  /zenodo.org/badg
+00000440: 652f 6c61 7465 7374 646f 692f 3234 3131  e/latestdoi/2411
+00000450: 3337 3933 3929 0a0a 2320 6070 7964 6976  37939)..# `pydiv
+00000460: 7375 6673 6f72 7460 3a20 6269 6e64 696e  sufsort`: bindin
+00000470: 6773 2074 6f20 6c69 6264 6976 7375 6673  gs to libdivsufs
+00000480: 6f72 740a 0a60 7079 6469 7673 7566 736f  ort..`pydivsufso
+00000490: 7274 6020 7072 6562 7569 6c64 7320 606c  rt` prebuilds `l
+000004a0: 6962 6469 7673 7566 736f 7274 6020 6173  ibdivsufsort` as
+000004b0: 2061 2073 6861 7265 6420 6c69 6272 6172   a shared librar
+000004c0: 7920 616e 640a 696e 636c 7564 6573 2069  y and.includes i
+000004d0: 7420 696e 2061 2050 7974 686f 6e20 7061  t in a Python pa
+000004e0: 636b 6167 6520 7769 7468 2062 696e 6469  ckage with bindi
+000004f0: 6e67 732e 2057 6865 656c 7320 6172 6520  ngs. Wheels are 
+00000500: 6275 696c 7420 666f 7220 4c69 6e75 782c  built for Linux,
+00000510: 206d 6163 4f53 2061 6e64 2057 696e 646f   macOS and Windo
+00000520: 7773 2028 3332 2061 6e64 2036 3420 6269  ws (32 and 64 bi
+00000530: 7473 2920 7573 696e 6720 6063 6962 7569  ts) using `cibui
+00000540: 6c64 7768 6565 6c60 2061 6e64 2047 6974  ldwheel` and Git
+00000550: 4875 6220 4163 7469 6f6e 732e 2042 6173  Hub Actions. Bas
+00000560: 6963 616c 6c79 2c20 796f 7520 7368 6f75  ically, you shou
+00000570: 6c64 2062 6520 6162 6c65 2074 6f20 696e  ld be able to in
+00000580: 7374 616c 6c20 6974 2077 6974 6820 6070  stall it with `p
+00000590: 6970 2069 6e73 7461 6c6c 2070 7964 6976  ip install pydiv
+000005a0: 7375 6673 6f72 7460 206f 6e20 616e 7920  sufsort` on any 
+000005b0: 7379 7374 656d 2061 6e64 2069 7420 7368  system and it sh
+000005c0: 6f75 6c64 2077 6f72 6b20 6f75 7420 6f66  ould work out of
+000005d0: 2074 6865 2062 6f78 2e20 4966 2069 7420   the box. If it 
+000005e0: 646f 6573 6e27 742c 2070 6c65 6173 6520  doesn't, please 
+000005f0: 6372 6561 7465 2061 6e20 6973 7375 652e  create an issue.
+00000600: 0a0a 2a2a 4665 6174 7572 6573 2a2a 3a0a  ..**Features**:.
+00000610: 0a2d 2062 696e 6469 6e67 7320 746f 2060  .- bindings to `
+00000620: 6469 7673 7566 736f 7274 6020 7468 6174  divsufsort` that
+00000630: 2072 6574 7572 6e20 6e75 6d70 7920 6172   return numpy ar
+00000640: 7261 7973 0a2d 2068 616e 646c 6520 7374  rays.- handle st
+00000650: 7269 6e67 2c20 6279 7465 7320 616e 6420  ring, bytes and 
+00000660: 616c 6d6f 7374 2061 6e79 2069 6e74 6567  almost any integ
+00000670: 6572 2064 6174 6120 7479 7065 2028 652e  er data type (e.
+00000680: 672e 2060 696e 7436 3460 2920 616e 6420  g. `int64`) and 
+00000690: 6e6f 7420 6f6e 6c79 2060 6368 6172 600a  not only `char`.
+000006a0: 2d20 616c 676f 7269 7468 6d73 2077 6f72  - algorithms wor
+000006b0: 6b20 6576 656e 2066 6f72 206e 6f6e 2063  k even for non c
+000006c0: 6861 7220 696e 7075 7473 0a2d 2061 6464  har inputs.- add
+000006d0: 6974 696f 6e61 6c20 7374 7269 6e67 2061  itional string a
+000006e0: 6c67 6f72 6974 686d 7320 636f 6465 6420  lgorithms coded 
+000006f0: 696e 2043 7974 686f 6e0a 0a23 2320 496e  in Cython..## In
+00000700: 7374 616c 6c61 7469 6f6e 0a0a 4f6e 204c  stallation..On L
+00000710: 696e 7578 2c20 6d61 634f 5320 616e 6420  inux, macOS and 
+00000720: 5769 6e64 6f77 733a 0a0a 6060 600a 7079  Windows:..```.py
+00000730: 7468 6f6e 202d 6d20 7069 7020 696e 7374  thon -m pip inst
+00000740: 616c 6c20 7079 6469 7673 7566 736f 7274  all pydivsufsort
+00000750: 0a60 6060 0a0a 5765 2070 726f 7669 6465  .```..We provide
+00000760: 2070 7265 636f 6d70 696c 6564 2077 6865   precompiled whe
+00000770: 656c 7320 666f 7220 636f 6d6d 6f6e 2073  els for common s
+00000780: 7973 7465 6d73 2075 7369 6e67 2060 6369  ystems using `ci
+00000790: 6275 696c 6477 6865 656c 602c 2061 6e64  buildwheel`, and
+000007a0: 2061 2073 6f75 7263 6520 6469 7374 7269   a source distri
+000007b0: 6275 7469 6f6e 2066 6f72 2055 6e69 7820  bution for Unix 
+000007c0: 7379 7374 656d 732e 204d 616e 7561 6c20  systems. Manual 
+000007d0: 636f 6d70 696c 6174 696f 6e20 6f6e 2057  compilation on W
+000007e0: 696e 646f 7773 206d 6967 6874 2072 6571  indows might req
+000007f0: 7569 7265 2073 6f6d 6520 7477 6561 6b69  uire some tweaki
+00000800: 6e67 2c20 706c 6561 7365 2063 7265 6174  ng, please creat
+00000810: 6520 616e 2069 7373 7565 2e0a 0a23 2320  e an issue...## 
+00000820: 4665 6174 7572 6573 0a0a 416c 6c20 6d65  Features..All me
+00000830: 7468 6f64 7320 7375 7070 6f72 7420 7374  thods support st
+00000840: 7269 6e67 2c20 6279 7465 7320 616e 6420  ring, bytes and 
+00000850: 6e75 6d70 7920 6172 7261 7920 696e 7075  numpy array inpu
+00000860: 7473 2c20 696e 636c 7564 696e 6720 6461  ts, including da
+00000870: 7461 7479 7065 7320 6772 6561 7465 7220  tatypes greater 
+00000880: 7468 616e 2060 7569 6e74 385f 7460 2028  than `uint8_t` (
+00000890: 652e 672e 2060 7569 6e74 3634 5f74 6029  e.g. `uint64_t`)
+000008a0: 2e20 4265 6c6f 7720 6172 6520 7468 6520  . Below are the 
+000008b0: 7369 676e 6174 7572 6573 206f 6620 616c  signatures of al
+000008c0: 6c20 6d65 7468 6f64 7320 6578 706f 7365  l methods expose
+000008d0: 6420 6279 2060 7079 6469 7673 7566 736f  d by `pydivsufso
+000008e0: 7274 602e 2054 6f20 696d 706f 7274 2061  rt`. To import a
+000008f0: 206d 6574 686f 642c 206a 7573 7420 646f   method, just do
+00000900: 2060 6672 6f6d 2070 7964 6976 7375 6673   `from pydivsufs
+00000910: 6f72 7420 696d 706f 7274 206d 6574 686f  ort import metho
+00000920: 645f 6e61 6d65 602e 2041 6c6c 206d 6574  d_name`. All met
+00000930: 686f 6473 2061 7265 2064 6f63 756d 656e  hods are documen
+00000940: 7465 6420 696e 2074 6865 2064 6f63 7374  ted in the docst
+00000950: 7269 6e67 732e 2059 6f75 2063 616e 2064  rings. You can d
+00000960: 6973 706c 6179 2074 6865 6d20 7769 7468  isplay them with
+00000970: 2060 6865 6c70 286d 6574 686f 645f 6e61   `help(method_na
+00000980: 6d65 2960 2e0a 0a41 206e 6963 6572 2069  me)`...A nicer i
+00000990: 6e74 6572 6661 6365 2074 6f20 7265 7573  nterface to reus
+000009a0: 6520 636f 6d70 7574 6174 696f 6e73 206c  e computations l
+000009b0: 617a 696c 7920 6973 2070 726f 7669 6465  azily is provide
+000009c0: 6420 696e 2057 6f6e 6465 7253 7472 696e  d in WonderStrin
+000009d0: 6720 6275 7420 6375 7272 656e 746c 7920  g but currently 
+000009e0: 756e 646f 6375 6d65 6e74 6564 2e20 506c  undocumented. Pl
+000009f0: 6561 7365 2063 7265 6174 6520 616e 2069  ease create an i
+00000a00: 7373 7565 2069 6620 796f 7520 6172 6520  ssue if you are 
+00000a10: 696e 7465 7265 7374 6564 2e0a 0a23 2323  interested...###
+00000a20: 204d 6574 686f 6473 2065 7870 6f73 6564   Methods exposed
+00000a30: 2066 726f 6d20 6c69 6264 6976 7375 6673   from libdivsufs
+00000a40: 6f72 740a 0a2d 2060 6469 7673 7566 736f  ort..- `divsufso
+00000a50: 7274 2873 7472 696e 6729 603a 2073 7566  rt(string)`: suf
+00000a60: 6669 7820 6172 7261 790a 2d20 6062 775f  fix array.- `bw_
+00000a70: 7472 616e 7366 6f72 6d28 7374 7269 6e67  transform(string
+00000a80: 2960 3a20 4275 7272 6f77 732d 5768 6565  )`: Burrows-Whee
+00000a90: 6c65 7220 7472 616e 7366 6f72 6d0a 2d20  ler transform.- 
+00000aa0: 6069 6e76 6572 7365 5f62 775f 7472 616e  `inverse_bw_tran
+00000ab0: 7366 6f72 6d28 6964 782c 2073 7472 696e  sform(idx, strin
+00000ac0: 6729 603a 2069 6e76 6572 7365 2042 7572  g)`: inverse Bur
+00000ad0: 726f 7773 2d57 6865 656c 6572 2074 7261  rows-Wheeler tra
+00000ae0: 6e73 666f 726d 0a2d 2060 7361 5f73 6561  nsform.- `sa_sea
+00000af0: 7263 6828 7374 7269 6e67 2c20 7375 6666  rch(string, suff
+00000b00: 6978 5f61 7272 6179 2c20 7061 7474 6572  ix_array, patter
+00000b10: 6e29 603a 2073 6561 7263 6820 666f 7220  n)`: search for 
+00000b20: 6120 7061 7474 6572 6e20 696e 2061 2073  a pattern in a s
+00000b30: 7566 6669 7820 6172 7261 790a 0a0a 2323  uffix array...##
+00000b40: 2320 4164 6469 7469 6f6e 616c 2073 7472  # Additional str
+00000b50: 696e 6720 616c 676f 7269 7468 6d73 0a0a  ing algorithms..
+00000b60: 2d20 606b 6173 6169 2873 7472 696e 672c  - `kasai(string,
+00000b70: 2073 7566 6669 785f 6172 7261 793d 4e6f   suffix_array=No
+00000b80: 6e65 2960 3a20 4c43 5020 6172 7261 7920  ne)`: LCP array 
+00000b90: 636f 6d70 7574 6174 696f 6e20 286c 617a  computation (laz
+00000ba0: 696c 7920 636f 6d70 7574 6573 2074 6865  ily computes the
+00000bb0: 2073 7566 6669 7820 6172 7261 7920 6966   suffix array if
+00000bc0: 206e 6f74 2070 726f 7669 6465 6429 0a2d   not provided).-
+00000bd0: 2060 6c63 705f 7365 6774 7265 6528 7374   `lcp_segtree(st
+00000be0: 7269 6e67 2c20 7375 6666 6978 5f61 7272  ring, suffix_arr
+00000bf0: 6179 3d4e 6f6e 652c 206c 6370 3d4e 6f6e  ay=None, lcp=Non
+00000c00: 6529 603a 2062 7569 6c64 2061 2073 6567  e)`: build a seg
+00000c10: 6d65 6e74 2074 7265 6520 666f 7220 4c43  ment tree for LC
+00000c20: 5020 7175 6572 6965 7320 286c 617a 696c  P queries (lazil
+00000c30: 7920 636f 6d70 7574 6573 2074 6865 2073  y computes the s
+00000c40: 7566 6669 7820 6172 7261 7920 616e 6420  uffix array and 
+00000c50: 4c43 5020 6172 7261 7920 6966 206e 6f74  LCP array if not
+00000c60: 2070 726f 7669 6465 6429 0a2d 2060 6c63   provided).- `lc
+00000c70: 705f 7175 6572 7928 7365 6774 7265 652c  p_query(segtree,
+00000c80: 2071 7565 7269 6573 2960 3a20 7175 6572   queries)`: quer
+00000c90: 7920 6120 7365 676d 656e 7420 7472 6565  y a segment tree
+00000ca0: 2066 6f72 204c 4350 2071 7565 7269 6573   for LCP queries
+00000cb0: 2e20 5175 6572 6965 7320 6172 6520 7061  . Queries are pa
+00000cc0: 6972 7320 6f66 2069 6e64 6963 6573 2e0a  irs of indices..
+00000cd0: 2d20 606c 6576 656e 7368 7465 696e 2873  - `levenshtein(s
+00000ce0: 7472 696e 6731 2c20 7374 7269 6e67 3229  tring1, string2)
+00000cf0: 603a 204c 6576 656e 7368 7465 696e 2064  `: Levenshtein d
+00000d00: 6973 7461 6e63 650a 2d20 606d 6f73 745f  istance.- `most_
+00000d10: 6672 6571 7565 6e74 5f73 7562 7374 7269  frequent_substri
+00000d20: 6e67 7328 6c63 702c 206c 656e 6774 682c  ngs(lcp, length,
+00000d30: 206c 696d 6974 3d30 2c20 6d69 6e69 6d75   limit=0, minimu
+00000d40: 6d5f 636f 756e 743d 3129 603a 206d 6f73  m_count=1)`: mos
+00000d50: 7420 6672 6571 7565 6e74 2073 7562 7374  t frequent subst
+00000d60: 7269 6e67 732e 2053 6565 2074 6865 2064  rings. See the d
+00000d70: 6f63 7374 7269 6e67 2066 6f72 2064 6574  ocstring for det
+00000d80: 6169 6c73 2e0a 2d20 6063 6f6d 6d6f 6e5f  ails..- `common_
+00000d90: 7375 6273 7472 696e 6773 2873 7472 696e  substrings(strin
+00000da0: 6731 2c20 7374 7269 6e67 322c 206c 696d  g1, string2, lim
+00000db0: 6974 3d32 3529 603a 2063 6f6d 6d6f 6e20  it=25)`: common 
+00000dc0: 7375 6273 7472 696e 6773 2062 6574 7765  substrings betwe
+00000dd0: 656e 2074 776f 2073 7472 696e 6773 2e0a  en two strings..
+00000de0: 0a0a 2323 2320 4578 616d 706c 6520 7573  ..### Example us
+00000df0: 6167 650a 0a60 6060 7079 7468 6f6e 0a66  age..```python.f
+00000e00: 726f 6d20 7079 6469 7673 7566 736f 7274  rom pydivsufsort
+00000e10: 2069 6d70 6f72 7420 6469 7673 7566 736f   import divsufso
+00000e20: 7274 2c20 6b61 7361 690a 0a73 7472 696e  rt, kasai..strin
+00000e30: 675f 696e 7020 3d20 2262 616e 616e 6124  g_inp = "banana$
+00000e40: 220a 7374 7269 6e67 5f73 7566 6669 785f  ".string_suffix_
+00000e50: 6172 7261 7920 3d20 6469 7673 7566 736f  array = divsufso
+00000e60: 7274 2873 7472 696e 675f 696e 7029 0a73  rt(string_inp).s
+00000e70: 7472 696e 675f 6c63 705f 6172 7261 7920  tring_lcp_array 
+00000e80: 3d20 6b61 7361 6928 7374 7269 6e67 5f69  = kasai(string_i
+00000e90: 6e70 2c20 7374 7269 6e67 5f73 7566 6669  np, string_suffi
+00000ea0: 785f 6172 7261 7929 0a70 7269 6e74 2873  x_array).print(s
+00000eb0: 7472 696e 675f 7375 6666 6978 5f61 7272  tring_suffix_arr
+00000ec0: 6179 2c20 7374 7269 6e67 5f6c 6370 5f61  ay, string_lcp_a
+00000ed0: 7272 6179 290a 2320 5b36 2035 2033 2031  rray).# [6 5 3 1
+00000ee0: 2030 2034 2032 5d20 5b30 2031 2033 2030   0 4 2] [0 1 3 0
+00000ef0: 2030 2032 2030 5d0a 0a23 2059 6f75 2063   0 2 0]..# You c
+00000f00: 616e 2061 6c73 6f20 636f 6e76 6572 7420  an also convert 
+00000f10: 7468 6520 7374 7269 6e67 2069 6e70 7574  the string input
+00000f20: 2074 6f20 696e 7465 6765 7273 2066 6972   to integers fir
+00000f30: 7374 0a0a 696d 706f 7274 206e 756d 7079  st..import numpy
+00000f40: 2061 7320 6e70 0a0a 696e 745f 696e 7020   as np..int_inp 
+00000f50: 3d20 6e70 2e75 6e69 7175 6528 6e70 2e61  = np.unique(np.a
+00000f60: 7272 6179 286c 6973 7428 7374 7269 6e67  rray(list(string
+00000f70: 5f69 6e70 2929 2c20 7265 7475 726e 5f69  _inp)), return_i
+00000f80: 6e76 6572 7365 3d54 7275 6529 5b31 5d0a  nverse=True)[1].
+00000f90: 696e 745f 7375 6666 6978 5f61 7272 6179  int_suffix_array
+00000fa0: 203d 2064 6976 7375 6673 6f72 7428 696e   = divsufsort(in
+00000fb0: 745f 696e 7029 0a69 6e74 5f6c 6370 5f61  t_inp).int_lcp_a
+00000fc0: 7272 6179 203d 206b 6173 6169 2869 6e74  rray = kasai(int
+00000fd0: 5f69 6e70 2c20 696e 745f 7375 6666 6978  _inp, int_suffix
+00000fe0: 5f61 7272 6179 290a 7072 696e 7428 696e  _array).print(in
+00000ff0: 745f 7375 6666 6978 5f61 7272 6179 2c20  t_suffix_array, 
+00001000: 696e 745f 6c63 705f 6172 7261 7929 0a23  int_lcp_array).#
+00001010: 205b 3620 3520 3320 3120 3020 3420 325d   [6 5 3 1 0 4 2]
+00001020: 205b 3020 3120 3320 3020 3020 3220 305d   [0 1 3 0 0 2 0]
+00001030: 0a60 6060 0a0a 0a23 2320 4465 7665 6c6f  .```...## Develo
+00001040: 706d 656e 740a 0a59 6f75 2063 616e 2069  pment..You can i
+00001050: 6e73 7461 6c6c 206c 6f63 616c 6c79 2077  nstall locally w
+00001060: 6974 680a 0a60 6060 0a70 6970 2069 6e73  ith..```.pip ins
+00001070: 7461 6c6c 202d 6520 2e0a 6060 600a 0a41  tall -e ..```..A
+00001080: 2075 7365 6675 6c20 636f 6d6d 616e 6420   useful command 
+00001090: 746f 2069 7465 7261 7465 2071 7569 636b  to iterate quick
+000010a0: 6c79 2077 6865 6e20 6368 616e 6769 6e67  ly when changing
+000010b0: 2043 7974 686f 6e20 636f 6465 2069 730a   Cython code is.
+000010c0: 0a60 6060 0a70 7974 686f 6e20 7365 7475  .```.python setu
+000010d0: 702e 7079 2062 7569 6c64 5f65 7874 202d  p.py build_ext -
+000010e0: 2d69 6e70 6c61 6365 2026 2620 7079 7465  -inplace && pyte
+000010f0: 7374 202d 730a 6060 600a 0a23 2323 2050  st -s.```..### P
+00001100: 726f 6669 6c69 6e67 0a0a 5072 6f66 696c  rofiling..Profil
+00001110: 696e 6720 6361 6e20 6265 2061 6374 6976  ing can be activ
+00001120: 6174 6564 2077 6974 6820 7468 6520 656e  ated with the en
+00001130: 7669 726f 6e6d 656e 7420 7661 7269 6162  vironment variab
+00001140: 6c65 2060 5052 4f46 494c 4560 3a0a 0a60  le `PROFILE`:..`
+00001150: 6060 0a50 524f 4649 4c45 3d31 2070 7974  ``.PROFILE=1 pyt
+00001160: 686f 6e20 7365 7475 702e 7079 2062 7569  hon setup.py bui
+00001170: 6c64 5f65 7874 202d 2d69 6e70 6c61 6365  ld_ext --inplace
+00001180: 2026 2620 7079 7465 7374 202d 730a 6060   && pytest -s.``
+00001190: 600a 0a48 6572 6520 6973 2061 6e20 6578  `..Here is an ex
+000011a0: 616d 706c 6520 7769 7468 206c 696e 655f  ample with line_
+000011b0: 7072 6f66 696c 6572 2028 7265 7175 6972  profiler (requir
+000011c0: 6573 2060 7069 7020 696e 7374 616c 6c20  es `pip install 
+000011d0: 226c 696e 655f 7072 6f66 696c 6572 3c34  "line_profiler<4
+000011e0: 2260 293a 0a0a 6060 600a 696d 706f 7274  "`):..```.import
+000011f0: 206c 696e 655f 7072 6f66 696c 6572 0a66   line_profiler.f
+00001200: 726f 6d20 7079 6469 7673 7566 736f 7274  rom pydivsufsort
+00001210: 2069 6d70 6f72 7420 636f 6d6d 6f6e 5f73   import common_s
+00001220: 7562 7374 7269 6e67 730a 6672 6f6d 2070  ubstrings.from p
+00001230: 7964 6976 7375 6673 6f72 742e 7374 7269  ydivsufsort.stri
+00001240: 6e67 616c 6720 696d 706f 7274 2028 0a20  ngalg import (. 
+00001250: 2020 205f 636f 6d6d 6f6e 5f73 7562 7374     _common_subst
+00001260: 7269 6e67 732c 0a20 2020 2072 6570 6561  rings,.    repea
+00001270: 7465 645f 7375 6273 7472 696e 6773 2c0a  ted_substrings,.
+00001280: 290a 0a73 3120 3d20 2262 616e 616e 6122  )..s1 = "banana"
+00001290: 202a 2031 3030 3030 0a73 3220 3d20 2261   * 10000.s2 = "a
+000012a0: 6e61 6e61 7322 202a 2031 3030 3030 0a0a  nanas" * 10000..
+000012b0: 6675 6e63 203d 2063 6f6d 6d6f 6e5f 7375  func = common_su
+000012c0: 6273 7472 696e 6773 0a70 726f 6669 6c65  bstrings.profile
+000012d0: 203d 206c 696e 655f 7072 6f66 696c 6572   = line_profiler
+000012e0: 2e4c 696e 6550 726f 6669 6c65 7228 6675  .LineProfiler(fu
+000012f0: 6e63 290a 7072 6f66 696c 652e 6164 645f  nc).profile.add_
+00001300: 6675 6e63 7469 6f6e 285f 636f 6d6d 6f6e  function(_common
+00001310: 5f73 7562 7374 7269 6e67 7329 0a70 726f  _substrings).pro
+00001320: 6669 6c65 2e61 6464 5f66 756e 6374 696f  file.add_functio
+00001330: 6e28 7265 7065 6174 6564 5f73 7562 7374  n(repeated_subst
+00001340: 7269 6e67 7329 0a70 726f 6669 6c65 2e72  rings).profile.r
+00001350: 756e 6361 6c6c 2866 756e 632c 2073 312c  uncall(func, s1,
+00001360: 2073 322c 206c 696d 6974 3d31 3529 0a70   s2, limit=15).p
+00001370: 726f 6669 6c65 2e70 7269 6e74 5f73 7461  rofile.print_sta
+00001380: 7473 2829 0a60 6060 0a0a 2323 2054 6573  ts().```..## Tes
+00001390: 7469 6e67 0a0a 6060 600a 7079 7465 7374  ting..```.pytest
+000013a0: 0a60 6060 0a0a 2323 2054 6563 686e 6963  .```..## Technic
+000013b0: 616c 2064 6574 6169 6c73 2028 666f 7220  al details (for 
+000013c0: 7065 7266 6f72 6d61 6e63 6520 7477 6561  performance twea
+000013d0: 6b73 290a 0a60 6c69 6264 6976 7375 6673  ks)..`libdivsufs
+000013e0: 6f72 7460 2069 7320 636f 6d70 696c 6564  ort` is compiled
+000013f0: 2069 6e20 626f 7468 2033 3220 616e 6420   in both 32 and 
+00001400: 3634 2062 6974 732c 2061 7320 5b74 6865  64 bits, as [the
+00001410: 2033 3220 6269 7473 2076 6572 7369 6f6e   32 bits version
+00001420: 2069 7320 6661 7374 6572 5d28 6874 7470   is faster](http
+00001430: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f79  s://github.com/y
+00001440: 2d32 3536 2f6c 6962 6469 7673 7566 736f  -256/libdivsufso
+00001450: 7274 2f69 7373 7565 732f 3231 292e 2060  rt/issues/21). `
+00001460: 7079 6469 7673 7566 736f 7274 6020 6175  pydivsufsort` au
+00001470: 746f 6d61 7469 6361 6c6c 7920 6368 6f6f  tomatically choo
+00001480: 7365 7320 746f 2075 7365 2074 6865 2033  ses to use the 3
+00001490: 3220 6269 7473 2076 6572 7369 6f6e 2077  2 bits version w
+000014a0: 6865 6e20 706f 7373 6962 6c65 2028 616b  hen possible (ak
+000014b0: 6120 7768 656e 2074 6865 2069 6e70 7574  a when the input
+000014c0: 2073 697a 6520 6973 206c 6573 7320 7468   size is less th
+000014d0: 616e 2060 322a 2a33 312d 3160 292e 0a0a  an `2**31-1`)...
+000014e0: 466f 7220 6265 7374 2070 6572 666f 726d  For best perform
+000014f0: 616e 6365 2c20 7573 6520 636f 6e74 6967  ance, use contig
+00001500: 756f 7573 2061 7272 6179 732e 2049 6620  uous arrays. If 
+00001510: 796f 7520 6861 7665 2061 2073 6c69 6365  you have a slice
+00001520: 6420 6172 7261 792c 2070 7964 6976 7375  d array, pydivsu
+00001530: 6673 6f72 7420 636f 6e76 6572 7473 2069  fsort converts i
+00001540: 7420 6175 746f 6d61 7469 6361 6c6c 7920  t automatically 
+00001550: 7769 7468 205b 606e 756d 7079 2e61 7363  with [`numpy.asc
+00001560: 6f6e 7469 6775 6f75 7361 7272 6179 605d  ontiguousarray`]
+00001570: 2868 7474 7073 3a2f 2f64 6f63 732e 7363  (https://docs.sc
+00001580: 6970 792e 6f72 672f 646f 632f 6e75 6d70  ipy.org/doc/nump
+00001590: 792f 7265 6665 7265 6e63 652f 6765 6e65  y/reference/gene
+000015a0: 7261 7465 642f 6e75 6d70 792e 6173 636f  rated/numpy.asco
+000015b0: 6e74 6967 756f 7573 6172 7261 792e 6874  ntiguousarray.ht
+000015c0: 6d6c 292e 0a0a 5468 6520 7072 6563 6f6d  ml)...The precom
+000015d0: 7069 6c65 6420 6c69 6272 6172 6965 7320  piled libraries 
+000015e0: 7573 6520 4f70 656e 4d50 2e20 596f 7520  use OpenMP. You 
+000015f0: 6361 6e20 6469 7361 626c 6520 6974 2062  can disable it b
+00001600: 7920 7365 7474 696e 6720 7468 6520 656e  y setting the en
+00001610: 7620 7661 7269 6162 6c65 2060 4f4d 505f  v variable `OMP_
+00001620: 4e55 4d5f 5448 5245 4144 533d 3160 2c20  NUM_THREADS=1`, 
+00001630: 616e 6420 6974 2077 696c 6c20 7969 656c  and it will yiel
+00001640: 6420 7468 6520 7361 6d65 2070 6572 666f  d the same perfo
+00001650: 726d 616e 6365 2061 7320 7468 6520 7665  rmance as the ve
+00001660: 7273 696f 6e20 636f 6d70 696c 6564 2077  rsion compiled w
+00001670: 6974 686f 7574 204f 7065 6e4d 500a 0a54  ithout OpenMP..T
+00001680: 6865 206f 7269 6769 6e61 6c20 606c 6962  he original `lib
+00001690: 6469 7673 7566 736f 7274 6020 6f6e 6c79  divsufsort` only
+000016a0: 2073 7570 706f 7274 7320 6368 6172 2061   supports char a
+000016b0: 7320 7468 6520 6261 7365 2074 7970 652e  s the base type.
+000016c0: 2060 7079 6469 7673 7566 736f 7274 6020   `pydivsufsort` 
+000016d0: 6361 6e20 6861 6e64 6c65 2061 7272 6179  can handle array
+000016e0: 7320 6f66 2061 6e79 2069 6e74 6567 6572  s of any integer
+000016f0: 2074 7970 6520 2865 7665 6e20 7369 676e   type (even sign
+00001700: 6564 292c 2062 7920 656e 636f 6469 6e67  ed), by encoding
+00001710: 2065 6163 6820 656c 656d 656e 7420 6173   each element as
+00001720: 206d 756c 7469 706c 6520 6368 6172 732c   multiple chars,
+00001730: 2077 6869 6368 206d 616b 6573 2074 6865   which makes the
+00001740: 2063 6f6d 7075 7461 7469 6f6e 2073 6c6f   computation slo
+00001750: 7765 722e 2049 6620 796f 7572 2076 616c  wer. If your val
+00001760: 7565 7320 7573 6520 616e 2069 6e74 6567  ues use an integ
+00001770: 6572 2074 7970 6520 7468 6174 2069 7320  er type that is 
+00001780: 6269 6767 6572 2074 6861 6e20 7265 7175  bigger than requ
+00001790: 6972 6564 2c20 6275 7420 7468 6579 2073  ired, but they s
+000017a0: 7061 6e20 6f76 6572 2061 2073 6d61 6c6c  pan over a small
+000017b0: 2063 6f6e 7469 6775 6f75 7320 7261 6e67   contiguous rang
+000017c0: 652c 2060 7079 6469 7673 7566 736f 7274  e, `pydivsufsort
+000017d0: 6020 7769 6c6c 2061 7574 6f6d 6174 6963  ` will automatic
+000017e0: 616c 6c79 2063 6861 6e67 6520 7468 6569  ally change thei
+000017f0: 7220 7479 7065 2028 7365 6520 5b23 365d  r type (see [#6]
+00001800: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00001810: 636f 6d2f 6c6f 7569 7361 6272 6168 616d  com/louisabraham
+00001820: 2f70 7964 6976 7375 6673 6f72 742f 6973  /pydivsufsort/is
+00001830: 7375 6573 2f36 2929 2e0a 0a23 2320 4163  sues/6))...## Ac
+00001840: 6b6e 6f77 6c65 6467 656d 656e 7473 0a0a  knowledgements..
+00001850: 2d20 5b59 7574 6120 4d6f 7269 5d28 6874  - [Yuta Mori](ht
+00001860: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001870: 2f79 2d32 3536 2920 666f 7220 7772 6974  /y-256) for writ
+00001880: 696e 6720 5b6c 6962 6469 7673 7566 736f  ing [libdivsufso
+00001890: 7274 5d28 6874 7470 733a 2f2f 6769 7468  rt](https://gith
+000018a0: 7562 2e63 6f6d 2f79 2d32 3536 2f6c 6962  ub.com/y-256/lib
+000018b0: 6469 7673 7566 736f 7274 290a 2d20 5b53  divsufsort).- [S
+000018c0: 6561 6e20 4c61 775d 2868 7474 703a 2f2f  ean Law](http://
+000018d0: 7365 616e 6c61 772e 6769 7468 7562 2e69  seanlaw.github.i
+000018e0: 6f2f 2920 666f 7220 696e 6974 6961 7469  o/) for initiati
+000018f0: 6e67 2074 6869 7320 7072 6f6a 6563 7420  ng this project 
+00001900: 616e 6420 636f 6e74 7269 6275 7469 6e67  and contributing
+00001910: 0a0a 2323 2043 6974 696e 670a 0a49 6620  ..## Citing..If 
+00001920: 796f 7520 6861 7665 2075 7365 6420 7468  you have used th
+00001930: 6973 2073 6f66 7477 6172 6520 696e 2061  is software in a
+00001940: 2073 6369 656e 7469 6669 6320 7075 626c   scientific publ
+00001950: 6963 6174 696f 6e2c 2070 6c65 6173 6520  ication, please 
+00001960: 6369 7465 2069 7420 7573 696e 6720 7468  cite it using th
+00001970: 6520 666f 6c6c 6f77 696e 6720 4269 624c  e following BibL
+00001980: 6154 6558 2063 6f64 653a 0a0a 6060 600a  aTeX code:..```.
+00001990: 4073 6f66 7477 6172 657b 7079 6469 7673  @software{pydivs
+000019a0: 7566 736f 7274 2c0a 2020 6175 7468 6f72  ufsort,.  author
+000019b0: 2020 2020 2020 203d 207b 4c6f 7569 7320         = {Louis 
+000019c0: 4162 7261 6861 6d7d 2c0a 2020 7469 746c  Abraham},.  titl
+000019d0: 6520 2020 2020 2020 203d 207b 7079 6469  e        = {pydi
+000019e0: 7673 7566 736f 7274 7d2c 0a20 2079 6561  vsufsort},.  yea
+000019f0: 7220 2020 2020 2020 2020 3d20 3230 3233  r         = 2023
+00001a00: 2c0a 2020 7075 626c 6973 6865 7220 2020  ,.  publisher   
+00001a10: 203d 207b 5a65 6e6f 646f 7d2c 0a20 2064   = {Zenodo},.  d
+00001a20: 6f69 2020 2020 2020 2020 2020 3d20 7b31  oi          = {1
+00001a30: 302e 3532 3831 2f7a 656e 6f64 6f2e 3739  0.5281/zenodo.79
+00001a40: 3332 3435 387d 2c0a 2020 7572 6c20 2020  32458},.  url   
+00001a50: 2020 2020 2020 203d 207b 6874 7470 733a         = {https:
+00001a60: 2f2f 6769 7468 7562 2e63 6f6d 2f6c 6f75  //github.com/lou
+00001a70: 6973 6162 7261 6861 6d2f 7079 6469 7673  isabraham/pydivs
+00001a80: 7566 736f 7274 7d0a 7d0a 6060 600a       ufsort}.}.```.
```

### Comparing `pydivsufsort-0.0.8/build.sh` & `pydivsufsort-0.0.9/build.sh`

 * *Files identical despite different names*

### Comparing `pydivsufsort-0.0.8/libdivsufsort/CHANGELOG.md` & `pydivsufsort-0.0.9/libdivsufsort/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pydivsufsort-0.0.8/libdivsufsort/CMakeLists.txt` & `pydivsufsort-0.0.9/libdivsufsort/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pydivsufsort-0.0.8/libdivsufsort/CMakeModules/AppendCompilerFlags.cmake` & `pydivsufsort-0.0.9/libdivsufsort/CMakeModules/AppendCompilerFlags.cmake`

 * *Files identical despite different names*

### Comparing `pydivsufsort-0.0.8/libdivsufsort/CMakeModules/CheckFunctionKeywords.cmake` & `pydivsufsort-0.0.9/libdivsufsort/CMakeModules/CheckFunctionKeywords.cmake`

 * *Files identical despite different names*

### Comparing `pydivsufsort-0.0.8/libdivsufsort/CMakeModules/CheckLFS.cmake` & `pydivsufsort-0.0.9/libdivsufsort/CMakeModules/CheckLFS.cmake`

 * *Files identical despite different names*

### Comparing `pydivsufsort-0.0.8/libdivsufsort/CMakeModules/ProjectCPack.cmake` & `pydivsufsort-0.0.9/libdivsufsort/CMakeModules/ProjectCPack.cmake`

 * *Files identical despite different names*

### Comparing `pydivsufsort-0.0.8/libdivsufsort/CMakeModules/cmake_uninstall.cmake.in` & `pydivsufsort-0.0.9/libdivsufsort/CMakeModules/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `pydivsufsort-0.0.8/libdivsufsort/LICENSE` & `pydivsufsort-0.0.9/libdivsufsort/LICENSE`

 * *Files identical despite different names*

### Comparing `pydivsufsort-0.0.8/libdivsufsort/README.md` & `pydivsufsort-0.0.9/libdivsufsort/README.md`

 * *Files identical despite different names*

### Comparing `pydivsufsort-0.0.8/libdivsufsort/VERSION.cmake` & `pydivsufsort-0.0.9/libdivsufsort/VERSION.cmake`

 * *Files identical despite different names*

### Comparing `pydivsufsort-0.0.8/libdivsufsort/examples/bwt.c` & `pydivsufsort-0.0.9/libdivsufsort/examples/bwt.c`

 * *Files identical despite different names*

### Comparing `pydivsufsort-0.0.8/libdivsufsort/examples/mksary.c` & `pydivsufsort-0.0.9/libdivsufsort/examples/mksary.c`

 * *Files identical despite different names*

### Comparing `pydivsufsort-0.0.8/libdivsufsort/examples/sasearch.c` & `pydivsufsort-0.0.9/libdivsufsort/examples/sasearch.c`

 * *Files identical despite different names*

### Comparing `pydivsufsort-0.0.8/libdivsufsort/examples/suftest.c` & `pydivsufsort-0.0.9/libdivsufsort/examples/suftest.c`

 * *Files identical despite different names*

### Comparing `pydivsufsort-0.0.8/libdivsufsort/examples/unbwt.c` & `pydivsufsort-0.0.9/libdivsufsort/examples/unbwt.c`

 * *Files identical despite different names*

### Comparing `pydivsufsort-0.0.8/libdivsufsort/include/CMakeLists.txt` & `pydivsufsort-0.0.9/libdivsufsort/include/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pydivsufsort-0.0.8/libdivsufsort/include/config.h.cmake` & `pydivsufsort-0.0.9/libdivsufsort/include/config.h.cmake`

 * *Files identical despite different names*

### Comparing `pydivsufsort-0.0.8/libdivsufsort/include/divsufsort.h.cmake` & `pydivsufsort-0.0.9/libdivsufsort/include/divsufsort.h.cmake`

 * *Files identical despite different names*

### Comparing `pydivsufsort-0.0.8/libdivsufsort/include/divsufsort_private.h` & `pydivsufsort-0.0.9/libdivsufsort/include/divsufsort_private.h`

 * *Files identical despite different names*

### Comparing `pydivsufsort-0.0.8/libdivsufsort/include/lfs.h.cmake` & `pydivsufsort-0.0.9/libdivsufsort/include/lfs.h.cmake`

 * *Files identical despite different names*

### Comparing `pydivsufsort-0.0.8/libdivsufsort/lib/CMakeLists.txt` & `pydivsufsort-0.0.9/libdivsufsort/lib/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pydivsufsort-0.0.8/libdivsufsort/lib/divsufsort.c` & `pydivsufsort-0.0.9/libdivsufsort/lib/divsufsort.c`

 * *Files identical despite different names*

### Comparing `pydivsufsort-0.0.8/libdivsufsort/lib/sssort.c` & `pydivsufsort-0.0.9/libdivsufsort/lib/sssort.c`

 * *Files identical despite different names*

### Comparing `pydivsufsort-0.0.8/libdivsufsort/lib/trsort.c` & `pydivsufsort-0.0.9/libdivsufsort/lib/trsort.c`

 * *Files identical despite different names*

### Comparing `pydivsufsort-0.0.8/libdivsufsort/lib/utils.c` & `pydivsufsort-0.0.9/libdivsufsort/lib/utils.c`

 * *Files identical despite different names*

### Comparing `pydivsufsort-0.0.8/libdivsufsort/pkgconfig/CMakeLists.txt` & `pydivsufsort-0.0.9/libdivsufsort/pkgconfig/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pydivsufsort-0.0.8/pydivsufsort/divsufsort.py` & `pydivsufsort-0.0.9/pydivsufsort/divsufsort.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,16 +49,15 @@
 
 _SUPPORTED_DTYPES = {
     np.dtype(f"{signed}int{bits}") for signed in ["", "u"] for bits in [8, 16, 32, 64]
 }
 
 
 def _get_bytes_pointer(inp):
-    """Returns pointer to bytes-like input
-    """
+    """Returns pointer to bytes-like input"""
     if isinstance(inp, np.ndarray):
         assert inp.dtype == np.uint8
         # https://stackoverflow.com/q/60848009/5133167
         if not inp.flags["C_CONTIGUOUS"]:
             # Make a contiguous copy of the numpy array.
             inp = np.ascontiguousarray(inp)
         return ctypes.pointer(np.ctypeslib.as_ctypes(inp))
```

### Comparing `pydivsufsort-0.0.8/pydivsufsort/dll.py` & `pydivsufsort-0.0.9/pydivsufsort/dll.py`

 * *Files identical despite different names*

### Comparing `pydivsufsort-0.0.8/pydivsufsort/stringalg.cpp` & `pydivsufsort-0.0.9/pydivsufsort/stringalg.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 /* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "extra_compile_args": [
             "-O3"
         ],
         "include_dirs": [
-            "/tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/core/include"
+            "/tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/core/include"
         ],
         "language": "c++",
         "name": "pydivsufsort.stringalg",
         "sources": [
             "pydivsufsort/stringalg.pyx"
         ]
     },
@@ -1151,195 +1151,195 @@
 #define __Pyx_PyGILState_Ensure PyGILState_Ensure
 #define __Pyx_PyGILState_Release PyGILState_Release
 #define __Pyx_FastGIL_Remember()
 #define __Pyx_FastGIL_Forget()
 #define __Pyx_FastGilFuncInit()
 
 
-/* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":689
+/* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":696
+/* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":703
+/* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":713
+/* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":717
+/* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":721
+/* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":724
+/* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1379,42 +1379,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":728
+/* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":732
+/* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2900,29 +2900,30 @@
 static const char __pyx_k_uint16_t[] = "uint16_t";
 static const char __pyx_k_uint32_t[] = "uint32_t";
 static const char __pyx_k_uint64_t[] = "uint64_t";
 static const char __pyx_k_warnings[] = "warnings";
 static const char __pyx_k_TypeError[] = "TypeError";
 static const char __pyx_k_cur_count[] = "cur_count";
 static const char __pyx_k_enumerate[] = "enumerate";
-static const char __pyx_k_lcp_query[] = "lcp_query";
+static const char __pyx_k_lcp_query[] = "_lcp_query";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_IndexError[] = "IndexError";
 static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_divsufsort[] = "divsufsort";
 static const char __pyx_k_empty_like[] = "empty_like";
 static const char __pyx_k_pyx_result[] = "__pyx_result";
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
 static const char __pyx_k_signatures[] = "signatures";
 static const char __pyx_k_ImportError[] = "ImportError";
 static const char __pyx_k_MemoryError[] = "MemoryError";
 static const char __pyx_k_PickleError[] = "PickleError";
 static const char __pyx_k_concatenate[] = "concatenate";
 static const char __pyx_k_kasai_bytes[] = "_kasai_bytes";
+static const char __pyx_k_lcp_query_2[] = "lcp_query";
 static const char __pyx_k_lcp_segtree[] = "_lcp_segtree";
 static const char __pyx_k_levenshtein[] = "_levenshtein";
 static const char __pyx_k_C_CONTIGUOUS[] = "C_CONTIGUOUS";
 static const char __pyx_k_handle_input[] = "handle_input";
 static const char __pyx_k_pyx_checksum[] = "__pyx_checksum";
 static const char __pyx_k_stringsource[] = "stringsource";
 static const char __pyx_k_suffix_array[] = "suffix_array";
@@ -3094,14 +3095,15 @@
 static PyObject *__pyx_n_s_key;
 static PyObject *__pyx_n_s_kind;
 static PyObject *__pyx_n_s_kwargs;
 static PyObject *__pyx_n_s_l;
 static PyObject *__pyx_n_s_last;
 static PyObject *__pyx_n_s_lcp;
 static PyObject *__pyx_n_s_lcp_query;
+static PyObject *__pyx_n_s_lcp_query_2;
 static PyObject *__pyx_n_s_lcp_segtree;
 static PyObject *__pyx_n_s_lcp_segtree_2;
 static PyObject *__pyx_n_s_len1;
 static PyObject *__pyx_n_s_length;
 static PyObject *__pyx_n_s_levenshtein;
 static PyObject *__pyx_n_s_levenshtein_2;
 static PyObject *__pyx_n_s_limit;
@@ -3189,15 +3191,14 @@
 static PyObject *__pyx_kp_s_unable_to_allocate_shape_and_str;
 static PyObject *__pyx_n_s_unpack;
 static PyObject *__pyx_n_s_update;
 static PyObject *__pyx_n_s_warn;
 static PyObject *__pyx_n_s_warnings;
 static PyObject *__pyx_pf_12pydivsufsort_9stringalg_handle_input(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s); /* proto */
 static PyObject *__pyx_pf_12pydivsufsort_9stringalg_2_kasai(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_signatures, PyObject *__pyx_v_args, PyObject *__pyx_v_kwargs, CYTHON_UNUSED PyObject *__pyx_v_defaults); /* proto */
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_24_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa); /* proto */
 static PyObject *__pyx_pf_12pydivsufsort_9stringalg_26_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa); /* proto */
 static PyObject *__pyx_pf_12pydivsufsort_9stringalg_28_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa); /* proto */
 static PyObject *__pyx_pf_12pydivsufsort_9stringalg_30_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa); /* proto */
 static PyObject *__pyx_pf_12pydivsufsort_9stringalg_32_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa); /* proto */
 static PyObject *__pyx_pf_12pydivsufsort_9stringalg_34_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa); /* proto */
 static PyObject *__pyx_pf_12pydivsufsort_9stringalg_36_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa); /* proto */
 static PyObject *__pyx_pf_12pydivsufsort_9stringalg_38_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa); /* proto */
@@ -3205,20 +3206,20 @@
 static PyObject *__pyx_pf_12pydivsufsort_9stringalg_42_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa); /* proto */
 static PyObject *__pyx_pf_12pydivsufsort_9stringalg_44_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa); /* proto */
 static PyObject *__pyx_pf_12pydivsufsort_9stringalg_46_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa); /* proto */
 static PyObject *__pyx_pf_12pydivsufsort_9stringalg_48_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa); /* proto */
 static PyObject *__pyx_pf_12pydivsufsort_9stringalg_50_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa); /* proto */
 static PyObject *__pyx_pf_12pydivsufsort_9stringalg_52_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa); /* proto */
 static PyObject *__pyx_pf_12pydivsufsort_9stringalg_54_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa); /* proto */
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_56_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa); /* proto */
 static PyObject *__pyx_pf_12pydivsufsort_9stringalg_4_kasai_bytes(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_signatures, PyObject *__pyx_v_args, PyObject *__pyx_v_kwargs, CYTHON_UNUSED PyObject *__pyx_v_defaults); /* proto */
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_58_kasai_bytes(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa); /* proto */
 static PyObject *__pyx_pf_12pydivsufsort_9stringalg_60_kasai_bytes(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa); /* proto */
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_62_kasai_bytes(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa); /* proto */
 static PyObject *__pyx_pf_12pydivsufsort_9stringalg_6kasai(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s, PyObject *__pyx_v_sa); /* proto */
 static PyObject *__pyx_pf_12pydivsufsort_9stringalg_8_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_signatures, PyObject *__pyx_v_args, PyObject *__pyx_v_kwargs, CYTHON_UNUSED PyObject *__pyx_v_defaults); /* proto */
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_64_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp); /* proto */
 static PyObject *__pyx_pf_12pydivsufsort_9stringalg_66_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp); /* proto */
 static PyObject *__pyx_pf_12pydivsufsort_9stringalg_68_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp); /* proto */
 static PyObject *__pyx_pf_12pydivsufsort_9stringalg_70_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp); /* proto */
 static PyObject *__pyx_pf_12pydivsufsort_9stringalg_72_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp); /* proto */
 static PyObject *__pyx_pf_12pydivsufsort_9stringalg_74_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp); /* proto */
 static PyObject *__pyx_pf_12pydivsufsort_9stringalg_76_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp); /* proto */
 static PyObject *__pyx_pf_12pydivsufsort_9stringalg_78_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp); /* proto */
@@ -3226,36 +3227,38 @@
 static PyObject *__pyx_pf_12pydivsufsort_9stringalg_82_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp); /* proto */
 static PyObject *__pyx_pf_12pydivsufsort_9stringalg_84_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp); /* proto */
 static PyObject *__pyx_pf_12pydivsufsort_9stringalg_86_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp); /* proto */
 static PyObject *__pyx_pf_12pydivsufsort_9stringalg_88_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp); /* proto */
 static PyObject *__pyx_pf_12pydivsufsort_9stringalg_90_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp); /* proto */
 static PyObject *__pyx_pf_12pydivsufsort_9stringalg_92_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp); /* proto */
 static PyObject *__pyx_pf_12pydivsufsort_9stringalg_94_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp); /* proto */
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_96_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp); /* proto */
 static PyObject *__pyx_pf_12pydivsufsort_9stringalg_10lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s, PyObject *__pyx_v_sa, PyObject *__pyx_v_lcp); /* proto */
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_12lcp_query(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_signatures, PyObject *__pyx_v_args, PyObject *__pyx_v_kwargs, CYTHON_UNUSED PyObject *__pyx_v_defaults); /* proto */
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_98lcp_query(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_rank, PyArrayObject *__pyx_v_segtree, PyObject *__pyx_v_queries); /* proto */
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_100lcp_query(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_rank, PyArrayObject *__pyx_v_segtree, PyObject *__pyx_v_queries); /* proto */
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_14_levenshtein(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_signatures, PyObject *__pyx_v_args, PyObject *__pyx_v_kwargs, CYTHON_UNUSED PyObject *__pyx_v_defaults); /* proto */
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_104_levenshtein(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_a, __Pyx_memviewslice __pyx_v_b); /* proto */
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_12_lcp_query(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_signatures, PyObject *__pyx_v_args, PyObject *__pyx_v_kwargs, CYTHON_UNUSED PyObject *__pyx_v_defaults); /* proto */
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_100_lcp_query(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_rank, PyArrayObject *__pyx_v_segtree, PyObject *__pyx_v_queries); /* proto */
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_102_lcp_query(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_rank, PyArrayObject *__pyx_v_segtree, PyObject *__pyx_v_queries); /* proto */
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_14lcp_query(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_segtree, PyObject *__pyx_v_queries); /* proto */
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_16_levenshtein(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_signatures, PyObject *__pyx_v_args, PyObject *__pyx_v_kwargs, CYTHON_UNUSED PyObject *__pyx_v_defaults); /* proto */
 static PyObject *__pyx_pf_12pydivsufsort_9stringalg_106_levenshtein(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_a, __Pyx_memviewslice __pyx_v_b); /* proto */
 static PyObject *__pyx_pf_12pydivsufsort_9stringalg_108_levenshtein(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_a, __Pyx_memviewslice __pyx_v_b); /* proto */
 static PyObject *__pyx_pf_12pydivsufsort_9stringalg_110_levenshtein(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_a, __Pyx_memviewslice __pyx_v_b); /* proto */
 static PyObject *__pyx_pf_12pydivsufsort_9stringalg_112_levenshtein(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_a, __Pyx_memviewslice __pyx_v_b); /* proto */
 static PyObject *__pyx_pf_12pydivsufsort_9stringalg_114_levenshtein(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_a, __Pyx_memviewslice __pyx_v_b); /* proto */
 static PyObject *__pyx_pf_12pydivsufsort_9stringalg_116_levenshtein(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_a, __Pyx_memviewslice __pyx_v_b); /* proto */
 static PyObject *__pyx_pf_12pydivsufsort_9stringalg_118_levenshtein(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_a, __Pyx_memviewslice __pyx_v_b); /* proto */
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_16levenshtein(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_a, PyObject *__pyx_v_b); /* proto */
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_18most_frequent_substrings(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_signatures, PyObject *__pyx_v_args, PyObject *__pyx_v_kwargs, CYTHON_UNUSED PyObject *__pyx_v_defaults); /* proto */
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_132__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_122most_frequent_substrings(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_lcp, __pyx_t_5numpy_int32_t __pyx_v_length, __pyx_t_5numpy_int32_t __pyx_v_limit, __pyx_t_5numpy_int32_t __pyx_v_minimum_count); /* proto */
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_120_levenshtein(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_a, __Pyx_memviewslice __pyx_v_b); /* proto */
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_18levenshtein(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_a, PyObject *__pyx_v_b); /* proto */
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_20most_frequent_substrings(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_signatures, PyObject *__pyx_v_args, PyObject *__pyx_v_kwargs, CYTHON_UNUSED PyObject *__pyx_v_defaults); /* proto */
 static PyObject *__pyx_pf_12pydivsufsort_9stringalg_134__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_124most_frequent_substrings(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_lcp, __pyx_t_5numpy_int64_t __pyx_v_length, __pyx_t_5numpy_int64_t __pyx_v_limit, __pyx_t_5numpy_int64_t __pyx_v_minimum_count); /* proto */
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_20repeated_substrings(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_suffix_array, __Pyx_memviewslice __pyx_v_lcp); /* proto */
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_124most_frequent_substrings(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_lcp, __pyx_t_5numpy_int32_t __pyx_v_length, __pyx_t_5numpy_int32_t __pyx_v_limit, __pyx_t_5numpy_int32_t __pyx_v_minimum_count); /* proto */
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_136__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_126most_frequent_substrings(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_lcp, __pyx_t_5numpy_int64_t __pyx_v_length, __pyx_t_5numpy_int64_t __pyx_v_limit, __pyx_t_5numpy_int64_t __pyx_v_minimum_count); /* proto */
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_22repeated_substrings(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_suffix_array, __Pyx_memviewslice __pyx_v_lcp); /* proto */
 static PyObject *__pyx_lambda_funcdef_lambda(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_x); /* proto */
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_22_common_substrings(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_suffix_array, __Pyx_memviewslice __pyx_v_lcp, __pyx_t_12pydivsufsort_9stringalg_ull __pyx_v_len1, __pyx_t_12pydivsufsort_9stringalg_ull __pyx_v_limit); /* proto */
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_24_common_substrings(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_suffix_array, __Pyx_memviewslice __pyx_v_lcp, __pyx_t_12pydivsufsort_9stringalg_ull __pyx_v_len1, __pyx_t_12pydivsufsort_9stringalg_ull __pyx_v_limit); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array___cinit__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_shape, Py_ssize_t __pyx_v_itemsize, PyObject *__pyx_v_format, PyObject *__pyx_v_mode, int __pyx_v_allocate_buffer); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array_2__getbuffer__(struct __pyx_array_obj *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /* proto */
 static void __pyx_array___pyx_pf_15View_dot_MemoryView_5array_4__dealloc__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView_5array_7memview___get__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static Py_ssize_t __pyx_array___pyx_pf_15View_dot_MemoryView_5array_6__len__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_8__getattr__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_attr); /* proto */
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_10__getitem__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_item); /* proto */
@@ -3341,31 +3344,33 @@
 static PyObject *__pyx_tuple__40;
 static PyObject *__pyx_tuple__42;
 static PyObject *__pyx_tuple__44;
 static PyObject *__pyx_tuple__46;
 static PyObject *__pyx_tuple__48;
 static PyObject *__pyx_tuple__50;
 static PyObject *__pyx_tuple__52;
-static PyObject *__pyx_tuple__53;
 static PyObject *__pyx_tuple__54;
 static PyObject *__pyx_tuple__55;
 static PyObject *__pyx_tuple__56;
 static PyObject *__pyx_tuple__57;
+static PyObject *__pyx_tuple__58;
+static PyObject *__pyx_tuple__59;
 static PyObject *__pyx_codeobj__31;
 static PyObject *__pyx_codeobj__33;
 static PyObject *__pyx_codeobj__35;
 static PyObject *__pyx_codeobj__37;
 static PyObject *__pyx_codeobj__39;
 static PyObject *__pyx_codeobj__41;
 static PyObject *__pyx_codeobj__43;
 static PyObject *__pyx_codeobj__45;
 static PyObject *__pyx_codeobj__47;
 static PyObject *__pyx_codeobj__49;
 static PyObject *__pyx_codeobj__51;
-static PyObject *__pyx_codeobj__58;
+static PyObject *__pyx_codeobj__53;
+static PyObject *__pyx_codeobj__60;
 /* Late includes */
 
 /* "pydivsufsort/stringalg.pyx":26
  *     np.int64_t
  * 
  * def handle_input(s):             # <<<<<<<<<<<<<<
  *     if isinstance(s, np.ndarray):
@@ -4766,17 +4771,17 @@
   __Pyx_XDECREF(__pyx_v_kwargs);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_0_0__pyx_pw_12pydivsufsort_9stringalg_25_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_0_0__pyx_mdef_12pydivsufsort_9stringalg_25_kasai = {"__pyx_fuse_0_0_kasai", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_0_0__pyx_pw_12pydivsufsort_9stringalg_25_kasai, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_fuse_0_0__pyx_pw_12pydivsufsort_9stringalg_25_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_0_0__pyx_pw_12pydivsufsort_9stringalg_27_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_0_0__pyx_mdef_12pydivsufsort_9stringalg_27_kasai = {"__pyx_fuse_0_0_kasai", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_0_0__pyx_pw_12pydivsufsort_9stringalg_27_kasai, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_fuse_0_0__pyx_pw_12pydivsufsort_9stringalg_27_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_s = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_sa = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -4829,26 +4834,26 @@
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(((PyObject *)__pyx_v_s.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "s"); __PYX_ERR(0, 47, __pyx_L1_error)
   }
   if (unlikely(((PyObject *)__pyx_v_sa.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "sa"); __PYX_ERR(0, 47, __pyx_L1_error)
   }
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_24_kasai(__pyx_self, __pyx_v_s, __pyx_v_sa);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_26_kasai(__pyx_self, __pyx_v_s, __pyx_v_sa);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_24_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_26_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa) {
   __pyx_t_5numpy_int32_t __pyx_v_i;
   __pyx_t_5numpy_int32_t __pyx_v_j;
   __pyx_t_5numpy_int32_t __pyx_v_n;
   __pyx_t_5numpy_int32_t __pyx_v_k;
   PyArrayObject *__pyx_v_lcp = 0;
   PyArrayObject *__pyx_v_rank = 0;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_lcp;
@@ -5202,17 +5207,17 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_sa, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_0_1__pyx_pw_12pydivsufsort_9stringalg_27_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_0_1__pyx_mdef_12pydivsufsort_9stringalg_27_kasai = {"__pyx_fuse_0_1_kasai", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_0_1__pyx_pw_12pydivsufsort_9stringalg_27_kasai, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_fuse_0_1__pyx_pw_12pydivsufsort_9stringalg_27_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_0_1__pyx_pw_12pydivsufsort_9stringalg_29_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_0_1__pyx_mdef_12pydivsufsort_9stringalg_29_kasai = {"__pyx_fuse_0_1_kasai", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_0_1__pyx_pw_12pydivsufsort_9stringalg_29_kasai, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_fuse_0_1__pyx_pw_12pydivsufsort_9stringalg_29_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_s = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_sa = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -5265,26 +5270,26 @@
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(((PyObject *)__pyx_v_s.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "s"); __PYX_ERR(0, 47, __pyx_L1_error)
   }
   if (unlikely(((PyObject *)__pyx_v_sa.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "sa"); __PYX_ERR(0, 47, __pyx_L1_error)
   }
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_26_kasai(__pyx_self, __pyx_v_s, __pyx_v_sa);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_28_kasai(__pyx_self, __pyx_v_s, __pyx_v_sa);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_26_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_28_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa) {
   __pyx_t_5numpy_int64_t __pyx_v_i;
   __pyx_t_5numpy_int64_t __pyx_v_j;
   __pyx_t_5numpy_int64_t __pyx_v_n;
   __pyx_t_5numpy_int64_t __pyx_v_k;
   PyArrayObject *__pyx_v_lcp = 0;
   PyArrayObject *__pyx_v_rank = 0;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_lcp;
@@ -5638,17 +5643,17 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_sa, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_1_0__pyx_pw_12pydivsufsort_9stringalg_29_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_1_0__pyx_mdef_12pydivsufsort_9stringalg_29_kasai = {"__pyx_fuse_1_0_kasai", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_1_0__pyx_pw_12pydivsufsort_9stringalg_29_kasai, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_fuse_1_0__pyx_pw_12pydivsufsort_9stringalg_29_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_1_0__pyx_pw_12pydivsufsort_9stringalg_31_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_1_0__pyx_mdef_12pydivsufsort_9stringalg_31_kasai = {"__pyx_fuse_1_0_kasai", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_1_0__pyx_pw_12pydivsufsort_9stringalg_31_kasai, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_fuse_1_0__pyx_pw_12pydivsufsort_9stringalg_31_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_s = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_sa = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -5701,26 +5706,26 @@
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(((PyObject *)__pyx_v_s.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "s"); __PYX_ERR(0, 47, __pyx_L1_error)
   }
   if (unlikely(((PyObject *)__pyx_v_sa.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "sa"); __PYX_ERR(0, 47, __pyx_L1_error)
   }
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_28_kasai(__pyx_self, __pyx_v_s, __pyx_v_sa);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_30_kasai(__pyx_self, __pyx_v_s, __pyx_v_sa);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_28_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_30_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa) {
   __pyx_t_5numpy_int32_t __pyx_v_i;
   __pyx_t_5numpy_int32_t __pyx_v_j;
   __pyx_t_5numpy_int32_t __pyx_v_n;
   __pyx_t_5numpy_int32_t __pyx_v_k;
   PyArrayObject *__pyx_v_lcp = 0;
   PyArrayObject *__pyx_v_rank = 0;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_lcp;
@@ -6074,17 +6079,17 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_sa, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_1_1__pyx_pw_12pydivsufsort_9stringalg_31_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_1_1__pyx_mdef_12pydivsufsort_9stringalg_31_kasai = {"__pyx_fuse_1_1_kasai", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_1_1__pyx_pw_12pydivsufsort_9stringalg_31_kasai, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_fuse_1_1__pyx_pw_12pydivsufsort_9stringalg_31_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_1_1__pyx_pw_12pydivsufsort_9stringalg_33_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_1_1__pyx_mdef_12pydivsufsort_9stringalg_33_kasai = {"__pyx_fuse_1_1_kasai", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_1_1__pyx_pw_12pydivsufsort_9stringalg_33_kasai, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_fuse_1_1__pyx_pw_12pydivsufsort_9stringalg_33_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_s = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_sa = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -6137,26 +6142,26 @@
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(((PyObject *)__pyx_v_s.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "s"); __PYX_ERR(0, 47, __pyx_L1_error)
   }
   if (unlikely(((PyObject *)__pyx_v_sa.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "sa"); __PYX_ERR(0, 47, __pyx_L1_error)
   }
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_30_kasai(__pyx_self, __pyx_v_s, __pyx_v_sa);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_32_kasai(__pyx_self, __pyx_v_s, __pyx_v_sa);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_30_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_32_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa) {
   __pyx_t_5numpy_int64_t __pyx_v_i;
   __pyx_t_5numpy_int64_t __pyx_v_j;
   __pyx_t_5numpy_int64_t __pyx_v_n;
   __pyx_t_5numpy_int64_t __pyx_v_k;
   PyArrayObject *__pyx_v_lcp = 0;
   PyArrayObject *__pyx_v_rank = 0;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_lcp;
@@ -6510,17 +6515,17 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_sa, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_2_0__pyx_pw_12pydivsufsort_9stringalg_33_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_2_0__pyx_mdef_12pydivsufsort_9stringalg_33_kasai = {"__pyx_fuse_2_0_kasai", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_2_0__pyx_pw_12pydivsufsort_9stringalg_33_kasai, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_fuse_2_0__pyx_pw_12pydivsufsort_9stringalg_33_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_2_0__pyx_pw_12pydivsufsort_9stringalg_35_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_2_0__pyx_mdef_12pydivsufsort_9stringalg_35_kasai = {"__pyx_fuse_2_0_kasai", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_2_0__pyx_pw_12pydivsufsort_9stringalg_35_kasai, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_fuse_2_0__pyx_pw_12pydivsufsort_9stringalg_35_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_s = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_sa = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -6573,26 +6578,26 @@
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(((PyObject *)__pyx_v_s.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "s"); __PYX_ERR(0, 47, __pyx_L1_error)
   }
   if (unlikely(((PyObject *)__pyx_v_sa.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "sa"); __PYX_ERR(0, 47, __pyx_L1_error)
   }
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_32_kasai(__pyx_self, __pyx_v_s, __pyx_v_sa);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_34_kasai(__pyx_self, __pyx_v_s, __pyx_v_sa);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_32_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_34_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa) {
   __pyx_t_5numpy_int32_t __pyx_v_i;
   __pyx_t_5numpy_int32_t __pyx_v_j;
   __pyx_t_5numpy_int32_t __pyx_v_n;
   __pyx_t_5numpy_int32_t __pyx_v_k;
   PyArrayObject *__pyx_v_lcp = 0;
   PyArrayObject *__pyx_v_rank = 0;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_lcp;
@@ -6946,17 +6951,17 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_sa, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_2_1__pyx_pw_12pydivsufsort_9stringalg_35_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_2_1__pyx_mdef_12pydivsufsort_9stringalg_35_kasai = {"__pyx_fuse_2_1_kasai", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_2_1__pyx_pw_12pydivsufsort_9stringalg_35_kasai, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_fuse_2_1__pyx_pw_12pydivsufsort_9stringalg_35_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_2_1__pyx_pw_12pydivsufsort_9stringalg_37_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_2_1__pyx_mdef_12pydivsufsort_9stringalg_37_kasai = {"__pyx_fuse_2_1_kasai", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_2_1__pyx_pw_12pydivsufsort_9stringalg_37_kasai, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_fuse_2_1__pyx_pw_12pydivsufsort_9stringalg_37_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_s = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_sa = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -7009,26 +7014,26 @@
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(((PyObject *)__pyx_v_s.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "s"); __PYX_ERR(0, 47, __pyx_L1_error)
   }
   if (unlikely(((PyObject *)__pyx_v_sa.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "sa"); __PYX_ERR(0, 47, __pyx_L1_error)
   }
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_34_kasai(__pyx_self, __pyx_v_s, __pyx_v_sa);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_36_kasai(__pyx_self, __pyx_v_s, __pyx_v_sa);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_34_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_36_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa) {
   __pyx_t_5numpy_int64_t __pyx_v_i;
   __pyx_t_5numpy_int64_t __pyx_v_j;
   __pyx_t_5numpy_int64_t __pyx_v_n;
   __pyx_t_5numpy_int64_t __pyx_v_k;
   PyArrayObject *__pyx_v_lcp = 0;
   PyArrayObject *__pyx_v_rank = 0;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_lcp;
@@ -7382,17 +7387,17 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_sa, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_3_0__pyx_pw_12pydivsufsort_9stringalg_37_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_3_0__pyx_mdef_12pydivsufsort_9stringalg_37_kasai = {"__pyx_fuse_3_0_kasai", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_3_0__pyx_pw_12pydivsufsort_9stringalg_37_kasai, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_fuse_3_0__pyx_pw_12pydivsufsort_9stringalg_37_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_3_0__pyx_pw_12pydivsufsort_9stringalg_39_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_3_0__pyx_mdef_12pydivsufsort_9stringalg_39_kasai = {"__pyx_fuse_3_0_kasai", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_3_0__pyx_pw_12pydivsufsort_9stringalg_39_kasai, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_fuse_3_0__pyx_pw_12pydivsufsort_9stringalg_39_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_s = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_sa = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -7445,26 +7450,26 @@
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(((PyObject *)__pyx_v_s.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "s"); __PYX_ERR(0, 47, __pyx_L1_error)
   }
   if (unlikely(((PyObject *)__pyx_v_sa.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "sa"); __PYX_ERR(0, 47, __pyx_L1_error)
   }
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_36_kasai(__pyx_self, __pyx_v_s, __pyx_v_sa);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_38_kasai(__pyx_self, __pyx_v_s, __pyx_v_sa);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_36_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_38_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa) {
   __pyx_t_5numpy_int32_t __pyx_v_i;
   __pyx_t_5numpy_int32_t __pyx_v_j;
   __pyx_t_5numpy_int32_t __pyx_v_n;
   __pyx_t_5numpy_int32_t __pyx_v_k;
   PyArrayObject *__pyx_v_lcp = 0;
   PyArrayObject *__pyx_v_rank = 0;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_lcp;
@@ -7818,17 +7823,17 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_sa, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_3_1__pyx_pw_12pydivsufsort_9stringalg_39_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_3_1__pyx_mdef_12pydivsufsort_9stringalg_39_kasai = {"__pyx_fuse_3_1_kasai", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_3_1__pyx_pw_12pydivsufsort_9stringalg_39_kasai, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_fuse_3_1__pyx_pw_12pydivsufsort_9stringalg_39_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_3_1__pyx_pw_12pydivsufsort_9stringalg_41_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_3_1__pyx_mdef_12pydivsufsort_9stringalg_41_kasai = {"__pyx_fuse_3_1_kasai", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_3_1__pyx_pw_12pydivsufsort_9stringalg_41_kasai, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_fuse_3_1__pyx_pw_12pydivsufsort_9stringalg_41_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_s = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_sa = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -7881,26 +7886,26 @@
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(((PyObject *)__pyx_v_s.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "s"); __PYX_ERR(0, 47, __pyx_L1_error)
   }
   if (unlikely(((PyObject *)__pyx_v_sa.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "sa"); __PYX_ERR(0, 47, __pyx_L1_error)
   }
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_38_kasai(__pyx_self, __pyx_v_s, __pyx_v_sa);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_40_kasai(__pyx_self, __pyx_v_s, __pyx_v_sa);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_38_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_40_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa) {
   __pyx_t_5numpy_int64_t __pyx_v_i;
   __pyx_t_5numpy_int64_t __pyx_v_j;
   __pyx_t_5numpy_int64_t __pyx_v_n;
   __pyx_t_5numpy_int64_t __pyx_v_k;
   PyArrayObject *__pyx_v_lcp = 0;
   PyArrayObject *__pyx_v_rank = 0;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_lcp;
@@ -8254,17 +8259,17 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_sa, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_4_0__pyx_pw_12pydivsufsort_9stringalg_41_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_4_0__pyx_mdef_12pydivsufsort_9stringalg_41_kasai = {"__pyx_fuse_4_0_kasai", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_4_0__pyx_pw_12pydivsufsort_9stringalg_41_kasai, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_fuse_4_0__pyx_pw_12pydivsufsort_9stringalg_41_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_4_0__pyx_pw_12pydivsufsort_9stringalg_43_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_4_0__pyx_mdef_12pydivsufsort_9stringalg_43_kasai = {"__pyx_fuse_4_0_kasai", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_4_0__pyx_pw_12pydivsufsort_9stringalg_43_kasai, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_fuse_4_0__pyx_pw_12pydivsufsort_9stringalg_43_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_s = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_sa = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -8317,26 +8322,26 @@
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(((PyObject *)__pyx_v_s.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "s"); __PYX_ERR(0, 47, __pyx_L1_error)
   }
   if (unlikely(((PyObject *)__pyx_v_sa.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "sa"); __PYX_ERR(0, 47, __pyx_L1_error)
   }
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_40_kasai(__pyx_self, __pyx_v_s, __pyx_v_sa);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_42_kasai(__pyx_self, __pyx_v_s, __pyx_v_sa);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_40_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_42_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa) {
   __pyx_t_5numpy_int32_t __pyx_v_i;
   __pyx_t_5numpy_int32_t __pyx_v_j;
   __pyx_t_5numpy_int32_t __pyx_v_n;
   __pyx_t_5numpy_int32_t __pyx_v_k;
   PyArrayObject *__pyx_v_lcp = 0;
   PyArrayObject *__pyx_v_rank = 0;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_lcp;
@@ -8690,17 +8695,17 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_sa, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_4_1__pyx_pw_12pydivsufsort_9stringalg_43_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_4_1__pyx_mdef_12pydivsufsort_9stringalg_43_kasai = {"__pyx_fuse_4_1_kasai", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_4_1__pyx_pw_12pydivsufsort_9stringalg_43_kasai, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_fuse_4_1__pyx_pw_12pydivsufsort_9stringalg_43_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_4_1__pyx_pw_12pydivsufsort_9stringalg_45_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_4_1__pyx_mdef_12pydivsufsort_9stringalg_45_kasai = {"__pyx_fuse_4_1_kasai", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_4_1__pyx_pw_12pydivsufsort_9stringalg_45_kasai, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_fuse_4_1__pyx_pw_12pydivsufsort_9stringalg_45_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_s = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_sa = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -8753,26 +8758,26 @@
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(((PyObject *)__pyx_v_s.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "s"); __PYX_ERR(0, 47, __pyx_L1_error)
   }
   if (unlikely(((PyObject *)__pyx_v_sa.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "sa"); __PYX_ERR(0, 47, __pyx_L1_error)
   }
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_42_kasai(__pyx_self, __pyx_v_s, __pyx_v_sa);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_44_kasai(__pyx_self, __pyx_v_s, __pyx_v_sa);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_42_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_44_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa) {
   __pyx_t_5numpy_int64_t __pyx_v_i;
   __pyx_t_5numpy_int64_t __pyx_v_j;
   __pyx_t_5numpy_int64_t __pyx_v_n;
   __pyx_t_5numpy_int64_t __pyx_v_k;
   PyArrayObject *__pyx_v_lcp = 0;
   PyArrayObject *__pyx_v_rank = 0;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_lcp;
@@ -9126,17 +9131,17 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_sa, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_5_0__pyx_pw_12pydivsufsort_9stringalg_45_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_5_0__pyx_mdef_12pydivsufsort_9stringalg_45_kasai = {"__pyx_fuse_5_0_kasai", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_5_0__pyx_pw_12pydivsufsort_9stringalg_45_kasai, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_fuse_5_0__pyx_pw_12pydivsufsort_9stringalg_45_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_5_0__pyx_pw_12pydivsufsort_9stringalg_47_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_5_0__pyx_mdef_12pydivsufsort_9stringalg_47_kasai = {"__pyx_fuse_5_0_kasai", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_5_0__pyx_pw_12pydivsufsort_9stringalg_47_kasai, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_fuse_5_0__pyx_pw_12pydivsufsort_9stringalg_47_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_s = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_sa = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -9189,26 +9194,26 @@
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(((PyObject *)__pyx_v_s.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "s"); __PYX_ERR(0, 47, __pyx_L1_error)
   }
   if (unlikely(((PyObject *)__pyx_v_sa.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "sa"); __PYX_ERR(0, 47, __pyx_L1_error)
   }
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_44_kasai(__pyx_self, __pyx_v_s, __pyx_v_sa);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_46_kasai(__pyx_self, __pyx_v_s, __pyx_v_sa);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_44_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_46_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa) {
   __pyx_t_5numpy_int32_t __pyx_v_i;
   __pyx_t_5numpy_int32_t __pyx_v_j;
   __pyx_t_5numpy_int32_t __pyx_v_n;
   __pyx_t_5numpy_int32_t __pyx_v_k;
   PyArrayObject *__pyx_v_lcp = 0;
   PyArrayObject *__pyx_v_rank = 0;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_lcp;
@@ -9562,17 +9567,17 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_sa, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_5_1__pyx_pw_12pydivsufsort_9stringalg_47_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_5_1__pyx_mdef_12pydivsufsort_9stringalg_47_kasai = {"__pyx_fuse_5_1_kasai", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_5_1__pyx_pw_12pydivsufsort_9stringalg_47_kasai, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_fuse_5_1__pyx_pw_12pydivsufsort_9stringalg_47_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_5_1__pyx_pw_12pydivsufsort_9stringalg_49_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_5_1__pyx_mdef_12pydivsufsort_9stringalg_49_kasai = {"__pyx_fuse_5_1_kasai", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_5_1__pyx_pw_12pydivsufsort_9stringalg_49_kasai, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_fuse_5_1__pyx_pw_12pydivsufsort_9stringalg_49_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_s = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_sa = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -9625,26 +9630,26 @@
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(((PyObject *)__pyx_v_s.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "s"); __PYX_ERR(0, 47, __pyx_L1_error)
   }
   if (unlikely(((PyObject *)__pyx_v_sa.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "sa"); __PYX_ERR(0, 47, __pyx_L1_error)
   }
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_46_kasai(__pyx_self, __pyx_v_s, __pyx_v_sa);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_48_kasai(__pyx_self, __pyx_v_s, __pyx_v_sa);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_46_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_48_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa) {
   __pyx_t_5numpy_int64_t __pyx_v_i;
   __pyx_t_5numpy_int64_t __pyx_v_j;
   __pyx_t_5numpy_int64_t __pyx_v_n;
   __pyx_t_5numpy_int64_t __pyx_v_k;
   PyArrayObject *__pyx_v_lcp = 0;
   PyArrayObject *__pyx_v_rank = 0;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_lcp;
@@ -9998,17 +10003,17 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_sa, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_6_0__pyx_pw_12pydivsufsort_9stringalg_49_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_6_0__pyx_mdef_12pydivsufsort_9stringalg_49_kasai = {"__pyx_fuse_6_0_kasai", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_6_0__pyx_pw_12pydivsufsort_9stringalg_49_kasai, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_fuse_6_0__pyx_pw_12pydivsufsort_9stringalg_49_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_6_0__pyx_pw_12pydivsufsort_9stringalg_51_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_6_0__pyx_mdef_12pydivsufsort_9stringalg_51_kasai = {"__pyx_fuse_6_0_kasai", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_6_0__pyx_pw_12pydivsufsort_9stringalg_51_kasai, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_fuse_6_0__pyx_pw_12pydivsufsort_9stringalg_51_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_s = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_sa = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -10061,26 +10066,26 @@
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(((PyObject *)__pyx_v_s.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "s"); __PYX_ERR(0, 47, __pyx_L1_error)
   }
   if (unlikely(((PyObject *)__pyx_v_sa.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "sa"); __PYX_ERR(0, 47, __pyx_L1_error)
   }
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_48_kasai(__pyx_self, __pyx_v_s, __pyx_v_sa);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_50_kasai(__pyx_self, __pyx_v_s, __pyx_v_sa);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_48_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_50_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa) {
   __pyx_t_5numpy_int32_t __pyx_v_i;
   __pyx_t_5numpy_int32_t __pyx_v_j;
   __pyx_t_5numpy_int32_t __pyx_v_n;
   __pyx_t_5numpy_int32_t __pyx_v_k;
   PyArrayObject *__pyx_v_lcp = 0;
   PyArrayObject *__pyx_v_rank = 0;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_lcp;
@@ -10434,17 +10439,17 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_sa, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_6_1__pyx_pw_12pydivsufsort_9stringalg_51_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_6_1__pyx_mdef_12pydivsufsort_9stringalg_51_kasai = {"__pyx_fuse_6_1_kasai", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_6_1__pyx_pw_12pydivsufsort_9stringalg_51_kasai, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_fuse_6_1__pyx_pw_12pydivsufsort_9stringalg_51_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_6_1__pyx_pw_12pydivsufsort_9stringalg_53_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_6_1__pyx_mdef_12pydivsufsort_9stringalg_53_kasai = {"__pyx_fuse_6_1_kasai", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_6_1__pyx_pw_12pydivsufsort_9stringalg_53_kasai, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_fuse_6_1__pyx_pw_12pydivsufsort_9stringalg_53_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_s = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_sa = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -10497,26 +10502,26 @@
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(((PyObject *)__pyx_v_s.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "s"); __PYX_ERR(0, 47, __pyx_L1_error)
   }
   if (unlikely(((PyObject *)__pyx_v_sa.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "sa"); __PYX_ERR(0, 47, __pyx_L1_error)
   }
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_50_kasai(__pyx_self, __pyx_v_s, __pyx_v_sa);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_52_kasai(__pyx_self, __pyx_v_s, __pyx_v_sa);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_50_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_52_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa) {
   __pyx_t_5numpy_int64_t __pyx_v_i;
   __pyx_t_5numpy_int64_t __pyx_v_j;
   __pyx_t_5numpy_int64_t __pyx_v_n;
   __pyx_t_5numpy_int64_t __pyx_v_k;
   PyArrayObject *__pyx_v_lcp = 0;
   PyArrayObject *__pyx_v_rank = 0;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_lcp;
@@ -10870,17 +10875,17 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_sa, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_7_0__pyx_pw_12pydivsufsort_9stringalg_53_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_7_0__pyx_mdef_12pydivsufsort_9stringalg_53_kasai = {"__pyx_fuse_7_0_kasai", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_7_0__pyx_pw_12pydivsufsort_9stringalg_53_kasai, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_fuse_7_0__pyx_pw_12pydivsufsort_9stringalg_53_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_7_0__pyx_pw_12pydivsufsort_9stringalg_55_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_7_0__pyx_mdef_12pydivsufsort_9stringalg_55_kasai = {"__pyx_fuse_7_0_kasai", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_7_0__pyx_pw_12pydivsufsort_9stringalg_55_kasai, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_fuse_7_0__pyx_pw_12pydivsufsort_9stringalg_55_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_s = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_sa = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -10933,26 +10938,26 @@
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(((PyObject *)__pyx_v_s.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "s"); __PYX_ERR(0, 47, __pyx_L1_error)
   }
   if (unlikely(((PyObject *)__pyx_v_sa.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "sa"); __PYX_ERR(0, 47, __pyx_L1_error)
   }
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_52_kasai(__pyx_self, __pyx_v_s, __pyx_v_sa);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_54_kasai(__pyx_self, __pyx_v_s, __pyx_v_sa);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_52_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_54_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa) {
   __pyx_t_5numpy_int32_t __pyx_v_i;
   __pyx_t_5numpy_int32_t __pyx_v_j;
   __pyx_t_5numpy_int32_t __pyx_v_n;
   __pyx_t_5numpy_int32_t __pyx_v_k;
   PyArrayObject *__pyx_v_lcp = 0;
   PyArrayObject *__pyx_v_rank = 0;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_lcp;
@@ -11306,17 +11311,17 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_sa, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_7_1__pyx_pw_12pydivsufsort_9stringalg_55_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_7_1__pyx_mdef_12pydivsufsort_9stringalg_55_kasai = {"__pyx_fuse_7_1_kasai", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_7_1__pyx_pw_12pydivsufsort_9stringalg_55_kasai, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_fuse_7_1__pyx_pw_12pydivsufsort_9stringalg_55_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_7_1__pyx_pw_12pydivsufsort_9stringalg_57_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_7_1__pyx_mdef_12pydivsufsort_9stringalg_57_kasai = {"__pyx_fuse_7_1_kasai", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_7_1__pyx_pw_12pydivsufsort_9stringalg_57_kasai, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_fuse_7_1__pyx_pw_12pydivsufsort_9stringalg_57_kasai(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_s = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_sa = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -11369,26 +11374,26 @@
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(((PyObject *)__pyx_v_s.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "s"); __PYX_ERR(0, 47, __pyx_L1_error)
   }
   if (unlikely(((PyObject *)__pyx_v_sa.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "sa"); __PYX_ERR(0, 47, __pyx_L1_error)
   }
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_54_kasai(__pyx_self, __pyx_v_s, __pyx_v_sa);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_56_kasai(__pyx_self, __pyx_v_s, __pyx_v_sa);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_54_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_56_kasai(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa) {
   __pyx_t_5numpy_int64_t __pyx_v_i;
   __pyx_t_5numpy_int64_t __pyx_v_j;
   __pyx_t_5numpy_int64_t __pyx_v_n;
   __pyx_t_5numpy_int64_t __pyx_v_k;
   PyArrayObject *__pyx_v_lcp = 0;
   PyArrayObject *__pyx_v_rank = 0;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_lcp;
@@ -12297,17 +12302,17 @@
   __Pyx_XDECREF(__pyx_v_kwargs);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_0__pyx_pw_12pydivsufsort_9stringalg_59_kasai_bytes(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_0__pyx_mdef_12pydivsufsort_9stringalg_59_kasai_bytes = {"__pyx_fuse_0_kasai_bytes", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_0__pyx_pw_12pydivsufsort_9stringalg_59_kasai_bytes, METH_VARARGS|METH_KEYWORDS, __pyx_doc_12pydivsufsort_9stringalg_4_kasai_bytes};
-static PyObject *__pyx_fuse_0__pyx_pw_12pydivsufsort_9stringalg_59_kasai_bytes(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_0__pyx_pw_12pydivsufsort_9stringalg_61_kasai_bytes(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_0__pyx_mdef_12pydivsufsort_9stringalg_61_kasai_bytes = {"__pyx_fuse_0_kasai_bytes", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_0__pyx_pw_12pydivsufsort_9stringalg_61_kasai_bytes, METH_VARARGS|METH_KEYWORDS, __pyx_doc_12pydivsufsort_9stringalg_4_kasai_bytes};
+static PyObject *__pyx_fuse_0__pyx_pw_12pydivsufsort_9stringalg_61_kasai_bytes(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_s = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_sa = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -12360,26 +12365,26 @@
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(((PyObject *)__pyx_v_s.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "s"); __PYX_ERR(0, 72, __pyx_L1_error)
   }
   if (unlikely(((PyObject *)__pyx_v_sa.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "sa"); __PYX_ERR(0, 72, __pyx_L1_error)
   }
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_58_kasai_bytes(__pyx_self, __pyx_v_s, __pyx_v_sa);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_60_kasai_bytes(__pyx_self, __pyx_v_s, __pyx_v_sa);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_58_kasai_bytes(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_60_kasai_bytes(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa) {
   __pyx_t_5numpy_int32_t __pyx_v_i;
   __pyx_t_5numpy_int32_t __pyx_v_j;
   __pyx_t_5numpy_int32_t __pyx_v_n;
   __pyx_t_5numpy_int32_t __pyx_v_k;
   PyArrayObject *__pyx_v_lcp = 0;
   PyArrayObject *__pyx_v_rank = 0;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_lcp;
@@ -12733,17 +12738,17 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_sa, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_1__pyx_pw_12pydivsufsort_9stringalg_61_kasai_bytes(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_1__pyx_mdef_12pydivsufsort_9stringalg_61_kasai_bytes = {"__pyx_fuse_1_kasai_bytes", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_1__pyx_pw_12pydivsufsort_9stringalg_61_kasai_bytes, METH_VARARGS|METH_KEYWORDS, __pyx_doc_12pydivsufsort_9stringalg_4_kasai_bytes};
-static PyObject *__pyx_fuse_1__pyx_pw_12pydivsufsort_9stringalg_61_kasai_bytes(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_1__pyx_pw_12pydivsufsort_9stringalg_63_kasai_bytes(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_1__pyx_mdef_12pydivsufsort_9stringalg_63_kasai_bytes = {"__pyx_fuse_1_kasai_bytes", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_1__pyx_pw_12pydivsufsort_9stringalg_63_kasai_bytes, METH_VARARGS|METH_KEYWORDS, __pyx_doc_12pydivsufsort_9stringalg_4_kasai_bytes};
+static PyObject *__pyx_fuse_1__pyx_pw_12pydivsufsort_9stringalg_63_kasai_bytes(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_s = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_sa = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -12796,26 +12801,26 @@
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(((PyObject *)__pyx_v_s.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "s"); __PYX_ERR(0, 72, __pyx_L1_error)
   }
   if (unlikely(((PyObject *)__pyx_v_sa.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "sa"); __PYX_ERR(0, 72, __pyx_L1_error)
   }
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_60_kasai_bytes(__pyx_self, __pyx_v_s, __pyx_v_sa);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_62_kasai_bytes(__pyx_self, __pyx_v_s, __pyx_v_sa);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_60_kasai_bytes(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_62_kasai_bytes(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_s, __Pyx_memviewslice __pyx_v_sa) {
   __pyx_t_5numpy_int64_t __pyx_v_i;
   __pyx_t_5numpy_int64_t __pyx_v_j;
   __pyx_t_5numpy_int64_t __pyx_v_n;
   __pyx_t_5numpy_int64_t __pyx_v_k;
   PyArrayObject *__pyx_v_lcp = 0;
   PyArrayObject *__pyx_v_rank = 0;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_lcp;
@@ -14576,17 +14581,17 @@
   __Pyx_XDECREF(__pyx_v_kwargs);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_0_0__pyx_pw_12pydivsufsort_9stringalg_65_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_0_0__pyx_mdef_12pydivsufsort_9stringalg_65_lcp_segtree = {"__pyx_fuse_0_0_lcp_segtree", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_0_0__pyx_pw_12pydivsufsort_9stringalg_65_lcp_segtree, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_fuse_0_0__pyx_pw_12pydivsufsort_9stringalg_65_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_0_0__pyx_pw_12pydivsufsort_9stringalg_67_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_0_0__pyx_mdef_12pydivsufsort_9stringalg_67_lcp_segtree = {"__pyx_fuse_0_0_lcp_segtree", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_0_0__pyx_pw_12pydivsufsort_9stringalg_67_lcp_segtree, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_fuse_0_0__pyx_pw_12pydivsufsort_9stringalg_67_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s = { 0, 0, { 0 }, { 0 }, { 0 } };
   PyArrayObject *__pyx_v_sa = 0;
   PyArrayObject *__pyx_v_lcp = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -14649,26 +14654,26 @@
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(((PyObject *)__pyx_v_s.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "s"); __PYX_ERR(0, 112, __pyx_L1_error)
   }
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_sa), __pyx_ptype_5numpy_ndarray, 0, "sa", 0))) __PYX_ERR(0, 113, __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_lcp), __pyx_ptype_5numpy_ndarray, 0, "lcp", 0))) __PYX_ERR(0, 114, __pyx_L1_error)
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_64_lcp_segtree(__pyx_self, __pyx_v_s, __pyx_v_sa, __pyx_v_lcp);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_66_lcp_segtree(__pyx_self, __pyx_v_s, __pyx_v_sa, __pyx_v_lcp);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_64_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_66_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp) {
   __pyx_t_5numpy_int32_t __pyx_v_i;
   __pyx_t_5numpy_int32_t __pyx_v_n;
   PyArrayObject *__pyx_v_segtree = 0;
   PyArrayObject *__pyx_v_rank = 0;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_lcp;
   __Pyx_Buffer __pyx_pybuffer_lcp;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_sa;
@@ -14940,17 +14945,17 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_s, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_0_1__pyx_pw_12pydivsufsort_9stringalg_67_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_0_1__pyx_mdef_12pydivsufsort_9stringalg_67_lcp_segtree = {"__pyx_fuse_0_1_lcp_segtree", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_0_1__pyx_pw_12pydivsufsort_9stringalg_67_lcp_segtree, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_fuse_0_1__pyx_pw_12pydivsufsort_9stringalg_67_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_0_1__pyx_pw_12pydivsufsort_9stringalg_69_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_0_1__pyx_mdef_12pydivsufsort_9stringalg_69_lcp_segtree = {"__pyx_fuse_0_1_lcp_segtree", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_0_1__pyx_pw_12pydivsufsort_9stringalg_69_lcp_segtree, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_fuse_0_1__pyx_pw_12pydivsufsort_9stringalg_69_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s = { 0, 0, { 0 }, { 0 }, { 0 } };
   PyArrayObject *__pyx_v_sa = 0;
   PyArrayObject *__pyx_v_lcp = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -15013,26 +15018,26 @@
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(((PyObject *)__pyx_v_s.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "s"); __PYX_ERR(0, 112, __pyx_L1_error)
   }
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_sa), __pyx_ptype_5numpy_ndarray, 0, "sa", 0))) __PYX_ERR(0, 113, __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_lcp), __pyx_ptype_5numpy_ndarray, 0, "lcp", 0))) __PYX_ERR(0, 114, __pyx_L1_error)
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_66_lcp_segtree(__pyx_self, __pyx_v_s, __pyx_v_sa, __pyx_v_lcp);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_68_lcp_segtree(__pyx_self, __pyx_v_s, __pyx_v_sa, __pyx_v_lcp);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_66_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_68_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp) {
   __pyx_t_5numpy_int64_t __pyx_v_i;
   __pyx_t_5numpy_int64_t __pyx_v_n;
   PyArrayObject *__pyx_v_segtree = 0;
   PyArrayObject *__pyx_v_rank = 0;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_lcp;
   __Pyx_Buffer __pyx_pybuffer_lcp;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_sa;
@@ -15304,17 +15309,17 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_s, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_1_0__pyx_pw_12pydivsufsort_9stringalg_69_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_1_0__pyx_mdef_12pydivsufsort_9stringalg_69_lcp_segtree = {"__pyx_fuse_1_0_lcp_segtree", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_1_0__pyx_pw_12pydivsufsort_9stringalg_69_lcp_segtree, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_fuse_1_0__pyx_pw_12pydivsufsort_9stringalg_69_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_1_0__pyx_pw_12pydivsufsort_9stringalg_71_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_1_0__pyx_mdef_12pydivsufsort_9stringalg_71_lcp_segtree = {"__pyx_fuse_1_0_lcp_segtree", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_1_0__pyx_pw_12pydivsufsort_9stringalg_71_lcp_segtree, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_fuse_1_0__pyx_pw_12pydivsufsort_9stringalg_71_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s = { 0, 0, { 0 }, { 0 }, { 0 } };
   PyArrayObject *__pyx_v_sa = 0;
   PyArrayObject *__pyx_v_lcp = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -15377,26 +15382,26 @@
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(((PyObject *)__pyx_v_s.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "s"); __PYX_ERR(0, 112, __pyx_L1_error)
   }
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_sa), __pyx_ptype_5numpy_ndarray, 0, "sa", 0))) __PYX_ERR(0, 113, __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_lcp), __pyx_ptype_5numpy_ndarray, 0, "lcp", 0))) __PYX_ERR(0, 114, __pyx_L1_error)
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_68_lcp_segtree(__pyx_self, __pyx_v_s, __pyx_v_sa, __pyx_v_lcp);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_70_lcp_segtree(__pyx_self, __pyx_v_s, __pyx_v_sa, __pyx_v_lcp);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_68_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_70_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp) {
   __pyx_t_5numpy_int32_t __pyx_v_i;
   __pyx_t_5numpy_int32_t __pyx_v_n;
   PyArrayObject *__pyx_v_segtree = 0;
   PyArrayObject *__pyx_v_rank = 0;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_lcp;
   __Pyx_Buffer __pyx_pybuffer_lcp;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_sa;
@@ -15668,17 +15673,17 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_s, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_1_1__pyx_pw_12pydivsufsort_9stringalg_71_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_1_1__pyx_mdef_12pydivsufsort_9stringalg_71_lcp_segtree = {"__pyx_fuse_1_1_lcp_segtree", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_1_1__pyx_pw_12pydivsufsort_9stringalg_71_lcp_segtree, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_fuse_1_1__pyx_pw_12pydivsufsort_9stringalg_71_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_1_1__pyx_pw_12pydivsufsort_9stringalg_73_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_1_1__pyx_mdef_12pydivsufsort_9stringalg_73_lcp_segtree = {"__pyx_fuse_1_1_lcp_segtree", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_1_1__pyx_pw_12pydivsufsort_9stringalg_73_lcp_segtree, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_fuse_1_1__pyx_pw_12pydivsufsort_9stringalg_73_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s = { 0, 0, { 0 }, { 0 }, { 0 } };
   PyArrayObject *__pyx_v_sa = 0;
   PyArrayObject *__pyx_v_lcp = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -15741,26 +15746,26 @@
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(((PyObject *)__pyx_v_s.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "s"); __PYX_ERR(0, 112, __pyx_L1_error)
   }
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_sa), __pyx_ptype_5numpy_ndarray, 0, "sa", 0))) __PYX_ERR(0, 113, __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_lcp), __pyx_ptype_5numpy_ndarray, 0, "lcp", 0))) __PYX_ERR(0, 114, __pyx_L1_error)
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_70_lcp_segtree(__pyx_self, __pyx_v_s, __pyx_v_sa, __pyx_v_lcp);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_72_lcp_segtree(__pyx_self, __pyx_v_s, __pyx_v_sa, __pyx_v_lcp);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_70_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_72_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp) {
   __pyx_t_5numpy_int64_t __pyx_v_i;
   __pyx_t_5numpy_int64_t __pyx_v_n;
   PyArrayObject *__pyx_v_segtree = 0;
   PyArrayObject *__pyx_v_rank = 0;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_lcp;
   __Pyx_Buffer __pyx_pybuffer_lcp;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_sa;
@@ -16032,17 +16037,17 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_s, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_2_0__pyx_pw_12pydivsufsort_9stringalg_73_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_2_0__pyx_mdef_12pydivsufsort_9stringalg_73_lcp_segtree = {"__pyx_fuse_2_0_lcp_segtree", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_2_0__pyx_pw_12pydivsufsort_9stringalg_73_lcp_segtree, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_fuse_2_0__pyx_pw_12pydivsufsort_9stringalg_73_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_2_0__pyx_pw_12pydivsufsort_9stringalg_75_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_2_0__pyx_mdef_12pydivsufsort_9stringalg_75_lcp_segtree = {"__pyx_fuse_2_0_lcp_segtree", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_2_0__pyx_pw_12pydivsufsort_9stringalg_75_lcp_segtree, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_fuse_2_0__pyx_pw_12pydivsufsort_9stringalg_75_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s = { 0, 0, { 0 }, { 0 }, { 0 } };
   PyArrayObject *__pyx_v_sa = 0;
   PyArrayObject *__pyx_v_lcp = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -16105,26 +16110,26 @@
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(((PyObject *)__pyx_v_s.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "s"); __PYX_ERR(0, 112, __pyx_L1_error)
   }
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_sa), __pyx_ptype_5numpy_ndarray, 0, "sa", 0))) __PYX_ERR(0, 113, __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_lcp), __pyx_ptype_5numpy_ndarray, 0, "lcp", 0))) __PYX_ERR(0, 114, __pyx_L1_error)
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_72_lcp_segtree(__pyx_self, __pyx_v_s, __pyx_v_sa, __pyx_v_lcp);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_74_lcp_segtree(__pyx_self, __pyx_v_s, __pyx_v_sa, __pyx_v_lcp);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_72_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_74_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp) {
   __pyx_t_5numpy_int32_t __pyx_v_i;
   __pyx_t_5numpy_int32_t __pyx_v_n;
   PyArrayObject *__pyx_v_segtree = 0;
   PyArrayObject *__pyx_v_rank = 0;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_lcp;
   __Pyx_Buffer __pyx_pybuffer_lcp;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_sa;
@@ -16396,17 +16401,17 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_s, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_2_1__pyx_pw_12pydivsufsort_9stringalg_75_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_2_1__pyx_mdef_12pydivsufsort_9stringalg_75_lcp_segtree = {"__pyx_fuse_2_1_lcp_segtree", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_2_1__pyx_pw_12pydivsufsort_9stringalg_75_lcp_segtree, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_fuse_2_1__pyx_pw_12pydivsufsort_9stringalg_75_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_2_1__pyx_pw_12pydivsufsort_9stringalg_77_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_2_1__pyx_mdef_12pydivsufsort_9stringalg_77_lcp_segtree = {"__pyx_fuse_2_1_lcp_segtree", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_2_1__pyx_pw_12pydivsufsort_9stringalg_77_lcp_segtree, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_fuse_2_1__pyx_pw_12pydivsufsort_9stringalg_77_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s = { 0, 0, { 0 }, { 0 }, { 0 } };
   PyArrayObject *__pyx_v_sa = 0;
   PyArrayObject *__pyx_v_lcp = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -16469,26 +16474,26 @@
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(((PyObject *)__pyx_v_s.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "s"); __PYX_ERR(0, 112, __pyx_L1_error)
   }
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_sa), __pyx_ptype_5numpy_ndarray, 0, "sa", 0))) __PYX_ERR(0, 113, __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_lcp), __pyx_ptype_5numpy_ndarray, 0, "lcp", 0))) __PYX_ERR(0, 114, __pyx_L1_error)
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_74_lcp_segtree(__pyx_self, __pyx_v_s, __pyx_v_sa, __pyx_v_lcp);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_76_lcp_segtree(__pyx_self, __pyx_v_s, __pyx_v_sa, __pyx_v_lcp);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_74_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_76_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp) {
   __pyx_t_5numpy_int64_t __pyx_v_i;
   __pyx_t_5numpy_int64_t __pyx_v_n;
   PyArrayObject *__pyx_v_segtree = 0;
   PyArrayObject *__pyx_v_rank = 0;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_lcp;
   __Pyx_Buffer __pyx_pybuffer_lcp;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_sa;
@@ -16760,17 +16765,17 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_s, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_3_0__pyx_pw_12pydivsufsort_9stringalg_77_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_3_0__pyx_mdef_12pydivsufsort_9stringalg_77_lcp_segtree = {"__pyx_fuse_3_0_lcp_segtree", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_3_0__pyx_pw_12pydivsufsort_9stringalg_77_lcp_segtree, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_fuse_3_0__pyx_pw_12pydivsufsort_9stringalg_77_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_3_0__pyx_pw_12pydivsufsort_9stringalg_79_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_3_0__pyx_mdef_12pydivsufsort_9stringalg_79_lcp_segtree = {"__pyx_fuse_3_0_lcp_segtree", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_3_0__pyx_pw_12pydivsufsort_9stringalg_79_lcp_segtree, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_fuse_3_0__pyx_pw_12pydivsufsort_9stringalg_79_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s = { 0, 0, { 0 }, { 0 }, { 0 } };
   PyArrayObject *__pyx_v_sa = 0;
   PyArrayObject *__pyx_v_lcp = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -16833,26 +16838,26 @@
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(((PyObject *)__pyx_v_s.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "s"); __PYX_ERR(0, 112, __pyx_L1_error)
   }
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_sa), __pyx_ptype_5numpy_ndarray, 0, "sa", 0))) __PYX_ERR(0, 113, __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_lcp), __pyx_ptype_5numpy_ndarray, 0, "lcp", 0))) __PYX_ERR(0, 114, __pyx_L1_error)
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_76_lcp_segtree(__pyx_self, __pyx_v_s, __pyx_v_sa, __pyx_v_lcp);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_78_lcp_segtree(__pyx_self, __pyx_v_s, __pyx_v_sa, __pyx_v_lcp);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_76_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_78_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp) {
   __pyx_t_5numpy_int32_t __pyx_v_i;
   __pyx_t_5numpy_int32_t __pyx_v_n;
   PyArrayObject *__pyx_v_segtree = 0;
   PyArrayObject *__pyx_v_rank = 0;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_lcp;
   __Pyx_Buffer __pyx_pybuffer_lcp;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_sa;
@@ -17124,17 +17129,17 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_s, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_3_1__pyx_pw_12pydivsufsort_9stringalg_79_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_3_1__pyx_mdef_12pydivsufsort_9stringalg_79_lcp_segtree = {"__pyx_fuse_3_1_lcp_segtree", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_3_1__pyx_pw_12pydivsufsort_9stringalg_79_lcp_segtree, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_fuse_3_1__pyx_pw_12pydivsufsort_9stringalg_79_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_3_1__pyx_pw_12pydivsufsort_9stringalg_81_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_3_1__pyx_mdef_12pydivsufsort_9stringalg_81_lcp_segtree = {"__pyx_fuse_3_1_lcp_segtree", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_3_1__pyx_pw_12pydivsufsort_9stringalg_81_lcp_segtree, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_fuse_3_1__pyx_pw_12pydivsufsort_9stringalg_81_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s = { 0, 0, { 0 }, { 0 }, { 0 } };
   PyArrayObject *__pyx_v_sa = 0;
   PyArrayObject *__pyx_v_lcp = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -17197,26 +17202,26 @@
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(((PyObject *)__pyx_v_s.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "s"); __PYX_ERR(0, 112, __pyx_L1_error)
   }
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_sa), __pyx_ptype_5numpy_ndarray, 0, "sa", 0))) __PYX_ERR(0, 113, __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_lcp), __pyx_ptype_5numpy_ndarray, 0, "lcp", 0))) __PYX_ERR(0, 114, __pyx_L1_error)
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_78_lcp_segtree(__pyx_self, __pyx_v_s, __pyx_v_sa, __pyx_v_lcp);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_80_lcp_segtree(__pyx_self, __pyx_v_s, __pyx_v_sa, __pyx_v_lcp);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_78_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_80_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp) {
   __pyx_t_5numpy_int64_t __pyx_v_i;
   __pyx_t_5numpy_int64_t __pyx_v_n;
   PyArrayObject *__pyx_v_segtree = 0;
   PyArrayObject *__pyx_v_rank = 0;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_lcp;
   __Pyx_Buffer __pyx_pybuffer_lcp;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_sa;
@@ -17488,17 +17493,17 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_s, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_4_0__pyx_pw_12pydivsufsort_9stringalg_81_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_4_0__pyx_mdef_12pydivsufsort_9stringalg_81_lcp_segtree = {"__pyx_fuse_4_0_lcp_segtree", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_4_0__pyx_pw_12pydivsufsort_9stringalg_81_lcp_segtree, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_fuse_4_0__pyx_pw_12pydivsufsort_9stringalg_81_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_4_0__pyx_pw_12pydivsufsort_9stringalg_83_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_4_0__pyx_mdef_12pydivsufsort_9stringalg_83_lcp_segtree = {"__pyx_fuse_4_0_lcp_segtree", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_4_0__pyx_pw_12pydivsufsort_9stringalg_83_lcp_segtree, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_fuse_4_0__pyx_pw_12pydivsufsort_9stringalg_83_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s = { 0, 0, { 0 }, { 0 }, { 0 } };
   PyArrayObject *__pyx_v_sa = 0;
   PyArrayObject *__pyx_v_lcp = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -17561,26 +17566,26 @@
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(((PyObject *)__pyx_v_s.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "s"); __PYX_ERR(0, 112, __pyx_L1_error)
   }
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_sa), __pyx_ptype_5numpy_ndarray, 0, "sa", 0))) __PYX_ERR(0, 113, __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_lcp), __pyx_ptype_5numpy_ndarray, 0, "lcp", 0))) __PYX_ERR(0, 114, __pyx_L1_error)
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_80_lcp_segtree(__pyx_self, __pyx_v_s, __pyx_v_sa, __pyx_v_lcp);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_82_lcp_segtree(__pyx_self, __pyx_v_s, __pyx_v_sa, __pyx_v_lcp);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_80_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_82_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp) {
   __pyx_t_5numpy_int32_t __pyx_v_i;
   __pyx_t_5numpy_int32_t __pyx_v_n;
   PyArrayObject *__pyx_v_segtree = 0;
   PyArrayObject *__pyx_v_rank = 0;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_lcp;
   __Pyx_Buffer __pyx_pybuffer_lcp;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_sa;
@@ -17852,17 +17857,17 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_s, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_4_1__pyx_pw_12pydivsufsort_9stringalg_83_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_4_1__pyx_mdef_12pydivsufsort_9stringalg_83_lcp_segtree = {"__pyx_fuse_4_1_lcp_segtree", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_4_1__pyx_pw_12pydivsufsort_9stringalg_83_lcp_segtree, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_fuse_4_1__pyx_pw_12pydivsufsort_9stringalg_83_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_4_1__pyx_pw_12pydivsufsort_9stringalg_85_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_4_1__pyx_mdef_12pydivsufsort_9stringalg_85_lcp_segtree = {"__pyx_fuse_4_1_lcp_segtree", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_4_1__pyx_pw_12pydivsufsort_9stringalg_85_lcp_segtree, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_fuse_4_1__pyx_pw_12pydivsufsort_9stringalg_85_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s = { 0, 0, { 0 }, { 0 }, { 0 } };
   PyArrayObject *__pyx_v_sa = 0;
   PyArrayObject *__pyx_v_lcp = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -17925,26 +17930,26 @@
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(((PyObject *)__pyx_v_s.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "s"); __PYX_ERR(0, 112, __pyx_L1_error)
   }
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_sa), __pyx_ptype_5numpy_ndarray, 0, "sa", 0))) __PYX_ERR(0, 113, __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_lcp), __pyx_ptype_5numpy_ndarray, 0, "lcp", 0))) __PYX_ERR(0, 114, __pyx_L1_error)
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_82_lcp_segtree(__pyx_self, __pyx_v_s, __pyx_v_sa, __pyx_v_lcp);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_84_lcp_segtree(__pyx_self, __pyx_v_s, __pyx_v_sa, __pyx_v_lcp);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_82_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_84_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp) {
   __pyx_t_5numpy_int64_t __pyx_v_i;
   __pyx_t_5numpy_int64_t __pyx_v_n;
   PyArrayObject *__pyx_v_segtree = 0;
   PyArrayObject *__pyx_v_rank = 0;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_lcp;
   __Pyx_Buffer __pyx_pybuffer_lcp;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_sa;
@@ -18216,17 +18221,17 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_s, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_5_0__pyx_pw_12pydivsufsort_9stringalg_85_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_5_0__pyx_mdef_12pydivsufsort_9stringalg_85_lcp_segtree = {"__pyx_fuse_5_0_lcp_segtree", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_5_0__pyx_pw_12pydivsufsort_9stringalg_85_lcp_segtree, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_fuse_5_0__pyx_pw_12pydivsufsort_9stringalg_85_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_5_0__pyx_pw_12pydivsufsort_9stringalg_87_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_5_0__pyx_mdef_12pydivsufsort_9stringalg_87_lcp_segtree = {"__pyx_fuse_5_0_lcp_segtree", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_5_0__pyx_pw_12pydivsufsort_9stringalg_87_lcp_segtree, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_fuse_5_0__pyx_pw_12pydivsufsort_9stringalg_87_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s = { 0, 0, { 0 }, { 0 }, { 0 } };
   PyArrayObject *__pyx_v_sa = 0;
   PyArrayObject *__pyx_v_lcp = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -18289,26 +18294,26 @@
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(((PyObject *)__pyx_v_s.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "s"); __PYX_ERR(0, 112, __pyx_L1_error)
   }
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_sa), __pyx_ptype_5numpy_ndarray, 0, "sa", 0))) __PYX_ERR(0, 113, __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_lcp), __pyx_ptype_5numpy_ndarray, 0, "lcp", 0))) __PYX_ERR(0, 114, __pyx_L1_error)
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_84_lcp_segtree(__pyx_self, __pyx_v_s, __pyx_v_sa, __pyx_v_lcp);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_86_lcp_segtree(__pyx_self, __pyx_v_s, __pyx_v_sa, __pyx_v_lcp);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_84_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_86_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp) {
   __pyx_t_5numpy_int32_t __pyx_v_i;
   __pyx_t_5numpy_int32_t __pyx_v_n;
   PyArrayObject *__pyx_v_segtree = 0;
   PyArrayObject *__pyx_v_rank = 0;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_lcp;
   __Pyx_Buffer __pyx_pybuffer_lcp;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_sa;
@@ -18580,17 +18585,17 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_s, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_5_1__pyx_pw_12pydivsufsort_9stringalg_87_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_5_1__pyx_mdef_12pydivsufsort_9stringalg_87_lcp_segtree = {"__pyx_fuse_5_1_lcp_segtree", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_5_1__pyx_pw_12pydivsufsort_9stringalg_87_lcp_segtree, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_fuse_5_1__pyx_pw_12pydivsufsort_9stringalg_87_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_5_1__pyx_pw_12pydivsufsort_9stringalg_89_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_5_1__pyx_mdef_12pydivsufsort_9stringalg_89_lcp_segtree = {"__pyx_fuse_5_1_lcp_segtree", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_5_1__pyx_pw_12pydivsufsort_9stringalg_89_lcp_segtree, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_fuse_5_1__pyx_pw_12pydivsufsort_9stringalg_89_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s = { 0, 0, { 0 }, { 0 }, { 0 } };
   PyArrayObject *__pyx_v_sa = 0;
   PyArrayObject *__pyx_v_lcp = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -18653,26 +18658,26 @@
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(((PyObject *)__pyx_v_s.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "s"); __PYX_ERR(0, 112, __pyx_L1_error)
   }
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_sa), __pyx_ptype_5numpy_ndarray, 0, "sa", 0))) __PYX_ERR(0, 113, __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_lcp), __pyx_ptype_5numpy_ndarray, 0, "lcp", 0))) __PYX_ERR(0, 114, __pyx_L1_error)
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_86_lcp_segtree(__pyx_self, __pyx_v_s, __pyx_v_sa, __pyx_v_lcp);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_88_lcp_segtree(__pyx_self, __pyx_v_s, __pyx_v_sa, __pyx_v_lcp);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_86_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_88_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp) {
   __pyx_t_5numpy_int64_t __pyx_v_i;
   __pyx_t_5numpy_int64_t __pyx_v_n;
   PyArrayObject *__pyx_v_segtree = 0;
   PyArrayObject *__pyx_v_rank = 0;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_lcp;
   __Pyx_Buffer __pyx_pybuffer_lcp;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_sa;
@@ -18944,17 +18949,17 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_s, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_6_0__pyx_pw_12pydivsufsort_9stringalg_89_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_6_0__pyx_mdef_12pydivsufsort_9stringalg_89_lcp_segtree = {"__pyx_fuse_6_0_lcp_segtree", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_6_0__pyx_pw_12pydivsufsort_9stringalg_89_lcp_segtree, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_fuse_6_0__pyx_pw_12pydivsufsort_9stringalg_89_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_6_0__pyx_pw_12pydivsufsort_9stringalg_91_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_6_0__pyx_mdef_12pydivsufsort_9stringalg_91_lcp_segtree = {"__pyx_fuse_6_0_lcp_segtree", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_6_0__pyx_pw_12pydivsufsort_9stringalg_91_lcp_segtree, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_fuse_6_0__pyx_pw_12pydivsufsort_9stringalg_91_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s = { 0, 0, { 0 }, { 0 }, { 0 } };
   PyArrayObject *__pyx_v_sa = 0;
   PyArrayObject *__pyx_v_lcp = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -19017,26 +19022,26 @@
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(((PyObject *)__pyx_v_s.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "s"); __PYX_ERR(0, 112, __pyx_L1_error)
   }
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_sa), __pyx_ptype_5numpy_ndarray, 0, "sa", 0))) __PYX_ERR(0, 113, __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_lcp), __pyx_ptype_5numpy_ndarray, 0, "lcp", 0))) __PYX_ERR(0, 114, __pyx_L1_error)
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_88_lcp_segtree(__pyx_self, __pyx_v_s, __pyx_v_sa, __pyx_v_lcp);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_90_lcp_segtree(__pyx_self, __pyx_v_s, __pyx_v_sa, __pyx_v_lcp);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_88_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_90_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp) {
   __pyx_t_5numpy_int32_t __pyx_v_i;
   __pyx_t_5numpy_int32_t __pyx_v_n;
   PyArrayObject *__pyx_v_segtree = 0;
   PyArrayObject *__pyx_v_rank = 0;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_lcp;
   __Pyx_Buffer __pyx_pybuffer_lcp;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_sa;
@@ -19308,17 +19313,17 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_s, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_6_1__pyx_pw_12pydivsufsort_9stringalg_91_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_6_1__pyx_mdef_12pydivsufsort_9stringalg_91_lcp_segtree = {"__pyx_fuse_6_1_lcp_segtree", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_6_1__pyx_pw_12pydivsufsort_9stringalg_91_lcp_segtree, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_fuse_6_1__pyx_pw_12pydivsufsort_9stringalg_91_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_6_1__pyx_pw_12pydivsufsort_9stringalg_93_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_6_1__pyx_mdef_12pydivsufsort_9stringalg_93_lcp_segtree = {"__pyx_fuse_6_1_lcp_segtree", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_6_1__pyx_pw_12pydivsufsort_9stringalg_93_lcp_segtree, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_fuse_6_1__pyx_pw_12pydivsufsort_9stringalg_93_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s = { 0, 0, { 0 }, { 0 }, { 0 } };
   PyArrayObject *__pyx_v_sa = 0;
   PyArrayObject *__pyx_v_lcp = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -19381,26 +19386,26 @@
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(((PyObject *)__pyx_v_s.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "s"); __PYX_ERR(0, 112, __pyx_L1_error)
   }
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_sa), __pyx_ptype_5numpy_ndarray, 0, "sa", 0))) __PYX_ERR(0, 113, __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_lcp), __pyx_ptype_5numpy_ndarray, 0, "lcp", 0))) __PYX_ERR(0, 114, __pyx_L1_error)
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_90_lcp_segtree(__pyx_self, __pyx_v_s, __pyx_v_sa, __pyx_v_lcp);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_92_lcp_segtree(__pyx_self, __pyx_v_s, __pyx_v_sa, __pyx_v_lcp);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_90_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_92_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp) {
   __pyx_t_5numpy_int64_t __pyx_v_i;
   __pyx_t_5numpy_int64_t __pyx_v_n;
   PyArrayObject *__pyx_v_segtree = 0;
   PyArrayObject *__pyx_v_rank = 0;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_lcp;
   __Pyx_Buffer __pyx_pybuffer_lcp;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_sa;
@@ -19672,17 +19677,17 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_s, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_7_0__pyx_pw_12pydivsufsort_9stringalg_93_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_7_0__pyx_mdef_12pydivsufsort_9stringalg_93_lcp_segtree = {"__pyx_fuse_7_0_lcp_segtree", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_7_0__pyx_pw_12pydivsufsort_9stringalg_93_lcp_segtree, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_fuse_7_0__pyx_pw_12pydivsufsort_9stringalg_93_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_7_0__pyx_pw_12pydivsufsort_9stringalg_95_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_7_0__pyx_mdef_12pydivsufsort_9stringalg_95_lcp_segtree = {"__pyx_fuse_7_0_lcp_segtree", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_7_0__pyx_pw_12pydivsufsort_9stringalg_95_lcp_segtree, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_fuse_7_0__pyx_pw_12pydivsufsort_9stringalg_95_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s = { 0, 0, { 0 }, { 0 }, { 0 } };
   PyArrayObject *__pyx_v_sa = 0;
   PyArrayObject *__pyx_v_lcp = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -19745,26 +19750,26 @@
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(((PyObject *)__pyx_v_s.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "s"); __PYX_ERR(0, 112, __pyx_L1_error)
   }
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_sa), __pyx_ptype_5numpy_ndarray, 0, "sa", 0))) __PYX_ERR(0, 113, __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_lcp), __pyx_ptype_5numpy_ndarray, 0, "lcp", 0))) __PYX_ERR(0, 114, __pyx_L1_error)
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_92_lcp_segtree(__pyx_self, __pyx_v_s, __pyx_v_sa, __pyx_v_lcp);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_94_lcp_segtree(__pyx_self, __pyx_v_s, __pyx_v_sa, __pyx_v_lcp);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_92_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_94_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp) {
   __pyx_t_5numpy_int32_t __pyx_v_i;
   __pyx_t_5numpy_int32_t __pyx_v_n;
   PyArrayObject *__pyx_v_segtree = 0;
   PyArrayObject *__pyx_v_rank = 0;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_lcp;
   __Pyx_Buffer __pyx_pybuffer_lcp;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_sa;
@@ -20036,17 +20041,17 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_s, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_7_1__pyx_pw_12pydivsufsort_9stringalg_95_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_7_1__pyx_mdef_12pydivsufsort_9stringalg_95_lcp_segtree = {"__pyx_fuse_7_1_lcp_segtree", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_7_1__pyx_pw_12pydivsufsort_9stringalg_95_lcp_segtree, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_fuse_7_1__pyx_pw_12pydivsufsort_9stringalg_95_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_7_1__pyx_pw_12pydivsufsort_9stringalg_97_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_7_1__pyx_mdef_12pydivsufsort_9stringalg_97_lcp_segtree = {"__pyx_fuse_7_1_lcp_segtree", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_7_1__pyx_pw_12pydivsufsort_9stringalg_97_lcp_segtree, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_fuse_7_1__pyx_pw_12pydivsufsort_9stringalg_97_lcp_segtree(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s = { 0, 0, { 0 }, { 0 }, { 0 } };
   PyArrayObject *__pyx_v_sa = 0;
   PyArrayObject *__pyx_v_lcp = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -20109,26 +20114,26 @@
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(((PyObject *)__pyx_v_s.memview) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "s"); __PYX_ERR(0, 112, __pyx_L1_error)
   }
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_sa), __pyx_ptype_5numpy_ndarray, 0, "sa", 0))) __PYX_ERR(0, 113, __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_lcp), __pyx_ptype_5numpy_ndarray, 0, "lcp", 0))) __PYX_ERR(0, 114, __pyx_L1_error)
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_94_lcp_segtree(__pyx_self, __pyx_v_s, __pyx_v_sa, __pyx_v_lcp);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_96_lcp_segtree(__pyx_self, __pyx_v_s, __pyx_v_sa, __pyx_v_lcp);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_94_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_96_lcp_segtree(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED __Pyx_memviewslice __pyx_v_s, PyArrayObject *__pyx_v_sa, PyArrayObject *__pyx_v_lcp) {
   __pyx_t_5numpy_int64_t __pyx_v_i;
   __pyx_t_5numpy_int64_t __pyx_v_n;
   PyArrayObject *__pyx_v_segtree = 0;
   PyArrayObject *__pyx_v_rank = 0;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_lcp;
   __Pyx_Buffer __pyx_pybuffer_lcp;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_sa;
@@ -20780,23 +20785,23 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "pydivsufsort/stringalg.pyx":144
  * 
  * 
- * def lcp_query(             # <<<<<<<<<<<<<<
+ * def _lcp_query(             # <<<<<<<<<<<<<<
  *         np.ndarray[sa_t, ndim=1] rank not None,
  *         np.ndarray[sa_t, ndim=1] segtree not None,
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_12pydivsufsort_9stringalg_13lcp_query(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_mdef_12pydivsufsort_9stringalg_13lcp_query = {"lcp_query", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_12pydivsufsort_9stringalg_13lcp_query, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_12pydivsufsort_9stringalg_13lcp_query(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_12pydivsufsort_9stringalg_13_lcp_query(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_12pydivsufsort_9stringalg_13_lcp_query = {"_lcp_query", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_12pydivsufsort_9stringalg_13_lcp_query, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_12pydivsufsort_9stringalg_13_lcp_query(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_signatures = 0;
   PyObject *__pyx_v_args = 0;
   PyObject *__pyx_v_kwargs = 0;
   CYTHON_UNUSED PyObject *__pyx_v_defaults = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -20865,22 +20870,22 @@
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__pyx_fused_cpdef", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 144, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pydivsufsort.stringalg.__pyx_fused_cpdef", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_12lcp_query(__pyx_self, __pyx_v_signatures, __pyx_v_args, __pyx_v_kwargs, __pyx_v_defaults);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_12_lcp_query(__pyx_self, __pyx_v_signatures, __pyx_v_args, __pyx_v_kwargs, __pyx_v_defaults);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_12lcp_query(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_signatures, PyObject *__pyx_v_args, PyObject *__pyx_v_kwargs, CYTHON_UNUSED PyObject *__pyx_v_defaults) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_12_lcp_query(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_signatures, PyObject *__pyx_v_args, PyObject *__pyx_v_kwargs, CYTHON_UNUSED PyObject *__pyx_v_defaults) {
   PyObject *__pyx_v_dest_sig = NULL;
   Py_ssize_t __pyx_v_i;
   PyTypeObject *__pyx_v_ndarray = 0;
   __Pyx_memviewslice __pyx_v_memslice;
   Py_ssize_t __pyx_v_itemsize;
   int __pyx_v_dtype_signed;
   char __pyx_v_kind;
@@ -20913,15 +20918,15 @@
   Py_ssize_t __pyx_t_15;
   Py_ssize_t __pyx_t_16;
   Py_ssize_t __pyx_t_17;
   int __pyx_t_18;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("lcp_query", 0);
+  __Pyx_RefNannySetupContext("_lcp_query", 0);
   __Pyx_INCREF(__pyx_v_kwargs);
   __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 144, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   PyList_SET_ITEM(__pyx_t_1, 0, Py_None);
   __pyx_v_dest_sig = ((PyObject*)__pyx_t_1);
@@ -21332,26 +21337,26 @@
   __Pyx_XDECREF(__pyx_v_kwargs);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_0__pyx_pw_12pydivsufsort_9stringalg_99lcp_query(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_0__pyx_mdef_12pydivsufsort_9stringalg_99lcp_query = {"__pyx_fuse_0lcp_query", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_0__pyx_pw_12pydivsufsort_9stringalg_99lcp_query, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_fuse_0__pyx_pw_12pydivsufsort_9stringalg_99lcp_query(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_0__pyx_pw_12pydivsufsort_9stringalg_101_lcp_query(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_0__pyx_mdef_12pydivsufsort_9stringalg_101_lcp_query = {"__pyx_fuse_0_lcp_query", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_0__pyx_pw_12pydivsufsort_9stringalg_101_lcp_query, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_fuse_0__pyx_pw_12pydivsufsort_9stringalg_101_lcp_query(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyArrayObject *__pyx_v_rank = 0;
   PyArrayObject *__pyx_v_segtree = 0;
   PyObject *__pyx_v_queries = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("lcp_query (wrapper)", 0);
+  __Pyx_RefNannySetupContext("_lcp_query (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_rank,&__pyx_n_s_segtree,&__pyx_n_s_queries,0};
     PyObject* values[3] = {0,0,0};
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
@@ -21369,59 +21374,59 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_rank)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_segtree)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("lcp_query", 1, 3, 3, 1); __PYX_ERR(0, 144, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_lcp_query", 1, 3, 3, 1); __PYX_ERR(0, 144, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_queries)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("lcp_query", 1, 3, 3, 2); __PYX_ERR(0, 144, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_lcp_query", 1, 3, 3, 2); __PYX_ERR(0, 144, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "lcp_query") < 0)) __PYX_ERR(0, 144, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_lcp_query") < 0)) __PYX_ERR(0, 144, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_rank = ((PyArrayObject *)values[0]);
     __pyx_v_segtree = ((PyArrayObject *)values[1]);
     __pyx_v_queries = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("lcp_query", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 144, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_lcp_query", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 144, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("pydivsufsort.stringalg.lcp_query", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pydivsufsort.stringalg._lcp_query", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_rank), __pyx_ptype_5numpy_ndarray, 0, "rank", 0))) __PYX_ERR(0, 145, __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_segtree), __pyx_ptype_5numpy_ndarray, 0, "segtree", 0))) __PYX_ERR(0, 146, __pyx_L1_error)
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_98lcp_query(__pyx_self, __pyx_v_rank, __pyx_v_segtree, __pyx_v_queries);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_100_lcp_query(__pyx_self, __pyx_v_rank, __pyx_v_segtree, __pyx_v_queries);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_98lcp_query(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_rank, PyArrayObject *__pyx_v_segtree, PyObject *__pyx_v_queries) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_100_lcp_query(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_rank, PyArrayObject *__pyx_v_segtree, PyObject *__pyx_v_queries) {
   __pyx_t_5numpy_int32_t __pyx_v_n;
   __pyx_t_5numpy_int32_t __pyx_v_q;
   __pyx_t_5numpy_int32_t __pyx_v_i;
   unsigned PY_LONG_LONG __pyx_v_l;
   unsigned PY_LONG_LONG __pyx_v_r;
   PyArrayObject *__pyx_v_ans = 0;
   PyObject *__pyx_v_res = NULL;
@@ -21449,15 +21454,15 @@
   __pyx_t_5numpy_int32_t __pyx_t_14;
   __pyx_t_5numpy_int32_t __pyx_t_15;
   int __pyx_t_16;
   Py_ssize_t __pyx_t_17;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_fuse_0lcp_query", 0);
+  __Pyx_RefNannySetupContext("__pyx_fuse_0_lcp_query", 0);
   __pyx_pybuffer_ans.pybuffer.buf = NULL;
   __pyx_pybuffer_ans.refcount = 0;
   __pyx_pybuffernd_ans.data = NULL;
   __pyx_pybuffernd_ans.rcbuffer = &__pyx_pybuffer_ans;
   __pyx_pybuffer_rank.pybuffer.buf = NULL;
   __pyx_pybuffer_rank.refcount = 0;
   __pyx_pybuffernd_rank.data = NULL;
@@ -21872,25 +21877,25 @@
   }
 
   /* "pydivsufsort/stringalg.pyx":182
  *             r >>= 1
  *         ans[i] = res
  *     return ans             # <<<<<<<<<<<<<<
  * 
- * def _levenshtein(string_t[::1] a not None, string_t[::1] b not None):
+ * def lcp_query(segtree, queries):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_ans));
   __pyx_r = ((PyObject *)__pyx_v_ans);
   goto __pyx_L0;
 
   /* "pydivsufsort/stringalg.pyx":144
  * 
  * 
- * def lcp_query(             # <<<<<<<<<<<<<<
+ * def _lcp_query(             # <<<<<<<<<<<<<<
  *         np.ndarray[sa_t, ndim=1] rank not None,
  *         np.ndarray[sa_t, ndim=1] segtree not None,
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
@@ -21901,15 +21906,15 @@
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&__pyx_type, &__pyx_value, &__pyx_tb);
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_ans.rcbuffer->pybuffer);
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_rank.rcbuffer->pybuffer);
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_segtree.rcbuffer->pybuffer);
   __Pyx_ErrRestore(__pyx_type, __pyx_value, __pyx_tb);}
-  __Pyx_AddTraceback("pydivsufsort.stringalg.lcp_query", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pydivsufsort.stringalg._lcp_query", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   goto __pyx_L2;
   __pyx_L0:;
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_ans.rcbuffer->pybuffer);
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_rank.rcbuffer->pybuffer);
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_segtree.rcbuffer->pybuffer);
   __pyx_L2:;
@@ -21917,26 +21922,26 @@
   __Pyx_XDECREF(__pyx_v_res);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_1__pyx_pw_12pydivsufsort_9stringalg_101lcp_query(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_1__pyx_mdef_12pydivsufsort_9stringalg_101lcp_query = {"__pyx_fuse_1lcp_query", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_1__pyx_pw_12pydivsufsort_9stringalg_101lcp_query, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_fuse_1__pyx_pw_12pydivsufsort_9stringalg_101lcp_query(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_1__pyx_pw_12pydivsufsort_9stringalg_103_lcp_query(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_1__pyx_mdef_12pydivsufsort_9stringalg_103_lcp_query = {"__pyx_fuse_1_lcp_query", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_1__pyx_pw_12pydivsufsort_9stringalg_103_lcp_query, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_fuse_1__pyx_pw_12pydivsufsort_9stringalg_103_lcp_query(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyArrayObject *__pyx_v_rank = 0;
   PyArrayObject *__pyx_v_segtree = 0;
   PyObject *__pyx_v_queries = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("lcp_query (wrapper)", 0);
+  __Pyx_RefNannySetupContext("_lcp_query (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_rank,&__pyx_n_s_segtree,&__pyx_n_s_queries,0};
     PyObject* values[3] = {0,0,0};
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
@@ -21954,59 +21959,59 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_rank)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_segtree)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("lcp_query", 1, 3, 3, 1); __PYX_ERR(0, 144, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_lcp_query", 1, 3, 3, 1); __PYX_ERR(0, 144, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_queries)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("lcp_query", 1, 3, 3, 2); __PYX_ERR(0, 144, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_lcp_query", 1, 3, 3, 2); __PYX_ERR(0, 144, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "lcp_query") < 0)) __PYX_ERR(0, 144, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_lcp_query") < 0)) __PYX_ERR(0, 144, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_rank = ((PyArrayObject *)values[0]);
     __pyx_v_segtree = ((PyArrayObject *)values[1]);
     __pyx_v_queries = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("lcp_query", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 144, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_lcp_query", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 144, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("pydivsufsort.stringalg.lcp_query", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pydivsufsort.stringalg._lcp_query", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_rank), __pyx_ptype_5numpy_ndarray, 0, "rank", 0))) __PYX_ERR(0, 145, __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_segtree), __pyx_ptype_5numpy_ndarray, 0, "segtree", 0))) __PYX_ERR(0, 146, __pyx_L1_error)
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_100lcp_query(__pyx_self, __pyx_v_rank, __pyx_v_segtree, __pyx_v_queries);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_102_lcp_query(__pyx_self, __pyx_v_rank, __pyx_v_segtree, __pyx_v_queries);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_100lcp_query(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_rank, PyArrayObject *__pyx_v_segtree, PyObject *__pyx_v_queries) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_102_lcp_query(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_rank, PyArrayObject *__pyx_v_segtree, PyObject *__pyx_v_queries) {
   __pyx_t_5numpy_int64_t __pyx_v_n;
   __pyx_t_5numpy_int64_t __pyx_v_q;
   __pyx_t_5numpy_int64_t __pyx_v_i;
   unsigned PY_LONG_LONG __pyx_v_l;
   unsigned PY_LONG_LONG __pyx_v_r;
   PyArrayObject *__pyx_v_ans = 0;
   PyObject *__pyx_v_res = NULL;
@@ -22033,15 +22038,15 @@
   unsigned PY_LONG_LONG __pyx_t_13;
   __pyx_t_5numpy_int64_t __pyx_t_14;
   __pyx_t_5numpy_int64_t __pyx_t_15;
   int __pyx_t_16;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_fuse_1lcp_query", 0);
+  __Pyx_RefNannySetupContext("__pyx_fuse_1_lcp_query", 0);
   __pyx_pybuffer_ans.pybuffer.buf = NULL;
   __pyx_pybuffer_ans.refcount = 0;
   __pyx_pybuffernd_ans.data = NULL;
   __pyx_pybuffernd_ans.rcbuffer = &__pyx_pybuffer_ans;
   __pyx_pybuffer_rank.pybuffer.buf = NULL;
   __pyx_pybuffer_rank.refcount = 0;
   __pyx_pybuffernd_rank.data = NULL;
@@ -22456,25 +22461,25 @@
   }
 
   /* "pydivsufsort/stringalg.pyx":182
  *             r >>= 1
  *         ans[i] = res
  *     return ans             # <<<<<<<<<<<<<<
  * 
- * def _levenshtein(string_t[::1] a not None, string_t[::1] b not None):
+ * def lcp_query(segtree, queries):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_ans));
   __pyx_r = ((PyObject *)__pyx_v_ans);
   goto __pyx_L0;
 
   /* "pydivsufsort/stringalg.pyx":144
  * 
  * 
- * def lcp_query(             # <<<<<<<<<<<<<<
+ * def _lcp_query(             # <<<<<<<<<<<<<<
  *         np.ndarray[sa_t, ndim=1] rank not None,
  *         np.ndarray[sa_t, ndim=1] segtree not None,
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
@@ -22485,15 +22490,15 @@
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&__pyx_type, &__pyx_value, &__pyx_tb);
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_ans.rcbuffer->pybuffer);
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_rank.rcbuffer->pybuffer);
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_segtree.rcbuffer->pybuffer);
   __Pyx_ErrRestore(__pyx_type, __pyx_value, __pyx_tb);}
-  __Pyx_AddTraceback("pydivsufsort.stringalg.lcp_query", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pydivsufsort.stringalg._lcp_query", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   goto __pyx_L2;
   __pyx_L0:;
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_ans.rcbuffer->pybuffer);
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_rank.rcbuffer->pybuffer);
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_segtree.rcbuffer->pybuffer);
   __pyx_L2:;
@@ -22503,23 +22508,159 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "pydivsufsort/stringalg.pyx":184
  *     return ans
  * 
+ * def lcp_query(segtree, queries):             # <<<<<<<<<<<<<<
+ *     return _lcp_query(*segtree, queries)
+ * 
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_12pydivsufsort_9stringalg_15lcp_query(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_12pydivsufsort_9stringalg_15lcp_query = {"lcp_query", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_12pydivsufsort_9stringalg_15lcp_query, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_12pydivsufsort_9stringalg_15lcp_query(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  PyObject *__pyx_v_segtree = 0;
+  PyObject *__pyx_v_queries = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("lcp_query (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_segtree,&__pyx_n_s_queries,0};
+    PyObject* values[2] = {0,0};
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_segtree)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_queries)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("lcp_query", 1, 2, 2, 1); __PYX_ERR(0, 184, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "lcp_query") < 0)) __PYX_ERR(0, 184, __pyx_L3_error)
+      }
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+    }
+    __pyx_v_segtree = values[0];
+    __pyx_v_queries = values[1];
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("lcp_query", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 184, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("pydivsufsort.stringalg.lcp_query", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_14lcp_query(__pyx_self, __pyx_v_segtree, __pyx_v_queries);
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_14lcp_query(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_segtree, PyObject *__pyx_v_queries) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("lcp_query", 0);
+
+  /* "pydivsufsort/stringalg.pyx":185
+ * 
+ * def lcp_query(segtree, queries):
+ *     return _lcp_query(*segtree, queries)             # <<<<<<<<<<<<<<
+ * 
+ * def _levenshtein(string_t[::1] a not None, string_t[::1] b not None):
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_lcp_query); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 185, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = __Pyx_PySequence_Tuple(__pyx_v_segtree); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 185, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 185, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_INCREF(__pyx_v_queries);
+  __Pyx_GIVEREF(__pyx_v_queries);
+  PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_queries);
+  __pyx_t_4 = PyNumber_Add(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 185, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 185, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_r = __pyx_t_3;
+  __pyx_t_3 = 0;
+  goto __pyx_L0;
+
+  /* "pydivsufsort/stringalg.pyx":184
+ *     return ans
+ * 
+ * def lcp_query(segtree, queries):             # <<<<<<<<<<<<<<
+ *     return _lcp_query(*segtree, queries)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_AddTraceback("pydivsufsort.stringalg.lcp_query", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "pydivsufsort/stringalg.pyx":187
+ *     return _lcp_query(*segtree, queries)
+ * 
  * def _levenshtein(string_t[::1] a not None, string_t[::1] b not None):             # <<<<<<<<<<<<<<
  *     cdef unsigned long long n, m, i, j, d
  *     n = len(a)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_12pydivsufsort_9stringalg_15_levenshtein(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_mdef_12pydivsufsort_9stringalg_15_levenshtein = {"_levenshtein", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_12pydivsufsort_9stringalg_15_levenshtein, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_12pydivsufsort_9stringalg_15_levenshtein(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_12pydivsufsort_9stringalg_17_levenshtein(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_12pydivsufsort_9stringalg_17_levenshtein = {"_levenshtein", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_12pydivsufsort_9stringalg_17_levenshtein, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_12pydivsufsort_9stringalg_17_levenshtein(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_signatures = 0;
   PyObject *__pyx_v_args = 0;
   PyObject *__pyx_v_kwargs = 0;
   CYTHON_UNUSED PyObject *__pyx_v_defaults = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -22549,31 +22690,31 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_signatures)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_args)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fused_cpdef", 1, 4, 4, 1); __PYX_ERR(0, 184, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fused_cpdef", 1, 4, 4, 1); __PYX_ERR(0, 187, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_kwargs)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fused_cpdef", 1, 4, 4, 2); __PYX_ERR(0, 184, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fused_cpdef", 1, 4, 4, 2); __PYX_ERR(0, 187, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_defaults)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fused_cpdef", 1, 4, 4, 3); __PYX_ERR(0, 184, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fused_cpdef", 1, 4, 4, 3); __PYX_ERR(0, 187, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fused_cpdef") < 0)) __PYX_ERR(0, 184, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fused_cpdef") < 0)) __PYX_ERR(0, 187, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 4) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
@@ -22582,28 +22723,28 @@
     __pyx_v_signatures = values[0];
     __pyx_v_args = values[1];
     __pyx_v_kwargs = values[2];
     __pyx_v_defaults = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__pyx_fused_cpdef", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 184, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__pyx_fused_cpdef", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 187, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pydivsufsort.stringalg.__pyx_fused_cpdef", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_14_levenshtein(__pyx_self, __pyx_v_signatures, __pyx_v_args, __pyx_v_kwargs, __pyx_v_defaults);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_16_levenshtein(__pyx_self, __pyx_v_signatures, __pyx_v_args, __pyx_v_kwargs, __pyx_v_defaults);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_14_levenshtein(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_signatures, PyObject *__pyx_v_args, PyObject *__pyx_v_kwargs, CYTHON_UNUSED PyObject *__pyx_v_defaults) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_16_levenshtein(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_signatures, PyObject *__pyx_v_args, PyObject *__pyx_v_kwargs, CYTHON_UNUSED PyObject *__pyx_v_defaults) {
   PyObject *__pyx_v_dest_sig = NULL;
   Py_ssize_t __pyx_v_i;
   PyTypeObject *__pyx_v_ndarray = 0;
   __Pyx_memviewslice __pyx_v_memslice;
   Py_ssize_t __pyx_v_itemsize;
   int __pyx_v_dtype_signed;
   char __pyx_v_kind;
@@ -22644,59 +22785,59 @@
   Py_ssize_t __pyx_t_17;
   int __pyx_t_18;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_levenshtein", 0);
   __Pyx_INCREF(__pyx_v_kwargs);
-  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 184, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   PyList_SET_ITEM(__pyx_t_1, 0, Py_None);
   __pyx_v_dest_sig = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_v_kwargs != Py_None);
   __pyx_t_4 = (__pyx_t_3 != 0);
   if (__pyx_t_4) {
   } else {
     __pyx_t_2 = __pyx_t_4;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_kwargs); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 184, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_kwargs); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 187, __pyx_L1_error)
   __pyx_t_3 = ((!__pyx_t_4) != 0);
   __pyx_t_2 = __pyx_t_3;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_2) {
     __Pyx_INCREF(Py_None);
     __Pyx_DECREF_SET(__pyx_v_kwargs, Py_None);
   }
-  __pyx_t_1 = ((PyObject *)__Pyx_ImportNumPyArrayTypeIfAvailable()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 184, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__Pyx_ImportNumPyArrayTypeIfAvailable()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_ndarray = ((PyTypeObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   __pyx_v_itemsize = -1L;
   __pyx_v____pyx_uint8_t_is_signed = (!((((__pyx_t_5numpy_uint8_t)-1L) > 0) != 0));
   __pyx_v____pyx_uint16_t_is_signed = (!((((__pyx_t_5numpy_uint16_t)-1L) > 0) != 0));
   __pyx_v____pyx_uint32_t_is_signed = (!((((__pyx_t_5numpy_uint32_t)-1L) > 0) != 0));
   __pyx_v____pyx_uint64_t_is_signed = (!((((__pyx_t_5numpy_uint64_t)-1L) > 0) != 0));
   __pyx_v____pyx_int8_t_is_signed = (!((((__pyx_t_5numpy_int8_t)-1L) > 0) != 0));
   __pyx_v____pyx_int16_t_is_signed = (!((((__pyx_t_5numpy_int16_t)-1L) > 0) != 0));
   __pyx_v____pyx_int32_t_is_signed = (!((((__pyx_t_5numpy_int32_t)-1L) > 0) != 0));
   __pyx_v____pyx_int64_t_is_signed = (!((((__pyx_t_5numpy_int64_t)-1L) > 0) != 0));
   if (unlikely(__pyx_v_args == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 184, __pyx_L1_error)
+    __PYX_ERR(0, 187, __pyx_L1_error)
   }
-  __pyx_t_5 = PyTuple_GET_SIZE(((PyObject*)__pyx_v_args)); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 184, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_GET_SIZE(((PyObject*)__pyx_v_args)); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 187, __pyx_L1_error)
   __pyx_t_2 = ((0 < __pyx_t_5) != 0);
   if (__pyx_t_2) {
     if (unlikely(__pyx_v_args == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 184, __pyx_L1_error)
+      __PYX_ERR(0, 187, __pyx_L1_error)
     }
     __pyx_t_1 = PyTuple_GET_ITEM(((PyObject*)__pyx_v_args), 0);
     __Pyx_INCREF(__pyx_t_1);
     __pyx_v_arg = __pyx_t_1;
     __pyx_t_1 = 0;
     goto __pyx_L6;
   }
@@ -22705,85 +22846,85 @@
   if (__pyx_t_4) {
   } else {
     __pyx_t_2 = __pyx_t_4;
     goto __pyx_L7_bool_binop_done;
   }
   if (unlikely(__pyx_v_kwargs == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-    __PYX_ERR(0, 184, __pyx_L1_error)
+    __PYX_ERR(0, 187, __pyx_L1_error)
   }
-  __pyx_t_4 = (__Pyx_PyDict_ContainsTF(__pyx_n_s_a, ((PyObject*)__pyx_v_kwargs), Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 184, __pyx_L1_error)
+  __pyx_t_4 = (__Pyx_PyDict_ContainsTF(__pyx_n_s_a, ((PyObject*)__pyx_v_kwargs), Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 187, __pyx_L1_error)
   __pyx_t_3 = (__pyx_t_4 != 0);
   __pyx_t_2 = __pyx_t_3;
   __pyx_L7_bool_binop_done:;
   if (__pyx_t_2) {
     if (unlikely(__pyx_v_kwargs == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 184, __pyx_L1_error)
+      __PYX_ERR(0, 187, __pyx_L1_error)
     }
-    __pyx_t_1 = __Pyx_PyDict_GetItem(((PyObject*)__pyx_v_kwargs), __pyx_n_s_a); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 184, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyDict_GetItem(((PyObject*)__pyx_v_kwargs), __pyx_n_s_a); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 187, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_arg = __pyx_t_1;
     __pyx_t_1 = 0;
     goto __pyx_L6;
   }
   /*else*/ {
     if (unlikely(__pyx_v_args == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-      __PYX_ERR(0, 184, __pyx_L1_error)
+      __PYX_ERR(0, 187, __pyx_L1_error)
     }
-    __pyx_t_5 = PyTuple_GET_SIZE(((PyObject*)__pyx_v_args)); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 184, __pyx_L1_error)
-    __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 184, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_GET_SIZE(((PyObject*)__pyx_v_args)); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 187, __pyx_L1_error)
+    __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 187, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_6 = PyTuple_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 184, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 187, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_INCREF(__pyx_int_2);
     __Pyx_GIVEREF(__pyx_int_2);
     PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_int_2);
     __Pyx_INCREF(__pyx_n_s_s);
     __Pyx_GIVEREF(__pyx_n_s_s);
     PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_n_s_s);
     __Pyx_GIVEREF(__pyx_t_1);
     PyTuple_SET_ITEM(__pyx_t_6, 2, __pyx_t_1);
     __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyString_Format(__pyx_kp_s_Expected_at_least_d_argument_s_g, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 184, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyString_Format(__pyx_kp_s_Expected_at_least_d_argument_s_g, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 187, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 184, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 187, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_6, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __PYX_ERR(0, 184, __pyx_L1_error)
+    __PYX_ERR(0, 187, __pyx_L1_error)
   }
   __pyx_L6:;
   while (1) {
     __pyx_t_2 = (__pyx_v_ndarray != ((PyTypeObject*)Py_None));
     __pyx_t_3 = (__pyx_t_2 != 0);
     if (__pyx_t_3) {
       __pyx_t_3 = __Pyx_TypeCheck(__pyx_v_arg, __pyx_v_ndarray); 
       __pyx_t_2 = (__pyx_t_3 != 0);
       if (__pyx_t_2) {
-        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_dtype); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 184, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_dtype); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 187, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         __pyx_v_dtype = __pyx_t_6;
         __pyx_t_6 = 0;
         goto __pyx_L12;
       }
       __pyx_t_2 = __pyx_memoryview_check(__pyx_v_arg); 
       __pyx_t_3 = (__pyx_t_2 != 0);
       if (__pyx_t_3) {
-        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_base); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 184, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_base); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 187, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         __pyx_v_arg_base = __pyx_t_6;
         __pyx_t_6 = 0;
         __pyx_t_3 = __Pyx_TypeCheck(__pyx_v_arg_base, __pyx_v_ndarray); 
         __pyx_t_2 = (__pyx_t_3 != 0);
         if (__pyx_t_2) {
-          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg_base, __pyx_n_s_dtype); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 184, __pyx_L1_error)
+          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg_base, __pyx_n_s_dtype); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 187, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
           __pyx_v_dtype = __pyx_t_6;
           __pyx_t_6 = 0;
           goto __pyx_L13;
         }
         /*else*/ {
           __Pyx_INCREF(Py_None);
@@ -22797,210 +22938,210 @@
         __pyx_v_dtype = Py_None;
       }
       __pyx_L12:;
       __pyx_v_itemsize = -1L;
       __pyx_t_2 = (__pyx_v_dtype != Py_None);
       __pyx_t_3 = (__pyx_t_2 != 0);
       if (__pyx_t_3) {
-        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_dtype, __pyx_n_s_itemsize); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 184, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_dtype, __pyx_n_s_itemsize); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 187, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
-        __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 184, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 187, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __pyx_v_itemsize = __pyx_t_5;
-        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_dtype, __pyx_n_s_kind); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 184, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_dtype, __pyx_n_s_kind); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 187, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
-        __pyx_t_7 = __Pyx_PyObject_Ord(__pyx_t_6); if (unlikely(__pyx_t_7 == ((long)(long)(Py_UCS4)-1))) __PYX_ERR(0, 184, __pyx_L1_error)
+        __pyx_t_7 = __Pyx_PyObject_Ord(__pyx_t_6); if (unlikely(__pyx_t_7 == ((long)(long)(Py_UCS4)-1))) __PYX_ERR(0, 187, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __pyx_v_kind = __pyx_t_7;
         __pyx_v_dtype_signed = (__pyx_v_kind == 'i');
         switch (__pyx_v_kind) {
           case 'i':
           case 'u':
           __pyx_t_2 = (((sizeof(__pyx_t_5numpy_uint8_t)) == __pyx_v_itemsize) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L16_bool_binop_done;
           }
-          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 184, __pyx_L1_error)
+          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 187, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
-          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 184, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 187, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           __pyx_t_2 = ((((Py_ssize_t)__pyx_t_5) == 1) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L16_bool_binop_done;
           }
           __pyx_t_2 = ((!((__pyx_v____pyx_uint8_t_is_signed ^ __pyx_v_dtype_signed) != 0)) != 0);
           __pyx_t_3 = __pyx_t_2;
           __pyx_L16_bool_binop_done:;
           if (__pyx_t_3) {
-            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_uint8_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 184, __pyx_L1_error)
+            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_uint8_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 187, __pyx_L1_error)
             goto __pyx_L10_break;
           }
           __pyx_t_2 = (((sizeof(__pyx_t_5numpy_uint16_t)) == __pyx_v_itemsize) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L20_bool_binop_done;
           }
-          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 184, __pyx_L1_error)
+          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 187, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
-          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 184, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 187, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           __pyx_t_2 = ((((Py_ssize_t)__pyx_t_5) == 1) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L20_bool_binop_done;
           }
           __pyx_t_2 = ((!((__pyx_v____pyx_uint16_t_is_signed ^ __pyx_v_dtype_signed) != 0)) != 0);
           __pyx_t_3 = __pyx_t_2;
           __pyx_L20_bool_binop_done:;
           if (__pyx_t_3) {
-            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_uint16_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 184, __pyx_L1_error)
+            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_uint16_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 187, __pyx_L1_error)
             goto __pyx_L10_break;
           }
           __pyx_t_2 = (((sizeof(__pyx_t_5numpy_uint32_t)) == __pyx_v_itemsize) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L24_bool_binop_done;
           }
-          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 184, __pyx_L1_error)
+          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 187, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
-          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 184, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 187, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           __pyx_t_2 = ((((Py_ssize_t)__pyx_t_5) == 1) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L24_bool_binop_done;
           }
           __pyx_t_2 = ((!((__pyx_v____pyx_uint32_t_is_signed ^ __pyx_v_dtype_signed) != 0)) != 0);
           __pyx_t_3 = __pyx_t_2;
           __pyx_L24_bool_binop_done:;
           if (__pyx_t_3) {
-            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_uint32_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 184, __pyx_L1_error)
+            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_uint32_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 187, __pyx_L1_error)
             goto __pyx_L10_break;
           }
           __pyx_t_2 = (((sizeof(__pyx_t_5numpy_uint64_t)) == __pyx_v_itemsize) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L28_bool_binop_done;
           }
-          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 184, __pyx_L1_error)
+          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 187, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
-          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 184, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 187, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           __pyx_t_2 = ((((Py_ssize_t)__pyx_t_5) == 1) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L28_bool_binop_done;
           }
           __pyx_t_2 = ((!((__pyx_v____pyx_uint64_t_is_signed ^ __pyx_v_dtype_signed) != 0)) != 0);
           __pyx_t_3 = __pyx_t_2;
           __pyx_L28_bool_binop_done:;
           if (__pyx_t_3) {
-            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_uint64_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 184, __pyx_L1_error)
+            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_uint64_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 187, __pyx_L1_error)
             goto __pyx_L10_break;
           }
           __pyx_t_2 = (((sizeof(__pyx_t_5numpy_int8_t)) == __pyx_v_itemsize) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L32_bool_binop_done;
           }
-          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 184, __pyx_L1_error)
+          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 187, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
-          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 184, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 187, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           __pyx_t_2 = ((((Py_ssize_t)__pyx_t_5) == 1) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L32_bool_binop_done;
           }
           __pyx_t_2 = ((!((__pyx_v____pyx_int8_t_is_signed ^ __pyx_v_dtype_signed) != 0)) != 0);
           __pyx_t_3 = __pyx_t_2;
           __pyx_L32_bool_binop_done:;
           if (__pyx_t_3) {
-            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int8_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 184, __pyx_L1_error)
+            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int8_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 187, __pyx_L1_error)
             goto __pyx_L10_break;
           }
           __pyx_t_2 = (((sizeof(__pyx_t_5numpy_int16_t)) == __pyx_v_itemsize) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L36_bool_binop_done;
           }
-          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 184, __pyx_L1_error)
+          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 187, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
-          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 184, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 187, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           __pyx_t_2 = ((((Py_ssize_t)__pyx_t_5) == 1) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L36_bool_binop_done;
           }
           __pyx_t_2 = ((!((__pyx_v____pyx_int16_t_is_signed ^ __pyx_v_dtype_signed) != 0)) != 0);
           __pyx_t_3 = __pyx_t_2;
           __pyx_L36_bool_binop_done:;
           if (__pyx_t_3) {
-            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int16_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 184, __pyx_L1_error)
+            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int16_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 187, __pyx_L1_error)
             goto __pyx_L10_break;
           }
           __pyx_t_2 = (((sizeof(__pyx_t_5numpy_int32_t)) == __pyx_v_itemsize) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L40_bool_binop_done;
           }
-          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 184, __pyx_L1_error)
+          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 187, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
-          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 184, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 187, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           __pyx_t_2 = ((((Py_ssize_t)__pyx_t_5) == 1) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L40_bool_binop_done;
           }
           __pyx_t_2 = ((!((__pyx_v____pyx_int32_t_is_signed ^ __pyx_v_dtype_signed) != 0)) != 0);
           __pyx_t_3 = __pyx_t_2;
           __pyx_L40_bool_binop_done:;
           if (__pyx_t_3) {
-            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int32_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 184, __pyx_L1_error)
+            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int32_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 187, __pyx_L1_error)
             goto __pyx_L10_break;
           }
           __pyx_t_2 = (((sizeof(__pyx_t_5numpy_int64_t)) == __pyx_v_itemsize) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L44_bool_binop_done;
           }
-          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 184, __pyx_L1_error)
+          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 187, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
-          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 184, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 187, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           __pyx_t_2 = ((((Py_ssize_t)__pyx_t_5) == 1) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L44_bool_binop_done;
           }
           __pyx_t_2 = ((!((__pyx_v____pyx_int64_t_is_signed ^ __pyx_v_dtype_signed) != 0)) != 0);
           __pyx_t_3 = __pyx_t_2;
           __pyx_L44_bool_binop_done:;
           if (__pyx_t_3) {
-            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int64_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 184, __pyx_L1_error)
+            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int64_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 187, __pyx_L1_error)
             goto __pyx_L10_break;
           }
           break;
           case 'f':
           break;
           case 'c':
           break;
@@ -23021,15 +23162,15 @@
     __pyx_L48_bool_binop_done:;
     if (__pyx_t_3) {
       __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_uint8_t(__pyx_v_arg, 0); 
       __pyx_v_memslice = __pyx_t_8;
       __pyx_t_3 = (__pyx_v_memslice.memview != 0);
       if (__pyx_t_3) {
         __PYX_XDEC_MEMVIEW((&__pyx_v_memslice), 1); 
-        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_uint8_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 184, __pyx_L1_error)
+        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_uint8_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 187, __pyx_L1_error)
         goto __pyx_L10_break;
       }
       /*else*/ {
         PyErr_Clear(); 
       }
     }
     __pyx_t_2 = ((__pyx_v_itemsize == -1L) != 0);
@@ -23043,15 +23184,15 @@
     __pyx_L52_bool_binop_done:;
     if (__pyx_t_3) {
       __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_uint16_t(__pyx_v_arg, 0); 
       __pyx_v_memslice = __pyx_t_8;
       __pyx_t_3 = (__pyx_v_memslice.memview != 0);
       if (__pyx_t_3) {
         __PYX_XDEC_MEMVIEW((&__pyx_v_memslice), 1); 
-        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_uint16_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 184, __pyx_L1_error)
+        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_uint16_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 187, __pyx_L1_error)
         goto __pyx_L10_break;
       }
       /*else*/ {
         PyErr_Clear(); 
       }
     }
     __pyx_t_2 = ((__pyx_v_itemsize == -1L) != 0);
@@ -23065,15 +23206,15 @@
     __pyx_L56_bool_binop_done:;
     if (__pyx_t_3) {
       __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_uint32_t(__pyx_v_arg, 0); 
       __pyx_v_memslice = __pyx_t_8;
       __pyx_t_3 = (__pyx_v_memslice.memview != 0);
       if (__pyx_t_3) {
         __PYX_XDEC_MEMVIEW((&__pyx_v_memslice), 1); 
-        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_uint32_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 184, __pyx_L1_error)
+        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_uint32_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 187, __pyx_L1_error)
         goto __pyx_L10_break;
       }
       /*else*/ {
         PyErr_Clear(); 
       }
     }
     __pyx_t_2 = ((__pyx_v_itemsize == -1L) != 0);
@@ -23087,15 +23228,15 @@
     __pyx_L60_bool_binop_done:;
     if (__pyx_t_3) {
       __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_uint64_t(__pyx_v_arg, 0); 
       __pyx_v_memslice = __pyx_t_8;
       __pyx_t_3 = (__pyx_v_memslice.memview != 0);
       if (__pyx_t_3) {
         __PYX_XDEC_MEMVIEW((&__pyx_v_memslice), 1); 
-        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_uint64_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 184, __pyx_L1_error)
+        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_uint64_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 187, __pyx_L1_error)
         goto __pyx_L10_break;
       }
       /*else*/ {
         PyErr_Clear(); 
       }
     }
     __pyx_t_2 = ((__pyx_v_itemsize == -1L) != 0);
@@ -23109,15 +23250,15 @@
     __pyx_L64_bool_binop_done:;
     if (__pyx_t_3) {
       __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_int8_t(__pyx_v_arg, 0); 
       __pyx_v_memslice = __pyx_t_8;
       __pyx_t_3 = (__pyx_v_memslice.memview != 0);
       if (__pyx_t_3) {
         __PYX_XDEC_MEMVIEW((&__pyx_v_memslice), 1); 
-        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int8_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 184, __pyx_L1_error)
+        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int8_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 187, __pyx_L1_error)
         goto __pyx_L10_break;
       }
       /*else*/ {
         PyErr_Clear(); 
       }
     }
     __pyx_t_2 = ((__pyx_v_itemsize == -1L) != 0);
@@ -23131,15 +23272,15 @@
     __pyx_L68_bool_binop_done:;
     if (__pyx_t_3) {
       __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_int16_t(__pyx_v_arg, 0); 
       __pyx_v_memslice = __pyx_t_8;
       __pyx_t_3 = (__pyx_v_memslice.memview != 0);
       if (__pyx_t_3) {
         __PYX_XDEC_MEMVIEW((&__pyx_v_memslice), 1); 
-        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int16_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 184, __pyx_L1_error)
+        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int16_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 187, __pyx_L1_error)
         goto __pyx_L10_break;
       }
       /*else*/ {
         PyErr_Clear(); 
       }
     }
     __pyx_t_2 = ((__pyx_v_itemsize == -1L) != 0);
@@ -23153,15 +23294,15 @@
     __pyx_L72_bool_binop_done:;
     if (__pyx_t_3) {
       __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_int32_t(__pyx_v_arg, 0); 
       __pyx_v_memslice = __pyx_t_8;
       __pyx_t_3 = (__pyx_v_memslice.memview != 0);
       if (__pyx_t_3) {
         __PYX_XDEC_MEMVIEW((&__pyx_v_memslice), 1); 
-        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int32_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 184, __pyx_L1_error)
+        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int32_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 187, __pyx_L1_error)
         goto __pyx_L10_break;
       }
       /*else*/ {
         PyErr_Clear(); 
       }
     }
     __pyx_t_2 = ((__pyx_v_itemsize == -1L) != 0);
@@ -23175,100 +23316,100 @@
     __pyx_L76_bool_binop_done:;
     if (__pyx_t_3) {
       __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_int64_t(__pyx_v_arg, 0); 
       __pyx_v_memslice = __pyx_t_8;
       __pyx_t_3 = (__pyx_v_memslice.memview != 0);
       if (__pyx_t_3) {
         __PYX_XDEC_MEMVIEW((&__pyx_v_memslice), 1); 
-        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int64_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 184, __pyx_L1_error)
+        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int64_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 187, __pyx_L1_error)
         goto __pyx_L10_break;
       }
       /*else*/ {
         PyErr_Clear(); 
       }
     }
-    if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, Py_None, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 184, __pyx_L1_error)
+    if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, Py_None, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 187, __pyx_L1_error)
     goto __pyx_L10_break;
   }
   __pyx_L10_break:;
-  __pyx_t_6 = PyList_New(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 184, __pyx_L1_error)
+  __pyx_t_6 = PyList_New(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_v_candidates = ((PyObject*)__pyx_t_6);
   __pyx_t_6 = 0;
   __pyx_t_5 = 0;
   if (unlikely(__pyx_v_signatures == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-    __PYX_ERR(0, 184, __pyx_L1_error)
+    __PYX_ERR(0, 187, __pyx_L1_error)
   }
-  __pyx_t_1 = __Pyx_dict_iterator(((PyObject*)__pyx_v_signatures), 1, ((PyObject *)NULL), (&__pyx_t_9), (&__pyx_t_10)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 184, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_dict_iterator(((PyObject*)__pyx_v_signatures), 1, ((PyObject *)NULL), (&__pyx_t_9), (&__pyx_t_10)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_6);
   __pyx_t_6 = __pyx_t_1;
   __pyx_t_1 = 0;
   while (1) {
     __pyx_t_11 = __Pyx_dict_iter_next(__pyx_t_6, __pyx_t_9, &__pyx_t_5, &__pyx_t_1, NULL, NULL, __pyx_t_10);
     if (unlikely(__pyx_t_11 == 0)) break;
-    if (unlikely(__pyx_t_11 == -1)) __PYX_ERR(0, 184, __pyx_L1_error)
+    if (unlikely(__pyx_t_11 == -1)) __PYX_ERR(0, 187, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_XDECREF_SET(__pyx_v_sig, __pyx_t_1);
     __pyx_t_1 = 0;
     __pyx_v_match_found = 0;
-    __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_v_sig, __pyx_n_s_strip); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 184, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_v_sig, __pyx_n_s_strip); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 187, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_13);
     __pyx_t_14 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_13))) {
       __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_13);
       if (likely(__pyx_t_14)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_13);
         __Pyx_INCREF(__pyx_t_14);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_13, function);
       }
     }
     __pyx_t_12 = (__pyx_t_14) ? __Pyx_PyObject_Call2Args(__pyx_t_13, __pyx_t_14, __pyx_kp_s__2) : __Pyx_PyObject_CallOneArg(__pyx_t_13, __pyx_kp_s__2);
     __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
-    if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 184, __pyx_L1_error)
+    if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 187, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_12);
     __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-    __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_split); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 184, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_split); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 187, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_13);
     __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
     __pyx_t_12 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_13))) {
       __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_13);
       if (likely(__pyx_t_12)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_13);
         __Pyx_INCREF(__pyx_t_12);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_13, function);
       }
     }
     __pyx_t_1 = (__pyx_t_12) ? __Pyx_PyObject_Call2Args(__pyx_t_13, __pyx_t_12, __pyx_kp_s__3) : __Pyx_PyObject_CallOneArg(__pyx_t_13, __pyx_kp_s__3);
     __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 184, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 187, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
     __Pyx_XDECREF_SET(__pyx_v_src_sig, __pyx_t_1);
     __pyx_t_1 = 0;
-    __pyx_t_15 = PyList_GET_SIZE(__pyx_v_dest_sig); if (unlikely(__pyx_t_15 == ((Py_ssize_t)-1))) __PYX_ERR(0, 184, __pyx_L1_error)
+    __pyx_t_15 = PyList_GET_SIZE(__pyx_v_dest_sig); if (unlikely(__pyx_t_15 == ((Py_ssize_t)-1))) __PYX_ERR(0, 187, __pyx_L1_error)
     __pyx_t_16 = __pyx_t_15;
     for (__pyx_t_17 = 0; __pyx_t_17 < __pyx_t_16; __pyx_t_17+=1) {
       __pyx_v_i = __pyx_t_17;
       __pyx_t_1 = PyList_GET_ITEM(__pyx_v_dest_sig, __pyx_v_i);
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_XDECREF_SET(__pyx_v_dst_type, __pyx_t_1);
       __pyx_t_1 = 0;
       __pyx_t_3 = (__pyx_v_dst_type != Py_None);
       __pyx_t_2 = (__pyx_t_3 != 0);
       if (__pyx_t_2) {
-        __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_src_sig, __pyx_v_i, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 184, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_src_sig, __pyx_v_i, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 187, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_13 = PyObject_RichCompare(__pyx_t_1, __pyx_v_dst_type, Py_EQ); __Pyx_XGOTREF(__pyx_t_13); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 184, __pyx_L1_error)
+        __pyx_t_13 = PyObject_RichCompare(__pyx_t_1, __pyx_v_dst_type, Py_EQ); __Pyx_XGOTREF(__pyx_t_13); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 187, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_13); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 184, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_13); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 187, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
         if (__pyx_t_2) {
           __pyx_v_match_found = 1;
           goto __pyx_L84;
         }
         /*else*/ {
           __pyx_v_match_found = 0;
@@ -23276,43 +23417,43 @@
         }
         __pyx_L84:;
       }
     }
     __pyx_L82_break:;
     __pyx_t_2 = (__pyx_v_match_found != 0);
     if (__pyx_t_2) {
-      __pyx_t_18 = __Pyx_PyList_Append(__pyx_v_candidates, __pyx_v_sig); if (unlikely(__pyx_t_18 == ((int)-1))) __PYX_ERR(0, 184, __pyx_L1_error)
+      __pyx_t_18 = __Pyx_PyList_Append(__pyx_v_candidates, __pyx_v_sig); if (unlikely(__pyx_t_18 == ((int)-1))) __PYX_ERR(0, 187, __pyx_L1_error)
     }
   }
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_2 = (PyList_GET_SIZE(__pyx_v_candidates) != 0);
   __pyx_t_3 = ((!__pyx_t_2) != 0);
   if (__pyx_t_3) {
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 184, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 187, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_Raise(__pyx_t_6, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __PYX_ERR(0, 184, __pyx_L1_error)
+    __PYX_ERR(0, 187, __pyx_L1_error)
   }
-  __pyx_t_9 = PyList_GET_SIZE(__pyx_v_candidates); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 184, __pyx_L1_error)
+  __pyx_t_9 = PyList_GET_SIZE(__pyx_v_candidates); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 187, __pyx_L1_error)
   __pyx_t_3 = ((__pyx_t_9 > 1) != 0);
   if (__pyx_t_3) {
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 184, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 187, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_Raise(__pyx_t_6, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __PYX_ERR(0, 184, __pyx_L1_error)
+    __PYX_ERR(0, 187, __pyx_L1_error)
   }
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     if (unlikely(__pyx_v_signatures == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 184, __pyx_L1_error)
+      __PYX_ERR(0, 187, __pyx_L1_error)
     }
-    __pyx_t_6 = __Pyx_PyDict_GetItem(((PyObject*)__pyx_v_signatures), PyList_GET_ITEM(__pyx_v_candidates, 0)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 184, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyDict_GetItem(((PyObject*)__pyx_v_signatures), PyList_GET_ITEM(__pyx_v_candidates, 0)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 187, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_r = __pyx_t_6;
     __pyx_t_6 = 0;
     goto __pyx_L0;
   }
 
   /* function exit code */
@@ -23337,17 +23478,17 @@
   __Pyx_XDECREF(__pyx_v_kwargs);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_0__pyx_pw_12pydivsufsort_9stringalg_105_levenshtein(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_0__pyx_mdef_12pydivsufsort_9stringalg_105_levenshtein = {"__pyx_fuse_0_levenshtein", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_0__pyx_pw_12pydivsufsort_9stringalg_105_levenshtein, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_fuse_0__pyx_pw_12pydivsufsort_9stringalg_105_levenshtein(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_0__pyx_pw_12pydivsufsort_9stringalg_107_levenshtein(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_0__pyx_mdef_12pydivsufsort_9stringalg_107_levenshtein = {"__pyx_fuse_0_levenshtein", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_0__pyx_pw_12pydivsufsort_9stringalg_107_levenshtein, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_fuse_0__pyx_pw_12pydivsufsort_9stringalg_107_levenshtein(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_a = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_b = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -23371,55 +23512,55 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_a)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_b)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_levenshtein", 1, 2, 2, 1); __PYX_ERR(0, 184, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_levenshtein", 1, 2, 2, 1); __PYX_ERR(0, 187, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_levenshtein") < 0)) __PYX_ERR(0, 184, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_levenshtein") < 0)) __PYX_ERR(0, 187, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
-    __pyx_v_a = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_uint8_t(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_a.memview)) __PYX_ERR(0, 184, __pyx_L3_error)
-    __pyx_v_b = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_uint8_t(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_b.memview)) __PYX_ERR(0, 184, __pyx_L3_error)
+    __pyx_v_a = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_uint8_t(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_a.memview)) __PYX_ERR(0, 187, __pyx_L3_error)
+    __pyx_v_b = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_uint8_t(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_b.memview)) __PYX_ERR(0, 187, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_levenshtein", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 184, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_levenshtein", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 187, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pydivsufsort.stringalg._levenshtein", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(((PyObject *)__pyx_v_a.memview) == Py_None)) {
-    PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "a"); __PYX_ERR(0, 184, __pyx_L1_error)
+    PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "a"); __PYX_ERR(0, 187, __pyx_L1_error)
   }
   if (unlikely(((PyObject *)__pyx_v_b.memview) == Py_None)) {
-    PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "b"); __PYX_ERR(0, 184, __pyx_L1_error)
+    PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "b"); __PYX_ERR(0, 187, __pyx_L1_error)
   }
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_104_levenshtein(__pyx_self, __pyx_v_a, __pyx_v_b);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_106_levenshtein(__pyx_self, __pyx_v_a, __pyx_v_b);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_104_levenshtein(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_a, __Pyx_memviewslice __pyx_v_b) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_106_levenshtein(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_a, __Pyx_memviewslice __pyx_v_b) {
   unsigned PY_LONG_LONG __pyx_v_n;
   unsigned PY_LONG_LONG __pyx_v_m;
   unsigned PY_LONG_LONG __pyx_v_i;
   unsigned PY_LONG_LONG __pyx_v_j;
   PyArrayObject *__pyx_v_temp = 0;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_temp;
   __Pyx_Buffer __pyx_pybuffer_temp;
@@ -23446,225 +23587,225 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_0_levenshtein", 0);
   __pyx_pybuffer_temp.pybuffer.buf = NULL;
   __pyx_pybuffer_temp.refcount = 0;
   __pyx_pybuffernd_temp.data = NULL;
   __pyx_pybuffernd_temp.rcbuffer = &__pyx_pybuffer_temp;
 
-  /* "pydivsufsort/stringalg.pyx":186
+  /* "pydivsufsort/stringalg.pyx":189
  * def _levenshtein(string_t[::1] a not None, string_t[::1] b not None):
  *     cdef unsigned long long n, m, i, j, d
  *     n = len(a)             # <<<<<<<<<<<<<<
  *     m = len(b)
  *     cdef np.ndarray[np.uint64_t, ndim=2] temp = np.empty((n+1, m+1), dtype=np.uint64)
  */
   __pyx_t_1 = __Pyx_MemoryView_Len(__pyx_v_a); 
   __pyx_v_n = __pyx_t_1;
 
-  /* "pydivsufsort/stringalg.pyx":187
+  /* "pydivsufsort/stringalg.pyx":190
  *     cdef unsigned long long n, m, i, j, d
  *     n = len(a)
  *     m = len(b)             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.uint64_t, ndim=2] temp = np.empty((n+1, m+1), dtype=np.uint64)
  *     for i in range(n):
  */
   __pyx_t_1 = __Pyx_MemoryView_Len(__pyx_v_b); 
   __pyx_v_m = __pyx_t_1;
 
-  /* "pydivsufsort/stringalg.pyx":188
+  /* "pydivsufsort/stringalg.pyx":191
  *     n = len(a)
  *     m = len(b)
  *     cdef np.ndarray[np.uint64_t, ndim=2] temp = np.empty((n+1, m+1), dtype=np.uint64)             # <<<<<<<<<<<<<<
  *     for i in range(n):
  *         temp[i][0] = i
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG((__pyx_v_n + 1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG((__pyx_v_n + 1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG((__pyx_v_m + 1)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG((__pyx_v_m + 1)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_4);
   __pyx_t_2 = 0;
   __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5);
   __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_uint64); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_uint64); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 188, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 188, __pyx_L1_error)
+  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 191, __pyx_L1_error)
   __pyx_t_7 = ((PyArrayObject *)__pyx_t_6);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_temp.rcbuffer->pybuffer, (PyObject*)__pyx_t_7, &__Pyx_TypeInfo_nn___pyx_t_5numpy_uint64_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_temp = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_temp.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 188, __pyx_L1_error)
+      __PYX_ERR(0, 191, __pyx_L1_error)
     } else {__pyx_pybuffernd_temp.diminfo[0].strides = __pyx_pybuffernd_temp.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_temp.diminfo[0].shape = __pyx_pybuffernd_temp.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_temp.diminfo[1].strides = __pyx_pybuffernd_temp.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_temp.diminfo[1].shape = __pyx_pybuffernd_temp.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_t_7 = 0;
   __pyx_v_temp = ((PyArrayObject *)__pyx_t_6);
   __pyx_t_6 = 0;
 
-  /* "pydivsufsort/stringalg.pyx":189
+  /* "pydivsufsort/stringalg.pyx":192
  *     m = len(b)
  *     cdef np.ndarray[np.uint64_t, ndim=2] temp = np.empty((n+1, m+1), dtype=np.uint64)
  *     for i in range(n):             # <<<<<<<<<<<<<<
  *         temp[i][0] = i
  *     for j in range(m):
  */
   __pyx_t_8 = __pyx_v_n;
   __pyx_t_9 = __pyx_t_8;
   for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
     __pyx_v_i = __pyx_t_10;
 
-    /* "pydivsufsort/stringalg.pyx":190
+    /* "pydivsufsort/stringalg.pyx":193
  *     cdef np.ndarray[np.uint64_t, ndim=2] temp = np.empty((n+1, m+1), dtype=np.uint64)
  *     for i in range(n):
  *         temp[i][0] = i             # <<<<<<<<<<<<<<
  *     for j in range(m):
  *         temp[0][j] = j
  */
-    __pyx_t_6 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG(__pyx_v_i); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 190, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG(__pyx_v_i); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 193, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 190, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 193, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (unlikely(__Pyx_SetItemInt(__pyx_t_5, 0, __pyx_t_6, long, 1, __Pyx_PyInt_From_long, 0, 0, 0) < 0)) __PYX_ERR(0, 190, __pyx_L1_error)
+    if (unlikely(__Pyx_SetItemInt(__pyx_t_5, 0, __pyx_t_6, long, 1, __Pyx_PyInt_From_long, 0, 0, 0) < 0)) __PYX_ERR(0, 193, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
 
-  /* "pydivsufsort/stringalg.pyx":191
+  /* "pydivsufsort/stringalg.pyx":194
  *     for i in range(n):
  *         temp[i][0] = i
  *     for j in range(m):             # <<<<<<<<<<<<<<
  *         temp[0][j] = j
  *     for i in range(n):
  */
   __pyx_t_8 = __pyx_v_m;
   __pyx_t_9 = __pyx_t_8;
   for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
     __pyx_v_j = __pyx_t_10;
 
-    /* "pydivsufsort/stringalg.pyx":192
+    /* "pydivsufsort/stringalg.pyx":195
  *         temp[i][0] = i
  *     for j in range(m):
  *         temp[0][j] = j             # <<<<<<<<<<<<<<
  *     for i in range(n):
  *         for j in range(m):
  */
-    __pyx_t_6 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG(__pyx_v_j); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 192, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG(__pyx_v_j); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 195, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 192, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (unlikely(__Pyx_SetItemInt(__pyx_t_5, __pyx_v_j, __pyx_t_6, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0) < 0)) __PYX_ERR(0, 192, __pyx_L1_error)
+    if (unlikely(__Pyx_SetItemInt(__pyx_t_5, __pyx_v_j, __pyx_t_6, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0) < 0)) __PYX_ERR(0, 195, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
 
-  /* "pydivsufsort/stringalg.pyx":193
+  /* "pydivsufsort/stringalg.pyx":196
  *     for j in range(m):
  *         temp[0][j] = j
  *     for i in range(n):             # <<<<<<<<<<<<<<
  *         for j in range(m):
  *             temp[i+1][j+1] = min(temp[i][j+1] + 1, temp[i+1][j] + 1, temp[i][j] + (a[i] != b[j]))
  */
   __pyx_t_8 = __pyx_v_n;
   __pyx_t_9 = __pyx_t_8;
   for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
     __pyx_v_i = __pyx_t_10;
 
-    /* "pydivsufsort/stringalg.pyx":194
+    /* "pydivsufsort/stringalg.pyx":197
  *         temp[0][j] = j
  *     for i in range(n):
  *         for j in range(m):             # <<<<<<<<<<<<<<
  *             temp[i+1][j+1] = min(temp[i][j+1] + 1, temp[i+1][j] + 1, temp[i][j] + (a[i] != b[j]))
  *     return temp[n][m]
  */
     __pyx_t_11 = __pyx_v_m;
     __pyx_t_12 = __pyx_t_11;
     for (__pyx_t_13 = 0; __pyx_t_13 < __pyx_t_12; __pyx_t_13+=1) {
       __pyx_v_j = __pyx_t_13;
 
-      /* "pydivsufsort/stringalg.pyx":195
+      /* "pydivsufsort/stringalg.pyx":198
  *     for i in range(n):
  *         for j in range(m):
  *             temp[i+1][j+1] = min(temp[i][j+1] + 1, temp[i+1][j] + 1, temp[i][j] + (a[i] != b[j]))             # <<<<<<<<<<<<<<
  *     return temp[n][m]
  * 
  */
       __pyx_t_14 = (__pyx_v_i + 1);
-      __pyx_t_6 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_t_14, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_t_14, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_5 = __Pyx_GetItemInt(__pyx_t_6, __pyx_v_j, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_GetItemInt(__pyx_t_6, __pyx_v_j, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __pyx_t_6 = __Pyx_PyInt_AddObjC(__pyx_t_5, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyInt_AddObjC(__pyx_t_5, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_5, __pyx_v_j, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_5, __pyx_v_j, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_t_14 = __pyx_v_i;
       __pyx_t_15 = __pyx_v_j;
-      __pyx_t_5 = __Pyx_PyBool_FromLong(((*((__pyx_t_5numpy_uint8_t *) ( /* dim=0 */ ((char *) (((__pyx_t_5numpy_uint8_t *) __pyx_v_a.data) + __pyx_t_14)) ))) != (*((__pyx_t_5numpy_uint8_t *) ( /* dim=0 */ ((char *) (((__pyx_t_5numpy_uint8_t *) __pyx_v_b.data) + __pyx_t_15)) ))))); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyBool_FromLong(((*((__pyx_t_5numpy_uint8_t *) ( /* dim=0 */ ((char *) (((__pyx_t_5numpy_uint8_t *) __pyx_v_a.data) + __pyx_t_14)) ))) != (*((__pyx_t_5numpy_uint8_t *) ( /* dim=0 */ ((char *) (((__pyx_t_5numpy_uint8_t *) __pyx_v_b.data) + __pyx_t_15)) ))))); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_3 = PyNumber_Add(__pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_3 = PyNumber_Add(__pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __pyx_t_15 = (__pyx_v_j + 1);
-      __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_5, __pyx_t_15, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_5, __pyx_t_15, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_5 = __Pyx_PyInt_AddObjC(__pyx_t_4, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyInt_AddObjC(__pyx_t_4, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_2 = PyObject_RichCompare(__pyx_t_6, __pyx_t_5, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 195, __pyx_L1_error)
-      __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_2 = PyObject_RichCompare(__pyx_t_6, __pyx_t_5, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 198, __pyx_L1_error)
+      __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       if (__pyx_t_16) {
         __Pyx_INCREF(__pyx_t_6);
         __pyx_t_4 = __pyx_t_6;
       } else {
         __Pyx_INCREF(__pyx_t_5);
         __pyx_t_4 = __pyx_t_5;
       }
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_INCREF(__pyx_t_4);
       __pyx_t_5 = __pyx_t_4;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_2 = PyObject_RichCompare(__pyx_t_3, __pyx_t_5, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 195, __pyx_L1_error)
-      __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_2 = PyObject_RichCompare(__pyx_t_3, __pyx_t_5, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 198, __pyx_L1_error)
+      __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       if (__pyx_t_16) {
         __Pyx_INCREF(__pyx_t_3);
         __pyx_t_4 = __pyx_t_3;
       } else {
         __Pyx_INCREF(__pyx_t_5);
         __pyx_t_4 = __pyx_t_5;
@@ -23672,42 +23813,42 @@
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __pyx_t_6 = __pyx_t_4;
       __Pyx_INCREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_t_15 = (__pyx_v_i + 1);
-      __pyx_t_4 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_t_15, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_t_15, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_15 = (__pyx_v_j + 1);
-      if (unlikely(__Pyx_SetItemInt(__pyx_t_4, __pyx_t_15, __pyx_t_6, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0) < 0)) __PYX_ERR(0, 195, __pyx_L1_error)
+      if (unlikely(__Pyx_SetItemInt(__pyx_t_4, __pyx_t_15, __pyx_t_6, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0) < 0)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
   }
 
-  /* "pydivsufsort/stringalg.pyx":196
+  /* "pydivsufsort/stringalg.pyx":199
  *         for j in range(m):
  *             temp[i+1][j+1] = min(temp[i][j+1] + 1, temp[i+1][j] + 1, temp[i][j] + (a[i] != b[j]))
  *     return temp[n][m]             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_6 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_n, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 196, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_n, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_6, __pyx_v_m, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 196, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_6, __pyx_v_m, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "pydivsufsort/stringalg.pyx":184
- *     return ans
+  /* "pydivsufsort/stringalg.pyx":187
+ *     return _lcp_query(*segtree, queries)
  * 
  * def _levenshtein(string_t[::1] a not None, string_t[::1] b not None):             # <<<<<<<<<<<<<<
  *     cdef unsigned long long n, m, i, j, d
  *     n = len(a)
  */
 
   /* function exit code */
@@ -23734,17 +23875,17 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_b, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_1__pyx_pw_12pydivsufsort_9stringalg_107_levenshtein(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_1__pyx_mdef_12pydivsufsort_9stringalg_107_levenshtein = {"__pyx_fuse_1_levenshtein", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_1__pyx_pw_12pydivsufsort_9stringalg_107_levenshtein, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_fuse_1__pyx_pw_12pydivsufsort_9stringalg_107_levenshtein(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_1__pyx_pw_12pydivsufsort_9stringalg_109_levenshtein(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_1__pyx_mdef_12pydivsufsort_9stringalg_109_levenshtein = {"__pyx_fuse_1_levenshtein", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_1__pyx_pw_12pydivsufsort_9stringalg_109_levenshtein, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_fuse_1__pyx_pw_12pydivsufsort_9stringalg_109_levenshtein(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_a = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_b = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -23768,55 +23909,55 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_a)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_b)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_levenshtein", 1, 2, 2, 1); __PYX_ERR(0, 184, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_levenshtein", 1, 2, 2, 1); __PYX_ERR(0, 187, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_levenshtein") < 0)) __PYX_ERR(0, 184, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_levenshtein") < 0)) __PYX_ERR(0, 187, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
-    __pyx_v_a = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_uint16_t(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_a.memview)) __PYX_ERR(0, 184, __pyx_L3_error)
-    __pyx_v_b = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_uint16_t(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_b.memview)) __PYX_ERR(0, 184, __pyx_L3_error)
+    __pyx_v_a = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_uint16_t(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_a.memview)) __PYX_ERR(0, 187, __pyx_L3_error)
+    __pyx_v_b = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_uint16_t(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_b.memview)) __PYX_ERR(0, 187, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_levenshtein", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 184, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_levenshtein", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 187, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pydivsufsort.stringalg._levenshtein", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(((PyObject *)__pyx_v_a.memview) == Py_None)) {
-    PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "a"); __PYX_ERR(0, 184, __pyx_L1_error)
+    PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "a"); __PYX_ERR(0, 187, __pyx_L1_error)
   }
   if (unlikely(((PyObject *)__pyx_v_b.memview) == Py_None)) {
-    PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "b"); __PYX_ERR(0, 184, __pyx_L1_error)
+    PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "b"); __PYX_ERR(0, 187, __pyx_L1_error)
   }
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_106_levenshtein(__pyx_self, __pyx_v_a, __pyx_v_b);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_108_levenshtein(__pyx_self, __pyx_v_a, __pyx_v_b);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_106_levenshtein(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_a, __Pyx_memviewslice __pyx_v_b) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_108_levenshtein(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_a, __Pyx_memviewslice __pyx_v_b) {
   unsigned PY_LONG_LONG __pyx_v_n;
   unsigned PY_LONG_LONG __pyx_v_m;
   unsigned PY_LONG_LONG __pyx_v_i;
   unsigned PY_LONG_LONG __pyx_v_j;
   PyArrayObject *__pyx_v_temp = 0;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_temp;
   __Pyx_Buffer __pyx_pybuffer_temp;
@@ -23843,225 +23984,225 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_1_levenshtein", 0);
   __pyx_pybuffer_temp.pybuffer.buf = NULL;
   __pyx_pybuffer_temp.refcount = 0;
   __pyx_pybuffernd_temp.data = NULL;
   __pyx_pybuffernd_temp.rcbuffer = &__pyx_pybuffer_temp;
 
-  /* "pydivsufsort/stringalg.pyx":186
+  /* "pydivsufsort/stringalg.pyx":189
  * def _levenshtein(string_t[::1] a not None, string_t[::1] b not None):
  *     cdef unsigned long long n, m, i, j, d
  *     n = len(a)             # <<<<<<<<<<<<<<
  *     m = len(b)
  *     cdef np.ndarray[np.uint64_t, ndim=2] temp = np.empty((n+1, m+1), dtype=np.uint64)
  */
   __pyx_t_1 = __Pyx_MemoryView_Len(__pyx_v_a); 
   __pyx_v_n = __pyx_t_1;
 
-  /* "pydivsufsort/stringalg.pyx":187
+  /* "pydivsufsort/stringalg.pyx":190
  *     cdef unsigned long long n, m, i, j, d
  *     n = len(a)
  *     m = len(b)             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.uint64_t, ndim=2] temp = np.empty((n+1, m+1), dtype=np.uint64)
  *     for i in range(n):
  */
   __pyx_t_1 = __Pyx_MemoryView_Len(__pyx_v_b); 
   __pyx_v_m = __pyx_t_1;
 
-  /* "pydivsufsort/stringalg.pyx":188
+  /* "pydivsufsort/stringalg.pyx":191
  *     n = len(a)
  *     m = len(b)
  *     cdef np.ndarray[np.uint64_t, ndim=2] temp = np.empty((n+1, m+1), dtype=np.uint64)             # <<<<<<<<<<<<<<
  *     for i in range(n):
  *         temp[i][0] = i
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG((__pyx_v_n + 1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG((__pyx_v_n + 1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG((__pyx_v_m + 1)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG((__pyx_v_m + 1)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_4);
   __pyx_t_2 = 0;
   __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5);
   __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_uint64); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_uint64); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 188, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 188, __pyx_L1_error)
+  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 191, __pyx_L1_error)
   __pyx_t_7 = ((PyArrayObject *)__pyx_t_6);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_temp.rcbuffer->pybuffer, (PyObject*)__pyx_t_7, &__Pyx_TypeInfo_nn___pyx_t_5numpy_uint64_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_temp = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_temp.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 188, __pyx_L1_error)
+      __PYX_ERR(0, 191, __pyx_L1_error)
     } else {__pyx_pybuffernd_temp.diminfo[0].strides = __pyx_pybuffernd_temp.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_temp.diminfo[0].shape = __pyx_pybuffernd_temp.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_temp.diminfo[1].strides = __pyx_pybuffernd_temp.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_temp.diminfo[1].shape = __pyx_pybuffernd_temp.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_t_7 = 0;
   __pyx_v_temp = ((PyArrayObject *)__pyx_t_6);
   __pyx_t_6 = 0;
 
-  /* "pydivsufsort/stringalg.pyx":189
+  /* "pydivsufsort/stringalg.pyx":192
  *     m = len(b)
  *     cdef np.ndarray[np.uint64_t, ndim=2] temp = np.empty((n+1, m+1), dtype=np.uint64)
  *     for i in range(n):             # <<<<<<<<<<<<<<
  *         temp[i][0] = i
  *     for j in range(m):
  */
   __pyx_t_8 = __pyx_v_n;
   __pyx_t_9 = __pyx_t_8;
   for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
     __pyx_v_i = __pyx_t_10;
 
-    /* "pydivsufsort/stringalg.pyx":190
+    /* "pydivsufsort/stringalg.pyx":193
  *     cdef np.ndarray[np.uint64_t, ndim=2] temp = np.empty((n+1, m+1), dtype=np.uint64)
  *     for i in range(n):
  *         temp[i][0] = i             # <<<<<<<<<<<<<<
  *     for j in range(m):
  *         temp[0][j] = j
  */
-    __pyx_t_6 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG(__pyx_v_i); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 190, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG(__pyx_v_i); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 193, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 190, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 193, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (unlikely(__Pyx_SetItemInt(__pyx_t_5, 0, __pyx_t_6, long, 1, __Pyx_PyInt_From_long, 0, 0, 0) < 0)) __PYX_ERR(0, 190, __pyx_L1_error)
+    if (unlikely(__Pyx_SetItemInt(__pyx_t_5, 0, __pyx_t_6, long, 1, __Pyx_PyInt_From_long, 0, 0, 0) < 0)) __PYX_ERR(0, 193, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
 
-  /* "pydivsufsort/stringalg.pyx":191
+  /* "pydivsufsort/stringalg.pyx":194
  *     for i in range(n):
  *         temp[i][0] = i
  *     for j in range(m):             # <<<<<<<<<<<<<<
  *         temp[0][j] = j
  *     for i in range(n):
  */
   __pyx_t_8 = __pyx_v_m;
   __pyx_t_9 = __pyx_t_8;
   for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
     __pyx_v_j = __pyx_t_10;
 
-    /* "pydivsufsort/stringalg.pyx":192
+    /* "pydivsufsort/stringalg.pyx":195
  *         temp[i][0] = i
  *     for j in range(m):
  *         temp[0][j] = j             # <<<<<<<<<<<<<<
  *     for i in range(n):
  *         for j in range(m):
  */
-    __pyx_t_6 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG(__pyx_v_j); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 192, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG(__pyx_v_j); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 195, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 192, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (unlikely(__Pyx_SetItemInt(__pyx_t_5, __pyx_v_j, __pyx_t_6, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0) < 0)) __PYX_ERR(0, 192, __pyx_L1_error)
+    if (unlikely(__Pyx_SetItemInt(__pyx_t_5, __pyx_v_j, __pyx_t_6, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0) < 0)) __PYX_ERR(0, 195, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
 
-  /* "pydivsufsort/stringalg.pyx":193
+  /* "pydivsufsort/stringalg.pyx":196
  *     for j in range(m):
  *         temp[0][j] = j
  *     for i in range(n):             # <<<<<<<<<<<<<<
  *         for j in range(m):
  *             temp[i+1][j+1] = min(temp[i][j+1] + 1, temp[i+1][j] + 1, temp[i][j] + (a[i] != b[j]))
  */
   __pyx_t_8 = __pyx_v_n;
   __pyx_t_9 = __pyx_t_8;
   for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
     __pyx_v_i = __pyx_t_10;
 
-    /* "pydivsufsort/stringalg.pyx":194
+    /* "pydivsufsort/stringalg.pyx":197
  *         temp[0][j] = j
  *     for i in range(n):
  *         for j in range(m):             # <<<<<<<<<<<<<<
  *             temp[i+1][j+1] = min(temp[i][j+1] + 1, temp[i+1][j] + 1, temp[i][j] + (a[i] != b[j]))
  *     return temp[n][m]
  */
     __pyx_t_11 = __pyx_v_m;
     __pyx_t_12 = __pyx_t_11;
     for (__pyx_t_13 = 0; __pyx_t_13 < __pyx_t_12; __pyx_t_13+=1) {
       __pyx_v_j = __pyx_t_13;
 
-      /* "pydivsufsort/stringalg.pyx":195
+      /* "pydivsufsort/stringalg.pyx":198
  *     for i in range(n):
  *         for j in range(m):
  *             temp[i+1][j+1] = min(temp[i][j+1] + 1, temp[i+1][j] + 1, temp[i][j] + (a[i] != b[j]))             # <<<<<<<<<<<<<<
  *     return temp[n][m]
  * 
  */
       __pyx_t_14 = (__pyx_v_i + 1);
-      __pyx_t_6 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_t_14, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_t_14, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_5 = __Pyx_GetItemInt(__pyx_t_6, __pyx_v_j, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_GetItemInt(__pyx_t_6, __pyx_v_j, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __pyx_t_6 = __Pyx_PyInt_AddObjC(__pyx_t_5, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyInt_AddObjC(__pyx_t_5, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_5, __pyx_v_j, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_5, __pyx_v_j, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_t_14 = __pyx_v_i;
       __pyx_t_15 = __pyx_v_j;
-      __pyx_t_5 = __Pyx_PyBool_FromLong(((*((__pyx_t_5numpy_uint16_t *) ( /* dim=0 */ ((char *) (((__pyx_t_5numpy_uint16_t *) __pyx_v_a.data) + __pyx_t_14)) ))) != (*((__pyx_t_5numpy_uint16_t *) ( /* dim=0 */ ((char *) (((__pyx_t_5numpy_uint16_t *) __pyx_v_b.data) + __pyx_t_15)) ))))); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyBool_FromLong(((*((__pyx_t_5numpy_uint16_t *) ( /* dim=0 */ ((char *) (((__pyx_t_5numpy_uint16_t *) __pyx_v_a.data) + __pyx_t_14)) ))) != (*((__pyx_t_5numpy_uint16_t *) ( /* dim=0 */ ((char *) (((__pyx_t_5numpy_uint16_t *) __pyx_v_b.data) + __pyx_t_15)) ))))); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_3 = PyNumber_Add(__pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_3 = PyNumber_Add(__pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __pyx_t_15 = (__pyx_v_j + 1);
-      __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_5, __pyx_t_15, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_5, __pyx_t_15, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_5 = __Pyx_PyInt_AddObjC(__pyx_t_4, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyInt_AddObjC(__pyx_t_4, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_2 = PyObject_RichCompare(__pyx_t_6, __pyx_t_5, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 195, __pyx_L1_error)
-      __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_2 = PyObject_RichCompare(__pyx_t_6, __pyx_t_5, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 198, __pyx_L1_error)
+      __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       if (__pyx_t_16) {
         __Pyx_INCREF(__pyx_t_6);
         __pyx_t_4 = __pyx_t_6;
       } else {
         __Pyx_INCREF(__pyx_t_5);
         __pyx_t_4 = __pyx_t_5;
       }
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_INCREF(__pyx_t_4);
       __pyx_t_5 = __pyx_t_4;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_2 = PyObject_RichCompare(__pyx_t_3, __pyx_t_5, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 195, __pyx_L1_error)
-      __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_2 = PyObject_RichCompare(__pyx_t_3, __pyx_t_5, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 198, __pyx_L1_error)
+      __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       if (__pyx_t_16) {
         __Pyx_INCREF(__pyx_t_3);
         __pyx_t_4 = __pyx_t_3;
       } else {
         __Pyx_INCREF(__pyx_t_5);
         __pyx_t_4 = __pyx_t_5;
@@ -24069,42 +24210,42 @@
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __pyx_t_6 = __pyx_t_4;
       __Pyx_INCREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_t_15 = (__pyx_v_i + 1);
-      __pyx_t_4 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_t_15, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_t_15, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_15 = (__pyx_v_j + 1);
-      if (unlikely(__Pyx_SetItemInt(__pyx_t_4, __pyx_t_15, __pyx_t_6, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0) < 0)) __PYX_ERR(0, 195, __pyx_L1_error)
+      if (unlikely(__Pyx_SetItemInt(__pyx_t_4, __pyx_t_15, __pyx_t_6, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0) < 0)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
   }
 
-  /* "pydivsufsort/stringalg.pyx":196
+  /* "pydivsufsort/stringalg.pyx":199
  *         for j in range(m):
  *             temp[i+1][j+1] = min(temp[i][j+1] + 1, temp[i+1][j] + 1, temp[i][j] + (a[i] != b[j]))
  *     return temp[n][m]             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_6 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_n, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 196, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_n, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_6, __pyx_v_m, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 196, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_6, __pyx_v_m, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "pydivsufsort/stringalg.pyx":184
- *     return ans
+  /* "pydivsufsort/stringalg.pyx":187
+ *     return _lcp_query(*segtree, queries)
  * 
  * def _levenshtein(string_t[::1] a not None, string_t[::1] b not None):             # <<<<<<<<<<<<<<
  *     cdef unsigned long long n, m, i, j, d
  *     n = len(a)
  */
 
   /* function exit code */
@@ -24131,17 +24272,17 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_b, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_2__pyx_pw_12pydivsufsort_9stringalg_109_levenshtein(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_2__pyx_mdef_12pydivsufsort_9stringalg_109_levenshtein = {"__pyx_fuse_2_levenshtein", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_2__pyx_pw_12pydivsufsort_9stringalg_109_levenshtein, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_fuse_2__pyx_pw_12pydivsufsort_9stringalg_109_levenshtein(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_2__pyx_pw_12pydivsufsort_9stringalg_111_levenshtein(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_2__pyx_mdef_12pydivsufsort_9stringalg_111_levenshtein = {"__pyx_fuse_2_levenshtein", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_2__pyx_pw_12pydivsufsort_9stringalg_111_levenshtein, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_fuse_2__pyx_pw_12pydivsufsort_9stringalg_111_levenshtein(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_a = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_b = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -24165,55 +24306,55 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_a)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_b)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_levenshtein", 1, 2, 2, 1); __PYX_ERR(0, 184, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_levenshtein", 1, 2, 2, 1); __PYX_ERR(0, 187, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_levenshtein") < 0)) __PYX_ERR(0, 184, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_levenshtein") < 0)) __PYX_ERR(0, 187, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
-    __pyx_v_a = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_uint32_t(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_a.memview)) __PYX_ERR(0, 184, __pyx_L3_error)
-    __pyx_v_b = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_uint32_t(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_b.memview)) __PYX_ERR(0, 184, __pyx_L3_error)
+    __pyx_v_a = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_uint32_t(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_a.memview)) __PYX_ERR(0, 187, __pyx_L3_error)
+    __pyx_v_b = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_uint32_t(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_b.memview)) __PYX_ERR(0, 187, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_levenshtein", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 184, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_levenshtein", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 187, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pydivsufsort.stringalg._levenshtein", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(((PyObject *)__pyx_v_a.memview) == Py_None)) {
-    PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "a"); __PYX_ERR(0, 184, __pyx_L1_error)
+    PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "a"); __PYX_ERR(0, 187, __pyx_L1_error)
   }
   if (unlikely(((PyObject *)__pyx_v_b.memview) == Py_None)) {
-    PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "b"); __PYX_ERR(0, 184, __pyx_L1_error)
+    PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "b"); __PYX_ERR(0, 187, __pyx_L1_error)
   }
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_108_levenshtein(__pyx_self, __pyx_v_a, __pyx_v_b);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_110_levenshtein(__pyx_self, __pyx_v_a, __pyx_v_b);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_108_levenshtein(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_a, __Pyx_memviewslice __pyx_v_b) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_110_levenshtein(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_a, __Pyx_memviewslice __pyx_v_b) {
   unsigned PY_LONG_LONG __pyx_v_n;
   unsigned PY_LONG_LONG __pyx_v_m;
   unsigned PY_LONG_LONG __pyx_v_i;
   unsigned PY_LONG_LONG __pyx_v_j;
   PyArrayObject *__pyx_v_temp = 0;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_temp;
   __Pyx_Buffer __pyx_pybuffer_temp;
@@ -24240,225 +24381,225 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_2_levenshtein", 0);
   __pyx_pybuffer_temp.pybuffer.buf = NULL;
   __pyx_pybuffer_temp.refcount = 0;
   __pyx_pybuffernd_temp.data = NULL;
   __pyx_pybuffernd_temp.rcbuffer = &__pyx_pybuffer_temp;
 
-  /* "pydivsufsort/stringalg.pyx":186
+  /* "pydivsufsort/stringalg.pyx":189
  * def _levenshtein(string_t[::1] a not None, string_t[::1] b not None):
  *     cdef unsigned long long n, m, i, j, d
  *     n = len(a)             # <<<<<<<<<<<<<<
  *     m = len(b)
  *     cdef np.ndarray[np.uint64_t, ndim=2] temp = np.empty((n+1, m+1), dtype=np.uint64)
  */
   __pyx_t_1 = __Pyx_MemoryView_Len(__pyx_v_a); 
   __pyx_v_n = __pyx_t_1;
 
-  /* "pydivsufsort/stringalg.pyx":187
+  /* "pydivsufsort/stringalg.pyx":190
  *     cdef unsigned long long n, m, i, j, d
  *     n = len(a)
  *     m = len(b)             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.uint64_t, ndim=2] temp = np.empty((n+1, m+1), dtype=np.uint64)
  *     for i in range(n):
  */
   __pyx_t_1 = __Pyx_MemoryView_Len(__pyx_v_b); 
   __pyx_v_m = __pyx_t_1;
 
-  /* "pydivsufsort/stringalg.pyx":188
+  /* "pydivsufsort/stringalg.pyx":191
  *     n = len(a)
  *     m = len(b)
  *     cdef np.ndarray[np.uint64_t, ndim=2] temp = np.empty((n+1, m+1), dtype=np.uint64)             # <<<<<<<<<<<<<<
  *     for i in range(n):
  *         temp[i][0] = i
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG((__pyx_v_n + 1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG((__pyx_v_n + 1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG((__pyx_v_m + 1)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG((__pyx_v_m + 1)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_4);
   __pyx_t_2 = 0;
   __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5);
   __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_uint64); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_uint64); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 188, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 188, __pyx_L1_error)
+  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 191, __pyx_L1_error)
   __pyx_t_7 = ((PyArrayObject *)__pyx_t_6);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_temp.rcbuffer->pybuffer, (PyObject*)__pyx_t_7, &__Pyx_TypeInfo_nn___pyx_t_5numpy_uint64_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_temp = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_temp.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 188, __pyx_L1_error)
+      __PYX_ERR(0, 191, __pyx_L1_error)
     } else {__pyx_pybuffernd_temp.diminfo[0].strides = __pyx_pybuffernd_temp.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_temp.diminfo[0].shape = __pyx_pybuffernd_temp.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_temp.diminfo[1].strides = __pyx_pybuffernd_temp.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_temp.diminfo[1].shape = __pyx_pybuffernd_temp.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_t_7 = 0;
   __pyx_v_temp = ((PyArrayObject *)__pyx_t_6);
   __pyx_t_6 = 0;
 
-  /* "pydivsufsort/stringalg.pyx":189
+  /* "pydivsufsort/stringalg.pyx":192
  *     m = len(b)
  *     cdef np.ndarray[np.uint64_t, ndim=2] temp = np.empty((n+1, m+1), dtype=np.uint64)
  *     for i in range(n):             # <<<<<<<<<<<<<<
  *         temp[i][0] = i
  *     for j in range(m):
  */
   __pyx_t_8 = __pyx_v_n;
   __pyx_t_9 = __pyx_t_8;
   for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
     __pyx_v_i = __pyx_t_10;
 
-    /* "pydivsufsort/stringalg.pyx":190
+    /* "pydivsufsort/stringalg.pyx":193
  *     cdef np.ndarray[np.uint64_t, ndim=2] temp = np.empty((n+1, m+1), dtype=np.uint64)
  *     for i in range(n):
  *         temp[i][0] = i             # <<<<<<<<<<<<<<
  *     for j in range(m):
  *         temp[0][j] = j
  */
-    __pyx_t_6 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG(__pyx_v_i); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 190, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG(__pyx_v_i); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 193, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 190, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 193, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (unlikely(__Pyx_SetItemInt(__pyx_t_5, 0, __pyx_t_6, long, 1, __Pyx_PyInt_From_long, 0, 0, 0) < 0)) __PYX_ERR(0, 190, __pyx_L1_error)
+    if (unlikely(__Pyx_SetItemInt(__pyx_t_5, 0, __pyx_t_6, long, 1, __Pyx_PyInt_From_long, 0, 0, 0) < 0)) __PYX_ERR(0, 193, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
 
-  /* "pydivsufsort/stringalg.pyx":191
+  /* "pydivsufsort/stringalg.pyx":194
  *     for i in range(n):
  *         temp[i][0] = i
  *     for j in range(m):             # <<<<<<<<<<<<<<
  *         temp[0][j] = j
  *     for i in range(n):
  */
   __pyx_t_8 = __pyx_v_m;
   __pyx_t_9 = __pyx_t_8;
   for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
     __pyx_v_j = __pyx_t_10;
 
-    /* "pydivsufsort/stringalg.pyx":192
+    /* "pydivsufsort/stringalg.pyx":195
  *         temp[i][0] = i
  *     for j in range(m):
  *         temp[0][j] = j             # <<<<<<<<<<<<<<
  *     for i in range(n):
  *         for j in range(m):
  */
-    __pyx_t_6 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG(__pyx_v_j); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 192, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG(__pyx_v_j); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 195, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 192, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (unlikely(__Pyx_SetItemInt(__pyx_t_5, __pyx_v_j, __pyx_t_6, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0) < 0)) __PYX_ERR(0, 192, __pyx_L1_error)
+    if (unlikely(__Pyx_SetItemInt(__pyx_t_5, __pyx_v_j, __pyx_t_6, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0) < 0)) __PYX_ERR(0, 195, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
 
-  /* "pydivsufsort/stringalg.pyx":193
+  /* "pydivsufsort/stringalg.pyx":196
  *     for j in range(m):
  *         temp[0][j] = j
  *     for i in range(n):             # <<<<<<<<<<<<<<
  *         for j in range(m):
  *             temp[i+1][j+1] = min(temp[i][j+1] + 1, temp[i+1][j] + 1, temp[i][j] + (a[i] != b[j]))
  */
   __pyx_t_8 = __pyx_v_n;
   __pyx_t_9 = __pyx_t_8;
   for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
     __pyx_v_i = __pyx_t_10;
 
-    /* "pydivsufsort/stringalg.pyx":194
+    /* "pydivsufsort/stringalg.pyx":197
  *         temp[0][j] = j
  *     for i in range(n):
  *         for j in range(m):             # <<<<<<<<<<<<<<
  *             temp[i+1][j+1] = min(temp[i][j+1] + 1, temp[i+1][j] + 1, temp[i][j] + (a[i] != b[j]))
  *     return temp[n][m]
  */
     __pyx_t_11 = __pyx_v_m;
     __pyx_t_12 = __pyx_t_11;
     for (__pyx_t_13 = 0; __pyx_t_13 < __pyx_t_12; __pyx_t_13+=1) {
       __pyx_v_j = __pyx_t_13;
 
-      /* "pydivsufsort/stringalg.pyx":195
+      /* "pydivsufsort/stringalg.pyx":198
  *     for i in range(n):
  *         for j in range(m):
  *             temp[i+1][j+1] = min(temp[i][j+1] + 1, temp[i+1][j] + 1, temp[i][j] + (a[i] != b[j]))             # <<<<<<<<<<<<<<
  *     return temp[n][m]
  * 
  */
       __pyx_t_14 = (__pyx_v_i + 1);
-      __pyx_t_6 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_t_14, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_t_14, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_5 = __Pyx_GetItemInt(__pyx_t_6, __pyx_v_j, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_GetItemInt(__pyx_t_6, __pyx_v_j, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __pyx_t_6 = __Pyx_PyInt_AddObjC(__pyx_t_5, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyInt_AddObjC(__pyx_t_5, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_5, __pyx_v_j, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_5, __pyx_v_j, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_t_14 = __pyx_v_i;
       __pyx_t_15 = __pyx_v_j;
-      __pyx_t_5 = __Pyx_PyBool_FromLong(((*((__pyx_t_5numpy_uint32_t *) ( /* dim=0 */ ((char *) (((__pyx_t_5numpy_uint32_t *) __pyx_v_a.data) + __pyx_t_14)) ))) != (*((__pyx_t_5numpy_uint32_t *) ( /* dim=0 */ ((char *) (((__pyx_t_5numpy_uint32_t *) __pyx_v_b.data) + __pyx_t_15)) ))))); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyBool_FromLong(((*((__pyx_t_5numpy_uint32_t *) ( /* dim=0 */ ((char *) (((__pyx_t_5numpy_uint32_t *) __pyx_v_a.data) + __pyx_t_14)) ))) != (*((__pyx_t_5numpy_uint32_t *) ( /* dim=0 */ ((char *) (((__pyx_t_5numpy_uint32_t *) __pyx_v_b.data) + __pyx_t_15)) ))))); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_3 = PyNumber_Add(__pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_3 = PyNumber_Add(__pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __pyx_t_15 = (__pyx_v_j + 1);
-      __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_5, __pyx_t_15, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_5, __pyx_t_15, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_5 = __Pyx_PyInt_AddObjC(__pyx_t_4, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyInt_AddObjC(__pyx_t_4, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_2 = PyObject_RichCompare(__pyx_t_6, __pyx_t_5, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 195, __pyx_L1_error)
-      __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_2 = PyObject_RichCompare(__pyx_t_6, __pyx_t_5, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 198, __pyx_L1_error)
+      __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       if (__pyx_t_16) {
         __Pyx_INCREF(__pyx_t_6);
         __pyx_t_4 = __pyx_t_6;
       } else {
         __Pyx_INCREF(__pyx_t_5);
         __pyx_t_4 = __pyx_t_5;
       }
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_INCREF(__pyx_t_4);
       __pyx_t_5 = __pyx_t_4;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_2 = PyObject_RichCompare(__pyx_t_3, __pyx_t_5, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 195, __pyx_L1_error)
-      __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_2 = PyObject_RichCompare(__pyx_t_3, __pyx_t_5, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 198, __pyx_L1_error)
+      __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       if (__pyx_t_16) {
         __Pyx_INCREF(__pyx_t_3);
         __pyx_t_4 = __pyx_t_3;
       } else {
         __Pyx_INCREF(__pyx_t_5);
         __pyx_t_4 = __pyx_t_5;
@@ -24466,42 +24607,42 @@
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __pyx_t_6 = __pyx_t_4;
       __Pyx_INCREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_t_15 = (__pyx_v_i + 1);
-      __pyx_t_4 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_t_15, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_t_15, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_15 = (__pyx_v_j + 1);
-      if (unlikely(__Pyx_SetItemInt(__pyx_t_4, __pyx_t_15, __pyx_t_6, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0) < 0)) __PYX_ERR(0, 195, __pyx_L1_error)
+      if (unlikely(__Pyx_SetItemInt(__pyx_t_4, __pyx_t_15, __pyx_t_6, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0) < 0)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
   }
 
-  /* "pydivsufsort/stringalg.pyx":196
+  /* "pydivsufsort/stringalg.pyx":199
  *         for j in range(m):
  *             temp[i+1][j+1] = min(temp[i][j+1] + 1, temp[i+1][j] + 1, temp[i][j] + (a[i] != b[j]))
  *     return temp[n][m]             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_6 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_n, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 196, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_n, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_6, __pyx_v_m, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 196, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_6, __pyx_v_m, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "pydivsufsort/stringalg.pyx":184
- *     return ans
+  /* "pydivsufsort/stringalg.pyx":187
+ *     return _lcp_query(*segtree, queries)
  * 
  * def _levenshtein(string_t[::1] a not None, string_t[::1] b not None):             # <<<<<<<<<<<<<<
  *     cdef unsigned long long n, m, i, j, d
  *     n = len(a)
  */
 
   /* function exit code */
@@ -24528,17 +24669,17 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_b, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_3__pyx_pw_12pydivsufsort_9stringalg_111_levenshtein(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_3__pyx_mdef_12pydivsufsort_9stringalg_111_levenshtein = {"__pyx_fuse_3_levenshtein", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_3__pyx_pw_12pydivsufsort_9stringalg_111_levenshtein, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_fuse_3__pyx_pw_12pydivsufsort_9stringalg_111_levenshtein(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_3__pyx_pw_12pydivsufsort_9stringalg_113_levenshtein(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_3__pyx_mdef_12pydivsufsort_9stringalg_113_levenshtein = {"__pyx_fuse_3_levenshtein", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_3__pyx_pw_12pydivsufsort_9stringalg_113_levenshtein, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_fuse_3__pyx_pw_12pydivsufsort_9stringalg_113_levenshtein(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_a = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_b = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -24562,55 +24703,55 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_a)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_b)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_levenshtein", 1, 2, 2, 1); __PYX_ERR(0, 184, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_levenshtein", 1, 2, 2, 1); __PYX_ERR(0, 187, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_levenshtein") < 0)) __PYX_ERR(0, 184, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_levenshtein") < 0)) __PYX_ERR(0, 187, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
-    __pyx_v_a = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_uint64_t(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_a.memview)) __PYX_ERR(0, 184, __pyx_L3_error)
-    __pyx_v_b = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_uint64_t(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_b.memview)) __PYX_ERR(0, 184, __pyx_L3_error)
+    __pyx_v_a = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_uint64_t(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_a.memview)) __PYX_ERR(0, 187, __pyx_L3_error)
+    __pyx_v_b = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_uint64_t(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_b.memview)) __PYX_ERR(0, 187, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_levenshtein", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 184, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_levenshtein", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 187, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pydivsufsort.stringalg._levenshtein", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(((PyObject *)__pyx_v_a.memview) == Py_None)) {
-    PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "a"); __PYX_ERR(0, 184, __pyx_L1_error)
+    PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "a"); __PYX_ERR(0, 187, __pyx_L1_error)
   }
   if (unlikely(((PyObject *)__pyx_v_b.memview) == Py_None)) {
-    PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "b"); __PYX_ERR(0, 184, __pyx_L1_error)
+    PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "b"); __PYX_ERR(0, 187, __pyx_L1_error)
   }
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_110_levenshtein(__pyx_self, __pyx_v_a, __pyx_v_b);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_112_levenshtein(__pyx_self, __pyx_v_a, __pyx_v_b);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_110_levenshtein(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_a, __Pyx_memviewslice __pyx_v_b) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_112_levenshtein(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_a, __Pyx_memviewslice __pyx_v_b) {
   unsigned PY_LONG_LONG __pyx_v_n;
   unsigned PY_LONG_LONG __pyx_v_m;
   unsigned PY_LONG_LONG __pyx_v_i;
   unsigned PY_LONG_LONG __pyx_v_j;
   PyArrayObject *__pyx_v_temp = 0;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_temp;
   __Pyx_Buffer __pyx_pybuffer_temp;
@@ -24637,225 +24778,225 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_3_levenshtein", 0);
   __pyx_pybuffer_temp.pybuffer.buf = NULL;
   __pyx_pybuffer_temp.refcount = 0;
   __pyx_pybuffernd_temp.data = NULL;
   __pyx_pybuffernd_temp.rcbuffer = &__pyx_pybuffer_temp;
 
-  /* "pydivsufsort/stringalg.pyx":186
+  /* "pydivsufsort/stringalg.pyx":189
  * def _levenshtein(string_t[::1] a not None, string_t[::1] b not None):
  *     cdef unsigned long long n, m, i, j, d
  *     n = len(a)             # <<<<<<<<<<<<<<
  *     m = len(b)
  *     cdef np.ndarray[np.uint64_t, ndim=2] temp = np.empty((n+1, m+1), dtype=np.uint64)
  */
   __pyx_t_1 = __Pyx_MemoryView_Len(__pyx_v_a); 
   __pyx_v_n = __pyx_t_1;
 
-  /* "pydivsufsort/stringalg.pyx":187
+  /* "pydivsufsort/stringalg.pyx":190
  *     cdef unsigned long long n, m, i, j, d
  *     n = len(a)
  *     m = len(b)             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.uint64_t, ndim=2] temp = np.empty((n+1, m+1), dtype=np.uint64)
  *     for i in range(n):
  */
   __pyx_t_1 = __Pyx_MemoryView_Len(__pyx_v_b); 
   __pyx_v_m = __pyx_t_1;
 
-  /* "pydivsufsort/stringalg.pyx":188
+  /* "pydivsufsort/stringalg.pyx":191
  *     n = len(a)
  *     m = len(b)
  *     cdef np.ndarray[np.uint64_t, ndim=2] temp = np.empty((n+1, m+1), dtype=np.uint64)             # <<<<<<<<<<<<<<
  *     for i in range(n):
  *         temp[i][0] = i
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG((__pyx_v_n + 1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG((__pyx_v_n + 1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG((__pyx_v_m + 1)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG((__pyx_v_m + 1)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_4);
   __pyx_t_2 = 0;
   __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5);
   __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_uint64); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_uint64); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 188, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 188, __pyx_L1_error)
+  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 191, __pyx_L1_error)
   __pyx_t_7 = ((PyArrayObject *)__pyx_t_6);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_temp.rcbuffer->pybuffer, (PyObject*)__pyx_t_7, &__Pyx_TypeInfo_nn___pyx_t_5numpy_uint64_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_temp = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_temp.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 188, __pyx_L1_error)
+      __PYX_ERR(0, 191, __pyx_L1_error)
     } else {__pyx_pybuffernd_temp.diminfo[0].strides = __pyx_pybuffernd_temp.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_temp.diminfo[0].shape = __pyx_pybuffernd_temp.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_temp.diminfo[1].strides = __pyx_pybuffernd_temp.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_temp.diminfo[1].shape = __pyx_pybuffernd_temp.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_t_7 = 0;
   __pyx_v_temp = ((PyArrayObject *)__pyx_t_6);
   __pyx_t_6 = 0;
 
-  /* "pydivsufsort/stringalg.pyx":189
+  /* "pydivsufsort/stringalg.pyx":192
  *     m = len(b)
  *     cdef np.ndarray[np.uint64_t, ndim=2] temp = np.empty((n+1, m+1), dtype=np.uint64)
  *     for i in range(n):             # <<<<<<<<<<<<<<
  *         temp[i][0] = i
  *     for j in range(m):
  */
   __pyx_t_8 = __pyx_v_n;
   __pyx_t_9 = __pyx_t_8;
   for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
     __pyx_v_i = __pyx_t_10;
 
-    /* "pydivsufsort/stringalg.pyx":190
+    /* "pydivsufsort/stringalg.pyx":193
  *     cdef np.ndarray[np.uint64_t, ndim=2] temp = np.empty((n+1, m+1), dtype=np.uint64)
  *     for i in range(n):
  *         temp[i][0] = i             # <<<<<<<<<<<<<<
  *     for j in range(m):
  *         temp[0][j] = j
  */
-    __pyx_t_6 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG(__pyx_v_i); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 190, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG(__pyx_v_i); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 193, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 190, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 193, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (unlikely(__Pyx_SetItemInt(__pyx_t_5, 0, __pyx_t_6, long, 1, __Pyx_PyInt_From_long, 0, 0, 0) < 0)) __PYX_ERR(0, 190, __pyx_L1_error)
+    if (unlikely(__Pyx_SetItemInt(__pyx_t_5, 0, __pyx_t_6, long, 1, __Pyx_PyInt_From_long, 0, 0, 0) < 0)) __PYX_ERR(0, 193, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
 
-  /* "pydivsufsort/stringalg.pyx":191
+  /* "pydivsufsort/stringalg.pyx":194
  *     for i in range(n):
  *         temp[i][0] = i
  *     for j in range(m):             # <<<<<<<<<<<<<<
  *         temp[0][j] = j
  *     for i in range(n):
  */
   __pyx_t_8 = __pyx_v_m;
   __pyx_t_9 = __pyx_t_8;
   for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
     __pyx_v_j = __pyx_t_10;
 
-    /* "pydivsufsort/stringalg.pyx":192
+    /* "pydivsufsort/stringalg.pyx":195
  *         temp[i][0] = i
  *     for j in range(m):
  *         temp[0][j] = j             # <<<<<<<<<<<<<<
  *     for i in range(n):
  *         for j in range(m):
  */
-    __pyx_t_6 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG(__pyx_v_j); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 192, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG(__pyx_v_j); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 195, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 192, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (unlikely(__Pyx_SetItemInt(__pyx_t_5, __pyx_v_j, __pyx_t_6, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0) < 0)) __PYX_ERR(0, 192, __pyx_L1_error)
+    if (unlikely(__Pyx_SetItemInt(__pyx_t_5, __pyx_v_j, __pyx_t_6, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0) < 0)) __PYX_ERR(0, 195, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
 
-  /* "pydivsufsort/stringalg.pyx":193
+  /* "pydivsufsort/stringalg.pyx":196
  *     for j in range(m):
  *         temp[0][j] = j
  *     for i in range(n):             # <<<<<<<<<<<<<<
  *         for j in range(m):
  *             temp[i+1][j+1] = min(temp[i][j+1] + 1, temp[i+1][j] + 1, temp[i][j] + (a[i] != b[j]))
  */
   __pyx_t_8 = __pyx_v_n;
   __pyx_t_9 = __pyx_t_8;
   for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
     __pyx_v_i = __pyx_t_10;
 
-    /* "pydivsufsort/stringalg.pyx":194
+    /* "pydivsufsort/stringalg.pyx":197
  *         temp[0][j] = j
  *     for i in range(n):
  *         for j in range(m):             # <<<<<<<<<<<<<<
  *             temp[i+1][j+1] = min(temp[i][j+1] + 1, temp[i+1][j] + 1, temp[i][j] + (a[i] != b[j]))
  *     return temp[n][m]
  */
     __pyx_t_11 = __pyx_v_m;
     __pyx_t_12 = __pyx_t_11;
     for (__pyx_t_13 = 0; __pyx_t_13 < __pyx_t_12; __pyx_t_13+=1) {
       __pyx_v_j = __pyx_t_13;
 
-      /* "pydivsufsort/stringalg.pyx":195
+      /* "pydivsufsort/stringalg.pyx":198
  *     for i in range(n):
  *         for j in range(m):
  *             temp[i+1][j+1] = min(temp[i][j+1] + 1, temp[i+1][j] + 1, temp[i][j] + (a[i] != b[j]))             # <<<<<<<<<<<<<<
  *     return temp[n][m]
  * 
  */
       __pyx_t_14 = (__pyx_v_i + 1);
-      __pyx_t_6 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_t_14, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_t_14, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_5 = __Pyx_GetItemInt(__pyx_t_6, __pyx_v_j, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_GetItemInt(__pyx_t_6, __pyx_v_j, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __pyx_t_6 = __Pyx_PyInt_AddObjC(__pyx_t_5, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyInt_AddObjC(__pyx_t_5, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_5, __pyx_v_j, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_5, __pyx_v_j, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_t_14 = __pyx_v_i;
       __pyx_t_15 = __pyx_v_j;
-      __pyx_t_5 = __Pyx_PyBool_FromLong(((*((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ ((char *) (((__pyx_t_5numpy_uint64_t *) __pyx_v_a.data) + __pyx_t_14)) ))) != (*((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ ((char *) (((__pyx_t_5numpy_uint64_t *) __pyx_v_b.data) + __pyx_t_15)) ))))); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyBool_FromLong(((*((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ ((char *) (((__pyx_t_5numpy_uint64_t *) __pyx_v_a.data) + __pyx_t_14)) ))) != (*((__pyx_t_5numpy_uint64_t *) ( /* dim=0 */ ((char *) (((__pyx_t_5numpy_uint64_t *) __pyx_v_b.data) + __pyx_t_15)) ))))); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_3 = PyNumber_Add(__pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_3 = PyNumber_Add(__pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __pyx_t_15 = (__pyx_v_j + 1);
-      __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_5, __pyx_t_15, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_5, __pyx_t_15, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_5 = __Pyx_PyInt_AddObjC(__pyx_t_4, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyInt_AddObjC(__pyx_t_4, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_2 = PyObject_RichCompare(__pyx_t_6, __pyx_t_5, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 195, __pyx_L1_error)
-      __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_2 = PyObject_RichCompare(__pyx_t_6, __pyx_t_5, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 198, __pyx_L1_error)
+      __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       if (__pyx_t_16) {
         __Pyx_INCREF(__pyx_t_6);
         __pyx_t_4 = __pyx_t_6;
       } else {
         __Pyx_INCREF(__pyx_t_5);
         __pyx_t_4 = __pyx_t_5;
       }
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_INCREF(__pyx_t_4);
       __pyx_t_5 = __pyx_t_4;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_2 = PyObject_RichCompare(__pyx_t_3, __pyx_t_5, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 195, __pyx_L1_error)
-      __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_2 = PyObject_RichCompare(__pyx_t_3, __pyx_t_5, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 198, __pyx_L1_error)
+      __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       if (__pyx_t_16) {
         __Pyx_INCREF(__pyx_t_3);
         __pyx_t_4 = __pyx_t_3;
       } else {
         __Pyx_INCREF(__pyx_t_5);
         __pyx_t_4 = __pyx_t_5;
@@ -24863,42 +25004,42 @@
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __pyx_t_6 = __pyx_t_4;
       __Pyx_INCREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_t_15 = (__pyx_v_i + 1);
-      __pyx_t_4 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_t_15, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_t_15, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_15 = (__pyx_v_j + 1);
-      if (unlikely(__Pyx_SetItemInt(__pyx_t_4, __pyx_t_15, __pyx_t_6, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0) < 0)) __PYX_ERR(0, 195, __pyx_L1_error)
+      if (unlikely(__Pyx_SetItemInt(__pyx_t_4, __pyx_t_15, __pyx_t_6, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0) < 0)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
   }
 
-  /* "pydivsufsort/stringalg.pyx":196
+  /* "pydivsufsort/stringalg.pyx":199
  *         for j in range(m):
  *             temp[i+1][j+1] = min(temp[i][j+1] + 1, temp[i+1][j] + 1, temp[i][j] + (a[i] != b[j]))
  *     return temp[n][m]             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_6 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_n, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 196, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_n, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_6, __pyx_v_m, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 196, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_6, __pyx_v_m, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "pydivsufsort/stringalg.pyx":184
- *     return ans
+  /* "pydivsufsort/stringalg.pyx":187
+ *     return _lcp_query(*segtree, queries)
  * 
  * def _levenshtein(string_t[::1] a not None, string_t[::1] b not None):             # <<<<<<<<<<<<<<
  *     cdef unsigned long long n, m, i, j, d
  *     n = len(a)
  */
 
   /* function exit code */
@@ -24925,17 +25066,17 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_b, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_4__pyx_pw_12pydivsufsort_9stringalg_113_levenshtein(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_4__pyx_mdef_12pydivsufsort_9stringalg_113_levenshtein = {"__pyx_fuse_4_levenshtein", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_4__pyx_pw_12pydivsufsort_9stringalg_113_levenshtein, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_fuse_4__pyx_pw_12pydivsufsort_9stringalg_113_levenshtein(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_4__pyx_pw_12pydivsufsort_9stringalg_115_levenshtein(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_4__pyx_mdef_12pydivsufsort_9stringalg_115_levenshtein = {"__pyx_fuse_4_levenshtein", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_4__pyx_pw_12pydivsufsort_9stringalg_115_levenshtein, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_fuse_4__pyx_pw_12pydivsufsort_9stringalg_115_levenshtein(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_a = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_b = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -24959,55 +25100,55 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_a)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_b)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_levenshtein", 1, 2, 2, 1); __PYX_ERR(0, 184, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_levenshtein", 1, 2, 2, 1); __PYX_ERR(0, 187, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_levenshtein") < 0)) __PYX_ERR(0, 184, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_levenshtein") < 0)) __PYX_ERR(0, 187, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
-    __pyx_v_a = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_int8_t(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_a.memview)) __PYX_ERR(0, 184, __pyx_L3_error)
-    __pyx_v_b = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_int8_t(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_b.memview)) __PYX_ERR(0, 184, __pyx_L3_error)
+    __pyx_v_a = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_int8_t(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_a.memview)) __PYX_ERR(0, 187, __pyx_L3_error)
+    __pyx_v_b = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_int8_t(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_b.memview)) __PYX_ERR(0, 187, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_levenshtein", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 184, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_levenshtein", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 187, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pydivsufsort.stringalg._levenshtein", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(((PyObject *)__pyx_v_a.memview) == Py_None)) {
-    PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "a"); __PYX_ERR(0, 184, __pyx_L1_error)
+    PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "a"); __PYX_ERR(0, 187, __pyx_L1_error)
   }
   if (unlikely(((PyObject *)__pyx_v_b.memview) == Py_None)) {
-    PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "b"); __PYX_ERR(0, 184, __pyx_L1_error)
+    PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "b"); __PYX_ERR(0, 187, __pyx_L1_error)
   }
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_112_levenshtein(__pyx_self, __pyx_v_a, __pyx_v_b);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_114_levenshtein(__pyx_self, __pyx_v_a, __pyx_v_b);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_112_levenshtein(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_a, __Pyx_memviewslice __pyx_v_b) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_114_levenshtein(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_a, __Pyx_memviewslice __pyx_v_b) {
   unsigned PY_LONG_LONG __pyx_v_n;
   unsigned PY_LONG_LONG __pyx_v_m;
   unsigned PY_LONG_LONG __pyx_v_i;
   unsigned PY_LONG_LONG __pyx_v_j;
   PyArrayObject *__pyx_v_temp = 0;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_temp;
   __Pyx_Buffer __pyx_pybuffer_temp;
@@ -25034,225 +25175,225 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_4_levenshtein", 0);
   __pyx_pybuffer_temp.pybuffer.buf = NULL;
   __pyx_pybuffer_temp.refcount = 0;
   __pyx_pybuffernd_temp.data = NULL;
   __pyx_pybuffernd_temp.rcbuffer = &__pyx_pybuffer_temp;
 
-  /* "pydivsufsort/stringalg.pyx":186
+  /* "pydivsufsort/stringalg.pyx":189
  * def _levenshtein(string_t[::1] a not None, string_t[::1] b not None):
  *     cdef unsigned long long n, m, i, j, d
  *     n = len(a)             # <<<<<<<<<<<<<<
  *     m = len(b)
  *     cdef np.ndarray[np.uint64_t, ndim=2] temp = np.empty((n+1, m+1), dtype=np.uint64)
  */
   __pyx_t_1 = __Pyx_MemoryView_Len(__pyx_v_a); 
   __pyx_v_n = __pyx_t_1;
 
-  /* "pydivsufsort/stringalg.pyx":187
+  /* "pydivsufsort/stringalg.pyx":190
  *     cdef unsigned long long n, m, i, j, d
  *     n = len(a)
  *     m = len(b)             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.uint64_t, ndim=2] temp = np.empty((n+1, m+1), dtype=np.uint64)
  *     for i in range(n):
  */
   __pyx_t_1 = __Pyx_MemoryView_Len(__pyx_v_b); 
   __pyx_v_m = __pyx_t_1;
 
-  /* "pydivsufsort/stringalg.pyx":188
+  /* "pydivsufsort/stringalg.pyx":191
  *     n = len(a)
  *     m = len(b)
  *     cdef np.ndarray[np.uint64_t, ndim=2] temp = np.empty((n+1, m+1), dtype=np.uint64)             # <<<<<<<<<<<<<<
  *     for i in range(n):
  *         temp[i][0] = i
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG((__pyx_v_n + 1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG((__pyx_v_n + 1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG((__pyx_v_m + 1)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG((__pyx_v_m + 1)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_4);
   __pyx_t_2 = 0;
   __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5);
   __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_uint64); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_uint64); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 188, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 188, __pyx_L1_error)
+  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 191, __pyx_L1_error)
   __pyx_t_7 = ((PyArrayObject *)__pyx_t_6);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_temp.rcbuffer->pybuffer, (PyObject*)__pyx_t_7, &__Pyx_TypeInfo_nn___pyx_t_5numpy_uint64_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_temp = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_temp.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 188, __pyx_L1_error)
+      __PYX_ERR(0, 191, __pyx_L1_error)
     } else {__pyx_pybuffernd_temp.diminfo[0].strides = __pyx_pybuffernd_temp.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_temp.diminfo[0].shape = __pyx_pybuffernd_temp.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_temp.diminfo[1].strides = __pyx_pybuffernd_temp.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_temp.diminfo[1].shape = __pyx_pybuffernd_temp.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_t_7 = 0;
   __pyx_v_temp = ((PyArrayObject *)__pyx_t_6);
   __pyx_t_6 = 0;
 
-  /* "pydivsufsort/stringalg.pyx":189
+  /* "pydivsufsort/stringalg.pyx":192
  *     m = len(b)
  *     cdef np.ndarray[np.uint64_t, ndim=2] temp = np.empty((n+1, m+1), dtype=np.uint64)
  *     for i in range(n):             # <<<<<<<<<<<<<<
  *         temp[i][0] = i
  *     for j in range(m):
  */
   __pyx_t_8 = __pyx_v_n;
   __pyx_t_9 = __pyx_t_8;
   for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
     __pyx_v_i = __pyx_t_10;
 
-    /* "pydivsufsort/stringalg.pyx":190
+    /* "pydivsufsort/stringalg.pyx":193
  *     cdef np.ndarray[np.uint64_t, ndim=2] temp = np.empty((n+1, m+1), dtype=np.uint64)
  *     for i in range(n):
  *         temp[i][0] = i             # <<<<<<<<<<<<<<
  *     for j in range(m):
  *         temp[0][j] = j
  */
-    __pyx_t_6 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG(__pyx_v_i); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 190, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG(__pyx_v_i); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 193, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 190, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 193, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (unlikely(__Pyx_SetItemInt(__pyx_t_5, 0, __pyx_t_6, long, 1, __Pyx_PyInt_From_long, 0, 0, 0) < 0)) __PYX_ERR(0, 190, __pyx_L1_error)
+    if (unlikely(__Pyx_SetItemInt(__pyx_t_5, 0, __pyx_t_6, long, 1, __Pyx_PyInt_From_long, 0, 0, 0) < 0)) __PYX_ERR(0, 193, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
 
-  /* "pydivsufsort/stringalg.pyx":191
+  /* "pydivsufsort/stringalg.pyx":194
  *     for i in range(n):
  *         temp[i][0] = i
  *     for j in range(m):             # <<<<<<<<<<<<<<
  *         temp[0][j] = j
  *     for i in range(n):
  */
   __pyx_t_8 = __pyx_v_m;
   __pyx_t_9 = __pyx_t_8;
   for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
     __pyx_v_j = __pyx_t_10;
 
-    /* "pydivsufsort/stringalg.pyx":192
+    /* "pydivsufsort/stringalg.pyx":195
  *         temp[i][0] = i
  *     for j in range(m):
  *         temp[0][j] = j             # <<<<<<<<<<<<<<
  *     for i in range(n):
  *         for j in range(m):
  */
-    __pyx_t_6 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG(__pyx_v_j); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 192, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG(__pyx_v_j); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 195, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 192, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (unlikely(__Pyx_SetItemInt(__pyx_t_5, __pyx_v_j, __pyx_t_6, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0) < 0)) __PYX_ERR(0, 192, __pyx_L1_error)
+    if (unlikely(__Pyx_SetItemInt(__pyx_t_5, __pyx_v_j, __pyx_t_6, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0) < 0)) __PYX_ERR(0, 195, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
 
-  /* "pydivsufsort/stringalg.pyx":193
+  /* "pydivsufsort/stringalg.pyx":196
  *     for j in range(m):
  *         temp[0][j] = j
  *     for i in range(n):             # <<<<<<<<<<<<<<
  *         for j in range(m):
  *             temp[i+1][j+1] = min(temp[i][j+1] + 1, temp[i+1][j] + 1, temp[i][j] + (a[i] != b[j]))
  */
   __pyx_t_8 = __pyx_v_n;
   __pyx_t_9 = __pyx_t_8;
   for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
     __pyx_v_i = __pyx_t_10;
 
-    /* "pydivsufsort/stringalg.pyx":194
+    /* "pydivsufsort/stringalg.pyx":197
  *         temp[0][j] = j
  *     for i in range(n):
  *         for j in range(m):             # <<<<<<<<<<<<<<
  *             temp[i+1][j+1] = min(temp[i][j+1] + 1, temp[i+1][j] + 1, temp[i][j] + (a[i] != b[j]))
  *     return temp[n][m]
  */
     __pyx_t_11 = __pyx_v_m;
     __pyx_t_12 = __pyx_t_11;
     for (__pyx_t_13 = 0; __pyx_t_13 < __pyx_t_12; __pyx_t_13+=1) {
       __pyx_v_j = __pyx_t_13;
 
-      /* "pydivsufsort/stringalg.pyx":195
+      /* "pydivsufsort/stringalg.pyx":198
  *     for i in range(n):
  *         for j in range(m):
  *             temp[i+1][j+1] = min(temp[i][j+1] + 1, temp[i+1][j] + 1, temp[i][j] + (a[i] != b[j]))             # <<<<<<<<<<<<<<
  *     return temp[n][m]
  * 
  */
       __pyx_t_14 = (__pyx_v_i + 1);
-      __pyx_t_6 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_t_14, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_t_14, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_5 = __Pyx_GetItemInt(__pyx_t_6, __pyx_v_j, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_GetItemInt(__pyx_t_6, __pyx_v_j, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __pyx_t_6 = __Pyx_PyInt_AddObjC(__pyx_t_5, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyInt_AddObjC(__pyx_t_5, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_5, __pyx_v_j, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_5, __pyx_v_j, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_t_14 = __pyx_v_i;
       __pyx_t_15 = __pyx_v_j;
-      __pyx_t_5 = __Pyx_PyBool_FromLong(((*((__pyx_t_5numpy_int8_t *) ( /* dim=0 */ ((char *) (((__pyx_t_5numpy_int8_t *) __pyx_v_a.data) + __pyx_t_14)) ))) != (*((__pyx_t_5numpy_int8_t *) ( /* dim=0 */ ((char *) (((__pyx_t_5numpy_int8_t *) __pyx_v_b.data) + __pyx_t_15)) ))))); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyBool_FromLong(((*((__pyx_t_5numpy_int8_t *) ( /* dim=0 */ ((char *) (((__pyx_t_5numpy_int8_t *) __pyx_v_a.data) + __pyx_t_14)) ))) != (*((__pyx_t_5numpy_int8_t *) ( /* dim=0 */ ((char *) (((__pyx_t_5numpy_int8_t *) __pyx_v_b.data) + __pyx_t_15)) ))))); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_3 = PyNumber_Add(__pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_3 = PyNumber_Add(__pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __pyx_t_15 = (__pyx_v_j + 1);
-      __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_5, __pyx_t_15, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_5, __pyx_t_15, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_5 = __Pyx_PyInt_AddObjC(__pyx_t_4, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyInt_AddObjC(__pyx_t_4, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_2 = PyObject_RichCompare(__pyx_t_6, __pyx_t_5, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 195, __pyx_L1_error)
-      __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_2 = PyObject_RichCompare(__pyx_t_6, __pyx_t_5, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 198, __pyx_L1_error)
+      __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       if (__pyx_t_16) {
         __Pyx_INCREF(__pyx_t_6);
         __pyx_t_4 = __pyx_t_6;
       } else {
         __Pyx_INCREF(__pyx_t_5);
         __pyx_t_4 = __pyx_t_5;
       }
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_INCREF(__pyx_t_4);
       __pyx_t_5 = __pyx_t_4;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_2 = PyObject_RichCompare(__pyx_t_3, __pyx_t_5, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 195, __pyx_L1_error)
-      __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_2 = PyObject_RichCompare(__pyx_t_3, __pyx_t_5, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 198, __pyx_L1_error)
+      __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       if (__pyx_t_16) {
         __Pyx_INCREF(__pyx_t_3);
         __pyx_t_4 = __pyx_t_3;
       } else {
         __Pyx_INCREF(__pyx_t_5);
         __pyx_t_4 = __pyx_t_5;
@@ -25260,42 +25401,42 @@
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __pyx_t_6 = __pyx_t_4;
       __Pyx_INCREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_t_15 = (__pyx_v_i + 1);
-      __pyx_t_4 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_t_15, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_t_15, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_15 = (__pyx_v_j + 1);
-      if (unlikely(__Pyx_SetItemInt(__pyx_t_4, __pyx_t_15, __pyx_t_6, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0) < 0)) __PYX_ERR(0, 195, __pyx_L1_error)
+      if (unlikely(__Pyx_SetItemInt(__pyx_t_4, __pyx_t_15, __pyx_t_6, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0) < 0)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
   }
 
-  /* "pydivsufsort/stringalg.pyx":196
+  /* "pydivsufsort/stringalg.pyx":199
  *         for j in range(m):
  *             temp[i+1][j+1] = min(temp[i][j+1] + 1, temp[i+1][j] + 1, temp[i][j] + (a[i] != b[j]))
  *     return temp[n][m]             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_6 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_n, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 196, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_n, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_6, __pyx_v_m, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 196, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_6, __pyx_v_m, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "pydivsufsort/stringalg.pyx":184
- *     return ans
+  /* "pydivsufsort/stringalg.pyx":187
+ *     return _lcp_query(*segtree, queries)
  * 
  * def _levenshtein(string_t[::1] a not None, string_t[::1] b not None):             # <<<<<<<<<<<<<<
  *     cdef unsigned long long n, m, i, j, d
  *     n = len(a)
  */
 
   /* function exit code */
@@ -25322,17 +25463,17 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_b, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_5__pyx_pw_12pydivsufsort_9stringalg_115_levenshtein(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_5__pyx_mdef_12pydivsufsort_9stringalg_115_levenshtein = {"__pyx_fuse_5_levenshtein", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_5__pyx_pw_12pydivsufsort_9stringalg_115_levenshtein, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_fuse_5__pyx_pw_12pydivsufsort_9stringalg_115_levenshtein(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_5__pyx_pw_12pydivsufsort_9stringalg_117_levenshtein(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_5__pyx_mdef_12pydivsufsort_9stringalg_117_levenshtein = {"__pyx_fuse_5_levenshtein", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_5__pyx_pw_12pydivsufsort_9stringalg_117_levenshtein, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_fuse_5__pyx_pw_12pydivsufsort_9stringalg_117_levenshtein(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_a = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_b = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -25356,55 +25497,55 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_a)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_b)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_levenshtein", 1, 2, 2, 1); __PYX_ERR(0, 184, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_levenshtein", 1, 2, 2, 1); __PYX_ERR(0, 187, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_levenshtein") < 0)) __PYX_ERR(0, 184, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_levenshtein") < 0)) __PYX_ERR(0, 187, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
-    __pyx_v_a = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_int16_t(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_a.memview)) __PYX_ERR(0, 184, __pyx_L3_error)
-    __pyx_v_b = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_int16_t(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_b.memview)) __PYX_ERR(0, 184, __pyx_L3_error)
+    __pyx_v_a = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_int16_t(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_a.memview)) __PYX_ERR(0, 187, __pyx_L3_error)
+    __pyx_v_b = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_int16_t(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_b.memview)) __PYX_ERR(0, 187, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_levenshtein", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 184, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_levenshtein", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 187, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pydivsufsort.stringalg._levenshtein", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(((PyObject *)__pyx_v_a.memview) == Py_None)) {
-    PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "a"); __PYX_ERR(0, 184, __pyx_L1_error)
+    PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "a"); __PYX_ERR(0, 187, __pyx_L1_error)
   }
   if (unlikely(((PyObject *)__pyx_v_b.memview) == Py_None)) {
-    PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "b"); __PYX_ERR(0, 184, __pyx_L1_error)
+    PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "b"); __PYX_ERR(0, 187, __pyx_L1_error)
   }
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_114_levenshtein(__pyx_self, __pyx_v_a, __pyx_v_b);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_116_levenshtein(__pyx_self, __pyx_v_a, __pyx_v_b);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_114_levenshtein(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_a, __Pyx_memviewslice __pyx_v_b) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_116_levenshtein(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_a, __Pyx_memviewslice __pyx_v_b) {
   unsigned PY_LONG_LONG __pyx_v_n;
   unsigned PY_LONG_LONG __pyx_v_m;
   unsigned PY_LONG_LONG __pyx_v_i;
   unsigned PY_LONG_LONG __pyx_v_j;
   PyArrayObject *__pyx_v_temp = 0;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_temp;
   __Pyx_Buffer __pyx_pybuffer_temp;
@@ -25431,225 +25572,225 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_5_levenshtein", 0);
   __pyx_pybuffer_temp.pybuffer.buf = NULL;
   __pyx_pybuffer_temp.refcount = 0;
   __pyx_pybuffernd_temp.data = NULL;
   __pyx_pybuffernd_temp.rcbuffer = &__pyx_pybuffer_temp;
 
-  /* "pydivsufsort/stringalg.pyx":186
+  /* "pydivsufsort/stringalg.pyx":189
  * def _levenshtein(string_t[::1] a not None, string_t[::1] b not None):
  *     cdef unsigned long long n, m, i, j, d
  *     n = len(a)             # <<<<<<<<<<<<<<
  *     m = len(b)
  *     cdef np.ndarray[np.uint64_t, ndim=2] temp = np.empty((n+1, m+1), dtype=np.uint64)
  */
   __pyx_t_1 = __Pyx_MemoryView_Len(__pyx_v_a); 
   __pyx_v_n = __pyx_t_1;
 
-  /* "pydivsufsort/stringalg.pyx":187
+  /* "pydivsufsort/stringalg.pyx":190
  *     cdef unsigned long long n, m, i, j, d
  *     n = len(a)
  *     m = len(b)             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.uint64_t, ndim=2] temp = np.empty((n+1, m+1), dtype=np.uint64)
  *     for i in range(n):
  */
   __pyx_t_1 = __Pyx_MemoryView_Len(__pyx_v_b); 
   __pyx_v_m = __pyx_t_1;
 
-  /* "pydivsufsort/stringalg.pyx":188
+  /* "pydivsufsort/stringalg.pyx":191
  *     n = len(a)
  *     m = len(b)
  *     cdef np.ndarray[np.uint64_t, ndim=2] temp = np.empty((n+1, m+1), dtype=np.uint64)             # <<<<<<<<<<<<<<
  *     for i in range(n):
  *         temp[i][0] = i
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG((__pyx_v_n + 1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG((__pyx_v_n + 1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG((__pyx_v_m + 1)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG((__pyx_v_m + 1)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_4);
   __pyx_t_2 = 0;
   __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5);
   __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_uint64); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_uint64); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 188, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 188, __pyx_L1_error)
+  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 191, __pyx_L1_error)
   __pyx_t_7 = ((PyArrayObject *)__pyx_t_6);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_temp.rcbuffer->pybuffer, (PyObject*)__pyx_t_7, &__Pyx_TypeInfo_nn___pyx_t_5numpy_uint64_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_temp = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_temp.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 188, __pyx_L1_error)
+      __PYX_ERR(0, 191, __pyx_L1_error)
     } else {__pyx_pybuffernd_temp.diminfo[0].strides = __pyx_pybuffernd_temp.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_temp.diminfo[0].shape = __pyx_pybuffernd_temp.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_temp.diminfo[1].strides = __pyx_pybuffernd_temp.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_temp.diminfo[1].shape = __pyx_pybuffernd_temp.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_t_7 = 0;
   __pyx_v_temp = ((PyArrayObject *)__pyx_t_6);
   __pyx_t_6 = 0;
 
-  /* "pydivsufsort/stringalg.pyx":189
+  /* "pydivsufsort/stringalg.pyx":192
  *     m = len(b)
  *     cdef np.ndarray[np.uint64_t, ndim=2] temp = np.empty((n+1, m+1), dtype=np.uint64)
  *     for i in range(n):             # <<<<<<<<<<<<<<
  *         temp[i][0] = i
  *     for j in range(m):
  */
   __pyx_t_8 = __pyx_v_n;
   __pyx_t_9 = __pyx_t_8;
   for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
     __pyx_v_i = __pyx_t_10;
 
-    /* "pydivsufsort/stringalg.pyx":190
+    /* "pydivsufsort/stringalg.pyx":193
  *     cdef np.ndarray[np.uint64_t, ndim=2] temp = np.empty((n+1, m+1), dtype=np.uint64)
  *     for i in range(n):
  *         temp[i][0] = i             # <<<<<<<<<<<<<<
  *     for j in range(m):
  *         temp[0][j] = j
  */
-    __pyx_t_6 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG(__pyx_v_i); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 190, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG(__pyx_v_i); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 193, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 190, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 193, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (unlikely(__Pyx_SetItemInt(__pyx_t_5, 0, __pyx_t_6, long, 1, __Pyx_PyInt_From_long, 0, 0, 0) < 0)) __PYX_ERR(0, 190, __pyx_L1_error)
+    if (unlikely(__Pyx_SetItemInt(__pyx_t_5, 0, __pyx_t_6, long, 1, __Pyx_PyInt_From_long, 0, 0, 0) < 0)) __PYX_ERR(0, 193, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
 
-  /* "pydivsufsort/stringalg.pyx":191
+  /* "pydivsufsort/stringalg.pyx":194
  *     for i in range(n):
  *         temp[i][0] = i
  *     for j in range(m):             # <<<<<<<<<<<<<<
  *         temp[0][j] = j
  *     for i in range(n):
  */
   __pyx_t_8 = __pyx_v_m;
   __pyx_t_9 = __pyx_t_8;
   for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
     __pyx_v_j = __pyx_t_10;
 
-    /* "pydivsufsort/stringalg.pyx":192
+    /* "pydivsufsort/stringalg.pyx":195
  *         temp[i][0] = i
  *     for j in range(m):
  *         temp[0][j] = j             # <<<<<<<<<<<<<<
  *     for i in range(n):
  *         for j in range(m):
  */
-    __pyx_t_6 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG(__pyx_v_j); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 192, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG(__pyx_v_j); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 195, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 192, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (unlikely(__Pyx_SetItemInt(__pyx_t_5, __pyx_v_j, __pyx_t_6, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0) < 0)) __PYX_ERR(0, 192, __pyx_L1_error)
+    if (unlikely(__Pyx_SetItemInt(__pyx_t_5, __pyx_v_j, __pyx_t_6, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0) < 0)) __PYX_ERR(0, 195, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
 
-  /* "pydivsufsort/stringalg.pyx":193
+  /* "pydivsufsort/stringalg.pyx":196
  *     for j in range(m):
  *         temp[0][j] = j
  *     for i in range(n):             # <<<<<<<<<<<<<<
  *         for j in range(m):
  *             temp[i+1][j+1] = min(temp[i][j+1] + 1, temp[i+1][j] + 1, temp[i][j] + (a[i] != b[j]))
  */
   __pyx_t_8 = __pyx_v_n;
   __pyx_t_9 = __pyx_t_8;
   for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
     __pyx_v_i = __pyx_t_10;
 
-    /* "pydivsufsort/stringalg.pyx":194
+    /* "pydivsufsort/stringalg.pyx":197
  *         temp[0][j] = j
  *     for i in range(n):
  *         for j in range(m):             # <<<<<<<<<<<<<<
  *             temp[i+1][j+1] = min(temp[i][j+1] + 1, temp[i+1][j] + 1, temp[i][j] + (a[i] != b[j]))
  *     return temp[n][m]
  */
     __pyx_t_11 = __pyx_v_m;
     __pyx_t_12 = __pyx_t_11;
     for (__pyx_t_13 = 0; __pyx_t_13 < __pyx_t_12; __pyx_t_13+=1) {
       __pyx_v_j = __pyx_t_13;
 
-      /* "pydivsufsort/stringalg.pyx":195
+      /* "pydivsufsort/stringalg.pyx":198
  *     for i in range(n):
  *         for j in range(m):
  *             temp[i+1][j+1] = min(temp[i][j+1] + 1, temp[i+1][j] + 1, temp[i][j] + (a[i] != b[j]))             # <<<<<<<<<<<<<<
  *     return temp[n][m]
  * 
  */
       __pyx_t_14 = (__pyx_v_i + 1);
-      __pyx_t_6 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_t_14, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_t_14, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_5 = __Pyx_GetItemInt(__pyx_t_6, __pyx_v_j, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_GetItemInt(__pyx_t_6, __pyx_v_j, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __pyx_t_6 = __Pyx_PyInt_AddObjC(__pyx_t_5, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyInt_AddObjC(__pyx_t_5, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_5, __pyx_v_j, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_5, __pyx_v_j, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_t_14 = __pyx_v_i;
       __pyx_t_15 = __pyx_v_j;
-      __pyx_t_5 = __Pyx_PyBool_FromLong(((*((__pyx_t_5numpy_int16_t *) ( /* dim=0 */ ((char *) (((__pyx_t_5numpy_int16_t *) __pyx_v_a.data) + __pyx_t_14)) ))) != (*((__pyx_t_5numpy_int16_t *) ( /* dim=0 */ ((char *) (((__pyx_t_5numpy_int16_t *) __pyx_v_b.data) + __pyx_t_15)) ))))); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyBool_FromLong(((*((__pyx_t_5numpy_int16_t *) ( /* dim=0 */ ((char *) (((__pyx_t_5numpy_int16_t *) __pyx_v_a.data) + __pyx_t_14)) ))) != (*((__pyx_t_5numpy_int16_t *) ( /* dim=0 */ ((char *) (((__pyx_t_5numpy_int16_t *) __pyx_v_b.data) + __pyx_t_15)) ))))); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_3 = PyNumber_Add(__pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_3 = PyNumber_Add(__pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __pyx_t_15 = (__pyx_v_j + 1);
-      __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_5, __pyx_t_15, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_5, __pyx_t_15, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_5 = __Pyx_PyInt_AddObjC(__pyx_t_4, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyInt_AddObjC(__pyx_t_4, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_2 = PyObject_RichCompare(__pyx_t_6, __pyx_t_5, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 195, __pyx_L1_error)
-      __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_2 = PyObject_RichCompare(__pyx_t_6, __pyx_t_5, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 198, __pyx_L1_error)
+      __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       if (__pyx_t_16) {
         __Pyx_INCREF(__pyx_t_6);
         __pyx_t_4 = __pyx_t_6;
       } else {
         __Pyx_INCREF(__pyx_t_5);
         __pyx_t_4 = __pyx_t_5;
       }
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_INCREF(__pyx_t_4);
       __pyx_t_5 = __pyx_t_4;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_2 = PyObject_RichCompare(__pyx_t_3, __pyx_t_5, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 195, __pyx_L1_error)
-      __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_2 = PyObject_RichCompare(__pyx_t_3, __pyx_t_5, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 198, __pyx_L1_error)
+      __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       if (__pyx_t_16) {
         __Pyx_INCREF(__pyx_t_3);
         __pyx_t_4 = __pyx_t_3;
       } else {
         __Pyx_INCREF(__pyx_t_5);
         __pyx_t_4 = __pyx_t_5;
@@ -25657,42 +25798,42 @@
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __pyx_t_6 = __pyx_t_4;
       __Pyx_INCREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_t_15 = (__pyx_v_i + 1);
-      __pyx_t_4 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_t_15, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_t_15, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_15 = (__pyx_v_j + 1);
-      if (unlikely(__Pyx_SetItemInt(__pyx_t_4, __pyx_t_15, __pyx_t_6, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0) < 0)) __PYX_ERR(0, 195, __pyx_L1_error)
+      if (unlikely(__Pyx_SetItemInt(__pyx_t_4, __pyx_t_15, __pyx_t_6, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0) < 0)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
   }
 
-  /* "pydivsufsort/stringalg.pyx":196
+  /* "pydivsufsort/stringalg.pyx":199
  *         for j in range(m):
  *             temp[i+1][j+1] = min(temp[i][j+1] + 1, temp[i+1][j] + 1, temp[i][j] + (a[i] != b[j]))
  *     return temp[n][m]             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_6 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_n, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 196, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_n, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_6, __pyx_v_m, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 196, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_6, __pyx_v_m, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "pydivsufsort/stringalg.pyx":184
- *     return ans
+  /* "pydivsufsort/stringalg.pyx":187
+ *     return _lcp_query(*segtree, queries)
  * 
  * def _levenshtein(string_t[::1] a not None, string_t[::1] b not None):             # <<<<<<<<<<<<<<
  *     cdef unsigned long long n, m, i, j, d
  *     n = len(a)
  */
 
   /* function exit code */
@@ -25719,17 +25860,17 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_b, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_6__pyx_pw_12pydivsufsort_9stringalg_117_levenshtein(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_6__pyx_mdef_12pydivsufsort_9stringalg_117_levenshtein = {"__pyx_fuse_6_levenshtein", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_6__pyx_pw_12pydivsufsort_9stringalg_117_levenshtein, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_fuse_6__pyx_pw_12pydivsufsort_9stringalg_117_levenshtein(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_6__pyx_pw_12pydivsufsort_9stringalg_119_levenshtein(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_6__pyx_mdef_12pydivsufsort_9stringalg_119_levenshtein = {"__pyx_fuse_6_levenshtein", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_6__pyx_pw_12pydivsufsort_9stringalg_119_levenshtein, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_fuse_6__pyx_pw_12pydivsufsort_9stringalg_119_levenshtein(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_a = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_b = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -25753,55 +25894,55 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_a)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_b)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_levenshtein", 1, 2, 2, 1); __PYX_ERR(0, 184, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_levenshtein", 1, 2, 2, 1); __PYX_ERR(0, 187, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_levenshtein") < 0)) __PYX_ERR(0, 184, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_levenshtein") < 0)) __PYX_ERR(0, 187, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
-    __pyx_v_a = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_int32_t(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_a.memview)) __PYX_ERR(0, 184, __pyx_L3_error)
-    __pyx_v_b = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_int32_t(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_b.memview)) __PYX_ERR(0, 184, __pyx_L3_error)
+    __pyx_v_a = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_int32_t(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_a.memview)) __PYX_ERR(0, 187, __pyx_L3_error)
+    __pyx_v_b = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_int32_t(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_b.memview)) __PYX_ERR(0, 187, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_levenshtein", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 184, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_levenshtein", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 187, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pydivsufsort.stringalg._levenshtein", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(((PyObject *)__pyx_v_a.memview) == Py_None)) {
-    PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "a"); __PYX_ERR(0, 184, __pyx_L1_error)
+    PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "a"); __PYX_ERR(0, 187, __pyx_L1_error)
   }
   if (unlikely(((PyObject *)__pyx_v_b.memview) == Py_None)) {
-    PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "b"); __PYX_ERR(0, 184, __pyx_L1_error)
+    PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "b"); __PYX_ERR(0, 187, __pyx_L1_error)
   }
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_116_levenshtein(__pyx_self, __pyx_v_a, __pyx_v_b);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_118_levenshtein(__pyx_self, __pyx_v_a, __pyx_v_b);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_116_levenshtein(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_a, __Pyx_memviewslice __pyx_v_b) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_118_levenshtein(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_a, __Pyx_memviewslice __pyx_v_b) {
   unsigned PY_LONG_LONG __pyx_v_n;
   unsigned PY_LONG_LONG __pyx_v_m;
   unsigned PY_LONG_LONG __pyx_v_i;
   unsigned PY_LONG_LONG __pyx_v_j;
   PyArrayObject *__pyx_v_temp = 0;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_temp;
   __Pyx_Buffer __pyx_pybuffer_temp;
@@ -25828,225 +25969,225 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_6_levenshtein", 0);
   __pyx_pybuffer_temp.pybuffer.buf = NULL;
   __pyx_pybuffer_temp.refcount = 0;
   __pyx_pybuffernd_temp.data = NULL;
   __pyx_pybuffernd_temp.rcbuffer = &__pyx_pybuffer_temp;
 
-  /* "pydivsufsort/stringalg.pyx":186
+  /* "pydivsufsort/stringalg.pyx":189
  * def _levenshtein(string_t[::1] a not None, string_t[::1] b not None):
  *     cdef unsigned long long n, m, i, j, d
  *     n = len(a)             # <<<<<<<<<<<<<<
  *     m = len(b)
  *     cdef np.ndarray[np.uint64_t, ndim=2] temp = np.empty((n+1, m+1), dtype=np.uint64)
  */
   __pyx_t_1 = __Pyx_MemoryView_Len(__pyx_v_a); 
   __pyx_v_n = __pyx_t_1;
 
-  /* "pydivsufsort/stringalg.pyx":187
+  /* "pydivsufsort/stringalg.pyx":190
  *     cdef unsigned long long n, m, i, j, d
  *     n = len(a)
  *     m = len(b)             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.uint64_t, ndim=2] temp = np.empty((n+1, m+1), dtype=np.uint64)
  *     for i in range(n):
  */
   __pyx_t_1 = __Pyx_MemoryView_Len(__pyx_v_b); 
   __pyx_v_m = __pyx_t_1;
 
-  /* "pydivsufsort/stringalg.pyx":188
+  /* "pydivsufsort/stringalg.pyx":191
  *     n = len(a)
  *     m = len(b)
  *     cdef np.ndarray[np.uint64_t, ndim=2] temp = np.empty((n+1, m+1), dtype=np.uint64)             # <<<<<<<<<<<<<<
  *     for i in range(n):
  *         temp[i][0] = i
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG((__pyx_v_n + 1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG((__pyx_v_n + 1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG((__pyx_v_m + 1)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG((__pyx_v_m + 1)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_4);
   __pyx_t_2 = 0;
   __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5);
   __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_uint64); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_uint64); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 188, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 188, __pyx_L1_error)
+  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 191, __pyx_L1_error)
   __pyx_t_7 = ((PyArrayObject *)__pyx_t_6);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_temp.rcbuffer->pybuffer, (PyObject*)__pyx_t_7, &__Pyx_TypeInfo_nn___pyx_t_5numpy_uint64_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_temp = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_temp.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 188, __pyx_L1_error)
+      __PYX_ERR(0, 191, __pyx_L1_error)
     } else {__pyx_pybuffernd_temp.diminfo[0].strides = __pyx_pybuffernd_temp.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_temp.diminfo[0].shape = __pyx_pybuffernd_temp.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_temp.diminfo[1].strides = __pyx_pybuffernd_temp.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_temp.diminfo[1].shape = __pyx_pybuffernd_temp.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_t_7 = 0;
   __pyx_v_temp = ((PyArrayObject *)__pyx_t_6);
   __pyx_t_6 = 0;
 
-  /* "pydivsufsort/stringalg.pyx":189
+  /* "pydivsufsort/stringalg.pyx":192
  *     m = len(b)
  *     cdef np.ndarray[np.uint64_t, ndim=2] temp = np.empty((n+1, m+1), dtype=np.uint64)
  *     for i in range(n):             # <<<<<<<<<<<<<<
  *         temp[i][0] = i
  *     for j in range(m):
  */
   __pyx_t_8 = __pyx_v_n;
   __pyx_t_9 = __pyx_t_8;
   for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
     __pyx_v_i = __pyx_t_10;
 
-    /* "pydivsufsort/stringalg.pyx":190
+    /* "pydivsufsort/stringalg.pyx":193
  *     cdef np.ndarray[np.uint64_t, ndim=2] temp = np.empty((n+1, m+1), dtype=np.uint64)
  *     for i in range(n):
  *         temp[i][0] = i             # <<<<<<<<<<<<<<
  *     for j in range(m):
  *         temp[0][j] = j
  */
-    __pyx_t_6 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG(__pyx_v_i); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 190, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG(__pyx_v_i); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 193, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 190, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 193, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (unlikely(__Pyx_SetItemInt(__pyx_t_5, 0, __pyx_t_6, long, 1, __Pyx_PyInt_From_long, 0, 0, 0) < 0)) __PYX_ERR(0, 190, __pyx_L1_error)
+    if (unlikely(__Pyx_SetItemInt(__pyx_t_5, 0, __pyx_t_6, long, 1, __Pyx_PyInt_From_long, 0, 0, 0) < 0)) __PYX_ERR(0, 193, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
 
-  /* "pydivsufsort/stringalg.pyx":191
+  /* "pydivsufsort/stringalg.pyx":194
  *     for i in range(n):
  *         temp[i][0] = i
  *     for j in range(m):             # <<<<<<<<<<<<<<
  *         temp[0][j] = j
  *     for i in range(n):
  */
   __pyx_t_8 = __pyx_v_m;
   __pyx_t_9 = __pyx_t_8;
   for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
     __pyx_v_j = __pyx_t_10;
 
-    /* "pydivsufsort/stringalg.pyx":192
+    /* "pydivsufsort/stringalg.pyx":195
  *         temp[i][0] = i
  *     for j in range(m):
  *         temp[0][j] = j             # <<<<<<<<<<<<<<
  *     for i in range(n):
  *         for j in range(m):
  */
-    __pyx_t_6 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG(__pyx_v_j); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 192, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG(__pyx_v_j); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 195, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 192, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (unlikely(__Pyx_SetItemInt(__pyx_t_5, __pyx_v_j, __pyx_t_6, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0) < 0)) __PYX_ERR(0, 192, __pyx_L1_error)
+    if (unlikely(__Pyx_SetItemInt(__pyx_t_5, __pyx_v_j, __pyx_t_6, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0) < 0)) __PYX_ERR(0, 195, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
 
-  /* "pydivsufsort/stringalg.pyx":193
+  /* "pydivsufsort/stringalg.pyx":196
  *     for j in range(m):
  *         temp[0][j] = j
  *     for i in range(n):             # <<<<<<<<<<<<<<
  *         for j in range(m):
  *             temp[i+1][j+1] = min(temp[i][j+1] + 1, temp[i+1][j] + 1, temp[i][j] + (a[i] != b[j]))
  */
   __pyx_t_8 = __pyx_v_n;
   __pyx_t_9 = __pyx_t_8;
   for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
     __pyx_v_i = __pyx_t_10;
 
-    /* "pydivsufsort/stringalg.pyx":194
+    /* "pydivsufsort/stringalg.pyx":197
  *         temp[0][j] = j
  *     for i in range(n):
  *         for j in range(m):             # <<<<<<<<<<<<<<
  *             temp[i+1][j+1] = min(temp[i][j+1] + 1, temp[i+1][j] + 1, temp[i][j] + (a[i] != b[j]))
  *     return temp[n][m]
  */
     __pyx_t_11 = __pyx_v_m;
     __pyx_t_12 = __pyx_t_11;
     for (__pyx_t_13 = 0; __pyx_t_13 < __pyx_t_12; __pyx_t_13+=1) {
       __pyx_v_j = __pyx_t_13;
 
-      /* "pydivsufsort/stringalg.pyx":195
+      /* "pydivsufsort/stringalg.pyx":198
  *     for i in range(n):
  *         for j in range(m):
  *             temp[i+1][j+1] = min(temp[i][j+1] + 1, temp[i+1][j] + 1, temp[i][j] + (a[i] != b[j]))             # <<<<<<<<<<<<<<
  *     return temp[n][m]
  * 
  */
       __pyx_t_14 = (__pyx_v_i + 1);
-      __pyx_t_6 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_t_14, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_t_14, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_5 = __Pyx_GetItemInt(__pyx_t_6, __pyx_v_j, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_GetItemInt(__pyx_t_6, __pyx_v_j, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __pyx_t_6 = __Pyx_PyInt_AddObjC(__pyx_t_5, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyInt_AddObjC(__pyx_t_5, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_5, __pyx_v_j, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_5, __pyx_v_j, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_t_14 = __pyx_v_i;
       __pyx_t_15 = __pyx_v_j;
-      __pyx_t_5 = __Pyx_PyBool_FromLong(((*((__pyx_t_5numpy_int32_t *) ( /* dim=0 */ ((char *) (((__pyx_t_5numpy_int32_t *) __pyx_v_a.data) + __pyx_t_14)) ))) != (*((__pyx_t_5numpy_int32_t *) ( /* dim=0 */ ((char *) (((__pyx_t_5numpy_int32_t *) __pyx_v_b.data) + __pyx_t_15)) ))))); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyBool_FromLong(((*((__pyx_t_5numpy_int32_t *) ( /* dim=0 */ ((char *) (((__pyx_t_5numpy_int32_t *) __pyx_v_a.data) + __pyx_t_14)) ))) != (*((__pyx_t_5numpy_int32_t *) ( /* dim=0 */ ((char *) (((__pyx_t_5numpy_int32_t *) __pyx_v_b.data) + __pyx_t_15)) ))))); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_3 = PyNumber_Add(__pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_3 = PyNumber_Add(__pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __pyx_t_15 = (__pyx_v_j + 1);
-      __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_5, __pyx_t_15, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_5, __pyx_t_15, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_5 = __Pyx_PyInt_AddObjC(__pyx_t_4, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyInt_AddObjC(__pyx_t_4, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_2 = PyObject_RichCompare(__pyx_t_6, __pyx_t_5, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 195, __pyx_L1_error)
-      __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_2 = PyObject_RichCompare(__pyx_t_6, __pyx_t_5, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 198, __pyx_L1_error)
+      __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       if (__pyx_t_16) {
         __Pyx_INCREF(__pyx_t_6);
         __pyx_t_4 = __pyx_t_6;
       } else {
         __Pyx_INCREF(__pyx_t_5);
         __pyx_t_4 = __pyx_t_5;
       }
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_INCREF(__pyx_t_4);
       __pyx_t_5 = __pyx_t_4;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_2 = PyObject_RichCompare(__pyx_t_3, __pyx_t_5, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 195, __pyx_L1_error)
-      __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_2 = PyObject_RichCompare(__pyx_t_3, __pyx_t_5, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 198, __pyx_L1_error)
+      __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       if (__pyx_t_16) {
         __Pyx_INCREF(__pyx_t_3);
         __pyx_t_4 = __pyx_t_3;
       } else {
         __Pyx_INCREF(__pyx_t_5);
         __pyx_t_4 = __pyx_t_5;
@@ -26054,42 +26195,42 @@
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __pyx_t_6 = __pyx_t_4;
       __Pyx_INCREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_t_15 = (__pyx_v_i + 1);
-      __pyx_t_4 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_t_15, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_t_15, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_15 = (__pyx_v_j + 1);
-      if (unlikely(__Pyx_SetItemInt(__pyx_t_4, __pyx_t_15, __pyx_t_6, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0) < 0)) __PYX_ERR(0, 195, __pyx_L1_error)
+      if (unlikely(__Pyx_SetItemInt(__pyx_t_4, __pyx_t_15, __pyx_t_6, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0) < 0)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
   }
 
-  /* "pydivsufsort/stringalg.pyx":196
+  /* "pydivsufsort/stringalg.pyx":199
  *         for j in range(m):
  *             temp[i+1][j+1] = min(temp[i][j+1] + 1, temp[i+1][j] + 1, temp[i][j] + (a[i] != b[j]))
  *     return temp[n][m]             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_6 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_n, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 196, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_n, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_6, __pyx_v_m, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 196, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_6, __pyx_v_m, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "pydivsufsort/stringalg.pyx":184
- *     return ans
+  /* "pydivsufsort/stringalg.pyx":187
+ *     return _lcp_query(*segtree, queries)
  * 
  * def _levenshtein(string_t[::1] a not None, string_t[::1] b not None):             # <<<<<<<<<<<<<<
  *     cdef unsigned long long n, m, i, j, d
  *     n = len(a)
  */
 
   /* function exit code */
@@ -26116,17 +26257,17 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_b, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_7__pyx_pw_12pydivsufsort_9stringalg_119_levenshtein(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_7__pyx_mdef_12pydivsufsort_9stringalg_119_levenshtein = {"__pyx_fuse_7_levenshtein", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_7__pyx_pw_12pydivsufsort_9stringalg_119_levenshtein, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_fuse_7__pyx_pw_12pydivsufsort_9stringalg_119_levenshtein(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_7__pyx_pw_12pydivsufsort_9stringalg_121_levenshtein(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_7__pyx_mdef_12pydivsufsort_9stringalg_121_levenshtein = {"__pyx_fuse_7_levenshtein", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_7__pyx_pw_12pydivsufsort_9stringalg_121_levenshtein, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_fuse_7__pyx_pw_12pydivsufsort_9stringalg_121_levenshtein(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_a = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_b = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -26150,55 +26291,55 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_a)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_b)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_levenshtein", 1, 2, 2, 1); __PYX_ERR(0, 184, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_levenshtein", 1, 2, 2, 1); __PYX_ERR(0, 187, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_levenshtein") < 0)) __PYX_ERR(0, 184, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_levenshtein") < 0)) __PYX_ERR(0, 187, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
-    __pyx_v_a = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_int64_t(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_a.memview)) __PYX_ERR(0, 184, __pyx_L3_error)
-    __pyx_v_b = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_int64_t(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_b.memview)) __PYX_ERR(0, 184, __pyx_L3_error)
+    __pyx_v_a = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_int64_t(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_a.memview)) __PYX_ERR(0, 187, __pyx_L3_error)
+    __pyx_v_b = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_int64_t(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_b.memview)) __PYX_ERR(0, 187, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_levenshtein", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 184, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_levenshtein", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 187, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pydivsufsort.stringalg._levenshtein", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(((PyObject *)__pyx_v_a.memview) == Py_None)) {
-    PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "a"); __PYX_ERR(0, 184, __pyx_L1_error)
+    PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "a"); __PYX_ERR(0, 187, __pyx_L1_error)
   }
   if (unlikely(((PyObject *)__pyx_v_b.memview) == Py_None)) {
-    PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "b"); __PYX_ERR(0, 184, __pyx_L1_error)
+    PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "b"); __PYX_ERR(0, 187, __pyx_L1_error)
   }
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_118_levenshtein(__pyx_self, __pyx_v_a, __pyx_v_b);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_120_levenshtein(__pyx_self, __pyx_v_a, __pyx_v_b);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_118_levenshtein(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_a, __Pyx_memviewslice __pyx_v_b) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_120_levenshtein(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_a, __Pyx_memviewslice __pyx_v_b) {
   unsigned PY_LONG_LONG __pyx_v_n;
   unsigned PY_LONG_LONG __pyx_v_m;
   unsigned PY_LONG_LONG __pyx_v_i;
   unsigned PY_LONG_LONG __pyx_v_j;
   PyArrayObject *__pyx_v_temp = 0;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_temp;
   __Pyx_Buffer __pyx_pybuffer_temp;
@@ -26225,225 +26366,225 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_7_levenshtein", 0);
   __pyx_pybuffer_temp.pybuffer.buf = NULL;
   __pyx_pybuffer_temp.refcount = 0;
   __pyx_pybuffernd_temp.data = NULL;
   __pyx_pybuffernd_temp.rcbuffer = &__pyx_pybuffer_temp;
 
-  /* "pydivsufsort/stringalg.pyx":186
+  /* "pydivsufsort/stringalg.pyx":189
  * def _levenshtein(string_t[::1] a not None, string_t[::1] b not None):
  *     cdef unsigned long long n, m, i, j, d
  *     n = len(a)             # <<<<<<<<<<<<<<
  *     m = len(b)
  *     cdef np.ndarray[np.uint64_t, ndim=2] temp = np.empty((n+1, m+1), dtype=np.uint64)
  */
   __pyx_t_1 = __Pyx_MemoryView_Len(__pyx_v_a); 
   __pyx_v_n = __pyx_t_1;
 
-  /* "pydivsufsort/stringalg.pyx":187
+  /* "pydivsufsort/stringalg.pyx":190
  *     cdef unsigned long long n, m, i, j, d
  *     n = len(a)
  *     m = len(b)             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.uint64_t, ndim=2] temp = np.empty((n+1, m+1), dtype=np.uint64)
  *     for i in range(n):
  */
   __pyx_t_1 = __Pyx_MemoryView_Len(__pyx_v_b); 
   __pyx_v_m = __pyx_t_1;
 
-  /* "pydivsufsort/stringalg.pyx":188
+  /* "pydivsufsort/stringalg.pyx":191
  *     n = len(a)
  *     m = len(b)
  *     cdef np.ndarray[np.uint64_t, ndim=2] temp = np.empty((n+1, m+1), dtype=np.uint64)             # <<<<<<<<<<<<<<
  *     for i in range(n):
  *         temp[i][0] = i
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG((__pyx_v_n + 1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG((__pyx_v_n + 1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG((__pyx_v_m + 1)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG((__pyx_v_m + 1)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_4);
   __pyx_t_2 = 0;
   __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5);
   __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_uint64); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_uint64); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 188, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 188, __pyx_L1_error)
+  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 191, __pyx_L1_error)
   __pyx_t_7 = ((PyArrayObject *)__pyx_t_6);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_temp.rcbuffer->pybuffer, (PyObject*)__pyx_t_7, &__Pyx_TypeInfo_nn___pyx_t_5numpy_uint64_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_temp = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_temp.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 188, __pyx_L1_error)
+      __PYX_ERR(0, 191, __pyx_L1_error)
     } else {__pyx_pybuffernd_temp.diminfo[0].strides = __pyx_pybuffernd_temp.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_temp.diminfo[0].shape = __pyx_pybuffernd_temp.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_temp.diminfo[1].strides = __pyx_pybuffernd_temp.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_temp.diminfo[1].shape = __pyx_pybuffernd_temp.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_t_7 = 0;
   __pyx_v_temp = ((PyArrayObject *)__pyx_t_6);
   __pyx_t_6 = 0;
 
-  /* "pydivsufsort/stringalg.pyx":189
+  /* "pydivsufsort/stringalg.pyx":192
  *     m = len(b)
  *     cdef np.ndarray[np.uint64_t, ndim=2] temp = np.empty((n+1, m+1), dtype=np.uint64)
  *     for i in range(n):             # <<<<<<<<<<<<<<
  *         temp[i][0] = i
  *     for j in range(m):
  */
   __pyx_t_8 = __pyx_v_n;
   __pyx_t_9 = __pyx_t_8;
   for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
     __pyx_v_i = __pyx_t_10;
 
-    /* "pydivsufsort/stringalg.pyx":190
+    /* "pydivsufsort/stringalg.pyx":193
  *     cdef np.ndarray[np.uint64_t, ndim=2] temp = np.empty((n+1, m+1), dtype=np.uint64)
  *     for i in range(n):
  *         temp[i][0] = i             # <<<<<<<<<<<<<<
  *     for j in range(m):
  *         temp[0][j] = j
  */
-    __pyx_t_6 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG(__pyx_v_i); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 190, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG(__pyx_v_i); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 193, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 190, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 193, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (unlikely(__Pyx_SetItemInt(__pyx_t_5, 0, __pyx_t_6, long, 1, __Pyx_PyInt_From_long, 0, 0, 0) < 0)) __PYX_ERR(0, 190, __pyx_L1_error)
+    if (unlikely(__Pyx_SetItemInt(__pyx_t_5, 0, __pyx_t_6, long, 1, __Pyx_PyInt_From_long, 0, 0, 0) < 0)) __PYX_ERR(0, 193, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
 
-  /* "pydivsufsort/stringalg.pyx":191
+  /* "pydivsufsort/stringalg.pyx":194
  *     for i in range(n):
  *         temp[i][0] = i
  *     for j in range(m):             # <<<<<<<<<<<<<<
  *         temp[0][j] = j
  *     for i in range(n):
  */
   __pyx_t_8 = __pyx_v_m;
   __pyx_t_9 = __pyx_t_8;
   for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
     __pyx_v_j = __pyx_t_10;
 
-    /* "pydivsufsort/stringalg.pyx":192
+    /* "pydivsufsort/stringalg.pyx":195
  *         temp[i][0] = i
  *     for j in range(m):
  *         temp[0][j] = j             # <<<<<<<<<<<<<<
  *     for i in range(n):
  *         for j in range(m):
  */
-    __pyx_t_6 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG(__pyx_v_j); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 192, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG(__pyx_v_j); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 195, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 192, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (unlikely(__Pyx_SetItemInt(__pyx_t_5, __pyx_v_j, __pyx_t_6, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0) < 0)) __PYX_ERR(0, 192, __pyx_L1_error)
+    if (unlikely(__Pyx_SetItemInt(__pyx_t_5, __pyx_v_j, __pyx_t_6, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0) < 0)) __PYX_ERR(0, 195, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
 
-  /* "pydivsufsort/stringalg.pyx":193
+  /* "pydivsufsort/stringalg.pyx":196
  *     for j in range(m):
  *         temp[0][j] = j
  *     for i in range(n):             # <<<<<<<<<<<<<<
  *         for j in range(m):
  *             temp[i+1][j+1] = min(temp[i][j+1] + 1, temp[i+1][j] + 1, temp[i][j] + (a[i] != b[j]))
  */
   __pyx_t_8 = __pyx_v_n;
   __pyx_t_9 = __pyx_t_8;
   for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
     __pyx_v_i = __pyx_t_10;
 
-    /* "pydivsufsort/stringalg.pyx":194
+    /* "pydivsufsort/stringalg.pyx":197
  *         temp[0][j] = j
  *     for i in range(n):
  *         for j in range(m):             # <<<<<<<<<<<<<<
  *             temp[i+1][j+1] = min(temp[i][j+1] + 1, temp[i+1][j] + 1, temp[i][j] + (a[i] != b[j]))
  *     return temp[n][m]
  */
     __pyx_t_11 = __pyx_v_m;
     __pyx_t_12 = __pyx_t_11;
     for (__pyx_t_13 = 0; __pyx_t_13 < __pyx_t_12; __pyx_t_13+=1) {
       __pyx_v_j = __pyx_t_13;
 
-      /* "pydivsufsort/stringalg.pyx":195
+      /* "pydivsufsort/stringalg.pyx":198
  *     for i in range(n):
  *         for j in range(m):
  *             temp[i+1][j+1] = min(temp[i][j+1] + 1, temp[i+1][j] + 1, temp[i][j] + (a[i] != b[j]))             # <<<<<<<<<<<<<<
  *     return temp[n][m]
  * 
  */
       __pyx_t_14 = (__pyx_v_i + 1);
-      __pyx_t_6 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_t_14, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_t_14, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_5 = __Pyx_GetItemInt(__pyx_t_6, __pyx_v_j, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_GetItemInt(__pyx_t_6, __pyx_v_j, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __pyx_t_6 = __Pyx_PyInt_AddObjC(__pyx_t_5, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyInt_AddObjC(__pyx_t_5, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_5, __pyx_v_j, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_5, __pyx_v_j, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_t_14 = __pyx_v_i;
       __pyx_t_15 = __pyx_v_j;
-      __pyx_t_5 = __Pyx_PyBool_FromLong(((*((__pyx_t_5numpy_int64_t *) ( /* dim=0 */ ((char *) (((__pyx_t_5numpy_int64_t *) __pyx_v_a.data) + __pyx_t_14)) ))) != (*((__pyx_t_5numpy_int64_t *) ( /* dim=0 */ ((char *) (((__pyx_t_5numpy_int64_t *) __pyx_v_b.data) + __pyx_t_15)) ))))); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyBool_FromLong(((*((__pyx_t_5numpy_int64_t *) ( /* dim=0 */ ((char *) (((__pyx_t_5numpy_int64_t *) __pyx_v_a.data) + __pyx_t_14)) ))) != (*((__pyx_t_5numpy_int64_t *) ( /* dim=0 */ ((char *) (((__pyx_t_5numpy_int64_t *) __pyx_v_b.data) + __pyx_t_15)) ))))); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_3 = PyNumber_Add(__pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_3 = PyNumber_Add(__pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_i, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __pyx_t_15 = (__pyx_v_j + 1);
-      __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_5, __pyx_t_15, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_5, __pyx_t_15, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_5 = __Pyx_PyInt_AddObjC(__pyx_t_4, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyInt_AddObjC(__pyx_t_4, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_2 = PyObject_RichCompare(__pyx_t_6, __pyx_t_5, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 195, __pyx_L1_error)
-      __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_2 = PyObject_RichCompare(__pyx_t_6, __pyx_t_5, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 198, __pyx_L1_error)
+      __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       if (__pyx_t_16) {
         __Pyx_INCREF(__pyx_t_6);
         __pyx_t_4 = __pyx_t_6;
       } else {
         __Pyx_INCREF(__pyx_t_5);
         __pyx_t_4 = __pyx_t_5;
       }
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_INCREF(__pyx_t_4);
       __pyx_t_5 = __pyx_t_4;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_2 = PyObject_RichCompare(__pyx_t_3, __pyx_t_5, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 195, __pyx_L1_error)
-      __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_2 = PyObject_RichCompare(__pyx_t_3, __pyx_t_5, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 198, __pyx_L1_error)
+      __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       if (__pyx_t_16) {
         __Pyx_INCREF(__pyx_t_3);
         __pyx_t_4 = __pyx_t_3;
       } else {
         __Pyx_INCREF(__pyx_t_5);
         __pyx_t_4 = __pyx_t_5;
@@ -26451,42 +26592,42 @@
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __pyx_t_6 = __pyx_t_4;
       __Pyx_INCREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_t_15 = (__pyx_v_i + 1);
-      __pyx_t_4 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_t_15, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_t_15, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_15 = (__pyx_v_j + 1);
-      if (unlikely(__Pyx_SetItemInt(__pyx_t_4, __pyx_t_15, __pyx_t_6, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0) < 0)) __PYX_ERR(0, 195, __pyx_L1_error)
+      if (unlikely(__Pyx_SetItemInt(__pyx_t_4, __pyx_t_15, __pyx_t_6, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0) < 0)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
   }
 
-  /* "pydivsufsort/stringalg.pyx":196
+  /* "pydivsufsort/stringalg.pyx":199
  *         for j in range(m):
  *             temp[i+1][j+1] = min(temp[i][j+1] + 1, temp[i+1][j] + 1, temp[i][j] + (a[i] != b[j]))
  *     return temp[n][m]             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_6 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_n, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 196, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_GetItemInt(((PyObject *)__pyx_v_temp), __pyx_v_n, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_6, __pyx_v_m, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 196, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_6, __pyx_v_m, unsigned PY_LONG_LONG, 0, __Pyx_PyInt_From_unsigned_PY_LONG_LONG, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "pydivsufsort/stringalg.pyx":184
- *     return ans
+  /* "pydivsufsort/stringalg.pyx":187
+ *     return _lcp_query(*segtree, queries)
  * 
  * def _levenshtein(string_t[::1] a not None, string_t[::1] b not None):             # <<<<<<<<<<<<<<
  *     cdef unsigned long long n, m, i, j, d
  *     n = len(a)
  */
 
   /* function exit code */
@@ -26512,26 +26653,26 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_a, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_b, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pydivsufsort/stringalg.pyx":199
+/* "pydivsufsort/stringalg.pyx":202
  * 
  * 
  * def levenshtein(a, b):             # <<<<<<<<<<<<<<
  *     a = handle_input(a)
  *     b = handle_input(b)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_12pydivsufsort_9stringalg_17levenshtein(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_mdef_12pydivsufsort_9stringalg_17levenshtein = {"levenshtein", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_12pydivsufsort_9stringalg_17levenshtein, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_12pydivsufsort_9stringalg_17levenshtein(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_12pydivsufsort_9stringalg_19levenshtein(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_12pydivsufsort_9stringalg_19levenshtein = {"levenshtein", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_12pydivsufsort_9stringalg_19levenshtein, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_12pydivsufsort_9stringalg_19levenshtein(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_a = 0;
   PyObject *__pyx_v_b = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -26555,45 +26696,45 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_a)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_b)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("levenshtein", 1, 2, 2, 1); __PYX_ERR(0, 199, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("levenshtein", 1, 2, 2, 1); __PYX_ERR(0, 202, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "levenshtein") < 0)) __PYX_ERR(0, 199, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "levenshtein") < 0)) __PYX_ERR(0, 202, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_a = values[0];
     __pyx_v_b = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("levenshtein", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 199, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("levenshtein", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 202, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pydivsufsort.stringalg.levenshtein", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_16levenshtein(__pyx_self, __pyx_v_a, __pyx_v_b);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_18levenshtein(__pyx_self, __pyx_v_a, __pyx_v_b);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_16levenshtein(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_a, PyObject *__pyx_v_b) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_18levenshtein(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_a, PyObject *__pyx_v_b) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_t_5;
@@ -26602,141 +26743,141 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("levenshtein", 0);
   __Pyx_INCREF(__pyx_v_a);
   __Pyx_INCREF(__pyx_v_b);
 
-  /* "pydivsufsort/stringalg.pyx":200
+  /* "pydivsufsort/stringalg.pyx":203
  * 
  * def levenshtein(a, b):
  *     a = handle_input(a)             # <<<<<<<<<<<<<<
  *     b = handle_input(b)
  *     if isinstance(a, bytes):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_handle_input); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 200, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_handle_input); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 203, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_a) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_a);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 200, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 203, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF_SET(__pyx_v_a, __pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pydivsufsort/stringalg.pyx":201
+  /* "pydivsufsort/stringalg.pyx":204
  * def levenshtein(a, b):
  *     a = handle_input(a)
  *     b = handle_input(b)             # <<<<<<<<<<<<<<
  *     if isinstance(a, bytes):
  *         # tofix
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_handle_input); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 201, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_handle_input); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 204, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_b) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_b);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 204, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF_SET(__pyx_v_b, __pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pydivsufsort/stringalg.pyx":202
+  /* "pydivsufsort/stringalg.pyx":205
  *     a = handle_input(a)
  *     b = handle_input(b)
  *     if isinstance(a, bytes):             # <<<<<<<<<<<<<<
  *         # tofix
  *         a = bytearray(a)
  */
   __pyx_t_4 = PyBytes_Check(__pyx_v_a); 
   __pyx_t_5 = (__pyx_t_4 != 0);
   if (__pyx_t_5) {
 
-    /* "pydivsufsort/stringalg.pyx":204
+    /* "pydivsufsort/stringalg.pyx":207
  *     if isinstance(a, bytes):
  *         # tofix
  *         a = bytearray(a)             # <<<<<<<<<<<<<<
  *     if isinstance(b, bytes):
  *         # tofix
  */
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyByteArray_Type)), __pyx_v_a); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 204, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyByteArray_Type)), __pyx_v_a); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 207, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF_SET(__pyx_v_a, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "pydivsufsort/stringalg.pyx":202
+    /* "pydivsufsort/stringalg.pyx":205
  *     a = handle_input(a)
  *     b = handle_input(b)
  *     if isinstance(a, bytes):             # <<<<<<<<<<<<<<
  *         # tofix
  *         a = bytearray(a)
  */
   }
 
-  /* "pydivsufsort/stringalg.pyx":205
+  /* "pydivsufsort/stringalg.pyx":208
  *         # tofix
  *         a = bytearray(a)
  *     if isinstance(b, bytes):             # <<<<<<<<<<<<<<
  *         # tofix
  *         b = bytearray(b)
  */
   __pyx_t_5 = PyBytes_Check(__pyx_v_b); 
   __pyx_t_4 = (__pyx_t_5 != 0);
   if (__pyx_t_4) {
 
-    /* "pydivsufsort/stringalg.pyx":207
+    /* "pydivsufsort/stringalg.pyx":210
  *     if isinstance(b, bytes):
  *         # tofix
  *         b = bytearray(b)             # <<<<<<<<<<<<<<
  *     return _levenshtein(a, b)
  * 
  */
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyByteArray_Type)), __pyx_v_b); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 207, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyByteArray_Type)), __pyx_v_b); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 210, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF_SET(__pyx_v_b, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "pydivsufsort/stringalg.pyx":205
+    /* "pydivsufsort/stringalg.pyx":208
  *         # tofix
  *         a = bytearray(a)
  *     if isinstance(b, bytes):             # <<<<<<<<<<<<<<
  *         # tofix
  *         b = bytearray(b)
  */
   }
 
-  /* "pydivsufsort/stringalg.pyx":208
+  /* "pydivsufsort/stringalg.pyx":211
  *         # tofix
  *         b = bytearray(b)
  *     return _levenshtein(a, b)             # <<<<<<<<<<<<<<
  * 
  * from libcpp.pair cimport pair
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_levenshtein); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 208, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_levenshtein); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 211, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -26745,49 +26886,49 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_a, __pyx_v_b};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 208, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 211, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_a, __pyx_v_b};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 208, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 211, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   {
-    __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 208, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 211, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     if (__pyx_t_3) {
       __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_3); __pyx_t_3 = NULL;
     }
     __Pyx_INCREF(__pyx_v_a);
     __Pyx_GIVEREF(__pyx_v_a);
     PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_v_a);
     __Pyx_INCREF(__pyx_v_b);
     __Pyx_GIVEREF(__pyx_v_b);
     PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_v_b);
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 208, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 211, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pydivsufsort/stringalg.pyx":199
+  /* "pydivsufsort/stringalg.pyx":202
  * 
  * 
  * def levenshtein(a, b):             # <<<<<<<<<<<<<<
  *     a = handle_input(a)
  *     b = handle_input(b)
  */
 
@@ -26803,27 +26944,27 @@
   __Pyx_XDECREF(__pyx_v_a);
   __Pyx_XDECREF(__pyx_v_b);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pydivsufsort/stringalg.pyx":220
+/* "pydivsufsort/stringalg.pyx":223
  * 
  * 
  * def most_frequent_substrings(             # <<<<<<<<<<<<<<
  *     np.ndarray[sa_t, ndim=1] lcp not None,
  *     sa_t length,
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_12pydivsufsort_9stringalg_19most_frequent_substrings(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_12pydivsufsort_9stringalg_18most_frequent_substrings[] = "\n    Parameters\n    ----------\n\n    lcp : np.ndarray\n        LCP array\n    length : int\n        length of the substrings to compare\n    limit : int (default 0)\n        number of substrings to extract, 0 for all of them\n    minimum_count : int (default 1)\n        ignore the substrings that occur less than `minimum_count` times\n    \n\n    Returns\n    -------\n    positions : np.ndarray\n        position in the suffix array\n    counts : np.ndarray\n        number of occurrences, decreasing\n    ";
-static PyMethodDef __pyx_mdef_12pydivsufsort_9stringalg_19most_frequent_substrings = {"most_frequent_substrings", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_12pydivsufsort_9stringalg_19most_frequent_substrings, METH_VARARGS|METH_KEYWORDS, __pyx_doc_12pydivsufsort_9stringalg_18most_frequent_substrings};
-static PyObject *__pyx_pw_12pydivsufsort_9stringalg_19most_frequent_substrings(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_12pydivsufsort_9stringalg_21most_frequent_substrings(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_12pydivsufsort_9stringalg_20most_frequent_substrings[] = "\n    Find the most frequent substrings of a given length in a string.\n    If `limit` is not 0, only the `limit` most frequent substrings are returned.\n    If `minimum_count` is not 1, only the substrings that occur at least `minimum_count` times are returned.\n\n    Parameters\n    ----------\n\n    lcp : np.ndarray\n        LCP array\n    length : int\n        length of the substrings to compare\n    limit : int (default 0)\n        number of substrings to extract, 0 for all of them\n    minimum_count : int (default 1)\n        ignore the substrings that occur less than `minimum_count` times\n    \n\n    Returns\n    -------\n    positions : np.ndarray\n        position in the suffix array\n    counts : np.ndarray\n        number of occurrences, decreasing\n    ";
+static PyMethodDef __pyx_mdef_12pydivsufsort_9stringalg_21most_frequent_substrings = {"most_frequent_substrings", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_12pydivsufsort_9stringalg_21most_frequent_substrings, METH_VARARGS|METH_KEYWORDS, __pyx_doc_12pydivsufsort_9stringalg_20most_frequent_substrings};
+static PyObject *__pyx_pw_12pydivsufsort_9stringalg_21most_frequent_substrings(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_signatures = 0;
   PyObject *__pyx_v_args = 0;
   PyObject *__pyx_v_kwargs = 0;
   CYTHON_UNUSED PyObject *__pyx_v_defaults = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -26855,15 +26996,15 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_signatures)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_args)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fused_cpdef", 1, 4, 4, 1); __PYX_ERR(0, 220, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fused_cpdef", 1, 4, 4, 1); __PYX_ERR(0, 223, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_kwargs);
           if (value) { values[2] = value; kw_args--; }
         }
@@ -26871,15 +27012,15 @@
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_defaults);
           if (value) { values[3] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fused_cpdef") < 0)) __PYX_ERR(0, 220, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fused_cpdef") < 0)) __PYX_ERR(0, 223, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 4) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
@@ -26888,28 +27029,28 @@
     __pyx_v_signatures = values[0];
     __pyx_v_args = values[1];
     __pyx_v_kwargs = values[2];
     __pyx_v_defaults = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__pyx_fused_cpdef", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 220, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__pyx_fused_cpdef", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 223, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pydivsufsort.stringalg.__pyx_fused_cpdef", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_18most_frequent_substrings(__pyx_self, __pyx_v_signatures, __pyx_v_args, __pyx_v_kwargs, __pyx_v_defaults);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_20most_frequent_substrings(__pyx_self, __pyx_v_signatures, __pyx_v_args, __pyx_v_kwargs, __pyx_v_defaults);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_18most_frequent_substrings(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_signatures, PyObject *__pyx_v_args, PyObject *__pyx_v_kwargs, CYTHON_UNUSED PyObject *__pyx_v_defaults) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_20most_frequent_substrings(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_signatures, PyObject *__pyx_v_args, PyObject *__pyx_v_kwargs, CYTHON_UNUSED PyObject *__pyx_v_defaults) {
   PyObject *__pyx_v_dest_sig = NULL;
   Py_ssize_t __pyx_v_i;
   PyTypeObject *__pyx_v_ndarray = 0;
   __Pyx_memviewslice __pyx_v_memslice;
   Py_ssize_t __pyx_v_itemsize;
   int __pyx_v_dtype_signed;
   char __pyx_v_kind;
@@ -26944,53 +27085,53 @@
   Py_ssize_t __pyx_t_17;
   int __pyx_t_18;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("most_frequent_substrings", 0);
   __Pyx_INCREF(__pyx_v_kwargs);
-  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   PyList_SET_ITEM(__pyx_t_1, 0, Py_None);
   __pyx_v_dest_sig = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_v_kwargs != Py_None);
   __pyx_t_4 = (__pyx_t_3 != 0);
   if (__pyx_t_4) {
   } else {
     __pyx_t_2 = __pyx_t_4;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_kwargs); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_kwargs); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 223, __pyx_L1_error)
   __pyx_t_3 = ((!__pyx_t_4) != 0);
   __pyx_t_2 = __pyx_t_3;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_2) {
     __Pyx_INCREF(Py_None);
     __Pyx_DECREF_SET(__pyx_v_kwargs, Py_None);
   }
-  __pyx_t_1 = ((PyObject *)__Pyx_ImportNumPyArrayTypeIfAvailable()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__Pyx_ImportNumPyArrayTypeIfAvailable()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_ndarray = ((PyTypeObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   __pyx_v_itemsize = -1L;
   __pyx_v____pyx_int32_t_is_signed = (!((((__pyx_t_5numpy_int32_t)-1L) > 0) != 0));
   __pyx_v____pyx_int64_t_is_signed = (!((((__pyx_t_5numpy_int64_t)-1L) > 0) != 0));
   if (unlikely(__pyx_v_args == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 220, __pyx_L1_error)
+    __PYX_ERR(0, 223, __pyx_L1_error)
   }
-  __pyx_t_5 = PyTuple_GET_SIZE(((PyObject*)__pyx_v_args)); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_GET_SIZE(((PyObject*)__pyx_v_args)); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 223, __pyx_L1_error)
   __pyx_t_2 = ((0 < __pyx_t_5) != 0);
   if (__pyx_t_2) {
     if (unlikely(__pyx_v_args == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 220, __pyx_L1_error)
+      __PYX_ERR(0, 223, __pyx_L1_error)
     }
     __pyx_t_1 = PyTuple_GET_ITEM(((PyObject*)__pyx_v_args), 0);
     __Pyx_INCREF(__pyx_t_1);
     __pyx_v_arg = __pyx_t_1;
     __pyx_t_1 = 0;
     goto __pyx_L6;
   }
@@ -26999,85 +27140,85 @@
   if (__pyx_t_4) {
   } else {
     __pyx_t_2 = __pyx_t_4;
     goto __pyx_L7_bool_binop_done;
   }
   if (unlikely(__pyx_v_kwargs == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-    __PYX_ERR(0, 220, __pyx_L1_error)
+    __PYX_ERR(0, 223, __pyx_L1_error)
   }
-  __pyx_t_4 = (__Pyx_PyDict_ContainsTF(__pyx_n_s_lcp, ((PyObject*)__pyx_v_kwargs), Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_t_4 = (__Pyx_PyDict_ContainsTF(__pyx_n_s_lcp, ((PyObject*)__pyx_v_kwargs), Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 223, __pyx_L1_error)
   __pyx_t_3 = (__pyx_t_4 != 0);
   __pyx_t_2 = __pyx_t_3;
   __pyx_L7_bool_binop_done:;
   if (__pyx_t_2) {
     if (unlikely(__pyx_v_kwargs == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 220, __pyx_L1_error)
+      __PYX_ERR(0, 223, __pyx_L1_error)
     }
-    __pyx_t_1 = __Pyx_PyDict_GetItem(((PyObject*)__pyx_v_kwargs), __pyx_n_s_lcp); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 220, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyDict_GetItem(((PyObject*)__pyx_v_kwargs), __pyx_n_s_lcp); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 223, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_arg = __pyx_t_1;
     __pyx_t_1 = 0;
     goto __pyx_L6;
   }
   /*else*/ {
     if (unlikely(__pyx_v_args == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-      __PYX_ERR(0, 220, __pyx_L1_error)
+      __PYX_ERR(0, 223, __pyx_L1_error)
     }
-    __pyx_t_5 = PyTuple_GET_SIZE(((PyObject*)__pyx_v_args)); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 220, __pyx_L1_error)
-    __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 220, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_GET_SIZE(((PyObject*)__pyx_v_args)); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 223, __pyx_L1_error)
+    __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 223, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_6 = PyTuple_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 220, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 223, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_INCREF(__pyx_int_2);
     __Pyx_GIVEREF(__pyx_int_2);
     PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_int_2);
     __Pyx_INCREF(__pyx_n_s_s);
     __Pyx_GIVEREF(__pyx_n_s_s);
     PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_n_s_s);
     __Pyx_GIVEREF(__pyx_t_1);
     PyTuple_SET_ITEM(__pyx_t_6, 2, __pyx_t_1);
     __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyString_Format(__pyx_kp_s_Expected_at_least_d_argument_s_g, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 220, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyString_Format(__pyx_kp_s_Expected_at_least_d_argument_s_g, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 223, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 220, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 223, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_6, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __PYX_ERR(0, 220, __pyx_L1_error)
+    __PYX_ERR(0, 223, __pyx_L1_error)
   }
   __pyx_L6:;
   while (1) {
     __pyx_t_2 = (__pyx_v_ndarray != ((PyTypeObject*)Py_None));
     __pyx_t_3 = (__pyx_t_2 != 0);
     if (__pyx_t_3) {
       __pyx_t_3 = __Pyx_TypeCheck(__pyx_v_arg, __pyx_v_ndarray); 
       __pyx_t_2 = (__pyx_t_3 != 0);
       if (__pyx_t_2) {
-        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_dtype); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 220, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_dtype); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 223, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         __pyx_v_dtype = __pyx_t_6;
         __pyx_t_6 = 0;
         goto __pyx_L12;
       }
       __pyx_t_2 = __pyx_memoryview_check(__pyx_v_arg); 
       __pyx_t_3 = (__pyx_t_2 != 0);
       if (__pyx_t_3) {
-        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_base); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 220, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_base); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 223, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         __pyx_v_arg_base = __pyx_t_6;
         __pyx_t_6 = 0;
         __pyx_t_3 = __Pyx_TypeCheck(__pyx_v_arg_base, __pyx_v_ndarray); 
         __pyx_t_2 = (__pyx_t_3 != 0);
         if (__pyx_t_2) {
-          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg_base, __pyx_n_s_dtype); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 220, __pyx_L1_error)
+          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg_base, __pyx_n_s_dtype); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 223, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
           __pyx_v_dtype = __pyx_t_6;
           __pyx_t_6 = 0;
           goto __pyx_L13;
         }
         /*else*/ {
           __Pyx_INCREF(Py_None);
@@ -27091,72 +27232,72 @@
         __pyx_v_dtype = Py_None;
       }
       __pyx_L12:;
       __pyx_v_itemsize = -1L;
       __pyx_t_2 = (__pyx_v_dtype != Py_None);
       __pyx_t_3 = (__pyx_t_2 != 0);
       if (__pyx_t_3) {
-        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_dtype, __pyx_n_s_itemsize); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 220, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_dtype, __pyx_n_s_itemsize); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 223, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
-        __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 220, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 223, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __pyx_v_itemsize = __pyx_t_5;
-        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_dtype, __pyx_n_s_kind); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 220, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_dtype, __pyx_n_s_kind); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 223, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
-        __pyx_t_7 = __Pyx_PyObject_Ord(__pyx_t_6); if (unlikely(__pyx_t_7 == ((long)(long)(Py_UCS4)-1))) __PYX_ERR(0, 220, __pyx_L1_error)
+        __pyx_t_7 = __Pyx_PyObject_Ord(__pyx_t_6); if (unlikely(__pyx_t_7 == ((long)(long)(Py_UCS4)-1))) __PYX_ERR(0, 223, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __pyx_v_kind = __pyx_t_7;
         __pyx_v_dtype_signed = (__pyx_v_kind == 'i');
         switch (__pyx_v_kind) {
           case 'i':
           case 'u':
           __pyx_t_2 = (((sizeof(__pyx_t_5numpy_int32_t)) == __pyx_v_itemsize) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L16_bool_binop_done;
           }
-          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 220, __pyx_L1_error)
+          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 223, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
-          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 220, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 223, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           __pyx_t_2 = ((((Py_ssize_t)__pyx_t_5) == 1) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L16_bool_binop_done;
           }
           __pyx_t_2 = ((!((__pyx_v____pyx_int32_t_is_signed ^ __pyx_v_dtype_signed) != 0)) != 0);
           __pyx_t_3 = __pyx_t_2;
           __pyx_L16_bool_binop_done:;
           if (__pyx_t_3) {
-            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int32_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 220, __pyx_L1_error)
+            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int32_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 223, __pyx_L1_error)
             goto __pyx_L10_break;
           }
           __pyx_t_2 = (((sizeof(__pyx_t_5numpy_int64_t)) == __pyx_v_itemsize) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L20_bool_binop_done;
           }
-          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 220, __pyx_L1_error)
+          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 223, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
-          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 220, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 223, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           __pyx_t_2 = ((((Py_ssize_t)__pyx_t_5) == 1) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L20_bool_binop_done;
           }
           __pyx_t_2 = ((!((__pyx_v____pyx_int64_t_is_signed ^ __pyx_v_dtype_signed) != 0)) != 0);
           __pyx_t_3 = __pyx_t_2;
           __pyx_L20_bool_binop_done:;
           if (__pyx_t_3) {
-            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int64_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 220, __pyx_L1_error)
+            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int64_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 223, __pyx_L1_error)
             goto __pyx_L10_break;
           }
           break;
           case 'f':
           break;
           case 'c':
           break;
@@ -27177,15 +27318,15 @@
     __pyx_L24_bool_binop_done:;
     if (__pyx_t_3) {
       __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_int32_t(__pyx_v_arg, 0); 
       __pyx_v_memslice = __pyx_t_8;
       __pyx_t_3 = (__pyx_v_memslice.memview != 0);
       if (__pyx_t_3) {
         __PYX_XDEC_MEMVIEW((&__pyx_v_memslice), 1); 
-        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int32_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 220, __pyx_L1_error)
+        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int32_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 223, __pyx_L1_error)
         goto __pyx_L10_break;
       }
       /*else*/ {
         PyErr_Clear(); 
       }
     }
     __pyx_t_2 = ((__pyx_v_itemsize == -1L) != 0);
@@ -27199,100 +27340,100 @@
     __pyx_L28_bool_binop_done:;
     if (__pyx_t_3) {
       __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_int64_t(__pyx_v_arg, 0); 
       __pyx_v_memslice = __pyx_t_8;
       __pyx_t_3 = (__pyx_v_memslice.memview != 0);
       if (__pyx_t_3) {
         __PYX_XDEC_MEMVIEW((&__pyx_v_memslice), 1); 
-        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int64_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 220, __pyx_L1_error)
+        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int64_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 223, __pyx_L1_error)
         goto __pyx_L10_break;
       }
       /*else*/ {
         PyErr_Clear(); 
       }
     }
-    if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, Py_None, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 220, __pyx_L1_error)
+    if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, Py_None, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 223, __pyx_L1_error)
     goto __pyx_L10_break;
   }
   __pyx_L10_break:;
-  __pyx_t_6 = PyList_New(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_t_6 = PyList_New(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_v_candidates = ((PyObject*)__pyx_t_6);
   __pyx_t_6 = 0;
   __pyx_t_5 = 0;
   if (unlikely(__pyx_v_signatures == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-    __PYX_ERR(0, 220, __pyx_L1_error)
+    __PYX_ERR(0, 223, __pyx_L1_error)
   }
-  __pyx_t_1 = __Pyx_dict_iterator(((PyObject*)__pyx_v_signatures), 1, ((PyObject *)NULL), (&__pyx_t_9), (&__pyx_t_10)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_dict_iterator(((PyObject*)__pyx_v_signatures), 1, ((PyObject *)NULL), (&__pyx_t_9), (&__pyx_t_10)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_6);
   __pyx_t_6 = __pyx_t_1;
   __pyx_t_1 = 0;
   while (1) {
     __pyx_t_11 = __Pyx_dict_iter_next(__pyx_t_6, __pyx_t_9, &__pyx_t_5, &__pyx_t_1, NULL, NULL, __pyx_t_10);
     if (unlikely(__pyx_t_11 == 0)) break;
-    if (unlikely(__pyx_t_11 == -1)) __PYX_ERR(0, 220, __pyx_L1_error)
+    if (unlikely(__pyx_t_11 == -1)) __PYX_ERR(0, 223, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_XDECREF_SET(__pyx_v_sig, __pyx_t_1);
     __pyx_t_1 = 0;
     __pyx_v_match_found = 0;
-    __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_v_sig, __pyx_n_s_strip); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 220, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_v_sig, __pyx_n_s_strip); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 223, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_13);
     __pyx_t_14 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_13))) {
       __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_13);
       if (likely(__pyx_t_14)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_13);
         __Pyx_INCREF(__pyx_t_14);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_13, function);
       }
     }
     __pyx_t_12 = (__pyx_t_14) ? __Pyx_PyObject_Call2Args(__pyx_t_13, __pyx_t_14, __pyx_kp_s__2) : __Pyx_PyObject_CallOneArg(__pyx_t_13, __pyx_kp_s__2);
     __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
-    if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 220, __pyx_L1_error)
+    if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 223, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_12);
     __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-    __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_split); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 220, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_split); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 223, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_13);
     __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
     __pyx_t_12 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_13))) {
       __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_13);
       if (likely(__pyx_t_12)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_13);
         __Pyx_INCREF(__pyx_t_12);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_13, function);
       }
     }
     __pyx_t_1 = (__pyx_t_12) ? __Pyx_PyObject_Call2Args(__pyx_t_13, __pyx_t_12, __pyx_kp_s__3) : __Pyx_PyObject_CallOneArg(__pyx_t_13, __pyx_kp_s__3);
     __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 220, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 223, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
     __Pyx_XDECREF_SET(__pyx_v_src_sig, __pyx_t_1);
     __pyx_t_1 = 0;
-    __pyx_t_15 = PyList_GET_SIZE(__pyx_v_dest_sig); if (unlikely(__pyx_t_15 == ((Py_ssize_t)-1))) __PYX_ERR(0, 220, __pyx_L1_error)
+    __pyx_t_15 = PyList_GET_SIZE(__pyx_v_dest_sig); if (unlikely(__pyx_t_15 == ((Py_ssize_t)-1))) __PYX_ERR(0, 223, __pyx_L1_error)
     __pyx_t_16 = __pyx_t_15;
     for (__pyx_t_17 = 0; __pyx_t_17 < __pyx_t_16; __pyx_t_17+=1) {
       __pyx_v_i = __pyx_t_17;
       __pyx_t_1 = PyList_GET_ITEM(__pyx_v_dest_sig, __pyx_v_i);
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_XDECREF_SET(__pyx_v_dst_type, __pyx_t_1);
       __pyx_t_1 = 0;
       __pyx_t_3 = (__pyx_v_dst_type != Py_None);
       __pyx_t_2 = (__pyx_t_3 != 0);
       if (__pyx_t_2) {
-        __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_src_sig, __pyx_v_i, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 220, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_src_sig, __pyx_v_i, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 223, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_13 = PyObject_RichCompare(__pyx_t_1, __pyx_v_dst_type, Py_EQ); __Pyx_XGOTREF(__pyx_t_13); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 220, __pyx_L1_error)
+        __pyx_t_13 = PyObject_RichCompare(__pyx_t_1, __pyx_v_dst_type, Py_EQ); __Pyx_XGOTREF(__pyx_t_13); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 223, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_13); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 220, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_13); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 223, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
         if (__pyx_t_2) {
           __pyx_v_match_found = 1;
           goto __pyx_L36;
         }
         /*else*/ {
           __pyx_v_match_found = 0;
@@ -27300,43 +27441,43 @@
         }
         __pyx_L36:;
       }
     }
     __pyx_L34_break:;
     __pyx_t_2 = (__pyx_v_match_found != 0);
     if (__pyx_t_2) {
-      __pyx_t_18 = __Pyx_PyList_Append(__pyx_v_candidates, __pyx_v_sig); if (unlikely(__pyx_t_18 == ((int)-1))) __PYX_ERR(0, 220, __pyx_L1_error)
+      __pyx_t_18 = __Pyx_PyList_Append(__pyx_v_candidates, __pyx_v_sig); if (unlikely(__pyx_t_18 == ((int)-1))) __PYX_ERR(0, 223, __pyx_L1_error)
     }
   }
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_2 = (PyList_GET_SIZE(__pyx_v_candidates) != 0);
   __pyx_t_3 = ((!__pyx_t_2) != 0);
   if (__pyx_t_3) {
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 220, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 223, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_Raise(__pyx_t_6, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __PYX_ERR(0, 220, __pyx_L1_error)
+    __PYX_ERR(0, 223, __pyx_L1_error)
   }
-  __pyx_t_9 = PyList_GET_SIZE(__pyx_v_candidates); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_t_9 = PyList_GET_SIZE(__pyx_v_candidates); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 223, __pyx_L1_error)
   __pyx_t_3 = ((__pyx_t_9 > 1) != 0);
   if (__pyx_t_3) {
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 220, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 223, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_Raise(__pyx_t_6, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __PYX_ERR(0, 220, __pyx_L1_error)
+    __PYX_ERR(0, 223, __pyx_L1_error)
   }
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     if (unlikely(__pyx_v_signatures == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 220, __pyx_L1_error)
+      __PYX_ERR(0, 223, __pyx_L1_error)
     }
-    __pyx_t_6 = __Pyx_PyDict_GetItem(((PyObject*)__pyx_v_signatures), PyList_GET_ITEM(__pyx_v_candidates, 0)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 220, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyDict_GetItem(((PyObject*)__pyx_v_signatures), PyList_GET_ITEM(__pyx_v_candidates, 0)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 223, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_r = __pyx_t_6;
     __pyx_t_6 = 0;
     goto __pyx_L0;
   }
 
   /* function exit code */
@@ -27360,38 +27501,38 @@
   __Pyx_XDECREF(__pyx_v_dst_type);
   __Pyx_XDECREF(__pyx_v_kwargs);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_132__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_134__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__defaults__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_npy_int32(__Pyx_CyFunction_Defaults(__pyx_defaults2, __pyx_self)->__pyx_arg_limit); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_npy_int32(__Pyx_CyFunction_Defaults(__pyx_defaults2, __pyx_self)->__pyx_arg_limit); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyInt_From_npy_int32(__Pyx_CyFunction_Defaults(__pyx_defaults2, __pyx_self)->__pyx_arg_minimum_count); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_npy_int32(__Pyx_CyFunction_Defaults(__pyx_defaults2, __pyx_self)->__pyx_arg_minimum_count); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_2);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   PyTuple_SET_ITEM(__pyx_t_2, 1, Py_None);
   __pyx_t_3 = 0;
@@ -27409,17 +27550,17 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_0__pyx_pw_12pydivsufsort_9stringalg_123most_frequent_substrings(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_0__pyx_mdef_12pydivsufsort_9stringalg_123most_frequent_substrings = {"__pyx_fuse_0most_frequent_substrings", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_0__pyx_pw_12pydivsufsort_9stringalg_123most_frequent_substrings, METH_VARARGS|METH_KEYWORDS, __pyx_doc_12pydivsufsort_9stringalg_18most_frequent_substrings};
-static PyObject *__pyx_fuse_0__pyx_pw_12pydivsufsort_9stringalg_123most_frequent_substrings(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_0__pyx_pw_12pydivsufsort_9stringalg_125most_frequent_substrings(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_0__pyx_mdef_12pydivsufsort_9stringalg_125most_frequent_substrings = {"__pyx_fuse_0most_frequent_substrings", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_0__pyx_pw_12pydivsufsort_9stringalg_125most_frequent_substrings, METH_VARARGS|METH_KEYWORDS, __pyx_doc_12pydivsufsort_9stringalg_20most_frequent_substrings};
+static PyObject *__pyx_fuse_0__pyx_pw_12pydivsufsort_9stringalg_125most_frequent_substrings(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyArrayObject *__pyx_v_lcp = 0;
   __pyx_t_5numpy_int32_t __pyx_v_length;
   __pyx_t_5numpy_int32_t __pyx_v_limit;
   __pyx_t_5numpy_int32_t __pyx_v_minimum_count;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -27450,15 +27591,15 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_lcp)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_length)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("most_frequent_substrings", 0, 2, 4, 1); __PYX_ERR(0, 220, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("most_frequent_substrings", 0, 2, 4, 1); __PYX_ERR(0, 223, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_limit);
           if (value) { values[2] = value; kw_args--; }
         }
@@ -27466,62 +27607,62 @@
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_minimum_count);
           if (value) { values[3] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "most_frequent_substrings") < 0)) __PYX_ERR(0, 220, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "most_frequent_substrings") < 0)) __PYX_ERR(0, 223, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_lcp = ((PyArrayObject *)values[0]);
-    __pyx_v_length = __Pyx_PyInt_As_npy_int32(values[1]); if (unlikely((__pyx_v_length == ((npy_int32)-1)) && PyErr_Occurred())) __PYX_ERR(0, 222, __pyx_L3_error)
+    __pyx_v_length = __Pyx_PyInt_As_npy_int32(values[1]); if (unlikely((__pyx_v_length == ((npy_int32)-1)) && PyErr_Occurred())) __PYX_ERR(0, 225, __pyx_L3_error)
     if (values[2]) {
-      __pyx_v_limit = __Pyx_PyInt_As_npy_int32(values[2]); if (unlikely((__pyx_v_limit == ((npy_int32)-1)) && PyErr_Occurred())) __PYX_ERR(0, 223, __pyx_L3_error)
+      __pyx_v_limit = __Pyx_PyInt_As_npy_int32(values[2]); if (unlikely((__pyx_v_limit == ((npy_int32)-1)) && PyErr_Occurred())) __PYX_ERR(0, 226, __pyx_L3_error)
     } else {
       __pyx_v_limit = __pyx_dynamic_args->__pyx_arg_limit;
     }
     if (values[3]) {
-      __pyx_v_minimum_count = __Pyx_PyInt_As_npy_int32(values[3]); if (unlikely((__pyx_v_minimum_count == ((npy_int32)-1)) && PyErr_Occurred())) __PYX_ERR(0, 224, __pyx_L3_error)
+      __pyx_v_minimum_count = __Pyx_PyInt_As_npy_int32(values[3]); if (unlikely((__pyx_v_minimum_count == ((npy_int32)-1)) && PyErr_Occurred())) __PYX_ERR(0, 227, __pyx_L3_error)
     } else {
       __pyx_v_minimum_count = __pyx_dynamic_args->__pyx_arg_minimum_count;
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("most_frequent_substrings", 0, 2, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 220, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("most_frequent_substrings", 0, 2, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 223, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pydivsufsort.stringalg.most_frequent_substrings", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_lcp), __pyx_ptype_5numpy_ndarray, 0, "lcp", 0))) __PYX_ERR(0, 221, __pyx_L1_error)
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_122most_frequent_substrings(__pyx_self, __pyx_v_lcp, __pyx_v_length, __pyx_v_limit, __pyx_v_minimum_count);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_lcp), __pyx_ptype_5numpy_ndarray, 0, "lcp", 0))) __PYX_ERR(0, 224, __pyx_L1_error)
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_124most_frequent_substrings(__pyx_self, __pyx_v_lcp, __pyx_v_length, __pyx_v_limit, __pyx_v_minimum_count);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_122most_frequent_substrings(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_lcp, __pyx_t_5numpy_int32_t __pyx_v_length, __pyx_t_5numpy_int32_t __pyx_v_limit, __pyx_t_5numpy_int32_t __pyx_v_minimum_count) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_124most_frequent_substrings(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_lcp, __pyx_t_5numpy_int32_t __pyx_v_length, __pyx_t_5numpy_int32_t __pyx_v_limit, __pyx_t_5numpy_int32_t __pyx_v_minimum_count) {
   __pyx_t_5numpy_int32_t __pyx_v_n;
   __pyx_t_5numpy_int32_t __pyx_v_i;
   __pyx_t_5numpy_int32_t __pyx_v_cur;
   __pyx_t_5numpy_int32_t __pyx_v_cur_count;
   std::vector<std::pair<__pyx_t_5numpy_int32_t,__pyx_t_5numpy_int32_t> >  __pyx_v_count;
   PyArrayObject *__pyx_v_pos = 0;
   PyArrayObject *__pyx_v_cnt = 0;
@@ -27564,256 +27705,256 @@
   __pyx_pybuffernd_cnt.rcbuffer = &__pyx_pybuffer_cnt;
   __pyx_pybuffer_lcp.pybuffer.buf = NULL;
   __pyx_pybuffer_lcp.refcount = 0;
   __pyx_pybuffernd_lcp.data = NULL;
   __pyx_pybuffernd_lcp.rcbuffer = &__pyx_pybuffer_lcp;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_lcp.rcbuffer->pybuffer, (PyObject*)__pyx_v_lcp, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 220, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_lcp.rcbuffer->pybuffer, (PyObject*)__pyx_v_lcp, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 223, __pyx_L1_error)
   }
   __pyx_pybuffernd_lcp.diminfo[0].strides = __pyx_pybuffernd_lcp.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_lcp.diminfo[0].shape = __pyx_pybuffernd_lcp.rcbuffer->pybuffer.shape[0];
 
-  /* "pydivsufsort/stringalg.pyx":253
+  /* "pydivsufsort/stringalg.pyx":260
  *     cdef vector[pair[sa_t, sa_t]] count
  * 
  *     if minimum_count < 1:             # <<<<<<<<<<<<<<
  *         minimum_count = 1
  * 
  */
   __pyx_t_1 = ((__pyx_v_minimum_count < 1) != 0);
   if (__pyx_t_1) {
 
-    /* "pydivsufsort/stringalg.pyx":254
+    /* "pydivsufsort/stringalg.pyx":261
  * 
  *     if minimum_count < 1:
  *         minimum_count = 1             # <<<<<<<<<<<<<<
  * 
  *     n = len(lcp)
  */
     __pyx_v_minimum_count = 1;
 
-    /* "pydivsufsort/stringalg.pyx":253
+    /* "pydivsufsort/stringalg.pyx":260
  *     cdef vector[pair[sa_t, sa_t]] count
  * 
  *     if minimum_count < 1:             # <<<<<<<<<<<<<<
  *         minimum_count = 1
  * 
  */
   }
 
-  /* "pydivsufsort/stringalg.pyx":256
+  /* "pydivsufsort/stringalg.pyx":263
  *         minimum_count = 1
  * 
  *     n = len(lcp)             # <<<<<<<<<<<<<<
  *     cur = 0
  *     cur_count = 1
  */
-  __pyx_t_2 = PyObject_Length(((PyObject *)__pyx_v_lcp)); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 256, __pyx_L1_error)
+  __pyx_t_2 = PyObject_Length(((PyObject *)__pyx_v_lcp)); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 263, __pyx_L1_error)
   __pyx_v_n = __pyx_t_2;
 
-  /* "pydivsufsort/stringalg.pyx":257
+  /* "pydivsufsort/stringalg.pyx":264
  * 
  *     n = len(lcp)
  *     cur = 0             # <<<<<<<<<<<<<<
  *     cur_count = 1
  *     for i in range(n-1):
  */
   __pyx_v_cur = 0;
 
-  /* "pydivsufsort/stringalg.pyx":258
+  /* "pydivsufsort/stringalg.pyx":265
  *     n = len(lcp)
  *     cur = 0
  *     cur_count = 1             # <<<<<<<<<<<<<<
  *     for i in range(n-1):
  *         if lcp[i] >= length:
  */
   __pyx_v_cur_count = 1;
 
-  /* "pydivsufsort/stringalg.pyx":259
+  /* "pydivsufsort/stringalg.pyx":266
  *     cur = 0
  *     cur_count = 1
  *     for i in range(n-1):             # <<<<<<<<<<<<<<
  *         if lcp[i] >= length:
  *             cur_count += 1
  */
   __pyx_t_3 = (__pyx_v_n - 1);
   __pyx_t_4 = __pyx_t_3;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
     __pyx_v_i = __pyx_t_5;
 
-    /* "pydivsufsort/stringalg.pyx":260
+    /* "pydivsufsort/stringalg.pyx":267
  *     cur_count = 1
  *     for i in range(n-1):
  *         if lcp[i] >= length:             # <<<<<<<<<<<<<<
  *             cur_count += 1
  *         else:
  */
     __pyx_t_6 = __pyx_v_i;
     __pyx_t_1 = (((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_lcp.rcbuffer->pybuffer.buf, __pyx_t_6, __pyx_pybuffernd_lcp.diminfo[0].strides)) >= __pyx_v_length) != 0);
     if (__pyx_t_1) {
 
-      /* "pydivsufsort/stringalg.pyx":261
+      /* "pydivsufsort/stringalg.pyx":268
  *     for i in range(n-1):
  *         if lcp[i] >= length:
  *             cur_count += 1             # <<<<<<<<<<<<<<
  *         else:
  *             if cur_count >= minimum_count:
  */
       __pyx_v_cur_count = (__pyx_v_cur_count + 1);
 
-      /* "pydivsufsort/stringalg.pyx":260
+      /* "pydivsufsort/stringalg.pyx":267
  *     cur_count = 1
  *     for i in range(n-1):
  *         if lcp[i] >= length:             # <<<<<<<<<<<<<<
  *             cur_count += 1
  *         else:
  */
       goto __pyx_L6;
     }
 
-    /* "pydivsufsort/stringalg.pyx":263
+    /* "pydivsufsort/stringalg.pyx":270
  *             cur_count += 1
  *         else:
  *             if cur_count >= minimum_count:             # <<<<<<<<<<<<<<
  *                 count.push_back((cur_count, cur))
  *             cur = i + 1
  */
     /*else*/ {
       __pyx_t_1 = ((__pyx_v_cur_count >= __pyx_v_minimum_count) != 0);
       if (__pyx_t_1) {
 
-        /* "pydivsufsort/stringalg.pyx":264
+        /* "pydivsufsort/stringalg.pyx":271
  *         else:
  *             if cur_count >= minimum_count:
  *                 count.push_back((cur_count, cur))             # <<<<<<<<<<<<<<
  *             cur = i + 1
  *             cur_count = 1
  */
-        __pyx_t_7 = __Pyx_PyInt_From_npy_int32(__pyx_v_cur_count); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 264, __pyx_L1_error)
+        __pyx_t_7 = __Pyx_PyInt_From_npy_int32(__pyx_v_cur_count); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 271, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
-        __pyx_t_8 = __Pyx_PyInt_From_npy_int32(__pyx_v_cur); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 264, __pyx_L1_error)
+        __pyx_t_8 = __Pyx_PyInt_From_npy_int32(__pyx_v_cur); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 271, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
-        __pyx_t_9 = PyTuple_New(2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 264, __pyx_L1_error)
+        __pyx_t_9 = PyTuple_New(2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 271, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_9);
         __Pyx_GIVEREF(__pyx_t_7);
         PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_7);
         __Pyx_GIVEREF(__pyx_t_8);
         PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_t_8);
         __pyx_t_7 = 0;
         __pyx_t_8 = 0;
-        __pyx_t_10 = __pyx_convert_pair_from_py___pyx_t_5numpy_int32_t__and___pyx_t_5numpy_int32_t(__pyx_t_9); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 264, __pyx_L1_error)
+        __pyx_t_10 = __pyx_convert_pair_from_py___pyx_t_5numpy_int32_t__and___pyx_t_5numpy_int32_t(__pyx_t_9); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 271, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         try {
           __pyx_v_count.push_back(__pyx_t_10);
         } catch(...) {
           __Pyx_CppExn2PyErr();
-          __PYX_ERR(0, 264, __pyx_L1_error)
+          __PYX_ERR(0, 271, __pyx_L1_error)
         }
 
-        /* "pydivsufsort/stringalg.pyx":263
+        /* "pydivsufsort/stringalg.pyx":270
  *             cur_count += 1
  *         else:
  *             if cur_count >= minimum_count:             # <<<<<<<<<<<<<<
  *                 count.push_back((cur_count, cur))
  *             cur = i + 1
  */
       }
 
-      /* "pydivsufsort/stringalg.pyx":265
+      /* "pydivsufsort/stringalg.pyx":272
  *             if cur_count >= minimum_count:
  *                 count.push_back((cur_count, cur))
  *             cur = i + 1             # <<<<<<<<<<<<<<
  *             cur_count = 1
  *     if cur_count >= minimum_count:
  */
       __pyx_v_cur = (__pyx_v_i + 1);
 
-      /* "pydivsufsort/stringalg.pyx":266
+      /* "pydivsufsort/stringalg.pyx":273
  *                 count.push_back((cur_count, cur))
  *             cur = i + 1
  *             cur_count = 1             # <<<<<<<<<<<<<<
  *     if cur_count >= minimum_count:
  *         count.push_back((cur_count, cur))
  */
       __pyx_v_cur_count = 1;
     }
     __pyx_L6:;
   }
 
-  /* "pydivsufsort/stringalg.pyx":267
+  /* "pydivsufsort/stringalg.pyx":274
  *             cur = i + 1
  *             cur_count = 1
  *     if cur_count >= minimum_count:             # <<<<<<<<<<<<<<
  *         count.push_back((cur_count, cur))
  * 
  */
   __pyx_t_1 = ((__pyx_v_cur_count >= __pyx_v_minimum_count) != 0);
   if (__pyx_t_1) {
 
-    /* "pydivsufsort/stringalg.pyx":268
+    /* "pydivsufsort/stringalg.pyx":275
  *             cur_count = 1
  *     if cur_count >= minimum_count:
  *         count.push_back((cur_count, cur))             # <<<<<<<<<<<<<<
  * 
  *     sort(count.begin(), count.end())
  */
-    __pyx_t_9 = __Pyx_PyInt_From_npy_int32(__pyx_v_cur_count); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 268, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyInt_From_npy_int32(__pyx_v_cur_count); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 275, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
-    __pyx_t_8 = __Pyx_PyInt_From_npy_int32(__pyx_v_cur); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 268, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyInt_From_npy_int32(__pyx_v_cur); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 275, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_7 = PyTuple_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 268, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 275, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_9);
     PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_9);
     __Pyx_GIVEREF(__pyx_t_8);
     PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_t_8);
     __pyx_t_9 = 0;
     __pyx_t_8 = 0;
-    __pyx_t_10 = __pyx_convert_pair_from_py___pyx_t_5numpy_int32_t__and___pyx_t_5numpy_int32_t(__pyx_t_7); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 268, __pyx_L1_error)
+    __pyx_t_10 = __pyx_convert_pair_from_py___pyx_t_5numpy_int32_t__and___pyx_t_5numpy_int32_t(__pyx_t_7); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 275, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     try {
       __pyx_v_count.push_back(__pyx_t_10);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 268, __pyx_L1_error)
+      __PYX_ERR(0, 275, __pyx_L1_error)
     }
 
-    /* "pydivsufsort/stringalg.pyx":267
+    /* "pydivsufsort/stringalg.pyx":274
  *             cur = i + 1
  *             cur_count = 1
  *     if cur_count >= minimum_count:             # <<<<<<<<<<<<<<
  *         count.push_back((cur_count, cur))
  * 
  */
   }
 
-  /* "pydivsufsort/stringalg.pyx":270
+  /* "pydivsufsort/stringalg.pyx":277
  *         count.push_back((cur_count, cur))
  * 
  *     sort(count.begin(), count.end())             # <<<<<<<<<<<<<<
  *     reverse(count.begin(), count.end())
  *     if limit and limit < count.size():
  */
   std::sort<std::vector<std::pair<__pyx_t_5numpy_int32_t,__pyx_t_5numpy_int32_t> > ::iterator>(__pyx_v_count.begin(), __pyx_v_count.end());
 
-  /* "pydivsufsort/stringalg.pyx":271
+  /* "pydivsufsort/stringalg.pyx":278
  * 
  *     sort(count.begin(), count.end())
  *     reverse(count.begin(), count.end())             # <<<<<<<<<<<<<<
  *     if limit and limit < count.size():
  *         count.resize(limit)
  */
   try {
     std::reverse<std::vector<std::pair<__pyx_t_5numpy_int32_t,__pyx_t_5numpy_int32_t> > ::iterator>(__pyx_v_count.begin(), __pyx_v_count.end());
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 271, __pyx_L1_error)
+    __PYX_ERR(0, 278, __pyx_L1_error)
   }
 
-  /* "pydivsufsort/stringalg.pyx":272
+  /* "pydivsufsort/stringalg.pyx":279
  *     sort(count.begin(), count.end())
  *     reverse(count.begin(), count.end())
  *     if limit and limit < count.size():             # <<<<<<<<<<<<<<
  *         count.resize(limit)
  * 
  */
   __pyx_t_11 = (__pyx_v_limit != 0);
@@ -27823,190 +27964,190 @@
     goto __pyx_L10_bool_binop_done;
   }
   __pyx_t_11 = ((__pyx_v_limit < __pyx_v_count.size()) != 0);
   __pyx_t_1 = __pyx_t_11;
   __pyx_L10_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "pydivsufsort/stringalg.pyx":273
+    /* "pydivsufsort/stringalg.pyx":280
  *     reverse(count.begin(), count.end())
  *     if limit and limit < count.size():
  *         count.resize(limit)             # <<<<<<<<<<<<<<
  * 
  *     n = count.size()
  */
     try {
       __pyx_v_count.resize(__pyx_v_limit);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 273, __pyx_L1_error)
+      __PYX_ERR(0, 280, __pyx_L1_error)
     }
 
-    /* "pydivsufsort/stringalg.pyx":272
+    /* "pydivsufsort/stringalg.pyx":279
  *     sort(count.begin(), count.end())
  *     reverse(count.begin(), count.end())
  *     if limit and limit < count.size():             # <<<<<<<<<<<<<<
  *         count.resize(limit)
  * 
  */
   }
 
-  /* "pydivsufsort/stringalg.pyx":275
+  /* "pydivsufsort/stringalg.pyx":282
  *         count.resize(limit)
  * 
  *     n = count.size()             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[sa_t, ndim=1] pos = np.empty(n, dtype=lcp.dtype)
  *     cdef np.ndarray[sa_t, ndim=1] cnt = np.empty(n, dtype=lcp.dtype)
  */
   __pyx_v_n = __pyx_v_count.size();
 
-  /* "pydivsufsort/stringalg.pyx":276
+  /* "pydivsufsort/stringalg.pyx":283
  * 
  *     n = count.size()
  *     cdef np.ndarray[sa_t, ndim=1] pos = np.empty(n, dtype=lcp.dtype)             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[sa_t, ndim=1] cnt = np.empty(n, dtype=lcp.dtype)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 283, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_empty); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_empty); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 283, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_PyInt_From_npy_int32(__pyx_v_n); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_From_npy_int32(__pyx_v_n); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 283, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_9 = PyTuple_New(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __pyx_t_9 = PyTuple_New(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 283, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_GIVEREF(__pyx_t_7);
   PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_7);
   __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 283, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_12 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_lcp), __pyx_n_s_dtype); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __pyx_t_12 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_lcp), __pyx_n_s_dtype); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 283, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_dtype, __pyx_t_12) < 0) __PYX_ERR(0, 276, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_dtype, __pyx_t_12) < 0) __PYX_ERR(0, 283, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-  __pyx_t_12 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_t_9, __pyx_t_7); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __pyx_t_12 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_t_9, __pyx_t_7); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 283, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (!(likely(((__pyx_t_12) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_12, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 276, __pyx_L1_error)
+  if (!(likely(((__pyx_t_12) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_12, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 283, __pyx_L1_error)
   __pyx_t_13 = ((PyArrayObject *)__pyx_t_12);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_pos.rcbuffer->pybuffer, (PyObject*)__pyx_t_13, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_pos = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_pos.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 276, __pyx_L1_error)
+      __PYX_ERR(0, 283, __pyx_L1_error)
     } else {__pyx_pybuffernd_pos.diminfo[0].strides = __pyx_pybuffernd_pos.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_pos.diminfo[0].shape = __pyx_pybuffernd_pos.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_13 = 0;
   __pyx_v_pos = ((PyArrayObject *)__pyx_t_12);
   __pyx_t_12 = 0;
 
-  /* "pydivsufsort/stringalg.pyx":277
+  /* "pydivsufsort/stringalg.pyx":284
  *     n = count.size()
  *     cdef np.ndarray[sa_t, ndim=1] pos = np.empty(n, dtype=lcp.dtype)
  *     cdef np.ndarray[sa_t, ndim=1] cnt = np.empty(n, dtype=lcp.dtype)             # <<<<<<<<<<<<<<
  * 
  *     for i in range(n):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_np); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 277, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_np); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 284, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_empty); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 277, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_empty); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 284, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-  __pyx_t_12 = __Pyx_PyInt_From_npy_int32(__pyx_v_n); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 277, __pyx_L1_error)
+  __pyx_t_12 = __Pyx_PyInt_From_npy_int32(__pyx_v_n); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 284, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
-  __pyx_t_9 = PyTuple_New(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 277, __pyx_L1_error)
+  __pyx_t_9 = PyTuple_New(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 284, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_GIVEREF(__pyx_t_12);
   PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_12);
   __pyx_t_12 = 0;
-  __pyx_t_12 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 277, __pyx_L1_error)
+  __pyx_t_12 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 284, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_lcp), __pyx_n_s_dtype); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 277, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_lcp), __pyx_n_s_dtype); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 284, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  if (PyDict_SetItem(__pyx_t_12, __pyx_n_s_dtype, __pyx_t_8) < 0) __PYX_ERR(0, 277, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_12, __pyx_n_s_dtype, __pyx_t_8) < 0) __PYX_ERR(0, 284, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_9, __pyx_t_12); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 277, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_9, __pyx_t_12); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 284, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-  if (!(likely(((__pyx_t_8) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_8, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 277, __pyx_L1_error)
+  if (!(likely(((__pyx_t_8) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_8, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 284, __pyx_L1_error)
   __pyx_t_14 = ((PyArrayObject *)__pyx_t_8);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_cnt.rcbuffer->pybuffer, (PyObject*)__pyx_t_14, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_cnt = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_cnt.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 277, __pyx_L1_error)
+      __PYX_ERR(0, 284, __pyx_L1_error)
     } else {__pyx_pybuffernd_cnt.diminfo[0].strides = __pyx_pybuffernd_cnt.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_cnt.diminfo[0].shape = __pyx_pybuffernd_cnt.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_14 = 0;
   __pyx_v_cnt = ((PyArrayObject *)__pyx_t_8);
   __pyx_t_8 = 0;
 
-  /* "pydivsufsort/stringalg.pyx":279
+  /* "pydivsufsort/stringalg.pyx":286
  *     cdef np.ndarray[sa_t, ndim=1] cnt = np.empty(n, dtype=lcp.dtype)
  * 
  *     for i in range(n):             # <<<<<<<<<<<<<<
  *         pos[i] = count[i].second
  *         cnt[i] = count[i].first
  */
   __pyx_t_5 = __pyx_v_n;
   __pyx_t_15 = __pyx_t_5;
   for (__pyx_t_16 = 0; __pyx_t_16 < __pyx_t_15; __pyx_t_16+=1) {
     __pyx_v_i = __pyx_t_16;
 
-    /* "pydivsufsort/stringalg.pyx":280
+    /* "pydivsufsort/stringalg.pyx":287
  * 
  *     for i in range(n):
  *         pos[i] = count[i].second             # <<<<<<<<<<<<<<
  *         cnt[i] = count[i].first
  * 
  */
     __pyx_t_17 = (__pyx_v_count[__pyx_v_i]).second;
     __pyx_t_6 = __pyx_v_i;
     *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_pos.rcbuffer->pybuffer.buf, __pyx_t_6, __pyx_pybuffernd_pos.diminfo[0].strides) = __pyx_t_17;
 
-    /* "pydivsufsort/stringalg.pyx":281
+    /* "pydivsufsort/stringalg.pyx":288
  *     for i in range(n):
  *         pos[i] = count[i].second
  *         cnt[i] = count[i].first             # <<<<<<<<<<<<<<
  * 
  *     return pos, cnt
  */
     __pyx_t_17 = (__pyx_v_count[__pyx_v_i]).first;
     __pyx_t_6 = __pyx_v_i;
     *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_cnt.rcbuffer->pybuffer.buf, __pyx_t_6, __pyx_pybuffernd_cnt.diminfo[0].strides) = __pyx_t_17;
   }
 
-  /* "pydivsufsort/stringalg.pyx":283
+  /* "pydivsufsort/stringalg.pyx":290
  *         cnt[i] = count[i].first
  * 
  *     return pos, cnt             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_8 = PyTuple_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 283, __pyx_L1_error)
+  __pyx_t_8 = PyTuple_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 290, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_INCREF(((PyObject *)__pyx_v_pos));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_pos));
   PyTuple_SET_ITEM(__pyx_t_8, 0, ((PyObject *)__pyx_v_pos));
   __Pyx_INCREF(((PyObject *)__pyx_v_cnt));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_cnt));
   PyTuple_SET_ITEM(__pyx_t_8, 1, ((PyObject *)__pyx_v_cnt));
   __pyx_r = __pyx_t_8;
   __pyx_t_8 = 0;
   goto __pyx_L0;
 
-  /* "pydivsufsort/stringalg.pyx":220
+  /* "pydivsufsort/stringalg.pyx":223
  * 
  * 
  * def most_frequent_substrings(             # <<<<<<<<<<<<<<
  *     np.ndarray[sa_t, ndim=1] lcp not None,
  *     sa_t length,
  */
 
@@ -28035,38 +28176,38 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_pos);
   __Pyx_XDECREF((PyObject *)__pyx_v_cnt);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_134__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_136__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__defaults__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_npy_int64(__Pyx_CyFunction_Defaults(__pyx_defaults3, __pyx_self)->__pyx_arg_limit); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_npy_int64(__Pyx_CyFunction_Defaults(__pyx_defaults3, __pyx_self)->__pyx_arg_limit); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyInt_From_npy_int64(__Pyx_CyFunction_Defaults(__pyx_defaults3, __pyx_self)->__pyx_arg_minimum_count); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_npy_int64(__Pyx_CyFunction_Defaults(__pyx_defaults3, __pyx_self)->__pyx_arg_minimum_count); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_2);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   PyTuple_SET_ITEM(__pyx_t_2, 1, Py_None);
   __pyx_t_3 = 0;
@@ -28084,17 +28225,17 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_1__pyx_pw_12pydivsufsort_9stringalg_125most_frequent_substrings(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_1__pyx_mdef_12pydivsufsort_9stringalg_125most_frequent_substrings = {"__pyx_fuse_1most_frequent_substrings", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_1__pyx_pw_12pydivsufsort_9stringalg_125most_frequent_substrings, METH_VARARGS|METH_KEYWORDS, __pyx_doc_12pydivsufsort_9stringalg_18most_frequent_substrings};
-static PyObject *__pyx_fuse_1__pyx_pw_12pydivsufsort_9stringalg_125most_frequent_substrings(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_1__pyx_pw_12pydivsufsort_9stringalg_127most_frequent_substrings(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_1__pyx_mdef_12pydivsufsort_9stringalg_127most_frequent_substrings = {"__pyx_fuse_1most_frequent_substrings", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_1__pyx_pw_12pydivsufsort_9stringalg_127most_frequent_substrings, METH_VARARGS|METH_KEYWORDS, __pyx_doc_12pydivsufsort_9stringalg_20most_frequent_substrings};
+static PyObject *__pyx_fuse_1__pyx_pw_12pydivsufsort_9stringalg_127most_frequent_substrings(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyArrayObject *__pyx_v_lcp = 0;
   __pyx_t_5numpy_int64_t __pyx_v_length;
   __pyx_t_5numpy_int64_t __pyx_v_limit;
   __pyx_t_5numpy_int64_t __pyx_v_minimum_count;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -28125,15 +28266,15 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_lcp)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_length)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("most_frequent_substrings", 0, 2, 4, 1); __PYX_ERR(0, 220, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("most_frequent_substrings", 0, 2, 4, 1); __PYX_ERR(0, 223, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_limit);
           if (value) { values[2] = value; kw_args--; }
         }
@@ -28141,62 +28282,62 @@
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_minimum_count);
           if (value) { values[3] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "most_frequent_substrings") < 0)) __PYX_ERR(0, 220, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "most_frequent_substrings") < 0)) __PYX_ERR(0, 223, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_lcp = ((PyArrayObject *)values[0]);
-    __pyx_v_length = __Pyx_PyInt_As_npy_int64(values[1]); if (unlikely((__pyx_v_length == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 222, __pyx_L3_error)
+    __pyx_v_length = __Pyx_PyInt_As_npy_int64(values[1]); if (unlikely((__pyx_v_length == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 225, __pyx_L3_error)
     if (values[2]) {
-      __pyx_v_limit = __Pyx_PyInt_As_npy_int64(values[2]); if (unlikely((__pyx_v_limit == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 223, __pyx_L3_error)
+      __pyx_v_limit = __Pyx_PyInt_As_npy_int64(values[2]); if (unlikely((__pyx_v_limit == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 226, __pyx_L3_error)
     } else {
       __pyx_v_limit = __pyx_dynamic_args->__pyx_arg_limit;
     }
     if (values[3]) {
-      __pyx_v_minimum_count = __Pyx_PyInt_As_npy_int64(values[3]); if (unlikely((__pyx_v_minimum_count == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 224, __pyx_L3_error)
+      __pyx_v_minimum_count = __Pyx_PyInt_As_npy_int64(values[3]); if (unlikely((__pyx_v_minimum_count == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 227, __pyx_L3_error)
     } else {
       __pyx_v_minimum_count = __pyx_dynamic_args->__pyx_arg_minimum_count;
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("most_frequent_substrings", 0, 2, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 220, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("most_frequent_substrings", 0, 2, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 223, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pydivsufsort.stringalg.most_frequent_substrings", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_lcp), __pyx_ptype_5numpy_ndarray, 0, "lcp", 0))) __PYX_ERR(0, 221, __pyx_L1_error)
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_124most_frequent_substrings(__pyx_self, __pyx_v_lcp, __pyx_v_length, __pyx_v_limit, __pyx_v_minimum_count);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_lcp), __pyx_ptype_5numpy_ndarray, 0, "lcp", 0))) __PYX_ERR(0, 224, __pyx_L1_error)
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_126most_frequent_substrings(__pyx_self, __pyx_v_lcp, __pyx_v_length, __pyx_v_limit, __pyx_v_minimum_count);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_124most_frequent_substrings(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_lcp, __pyx_t_5numpy_int64_t __pyx_v_length, __pyx_t_5numpy_int64_t __pyx_v_limit, __pyx_t_5numpy_int64_t __pyx_v_minimum_count) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_126most_frequent_substrings(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_lcp, __pyx_t_5numpy_int64_t __pyx_v_length, __pyx_t_5numpy_int64_t __pyx_v_limit, __pyx_t_5numpy_int64_t __pyx_v_minimum_count) {
   __pyx_t_5numpy_int64_t __pyx_v_n;
   __pyx_t_5numpy_int64_t __pyx_v_i;
   __pyx_t_5numpy_int64_t __pyx_v_cur;
   __pyx_t_5numpy_int64_t __pyx_v_cur_count;
   std::vector<std::pair<__pyx_t_5numpy_int64_t,__pyx_t_5numpy_int64_t> >  __pyx_v_count;
   PyArrayObject *__pyx_v_pos = 0;
   PyArrayObject *__pyx_v_cnt = 0;
@@ -28237,256 +28378,256 @@
   __pyx_pybuffernd_cnt.rcbuffer = &__pyx_pybuffer_cnt;
   __pyx_pybuffer_lcp.pybuffer.buf = NULL;
   __pyx_pybuffer_lcp.refcount = 0;
   __pyx_pybuffernd_lcp.data = NULL;
   __pyx_pybuffernd_lcp.rcbuffer = &__pyx_pybuffer_lcp;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_lcp.rcbuffer->pybuffer, (PyObject*)__pyx_v_lcp, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 220, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_lcp.rcbuffer->pybuffer, (PyObject*)__pyx_v_lcp, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 223, __pyx_L1_error)
   }
   __pyx_pybuffernd_lcp.diminfo[0].strides = __pyx_pybuffernd_lcp.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_lcp.diminfo[0].shape = __pyx_pybuffernd_lcp.rcbuffer->pybuffer.shape[0];
 
-  /* "pydivsufsort/stringalg.pyx":253
+  /* "pydivsufsort/stringalg.pyx":260
  *     cdef vector[pair[sa_t, sa_t]] count
  * 
  *     if minimum_count < 1:             # <<<<<<<<<<<<<<
  *         minimum_count = 1
  * 
  */
   __pyx_t_1 = ((__pyx_v_minimum_count < 1) != 0);
   if (__pyx_t_1) {
 
-    /* "pydivsufsort/stringalg.pyx":254
+    /* "pydivsufsort/stringalg.pyx":261
  * 
  *     if minimum_count < 1:
  *         minimum_count = 1             # <<<<<<<<<<<<<<
  * 
  *     n = len(lcp)
  */
     __pyx_v_minimum_count = 1;
 
-    /* "pydivsufsort/stringalg.pyx":253
+    /* "pydivsufsort/stringalg.pyx":260
  *     cdef vector[pair[sa_t, sa_t]] count
  * 
  *     if minimum_count < 1:             # <<<<<<<<<<<<<<
  *         minimum_count = 1
  * 
  */
   }
 
-  /* "pydivsufsort/stringalg.pyx":256
+  /* "pydivsufsort/stringalg.pyx":263
  *         minimum_count = 1
  * 
  *     n = len(lcp)             # <<<<<<<<<<<<<<
  *     cur = 0
  *     cur_count = 1
  */
-  __pyx_t_2 = PyObject_Length(((PyObject *)__pyx_v_lcp)); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 256, __pyx_L1_error)
+  __pyx_t_2 = PyObject_Length(((PyObject *)__pyx_v_lcp)); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 263, __pyx_L1_error)
   __pyx_v_n = __pyx_t_2;
 
-  /* "pydivsufsort/stringalg.pyx":257
+  /* "pydivsufsort/stringalg.pyx":264
  * 
  *     n = len(lcp)
  *     cur = 0             # <<<<<<<<<<<<<<
  *     cur_count = 1
  *     for i in range(n-1):
  */
   __pyx_v_cur = 0;
 
-  /* "pydivsufsort/stringalg.pyx":258
+  /* "pydivsufsort/stringalg.pyx":265
  *     n = len(lcp)
  *     cur = 0
  *     cur_count = 1             # <<<<<<<<<<<<<<
  *     for i in range(n-1):
  *         if lcp[i] >= length:
  */
   __pyx_v_cur_count = 1;
 
-  /* "pydivsufsort/stringalg.pyx":259
+  /* "pydivsufsort/stringalg.pyx":266
  *     cur = 0
  *     cur_count = 1
  *     for i in range(n-1):             # <<<<<<<<<<<<<<
  *         if lcp[i] >= length:
  *             cur_count += 1
  */
   __pyx_t_3 = (__pyx_v_n - 1);
   __pyx_t_4 = __pyx_t_3;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
     __pyx_v_i = __pyx_t_5;
 
-    /* "pydivsufsort/stringalg.pyx":260
+    /* "pydivsufsort/stringalg.pyx":267
  *     cur_count = 1
  *     for i in range(n-1):
  *         if lcp[i] >= length:             # <<<<<<<<<<<<<<
  *             cur_count += 1
  *         else:
  */
     __pyx_t_6 = __pyx_v_i;
     __pyx_t_1 = (((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int64_t *, __pyx_pybuffernd_lcp.rcbuffer->pybuffer.buf, __pyx_t_6, __pyx_pybuffernd_lcp.diminfo[0].strides)) >= __pyx_v_length) != 0);
     if (__pyx_t_1) {
 
-      /* "pydivsufsort/stringalg.pyx":261
+      /* "pydivsufsort/stringalg.pyx":268
  *     for i in range(n-1):
  *         if lcp[i] >= length:
  *             cur_count += 1             # <<<<<<<<<<<<<<
  *         else:
  *             if cur_count >= minimum_count:
  */
       __pyx_v_cur_count = (__pyx_v_cur_count + 1);
 
-      /* "pydivsufsort/stringalg.pyx":260
+      /* "pydivsufsort/stringalg.pyx":267
  *     cur_count = 1
  *     for i in range(n-1):
  *         if lcp[i] >= length:             # <<<<<<<<<<<<<<
  *             cur_count += 1
  *         else:
  */
       goto __pyx_L6;
     }
 
-    /* "pydivsufsort/stringalg.pyx":263
+    /* "pydivsufsort/stringalg.pyx":270
  *             cur_count += 1
  *         else:
  *             if cur_count >= minimum_count:             # <<<<<<<<<<<<<<
  *                 count.push_back((cur_count, cur))
  *             cur = i + 1
  */
     /*else*/ {
       __pyx_t_1 = ((__pyx_v_cur_count >= __pyx_v_minimum_count) != 0);
       if (__pyx_t_1) {
 
-        /* "pydivsufsort/stringalg.pyx":264
+        /* "pydivsufsort/stringalg.pyx":271
  *         else:
  *             if cur_count >= minimum_count:
  *                 count.push_back((cur_count, cur))             # <<<<<<<<<<<<<<
  *             cur = i + 1
  *             cur_count = 1
  */
-        __pyx_t_7 = __Pyx_PyInt_From_npy_int64(__pyx_v_cur_count); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 264, __pyx_L1_error)
+        __pyx_t_7 = __Pyx_PyInt_From_npy_int64(__pyx_v_cur_count); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 271, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
-        __pyx_t_8 = __Pyx_PyInt_From_npy_int64(__pyx_v_cur); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 264, __pyx_L1_error)
+        __pyx_t_8 = __Pyx_PyInt_From_npy_int64(__pyx_v_cur); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 271, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
-        __pyx_t_9 = PyTuple_New(2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 264, __pyx_L1_error)
+        __pyx_t_9 = PyTuple_New(2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 271, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_9);
         __Pyx_GIVEREF(__pyx_t_7);
         PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_7);
         __Pyx_GIVEREF(__pyx_t_8);
         PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_t_8);
         __pyx_t_7 = 0;
         __pyx_t_8 = 0;
-        __pyx_t_10 = __pyx_convert_pair_from_py___pyx_t_5numpy_int64_t__and___pyx_t_5numpy_int64_t(__pyx_t_9); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 264, __pyx_L1_error)
+        __pyx_t_10 = __pyx_convert_pair_from_py___pyx_t_5numpy_int64_t__and___pyx_t_5numpy_int64_t(__pyx_t_9); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 271, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         try {
           __pyx_v_count.push_back(__pyx_t_10);
         } catch(...) {
           __Pyx_CppExn2PyErr();
-          __PYX_ERR(0, 264, __pyx_L1_error)
+          __PYX_ERR(0, 271, __pyx_L1_error)
         }
 
-        /* "pydivsufsort/stringalg.pyx":263
+        /* "pydivsufsort/stringalg.pyx":270
  *             cur_count += 1
  *         else:
  *             if cur_count >= minimum_count:             # <<<<<<<<<<<<<<
  *                 count.push_back((cur_count, cur))
  *             cur = i + 1
  */
       }
 
-      /* "pydivsufsort/stringalg.pyx":265
+      /* "pydivsufsort/stringalg.pyx":272
  *             if cur_count >= minimum_count:
  *                 count.push_back((cur_count, cur))
  *             cur = i + 1             # <<<<<<<<<<<<<<
  *             cur_count = 1
  *     if cur_count >= minimum_count:
  */
       __pyx_v_cur = (__pyx_v_i + 1);
 
-      /* "pydivsufsort/stringalg.pyx":266
+      /* "pydivsufsort/stringalg.pyx":273
  *                 count.push_back((cur_count, cur))
  *             cur = i + 1
  *             cur_count = 1             # <<<<<<<<<<<<<<
  *     if cur_count >= minimum_count:
  *         count.push_back((cur_count, cur))
  */
       __pyx_v_cur_count = 1;
     }
     __pyx_L6:;
   }
 
-  /* "pydivsufsort/stringalg.pyx":267
+  /* "pydivsufsort/stringalg.pyx":274
  *             cur = i + 1
  *             cur_count = 1
  *     if cur_count >= minimum_count:             # <<<<<<<<<<<<<<
  *         count.push_back((cur_count, cur))
  * 
  */
   __pyx_t_1 = ((__pyx_v_cur_count >= __pyx_v_minimum_count) != 0);
   if (__pyx_t_1) {
 
-    /* "pydivsufsort/stringalg.pyx":268
+    /* "pydivsufsort/stringalg.pyx":275
  *             cur_count = 1
  *     if cur_count >= minimum_count:
  *         count.push_back((cur_count, cur))             # <<<<<<<<<<<<<<
  * 
  *     sort(count.begin(), count.end())
  */
-    __pyx_t_9 = __Pyx_PyInt_From_npy_int64(__pyx_v_cur_count); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 268, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyInt_From_npy_int64(__pyx_v_cur_count); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 275, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
-    __pyx_t_8 = __Pyx_PyInt_From_npy_int64(__pyx_v_cur); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 268, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyInt_From_npy_int64(__pyx_v_cur); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 275, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_7 = PyTuple_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 268, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 275, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_9);
     PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_9);
     __Pyx_GIVEREF(__pyx_t_8);
     PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_t_8);
     __pyx_t_9 = 0;
     __pyx_t_8 = 0;
-    __pyx_t_10 = __pyx_convert_pair_from_py___pyx_t_5numpy_int64_t__and___pyx_t_5numpy_int64_t(__pyx_t_7); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 268, __pyx_L1_error)
+    __pyx_t_10 = __pyx_convert_pair_from_py___pyx_t_5numpy_int64_t__and___pyx_t_5numpy_int64_t(__pyx_t_7); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 275, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     try {
       __pyx_v_count.push_back(__pyx_t_10);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 268, __pyx_L1_error)
+      __PYX_ERR(0, 275, __pyx_L1_error)
     }
 
-    /* "pydivsufsort/stringalg.pyx":267
+    /* "pydivsufsort/stringalg.pyx":274
  *             cur = i + 1
  *             cur_count = 1
  *     if cur_count >= minimum_count:             # <<<<<<<<<<<<<<
  *         count.push_back((cur_count, cur))
  * 
  */
   }
 
-  /* "pydivsufsort/stringalg.pyx":270
+  /* "pydivsufsort/stringalg.pyx":277
  *         count.push_back((cur_count, cur))
  * 
  *     sort(count.begin(), count.end())             # <<<<<<<<<<<<<<
  *     reverse(count.begin(), count.end())
  *     if limit and limit < count.size():
  */
   std::sort<std::vector<std::pair<__pyx_t_5numpy_int64_t,__pyx_t_5numpy_int64_t> > ::iterator>(__pyx_v_count.begin(), __pyx_v_count.end());
 
-  /* "pydivsufsort/stringalg.pyx":271
+  /* "pydivsufsort/stringalg.pyx":278
  * 
  *     sort(count.begin(), count.end())
  *     reverse(count.begin(), count.end())             # <<<<<<<<<<<<<<
  *     if limit and limit < count.size():
  *         count.resize(limit)
  */
   try {
     std::reverse<std::vector<std::pair<__pyx_t_5numpy_int64_t,__pyx_t_5numpy_int64_t> > ::iterator>(__pyx_v_count.begin(), __pyx_v_count.end());
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 271, __pyx_L1_error)
+    __PYX_ERR(0, 278, __pyx_L1_error)
   }
 
-  /* "pydivsufsort/stringalg.pyx":272
+  /* "pydivsufsort/stringalg.pyx":279
  *     sort(count.begin(), count.end())
  *     reverse(count.begin(), count.end())
  *     if limit and limit < count.size():             # <<<<<<<<<<<<<<
  *         count.resize(limit)
  * 
  */
   __pyx_t_11 = (__pyx_v_limit != 0);
@@ -28496,190 +28637,190 @@
     goto __pyx_L10_bool_binop_done;
   }
   __pyx_t_11 = ((__pyx_v_limit < __pyx_v_count.size()) != 0);
   __pyx_t_1 = __pyx_t_11;
   __pyx_L10_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "pydivsufsort/stringalg.pyx":273
+    /* "pydivsufsort/stringalg.pyx":280
  *     reverse(count.begin(), count.end())
  *     if limit and limit < count.size():
  *         count.resize(limit)             # <<<<<<<<<<<<<<
  * 
  *     n = count.size()
  */
     try {
       __pyx_v_count.resize(__pyx_v_limit);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 273, __pyx_L1_error)
+      __PYX_ERR(0, 280, __pyx_L1_error)
     }
 
-    /* "pydivsufsort/stringalg.pyx":272
+    /* "pydivsufsort/stringalg.pyx":279
  *     sort(count.begin(), count.end())
  *     reverse(count.begin(), count.end())
  *     if limit and limit < count.size():             # <<<<<<<<<<<<<<
  *         count.resize(limit)
  * 
  */
   }
 
-  /* "pydivsufsort/stringalg.pyx":275
+  /* "pydivsufsort/stringalg.pyx":282
  *         count.resize(limit)
  * 
  *     n = count.size()             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[sa_t, ndim=1] pos = np.empty(n, dtype=lcp.dtype)
  *     cdef np.ndarray[sa_t, ndim=1] cnt = np.empty(n, dtype=lcp.dtype)
  */
   __pyx_v_n = __pyx_v_count.size();
 
-  /* "pydivsufsort/stringalg.pyx":276
+  /* "pydivsufsort/stringalg.pyx":283
  * 
  *     n = count.size()
  *     cdef np.ndarray[sa_t, ndim=1] pos = np.empty(n, dtype=lcp.dtype)             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[sa_t, ndim=1] cnt = np.empty(n, dtype=lcp.dtype)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 283, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_empty); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_empty); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 283, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_PyInt_From_npy_int64(__pyx_v_n); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_From_npy_int64(__pyx_v_n); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 283, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_9 = PyTuple_New(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __pyx_t_9 = PyTuple_New(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 283, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_GIVEREF(__pyx_t_7);
   PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_7);
   __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 283, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_12 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_lcp), __pyx_n_s_dtype); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __pyx_t_12 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_lcp), __pyx_n_s_dtype); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 283, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_dtype, __pyx_t_12) < 0) __PYX_ERR(0, 276, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_dtype, __pyx_t_12) < 0) __PYX_ERR(0, 283, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-  __pyx_t_12 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_t_9, __pyx_t_7); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __pyx_t_12 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_t_9, __pyx_t_7); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 283, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (!(likely(((__pyx_t_12) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_12, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 276, __pyx_L1_error)
+  if (!(likely(((__pyx_t_12) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_12, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 283, __pyx_L1_error)
   __pyx_t_13 = ((PyArrayObject *)__pyx_t_12);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_pos.rcbuffer->pybuffer, (PyObject*)__pyx_t_13, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int64_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_pos = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_pos.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 276, __pyx_L1_error)
+      __PYX_ERR(0, 283, __pyx_L1_error)
     } else {__pyx_pybuffernd_pos.diminfo[0].strides = __pyx_pybuffernd_pos.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_pos.diminfo[0].shape = __pyx_pybuffernd_pos.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_13 = 0;
   __pyx_v_pos = ((PyArrayObject *)__pyx_t_12);
   __pyx_t_12 = 0;
 
-  /* "pydivsufsort/stringalg.pyx":277
+  /* "pydivsufsort/stringalg.pyx":284
  *     n = count.size()
  *     cdef np.ndarray[sa_t, ndim=1] pos = np.empty(n, dtype=lcp.dtype)
  *     cdef np.ndarray[sa_t, ndim=1] cnt = np.empty(n, dtype=lcp.dtype)             # <<<<<<<<<<<<<<
  * 
  *     for i in range(n):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_np); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 277, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_np); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 284, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_empty); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 277, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_empty); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 284, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-  __pyx_t_12 = __Pyx_PyInt_From_npy_int64(__pyx_v_n); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 277, __pyx_L1_error)
+  __pyx_t_12 = __Pyx_PyInt_From_npy_int64(__pyx_v_n); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 284, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
-  __pyx_t_9 = PyTuple_New(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 277, __pyx_L1_error)
+  __pyx_t_9 = PyTuple_New(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 284, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_GIVEREF(__pyx_t_12);
   PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_12);
   __pyx_t_12 = 0;
-  __pyx_t_12 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 277, __pyx_L1_error)
+  __pyx_t_12 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 284, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_lcp), __pyx_n_s_dtype); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 277, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_lcp), __pyx_n_s_dtype); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 284, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  if (PyDict_SetItem(__pyx_t_12, __pyx_n_s_dtype, __pyx_t_8) < 0) __PYX_ERR(0, 277, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_12, __pyx_n_s_dtype, __pyx_t_8) < 0) __PYX_ERR(0, 284, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_9, __pyx_t_12); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 277, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_9, __pyx_t_12); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 284, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-  if (!(likely(((__pyx_t_8) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_8, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 277, __pyx_L1_error)
+  if (!(likely(((__pyx_t_8) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_8, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 284, __pyx_L1_error)
   __pyx_t_14 = ((PyArrayObject *)__pyx_t_8);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_cnt.rcbuffer->pybuffer, (PyObject*)__pyx_t_14, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int64_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_cnt = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_cnt.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 277, __pyx_L1_error)
+      __PYX_ERR(0, 284, __pyx_L1_error)
     } else {__pyx_pybuffernd_cnt.diminfo[0].strides = __pyx_pybuffernd_cnt.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_cnt.diminfo[0].shape = __pyx_pybuffernd_cnt.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_14 = 0;
   __pyx_v_cnt = ((PyArrayObject *)__pyx_t_8);
   __pyx_t_8 = 0;
 
-  /* "pydivsufsort/stringalg.pyx":279
+  /* "pydivsufsort/stringalg.pyx":286
  *     cdef np.ndarray[sa_t, ndim=1] cnt = np.empty(n, dtype=lcp.dtype)
  * 
  *     for i in range(n):             # <<<<<<<<<<<<<<
  *         pos[i] = count[i].second
  *         cnt[i] = count[i].first
  */
   __pyx_t_3 = __pyx_v_n;
   __pyx_t_4 = __pyx_t_3;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
     __pyx_v_i = __pyx_t_5;
 
-    /* "pydivsufsort/stringalg.pyx":280
+    /* "pydivsufsort/stringalg.pyx":287
  * 
  *     for i in range(n):
  *         pos[i] = count[i].second             # <<<<<<<<<<<<<<
  *         cnt[i] = count[i].first
  * 
  */
     __pyx_t_6 = (__pyx_v_count[__pyx_v_i]).second;
     __pyx_t_15 = __pyx_v_i;
     *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int64_t *, __pyx_pybuffernd_pos.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_pos.diminfo[0].strides) = __pyx_t_6;
 
-    /* "pydivsufsort/stringalg.pyx":281
+    /* "pydivsufsort/stringalg.pyx":288
  *     for i in range(n):
  *         pos[i] = count[i].second
  *         cnt[i] = count[i].first             # <<<<<<<<<<<<<<
  * 
  *     return pos, cnt
  */
     __pyx_t_6 = (__pyx_v_count[__pyx_v_i]).first;
     __pyx_t_15 = __pyx_v_i;
     *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int64_t *, __pyx_pybuffernd_cnt.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_cnt.diminfo[0].strides) = __pyx_t_6;
   }
 
-  /* "pydivsufsort/stringalg.pyx":283
+  /* "pydivsufsort/stringalg.pyx":290
  *         cnt[i] = count[i].first
  * 
  *     return pos, cnt             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_8 = PyTuple_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 283, __pyx_L1_error)
+  __pyx_t_8 = PyTuple_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 290, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_INCREF(((PyObject *)__pyx_v_pos));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_pos));
   PyTuple_SET_ITEM(__pyx_t_8, 0, ((PyObject *)__pyx_v_pos));
   __Pyx_INCREF(((PyObject *)__pyx_v_cnt));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_cnt));
   PyTuple_SET_ITEM(__pyx_t_8, 1, ((PyObject *)__pyx_v_cnt));
   __pyx_r = __pyx_t_8;
   __pyx_t_8 = 0;
   goto __pyx_L0;
 
-  /* "pydivsufsort/stringalg.pyx":220
+  /* "pydivsufsort/stringalg.pyx":223
  * 
  * 
  * def most_frequent_substrings(             # <<<<<<<<<<<<<<
  *     np.ndarray[sa_t, ndim=1] lcp not None,
  *     sa_t length,
  */
 
@@ -28708,23 +28849,23 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_pos);
   __Pyx_XDECREF((PyObject *)__pyx_v_cnt);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pydivsufsort/stringalg.pyx":286
+/* "pydivsufsort/stringalg.pyx":293
  * 
  * 
  * cpdef repeated_substrings(ull[::1] suffix_array, ull[::1] lcp):             # <<<<<<<<<<<<<<
  *     """
  *     See https://github.com/louisabraham/pydivsufsort/issues/42 for more details
  */
 
-static PyObject *__pyx_pw_12pydivsufsort_9stringalg_21repeated_substrings(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyObject *__pyx_pw_12pydivsufsort_9stringalg_23repeated_substrings(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_f_12pydivsufsort_9stringalg_repeated_substrings(CYTHON_UNUSED __Pyx_memviewslice __pyx_v_suffix_array, __Pyx_memviewslice __pyx_v_lcp, CYTHON_UNUSED int __pyx_skip_dispatch) {
   std::vector<std::pair<__pyx_t_12pydivsufsort_9stringalg_ull,__pyx_t_12pydivsufsort_9stringalg_ull> >  __pyx_v_stack;
   __pyx_t_12pydivsufsort_9stringalg_ull __pyx_v_n;
   __pyx_t_12pydivsufsort_9stringalg_ull __pyx_v_idx;
   __pyx_t_12pydivsufsort_9stringalg_ull __pyx_v_start;
   __pyx_t_12pydivsufsort_9stringalg_ull __pyx_v_length;
   PyObject *__pyx_v_ans = 0;
@@ -28746,49 +28887,49 @@
   __pyx_t_12pydivsufsort_9stringalg_ull __pyx_t_14;
   int __pyx_t_15;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("repeated_substrings", 0);
 
-  /* "pydivsufsort/stringalg.pyx":307
+  /* "pydivsufsort/stringalg.pyx":314
  *     cdef pair[ull, ull] key
  *     cdef ull n, idx, end_pos, len_range, start, length
  *     cdef list ans = []             # <<<<<<<<<<<<<<
  *     n = len(lcp)
  *     for idx in range(n):
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 307, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 314, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_ans = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pydivsufsort/stringalg.pyx":308
+  /* "pydivsufsort/stringalg.pyx":315
  *     cdef ull n, idx, end_pos, len_range, start, length
  *     cdef list ans = []
  *     n = len(lcp)             # <<<<<<<<<<<<<<
  *     for idx in range(n):
  *         if stack.empty() or lcp[idx] > stack.back().first:
  */
   __pyx_t_2 = __Pyx_MemoryView_Len(__pyx_v_lcp); 
   __pyx_v_n = __pyx_t_2;
 
-  /* "pydivsufsort/stringalg.pyx":309
+  /* "pydivsufsort/stringalg.pyx":316
  *     cdef list ans = []
  *     n = len(lcp)
  *     for idx in range(n):             # <<<<<<<<<<<<<<
  *         if stack.empty() or lcp[idx] > stack.back().first:
  *             if lcp[idx] > 0:
  */
   __pyx_t_3 = __pyx_v_n;
   __pyx_t_4 = __pyx_t_3;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
     __pyx_v_idx = __pyx_t_5;
 
-    /* "pydivsufsort/stringalg.pyx":310
+    /* "pydivsufsort/stringalg.pyx":317
  *     n = len(lcp)
  *     for idx in range(n):
  *         if stack.empty() or lcp[idx] > stack.back().first:             # <<<<<<<<<<<<<<
  *             if lcp[idx] > 0:
  *                 stack.push_back((lcp[idx], idx))
  */
     __pyx_t_7 = (__pyx_v_stack.empty() != 0);
@@ -28799,74 +28940,74 @@
     }
     __pyx_t_8 = __pyx_v_idx;
     __pyx_t_7 = (((*((__pyx_t_12pydivsufsort_9stringalg_ull *) ( /* dim=0 */ ((char *) (((__pyx_t_12pydivsufsort_9stringalg_ull *) __pyx_v_lcp.data) + __pyx_t_8)) ))) > __pyx_v_stack.back().first) != 0);
     __pyx_t_6 = __pyx_t_7;
     __pyx_L6_bool_binop_done:;
     if (__pyx_t_6) {
 
-      /* "pydivsufsort/stringalg.pyx":311
+      /* "pydivsufsort/stringalg.pyx":318
  *     for idx in range(n):
  *         if stack.empty() or lcp[idx] > stack.back().first:
  *             if lcp[idx] > 0:             # <<<<<<<<<<<<<<
  *                 stack.push_back((lcp[idx], idx))
  *         else:
  */
       __pyx_t_8 = __pyx_v_idx;
       __pyx_t_6 = (((*((__pyx_t_12pydivsufsort_9stringalg_ull *) ( /* dim=0 */ ((char *) (((__pyx_t_12pydivsufsort_9stringalg_ull *) __pyx_v_lcp.data) + __pyx_t_8)) ))) > 0) != 0);
       if (__pyx_t_6) {
 
-        /* "pydivsufsort/stringalg.pyx":312
+        /* "pydivsufsort/stringalg.pyx":319
  *         if stack.empty() or lcp[idx] > stack.back().first:
  *             if lcp[idx] > 0:
  *                 stack.push_back((lcp[idx], idx))             # <<<<<<<<<<<<<<
  *         else:
  *             while not stack.empty() and lcp[idx] < stack.back().first:
  */
         __pyx_t_8 = __pyx_v_idx;
-        __pyx_t_1 = __Pyx_PyInt_From_npy_uint64((*((__pyx_t_12pydivsufsort_9stringalg_ull *) ( /* dim=0 */ ((char *) (((__pyx_t_12pydivsufsort_9stringalg_ull *) __pyx_v_lcp.data) + __pyx_t_8)) )))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 312, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyInt_From_npy_uint64((*((__pyx_t_12pydivsufsort_9stringalg_ull *) ( /* dim=0 */ ((char *) (((__pyx_t_12pydivsufsort_9stringalg_ull *) __pyx_v_lcp.data) + __pyx_t_8)) )))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 319, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_9 = __Pyx_PyInt_From_npy_uint64(__pyx_v_idx); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 312, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyInt_From_npy_uint64(__pyx_v_idx); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 319, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_9);
-        __pyx_t_10 = PyTuple_New(2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 312, __pyx_L1_error)
+        __pyx_t_10 = PyTuple_New(2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 319, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_10);
         __Pyx_GIVEREF(__pyx_t_1);
         PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_1);
         __Pyx_GIVEREF(__pyx_t_9);
         PyTuple_SET_ITEM(__pyx_t_10, 1, __pyx_t_9);
         __pyx_t_1 = 0;
         __pyx_t_9 = 0;
-        __pyx_t_11 = __pyx_convert_pair_from_py___pyx_t_12pydivsufsort_9stringalg_ull__and___pyx_t_12pydivsufsort_9stringalg_ull(__pyx_t_10); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 312, __pyx_L1_error)
+        __pyx_t_11 = __pyx_convert_pair_from_py___pyx_t_12pydivsufsort_9stringalg_ull__and___pyx_t_12pydivsufsort_9stringalg_ull(__pyx_t_10); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 319, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
         try {
           __pyx_v_stack.push_back(__pyx_t_11);
         } catch(...) {
           __Pyx_CppExn2PyErr();
-          __PYX_ERR(0, 312, __pyx_L1_error)
+          __PYX_ERR(0, 319, __pyx_L1_error)
         }
 
-        /* "pydivsufsort/stringalg.pyx":311
+        /* "pydivsufsort/stringalg.pyx":318
  *     for idx in range(n):
  *         if stack.empty() or lcp[idx] > stack.back().first:
  *             if lcp[idx] > 0:             # <<<<<<<<<<<<<<
  *                 stack.push_back((lcp[idx], idx))
  *         else:
  */
       }
 
-      /* "pydivsufsort/stringalg.pyx":310
+      /* "pydivsufsort/stringalg.pyx":317
  *     n = len(lcp)
  *     for idx in range(n):
  *         if stack.empty() or lcp[idx] > stack.back().first:             # <<<<<<<<<<<<<<
  *             if lcp[idx] > 0:
  *                 stack.push_back((lcp[idx], idx))
  */
       goto __pyx_L5;
     }
 
-    /* "pydivsufsort/stringalg.pyx":314
+    /* "pydivsufsort/stringalg.pyx":321
  *                 stack.push_back((lcp[idx], idx))
  *         else:
  *             while not stack.empty() and lcp[idx] < stack.back().first:             # <<<<<<<<<<<<<<
  *                 length, start = stack.back()
  *                 stack.pop_back()
  */
     /*else*/ {
@@ -28879,114 +29020,114 @@
         }
         __pyx_t_8 = __pyx_v_idx;
         __pyx_t_7 = (((*((__pyx_t_12pydivsufsort_9stringalg_ull *) ( /* dim=0 */ ((char *) (((__pyx_t_12pydivsufsort_9stringalg_ull *) __pyx_v_lcp.data) + __pyx_t_8)) ))) < __pyx_v_stack.back().first) != 0);
         __pyx_t_6 = __pyx_t_7;
         __pyx_L11_bool_binop_done:;
         if (!__pyx_t_6) break;
 
-        /* "pydivsufsort/stringalg.pyx":315
+        /* "pydivsufsort/stringalg.pyx":322
  *         else:
  *             while not stack.empty() and lcp[idx] < stack.back().first:
  *                 length, start = stack.back()             # <<<<<<<<<<<<<<
  *                 stack.pop_back()
  *                 ans.append((start, idx + 1, length))
  */
-        __pyx_t_10 = __pyx_convert_pair_to_py___pyx_t_12pydivsufsort_9stringalg_ull______pyx_t_12pydivsufsort_9stringalg_ull(__pyx_v_stack.back()); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 315, __pyx_L1_error)
+        __pyx_t_10 = __pyx_convert_pair_to_py___pyx_t_12pydivsufsort_9stringalg_ull______pyx_t_12pydivsufsort_9stringalg_ull(__pyx_v_stack.back()); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 322, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_10);
         if ((likely(PyTuple_CheckExact(__pyx_t_10))) || (PyList_CheckExact(__pyx_t_10))) {
           PyObject* sequence = __pyx_t_10;
           Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
           if (unlikely(size != 2)) {
             if (size > 2) __Pyx_RaiseTooManyValuesError(2);
             else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-            __PYX_ERR(0, 315, __pyx_L1_error)
+            __PYX_ERR(0, 322, __pyx_L1_error)
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
           if (likely(PyTuple_CheckExact(sequence))) {
             __pyx_t_9 = PyTuple_GET_ITEM(sequence, 0); 
             __pyx_t_1 = PyTuple_GET_ITEM(sequence, 1); 
           } else {
             __pyx_t_9 = PyList_GET_ITEM(sequence, 0); 
             __pyx_t_1 = PyList_GET_ITEM(sequence, 1); 
           }
           __Pyx_INCREF(__pyx_t_9);
           __Pyx_INCREF(__pyx_t_1);
           #else
-          __pyx_t_9 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 315, __pyx_L1_error)
+          __pyx_t_9 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 322, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_9);
-          __pyx_t_1 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 315, __pyx_L1_error)
+          __pyx_t_1 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 322, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_1);
           #endif
           __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
         } else {
           Py_ssize_t index = -1;
-          __pyx_t_12 = PyObject_GetIter(__pyx_t_10); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 315, __pyx_L1_error)
+          __pyx_t_12 = PyObject_GetIter(__pyx_t_10); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 322, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_12);
           __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
           __pyx_t_13 = Py_TYPE(__pyx_t_12)->tp_iternext;
           index = 0; __pyx_t_9 = __pyx_t_13(__pyx_t_12); if (unlikely(!__pyx_t_9)) goto __pyx_L13_unpacking_failed;
           __Pyx_GOTREF(__pyx_t_9);
           index = 1; __pyx_t_1 = __pyx_t_13(__pyx_t_12); if (unlikely(!__pyx_t_1)) goto __pyx_L13_unpacking_failed;
           __Pyx_GOTREF(__pyx_t_1);
-          if (__Pyx_IternextUnpackEndCheck(__pyx_t_13(__pyx_t_12), 2) < 0) __PYX_ERR(0, 315, __pyx_L1_error)
+          if (__Pyx_IternextUnpackEndCheck(__pyx_t_13(__pyx_t_12), 2) < 0) __PYX_ERR(0, 322, __pyx_L1_error)
           __pyx_t_13 = NULL;
           __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
           goto __pyx_L14_unpacking_done;
           __pyx_L13_unpacking_failed:;
           __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
           __pyx_t_13 = NULL;
           if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-          __PYX_ERR(0, 315, __pyx_L1_error)
+          __PYX_ERR(0, 322, __pyx_L1_error)
           __pyx_L14_unpacking_done:;
         }
-        __pyx_t_8 = __Pyx_PyInt_As_npy_uint64(__pyx_t_9); if (unlikely((__pyx_t_8 == ((npy_uint64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 315, __pyx_L1_error)
+        __pyx_t_8 = __Pyx_PyInt_As_npy_uint64(__pyx_t_9); if (unlikely((__pyx_t_8 == ((npy_uint64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 322, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-        __pyx_t_14 = __Pyx_PyInt_As_npy_uint64(__pyx_t_1); if (unlikely((__pyx_t_14 == ((npy_uint64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 315, __pyx_L1_error)
+        __pyx_t_14 = __Pyx_PyInt_As_npy_uint64(__pyx_t_1); if (unlikely((__pyx_t_14 == ((npy_uint64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 322, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __pyx_v_length = __pyx_t_8;
         __pyx_v_start = __pyx_t_14;
 
-        /* "pydivsufsort/stringalg.pyx":316
+        /* "pydivsufsort/stringalg.pyx":323
  *             while not stack.empty() and lcp[idx] < stack.back().first:
  *                 length, start = stack.back()
  *                 stack.pop_back()             # <<<<<<<<<<<<<<
  *                 ans.append((start, idx + 1, length))
  * 
  */
         __pyx_v_stack.pop_back();
 
-        /* "pydivsufsort/stringalg.pyx":317
+        /* "pydivsufsort/stringalg.pyx":324
  *                 length, start = stack.back()
  *                 stack.pop_back()
  *                 ans.append((start, idx + 1, length))             # <<<<<<<<<<<<<<
  * 
  *             if stack.empty() and lcp[idx] > 0 or lcp[idx] > stack.back().first:
  */
-        __pyx_t_10 = __Pyx_PyInt_From_npy_uint64(__pyx_v_start); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 317, __pyx_L1_error)
+        __pyx_t_10 = __Pyx_PyInt_From_npy_uint64(__pyx_v_start); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 324, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_10);
-        __pyx_t_1 = __Pyx_PyInt_From_npy_uint64((__pyx_v_idx + 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 317, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyInt_From_npy_uint64((__pyx_v_idx + 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 324, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_9 = __Pyx_PyInt_From_npy_uint64(__pyx_v_length); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 317, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyInt_From_npy_uint64(__pyx_v_length); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 324, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_9);
-        __pyx_t_12 = PyTuple_New(3); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 317, __pyx_L1_error)
+        __pyx_t_12 = PyTuple_New(3); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 324, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_12);
         __Pyx_GIVEREF(__pyx_t_10);
         PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_t_10);
         __Pyx_GIVEREF(__pyx_t_1);
         PyTuple_SET_ITEM(__pyx_t_12, 1, __pyx_t_1);
         __Pyx_GIVEREF(__pyx_t_9);
         PyTuple_SET_ITEM(__pyx_t_12, 2, __pyx_t_9);
         __pyx_t_10 = 0;
         __pyx_t_1 = 0;
         __pyx_t_9 = 0;
-        __pyx_t_15 = __Pyx_PyList_Append(__pyx_v_ans, __pyx_t_12); if (unlikely(__pyx_t_15 == ((int)-1))) __PYX_ERR(0, 317, __pyx_L1_error)
+        __pyx_t_15 = __Pyx_PyList_Append(__pyx_v_ans, __pyx_t_12); if (unlikely(__pyx_t_15 == ((int)-1))) __PYX_ERR(0, 324, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
       }
 
-      /* "pydivsufsort/stringalg.pyx":319
+      /* "pydivsufsort/stringalg.pyx":326
  *                 ans.append((start, idx + 1, length))
  * 
  *             if stack.empty() and lcp[idx] > 0 or lcp[idx] > stack.back().first:             # <<<<<<<<<<<<<<
  *                 stack.push_back((lcp[idx], start))
  *     # stack is empty because lcp[n-1] == 0
  */
       __pyx_t_7 = (__pyx_v_stack.empty() != 0);
@@ -29004,68 +29145,68 @@
       __pyx_L17_next_or:;
       __pyx_t_14 = __pyx_v_idx;
       __pyx_t_7 = (((*((__pyx_t_12pydivsufsort_9stringalg_ull *) ( /* dim=0 */ ((char *) (((__pyx_t_12pydivsufsort_9stringalg_ull *) __pyx_v_lcp.data) + __pyx_t_14)) ))) > __pyx_v_stack.back().first) != 0);
       __pyx_t_6 = __pyx_t_7;
       __pyx_L16_bool_binop_done:;
       if (__pyx_t_6) {
 
-        /* "pydivsufsort/stringalg.pyx":320
+        /* "pydivsufsort/stringalg.pyx":327
  * 
  *             if stack.empty() and lcp[idx] > 0 or lcp[idx] > stack.back().first:
  *                 stack.push_back((lcp[idx], start))             # <<<<<<<<<<<<<<
  *     # stack is empty because lcp[n-1] == 0
  *     # note: lcp[n-2] is also 0 because of sep
  */
         __pyx_t_14 = __pyx_v_idx;
-        __pyx_t_12 = __Pyx_PyInt_From_npy_uint64((*((__pyx_t_12pydivsufsort_9stringalg_ull *) ( /* dim=0 */ ((char *) (((__pyx_t_12pydivsufsort_9stringalg_ull *) __pyx_v_lcp.data) + __pyx_t_14)) )))); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 320, __pyx_L1_error)
+        __pyx_t_12 = __Pyx_PyInt_From_npy_uint64((*((__pyx_t_12pydivsufsort_9stringalg_ull *) ( /* dim=0 */ ((char *) (((__pyx_t_12pydivsufsort_9stringalg_ull *) __pyx_v_lcp.data) + __pyx_t_14)) )))); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 327, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_12);
-        __pyx_t_9 = __Pyx_PyInt_From_npy_uint64(__pyx_v_start); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 320, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyInt_From_npy_uint64(__pyx_v_start); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 327, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_9);
-        __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 320, __pyx_L1_error)
+        __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 327, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_GIVEREF(__pyx_t_12);
         PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_12);
         __Pyx_GIVEREF(__pyx_t_9);
         PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_9);
         __pyx_t_12 = 0;
         __pyx_t_9 = 0;
-        __pyx_t_11 = __pyx_convert_pair_from_py___pyx_t_12pydivsufsort_9stringalg_ull__and___pyx_t_12pydivsufsort_9stringalg_ull(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 320, __pyx_L1_error)
+        __pyx_t_11 = __pyx_convert_pair_from_py___pyx_t_12pydivsufsort_9stringalg_ull__and___pyx_t_12pydivsufsort_9stringalg_ull(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 327, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         try {
           __pyx_v_stack.push_back(__pyx_t_11);
         } catch(...) {
           __Pyx_CppExn2PyErr();
-          __PYX_ERR(0, 320, __pyx_L1_error)
+          __PYX_ERR(0, 327, __pyx_L1_error)
         }
 
-        /* "pydivsufsort/stringalg.pyx":319
+        /* "pydivsufsort/stringalg.pyx":326
  *                 ans.append((start, idx + 1, length))
  * 
  *             if stack.empty() and lcp[idx] > 0 or lcp[idx] > stack.back().first:             # <<<<<<<<<<<<<<
  *                 stack.push_back((lcp[idx], start))
  *     # stack is empty because lcp[n-1] == 0
  */
       }
     }
     __pyx_L5:;
   }
 
-  /* "pydivsufsort/stringalg.pyx":324
+  /* "pydivsufsort/stringalg.pyx":331
  *     # note: lcp[n-2] is also 0 because of sep
  * 
  *     return ans             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_ans);
   __pyx_r = __pyx_v_ans;
   goto __pyx_L0;
 
-  /* "pydivsufsort/stringalg.pyx":286
+  /* "pydivsufsort/stringalg.pyx":293
  * 
  * 
  * cpdef repeated_substrings(ull[::1] suffix_array, ull[::1] lcp):             # <<<<<<<<<<<<<<
  *     """
  *     See https://github.com/louisabraham/pydivsufsort/issues/42 for more details
  */
 
@@ -29081,17 +29222,17 @@
   __Pyx_XDECREF(__pyx_v_ans);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_12pydivsufsort_9stringalg_21repeated_substrings(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_12pydivsufsort_9stringalg_20repeated_substrings[] = "\n    See https://github.com/louisabraham/pydivsufsort/issues/42 for more details\n    \n    Parameters\n    ----------\n    suffix_array : np.ndarray\n        suffix array\n    lcp : np.ndarray\n        LCP array\n    \n    Returns\n    -------\n    ranges : list\n        list of (start, end, length) tuples\n        All positions in suffix_array[start:end] correspond to\n        the same repeated substring with that length.\n    ";
-static PyObject *__pyx_pw_12pydivsufsort_9stringalg_21repeated_substrings(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_12pydivsufsort_9stringalg_23repeated_substrings(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_12pydivsufsort_9stringalg_22repeated_substrings[] = "\n    See https://github.com/louisabraham/pydivsufsort/issues/42 for more details\n    \n    Parameters\n    ----------\n    suffix_array : np.ndarray\n        suffix array\n    lcp : np.ndarray\n        LCP array\n    \n    Returns\n    -------\n    ranges : list\n        list of (start, end, length) tuples\n        All positions in suffix_array[start:end] correspond to\n        the same repeated substring with that length.\n    ";
+static PyObject *__pyx_pw_12pydivsufsort_9stringalg_23repeated_substrings(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_suffix_array = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_lcp = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -29115,56 +29256,56 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_suffix_array)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_lcp)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("repeated_substrings", 1, 2, 2, 1); __PYX_ERR(0, 286, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("repeated_substrings", 1, 2, 2, 1); __PYX_ERR(0, 293, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "repeated_substrings") < 0)) __PYX_ERR(0, 286, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "repeated_substrings") < 0)) __PYX_ERR(0, 293, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
-    __pyx_v_suffix_array = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_12pydivsufsort_9stringalg_ull(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_suffix_array.memview)) __PYX_ERR(0, 286, __pyx_L3_error)
-    __pyx_v_lcp = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_12pydivsufsort_9stringalg_ull(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_lcp.memview)) __PYX_ERR(0, 286, __pyx_L3_error)
+    __pyx_v_suffix_array = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_12pydivsufsort_9stringalg_ull(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_suffix_array.memview)) __PYX_ERR(0, 293, __pyx_L3_error)
+    __pyx_v_lcp = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_12pydivsufsort_9stringalg_ull(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_lcp.memview)) __PYX_ERR(0, 293, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("repeated_substrings", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 286, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("repeated_substrings", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 293, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pydivsufsort.stringalg.repeated_substrings", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_20repeated_substrings(__pyx_self, __pyx_v_suffix_array, __pyx_v_lcp);
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_22repeated_substrings(__pyx_self, __pyx_v_suffix_array, __pyx_v_lcp);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_20repeated_substrings(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_suffix_array, __Pyx_memviewslice __pyx_v_lcp) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_22repeated_substrings(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_suffix_array, __Pyx_memviewslice __pyx_v_lcp) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("repeated_substrings", 0);
   __Pyx_XDECREF(__pyx_r);
-  if (unlikely(!__pyx_v_suffix_array.memview)) { __Pyx_RaiseUnboundLocalError("suffix_array"); __PYX_ERR(0, 286, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_lcp.memview)) { __Pyx_RaiseUnboundLocalError("lcp"); __PYX_ERR(0, 286, __pyx_L1_error) }
-  __pyx_t_1 = __pyx_f_12pydivsufsort_9stringalg_repeated_substrings(__pyx_v_suffix_array, __pyx_v_lcp, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 286, __pyx_L1_error)
+  if (unlikely(!__pyx_v_suffix_array.memview)) { __Pyx_RaiseUnboundLocalError("suffix_array"); __PYX_ERR(0, 293, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_lcp.memview)) { __Pyx_RaiseUnboundLocalError("lcp"); __PYX_ERR(0, 293, __pyx_L1_error) }
+  __pyx_t_1 = __pyx_f_12pydivsufsort_9stringalg_repeated_substrings(__pyx_v_suffix_array, __pyx_v_lcp, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 293, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -29175,26 +29316,26 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_suffix_array, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_lcp, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pydivsufsort/stringalg.pyx":327
+/* "pydivsufsort/stringalg.pyx":334
  * 
  * 
  * def _common_substrings(np.ndarray[ull, ndim=1] suffix_array, ull[::1] lcp, ull len1, ull limit):             # <<<<<<<<<<<<<<
  *     n = len(suffix_array)
  *     ranges = repeated_substrings(suffix_array, lcp)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_12pydivsufsort_9stringalg_23_common_substrings(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_mdef_12pydivsufsort_9stringalg_23_common_substrings = {"_common_substrings", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_12pydivsufsort_9stringalg_23_common_substrings, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_12pydivsufsort_9stringalg_23_common_substrings(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_12pydivsufsort_9stringalg_25_common_substrings(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_12pydivsufsort_9stringalg_25_common_substrings = {"_common_substrings", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_12pydivsufsort_9stringalg_25_common_substrings, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_12pydivsufsort_9stringalg_25_common_substrings(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyArrayObject *__pyx_v_suffix_array = 0;
   __Pyx_memviewslice __pyx_v_lcp = { 0, 0, { 0 }, { 0 }, { 0 } };
   __pyx_t_12pydivsufsort_9stringalg_ull __pyx_v_len1;
   __pyx_t_12pydivsufsort_9stringalg_ull __pyx_v_limit;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -29224,66 +29365,66 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_suffix_array)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_lcp)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_common_substrings", 1, 4, 4, 1); __PYX_ERR(0, 327, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_common_substrings", 1, 4, 4, 1); __PYX_ERR(0, 334, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_len1)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_common_substrings", 1, 4, 4, 2); __PYX_ERR(0, 327, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_common_substrings", 1, 4, 4, 2); __PYX_ERR(0, 334, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_limit)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_common_substrings", 1, 4, 4, 3); __PYX_ERR(0, 327, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_common_substrings", 1, 4, 4, 3); __PYX_ERR(0, 334, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_common_substrings") < 0)) __PYX_ERR(0, 327, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_common_substrings") < 0)) __PYX_ERR(0, 334, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 4) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
       values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
     }
     __pyx_v_suffix_array = ((PyArrayObject *)values[0]);
-    __pyx_v_lcp = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_12pydivsufsort_9stringalg_ull(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_lcp.memview)) __PYX_ERR(0, 327, __pyx_L3_error)
-    __pyx_v_len1 = __Pyx_PyInt_As_npy_uint64(values[2]); if (unlikely((__pyx_v_len1 == ((npy_uint64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 327, __pyx_L3_error)
-    __pyx_v_limit = __Pyx_PyInt_As_npy_uint64(values[3]); if (unlikely((__pyx_v_limit == ((npy_uint64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 327, __pyx_L3_error)
+    __pyx_v_lcp = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_12pydivsufsort_9stringalg_ull(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_lcp.memview)) __PYX_ERR(0, 334, __pyx_L3_error)
+    __pyx_v_len1 = __Pyx_PyInt_As_npy_uint64(values[2]); if (unlikely((__pyx_v_len1 == ((npy_uint64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 334, __pyx_L3_error)
+    __pyx_v_limit = __Pyx_PyInt_As_npy_uint64(values[3]); if (unlikely((__pyx_v_limit == ((npy_uint64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 334, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_common_substrings", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 327, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_common_substrings", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 334, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pydivsufsort.stringalg._common_substrings", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_suffix_array), __pyx_ptype_5numpy_ndarray, 1, "suffix_array", 0))) __PYX_ERR(0, 327, __pyx_L1_error)
-  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_22_common_substrings(__pyx_self, __pyx_v_suffix_array, __pyx_v_lcp, __pyx_v_len1, __pyx_v_limit);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_suffix_array), __pyx_ptype_5numpy_ndarray, 1, "suffix_array", 0))) __PYX_ERR(0, 334, __pyx_L1_error)
+  __pyx_r = __pyx_pf_12pydivsufsort_9stringalg_24_common_substrings(__pyx_self, __pyx_v_suffix_array, __pyx_v_lcp, __pyx_v_len1, __pyx_v_limit);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pydivsufsort/stringalg.pyx":339
+/* "pydivsufsort/stringalg.pyx":346
  *     cdef cpp_map[pair[ull, ull], ull] ans
  *     cdef vector[np.uint64_t] start1, start2
  *     ranges.sort(key=lambda x: x[2]) # sort to avoid membership test             # <<<<<<<<<<<<<<
  *     cdef ull start, end, length, diff
  *     for start, end, length in ranges:
  */
 
@@ -29306,15 +29447,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("lambda", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_x, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 339, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_x, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 346, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -29323,23 +29464,23 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pydivsufsort/stringalg.pyx":327
+/* "pydivsufsort/stringalg.pyx":334
  * 
  * 
  * def _common_substrings(np.ndarray[ull, ndim=1] suffix_array, ull[::1] lcp, ull len1, ull limit):             # <<<<<<<<<<<<<<
  *     n = len(suffix_array)
  *     ranges = repeated_substrings(suffix_array, lcp)
  */
 
-static PyObject *__pyx_pf_12pydivsufsort_9stringalg_22_common_substrings(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_suffix_array, __Pyx_memviewslice __pyx_v_lcp, __pyx_t_12pydivsufsort_9stringalg_ull __pyx_v_len1, __pyx_t_12pydivsufsort_9stringalg_ull __pyx_v_limit) {
+static PyObject *__pyx_pf_12pydivsufsort_9stringalg_24_common_substrings(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_suffix_array, __Pyx_memviewslice __pyx_v_lcp, __pyx_t_12pydivsufsort_9stringalg_ull __pyx_v_len1, __pyx_t_12pydivsufsort_9stringalg_ull __pyx_v_limit) {
   PyObject *__pyx_v_n = NULL;
   PyObject *__pyx_v_ranges = NULL;
   PyObject *__pyx_v_origin = NULL;
   PyArrayObject *__pyx_v_origin_cumsum = 0;
   std::map<std::pair<__pyx_t_12pydivsufsort_9stringalg_ull,__pyx_t_12pydivsufsort_9stringalg_ull> ,__pyx_t_12pydivsufsort_9stringalg_ull>  __pyx_v_ans;
   std::vector<__pyx_t_5numpy_uint64_t>  __pyx_v_start1;
   std::vector<__pyx_t_5numpy_uint64_t>  __pyx_v_start2;
@@ -29399,222 +29540,222 @@
   __pyx_pybuffernd_origin_cumsum.rcbuffer = &__pyx_pybuffer_origin_cumsum;
   __pyx_pybuffer_suffix_array.pybuffer.buf = NULL;
   __pyx_pybuffer_suffix_array.refcount = 0;
   __pyx_pybuffernd_suffix_array.data = NULL;
   __pyx_pybuffernd_suffix_array.rcbuffer = &__pyx_pybuffer_suffix_array;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_suffix_array.rcbuffer->pybuffer, (PyObject*)__pyx_v_suffix_array, &__Pyx_TypeInfo_nn___pyx_t_12pydivsufsort_9stringalg_ull, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 327, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_suffix_array.rcbuffer->pybuffer, (PyObject*)__pyx_v_suffix_array, &__Pyx_TypeInfo_nn___pyx_t_12pydivsufsort_9stringalg_ull, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 334, __pyx_L1_error)
   }
   __pyx_pybuffernd_suffix_array.diminfo[0].strides = __pyx_pybuffernd_suffix_array.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_suffix_array.diminfo[0].shape = __pyx_pybuffernd_suffix_array.rcbuffer->pybuffer.shape[0];
 
-  /* "pydivsufsort/stringalg.pyx":328
+  /* "pydivsufsort/stringalg.pyx":335
  * 
  * def _common_substrings(np.ndarray[ull, ndim=1] suffix_array, ull[::1] lcp, ull len1, ull limit):
  *     n = len(suffix_array)             # <<<<<<<<<<<<<<
  *     ranges = repeated_substrings(suffix_array, lcp)
  *     # origin_cumsum can be use to check faster that
  */
-  __pyx_t_1 = PyObject_Length(((PyObject *)__pyx_v_suffix_array)); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 328, __pyx_L1_error)
-  __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 328, __pyx_L1_error)
+  __pyx_t_1 = PyObject_Length(((PyObject *)__pyx_v_suffix_array)); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 335, __pyx_L1_error)
+  __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 335, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_v_n = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "pydivsufsort/stringalg.pyx":329
+  /* "pydivsufsort/stringalg.pyx":336
  * def _common_substrings(np.ndarray[ull, ndim=1] suffix_array, ull[::1] lcp, ull len1, ull limit):
  *     n = len(suffix_array)
  *     ranges = repeated_substrings(suffix_array, lcp)             # <<<<<<<<<<<<<<
  *     # origin_cumsum can be use to check faster that
  *     # a range contains only suffixes from s1 or s2
  */
-  __pyx_t_3 = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_12pydivsufsort_9stringalg_ull(((PyObject *)__pyx_v_suffix_array), PyBUF_WRITABLE); if (unlikely(!__pyx_t_3.memview)) __PYX_ERR(0, 329, __pyx_L1_error)
-  __pyx_t_2 = __pyx_f_12pydivsufsort_9stringalg_repeated_substrings(__pyx_t_3, __pyx_v_lcp, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 329, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_12pydivsufsort_9stringalg_ull(((PyObject *)__pyx_v_suffix_array), PyBUF_WRITABLE); if (unlikely(!__pyx_t_3.memview)) __PYX_ERR(0, 336, __pyx_L1_error)
+  __pyx_t_2 = __pyx_f_12pydivsufsort_9stringalg_repeated_substrings(__pyx_t_3, __pyx_v_lcp, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 336, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __PYX_XDEC_MEMVIEW(&__pyx_t_3, 1);
   __pyx_t_3.memview = NULL;
   __pyx_t_3.data = NULL;
   __pyx_v_ranges = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "pydivsufsort/stringalg.pyx":332
+  /* "pydivsufsort/stringalg.pyx":339
  *     # origin_cumsum can be use to check faster that
  *     # a range contains only suffixes from s1 or s2
  *     origin = suffix_array < len1             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[ull, ndim=1] origin_cumsum = np.empty(n + 1, dtype=np.uint64)
  *     origin_cumsum[0] = 0
  */
-  __pyx_t_2 = __Pyx_PyInt_From_npy_uint64(__pyx_v_len1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 332, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_npy_uint64(__pyx_v_len1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 339, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = PyObject_RichCompare(((PyObject *)__pyx_v_suffix_array), __pyx_t_2, Py_LT); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 332, __pyx_L1_error)
+  __pyx_t_4 = PyObject_RichCompare(((PyObject *)__pyx_v_suffix_array), __pyx_t_2, Py_LT); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 339, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_origin = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "pydivsufsort/stringalg.pyx":333
+  /* "pydivsufsort/stringalg.pyx":340
  *     # a range contains only suffixes from s1 or s2
  *     origin = suffix_array < len1
  *     cdef np.ndarray[ull, ndim=1] origin_cumsum = np.empty(n + 1, dtype=np.uint64)             # <<<<<<<<<<<<<<
  *     origin_cumsum[0] = 0
  *     origin_cumsum[1:] = np.cumsum(origin)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 333, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 340, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 333, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 340, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyInt_AddObjC(__pyx_v_n, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 333, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_AddObjC(__pyx_v_n, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 340, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 333, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 340, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_4);
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 333, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 340, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 333, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 340, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_uint64); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 333, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_uint64); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 340, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_7) < 0) __PYX_ERR(0, 333, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_7) < 0) __PYX_ERR(0, 340, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 333, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 340, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (!(likely(((__pyx_t_7) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_7, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 333, __pyx_L1_error)
+  if (!(likely(((__pyx_t_7) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_7, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 340, __pyx_L1_error)
   __pyx_t_8 = ((PyArrayObject *)__pyx_t_7);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_origin_cumsum.rcbuffer->pybuffer, (PyObject*)__pyx_t_8, &__Pyx_TypeInfo_nn___pyx_t_12pydivsufsort_9stringalg_ull, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_origin_cumsum = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_origin_cumsum.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 333, __pyx_L1_error)
+      __PYX_ERR(0, 340, __pyx_L1_error)
     } else {__pyx_pybuffernd_origin_cumsum.diminfo[0].strides = __pyx_pybuffernd_origin_cumsum.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_origin_cumsum.diminfo[0].shape = __pyx_pybuffernd_origin_cumsum.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_8 = 0;
   __pyx_v_origin_cumsum = ((PyArrayObject *)__pyx_t_7);
   __pyx_t_7 = 0;
 
-  /* "pydivsufsort/stringalg.pyx":334
+  /* "pydivsufsort/stringalg.pyx":341
  *     origin = suffix_array < len1
  *     cdef np.ndarray[ull, ndim=1] origin_cumsum = np.empty(n + 1, dtype=np.uint64)
  *     origin_cumsum[0] = 0             # <<<<<<<<<<<<<<
  *     origin_cumsum[1:] = np.cumsum(origin)
  * 
  */
   __pyx_t_9 = 0;
   *__Pyx_BufPtrStrided1d(__pyx_t_12pydivsufsort_9stringalg_ull *, __pyx_pybuffernd_origin_cumsum.rcbuffer->pybuffer.buf, __pyx_t_9, __pyx_pybuffernd_origin_cumsum.diminfo[0].strides) = 0;
 
-  /* "pydivsufsort/stringalg.pyx":335
+  /* "pydivsufsort/stringalg.pyx":342
  *     cdef np.ndarray[ull, ndim=1] origin_cumsum = np.empty(n + 1, dtype=np.uint64)
  *     origin_cumsum[0] = 0
  *     origin_cumsum[1:] = np.cumsum(origin)             # <<<<<<<<<<<<<<
  * 
  *     cdef cpp_map[pair[ull, ull], ull] ans
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 335, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 342, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_cumsum); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 335, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_cumsum); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 342, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_7 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_4, __pyx_v_origin) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_v_origin);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 335, __pyx_L1_error)
+  if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 342, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_origin_cumsum), __pyx_slice__8, __pyx_t_7) < 0)) __PYX_ERR(0, 335, __pyx_L1_error)
+  if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_origin_cumsum), __pyx_slice__8, __pyx_t_7) < 0)) __PYX_ERR(0, 342, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pydivsufsort/stringalg.pyx":339
+  /* "pydivsufsort/stringalg.pyx":346
  *     cdef cpp_map[pair[ull, ull], ull] ans
  *     cdef vector[np.uint64_t] start1, start2
  *     ranges.sort(key=lambda x: x[2]) # sort to avoid membership test             # <<<<<<<<<<<<<<
  *     cdef ull start, end, length, diff
  *     for start, end, length in ranges:
  */
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_ranges, __pyx_n_s_sort); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 339, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_ranges, __pyx_n_s_sort); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 346, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 339, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 346, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_12pydivsufsort_9stringalg_18_common_substrings_lambda, 0, __pyx_n_s_common_substrings_locals_lambda, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 339, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_12pydivsufsort_9stringalg_18_common_substrings_lambda, 0, __pyx_n_s_common_substrings_locals_lambda, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 346, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_key, __pyx_t_4) < 0) __PYX_ERR(0, 339, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_key, __pyx_t_4) < 0) __PYX_ERR(0, 346, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_empty_tuple, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 339, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_empty_tuple, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 346, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "pydivsufsort/stringalg.pyx":341
+  /* "pydivsufsort/stringalg.pyx":348
  *     ranges.sort(key=lambda x: x[2]) # sort to avoid membership test
  *     cdef ull start, end, length, diff
  *     for start, end, length in ranges:             # <<<<<<<<<<<<<<
  *         if length < limit:
  *             continue
  */
   if (likely(PyList_CheckExact(__pyx_v_ranges)) || PyTuple_CheckExact(__pyx_v_ranges)) {
     __pyx_t_4 = __pyx_v_ranges; __Pyx_INCREF(__pyx_t_4); __pyx_t_1 = 0;
     __pyx_t_10 = NULL;
   } else {
-    __pyx_t_1 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_ranges); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 341, __pyx_L1_error)
+    __pyx_t_1 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_ranges); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 348, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_10 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 341, __pyx_L1_error)
+    __pyx_t_10 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 348, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_10)) {
       if (likely(PyList_CheckExact(__pyx_t_4))) {
         if (__pyx_t_1 >= PyList_GET_SIZE(__pyx_t_4)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_5 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 341, __pyx_L1_error)
+        __pyx_t_5 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 348, __pyx_L1_error)
         #else
-        __pyx_t_5 = PySequence_ITEM(__pyx_t_4, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 341, __pyx_L1_error)
+        __pyx_t_5 = PySequence_ITEM(__pyx_t_4, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 348, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         #endif
       } else {
         if (__pyx_t_1 >= PyTuple_GET_SIZE(__pyx_t_4)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 341, __pyx_L1_error)
+        __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 348, __pyx_L1_error)
         #else
-        __pyx_t_5 = PySequence_ITEM(__pyx_t_4, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 341, __pyx_L1_error)
+        __pyx_t_5 = PySequence_ITEM(__pyx_t_4, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 348, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         #endif
       }
     } else {
       __pyx_t_5 = __pyx_t_10(__pyx_t_4);
       if (unlikely(!__pyx_t_5)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 341, __pyx_L1_error)
+          else __PYX_ERR(0, 348, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_5);
     }
     if ((likely(PyTuple_CheckExact(__pyx_t_5))) || (PyList_CheckExact(__pyx_t_5))) {
       PyObject* sequence = __pyx_t_5;
       Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
       if (unlikely(size != 3)) {
         if (size > 3) __Pyx_RaiseTooManyValuesError(3);
         else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-        __PYX_ERR(0, 341, __pyx_L1_error)
+        __PYX_ERR(0, 348, __pyx_L1_error)
       }
       #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
       if (likely(PyTuple_CheckExact(sequence))) {
         __pyx_t_7 = PyTuple_GET_ITEM(sequence, 0); 
         __pyx_t_2 = PyTuple_GET_ITEM(sequence, 1); 
         __pyx_t_6 = PyTuple_GET_ITEM(sequence, 2); 
       } else {
@@ -29622,95 +29763,95 @@
         __pyx_t_2 = PyList_GET_ITEM(sequence, 1); 
         __pyx_t_6 = PyList_GET_ITEM(sequence, 2); 
       }
       __Pyx_INCREF(__pyx_t_7);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_6);
       #else
-      __pyx_t_7 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 341, __pyx_L1_error)
+      __pyx_t_7 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 348, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
-      __pyx_t_2 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 341, __pyx_L1_error)
+      __pyx_t_2 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 348, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_6 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 341, __pyx_L1_error)
+      __pyx_t_6 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 348, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       #endif
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     } else {
       Py_ssize_t index = -1;
-      __pyx_t_11 = PyObject_GetIter(__pyx_t_5); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 341, __pyx_L1_error)
+      __pyx_t_11 = PyObject_GetIter(__pyx_t_5); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 348, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_t_12 = Py_TYPE(__pyx_t_11)->tp_iternext;
       index = 0; __pyx_t_7 = __pyx_t_12(__pyx_t_11); if (unlikely(!__pyx_t_7)) goto __pyx_L5_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_7);
       index = 1; __pyx_t_2 = __pyx_t_12(__pyx_t_11); if (unlikely(!__pyx_t_2)) goto __pyx_L5_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_2);
       index = 2; __pyx_t_6 = __pyx_t_12(__pyx_t_11); if (unlikely(!__pyx_t_6)) goto __pyx_L5_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_6);
-      if (__Pyx_IternextUnpackEndCheck(__pyx_t_12(__pyx_t_11), 3) < 0) __PYX_ERR(0, 341, __pyx_L1_error)
+      if (__Pyx_IternextUnpackEndCheck(__pyx_t_12(__pyx_t_11), 3) < 0) __PYX_ERR(0, 348, __pyx_L1_error)
       __pyx_t_12 = NULL;
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
       goto __pyx_L6_unpacking_done;
       __pyx_L5_unpacking_failed:;
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
       __pyx_t_12 = NULL;
       if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-      __PYX_ERR(0, 341, __pyx_L1_error)
+      __PYX_ERR(0, 348, __pyx_L1_error)
       __pyx_L6_unpacking_done:;
     }
-    __pyx_t_13 = __Pyx_PyInt_As_npy_uint64(__pyx_t_7); if (unlikely((__pyx_t_13 == ((npy_uint64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 341, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyInt_As_npy_uint64(__pyx_t_7); if (unlikely((__pyx_t_13 == ((npy_uint64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 348, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_14 = __Pyx_PyInt_As_npy_uint64(__pyx_t_2); if (unlikely((__pyx_t_14 == ((npy_uint64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 341, __pyx_L1_error)
+    __pyx_t_14 = __Pyx_PyInt_As_npy_uint64(__pyx_t_2); if (unlikely((__pyx_t_14 == ((npy_uint64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 348, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_15 = __Pyx_PyInt_As_npy_uint64(__pyx_t_6); if (unlikely((__pyx_t_15 == ((npy_uint64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 341, __pyx_L1_error)
+    __pyx_t_15 = __Pyx_PyInt_As_npy_uint64(__pyx_t_6); if (unlikely((__pyx_t_15 == ((npy_uint64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 348, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_v_start = __pyx_t_13;
     __pyx_v_end = __pyx_t_14;
     __pyx_v_length = __pyx_t_15;
 
-    /* "pydivsufsort/stringalg.pyx":342
+    /* "pydivsufsort/stringalg.pyx":349
  *     cdef ull start, end, length, diff
  *     for start, end, length in ranges:
  *         if length < limit:             # <<<<<<<<<<<<<<
  *             continue
  *         diff = origin_cumsum[end] - origin_cumsum[start]
  */
     __pyx_t_16 = ((__pyx_v_length < __pyx_v_limit) != 0);
     if (__pyx_t_16) {
 
-      /* "pydivsufsort/stringalg.pyx":343
+      /* "pydivsufsort/stringalg.pyx":350
  *     for start, end, length in ranges:
  *         if length < limit:
  *             continue             # <<<<<<<<<<<<<<
  *         diff = origin_cumsum[end] - origin_cumsum[start]
  *         if diff == 0 or diff == end - start:
  */
       goto __pyx_L3_continue;
 
-      /* "pydivsufsort/stringalg.pyx":342
+      /* "pydivsufsort/stringalg.pyx":349
  *     cdef ull start, end, length, diff
  *     for start, end, length in ranges:
  *         if length < limit:             # <<<<<<<<<<<<<<
  *             continue
  *         diff = origin_cumsum[end] - origin_cumsum[start]
  */
     }
 
-    /* "pydivsufsort/stringalg.pyx":344
+    /* "pydivsufsort/stringalg.pyx":351
  *         if length < limit:
  *             continue
  *         diff = origin_cumsum[end] - origin_cumsum[start]             # <<<<<<<<<<<<<<
  *         if diff == 0 or diff == end - start:
  *             continue
  */
     __pyx_t_15 = __pyx_v_end;
     __pyx_t_14 = __pyx_v_start;
     __pyx_v_diff = ((*__Pyx_BufPtrStrided1d(__pyx_t_12pydivsufsort_9stringalg_ull *, __pyx_pybuffernd_origin_cumsum.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_origin_cumsum.diminfo[0].strides)) - (*__Pyx_BufPtrStrided1d(__pyx_t_12pydivsufsort_9stringalg_ull *, __pyx_pybuffernd_origin_cumsum.rcbuffer->pybuffer.buf, __pyx_t_14, __pyx_pybuffernd_origin_cumsum.diminfo[0].strides)));
 
-    /* "pydivsufsort/stringalg.pyx":345
+    /* "pydivsufsort/stringalg.pyx":352
  *             continue
  *         diff = origin_cumsum[end] - origin_cumsum[start]
  *         if diff == 0 or diff == end - start:             # <<<<<<<<<<<<<<
  *             continue
  *         start1.clear()
  */
     __pyx_t_17 = ((__pyx_v_diff == 0) != 0);
@@ -29720,633 +29861,633 @@
       goto __pyx_L9_bool_binop_done;
     }
     __pyx_t_17 = ((__pyx_v_diff == (__pyx_v_end - __pyx_v_start)) != 0);
     __pyx_t_16 = __pyx_t_17;
     __pyx_L9_bool_binop_done:;
     if (__pyx_t_16) {
 
-      /* "pydivsufsort/stringalg.pyx":346
+      /* "pydivsufsort/stringalg.pyx":353
  *         diff = origin_cumsum[end] - origin_cumsum[start]
  *         if diff == 0 or diff == end - start:
  *             continue             # <<<<<<<<<<<<<<
  *         start1.clear()
  *         start2.clear()
  */
       goto __pyx_L3_continue;
 
-      /* "pydivsufsort/stringalg.pyx":345
+      /* "pydivsufsort/stringalg.pyx":352
  *             continue
  *         diff = origin_cumsum[end] - origin_cumsum[start]
  *         if diff == 0 or diff == end - start:             # <<<<<<<<<<<<<<
  *             continue
  *         start1.clear()
  */
     }
 
-    /* "pydivsufsort/stringalg.pyx":347
+    /* "pydivsufsort/stringalg.pyx":354
  *         if diff == 0 or diff == end - start:
  *             continue
  *         start1.clear()             # <<<<<<<<<<<<<<
  *         start2.clear()
  *         for i in range(start, end):
  */
     __pyx_v_start1.clear();
 
-    /* "pydivsufsort/stringalg.pyx":348
+    /* "pydivsufsort/stringalg.pyx":355
  *             continue
  *         start1.clear()
  *         start2.clear()             # <<<<<<<<<<<<<<
  *         for i in range(start, end):
  *             pos = suffix_array[i]
  */
     __pyx_v_start2.clear();
 
-    /* "pydivsufsort/stringalg.pyx":349
+    /* "pydivsufsort/stringalg.pyx":356
  *         start1.clear()
  *         start2.clear()
  *         for i in range(start, end):             # <<<<<<<<<<<<<<
  *             pos = suffix_array[i]
  *             if origin[i]: # might be faster than pos < len1 thanks to cache lookup
  */
-    __pyx_t_5 = __Pyx_PyInt_From_npy_uint64(__pyx_v_start); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 349, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_From_npy_uint64(__pyx_v_start); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 356, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = __Pyx_PyInt_From_npy_uint64(__pyx_v_end); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 349, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_From_npy_uint64(__pyx_v_end); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 356, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 349, __pyx_L1_error)
+    __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 356, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_6);
     PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_6);
     __pyx_t_5 = 0;
     __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_range, __pyx_t_2, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 349, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_range, __pyx_t_2, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 356, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     if (likely(PyList_CheckExact(__pyx_t_6)) || PyTuple_CheckExact(__pyx_t_6)) {
       __pyx_t_2 = __pyx_t_6; __Pyx_INCREF(__pyx_t_2); __pyx_t_18 = 0;
       __pyx_t_19 = NULL;
     } else {
-      __pyx_t_18 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 349, __pyx_L1_error)
+      __pyx_t_18 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 356, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_19 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 349, __pyx_L1_error)
+      __pyx_t_19 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 356, __pyx_L1_error)
     }
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     for (;;) {
       if (likely(!__pyx_t_19)) {
         if (likely(PyList_CheckExact(__pyx_t_2))) {
           if (__pyx_t_18 >= PyList_GET_SIZE(__pyx_t_2)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_6 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_18); __Pyx_INCREF(__pyx_t_6); __pyx_t_18++; if (unlikely(0 < 0)) __PYX_ERR(0, 349, __pyx_L1_error)
+          __pyx_t_6 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_18); __Pyx_INCREF(__pyx_t_6); __pyx_t_18++; if (unlikely(0 < 0)) __PYX_ERR(0, 356, __pyx_L1_error)
           #else
-          __pyx_t_6 = PySequence_ITEM(__pyx_t_2, __pyx_t_18); __pyx_t_18++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 349, __pyx_L1_error)
+          __pyx_t_6 = PySequence_ITEM(__pyx_t_2, __pyx_t_18); __pyx_t_18++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 356, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
           #endif
         } else {
           if (__pyx_t_18 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_6 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_18); __Pyx_INCREF(__pyx_t_6); __pyx_t_18++; if (unlikely(0 < 0)) __PYX_ERR(0, 349, __pyx_L1_error)
+          __pyx_t_6 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_18); __Pyx_INCREF(__pyx_t_6); __pyx_t_18++; if (unlikely(0 < 0)) __PYX_ERR(0, 356, __pyx_L1_error)
           #else
-          __pyx_t_6 = PySequence_ITEM(__pyx_t_2, __pyx_t_18); __pyx_t_18++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 349, __pyx_L1_error)
+          __pyx_t_6 = PySequence_ITEM(__pyx_t_2, __pyx_t_18); __pyx_t_18++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 356, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
           #endif
         }
       } else {
         __pyx_t_6 = __pyx_t_19(__pyx_t_2);
         if (unlikely(!__pyx_t_6)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 349, __pyx_L1_error)
+            else __PYX_ERR(0, 356, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_6);
       }
       __Pyx_XDECREF_SET(__pyx_v_i, __pyx_t_6);
       __pyx_t_6 = 0;
 
-      /* "pydivsufsort/stringalg.pyx":350
+      /* "pydivsufsort/stringalg.pyx":357
  *         start2.clear()
  *         for i in range(start, end):
  *             pos = suffix_array[i]             # <<<<<<<<<<<<<<
  *             if origin[i]: # might be faster than pos < len1 thanks to cache lookup
  *                 start1.push_back(pos)
  */
-      __pyx_t_6 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_suffix_array), __pyx_v_i); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 350, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_suffix_array), __pyx_v_i); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 357, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_XDECREF_SET(__pyx_v_pos, __pyx_t_6);
       __pyx_t_6 = 0;
 
-      /* "pydivsufsort/stringalg.pyx":351
+      /* "pydivsufsort/stringalg.pyx":358
  *         for i in range(start, end):
  *             pos = suffix_array[i]
  *             if origin[i]: # might be faster than pos < len1 thanks to cache lookup             # <<<<<<<<<<<<<<
  *                 start1.push_back(pos)
  *             else:
  */
-      __pyx_t_6 = __Pyx_PyObject_GetItem(__pyx_v_origin, __pyx_v_i); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 351, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_GetItem(__pyx_v_origin, __pyx_v_i); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 358, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(0, 351, __pyx_L1_error)
+      __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(0, 358, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       if (__pyx_t_16) {
 
-        /* "pydivsufsort/stringalg.pyx":352
+        /* "pydivsufsort/stringalg.pyx":359
  *             pos = suffix_array[i]
  *             if origin[i]: # might be faster than pos < len1 thanks to cache lookup
  *                 start1.push_back(pos)             # <<<<<<<<<<<<<<
  *             else:
  *                 start2.push_back(pos - len1 - 1)
  */
-        __pyx_t_20 = __Pyx_PyInt_As_npy_uint64(__pyx_v_pos); if (unlikely((__pyx_t_20 == ((npy_uint64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 352, __pyx_L1_error)
+        __pyx_t_20 = __Pyx_PyInt_As_npy_uint64(__pyx_v_pos); if (unlikely((__pyx_t_20 == ((npy_uint64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 359, __pyx_L1_error)
         try {
           __pyx_v_start1.push_back(__pyx_t_20);
         } catch(...) {
           __Pyx_CppExn2PyErr();
-          __PYX_ERR(0, 352, __pyx_L1_error)
+          __PYX_ERR(0, 359, __pyx_L1_error)
         }
 
-        /* "pydivsufsort/stringalg.pyx":351
+        /* "pydivsufsort/stringalg.pyx":358
  *         for i in range(start, end):
  *             pos = suffix_array[i]
  *             if origin[i]: # might be faster than pos < len1 thanks to cache lookup             # <<<<<<<<<<<<<<
  *                 start1.push_back(pos)
  *             else:
  */
         goto __pyx_L13;
       }
 
-      /* "pydivsufsort/stringalg.pyx":354
+      /* "pydivsufsort/stringalg.pyx":361
  *                 start1.push_back(pos)
  *             else:
  *                 start2.push_back(pos - len1 - 1)             # <<<<<<<<<<<<<<
  *         sort(start1.begin(), start1.end())
  *         sort(start2.begin(), start2.end())
  */
       /*else*/ {
-        __pyx_t_6 = __Pyx_PyInt_From_npy_uint64(__pyx_v_len1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 354, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyInt_From_npy_uint64(__pyx_v_len1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 361, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
-        __pyx_t_5 = PyNumber_Subtract(__pyx_v_pos, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 354, __pyx_L1_error)
+        __pyx_t_5 = PyNumber_Subtract(__pyx_v_pos, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 361, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-        __pyx_t_6 = __Pyx_PyInt_SubtractObjC(__pyx_t_5, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 354, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyInt_SubtractObjC(__pyx_t_5, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 361, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-        __pyx_t_20 = __Pyx_PyInt_As_npy_uint64(__pyx_t_6); if (unlikely((__pyx_t_20 == ((npy_uint64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 354, __pyx_L1_error)
+        __pyx_t_20 = __Pyx_PyInt_As_npy_uint64(__pyx_t_6); if (unlikely((__pyx_t_20 == ((npy_uint64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 361, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         try {
           __pyx_v_start2.push_back(__pyx_t_20);
         } catch(...) {
           __Pyx_CppExn2PyErr();
-          __PYX_ERR(0, 354, __pyx_L1_error)
+          __PYX_ERR(0, 361, __pyx_L1_error)
         }
       }
       __pyx_L13:;
 
-      /* "pydivsufsort/stringalg.pyx":349
+      /* "pydivsufsort/stringalg.pyx":356
  *         start1.clear()
  *         start2.clear()
  *         for i in range(start, end):             # <<<<<<<<<<<<<<
  *             pos = suffix_array[i]
  *             if origin[i]: # might be faster than pos < len1 thanks to cache lookup
  */
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "pydivsufsort/stringalg.pyx":355
+    /* "pydivsufsort/stringalg.pyx":362
  *             else:
  *                 start2.push_back(pos - len1 - 1)
  *         sort(start1.begin(), start1.end())             # <<<<<<<<<<<<<<
  *         sort(start2.begin(), start2.end())
  *         for i in start1:
  */
     std::sort<std::vector<__pyx_t_5numpy_uint64_t> ::iterator>(__pyx_v_start1.begin(), __pyx_v_start1.end());
 
-    /* "pydivsufsort/stringalg.pyx":356
+    /* "pydivsufsort/stringalg.pyx":363
  *                 start2.push_back(pos - len1 - 1)
  *         sort(start1.begin(), start1.end())
  *         sort(start2.begin(), start2.end())             # <<<<<<<<<<<<<<
  *         for i in start1:
  *             for j in start2:
  */
     std::sort<std::vector<__pyx_t_5numpy_uint64_t> ::iterator>(__pyx_v_start2.begin(), __pyx_v_start2.end());
 
-    /* "pydivsufsort/stringalg.pyx":357
+    /* "pydivsufsort/stringalg.pyx":364
  *         sort(start1.begin(), start1.end())
  *         sort(start2.begin(), start2.end())
  *         for i in start1:             # <<<<<<<<<<<<<<
  *             for j in start2:
  *                 # deduplicate start positions
  */
     __pyx_t_21 = __pyx_v_start1.begin();
     for (;;) {
       if (!(__pyx_t_21 != __pyx_v_start1.end())) break;
       __pyx_t_20 = *__pyx_t_21;
       ++__pyx_t_21;
-      __pyx_t_2 = __Pyx_PyInt_From_npy_uint64(__pyx_t_20); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 357, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyInt_From_npy_uint64(__pyx_t_20); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 364, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_XDECREF_SET(__pyx_v_i, __pyx_t_2);
       __pyx_t_2 = 0;
 
-      /* "pydivsufsort/stringalg.pyx":358
+      /* "pydivsufsort/stringalg.pyx":365
  *         sort(start2.begin(), start2.end())
  *         for i in start1:
  *             for j in start2:             # <<<<<<<<<<<<<<
  *                 # deduplicate start positions
  *                 # needed first to remove smaller matches
  */
       __pyx_t_22 = __pyx_v_start2.begin();
       for (;;) {
         if (!(__pyx_t_22 != __pyx_v_start2.end())) break;
         __pyx_t_20 = *__pyx_t_22;
         ++__pyx_t_22;
-        __pyx_t_2 = __Pyx_PyInt_From_npy_uint64(__pyx_t_20); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 358, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PyInt_From_npy_uint64(__pyx_t_20); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 365, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_XDECREF_SET(__pyx_v_j, __pyx_t_2);
         __pyx_t_2 = 0;
 
-        /* "pydivsufsort/stringalg.pyx":361
+        /* "pydivsufsort/stringalg.pyx":368
  *                 # deduplicate start positions
  *                 # needed first to remove smaller matches
  *                 ans[i, j] = length             # <<<<<<<<<<<<<<
  * 
  *     # deduplicate end positions
  */
-        __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 361, __pyx_L1_error)
+        __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 368, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_INCREF(__pyx_v_i);
         __Pyx_GIVEREF(__pyx_v_i);
         PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_i);
         __Pyx_INCREF(__pyx_v_j);
         __Pyx_GIVEREF(__pyx_v_j);
         PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_v_j);
-        __pyx_t_23 = __pyx_convert_pair_from_py___pyx_t_12pydivsufsort_9stringalg_ull__and___pyx_t_12pydivsufsort_9stringalg_ull(__pyx_t_2); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 361, __pyx_L1_error)
+        __pyx_t_23 = __pyx_convert_pair_from_py___pyx_t_12pydivsufsort_9stringalg_ull__and___pyx_t_12pydivsufsort_9stringalg_ull(__pyx_t_2); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 368, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         (__pyx_v_ans[__pyx_t_23]) = __pyx_v_length;
 
-        /* "pydivsufsort/stringalg.pyx":358
+        /* "pydivsufsort/stringalg.pyx":365
  *         sort(start2.begin(), start2.end())
  *         for i in start1:
  *             for j in start2:             # <<<<<<<<<<<<<<
  *                 # deduplicate start positions
  *                 # needed first to remove smaller matches
  */
       }
 
-      /* "pydivsufsort/stringalg.pyx":357
+      /* "pydivsufsort/stringalg.pyx":364
  *         sort(start1.begin(), start1.end())
  *         sort(start2.begin(), start2.end())
  *         for i in start1:             # <<<<<<<<<<<<<<
  *             for j in start2:
  *                 # deduplicate start positions
  */
     }
 
-    /* "pydivsufsort/stringalg.pyx":341
+    /* "pydivsufsort/stringalg.pyx":348
  *     ranges.sort(key=lambda x: x[2]) # sort to avoid membership test
  *     cdef ull start, end, length, diff
  *     for start, end, length in ranges:             # <<<<<<<<<<<<<<
  *         if length < limit:
  *             continue
  */
     __pyx_L3_continue:;
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "pydivsufsort/stringalg.pyx":365
+  /* "pydivsufsort/stringalg.pyx":372
  *     # deduplicate end positions
  *     cdef cpp_map[pair[ull, ull], ull] ans1
  *     for (i, j), l in ans:             # <<<<<<<<<<<<<<
  *         i += l
  *         j += l
  */
   __pyx_t_24 = __pyx_v_ans.begin();
   for (;;) {
     if (!(__pyx_t_24 != __pyx_v_ans.end())) break;
     __pyx_t_25 = *__pyx_t_24;
     ++__pyx_t_24;
-    __pyx_t_4 = __pyx_convert_pair_to_py_std_3a__3a_pair_3c___pyx_t_12pydivsufsort_9stringalg_ull_2c___pyx_t_12pydivsufsort_9stringalg_ull_3e_________pyx_t_12pydivsufsort_9stringalg_ull(__pyx_t_25); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 365, __pyx_L1_error)
+    __pyx_t_4 = __pyx_convert_pair_to_py_std_3a__3a_pair_3c___pyx_t_12pydivsufsort_9stringalg_ull_2c___pyx_t_12pydivsufsort_9stringalg_ull_3e_________pyx_t_12pydivsufsort_9stringalg_ull(__pyx_t_25); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 372, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     if ((likely(PyTuple_CheckExact(__pyx_t_4))) || (PyList_CheckExact(__pyx_t_4))) {
       PyObject* sequence = __pyx_t_4;
       Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
       if (unlikely(size != 2)) {
         if (size > 2) __Pyx_RaiseTooManyValuesError(2);
         else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-        __PYX_ERR(0, 365, __pyx_L1_error)
+        __PYX_ERR(0, 372, __pyx_L1_error)
       }
       #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
       if (likely(PyTuple_CheckExact(sequence))) {
         __pyx_t_2 = PyTuple_GET_ITEM(sequence, 0); 
         __pyx_t_6 = PyTuple_GET_ITEM(sequence, 1); 
       } else {
         __pyx_t_2 = PyList_GET_ITEM(sequence, 0); 
         __pyx_t_6 = PyList_GET_ITEM(sequence, 1); 
       }
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_6);
       #else
-      __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 365, __pyx_L1_error)
+      __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 372, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_6 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 365, __pyx_L1_error)
+      __pyx_t_6 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 372, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       #endif
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     } else {
       Py_ssize_t index = -1;
-      __pyx_t_5 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 365, __pyx_L1_error)
+      __pyx_t_5 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 372, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_t_12 = Py_TYPE(__pyx_t_5)->tp_iternext;
       index = 0; __pyx_t_2 = __pyx_t_12(__pyx_t_5); if (unlikely(!__pyx_t_2)) goto __pyx_L20_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_2);
       index = 1; __pyx_t_6 = __pyx_t_12(__pyx_t_5); if (unlikely(!__pyx_t_6)) goto __pyx_L20_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_6);
-      if (__Pyx_IternextUnpackEndCheck(__pyx_t_12(__pyx_t_5), 2) < 0) __PYX_ERR(0, 365, __pyx_L1_error)
+      if (__Pyx_IternextUnpackEndCheck(__pyx_t_12(__pyx_t_5), 2) < 0) __PYX_ERR(0, 372, __pyx_L1_error)
       __pyx_t_12 = NULL;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       goto __pyx_L21_unpacking_done;
       __pyx_L20_unpacking_failed:;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_t_12 = NULL;
       if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-      __PYX_ERR(0, 365, __pyx_L1_error)
+      __PYX_ERR(0, 372, __pyx_L1_error)
       __pyx_L21_unpacking_done:;
     }
     if ((likely(PyTuple_CheckExact(__pyx_t_2))) || (PyList_CheckExact(__pyx_t_2))) {
       PyObject* sequence = __pyx_t_2;
       Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
       if (unlikely(size != 2)) {
         if (size > 2) __Pyx_RaiseTooManyValuesError(2);
         else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-        __PYX_ERR(0, 365, __pyx_L1_error)
+        __PYX_ERR(0, 372, __pyx_L1_error)
       }
       #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
       if (likely(PyTuple_CheckExact(sequence))) {
         __pyx_t_5 = PyTuple_GET_ITEM(sequence, 0); 
         __pyx_t_7 = PyTuple_GET_ITEM(sequence, 1); 
       } else {
         __pyx_t_5 = PyList_GET_ITEM(sequence, 0); 
         __pyx_t_7 = PyList_GET_ITEM(sequence, 1); 
       }
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_7);
       #else
-      __pyx_t_5 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 365, __pyx_L1_error)
+      __pyx_t_5 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 372, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_7 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 365, __pyx_L1_error)
+      __pyx_t_7 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 372, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       #endif
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     } else {
       Py_ssize_t index = -1;
-      __pyx_t_11 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 365, __pyx_L1_error)
+      __pyx_t_11 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 372, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __pyx_t_12 = Py_TYPE(__pyx_t_11)->tp_iternext;
       index = 0; __pyx_t_5 = __pyx_t_12(__pyx_t_11); if (unlikely(!__pyx_t_5)) goto __pyx_L22_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_5);
       index = 1; __pyx_t_7 = __pyx_t_12(__pyx_t_11); if (unlikely(!__pyx_t_7)) goto __pyx_L22_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_7);
-      if (__Pyx_IternextUnpackEndCheck(__pyx_t_12(__pyx_t_11), 2) < 0) __PYX_ERR(0, 365, __pyx_L1_error)
+      if (__Pyx_IternextUnpackEndCheck(__pyx_t_12(__pyx_t_11), 2) < 0) __PYX_ERR(0, 372, __pyx_L1_error)
       __pyx_t_12 = NULL;
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
       goto __pyx_L23_unpacking_done;
       __pyx_L22_unpacking_failed:;
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
       __pyx_t_12 = NULL;
       if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-      __PYX_ERR(0, 365, __pyx_L1_error)
+      __PYX_ERR(0, 372, __pyx_L1_error)
       __pyx_L23_unpacking_done:;
     }
     __Pyx_XDECREF_SET(__pyx_v_i, __pyx_t_5);
     __pyx_t_5 = 0;
     __Pyx_XDECREF_SET(__pyx_v_j, __pyx_t_7);
     __pyx_t_7 = 0;
     __Pyx_XDECREF_SET(__pyx_v_l, __pyx_t_6);
     __pyx_t_6 = 0;
 
-    /* "pydivsufsort/stringalg.pyx":366
+    /* "pydivsufsort/stringalg.pyx":373
  *     cdef cpp_map[pair[ull, ull], ull] ans1
  *     for (i, j), l in ans:
  *         i += l             # <<<<<<<<<<<<<<
  *         j += l
  *         if ans1[i, j] < l:
  */
-    __pyx_t_4 = PyNumber_InPlaceAdd(__pyx_v_i, __pyx_v_l); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 366, __pyx_L1_error)
+    __pyx_t_4 = PyNumber_InPlaceAdd(__pyx_v_i, __pyx_v_l); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 373, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF_SET(__pyx_v_i, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "pydivsufsort/stringalg.pyx":367
+    /* "pydivsufsort/stringalg.pyx":374
  *     for (i, j), l in ans:
  *         i += l
  *         j += l             # <<<<<<<<<<<<<<
  *         if ans1[i, j] < l:
  *             ans1[i, j] = l
  */
-    __pyx_t_4 = PyNumber_InPlaceAdd(__pyx_v_j, __pyx_v_l); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 367, __pyx_L1_error)
+    __pyx_t_4 = PyNumber_InPlaceAdd(__pyx_v_j, __pyx_v_l); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 374, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF_SET(__pyx_v_j, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "pydivsufsort/stringalg.pyx":368
+    /* "pydivsufsort/stringalg.pyx":375
  *         i += l
  *         j += l
  *         if ans1[i, j] < l:             # <<<<<<<<<<<<<<
  *             ans1[i, j] = l
  * 
  */
-    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 368, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 375, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_INCREF(__pyx_v_i);
     __Pyx_GIVEREF(__pyx_v_i);
     PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_v_i);
     __Pyx_INCREF(__pyx_v_j);
     __Pyx_GIVEREF(__pyx_v_j);
     PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_v_j);
-    __pyx_t_23 = __pyx_convert_pair_from_py___pyx_t_12pydivsufsort_9stringalg_ull__and___pyx_t_12pydivsufsort_9stringalg_ull(__pyx_t_4); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 368, __pyx_L1_error)
+    __pyx_t_23 = __pyx_convert_pair_from_py___pyx_t_12pydivsufsort_9stringalg_ull__and___pyx_t_12pydivsufsort_9stringalg_ull(__pyx_t_4); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 375, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyInt_From_npy_uint64((__pyx_v_ans1[__pyx_t_23])); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 368, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_npy_uint64((__pyx_v_ans1[__pyx_t_23])); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 375, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_6 = PyObject_RichCompare(__pyx_t_4, __pyx_v_l, Py_LT); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 368, __pyx_L1_error)
+    __pyx_t_6 = PyObject_RichCompare(__pyx_t_4, __pyx_v_l, Py_LT); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 375, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(0, 368, __pyx_L1_error)
+    __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(0, 375, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     if (__pyx_t_16) {
 
-      /* "pydivsufsort/stringalg.pyx":369
+      /* "pydivsufsort/stringalg.pyx":376
  *         j += l
  *         if ans1[i, j] < l:
  *             ans1[i, j] = l             # <<<<<<<<<<<<<<
  * 
  *     ans2 = [(i - l, j - l, l) for (i, j), l in ans1]
  */
-      __pyx_t_14 = __Pyx_PyInt_As_npy_uint64(__pyx_v_l); if (unlikely((__pyx_t_14 == ((npy_uint64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 369, __pyx_L1_error)
-      __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 369, __pyx_L1_error)
+      __pyx_t_14 = __Pyx_PyInt_As_npy_uint64(__pyx_v_l); if (unlikely((__pyx_t_14 == ((npy_uint64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 376, __pyx_L1_error)
+      __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 376, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_INCREF(__pyx_v_i);
       __Pyx_GIVEREF(__pyx_v_i);
       PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_v_i);
       __Pyx_INCREF(__pyx_v_j);
       __Pyx_GIVEREF(__pyx_v_j);
       PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_v_j);
-      __pyx_t_23 = __pyx_convert_pair_from_py___pyx_t_12pydivsufsort_9stringalg_ull__and___pyx_t_12pydivsufsort_9stringalg_ull(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 369, __pyx_L1_error)
+      __pyx_t_23 = __pyx_convert_pair_from_py___pyx_t_12pydivsufsort_9stringalg_ull__and___pyx_t_12pydivsufsort_9stringalg_ull(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 376, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       (__pyx_v_ans1[__pyx_t_23]) = __pyx_t_14;
 
-      /* "pydivsufsort/stringalg.pyx":368
+      /* "pydivsufsort/stringalg.pyx":375
  *         i += l
  *         j += l
  *         if ans1[i, j] < l:             # <<<<<<<<<<<<<<
  *             ans1[i, j] = l
  * 
  */
     }
 
-    /* "pydivsufsort/stringalg.pyx":365
+    /* "pydivsufsort/stringalg.pyx":372
  *     # deduplicate end positions
  *     cdef cpp_map[pair[ull, ull], ull] ans1
  *     for (i, j), l in ans:             # <<<<<<<<<<<<<<
  *         i += l
  *         j += l
  */
   }
 
-  /* "pydivsufsort/stringalg.pyx":371
+  /* "pydivsufsort/stringalg.pyx":378
  *             ans1[i, j] = l
  * 
  *     ans2 = [(i - l, j - l, l) for (i, j), l in ans1]             # <<<<<<<<<<<<<<
  *     ans2.sort()
  *     return ans2
  */
   { /* enter inner scope */
-    __pyx_t_6 = PyList_New(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 371, __pyx_L27_error)
+    __pyx_t_6 = PyList_New(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 378, __pyx_L27_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_24 = __pyx_v_ans1.begin();
     for (;;) {
       if (!(__pyx_t_24 != __pyx_v_ans1.end())) break;
       __pyx_t_25 = *__pyx_t_24;
       ++__pyx_t_24;
-      __pyx_t_4 = __pyx_convert_pair_to_py_std_3a__3a_pair_3c___pyx_t_12pydivsufsort_9stringalg_ull_2c___pyx_t_12pydivsufsort_9stringalg_ull_3e_________pyx_t_12pydivsufsort_9stringalg_ull(__pyx_t_25); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 371, __pyx_L27_error)
+      __pyx_t_4 = __pyx_convert_pair_to_py_std_3a__3a_pair_3c___pyx_t_12pydivsufsort_9stringalg_ull_2c___pyx_t_12pydivsufsort_9stringalg_ull_3e_________pyx_t_12pydivsufsort_9stringalg_ull(__pyx_t_25); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 378, __pyx_L27_error)
       __Pyx_GOTREF(__pyx_t_4);
       if ((likely(PyTuple_CheckExact(__pyx_t_4))) || (PyList_CheckExact(__pyx_t_4))) {
         PyObject* sequence = __pyx_t_4;
         Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
         if (unlikely(size != 2)) {
           if (size > 2) __Pyx_RaiseTooManyValuesError(2);
           else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-          __PYX_ERR(0, 371, __pyx_L27_error)
+          __PYX_ERR(0, 378, __pyx_L27_error)
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
         if (likely(PyTuple_CheckExact(sequence))) {
           __pyx_t_2 = PyTuple_GET_ITEM(sequence, 0); 
           __pyx_t_7 = PyTuple_GET_ITEM(sequence, 1); 
         } else {
           __pyx_t_2 = PyList_GET_ITEM(sequence, 0); 
           __pyx_t_7 = PyList_GET_ITEM(sequence, 1); 
         }
         __Pyx_INCREF(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_7);
         #else
-        __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 371, __pyx_L27_error)
+        __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 378, __pyx_L27_error)
         __Pyx_GOTREF(__pyx_t_2);
-        __pyx_t_7 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 371, __pyx_L27_error)
+        __pyx_t_7 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 378, __pyx_L27_error)
         __Pyx_GOTREF(__pyx_t_7);
         #endif
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       } else {
         Py_ssize_t index = -1;
-        __pyx_t_5 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 371, __pyx_L27_error)
+        __pyx_t_5 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 378, __pyx_L27_error)
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __pyx_t_12 = Py_TYPE(__pyx_t_5)->tp_iternext;
         index = 0; __pyx_t_2 = __pyx_t_12(__pyx_t_5); if (unlikely(!__pyx_t_2)) goto __pyx_L30_unpacking_failed;
         __Pyx_GOTREF(__pyx_t_2);
         index = 1; __pyx_t_7 = __pyx_t_12(__pyx_t_5); if (unlikely(!__pyx_t_7)) goto __pyx_L30_unpacking_failed;
         __Pyx_GOTREF(__pyx_t_7);
-        if (__Pyx_IternextUnpackEndCheck(__pyx_t_12(__pyx_t_5), 2) < 0) __PYX_ERR(0, 371, __pyx_L27_error)
+        if (__Pyx_IternextUnpackEndCheck(__pyx_t_12(__pyx_t_5), 2) < 0) __PYX_ERR(0, 378, __pyx_L27_error)
         __pyx_t_12 = NULL;
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         goto __pyx_L31_unpacking_done;
         __pyx_L30_unpacking_failed:;
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         __pyx_t_12 = NULL;
         if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-        __PYX_ERR(0, 371, __pyx_L27_error)
+        __PYX_ERR(0, 378, __pyx_L27_error)
         __pyx_L31_unpacking_done:;
       }
       if ((likely(PyTuple_CheckExact(__pyx_t_2))) || (PyList_CheckExact(__pyx_t_2))) {
         PyObject* sequence = __pyx_t_2;
         Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
         if (unlikely(size != 2)) {
           if (size > 2) __Pyx_RaiseTooManyValuesError(2);
           else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-          __PYX_ERR(0, 371, __pyx_L27_error)
+          __PYX_ERR(0, 378, __pyx_L27_error)
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
         if (likely(PyTuple_CheckExact(sequence))) {
           __pyx_t_5 = PyTuple_GET_ITEM(sequence, 0); 
           __pyx_t_11 = PyTuple_GET_ITEM(sequence, 1); 
         } else {
           __pyx_t_5 = PyList_GET_ITEM(sequence, 0); 
           __pyx_t_11 = PyList_GET_ITEM(sequence, 1); 
         }
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_11);
         #else
-        __pyx_t_5 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 371, __pyx_L27_error)
+        __pyx_t_5 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 378, __pyx_L27_error)
         __Pyx_GOTREF(__pyx_t_5);
-        __pyx_t_11 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 371, __pyx_L27_error)
+        __pyx_t_11 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 378, __pyx_L27_error)
         __Pyx_GOTREF(__pyx_t_11);
         #endif
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       } else {
         Py_ssize_t index = -1;
-        __pyx_t_26 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_26)) __PYX_ERR(0, 371, __pyx_L27_error)
+        __pyx_t_26 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_26)) __PYX_ERR(0, 378, __pyx_L27_error)
         __Pyx_GOTREF(__pyx_t_26);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_t_12 = Py_TYPE(__pyx_t_26)->tp_iternext;
         index = 0; __pyx_t_5 = __pyx_t_12(__pyx_t_26); if (unlikely(!__pyx_t_5)) goto __pyx_L32_unpacking_failed;
         __Pyx_GOTREF(__pyx_t_5);
         index = 1; __pyx_t_11 = __pyx_t_12(__pyx_t_26); if (unlikely(!__pyx_t_11)) goto __pyx_L32_unpacking_failed;
         __Pyx_GOTREF(__pyx_t_11);
-        if (__Pyx_IternextUnpackEndCheck(__pyx_t_12(__pyx_t_26), 2) < 0) __PYX_ERR(0, 371, __pyx_L27_error)
+        if (__Pyx_IternextUnpackEndCheck(__pyx_t_12(__pyx_t_26), 2) < 0) __PYX_ERR(0, 378, __pyx_L27_error)
         __pyx_t_12 = NULL;
         __Pyx_DECREF(__pyx_t_26); __pyx_t_26 = 0;
         goto __pyx_L33_unpacking_done;
         __pyx_L32_unpacking_failed:;
         __Pyx_DECREF(__pyx_t_26); __pyx_t_26 = 0;
         __pyx_t_12 = NULL;
         if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-        __PYX_ERR(0, 371, __pyx_L27_error)
+        __PYX_ERR(0, 378, __pyx_L27_error)
         __pyx_L33_unpacking_done:;
       }
       __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_i, __pyx_t_5);
       __pyx_t_5 = 0;
       __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_j, __pyx_t_11);
       __pyx_t_11 = 0;
       __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_l, __pyx_t_7);
       __pyx_t_7 = 0;
-      __pyx_t_4 = PyNumber_Subtract(__pyx_7genexpr__pyx_v_i, __pyx_7genexpr__pyx_v_l); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 371, __pyx_L27_error)
+      __pyx_t_4 = PyNumber_Subtract(__pyx_7genexpr__pyx_v_i, __pyx_7genexpr__pyx_v_l); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 378, __pyx_L27_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_7 = PyNumber_Subtract(__pyx_7genexpr__pyx_v_j, __pyx_7genexpr__pyx_v_l); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 371, __pyx_L27_error)
+      __pyx_t_7 = PyNumber_Subtract(__pyx_7genexpr__pyx_v_j, __pyx_7genexpr__pyx_v_l); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 378, __pyx_L27_error)
       __Pyx_GOTREF(__pyx_t_7);
-      __pyx_t_2 = PyTuple_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 371, __pyx_L27_error)
+      __pyx_t_2 = PyTuple_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 378, __pyx_L27_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_GIVEREF(__pyx_t_4);
       PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_4);
       __Pyx_GIVEREF(__pyx_t_7);
       PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_7);
       __Pyx_INCREF(__pyx_7genexpr__pyx_v_l);
       __Pyx_GIVEREF(__pyx_7genexpr__pyx_v_l);
       PyTuple_SET_ITEM(__pyx_t_2, 2, __pyx_7genexpr__pyx_v_l);
       __pyx_t_4 = 0;
       __pyx_t_7 = 0;
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_6, (PyObject*)__pyx_t_2))) __PYX_ERR(0, 371, __pyx_L27_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_6, (PyObject*)__pyx_t_2))) __PYX_ERR(0, 378, __pyx_L27_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __Pyx_XDECREF(__pyx_7genexpr__pyx_v_i); __pyx_7genexpr__pyx_v_i = 0;
     __Pyx_XDECREF(__pyx_7genexpr__pyx_v_j); __pyx_7genexpr__pyx_v_j = 0;
     __Pyx_XDECREF(__pyx_7genexpr__pyx_v_l); __pyx_7genexpr__pyx_v_l = 0;
     goto __pyx_L34_exit_scope;
     __pyx_L27_error:;
@@ -30355,33 +30496,33 @@
     __Pyx_XDECREF(__pyx_7genexpr__pyx_v_l); __pyx_7genexpr__pyx_v_l = 0;
     goto __pyx_L1_error;
     __pyx_L34_exit_scope:;
   } /* exit inner scope */
   __pyx_v_ans2 = ((PyObject*)__pyx_t_6);
   __pyx_t_6 = 0;
 
-  /* "pydivsufsort/stringalg.pyx":372
+  /* "pydivsufsort/stringalg.pyx":379
  * 
  *     ans2 = [(i - l, j - l, l) for (i, j), l in ans1]
  *     ans2.sort()             # <<<<<<<<<<<<<<
  *     return ans2
  */
-  __pyx_t_27 = PyList_Sort(__pyx_v_ans2); if (unlikely(__pyx_t_27 == ((int)-1))) __PYX_ERR(0, 372, __pyx_L1_error)
+  __pyx_t_27 = PyList_Sort(__pyx_v_ans2); if (unlikely(__pyx_t_27 == ((int)-1))) __PYX_ERR(0, 379, __pyx_L1_error)
 
-  /* "pydivsufsort/stringalg.pyx":373
+  /* "pydivsufsort/stringalg.pyx":380
  *     ans2 = [(i - l, j - l, l) for (i, j), l in ans1]
  *     ans2.sort()
  *     return ans2             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_ans2);
   __pyx_r = __pyx_v_ans2;
   goto __pyx_L0;
 
-  /* "pydivsufsort/stringalg.pyx":327
+  /* "pydivsufsort/stringalg.pyx":334
  * 
  * 
  * def _common_substrings(np.ndarray[ull, ndim=1] suffix_array, ull[::1] lcp, ull len1, ull limit):             # <<<<<<<<<<<<<<
  *     n = len(suffix_array)
  *     ranges = repeated_substrings(suffix_array, lcp)
  */
 
@@ -30423,15 +30564,15 @@
   __Pyx_XDECREF(__pyx_7genexpr__pyx_v_l);
   __PYX_XDEC_MEMVIEW(&__pyx_v_lcp, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":734
+/* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -30440,29 +30581,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -30473,15 +30614,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":737
+/* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -30490,29 +30631,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -30523,15 +30664,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":740
+/* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -30540,29 +30681,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -30573,15 +30714,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":743
+/* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -30590,29 +30731,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -30623,15 +30764,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":746
+/* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -30640,29 +30781,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -30673,212 +30814,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":749
+/* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":928
+/* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":932
+/* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":940
+/* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -30894,15 +31035,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -30910,53 +31051,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
@@ -30964,30 +31105,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -31002,15 +31143,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":946
+/* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -31026,15 +31167,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -31042,53 +31183,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
@@ -31096,30 +31237,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -31134,15 +31275,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":952
+/* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -31158,15 +31299,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -31174,53 +31315,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
@@ -31228,30 +31369,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -31266,176 +31407,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":966
+/* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":981
+/* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":996
+/* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -45655,15 +45796,15 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
-  {"repeated_substrings", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_12pydivsufsort_9stringalg_21repeated_substrings, METH_VARARGS|METH_KEYWORDS, __pyx_doc_12pydivsufsort_9stringalg_20repeated_substrings},
+  {"repeated_substrings", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_12pydivsufsort_9stringalg_23repeated_substrings, METH_VARARGS|METH_KEYWORDS, __pyx_doc_12pydivsufsort_9stringalg_22repeated_substrings},
   {0, 0, 0, 0}
 };
 
 #if PY_MAJOR_VERSION >= 3
 #if CYTHON_PEP489_MULTI_PHASE_INIT
 static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
 static int __pyx_pymod_exec_stringalg(PyObject* module); /*proto*/
@@ -45806,14 +45947,15 @@
   {&__pyx_n_s_key, __pyx_k_key, sizeof(__pyx_k_key), 0, 0, 1, 1},
   {&__pyx_n_s_kind, __pyx_k_kind, sizeof(__pyx_k_kind), 0, 0, 1, 1},
   {&__pyx_n_s_kwargs, __pyx_k_kwargs, sizeof(__pyx_k_kwargs), 0, 0, 1, 1},
   {&__pyx_n_s_l, __pyx_k_l, sizeof(__pyx_k_l), 0, 0, 1, 1},
   {&__pyx_n_s_last, __pyx_k_last, sizeof(__pyx_k_last), 0, 0, 1, 1},
   {&__pyx_n_s_lcp, __pyx_k_lcp, sizeof(__pyx_k_lcp), 0, 0, 1, 1},
   {&__pyx_n_s_lcp_query, __pyx_k_lcp_query, sizeof(__pyx_k_lcp_query), 0, 0, 1, 1},
+  {&__pyx_n_s_lcp_query_2, __pyx_k_lcp_query_2, sizeof(__pyx_k_lcp_query_2), 0, 0, 1, 1},
   {&__pyx_n_s_lcp_segtree, __pyx_k_lcp_segtree, sizeof(__pyx_k_lcp_segtree), 0, 0, 1, 1},
   {&__pyx_n_s_lcp_segtree_2, __pyx_k_lcp_segtree_2, sizeof(__pyx_k_lcp_segtree_2), 0, 0, 1, 1},
   {&__pyx_n_s_len1, __pyx_k_len1, sizeof(__pyx_k_len1), 0, 0, 1, 1},
   {&__pyx_n_s_length, __pyx_k_length, sizeof(__pyx_k_length), 0, 0, 1, 1},
   {&__pyx_n_s_levenshtein, __pyx_k_levenshtein, sizeof(__pyx_k_levenshtein), 0, 0, 1, 1},
   {&__pyx_n_s_levenshtein_2, __pyx_k_levenshtein_2, sizeof(__pyx_k_levenshtein_2), 0, 0, 1, 1},
   {&__pyx_n_s_limit, __pyx_k_limit, sizeof(__pyx_k_limit), 0, 0, 1, 1},
@@ -45946,37 +46088,37 @@
   __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_No_matching_signature_found); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
   __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_s_Function_call_with_ambiguous_arg); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
-  /* "pydivsufsort/stringalg.pyx":335
+  /* "pydivsufsort/stringalg.pyx":342
  *     cdef np.ndarray[ull, ndim=1] origin_cumsum = np.empty(n + 1, dtype=np.uint64)
  *     origin_cumsum[0] = 0
  *     origin_cumsum[1:] = np.cumsum(origin)             # <<<<<<<<<<<<<<
  * 
  *     cdef cpp_map[pair[ull, ull], ull] ans
  */
-  __pyx_slice__8 = PySlice_New(__pyx_int_1, Py_None, Py_None); if (unlikely(!__pyx_slice__8)) __PYX_ERR(0, 335, __pyx_L1_error)
+  __pyx_slice__8 = PySlice_New(__pyx_int_1, Py_None, Py_None); if (unlikely(!__pyx_slice__8)) __PYX_ERR(0, 342, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_slice__8);
   __Pyx_GIVEREF(__pyx_slice__8);
 
-  /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(1, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../../../tmp/build-env-_aqb9ylv/lib/python3.11/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../tmp/build-env-72gmrv88/lib/python3.11/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(1, 950, __pyx_L1_error)
@@ -46249,135 +46391,147 @@
   __Pyx_GOTREF(__pyx_tuple__40);
   __Pyx_GIVEREF(__pyx_tuple__40);
   __pyx_codeobj__41 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__40, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pydivsufsort_stringalg_pyx, __pyx_n_s_lcp_segtree_2, 132, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__41)) __PYX_ERR(0, 132, __pyx_L1_error)
 
   /* "pydivsufsort/stringalg.pyx":144
  * 
  * 
- * def lcp_query(             # <<<<<<<<<<<<<<
+ * def _lcp_query(             # <<<<<<<<<<<<<<
  *         np.ndarray[sa_t, ndim=1] rank not None,
  *         np.ndarray[sa_t, ndim=1] segtree not None,
  */
   __pyx_tuple__42 = PyTuple_Pack(10, __pyx_n_s_rank, __pyx_n_s_segtree, __pyx_n_s_queries, __pyx_n_s_n, __pyx_n_s_q, __pyx_n_s_i, __pyx_n_s_l, __pyx_n_s_r, __pyx_n_s_ans, __pyx_n_s_res); if (unlikely(!__pyx_tuple__42)) __PYX_ERR(0, 144, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__42);
   __Pyx_GIVEREF(__pyx_tuple__42);
   __pyx_codeobj__43 = (PyObject*)__Pyx_PyCode_New(3, 0, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__42, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pydivsufsort_stringalg_pyx, __pyx_n_s_lcp_query, 144, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__43)) __PYX_ERR(0, 144, __pyx_L1_error)
 
   /* "pydivsufsort/stringalg.pyx":184
  *     return ans
  * 
+ * def lcp_query(segtree, queries):             # <<<<<<<<<<<<<<
+ *     return _lcp_query(*segtree, queries)
+ * 
+ */
+  __pyx_tuple__44 = PyTuple_Pack(2, __pyx_n_s_segtree, __pyx_n_s_queries); if (unlikely(!__pyx_tuple__44)) __PYX_ERR(0, 184, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__44);
+  __Pyx_GIVEREF(__pyx_tuple__44);
+  __pyx_codeobj__45 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__44, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pydivsufsort_stringalg_pyx, __pyx_n_s_lcp_query_2, 184, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__45)) __PYX_ERR(0, 184, __pyx_L1_error)
+
+  /* "pydivsufsort/stringalg.pyx":187
+ *     return _lcp_query(*segtree, queries)
+ * 
  * def _levenshtein(string_t[::1] a not None, string_t[::1] b not None):             # <<<<<<<<<<<<<<
  *     cdef unsigned long long n, m, i, j, d
  *     n = len(a)
  */
-  __pyx_tuple__44 = PyTuple_Pack(8, __pyx_n_s_a, __pyx_n_s_b, __pyx_n_s_n, __pyx_n_s_m, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_d, __pyx_n_s_temp); if (unlikely(!__pyx_tuple__44)) __PYX_ERR(0, 184, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__44);
-  __Pyx_GIVEREF(__pyx_tuple__44);
-  __pyx_codeobj__45 = (PyObject*)__Pyx_PyCode_New(2, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__44, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pydivsufsort_stringalg_pyx, __pyx_n_s_levenshtein, 184, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__45)) __PYX_ERR(0, 184, __pyx_L1_error)
+  __pyx_tuple__46 = PyTuple_Pack(8, __pyx_n_s_a, __pyx_n_s_b, __pyx_n_s_n, __pyx_n_s_m, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_d, __pyx_n_s_temp); if (unlikely(!__pyx_tuple__46)) __PYX_ERR(0, 187, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__46);
+  __Pyx_GIVEREF(__pyx_tuple__46);
+  __pyx_codeobj__47 = (PyObject*)__Pyx_PyCode_New(2, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__46, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pydivsufsort_stringalg_pyx, __pyx_n_s_levenshtein, 187, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__47)) __PYX_ERR(0, 187, __pyx_L1_error)
 
-  /* "pydivsufsort/stringalg.pyx":199
+  /* "pydivsufsort/stringalg.pyx":202
  * 
  * 
  * def levenshtein(a, b):             # <<<<<<<<<<<<<<
  *     a = handle_input(a)
  *     b = handle_input(b)
  */
-  __pyx_tuple__46 = PyTuple_Pack(2, __pyx_n_s_a, __pyx_n_s_b); if (unlikely(!__pyx_tuple__46)) __PYX_ERR(0, 199, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__46);
-  __Pyx_GIVEREF(__pyx_tuple__46);
-  __pyx_codeobj__47 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__46, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pydivsufsort_stringalg_pyx, __pyx_n_s_levenshtein_2, 199, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__47)) __PYX_ERR(0, 199, __pyx_L1_error)
+  __pyx_tuple__48 = PyTuple_Pack(2, __pyx_n_s_a, __pyx_n_s_b); if (unlikely(!__pyx_tuple__48)) __PYX_ERR(0, 202, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__48);
+  __Pyx_GIVEREF(__pyx_tuple__48);
+  __pyx_codeobj__49 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__48, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pydivsufsort_stringalg_pyx, __pyx_n_s_levenshtein_2, 202, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__49)) __PYX_ERR(0, 202, __pyx_L1_error)
 
-  /* "pydivsufsort/stringalg.pyx":220
+  /* "pydivsufsort/stringalg.pyx":223
  * 
  * 
  * def most_frequent_substrings(             # <<<<<<<<<<<<<<
  *     np.ndarray[sa_t, ndim=1] lcp not None,
  *     sa_t length,
  */
-  __pyx_tuple__48 = PyTuple_Pack(12, __pyx_n_s_lcp, __pyx_n_s_length, __pyx_n_s_limit, __pyx_n_s_minimum_count, __pyx_n_s_n, __pyx_n_s_i, __pyx_n_s_cur, __pyx_n_s_cur_count, __pyx_n_s_last, __pyx_n_s_count, __pyx_n_s_pos, __pyx_n_s_cnt); if (unlikely(!__pyx_tuple__48)) __PYX_ERR(0, 220, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__48);
-  __Pyx_GIVEREF(__pyx_tuple__48);
-  __pyx_codeobj__49 = (PyObject*)__Pyx_PyCode_New(4, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__48, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pydivsufsort_stringalg_pyx, __pyx_n_s_most_frequent_substrings, 220, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__49)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_tuple__50 = PyTuple_Pack(12, __pyx_n_s_lcp, __pyx_n_s_length, __pyx_n_s_limit, __pyx_n_s_minimum_count, __pyx_n_s_n, __pyx_n_s_i, __pyx_n_s_cur, __pyx_n_s_cur_count, __pyx_n_s_last, __pyx_n_s_count, __pyx_n_s_pos, __pyx_n_s_cnt); if (unlikely(!__pyx_tuple__50)) __PYX_ERR(0, 223, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__50);
+  __Pyx_GIVEREF(__pyx_tuple__50);
+  __pyx_codeobj__51 = (PyObject*)__Pyx_PyCode_New(4, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__50, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pydivsufsort_stringalg_pyx, __pyx_n_s_most_frequent_substrings, 223, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__51)) __PYX_ERR(0, 223, __pyx_L1_error)
 
-  /* "pydivsufsort/stringalg.pyx":327
+  /* "pydivsufsort/stringalg.pyx":334
  * 
  * 
  * def _common_substrings(np.ndarray[ull, ndim=1] suffix_array, ull[::1] lcp, ull len1, ull limit):             # <<<<<<<<<<<<<<
  *     n = len(suffix_array)
  *     ranges = repeated_substrings(suffix_array, lcp)
  */
-  __pyx_tuple__50 = PyTuple_Pack(24, __pyx_n_s_suffix_array, __pyx_n_s_lcp, __pyx_n_s_len1, __pyx_n_s_limit, __pyx_n_s_n, __pyx_n_s_ranges, __pyx_n_s_origin, __pyx_n_s_origin_cumsum, __pyx_n_s_ans, __pyx_n_s_start1, __pyx_n_s_start2, __pyx_n_s_start, __pyx_n_s_end, __pyx_n_s_length, __pyx_n_s_diff, __pyx_n_s_i, __pyx_n_s_pos, __pyx_n_s_j, __pyx_n_s_ans1, __pyx_n_s_l, __pyx_n_s_ans2, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_l); if (unlikely(!__pyx_tuple__50)) __PYX_ERR(0, 327, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__50);
-  __Pyx_GIVEREF(__pyx_tuple__50);
-  __pyx_codeobj__51 = (PyObject*)__Pyx_PyCode_New(4, 0, 24, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__50, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pydivsufsort_stringalg_pyx, __pyx_n_s_common_substrings, 327, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__51)) __PYX_ERR(0, 327, __pyx_L1_error)
+  __pyx_tuple__52 = PyTuple_Pack(24, __pyx_n_s_suffix_array, __pyx_n_s_lcp, __pyx_n_s_len1, __pyx_n_s_limit, __pyx_n_s_n, __pyx_n_s_ranges, __pyx_n_s_origin, __pyx_n_s_origin_cumsum, __pyx_n_s_ans, __pyx_n_s_start1, __pyx_n_s_start2, __pyx_n_s_start, __pyx_n_s_end, __pyx_n_s_length, __pyx_n_s_diff, __pyx_n_s_i, __pyx_n_s_pos, __pyx_n_s_j, __pyx_n_s_ans1, __pyx_n_s_l, __pyx_n_s_ans2, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_l); if (unlikely(!__pyx_tuple__52)) __PYX_ERR(0, 334, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__52);
+  __Pyx_GIVEREF(__pyx_tuple__52);
+  __pyx_codeobj__53 = (PyObject*)__Pyx_PyCode_New(4, 0, 24, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__52, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pydivsufsort_stringalg_pyx, __pyx_n_s_common_substrings, 334, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__53)) __PYX_ERR(0, 334, __pyx_L1_error)
 
   /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
  */
-  __pyx_tuple__52 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct_or_indirect); if (unlikely(!__pyx_tuple__52)) __PYX_ERR(2, 287, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__52);
-  __Pyx_GIVEREF(__pyx_tuple__52);
+  __pyx_tuple__54 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct_or_indirect); if (unlikely(!__pyx_tuple__54)) __PYX_ERR(2, 287, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__54);
+  __Pyx_GIVEREF(__pyx_tuple__54);
 
   /* "View.MemoryView":288
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default             # <<<<<<<<<<<<<<
  * cdef indirect = Enum("<strided and indirect>")
  * 
  */
-  __pyx_tuple__53 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct); if (unlikely(!__pyx_tuple__53)) __PYX_ERR(2, 288, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__53);
-  __Pyx_GIVEREF(__pyx_tuple__53);
+  __pyx_tuple__55 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct); if (unlikely(!__pyx_tuple__55)) __PYX_ERR(2, 288, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__55);
+  __Pyx_GIVEREF(__pyx_tuple__55);
 
   /* "View.MemoryView":289
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__54 = PyTuple_Pack(1, __pyx_kp_s_strided_and_indirect); if (unlikely(!__pyx_tuple__54)) __PYX_ERR(2, 289, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__54);
-  __Pyx_GIVEREF(__pyx_tuple__54);
+  __pyx_tuple__56 = PyTuple_Pack(1, __pyx_kp_s_strided_and_indirect); if (unlikely(!__pyx_tuple__56)) __PYX_ERR(2, 289, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__56);
+  __Pyx_GIVEREF(__pyx_tuple__56);
 
   /* "View.MemoryView":292
  * 
  * 
  * cdef contiguous = Enum("<contiguous and direct>")             # <<<<<<<<<<<<<<
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")
  * 
  */
-  __pyx_tuple__55 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_direct); if (unlikely(!__pyx_tuple__55)) __PYX_ERR(2, 292, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__55);
-  __Pyx_GIVEREF(__pyx_tuple__55);
+  __pyx_tuple__57 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_direct); if (unlikely(!__pyx_tuple__57)) __PYX_ERR(2, 292, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__57);
+  __Pyx_GIVEREF(__pyx_tuple__57);
 
   /* "View.MemoryView":293
  * 
  * cdef contiguous = Enum("<contiguous and direct>")
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__56 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_indirect); if (unlikely(!__pyx_tuple__56)) __PYX_ERR(2, 293, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__56);
-  __Pyx_GIVEREF(__pyx_tuple__56);
+  __pyx_tuple__58 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_indirect); if (unlikely(!__pyx_tuple__58)) __PYX_ERR(2, 293, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__58);
+  __Pyx_GIVEREF(__pyx_tuple__58);
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_Enum(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_tuple__57 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__57)) __PYX_ERR(2, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__57);
-  __Pyx_GIVEREF(__pyx_tuple__57);
-  __pyx_codeobj__58 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__57, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__58)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __pyx_tuple__59 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__59)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__59);
+  __Pyx_GIVEREF(__pyx_tuple__59);
+  __pyx_codeobj__60 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__59, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__60)) __PYX_ERR(2, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -46854,90 +47008,90 @@
  * 
  * def _kasai(string_t[::1] s not None, sa_t[::1] sa not None):             # <<<<<<<<<<<<<<
  * 
  *     cdef sa_t i, j, n, k
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(16); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_0_0__pyx_mdef_12pydivsufsort_9stringalg_25_kasai, 0, __pyx_n_s_kasai, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_0_0__pyx_mdef_12pydivsufsort_9stringalg_27_kasai, 0, __pyx_n_s_kasai, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_empty_tuple);
   if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_uint8_t_int32_t, __pyx_t_1) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_0_1__pyx_mdef_12pydivsufsort_9stringalg_27_kasai, 0, __pyx_n_s_kasai, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_0_1__pyx_mdef_12pydivsufsort_9stringalg_29_kasai, 0, __pyx_n_s_kasai, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_empty_tuple);
   if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_uint8_t_int64_t, __pyx_t_1) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_1_0__pyx_mdef_12pydivsufsort_9stringalg_29_kasai, 0, __pyx_n_s_kasai, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_1_0__pyx_mdef_12pydivsufsort_9stringalg_31_kasai, 0, __pyx_n_s_kasai, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_empty_tuple);
   if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_uint16_t_int32_t, __pyx_t_1) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_1_1__pyx_mdef_12pydivsufsort_9stringalg_31_kasai, 0, __pyx_n_s_kasai, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_1_1__pyx_mdef_12pydivsufsort_9stringalg_33_kasai, 0, __pyx_n_s_kasai, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_empty_tuple);
   if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_uint16_t_int64_t, __pyx_t_1) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_2_0__pyx_mdef_12pydivsufsort_9stringalg_33_kasai, 0, __pyx_n_s_kasai, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_2_0__pyx_mdef_12pydivsufsort_9stringalg_35_kasai, 0, __pyx_n_s_kasai, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_empty_tuple);
   if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_uint32_t_int32_t, __pyx_t_1) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_2_1__pyx_mdef_12pydivsufsort_9stringalg_35_kasai, 0, __pyx_n_s_kasai, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_2_1__pyx_mdef_12pydivsufsort_9stringalg_37_kasai, 0, __pyx_n_s_kasai, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_empty_tuple);
   if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_uint32_t_int64_t, __pyx_t_1) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_3_0__pyx_mdef_12pydivsufsort_9stringalg_37_kasai, 0, __pyx_n_s_kasai, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_3_0__pyx_mdef_12pydivsufsort_9stringalg_39_kasai, 0, __pyx_n_s_kasai, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_empty_tuple);
   if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_uint64_t_int32_t, __pyx_t_1) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_3_1__pyx_mdef_12pydivsufsort_9stringalg_39_kasai, 0, __pyx_n_s_kasai, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_3_1__pyx_mdef_12pydivsufsort_9stringalg_41_kasai, 0, __pyx_n_s_kasai, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_empty_tuple);
   if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_uint64_t_int64_t, __pyx_t_1) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_4_0__pyx_mdef_12pydivsufsort_9stringalg_41_kasai, 0, __pyx_n_s_kasai, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_4_0__pyx_mdef_12pydivsufsort_9stringalg_43_kasai, 0, __pyx_n_s_kasai, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_empty_tuple);
   if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_int8_t_int32_t, __pyx_t_1) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_4_1__pyx_mdef_12pydivsufsort_9stringalg_43_kasai, 0, __pyx_n_s_kasai, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_4_1__pyx_mdef_12pydivsufsort_9stringalg_45_kasai, 0, __pyx_n_s_kasai, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_empty_tuple);
   if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_int8_t_int64_t, __pyx_t_1) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_5_0__pyx_mdef_12pydivsufsort_9stringalg_45_kasai, 0, __pyx_n_s_kasai, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_5_0__pyx_mdef_12pydivsufsort_9stringalg_47_kasai, 0, __pyx_n_s_kasai, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_empty_tuple);
   if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_int16_t_int32_t, __pyx_t_1) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_5_1__pyx_mdef_12pydivsufsort_9stringalg_47_kasai, 0, __pyx_n_s_kasai, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_5_1__pyx_mdef_12pydivsufsort_9stringalg_49_kasai, 0, __pyx_n_s_kasai, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_empty_tuple);
   if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_int16_t_int64_t, __pyx_t_1) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_6_0__pyx_mdef_12pydivsufsort_9stringalg_49_kasai, 0, __pyx_n_s_kasai, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_6_0__pyx_mdef_12pydivsufsort_9stringalg_51_kasai, 0, __pyx_n_s_kasai, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_empty_tuple);
   if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_int32_t_int32_t, __pyx_t_1) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_6_1__pyx_mdef_12pydivsufsort_9stringalg_51_kasai, 0, __pyx_n_s_kasai, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_6_1__pyx_mdef_12pydivsufsort_9stringalg_53_kasai, 0, __pyx_n_s_kasai, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_empty_tuple);
   if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_int32_t_int64_t, __pyx_t_1) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_7_0__pyx_mdef_12pydivsufsort_9stringalg_53_kasai, 0, __pyx_n_s_kasai, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_7_0__pyx_mdef_12pydivsufsort_9stringalg_55_kasai, 0, __pyx_n_s_kasai, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_empty_tuple);
   if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_int64_t_int32_t, __pyx_t_1) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_7_1__pyx_mdef_12pydivsufsort_9stringalg_55_kasai, 0, __pyx_n_s_kasai, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_7_1__pyx_mdef_12pydivsufsort_9stringalg_57_kasai, 0, __pyx_n_s_kasai, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_empty_tuple);
   if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_int64_t_int64_t, __pyx_t_1) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_mdef_12pydivsufsort_9stringalg_3_kasai, 0, __pyx_n_s_kasai, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_empty_tuple);
@@ -46952,20 +47106,20 @@
  * 
  * def _kasai_bytes(const unsigned char[::1] s not None, sa_t[::1] sa not None):             # <<<<<<<<<<<<<<
  *     """Same as _kasai but with a const first argument.
  * 
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_fuse_0__pyx_mdef_12pydivsufsort_9stringalg_59_kasai_bytes, 0, __pyx_n_s_kasai_bytes, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__35)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 72, __pyx_L1_error)
+  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_fuse_0__pyx_mdef_12pydivsufsort_9stringalg_61_kasai_bytes, 0, __pyx_n_s_kasai_bytes, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__35)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_empty_tuple);
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_int32_t, __pyx_t_2) < 0) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_fuse_1__pyx_mdef_12pydivsufsort_9stringalg_61_kasai_bytes, 0, __pyx_n_s_kasai_bytes, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__35)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 72, __pyx_L1_error)
+  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_fuse_1__pyx_mdef_12pydivsufsort_9stringalg_63_kasai_bytes, 0, __pyx_n_s_kasai_bytes, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__35)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_empty_tuple);
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_int64_t, __pyx_t_2) < 0) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_mdef_12pydivsufsort_9stringalg_5_kasai_bytes, 0, __pyx_n_s_kasai_bytes, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__35)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_empty_tuple);
@@ -46992,90 +47146,90 @@
  * 
  * def _lcp_segtree(             # <<<<<<<<<<<<<<
  *         string_t[::1] s not None,
  *         np.ndarray[sa_t, ndim=1] sa not None,
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(16); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_0_0__pyx_mdef_12pydivsufsort_9stringalg_65_lcp_segtree, 0, __pyx_n_s_lcp_segtree, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__39)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_0_0__pyx_mdef_12pydivsufsort_9stringalg_67_lcp_segtree, 0, __pyx_n_s_lcp_segtree, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__39)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_empty_tuple);
   if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_uint8_t_int32_t, __pyx_t_1) < 0) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_0_1__pyx_mdef_12pydivsufsort_9stringalg_67_lcp_segtree, 0, __pyx_n_s_lcp_segtree, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__39)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_0_1__pyx_mdef_12pydivsufsort_9stringalg_69_lcp_segtree, 0, __pyx_n_s_lcp_segtree, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__39)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_empty_tuple);
   if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_uint8_t_int64_t, __pyx_t_1) < 0) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_1_0__pyx_mdef_12pydivsufsort_9stringalg_69_lcp_segtree, 0, __pyx_n_s_lcp_segtree, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__39)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_1_0__pyx_mdef_12pydivsufsort_9stringalg_71_lcp_segtree, 0, __pyx_n_s_lcp_segtree, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__39)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_empty_tuple);
   if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_uint16_t_int32_t, __pyx_t_1) < 0) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_1_1__pyx_mdef_12pydivsufsort_9stringalg_71_lcp_segtree, 0, __pyx_n_s_lcp_segtree, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__39)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_1_1__pyx_mdef_12pydivsufsort_9stringalg_73_lcp_segtree, 0, __pyx_n_s_lcp_segtree, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__39)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_empty_tuple);
   if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_uint16_t_int64_t, __pyx_t_1) < 0) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_2_0__pyx_mdef_12pydivsufsort_9stringalg_73_lcp_segtree, 0, __pyx_n_s_lcp_segtree, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__39)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_2_0__pyx_mdef_12pydivsufsort_9stringalg_75_lcp_segtree, 0, __pyx_n_s_lcp_segtree, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__39)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_empty_tuple);
   if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_uint32_t_int32_t, __pyx_t_1) < 0) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_2_1__pyx_mdef_12pydivsufsort_9stringalg_75_lcp_segtree, 0, __pyx_n_s_lcp_segtree, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__39)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_2_1__pyx_mdef_12pydivsufsort_9stringalg_77_lcp_segtree, 0, __pyx_n_s_lcp_segtree, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__39)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_empty_tuple);
   if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_uint32_t_int64_t, __pyx_t_1) < 0) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_3_0__pyx_mdef_12pydivsufsort_9stringalg_77_lcp_segtree, 0, __pyx_n_s_lcp_segtree, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__39)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_3_0__pyx_mdef_12pydivsufsort_9stringalg_79_lcp_segtree, 0, __pyx_n_s_lcp_segtree, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__39)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_empty_tuple);
   if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_uint64_t_int32_t, __pyx_t_1) < 0) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_3_1__pyx_mdef_12pydivsufsort_9stringalg_79_lcp_segtree, 0, __pyx_n_s_lcp_segtree, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__39)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_3_1__pyx_mdef_12pydivsufsort_9stringalg_81_lcp_segtree, 0, __pyx_n_s_lcp_segtree, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__39)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_empty_tuple);
   if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_uint64_t_int64_t, __pyx_t_1) < 0) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_4_0__pyx_mdef_12pydivsufsort_9stringalg_81_lcp_segtree, 0, __pyx_n_s_lcp_segtree, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__39)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_4_0__pyx_mdef_12pydivsufsort_9stringalg_83_lcp_segtree, 0, __pyx_n_s_lcp_segtree, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__39)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_empty_tuple);
   if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_int8_t_int32_t, __pyx_t_1) < 0) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_4_1__pyx_mdef_12pydivsufsort_9stringalg_83_lcp_segtree, 0, __pyx_n_s_lcp_segtree, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__39)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_4_1__pyx_mdef_12pydivsufsort_9stringalg_85_lcp_segtree, 0, __pyx_n_s_lcp_segtree, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__39)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_empty_tuple);
   if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_int8_t_int64_t, __pyx_t_1) < 0) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_5_0__pyx_mdef_12pydivsufsort_9stringalg_85_lcp_segtree, 0, __pyx_n_s_lcp_segtree, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__39)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_5_0__pyx_mdef_12pydivsufsort_9stringalg_87_lcp_segtree, 0, __pyx_n_s_lcp_segtree, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__39)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_empty_tuple);
   if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_int16_t_int32_t, __pyx_t_1) < 0) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_5_1__pyx_mdef_12pydivsufsort_9stringalg_87_lcp_segtree, 0, __pyx_n_s_lcp_segtree, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__39)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_5_1__pyx_mdef_12pydivsufsort_9stringalg_89_lcp_segtree, 0, __pyx_n_s_lcp_segtree, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__39)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_empty_tuple);
   if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_int16_t_int64_t, __pyx_t_1) < 0) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_6_0__pyx_mdef_12pydivsufsort_9stringalg_89_lcp_segtree, 0, __pyx_n_s_lcp_segtree, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__39)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_6_0__pyx_mdef_12pydivsufsort_9stringalg_91_lcp_segtree, 0, __pyx_n_s_lcp_segtree, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__39)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_empty_tuple);
   if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_int32_t_int32_t, __pyx_t_1) < 0) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_6_1__pyx_mdef_12pydivsufsort_9stringalg_91_lcp_segtree, 0, __pyx_n_s_lcp_segtree, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__39)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_6_1__pyx_mdef_12pydivsufsort_9stringalg_93_lcp_segtree, 0, __pyx_n_s_lcp_segtree, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__39)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_empty_tuple);
   if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_int32_t_int64_t, __pyx_t_1) < 0) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_7_0__pyx_mdef_12pydivsufsort_9stringalg_93_lcp_segtree, 0, __pyx_n_s_lcp_segtree, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__39)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_7_0__pyx_mdef_12pydivsufsort_9stringalg_95_lcp_segtree, 0, __pyx_n_s_lcp_segtree, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__39)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_empty_tuple);
   if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_int64_t_int32_t, __pyx_t_1) < 0) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_7_1__pyx_mdef_12pydivsufsort_9stringalg_95_lcp_segtree, 0, __pyx_n_s_lcp_segtree, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__39)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_7_1__pyx_mdef_12pydivsufsort_9stringalg_97_lcp_segtree, 0, __pyx_n_s_lcp_segtree, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__39)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_empty_tuple);
   if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_int64_t_int64_t, __pyx_t_1) < 0) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_mdef_12pydivsufsort_9stringalg_9_lcp_segtree, 0, __pyx_n_s_lcp_segtree, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__39)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_empty_tuple);
@@ -47096,218 +47250,230 @@
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_lcp_segtree_2, __pyx_t_1) < 0) __PYX_ERR(0, 132, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "pydivsufsort/stringalg.pyx":144
  * 
  * 
- * def lcp_query(             # <<<<<<<<<<<<<<
+ * def _lcp_query(             # <<<<<<<<<<<<<<
  *         np.ndarray[sa_t, ndim=1] rank not None,
  *         np.ndarray[sa_t, ndim=1] segtree not None,
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 144, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_fuse_0__pyx_mdef_12pydivsufsort_9stringalg_99lcp_query, 0, __pyx_n_s_lcp_query, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__43)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 144, __pyx_L1_error)
+  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_fuse_0__pyx_mdef_12pydivsufsort_9stringalg_101_lcp_query, 0, __pyx_n_s_lcp_query, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__43)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 144, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_empty_tuple);
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_int32_t, __pyx_t_2) < 0) __PYX_ERR(0, 144, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_fuse_1__pyx_mdef_12pydivsufsort_9stringalg_101lcp_query, 0, __pyx_n_s_lcp_query, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__43)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 144, __pyx_L1_error)
+  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_fuse_1__pyx_mdef_12pydivsufsort_9stringalg_103_lcp_query, 0, __pyx_n_s_lcp_query, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__43)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 144, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_empty_tuple);
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_int64_t, __pyx_t_2) < 0) __PYX_ERR(0, 144, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_mdef_12pydivsufsort_9stringalg_13lcp_query, 0, __pyx_n_s_lcp_query, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__43)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 144, __pyx_L1_error)
+  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_mdef_12pydivsufsort_9stringalg_13_lcp_query, 0, __pyx_n_s_lcp_query, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__43)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 144, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_empty_tuple);
   ((__pyx_FusedFunctionObject *) __pyx_t_2)->__signatures__ = __pyx_t_1;
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_lcp_query, __pyx_t_2) < 0) __PYX_ERR(0, 144, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pydivsufsort/stringalg.pyx":184
  *     return ans
  * 
+ * def lcp_query(segtree, queries):             # <<<<<<<<<<<<<<
+ *     return _lcp_query(*segtree, queries)
+ * 
+ */
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_12pydivsufsort_9stringalg_15lcp_query, NULL, __pyx_n_s_pydivsufsort_stringalg); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 184, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_lcp_query_2, __pyx_t_2) < 0) __PYX_ERR(0, 184, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  /* "pydivsufsort/stringalg.pyx":187
+ *     return _lcp_query(*segtree, queries)
+ * 
  * def _levenshtein(string_t[::1] a not None, string_t[::1] b not None):             # <<<<<<<<<<<<<<
  *     cdef unsigned long long n, m, i, j, d
  *     n = len(a)
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 184, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_0__pyx_mdef_12pydivsufsort_9stringalg_105_levenshtein, 0, __pyx_n_s_levenshtein, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__45)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 184, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_0__pyx_mdef_12pydivsufsort_9stringalg_107_levenshtein, 0, __pyx_n_s_levenshtein, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__47)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_empty_tuple);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_uint8_t, __pyx_t_1) < 0) __PYX_ERR(0, 184, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_uint8_t, __pyx_t_1) < 0) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_1__pyx_mdef_12pydivsufsort_9stringalg_107_levenshtein, 0, __pyx_n_s_levenshtein, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__45)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 184, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_1__pyx_mdef_12pydivsufsort_9stringalg_109_levenshtein, 0, __pyx_n_s_levenshtein, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__47)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_empty_tuple);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_uint16_t, __pyx_t_1) < 0) __PYX_ERR(0, 184, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_uint16_t, __pyx_t_1) < 0) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_2__pyx_mdef_12pydivsufsort_9stringalg_109_levenshtein, 0, __pyx_n_s_levenshtein, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__45)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 184, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_2__pyx_mdef_12pydivsufsort_9stringalg_111_levenshtein, 0, __pyx_n_s_levenshtein, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__47)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_empty_tuple);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_uint32_t, __pyx_t_1) < 0) __PYX_ERR(0, 184, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_uint32_t, __pyx_t_1) < 0) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_3__pyx_mdef_12pydivsufsort_9stringalg_111_levenshtein, 0, __pyx_n_s_levenshtein, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__45)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 184, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_3__pyx_mdef_12pydivsufsort_9stringalg_113_levenshtein, 0, __pyx_n_s_levenshtein, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__47)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_empty_tuple);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_uint64_t, __pyx_t_1) < 0) __PYX_ERR(0, 184, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_uint64_t, __pyx_t_1) < 0) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_4__pyx_mdef_12pydivsufsort_9stringalg_113_levenshtein, 0, __pyx_n_s_levenshtein, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__45)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 184, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_4__pyx_mdef_12pydivsufsort_9stringalg_115_levenshtein, 0, __pyx_n_s_levenshtein, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__47)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_empty_tuple);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_int8_t, __pyx_t_1) < 0) __PYX_ERR(0, 184, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_int8_t, __pyx_t_1) < 0) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_5__pyx_mdef_12pydivsufsort_9stringalg_115_levenshtein, 0, __pyx_n_s_levenshtein, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__45)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 184, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_5__pyx_mdef_12pydivsufsort_9stringalg_117_levenshtein, 0, __pyx_n_s_levenshtein, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__47)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_empty_tuple);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_int16_t, __pyx_t_1) < 0) __PYX_ERR(0, 184, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_int16_t, __pyx_t_1) < 0) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_6__pyx_mdef_12pydivsufsort_9stringalg_117_levenshtein, 0, __pyx_n_s_levenshtein, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__45)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 184, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_6__pyx_mdef_12pydivsufsort_9stringalg_119_levenshtein, 0, __pyx_n_s_levenshtein, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__47)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_empty_tuple);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_int32_t, __pyx_t_1) < 0) __PYX_ERR(0, 184, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_int32_t, __pyx_t_1) < 0) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_7__pyx_mdef_12pydivsufsort_9stringalg_119_levenshtein, 0, __pyx_n_s_levenshtein, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__45)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 184, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_7__pyx_mdef_12pydivsufsort_9stringalg_121_levenshtein, 0, __pyx_n_s_levenshtein, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__47)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_empty_tuple);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_int64_t, __pyx_t_1) < 0) __PYX_ERR(0, 184, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_int64_t, __pyx_t_1) < 0) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_mdef_12pydivsufsort_9stringalg_15_levenshtein, 0, __pyx_n_s_levenshtein, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__45)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 184, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_mdef_12pydivsufsort_9stringalg_17_levenshtein, 0, __pyx_n_s_levenshtein, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__47)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_empty_tuple);
   ((__pyx_FusedFunctionObject *) __pyx_t_1)->__signatures__ = __pyx_t_2;
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_levenshtein, __pyx_t_1) < 0) __PYX_ERR(0, 184, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_levenshtein, __pyx_t_1) < 0) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pydivsufsort/stringalg.pyx":199
+  /* "pydivsufsort/stringalg.pyx":202
  * 
  * 
  * def levenshtein(a, b):             # <<<<<<<<<<<<<<
  *     a = handle_input(a)
  *     b = handle_input(b)
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_12pydivsufsort_9stringalg_17levenshtein, NULL, __pyx_n_s_pydivsufsort_stringalg); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 199, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_12pydivsufsort_9stringalg_19levenshtein, NULL, __pyx_n_s_pydivsufsort_stringalg); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_levenshtein_2, __pyx_t_1) < 0) __PYX_ERR(0, 199, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_levenshtein_2, __pyx_t_1) < 0) __PYX_ERR(0, 202, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pydivsufsort/stringalg.pyx":223
+  /* "pydivsufsort/stringalg.pyx":226
  *     np.ndarray[sa_t, ndim=1] lcp not None,
  *     sa_t length,
  *     sa_t limit = 0,             # <<<<<<<<<<<<<<
  *     sa_t minimum_count = 1
  *     ):
  */
-  __pyx_t_1 = __Pyx_PyInt_From_long(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 223, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_long(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 226, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "pydivsufsort/stringalg.pyx":224
+  /* "pydivsufsort/stringalg.pyx":227
  *     sa_t length,
  *     sa_t limit = 0,
  *     sa_t minimum_count = 1             # <<<<<<<<<<<<<<
  *     ):
  *     """
  */
-  __pyx_t_2 = __Pyx_PyInt_From_long(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 224, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_long(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 227, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  /* "pydivsufsort/stringalg.pyx":220
+  /* "pydivsufsort/stringalg.pyx":223
  * 
  * 
  * def most_frequent_substrings(             # <<<<<<<<<<<<<<
  *     np.ndarray[sa_t, ndim=1] lcp not None,
  *     sa_t length,
  */
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_2);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
 
-  /* "pydivsufsort/stringalg.pyx":223
+  /* "pydivsufsort/stringalg.pyx":226
  *     np.ndarray[sa_t, ndim=1] lcp not None,
  *     sa_t length,
  *     sa_t limit = 0,             # <<<<<<<<<<<<<<
  *     sa_t minimum_count = 1
  *     ):
  */
-  __pyx_t_2 = __Pyx_PyInt_From_long(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 223, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_long(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 226, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_k__6 = __pyx_t_2;
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "pydivsufsort/stringalg.pyx":224
+  /* "pydivsufsort/stringalg.pyx":227
  *     sa_t length,
  *     sa_t limit = 0,
  *     sa_t minimum_count = 1             # <<<<<<<<<<<<<<
  *     ):
  *     """
  */
-  __pyx_t_2 = __Pyx_PyInt_From_long(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 224, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_long(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 227, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_k__7 = __pyx_t_2;
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "pydivsufsort/stringalg.pyx":220
+  /* "pydivsufsort/stringalg.pyx":223
  * 
  * 
  * def most_frequent_substrings(             # <<<<<<<<<<<<<<
  *     np.ndarray[sa_t, ndim=1] lcp not None,
  *     sa_t length,
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_0__pyx_mdef_12pydivsufsort_9stringalg_123most_frequent_substrings, 0, __pyx_n_s_most_frequent_substrings, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__49)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_0__pyx_mdef_12pydivsufsort_9stringalg_125most_frequent_substrings, 0, __pyx_n_s_most_frequent_substrings, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__51)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (!__Pyx_CyFunction_InitDefaults(__pyx_t_1, sizeof(__pyx_defaults2), 0)) __PYX_ERR(0, 220, __pyx_L1_error)
+  if (!__Pyx_CyFunction_InitDefaults(__pyx_t_1, sizeof(__pyx_defaults2), 0)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_CyFunction_Defaults(__pyx_defaults2, __pyx_t_1)->__pyx_arg_limit = 0;
   __Pyx_CyFunction_Defaults(__pyx_defaults2, __pyx_t_1)->__pyx_arg_minimum_count = 1;
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_t_3);
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_1, __pyx_pf_12pydivsufsort_9stringalg_132__defaults__);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_int32_t, __pyx_t_1) < 0) __PYX_ERR(0, 220, __pyx_L1_error)
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_1, __pyx_pf_12pydivsufsort_9stringalg_134__defaults__);
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_int32_t, __pyx_t_1) < 0) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_1__pyx_mdef_12pydivsufsort_9stringalg_125most_frequent_substrings, 0, __pyx_n_s_most_frequent_substrings, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__49)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_1__pyx_mdef_12pydivsufsort_9stringalg_127most_frequent_substrings, 0, __pyx_n_s_most_frequent_substrings, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__51)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (!__Pyx_CyFunction_InitDefaults(__pyx_t_1, sizeof(__pyx_defaults3), 0)) __PYX_ERR(0, 220, __pyx_L1_error)
+  if (!__Pyx_CyFunction_InitDefaults(__pyx_t_1, sizeof(__pyx_defaults3), 0)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_CyFunction_Defaults(__pyx_defaults3, __pyx_t_1)->__pyx_arg_limit = 0;
   __Pyx_CyFunction_Defaults(__pyx_defaults3, __pyx_t_1)->__pyx_arg_minimum_count = 1;
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_t_3);
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_1, __pyx_pf_12pydivsufsort_9stringalg_134__defaults__);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_int64_t, __pyx_t_1) < 0) __PYX_ERR(0, 220, __pyx_L1_error)
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_1, __pyx_pf_12pydivsufsort_9stringalg_136__defaults__);
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_int64_t, __pyx_t_1) < 0) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_mdef_12pydivsufsort_9stringalg_19most_frequent_substrings, 0, __pyx_n_s_most_frequent_substrings, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__49)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_mdef_12pydivsufsort_9stringalg_21most_frequent_substrings, 0, __pyx_n_s_most_frequent_substrings, NULL, __pyx_n_s_pydivsufsort_stringalg, __pyx_d, ((PyObject *)__pyx_codeobj__51)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_t_3);
   ((__pyx_FusedFunctionObject *) __pyx_t_1)->__signatures__ = __pyx_t_2;
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_most_frequent_substrings, __pyx_t_1) < 0) __PYX_ERR(0, 220, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_most_frequent_substrings, __pyx_t_1) < 0) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pydivsufsort/stringalg.pyx":327
+  /* "pydivsufsort/stringalg.pyx":334
  * 
  * 
  * def _common_substrings(np.ndarray[ull, ndim=1] suffix_array, ull[::1] lcp, ull len1, ull limit):             # <<<<<<<<<<<<<<
  *     n = len(suffix_array)
  *     ranges = repeated_substrings(suffix_array, lcp)
  */
-  __pyx_t_3 = PyCFunction_NewEx(&__pyx_mdef_12pydivsufsort_9stringalg_23_common_substrings, NULL, __pyx_n_s_pydivsufsort_stringalg); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 327, __pyx_L1_error)
+  __pyx_t_3 = PyCFunction_NewEx(&__pyx_mdef_12pydivsufsort_9stringalg_25_common_substrings, NULL, __pyx_n_s_pydivsufsort_stringalg); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 334, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_common_substrings, __pyx_t_3) < 0) __PYX_ERR(0, 327, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_common_substrings, __pyx_t_3) < 0) __PYX_ERR(0, 334, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "pydivsufsort/stringalg.pyx":1
  * # cython: language_level=3, wraparound=False, boundscheck=False             # <<<<<<<<<<<<<<
  * # distutils: extra_compile_args=-O3
  * 
  */
@@ -47332,71 +47498,71 @@
   /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
  */
-  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__52, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 287, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__54, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 287, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_XGOTREF(generic);
   __Pyx_DECREF_SET(generic, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_3);
   __pyx_t_3 = 0;
 
   /* "View.MemoryView":288
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default             # <<<<<<<<<<<<<<
  * cdef indirect = Enum("<strided and indirect>")
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__53, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 288, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__55, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 288, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_XGOTREF(strided);
   __Pyx_DECREF_SET(strided, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_3);
   __pyx_t_3 = 0;
 
   /* "View.MemoryView":289
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__54, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 289, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__56, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 289, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_XGOTREF(indirect);
   __Pyx_DECREF_SET(indirect, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_3);
   __pyx_t_3 = 0;
 
   /* "View.MemoryView":292
  * 
  * 
  * cdef contiguous = Enum("<contiguous and direct>")             # <<<<<<<<<<<<<<
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__55, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 292, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__57, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 292, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_XGOTREF(contiguous);
   __Pyx_DECREF_SET(contiguous, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_3);
   __pyx_t_3 = 0;
 
   /* "View.MemoryView":293
  * 
  * cdef contiguous = Enum("<contiguous and direct>")
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__56, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 293, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__58, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 293, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_XGOTREF(indirect_contiguous);
   __Pyx_DECREF_SET(indirect_contiguous, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_3);
   __pyx_t_3 = 0;
 
   /* "View.MemoryView":317
```

### Comparing `pydivsufsort-0.0.8/pydivsufsort/stringalg.pyx` & `pydivsufsort-0.0.9/pydivsufsort/stringalg.pyx`

 * *Files 4% similar despite different names*

```diff
@@ -137,15 +137,15 @@
         lcp = kasai(s, sa)
     if isinstance(s, bytes):
         # tofix
         s = bytearray(s)
     return _lcp_segtree(s, sa, lcp)
 
 
-def lcp_query(
+def _lcp_query(
         np.ndarray[sa_t, ndim=1] rank not None,
         np.ndarray[sa_t, ndim=1] segtree not None,
         queries
     ):
     cdef sa_t n, q, i
 
     # note: l and r could hold 2*n-1
@@ -177,14 +177,17 @@
                 if segtree[r] < res:
                     res = segtree[r]
             l >>= 1 
             r >>= 1 
         ans[i] = res
     return ans
 
+def lcp_query(segtree, queries):
+    return _lcp_query(*segtree, queries)
+
 def _levenshtein(string_t[::1] a not None, string_t[::1] b not None):
     cdef unsigned long long n, m, i, j, d
     n = len(a)
     m = len(b)
     cdef np.ndarray[np.uint64_t, ndim=2] temp = np.empty((n+1, m+1), dtype=np.uint64)
     for i in range(n):
         temp[i][0] = i
@@ -220,14 +223,18 @@
 def most_frequent_substrings(
     np.ndarray[sa_t, ndim=1] lcp not None,
     sa_t length,
     sa_t limit = 0,
     sa_t minimum_count = 1
     ):
     """
+    Find the most frequent substrings of a given length in a string.
+    If `limit` is not 0, only the `limit` most frequent substrings are returned.
+    If `minimum_count` is not 1, only the substrings that occur at least `minimum_count` times are returned.
+
     Parameters
     ----------
 
     lcp : np.ndarray
         LCP array
     length : int
         length of the substrings to compare
```

### Comparing `pydivsufsort-0.0.8/pydivsufsort/wonderstring.py` & `pydivsufsort-0.0.9/pydivsufsort/wonderstring.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import numpy as np
 from collections import namedtuple
 
-from .divsufsort import _cast
 from . import (
     divsufsort,
     sa_search,
     kasai,
     lcp_segtree,
     lcp_query,
     most_frequent_substrings,
@@ -21,15 +20,15 @@
     if isinstance(inp, str):
         try:
             inp = inp.encode("ascii")
         except UnicodeEncodeError:
             raise TypeError("str must only contain ascii chars")
     if isinstance(inp, bytes):
         inp = np.frombuffer(inp, dtype=np.uint8)
-    return np.ascontiguousarray(_cast(np.array(inp, copy=copy)))
+    return np.ascontiguousarray(np.array(inp, copy=copy))
 
 
 class WonderString:
     def __init__(self, inp, copy=True):
         self.string = cast_to_numpy(inp, copy)
         self.itemsize = self.string.dtype.itemsize
 
@@ -54,14 +53,15 @@
             if self.itemsize == 1:
                 self._suffix_array = self.suffix_array_bytes
             else:
                 self._suffix_array = np.ascontiguousarray(
                     self.suffix_array_bytes[
                         self.suffix_array_bytes % self.itemsize == 0
                     ]
+                    // self.itemsize
                 )
         return self._suffix_array
 
     def search(self, pattern, return_positions=False):
         if self.itemsize != 1:
             raise NotImplementedError(
                 "Not supported for non byte strings.\n"
@@ -69,15 +69,15 @@
                 "<https://github.com/louisabraham/pydivsufsort/issues>"
             )
 
         ans = SearchResult(*sa_search(self.string, self.suffix_array, pattern))
 
         if return_positions:
             if not ans.count:
-                return None
+                return self.suffix_array[:0]
             return self.suffix_array[ans.position : ans.position + ans.count]
         return ans
 
     @property
     def lcp_array(self):
         if not hasattr(self, "_lcp_array"):
             self._lcp_array = kasai(self.string, self.suffix_array)
@@ -89,17 +89,17 @@
             self.__lcp_segtree = lcp_segtree(
                 self.string, self.suffix_array, self.lcp_array
             )
         return self.__lcp_segtree
 
     def lcp(self, *args):
         if len(args) == 1:
-            return lcp_query(*self._lcp_segtree, args[0])
+            return lcp_query(self._lcp_segtree, args[0])
         elif len(args) == 2:
-            return lcp_query(*self._lcp_segtree, [args])[0]
+            return lcp_query(self._lcp_segtree, [args])[0]
 
     def most_frequent_substrings(self, length, limit=0, minimum_count=1):
         """
         Parameters
         ----------
 
         lcp : np.ndarray
```

### Comparing `pydivsufsort-0.0.8/pydivsufsort.egg-info/PKG-INFO` & `pydivsufsort-0.0.9/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,348 +1,407 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 7079 6469  : 2.1.Name: pydi
-00000020: 7673 7566 736f 7274 0a56 6572 7369 6f6e  vsufsort.Version
-00000030: 3a20 302e 302e 380a 5375 6d6d 6172 793a  : 0.0.8.Summary:
-00000040: 2053 7472 696e 6720 616c 676f 7269 7468   String algorith
-00000050: 6d73 0a48 6f6d 652d 7061 6765 3a20 6874  ms.Home-page: ht
-00000060: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000070: 2f6c 6f75 6973 6162 7261 6861 6d2f 7079  /louisabraham/py
-00000080: 6469 7673 7566 736f 7274 0a41 7574 686f  divsufsort.Autho
-00000090: 723a 204c 6f75 6973 2041 6272 6168 616d  r: Louis Abraham
-000000a0: 0a41 7574 686f 722d 656d 6169 6c3a 206c  .Author-email: l
-000000b0: 6f75 6973 2e61 6272 6168 616d 4079 6168  ouis.abraham@yah
-000000c0: 6f6f 2e66 720a 4c69 6365 6e73 653a 204d  oo.fr.License: M
-000000d0: 4954 0a52 6571 7569 7265 732d 5079 7468  IT.Requires-Pyth
-000000e0: 6f6e 3a20 3e3d 332e 360a 4465 7363 7269  on: >=3.6.Descri
-000000f0: 7074 696f 6e2d 436f 6e74 656e 742d 5479  ption-Content-Ty
-00000100: 7065 3a20 7465 7874 2f6d 6172 6b64 6f77  pe: text/markdow
-00000110: 6e0a 4c69 6365 6e73 652d 4669 6c65 3a20  n.License-File: 
-00000120: 4c49 4345 4e53 450a 0a5b 215b 5079 5049  LICENSE..[![PyPI
-00000130: 0a76 6572 7369 6f6e 5d28 6874 7470 733a  .version](https:
-00000140: 2f2f 6261 6467 652e 6675 7279 2e69 6f2f  //badge.fury.io/
-00000150: 7079 2f70 7964 6976 7375 6673 6f72 742e  py/pydivsufsort.
-00000160: 7376 6729 5d28 6874 7470 733a 2f2f 6261  svg)](https://ba
-00000170: 6467 652e 6675 7279 2e69 6f2f 7079 2f70  dge.fury.io/py/p
-00000180: 7964 6976 7375 6673 6f72 7429 205b 215b  ydivsufsort) [![
-00000190: 446f 776e 6c6f 6164 735d 2868 7474 7073  Downloads](https
-000001a0: 3a2f 2f70 6570 792e 7465 6368 2f62 6164  ://pepy.tech/bad
-000001b0: 6765 2f70 7964 6976 7375 6673 6f72 7429  ge/pydivsufsort)
-000001c0: 5d28 6874 7470 733a 2f2f 7065 7079 2e74  ](https://pepy.t
-000001d0: 6563 682f 7072 6f6a 6563 742f 7079 6469  ech/project/pydi
-000001e0: 7673 7566 736f 7274 2920 5b21 5b54 6573  vsufsort) [![Tes
-000001f0: 745d 2868 7474 7073 3a2f 2f67 6974 6875  t](https://githu
-00000200: 622e 636f 6d2f 6c6f 7569 7361 6272 6168  b.com/louisabrah
-00000210: 616d 2f70 7964 6976 7375 6673 6f72 742f  am/pydivsufsort/
-00000220: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
-00000230: 732f 7465 7374 2e79 6d6c 2f62 6164 6765  s/test.yml/badge
-00000240: 2e73 7667 295d 2868 7474 7073 3a2f 2f67  .svg)](https://g
-00000250: 6974 6875 622e 636f 6d2f 6c6f 7569 7361  ithub.com/louisa
-00000260: 6272 6168 616d 2f70 7964 6976 7375 6673  braham/pydivsufs
-00000270: 6f72 742f 6163 7469 6f6e 732f 776f 726b  ort/actions/work
-00000280: 666c 6f77 732f 7465 7374 2e79 6d6c 2920  flows/test.yml) 
-00000290: 5b21 5b42 7569 6c64 2061 6e64 2075 706c  [![Build and upl
-000002a0: 6f61 645d 2868 7474 7073 3a2f 2f67 6974  oad](https://git
-000002b0: 6875 622e 636f 6d2f 6c6f 7569 7361 6272  hub.com/louisabr
-000002c0: 6168 616d 2f70 7964 6976 7375 6673 6f72  aham/pydivsufsor
-000002d0: 742f 6163 7469 6f6e 732f 776f 726b 666c  t/actions/workfl
-000002e0: 6f77 732f 6275 696c 642d 616e 642d 7570  ows/build-and-up
-000002f0: 6c6f 6164 2e79 6d6c 2f62 6164 6765 2e73  load.yml/badge.s
-00000300: 7667 295d 2868 7474 7073 3a2f 2f67 6974  vg)](https://git
-00000310: 6875 622e 636f 6d2f 6c6f 7569 7361 6272  hub.com/louisabr
-00000320: 6168 616d 2f70 7964 6976 7375 6673 6f72  aham/pydivsufsor
-00000330: 742f 6163 7469 6f6e 732f 776f 726b 666c  t/actions/workfl
-00000340: 6f77 732f 6275 696c 642d 616e 642d 7570  ows/build-and-up
-00000350: 6c6f 6164 2e79 6d6c 2920 5b21 5b63 6f64  load.yml) [![cod
-00000360: 6563 6f76 5d28 6874 7470 733a 2f2f 636f  ecov](https://co
-00000370: 6465 636f 762e 696f 2f67 682f 6c6f 7569  decov.io/gh/loui
-00000380: 7361 6272 6168 616d 2f70 7964 6976 7375  sabraham/pydivsu
-00000390: 6673 6f72 742f 6272 616e 6368 2f6d 6173  fsort/branch/mas
-000003a0: 7465 722f 6772 6170 682f 6261 6467 652e  ter/graph/badge.
-000003b0: 7376 673f 746f 6b65 6e3d 4131 424d 3955  svg?token=A1BM9U
-000003c0: 314f 4c56 295d 2868 7474 7073 3a2f 2f63  1OLV)](https://c
-000003d0: 6f64 6563 6f76 2e69 6f2f 6768 2f6c 6f75  odecov.io/gh/lou
-000003e0: 6973 6162 7261 6861 6d2f 7079 6469 7673  isabraham/pydivs
-000003f0: 7566 736f 7274 2920 5b21 5b44 4f49 5d28  ufsort) [![DOI](
-00000400: 6874 7470 733a 2f2f 7a65 6e6f 646f 2e6f  https://zenodo.o
-00000410: 7267 2f62 6164 6765 2f32 3431 3133 3739  rg/badge/2411379
-00000420: 3339 2e73 7667 295d 2868 7474 7073 3a2f  39.svg)](https:/
-00000430: 2f7a 656e 6f64 6f2e 6f72 672f 6261 6467  /zenodo.org/badg
-00000440: 652f 6c61 7465 7374 646f 692f 3234 3131  e/latestdoi/2411
-00000450: 3337 3933 3929 0a0a 2320 6070 7964 6976  37939)..# `pydiv
-00000460: 7375 6673 6f72 7460 3a20 6269 6e64 696e  sufsort`: bindin
-00000470: 6773 2074 6f20 6c69 6264 6976 7375 6673  gs to libdivsufs
-00000480: 6f72 740a 0a60 7079 6469 7673 7566 736f  ort..`pydivsufso
-00000490: 7274 6020 7072 6562 7569 6c64 7320 606c  rt` prebuilds `l
-000004a0: 6962 6469 7673 7566 736f 7274 6020 6173  ibdivsufsort` as
-000004b0: 2061 2073 6861 7265 6420 6c69 6272 6172   a shared librar
-000004c0: 7920 616e 640a 696e 636c 7564 6573 2069  y and.includes i
-000004d0: 7420 696e 2061 2050 7974 686f 6e20 7061  t in a Python pa
-000004e0: 636b 6167 6520 7769 7468 2062 696e 6469  ckage with bindi
-000004f0: 6e67 732e 0a0a 2a2a 4665 6174 7572 6573  ngs...**Features
-00000500: 2a2a 3a0a 0a2d 2062 696e 6469 6e67 7320  **:..- bindings 
-00000510: 746f 2060 6469 7673 7566 736f 7274 6020  to `divsufsort` 
-00000520: 7468 6174 2072 6574 7572 6e20 6e75 6d70  that return nump
-00000530: 7920 6172 7261 7973 0a2d 2068 616e 646c  y arrays.- handl
-00000540: 6520 616c 6d6f 7374 2061 6e79 2069 6e74  e almost any int
-00000550: 6567 6572 2064 6174 6120 7479 7065 2028  eger data type (
-00000560: 652e 672e 2060 696e 7436 3460 2920 616e  e.g. `int64`) an
-00000570: 6420 6e6f 7420 6f6e 6c79 2060 6368 6172  d not only `char
-00000580: 600a 2d20 6164 6469 7469 6f6e 616c 2073  `.- additional s
-00000590: 7472 696e 6720 616c 676f 7269 7468 6d73  tring algorithms
-000005a0: 0a0a 2323 2049 6e73 7461 6c6c 6174 696f  ..## Installatio
-000005b0: 6e0a 0a4f 6e20 4c69 6e75 782c 206d 6163  n..On Linux, mac
-000005c0: 4f53 2061 6e64 2057 696e 646f 7773 3a0a  OS and Windows:.
-000005d0: 0a60 6060 0a70 7974 686f 6e20 2d6d 2070  .```.python -m p
-000005e0: 6970 2069 6e73 7461 6c6c 2070 7964 6976  ip install pydiv
-000005f0: 7375 6673 6f72 740a 6060 600a 0a57 6520  sufsort.```..We 
-00000600: 7072 6f76 6964 6520 7072 6563 6f6d 7069  provide precompi
-00000610: 6c65 6420 7768 6565 6c73 2066 6f72 2063  led wheels for c
-00000620: 6f6d 6d6f 6e20 7379 7374 656d 7320 7573  ommon systems us
-00000630: 696e 6720 6063 6962 7569 6c64 7768 6565  ing `cibuildwhee
-00000640: 6c60 2c20 616e 6420 6120 736f 7572 6365  l`, and a source
-00000650: 2064 6973 7472 6962 7574 696f 6e20 666f   distribution fo
-00000660: 7220 556e 6978 2073 7973 7465 6d73 2e20  r Unix systems. 
-00000670: 4d61 6e75 616c 2063 6f6d 7069 6c61 7469  Manual compilati
-00000680: 6f6e 206f 6e20 5769 6e64 6f77 7320 6d69  on on Windows mi
-00000690: 6768 7420 7265 7175 6972 6520 736f 6d65  ght require some
-000006a0: 2074 7765 616b 696e 672c 2070 6c65 6173   tweaking, pleas
-000006b0: 6520 6372 6561 7465 2061 6e20 6973 7375  e create an issu
-000006c0: 652e 0a0a 2323 2055 7361 6765 0a0a 2323  e...## Usage..##
-000006d0: 2320 5573 696e 6720 5374 7269 6e67 2049  # Using String I
-000006e0: 6e70 7574 730a 0a60 6060 7079 7468 6f6e  nputs..```python
-000006f0: 0a69 6d70 6f72 7420 6e75 6d70 7920 6173  .import numpy as
-00000700: 206e 700a 6672 6f6d 2070 7964 6976 7375   np.from pydivsu
-00000710: 6673 6f72 7420 696d 706f 7274 2064 6976  fsort import div
-00000720: 7375 6673 6f72 742c 206b 6173 6169 0a0a  sufsort, kasai..
-00000730: 7374 7269 6e67 5f69 6e70 203d 2022 6261  string_inp = "ba
-00000740: 6e61 6e61 2422 0a73 7472 696e 675f 7375  nana$".string_su
-00000750: 6666 6978 5f61 7272 6179 203d 2064 6976  ffix_array = div
-00000760: 7375 6673 6f72 7428 7374 7269 6e67 5f69  sufsort(string_i
-00000770: 6e70 290a 7374 7269 6e67 5f6c 6370 5f61  np).string_lcp_a
-00000780: 7272 6179 203d 206b 6173 6169 2873 7472  rray = kasai(str
-00000790: 696e 675f 696e 702c 2073 7472 696e 675f  ing_inp, string_
-000007a0: 7375 6666 6978 5f61 7272 6179 290a 7072  suffix_array).pr
-000007b0: 696e 7428 7374 7269 6e67 5f73 7566 6669  int(string_suffi
-000007c0: 785f 6172 7261 792c 2073 7472 696e 675f  x_array, string_
-000007d0: 6c63 705f 6172 7261 7929 0a23 205b 3620  lcp_array).# [6 
-000007e0: 3520 3320 3120 3020 3420 325d 205b 3020  5 3 1 0 4 2] [0 
-000007f0: 3120 3320 3020 3020 3220 305d 0a60 6060  1 3 0 0 2 0].```
-00000800: 0a0a 2323 2320 5573 696e 6720 496e 7465  ..### Using Inte
-00000810: 6765 7220 496e 7075 7473 0a0a 6060 6070  ger Inputs..```p
-00000820: 7974 686f 6e0a 696d 706f 7274 206e 756d  ython.import num
-00000830: 7079 2061 7320 6e70 0a66 726f 6d20 7079  py as np.from py
-00000840: 6469 7673 7566 736f 7274 2069 6d70 6f72  divsufsort impor
-00000850: 7420 6469 7673 7566 736f 7274 2c20 6b61  t divsufsort, ka
-00000860: 7361 690a 0a73 7472 696e 675f 696e 7020  sai..string_inp 
-00000870: 3d20 2262 616e 616e 6124 220a 0a23 2043  = "banana$"..# C
-00000880: 6f6e 7665 7274 2074 6865 2073 7472 696e  onvert the strin
-00000890: 6720 696e 7075 7420 746f 2069 6e74 6567  g input to integ
-000008a0: 6572 7320 6669 7273 740a 696e 745f 696e  ers first.int_in
-000008b0: 7020 3d20 6e70 2e75 6e69 7175 6528 6e70  p = np.unique(np
-000008c0: 2e61 7272 6179 286c 6973 7428 7374 7269  .array(list(stri
-000008d0: 6e67 5f69 6e70 2929 2c20 7265 7475 726e  ng_inp)), return
-000008e0: 5f69 6e76 6572 7365 3d54 7275 6529 5b31  _inverse=True)[1
-000008f0: 5d0a 696e 745f 7375 6666 6978 5f61 7272  ].int_suffix_arr
-00000900: 6179 203d 2064 6976 7375 6673 6f72 7428  ay = divsufsort(
-00000910: 696e 745f 696e 7029 0a69 6e74 5f6c 6370  int_inp).int_lcp
-00000920: 5f61 7272 6179 203d 206b 6173 6169 2869  _array = kasai(i
-00000930: 6e74 5f69 6e70 2c20 696e 745f 7375 6666  nt_inp, int_suff
-00000940: 6978 5f61 7272 6179 290a 7072 696e 7428  ix_array).print(
-00000950: 696e 745f 7375 6666 6978 5f61 7272 6179  int_suffix_array
-00000960: 2c20 696e 745f 6c63 705f 6172 7261 7929  , int_lcp_array)
-00000970: 0a23 205b 3620 3520 3320 3120 3020 3420  .# [6 5 3 1 0 4 
-00000980: 325d 205b 3020 3120 3320 3020 3020 3220  2] [0 1 3 0 0 2 
-00000990: 305d 0a60 6060 0a0a 2323 2320 5573 696e  0].```..### Usin
-000009a0: 6720 4d75 6c74 6970 6c65 2053 656e 7469  g Multiple Senti
-000009b0: 6e65 6c20 4368 6172 6163 7465 7273 2057  nel Characters W
-000009c0: 6974 696e 2041 2053 7472 696e 670a 0a60  itin A String..`
-000009d0: 6060 7079 7468 6f6e 0a69 6d70 6f72 7420  ``python.import 
-000009e0: 6e75 6d70 7920 6173 206e 700a 6672 6f6d  numpy as np.from
-000009f0: 2070 7964 6976 7375 6673 6f72 7420 696d   pydivsufsort im
-00000a00: 706f 7274 2064 6976 7375 6673 6f72 742c  port divsufsort,
-00000a10: 206b 6173 6169 0a0a 7365 6e74 696e 656c   kasai..sentinel
-00000a20: 5f69 6e70 203d 2022 6124 6261 6e61 6e61  _inp = "a$banana
-00000a30: 2361 6e64 4061 2a62 616e 6461 6e61 2b22  #and@a*bandana+"
-00000a40: 0a73 656e 7469 6e65 6c5f 7375 6666 6978  .sentinel_suffix
-00000a50: 5f61 7272 6179 203d 2064 6976 7375 6673  _array = divsufs
-00000a60: 6f72 7428 7365 6e74 696e 656c 5f69 6e70  ort(sentinel_inp
-00000a70: 290a 7365 6e74 696e 656c 5f6c 6370 5f61  ).sentinel_lcp_a
-00000a80: 7272 6179 203d 206b 6173 6169 2873 656e  rray = kasai(sen
-00000a90: 7469 6e65 6c5f 696e 702c 2073 656e 7469  tinel_inp, senti
-00000aa0: 6e65 6c5f 7375 6666 6978 5f61 7272 6179  nel_suffix_array
-00000ab0: 290a 7072 696e 7428 7365 6e74 696e 656c  ).print(sentinel
-00000ac0: 5f73 7566 6669 785f 6172 7261 792c 2073  _suffix_array, s
-00000ad0: 656e 7469 6e65 6c5f 6c63 705f 6172 7261  entinel_lcp_arra
-00000ae0: 7929 0a23 205b 2038 2020 3120 3134 2032  y).# [ 8  1 14 2
-00000af0: 3220 3132 2020 3720 2030 2031 3320 3231  2 12  7  0 13 21
-00000b00: 2020 3520 3139 2020 3320 2039 2031 3620    5 19  3  9 16 
-00000b10: 2032 2031 3520 3131 2031 3820 2036 2032   2 15 11 18  6 2
-00000b20: 3020 2034 2031 3020 3137 5d20 5b30 2030  0  4 10 17] [0 0
-00000b30: 2030 2030 2030 2031 2031 2031 2031 2033   0 0 0 1 1 1 1 3
-00000b40: 2033 2032 2033 2030 2033 2030 2031 2030   3 2 3 0 3 0 1 0
-00000b50: 2032 2032 2031 2032 2030 5d0a 6060 600a   2 2 1 2 0].```.
-00000b60: 0a0a 2323 2044 6576 656c 6f70 6d65 6e74  ..## Development
-00000b70: 0a0a 596f 7520 6361 6e20 696e 7374 616c  ..You can instal
-00000b80: 6c20 6c6f 6361 6c6c 7920 7769 7468 0a0a  l locally with..
-00000b90: 6060 600a 7069 7020 696e 7374 616c 6c20  ```.pip install 
-00000ba0: 2d65 202e 0a60 6060 0a0a 4120 7573 6566  -e ..```..A usef
-00000bb0: 756c 2063 6f6d 6d61 6e64 2074 6f20 6974  ul command to it
-00000bc0: 6572 6174 6520 7175 6963 6b6c 7920 7768  erate quickly wh
-00000bd0: 656e 2063 6861 6e67 696e 6720 4379 7468  en changing Cyth
-00000be0: 6f6e 2063 6f64 6520 6973 0a0a 6060 600a  on code is..```.
-00000bf0: 7079 7468 6f6e 2073 6574 7570 2e70 7920  python setup.py 
-00000c00: 6275 696c 645f 6578 7420 2d2d 696e 706c  build_ext --inpl
-00000c10: 6163 6520 2626 2070 7974 6573 7420 2d73  ace && pytest -s
-00000c20: 0a60 6060 0a0a 2323 2320 5072 6f66 696c  .```..### Profil
-00000c30: 696e 670a 0a50 726f 6669 6c69 6e67 2063  ing..Profiling c
-00000c40: 616e 2062 6520 6163 7469 7661 7465 6420  an be activated 
-00000c50: 7769 7468 2074 6865 2065 6e76 6972 6f6e  with the environ
-00000c60: 6d65 6e74 2076 6172 6961 626c 6520 6050  ment variable `P
-00000c70: 524f 4649 4c45 603a 0a0a 6060 600a 5052  ROFILE`:..```.PR
-00000c80: 4f46 494c 453d 3120 7079 7468 6f6e 2073  OFILE=1 python s
-00000c90: 6574 7570 2e70 7920 6275 696c 645f 6578  etup.py build_ex
-00000ca0: 7420 2d2d 696e 706c 6163 6520 2626 2070  t --inplace && p
-00000cb0: 7974 6573 7420 2d73 0a60 6060 0a0a 4865  ytest -s.```..He
-00000cc0: 7265 2069 7320 616e 2065 7861 6d70 6c65  re is an example
-00000cd0: 2077 6974 6820 6c69 6e65 5f70 726f 6669   with line_profi
-00000ce0: 6c65 7220 2872 6571 7569 7265 7320 6070  ler (requires `p
-00000cf0: 6970 2069 6e73 7461 6c6c 2022 6c69 6e65  ip install "line
-00000d00: 5f70 726f 6669 6c65 723c 3422 6029 3a0a  _profiler<4"`):.
-00000d10: 0a60 6060 0a69 6d70 6f72 7420 6c69 6e65  .```.import line
-00000d20: 5f70 726f 6669 6c65 720a 6672 6f6d 2070  _profiler.from p
-00000d30: 7964 6976 7375 6673 6f72 7420 696d 706f  ydivsufsort impo
-00000d40: 7274 2063 6f6d 6d6f 6e5f 7375 6273 7472  rt common_substr
-00000d50: 696e 6773 0a66 726f 6d20 7079 6469 7673  ings.from pydivs
-00000d60: 7566 736f 7274 2e73 7472 696e 6761 6c67  ufsort.stringalg
-00000d70: 2069 6d70 6f72 7420 280a 2020 2020 5f63   import (.    _c
-00000d80: 6f6d 6d6f 6e5f 7375 6273 7472 696e 6773  ommon_substrings
-00000d90: 2c0a 2020 2020 7265 7065 6174 6564 5f73  ,.    repeated_s
-00000da0: 7562 7374 7269 6e67 732c 0a29 0a0a 7331  ubstrings,.)..s1
-00000db0: 203d 2022 6261 6e61 6e61 2220 2a20 3130   = "banana" * 10
-00000dc0: 3030 300a 7332 203d 2022 616e 616e 6173  000.s2 = "ananas
-00000dd0: 2220 2a20 3130 3030 300a 0a66 756e 6320  " * 10000..func 
-00000de0: 3d20 636f 6d6d 6f6e 5f73 7562 7374 7269  = common_substri
-00000df0: 6e67 730a 7072 6f66 696c 6520 3d20 6c69  ngs.profile = li
-00000e00: 6e65 5f70 726f 6669 6c65 722e 4c69 6e65  ne_profiler.Line
-00000e10: 5072 6f66 696c 6572 2866 756e 6329 0a70  Profiler(func).p
-00000e20: 726f 6669 6c65 2e61 6464 5f66 756e 6374  rofile.add_funct
-00000e30: 696f 6e28 5f63 6f6d 6d6f 6e5f 7375 6273  ion(_common_subs
-00000e40: 7472 696e 6773 290a 7072 6f66 696c 652e  trings).profile.
-00000e50: 6164 645f 6675 6e63 7469 6f6e 2872 6570  add_function(rep
-00000e60: 6561 7465 645f 7375 6273 7472 696e 6773  eated_substrings
-00000e70: 290a 7072 6f66 696c 652e 7275 6e63 616c  ).profile.runcal
-00000e80: 6c28 6675 6e63 2c20 7331 2c20 7332 2c20  l(func, s1, s2, 
-00000e90: 6c69 6d69 743d 3135 290a 7072 6f66 696c  limit=15).profil
-00000ea0: 652e 7072 696e 745f 7374 6174 7328 290a  e.print_stats().
-00000eb0: 6060 600a 0a23 2320 5465 7374 696e 670a  ```..## Testing.
-00000ec0: 0a60 6060 0a70 7974 6573 740a 6060 600a  .```.pytest.```.
-00000ed0: 0a23 2320 5465 6368 6e69 6361 6c20 6465  .## Technical de
-00000ee0: 7461 696c 7320 2866 6f72 2070 6572 666f  tails (for perfo
-00000ef0: 726d 616e 6365 2074 7765 616b 7329 0a0a  rmance tweaks)..
-00000f00: 606c 6962 6469 7673 7566 736f 7274 6020  `libdivsufsort` 
-00000f10: 6973 2063 6f6d 7069 6c65 6420 696e 2062  is compiled in b
-00000f20: 6f74 6820 3332 2061 6e64 2036 3420 6269  oth 32 and 64 bi
-00000f30: 7473 2c20 6173 205b 7468 6520 3332 2062  ts, as [the 32 b
-00000f40: 6974 7320 7665 7273 696f 6e20 6973 2066  its version is f
-00000f50: 6173 7465 725d 2868 7474 7073 3a2f 2f67  aster](https://g
-00000f60: 6974 6875 622e 636f 6d2f 792d 3235 362f  ithub.com/y-256/
-00000f70: 6c69 6264 6976 7375 6673 6f72 742f 6973  libdivsufsort/is
-00000f80: 7375 6573 2f32 3129 2e20 6070 7964 6976  sues/21). `pydiv
-00000f90: 7375 6673 6f72 7460 2061 7574 6f6d 6174  sufsort` automat
-00000fa0: 6963 616c 6c79 2063 686f 6f73 6573 2074  ically chooses t
-00000fb0: 6f20 7573 6520 7468 6520 3332 2062 6974  o use the 32 bit
-00000fc0: 7320 7665 7273 696f 6e20 7768 656e 2070  s version when p
-00000fd0: 6f73 7369 626c 6520 2861 6b61 2077 6865  ossible (aka whe
-00000fe0: 6e20 7468 6520 696e 7075 7420 7369 7a65  n the input size
-00000ff0: 2069 7320 6c65 7373 2074 6861 6e20 6032   is less than `2
-00001000: 2a2a 3331 2d31 6029 2e0a 0a46 6f72 2062  **31-1`)...For b
-00001010: 6573 7420 7065 7266 6f72 6d61 6e63 652c  est performance,
-00001020: 2075 7365 2063 6f6e 7469 6775 6f75 7320   use contiguous 
-00001030: 6172 7261 7973 2e20 4966 2079 6f75 2068  arrays. If you h
-00001040: 6176 6520 6120 736c 6963 6564 2061 7272  ave a sliced arr
-00001050: 6179 2c20 7079 6469 7673 7566 736f 7274  ay, pydivsufsort
-00001060: 2063 6f6e 7665 7274 7320 6974 2061 7574   converts it aut
-00001070: 6f6d 6174 6963 616c 6c79 2077 6974 6820  omatically with 
-00001080: 5b60 6e75 6d70 792e 6173 636f 6e74 6967  [`numpy.ascontig
-00001090: 756f 7573 6172 7261 7960 5d28 6874 7470  uousarray`](http
-000010a0: 733a 2f2f 646f 6373 2e73 6369 7079 2e6f  s://docs.scipy.o
-000010b0: 7267 2f64 6f63 2f6e 756d 7079 2f72 6566  rg/doc/numpy/ref
-000010c0: 6572 656e 6365 2f67 656e 6572 6174 6564  erence/generated
-000010d0: 2f6e 756d 7079 2e61 7363 6f6e 7469 6775  /numpy.ascontigu
-000010e0: 6f75 7361 7272 6179 2e68 746d 6c29 2e0a  ousarray.html)..
-000010f0: 0a54 6865 2070 7265 636f 6d70 696c 6564  .The precompiled
-00001100: 206c 6962 7261 7269 6573 2075 7365 204f   libraries use O
-00001110: 7065 6e4d 502e 2059 6f75 2063 616e 2064  penMP. You can d
-00001120: 6973 6162 6c65 2069 7420 6279 2073 6574  isable it by set
-00001130: 7469 6e67 2074 6865 2065 6e76 2076 6172  ting the env var
-00001140: 6961 626c 6520 604f 4d50 5f4e 554d 5f54  iable `OMP_NUM_T
-00001150: 4852 4541 4453 3d31 602c 2061 6e64 2069  HREADS=1`, and i
-00001160: 7420 7769 6c6c 2079 6965 6c64 2074 6865  t will yield the
-00001170: 2073 616d 6520 7065 7266 6f72 6d61 6e63   same performanc
-00001180: 6520 6173 2074 6865 2076 6572 7369 6f6e  e as the version
-00001190: 2063 6f6d 7069 6c65 6420 7769 7468 6f75   compiled withou
-000011a0: 7420 4f70 656e 4d50 0a0a 5468 6520 6f72  t OpenMP..The or
-000011b0: 6967 696e 616c 2060 6c69 6264 6976 7375  iginal `libdivsu
-000011c0: 6673 6f72 7460 206f 6e6c 7920 7375 7070  fsort` only supp
-000011d0: 6f72 7473 2063 6861 7220 6173 2074 6865  orts char as the
-000011e0: 2062 6173 6520 7479 7065 2e20 6070 7964   base type. `pyd
-000011f0: 6976 7375 6673 6f72 7460 2063 616e 2068  ivsufsort` can h
-00001200: 616e 646c 6520 6172 7261 7973 206f 6620  andle arrays of 
-00001210: 616e 7920 696e 7465 6765 7220 7479 7065  any integer type
-00001220: 2028 6576 656e 2073 6967 6e65 6429 2c20   (even signed), 
-00001230: 6279 2065 6e63 6f64 696e 6720 6561 6368  by encoding each
-00001240: 2065 6c65 6d65 6e74 2061 7320 6d75 6c74   element as mult
-00001250: 6970 6c65 2063 6861 7273 2c20 7768 6963  iple chars, whic
-00001260: 6820 6d61 6b65 7320 7468 6520 636f 6d70  h makes the comp
-00001270: 7574 6174 696f 6e20 736c 6f77 6572 2e20  utation slower. 
-00001280: 4966 2079 6f75 7220 7661 6c75 6573 2075  If your values u
-00001290: 7365 2061 6e20 696e 7465 6765 7220 7479  se an integer ty
-000012a0: 7065 2074 6861 7420 6973 2062 6967 6765  pe that is bigge
-000012b0: 7220 7468 616e 2072 6571 7569 7265 642c  r than required,
-000012c0: 2062 7574 2074 6865 7920 7370 616e 206f   but they span o
-000012d0: 7665 7220 6120 736d 616c 6c20 636f 6e74  ver a small cont
-000012e0: 6967 756f 7573 2072 616e 6765 2c20 6070  iguous range, `p
-000012f0: 7964 6976 7375 6673 6f72 7460 2077 696c  ydivsufsort` wil
-00001300: 6c20 6175 746f 6d61 7469 6361 6c6c 7920  l automatically 
-00001310: 6368 616e 6765 2074 6865 6972 2074 7970  change their typ
-00001320: 6520 2873 6565 205b 2336 5d28 6874 7470  e (see [#6](http
-00001330: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6c  s://github.com/l
-00001340: 6f75 6973 6162 7261 6861 6d2f 7079 6469  ouisabraham/pydi
-00001350: 7673 7566 736f 7274 2f69 7373 7565 732f  vsufsort/issues/
-00001360: 3629 292e 0a0a 2323 2041 636b 6e6f 776c  6))...## Acknowl
-00001370: 6564 6765 6d65 6e74 730a 0a2d 205b 5975  edgements..- [Yu
-00001380: 7461 204d 6f72 695d 2868 7474 7073 3a2f  ta Mori](https:/
-00001390: 2f67 6974 6875 622e 636f 6d2f 792d 3235  /github.com/y-25
-000013a0: 3629 2066 6f72 2077 7269 7469 6e67 205b  6) for writing [
-000013b0: 6c69 6264 6976 7375 6673 6f72 745d 2868  libdivsufsort](h
-000013c0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000013d0: 6d2f 792d 3235 362f 6c69 6264 6976 7375  m/y-256/libdivsu
-000013e0: 6673 6f72 7429 0a2d 205b 5365 616e 204c  fsort).- [Sean L
-000013f0: 6177 5d28 6874 7470 3a2f 2f73 6561 6e6c  aw](http://seanl
-00001400: 6177 2e67 6974 6875 622e 696f 2f29 2066  aw.github.io/) f
-00001410: 6f72 2069 6e69 7469 6174 696e 6720 7468  or initiating th
-00001420: 6973 2070 726f 6a65 6374 2061 6e64 2063  is project and c
-00001430: 6f6e 7472 6962 7574 696e 670a 0a23 2320  ontributing..## 
-00001440: 4369 7469 6e67 0a0a 4966 2079 6f75 2068  Citing..If you h
-00001450: 6176 6520 7573 6564 2074 6869 7320 736f  ave used this so
-00001460: 6674 7761 7265 2069 6e20 6120 7363 6965  ftware in a scie
-00001470: 6e74 6966 6963 2070 7562 6c69 6361 7469  ntific publicati
-00001480: 6f6e 2c20 706c 6561 7365 2063 6974 6520  on, please cite 
-00001490: 6974 2075 7369 6e67 2074 6865 2066 6f6c  it using the fol
-000014a0: 6c6f 7769 6e67 2042 6962 4c61 5465 5820  lowing BibLaTeX 
-000014b0: 636f 6465 3a0a 0a60 6060 0a40 736f 6674  code:..```.@soft
-000014c0: 7761 7265 7b70 7964 6976 7375 6673 6f72  ware{pydivsufsor
-000014d0: 742c 0a20 2061 7574 686f 7220 2020 2020  t,.  author     
-000014e0: 2020 3d20 7b4c 6f75 6973 2041 6272 6168    = {Louis Abrah
-000014f0: 616d 7d2c 0a20 2074 6974 6c65 2020 2020  am},.  title    
-00001500: 2020 2020 3d20 7b70 7964 6976 7375 6673      = {pydivsufs
-00001510: 6f72 747d 2c0a 2020 7965 6172 2020 2020  ort},.  year    
-00001520: 2020 2020 203d 2032 3032 332c 0a20 2070       = 2023,.  p
-00001530: 7562 6c69 7368 6572 2020 2020 3d20 7b5a  ublisher    = {Z
-00001540: 656e 6f64 6f7d 2c0a 2020 646f 6920 2020  enodo},.  doi   
-00001550: 2020 2020 2020 203d 207b 3130 2e35 3238         = {10.528
-00001560: 312f 7a65 6e6f 646f 2e37 3933 3234 3538  1/zenodo.7932458
-00001570: 7d2c 0a20 2075 726c 2020 2020 2020 2020  },.  url        
-00001580: 2020 3d20 7b68 7474 7073 3a2f 2f67 6974    = {https://git
-00001590: 6875 622e 636f 6d2f 6c6f 7569 7361 6272  hub.com/louisabr
-000015a0: 6168 616d 2f70 7964 6976 7375 6673 6f72  aham/pydivsufsor
-000015b0: 747d 0a7d 0a60 6060 0a                   t}.}.```.
+00000000: 5b21 5b50 7950 490a 7665 7273 696f 6e5d  [![PyPI.version]
+00000010: 2868 7474 7073 3a2f 2f62 6164 6765 2e66  (https://badge.f
+00000020: 7572 792e 696f 2f70 792f 7079 6469 7673  ury.io/py/pydivs
+00000030: 7566 736f 7274 2e73 7667 295d 2868 7474  ufsort.svg)](htt
+00000040: 7073 3a2f 2f62 6164 6765 2e66 7572 792e  ps://badge.fury.
+00000050: 696f 2f70 792f 7079 6469 7673 7566 736f  io/py/pydivsufso
+00000060: 7274 2920 5b21 5b44 6f77 6e6c 6f61 6473  rt) [![Downloads
+00000070: 5d28 6874 7470 733a 2f2f 7065 7079 2e74  ](https://pepy.t
+00000080: 6563 682f 6261 6467 652f 7079 6469 7673  ech/badge/pydivs
+00000090: 7566 736f 7274 295d 2868 7474 7073 3a2f  ufsort)](https:/
+000000a0: 2f70 6570 792e 7465 6368 2f70 726f 6a65  /pepy.tech/proje
+000000b0: 6374 2f70 7964 6976 7375 6673 6f72 7429  ct/pydivsufsort)
+000000c0: 205b 215b 5465 7374 5d28 6874 7470 733a   [![Test](https:
+000000d0: 2f2f 6769 7468 7562 2e63 6f6d 2f6c 6f75  //github.com/lou
+000000e0: 6973 6162 7261 6861 6d2f 7079 6469 7673  isabraham/pydivs
+000000f0: 7566 736f 7274 2f61 6374 696f 6e73 2f77  ufsort/actions/w
+00000100: 6f72 6b66 6c6f 7773 2f74 6573 742e 796d  orkflows/test.ym
+00000110: 6c2f 6261 6467 652e 7376 6729 5d28 6874  l/badge.svg)](ht
+00000120: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000130: 2f6c 6f75 6973 6162 7261 6861 6d2f 7079  /louisabraham/py
+00000140: 6469 7673 7566 736f 7274 2f61 6374 696f  divsufsort/actio
+00000150: 6e73 2f77 6f72 6b66 6c6f 7773 2f74 6573  ns/workflows/tes
+00000160: 742e 796d 6c29 205b 215b 4275 696c 6420  t.yml) [![Build 
+00000170: 616e 6420 7570 6c6f 6164 5d28 6874 7470  and upload](http
+00000180: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6c  s://github.com/l
+00000190: 6f75 6973 6162 7261 6861 6d2f 7079 6469  ouisabraham/pydi
+000001a0: 7673 7566 736f 7274 2f61 6374 696f 6e73  vsufsort/actions
+000001b0: 2f77 6f72 6b66 6c6f 7773 2f62 7569 6c64  /workflows/build
+000001c0: 2d61 6e64 2d75 706c 6f61 642e 796d 6c2f  -and-upload.yml/
+000001d0: 6261 6467 652e 7376 6729 5d28 6874 7470  badge.svg)](http
+000001e0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6c  s://github.com/l
+000001f0: 6f75 6973 6162 7261 6861 6d2f 7079 6469  ouisabraham/pydi
+00000200: 7673 7566 736f 7274 2f61 6374 696f 6e73  vsufsort/actions
+00000210: 2f77 6f72 6b66 6c6f 7773 2f62 7569 6c64  /workflows/build
+00000220: 2d61 6e64 2d75 706c 6f61 642e 796d 6c29  -and-upload.yml)
+00000230: 205b 215b 636f 6465 636f 765d 2868 7474   [![codecov](htt
+00000240: 7073 3a2f 2f63 6f64 6563 6f76 2e69 6f2f  ps://codecov.io/
+00000250: 6768 2f6c 6f75 6973 6162 7261 6861 6d2f  gh/louisabraham/
+00000260: 7079 6469 7673 7566 736f 7274 2f62 7261  pydivsufsort/bra
+00000270: 6e63 682f 6d61 7374 6572 2f67 7261 7068  nch/master/graph
+00000280: 2f62 6164 6765 2e73 7667 3f74 6f6b 656e  /badge.svg?token
+00000290: 3d41 3142 4d39 5531 4f4c 5629 5d28 6874  =A1BM9U1OLV)](ht
+000002a0: 7470 733a 2f2f 636f 6465 636f 762e 696f  tps://codecov.io
+000002b0: 2f67 682f 6c6f 7569 7361 6272 6168 616d  /gh/louisabraham
+000002c0: 2f70 7964 6976 7375 6673 6f72 7429 205b  /pydivsufsort) [
+000002d0: 215b 444f 495d 2868 7474 7073 3a2f 2f7a  ![DOI](https://z
+000002e0: 656e 6f64 6f2e 6f72 672f 6261 6467 652f  enodo.org/badge/
+000002f0: 3234 3131 3337 3933 392e 7376 6729 5d28  241137939.svg)](
+00000300: 6874 7470 733a 2f2f 7a65 6e6f 646f 2e6f  https://zenodo.o
+00000310: 7267 2f62 6164 6765 2f6c 6174 6573 7464  rg/badge/latestd
+00000320: 6f69 2f32 3431 3133 3739 3339 290a 0a23  oi/241137939)..#
+00000330: 2060 7079 6469 7673 7566 736f 7274 603a   `pydivsufsort`:
+00000340: 2062 696e 6469 6e67 7320 746f 206c 6962   bindings to lib
+00000350: 6469 7673 7566 736f 7274 0a0a 6070 7964  divsufsort..`pyd
+00000360: 6976 7375 6673 6f72 7460 2070 7265 6275  ivsufsort` prebu
+00000370: 696c 6473 2060 6c69 6264 6976 7375 6673  ilds `libdivsufs
+00000380: 6f72 7460 2061 7320 6120 7368 6172 6564  ort` as a shared
+00000390: 206c 6962 7261 7279 2061 6e64 0a69 6e63   library and.inc
+000003a0: 6c75 6465 7320 6974 2069 6e20 6120 5079  ludes it in a Py
+000003b0: 7468 6f6e 2070 6163 6b61 6765 2077 6974  thon package wit
+000003c0: 6820 6269 6e64 696e 6773 2e20 5768 6565  h bindings. Whee
+000003d0: 6c73 2061 7265 2062 7569 6c74 2066 6f72  ls are built for
+000003e0: 204c 696e 7578 2c20 6d61 634f 5320 616e   Linux, macOS an
+000003f0: 6420 5769 6e64 6f77 7320 2833 3220 616e  d Windows (32 an
+00000400: 6420 3634 2062 6974 7329 2075 7369 6e67  d 64 bits) using
+00000410: 2060 6369 6275 696c 6477 6865 656c 6020   `cibuildwheel` 
+00000420: 616e 6420 4769 7448 7562 2041 6374 696f  and GitHub Actio
+00000430: 6e73 2e20 4261 7369 6361 6c6c 792c 2079  ns. Basically, y
+00000440: 6f75 2073 686f 756c 6420 6265 2061 626c  ou should be abl
+00000450: 6520 746f 2069 6e73 7461 6c6c 2069 7420  e to install it 
+00000460: 7769 7468 2060 7069 7020 696e 7374 616c  with `pip instal
+00000470: 6c20 7079 6469 7673 7566 736f 7274 6020  l pydivsufsort` 
+00000480: 6f6e 2061 6e79 2073 7973 7465 6d20 616e  on any system an
+00000490: 6420 6974 2073 686f 756c 6420 776f 726b  d it should work
+000004a0: 206f 7574 206f 6620 7468 6520 626f 782e   out of the box.
+000004b0: 2049 6620 6974 2064 6f65 736e 2774 2c20   If it doesn't, 
+000004c0: 706c 6561 7365 2063 7265 6174 6520 616e  please create an
+000004d0: 2069 7373 7565 2e0a 0a2a 2a46 6561 7475   issue...**Featu
+000004e0: 7265 732a 2a3a 0a0a 2d20 6269 6e64 696e  res**:..- bindin
+000004f0: 6773 2074 6f20 6064 6976 7375 6673 6f72  gs to `divsufsor
+00000500: 7460 2074 6861 7420 7265 7475 726e 206e  t` that return n
+00000510: 756d 7079 2061 7272 6179 730a 2d20 6861  umpy arrays.- ha
+00000520: 6e64 6c65 2073 7472 696e 672c 2062 7974  ndle string, byt
+00000530: 6573 2061 6e64 2061 6c6d 6f73 7420 616e  es and almost an
+00000540: 7920 696e 7465 6765 7220 6461 7461 2074  y integer data t
+00000550: 7970 6520 2865 2e67 2e20 6069 6e74 3634  ype (e.g. `int64
+00000560: 6029 2061 6e64 206e 6f74 206f 6e6c 7920  `) and not only 
+00000570: 6063 6861 7260 0a2d 2061 6c67 6f72 6974  `char`.- algorit
+00000580: 686d 7320 776f 726b 2065 7665 6e20 666f  hms work even fo
+00000590: 7220 6e6f 6e20 6368 6172 2069 6e70 7574  r non char input
+000005a0: 730a 2d20 6164 6469 7469 6f6e 616c 2073  s.- additional s
+000005b0: 7472 696e 6720 616c 676f 7269 7468 6d73  tring algorithms
+000005c0: 2063 6f64 6564 2069 6e20 4379 7468 6f6e   coded in Cython
+000005d0: 0a0a 2323 2049 6e73 7461 6c6c 6174 696f  ..## Installatio
+000005e0: 6e0a 0a4f 6e20 4c69 6e75 782c 206d 6163  n..On Linux, mac
+000005f0: 4f53 2061 6e64 2057 696e 646f 7773 3a0a  OS and Windows:.
+00000600: 0a60 6060 0a70 7974 686f 6e20 2d6d 2070  .```.python -m p
+00000610: 6970 2069 6e73 7461 6c6c 2070 7964 6976  ip install pydiv
+00000620: 7375 6673 6f72 740a 6060 600a 0a57 6520  sufsort.```..We 
+00000630: 7072 6f76 6964 6520 7072 6563 6f6d 7069  provide precompi
+00000640: 6c65 6420 7768 6565 6c73 2066 6f72 2063  led wheels for c
+00000650: 6f6d 6d6f 6e20 7379 7374 656d 7320 7573  ommon systems us
+00000660: 696e 6720 6063 6962 7569 6c64 7768 6565  ing `cibuildwhee
+00000670: 6c60 2c20 616e 6420 6120 736f 7572 6365  l`, and a source
+00000680: 2064 6973 7472 6962 7574 696f 6e20 666f   distribution fo
+00000690: 7220 556e 6978 2073 7973 7465 6d73 2e20  r Unix systems. 
+000006a0: 4d61 6e75 616c 2063 6f6d 7069 6c61 7469  Manual compilati
+000006b0: 6f6e 206f 6e20 5769 6e64 6f77 7320 6d69  on on Windows mi
+000006c0: 6768 7420 7265 7175 6972 6520 736f 6d65  ght require some
+000006d0: 2074 7765 616b 696e 672c 2070 6c65 6173   tweaking, pleas
+000006e0: 6520 6372 6561 7465 2061 6e20 6973 7375  e create an issu
+000006f0: 652e 0a0a 2323 2046 6561 7475 7265 730a  e...## Features.
+00000700: 0a41 6c6c 206d 6574 686f 6473 2073 7570  .All methods sup
+00000710: 706f 7274 2073 7472 696e 672c 2062 7974  port string, byt
+00000720: 6573 2061 6e64 206e 756d 7079 2061 7272  es and numpy arr
+00000730: 6179 2069 6e70 7574 732c 2069 6e63 6c75  ay inputs, inclu
+00000740: 6469 6e67 2064 6174 6174 7970 6573 2067  ding datatypes g
+00000750: 7265 6174 6572 2074 6861 6e20 6075 696e  reater than `uin
+00000760: 7438 5f74 6020 2865 2e67 2e20 6075 696e  t8_t` (e.g. `uin
+00000770: 7436 345f 7460 292e 2042 656c 6f77 2061  t64_t`). Below a
+00000780: 7265 2074 6865 2073 6967 6e61 7475 7265  re the signature
+00000790: 7320 6f66 2061 6c6c 206d 6574 686f 6473  s of all methods
+000007a0: 2065 7870 6f73 6564 2062 7920 6070 7964   exposed by `pyd
+000007b0: 6976 7375 6673 6f72 7460 2e20 546f 2069  ivsufsort`. To i
+000007c0: 6d70 6f72 7420 6120 6d65 7468 6f64 2c20  mport a method, 
+000007d0: 6a75 7374 2064 6f20 6066 726f 6d20 7079  just do `from py
+000007e0: 6469 7673 7566 736f 7274 2069 6d70 6f72  divsufsort impor
+000007f0: 7420 6d65 7468 6f64 5f6e 616d 6560 2e20  t method_name`. 
+00000800: 416c 6c20 6d65 7468 6f64 7320 6172 6520  All methods are 
+00000810: 646f 6375 6d65 6e74 6564 2069 6e20 7468  documented in th
+00000820: 6520 646f 6373 7472 696e 6773 2e20 596f  e docstrings. Yo
+00000830: 7520 6361 6e20 6469 7370 6c61 7920 7468  u can display th
+00000840: 656d 2077 6974 6820 6068 656c 7028 6d65  em with `help(me
+00000850: 7468 6f64 5f6e 616d 6529 602e 0a0a 4120  thod_name)`...A 
+00000860: 6e69 6365 7220 696e 7465 7266 6163 6520  nicer interface 
+00000870: 746f 2072 6575 7365 2063 6f6d 7075 7461  to reuse computa
+00000880: 7469 6f6e 7320 6c61 7a69 6c79 2069 7320  tions lazily is 
+00000890: 7072 6f76 6964 6564 2069 6e20 576f 6e64  provided in Wond
+000008a0: 6572 5374 7269 6e67 2062 7574 2063 7572  erString but cur
+000008b0: 7265 6e74 6c79 2075 6e64 6f63 756d 656e  rently undocumen
+000008c0: 7465 642e 2050 6c65 6173 6520 6372 6561  ted. Please crea
+000008d0: 7465 2061 6e20 6973 7375 6520 6966 2079  te an issue if y
+000008e0: 6f75 2061 7265 2069 6e74 6572 6573 7465  ou are intereste
+000008f0: 642e 0a0a 2323 2320 4d65 7468 6f64 7320  d...### Methods 
+00000900: 6578 706f 7365 6420 6672 6f6d 206c 6962  exposed from lib
+00000910: 6469 7673 7566 736f 7274 0a0a 2d20 6064  divsufsort..- `d
+00000920: 6976 7375 6673 6f72 7428 7374 7269 6e67  ivsufsort(string
+00000930: 2960 3a20 7375 6666 6978 2061 7272 6179  )`: suffix array
+00000940: 0a2d 2060 6277 5f74 7261 6e73 666f 726d  .- `bw_transform
+00000950: 2873 7472 696e 6729 603a 2042 7572 726f  (string)`: Burro
+00000960: 7773 2d57 6865 656c 6572 2074 7261 6e73  ws-Wheeler trans
+00000970: 666f 726d 0a2d 2060 696e 7665 7273 655f  form.- `inverse_
+00000980: 6277 5f74 7261 6e73 666f 726d 2869 6478  bw_transform(idx
+00000990: 2c20 7374 7269 6e67 2960 3a20 696e 7665  , string)`: inve
+000009a0: 7273 6520 4275 7272 6f77 732d 5768 6565  rse Burrows-Whee
+000009b0: 6c65 7220 7472 616e 7366 6f72 6d0a 2d20  ler transform.- 
+000009c0: 6073 615f 7365 6172 6368 2873 7472 696e  `sa_search(strin
+000009d0: 672c 2073 7566 6669 785f 6172 7261 792c  g, suffix_array,
+000009e0: 2070 6174 7465 726e 2960 3a20 7365 6172   pattern)`: sear
+000009f0: 6368 2066 6f72 2061 2070 6174 7465 726e  ch for a pattern
+00000a00: 2069 6e20 6120 7375 6666 6978 2061 7272   in a suffix arr
+00000a10: 6179 0a0a 0a23 2323 2041 6464 6974 696f  ay...### Additio
+00000a20: 6e61 6c20 7374 7269 6e67 2061 6c67 6f72  nal string algor
+00000a30: 6974 686d 730a 0a2d 2060 6b61 7361 6928  ithms..- `kasai(
+00000a40: 7374 7269 6e67 2c20 7375 6666 6978 5f61  string, suffix_a
+00000a50: 7272 6179 3d4e 6f6e 6529 603a 204c 4350  rray=None)`: LCP
+00000a60: 2061 7272 6179 2063 6f6d 7075 7461 7469   array computati
+00000a70: 6f6e 2028 6c61 7a69 6c79 2063 6f6d 7075  on (lazily compu
+00000a80: 7465 7320 7468 6520 7375 6666 6978 2061  tes the suffix a
+00000a90: 7272 6179 2069 6620 6e6f 7420 7072 6f76  rray if not prov
+00000aa0: 6964 6564 290a 2d20 606c 6370 5f73 6567  ided).- `lcp_seg
+00000ab0: 7472 6565 2873 7472 696e 672c 2073 7566  tree(string, suf
+00000ac0: 6669 785f 6172 7261 793d 4e6f 6e65 2c20  fix_array=None, 
+00000ad0: 6c63 703d 4e6f 6e65 2960 3a20 6275 696c  lcp=None)`: buil
+00000ae0: 6420 6120 7365 676d 656e 7420 7472 6565  d a segment tree
+00000af0: 2066 6f72 204c 4350 2071 7565 7269 6573   for LCP queries
+00000b00: 2028 6c61 7a69 6c79 2063 6f6d 7075 7465   (lazily compute
+00000b10: 7320 7468 6520 7375 6666 6978 2061 7272  s the suffix arr
+00000b20: 6179 2061 6e64 204c 4350 2061 7272 6179  ay and LCP array
+00000b30: 2069 6620 6e6f 7420 7072 6f76 6964 6564   if not provided
+00000b40: 290a 2d20 606c 6370 5f71 7565 7279 2873  ).- `lcp_query(s
+00000b50: 6567 7472 6565 2c20 7175 6572 6965 7329  egtree, queries)
+00000b60: 603a 2071 7565 7279 2061 2073 6567 6d65  `: query a segme
+00000b70: 6e74 2074 7265 6520 666f 7220 4c43 5020  nt tree for LCP 
+00000b80: 7175 6572 6965 732e 2051 7565 7269 6573  queries. Queries
+00000b90: 2061 7265 2070 6169 7273 206f 6620 696e   are pairs of in
+00000ba0: 6469 6365 732e 0a2d 2060 6c65 7665 6e73  dices..- `levens
+00000bb0: 6874 6569 6e28 7374 7269 6e67 312c 2073  htein(string1, s
+00000bc0: 7472 696e 6732 2960 3a20 4c65 7665 6e73  tring2)`: Levens
+00000bd0: 6874 6569 6e20 6469 7374 616e 6365 0a2d  htein distance.-
+00000be0: 2060 6d6f 7374 5f66 7265 7175 656e 745f   `most_frequent_
+00000bf0: 7375 6273 7472 696e 6773 286c 6370 2c20  substrings(lcp, 
+00000c00: 6c65 6e67 7468 2c20 6c69 6d69 743d 302c  length, limit=0,
+00000c10: 206d 696e 696d 756d 5f63 6f75 6e74 3d31   minimum_count=1
+00000c20: 2960 3a20 6d6f 7374 2066 7265 7175 656e  )`: most frequen
+00000c30: 7420 7375 6273 7472 696e 6773 2e20 5365  t substrings. Se
+00000c40: 6520 7468 6520 646f 6373 7472 696e 6720  e the docstring 
+00000c50: 666f 7220 6465 7461 696c 732e 0a2d 2060  for details..- `
+00000c60: 636f 6d6d 6f6e 5f73 7562 7374 7269 6e67  common_substring
+00000c70: 7328 7374 7269 6e67 312c 2073 7472 696e  s(string1, strin
+00000c80: 6732 2c20 6c69 6d69 743d 3235 2960 3a20  g2, limit=25)`: 
+00000c90: 636f 6d6d 6f6e 2073 7562 7374 7269 6e67  common substring
+00000ca0: 7320 6265 7477 6565 6e20 7477 6f20 7374  s between two st
+00000cb0: 7269 6e67 732e 0a0a 0a23 2323 2045 7861  rings....### Exa
+00000cc0: 6d70 6c65 2075 7361 6765 0a0a 6060 6070  mple usage..```p
+00000cd0: 7974 686f 6e0a 6672 6f6d 2070 7964 6976  ython.from pydiv
+00000ce0: 7375 6673 6f72 7420 696d 706f 7274 2064  sufsort import d
+00000cf0: 6976 7375 6673 6f72 742c 206b 6173 6169  ivsufsort, kasai
+00000d00: 0a0a 7374 7269 6e67 5f69 6e70 203d 2022  ..string_inp = "
+00000d10: 6261 6e61 6e61 2422 0a73 7472 696e 675f  banana$".string_
+00000d20: 7375 6666 6978 5f61 7272 6179 203d 2064  suffix_array = d
+00000d30: 6976 7375 6673 6f72 7428 7374 7269 6e67  ivsufsort(string
+00000d40: 5f69 6e70 290a 7374 7269 6e67 5f6c 6370  _inp).string_lcp
+00000d50: 5f61 7272 6179 203d 206b 6173 6169 2873  _array = kasai(s
+00000d60: 7472 696e 675f 696e 702c 2073 7472 696e  tring_inp, strin
+00000d70: 675f 7375 6666 6978 5f61 7272 6179 290a  g_suffix_array).
+00000d80: 7072 696e 7428 7374 7269 6e67 5f73 7566  print(string_suf
+00000d90: 6669 785f 6172 7261 792c 2073 7472 696e  fix_array, strin
+00000da0: 675f 6c63 705f 6172 7261 7929 0a23 205b  g_lcp_array).# [
+00000db0: 3620 3520 3320 3120 3020 3420 325d 205b  6 5 3 1 0 4 2] [
+00000dc0: 3020 3120 3320 3020 3020 3220 305d 0a0a  0 1 3 0 0 2 0]..
+00000dd0: 2320 596f 7520 6361 6e20 616c 736f 2063  # You can also c
+00000de0: 6f6e 7665 7274 2074 6865 2073 7472 696e  onvert the strin
+00000df0: 6720 696e 7075 7420 746f 2069 6e74 6567  g input to integ
+00000e00: 6572 7320 6669 7273 740a 0a69 6d70 6f72  ers first..impor
+00000e10: 7420 6e75 6d70 7920 6173 206e 700a 0a69  t numpy as np..i
+00000e20: 6e74 5f69 6e70 203d 206e 702e 756e 6971  nt_inp = np.uniq
+00000e30: 7565 286e 702e 6172 7261 7928 6c69 7374  ue(np.array(list
+00000e40: 2873 7472 696e 675f 696e 7029 292c 2072  (string_inp)), r
+00000e50: 6574 7572 6e5f 696e 7665 7273 653d 5472  eturn_inverse=Tr
+00000e60: 7565 295b 315d 0a69 6e74 5f73 7566 6669  ue)[1].int_suffi
+00000e70: 785f 6172 7261 7920 3d20 6469 7673 7566  x_array = divsuf
+00000e80: 736f 7274 2869 6e74 5f69 6e70 290a 696e  sort(int_inp).in
+00000e90: 745f 6c63 705f 6172 7261 7920 3d20 6b61  t_lcp_array = ka
+00000ea0: 7361 6928 696e 745f 696e 702c 2069 6e74  sai(int_inp, int
+00000eb0: 5f73 7566 6669 785f 6172 7261 7929 0a70  _suffix_array).p
+00000ec0: 7269 6e74 2869 6e74 5f73 7566 6669 785f  rint(int_suffix_
+00000ed0: 6172 7261 792c 2069 6e74 5f6c 6370 5f61  array, int_lcp_a
+00000ee0: 7272 6179 290a 2320 5b36 2035 2033 2031  rray).# [6 5 3 1
+00000ef0: 2030 2034 2032 5d20 5b30 2031 2033 2030   0 4 2] [0 1 3 0
+00000f00: 2030 2032 2030 5d0a 6060 600a 0a0a 2323   0 2 0].```...##
+00000f10: 2044 6576 656c 6f70 6d65 6e74 0a0a 596f   Development..Yo
+00000f20: 7520 6361 6e20 696e 7374 616c 6c20 6c6f  u can install lo
+00000f30: 6361 6c6c 7920 7769 7468 0a0a 6060 600a  cally with..```.
+00000f40: 7069 7020 696e 7374 616c 6c20 2d65 202e  pip install -e .
+00000f50: 0a60 6060 0a0a 4120 7573 6566 756c 2063  .```..A useful c
+00000f60: 6f6d 6d61 6e64 2074 6f20 6974 6572 6174  ommand to iterat
+00000f70: 6520 7175 6963 6b6c 7920 7768 656e 2063  e quickly when c
+00000f80: 6861 6e67 696e 6720 4379 7468 6f6e 2063  hanging Cython c
+00000f90: 6f64 6520 6973 0a0a 6060 600a 7079 7468  ode is..```.pyth
+00000fa0: 6f6e 2073 6574 7570 2e70 7920 6275 696c  on setup.py buil
+00000fb0: 645f 6578 7420 2d2d 696e 706c 6163 6520  d_ext --inplace 
+00000fc0: 2626 2070 7974 6573 7420 2d73 0a60 6060  && pytest -s.```
+00000fd0: 0a0a 2323 2320 5072 6f66 696c 696e 670a  ..### Profiling.
+00000fe0: 0a50 726f 6669 6c69 6e67 2063 616e 2062  .Profiling can b
+00000ff0: 6520 6163 7469 7661 7465 6420 7769 7468  e activated with
+00001000: 2074 6865 2065 6e76 6972 6f6e 6d65 6e74   the environment
+00001010: 2076 6172 6961 626c 6520 6050 524f 4649   variable `PROFI
+00001020: 4c45 603a 0a0a 6060 600a 5052 4f46 494c  LE`:..```.PROFIL
+00001030: 453d 3120 7079 7468 6f6e 2073 6574 7570  E=1 python setup
+00001040: 2e70 7920 6275 696c 645f 6578 7420 2d2d  .py build_ext --
+00001050: 696e 706c 6163 6520 2626 2070 7974 6573  inplace && pytes
+00001060: 7420 2d73 0a60 6060 0a0a 4865 7265 2069  t -s.```..Here i
+00001070: 7320 616e 2065 7861 6d70 6c65 2077 6974  s an example wit
+00001080: 6820 6c69 6e65 5f70 726f 6669 6c65 7220  h line_profiler 
+00001090: 2872 6571 7569 7265 7320 6070 6970 2069  (requires `pip i
+000010a0: 6e73 7461 6c6c 2022 6c69 6e65 5f70 726f  nstall "line_pro
+000010b0: 6669 6c65 723c 3422 6029 3a0a 0a60 6060  filer<4"`):..```
+000010c0: 0a69 6d70 6f72 7420 6c69 6e65 5f70 726f  .import line_pro
+000010d0: 6669 6c65 720a 6672 6f6d 2070 7964 6976  filer.from pydiv
+000010e0: 7375 6673 6f72 7420 696d 706f 7274 2063  sufsort import c
+000010f0: 6f6d 6d6f 6e5f 7375 6273 7472 696e 6773  ommon_substrings
+00001100: 0a66 726f 6d20 7079 6469 7673 7566 736f  .from pydivsufso
+00001110: 7274 2e73 7472 696e 6761 6c67 2069 6d70  rt.stringalg imp
+00001120: 6f72 7420 280a 2020 2020 5f63 6f6d 6d6f  ort (.    _commo
+00001130: 6e5f 7375 6273 7472 696e 6773 2c0a 2020  n_substrings,.  
+00001140: 2020 7265 7065 6174 6564 5f73 7562 7374    repeated_subst
+00001150: 7269 6e67 732c 0a29 0a0a 7331 203d 2022  rings,.)..s1 = "
+00001160: 6261 6e61 6e61 2220 2a20 3130 3030 300a  banana" * 10000.
+00001170: 7332 203d 2022 616e 616e 6173 2220 2a20  s2 = "ananas" * 
+00001180: 3130 3030 300a 0a66 756e 6320 3d20 636f  10000..func = co
+00001190: 6d6d 6f6e 5f73 7562 7374 7269 6e67 730a  mmon_substrings.
+000011a0: 7072 6f66 696c 6520 3d20 6c69 6e65 5f70  profile = line_p
+000011b0: 726f 6669 6c65 722e 4c69 6e65 5072 6f66  rofiler.LineProf
+000011c0: 696c 6572 2866 756e 6329 0a70 726f 6669  iler(func).profi
+000011d0: 6c65 2e61 6464 5f66 756e 6374 696f 6e28  le.add_function(
+000011e0: 5f63 6f6d 6d6f 6e5f 7375 6273 7472 696e  _common_substrin
+000011f0: 6773 290a 7072 6f66 696c 652e 6164 645f  gs).profile.add_
+00001200: 6675 6e63 7469 6f6e 2872 6570 6561 7465  function(repeate
+00001210: 645f 7375 6273 7472 696e 6773 290a 7072  d_substrings).pr
+00001220: 6f66 696c 652e 7275 6e63 616c 6c28 6675  ofile.runcall(fu
+00001230: 6e63 2c20 7331 2c20 7332 2c20 6c69 6d69  nc, s1, s2, limi
+00001240: 743d 3135 290a 7072 6f66 696c 652e 7072  t=15).profile.pr
+00001250: 696e 745f 7374 6174 7328 290a 6060 600a  int_stats().```.
+00001260: 0a23 2320 5465 7374 696e 670a 0a60 6060  .## Testing..```
+00001270: 0a70 7974 6573 740a 6060 600a 0a23 2320  .pytest.```..## 
+00001280: 5465 6368 6e69 6361 6c20 6465 7461 696c  Technical detail
+00001290: 7320 2866 6f72 2070 6572 666f 726d 616e  s (for performan
+000012a0: 6365 2074 7765 616b 7329 0a0a 606c 6962  ce tweaks)..`lib
+000012b0: 6469 7673 7566 736f 7274 6020 6973 2063  divsufsort` is c
+000012c0: 6f6d 7069 6c65 6420 696e 2062 6f74 6820  ompiled in both 
+000012d0: 3332 2061 6e64 2036 3420 6269 7473 2c20  32 and 64 bits, 
+000012e0: 6173 205b 7468 6520 3332 2062 6974 7320  as [the 32 bits 
+000012f0: 7665 7273 696f 6e20 6973 2066 6173 7465  version is faste
+00001300: 725d 2868 7474 7073 3a2f 2f67 6974 6875  r](https://githu
+00001310: 622e 636f 6d2f 792d 3235 362f 6c69 6264  b.com/y-256/libd
+00001320: 6976 7375 6673 6f72 742f 6973 7375 6573  ivsufsort/issues
+00001330: 2f32 3129 2e20 6070 7964 6976 7375 6673  /21). `pydivsufs
+00001340: 6f72 7460 2061 7574 6f6d 6174 6963 616c  ort` automatical
+00001350: 6c79 2063 686f 6f73 6573 2074 6f20 7573  ly chooses to us
+00001360: 6520 7468 6520 3332 2062 6974 7320 7665  e the 32 bits ve
+00001370: 7273 696f 6e20 7768 656e 2070 6f73 7369  rsion when possi
+00001380: 626c 6520 2861 6b61 2077 6865 6e20 7468  ble (aka when th
+00001390: 6520 696e 7075 7420 7369 7a65 2069 7320  e input size is 
+000013a0: 6c65 7373 2074 6861 6e20 6032 2a2a 3331  less than `2**31
+000013b0: 2d31 6029 2e0a 0a46 6f72 2062 6573 7420  -1`)...For best 
+000013c0: 7065 7266 6f72 6d61 6e63 652c 2075 7365  performance, use
+000013d0: 2063 6f6e 7469 6775 6f75 7320 6172 7261   contiguous arra
+000013e0: 7973 2e20 4966 2079 6f75 2068 6176 6520  ys. If you have 
+000013f0: 6120 736c 6963 6564 2061 7272 6179 2c20  a sliced array, 
+00001400: 7079 6469 7673 7566 736f 7274 2063 6f6e  pydivsufsort con
+00001410: 7665 7274 7320 6974 2061 7574 6f6d 6174  verts it automat
+00001420: 6963 616c 6c79 2077 6974 6820 5b60 6e75  ically with [`nu
+00001430: 6d70 792e 6173 636f 6e74 6967 756f 7573  mpy.ascontiguous
+00001440: 6172 7261 7960 5d28 6874 7470 733a 2f2f  array`](https://
+00001450: 646f 6373 2e73 6369 7079 2e6f 7267 2f64  docs.scipy.org/d
+00001460: 6f63 2f6e 756d 7079 2f72 6566 6572 656e  oc/numpy/referen
+00001470: 6365 2f67 656e 6572 6174 6564 2f6e 756d  ce/generated/num
+00001480: 7079 2e61 7363 6f6e 7469 6775 6f75 7361  py.ascontiguousa
+00001490: 7272 6179 2e68 746d 6c29 2e0a 0a54 6865  rray.html)...The
+000014a0: 2070 7265 636f 6d70 696c 6564 206c 6962   precompiled lib
+000014b0: 7261 7269 6573 2075 7365 204f 7065 6e4d  raries use OpenM
+000014c0: 502e 2059 6f75 2063 616e 2064 6973 6162  P. You can disab
+000014d0: 6c65 2069 7420 6279 2073 6574 7469 6e67  le it by setting
+000014e0: 2074 6865 2065 6e76 2076 6172 6961 626c   the env variabl
+000014f0: 6520 604f 4d50 5f4e 554d 5f54 4852 4541  e `OMP_NUM_THREA
+00001500: 4453 3d31 602c 2061 6e64 2069 7420 7769  DS=1`, and it wi
+00001510: 6c6c 2079 6965 6c64 2074 6865 2073 616d  ll yield the sam
+00001520: 6520 7065 7266 6f72 6d61 6e63 6520 6173  e performance as
+00001530: 2074 6865 2076 6572 7369 6f6e 2063 6f6d   the version com
+00001540: 7069 6c65 6420 7769 7468 6f75 7420 4f70  piled without Op
+00001550: 656e 4d50 0a0a 5468 6520 6f72 6967 696e  enMP..The origin
+00001560: 616c 2060 6c69 6264 6976 7375 6673 6f72  al `libdivsufsor
+00001570: 7460 206f 6e6c 7920 7375 7070 6f72 7473  t` only supports
+00001580: 2063 6861 7220 6173 2074 6865 2062 6173   char as the bas
+00001590: 6520 7479 7065 2e20 6070 7964 6976 7375  e type. `pydivsu
+000015a0: 6673 6f72 7460 2063 616e 2068 616e 646c  fsort` can handl
+000015b0: 6520 6172 7261 7973 206f 6620 616e 7920  e arrays of any 
+000015c0: 696e 7465 6765 7220 7479 7065 2028 6576  integer type (ev
+000015d0: 656e 2073 6967 6e65 6429 2c20 6279 2065  en signed), by e
+000015e0: 6e63 6f64 696e 6720 6561 6368 2065 6c65  ncoding each ele
+000015f0: 6d65 6e74 2061 7320 6d75 6c74 6970 6c65  ment as multiple
+00001600: 2063 6861 7273 2c20 7768 6963 6820 6d61   chars, which ma
+00001610: 6b65 7320 7468 6520 636f 6d70 7574 6174  kes the computat
+00001620: 696f 6e20 736c 6f77 6572 2e20 4966 2079  ion slower. If y
+00001630: 6f75 7220 7661 6c75 6573 2075 7365 2061  our values use a
+00001640: 6e20 696e 7465 6765 7220 7479 7065 2074  n integer type t
+00001650: 6861 7420 6973 2062 6967 6765 7220 7468  hat is bigger th
+00001660: 616e 2072 6571 7569 7265 642c 2062 7574  an required, but
+00001670: 2074 6865 7920 7370 616e 206f 7665 7220   they span over 
+00001680: 6120 736d 616c 6c20 636f 6e74 6967 756f  a small contiguo
+00001690: 7573 2072 616e 6765 2c20 6070 7964 6976  us range, `pydiv
+000016a0: 7375 6673 6f72 7460 2077 696c 6c20 6175  sufsort` will au
+000016b0: 746f 6d61 7469 6361 6c6c 7920 6368 616e  tomatically chan
+000016c0: 6765 2074 6865 6972 2074 7970 6520 2873  ge their type (s
+000016d0: 6565 205b 2336 5d28 6874 7470 733a 2f2f  ee [#6](https://
+000016e0: 6769 7468 7562 2e63 6f6d 2f6c 6f75 6973  github.com/louis
+000016f0: 6162 7261 6861 6d2f 7079 6469 7673 7566  abraham/pydivsuf
+00001700: 736f 7274 2f69 7373 7565 732f 3629 292e  sort/issues/6)).
+00001710: 0a0a 2323 2041 636b 6e6f 776c 6564 6765  ..## Acknowledge
+00001720: 6d65 6e74 730a 0a2d 205b 5975 7461 204d  ments..- [Yuta M
+00001730: 6f72 695d 2868 7474 7073 3a2f 2f67 6974  ori](https://git
+00001740: 6875 622e 636f 6d2f 792d 3235 3629 2066  hub.com/y-256) f
+00001750: 6f72 2077 7269 7469 6e67 205b 6c69 6264  or writing [libd
+00001760: 6976 7375 6673 6f72 745d 2868 7474 7073  ivsufsort](https
+00001770: 3a2f 2f67 6974 6875 622e 636f 6d2f 792d  ://github.com/y-
+00001780: 3235 362f 6c69 6264 6976 7375 6673 6f72  256/libdivsufsor
+00001790: 7429 0a2d 205b 5365 616e 204c 6177 5d28  t).- [Sean Law](
+000017a0: 6874 7470 3a2f 2f73 6561 6e6c 6177 2e67  http://seanlaw.g
+000017b0: 6974 6875 622e 696f 2f29 2066 6f72 2069  ithub.io/) for i
+000017c0: 6e69 7469 6174 696e 6720 7468 6973 2070  nitiating this p
+000017d0: 726f 6a65 6374 2061 6e64 2063 6f6e 7472  roject and contr
+000017e0: 6962 7574 696e 670a 0a23 2320 4369 7469  ibuting..## Citi
+000017f0: 6e67 0a0a 4966 2079 6f75 2068 6176 6520  ng..If you have 
+00001800: 7573 6564 2074 6869 7320 736f 6674 7761  used this softwa
+00001810: 7265 2069 6e20 6120 7363 6965 6e74 6966  re in a scientif
+00001820: 6963 2070 7562 6c69 6361 7469 6f6e 2c20  ic publication, 
+00001830: 706c 6561 7365 2063 6974 6520 6974 2075  please cite it u
+00001840: 7369 6e67 2074 6865 2066 6f6c 6c6f 7769  sing the followi
+00001850: 6e67 2042 6962 4c61 5465 5820 636f 6465  ng BibLaTeX code
+00001860: 3a0a 0a60 6060 0a40 736f 6674 7761 7265  :..```.@software
+00001870: 7b70 7964 6976 7375 6673 6f72 742c 0a20  {pydivsufsort,. 
+00001880: 2061 7574 686f 7220 2020 2020 2020 3d20   author       = 
+00001890: 7b4c 6f75 6973 2041 6272 6168 616d 7d2c  {Louis Abraham},
+000018a0: 0a20 2074 6974 6c65 2020 2020 2020 2020  .  title        
+000018b0: 3d20 7b70 7964 6976 7375 6673 6f72 747d  = {pydivsufsort}
+000018c0: 2c0a 2020 7965 6172 2020 2020 2020 2020  ,.  year        
+000018d0: 203d 2032 3032 332c 0a20 2070 7562 6c69   = 2023,.  publi
+000018e0: 7368 6572 2020 2020 3d20 7b5a 656e 6f64  sher    = {Zenod
+000018f0: 6f7d 2c0a 2020 646f 6920 2020 2020 2020  o},.  doi       
+00001900: 2020 203d 207b 3130 2e35 3238 312f 7a65     = {10.5281/ze
+00001910: 6e6f 646f 2e37 3933 3234 3538 7d2c 0a20  nodo.7932458},. 
+00001920: 2075 726c 2020 2020 2020 2020 2020 3d20   url          = 
+00001930: 7b68 7474 7073 3a2f 2f67 6974 6875 622e  {https://github.
+00001940: 636f 6d2f 6c6f 7569 7361 6272 6168 616d  com/louisabraham
+00001950: 2f70 7964 6976 7375 6673 6f72 747d 0a7d  /pydivsufsort}.}
+00001960: 0a60 6060                                .```
```

### Comparing `pydivsufsort-0.0.8/pydivsufsort.egg-info/SOURCES.txt` & `pydivsufsort-0.0.9/pydivsufsort.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydivsufsort-0.0.8/setup.py` & `pydivsufsort-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         language="c++",
         define_macros=[("CYTHON_TRACE", "1")] if PROFILE else None,
     )
 ]
 
 setup(
     name="pydivsufsort",
-    version="0.0.8",
+    version="0.0.9",
     author="Louis Abraham",
     license="MIT",
     author_email="louis.abraham@yahoo.fr",
     description="String algorithms",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     url="https://github.com/louisabraham/pydivsufsort",
```

### Comparing `pydivsufsort-0.0.8/tests/test_correct.py` & `pydivsufsort-0.0.9/tests/test_correct.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     sa = suffix_array(inp)
     assert (divsufsort(inp) == sa).all(), inp
 
     segtree = lcp_segtree(inp)
     if queries is None:
         n = len(inp)
         queries = [[0, 0], [0, n - 2], [0, n - 1], [n - 2, n - 2], [n - 1, n - 1]]
-    lcp_opt = lcp_query(*segtree, queries)
+    lcp_opt = lcp_query(segtree, queries)
     lcp_naive = [longest_common_prefix(inp, i, j) for i, j in queries]
     assert (lcp_opt == lcp_naive).all(), (inp, lcp_naive, lcp_opt)
 
     if not (isinstance(inp, np.ndarray) and inp.dtype != np.uint8):
         bwt_opt = bw_transform(inp)
         bwt_naive = BWT(inp)
         assert bwt_opt[0] == bwt_naive[0]
```

