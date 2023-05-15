# Comparing `tmp/fstd2nc-0.20230328.0.tar.gz` & `tmp/fstd2nc-0.20230515.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fstd2nc-0.20230328.0.tar", last modified: Wed Mar 29 16:08:02 2023, max compression
+gzip compressed data, was "dist/fstd2nc-0.20230515.0.tar", last modified: Mon May 15 23:30:03 2023, max compression
```

## Comparing `fstd2nc-0.20230328.0.tar` & `fstd2nc-0.20230515.0.tar`

### file list

```diff
@@ -1,47 +1,59 @@
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-03-29 16:08:02.000000 fstd2nc-0.20230328.0/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     2432 2022-07-13 22:02:23.000000 fstd2nc-0.20230328.0/setup.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    16247 2023-03-29 16:08:02.000000 fstd2nc-0.20230328.0/PKG-INFO
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-03-29 16:08:02.000000 fstd2nc-0.20230328.0/fstd2nc.egg-info/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      930 2023-03-29 16:08:02.000000 fstd2nc-0.20230328.0/fstd2nc.egg-info/SOURCES.txt
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    16247 2023-03-29 16:08:02.000000 fstd2nc-0.20230328.0/fstd2nc.egg-info/PKG-INFO
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)        1 2023-03-29 16:08:02.000000 fstd2nc-0.20230328.0/fstd2nc.egg-info/dependency_links.txt
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)        8 2023-03-29 16:08:02.000000 fstd2nc-0.20230328.0/fstd2nc.egg-info/top_level.txt
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      107 2023-03-29 16:08:02.000000 fstd2nc-0.20230328.0/fstd2nc.egg-info/entry_points.txt
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      218 2023-03-29 16:08:02.000000 fstd2nc-0.20230328.0/fstd2nc.egg-info/requires.txt
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     7651 2022-04-13 02:52:23.000000 fstd2nc-0.20230328.0/COPYING.LESSER
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    35147 2022-04-13 02:52:23.000000 fstd2nc-0.20230328.0/COPYING
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-03-29 16:08:02.000000 fstd2nc-0.20230328.0/fstd2nc/
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-03-29 16:08:02.000000 fstd2nc-0.20230328.0/fstd2nc/locale/
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-03-29 16:08:02.000000 fstd2nc-0.20230328.0/fstd2nc/locale/fr_CA/
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-03-29 16:08:02.000000 fstd2nc-0.20230328.0/fstd2nc/locale/fr_CA/LC_MESSAGES/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    22475 2023-03-29 16:07:45.000000 fstd2nc-0.20230328.0/fstd2nc/locale/fr_CA/LC_MESSAGES/fstd2nc.mo
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3743 2023-03-28 22:16:16.000000 fstd2nc-0.20230328.0/fstd2nc/__init__.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    14256 2023-03-28 19:48:27.000000 fstd2nc-0.20230328.0/fstd2nc/extra.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     2583 2023-03-09 16:06:03.000000 fstd2nc-0.20230328.0/fstd2nc/stdout.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     9892 2023-02-22 19:45:21.000000 fstd2nc-0.20230328.0/fstd2nc/__main__.py
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-03-29 16:08:02.000000 fstd2nc-0.20230328.0/fstd2nc/mixins/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    14413 2023-03-27 15:06:10.000000 fstd2nc-0.20230328.0/fstd2nc/mixins/gridhacks.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    20231 2023-03-27 15:06:10.000000 fstd2nc-0.20230328.0/fstd2nc/mixins/compat.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3565 2023-03-09 23:44:53.000000 fstd2nc-0.20230328.0/fstd2nc/mixins/filter.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3130 2022-07-13 22:02:23.000000 fstd2nc-0.20230328.0/fstd2nc/mixins/ensembles.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1735 2022-11-15 20:24:37.000000 fstd2nc-0.20230328.0/fstd2nc/mixins/pruneaxes.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     4790 2023-02-22 19:45:21.000000 fstd2nc-0.20230328.0/fstd2nc/mixins/removestuff.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3138 2022-07-29 01:07:28.000000 fstd2nc-0.20230328.0/fstd2nc/mixins/diaghacks.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     5787 2022-11-23 20:43:24.000000 fstd2nc-0.20230328.0/fstd2nc/mixins/dates.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     6683 2023-02-22 19:45:21.000000 fstd2nc-0.20230328.0/fstd2nc/mixins/sfc_codes.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    29767 2023-03-27 15:06:10.000000 fstd2nc-0.20230328.0/fstd2nc/mixins/vcoords.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    34548 2023-03-27 15:06:10.000000 fstd2nc-0.20230328.0/fstd2nc/mixins/__init__.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     9719 2023-03-28 19:48:38.000000 fstd2nc-0.20230328.0/fstd2nc/mixins/fstd.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     4929 2022-07-13 22:02:23.000000 fstd2nc-0.20230328.0/fstd2nc/mixins/mesh.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     7339 2023-03-28 21:50:33.000000 fstd2nc-0.20230328.0/fstd2nc/mixins/vardict.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     7003 2023-03-28 19:48:27.000000 fstd2nc-0.20230328.0/fstd2nc/mixins/masks.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    14637 2023-03-27 15:06:10.000000 fstd2nc-0.20230328.0/fstd2nc/mixins/series.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1571 2022-07-13 22:02:23.000000 fstd2nc-0.20230328.0/fstd2nc/mixins/misc.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     2610 2022-11-18 18:26:52.000000 fstd2nc-0.20230328.0/fstd2nc/mixins/select.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    20686 2023-03-28 21:50:35.000000 fstd2nc-0.20230328.0/fstd2nc/mixins/netcdf.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    17324 2023-03-27 15:06:10.000000 fstd2nc-0.20230328.0/fstd2nc/mixins/extern.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1871 2023-02-22 19:45:21.000000 fstd2nc-0.20230328.0/fstd2nc/mixins/ascii.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    37534 2023-03-27 15:06:10.000000 fstd2nc-0.20230328.0/fstd2nc/mixins/xycoords.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)       38 2023-03-29 16:08:02.000000 fstd2nc-0.20230328.0/setup.cfg
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    13196 2023-02-22 19:45:21.000000 fstd2nc-0.20230328.0/README.md
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)       59 2022-12-28 20:25:42.000000 fstd2nc-0.20230328.0/pyproject.toml
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-15 23:30:03.451427 fstd2nc-0.20230515.0/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    35147 2022-04-13 02:52:23.000000 fstd2nc-0.20230515.0/COPYING
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     7651 2022-04-13 02:52:23.000000 fstd2nc-0.20230515.0/COPYING.LESSER
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    13943 2023-05-15 23:30:03.451173 fstd2nc-0.20230515.0/PKG-INFO
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    13196 2023-02-22 19:45:21.000000 fstd2nc-0.20230515.0/README.md
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-15 23:30:03.439498 fstd2nc-0.20230515.0/cccbuffer/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      777 2023-05-10 00:52:26.000000 fstd2nc-0.20230515.0/cccbuffer/__init__.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      182 2023-05-10 00:52:26.000000 fstd2nc-0.20230515.0/cccbuffer/__main__.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      149 2023-05-10 00:52:26.000000 fstd2nc-0.20230515.0/cccbuffer/cccdump.py
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-15 23:30:03.442374 fstd2nc-0.20230515.0/cccbuffer/mixins/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-10 00:52:26.000000 fstd2nc-0.20230515.0/cccbuffer/mixins/__init__.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3910 2023-05-10 00:52:26.000000 fstd2nc-0.20230515.0/cccbuffer/mixins/ccc.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1193 2023-05-10 00:52:26.000000 fstd2nc-0.20230515.0/cccbuffer/mixins/char.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     2289 2023-05-10 00:52:26.000000 fstd2nc-0.20230515.0/cccbuffer/mixins/grid.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     4359 2023-05-10 00:52:26.000000 fstd2nc-0.20230515.0/cccbuffer/mixins/levels.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3047 2023-05-10 00:52:26.000000 fstd2nc-0.20230515.0/cccbuffer/mixins/superlabels.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     6112 2023-05-10 00:52:26.000000 fstd2nc-0.20230515.0/cccbuffer/mixins/times.py
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-15 23:30:03.443501 fstd2nc-0.20230515.0/fstd2nc/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3743 2023-05-15 23:27:01.000000 fstd2nc-0.20230515.0/fstd2nc/__init__.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     9892 2023-04-12 22:40:03.000000 fstd2nc-0.20230515.0/fstd2nc/__main__.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    14256 2023-04-12 22:40:03.000000 fstd2nc-0.20230515.0/fstd2nc/extra.py
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-15 23:30:03.436426 fstd2nc-0.20230515.0/fstd2nc/locale/
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-15 23:30:03.436484 fstd2nc-0.20230515.0/fstd2nc/locale/fr_CA/
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-15 23:30:03.445032 fstd2nc-0.20230515.0/fstd2nc/locale/fr_CA/LC_MESSAGES/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    22410 2023-05-15 23:29:20.000000 fstd2nc-0.20230515.0/fstd2nc/locale/fr_CA/LC_MESSAGES/fstd2nc.mo
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-15 23:30:03.450803 fstd2nc-0.20230515.0/fstd2nc/mixins/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    35585 2023-05-15 23:00:04.000000 fstd2nc-0.20230515.0/fstd2nc/mixins/__init__.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1871 2023-04-12 22:40:04.000000 fstd2nc-0.20230515.0/fstd2nc/mixins/ascii.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    20216 2023-05-10 00:52:26.000000 fstd2nc-0.20230515.0/fstd2nc/mixins/compat.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     5787 2023-05-15 23:00:04.000000 fstd2nc-0.20230515.0/fstd2nc/mixins/dates.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3138 2023-04-12 22:40:03.000000 fstd2nc-0.20230515.0/fstd2nc/mixins/diaghacks.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3130 2023-04-12 22:40:03.000000 fstd2nc-0.20230515.0/fstd2nc/mixins/ensembles.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    19350 2023-05-15 23:00:04.000000 fstd2nc-0.20230515.0/fstd2nc/mixins/extern.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3565 2023-04-12 22:40:03.000000 fstd2nc-0.20230515.0/fstd2nc/mixins/filter.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     9126 2023-05-10 00:52:26.000000 fstd2nc-0.20230515.0/fstd2nc/mixins/fstd.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    15447 2023-05-10 00:52:26.000000 fstd2nc-0.20230515.0/fstd2nc/mixins/gridhacks.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     7119 2023-05-10 00:52:26.000000 fstd2nc-0.20230515.0/fstd2nc/mixins/masks.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     4929 2023-04-12 22:40:04.000000 fstd2nc-0.20230515.0/fstd2nc/mixins/mesh.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1571 2023-04-12 22:40:04.000000 fstd2nc-0.20230515.0/fstd2nc/mixins/misc.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    20811 2023-05-10 00:52:26.000000 fstd2nc-0.20230515.0/fstd2nc/mixins/netcdf.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1735 2023-04-12 22:40:03.000000 fstd2nc-0.20230515.0/fstd2nc/mixins/pruneaxes.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     4790 2023-04-12 22:40:03.000000 fstd2nc-0.20230515.0/fstd2nc/mixins/removestuff.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     2610 2023-04-12 22:40:04.000000 fstd2nc-0.20230515.0/fstd2nc/mixins/select.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    14637 2023-04-12 22:40:04.000000 fstd2nc-0.20230515.0/fstd2nc/mixins/series.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     6683 2023-04-12 22:40:03.000000 fstd2nc-0.20230515.0/fstd2nc/mixins/sfc_codes.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     7339 2023-04-12 22:40:04.000000 fstd2nc-0.20230515.0/fstd2nc/mixins/vardict.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    32765 2023-04-13 18:26:53.000000 fstd2nc-0.20230515.0/fstd2nc/mixins/vcoords.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    37809 2023-05-15 23:00:04.000000 fstd2nc-0.20230515.0/fstd2nc/mixins/xycoords.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     2583 2023-04-12 22:40:03.000000 fstd2nc-0.20230515.0/fstd2nc/stdout.py
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-15 23:30:03.444792 fstd2nc-0.20230515.0/fstd2nc.egg-info/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    13943 2023-05-15 23:30:02.000000 fstd2nc-0.20230515.0/fstd2nc.egg-info/PKG-INFO
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1183 2023-05-15 23:30:03.444001 fstd2nc-0.20230515.0/fstd2nc.egg-info/SOURCES.txt
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)        1 2023-05-15 23:30:02.000000 fstd2nc-0.20230515.0/fstd2nc.egg-info/dependency_links.txt
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      170 2023-05-15 23:30:03.444396 fstd2nc-0.20230515.0/fstd2nc.egg-info/entry_points.txt
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      218 2023-05-15 23:30:03.444605 fstd2nc-0.20230515.0/fstd2nc.egg-info/requires.txt
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)       18 2023-05-15 23:30:03.444833 fstd2nc-0.20230515.0/fstd2nc.egg-info/top_level.txt
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)       59 2022-12-28 20:25:42.000000 fstd2nc-0.20230515.0/pyproject.toml
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)       38 2023-05-15 23:30:03.451490 fstd2nc-0.20230515.0/setup.cfg
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     2514 2023-05-10 00:52:26.000000 fstd2nc-0.20230515.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `fstd2nc-0.20230328.0/setup.py` & `fstd2nc-0.20230515.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2021 - Climate Research Division
+# Copyright 2017-2023 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
@@ -54,12 +54,14 @@
   package_data = {
     'fstd2nc': ['locale/*/LC_MESSAGES/fstd2nc.mo'],
   },
   entry_points={
     'console_scripts': [
       'fstd2nc = fstd2nc.__main__:_fstd2nc_cmdline_trapped',
       'fstdump = fstd2nc.__main__:_fstdump',
+      'ccc2nc = cccbuffer.__main__:run',
+      'cccdump = cccbuffer.cccdump:run',
     ],
   },
 
 )
```

### Comparing `fstd2nc-0.20230328.0/PKG-INFO` & `fstd2nc-0.20230515.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,313 +1,293 @@
-Metadata-Version: 2.1
-Name: fstd2nc
-Version: 0.20230328.0
-Summary: Converts RPN standard files (from Environment Canada) to netCDF files.
-Home-page: https://github.com/neishm/fstd2nc
-Author: Mike Neish
-License: LGPL-3
-Description: [Version française](README_fr.md)
-        
-        Overview
-        ========
-        This module provides a mechanism for converting between FSTD and netCDF file formats, either through Python or the command-line.
-        
-        
-        Installing
-        ==========
-        
-        The easiest way to install is using [pip](https://pip.pypa.io/en/stable):
-        ```
-        pip install fstd2nc
-        ```
-        
-        
-        Basic Usage
-        ===========
-        
-        From the command-line
-        ---------------------
-        ```
-        python -m fstd2nc [options] <infile(s)> <outfile>
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          --version             show program's version number and exit
-          --no-progress         Disable the progress bar.
-          --serial              Disables multithreading/multiprocessing. Useful for
-                                resource-limited machines.
-          --minimal-metadata    Don't include internal record attributes and other
-                                internal information in the output metadata. This is
-                                the default behaviour.
-          --internal-metadata, --rpnstd-metadata
-                                Include all internal record attributes in the output
-                                metadata.
-          --metadata-list nomvar,..., --rpnstd-metadata-list nomvar,...
-                                Specify a minimal set of internal record attributes to
-                                include in the output file.
-          --ignore-typvar       Tells the converter to ignore the typvar when deciding
-                                if two records are part of the same field. Default is
-                                to split the variable on different typvars.
-          --ignore-etiket       Tells the converter to ignore the etiket when deciding
-                                if two records are part of the same field. Default is
-                                to split the variable on different etikets.
-          --vars VAR1,VAR2,...  Comma-separated list of variables to convert. By
-                                default, all variables are converted.
-          --fill-value FILL_VALUE
-                                The fill value to use for masked (missing) data. Gets
-                                stored as '_FillValue' attribute in the metadata.
-                                Default is '1e+30'.
-          --datev, --squash-forecasts
-                                Use the date of validity for the "time" axis. This is
-                                the default.
-          --dateo, --forecast-axis
-                                Use the date of original analysis for the time axis,
-                                and put the forecast times into a separate "forecast"
-                                axis.
-          --ensembles           Collect different etikets for the same variable
-                                together into an "ensemble" axis.
-          --profile-momentum-vars VAR1,VAR2,...
-                                Comma-separated list of variables that use momentum
-                                levels.
-          --profile-thermodynamic-vars VAR1,VAR2,...
-                                Comma-separated list of variables that use
-                                thermodynamic levels.
-          --missing-bottom-profile-level
-                                Assume the bottom level of the profile data is
-                                missing.
-          --vardict VARDICT     Use metadata from the specified variable dictionary
-                                (XML format).
-          --opdict              Similar to above, but use the standard CMC-RPN
-                                operational dictionary.
-          --sfc-agg-vars NAME,NAME,...
-                                Define additional surface aggregate fields.
-          --soil-depths SOIL_DEPTHS
-                                Define custom depths for soil fields (WSOL,ISOL).
-                                Defaults are 0.05,0.1,0.2,0.4,1.0,2.0,3.0.
-          --strict-vcoord-match
-                                Require the IP1/IP2/IP3 parameters of the vertical
-                                coordinate to match the IG1/IG2/IG3 paramters of the
-                                field in order to be used. The default behaviour is to
-                                use the vertical record anyway if it's the only one in
-                                the file.
-          --diag-as-model-level
-                                Treat diagnostic (near-surface) data as model level
-                                '1.0'. This is the default behaviour.
-          --split-diag-level    Put the diagnostic (near-surface) data in a separate
-                                variable, away from the 3D model output. Suffices will
-                                be added to distinguish the different types of levels
-                                (i.e. _diag_level and _model_levels for diagnostic
-                                height and hybrid levels respectively).
-          --ignore-diag-level   Ignore data on diagnostic (near-surface) height.
-          --only-diag-level     Only use the diagnostic (near-surface) height,
-                                ignoring other atmospheric levels.
-          --thermodynamic-levels, --tlev
-                                Only convert data that's on 'thermodynamic' vertical
-                                levels.
-          --momentum-levels, --mlev
-                                Only convert data that's on 'momentum' vertical
-                                levels.
-          --vertical-velocity-levels, --wlev
-                                Only convert data that's on 'vertical velocity'
-                                levels.
-          --subgrid-axis        For data on supergrids, split the subgrids along a
-                                "subgrid" axis. The default is to leave the subgrids
-                                stacked together as they are in the RPN file.
-          --keep-LA-LO          Include LA and LO records, even if they appear to be
-                                redundant.
-          --no-adjust-rlon      For rotated grids, do NOT adjust rlon coordinate to
-                                keep the range in -180..180. Allow the rlon value to
-                                be whatever librmn says it should be.
-          --bounds              Include grid cell boundaries in the output.
-          --filter CONDITION    Subset RPN standard file records using the given
-                                criteria. For example, to convert only 24-hour
-                                forecasts you could use --filter ip2==24
-          --exclude NAME,NAME,...
-                                Exclude some axes, attributes, or derived variables
-                                from the output. For instance, excluding
-                                'leadtime,reftime' can help for netCDF tools that
-                                don't recognize leadtime and reftime as valid
-                                coordinates. Note that axes will only be excluded if
-                                they have a length of 1.
-          --yin                 Select first subgrid from a supergrid.
-          --yang                Select second subgrid from a supergrid.
-          --crop-to-smallest-grid
-                                Crop grids to the smaller (inner core) domain for LAM
-                                outputs.
-          --metadata-file METADATA_FILE
-                                Use metadata from the specified file. You can repeat
-                                this option multiple times to build metadata from
-                                different sources.
-          --rename OLDNAME=NEWNAME,...
-                                Apply the specified name changes to the variables.
-          --conventions CONVENTIONS
-                                Set the "Conventions" attribute for the netCDF file.
-                                Default is "CF-1.6". Note that this has no effect on
-                                the structure of the file.
-          --no-conventions      Omit the "Conventions" attribute from the netCDF file
-                                entirely. This can help for netCDF tools that have
-                                trouble recognizing the CF conventions encoded in the
-                                file.
-          --time-units {seconds,minutes,hours,days}
-                                The units for the output time axis. Default is hours.
-          --reference-date YYYY-MM-DD
-                                The reference date for the output time axis. The
-                                default is the starting date in the RPN standard file.
-          --fstd-compat         Adds a compatibility layer to the netCDF output file,
-                                so it can also function as a valid FSTD file.
-                                EXPERIMENTAL.
-          --msglvl {0,DEBUG,2,INFORM,4,WARNIN,6,ERRORS,8,FATALE,10,SYSTEM,CATAST}
-                                How much information to print to stdout during the
-                                conversion. Default is WARNIN.
-          --nc-format {NETCDF4,NETCDF4_CLASSIC,NETCDF3_CLASSIC,NETCDF3_64BIT_OFFSET,NETCDF3_64BIT_DATA}
-                                Which variant of netCDF to write. Default is NETCDF4.
-          --zlib                Turn on compression for the netCDF file. Only works
-                                for NETCDF4 and NETCDF4_CLASSIC formats.
-          --compression COMPRESSION
-                                Compression level for the netCDF file. Only used if
-                                --zlib is set. Default: 4.
-          -f, --force           Overwrite the output file if it already exists.
-          --no-history          Don't put the command-line invocation in the netCDF
-                                metadata.
-          -q, --quiet           Don't display any information except for critical
-                                error messages. Implies --no-progress.
-        ```
-        
-        Using in a Python script
-        ========================
-        
-        Simple conversion
-        --------------------------------------
-        ```python
-        import fstd2nc
-        data = fstd2nc.Buffer("myfile.fst")
-        data.to_netcdf("myfile.nc")
-        ```
-        
-        You can control `fstd2nc.Buffer` using parameters similar to the command-line arguments.  The convention is that *--arg-name* from the command-line would be passed as *arg_name* from Python.
-        
-        For example:
-        ```python
-        import fstd2nc
-        # Select only TT,HU variables.
-        data = fstd2nc.Buffer("myfile.fst", vars=['TT','HU'])
-        # Set the reference date to Jan 1, 2000 in the netCDF file.
-        data.to_netcdf("myfile.nc", reference_date='2000-01-01')
-        ```
-        
-        Interfacing with xarray
-        ---------------------------------------------------------------------------------
-        
-        For more complicated conversions, you can manipulate the data as an [xarray.Dataset](http://xarray.pydata.org/en/stable/data-structures.html#dataset) object by using the `to_xarray()` method:
-        ```python
-        import fstd2nc
-        
-        # Open the FSTD file.
-        data = fstd2nc.Buffer("myfile.fst")
-        
-        # Access the data as an xarray.Dataset object.
-        dataset = data.to_xarray()
-        print (dataset)
-        
-        # Convert surface pressure to Pa.
-        dataset['P0'] *= 100
-        dataset['P0'].attrs['units'] = 'Pa'
-        
-        # (Can further manipulate the dataset here)
-        # ...
-        
-        # Write the final result to netCDF using xarray:
-        dataset.to_netcdf("myfile.nc")
-        ```
-        
-        Interfacing with iris
-        ---------------------------------------------------------------------------------
-        
-        You can interface with [iris](https://scitools.org.uk/iris/docs/latest/index.html) by using the `.to_iris()` method (requires iris version 2.0 or greater).
-        This will give you an [iris.cube.CubeList](https://scitools.org.uk/iris/docs/latest/iris/iris/cube.html#iris.cube.CubeList) object:
-        ```python
-        import fstd2nc
-        import iris.quickplot as qp
-        from matplotlib import pyplot as pl
-        
-        # Open the FSTD file.
-        data = fstd2nc.Buffer("myfile.fst")
-        
-        # Access the data as an iris.cube.CubeList object.
-        cubes = data.to_iris()
-        print (cubes)
-        
-        # Plot all the data (assuming we have 2D fields)
-        for cube in cubes:
-          qp.contourf(cube)
-          pl.gca().coastlines()
-        
-        pl.show()
-        ```
-        
-        Interfacing with pygeode
-        ---------------------------------------------------------------------------------
-        
-        You can create a [pygeode.Dataset](http://pygeode.github.io/dataset.html) object using the `.to_pygeode()` method (requires pygeode version 1.2.2 or greater):
-        ```python
-        import fstd2nc
-        
-        # Open the FSTD file.
-        data = fstd2nc.Buffer("myfile.fst")
-        
-        # Access the data as a pygeode.Dataset object.
-        dataset = data.to_pygeode()
-        print (dataset)
-        ```
-        
-        Interfacing with fstpy
-        ---------------------------------------------------------------------------------
-        
-        You can load data from an [fstpy](https://gitlab.science.gc.ca/CMDS/fstpy) table using the `.from_fstpy()` method (requires fstpy version 2.1.9 or greater):
-        ```python
-        import fstd2nc
-        import fstpy
-        table = fstpy.StandardFileReader('myfile.fst').to_pandas()
-        data = fstd2nc.Buffer.from_fstpy(table)
-        ```
-        You can also export to an fstpy table using the `.to_fstpy()` method:
-        ```python
-        import fstd2nc
-        table = fstd2nc.Buffer('myfile.fst').to_fstpy()
-        ```
-        
-        
-        Requirements
-        ============
-        
-        Basic requirements
-        --------------------
-        
-        This package requires [Python-RPN](https://github.com/meteokid/python-rpn) for reading/writing FSTD files, and [netcdf4-python](https://github.com/Unidata/netcdf4-python) for reading/writing netCDF files.
-        
-        Optional dependencies
-        ---------------------
-        
-        A useful variable dictionary for the `--vardict` option is available [here](https://collaboration.cmc.ec.gc.ca/cmc/CMOI/VariableDictionary/).
-        
-        For reading large numbers of input files (>100), this utility can leverage [pandas](https://github.com/pandas-dev/pandas) to quickly process the FSTD record headers.
-        
-        The `.to_xarray()` Python method requires the [xarray](https://github.com/pydata/xarray) and [dask](https://github.com/dask/dask) packages.
-        
-        The `.to_iris()` Python method requires the [iris](https://scitools.org.uk/iris/docs/latest/index.html) package, along with the `.to_xarray()` dependencies.
-        
-        The `.to_pygeode()` Python method requires the [pygeode](https://github.com/pygeode/pygeode) package, along with the `.to_xarray()` dependencies.
-        
-        The `.to_fstpy()` Python method requires the [fstpy](https://gitlab.science.gc.ca/CMDS/fstpy) package (*internal link*).
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Programming Language :: Python
-Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
-Description-Content-Type: text/markdown
-Provides-Extra: iris
-Provides-Extra: manyfiles
-Provides-Extra: pygeode
-Provides-Extra: array
+[Version française](README_fr.md)
+
+Overview
+========
+This module provides a mechanism for converting between FSTD and netCDF file formats, either through Python or the command-line.
+
+
+Installing
+==========
+
+The easiest way to install is using [pip](https://pip.pypa.io/en/stable):
+```
+pip install fstd2nc
+```
+
+
+Basic Usage
+===========
+
+From the command-line
+---------------------
+```
+python -m fstd2nc [options] <infile(s)> <outfile>
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --version             show program's version number and exit
+  --no-progress         Disable the progress bar.
+  --serial              Disables multithreading/multiprocessing. Useful for
+                        resource-limited machines.
+  --minimal-metadata    Don't include internal record attributes and other
+                        internal information in the output metadata. This is
+                        the default behaviour.
+  --internal-metadata, --rpnstd-metadata
+                        Include all internal record attributes in the output
+                        metadata.
+  --metadata-list nomvar,..., --rpnstd-metadata-list nomvar,...
+                        Specify a minimal set of internal record attributes to
+                        include in the output file.
+  --ignore-typvar       Tells the converter to ignore the typvar when deciding
+                        if two records are part of the same field. Default is
+                        to split the variable on different typvars.
+  --ignore-etiket       Tells the converter to ignore the etiket when deciding
+                        if two records are part of the same field. Default is
+                        to split the variable on different etikets.
+  --vars VAR1,VAR2,...  Comma-separated list of variables to convert. By
+                        default, all variables are converted.
+  --fill-value FILL_VALUE
+                        The fill value to use for masked (missing) data. Gets
+                        stored as '_FillValue' attribute in the metadata.
+                        Default is '1e+30'.
+  --datev, --squash-forecasts
+                        Use the date of validity for the "time" axis. This is
+                        the default.
+  --dateo, --forecast-axis
+                        Use the date of original analysis for the time axis,
+                        and put the forecast times into a separate "forecast"
+                        axis.
+  --ensembles           Collect different etikets for the same variable
+                        together into an "ensemble" axis.
+  --profile-momentum-vars VAR1,VAR2,...
+                        Comma-separated list of variables that use momentum
+                        levels.
+  --profile-thermodynamic-vars VAR1,VAR2,...
+                        Comma-separated list of variables that use
+                        thermodynamic levels.
+  --missing-bottom-profile-level
+                        Assume the bottom level of the profile data is
+                        missing.
+  --vardict VARDICT     Use metadata from the specified variable dictionary
+                        (XML format).
+  --opdict              Similar to above, but use the standard CMC-RPN
+                        operational dictionary.
+  --sfc-agg-vars NAME,NAME,...
+                        Define additional surface aggregate fields.
+  --soil-depths SOIL_DEPTHS
+                        Define custom depths for soil fields (WSOL,ISOL).
+                        Defaults are 0.05,0.1,0.2,0.4,1.0,2.0,3.0.
+  --strict-vcoord-match
+                        Require the IP1/IP2/IP3 parameters of the vertical
+                        coordinate to match the IG1/IG2/IG3 paramters of the
+                        field in order to be used. The default behaviour is to
+                        use the vertical record anyway if it's the only one in
+                        the file.
+  --diag-as-model-level
+                        Treat diagnostic (near-surface) data as model level
+                        '1.0'. This is the default behaviour.
+  --split-diag-level    Put the diagnostic (near-surface) data in a separate
+                        variable, away from the 3D model output. Suffices will
+                        be added to distinguish the different types of levels
+                        (i.e. _diag_level and _model_levels for diagnostic
+                        height and hybrid levels respectively).
+  --ignore-diag-level   Ignore data on diagnostic (near-surface) height.
+  --only-diag-level     Only use the diagnostic (near-surface) height,
+                        ignoring other atmospheric levels.
+  --thermodynamic-levels, --tlev
+                        Only convert data that's on 'thermodynamic' vertical
+                        levels.
+  --momentum-levels, --mlev
+                        Only convert data that's on 'momentum' vertical
+                        levels.
+  --vertical-velocity-levels, --wlev
+                        Only convert data that's on 'vertical velocity'
+                        levels.
+  --subgrid-axis        For data on supergrids, split the subgrids along a
+                        "subgrid" axis. The default is to leave the subgrids
+                        stacked together as they are in the RPN file.
+  --keep-LA-LO          Include LA and LO records, even if they appear to be
+                        redundant.
+  --no-adjust-rlon      For rotated grids, do NOT adjust rlon coordinate to
+                        keep the range in -180..180. Allow the rlon value to
+                        be whatever librmn says it should be.
+  --bounds              Include grid cell boundaries in the output.
+  --filter CONDITION    Subset RPN standard file records using the given
+                        criteria. For example, to convert only 24-hour
+                        forecasts you could use --filter ip2==24
+  --exclude NAME,NAME,...
+                        Exclude some axes, attributes, or derived variables
+                        from the output. For instance, excluding
+                        'leadtime,reftime' can help for netCDF tools that
+                        don't recognize leadtime and reftime as valid
+                        coordinates. Note that axes will only be excluded if
+                        they have a length of 1.
+  --yin                 Select first subgrid from a supergrid.
+  --yang                Select second subgrid from a supergrid.
+  --crop-to-smallest-grid
+                        Crop grids to the smaller (inner core) domain for LAM
+                        outputs.
+  --metadata-file METADATA_FILE
+                        Use metadata from the specified file. You can repeat
+                        this option multiple times to build metadata from
+                        different sources.
+  --rename OLDNAME=NEWNAME,...
+                        Apply the specified name changes to the variables.
+  --conventions CONVENTIONS
+                        Set the "Conventions" attribute for the netCDF file.
+                        Default is "CF-1.6". Note that this has no effect on
+                        the structure of the file.
+  --no-conventions      Omit the "Conventions" attribute from the netCDF file
+                        entirely. This can help for netCDF tools that have
+                        trouble recognizing the CF conventions encoded in the
+                        file.
+  --time-units {seconds,minutes,hours,days}
+                        The units for the output time axis. Default is hours.
+  --reference-date YYYY-MM-DD
+                        The reference date for the output time axis. The
+                        default is the starting date in the RPN standard file.
+  --fstd-compat         Adds a compatibility layer to the netCDF output file,
+                        so it can also function as a valid FSTD file.
+                        EXPERIMENTAL.
+  --msglvl {0,DEBUG,2,INFORM,4,WARNIN,6,ERRORS,8,FATALE,10,SYSTEM,CATAST}
+                        How much information to print to stdout during the
+                        conversion. Default is WARNIN.
+  --nc-format {NETCDF4,NETCDF4_CLASSIC,NETCDF3_CLASSIC,NETCDF3_64BIT_OFFSET,NETCDF3_64BIT_DATA}
+                        Which variant of netCDF to write. Default is NETCDF4.
+  --zlib                Turn on compression for the netCDF file. Only works
+                        for NETCDF4 and NETCDF4_CLASSIC formats.
+  --compression COMPRESSION
+                        Compression level for the netCDF file. Only used if
+                        --zlib is set. Default: 4.
+  -f, --force           Overwrite the output file if it already exists.
+  --no-history          Don't put the command-line invocation in the netCDF
+                        metadata.
+  -q, --quiet           Don't display any information except for critical
+                        error messages. Implies --no-progress.
+```
+
+Using in a Python script
+========================
+
+Simple conversion
+--------------------------------------
+```python
+import fstd2nc
+data = fstd2nc.Buffer("myfile.fst")
+data.to_netcdf("myfile.nc")
+```
+
+You can control `fstd2nc.Buffer` using parameters similar to the command-line arguments.  The convention is that *--arg-name* from the command-line would be passed as *arg_name* from Python.
+
+For example:
+```python
+import fstd2nc
+# Select only TT,HU variables.
+data = fstd2nc.Buffer("myfile.fst", vars=['TT','HU'])
+# Set the reference date to Jan 1, 2000 in the netCDF file.
+data.to_netcdf("myfile.nc", reference_date='2000-01-01')
+```
+
+Interfacing with xarray
+---------------------------------------------------------------------------------
+
+For more complicated conversions, you can manipulate the data as an [xarray.Dataset](http://xarray.pydata.org/en/stable/data-structures.html#dataset) object by using the `to_xarray()` method:
+```python
+import fstd2nc
+
+# Open the FSTD file.
+data = fstd2nc.Buffer("myfile.fst")
+
+# Access the data as an xarray.Dataset object.
+dataset = data.to_xarray()
+print (dataset)
+
+# Convert surface pressure to Pa.
+dataset['P0'] *= 100
+dataset['P0'].attrs['units'] = 'Pa'
+
+# (Can further manipulate the dataset here)
+# ...
+
+# Write the final result to netCDF using xarray:
+dataset.to_netcdf("myfile.nc")
+```
+
+Interfacing with iris
+---------------------------------------------------------------------------------
+
+You can interface with [iris](https://scitools.org.uk/iris/docs/latest/index.html) by using the `.to_iris()` method (requires iris version 2.0 or greater).
+This will give you an [iris.cube.CubeList](https://scitools.org.uk/iris/docs/latest/iris/iris/cube.html#iris.cube.CubeList) object:
+```python
+import fstd2nc
+import iris.quickplot as qp
+from matplotlib import pyplot as pl
+
+# Open the FSTD file.
+data = fstd2nc.Buffer("myfile.fst")
+
+# Access the data as an iris.cube.CubeList object.
+cubes = data.to_iris()
+print (cubes)
+
+# Plot all the data (assuming we have 2D fields)
+for cube in cubes:
+  qp.contourf(cube)
+  pl.gca().coastlines()
+
+pl.show()
+```
+
+Interfacing with pygeode
+---------------------------------------------------------------------------------
+
+You can create a [pygeode.Dataset](http://pygeode.github.io/dataset.html) object using the `.to_pygeode()` method (requires pygeode version 1.2.2 or greater):
+```python
+import fstd2nc
+
+# Open the FSTD file.
+data = fstd2nc.Buffer("myfile.fst")
+
+# Access the data as a pygeode.Dataset object.
+dataset = data.to_pygeode()
+print (dataset)
+```
+
+Interfacing with fstpy
+---------------------------------------------------------------------------------
+
+You can load data from an [fstpy](https://gitlab.science.gc.ca/CMDS/fstpy) table using the `.from_fstpy()` method (requires fstpy version 2.1.9 or greater):
+```python
+import fstd2nc
+import fstpy
+table = fstpy.StandardFileReader('myfile.fst').to_pandas()
+data = fstd2nc.Buffer.from_fstpy(table)
+```
+You can also export to an fstpy table using the `.to_fstpy()` method:
+```python
+import fstd2nc
+table = fstd2nc.Buffer('myfile.fst').to_fstpy()
+```
+
+
+Requirements
+============
+
+Basic requirements
+--------------------
+
+This package requires [Python-RPN](https://github.com/meteokid/python-rpn) for reading/writing FSTD files, and [netcdf4-python](https://github.com/Unidata/netcdf4-python) for reading/writing netCDF files.
+
+Optional dependencies
+---------------------
+
+A useful variable dictionary for the `--vardict` option is available [here](https://collaboration.cmc.ec.gc.ca/cmc/CMOI/VariableDictionary/).
+
+For reading large numbers of input files (>100), this utility can leverage [pandas](https://github.com/pandas-dev/pandas) to quickly process the FSTD record headers.
+
+The `.to_xarray()` Python method requires the [xarray](https://github.com/pydata/xarray) and [dask](https://github.com/dask/dask) packages.
+
+The `.to_iris()` Python method requires the [iris](https://scitools.org.uk/iris/docs/latest/index.html) package, along with the `.to_xarray()` dependencies.
+
+The `.to_pygeode()` Python method requires the [pygeode](https://github.com/pygeode/pygeode) package, along with the `.to_xarray()` dependencies.
+
+The `.to_fstpy()` Python method requires the [fstpy](https://gitlab.science.gc.ca/CMDS/fstpy) package (*internal link*).
```

### Comparing `fstd2nc-0.20230328.0/fstd2nc.egg-info/SOURCES.txt` & `fstd2nc-0.20230515.0/fstd2nc.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 COPYING
 COPYING.LESSER
 README.md
 pyproject.toml
 setup.py
+cccbuffer/__init__.py
+cccbuffer/__main__.py
+cccbuffer/cccdump.py
+cccbuffer/mixins/__init__.py
+cccbuffer/mixins/ccc.py
+cccbuffer/mixins/char.py
+cccbuffer/mixins/grid.py
+cccbuffer/mixins/levels.py
+cccbuffer/mixins/superlabels.py
+cccbuffer/mixins/times.py
 fstd2nc/__init__.py
 fstd2nc/__main__.py
 fstd2nc/extra.py
 fstd2nc/stdout.py
 fstd2nc.egg-info/PKG-INFO
 fstd2nc.egg-info/SOURCES.txt
 fstd2nc.egg-info/dependency_links.txt
```

### Comparing `fstd2nc-0.20230328.0/fstd2nc.egg-info/PKG-INFO` & `fstd2nc-0.20230515.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,313 +1,317 @@
 Metadata-Version: 2.1
 Name: fstd2nc
-Version: 0.20230328.0
+Version: 0.20230515.0
 Summary: Converts RPN standard files (from Environment Canada) to netCDF files.
 Home-page: https://github.com/neishm/fstd2nc
 Author: Mike Neish
 License: LGPL-3
-Description: [Version française](README_fr.md)
-        
-        Overview
-        ========
-        This module provides a mechanism for converting between FSTD and netCDF file formats, either through Python or the command-line.
-        
-        
-        Installing
-        ==========
-        
-        The easiest way to install is using [pip](https://pip.pypa.io/en/stable):
-        ```
-        pip install fstd2nc
-        ```
-        
-        
-        Basic Usage
-        ===========
-        
-        From the command-line
-        ---------------------
-        ```
-        python -m fstd2nc [options] <infile(s)> <outfile>
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          --version             show program's version number and exit
-          --no-progress         Disable the progress bar.
-          --serial              Disables multithreading/multiprocessing. Useful for
-                                resource-limited machines.
-          --minimal-metadata    Don't include internal record attributes and other
-                                internal information in the output metadata. This is
-                                the default behaviour.
-          --internal-metadata, --rpnstd-metadata
-                                Include all internal record attributes in the output
-                                metadata.
-          --metadata-list nomvar,..., --rpnstd-metadata-list nomvar,...
-                                Specify a minimal set of internal record attributes to
-                                include in the output file.
-          --ignore-typvar       Tells the converter to ignore the typvar when deciding
-                                if two records are part of the same field. Default is
-                                to split the variable on different typvars.
-          --ignore-etiket       Tells the converter to ignore the etiket when deciding
-                                if two records are part of the same field. Default is
-                                to split the variable on different etikets.
-          --vars VAR1,VAR2,...  Comma-separated list of variables to convert. By
-                                default, all variables are converted.
-          --fill-value FILL_VALUE
-                                The fill value to use for masked (missing) data. Gets
-                                stored as '_FillValue' attribute in the metadata.
-                                Default is '1e+30'.
-          --datev, --squash-forecasts
-                                Use the date of validity for the "time" axis. This is
-                                the default.
-          --dateo, --forecast-axis
-                                Use the date of original analysis for the time axis,
-                                and put the forecast times into a separate "forecast"
-                                axis.
-          --ensembles           Collect different etikets for the same variable
-                                together into an "ensemble" axis.
-          --profile-momentum-vars VAR1,VAR2,...
-                                Comma-separated list of variables that use momentum
-                                levels.
-          --profile-thermodynamic-vars VAR1,VAR2,...
-                                Comma-separated list of variables that use
-                                thermodynamic levels.
-          --missing-bottom-profile-level
-                                Assume the bottom level of the profile data is
-                                missing.
-          --vardict VARDICT     Use metadata from the specified variable dictionary
-                                (XML format).
-          --opdict              Similar to above, but use the standard CMC-RPN
-                                operational dictionary.
-          --sfc-agg-vars NAME,NAME,...
-                                Define additional surface aggregate fields.
-          --soil-depths SOIL_DEPTHS
-                                Define custom depths for soil fields (WSOL,ISOL).
-                                Defaults are 0.05,0.1,0.2,0.4,1.0,2.0,3.0.
-          --strict-vcoord-match
-                                Require the IP1/IP2/IP3 parameters of the vertical
-                                coordinate to match the IG1/IG2/IG3 paramters of the
-                                field in order to be used. The default behaviour is to
-                                use the vertical record anyway if it's the only one in
-                                the file.
-          --diag-as-model-level
-                                Treat diagnostic (near-surface) data as model level
-                                '1.0'. This is the default behaviour.
-          --split-diag-level    Put the diagnostic (near-surface) data in a separate
-                                variable, away from the 3D model output. Suffices will
-                                be added to distinguish the different types of levels
-                                (i.e. _diag_level and _model_levels for diagnostic
-                                height and hybrid levels respectively).
-          --ignore-diag-level   Ignore data on diagnostic (near-surface) height.
-          --only-diag-level     Only use the diagnostic (near-surface) height,
-                                ignoring other atmospheric levels.
-          --thermodynamic-levels, --tlev
-                                Only convert data that's on 'thermodynamic' vertical
-                                levels.
-          --momentum-levels, --mlev
-                                Only convert data that's on 'momentum' vertical
-                                levels.
-          --vertical-velocity-levels, --wlev
-                                Only convert data that's on 'vertical velocity'
-                                levels.
-          --subgrid-axis        For data on supergrids, split the subgrids along a
-                                "subgrid" axis. The default is to leave the subgrids
-                                stacked together as they are in the RPN file.
-          --keep-LA-LO          Include LA and LO records, even if they appear to be
-                                redundant.
-          --no-adjust-rlon      For rotated grids, do NOT adjust rlon coordinate to
-                                keep the range in -180..180. Allow the rlon value to
-                                be whatever librmn says it should be.
-          --bounds              Include grid cell boundaries in the output.
-          --filter CONDITION    Subset RPN standard file records using the given
-                                criteria. For example, to convert only 24-hour
-                                forecasts you could use --filter ip2==24
-          --exclude NAME,NAME,...
-                                Exclude some axes, attributes, or derived variables
-                                from the output. For instance, excluding
-                                'leadtime,reftime' can help for netCDF tools that
-                                don't recognize leadtime and reftime as valid
-                                coordinates. Note that axes will only be excluded if
-                                they have a length of 1.
-          --yin                 Select first subgrid from a supergrid.
-          --yang                Select second subgrid from a supergrid.
-          --crop-to-smallest-grid
-                                Crop grids to the smaller (inner core) domain for LAM
-                                outputs.
-          --metadata-file METADATA_FILE
-                                Use metadata from the specified file. You can repeat
-                                this option multiple times to build metadata from
-                                different sources.
-          --rename OLDNAME=NEWNAME,...
-                                Apply the specified name changes to the variables.
-          --conventions CONVENTIONS
-                                Set the "Conventions" attribute for the netCDF file.
-                                Default is "CF-1.6". Note that this has no effect on
-                                the structure of the file.
-          --no-conventions      Omit the "Conventions" attribute from the netCDF file
-                                entirely. This can help for netCDF tools that have
-                                trouble recognizing the CF conventions encoded in the
-                                file.
-          --time-units {seconds,minutes,hours,days}
-                                The units for the output time axis. Default is hours.
-          --reference-date YYYY-MM-DD
-                                The reference date for the output time axis. The
-                                default is the starting date in the RPN standard file.
-          --fstd-compat         Adds a compatibility layer to the netCDF output file,
-                                so it can also function as a valid FSTD file.
-                                EXPERIMENTAL.
-          --msglvl {0,DEBUG,2,INFORM,4,WARNIN,6,ERRORS,8,FATALE,10,SYSTEM,CATAST}
-                                How much information to print to stdout during the
-                                conversion. Default is WARNIN.
-          --nc-format {NETCDF4,NETCDF4_CLASSIC,NETCDF3_CLASSIC,NETCDF3_64BIT_OFFSET,NETCDF3_64BIT_DATA}
-                                Which variant of netCDF to write. Default is NETCDF4.
-          --zlib                Turn on compression for the netCDF file. Only works
-                                for NETCDF4 and NETCDF4_CLASSIC formats.
-          --compression COMPRESSION
-                                Compression level for the netCDF file. Only used if
-                                --zlib is set. Default: 4.
-          -f, --force           Overwrite the output file if it already exists.
-          --no-history          Don't put the command-line invocation in the netCDF
-                                metadata.
-          -q, --quiet           Don't display any information except for critical
-                                error messages. Implies --no-progress.
-        ```
-        
-        Using in a Python script
-        ========================
-        
-        Simple conversion
-        --------------------------------------
-        ```python
-        import fstd2nc
-        data = fstd2nc.Buffer("myfile.fst")
-        data.to_netcdf("myfile.nc")
-        ```
-        
-        You can control `fstd2nc.Buffer` using parameters similar to the command-line arguments.  The convention is that *--arg-name* from the command-line would be passed as *arg_name* from Python.
-        
-        For example:
-        ```python
-        import fstd2nc
-        # Select only TT,HU variables.
-        data = fstd2nc.Buffer("myfile.fst", vars=['TT','HU'])
-        # Set the reference date to Jan 1, 2000 in the netCDF file.
-        data.to_netcdf("myfile.nc", reference_date='2000-01-01')
-        ```
-        
-        Interfacing with xarray
-        ---------------------------------------------------------------------------------
-        
-        For more complicated conversions, you can manipulate the data as an [xarray.Dataset](http://xarray.pydata.org/en/stable/data-structures.html#dataset) object by using the `to_xarray()` method:
-        ```python
-        import fstd2nc
-        
-        # Open the FSTD file.
-        data = fstd2nc.Buffer("myfile.fst")
-        
-        # Access the data as an xarray.Dataset object.
-        dataset = data.to_xarray()
-        print (dataset)
-        
-        # Convert surface pressure to Pa.
-        dataset['P0'] *= 100
-        dataset['P0'].attrs['units'] = 'Pa'
-        
-        # (Can further manipulate the dataset here)
-        # ...
-        
-        # Write the final result to netCDF using xarray:
-        dataset.to_netcdf("myfile.nc")
-        ```
-        
-        Interfacing with iris
-        ---------------------------------------------------------------------------------
-        
-        You can interface with [iris](https://scitools.org.uk/iris/docs/latest/index.html) by using the `.to_iris()` method (requires iris version 2.0 or greater).
-        This will give you an [iris.cube.CubeList](https://scitools.org.uk/iris/docs/latest/iris/iris/cube.html#iris.cube.CubeList) object:
-        ```python
-        import fstd2nc
-        import iris.quickplot as qp
-        from matplotlib import pyplot as pl
-        
-        # Open the FSTD file.
-        data = fstd2nc.Buffer("myfile.fst")
-        
-        # Access the data as an iris.cube.CubeList object.
-        cubes = data.to_iris()
-        print (cubes)
-        
-        # Plot all the data (assuming we have 2D fields)
-        for cube in cubes:
-          qp.contourf(cube)
-          pl.gca().coastlines()
-        
-        pl.show()
-        ```
-        
-        Interfacing with pygeode
-        ---------------------------------------------------------------------------------
-        
-        You can create a [pygeode.Dataset](http://pygeode.github.io/dataset.html) object using the `.to_pygeode()` method (requires pygeode version 1.2.2 or greater):
-        ```python
-        import fstd2nc
-        
-        # Open the FSTD file.
-        data = fstd2nc.Buffer("myfile.fst")
-        
-        # Access the data as a pygeode.Dataset object.
-        dataset = data.to_pygeode()
-        print (dataset)
-        ```
-        
-        Interfacing with fstpy
-        ---------------------------------------------------------------------------------
-        
-        You can load data from an [fstpy](https://gitlab.science.gc.ca/CMDS/fstpy) table using the `.from_fstpy()` method (requires fstpy version 2.1.9 or greater):
-        ```python
-        import fstd2nc
-        import fstpy
-        table = fstpy.StandardFileReader('myfile.fst').to_pandas()
-        data = fstd2nc.Buffer.from_fstpy(table)
-        ```
-        You can also export to an fstpy table using the `.to_fstpy()` method:
-        ```python
-        import fstd2nc
-        table = fstd2nc.Buffer('myfile.fst').to_fstpy()
-        ```
-        
-        
-        Requirements
-        ============
-        
-        Basic requirements
-        --------------------
-        
-        This package requires [Python-RPN](https://github.com/meteokid/python-rpn) for reading/writing FSTD files, and [netcdf4-python](https://github.com/Unidata/netcdf4-python) for reading/writing netCDF files.
-        
-        Optional dependencies
-        ---------------------
-        
-        A useful variable dictionary for the `--vardict` option is available [here](https://collaboration.cmc.ec.gc.ca/cmc/CMOI/VariableDictionary/).
-        
-        For reading large numbers of input files (>100), this utility can leverage [pandas](https://github.com/pandas-dev/pandas) to quickly process the FSTD record headers.
-        
-        The `.to_xarray()` Python method requires the [xarray](https://github.com/pydata/xarray) and [dask](https://github.com/dask/dask) packages.
-        
-        The `.to_iris()` Python method requires the [iris](https://scitools.org.uk/iris/docs/latest/index.html) package, along with the `.to_xarray()` dependencies.
-        
-        The `.to_pygeode()` Python method requires the [pygeode](https://github.com/pygeode/pygeode) package, along with the `.to_xarray()` dependencies.
-        
-        The `.to_fstpy()` Python method requires the [fstpy](https://gitlab.science.gc.ca/CMDS/fstpy) package (*internal link*).
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Description-Content-Type: text/markdown
-Provides-Extra: iris
 Provides-Extra: manyfiles
-Provides-Extra: pygeode
 Provides-Extra: array
+Provides-Extra: iris
+Provides-Extra: pygeode
+License-File: COPYING
+License-File: COPYING.LESSER
+
+[Version française](README_fr.md)
+
+Overview
+========
+This module provides a mechanism for converting between FSTD and netCDF file formats, either through Python or the command-line.
+
+
+Installing
+==========
+
+The easiest way to install is using [pip](https://pip.pypa.io/en/stable):
+```
+pip install fstd2nc
+```
+
+
+Basic Usage
+===========
+
+From the command-line
+---------------------
+```
+python -m fstd2nc [options] <infile(s)> <outfile>
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --version             show program's version number and exit
+  --no-progress         Disable the progress bar.
+  --serial              Disables multithreading/multiprocessing. Useful for
+                        resource-limited machines.
+  --minimal-metadata    Don't include internal record attributes and other
+                        internal information in the output metadata. This is
+                        the default behaviour.
+  --internal-metadata, --rpnstd-metadata
+                        Include all internal record attributes in the output
+                        metadata.
+  --metadata-list nomvar,..., --rpnstd-metadata-list nomvar,...
+                        Specify a minimal set of internal record attributes to
+                        include in the output file.
+  --ignore-typvar       Tells the converter to ignore the typvar when deciding
+                        if two records are part of the same field. Default is
+                        to split the variable on different typvars.
+  --ignore-etiket       Tells the converter to ignore the etiket when deciding
+                        if two records are part of the same field. Default is
+                        to split the variable on different etikets.
+  --vars VAR1,VAR2,...  Comma-separated list of variables to convert. By
+                        default, all variables are converted.
+  --fill-value FILL_VALUE
+                        The fill value to use for masked (missing) data. Gets
+                        stored as '_FillValue' attribute in the metadata.
+                        Default is '1e+30'.
+  --datev, --squash-forecasts
+                        Use the date of validity for the "time" axis. This is
+                        the default.
+  --dateo, --forecast-axis
+                        Use the date of original analysis for the time axis,
+                        and put the forecast times into a separate "forecast"
+                        axis.
+  --ensembles           Collect different etikets for the same variable
+                        together into an "ensemble" axis.
+  --profile-momentum-vars VAR1,VAR2,...
+                        Comma-separated list of variables that use momentum
+                        levels.
+  --profile-thermodynamic-vars VAR1,VAR2,...
+                        Comma-separated list of variables that use
+                        thermodynamic levels.
+  --missing-bottom-profile-level
+                        Assume the bottom level of the profile data is
+                        missing.
+  --vardict VARDICT     Use metadata from the specified variable dictionary
+                        (XML format).
+  --opdict              Similar to above, but use the standard CMC-RPN
+                        operational dictionary.
+  --sfc-agg-vars NAME,NAME,...
+                        Define additional surface aggregate fields.
+  --soil-depths SOIL_DEPTHS
+                        Define custom depths for soil fields (WSOL,ISOL).
+                        Defaults are 0.05,0.1,0.2,0.4,1.0,2.0,3.0.
+  --strict-vcoord-match
+                        Require the IP1/IP2/IP3 parameters of the vertical
+                        coordinate to match the IG1/IG2/IG3 paramters of the
+                        field in order to be used. The default behaviour is to
+                        use the vertical record anyway if it's the only one in
+                        the file.
+  --diag-as-model-level
+                        Treat diagnostic (near-surface) data as model level
+                        '1.0'. This is the default behaviour.
+  --split-diag-level    Put the diagnostic (near-surface) data in a separate
+                        variable, away from the 3D model output. Suffices will
+                        be added to distinguish the different types of levels
+                        (i.e. _diag_level and _model_levels for diagnostic
+                        height and hybrid levels respectively).
+  --ignore-diag-level   Ignore data on diagnostic (near-surface) height.
+  --only-diag-level     Only use the diagnostic (near-surface) height,
+                        ignoring other atmospheric levels.
+  --thermodynamic-levels, --tlev
+                        Only convert data that's on 'thermodynamic' vertical
+                        levels.
+  --momentum-levels, --mlev
+                        Only convert data that's on 'momentum' vertical
+                        levels.
+  --vertical-velocity-levels, --wlev
+                        Only convert data that's on 'vertical velocity'
+                        levels.
+  --subgrid-axis        For data on supergrids, split the subgrids along a
+                        "subgrid" axis. The default is to leave the subgrids
+                        stacked together as they are in the RPN file.
+  --keep-LA-LO          Include LA and LO records, even if they appear to be
+                        redundant.
+  --no-adjust-rlon      For rotated grids, do NOT adjust rlon coordinate to
+                        keep the range in -180..180. Allow the rlon value to
+                        be whatever librmn says it should be.
+  --bounds              Include grid cell boundaries in the output.
+  --filter CONDITION    Subset RPN standard file records using the given
+                        criteria. For example, to convert only 24-hour
+                        forecasts you could use --filter ip2==24
+  --exclude NAME,NAME,...
+                        Exclude some axes, attributes, or derived variables
+                        from the output. For instance, excluding
+                        'leadtime,reftime' can help for netCDF tools that
+                        don't recognize leadtime and reftime as valid
+                        coordinates. Note that axes will only be excluded if
+                        they have a length of 1.
+  --yin                 Select first subgrid from a supergrid.
+  --yang                Select second subgrid from a supergrid.
+  --crop-to-smallest-grid
+                        Crop grids to the smaller (inner core) domain for LAM
+                        outputs.
+  --metadata-file METADATA_FILE
+                        Use metadata from the specified file. You can repeat
+                        this option multiple times to build metadata from
+                        different sources.
+  --rename OLDNAME=NEWNAME,...
+                        Apply the specified name changes to the variables.
+  --conventions CONVENTIONS
+                        Set the "Conventions" attribute for the netCDF file.
+                        Default is "CF-1.6". Note that this has no effect on
+                        the structure of the file.
+  --no-conventions      Omit the "Conventions" attribute from the netCDF file
+                        entirely. This can help for netCDF tools that have
+                        trouble recognizing the CF conventions encoded in the
+                        file.
+  --time-units {seconds,minutes,hours,days}
+                        The units for the output time axis. Default is hours.
+  --reference-date YYYY-MM-DD
+                        The reference date for the output time axis. The
+                        default is the starting date in the RPN standard file.
+  --fstd-compat         Adds a compatibility layer to the netCDF output file,
+                        so it can also function as a valid FSTD file.
+                        EXPERIMENTAL.
+  --msglvl {0,DEBUG,2,INFORM,4,WARNIN,6,ERRORS,8,FATALE,10,SYSTEM,CATAST}
+                        How much information to print to stdout during the
+                        conversion. Default is WARNIN.
+  --nc-format {NETCDF4,NETCDF4_CLASSIC,NETCDF3_CLASSIC,NETCDF3_64BIT_OFFSET,NETCDF3_64BIT_DATA}
+                        Which variant of netCDF to write. Default is NETCDF4.
+  --zlib                Turn on compression for the netCDF file. Only works
+                        for NETCDF4 and NETCDF4_CLASSIC formats.
+  --compression COMPRESSION
+                        Compression level for the netCDF file. Only used if
+                        --zlib is set. Default: 4.
+  -f, --force           Overwrite the output file if it already exists.
+  --no-history          Don't put the command-line invocation in the netCDF
+                        metadata.
+  -q, --quiet           Don't display any information except for critical
+                        error messages. Implies --no-progress.
+```
+
+Using in a Python script
+========================
+
+Simple conversion
+--------------------------------------
+```python
+import fstd2nc
+data = fstd2nc.Buffer("myfile.fst")
+data.to_netcdf("myfile.nc")
+```
+
+You can control `fstd2nc.Buffer` using parameters similar to the command-line arguments.  The convention is that *--arg-name* from the command-line would be passed as *arg_name* from Python.
+
+For example:
+```python
+import fstd2nc
+# Select only TT,HU variables.
+data = fstd2nc.Buffer("myfile.fst", vars=['TT','HU'])
+# Set the reference date to Jan 1, 2000 in the netCDF file.
+data.to_netcdf("myfile.nc", reference_date='2000-01-01')
+```
+
+Interfacing with xarray
+---------------------------------------------------------------------------------
+
+For more complicated conversions, you can manipulate the data as an [xarray.Dataset](http://xarray.pydata.org/en/stable/data-structures.html#dataset) object by using the `to_xarray()` method:
+```python
+import fstd2nc
+
+# Open the FSTD file.
+data = fstd2nc.Buffer("myfile.fst")
+
+# Access the data as an xarray.Dataset object.
+dataset = data.to_xarray()
+print (dataset)
+
+# Convert surface pressure to Pa.
+dataset['P0'] *= 100
+dataset['P0'].attrs['units'] = 'Pa'
+
+# (Can further manipulate the dataset here)
+# ...
+
+# Write the final result to netCDF using xarray:
+dataset.to_netcdf("myfile.nc")
+```
+
+Interfacing with iris
+---------------------------------------------------------------------------------
+
+You can interface with [iris](https://scitools.org.uk/iris/docs/latest/index.html) by using the `.to_iris()` method (requires iris version 2.0 or greater).
+This will give you an [iris.cube.CubeList](https://scitools.org.uk/iris/docs/latest/iris/iris/cube.html#iris.cube.CubeList) object:
+```python
+import fstd2nc
+import iris.quickplot as qp
+from matplotlib import pyplot as pl
+
+# Open the FSTD file.
+data = fstd2nc.Buffer("myfile.fst")
+
+# Access the data as an iris.cube.CubeList object.
+cubes = data.to_iris()
+print (cubes)
+
+# Plot all the data (assuming we have 2D fields)
+for cube in cubes:
+  qp.contourf(cube)
+  pl.gca().coastlines()
+
+pl.show()
+```
+
+Interfacing with pygeode
+---------------------------------------------------------------------------------
+
+You can create a [pygeode.Dataset](http://pygeode.github.io/dataset.html) object using the `.to_pygeode()` method (requires pygeode version 1.2.2 or greater):
+```python
+import fstd2nc
+
+# Open the FSTD file.
+data = fstd2nc.Buffer("myfile.fst")
+
+# Access the data as a pygeode.Dataset object.
+dataset = data.to_pygeode()
+print (dataset)
+```
+
+Interfacing with fstpy
+---------------------------------------------------------------------------------
+
+You can load data from an [fstpy](https://gitlab.science.gc.ca/CMDS/fstpy) table using the `.from_fstpy()` method (requires fstpy version 2.1.9 or greater):
+```python
+import fstd2nc
+import fstpy
+table = fstpy.StandardFileReader('myfile.fst').to_pandas()
+data = fstd2nc.Buffer.from_fstpy(table)
+```
+You can also export to an fstpy table using the `.to_fstpy()` method:
+```python
+import fstd2nc
+table = fstd2nc.Buffer('myfile.fst').to_fstpy()
+```
+
+
+Requirements
+============
+
+Basic requirements
+--------------------
+
+This package requires [Python-RPN](https://github.com/meteokid/python-rpn) for reading/writing FSTD files, and [netcdf4-python](https://github.com/Unidata/netcdf4-python) for reading/writing netCDF files.
+
+Optional dependencies
+---------------------
+
+A useful variable dictionary for the `--vardict` option is available [here](https://collaboration.cmc.ec.gc.ca/cmc/CMOI/VariableDictionary/).
+
+For reading large numbers of input files (>100), this utility can leverage [pandas](https://github.com/pandas-dev/pandas) to quickly process the FSTD record headers.
+
+The `.to_xarray()` Python method requires the [xarray](https://github.com/pydata/xarray) and [dask](https://github.com/dask/dask) packages.
+
+The `.to_iris()` Python method requires the [iris](https://scitools.org.uk/iris/docs/latest/index.html) package, along with the `.to_xarray()` dependencies.
+
+The `.to_pygeode()` Python method requires the [pygeode](https://github.com/pygeode/pygeode) package, along with the `.to_xarray()` dependencies.
+
+The `.to_fstpy()` Python method requires the [fstpy](https://gitlab.science.gc.ca/CMDS/fstpy) package (*internal link*).
+
+
```

### Comparing `fstd2nc-0.20230328.0/COPYING.LESSER` & `fstd2nc-0.20230515.0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230328.0/COPYING` & `fstd2nc-0.20230515.0/COPYING`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230328.0/fstd2nc/locale/fr_CA/LC_MESSAGES/fstd2nc.mo` & `fstd2nc-0.20230515.0/fstd2nc/locale/fr_CA/LC_MESSAGES/fstd2nc.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: fstd2nc\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-03-28 05:06+0000\n"
+"POT-Creation-Date: 2023-05-15 23:29+0000\n"
 "PO-Revision-Date: 2022-11-25 17:40+0000\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: fr_CA\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=ISO-8859-1\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -558,17 +558,14 @@
 
 msgid "an RPN standard file"
 msgstr "un fichier standard RPN"
 
 msgid "argument \"-\" with mode %r"
 msgstr "argument \"-\" avec le mode %r"
 
-msgid "can't open '%s': %s"
-msgstr "impossible d'ouvrir '%s': %s"
-
 msgid "cannot have multiple subparser arguments"
 msgstr "impossible d'avoir plusiers arguments de sous-analyseur"
 
 msgid "cannot merge actions - two groups are named %r"
 msgstr "impossible de fusionner les actions - deux groupes sont nommés %r"
 
 msgid "conflicting option string: %s"
```

### Comparing `fstd2nc-0.20230328.0/fstd2nc/__init__.py` & `fstd2nc-0.20230515.0/fstd2nc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2021 - Climate Research Division
+# Copyright 2017-2023 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
@@ -19,15 +19,15 @@
 ###############################################################################
 
 
 """
 Functionality for converting between FSTD and netCDF files.
 """
 
-__version__ = "0.20230328.0"
+__version__ = "0.20230515.0"
 
 
 # Check for bundled rpnpy package.
 # Fall back to this one if no standard rpnpy package available.
 try:
   # Importing the module will set up the appropriate search paths.
   import fstd2nc_deps
```

### Comparing `fstd2nc-0.20230328.0/fstd2nc/extra.py` & `fstd2nc-0.20230515.0/fstd2nc/extra.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2021 - Climate Research Division
+# Copyright 2017-2023 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
```

### Comparing `fstd2nc-0.20230328.0/fstd2nc/stdout.py` & `fstd2nc-0.20230515.0/fstd2nc/stdout.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2021 - Climate Research Division
+# Copyright 2017-2023 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
```

### Comparing `fstd2nc-0.20230328.0/fstd2nc/__main__.py` & `fstd2nc-0.20230515.0/fstd2nc/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2021 - Climate Research Division
+# Copyright 2017-2023 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
```

### Comparing `fstd2nc-0.20230328.0/fstd2nc/mixins/gridhacks.py` & `fstd2nc-0.20230515.0/fstd2nc/mixins/gridhacks.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2021 - Climate Research Division
+# Copyright 2017-2023 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
@@ -17,14 +17,21 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with "fstd2nc".  If not, see <http://www.gnu.org/licenses/>.
 ###############################################################################
 
 from fstd2nc.stdout import _, info, warn, error
 from fstd2nc.mixins import BufferBase
 
+
+# Define a lock for controlling threaded access to ezscint, etc.
+from threading import RLock
+_lock = RLock()
+del RLock
+
+
 ############################################################
 # Mixin for questionable modifications to the headers table.
 #
 
 class GridHacks (BufferBase):
   # Switch on hacks.
   def _enable_hacks (self):
@@ -71,30 +78,55 @@
     if 'ax' in gid:
       new_recs.append(dict(prm, nomvar='>>  ', ni=gid['ni'], d=gid['ax']))
     if 'ay' in gid:
       new_recs.append(dict(prm, nomvar='^^  ', nj=gid['nj'], d=gid['ay']))
     if 'axy' in gid:
       new_recs.append(dict(prm, nomvar='^>  ', ni=gid['ni'], nj=gid['nj'], d=gid['axy']))
     for k,v in self._headers.items():
-      self._headers[k] = np.zeros_like(v, shape=nrecs + len(new_recs))
+      if hasattr(v,'mask'):
+        self._headers[k] = np.ma.zeros(shape=nrecs + len(new_recs), dtype=v.dtype)
+      else:
+        self._headers[k] = np.zeros(shape=nrecs + len(new_recs), dtype=v.dtype)
       self._headers[k][:nrecs] = v[:]
     for i in range(len(new_recs)):
       for k,v in new_recs[i].items():
         if k in self._headers:
           if isinstance(v,str): v = v.encode()
           self._headers[k][nrecs+i] = v
       self._hacks[nrecs+i] = new_recs[i]
     self._nrecs += len(new_recs)
 
 
 #################################################
 # Mixin for on-the-fly grid interpolation.
 #
 
+
+# Helper method - given an interpolation grid string, return a grid id.
+def _get_interp_grid (interp):
+  import rpnpy.librmn.all as rmn
+  # Extract interpolation grid.
+  def number(x):
+    try: return int(x)
+    except ValueError: return float(x)
+  with _lock:
+    interp = interp.split(',')
+    grtyp = interp[0]
+    grid_args = [number(v) for v in interp[1:] if '=' not in v]
+    grid_kwargs = dict(v.split('=') for v in interp[1:] if '=' in v)
+    grid_kwargs = dict((k,number(v)) for k,v in grid_kwargs.items())
+    if not hasattr(rmn,'defGrid_'+grtyp):
+      error(_("Unknown grid '%s'")%grtyp)
+    return getattr(rmn,'defGrid_'+grtyp)(*grid_args,**grid_kwargs)
+
+# Keep track of valid grid ids (to detect if we have a problem with grid ids)
+_valid_gids = set()
+
 class Interp (BufferBase):
+
   @classmethod
   def _cmdline_args (cls, parser):
     from argparse import SUPPRESS
     super(Interp,cls)._cmdline_args(parser)
     #parser.add_argument('--interp', metavar="GRTYP,PARAM=VAL,PARAM=VAL,...", help=_("Interpolate to the specified grid."))
     parser.add_argument('--interp', metavar="GRTYP,PARAM=VAL,PARAM=VAL,...", help=SUPPRESS)
 
@@ -104,39 +136,28 @@
         Interpolate to the specified grid.
     """
     import rpnpy.librmn.all as rmn
     import numpy as np
     interp = kwargs.pop('interp',None)
     super(Interp,self).__init__(*args,**kwargs)
     # Extract interpolation grid.
-    def number(x):
-      try: return int(x)
-      except ValueError: return float(x)
     if interp is not None:
-      interp = interp.split(',')
-      grtyp = interp[0]
-      grid_args = [number(v) for v in interp[1:] if '=' not in v]
-      grid_kwargs = dict(v.split('=') for v in interp[1:] if '=' in v)
-      grid_kwargs = dict((k,number(v)) for k,v in grid_kwargs.items())
-      if not hasattr(rmn,'defGrid_'+grtyp):
-        error(_("Unknown grid '%s'")%grtyp)
-      self._interp_grid = getattr(rmn,'defGrid_'+grtyp)(*grid_args,**grid_kwargs)
+      interp_grid = _get_interp_grid(interp)
+      self._interp_grid = interp_grid
       # Hack the new grid descriptors into the headers.
-      self._writeGrid (self._interp_grid)
+      self._writeGrid (interp_grid)
+      _valid_gids.add(interp_grid['id'])
 
       # Store original and modified versions of the grid descriptors.
-      ismeta = self._headers['ismeta']
-      self._original_grid = dict()
-      self._modified_grid = dict()
-      for key in ('grtyp','ni','nj','ig1','ig2','ig3','ig4'):
-        self._original_grid[key] = self._headers[key]
-        self._modified_grid[key] = np.array(self._headers[key])
-        self._modified_grid[key][:] = np.where(ismeta, self._headers[key], self._interp_grid[key])
+      self._decoder_extra_args = self._decoder_extra_args + ('source_gid','dest_gid')
+      self._ignore_atts = self._ignore_atts + ('source_gid','dest_gid')
+      self._headers['source_gid'] = np.empty(self._nrecs,dtype=object)
 
       # Set up some options for ezsint.
+      import rpnpy.librmn.all as rmn
       rmn.ezsetopt (rmn.EZ_OPT_EXTRAP_DEGREE, rmn.EZ_EXTRAP_VALUE)
       rmn.ezsetopt (rmn.EZ_OPT_EXTRAP_VALUE, self._fill_value)
 
 
   def _makevars (self):
     from fstd2nc.mixins import _iter_type
     import numpy as np
@@ -145,45 +166,57 @@
       return super(Interp,self)._makevars()
 
     # Run _makevars chain with original grid descriptors to allow
     # xycoords to give us source grid ids,
     # switch out the grid descriptors in the table, then let xycoords
     # construct the target grid axes for us.
     super(Interp,self)._makevars()
-    self._source_gids = np.array(self._gids)
-    self._headers.update(self._modified_grid)
+    self._headers['source_gid'][:] = np.array(self._gids)
+    _valid_gids.update(g for g in self._gids if g >= 0)
+    # Now, use interpolated grid descriptors.
+    ismeta = self._headers['ismeta']
+    for key in ('grtyp','ni','nj','ig1','ig2','ig3','ig4'):
+      self._headers[key][:] = np.where(ismeta, self._headers[key], self._interp_grid[key])
     super(Interp,self)._makevars()
 
     # Add fill value to the data.
     # Modified from code in from mask mixin.
     # Set this fill value for any interpolated data, since it may contain
     # points outside the original boundary.
     for var in self._varlist:
       if isinstance(var,_iter_type):
         var.atts['_FillValue'] = var.dtype.type(self._fill_value)
 
+  def _decoder_scalar_args (self):
+    args = super(Interp,self)._decoder_scalar_args()
+    if hasattr(self,'_interp_grid'):
+      args['dest_gid'] = self._interp_grid['id']
+    return args
+
   # Handle grid interpolations from raw binary array.
-  def _decode (self, data, rec_id, _grid_cache={}):
+  @classmethod
+  def _decode (cls, data, source_gid=None, dest_gid=None, **kwargs):
     import rpnpy.librmn.all as rmn
     import numpy as np
-    if self._headers['ismeta'][rec_id] or not hasattr(self,'_interp_grid'):
-      return super(Interp,self)._decode (data, rec_id)
+    if source_gid is None or dest_gid is None:
+      return super(Interp,cls)._decode (data, **kwargs)
+    if source_gid not in _valid_gids or dest_gid not in _valid_gids:
+      error(_("Problem finding grid id.  It's possible that you're running this in a multi-processing environment, which does not support the 'interp' option."))
     # Retrieve an active librmn grid id associated with this grid.
-    # (must be supplied by xycoords mixin).
-    ingrid = int(self._source_gids[rec_id])
-    if ingrid < 0:
+    if source_gid < 0:
       raise ValueError("Source data is not on a recognized grid.  Unable to interpolate.")
-    d = super(Interp,self)._decode (data, rec_id).T
-    with self._lock:
+    d = super(Interp,cls)._decode (data, **kwargs).T
+    with _lock:
       # Propogate any fill values to the interpolated grid.
+      fill_value = kwargs.get('fill_value')
       in_mask = np.zeros(d.shape, order='F', dtype='float32')
-      in_mask[d==self._fill_value] = 1.0
-      d = rmn.ezsint (self._interp_grid, ingrid, d)
-      out_mask = rmn.ezsint (self._interp_grid, ingrid, in_mask)
-      d[out_mask!=0] = self._fill_value
+      in_mask[d==fill_value] = 1.0
+      d = rmn.ezsint (dest_gid, source_gid, d)
+      out_mask = rmn.ezsint (dest_gid, source_gid, in_mask)
+      d[out_mask!=0] = fill_value
       # Return the data for the interpolated field.
       return d.T
 
 
 #################################################
 # Mixin for yin/yang grid subsetting.
 #
@@ -242,25 +275,31 @@
       ig2 = int(self._headers['ig2'][rec_id])
       ig3 = int(self._headers['ig3'][rec_id])
       ig4 = int(self._headers['ig4'][rec_id])
       submask = mask & (self._headers['ig1'] == ig1) & (self._headers['ig2'] == ig2) & (self._headers['ig3'] == ig3) & (self._headers['ig4'] == ig4)
       for key in ('grtyp','ni','nj','ig1','ig2','ig3','ig4'):
         self._headers[key][submask] = dest_grid[key]
 
+  def _decoder_scalar_args (self):
+    kwargs = super(YinYang,self)._decoder_scalar_args()
+    if self._yin: kwargs['yin'] = True
+    if self._yang: kwargs['yang'] = True
+    return kwargs
 
   # Handle grid interpolations from raw binary array.
-  def _decode (self, data, unused):
-    if not self._yin and not self._yang:
-      return super(YinYang,self)._decode (data, unused)
-    prm = self._decode_headers(data[:72])
+  @classmethod
+  def _decode (cls, data, yin=False, yang=False, **kwargs):
+    if not yin and not yang:
+      return super(YinYang,cls)._decode (data, **kwargs)
+    prm = cls._decode_headers(data[:72])
     prm = dict((k,v[0]) for k,v in prm.items())
-    d = super(YinYang,self)._decode (data, unused).T
-    if prm['grtyp'] == b'U' and self._yin:
+    d = super(YinYang,cls)._decode (data, **kwargs).T
+    if prm['grtyp'] == b'U' and yin:
       d = d[:,:prm['nj']//2]
-    elif prm['grtyp'] == b'U' and self._yang:
+    elif prm['grtyp'] == b'U' and yang:
       d = d[:,prm['nj']//2:]
     return d.T
 
 #################################################
 # Mixin for grid cropping.
 #
 
@@ -283,18 +322,18 @@
     # Load the metadata from the file(s).
     super(Crop,self).__init__(*args,**kwargs)
 
     if not self._crop_to_smallest_grid:
       return
 
     # Keep track of cropping regions for the data.
-    self._headers['i0'] = np.zeros(self._nrecs,'uint16')
-    self._headers['iN'] = np.array(self._headers['ni'],'uint16')
-    self._headers['j0'] = np.zeros(self._nrecs,'uint16')
-    self._headers['jN'] = np.array(self._headers['nj'],'uint16')
+    self._decoder_extra_args = self._decoder_extra_args + ('crop_j','crop_i')
+    self._headers['crop_j'] = np.empty(self._nrecs,object)
+    self._headers['crop_i'] = np.empty(self._nrecs,object)
+    self._ignore_atts = self._ignore_atts + ('crop_j','crop_i')
 
     # Run _makevars early to generate grid ids with xycoords mixin.
     # Silence warnings from makevars, which might not be relevant to the final
     # state after we make our grid modifications.
     import fstd2nc
     streams = fstd2nc.stdout.streams
     fstd2nc.stdout.streams = ()
@@ -336,29 +375,21 @@
         if jN-j0 != smallest_grid['nj']: continue
         if np.any(grid['ax'].flatten()[i0:iN] != smallest_grid['ax'].flatten()): continue
         if np.any(grid['ay'].flatten()[j0:jN] != smallest_grid['ay'].flatten()): continue
         # Able to crop, so update the headers to point to the cropped coordinates.
         submask = (self._headers['ig1'] == grid['tag1']) & (self._headers['ig2'] == grid['tag2']) & (self._headers['ig3'] == grid['tag3'])
         for key in ('grtyp','ni','nj','ig1','ig2','ig3','ig4'):
           self._headers[key][submask] = smallest_grid[key]
-        self._headers['i0'][submask] = i0
-        self._headers['iN'][submask] = iN
-        self._headers['j0'][submask] = j0
-        self._headers['jN'][submask] = jN
-
+        self._headers['crop_j'][submask] = slice(j0,jN)
+        self._headers['crop_i'][submask] = slice(i0,iN)
 
   # Handle cropping from raw binary array.
-  def _decode (self, data, rec_id):
-    import numpy as np
-    d = super(Crop,self)._decode (data, rec_id)
-    if not self._crop_to_smallest_grid: return d
-    # Check if cropping necessary.
-    ni = self._headers['ni'][rec_id]
-    nj = self._headers['nj'][rec_id]
-    if d.shape == (nj,ni): return d
-    i0 = self._headers['i0'][rec_id]
-    iN = self._headers['iN'][rec_id]
-    j0 = self._headers['j0'][rec_id]
-    jN = self._headers['jN'][rec_id]
-    d = d[j0:jN,i0:iN]
+  @classmethod
+  def _decode (cls, data, crop_j=None, crop_i=None, **kwargs):
+    d = super(Crop,cls)._decode (data, **kwargs)
+    if crop_j is not None:
+      d = d[crop_j,:]
+    if crop_i is not None:
+      d = d[:,crop_i]
     return d
 
+
```

### Comparing `fstd2nc-0.20230328.0/fstd2nc/mixins/compat.py` & `fstd2nc-0.20230515.0/fstd2nc/mixins/compat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2021 - Climate Research Division
+# Copyright 2017-2023 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
@@ -201,18 +201,18 @@
           v = f.createVariable(var.name, datatype=var.array.dtype, dimensions=var.dims, zlib=zlib, complevel=compression)
         # Write the metadata.
         v.setncatts(var.atts)
         direct_addresses[var.array.tobytes()] = write_data (v, (), var.array)
         continue
       # Hard case: only have the record indices, need to loop over the records.
       # Get the shape of a single record for the variable.
-      if hasattr(var,'record_id'):
+      if hasattr(var, 'chunks'):
+        continue  #TODO
+      elif hasattr(var,'record_id'):
         record_shape = var.shape[var.record_id.ndim:]
-      elif hasattr(var,'chunksize'):
-        record_shape = var.chunksize
       else:
         continue
       # Use this as the "chunk size" for the netCDF file, to improve I/O
       # performance.
       chunksizes = (1,)*(len(var.axes)-len(record_shape)) + record_shape
       if hasattr(self,'_fill_value') and var.dtype.name.startswith('float32'):
         fill_value = self._fill_value
```

### Comparing `fstd2nc-0.20230328.0/fstd2nc/mixins/filter.py` & `fstd2nc-0.20230515.0/fstd2nc/mixins/filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2021 - Climate Research Division
+# Copyright 2017-2023 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
```

### Comparing `fstd2nc-0.20230328.0/fstd2nc/mixins/ensembles.py` & `fstd2nc-0.20230515.0/fstd2nc/mixins/ensembles.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2021 - Climate Research Division
+# Copyright 2017-2023 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
```

### Comparing `fstd2nc-0.20230328.0/fstd2nc/mixins/pruneaxes.py` & `fstd2nc-0.20230515.0/fstd2nc/mixins/pruneaxes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2021 - Climate Research Division
+# Copyright 2017-2023 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
```

### Comparing `fstd2nc-0.20230328.0/fstd2nc/mixins/removestuff.py` & `fstd2nc-0.20230515.0/fstd2nc/mixins/removestuff.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2021 - Climate Research Division
+# Copyright 2017-2023 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
```

### Comparing `fstd2nc-0.20230328.0/fstd2nc/mixins/diaghacks.py` & `fstd2nc-0.20230515.0/fstd2nc/mixins/diaghacks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2021 - Climate Research Division
+# Copyright 2017-2023 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
```

### Comparing `fstd2nc-0.20230328.0/fstd2nc/mixins/dates.py` & `fstd2nc-0.20230515.0/fstd2nc/mixins/dates.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2021 - Climate Research Division
+# Copyright 2017-2023 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
```

### Comparing `fstd2nc-0.20230328.0/fstd2nc/mixins/sfc_codes.py` & `fstd2nc-0.20230515.0/fstd2nc/mixins/sfc_codes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2021 - Climate Research Division
+# Copyright 2017-2023 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
```

### Comparing `fstd2nc-0.20230328.0/fstd2nc/mixins/vcoords.py` & `fstd2nc-0.20230515.0/fstd2nc/mixins/vcoords.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2021 - Climate Research Division
+# Copyright 2017-2023 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
@@ -286,14 +286,20 @@
 
     vrecs = self._vrecs
 
     # If this becomes True by the end, then we need to rerun this routine
     # again with updated information.
     rerun = False
 
+    # Check if cell boundaries are requested.
+    # This is controlled from the xycoords mixin, but we can also add
+    # vertical bounds as well.
+    bounds = self._bounds
+    from fstd2nc.mixins.xycoords import bnds2
+
     # Scan through the data, and look for any use of vertical coordinates.
     vaxes = OrderedDict()
     prefs = dict()  # Reference pressure scalar variables.
     for var in self._varlist:
       level_axis = var.getaxis('level')
       if level_axis is None: continue
       # Degenerate vertical axis (0mb or 0hy?)
@@ -339,14 +345,15 @@
 
         # Keep track of any extra arrays needed for this axis.
         coordinates = []
         internal_atts = OrderedDict()
         atts = OrderedDict()
         name = 'level'
         new_axis = _axis_type(name, atts, level_axis.array)
+        new_bnds = _var_type(name+'_bnds', {}, [new_axis,bnds2], None)
 
         # Check if we have a vertical coordinate record to use.
         if key in vrecs:
           header = vrecs[key]
           # Add in metadata from the coordinate.
           atts.update(self._get_header_atts(header))
           # Add type-specific metadata.
@@ -363,14 +370,18 @@
             except VGDError:
               warn (_("Problem decoding !! record."))
               continue
             # Partial definition of a/b coordinates for formula_terms reference.
             coordA = _var_type('a', {}, [new_axis], None)
             coordB = _var_type('b', {}, [new_axis], None)
             coordC = _var_type('c', {}, [new_axis], None)
+            # Partial definition of a/b boundaries.
+            coordA_bnds = _var_type('a_bnds', {}, [new_axis,bnds2], None)
+            coordB_bnds = _var_type('b_bnds', {}, [new_axis,bnds2], None)
+            coordC_bnds = _var_type('c_bnds', {}, [new_axis,bnds2], None)
 
             # First, patch up VGD_OPR_KEYS to include SLEVE coordinates?
             #TODO: remove this once rpnpy has full support for this.
             original_opr_double_keys = list(VGD_OPR_KEYS['get_double_1d'])
             original_opr_float_keys = list(VGD_OPR_KEYS['get_float_1d'])
             if sleve:
               VGD_OPR_KEYS['get_double_1d'].extend(['CC_M','CC_T'])
@@ -428,19 +439,50 @@
                 ind = all_z.index(z)
                 A.append(all_a[ind])
                 B.append(all_b[ind])
                 if sleve: C.append(all_c[ind])
               coordA.array = np.asarray(A)
               coordB.array = np.asarray(B)
               coordC.array = np.asarray(C)
+              # Find vertical layer boundaries.
+              if bounds:
+                A_bnds1, A_bnds2 = [], []
+                B_bnds1, B_bnds2 = [], []
+                C_bnds1, C_bnds2 = [], []
+                z_bnds1, z_bnds2 = [], []
+                all_z_sorted = sorted(all_z)
+                for z in levels:
+                  ind = all_z_sorted.index(z)
+                  z1 = all_z_sorted[ind-1]
+                  z2 = all_z_sorted[ind+1]
+                  ind1 = all_z.index(z1)
+                  ind2 = all_z.index(z2)
+                  A_bnds1.append(all_a[ind1])
+                  A_bnds2.append(all_a[ind2])
+                  B_bnds1.append(all_b[ind1])
+                  B_bnds2.append(all_b[ind2])
+                  z_bnds1.append(all_z[ind1])
+                  z_bnds2.append(all_z[ind2])
+                  if sleve:
+                    C_bnds1.append(all_c[ind1])
+                    C_bnds2.append(all_c[ind2])
+                coordA_bnds.array = np.array(np.asarray([A_bnds1,A_bnds2]).T)
+                coordB_bnds.array = np.array(np.asarray([B_bnds1,B_bnds2]).T)
+                new_bnds.array = np.array(np.asarray([z_bnds1,z_bnds2]).T)
+                if sleve:
+                  coordC_bnds.array = np.array(np.asarray([C_bnds1,C_bnds2]).T)
             except (KeyError,ValueError,VGDError):
               warn (_("Unable to get A/B coefficients for %s.")%var.name)
               coordA = None
               coordB = None
               coordC = None
+              coordA_bnds = None
+              coordB_bnds = None
+              coordC_bnds = None
+              new_bnds = None
             vgd_free (vgd_id)
         ###
 
         # Get metadata that's specific to this axis.
         atts['axis'] = 'Z'
         # Reference: http://web-mrb.cmc.ec.gc.ca/science//si/eng/si/libraries/rmnlib/fstd/main.html#RTFToC11
         # Also: https://wiki.cmc.ec.gc.ca/wiki/Vgrid/vcode
@@ -515,14 +557,15 @@
                   atts['formula_terms']['pref'] = prefs[pref]
                 except (KeyError,VGDError):
                   pass # Don't have PREF available for some reason?
               else:
                 atts['standard_name'] = 'atmosphere_hybrid_sigma_pressure_coordinate'
                 if None not in (coordA,coordB):
                   coordA.array /= 100.0  # Use hPa for final units.
+                  if coordA_bnds is not None and coordA_bnds.array is not None: coordA_bnds.array /= 100.0
                   atts['formula'] = 'p = ap + b*ps'
                   coordA.name = 'ap'
                   atts['formula_terms'] = OrderedDict([('ap',coordA),('b',coordB),('ps','P0')])
                   coordinates.extend([coordA,coordB])
 
             # Not a '!!' coordinate, so must be 'HY'?
             else:
@@ -571,14 +614,33 @@
             atts['standard_name'] = 'atmosphere_hybrid_height_coordinate'
             atts['positive'] = 'up'
             if None not in (coordA,coordB):
               atts['formula'] = 'z = a + b*orog'
               atts['formula_terms'] = OrderedDict([('a',coordA),('b',coordB),('orog','ME')])
               coordinates.extend([coordA,coordB])
 
+        # Attach vertical boundaries?
+        if bounds and new_bnds is not None:
+          atts['bounds'] = new_bnds
+          # Attach a/b bounds
+          if 'formula_terms' in atts:
+            new_bnds.atts['formula_terms'] = atts['formula_terms'].copy()
+            for k, v in new_bnds.atts['formula_terms'].items():
+              if v is coordA:
+                new_bnds.atts['formula_terms'][k] = coordA_bnds
+                coordA.atts['bounds'] = coordA_bnds
+                coordA_bnds.name = coordA.name+'_bnds'
+              if v is coordB:
+                new_bnds.atts['formula_terms'][k] = coordB_bnds
+                coordB.atts['bounds'] = coordB_bnds
+                coordB_bnds.name = coordB.name+'_bnds'
+              if v is coordC:
+                new_bnds.atts['formula_terms'][k] = coordC_bnds
+                coordC.atts['bounds'] = coordC_bnds
+                coordC_bnds.name = coordC.name+'_bnds'
         # Add this vertical axis.
         if len(coordinates) > 0:
           atts['coordinates'] = coordinates
         # Update axis name.
         new_axis.name = name
         # Now have a fully defined axis to use.
         vaxes[(id(level_axis),kind,version)] = new_axis
```

### Comparing `fstd2nc-0.20230328.0/fstd2nc/mixins/__init__.py` & `fstd2nc-0.20230515.0/fstd2nc/mixins/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2021 - Climate Research Division
+# Copyright 2017-2023 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
@@ -126,32 +126,23 @@
     self.dtype = dtype
     self.record_id = record_id
     self.deps = []
 
 # Similar to above, but more general.
 # Can allow for multiple records along the inner axes.
 class _chunk_type (_base_type):
-  __slots__ = ('name','atts','axes','dtype','chunks','chunksize','deps')
-  def __init__ (self, name, atts, axes, dtype, chunks, chunksize):
+  __slots__ = ('name','atts','axes','dtype','chunks','record_id','deps')
+  def __init__ (self, name, atts, axes, dtype, chunks, record_id):
     self.name = name
     self.atts = atts
     self.axes = axes
     self.dtype = dtype
     self.chunks = chunks
-    self.chunksize = chunksize
+    self.record_id = record_id
     self.deps = []
-  def items(self):
-    for key, value in self.chunks.items():
-      key = tuple(k if isinstance(k,int) else slice(*k) for k in key)
-      yield key, value
-  def keys(self):
-    for key, value in self.items():
-      yield key
-  def values(self):
-    return self.chunks.values()
 
 # Fake progress bar - does nothing.
 class _FakeBar (object):
   def __init__ (self, *args, **kwargs): pass
   def iter(self, it):
     for i in it: yield i
   def __next__(self): pass
@@ -239,14 +230,29 @@
   # Uses string formatting operations on the variable metadata.
   _human_var_id = ()
 
   # Record parameters which should not be used as nc variable attributes.
   # (They're either internal to the file, or part of the data, not metadata).
   _ignore_atts = ('file_id','name','address','length','dtype','selected')
 
+  # Header columns which contain extra data that should be passed to _decode.
+  # Tuple of (offset, length, d) where:
+  # - offset is the address in the file where the data is located.
+  # - length is how much data to read.
+  # - d is an alternate source (dask graph?) for case where data is not
+  #   stored in a file.
+  _decoder_data = (('data',('address','length','d')),)
+
+  # Extra arguments to pull from columns of the table.
+  _decoder_extra_args = ()
+
+  # Extra (scalar) arguments needed for the decoder at runtime.
+  def _decoder_scalar_args (self):
+    return {}
+
   # Define any command-line arguments for reading FSTD files.
   @classmethod
   def _cmdline_args (cls, parser):
     from fstd2nc import __version__
     from argparse import SUPPRESS
     from sys import stdout
     parser.add_argument('--version', action='version', version=__version__, help=_("show program's version number and exit"))
@@ -882,34 +888,59 @@
       for o in self._iter_objects(obj.atts,handled):
         yield o
     if hasattr(obj,'deps'):
       for o in self._iter_objects(obj.deps,handled):
         yield o
 
   # How to decode the data from a raw binary array.
-  def _decode (self, data, unused):
+  @classmethod
+  def _decode (cls, data):
     raise NotImplementedError("No decoder found.")
 
   # Shortcuts to header decoding functions.
   # Put into the class so they can potentially be overridden for other formats.
   @staticmethod
   def _decode_headers (headers):
     raise NotImplementedError("No decoder found.")
   @staticmethod
   def _raw_headers (filename):
     raise NotImplementedError("No decoder found.")
 
   # Shortcut for reading a record, given a record id.
   def _read_record (self, rec):
     import numpy as np
-    with open(self._files[self._headers['file_id'][rec]],'rb') as f:
-      f.seek(self._headers['address'][rec],0)
-      data = np.fromfile(f,'B',self._headers['length'][rec])
-      data = self._decode(data,rec)
-    return data
+    kwargs = {}
+    # Add file-based data.
+    file_id = self._headers['file_id'][rec]
+    if file_id >= 0:
+      f = open(self._files[file_id], 'rb')
+    else:
+      f = None
+    for key, (addr_key, len_key, d_key) in self._decoder_data:
+      if addr_key not in self._headers: continue
+      # Special case: have dask array to read.
+      if d_key in self._headers:
+        d = self._headers[d_key][rec]
+        if d is not None:
+          kwargs[key] = d.T
+          continue
+      address = self._headers[addr_key][rec]
+      length = self._headers[len_key][rec]
+      if address == -1 or length == -1: continue
+      f.seek(address,0)
+      data = np.fromfile(f,'B',length)
+      kwargs[key] = data
+    for key in self._decoder_extra_args:
+      if key in self._headers:
+        value = self._headers[key][rec]
+        kwargs[key] = value
+    kwargs.update(self._decoder_scalar_args())
+    if f is not None:
+      f.close()
+    return self._decode(**kwargs)
 
 
   #
   ###############################################
```

### Comparing `fstd2nc-0.20230328.0/fstd2nc/mixins/fstd.py` & `fstd2nc-0.20230515.0/fstd2nc/mixins/fstd.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2021 - Climate Research Division
+# Copyright 2017-2023 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
@@ -49,23 +49,14 @@
 def fast_dtype_fst2numpy (datyp, nbits):
   import numpy as np
   args = np.array(datyp,'uint64')
   args <<= 32
   args += np.asarray(nbits,'uint64')
   return packed_dtype_fst2numpy(args)
 
-# Define a lock for controlling threaded access to the RPN file(s).
-# This is necessary because we can only open a limited number of files
-# at a time, so need to control which ones are opened and available in
-# a thread-safe way.
-from threading import RLock
-_lock = RLock()
-del RLock
-
-
 # Define a class for encoding / decoding FSTD data.
 class FSTD (BufferBase):
   _format = _("RPN standard file")
   _format_singular = _("an RPN standard file")
   _format_plural = _("RPN standard file(s)")
 
   # Keep a reference to fstd98 so it's available during cleanup.
@@ -110,22 +101,14 @@
   # Note: not the fastest method.  Should be used sparingly.
   def _fstlir (self, **criteria):
     recs = self._fstinl(**criteria)
     if len(recs) == 0: return None
     rec = recs[0]
     return self._fstluk(rec)
 
-  # Control the pickling / unpickling of BufferBase objects.
-  def __getstate__ (self):
-    state = super(FSTD,self).__getstate__()
-    state.pop('_lock',None)  # librmn lock will be defined upon unpickling.
-    return state
-  def __setstate__ (self, state):
-    super(FSTD,self).__setstate__(state)
-    self._lock = _lock
 
 
   ###############################################
   # Basic flow for reading data
 
   def __init__ (self, *args, **kwargs):
     """
@@ -136,19 +119,14 @@
     ignore_etiket : bool, optional
         Tells the converter to ignore the etiket when deciding if two
         records are part of the same field.  Default is to split the
         variable on different etikets.
     """
     import numpy as np
 
-    # Set up lock for threading.
-    # The same lock is shared for all Buffer objects, to synchronize access to
-    # librmn.
-    self._lock = _lock
-
     self._inner_axes = ('k','j','i')
 
     # Note: name should always be the first attribute
     self._var_id = ('name','ni','nj','nk') + self._var_id
     self._human_var_id = ('%(name)s', '%(ni)sx%(nj)s', '%(nk)sL') + self._human_var_id
     self._ignore_atts = ('swa','lng','dltf','ubc','xtra1','xtra2','xtra3','i','j','k','ismeta','d') + self._ignore_atts
 
@@ -194,16 +172,21 @@
       self._headers['address'] = np.array(self._headers['swa'],int)*8-8
     if 'lng' in self._headers:
       self._headers['length'] = np.array(self._headers['lng'],int)*4
     self._headers['dtype'] = np.array(fast_dtype_fst2numpy(self._headers['datyp'],self._headers['nbits']))
     self._headers['selected'] = (self._headers['dltf']==0) & (self._headers['ismeta'] == False)
 
   # How to decode the data from a raw binary array.
-  def _decode (self, data, unused):
+  @classmethod
+  def _decode (cls, data):
     from fstd2nc.extra import decode
+    # Degenerate case: decoding handled in opaque dask layer, nothing to do.
+    if hasattr(data,'dask'):
+      import numpy as np
+      return np.array(data.T)
     nbits = int(data[0x0b])
     datyp = int(data[0x13])
     dtype = dtype_fst2numpy(datyp, nbits)
     out = decode(data).view(dtype)
     return out
 
   # Shortcuts to header decoding functions.
```

### Comparing `fstd2nc-0.20230328.0/fstd2nc/mixins/mesh.py` & `fstd2nc-0.20230515.0/fstd2nc/mixins/mesh.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2021 - Climate Research Division
+# Copyright 2017-2023 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
```

### Comparing `fstd2nc-0.20230328.0/fstd2nc/mixins/vardict.py` & `fstd2nc-0.20230515.0/fstd2nc/mixins/vardict.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2021 - Climate Research Division
+# Copyright 2017-2023 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
```

### Comparing `fstd2nc-0.20230328.0/fstd2nc/mixins/masks.py` & `fstd2nc-0.20230515.0/fstd2nc/mixins/masks.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2021 - Climate Research Division
+# Copyright 2017-2023 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
@@ -45,117 +45,117 @@
   def __init__ (self, *args, **kwargs):
     """
     fill_value : scalar, optional
         The fill value to use for masked (missing) data.  Gets stored as
         '_FillValue' attribute in the metadata.  Default is 1e30.
     """
     import numpy as np
+    from fstd2nc.extra import structured_array
+    from collections import OrderedDict
+
+    self._decoder_data = self._decoder_data + (('mask',('mask_address','mask_length','mask_d')),)
+
     self._fill_value = kwargs.pop('fill_value',1e30)
+    self._decoder_extra_args = self._decoder_extra_args + ('alt_mask',)
+    self._ignore_atts = ('mask_record','mask_length','alt_mask') + self._ignore_atts
     super(Masks,self).__init__(*args,**kwargs)
-    # Modify 'lng' to overlap the data and mask fields (where they are stored
-    # consecutively).
-    # This will allow the _decode method to apply the mask directly.
+
+    # Check for usage of the alternate masking technique (flag 64).
+    # By convention (as far as I know), the maximum value in the field is
+    # a special value indicating where data is masked out.
+    self._headers['alt_mask'] = (self._headers['datyp']&64) == 64
+
     nomvar = self._headers['nomvar']
     typvar = self._headers['typvar']
     etiket = self._headers['etiket']
     datev = self._headers['datev']
     ip1 = self._headers['ip1']
     ip2 = self._headers['ip2']
     ip3 = self._headers['ip3']
+    dltf = self._headers['dltf']
     uses_mask = np.array(typvar,dtype='|S2').view('|S1').reshape(-1,2)[:,1] == b'@'
+    if not np.any(uses_mask): return
 
-    # If data is from an FSTD file on disk, then try overlapping the read of
-    # the data and mask.
-    try:
-      swa = self._headers['swa']
-      lng = self._headers['lng'].copy()
-      dltf = self._headers['dltf']
-      if np.sum(uses_mask) > 0:
-        overlap = (nomvar[:-1] == nomvar[1:]) & (etiket[:-1] == etiket[1:]) & (datev[:-1] == datev[1:]) & (ip1[:-1] == ip1[1:]) & (ip2[:-1] == ip2[1:]) & (ip3[:-1] == ip3[1:]) & uses_mask[:-1] & uses_mask[1:] & (dltf[:-1] == dltf[1:])
-        overlap = np.where(overlap)[0]
-        lng[overlap] = swa[overlap+1]*2 + lng[overlap+1] - swa[overlap]*2
-        self._headers['lng'] = lng
-        self._headers['length'] = lng*4  # Length in bytes used for _decode
-    except KeyError:
-      pass  # Not our data from disk (maybe from fstpy?) so can't do that.
     # Remove all mask records from the table, they should not become variables
     # themselves.
     is_mask = (self._headers['typvar'] == b'@@')
     self._headers['selected'][is_mask] = False
 
+    nrecs = len(self._headers['name'])
+
+    has_mask = (nomvar[:-1] == nomvar[1:]) & (etiket[:-1] == etiket[1:]) & (datev[:-1] == datev[1:]) & (ip1[:-1] == ip1[1:]) & (ip2[:-1] == ip2[1:]) & (ip3[:-1] == ip3[1:]) & uses_mask[:-1] & uses_mask[1:] & (dltf[:-1] == dltf[1:])
+    has_mask = np.where(has_mask)[0]
+
+    # Figure out how to pair up the data and mask.
+    # Requires O(n log n) time, which is better than O(n^2) for naive lookup
+    # on each record.
+    # Easy case - masks appear immediately following the data.
+    # (Removed in current implementation, no longer reading mask and data together).
+
+    # Harder case - masks are in the file, but in random order.
+
+    keys = OrderedDict([('dltf',dltf),('nomvar',nomvar),('etiket',etiket),('datev',datev),('ip1',ip1),('ip2',ip2),('ip3',ip3),('typvar',typvar)])
+    ind = np.argsort(structured_array(keys))
+    # Find mask / data pairs.
+    # (In this case, with the above sort, masks will appear before the data)
+    # Use similar comparisons as with the easy case.
+    nomvar = nomvar[ind]
+    typvar = typvar[ind]
+    etiket = etiket[ind]
+    datev = datev[ind]
+    ip1 = ip1[ind]
+    ip2 = ip2[ind]
+    ip3 = ip3[ind]
+    dltf = dltf[ind]
+    uses_mask = np.array(typvar,dtype='|S2').view('|S1').reshape(-1,2)[:,1] == b'@'
+    has_mask = (nomvar[:-1] == nomvar[1:]) & (etiket[:-1] == etiket[1:]) & (datev[:-1] == datev[1:]) & (ip1[:-1] == ip1[1:]) & (ip2[:-1] == ip2[1:]) & (ip3[:-1] == ip3[1:]) & uses_mask[:-1] & uses_mask[1:] & (dltf[:-1] == dltf[1:])
+    has_mask = np.where(has_mask)[0]
+    has_mask += 1  # Data appears after mask in this case.
+    rec_id = np.arange(nrecs)[ind]
+    self._headers['mask_address'] = np.empty(nrecs,'int32')
+    self._headers['mask_address'][:] = -1
+    self._headers['mask_address'][rec_id[has_mask]] = self._headers['address'][rec_id[has_mask-1]]
+    self._headers['mask_length'] = np.empty(nrecs,'int32')
+    self._headers['mask_length'][:] = -1
+    self._headers['mask_length'][rec_id[has_mask]] = self._headers['length'][rec_id[has_mask-1]]
+    #TODO: mask_d array
+    del nomvar, typvar, etiket, datev, ip1, ip2, ip3, dltf, uses_mask, has_mask
+
   # Apply the fill value to the data.
   def _makevars (self):
     from fstd2nc.mixins import _iter_type
     super(Masks,self)._makevars()
     for var in self._varlist:
       if not isinstance(var,_iter_type):
         continue
       # Look for typvars such as 'P@'.
       if var.atts.get('typvar','').endswith('@') or var.atts.get('datyp',0) & 64 == 64:
         try:
           var.atts['_FillValue'] = var.dtype.type(self._fill_value)
         except OverflowError:
           warn(_("Can't set fill value '%g' for %s.")%(self._fill_value,var.name))
 
+  def _decoder_scalar_args (self):
+    args = super(Masks,self)._decoder_scalar_args()
+    args['fill_value'] = self._fill_value
+    return args
+
   # Apply the mask data from raw binary array.
-  def _decode (self, data, unused):
+  @classmethod
+  def _decode (cls, data, fill_value, mask=None, alt_mask=False, **kwargs):
     import numpy as np
-    d = data.view('>i4')
     # Get first field.
-    code1 = (d[12]&0x000FFF00)>>8
-    field1 = super(Masks,self)._decode(data, unused)
+    field1 = super(Masks,cls)._decode(data, **kwargs)
     # If this data is encoded by the datyp+64 flag, then mask out the
     # largest value, assuming the mask was generated by (max-min)*1.01
     # or something similar.
     # TODO: Use the proper interface once it's wrapped in rpnpy.
-    if (d[4] & 64) == 64:
+    if alt_mask:
       mx = field1.max()
-      field1 = np.where(field1==mx, self._fill_value, field1)
-      return field1
-    # If typvar doesn't end in '@', then nothing to do here.
-    if (code1 & 0x3F) != 32:
+      field1 = np.where(field1==mx, fill_value, field1)
       return field1
-    # Find out where the next field should be.
-    swa = d[1]
-    offset = d[0]&(0x00FFFFFF)
-    while offset < len(d)//2 and (swa+offset != d[offset*2+1] or d[offset*2] == 2308):
-      offset += 1
-    else:
-      # No extra fields found?
-      if offset >= len(d)//2:
-        # Since the mask wasn't conveniently located right after the data
-        # record, need to go hunting for it.
-        # TODO: search for it ahead of time (in __init__ stage) if an efficient
-        # way of matching masks is found.
-        prm = self._decode_headers(data[:72])
-        criteria = True
-        for name in ('nomvar', 'datev', 'etiket', 'ip1', 'ip2', 'ip3'):
-          criteria = criteria & (self._headers[name] == prm[name][0])
-        criteria &= (self._headers['typvar'] == b'@@')
-        # Ignore deleted masks
-        criteria &= (self._headers['dltf'] == 0)
-        ind = np.where(criteria)[0]
-        # If still no mask found, then give up.
-        if len(ind) == 0:
-          return field1
-        rec_id = ind[0]
-        filename = self._files[self._headers['file_id'][rec_id]]
-        with open (filename, 'rb') as f:
-          f.seek(int(self._headers['swa'][rec_id])*8-8)
-          mask = np.fromfile(f,'B',self._headers['lng'][rec_id]*4)
-        mask = super(Masks,self)._decode(mask, unused)
-        return ((field1*(mask>0)) + self._fill_value * (mask==0)).astype(field1.dtype)
-    # Ok, back to the case where the other field is available conveniently
-    # after the first.
-    data = data.view('>i4')[offset*2:].view(data.dtype)
-    d = data.view('>i4')
-    # Get second field.
-    code2 = (d[12]&0x000FFF00)>>8
-    field2 = super(Masks,self)._decode(data, unused)
-    # Apply the mask.
-    if code1 == 2080:
-      return (((field1>0)*field2) + self._fill_value * (field1==0)).astype(field2.dtype)
-    elif code2 == 2080:
-      return ((field1*(field2>0)) + self._fill_value * (field2==0)).astype(field1.dtype)
-    else:
-      # Don't know how to apply this typvar for masking purposes.
+    # Is there a mask field available?
+    # Otherwise, nothing else to do here.
+    if mask is None:
       return field1
+    field2 = super(Masks,cls)._decode(mask, **kwargs)
+    return ((field1*(field2>0)) + fill_value * (field2==0)).astype(field1.dtype)
```

### Comparing `fstd2nc-0.20230328.0/fstd2nc/mixins/series.py` & `fstd2nc-0.20230515.0/fstd2nc/mixins/series.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2021 - Climate Research Division
+# Copyright 2017-2023 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
```

### Comparing `fstd2nc-0.20230328.0/fstd2nc/mixins/misc.py` & `fstd2nc-0.20230515.0/fstd2nc/mixins/misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2021 - Climate Research Division
+# Copyright 2017-2023 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
```

### Comparing `fstd2nc-0.20230328.0/fstd2nc/mixins/select.py` & `fstd2nc-0.20230515.0/fstd2nc/mixins/select.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2021 - Climate Research Division
+# Copyright 2017-2023 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
```

### Comparing `fstd2nc-0.20230328.0/fstd2nc/mixins/netcdf.py` & `fstd2nc-0.20230515.0/fstd2nc/mixins/netcdf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2021 - Climate Research Division
+# Copyright 2017-2023 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
@@ -395,18 +395,18 @@
         v = f.createVariable(var.name, datatype=var.array.dtype, dimensions=var.dims, zlib=zlib, complevel=compression)
         # Write the metadata.
         v.setncatts(var.atts)
         v[()] = var.array
         continue
       # Hard case: only have the record indices, need to loop over the records.
       # Get the shape of a single record for the variable.
-      if hasattr(var,'record_id'):
+      if hasattr(var, 'chunks'):
+        continue  #TODO
+      elif hasattr(var,'record_id'):
         record_shape = var.shape[var.record_id.ndim:]
-      elif hasattr(var,'chunksize'):
-        record_shape = var.chunksize
       else:
         continue
       # Use this as the "chunk size" for the netCDF file, to improve I/O
       # performance.
       chunksizes = (1,)*(len(var.axes)-len(record_shape)) + record_shape
       if hasattr(self,'_fill_value') and var.dtype.name.startswith('float32'):
         fill_value = self._fill_value
@@ -446,45 +446,59 @@
     Bar = _ProgressBar if (progress is True and len(io) > 0) else _FakeBar
     bar = Bar(_("Saving netCDF file"), suffix="%(percent)d%% [%(myeta)s]", max=len(io)-1)
     if turbo:
       from multiprocessing import Pool
       import numpy as np
       io = sorted(io)
       with Pool() as p:
-        raw = p.imap (_quick_load, ((self._files[self._headers['file_id'][r]], self._headers['address'][r], self._headers['length'][r]) for r,shape,v,ind in io))
+        raw = p.imap (_quick_load, ((self, r) for r,shape,v,ind in io))
         raw = bar.iter(raw)
         for (r,shape,v,ind), stuff in zip(io, raw):
-          data = self._decode (stuff, r)
+          data = self._decode (**stuff)
           v[ind] = data.astype(v.dtype).reshape(shape)
         bar.finish()
     else:
       for r,shape,v,ind in bar.iter(sorted(io)):
         try:
-          stuff = _quick_load ((self._files[self._headers['file_id'][r]], self._headers['address'][r], self._headers['length'][r]))
-          data = self._decode (stuff, r)
+          stuff = _quick_load ((self, r))
+          data = self._decode (**stuff)
           v[ind] = data.astype(v.dtype).reshape(shape)
         except (IndexError,ValueError):
           warn(_("Internal problem with the script - unable to get data for '%s'")%v.name)
           continue
 
     f.close()
 
   # Alias "to_netcdf" as "write_nc_file" for backwards compatibility.
   write_nc_file = to_netcdf
 
 # Internal helper method for delegating the load to a multiprocessing Pool.
 def _quick_load (args):
   import numpy as np
-  filename, address, length = args
-  # Check if this was from an external source, in which case we have no file
-  # data to provide.  The _decode method will have to find the data from the
-  # other argument (record index).
-  if address is None or length is None:
-    # Return some minimal amount of empty data, in case a mixin tries to
-    # access this data.  This is probably a bad idea (in case the mixin
-    # does something weird with the zero values).
-    #TODO: fix the mixins so they don't try to read these values directly.
-    return np.zeros(256,'B')
-  with open (filename, 'rb') as f:
-    f.seek (address, 0)
-    return np.fromfile(f,'B',length)
+  b, r = args
+  out = dict()
+  # Load data array(s).
+  file_id = b._headers['file_id'][r]
+  if file_id >= 0:
+    filename = b._files[file_id]
+    with open (filename, 'rb') as f:
+      for key, (addr_col,len_col,d_col) in b._decoder_data:
+        if d_col in b._headers and b._headers[d_col][r] is not None:
+          out[key] = b._headers[d_col][r]
+        elif addr_col in b._headers and len_col in b._headers:
+          address = int(b._headers[addr_col][r])
+          length = int(b._headers[len_col][r])
+          if address >= 0 and length >= 0:
+            f.seek (address, 0)
+            out[key] = np.fromfile(f,'B',length)
+  else:
+    for key, (addr_col,len_col,d_col) in b._decoder_data:
+      if d_col in b._headers and b._headers[d_col][r] is not None:
+        out[key] = b._headers[d_col][r]
+
+  # Get other arguments
+  for key in b._decoder_extra_args:
+    if key in b._headers:
+      out[key] = b._headers[key][r]
+  out.update(b._decoder_scalar_args())
+  return out
```

### Comparing `fstd2nc-0.20230328.0/fstd2nc/mixins/extern.py` & `fstd2nc-0.20230515.0/fstd2nc/mixins/extern.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2021 - Climate Research Division
+# Copyright 2017-2023 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
@@ -64,153 +64,207 @@
   class _FSTD_Callback (Callback):
     def _start_state (self, dsk, state):
       # Try sorting by FSTD filename, offset (if applicable)
       try:
         ready = sorted(state['ready'][::-1],key=_RecordOrder(dsk))
         state['ready'] = ready[::-1]
       except TypeError: pass  # Not applicable for this graph.
-  _FSTD_Callback().register()
   del Callback
-
 except ImportError:
   pass
 
+# Only turn on this callback if explicitly requested by the user.
+# It may cause problems when there are large graphs being communicated
+# to a dask cluster environment.
+def force_strict_ordering ():
+  _FSTD_Callback().register()
 
 # Method for reading a block from a file.
 def _read_block (filename, offset, length):
   import numpy as np
+  # Scalar version first.
+  if not hasattr(offset,'__len__'):
+    with open(filename,'rb') as f:
+      f.seek (offset,0)
+      return np.fromfile(f,'B',length)
+  # Vectorized version.
+  out = []
   with open(filename,'rb') as f:
-    f.seek (offset,0)
-    return np.fromfile(f,'B',length)
+    for o, l in zip(offset, length):
+      f.seek (o,0)
+      out.append(np.fromfile(f,'B',l))
+  return out
 
 
 class ExternOutput (BufferBase):
 
-  # Helper method to get graph for raw input data.
-  def _graphs (self):
+  # Helper method to call decode routine using the given inputs.
+  @classmethod
+  def _dasked_decode (cls, *args):
+    keys = args[:-1:2]
+    values = args[1::2]
+    # Scalar case (decoding single record)
+    if not any(isinstance(v,list) for v in values):
+      kwargs = dict(zip(keys,values))
+      return cls._decode(**kwargs)
+    # Vectorized case (decoding multiple records into a single fused array)
+    nrec = [len(v) for v in values if isinstance(v,list)][0]
+    values = [v if isinstance(v,list) else [v]*nrec for v in values]
+    out = []
+    for i in range(nrec):
+      kwargs = dict((k,v[i]) for k,v in zip(keys,values))
+      out.append(cls._decode(**kwargs))
     import numpy as np
-    import pandas as pd
-    graphs = [None] * self._nrecs
-    ###
-    # Special case: already have a dask object from external source.
-    # (E.g., from fstpy)
-    if hasattr(self, '_extern_table'):
-      for rec_id in range(self._nrecs):
-        d = self._extern_table['d'].iloc[rec_id]
-        if hasattr(d,'compute'):
-          # Start a dask graph using the external dask array as the source.
-          graph = (d.compute,)
-          graph = (np.ravel, graph, 'K')
-        else:  # Special case: have a numpy array in memory.
-          graph = d
-          graph = np.ravel(graph, 'K')
-        graphs[rec_id] = graph
-      return graphs
-    ###
-    # Otherwise, construct graphs with our own dask wrapper.
-    files = np.array(self._files, dtype=object)
-    # Only construct graphs for records that will ultimately appear in the
-    # dask objects.
-    active = self._headers['selected'] == True
-    nrecs = np.sum(active)
-    filenames = files[self._headers['file_id'][active]]
-    graphs = zip([_read_block]*nrecs, filenames, self._headers['address'][active], self._headers['length'][active])
-    graphs = zip([self._decode]*nrecs, graphs, np.where(active)[0])
-    g = np.empty(nrecs, dtype=object)
-    g[:] = list(graphs)
-    out = np.empty(self._nrecs, dtype=object)
-    out[active] = g
-    return out
+    return np.concatenate(out)
 
-  def _iter_dask (self, include_coords=True):
+  def _iter_dask (self, include_coords=True, fused=True):
     """
     Iterate over all the variables, and convert to dask arrays.
     """
     from fstd2nc.mixins import _iter_type, _chunk_type, _var_type
     from dask import array as da
     from dask.base import tokenize
     import numpy as np
     from itertools import product
-    from dask import delayed
     unique_token = tokenize(self._files,id(self))
-    graphs = self._graphs()
+    files = np.array(self._files, dtype=object)
     self._makevars()
     for var in self._iter_objects():
       if not include_coords:
         if var not in self._varlist:
           continue
       if not isinstance(var,(_iter_type,_chunk_type)):
         yield var
         continue
       name = var.name+"-"+unique_token
       ndim = len(var.axes)
       shape = var.shape
       # Convert _iter_type to more generic _chunk_type.
       if isinstance(var,_iter_type):
-        chunks = {}
         ndim_outer = var.record_id.ndim
         ndim_inner = ndim - ndim_outer
-        chunk_shape = shape[ndim_outer:]
-        for ind in product(*map(range,var.record_id.shape)):
-          rec_id = var.record_id[ind]
-          ind = ind + tuple((0,dx) for dx in shape[ndim_outer:])
-          chunks[ind] = rec_id
-        var = _chunk_type (var.name, var.atts, var.axes, var.dtype, chunks, chunk_shape)
-      # Convert _chunk_type to dask Array objects.
-      if isinstance(var,_chunk_type):
-        ndim_inner = len(var.chunksize)
-        ndim_outer = ndim - ndim_inner
-        # Get chunk dimensions.
-        # First, size of single (untruncated) chunk, full indices.
-        untruncated_chunksize = (1,)*(ndim-len(var.chunksize)) + var.chunksize
-        # Next, breakdown of chunks along all variable dimensions.
-        chunks = []
-        chunk_indices = []
-        for i in range(ndim):
-          dx = untruncated_chunksize[i]
-          ch = tuple(dx for j in range(dx,shape[i]+1,dx))
-          if shape[i] % dx > 0:
-            ch = ch + (shape[i] % dx, )
-          chunks.append(ch)
-          chunk_indices.append(range(len(ch)))
-        # Loop over all indices, generate dask graph.
-        dsk = dict()
-        for ind, chunk_shape in zip(product(*chunk_indices), product(*chunks)):
-          # Unique key for this graph member.
-          key = (name,) + ind
-          # Get record id.
-          slices = [(i*dx,i*dx+res) for i,dx,res in zip(ind,untruncated_chunksize,chunk_shape)]
-          slices[:ndim_outer] = ind[:ndim_outer]
-          rec_id = var.chunks.get(tuple(slices),-1)
-          # Add this record as a chunk in the dask Array.
-          # Also, specify the preferred order of reading the chunks within the
-          # file.
-          if rec_id >= 0:
-            graph = graphs[rec_id]
-            dsk[key] = (np.reshape, graph, chunk_shape)
+        chunks = [(1,)*n for n in shape[:ndim_outer]] + [(n,) for n in shape[ndim_outer:]]
+        record_id = var.record_id.reshape(shape[:ndim_outer] + (1,)*ndim_inner)
+        var = _chunk_type (var.name, var.atts, var.axes, var.dtype, chunks, record_id)
+
+      # Fuse the records to make larger (and more dask-friendly) chunks.
+      # Disable fusing for dask-based arrays.
+      # Could make it work, but would need more explicit looping over
+      # records to see where dask arrays are available (slower?)
+      if 'd' in self._headers and any(d is not None for d in self._headers['d'][var.record_id].flatten()):
+        pass # Shut off fusion.
+      elif fused:
+        file_ids = self._headers['file_id'][var.record_id]
+        # Find dimension to fuse.
+        dim = var.record_id.ndim-1
+        while dim >= 0 and len(var.chunks[dim]) == 1:
+          dim -= 1
+        # Check if there is something available to fuse.
+        if dim >= 0:
+          # Look at part of record to guess at number of records to chunk.
+          # Can only chunk within a file.
+          sample = file_ids[(0,)*dim].squeeze()
+          dx = sum(sample==sample[0])
+          # Check if this guessed chunk size works for the data shape.
+          if var.record_id.shape[dim] % dx == 0:
+            if dx > 1:
+              dy = var.record_id.shape[dim] // dx
+              # Check if we always stay within file bounds.
+              shape = var.record_id.shape[:dim] + (dy, dx)
+              check = file_ids.reshape(shape)
+              if np.all(check[...,:] == check[...,0:1]):
+                chunks = list(var.chunks)
+                chunks[dim] = (dx,)*dy
+                shape = var.record_id.shape[:dim] + (dy,) + var.record_id.shape[dim+1:] + (dx,)
+                # Put chunks record ids in extra dimension at end.
+                record_id = var.record_id.reshape(shape)
+                var = _chunk_type (var.name, var.atts, var.axes, var.dtype, chunks, record_id)
+              else:
+                warn(_("Unable to fuse some variables."))
           else:
-            # Fill missing chunks with fill value or NaN.
-            if hasattr(self,'_fill_value'):
-              var.atts['_FillValue'] = self._fill_value
-              dsk[key] = (np.full, chunk_shape, self._fill_value, var.dtype)
-            else:
-              dsk[key] = (np.full, chunk_shape, float('nan'), var.dtype)
-        array = da.Array(dsk, name, chunks, var.dtype)
-        var = _var_type(var.name,var.atts,var.axes,array)
+            warn(_("Unable to fuse some variables."))
+
+      # Transform _chunk_type data from record indices to graphs.
+      # For fused data, use 2D record_id array (chunk, ids).
+      # For unfused data, use 1D record_id array.
+      if var.record_id.ndim > len(var.chunks):
+        record_id = var.record_id.reshape(-1,var.record_id.shape[-1])
+      else:
+        record_id = var.record_id.flatten()
+      file_ids = self._headers['file_id'][record_id]
+      file_ids[record_id<0] = -1
+      # Assume same file within chunk.
+      if file_ids.ndim > 1: file_ids = file_ids[:,0]
+      nchunks = record_id.shape[0]
+      args = []
+      # Add data sources (primary data plus possible secondary like mask).
+      for key, (addr_col, len_col, dname) in self._decoder_data:
+        if addr_col not in self._headers: continue # Skip inactive arguments.
+        fname = files[file_ids]
+        addr = self._headers[addr_col][record_id]
+        if addr.ndim > 1: addr = map(list,addr)
+        length = self._headers[len_col][record_id]
+        if length.ndim > 1: length = map(list,length)
+        rb = zip([_read_block]*nchunks, fname, addr, length)
+        # Skip the _read_blocks construct where we don't have file data.
+        # (e.g. for missing records or where data coming from dask).
+        rb = [_rb if fid >= 0 else None for _rb,fid in zip(rb,file_ids)]
+        # Inject dask array data where it's available.
+        if dname in self._headers:
+          rb = [d if d is not None else _rb for d,_rb in zip(self._headers[dname][record_id].flatten(),rb)]
+        args.extend([[key]*nchunks, rb])
+      # Add extra arguments from columns.
+      for key in self._decoder_extra_args:
+        if key not in self._headers: continue  # Skip inactive arguments.
+        values = self._headers[key][record_id]
+        if values.ndim > 1:
+          values = map(list,values)
+          # For case where all values are identical, reduce to scalar.
+          values = [v[0] if len(set(v)) == 1 else v for v in values]
+        args.extend([[key]*nchunks, values])
+      # Add scalar arguments.
+      for key, value in self._decoder_scalar_args().items():
+        args.extend([[key]*nchunks, [value]*nchunks])
+      graphs = zip([self._dasked_decode]*nchunks, *args)
+      array = np.empty(nchunks, dtype=object)
+      array[:] = list(graphs)
+      shape = tuple(len(c) for c in var.chunks)
+      array = array.reshape(shape)
+
+      # Create dask array from this info.
+      chunk_indices = [np.cumsum((0,)+c)[:-1] for c in var.chunks]
+      # Loop over all indices, generate dask graph.
+      dsk = dict()
+      for ind, chunk_coord, chunk_shape in zip(np.ndindex(array.shape), product(*chunk_indices), product(*var.chunks)):
+        # Unique key for this graph member.
+        key = (name,) + chunk_coord
+        # Add this record as a chunk in the dask Array.
+        graph = array[ind]
+        if graph is not None:
+          dsk[key] = (np.reshape, graph, chunk_shape)
+        else:
+          # Fill missing chunks with fill value or NaN.
+          if hasattr(self,'_fill_value'):
+            var.atts['_FillValue'] = self._fill_value
+            dsk[key] = (np.full, chunk_shape, self._fill_value, var.dtype)
+          else:
+            dsk[key] = (np.full, chunk_shape, float('nan'), var.dtype)
+      array = da.Array(dsk, name, var.chunks, var.dtype)
+      var = _var_type(var.name,var.atts,var.axes,array)
       yield var
 
-  def to_xarray (self):
+  def to_xarray (self, fused=True):
     """
     Create an xarray interface for the RPN data.
     Requires the xarray and dask packages.
     """
     from collections import OrderedDict
     import xarray as xr
     out = OrderedDict()
-    for var in self._iter_dask():
+    for var in self._iter_dask(fused=fused):
       if not hasattr(var,'array'): continue
       out[var.name] = xr.DataArray(data=var.array, dims=var.dims, name=var.name, attrs=var.atts)
       # Preserve chunking information for writing to netCDF4.
       if hasattr(var.array,'chunks'):
         chunk_shape = [c[0] for c in var.array.chunks]
         out[var.name].encoding['chunksizes'] = chunk_shape
         out[var.name].encoding['original_shape'] = out[var.name].shape
@@ -219,30 +273,35 @@
     out = xr.Dataset(out)
     # Decode CF metadata
     out = xr.conventions.decode_cf(out)
 
     # Make the time dimension unlimited when writing to netCDF.
     out.encoding['unlimited_dims'] = ('time',)
 
+    # Remove coordinates from encoding, so that xarray can determine the
+    # appropriate values upon writing to netCDF4.
+    for var in out.variables:
+      out[var].encoding.pop('coordinates',None)
+
     return out
 
-  def to_xarray_list (self):
+  def to_xarray_list (self, fused=True):
     """
     Similar to the to_xarray method, but returns a list of xarray Datasets,
     one for each variable, instead of a single Dataset object.
     Could be useful for case where the dimension names are non-unique, to avoid
     name clobbering (in conjunction with unique_names initialization option).
     E.g.,
     Buffer("filename",unique_names=False).to_xarray_list()
     """
     from collections import OrderedDict
     import xarray as xr
     from fstd2nc.mixins import _axis_type
     out_list = []
-    for var in self._iter_dask(include_coords=False):
+    for var in self._iter_dask(include_coords=False, fused=fused):
       if not hasattr(var,'array'): continue
       out = OrderedDict()
       out[var.name] = xr.DataArray(data=var.array, dims=var.dims, name=var.name, attrs=var.atts)
       for extra in self._iter_objects(var):
         if not hasattr(extra,'array'): continue
         out[extra.name] = xr.DataArray(data=extra.array, dims=extra.dims, name=extra.name, attrs=extra.atts)
       # Preserve chunking information for writing to netCDF4.
@@ -295,54 +354,58 @@
   def to_fstpy (self):
     """
     Create a table compatible with the fstpy module.
     Requires pandas and dask.
     """
     import pandas as pd
     import numpy as np
-    from fstpy.dataframe import add_grid_column
-    from fstpy.std_io import add_dask_column
-    # Special case: our data is already from an fstpy table, not from an FSTD
-    # file in our control.
-    # E.g., if some smartass does Buffer.from_fstpy(df).to_fstpy()
-    if hasattr(self, '_extern_table'):
-      return self._extern_table
+    from fstd2nc.extra import decode
+    from dask import delayed
+    import dask.array as da
     # Put all the header info into a dictionary.
     fields = ['nomvar', 'typvar', 'etiket', 'ni', 'nj', 'nk', 'dateo', 'ip1', 'ip2', 'ip3', 'deet', 'npas', 'datyp', 'nbits', 'grtyp', 'ig1', 'ig2', 'ig3', 'ig4', 'datev']
     table = dict()
     # Create a mask to exclude deleted / overwritten / unselected records.
     # Include all meta (coordinate) records in the output.
     mask = self._headers['selected'] | self._headers['ismeta']
     for field in fields:
       col = self._headers[field][mask]
       # Convert byte arrays to strings, which is what fstpy expects.
       if col.dtype.str.startswith('|S'):
         col = np.asarray(col,dtype=col.dtype.str.replace('|S','<U'))
       table[field] = col
     # Convert to pandas table.
     table = pd.DataFrame.from_dict(table)
-    # Add grid info.
-    add_grid_column (table)
-    # Temporarily insert some extra columns needed for the data.
-    table['shape'] = list(zip(table['ni'],table['nj']))
-    filenames = dict((i,f) for i,f in enumerate(self._files))
-    table['path'] = pd.Series(self._headers['file_id'][mask]).map(filenames)
-    key = np.zeros(len(self._headers['name']),'int32')
-    for file_id in range(len(self._files)):
-      selection = self._headers['file_id'] == file_id
-      indices = np.arange(np.sum(selection), dtype='int32')
-      key[selection] = (indices % 256) | ((indices//256)<<9)
-    table['key'] = key[mask] << 10
-    # Generate dask objects
-    #TODO: use our own, in case we modified the data?
-    # (doesn't normally happen, but you never know...)
-    # For instance could happen if interp is used.
-    add_dask_column(table)
-    # Clean up temporary columns and return.
-    table.drop(columns=['shape','path','key'], inplace=True)
+    # Generate dask objects.
+    # NOTE: using raw (records for this, no transformations / masking applied).
+    if 'file_id' in self._headers and 'address' in self._headers and 'length' in self._headers:
+      filenames = np.array(self._files+[None])
+      filenames = filenames[self._headers['file_id']]
+      arrays = map(delayed(_read_block), filenames, self._headers['address'], self._headers['length'])
+      arrays = map(delayed(decode), arrays)
+      shape = zip(self._headers['nj'], self._headers['ni'])
+      arrays = map(delayed(np.reshape), arrays, shape)
+      arrays = map(delayed(np.transpose), arrays)
+      shape = zip(self._headers['ni'], self._headers['nj'])
+      arrays = map(da.from_delayed, arrays, shape, self._headers['dtype'])
+      arrays = list(arrays)
+      d = np.empty(self._nrecs, dtype=object)
+      isvalid = self._headers['file_id'] >= 0
+      for i in range(self._nrecs):
+        if isvalid[i]:
+          d[i] = arrays[i]
+    else:
+      d = np.empty(self._nrecs, dtype=object)
+    # Check if we already have dask arrays to use.
+    if 'd' in self._headers:
+      isvalid = self._headers['d'] != None
+      for i in range(self._nrecs):
+        if isvalid[i]:
+          d[i] = self._headers['d'][i]
+    table['d'] = d[mask]
     return table
 
 # Workaround for recent xarray (>0.10.0) which changed the methods in the
 # conventions module.
 # Fixes an AttributeError when using to_pygeode().
 def _fix_to_pygeode (fixed=[False]):
   if fixed[0] is True: return
@@ -354,18 +417,14 @@
     if not hasattr(conventions,'maybe_encode_timedelta'):
       conventions.maybe_encode_timedelta = times.CFTimedeltaCoder().encode
   except (ImportError,AttributeError):
     pass
   fixed[0] = True
 
 class ExternInput (BufferBase):
-  def __init__ (self, *args, **kwargs):
-    if '_extern_table' in kwargs:
-      self._extern_table = kwargs.pop('_extern_table')
-    super(ExternInput,self).__init__(*args,**kwargs)
   @classmethod
   def from_fstpy (cls, table, **kwargs):
     import numpy as np
     if hasattr(table,'to_pandas'):
       table = table.to_pandas()
     # Construct the record header info from the table.
     fields = ['nomvar', 'typvar', 'etiket', 'ni', 'nj', 'nk', 'dateo', 'ip1', 'ip2', 'ip3', 'deet', 'npas', 'datyp', 'nbits', 'grtyp', 'ig1', 'ig2', 'ig3', 'ig4', 'datev']
@@ -384,49 +443,23 @@
     if 'dltf' not in headers:
       headers['dltf'] = np.zeros(len(headers['nomvar']), dtype='int32')
       # We don't have file address info, so mark this as 'None' in case
       # any subroutine is looking for this info.
       headers['address'] = np.empty(len(headers['nomvar']), dtype=object)
       headers['length'] = np.empty(len(headers['nomvar']), dtype=object)
     # Fake file id (just so netcdf mixin _quick_load function doesn't crash).
-    headers['file_id'] = np.zeros(len(headers['nomvar']), dtype='int32')
+    headers['file_id'] = np.empty(len(headers['nomvar']), dtype='int32')
+    headers['file_id'][:] = -1
+    # Add in data.
+    headers['d'] = np.empty(len(headers['nomvar']), dtype=object)
+    headers['d'][:] = table['d']
 
     # Encapsulate this info in a structure.
     fake_buffer = cls.__new__(cls)
     fake_buffer._files = [None]
     fake_buffer._headers = headers
 
     # Initialize a Buffer object with this info.
-    # Also save the dataframe for reference.
-    # Will need the dask objects for getting the data.
-    b = cls(fake_buffer, _extern_table=table, **kwargs)
+    b = cls(fake_buffer, **kwargs)
 
     return b
 
-  # Handle external data for read_record method.
-  # Use data from _extern_table.
-  def _read_record (self, rec_id):
-    import numpy as np
-    # Check if there is custom data enabled for this Buffer.
-    if hasattr(self, '_extern_table'):
-      # Extract the record info from the table.
-      rec = self._extern_table.iloc[rec_id].to_dict()
-      # Load the data (if delayed).
-      rec['d'] = np.asarray(rec['d'])
-      return rec['d'].T
-    # Otherwise, continue as usual.
-    return super(ExternInput,self)._read_record (rec_id)
-
-  # Handle external data for _decode method.
-  # In this case, the first argument is ignored (no file data was read).
-  def _decode (self, maybe_data, rec_id):
-    import numpy as np
-    # Check if there is custom data enabled for this Buffer.
-    if hasattr(self, '_extern_table'):
-      # Extract the record info from the table.
-      rec = self._extern_table.iloc[rec_id].to_dict()
-      # Load the data (if delayed).
-      rec['d'] = np.asarray(rec['d'])
-      return rec['d'].T
-    # Otherwise, continue as usual.
-    return super(ExternInput,self)._decode (maybe_data, rec_id)
-
```

### Comparing `fstd2nc-0.20230328.0/fstd2nc/mixins/ascii.py` & `fstd2nc-0.20230515.0/fstd2nc/mixins/ascii.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2021 - Climate Research Division
+# Copyright 2017-2023 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
```

### Comparing `fstd2nc-0.20230328.0/fstd2nc/mixins/xycoords.py` & `fstd2nc-0.20230515.0/fstd2nc/mixins/xycoords.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2021 - Climate Research Division
+# Copyright 2017-2023 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
@@ -803,27 +803,29 @@
     tiles = OrderedDict()
     for var in self._varlist:
       if var.atts.get('grtyp',None) == '#':
         key = tuple([var.atts.get(n,None) for n in self._var_id if n not in ('ni','nj','ig3','ig4')])
         tiles.setdefault(key,[]).append(var)
     self._varlist = [v for v in self._varlist if v.atts.get('grtyp',None) != '#']
     for key, vars in tiles.items():
-      # Get dimensions of a single (untruncated) chunk.
-      chunk_i = max(v.atts['ni'] for v in vars)
-      chunk_j = max(v.atts['nj'] for v in vars)
-      nj, ni = var.shape[-2:]
-      chunks = OrderedDict()
-      for var in vars:
-        for sl in np.ndindex(var.record_id.shape):
-          i1 = var.atts['ig3'] - 1
-          j1 = var.atts['ig4'] - 1
-          i2 = min(i1+chunk_i,ni)
-          j2 = min(j1+chunk_j,nj)
-          chunks[sl+((j1,j2),(i1,i2))] = var.record_id[sl]
-      var = _chunk_type (vars[0].name, vars[0].atts, vars[0].axes, vars[0].dtype, chunks, (chunk_j,chunk_i))
+      #TODO
+      # Get i/j coordinates.
+      ig3_list = sorted(set([v.atts['ig3'] for v in vars]))
+      ig4_list = sorted(set([v.atts['ig4'] for v in vars]))
+      # Arrange the tiles in their natural 2D order.
+      var_tiles = np.empty((len(ig4_list),len(ig3_list)), dtype='object')
+      for v in vars:
+        ind = (ig4_list.index(v.atts['ig4']), ig3_list.index(v.atts['ig3']))
+        var_tiles[ind] = v
+      chunks = [(1,)*n for n in vars[0].record_id.shape] + [tuple(v.atts['nj'] for v in var_tiles[:,0])] + [tuple(v.atts['ni'] for v in var_tiles[0,:])]
+      record_id = np.empty(vars[0].shape[:-2]+var_tiles.shape, dtype=int)
+      record_id[()] = -1
+      for ind in np.ndindex(var_tiles.shape):
+        record_id[...,ind] = var_tiles[ind].record_id
+      var = _chunk_type (vars[0].name, vars[0].atts, vars[0].axes, vars[0].dtype, chunks, record_id)
       self._varlist.append(var)
 
     # Special case - there are no data records, ONLY a pair of lat/lon
     # coordinates.  In this case, include the lat/lon as variables.
     if len(self._varlist) == 0 and len(lats) == 1 and len(lons) == 1:
       self._varlist = [list(lats.values())[0], list(lons.values())[0]]
       # Add grid mapping info.
```

### Comparing `fstd2nc-0.20230328.0/README.md` & `fstd2nc-0.20230515.0/fstd2nc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: fstd2nc
+Version: 0.20230515.0
+Summary: Converts RPN standard files (from Environment Canada) to netCDF files.
+Home-page: https://github.com/neishm/fstd2nc
+Author: Mike Neish
+License: LGPL-3
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: Programming Language :: Python
+Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
+Description-Content-Type: text/markdown
+Provides-Extra: manyfiles
+Provides-Extra: array
+Provides-Extra: iris
+Provides-Extra: pygeode
+License-File: COPYING
+License-File: COPYING.LESSER
+
 [Version française](README_fr.md)
 
 Overview
 ========
 This module provides a mechanism for converting between FSTD and netCDF file formats, either through Python or the command-line.
 
 
@@ -287,7 +309,9 @@
 The `.to_xarray()` Python method requires the [xarray](https://github.com/pydata/xarray) and [dask](https://github.com/dask/dask) packages.
 
 The `.to_iris()` Python method requires the [iris](https://scitools.org.uk/iris/docs/latest/index.html) package, along with the `.to_xarray()` dependencies.
 
 The `.to_pygeode()` Python method requires the [pygeode](https://github.com/pygeode/pygeode) package, along with the `.to_xarray()` dependencies.
 
 The `.to_fstpy()` Python method requires the [fstpy](https://gitlab.science.gc.ca/CMDS/fstpy) package (*internal link*).
+
+
```

