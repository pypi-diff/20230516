# Comparing `tmp/rvc3python-0.2.3.tar.gz` & `tmp/rvc3python-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/corkep/Dropbox/code/RVC3-python/dist/.tmp-6u877iqw/rvc3python-0.2.3.tar", last modified: Sun Jan 15 05:29:42 2023, max compression
+gzip compressed data, was "rvc3python-0.9.0.tar", last modified: Tue May 16 10:36:08 2023, max compression
```

## Comparing `rvc3python-0.2.3.tar` & `rvc3python-0.9.0.tar`

### file list

```diff
@@ -1,89 +1,96 @@
-drwxrwx---   0 corkep     (503) staff       (20)        0 2023-01-15 05:29:42.144052 rvc3python-0.2.3/
--rw-r--r--   0 corkep     (503) staff       (20)     1068 2022-03-03 04:50:52.000000 rvc3python-0.2.3/LICENSE
--rw-r--r--   0 corkep     (503) staff       (20)      300 2022-04-10 21:26:30.000000 rvc3python-0.2.3/MANIFEST.in
--rw-rw----   0 corkep     (503) staff       (20)    12934 2023-01-15 05:29:42.143792 rvc3python-0.2.3/PKG-INFO
--rw-r--r--   0 corkep     (503) staff       (20)    11361 2023-01-05 21:33:30.000000 rvc3python-0.2.3/README.md
-drwxrwx---   0 corkep     (503) staff       (20)        0 2023-01-15 05:29:42.091053 rvc3python-0.2.3/RVC3/
--rw-r--r--   0 corkep     (503) staff       (20)        0 2022-12-04 10:24:14.000000 rvc3python-0.2.3/RVC3/__init__.py
-drwxrwx---   0 corkep     (503) staff       (20)        0 2023-01-15 05:29:42.092124 rvc3python-0.2.3/RVC3/bin/
--rwxr--r--   0 corkep     (503) staff       (20)      115 2022-12-04 09:46:52.000000 rvc3python-0.2.3/RVC3/bin/bdsim_path
--rwxr--r--   0 corkep     (503) staff       (20)     8519 2022-12-05 11:01:49.000000 rvc3python-0.2.3/RVC3/bin/rvctool
-drwxrwx---   0 corkep     (503) staff       (20)        0 2023-01-15 05:29:42.097077 rvc3python-0.2.3/RVC3/examples/
--rw-r--r--   0 corkep     (503) staff       (20)        0 2022-03-27 04:11:07.000000 rvc3python-0.2.3/RVC3/examples/__init__.py
-drwxrwx---   0 corkep     (503) staff       (20)        0 2023-01-15 05:29:42.103034 rvc3python-0.2.3/RVC3/examples/hershey/
--rw-r--r--   0 corkep     (503) staff       (20)     3655 2021-07-07 23:37:23.000000 rvc3python-0.2.3/RVC3/examples/hershey/genhershey.py
--rw-r--r--   0 corkep     (503) staff       (20)    22558 2021-07-07 23:37:37.000000 rvc3python-0.2.3/RVC3/examples/hershey/hershey.json
--rw-r--r--   0 corkep     (503) staff       (20)   109512 2021-04-08 10:54:54.000000 rvc3python-0.2.3/RVC3/examples/hershey/hershey.txt
--rw-r--r--   0 corkep     (503) staff       (20)      271 2021-04-08 10:54:54.000000 rvc3python-0.2.3/RVC3/examples/hershey/roman-plain.txt
--rw-r--r--   0 corkep     (503) staff       (20)      277 2021-04-08 10:54:54.000000 rvc3python-0.2.3/RVC3/examples/hershey/roman-simplex.txt
--rw-r--r--   0 corkep     (503) staff       (20)      287 2021-04-08 10:54:54.000000 rvc3python-0.2.3/RVC3/examples/hershey/roman-triplex.txt
--rwxr--r--   0 corkep     (503) staff       (20)     2514 2023-01-07 00:39:10.000000 rvc3python-0.2.3/RVC3/examples/imu_data.py
--rwxr--r--   0 corkep     (503) staff       (20)      986 2023-01-08 14:11:21.000000 rvc3python-0.2.3/RVC3/examples/mosaic.py
--rwxr--r--   0 corkep     (503) staff       (20)     2099 2022-10-04 10:46:02.000000 rvc3python-0.2.3/RVC3/examples/ransac_line.py
--rwxr--r--   0 corkep     (503) staff       (20)     4114 2023-01-08 13:29:36.000000 rvc3python-0.2.3/RVC3/examples/visodom.py
--rwxr--r--   0 corkep     (503) staff       (20)     3443 2022-03-27 04:59:28.000000 rvc3python-0.2.3/RVC3/examples/walking.py
--rwxr--r--   0 corkep     (503) staff       (20)      985 2022-03-13 02:43:06.000000 rvc3python-0.2.3/RVC3/examples/writing.py
-drwxrwx---   0 corkep     (503) staff       (20)        0 2023-01-15 05:29:42.123092 rvc3python-0.2.3/RVC3/models/
--rw-r--r--   0 corkep     (503) staff       (20)      889 2022-11-21 11:09:41.000000 rvc3python-0.2.3/RVC3/models/IBVS-arm-main.py
--rw-r--r--   0 corkep     (503) staff       (20)     1002 2022-11-27 21:17:34.000000 rvc3python-0.2.3/RVC3/models/IBVS-holonomic-main.py
--rw-r--r--   0 corkep     (503) staff       (20)      720 2022-10-04 10:46:18.000000 rvc3python-0.2.3/RVC3/models/IBVS-main.py
--rw-r--r--   0 corkep     (503) staff       (20)     1764 2022-10-04 10:44:19.000000 rvc3python-0.2.3/RVC3/models/IBVS-nonholonomic-main.py
--rw-r--r--   0 corkep     (503) staff       (20)     1053 2022-01-05 02:19:15.000000 rvc3python-0.2.3/RVC3/models/IBVS-partitioned-main.py
--rw-r--r--   0 corkep     (503) staff       (20)     2212 2022-10-04 10:44:19.000000 rvc3python-0.2.3/RVC3/models/IBVS-quadrotor-main.py
--rw-r--r--   0 corkep     (503) staff       (20)     1244 2022-10-04 10:46:18.000000 rvc3python-0.2.3/RVC3/models/RRMC.py
--rw-r--r--   0 corkep     (503) staff       (20)     1556 2022-10-04 10:46:18.000000 rvc3python-0.2.3/RVC3/models/RRMC2.py
--rw-r--r--   0 corkep     (503) staff       (20)     2494 2022-10-04 10:44:19.000000 rvc3python-0.2.3/RVC3/models/SEA.py
--rw-r--r--   0 corkep     (503) staff       (20)        0 2022-12-04 09:00:09.000000 rvc3python-0.2.3/RVC3/models/__init__.py
--rwxr--r--   0 corkep     (503) staff       (20)     1592 2022-10-04 10:44:19.000000 rvc3python-0.2.3/RVC3/models/braitenberg.py
--rwxr--r--   0 corkep     (503) staff       (20)     2797 2022-10-04 10:44:19.000000 rvc3python-0.2.3/RVC3/models/driveconfig.py
--rwxr--r--   0 corkep     (503) staff       (20)     1326 2022-10-04 10:44:19.000000 rvc3python-0.2.3/RVC3/models/driveline.py
--rwxr--r--   0 corkep     (503) staff       (20)     1305 2022-10-21 09:46:25.000000 rvc3python-0.2.3/RVC3/models/drivepoint.py
--rwxr--r--   0 corkep     (503) staff       (20)     2533 2022-10-04 10:44:19.000000 rvc3python-0.2.3/RVC3/models/drivepursuit.py
--rwxr--r--   0 corkep     (503) staff       (20)      533 2022-10-04 10:44:19.000000 rvc3python-0.2.3/RVC3/models/jointspace.py
--rwxr--r--   0 corkep     (503) staff       (20)      488 2022-10-18 07:20:02.000000 rvc3python-0.2.3/RVC3/models/lanechange.py
--rw-r--r--   0 corkep     (503) staff       (20)     3724 2022-10-04 10:46:02.000000 rvc3python-0.2.3/RVC3/models/opspace.py
--rw-r--r--   0 corkep     (503) staff       (20)     1835 2022-10-04 10:44:19.000000 rvc3python-0.2.3/RVC3/models/ploop.py
--rw-r--r--   0 corkep     (503) staff       (20)     1172 2022-03-08 00:14:23.000000 rvc3python-0.2.3/RVC3/models/ploop_test.py
--rw-r--r--   0 corkep     (503) staff       (20)      666 2022-10-04 10:44:19.000000 rvc3python-0.2.3/RVC3/models/puma_collapse.py
--rwxr--r--   0 corkep     (503) staff       (20)     2090 2022-01-11 11:13:44.000000 rvc3python-0.2.3/RVC3/models/quadrotor-main.py
--rwxr--r--   0 corkep     (503) staff       (20)     3651 2022-10-04 10:44:19.000000 rvc3python-0.2.3/RVC3/models/quadrotor.py
--rw-r--r--   0 corkep     (503) staff       (20)     1155 2022-10-04 10:44:19.000000 rvc3python-0.2.3/RVC3/models/vloop.py
--rw-r--r--   0 corkep     (503) staff       (20)     1379 2022-03-08 00:11:38.000000 rvc3python-0.2.3/RVC3/models/vloop_test.py
--rwxr--r--   0 corkep     (503) staff       (20)      556 2022-10-04 10:46:02.000000 rvc3python-0.2.3/RVC3/models/zerotorque.py
-drwxrwx---   0 corkep     (503) staff       (20)        0 2023-01-15 05:29:42.123938 rvc3python-0.2.3/RVC3/tools/
--rw-r--r--   0 corkep     (503) staff       (20)        0 2022-12-04 10:32:34.000000 rvc3python-0.2.3/RVC3/tools/__init__.py
--rw-r--r--   0 corkep     (503) staff       (20)     7358 2023-01-15 01:05:41.000000 rvc3python-0.2.3/RVC3/tools/rvcprint.py
--rw-r--r--   0 corkep     (503) staff       (20)       72 2022-12-04 21:35:33.000000 rvc3python-0.2.3/Untitled.ipynb
-drwxrwx---   0 corkep     (503) staff       (20)        0 2023-01-15 05:29:42.125820 rvc3python-0.2.3/rvc3python.egg-info/
--rw-rw----   0 corkep     (503) staff       (20)    12934 2023-01-15 05:29:42.000000 rvc3python-0.2.3/rvc3python.egg-info/PKG-INFO
--rw-rw----   0 corkep     (503) staff       (20)     1831 2023-01-15 05:29:42.000000 rvc3python-0.2.3/rvc3python.egg-info/SOURCES.txt
--rw-rw----   0 corkep     (503) staff       (20)        1 2023-01-15 05:29:42.000000 rvc3python-0.2.3/rvc3python.egg-info/dependency_links.txt
--rw-rw----   0 corkep     (503) staff       (20)      115 2023-01-15 05:29:42.000000 rvc3python-0.2.3/rvc3python.egg-info/requires.txt
--rw-rw----   0 corkep     (503) staff       (20)       11 2023-01-15 05:29:42.000000 rvc3python-0.2.3/rvc3python.egg-info/top_level.txt
--rw-rw----   0 corkep     (503) staff       (20)       38 2023-01-15 05:29:42.144145 rvc3python-0.2.3/setup.cfg
--rw-r--r--   0 corkep     (503) staff       (20)     3045 2023-01-15 05:29:15.000000 rvc3python-0.2.3/setup.py
-drwxrwx---   0 corkep     (503) staff       (20)        0 2023-01-15 05:29:42.143158 rvc3python-0.2.3/tools/
--rw-r--r--   0 corkep     (503) staff       (20)        0 2022-12-04 09:17:55.000000 rvc3python-0.2.3/tools/__init__.py
--rw-r--r--   0 corkep     (503) staff       (20)     2604 2022-03-03 04:50:52.000000 rvc3python-0.2.3/tools/bookcheck.py
--rwxr--r--   0 corkep     (503) staff       (20)     1682 2022-03-21 08:31:46.000000 rvc3python-0.2.3/tools/bookurls.py
--rw-r--r--   0 corkep     (503) staff       (20)      973 2021-04-06 07:37:55.000000 rvc3python-0.2.3/tools/crop.py
--rw-r--r--   0 corkep     (503) staff       (20)      570 2021-02-24 23:53:49.000000 rvc3python-0.2.3/tools/export.py
--rwxr--r--   0 corkep     (503) staff       (20)      322 2022-03-13 11:23:18.000000 rvc3python-0.2.3/tools/fixidx.py
--rwxr--r--   0 corkep     (503) staff       (20)     1626 2022-03-23 01:49:56.000000 rvc3python-0.2.3/tools/grepall.py
--rwxr--r--   0 corkep     (503) staff       (20)     1818 2022-05-01 01:28:32.000000 rvc3python-0.2.3/tools/https.py
--rw-r--r--   0 corkep     (503) staff       (20)     1720 2022-10-04 10:44:17.000000 rvc3python-0.2.3/tools/ipy.py
--rwxr--r--   0 corkep     (503) staff       (20)     2955 2022-10-04 10:44:18.000000 rvc3python-0.2.3/tools/m2p.py
--rwxr--r--   0 corkep     (503) staff       (20)     1580 2022-02-20 21:18:03.000000 rvc3python-0.2.3/tools/mgrepall.py
--rw-r--r--   0 corkep     (503) staff       (20)    10722 2022-10-04 10:46:18.000000 rvc3python-0.2.3/tools/pvplus.py
--rw-r--r--   0 corkep     (503) staff       (20)      863 2021-02-22 11:04:45.000000 rvc3python-0.2.3/tools/pycon.py
--rwxr--r--   0 corkep     (503) staff       (20)    21211 2022-01-10 10:10:14.000000 rvc3python-0.2.3/tools/pyrun (original).py
--rw-r--r--   0 corkep     (503) staff       (20)     4828 2021-05-02 01:32:54.000000 rvc3python-0.2.3/tools/pyrun-old.py
--rwxr--r--   0 corkep     (503) staff       (20)    21131 2021-12-29 23:03:44.000000 rvc3python-0.2.3/tools/pyrun-old2.py
--rw-r--r--   0 corkep     (503) staff       (20)     4027 2021-04-28 00:52:30.000000 rvc3python-0.2.3/tools/pyrun-working.py
--rwxr--r--   0 corkep     (503) staff       (20)    22595 2022-10-04 10:46:18.000000 rvc3python-0.2.3/tools/pyrun.py
--rwxr--r--   0 corkep     (503) staff       (20)     1357 2022-03-20 04:51:13.000000 rvc3python-0.2.3/tools/rmfigs.py
--rwxr--r--   0 corkep     (503) staff       (20)      977 2022-01-13 21:06:50.000000 rvc3python-0.2.3/tools/rmoldfigs.py
--rwxr--r--   0 corkep     (503) staff       (20)     1853 2022-10-04 10:44:18.000000 rvc3python-0.2.3/tools/runall.py
--rw-r--r--   0 corkep     (503) staff       (20)     4831 2022-10-04 10:44:19.000000 rvc3python-0.2.3/tools/rvcprint.py
--rw-r--r--   0 corkep     (503) staff       (20)      724 2021-02-22 11:30:43.000000 rvc3python-0.2.3/tools/test1.py
--rwxr--r--   0 corkep     (503) staff       (20)     1418 2022-10-16 21:41:41.000000 rvc3python-0.2.3/tools/tex2py.py
+drwxrwx---   0 corkep     (503) staff       (20)        0 2023-05-16 10:36:08.948825 rvc3python-0.9.0/
+-rw-r--r--   0 corkep     (503) staff       (20)     1068 2022-03-03 04:50:52.000000 rvc3python-0.9.0/LICENSE
+-rw-r--r--   0 corkep     (503) staff       (20)      325 2023-05-01 11:27:49.000000 rvc3python-0.9.0/MANIFEST.in
+-rw-rw----   0 corkep     (503) staff       (20)    17476 2023-05-16 10:36:08.948134 rvc3python-0.9.0/PKG-INFO
+-rw-r--r--   0 corkep     (503) staff       (20)    15779 2023-05-14 01:09:13.000000 rvc3python-0.9.0/README.md
+drwxrwx---   0 corkep     (503) staff       (20)        0 2023-05-16 10:36:08.837525 rvc3python-0.9.0/RVC3/
+-rw-r--r--   0 corkep     (503) staff       (20)      110 2023-01-26 06:28:11.000000 rvc3python-0.9.0/RVC3/__init__.py
+drwxrwx---   0 corkep     (503) staff       (20)        0 2023-05-16 10:36:08.839956 rvc3python-0.9.0/RVC3/bin/
+-rw-rw----   0 corkep     (503) staff       (20)        0 2023-01-25 00:33:56.000000 rvc3python-0.9.0/RVC3/bin/__init__.py
+-rwxr--r--   0 corkep     (503) staff       (20)      170 2023-01-26 06:30:34.000000 rvc3python-0.9.0/RVC3/bin/bdsim_path.py
+-rwxr--r--   0 corkep     (503) staff       (20)    10533 2023-05-01 10:34:07.000000 rvc3python-0.9.0/RVC3/bin/rvctool.py
+drwxrwx---   0 corkep     (503) staff       (20)        0 2023-05-16 10:36:08.846446 rvc3python-0.9.0/RVC3/examples/
+-rw-r--r--   0 corkep     (503) staff       (20)        0 2022-03-27 04:11:07.000000 rvc3python-0.9.0/RVC3/examples/__init__.py
+drwxrwx---   0 corkep     (503) staff       (20)        0 2023-05-16 10:36:08.873358 rvc3python-0.9.0/RVC3/examples/hershey/
+-rw-r--r--   0 corkep     (503) staff       (20)     3655 2021-07-07 23:37:23.000000 rvc3python-0.9.0/RVC3/examples/hershey/genhershey.py
+-rw-r--r--   0 corkep     (503) staff       (20)    22558 2021-07-07 23:37:37.000000 rvc3python-0.9.0/RVC3/examples/hershey/hershey.json
+-rw-r--r--   0 corkep     (503) staff       (20)   109512 2021-04-08 10:54:54.000000 rvc3python-0.9.0/RVC3/examples/hershey/hershey.txt
+-rw-r--r--   0 corkep     (503) staff       (20)      271 2021-04-08 10:54:54.000000 rvc3python-0.9.0/RVC3/examples/hershey/roman-plain.txt
+-rw-r--r--   0 corkep     (503) staff       (20)      277 2021-04-08 10:54:54.000000 rvc3python-0.9.0/RVC3/examples/hershey/roman-simplex.txt
+-rw-r--r--   0 corkep     (503) staff       (20)      287 2021-04-08 10:54:54.000000 rvc3python-0.9.0/RVC3/examples/hershey/roman-triplex.txt
+-rwxr--r--   0 corkep     (503) staff       (20)     2514 2023-01-07 00:39:10.000000 rvc3python-0.9.0/RVC3/examples/imu_data.py
+-rwxr--r--   0 corkep     (503) staff       (20)      986 2023-01-08 14:11:21.000000 rvc3python-0.9.0/RVC3/examples/mosaic.py
+-rwxr--r--   0 corkep     (503) staff       (20)     2099 2022-10-04 10:46:02.000000 rvc3python-0.9.0/RVC3/examples/ransac_line.py
+-rwxr--r--   0 corkep     (503) staff       (20)     4114 2023-01-08 13:29:36.000000 rvc3python-0.9.0/RVC3/examples/visodom.py
+-rwxr--r--   0 corkep     (503) staff       (20)     3443 2022-03-27 04:59:28.000000 rvc3python-0.9.0/RVC3/examples/walking.py
+-rwxr--r--   0 corkep     (503) staff       (20)      985 2022-03-13 02:43:06.000000 rvc3python-0.9.0/RVC3/examples/writing.py
+drwxrwx---   0 corkep     (503) staff       (20)        0 2023-05-16 10:36:08.941162 rvc3python-0.9.0/RVC3/models/
+-rwxr-xr--   0 corkep     (503) staff       (20)      908 2023-04-30 06:30:00.000000 rvc3python-0.9.0/RVC3/models/IBVS-arm-main.py
+-rw-r--r--   0 corkep     (503) staff       (20)    43781 2023-05-12 05:09:05.000000 rvc3python-0.9.0/RVC3/models/IBVS-arm.bd
+-rwxr-xr--   0 corkep     (503) staff       (20)     1155 2023-04-30 06:30:25.000000 rvc3python-0.9.0/RVC3/models/IBVS-holonomic-main.py
+-rw-r--r--   0 corkep     (503) staff       (20)    40660 2023-05-12 05:09:30.000000 rvc3python-0.9.0/RVC3/models/IBVS-holonomic.bd
+-rwxr-xr--   0 corkep     (503) staff       (20)      586 2023-05-03 10:34:50.000000 rvc3python-0.9.0/RVC3/models/IBVS-main.py
+-rwxr-xr--   0 corkep     (503) staff       (20)     1922 2023-04-30 06:43:51.000000 rvc3python-0.9.0/RVC3/models/IBVS-nonholonomic-main.py
+-rw-r--r--   0 corkep     (503) staff       (20)    71669 2023-05-12 05:09:39.000000 rvc3python-0.9.0/RVC3/models/IBVS-nonholonomic.bd
+-rwxr-xr--   0 corkep     (503) staff       (20)      997 2023-05-03 10:35:10.000000 rvc3python-0.9.0/RVC3/models/IBVS-partitioned-main.py
+-rw-r--r--   0 corkep     (503) staff       (20)    47445 2023-05-12 05:09:57.000000 rvc3python-0.9.0/RVC3/models/IBVS-partitioned.bd
+-rwxr-xr--   0 corkep     (503) staff       (20)     3614 2023-04-30 22:13:37.000000 rvc3python-0.9.0/RVC3/models/IBVS-quadrotor-main.py
+-rw-r--r--   0 corkep     (503) staff       (20)    67100 2023-05-12 05:10:35.000000 rvc3python-0.9.0/RVC3/models/IBVS-quadrotor.bd
+-rw-r--r--   0 corkep     (503) staff       (20)    30462 2022-10-04 10:46:18.000000 rvc3python-0.9.0/RVC3/models/IBVS.bd
+-rw-r--r--   0 corkep     (503) staff       (20)    11048 2022-10-04 10:46:18.000000 rvc3python-0.9.0/RVC3/models/RRMC.bd
+-rwxr-xr--   0 corkep     (503) staff       (20)      940 2023-05-03 10:35:39.000000 rvc3python-0.9.0/RVC3/models/RRMC.py
+-rw-r--r--   0 corkep     (503) staff       (20)    19606 2022-10-04 10:46:18.000000 rvc3python-0.9.0/RVC3/models/RRMC2.bd
+-rwxr-xr--   0 corkep     (503) staff       (20)     1682 2023-05-03 10:35:54.000000 rvc3python-0.9.0/RVC3/models/RRMC2.py
+-rwxr-x---   0 corkep     (503) staff       (20)      572 2023-04-30 06:09:05.000000 rvc3python-0.9.0/RVC3/models/SEA-main.py
+-rw-r--r--   0 corkep     (503) staff       (20)    43915 2023-04-30 04:14:43.000000 rvc3python-0.9.0/RVC3/models/SEA.bd
+-rwxr-xr--   0 corkep     (503) staff       (20)     2602 2023-05-03 10:36:23.000000 rvc3python-0.9.0/RVC3/models/SEA.py
+-rwxr-xr--   0 corkep     (503) staff       (20)        0 2022-12-04 09:00:09.000000 rvc3python-0.9.0/RVC3/models/__init__.py
+-rw-r--r--   0 corkep     (503) staff       (20)    26126 2023-05-12 05:03:56.000000 rvc3python-0.9.0/RVC3/models/braitenberg.bd
+-rwxr-xr--   0 corkep     (503) staff       (20)     1639 2023-05-03 10:36:41.000000 rvc3python-0.9.0/RVC3/models/braitenberg.py
+-rw-r--r--   0 corkep     (503) staff       (20)     6868 2022-10-04 10:44:19.000000 rvc3python-0.9.0/RVC3/models/cartspace.bd
+-rwxr-x---   0 corkep     (503) staff       (20)      541 2023-04-30 06:05:47.000000 rvc3python-0.9.0/RVC3/models/computed-torque-main.py
+-rw-r--r--   0 corkep     (503) staff       (20)    26667 2023-04-30 01:25:50.000000 rvc3python-0.9.0/RVC3/models/computed-torque.bd
+-rw-r--r--   0 corkep     (503) staff       (20)    47832 2022-10-04 10:44:19.000000 rvc3python-0.9.0/RVC3/models/driveconfig.bd
+-rwxr-xr--   0 corkep     (503) staff       (20)     3001 2023-05-03 10:36:53.000000 rvc3python-0.9.0/RVC3/models/driveconfig.py
+-rw-r--r--   0 corkep     (503) staff       (20)    24930 2022-10-04 10:46:02.000000 rvc3python-0.9.0/RVC3/models/driveline.bd
+-rwxr-xr--   0 corkep     (503) staff       (20)     1656 2023-05-03 10:37:05.000000 rvc3python-0.9.0/RVC3/models/driveline.py
+-rw-r--r--   0 corkep     (503) staff       (20)    27760 2022-10-04 10:46:18.000000 rvc3python-0.9.0/RVC3/models/drivepoint.bd
+-rwxr-xr--   0 corkep     (503) staff       (20)     1582 2023-05-03 10:37:14.000000 rvc3python-0.9.0/RVC3/models/drivepoint.py
+-rw-r--r--   0 corkep     (503) staff       (20)    23208 2023-04-18 11:09:49.000000 rvc3python-0.9.0/RVC3/models/drivepursuit.bd
+-rwxr-xr--   0 corkep     (503) staff       (20)     2593 2023-05-03 10:37:30.000000 rvc3python-0.9.0/RVC3/models/drivepursuit.py
+-rwxr-x---   0 corkep     (503) staff       (20)      714 2023-05-07 10:28:12.000000 rvc3python-0.9.0/RVC3/models/feedforward-main.py
+-rw-r--r--   0 corkep     (503) staff       (20)    32877 2023-05-12 05:07:32.000000 rvc3python-0.9.0/RVC3/models/feedforward.bd
+-rw-r--r--   0 corkep     (503) staff       (20)     8695 2022-10-04 10:44:19.000000 rvc3python-0.9.0/RVC3/models/jointspace.bd
+-rwxr-xr--   0 corkep     (503) staff       (20)      619 2023-04-30 23:26:33.000000 rvc3python-0.9.0/RVC3/models/jointspace.py
+-rw-r--r--   0 corkep     (503) staff       (20)     5273 2023-04-18 21:48:51.000000 rvc3python-0.9.0/RVC3/models/lanechange.bd
+-rwxr-xr--   0 corkep     (503) staff       (20)      609 2023-05-03 10:37:50.000000 rvc3python-0.9.0/RVC3/models/lanechange.py
+-rwxr-x---   0 corkep     (503) staff       (20)     1856 2023-05-12 04:59:54.000000 rvc3python-0.9.0/RVC3/models/opspace-main.py
+-rw-r--r--   0 corkep     (503) staff       (20)    57493 2023-05-12 04:51:21.000000 rvc3python-0.9.0/RVC3/models/opspace.bd
+-rwxr-xr--   0 corkep     (503) staff       (20)     3860 2023-05-12 04:54:29.000000 rvc3python-0.9.0/RVC3/models/opspace.py
+-rw-r--r--   0 corkep     (503) staff       (20)    24713 2022-10-04 10:44:19.000000 rvc3python-0.9.0/RVC3/models/ploop.bd
+-rwxr-xr--   0 corkep     (503) staff       (20)     1980 2023-04-30 06:07:17.000000 rvc3python-0.9.0/RVC3/models/ploop.py
+-rw-r--r--   0 corkep     (503) staff       (20)    11860 2022-11-21 10:01:57.000000 rvc3python-0.9.0/RVC3/models/ploop_test.bd
+-rwxr-xr--   0 corkep     (503) staff       (20)     1206 2023-05-03 10:38:27.000000 rvc3python-0.9.0/RVC3/models/ploop_test.py
+-rwxr-x---   0 corkep     (503) staff       (20)     4407 2023-03-13 03:01:39.000000 rvc3python-0.9.0/RVC3/models/quad_model.py
+-rwxr-xr--   0 corkep     (503) staff       (20)     2172 2023-05-03 10:38:49.000000 rvc3python-0.9.0/RVC3/models/quadrotor-main.py
+-rw-r--r--   0 corkep     (503) staff       (20)    57216 2023-05-12 05:12:18.000000 rvc3python-0.9.0/RVC3/models/quadrotor.bd
+-rwxr-xr--   0 corkep     (503) staff       (20)     3760 2023-05-03 10:39:10.000000 rvc3python-0.9.0/RVC3/models/quadrotor.py
+-rw-r--r--   0 corkep     (503) staff       (20)    39699 2022-10-04 10:44:19.000000 rvc3python-0.9.0/RVC3/models/vloop.bd
+-rwxr-xr--   0 corkep     (503) staff       (20)     1290 2023-04-30 06:09:33.000000 rvc3python-0.9.0/RVC3/models/vloop.py
+-rw-r--r--   0 corkep     (503) staff       (20)    16230 2022-01-05 20:50:13.000000 rvc3python-0.9.0/RVC3/models/vloop_test.bd
+-rwxr-xr--   0 corkep     (503) staff       (20)     1340 2023-05-03 10:39:25.000000 rvc3python-0.9.0/RVC3/models/vloop_test.py
+-rw-r--r--   0 corkep     (503) staff       (20)     3690 2022-10-04 10:44:19.000000 rvc3python-0.9.0/RVC3/models/zerotorque.bd
+-rwxr-xr--   0 corkep     (503) staff       (20)      662 2023-05-03 10:39:34.000000 rvc3python-0.9.0/RVC3/models/zerotorque.py
+drwxrwx---   0 corkep     (503) staff       (20)        0 2023-05-16 10:36:08.943149 rvc3python-0.9.0/RVC3/tools/
+-rw-r--r--   0 corkep     (503) staff       (20)        0 2022-12-04 10:32:34.000000 rvc3python-0.9.0/RVC3/tools/__init__.py
+-rw-r--r--   0 corkep     (503) staff       (20)     7358 2023-01-15 01:05:41.000000 rvc3python-0.9.0/RVC3/tools/rvcprint.py
+-rw-r--r--   0 corkep     (503) staff       (20)       72 2022-12-04 21:35:33.000000 rvc3python-0.9.0/Untitled.ipynb
+-rw-rw----   0 corkep     (503) staff       (20)     2646 2023-05-14 01:14:42.000000 rvc3python-0.9.0/pyproject.toml
+drwxrwx---   0 corkep     (503) staff       (20)        0 2023-05-16 10:36:08.947338 rvc3python-0.9.0/rvc3python.egg-info/
+-rw-rw----   0 corkep     (503) staff       (20)    17476 2023-05-16 10:36:08.000000 rvc3python-0.9.0/rvc3python.egg-info/PKG-INFO
+-rw-rw----   0 corkep     (503) staff       (20)     2272 2023-05-16 10:36:08.000000 rvc3python-0.9.0/rvc3python.egg-info/SOURCES.txt
+-rw-rw----   0 corkep     (503) staff       (20)        1 2023-05-16 10:36:08.000000 rvc3python-0.9.0/rvc3python.egg-info/dependency_links.txt
+-rw-rw----   0 corkep     (503) staff       (20)       88 2023-05-16 10:36:08.000000 rvc3python-0.9.0/rvc3python.egg-info/entry_points.txt
+-rw-rw----   0 corkep     (503) staff       (20)      129 2023-05-16 10:36:08.000000 rvc3python-0.9.0/rvc3python.egg-info/requires.txt
+-rw-rw----   0 corkep     (503) staff       (20)        5 2023-05-16 10:36:08.000000 rvc3python-0.9.0/rvc3python.egg-info/top_level.txt
+-rw-rw----   0 corkep     (503) staff       (20)       38 2023-05-16 10:36:08.948956 rvc3python-0.9.0/setup.cfg
```

### Comparing `rvc3python-0.2.3/LICENSE` & `rvc3python-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rvc3python-0.2.3/PKG-INFO` & `rvc3python-0.9.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,67 +1,77 @@
-Metadata-Version: 2.1
-Name: rvc3python
-Version: 0.2.3
-Summary: Support for book: Robotics, Vision & Control 3 in Python
-Home-page: https://github.com/petercorke/RVC3-python
-Author: Peter Corke
-License: MIT
-Project-URL: Documentation, https://petercorke.github.io/RVC3-python
-Project-URL: Source, https://github.com/petercorke/RVC3-python
-Project-URL: Tracker, https://github.com/petercorke/RVC3-python/issues
-Keywords: robotics,robot,manipulator,robot arm,mobile robot,mobile manipulation,path planning,SLAM,pose graph,Dubins,Reeds-Shepp,lattice planner,RRT,PRM,rapidly exploring random tree,probabilistic roadmap planner,force control,kinematics,Jacobian,position control,velocity control,spatial math,SO(2),SE(2),SO(3),SE(3),twist,product of exponential,translation,orientation,angle-axis,Lie group,skew symmetric matrix,pose,translation,rotation matrix,rigid body transform,homogeneous transformation,Euler angles,roll-pitch-yaw angles,quaternion,unit-quaternioncomputer vision,machine vision,robotic vision,color space,blackbody,image segmentation,blobs,Hough transform,k-means,homography,camera calibration,visual odometry,bundle adjustment,stereo vision,rectification
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: pytorch
-License-File: LICENSE
-
 # Robotics, Vision & Control: 3rd edition in Python (2023)
 [![A Python Robotics Package](https://raw.githubusercontent.com/petercorke/robotics-toolbox-python/master/.github/svg/py_collection.min.svg)](https://github.com/petercorke/robotics-toolbox-python)
 [![QUT Centre for Robotics Open Source](https://github.com/qcr/qcr.github.io/raw/master/misc/badge.svg)](https://qcr.github.io)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 [![PyPI version](https://badge.fury.io/py/rvc3python.svg)](https://badge.fury.io/py/rvc3python)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rvc3python.svg)
 [![PyPI - Downloads](https://img.shields.io/pypi/dw/rvc3python)](https://pypistats.org/packages/rvc3python)
 
-
-coming soon, this is a work in progress, please don't post issues
-
+<table style="border:0px">
+<tr style="border:0px">
+<td style="border:0px">
 <img src="https://github.com/petercorke/RVC3-python/raw/main/doc/frontcover.png" alt="Front cover 978-3-031-06468-5_5208" width="300">
+</td>
+<td style="border:0px">
+Welcome to the online hub for the book:
+<ul type="none">
+<li><b>Robotics, Vision & Control</b>: fundamental algorithms in Python (3rd edition) 
+<li>Peter Corke, published by Springer-Nature 2023.</li>
+<li><b>ISBN</b> 978-3-031-06468-5 (hardcopy), 978-3-031-06469-2 (eBook)</li>
+<li><b>DOI</b> <a href="https://doi.org/10.1007/978-3-031-06469-2">10.1007/978-3-031-06469-2</a></li>
+</ul>
+<br><br>
+<p>Report an issue with the book or its supporting code <a href="https://github.com/petercorke/RVC3-python/issues/new/choose">here</a>.</p>
+
+<p>Knwon errata for the book can be viewed <a href="https://github.com/petercorke/RVC3-python/wiki/Errata">here</a>.</p>
+</td>
+</tr>
+</table>
 
-This book depends on the following open-source Python packages
 
-<a href="https://github.com/petercorke/robotics-toolbox-python"><img alt="Robotics Toolbox for Python" src="https://github.com/petercorke/robotics-toolbox-python/raw/master/docs/figs/RobToolBox_RoundLogoB.png" width="150"></a>
+This book uses many examples based on the following open-source Python packages
+
+<a href="https://github.com/petercorke/robotics-toolbox-python"><img alt="Robotics Toolbox for Python" src="https://github.com/petercorke/robotics-toolbox-python/raw/master/docs/figs/RobToolBox_RoundLogoB.png" width="130"></a>
 <a href="https://github.com/petercorke/machinevision-toolbox-python"><img alt="Machine Vision Toolbox for Python" src="https://github.com/petercorke/machinevision-toolbox-python/raw/master/figs/VisionToolboxLogo_NoBackgnd@2x.png" width="150"></a>
+<a href="https://github.com/petercorke/spatialmath-python"><img alt="Spatial Maths Toolbox for Python" src="https://github.com/petercorke/spatialmath-python/raw/master/docs/figs/CartesianSnakes_LogoW.png" width="130"></a>
+<a href="https://github.com/petercorke/bdsim"><img alt="Block diagram simulation for Python" src="https://github.com/petercorke/bdsim/raw/master/figs/BDSimLogo_NoBackgnd@2x.png" width="250"></a>
 
-which in turn have dependencies on other packages created by the author and
+**Robotics Toolbox for Python**, **Machine Vision Toolbox for Python**, **Spatial Maths Toolbox for Python**, **Block Diagram Simulation for Python**.  These in turn have dependencies on other packages created by the author and
 third parties.
 
 ## Installing the package
 
-This package provides a simple one-step installation of the required Toolboxes
+This package provides a simple one-step installation of *all* the required Toolboxes
 ```shell
 pip install rvc3python
 ```
 or
 ```shell
 conda install rvc3python
 ```
 
+There are a lot of dependencies and this might take a minute or so.  You now have a very
+powerful computing environment for robotics and computer vision.
+
+### Python version
+
+Given the rapid rate of language additions, particularly around type hinting, use at
+least Python 3.8.  Python 3.7 goes end of life in June 2023.
+
+Not all package dependencies will work with the latest release of Python.  In particular, check:
+* [PyTorch](https://pypi.org/project/torch/) used for segmentation examples in Chapter 12
+* [Open3D](https://pypi.org/project/open3d), used for point cloud examples in Chapter 14.
+
 ### Installing into a Conda environment
 
 It's probably a good idea to create a virtual environment to keep this package
-and its dependencies separated from your other Python code and projects.  This
-is really easy using Conda conda, and only adds a couple of extra lines
+and its dependencies separated from your other Python code and projects.  If you've
+never used virtual environments before this might be a good time to start, and it
+is really easy [using Conda](https://conda.io/projects/conda/en/latest/user-guide/install/index.html):
 ```shell
 conda create -n RVC3 python=3.10
 conda activate RVC3
 pip install rvc3python
 ```
 
 ### Installing deep learning tools
@@ -83,44 +93,51 @@
 $ rvctool
  ____       _           _   _             __     ___     _                ___      ____            _             _   _____ 
 |  _ \ ___ | |__   ___ | |_(_) ___ ___    \ \   / (_)___(_) ___  _ __    ( _ )    / ___|___  _ __ | |_ _ __ ___ | | |___ / 
 | |_) / _ \| '_ \ / _ \| __| |/ __/ __|    \ \ / /| / __| |/ _ \| '_ \   / _ \/\ | |   / _ \| '_ \| __| '__/ _ \| |   |_ \ 
 |  _ < (_) | |_) | (_) | |_| | (__\__ \_    \ V / | \__ \ | (_) | | | | | (_>  < | |__| (_) | | | | |_| | | (_) | |  ___) |
 |_| \_\___/|_.__/ \___/ \__|_|\___|___( )    \_/  |_|___/_|\___/|_| |_|  \___/\/  \____\___/|_| |_|\__|_|  \___/|_| |____/ 
                                       |/                                                                                   
-for Python (RTB==1.0.2, MVTB==0.9.1, SMTB==1.0.0)
-
-import numpy as np
-import scipy as sp
-import matplotlib.pyplot as plt
-from math import pi
-from spatialmath import *
-from spatialmath.base import *
-from roboticstoolbox import *
-from machinevisiontoolbox import *
-import machinevisiontoolbox.base as mvbase
-
-func/object?       - show brief help
-help(func/object)  - show detailed help
-func/object??      - show source code
+                                                                                 
+for Python (RTB==1.1.0, MVTB==0.9.5, SG==1.1.7, SMTB==1.1.7, NumPy==1.24.2, SciPy==1.10.1, Matplotlib==3.7.1)
 
+    import math
+    import numpy as np
+    from scipy import linalg, optimize
+    import matplotlib.pyplot as plt
+    from spatialmath import *
+    from spatialmath.base import *
+    from spatialmath.base import sym
+    from spatialgeometry import *
+    from roboticstoolbox import *
+    from machinevisiontoolbox import *
+    import machinevisiontoolbox.base as mvb
+    
+    # useful variables
+    from math import pi
+    puma = models.DH.Puma560()
+    panda = models.DH.Panda()
+
+    func/object?       - show brief help
+    help(func/object)  - show detailed help
+    func/object??      - show source code
 
 Results of assignments will be displayed, use trailing ; to suppress
-
- 
-Python 3.8.5 (default, Sep  4 2020, 02:22:02) 
+    
+Python 3.10.9 | packaged by conda-forge | (main, Feb  2 2023, 20:24:27) [Clang 14.0.6 ]
 Type 'copyright', 'credits' or 'license' for more information
-IPython 8.0.1 -- An enhanced Interactive Python. Type '?' for help.
+IPython 8.11.0 -- An enhanced Interactive Python. Type '?' for help.
 
 
 >>> 
 ```
 
-This provides an interactive Python (IPython) session with all the Toolboxes
-preloaded, and ready to go.  It's a highly capable, convenient, and
+This provides an interactive Python
+([IPython](https://ipython.readthedocs.io/en/stable)) session with all the Toolboxes and
+supporting packages imported, and ready to go.  It's a highly capable, convenient, and
 "MATLAB-like" workbench environment for robotics and computer vision.
 
 For example to load an ETS model of a Panda robot, solve a forward kinematics
 and inverse kinematics problem, and an interactive graphical display is simply:
 
 ```python
 >>> panda = models.ETS.Panda()
@@ -172,37 +189,82 @@
 >>> matches = sf1.match(sf2)
 >>> matches.subset(100).plot("w")
 ```
 ![](https://github.com/petercorke/machinevision-toolbox-python/raw/master/figs/matching.png)
 
 `rvctool` is a wrapper around
 [IPython](https://ipython.readthedocs.io/en/stable) where:
-- functions and classes can be accessed without needing package prefixes
+- robotics and vision functions and classes can be accessed without needing
+  package prefixes
 - results are displayed by default like MATLAB does, and like MATLAB you need to
   put a semicolon on the end of the line to prevent this
 - the prompt is the standard Python REPL prompt `>>>` rather than the IPython
   prompt, this can be overridden by a command-line switch
 - allows cutting and pasting in lines from the book, and prompt characters are
   ignored
 
 The Robotics, Vision & Control book uses `rvctool` for all the included
 examples.
 
 `rvctool` imports the all the above mentioned packages using `import *` which is
 not considered best Python practice.  It is very convenient for interactive
-experimentation, but in your own code you can control the imports as you see
+experimentation, but in your own code you can handle the imports as you see
 fit.
 
+### Cutting and pasting
+
+IPython is very forgiving when it comes to cutting and pasting in blocks of Python
+code.  It will strip off the `>>>` prompt character and ignore indentation.  The normal
+python REPL is not so forgiving.  IPython also allows maintains a command history and
+allows command editing.
+### Simple scripting
+You can write very simple scripts, for example `test.py` is
+
+```python
+T = puma.fkine(puma.qn)
+sol = puma.ikine_LM(T)
+sol.q
+puma.plot(sol.q);
+```
+
+then 
+
+```shell
+$ rvctool test.py
+   0         0         1         0.5963    
+   0         1         0        -0.1501    
+  -1         0         0         0.6575    
+   0         0         0         1         
+
+IKSolution(q=array([7.235e-08,  -0.8335,  0.09396,    3.142,   0.8312,   -3.142]), success=True, iterations=15, searches=1, residual=1.406125546650288e-07, reason='Success')
+array([7.235e-08,  -0.8335,  0.09396,    3.142,   0.8312,   -3.142])
+PyPlot3D backend, t = 0.05, scene:
+  robot: Text(0.0, 0.0, 'Puma 560')
+>>>
+```
+and you are dropped into an IPython session after the script has run.
+
+## Using Jupyter and Colab
+
+Graphics and animations are problematic in these environments, some things work
+well, some don't.  As much as possible I've tweaked the Jupyter notebooks to work
+as best they can in these environments.
+
+For local use the [Jupyter plugin for Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter) is pretty decent.  Colab suffers
+from old versions of major packages (though they are getting better at keeping up to date)
+and animations can suffer from slow update over the network.
 ## Other command line tools
 
-This package provides additional command line tools including:
+Additional command line tools available (from the Robotics Toolbox) include:
 - `eigdemo`, animation showing linear transformation of a rotating unit vector
   which demonstrates eigenvalues and eigenvectors.
-- `tripleangledemo`, experiment with various triple-angle sequences.
-- `twistdemo`, experiment with 3D twists.
+- `tripleangledemo`, Swift visualization that lets you experiment with various triple-angle sequences.
+- `twistdemo`, Swift visualization that lets you experiment with 3D twists. The screw axis is the blue rod and you can
+   position and orient it using the sliders, and adjust its pitch. Then apply a rotation
+   about the screw using the bottom slider.
 # Block diagram models
 
 <a href="https://github.com/petercorke/bdsim"><img
 src="https://github.com/petercorke/bdsim/raw/master/figs/BDSimLogo_NoBackgnd%402x.png"
 alt="bdsim logo" width="300"></a>
 
 Block diagram models are key to the pedagogy of the RVC3 book and 25 models are
@@ -242,11 +304,11 @@
 - The code to produce every Python/Matplotlib (2D) figure in the book, see the [`figures`](figures) folder
 - 3D points clouds from chapter 14, and the code to create them, see
   the [`pointclouds`](../pointclouds) folder.
 - 3D figures from chapters 2-3, 7-9, and the code to create them, see the [`3dfigures`](../3dfigures) folder.
 - All example scripts, see the [`examples`](examples) folder.
 - To run the visual odometry example in Sect. 14.8.3 you need to download two image sequence, each over 100MB, [see the instructions here](https://github.com/petercorke/machinevision-toolbox-python/blob/master/mvtb-data/README.md#install-big-image-files). 
 
-To get this material you must clone the repo
+To get that material you must clone the repo
 ```shell
 git clone https://github.com/petercorke/RVC3-python.git
-```
+```
```

#### html2text {}

```diff
@@ -1,78 +1,86 @@
-Metadata-Version: 2.1 Name: rvc3python Version: 0.2.3 Summary: Support for
-book: Robotics, Vision & Control 3 in Python Home-page: https://github.com/
-petercorke/RVC3-python Author: Peter Corke License: MIT Project-URL:
-Documentation, https://petercorke.github.io/RVC3-python Project-URL: Source,
-https://github.com/petercorke/RVC3-python Project-URL: Tracker, https://
-github.com/petercorke/RVC3-python/issues Keywords:
-robotics,robot,manipulator,robot arm,mobile robot,mobile manipulation,path
-planning,SLAM,pose graph,Dubins,Reeds-Shepp,lattice planner,RRT,PRM,rapidly
-exploring random tree,probabilistic roadmap planner,force
-control,kinematics,Jacobian,position control,velocity control,spatial math,SO
-(2),SE(2),SO(3),SE(3),twist,product of
-exponential,translation,orientation,angle-axis,Lie group,skew symmetric
-matrix,pose,translation,rotation matrix,rigid body transform,homogeneous
-transformation,Euler angles,roll-pitch-yaw angles,quaternion,unit-
-quaternioncomputer vision,machine vision,robotic vision,color
-space,blackbody,image segmentation,blobs,Hough transform,k-
-means,homography,camera calibration,visual odometry,bundle adjustment,stereo
-vision,rectification Classifier: Development Status :: 4 - Beta Classifier:
-Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
-License Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Requires-Python: >=3.7 Description-Content-Type: text/markdown
-Provides-Extra: pytorch License-File: LICENSE # Robotics, Vision & Control: 3rd
-edition in Python (2023) [![A Python Robotics Package](https://
-raw.githubusercontent.com/petercorke/robotics-toolbox-python/master/.github/
-svg/py_collection.min.svg)](https://github.com/petercorke/robotics-toolbox-
-python) [![QUT Centre for Robotics Open Source](https://github.com/qcr/
-qcr.github.io/raw/master/misc/badge.svg)](https://qcr.github.io) [![License:
-MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://
+# Robotics, Vision & Control: 3rd edition in Python (2023) [![A Python Robotics
+Package](https://raw.githubusercontent.com/petercorke/robotics-toolbox-python/
+master/.github/svg/py_collection.min.svg)](https://github.com/petercorke/
+robotics-toolbox-python) [![QUT Centre for Robotics Open Source](https://
+github.com/qcr/qcr.github.io/raw/master/misc/badge.svg)](https://qcr.github.io)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://
 opensource.org/licenses/MIT) [![PyPI version](https://badge.fury.io/py/
 rvc3python.svg)](https://badge.fury.io/py/rvc3python) ![PyPI - Python Version]
 (https://img.shields.io/pypi/pyversions/rvc3python.svg) [![PyPI - Downloads]
 (https://img.shields.io/pypi/dw/rvc3python)](https://pypistats.org/packages/
-rvc3python) coming soon, this is a work in progress, please don't post issues
-[Front cover 978-3-031-06468-5_5208] This book depends on the following open-
-source Python packages [Robotics_Toolbox_for_Python] [Machine_Vision_Toolbox
-for_Python] which in turn have dependencies on other packages created by the
-author and third parties. ## Installing the package This package provides a
-simple one-step installation of the required Toolboxes ```shell pip install
-rvc3python ``` or ```shell conda install rvc3python ``` ### Installing into a
-Conda environment It's probably a good idea to create a virtual environment to
-keep this package and its dependencies separated from your other Python code
-and projects. This is really easy using Conda conda, and only adds a couple of
-extra lines ```shell conda create -n RVC3 python=3.10 conda activate RVC3 pip
-install rvc3python ``` ### Installing deep learning tools Chapter 11 has some
-deep learning examples based on PyTorch. If you don't have PyTorch installed
-you can use the `pytorch` install option ```shell pip install rvc3python
-[pytorch] ``` or ```shell conda install rvc3python[pytorch] ``` ## Using the
-Toolboxes The simplest way to get going is to use the command line tool
-```shell $ rvctool ____ _ _ _ __ ___ _ ___ ____ _ _ _____ | _ \ ___ | |__ ___ |
-|_(_) ___ ___ \ \ / (_)___(_) ___ _ __ ( _ ) / ___|___ _ __ | |_ _ __ ___ | |
-|___ / | |_) / _ \| '_ \ / _ \| __| |/ __/ __| \ \ / /| / __| |/ _ \| '_ \ / _
-\/\ | | / _ \| '_ \| __| '__/ _ \| | |_ \ | _ < (_) | |_) | (_) | |_| | (__\__
-\_ \ V / | \__ \ | (_) | | | | | (_> < | |__| (_) | | | | |_| | | (_) | | ___)
-| |_| \_\___/|_.__/ \___/ \__|_|\___|___( ) \_/ |_|___/_|\___/|_| |_| \___/\/
-\____\___/|_| |_|\__|_| \___/|_| |____/ |/ for Python (RTB==1.0.2, MVTB==0.9.1,
-SMTB==1.0.0) import numpy as np import scipy as sp import matplotlib.pyplot as
-plt from math import pi from spatialmath import * from spatialmath.base import
-* from roboticstoolbox import * from machinevisiontoolbox import * import
-machinevisiontoolbox.base as mvbase func/object? - show brief help help(func/
-object) - show detailed help func/object?? - show source code Results of
-assignments will be displayed, use trailing ; to suppress Python 3.8.5
-(default, Sep 4 2020, 02:22:02) Type 'copyright', 'credits' or 'license' for
-more information IPython 8.0.1 -- An enhanced Interactive Python. Type '?' for
-help. >>> ``` This provides an interactive Python (IPython) session with all
-the Toolboxes preloaded, and ready to go. It's a highly capable, convenient,
-and "MATLAB-like" workbench environment for robotics and computer vision. For
-example to load an ETS model of a Panda robot, solve a forward kinematics and
-inverse kinematics problem, and an interactive graphical display is simply:
-```python >>> panda = models.ETS.Panda() ERobot: Panda (by Franka Emika), 7
-joints (RRRRRRR)
+rvc3python)
+                                     Welcome to the online hub for the book:
+                                         # Robotics, Vision & Control:
+                                           fundamental algorithms in Python
+                                           (3rd edition)
+                                         # Peter Corke, published by Springer-
+                                           Nature 2023.
+                                         # ISBN 978-3-031-06468-5 (hardcopy),
+[Front cover 978-3-031-06468-5_5208]       978-3-031-06469-2 (eBook)
+                                         # DOI 10.1007/978-3-031-06469-2
+
+
+                                     Report an issue with the book or its
+                                     supporting code here.
+                                     Knwon errata for the book can be viewed
+                                     here.
+This book uses many examples based on the following open-source Python packages
+[Robotics_Toolbox_for_Python] [Machine_Vision_Toolbox_for_Python] [Spatial
+Maths_Toolbox_for_Python] [Block_diagram_simulation_for_Python] **Robotics
+Toolbox for Python**, **Machine Vision Toolbox for Python**, **Spatial Maths
+Toolbox for Python**, **Block Diagram Simulation for Python**. These in turn
+have dependencies on other packages created by the author and third parties. ##
+Installing the package This package provides a simple one-step installation of
+*all* the required Toolboxes ```shell pip install rvc3python ``` or ```shell
+conda install rvc3python ``` There are a lot of dependencies and this might
+take a minute or so. You now have a very powerful computing environment for
+robotics and computer vision. ### Python version Given the rapid rate of
+language additions, particularly around type hinting, use at least Python 3.8.
+Python 3.7 goes end of life in June 2023. Not all package dependencies will
+work with the latest release of Python. In particular, check: * [PyTorch]
+(https://pypi.org/project/torch/) used for segmentation examples in Chapter 12
+* [Open3D](https://pypi.org/project/open3d), used for point cloud examples in
+Chapter 14. ### Installing into a Conda environment It's probably a good idea
+to create a virtual environment to keep this package and its dependencies
+separated from your other Python code and projects. If you've never used
+virtual environments before this might be a good time to start, and it is
+really easy [using Conda](https://conda.io/projects/conda/en/latest/user-guide/
+install/index.html): ```shell conda create -n RVC3 python=3.10 conda activate
+RVC3 pip install rvc3python ``` ### Installing deep learning tools Chapter 11
+has some deep learning examples based on PyTorch. If you don't have PyTorch
+installed you can use the `pytorch` install option ```shell pip install
+rvc3python[pytorch] ``` or ```shell conda install rvc3python[pytorch] ``` ##
+Using the Toolboxes The simplest way to get going is to use the command line
+tool ```shell $ rvctool ____ _ _ _ __ ___ _ ___ ____ _ _ _____ | _ \ ___ | |__
+___ | |_(_) ___ ___ \ \ / (_)___(_) ___ _ __ ( _ ) / ___|___ _ __ | |_ _ __ ___
+| | |___ / | |_) / _ \| '_ \ / _ \| __| |/ __/ __| \ \ / /| / __| |/ _ \| '_ \
+/ _ \/\ | | / _ \| '_ \| __| '__/ _ \| | |_ \ | _ < (_) | |_) | (_) | |_| |
+(__\__ \_ \ V / | \__ \ | (_) | | | | | (_> < | |__| (_) | | | | |_| | | (_) |
+| ___) | |_| \_\___/|_.__/ \___/ \__|_|\___|___( ) \_/ |_|___/_|\___/|_| |_|
+\___/\/ \____\___/|_| |_|\__|_| \___/|_| |____/ |/ for Python (RTB==1.1.0,
+MVTB==0.9.5, SG==1.1.7, SMTB==1.1.7, NumPy==1.24.2, SciPy==1.10.1,
+Matplotlib==3.7.1) import math import numpy as np from scipy import linalg,
+optimize import matplotlib.pyplot as plt from spatialmath import * from
+spatialmath.base import * from spatialmath.base import sym from spatialgeometry
+import * from roboticstoolbox import * from machinevisiontoolbox import *
+import machinevisiontoolbox.base as mvb # useful variables from math import pi
+puma = models.DH.Puma560() panda = models.DH.Panda() func/object? - show brief
+help help(func/object) - show detailed help func/object?? - show source code
+Results of assignments will be displayed, use trailing ; to suppress Python
+3.10.9 | packaged by conda-forge | (main, Feb 2 2023, 20:24:27) [Clang 14.0.6 ]
+Type 'copyright', 'credits' or 'license' for more information IPython 8.11.0 -
+- An enhanced Interactive Python. Type '?' for help. >>> ``` This provides an
+interactive Python ([IPython](https://ipython.readthedocs.io/en/stable))
+session with all the Toolboxes and supporting packages imported, and ready to
+go. It's a highly capable, convenient, and "MATLAB-like" workbench environment
+for robotics and computer vision. For example to load an ETS model of a Panda
+robot, solve a forward kinematics and inverse kinematics problem, and an
+interactive graphical display is simply: ```python >>> panda = models.ETS.Panda
+() ERobot: Panda (by Franka Emika), 7 joints (RRRRRRR)
 âââââââ¬ââââââââ¬ââââââââ¬âââââââââ¬ââââââââââââââââââââââââââââââââââââââââââââââ
 âlink â link â joint â parent â ETS: parent to link â
 âââââââ¼ââââââââ¼ââââââââ¼âââââââââ¼ââââââââââââââââââââââââââââââââââââââââââââââ¤
 â 0 â link0 â 0 â BASE â tz(0.333) â Rz(q0) â â 1 â link1 â
 1 â link0 â Rx(-90Â°) â Rz(q1) â â 2 â link2 â 2 â link1 â Rx
 (90Â°) â tz(0.316) â Rz(q2) â â 3 â link3 â 3 â link2 â tx
 (0.0825) â Rx(90Â°) â Rz(q3) â â 4 â link4 â 4 â link3 â tx(-
@@ -98,47 +106,70 @@
 (sigma=5)]).disp() ``` ![](https://github.com/petercorke/machinevision-toolbox-
 python/raw/master/figs/mona%2Bsmooth.png) or load two images of the same scene,
 compute SIFT features and display putative matches ```python >>> sf1 =
 Image.Read("eiffel-1.png", mono=True).SIFT() >>> sf2 = Image.Read("eiffel-
 2.png", mono=True).SIFT() >>> matches = sf1.match(sf2) >>> matches.subset
 (100).plot("w") ``` ![](https://github.com/petercorke/machinevision-toolbox-
 python/raw/master/figs/matching.png) `rvctool` is a wrapper around [IPython]
-(https://ipython.readthedocs.io/en/stable) where: - functions and classes can
-be accessed without needing package prefixes - results are displayed by default
-like MATLAB does, and like MATLAB you need to put a semicolon on the end of the
-line to prevent this - the prompt is the standard Python REPL prompt `>>>`
-rather than the IPython prompt, this can be overridden by a command-line switch
-- allows cutting and pasting in lines from the book, and prompt characters are
-ignored The Robotics, Vision & Control book uses `rvctool` for all the included
-examples. `rvctool` imports the all the above mentioned packages using `import
-*` which is not considered best Python practice. It is very convenient for
-interactive experimentation, but in your own code you can control the imports
-as you see fit. ## Other command line tools This package provides additional
-command line tools including: - `eigdemo`, animation showing linear
-transformation of a rotating unit vector which demonstrates eigenvalues and
-eigenvectors. - `tripleangledemo`, experiment with various triple-angle
-sequences. - `twistdemo`, experiment with 3D twists. # Block diagram models
-[bdsim_logo] Block diagram models are key to the pedagogy of the RVC3 book and
-25 models are included. To simulate these models we use the Python package
-[bdsim](https://github.com/petercorke/bdsim) which can run models: - written in
-Python using [bdsim](https://github.com/petercorke/bdsim#getting-started)
-blocks and wiring. - created graphically using [bdedit](https://github.com/
-petercorke/bdsim#bdedit-the-graphical-editing-tool) and saved as a `.bd` (JSON
-format) file. The models are included in the `RVC3` package when it is
-installed and `rvctool` adds them to the module search path. This means you can
-invoke them from `rvctool` by ```python >>> %run -m vloop_test ``` If you want
-to directly access the folder containing the models, the command line tool
-```shell bdsim_path ``` will display the full path to where they have been
-installed in the Python package tree. # Additional book resources [Front cover
-978-3-031-06468-5_5208] This GitHub repo provides additional resources for
-readers including: - Jupyter notebooks containing all code lines from each
-chapter, see the [`notebooks`](notebooks) folder - The code to produce every
-Python/Matplotlib (2D) figure in the book, see the [`figures`](figures) folder
-- 3D points clouds from chapter 14, and the code to create them, see the
-[`pointclouds`](../pointclouds) folder. - 3D figures from chapters 2-3, 7-9,
-and the code to create them, see the [`3dfigures`](../3dfigures) folder. - All
-example scripts, see the [`examples`](examples) folder. - To run the visual
-odometry example in Sect. 14.8.3 you need to download two image sequence, each
-over 100MB, [see the instructions here](https://github.com/petercorke/
-machinevision-toolbox-python/blob/master/mvtb-data/README.md#install-big-image-
-files). To get this material you must clone the repo ```shell git clone https:/
-/github.com/petercorke/RVC3-python.git ```
+(https://ipython.readthedocs.io/en/stable) where: - robotics and vision
+functions and classes can be accessed without needing package prefixes -
+results are displayed by default like MATLAB does, and like MATLAB you need to
+put a semicolon on the end of the line to prevent this - the prompt is the
+standard Python REPL prompt `>>>` rather than the IPython prompt, this can be
+overridden by a command-line switch - allows cutting and pasting in lines from
+the book, and prompt characters are ignored The Robotics, Vision & Control book
+uses `rvctool` for all the included examples. `rvctool` imports the all the
+above mentioned packages using `import *` which is not considered best Python
+practice. It is very convenient for interactive experimentation, but in your
+own code you can handle the imports as you see fit. ### Cutting and pasting
+IPython is very forgiving when it comes to cutting and pasting in blocks of
+Python code. It will strip off the `>>>` prompt character and ignore
+indentation. The normal python REPL is not so forgiving. IPython also allows
+maintains a command history and allows command editing. ### Simple scripting
+You can write very simple scripts, for example `test.py` is ```python T =
+puma.fkine(puma.qn) sol = puma.ikine_LM(T) sol.q puma.plot(sol.q); ``` then
+```shell $ rvctool test.py 0 0 1 0.5963 0 1 0 -0.1501 -1 0 0 0.6575 0 0 0 1
+IKSolution(q=array([7.235e-08, -0.8335, 0.09396, 3.142, 0.8312, -3.142]),
+success=True, iterations=15, searches=1, residual=1.406125546650288e-07,
+reason='Success') array([7.235e-08, -0.8335, 0.09396, 3.142, 0.8312, -3.142])
+PyPlot3D backend, t = 0.05, scene: robot: Text(0.0, 0.0, 'Puma 560') >>> ```
+and you are dropped into an IPython session after the script has run. ## Using
+Jupyter and Colab Graphics and animations are problematic in these
+environments, some things work well, some don't. As much as possible I've
+tweaked the Jupyter notebooks to work as best they can in these environments.
+For local use the [Jupyter plugin for Visual Studio Code](https://
+marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter) is pretty
+decent. Colab suffers from old versions of major packages (though they are
+getting better at keeping up to date) and animations can suffer from slow
+update over the network. ## Other command line tools Additional command line
+tools available (from the Robotics Toolbox) include: - `eigdemo`, animation
+showing linear transformation of a rotating unit vector which demonstrates
+eigenvalues and eigenvectors. - `tripleangledemo`, Swift visualization that
+lets you experiment with various triple-angle sequences. - `twistdemo`, Swift
+visualization that lets you experiment with 3D twists. The screw axis is the
+blue rod and you can position and orient it using the sliders, and adjust its
+pitch. Then apply a rotation about the screw using the bottom slider. # Block
+diagram models [bdsim_logo] Block diagram models are key to the pedagogy of the
+RVC3 book and 25 models are included. To simulate these models we use the
+Python package [bdsim](https://github.com/petercorke/bdsim) which can run
+models: - written in Python using [bdsim](https://github.com/petercorke/
+bdsim#getting-started) blocks and wiring. - created graphically using [bdedit]
+(https://github.com/petercorke/bdsim#bdedit-the-graphical-editing-tool) and
+saved as a `.bd` (JSON format) file. The models are included in the `RVC3`
+package when it is installed and `rvctool` adds them to the module search path.
+This means you can invoke them from `rvctool` by ```python >>> %run -
+m vloop_test ``` If you want to directly access the folder containing the
+models, the command line tool ```shell bdsim_path ``` will display the full
+path to where they have been installed in the Python package tree. # Additional
+book resources [Front cover 978-3-031-06468-5_5208] This GitHub repo provides
+additional resources for readers including: - Jupyter notebooks containing all
+code lines from each chapter, see the [`notebooks`](notebooks) folder - The
+code to produce every Python/Matplotlib (2D) figure in the book, see the
+[`figures`](figures) folder - 3D points clouds from chapter 14, and the code to
+create them, see the [`pointclouds`](../pointclouds) folder. - 3D figures from
+chapters 2-3, 7-9, and the code to create them, see the [`3dfigures`](../
+3dfigures) folder. - All example scripts, see the [`examples`](examples)
+folder. - To run the visual odometry example in Sect. 14.8.3 you need to
+download two image sequence, each over 100MB, [see the instructions here]
+(https://github.com/petercorke/machinevision-toolbox-python/blob/master/mvtb-
+data/README.md#install-big-image-files). To get that material you must clone
+the repo ```shell git clone https://github.com/petercorke/RVC3-python.git ```
```

### Comparing `rvc3python-0.2.3/RVC3/bin/rvctool` & `rvc3python-0.9.0/RVC3/bin/rvctool.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,292 +5,350 @@
 #
 # Run it from the shell
 #  $ rvctool
 #
 # Default switches can be set using the environent variables RVCTOOL, eg.
 #
 #  setenv RVCTOOL "-n"
-#  export RVCTOOL="-n" 
+#  export RVCTOOL="-n"
 
 # import stuff
 import os
 from pathlib import Path
 import sys
 from importlib.metadata import version
 import argparse
 
 from pygments.token import Token
 from IPython.terminal.prompts import Prompts
 from IPython.terminal.prompts import ClassicPrompts
 from traitlets.config import Config
 import IPython
+import matplotlib as mpl
 
 try:
     from colored import fg, bg, attr
 
     _colored = True
     # print('using colored output')
 except ImportError:
     # print('colored not found')
     _colored = False
 
-parser = argparse.ArgumentParser("rvctool",
-    epilog="To set defaults put the relevant command line switches as a string in the environment varible RVCTOOL.",
-    description="Interactive python enviroment for Robotics & Machine Vision toolboxes")
-parser.add_argument("script", default=None, nargs="?", help="specify script to run")
-parser.add_argument("--backend", "-B", default=None, help="specify graphics backend")
-parser.add_argument(
-    "--color",
-    "-C",
-    default="neutral",
-    help="specify terminal color scheme (neutral, lightbg, nocolor, linux), linux is for dark mode",
-)
-parser.add_argument("--confirmexit", "-x", default=False,
-    help="confirm exit")
-parser.add_argument("--prompt", "-p", default=None,
-    help="input prompt")
-parser.add_argument(
-    "--resultprefix",
-    "-r",
-    default=None,
-    help="execution result prefix, include {} for execution count number",
-)
-parser.add_argument(
-    "--nobanner", "-b",
-    dest="banner",
-    default=True, action="store_false",
-    help="suppress startup banner",
-)
-parser.add_argument(
-    "--nocwd", "-c",
-    dest="cwd",
-    default=True, action="store_false",
-    help="suppress cwd to RVC3 folder",
-)
-parser.add_argument(
-    "--showassign",
-    "-a",
-    default=False,
-    action="store_true",
-    help="do not display the result of assignments",
-)
-parser.add_argument(
-    "--normal", "-n",
-    dest="book",
-    default=True, action="store_false",
-    help="use normal ipython settings for prompts and display on assignment"
-)
-parser.add_argument(
-    "--norobot", "-R",
-    dest="robot",
-    default=True, action="store_false",
-    help="do not import robotics toolbox (RTB-P)"
-)
-parser.add_argument(
-    "--novision", "-V",
-    dest="vision",
-    default=True, action="store_false",
-    help="do not import vision toolbox (MVTB-P)"
-)
-parser.add_argument(
-    "--ansi",
-    default=False,
-    action="store_true",
-    help="use ANSImatrix to display matrices",
-)
-parser.add_argument(
-    "--examples",
-    "-e",
-    default=False,
-    action="store_true",
-    help="change working directory to shipped examples",
-)
-parser.add_argument(
-    "--swift",
-    "-s",
-    default=False,
-    action="store_true",
-    help="use Swift as default backend",
-)
-
-# add options for light/dark mode
-
-env = os.getenv("RVCTOOL")
-if env is not None:
-    # if envariable is set, parse it just like command line options
-    args = parser.parse_args(env.split())
-    # then use it to set the defaults for the actual command line parsing
-    parser.set_defaults(**args.__dict__)
-
-args = parser.parse_args()
-
-sys.argv = [sys.argv[0]]
-
-# http://patorjk.com/software/taag/#p=display&f=Standard&t=RVC%203
-banner = fg("yellow")
-banner += r""" ____       _           _   _             __     ___     _                ___      ____            _             _   _____ 
+# imports for use by IPython and user
+from math import pi  # lgtm [py/unused-import]
+import numpy as np
+from scipy import linalg, optimize
+import matplotlib.pyplot as plt  # lgtm [py/unused-import]
+from spatialmath import *  # lgtm [py/polluting-import]
+from spatialmath.base import *
+from spatialmath.base import sym
+from spatialgeometry import *  # lgtm [py/polluting-import]
+
+
+def parse_arguments():
+    parser = argparse.ArgumentParser(
+        prog="rvctool",
+        epilog=(
+            "To set defaults put the relevant command line switches as a string in the"
+            " environment varible RVCTOOL."
+        ),
+        description=(
+            "Interactive python enviroment for exploring the Robotics & Machine Vision"
+            " toolboxes for Python"
+        ),
+    )
+    parser.add_argument("script", default=None, nargs="?", help="specify script to run")
+
+    parser.add_argument(
+        "-B", "--backend", default=None, help="specify graphics backend"
+    )
+    parser.add_argument(
+        "-C",
+        "--color",
+        default="neutral",
+        help=(
+            "specify terminal color scheme (neutral, lightbg, nocolor, linux), linux is"
+            " for dark mode"
+        ),
+    )
+    parser.add_argument("--confirmexit", "-x", default=False, help="confirm exit")
+    parser.add_argument("--prompt", "-p", default=None, help="input prompt")
+    parser.add_argument(
+        "-r",
+        "--resultprefix",
+        default=None,
+        help="execution result prefix, include {} for execution count number",
+    )
+    parser.add_argument(
+        "-b",
+        "--no-banner",
+        dest="banner",
+        default=True,
+        action="store_false",
+        help="suppress startup banner",
+    )
+    parser.add_argument(
+        "-c",
+        "--nocwd",
+        dest="cwd",
+        default=True,
+        action="store_false",
+        help="suppress cwd to RVC3 folder",
+    )
+    parser.add_argument(
+        "-a",
+        "--showassign",
+        default=False,
+        action="store_true",
+        help="do not display the result of assignments",
+    )
+    parser.add_argument(
+        "-n",
+        "--normal",
+        dest="book",
+        default=True,
+        action="store_false",
+        help="use normal ipython settings for prompts and display on assignment",
+    )
+    parser.add_argument(
+        "-R",
+        "--no-robot",
+        dest="robot",
+        default=True,
+        action="store_false",
+        help="do not import robotics toolbox (RTB-P)",
+    )
+    parser.add_argument(
+        "-V",
+        "--no-vision",
+        dest="vision",
+        default=True,
+        action="store_false",
+        help="do not import vision toolbox (MVTB-P)",
+    )
+    parser.add_argument(
+        "--ansi",
+        default=False,
+        action="store_true",
+        help="use ANSImatrix to display matrices",
+    )
+    parser.add_argument(
+        "-e",
+        "--examples",
+        default=False,
+        action="store_true",
+        help="change working directory to shipped examples",
+    )
+    parser.add_argument(
+        "-s",
+        "--swift",
+        default=False,
+        action="store_true",
+        help="use Swift as default backend",
+    )
+
+    # add options for light/dark mode
+
+    env = os.getenv("RVCTOOL")
+    if env is not None:
+        # if envariable is set, parse it just like command line options
+        args = parser.parse_args(env.split())
+        # then use it to set the defaults for the actual command line parsing
+        parser.set_defaults(**args.__dict__)
+
+    args, rest = parser.parse_known_args()
+
+    # remove the arguments we've just parsed from sys.argv so that IPython can have a
+    # go at them later
+    sys.argv = [sys.argv[0]] + rest
+
+    if args.script is not None:
+        args.banner = False
+
+    return args
+
+
+def make_banner(args):
+    # http://patorjk.com/software/taag/#p=display&f=Standard&t=RVC%203
+    # print the banner: standard
+    # https://patorjk.com/software/taag/#p=display&f=Standard&t=Robotics%2C%20Vision%20%26%20Control%203
+
+    banner = fg("yellow")
+    banner += r""" ____       _           _   _             __     ___     _                ___      ____            _             _   _____ 
 |  _ \ ___ | |__   ___ | |_(_) ___ ___    \ \   / (_)___(_) ___  _ __    ( _ )    / ___|___  _ __ | |_ _ __ ___ | | |___ / 
 | |_) / _ \| '_ \ / _ \| __| |/ __/ __|    \ \ / /| / __| |/ _ \| '_ \   / _ \/\ | |   / _ \| '_ \| __| '__/ _ \| |   |_ \ 
 |  _ < (_) | |_) | (_) | |_| | (__\__ \_    \ V / | \__ \ | (_) | | | | | (_>  < | |__| (_) | | | | |_| | | (_) | |  ___) |
 |_| \_\___/|_.__/ \___/ \__|_|\___|___( )    \_/  |_|___/_|\___/|_| |_|  \___/\/  \____\___/|_| |_|\__|_|  \___/|_| |____/ 
-                                      |/                                                                                   
+                                          |/                                                                                   
 for Python"""
 
-if args.book:
-    # set book options
-    args.resultprefix = ""
-    args.prompt = ">>> "
-    args.showassign = True
-    args.ansi = False
-    args.examples = True
-
-from math import pi  # lgtm [py/unused-import]
-
-import numpy as np
-import scipy as sp
-import matplotlib.pyplot as plt  # lgtm [py/unused-import]
-
-# setup defaults
-np.set_printoptions(
-    linewidth=120,
-    formatter={"float": lambda x: f"{x:8.4g}" if abs(x) > 1e-10 else f"{0:8.4g}"},
-)
-
-if args.robot:
-    from roboticstoolbox import *  # lgtm [py/unused-import]
-
-if args.vision:
-    from machinevisiontoolbox import *
-    import machinevisiontoolbox.base as mvbase
+    versions = []
+    if args.robot:
+        versions.append(f"RTB=={version('roboticstoolbox-python')}")
+    if args.vision:
+        versions.append(f"MVTB=={version('machinevision-toolbox-python')}")
+    try:
+        versions.append(f"SG=={version('spatialmath-python')}")
+    except:
+        pass
+    versions.append(f"SMTB=={version('spatialmath-python')}")
+    versions.append(f"NumPy=={version('numpy')}")
+    versions.append(f"SciPy=={version('scipy')}")
+    versions.append(f"Matplotlib=={version('matplotlib')}")
+
+    # create banner
+    banner += " (" + ", ".join(versions) + ")"
+    banner += r"""
+
+    import math
+    import numpy as np
+    from scipy import linalg, optimize
+    import matplotlib.pyplot as plt
+    from spatialmath import *
+    from spatialmath.base import *
+    from spatialmath.base import sym
+    from spatialgeometry import *
+    """
+    if args.robot:
+        banner += "from roboticstoolbox import *\n"
+    if args.vision:
+        banner += """    from machinevisiontoolbox import *
+    import machinevisiontoolbox.base as mvb
+    """
+
+    banner += r"""
+    # useful variables
+    from math import pi
+    puma = models.DH.Puma560()
+    panda = models.DH.Panda()
+
+    func/object?       - show brief help
+    help(func/object)  - show detailed help
+    func/object??      - show source code
+    """
+    banner += attr(0)
+
+    return banner
+
+
+def startup():
+    plt.ion()
+
+
+def main():
+    args = parse_arguments()
+    # print(args)
+
+    if args.book:
+        # set book options
+        args.resultprefix = ""
+        args.prompt = ">>> "
+        args.showassign = True
+        args.ansi = False
+        args.examples = True
+
+    # setup defaults
+    np.set_printoptions(
+        linewidth=120,
+        formatter={"float": lambda x: f"{x:8.4g}" if abs(x) > 1e-10 else f"{0:8.4g}"},
+    )
 
-from spatialmath import *  # lgtm [py/polluting-import]
-from spatialgeometry import *  # lgtm [py/polluting-import]
-from spatialmath.base import *
+    globs = globals()
+    if args.robot:
+        exec("from roboticstoolbox import *", globs)
+        from roboticstoolbox import __path__
+
+        sys.path.append(str(Path(__path__[0]) / "examples"))
+
+        # load some robot models
+        globs["puma"] = models.DH.Puma560()
+        globs["panda"] = models.DH.Panda()
+
+        # set default backend for Robot.plot
+        if args.swift:
+            Robot.default_backend = "swift"
+
+    if args.vision:
+        exec("from machinevisiontoolbox import *", globs)
+        exec("import machinevisiontoolbox.base as mvbase", globs)
+
+    # set matrix printing mode for spatialmath
+    SE3._ansimatrix = args.ansi
+
+    # set default matplotlib backend
+    if args.backend is not None:
+        print(f"Using matplotlib backend {args.backend}")
+        mpl.use(args.backend)
+
+    if args.banner:
+        banner = make_banner(args)
+        print(banner)
+
+    if args.showassign and args.banner:
+        print(
+            fg("red")
+            + "Results of assignments will be displayed, use trailing ; to suppress"
+            + attr(0)
+            + "\n"
+        )
+
+    # append to the module path
+    # - RVC3 models and examples
+    # - RTB examples
+    root = Path(__file__).absolute().parent.parent
+    sys.path.append(str(root / "models"))
+    sys.path.append(str(root / "examples"))
+
+    if args.cwd:
+        os.chdir(root)
+
+    class MyPrompt(Prompts):
+        def in_prompt_tokens(self, cli=None):
+            if args.prompt is None:
+                return super().in_prompt_tokens()
+            else:
+                return [(Token.Prompt, args.prompt)]
+
+        def out_prompt_tokens(self, cli=None):
+            if args.resultprefix is None:
+                # traditional behaviour
+                return super().out_prompt_tokens()
+            else:
+                return [
+                    (Token.Prompt, args.resultprefix.format(self.shell.execution_count))
+                ]
+
+    # set configuration options, there are lots, see
+    # https://ipython.readthedocs.io/en/stable/config/options/terminal.html
+    c = Config()
+    c.InteractiveShellEmbed.colors = args.color
+    c.InteractiveShell.confirm_exit = args.confirmexit
+    # c.InteractiveShell.prompts_class = ClassicPrompts
+    c.InteractiveShell.prompts_class = MyPrompt
+    if args.showassign:
+        c.InteractiveShell.ast_node_interactivity = "last_expr_or_assign"
+    c.TerminalIPythonApp.display_banner = args.banner
+
+    # set precision, same as %precision
+    c.PlainTextFormatter.float_precision = "%.3f"
+
+    # set up a script to be executed by IPython when we get there
+    code = None
+    if args.script is not None:
+        path = Path(args.script)
+        if not path.exists():
+            raise ValueError(f"script does not exist: {args.script}")
+        code = path.open("r").readlines()
+
+    if code is None:
+        code = [
+            "startup()",
+            "%precision %.3g;",
+        ]
 
-# set matrix printing mode for spatialmath
-SE3._ansimatrix = args.ansi
+    c.InteractiveShellApp.exec_lines = code
+    IPython.start_ipython(config=c, user_ns=globals())
 
-# set default matplotlib backend
-if args.backend is not None:
-    print(f"Using matplotlib backend {args.backend}")
-    mpl.use(args.backend)
-
-# load some robot models
-puma = models.DH.Puma560()
-panda = models.DH.Panda()
-
-# print the banner: standard
-# https://patorjk.com/software/taag/#p=display&f=Standard&t=Robotics%2C%20Vision%20%26%20Control%203
-
-# set default backend for Robot.plot
-if args.swift:
-    Robot.default_backend = "swift"
-
-versions = []
-if args.robot:
-    versions.append(f"RTB=={version('roboticstoolbox-python')}")
-if args.vision:
-    versions.append(f"MVTB=={version('machinevision-toolbox-python')}")
-versions.append(f"SMTB=={version('spatialmath-python')}")
-versions.append(f"NumPy=={version('numpy')}")
-versions.append(f"SciPy=={version('scipy')}")
-
-# create banner
-banner += " (" + ", ".join(versions) + ")"
-banner += r"""
 
-import numpy as np
-import scipy as sp
-import matplotlib.pyplot as plt
-from math import pi
-from spatialmath import *
-from spatialmath.base import *
-"""
-if args.robot:
-    banner += "from roboticstoolbox import *\n"
-if args.vision:
-    banner += """from machinevisiontoolbox import *
-import machinevisiontoolbox.base as mvbase
-"""
-
-banner += r"""
-func/object?       - show brief help
-help(func/object)  - show detailed help
-func/object??      - show source code
-
-"""
-banner += attr(0)
-
-if args.banner:
-    print(banner)
-
-# append to the module path
-# - RVC3 models and examples
-# - RTB examples
-root = Path(__file__).absolute().parent.parent
-sys.path.append(str(root / "models"))
-sys.path.append(str(root / "examples"))
-
-if args.robot:
-    import roboticstoolbox as rtb
-    sys.path.append(str(Path(rtb.__path__[0]) / "examples"))
-
-if args.cwd:
-    os.chdir(root)
-
-if args.showassign and args.banner:
-    print(
-        fg("red")
-        + """Results of assignments will be displayed, use trailing ; to suppress
-
-""",
-        attr(0),
-    )
-
-class MyPrompt(Prompts):
-    def in_prompt_tokens(self, cli=None):
-        if args.prompt is None:
-            return super().in_prompt_tokens()
-        else:
-            return [(Token.Prompt, args.prompt)]
-
-    def out_prompt_tokens(self, cli=None):
-        if args.resultprefix is None:
-            # traditional behaviour
-            return super().out_prompt_tokens()
-        else:
-            return [
-                (Token.Prompt, args.resultprefix.format(self.shell.execution_count))
-            ]
-
-# set configuration options, there are lots, see
-# https://ipython.readthedocs.io/en/stable/config/options/terminal.html
-c = Config()
-c.InteractiveShellEmbed.colors = args.color
-c.InteractiveShell.confirm_exit = args.confirmexit
-# c.InteractiveShell.prompts_class = ClassicPrompts
-c.InteractiveShell.prompts_class = MyPrompt
-if args.showassign:
-    c.InteractiveShell.ast_node_interactivity = "last_expr_or_assign"
-c.TerminalIPythonApp.display_banner = args.banner
-
-# set precision, same as %precision
-c.PlainTextFormatter.float_precision = "%.3f"
-
-# set up a script to be executed by IPython when we get there
-code = None
-if args.script is not None:
-    path = Path(args.script)
-    print(path)
-    if not path.exists():
-        raise ValueError(f"script does not exist: {args.script}")
-    code = path.open("r").readlines()
-if code is None:
-    code = [
-        "%precision %.3g;",
-        "plt.ion();",
-    ]
-
-else:
-    code.append("plt.ion()")
-c.InteractiveShellApp.exec_lines = code
-IPython.start_ipython(config=c, user_ns=globals())
+if __name__ == "__main__":
+    main()
```

### Comparing `rvc3python-0.2.3/RVC3/examples/hershey/genhershey.py` & `rvc3python-0.9.0/RVC3/examples/hershey/genhershey.py`

 * *Files identical despite different names*

### Comparing `rvc3python-0.2.3/RVC3/examples/hershey/hershey.json` & `rvc3python-0.9.0/RVC3/examples/hershey/hershey.json`

 * *Files identical despite different names*

### Comparing `rvc3python-0.2.3/RVC3/examples/hershey/hershey.txt` & `rvc3python-0.9.0/RVC3/examples/hershey/hershey.txt`

 * *Files identical despite different names*

### Comparing `rvc3python-0.2.3/RVC3/examples/imu_data.py` & `rvc3python-0.9.0/RVC3/examples/imu_data.py`

 * *Files identical despite different names*

### Comparing `rvc3python-0.2.3/RVC3/examples/mosaic.py` & `rvc3python-0.9.0/RVC3/examples/mosaic.py`

 * *Files identical despite different names*

### Comparing `rvc3python-0.2.3/RVC3/examples/ransac_line.py` & `rvc3python-0.9.0/RVC3/examples/ransac_line.py`

 * *Files identical despite different names*

### Comparing `rvc3python-0.2.3/RVC3/examples/visodom.py` & `rvc3python-0.9.0/RVC3/examples/visodom.py`

 * *Files identical despite different names*

### Comparing `rvc3python-0.2.3/RVC3/examples/walking.py` & `rvc3python-0.9.0/RVC3/examples/walking.py`

 * *Files identical despite different names*

### Comparing `rvc3python-0.2.3/RVC3/examples/writing.py` & `rvc3python-0.9.0/RVC3/examples/writing.py`

 * *Files identical despite different names*

### Comparing `rvc3python-0.2.3/RVC3/models/IBVS-holonomic-main.py` & `rvc3python-0.9.0/RVC3/models/IBVS-partitioned-main.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,48 +1,49 @@
+#! /usr/bin/env python
+
 from pathlib import Path
 from machinevisiontoolbox import *
-from roboticstoolbox import *
-
 from bdsim import Clock, bdload, BDSim
-from spatialmath import SE3
+from spatialmath import SE3, Polygon2
+from spatialmath.base import angdiff
+from math import atan2, sqrt
 import matplotlib.pyplot as plt
-from math import pi
 
 
-sim = BDSim(animation=True) #debug='i')
+sim = BDSim(animation=True)  # debug='i')
 bd = sim.blockdiagram()
-sim.set_options(animation=True)
-clock = bd.clock(0.1, unit='s')
-
-# wide angle camera
-camera = CentralCamera.Default(f=0.002)
 
-# camera optical axis is upward
-T_B_C = SE3(0.2, 0.1, 0.3) 
+clock = bd.clock(0.1, unit="s")
+camera = CentralCamera.Default()
 
-# landmark points on the ceiling
-P = np.array([[0, 1, 3], [0, -1, 3]]).T;
+pose_0 = SE3(1, 1, -3) * SE3.Rz(0.6)
 
-# desired landmark position on the image plane
-pd = camera.project_point(P, pose=SE3(-2, 0, 0)*T_B_C)
+model = Path(__file__).parent / "IBVS-partitioned.bd"
+print(model)
 
-q0 = [-6, 2, 0.6]
-lmbda = 1
 
 def plot_init(camera):
-	camera.plot_point(pd, 'b*')
+    print("@@@@@plot_init")
+    camera.plot_point(bd["p*"].value, "b*")
 
-def world_init(ax):
-	# plot X, Y coords of world points
-	ax.plot(P[0, :], P[1, :], 'b*')
 
-# load the bdsim model
-model = Path(__file__).parent / "IBVS-holonomic.bd"
-bd = bdload(bd, model, globalvars=globals())
+def rho_theta(p):
+    A_d = 200
+    theta_d = 0
+
+    # square is 400x400
+
+    rho = 1 - sqrt(Polygon2(p).area()) / A_d
 
+    # this is the edge parallel to the x-axis
+    theta = atan2(p[1, 2] - p[1, 1], p[0, 2] - p[0, 1])
+    theta = angdiff(theta_d - theta)
+
+    return np.r_[rho, theta]
+
+
+bd = bdload(bd, model, globalvars=globals())
 bd.compile()
-bd.report()
 
+sim.report(bd)
+out = sim.run(bd, 150)
 print(out)
-
-# sim.done(bd)
-# plt.pause(5)
```

### Comparing `rvc3python-0.2.3/RVC3/models/IBVS-nonholonomic-main.py` & `rvc3python-0.9.0/RVC3/models/IBVS-nonholonomic-main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,75 +1,85 @@
+#! /usr/bin/env python
+
+"""
+Creates Fig 16.8
+Robotics, Vision & Control for Python, P. Corke, Springer 2023.
+Copyright (c) 2021- Peter Corke
+"""
+
 from pathlib import Path
 from machinevisiontoolbox import *
 from roboticstoolbox import *
 
-from bdsim import Clock, bdload, BDSim
+from bdsim import bdload, BDSim
 from spatialmath import SE3
 import matplotlib.pyplot as plt
 from math import pi, sqrt, atan2
 
 
-sim = BDSim(animation=True) #debug='i')
+sim = BDSim(animation=True)  # debug='i')
 bd = sim.blockdiagram()
 
-clock = bd.clock(0.1, unit='s')
-
 # wide angle camera
 camera = CentralCamera.Default(f=0.002)
-T_vc = SE3(0.2, 0.1, 0.3) * SE3.Ry(pi/2) * SE3.Rz(-pi/2) #*trotx(-pi/4);   
+T_vc = SE3(0.2, 0.1, 0.3) * SE3.Ry(pi / 2) * SE3.Rz(-pi / 2)  # *trotx(-pi/4);
 P = np.array([[4.0, 10, 3], [9, 9, 2], [6, 8, 3], [8, 10, 4], [10, 7, 2]]).T
-T_B_C = SE3(0.2, 0.1, 0.5) * SE3.Ry(pi/2) * SE3.Rz(-pi/2)
-x0 = [2, 2, 0];
+T_B_C = SE3(0.2, 0.1, 0.5) * SE3.Ry(pi / 2) * SE3.Rz(-pi / 2)
+x0 = [2, 2, 0]
 # xg = [5 5 pi/2];
 
+
+def plot_init(camera):
+    pd = camera.project_point(P, pose=SE3(-2, 0, 0) * T_B_C)
+    camera.plot_point(pd, "b*")
+
+
 # convert x,y,theta state to polar form
 def polar(x, dict):
-    rho = sqrt(x[0]**2 + x[1]**2)
+    rho = sqrt(x[0] ** 2 + x[1] ** 2)
 
-    if not 'direction' in dict:
+    if not "direction" in dict:
         # direction not yet set, set it
         beta = -atan2(-x[1], -x[0])
         alpha = -x[2] - beta
-        print('alpha', alpha)
+        print("alpha", alpha)
         if -pi / 2 <= alpha <= pi / 2:
-            dict['direction'] = 1
+            dict["direction"] = 1
         else:
-            dict['direction'] = -1
-        print('set direction to ', dict['direction'])
+            dict["direction"] = -1
+        print("set direction to ", dict["direction"])
 
-    if dict['direction'] == -1:
-        beta = -atan2(x[1], x[0]);
+    if dict["direction"] == -1:
+        beta = -atan2(x[1], x[0])
     else:
         beta = -atan2(-x[1], -x[0])
     alpha = -x[2] - beta
 
     # clip alpha
-    if alpha > pi/2:
-        alpha = pi/2
-    elif alpha < -pi/2:
-        alpha = -pi/2  
+    if alpha > pi / 2:
+        alpha = pi / 2
+    elif alpha < -pi / 2:
+        alpha = -pi / 2
+
+    return [
+        dict["direction"],
+        rho,
+        alpha,
+        beta,
+    ]
 
-    return [dict['direction'], rho, alpha, beta, ]
 
 model = Path(__file__).parent / "IBVS-nonholonomic.bd"
 print(model)
 
 
 def world_init(ax):
-	# plot X, Y coords of world points
-	ax.plot(P[0, :], P[1, :], 'b*')
+    # plot X, Y coords of world points
+    ax.plot(P[0, :], P[1, :], "b*")
 
 
 bd = bdload(bd, model, globalvars=globals())
-bd.report()
 bd.compile()
-bd.report()
 
-print('about to run')
-print(sim.options)
-sim.set_options(animation=False)
-out = sim.run(bd, 30)
-print('done')
+sim.report(bd)
+out = sim.run(bd, 10)
 print(out)
-
-# sim.done(bd)
-# plt.pause(5)
```

### Comparing `rvc3python-0.2.3/RVC3/models/RRMC2.py` & `rvc3python-0.9.0/RVC3/models/RRMC2.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,25 @@
-# fig 8.7
+#! /usr/bin/env python
+
+"""
+Creates Fig 8.5
+Robotics, Vision & Control for Python, P. Corke, Springer 2023.
+Copyright (c) 2021- Peter Corke
+"""
 
 import bdsim
 from math import pi, sin, cos
 import numpy as np
 from roboticstoolbox.models.DH import Puma560
 from spatialmath import SE3
 
-sim = bdsim.BDSim(verbose=True)
+sim = bdsim.BDSim()
 bd = sim.blockdiagram()
 
-clock = bd.clock(100, 'Hz')
+clock = bd.clock(100, "Hz")
 puma = Puma560()
 
 # define the blocks
 
 # q0 = [0, pi/4, pi, 0, pi/4, 0]
 
 Te = SE3([0.6, -0.2, 0.7]) * SE3.Ry(np.pi)
@@ -30,22 +36,22 @@
 #     y = r * np.sin(t / T * 2 * pi) + cc[1]
 #     return SE3(x, y, cc[2]) * SE3.Ry(pi)
 # goal = bd.FUNCTION(circle)
 
 # time = bd.TIME()
 # bd.connect(time, goal)
 
-goal = bd.CIRCLEPATH(radius=r, centre=cc, frequency=1/T, unit="rps", pose=SE3.Ry(pi))
+goal = bd.CIRCLEPATH(radius=r, centre=cc, frequency=1 / T, unit="rps", pose=SE3.Ry(pi))
 delta = bd.TR2DELTA()
-jacobian = bd.JACOBIAN(robot=puma, frame='e', inverse=True, name='Jacobian')
+jacobian = bd.JACOBIAN(robot=puma, frame="e", inverse=True, name="Jacobian")
 gain = bd.GAIN(Kp)
-qdot = bd.PROD('**', matrix=True)
-integrator = bd.DINTEGRATOR(clock, x0=q0, name='q')
+qdot = bd.PROD("**", matrix=True)
+integrator = bd.DINTEGRATOR(clock, x0=q0, name="q")
 fkine = bd.FKINE(puma)
-robot = bd.ARMPLOT(robot=puma, q0=q0, name='plot')
+robot = bd.ARMPLOT(robot=puma, q0=q0, name="plot")
 tr2t = bd.TR2T()
 scope = bd.SCOPEXY(scale=[0.5, 0.7, -0.3, -0.10])
 scope_norm = bd.SCOPE()
 norm = bd.NORM()
 
 # connect the blocks
 bd.connect(goal, delta[1])
@@ -59,11 +65,10 @@
 bd.connect(tr2t[1], scope[1])
 bd.connect(jacobian, qdot[0])
 
 bd.connect(delta, norm)
 bd.connect(norm, scope_norm)
 
 bd.compile()
-bd.report()
 
+sim.report(bd)
 out = sim.run(bd, 5, minstepsize=1e-6)  # simulate for 5s
-
```

### Comparing `rvc3python-0.2.3/RVC3/models/SEA.py` & `rvc3python-0.9.0/RVC3/models/SEA.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,60 @@
-# fig 9.24
+#! /usr/bin/env python
+
+"""
+Creates Fig 9.28
+Robotics, Vision & Control for Python, P. Corke, Springer 2023.
+Copyright (c) 2021- Peter Corke
+"""
 
 import numpy as np
 import bdsim
 
+
 def SEA(obstacle_pos=0.8, block=False, graphics=False):
-    sim = bdsim.BDSim(name='SEA', graphics=graphics)
+    sim = bdsim.BDSim(name="SEA", graphics=graphics)
 
     bd = sim.blockdiagram()
 
     m1 = 0.5
     m2 = 1
     LQR = np.c_[169.9563, 62.9010, -19.9563, 71.1092].T
     print(LQR)
     Ks = 5
     force_lim = 2
 
     # define the blocks
     step = bd.STEP(1)
     inputgain = bd.GAIN(np.r_[1, 0, 1, 0])
-    sum1 = bd.SUM('+-')
+    sum1 = bd.SUM("+-")
     lqr = bd.GAIN(LQR)
-    limit = bd.CLIP(min=-force_lim, max=force_lim, name='torquelimit')
+    limit = bd.CLIP(min=-force_lim, max=force_lim, name="torquelimit")
 
-    motor_sum = bd.SUM('+-')
+    motor_sum = bd.SUM("+-")
     motor_accel = bd.GAIN(1 / m1)
     motor_vel = bd.INTEGRATOR(x0=0)
     motor_pos = bd.INTEGRATOR(x0=0)
 
-    spring_sum = bd.SUM('+-')
+    spring_sum = bd.SUM("+-")
     spring_force = bd.GAIN(Ks)
 
     load_accel = bd.GAIN(1 / m2)
     load_vel = bd.INTEGRATOR(x0=0)
     load_pos = bd.INTEGRATOR(x0=0)
     obstacle = bd.FUNCTION(lambda x: 0 if x >= obstacle_pos else 1)
-    load_prod = bd.PROD('**')
+    load_prod = bd.PROD("**")
 
-    spring_scope = bd.SCOPE(name='spring scope')
-    state_scope = bd.SCOPE(vector=4, labels=['$x_m$', r'$\dot{x}_m$', '$x_l$', r'$\dot{x}_l$'], name='state scope')
+    spring_scope = bd.SCOPE(name="spring scope")
+    state_scope = bd.SCOPE(
+        vector=4,
+        labels=["$x_m$", r"$\dot{x}_m$", "$x_l$", r"$\dot{x}_l$"],
+        name="state scope",
+    )
 
-    fig_scope = bd.SCOPE(nin=3, labels=['$x_l$', '$u$', '$F_s$'], name='figure scope')
+    fig_scope = bd.SCOPE(nin=3, labels=["$x_l$", "$u$", "$F_s$"], name="figure scope")
     mux = bd.MUX(4)
 
     # connect the blocks
 
     # controller
     bd.connect(step, inputgain)
     bd.connect(inputgain, sum1[0])
@@ -67,21 +78,20 @@
 
     # spring block
     bd.connect(spring_sum, spring_force)
     bd.connect(spring_force, motor_sum[1], load_accel, spring_scope, fig_scope[2])
 
     bd.connect(mux, state_scope)
 
-    bd.compile()   # check the diagram
-    bd.report()    # list all blocks and wires
+    bd.compile()  # check the diagram
 
+    sim.report(bd)
     out = sim.run(bd, 5, dt=5e-3, watch=[limit, spring_force])
     # out = vloop.run(2, checkstep=1e-6)  # simulate for 5s
     # # vloop.dotfile('bd1.dot')  # output a graphviz dot file
     # # vloop.savefig('pdf')      # save all figures as pdf
-    sim.done(bd, block=block)
 
     return out
 
-if __name__ == "__main__":
 
-    SEA(block=True, graphics=True)
+if __name__ == "__main__":
+    SEA(block=True, graphics=True)
```

### Comparing `rvc3python-0.2.3/RVC3/models/braitenberg.py` & `rvc3python-0.9.0/RVC3/models/braitenberg.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,65 +1,76 @@
 #!/usr/bin/env python3
 
+"""
+Creates Fig 5.4
+Robotics, Vision & Control for Python, P. Corke, Springer 2023.
+Copyright (c) 2021- Peter Corke
+"""
+
 import bdsim
 import math
 import numpy as np
 from spatialmath import SE2
 
 
 sim = bdsim.BDSim(animation=True, graphics=True)
 bd = sim.blockdiagram()
 
+
 def sensorfield(x, y):
     xc = 60
-    yc = 90;
+    yc = 90
     return 200 / ((x - xc) ** 2 + (y - yc) ** 2 + 200)
 
+
 def background_graphics(ax):
     v = np.arange(0, 100)
     X, Y = np.meshgrid(v, v)
     Z = sensorfield(X, Y)
-    a = ax.imshow(Z, cmap='viridis')
+    a = ax.imshow(Z, cmap="viridis")
     ax.figure.colorbar(a)
-    
-speed = bd.CONSTANT(2, name='speed')
-sum1 = bd.SUM('+--')
-sum2 = bd.SUM('+-')
-
-Kv = bd.GAIN(50, name='Kv')
-Ks = bd.GAIN(5, name='Ks')
-bike = bd.BICYCLE(x0=[5, 5, 0], speed_max=1, name='vehicle')
+
+
+speed = bd.CONSTANT(2, name="speed")
+sum1 = bd.SUM("+--")
+sum2 = bd.SUM("+-")
+
+Kv = bd.GAIN(50, name="Kv")
+Ks = bd.GAIN(5, name="Ks")
+bike = bd.BICYCLE(x0=[5, 5, 0], speed_max=1, name="vehicle")
+
 
 def sensorfunc(x, offset):
     xy = SE2(x) * offset
     return sensorfield(xy[0], xy[1])[0]
 
+
 # offset = np.r_[0, 2]
-leftsensor = bd.FUNCTION(sensorfunc, nin=1, fargs=([0, -2],), name='leftsensor')
-rightsensor = bd.FUNCTION(sensorfunc, nin=1, fargs=([0, 2],), name='rightsensor')
+leftsensor = bd.FUNCTION(sensorfunc, nin=1, fargs=([0, -2],), name="leftsensor")
+rightsensor = bd.FUNCTION(sensorfunc, nin=1, fargs=([0, 2],), name="rightsensor")
 
-vplot = bd.VEHICLEPLOT(scale=[0, 100], size=5, shape='box', trail=True,
-    name='sensor field', init=background_graphics)
-vscope = bd.SCOPE(name='velocity')
-wscope = bd.SCOPE(name='steering rate')
+vplot = bd.VEHICLEPLOT(
+    scale=[0, 100],
+    size=5,
+    shape="box",
+    trail=True,
+    name="sensor field",
+    init=background_graphics,
+)
+vscope = bd.SCOPE(name="velocity")
+wscope = bd.SCOPE(name="steering rate")
 
 bd.connect(bike, leftsensor, rightsensor, vplot)
 bd.connect(rightsensor, sum1[1], sum2[0])
 bd.connect(speed, sum1[0])
 bd.connect(leftsensor, sum1[2], sum2[1])
 bd.connect(sum1, Kv)
 bd.connect(Kv, vscope, bike.v)
 
 bd.connect(sum2, wscope, Ks)
 bd.connect(Ks, bike.gamma)
 
 bd.compile()
 
 if __name__ == "__main__":
-    bd.report()
-
+    sim.report(bd)
     out = sim.run(bd, T=125, dt=0.2)
-
-    sim.done(bd, block=False)
-
-    sim = bdsim.BDSim(animation=False)
-    bd = sim.blockdiagram()
```

### Comparing `rvc3python-0.2.3/RVC3/models/driveconfig.py` & `rvc3python-0.9.0/RVC3/models/driveconfig.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,101 +1,126 @@
 #!/usr/bin/env python3
 
+"""
+Creates Fig 4.14
+Robotics, Vision & Control for Python, P. Corke, Springer 2023.
+Copyright (c) 2021- Peter Corke
+"""
+
 # run with command line -a switch to show animation
 
-import bdsim
 from math import pi, sqrt, atan, atan2
+import bdsim
 
-sim = bdsim.BDSim()
+sim = bdsim.BDSim(animation=True)
 bd = sim.blockdiagram()
 
 # parameters
-xg = [5, 5, pi/2]
-Krho = bd.GAIN(1, name='Krho')
-Kalpha = bd.GAIN(5, name='Kalpha')
-Kbeta = bd.GAIN(-2, name='Kbeta')
+xg = [5, 5, pi / 2]
+Krho = bd.GAIN(1, name="Krho")
+Kalpha = bd.GAIN(5, name="Kalpha")
+Kbeta = bd.GAIN(-2, name="Kbeta")
 
-xg = [5, 5, pi/2]
+xg = [5, 5, pi / 2]
 x0 = [5, 2, 0]
 x0 = [5, 9, 0]
 
-x0 = [8, 5, pi/2]
 
 # annotate the graphics
 def background_graphics(ax):
-    ax.plot(*xg[:2], '*')
-    ax.plot(*x0[:2], 'o')
+    ax.plot(*xg[:2], "*")
+    ax.plot(*x0[:2], "o")
+
 
 # convert x,y,theta state to polar form
 def polar(x, dict):
-    rho = sqrt(x[0]**2 + x[1]**2)
+    rho = sqrt(x[0] ** 2 + x[1] ** 2)
 
-    if not 'direction' in dict:
+    if not "direction" in dict:
         # direction not yet set, set it
         beta = -atan2(-x[1], -x[0])
         alpha = -x[2] - beta
-        print('alpha', alpha)
+        print("alpha", alpha)
         if -pi / 2 <= alpha <= pi / 2:
-            dict['direction'] = 1
+            dict["direction"] = 1
         else:
-            dict['direction'] = -1
-        print('set direction to ', dict['direction'])
+            dict["direction"] = -1
+        print("set direction to ", dict["direction"])
 
-    if dict['direction'] == -1:
-        beta = -atan2(x[1], x[0]);
+    if dict["direction"] == -1:
+        beta = -atan2(x[1], x[0])
     else:
         beta = -atan2(-x[1], -x[0])
     alpha = -x[2] - beta
 
     # clip alpha
-    if alpha > pi/2:
-        alpha = pi/2
-    elif alpha < -pi/2:
-        alpha = -pi/2  
+    if alpha > pi / 2:
+        alpha = pi / 2
+    elif alpha < -pi / 2:
+        alpha = -pi / 2
+
+    return [
+        dict["direction"],
+        rho,
+        alpha,
+        beta,
+    ]
 
-    return [dict['direction'], rho, alpha, beta, ]
 
 # constants
-goal0 = bd.CONSTANT([xg[0], xg[1], 0], name='goal_pos')
-goalh = bd.CONSTANT(xg[2], name='goal_heading')
+goal0 = bd.CONSTANT([xg[0], xg[1], 0], name="goal_pos")
+goalh = bd.CONSTANT(xg[2], name="goal_heading")
 
 # stateful blocks
-bike = bd.BICYCLE(x0=x0, vlim=2, slim=1.3, name='vehicle')
+bike = bd.BICYCLE(x0=x0, vlim=2, slim=1.3, name="vehicle")
 
 # functions
-fabs = bd.FUNCTION(lambda x: abs(x), name='abs')
-polar = bd.FUNCTION(polar, nout=4, persistent=True, name='polar', inames=('x',),
-    onames=('direction', r'$\rho$', r'$\alpha$', r'$\beta'))
-stop = bd.STOP(lambda x: x < 0.01, name='close enough')
-steer_rate = bd.FUNCTION(lambda u: atan(u), name='atan')
+fabs = bd.FUNCTION(lambda x: abs(x), name="abs")
+polar = bd.FUNCTION(
+    polar,
+    nout=4,
+    persistent=True,
+    name="polar",
+    inames=("x",),
+    onames=("direction", r"$\rho$", r"$\alpha$", r"$\beta"),
+)
+stop = bd.STOP(lambda x: x < 0.01, name="close enough")
+steer_rate = bd.FUNCTION(lambda u: atan(u), name="atan")
 
 # arithmetic
-vprod = bd.PROD('**', name='vprod')
-wprod = bd.PROD('**/', name='aprod')
-xerror = bd.SUM('+-')
-heading_sum = bd.SUM('++')
-gsum = bd.SUM('++')
+vprod = bd.PROD("**", name="vprod")
+wprod = bd.PROD("**/", name="aprod")
+xerror = bd.SUM("+-")
+heading_sum = bd.SUM("++")
+gsum = bd.SUM("++")
 
 # displays
-vplot = bd.VEHICLEPLOT(scale=[0, 10], size=0.7, shape='box', init=background_graphics, movie='rvc4_11.mp4')
-ascope = bd.SCOPE(name=r'$\alpha$')
-bscope = bd.SCOPE(name=r'$\beta$')
+vplot = bd.VEHICLEPLOT(
+    scale=[0, 10],
+    size=0.7,
+    shape="box",
+    path="b:",
+    init=background_graphics,
+)
+# movie="rvc4_11.mp4",)
+ascope = bd.SCOPE(name=r"$\alpha$")
+bscope = bd.SCOPE(name=r"$\beta$")
 
 # connections
 
 bd.connect(bike, vplot)
 bd.connect(bike, xerror[0])
 bd.connect(goal0, xerror[1])
 
 bd.connect(xerror, polar)
-bd.connect(polar[1], Krho, stop) # rho
+bd.connect(polar[1], Krho, stop)  # rho
 bd.connect(Krho, vprod[1])
-bd.connect(polar[2], Kalpha, ascope) # alpha
+bd.connect(polar[2], Kalpha, ascope)  # alpha
 bd.connect(Kalpha, gsum[0])
-bd.connect(polar[3], heading_sum[0]) # beta
+bd.connect(polar[3], heading_sum[0])  # beta
 bd.connect(goalh, heading_sum[1])
 bd.connect(heading_sum, Kbeta, bscope)
 
 bd.connect(polar[0], vprod[0], wprod[1])
 bd.connect(vprod, fabs, bike.v)
 bd.connect(fabs, wprod[2])
 bd.connect(wprod, steer_rate)
@@ -103,11 +128,10 @@
 
 bd.connect(Kbeta, gsum[1])
 bd.connect(gsum, wprod[0])
 
 bd.compile()
 
 if __name__ == "__main__":
-    bd.report_summary()
-    out = sim.run(bd, T=10)
 
-    bd.done(block=True)
+    sim.report(bd)
+    out = sim.run(bd, T=10)
```

### Comparing `rvc3python-0.2.3/RVC3/models/driveline.py` & `rvc3python-0.9.0/RVC3/models/drivepoint.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,66 @@
 #!/usr/bin/env python3
 
+"""
+Creates Fig 4.7
+Robotics, Vision & Control for Python, P. Corke, Springer 2023.
+Copyright (c) 2021- Peter Corke
+"""
+
 # run with command line -a switch to show animation
 
-import bdsim
 import math
-import numpy as np
+import bdsim
 
-sim = bdsim.BDSim()
-bd = sim.blockdiagram()
-from spatialmath import base
+# handle globals that might be passed in from ipython %run -i
+if "pgoal" not in globals():
+    pgoal = [5, 5]
+if "qs" not in globals():
+    qs = [5, 2, 0]
+
+sim = bdsim.BDSim(animation=True)
+sim.set_globals(globals())  # allow setting via command line --global
 
-#x0 = [8, 5, math.pi/2]
-x0 = [5, 2, 0]
-L = [1, -2, 4]
+bd = sim.blockdiagram()
 
 
 def background_graphics(ax):
-    base.plot_homline(L, "r--", ax=ax, xlim=np.r_[0, 10], ylim=np.r_[0, 10])
-    ax.plot(x0[0], x0[1], 'o')
+    ax.plot(5, 5, "*")
+    ax.plot(5, 2, "o")
 
-speed = bd.CONSTANT(0.5)
-slope = bd.CONSTANT(math.atan2(L[0], -L[1]))
-d2line = bd.FUNCTION(lambda u: (u[0] * L[0] + u[1] * L[1] + L[2])/math.sqrt(L[0]**2 + L[1]**2))
-heading_error = bd.SUM('+-', mode='c')
-steer_sum = bd.SUM('++')
-Kd = bd.GAIN(0.5, name='Kd')
-Kh = bd.GAIN(1, name='Kh')
-bike = bd.BICYCLE(x0=x0, name='vehicle')
-vplot = bd.VEHICLEPLOT(scale=[0, 10], size=0.7, shape='box', init=background_graphics)
-hscope = bd.SCOPE(name='heading')
-
-xy = bd.INDEX([0, 1], name='xy')
-theta = bd.INDEX([2], name='theta')
-
-bd.connect(d2line, Kd)
-bd.connect(Kd, steer_sum[1])
-bd.connect(steer_sum, bike.gamma)
-bd.connect(speed, bike.v)
 
-bd.connect(slope, heading_error[0])
+goal = bd.CONSTANT(pgoal, name="goal")
+pos_error = bd.SUM("+-")
+d2goal = bd.FUNCTION(lambda d: math.sqrt(d[0] ** 2 + d[1] ** 2))
+h2goal = bd.FUNCTION(lambda d: math.atan2(d[1], d[0]))
+heading_error = bd.SUM("+-", mode="c")
+Kv = bd.GAIN(0.5)
+Kh = bd.GAIN(1.5)
+bike = bd.BICYCLE(x0=qs, name="vehicle")
+vplot = bd.VEHICLEPLOT(
+    scale=[0, 10], size=0.7, shape="box", path="b:", init=background_graphics
+)  # , movie='rvc4_4.mp4')
+vscope = bd.SCOPE(name="velocity")
+hscope = bd.SCOPE(name="heading")
+
+
+xy = bd.INDEX([0, 1], name="xy")
+theta = bd.INDEX([2], name="theta")
+
+bd.connect(goal, pos_error[0])
+bd.connect(pos_error, d2goal, h2goal)
+bd.connect(d2goal, Kv)
+bd.connect(Kv, bike.v, vscope)
+bd.connect(h2goal, heading_error[0])
 bd.connect(theta, heading_error[1])
-
-bd.connect(heading_error, Kh)
-bd.connect(Kh, steer_sum[0])
-
-bd.connect(xy, d2line)
-
+bd.connect(heading_error, Kh, hscope)
+bd.connect(Kh, bike.gamma)
 bd.connect(bike, xy, theta, vplot)
-bd.connect(theta, hscope)
+bd.connect(xy, pos_error[1])
 
 bd.compile()
 
 if __name__ == "__main__":
-    bd.report()
-    out = sim.run(bd, T=20)
+    sim.report(bd)
+
+    out = sim.run(bd, T=10)
+    pass
```

### Comparing `rvc3python-0.2.3/RVC3/models/drivepursuit.py` & `rvc3python-0.9.0/RVC3/models/drivepursuit.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,88 +1,93 @@
 #!/usr/bin/env python3
 
+"""
+Creates Fig 4.11
+Robotics, Vision & Control for Python, P. Corke, Springer 2023.
+Copyright (c) 2021- Peter Corke
+"""
+
 # run with command line -a switch to show animation
 
-import bdsim
 import numpy as np
 import math
 import roboticstoolbox as rtb
 import bdsim
 
 # parameters for the path
 look_ahead = 5
 speed = 1
 dt = 0.1
 tacc = 1
 x0 = [2, 2, 0]
 
 # create the path
-path = np.array([
-    [10, 10],
-    [10, 60],
-    [80, 80],
-    [50, 10]
-    ])
-      
-robot_traj = rtb.mstraj(path[1:,:], qdmax=speed, q0=path[0,:], dt=0.1, tacc=tacc).q
+path = np.array([[10, 10], [10, 60], [80, 80], [50, 10]])
+
+robot_traj = rtb.mstraj(path[1:, :], qdmax=speed, q0=path[0, :], dt=0.1, tacc=tacc).q
 total_time = robot_traj.shape[0] * dt + look_ahead / speed
 print(robot_traj.shape)
 
-sim = bdsim.BDSim(graphics=False)
+sim = bdsim.BDSim(animation=True)
 bd = sim.blockdiagram()
 
+
 def background_graphics(ax):
-    ax.plot(path[:,0], path[:,1], 'r', linewidth=3, alpha=0.7)
+    ax.plot(path[:, 0], path[:, 1], "r", linewidth=3, alpha=0.7)
+
 
 def pure_pursuit(cp, R=None, traj=None):
     # find closest point on the path to current point
-    d = np.linalg.norm(traj-cp, axis=1) # rely on implicit expansion
+    d = np.linalg.norm(traj - cp, axis=1)  # rely on implicit expansion
     i = np.argmin(d)
-    
+
     # find all points on the path at least R away
-    k, = np.where(d[i+1:] >= R)  # find all points beyond horizon
+    (k,) = np.where(d[i + 1 :] >= R)  # find all points beyond horizon
     if len(k) == 0:
         # no such points, we must be near the end, goal is the end
-        pstar = traj[-1,:]
+        pstar = traj[-1, :]
     else:
         # many such points, take the first one
         k = k[0]  # first point beyond look ahead distance
-        pstar = traj[k+i,:]
+        pstar = traj[k + i, :]
     return pstar.flatten()
 
 
-speed = bd.CONSTANT(speed, name='speed')
-pos_error = bd.SUM('+-', name='err')
-#d2goal = bd.FUNCTION(lambda d: math.sqrt(d[0]**2 + d[1]**2), name='d2goal')
-h2goal = bd.FUNCTION(lambda d: math.atan2(d[1], d[0]), name='h2goal')
-heading_error = bd.SUM('+-', mode='c', name='herr')
-Kh = bd.GAIN(0.5, name='Kh')
+speed = bd.CONSTANT(speed, name="speed")
+pos_error = bd.SUM("+-", name="err")
+# d2goal = bd.FUNCTION(lambda d: math.sqrt(d[0]**2 + d[1]**2), name='d2goal')
+h2goal = bd.FUNCTION(lambda d: math.atan2(d[1], d[0]), name="h2goal")
+heading_error = bd.SUM("+-", mode="c", name="herr")
+Kh = bd.GAIN(0.5, name="Kh")
 bike = bd.BICYCLE(x0=x0)
-vplot = bd.VEHICLEPLOT(scale=[0, 80, 0, 80], size=0.7, shape='box', init=background_graphics) #, movie='rvc4_8.mp4')
-sscope = bd.SCOPE(name='steer angle')
-hscope = bd.SCOPE(name='heading angle')
-stop = bd.STOP(lambda x: np.linalg.norm(x - np.r_[50,10]) < 0.1, name='close_enough')
-pp = bd.FUNCTION(pure_pursuit, fkwargs={'R': look_ahead, 'traj': robot_traj}, name='pure_pursuit')
+vplot = bd.VEHICLEPLOT(
+    scale=[0, 80, 0, 80], size=0.7, shape="box", init=background_graphics
+)  # , movie='rvc4_8.mp4')
+sscope = bd.SCOPE(name="steer angle")
+hscope = bd.SCOPE(name="heading angle")
+stop = bd.STOP(lambda x: np.linalg.norm(x - np.r_[50, 10]) < 0.1, name="close_enough")
+pp = bd.FUNCTION(
+    pure_pursuit, fkwargs={"R": look_ahead, "traj": robot_traj}, name="pure_pursuit"
+)
 
-xy = bd.INDEX([0, 1], name='xy')
-theta = bd.INDEX([2], name='theta')
+xy = bd.INDEX([0, 1], name="xy")
+theta = bd.INDEX([2], name="theta")
 
 bd.connect(pp, pos_error[0])
 bd.connect(pos_error, h2goal)
-#bd.connect(d2goal, stop)
+# bd.connect(d2goal, stop)
 
 bd.connect(h2goal, heading_error[0])
 bd.connect(theta, heading_error[1], hscope)
 bd.connect(heading_error, Kh)
 bd.connect(Kh, bike.gamma, sscope)
 bd.connect(speed, bike.v)
 
 bd.connect(xy, pp, stop, pos_error[1])
 
 bd.connect(bike, xy, theta, vplot)
 
 bd.compile()
 
 if __name__ == "__main__":
-    bd.report()
-    print('\nSimulating for ', total_time, ' seconds')
+    sim.report(bd)
     out = sim.run(bd, T=total_time)
```

### Comparing `rvc3python-0.2.3/RVC3/models/opspace.py` & `rvc3python-0.9.0/RVC3/models/opspace.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,17 @@
-# fig 9.24
+#! /usr/bin/env python
+
+"""
+Creates Fig 9.25 using pure Python code
+Robotics, Vision & Control for Python, P. Corke, Springer 2023.
+Copyright (c) 2021- Peter Corke
+"""
 
-from re import X
 import numpy as np
-import scipy as sp
+from scipy import linalg
 import bdsim
 from roboticstoolbox import models
 import spatialmath.base as smb
 from spatialmath import SE3
 
 # equation numbers are with reference to:
 #  A Unified Approach for Motion and Force Control of Robot Manipulators: The
@@ -21,83 +26,94 @@
 # compliance frame is EE frame, constant in this case
 Sf = T_E.R
 
 # compliance specification
 # edit next 2 lines to change compliant motion axes
 #  1 = freespace controlled motion
 #  0 = constrained compliant motion
-sigma_t = np.diag([1, 1, 0]);  # position specification matrix, Sigma_f in (1)
-sigma_r = np.diag([1, 1, 1]);  # rotation specification matrix, Sigma_tau
+sigma_t = np.diag([1, 1, 0])
+# position specification matrix, Sigma_f in (1)
+sigma_r = np.diag([1, 1, 1])
+# rotation specification matrix, Sigma_tau
 
 # compute the generalized task specification matrices (3) and (4)
-omega_p = sp.linalg.block_diag(Sf.T @ sigma_t @ Sf, Sf.T @ sigma_r @ Sf)
+omega_p = linalg.block_diag(Sf.T @ sigma_t @ Sf, Sf.T @ sigma_r @ Sf)
 one = np.eye(3)
-omega_f = sp.linalg.block_diag(Sf.T @ (one - sigma_t) @ Sf, 
-                               Sf.T @ (one - sigma_r) @ Sf)
+omega_f = linalg.block_diag(Sf.T @ (one - sigma_t) @ Sf, Sf.T @ (one - sigma_r) @ Sf)
 
 # setpoints
 Fstar = np.r_[0, 0, -5, 0, 0, 0]
 Xstar = np.r_[0.8, 0.2, 0.3, 0, np.pi / 2, 0]
 
 # control parameters
 Kvf = 20.0
 Kf = 20.0
 Kp = 100.0
 Kv = 50.0
 
 # choose a representation that is singularity free for tool down configuration
-rep = 'rpy/xyz'
+rep = "rpy/xyz"
 
 ## create block diagram
 sim = bdsim.BDSim(graphics=True)
-bd = sim.blockdiagram(name='opspace')
+bd = sim.blockdiagram(name="opspace")
 
 # blocks
 robot_x = bd.FDYN_X(robot, q0=sol.q, gravcomp=True, velcomp=True, representation=rep)
 
-fstar = bd.CONSTANT(Fstar, name='f*')
-xstar = bd.CONSTANT(Xstar, name='x*')
-xdstar = bd.CONSTANT(np.zeros((6,)), name='xd*')
-
-fprod = bd.PROD(matrix=True, name='fprod')
-pprod = bd.PROD(matrix=True, name='pprod')
-fsum = bd.SUM('+-', name='fsum')
+fstar = bd.CONSTANT(Fstar, name="f*")
+xstar = bd.CONSTANT(Xstar, name="x*")
+xdstar = bd.CONSTANT(np.zeros((6,)), name="xd*")
+
+fprod = bd.PROD("**", matrix=True, name="fprod")
+pprod = bd.PROD("**", matrix=True, name="pprod")
+fsum = bd.SUM("+-", name="fsum")
+
 
 # force/torque sensor
 def ft_sensor_func(x):
     z = x[2]
     surface = 0.5
     stiffness = 100
 
     if z <= surface:
         f = stiffness * (z - surface)
     else:
         f = 0
-    
+
     return np.r_[0, 0, f, 0, 0, 0]
 
-ftsensor = bd.FUNCTION(ft_sensor_func, name='f/t sensor')
+
+ftsensor = bd.FUNCTION(ft_sensor_func, name="f/t sensor")
+
 
 # x error
 def x_error_func(x1, x2):
     e = x1 - x2
     e[3:] = smb.angdiff(e[3:])
     return e
-x_error = bd.FUNCTION(x_error_func, nin=2, name='xerror')
+
+
+x_error = bd.FUNCTION(x_error_func, nin=2, name="xerror")
 
 Mx = bd.INERTIA_X(robot, representation=rep)
 
 # scopes
-pos_scope = bd.SCOPE(vector=3, labels=['x', 'y', 'z'], styles=['r', 'g', 'b--'], name='position')
-force_scope = bd.SCOPE(vector=6, name='force/torque')
-wrench_scope = bd.SCOPE(vector=3, labels=['x', 'y', 'z'], styles=['r', 'g', 'b--'], name='command wrench')
-xe_scope = bd.SCOPE(vector=6, name='x error')
-fsum_scope = bd.SCOPE(vector=6, name='fsum scope')
-fprod_scope = bd.SCOPE(vector=6, name='fprod scope')
-sum1_scope = bd.SCOPE(vector=6, name='_sum1 scope')
+pos_scope = bd.SCOPE(
+    vector=3, labels=["x", "y", "z"], styles=["r", "g", "b--"], name="position"
+)
+force_scope = bd.SCOPE(vector=6, name="force/torque")
+wrench_scope = bd.SCOPE(
+    vector=3, labels=["x", "y", "z"], styles=["r", "g", "b--"], name="command wrench"
+)
+xe_scope = bd.SCOPE(vector=6, name="x error")
+fsum_scope = bd.SCOPE(vector=6, name="fsum scope")
+fprod_scope = bd.SCOPE(vector=6, name="fprod scope")
+sum1_scope = bd.SCOPE(vector=6, name="_sum1 scope")
+x_scope = bd.SCOPE(vector=6, name="x scope")
 
 ##  connect the blocks
 
 # force control
 fsum[0] = omega_f * (fstar + (fstar - ftsensor) * Kf)
 fsum[1] = fprod
 fprod[1] = omega_f * Kvf * robot_x.xd
@@ -108,24 +124,24 @@
 x_error[1] = robot_x.x
 
 # the rest
 robot_x.w = fsum + pprod
 Mx[0] = robot_x.q
 bd.connect(Mx, fprod[0], pprod[0])
 ftsensor[0] = robot_x.x
+x_scope[0] = robot_x.x
 
-pos_scope[0] = robot_x.x >> bd.INDEX([0, 1, 2]) 
+pos_scope[0] = robot_x.x >> bd.INDEX([0, 1, 2])
 force_scope[0] = ftsensor
 wrench_scope[0] = pprod >> bd.INDEX([0, 1, 2])
 xe_scope[0] = x_error
 fsum_scope[0] = fsum
 fprod_scope[0] = fprod
-sum1_scope[0] = bd['_sum.1']
+sum1_scope[0] = bd["_sum.1"]
 
-bd.compile()   # check the diagram
-bd.report()    # list all blocks and wires
-bd.plan_dotfile('opspace.dot')
+bd.compile()  # check the diagram
+sim.report(bd, sortby="type")
 
 if __name__ == "__main__":
-
-    out = sim.run(bd, 2, dt=5e-3, watch=[x_error, pprod, robot_x.x, robot_x.xd, robot_x.xdd])
-    sim.done(bd, block=True)
+    out = sim.run(
+        bd, 2, dt=5e-3, watch=[x_error, pprod, robot_x.x, robot_x.xd, robot_x.xdd]
+    )
```

### Comparing `rvc3python-0.2.3/RVC3/models/ploop.py` & `rvc3python-0.9.0/RVC3/models/ploop.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,41 @@
+#! /usr/bin/env python
+
+"""
+Creates Fig 9.13
+Robotics, Vision & Control for Python, P. Corke, Springer 2023.
+Copyright (c) 2021- Peter Corke
+"""
+
 import site
 import numpy as np
 import bdsim
 
-site.addsitedir('bdsim')
+site.addsitedir("bdsim")
 
 from vloop import vloop
 
 sim = bdsim.BDSim()
 ploop = sim.blockdiagram()
 
 Kp = 4000.0
 Kff = 0.0
 G = 107.815
 
 # define blocks
-inp = ploop.INPORT(3, onames=('theta*', 'w*', 'tau_d'), name='in')
-outp = ploop.OUTPORT(4,  name='out') # inames=('theta', 'theta_err'),
-sum1 = ploop.SUM('+-')
-sum2 = ploop.SUM('++')
-kp = ploop.GAIN(Kp, name='Kp')
-kff = ploop.GAIN(Kff, name='Kff')
+inp = ploop.INPORT(3, onames=("theta*", "w*", "tau_d"), name="in")
+outp = ploop.OUTPORT(4, name="out")  # inames=('theta', 'theta_err'),
+sum1 = ploop.SUM("+-")
+sum2 = ploop.SUM("++")
+kp = ploop.GAIN(Kp, name="Kp")
+kff = ploop.GAIN(Kff, name="Kff")
 gearbox = ploop.GAIN(1 / G)
 theta = ploop.INTEGRATOR(x0=0)
 fftorque = ploop.CONSTANT(0)
-VLOOP = ploop.SUBSYSTEM(vloop, name='VLOOP')
+VLOOP = ploop.SUBSYSTEM(vloop, name="VLOOP")
 
 # s1 = ploop.SCOPE()
 # s2 = ploop.SCOPE()
 # s3 = ploop.SCOPE()
 
 # wire them up
 ploop.connect(inp[0], sum1[0])
@@ -43,17 +51,16 @@
 ploop.connect(gearbox, theta)  # theta
 ploop.connect(theta, outp[0])
 
 ploop.connect(VLOOP[1], outp[2])
 ploop.connect(VLOOP[2], outp[3])
 
 
-
 # if __name__ == "__main__":
-#     # test harness 
+#     # test harness
 #     bd = bdsim.BlockDiagram()
 
 #     # position = bd.LSPB(0) HACK
 #     position = bd.STEP(T=0.5, on=1, name='tghack')
 #     vel = bd.CONSTANT(0)
 #     taud = bd.CONSTANT(20 / G)
 #     # speed = bd.WAVEFORM(wave='triangle', freq=2, amplitude=25)
@@ -65,8 +72,8 @@
 #     bd.connect(taud, PLOOP[2])
 #     bd.connect(PLOOP[0], scope[1])
 
 #     bd.compile()   # check the diagram
 #     bd.report()    # list all blocks and wires
 
 #     out = bd.run(1, dt=1e-3)
-#     bd.done(block=True)
+#     bd.done(block=True)
```

### Comparing `rvc3python-0.2.3/RVC3/models/ploop_test.py` & `rvc3python-0.9.0/RVC3/models/ploop_test.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,51 @@
+#! /usr/bin/env python
+
+"""
+Creates Fig 9.13
+Robotics, Vision & Control for Python, P. Corke, Springer 2023.
+Copyright (c) 2021- Peter Corke
+"""
+
 import site
 import numpy as np
 import bdsim
 
 from roboticstoolbox import quintic_func
 
-site.addsitedir('bdsim')
+site.addsitedir("bdsim")
 
 from ploop import ploop, G
 
-# test harness 
+# test harness
 sim = bdsim.BDSim()
 bd = sim.blockdiagram()
 
 # position = bd.quintic(0) HACK
 
 quinticfunc = quintic_func(0, 1, 1)
-trajectory = bd.FUNCTION(quinticfunc, nout=3, name='quintic')
+trajectory = bd.FUNCTION(quinticfunc, nout=3, name="quintic")
 time = bd.TIME()
 
 taud = bd.CONSTANT(20 / G)
 # speed = bd.WAVEFORM(wave='triangle', freq=2, amplitude=25)
-PLOOP = bd.SUBSYSTEM(ploop, name='PLOOP')
-theta_scope = bd.SCOPE(nin=2, name=r'$\theta$', labels=['actual', 'demand'])
-werr_scope = bd.SCOPE(name=r'$\omega$ error')
-tau_scope = bd.SCOPE(name=r'$\tau$')
-wff_scope = bd.SCOPE(name=r'$\omega_{ff}$')
+PLOOP = bd.SUBSYSTEM(ploop, name="PLOOP")
+theta_scope = bd.SCOPE(nin=2, name=r"$\theta$", labels=["actual", "demand"])
+werr_scope = bd.SCOPE(name=r"$\omega$ error")
+tau_scope = bd.SCOPE(name=r"$\tau$")
+wff_scope = bd.SCOPE(name=r"$\omega_{ff}$")
 
 bd.connect(time, trajectory)
 bd.connect(trajectory[0], PLOOP[0], theta_scope[1])
 bd.connect(trajectory[1], PLOOP[1], wff_scope)
 bd.connect(taud, PLOOP[2])
 bd.connect(PLOOP[0], theta_scope[0])
 
 bd.connect(PLOOP[2], werr_scope)
 bd.connect(PLOOP[3], tau_scope)
 
-bd.compile()   # check the diagram
-bd.report()    # list all blocks and wires
+bd.compile()  # check the diagram
 
 
 if __name__ == "__main__":
-
+    sim.report(bd)
     out = sim.run(bd, 1, dt=1e-3)
-    bd.done(block=True)
-
-    import matplotlib.pyplot as plt
-    plt.show(block=True)
```

### Comparing `rvc3python-0.2.3/RVC3/models/puma_collapse.py` & `rvc3python-0.9.0/RVC3/models/zerotorque.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-# fig 9.18
+#! /usr/bin/env python
+
+"""
+Creates Fig 9.18
+Robotics, Vision & Control for Python, P. Corke, Springer 2023.
+Copyright (c) 2021- Peter Corke
+"""
 
 import bdsim
 from math import pi
 import numpy as np
 from roboticstoolbox.models.DH import Puma560
 
-def PumaCollapse():
-    bd = bdsim.BlockDiagram(name='Puma collapsing', graphics=False)
-
-    puma = Puma560().nofriction()
-
-    # define the blocks
-
-    torque = bd.CONSTANT([0, 0, 0, 0, 0, 0])
-    robot = bd.FOWARDDYNAMICS(robot=puma)
-    plot = bd.ARMPLOT(puma)
+sim = bdsim.BDSim(animation=True)
+bd = sim.blockdiagram()
 
-    # connect the blocks
-    bd.connect(torque, robot)
-    bd.connect(robot[0], plot)
+puma = Puma560().nofriction()
 
-    bd.compile()   # check the diagram
-    bd.report()    # list all blocks and wires
-    out = bd.run(5)  # simulate for 5s
+# define the blocks
+torque = bd.CONSTANT([0, 0, 0, 0, 0, 0])
+robot = bd.FDYN(robot=puma, q0=puma.qz)
+plot = bd.ARMPLOT(puma)
 
-    bd.done()
+# connect the blocks
+bd.connect(torque, robot)
+bd.connect(robot[0], plot)
 
-    return out
+bd.compile()  # check the diagram
 
 if __name__ == "__main__":
+    sim.report(bd)
 
-    PumaCollapse()
+    out = sim.run(bd, 5)  # simulate for 5s
```

### Comparing `rvc3python-0.2.3/RVC3/models/quadrotor-main.py` & `rvc3python-0.9.0/RVC3/models/quadrotor-main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,30 @@
-#!/usr/bin/env python3
+#! /usr/bin/env python
+
+"""
+Creates Fig 4.24
+Robotics, Vision & Control for Python, P. Corke, Springer 2023.
+Copyright (c) 2021- Peter Corke
+"""
 
 from pathlib import Path
 
 from enum import IntEnum
 import numpy as np
 from spatialmath import SE3, SO2
 from bdsim import Clock, bdload, BDSim
 from math import pi, sqrt, atan, atan2
 
+# dict of quadrotor parameters
+from RVC3.models.quad_model import quadrotor
+
 sim = BDSim(animation=True)
 bd = sim.blockdiagram()
 
+
 # state vector indices
 #   would expect the order to R, P, Y but this is compatible with the
 #   MATLAB version
 class E(IntEnum):
     X = 0
     Y = 1
     Z = 2
@@ -25,76 +35,75 @@
     YW = 0
     P = 1
     R = 2
     YWD = 3
     PD = 4
     RD = 5
 
+
 # controller parameters
 Kp_yaw = 100
 Kd_yaw = 0.1
 Kp_z = 40
 Kd_z = 1
 T0 = 40
 Kp_xy = 0.1
 Kd_xy = 2
 
 Kp_rp = 20
 Kd_rp = 0.1
 
+
 # yaw control
 def yaw_controller(yaw_dmd, x):
-    r = x['rot']
+    r = x["rot"]
     return [(Kp_yaw) * (yaw_dmd - r[E.YW] - Kd_yaw * r[E.YWD]), r[E.YW]]
 
+
 # height control
 def height_controller(height_dmd, x):
-    t = x['trans']
-    T =  (-Kp_z) * (height_dmd - t[E.Z] - Kd_z * t[E.ZD]) + T0
+    t = x["trans"]
+    T = (-Kp_z) * (height_dmd - t[E.Z] - Kd_z * t[E.ZD]) + T0
     # print('h', x[2], z, x[8])
     return -T
 
+
 # velocity control
 def velocity_controller(xy_dmd, x):
-    t = x['trans']
+    t = x["trans"]
     xyerr_B = xy_dmd.ravel() - t[[E.X, E.Y]]
     # xyerr_B = SO2(-x['rot'][E.YW]) * xyerr_0  # in {B}
     K = Kp_xy * np.array([[0, 1], [-1, 0]])
     return K @ (xyerr_B.ravel() - Kd_xy * t[[E.XD, E.YD]])
 
+
 # attitude control
 def attitude_controller(rp_dmd, x):
-    r = x['rot']
+    r = x["rot"]
     rp_torque = (Kp_rp) * (rp_dmd - r[[E.R, E.P]] - Kd_rp * r[[E.RD, E.PD]])
     return list(rp_torque)
 
-# dict of quadrotor parameters
-from bdsim.blocks.quad_model import quadrotor as quad_model
 
 # ----------------------------------
 model = Path(__file__).parent / "quadrotor.bd"
 
 bd = bdload(bd, model, globalvars=globals(), verbose=False)
 
 # build it
 bd.compile()
 
 
 if __name__ == "__main__":
-    bd.report_summary()
-
+    sim.report(bd)
     out = sim.run(bd, T=10, dt=0.05)
 
-    bd.done(block=True)
-
-
 # np.set_printoptions(linewidth=300, suppress=True, precision=4)
 # quad.setstate(np.r_[1, 2, -3, 0.1, 0.2, 0.3,  0.1, 0.2, 0.3, 0.1, 0,2, 0.3])
 
 # quad.inputs = [900 * np.r_[1, .9, 1.1, 1]]
 
 # # check outputs
 # x = quad.output(t=0)
 # xd = quad.deriv()
 
 # print('x: ', x)
-# print('xd:', xd)
+# print('xd:', xd)
```

### Comparing `rvc3python-0.2.3/RVC3/models/quadrotor.py` & `rvc3python-0.9.0/RVC3/models/quadrotor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,30 @@
-#!/usr/bin/env python3
+#! /usr/bin/env python
+
+"""
+Creates Fig 4.24
+Robotics, Vision & Control for Python, P. Corke, Springer 2023.
+Copyright (c) 2021- Peter Corke
+"""
 
 from enum import IntEnum
 import numpy as np
 from spatialmath import SO2
 from bdsim.blockdiagram import BlockDiagram
 from math import pi, sqrt, atan, atan2
 import bdsim
 
-sim = bdsim.BDSim(animation=True, debug='g')
+
+# dict of quadrotor parameters
+from RVC3.models.quad_model import quadrotor
+
+sim = bdsim.BDSim(animation=True)
 bd = sim.blockdiagram()
 
+
 # state vector indices
 #   would expect the order to R, P, Y but this is compatible with the
 #   MATLAB version
 class E(IntEnum):
     X = 0
     Y = 1
     Z = 2
@@ -24,87 +35,99 @@
     YW = 0
     P = 1
     R = 2
     YWD = 3
     PD = 4
     RD = 5
 
+
 # controller parameters
 Kp_yaw = 100
 Kd_yaw = 0.1
 Kp_z = 40
 Kd_z = 1
 T0 = 40
 Kp_xy = 0.1
 Kd_xy = 2
 
 Kp_rp = 20
 Kd_rp = 0.1
 
 
 # demand signals
-x_dmd = bd.WAVEFORM('sine', freq=0.25, unit='Hz', phase=0.25)
-y_dmd = bd.WAVEFORM('sine', freq=0.25, unit='Hz')
-xy_dmd = bd.MUX(nin=2, inputs=(x_dmd, y_dmd), name='xy_demand')
+x_dmd = bd.WAVEFORM("sine", freq=0.25, unit="Hz", phase=0.25)
+y_dmd = bd.WAVEFORM("sine", freq=0.25, unit="Hz")
+xy_dmd = bd.MUX(nin=2, inputs=(x_dmd, y_dmd), name="xy_demand")
+
+yaw_dmd = bd.RAMP(slope=0.1, T=3, off=0, name="yaw demand")
+
+z_dmd = bd.INTERPOLATE(
+    (0, 0.5, 5.5, np.inf), (0, 0, -5, -5), time=True, name="height demand"
+)
 
-yaw_dmd = bd.RAMP(slope=0.1, T=3, off=0, name='yaw demand')
-
-z_dmd = bd.INTERPOLATE((0, 0.5, 5.5, np.inf), (0, 0, -5, -5), time=True, name='height demand')
 
 # yaw control
 def yaw_controller(yaw_dmd, x):
-    r = x['rot']
+    r = x["rot"]
     return (Kp_yaw) * (yaw_dmd - r[E.YW] - Kd_yaw * r[E.YWD])
 
-yaw = bd.FUNCTION(yaw_controller, nin=2, nout=1, name='yawcontrol')
+
+yaw = bd.FUNCTION(yaw_controller, nin=2, nout=1, name="yawcontrol")
+
 
 # height control
 def height_controller(height_dmd, x):
-    t = x['trans']
-    T =  (-Kp_z) * (height_dmd - t[E.Z] - Kd_z * t[E.ZD]) + T0
+    t = x["trans"]
+    T = (-Kp_z) * (height_dmd - t[E.Z] - Kd_z * t[E.ZD]) + T0
     # print('h', x[2], z, x[8])
     return -T
 
-height = bd.FUNCTION(height_controller, nin=2, nout=1, name='zcontrol')
+
+height = bd.FUNCTION(height_controller, nin=2, nout=1, name="zcontrol")
+
 
 # velocity control
 def velocity_controller(xy_dmd, x):
-    t = x['trans']
+    t = x["trans"]
     xyerr_0 = xy_dmd - t[[E.X, E.Y]]
-    xyerr_B = SO2(-x['rot'][E.YW]) * xyerr_0  # in {B}
+    xyerr_B = SO2(-x["rot"][E.YW]) * xyerr_0  # in {B}
     K = Kp_xy * np.array([[0, 1], [-1, 0]])
     return K @ (xyerr_B.ravel() - Kd_xy * t[[E.XD, E.YD]])
 
-velocity = bd.FUNCTION(velocity_controller, nin=2, nout=1, name='velcontrol')
+
+velocity = bd.FUNCTION(velocity_controller, nin=2, nout=1, name="velcontrol")
+
 
 # attitude control
 def attitude_controller(rp_dmd, x):
-    r = x['rot']
+    r = x["rot"]
     rp_torque = (Kp_rp) * (rp_dmd - r[[E.R, E.P]] - Kd_rp * r[[E.RD, E.PD]])
     return list(rp_torque)
 
-attitude = bd.FUNCTION(attitude_controller, nin=2, nout=2, name='attitudecontrol')
 
-# dict of quadrotor parameters
-from bdsim.blocks.quad_model import quadrotor
+attitude = bd.FUNCTION(attitude_controller, nin=2, nout=2, name="attitudecontrol")
 
 # drone + input mixer
-mixer = bd.MULTIROTORMIXER(quadrotor, name='mixer', wmax=1500)
-quad = bd.MULTIROTOR(quadrotor, name='quadrotor')
+mixer = bd.MULTIROTORMIXER(quadrotor, name="mixer", wmax=1500)
+quad = bd.MULTIROTOR(quadrotor, name="quadrotor")
 
 # plot abs value of rotor speeds
-abs_rotorspeed = bd.FUNCTION(lambda x: np.abs(x), name='absval')
-scope_rotorspeed = bd.SCOPE(vector=4, labels=list("0123"), name='rotor speed (abs.val)', inputs=abs_rotorspeed)
+abs_rotorspeed = bd.FUNCTION(lambda x: np.abs(x), name="absval")
+scope_rotorspeed = bd.SCOPE(
+    vector=4, labels=list("0123"), name="rotor speed (abs.val)", inputs=abs_rotorspeed
+)
 
 # plot position and attitude
-x = bd.ITEM('x', name='state')
+x = bd.ITEM("x", name="state")
 xyz = bd.SLICE1([0, 1, 2], inputs=x)
-scope_xyz = bd.SCOPE(vector=3, labels=list("XYZ"), name='position', inputs=xyz)
+scope_xyz = bd.SCOPE(vector=3, labels=list("XYZ"), name="position", inputs=xyz)
 att = bd.SLICE1([3, 4, 5], inputs=x)
-scope_attitude = bd.SCOPE(vector=3, labels=['yaw', 'pitch', 'roll'], name='attitude', inputs=att)
+scope_attitude = bd.SCOPE(
+    vector=3, labels=["yaw", "pitch", "roll"], name="attitude", inputs=att
+)
 
 # animation of quad
 quadplot = bd.MULTIROTORPLOT(quadrotor)
 
 # wiring
 bd.connect(quad, yaw[1], height[1], velocity[1], attitude[1], x)  # state
 bd.connect(yaw_dmd, yaw[0])
@@ -117,25 +140,23 @@
 bd.connect(mixer, quad, abs_rotorspeed)
 bd.connect(quad, quadplot)
 
 # build it
 bd.compile()
 
 if __name__ == "__main__":
-    bd.report_summary()
+    sim.report(bd)
 
     out = sim.run(bd, T=10, dt=0.05)
 
-    bd.done(block=True)
-
 
 # np.set_printoptions(linewidth=300, suppress=True, precision=4)
 # quad.setstate(np.r_[1, 2, -3, 0.1, 0.2, 0.3,  0.1, 0.2, 0.3, 0.1, 0,2, 0.3])
 
 # quad.inputs = [900 * np.r_[1, .9, 1.1, 1]]
 
 # # check outputs
 # x = quad.output(t=0)
 # xd = quad.deriv()
 
 # print('x: ', x)
-# print('xd:', xd)
+# print('xd:', xd)
```

### Comparing `rvc3python-0.2.3/RVC3/models/vloop_test.py` & `rvc3python-0.9.0/RVC3/models/vloop_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,14 @@
-# vloop
+#! /usr/bin/env python
+
+"""
+Creates Fig 9.8
+Robotics, Vision & Control for Python, P. Corke, Springer 2023.
+Copyright (c) 2021- Peter Corke
+"""
 
 import numpy as np
 import bdsim
 
 import site
 import numpy as np
 import bdsim
@@ -11,50 +17,42 @@
 
 
 # test harness for velocity loop
 sim = bdsim.BDSim(graphics=True, progress=False)
 bd = sim.blockdiagram()
 
 # parameters
-disturbance = bd.CONSTANT(0, name='disturbance')
+disturbance = bd.CONSTANT(0, name="disturbance")
 feedforward = bd.CONSTANT(0)
 # speed = bd.WAVEFORM(wave='triangle', freq=2, amplitude=25)
-speed = bd.INTERPOLATE(x=(0, 0.1, 0.3, 0.4, 0.6, 1), y=(0, 0, 50, 50, 0, 0), 
-    time=True, name='demand')
+speed = bd.INTERPOLATE(
+    x=(0, 0.1, 0.3, 0.4, 0.6, 1), y=(0, 0, 50, 50, 0, 0), time=True, name="demand"
+)
 
 # import the velocity loop
-VLOOP = bd.SUBSYSTEM(vloop, name='VLOOP')
+VLOOP = bd.SUBSYSTEM(vloop, name="VLOOP")
 
 # scopes
-w_scope = bd.SCOPE(nin=2, name=r'$\omega$', labels=['actual', 'demand'])
-werr_scope = bd.SCOPE(name=r'$\omega_{err}$')
-tau_scope = bd.SCOPE(name=r'$\tau$')
-integral_scope = bd.SCOPE(name='integral')
+w_scope = bd.SCOPE(nin=2, name=r"$\omega$", labels=["actual", "demand"])
+werr_scope = bd.SCOPE(name=r"$\omega_{err}$")
+tau_scope = bd.SCOPE(name=r"$\tau$")
+integral_scope = bd.SCOPE(name="integral")
 
-demand_scope = bd.SCOPE(name='demand scope')
+demand_scope = bd.SCOPE(name="demand scope")
 
 bd.connect(speed, demand_scope)
 
 bd.connect(VLOOP[0], w_scope[0])
 bd.connect(VLOOP[1], werr_scope)
 bd.connect(VLOOP[2], tau_scope)
 bd.connect(VLOOP[3], integral_scope)
 
 bd.connect(disturbance, VLOOP[1])
 bd.connect(speed, VLOOP[0], w_scope[1])
 bd.connect(feedforward, VLOOP[2])
 
-
-bd.compile()   # check the diagram
-bd.report()    # list all blocks and wires
-# bd.report_summary()
+bd.compile()  # check the diagram
 
 if __name__ == "__main__":
-    bd.plan_print()
-
-    # bd.showgraph()
+    sim.report(bd)
 
     out = sim.run(bd, 1, dt=1e-3)
-    bd.done(block=True)
-
-    import matplotlib.pyplot as plt
-    plt.show(block=True)
```

### Comparing `rvc3python-0.2.3/RVC3/tools/rvcprint.py` & `rvc3python-0.9.0/RVC3/tools/rvcprint.py`

 * *Files identical despite different names*

### Comparing `rvc3python-0.2.3/rvc3python.egg-info/PKG-INFO` & `rvc3python-0.9.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,67 +1,100 @@
 Metadata-Version: 2.1
 Name: rvc3python
-Version: 0.2.3
+Version: 0.9.0
 Summary: Support for book: Robotics, Vision & Control 3 in Python
-Home-page: https://github.com/petercorke/RVC3-python
-Author: Peter Corke
-License: MIT
-Project-URL: Documentation, https://petercorke.github.io/RVC3-python
+Author-email: Peter Corke <rvc@petercorke.com>
+Project-URL: Homepage, https://github.com/petercorke/RVC3-python
+Project-URL: Bug Tracker, https://github.com/petercorke/RVC3-python/issues
 Project-URL: Source, https://github.com/petercorke/RVC3-python
-Project-URL: Tracker, https://github.com/petercorke/RVC3-python/issues
-Keywords: robotics,robot,manipulator,robot arm,mobile robot,mobile manipulation,path planning,SLAM,pose graph,Dubins,Reeds-Shepp,lattice planner,RRT,PRM,rapidly exploring random tree,probabilistic roadmap planner,force control,kinematics,Jacobian,position control,velocity control,spatial math,SO(2),SE(2),SO(3),SE(3),twist,product of exponential,translation,orientation,angle-axis,Lie group,skew symmetric matrix,pose,translation,rotation matrix,rigid body transform,homogeneous transformation,Euler angles,roll-pitch-yaw angles,quaternion,unit-quaternioncomputer vision,machine vision,robotic vision,color space,blackbody,image segmentation,blobs,Hough transform,k-means,homography,camera calibration,visual odometry,bundle adjustment,stereo vision,rectification
-Classifier: Development Status :: 4 - Beta
+Keywords: robotics,robot,manipulator,robot arm,mobile robot,mobile manipulation,path planning,SLAM,pose graph,Dubins,Reeds-Shepp,lattice planner,RRT,PRM,rapidly exploring random tree,probabilistic roadmap planner,force control,kinematics,Jacobian,position control,velocity control,spatial math,SO(2),SE(2),SO(3),SE(3),twist,product of exponential,translation,orientation,angle-axis,Lie group,skew symmetric matrix,pose,translation,rotation matrix,rigid body transform,homogeneous transformation,Euler angles,roll-pitch-yaw angles,quaternion,unit-quaternion,computer vision,machine vision,robotic vision,color space,blackbody,image segmentation,blobs,Hough transform,k-means,homography,camera calibration,visual odometry,bundle adjustment,stereo vision,rectification
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: pytorch
 License-File: LICENSE
 
 # Robotics, Vision & Control: 3rd edition in Python (2023)
 [![A Python Robotics Package](https://raw.githubusercontent.com/petercorke/robotics-toolbox-python/master/.github/svg/py_collection.min.svg)](https://github.com/petercorke/robotics-toolbox-python)
 [![QUT Centre for Robotics Open Source](https://github.com/qcr/qcr.github.io/raw/master/misc/badge.svg)](https://qcr.github.io)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 [![PyPI version](https://badge.fury.io/py/rvc3python.svg)](https://badge.fury.io/py/rvc3python)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rvc3python.svg)
 [![PyPI - Downloads](https://img.shields.io/pypi/dw/rvc3python)](https://pypistats.org/packages/rvc3python)
 
-
-coming soon, this is a work in progress, please don't post issues
-
+<table style="border:0px">
+<tr style="border:0px">
+<td style="border:0px">
 <img src="https://github.com/petercorke/RVC3-python/raw/main/doc/frontcover.png" alt="Front cover 978-3-031-06468-5_5208" width="300">
+</td>
+<td style="border:0px">
+Welcome to the online hub for the book:
+<ul type="none">
+<li><b>Robotics, Vision & Control</b>: fundamental algorithms in Python (3rd edition) 
+<li>Peter Corke, published by Springer-Nature 2023.</li>
+<li><b>ISBN</b> 978-3-031-06468-5 (hardcopy), 978-3-031-06469-2 (eBook)</li>
+<li><b>DOI</b> <a href="https://doi.org/10.1007/978-3-031-06469-2">10.1007/978-3-031-06469-2</a></li>
+</ul>
+<br><br>
+<p>Report an issue with the book or its supporting code <a href="https://github.com/petercorke/RVC3-python/issues/new/choose">here</a>.</p>
+
+<p>Knwon errata for the book can be viewed <a href="https://github.com/petercorke/RVC3-python/wiki/Errata">here</a>.</p>
+</td>
+</tr>
+</table>
+
 
-This book depends on the following open-source Python packages
+This book uses many examples based on the following open-source Python packages
 
-<a href="https://github.com/petercorke/robotics-toolbox-python"><img alt="Robotics Toolbox for Python" src="https://github.com/petercorke/robotics-toolbox-python/raw/master/docs/figs/RobToolBox_RoundLogoB.png" width="150"></a>
+<a href="https://github.com/petercorke/robotics-toolbox-python"><img alt="Robotics Toolbox for Python" src="https://github.com/petercorke/robotics-toolbox-python/raw/master/docs/figs/RobToolBox_RoundLogoB.png" width="130"></a>
 <a href="https://github.com/petercorke/machinevision-toolbox-python"><img alt="Machine Vision Toolbox for Python" src="https://github.com/petercorke/machinevision-toolbox-python/raw/master/figs/VisionToolboxLogo_NoBackgnd@2x.png" width="150"></a>
+<a href="https://github.com/petercorke/spatialmath-python"><img alt="Spatial Maths Toolbox for Python" src="https://github.com/petercorke/spatialmath-python/raw/master/docs/figs/CartesianSnakes_LogoW.png" width="130"></a>
+<a href="https://github.com/petercorke/bdsim"><img alt="Block diagram simulation for Python" src="https://github.com/petercorke/bdsim/raw/master/figs/BDSimLogo_NoBackgnd@2x.png" width="250"></a>
 
-which in turn have dependencies on other packages created by the author and
+**Robotics Toolbox for Python**, **Machine Vision Toolbox for Python**, **Spatial Maths Toolbox for Python**, **Block Diagram Simulation for Python**.  These in turn have dependencies on other packages created by the author and
 third parties.
 
 ## Installing the package
 
-This package provides a simple one-step installation of the required Toolboxes
+This package provides a simple one-step installation of *all* the required Toolboxes
 ```shell
 pip install rvc3python
 ```
 or
 ```shell
 conda install rvc3python
 ```
 
+There are a lot of dependencies and this might take a minute or so.  You now have a very
+powerful computing environment for robotics and computer vision.
+
+### Python version
+
+Given the rapid rate of language additions, particularly around type hinting, use at
+least Python 3.8.  Python 3.7 goes end of life in June 2023.
+
+Not all package dependencies will work with the latest release of Python.  In particular, check:
+* [PyTorch](https://pypi.org/project/torch/) used for segmentation examples in Chapter 12
+* [Open3D](https://pypi.org/project/open3d), used for point cloud examples in Chapter 14.
+
 ### Installing into a Conda environment
 
 It's probably a good idea to create a virtual environment to keep this package
-and its dependencies separated from your other Python code and projects.  This
-is really easy using Conda conda, and only adds a couple of extra lines
+and its dependencies separated from your other Python code and projects.  If you've
+never used virtual environments before this might be a good time to start, and it
+is really easy [using Conda](https://conda.io/projects/conda/en/latest/user-guide/install/index.html):
 ```shell
 conda create -n RVC3 python=3.10
 conda activate RVC3
 pip install rvc3python
 ```
 
 ### Installing deep learning tools
@@ -83,44 +116,51 @@
 $ rvctool
  ____       _           _   _             __     ___     _                ___      ____            _             _   _____ 
 |  _ \ ___ | |__   ___ | |_(_) ___ ___    \ \   / (_)___(_) ___  _ __    ( _ )    / ___|___  _ __ | |_ _ __ ___ | | |___ / 
 | |_) / _ \| '_ \ / _ \| __| |/ __/ __|    \ \ / /| / __| |/ _ \| '_ \   / _ \/\ | |   / _ \| '_ \| __| '__/ _ \| |   |_ \ 
 |  _ < (_) | |_) | (_) | |_| | (__\__ \_    \ V / | \__ \ | (_) | | | | | (_>  < | |__| (_) | | | | |_| | | (_) | |  ___) |
 |_| \_\___/|_.__/ \___/ \__|_|\___|___( )    \_/  |_|___/_|\___/|_| |_|  \___/\/  \____\___/|_| |_|\__|_|  \___/|_| |____/ 
                                       |/                                                                                   
-for Python (RTB==1.0.2, MVTB==0.9.1, SMTB==1.0.0)
-
-import numpy as np
-import scipy as sp
-import matplotlib.pyplot as plt
-from math import pi
-from spatialmath import *
-from spatialmath.base import *
-from roboticstoolbox import *
-from machinevisiontoolbox import *
-import machinevisiontoolbox.base as mvbase
-
-func/object?       - show brief help
-help(func/object)  - show detailed help
-func/object??      - show source code
+                                                                                 
+for Python (RTB==1.1.0, MVTB==0.9.5, SG==1.1.7, SMTB==1.1.7, NumPy==1.24.2, SciPy==1.10.1, Matplotlib==3.7.1)
 
+    import math
+    import numpy as np
+    from scipy import linalg, optimize
+    import matplotlib.pyplot as plt
+    from spatialmath import *
+    from spatialmath.base import *
+    from spatialmath.base import sym
+    from spatialgeometry import *
+    from roboticstoolbox import *
+    from machinevisiontoolbox import *
+    import machinevisiontoolbox.base as mvb
+    
+    # useful variables
+    from math import pi
+    puma = models.DH.Puma560()
+    panda = models.DH.Panda()
+
+    func/object?       - show brief help
+    help(func/object)  - show detailed help
+    func/object??      - show source code
 
 Results of assignments will be displayed, use trailing ; to suppress
-
- 
-Python 3.8.5 (default, Sep  4 2020, 02:22:02) 
+    
+Python 3.10.9 | packaged by conda-forge | (main, Feb  2 2023, 20:24:27) [Clang 14.0.6 ]
 Type 'copyright', 'credits' or 'license' for more information
-IPython 8.0.1 -- An enhanced Interactive Python. Type '?' for help.
+IPython 8.11.0 -- An enhanced Interactive Python. Type '?' for help.
 
 
 >>> 
 ```
 
-This provides an interactive Python (IPython) session with all the Toolboxes
-preloaded, and ready to go.  It's a highly capable, convenient, and
+This provides an interactive Python
+([IPython](https://ipython.readthedocs.io/en/stable)) session with all the Toolboxes and
+supporting packages imported, and ready to go.  It's a highly capable, convenient, and
 "MATLAB-like" workbench environment for robotics and computer vision.
 
 For example to load an ETS model of a Panda robot, solve a forward kinematics
 and inverse kinematics problem, and an interactive graphical display is simply:
 
 ```python
 >>> panda = models.ETS.Panda()
@@ -172,37 +212,82 @@
 >>> matches = sf1.match(sf2)
 >>> matches.subset(100).plot("w")
 ```
 ![](https://github.com/petercorke/machinevision-toolbox-python/raw/master/figs/matching.png)
 
 `rvctool` is a wrapper around
 [IPython](https://ipython.readthedocs.io/en/stable) where:
-- functions and classes can be accessed without needing package prefixes
+- robotics and vision functions and classes can be accessed without needing
+  package prefixes
 - results are displayed by default like MATLAB does, and like MATLAB you need to
   put a semicolon on the end of the line to prevent this
 - the prompt is the standard Python REPL prompt `>>>` rather than the IPython
   prompt, this can be overridden by a command-line switch
 - allows cutting and pasting in lines from the book, and prompt characters are
   ignored
 
 The Robotics, Vision & Control book uses `rvctool` for all the included
 examples.
 
 `rvctool` imports the all the above mentioned packages using `import *` which is
 not considered best Python practice.  It is very convenient for interactive
-experimentation, but in your own code you can control the imports as you see
+experimentation, but in your own code you can handle the imports as you see
 fit.
 
+### Cutting and pasting
+
+IPython is very forgiving when it comes to cutting and pasting in blocks of Python
+code.  It will strip off the `>>>` prompt character and ignore indentation.  The normal
+python REPL is not so forgiving.  IPython also allows maintains a command history and
+allows command editing.
+### Simple scripting
+You can write very simple scripts, for example `test.py` is
+
+```python
+T = puma.fkine(puma.qn)
+sol = puma.ikine_LM(T)
+sol.q
+puma.plot(sol.q);
+```
+
+then 
+
+```shell
+$ rvctool test.py
+   0         0         1         0.5963    
+   0         1         0        -0.1501    
+  -1         0         0         0.6575    
+   0         0         0         1         
+
+IKSolution(q=array([7.235e-08,  -0.8335,  0.09396,    3.142,   0.8312,   -3.142]), success=True, iterations=15, searches=1, residual=1.406125546650288e-07, reason='Success')
+array([7.235e-08,  -0.8335,  0.09396,    3.142,   0.8312,   -3.142])
+PyPlot3D backend, t = 0.05, scene:
+  robot: Text(0.0, 0.0, 'Puma 560')
+>>>
+```
+and you are dropped into an IPython session after the script has run.
+
+## Using Jupyter and Colab
+
+Graphics and animations are problematic in these environments, some things work
+well, some don't.  As much as possible I've tweaked the Jupyter notebooks to work
+as best they can in these environments.
+
+For local use the [Jupyter plugin for Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter) is pretty decent.  Colab suffers
+from old versions of major packages (though they are getting better at keeping up to date)
+and animations can suffer from slow update over the network.
 ## Other command line tools
 
-This package provides additional command line tools including:
+Additional command line tools available (from the Robotics Toolbox) include:
 - `eigdemo`, animation showing linear transformation of a rotating unit vector
   which demonstrates eigenvalues and eigenvectors.
-- `tripleangledemo`, experiment with various triple-angle sequences.
-- `twistdemo`, experiment with 3D twists.
+- `tripleangledemo`, Swift visualization that lets you experiment with various triple-angle sequences.
+- `twistdemo`, Swift visualization that lets you experiment with 3D twists. The screw axis is the blue rod and you can
+   position and orient it using the sliders, and adjust its pitch. Then apply a rotation
+   about the screw using the bottom slider.
 # Block diagram models
 
 <a href="https://github.com/petercorke/bdsim"><img
 src="https://github.com/petercorke/bdsim/raw/master/figs/BDSimLogo_NoBackgnd%402x.png"
 alt="bdsim logo" width="300"></a>
 
 Block diagram models are key to the pedagogy of the RVC3 book and 25 models are
@@ -242,11 +327,11 @@
 - The code to produce every Python/Matplotlib (2D) figure in the book, see the [`figures`](figures) folder
 - 3D points clouds from chapter 14, and the code to create them, see
   the [`pointclouds`](../pointclouds) folder.
 - 3D figures from chapters 2-3, 7-9, and the code to create them, see the [`3dfigures`](../3dfigures) folder.
 - All example scripts, see the [`examples`](examples) folder.
 - To run the visual odometry example in Sect. 14.8.3 you need to download two image sequence, each over 100MB, [see the instructions here](https://github.com/petercorke/machinevision-toolbox-python/blob/master/mvtb-data/README.md#install-big-image-files). 
 
-To get this material you must clone the repo
+To get that material you must clone the repo
 ```shell
 git clone https://github.com/petercorke/RVC3-python.git
 ```
```

#### html2text {}

```diff
@@ -1,78 +1,110 @@
-Metadata-Version: 2.1 Name: rvc3python Version: 0.2.3 Summary: Support for
-book: Robotics, Vision & Control 3 in Python Home-page: https://github.com/
-petercorke/RVC3-python Author: Peter Corke License: MIT Project-URL:
-Documentation, https://petercorke.github.io/RVC3-python Project-URL: Source,
-https://github.com/petercorke/RVC3-python Project-URL: Tracker, https://
-github.com/petercorke/RVC3-python/issues Keywords:
+Metadata-Version: 2.1 Name: rvc3python Version: 0.9.0 Summary: Support for
+book: Robotics, Vision & Control 3 in Python Author-email: Peter Corke
+petercorke.com> Project-URL: Homepage, https://github.com/petercorke/RVC3-
+python Project-URL: Bug Tracker, https://github.com/petercorke/RVC3-python/
+issues Project-URL: Source, https://github.com/petercorke/RVC3-python Keywords:
 robotics,robot,manipulator,robot arm,mobile robot,mobile manipulation,path
 planning,SLAM,pose graph,Dubins,Reeds-Shepp,lattice planner,RRT,PRM,rapidly
 exploring random tree,probabilistic roadmap planner,force
 control,kinematics,Jacobian,position control,velocity control,spatial math,SO
 (2),SE(2),SO(3),SE(3),twist,product of
 exponential,translation,orientation,angle-axis,Lie group,skew symmetric
 matrix,pose,translation,rotation matrix,rigid body transform,homogeneous
 transformation,Euler angles,roll-pitch-yaw angles,quaternion,unit-
-quaternioncomputer vision,machine vision,robotic vision,color
+quaternion,computer vision,machine vision,robotic vision,color
 space,blackbody,image segmentation,blobs,Hough transform,k-
 means,homography,camera calibration,visual odometry,bundle adjustment,stereo
-vision,rectification Classifier: Development Status :: 4 - Beta Classifier:
-Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
-License Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Requires-Python: >=3.7 Description-Content-Type: text/markdown
+vision,rectification Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers Classifier: Programming Language ::
+Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+License :: OSI Approved :: MIT License Classifier: Operating System :: OS
+Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
 Provides-Extra: pytorch License-File: LICENSE # Robotics, Vision & Control: 3rd
 edition in Python (2023) [![A Python Robotics Package](https://
 raw.githubusercontent.com/petercorke/robotics-toolbox-python/master/.github/
 svg/py_collection.min.svg)](https://github.com/petercorke/robotics-toolbox-
 python) [![QUT Centre for Robotics Open Source](https://github.com/qcr/
 qcr.github.io/raw/master/misc/badge.svg)](https://qcr.github.io) [![License:
 MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://
 opensource.org/licenses/MIT) [![PyPI version](https://badge.fury.io/py/
 rvc3python.svg)](https://badge.fury.io/py/rvc3python) ![PyPI - Python Version]
 (https://img.shields.io/pypi/pyversions/rvc3python.svg) [![PyPI - Downloads]
 (https://img.shields.io/pypi/dw/rvc3python)](https://pypistats.org/packages/
-rvc3python) coming soon, this is a work in progress, please don't post issues
-[Front cover 978-3-031-06468-5_5208] This book depends on the following open-
-source Python packages [Robotics_Toolbox_for_Python] [Machine_Vision_Toolbox
-for_Python] which in turn have dependencies on other packages created by the
-author and third parties. ## Installing the package This package provides a
-simple one-step installation of the required Toolboxes ```shell pip install
-rvc3python ``` or ```shell conda install rvc3python ``` ### Installing into a
-Conda environment It's probably a good idea to create a virtual environment to
-keep this package and its dependencies separated from your other Python code
-and projects. This is really easy using Conda conda, and only adds a couple of
-extra lines ```shell conda create -n RVC3 python=3.10 conda activate RVC3 pip
-install rvc3python ``` ### Installing deep learning tools Chapter 11 has some
-deep learning examples based on PyTorch. If you don't have PyTorch installed
-you can use the `pytorch` install option ```shell pip install rvc3python
-[pytorch] ``` or ```shell conda install rvc3python[pytorch] ``` ## Using the
-Toolboxes The simplest way to get going is to use the command line tool
-```shell $ rvctool ____ _ _ _ __ ___ _ ___ ____ _ _ _____ | _ \ ___ | |__ ___ |
-|_(_) ___ ___ \ \ / (_)___(_) ___ _ __ ( _ ) / ___|___ _ __ | |_ _ __ ___ | |
-|___ / | |_) / _ \| '_ \ / _ \| __| |/ __/ __| \ \ / /| / __| |/ _ \| '_ \ / _
-\/\ | | / _ \| '_ \| __| '__/ _ \| | |_ \ | _ < (_) | |_) | (_) | |_| | (__\__
-\_ \ V / | \__ \ | (_) | | | | | (_> < | |__| (_) | | | | |_| | | (_) | | ___)
-| |_| \_\___/|_.__/ \___/ \__|_|\___|___( ) \_/ |_|___/_|\___/|_| |_| \___/\/
-\____\___/|_| |_|\__|_| \___/|_| |____/ |/ for Python (RTB==1.0.2, MVTB==0.9.1,
-SMTB==1.0.0) import numpy as np import scipy as sp import matplotlib.pyplot as
-plt from math import pi from spatialmath import * from spatialmath.base import
-* from roboticstoolbox import * from machinevisiontoolbox import * import
-machinevisiontoolbox.base as mvbase func/object? - show brief help help(func/
-object) - show detailed help func/object?? - show source code Results of
-assignments will be displayed, use trailing ; to suppress Python 3.8.5
-(default, Sep 4 2020, 02:22:02) Type 'copyright', 'credits' or 'license' for
-more information IPython 8.0.1 -- An enhanced Interactive Python. Type '?' for
-help. >>> ``` This provides an interactive Python (IPython) session with all
-the Toolboxes preloaded, and ready to go. It's a highly capable, convenient,
-and "MATLAB-like" workbench environment for robotics and computer vision. For
-example to load an ETS model of a Panda robot, solve a forward kinematics and
-inverse kinematics problem, and an interactive graphical display is simply:
-```python >>> panda = models.ETS.Panda() ERobot: Panda (by Franka Emika), 7
-joints (RRRRRRR)
+rvc3python)
+                                     Welcome to the online hub for the book:
+                                         # Robotics, Vision & Control:
+                                           fundamental algorithms in Python
+                                           (3rd edition)
+                                         # Peter Corke, published by Springer-
+                                           Nature 2023.
+                                         # ISBN 978-3-031-06468-5 (hardcopy),
+[Front cover 978-3-031-06468-5_5208]       978-3-031-06469-2 (eBook)
+                                         # DOI 10.1007/978-3-031-06469-2
+
+
+                                     Report an issue with the book or its
+                                     supporting code here.
+                                     Knwon errata for the book can be viewed
+                                     here.
+This book uses many examples based on the following open-source Python packages
+[Robotics_Toolbox_for_Python] [Machine_Vision_Toolbox_for_Python] [Spatial
+Maths_Toolbox_for_Python] [Block_diagram_simulation_for_Python] **Robotics
+Toolbox for Python**, **Machine Vision Toolbox for Python**, **Spatial Maths
+Toolbox for Python**, **Block Diagram Simulation for Python**. These in turn
+have dependencies on other packages created by the author and third parties. ##
+Installing the package This package provides a simple one-step installation of
+*all* the required Toolboxes ```shell pip install rvc3python ``` or ```shell
+conda install rvc3python ``` There are a lot of dependencies and this might
+take a minute or so. You now have a very powerful computing environment for
+robotics and computer vision. ### Python version Given the rapid rate of
+language additions, particularly around type hinting, use at least Python 3.8.
+Python 3.7 goes end of life in June 2023. Not all package dependencies will
+work with the latest release of Python. In particular, check: * [PyTorch]
+(https://pypi.org/project/torch/) used for segmentation examples in Chapter 12
+* [Open3D](https://pypi.org/project/open3d), used for point cloud examples in
+Chapter 14. ### Installing into a Conda environment It's probably a good idea
+to create a virtual environment to keep this package and its dependencies
+separated from your other Python code and projects. If you've never used
+virtual environments before this might be a good time to start, and it is
+really easy [using Conda](https://conda.io/projects/conda/en/latest/user-guide/
+install/index.html): ```shell conda create -n RVC3 python=3.10 conda activate
+RVC3 pip install rvc3python ``` ### Installing deep learning tools Chapter 11
+has some deep learning examples based on PyTorch. If you don't have PyTorch
+installed you can use the `pytorch` install option ```shell pip install
+rvc3python[pytorch] ``` or ```shell conda install rvc3python[pytorch] ``` ##
+Using the Toolboxes The simplest way to get going is to use the command line
+tool ```shell $ rvctool ____ _ _ _ __ ___ _ ___ ____ _ _ _____ | _ \ ___ | |__
+___ | |_(_) ___ ___ \ \ / (_)___(_) ___ _ __ ( _ ) / ___|___ _ __ | |_ _ __ ___
+| | |___ / | |_) / _ \| '_ \ / _ \| __| |/ __/ __| \ \ / /| / __| |/ _ \| '_ \
+/ _ \/\ | | / _ \| '_ \| __| '__/ _ \| | |_ \ | _ < (_) | |_) | (_) | |_| |
+(__\__ \_ \ V / | \__ \ | (_) | | | | | (_> < | |__| (_) | | | | |_| | | (_) |
+| ___) | |_| \_\___/|_.__/ \___/ \__|_|\___|___( ) \_/ |_|___/_|\___/|_| |_|
+\___/\/ \____\___/|_| |_|\__|_| \___/|_| |____/ |/ for Python (RTB==1.1.0,
+MVTB==0.9.5, SG==1.1.7, SMTB==1.1.7, NumPy==1.24.2, SciPy==1.10.1,
+Matplotlib==3.7.1) import math import numpy as np from scipy import linalg,
+optimize import matplotlib.pyplot as plt from spatialmath import * from
+spatialmath.base import * from spatialmath.base import sym from spatialgeometry
+import * from roboticstoolbox import * from machinevisiontoolbox import *
+import machinevisiontoolbox.base as mvb # useful variables from math import pi
+puma = models.DH.Puma560() panda = models.DH.Panda() func/object? - show brief
+help help(func/object) - show detailed help func/object?? - show source code
+Results of assignments will be displayed, use trailing ; to suppress Python
+3.10.9 | packaged by conda-forge | (main, Feb 2 2023, 20:24:27) [Clang 14.0.6 ]
+Type 'copyright', 'credits' or 'license' for more information IPython 8.11.0 -
+- An enhanced Interactive Python. Type '?' for help. >>> ``` This provides an
+interactive Python ([IPython](https://ipython.readthedocs.io/en/stable))
+session with all the Toolboxes and supporting packages imported, and ready to
+go. It's a highly capable, convenient, and "MATLAB-like" workbench environment
+for robotics and computer vision. For example to load an ETS model of a Panda
+robot, solve a forward kinematics and inverse kinematics problem, and an
+interactive graphical display is simply: ```python >>> panda = models.ETS.Panda
+() ERobot: Panda (by Franka Emika), 7 joints (RRRRRRR)
 âââââââ¬ââââââââ¬ââââââââ¬âââââââââ¬ââââââââââââââââââââââââââââââââââââââââââââââ
 âlink â link â joint â parent â ETS: parent to link â
 âââââââ¼ââââââââ¼ââââââââ¼âââââââââ¼ââââââââââââââââââââââââââââââââââââââââââââââ¤
 â 0 â link0 â 0 â BASE â tz(0.333) â Rz(q0) â â 1 â link1 â
 1 â link0 â Rx(-90Â°) â Rz(q1) â â 2 â link2 â 2 â link1 â Rx
 (90Â°) â tz(0.316) â Rz(q2) â â 3 â link3 â 3 â link2 â tx
 (0.0825) â Rx(90Â°) â Rz(q3) â â 4 â link4 â 4 â link3 â tx(-
@@ -98,47 +130,70 @@
 (sigma=5)]).disp() ``` ![](https://github.com/petercorke/machinevision-toolbox-
 python/raw/master/figs/mona%2Bsmooth.png) or load two images of the same scene,
 compute SIFT features and display putative matches ```python >>> sf1 =
 Image.Read("eiffel-1.png", mono=True).SIFT() >>> sf2 = Image.Read("eiffel-
 2.png", mono=True).SIFT() >>> matches = sf1.match(sf2) >>> matches.subset
 (100).plot("w") ``` ![](https://github.com/petercorke/machinevision-toolbox-
 python/raw/master/figs/matching.png) `rvctool` is a wrapper around [IPython]
-(https://ipython.readthedocs.io/en/stable) where: - functions and classes can
-be accessed without needing package prefixes - results are displayed by default
-like MATLAB does, and like MATLAB you need to put a semicolon on the end of the
-line to prevent this - the prompt is the standard Python REPL prompt `>>>`
-rather than the IPython prompt, this can be overridden by a command-line switch
-- allows cutting and pasting in lines from the book, and prompt characters are
-ignored The Robotics, Vision & Control book uses `rvctool` for all the included
-examples. `rvctool` imports the all the above mentioned packages using `import
-*` which is not considered best Python practice. It is very convenient for
-interactive experimentation, but in your own code you can control the imports
-as you see fit. ## Other command line tools This package provides additional
-command line tools including: - `eigdemo`, animation showing linear
-transformation of a rotating unit vector which demonstrates eigenvalues and
-eigenvectors. - `tripleangledemo`, experiment with various triple-angle
-sequences. - `twistdemo`, experiment with 3D twists. # Block diagram models
-[bdsim_logo] Block diagram models are key to the pedagogy of the RVC3 book and
-25 models are included. To simulate these models we use the Python package
-[bdsim](https://github.com/petercorke/bdsim) which can run models: - written in
-Python using [bdsim](https://github.com/petercorke/bdsim#getting-started)
-blocks and wiring. - created graphically using [bdedit](https://github.com/
-petercorke/bdsim#bdedit-the-graphical-editing-tool) and saved as a `.bd` (JSON
-format) file. The models are included in the `RVC3` package when it is
-installed and `rvctool` adds them to the module search path. This means you can
-invoke them from `rvctool` by ```python >>> %run -m vloop_test ``` If you want
-to directly access the folder containing the models, the command line tool
-```shell bdsim_path ``` will display the full path to where they have been
-installed in the Python package tree. # Additional book resources [Front cover
-978-3-031-06468-5_5208] This GitHub repo provides additional resources for
-readers including: - Jupyter notebooks containing all code lines from each
-chapter, see the [`notebooks`](notebooks) folder - The code to produce every
-Python/Matplotlib (2D) figure in the book, see the [`figures`](figures) folder
-- 3D points clouds from chapter 14, and the code to create them, see the
-[`pointclouds`](../pointclouds) folder. - 3D figures from chapters 2-3, 7-9,
-and the code to create them, see the [`3dfigures`](../3dfigures) folder. - All
-example scripts, see the [`examples`](examples) folder. - To run the visual
-odometry example in Sect. 14.8.3 you need to download two image sequence, each
-over 100MB, [see the instructions here](https://github.com/petercorke/
-machinevision-toolbox-python/blob/master/mvtb-data/README.md#install-big-image-
-files). To get this material you must clone the repo ```shell git clone https:/
-/github.com/petercorke/RVC3-python.git ```
+(https://ipython.readthedocs.io/en/stable) where: - robotics and vision
+functions and classes can be accessed without needing package prefixes -
+results are displayed by default like MATLAB does, and like MATLAB you need to
+put a semicolon on the end of the line to prevent this - the prompt is the
+standard Python REPL prompt `>>>` rather than the IPython prompt, this can be
+overridden by a command-line switch - allows cutting and pasting in lines from
+the book, and prompt characters are ignored The Robotics, Vision & Control book
+uses `rvctool` for all the included examples. `rvctool` imports the all the
+above mentioned packages using `import *` which is not considered best Python
+practice. It is very convenient for interactive experimentation, but in your
+own code you can handle the imports as you see fit. ### Cutting and pasting
+IPython is very forgiving when it comes to cutting and pasting in blocks of
+Python code. It will strip off the `>>>` prompt character and ignore
+indentation. The normal python REPL is not so forgiving. IPython also allows
+maintains a command history and allows command editing. ### Simple scripting
+You can write very simple scripts, for example `test.py` is ```python T =
+puma.fkine(puma.qn) sol = puma.ikine_LM(T) sol.q puma.plot(sol.q); ``` then
+```shell $ rvctool test.py 0 0 1 0.5963 0 1 0 -0.1501 -1 0 0 0.6575 0 0 0 1
+IKSolution(q=array([7.235e-08, -0.8335, 0.09396, 3.142, 0.8312, -3.142]),
+success=True, iterations=15, searches=1, residual=1.406125546650288e-07,
+reason='Success') array([7.235e-08, -0.8335, 0.09396, 3.142, 0.8312, -3.142])
+PyPlot3D backend, t = 0.05, scene: robot: Text(0.0, 0.0, 'Puma 560') >>> ```
+and you are dropped into an IPython session after the script has run. ## Using
+Jupyter and Colab Graphics and animations are problematic in these
+environments, some things work well, some don't. As much as possible I've
+tweaked the Jupyter notebooks to work as best they can in these environments.
+For local use the [Jupyter plugin for Visual Studio Code](https://
+marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter) is pretty
+decent. Colab suffers from old versions of major packages (though they are
+getting better at keeping up to date) and animations can suffer from slow
+update over the network. ## Other command line tools Additional command line
+tools available (from the Robotics Toolbox) include: - `eigdemo`, animation
+showing linear transformation of a rotating unit vector which demonstrates
+eigenvalues and eigenvectors. - `tripleangledemo`, Swift visualization that
+lets you experiment with various triple-angle sequences. - `twistdemo`, Swift
+visualization that lets you experiment with 3D twists. The screw axis is the
+blue rod and you can position and orient it using the sliders, and adjust its
+pitch. Then apply a rotation about the screw using the bottom slider. # Block
+diagram models [bdsim_logo] Block diagram models are key to the pedagogy of the
+RVC3 book and 25 models are included. To simulate these models we use the
+Python package [bdsim](https://github.com/petercorke/bdsim) which can run
+models: - written in Python using [bdsim](https://github.com/petercorke/
+bdsim#getting-started) blocks and wiring. - created graphically using [bdedit]
+(https://github.com/petercorke/bdsim#bdedit-the-graphical-editing-tool) and
+saved as a `.bd` (JSON format) file. The models are included in the `RVC3`
+package when it is installed and `rvctool` adds them to the module search path.
+This means you can invoke them from `rvctool` by ```python >>> %run -
+m vloop_test ``` If you want to directly access the folder containing the
+models, the command line tool ```shell bdsim_path ``` will display the full
+path to where they have been installed in the Python package tree. # Additional
+book resources [Front cover 978-3-031-06468-5_5208] This GitHub repo provides
+additional resources for readers including: - Jupyter notebooks containing all
+code lines from each chapter, see the [`notebooks`](notebooks) folder - The
+code to produce every Python/Matplotlib (2D) figure in the book, see the
+[`figures`](figures) folder - 3D points clouds from chapter 14, and the code to
+create them, see the [`pointclouds`](../pointclouds) folder. - 3D figures from
+chapters 2-3, 7-9, and the code to create them, see the [`3dfigures`](../
+3dfigures) folder. - All example scripts, see the [`examples`](examples)
+folder. - To run the visual odometry example in Sect. 14.8.3 you need to
+download two image sequence, each over 100MB, [see the instructions here]
+(https://github.com/petercorke/machinevision-toolbox-python/blob/master/mvtb-
+data/README.md#install-big-image-files). To get that material you must clone
+the repo ```shell git clone https://github.com/petercorke/RVC3-python.git ```
```

### Comparing `rvc3python-0.2.3/setup.py` & `rvc3python-0.9.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,81 +1,91 @@
-from setuptools import setup, find_packages
-import os
-
+[project]
+name = "rvc3python"
+version = "0.9.0"
+authors = [
+  { name="Peter Corke", email="rvc@petercorke.com" },
+]
+description = "Support for book: Robotics, Vision & Control 3 in Python"
+readme = "README.md"
+requires-python = ">=3.7"
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    # Indicate who your project is intended for
+    "Intended Audience :: Developers",
+    # Specify the Python versions you support here.
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 
-here = os.path.abspath(os.path.dirname(__file__))
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+keywords = [
+    "robotics", "robot", "manipulator", "robot arm", 
+    "mobile robot", "mobile manipulation",
+    "path planning", "SLAM", "pose graph", 
+    "Dubins", "Reeds-Shepp", "lattice planner", "RRT", "PRM",
+    "rapidly exploring random tree", "probabilistic roadmap planner",
+    "force control", "kinematics", "Jacobian", "position control", "velocity control",
+    "spatial math", 
+    "SO(2)", "SE(2)", "SO(3)", "SE(3)",
+    "twist", "product of exponential", "translation", "orientation",
+    "angle-axis", "Lie group", "skew symmetric matrix",
+    "pose", "translation", "rotation matrix", "rigid body transform", "homogeneous transformation",
+    "Euler angles", "roll-pitch-yaw angles", "quaternion", "unit-quaternion",
+    "computer vision", "machine vision", "robotic vision",
+    "color space", "blackbody", "image segmentation", "blobs",
+    "Hough transform", "k-means", "homography", "camera calibration", "visual odometry",
+    "bundle adjustment",  "stereo vision", "rectification",
+]
 
-req = [
+dependencies = [
     "matplotlib",
     "roboticstoolbox-python >= 1",
     "machinevision-toolbox-python",
-    "bdsim",
+    "bdsim >= 1.1",
     "IPython",
     "sympy",
+    "pybullet",
 ]
 
-pytorch_req = [
+[project.urls]
+"Homepage" = "https://github.com/petercorke/RVC3-python"
+"Bug Tracker" = "https://github.com/petercorke/RVC3-python/issues"
+"Source" = "https://github.com/petercorke/RVC3-python"
+
+[project.optional-dependencies]
+
+pytorch = [
     "torch",
     "torchvision",
 ]
 
-# Get the long description from the README file
-with open(os.path.join(here, "README.md"), encoding="utf-8") as f:
-    long_description = f.read()
-
-setup(
-    name="rvc3python",
-    version="0.2.3",
-    description="Support for book: Robotics, Vision & Control 3 in Python",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/petercorke/RVC3-python",
-    author="Peter Corke",
-    license="MIT",
-    classifiers=[
-        #   3 - Alpha
-        #   4 - Beta
-        #   5 - Production/Stable
-        "Development Status :: 4 - Beta",
-        # Indicate who your project is intended for
-        "Intended Audience :: Developers",
-        # Pick your license as you wish (should match "license" above)
-        "License :: OSI Approved :: MIT License",
-        # Specify the Python versions you support here. In particular, ensure
-        # that you indicate whether you support Python 2, Python 3 or both.
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-    ],
-    python_requires=">=3.7",
-    project_urls={
-        "Documentation": "https://petercorke.github.io/RVC3-python",
-        "Source": "https://github.com/petercorke/RVC3-python",
-        "Tracker": "https://github.com/petercorke/RVC3-python/issues",
-    },
-    keywords=["robotics", "robot", "manipulator", "robot arm", 
-        "mobile robot", "mobile manipulation",
-        "path planning", "SLAM", "pose graph", 
-        "Dubins", "Reeds-Shepp", "lattice planner", "RRT", "PRM",
-        "rapidly exploring random tree", "probabilistic roadmap planner",
-        "force control", "kinematics", "Jacobian", "position control", "velocity control",
-        "spatial math", 
-        "SO(2)", "SE(2)", "SO(3)", "SE(3)",
-        "twist", "product of exponential", "translation", "orientation",
-        "angle-axis", "Lie group", "skew symmetric matrix",
-        "pose", "translation", "rotation matrix", "rigid body transform", "homogeneous transformation",
-        "Euler angles", "roll-pitch-yaw angles", "quaternion", "unit-quaternion"
-        "computer vision", "machine vision", "robotic vision",
-        "color space", "blackbody", "image segmentation", "blobs",
-        "Hough transform", "k-means", "homography", "camera calibration", "visual odometry",
-        "bundle adjustment",  "stereo vision", "rectification"
-        ],
-    #packages=["RVC3"],
-    packages=find_packages(),
-    # package_data={"roboticstoolbox": extra_files},
-    # include_package_data=False,
-    scripts=["RVC3/bin/rvctool", "RVC3/bin/bdsim_path"],
-    install_requires=req,
-    extras_require={
-            "pytorch": pytorch_req,
-    },
-)
+[project.scripts]
+
+rvctool = "RVC3.bin.rvctool:main"
+bdsim_path = "RVC3.bin.bdsim_path:main"
+
+
+[build-system]
+
+requires = ["setuptools", "oldest-supported-numpy"]
+build-backend = "setuptools.build_meta"
+
+# [tool.setuptools.packages.find]
+# where = ["."]
+
+[tool.setuptools.package-data]
+models = ["*.bd"]
+
+[tool.setuptools]
+ 
+packages = [
+    "RVC3",
+    "RVC3.examples",
+    "RVC3.tools",
+    "RVC3.bin",
+    "RVC3.models",
+]
+
```

