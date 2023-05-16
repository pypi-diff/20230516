# Comparing `tmp/fasttextsearch-0.1.tar.gz` & `tmp/fasttextsearch-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/ceph-kw/kangwei/code/text_search/dist/.tmp-_s7hseij/fasttextsearch-0.1.tar", last modified: Tue May 16 09:22:27 2023, max compression
+gzip compressed data, was "/ceph-kw/kangwei/code/text_search/dist/.tmp-jhwwqh34/fasttextsearch-0.2.tar", last modified: Tue May 16 09:39:01 2023, max compression
```

## Comparing `fasttextsearch-0.1.tar` & `fasttextsearch-0.2.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-05-16 09:22:27.412606 fasttextsearch-0.1/
--rw-r--r--   0 kangwei   (1092) root         (0)     2277 2023-05-16 08:11:03.000000 fasttextsearch-0.1/CMakeLists.txt
--rw-r--r--   0 kangwei   (1092) root         (0)      143 2023-05-16 08:44:49.000000 fasttextsearch-0.1/MANIFEST.in
--rw-r--r--   0 kangwei   (1092) root         (0)     1199 2023-05-16 09:22:27.411606 fasttextsearch-0.1/PKG-INFO
--rw-r--r--   0 kangwei   (1092) root         (0)      593 2023-04-24 12:23:40.000000 fasttextsearch-0.1/README.md
-drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-05-16 09:22:27.359606 fasttextsearch-0.1/cmake/
-drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-05-16 09:22:27.361606 fasttextsearch-0.1/cmake/Modules/
-drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-05-16 09:22:27.362606 fasttextsearch-0.1/cmake/Modules/FetchContent/
--rw-r--r--   0 kangwei   (1092) root         (0)      831 2023-02-18 07:20:27.000000 fasttextsearch-0.1/cmake/Modules/FetchContent/CMakeLists.cmake.in
--rw-r--r--   0 kangwei   (1092) root         (0)    38023 2023-02-18 07:20:27.000000 fasttextsearch-0.1/cmake/Modules/FetchContent.cmake
--rw-r--r--   0 kangwei   (1092) root         (0)      135 2023-02-18 07:20:27.000000 fasttextsearch-0.1/cmake/Modules/README.md
--rw-r--r--   0 kangwei   (1092) root         (0)        0 2023-02-18 07:20:27.000000 fasttextsearch-0.1/cmake/__init__.py
--rw-r--r--   0 kangwei   (1092) root         (0)     3421 2023-03-31 03:33:51.000000 fasttextsearch-0.1/cmake/googletest.cmake
--rw-r--r--   0 kangwei   (1092) root         (0)     1800 2023-03-31 03:33:51.000000 fasttextsearch-0.1/cmake/pybind11.cmake
-drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-05-16 09:22:27.366606 fasttextsearch-0.1/fasttextsearch.egg-info/
--rw-r--r--   0 kangwei   (1092) root         (0)     1199 2023-05-16 09:22:27.000000 fasttextsearch-0.1/fasttextsearch.egg-info/PKG-INFO
--rw-r--r--   0 kangwei   (1092) root         (0)     2357 2023-05-16 09:22:27.000000 fasttextsearch-0.1/fasttextsearch.egg-info/SOURCES.txt
--rw-r--r--   0 kangwei   (1092) root         (0)        1 2023-05-16 09:22:27.000000 fasttextsearch-0.1/fasttextsearch.egg-info/dependency_links.txt
--rw-r--r--   0 kangwei   (1092) root         (0)        6 2023-05-16 09:22:27.000000 fasttextsearch-0.1/fasttextsearch.egg-info/requires.txt
--rw-r--r--   0 kangwei   (1092) root         (0)       24 2023-05-16 09:22:27.000000 fasttextsearch-0.1/fasttextsearch.egg-info/top_level.txt
--rw-r--r--   0 kangwei   (1092) root         (0)      827 2023-05-16 09:22:11.000000 fasttextsearch-0.1/pyproject.toml
--rw-r--r--   0 kangwei   (1092) root         (0)        6 2023-05-16 07:33:05.000000 fasttextsearch-0.1/requirements.txt
--rw-r--r--   0 kangwei   (1092) root         (0)       38 2023-05-16 09:22:27.412606 fasttextsearch-0.1/setup.cfg
--rw-r--r--   0 kangwei   (1092) root         (0)     2901 2023-05-16 09:05:31.000000 fasttextsearch-0.1/setup.py
-drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-05-16 09:22:27.367606 fasttextsearch-0.1/textsearch/
--rw-r--r--   0 kangwei   (1092) root         (0)       48 2023-02-18 12:05:47.000000 fasttextsearch-0.1/textsearch/CMakeLists.txt
-drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-05-16 09:22:27.378606 fasttextsearch-0.1/textsearch/csrc/
--rw-r--r--   0 kangwei   (1092) root         (0)      695 2023-05-16 07:24:32.000000 fasttextsearch-0.1/textsearch/csrc/CMakeLists.txt
--rw-r--r--   0 kangwei   (1092) root         (0)    13272 2023-05-04 04:46:37.000000 fasttextsearch-0.1/textsearch/csrc/levenshtein.h
--rw-r--r--   0 kangwei   (1092) root         (0)     4137 2023-05-04 04:46:37.000000 fasttextsearch-0.1/textsearch/csrc/levenshtein_test.cc
--rw-r--r--   0 kangwei   (1092) root         (0)     4664 2023-05-04 04:46:37.000000 fasttextsearch-0.1/textsearch/csrc/match.cc
--rw-r--r--   0 kangwei   (1092) root         (0)     4611 2023-05-04 04:46:37.000000 fasttextsearch-0.1/textsearch/csrc/match.h
--rw-r--r--   0 kangwei   (1092) root         (0)     3248 2023-05-04 04:46:37.000000 fasttextsearch-0.1/textsearch/csrc/match_test.cc
--rw-r--r--   0 kangwei   (1092) root         (0)     5273 2023-04-12 07:57:56.000000 fasttextsearch-0.1/textsearch/csrc/suffix_array.cc
--rw-r--r--   0 kangwei   (1092) root         (0)     3207 2023-03-31 03:33:51.000000 fasttextsearch-0.1/textsearch/csrc/suffix_array.h
--rw-r--r--   0 kangwei   (1092) root         (0)     3883 2023-04-24 11:25:03.000000 fasttextsearch-0.1/textsearch/csrc/suffix_array_test.cc
--rw-r--r--   0 kangwei   (1092) root         (0)     2880 2023-04-24 11:25:03.000000 fasttextsearch-0.1/textsearch/csrc/utils.cc
--rw-r--r--   0 kangwei   (1092) root         (0)     3508 2023-04-24 11:25:03.000000 fasttextsearch-0.1/textsearch/csrc/utils.h
--rw-r--r--   0 kangwei   (1092) root         (0)     4862 2023-04-24 11:25:03.000000 fasttextsearch-0.1/textsearch/csrc/utils_test.cc
-drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-05-16 09:22:27.379606 fasttextsearch-0.1/textsearch/python/
--rw-r--r--   0 kangwei   (1092) root         (0)       78 2023-05-16 07:26:44.000000 fasttextsearch-0.1/textsearch/python/CMakeLists.txt
-drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-05-16 09:22:27.389606 fasttextsearch-0.1/textsearch/python/csrc/
--rw-r--r--   0 kangwei   (1092) root         (0)      169 2023-05-16 07:25:08.000000 fasttextsearch-0.1/textsearch/python/csrc/CMakeLists.txt
--rw-r--r--   0 kangwei   (1092) root         (0)     4925 2023-05-04 04:46:37.000000 fasttextsearch-0.1/textsearch/python/csrc/levenshtein.cc
--rw-r--r--   0 kangwei   (1092) root         (0)      985 2023-03-06 09:09:29.000000 fasttextsearch-0.1/textsearch/python/csrc/levenshtein.h
--rw-r--r--   0 kangwei   (1092) root         (0)     1850 2023-05-04 04:46:37.000000 fasttextsearch-0.1/textsearch/python/csrc/match.cc
--rw-r--r--   0 kangwei   (1092) root         (0)      961 2023-05-04 04:46:37.000000 fasttextsearch-0.1/textsearch/python/csrc/match.h
--rw-r--r--   0 kangwei   (1092) root         (0)     1637 2023-04-13 03:32:42.000000 fasttextsearch-0.1/textsearch/python/csrc/suffix_array.cc
--rw-r--r--   0 kangwei   (1092) root         (0)      988 2023-03-06 09:09:29.000000 fasttextsearch-0.1/textsearch/python/csrc/suffix_array.h
--rw-r--r--   0 kangwei   (1092) root         (0)      568 2023-05-04 04:46:37.000000 fasttextsearch-0.1/textsearch/python/csrc/text_search.cc
--rw-r--r--   0 kangwei   (1092) root         (0)      357 2023-03-31 03:33:51.000000 fasttextsearch-0.1/textsearch/python/csrc/text_search.h
--rw-r--r--   0 kangwei   (1092) root         (0)     4599 2023-04-24 11:25:03.000000 fasttextsearch-0.1/textsearch/python/csrc/utils.cc
--rw-r--r--   0 kangwei   (1092) root         (0)      318 2023-04-21 06:51:44.000000 fasttextsearch-0.1/textsearch/python/csrc/utils.h
-drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-05-16 09:22:27.398606 fasttextsearch-0.1/textsearch/python/tests/
--rw-r--r--   0 kangwei   (1092) root         (0)      853 2023-05-04 04:46:37.000000 fasttextsearch-0.1/textsearch/python/tests/CMakeLists.txt
--rwxr-xr-x   0 kangwei   (1092) root         (0)     4748 2023-04-24 11:25:03.000000 fasttextsearch-0.1/textsearch/python/tests/test_find_close_matches.py
--rwxr-xr-x   0 kangwei   (1092) root         (0)     1943 2023-04-13 03:32:42.000000 fasttextsearch-0.1/textsearch/python/tests/test_levenshtein_distance.py
--rwxr-xr-x   0 kangwei   (1092) root         (0)     1414 2023-05-04 04:46:37.000000 fasttextsearch-0.1/textsearch/python/tests/test_match.py
--rwxr-xr-x   0 kangwei   (1092) root         (0)      950 2023-03-31 03:33:51.000000 fasttextsearch-0.1/textsearch/python/tests/test_row_ids_to_row_splits.py
--rwxr-xr-x   0 kangwei   (1092) root         (0)    10687 2023-04-13 03:32:42.000000 fasttextsearch-0.1/textsearch/python/tests/test_sourced_text.py
--rwxr-xr-x   0 kangwei   (1092) root         (0)     1359 2023-04-24 11:25:03.000000 fasttextsearch-0.1/textsearch/python/tests/test_suffix_array.py
--rwxr-xr-x   0 kangwei   (1092) root         (0)     2007 2023-03-31 03:33:51.000000 fasttextsearch-0.1/textsearch/python/tests/test_text_source.py
--rwxr-xr-x   0 kangwei   (1092) root         (0)     2314 2023-03-31 03:33:51.000000 fasttextsearch-0.1/textsearch/python/tests/test_transcript.py
-drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-05-16 09:22:27.403607 fasttextsearch-0.1/textsearch/python/textsearch/
--rw-r--r--   0 kangwei   (1092) root         (0)     1611 2023-05-16 09:22:27.000000 fasttextsearch-0.1/textsearch/python/textsearch/__init__.py
-drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-05-16 09:22:27.410606 fasttextsearch-0.1/textsearch/python/textsearch/__pycache__/
--rw-r--r--   0 kangwei   (1092) root         (0)      948 2023-05-05 09:46:59.000000 fasttextsearch-0.1/textsearch/python/textsearch/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 kangwei   (1092) root         (0)     8961 2023-05-05 09:46:59.000000 fasttextsearch-0.1/textsearch/python/textsearch/__pycache__/datatypes.cpython-38.pyc
--rw-r--r--   0 kangwei   (1092) root         (0)     2543 2023-05-05 09:46:59.000000 fasttextsearch-0.1/textsearch/python/textsearch/__pycache__/levenshtein.cpython-38.pyc
--rw-r--r--   0 kangwei   (1092) root         (0)    23034 2023-05-06 08:03:54.000000 fasttextsearch-0.1/textsearch/python/textsearch/__pycache__/match.cpython-38.pyc
--rw-r--r--   0 kangwei   (1092) root         (0)     5139 2023-05-05 09:47:40.000000 fasttextsearch-0.1/textsearch/python/textsearch/__pycache__/suffix_array.cpython-38.pyc
--rw-r--r--   0 kangwei   (1092) root         (0)     2910 2023-04-13 07:06:10.000000 fasttextsearch-0.1/textsearch/python/textsearch/__pycache__/text_search.cpython-38.pyc
--rw-r--r--   0 kangwei   (1092) root         (0)     3328 2023-05-05 09:46:59.000000 fasttextsearch-0.1/textsearch/python/textsearch/__pycache__/utils.cpython-38.pyc
--rw-r--r--   0 kangwei   (1092) root         (0)    12992 2023-04-24 11:25:03.000000 fasttextsearch-0.1/textsearch/python/textsearch/datatypes.py
--rw-r--r--   0 kangwei   (1092) root         (0)     3594 2023-04-24 11:25:03.000000 fasttextsearch-0.1/textsearch/python/textsearch/levenshtein.py
--rw-r--r--   0 kangwei   (1092) root         (0)    39883 2023-05-16 07:26:01.000000 fasttextsearch-0.1/textsearch/python/textsearch/match.py
--rw-r--r--   0 kangwei   (1092) root         (0)     6695 2023-05-16 07:26:33.000000 fasttextsearch-0.1/textsearch/python/textsearch/suffix_array.py
--rw-r--r--   0 kangwei   (1092) root         (0)     3165 2023-05-16 07:26:31.000000 fasttextsearch-0.1/textsearch/python/textsearch/utils.py
+drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-05-16 09:39:01.030509 fasttextsearch-0.2/
+-rw-r--r--   0 kangwei   (1092) root         (0)     2277 2023-05-16 08:11:03.000000 fasttextsearch-0.2/CMakeLists.txt
+-rw-r--r--   0 kangwei   (1092) root         (0)      143 2023-05-16 08:44:49.000000 fasttextsearch-0.2/MANIFEST.in
+-rw-r--r--   0 kangwei   (1092) root         (0)     1199 2023-05-16 09:39:01.029509 fasttextsearch-0.2/PKG-INFO
+-rw-r--r--   0 kangwei   (1092) root         (0)      593 2023-04-24 12:23:40.000000 fasttextsearch-0.2/README.md
+drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-05-16 09:39:00.977509 fasttextsearch-0.2/cmake/
+drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-05-16 09:39:00.979509 fasttextsearch-0.2/cmake/Modules/
+drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-05-16 09:39:00.980509 fasttextsearch-0.2/cmake/Modules/FetchContent/
+-rw-r--r--   0 kangwei   (1092) root         (0)      831 2023-02-18 07:20:27.000000 fasttextsearch-0.2/cmake/Modules/FetchContent/CMakeLists.cmake.in
+-rw-r--r--   0 kangwei   (1092) root         (0)    38023 2023-02-18 07:20:27.000000 fasttextsearch-0.2/cmake/Modules/FetchContent.cmake
+-rw-r--r--   0 kangwei   (1092) root         (0)      135 2023-02-18 07:20:27.000000 fasttextsearch-0.2/cmake/Modules/README.md
+-rw-r--r--   0 kangwei   (1092) root         (0)        0 2023-02-18 07:20:27.000000 fasttextsearch-0.2/cmake/__init__.py
+-rw-r--r--   0 kangwei   (1092) root         (0)     3421 2023-03-31 03:33:51.000000 fasttextsearch-0.2/cmake/googletest.cmake
+-rw-r--r--   0 kangwei   (1092) root         (0)     1800 2023-03-31 03:33:51.000000 fasttextsearch-0.2/cmake/pybind11.cmake
+drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-05-16 09:39:00.986509 fasttextsearch-0.2/fasttextsearch.egg-info/
+-rw-r--r--   0 kangwei   (1092) root         (0)     1199 2023-05-16 09:39:00.000000 fasttextsearch-0.2/fasttextsearch.egg-info/PKG-INFO
+-rw-r--r--   0 kangwei   (1092) root         (0)     2357 2023-05-16 09:39:00.000000 fasttextsearch-0.2/fasttextsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 kangwei   (1092) root         (0)        1 2023-05-16 09:39:00.000000 fasttextsearch-0.2/fasttextsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 kangwei   (1092) root         (0)        6 2023-05-16 09:39:00.000000 fasttextsearch-0.2/fasttextsearch.egg-info/requires.txt
+-rw-r--r--   0 kangwei   (1092) root         (0)       24 2023-05-16 09:39:00.000000 fasttextsearch-0.2/fasttextsearch.egg-info/top_level.txt
+-rw-r--r--   0 kangwei   (1092) root         (0)      845 2023-05-16 09:38:50.000000 fasttextsearch-0.2/pyproject.toml
+-rw-r--r--   0 kangwei   (1092) root         (0)        6 2023-05-16 07:33:05.000000 fasttextsearch-0.2/requirements.txt
+-rw-r--r--   0 kangwei   (1092) root         (0)       38 2023-05-16 09:39:01.030509 fasttextsearch-0.2/setup.cfg
+-rw-r--r--   0 kangwei   (1092) root         (0)     2901 2023-05-16 09:05:31.000000 fasttextsearch-0.2/setup.py
+drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-05-16 09:39:00.987509 fasttextsearch-0.2/textsearch/
+-rw-r--r--   0 kangwei   (1092) root         (0)       48 2023-02-18 12:05:47.000000 fasttextsearch-0.2/textsearch/CMakeLists.txt
+drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-05-16 09:39:00.998509 fasttextsearch-0.2/textsearch/csrc/
+-rw-r--r--   0 kangwei   (1092) root         (0)      695 2023-05-16 07:24:32.000000 fasttextsearch-0.2/textsearch/csrc/CMakeLists.txt
+-rw-r--r--   0 kangwei   (1092) root         (0)    13272 2023-05-04 04:46:37.000000 fasttextsearch-0.2/textsearch/csrc/levenshtein.h
+-rw-r--r--   0 kangwei   (1092) root         (0)     4137 2023-05-04 04:46:37.000000 fasttextsearch-0.2/textsearch/csrc/levenshtein_test.cc
+-rw-r--r--   0 kangwei   (1092) root         (0)     4664 2023-05-04 04:46:37.000000 fasttextsearch-0.2/textsearch/csrc/match.cc
+-rw-r--r--   0 kangwei   (1092) root         (0)     4611 2023-05-04 04:46:37.000000 fasttextsearch-0.2/textsearch/csrc/match.h
+-rw-r--r--   0 kangwei   (1092) root         (0)     3248 2023-05-04 04:46:37.000000 fasttextsearch-0.2/textsearch/csrc/match_test.cc
+-rw-r--r--   0 kangwei   (1092) root         (0)     5273 2023-04-12 07:57:56.000000 fasttextsearch-0.2/textsearch/csrc/suffix_array.cc
+-rw-r--r--   0 kangwei   (1092) root         (0)     3207 2023-03-31 03:33:51.000000 fasttextsearch-0.2/textsearch/csrc/suffix_array.h
+-rw-r--r--   0 kangwei   (1092) root         (0)     3883 2023-04-24 11:25:03.000000 fasttextsearch-0.2/textsearch/csrc/suffix_array_test.cc
+-rw-r--r--   0 kangwei   (1092) root         (0)     2880 2023-04-24 11:25:03.000000 fasttextsearch-0.2/textsearch/csrc/utils.cc
+-rw-r--r--   0 kangwei   (1092) root         (0)     3508 2023-04-24 11:25:03.000000 fasttextsearch-0.2/textsearch/csrc/utils.h
+-rw-r--r--   0 kangwei   (1092) root         (0)     4862 2023-04-24 11:25:03.000000 fasttextsearch-0.2/textsearch/csrc/utils_test.cc
+drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-05-16 09:39:00.998509 fasttextsearch-0.2/textsearch/python/
+-rw-r--r--   0 kangwei   (1092) root         (0)       78 2023-05-16 07:26:44.000000 fasttextsearch-0.2/textsearch/python/CMakeLists.txt
+drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-05-16 09:39:01.008509 fasttextsearch-0.2/textsearch/python/csrc/
+-rw-r--r--   0 kangwei   (1092) root         (0)      169 2023-05-16 07:25:08.000000 fasttextsearch-0.2/textsearch/python/csrc/CMakeLists.txt
+-rw-r--r--   0 kangwei   (1092) root         (0)     4925 2023-05-04 04:46:37.000000 fasttextsearch-0.2/textsearch/python/csrc/levenshtein.cc
+-rw-r--r--   0 kangwei   (1092) root         (0)      985 2023-03-06 09:09:29.000000 fasttextsearch-0.2/textsearch/python/csrc/levenshtein.h
+-rw-r--r--   0 kangwei   (1092) root         (0)     1850 2023-05-04 04:46:37.000000 fasttextsearch-0.2/textsearch/python/csrc/match.cc
+-rw-r--r--   0 kangwei   (1092) root         (0)      961 2023-05-04 04:46:37.000000 fasttextsearch-0.2/textsearch/python/csrc/match.h
+-rw-r--r--   0 kangwei   (1092) root         (0)     1637 2023-04-13 03:32:42.000000 fasttextsearch-0.2/textsearch/python/csrc/suffix_array.cc
+-rw-r--r--   0 kangwei   (1092) root         (0)      988 2023-03-06 09:09:29.000000 fasttextsearch-0.2/textsearch/python/csrc/suffix_array.h
+-rw-r--r--   0 kangwei   (1092) root         (0)      568 2023-05-04 04:46:37.000000 fasttextsearch-0.2/textsearch/python/csrc/text_search.cc
+-rw-r--r--   0 kangwei   (1092) root         (0)      357 2023-03-31 03:33:51.000000 fasttextsearch-0.2/textsearch/python/csrc/text_search.h
+-rw-r--r--   0 kangwei   (1092) root         (0)     4599 2023-04-24 11:25:03.000000 fasttextsearch-0.2/textsearch/python/csrc/utils.cc
+-rw-r--r--   0 kangwei   (1092) root         (0)      318 2023-04-21 06:51:44.000000 fasttextsearch-0.2/textsearch/python/csrc/utils.h
+drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-05-16 09:39:01.016509 fasttextsearch-0.2/textsearch/python/tests/
+-rw-r--r--   0 kangwei   (1092) root         (0)      853 2023-05-04 04:46:37.000000 fasttextsearch-0.2/textsearch/python/tests/CMakeLists.txt
+-rwxr-xr-x   0 kangwei   (1092) root         (0)     4748 2023-04-24 11:25:03.000000 fasttextsearch-0.2/textsearch/python/tests/test_find_close_matches.py
+-rwxr-xr-x   0 kangwei   (1092) root         (0)     1943 2023-04-13 03:32:42.000000 fasttextsearch-0.2/textsearch/python/tests/test_levenshtein_distance.py
+-rwxr-xr-x   0 kangwei   (1092) root         (0)     1414 2023-05-04 04:46:37.000000 fasttextsearch-0.2/textsearch/python/tests/test_match.py
+-rwxr-xr-x   0 kangwei   (1092) root         (0)      950 2023-03-31 03:33:51.000000 fasttextsearch-0.2/textsearch/python/tests/test_row_ids_to_row_splits.py
+-rwxr-xr-x   0 kangwei   (1092) root         (0)    10687 2023-04-13 03:32:42.000000 fasttextsearch-0.2/textsearch/python/tests/test_sourced_text.py
+-rwxr-xr-x   0 kangwei   (1092) root         (0)     1359 2023-04-24 11:25:03.000000 fasttextsearch-0.2/textsearch/python/tests/test_suffix_array.py
+-rwxr-xr-x   0 kangwei   (1092) root         (0)     2007 2023-03-31 03:33:51.000000 fasttextsearch-0.2/textsearch/python/tests/test_text_source.py
+-rwxr-xr-x   0 kangwei   (1092) root         (0)     2314 2023-03-31 03:33:51.000000 fasttextsearch-0.2/textsearch/python/tests/test_transcript.py
+drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-05-16 09:39:01.022509 fasttextsearch-0.2/textsearch/python/textsearch/
+-rw-r--r--   0 kangwei   (1092) root         (0)     1691 2023-05-16 09:39:00.000000 fasttextsearch-0.2/textsearch/python/textsearch/__init__.py
+drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-05-16 09:39:01.028509 fasttextsearch-0.2/textsearch/python/textsearch/__pycache__/
+-rw-r--r--   0 kangwei   (1092) root         (0)      948 2023-05-05 09:46:59.000000 fasttextsearch-0.2/textsearch/python/textsearch/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 kangwei   (1092) root         (0)     8961 2023-05-05 09:46:59.000000 fasttextsearch-0.2/textsearch/python/textsearch/__pycache__/datatypes.cpython-38.pyc
+-rw-r--r--   0 kangwei   (1092) root         (0)     2543 2023-05-05 09:46:59.000000 fasttextsearch-0.2/textsearch/python/textsearch/__pycache__/levenshtein.cpython-38.pyc
+-rw-r--r--   0 kangwei   (1092) root         (0)    23034 2023-05-06 08:03:54.000000 fasttextsearch-0.2/textsearch/python/textsearch/__pycache__/match.cpython-38.pyc
+-rw-r--r--   0 kangwei   (1092) root         (0)     5139 2023-05-05 09:47:40.000000 fasttextsearch-0.2/textsearch/python/textsearch/__pycache__/suffix_array.cpython-38.pyc
+-rw-r--r--   0 kangwei   (1092) root         (0)     2910 2023-04-13 07:06:10.000000 fasttextsearch-0.2/textsearch/python/textsearch/__pycache__/text_search.cpython-38.pyc
+-rw-r--r--   0 kangwei   (1092) root         (0)     3328 2023-05-05 09:46:59.000000 fasttextsearch-0.2/textsearch/python/textsearch/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0 kangwei   (1092) root         (0)    12992 2023-04-24 11:25:03.000000 fasttextsearch-0.2/textsearch/python/textsearch/datatypes.py
+-rw-r--r--   0 kangwei   (1092) root         (0)     3594 2023-04-24 11:25:03.000000 fasttextsearch-0.2/textsearch/python/textsearch/levenshtein.py
+-rw-r--r--   0 kangwei   (1092) root         (0)    39883 2023-05-16 07:26:01.000000 fasttextsearch-0.2/textsearch/python/textsearch/match.py
+-rw-r--r--   0 kangwei   (1092) root         (0)     6695 2023-05-16 07:26:33.000000 fasttextsearch-0.2/textsearch/python/textsearch/suffix_array.py
+-rw-r--r--   0 kangwei   (1092) root         (0)     3165 2023-05-16 07:26:31.000000 fasttextsearch-0.2/textsearch/python/textsearch/utils.py
```

### Comparing `fasttextsearch-0.1/CMakeLists.txt` & `fasttextsearch-0.2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/PKG-INFO` & `fasttextsearch-0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: fasttextsearch
-Version: 0.1
+Version: 0.2
 Summary: Some fast-ish algorithms for batch text search in moderate-sized collections, intended for data cleanup.
 Author-email: Next-gen Kaldi development team <wkang.pku@gmail.com>
-Project-URL: Homepage, https://github.com/k2-fsa/text-search
-Project-URL: Bug Tracker, https://github.com/k2-fsa/text-search/issues
+Project-URL: Homepage, https://github.com/k2-fsa/text_search
+Project-URL: Bug Tracker, https://github.com/k2-fsa/text_search/issues
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `fasttextsearch-0.1/README.md` & `fasttextsearch-0.2/README.md`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/cmake/Modules/FetchContent/CMakeLists.cmake.in` & `fasttextsearch-0.2/cmake/Modules/FetchContent/CMakeLists.cmake.in`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/cmake/Modules/FetchContent.cmake` & `fasttextsearch-0.2/cmake/Modules/FetchContent.cmake`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/cmake/googletest.cmake` & `fasttextsearch-0.2/cmake/googletest.cmake`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/cmake/pybind11.cmake` & `fasttextsearch-0.2/cmake/pybind11.cmake`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/fasttextsearch.egg-info/PKG-INFO` & `fasttextsearch-0.2/fasttextsearch.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: fasttextsearch
-Version: 0.1
+Version: 0.2
 Summary: Some fast-ish algorithms for batch text search in moderate-sized collections, intended for data cleanup.
 Author-email: Next-gen Kaldi development team <wkang.pku@gmail.com>
-Project-URL: Homepage, https://github.com/k2-fsa/text-search
-Project-URL: Bug Tracker, https://github.com/k2-fsa/text-search/issues
+Project-URL: Homepage, https://github.com/k2-fsa/text_search
+Project-URL: Bug Tracker, https://github.com/k2-fsa/text_search/issues
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `fasttextsearch-0.1/fasttextsearch.egg-info/SOURCES.txt` & `fasttextsearch-0.2/fasttextsearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/pyproject.toml` & `fasttextsearch-0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "cmake>=3.8",
 ]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "fasttextsearch"
-version = "0.1"
+version = "0.2"
 authors = [
   { name="Next-gen Kaldi development team", email="wkang.pku@gmail.com" },
 ]
 description="Some fast-ish algorithms for batch text search in moderate-sized collections, intended for data cleanup."
 dependencies = [
   "numpy",
 ]
@@ -23,15 +23,15 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 
 [tool.setuptools.packages.find]
-include = ['textsearch']
+include = ['textsearch.python.textsearch']
 
 [project.urls]
-"Homepage" = "https://github.com/k2-fsa/text-search"
-"Bug Tracker" = "https://github.com/k2-fsa/text-search/issues"
+"Homepage" = "https://github.com/k2-fsa/text_search"
+"Bug Tracker" = "https://github.com/k2-fsa/text_search/issues"
```

### Comparing `fasttextsearch-0.1/setup.py` & `fasttextsearch-0.2/setup.py`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/textsearch/csrc/CMakeLists.txt` & `fasttextsearch-0.2/textsearch/csrc/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/textsearch/csrc/levenshtein.h` & `fasttextsearch-0.2/textsearch/csrc/levenshtein.h`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/textsearch/csrc/levenshtein_test.cc` & `fasttextsearch-0.2/textsearch/csrc/levenshtein_test.cc`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/textsearch/csrc/match.cc` & `fasttextsearch-0.2/textsearch/csrc/match.cc`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/textsearch/csrc/match.h` & `fasttextsearch-0.2/textsearch/csrc/match.h`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/textsearch/csrc/match_test.cc` & `fasttextsearch-0.2/textsearch/csrc/match_test.cc`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/textsearch/csrc/suffix_array.cc` & `fasttextsearch-0.2/textsearch/csrc/suffix_array.cc`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/textsearch/csrc/suffix_array.h` & `fasttextsearch-0.2/textsearch/csrc/suffix_array.h`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/textsearch/csrc/suffix_array_test.cc` & `fasttextsearch-0.2/textsearch/csrc/suffix_array_test.cc`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/textsearch/csrc/utils.cc` & `fasttextsearch-0.2/textsearch/csrc/utils.cc`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/textsearch/csrc/utils.h` & `fasttextsearch-0.2/textsearch/csrc/utils.h`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/textsearch/csrc/utils_test.cc` & `fasttextsearch-0.2/textsearch/csrc/utils_test.cc`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/textsearch/python/csrc/levenshtein.cc` & `fasttextsearch-0.2/textsearch/python/csrc/levenshtein.cc`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/textsearch/python/csrc/levenshtein.h` & `fasttextsearch-0.2/textsearch/python/csrc/levenshtein.h`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/textsearch/python/csrc/match.cc` & `fasttextsearch-0.2/textsearch/python/csrc/match.cc`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/textsearch/python/csrc/match.h` & `fasttextsearch-0.2/textsearch/python/csrc/match.h`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/textsearch/python/csrc/suffix_array.cc` & `fasttextsearch-0.2/textsearch/python/csrc/suffix_array.cc`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/textsearch/python/csrc/suffix_array.h` & `fasttextsearch-0.2/textsearch/python/csrc/suffix_array.h`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/textsearch/python/csrc/text_search.cc` & `fasttextsearch-0.2/textsearch/python/csrc/text_search.cc`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/textsearch/python/csrc/utils.cc` & `fasttextsearch-0.2/textsearch/python/csrc/utils.cc`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/textsearch/python/tests/CMakeLists.txt` & `fasttextsearch-0.2/textsearch/python/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/textsearch/python/tests/test_find_close_matches.py` & `fasttextsearch-0.2/textsearch/python/tests/test_find_close_matches.py`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/textsearch/python/tests/test_levenshtein_distance.py` & `fasttextsearch-0.2/textsearch/python/tests/test_levenshtein_distance.py`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/textsearch/python/tests/test_match.py` & `fasttextsearch-0.2/textsearch/python/tests/test_match.py`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/textsearch/python/tests/test_row_ids_to_row_splits.py` & `fasttextsearch-0.2/textsearch/python/tests/test_row_ids_to_row_splits.py`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/textsearch/python/tests/test_sourced_text.py` & `fasttextsearch-0.2/textsearch/python/tests/test_sourced_text.py`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/textsearch/python/tests/test_suffix_array.py` & `fasttextsearch-0.2/textsearch/python/tests/test_suffix_array.py`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/textsearch/python/tests/test_text_source.py` & `fasttextsearch-0.2/textsearch/python/tests/test_text_source.py`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/textsearch/python/tests/test_transcript.py` & `fasttextsearch-0.2/textsearch/python/tests/test_transcript.py`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/textsearch/python/textsearch/__init__.py` & `fasttextsearch-0.2/textsearch/python/textsearch/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -62,7 +62,11 @@
 __version__ = '0.1'
 __version__ = '0.1'
 __version__ = '0.1'
 __version__ = '0.1'
 __version__ = '0.1'
 __version__ = '0.1'
 __version__ = '0.1'
+__version__ = '0.1'
+__version__ = '0.1'
+__version__ = '0.1'
+__version__ = '0.1'
```

### Comparing `fasttextsearch-0.1/textsearch/python/textsearch/__pycache__/__init__.cpython-38.pyc` & `fasttextsearch-0.2/textsearch/python/textsearch/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/textsearch/python/textsearch/__pycache__/datatypes.cpython-38.pyc` & `fasttextsearch-0.2/textsearch/python/textsearch/__pycache__/datatypes.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/textsearch/python/textsearch/__pycache__/levenshtein.cpython-38.pyc` & `fasttextsearch-0.2/textsearch/python/textsearch/__pycache__/levenshtein.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/textsearch/python/textsearch/__pycache__/match.cpython-38.pyc` & `fasttextsearch-0.2/textsearch/python/textsearch/__pycache__/match.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/textsearch/python/textsearch/__pycache__/suffix_array.cpython-38.pyc` & `fasttextsearch-0.2/textsearch/python/textsearch/__pycache__/suffix_array.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/textsearch/python/textsearch/__pycache__/text_search.cpython-38.pyc` & `fasttextsearch-0.2/textsearch/python/textsearch/__pycache__/text_search.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/textsearch/python/textsearch/__pycache__/utils.cpython-38.pyc` & `fasttextsearch-0.2/textsearch/python/textsearch/__pycache__/utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/textsearch/python/textsearch/datatypes.py` & `fasttextsearch-0.2/textsearch/python/textsearch/datatypes.py`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/textsearch/python/textsearch/levenshtein.py` & `fasttextsearch-0.2/textsearch/python/textsearch/levenshtein.py`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/textsearch/python/textsearch/match.py` & `fasttextsearch-0.2/textsearch/python/textsearch/match.py`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/textsearch/python/textsearch/suffix_array.py` & `fasttextsearch-0.2/textsearch/python/textsearch/suffix_array.py`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.1/textsearch/python/textsearch/utils.py` & `fasttextsearch-0.2/textsearch/python/textsearch/utils.py`

 * *Files identical despite different names*

