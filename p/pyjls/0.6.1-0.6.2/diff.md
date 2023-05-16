# Comparing `tmp/pyjls-0.6.1.tar.gz` & `tmp/pyjls-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjls-0.6.1.tar", last modified: Thu Apr 27 22:12:27 2023, max compression
+gzip compressed data, was "pyjls-0.6.2.tar", last modified: Fri Apr 28 18:55:36 2023, max compression
```

## Comparing `pyjls-0.6.1.tar` & `pyjls-0.6.2.tar`

### file list

```diff
@@ -1,78 +1,79 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 22:12:27.400065 pyjls-0.6.1/
--rw-rw-rw-   0        0        0     4219 2023-04-27 22:08:49.000000 pyjls-0.6.1/CHANGELOG.md
--rw-rw-rw-   0        0        0     3039 2021-03-18 16:48:36.000000 pyjls-0.6.1/CREDITS.html
--rw-rw-rw-   0        0        0    11558 2018-07-03 17:53:12.000000 pyjls-0.6.1/LICENSE
--rw-rw-rw-   0        0        0      177 2021-03-10 13:52:18.000000 pyjls-0.6.1/MANIFEST.in
--rw-rw-rw-   0        0        0    14665 2023-04-27 22:12:27.399565 pyjls-0.6.1/PKG-INFO
--rw-rw-rw-   0        0        0    13054 2022-03-07 15:46:24.000000 pyjls-0.6.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 22:12:27.369250 pyjls-0.6.1/include/
-drwxrwxrwx   0        0        0        0 2023-04-27 22:12:27.375270 pyjls-0.6.1/include/jls/
--rw-rw-rw-   0        0        0     2729 2023-04-19 20:33:33.000000 pyjls-0.6.1/include/jls/backend.h
--rw-rw-rw-   0        0        0     2068 2022-03-05 19:14:45.000000 pyjls-0.6.1/include/jls/cmacro.h
--rw-rw-rw-   0        0        0     1585 2022-03-05 19:14:45.000000 pyjls-0.6.1/include/jls/crc32c.h
--rw-rw-rw-   0        0        0     4064 2022-03-05 19:14:45.000000 pyjls-0.6.1/include/jls/ec.h
--rw-rw-rw-   0        0        0    24468 2023-04-26 11:42:25.000000 pyjls-0.6.1/include/jls/format.h
--rw-rw-rw-   0        0        0    11561 2023-04-26 14:23:01.000000 pyjls-0.6.1/include/jls/log.h
--rw-rw-rw-   0        0        0     6351 2022-03-05 19:14:45.000000 pyjls-0.6.1/include/jls/raw.h
--rw-rw-rw-   0        0        0    10319 2023-04-26 17:43:17.000000 pyjls-0.6.1/include/jls/reader.h
--rw-rw-rw-   0        0        0     4133 2022-03-05 19:14:45.000000 pyjls-0.6.1/include/jls/statistics.h
--rw-rw-rw-   0        0        0     2561 2022-03-05 19:14:45.000000 pyjls-0.6.1/include/jls/threaded_writer.h
--rw-rw-rw-   0        0        0    12420 2023-04-19 20:31:02.000000 pyjls-0.6.1/include/jls/time.h
--rw-rw-rw-   0        0        0     2760 2023-04-27 22:10:57.000000 pyjls-0.6.1/include/jls/version.h
--rw-rw-rw-   0        0        0     5775 2022-03-05 19:14:45.000000 pyjls-0.6.1/include/jls/writer.h
--rw-rw-rw-   0        0        0      895 2022-03-05 19:14:45.000000 pyjls-0.6.1/include/jls.h
-drwxrwxrwx   0        0        0        0 2023-04-27 22:12:27.364542 pyjls-0.6.1/include_prv/
-drwxrwxrwx   0        0        0        0 2023-04-27 22:12:27.378770 pyjls-0.6.1/include_prv/jls/
--rw-rw-rw-   0        0        0     1385 2022-03-07 15:46:24.000000 pyjls-0.6.1/include_prv/jls/bit_shift.h
--rw-rw-rw-   0        0        0     2099 2022-03-05 19:14:45.000000 pyjls-0.6.1/include_prv/jls/cdef.h
--rw-rw-rw-   0        0        0     1524 2022-03-07 15:46:24.000000 pyjls-0.6.1/include_prv/jls/datatype.h
--rw-rw-rw-   0        0        0     2676 2022-03-05 19:14:45.000000 pyjls-0.6.1/include_prv/jls/msg_ring_buffer.h
--rw-rw-rw-   0        0        0     1784 2023-04-26 18:12:34.000000 pyjls-0.6.1/include_prv/jls/rd_fsr.h
--rw-rw-rw-   0        0        0     1276 2022-03-05 19:14:45.000000 pyjls-0.6.1/include_prv/jls/util.h
--rw-rw-rw-   0        0        0     1945 2022-03-05 19:14:45.000000 pyjls-0.6.1/include_prv/jls/wr_fsr.h
--rw-rw-rw-   0        0        0     1744 2022-03-05 19:14:45.000000 pyjls-0.6.1/include_prv/jls/wr_prv.h
--rw-rw-rw-   0        0        0     3042 2022-03-05 19:14:45.000000 pyjls-0.6.1/include_prv/jls/wr_ts.h
-drwxrwxrwx   0        0        0        0 2023-04-27 22:12:27.381783 pyjls-0.6.1/pyjls/
--rw-rw-rw-   0        0        0     1208 2023-03-04 20:14:09.000000 pyjls-0.6.1/pyjls/__init__.py
--rw-rw-rw-   0        0        0     2557 2022-03-05 19:14:45.000000 pyjls-0.6.1/pyjls/__main__.py
--rw-rw-rw-   0        0        0  1587118 2023-04-26 19:59:45.000000 pyjls-0.6.1/pyjls/binding.c
-drwxrwxrwx   0        0        0        0 2023-04-27 22:12:27.390296 pyjls-0.6.1/pyjls/entry_points/
--rw-rw-rw-   0        0        0      853 2022-03-05 19:14:45.000000 pyjls-0.6.1/pyjls/entry_points/__init__.py
--rw-rw-rw-   0        0        0     2738 2022-03-05 19:14:45.000000 pyjls-0.6.1/pyjls/entry_points/annotate.py
--rw-rw-rw-   0        0        0     1621 2022-03-05 19:14:45.000000 pyjls-0.6.1/pyjls/entry_points/info.py
--rw-rw-rw-   0        0        0     2206 2023-04-26 14:31:44.000000 pyjls-0.6.1/pyjls/structs.py
-drwxrwxrwx   0        0        0        0 2023-04-27 22:12:27.390796 pyjls-0.6.1/pyjls/test/
--rw-rw-rw-   0        0        0      594 2022-03-05 19:14:45.000000 pyjls-0.6.1/pyjls/test/__init__.py
--rw-rw-rw-   0        0        0    10313 2023-04-26 19:18:13.000000 pyjls-0.6.1/pyjls/test/test_binding.py
-drwxrwxrwx   0        0        0        0 2023-04-27 22:12:27.390796 pyjls-0.6.1/pyjls/v1/
--rw-rw-rw-   0        0        0      594 2022-03-05 19:14:45.000000 pyjls-0.6.1/pyjls/v1/__init__.py
--rw-rw-rw-   0        0        0     1059 2023-04-27 22:10:57.000000 pyjls-0.6.1/pyjls/version.py
-drwxrwxrwx   0        0        0        0 2023-04-27 22:12:27.388793 pyjls-0.6.1/pyjls.egg-info/
--rw-rw-rw-   0        0        0    14665 2023-04-27 22:12:27.000000 pyjls-0.6.1/pyjls.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1310 2023-04-27 22:12:27.000000 pyjls-0.6.1/pyjls.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 22:12:27.000000 pyjls-0.6.1/pyjls.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-04-27 22:12:27.000000 pyjls-0.6.1/pyjls.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       53 2023-04-27 22:12:27.000000 pyjls-0.6.1/pyjls.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-27 22:12:27.000000 pyjls-0.6.1/pyjls.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      851 2022-11-30 13:53:49.000000 pyjls-0.6.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-27 22:12:27.400065 pyjls-0.6.1/setup.cfg
--rw-rw-rw-   0        0        0     6742 2023-04-27 15:16:07.000000 pyjls-0.6.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-27 22:12:27.399061 pyjls-0.6.1/src/
--rw-rw-rw-   0        0        0     8684 2023-04-19 20:32:02.000000 pyjls-0.6.1/src/backend_posix.c
--rw-rw-rw-   0        0        0     9046 2023-04-19 20:31:50.000000 pyjls-0.6.1/src/backend_win.c
--rw-rw-rw-   0        0        0     1179 2022-03-07 15:46:24.000000 pyjls-0.6.1/src/bit_shift.c
--rw-rw-rw-   0        0        0     1855 2022-03-05 19:14:45.000000 pyjls-0.6.1/src/crc32c_arm_neon.c
--rw-rw-rw-   0        0        0     2433 2022-03-05 19:14:45.000000 pyjls-0.6.1/src/crc32c_intel_sse4.c
--rw-rw-rw-   0        0        0    33673 2022-03-05 19:14:45.000000 pyjls-0.6.1/src/crc32c_sw.c
--rw-rw-rw-   0        0        0     3589 2022-03-07 15:46:24.000000 pyjls-0.6.1/src/datatype.c
--rw-rw-rw-   0        0        0     1113 2022-03-05 19:14:45.000000 pyjls-0.6.1/src/ec.c
--rw-rw-rw-   0        0        0     1631 2023-04-19 17:02:27.000000 pyjls-0.6.1/src/log.c
--rw-rw-rw-   0        0        0     3970 2022-03-07 15:46:24.000000 pyjls-0.6.1/src/msg_ring_buffer.c
--rw-rw-rw-   0        0        0    17311 2023-04-19 20:32:58.000000 pyjls-0.6.1/src/raw.c
--rw-rw-rw-   0        0        0     5903 2023-04-26 19:35:45.000000 pyjls-0.6.1/src/rd_fsr.c
--rw-rw-rw-   0        0        0    54497 2023-04-27 17:06:33.000000 pyjls-0.6.1/src/reader.c
--rw-rw-rw-   0        0        0     4302 2022-03-05 19:14:45.000000 pyjls-0.6.1/src/statistics.c
--rw-rw-rw-   0        0        0    11622 2023-04-27 15:21:50.000000 pyjls-0.6.1/src/threaded_writer.c
--rw-rw-rw-   0        0        0    27653 2023-04-27 21:59:42.000000 pyjls-0.6.1/src/wr_fsr.c
--rw-rw-rw-   0        0        0     9691 2023-04-26 14:57:54.000000 pyjls-0.6.1/src/wr_ts.c
--rw-rw-rw-   0        0        0    30342 2023-04-26 12:23:06.000000 pyjls-0.6.1/src/writer.c
+drwxrwxrwx   0        0        0        0 2023-04-28 18:55:36.929698 pyjls-0.6.2/
+-rw-rw-rw-   0        0        0     4410 2023-04-28 18:32:52.000000 pyjls-0.6.2/CHANGELOG.md
+-rw-rw-rw-   0        0        0     3039 2021-03-18 16:48:36.000000 pyjls-0.6.2/CREDITS.html
+-rw-rw-rw-   0        0        0    11558 2018-07-03 17:53:12.000000 pyjls-0.6.2/LICENSE
+-rw-rw-rw-   0        0        0      177 2021-03-10 13:52:18.000000 pyjls-0.6.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    14665 2023-04-28 18:55:36.929198 pyjls-0.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0    13054 2022-03-07 15:46:24.000000 pyjls-0.6.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 18:55:36.898654 pyjls-0.6.2/include/
+drwxrwxrwx   0        0        0        0 2023-04-28 18:55:36.904661 pyjls-0.6.2/include/jls/
+-rw-rw-rw-   0        0        0     2729 2023-04-19 20:33:33.000000 pyjls-0.6.2/include/jls/backend.h
+-rw-rw-rw-   0        0        0     2068 2022-03-05 19:14:45.000000 pyjls-0.6.2/include/jls/cmacro.h
+-rw-rw-rw-   0        0        0     1585 2022-03-05 19:14:45.000000 pyjls-0.6.2/include/jls/crc32c.h
+-rw-rw-rw-   0        0        0     4064 2022-03-05 19:14:45.000000 pyjls-0.6.2/include/jls/ec.h
+-rw-rw-rw-   0        0        0    24468 2023-04-26 11:42:25.000000 pyjls-0.6.2/include/jls/format.h
+-rw-rw-rw-   0        0        0    11561 2023-04-26 14:23:01.000000 pyjls-0.6.2/include/jls/log.h
+-rw-rw-rw-   0        0        0     6351 2022-03-05 19:14:45.000000 pyjls-0.6.2/include/jls/raw.h
+-rw-rw-rw-   0        0        0    10319 2023-04-26 17:43:17.000000 pyjls-0.6.2/include/jls/reader.h
+-rw-rw-rw-   0        0        0     4133 2022-03-05 19:14:45.000000 pyjls-0.6.2/include/jls/statistics.h
+-rw-rw-rw-   0        0        0     2561 2022-03-05 19:14:45.000000 pyjls-0.6.2/include/jls/threaded_writer.h
+-rw-rw-rw-   0        0        0    12420 2023-04-19 20:31:02.000000 pyjls-0.6.2/include/jls/time.h
+-rw-rw-rw-   0        0        0     2760 2023-04-28 12:38:47.000000 pyjls-0.6.2/include/jls/version.h
+-rw-rw-rw-   0        0        0     5775 2022-03-05 19:14:45.000000 pyjls-0.6.2/include/jls/writer.h
+-rw-rw-rw-   0        0        0      895 2022-03-05 19:14:45.000000 pyjls-0.6.2/include/jls.h
+drwxrwxrwx   0        0        0        0 2023-04-28 18:55:36.894186 pyjls-0.6.2/include_prv/
+drwxrwxrwx   0        0        0        0 2023-04-28 18:55:36.908165 pyjls-0.6.2/include_prv/jls/
+-rw-rw-rw-   0        0        0     1385 2022-03-07 15:46:24.000000 pyjls-0.6.2/include_prv/jls/bit_shift.h
+-rw-rw-rw-   0        0        0     2099 2022-03-05 19:14:45.000000 pyjls-0.6.2/include_prv/jls/cdef.h
+-rw-rw-rw-   0        0        0     1524 2022-03-07 15:46:24.000000 pyjls-0.6.2/include_prv/jls/datatype.h
+-rw-rw-rw-   0        0        0     2676 2022-03-05 19:14:45.000000 pyjls-0.6.2/include_prv/jls/msg_ring_buffer.h
+-rw-rw-rw-   0        0        0     1784 2023-04-26 18:12:34.000000 pyjls-0.6.2/include_prv/jls/rd_fsr.h
+-rw-rw-rw-   0        0        0     1276 2022-03-05 19:14:45.000000 pyjls-0.6.2/include_prv/jls/util.h
+-rw-rw-rw-   0        0        0     1945 2022-03-05 19:14:45.000000 pyjls-0.6.2/include_prv/jls/wr_fsr.h
+-rw-rw-rw-   0        0        0     1744 2022-03-05 19:14:45.000000 pyjls-0.6.2/include_prv/jls/wr_prv.h
+-rw-rw-rw-   0        0        0     3042 2022-03-05 19:14:45.000000 pyjls-0.6.2/include_prv/jls/wr_ts.h
+drwxrwxrwx   0        0        0        0 2023-04-28 18:55:36.911170 pyjls-0.6.2/pyjls/
+-rw-rw-rw-   0        0        0     1208 2023-03-04 20:14:09.000000 pyjls-0.6.2/pyjls/__init__.py
+-rw-rw-rw-   0        0        0     2557 2022-03-05 19:14:45.000000 pyjls-0.6.2/pyjls/__main__.py
+-rw-rw-rw-   0        0        0  1587118 2023-04-26 19:59:45.000000 pyjls-0.6.2/pyjls/binding.c
+drwxrwxrwx   0        0        0        0 2023-04-28 18:55:36.919679 pyjls-0.6.2/pyjls/entry_points/
+-rw-rw-rw-   0        0        0      869 2023-04-28 18:19:13.000000 pyjls-0.6.2/pyjls/entry_points/__init__.py
+-rw-rw-rw-   0        0        0     2738 2022-03-05 19:14:45.000000 pyjls-0.6.2/pyjls/entry_points/annotate.py
+-rw-rw-rw-   0        0        0     2561 2023-04-28 18:26:31.000000 pyjls-0.6.2/pyjls/entry_points/export.py
+-rw-rw-rw-   0        0        0     2019 2023-04-28 12:29:04.000000 pyjls-0.6.2/pyjls/entry_points/info.py
+-rw-rw-rw-   0        0        0     2333 2023-04-28 12:48:59.000000 pyjls-0.6.2/pyjls/structs.py
+drwxrwxrwx   0        0        0        0 2023-04-28 18:55:36.920179 pyjls-0.6.2/pyjls/test/
+-rw-rw-rw-   0        0        0      594 2022-03-05 19:14:45.000000 pyjls-0.6.2/pyjls/test/__init__.py
+-rw-rw-rw-   0        0        0    10313 2023-04-26 19:18:13.000000 pyjls-0.6.2/pyjls/test/test_binding.py
+drwxrwxrwx   0        0        0        0 2023-04-28 18:55:36.921181 pyjls-0.6.2/pyjls/v1/
+-rw-rw-rw-   0        0        0      594 2022-03-05 19:14:45.000000 pyjls-0.6.2/pyjls/v1/__init__.py
+-rw-rw-rw-   0        0        0     1059 2023-04-28 12:38:47.000000 pyjls-0.6.2/pyjls/version.py
+drwxrwxrwx   0        0        0        0 2023-04-28 18:55:36.918179 pyjls-0.6.2/pyjls.egg-info/
+-rw-rw-rw-   0        0        0    14665 2023-04-28 18:55:36.000000 pyjls-0.6.2/pyjls.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1339 2023-04-28 18:55:36.000000 pyjls-0.6.2/pyjls.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 18:55:36.000000 pyjls-0.6.2/pyjls.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-04-28 18:55:36.000000 pyjls-0.6.2/pyjls.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       53 2023-04-28 18:55:36.000000 pyjls-0.6.2/pyjls.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-28 18:55:36.000000 pyjls-0.6.2/pyjls.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      851 2022-11-30 13:53:49.000000 pyjls-0.6.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-28 18:55:36.929698 pyjls-0.6.2/setup.cfg
+-rw-rw-rw-   0        0        0     6742 2023-04-27 15:16:07.000000 pyjls-0.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 18:55:36.928698 pyjls-0.6.2/src/
+-rw-rw-rw-   0        0        0     8684 2023-04-19 20:32:02.000000 pyjls-0.6.2/src/backend_posix.c
+-rw-rw-rw-   0        0        0     9046 2023-04-19 20:31:50.000000 pyjls-0.6.2/src/backend_win.c
+-rw-rw-rw-   0        0        0     1179 2022-03-07 15:46:24.000000 pyjls-0.6.2/src/bit_shift.c
+-rw-rw-rw-   0        0        0     1855 2022-03-05 19:14:45.000000 pyjls-0.6.2/src/crc32c_arm_neon.c
+-rw-rw-rw-   0        0        0     2433 2022-03-05 19:14:45.000000 pyjls-0.6.2/src/crc32c_intel_sse4.c
+-rw-rw-rw-   0        0        0    33673 2022-03-05 19:14:45.000000 pyjls-0.6.2/src/crc32c_sw.c
+-rw-rw-rw-   0        0        0     3589 2022-03-07 15:46:24.000000 pyjls-0.6.2/src/datatype.c
+-rw-rw-rw-   0        0        0     1113 2022-03-05 19:14:45.000000 pyjls-0.6.2/src/ec.c
+-rw-rw-rw-   0        0        0     1631 2023-04-19 17:02:27.000000 pyjls-0.6.2/src/log.c
+-rw-rw-rw-   0        0        0     3970 2022-03-07 15:46:24.000000 pyjls-0.6.2/src/msg_ring_buffer.c
+-rw-rw-rw-   0        0        0    17311 2023-04-19 20:32:58.000000 pyjls-0.6.2/src/raw.c
+-rw-rw-rw-   0        0        0     5903 2023-04-26 19:35:45.000000 pyjls-0.6.2/src/rd_fsr.c
+-rw-rw-rw-   0        0        0    54650 2023-04-28 12:42:07.000000 pyjls-0.6.2/src/reader.c
+-rw-rw-rw-   0        0        0     4302 2022-03-05 19:14:45.000000 pyjls-0.6.2/src/statistics.c
+-rw-rw-rw-   0        0        0    11622 2023-04-27 15:21:50.000000 pyjls-0.6.2/src/threaded_writer.c
+-rw-rw-rw-   0        0        0    27815 2023-04-28 18:27:16.000000 pyjls-0.6.2/src/wr_fsr.c
+-rw-rw-rw-   0        0        0     9691 2023-04-26 14:57:54.000000 pyjls-0.6.2/src/wr_ts.c
+-rw-rw-rw-   0        0        0    30342 2023-04-26 12:23:06.000000 pyjls-0.6.2/src/writer.c
```

### Comparing `pyjls-0.6.1/CHANGELOG.md` & `pyjls-0.6.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 
 # CHANGELOG
 
 This file contains the list of changes made to the JLS project.
 
 
+## 0.6.2
+
+2023 Apr 28
+
+* Improved UTC read processing.
+* Added "--utc" option to info entry point.
+* Fixed incorrect NaNs in summary on write.
+* Added "export" pyjls entry point.
+
+
 ## 0.6.1
 
 2023 Apr 27
 
 * Added FSR support for missing and duplicate data.
 * Added FSR support for unaligned u1 and u4 data.
 * Improved log messages.
```

### Comparing `pyjls-0.6.1/CREDITS.html` & `pyjls-0.6.2/CREDITS.html`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/LICENSE` & `pyjls-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/PKG-INFO` & `pyjls-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjls
-Version: 0.6.1
+Version: 0.6.2
 Summary: Joulescope™ file format
 Home-page: https://joulescope.readthedocs.io
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/jetperch/jls/issues
 Project-URL: Funding, https://www.joulescope.com
```

### Comparing `pyjls-0.6.1/README.md` & `pyjls-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/include/jls/backend.h` & `pyjls-0.6.2/include/jls/backend.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/include/jls/cmacro.h` & `pyjls-0.6.2/include/jls/cmacro.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/include/jls/crc32c.h` & `pyjls-0.6.2/include/jls/crc32c.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/include/jls/ec.h` & `pyjls-0.6.2/include/jls/ec.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/include/jls/format.h` & `pyjls-0.6.2/include/jls/format.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/include/jls/log.h` & `pyjls-0.6.2/include/jls/log.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/include/jls/raw.h` & `pyjls-0.6.2/include/jls/raw.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/include/jls/reader.h` & `pyjls-0.6.2/include/jls/reader.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/include/jls/statistics.h` & `pyjls-0.6.2/include/jls/statistics.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/include/jls/threaded_writer.h` & `pyjls-0.6.2/include/jls/threaded_writer.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/include/jls/time.h` & `pyjls-0.6.2/include/jls/time.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/include/jls/version.h` & `pyjls-0.6.2/include/jls/version.h`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
  */
 
 JLS_CPP_GUARD_START
 
 // Use version_update.py to update.
 #define JLS_VERSION_MAJOR 0
 #define JLS_VERSION_MINOR 6
-#define JLS_VERSION_PATCH 1
+#define JLS_VERSION_PATCH 2
 
 /**
  * \brief Macro to encode version to uint32_t.
  *
  * \param major The major release number (0 to 255)
  * \param minor The minor release number (0 to 255)
  * \param patch The patch release number (0 to 65535)
```

### Comparing `pyjls-0.6.1/include/jls/writer.h` & `pyjls-0.6.2/include/jls/writer.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/include/jls.h` & `pyjls-0.6.2/include/jls.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/include_prv/jls/bit_shift.h` & `pyjls-0.6.2/include_prv/jls/bit_shift.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/include_prv/jls/cdef.h` & `pyjls-0.6.2/include_prv/jls/cdef.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/include_prv/jls/datatype.h` & `pyjls-0.6.2/include_prv/jls/datatype.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/include_prv/jls/msg_ring_buffer.h` & `pyjls-0.6.2/include_prv/jls/msg_ring_buffer.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/include_prv/jls/rd_fsr.h` & `pyjls-0.6.2/include_prv/jls/rd_fsr.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/include_prv/jls/util.h` & `pyjls-0.6.2/include_prv/jls/util.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/include_prv/jls/wr_fsr.h` & `pyjls-0.6.2/include_prv/jls/wr_fsr.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/include_prv/jls/wr_prv.h` & `pyjls-0.6.2/include_prv/jls/wr_prv.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/include_prv/jls/wr_ts.h` & `pyjls-0.6.2/include_prv/jls/wr_ts.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/pyjls/__init__.py` & `pyjls-0.6.2/pyjls/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/pyjls/__main__.py` & `pyjls-0.6.2/pyjls/__main__.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/pyjls/binding.c` & `pyjls-0.6.2/pyjls/binding.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/pyjls/entry_points/__init__.py` & `pyjls-0.6.2/pyjls/entry_points/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,13 +8,13 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from . import annotate, info
+from . import annotate, export, info
 
-__all__ = [annotate, info]
+__all__ = [annotate, export, info]
 """This list of available command modules.  Each module must contain a 
 parser_config(subparser) function.  The function must return the callable(args)
 that will be executed for the command."""
```

### Comparing `pyjls-0.6.1/pyjls/entry_points/annotate.py` & `pyjls-0.6.2/pyjls/entry_points/annotate.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/pyjls/entry_points/info.py` & `pyjls-0.6.2/pyjls/entry_points/info.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,14 +20,17 @@
 
 
 def parser_config(p):
     """JLS file info."""
     p.add_argument('--verbose', '-v',
                    action='store_true',
                    help='Display verbose information.')
+    p.add_argument('--utc',
+                   action='store_true',
+                   help='Display the UTC data for each channel.')
     p.add_argument('filename',
                    help='JLS filename')
     return on_cmd
 
 
 def _user_data_cbk(chunk_meta, data):
     suffix = ''
@@ -43,10 +46,16 @@
         for source in r.sources.values():
             s = source.info(verbose=args.verbose)
             print(textwrap.indent(s, "    "))
         print('Signals:')
         for signal in r.signals.values():
             s = signal.info(verbose=args.verbose)
             print(textwrap.indent(s, "    "))
+            if args.utc:
+                def on_utc(entries):
+                    for sample_id, timestamp in entries:
+                        print(f'       {sample_id}, {timestamp}')
+                r.utc(signal.signal_id, -signal.sample_rate, on_utc)
+
         print('User Data:')
         r.user_data(_user_data_cbk)
```

### Comparing `pyjls-0.6.1/pyjls/structs.py` & `pyjls-0.6.2/pyjls/structs.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,18 @@
     utc_decimate_factor: int = 100
     sample_id_offset: int = 0
     name: str = None
     units: str = None
     length: int = 0
 
     def info(self, verbose=None) -> str:
-        strs = [f'{self.signal_id}: {self.name}']
+        hdr = f'{self.signal_id}: {self.name}'
+        if self.signal_type == 0:
+            hdr += f' ({self.length} samples at {self.sample_rate} Hz)'
+        strs = [hdr]
         if verbose:
             for field in ['source_id', 'signal_type', 'data_type', 'sample_rate',
                           'samples_per_data', 'sample_decimate_factor',
                           'entries_per_summary', 'summary_decimate_factor',
                           'annotation_decimate_factor', 'utc_decimate_factor',
                           'sample_id_offset',
                           'units', 'length']:
```

### Comparing `pyjls-0.6.1/pyjls/test/__init__.py` & `pyjls-0.6.2/pyjls/test/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/pyjls/test/test_binding.py` & `pyjls-0.6.2/pyjls/test/test_binding.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/pyjls/v1/__init__.py` & `pyjls-0.6.2/pyjls/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/pyjls/version.py` & `pyjls-0.6.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-# Copyright 2021-2022 Jetperch LLC
+# Copyright 2022 Jetperch LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+# See https://peps.python.org/pep-0518/
+# See https://toml.io/
 
-__version__ = "0.6.1"
-
-__title__ = "pyjls"
-__description__ = 'Joulescope™ file format'
-__url__ = 'https://joulescope.readthedocs.io'
-__author__ = 'Jetperch LLC'
-__author_email__ = 'joulescope-dev@jetperch.com'
-__license__ = 'Apache 2.0'
-__copyright__ = 'Copyright 2021-2022 Jetperch LLC'
-
-__all__ = ['__version__', '__title__', '__description__', '__url__',
-           '__author__', '__author_email__', '__license__',
-           '__copyright__']
+[build-system]
+# Minimum requirements for the build system to execute.
+requires = [
+    "Cython",
+    "numpy",
+    "pywin32; sys_platform == 'win32'",
+    "setuptools",
+    "wheel",
+]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyjls-0.6.1/pyjls.egg-info/PKG-INFO` & `pyjls-0.6.2/pyjls.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjls
-Version: 0.6.1
+Version: 0.6.2
 Summary: Joulescope™ file format
 Home-page: https://joulescope.readthedocs.io
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/jetperch/jls/issues
 Project-URL: Funding, https://www.joulescope.com
```

### Comparing `pyjls-0.6.1/pyjls.egg-info/SOURCES.txt` & `pyjls-0.6.2/pyjls.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 pyjls.egg-info/SOURCES.txt
 pyjls.egg-info/dependency_links.txt
 pyjls.egg-info/entry_points.txt
 pyjls.egg-info/requires.txt
 pyjls.egg-info/top_level.txt
 pyjls/entry_points/__init__.py
 pyjls/entry_points/annotate.py
+pyjls/entry_points/export.py
 pyjls/entry_points/info.py
 pyjls/test/__init__.py
 pyjls/test/test_binding.py
 pyjls/v1/__init__.py
 src/backend_posix.c
 src/backend_win.c
 src/bit_shift.c
```

### Comparing `pyjls-0.6.1/setup.py` & `pyjls-0.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/src/backend_posix.c` & `pyjls-0.6.2/src/backend_posix.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/src/backend_win.c` & `pyjls-0.6.2/src/backend_win.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/src/bit_shift.c` & `pyjls-0.6.2/src/bit_shift.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/src/crc32c_arm_neon.c` & `pyjls-0.6.2/src/crc32c_arm_neon.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/src/crc32c_intel_sse4.c` & `pyjls-0.6.2/src/crc32c_intel_sse4.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/src/crc32c_sw.c` & `pyjls-0.6.2/src/crc32c_sw.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/src/datatype.c` & `pyjls-0.6.2/src/datatype.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/src/ec.c` & `pyjls-0.6.2/src/ec.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/src/log.c` & `pyjls-0.6.2/src/log.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/src/msg_ring_buffer.c` & `pyjls-0.6.2/src/msg_ring_buffer.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/src/raw.c` & `pyjls-0.6.2/src/raw.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/src/rd_fsr.c` & `pyjls-0.6.2/src/rd_fsr.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/src/reader.c` & `pyjls-0.6.2/src/reader.c`

 * *Files 0% similar despite different names*

```diff
@@ -1423,15 +1423,17 @@
     if (NULL != signal->rd_fsr) {
         return 0;
     }
     signal->rd_fsr = jls_rd_fsr_alloc(self->signal_def[signal_id].sample_rate);
     if (NULL == signal->rd_fsr) {
         return JLS_ERROR_NOT_ENOUGH_MEMORY;
     }
-    return jls_rd_utc(self, signal_id, 0, jls_rd_fsr_add_cbk, signal->rd_fsr);
+    int64_t sample_rate = self->signal_def[signal_id].sample_rate;
+    int64_t sample_start = -3600 * sample_rate;  // within the last hour
+    return jls_rd_utc(self, signal_id, sample_start, jls_rd_fsr_add_cbk, signal->rd_fsr);
 }
 
 int32_t jls_rd_sample_id_to_timestamp(struct jls_rd_s * self, uint16_t signal_id,
                                       int64_t sample_id, int64_t * timestamp) {
     ROE(utc_load(self, signal_id));
     return jls_rd_fsr_sample_id_to_timestamp(self->signals[signal_id].rd_fsr, sample_id, timestamp);
 }
```

### Comparing `pyjls-0.6.1/src/statistics.c` & `pyjls-0.6.2/src/statistics.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/src/threaded_writer.c` & `pyjls-0.6.2/src/threaded_writer.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/src/wr_fsr.c` & `pyjls-0.6.2/src/wr_fsr.c`

 * *Files 1% similar despite different names*

```diff
@@ -385,14 +385,15 @@
         double v_min = DBL_MAX;                                                             \
         double v_max = -DBL_MAX;                                                            \
         double v_var = 0.0;                                                                 \
         for (uint32_t sample = 0; sample < self->def.summary_decimate_factor; ++sample) {   \
             uint32_t offset = sample_idx * JLS_SUMMARY_FSR_COUNT;                           \
             v = src_data[offset + JLS_SUMMARY_FSR_MEAN];                                    \
             if (isfinite(v)) {                                                              \
+                ++count;                                                                    \
                 v_mean += v;                                                                \
                 if (src_data[offset + JLS_SUMMARY_FSR_MIN] < v_min) {                       \
                     v_min = src_data[offset + JLS_SUMMARY_FSR_MIN];                         \
                 }                                                                           \
                 if (src_data[offset + JLS_SUMMARY_FSR_MAX] > v_max) {                       \
                     v_max = src_data[offset + JLS_SUMMARY_FSR_MAX];                         \
                 }                                                                           \
@@ -629,16 +630,17 @@
                     ROE(wr_data_inner(self, self->buffer_u64, (uint32_t) entries));
                     data_u8 += sz - 1;
                 }
                 return 0;
             }
         }
     } else {
-        JLS_LOGW("fsr skip: in=%" PRIi64 " expect=%" PRIi64,
-                 sample_id, sample_id_next);
+        JLS_LOGW("fsr skip: in=%" PRIi64 " expect=%" PRIi64 ", skipped=%" PRIi64,
+                 sample_id, sample_id_next,
+                 sample_id - sample_id_next);
         size_t skip = (size_t) (sample_id - sample_id_next);
         size_t buf_sz = 0;
         if (self->def.data_type == JLS_DATATYPE_F32) {
             float * f32 = (float *) self->buffer_u64;
             buf_sz = sizeof(self->buffer_u64);
             buf_sz /= sizeof(float);
             for (size_t idx = 0; idx < buf_sz; ++idx) {
```

### Comparing `pyjls-0.6.1/src/wr_ts.c` & `pyjls-0.6.2/src/wr_ts.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.1/src/writer.c` & `pyjls-0.6.2/src/writer.c`

 * *Files identical despite different names*

