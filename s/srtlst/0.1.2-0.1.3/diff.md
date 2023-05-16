# Comparing `tmp/srtlst-0.1.2.tar.gz` & `tmp/srtlst-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srtlst-0.1.2.tar", max compression
+gzip compressed data, was "srtlst-0.1.3.tar", max compression
```

## Comparing `srtlst-0.1.2.tar` & `srtlst-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0      586 2023-05-02 18:41:54.812574 srtlst-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2470 2023-05-02 13:10:13.468329 srtlst-0.1.2/readme.md
--rw-r--r--   0        0        0      155 2023-04-30 18:54:26.210904 srtlst-0.1.2/src/srtlst/__init__.py
--rw-r--r--   0        0        0      118 2023-05-02 13:30:41.414018 srtlst-0.1.2/src/srtlst/protocols.py
--rw-r--r--   0        0        0        0 2023-04-30 13:23:02.474724 srtlst-0.1.2/src/srtlst/py.typed
--rw-r--r--   0        0        0     7665 2023-05-02 18:40:35.615071 srtlst-0.1.2/src/srtlst/sorted_list.py
--rw-r--r--   0        0        0     1338 2023-05-02 17:19:59.579620 srtlst-0.1.2/src/srtlst/sorted_list_by_key.py
--rw-r--r--   0        0        0     2870 1970-01-01 00:00:00.000000 srtlst-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-07 18:30:37.563519 srtlst-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1073 2023-05-16 13:35:55.200320 srtlst-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2628 2023-05-07 18:30:37.564820 srtlst-0.1.3/readme.md
+-rw-r--r--   0        0        0      141 2023-05-16 13:33:41.633609 srtlst-0.1.3/src/srtlst/__init__.py
+-rw-r--r--   0        0        0      118 2023-05-07 18:30:37.565554 srtlst-0.1.3/src/srtlst/protocols.py
+-rw-r--r--   0        0        0        0 2023-05-07 18:30:37.565639 srtlst-0.1.3/src/srtlst/py.typed
+-rw-r--r--   0        0        0     7665 2023-05-16 13:34:08.254186 srtlst-0.1.3/src/srtlst/sorted_list.py
+-rw-r--r--   0        0        0     1338 2023-05-16 13:34:08.254697 srtlst-0.1.3/src/srtlst/sorted_list_by_key.py
+-rw-r--r--   0        0        0     3549 1970-01-01 00:00:00.000000 srtlst-0.1.3/PKG-INFO
```

### Comparing `srtlst-0.1.2/readme.md` & `srtlst-0.1.3/readme.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # srtlst
 
-_a simple, generically typed-hinted, sorted list_
+_a simple, generically type-annotated, sorted list_
+
+![python_version](https://img.shields.io/pypi/pyversions/srtlst)
+[![mypy_checked](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
 
 ### usage
 
 Create a sorted list like this:
 
 ```python
 >>> from srtlst import SortedList
@@ -39,15 +42,15 @@
 >>> from srtlst import SortedListByKey
 >>> my_function = lambda x: x * (-1) ** x
 >>> s = SortedListByKey([1, 2, 3, 4], key=my_function)
 >>> print(s)
 [3, 1, 2, 4]
 ```
 
-`SortedListByKey` behaves like a `SortedList` in all other ways, and indeed, inherits from it.
+`SortedListByKey` behaves like a `SortedList` in all other ways, and indeed inherits from it.
 However, when type checking, a `SortedList` only accepts values for which a less-than (`<`) method is defined (`__lt__()`).
 
 `SortedListByKey` accepts any type of object, as long as an appropriate key function is provided.
 The key function must return comparable values for the items in the list.
 
 ### installation
 
@@ -66,15 +69,15 @@
 
 ```python
 s: SortedList[int] = SortedList([3, 2, 1])
 ```
 
 ### performance
 
-This library aims to provide a simple sorted list without any dependencies, that is ready for use.
+This library aims to provide a simple sorted list without any dependencies which is ready for use.
 Some of the list operations are reimplemented to take advantage of the list's sortedness using Python's standard `bisect` library.
 
 This library should suit your needs if you just want to keep stuff sorted, without having to implement the bookkeeping yourself.
 However, if your sorting needs arise from the need for performance, you should also consider this library:
 [sortedcontainers](https://grantjenks.com/docs/sortedcontainers/).  
 
 ### documentation
```

### Comparing `srtlst-0.1.2/src/srtlst/sorted_list.py` & `srtlst-0.1.3/src/srtlst/sorted_list.py`

 * *Files identical despite different names*

### Comparing `srtlst-0.1.2/src/srtlst/sorted_list_by_key.py` & `srtlst-0.1.3/src/srtlst/sorted_list_by_key.py`

 * *Files identical despite different names*

