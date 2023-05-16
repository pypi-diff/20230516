# Comparing `tmp/pyfsdb-2.1.3.tar.gz` & `tmp/pyfsdb-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfsdb-2.1.3.tar", last modified: Thu May 11 20:24:18 2023, max compression
+gzip compressed data, was "pyfsdb-2.1.4.tar", last modified: Tue May 16 17:45:43 2023, max compression
```

## Comparing `pyfsdb-2.1.3.tar` & `pyfsdb-2.1.4.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-05-11 20:24:18.202106 pyfsdb-2.1.3/
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1127 2021-03-18 13:10:45.000000 pyfsdb-2.1.3/LICENSE
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     6054 2023-05-11 20:24:18.202106 pyfsdb-2.1.3/PKG-INFO
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     5649 2023-01-17 14:56:42.000000 pyfsdb-2.1.3/README.md
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-05-11 20:24:18.190106 pyfsdb-2.1.3/pyfsdb/
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      167 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/__init__.py
--rwxr-xr-x   0 hardaker  (2174) hardaker  (2174)    35086 2023-01-25 14:19:32.000000 pyfsdb-2.1.3/pyfsdb/fsdb.py
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-05-11 20:24:18.195106 pyfsdb-2.1.3/pyfsdb/obsolete/
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)        0 2021-04-11 14:12:46.000000 pyfsdb-2.1.3/pyfsdb/obsolete/__init__.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      198 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/obsolete/db2tex.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      210 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/obsolete/dbaugment.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      210 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/obsolete/dbcoluniq.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      226 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/obsolete/dbdatetoepoch.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      206 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/obsolete/dbensure.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      206 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/obsolete/dbformat.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      218 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/obsolete/dbfullpivot.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      210 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/obsolete/dbheatmap.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      218 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/obsolete/dbkeyedsort.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      218 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/obsolete/dbnormalize.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      214 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/obsolete/dbreescape.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      230 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/obsolete/dbreversepivot.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      214 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/obsolete/dbsplitter.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      194 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/obsolete/dbsum.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      198 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/obsolete/dbtopn.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      214 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/obsolete/dbzerofill.py
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-05-11 20:24:18.202106 pyfsdb-2.1.3/pyfsdb/tools/
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)        0 2021-04-11 14:12:46.000000 pyfsdb-2.1.3/pyfsdb/tools/__init__.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     1989 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/tools/bro2fsdb.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     3355 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/tools/fsdb2json.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     1868 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/tools/fsdb2many.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     2360 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/tools/json2fsdb.py
--rwxr-xr-x   0 hardaker  (2174) hardaker  (2174)    10589 2022-11-12 21:47:13.000000 pyfsdb-2.1.3/pyfsdb/tools/pdb2sql.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     2845 2023-01-05 01:36:03.000000 pyfsdb-2.1.3/pyfsdb/tools/pdb2tex.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1133 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/tools/pdb2to1.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     2665 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/tools/pdbaddtypes.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     7015 2023-01-06 15:32:58.000000 pyfsdb-2.1.3/pyfsdb/tools/pdbaugment.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     3510 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/tools/pdbcdf.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     3430 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/tools/pdbcoluniq.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1866 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/tools/pdbdatetoepoch.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     2134 2023-01-05 01:16:54.000000 pyfsdb-2.1.3/pyfsdb/tools/pdbensure.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     1900 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/tools/pdbepochtodate.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     1398 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/tools/pdbformat.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     3022 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/tools/pdbfullpivot.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)    10044 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/tools/pdbheatmap.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     2373 2023-01-21 22:46:03.000000 pyfsdb-2.1.3/pyfsdb/tools/pdbjinja.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     3707 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/tools/pdbkeyedsort.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1570 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/tools/pdbnormalize.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     1426 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/tools/pdbreescape.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     2663 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/tools/pdbreversepivot.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     3585 2022-08-21 13:26:37.000000 pyfsdb-2.1.3/pyfsdb/tools/pdbroc.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     2601 2023-05-10 21:40:55.000000 pyfsdb-2.1.3/pyfsdb/tools/pdbrow.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     3325 2023-05-10 21:42:43.000000 pyfsdb-2.1.3/pyfsdb/tools/pdbroweval.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     3513 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/tools/pdbsplitter.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     3075 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/tools/pdbsum.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     3357 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/tools/pdbtopn.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     2297 2023-02-06 19:45:06.000000 pyfsdb-2.1.3/pyfsdb/tools/pdbzerofill.py
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-05-11 20:24:18.191106 pyfsdb-2.1.3/pyfsdb.egg-info/
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     6054 2023-05-11 20:24:17.000000 pyfsdb-2.1.3/pyfsdb.egg-info/PKG-INFO
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1505 2023-05-11 20:24:18.000000 pyfsdb-2.1.3/pyfsdb.egg-info/SOURCES.txt
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)        1 2023-05-11 20:24:17.000000 pyfsdb-2.1.3/pyfsdb.egg-info/dependency_links.txt
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1861 2023-05-11 20:24:17.000000 pyfsdb-2.1.3/pyfsdb.egg-info/entry_points.txt
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)        7 2023-05-11 20:24:17.000000 pyfsdb-2.1.3/pyfsdb.egg-info/top_level.txt
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)       38 2023-05-11 20:24:18.202106 pyfsdb-2.1.3/setup.cfg
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     3323 2023-05-11 20:17:26.000000 pyfsdb-2.1.3/setup.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-05-16 17:45:43.790657 pyfsdb-2.1.4/
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1127 2021-03-18 13:10:45.000000 pyfsdb-2.1.4/LICENSE
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     6054 2023-05-16 17:45:43.789657 pyfsdb-2.1.4/PKG-INFO
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     5649 2023-01-17 14:56:42.000000 pyfsdb-2.1.4/README.md
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-05-16 17:45:43.604657 pyfsdb-2.1.4/pyfsdb/
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      167 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/__init__.py
+-rwxr-xr-x   0 hardaker  (2174) hardaker  (2174)    35086 2023-01-25 14:19:32.000000 pyfsdb-2.1.4/pyfsdb/fsdb.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-05-16 17:45:43.609657 pyfsdb-2.1.4/pyfsdb/obsolete/
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)        0 2021-04-11 14:12:46.000000 pyfsdb-2.1.4/pyfsdb/obsolete/__init__.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      198 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/obsolete/db2tex.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      210 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/obsolete/dbaugment.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      210 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/obsolete/dbcoluniq.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      226 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/obsolete/dbdatetoepoch.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      206 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/obsolete/dbensure.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      206 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/obsolete/dbformat.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      218 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/obsolete/dbfullpivot.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      210 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/obsolete/dbheatmap.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      218 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/obsolete/dbkeyedsort.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      218 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/obsolete/dbnormalize.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      214 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/obsolete/dbreescape.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      230 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/obsolete/dbreversepivot.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      214 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/obsolete/dbsplitter.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      194 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/obsolete/dbsum.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      198 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/obsolete/dbtopn.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      214 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/obsolete/dbzerofill.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-05-16 17:45:43.788657 pyfsdb-2.1.4/pyfsdb/tools/
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)        0 2021-04-11 14:12:46.000000 pyfsdb-2.1.4/pyfsdb/tools/__init__.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     1989 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/tools/bro2fsdb.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     3355 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/tools/fsdb2json.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     1868 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/tools/fsdb2many.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     2360 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/tools/json2fsdb.py
+-rwxr-xr-x   0 hardaker  (2174) hardaker  (2174)    10589 2022-11-12 21:47:13.000000 pyfsdb-2.1.4/pyfsdb/tools/pdb2sql.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     2845 2023-01-05 01:36:03.000000 pyfsdb-2.1.4/pyfsdb/tools/pdb2tex.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1133 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/tools/pdb2to1.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     2665 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/tools/pdbaddtypes.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     7015 2023-01-06 15:32:58.000000 pyfsdb-2.1.4/pyfsdb/tools/pdbaugment.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     3510 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/tools/pdbcdf.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     3430 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/tools/pdbcoluniq.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1866 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/tools/pdbdatetoepoch.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     2134 2023-01-05 01:16:54.000000 pyfsdb-2.1.4/pyfsdb/tools/pdbensure.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     1900 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/tools/pdbepochtodate.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     1398 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/tools/pdbformat.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     3022 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/tools/pdbfullpivot.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)    10044 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/tools/pdbheatmap.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     2373 2023-01-21 22:46:03.000000 pyfsdb-2.1.4/pyfsdb/tools/pdbjinja.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     3707 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/tools/pdbkeyedsort.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1570 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/tools/pdbnormalize.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     1426 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/tools/pdbreescape.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     2663 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/tools/pdbreversepivot.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     3585 2022-08-21 13:26:37.000000 pyfsdb-2.1.4/pyfsdb/tools/pdbroc.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     3230 2023-05-13 04:31:26.000000 pyfsdb-2.1.4/pyfsdb/tools/pdbrow.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     3524 2023-05-11 20:36:19.000000 pyfsdb-2.1.4/pyfsdb/tools/pdbroweval.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     3513 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/tools/pdbsplitter.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     3075 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/tools/pdbsum.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     3357 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/tools/pdbtopn.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     2297 2023-02-06 19:45:06.000000 pyfsdb-2.1.4/pyfsdb/tools/pdbzerofill.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-05-16 17:45:43.605657 pyfsdb-2.1.4/pyfsdb.egg-info/
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     6054 2023-05-16 17:45:43.000000 pyfsdb-2.1.4/pyfsdb.egg-info/PKG-INFO
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1505 2023-05-16 17:45:43.000000 pyfsdb-2.1.4/pyfsdb.egg-info/SOURCES.txt
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)        1 2023-05-16 17:45:43.000000 pyfsdb-2.1.4/pyfsdb.egg-info/dependency_links.txt
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1861 2023-05-16 17:45:43.000000 pyfsdb-2.1.4/pyfsdb.egg-info/entry_points.txt
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)        7 2023-05-16 17:45:43.000000 pyfsdb-2.1.4/pyfsdb.egg-info/top_level.txt
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)       38 2023-05-16 17:45:43.790657 pyfsdb-2.1.4/setup.cfg
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     3323 2023-05-16 17:45:09.000000 pyfsdb-2.1.4/setup.py
```

### Comparing `pyfsdb-2.1.3/LICENSE` & `pyfsdb-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.3/PKG-INFO` & `pyfsdb-2.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfsdb
-Version: 2.1.3
+Version: 2.1.4
 Summary: A python implementation of the flat-file streaming database
 Home-page: https://github.com/gawseed/pyfsdb
 Author: Wes Hardaker
 Author-email: opensource@hardakers.net
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `pyfsdb-2.1.3/README.md` & `pyfsdb-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.3/pyfsdb/fsdb.py` & `pyfsdb-2.1.4/pyfsdb/fsdb.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.3/pyfsdb/tools/bro2fsdb.py` & `pyfsdb-2.1.4/pyfsdb/tools/bro2fsdb.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.3/pyfsdb/tools/fsdb2json.py` & `pyfsdb-2.1.4/pyfsdb/tools/fsdb2json.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.3/pyfsdb/tools/fsdb2many.py` & `pyfsdb-2.1.4/pyfsdb/tools/fsdb2many.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.3/pyfsdb/tools/json2fsdb.py` & `pyfsdb-2.1.4/pyfsdb/tools/json2fsdb.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.3/pyfsdb/tools/pdb2sql.py` & `pyfsdb-2.1.4/pyfsdb/tools/pdb2sql.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.3/pyfsdb/tools/pdb2tex.py` & `pyfsdb-2.1.4/pyfsdb/tools/pdb2tex.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.3/pyfsdb/tools/pdb2to1.py` & `pyfsdb-2.1.4/pyfsdb/tools/pdb2to1.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.3/pyfsdb/tools/pdbaddtypes.py` & `pyfsdb-2.1.4/pyfsdb/tools/pdbaddtypes.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.3/pyfsdb/tools/pdbaugment.py` & `pyfsdb-2.1.4/pyfsdb/tools/pdbaugment.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.3/pyfsdb/tools/pdbcdf.py` & `pyfsdb-2.1.4/pyfsdb/tools/pdbcdf.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.3/pyfsdb/tools/pdbcoluniq.py` & `pyfsdb-2.1.4/pyfsdb/tools/pdbcoluniq.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.3/pyfsdb/tools/pdbdatetoepoch.py` & `pyfsdb-2.1.4/pyfsdb/tools/pdbdatetoepoch.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.3/pyfsdb/tools/pdbensure.py` & `pyfsdb-2.1.4/pyfsdb/tools/pdbensure.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.3/pyfsdb/tools/pdbepochtodate.py` & `pyfsdb-2.1.4/pyfsdb/tools/pdbepochtodate.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.3/pyfsdb/tools/pdbformat.py` & `pyfsdb-2.1.4/pyfsdb/tools/pdbformat.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.3/pyfsdb/tools/pdbfullpivot.py` & `pyfsdb-2.1.4/pyfsdb/tools/pdbfullpivot.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.3/pyfsdb/tools/pdbheatmap.py` & `pyfsdb-2.1.4/pyfsdb/tools/pdbheatmap.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.3/pyfsdb/tools/pdbjinja.py` & `pyfsdb-2.1.4/pyfsdb/tools/pdbjinja.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.3/pyfsdb/tools/pdbkeyedsort.py` & `pyfsdb-2.1.4/pyfsdb/tools/pdbkeyedsort.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.3/pyfsdb/tools/pdbnormalize.py` & `pyfsdb-2.1.4/pyfsdb/tools/pdbnormalize.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.3/pyfsdb/tools/pdbreescape.py` & `pyfsdb-2.1.4/pyfsdb/tools/pdbreescape.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.3/pyfsdb/tools/pdbreversepivot.py` & `pyfsdb-2.1.4/pyfsdb/tools/pdbreversepivot.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.3/pyfsdb/tools/pdbroc.py` & `pyfsdb-2.1.4/pyfsdb/tools/pdbroc.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.3/pyfsdb/tools/pdbrow.py` & `pyfsdb-2.1.4/pyfsdb/tools/pdbrow.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,14 +18,22 @@
         "-u",
         "--underbars",
         action="store_true",
         help="Use variable names with _ prefixes to the column names",
     )
 
     parser.add_argument(
+        "-n",
+        "--namedtuple",
+        default=None,
+        type=str,
+        help="Use a namedtuple under this name to store data",
+    )
+
+    parser.add_argument(
         "-i", "--init-code", help="Initialization code to execute first (eg, imports)"
     )
 
     parser.add_argument(
         "--log-level", default="info", help="Define the logging verbosity level."
     )
 
@@ -58,38 +66,53 @@
 
 def process_pdbrow(
     input_file,
     output_file,
     expression,
     init_code=None,
     use_underbars=False,
+    use_namedtuple=None,
 ):
 
+    return_type = pyfsdb.RETURN_AS_DICTIONARY
+    if use_namedtuple:
+        return_type = pyfsdb.RETURN_AS_ARRAY
+
     # open input and output fsdb handles
-    fh = pyfsdb.Fsdb(file_handle=input_file, return_type=pyfsdb.RETURN_AS_DICTIONARY)
+    fh = pyfsdb.Fsdb(file_handle=input_file, return_type=return_type)
     oh = pyfsdb.Fsdb(out_file_handle=output_file)
 
     # crate output columns
     oh.out_column_names = fh.column_names
 
     globals = {}
 
     if init_code:
         exec(compile(init_code, "<string>", "exec"), globals)
 
     compiled_expression = compile(f"{expression}", "<string>", "eval")
 
+    if use_namedtuple:
+        from collections import namedtuple
+
+        named_row = namedtuple("named_row", fh.column_names)
+
     # process the rows
     for row in fh:
 
         # if they wanted under-bar based names, add them
         if use_underbars:
             result = eval(
                 compiled_expression, globals, {"_" + k: v for k, v in row.items()}
             )
+
+        elif use_namedtuple:
+            contents = named_row(*row)
+            result = eval(compiled_expression, globals, {use_namedtuple: contents})
+
         else:
             result = eval(compiled_expression, globals, row)
 
         if result:
             oh.append(row)
 
     oh.close()
@@ -99,12 +122,14 @@
     args = parse_args()
 
     process_pdbrow(
         args.input_file,
         args.output_file,
         args.expression,
         args.init_code,
+        args.underbars,
+        args.namedtuple,
     )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pyfsdb-2.1.3/pyfsdb/tools/pdbroweval.py` & `pyfsdb-2.1.4/pyfsdb/tools/pdbroweval.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,41 +76,42 @@
 
 
 def process_pdbroweval(
     input_file,
     output_file,
     expression,
     init_code=None,
-    from_file=False,
-    init_code_file=False,
+    expression_is_file=False,
+    init_code_is_file=False,
     use_underbars=False,
 ):
 
     # open input and output fsdb handles
     fh = pyfsdb.Fsdb(file_handle=input_file, return_type=pyfsdb.RETURN_AS_DICTIONARY)
     oh = pyfsdb.Fsdb(out_file_handle=output_file)
 
     # crate output columns
     oh.out_column_names = fh.column_names
 
     globals = {}
 
     if init_code:
-        if init_code_file:
+        if init_code_is_file:
             init_code = init_code.read()
         exec(compile(init_code, "<string>", "exec"), globals)
 
-    if from_file:
+    if expression_is_file:
         expression = expression.read()
         error(expression)
     compiled_expression = compile(f"{expression}", "<string>", "exec")
 
     # if they wanted under-bar based names
     if use_underbars:
         fh.column_names = ["_" + x for x in fh.column_names]
+        fh.converters = {"_" + x: y for x, y in fh.converters.items()}
 
     # process the rows
     for row in fh:
 
         # execute the expression and check its result
         exec(compiled_expression, globals, row)
         if use_underbars:
@@ -122,16 +123,17 @@
 
 def main():
     args = parse_args()
 
     process_pdbroweval(
         args.input_file,
         args.output_file,
-        args.expression,
-        args.init_code,
-        args.expression_is_file,
-        args.underbars,
+        expression=args.expression,
+        init_code=args.init_code,
+        expression_is_file=args.expression_is_file,
+        init_code_is_file=args.init_code_is_file,
+        use_underbars=args.underbars,
     )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pyfsdb-2.1.3/pyfsdb/tools/pdbsplitter.py` & `pyfsdb-2.1.4/pyfsdb/tools/pdbsplitter.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.3/pyfsdb/tools/pdbsum.py` & `pyfsdb-2.1.4/pyfsdb/tools/pdbsum.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.3/pyfsdb/tools/pdbtopn.py` & `pyfsdb-2.1.4/pyfsdb/tools/pdbtopn.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.3/pyfsdb/tools/pdbzerofill.py` & `pyfsdb-2.1.4/pyfsdb/tools/pdbzerofill.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.3/pyfsdb.egg-info/PKG-INFO` & `pyfsdb-2.1.4/pyfsdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfsdb
-Version: 2.1.3
+Version: 2.1.4
 Summary: A python implementation of the flat-file streaming database
 Home-page: https://github.com/gawseed/pyfsdb
 Author: Wes Hardaker
 Author-email: opensource@hardakers.net
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `pyfsdb-2.1.3/pyfsdb.egg-info/SOURCES.txt` & `pyfsdb-2.1.4/pyfsdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.3/pyfsdb.egg-info/entry_points.txt` & `pyfsdb-2.1.4/pyfsdb.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.3/setup.py` & `pyfsdb-2.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyfsdb",
-    version="2.1.3",
+    version="2.1.4",
     author="Wes Hardaker",
     author_email="opensource@hardakers.net",
     description="A python implementation of the flat-file streaming database",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gawseed/pyfsdb",
     packages=setuptools.find_packages(),
```

