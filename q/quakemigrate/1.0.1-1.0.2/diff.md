# Comparing `tmp/quakemigrate-1.0.1.tar.gz` & `tmp/quakemigrate-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quakemigrate-1.0.1.tar", last modified: Mon Apr 10 15:49:27 2023, max compression
+gzip compressed data, was "quakemigrate-1.0.2.tar", last modified: Mon May 15 23:35:44 2023, max compression
```

## Comparing `quakemigrate-1.0.1.tar` & `quakemigrate-1.0.2.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:49:27.421152 quakemigrate-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-10 15:49:14.000000 quakemigrate-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-10 15:49:14.000000 quakemigrate-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7702 2023-04-10 15:49:27.421152 quakemigrate-1.0.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     6220 2023-04-10 15:49:14.000000 quakemigrate-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:49:27.413152 quakemigrate-1.0.1/quakemigrate/
--rwxr-xr-x   0 runner    (1001) docker     (123)      773 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/quakemigrate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:49:27.413152 quakemigrate-1.0.1/quakemigrate/core/
--rwxr-xr-x   0 runner    (1001) docker     (123)      673 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/quakemigrate/core/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4278 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/quakemigrate/core/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/quakemigrate/core/libnames.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:49:27.417152 quakemigrate-1.0.1/quakemigrate/core/src/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/quakemigrate/core/src/qmlib.def
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/quakemigrate/core/src/qmlib.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     3929 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/quakemigrate/core/src/quakemigrate.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:49:27.417152 quakemigrate-1.0.1/quakemigrate/export/
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/quakemigrate/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/quakemigrate/export/to_mfast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/quakemigrate/export/to_nlloc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11553 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/quakemigrate/export/to_obspy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/quakemigrate/export/to_snuffler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:49:27.417152 quakemigrate-1.0.1/quakemigrate/io/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1845 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/quakemigrate/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/quakemigrate/io/amplitudes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/quakemigrate/io/availability.py
--rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/quakemigrate/io/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6919 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/quakemigrate/io/cut_waveforms.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    30763 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/quakemigrate/io/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    22692 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/quakemigrate/io/event.py
--rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/quakemigrate/io/scanmseed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/quakemigrate/io/triggered_events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:49:27.417152 quakemigrate-1.0.1/quakemigrate/lut/
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/quakemigrate/lut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29700 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/quakemigrate/lut/create_lut.py
--rw-r--r--   0 runner    (1001) docker     (123)    31837 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/quakemigrate/lut/lut.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:49:27.417152 quakemigrate-1.0.1/quakemigrate/plot/
--rwxr-xr-x   0 runner    (1001) docker     (123)      696 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/quakemigrate/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9581 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/quakemigrate/plot/amplitudes.py
--rw-r--r--   0 runner    (1001) docker     (123)    15912 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/quakemigrate/plot/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     9435 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/quakemigrate/plot/phase_picks.py
--rw-r--r--   0 runner    (1001) docker     (123)    20330 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/quakemigrate/plot/trigger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:49:27.417152 quakemigrate-1.0.1/quakemigrate/signal/
--rwxr-xr-x   0 runner    (1001) docker     (123)      609 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/quakemigrate/signal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:49:27.417152 quakemigrate-1.0.1/quakemigrate/signal/local_mag/
--rwxr-xr-x   0 runner    (1001) docker     (123)      762 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/quakemigrate/signal/local_mag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41913 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/quakemigrate/signal/local_mag/amplitude.py
--rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/quakemigrate/signal/local_mag/local_mag.py
--rw-r--r--   0 runner    (1001) docker     (123)    38560 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/quakemigrate/signal/local_mag/magnitude.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:49:27.417152 quakemigrate-1.0.1/quakemigrate/signal/onsets/
--rwxr-xr-x   0 runner    (1001) docker     (123)      541 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/quakemigrate/signal/onsets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/quakemigrate/signal/onsets/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    25729 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/quakemigrate/signal/onsets/stalta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:49:27.421152 quakemigrate-1.0.1/quakemigrate/signal/pickers/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/quakemigrate/signal/pickers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/quakemigrate/signal/pickers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23835 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/quakemigrate/signal/pickers/gaussian.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    43523 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/quakemigrate/signal/scan.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23480 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/quakemigrate/signal/trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)    32627 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/quakemigrate/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:49:27.413152 quakemigrate-1.0.1/quakemigrate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7702 2023-04-10 15:49:27.000000 quakemigrate-1.0.1/quakemigrate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-10 15:49:27.000000 quakemigrate-1.0.1/quakemigrate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 15:49:27.000000 quakemigrate-1.0.1/quakemigrate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-10 15:49:27.000000 quakemigrate-1.0.1/quakemigrate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-10 15:49:27.000000 quakemigrate-1.0.1/quakemigrate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 15:49:27.421152 quakemigrate-1.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     5583 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:49:27.421152 quakemigrate-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7709 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/tests/test_benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-10 15:49:15.000000 quakemigrate-1.0.1/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:35:44.276577 quakemigrate-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-15 23:35:30.000000 quakemigrate-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-15 23:35:30.000000 quakemigrate-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-05-15 23:35:44.276577 quakemigrate-1.0.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6235 2023-05-15 23:35:30.000000 quakemigrate-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:35:44.264577 quakemigrate-1.0.2/quakemigrate/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      775 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/quakemigrate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:35:44.268577 quakemigrate-1.0.2/quakemigrate/core/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      673 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/quakemigrate/core/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4337 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/quakemigrate/core/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/quakemigrate/core/libnames.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:35:44.268577 quakemigrate-1.0.2/quakemigrate/core/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/quakemigrate/core/src/qmlib.def
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/quakemigrate/core/src/qmlib.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3927 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/quakemigrate/core/src/quakemigrate.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:35:44.268577 quakemigrate-1.0.2/quakemigrate/export/
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/quakemigrate/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/quakemigrate/export/to_mfast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/quakemigrate/export/to_nlloc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/quakemigrate/export/to_obspy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/quakemigrate/export/to_snuffler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:35:44.272577 quakemigrate-1.0.2/quakemigrate/io/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1860 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/quakemigrate/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/quakemigrate/io/amplitudes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/quakemigrate/io/availability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/quakemigrate/io/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/quakemigrate/io/cut_waveforms.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30524 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/quakemigrate/io/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22382 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/quakemigrate/io/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12001 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/quakemigrate/io/scanmseed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/quakemigrate/io/triggered_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:35:44.272577 quakemigrate-1.0.2/quakemigrate/lut/
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/quakemigrate/lut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29540 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/quakemigrate/lut/create_lut.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32144 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/quakemigrate/lut/lut.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:35:44.272577 quakemigrate-1.0.2/quakemigrate/plot/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      696 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/quakemigrate/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/quakemigrate/plot/amplitudes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16061 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/quakemigrate/plot/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9941 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/quakemigrate/plot/phase_picks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20505 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/quakemigrate/plot/trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:35:44.272577 quakemigrate-1.0.2/quakemigrate/signal/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      609 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/quakemigrate/signal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:35:44.276577 quakemigrate-1.0.2/quakemigrate/signal/local_mag/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      761 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/quakemigrate/signal/local_mag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41539 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/quakemigrate/signal/local_mag/amplitude.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8861 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/quakemigrate/signal/local_mag/local_mag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38548 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/quakemigrate/signal/local_mag/magnitude.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:35:44.276577 quakemigrate-1.0.2/quakemigrate/signal/onsets/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      541 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/quakemigrate/signal/onsets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/quakemigrate/signal/onsets/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25652 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/quakemigrate/signal/onsets/stalta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:35:44.276577 quakemigrate-1.0.2/quakemigrate/signal/pickers/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/quakemigrate/signal/pickers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/quakemigrate/signal/pickers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23864 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/quakemigrate/signal/pickers/gaussian.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43256 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/quakemigrate/signal/scan.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23537 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/quakemigrate/signal/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31479 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/quakemigrate/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:35:44.268577 quakemigrate-1.0.2/quakemigrate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-05-15 23:35:44.000000 quakemigrate-1.0.2/quakemigrate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-15 23:35:44.000000 quakemigrate-1.0.2/quakemigrate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 23:35:44.000000 quakemigrate-1.0.2/quakemigrate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-15 23:35:44.000000 quakemigrate-1.0.2/quakemigrate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-15 23:35:44.000000 quakemigrate-1.0.2/quakemigrate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 23:35:44.276577 quakemigrate-1.0.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4736 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:35:44.276577 quakemigrate-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7709 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/tests/test_benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-15 23:35:32.000000 quakemigrate-1.0.2/tests/test_util.py
```

### Comparing `quakemigrate-1.0.1/LICENSE` & `quakemigrate-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quakemigrate-1.0.1/PKG-INFO` & `quakemigrate-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quakemigrate
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python package for automatic earthquake detection and location using waveform migration and stacking.
 Author-email: The QuakeMigrate Development Team <quakemigrate.developers@gmail.com>, Tom Winder <tom.winder@esc.cam.ac.uk>, Conor Bacon <cbacon@ldeo.columbia.edu>
 Maintainer-email: Tom Winder <tom.winder@esc.cam.ac.uk>, Conor Bacon <cbacon@ldeo.columbia.edu>
 License: GPLv3
 Project-URL: GitHub, https://github.com/QuakeMigrate/QuakeMigrate
 Project-URL: Issues, https://github.com/QuakeMigrate/QuakeMigrate/issues
 Keywords: seismic event detection,seismic event location,waveform migration,array,seismic,seismology,earthquake,seismic waves,waveform,processing
@@ -68,15 +68,15 @@
 
 <p align="center">
 <img src="https://github.com/QuakeMigrate/QuakeMigrate/raw/master/docs/img/QMlogoBig.png", width="80%">
 </p>
 
 Key Features
 ------------
-QuakeMigrate uses a waveform migration and stacking algorithm to search for coherent seismic phase arrivals across a network of instruments. It produces—from raw data—catalogues of earthquakes with locations, origin times, phase arrival picks, and local magnitude estimates, as well as well as rigorous estimates of the associated uncertainties.
+QuakeMigrate uses a waveform migration and stacking algorithm to search for coherent seismic phase arrivals across a network of instruments. It produces—from raw data—catalogues of earthquakes with locations, origin times, phase arrival picks, and local magnitude estimates, as well as rigorous estimates of the associated uncertainties.
 
 The package has been built with a modular architecture, providing the potential for extension and adaptation at numerous entry points. This includes, but is not limited to:
 * the calculation or import of traveltime grids
 * the choice of algorithm used to identify phase arrivals (for example by kurtosis, cross-covariance analysis between multiple components, machine learning techniques and more)
 * the stacking function used to combine onset functions
 * the algorithm used to perform phase picking
 
@@ -121,24 +121,22 @@
 
 ```console
 Winder, T., Bacon, C.A., Smith, J.D., Hudson, T.S., Drew, J., and White, R.S. QuakeMigrate: a Python Package for Automatic Earthquake Detection and Location Using Waveform Migration and Stacking. (to be submitted to Seismica).
 ```
 
 Contributing to QuakeMigrate
 ----------------------------
-Contributions to QuakeMigrate are welcomed. The first stop should be to reach out, either directly or—preferably—via the GitHub Issues panel, to discuss the proposed changes. Next, simply fork the QuakeMigrate repository, make your changes/add your new contribution, then make a [pull request](https://help.github.com/articles/about-pull-requests/).
+Contributions to QuakeMigrate are welcomed. Whether you have identified a bug or would like to request a new feature, your first stop should be to reach out, either directly or—preferably—via the GitHub Issues panel, to discuss the proposed changes. Once we have had a chance to scope out the proposed changes you can proceed with making your contribution following the instructions in our [contributions guidelines](https://github.com/QuakeMigrate/QuakeMigrate/blob/master/CONTRIBUTING.md).
 
 Bug reports, suggestions for new features and enhancements, and even links to projects that have made use of QuakeMigrate are most welcome.
 
-See our [contributions page](https://github.com/QuakeMigrate/QuakeMigrate/blob/master/CONTRIBUTING.md) for more information.
-
 Contact
 -------
 You can contact us directly at: quakemigrate.developers@gmail.com
 
 Any additional comments/questions can be directed to:
 * **Tom Winder** - tom.winder@esc.cam.ac.uk
 * **Conor Bacon** - conor.bacon@cantab.net
 
 License
 -------
-This package is written and maintained by the QuakeMigrate developers, Copyright QuakeMigrate developers 2023. It is distributed under the GPLv3 License. Please see the [LICENSE](LICENSE) file for a complete description of the rights and freedoms that this provides the user.
+This package is written and maintained by the QuakeMigrate developers, Copyright QuakeMigrate developers 2020–2023. It is distributed under the GPLv3 License. Please see the [LICENSE](LICENSE) file for a complete description of the rights and freedoms that this provides the user.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: quakemigrate Version: 1.0.1 Summary: A Python
+Metadata-Version: 2.1 Name: quakemigrate Version: 1.0.2 Summary: A Python
 package for automatic earthquake detection and location using waveform
 migration and stacking. Author-email: The QuakeMigrate Development Team
 developers@gmail.com>, Tom Winder
 winder@esc.cam.ac.uk>, Conor Bacon
 ldeo.columbia.edu> Maintainer-email: Tom Winder
 winder@esc.cam.ac.uk>, Conor Bacon
 ldeo.columbia.edu> License: GPLv3 Project-URL: GitHub, https://github.com/
@@ -29,39 +29,38 @@
     QuakeMigrate is a Python package for automatic earthquake detection and
                 location using waveform migration and stacking.
                                   width="80%">
 Key Features ------------ QuakeMigrate uses a waveform migration and stacking
 algorithm to search for coherent seismic phase arrivals across a network of
 instruments. It producesâfrom raw dataâcatalogues of earthquakes with
 locations, origin times, phase arrival picks, and local magnitude estimates, as
-well as well as rigorous estimates of the associated uncertainties. The package
-has been built with a modular architecture, providing the potential for
-extension and adaptation at numerous entry points. This includes, but is not
-limited to: * the calculation or import of traveltime grids * the choice of
-algorithm used to identify phase arrivals (for example by kurtosis, cross-
-covariance analysis between multiple components, machine learning techniques
-and more) * the stacking function used to combine onset functions * the
-algorithm used to perform phase picking Documentation ------------
-- Documentation for QuakeMigrate is hosted [here](https://
-quakemigrate.readthedocs.io/en/latest/index.html). Installation -----------
-- Detailed installation instructions can be found [here](https://
-quakemigrate.readthedocs.io/en/latest/installation.html). If you're comfortable
-with virtual environments and just want to get started, QuakeMigrate is
-available via the Python Package Index, and can be installed via pip:
-```console pip install quakemigrate ``` Usage ----- We are working on tutorials
-covering how each individual aspect of the package works, as well as example
-use cases where we provide substantive reasoning for the parameter choices
-used. These examples include applications to cryoseismicity and volcano
-seismology. This is a work in progress - [see our documentation for full
-details](https://quakemigrate.readthedocs.io/en/latest/tutorials.html). ###
-Examples you can run in your browser To quickly get a taste for how the
-software works, try out the two icequake examples hosted on Binder: * Icequakes
-at the Rutford Ice Stream, Antarctica [![badge](https://img.shields.io/badge/
-launch-Icequake%20Rutford%20notebook-579ACA.svg)](https://mybinder.org/v2/gh/
-QuakeMigrate/QuakeMigrate/
+well as rigorous estimates of the associated uncertainties. The package has
+been built with a modular architecture, providing the potential for extension
+and adaptation at numerous entry points. This includes, but is not limited to:
+* the calculation or import of traveltime grids * the choice of algorithm used
+to identify phase arrivals (for example by kurtosis, cross-covariance analysis
+between multiple components, machine learning techniques and more) * the
+stacking function used to combine onset functions * the algorithm used to
+perform phase picking Documentation ------------- Documentation for
+QuakeMigrate is hosted [here](https://quakemigrate.readthedocs.io/en/latest/
+index.html). Installation ------------ Detailed installation instructions can
+be found [here](https://quakemigrate.readthedocs.io/en/latest/
+installation.html). If you're comfortable with virtual environments and just
+want to get started, QuakeMigrate is available via the Python Package Index,
+and can be installed via pip: ```console pip install quakemigrate ``` Usage ---
+-- We are working on tutorials covering how each individual aspect of the
+package works, as well as example use cases where we provide substantive
+reasoning for the parameter choices used. These examples include applications
+to cryoseismicity and volcano seismology. This is a work in progress - [see our
+documentation for full details](https://quakemigrate.readthedocs.io/en/latest/
+tutorials.html). ### Examples you can run in your browser To quickly get a
+taste for how the software works, try out the two icequake examples hosted on
+Binder: * Icequakes at the Rutford Ice Stream, Antarctica [![badge](https://
+img.shields.io/badge/launch-Icequake%20Rutford%20notebook-579ACA.svg)](https://
+mybinder.org/v2/gh/QuakeMigrate/QuakeMigrate/
 master?filepath=examples%2FIcequake_Rutford%2Ficequakes_rutford.ipynb) *
 Icequakes at the SkeiÃ°arÃ¡rjÃ¶kull outlet glacier, Iceland [![badge](https://
 img.shields.io/badge/launch-Icequake%20Iceland%20notebook-E66581.svg)](https://
 mybinder.org/v2/gh/QuakeMigrate/QuakeMigrate/
 master?filepath=examples%2FIcequake_Iceland%2Ficequakes_iceland.ipynb) And for
 a more comprehensive demonstration of the options available, see the [template
 scripts](examples/template_scripts). Citation -------- If you use this package
@@ -71,22 +70,23 @@
 Earthquake Detection and Location. In AGU Fall Meeting 2020. AGU. ``` as well
 as the relevant version of the source code on [Zenodo](https://doi.org/10.5281/
 zenodo.4442749). We hope to have a publication coming out soon: ```console
 Winder, T., Bacon, C.A., Smith, J.D., Hudson, T.S., Drew, J., and White, R.S.
 QuakeMigrate: a Python Package for Automatic Earthquake Detection and Location
 Using Waveform Migration and Stacking. (to be submitted to Seismica). ```
 Contributing to QuakeMigrate ---------------------------- Contributions to
-QuakeMigrate are welcomed. The first stop should be to reach out, either
-directly orâpreferablyâvia the GitHub Issues panel, to discuss the proposed
-changes. Next, simply fork the QuakeMigrate repository, make your changes/add
-your new contribution, then make a [pull request](https://help.github.com/
-articles/about-pull-requests/). Bug reports, suggestions for new features and
-enhancements, and even links to projects that have made use of QuakeMigrate are
-most welcome. See our [contributions page](https://github.com/QuakeMigrate/
-QuakeMigrate/blob/master/CONTRIBUTING.md) for more information. Contact ------
-- You can contact us directly at: quakemigrate.developers@gmail.com Any
-additional comments/questions can be directed to: * **Tom Winder** -
-tom.winder@esc.cam.ac.uk * **Conor Bacon** - conor.bacon@cantab.net License ---
----- This package is written and maintained by the QuakeMigrate developers,
-Copyright QuakeMigrate developers 2023. It is distributed under the GPLv3
-License. Please see the [LICENSE](LICENSE) file for a complete description of
-the rights and freedoms that this provides the user.
+QuakeMigrate are welcomed. Whether you have identified a bug or would like to
+request a new feature, your first stop should be to reach out, either directly
+orâpreferablyâvia the GitHub Issues panel, to discuss the proposed changes.
+Once we have had a chance to scope out the proposed changes you can proceed
+with making your contribution following the instructions in our [contributions
+guidelines](https://github.com/QuakeMigrate/QuakeMigrate/blob/master/
+CONTRIBUTING.md). Bug reports, suggestions for new features and enhancements,
+and even links to projects that have made use of QuakeMigrate are most welcome.
+Contact ------- You can contact us directly at:
+quakemigrate.developers@gmail.com Any additional comments/questions can be
+directed to: * **Tom Winder** - tom.winder@esc.cam.ac.uk * **Conor Bacon** -
+conor.bacon@cantab.net License ------- This package is written and maintained
+by the QuakeMigrate developers, Copyright QuakeMigrate developers 2020â2023.
+It is distributed under the GPLv3 License. Please see the [LICENSE](LICENSE)
+file for a complete description of the rights and freedoms that this provides
+the user.
```

### Comparing `quakemigrate-1.0.1/README.md` & `quakemigrate-1.0.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 <p align="center">
 <img src="https://github.com/QuakeMigrate/QuakeMigrate/raw/master/docs/img/QMlogoBig.png", width="80%">
 </p>
 
 Key Features
 ------------
-QuakeMigrate uses a waveform migration and stacking algorithm to search for coherent seismic phase arrivals across a network of instruments. It produces—from raw data—catalogues of earthquakes with locations, origin times, phase arrival picks, and local magnitude estimates, as well as well as rigorous estimates of the associated uncertainties.
+QuakeMigrate uses a waveform migration and stacking algorithm to search for coherent seismic phase arrivals across a network of instruments. It produces—from raw data—catalogues of earthquakes with locations, origin times, phase arrival picks, and local magnitude estimates, as well as rigorous estimates of the associated uncertainties.
 
 The package has been built with a modular architecture, providing the potential for extension and adaptation at numerous entry points. This includes, but is not limited to:
 * the calculation or import of traveltime grids
 * the choice of algorithm used to identify phase arrivals (for example by kurtosis, cross-covariance analysis between multiple components, machine learning techniques and more)
 * the stacking function used to combine onset functions
 * the algorithm used to perform phase picking
 
@@ -92,24 +92,22 @@
 
 ```console
 Winder, T., Bacon, C.A., Smith, J.D., Hudson, T.S., Drew, J., and White, R.S. QuakeMigrate: a Python Package for Automatic Earthquake Detection and Location Using Waveform Migration and Stacking. (to be submitted to Seismica).
 ```
 
 Contributing to QuakeMigrate
 ----------------------------
-Contributions to QuakeMigrate are welcomed. The first stop should be to reach out, either directly or—preferably—via the GitHub Issues panel, to discuss the proposed changes. Next, simply fork the QuakeMigrate repository, make your changes/add your new contribution, then make a [pull request](https://help.github.com/articles/about-pull-requests/).
+Contributions to QuakeMigrate are welcomed. Whether you have identified a bug or would like to request a new feature, your first stop should be to reach out, either directly or—preferably—via the GitHub Issues panel, to discuss the proposed changes. Once we have had a chance to scope out the proposed changes you can proceed with making your contribution following the instructions in our [contributions guidelines](https://github.com/QuakeMigrate/QuakeMigrate/blob/master/CONTRIBUTING.md).
 
 Bug reports, suggestions for new features and enhancements, and even links to projects that have made use of QuakeMigrate are most welcome.
 
-See our [contributions page](https://github.com/QuakeMigrate/QuakeMigrate/blob/master/CONTRIBUTING.md) for more information.
-
 Contact
 -------
 You can contact us directly at: quakemigrate.developers@gmail.com
 
 Any additional comments/questions can be directed to:
 * **Tom Winder** - tom.winder@esc.cam.ac.uk
 * **Conor Bacon** - conor.bacon@cantab.net
 
 License
 -------
-This package is written and maintained by the QuakeMigrate developers, Copyright QuakeMigrate developers 2023. It is distributed under the GPLv3 License. Please see the [LICENSE](LICENSE) file for a complete description of the rights and freedoms that this provides the user.
+This package is written and maintained by the QuakeMigrate developers, Copyright QuakeMigrate developers 2020–2023. It is distributed under the GPLv3 License. Please see the [LICENSE](LICENSE) file for a complete description of the rights and freedoms that this provides the user.
```

#### html2text {}

```diff
@@ -7,39 +7,38 @@
     QuakeMigrate is a Python package for automatic earthquake detection and
                 location using waveform migration and stacking.
                                   width="80%">
 Key Features ------------ QuakeMigrate uses a waveform migration and stacking
 algorithm to search for coherent seismic phase arrivals across a network of
 instruments. It producesâfrom raw dataâcatalogues of earthquakes with
 locations, origin times, phase arrival picks, and local magnitude estimates, as
-well as well as rigorous estimates of the associated uncertainties. The package
-has been built with a modular architecture, providing the potential for
-extension and adaptation at numerous entry points. This includes, but is not
-limited to: * the calculation or import of traveltime grids * the choice of
-algorithm used to identify phase arrivals (for example by kurtosis, cross-
-covariance analysis between multiple components, machine learning techniques
-and more) * the stacking function used to combine onset functions * the
-algorithm used to perform phase picking Documentation ------------
-- Documentation for QuakeMigrate is hosted [here](https://
-quakemigrate.readthedocs.io/en/latest/index.html). Installation -----------
-- Detailed installation instructions can be found [here](https://
-quakemigrate.readthedocs.io/en/latest/installation.html). If you're comfortable
-with virtual environments and just want to get started, QuakeMigrate is
-available via the Python Package Index, and can be installed via pip:
-```console pip install quakemigrate ``` Usage ----- We are working on tutorials
-covering how each individual aspect of the package works, as well as example
-use cases where we provide substantive reasoning for the parameter choices
-used. These examples include applications to cryoseismicity and volcano
-seismology. This is a work in progress - [see our documentation for full
-details](https://quakemigrate.readthedocs.io/en/latest/tutorials.html). ###
-Examples you can run in your browser To quickly get a taste for how the
-software works, try out the two icequake examples hosted on Binder: * Icequakes
-at the Rutford Ice Stream, Antarctica [![badge](https://img.shields.io/badge/
-launch-Icequake%20Rutford%20notebook-579ACA.svg)](https://mybinder.org/v2/gh/
-QuakeMigrate/QuakeMigrate/
+well as rigorous estimates of the associated uncertainties. The package has
+been built with a modular architecture, providing the potential for extension
+and adaptation at numerous entry points. This includes, but is not limited to:
+* the calculation or import of traveltime grids * the choice of algorithm used
+to identify phase arrivals (for example by kurtosis, cross-covariance analysis
+between multiple components, machine learning techniques and more) * the
+stacking function used to combine onset functions * the algorithm used to
+perform phase picking Documentation ------------- Documentation for
+QuakeMigrate is hosted [here](https://quakemigrate.readthedocs.io/en/latest/
+index.html). Installation ------------ Detailed installation instructions can
+be found [here](https://quakemigrate.readthedocs.io/en/latest/
+installation.html). If you're comfortable with virtual environments and just
+want to get started, QuakeMigrate is available via the Python Package Index,
+and can be installed via pip: ```console pip install quakemigrate ``` Usage ---
+-- We are working on tutorials covering how each individual aspect of the
+package works, as well as example use cases where we provide substantive
+reasoning for the parameter choices used. These examples include applications
+to cryoseismicity and volcano seismology. This is a work in progress - [see our
+documentation for full details](https://quakemigrate.readthedocs.io/en/latest/
+tutorials.html). ### Examples you can run in your browser To quickly get a
+taste for how the software works, try out the two icequake examples hosted on
+Binder: * Icequakes at the Rutford Ice Stream, Antarctica [![badge](https://
+img.shields.io/badge/launch-Icequake%20Rutford%20notebook-579ACA.svg)](https://
+mybinder.org/v2/gh/QuakeMigrate/QuakeMigrate/
 master?filepath=examples%2FIcequake_Rutford%2Ficequakes_rutford.ipynb) *
 Icequakes at the SkeiÃ°arÃ¡rjÃ¶kull outlet glacier, Iceland [![badge](https://
 img.shields.io/badge/launch-Icequake%20Iceland%20notebook-E66581.svg)](https://
 mybinder.org/v2/gh/QuakeMigrate/QuakeMigrate/
 master?filepath=examples%2FIcequake_Iceland%2Ficequakes_iceland.ipynb) And for
 a more comprehensive demonstration of the options available, see the [template
 scripts](examples/template_scripts). Citation -------- If you use this package
@@ -49,22 +48,23 @@
 Earthquake Detection and Location. In AGU Fall Meeting 2020. AGU. ``` as well
 as the relevant version of the source code on [Zenodo](https://doi.org/10.5281/
 zenodo.4442749). We hope to have a publication coming out soon: ```console
 Winder, T., Bacon, C.A., Smith, J.D., Hudson, T.S., Drew, J., and White, R.S.
 QuakeMigrate: a Python Package for Automatic Earthquake Detection and Location
 Using Waveform Migration and Stacking. (to be submitted to Seismica). ```
 Contributing to QuakeMigrate ---------------------------- Contributions to
-QuakeMigrate are welcomed. The first stop should be to reach out, either
-directly orâpreferablyâvia the GitHub Issues panel, to discuss the proposed
-changes. Next, simply fork the QuakeMigrate repository, make your changes/add
-your new contribution, then make a [pull request](https://help.github.com/
-articles/about-pull-requests/). Bug reports, suggestions for new features and
-enhancements, and even links to projects that have made use of QuakeMigrate are
-most welcome. See our [contributions page](https://github.com/QuakeMigrate/
-QuakeMigrate/blob/master/CONTRIBUTING.md) for more information. Contact ------
-- You can contact us directly at: quakemigrate.developers@gmail.com Any
-additional comments/questions can be directed to: * **Tom Winder** -
-tom.winder@esc.cam.ac.uk * **Conor Bacon** - conor.bacon@cantab.net License ---
----- This package is written and maintained by the QuakeMigrate developers,
-Copyright QuakeMigrate developers 2023. It is distributed under the GPLv3
-License. Please see the [LICENSE](LICENSE) file for a complete description of
-the rights and freedoms that this provides the user.
+QuakeMigrate are welcomed. Whether you have identified a bug or would like to
+request a new feature, your first stop should be to reach out, either directly
+orâpreferablyâvia the GitHub Issues panel, to discuss the proposed changes.
+Once we have had a chance to scope out the proposed changes you can proceed
+with making your contribution following the instructions in our [contributions
+guidelines](https://github.com/QuakeMigrate/QuakeMigrate/blob/master/
+CONTRIBUTING.md). Bug reports, suggestions for new features and enhancements,
+and even links to projects that have made use of QuakeMigrate are most welcome.
+Contact ------- You can contact us directly at:
+quakemigrate.developers@gmail.com Any additional comments/questions can be
+directed to: * **Tom Winder** - tom.winder@esc.cam.ac.uk * **Conor Bacon** -
+conor.bacon@cantab.net License ------- This package is written and maintained
+by the QuakeMigrate developers, Copyright QuakeMigrate developers 2020â2023.
+It is distributed under the GPLv3 License. Please see the [LICENSE](LICENSE)
+file for a complete description of the rights and freedoms that this provides
+the user.
```

### Comparing `quakemigrate-1.0.1/pyproject.toml` & `quakemigrate-1.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ]
 
 [tool.setuptools.packages.find]
 include = ["quakemigrate*"]
 
 [project]
 name = "quakemigrate"
-version = "1.0.1"
+version = "1.0.2"
 description = "A Python package for automatic earthquake detection and location using waveform migration and stacking."
 readme = "README.md"
 license = {text = "GPLv3"}
 requires-python = ">=3.8"
 authors = [
     {name = "The QuakeMigrate Development Team", email = "quakemigrate.developers@gmail.com"},
     {name = "Tom Winder", email = "tom.winder@esc.cam.ac.uk"},
@@ -64,18 +64,17 @@
     "obspy>=1.3",
     "pandas",
     "pyproj>=2.5",
     "scipy",
 ]
 
 [project.optional-dependencies]
-dev = ["black", "ipython"]
+dev = ["black", "ipython", "pre-commit", "ruff", "coverage"]
 docs = ["docutils<0.17", "mock", "Sphinx >= 4.3.0", "sphinx_rtd_theme>=0.5.1"]
 fmm = ["scikit-fmm"]
 
 [project.urls]
 GitHub = "https://github.com/QuakeMigrate/QuakeMigrate"
 Issues = "https://github.com/QuakeMigrate/QuakeMigrate/issues"
 
 [tool.black]
 line-length = 88
-
```

### Comparing `quakemigrate-1.0.1/quakemigrate/__init__.py` & `quakemigrate-1.0.2/quakemigrate/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 QuakeMigrate - a Python package for automatic earthquake detection and location
 using waveform migration and stacking.
 
 :copyright:
-    2020-2022, QuakeMigrate developers.
+    2020–2023, QuakeMigrate developers.
 :license:
     GNU General Public License, Version 3
     (https://www.gnu.org/licenses/gpl-3.0.html)
 
 """
 
 import pkg_resources
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quakemigrate-1.0.1/quakemigrate/core/__init__.py` & `quakemigrate-1.0.2/quakemigrate/core/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     * Migrate onsets - This routine performs the continuous migration through \
     time and space of the onset functions. It has been parallelised with \
     openMP.
     * Find maximum coalescence - This routine finds the continuous maximum \
     coalescence amplitude in the 4-D coalesence volume.
 
 :copyright:
-    2020 - 2021, QuakeMigrate developers.
+    2020–2023, QuakeMigrate developers.
 :license:
     GNU General Public License, Version 3
     (https://www.gnu.org/licenses/gpl-3.0.html)
 
 """
 
 from .lib import migrate, find_max_coa  # NOQA
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quakemigrate-1.0.1/quakemigrate/core/lib.py` & `quakemigrate-1.0.2/quakemigrate/core/lib.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 Bindings for the C library functions, migrate and find_max_coa.
 
 :copyright:
-    2020 - 2021, QuakeMigrate developers.
+    2020–2023, QuakeMigrate developers.
 :license:
     GNU General Public License, Version 3
     (https://www.gnu.org/licenses/gpl-3.0.html)
 
 """
 
 import numpy as np
@@ -22,30 +22,40 @@
 c_int32 = clib.ctypes.c_int32
 c_int64 = clib.ctypes.c_int64
 c_dPt = clib.ndpointer(dtype=np.float64, flags="C_CONTIGUOUS")
 c_i32Pt = clib.ndpointer(dtype=np.int32, flags="C_CONTIGUOUS")
 c_i64Pt = clib.ndpointer(dtype=np.int64, flags="C_CONTIGUOUS")
 
 
-qmlib.migrate.argtypes = [c_dPt, c_i32Pt, c_dPt, c_int32, c_int32, c_int32,
-                          c_int32, c_int32, c_int64, c_int64]
+qmlib.migrate.argtypes = [
+    c_dPt,
+    c_i32Pt,
+    c_dPt,
+    c_int32,
+    c_int32,
+    c_int32,
+    c_int32,
+    c_int32,
+    c_int64,
+    c_int64,
+]
 
 
 @util.timeit()
 def migrate(onsets, traveltimes, first_idx, last_idx, available, threads):
     """
     Computes 4-D coalescence map by migrating seismic phase onset functions.
 
     Parameters
     ----------
     onsets : `numpy.ndarry` of float
         Onset functions for each seismic phase, shape(nonsets, nsamples).
     traveltimes : `numpy.ndarry` of int
-        Grids of seismic phase traveltimes, converted to an integer multiple of
-        the sampling rate, shape(nx, ny, nz, nonsets).
+        Grids of seismic phase traveltimes, converted to an integer multiple of the
+        sampling rate, shape(nx, ny, nz, nonsets).
     first_idx : int
         Index of first sample in array from which to scan.
     last_idx : int
         Index of last sample in array up to which to scan.
     available : int
         Number of available onset functions.
     threads : int
@@ -55,74 +65,89 @@
     -------
     map4d : `numpy.ndarray` of `numpy.double`
         4-D coalescence map, shape(nx, ny, nz, nsamples).
 
     Raises
     ------
     ValueError
-        If mismatch between number of onset functions and traveltime lookup
-        tables - expect both to be equal to the no. stations * no. phases.
+        If mismatch between number of onset functions and traveltime lookup tables.
+        Expect both to be equal to the no. stations * no. phases.
     ValueError
-        If the number of samples in the onset functions is less than the number
-        of samples  array is smaller than map4d[0, 0, 0, :].
+        If the number of samples in the onset functions is less than the number of
+        samples array is smaller than map4d[0, 0, 0, :].
 
     """
 
     *grid_dimensions, n_luts = traveltimes.shape
     n_onsets, t_samples = onsets.shape
     n_samples = t_samples - first_idx - last_idx
     map4d = np.zeros(tuple(grid_dimensions) + (n_samples,), dtype=np.float64)
     n_nodes = np.prod(grid_dimensions)
 
     if not n_luts == n_onsets:
-        raise ValueError("Mismatch between number of stations for data and "
-                         f"LUT, {n_onsets} - {n_luts}")
+        raise ValueError(
+            f"Mismatch between number of stations for data and LUT, {n_onsets}:{n_luts}"
+        )
     if onsets.size < n_samples + first_idx:
         raise ValueError("Data array smaller than coalescence array.")
 
-    qmlib.migrate(onsets, traveltimes, map4d, c_int32(first_idx),
-                  c_int32(last_idx), c_int32(n_samples), c_int32(n_onsets),
-                  c_int32(available), c_int64(n_nodes), c_int64(threads))
+    qmlib.migrate(
+        onsets,
+        traveltimes,
+        map4d,
+        c_int32(first_idx),
+        c_int32(last_idx),
+        c_int32(n_samples),
+        c_int32(n_onsets),
+        c_int32(available),
+        c_int64(n_nodes),
+        c_int64(threads),
+    )
 
     return map4d
 
 
-qmlib.find_max_coa.argtypes = [c_dPt, c_dPt, c_dPt, c_i64Pt, c_int32, c_int64,
-                               c_int64]
+qmlib.find_max_coa.argtypes = [c_dPt, c_dPt, c_dPt, c_i64Pt, c_int32, c_int64, c_int64]
 
 
 @util.timeit()
 def find_max_coa(map4d, threads):
     """
-    Finds time series of the maximum coalescence/normalised coalescence in the
-    3-D volume, and the corresponding grid indices.
+    Finds time series of the maximum coalescence/normalised coalescence in the 3-D
+    volume, and the corresponding grid indices.
 
     Parameters
     ----------
     map4d : `numpy.ndarray` of `numpy.double`
         4-D coalescence map, shape(nx, ny, nz, nsamples).
     threads : int
         Number of threads with which to perform the scan.
 
     Returns
     -------
     max_coa : `numpy.ndarray` of `numpy.double`
         Time series of the maximum coalescence value in the 3-D volume.
     max_norm_coa : `numpy.ndarray` of `numpy.double`
-        Times series of the maximum normalised coalescence value in the 3-D
-        volume.
+        Times series of the maximum normalised coalescence value in the 3-D volume.
     max_coa_idx : `numpy.ndarray` of int
         Time series of the flattened grid indices corresponding to the maximum
         coalescence value in the 3-D volume.
 
     """
 
     *grid_dimensions, n_samples = map4d.shape
     n_nodes = np.prod(grid_dimensions)
     max_coa = np.zeros(n_samples, dtype=np.double)
     max_norm_coa = np.zeros(n_samples, dtype=np.double)
     max_coa_idx = np.zeros(n_samples, dtype=np.int64)
 
-    qmlib.find_max_coa(map4d, max_coa, max_norm_coa, max_coa_idx,
-                       c_int32(n_samples), c_int64(n_nodes), c_int64(threads))
+    qmlib.find_max_coa(
+        map4d,
+        max_coa,
+        max_norm_coa,
+        max_coa_idx,
+        c_int32(n_samples),
+        c_int64(n_nodes),
+        c_int64(threads),
+    )
 
     return max_coa, max_norm_coa, max_coa_idx
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quakemigrate-1.0.1/quakemigrate/core/libnames.py` & `quakemigrate-1.0.2/quakemigrate/core/libnames.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 # -*- coding: utf-8 -*-
 """
 Helper to load compiled C library.
 
 :copyright:
-    2020 - 2021, QuakeMigrate developers.
+    2020–2023, QuakeMigrate developers.
 :license:
     GNU General Public License, Version 3
     (https://www.gnu.org/licenses/gpl-3.0.html)
 
 """
 
 import ctypes
 from distutils import sysconfig
 import pathlib
 
 
 def _load_cdll(name):
     """
-    Helper function to load an extension built using setuptools/distutils
-    Extension.
+    Helper function to load an extension built using setuptools Extension.
 
     Parameters
     ----------
     name : str
         Name of library to load.
 
     Returns
     -------
-    `ctypes.CDLL`
+    cdll : `ctypes.CDLL`
         Shared library object.
 
     """
 
-    # our custom defined part of the extension file name
+    # Our custom defined part of the extension file name
     libpath = pathlib.Path(__file__).parent / "src" / name
     lib = libpath.with_suffix(sysconfig.get_config_var("EXT_SUFFIX"))
     try:
         cdll = ctypes.CDLL(str(lib))
     except Exception as e:
-        msg = (f"Could not load extension library '{libpath.name}'.\n\n{e}\n\n"
-               "If you have chosen to install from a clone of the github "
-               "repository, please ensure you have run 'python setup.py install', which will "
-               "compile and install the C library. See the installation documentation for more details.")
-        raise ImportError(msg)
+        raise ImportError(
+            f"Could not load extension library '{libpath.name}'.\n\n{e}\n\nIf you have "
+            "chosen to install from a clone of the github repository, please ensure "
+            "you have run 'python setup.py install', which will compile and install "
+            "the C library. See the installation documentation for more details."
+        )
 
     return cdll
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quakemigrate-1.0.1/quakemigrate/core/src/qmlib.h` & `quakemigrate-1.0.2/quakemigrate/core/src/qmlib.h`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
  * =============================================================================
  *
  *       Filename:  qmlib.h
  *
  *        Purpose:  Header file to bring together definitions used in the
  *                  quakemigrate.c library.
  *
- *      Copyright:  2020 - 2021, QuakeMigrate developers.
+ *      Copyright:  2020-2023, QuakeMigrate developers.
  *        License:  GNU General Public License, Version 3
  *                  (https://www.gnu.org/licenses/gpl-3.0.html)
  *
  * =============================================================================
  */
 
 #include <stdint.h>
```

### Comparing `quakemigrate-1.0.1/quakemigrate/core/src/quakemigrate.c` & `quakemigrate-1.0.2/quakemigrate/core/src/quakemigrate.c`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
  * =============================================================================
  *
  *       Filename:  quakemigrate.c
  *
  *        Purpose:  Routines for computing the 4-D coalescence function and
  *                  determining the maximum values.
  *
- *      Copyright:  2020 - 2021, QuakeMigrate developers.
+ *      Copyright:  2020-2023, QuakeMigrate developers.
  *        License:  GNU General Public License, Version 3
  *                  (https://www.gnu.org/licenses/gpl-3.0.html)
  *
  * =============================================================================
  */
 
 #include "qmlib.h"
```

### Comparing `quakemigrate-1.0.1/quakemigrate/export/__init__.py` & `quakemigrate-1.0.2/quakemigrate/export/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # -*- coding: utf-8 -*-
 """
-The :mod:`quakemigrate.export` module provides some utility functions to export
-the outputs of QuakeMigrate to other catalogue formats/software inputs:
+The :mod:`quakemigrate.export` module provides some utility functions to export the
+outputs of QuakeMigrate to other catalogue formats/software inputs:
 
     * Input files for NonLinLoc
     * ObsPy Catalog object
     * Snuffler pick/event files for manual phase picking
     * MFAST for shear-wave splitting analysis
 
 .. warning:: Export modules are an ongoing work in progress. The functionality\
  of the core module `to_obspy` has been validated, but there may still be bugs\
  elsewhere. If you are interested in using these, or wish to add additional \
 functionality, please contact the QuakeMigrate developers at: \
 quakemigrate.developers@gmail.com .
 
 :copyright:
-    2020 - 2021, QuakeMigrate developers.
+    2020–2023, QuakeMigrate developers.
 :license:
     GNU General Public License, Version 3
     (https://www.gnu.org/licenses/gpl-3.0.html)
 
 """
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quakemigrate-1.0.1/quakemigrate/export/to_mfast.py` & `quakemigrate-1.0.2/quakemigrate/export/to_mfast.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """
-This module provides parsers to generate SAC waveform files from an ObsPy
-Catalog, with headers correctly populated for MFAST.
+This module provides parsers to generate SAC waveform files from an ObsPy Catalog, with
+headers correctly populated for MFAST.
 
 :copyright:
-    2020 - 2021, QuakeMigrate developers.
+    2020–2023, QuakeMigrate developers.
 :license:
     GNU General Public License, Version 3
     (https://www.gnu.org/licenses/gpl-3.0.html)
 
 """
 
 import pathlib
@@ -25,16 +25,15 @@
 def sac_mfast(event, stations, output_path, units, filename=None):
     """
     Function to create the SAC file.
 
     Parameters
     ----------
     event : `ObsPy.Event` object
-        Contains information about the origin time and a list of associated
-        picks.
+        Contains information about the origin time and a list of associated picks.
     stations : `pandas.DataFrame` object
         DataFrame containing station information.
     output_path : str
         Location to save the SAC file.
     units : {"km", "m"}
         Grid projection coordinates for QM LUT (determines units of depths and
         uncertainties in the .event files).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quakemigrate-1.0.1/quakemigrate/export/to_nlloc.py` & `quakemigrate-1.0.2/quakemigrate/export/to_nlloc.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 """
-This module provides parsers to export an ObsPy Catalog to the NonLinLoc input
-file format. We prefer this to the one offered by ObsPy as it includes the
-additional weighting term.
+This module provides parsers to export an ObsPy Catalog to the NonLinLoc input file
+format. We prefer this to the one offered by ObsPy as it includes the additional
+weighting term.
 
 :copyright:
-    2020 - 2021, QuakeMigrate developers.
+    2020–2023, QuakeMigrate developers.
 :license:
     GNU General Public License, Version 3
     (https://www.gnu.org/licenses/gpl-3.0.html)
 
 """
 
 import warnings
@@ -30,34 +30,37 @@
     Parameters
     ----------
     event : `obspy.Event` object
         Contains information on a single event.
     filename : str
         Name of NonLinLoc phase file.
     autopick : bool, optional
-        Whether to read the autopicks or the modelled arrival times. Default:
-        True (use autopicks).
+        Whether to read the autopicks or the modelled arrival times.
+        Default: True (use autopicks).
 
     """
 
     info = []
 
     if autopick:
         method = "autopick"
     else:
         method = "modelled"
 
     if not isinstance(event, Event):
-        msg = ("Writing NonLinLoc Phase file is only supported for a single "
-               " Event at a time. Use a for loop over the catalog and "
-               "provide an output file name for each event).")
-        raise ValueError(msg)
-
-    fmt = ("{:s} {:s} {:s} {:s} {:s} {:s} {:s} {:s} " +
-           "{:7.4f} GAU {:9.2e} {:9.2e} {:9.2e} {:9.2e} {:9.2e}")
+        raise ValueError(
+            "Writing NonLinLoc Phase file is only supported for a single Event at a "
+            "time. Use a for loop over the catalog and provide an output file name for "
+            "each event)."
+        )
+
+    fmt = (
+        "{:s} {:s} {:s} {:s} {:s} {:s} {:s} {:s} "
+        "{:7.4f} GAU {:9.2e} {:9.2e} {:9.2e} {:9.2e} {:9.2e}"
+    )
 
     for pick in event.picks:
         if pick.method_id != method:
             continue
         wid = pick.waveform_id
         station = wid.station_code or "?"
         component = wid.channel_code and wid.channel_code[-1].upper() or "?"
@@ -68,25 +71,38 @@
         polarity = POLARITIES_REVERSE.get(pick.polarity, "?")
         date = pick.time.strftime("%Y%m%d")
         hourminute = pick.time.strftime("%H%M")
         seconds = pick.time.second + pick.time.microsecond * 1e-6
         time_error = pick.time_errors.uncertainty or -1
         if time_error == -1:
             try:
-                time_error = (pick.time_errors.upper_uncertainty +
-                              pick.time_errors.lower_uncertainty) / 2.0
+                time_error = (
+                    pick.time_errors.upper_uncertainty
+                    + pick.time_errors.lower_uncertainty
+                ) / 2.0
             except Exception:
                 pass
-        info_ = fmt.format(station.ljust(6), "?".ljust(4), component.ljust(4),
-                           onset.ljust(1), phase_type.ljust(6),
-                           polarity.ljust(1), date, hourminute, seconds,
-                           time_error, -1, -1, -1, 1)
+        info_ = fmt.format(
+            station.ljust(6),
+            "?".ljust(4),
+            component.ljust(4),
+            onset.ljust(1),
+            phase_type.ljust(6),
+            polarity.ljust(1),
+            date,
+            hourminute,
+            seconds,
+            time_error,
+            -1,
+            -1,
+            -1,
+            1,
+        )
         info.append(info_)
 
     if info:
         info = "\n".join(sorted(info) + [""])
     else:
-        msg = "No pick information, writing empty NLLOC OBS file."
-        warnings.warn(msg)
+        warnings.warn("No pick information, writing empty NLLOC OBS file.")
     with open(filename, "w") as fh:
         for line in info:
             fh.write(line)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quakemigrate-1.0.1/quakemigrate/export/to_obspy.py` & `quakemigrate-1.0.2/quakemigrate/export/to_obspy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,60 +1,69 @@
 # -*- coding: utf-8 -*-
 """
-This module provides parsers to export the output of a QuakeMigrate run to an
-ObsPy Catalog.
+This module provides parsers to export the output of a QuakeMigrate run to an ObsPy
+Catalog.
 
 :copyright:
-    2020 - 2021, QuakeMigrate developers.
+    2020–2023, QuakeMigrate developers.
 :license:
     GNU General Public License, Version 3
     (https://www.gnu.org/licenses/gpl-3.0.html)
 
 """
 
 from itertools import chain
 import pathlib
 
 import pandas as pd
 
 from obspy import Catalog, UTCDateTime, __version__
 from obspy.core import AttribDict
-from obspy.core.event import (Event, Origin, OriginUncertainty,
-                              ConfidenceEllipsoid, Pick, TimeWindow,
-                              WaveformStreamID, CreationInfo,
-                              Amplitude, StationMagnitude, Magnitude)
+from obspy.core.event import (
+    Event,
+    Origin,
+    OriginUncertainty,
+    ConfidenceEllipsoid,
+    Pick,
+    TimeWindow,
+    WaveformStreamID,
+    CreationInfo,
+    Amplitude,
+    StationMagnitude,
+    Magnitude,
+)
 from obspy.geodetics import kilometer2degrees
 
 import quakemigrate
 
 
 ns = "http://quakemigrate.github.io/xmlns/event"
 
 
 def read_quakemigrate(run_dir, units, run_subname="", local_mag_ph="S"):
     """
     Reads the .event and .picks outputs, and .amps outputs if available, from a
     QuakeMigrate run into an obspy Catalog object.
 
-    NOTE: if a station_corrections dict was used to calculate the
-    network-averaged local magnitude, this information will not be included in
-    the obspy event object. There might therefore be a discrepancy between the
-    mean of the StationMagnitudes and the event magnitude.
+    NOTE: if a station_corrections dict was used to calculate the network-averaged local
+    magnitude, this information will not be included in the ObsPy event object. There
+    might therefore be a discrepancy between the mean of the StationMagnitudes and the
+    event magnitude.
 
     Parameters
     ----------
     run_dir : str
         Path to QuakeMigrate run directory.
     units : {"km", "m"}
         Grid projection coordinates for QM LUT (determines units of depths and
         uncertainties in the .event files).
     run_subname : str, optional
         Run_subname string (if applicable).
     local_mag_ph : {"S", "P"}, optional
-        Amplitude measurement used to calculate local magnitudes. (Default "S")
+        Amplitude measurement used to calculate local magnitudes. (Default "S").
 
     Returns
     -------
     cat : `obspy.Catalog` object
         Catalog containing events in the specified QuakeMigrate run directory.
 
     """
@@ -76,15 +85,15 @@
         event = _read_single_event(eventf, locate_dir, units, local_mag_ph)
         if event is None:
             continue
         else:
             cat.append(event)
 
     cat.creation_info.creation_time = UTCDateTime()
-    cat.creation_info.version = "ObsPy %s" % __version__
+    cat.creation_info.version = f"ObsPy {__version__}"
 
     return cat
 
 
 def _read_single_event(event_file, locate_dir, units, local_mag_ph):
     """
     Parse an event file from QuakeMigrate into an obspy Event object.
@@ -101,16 +110,16 @@
     local_mag_ph : {"S", "P"}
         Amplitude measurement used to calculate local magnitudes.
 
     Returns
     -------
     event : `obspy.Event` object
         Event object populated with all available information output by
-        :class:`~quakemigrate.signal.scan.locate()`, including event locations
-        and uncertainties, picks, and amplitudes and magnitudes if available.
+        :class:`~quakemigrate.signal.scan.locate()`, including event locations and
+        uncertainties, picks, and amplitudes and magnitudes if available.
 
     """
 
     # Parse information from event file
     event_info = pd.read_csv(event_file).iloc[0]
     event_uid = str(event_info["EventID"])
 
@@ -122,45 +131,44 @@
     else:
         raise AttributeError(f"units must be 'km' or 'm'; not {units}")
 
     # Create event object to store origin and pick information
     event = Event()
     event.extra = AttribDict()
     event.resource_id = str(event_info["EventID"])
-    event.creation_info = CreationInfo(author="QuakeMigrate",
-                                       version=quakemigrate.__version__)
+    event.creation_info = CreationInfo(
+        author="QuakeMigrate", version=quakemigrate.__version__
+    )
 
     # Add COA info to extra
-    event.extra.coa = {"value": event_info["COA"],
-                       "namespace": ns}
-    event.extra.coa_norm = {"value": event_info["COA_NORM"],
-                            "namespace": ns}
-    event.extra.trig_coa = {"value": event_info["TRIG_COA"],
-                            "namespace": ns}
-    event.extra.dec_coa = {"value": event_info["DEC_COA"],
-                           "namespace": ns}
-    event.extra.dec_coa_norm = {"value": event_info["DEC_COA_NORM"],
-                                "namespace": ns}
+    event.extra.coa = {"value": event_info["COA"], "namespace": ns}
+    event.extra.coa_norm = {"value": event_info["COA_NORM"], "namespace": ns}
+    event.extra.trig_coa = {"value": event_info["TRIG_COA"], "namespace": ns}
+    event.extra.dec_coa = {"value": event_info["DEC_COA"], "namespace": ns}
+    event.extra.dec_coa_norm = {"value": event_info["DEC_COA_NORM"], "namespace": ns}
 
     # Determine location of cut waveform data - add to event object as a
     # custom extra attribute.
     mseed = locate_dir / "raw_cut_waveforms" / event_uid
     event.extra.cut_waveforms_file = {
         "value": str(mseed.with_suffix(".m").resolve()),
-        "namespace": ns}
+        "namespace": ns,
+    }
     if (locate_dir / "real_cut_waveforms").exists():
         mseed = locate_dir / "real_cut_waveforms" / event_uid
         event.extra.real_cut_waveforms_file = {
             "value": str(mseed.with_suffix(".m").resolve()),
-            "namespace": ns}
+            "namespace": ns,
+        }
     if (locate_dir / "wa_cut_waveforms").exists():
         mseed = locate_dir / "wa_cut_waveforms" / event_uid
         event.extra.wa_cut_waveforms_file = {
             "value": str(mseed.with_suffix(".m").resolve()),
-            "namespace": ns}
+            "namespace": ns,
+        }
 
     # Create origin with spline location and set to preferred event origin.
     origin = Origin()
     origin.method_id = "spline"
     origin.longitude = event_info["X"]
     origin.latitude = event_info["Y"]
     origin.depth = event_info["Z"] * factor
@@ -187,17 +195,19 @@
     ce.major_axis_rotation = 0
     ouc.confidence_ellipsoid = ce
     ouc.preferred_description = "confidence ellipsoid"
 
     # Set uncertainties for both as the gaussian uncertainties
     for origin in event.origins:
         origin.longitude_errors.uncertainty = kilometer2degrees(
-            event_info["GAU_ErrX"] * factor / 1e3)
+            event_info["GAU_ErrX"] * factor / 1e3
+        )
         origin.latitude_errors.uncertainty = kilometer2degrees(
-            event_info["GAU_ErrY"] * factor / 1e3)
+            event_info["GAU_ErrY"] * factor / 1e3
+        )
         origin.depth_errors.uncertainty = event_info["GAU_ErrZ"] * factor
         origin.origin_uncertainty = ouc
 
     # Add OriginQuality info to each origin?
     for origin in event.origins:
         origin.origin_type = "hypocenter"
         origin.evaluation_mode = "automatic"
@@ -219,88 +229,94 @@
             pick.extra = AttribDict()
             pick.waveform_id = wid
             pick.method_id = method
             pick.phase_hint = phase
             if method == "autopick" and str(pickline["PickTime"]) != "-1":
                 pick.time = UTCDateTime(pickline["PickTime"])
                 pick.time_errors.uncertainty = float(pickline["PickError"])
-                pick.extra.snr = {"value": float(pickline["SNR"]),
-                                  "namespace": ns}
+                pick.extra.snr = {"value": float(pickline["SNR"]), "namespace": ns}
             elif method == "modelled":
                 pick.time = UTCDateTime(pickline["ModelledTime"])
             else:
                 continue
             event.picks.append(pick)
 
     # --- Handle amplitudes file ---
     amps_file = locate_dir / "amplitudes" / event_uid
     if amps_file.with_suffix(".amps").is_file():
         amps = pd.read_csv(amps_file.with_suffix(".amps"))
 
         i = 0
         for _, ampsline in amps.iterrows():
             wid = WaveformStreamID(seed_string=ampsline["id"])
-            noise_amp = ampsline["Noise_amp"] / 1000 # mm to m
+            noise_amp = ampsline["Noise_amp"] / 1000  # mm to m
             for phase in ["P_amp", "S_amp"]:
                 amp = Amplitude()
                 if pd.isna(ampsline[phase]):
                     continue
                 amp.generic_amplitude = ampsline[phase] / 1000  # mm to m
                 amp.generic_amplitude_errors.uncertainty = noise_amp
                 amp.unit = "m"
                 amp.type = "AML"
                 amp.method_id = phase
                 amp.period = 1 / ampsline[f"{phase[0]}_freq"]
                 amp.time_window = TimeWindow(
-                    reference=UTCDateTime(ampsline[f"{phase[0]}_time"]))
+                    reference=UTCDateTime(ampsline[f"{phase[0]}_time"])
+                )
                 # amp.pick_id = ?
                 amp.waveform_id = wid
                 # amp.filter_id = ?
                 amp.magnitude_hint = "ML"
                 amp.evaluation_mode = "automatic"
                 amp.extra = AttribDict()
                 try:
                     amp.extra.filter_gain = {
                         "value": ampsline[f"{phase[0]}_filter_gain"],
-                        "namespace": ns}
+                        "namespace": ns,
+                    }
                     amp.extra.avg_amp = {
                         "value": ampsline[f"{phase[0]}_avg_amp"] / 1000,  # m
-                        "namespace": ns}
+                        "namespace": ns,
+                    }
                 except KeyError:
                     pass
 
                 if phase[0] == local_mag_ph and not pd.isna(ampsline["ML"]):
                     i += 1
                     stat_mag = StationMagnitude()
                     stat_mag.extra = AttribDict()
                     # stat_mag.origin_id = ? local_mag_loc
                     stat_mag.mag = ampsline["ML"]
                     stat_mag.mag_errors.uncertainty = ampsline["ML_Err"]
                     stat_mag.station_magnitude_type = "ML"
                     stat_mag.amplitude_id = amp.resource_id
-                    stat_mag.extra.picked = {"value": ampsline["is_picked"],
-                                             "namespace": ns}
-                    stat_mag.extra.epi_dist = {"value": ampsline["epi_dist"],
-                                               "namespace": ns}
-                    stat_mag.extra.z_dist = {"value": ampsline["z_dist"],
-                                             "namespace": ns}
+                    stat_mag.extra.picked = {
+                        "value": ampsline["is_picked"],
+                        "namespace": ns,
+                    }
+                    stat_mag.extra.epi_dist = {
+                        "value": ampsline["epi_dist"],
+                        "namespace": ns,
+                    }
+                    stat_mag.extra.z_dist = {
+                        "value": ampsline["z_dist"],
+                        "namespace": ns,
+                    }
 
                     event.station_magnitudes.append(stat_mag)
 
                 event.amplitudes.append(amp)
 
         mag = Magnitude()
         mag.extra = AttribDict()
         mag.mag = event_info["ML"]
         mag.mag_errors.uncertainty = event_info["ML_Err"]
         mag.magnitude_type = "ML"
         # mag.origin_id = ?
         mag.station_count = i
         mag.evaluation_mode = "automatic"
-        mag.extra.r2 = {"value": event_info["ML_r2"],
-                        "namespace": ns}
+        mag.extra.r2 = {"value": event_info["ML_r2"], "namespace": ns}
 
         event.magnitudes = [mag]
         event.preferred_magnitude_id = mag.resource_id
 
-
     return event
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quakemigrate-1.0.1/quakemigrate/export/to_snuffler.py` & `quakemigrate-1.0.2/quakemigrate/export/to_snuffler.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding:utf-8 -*-
 """
-This module provides parsers to generate input files for Snuffler, a manual
-phase picking interface from the Pyrocko package.
+This module provides parsers to generate input files for Snuffler, a manual phase
+picking interface from the Pyrocko package.
 
 :copyright:
-    2020 - 2021, QuakeMigrate developers.
+    2020–2023, QuakeMigrate developers.
 :license:
     GNU General Public License, Version 3
     (https://www.gnu.org/licenses/gpl-3.0.html)
 
 """
 
 import pathlib
@@ -39,81 +39,90 @@
         for i, station in stations.iterrows():
             if network_code is None:
                 try:
                     network_code = station["Network"]
                 except KeyError:
                     network_code = ""
 
-            line = line_template.format(nw=network_code,
-                                        stat=station["Name"],
-                                        lat=station["Latitude"],
-                                        lon=station["Longitude"],
-                                        elev=station["Elevation"],
-                                        dep="0")
+            line = line_template.format(
+                nw=network_code,
+                stat=station["Name"],
+                lat=station["Latitude"],
+                lon=station["Longitude"],
+                elev=station["Elevation"],
+                dep="0",
+            )
 
             f.write(line)
 
 
 def snuffler_markers(event, output_path, filename=None):
     """
     Function to create marker files compatible with snuffler
 
     Parameters
     ----------
     event : `ObsPy.Event` object
-        Contains information about the origin time and a list of associated
-        picks
+        Contains information about the origin time and a list of associated picks.
     output_path : str
-        Location to save the marker file
+        Location to save the marker file.
     filename : str, optional
-        Name of marker file - defaults to eventid/eventid.markers
+        Name of marker file - defaults to 'eventid/eventid.markers'.
 
     """
 
     if filename is None:
-        filename = "{0}.markers".format(str(event.resource_id))
+        filename = f"{event.resource_id}.markers"
 
     output_path = pathlib.Path(output_path) / str(event.resource_id)
     output_path.mkdir(parents=True, exist_ok=True)
 
     output = output_path / filename
 
-    line_template = "phase: {year}-{month}-{day} {hr}:{min}:{sec}.{msec} 5 "
-    line_template += "{nw}.{stat}..{comp} None None None {phase} None False\n"
+    line_template = (
+        "phase: {year}-{month}-{day} {hr}:{min}:{sec}.{msec} 5 {nw}.{stat}..{comp} "
+        "None None None {phase} None False\n"
+    )
 
     origin = event.origins[0]
 
     # Write event line to file
-    event_line = "event: {year}-{month}-{day} {hr}:{min}:{sec}.{msec} 0 "
-    event_line += "{eventid} 0.0 0.0 None None None Event None\n"
-
-    event_line = event_line.format(year=origin.time.year,
-                                   month=str(origin.time.month).zfill(2),
-                                   day=str(origin.time.day).zfill(2),
-                                   hr=str(origin.time.hour).zfill(2),
-                                   min=str(origin.time.minute).zfill(2),
-                                   sec=str(origin.time.second).zfill(2),
-                                   msec=origin.time.microsecond,
-                                   eventid=str(event.resource_id))
+    event_line = (
+        "event: {year}-{month}-{day} {hr}:{min}:{sec}.{msec} 0 {eventid} 0.0 0.0 None "
+        "None None Event None\n"
+    )
+
+    event_line = event_line.format(
+        year=origin.time.year,
+        month=str(origin.time.month).zfill(2),
+        day=str(origin.time.day).zfill(2),
+        hr=str(origin.time.hour).zfill(2),
+        min=str(origin.time.minute).zfill(2),
+        sec=str(origin.time.second).zfill(2),
+        msec=origin.time.microsecond,
+        eventid=str(event.resource_id),
+    )
 
     with output.open("w") as f:
         f.write("# Snuffler Markers File Version 0.2\n")
         f.write(event_line)
 
         for pick in event.picks:
             if pick.phase_hint == "P":
                 comp = "BHZ"
             elif pick.phase_hint == "S":
                 comp = "BHN"
-            line = line_template.format(year=pick.time.year,
-                                        month=str(pick.time.month).zfill(2),
-                                        day=str(pick.time.day).zfill(2),
-                                        hr=str(pick.time.hour).zfill(2),
-                                        min=str(pick.time.minute).zfill(2),
-                                        sec=str(pick.time.second).zfill(2),
-                                        msec=pick.time.microsecond,
-                                        nw=pick.waveform_id.network_code,
-                                        stat=pick.waveform_id.station_code,
-                                        comp=comp,
-                                        phase=pick.phase_hint)
+            line = line_template.format(
+                year=pick.time.year,
+                month=str(pick.time.month).zfill(2),
+                day=str(pick.time.day).zfill(2),
+                hr=str(pick.time.hour).zfill(2),
+                min=str(pick.time.minute).zfill(2),
+                sec=str(pick.time.second).zfill(2),
+                msec=pick.time.microsecond,
+                nw=pick.waveform_id.network_code,
+                stat=pick.waveform_id.station_code,
+                comp=comp,
+                phase=pick.phase_hint,
+            )
 
             f.write(line)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quakemigrate-1.0.1/quakemigrate/io/__init__.py` & `quakemigrate-1.0.2/quakemigrate/io/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 """
-The :mod:`quakemigrate.io` module handles the various input/output operations
-performed by QuakeMigrate. This includes:
+The :mod:`quakemigrate.io` module handles the various input/output operations performed
+by QuakeMigrate. This includes:
 
     * Reading waveform data - The submodule data.py can handle any waveform \
       data archive with a regular directory structure. It also provides \
       functions for checking data quality and removing/simulating instrument \
       reponse.
     * Reading station files, velocity model files, instrument response \
       inventories and QuakeMigrate lookup tables.
@@ -16,24 +16,29 @@
       event, and provides functionality to write ".event" files.
     * Reading and writing results, including station availablity data and \
       continuous coalescence output from detect; triggered event files from \
       trigger, amplitude and local magnitude measurements and cut waveforms \
       for located events.
 
 :copyright:
-    2020 - 2021, QuakeMigrate developers.
+    2020–2023, QuakeMigrate developers.
 :license:
     GNU General Public License, Version 3
     (https://www.gnu.org/licenses/gpl-3.0.html)
 
 """
 
 from .amplitudes import write_amplitudes  # NOQA
 from .availability import read_availability, write_availability  # NOQA
 from .cut_waveforms import write_cut_waveforms  # NOQA
 from .data import Archive  # NOQA
 from .event import Event  # NOQA
-from .core import (read_lut, read_response_inv, read_stations,  # NOQA
-                   read_vmodel, stations, Run)
+from .core import (
+    read_lut,  # NOQA
+    read_response_inv,  # NOQA
+    read_stations,  # NOQA
+    read_vmodel,  # NOQA
+    stations,  # NOQA
+    Run,  # NOQA
+)
 from .scanmseed import ScanmSEED, read_scanmseed  # NOQA
-from .triggered_events import (read_triggered_events,  # NOQA
-                               write_triggered_events)
+from .triggered_events import read_triggered_events, write_triggered_events  # NOQA
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quakemigrate-1.0.1/quakemigrate/io/amplitudes.py` & `quakemigrate-1.0.2/quakemigrate/io/amplitudes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 # -*- coding: utf-8 -*-
 """
 Module to handle input/output of .amps files.
 
 :copyright:
-    2020 - 2021, QuakeMigrate developers.
+    2020–2023, QuakeMigrate developers.
 :license:
     GNU General Public License, Version 3
     (https://www.gnu.org/licenses/gpl-3.0.html)
 
 """
 
 
 def write_amplitudes(run, amplitudes, event):
     """
-    Write amplitude results to a new .amps file. This includes amplitude
-    measurements, and the magnitude estimates derived from them (with station
-    correction terms appied, if provided).
+    Write amplitude results to a new .amps file. This includes amplitude measurements,
+    and the magnitude estimates derived from them (with station correction terms
+    applied, if provided).
 
     Parameters
     ----------
     run : :class:`~quakemigrate.io.core.Run` object
         Light class encapsulating i/o path information for a given run.
     amplitudes : `pandas.DataFrame` object
-        P- and S-wave amplitude measurements for each component of each
-        station in the station file, and individual local magnitude estimates
-        derived from them.
+        P- and S-wave amplitude measurements for each component of each station in the
+        station file, and individual local magnitude estimates derived from them.
         Columns = ["epi_dist", "z_dist", "P_amp", "P_freq", "P_time",
                    "P_avg_amp", "P_filter_gain", "S_amp", "S_freq", "S_time",
                    "S_avg_amp", "S_filter_gain", "Noise_amp", "is_picked",
                    "ML", "ML_Err"]
         Index = Trace ID (see `obspy.Trace` object property 'id')
     event : :class:`~quakemigrate.io.event.Event` object
         Light class encapsulating waveforms, coalescence information, picks and
@@ -39,21 +38,26 @@
     fpath = run.path / "locate" / run.subname / "amplitudes"
     fpath.mkdir(exist_ok=True, parents=True)
 
     # Work on a copy
     amplitudes = amplitudes.copy()
 
     # Set floating point precision for output file
-    for col in ["epi_dist", "z_dist", "P_amp", "P_avg_amp", "S_amp",
-                "S_avg_amp", "Noise_amp"]:
-        amplitudes[col] = amplitudes[col].map(lambda x: f"{x:.5g}",
-                                              na_action="ignore")
+    for col in [
+        "epi_dist",
+        "z_dist",
+        "P_amp",
+        "P_avg_amp",
+        "S_amp",
+        "S_avg_amp",
+        "Noise_amp",
+    ]:
+        amplitudes[col] = amplitudes[col].map(lambda x: f"{x:.5g}", na_action="ignore")
     for col in ["P_freq", "S_freq"]:
-        amplitudes[col] = amplitudes[col].map(lambda x: f"{x:.2g}",
-                                              na_action="ignore")
+        amplitudes[col] = amplitudes[col].map(lambda x: f"{x:.2g}", na_action="ignore")
     for col in ["P_filter_gain", "S_filter_gain", "ML", "ML_Err"]:
-        amplitudes[col] = amplitudes[col].map(lambda x: f"{x:.3g}",
-                                              na_action="ignore")
+        amplitudes[col] = amplitudes[col].map(lambda x: f"{x:.3g}", na_action="ignore")
 
     fstem = f"{event.uid}"
     file = (fpath / fstem).with_suffix(".amps")
+
     amplitudes.to_csv(file, index=True)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quakemigrate-1.0.1/quakemigrate/io/availability.py` & `quakemigrate-1.0.2/quakemigrate/io/availability.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 Module to handle input/output of StationAvailability.csv files.
 
 :copyright:
-    2020 - 2021, QuakeMigrate developers.
+    2020–2023, QuakeMigrate developers.
 :license:
     GNU General Public License, Version 3
     (https://www.gnu.org/licenses/gpl-3.0.html)
 
 """
 
 import logging
@@ -16,16 +16,16 @@
 import pandas as pd
 
 import quakemigrate.util as util
 
 
 def read_availability(run, starttime, endtime):
     """
-    Read in station availability data to a `pandas.DataFrame` from csv files
-    split by Julian day.
+    Read in station availability data to a `pandas.DataFrame` from csv files split by
+    Julian day.
 
     Parameters
     ----------
     run : :class:`~quakemigrate.io.core.Run` object
         Light class encapsulating i/o path information for a given run.
     starttime : `obspy.UTCDateTime` object
         Timestamp from which to read the station availability.
@@ -51,45 +51,47 @@
         try:
             if availability is None:
                 availability = _handle_old_structure(file)
             else:
                 tmp = _handle_old_structure(file)
                 availability = pd.concat([availability, tmp])
         except FileNotFoundError:
-            logging.info("\tNo .StationAvailability file found for "
-                         f"{readstart.year} - {readstart.julday:03d}")
+            logging.info(
+                "\tNo .StationAvailability file found for "
+                f"{readstart.year} - {readstart.julday:03d}"
+            )
         readstart += 86400
 
     if availability is None:
         raise util.NoStationAvailabilityDataException
 
     starttime, endtime = availability.index[0], availability.index[-1]
     logging.debug(f"\t\t...from {starttime} - {endtime}")
 
     return availability
 
 
 def _handle_old_structure(availability_in_file, permanent_conversion=False):
     """
-    A short utility function that dynamically converts the old style
-    availability files (with column names simply the station) to the new style
-    (with separate columns for each station/phase combination). This uses the
-    knowledge that an availability of '1' in the old style meant that all data
-    was available (e.g. <station>_P and <station>_S available).
+    A short utility function that dynamically converts the old style availability files
+    (with column names simply the station) to the new style (with separate columns for
+    each station/phase combination). This uses the knowledge that an availability of '1'
+    in the old style meant that all data was available (e.g. <station>_P and <station>_S
+    available).
 
-    This is only done if the file was in the old format - otherwise it just
-    returns the original, unaltered dataframe.
+    This is only done if the file was in the old format - otherwise it just returns the
+    original, unaltered dataframe.
 
     Parameters
     ----------
     availability_in_file : `pathlib.Path` object
         An availability file to be read in, tested and potentially converted.
     permanent_conversion : bool, optional
-        If toggled, the availability file will be permanently converted to the
-        new file structure.
+        If toggled, the availability file will be permanently converted to the new file
+        structure.
 
     Returns
     -------
     availability_out : `pandas.DataFrame` object
         The corrected (if necessary) availability dataframe.
 
     """
@@ -99,32 +101,32 @@
     cols = [col_names.split("_") for col_names in availability_in.columns]
 
     # Check if station + phase are already in the column names
     if len(cols[0]) == 2:
         return availability_in
 
     availability_out = pd.DataFrame()
-    logging.info("\t\tWarning: an availability file is in the old format - "
-                 "converting...")
+    logging.info(
+        "\t\tWarning: an availability file is in the old format - converting..."
+    )
     for phase in "PS":
         for stat in cols:
             new_key = f"{stat[0]}_{phase}"
             availability_out[new_key] = availability_in[stat[0]].values
     availability_out.index = availability_in.index
 
     if permanent_conversion:
         availability_out.to_csv(availability_in_file)
 
     return availability_out
 
 
 def write_availability(run, availability):
     """
-    Write out csv files (split by Julian day) containing station availability
-    data.
+    Write out csv files (split by Julian day) containing station availability data.
 
     Parameters
     ----------
     run : :class:`~quakemigrate.io.core.Run` object
         Light class encapsulating i/o path information for a given run.
     availability : `pandas.DataFrame` object
         Details the availability of each station for each timestep of detect.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quakemigrate-1.0.1/quakemigrate/io/core.py` & `quakemigrate-1.0.2/quakemigrate/io/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 Module to handle input/output for QuakeMigrate.
 
 :copyright:
-    2020 - 2021, QuakeMigrate developers.
+    2020–2023, QuakeMigrate developers.
 :license:
     GNU General Public License, Version 3
     (https://www.gnu.org/licenses/gpl-3.0.html)
 
 """
 
 import logging
@@ -19,16 +19,15 @@
 
 import quakemigrate.util as util
 from quakemigrate.lut import LUT
 
 
 def read_lut(lut_file):
     """
-    Read the contents of a pickle file and restore state of the lookup table
-    object.
+    Read the contents of a pickle file and restore state of the lookup table object.
 
     Parameters
     ----------
     lut_file : str
         Path to pickle file to load.
 
     Returns
@@ -39,26 +38,29 @@
     """
 
     lut = LUT()
     with open(lut_file, "rb") as f:
         lut.__dict__.update(pickle.load(f))
 
     if hasattr(lut, "maps"):
-        print("FutureWarning: The internal data structure of LUT has changed."
-              "\nTo remove this warning you will need to convert your lookup "
-              "table to the new-style\nusing `quakemigrate.lut.update_lut`.")
+        print(
+            "FutureWarning: The internal data structure of LUT has changed."
+            "\nTo remove this warning you will need to convert your lookup "
+            "table to the new-style\nusing `quakemigrate.lut.update_lut`."
+        )
 
     return lut
 
 
 def stations(station_file, **kwargs):
     """Alias for read_stations."""
-    print("FutureWarning: function name has changed - continuing.")
-    print("To remove this message, change:")
-    print("\t'stations' -> 'read_stations'")
+    print(
+        "FutureWarning: function name has changed - continuing.\n"
+        "To remove this message, change:\t'stations' -> 'read_stations'"
+    )
 
     return read_stations(station_file, **kwargs)
 
 
 def read_stations(station_file, **kwargs):
     """
     Reads station information from file.
@@ -83,41 +85,39 @@
     StationFileHeaderException
         Raised if the input file is missing required entries in the header.
 
     """
 
     stn_data = pd.read_csv(station_file, **kwargs)
 
-    if ("Latitude" or "Longitude" or "Elevation" or "Name") \
-       not in stn_data.columns:
+    if ("Latitude" or "Longitude" or "Elevation" or "Name") not in stn_data.columns:
         raise util.StationFileHeaderException
 
-    stn_data["Elevation"] = stn_data["Elevation"].apply(lambda x: -1*x)
+    stn_data["Elevation"] = stn_data["Elevation"].apply(lambda x: -1 * x)
 
     # Ensure station names are strings
     stn_data = stn_data.astype({"Name": "str"})
 
     return stn_data
 
 
 def read_response_inv(response_file, sac_pz_format=False):
     """
-    Reads response information from file, returning it as a `obspy.Inventory`
-    object.
+    Reads response information from file, returning it as a `obspy.Inventory` object.
 
     Parameters
     ----------
     response_file : str
         Path to response file.
-        Please see the `obspy.read_inventory()` documentation for a full list
-        of supported file formats. This includes a dataless.seed volume, a
-        concatenated series of RESP files or a stationXML file.
+        Please see the `obspy.read_inventory()` documentation for a full list of
+        supported file formats. This includes a dataless.seed volume, a concatenated
+        series of RESP files or a stationXML file.
     sac_pz_format : bool, optional
-        Toggle to indicate that response information is being provided in SAC
-        Pole-Zero files. NOTE: not yet supported.
+        Toggle to indicate that response information is being provided in SAC Pole-Zero
+        files. NOTE: not yet supported.
 
     Returns
     -------
     response_inv : `obspy.Inventory` object
         ObsPy response inventory.
 
     Raises
@@ -126,23 +126,25 @@
         If the user selects `sac_pz_format=True`.
     TypeError
         If the user provides a response file that is not readable by ObsPy.
 
     """
 
     if sac_pz_format:
-        raise NotImplementedError("SAC_PZ is not yet supported. Please contact "
-                                  "the QuakeMigrate developers.")
+        raise NotImplementedError(
+            "SAC_PZ is not yet supported. Please contact the QuakeMigrate developers."
+        )
     else:
         try:
             response_inv = read_inventory(response_file)
         except TypeError as e:
-            msg = (f"Response file not readable by ObsPy: {e}\n"
-                   "Please consult the ObsPy documentation.")
-            raise TypeError(msg)
+            raise TypeError(
+                f"Response file not readable by ObsPy: {e}\n"
+                "Please consult the ObsPy documentation."
+            )
 
     return response_inv
 
 
 def read_vmodel(vmodel_file, **kwargs):
     """
     Reads velocity model information from file.
@@ -188,34 +190,34 @@
     Light class to encapsulate i/o path information for a given run.
 
     Parameters
     ----------
     stage : str
         Specifies run stage of QuakeMigrate ("detect", "trigger", or "locate").
     path : str
-        Points to the top level directory containing all input files, under
-        which the specific run directory will be created.
+        Points to the top level directory containing all input files, under which the
+        specific run directory will be created.
     name : str
         Name of the current QuakeMigrate run.
     subname : str, optional
-        Optional name of a sub-run - useful when testing different trigger
-        parameters, for example.
+        Optional name of a sub-run - useful when testing different trigger parameters,
+        for example.
 
     Attributes
     ----------
     path : `pathlib.Path` object
-        Points to the top level directory containing all input files, under
-        which the specific run directory will be created.
+        Points to the top level directory containing all input files, under which the
+        specific run directory will be created.
     name : str
         Name of the current QuakeMigrate run.
     run_path : `pathlib.Path` object
         Points to the run directory into which files will be written.
     subname : str
-        Optional name of a sub-run - useful when testing different trigger
-        parameters, for example.
+        Optional name of a sub-run - useful when testing different trigger parameters,
+        for example.
     stage : {"detect", "trigger", "locate"}, optional
         Track which stage of QuakeMigrate is being run.
     loglevel : {"info", "debug"}, optional
         Set the logging level. (Default "info")
 
     Methods
     -------
@@ -224,41 +226,44 @@
 
     """
 
     def __init__(self, path, name, subname="", stage=None, loglevel="info"):
         """Instantiate the Run object."""
 
         if "." in name or "." in subname:
-            print("Warning: The character '.' is not allowed in run"
-                  "names/subnames - replacing with '_'.")
+            print(
+                "Warning: The character '.' is not allowed in run names/subnames - "
+                "replacing with '_'."
+            )
             name = name.replace(".", "_")
             subname = subname.replace(".", "_")
 
         self.path = pathlib.Path(path) / name
         self._name = name
         self.stage = stage
         self.subname = subname
         self.loglevel = loglevel
 
     def __str__(self):
         """Return short summary string of the Run object."""
 
-        return (f"{util.log_spacer}\n{util.log_spacer}\n"
-                f"\tQuakeMigrate RUN - Path: {self.path} - Name: {self.name}\n"
-                f"{util.log_spacer}\n{util.log_spacer}\n")
+        return (
+            f"{util.log_spacer}\n{util.log_spacer}\n"
+            f"\tQuakeMigrate RUN - Path: {self.path} - Name: {self.name}\n"
+            f"{util.log_spacer}\n{util.log_spacer}\n"
+        )
 
     def logger(self, log):
         """
         Configures the logging feature.
 
         Parameters
         ----------
         log : bool
-            Toggle for logging. If True, will output to stdout and generate a
-            log file.
+            Toggle for logging. If True, will output to stdout and generate a log file.
 
         """
 
         logstem = self.path / self.stage / self.subname / "logs" / self.name
         util.logger(logstem, log, loglevel=self.loglevel)
         logging.info(self)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quakemigrate-1.0.1/quakemigrate/io/cut_waveforms.py` & `quakemigrate-1.0.2/quakemigrate/io/cut_waveforms.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,80 +1,89 @@
 # -*- coding: utf-8 -*-
 """
 Module to handle input/output of cut waveforms.
 
 :copyright:
-    2020 - 2021, QuakeMigrate developers.
+    2020–2023, QuakeMigrate developers.
 :license:
     GNU General Public License, Version 3
     (https://www.gnu.org/licenses/gpl-3.0.html)
 
 """
 
 import logging
 import warnings
 
 from obspy import Stream
 
 import quakemigrate.util as util
 
 
-warnings.filterwarnings("ignore", message=("File will be written with more tha"
-                                           "n one different record lengths.\nT"
-                                           "his might have a negative influenc"
-                                           "e on the compatibility with other "
-                                           "programs."))
-warnings.filterwarnings("ignore", message=("File will be written with more tha"
-                                           "n one different encodings.\nThis m"
-                                           "ight have a negative influence on "
-                                           "the compatibility with other progr"
-                                           "ams."))
-warnings.filterwarnings("ignore", message=("The encoding specified in "
-                                           "trace.stats.mseed.encoding does "
-                                           "not match the dtype of the data.\n"
-                                           "A suitable encoding will be "
-                                           "chosen."))
-
+warnings.filterwarnings(
+    "ignore",
+    message=(
+        "File will be written with more than one different record lengths.\nThis might "
+        "have a negative influence on the compatibility with other programs."
+    ),
+)
+warnings.filterwarnings(
+    "ignore",
+    message=(
+        "File will be written with more than one different encodings.\nThis might have "
+        "a negative influence on the compatibility with other programs."
+    ),
+)
+warnings.filterwarnings(
+    "ignore",
+    message=(
+        "The encoding specified in trace.stats.mseed.encoding does not match the dtype "
+        "of the data.\nA suitable encoding will be chosen."
+    ),
+)
 
 
 @util.timeit("info")
-def write_cut_waveforms(run, event, file_format, pre_cut=0., post_cut=0.,
-                        waveform_type="raw", units="displacement"):
+def write_cut_waveforms(
+    run,
+    event,
+    file_format,
+    pre_cut=0.0,
+    post_cut=0.0,
+    waveform_type="raw",
+    units="displacement",
+):
     """
     Output cut waveform data as a waveform file -- defaults to miniSEED format.
 
     Parameters
     ----------
     run : :class:`~quakemigrate.io.core.Run` object
         Light class encapsulating i/o path information for a given run.
     event : :class:`~quakemigrate.io.event.Event` object
-        Light class encapsulating waveforms, coalescence information, picks and
-        location information for a given event.
+        Light class encapsulating waveforms, coalescence information, picks and location
+        information for a given event.
     file_format : str, optional
-        File format to write waveform data to. Options are all file formats
-        supported by obspy, including: "MSEED" (default), "SAC", "SEGY",
-        "GSE2"
+        File format to write waveform data to. Options are all file formats supported by
+        ObsPy, including: "MSEED" (default), "SAC", "SEGY", "GSE2"
     pre_cut : float or None, optional
-        Specify how long before the event origin time to cut the waveform
-        data from.
+        Specify how long before the event origin time to cut the waveform data from.
     post_cut : float or None, optional
-        Specify how long after the event origin time to cut the waveform
-        data to.
+        Specify how long after the event origin time to cut the waveform data to.
     waveform_type : {"raw", "real", "wa"}, optional
         Whether to output raw, real or Wood-Anderson simulated waveforms.
         Default: "raw"
     units : {"displacement", "velocity"}, optional
-        Whether to output displacement waveforms or velocity waveforms for
-        real / Wood-Anderson corrected traces. Default: displacement
+        Whether to output displacement waveforms or velocity waveforms for real/
+        Wood-Anderson corrected traces. Default: displacement
 
     Raises
     ------
     AttributeError
-        If real or wa waveforms are requested and no response inventory has
-        been provided.
+        If real or wa waveforms are requested and no response inventory has been
+        provided.
 
     """
 
     logging.info(f"\tSaving {waveform_type} cut waveforms...")
 
     fpath = run.path / "locate" / run.subname / f"{waveform_type}_cut_waveforms"
     fpath.mkdir(exist_ok=True, parents=True)
@@ -92,59 +101,64 @@
 
     # Remove empty traces
     for tr in st:
         if not bool(tr):
             st.remove(tr)
 
     if waveform_type == "real" or waveform_type == "wa":
-        if waveform_type == "real" and \
-            isinstance(event.data.real_waveforms, Stream) and not pre_cut \
-            and not post_cut:
+        if (
+            waveform_type == "real"
+            and isinstance(event.data.real_waveforms, Stream)
+            and not pre_cut
+            and not post_cut
+        ):
             st = event.data.real_waveforms
-        elif waveform_type == "wa" and \
-            isinstance(event.data.wa_waveforms, Stream) and not pre_cut \
-            and not post_cut:
+        elif (
+            waveform_type == "wa"
+            and isinstance(event.data.wa_waveforms, Stream)
+            and not pre_cut
+            and not post_cut
+        ):
             st = event.data.wa_waveforms
         else:
             try:
                 st = get_waveforms(st, event, waveform_type, units)
             except AttributeError as e:
-                raise AttributeError("To output real or Wood-Anderson"
-                                     " cut waveforms you must supply an "
-                                     "instrument response inventory.") from e
+                raise AttributeError(
+                    "To output real or Wood-Anderson cut waveforms you must supply an "
+                    "instrument response inventory."
+                ) from e
 
     if bool(st):
         write_waveforms(st, fpath, fstem, file_format)
     else:
-        logging.info(f"\t\tNo {waveform_type} cut waveform data for event "
-                     f"{event.uid} !")
+        logging.info(f"\t\tNo {waveform_type} cut waveform data for event{event.uid}!")
 
 
 @util.timeit("debug")
 def get_waveforms(st, event, waveform_type, units):
     """
     Get real or simulated waveforms for a Stream.
 
     Parameters
     ----------
     st : `obspy.Stream` object
         Stream for which to get real or simulated waveforms.
     event : :class:`~quakemigrate.io.event.Event` object
-        Light class encapsulating waveforms, coalescence information, picks and
-        location information for a given event.
+        Light class encapsulating waveforms, coalescence information, picks and location
+        information for a given event.
     waveform_type : {"real", "wa"}
         Whether to get real or Wood-Anderson simulated waveforms.
     units : {"displacement", "velocity"}
         Units to return waveforms in.
 
     Returns
     -------
     st_out : `obspy.Stream` object
-        Stream of real or Wood-Anderson simulated waveforms in the requested
-        units.
+        Stream of real or Wood-Anderson simulated waveforms in the requested units.
 
     """
 
     # Work on a copy
     st = st.copy()
     st_out = Stream()
 
@@ -155,16 +169,15 @@
         if bool(tr) and tr.data.max() != tr.data.min():
             try:
                 if waveform_type == "real":
                     tr = event.data.get_real_waveform(tr, velocity)
                 else:
                     tr = event.data.get_wa_waveform(tr, velocity)
                 st_out.append(tr)
-            except (util.ResponseNotFoundError,
-                    util.ResponseRemovalError) as e:
+            except (util.ResponseNotFoundError, util.ResponseRemovalError) as e:
                 logging.warning(e)
 
     return st_out
 
 
 @util.timeit("debug")
 def write_waveforms(st, fpath, fstem, file_format):
@@ -176,17 +189,16 @@
     st : `obspy.Stream` object
         Waveforms to be written to file.
     fpath : `pathlib.Path` object
         Path to output directory.
     fstem : str
         File name (without suffix).
     file_format : str
-        File format to write waveform data to. Options are all file formats
-        supported by obspy, including: "MSEED" (default), "SAC", "SEGY",
-        "GSE2"
+        File format to write waveform data to. Options are all file formats supported by
+        ObsPy, including: "MSEED" (default), "SAC", "SEGY", "GSE2"
 
     """
 
     if file_format == "MSEED":
         suffix = ".m"
     elif file_format == "SAC":
         suffix = ".sac"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quakemigrate-1.0.1/quakemigrate/io/data.py` & `quakemigrate-1.0.2/quakemigrate/io/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 Module for processing waveform files stored in a data archive.
 
 :copyright:
-    2020 - 2021, QuakeMigrate developers.
+    2020–2023, QuakeMigrate developers.
 :license:
     GNU General Public License, Version 3
     (https://www.gnu.org/licenses/gpl-3.0.html)
 
 """
 
 from itertools import chain
@@ -19,84 +19,80 @@
 import quakemigrate.util as util
 
 
 class Archive:
     """
     The Archive class handles the reading of archived waveform data.
 
-    It is capable of handling any regular archive structure. Requests to read
-    waveform data are served up as a
-    :class:`~quakemigrate.io.data.WaveformData` object.
-
-    If provided, a response inventory for the archive will be stored with the
-    waveform data for response removal, if needed (e.g. for local magnitude
-    calculation, or to output real cut waveforms).
-
-    By default, data with mismatched sampling rates will only be decimated.
-    If necessary, and if the user specifies `resample = True` and an
-    upfactor to upsample by `upfactor = int` for the waveform archive, data
-    can also be upsampled and then, if necessary, subsequently decimated to
-    achieve the desired sampling rate.
-
-    For example, for raw input data sampled at a mix of 40, 50 and 100 Hz,
-    to achieve a unified sampling rate of 50 Hz, the user would have to
-    specify an upfactor of 5; 40 Hz x 5 = 200 Hz, which can then be
-    decimated to 50 Hz - see :func:`~quakemigrate.util.resample`.
+    It is capable of handling any regular archive structure. Requests to read waveform
+    data are served up as a :class:`~quakemigrate.io.data.WaveformData` object.
+
+    If provided, a response inventory for the archive will be stored with the waveform
+    data for response removal, if needed (e.g. for local magnitude calculation, or to
+    output real cut waveforms).
+
+    By default, data with mismatched sampling rates will only be decimated. If
+    necessary, and if the user specifies `resample = True` and an upfactor to upsample
+    by `upfactor = int` for the waveform archive, data can also be upsampled and then,
+    if necessary, subsequently decimated to achieve the desired sampling rate.
+
+    For example, for raw input data sampled at a mix of 40, 50 and 100 Hz, to achieve a
+    unified sampling rate of 50 Hz, the user would have to specify an upfactor of 5;
+    40 Hz x 5 = 200 Hz, which can then be decimated to 50 Hz - see
+    :func:`~quakemigrate.util.resample`.
 
     Parameters
     ----------
     archive_path : str
         Location of seismic data archive: e.g.: "./DATA_ARCHIVE".
     stations : `pandas.DataFrame` object
         Station information.
-        Columns ["Latitude", "Longitude", "Elevation", "Name"]. See
-        :func:`~quakemigrate.io.core.read_stations`
+        Columns ["Latitude", "Longitude", "Elevation", "Name"].
+        See :func:`~quakemigrate.io.core.read_stations`
     archive_format : str, optional
-        Sets directory structure and file naming format for different archive
-        formats. See :func:`~quakemigrate.io.data.Archive.path_structure`
+        Sets directory structure and file naming format for different archive formats.
+        See :func:`~quakemigrate.io.data.Archive.path_structure`
     kwargs : **dict
         See Archive Attributes for details.
 
     Attributes
     ----------
     archive_path : `pathlib.Path` object
         Location of seismic data archive: e.g.: ./DATA_ARCHIVE.
     stations : `pandas.Series` object
         Series object containing station names.
     format : str
         Directory structure and file naming format of data archive.
     read_all_stations : bool, optional
-        If True, read all stations in archive for that time period. Else, only
-        read specified stations.
+        If True, read all stations in archive for that time period. Else, only read
+        specified stations.
     resample : bool, optional
-        If true, perform resampling of data which cannot be decimated directly
-        to the desired sampling rate. See :func:`~quakemigrate.util.resample`
+        If true, perform resampling of data which cannot be decimated directly to the
+        desired sampling rate. See :func:`~quakemigrate.util.resample`
     response_inv : `obspy.Inventory` object, optional
-        ObsPy response inventory for this waveform archive, containing
-        response information for each channel of each station of each network.
+        ObsPy response inventory for this waveform archive, containing response
+        information for each channel of each station of each network.
     pre_filt : tuple of floats
         Pre-filter to apply during the instrument response removal. E.g.
         (0.03, 0.05, 30., 35.) - all in Hz. (Default None)
     water_level : float
         Water level to use in instrument response removal. (Default 60.)
     remove_full_response : bool
-        Whether to remove the full response (including the effect of
-        digital FIR filters) or just the instrument transform function (as
-        defined by the PolesZeros Response Stage). Significantly slower.
-        (Default False)
+        Whether to remove the full response (including the effect of digital FIR
+        filters) or just the instrument transform function (as defined by the PolesZeros
+        Response Stage). Significantly slower. (Default False)
     upfactor : int, optional
-        Factor by which to upsample the data to enable it to be decimated to
-        the desired sampling rate, e.g. 40Hz -> 50Hz requires upfactor = 5.
+        Factor by which to upsample the data to enable it to be decimated to the desired
+        sampling rate, e.g. 40Hz -> 50Hz requires upfactor = 5.
         See :func:`~quakemigrate.util.resample`
     interpolate : bool, optional
-        If data is timestamped "off-sample" (i.e. a non-integer number of
-        samples after midnight), whether to interpolate the data to apply the
-        necessary correction. Default behaviour is to just alter the metadata,
-        resulting in a sub-sample timing offset. See
-        :func:`~quakemigrate.util.shift_to_sample`.
+        If data is timestamped "off-sample" (i.e. a non-integer number of samples after
+        midnight), whether to interpolate the data to apply the necessary correction.
+        Default behaviour is to just alter the metadata, resulting in a sub-sample
+        timing offset. See :func:`~quakemigrate.util.shift_to_sample`.
 
     Methods
     -------
     path_structure(archive_format, channels="*")
         Set the directory structure and file naming format of the data archive.
     read_waveform_data(starttime, endtime)
         Read in waveform data between two times.
@@ -119,34 +115,33 @@
         self.resample = kwargs.get("resample", False)
         self.upfactor = kwargs.get("upfactor")
         self.interpolate = kwargs.get("interpolate", False)
         # Response removal parameters
         self.response_inv = kwargs.get("response_inv")
         response_removal_params = kwargs.get("response_removal_params", {})
         if self.response_inv and "water_level" not in response_removal_params.keys():
-            msg = (
+            print(  # Logger not yet spun up
                 "Warning: 'water level' for instrument correction not "
                 "specified. Set to default: 60"
             )
-            print(msg)  # Logger not yet spun up
         self.water_level = response_removal_params.get("water_level", 60.0)
         self.pre_filt = response_removal_params.get("pre_filt")
         self.remove_full_response = response_removal_params.get(
             "remove_full_response", False
         )
 
     def __str__(self, response_only=False):
         """
         Returns a short summary string of the Archive object.
 
         Parameters
         ----------
         response_only : bool, optional
-            Whether to just output the a string describing the instrument
-            response parameters.
+            Whether to just output the a string describing the instrument response
+            parameters.
 
         Returns
         -------
         out : str
             Summary string.
 
         """
@@ -181,24 +176,22 @@
         else:
             out = response_str
 
         return out
 
     def path_structure(self, archive_format="YEAR/JD/STATION", channels="*"):
         """
-        Define the directory structure and file naming format of the data
-        archive.
+        Define the directory structure and file naming format of the data archive.
 
         Parameters
         ----------
         archive_format : str, optional
-            Directory structure and file naming format of the data archive.
-            This may be the name of a generic archive format (e.g. SeisComp3),
-            or one of a selection of additional formats built into
-            QuakeMigrate.
+            Directory structure and file naming format of the data archive. This may be
+            the name of a generic archive format (e.g. SeisComp3), or one of a selection
+            of additional formats built into QuakeMigrate.
         channels : str, optional
             Channel codes to include. E.g. channels="[B,H]H*". (Default "*")
 
         Raises
         ------
         ArchivePathStructureError
             If the `archive_format` specified by the user is not a valid option.
@@ -225,21 +218,20 @@
         else:
             raise util.ArchivePathStructureError(archive_format)
 
     def read_waveform_data(self, starttime, endtime, pre_pad=0.0, post_pad=0.0):
         """
         Read in waveform data from the archive between two times.
 
-        Supports all formats currently supported by ObsPy, including: "MSEED",
-        "SAC", "SEGY", "GSE2" .
+        Supports all formats currently supported by ObsPy, including: "MSEED", "SAC",
+        "SEGY", "GSE2".
 
-        Optionally, read data with some pre- and post-pad, and for all stations
-        in the archive - this will be stored in `data.raw_waveforms`, while
-        `data.waveforms` will contain only data for selected stations between
-        `starttime` and `endtime`.
+        Optionally, read data with some pre- and post-pad, and for all stations in the
+        archive - this will be stored in `data.raw_waveforms`, while `data.waveforms`
+        will contain only data for selected stations between `starttime` and `endtime`.
 
         Parameters
         ----------
         starttime : `obspy.UTCDateTime` object
             Timestamp from which to read waveform data.
         endtime : `obspy.UTCDateTime` object
             Timestamp up to which to read waveform data.
@@ -247,24 +239,24 @@
             Additional pre pad of data to read. Defaults to 0.
         post_pad : float, optional
             Additional post pad of data to read. Defaults to 0.
 
         Returns
         -------
         data : :class:`~quakemigrate.io.data.WaveformData` object
-            Object containing the waveform data read from the archive that
-            satisfies the query.
+            Object containing the waveform data read from the archive that satisfies the
+            query.
 
         Raises
         ------
         ArchiveEmptyException
             If no data files are found in the archive for this day(s).
         DataAvailabilityException
-            If no data is found in the archive for the specified stations
-            within the specified time window.
+            If no data is found in the archive for the specified stations within the
+            specified time window.
 
         """
 
         # Ensure pre-pad and post-pad are not negative.
         pre_pad = max(0.0, pre_pad)
         post_pad = max(0.0, post_pad)
 
@@ -306,18 +298,17 @@
 
             # Merge waveforms channel-by-channel with no-clobber merge
             st = util.merge_stream(st)
 
             # Make copy of raw waveforms to output if requested
             data.raw_waveforms = st.copy()
 
-            # Ensure data is timestamped "on-sample" (i.e. an integer number
-            # of samples after midnight). Otherwise the data will be implicitly
-            # shifted when it is used to calculate the onset function /
-            # migrated.
+            # Ensure data is timestamped "on-sample" (i.e. an integer number of samples
+            # after midnight). Otherwise the data will be implicitly shifted when it is
+            # used to calculate the onset function / migrated.
             st = util.shift_to_sample(st, interpolate=self.interpolate)
 
             if self.read_all_stations:
                 # Re-populate st with only stations in station file
                 st_selected = Stream()
                 for station in self.stations:
                     st_selected += st.select(station=station)
@@ -394,52 +385,51 @@
             loadstart = UTCDateTime(loadstart.date) + 86400
 
         return files
 
 
 class WaveformData:
     """
-    The WaveformData class encapsulates the waveform data returned by an
-    Archive query.
+    The WaveformData class encapsulates the waveform data returned by an Archive query.
 
-    It also provides a number of utility functions. These include removing
-    instrument response and checking data availability against a flexible set
-    of data quality criteria.
+    It also provides a number of utility functions. These include removing instrument
+    response and checking data availability against a flexible set of data quality
+    criteria.
 
     Parameters
     ----------
     starttime : `obspy.UTCDateTime` object
         Timestamp of first sample of waveform data requested from the archive.
     endtime : `obspy.UTCDateTime` object
         Timestamp of last sample of waveform data requested from the archive.
     stations : `pandas.Series` object, optional
         Series object containing station names.
     read_all_stations : bool, optional
-        If True, `raw_waveforms` contain all stations in archive for that time
-        period. Else, only selected stations will be included.
+        If True, `raw_waveforms` contain all stations in archive for that time period.
+        Else, only selected stations will be included.
     resample : bool, optional
-        If true, allow resampling of data which cannot be decimated directly
-        to the desired sampling rate. See :func:`~quakemigrate.util.resample`
+        If true, allow resampling of data which cannot be decimated directly to the
+        desired sampling rate. See :func:`~quakemigrate.util.resample`
         Default: False
     upfactor : int, optional
-        Factor by which to upsample the data to enable it to be decimated to
-        the desired sampling rate, e.g. 40Hz -> 50Hz requires upfactor = 5.
+        Factor by which to upsample the data to enable it to be decimated to the desired
+        sampling rate, e.g. 40Hz -> 50Hz requires upfactor = 5.
         See :func:`~quakemigrate.util.resample`
     response_inv : `obspy.Inventory` object, optional
-        ObsPy response inventory for this waveform data, containing response
-        information for each channel of each station of each network.
+        ObsPy response inventory for this waveform data, containing response information
+        for each channel of each station of each network.
     pre_filt : tuple of floats
         Pre-filter to apply during the instrument response removal. E.g.
         (0.03, 0.05, 30., 35.) - all in Hz. (Default None)
     water_level : float
         Water level to use in instrument response removal. (Default 60.)
     remove_full_response : bool
-        Whether to remove the full response (including the effect of
-        digital FIR filters) or just the instrument transform function (as
-        defined by the PolesZeros Response Stage). Significantly slower.
+        Whether to remove the full response (including the effect of digital FIR
+        filters) or just the instrument transform function (as defined by the PolesZeros
+        Response Stage). Significantly slower.
         (Default False)
     pre_pad : float, optional
         Additional pre pad of data included in `raw_waveforms`.
     post_pad : float, optional
         Additional post pad of data included in `raw_waveforms`.
 
     Attributes
@@ -447,37 +437,35 @@
     starttime : `obspy.UTCDateTime` object
         Timestamp of first sample of waveform data requested from the archive.
     endtime : `obspy.UTCDateTime` object
         Timestamp of last sample of waveform data requested from the archive.
     stations : `pandas.Series` object
         Series object containing station names.
     read_all_stations : bool
-        If True, `raw_waveforms` contain all stations in archive for that time
-        period. Else, only selected stations will be included.
+        If True, `raw_waveforms` contain all stations in archive for that time period.
+        Else, only selected stations will be included.
     raw_waveforms : `obspy.Stream` object
-        Raw seismic data read in from the archive. This may be for all stations
-        in the archive, or only those specified by the user. See
-        `read_all_stations`. It may also cover the time period between
-        `starttime` and `endtime`, or feature an additional pre- and post-pad.
-        See `pre_pad` and `post_pad`.
+        Raw seismic data read in from the archive. This may be for all stations in the
+        archive, or only those specified by the user. See `read_all_stations`. It may
+        also cover the time period between `starttime` and `endtime`, or feature an
+        additional pre- and post-pad. See `pre_pad` and `post_pad`.
     waveforms : `obspy.Stream` object
-        Seismic data read in from the archive for the specified list of
-        stations, between `starttime` and `endtime`.
+        Seismic data read in from the archive for the specified list of stations,
+        between `starttime` and `endtime`.
     pre_pad : float
         Additional pre pad of data included in `raw_waveforms`.
     post_pad : float
         Additional post pad of data included in `raw_waveforms`.
 
     Methods
     -------
     check_availability(stream, **data_quality_params)
         Check data availability against a set of data quality criteria.
     get_wa_waveform(trace, **response_removal_params)
-        Calculate the Wood-Anderson corrected waveform for a `obspy.Trace`
-        object.
+        Calculate the Wood-Anderson corrected waveform for a `obspy.Trace` object.
 
     Raises
     ------
     NotImplementedError
         If the user attempts to use the get_real_waveform() method.
 
     """
@@ -528,60 +516,58 @@
         check_sampling_rate=False,
         sampling_rate=None,
         check_start_end_times=False,
     ):
         """
         Check waveform availability against data quality criteria.
 
-        There are a number of hard-coded checks: for whether any data is
-        present; for whether the data is a flatline (all samples have the same
-        value); and for whether the data contains overlaps. There are a
-        selection of additional optional checks which can be specified
-        according to the onset function / user preference.
+        There are a number of hard-coded checks: for whether any data is present; for
+        whether the data is a flatline (all samples have the same value); and for
+        whether the data contains overlaps. There are a selection of additional optional
+        checks which can be specified according to the onset function / user preference.
 
         Parameters
         ----------
         st : `obspy.Stream` object
-            Stream containing the waveform data to check against the
-            availability criteria.
+            Stream containing the waveform data to check against the availability
+            criteria.
         all_channels : bool, optional
-            Whether all supplied channels (distinguished by SEED id) need to
-            meet the availability criteria to mark the data as 'available'.
+            Whether all supplied channels (distinguished by SEED id) need to meet the
+            availability criteria to mark the data as 'available'.
         n_channels : int, optional
-            If `all_channels=True`, this argument is required (in order to
-            specify the number of channels expected to be present).
+            If `all_channels=True`, this argument is required (in order to specify the
+            number of channels expected to be present).
         allow_gaps : bool, optional
             Whether to allow gaps.
         full_timespan : bool, optional
-            Whether to ensure the data covers the entire timespan requested;
-            note that this implicitly requires that there be no gaps. Checks
-            the number of samples in the trace, not the start and end times;
-            for that see `check_start_end_times`.
+            Whether to ensure the data covers the entire timespan requested; note that
+            this implicitly requires that there be no gaps. Checks the number of samples
+            in the trace, not the start and end times; for that see
+            `check_start_end_times`.
         check_sampling_rate : bool, optional
             Check that all channels are at the desired sampling rate.
         sampling_rate : float, optional
-            If `check_sampling_rate=True`, this argument is required to specify
-            the sampling rate that the data should be at.
+            If `check_sampling_rate=True`, this argument is required to specify the
+            sampling rate that the data should be at.
         check_start_end_times : bool, optional
-            A stricter alternative to `full_timespan`; checks that the first
-            and last sample of the trace have exactly the requested timestamps.
+            A stricter alternative to `full_timespan`; checks that the first and last
+            sample of the trace have exactly the requested timestamps.
 
         Returns
         -------
         available : int
             0 if data doesn't meet the availability requirements; 1 if it does.
         availability : dict
-            Dict of {tr_id : available} for each unique SEED ID in the input
-            stream (available is again 0 or 1).
+            Dict of {tr_id : available} for each unique SEED ID in the input stream
+            (available is again 0 or 1).
 
         Raises
         ------
         TypeError
-            If the user specifies `all_channels=True` but does not specify
-            `n_channels`.
+            If the user specifies `all_channels=True` but does not specify `n_channels`.
 
         """
 
         availability = {}
         available = 0
         timespan = self.endtime - self.starttime
 
@@ -604,17 +590,16 @@
                     gaps = st_id.get_gaps()  # Overlaps already dealt with
                     if len(gaps) != 0:
                         continue
                 # Check sampling rate
                 if check_sampling_rate:
                     if not sampling_rate:
                         raise TypeError(
-                            "Please specify sampling_rate if you "
-                            "wish to check all channels are at the"
-                            " correct sampling rate."
+                            "Please specify sampling_rate if you wish to check all "
+                            "channels are at the correct sampling rate."
                         )
                     if any(tr.stats.sampling_rate != sampling_rate for tr in st_id):
                         continue
                 # Check data covers full timespan (if requested) - this
                 # strictly checks the *timespan*, so uses the trace sampling
                 # rate as provided. To check that as well, use
                 # `check_sampling_rate=True` and specify a sampling rate.
@@ -640,71 +625,67 @@
             # Return availability based on "all_channels" setting
             if all(ava == 1 for ava in availability.values()):
                 if all_channels:
                     # If all_channels requested, must also check that the
                     # expected number of channels are present
                     if not n_channels:
                         raise TypeError(
-                            "Please specify n_channels if you wish"
-                            " to check all channels meet the "
-                            "availability criteria."
+                            "Please specify n_channels if you wish to check all "
+                            "channels meet the availability criteria."
                         )
                     elif len(availability) == n_channels:
                         available = 1
                 else:
                     available = 1
             elif not all_channels and any(ava == 1 for ava in availability.values()):
                 available = 1
 
         return available, availability
 
     def get_real_waveform(self, tr, velocity=True):
         """
-        Calculate the real waveform for a Trace by removing the instrument
-        response.
+        Calculate the real waveform for a Trace by removing the instrument response.
 
         Parameters
         ----------
         tr : `obspy.Trace` object
-            Trace containing the waveform for which to remove the instrument
-            response.
+            Trace containing the waveform for which to remove the instrument response.
         velocity : bool, optional
             Output velocity waveform (as opposed to displacement).
             Default: True.
 
         Returns
         -------
         tr : `obspy.Trace` object
             Trace with instrument response removed.
 
         Raises
         ------
         AttributeError
             If no response inventory has been supplied.
         ResponseNotFoundError
-            If the response information for a trace can't be found in the
-            supplied response inventory.
+            If the response information for a trace can't be found in the supplied
+            response inventory.
         ResponseRemovalError
             If the deconvolution of the instrument response is unsuccessful.
 
         """
 
         if not self.response_inv:
             raise AttributeError("No response inventory provided!")
 
         # Copy the Trace before operating on it
         tr = tr.copy()
         tr.detrend("linear")
 
         if not self.remove_full_response:
-            # Just remove the response encapsulated in the instrument transfer
-            # function (stored as a PolesAndZeros response). NOTE: this does
-            # not account for the effect of the digital FIR filters applied to
-            # the recorded waveforms. However, due to this it is significantly
-            # faster to compute.
+            # Just remove the response encapsulated in the instrument transfer function
+            # (stored as a PolesAndZeros response). NOTE: this does not account for the
+            # effect of the digital FIR filters applied to the recorded waveforms.
+            # However, due to this it is significantly faster to compute.
             try:
                 response = self.response_inv.get_response(tr.id, tr.stats.starttime)
             except Exception as e:
                 raise util.ResponseNotFoundError(str(e), tr.id)
 
             # Get the instrument transfer function as a PAZ dictionary
             paz = response.get_paz()
@@ -722,21 +703,21 @@
             try:
                 tr.simulate(
                     paz_remove=paz_dict,
                     pre_filt=self.pre_filt,
                     water_level=self.water_level,
                     taper=True,
                     sacsim=True,  # To replicate remove_response()
-                    pitsasim=False,   # To replicate remove_response()
+                    pitsasim=False,  # To replicate remove_response()
                 )
             except ValueError as e:
                 raise util.ResponseRemovalError(e, tr.id)
         else:
-            # Use remove_response(), which removes the effect of _all_ response
-            # stages, including the FIR stages. Considerably slower.
+            # Use remove_response(), which removes the effect of _all_ response stages,
+            # including the FIR stages. Considerably slower.
             output = "VEL" if velocity else "DISP"
 
             try:
                 tr.remove_response(
                     inventory=self.response_inv,
                     output=output,
                     pre_filt=self.pre_filt,
@@ -757,20 +738,19 @@
     def get_wa_waveform(self, tr, velocity=False):
         """
         Calculate simulated Wood Anderson displacement waveform for a Trace.
 
         Parameters
         ----------
         tr : `obspy.Trace` object
-            Trace containing the waveform to be corrected to a Wood-Anderson
-            response
+            Trace containing the waveform to be corrected to a Wood-Anderson response.
         velocity : bool, optional
             Output velocity waveform, instead of displacement. Default: False.
-            NOTE: all attenuation functions provided within the QM local_mags
-            module are calculated for displacement seismograms.
+            NOTE: all attenuation functions provided within the QM local_mags module are
+            calculated for displacement seismograms.
 
         Returns
         -------
         tr : `obspy.Trace` object
             Trace corrected to Wood-Anderson response.
 
         """
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quakemigrate-1.0.1/quakemigrate/io/event.py` & `quakemigrate-1.0.2/quakemigrate/io/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """
-Module containing the Event class, which stores information related to an
-individual event.
+Module containing the Event class, which stores information related to an individual
+event.
 
 :copyright:
-    2020 - 2021, QuakeMigrate developers.
+    2020–2023, QuakeMigrate developers.
 :license:
     GNU General Public License, Version 3
     (https://www.gnu.org/licenses/gpl-3.0.html)
 
 """
 
 import logging
@@ -16,35 +16,50 @@
 import numpy as np
 from obspy import Trace
 import pandas as pd
 
 import quakemigrate.util as util
 
 
-EVENT_FILE_COLS = ["EventID", "DT", "X", "Y", "Z", "COA", "COA_NORM",
-                   "GAU_X", "GAU_Y", "GAU_Z",
-                   "GAU_ErrX", "GAU_ErrY", "GAU_ErrZ",
-                   "COV_ErrX", "COV_ErrY", "COV_ErrZ",
-                   "TRIG_COA", "DEC_COA", "DEC_COA_NORM"]
+EVENT_FILE_COLS = [
+    "EventID",
+    "DT",
+    "X",
+    "Y",
+    "Z",
+    "COA",
+    "COA_NORM",
+    "GAU_X",
+    "GAU_Y",
+    "GAU_Z",
+    "GAU_ErrX",
+    "GAU_ErrY",
+    "GAU_ErrZ",
+    "COV_ErrX",
+    "COV_ErrY",
+    "COV_ErrZ",
+    "TRIG_COA",
+    "DEC_COA",
+    "DEC_COA_NORM",
+]
 
 XYZ, ERR_XYZ = ["X", "Y", "Z"], ["ErrX", "ErrY", "ErrZ"]
 
 
 class Event:
     """
-    Light class to encapsulate information about an event, including waveform
-    data, coalescence information, origin time, locations, picks, magnitudes.
+    Light class to encapsulate information about an event, including waveform data,
+    coalescence information, origin time, locations, picks, magnitudes.
 
     Parameters
     ----------
     marginal_window : float
-        Estimate of the uncertainty in the event origin time; time window
-        over which the 4-D coalescence image is marginalised around the peak
-        coalescence time (event origin time) to produce the 3-D coalescence
-        map.
+        Estimate of the uncertainty in the event origin time; time window over which the
+        4-D coalescence image is marginalised around the peak coalescence time (event
+        origin time) to produce the 3-D coalescence map.
     triggered_event : `pandas.Series` object, optional
         Contains information on the candidate event identified by
         :func:`~quakemigrate.signal.trigger.Trigger.trigger`
 
     Attributes
     ----------
     coa_data : `pandas.DataFrame` object
@@ -52,101 +67,99 @@
         DT : `numpy.ndarray` of `obspy.UTCDateTime` objects, shape(nsamples)
             Timestamps for the coalescence data.
         COA : `numpy.ndarray` of floats, shape(nsamples)
             Max coalescence value in the grid at each timestep.
         COA_NORM : `numpy.ndarray` of floats, shape(nsamples)
             Normalised max coalescence value in the grid at each timestep.
         X : `numpy.ndarray` of floats, shape(nsamples)
-            X coordinate of maximum coalescence value in the grid at each
-            timestep, in input (geographic) projection coordinates.
+            X coordinate of maximum coalescence value in the grid at each timestep, in
+            input (geographic) projection coordinates.
         Y : `numpy.ndarray` of floats, shape(nsamples)
-            Y coordinate of maximum coalescence value in the grid at each
-            timestep, in input (geographic) projection coordinates.
+            Y coordinate of maximum coalescence value in the grid at each timestep, in
+            input (geographic) projection coordinates.
         Z : `numpy.ndarray` of floats, shape(nsamples)
-            Z coordinate of maximum coalescence value in the grid at each
-            timestep, in input (geographic) projection coordinates.
+            Z coordinate of maximum coalescence value in the grid at each timestep, in
+            input (geographic) projection coordinates.
     data : :class:`~quakemigrate.io.data.WaveformData` object
         Light class encapsulating waveform data returned from an archive query.
     hypocentre : `numpy.ndarray` of floats
         [X, Y, Z]; Geographical coordinates of the event hypocentre (default is
         interpolated peak of a spline function fitted to the marginalised 3-D
         coalescence map).
     locations : dict
         Information on the various locations and reported uncertainties.\n
         spline : dict
             The location of the peak coalescence value in the marginalised 3-D
-            coalescence map, interpolated using a 3-D spline. If no spline fit
-            was able to be made, it is just the gridded peak location.
+            coalescence map, interpolated using a 3-D spline. If no spline fit was able
+            to be made, it is just the gridded peak location.
         gaussian : dict
-            The location and uncertainty as determined by fitting a 3-D
-            Gaussian to the marginalised 3-D coalescence map in a small region
-            around the (gridded) peak coalescence location.
+            The location and uncertainty as determined by fitting a 3-D Gaussian to the
+            marginalised 3-D coalescence map in a small region around the (gridded) peak
+            coalescence location.
         covariance : dict
-            The location and uncertainty as determined by calculating the
-            covariance of the coalescence values in X, Y, and Z above some
-            percentile of the max coalescence value in the marginalised 3-D
-            coalescence map.
+            The location and uncertainty as determined by calculating the covariance of
+            the coalescence values in X, Y, and Z above some percentile of the max
+            coalescence value in the marginalised 3-D coalescence map.
     map4d : `numpy.ndarray`, shape(nx, ny, nz, nsamp), optional
         4-D coalescence map generated in
         :func:`~quakemigrate.signal.scan.QuakeScan.locate`.
     max_coalescence : dict
-        Dictionary containing the raw and normalised maximum coalescence values
-        in the 3-D grid at the timestamp corresponding to the instantaneous
-        (non-marginalised) maximum coalescence value in the 4-D grid (i.e.
-        the event origin time).
+        Dictionary containing the raw and normalised maximum coalescence values in the
+        3-D grid at the timestamp corresponding to the instantaneous (non-marginalised)
+        maximum coalescence value in the 4-D grid (i.e. the event origin time).
     onset_data : :class:`~quakemigrate.signal.onsets.base.OnsetData` object
         Light class encapsulating data generated during onset calculation.
     otime : `obspy.UTCDateTime` object
-        Timestamp of the instantaneous peak in the 4-D coalescence function
-        generated in :func:`~quakemigrate.signal.scan.QuakeScan.locate` - best
-        estimate of the event origin time.
+        Timestamp of the instantaneous peak in the 4-D coalescence function generated in
+        :func:`~quakemigrate.signal.scan.QuakeScan.locate` - best estimate of the event
+        origin time.
     trigger_info : dict
         Useful information about the triggered event to be fed forward.\n
         TRIG_COA : float
             The peak value of the coalescence stream used to trigger the event.
         DEC_COA : float
-            The coalescence value of the "raw" maximum coalsecence stream
-            at the `trigger_time`.
+            The coalescence value of the "raw" maximum coalsecence stream at the
+            `trigger_time`.
         DEC_COA_NORM : float
-            The coalescence value of the normalised maximum coalsecence stream
-            at the `trigger_time`.
+            The coalescence value of the normalised maximum coalsecence stream at the
+            `trigger_time`.
     trigger_time : `obspy.UTCDateTime` object
-        The time of the peak in the continuous coalescence stream (output by
-        detect) corresponding to the triggered event.
+        The time of the peak in the continuous coalescence stream (output by detect)
+        corresponding to the triggered event.
     uid : str
         A unique identifier for the event based on the event trigger time.
 
     Methods
     -------
     add_compute_output(times, max_coa, max_coa_n, coord, map4d, onset_data)
-        Add values returned by
-        :func:`~quakemigrate.signal.scan.QuakeScan._compute` to the event.
+        Add values returned by :func:`~quakemigrate.signal.scan.QuakeScan._compute` to
+        the event.
     add_covariance_location(xyz, xyz_unc)
         Add the covariance location and uncertainty to the event.
     add_gaussian_location(xyz, xyz_unc)
         Add the gaussian location and uncertainty to the event.
     add_spline_location(xyz)
         Add the spline-interpolated location to the event.
     add_picks(pick_df)
         Add phase picks to the event.
     add_local_magnitude(mag, mag_err, mag_r2)
         Add local magnitude to the event.
     add_waveform_data(data)
         Add waveform data read from the archive to the event (as a
         :class:`~quakemigrate.io.data.WaveformData` object).
     in_marginal_window(marginal_window)
-        Simple test to see if event is within the marginal window around the
-        event origin time (time of max instantaneous coalescence value).
+        Simple test to see if event is within the marginal window around the event
+        origin time (time of max instantaneous coalescence value).
     mw_times(marginal_window, sampling_rate)
-        Generates timestamps for data in the window around the event trigger
-        scanned by :func:`~quakemigrate.signal.scan.QuakeScan._compute`;
+        Generates timestamps for data in the window around the event trigger scanned by
+        :func:`~quakemigrate.signal.scan.QuakeScan._compute`;
         `trigger_time` +/- 2*`marginal_window`.
     trim2window(marginal_window)
-        Trim the coalescence data and `map4d` to the marginal window about the
-        event origin time.
+        Trim the coalescence data and `map4d` to the marginal window about the event
+        origin time.
     write(run)
         Output the event to a .event file.
     get_hypocentre(method)
         Get the event hypocentre estimate calculated by a specific method;
         {"gaussian", "covariance", "spline"}.
 
     """
@@ -168,61 +181,63 @@
         self.otime = None
         self.locations = {}
         self.picks = {}
         self.localmag = {}
 
     def add_waveform_data(self, data):
         """
-        Add waveform data in the form of a
-        :class:`~quakemigrate.io.data.WaveformData` object.
+        Add waveform data in the form of a :class:`~quakemigrate.io.data.WaveformData`
+        object.
 
         Parameters
         ----------
         data : :class:`~quakemigrate.io.data.WaveformData` object
-            Contains cut waveforms - `raw_waveforms` may be for all stations
-            in the archive, and include an additional pre- and post-pad;
-            `waveforms` contains data only for the stations and time period
-            required for migration.
+            Contains cut waveforms - `raw_waveforms` may be for all stations in the
+            archive, and include an additional pre- and post-pad; `waveforms` contains
+            data only for the stations and time period required for migration.
 
         """
 
         self.data = data
 
-    def add_compute_output(self, times, max_coa, max_coa_n, coord, map4d,
-                           onset_data):
+    def add_compute_output(self, times, max_coa, max_coa_n, coord, map4d, onset_data):
         """
-        Append outputs of compute to the Event object. This includes time
-        series of the maximum coalescence values in the 3-D grid at each
-        timestep, and their locations, the full 4-D coalescence map, and the
-        onset data generated for migration.
+        Append outputs of compute to the Event object. This includes time series of the
+        maximum coalescence values in the 3-D grid at each timestep, and their
+        locations, the full 4-D coalescence map, and the onset data generated for
+        migration.
 
         Parameters
         ----------
         times : `numpy.ndarray` of `obspy.UTCDateTime` objects, shape(nsamples)
             Timestamps for the coalescence data.
         max_coa : `numpy.ndarray` of floats, shape(nsamples)
             Max coalescence value in the grid at each timestep.
         max_coa_n : `numpy.ndarray` of floats, shape(nsamples)
             Normalised max coalescence value in the grid at each timestep.
         coord : `numpy.ndarray` of floats, shape(nsamples, 3)
-            [x, y, z] Location of maximum coalescence in the grid at each
-            timestep, in input (geographic) projection coordinates
+            [x, y, z] Location of maximum coalescence in the grid at each timestep, in
+            input (geographic) projection coordinates
         map4d : `numpy.ndarry`, shape(nx, ny, nz, nsamp)
             4-D coalescence map.
         onset_data : :class:`~quakemigrate.signal.onsets.base.OnsetData` object
             Light class encapsulating data generated during onset calculation.
 
         """
 
-        self.coa_data = pd.DataFrame({"DT": times,
-                                      "COA": max_coa,
-                                      "COA_NORM": max_coa_n,
-                                      "X": coord[:, 0],
-                                      "Y": coord[:, 1],
-                                      "Z": coord[:, 2]})
+        self.coa_data = pd.DataFrame(
+            {
+                "DT": times,
+                "COA": max_coa,
+                "COA_NORM": max_coa_n,
+                "X": coord[:, 0],
+                "Y": coord[:, 1],
+                "Z": coord[:, 2],
+            }
+        )
         self.map4d = map4d
         idxmax = self.coa_data["COA"].astype(float).idxmax()
         self.otime = self.coa_data.iloc[idxmax]["DT"]
 
         self.onset_data = onset_data
 
     def add_covariance_location(self, xyz, xyz_unc):
@@ -231,52 +246,56 @@
         marginalised coalescence map filtered above a percentile threshold.
 
         Parameters
         ----------
         xyz : `numpy.ndarray` of floats, shape(3)
             Geographical coordinates (lon/lat/depth) of covariance location.
         xyz_unc : `numpy.ndarray' of floats, shape(3)
-            One sigma uncertainties on the covariance location (units
-            determined by the LUT projection units).
+            One sigma uncertainties on the covariance location (units determined by the
+            LUT projection units).
 
         """
 
-        self.locations["covariance"] = {"X": xyz[0],
-                                        "Y": xyz[1],
-                                        "Z": xyz[2],
-                                        "ErrX": xyz_unc[0],
-                                        "ErrY": xyz_unc[1],
-                                        "ErrZ": xyz_unc[2]}
+        self.locations["covariance"] = {
+            "X": xyz[0],
+            "Y": xyz[1],
+            "Z": xyz[2],
+            "ErrX": xyz_unc[0],
+            "ErrY": xyz_unc[1],
+            "ErrZ": xyz_unc[2],
+        }
 
     def add_gaussian_location(self, xyz, xyz_unc):
         """
-        Add the location determined by fitting a 3-D Gaussian to a small window
-        around the Gaussian smoothed maximum coalescence location.
+        Add the location determined by fitting a 3-D Gaussian to a small window around
+        the Gaussian smoothed maximum coalescence location.
 
         Parameters
         ----------
         xyz : `numpy.ndarray` of floats, shape(3)
             Geographical coordinates (lon/lat/depth) of Gaussian location.
         xyz_unc : `numpy.ndarray' of floats, shape(3)
-            One sigma uncertainties on the Gaussian location (units determined
-            by the LUT projection units).
+            One sigma uncertainties on the Gaussian location (units determined by the
+            LUT projection units).
 
         """
 
-        self.locations["gaussian"] = {"X": xyz[0],
-                                      "Y": xyz[1],
-                                      "Z": xyz[2],
-                                      "ErrX": xyz_unc[0],
-                                      "ErrY": xyz_unc[1],
-                                      "ErrZ": xyz_unc[2]}
+        self.locations["gaussian"] = {
+            "X": xyz[0],
+            "Y": xyz[1],
+            "Z": xyz[2],
+            "ErrX": xyz_unc[0],
+            "ErrY": xyz_unc[1],
+            "ErrZ": xyz_unc[2],
+        }
 
     def add_spline_location(self, xyz):
         """
-        Add the location determined by fitting a 3-D spline to a small window
-        around the maximum coalescence location and interpolating.
+        Add the location determined by fitting a 3-D spline to a small window around the
+        maximum coalescence location and interpolating.
 
         Parameters
         ----------
         xyz : `numpy.ndarray` of floats, shape(3)
             Geographical coordinates (lon/lat/depth) of best-fitting location.
 
         """
@@ -322,134 +341,143 @@
         Add outputs from local magnitude calculation to the Event object.
 
         Parameters
         ----------
         mag : float
             Network-averaged local magnitude estimate for the event.
         mag_err : float
-            (Weighted) standard deviation of the magnitude estimates from
-            amplitude measurements on individual stations/channels.
+            (Weighted) standard deviation of the magnitude estimates from amplitude
+            measurements on individual stations/channels.
         mag_r2 : float
-            r-squared statistic describing the fit of the amplitude vs.
-            distance curve predicted by the calculated mean_mag and chosen
-            attenuation model to the measured amplitude observations. This is
-            intended to be used to help discriminate between 'real' events, for
-            which the predicted amplitude vs. distance curve should provide a
-            good fit to the observations, from artefacts, which in general will
-            not.
+            r-squared statistic describing the fit of the amplitude vs. distance curve
+            predicted by the calculated mean_mag and chosen attenuation model to the
+            measured amplitude observations. This is intended to be used to help
+            discriminate between 'real' events, for which the predicted amplitude vs.
+            distance curve should provide a good fit to the observations, from
+            artefacts, which in general will not.
 
         """
 
         self.localmag["ML"] = mag
         self.localmag["ML_Err"] = mag_err
         self.localmag["ML_r2"] = mag_r2
 
     def in_marginal_window(self):
         """
-        Test if triggered event time is within marginal window around
-        the maximum coalescence time (origin time).
+        Test if triggered event time is within marginal window around the maximum
+        coalescence time (origin time).
 
         Returns
         -------
         cond : bool
             Result of test.
 
         """
 
         window_start = self.otime - self.marginal_window
         window_end = self.otime + self.marginal_window
-        cond = (self.trigger_time > window_start
-                and self.trigger_time < window_end)
+        cond = self.trigger_time > window_start and self.trigger_time < window_end
         if not cond:
             logging.info(f"\tEvent {self.uid} is outside marginal window.")
-            logging.info("\tDefine more realistic error - the marginal "
-                         "window should be an estimate of overall uncertainty")
-            logging.info("\tdetermined from expected spatial uncertainty"
-                         " and uncertainty in the seismic velocity model.\n")
+            logging.info(
+                "\tDefine more realistic error - the marginal window should be an "
+                "estimate of overall uncertainty"
+            )
+            logging.info(
+                "\tdetermined from expected spatial uncertainty and uncertainty in the "
+                "seismic velocity model.\n"
+            )
             logging.info(util.log_spacer)
 
         return cond
 
     def mw_times(self, sampling_rate):
         """
-        Utility function to generate timestamps for the time period around the
-        trigger time for which the 4-D coalescence function is calculated in
+        Utility function to generate timestamps for the time period around the trigger
+        time for which the 4-D coalescence function is calculated in
         :func:`~quakemigrate.signal.scan.QuakeScan._compute`.
 
         Returns
         -------
         times : `numpy.ndarray` of `obspy.UTCDateTime`, shape(nsamples)
             Timestamps for time range `trigger_time` +/- 2 * `marginal_window`.
 
         """
 
         # Utilise the .times() method of `obspy.Trace` objects
-        tr = Trace(header={
-            "npts": 4 * self.marginal_window * sampling_rate + 1,
-            "sampling_rate": sampling_rate,
-            "starttime": self.trigger_time - 2 * self.marginal_window})
+        tr = Trace(
+            header={
+                "npts": 4 * self.marginal_window * sampling_rate + 1,
+                "sampling_rate": sampling_rate,
+                "starttime": self.trigger_time - 2 * self.marginal_window,
+            }
+        )
         return tr.times(type="utcdatetime")
 
     def trim2window(self):
         """
         Trim the coalescence data to be within the marginal window.
 
         """
 
         window_start = self.otime - self.marginal_window
         window_end = self.otime + self.marginal_window
 
-        self.coa_data = self.coa_data[(self.coa_data["DT"] >= window_start) &
-                                      (self.coa_data["DT"] <= window_end)]
-        self.map4d = self.map4d[:, :, :,
-                                self.coa_data.index[0]:self.coa_data.index[-1]]
+        self.coa_data = self.coa_data[
+            (self.coa_data["DT"] >= window_start) & (self.coa_data["DT"] <= window_end)
+        ]
+        self.map4d = self.map4d[
+            :, :, :, self.coa_data.index[0] : self.coa_data.index[-1]
+        ]
         self.coa_data.reset_index(drop=True, inplace=True)
 
         idxmax = self.coa_data["COA"].astype(float).idxmax()
         self.otime = self.coa_data.iloc[idxmax]["DT"]
 
     def write(self, run, lut):
         """
         Write event to a .event file.
 
         Parameters
         ----------
         run : :class:`~quakemigrate.io.core.Run` object
             Light class encapsulating i/o path information for a given run.
         lut : :class:`~quakemigrate.lut.lut.LUT` object
-            Contains the traveltime lookup tables for seismic phases, computed
-            for some pre-defined velocity model.
+            Contains the traveltime lookup tables for seismic phases, computed for some
+            pre-defined velocity model.
 
         """
 
         fpath = run.path / "locate" / run.subname / "events"
         fpath.mkdir(exist_ok=True, parents=True)
 
         out = {"EventID": self.uid, **self.trigger_info, **self.localmag}
         out = {**out, **self.max_coalescence}
 
         # Rename keys for locations; do not output covariance loc (just err)
         loc = self.locations["spline"]
-        gau = dict((f"GAU_{key}", value) for (key, value)
-                   in self.locations["gaussian"].items())
-        cov = dict((f"COV_{key}", value) for (key, value)
-                   in list(self.locations["covariance"].items())[3:])
+        gau = dict(
+            (f"GAU_{key}", value) for (key, value) in self.locations["gaussian"].items()
+        )
+        cov = dict(
+            (f"COV_{key}", value)
+            for (key, value) in list(self.locations["covariance"].items())[3:]
+        )
         out = {**out, **loc, **gau, **cov}
 
         if self.localmag.get("ML") is not None:
             event_file_cols = EVENT_FILE_COLS + ["ML", "ML_Err", "ML_r2"]
         else:
             event_file_cols = EVENT_FILE_COLS
 
         event_df = pd.DataFrame([out])[event_file_cols]
 
         # Set floating point precision for COA values
         for col in event_df.filter(like="COA").columns:
-            event_df[col] = event_df[col].map(lambda x: f"{x:.4g}",
-                                              na_action="ignore")
+            event_df[col] = event_df[col].map(lambda x: f"{x:.4g}", na_action="ignore")
 
         # Set floating point precision for locations & loc uncertainties
         for axis_precision, axis in zip(lut.precision, XYZ):
             # Sort out which columns to format
             cols = [axis, f"GAU_{axis}"]
             if axis == "Z":
                 unit_correction = 3 if lut.unit_name == "km" else 0
@@ -461,35 +489,36 @@
                 event_df[col] = event_df.loc[:, col].round(decimals=decimals)
                 if decimals <= 0:
                     event_df[col] = event_df.loc[:, col].astype(int)
 
         # Set floating point precision for mags (if applicable)
         if self.localmag.get("ML") is not None:
             for col in ["ML", "ML_Err", "ML_r2"]:
-                event_df[col] = event_df[col].map(lambda x: f"{x:.3g}",
-                                                  na_action="ignore")
+                event_df[col] = event_df[col].map(
+                    lambda x: f"{x:.3g}", na_action="ignore"
+                )
 
         fstem = f"{self.uid}"
         file = (fpath / fstem).with_suffix(".event")
         event_df.to_csv(file, index=False)
 
     def get_hypocentre(self, method="spline"):
         """
         Get an estimate of the event hypocentre location.
 
         Parameters
         ----------
         method : {"spline", "gaussian", "covariance"}, optional
-            Which location result to return. (Default "spline")
+            Which location result to return. (Default "spline").
 
         Returns
         -------
         ev_loc : `numpy.ndarray` of floats
-            [x_coordinate, y_coordinate, z_coordinate] of event hypocentre, in
-            the global (geographic) coordinate system.
+            [x_coordinate, y_coordinate, z_coordinate] of event hypocentre, in the
+            global (geographic) coordinate system.
 
         """
 
         hypocentre = self.locations[method]
 
         ev_loc = np.array([hypocentre[k] for k in XYZ])
 
@@ -500,21 +529,21 @@
     def get_loc_uncertainty(self, method="gaussian"):
         """
         Get an estimate of the hypocentre location uncertainty.
 
         Parameters
         ----------
         method : {"gaussian", "covariance"}, optional
-            Which location result to return. (Default "gaussian")
+            Which location result to return. (Default "gaussian").
 
         Returns
         -------
         ev_loc_unc : `numpy.ndarray` of floats
-            [x_uncertainty, y_uncertainty, z_uncertainty] of event hypocentre;
-            units are determined by the LUT projection units.
+            [x_uncertainty, y_uncertainty, z_uncertainty] of event hypocentre; units are
+            determined by the LUT projection units.
 
         """
 
         loc = self.locations[method]
 
         ev_loc_unc = np.array([loc[k] for k in ERR_XYZ])
 
@@ -538,33 +567,39 @@
         max_coa = self.coa_data.iloc[idxmax]
         keys = ["DT", "COA", "COA_NORM"]
 
         return dict(zip(keys, max_coa[keys].values))
 
     def _parse_triggered_event(self, event_data):
         """
-        Parse the information from a triggered event `pandas.Series` object
-        into the Event object.
+        Parse the information from a triggered event `pandas.Series` object into the
+        Event object.
 
         Parameters
         ----------
         event_data : `~pandas.Series` object
             Contains information on the event output by the trigger stage.
 
         """
 
         try:
-            trigger_info = {"TRIG_COA": event_data["TRIG_COA"],
-                            "DEC_COA": event_data["COA"],
-                            "DEC_COA_NORM": event_data["COA_NORM"]}
+            trigger_info = {
+                "TRIG_COA": event_data["TRIG_COA"],
+                "DEC_COA": event_data["COA"],
+                "DEC_COA_NORM": event_data["COA_NORM"],
+            }
         except KeyError:
             # --- Backwards compatibility ---
             try:
-                trigger_info = {"TRIG_COA": event_data["COA_V"],
-                                "DEC_COA": event_data["COA"],
-                                "DEC_COA_NORM": event_data["COA_NORM"]}
+                trigger_info = {
+                    "TRIG_COA": event_data["COA_V"],
+                    "DEC_COA": event_data["COA"],
+                    "DEC_COA_NORM": event_data["COA_NORM"],
+                }
             except KeyError:
-                trigger_info = {"TRIG_COA": event_data["COA_V"],
-                                "DEC_COA": np.nan,
-                                "DEC_COA_NORM": np.nan}
+                trigger_info = {
+                    "TRIG_COA": event_data["COA_V"],
+                    "DEC_COA": np.nan,
+                    "DEC_COA_NORM": np.nan,
+                }
 
         return trigger_info
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quakemigrate-1.0.1/quakemigrate/io/scanmseed.py` & `quakemigrate-1.0.2/quakemigrate/io/scanmseed.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 Module to handle input/output of .scanmseed files.
 
 :copyright:
-    2020 - 2021, QuakeMigrate developers.
+    2020–2023, QuakeMigrate developers.
 :license:
     GNU General Public License, Version 3
     (https://www.gnu.org/licenses/gpl-3.0.html)
 
 """
 
 import logging
@@ -18,50 +18,48 @@
 import pandas as pd
 
 import quakemigrate.util as util
 
 
 class ScanmSEED:
     """
-    Light class to encapsulate the data output by the detect stage of
-    QuakeMigrate. This data is stored in an `obspy.Stream` object with the
-    channels: ["COA", "COA_N", "X", "Y", "Z"].
+    Light class to encapsulate the data output by the detect stage of QuakeMigrate. This
+    data is stored in an `obspy.Stream` object with the channels:
+    ["COA", "COA_N", "X", "Y", "Z"].
 
     Parameters
     ----------
     run : :class:`~quakemigrate.io.core.Run` object
         Light class encapsulating i/o path information for a given run.
     continuous_write : bool
         Option to continuously write the .scanmseed file output by
-        :func:`~quakemigrate.signal.scan.QuakeScan.detect()` at the end of
-        every time step. Default behaviour is to write in day chunks where
-        possible.
+        :func:`~quakemigrate.signal.scan.QuakeScan.detect()` at the end of every time
+        step. Default behaviour is to write in day chunks where possible.
     sampling_rate : int
-        Desired sampling rate of input data; sampling rate at which to compute
-        the coalescence function. Default: 50 Hz.
+        Desired sampling rate of input data; sampling rate at which to compute the
+        coalescence function. Default: 50 Hz.
 
     Attributes
     ----------
     stream : `obspy.Stream` object
-        Output of :func:`~quakemigrate.signal.scan.QuakeScan.detect()` stored
-        in `obspy.Stream` object. The values have been multiplied by a factor
-        to make use of more efficient compression.
+        Output of :func:`~quakemigrate.signal.scan.QuakeScan.detect()` stored in
+        `obspy.Stream` object. The values have been multiplied by a factor to make use
+        of more efficient compression.
         Channels: ["COA", "COA_N", "X", "Y", "Z"]
     written : bool
         Tracker for whether the data appended has been written recently.
 
     Methods
     -------
     append(times, max_coa, max_coa_n, coord, map4d=None)
-        Append the output of
-        :func:`~quakemigrate.signal.scan.QuakeScan._compute()` to the
-        coalescence stream.
+        Append the output of :func:`~quakemigrate.signal.scan.QuakeScan._compute()` to
+        the coalescence stream.
     empty(starttime, timestep, i, msg)
-        Create an set of empty arrays for a given timestep and append to the
-        coalescence stream.
+        Create an set of empty arrays for a given timestep and append to the coalescence
+        stream.
     write(write_start=None, write_end=None)
         Write the coalescence stream to a .scanmseed file.
 
     """
 
     def __init__(self, run, continuous_write, sampling_rate):
         """Instantiate the ScanmSEED object."""
@@ -71,62 +69,69 @@
         self.sampling_rate = sampling_rate
 
         self.written = False
         self.stream = Stream()
 
     def append(self, starttime, max_coa, max_coa_n, coord, ucf):
         """
-        Append latest timestep of
-        :func:`~quakemigrate.signal.scan.QuakeScan.detect()` output to
-        `obspy.Stream` object.
+        Append latest timestep of :func:`~quakemigrate.signal.scan.QuakeScan.detect()`
+        output to `obspy.Stream` object.
 
         Multiply channels ["COA", "COA_N", "X", "Y", "Z"] by factors of
-        ["1e5", "1e5", "1e6", "1e6", "1e3"] respectively, round and convert to
-        int32 as this dramatically reduces memory usage, and allows the
-        coastream data to be saved in mSEED format with STEIM2 compression.
-        The multiplication factor is removed when the data is read back in.
+        ["1e5", "1e5", "1e6", "1e6", "1e3"] respectively, round and convert to int32 as
+        this dramatically reduces memory usage, and allows the coastream data to be
+        saved in mSEED format with STEIM2 compression. The multiplication factor is
+        removed when the data is read back in.
 
         Parameters
         ----------
         starttime : `obspy.UTCDateTime` object
             Timestamp of first sample of coalescence data.
         max_coa : `numpy.ndarray` of floats, shape(nsamples)
             Coalescence value through time.
         max_coa_n : `numpy.ndarray` of floats, shape(nsamples)
             Normalised coalescence value through time.
         coord : `numpy.ndarray` of floats, shape(nsamples)
-            Location of maximum coalescence through time in input projection
-            space.
+            Location of maximum coalescence through time in input projection space.
         ucf : float
-            A conversion factor based on the lookup table grid projection. Used
-            to ensure the same level of precision (millimetre) is retained
-            during compression, irrespective of the units of the grid
-            projection.
+            A conversion factor based on the lookup table grid projection. Used to
+            ensure the same level of precision (millimetre) is retained during
+            compression, irrespective of the units of the grid projection.
 
         """
 
         # Clip max value of COA to prevent int overflow
-        max_coa[max_coa > 21474.] = 21474.
-        max_coa_n[max_coa_n > 21474.] = 21474.
+        max_coa[max_coa > 21474.0] = 21474.0
+        max_coa_n[max_coa_n > 21474.0] = 21474.0
 
-        meta = {"network": "NW",
-                "npts": len(max_coa) - 1,
-                "sampling_rate": self.sampling_rate,
-                "starttime": starttime}
-
-        self.stream += Trace(data=self._data2int(max_coa[:-1], 1e5),
-                             header={**{"station": "COA"}, **meta})
-        self.stream += Trace(data=self._data2int(max_coa_n[:-1], 1e5),
-                             header={**{"station": "COA_N"}, **meta})
-        self.stream += Trace(data=self._data2int(coord[:-1, 0], 1e6),
-                             header={**{"station": "X"}, **meta})
-        self.stream += Trace(data=self._data2int(coord[:-1, 1], 1e6),
-                             header={**{"station": "Y"}, **meta})
-        self.stream += Trace(data=self._data2int(coord[:-1, 2], 1e3*ucf),
-                             header={**{"station": "Z"}, **meta})
+        meta = {
+            "network": "NW",
+            "npts": len(max_coa) - 1,
+            "sampling_rate": self.sampling_rate,
+            "starttime": starttime,
+        }
+
+        self.stream += Trace(
+            data=self._data2int(max_coa[:-1], 1e5),
+            header={**{"station": "COA"}, **meta},
+        )
+        self.stream += Trace(
+            data=self._data2int(max_coa_n[:-1], 1e5),
+            header={**{"station": "COA_N"}, **meta},
+        )
+        self.stream += Trace(
+            data=self._data2int(coord[:-1, 0], 1e6), header={**{"station": "X"}, **meta}
+        )
+        self.stream += Trace(
+            data=self._data2int(coord[:-1, 1], 1e6), header={**{"station": "Y"}, **meta}
+        )
+        self.stream += Trace(
+            data=self._data2int(coord[:-1, 2], 1e3 * ucf),
+            header={**{"station": "Z"}, **meta},
+        )
         self.stream.merge(method=-1)
 
         # Write to file if passed day line
         self.written = False
         stats = self.stream[0].stats
         if stats.starttime.julday != stats.endtime.julday:
             write_start = stats.starttime
@@ -135,53 +140,50 @@
             self.stream.trim(starttime=write_end + stats.delta)
 
         if self.continuous_write and not self.written:
             self.write()
 
     def empty(self, starttime, timestep, i, msg, ucf):
         """
-        Create an empty set of arrays to write to .scanmseed; used where there
-        is no data available to run
-        :func:`~quakemigrate.signal.scan.QuakeScan._compute()`.
+        Create an empty set of arrays to write to .scanmseed; used where there is no
+        data available to run :func:`~quakemigrate.signal.scan.QuakeScan._compute()`.
 
         Parameters
         ----------
         starttime : `obspy.UTCDateTime` object
             Timestamp of first sample in the given timestep.
         timestep : float
             Length (in seconds) of timestep used in detect().
         i : int
             The ith timestep of the continuous compute.
         msg : str
-            Message to output to log giving details as to why this timestep is
-            empty.
+            Message to output to log giving details as to why this timestep is empty.
         ucf : float
-            A conversion factor based on the lookup table grid projection. Used
-            to ensure the same level of precision (millimetre) is retained
-            during compression, irrespective of the units of the grid
-            projection.
+            A conversion factor based on the lookup table grid projection. Used to
+            ensure the same level of precision (millimetre) is retained during
+            compression, irrespective of the units of the grid projection.
 
         """
 
         logging.info(msg)
 
-        starttime = starttime + timestep*i
+        starttime = starttime + timestep * i
         n = util.time2sample(timestep, self.sampling_rate) + 1
         max_coa = max_coa_n = np.full(n, 0)
         coord = np.full((n, 3), 0)
 
         self.append(starttime, max_coa, max_coa_n, coord, ucf)
 
     def write(self, write_start=None, write_end=None):
         """
-        Write a new .scanmseed file from an `obspy.Stream` object containing
-        the data output from detect(). Note: values have been multiplied by a
-        power of ten, rounded and converted to an int32 array so the data can
-        be saved as mSEED with STEIM2 compression. This multiplication factor
-        is removed when the data is read back in with read_scanmseed().
+        Write a new .scanmseed file from an `obspy.Stream` object containing the data
+        output from detect(). Note: values have been multiplied by a power of ten,
+        rounded and converted to an int32 array so the data can be saved as mSEED with
+        STEIM2 compression. This multiplication factor is removed when the data is read
+        back in with read_scanmseed().
 
         Parameters
         ----------
         write_start : `obspy.UTCDateTime` object, optional
             Timestamp from which to write the coalescence stream to file.
         write_end : `obspy.UTCDateTime` object, optional
             Timestamp up to which to write the coalescence stream to file.
@@ -199,17 +201,18 @@
         starttime = st[0].stats.starttime
         fstem = f"{starttime.year}_{starttime.julday:03d}"
         file = (fpath / fstem).with_suffix(".scanmseed")
 
         try:
             st.write(str(file), format="MSEED", encoding="STEIM2")
         except InternalMSEEDError as e:
-            logging.debug(f"Cannot compress data: {e}\n"
-                          "Unable to compress data using STEIM2 - falling back"
-                          " on STEIM1.")
+            logging.debug(
+                f"Cannot compress data: {e}\nUnable to compress data using STEIM2 - "
+                "falling back on STEIM1."
+            )
             st.write(str(file), format="MSEED", encoding="STEIM1")
         self.written = True
 
     def _data2int(self, data, factor):
         """
         Utility function to convert data to ints before writing.
 
@@ -223,45 +226,45 @@
         Returns
         -------
         out : `numpy.Array`, int
             Original data stream multiplied by factor and converted to int.
 
         """
 
-        return np.round(data*factor).astype(np.int32)
+        return np.round(data * factor).astype(np.int32)
 
 
 @util.timeit()
 def read_scanmseed(run, starttime, endtime, pad, ucf):
     """
-    Read .scanmseed files between two time stamps. Files are labelled by year
-    and Julian day.
+    Read .scanmseed files between two time stamps. Files are labelled by year and Julian
+    day.
 
     Parameters
     ----------
     run : :class:`~quakemigrate.io.core.Run` object
         Light class encapsulating i/o path information for a given run.
     starttime : `obspy.UTCDateTime` object
         Timestamp from which to read the coalescence stream.
     endtime : `obspy.UTCDateTime` object
         Timestamp up to which to read the coalescence stream.
     pad : float
         Read in "pad" seconds of additional data on either end.
     ucf : float
-        A conversion factor based on the lookup table grid projection. Used to
-        ensure the same level of precision (millimetre) is retained during
-        compression, irrespective of the units of the grid projection.
+        A conversion factor based on the lookup table grid projection. Used to ensure
+        the same level of precision (millimetre) is retained during compression,
+        irrespective of the units of the grid projection.
 
     Returns
     -------
     data : `pandas.DataFrame` object
         Data output by detect() -- decimated scan.
         Columns: ["DT", "COA", "COA_N", "X", "Y", "Z"] - X/Y/Z as lon/lat/units
-        where units is the user-selected units of the lookup table grid
-        projection (either metres or kilometres).
+        where units is the user-selected units of the lookup table grid projection
+        (either metres or kilometres).
     stats : `obspy.trace.Stats` object
         Container for additional header information for coalescence trace.
         Contains keys: network, station, channel, starttime, endtime,
                        sampling_rate, delta, npts, calib, _format, mseed
 
     """
 
@@ -274,16 +277,17 @@
     scanmseed = Stream()
     # Loop through days trying to read .scanmseed files
     while startday + (dy * 86400) <= readend:
         now = readstart + (dy * 86400)
         fstem = f"{now.year}_{now.julday:03d}"
         file = (fpath / fstem).with_suffix(".scanmseed")
         try:
-            scanmseed += read(str(file), starttime=readstart,
-                              endtime=readend, format="MSEED")
+            scanmseed += read(
+                str(file), starttime=readstart, endtime=readend, format="MSEED"
+            )
         except FileNotFoundError:
             logging.info(f"\n\t    No .scanmseed file found for day {fstem}!")
         dy += 1
 
     if not bool(scanmseed):
         raise util.NoScanMseedDataException
 
@@ -292,23 +296,23 @@
 
     data = pd.DataFrame()
     data["DT"] = scanmseed[0].times(type="utcdatetime")
     data["COA"] = scanmseed.select(station="COA")[0].data / 1e5
     data["COA_N"] = scanmseed.select(station="COA_N")[0].data / 1e5
     data["X"] = scanmseed.select(station="X")[0].data / 1e6
     data["Y"] = scanmseed.select(station="Y")[0].data / 1e6
-    data["Z"] = scanmseed.select(station="Z")[0].data / (1e3*ucf)
+    data["Z"] = scanmseed.select(station="Z")[0].data / (1e3 * ucf)
 
     # Check if the data covers the entirety of the requested period
     if stats.starttime > starttime:
-        logging.info("\n\t    Warning! .scanmseed starttime is later than "
-                     "trigger() starttime!")
+        logging.info(
+            "\n\t    Warning! .scanmseed starttime is later than trigger() starttime!"
+        )
     elif stats.starttime > readstart:
         logging.info("\t    Warning! No .scanmseed data found for pre-pad!")
     if stats.endtime < endtime - stats.delta:
-        logging.info("\n\t    Warning! .scanmseed endtime is before trigger() "
-                     "endtime!")
+        logging.info("\n\t    Warning! .scanmseed endtime is before trigger() endtime!")
     elif stats.endtime < readend:
         logging.info("\t    Warning! No .scanmseed data found for post-pad!")
     logging.info(f"\t    ...from {stats.starttime} - {stats.endtime}.")
 
     return data, stats
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quakemigrate-1.0.1/quakemigrate/io/triggered_events.py` & `quakemigrate-1.0.2/quakemigrate/io/triggered_events.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 Module to handle input/output of TriggeredEvents.csv files.
 
 :copyright:
-    2020 - 2021, QuakeMigrate developers.
+    2020–2023, QuakeMigrate developers.
 :license:
     GNU General Public License, Version 3
     (https://www.gnu.org/licenses/gpl-3.0.html)
 
 """
 
 import logging
@@ -32,16 +32,16 @@
         Timestamp up to which to include events in the locate scan.
     trigger_file : str, optional
         File containing triggered events to be located.
 
     Returns
     -------
     events : `pandas.DataFrame` object
-        Triggered events information. Columns: ["EventID", "CoaTime",
-        "TRIG_COA", "COA_X", "COA_Y", "COA_Z", "COA", "COA_NORM"].
+        Triggered events information. Columns: ["EventID", "CoaTime", "TRIG_COA",
+        "COA_X", "COA_Y", "COA_Z", "COA", "COA_NORM"].
 
     """
 
     starttime = kwargs.get("starttime", None)
     endtime = kwargs.get("endtime", None)
     trigger_file = kwargs.get("trigger_file", None)
 
@@ -58,51 +58,63 @@
             if file.is_file():
                 trigger_files.append(file)
             else:
                 logging.info(f"\n\t    Cannot find file: {fstem}")
             readstart += 86400
         if len(trigger_files) == 0:
             raise util.NoTriggerFilesFound
-        events = pd.concat((pd.read_csv(f) for f in trigger_files),
-                           ignore_index=True)
+        events = pd.concat((pd.read_csv(f) for f in trigger_files), ignore_index=True)
 
     events["CoaTime"] = events["CoaTime"].apply(UTCDateTime)
 
     if starttime is not None and endtime is not None:
-        events = events[(events["CoaTime"] >= starttime) &
-                        (events["CoaTime"] <= endtime)]
+        events = events[
+            (events["CoaTime"] >= starttime) & (events["CoaTime"] <= endtime)
+        ]
 
     if len(events) == 0:
-        logging.info("\n\t    No triggered events found! Check your trigger "
-                     "output files.\n")
+        logging.info(
+            "\n\t    No triggered events found! Check your trigger output files.\n"
+        )
 
     return events.reset_index()
 
 
 @util.timeit("info")
 def write_triggered_events(run, events, starttime):
     """
     Write triggered events to a .csv file.
 
     Parameters
     ----------
     run : :class:`~quakemigrate.io.core.Run` object
         Light class encapsulating i/o path information for a given run.
     events : `pandas.DataFrame` object
-        Triggered events information. Columns: ["EventID", "CoaTime",
-        "TRIG_COA", "COA_X", "COA_Y", "COA_Z", "COA", "COA_NORM"].
+        Triggered events information. Columns: ["EventID", "CoaTime", "TRIG_COA",
+        "COA_X", "COA_Y", "COA_Z", "COA", "COA_NORM"].
     starttime : `obspy.UTCDateTime` object
         Timestamp from which events have been triggered.
 
     """
 
     fpath = run.path / "trigger" / run.subname / "events"
     fpath.mkdir(exist_ok=True, parents=True)
 
     # Work on a copy
     events = events.copy()
-    events = events.loc[:, ["EventID", "CoaTime", "TRIG_COA", "COA_X", "COA_Y",
-                            "COA_Z", "COA", "COA_NORM"]]
+    events = events.loc[
+        :,
+        [
+            "EventID",
+            "CoaTime",
+            "TRIG_COA",
+            "COA_X",
+            "COA_Y",
+            "COA_Z",
+            "COA",
+            "COA_NORM",
+        ],
+    ]
 
     fstem = f"{run.name}_{starttime.year}_{starttime.julday:03d}"
     file = (fpath / f"{fstem}_TriggeredEvents").with_suffix(".csv")
     events.to_csv(file, index=False)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quakemigrate-1.0.1/quakemigrate/lut/__init__.py` & `quakemigrate-1.0.2/quakemigrate/lut/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 The :mod:`quakemigrate.lut` module handles the definition and generation of the
 traveltime lookup tables used in QuakeMigrate.
 
 :copyright:
-    2020 - 2021, QuakeMigrate developers.
+    2020–2023, QuakeMigrate developers.
 :license:
     GNU General Public License, Version 3
     (https://www.gnu.org/licenses/gpl-3.0.html)
 
 """
 
 import pyproj
@@ -16,20 +16,20 @@
 from .create_lut import compute_traveltimes, read_nlloc  # NOQA
 from .lut import LUT  # NOQA
 
 
 # Handle bugged version of PROJ
 proj_major, proj_minor, proj_patch = pyproj.proj_version_str.split(".")
 if proj_major == "6" and proj_minor == "2":
-    raise ImportError(f"PROJ version {proj_major}.{proj_minor}.{proj_patch} is"
-                      " being used as the backend for pyproj. This version "
-                      "has a\nbug with the conversion of Z units when using "
-                      "units that are not metres. Please consult the \n"
-                      "QuakeMigrate installation instructions for how to "
-                      "update the PROJ backend.")
+    raise ImportError(
+        f"PROJ version {proj_major}.{proj_minor}.{proj_patch} is being used as the "
+        "backend for pyproj. This version has a\nbug with the conversion of Z units "
+        "when using units that are not metres. Please consult the \nQuakeMigrate "
+        "installation instructions for how to update the PROJ backend."
+    )
 
 
 def update_lut(old_lut_file, save_file):
     """
     Utility function to convert old-style LUTs to new-style LUTs.
 
     Parameters
@@ -46,16 +46,15 @@
     lut = read_lut(old_lut_file)
 
     try:
         traveltimes = {}
         for station, phases in lut.maps.items():
             for phase, ttimes in phases.items():
                 phase_code = phase.split("_")[1]
-                traveltimes.setdefault(station, {}).update(
-                    {phase_code: ttimes})
+                traveltimes.setdefault(station, {}).update({phase_code: ttimes})
         lut.traveltimes = traveltimes
         del lut.maps
     except AttributeError:
         pass
     lut.phases = ["P", "S"]
     lut.fraction_tt = 0.1
     try:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quakemigrate-1.0.1/quakemigrate/lut/create_lut.py` & `quakemigrate-1.0.2/quakemigrate/lut/create_lut.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 Module to produce traveltime lookup tables defined on a Cartesian grid.
 
 :copyright:
-    2020 - 2021, QuakeMigrate developers.
+    2020–2023, QuakeMigrate developers.
 :license:
     GNU General Public License, Version 3
     (https://www.gnu.org/licenses/gpl-3.0.html)
 
 """
 
 import logging
@@ -47,16 +47,15 @@
     log : bool, optional
         Toggle for logging - default is to only print information to stdout.
         If True, will also create a log file.
 
     Returns
     -------
     lut : :class:`~quakemigrate.lut.lut.LUT` object
-        Lookup table populated with traveltimes from the NonLinLoc lookup table
-        files.
+        Lookup table populated with traveltimes from the NonLinLoc lookup table files.
 
     Raises
     ------
     NotImplementedError
         If the specified projection type is not supported.
 
     """
@@ -76,15 +75,15 @@
                 node_count = np.array(gridspec[0])
                 grid_origin = np.array(gridspec[1])
                 node_spacing = np.array(gridspec[2])
 
                 gproj, cproj, gproj_string = transform
                 if gproj is None:
                     raise NotImplementedError(
-                        f"Projection type {gproj_string}" " not supported."
+                        f"Projection type {gproj_string} not supported."
                     )
 
                 # Transform from grid projection origin to a coord origin
                 ll_corner = Transformer.from_proj(gproj, cproj).transform(*grid_origin)
 
                 # Calculate the ur corner
                 ur_corner = np.array(grid_origin) + (node_count - 1) * node_spacing
@@ -122,39 +121,38 @@
     save_file=None,
     log=False,
     **kwargs,
 ):
     """
     Top-level method for computing traveltime lookup tables.
 
-    This function takes a grid specification and is capable of computing
-    traveltimes for an arbitrary number of phases using a variety of
-    techniques.
+    This function takes a grid specification and is capable of computing traveltimes for
+    an arbitrary number of phases using a variety of techniques.
 
     Parameters
     ----------
     grid_spec : dict
-        Dictionary containing all of the defining parameters for the underlying
-        3-D grid on which the traveltimes are to be calculated. For expected
-        keys, see :class:`~quakemigrate.lut.lut.Grid3D`.
+        Dictionary containing all of the defining parameters for the underlying 3-D grid
+        on which the traveltimes are to be calculated. For expected keys, see
+        :class:`~quakemigrate.lut.lut.Grid3D`.
     stations : `pandas.DataFrame`
         DataFrame containing station information (lat/lon/elev).
     method : str
         Method to be used when computing the traveltime lookup tables.\n
             "homogeneous" - straight line velocities.\n
             "1dfmm" - 1-D fast-marching method using scikit-fmm.\n
             "1dnlloc" - a 2-D traveltime grid is calculated from the 1-D\
                         velocity model using the Grid2Time eikonal solver in\
                         NonLinLoc, then swept over the 3-D grid using a\
                         bilinear interpolation scheme.
     phases : list of str, optional
         List of seismic phases for which to calculate traveltimes.
     fraction_tt : float, optional
-        An estimate of the uncertainty in the velocity model as a function of
-        a fraction of the traveltime. (Default 0.1 == 10%)
+        An estimate of the uncertainty in the velocity model as a function of a fraction
+        of the traveltime. (Default 0.1 == 10%)
     save_file : str, optional
         Path to location to save pickled lookup table.
     log : bool, optional
         Toggle for logging - default is to only print information to stdout.
         If True, will also create a log file.
     kwargs : dict
         Dictionary of all keyword arguments passed to compute when called.
@@ -211,44 +209,42 @@
 
         for phase in phases:
             logging.info(f"\t...phase: {phase}...")
             _compute_1d_fmm(lut, phase, vmodel)
 
     elif method == "3dfmm":
         raise NotImplementedError(
-            "Feature coming soon - please contact the " "QuakeMigrate developers."
+            "Feature coming soon - please contact the QuakeMigrate developers."
         )
 
     elif method == "1dnlloc":
         logging.info("Computing 1-D nlloc traveltimes for...")
         lut.velocity_model = vmodel = kwargs.get("vmod")
         if vmodel is None:
             raise TypeError("Missing argument: 'vmod'")
 
         for phase in phases:
             logging.info(f"\t...phase: {phase}...")
             _compute_1d_nlloc(lut, phase, vmodel, **kwargs)
 
     else:
         raise ValueError(
-            f"'{method} is not a valid method. Please consult the"
-            "documentation. Valid options are 'homogeneous', "
-            "'1dfmm' and '1dnlloc'."
+            f"'{method} is not a valid method. Please consult the documentation. Valid "
+            "options are 'homogeneous', '1dfmm', and '1dnlloc'."
         )
 
     if save_file is not None:
         lut.save(save_file)
 
     return lut
 
 
 def _compute_homogeneous(lut, phase, velocity):
     """
-    Calculate the traveltime lookup table for a station in a homogeneous
-    velocity model.
+    Calculate the traveltime lookup table for a station in a homogeneous velocity model.
 
     Parameters
     ----------
     lut : :class:`~quakemigrate.lut.lut.LUT` object
         Defines the grid on which the traveltimes are to be calculated.
     phase : str
         The seismic phase for which to calculate traveltimes.
@@ -257,28 +253,26 @@
 
     """
 
     grid_xyz = lut.grid_xyz
     stations_xyz = lut.stations_xyz
 
     for i, station in enumerate(lut.station_data["Name"].values):
-        logging.info(
-            f"\t\t...station: {station} - {i+1} of " f"{stations_xyz.shape[0]}"
-        )
+        logging.info(f"\t\t...station: {station} - {i+1} of {stations_xyz.shape[0]}")
 
         dx, dy, dz = [grid_xyz[j] - stations_xyz[i, j] for j in range(3)]
         dist = np.sqrt(dx**2 + dy**2 + dz**2)
 
         lut.traveltimes.setdefault(station, {}).update({phase: dist / velocity})
 
 
 def _compute_1d_fmm(lut, phase, vmodel):
     """
-    Calculate traveltime lookup tables for each station in a 1-D velocity
-    model using the fast-marching method.
+    Calculate traveltime lookup tables for each station in a 1-D velocity model using
+    the fast-marching method.
 
     Parameters
     ----------
     lut : :class:`~quakemigrate.lut.lut.LUT` object
         Defines the grid on which the traveltimes are to be calculated.
     phase : str
         The seismic phase for which to calculate traveltimes.
@@ -287,16 +281,16 @@
         Columns:
             "Depth" of each layer in model (positive down)
             "V<phase>" velocity for each layer in model (e.g. "Vp")
 
     Raises
     ------
     InvalidVelocityModelHeader
-        If the velocity model does not contain the key corresponding to the
-        specified seismic `phase`. (E.g. "Vp" for "P" phase.)
+        If the velocity model does not contain the key corresponding to the specified
+        seismic `phase`. (E.g. "Vp" for "P" phase.)
 
     """
 
     try:
         depths, vmodel = vmodel[["Depth", f"V{phase.lower()}"]].values.T
     except KeyError:
         raise util.InvalidVelocityModelHeader(f"V{phase.lower()}")
@@ -309,85 +303,79 @@
     stations_xyz = lut.stations_xyz
 
     # Check that all stations are contained within grid
     if (lut.stations_xyz < lut.ll_corner).any() or (
         lut.stations_xyz > lut.ur_corner
     ).any():
         raise ValueError(
-            "Cannot calculate traveltimes with method '1dfmm' "
-            "unless all stations are contained within the grid! "
-            "Please either use method '1dnlloc' or increase the "
-            "grid extent to contain all stations"
+            "Cannot calculate traveltimes with method '1dfmm' unless all stations are "
+            "contained within the grid! Please either use method '1dnlloc' or increase "
+            "the grid extent to contain all stations"
         )
 
     # Interpolate the velocity model in the Z-dimension
     f = interp1d(depths, vmodel)
     int_vmodel = f(grid_xyz[2])
 
     for i, station in enumerate(lut.station_data["Name"].values):
-        logging.info(
-            f"\t\t...station: {station} - {i+1} of " f"{stations_xyz.shape[0]}"
-        )
+        logging.info(f"\t\t...station: {station} - {i+1} of {stations_xyz.shape[0]}")
 
         lut.traveltimes.setdefault(station, {}).update(
             {
                 phase: _eikonal_fmm(
                     grid_xyz, lut.node_spacing, int_vmodel, stations_xyz[i]
                 )
             }
         )
 
 
 def _eikonal_fmm(grid_xyz, node_spacing, velocity_grid, station_xyz):
     """
-    Calculates the traveltime lookup tables by solving the eikonal equation
-    using an implementation of the fast-marching algorithm.
+    Calculates the traveltime lookup tables by solving the eikonal equation using an
+    implementation of the fast-marching algorithm.
 
-    Traveltime calculation can only be performed between grid nodes: the
-    station location is therefore taken as the closest grid node. Note that
-    for large node spacings this may cause a modest error in the calculated
-    traveltimes.
+    Traveltime calculation can only be performed between grid nodes: the station
+    location is therefore taken as the closest grid node. Note that for large node
+    spacings this may cause a modest error in the calculated traveltimes.
 
     .. warning:: Requires the scikit-fmm python package.
 
     Parameters
     ----------
     grid_xyz : array-like
         [X, Y, Z] coordinates of each node.
     node_spacing : array-like
         [X, Y, Z] distances between each node.
     velocity_grid : array-like
-        Contains the speed of interface propagation at each point in the
-        domain.
+        Contains the speed of interface propagation at each point in the domain.
     station_xyz : array-like
         Station location (in grid xyz).
 
     Returns
     -------
     traveltimes : array-like, same shape as grid_xyz
-        Contains the traveltime from the zero contour (zero level set) of phi
-        to each point in the array given the scalar velocity field speed. If
-        the input array speed has values less than or equal to zero the return
-        value will be a masked array.
+        Contains the traveltime from the zero contour (zero level set) of phi to each
+        point in the array given the scalar velocity field speed. If the input array
+        speed has values less than or equal to zero the return value will be a masked
+        array.
 
     Raises
     ------
     ImportError
         If scikit-fmm is not installed.
 
     """
 
     try:
         import skfmm
     except ImportError:
         raise ImportError(
-            "Unable to import skfmm - you need to install "
-            "scikit-fmm to use this method.\nSee the "
-            "installation instructions in the documentation"
-            "for more details."
+            "Unable to import skfmm - you need to install scikit-fmm to use this "
+            "method.\nSee the installation instructions in the documentation for more "
+            "details."
         )
 
     phi = -np.ones(grid_xyz[0].shape)
     # Find closest grid node to true station location
     indx = np.argmin(
         abs(grid_xyz[0] - station_xyz[0])
         + abs(grid_xyz[1] - station_xyz[1])
@@ -398,21 +386,21 @@
     return skfmm.travel_time(phi, velocity_grid, dx=node_spacing)
 
 
 def _compute_1d_nlloc(lut, phase, vmodel, **kwargs):
     """
     Calculate 3-D traveltime lookup tables from a 1-D velocity model.
 
-    NonLinLoc Grid2Time is used to generate a 2-D lookup table which is then
-    swept around the full range of azimuths, centred on the station location,
-    to populate the 3-D traveltime grid.
-
-    .. warning:: Requires NonLinLoc to be installed, and `Vel2Grid` and
-    `Grid2Time` to be in the user's path. Alternatively, a custom path to
-    these executables can be specified with the kwarg `nlloc_path`.
+    NonLinLoc Grid2Time is used to generate a 2-D lookup table which is then swept
+    around the full range of azimuths, centred on the station location, to populate the
+    3-D traveltime grid.
+
+    .. warning:: Requires NonLinLoc to be installed, and `Vel2Grid` and `Grid2Time` to
+    be in the user's path. Alternatively, a custom path to these executables can be
+    specified with the kwarg `nlloc_path`.
 
     Parameters
     ----------
     lut : :class:`~quakemigrate.lut.lut.LUT` object
         Defines the grid on which the traveltimes are to be calculated.
     phase : str
         The seismic phase for which to calculate traveltimes.
@@ -424,25 +412,24 @@
     kwargs : dict
         Can contain:
         nlloc_dx : float, optional
             NLLoc 2D grid spacing (default: 0.1 km). Note: units must be km.
         nlloc_path : str, optional
             Path to NonLinLoc executables Vel2Grid and Grid2Time (default: "").
         block_model : bool, optional
-            Toggle to choose whether to interpret velocity model with constant
-            velocity blocks or a linear gradient (default: False).
+            Toggle to choose whether to interpret velocity model with constant velocity
+            blocks or a linear gradient (default: False).
         retain_nll_grids : bool, optional
-            Toggle to choose whether to keep the 2-D traveltime grids created
-            by NonLinLoc Grid2Time (default: False).
+            Toggle to choose whether to keep the 2-D traveltime grids created by
+            NonLinLoc Grid2Time (default: False).
 
     Raises
     ------
     FileNotFoundError
-        If the Vel2Grid and/or Grid2Time executables are not found in the
-        `nlloc_path`.
+        If the Vel2Grid and/or Grid2Time executables are not found in the `nlloc_path`.
     Exception
         If the execution of `Grid2Time` or `Vel2Grid` returns an error.
 
     """
 
     from subprocess import check_output, STDOUT
 
@@ -455,16 +442,16 @@
     # Check nlloc_path is valid and contains Vel2Grid and Grid2Time
     if kwargs.get("nlloc_path", "") != "":
         if (
             not (nlloc_path / "Vel2Grid").exists()
             or not (nlloc_path / "Grid2Time").exists()
         ):
             raise FileNotFoundError(
-                f"Incorrect nlloc_path? - Grid2Time and "
-                f"Vel2Grid not found in {nlloc_path}"
+                "Incorrect nlloc_path? - Grid2Time and Vel2Grid not found in "
+                f"{nlloc_path}"
             )
 
     # For NonLinLoc, distances/velocities must be in km - use conversion factor
     km_cf = 1000 / lut.unit_conversion_factor
     grid_xyz = [g / km_cf for g in lut.grid_xyz]
     stations_xyz = lut.stations_xyz / km_cf
     ll, *_, ur = lut.grid_corners / km_cf
@@ -473,26 +460,26 @@
     # Make folders in which to run NonLinLoc
     cwd = pathlib.Path.cwd()
     (cwd / "time").mkdir(exist_ok=True)
     (cwd / "model").mkdir(exist_ok=True)
 
     for i, station in enumerate(lut.station_data["Name"].values):
         logging.info(
-            f"\t\t...running Grid2Time - station: {station:5s} - "
-            f"{i+1} of {stations_xyz.shape[0]}"
+            f"\t\t...running Grid2Time - station: {station:5s} - {i+1} of "
+            f"{stations_xyz.shape[0]}"
         )
 
         dx, dy = [grid_xyz[j] - stations_xyz[i, j] for j in range(2)]
         distances = np.sqrt(dx**2 + dy**2).flatten()
         depths = grid_xyz[2].flatten()
         max_dist = np.max(distances)
 
-        # NLLoc needs the station to lie within the 2-D section -> we pick the
-        # depth extent of the 2-D grid from the max. possible extent of the
-        # station and the grid - [min_z, max_z]
+        # NLLoc needs the station to lie within the 2-D section -> we pick the depth
+        # extent of the 2-D grid from the max. possible extent of the station and the
+        # grid - [min_z, max_z]
         depth_span = [
             np.min([ll[2], stations_xyz[i, 2]]),
             np.max([ur[2], stations_xyz[i, 2]]),
         ]
 
         # Allow 2 nodes on depth extent as a computational buffer
         _write_control_file(
@@ -531,22 +518,22 @@
             for file in (cwd / "time").glob(f"layer.{phase}.{station}.time*"):
                 file.unlink()
             for file in (cwd / "time").glob(f"layer.{phase}.mod.*"):
                 file.unlink()
 
     if not retain_nll_grids:
         rmtree(cwd / "model")
-        # Check time directory is empty before removing (might have
-        # saved grids from previous runs)
+        # Check time directory is empty before removing (might have saved grids from
+        # previous runs)
         if not os.listdir(cwd / "time"):
             rmtree(cwd / "time")
         else:
             logging.info(
-                "Warning: time directory not empty; does it contain "
-                "traveltime grids from a previous run?\nNot removed."
+                "Warning: time directory not empty; does it contain traveltime grids "
+                "from a previous run?\nNot removed."
             )
 
 
 def _write_control_file(
     station_xyz, station, max_dist, vmodel, depth_span, phase, dx, block_model
 ):
     """
@@ -568,16 +555,16 @@
     depth_span : array-like
         Minimum/maximum extent of the grid in the z-dimension, in km.
     phase : str
         The seismic phase for which to calculate traveltimes.
     dx : float
         NLLoc 2D grid spacing, in km.
     block_model : bool
-        Toggle to choose whether to interpret velocity model with constant
-        velocity blocks or a linear gradient.
+        Toggle to choose whether to interpret velocity model with constant velocity
+        blocks or a linear gradient.
 
     """
 
     control_string = (
         "CONTROL 0 54321\n"
         "TRANS NONE\n\n"
         "VGOUT {model_path:s}\n"
@@ -614,24 +601,24 @@
     Parses in the header of a NonLinLoc file for the grid specification and the
     coordinate transforms. Then unpacks the binary buffer file containing the
     traveltimes.
 
     Parameters
     ----------
     fname : str
-        Path to file containing NonLinLoc traveltime lookup tables, without
-        the extension.
+        Path to file containing NonLinLoc traveltime lookup tables, without the
+        extension.
     ignore_proj : bool, optional
         Flag to suppress the "No projection specified" message.
 
     Returns
     -------
     gridspec : array-like
-        Details on the NonLinLoc grid specification. Contains the number of
-        nodes, the grid origin and the node spacings.
+        Details on the NonLinLoc grid specification. Contains the number of nodes, the
+        grid origin and the node spacings.
     transform : array of `pyproj.Proj` objects
         Array containing the grid and coordinate projections, respectively.
     traveltimes : array-like
         Traveltimes for the station.
 
     """
 
@@ -688,17 +675,16 @@
                 proj_ellipsoid = "bessel"
             elif proj_ellipsoid == "Hayford-1830":
                 proj_ellipsoid = "evrst30"
             elif proj_ellipsoid == "Sphere":
                 proj_ellipsoid = "sphere"
             else:
                 logging.info(
-                    f"Projection Ellipsoid {proj_ellipsoid} not "
-                    "supported!\n\tPlease notify the QuakeMigrate "
-                    "developers.\n\n\tWGS-84 used instead...\n"
+                    f"Projection Ellipsoid {proj_ellipsoid} not supported!\n\tPlease "
+                    "notify the QuakeMigrate developers.\n\n\tWGS-84 used instead...\n"
                 )
                 proj_ellipsoid = "WGS84"
 
             gproj = Proj(
                 proj="lcc",
                 lon_0=orig_lon,
                 lat_0=orig_lat,
@@ -725,26 +711,26 @@
     gridspec = np.array([[nx, ny, nz], [x0, y0, z0], [dx, dy, dz]])
 
     return gridspec, transform, traveltimes
 
 
 def _bilinear_interpolate(xz, xz_origin, xz_dimensions, traveltimes):
     """
-    Perform a bi-linear interpolation between 4 data points on the input
-    2-D lookup table to calculate the traveltime to nodes on the 3-D grid.
+    Perform a bi-linear interpolation between 4 data points on the input 2-D lookup
+    table to calculate the traveltime to nodes on the 3-D grid.
 
-    Note: x is used to denote the horizontal dimension over which the
-    interpolation is performed. Due to the NonLinLoc definition, this
-    corresponds to the y component of the grid.
+    Note: x is used to denote the horizontal dimension over which the interpolation is
+    performed. Due to the NonLinLoc definition, this corresponds to the y component of
+    the grid.
 
     Parameters
     ----------
     xz : array-like
-        Column-stacked array of distances from the station and depths for all
-        points in grid.
+        Column-stacked array of distances from the station and depths for all points in
+        grid.
     xz_origin : array-like
         The x (actually y) and z values of the grid origin.
     xz_dimensions : array-like
         The x (actually y) and z values of the node spacing.
     traveltimes : array-like
         A slice through the traveltime grid at x = 0, on which to perform the
         interpolation.
@@ -784,16 +770,16 @@
     ----------
     vmodel : `pandas.DataFrame` object
         DataFrame containing the velocity model to be used to generate the LUT.
         Columns:
             "Depth" of each layer in model (positive down), in km.
             "V<phase>" velocity for each layer in model (e.g. "Vp"), in km / s.
     block_model : bool
-        Toggle to choose whether to interpret velocity model with constant
-        velocity blocks or a linear gradient.
+        Toggle to choose whether to interpret velocity model with constant velocity
+        blocks or a linear gradient.
     phase : str
         The seismic phase for which to calculate traveltimes.
 
     Returns
     -------
     str_vmodel : str
         NonLinLoc formatted string describing the velocity model.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quakemigrate-1.0.1/quakemigrate/lut/lut.py` & `quakemigrate-1.0.2/quakemigrate/lut/lut.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 Module to produce traveltime lookup tables defined on a Cartesian grid.
 
 :copyright:
-    2020 - 2021, QuakeMigrate developers.
+    2020–2023, QuakeMigrate developers.
 :license:
     GNU General Public License, Version 3
     (https://www.gnu.org/licenses/gpl-3.0.html)
 
 """
 
 import copy
@@ -20,82 +20,75 @@
 from pyproj import Transformer
 from mpl_toolkits.axes_grid1.anchored_artists import AnchoredSizeBar
 from scipy.interpolate import RegularGridInterpolator
 
 
 class Grid3D:
     """
-    A grid object represents a collection of points in a 3-D Cartesian space
-    that can be used to produce regularised traveltime lookup tables that
-    sample the continuous traveltime space for each station in a seismic
-    network.
-
-    This class also provides the series of transformations required to move
-    between the input projection, the grid projection and the grid index
-    coordinate spaces.
-
-    The size and shape specifications of the grid are defined by providing the
-    (input projection) coordinates for the lower-left and upper-right corners,
-    a node spacing and the projections (defined using pyproj) of the input and
-    grid spaces.
+    A grid object represents a collection of points in a 3-D Cartesian space that can be
+    used to produce regularised traveltime lookup tables that sample the continuous
+    traveltime space for each station in a seismic network.
+
+    This class also provides the series of transformations required to move between the
+    input projection, the grid projection and the grid index coordinate spaces.
+
+    The size and shape specifications of the grid are defined by providing the (input
+    projection) coordinates for the lower-left and upper-right corners, a node spacing
+    and the projections (defined using pyproj) of the input and grid spaces.
 
     Attributes
     ----------
     coord_proj : `pyproj.Proj` object
         Input coordinate space projection.
     grid_corners : array-like, shape (8, 3)
         Positions of the corners of the grid in the grid coordinate space.
     grid_proj : `pyproj.Proj` object
         Grid space projection.
     grid_xyz : array-like, shape (3, nx, ny, nz)
-        Positions of the grid nodes in the grid coordinate space. The shape of
-        each element of the list is defined by the number of nodes in each
-        dimension.
+        Positions of the grid nodes in the grid coordinate space. The shape of each
+        element of the list is defined by the number of nodes in each dimension.
     ll_corner : array-like, [float, float, float]
-        Location of the lower-left corner of the grid in the grid
-        projection. Should also contain the minimum depth in the grid.
+        Location of the lower-left corner of the grid in the grid projection. Should
+        also contain the minimum depth in the grid.
     node_count : array-like, [int, int, int]
-        Number of nodes in each dimension of the grid. This is calculated by
-        finding the number of nodes with a given node spacing that fit between
-        the lower-left and upper-right corners. This value is rounded up if the
-        number of nodes returned is non-integer, to ensure the requested area
-        is included in the grid.
+        Number of nodes in each dimension of the grid. This is calculated by finding the
+        number of nodes with a given node spacing that fit between the lower-left and
+        upper-right corners. This value is rounded up if the number of nodes returned is
+        non-integer, to ensure the requested area is included in the grid.
     node_spacing : array-like, [float, float, float]
         Distance between nodes in each dimension of the grid.
     precision : list of float
-        An appropriate number of decimal places for distances as a function of
-        the node spacing and coordinate projection.
+        An appropriate number of decimal places for distances as a function of the node
+        spacing and coordinate projection.
     unit_conversion_factor : float
-        A conversion factor based on the grid projection, used to convert
-        between units of metres and kilometres.
+        A conversion factor based on the grid projection, used to convert between units
+        of metres and kilometres.
     unit_name : str
         Shorthand string for the units of the grid projection.
     ur_corner : array-like, [float, float, float]
-        Location of the upper-right corner of the grid in the grid
-        projection. Should also contain the maximum depth in the grid.
+        Location of the upper-right corner of the grid in the grid projection. Should
+        also contain the maximum depth in the grid.
 
     Methods
     -------
     coord2grid(value, inverse=False, clip=False)
-        Provides a transformation between the input projection and grid
-        coordinate spaces.
+        Provides a transformation between the input projection and grid coordinate
+        spaces.
     decimate(df, inplace=False)
         Downsamples the traveltime lookup tables by some decimation factor.
     index2coord(value, inverse=False, unravel=False, clip=False)
-        Provides a transformation between grid indices (can be a flattened
-        index or an [i, j, k] position) and the input projection coordinate
-        space.
+        Provides a transformation between grid indices (can be a flattened index or an
+        [i, j, k] position) and the input projection coordinate space.
     index2grid(value, inverse=False, unravel=False)
-        Provides a transformation between grid indices (can be a flattened
-        index or an [i, j, k] position) and the grid coordinate space.
+        Provides a transformation between grid indices (can be a flattened index or an
+        [i, j, k] position) and the grid coordinate space.
 
     """
 
-    def __init__(self, ll_corner, ur_corner, node_spacing, grid_proj,
-                 coord_proj):
+    def __init__(self, ll_corner, ur_corner, node_spacing, grid_proj, coord_proj):
         """Instantiate the Grid3D object."""
 
         self.grid_proj = grid_proj
         self.coord_proj = coord_proj
 
         # Transform the geographical grid corners into grid coordinates
         self.ll_corner = self.coord2grid(ll_corner)[0]
@@ -135,36 +128,36 @@
             grid = copy.deepcopy(self)
 
         grid.node_count = new_node_count
         grid.node_spacing = self.node_spacing * df
 
         for station, map_ in grid.traveltimes.items():
             for phase, ttimes in map_.items():
-                grid[station][phase] = ttimes[c1[0]::df[0],
-                                              c1[1]::df[1],
-                                              c1[2]::df[2]]
+                grid[station][phase] = ttimes[
+                    c1[0] :: df[0], c1[1] :: df[1], c1[2] :: df[2]
+                ]
 
         if not inplace:
             return grid
 
     def index2grid(self, value, inverse=False, unravel=False):
         """
         Convert between grid indices and grid coordinate space.
 
         Parameters
         ----------
         value : array-like
-            Array (of arrays) containing the grid indices (grid coordinates)
-            to be transformed. Can be an array of flattened indices.
+            Array (of arrays) containing the grid indices (grid coordinates) to be
+            transformed. Can be an array of flattened indices.
         inverse : bool, optionale
             Reverses the direction of the transform.
             Default indices -> grid coordinates.
         unravel : bool, optional
-            Convert a flat index or array of flat indices into a tuple of
-            coordinate arrays.
+            Convert a flat index or array of flat indices into a tuple of coordinate
+            arrays.
 
         Returns
         -------
         out : array-like
             Returns an array of arrays of the transformed values.
 
         """
@@ -189,17 +182,16 @@
     def coord2grid(self, value, inverse=False):
         """
         Convert between input coordinate space and grid coordinate space.
 
         Parameters
         ----------
         value : array-like
-            Array (of arrays) containing the coordinate locations to be
-            transformed. Each sub-array should describe a single point in the
-            3-D input space.
+            Array (of arrays) containing the coordinate locations to be transformed.
+            Each sub-array should describe a single point in the 3-D input space.
         inverse : bool, optional
             Reverses the direction of the transform.
             Default input coordinates -> grid coordinates
 
         Returns
         -------
         out : array-like
@@ -221,22 +213,22 @@
         Convert between grid indices and input coordinate space.
 
         This is a utility function that wraps the other two defined transforms.
 
         Parameters
         ----------
         value : array-like
-            Array (of arrays) containing the grid indices (grid coordinates)
-            to be transformed. Can be an array of flattened indices.
+            Array (of arrays) containing the grid indices (grid coordinates) to be
+            transformed. Can be an array of flattened indices.
         inverse : bool, optional
             Reverses the direction of the transform.
             Default indices -> input projection coordinates.
         unravel : bool, optional
-            Convert a flat index or array of flat indices into a tuple of
-            coordinate arrays.
+            Convert a flat index or array of flat indices into a tuple of coordinate
+            arrays.
 
         Returns
         -------
         out : array-like
             Returns an array of arrays of the transformed values.
 
         """
@@ -253,47 +245,49 @@
     @property
     def node_count(self):
         """Get and set the number of nodes in each dimension of the grid."""
 
         try:
             return self._node_count
         except AttributeError:
-            print("FutureWarning: The internal data structure of LUT has "
-                  "changed.\nTo remove this warning you will need to convert "
-                  "your lookup table to the new-style\nusing "
-                  "`quakemigrate.lut.update_lut`.")
+            print(
+                "FutureWarning: The internal data structure of LUT has changed.\nTo "
+                "remove this warning you will need to convert your lookup table to the "
+                "new-style\nusing `quakemigrate.lut.update_lut`."
+            )
             return self._cell_count
 
     @node_count.setter
     def node_count(self, value):
         value = np.array(value, dtype="int32")
-        assert (np.all(value > 0)), "Node count must be greater than [0]"
+        assert np.all(value > 0), "Node count must be greater than [0]"
         self._node_count = value
 
     @property
     def node_spacing(self):
         """Get and set the spacing of nodes in each dimension of the grid."""
 
         try:
             return self._node_spacing
         except AttributeError:
-            print("FutureWarning: The internal data structure of LUT has "
-                  "changed.\nTo remove this warning you will need to convert "
-                  "your lookup table to the new-style\nusing "
-                  "`quakemigrate.lut.update_lut`.")
+            print(
+                "FutureWarning: The internal data structure of LUT has changed.\nTo "
+                "remove this warning you will need to convert your lookup table to the "
+                "new-style\nusing `quakemigrate.lut.update_lut`."
+            )
             return self._cell_size
 
     @node_spacing.setter
     def node_spacing(self, value):
         value = np.array(value, dtype="float64")
         if value.size == 1:
             value = np.repeat(value, 3)
         else:
-            assert (value.shape == (3,)), "Node spacing must be an nx3 array."
-        assert (np.all(value > 0)), "Node spacing must be greater than [0]"
+            assert value.shape == (3,), "Node spacing must be an nx3 array."
+        assert np.all(value > 0), "Node spacing must be greater than [0]"
         self._node_spacing = value
 
     @property
     def grid_corners(self):
         """Get the xyz positions of the nodes on the corners of the grid."""
 
         c = self.node_count - 1
@@ -301,24 +295,22 @@
 
         return self.index2grid(np.c_[i.flatten(), j.flatten(), k.flatten()])
 
     def get_grid_extent(self, cells=False):
         """
         Get the minimum/maximum extent of each dimension of the grid.
 
-        The default returns the grid extent as the convex hull of the grid
-        nodes. It is useful, for visualisation purposes, to also be able to
-        determine the grid extent as the convex hull of a grid of cells centred
-        on the grid nodes.
+        The default returns the grid extent as the convex hull of the grid nodes. It is
+        useful, for visualisation purposes, to also be able to determine the grid extent
+        as the convex hull of a grid of cells centred on the grid nodes.
 
         Parameters
         ----------
         cells : bool, optional
-            Specifies the grid mode (nodes / cells) for which to calculate the
-            extent.
+            Specifies the grid mode (nodes / cells) for which to calculate the extent.
 
         Returns
         -------
         extent : array-like
             Pair of arrays representing two corners for the grid.
 
         """
@@ -342,21 +334,23 @@
         xyz = self.index2grid(np.column_stack([dim.flatten() for dim in ijk]))
 
         return [xyz[:, dim].reshape(nc) for dim in range(3)]
 
     @property
     def precision(self):
         """
-        Get appropriate number of decimal places as a function of the
-        node spacing and coordinate projection.
+        Get appropriate number of decimal places as a function of the node spacing and
+        coordinate projection.
 
         """
 
-        return [-int(np.format_float_scientific(axis).split("e")[1]) for axis
-                in np.subtract(*self.index2coord([[0, 0, 0], [1, 1, 1]]))]
+        return [
+            -int(np.format_float_scientific(axis).split("e")[1])
+            for axis in np.subtract(*self.index2coord([[0, 0, 0], [1, 1, 1]]))
+        ]
 
     @property
     def unit_conversion_factor(self):
         """Expose unit_conversion_factor of the grid projection."""
 
         return self.grid_proj.crs.axis_info[0].unit_conversion_factor
 
@@ -374,51 +368,55 @@
         """Handler for deprecated attribute name 'cell_count'"""
         return self.node_count
 
     @cell_count.setter
     def cell_count(self, value):
         if value is None:
             return
-        print("FutureWarning: Parameter name has changed - continuing.")
-        print("To remove this message, change:")
-        print("\t'cell_count' -> 'node_count'")
+        print(
+            "FutureWarning: Parameter name has changed - continuing.\n"
+            "To remove this message, change:\n"
+            "\t'cell_count' -> 'node_count'"
+        )
         self.node_count = value
 
     @property
     def cell_size(self):
         """Handler for deprecated attribute name 'cell_size'"""
         return self.node_spacing
 
     @cell_size.setter
     def cell_size(self, value):
         if value is None:
             return
-        print("FutureWarning: Parameter name has changed - continuing.")
-        print("To remove this message, change:")
-        print("\t'cell_size' -> 'node_spacing'")
+        print(
+            "FutureWarning: Parameter name has changed - continuing.\n"
+            "To remove this message, change:\n"
+            "\t'cell_size' -> 'node_spacing'"
+        )
         self.node_spacing = value
 
 
 class LUT(Grid3D):
     """
-    A lookup table (LUT) object is a simple data structure that is used to
-    store a series of regularised tables that, for each seismic station in a
-    network, store the traveltimes to every point in the 3-D volume. These
-    lookup tables are pre-computed to efficiently carry out the migration.
+    A lookup table (LUT) object is a simple data structure that is used to store a
+    series of regularised tables that, for each seismic station in a network, store the
+    traveltimes to every point in the 3-D volume. These lookup tables are pre-computed
+    to efficiently carry out the migration.
 
-    This class provides utility functions that can be used to serve up or query
-    these pre-computed lookup tables.
+    This class provides utility functions that can be used to serve up or query these
+    pre-computed lookup tables.
 
     This object is-a :class:`~quakemigrate.lut.lut.Grid3D`.
 
     Attributes
     ----------
     fraction_tt : float
-        An estimate of the uncertainty in the velocity model as a function of
-        a fraction of the traveltime. (Default 0.1 == 10%)
+        An estimate of the uncertainty in the velocity model as a function of a fraction
+        of the traveltime. (Default 0.1 == 10%)
     max_traveltime : float
         The maximum traveltime between any station and a point in the grid.
     phases : list of str
         Seismic phases for which there are traveltime lookup tables available.
     stations_xyz : array-like, shape (n, 3)
         Positions of the stations in the grid coordinate space.
     traveltimes : dict
@@ -436,23 +434,23 @@
         Contains the input velocity model specification.
 
     Methods
     -------
     serve_traveltimes(sampling_rate)
         Serve up the traveltime lookup tables.
     traveltime_to(phase, ijk)
-        Query traveltimes to a grid location (in terms of indices) for a
-        particular phase.
+        Query traveltimes to a grid location (in terms of indices) for a particular
+        phase.
     save(filename)
         Dumps the current state of the lookup table object to a pickle file.
     load(filename)
         Restore the state of the saved LUT object from a pickle file.
     plot(fig, gs, slices=None, hypocentre=None, station_clr="k")
-        Plot cross-sections of the LUT with station locations. Optionally plot
-        slices through a coalescence image.
+        Plot cross-sections of the LUT with station locations. Optionally plot slices
+        through a coalescence image.
 
     """
 
     def __init__(self, fraction_tt=0.1, lut_file=None, **grid_spec):
         """Instantiate the LUT object."""
 
         if grid_spec:
@@ -470,52 +468,61 @@
         self.station_data = pd.DataFrame()
 
     def __str__(self):
         """Return short summary string of the lookup table object."""
 
         ll, *_, ur = self.coord2grid(self.grid_corners, inverse=True)
 
-        out = ("QuakeMigrate traveltime lookup table\nGrid parameters"
-               "\n\tLower-left corner  : {lat1:10.5f}\u00b0N "
-               "{lon1:10.5f}\u00b0E {dep1:10.3f} {unit_name:s}"
-               "\n\tUpper-right corner : {lat2:10.5f}\u00b0N "
-               "{lon2:10.5f}\u00b0E {dep2:10.3f} {unit_name:s}"
-               f"\n\tNumber of nodes    : {self.node_count}"
-               f"\n\tNode spacing       : {self.node_spacing} {self.unit_name}"
-               "\n\n")
-
-        out = out.format(lat1=ll[0], lon1=ll[1], dep1=ll[2],
-                         lat2=ur[0], lon2=ur[1], dep2=ur[2],
-                         unit_name=self.unit_name)
-
-        out += ("\tVelocity model:\n"
-                "\t{}".format(str(self.velocity_model).replace("\n", "\n\t")))
+        out = (
+            "QuakeMigrate traveltime lookup table\nGrid parameters"
+            "\n\tLower-left corner  : {lat1:10.5f}\u00b0N "
+            "{lon1:10.5f}\u00b0E {dep1:10.3f} {unit_name:s}"
+            "\n\tUpper-right corner : {lat2:10.5f}\u00b0N "
+            "{lon2:10.5f}\u00b0E {dep2:10.3f} {unit_name:s}"
+            f"\n\tNumber of nodes    : {self.node_count}"
+            f"\n\tNode spacing       : {self.node_spacing} {self.unit_name}"
+            "\n\n"
+        )
+
+        out = out.format(
+            lat1=ll[0],
+            lon1=ll[1],
+            dep1=ll[2],
+            lat2=ur[0],
+            lon2=ur[1],
+            dep2=ur[2],
+            unit_name=self.unit_name,
+        )
+
+        out += "\tVelocity model:\n\t{}".format(
+            str(self.velocity_model).replace("\n", "\n\t")
+        )
 
         return out
 
     def serve_traveltimes(self, sampling_rate, availability=None):
         """
         Serve up the traveltime lookup tables.
 
-        The traveltimes are multiplied by the scan sampling rate and converted
-        to integers.
+        The traveltimes are multiplied by the scan sampling rate and converted to
+        integers.
 
         Parameters
         ----------
         sampling_rate : int
             Samples per second used in the scan run.
         availability : dict, optional
-            Dict of stations and phases for which to serve traveltime lookup
-            tables: keys "station_phase".
+            Dict of stations and phases for which to serve traveltime lookup tables:
+            keys "station_phase".
 
         Returns
         -------
         traveltimes : `numpy.ndarray` of `numpy.int`
-            Stacked traveltime lookup tables for all seismic phases, stacked
-            along the station axis, with shape(nx, ny, nz, nstations)
+            Stacked traveltime lookup tables for all seismic phases, stacked along the
+            station axis, with shape(nx, ny, nz, nstations)
 
         """
 
         if availability is None:
             # Serve all
             traveltimes = self._serve_traveltimes(self.phases)
         else:
@@ -537,17 +544,16 @@
         Parameters
         ----------
         phase : str
             The seismic phase to lookup.
         ijk : array-like
             Grid indices for which to serve traveltime.
         station : str or list-like (of str), optional
-            Station or stations for which to serve traveltimes. Can be str
-            (for a single station) or list / `pandas.Series` object for
-            multiple.
+            Station or stations for which to serve traveltimes. Can be str (for a single
+            station) or list / `pandas.Series` object for multiple.
 
         Returns
         -------
         traveltimes : array-like
             Array of interpolated traveltimes to the requested grid position.
 
         """
@@ -557,17 +563,17 @@
         if station is None:
             traveltimes = self._serve_traveltimes([phase])
         elif isinstance(station, str):
             traveltimes = self._serve_traveltimes([phase], [station])
         else:
             traveltimes = self._serve_traveltimes([phase], station)
 
-        interpolator = RegularGridInterpolator(grid, traveltimes,
-                                               bounds_error=False,
-                                               fill_value=None)
+        interpolator = RegularGridInterpolator(
+            grid, traveltimes, bounds_error=False, fill_value=None
+        )
 
         return interpolator(ijk)[0]
 
     def _serve_traveltimes(self, phases, stations=None):
         """
         Utility function to serve up traveltimes for a list of phases.
 
@@ -577,21 +583,19 @@
             List of phases for which to serve traveltime lookup tables.
         stations : list-like of str, optional
             List of stations for which to serve traveltime lookup tables.
 
         Returns
         -------
         traveltimes : `numpy.ndarray` of float
-            Array of stacked traveltimes, per the requested phases and
-            stations.
+            Array of stacked traveltimes, per the requested phases and stations.
 
         """
 
-        stations = (self.station_data["Name"].values
-                    if stations is None else stations)
+        stations = self.station_data["Name"].values if stations is None else stations
 
         traveltimes = []
         for phase in phases:
             for station in stations:
                 try:
                     traveltimes.append(self[station][phase])
                 except KeyError:
@@ -613,39 +617,42 @@
         pathlib.Path(filename).parent.mkdir(parents=True, exist_ok=True)
 
         with open(filename, "wb") as f:
             pickle.dump(self.__dict__, f, 4)
 
     def load(self, filename):
         """
-        Read the contents of a pickle file and restore state of the lookup
-        table object.
+        Read the contents of a pickle file and restore state of the lookup table object.
 
         Parameters
         ----------
         filename : str
             Path to pickle file to load.
 
         """
 
-        print("FutureWarning: This method of reading lookup tables has been"
-              "deprecated.\nTo remove this warning:\n"
-              "\tUse 'quakemigrate.io.read_lut(lut_file=/path/to/file'")
+        print(
+            "FutureWarning: This method of reading lookup tables has been deprecated.\n"
+            "To remove this warning:\n\tUse "
+            "'quakemigrate.io.read_lut(lut_file=/path/to/file'"
+        )
 
         with open(filename, "rb") as f:
             self.__dict__.update(pickle.load(f))
 
         if hasattr(self, "maps"):
-            print("FutureWarning: The internal data structure of LUT has "
-                  "changed.\nTo remove this warning you will need to convert "
-                  "your lookup table to the new-style\nusing "
-                  "`quakemigrate.lut.update_lut`.")
-
-    def plot(self, fig, gs, slices=None, hypocentre=None, station_clr="k",
-             station_list=None):
+            print(
+                "FutureWarning: The internal data structure of LUT has changed.\nTo "
+                "remove this warning you will need to convert your lookup table to the "
+                "new-style\nusing `quakemigrate.lut.update_lut`."
+            )
+
+    def plot(
+        self, fig, gs, slices=None, hypocentre=None, station_clr="k", station_list=None
+    ):
         """
         Plot the lookup table for a particular station.
 
         Parameters
         ----------
         fig : `matplotlib.Figure` object
             Canvas on which LUT is plotted.
@@ -654,16 +661,16 @@
         slices : array of arrays, optional
             Slices through a coalescence image to plot.
         hypocentre : array of floats
             Event hypocentre - will add cross-hair to plot.
         station_clr : str, optional
             Plot the stations with a particular colour.
         station_list : list-like of str, optional
-            List of stations from the LUT to plot - useful if only a subset
-            have been selected to be used in e.g. locate.
+            List of stations from the LUT to plot - useful if only a subset have been
+            selected to be used in e.g. locate.
 
         """
 
         xy = plt.subplot2grid(gs, (2, 0), colspan=5, rowspan=5, fig=fig)
         xz = plt.subplot2grid(gs, (7, 0), colspan=5, rowspan=2, fig=fig)
         yz = plt.subplot2grid(gs, (2, 5), colspan=2, rowspan=5, fig=fig)
 
@@ -696,90 +703,141 @@
 
             # --- Plot slices through coalescence volume ---
             if slices is None:
                 continue
 
             slice_ = slices[i + j - 1]
             nx, ny = [dim + 1 for dim in slice_.shape]
-            grid1, grid2 = np.mgrid[gminx:gmaxx:nx*1j, gminy:gmaxy:ny*1j]
+            grid1, grid2 = np.mgrid[gminx : gmaxx : nx * 1j, gminy : gmaxy : ny * 1j]
             sc = ax.pcolormesh(grid1, grid2, slice_, edgecolors="face")
 
             if i + j - 1 != 0:
                 continue
 
             # --- Add colourbar ---
             cax = plt.subplot2grid(gs, (7, 5), colspan=2, rowspan=2, fig=fig)
             cax.set_axis_off()
-            cb = fig.colorbar(sc, ax=cax, orientation="horizontal",
-                              fraction=0.8, aspect=8)
-            cb.ax.set_xlabel("Normalised coalescence\nvalue", rotation=0,
-                             fontsize=14)
+            cb = fig.colorbar(
+                sc, ax=cax, orientation="horizontal", fraction=0.8, aspect=8
+            )
+            cb.ax.set_xlabel("Normalised coalescence\nvalue", rotation=0, fontsize=14)
 
         # --- Plot stations ---
         if station_list is not None:
-            station_data = \
-                self.station_data[self.station_data["Name"].isin(station_list)]
+            station_data = self.station_data[
+                self.station_data["Name"].isin(station_list)
+            ]
         else:
             station_data = self.station_data
-        xy.scatter(station_data.Longitude.values,
-                   station_data.Latitude.values,
-                   s=15, marker="^", zorder=20, c=station_clr)
-        xz.scatter(station_data.Longitude.values,
-                   station_data.Elevation.values,
-                   s=15, marker="^", zorder=20, c=station_clr)
-        yz.scatter(station_data.Elevation.values,
-                   station_data.Latitude.values,
-                   s=15, marker="<", zorder=20, c=station_clr)
+        xy.scatter(
+            station_data.Longitude.values,
+            station_data.Latitude.values,
+            s=15,
+            marker="^",
+            zorder=20,
+            c=station_clr,
+        )
+        xz.scatter(
+            station_data.Longitude.values,
+            station_data.Elevation.values,
+            s=15,
+            marker="^",
+            zorder=20,
+            c=station_clr,
+        )
+        yz.scatter(
+            station_data.Elevation.values,
+            station_data.Latitude.values,
+            s=15,
+            marker="<",
+            zorder=20,
+            c=station_clr,
+        )
         for i, row in station_data.iterrows():
-            xy.annotate(row["Name"], [row.Longitude, row.Latitude], zorder=20,
-                        c=station_clr, clip_on=True)
+            xy.annotate(
+                row["Name"],
+                [row.Longitude, row.Latitude],
+                zorder=20,
+                c=station_clr,
+                clip_on=True,
+            )
 
         # --- Add scalebar ---
         num_cells = np.ceil(self.node_count[0] / 10)
         length = num_cells * self.node_spacing[0]
         size = extent[0] * length / grid_size[0]
-        scalebar = AnchoredSizeBar(xy.transData, size=size,
-                                   label=f"{length} {self.unit_name}",
-                                   loc="lower right", pad=0.5, sep=5,
-                                   frameon=False, color=station_clr)
+        scalebar = AnchoredSizeBar(
+            xy.transData,
+            size=size,
+            label=f"{length} {self.unit_name}",
+            loc="lower right",
+            pad=0.5,
+            sep=5,
+            frameon=False,
+            color=station_clr,
+        )
         xy.add_artist(scalebar)
 
         # --- Axes labelling ---
-        xy.tick_params(which="both", left=True, right=True, top=True,
-                       bottom=True, labelleft=True, labeltop=True,
-                       labelright=False, labelbottom=False)
+        xy.tick_params(
+            which="both",
+            left=True,
+            right=True,
+            top=True,
+            bottom=True,
+            labelleft=True,
+            labeltop=True,
+            labelright=False,
+            labelbottom=False,
+        )
         xy.set_ylabel("Latitude (deg)", fontsize=14)
         xy.yaxis.set_label_position("left")
 
         xz.invert_yaxis()
-        xz.tick_params(which="both", left=True, right=True, top=True,
-                       bottom=True, labelleft=True, labeltop=False,
-                       labelright=False, labelbottom=True)
+        xz.tick_params(
+            which="both",
+            left=True,
+            right=True,
+            top=True,
+            bottom=True,
+            labelleft=True,
+            labeltop=False,
+            labelright=False,
+            labelbottom=True,
+        )
         xz.set_xlabel("Longitude (deg)", fontsize=14)
         xz.set_ylabel(f"Depth ({self.unit_name})", fontsize=14)
         xz.yaxis.set_label_position("left")
 
-        yz.tick_params(which="both", left=True, right=True, top=True,
-                       bottom=True, labelleft=False, labeltop=True,
-                       labelright=True, labelbottom=True)
+        yz.tick_params(
+            which="both",
+            left=True,
+            right=True,
+            top=True,
+            bottom=True,
+            labelleft=False,
+            labeltop=True,
+            labelright=True,
+            labelbottom=True,
+        )
         yz.set_xlabel(f"Depth ({self.unit_name})", fontsize=14)
         yz.xaxis.set_label_position("bottom")
 
     @property
     def max_extent(self):
         """Get the minimum/maximum geographical extent of the stations/grid."""
 
         stat_min, stat_max = self.station_extent
         grid_min, grid_max = self.get_grid_extent(cells=True)
 
         min_extent = [min(a, b) for a, b in zip(stat_min, grid_min)]
         max_extent = [max(a, b) for a, b in zip(stat_max, grid_max)]
         diff = abs(np.subtract(max_extent, min_extent))
 
-        min_extent = np.subtract(min_extent, 0.05*diff)
+        min_extent = np.subtract(min_extent, 0.05 * diff)
         max_extent = np.add(max_extent, 0.05 * diff)
 
         return np.array([min_extent, max_extent])
 
     @property
     def max_traveltime(self):
         """Get the maximum traveltime from any station across the grid."""
@@ -802,18 +860,17 @@
 
         return self.coord2grid(coordinates.values)
 
     def __add__(self, other):
         """
         Define behaviour for the rich addition operator, "+".
 
-        Two lookup tables which have identical grid definitions (as per "==")
-        can be combined by adding the traveltime lookup tables from
-        other.traveltimes for which the station key is not already in
-        self.traveltimes.
+        Two lookup tables which have identical grid definitions (as per "==") can be
+        combined by adding the traveltime lookup tables from other.traveltimes for which
+        the station key is not already in self.traveltimes.
 
         Parameters
         ----------
         other : :class:`~quakemigrate.lut.lut.LUT` object
             LUT with traveltime lookup tables to add to self.
 
         """
@@ -850,23 +907,25 @@
             # Test equality of grid corners
             eq_corners = (self.grid_corners == other.grid_corners).all()
 
             # Test equality of node spacings
             eq_sizes = (self.node_spacing == other.node_spacing).all()
 
             # Test equality of projections
-            eq_projections = (self.grid_proj == other.grid_proj
-                              and self.coord_proj == other.coord_proj)
+            eq_projections = (
+                self.grid_proj == other.grid_proj
+                and self.coord_proj == other.coord_proj
+            )
 
             return eq_corners and eq_sizes and eq_projections
 
     def __getitem__(self, key):
         """
-        Provide a method to directly access traveltime tables by station key
-        without having to go through the traveltimes dictionary.
+        Provide a method to directly access traveltime tables by station key without
+        having to go through the traveltimes dictionary.
 
         Parameters
         ----------
         key : str
             Station ID for which to search.
 
         Returns
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quakemigrate-1.0.1/quakemigrate/plot/__init__.py` & `quakemigrate-1.0.2/quakemigrate/plot/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 figures in QuakeMigrate, including:
     * Event summaries
     * Phase pick summaries
     * Triggered event summaries
     * Amplitude / local magnitude summaries
 
 :copyright:
-    2020 - 2021, QuakeMigrate developers.
+    2020–2023, QuakeMigrate developers.
 :license:
     GNU General Public License, Version 3
     (https://www.gnu.org/licenses/gpl-3.0.html)
 
 """
 
 import matplotlib as mpl
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quakemigrate-1.0.1/quakemigrate/plot/amplitudes.py` & `quakemigrate-1.0.2/quakemigrate/plot/amplitudes.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,64 +1,62 @@
 # -*- coding: utf-8 -*-
 """
-Module to produce a summary plot for local magnitude calculation from
-Wood-Anderson corrected displacement amplitude measurements.
+Module to produce a summary plot for local magnitude calculation from Wood-Anderson
+corrected displacement amplitude measurements.
 
 :copyright:
-    2020 - 2021, QuakeMigrate developers.
+    2020–2023, QuakeMigrate developers.
 :license:
     GNU General Public License, Version 3
     (https://www.gnu.org/licenses/gpl-3.0.html)
 
 """
 
 import matplotlib.pyplot as plt
 import numpy as np
 
 
-def amplitudes_summary(magnitudes, amp_feature, amp_multiplier, dist_err,
-                       r_squared, noise_measure="RMS"):
+def amplitudes_summary(
+    magnitudes, amp_feature, amp_multiplier, dist_err, r_squared, noise_measure="RMS"
+):
     """
-    Plot figure showing the measured signal amplitudes against distance from
-    the event.
+    Plot figure showing the measured signal amplitudes against distance from the event.
 
     Parameters
     ----------
     magnitudes : `pandas.DataFrame` object
-        Contains P- and S-wave amplitude measurements for each component of
-        each station in the station file, and local magnitude estimates
-        calculated from them (output by calculate_magnitudes()). Note that
-        the amplitude observations are raw, but the ML estimates derived
-        from them include station corrections, if provided.
+        Contains P- and S-wave amplitude measurements for each component of each station
+        in the station file, and local magnitude estimates calculated from them (output
+        by calculate_magnitudes()). Note that the amplitude observations are raw, but
+        the ML estimates derived from them include station corrections, if provided.
         Columns = ["epi_dist", "z_dist", "P_amp", "P_freq", "P_time",
                    "P_avg_amp", "P_filter_gain", "S_amp", "S_freq",
                    "S_time", "S_avg_amp", "S_filter_gain", "Noise_amp",
                    "is_picked", "ML", "ML_Err"], "Noise_Filter",
                    "Trace_Filter", "Station_Filter", "Dist_Filter", "Dist",
                    "Used"]
     amp_feature : {"S_amp", "P_amp"}
-        Which phase amplitude measurement to use to calculate local
-        magnitude. (Default "S_amp")
+        Which phase amplitude measurement to use to calculate local magnitude.
+        (Default "S_amp")
     amp_multiplier : float
         Factor by which to multiply all measured amplitudes.
     dist_err : float
         (Epicentral or hypocentral) distance uncertainty - calculated from the
         LocalGaussian location uncertainties.
     r_squared : float
-        r-squared statistic describing the fit of the amplitude vs.
-        distance curve predicted by the calculated mean_mag and chosen
-        attenuation model to the measured amplitude observations. This is
-        intended to be used to help discriminate between 'real' events, for
-        which the predicted amplitude vs. distance curve should provide a
-        good fit to the observations, from artefacts, which in general will
-        not.
+        r-squared statistic describing the fit of the amplitude vs. distance curve
+        predicted by the calculated mean_mag and chosen attenuation model to the
+        measured amplitude observations. This is intended to be used to help
+        discriminate between 'real' events, for which the predicted amplitude vs.
+        distance curve should provide a good fit to the observations, from artefacts,
+        which in general will not.
     noise_measure : {"RMS", "STD", "ENV"}, optional
-        The method by which to measure the amplitude of the signal in the
-        noise window: root-mean-square, standard deviation or average
-        amplitude of the envelope of the signal. (Default "RMS")
+        The method by which to measure the amplitude of the signal in the noise window:
+        root-mean-square, standard deviation or average amplitude of the envelope of the
+        signal. (Default "RMS")
 
     Returns
     -------
     fig : `matplotlib.pyplot.Figure` object
         Figure showing the measured amplitudes against distance from the event.
     ax : `matplotlib.axes.Axes` object
         Figure axes.
@@ -66,99 +64,124 @@
     """
 
     # Initiate figure
     fig = plt.figure(figsize=(25, 15))
     ax = fig.add_subplot(111)
 
     # Correct noise amplitudes according to station corrections
-    noise_amps = magnitudes["Noise_amp"].values * amp_multiplier \
-                    * np.power(10, magnitudes["Station_Correction"])
+    noise_amps = (
+        magnitudes["Noise_amp"].values
+        * amp_multiplier
+        * np.power(10, magnitudes["Station_Correction"])
+    )
     filter_gains = magnitudes[f"{amp_feature[0]}_filter_gain"]
     if not filter_gains.isnull().values.any():
         noise_amps /= filter_gains
 
     # Set to loglog scale
-    ax.set_xscale('log')
-    ax.set_yscale('log')
+    ax.set_xscale("log")
+    ax.set_yscale("log")
 
     # Set axis tick label font size
-    ax.tick_params(axis='both', which='major', labelsize=14)
+    ax.tick_params(axis="both", which="major", labelsize=14)
 
     # Plot noise amps
-    noise_label = (f"Noise amplitude ({noise_measure} amplitude in noise "
-                   "window)")
-    ax.scatter(magnitudes["Dist"], noise_amps, marker="v", c="k",
-               label=noise_label)
+    noise_label = f"Noise amplitude ({noise_measure} amplitude in noise window)"
+    ax.scatter(magnitudes["Dist"], noise_amps, marker="v", c="k", label=noise_label)
 
     # Plot median noise amplitude
-    ax.axhline(np.median(noise_amps), linestyle=':', color='k',
-               label='Median noise amplitude')
+    ax.axhline(
+        np.median(noise_amps), linestyle=":", color="k", label="Median noise amplitude"
+    )
 
     # Plot amplitude obs for used observations
     used_mags = magnitudes[magnitudes["Used"]]
-    signal_label = (f"Signal amplitude (max amplitude in {amp_feature[0]}-wave"
-                    f" signal window)")
+    signal_label = (
+        f"Signal amplitude (max amplitude in {amp_feature[0]}-wave signal window)"
+    )
     # Plot amplitudes with station corrections applied
-    _, _, bars = ax.errorbar(used_mags["Dist"], used_mags[amp_feature] \
-                             * amp_multiplier * \
-                             np.power(10, used_mags["Station_Correction"]),
-                             xerr=dist_err,
-                             yerr=noise_amps[magnitudes["Used"]],
-                             marker="x", label=signal_label)
+    _, _, bars = ax.errorbar(
+        used_mags["Dist"],
+        used_mags[amp_feature]
+        * amp_multiplier
+        * np.power(10, used_mags["Station_Correction"]),
+        xerr=dist_err,
+        yerr=noise_amps[magnitudes["Used"]],
+        marker="x",
+        label=signal_label,
+    )
     _ = [errorbar.set_alpha(0.3) for errorbar in bars]
 
     # One label for each station, above highest observed amplitude; faff.
-    ax, stns = label_stations(ax, used_mags.index,
-                              used_mags[amp_feature] * amp_multiplier \
-                              * np.power(10, used_mags["Station_Correction"]),
-                              used_mags["Dist"])
+    ax, stns = label_stations(
+        ax,
+        used_mags.index,
+        used_mags[amp_feature]
+        * amp_multiplier
+        * np.power(10, used_mags["Station_Correction"]),
+        used_mags["Dist"],
+    )
 
     # Plot amplitude obs for rejected observations (if there are any)
     rejected_mags = magnitudes[~magnitudes["Used"]]
     if len(rejected_mags) > 0:
         unused_label = f"Unused {amp_feature[0]}-wave amplitude observations"
-        _, _, bars = ax.errorbar(rejected_mags["Dist"],
-                                 rejected_mags[amp_feature] * amp_multiplier \
-                                 * np.power(10,
-                                 rejected_mags["Station_Correction"]),
-                                 xerr=dist_err,
-                                 yerr=noise_amps[~magnitudes["Used"]], fmt="o",
-                                 marker="x", c="gray", label=unused_label)
+        _, _, bars = ax.errorbar(
+            rejected_mags["Dist"],
+            rejected_mags[amp_feature]
+            * amp_multiplier
+            * np.power(10, rejected_mags["Station_Correction"]),
+            xerr=dist_err,
+            yerr=noise_amps[~magnitudes["Used"]],
+            fmt="o",
+            marker="x",
+            c="gray",
+            label=unused_label,
+        )
         _ = [errorbar.set_alpha(0.3) for errorbar in bars]
 
         # Only label stations which were not already labelled
         rej_trids = []
         rej_amps = []
         rej_dists = []
         for i, tr_id in enumerate(rejected_mags.index):
             stn = tr_id[:-1]
             if stn in stns:
                 continue
             else:
                 rej_trids.append(tr_id)
-                rej_amps.append(rejected_mags[amp_feature].iloc[i] \
-                    * amp_multiplier * np.power(10,
-                    rejected_mags["Station_Correction"].iloc[i]))
+                rej_amps.append(
+                    rejected_mags[amp_feature].iloc[i]
+                    * amp_multiplier
+                    * np.power(10, rejected_mags["Station_Correction"].iloc[i])
+                )
                 rej_dists.append(rejected_mags["Dist"].iloc[i])
 
         # Only one label per new station; faff once again.
-        ax, _ = label_stations(ax, rej_trids, rej_amps, rej_dists,
-                               rejected=True)
+        ax, _ = label_stations(ax, rej_trids, rej_amps, rej_dists, rejected=True)
 
     # Label r-squared value
-    ax.text(0.98, 0.02, f'r-squared: {r_squared:.2f}', transform=ax.transAxes,
-            bbox=dict(boxstyle='round', fc='w', alpha=0.8), va='bottom',
-            ha='right', fontsize=16)
+    ax.text(
+        0.98,
+        0.02,
+        f"r-squared: {r_squared:.2f}",
+        transform=ax.transAxes,
+        bbox=dict(boxstyle="round", fc="w", alpha=0.8),
+        va="bottom",
+        ha="right",
+        fontsize=16,
+    )
 
     return fig, ax
 
+
 def label_stations(ax, tr_ids, amps, dists, rejected=False):
     """
-    Add station labels to the amplitudes vs. distance plot: only one label for
-    each station, above the highest observed amplitude. Much faff.
+    Add station labels to the amplitudes vs. distance plot: only one label for each
+    station, above the highest observed amplitude. Much faff.
 
     Parameters
     ----------
     ax : `matplotlib.axes.Axes` object
         Axes on which to add the station labels.
     tr_ids : list of str
         List of trace ID's for which there are amplitude observations to label.
@@ -185,56 +208,77 @@
         if not stn:
             stn = tr_id[:-1]
             stn_start = 0
             comps.append(tr_id[-1])
             continue
         elif tr_id[:-1] != stn:
             stn_end = i
-            distance = dists[i-1]
+            distance = dists[i - 1]
             amp = max(amps[stn_start:stn_end])
             compstring = ""
             for comp in comps:
                 compstring += f"{comp},"
             label = f"{stn}[{compstring[:-1]}]"
             if not rejected:
-                ax.annotate(label, (distance, amp), ha="center", va="bottom",
-                            fontsize=8)
+                ax.annotate(
+                    label, (distance, amp), ha="center", va="bottom", fontsize=8
+                )
             else:
-                ax.annotate(label, (distance, amp), color="gray", ha="center",
-                            va="bottom", fontsize=8)
+                ax.annotate(
+                    label,
+                    (distance, amp),
+                    color="gray",
+                    ha="center",
+                    va="bottom",
+                    fontsize=8,
+                )
             stns.append(stn)
             stn = tr_id[:-1]
             stn_start = i
             comps = [tr_id[-1]]
             if i == len(tr_ids) - 1:
                 distance = dists[i]
                 amp = max(amps[stn_start:])
                 compstring = ""
                 for comp in comps:
                     compstring += f"{comp},"
                 label = f"{stn}[{compstring[:-1]}]"
                 if not rejected:
-                    ax.annotate(label, (distance, amp), ha="center",
-                                va="bottom", fontsize=8)
+                    ax.annotate(
+                        label, (distance, amp), ha="center", va="bottom", fontsize=8
+                    )
                 else:
-                    ax.annotate(label, (distance, amp), color="gray",
-                                ha="center", va="bottom", fontsize=8)
+                    ax.annotate(
+                        label,
+                        (distance, amp),
+                        color="gray",
+                        ha="center",
+                        va="bottom",
+                        fontsize=8,
+                    )
         elif i == len(tr_ids) - 1:
             stn = tr_id[:-1]
             comps.append(tr_id[-1])
             distance = dists[i]
             amp = max(amps[stn_start:])
             compstring = ""
             for comp in comps:
                 compstring += f"{comp},"
             label = f"{stn}[{compstring[:-1]}]"
             if not rejected:
-                ax.annotate(label, (distance, amp), ha="center", va="bottom",
-                            fontsize=8)
+                ax.annotate(
+                    label, (distance, amp), ha="center", va="bottom", fontsize=8
+                )
             else:
-                ax.annotate(label, (distance, amp), color="gray", ha="center",
-                            va="bottom", fontsize=8)
+                ax.annotate(
+                    label,
+                    (distance, amp),
+                    color="gray",
+                    ha="center",
+                    va="bottom",
+                    fontsize=8,
+                )
             stns.append(stn)
         else:
             comps.append(tr_id[-1])
 
     return ax, stns
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quakemigrate-1.0.1/quakemigrate/plot/event.py` & `quakemigrate-1.0.2/quakemigrate/plot/event.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 Module containing methods to generate event summaries and videos.
 
 :copyright:
-    2020 - 2021, QuakeMigrate developers.
+    2020–2023, QuakeMigrate developers.
 :license:
     GNU General Public License, Version 3
     (https://www.gnu.org/licenses/gpl-3.0.html)
 
 """
 
 import logging
@@ -21,79 +21,78 @@
 import quakemigrate.util as util
 
 
 @util.timeit("info")
 def event_summary(run, event, marginalised_coa_map, lut, xy_files=None):
     """
     Plots an event summary illustrating the locate results: slices through the
-    marginalised coalescence map with the best location estimate (peak of
-    interpolated spline fitted to 3-D coalescence map) and uncertainty ellipse
-    from gaussian fit to gaussian-smoothed 3-D coalescence map. Plus a waveform
-    gather of the pre-processed waveform data used to calculate the onset
-    functions (sorted by distance from the event), and a plot of the maximum
-    value of the 4-D coalescence function through time.
+    marginalised coalescence map with the best location estimate (peak of interpolated
+    spline fitted to 3-D coalescence map) and uncertainty ellipse from gaussian fit to
+    gaussian-smoothed 3-D coalescence map. Plus a waveform gather of the pre-processed
+    waveform data used to calculate the onset functions (sorted by distance from the
+    event), and a plot of the maximum value of the 4-D coalescence function through
+    time.
 
     Parameters
     ----------
     run : :class:`~quakemigrate.io.core.Run` object
         Light class encapsulating i/o path information for a given run.
     event : :class:`~quakemigrate.io.event.Event` object
-        Light class encapsulating waveforms, coalescence information, picks and
-        location information for a given event.
+        Light class encapsulating waveforms, coalescence information, picks and location
+        information for a given event.
     marginalised_coa_map : `numpy.ndarray` of `numpy.double`
         Marginalised 3-D coalescence map, shape(nx, ny, nz).
     lut : :class:`~quakemigrate.lut.lut.LUT` object
-        Contains the traveltime lookup tables for seismic phases, computed for
-        some pre-defined velocity model.
+        Contains the traveltime lookup tables for seismic phases, computed for some
+        pre-defined velocity model.
     xy_files : str, optional
-        Path to comma-separated value file (.csv) containing a series of
-        coordinate files to plot. Columns: ["File", "Color", "Linewidth",
-        "Linestyle"], where "File" is the absolute path to the file containing
-        the coordinates to be plotted. E.g:
-        "/home/user/volcano_outlines.csv,black,0.5,-". Each .csv coordinate
-        file should contain coordinates only, with columns: ["Longitude",
-        "Latitude"]. E.g.: "-17.5,64.8". Lines pre-pended with ``#`` will be
-        treated as a comment - this can be used to include references. See the
+        Path to comma-separated value file (.csv) containing a series of coordinate
+        files to plot. Columns: ["File", "Color", "Linewidth", "Linestyle"], where
+        "File" is the absolute path to the file containing the coordinates to be
+        plotted. E.g: "/home/user/volcano_outlines.csv,black,0.5,-". Each .csv
+        coordinate file should contain coordinates only, with columns: ["Longitude",
+        "Latitude"]. E.g.: "-17.5,64.8". Lines pre-pended with ``#`` will be treated as
+        a comment - this can be used to include references. See the
         Volcanotectonic_Iceland example XY_files for a template.\n
         .. note:: Do not include a header line in either file.
 
     """
 
     logging.info("\tPlotting event summary figure...")
 
     # Extract indices and grid coordinates of maximum coalescence
     coa_map = np.ma.masked_invalid(marginalised_coa_map)
     idx_max = np.column_stack(np.where(coa_map == np.nanmax(coa_map)))[0]
-    slices = [coa_map[:, :, idx_max[2]],
-              coa_map[:, idx_max[1], :],
-              coa_map[idx_max[0], :, :].T]
+    slices = [
+        coa_map[:, :, idx_max[2]],
+        coa_map[:, idx_max[1], :],
+        coa_map[idx_max[0], :, :].T,
+    ]
     otime = event.otime
 
     fig = plt.figure(figsize=(25, 15))
 
     # Create plot axes, ordering: [WAVEFORMS, COA, XY, XZ, YZ]
     sig_spec = GridSpec(9, 15).new_subplotspec((0, 8), colspan=7, rowspan=7)
     fig.add_subplot(sig_spec)
     fig.canvas.draw()
     coa_spec = GridSpec(9, 15).new_subplotspec((7, 8), colspan=7, rowspan=2)
     fig.add_subplot(coa_spec)
 
     # --- Plot LUT, waveform gather, and max coalescence trace ---
-    lut.plot(fig, (9, 15), slices, event.hypocentre, "white",
-             event.data.stations)
+    lut.plot(fig, (9, 15), slices, event.hypocentre, "white", event.data.stations)
     _plot_waveform_gather(fig.axes[0], lut, event, idx_max)
     _plot_coalescence_trace(fig.axes[1], event)
 
     # --- Plot xy files on map ---
     _plot_xy_files(xy_files, fig.axes[2])
 
     # --- Add event origin time to waveform gather and coalescence plots ---
     for ax in fig.axes[:2]:
-        ax.axvline(otime.datetime, label="Origin time", ls="--", lw=2,
-                   c="#F03B20")
+        ax.axvline(otime.datetime, label="Origin time", ls="--", lw=2, c="#F03B20")
 
     # --- Create and plot covariance and Gaussian uncertainty ellipses ---
     gues = _make_ellipses(lut, event, "gaussian", "k")
     for ax, gue in zip(fig.axes[2:], gues):
         ax.add_patch(gue)
 
     # --- Write summary information ---
@@ -101,20 +100,30 @@
     _plot_text_summary(text, lut, event)
 
     # Deal with repeating labels in waveform gather legend; combine labels for
     # ["N", "1"], ["E", "2"]
     handles, labels = fig.axes[0].get_legend_handles_labels()
     for cp1, cp2 in [("N", "1"), ("E", "2")]:
         if all(x in labels for x in [f"{cp1} component", f"{cp2} component"]):
-            labels = [f"{cp2}, {cp1} component" if x == f"{cp1} component"
-                      or x == f"{cp2} component" else x for x in labels]
+            labels = [
+                f"{cp2}, {cp1} component"
+                if x == f"{cp1} component" or x == f"{cp2} component"
+                else x
+                for x in labels
+            ]
     by_label = dict(zip(labels, handles))
 
-    fig.axes[0].legend(by_label.values(), by_label.keys(), fontsize=14, loc=1,
-                       framealpha=1, markerscale=0.5)
+    fig.axes[0].legend(
+        by_label.values(),
+        by_label.keys(),
+        fontsize=14,
+        loc=1,
+        framealpha=1,
+        markerscale=0.5,
+    )
     fig.axes[1].legend(fontsize=14, loc=1, framealpha=1)
     fig.axes[2].legend(fontsize=14)
     fig.tight_layout(pad=1, h_pad=0)
     plt.subplots_adjust(wspace=0.3, hspace=0.3)
 
     # --- Adjust cross sections to match map aspect ratio ---
     # Get left, bottom, width, height of each subplot bounding box
@@ -127,16 +136,15 @@
     # Adjust bottom of xz cross section (if bottom of map has moved up)
     new_xz_bottom = xy_bottom - hdiff - xz_h
     fig.axes[3].set_position([xy_left, new_xz_bottom, xy_width, xz_h])
     # Adjust left of yz cross section (if right side of map has moved left)
     new_yz_left = xy_left + xy_width + wdiff
     # Take this opportunity to ensure the height of both cross sections is
     # equal by adjusting yz width (almost there from gridspec maths already)
-    new_yz_width = xz_h * (fig.get_size_inches()[1]
-                           / fig.get_size_inches()[0])
+    new_yz_width = xz_h * (fig.get_size_inches()[1] / fig.get_size_inches()[0])
     fig.axes[4].set_position([new_yz_left, xy_bottom, new_yz_width, xy_height])
 
     fpath = run.path / "locate" / run.subname / "summaries"
     fpath.mkdir(exist_ok=True, parents=True)
     fstem = f"{run.name}_{event.uid}_EventSummary"
     file = (fpath / fstem).with_suffix(".pdf")
     plt.savefig(file, dpi=400)
@@ -146,110 +154,122 @@
 WAVEFORM_COLOURS1 = ["#FB9A99", "#7570b3", "#1b9e77"]
 WAVEFORM_COLOURS2 = ["#33a02c", "#b2df8a", "#1f78b4"]
 PICK_COLOURS = ["#F03B20", "#3182BD"]
 
 
 def _plot_waveform_gather(ax, lut, event, idx):
     """
-    Utility function to bring all aspects of plotting the waveform gather into
-    one place.
+    Utility function to bring all aspects of plotting the waveform gather into one
+    place.
 
     Parameters
     ----------
     ax : `matplotlib.Axes` object
         Axes on which to plot the waveform gather.
     lut : :class:`~quakemigrate.lut.lut.LUT` object
-        Contains the traveltime lookup tables for seismic phases, computed for
-        some pre-defined velocity model.
+        Contains the traveltime lookup tables for seismic phases, computed for some
+        pre-defined velocity model.
     event : :class:`~quakemigrate.io.event.Event` object
-        Light class encapsulating waveforms, coalescence information, picks and
-        location information for a given event.
+        Light class encapsulating waveforms, coalescence information, picks and location
+        information for a given event.
     idx : `numpy.ndarray` of `numpy.double`
         Marginalised 3-D coalescence map, shape(nx, ny, nz).
 
     """
 
     phases = event.onset_data.phases
     stations = event.data.stations
 
     # --- Predicted traveltimes ---
-    traveltimes = np.array([lut.traveltime_to(phase, idx, stations)
-                            for phase in phases])
-    arrivals = [[(event.otime + tt).datetime for tt in tt_f]
-                for tt_f in traveltimes]
-
-    range_order = abs(np.argsort(np.argsort(arrivals[0]))
-                      - len(arrivals[0])) * 2
-    s = (ax.get_window_extent().height / (max(range_order)+1) * 1.2) ** 2
+    traveltimes = np.array(
+        [lut.traveltime_to(phase, idx, stations) for phase in phases]
+    )
+    arrivals = [[(event.otime + tt).datetime for tt in tt_f] for tt_f in traveltimes]
+
+    range_order = abs(np.argsort(np.argsort(arrivals[0])) - len(arrivals[0])) * 2
+    s = (ax.get_window_extent().height / (max(range_order) + 1) * 1.2) ** 2
 
     # Handle single-phase plotting
     pick_colours = PICK_COLOURS
     if len(phases) == 1:
         if phases[0] == "P":
             pick_colours = [PICK_COLOURS[0]]
     for arrival, c, phase in zip(arrivals, pick_colours, phases):
-        ax.scatter(arrival, range_order, s=s, c=c, marker="|", zorder=5,
-                   lw=1.5, label=f"Modelled {phase}")
+        ax.scatter(
+            arrival,
+            range_order,
+            s=s,
+            c=c,
+            marker="|",
+            zorder=5,
+            lw=1.5,
+            label=f"Modelled {phase}",
+        )
 
     # --- Waveforms ---
     waveforms = event.onset_data.filtered_waveforms
     # Min and max times to plot
     mint = event.otime - 0.1
-    maxt = min(event.otime + np.max(traveltimes)*1.5, event.data.endtime)
+    maxt = min(event.otime + np.max(traveltimes) * 1.5, event.data.endtime)
     # Convert to indices -- will still be the same for sub-sample shifts
     times_utc = waveforms[0].times("UTCDateTime")
     mint_i, maxt_i = [np.argmin(abs(times_utc - t)) for t in (mint, maxt)]
     for i, station in enumerate(stations):
         stn_waveforms = waveforms.select(station=station)
         for c, comp in zip(WAVEFORM_COLOURS1, ["Z", "[N,1]", "[E,2]"]):
             st = stn_waveforms.select(component=comp)
             if not bool(st):
                 continue
             tr = st[0]
             comp = tr.stats.component
             data = tr.data
 
             # Get station specific range for norm factor
-            stat_maxt = event.otime + max(traveltimes[:, i])*1.5
-            norm = max(abs(data[mint_i:np.argmin(abs(times_utc - stat_maxt))]))
+            stat_maxt = event.otime + max(traveltimes[:, i]) * 1.5
+            norm = max(abs(data[mint_i : np.argmin(abs(times_utc - stat_maxt))]))
 
             # Generate times for plotting
             times = tr.times("matplotlib")[mint_i:maxt_i]
 
             # Trim to plot limits, normalise, shift by range, then plot
             y = data[mint_i:maxt_i] / norm + range_order[i]
             label = f"{comp} component"
             ax.plot(times, y, c=c, lw=0.3, label=label, alpha=0.85)
 
     # --- Limits, annotations, and axis formatting ---
     ax.set_xlim([mint.datetime, maxt.datetime])
-    ax.set_ylim([0, max(range_order)+2])
+    ax.set_ylim([0, max(range_order) + 2])
     ax.xaxis.set_major_formatter(util.DateFormatter("%H:%M:%S.{ms}", 2))
     ax.yaxis.set_ticks(range_order)
     ax.yaxis.set_ticklabels(stations, fontsize=14)
 
 
 def _plot_coalescence_trace(ax, event):
     """
-    Utility function to plot the maximum coalescence trace around the event
-    origin time.
+    Utility function to plot the maximum coalescence trace around the event origin time.
 
     Parameters
     ----------
     ax : `matplotlib.Axes` object
         Axes on which to plot the coalescence trace.
     event : :class:`~quakemigrate.io.event.Event` object
-        Light class encapsulating waveforms, coalescence information, picks and
-        location information for a given event.
+        Light class encapsulating waveforms, coalescence information, picks and location
+        information for a given event.
 
     """
 
     times = [x.datetime for x in event.coa_data["DT"]]
-    ax.plot(times, event.coa_data["COA"], c="k", lw=0.5, zorder=10,
-            label="Maximum coalescence")
+    ax.plot(
+        times,
+        event.coa_data["COA"],
+        c="k",
+        lw=0.5,
+        zorder=10,
+        label="Maximum coalescence",
+    )
     ax.set_ylabel("Maximum coalescence", fontsize=14)
     ax.set_xlabel("DateTime", fontsize=14)
     ax.set_xlim([times[0], times[-1]])
     ax.xaxis.set_major_formatter(util.DateFormatter("%H:%M:%S.{ms}", 2))
 
 
 def _plot_text_summary(ax, lut, event):
@@ -257,36 +277,37 @@
     Utility function to plot the event summary information.
 
     Parameters
     ----------
     ax : `matplotlib.Axes` object
         Axes on which to plot the text summary.
     lut : :class:`~quakemigrate.lut.lut.LUT` object
-        Contains the traveltime lookup tables for seismic phases, computed for
-        some pre-defined velocity model.
+        Contains the traveltime lookup tables for seismic phases, computed for some
+        pre-defined velocity model.
     event : :class:`~quakemigrate.io.event.Event` object
-        Light class encapsulating waveforms, coalescence information, picks and
-        location information for a given event.
+        Light class encapsulating waveforms, coalescence information, picks and location
+        information for a given event.
 
     """
 
     # Grab a conversion factor based on the grid projection to convert the
     # hypocentre depth + uncertainties to the correct units and evaluate the
     # suitable precision to which to report results from the LUT.
     km_cf = 1000 / lut.unit_conversion_factor
     precision = [max((prec + 2), 6) for prec in lut.precision[:2]]
     unit_correction = 3 if lut.unit_name == "km" else 0
     precision.append(max((lut.precision[2] + 2), 0 + unit_correction))
 
-    hypocentre = [round(dimh, dimp) for dimh, dimp
-                  in zip(event.hypocentre, precision)]
-    gau_unc = [round(dim, precision[2]) for dim in event.loc_uncertainty/km_cf]
-    hypo = (f"{hypocentre[1]}\u00b0N \u00B1 {gau_unc[1]} km\n"
-            f"{hypocentre[0]}\u00b0E \u00B1 {gau_unc[0]} km\n"
-            f"{hypocentre[2]/km_cf} \u00B1 {gau_unc[2]} km")
+    hypocentre = [round(dimh, dimp) for dimh, dimp in zip(event.hypocentre, precision)]
+    gau_unc = [round(dim, precision[2]) for dim in event.loc_uncertainty / km_cf]
+    hypo = (
+        f"{hypocentre[1]}\u00b0N \u00B1 {gau_unc[1]} km\n"
+        f"{hypocentre[0]}\u00b0E \u00B1 {gau_unc[0]} km\n"
+        f"{hypocentre[2]/km_cf} \u00B1 {gau_unc[2]} km"
+    )
 
     # Grab the magnitude information
     mag_info = event.local_magnitude
 
     ax.text(0.25, 0.8, f"Event: {event.uid}", fontsize=20, fontweight="bold")
     ot_text = event.otime.strftime("%Y-%m-%d %H:%M:%S.")
     ot_text += event.otime.strftime("%f")[:3]
@@ -307,79 +328,93 @@
 def _make_ellipses(lut, event, uncertainty, clr):
     """
     Utility function to create uncertainty ellipses for plotting.
 
     Parameters
     ----------
     lut : :class:`~quakemigrate.lut.lut.LUT` object
-        Contains the traveltime lookup tables for seismic phases, computed for
-        some pre-defined velocity model.
+        Contains the traveltime lookup tables for seismic phases, computed for some
+        pre-defined velocity model.
     event : :class:`~quakemigrate.io.event.Event` object
-        Light class encapsulating waveforms, coalescence information, picks and
-        location information for a given event.
+        Light class encapsulating waveforms, coalescence information, picks and location
+        information for a given event.
     uncertainty : {"covariance", "gaussian"}
         Choice of uncertainty for which to generate ellipses.
     clr : str
-        Colour for the ellipses - see matplotlib documentation for more
-        details.
+        Colour for the ellipses - see matplotlib documentation for more details.
 
     Returns
     -------
     xy, yz, xz : `matplotlib.Ellipse` (Patch) objects
         Ellipses for the requested uncertainty measure.
 
     """
 
     coord = event.get_hypocentre(method=uncertainty)
     error = event.get_loc_uncertainty(method=uncertainty)
     xyz = lut.coord2grid(coord)[0]
     d = abs(coord - lut.coord2grid(xyz + error, inverse=True))[0]
 
-    xy = Ellipse((coord[0], coord[1]), 2*d[0], 2*d[1], lw=2, edgecolor=clr,
-                 fill=False, label=f"{uncertainty.capitalize()} uncertainty")
-    yz = Ellipse((coord[2], coord[1]), 2*d[2], 2*d[1], lw=2, edgecolor=clr,
-                 fill=False)
-    xz = Ellipse((coord[0], coord[2]), 2*d[0], 2*d[2], lw=2, edgecolor=clr,
-                 fill=False)
+    xy = Ellipse(
+        (coord[0], coord[1]),
+        2 * d[0],
+        2 * d[1],
+        lw=2,
+        edgecolor=clr,
+        fill=False,
+        label=f"{uncertainty.capitalize()} uncertainty",
+    )
+    yz = Ellipse(
+        (coord[2], coord[1]), 2 * d[2], 2 * d[1], lw=2, edgecolor=clr, fill=False
+    )
+    xz = Ellipse(
+        (coord[0], coord[2]), 2 * d[0], 2 * d[2], lw=2, edgecolor=clr, fill=False
+    )
 
     return xy, xz, yz
 
 
 def _plot_xy_files(xy_files, ax):
     """
     Plot xy files supplied by user.
 
-    The user can specify a list of xy files to plot by supplying a csv file
-    with columns: ["File", "Color", "Linewidth", "Linestyle"], where "File" is
-    the absolute path to the file containing the coordinates to be plotted.
+    The user can specify a list of xy files to plot by supplying a csv file with
+    columns: ["File", "Color", "Linewidth", "Linestyle"], where "File" is the absolute
+    path to the file containing the coordinates to be plotted.
     E.g: "/home/user/volcano_outlines.csv,black,0.5,-"
 
     Each specified xy file should contain coordinates only, with columns:
     ["Longitude", "Latitude"]. E.g.: "-17.5,64.8".
 
-    Lines pre-pended with `#` will be treated as a comment - this can be used
-    to include references. See the Volcanotectonic_Iceland example XY_files for
-    a template.\n
+    Lines pre-pended with `#` will be treated as a comment - this can be used to include
+    references. See the Volcanotectonic_Iceland example XY_files for a template.\n
 
     .. note:: Do not include a header line in either file.
 
     Parameters
     ----------
     xy_files : str
-        Path to .csv file containing a list of coordinates files to plot, and
-        the linecolor and style to plot them with.
+        Path to .csv file containing a list of coordinates files to plot, and the
+        linecolor and style to plot them with.
     ax : `matplotlib.Axes` object
         Axes on which to plot the xy files.
 
     """
 
     if xy_files is not None:
-        xy_files = pd.read_csv(xy_files,
-                               names=["File", "Color",
-                                      "Linewidth", "Linestyle"],
-                               header=None, comment="#")
+        xy_files = pd.read_csv(
+            xy_files,
+            names=["File", "Color", "Linewidth", "Linestyle"],
+            header=None,
+            comment="#",
+        )
         for _, f in xy_files.iterrows():
-            xy_file = pd.read_csv(f["File"], names=["Longitude", "Latitude"],
-                                  header=None, comment="#")
-            ax.plot(xy_file["Longitude"].values, xy_file["Latitude"].values,
-                    ls=f["Linestyle"], lw=f["Linewidth"],
-                    c=f["Color"])
+            xy_file = pd.read_csv(
+                f["File"], names=["Longitude", "Latitude"], header=None, comment="#"
+            )
+            ax.plot(
+                xy_file["Longitude"].values,
+                xy_file["Latitude"].values,
+                ls=f["Linestyle"],
+                lw=f["Linewidth"],
+                c=f["Color"],
+            )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quakemigrate-1.0.1/quakemigrate/plot/phase_picks.py` & `quakemigrate-1.0.2/quakemigrate/plot/phase_picks.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 Module to produce a summary plot for the phase picking.
 
 :copyright:
-    2020 - 2021, QuakeMigrate developers.
+    2020–2023, QuakeMigrate developers.
 :license:
     GNU General Public License, Version 3
     (https://www.gnu.org/licenses/gpl-3.0.html)
 
 """
 
 import logging
@@ -16,77 +16,83 @@
 import numpy as np
 
 import quakemigrate.util as util
 
 
 def pick_summary(event, station, waveforms, picks, onsets, ttimes, windows):
     """
-    Plot a figure showing the pre-processed traces for each data component and
-    the onset functions calculated from them for each phase. The search window
-    to make a phase pick is displayed, along with the dynamic pick threshold,
-    the phase pick time and its uncertainty (if made) and the Gaussian fit to
-    the onset function.
+    Plot a figure showing the pre-processed traces for each data component and the onset
+    functions calculated from them for each phase. The search window to make a phase
+    pick is displayed, along with the dynamic pick threshold, the phase pick time and
+    its uncertainty (if made) and the Gaussian fit to the onset function.
 
     Parameters
     ----------
     event : :class:`~quakemigrate.io.event.Event` object
-        Light class encapsulating waveforms, coalescence information, picks and
-        location information for a given event.
+        Light class encapsulating waveforms, coalescence information, picks and location
+        information for a given event.
     station : str
         Station code.
     waveforms : `obspy.Stream` object
         Filtered seismic data used to calculate the onset functions.
     picks : `pandas.DataFrame` object
         Phase pick times with columns ["Name", "Phase", "ModelledTime",
         "PickTime", "PickError", "SNR"]
         Each row contains the phase pick from one station/phase.
     onsets : dict of {str: `numpy.ndarray`}
         Keys are phases. Onset functions for each seismic phase.
     ttimes : list of float
-        Modelled traveltimes from the event hypocentre to the station
-        for each phase to be plotted.
+        Modelled traveltimes from the event hypocentre to the station for each phase to
+        be plotted.
     windows : dict of list, [int, int, int]
-        Keys are phase. Indices specifying the window within which the pick was
-        made [start, modelled_arrival, end].
+        Keys are phase. Indices specifying the window within which the pick was made
+        [start, modelled_arrival, end].
 
     Returns
     -------
     fig : `matplotlib.Figure` object
         Figure showing phase picking information.
 
     """
 
     fig = plt.figure(figsize=(30, 15))
 
     # Create plot axes, ordering: [Z data, N data, E data, P onset, S onset]
     for i in [2, 1, 3, 4, 5]:
-        ax = fig.add_subplot(3, 2, i+1)
+        ax = fig.add_subplot(3, 2, i + 1)
     axes = fig.axes
 
     # Share P-pick x-axes and set title
     axes[0].get_shared_x_axes().join(axes[0], axes[3])
     axes[0].set_xticklabels([])
     axes[0].set_yticklabels([])
-    axes[0].yaxis.set_ticks_position('none')
+    axes[0].yaxis.set_ticks_position("none")
     axes[0].set_title("P phase", fontsize=22, fontweight="bold")
     axes[3].set_xlabel("DateTime", fontsize=14)
 
     # Share S-pick x-axes and set title
     for ax in axes[1:3]:
         ax.get_shared_x_axes().join(ax, axes[4])
         ax.set_xticklabels([])
         ax.set_yticklabels([])
-        ax.yaxis.set_ticks_position('none')
+        ax.yaxis.set_ticks_position("none")
     axes[1].set_title("S phase", fontsize=22, fontweight="bold")
     axes[4].set_xlabel("DateTime", fontsize=14)
 
     # Add axis for text info
     text = fig.add_subplot(3, 2, 1)
-    text.text(0.5, 0.8, f"Event: {event.uid}\nStation: {station}", ha="center",
-              va="center", fontsize=22, fontweight="bold")
+    text.text(
+        0.5,
+        0.8,
+        f"Event: {event.uid}\nStation: {station}",
+        ha="center",
+        va="center",
+        fontsize=22,
+        fontweight="bold",
+    )
 
     # --- Grab event information once ---
     otime = event.otime
     times = waveforms[0].times(type="utcdatetime")
     dtimes = [x.datetime for x in times]
 
     phases = [phase for phase, _ in onsets.items()]
@@ -103,75 +109,111 @@
     min_win_idx = np.min([v[0] for v in windows.values()]) - 10
     max_win_idx = np.max([v[-1] for v in windows.values()]) + 10
     # Take min and max
     min_idx = min(min_t_idx, min_win_idx)
     max_idx = max(max_t_idx, max_win_idx)
     # Ensure min and max are within length of trace
     if min_idx < 0:
-        logging.debug(f"Min index is before start of trace for station "
-                      f"{station}! {min_idx}")
+        logging.debug(
+            f"Min index is before start of trace for station {station}! {min_idx}"
+        )
         min_idx = 0
     if max_idx >= len(times):
-        logging.debug(f"Max index is after end of trace for station "
-                      f"{station}! {max_idx} / {len(times)}")
+        logging.debug(
+            f"Max index is after end of trace for station "
+            f"{station}! {max_idx} / {len(times)}"
+        )
         max_idx = len(times) - 1
 
     # --- Plot waveforms ---
     for i, (ax, comp) in enumerate(zip(axes[:3], ["Z", "[N,1]", "[E,2]"])):
         tr = waveforms.select(component=comp)
         if not bool(tr):
             continue
         y = tr[0].data
-        ax.plot(dtimes[min_idx:max_idx+1], y[min_idx:max_idx+1], c="k", lw=0.5,
-                zorder=1)
+        ax.plot(
+            dtimes[min_idx : max_idx + 1],
+            y[min_idx : max_idx + 1],
+            c="k",
+            lw=0.5,
+            zorder=1,
+        )
         # Add label (SEED id)
-        ax.text(0.015, 0.95, f"{tr[0].id}", transform=ax.transAxes,
-                bbox=dict(boxstyle="round", fc="w", alpha=0.8), va="top",
-                ha="left", fontsize=18, zorder=2)
+        ax.text(
+            0.015,
+            0.95,
+            f"{tr[0].id}",
+            transform=ax.transAxes,
+            bbox=dict(boxstyle="round", fc="w", alpha=0.8),
+            va="top",
+            ha="left",
+            fontsize=18,
+            zorder=2,
+        )
         # Set ylim
-        y_max = max(abs(y[min_win_idx:max_win_idx+1]))
-        ax.set_ylim(ymin=-1.1*y_max, ymax=1.1*y_max)
+        y_max = max(abs(y[min_win_idx : max_win_idx + 1]))
+        ax.set_ylim(ymin=-1.1 * y_max, ymax=1.1 * y_max)
 
     # --- Plot onset functions ---
     # Handle case where only S phase is used
     n = 3
     if len(phases) == 1 and phases[0] == "S":
         n += 1
 
     # Loop through all relevant onset function axes
     for i, (ax, ph) in enumerate(zip(axes[n:5], phases)):
         # Plot onset functions
         y = onsets[i]
-        ax.plot(dtimes[min_idx:max_idx+1], y[min_idx:max_idx+1], c="k", lw=0.5,
-                zorder=1)
+        ax.plot(
+            dtimes[min_idx : max_idx + 1],
+            y[min_idx : max_idx + 1],
+            c="k",
+            lw=0.5,
+            zorder=1,
+        )
 
         # Plot labels
-        ax.text(0.015, 0.95, f"{ph} onset", transform=ax.transAxes,
-                bbox=dict(boxstyle="round", fc="w", alpha=0.8), va="top",
-                ha="left", fontsize=18, zorder=2)
+        ax.text(
+            0.015,
+            0.95,
+            f"{ph} onset",
+            transform=ax.transAxes,
+            bbox=dict(boxstyle="round", fc="w", alpha=0.8),
+            va="top",
+            ha="left",
+            fontsize=18,
+            zorder=2,
+        )
 
         # Plot pick threshold
         gau = event.picks["gaussfits"][station][ph]
         thresh = gau["PickThreshold"]
         ax.axhline(thresh, label="Pick threshold")
-        text.text(0.05+i*0.5, 0.2, f"Pick threshold: {thresh:5.3f}", ha="left",
-                  va="center", fontsize=18)
+        text.text(
+            0.05 + i * 0.5,
+            0.2,
+            f"Pick threshold: {thresh:5.3f}",
+            ha="left",
+            va="center",
+            fontsize=18,
+        )
 
         # Plot gaussian fit to onset function
         if not gau["PickValue"] == -1:
-            yy = util.gaussian_1d(gau["xdata"], gau["popt"][0],
-                                  gau["popt"][1], gau["popt"][2])
+            yy = util.gaussian_1d(
+                gau["xdata"], gau["popt"][0], gau["popt"][1], gau["popt"][2]
+            )
             dt = [x.datetime for x in gau["xdata_dt"]]
             ax.plot(dt, yy)
 
         # Set ylim
         win = windows[ph]
-        onset_max = max(onsets[i][win[0]:win[2]+1])
+        onset_max = max(onsets[i][win[0] : win[2] + 1])
         y_max = max(onset_max, thresh)
-        ax.set_ylim(0, y_max*1.1)
+        ax.set_ylim(0, y_max * 1.1)
 
     # --- Plot predicted arrival times ---
     # Handle case where only a single phase is used
     ax_ind = range(5)
     colors = ["#F03B20", "#3182BD"]
     if len(phases) == 1:
         if phases[0] == "P":
@@ -183,24 +225,26 @@
 
     # Loop through all relevant axes
     for ind in ax_ind:
         ax = axes[ind]
         # Plot model picks
         model_pick = otime + ttimes[0] if ind % 3 == 0 else otime + ttimes[-1]
         ph = phases[0] if ind % 3 == 0 else phases[-1]
-        ax.axvline(model_pick.datetime, alpha=0.9, c="k",
-                   label=f"Modelled {ph} arrival")
+        ax.axvline(
+            model_pick.datetime, alpha=0.9, c="k", label=f"Modelled {ph} arrival"
+        )
         # Plot event origin time if it is on plot:
         if times[min_idx] < otime:
             ax.axvline(otime.datetime, c="green", label="Event origin time")
         # Plot pick windows
         win = windows[phases[0]] if ind % 3 == 0 else windows[phases[-1]]
         clr = colors[0] if ind % 3 == 0 else colors[-1]
-        ax.axvspan(dtimes[win[0]], dtimes[win[2]], alpha=0.2, color=clr,
-                   label="Picking window")
+        ax.axvspan(
+            dtimes[win[0]], dtimes[win[2]], alpha=0.2, color=clr, label="Picking window"
+        )
         # Set xlim
         ax.set_xlim(dtimes[min_idx], dtimes[max_idx])
 
     # --- Plot picks and summary information ---
     for i, pick in picks.iterrows():
         # Pick lines
         if pick["Phase"] == "P":
@@ -214,22 +258,30 @@
                 _plot_phase_pick(ax, pick, clr)
         # Calculate residual:
         if pick.PickTime == -1:
             resid = -1
         else:
             resid = pick.PickTime - pick.ModelledTime
         # Summary text
-        text.text(0.1+i*0.5, 0.6, f"{pick.Phase} phase", ha="center",
-                  va="center", fontsize=20, fontweight="bold")
-        pick_info = (f"Pick time: {pick.PickTime}\n"
-                     f"Pick error: {pick.PickError:5.3f} s\n"
-                     f"Pick SNR: {pick.SNR:5.3f}\n"
-                     f"Pick residual: {resid:5.3f} s")
-        text.text(0.05+i*0.5, 0.4, pick_info, ha="left", va="center",
-                  fontsize=18)
+        text.text(
+            0.1 + i * 0.5,
+            0.6,
+            f"{pick.Phase} phase",
+            ha="center",
+            va="center",
+            fontsize=20,
+            fontweight="bold",
+        )
+        pick_info = (
+            f"Pick time: {pick.PickTime}\n"
+            f"Pick error: {pick.PickError:5.3f} s\n"
+            f"Pick SNR: {pick.SNR:5.3f}\n"
+            f"Pick residual: {resid:5.3f} s"
+        )
+        text.text(0.05 + i * 0.5, 0.4, pick_info, ha="left", va="center", fontsize=18)
     text.set_axis_off()
 
     # Add legend
     for ind in ax_ind:
         if ind > 2:
             axes[ind].legend(fontsize=16, loc="upper right")
 
@@ -252,10 +304,10 @@
     clr : str
         Colour to use when plotting the phase pick.
 
     """
 
     pick_time, pick_err = pick["PickTime"], pick["PickError"]
 
-    ax.axvline((pick_time - pick_err/2).datetime, ls="--", c=clr)
-    ax.axvline((pick_time + pick_err/2).datetime, ls="--", c=clr)
+    ax.axvline((pick_time - pick_err / 2).datetime, ls="--", c=clr)
+    ax.axvline((pick_time + pick_err / 2).datetime, ls="--", c=clr)
     ax.axvline((pick_time).datetime, c=clr, label=f"{pick.Phase} pick time")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quakemigrate-1.0.1/quakemigrate/plot/trigger.py` & `quakemigrate-1.0.2/quakemigrate/plot/trigger.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 Module to plot the triggered events on a decimated grid.
 
 :copyright:
-    2020 - 2021, QuakeMigrate developers.
+    2020–2023, QuakeMigrate developers.
 :license:
     GNU General Public License, Version 3
     (https://www.gnu.org/licenses/gpl-3.0.html)
 
 """
 
 import logging
@@ -18,76 +18,85 @@
 
 
 from quakemigrate.io import read_availability
 import quakemigrate.util as util
 
 
 @util.timeit("info")
-def trigger_summary(events, starttime, endtime, run, marginal_window,
-                    min_event_interval, detection_threshold,
-                    normalise_coalescence, lut, data, region, discarded_events,
-                    interactive, xy_files=None, plot_all_stns=True):
-    """
-    Plots the data from a .scanmseed file with annotations illustrating the
-    trigger results: event triggers and marginal windows on the coalescence
-    traces, and map and cross section view of the gridded triggered earthquake
-    locations.
+def trigger_summary(
+    events,
+    starttime,
+    endtime,
+    run,
+    marginal_window,
+    min_event_interval,
+    detection_threshold,
+    normalise_coalescence,
+    lut,
+    data,
+    region,
+    discarded_events,
+    interactive,
+    xy_files=None,
+    plot_all_stns=True,
+):
+    """
+    Plots the data from a .scanmseed file with annotations illustrating the trigger
+    results: event triggers and marginal windows on the coalescence traces, and map and
+    cross section view of the gridded triggered earthquake locations.
 
     Parameters
     ----------
     events : `pandas.DataFrame`
-        Triggered events information, columns: ["EventID", "CoaTime",
-        "TRIG_COA", "COA_X", "COA_Y", "COA_Z", "MinTime", "MaxTime", "COA",
-        "COA_NORM"].
+        Triggered events information, columns: ["EventID", "CoaTime", "TRIG_COA",
+        "COA_X", "COA_Y", "COA_Z", "MinTime", "MaxTime", "COA", "COA_NORM"].
     starttime : `obspy.UTCDateTime`
         Start time of trigger run.
     endtime : `obspy.UTCDateTime`
         End time of trigger run.
     run : :class:`~quakemigrate.io.core.Run` object
         Light class encapsulating i/o path information for a given run.
     marginal_window : float
         Time window over which to marginalise the 4D coalescence function.
     min_event_interval : float
         Minimum time interval between triggered events.
     detection_threshold : array-like
         Coalescence value above which to trigger events.
     normalise_coalescence : bool
-        If True, use coalescence normalised by the average coalescence value in
-        the 3-D grid at each timestep.
+        If True, use coalescence normalised by the average coalescence value in the 3-D
+        grid at each timestep.
     lut : :class:`~quakemigrate.lut.lut.LUT` object
-        Contains the traveltime lookup tables for the selected seismic phases,
-        computed for some pre-defined velocity model.
+        Contains the traveltime lookup tables for the selected seismic phases, computed
+        for some pre-defined velocity model.
     data : `pandas.DataFrame`
         Data output by :func:`~quakemigrate.signal.scan.QuakeScan.detect()` --
         continuous scan, columns: ["COA", "COA_N", "X", "Y", "Z"]
     region : list
-        Geographical region within which to trigger earthquakes; events located
-        outside this region will be discarded.
+        Geographical region within which to trigger earthquakes; events located outside
+        this region will be discarded.
     discarded_events : `pandas.DataFrame`
         Discarded triggered events information, columns: ["EventID", "CoaTime",
-        "TRIG_COA", "COA_X", "COA_Y", "COA_Z", "MinTime", "MaxTime", "COA",
-        "COA_NORM"].
+        "TRIG_COA", "COA_X", "COA_Y", "COA_Z", "MinTime", "MaxTime", "COA", "COA_NORM"].
     interactive : bool
         Toggles whether to produce an interactive plot.
     xy_files : str, optional
-        Path to comma-separated value file (.csv) containing a series of
-        coordinate files to plot. Columns: ["File", "Color", "Linewidth",
-        "Linestyle"], where "File" is the absolute path to the file containing
-        the coordinates to be plotted. E.g:
-        "/home/user/volcano_outlines.csv,black,0.5,-". Each .csv coordinate
-        file should contain coordinates only, with columns: ["Longitude",
-        "Latitude"]. E.g.: "-17.5,64.8". Lines pre-pended with ``#`` will be
-        treated as a comment - this can be used to include references. See the
+        Path to comma-separated value file (.csv) containing a series of coordinate
+        files to plot. Columns: ["File", "Color", "Linewidth", "Linestyle"], where
+        "File" is the absolute path to the file containing the coordinates to be
+        plotted. E.g: "/home/user/volcano_outlines.csv,black,0.5,-". Each .csv
+        coordinate file should contain coordinates only, with columns: ["Longitude",
+        "Latitude"]. E.g.: "-17.5,64.8". Lines pre-pended with ``#`` will be treated as
+        a comment - this can be used to include references. See the
         Volcanotectonic_Iceland example XY_files for a template.\n
         .. note:: Do not include a header line in either file.
     plot_all_stns : bool, optional
-        If true, plot all stations used for detect. Otherwise, only plot
-        stations which for which some data was available during the trigger
-        time window. NOTE: if no station availability data is found, all
-        stations in the LUT will be plotted. (Default, True)
+        If true, plot all stations used for detect. Otherwise, only plot stations which
+        for which some data was available during the trigger time window. NOTE: if no
+        station availability data is found, all stations in the LUT will be plotted.
+        (Default, True)
 
     """
 
     dt = pd.to_datetime(data["DT"].astype(str)).values
 
     fig = plt.figure(figsize=(30, 15))
     gs = (9, 18)
@@ -99,16 +108,17 @@
         ax = plt.subplot2grid(gs, (row, 8), colspan=10, rowspan=3, fig=fig)
         ax.set_xlim([starttime.datetime, endtime.datetime])
 
     # --- Plot LUT, coalescence traces, and station availability ---
     for ax in fig.axes[:2]:
         ax.get_shared_x_axes().join(ax, fig.axes[2])
     _plot_coalescence(fig.axes[0], dt, data.COA.values, "Maximum coalescence")
-    _plot_coalescence(fig.axes[1], dt, data.COA_N.values,
-                      "Normalised maximum coalescence")
+    _plot_coalescence(
+        fig.axes[1], dt, data.COA_N.values, "Normalised maximum coalescence"
+    )
     try:
         availability = read_availability(run, starttime, endtime)
         _plot_station_availability(fig.axes[2], availability, endtime)
     except util.NoStationAvailabilityDataException as e:
         logging.info(e)
         availability = None
 
@@ -128,42 +138,49 @@
 
     # --- Plot xy files on map ---
     _plot_xy_files(xy_files, fig.axes[3])
 
     # --- Plot trigger region (if any) ---
     if region is not None:
         _plot_trigger_region(fig.axes[3:], region)
-        _plot_event_windows(fig.axes[:2], discarded_events, marginal_window,
-                            discarded=True)
+        _plot_event_windows(
+            fig.axes[:2], discarded_events, marginal_window, discarded=True
+        )
         _plot_event_scatter(fig, discarded_events, discarded=True)
 
-
     # --- Plot event scatter on LUT and windows on coalescence traces ---
     if events is not None:
         _plot_event_windows(fig.axes[:2], events, marginal_window)
         _plot_event_scatter(fig, events)
 
         # Add trigger threshold to the correct coalescence trace
         ax_i = 1 if normalise_coalescence else 0
-        fig.axes[ax_i].step(dt, detection_threshold, where="mid", c="g",
-                        label="Detection threshold")
+        fig.axes[ax_i].step(
+            dt, detection_threshold, where="mid", c="g", label="Detection threshold"
+        )
 
     # --- Write summary information ---
     text = plt.subplot2grid(gs, (0, 0), colspan=8, rowspan=2, fig=fig)
     st, et = [t.strftime("%Y-%m-%d %H:%M:%S") for t in (starttime, endtime)]
-    text.text(0.42, 0.8, f"{st}  -  {et}", fontsize=20, fontweight="bold",
-              ha="center")
-    _plot_text_summary(text, events, detection_threshold, marginal_window,
-                       min_event_interval, normalise_coalescence)
+    text.text(0.42, 0.8, f"{st}  -  {et}", fontsize=20, fontweight="bold", ha="center")
+    _plot_text_summary(
+        text,
+        events,
+        detection_threshold,
+        marginal_window,
+        min_event_interval,
+        normalise_coalescence,
+    )
 
     # --- Handle legend for coalescence trace plot ---
     handles, labels = fig.axes[ax_i].get_legend_handles_labels()
     uniq_labels = dict(zip(labels, handles))
-    fig.axes[ax_i].legend(uniq_labels.values(), uniq_labels.keys(), loc=1,
-                          fontsize=14, framealpha=0.85).set_zorder(20)
+    fig.axes[ax_i].legend(
+        uniq_labels.values(), uniq_labels.keys(), loc=1, fontsize=14, framealpha=0.85
+    ).set_zorder(20)
 
     fig.tight_layout(pad=1, h_pad=0)
     plt.subplots_adjust(wspace=0.3, hspace=0.3)
 
     # --- Adjust cross sections to match map aspect ratio ---
     # Get left, bottom, width, height of each subplot bounding box
     xy_left, xy_bottom, xy_width, xy_height = fig.axes[3].get_position().bounds
@@ -175,16 +192,15 @@
     # Adjust bottom of xz cross section (if bottom of map has moved up)
     new_xz_bottom = xy_bottom - hdiff - xz_h
     fig.axes[4].set_position([xy_left, new_xz_bottom, xy_width, xz_h])
     # Adjust left of yz cross section (if right side of map has moved left)
     new_yz_left = xy_left + xy_width + wdiff
     # Take this opportunity to ensure the height of both cross sections is
     # equal by adjusting yz width (almost there from gridspec maths already)
-    new_yz_width = xz_h * (fig.get_size_inches()[1]
-                           / fig.get_size_inches()[0])
+    new_yz_width = xz_h * (fig.get_size_inches()[1] / fig.get_size_inches()[0])
     fig.axes[5].set_position([new_yz_left, xy_bottom, new_yz_width, xy_height])
 
     # Save figure
     fpath = run.path / "trigger" / run.subname / "summaries"
     fpath.mkdir(exist_ok=True, parents=True)
     fstem = f"{run.name}_{starttime.year}_{starttime.julday:03d}_Trigger"
     file = (fpath / fstem).with_suffix(".pdf")
@@ -194,49 +210,53 @@
         plt.show()
 
     plt.close(fig)
 
 
 def _plot_station_availability(ax, availability, endtime):
     """
-    Utility function to handle all aspects of plotting the station
-    availability.
+    Utility function to handle all aspects of plotting the station availability.
 
     Parameters
     ----------
     ax : `matplotlib.Axes` object
         Axes on which to plot the waveform gather.
     availability : `pandas.DataFrame` object
         Dataframe containing the availability of stations through time.
     endtime : `obspy.UTCDateTime`
         End time of trigger run.
 
     """
 
     # Get list of phases from station availability dataframe
-    phases = sorted(set([col_name.split("_")[1] for col_name in \
-        availability.columns]))
+    phases = sorted(set([col_name.split("_")[1] for col_name in availability.columns]))
     logging.debug(f"\t\t    Found phases: {phases}")
 
     # Sort out plotting options based on the number of phases
     if len(phases) > 2:
-        logging.warning("\t\t    Only P and/or S are currently supported! "
-                        "Plotting by station only.")
+        logging.warning(
+            "\t\t    Only P and/or S are currently supported! "
+            "Plotting by station only."
+        )
         phases = ["*"]
         colours = ["green"]
         divideby = len(phases)
     elif len(phases) == 1:
         if phases[0] == "P":
             colours = ["#F03B20"]
         else:
             colours = ["#3182BD"]
-    elif (availability.filter(like=f"_{phases[0]}").values ==
-          availability.filter(like=f"_{phases[1]}").values).all():
-        logging.info("\t\t    Station availability is identical for both "
-                     "phases; plotting by station only.")
+    elif (
+        availability.filter(like=f"_{phases[0]}").values
+        == availability.filter(like=f"_{phases[1]}").values
+    ).all():
+        logging.info(
+            "\t\t    Station availability is identical for both "
+            "phases; plotting by station only."
+        )
         divideby = len(phases)
         phases = ["*"]
         colours = ["green"]
     else:
         colours = ["#F03B20", "#3182BD"]
 
     # Loop through phases and plot
@@ -262,17 +282,16 @@
         ax.step(times, available, c=colour, where="post", label=phase)
 
         max_ava.append(max(available))
         min_ava.append(min(available))
 
     # Plot formatting
     _add_plot_tag(ax, "Station availability")
-    ax.set_ylim([int(min(min_ava)*0.8), int(np.ceil(max(max_ava)*1.1))])
-    ax.set_yticks(range(int(min(min_ava)*0.8),
-                        int(np.ceil(max(max_ava)*1.1))+1))
+    ax.set_ylim([int(min(min_ava) * 0.8), int(np.ceil(max(max_ava) * 1.1))])
+    ax.set_yticks(range(int(min(min_ava) * 0.8), int(np.ceil(max(max_ava) * 1.1)) + 1))
     ax.xaxis.set_major_formatter(util.DateFormatter("%H:%M:%S.{ms}", 2))
     ax.set_xlabel("DateTime", fontsize=14)
     ax.set_ylabel("Available stations", fontsize=14)
     if phases[0] != "*":
         ax.legend(loc=1, fontsize=14, framealpha=0.85).set_zorder(20)
 
 
@@ -289,16 +308,15 @@
     data : array-like
         Coalescence data to plot.
     label : str
         y-axis label.
 
     """
 
-    ax.plot(dt, data, c="k", lw=0.01, label="Coalesence value", alpha=0.8,
-            zorder=10)
+    ax.plot(dt, data, c="k", lw=0.01, label="Coalesence value", alpha=0.8, zorder=10)
     _add_plot_tag(ax, label)
     ax.set_ylabel(label, fontsize=14)
     ax.xaxis.set_major_formatter(util.DateFormatter("%H:%M:%S.{ms}", 2))
 
 
 def _add_plot_tag(ax, tag):
     """
@@ -309,33 +327,41 @@
     ax : `matplotlib.Axes` object
         Axes on which to plot the tag.
     tag : str
         Text to go in the tag.
 
     """
 
-    ax.text(0.01, 0.925, tag, ha="left", va="center", transform=ax.transAxes,
-            bbox=dict(boxstyle="round", fc="w", alpha=0.8), fontsize=18,
-            zorder=20)
+    ax.text(
+        0.01,
+        0.925,
+        tag,
+        ha="left",
+        va="center",
+        transform=ax.transAxes,
+        bbox=dict(boxstyle="round", fc="w", alpha=0.8),
+        fontsize=18,
+        zorder=20,
+    )
 
 
 def _plot_event_scatter(fig, events, discarded=False):
     """
-    Utility function for plotting the triggered events as a scatter on the
-    LUT map and cross-sections.
+    Utility function for plotting the triggered events as a scatter on the LUT map and
+    cross-sections.
 
     Parameters
     ----------
     fig : `matplotlib.Figure` object
         Figure containing axes on which to plot event scatter.
     events : `pandas.DataFrame` object
         Dataframe of triggered events.
     discarded : bool, optional
-         Whether supplied events are discarded (due to being outside the trigger
-         region, or outside the trigger time window).
+        Whether supplied events are discarded (due to being outside the trigger region,
+        or outside the trigger time window).
 
     """
 
     if discarded:
         x, y, z = events[["COA_X", "COA_Y", "COA_Z"]].values.T
         # Plot on XY
         fig.axes[3].scatter(x, y, s=50, c="grey")
@@ -343,73 +369,85 @@
         fig.axes[4].scatter(x, z, s=50, c="grey")
         # Plot on YZ
         fig.axes[5].scatter(z, y, s=50, c="grey")
 
     else:
         # Get bounds for cmap - hack to prevent inconsistent color being
         # assigned when only a single event has been triggered.
-        vmin, vmax = (events["TRIG_COA"].min() * 0.999,
-                    events["TRIG_COA"].max() * 1.001)
+        vmin, vmax = (
+            events["TRIG_COA"].min() * 0.999,
+            events["TRIG_COA"].max() * 1.001,
+        )
 
         # Plotting the scatter of the earthquake locations
         x, y, z = events[["COA_X", "COA_Y", "COA_Z"]].values.T
         c = events["TRIG_COA"].values
         sc = fig.axes[3].scatter(x, y, s=50, c=c, vmin=vmin, vmax=vmax)
         fig.axes[4].scatter(x, z, s=50, c=c, vmin=vmin, vmax=vmax)
         fig.axes[5].scatter(z, y, s=50, c=c, vmin=vmin, vmax=vmax)
 
         # --- Add colourbar ---
         cax = plt.subplot2grid((9, 18), (7, 5), colspan=2, rowspan=2, fig=fig)
         cax.set_axis_off()
-        cb = fig.colorbar(sc, ax=cax, orientation="horizontal", fraction=0.8,
-                        aspect=8)
+        cb = fig.colorbar(sc, ax=cax, orientation="horizontal", fraction=0.8, aspect=8)
         cb.ax.set_xlabel("Peak coalescence value", rotation=0, fontsize=14)
 
 
 def _plot_event_windows(axes, events, marginal_window, discarded=False):
     """
-    Utility function for plotting the marginal event window and minimum event
-    interval for triggered events.
+    Utility function for plotting the marginal event window and minimum event interval
+    for triggered events.
 
     Parameters
     ----------
     axes : list of `matplotlib.Axes` objects
         Axes on which to plot the event windows.
     events : `pandas.DataFrame` object
         Dataframe of triggered events.
     marginal_window : float
         Estimate of time error over which to marginalise the coalescence.
     discarded : bool, optional
-        Whether supplied events are discarded (due to being outside the trigger
-        region, or outside the trigger time window).
+        Whether supplied events are discarded (due to being outside the trigger region,
+        or outside the trigger time window).
 
     """
 
     for _, event in events.iterrows():
         min_dt = event["MinTime"].datetime
         max_dt = event["MaxTime"].datetime
         mw_stt = (event["CoaTime"] - marginal_window).datetime
         mw_end = (event["CoaTime"] + marginal_window).datetime
         for ax in axes:
             if discarded:
                 ax.axvspan(min_dt, max_dt, alpha=0.2, color="grey")
-                ax.axvline(event["CoaTime"].datetime, lw=0.01, alpha=0.4,
-                           color="grey")
+                ax.axvline(event["CoaTime"].datetime, lw=0.01, alpha=0.4, color="grey")
             else:
-                ax.axvspan(min_dt, mw_stt, label="Minimum event interval",
-                           alpha=0.2, color="#F03B20")
+                ax.axvspan(
+                    min_dt,
+                    mw_stt,
+                    label="Minimum event interval",
+                    alpha=0.2,
+                    color="#F03B20",
+                )
                 ax.axvspan(mw_end, max_dt, alpha=0.2, color="#F03B20")
-                ax.axvspan(mw_stt, mw_end, label="Marginal window", alpha=0.2,
-                           color="#3182BD")
-                ax.axvline(event["CoaTime"].datetime, label="Triggered event",
-                           lw=0.01, alpha=0.4, color="#1F77B4")
+                ax.axvspan(
+                    mw_stt, mw_end, label="Marginal window", alpha=0.2, color="#3182BD"
+                )
+                ax.axvline(
+                    event["CoaTime"].datetime,
+                    label="Triggered event",
+                    lw=0.01,
+                    alpha=0.4,
+                    color="#1F77B4",
+                )
 
 
-def _plot_text_summary(ax, events, threshold, marginal_window,
-                       min_event_interval, normalise_coalescence):
+def _plot_text_summary(
+    ax, events, threshold, marginal_window, min_event_interval, normalise_coalescence
+):
     """
     Utility function to plot the trigger summary information.
 
     Parameters
     ----------
     ax : `matplotlib.Axes` object
         Axes on which to plot the text summary.
@@ -418,16 +456,16 @@
     threshold : array-like
         Coalescence value above which to trigger events.
     marginal_window : float
         Time window over which to marginalise the 4-D coalescence function.
     min_event_interval : float
         Minimum time interval between triggered events.
     normalise_coalescence : bool
-        If True, use coalescence normalised by the average coalescence value in
-        the 3-D grid at each timestep.
+        If True, use coalescence normalised by the average coalescence value in the 3-D
+        grid at each timestep.
 
     """
 
     # Get threshold info
     if len(set(threshold)) == 1:
         threshold = f"{threshold[0]} (static)"
     else:
@@ -440,84 +478,106 @@
     with plt.rc_context({"font.size": 18}):
         ax.text(0.45, 0.65, "Trigger threshold:", ha="right", va="center")
         ax.text(0.47, 0.65, f"{threshold}", ha="left", va="center")
         ax.text(0.45, 0.5, "Marginal window:", ha="right", va="center")
         ax.text(0.47, 0.5, f"{marginal_window} s", ha="left", va="center")
         ax.text(0.45, 0.35, "Minimum event interval:", ha="right", va="center")
         ax.text(0.47, 0.35, f"{min_event_interval} s", ha="left", va="center")
-        ax.text(0.42, 0.15, f"Triggered {count} event(s) on the {trig} trace.",
-                ha="center", va="center")
+        ax.text(
+            0.42,
+            0.15,
+            f"Triggered {count} event(s) on the {trig} trace.",
+            ha="center",
+            va="center",
+        )
     ax.set_axis_off()
 
 
 def _plot_trigger_region(axes, region):
     """
-    Utility function for plotting the bounding geographical box used to filter
-    triggered events.
+    Utility function for plotting the bounding geographical box used to filter triggered
+    events.
 
     Parameters
     ----------
     axes : list of `matplotlib.Axes` objects
         Axes on which to plot the bounding boxes.
     region : list
         Geographical region within which to trigger earthquakes.
 
     """
 
     min_x, min_y, min_z, max_x, max_y, max_z = region
 
     # Plot on XY
-    axes[0].plot([min_x, min_x, max_x, max_x, min_x],
-                 [min_y, max_y, max_y, min_y, min_y],
-                 linestyle="--", color="#238b45", linewidth=1.5)
+    axes[0].plot(
+        [min_x, min_x, max_x, max_x, min_x],
+        [min_y, max_y, max_y, min_y, min_y],
+        linestyle="--",
+        color="#238b45",
+        linewidth=1.5,
+    )
 
     # Plot on XZ
-    axes[1].plot([min_x, min_x, max_x, max_x, min_x],
-                 [min_z, max_z, max_z, min_z, min_z],
-                 linestyle="--", color="#238b45", linewidth=1.5)
+    axes[1].plot(
+        [min_x, min_x, max_x, max_x, min_x],
+        [min_z, max_z, max_z, min_z, min_z],
+        linestyle="--",
+        color="#238b45",
+        linewidth=1.5,
+    )
 
     # Plot on YZ
-    axes[2].plot([min_z, max_z, max_z, min_z, min_z],
-                 [min_y, min_y, max_y, max_y, min_y],
-                 linestyle="--", color="#238b45", linewidth=1.5)
+    axes[2].plot(
+        [min_z, max_z, max_z, min_z, min_z],
+        [min_y, min_y, max_y, max_y, min_y],
+        linestyle="--",
+        color="#238b45",
+        linewidth=1.5,
+    )
 
 
 def _plot_xy_files(xy_files, ax):
     """
     Plot xy files supplied by user.
 
-    The user can specify a list of xy files to plot by supplying a csv file
-    with columns: ["File", "Color", "Linewidth", "Linestyle"], where "File" is
-    the absolute path to the file containing the coordinates to be plotted.
+    The user can specify a list of xy files to plot by supplying a csv file with
+    columns: ["File", "Color", "Linewidth", "Linestyle"], where "File" is the absolute
+    path to the file containing the coordinates to be plotted.
     E.g: "/home/user/volcano_outlines.csv,black,0.5,-"
 
     Each specified xy file should contain coordinates only, with columns:
     ["Longitude", "Latitude"]. E.g.: "-17.5,64.8".
 
-    Lines pre-pended with `#` will be treated as a comment - this can be used
-    to include references. See the Volcanotectonic_Iceland example XY_files for
-    a template.\n
+    Lines pre-pended with `#` will be treated as a comment - this can be used to include
+    references. See the Volcanotectonic_Iceland example XY_files for a template.\n
 
     .. note:: Do not include a header line in either file.
 
     Parameters
     ----------
     xy_files : str
-        Path to .csv file containing a list of coordinates files to plot, and
-        the linecolor and style to plot them with.
+        Path to .csv file containing a list of coordinates files to plot, and the
+        linecolor and style to plot them with.
     ax : `matplotlib.Axes` object
         Axes on which to plot the xy files.
 
     """
 
     if xy_files is not None:
-        xy_files = pd.read_csv(xy_files,
-                               names=["File", "Color",
-                                      "Linewidth", "Linestyle"],
-                               header=None, comment="#")
+        xy_files = pd.read_csv(
+            xy_files,
+            names=["File", "Color", "Linewidth", "Linestyle"],
+            header=None,
+            comment="#",
+        )
         for _, f in xy_files.iterrows():
-            xy_file = pd.read_csv(f["File"], names=["Longitude",
-                                                    "Latitude"],
-                                  header=None, comment="#")
-            ax.plot(xy_file["Longitude"], xy_file["Latitude"],
-                    ls=f["Linestyle"], lw=f["Linewidth"],
-                    c=f["Color"])
+            xy_file = pd.read_csv(
+                f["File"], names=["Longitude", "Latitude"], header=None, comment="#"
+            )
+            ax.plot(
+                xy_file["Longitude"],
+                xy_file["Latitude"],
+                ls=f["Linestyle"],
+                lw=f["Linewidth"],
+                c=f["Color"],
+            )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quakemigrate-1.0.1/quakemigrate/signal/__init__.py` & `quakemigrate-1.0.2/quakemigrate/signal/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # -*- coding: utf-8 -*-
 """
-The :mod:`quakemigrate.signal` module handles the core of the QuakeMigrate
-methods. This includes:
+The :mod:`quakemigrate.signal` module handles the core of the QuakeMigrate methods.
+This includes:
 
     * Generation of onset functions from raw data.
     * Picking of waveforms from onset functions.
     * Migration of onsets for detect() and locate().
     * Measurement of phase amplitudes and calculation of local earthquake \
       magnitudes.
 
 :copyright:
-    2020 - 2021, QuakeMigrate developers.
+    2020–2023, QuakeMigrate developers.
 :license:
     GNU General Public License, Version 3
     (https://www.gnu.org/licenses/gpl-3.0.html)
 
 """
 
 from .scan import QuakeScan  # NOQA
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quakemigrate-1.0.1/quakemigrate/signal/local_mag/__init__.py` & `quakemigrate-1.0.2/quakemigrate/signal/local_mag/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # -*- coding: utf-8 -*-
 """
-The :mod:`quakemigrate.local_mag` extension module handles the calculation of
-local magnitudes from Wood-Anderson simulated waveforms.
+The :mod:`quakemigrate.local_mag` extension module handles the calculation of local
+magnitudes from Wood-Anderson simulated waveforms.
 
 .. warning:: The local_mag modules are an ongoing work in progress. We hope to\
  continue to extend their functionality, which may result in some API changes.\
  If you have comments or suggestions, please contact the QuakeMigrate \
-developers at: quakemigrate.developers@gmail.com , or submit an issue on \
+developers at: quakemigrate.developers@gmail.com, or submit an issue on \
 GitHub.
 
 :copyright:
-    2020 - 2021, QuakeMigrate developers.
+    2020–2023, QuakeMigrate developers.
 :license:
     GNU General Public License, Version 3
     (https://www.gnu.org/licenses/gpl-3.0.html)
 
 """
 
 from .local_mag import LocalMag  # NOQA
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quakemigrate-1.0.1/quakemigrate/signal/local_mag/amplitude.py` & `quakemigrate-1.0.2/quakemigrate/signal/local_mag/amplitude.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """
-Module containing methods to measure Wood-Anderson corrected waveform
-amplitudes to be used for local magnitude calculation.
+Module containing methods to measure Wood-Anderson corrected waveform amplitudes to be
+used for local magnitude calculation.
 
 :copyright:
-    2020 - 2021, QuakeMigrate developers.
+    2020–2023, QuakeMigrate developers.
 :license:
     GNU General Public License, Version 3
     (https://www.gnu.org/licenses/gpl-3.0.html)
 
 """
 
 import logging
@@ -20,434 +20,450 @@
 from scipy.signal import find_peaks, iirfilter, sosfreqz, hilbert
 
 import quakemigrate.util as util
 
 
 class Amplitude:
     """
-    Part of the QuakeMigrate LocalMag class; measures Wood-Anderson corrected
-    waveform amplitudes to be used for local magnitude calculation.
+    Part of the QuakeMigrate LocalMag class; measures Wood-Anderson corrected waveform
+    amplitudes to be used for local magnitude calculation.
 
-    Simulates the Wood-Anderson waveforms using a user-supplied set of response
-    removal parameters, then measures the maximum peak-to-trough amplitude in
-    time windows around the P and S phase arrivals. These windows are
-    calculated from the phase pick times from the autopicker, if available, or
-    from the modelled pick times. The length of the S-wave signal window is
-    calculated according to a user-specified `signal_window` parameter.
-
-    The user may optionally specify a filter to apply to the waveforms before
-    amplitudes are measured, in order (for example) to reduce the impact of
-    high-amplitude noise associated with the oceanic microseisms on the
-    measurement of low-amplitude wavetrains associated with microseismic
-    events. Note this will generally result in an underestimate of the true
-    earthquake waveform amplitude, even when the filter gain is corrected for.
-
-    A measurement of the signal amplitude in a window preceding the P-wave
-    arrival is used to characterise the "noise" amplitude. This can be used
-    to filter out null observations, and to provide an estimate of the
-    uncertainty on the max amplitude measurements contributed by extraneous
-    noise.
+    Simulates the Wood-Anderson waveforms using a user-supplied set of response removal
+    parameters, then measures the maximum peak-to-trough amplitude in time windows
+    around the P and S phase arrivals. These windows are calculated from the phase pick
+    times from the autopicker, if available, or from the modelled pick times. The length
+    of the S-wave signal window is calculated according to a user-specified
+    `signal_window` parameter.
+
+    The user may optionally specify a filter to apply to the waveforms before amplitudes
+    are measured, in order (for example) to reduce the impact of high-amplitude noise
+    associated with the oceanic microseisms on the measurement of low-amplitude
+    wavetrains associated with microseismic events. Note this will generally result in
+    an underestimate of the true earthquake waveform amplitude, even when the filter
+    gain is corrected for.
+
+    A measurement of the signal amplitude in a window preceding the P-wave arrival is
+    used to characterise the "noise" amplitude. This can be used to filter out null
+    observations, and to provide an estimate of the uncertainty on the max amplitude
+    measurements contributed by extraneous noise.
 
     Attributes
     ----------
     signal_window : float
-        Length of S-wave signal window, in addition to the time window
-        associated with the marginal_window and traveltime uncertainty.
-        (Default 0 s)
+        Length of S-wave signal window, in addition to the time window associated with
+        the marginal_window and traveltime uncertainty. (Default 0 s)
     noise_window : float
-        Length of the time window before the P-wave signal window in which
-        to measure the noise amplitude. (Default 5 s)
+        Length of the time window before the P-wave signal window in which to measure
+        the noise amplitude. (Default 5 s)
     noise_measure : {"RMS", "STD", "ENV"}
-        Method by which to measure the noise amplitude; root-mean-quare,
-        standard deviation or average amplitude of the envelope of the signal.
-        (Default "RMS")
+        Method by which to measure the noise amplitude; root-mean-quare, standard
+        deviation or average amplitude of the envelope of the signal. (Default "RMS")
     loc_method : {"spline", "gaussian", "covariance"}
         Which event location estimate to use. (Default "spline")
     highpass_filter : bool
-        Whether to apply a high-pass filter before measuring amplitudes.
-        (Default False)
+        Whether to apply a high-pass filter before measuring amplitudes. (Default False)
     highpass_freq : float
         High-pass filter frequency. Required if highpass_filter is True.
     bandpass_filter : bool
-        Whether to apply a band-pass filter before measuring amplitudes.
-        (Default False)
+        Whether to apply a band-pass filter before measuring amplitudes. (Default False)
     bandpass_lowcut : float
-        Band-pass filter low-cut frequency. Required if bandpass_filter is
-        True.
+        Band-pass filter low-cut frequency. Required if bandpass_filter is True.
     bandpass_highcut : float
-        Band-pass filter high-cut frequency. Required if bandpass_filter is
-        True.
+        Band-pass filter high-cut frequency. Required if bandpass_filter is True.
     filter_corners : int
         number of corners for the chosen filter. (Default 4)
     prominence_multiplier : float
-        To set a prominence filter in the peak-finding algorithm.
-        (Default 0. = off)
+        To set a prominence filter in the peak-finding algorithm. (Default 0. = off)
         NOTE: not recommended for use in combination with a filter; filter gain
         corrections can lead to spurious results. Please see the
         `scipy.signal.find_peaks` documentation for further guidance.
 
     Methods
     -------
     get_amplitudes(event, lut)
 
     Raises
     ------
     AttributeError
-        If both `highpass_filter` and `bandpass_filter` are selected, or if the
-        user selects to apply a filter but does not provide the relevant
-        frequencies.
+        If both `highpass_filter` and `bandpass_filter` are selected, or if the user
+        selects to apply a filter but does not provide the relevant frequencies.
     AttributeError
         If response removal parameters are provided here instead of to the
         :class:`~quakemigrate.io.data.Archive` object.
 
     """
 
     def __init__(self, amplitude_params={}):
         """Instantiate the Amplitude object."""
 
         # Amplitude measurement parameters
         if "signal_window" not in amplitude_params.keys():
-            msg = ("Warning: 'signal_window' not specified. Set to default: 0")
-            logging.warning(msg)
-        self.signal_window = amplitude_params.get("signal_window", 0.)
+            logging.warning("Warning: 'signal_window' not specified. Set to default: 0")
+        self.signal_window = amplitude_params.get("signal_window", 0.0)
 
-        self.noise_window = amplitude_params.get("noise_window", 5.)
+        self.noise_window = amplitude_params.get("noise_window", 5.0)
         self.noise_measure = amplitude_params.get("noise_measure", "RMS")
 
-        self.prominence_multiplier = \
-            amplitude_params.get("prominence_multiplier", 0.)
+        self.prominence_multiplier = amplitude_params.get("prominence_multiplier", 0.0)
         self.loc_method = amplitude_params.get("loc_method", "spline")
 
         # Pre-processing parameters
         self.highpass_filter = amplitude_params.get("highpass_filter", False)
         if self.highpass_filter:
             try:
                 self.highpass_freq = amplitude_params["highpass_freq"]
             except KeyError as e:
-                msg = f"Highpass filter frequency not specified! {e}"
-                raise AttributeError(msg)
+                raise AttributeError(f"Highpass filter frequency not specified! {e}")
 
         self.bandpass_filter = amplitude_params.get("bandpass_filter", False)
         if self.bandpass_filter:
             try:
                 self.bandpass_lowcut = amplitude_params.get("bandpass_lowcut")
                 self.bandpass_highcut = amplitude_params.get("bandpass_highcut")
             except KeyError as e:
-                msg = f"Bandpass filter frequencies not specified! {e}"
-                raise AttributeError(msg)
+                raise AttributeError(f"Bandpass filter frequencies not specified! {e}")
         self.filter_corners = amplitude_params.get("filter_corners", 4)
 
         if self.highpass_filter and self.bandpass_filter:
-            msg = ("Both bandpass filter *and* highpass filter selected! "
-                   "Please choose one or the other.")
-            raise AttributeError(msg)
+            raise AttributeError(
+                "Both bandpass filter *and* highpass filter selected! "
+                "Please choose one or the other."
+            )
 
         # Handle deprecated response removal parameters
-        if any(param in amplitude_params.keys() for param in \
-            ["water_level", "pre_filt", "remove_full_response"]):
-            raise AttributeError("The response removal parameters "
-                                 "('water_level', 'pre_filt', "
-                                 "'remove_full_response') have been moved to "
-                                 "the Archive object. Please specify them "
-                                 "there as e.g. 'archive.water_level = 60.' or"
-                                 " by providing a dictionary of "
-                                 "response_removal parameters - see the "
-                                 "template locate script for guidance.")
+        if any(
+            param in amplitude_params.keys()
+            for param in ["water_level", "pre_filt", "remove_full_response"]
+        ):
+            raise AttributeError(
+                "The response removal parameters ('water_level', 'pre_filt', "
+                "'remove_full_response') have been moved to the Archive object. Please "
+                "specify them there as e.g. 'archive.water_level = 60.' or by "
+                "providing a dictionary of response_removal parameters - see the "
+                "template locate script for guidance."
+            )
 
     def __str__(self):
         """Return short summary string of the Amplitude object."""
 
-        out = ("\t    Amplitude parameters:\n"
-               f"\t\tSignal window    = {self.signal_window} s\n"
-               f"\t\tNoise window     = {self.noise_window} s\n"
-               f"\t\tNoise measure    = {self.noise_measure}\n"
-               f"\t\tLocation used    = {self.loc_method}\n")
-        if self.prominence_multiplier != 0.:
+        out = (
+            "\t    Amplitude parameters:\n"
+            f"\t\tSignal window    = {self.signal_window} s\n"
+            f"\t\tNoise window     = {self.noise_window} s\n"
+            f"\t\tNoise measure    = {self.noise_measure}\n"
+            f"\t\tLocation used    = {self.loc_method}\n"
+        )
+        if self.prominence_multiplier != 0.0:
             out += f"\t\tProminence multiplier = {self.prominence_multiplier}"
             out += "\n"
         if self.highpass_filter:
-            out += ("\t\tHighpass filter: \n"
-                    f"\t\t    Filter frequency = {self.highpass_freq} Hz\n"
-                    f"\t\t    Filter corners   = {self.filter_corners}\n")
+            out += (
+                "\t\tHighpass filter: \n"
+                f"\t\t    Filter frequency = {self.highpass_freq} Hz\n"
+                f"\t\t    Filter corners   = {self.filter_corners}\n"
+            )
         elif self.bandpass_filter:
-            out += ("\t\tBandpass filter: \n"
-                    f"\t\t    Lowcut frequency  = {self.bandpass_lowcut} Hz\n"
-                    f"\t\t    Highcut frequency = {self.bandpass_highcut} Hz\n"
-                    f"\t\t    Filter corners    = {self.filter_corners}\n")
+            out += (
+                "\t\tBandpass filter: \n"
+                f"\t\t    Lowcut frequency  = {self.bandpass_lowcut} Hz\n"
+                f"\t\t    Highcut frequency = {self.bandpass_highcut} Hz\n"
+                f"\t\t    Filter corners    = {self.filter_corners}\n"
+            )
 
         return out
 
     @util.timeit()
     def get_amplitudes(self, event, lut):
         """
         Measure phase amplitudes for an event.
 
         Parameters
         ----------
         event : :class:`~quakemigrate.io.event.Event` object
-            Light class encapsulating waveforms, coalescence information, picks
-            and location information for a given event.
+            Light class encapsulating waveforms, coalescence information, picks and
+            location information for a given event.
         lut : :class:`~quakemigrate.lut.lut.LUT` object
-            Contains the traveltime lookup tables for seismic phases, computed
-            for some pre-defined velocity model.
+            Contains the traveltime lookup tables for seismic phases, computed for some
+            pre-defined velocity model.
 
         Returns
         -------
         amplitudes : `pandas.DataFrame` object
-            P- and S-wave amplitude measurements for each component of each
-            station in the look-up table.
+            P- and S-wave amplitude measurements for each component of each station in
+            the look-up table.
             Columns:
                 epi_dist : float
-                    Epicentral distance between the station and the event
-                    hypocentre.
+                    Epicentral distance between the station and the event hypocentre.
                 z_dist : float
-                    Vertical distance between the station and the event
-                    hypocentre.
+                    Vertical distance between the station and the event hypocentre.
                 P_amp : float
-                    Half maximum peak-to-trough amplitude in the P signal
-                    window. In *millimetres*. Corrected for filter gain, if
-                    applicable.
+                    Half maximum peak-to-trough amplitude in the P signal window. In
+                    *millimetres*. Corrected for filter gain, if applicable.
                 P_freq : float
-                    Approximate frequency of the maximum amplitude P-wave
-                    signal. Calculated from the peak-to-trough time interval of
-                    the max peak-to-trough amplitude.
+                    Approximate frequency of the maximum amplitude P-wave signal.
+                    Calculated from the peak-to-trough time interval of the max
+                    peak-to-trough amplitude.
                 P_time : `obspy.UTCDateTime` object
-                    Approximate time of amplitude observation (halfway between
-                    peak and trough times).
+                    Approximate time of amplitude observation (halfway between peak and
+                    trough times).
                 P_avg_amp : float
-                    Average amplitude in the P signal window, measured by the
-                    same method as the Noise_amp (see `noise_measure`) and
-                    corrected for the same filter gain as `P_amp`. In
-                    *millimetres*.
+                    Average amplitude in the P signal window, measured by the same
+                    method as the Noise_amp (see `noise_measure`) and corrected for the
+                    same filter gain as `P_amp`. In *millimetres*.
                 P_filter_gain : float or NaN
-                    Filter gain at `P_freq` - which has been corrected for in
-                    the P_amp measurements - if a filter was applied prior to
-                    amplitude measurement; Else NaN.
+                    Filter gain at `P_freq` - which has been corrected for in the P_amp
+                    measurements - if a filter was applied prior to amplitude
+                    measurement; Else NaN.
                 S_amp : float
                     As for P, but in the S wave signal window.
                 S_freq : float
                     As for P.
                 S_time : `obspy.UTCDateTime` object
                     As for P.
                 S_avg_amp : float
                     As for P.
                 S_filter_gain : float or NaN.
                     As for P.
                 Noise_amp : float
-                    The average signal amplitude in the noise window. In
-                    *millimetres*. See `noise_measure` parameter.
+                    The average signal amplitude in the noise window. In *millimetres*.
+                    See `noise_measure` parameter.
                 is_picked : bool
-                    Whether at least one of the phase arrivals was picked by
-                    the autopicker.
+                    Whether at least one of the phase arrivals was picked by the
+                    autopicker.
             Index = Trace ID (see `obspy.Trace` object property 'id')
 
         """
 
         # Initialise amplitudes DataFrame
-        amplitudes = pd.DataFrame(columns=["id", "epi_dist", "z_dist",
-                                           "P_amp", "P_freq", "P_time",
-                                           "P_avg_amp", "P_filter_gain",
-                                           "S_amp", "S_freq", "S_time",
-                                           "S_avg_amp", "S_filter_gain",
-                                           "Noise_amp", "is_picked"])
+        amplitudes = pd.DataFrame(
+            columns=[
+                "id",
+                "epi_dist",
+                "z_dist",
+                "P_amp",
+                "P_freq",
+                "P_time",
+                "P_avg_amp",
+                "P_filter_gain",
+                "S_amp",
+                "S_freq",
+                "S_time",
+                "S_avg_amp",
+                "S_filter_gain",
+                "Noise_amp",
+                "is_picked",
+            ]
+        )
 
         # Get event hypocentre location
         ev_loc = event.get_hypocentre(self.loc_method)
 
         # Get traveltimes for all stations and phases: much quicker than
         # doing this multiple times in the loop
         event_ijk = lut.index2coord(ev_loc, inverse=True)[0]
         try:
             p_ttimes = lut.traveltime_to("P", event_ijk)
             s_ttimes = lut.traveltime_to("S", event_ijk)
         except KeyError:
-            msg = ("Both P and S traveltimes are required to measure phase "
-                   "amplitudes for local magnitude calculation. Please create "
-                   "a new lookup table with phases=['P', 'S']")
-            raise util.LUTPhasesException(msg)
+            raise util.LUTPhasesException(
+                "Both P and S traveltimes are required to measure phase "
+                "amplitudes for local magnitude calculation. Please create "
+                "a new lookup table with phases=['P', 'S']"
+            )
 
         # Get start of earliest possible noise window and end of latest
         # possible signal window
         max_tt = lut.max_traveltime
-        pre_pad, post_pad = self.pad(event.marginal_window, max_tt,
-                                     lut.fraction_tt)
+        pre_pad, post_pad = self.pad(event.marginal_window, max_tt, lut.fraction_tt)
         tr_start = event.otime - pre_pad
         tr_end = event.otime + post_pad
         logging.debug(f"{tr_start}, {tr_end}, {event.otime}")
 
         # Loop through stations in LUT, calculating amplitude info
         for i, station_data in lut.station_data.iterrows():
             station = station_data["Name"]
 
-            epi_dist, z_dist = self._get_distances(ev_loc, station_data,
-                                                   lut.unit_conversion_factor)
+            epi_dist, z_dist = self._get_distances(
+                ev_loc, station_data, lut.unit_conversion_factor
+            )
 
             # Columns: tr_id, epicentral distance, vertical distance, P_amp,
             #          P_freq, P_time, P_noise_ratio, S_amp, S_freq, S_time,
             #          S_noise_ratio, Noise_amp, picked
-            amps_template = ["", epi_dist, z_dist, np.nan, np.nan, np.nan,
-                             np.nan, np.nan, np.nan, np.nan, np.nan, np.nan,
-                             np.nan, np.nan, False]
+            amps_template = [
+                "",
+                epi_dist,
+                z_dist,
+                np.nan,
+                np.nan,
+                np.nan,
+                np.nan,
+                np.nan,
+                np.nan,
+                np.nan,
+                np.nan,
+                np.nan,
+                np.nan,
+                np.nan,
+                False,
+            ]
 
             # Read in raw waveforms -- work on a copy!!
             st = event.data.raw_waveforms.select(station=station).copy()
             # Trim to padding window to ensure taper does not encroach on the
             # noise or signal window.
             st.trim(starttime=tr_start, endtime=tr_end)
 
             for j, comp in enumerate(["[E,2]", "[N,1]", "Z"]):
                 amps = amps_template.copy()
                 tr = st.select(component=comp)
                 # if trace is empty (no traces) or there is more than 1 (gaps),
                 # or data isn't continuous within the time window where data is
                 # needed to make the amplitude measurements, skip
-                if bool(tr) and len(tr) == 1 and \
-                    tr[0].stats.starttime < (tr_start + tr[0].stats.delta) \
-                    and tr[0].stats.endtime > (tr_end - tr[0].stats.delta):
+                if (
+                    bool(tr)
+                    and len(tr) == 1
+                    and tr[0].stats.starttime < (tr_start + tr[0].stats.delta)
+                    and tr[0].stats.endtime > (tr_end - tr[0].stats.delta)
+                ):
                     tr = tr[0]
                 else:
                     amps[0] = f".{station}..{comp}"
-                    amplitudes.loc[i*3+j] = amps
+                    amplitudes.loc[i * 3 + j] = amps
                     continue
 
                 amps[0] = tr.id
 
                 # Do response removal
                 try:
                     tr = event.data.get_wa_waveform(tr, velocity=False)
-                except (util.ResponseNotFoundError,
-                        util.ResponseRemovalError) as e:
+                except (util.ResponseNotFoundError, util.ResponseRemovalError) as e:
                     logging.warning(e)
-                    amplitudes.loc[i*3+j] = amps
+                    amplitudes.loc[i * 3 + j] = amps
                     continue
 
                 if self.bandpass_filter or self.highpass_filter:
                     filter_sos = self._filter_trace(tr)
                 else:
                     filter_sos = None
 
                 try:
                     windows, picked = self._get_amplitude_windows(
-                        station, i, event, p_ttimes, s_ttimes, lut.fraction_tt)
+                        station, i, event, p_ttimes, s_ttimes, lut.fraction_tt
+                    )
                     amps[14] = picked
                 except util.PickOrderException as e:
                     logging.warning(f"{e}")
-                    amplitudes.loc[i*3+j] = amps
+                    amplitudes.loc[i * 3 + j] = amps
                     continue
 
-                amps = self._measure_signal_amps(amps, tr, windows,
-                                                 self.noise_measure,
-                                                 filter_sos)
+                amps = self._measure_signal_amps(
+                    amps, tr, windows, self.noise_measure, filter_sos
+                )
 
-                noise_amp = self._measure_noise_amp(tr, windows,
-                                                    self.noise_measure)
+                noise_amp = self._measure_noise_amp(tr, windows, self.noise_measure)
                 amps[13] = noise_amp
 
                 # 3 rows per station; one for each component
-                amplitudes.loc[i*3+j] = amps
+                amplitudes.loc[i * 3 + j] = amps
 
         amplitudes = amplitudes.set_index("id")
 
         return amplitudes
 
     def _get_distances(self, ev_loc, station_data, unit_conversion_factor):
         """
-        Get epicentral and vertical distances between a station and an event
-        hypocentre.
+        Get epicentral and vertical distances between a station and an event hypocentre.
 
         Parameters
         ----------
         ev_loc : array-like
             Event hypocentre location in geographic coordinate system.
         station_data : `pandas.Series` object
-            Station information - keys: ["Name", "Latitude", "Longitude",
-            "Elevation"].
+            Station information - keys: ["Name", "Latitude", "Longitude", "Elevation"].
         unit_conversion_factor : float
-            A conversion factor based on the lookup table grid projection, used
-            to ensure the distances returned have units of kilometres.
+            A conversion factor based on the lookup table grid projection, used to
+            ensure the distances returned have units of kilometres.
 
         Returns
         -------
         epi_dist : float
             Epicentral distance between the station and the event hypocentre.
         z_dist : float
             Vertical distance between the station and the event hypocentre.
 
         """
 
         # Get station location
-        stla, stlo, stel = station_data[["Latitude",
-                                         "Longitude",
-                                         "Elevation"]].values
+        stla, stlo, stel = station_data[["Latitude", "Longitude", "Elevation"]].values
 
         # Get event location
         evlo, evla, evdp = ev_loc
 
         # Evaluate epicentral distance between station and event.
         # gps2dist_azimuth returns distances in metres -- magnitudes
         # calculation requires distances in kilometres.
         epi_dist = gps2dist_azimuth(evla, evlo, stla, stlo)[0] / 1000
 
-        # Evaulate vertical distance between station and event. Convert to
-        # kilometres.
+        # Evaulate vertical distance between station and event. Convert to kilometres.
         km_cf = 1000 / unit_conversion_factor
         z_dist = (evdp - stel) / km_cf  # NOTE: stel is actually depth.
 
         return epi_dist, z_dist
 
     def _filter_trace(self, tr):
         """
-        Apply a highpass or bandpass filter to the supplied Trace. Filtering is
-        applied in-place on the `obspy.Trace` object.
+        Apply a highpass or bandpass filter to the supplied Trace. Filtering is applied
+        in-place on the `obspy.Trace` object.
 
         Parameters
         ----------
         tr : `obspy.Trace` object
             Trace to be filtered
 
         Returns
         -------
         filter_sos : `numpy.ndarray`
             Second-order sections representation of the applied filter.
 
         """
 
-        # Try to apply bandpass filter, unless the specified lowpass frequency
-        # is higher than the Nyquist. In this case, apply a highpass.
+        # Try to apply bandpass filter, unless the specified lowpass frequency is higher
+        # than the Nyquist. In this case, apply a highpass.
         if self.bandpass_filter:
             try:
                 filter_sos = self._bandpass_filter(tr)
             except util.NyquistException as e:
                 logging.warning(f"\t{e} Applying a high-pass filter instead..")
                 filter_sos = self._highpass_filter(tr)
         else:
             filter_sos = self._highpass_filter(tr)
 
         return filter_sos
 
     def _bandpass_filter(self, tr):
         """
-        Apply a bandpass filter to the supplied `obspy.Trace` object; filter
-        operation is applied in-place.
+        Apply a bandpass filter to the supplied `obspy.Trace` object; filter operation
+        is applied in-place.
 
         Parameters
         ----------
         tr : `obspy.Trace` object
             Trace to be filtered.
 
         Returns
         -------
         filter_sos : `numpy.ndarray`
             Second-order sections representation of the applied filter.
 
         Raises
         ------
         NyquistException
-            If the high-cut filter specified for the bandpass filter is higher
-            than the Nyquist frequency of a trace.
+            If the high-cut filter specified for the bandpass filter is higher than the
+            Nyquist frequency of a trace.
 
         """
 
         freqmin = self.bandpass_lowcut
         freqmax = self.bandpass_highcut
         corners = self.filter_corners
 
@@ -457,22 +473,31 @@
         high_f_crit = freqmax / f_nyquist
         if high_f_crit - 1.0 > -1e-6:
             raise util.NyquistException(freqmax, f_nyquist, tr.id)
 
         # Pre-process and apply filter
         tr.detrend("linear")
         tr.taper(0.05, "cosine")
-        tr.filter(type="bandpass", freqmin=freqmin, freqmax=freqmax,
-                  corners=corners, zerophase=False)
-
-        # Generate filter coefficients for the bandpass filter we
-        # applied; this is how the filter is designed within ObsPy
-        filter_sos = iirfilter(N=corners, Wn=[low_f_crit, high_f_crit],
-                               btype="bandpass", ftype="butter",
-                               output="sos")
+        tr.filter(
+            type="bandpass",
+            freqmin=freqmin,
+            freqmax=freqmax,
+            corners=corners,
+            zerophase=False,
+        )
+
+        # Generate filter coefficients for the bandpass filter we applied; this is how
+        # the filter is designed within ObsPy
+        filter_sos = iirfilter(
+            N=corners,
+            Wn=[low_f_crit, high_f_crit],
+            btype="bandpass",
+            ftype="butter",
+            output="sos",
+        )
 
         return filter_sos
 
     def _highpass_filter(self, tr):
         """
         Apply a highpass filter to the supplied `obspy.Trace` object; filter
         operation is applied in-place.
@@ -485,45 +510,45 @@
         Returns
         -------
         filter_sos : `numpy.ndarray`
             Second-order sections representation of the applied filter.
 
         """
 
-        # Check if we have been diverted here from trying to apply a bandpass
-        # filter. Else use specified params for highpass.
+        # Check if we have been diverted here from trying to apply a bandpass filter.
+        # Else use specified params for highpass.
         if self.bandpass_filter:
             filt_freq = self.bandpass_lowcut
         else:
             filt_freq = self.highpass_freq
         corners = self.filter_corners
 
         f_nyquist = 0.5 * tr.stats.sampling_rate
         f_crit = filt_freq / f_nyquist
 
         # Pre-process and apply filter
         tr.detrend("linear")
         tr.taper(0.05, "cosine")
-        tr.filter(type="highpass", freq=filt_freq, corners=corners,
-                  zerophase=False)
+        tr.filter(type="highpass", freq=filt_freq, corners=corners, zerophase=False)
 
-        # Generate filter coefficients for the highpass filter we
-        # applied; this is how the filter is designed within ObsPy
-        filter_sos = iirfilter(N=corners, Wn=f_crit, btype="highpass",
-                               ftype="butter", output="sos")
+        # Generate filter coefficients for the highpass filter we applied; this is how
+        # the filter is designed within ObsPy
+        filter_sos = iirfilter(
+            N=corners, Wn=f_crit, btype="highpass", ftype="butter", output="sos"
+        )
 
         return filter_sos
 
-    def _get_amplitude_windows(self, station, i, event, p_ttimes, s_ttimes,
-                               fraction_tt):
-        """
-        Calculate the start and end time of the windows to measure the max P-
-        and S- wave amplitudes in. This is done on the basis of the pick times,
-        the event marginal window, the traveltime and uncertainty and the
-        specified S-wave signal window.
+    def _get_amplitude_windows(
+        self, station, i, event, p_ttimes, s_ttimes, fraction_tt
+    ):
+        """
+        Calculate the start and end time of the windows to measure the max P- and S-wave
+        amplitudes in. This is done on the basis of the pick times, the event marginal
+        window, the traveltime and uncertainty and the specified S-wave signal window.
 
         P_window_start : P_pick - marginal_window - traveltime_uncertainty
         P_window_end : equivalent to start, or S_pick time; whichever is
                        earlier
         S_window_start : same as P
         S_window_end : S_pick + signal_window + marginal_window +
                        traveltime_uncertainty
@@ -534,23 +559,23 @@
         Parameters
         ----------
         station : str
             Station name.
         i : int
             Iterator variable.
         event : :class:`~quakemigrate.io.event.Event` object
-            Light class encapsulating signal, onset, pick and location
-            information for a given event.
+            Light class encapsulating signal, onset, pick and location information for a
+            given event.
         p_ttimes : array-like
             Array of interpolated P traveltimes to the requested grid position.
         s_ttimes : array-like
             Array of interpolated S traveltimes to the requested grid position.
         fraction_tt : float
-            An estimate of the uncertainty in the velocity model as a function
-            of the traveltime.
+            An estimate of the uncertainty in the velocity model as a function of the
+            traveltime.
 
         Returns
         -------
         windows : array-like
             [[P_window_start, P_window_end], [S_window_start, S_window_end]]
         picked : bool
             Whether at least one of the phases was picked by the autopicker.
@@ -567,21 +592,23 @@
         for pick, phase in [[p_pick, "P"], [s_pick, "S"]]:
             if not isinstance(pick, UTCDateTime):
                 if pick == "-1":
                     if phase == "P":
                         p_pick = event.otime + p_ttimes[i]
                     else:
                         s_pick = event.otime + s_ttimes[i]
-                # If there was no onset available for one phase, the pick for
-                # the other may not have been checked to ensure it was made
-                # before/after the modelled arrival time for the other phase.
-                # So use modelled arrival time for both phases.
+                # If there was no onset available for one phase, the pick for the other
+                # may not have been checked to ensure it was made before/after the
+                # modelled arrival time for the other phase. So use modelled arrival
+                # time for both phases.
                 elif pick == f"No {phase} onset":
-                    logging.debug(f"No onset available when picking {phase} on "
-                                  f"{station}. Using modelled arrival times.")
+                    logging.debug(
+                        f"No onset available when picking {phase} on "
+                        f"{station}. Using modelled arrival times."
+                    )
                     p_pick = event.otime + p_ttimes[i]
                     s_pick = event.otime + s_ttimes[i]
                     break
 
         # Check p_pick is before s_pick
         try:
             assert p_pick < s_pick
@@ -589,51 +616,50 @@
             raise util.PickOrderException(event.uid, station, p_pick, s_pick)
 
         # For P:
         p_start = p_pick - event.marginal_window - p_ttimes[i] * fraction_tt
         p_end = p_pick + event.marginal_window + p_ttimes[i] * fraction_tt
         # For S:
         s_start = s_pick - event.marginal_window - s_ttimes[i] * fraction_tt
-        s_end = s_pick + event.marginal_window + s_ttimes[i] * fraction_tt + \
-            self.signal_window
+        s_end = (
+            s_pick
+            + event.marginal_window
+            + s_ttimes[i] * fraction_tt
+            + self.signal_window
+        )
 
         # Check for overlaps
         if s_start < p_end:
             mid_time = p_end + (s_start - p_end) / 2
-            windows = [[p_start, mid_time],
-                       [mid_time, s_end]]
+            windows = [[p_start, mid_time], [mid_time, s_end]]
         elif s_start - p_end < self.signal_window:
-            windows = [[p_start, s_start],
-                       [s_start, s_end]]
+            windows = [[p_start, s_start], [s_start, s_end]]
         else:
-            windows = [[p_start, p_end + self.signal_window],
-                       [s_start, s_end]]
+            windows = [[p_start, p_end + self.signal_window], [s_start, s_end]]
 
         return windows, picked
 
     def _get_picks(self, station, event):
         """
-        Get picks from this station for this event. If no phase pick is
-        found, -1 is returned. If no picks at all are found, "No <phase> onset"
-        is returned.
+        Get picks from this station for this event. If no phase pick is found, -1 is
+        returned. If no picks at all are found, "No <phase> onset" is returned.
 
         Parameters
         ----------
         station : str
             Station name.
         event : :class:`~quakemigrate.io.event.Event` object
-            Light class encapsulating waveforms, coalescence information, picks
-            and location information for a given event.
+            Light class encapsulating waveforms, coalescence information, picks and
+            location information for a given event.
 
         Returns
         -------
         p_pick : `obspy.UTCDateTime` object, "-1" or "No_P_onset"
-            P pick time. Autopick time if available, otherwise -1. If no onset
-            function was available to the autopicker, "No_<phase>_onset" is
-            returned.
+            P pick time. Autopick time if available, otherwise -1. If no onset function
+            was available to the autopicker, "No_<phase>_onset" is returned.
         s_pick : `obspy.UTCDateTime` object, "-1" or "No_S_onset"
             As for P.
         picked : bool
             Whether at least one phase was picked by the auto-picker.
 
         """
 
@@ -659,78 +685,71 @@
             except ValueError:  # UTCDateTime("-1") -> ValueError
                 s_pick = "-1"
         else:
             p_pick = s_pick = "-1"
 
         return p_pick, s_pick, picked
 
-    def _measure_signal_amps(self, amps, tr, windows, method="RMS",
-                             filter_sos=None):
+    def _measure_signal_amps(self, amps, tr, windows, method="RMS", filter_sos=None):
         """
-        Loop through the windows and measure the maximum half peak-to-peak
-        amplitude, the approximate frequency (derived from the p2p time) and
-        the time at which it occurs.
-
-        Performs a linear detrend across the window before measuring
-        amplitudes.
-
-        NOTE: signal amplitudes are returned in *millimetres*. This may mean
-        the formulation of the local magnitude attenuation function being used
-        needs to be adjusted to match these units. All functions provided in QM
-        are in millimetres.
+        Loop through the windows and measure the maximum half peak-to-peak amplitude,
+        the approximate frequency (derived from the p2p time) and the time at which it
+        occurs.
+
+        Performs a linear detrend across the window before measuring amplitudes.
+
+        NOTE: signal amplitudes are returned in *millimetres*. This may mean the
+        formulation of the local magnitude attenuation function being used needs to be
+        adjusted to match these units. All functions provided in QM are in millimetres.
 
         Parameters
         ----------
         amps : list
             Amplitude information for this trace.
-            Columns = ["epi_dist", "z_dist", "P_amp", "P_freq", "P_time",
-                       "P_avg_amp", "P_filter_gain", "S_amp", "S_freq",
-                       "S_time", "S_avg_amp", "S_filter_gain", "Noise_amp",
-                       "is_picked"]
+            Columns = ["epi_dist", "z_dist", "P_amp", "P_freq", "P_time", "P_avg_amp",
+                       "P_filter_gain", "S_amp", "S_freq", "S_time", "S_avg_amp",
+                       "S_filter_gain", "Noise_amp", "is_picked"]
         tr : `obspy.Trace` object
             Trace from which to measure amplitudes.
         windows : array-like
             [[P_window_start, P_window_end], [S_window_start, S_window_end]]
         method : {"RMS", "STD", "ENV"}, optional
-            The method by which to measure the average amplitude in the signal
-            window: root-mean-square, standard deviation or average amplitude
-            of the envelope of the signal. (Default "RMS")
+            The method by which to measure the average amplitude in the signal window:
+            root-mean-square, standard deviation or average amplitude of the envelope of
+            the signal. (Default "RMS")
         filter_sos : `numpy.ndarray`, optional
-            Second-order sections representation of the filter applied to the
-            trace (if applicable).
+            Second-order sections representation of the filter applied to the trace (if
+            applicable).
 
         Returns
         -------
         amps : list
             Amplitude information for this trace.
-            Columns = ["epi_dist", "z_dist", "P_amp", "P_freq", "P_time",
-                       "P_avg_amp", "P_filter_gain", "S_amp", "S_freq",
-                       "S_time", "S_avg_amp", "S_filter_gain", "Noise_amp",
-                       "is_picked"]
+            Columns = ["epi_dist", "z_dist", "P_amp", "P_freq", "P_time", "P_avg_amp",
+                       "P_filter_gain", "S_amp", "S_freq", "S_time", "S_avg_amp",
+                       "S_filter_gain", "Noise_amp", "is_picked"]
             With newly populated values:
                 P_amp : float
-                    Half maximum peak-to-trough amplitude in the P signal
-                    window. In *millimetres*. Corrected for filter gain, if
-                    applicable.
+                    Half maximum peak-to-trough amplitude in the P signal window. In
+                    *millimetres*. Corrected for filter gain, if applicable.
                 P_freq : float
-                    Approximate frequency of the maximum amplitude P-wave
-                    signal. Calculated from the peak-to-trough time interval of
-                    the max peak-to-trough amplitude.
+                    Approximate frequency of the maximum amplitude P-wave signal.
+                    Calculated from the peak-to-trough time interval of the max
+                    peak-to-trough amplitude.
                 P_time : `obspy.UTCDateTime` object
-                    Approximate time of amplitude observation (halfway between
-                    peak and trough times).
+                    Approximate time of amplitude observation (halfway between peak and
+                    trough times).
                 P_avg_amp : float
-                    Average amplitude in the P signal window, measured by the
-                    same method as the Noise_amp (see `noise_measure`) and
-                    corrected for the same filter gain as `P_amp`. In
-                    *millimetres*.
+                    Average amplitude in the P signal window, measured by the same
+                    method as the Noise_amp (see `noise_measure`) and corrected for the
+                    same filter gain as `P_amp`. In *millimetres*.
                 P_filter_gain : float
-                    Filter gain at `P_freq`, which has been corrected for in
-                    the P_amp measurements (if a filter was applied prior to
-                    amplitude measurement).
+                    Filter gain at `P_freq`, which has been corrected for in the P_amp
+                    measurements (if a filter was applied prior to amplitude
+                    measurement).
                 S_amp : float
                     As for P, but in the S wave signal window.
                 S_freq : float
                     As for P.
                 S_time : `obspy.UTCDateTime` object
                     As for P.
                 S_avg_amp : float
@@ -739,90 +758,98 @@
                     As for P.
 
         """
 
         # Loop over windows, cut data and measure amplitude
         for k, (start_time, end_time) in enumerate(windows):
             window = tr.slice(start_time, end_time)
-            window.detrend('linear')
+            window.detrend("linear")
             data = window.data
-            phase = ['P', 'S'][k]
+            phase = ["P", "S"][k]
 
             # if trace (window) is empty (no data points) or a flat line, do
             # not make a measurement
             if not bool(window) or data.max() == data.min():
-                logging.warning(f"{phase} signal window doesn't contain any "
-                                f"data for trace {window.id}")
+                logging.warning(
+                    f"{phase} signal window doesn't contain any "
+                    f"data for trace {window.id}"
+                )
                 continue
 
             # Measure maximum half peak-to-trough amplitude
             try:
-                half_amp, approx_freq, p2t_time = \
-                    self._peak_to_trough_amplitude(window)
+                half_amp, approx_freq, p2t_time = self._peak_to_trough_amplitude(window)
             except util.PeakToTroughError as e:
-                logging.warning(f"Amplitude measurement failed in {phase} "
-                                f"signal window for trace {window.id}: {e.msg}")
+                logging.warning(
+                    f"Amplitude measurement failed in {phase} "
+                    f"signal window for trace {window.id}: {e.msg}"
+                )
                 continue
 
             # Measure average amplitude
             average_amp = self._average_amplitude(window, method)
 
             # Correct for filter gain at approximate frequency of
             # measured amplitude
             filter_gain = None
             if self.bandpass_filter or self.highpass_filter:
-                _, filter_gain = sosfreqz(filter_sos, worN=[approx_freq],
-                                          fs=tr.stats.sampling_rate)
+                _, filter_gain = sosfreqz(
+                    filter_sos, worN=[approx_freq], fs=tr.stats.sampling_rate
+                )
                 filter_gain = np.abs(filter_gain[0])
                 if not filter_gain:
-                    logging.info("\t    Warning: Invalid frequency ("
-                                 f"{approx_freq:.5g} Hz) for {phase}_amp "
-                                 f"measurement on:\n\t\t{tr}")
+                    logging.info(
+                        "\t    Warning: Invalid frequency ("
+                        f"{approx_freq:.5g} Hz) for {phase}_amp "
+                        f"measurement on:\n\t\t{tr}"
+                    )
                     continue
                 else:
                     half_amp /= filter_gain
                     average_amp /= filter_gain
 
-            # Put in relevant columns for P / S amplitude, approx_freq,
-            # p2t_time
-            amps[3+k*5:8+k*5] = (half_amp, approx_freq, p2t_time, average_amp,
-                                 filter_gain)
+            # Put in relevant columns for P / S amplitude, approx_freq, p2t_time
+            amps[3 + k * 5 : 8 + k * 5] = (
+                half_amp,
+                approx_freq,
+                p2t_time,
+                average_amp,
+                filter_gain,
+            )
 
         return amps
 
     def _peak_to_trough_amplitude(self, trace):
         """
-        Measure the maximum peak-to-trough amplitude for a given trace;
-        additionally output the approximate frequency of this signal (from
-        the peak-to-trough time) and the time at which it occurs.
+        Measure the maximum peak-to-trough amplitude for a given trace; additionally
+        output the approximate frequency of this signal (from the peak-to-trough time)
+        and the time at which it occurs.
 
-        NOTE: Returns *half* the maximum peak-to-trough amplitude, as this is
-        what the measurement of local magnitude is defined from.
+        NOTE: Returns *half* the maximum peak-to-trough amplitude, as this is what the
+        measurement of local magnitude is defined from.
 
         NOTE: Units are *millimetres*.
 
         Parameters
         ----------
         trace : `obspy.Trace` object
-            Waveform for which to measure max peak-to-trough amplitude
-            (corrected to displacement in units of metres).
+            Waveform for which to measure max peak-to-trough amplitude (corrected to
+            displacement in units of metres).
 
         Returns
         -------
         half_amp : float
-            Half the value of maximum peak-to-trough amplitude, *in
-            millimetres*.
+            Half the value of maximum peak-to-trough amplitude, *in millimetres*.
             Returns -1 if no measurement could be made.
         approx_freq : float
-            Approximate frequency of the arrival, based on the half-period
-            between the maximum peak/trough.
-            Returns -1 if no measurement could be made.
+            Approximate frequency of the arrival, based on the half-period between the
+            maximum peak/trough. Returns -1 if no measurement could be made.
         p2t_time : `obspy.UTCDateTime` object
-            Approximate time of amplitude observation (halfway between peak and
-            trough times.)
+            Approximate time of amplitude observation (halfway between peak and trough
+            times.)
 
         Raises
         ------
         PeakToTroughError
             If the measurement fails, due to no peaks or troughs being found or
             consecutive peaks or troughs being found.
 
@@ -871,70 +898,68 @@
             else:
                 pos = np.argmax(fp2)
                 full_amp = np.max(fp2)
                 peaks, troughs = c, d
 
         peak_time = trace.times()[peaks[pos]]
         trough_time = trace.times()[troughs[pos]]
-        p2t_time = trace.stats.starttime + peak_time + \
-            (trough_time - peak_time) / 2
+        p2t_time = trace.stats.starttime + peak_time + (trough_time - peak_time) / 2
 
         # Peak-to-trough is half a period
-        approx_freq = 1. / (np.abs(peak_time - trough_time) * 2.)
+        approx_freq = 1.0 / (np.abs(peak_time - trough_time) * 2.0)
 
-        # Local magnitude is defined based on maximum zero-to-peak amplitude
-        # in *millimetres*
+        # Local magnitude is defined based on maximum zero-to-peak amplitude in
+        # *millimetres*
         half_amp = full_amp * 1000 / 2
 
         return half_amp, approx_freq, p2t_time
 
     def _measure_noise_amp(self, tr, windows, method="RMS"):
         """
-        Make a measurement of the signal amplitude in a 'noise window' before
-        the P signal window. Several methods for making this measurement are
-        available.
-
-        Performs a linear detrend across the window before measuring
-        amplitudes.
-
-        NOTE: Returns the noise amplitude in millimetres: the chosen
-        formulation of the local magnitude attenuation function may have to be
-        adjusted to match these units.
+        Make a measurement of the signal amplitude in a 'noise window' before the P
+        signal window. Several methods for making this measurement are available.
+
+        Performs a linear detrend across the window before measuring amplitudes.
+
+        NOTE: Returns the noise amplitude in millimetres: the chosen formulation of the
+        local magnitude attenuation function may have to be adjusted to match these
+        units.
 
         Parameters
         ----------
         tr : `obspy.Trace` object
-            Trace from which to measure the noise amplitude (corrected to
-            displacement in units of metres).
+            Trace from which to measure the noise amplitude (corrected to displacement
+            in units of metres).
         windows : array-like
             [[P_window_start, P_window_end], [S_window_start, S_window_end]]
         method : {"RMS", "STD", "ENV"}, optional
-            The method by which to measure the amplitude of the signal in the
-            noise window: root-mean-square, standard deviation or average
-            amplitude of the envelope of the signal. (Default "RMS")
+            The method by which to measure the amplitude of the signal in the noise
+            window: root-mean-square, standard deviation or average amplitude of the
+            envelope of the signal. (Default "RMS")
 
         Returns
         -------
         noise_amp : float
-            An estimate of the signal amplitude in the noise window. In
-            millimetres. Not corrected for filter gain.
+            An estimate of the signal amplitude in the noise window. In millimetres. Not
+            corrected for filter gain.
 
         """
 
         p_start = windows[0][0]
 
-        # Make a noise measurement in a window of length noise_window,
-        # ending at the start of the p_window
+        # Make a noise measurement in a window of length noise_window, ending at the
+        # start of the p_window
         noise_start = p_start - self.noise_window
         noise_end = p_start
 
         noise = tr.slice(noise_start, noise_end)
         if not bool(noise) or noise.data.max() == noise.data.min():
-            logging.warning("Noise window doesn't contain any data for trace "
-                            f"{noise.id}")
+            logging.warning(
+                f"Noise window doesn't contain any data for trace {noise.id}"
+            )
             noise_amp = np.nan
         else:
             noise.detrend("linear")
             noise_amp = self._average_amplitude(noise, method)
 
         return noise_amp
 
@@ -943,20 +968,20 @@
         Measure the average amplitude of a trace.
 
         NOTE: returns amplitude in *millimetres*.
 
         Parameters
         ----------
         trace : `obspy.Trace` object
-            Trace from which to measure the amplitude (corrected to
-            displacement in units of metres).
+            Trace from which to measure the amplitude (corrected to displacement in
+            units of metres).
         method : {"RMS", "STD", "ENV"}
             The method by which to measure the average amplitude of the signal:
-            root-mean-square, standard deviation or average amplitude of the
-            envelope of the signal. (Default "RMS").
+            root-mean-square, standard deviation or average amplitude of the envelope of
+            the signal. (Default "RMS").
 
         Returns
         -------
         amp : float
             Average amplitude of the trace (in millimetres).
 
         Raises
@@ -969,58 +994,58 @@
         if method == "RMS":
             amp = np.sqrt(np.mean(np.square(trace.data)))
         elif method == "STD":
             amp = np.std(trace.data)
         elif method == "ENV":
             amp = np.mean(np.abs(hilbert(trace.data)))
         else:
-            raise NotImplementedError("Only 'RMS', 'STD' and 'ENV' are "
-                                      "available currently. Please contact the"
-                                      " QuakeMigrate developers.")
+            raise NotImplementedError(
+                "Only 'RMS', 'STD' and 'ENV' are available currently. Please contact "
+                "the QuakeMigrate developers."
+            )
 
         # Convert to *millimetres*
-        amp *= 1000.
+        amp *= 1000.0
 
         return amp
 
     def pad(self, marginal_window, max_tt, fraction_tt):
         """
-        Calculate padding, including an allowance for the taper applied when
-        filtering / removing instrument response, to ensure the noise and
-        signal window amplitude measurements are not affected by the taper.
+        Calculate padding, including an allowance for the taper applied when filtering/
+        removing instrument response, to ensure the noise and signal window amplitude
+        measurements are not affected by the taper.
 
         Parameters
         ----------
         marginal_window : float
-            Half-width of window centred on the maximum coalescence time of the
-            event over which the 4-D coalescence function is marginalised. Used
-            here as an estimate of the origin time uncertainity when
-            calculating the signal windows.
+            Half-width of window centred on the maximum coalescence time of the event
+            over which the 4-D coalescence function is marginalised. Used here as an
+            estimate of the origin time uncertainity when calculating the signal
+            windows.
         max_tt : float
             Maximum traveltime in the look-up table.
         fraction_tt : float
-            An estimate of the uncertainty in the velocity model as a function
-            of a fraction of the traveltime. (Default 0.1 == 10%)
+            An estimate of the uncertainty in the velocity model as a function of a
+            fraction of the traveltime. (Default 0.1 == 10%)
 
         Returns
         -------
         pre_pad : float
-            Time window by which to pre-pad the data when reading from the
-            waveform archive.
+            Time window by which to pre-pad the data when reading from the waveform
+            archive.
         post_pad : float
-            Time window by which to post-pad the data when reading from the
-            waveform archive.
+            Time window by which to post-pad the data when reading from the waveform
+            archive.
 
         """
 
         pre_pad = self.noise_window + marginal_window
         logging.debug(f"Raw pre-pad: {pre_pad}")
-        post_pad = self.signal_window + max_tt * (1 + fraction_tt) \
-            + marginal_window
+        post_pad = self.signal_window + max_tt * (1 + fraction_tt) + marginal_window
         logging.debug(f"Raw post-pad: {post_pad}")
 
         timespan = pre_pad + post_pad
-        pre_pad += np.ceil(timespan*0.06)
-        post_pad += np.ceil(timespan*0.06)
+        pre_pad += np.ceil(timespan * 0.06)
+        post_pad += np.ceil(timespan * 0.06)
         logging.debug(f"Final pre-pad: {pre_pad}, final post-pad: {post_pad}")
 
         return pre_pad, post_pad
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quakemigrate-1.0.1/quakemigrate/signal/local_mag/local_mag.py` & `quakemigrate-1.0.2/quakemigrate/signal/local_mag/local_mag.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """
-Module containing methods to calculate the local magnitude for an event located
-by :mod:`QuakeMigrate`.
+Module containing methods to calculate the local magnitude for an event located by
+:mod:`QuakeMigrate`.
 
 :copyright:
-    2020 - 2021, QuakeMigrate developers.
+    2020–2023, QuakeMigrate developers.
 :license:
     GNU General Public License, Version 3
     (https://www.gnu.org/licenses/gpl-3.0.html)
 
 """
 
 import logging
@@ -20,48 +20,45 @@
 from .magnitude import Magnitude
 
 
 class LocalMag:
     """
     QuakeMigrate extension class for calculating local magnitudes.
 
-    Provides functions for measuring amplitudes of earthquake waveforms and
-    using these to calculate local magnitudes.
+    Provides functions for measuring amplitudes of earthquake waveforms and using these
+    to calculate local magnitudes.
 
     Parameters
     ----------
     amp_params : dict
         All keys are optional, including:
         signal_window : float
-            Length of S-wave signal window, in addition to the time window
-            associated with the marginal_window and traveltime uncertainty.
-            (Default 0 s)
+            Length of S-wave signal window, in addition to the time window associated
+            with the marginal_window and traveltime uncertainty. (Default 0 s)
         noise_window : float
-            Length of the time window before the P-wave signal window in which
-            to measure the noise amplitude. (Default 10 s)
+            Length of the time window before the P-wave signal window in which to
+            measure the noise amplitude. (Default 10 s)
         noise_measure : {"RMS", "STD", "ENV"}
-            Method by which to measure the noise amplitude; root-mean-quare,
-            standard deviation or average amplitude of the envelope of the
-            signal. (Default "RMS")
+            Method by which to measure the noise amplitude; root-mean-quare, standard
+            deviation or average amplitude of the envelope of the signal.
+            (Default "RMS")
         loc_method : {"spline", "gaussian", "covariance"}
             Which event location estimate to use. (Default "spline")
         highpass_filter : bool
-            Whether to apply a highpass filter to the data before measuring
-            amplitudes. (Default False)
+            Whether to apply a highpass filter to the data before measuring amplitudes.
+            (Default False)
         highpass_freq : float
             High-pass filter frequency. Required if highpass_filter is True.
         bandpass_filter : bool
             Whether to apply a band-pass filter before measuring amplitudes.
             (Default: False)
         bandpass_lowcut : float
-            Band-pass filter low-cut frequency. Required if bandpass_filter is
-            True.
+            Band-pass filter low-cut frequency. Required if bandpass_filter is True.
         bandpass_highcut : float
-            Band-pass filter high-cut frequency. Required if bandpass_filter is
-            True.
+            Band-pass filter high-cut frequency. Required if bandpass_filter is True.
         filter_corners : int
             Number of corners for the chosen filter. Default: 4.
         prominence_multiplier : float
             To set a prominence filter in the peak-finding algorithm.
             (Default 0. = off).
             NOTE: not recommended for use in combination with a filter; filter
             gain corrections can lead to spurious results. Please see the
@@ -73,55 +70,53 @@
             {"Hutton-Boore", "keir2006", "UK", ...}. Alternatively specify a
             function which returns the attenuation factor at a specified
             (epicentral or hypocentral) distance. (Default "Hutton-Boore")
         All other keys are optional, including:
         station_corrections : dict {str : float}
             Dictionary of trace_id : magnitude-correction pairs. (Default None)
         amp_feature : {"S_amp", "P_amp"}
-            Which phase amplitude measurement to use to calculate local
-            magnitude. (Default "S_amp")
+            Which phase amplitude measurement to use to calculate local magnitude.
+            (Default "S_amp")
         amp_multiplier : float
             Factor by which to multiply all measured amplitudes.
         use_hyp_dist : bool, optional
-            Whether to use the hypocentral distance instead of the epicentral
-            distance in the local magnitude calculation. (Default False)
+            Whether to use the hypocentral distance instead of the epicentral distance
+            in the local magnitude calculation. (Default False)
         trace_filter : regex expression
             Expression by which to select traces to use for the mean_magnitude
             calculation. E.g. '.*H[NE]$'. (Default None)
         station_filter : list of str
             List of stations to exclude from the mean_magnitude calculation.
             E.g. ["KVE", "LIND"]. (Default None)
         dist_filter : float or False
             Whether to only use stations less than a specified (epicentral or
-            hypocentral) distance from an event in the mean_magnitude()
-            calculation. Distance in kilometres. (Default False)
+            hypocentral) distance from an event in the mean_magnitude() calculation.
+            Distance in kilometres. (Default False)
         pick_filter : bool
-            Whether to only use stations where at least one phase was picked by
-            the autopicker in the mean_magnitude calculation. (Default False)
+            Whether to only use stations where at least one phase was picked by the
+            autopicker in the mean_magnitude calculation. (Default False)
         noise_filter : float
-            Factor by which to multiply the measured noise amplitude before
-            excluding amplitude observations below the noise level.
+            Factor by which to multiply the measured noise amplitude before excluding
+            amplitude observations below the noise level.
             (Default 1.)
         weighted_mean : bool
-            Whether to do a weighted mean of the magnitudes when calculating
-            the mean_magnitude. (Default False)
+            Whether to do a weighted mean of the magnitudes when calculating the
+            mean_magnitude. (Default False)
     plot_amplitudes : bool, optional
         Plot amplitudes vs. distance plot for each event. (Default True)
 
     Attributes
     ----------
     amp : :class:`~quakemigrate.signal.local_mag.amplitude.Amplitude` object
         The Amplitude object for this instance of LocalMag. Contains functions
-        to measure Wood-Anderson corrected displacement amplitudes for an
-        event.
+        to measure Wood-Anderson corrected displacement amplitudes for an event.
     mag : :class:`~quakemigrate.signal.local_mag.magnitude.Magnitude` object
-        The Magnitude object for this instance of LocalMag. Contains functions
-        to calculate magnitudes from Wood-Anderson corrected displacement
-        amplitudes, and to combine them into a single magnitude estimate for
-        the event.
+        The Magnitude object for this instance of LocalMag. Contains functions to
+        calculate magnitudes from Wood-Anderson corrected displacement amplitudes, and
+        to combine them into a single magnitude estimate for the event.
 
     Methods
     -------
     calc_magnitude(event, lut, run)
 
     """
 
@@ -130,64 +125,67 @@
 
         self.amp = Amplitude(amp_params)
         self.mag = Magnitude(mag_params)
         self.plot = plot_amplitudes
 
     def __str__(self):
         """Return short summary string of the LocalMagnitudes object."""
-        out = ("\tCalculating local magnitudes from Wood-Anderson corrected "
-               "amplitude observations\n")
+        out = (
+            "\tCalculating local magnitudes from Wood-Anderson corrected "
+            "amplitude observations\n"
+        )
         out += str(self.amp)
         out += str(self.mag)
 
         return out
 
     @util.timeit("info")
     def calc_magnitude(self, event, lut, run):
         """
-        Wrapper function to calculate the local magnitude of an event by first
-        making Wood-Anderson corrected displacement amplitude measurements on
-        each trace, then calculating magnitudes from these individual
-        measurements, and a network-averaged (weighted) mean magnitude
-        estimate and associated uncertainty.
-
-        Additional functionality includes calculating an r^2 fit of the
-        predicted amplitude with distance curve to the observed amplitudes,
-        and an associated plot of amplitudes vs. distance.
+        Wrapper function to calculate the local magnitude of an event by first making
+        Wood-Anderson corrected displacement amplitude measurements on each trace, then
+        calculating magnitudes from these individual measurements, and a
+        network-averaged (weighted) mean magnitude estimate and associated uncertainty.
+
+        Additional functionality includes calculating an r^2 fit of the predicted
+        amplitude with distance curve to the observed amplitudes, and an associated plot
+        of amplitudes vs. distance.
 
         Parameters
         ----------
         event : :class:`~quakemigrate.io.event.Event` object
             Light class encapsulating waveform data, onset, pick and location
             information for a given event.
         lut : :class:`~quakemigrate.lut.lut.LUT` object
-            Contains the traveltime lookup tables for seismic phases, computed
-            for some pre-defined velocity model.
+            Contains the traveltime lookup tables for seismic phases, computed for some
+            pre-defined velocity model.
         run : :class:`~quakemigrate.io.core.Run` object
-            Light class encapsulating waveforms, coalescence information, picks
-            and location information for a given event.
+            Light class encapsulating waveforms, coalescence information, picks and
+            location information for a given event.
 
         Returns
         -------
         event : :class:`~quakemigrate.io.event.Event` object
-            Light class encapsulating waveforms, coalescence information, picks
-            and location information for a given event. Now also contains local
-            magnitude information.
+            Light class encapsulating waveforms, coalescence information, picks and
+            location information for a given event. Now also contains local magnitude
+            information.
         mag : float
             Network-averaged local magnitude estimate for this event.
 
         """
 
         # Measure amplitudes on all available traces
         amps = self.amp.get_amplitudes(event, lut)
 
         # Check if any amplitude measurements were made
         if amps[self.mag.amp_feature].isnull().all():
-            logging.warning("\t\tNo amplitude measurements were made! Skipping"
-                            " magnitude calculation")
+            logging.warning(
+                "\t\tNo amplitude measurements were made! Skipping"
+                " magnitude calculation"
+            )
             write_amplitudes(run, amps, event)
             event.add_local_magnitude(np.nan, np.nan, np.nan, amps)
 
             return event, np.nan
 
         # Calculate magnitudes for individual amplitude measurements
         mags = self.mag.calculate_magnitudes(amps)
@@ -199,12 +197,12 @@
         # magnitude for the event. Optionally output a plot of amplitudes vs
         # distance.
         mag, mag_err, mag_r2, mags = self.mag.mean_magnitude(mags)
 
         event.add_local_magnitude(mag, mag_err, mag_r2)
 
         if self.plot and mag is not np.nan:
-            self.mag.plot_amplitudes(mags, event, run,
-                                     lut.unit_conversion_factor,
-                                     self.amp.noise_measure)
+            self.mag.plot_amplitudes(
+                mags, event, run, lut.unit_conversion_factor, self.amp.noise_measure
+            )
 
         return event, mag
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quakemigrate-1.0.1/quakemigrate/signal/local_mag/magnitude.py` & `quakemigrate-1.0.2/quakemigrate/signal/local_mag/magnitude.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 """
-Module that supplies functions to calculate magnitudes from observations of
-trace amplitudes, earthquake location, station locations, and an estimated
-attenuation curve for the region of interest.
+Module that supplies functions to calculate magnitudes from observations of trace
+amplitudes, earthquake location, station locations, and an estimated attenuation curve
+for the region of interest.
 
 :copyright:
-    2020 - 2021, QuakeMigrate developers.
+    2020–2023, QuakeMigrate developers.
 :license:
     GNU General Public License, Version 3
     (https://www.gnu.org/licenses/gpl-3.0.html)
 
 """
 
 import logging
@@ -21,73 +21,72 @@
 
 
 class Magnitude:
     """
     Part of the QuakeMigrate LocalMag class; calculates local magnitudes from
     Wood-Anderson corrected waveform amplitude measurements.
 
-    Takes waveform amplitude measurements from the LocalMag Amplitude class,
-    and from these calculates local magnitude estimates using a local magnitude
-    attenuation function. Magnitude corrections for individual stations and
-    channels thereof can be applied, if provided.
-
-    Individual estimates are then combined to calculate a network-averaged
-    (weighted) mean local magnitude for the event. Also includes the function
-    to measure the r-squared statistic assessing the goodness of fit between
-    the predicted amplitude with distance from the nework-averaged local
-    magnitude for the event and chosen attenuation function, and the observed
-    amplitudes. This, provides a tool to distinguish between real microseismic
-    events and artefacts.
-
-    A summary plot illustrating the amplitude observations, their
-    uncertainties, and the predicted amplitude with distance for the network-
-    averaged local magnitude (and its uncertainties) can optionally be output.
+    Takes waveform amplitude measurements from the LocalMag Amplitude class, and from
+    these calculates local magnitude estimates using a local magnitude attenuation
+    function. Magnitude corrections for individual stations and channels thereof can be
+    applied, if provided.
+
+    Individual estimates are then combined to calculate a network-averaged (weighted)
+    mean local magnitude for the event. Also includes the function to measure the
+    r-squared statistic assessing the goodness of fit between the predicted amplitude
+    with distance from the nework-averaged local magnitude for the event and chosen
+    attenuation function, and the observed amplitudes. This, provides a tool to
+    distinguish between real microseismic events and artefacts.
+
+    A summary plot illustrating the amplitude observations, their uncertainties, and the
+    predicted amplitude with distance for the network-averaged local magnitude (and its
+    uncertainties) can optionally be output.
 
     Attributes
     ----------
     A0 : str or func
         Name of the attenuation function to use. Available options include
-        {"Hutton-Boore", "keir2006", "UK", ...}. Alternatively specify a
-        function which returns the attenuation factor at a specified
-        (epicentral or hypocentral) distance. (Default "Hutton-Boore")
+        {"Hutton-Boore", "keir2006", "UK", ...}. Alternatively specify a function which
+        returns the attenuation factor at a specified (epicentral or hypocentral)
+        distance. (Default "Hutton-Boore")
     use_hyp_dist : bool, optional
-        Whether to use the hypocentral distance instead of the epicentral
-        distance in the local magnitude calculation. (Default False)
+        Whether to use the hypocentral distance instead of the epicentral distance in
+        the local magnitude calculation. (Default False)
     amp_feature : {"S_amp", "P_amp"}
-        Which phase amplitude measurement to use to calculate local
-        magnitude. (Default "S_amp")
+        Which phase amplitude measurement to use to calculate local magnitude.
+        (Default "S_amp")
     station_corrections : dict {str : float}
         Dictionary of trace_id : magnitude-correction pairs. (Default None)
     amp_multiplier : float
         Factor by which to multiply all measured amplitudes.
     weighted_mean : bool
-        Whether to use a weighted mean to calculate the network-averaged
-        local magnitude estimate for the event. (Default False)
+        Whether to use a weighted mean to calculate the network-averaged local magnitude
+        estimate for the event. (Default False)
     trace_filter : regex expression
-        Expression by which to select traces to use for the mean_magnitude
-        calculation. E.g. ".*H[NE]$" . (Default None)
+        Expression by which to select traces to use for the mean_magnitude calculation.
+        E.g. ".*H[NE]$" . (Default None)
     noise_filter : float
-        Factor by which to multiply the measured noise amplitude before
-        excluding amplitude observations below the noise level.
+        Factor by which to multiply the measured noise amplitude before excluding
+        amplitude observations below the noise level.
         (Default 1.)
     station_filter : list of str
         List of stations to exclude from the mean_magnitude calculation.
         E.g. ["KVE", "LIND"]. (Default None)
     dist_filter : float or False
-        Whether to only use stations less than a specified (epicentral or
-        hypocentral) distance from an event in the mean_magnitude()
-        calculation. Distance in kilometres. (Default False)
+        Whether to only use stations less than a specified (epicentral or hypocentral)
+        distance from an event in the mean_magnitude() calculation. Distance in
+        kilometres. (Default False)
     pick_filter : bool
-        Whether to only use stations where at least one phase was picked by
-        the autopicker in the mean_magnitude calculation. (Default False)
+        Whether to only use stations where at least one phase was picked by the
+        autopicker in the mean_magnitude calculation. (Default False)
     r2_only_used : bool
         Whether to only use amplitude observations which were used for the mean
-        magnitude calculation when calculating the r-squared statistic for the
-        goodness of fit between the measured and predicted amplitudes. Default:
-        True; False is an experimental feature - use with caution.
+        magnitude calculation when calculating the r-squared statistic for the goodness
+        of fit between the measured and predicted amplitudes. Default: True; False is an
+        experimental feature - use with caution.
 
     Methods
     -------
     calculate_magnitudes(amplitudes)
     mean_magnitude(magnitudes)
     plot_amplitudes(event, run)
 
@@ -100,129 +99,127 @@
 
     """
 
     def __init__(self, magnitude_params={}):
         """Instantiate the Magnitude object."""
 
         # Parameters for individual magnitude calculation
-        self.A0 = magnitude_params.get('A0')
+        self.A0 = magnitude_params.get("A0")
         if not self.A0:
-            msg = "A0 attenuation correction not specified in params!"
-            raise TypeError(msg)
+            raise TypeError("A0 attenuation correction not specified in params!")
         self.use_hyp_dist = magnitude_params.get("use_hyp_dist", False)
         self.amp_feature = magnitude_params.get("amp_feature", "S_amp")
-        self.station_corrections = magnitude_params.get("station_corrections",
-                                                        {})
-        self.amp_multiplier = magnitude_params.get("amp_multiplier", 1.)
+        self.station_corrections = magnitude_params.get("station_corrections", {})
+        self.amp_multiplier = magnitude_params.get("amp_multiplier", 1.0)
 
         # Parameters for mean magnitude calculation
         self.weighted_mean = magnitude_params.get("weighted_mean", False)
         self.trace_filter = magnitude_params.get("trace_filter")
-        self.noise_filter = magnitude_params.get("noise_filter", 1.)
+        self.noise_filter = magnitude_params.get("noise_filter", 1.0)
         self.station_filter = magnitude_params.get("station_filter")
         self.dist_filter = magnitude_params.get("dist_filter", False)
         self.pick_filter = magnitude_params.get("pick_filter", False)
         self.r2_only_used = magnitude_params.get("r2_only_used", True)
 
     def __str__(self):
         """Return short summary string of the Magnitude object."""
 
-        out = ("\t    Magnitude parameters:\n"
-               f"\t\tA0 attenuation function = {self.A0}\n"
-               f"\t\tUse hyp distance        = {self.use_hyp_dist}\n"
-               f"\t\tAmplitude feature       = {self.amp_feature}\n")
+        out = (
+            "\t    Magnitude parameters:\n"
+            f"\t\tA0 attenuation function = {self.A0}\n"
+            f"\t\tUse hyp distance        = {self.use_hyp_dist}\n"
+            f"\t\tAmplitude feature       = {self.amp_feature}\n"
+        )
         if self.station_corrections:
             out += "\t\tUsing user-provided station corrections\n"
-        out += (f"\t\tAmplitude multiplier    = {self.amp_multiplier}\n"
-                f"\t\tUse weighted mean       = {self.weighted_mean}\n")
+        out += (
+            f"\t\tAmplitude multiplier    = {self.amp_multiplier}\n"
+            f"\t\tUse weighted mean       = {self.weighted_mean}\n"
+        )
         if self.trace_filter is not None:
             out += f"\t\tTrace filter            = {self.trace_filter}\n"
         out += f"\t\tNoise filter            = {self.noise_filter} x\n"
         if self.station_filter is not None:
             out += f"\t\tStation filter          = {self.station_filter}\n"
         if self.dist_filter:
             out += f"\t\tDistance filter         = {self.dist_filter} km\n"
         if self.pick_filter:
             out += "\t\tUsing only Amplitudes from picked traces.\n"
 
         return out
 
     def calculate_magnitudes(self, amplitudes):
         """
-        Calculate magnitude estimates from amplitude measurements on
-        individual stations / components.
+        Calculate magnitude estimates from amplitude measurements on individual stations
+        /components.
 
         Parameters
         ----------
         amplitudes : `pandas.DataFrame` object
-            P- and S-wave amplitude measurements for each component of each
-            station in the look-up table.
+            P- and S-wave amplitude measurements for each component of each station in
+            the look-up table.
             Columns:
                 epi_dist : float
-                    Epicentral distance between the station and the event
-                    hypocentre.
+                    Epicentral distance between the station and the event hypocentre.
                 z_dist : float
-                    Vertical distance between the station and the event
-                    hypocentre.
+                    Vertical distance between the station and the event hypocentre.
                 P_amp : float
-                    Half maximum peak-to-trough amplitude in the P signal
-                    window. In *millimetres*. Corrected for filter gain, if
-                    applicable.
+                    Half maximum peak-to-trough amplitude in the P signal window. In
+                    *millimetres*. Corrected for filter gain, if applicable.
                 P_freq : float
-                    Approximate frequency of the maximum amplitude P-wave
-                    signal. Calculated from the peak-to-trough time interval of
-                    the max peak-to-trough amplitude.
+                    Approximate frequency of the maximum amplitude P-wave signal.
+                    Calculated from the peak-to-trough time interval of the max
+                    peak-to-trough amplitude.
                 P_time : `obspy.UTCDateTime` object
-                    Approximate time of amplitude observation (halfway between
-                    peak and trough times).
+                    Approximate time of amplitude observation (halfway between peak and
+                    trough times).
                 P_avg_amp : float
-                    Average amplitude in the P signal window, measured by the
-                    same method as the Noise_amp (see `noise_measure`) and
-                    corrected for the same filter gain as `P_amp`. In
-                    *millimetres*.
+                    Average amplitude in the P signal window, measured by the same
+                    method as the Noise_amp (see `noise_measure`) and corrected for the
+                    same filter gain as `P_amp`. In *millimetres*.
                 P_filter_gain : float or NaN
-                    Filter gain at `P_freq` - which has been corrected for in
-                    the P_amp measurements - if a filter was applied prior to
-                    amplitude measurement; Else NaN.
+                    Filter gain at `P_freq` - which has been corrected for in the P_amp
+                    measurements - if a filter was applied prior to amplitude
+                    measurement; Else NaN.
                 S_amp : float
                     As for P, but in the S wave signal window.
                 S_freq : float
                     As for P.
                 S_time : `obspy.UTCDateTime` object
                     As for P.
                 S_avg_amp : float
                     As for P.
                 S_filter_gain : float or NaN.
                     As for P.
                 Noise_amp : float
-                    The average signal amplitude in the noise window. In
-                    *millimetres*. See `noise_measure` parameter.
+                    The average signal amplitude in the noise window. In *millimetres*.
+                    See `noise_measure` parameter.
                 is_picked : bool
-                    Whether at least one of the phase arrivals was picked by
-                    the autopicker.
+                    Whether at least one of the phase arrivals was picked by the
+                    autopicker.
             Index = Trace ID (see `obspy.Trace` object property 'id')
 
         Returns
         -------
         magnitudes : `pandas.DataFrame` object
-            The original amplitudes DataFrame, with columns containing the
-            calculated magnitude and an associated error now added.
+            The original amplitudes DataFrame, with columns containing the calculated
+            magnitude and an associated error now added.
             Columns = ["epi_dist", "z_dist", "P_amp", "P_freq", "P_time",
                    "P_avg_amp", "P_filter_gain", "S_amp", "S_freq", "S_time",
                    "S_avg_amp", "S_filter_gain", "Noise_amp", "is_picked",
                    "ML", "ML_Err"]
             Index = Trace ID (see `obspy.Trace.id`)
             Additional fields:
             ML : float
-                Magnitude calculated from the chosen amplitude measurement,
-                using the specified attenuation curve and station_corrections.
+                Magnitude calculated from the chosen amplitude measurement, using the
+                specified attenuation curve and station_corrections.
             ML_Err : float
-                estimate of the error on the calculated magnitude, based on
-                potential errors in the maximum amplitude measurement according
-                to the measured noise amplitude.
+                Estimate of the error on the calculated magnitude, based on potential
+                errors in the maximum amplitude measurement according to the measured
+                noise amplitude.
 
         Raises
         ------
         AttributeError
             If A0 attenuation correction is not specified.
 
         """
@@ -230,207 +227,205 @@
         trace_ids = amplitudes.index
         amps = amplitudes[self.amp_feature].values * self.amp_multiplier
         noise_amps = amplitudes["Noise_amp"].values * self.amp_multiplier
         filter_gains = amplitudes[f"{self.amp_feature[0]}_filter_gain"]
         if not filter_gains.isnull().values.any():
             noise_amps /= filter_gains
 
-        # Remove those amplitudes where the noise is greater than the amplitude
-        # and set amplitudes which = 0. to NaN (to avoid logs blowing up).
+        # Remove those amplitudes where the noise is greater than the amplitude and set
+        # amplitudes which = 0. to NaN (to avoid logs blowing up).
         with np.errstate(invalid="ignore"):
             amps[amps < noise_amps] = np.nan
-            amps[amps == 0.] = np.nan
+            amps[amps == 0.0] = np.nan
 
         # Calculate distances (hypocentral or epicentral)
         edist, zdist = amplitudes["epi_dist"], amplitudes["z_dist"]
         if self.use_hyp_dist:
             dist = np.sqrt(edist.values**2 + zdist.values**2)
         else:
             dist = edist.values
-        dist[dist == 0.] = np.nan
+        dist[dist == 0.0] = np.nan
 
         # Calculate magnitudes and associated errors
         mags, mag_errs = self._calc_mags(trace_ids, amps, noise_amps, dist)
 
         magnitudes = amplitudes.copy()
         magnitudes["ML"] = mags
         magnitudes["ML_Err"] = mag_errs
 
         return magnitudes
 
     def mean_magnitude(self, magnitudes):
         """
-        Calculate the network-averaged local magnitude for an event based on
-        the magnitude estimates calculated from amplitude measurements made on
-        each component of each station.
-
-        The user may specify distance, station, channel and a number of other
-        filters to restrict which observations are included in this best
-        estimate of the local magnitude of the event.
+        Calculate the network-averaged local magnitude for an event based on the
+        magnitude estimates calculated from amplitude measurements made on each
+        component of each station.
+
+        The user may specify distance, station, channel and a number of other filters to
+        restrict which observations are included in this best estimate of the local
+        magnitude of the event.
 
         Parameters
         ----------
         magnitudes : `pandas.DataFrame` object
-            Contains P- and S-wave amplitude measurements for each component of
-            each station in the look-up table, and local magnitude estimates
-            calculated from them (output by calculate_magnitudes()). Note that
-            the amplitude observations are raw, but the ML estimates derived
-            from them include station corrections, if provided.
+            Contains P- and S-wave amplitude measurements for each component of each
+            station in the look-up table, and local magnitude estimates calculated from
+            them (output by calculate_magnitudes()). Note that the amplitude
+            observations are raw, but the ML estimates derived from them include station
+            corrections, if provided.
             Columns:
                 epi_dist : float
-                    Epicentral distance between the station and the event
-                    hypocentre.
+                    Epicentral distance between the station and the event hypocentre.
                 z_dist : float
-                    Vertical distance between the station and the event
-                    hypocentre.
+                    Vertical distance between the station and the event hypocentre.
                 P_amp : float
-                    Half maximum peak-to-trough amplitude in the P signal
-                    window. In *millimetres*. Corrected for filter gain, if
-                    applicable.
+                    Half maximum peak-to-trough amplitude in the P signal window. In
+                    *millimetres*. Corrected for filter gain, if applicable.
                 P_freq : float
-                    Approximate frequency of the maximum amplitude P-wave
-                    signal. Calculated from the peak-to-trough time interval of
-                    the max peak-to-trough amplitude.
+                    Approximate frequency of the maximum amplitude P-wave signal.
+                    Calculated from the peak-to-trough time interval of the max
+                    peak-to-trough amplitude.
                 P_time : `obspy.UTCDateTime` object
-                    Approximate time of amplitude observation (halfway between
-                    peak and trough times).
+                    Approximate time of amplitude observation (halfway between peak and
+                    trough times).
                 P_avg_amp : float
-                    Average amplitude in the P signal window, measured by the
-                    same method as the Noise_amp (see `noise_measure`) and
-                    corrected for the same filter gain as `P_amp`. In
-                    *millimetres*.
+                    Average amplitude in the P signal window, measured by the same
+                    method as the Noise_amp (see `noise_measure`) and corrected for the
+                    same filter gain as `P_amp`. In *millimetres*.
                 P_filter_gain : float or NaN
-                    Filter gain at `P_freq` - which has been corrected for in
-                    the P_amp measurements - if a filter was applied prior to
-                    amplitude measurement; Else NaN.
+                    Filter gain at `P_freq` - which has been corrected for in the P_amp
+                    measurements - if a filter was applied prior to amplitude
+                    measurement; Else NaN.
                 S_amp : float
                     As for P, but in the S wave signal window.
                 S_freq : float
                     As for P.
                 S_time : `obspy.UTCDateTime` object
                     As for P.
                 S_avg_amp : float
                     As for P.
                 S_filter_gain : float or NaN.
                     As for P.
                 Noise_amp : float
-                    The average signal amplitude in the noise window. In
-                    *millimetres*. See `noise_measure` parameter.
+                    The average signal amplitude in the noise window. In *millimetres*.
+                    See `noise_measure` parameter.
                 is_picked : bool
-                    Whether at least one of the phase arrivals was picked by
-                    the autopicker.
+                    Whether at least one of the phase arrivals was picked by the
+                    autopicker.
                 ML : float
-                    Magnitude calculated from the chosen amplitude measurement,
-                    using the specified attenuation curve and
-                    station_corrections.
+                    Magnitude calculated from the chosen amplitude measurement, using
+                    the specified attenuation curve and station_corrections.
                 ML_Err : float
-                    estimate of the error on the calculated magnitude, based on
-                    potential errors in the maximum amplitude measurement
-                    according to the measured noise amplitude.
+                    Estimate of the error on the calculated magnitude, based on
+                    potential errors in the maximum amplitude measurement according to
+                    the measured noise amplitude.
             Index = Trace ID (see `obspy.Trace` object property 'id')
 
         Returns
         -------
         mean_mag : float or NaN
-            Network-averaged local magnitude estimate for the event. Mean (or
-            weighted mean) of the magnitude estimates calculated from each
-            individual channel after optionally removing some observations
-            based on trace ID, distance, etcetera.
+            Network-averaged local magnitude estimate for the event. Mean (or weighted
+            mean) of the magnitude estimates calculated from each individual channel
+            after optionally removing some observations based on trace ID, distance,
+            etcetera.
         mean_mag_err : float or NaN
-            Standard deviation (or weighted standard deviation) of the
-            magnitude estimates calculated from individual channels which
-            contributed to the calculation of the (weighted) mean magnitude.
+            Standard deviation (or weighted standard deviation) of the magnitude
+            estimates calculated from individual channels which contributed to the
+            calculation of the (weighted) mean magnitude.
         mag_r_squared : float or NaN
-            r-squared statistic describing the fit of the amplitude vs.
-            distance curve predicted by the calculated mean_mag and chosen
-            attenuation model to the measured amplitude observations. This is
-            intended to be used to help discriminate between 'real' events, for
-            which the predicted amplitude vs. distance curve should provide a
-            good fit to the observations, from artefacts, which in general will
-            not.
+            r-squared statistic describing the fit of the amplitude vs. distance curve
+            predicted by the calculated mean_mag and chosen attenuation model to the
+            measured amplitude observations. This is intended to be used to help
+            discriminate between 'real' events, for which the predicted amplitude vs.
+            distance curve should provide a good fit to the observations, from
+            artefacts, which in general will not.
 
         """
 
         # Get station corrections
-        corrs = [self.station_corrections[t] if t in
-                 self.station_corrections.keys() else 0. for t in
-                 magnitudes.index]
+        corrs = [
+            self.station_corrections[t] if t in self.station_corrections.keys() else 0.0
+            for t in magnitudes.index
+        ]
         magnitudes["Station_Correction"] = corrs
 
         # Correct noise amps for filter gain, if applicable
         filter_gains = magnitudes[f"{self.amp_feature[0]}_filter_gain"]
         if not filter_gains.isnull().values.any():
             magnitudes.loc[:, "Noise_amp"] /= filter_gains
 
         # Do filtering
         used_mags, all_mags = self._filter_mags(magnitudes)
 
         # Check if there are still some magnitude observations left
         if len(used_mags) == 0:
-            logging.warning("\t    No magnitude observations match the "
-                            "filtering criteria! Skipping.")
+            logging.warning(
+                "\t    No magnitude observations match the "
+                "filtering criteria! Skipping."
+            )
             return np.nan, np.nan, np.nan, all_mags
 
         mags = used_mags["ML"].values
 
         # If weighted, calculate weight as (1/error)^2. Else equal weighting.
         if self.weighted_mean:
             weights = (1 / used_mags["ML_Err"]) ** 2
         else:
             weights = np.ones_like(mags)
 
-        # Calculate mean and standard deviation. NOTE: makes the assumption
-        # that the distribution of these magnitude observations can locally be
-        # approximated by a normal distribution. In reality it will have a
-        # negative skew, making the mean magnitude a slight underestimate.
-        mean_mag = np.sum(mags*weights) / np.sum(weights)
-        mean_mag_err = np.sqrt(np.sum(((mags - mean_mag)*weights)**2)
-                               / np.sum(weights))
+        # Calculate mean and standard deviation. NOTE: makes the assumption that the
+        # distribution of these magnitude observations can locally be approximated by a
+        # normal distribution. In reality it will have a negative skew, making the mean
+        # magnitude a slight underestimate.
+        mean_mag = np.sum(mags * weights) / np.sum(weights)
+        mean_mag_err = np.sqrt(
+            np.sum(((mags - mean_mag) * weights) ** 2) / np.sum(weights)
+        )
 
         # Pass the magnitudes (filtered & un-filtered) to the _mag_r_squared
         # function.
-        mag_r_squared = self._mag_r_squared(all_mags, mean_mag,
-                                            only_used=self.r2_only_used)
+        mag_r_squared = self._mag_r_squared(
+            all_mags, mean_mag, only_used=self.r2_only_used
+        )
 
         return mean_mag, mean_mag_err, mag_r_squared, all_mags
 
-    def plot_amplitudes(self, magnitudes, event, run, unit_conversion_factor,
-                        noise_measure="RMS"):
-        """
-        Plot a figure showing the measured amplitude with distance vs.
-        predicted amplitude with distance derived from mean_mag and the chosen
-        attenuation model.
-
-        The amplitude observations (both for noise and signal amplitudes) are
-        corrected according to the same station corrections that were used in
-        calculating the individual local magnitude estimates that were used to
-        calculate the network-averaged local magnitude for the event.
+    def plot_amplitudes(
+        self, magnitudes, event, run, unit_conversion_factor, noise_measure="RMS"
+    ):
+        """
+        Plot a figure showing the measured amplitude with distance vs. predicted
+        amplitude with distance derived from mean_mag and the chosen attenuation model.
+
+        The amplitude observations (both for noise and signal amplitudes) are corrected
+        according to the same station corrections that were used in calculating the
+        individual local magnitude estimates that were used to calculate the
+        network-averaged local magnitude for the event.
 
         Parameters
         ----------
         magnitudes : `pandas.DataFrame` object
-            Contains P- and S-wave amplitude measurements for each component of
-            each station in the look-up table, and local magnitude estimates
-            calculated from them (output by calculate_magnitudes()). Note that
-            the amplitude observations are raw, but the ML estimates derived
-            from them include station corrections, if provided.
-            Columns = ["epi_dist", "z_dist", "P_amp", "P_freq", "P_time",
-                       "P_avg_amp", "P_filter_gain", "S_amp", "S_freq",
-                       "S_time", "S_avg_amp", "S_filter_gain", "Noise_amp",
-                       "is_picked", "ML", "ML_Err"], "Noise_Filter",
-                       "Trace_Filter", "Station_Filter", "Dist_Filter", "Dist",
-                       "Used"]
+            Contains P- and S-wave amplitude measurements for each component of each
+            station in the look-up table, and local magnitude estimates calculated from
+            them (output by calculate_magnitudes()). Note that the amplitude
+            observations are raw, but the ML estimates derived from them include station
+            corrections, if provided.
+            Columns = ["epi_dist", "z_dist", "P_amp", "P_freq", "P_time", "P_avg_amp",
+                       "P_filter_gain", "S_amp", "S_freq", "S_time", "S_avg_amp",
+                       "S_filter_gain", "Noise_amp", "is_picked", "ML", "ML_Err",
+                       "Noise_Filter", "Trace_Filter", "Station_Filter", "Dist_Filter",
+                       "Dist", "Used"]
         event : :class:`~quakemigrate.io.event.Event` object
-            Light class encapsulating waveforms, coalescence information, picks
-            and location information for a given event.
+            Light class encapsulating waveforms, coalescence information, picks and
+            location information for a given event.
         run : :class:`~quakemigrate.io.core.Run` object
             Light class encapsulating i/o path information for a given run.
         unit_conversion_factor : float
-            A conversion factor based on the lookup table grid projection, used
-            to ensure the location uncertainties have units of kilometres.
+            A conversion factor based on the lookup table grid projection, used to
+            ensure the location uncertainties have units of kilometres.
 
         """
 
         mag = event.localmag["ML"]
         mag_err = event.localmag["ML_Err"]
         mag_r2 = event.localmag["ML_r2"]
 
@@ -442,76 +437,95 @@
         epi_err = np.sqrt(x_err**2 + y_err**2)
 
         if self.use_hyp_dist:
             dist_err = np.sqrt(epi_err**2 + z_err**2)
         else:
             dist_err = epi_err
 
-        all_amps = magnitudes[self.amp_feature].values * self.amp_multiplier \
-                    * np.power(10, magnitudes["Station_Correction"])
-        noise_amps = magnitudes["Noise_amp"].values * self.amp_multiplier \
-                    * np.power(10, magnitudes["Station_Correction"])
+        all_amps = (
+            magnitudes[self.amp_feature].values
+            * self.amp_multiplier
+            * np.power(10, magnitudes["Station_Correction"])
+        )
+        noise_amps = (
+            magnitudes["Noise_amp"].values
+            * self.amp_multiplier
+            * np.power(10, magnitudes["Station_Correction"])
+        )
         filter_gains = magnitudes[f"{self.amp_feature[0]}_filter_gain"]
         if not filter_gains.isnull().values.any():
             noise_amps /= filter_gains
 
         dist = magnitudes["Dist"]
 
         # Find min/max values for x and y axes
         amps_max = all_amps.max() * 5
         amps_min = noise_amps.min() / 10
         dist_min = dist.min() / 2
         dist_max = dist.max() * 1.5
 
-        _, ax = amplitudes_summary(magnitudes, self.amp_feature,
-                                   self.amp_multiplier, dist_err, mag_r2,
-                                   noise_measure)
+        _, ax = amplitudes_summary(
+            magnitudes,
+            self.amp_feature,
+            self.amp_multiplier,
+            dist_err,
+            mag_r2,
+            noise_measure,
+        )
 
         # -- Calculate predicted amplitudes from ML & attenuation function --
-        # Upper and lower bounds for predicted amplitude from upper/lower
-        # bounds for mag
+        # Upper and lower bounds for predicted amplitude from upper/lower bounds for mag
         mag_upper = mag + mag_err
         mag_lower = mag - mag_err
 
         # Calculated attenuation correction for full range of distances
         distances = np.linspace(dist_min, dist_max, 10000)
         att = self._get_attenuation(distances)
 
         # Calculate predicted amplitude with distance
         predicted_amp = np.power(10, (mag - att))
         predicted_amp_upper = np.power(10, (mag_upper - att))
         predicted_amp_lower = np.power(10, (mag_lower - att))
 
         # Plot predicted amplitude with distance
-        label = (f'Predicted amplitude for ML = {mag:.2f} \u00B1 {mag_err:.2f}'
-                 f'\nusing attenuation curve "{self.A0}"')
-        ax.plot(distances, predicted_amp, linestyle='-', c='r', label=label)
-        ax.plot(distances, predicted_amp_upper, linestyle='--', c='r')
-        ax.plot(distances, predicted_amp_lower, linestyle='--', c='r')
+        label = (
+            f"Predicted amplitude for ML = {mag:.2f} \u00B1 {mag_err:.2f}"
+            f'\nusing attenuation curve "{self.A0}"'
+        )
+        ax.plot(distances, predicted_amp, linestyle="-", c="r", label=label)
+        ax.plot(distances, predicted_amp_upper, linestyle="--", c="r")
+        ax.plot(distances, predicted_amp_lower, linestyle="--", c="r")
 
         # If distance filter specified, add it to the plot
         if self.dist_filter:
-            ax.axvline(self.dist_filter, linestyle='--', ymin=0, ymax=amps_max,
-                       color='k', label='Distance filter')
+            ax.axvline(
+                self.dist_filter,
+                linestyle="--",
+                ymin=0,
+                ymax=amps_max,
+                color="k",
+                label="Distance filter",
+            )
 
         # Set axis limits
         ax.set_xlim(dist_min, dist_max)
         ax.set_ylim(amps_min, max(np.max(predicted_amp), amps_max))
 
         # Set figure and axis titles
-        ax.set_title(f'Amplitude vs distance plot for event: "{event.uid}"',
-                     fontsize=18)
-        ax.set_ylabel('Amplitude / mm', fontsize=16)
+        ax.set_title(
+            f'Amplitude vs distance plot for event: "{event.uid}"', fontsize=18
+        )
+        ax.set_ylabel("Amplitude / mm", fontsize=16)
         if self.use_hyp_dist:
-            ax.set_xlabel('Hypocentral Distance / km', fontsize=16)
+            ax.set_xlabel("Hypocentral Distance / km", fontsize=16)
         else:
-            ax.set_xlabel('Epicentral Distance / km', fontsize=16)
+            ax.set_xlabel("Epicentral Distance / km", fontsize=16)
 
         # Add legend
-        ax.legend(fontsize=16, loc='upper right')
+        ax.legend(fontsize=16, loc="upper right")
 
         # Specify tight layout
         plt.tight_layout()
 
         fpath = run.path / "locate" / run.subname / "amplitude_plots"
         fpath.mkdir(exist_ok=True, parents=True)
         fstem = f"{run.name}_{event.uid}_AmpVsDistance"
@@ -526,53 +540,54 @@
         Parameters
         ----------
         trace_ids : array-like, contains strings
             List of ID strings for each trace.
         amps : array-like, contains floats
             Measurements of *half* peak-to-trough amplitudes, in *millimetres*
         noise_amps : array-like, contains floats
-            Estimate of uncertainty in amplitude measurements caused by noise
-            on the signal. Also in mm.
+            Estimate of uncertainty in amplitude measurements caused by noise on the
+            signal. Also in mm.
         dist : array-like, contains floats
             Distances between source and receiver in kilometres.
 
         Returns
         -------
         mags : array-like
-            Magnitudes for each channel calculated from the chosen amplitude
-            measurement (P or S).
+            Magnitudes for each channel calculated from the chosen amplitude measurement
+            (P or S).
         mag_errs : array-like
-            Estimate of the error on the calculated magnitude, based on
-            potential errors in the maximum amplitude measurement according to
-            the measured noise amplitude.
+            Estimate of the error on the calculated magnitude, based on potential errors
+            in the maximum amplitude measurement according to the measured noise
+            amplitude.
 
         """
 
         # Read in station corrections for each trace
-        corrs = [self.station_corrections[t] if t in
-                 self.station_corrections.keys() else 0. for t in trace_ids]
+        corrs = [
+            self.station_corrections[t] if t in self.station_corrections.keys() else 0.0
+            for t in trace_ids
+        ]
 
         att = self._get_attenuation(dist)
 
         # Calculate magnitudes
         mags = np.log10(amps) + att + np.array(corrs)
 
-        # Simple estimate of magnitude error based on the upper and lower
-        # bounds of the amplitude measurements according to the measured noise
-        # amplitude
+        # Simple estimate of magnitude error based on the upper and lower bounds of the
+        # amplitude measurements according to the measured noise amplitude
         upper_mags = np.log10(amps + noise_amps) + att + np.array(corrs)
         lower_mags = np.log10(amps - noise_amps) + att + np.array(corrs)
         mag_errs = upper_mags - lower_mags
 
         return mags, mag_errs
 
     def _get_attenuation(self, dist):
         """
-        Calculate attenuation according to user-provided or built-in logA0
-        attenuation function.
+        Calculate attenuation according to user-provided or built-in logA0 attenuation
+        function.
 
         Parameters
         ----------
         dist : float or array-like
             Distance(s) between source and receiver.
 
         Returns
@@ -623,228 +638,236 @@
             If invalid A0 attenuation function is specified.
 
         """
 
         eqn = self.A0
 
         if eqn == "keir2006":
-            att = 1.196997*np.log10(dist/17.) + 0.001066*(dist - 17.) + 2.
+            att = 1.196997 * np.log10(dist / 17.0) + 0.001066 * (dist - 17.0) + 2.0
         elif eqn == "Danakil2017":
-            att = 1.274336*np.log10(dist/17.) - 0.000273*(dist - 17.) + 2.
+            att = 1.274336 * np.log10(dist / 17.0) - 0.000273 * (dist - 17.0) + 2.0
         elif eqn == "Greenfield2018_askja":
-            att = 1.4406*np.log10(dist/17.) + 0.003*(dist - 17.) + 2.
+            att = 1.4406 * np.log10(dist / 17.0) + 0.003 * (dist - 17.0) + 2.0
         elif eqn == "Greenfield2018_bardarbunga":
-            att = 1.2534*np.log10(dist/17.) + 0.0032*(dist - 17.) + 2.
+            att = 1.2534 * np.log10(dist / 17.0) + 0.0032 * (dist - 17.0) + 2.0
         elif eqn == "Greenfield2018_comb":
-            att = 1.1999*np.log10(dist/17.) + 0.0016*(dist - 17.) + 2.
+            att = 1.1999 * np.log10(dist / 17.0) + 0.0016 * (dist - 17.0) + 2.0
         elif eqn == "Hutton-Boore":
-            att = 1.11*np.log10(dist/100.) + 0.00189*(dist - 100.) + 3.
+            att = 1.11 * np.log10(dist / 100.0) + 0.00189 * (dist - 100.0) + 3.0
         elif eqn == "Langston1998":
-            att = 0.776*np.log10(dist/17.) + 0.000902*(dist - 17) + 2.
+            att = 0.776 * np.log10(dist / 17.0) + 0.000902 * (dist - 17) + 2.0
         elif eqn == "UK":
-            att = 1.11*np.log10(dist) + 0.00189*dist - 1.16*np.exp(-0.2*dist) \
+            att = (
+                1.11 * np.log10(dist)
+                + 0.00189 * dist
+                - 1.16 * np.exp(-0.2 * dist)
                 - 2.09
+            )
         else:
             raise ValueError(eqn, "is not a valid A0 attenuation function.")
 
         return att
 
     def _filter_mags(self, magnitudes):
         """
-        Filter magnitudes observations according to the user-specified filters
-        for source-station distance, trace ID, etc.
+        Filter magnitudes observations according to the user-specified filters for
+        source-station distance, trace ID, etc.
 
         Parameters
         ----------
         magnitudes : `pandas.DataFrame` object
-            Contains P- and S-wave amplitude measurements for each component of
-            each station in the look-up table, and local magnitude estimates
-            calculated from them (output by calculate_magnitudes()). Note that
-            the amplitude observations are raw, but the ML estimates derived
-            from them include station corrections, if provided.
-            Columns = ["epi_dist", "z_dist", "P_amp", "P_freq", "P_time",
-                       "P_avg_amp", "P_filter_gain", "S_amp", "S_freq",
-                       "S_time", "S_avg_amp", "S_filter_gain", "Noise_amp",
-                       "is_picked", "ML", "ML_Err"]
+            Contains P- and S-wave amplitude measurements for each component of each
+            station in the look-up table, and local magnitude estimates calculated from
+            them (output by calculate_magnitudes()). Note that the amplitude
+            observations are raw, but the ML estimates derived from them include station
+            corrections, if provided.
+            Columns = ["epi_dist", "z_dist", "P_amp", "P_freq", "P_time", "P_avg_amp",
+                       "P_filter_gain", "S_amp", "S_freq", "S_time", "S_avg_amp",
+                       "S_filter_gain", "Noise_amp", "is_picked", "ML", "ML_Err"]
 
         Returns
         -------
         used_mags : `pandas.DataFrame` object
-            As input, but only including individual amplitude measurements /
-            local magnitude estimates that meet the filters specified by the
-            user. Now with additional columns:
+            As input, but only including individual amplitude measurements / local
+            magnitude estimates that meet the filters specified by the user. Now with
+            additional columns:
             Noise_Filter : bool
                 Whether this observation meets the noise filter.
             Trace_Filter : bool
                 Whether this observation matches the trace filter.
             Station_Filter : bool
                 Whether this observation is not excluded by the station filter.
             Dist_Filter : bool
                 Whether this observation meets the distance filter.
             Dist : bool
-                The (epicentral or hypocentral) distance between the station
-                and event.
+                The (epicentral or hypocentral) distance between the station and event.
             Used : bool (== True)
                 Whether the observation meets all filter requirements.
         all_mags : `pandas.DataFrame` object
-            As for used_mags, but containing all observations from the input
-            magnitudes DataFrame, other than those which feature null values
-            for the signal or noise amplitude.
+            As for used_mags, but containing all observations from the input magnitudes
+            DataFrame, other than those which feature null values for the signal or
+            noise amplitude.
 
         """
 
         # Remove nan amplitude values
         magnitudes.dropna(subset=[self.amp_feature, "Noise_amp"], inplace=True)
 
         # Apply noise filter.
-        if self.noise_filter != 0.:
+        if self.noise_filter != 0.0:
             amps = magnitudes[self.amp_feature].values
             noise_amps = magnitudes["Noise_amp"].values
             magnitudes["Noise_Filter"] = False
             with np.errstate(invalid="ignore"):
-                magnitudes.loc[(amps > noise_amps * self.noise_filter),
-                               "Noise_Filter"] = True
+                magnitudes.loc[
+                    (amps > noise_amps * self.noise_filter), "Noise_Filter"
+                ] = True
 
         # Apply trace filter
         if self.trace_filter is not None:
             magnitudes["Trace_Filter"] = False
-            magnitudes.loc[magnitudes.index.str.contains(self.trace_filter),
-                           "Trace_Filter"] = True
+            magnitudes.loc[
+                magnitudes.index.str.contains(self.trace_filter), "Trace_Filter"
+            ] = True
 
         # Apply station filter
         if self.station_filter is not None:
             magnitudes["Station_Filter"] = True
             for stn in list(self.station_filter):
-                magnitudes.loc[magnitudes.index.str.contains(f".{stn}.",
-                                                             regex=False),
-                               "Station_Filter"] = False
+                magnitudes.loc[
+                    magnitudes.index.str.contains(f".{stn}.", regex=False),
+                    "Station_Filter",
+                ] = False
 
         # Calculate distances
         edist, zdist = magnitudes["epi_dist"], magnitudes["z_dist"]
         if self.use_hyp_dist:
             dist = np.sqrt(edist.values**2 + zdist.values**2)
         else:
             dist = edist.values
 
         # Apply distance filter
         if self.dist_filter:
             magnitudes["Dist_Filter"] = False
             magnitudes.loc[(dist <= self.dist_filter), "Dist_Filter"] = True
 
         # Set distances; remove dist=0 values (logs do not like this)
-        dist[dist == 0.] = np.nan
+        dist[dist == 0.0] = np.nan
         magnitudes["Dist"] = dist
 
         # Identify used mags (after applying all filters)
         magnitudes["Used"] = True
         if self.trace_filter is not None:
             magnitudes.loc[~magnitudes["Trace_Filter"], "Used"] = False
         if self.station_filter is not None:
             magnitudes.loc[~magnitudes["Station_Filter"], "Used"] = False
         if self.dist_filter:
             magnitudes.loc[~magnitudes["Dist_Filter"], "Used"] = False
         if self.pick_filter:
             magnitudes.loc[~magnitudes["is_picked"], "Used"] = False
-        if self.noise_filter != 0.:
+        if self.noise_filter != 0.0:
             magnitudes.loc[~magnitudes["Noise_Filter"], "Used"] = False
 
         used_mags = magnitudes[magnitudes["Used"]]
 
         return used_mags, magnitudes
 
     def _mag_r_squared(self, magnitudes, mean_mag, only_used=True):
         """
-        Calculate the r-squared statistic for the fit of the amplitudes vs
-        distance model predicted by the estimated event magnitude and the
-        chosen attenuation function to the observed amplitudes. The fit is
-        calculated in log(amplitude) space to linearise the data, in order for
-        the calculation of the r-squared statistic to be appropriate.
+        Calculate the r-squared statistic for the fit of the amplitudes vs distance
+        model predicted by the estimated event magnitude and the chosen attenuation
+        function to the observed amplitudes. The fit is calculated in log(amplitude)
+        space to linearise the data, in order for the calculation of the r-squared
+        statistic to be appropriate.
 
         The raw amplitude observations are corrected according to the station
-        corrections that were used in calculating the local magnitudes from
-        which the network-averaged local magnitude was calculated.
+        corrections that were used in calculating the local magnitudes from which the
+        network-averaged local magnitude was calculated.
 
         Parameters
         ----------
         magnitudes : `pandas.DataFrame` object
-            Contains P- and S-wave amplitude measurements for each component of
-            each station in the look-up table, and local magnitude estimates
-            calculated from them (output by calculate_magnitudes()). Note that
-            the amplitude observations are raw, but the ML estimates derived
-            from them include station corrections, if provided.
-            Columns = ["epi_dist", "z_dist", "P_amp", "P_freq", "P_time",
-                       "P_avg_amp", "P_filter_gain", "S_amp", "S_freq",
-                       "S_time", "S_avg_amp", "S_filter_gain", "Noise_amp",
-                       "is_picked", "ML", "ML_Err"], "Noise_Filter",
-                       "Trace_Filter", "Station_Filter", "Dist_Filter", "Dist",
-                       "Used"]
+            Contains P- and S-wave amplitude measurements for each component of each
+            station in the look-up table, and local magnitude estimates calculated from
+            them (output by calculate_magnitudes()). Note that the amplitude
+            observations are raw, but the ML estimates derived from them include station
+            corrections, if provided.
+            Columns = ["epi_dist", "z_dist", "P_amp", "P_freq", "P_time", "P_avg_amp",
+                       "P_filter_gain", "S_amp", "S_freq", "S_time", "S_avg_amp",
+                       "S_filter_gain", "Noise_amp", "is_picked", "ML", "ML_Err",
+                       "Noise_Filter", "Trace_Filter", "Station_Filter", "Dist_Filter",
+                       "Dist", "Used"]
         mean_mag : float or NaN
-            Network-averaged local magnitude estimate for the event. Mean (or
-            weighted mean) of the magnitude estimates calculated from each
-            individual channel after optionally removing some observations
-            based on trace ID, distance, etcetera.
+            Network-averaged local magnitude estimate for the event. Mean (or weighted
+            mean) of the magnitude estimates calculated from each individual channel
+            after optionally removing some observations based on trace ID, distance,
+            etcetera.
         only_used : bool
-            Only calculate the r-squared value from those magnitudes which were
-            included in calculating the network-averaged `mean_mag`.
+            Only calculate the r-squared value from those magnitudes which were included
+            in calculating the network-averaged `mean_mag`.
 
         Returns
         -------
         mag_r_squared : float or NaN
-            r-squared statistic describing the fit of the amplitude vs.
-            distance curve predicted by the calculated mean_mag and chosen
-            attenuation model to the measured amplitude observations. This is
-            intended to be used to help discriminate between 'real' events, for
-            which the predicted amplitude vs. distance curve should provide a
-            good fit to the observations, from artefacts, which in general will
-            not.
+            r-squared statistic describing the fit of the amplitude vs. distance curve
+            predicted by the calculated mean_mag and chosen attenuation model to the
+            measured amplitude observations. This is intended to be used to help
+            discriminate between 'real' events, for which the predicted amplitude vs.
+            distance curve should provide a good fit to the observations, from
+            artefacts, which in general will not.
 
         Raises
         ------
         AttributeError
-            If the user selects `only_used=False` but does not specify a noise
-            filter.
+            If the user selects `only_used=False` but does not specify a noise filter.
 
         """
 
         if only_used:
-            # Only keep magnitude estimates which meet all the user-specified
-            # filter requirements.
+            # Only keep magnitude estimates which meet all the user-specified filter
+            # requirements.
             magnitudes = magnitudes[magnitudes["Used"]]
         else:
-            # Apply a default set of filters (including some of the
-            # user-specified filters)
+            # Apply a default set of filters (including some of the user-specified
+            # filters)
             if self.trace_filter is not None:
                 magnitudes = magnitudes[magnitudes["Trace_Filter"]]
             if self.station_filter is not None:
                 magnitudes = magnitudes[magnitudes["Station_Filter"]]
             if self.dist_filter:
                 magnitudes = magnitudes[magnitudes["Dist_Filter"]]
-            # Apply a custom version of the noise filter, in order to keep
-            # observations where the signal would be expected to be above the
-            # noise threshold
-            if self.noise_filter <= 0.:
-                msg = ("Noise filter must be greater than 1 to use custom mag "
-                       "r-squared filtering. Change 'only_used' to True, or "
-                       f"set a noise filter (current = {self.noise_filter}")
-                raise AttributeError(msg)
+            # Apply a custom version of the noise filter, in order to keep observations
+            # where the signal would be expected to be above the noise threshold
+            if self.noise_filter <= 0.0:
+                raise AttributeError(
+                    "Noise filter must be greater than 1 to use custom mag "
+                    "r-squared filtering. Change 'only_used' to True, or "
+                    f"set a noise filter (current = {self.noise_filter}"
+                )
             for _, mag in magnitudes[~magnitudes["Noise_Filter"]].iterrows():
                 # Correct noise amp for station correction
-                noise_amp = mag["Noise_amp"] * self.amp_multiplier \
+                noise_amp = (
+                    mag["Noise_amp"]
+                    * self.amp_multiplier
                     * np.power(10, mag["Station_Correction"])
+                )
                 # Calculate predicted amp
                 att = self._get_attenuation(mag["Dist"])
                 predicted_amp = np.power(10, (mean_mag - att))
                 # If predicted amp is more than 5x larger than noise amp, keep
                 # this observation for mag_r2 calculation
                 if predicted_amp / noise_amp < 5:
                     magnitudes.drop(labels=mag.name)
 
         # Calculate amplitudes -- including station corrections!
-        amps = magnitudes[self.amp_feature].values * self.amp_multiplier * \
-            np.power(10, magnitudes["Station_Correction"])
+        amps = (
+            magnitudes[self.amp_feature].values
+            * self.amp_multiplier
+            * np.power(10, magnitudes["Station_Correction"])
+        )
 
         dist = magnitudes["Dist"]
         att = self._get_attenuation(dist)
 
         # Find variance of log(amplitude) observations -- doing this in log
         # space to linearise the problem (so that r_squared is meaningful)
         log_amp_mean = np.log10(amps).mean()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quakemigrate-1.0.1/quakemigrate/signal/onsets/__init__.py` & `quakemigrate-1.0.2/quakemigrate/signal/onsets/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
 """
-The :mod:`quakemigrate.onsets` module handles the generation of Onset
-functions. The default method uses the ratio between the short-term and
-long-term averages of the signal amplitude.
+The :mod:`quakemigrate.onsets` module handles the generation of Onset functions. The
+default method uses the ratio between the short-term and long-term averages of the
+signal amplitude.
 
 Feel free to contribute more Onset function options!
 
 :copyright:
-    2020 - 2021, QuakeMigrate developers.
+    2020–2023, QuakeMigrate developers.
 :license:
     GNU General Public License, Version 3
     (https://www.gnu.org/licenses/gpl-3.0.html)
 
 """
 
 from .base import Onset  # NOQA
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quakemigrate-1.0.1/quakemigrate/signal/onsets/base.py` & `quakemigrate-1.0.2/quakemigrate/signal/onsets/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # -*- coding: utf-8 -*-
 """
-A simple abstract base class with method stubs to enable users to extend
-QuakeMigrate with custom onset functions that remain compatible with the core
-of the package.
+A simple abstract base class with method stubs to enable users to extend QuakeMigrate
+with custom onset functions that remain compatible with the core of the package.
 
-Also contains a light class to encapsulate the data generated by the onset
-function, to be used for migration or phase picking.
+Also contains a light class to encapsulate the data generated by the onset function, to
+be used for migration or phase picking.
 
 :copyright:
-    2020 - 2021, QuakeMigrate developers.
+    2020–2023, QuakeMigrate developers.
 :license:
     GNU General Public License, Version 3
     (https://www.gnu.org/licenses/gpl-3.0.html)
 
 """
 
 from abc import ABC, abstractmethod
@@ -25,19 +24,19 @@
 class Onset(ABC):
     """
     QuakeMigrate default onset function class.
 
     Attributes
     ----------
     sampling_rate : int
-        Desired sampling rate for input data; sampling rate at which the onset
-        functions will be computed.
+        Desired sampling rate for input data; sampling rate at which the onset functions
+        will be computed.
     pre_pad : float, optional
-        Option to override the default pre-pad duration of data to read before
-        computing 4-D coalescence in detect() and locate().
+        Option to override the default pre-pad duration of data to read before computing
+        4-D coalescence in detect() and locate().
     post_pad : float
         Option to override the default post-pad duration of data to read before
         computing 4-D coalescence in detect() and locate().
 
     Methods
     -------
     calculate_onsets()
@@ -60,49 +59,50 @@
     def __str__(self):
         """Return short summary string of the Onset object."""
 
         return "Base Onset object - add a __str__ method to your Onset class"
 
     def pad(self, timespan):
         """
-        Determine the number of samples needed to pre- and post-pad the
-        timespan.
+        Determine the number of samples needed to pre- and post-pad the timespan.
 
         Parameters
         ----------
         timespan : float
             The time window to pad.
 
         Returns
         -------
         pre_pad : float
-            Option to override the default pre-pad duration of data to read
-            before computing 4-D coalescence in detect() and locate().
+            Option to override the default pre-pad duration of data to read before
+            computing 4-D coalescence in detect() and locate().
         post_pad : float
-            Option to override the default post-pad duration of data to read
-            before computing 4-D coalescence in detect() and locate().
+            Option to override the default post-pad duration of data to read before
+            computing 4-D coalescence in detect() and locate().
 
         """
 
         # Add additional padding for any tapering applied to data
-        timespan += (self.pre_pad + self.post_pad)
-        pre_pad = util.trim2sample(self.pre_pad + np.ceil(timespan*0.06),
-                                   self.sampling_rate)
-        post_pad = util.trim2sample(self.post_pad + np.ceil(timespan*0.06),
-                                    self.sampling_rate)
+        timespan += self.pre_pad + self.post_pad
+        pre_pad = util.trim2sample(
+            self.pre_pad + np.ceil(timespan * 0.06), self.sampling_rate
+        )
+        post_pad = util.trim2sample(
+            self.post_pad + np.ceil(timespan * 0.06), self.sampling_rate
+        )
 
         return pre_pad, post_pad
 
     def gaussian_halfwidth(self, phase):
         """Method stub for Gaussian half-width estimate."""
 
-        msg = ("In order to use the GaussianPicker module with a custom Onset,"
-               " you need to provide a 'gaussian_halfwidth' method.")
-
-        raise AttributeError(msg)
+        raise AttributeError(
+            "In order to use the GaussianPicker module with a custom Onset, you need "
+            "to provide a 'gaussian_halfwidth' method."
+        )
 
     @abstractmethod
     def calculate_onsets(self):
         """Method stub for calculation of onset functions."""
         pass
 
     @property
@@ -128,53 +128,60 @@
     def post_pad(self, value):
         """Set property stub for pre_pad."""
         self._post_pad = value
 
 
 class OnsetData:
     """
-    The OnsetData class encapsulates the onset functions calculated by
-    transforming seismic data using the chosen onset detection algorithm
-    (characteristic function).
-
-    This includes a dictionary describing which onset functions are available
-    for each station and phase, and the intermediary filtered or otherwise
-    pre-processed waveform data used to calculate the onset function.
+    The OnsetData class encapsulates the onset functions calculated by transforming
+    seismic data using the chosen onset detection algorithm (characteristic function).
+
+    This includes a dictionary describing which onset functions are available for each
+    station and phase, and the intermediary filtered or otherwise pre-processed waveform
+    data used to calculate the onset function.
 
     Parameters
     ----------
     onsets : dict of dicts
-        Keys "station", each of which contains keys for each phase, e.g. "P"
-        and "S". {"station": {"P": `p_onset`, "S": `s_onset`}}. Onset
-        functions are calculated by transforming the raw seismic data using
-        some characteristic function designed to highlight phase arrivals.
+        Keys "station", each of which contains keys for each phase, e.g. "P" and "S".
+        {"station": {"P": `p_onset`, "S": `s_onset`}}. Onset functions are calculated by
+        transforming the raw seismic data using some characteristic function designed to
+        highlight phase arrivals.
     phases : list of str
         Phases for which onsets have been calculated. (e.g. ["P", "S"])
     channel_maps : dict of str
         Data component maps - keys are phases. (e.g. {"P": "Z"})
     filtered_waveforms : `obspy.Stream` object
-        Filtered and/or resampled and otherwise processed seismic data
-        generated during onset function generation. Only contains waveforms
-        that have passed the quality control criteria, at a unified sampling
-        rate - see `sampling_rate`.
+        Filtered and/or resampled and otherwise processed seismic data generated during
+        onset function generation. Only contains waveforms that have passed the quality
+        control criteria, at a unified sampling rate - see `sampling_rate`.
     availability : dict
-        Dictionary with keys "station_phase", containing 1's or 0's
-        corresponding to whether an onset function is available for that
-        station and phase - determined by data availability and quality checks.
+        Dictionary with keys "station_phase", containing 1's or 0's corresponding to
+        whether an onset function is available for that station and phase - determined
+        by data availability and quality checks.
     starttime : `obspy.UTCDateTime` object
         Start time of onset functions.
     endtime : `obspy.UTCDateTime` object
         End time of onset functions.
     sampling_rate : int
         Sampling rate of filtered waveforms and onset functions.
 
     """
 
-    def __init__(self, onsets, phases, channel_maps, filtered_waveforms,
-                 availability, starttime, endtime, sampling_rate):
+    def __init__(
+        self,
+        onsets,
+        phases,
+        channel_maps,
+        filtered_waveforms,
+        availability,
+        starttime,
+        endtime,
+        sampling_rate,
+    ):
         """Instantiate the OnsetData object."""
 
         self.onsets = onsets
         self.phases = phases
         self.channel_maps = channel_maps
         self.filtered_waveforms = filtered_waveforms
         self.availability = availability
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quakemigrate-1.0.1/quakemigrate/signal/onsets/stalta.py` & `quakemigrate-1.0.2/quakemigrate/signal/onsets/stalta.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """
-The default onset function class - performs some pre-processing on raw
-seismic data and calculates STA/LTA onset (characteristic) function.
+The default onset function class - performs some pre-processing on raw seismic data and
+calculates STA/LTA onset (characteristic) function.
 
 :copyright:
-    2020 - 2021, QuakeMigrate developers.
+    2020–2023, QuakeMigrate developers.
 :license:
     GNU General Public License, Version 3
     (https://www.gnu.org/licenses/gpl-3.0.html)
 
 """
 
 import logging
@@ -19,331 +19,327 @@
 
 import quakemigrate.util as util
 from .base import Onset, OnsetData
 
 
 def sta_lta_centred(signal, nsta, nlta):
     """
-    Calculates the ratio of the average of a^2 in a short-term (signal) window
-    to a preceding long-term (noise) window. STA/LTA value is assigned to the
-    end of the LTA / one sample before the start of the STA.
+    Calculates the ratio of the average of a^2 in a short-term (signal) window to a
+    preceding long-term (noise) window. STA/LTA value is assigned to the end of the LTA
+    /one sample before the start of the STA.
 
     Parameters
     ----------
     signal : array-like
         Signal array
     nsta : int
         Number of samples in short-term window
     nlta : int
         Number of samples in long-term window
 
     Returns
     -------
     sta / lta : array-like
-        Ratio of a^2 in a short term average window to a preceding long term
-        average window. STA/LTA value is assigned to end of LTA window / one
-        sample before the start of STA window -- "centred".
+        Ratio of a^2 in a short term average window to a preceding long term average
+        window. STA/LTA value is assigned to end of LTA window / one sample before the
+        start of STA window -- "centred".
 
     """
 
     # Cumulative sum to calculate moving average
-    sta = np.cumsum(signal ** 2)
+    sta = np.cumsum(signal**2)
     sta = np.require(sta, dtype=float)
     lta = sta.copy()
 
     # Compute the STA and the LTA
     sta[nsta:] = sta[nsta:] - sta[:-nsta]
-    sta[nsta:-nsta] = sta[nsta*2:]
+    sta[nsta:-nsta] = sta[nsta * 2 :]
     sta /= nsta
 
     lta[nlta:] = lta[nlta:] - lta[:-nlta]
     lta /= nlta
 
-    sta[:(nlta - 1)] = 0
+    sta[: (nlta - 1)] = 0
     sta[-nsta:] = 0
 
     # Avoid division by zero by setting zero values to tiny float
     dtiny = np.finfo(float).tiny
     idx = lta < dtiny
     lta[idx] = dtiny
     sta[idx] = 0.0
 
     return sta / lta
 
 
-def pre_process(stream, sampling_rate, resample, upfactor, filter_,
-                starttime, endtime):
+def pre_process(stream, sampling_rate, resample, upfactor, filter_, starttime, endtime):
     """
-    Resample raw seismic data, detrend and apply cosine taper and zero
-    phase-shift Butterworth band-pass filter; all carried out using the
-    built-in obspy functions.
-
-    By default, data with mismatched sampling rates will only be decimated.
-    If necessary, and if the user has specified `resample = True` and an
-    `upfactor` to upsample by `upfactor = int` for the waveform archive, data
-    can also be upsampled and then, if necessary, subsequently decimated to
-    achieve the desired sampling rate.
-
-    For example, for raw input data sampled at a mix of 40, 50 and 100 Hz,
-    to achieve a unified sampling rate of 50 Hz, the user would have to
-    specify an `upfactor` of 5; 40 Hz x 5 = 200 Hz, which can then be
-    decimated to 50 Hz.
-
-    NOTE: data will be detrended and a cosine taper applied before
-    decimation, in order to avoid edge effects when applying the lowpass
-    filter. See :func:`~quakemigrate.util.resample`
+    Resample raw seismic data, detrend and apply cosine taper and zero phase-shift
+    Butterworth band-pass filter; all carried out using the built-in obspy functions.
+
+    By default, data with mismatched sampling rates will only be decimated. If
+    necessary, and if the user has specified `resample = True` and an `upfactor` to
+    upsample by `upfactor = int` for the waveform archive, data can also be upsampled
+    and then, if necessary, subsequently decimated to achieve the desired sampling rate.
+
+    For example, for raw input data sampled at a mix of 40, 50 and 100 Hz, to achieve a
+    unified sampling rate of 50 Hz, the user would have to specify an `upfactor` of 5;
+    40 Hz x 5 = 200 Hz, which can then be decimated to 50 Hz.
+
+    NOTE: data will be detrended and a cosine taper applied before decimation, in order
+    to avoid edge effects when applying the lowpass filter.
+    See :func:`~quakemigrate.util.resample`
 
     Parameters
     ----------
     stream : `obspy.Stream` object
         Waveform data to be pre-processed.
     sampling_rate : int
-        Desired sampling rate for data to be used to calculate onset. This will
-        be achieved by resampling the raw waveform data. By default, only
-        decimation will be applied, but data can also be upsampled if
-        specified by the user when creating the
-        :class:`~quakemigrate.io.data.Archive` object.
+        Desired sampling rate for data to be used to calculate onset. This will be
+        achieved by resampling the raw waveform data. By default, only decimation will
+        be applied, but data can also be upsampled if specified by the user when
+        creating the :class:`~quakemigrate.io.data.Archive` object.
     resample : bool, optional
-        If true, perform resampling of data which cannot be decimated directly
-        to the desired sampling rate. See :func:`~quakemigrate.util.resample`
+        If true, perform resampling of data which cannot be decimated directly to the
+        desired sampling rate. See :func:`~quakemigrate.util.resample`
     upfactor : int, optional
-        Factor by which to upsample the data to enable it to be decimated to
-        the desired sampling rate, e.g. 40Hz -> 50Hz requires upfactor = 5.
+        Factor by which to upsample the data to enable it to be decimated to the desired
+        sampling rate, e.g. 40Hz -> 50Hz requires upfactor = 5.
         See :func:`~quakemigrate.util.resample`
     filter_ : list
-        Filter specifications, as [lowcut (Hz), highcut (Hz), order]. NOTE -
-        two-pass filter effectively doubles the number of corners (order).
+        Filter specifications, as [lowcut (Hz), highcut (Hz), order]. NOTE - two-pass
+        filter effectively doubles the number of corners (order).
 
     Returns
     -------
     filtered_waveforms : `obspy.Stream` object
         Pre-processed seismic data.
 
     Raises
     ------
     NyquistException
-        If the high-cut filter specified for the bandpass filter is higher than
-        the Nyquist frequency of the `sampling_rate`.
+        If the high-cut filter specified for the bandpass filter is higher than the
+        Nyquist frequency of the `sampling_rate`.
 
     """
 
     logging.debug(stream.__str__(extended=True))
     logging.debug(f"Resample={resample}, Upfactor={upfactor}")
     # Resample the data here
-    resampled_stream = util.resample(stream, sampling_rate, resample, upfactor,
-                                     starttime, endtime)
+    resampled_stream = util.resample(
+        stream, sampling_rate, resample, upfactor, starttime, endtime
+    )
 
     # Grab filter info
     lowcut, highcut, order = filter_
     # Check that the filter is compatible with the sampling rate
     if highcut >= 0.5 * sampling_rate:
         raise util.NyquistException(highcut, 0.5 * sampling_rate, "")
 
     # Detrend, apply cosine taper then apply zero-phase band-pass filter
     # Copy to not operate in-place on the input stream
     filtered_waveforms = resampled_stream.copy()
     filtered_waveforms.detrend("linear")
     filtered_waveforms.detrend("constant")
     filtered_waveforms.taper(type="cosine", max_percentage=0.05)
-    filtered_waveforms.filter(type="bandpass", freqmin=lowcut, freqmax=highcut,
-                              corners=order, zerophase=True)
+    filtered_waveforms.filter(
+        type="bandpass", freqmin=lowcut, freqmax=highcut, corners=order, zerophase=True
+    )
 
     return filtered_waveforms
 
 
 class STALTAOnset(Onset):
     """
-    QuakeMigrate default onset function class - uses the Short-Term Average to
-    Long-Term Average ratio of the signal energy amplitude.
+    QuakeMigrate default onset function class - uses the Short-Term Average to Long-Term
+    Average ratio of the signal energy amplitude.
 
-    Raw seismic data will be pre-processed, including re-sampling if necessary
-    to reach the specified uniform sampling raate, checked against a user-
-    specified set of data quality criteria, then used to calculate onset
-    functions for each phase (using seismic channels as specified in
-    `channel_maps`) by computing the STA/LTA of s^2.
+    Raw seismic data will be pre-processed, including re-sampling if necessary to reach
+    the specified uniform sampling raate, checked against a user- specified set of data
+    quality criteria, then used to calculate onset functions for each phase (using
+    seismic channels as specified in `channel_maps`) by computing the STA/LTA of s^2.
 
     Attributes
     ----------
     phases : list of str
-        Which phases to calculate onset functions for. This will determine
-        which phases are used for migration/picking. The selected phases
-        must be present in the travel-time look-up table to be used for
-        these purposes.
+        Which phases to calculate onset functions for. This will determine which phases
+        are used for migration/picking. The selected phases must be present in the
+        travel-time look-up table to be used for these purposes.
     bandpass_filters : dict of [float, float, int]
         Butterworth bandpass filter specification - keys are phases.
         [lowpass (Hz), highpass (Hz), corners*]
         *NOTE: two-pass filter effectively doubles the number of corners.
     channel_maps : dict of str
         Data component maps - keys are phases. These are passed into the
         :meth:`ObsPy.stream.select` method.
     channel_counts : dict of int
-        Number of channels to be used to calculate the onset function for each
-        phase. Keys are phases.
+        Number of channels to be used to calculate the onset function for each phase.
+        Keys are phases.
     sta_lta_windows : dict of [float, float]
-        Short-term average (STA) and Long-term average (LTA) window lengths -
-        keys are phases. [STA, LTA] (both in seconds)
+        Short-term average (STA) and Long-term average (LTA) window lengths - keys are
+        phases. [STA, LTA] (both in seconds)
     all_channels : bool
-        If True, only calculate an onset function when all requested channels
-        meet the availability criteria. Otherwise, if at least one channel is
-        available (e.g. just the N component for the S phase) the onset
-        function will be calculated from that/those.
+        If True, only calculate an onset function when all requested channels meet the
+        availability criteria. Otherwise, if at least one channel is available (e.g.
+        just the N component for the S phase) the onset function will be calculated from
+        that/those.
     allow_gaps : bool
-        If True, allow gappy data to be used to calculate the onset function.
-        Gappy data will be detrended, tapered and filtered, then gaps padded
-        with zeros. This should help mitigate the expected spikes as data
-        goes on- and off-line, but will not eliminate it. Onset functions for
-        periods with no data will be filled with ~ zeros (smallest possible
-        float, to avoid divide by zero errors). NOTE: This feature is
-        experimental and still under development.
+        If True, allow gappy data to be used to calculate the onset function. Gappy data
+        will be detrended, tapered and filtered, then gaps padded with zeros. This
+        should help mitigate the expected spikes as data goes on- and off-line, but will
+        not eliminate it. Onset functions for periods with no data will be filled with
+        ~ zeros (smallest possible float, to avoid divide by zero errors). NOTE: This
+        feature is experimental and still under development.
     full_timespan : bool
-        If False, allow data which doesn't cover the full timespan requested
-        to be used for onset function calculation. This is a subtly different
-        test to `allow_gaps`; data must be continuous within the timespan, but
-        may not span the whole period. Data will be treated as described in
-        `allow_gaps`. NOTE: This feature is experimental and still under
-        development.
+        If False, allow data which doesn't cover the full timespan requested to be used
+        for onset function calculation. This is a subtly different test to `allow_gaps`;
+        data must be continuous within the timespan, but may not span the whole period.
+        Data will be treated as described in `allow_gaps`. NOTE: This feature is
+        experimental and still under development.
     position : str, optional
-        Compute centred STA/LTA (STA window is preceded by LTA window;
-        value is assigned to end of LTA window / start of STA window) or
-        classic STA/LTA (STA window is within LTA window; value is assigned
-        to end of STA & LTA windows). Default: "classic".
-
-        Centred gives less phase-shifted (late) onset function, and is
-        closer to a Gaussian approximation, but is far more sensitive to
-        data with sharp offsets due to instrument failures. We recommend
-        using classic for detect() and centred for locate() if your data
-        quality allows it. This is the default behaviour; override by
-        setting this variable.
+        Compute centred STA/LTA (STA window is preceded by LTA window; value is assigned
+        to end of LTA window / start of STA window) or classic STA/LTA (STA window is
+        within LTA window; value is assigned to end of STA & LTA windows).
+        Default: "classic".
+
+        Centred gives less phase-shifted (late) onset function, and is closer to a
+        Gaussian approximation, but is far more sensitive to data with sharp offsets due
+        to instrument failures. We recommend using classic for detect() and centred for
+        locate() if your data quality allows it. This is the default behaviour; override
+        by setting this variable.
     sampling_rate : int
-        Desired sampling rate for input data, in Hz; sampling rate at which
-        the onset functions will be computed.
+        Desired sampling rate for input data, in Hz; sampling rate at which the onset
+        functions will be computed.
 
     Methods
     -------
     calculate_onsets
         Generate onset functions that represent seismic phase arrivals.
     gaussian_halfwidth
-        Phase-appropriate Gaussian half-width estimate based on the short-term
-        average window length.
+        Phase-appropriate Gaussian half-width estimate based on the short-term average
+        window length.
 
     """
 
     def __init__(self, **kwargs):
         """Instantiate the STALTAOnset object."""
 
         super().__init__(**kwargs)
 
         self.position = kwargs.get("position", "classic")
         self.phases = kwargs.get("phases", ["P", "S"])
-        self.bandpass_filters = kwargs.get("bandpass_filters",
-                                           {"P": [2.0, 16.0, 2],
-                                            "S": [2.0, 16.0, 2]})
-        self.sta_lta_windows = kwargs.get("sta_lta_windows", {"P": [0.2, 1.0],
-                                                              "S": [0.2, 1.0]})
-        self.channel_maps = kwargs.get("channel_maps", {"P": "*Z",
-                                                        "S": "*[N,E,1,2]"})
-        self.channel_counts = kwargs.get("channel_counts", {"P": 1,
-                                                            "S": 2})
+        self.bandpass_filters = kwargs.get(
+            "bandpass_filters", {"P": [2.0, 16.0, 2], "S": [2.0, 16.0, 2]}
+        )
+        self.sta_lta_windows = kwargs.get(
+            "sta_lta_windows", {"P": [0.2, 1.0], "S": [0.2, 1.0]}
+        )
+        self.channel_maps = kwargs.get("channel_maps", {"P": "*Z", "S": "*[N,E,1,2]"})
+        self.channel_counts = kwargs.get("channel_counts", {"P": 1, "S": 2})
         self.all_channels = kwargs.get("all_channels", False)
         self.allow_gaps = kwargs.get("allow_gaps", False)
         self.full_timespan = kwargs.get("full_timespan", True)
 
         # --- Deprecated ---
         self.onset_centred = kwargs.get("onset_centred")
         self.p_bp_filter = kwargs.get("p_bp_filter")
         self.s_bp_filter = kwargs.get("s_bp_filter")
         self.p_onset_win = kwargs.get("p_onset_win")
         self.s_onset_win = kwargs.get("s_onset_win")
 
     def __str__(self):
         """Return short summary string of the Onset object."""
 
-        out = (f"\tOnset parameters - using the {self.position} STA/LTA onset"
-               f"\n\t\tOnset function sampling rate = {self.sampling_rate} Hz"
-               f"\n\t\tPhase(s) = {self.phases}\n")
+        out = (
+            f"\tOnset parameters - using the {self.position} STA/LTA onset"
+            f"\n\t\tOnset function sampling rate = {self.sampling_rate} Hz"
+            f"\n\t\tPhase(s) = {self.phases}\n"
+        )
         for phase, filt in self.bandpass_filters.items():
             out += f"\n\t\t{phase} bandpass filter  = {filt} (Hz, Hz, -)"
         out += "\n"
         for phase, windows in self.sta_lta_windows.items():
             out += f"\n\t\t{phase} onset [STA, LTA] = {windows} (s, s)"
         out += "\n"
 
         return out
 
     def calculate_onsets(self, data, log=True, timespan=None):
         """
         Calculate onset functions for the requested stations and phases.
 
-        Returns a stacked array of onset functions for the requested phases,
-        and an :class:`~quakemigrate.signal.onsets.base.OnsetData` object
-        containing all outputs from the onset function calculation: a dict of
-        the onset functions, a Stream containing the pre-processed input
-        waveforms, and a dict of availability info describing which of the
-        requested onset functions could be calculated (depending on data
-        availability and data quality checks).
+        Returns a stacked array of onset functions for the requested phases, and an
+        :class:`~quakemigrate.signal.onsets.base.OnsetData` object containing all
+        outputs from the onset function calculation: a dict of the onset functions, a
+        Stream containing the pre-processed input waveforms, and a dict of availability
+        info describing which of the requested onset functions could be calculated
+        (depending on data availability and data quality checks).
 
         Parameters
         ----------
         data : :class:`~quakemigrate.io.data.WaveformData` object
             Light class encapsulating data returned by an archive query.
         log : bool
             Calculate log(onset) if True, otherwise calculate the raw onset.
         timespan : float or None, optional
-            If the timespan for which the onsets are being generated is
-            provided, this will be used to calculate the tapered window of data
-            at the start and end of the onset function which should be
-            disregarded. This is necessary to accurately set the pick threshold
-            in GaussianPicker, for example.
+            If the timespan for which the onsets are being generated is provided, this
+            will be used to calculate the tapered window of data at the start and end of
+            the onset function which should be disregarded. This is necessary to
+            accurately set the pick threshold in GaussianPicker, for example.
 
         Returns
         -------
         onsets : `numpy.ndarray` of float
-            Stacked onset functions served up for migration,
-            shape(nonsets, nsamples).
+            Stacked onset functions served up for migration, shape(nonsets, nsamples).
         onset_data : :class:`~quakemigrate.signal.onsets.base.OnsetData` object
             Light class encapsulating data generated during onset calculation.
 
         """
 
         onsets = []
         onsets_dict = {}
         filtered_waveforms = Stream()
         availability = {}
 
         # Loop through phases, pre-process data, and calculate onsets.
         for phase in self.phases:
             # Select traces based on channel map for this phase
-            phase_waveforms = data.waveforms.select(
-                channel=self.channel_maps[phase])
+            phase_waveforms = data.waveforms.select(channel=self.channel_maps[phase])
 
             # Convert sta window, lta window lengths from seconds to samples.
             stw, ltw = self.sta_lta_windows[phase]
             stw = util.time2sample(stw, self.sampling_rate) + 1
             ltw = util.time2sample(ltw, self.sampling_rate) + 1
 
             # Pre-process the data. The ObsPy functions operate by trace, so
             # will not break on gappy data (we haven't checked availability
             # yet)
             filtered_phase_waveforms = pre_process(
-                phase_waveforms, self.sampling_rate, data.resample,
-                data.upfactor, self.bandpass_filters[phase],
-                data.starttime, data.endtime)
+                phase_waveforms,
+                self.sampling_rate,
+                data.resample,
+                data.upfactor,
+                self.bandpass_filters[phase],
+                data.starttime,
+                data.endtime,
+            )
 
             # Loop through stations, check data availability for this phase,
             # and store this info, filtered waveforms and calculated onsets
             for station in data.stations:
                 waveforms = filtered_phase_waveforms.select(station=station)
 
-                available, av_dict = data.check_availability(waveforms,
+                available, av_dict = data.check_availability(
+                    waveforms,
                     all_channels=self.all_channels,
                     n_channels=self.channel_counts[phase],
                     allow_gaps=self.allow_gaps,
                     full_timespan=self.full_timespan,
                     check_sampling_rate=True,
-                    sampling_rate=self.sampling_rate)
+                    sampling_rate=self.sampling_rate,
+                )
                 availability[f"{station}_{phase}"] = available
 
                 # If no data available, skip
                 if available == 0:
                     logging.info(f"\t\tNo {phase} onset for {station}.")
                     continue
 
@@ -366,60 +362,70 @@
                     waveforms.taper(type="cosine", max_percentage=0.05)
                     # Fill gaps
                     waveforms.merge(method=1, fill_value=tiny)
                     # Pad start/end; delta of +/-0.00001 is to avoid
                     # occasional obspy weirdness. `nearest_sample` is
                     # appropriate as data is at uniform sampling rate with
                     # off-sample data corrected by util.shift_to_sample()
-                    waveforms.trim(starttime=data.starttime-0.00001,
-                                   endtime=data.endtime+0.00001, pad=True,
-                                   fill_value=tiny, nearest_sample=False)
+                    waveforms.trim(
+                        starttime=data.starttime - 0.00001,
+                        endtime=data.endtime + 0.00001,
+                        pad=True,
+                        fill_value=tiny,
+                        nearest_sample=False,
+                    )
 
                 # Calculate onset and add to WaveForm data object; add filtered
                 # waveforms that have passed the availability check to
                 # WaveformData.filtered_waveforms
                 onsets_dict.setdefault(station, {}).update(
-                    {phase: self._onset(waveforms, stw, ltw, log, timespan)})
+                    {phase: self._onset(waveforms, stw, ltw, log, timespan)}
+                )
                 onsets.append(onsets_dict[station][phase])
                 filtered_waveforms += waveforms
 
         logging.debug(filtered_waveforms.__str__(extended=True))
 
         if sum(availability.values()) == 0:
             raise util.DataAvailabilityException
 
         onsets = np.stack(onsets, axis=0)
-        onset_data = OnsetData(onsets_dict, self.phases, self.channel_maps,
-                               filtered_waveforms, availability,
-                               data.starttime, data.endtime,
-                               self.sampling_rate)
+        onset_data = OnsetData(
+            onsets_dict,
+            self.phases,
+            self.channel_maps,
+            filtered_waveforms,
+            availability,
+            data.starttime,
+            data.endtime,
+            self.sampling_rate,
+        )
 
         return onsets, onset_data
 
     def _onset(self, stream, stw, ltw, log, timespan):
         """
-        Generates an onset (characteristic) function. If there are multiple
-        components, these are combined as the root-mean-square of the onset
-        functions AFTER taking a log (if requested).
+        Generates an onset (characteristic) function. If there are multiple components,
+        these are combined as the root-mean-square of the onset functions AFTER taking a
+        log (if requested).
 
         Parameters
         ----------
         stream : `obspy.Stream` object
-            Stream containing the pre-processed data from which to calculate
-            the onset function.
+            Stream containing the pre-processed data from which to calculate the onset
+            function.
         stw : int
             Number of samples in the short-term window.
         ltw : int
             Number of samples in the long-term window.
         log : bool
             Calculate log(onset) if True, otherwise calculate the raw onset.
         timespan : float or None
-            If a timespan is provided it will be used to calculate the tapered
-            window of data at the start and end of the onset function which
-            should be disregarded.
+            If a timespan is provided it will be used to calculate the tapered window of
+            data at the start and end of the onset function which should be disregarded.
 
         Returns
         -------
         onset : `numpy.ndarray` of float
             STA/LTA onset function.
 
         """
@@ -433,54 +439,51 @@
         if timespan:
             onsets = self._trim_taper_pad(onsets, stw, ltw, timespan)
 
         np.clip(1 + onsets, 0.8, np.inf, onsets)
         if log:
             np.log(onsets, onsets)
 
-        onset = np.sqrt(np.sum([onset ** 2 for onset in onsets], axis=0)
-                        / len(onsets))
+        onset = np.sqrt(np.sum([onset**2 for onset in onsets], axis=0) / len(onsets))
 
         return onset
 
     def _trim_taper_pad(self, onsets, stw, ltw, timespan):
         """
-        Set the value of the tapered windows at the start and end of the onset
-        function (plus one long-term window and one short-term window,
-        respectively) to 0.
+        Set the value of the tapered windows at the start and end of the onset function
+        (plus one long-term window and one short-term window, respectively) to 0.
 
         Parameters
         ----------
         onsets : `numpy.ndarray` of float
             STA/LTA onset function.
         stw : int
             Number of samples in the short-term window.
         ltw : int
             Number of samples in the long-term window.
         timespan : float
-            Used to calculate the tapered window of data at the start and end
-            of the onset function which should be disregarded.
+            Used to calculate the tapered window of data at the start and end of the
+            onset function which should be disregarded.
 
         Returns
         -------
         onsets : `numpy.ndarray` of float
-            STA/LTA onset function, with the value in the tapered regions of
-            data set to 0.
+            STA/LTA onset function, with the value in the tapered regions of data set to
+            0.
 
         """
 
         # Calculate duration of taper pre- and post-pad and convert to samples
         pre_pad, _ = self.pad(timespan)
         # Taper pre- and post-pad are identical - just calculate one
-        taper_pad = util.time2sample(pre_pad - self.pre_pad,
-                                     self.sampling_rate)
+        taper_pad = util.time2sample(pre_pad - self.pre_pad, self.sampling_rate)
 
         for onset in onsets:
-            onset[:(taper_pad + ltw - 1)] = 0
-            onset[-(stw + taper_pad):] = 0
+            onset[: (taper_pad + ltw - 1)] = 0
+            onset[-(stw + taper_pad) :] = 0
 
         return onsets
 
     def gaussian_halfwidth(self, phase):
         """
         Return the phase-appropriate Gaussian half-width estimate based on the
         short-term average window length.
@@ -494,40 +497,41 @@
 
         return self.sta_lta_windows[phase][0] * self.sampling_rate / 2
 
     @property
     def pre_pad(self):
         """Pre-pad is determined as a function of the onset windows"""
         windows = self.sta_lta_windows
-        pre_pad = (max([windows[key][1] for key in windows.keys()])
-                   + 3 * max([windows[key][0] for key in windows.keys()]))
+        pre_pad = max([windows[key][1] for key in windows.keys()]) + 3 * max(
+            [windows[key][0] for key in windows.keys()]
+        )
 
         return pre_pad
 
     @pre_pad.setter
     def pre_pad(self, value):
         """Setter for pre-pad"""
 
         self._pre_pad = value
 
     @property
     def post_pad(self):
         """
-        Post-pad is determined as a function of the max traveltime in the
-        grid and the onset windows
+        Post-pad is determined as a function of the max traveltime in the grid and the
+        onset windows
 
         """
 
         return self._post_pad
 
     @post_pad.setter
     def post_pad(self, ttmax):
         """
-        Define post-pad as a function of the maximum travel-time between a
-        station and a grid point plus the LTA (in case onset_centred is True)
+        Define post-pad as a function of the maximum travel-time between a station and a
+        grid point plus the LTA (in case onset_centred is True)
 
         """
         windows = self.sta_lta_windows
         lta_max = max([windows[key][1] for key in windows.keys()])
         self._post_pad = np.ceil(ttmax + 2 * lta_max)
 
     # --- Deprecation/Future handling ---
@@ -540,17 +544,19 @@
     def onset_centred(self, value):
         """
         Handle deprecated onset_centred kwarg / attribute and print warning.
 
         """
         if value is None:
             return
-        print("FutureWarning: Parameter name has changed - continuing.")
-        print("To remove this message, change:")
-        print("\t'onset_centred' -> 'position'")
+        print(
+            "FutureWarning: Parameter name has changed - continuing.\n"
+            "To remove this message, change:\n"
+            "\t'onset_centred' -> 'position'"
+        )
         if value:
             self.position = "centred"
         else:
             self.position = "classic"
 
     @property
     def p_bp_filter(self):
@@ -561,16 +567,18 @@
     def p_bp_filter(self, value):
         """
         Handle deprecated p_bp_filter kwarg / attribute and print warning.
 
         """
         if value is None:
             return
-        print("FutureWarning: Parameter name has changed - continuing.")
-        print("To remove this message, refer to the documentation.")
+        print(
+            "FutureWarning: Parameter name has changed - continuing.\n"
+            "To remove this message, refer to the documentation."
+        )
 
         self.bandpass_filters["P"] = value
 
     @property
     def s_bp_filter(self):
         """Handle deprecated s_bp_filter kwarg / attribute"""
         return self.bandpass_filters["S"]
@@ -579,16 +587,18 @@
     def s_bp_filter(self, value):
         """
         Handle deprecated s_bp_filter kwarg / attribute and print warning.
 
         """
         if value is None:
             return
-        print("FutureWarning: Parameter name has changed - continuing.")
-        print("To remove this message, refer to the documentation.")
+        print(
+            "FutureWarning: Parameter name has changed - continuing.\n"
+            "To remove this message, refer to the documentation."
+        )
 
         self.bandpass_filters["S"] = value
 
     @property
     def p_onset_win(self):
         """Handle deprecated p_onset_win kwarg / attribute"""
         return self.sta_lta_windows["P"]
@@ -597,16 +607,18 @@
     def p_onset_win(self, value):
         """
         Handle deprecated p_onset_win kwarg / attribute and print warning.
 
         """
         if value is None:
             return
-        print("FutureWarning: Parameter name has changed - continuing.")
-        print("To remove this message, refer to the documentation.")
+        print(
+            "FutureWarning: Parameter name has changed - continuing.\n"
+            "To remove this message, refer to the documentation."
+        )
 
         self.sta_lta_windows["P"] = value
 
     @property
     def s_onset_win(self):
         """Handle deprecated s_onset_win kwarg / attribute"""
         return self.sta_lta_windows["S"]
@@ -615,16 +627,18 @@
     def s_onset_win(self, value):
         """
         Handle deprecated s_onset_win kwarg / attribute and print warning.
 
         """
         if value is None:
             return
-        print("FutureWarning: Parameter name has changed - continuing.")
-        print("To remove this message, refer to the documentation.")
+        print(
+            "FutureWarning: Parameter name has changed - continuing.\n"
+            "To remove this message, refer to the documentation."
+        )
 
         self.sta_lta_windows["S"] = value
 
 
 class CentredSTALTAOnset(STALTAOnset):
     """
     QuakeMigrate default onset function class - uses a centred STA/LTA onset.
@@ -634,18 +648,20 @@
     """
 
     def __init__(self, **kwargs):
         """Instantiate CentredSTALTAOnset object."""
 
         super().__init__(**kwargs)
 
-        print("FutureWarning: This class has been deprecated - continuing.")
-        print("To remove this message:")
-        print("\tCentredSTALTAOnset -> STALTAOnset\n")
-        print("\tAnd add keyword argument 'position=centred'")
+        print(
+            "FutureWarning: This class has been deprecated - continuing.\n"
+            "To remove this message:\n"
+            "\tCentredSTALTAOnset -> STALTAOnset\n"
+            "\tAnd add keyword argument 'position=centred'\n"
+        )
         self.position = "centred"
 
 
 class ClassicSTALTAOnset(STALTAOnset):
     """
     QuakeMigrate default onset function class - uses a classic STA/LTA onset.
 
@@ -654,12 +670,14 @@
     """
 
     def __init__(self, **kwargs):
         """Instantiate ClassicSTALTAOnset object."""
 
         super().__init__(**kwargs)
 
-        print("FutureWarning: This class has been deprecated - continuing.")
-        print("To remove this message:")
-        print("\tClassicSTALTAOnset -> STALTAOnset")
-        print("\tAnd add keyword argument 'position=classic'\n")
+        print(
+            "FutureWarning: This class has been deprecated - continuing.\n"
+            "To remove this message:\n"
+            "\tClassicSTALTAOnset -> STALTAOnset\n"
+            "\tAnd add keyword argument 'position=classic'\n"
+        )
         self.position = "classic"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quakemigrate-1.0.1/quakemigrate/signal/pickers/base.py` & `quakemigrate-1.0.2/quakemigrate/signal/pickers/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # -*- coding: utf-8 -*-
 """
 A simple abstract base class with method stubs enabling simple modification of
-QuakeMigrate to use custom phase picking methods that remain compatible with
-the core of the package.
+QuakeMigrate to use custom phase picking methods that remain compatible with the core of
+the package.
 
 :copyright:
-    2020 - 2021, QuakeMigrate developers.
+    2020–2023, QuakeMigrate developers.
 :license:
     GNU General Public License, Version 3
     (https://www.gnu.org/licenses/gpl-3.0.html)
 
 """
 
 from abc import ABC, abstractmethod
 
 
 class PhasePicker(ABC):
     """
-    Abstract base class providing a simple way of modifying the default
-    picking function in QuakeMigrate.
+    Abstract base class providing a simple way of modifying the default picking function
+    in QuakeMigrate.
 
     Attributes
     ----------
     plot_picks : bool
         Toggle plotting of phase picks.
 
     Methods
@@ -38,17 +38,19 @@
 
     def __init__(self, **kwargs):
         """Instantiate the PhasePicker object."""
         self.plot_picks = kwargs.get("plot_picks", True)
 
     def __str__(self):
         """Returns a short summary string of the PhasePicker object."""
-        return ("Abstract PhasePicker object - consider adding a __repr__ "
-                "method to your custom PhasePicker class that gives the user "
-                "relevant information about the object.")
+        return (
+            "Abstract PhasePicker object - consider adding a __repr__ "
+            "method to your custom PhasePicker class that gives the user "
+            "relevant information about the object."
+        )
 
     @abstractmethod
     def pick_phases(self):
         """Method stub for phase picking."""
         pass
 
     def write(self, run, event_uid, phase_picks):
@@ -74,18 +76,21 @@
         fpath.mkdir(exist_ok=True, parents=True)
 
         # Work on a copy
         phase_picks = phase_picks.copy()
 
         # Set floating point precision for output file
         for col in ["PickError", "SNR"]:
-            phase_picks[col] = phase_picks[col].map(lambda x: f"{x:.3g}",
-                                                    na_action="ignore")
+            phase_picks[col] = phase_picks[col].map(
+                lambda x: f"{x:.3g}", na_action="ignore"
+            )
 
         fstem = f"{event_uid}"
         fname = (fpath / fstem).with_suffix(".picks")
         phase_picks.to_csv(fname, index=False)
 
     def plot(self):
         """Method stub for phase pick plotting."""
-        print(("Consider adding a plot method to your custom PhasePicker"
-               " class - see the GaussianPicker class for reference."))
+        print(
+            "Consider adding a plot method to your custom PhasePicker"
+            " class - see the GaussianPicker class for reference."
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quakemigrate-1.0.1/quakemigrate/signal/pickers/gaussian.py` & `quakemigrate-1.0.2/quakemigrate/signal/pickers/gaussian.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """
-The default seismic phase picking class - fits a 1-D Gaussian to the calculated
-onset functions.
+The default seismic phase picking class - fits a 1-D Gaussian to the calculated onset
+functions.
 
 :copyright:
-    2020 - 2021, QuakeMigrate developers.
+    2020–2023, QuakeMigrate developers.
 :license:
     GNU General Public License, Version 3
     (https://www.gnu.org/licenses/gpl-3.0.html)
 
 """
 
 import logging
@@ -22,111 +22,107 @@
 import quakemigrate.util as util
 from .base import PhasePicker
 
 
 class GaussianPicker(PhasePicker):
     """
     This class details the default method of making phase picks shipped with
-    QuakeMigrate, namely fitting a 1-D Gaussian function to the onset function
-    for each station and phase.
+    QuakeMigrate, namely fitting a 1-D Gaussian function to the onset function for each
+    station and phase.
 
     Attributes
     ----------
     phase_picks : dict
             "GAU_P" : array-like
                 Numpy array stack of Gaussian pick info (each as a dict)
                 for P phase
             "GAU_S" : array-like
                 Numpy array stack of Gaussian pick info (each as a dict)
                 for S phase
     threshold_method : {"MAD", "percentile"}
-        Which method to use to calculate the pick threshold; a percentile of
-        the data outside the pick windows (e.g. 0.99 = 99th percentile) or a
-        multiple of the Median Absolute Deviation of the signal outside the
-        pick windows. Default uses the MAD method.
+        Which method to use to calculate the pick threshold; a percentile of the data
+        outside the pick windows (e.g. 0.99 = 99th percentile) or a multiple of the
+        Median Absolute Deviation of the signal outside the pick windows. Default uses
+        the MAD method.
     percentile_pick_threshold : float, optional
-        Picks will only be made if the onset function exceeds this percentile
-        of the noise level (amplitude of onset function outside pick
-        windows). (Default: 1.0)
+        Picks will only be made if the onset function exceeds this percentile of the
+        noise level (amplitude of onset function outside pick windows). (Default: 1.0)
     mad_pick_threshold : float, optional
-        Picks will only be made if the onset function exceeds its median value
-        plus this multiple of the MAD (calculated from the onset data outside
-        the pick windows). (Default: 8)
+        Picks will only be made if the onset function exceeds its median value plus this
+        multiple of the MAD (calculated from the onset data outside the pick windows).
+        (Default: 8)
     plot_picks : bool
         Toggle plotting of phase picks.
 
     Methods
     -------
     pick_phases(event, lut, run)
-        Picks phase arrival times for located events by fitting a 1-D
-        Gaussian function to the P and/or S onset functions
+        Picks phase arrival times for located events by fitting a 1-D Gaussian function
+        to the P and/or S onset functions
 
     """
 
-    DEFAULT_GAUSSIAN_FIT = {"popt": 0,
-                            "xdata": 0,
-                            "xdata_dt": 0,
-                            "PickValue": -1}
+    DEFAULT_GAUSSIAN_FIT = {"popt": 0, "xdata": 0, "xdata_dt": 0, "PickValue": -1}
 
     def __init__(self, onset=None, **kwargs):
         """Instantiate the GaussianPicker object."""
         super().__init__(**kwargs)
 
         self.onset = onset
 
         # --- Get pick method and threshold ---
         self.threshold_method = kwargs.get("threshold_method", "MAD")
         if self.threshold_method == "percentile":
-            self.percentile_pick_threshold = \
-                kwargs.get("percentile_pick_threshold", 1.0)
+            self.percentile_pick_threshold = kwargs.get(
+                "percentile_pick_threshold", 1.0
+            )
         elif self.threshold_method == "MAD":
             self.mad_pick_threshold = kwargs.get("mad_pick_threshold", 8.0)
         else:
             raise util.InvalidPickThresholdMethodException
         # Handle deprecated `pick_threshold`
         if kwargs.get("pick_threshold"):
             self.pick_threshold = kwargs["pick_threshold"]
 
         self.plot_picks = kwargs.get("plot_picks", False)
 
         if "fraction_tt" in kwargs.keys():
-            print("FutureWarning: Fraction of traveltime argument moved to "
-                  "lookup tables.\nIt remains possible to override the "
-                  "fraction of traveltime here, if required, to further\ntune"
-                  "the phase picker.")
+            print(
+                "FutureWarning: Fraction of traveltime argument moved to lookup tables."
+                "\nIt remains possible to override the fraction of traveltime here, if "
+                "required, to further\ntune the phase picker."
+            )
         self._fraction_tt = kwargs.get("fraction_tt")
 
     def __str__(self):
         """Returns a short summary string of the GaussianPicker."""
 
         str_ = "\tPhase picking by fitting a 1-D Gaussian to onsets\n"
         if self.threshold_method == "percentile":
-            str_ += ("\t\tPercentile threshold  = "
-                     f"{self.percentile_pick_threshold}\n")
+            str_ += f"\t\tPercentile threshold  = {self.percentile_pick_threshold}\n"
         elif self.threshold_method == "MAD":
             str_ += f"\t\tMAD multiplier  = {self.mad_pick_threshold}\n"
         if self._fraction_tt is not None:
-            str_ += (f"\t\tSearch window   = {self._fraction_tt*100}% of "
-                     "traveltime\n")
+            str_ += f"\t\tSearch window   = {self._fraction_tt*100}% of traveltime\n"
 
         return str_
 
     @util.timeit("info")
     def pick_phases(self, event, lut, run):
         """
         Picks phase arrival times for located events.
 
         Parameters
         ----------
         event : :class:`~quakemigrate.io.event.Event` object
-            Light class encapsulating waveforms, coalescence information and
-            location information for a given event.
+            Light class encapsulating waveforms, coalescence information and location
+            information for a given event.
         lut : :class:`~quakemigrate.lut.lut.LUT` object
-            Contains the traveltime lookup tables for seismic phases, computed
-            for some pre-defined velocity model.
+            Contains the traveltime lookup tables for seismic phases, computed for some
+            pre-defined velocity model.
         run : :class:`~quakemigrate.io.core.Run` object
             Light class encapsulating i/o path information for a given run.
 
         Returns
         -------
         event : :class:`~quakemigrate.io.event.Event` object
             Event object provided to pick_phases(), but now with phase picks!
@@ -134,55 +130,73 @@
             DataFrame that contains the measured picks with columns:
             ["Name", "Phase", "ModelledTime", "PickTime", "PickError", "SNR"]
             Each row contains the phase pick from one station/phase.
 
         """
 
         # Onsets are recalculated without logging
-        _, onset_data = self.onset.calculate_onsets(event.data, log=False,
-            timespan=4*event.marginal_window)
+        _, onset_data = self.onset.calculate_onsets(
+            event.data, log=False, timespan=4 * event.marginal_window
+        )
 
         if self._fraction_tt is None:
             fraction_tt = lut.fraction_tt
         else:
             fraction_tt = self._fraction_tt
 
         e_ijk = lut.index2coord(event.hypocentre, inverse=True)[0]
 
         # Pre-define pick DataFrame and fit params and pick windows dicts
         p_idx = np.arange(sum([len(v) for _, v in onset_data.onsets.items()]))
-        picks = pd.DataFrame(index=p_idx,
-                             columns=["Station", "Phase", "ModelledTime",
-                                      "PickTime", "PickError", "SNR"])
+        picks = pd.DataFrame(
+            index=p_idx,
+            columns=[
+                "Station",
+                "Phase",
+                "ModelledTime",
+                "PickTime",
+                "PickError",
+                "SNR",
+            ],
+        )
         gaussfits = {}
         pick_windows = {}
         idx = 0
 
         for station, onsets in onset_data.onsets.items():
             for phase, onset in onsets.items():
                 traveltime = lut.traveltime_to(phase, e_ijk, station)[0]
                 pick_windows.setdefault(station, {}).update(
-                    {phase: self._determine_window(
-                        event, onset_data, traveltime, fraction_tt)})
+                    {
+                        phase: self._determine_window(
+                            event, onset_data, traveltime, fraction_tt
+                        )
+                    }
+                )
                 n_samples = len(onset)
 
             self._distinguish_windows(
-                pick_windows[station], list(onsets.keys()), n_samples)
+                pick_windows[station], list(onsets.keys()), n_samples
+            )
 
             for phase, onset in onsets.items():
                 # Find threshold from 'noise' part of onset
                 pick_threshold = self._find_pick_threshold(
-                    onset, pick_windows[station], self.threshold_method)
+                    onset, pick_windows[station], self.threshold_method
+                )
 
                 logging.debug(f"\t\tPicking {phase} at {station}...")
                 fit, *pick = self._fit_gaussian(
-                    onset, onset_data.sampling_rate,
+                    onset,
+                    onset_data.sampling_rate,
                     self.onset.gaussian_halfwidth(phase),
-                    onset_data.starttime, pick_threshold,
-                    pick_windows[station][phase])
+                    onset_data.starttime,
+                    pick_threshold,
+                    pick_windows[station][phase],
+                )
 
                 gaussfits.setdefault(station, {}).update({phase: fit})
 
                 traveltime = lut.traveltime_to(phase, e_ijk, station)[0]
                 model_time = event.otime + traveltime
                 picks.iloc[idx] = [station, phase, model_time, *pick]
                 idx += 1
@@ -190,65 +204,69 @@
         event.add_picks(picks, gaussfits=gaussfits, pick_windows=pick_windows)
 
         self.write(run, event.uid, picks)
 
         if self.plot_picks:
             logging.info("\t\tPlotting picks...")
             for station, onsets in onset_data.onsets.items():
-                traveltimes = [lut.traveltime_to(phase, e_ijk, station)[0]
-                               for phase in onsets.keys()]
+                traveltimes = [
+                    lut.traveltime_to(phase, e_ijk, station)[0]
+                    for phase in onsets.keys()
+                ]
                 self.plot(event, station, onset_data, picks, traveltimes, run)
 
         return event, picks
 
     def _determine_window(self, event, onset_data, tt, fraction_tt):
         """
-        Determine phase pick window upper and lower bounds based on the event
-        marginal window and a set percentage of the phase travel time.
+        Determine phase pick window upper and lower bounds based on the event marginal
+        window and a set percentage of the phase travel time.
 
         Parameters
         ----------
         event : :class:`~quakemigrate.io.event.Event` object
-            Light class to encapsulate information about an event, including
-            origin time, location and waveform data.
+            Light class to encapsulate information about an event, including origin
+            time, location and waveform data.
         onset_data : :class:`~quakemigrate.signal.onsets.base.OnsetData` object
             Light class encapsulating data generated during onset calculation.
         tt : float
             Traveltime for the requested phase.
         fraction_tt : float
-            Defines width of time window around expected phase arrival time in
-            which to search for a phase pick as a function of the traveltime
-            from the event location to that station -- should be an estimate of
-            the uncertainty in the velocity model.
+            Defines width of time window around expected phase arrival time in which to
+            search for a phase pick as a function of the traveltime from the event
+            location to that station -- should be an estimate of the uncertainty in the
+            velocity model.
 
         Returns
         -------
         lower_idx : int
             Index of lower bound for the phase pick window.
         arrival_idx : int
             Index of the modelled phase arrival time.
         upper_idx : int
             Index of upper bound for the phase pick window.
 
         """
 
-        arrival_idx = util.time2sample(event.otime + tt - onset_data.starttime,
-                                       onset_data.sampling_rate)
+        arrival_idx = util.time2sample(
+            event.otime + tt - onset_data.starttime, onset_data.sampling_rate
+        )
 
         # Add length of marginal window to this and convert to index
-        samples = util.time2sample(tt * fraction_tt + event.marginal_window,
-                                   onset_data.sampling_rate)
+        samples = util.time2sample(
+            tt * fraction_tt + event.marginal_window, onset_data.sampling_rate
+        )
 
         return [arrival_idx - samples, arrival_idx, arrival_idx + samples]
 
     def _distinguish_windows(self, windows, phases, samples):
         """
-        Ensure pick windows do not overlap - if they do, set the upper bound of
-        window one and the lower bound of window two to be the midpoint index
-        of the two modelled phase arrival times.
+        Ensure pick windows do not overlap - if they do, set the upper bound of window
+        one and the lower bound of window two to be the midpoint index of the two
+        modelled phase arrival times.
 
         Parameters
         ----------
         windows : dict
             Dictionary of windows with phases as keys.
         phases : list of str
             Phases being migrated.
@@ -270,80 +288,79 @@
 
         # Handle last key
         last_idx = windows[phases[-1]][2]
         windows[phases[-1]][2] = samples if last_idx > samples else last_idx
 
     def _find_pick_threshold(self, onset, windows, method):
         """
-        Determine a pick threshold from the onset data outside the pick
-        windows.
+        Determine a pick threshold from the onset data outside the pick windows.
 
         Parameters
         ----------
         onset : `numpy.ndarray` of `numpy.double`
             Onset (characteristic) function.
         windows : list of int
-            Indexes of the lower window bound, the phase arrival, and the upper
-            window bound.
+            Indexes of the lower window bound, the phase arrival, and the upper window
+            bound.
         method : {"percentile", "MAD"}
             Method used to calculate the pick threshold from the noise data.
 
         Return
         ------
         pick_threshold : float
-            The threshold calculated from the onset data outside the pick
-            windows, according to the specified `method`.
+            The threshold calculated from the onset data outside the pick windows,
+            according to the specified `method`.
 
         """
 
         onset_noise = onset.copy()
         for _, window in windows.items():
-            onset_noise[window[0]:window[2]] = -1
-        # Remove data during pick windows, and data set to 1 (in onset function
-        # taper pad windows)
+            onset_noise[window[0] : window[2]] = -1
+        # Remove data during pick windows, and data set to 1 (in onset function taper
+        # pad windows)
         onset_noise = onset_noise[onset_noise > 1]
 
         if method == "percentile":
-            pick_threshold = \
-                np.percentile(onset_noise, self.percentile_pick_threshold * 100)
+            pick_threshold = np.percentile(
+                onset_noise, self.percentile_pick_threshold * 100
+            )
         elif method == "MAD":
             med = np.median(onset_noise)
             mad = util.calculate_mad(onset_noise)
             pick_threshold = med + (mad * self.mad_pick_threshold)
 
         return pick_threshold
 
-    def _fit_gaussian(self, onset, sampling_rate, halfwidth, starttime,
-                      pick_threshold, window):
-        """
-        Fit a Gaussian to the onset function in order to make a time pick with
-        an associated uncertainty.
-
-        Uses the amplitude and timing of the onset function peak and some
-        knowledge of the onset function parameters (e.g. short-term average
-        window length, for the
-        :class:`~quakemigrate.signal.onsets.stalta.STALTAOnset`) to make an
-        initial estimate of a gaussian fit to the onset function.
+    def _fit_gaussian(
+        self, onset, sampling_rate, halfwidth, starttime, pick_threshold, window
+    ):
+        """
+        Fit a Gaussian to the onset function in order to make a time pick with an
+        associated uncertainty.
+
+        Uses the amplitude and timing of the onset function peak and some knowledge of
+        the onset function parameters (e.g. short-term average window length, for the
+        :class:`~quakemigrate.signal.onsets.stalta.STALTAOnset`) to make an initial
+        estimate of a gaussian fit to the onset function.
 
         Parameters
         ----------
         onset : `numpy.ndarray` of `numpy.double`
             Onset function.
         sampling_rate : int
             Sampling rate of the onset function.
         halfwidth : float
-            Initial estimate for the Gaussian half-width based on some function
-            of the onset function parameters.
+            Initial estimate for the Gaussian half-width based on some function of the
+            onset function parameters.
         starttime : `obspy.UTCDateTime` object
             Timestamp for first sample of the onset function.
         pick_threshold : float
             Value above which to threshold data based on noise.
         window : list of int, [start, arrival, end]
-            Indices for the window start, modelled phase arrival, and window
-            end.
+            Indices for the window start, modelled phase arrival, and window end.
 
         Returns
         -------
         gaussian_fit : dictionary
             Gaussian fit parameters: {"popt": popt,
                                       "xdata": x_data,
                                       "xdata_dt": x_data_dt,
@@ -355,92 +372,95 @@
             Sigma of Gaussian fit to onset function, i.e. the pick uncertainty.
         mean : `obspy.UTCDateTime`
             Mean of Gaussian fit to onset function, i.e. the pick time.
 
         """
 
         # Trim the onset function in the pick window
-        onset_signal = onset[window[0]:window[2]]
+        onset_signal = onset[window[0] : window[2]]
         logging.debug(f"\t\t    win_min: {window[0]}, win_max: {window[2]}")
 
         # Identify the peak in the windowed onset that exceeds this threshold
         # AND contains the maximum value in the window (i.e. the 'true' peak).
         try:
             peak_idxs = self._find_peak(onset_signal, pick_threshold)
-            # add an extra sample either side for the curve fitting. This makes
-            # the fitting more stable, and guarantees at least 3 samples -->
-            # avoids an under-constrained optimisation (3 fitting params).
+            # add an extra sample either side for the curve fitting. This makes the
+            # fitting more stable, and guarantees at least 3 samples --> avoids an
+            # under-constrained optimisation (3 fitting params).
             padded_peak_idxs = [peak_idxs[0] - 1, peak_idxs[1] + 1]
             padded_peak_idxs = [window[0] + p for p in padded_peak_idxs]
-            logging.debug(f"\t\t    padded_peak_idxmin: {padded_peak_idxs[0]},"
-                          f" padded_peak_idxmax: {padded_peak_idxs[1]}")
+            logging.debug(
+                f"\t\t    padded_peak_idxmin: {padded_peak_idxs[0]},"
+                f" padded_peak_idxmax: {padded_peak_idxs[1]}"
+            )
             x_data = np.arange(*padded_peak_idxs) / sampling_rate
-            y_data = onset[padded_peak_idxs[0]:padded_peak_idxs[1]]
+            y_data = onset[padded_peak_idxs[0] : padded_peak_idxs[1]]
         except util.NoOnsetPeak as e:
             logging.debug(e.msg)
             return self._pick_failure(pick_threshold)
 
         # Try to fit a 1-D Gaussian
         # Initial parameters (p0) are:
         #   height = max value of onset function
         #   mean   = time of max value
         #   sigma  = `halfwidth` - determined from onset function parameters
-        p0 = [max(y_data),
-              (padded_peak_idxs[0] + \
-              np.argmax(y_data)) / sampling_rate,
-              halfwidth / sampling_rate]
+        p0 = [
+            max(y_data),
+            (padded_peak_idxs[0] + np.argmax(y_data)) / sampling_rate,
+            halfwidth / sampling_rate,
+        ]
         try:
             popt, _ = curve_fit(util.gaussian_1d, x_data, y_data, p0)
         except (ValueError, RuntimeError) as e:
-            # curve_fit can fail for a number of reasons - primarily if the
-            # input data contains nans or if the least-squares minimisation
-            # fails. A warning may also be emitted to stdout if the covariance
-            # of the parameters could not be estimated - this is suppressed by
-            # default in scan.py.
-            logging.debug(f"\t\t    Failed curve_fit:\n{e}\n\t\t    "
-                          "Continuing...")
+            # curve_fit can fail for a number of reasons - primarily if the input data
+            # contains nans or if the least-squares minimisation fails. A warning may
+            # also be emitted to stdout if the covariance of the parameters could not
+            # be estimated - this is suppressed by default in scan.py.
+            logging.debug(f"\t\t    Failed curve_fit:\n{e}\n\t\t    Continuing...")
             return self._pick_failure(pick_threshold)
         except TypeError as e:
-            logging.debug("\t\t    Failed curve_fit - too few input data?"
-                          f"{e}\n\t\t    Continuing...")
+            logging.debug(
+                "\t\t    Failed curve_fit - too few input data?"
+                f"{e}\n\t\t    Continuing..."
+            )
 
         # Unpack results:
         #  popt = [height, mean (seconds), sigma (seconds)]
         max_onset = popt[0]
         mean = starttime + float(popt[1])
         sigma = np.absolute(popt[2])
 
         # Check pick mean is within the pick window.
         if not window[0] < popt[1] * sampling_rate < window[2]:
             logging.debug("\t\t    Pick mean out of bounds - continuing.")
             return self._pick_failure(pick_threshold)
 
-        gaussian_fit = {"popt": popt,
-                        "xdata": x_data,
-                        "xdata_dt": np.array([starttime + x for x in x_data]),
-                        "PickValue": max_onset,
-                        "PickThreshold": pick_threshold}
+        gaussian_fit = {
+            "popt": popt,
+            "xdata": x_data,
+            "xdata_dt": np.array([starttime + x for x in x_data]),
+            "PickValue": max_onset,
+            "PickThreshold": pick_threshold,
+        }
 
         return gaussian_fit, mean, sigma, max_onset
 
     def _pick_failure(self, pick_threshold):
         """
-        Short utility function to produce the default values when a pick cannot
-        be made.
+        Short utility function to produce the default values when a pick cannot be made.
 
         Parameters
         ----------
         pick_threshold : float
             Pick threshold value for onset data.
 
         Returns
         -------
         gaussian_fit : dictionary
-            The default Gaussian fit dictionary, with relevant pick threshold
-            value.
+            The default Gaussian fit dictionary, with relevant pick threshold value.
         max_onset : int
             A default of -1 value to indicate failure.
         sigma : int
             A default of -1 value to indicate failure.
         mean : int
             A default of -1 value to indicate failure.
 
@@ -450,18 +470,17 @@
         gaussian_fit["PickThreshold"] = pick_threshold
         mean = sigma = max_onset = -1
 
         return gaussian_fit, mean, sigma, max_onset
 
     def _find_peak(self, windowed_onset, pick_threshold):
         """
-        Identify peaks, if any, within the windowed onset that exceed the
-        specified threshold value. Of those peaks, this function seeks the one
-        that contains the maximum value within the window, i.e. the 'true'
-        peak - see the diagram below.
+        Identify peaks, if any, within the windowed onset that exceed the specified
+        threshold value. Of those peaks, this function seeks the one that contains the
+        maximum value within the window, i.e. the 'true' peak - see the diagram below.
 
                                              v
                                              *
                                             * *
                                     *      *   *
                          |         * *    *     *     |
                          |---------------#-------#----|
@@ -473,77 +492,76 @@
             The onset function within the picking window.
         pick_threshold : float
             Value above which to search for peaks in the onset data.
 
         Returns
         -------
         true_peak_idx : [int, int]
-            Start and end index values for the 'true' peak, with +1 added to
-            the last index so that all of the values above the threshold are
-            returned when slicing by index.
+            Start and end index values for the 'true' peak, with +1 added to the last
+            index so that all of the values above the threshold are returned when
+            slicing by index.
 
         Raises
         ------
         util.NoOnsetPeak
-            If no onset data, or only a single sample, exceeds the pick
-            threshold.
+            If no onset data, or only a single sample, exceeds the pick threshold.
 
         """
 
         exceedence = np.where(windowed_onset > pick_threshold)[0]
         if len(exceedence) == 0:
             raise util.NoOnsetPeak(pick_threshold)
 
-        # Identify all peaks - there are possibly multiple distinct periods
-        # of data that exceed the threshold. The following command simply seeks
-        # non-consecutive index values in the array of points that exceed
-        # the threshold and splits the array at these points into 'peaks'.
+        # Identify all peaks - there are possibly multiple distinct periods of data that
+        # exceed the threshold. The following command simply seeks non-consecutive index
+        # values in the array of points that exceed the threshold and splits the array
+        # at these points into 'peaks'.
         peaks = np.split(exceedence, np.where(np.diff(exceedence) != 1)[0] + 1)
 
         # Identify the peak that contains the true peak (maximum)
         true_maximum = np.argmax(windowed_onset)
         for i, peak in enumerate(peaks):
             if np.any(peak == true_maximum):
                 break
 
         # Check if there is more than a single sample above the threshold
         if len(peaks[i]) < 2:
             raise util.NoOnsetPeak(pick_threshold)
 
-        # Grab the peak and return the start/end index values. NOTE: + 1 is
-        # required so that the last sample is included when slicing by index
+        # Grab the peak and return the start/end index values. NOTE: + 1 is required so
+        # that the last sample is included when slicing by index
         true_peak_idxs = [peaks[i][0], peaks[i][-1] + 1]
 
         return true_peak_idxs
 
     @util.timeit()
     def plot(self, event, station, onset_data, picks_df, traveltimes, run):
         """
-        Plot figure showing the filtered traces for each data component and the
-        onset functions calculated from them (P and/or S) for each station. The
-        search window to make a phase pick is displayed, along with the dynamic
-        pick threshold, the phase pick time and its uncertainty (if made) and
-        the Gaussian fit to the onset function.
+        Plot figure showing the filtered traces for each data component and the onset
+        functions calculated from them (P and/or S) for each station. The search window
+        to make a phase pick is displayed, along with the dynamic pick threshold, the
+        phase pick time and its uncertainty (if made) and the Gaussian fit to the onset
+        function.
 
         Parameters
         ----------
         event : :class:`~quakemigrate.io.event.Event` object
-            Light class to encapsulate information about an event, including
-            origin time, location and waveform data.
+            Light class to encapsulate information about an event, including origin
+            time, location and waveform data.
         station : str
             Station name.
         onset_data : :class:`~quakemigrate.signal.onsets.base.OnsetData` object
             Light class encapsulating data generated during onset calculation.
         picks_df : `pandas.DataFrame` object
             DataFrame that contains the measured picks with columns:
             ["Name", "Phase", "ModelledTime", "PickTime", "PickError", "SNR"]
             Each row contains the phase pick from one station/phase.
         traveltimes : list of float
-            Modelled traveltimes from the event hypocentre to the station
-            for each phase to be plotted.
+            Modelled traveltimes from the event hypocentre to the station for each phase
+            to be plotted.
         run : :class:`~quakemigrate.io.core.Run` object
             Light class encapsulating i/o path information for a given run.
 
         """
 
         fpath = run.path / f"locate/{run.subname}/pick_plots/{event.uid}"
         fpath.mkdir(exist_ok=True, parents=True)
@@ -553,36 +571,40 @@
         # Check if any data available to plot
         if not bool(waveforms):
             return
         picks = picks_df[picks_df["Station"] == station].reset_index(drop=True)
         windows = event.picks["pick_windows"][station]
 
         # Call subroutine to plot phase pick figure
-        fig = pick_summary(event, station, waveforms, picks, onsets,
-                           traveltimes, windows)
+        fig = pick_summary(
+            event, station, waveforms, picks, onsets, traveltimes, windows
+        )
 
         fstem = f"{event.uid}_{station}"
         file = (fpath / fstem).with_suffix(".pdf")
         plt.savefig(file)
         plt.close(fig)
 
     @property
     def fraction_tt(self):
         """Handler for deprecated attribute 'fraction_tt'"""
         return self._fraction_tt
 
     @fraction_tt.setter
     def fraction_tt(self, value):
-        print("FutureWarning: Fraction of traveltime attribute has moved to "
-              "lookup table.\n Overriding...")
+        print(
+            "FutureWarning: Fraction of traveltime attribute has moved to lookup table."
+            "\nOverriding..."
+        )
         self._fraction_tt = value
 
     @property
     def pick_threshold(self):
         """Handler for deprecated attribute 'pick_threshold'"""
 
     @pick_threshold.setter
     def pick_threshold(self, value):
-        raise AttributeError("The 'pick_threshold' attribute has been "
-                             "deprecated. Select a threshold method from "
-                             "'percentile' or 'MAD', and see the docs for "
-                             "the syntax for the appropriate threshold.")
+        raise AttributeError(
+            "The 'pick_threshold' attribute has been deprecated. Select a threshold "
+            "method from 'percentile' or 'MAD', and see the docs for the syntax for "
+            "the appropriate threshold."
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quakemigrate-1.0.1/quakemigrate/signal/scan.py` & `quakemigrate-1.0.2/quakemigrate/signal/scan.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 Module to perform core QuakeMigrate functions: detect() and locate().
 
 :copyright:
-    2020 - 2021, QuakeMigrate developers.
+    2020–2023, QuakeMigrate developers.
 :license:
     GNU General Public License, Version 3
     (https://www.gnu.org/licenses/gpl-3.0.html)
 
 """
 
 import logging
@@ -17,177 +17,175 @@
 from obspy import UTCDateTime
 import pandas as pd
 from scipy.interpolate import Rbf
 from scipy.signal import fftconvolve
 
 import quakemigrate.util as util
 from quakemigrate.core import find_max_coa, migrate
-from quakemigrate.io import (Event, Run, ScanmSEED, read_triggered_events,
-                             write_availability, write_cut_waveforms)
+from quakemigrate.io import (
+    Event,
+    Run,
+    ScanmSEED,
+    read_triggered_events,
+    write_availability,
+    write_cut_waveforms,
+)
 from quakemigrate.plot.event import event_summary
 from .onsets import Onset
 from .pickers import GaussianPicker, PhasePicker
 from .local_mag import LocalMag
 
 # Filter warnings
-warnings.filterwarnings("ignore", message=("Covariance of the parameters could"
-                                           " not be estimated"))
+warnings.filterwarnings(
+    "ignore", message=("Covariance of the parameters could not be estimated")
+)
 
 
 class QuakeScan:
     """
     QuakeMigrate scanning class.
 
-    Provides an interface for the wrapped compiled C functions, used to perform
-    the continuous scan (detect) or refined event migrations (locate).
+    Provides an interface for the wrapped compiled C functions, used to perform the
+    continuous scan (detect) or refined event migrations (locate).
 
     Parameters
     ----------
     archive : :class:`~quakemigrate.io.data.Archive` object
-        Details the structure and location of a data archive and provides
-        methods for reading data from file.
+        Details the structure and location of a data archive and provides methods for
+        reading data from file.
     lut : :class:`~quakemigrate.lut.lut.LUT` object
-        Contains the traveltime lookup tables for seismic phases, computed for
-        some pre-defined velocity model.
+        Contains the traveltime lookup tables for seismic phases, computed for some
+        pre-defined velocity model.
     onset : :class:`~quakemigrate.signal.onsets.base.Onset` object
         Provides callback methods for calculation of onset functions.
     run_path : str
-        Points to the top level directory containing all input files, under
-        which the specific run directory will be created.
+        Points to the top level directory containing all input files, under which the
+        specific run directory will be created.
     run_name : str
         Name of the current QuakeMigrate run.
     kwargs : **dict
         See QuakeScan Attributes for details. In addition to these:
 
     Attributes
     ----------
     continuous_scanmseed_write : bool
-        Option to continuously write the .scanmseed file output by detect() at
-        the end of every time step. Default behaviour is to write in day chunks
-        where possible. Default: False.
+        Option to continuously write the .scanmseed file output by detect() at the end
+        of every time step. Default behaviour is to write in day chunks where possible.
+        Default: False.
     cut_waveform_format : str, optional
         File format used when writing waveform data. We support any format also
-        supported by ObSpy - "MSEED" (default), "SAC", "SEGY", "GSE2".
+        supported by ObsPy - "MSEED" (default), "SAC", "SEGY", "GSE2".
     log : bool, optional
-        Toggle for logging. If True, will output to stdout and generate a
-        log file. Default is to only output to stdout.
+        Toggle for logging. If True, will output to stdout and generate a log file.
+        Default is to only output to stdout.
     loglevel : {"info", "debug"}, optional
-        Toggle to set the logging level: "debug" will print out additional
-        diagnostic information to the log and stdout. (Default "info")
-    mags : :class:`~quakemigrate.signal.local_mag.local_mag.LocalMag` object, \
-        optional
-        Provides methods for calculating local magnitudes, performed during
-        locate.
+        Toggle to set the logging level: "debug" will print out additional diagnostic
+        information to the log and stdout. (Default "info")
+    mags : :class:`~quakemigrate.signal.local_mag.local_mag.LocalMag` object, optional
+        Provides methods for calculating local magnitudes, performed during locate.
     marginal_window : float, optional
-        Half-width of window centred on the maximum coalescence time. The
-        4-D coalescence functioned is marginalised over time across this window
-        such that the earthquake location and associated uncertainty can be
-        appropriately calculated. It should be an estimate of the time
-        uncertainty in the earthquake origin time, which itself is some
-        combination of the expected spatial uncertainty and uncertainty in the
-        seismic velocity model used. Default: 2 seconds.
-    picker : :class:`~quakemigrate.signal.pickers.base.PhasePicker` object, \
-        optional
+        Half-width of window centred on the maximum coalescence time. The 4-D
+        coalescence functioned is marginalised over time across this window such that
+        the earthquake location and associated uncertainty can be appropriately
+        calculated. It should be an estimate of the time uncertainty in the earthquake
+        origin time, which itself is some combination of the expected spatial
+        uncertainty and uncertainty in the seismic velocity model used.
+        Default: 2 seconds.
+    picker : :class:`~quakemigrate.signal.pickers.base.PhasePicker` object, optional
         Provides callback methods for phase picking, performed during locate.
     plot_event_summary : bool, optional
         Plot event summary figure - see `quakemigrate.plot` for more details.
         Default: True.
     plot_event_video : bool, optional
         Plot coalescence video for each located earthquake. Default: False.
     post_pad : float
-        Additional amount of data to read in after the timestep, used to
-        ensure the correct coalescence is calculated at every sample.
+        Additional amount of data to read in after the timestep, used to ensure the
+        correct coalescence is calculated at every sample.
     pre_pad : float
-        Additional amount of data to read in before the timestep, used to
-        ensure the correct coalescence is calculated at every sample.
+        Additional amount of data to read in before the timestep, used to ensure the
+        correct coalescence is calculated at every sample.
     real_waveform_units : {"displacement", "velocity"}
         Units to output real cut waveforms.
     run : :class:`~quakemigrate.io.core.Run` object
         Light class encapsulating i/o path information for a given run.
     scan_rate : int, optional
-        Sampling rate at which the 4-D coalescence map will be calculated.
-        Currently fixed to be the same as the onset function sampling rate (not
+        Sampling rate at which the 4-D coalescence map will be calculated. Currently
+        fixed to be the same as the onset function sampling rate (not
         user-configurable).
     threads : int, optional
         The number of threads for the C functions to use on the executing host.
         Default: 1 thread.
     timestep : float, optional
-        Length (in seconds) of timestep used in detect(). Note: total detect
-        run duration should be divisible by timestep. Increasing timestep will
-        increase RAM usage during detect, but will slightly speed up overall
-        detect run. Default: 120 seconds.
+        Length (in seconds) of timestep used in detect(). Note: total detect run
+        duration should be divisible by timestep. Increasing timestep will increase RAM
+        usage during detect, but will slightly speed up overall detect run.
+        Default: 120 seconds.
     wa_waveform_units : {"displacement", "velocity"}
         Units to output Wood-Anderson simulated cut waveforms.
     write_cut_waveforms : bool, optional
-        Write raw cut waveforms for all data read from the archive for each
-        event located by locate(). See `~quakemigrate.io.data.Archive`
-        parameter `read_all_stations`. Default: False.
+        Write raw cut waveforms for all data read from the archive for each event
+        located by locate(). See `~quakemigrate.io.data.Archive` parameter
+        `read_all_stations`. Default: False.
         NOTE: this data has not been processed or quality-checked!
     write_real_waveforms : bool, optional
-        Write real cut waveforms for all data read from the archive for each
-        event located by locate(). See `~quakemigrate.io.data.Archive`
-        parameter `read_all_stations`. Default: False.
-        NOTE: the units of this data (displacement or velocity) are controlled
-        by `real_waveform_units`.
+        Write real cut waveforms for all data read from the archive for each event
+        located by locate(). See `~quakemigrate.io.data.Archive` parameter
+        `read_all_stations`. Default: False.
+        NOTE: the units of this data (displacement or velocity) are controlled by
+        `real_waveform_units`.
         NOTE: this data has not been processed or quality-checked!
-        NOTE: no padding has been added to take into account the taper applied
-        during response removal.
+        NOTE: no padding has been added to take into account the taper applied during
+        response removal.
     write_wa_waveforms : bool, optional
-        Write Wood-Anderson simulated cut waveforms for all data read from the
-        archive for each event located by locate(). See
-        `~quakemigrate.io.data.Archive` parameter `read_all_stations`.
-        Default: False.
-        NOTE: the units of this data (displacement or velocity) are controlled
-        by `wa_waveform_units`.
+        Write Wood-Anderson simulated cut waveforms for all data read from the archive
+        for each event located by locate(). See `~quakemigrate.io.data.Archive`
+        parameter `read_all_stations`. Default: False.
+        NOTE: the units of this data (displacement or velocity) are controlled by
+        `wa_waveform_units`.
         NOTE: this data has not been processed or quality-checked!
-        NOTE: no padding has been added to take into account the taper applied
-        during response removal.
+        NOTE: no padding has been added to take into account the taper applied during
+        response removal.
     xy_files : str, optional
-        Path to comma-separated value file (.csv) containing a series of
-        coordinate files to plot. Columns: ["File", "Color", "Linewidth",
-        "Linestyle"], where "File" is the absolute path to the file containing
-        the coordinates to be plotted. E.g:
-        "/home/user/volcano_outlines.csv,black,0.5,-". Each .csv coordinate
-        file should contain coordinates only, with columns: ["Longitude",
-        "Latitude"]. E.g.: "-17.5,64.8". Lines pre-pended with ``#`` will be
-        treated as a comment - this can be used to include references. See the
+        Path to comma-separated value file (.csv) containing a series of coordinate
+        files to plot. Columns: ["File", "Color", "Linewidth", "Linestyle"], where
+        "File" is the absolute path to the file containing the coordinates to be
+        plotted. E.g: "/home/user/volcano_outlines.csv,black,0.5,-". Each .csv
+        coordinate file should contain coordinates only, with columns: ["Longitude",
+        "Latitude"]. E.g.: "-17.5,64.8". Lines pre-pended with ``#`` will be treated as
+        a comment - this can be used to include references. See the
         Volcanotectonic_Iceland example XY_files for a template.\n
         .. note:: Do not include a header line in either file.
 
     +++ TO BE REMOVED TO ARCHIVE CLASS +++
     pre_cut : float, optional
-        Specify how long before the event origin time to cut the waveform
-        data from
+        Specify how long before the event origin time to cut the waveform data from.
     post_cut : float, optional
-        Specify how long after the event origin time to cut the waveform
+        Specify how long after the event origin time to cut the waveform.
         data to
     +++ TO BE REMOVED TO ARCHIVE CLASS +++
 
     Methods
     -------
     detect(starttime, endtime)
         Core detection method -- compute decimated 3-D coalescence continuously
         throughout entire time period; output as .scanmseed (in mSEED format).
     locate(starttime, endtime) or locate(file)
-        Core locate method -- compute 3-D coalescence over short time window
-        around candidate earthquake triggered from continuous detect output;
-        output location & uncertainties (.event file), phase picks (.picks
-        file), plus multiple optional plots / data for further analysis and
-        processing.
+        Core locate method -- compute 3-D coalescence over short time window around
+        candidate earthquake triggered from continuous detect output; output location &
+        uncertainties (.event file), phase picks (.picks file), plus multiple optional
+        plots / data for further analysis and processing.
 
     Raises
     ------
     OnsetTypeError
-        If an object is passed in through the `onset` argument that is not
-        derived from the :class:`~quakemigrate.signal.onsets.base.Onset` base
-        class.
+        If an object is passed in through the `onset` argument that is not derived from
+        the :class:`~quakemigrate.signal.onsets.base.Onset` base class.
     PickerTypeError
-        If an object is passed in through the `picker` argument that is not
-        derived from the :class:`~quakemigrate.signal.pickers.base.PhasePicker`
-        base class.
+        If an object is passed in through the `picker` argument that is not derived from
+        the :class:`~quakemigrate.signal.pickers.base.PhasePicker` base class.
     RuntimeError
         If the user does not supply the locate function with valid arguments.
     TimeSpanException
         If the user supplies a starttime that is after the endtime.
 
     """
 
@@ -198,37 +196,41 @@
         self.lut = lut
         if isinstance(onset, Onset):
             self.onset = onset
         else:
             raise util.OnsetTypeError
         self.onset.post_pad = lut.max_traveltime
 
-        self.pre_pad = 0.
-        self.post_pad = 0.
+        self.pre_pad = 0.0
+        self.post_pad = 0.0
 
         # --- Set up i/o ---
-        self.run = Run(run_path, run_name, kwargs.get("run_subname", ""),
-                       loglevel=kwargs.get("loglevel", "info"))
+        self.run = Run(
+            run_path,
+            run_name,
+            kwargs.get("run_subname", ""),
+            loglevel=kwargs.get("loglevel", "info"),
+        )
         self.log = kwargs.get("log", False)
 
         picker = kwargs.get("picker")
         if picker is None:
             self.picker = GaussianPicker(onset=onset)
         elif isinstance(picker, PhasePicker):
             self.picker = picker
         else:
             raise util.PickerTypeError
 
         # --- Grab QuakeScan parameters or set defaults ---
         # Parameters related specifically to Detect
-        self.timestep = kwargs.get("timestep", 120.)
+        self.timestep = kwargs.get("timestep", 120.0)
         self.time_step = kwargs.get("time_step")  # DEPRECATING
 
         # Parameters related specifically to Locate
-        self.marginal_window = kwargs.get("marginal_window", 2.)
+        self.marginal_window = kwargs.get("marginal_window", 2.0)
 
         # General QuakeScan parameters
         self.threads = kwargs.get("threads", 1)
         self.n_cores = kwargs.get("n_cores")  # DEPRECATING
         self.sampling_rate = kwargs.get("sampling_rate")  # DEPRECATING
         self.scan_rate = self.onset.sampling_rate
 
@@ -242,35 +244,36 @@
         # Plotting toggles and parameters
         self.plot_event_summary = kwargs.get("plot_event_summary", True)
         self.plot_event_video = kwargs.get("plot_event_video", False)
         self.xy_files = kwargs.get("xy_files")
 
         # File writing toggles
         self.continuous_scanmseed_write = kwargs.get(
-            "continuous_scanmseed_write", False)
+            "continuous_scanmseed_write", False
+        )
         self.write_cut_waveforms = kwargs.get("write_cut_waveforms", False)
         self.write_real_waveforms = kwargs.get("write_real_waveforms", False)
-        self.real_waveform_units = kwargs.get("real_waveform_units",
-                                              "displacement")
+        self.real_waveform_units = kwargs.get("real_waveform_units", "displacement")
         self.write_wa_waveforms = kwargs.get("write_wa_waveforms", False)
-        self.wa_waveform_units = kwargs.get("wa_waveform_units",
-                                            "displacement")
+        self.wa_waveform_units = kwargs.get("wa_waveform_units", "displacement")
         self.cut_waveform_format = kwargs.get("cut_waveform_format", "MSEED")
 
         # +++ TO BE REMOVED TO ARCHIVE CLASS +++
         self.pre_cut = None
         self.post_cut = None
         # +++ TO BE REMOVED TO ARCHIVE CLASS +++
 
     def __str__(self):
         """Return short summary string of the QuakeScan object."""
 
-        out = ("\tScan parameters:\n"
-               f"\t\tScan sampling rate = {self.scan_rate} Hz\n"
-               f"\t\tThread count       = {self.threads}\n")
+        out = (
+            "\tScan parameters:\n"
+            f"\t\tScan sampling rate = {self.scan_rate} Hz\n"
+            f"\t\tThread count       = {self.threads}\n"
+        )
         if self.run.stage == "detect":
             out += f"\t\tTime step          = {self.timestep} s\n"
         elif self.run.stage == "locate":
             out += f"\t\tMarginal window    = {self.marginal_window} s\n"
 
         return out
 
@@ -281,16 +284,16 @@
 
         Parameters
         ----------
         starttime : str
             Timestamp from which to run continuous scan.
         endtime : str
             Timestamp up to which to run continuous scan.
-            Note: the last sample returned will be that which immediately
-            precedes this timestamp.
+            Note: the last sample returned will be that which immediately precedes this
+            timestamp.
 
         """
 
         # Configure logging
         self.run.stage = "detect"
         self.run.logger(self.log)
 
@@ -308,19 +311,19 @@
 
         self._continuous_compute(starttime, endtime)
 
         logging.info(util.log_spacer)
 
     def locate(self, starttime=None, endtime=None, trigger_file=None):
         """
-        Re-computes the coalescence on an undecimated grid for a short
-        time window around each candidate earthquake triggered from the
-        (decimated) continuous detect scan. Calculates event location and
-        uncertainties, makes phase arrival picks, plus multiple optional
-        plotting / data outputs for further analysis and processing.
+        Re-computes the coalescence on an undecimated grid for a short time window
+        around each candidate earthquake triggered from the (decimated) continuous
+        detect scan. Calculates event location and uncertainties, makes phase arrival
+        picks, plus multiple optional plotting / data outputs for further analysis and
+        processing.
 
         Parameters
         ----------
         starttime : str, optional
             Timestamp from which to include events in the locate scan.
         endtime : str, optional
             Timestamp up to which to include events in the locate scan.
@@ -371,72 +374,79 @@
 
         Parameters
         ----------
         starttime : `obspy.UTCDateTime` object
             Timestamp from which to compute continuous coalescence.
         endtime : `obspy.UTCDateTime` object
             Timestamp up to which to compute continuous compute.
-            Note: the last sample returned will be that which immediately
-            precedes this timestamp.
+            Note: the last sample returned will be that which immediately precedes this
+            timestamp.
 
         """
 
-        coalescence = ScanmSEED(self.run, self.continuous_scanmseed_write,
-                                self.scan_rate)
+        coalescence = ScanmSEED(
+            self.run, self.continuous_scanmseed_write, self.scan_rate
+        )
 
         self.pre_pad, self.post_pad = self.onset.pad(self.timestep)
         n_steps = int(np.ceil((endtime - starttime) / self.timestep))
-        availability_cols = np.array([[f"{stat}_{ph}" for stat
-                                       in self.archive.stations]
-                                      for ph in self.onset.phases]).flatten()
-        availability = pd.DataFrame(index=range(n_steps),
-                                    columns=availability_cols)
+        availability_cols = np.array(
+            [
+                [f"{stat}_{ph}" for stat in self.archive.stations]
+                for ph in self.onset.phases
+            ]
+        ).flatten()
+        availability = pd.DataFrame(index=range(n_steps), columns=availability_cols)
 
         for i in range(n_steps):
-            w_beg = starttime + self.timestep*i - self.pre_pad
-            w_end = starttime + self.timestep*(i + 1) + self.post_pad
+            w_beg = starttime + self.timestep * i - self.pre_pad
+            w_end = starttime + self.timestep * (i + 1) + self.post_pad
             logging.debug(f" Processing : {w_beg}-{w_end} ".center(110, "~"))
-            logging.info((f" Processing : {w_beg + self.pre_pad}-"
-                          f"{w_end - self.post_pad} ").center(110, "~"))
+            logging.info(
+                (
+                    f" Processing : {w_beg + self.pre_pad}-{w_end - self.post_pad} "
+                ).center(110, "~")
+            )
 
             try:
                 data = self.archive.read_waveform_data(w_beg, w_end)
-                time, max_coa, max_coa_n, coord, onset_data = \
-                    self._compute(data)
-                coalescence.append(time, max_coa, max_coa_n, coord,
-                                   self.lut.unit_conversion_factor)
+                time, max_coa, max_coa_n, coord, onset_data = self._compute(data)
+                coalescence.append(
+                    time, max_coa, max_coa_n, coord, self.lut.unit_conversion_factor
+                )
                 availability.loc[i] = onset_data.availability
             except util.ArchiveEmptyException as e:
-                coalescence.empty(starttime, self.timestep, i, e.msg,
-                                  self.lut.unit_conversion_factor)
-                availability.loc[i] = np.zeros(len(availability_cols),
-                                               dtype=int)
+                coalescence.empty(
+                    starttime, self.timestep, i, e.msg, self.lut.unit_conversion_factor
+                )
+                availability.loc[i] = np.zeros(len(availability_cols), dtype=int)
             except util.DataGapException as e:
-                coalescence.empty(starttime, self.timestep, i, e.msg,
-                                  self.lut.unit_conversion_factor)
-                availability.loc[i] = np.zeros(len(availability_cols),
-                                               dtype=int)
+                coalescence.empty(
+                    starttime, self.timestep, i, e.msg, self.lut.unit_conversion_factor
+                )
+                availability.loc[i] = np.zeros(len(availability_cols), dtype=int)
             except util.DataAvailabilityException as e:
-                coalescence.empty(starttime, self.timestep, i, e.msg,
-                                  self.lut.unit_conversion_factor)
-                availability.loc[i] = np.zeros(len(availability_cols),
-                                               dtype=int)
-
-            availability.rename(index={i: str(starttime + self.timestep*i)},
-                                inplace=True)
+                coalescence.empty(
+                    starttime, self.timestep, i, e.msg, self.lut.unit_conversion_factor
+                )
+                availability.loc[i] = np.zeros(len(availability_cols), dtype=int)
+
+            availability.rename(
+                index={i: str(starttime + self.timestep * i)}, inplace=True
+            )
 
         if not coalescence.written:
             coalescence.write()
         write_availability(self.run, availability)
 
     def _locate_events(self, **kwargs):
         """
-        Loop through list of earthquakes read in from trigger results and
-        re-compute coalescence; output phase picks, event location and
-        uncertainty, plus optional plots and outputs.
+        Loop through list of earthquakes read in from trigger results and re-compute
+        coalescence; output phase picks, event location and uncertainty, plus optional
+        plots and outputs.
 
         Parameters
         ----------
         kwargs : **dict
             Can contain:
             starttime : `obspy.UTCDateTime` object, optional
                 Timestamp from which to include events in the locate scan.
@@ -446,31 +456,31 @@
                 File containing triggered events to be located.
 
         """
 
         triggered_events = read_triggered_events(self.run, **kwargs)
         n_events = len(triggered_events.index)
 
-        self.pre_pad, self.post_pad = self.onset.pad(4*self.marginal_window)
+        self.pre_pad, self.post_pad = self.onset.pad(4 * self.marginal_window)
 
         for i, triggered_event in triggered_events.iterrows():
             event = Event(self.marginal_window, triggered_event)
-            w_beg = event.trigger_time - 2*self.marginal_window - self.pre_pad
-            w_end = event.trigger_time + 2*self.marginal_window + self.post_pad
+            w_beg = event.trigger_time - 2 * self.marginal_window - self.pre_pad
+            w_end = event.trigger_time + 2 * self.marginal_window + self.post_pad
             logging.info(util.log_spacer)
             logging.info(f"\tEVENT - {i+1} of {n_events} - {event.uid}")
             logging.info(util.log_spacer)
 
             try:
                 logging.info("\tReading waveform data...")
-                event.add_waveform_data(
-                    self._read_event_waveform_data(w_beg, w_end))
+                event.add_waveform_data(self._read_event_waveform_data(w_beg, w_end))
                 logging.info("\tComputing 4-D coalescence function...")
                 event.add_compute_output(  # pylint: disable=E1120
-                    *self._compute(event.data, event))
+                    *self._compute(event.data, event)
+                )
             except util.ArchiveEmptyException as e:
                 logging.info(e.msg)
                 continue
             except util.DataGapException as e:
                 logging.info(e.msg)
                 continue
             except util.DataAvailabilityException as e:
@@ -493,36 +503,53 @@
             if self.mags is not None:
                 logging.info("\tCalculating magnitude...")
                 event, _ = self.mags.calc_magnitude(event, self.lut, self.run)
 
             event.write(self.run, self.lut)
 
             if self.plot_event_summary:
-                event_summary(self.run, event, marginalised_coa_map,
-                              self.lut, xy_files=self.xy_files)
+                event_summary(
+                    self.run,
+                    event,
+                    marginalised_coa_map,
+                    self.lut,
+                    xy_files=self.xy_files,
+                )
 
             if self.plot_event_video:
                 logging.info("Support for event videos coming soon.")
 
             if self.write_cut_waveforms:
-                write_cut_waveforms(self.run, event, self.cut_waveform_format,
-                                    pre_cut=self.pre_cut,
-                                    post_cut=self.post_cut)
+                write_cut_waveforms(
+                    self.run,
+                    event,
+                    self.cut_waveform_format,
+                    pre_cut=self.pre_cut,
+                    post_cut=self.post_cut,
+                )
             if self.write_real_waveforms:
-                write_cut_waveforms(self.run, event, self.cut_waveform_format,
-                                    pre_cut=self.pre_cut,
-                                    post_cut=self.post_cut,
-                                    waveform_type="real",
-                                    units=self.real_waveform_units)
+                write_cut_waveforms(
+                    self.run,
+                    event,
+                    self.cut_waveform_format,
+                    pre_cut=self.pre_cut,
+                    post_cut=self.post_cut,
+                    waveform_type="real",
+                    units=self.real_waveform_units,
+                )
             if self.write_wa_waveforms:
-                write_cut_waveforms(self.run, event, self.cut_waveform_format,
-                                    pre_cut=self.pre_cut,
-                                    post_cut=self.post_cut,
-                                    waveform_type="wa",
-                                    units=self.wa_waveform_units)
+                write_cut_waveforms(
+                    self.run,
+                    event,
+                    self.cut_waveform_format,
+                    pre_cut=self.pre_cut,
+                    post_cut=self.post_cut,
+                    waveform_type="wa",
+                    units=self.wa_waveform_units,
+                )
 
             del event, marginalised_coa_map
             logging.info(util.log_spacer)
 
     @util.timeit("info")
     def _compute(self, data, event=None):
         """
@@ -538,35 +565,34 @@
         times : `numpy.ndarray` of `obspy.UTCDateTime` objects, shape(nsamples)
             Timestamps for the coalescence data.
         max_coa : `numpy.ndarray` of floats, shape(nsamples)
             Coalescence value through time.
         max_coa_n : `numpy.ndarray` of floats, shape(nsamples)
             Normalised coalescence value through time.
         coord : `numpy.ndarray` of floats, shape(nsamples)
-            Location of maximum coalescence through time in input projection
-            space.
+            Location of maximum coalescence through time in input projection space.
         map4d : `numpy.ndarry`, shape(nx, ny, nz, nsamp), optional
             4-D coalescence map.
 
         """
 
         # --- Calculate continuous coalescence within 3-D volume ---
         onsets, onset_data = self.onset.calculate_onsets(data)
         try:
-            traveltimes = self.lut.serve_traveltimes(onset_data.sampling_rate,
-                                                     onset_data.availability)
+            traveltimes = self.lut.serve_traveltimes(
+                onset_data.sampling_rate, onset_data.availability
+            )
         except KeyError as e:
-            msg = (f"Attempting to migrate phases {onset_data.phases}; but "
-                   f"traveltimes for {e} not found in the LUT. Please "
-                   "create a new lookup table with phases="
-                   f"{onset_data.phases}")
-            raise util.LUTPhasesException(msg)
-        # Here fsmp and lsmp are used to calculate the length of map4d from the
-        # shape of the onset functions --> need to use onset sampling_rate, not
-        # scan rate.
+            raise util.LUTPhasesException(
+                f"Attempting to migrate phases {onset_data.phases}; but traveltimes "
+                f"for {e} not found in the LUT. Please create a new lookup table with "
+                f"phases={onset_data.phases}"
+            )
+        # Here fsmp and lsmp are used to calculate the length of map4d from the shape of
+        # the onset functions --> need to use onset sampling_rate, not scan rate.
         fsmp = util.time2sample(self.pre_pad, onset_data.sampling_rate)
         lsmp = util.time2sample(self.post_pad, onset_data.sampling_rate)
         avail = np.sum([value for _, value in onset_data.availability.items()])
         map4d = migrate(onsets, traveltimes, fsmp, lsmp, avail, self.threads)
 
         # --- Find continuous peak coalescence in 3-D volume ---
         max_coa, max_coa_n, max_idx = find_max_coa(map4d, self.threads)
@@ -596,57 +622,56 @@
         -------
         data : :class:`~quakemigrate.io.data.WaveformData` object
             Light class encapsulating data returned by an archive query.
 
         """
 
         # Extra pre- and post-pad default to 0.
-        pre_pad = post_pad = 0.
+        pre_pad = post_pad = 0.0
 
         # If calculating magnitudes, read in padding required for amplitude
         # measurements.
         if self.mags:
             pre_pad, post_pad = self.mags.amp.pad(
-                self.marginal_window,
-                self.lut.max_traveltime,
-                self.lut.fraction_tt)
+                self.marginal_window, self.lut.max_traveltime, self.lut.fraction_tt
+            )
 
         # If a specific pre / post cut has been requested by the user,
         # check which is bigger.
         if self.pre_cut:
             pre_pad = max(pre_pad, self.pre_cut)
         if self.post_cut:
             post_pad = max(post_pad, self.post_cut)
 
-        # Trim the pre_pad and post_pad to avoid cutting more data than we
-        # need; only subtract 1*marginal_window so that if the event otime
-        # moves by this much (the maximum allowed) from the triggered event
-        # time, we still have the correct window of data to apply the pre_cut.
-        pre_pad = max(0., pre_pad - self.marginal_window - self.pre_pad)
-        post_pad = max(0., post_pad - self.marginal_window - self.post_pad)
+        # Trim the pre_pad and post_pad to avoid cutting more data than we need; only
+        # subtract 1*marginal_window so that if the event otime moves by this much (the
+        # maximum allowed) from the triggered event time, we still have the correct
+        # window of data to apply the pre_cut.
+        pre_pad = max(0.0, pre_pad - self.marginal_window - self.pre_pad)
+        post_pad = max(0.0, post_pad - self.marginal_window - self.post_pad)
 
         logging.debug(f"{w_beg}, {w_end}, {pre_pad}, {post_pad}")
         return self.archive.read_waveform_data(w_beg, w_end, pre_pad, post_pad)
 
     @util.timeit("info")
     def _calculate_location(self, event):
         """
-        Marginalise the 4-D coalescence grid and calculate a set of locations
-        and associated uncertainties by:
+        Marginalise the 4-D coalescence grid and calculate a set of locations and
+        associated uncertainties by:
             (1) calculating the covariance of the entire coalescence map;
             (2) smoothing and fitting a 3-D Gaussian function and ..
             (3) fitting a 3-D spline function ..
                 to a region around the maximum coalescence location in the
                 marginalised 3-D coalescence map.
 
         Parameters
         ----------
         event : :class:`~quakemigrate.io.event.Event` object
-            Light class encapsulating waveforms, coalescence information, picks
-            and location information for a given event.
+            Light class encapsulating waveforms, coalescence information, picks and
+            location information for a given event.
 
         Returns
         -------
         coa_map : array-like
             Marginalised 3-D coalescence map.
 
         """
@@ -666,25 +691,25 @@
         event.add_covariance_location(*self._covfit3d(np.copy(coa_map)))
 
         return coa_map
 
     @util.timeit()
     def _splineloc(self, coa_map, win=5, upscale=10):
         """
-        Fit a 3-D spline function to a region around the maximum coalescence
-        in the marginalised coalescence map and interpolate by factor `upscale`
-        to return a sub-grid maximum coalescence location.
+        Fit a 3-D spline function to a region around the maximum coalescence in the
+        marginalised coalescence map and interpolate by factor `upscale` to return a
+        sub-grid maximum coalescence location.
 
         Parameters
         ----------
         coa_map : array-like
             Marginalised 3-D coalescence map.
         win : int
-            Window of grid nodes (+/-(win-1)//2 in x, y and z) around max
-            value in coa_map to perform the fit over.
+            Window of grid nodes (+/-(win-1)//2 in x, y and z) around max value in
+            coa_map to perform the fit over.
         upscale : int
             Upscaling factor to interpolate the fitted 3-D spline function by.
 
         Returns
         -------
         location : array-like, [x, y, z]
             Max coalescence location from spline interpolation.
@@ -696,156 +721,170 @@
         n = np.array([nx, ny, nz])
 
         # Find maximum coalescence location in grid
         mx, my, mz = np.unravel_index(np.nanargmax(coa_map), coa_map.shape)
         i = np.array([mx, my, mz])
 
         # Determining window about maximum value and trimming coa grid
-        w2 = (win - 1)//2
+        w2 = (win - 1) // 2
         x1, y1, z1 = np.clip(i - w2, 0 * n, n)
         x2, y2, z2 = np.clip(i + w2 + 1, 0 * n, n)
 
         # If subgrid is not close to the edge
         if (x2 - x1) == (y2 - y1) == (z2 - z1):
             coa_map_trim = coa_map[x1:x2, y1:y2, z1:z2]
 
             # Defining the original interpolation function
-            xo = np.linspace(0, coa_map_trim.shape[0] - 1,
-                             coa_map_trim.shape[0])
-            yo = np.linspace(0, coa_map_trim.shape[1] - 1,
-                             coa_map_trim.shape[1])
-            zo = np.linspace(0, coa_map_trim.shape[2] - 1,
-                             coa_map_trim.shape[2])
+            xo = np.linspace(0, coa_map_trim.shape[0] - 1, coa_map_trim.shape[0])
+            yo = np.linspace(0, coa_map_trim.shape[1] - 1, coa_map_trim.shape[1])
+            zo = np.linspace(0, coa_map_trim.shape[2] - 1, coa_map_trim.shape[2])
             xog, yog, zog = np.meshgrid(xo, yo, zo)
-            interpgrid = Rbf(xog.flatten(), yog.flatten(), zog.flatten(),
-                             coa_map_trim.flatten(),
-                             function="cubic")
+            interpgrid = Rbf(
+                xog.flatten(),
+                yog.flatten(),
+                zog.flatten(),
+                coa_map_trim.flatten(),
+                function="cubic",
+            )
 
             # Creating the new interpolated grid
-            xx = np.linspace(0, coa_map_trim.shape[0] - 1,
-                             (coa_map_trim.shape[0] - 1) * upscale + 1)
-            yy = np.linspace(0, coa_map_trim.shape[1] - 1,
-                             (coa_map_trim.shape[1] - 1) * upscale + 1)
-            zz = np.linspace(0, coa_map_trim.shape[2] - 1,
-                             (coa_map_trim.shape[2] - 1) * upscale + 1)
+            xx = np.linspace(
+                0, coa_map_trim.shape[0] - 1, (coa_map_trim.shape[0] - 1) * upscale + 1
+            )
+            yy = np.linspace(
+                0, coa_map_trim.shape[1] - 1, (coa_map_trim.shape[1] - 1) * upscale + 1
+            )
+            zz = np.linspace(
+                0, coa_map_trim.shape[2] - 1, (coa_map_trim.shape[2] - 1) * upscale + 1
+            )
             xxg, yyg, zzg = np.meshgrid(xx, yy, zz)
 
             # Interpolate spline function on new grid
-            coa_map_int = interpgrid(xxg.flatten(), yyg.flatten(),
-                                     zzg.flatten()).reshape(xxg.shape)
+            coa_map_int = interpgrid(
+                xxg.flatten(), yyg.flatten(), zzg.flatten()
+            ).reshape(xxg.shape)
 
             # Calculate max coalescence location on interpolated grid
-            mxi, myi, mzi = np.unravel_index(np.nanargmax(coa_map_int),
-                                             coa_map_int.shape)
-            mxi = mxi/upscale + x1
-            myi = myi/upscale + y1
-            mzi = mzi/upscale + z1
+            mxi, myi, mzi = np.unravel_index(
+                np.nanargmax(coa_map_int), coa_map_int.shape
+            )
+            mxi = mxi / upscale + x1
+            myi = myi / upscale + y1
+            mzi = mzi / upscale + z1
             logging.debug(f"\t\tGridded loc: {mx}   {my}   {mz}")
             logging.debug(f"\t\tSpline  loc: {mxi} {myi} {mzi}")
 
             # Run check that spline location is within grid-cell
-            if (abs(mx - mxi) > 1) or (abs(my - myi) > 1) or \
-               (abs(mz - mzi) > 1):
-                logging.debug("\tSpline warning: spline location outside grid "
-                              "cell with maximum coalescence value")
+            if (abs(mx - mxi) > 1) or (abs(my - myi) > 1) or (abs(mz - mzi) > 1):
+                logging.debug(
+                    "\tSpline warning: spline location outside grid "
+                    "cell with maximum coalescence value"
+                )
 
             location = self.lut.index2coord([[mxi, myi, mzi]])[0]
 
             # Run check that spline location is within window
-            if (abs(mx - mxi) > w2) or (abs(my - myi) > w2) or \
-               (abs(mz - mzi) > w2):
-                logging.info("\t !!!! Spline error: location outside"
-                             "interpolation window !!!!")
+            if (abs(mx - mxi) > w2) or (abs(my - myi) > w2) or (abs(mz - mzi) > w2):
+                logging.info(
+                    "\t !!!! Spline error: location outside interpolation window !!!!"
+                )
                 logging.info("\t\t\tGridded Location returned")
 
                 location = self.lut.index2coord([[mx, my, mz]])[0]
         else:
-            logging.info("\t !!!! Spline error: interpolation window crosses "
-                         "edge of grid !!!!")
+            logging.info(
+                "\t !!!! Spline error: interpolation window crosses edge of grid !!!!"
+            )
             logging.info("\t\t\tGridded Location returned")
 
             location = self.lut.index2coord([[mx, my, mz]])[0]
 
         return location
 
     @util.timeit()
-    def _gaufit3d(self, coa_map, thresh=0., win=7):
+    def _gaufit3d(self, coa_map, thresh=0.0, win=7):
         """
-        Fit a 3-D Gaussian function to a region around the maximum coalescence
-        location in the 3-D marginalised coalescence map: return expectation
-        location and associated uncertainty.
+        Fit a 3-D Gaussian function to a region around the maximum coalescence location
+        in the 3-D marginalised coalescence map: return expectation location and
+        associated uncertainty.
 
         Parameters
         ----------
         coa_map : array-like
             Marginalised 3-D coalescence map.
         thresh : float (between 0 and 1), optional
-            Cut-off threshold (percentile) to trim coa_map: only data above
-            this percentile will be retained.
+            Cut-off threshold (percentile) to trim coa_map: only data above this
+            percentile will be retained.
         win : int, optional
-            Window of grid nodes (+/-(win-1)//2 in x, y and z) around max
-            value in coa_map to perform the fit over.
+            Window of grid nodes (+/-(win-1)//2 in x, y and z) around max value in
+            coa_map to perform the fit over.
 
         Returns
         -------
         location : array-like, [x, y, z]
             Expectation location from 3-D Gaussian fit.
         uncertainty : array-like, [sx, sy, sz]
-            One sigma uncertainties on expectation location from 3-D Gaussian
-            fit.
+            One sigma uncertainties on expectation location from 3-D Gaussian fit.
 
         """
 
         # Get shape of 3-D coalescence map and max coalescence grid location
         shape = coa_map.shape
         ijk = np.unravel_index(np.nanargmax(coa_map), shape)
 
-        # Only use grid nodes above threshold value, and within the specified
-        # window around the coalescence peak
+        # Only use grid nodes above threshold value, and within the specified window
+        # around the coalescence peak
         flag = np.logical_and(coa_map > thresh, self._mask3d(shape, ijk, win))
         ix, iy, iz = np.where(flag)
 
-        # Subtract mean of entire 3-D coalescence map from the local grid
-        # window so it is better approximated by a Gaussian (which goes to zero
-        # at infinity)
+        # Subtract mean of entire 3-D coalescence map from the local grid window so it
+        # is better approximated by a Gaussian (which goes to zero at infinity)
         coa_map = coa_map - np.nanmean(coa_map)
 
         ls = [np.arange(n) for n in shape]
 
         # Get ijk indices for points in the sub-grid
-        x, y, z = [l[idx] - i for l, idx, i in zip(ls, np.where(flag), ijk)]
+        x, y, z = [L[idx] - i for L, idx, i in zip(ls, np.where(flag), ijk)]
 
-        X = np.c_[x * x, y * y, z * z,
-                  x * y, x * z, y * z,
-                  x, y, z, np.ones(len(ix))].T
-        Y = -np.log(np.clip(coa_map.astype(np.float64)[ix, iy, iz],
-                            1e-300, np.inf))
+        X = np.c_[x * x, y * y, z * z, x * y, x * z, y * z, x, y, z, np.ones(len(ix))].T
+        Y = -np.log(np.clip(coa_map.astype(np.float64)[ix, iy, iz], 1e-300, np.inf))
 
         X_inv = np.linalg.pinv(X)
         P = np.matmul(Y, X_inv)
-        G = -np.array([2 * P[0], P[3], P[4],
-                       P[3], 2 * P[1], P[5],
-                       P[4], P[5], 2 * P[2]]).reshape((3, 3))
+        G = -np.array(
+            [2 * P[0], P[3], P[4], P[3], 2 * P[1], P[5], P[4], P[5], 2 * P[2]]
+        ).reshape((3, 3))
         H = np.array([P[6], P[7], P[8]])
         loc = np.matmul(np.linalg.inv(G), H)
         cx, cy, cz = loc
 
-        K = P[9]             \
-            - P[0] * cx ** 2 \
-            - P[1] * cy ** 2 \
-            - P[2] * cz ** 2 \
-            - P[3] * cx * cy \
-            - P[4] * cx * cz \
-            - P[5] * cy * cz \
-
-        M = np.array([P[0], P[3] / 2, P[4] / 2,
-                      P[3] / 2, P[1], P[5] / 2,
-                      P[4] / 2, P[5] / 2, P[2]]).reshape(3, 3)
+        K = (
+            P[9]
+            - P[0] * cx**2
+            - P[1] * cy**2
+            - P[2] * cz**2
+            - P[3] * cx * cy
+            - P[4] * cx * cz
+            - P[5] * cy * cz
+        )
+        M = np.array(
+            [
+                P[0],
+                P[3] / 2,
+                P[4] / 2,
+                P[3] / 2,
+                P[1],
+                P[5] / 2,
+                P[4] / 2,
+                P[5] / 2,
+                P[2],
+            ]
+        ).reshape(3, 3)
         egv, vec = np.linalg.eig(M)
-        sgm = np.sqrt(0.5 / np.clip(np.abs(egv), 1e-10, np.inf))/2
+        sgm = np.sqrt(0.5 / np.clip(np.abs(egv), 1e-10, np.inf)) / 2
         val = np.exp(-K)
         csgm = np.sqrt(0.5 / np.clip(np.abs(M.diagonal()), 1e-10, np.inf))
 
         # Convert back to whole-grid coordinates
         gau_3d = [loc + ijk, vec, sgm, csgm, val]
 
         # Convert grid location to XYZ / coordinates
@@ -855,48 +894,45 @@
         uncertainty = sgm * self.lut.node_spacing
 
         return location, uncertainty
 
     @util.timeit()
     def _covfit3d(self, coa_map, thresh=0.90, win=None):
         """
-        Calculate the 3-D covariance of the marginalised coalescence map,
-        filtered above a percentile threshold `thresh`. Optionally can also
-        perform the fit on a sub-window of the grid around the maximum
-        coalescence location.
+        Calculate the 3-D covariance of the marginalised coalescence map, filtered above
+        a percentile threshold `thresh`. Optionally can also perform the fit on a
+        sub-window of the grid around the maximum coalescence location.
 
         Parameters
         ----------
         coa_map : array-like
             Marginalised 3-D coalescence map.
         thresh : float (between 0 and 1), optional
-            Cut-off threshold (fractional percentile) to trim coa_map; only
-            data above this percentile will be retained.
+            Cut-off threshold (fractional percentile) to trim coa_map; only data above
+            this percentile will be retained.
         win : int, optional
-            Window of grid nodes (+/-(win-1)//2 in x, y and z) around max
-            value in coa_map to perform the fit over.
+            Window of grid nodes (+/-(win-1)//2 in x, y and z) around max value in
+            coa_map to perform the fit over.
 
         Returns
         -------
         location : array-like, [x, y, z]
             Expectation location from covariance fit.
         uncertainty : array-like, [sx, sy, sz]
-            One sigma uncertainties on expectation location from covariance
-            fit.
+            One sigma uncertainties on expectation location from covariance fit.
 
         """
 
         # Get shape of 3-D coalescence map and max coalesence grid location
         shape = coa_map.shape
         ijk = np.unravel_index(np.nanargmax(coa_map), coa_map.shape)
 
         # If window is specified, clip the grid to only look here.
         if win:
-            flag = np.logical_and(coa_map > thresh, self._mask3d(shape, ijk,
-                                                                 win))
+            flag = np.logical_and(coa_map > thresh, self._mask3d(shape, ijk, win))
         else:
             flag = np.where(coa_map > thresh, True, False)
 
         # Treat the coalescence values in the grid as the sample weights
         sw = coa_map.flatten()
         sw[~flag.flatten()] = np.nan
         ssw = np.nansum(sw)
@@ -927,24 +963,24 @@
         uncertainty = np.diag(np.sqrt(abs(cov_matrix)))
 
         return location, uncertainty
 
     @util.timeit()
     def _gaufilt3d(self, map3d, sgm=0.8, shp=None):
         """
-        Smooth the 3-D marginalised coalescence map using a 3-D Gaussian
-        function to enable a better Gaussian fit to the data to be calculated.
+        Smooth the 3-D marginalised coalescence map using a 3-D Gaussian function to
+        enable a better Gaussian fit to the data to be calculated.
 
         Parameters
         ----------
         map3d : array-like
             Marginalised 3-D coalescence map.
         sgm : float
-            Sigma value (in grid nodes) for the 3-D Gaussian filter function;
-            bigger sigma leads to more aggressive (long wavelength) smoothing.
+            Sigma value (in grid nodes) for the 3-D Gaussian filter function; bigger
+            sigma leads to more aggressive (long wavelength) smoothing.
         shp : array-like, optional
             Shape of volume.
 
         Returns
         -------
         smoothed_map : array-like
             Gaussian smoothed 3-D coalescence map.
@@ -1009,53 +1045,61 @@
     @scan_rate.setter
     def scan_rate(self, value):
         if value is None:
             return
         elif value == self.onset.sampling_rate:
             self._scan_rate = value
             return
-        print("Warning: Parameter not yet user-configurable. Currently ")
-        print("the scan sampling rate must be the same as the onset sampling ")
-        print(f"rate, which you have set to {self.scan_rate} Hz. Please ")
-        print("contact the QuakeMigrate developers for further info.")
+        print(
+            "Warning: Parameter not yet user-configurable. Currently\n"
+            "the scan sampling rate must be the same as the onset sampling\n"
+            f"rate, which you have set to {self.scan_rate} Hz. Please\n"
+            "contact the QuakeMigrate developers for further info."
+        )
 
     @property
     def sampling_rate(self):
         """Get sampling_rate"""
         return self.scan_rate
 
     @sampling_rate.setter
     def sampling_rate(self, value):
         if value is None:
             return
-        print("Warning: Parameter name has changed - continuing. Currently ")
-        print("the scan sampling rate must be the same as the onset sampling ")
-        print(f"rate, which you have set to {self.scan_rate} Hz. Please ")
-        print("contact the QuakeMigrate developers for further info.")
+        print(
+            "Warning: Parameter name has changed - continuing. Currently\n"
+            "the scan sampling rate must be the same as the onset sampling\n"
+            f"rate, which you have set to {self.scan_rate} Hz. Please\n"
+            "contact the QuakeMigrate developers for further info."
+        )
 
     @property
     def time_step(self):
         """Handler for deprecated attribute name 'time_step'"""
         return self.timestep
 
     @time_step.setter
     def time_step(self, value):
         if value is None:
             return
-        print("FutureWarning: Parameter name has changed - continuing.")
-        print("To remove this message, change:")
-        print("\t'time_step' -> 'timestep'")
+        print(
+            "FutureWarning: Parameter name has changed - continuing.\n"
+            "To remove this message, change:\n"
+            "\t'time_step' -> 'timestep'"
+        )
         self.timestep = value
 
     @property
     def n_cores(self):
         """Handler for deprecated attribute name 'n_cores'"""
         return self.threads
 
     @n_cores.setter
     def n_cores(self, value):
         if value is None:
             return
-        print("FutureWarning: Parameter name has changed - continuing.")
-        print("To remove this message, change:")
-        print("\t'n_cores' -> 'threads'")
+        print(
+            "FutureWarning: Parameter name has changed - continuing.\n"
+            "To remove this message, change:\n"
+            "\t'n_cores' -> 'threads'"
+        )
         self.threads = value
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quakemigrate-1.0.1/quakemigrate/signal/trigger.py` & `quakemigrate-1.0.2/quakemigrate/signal/trigger.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 Module to perform the trigger stage of QuakeMigrate.
 
 :copyright:
-    2020 - 2021, QuakeMigrate developers.
+    2020–2023, QuakeMigrate developers.
 :license:
     GNU General Public License, Version 3
     (https://www.gnu.org/licenses/gpl-3.0.html)
 
 """
 
 import logging
@@ -26,118 +26,136 @@
     Create a trace filled with chunks of the same value.
 
     Parameters:
     -----------
     a : array-like
         Array of chunks.
     new_shape : tuple of ints
-        (number of chunks, chunk_length)
+        (number of chunks, chunk_length).
 
     Returns:
     --------
     b : array-like
         Single array of values contained in `a`.
 
     """
 
     b = np.broadcast_to(a[:, None], new_shape)
     b = np.reshape(b, np.product(new_shape))
 
     return b
 
 
-CANDIDATES_COLS = ["EventNum", "CoaTime", "TRIG_COA", "COA_X", "COA_Y",
-                   "COA_Z", "MinTime", "MaxTime", "COA", "COA_NORM"]
-
-REFINED_EVENTS_COLS = ["EventID", "CoaTime", "TRIG_COA", "COA_X", "COA_Y",
-                       "COA_Z", "MinTime", "MaxTime", "COA", "COA_NORM"]
+CANDIDATES_COLS = [
+    "EventNum",
+    "CoaTime",
+    "TRIG_COA",
+    "COA_X",
+    "COA_Y",
+    "COA_Z",
+    "MinTime",
+    "MaxTime",
+    "COA",
+    "COA_NORM",
+]
+
+REFINED_EVENTS_COLS = [
+    "EventID",
+    "CoaTime",
+    "TRIG_COA",
+    "COA_X",
+    "COA_Y",
+    "COA_Z",
+    "MinTime",
+    "MaxTime",
+    "COA",
+    "COA_NORM",
+]
 
 
 class Trigger:
     """
     QuakeMigrate triggering class.
 
-    Triggers candidate earthquakes from the continuous maximum coalescence
-    through time data output by the decimated detect scan, ready to be run
-    through locate().
+    Triggers candidate earthquakes from the continuous maximum coalescence through time
+    data output by the decimated detect scan, ready to be run through locate().
 
     Parameters
     ----------
     lut : :class:`~quakemigrate.lut.lut.LUT` object
-        Contains the traveltime lookup tables for the selected seismic phases,
-        computed for some pre-defined velocity model.
+        Contains the traveltime lookup tables for the selected seismic phases, computed
+        for some pre-defined velocity model.
     run_path : str
-        Points to the top level directory containing all input files, under
-        which the specific run directory will be created.
+        Points to the top level directory containing all input files, under which the
+        specific run directory will be created.
     run_name : str
         Name of the current QuakeMigrate run.
     kwargs : **dict
         See Trigger Attributes for details. In addition to these:
         log : bool, optional
-            Toggle for logging. If True, will output to stdout and generate a
-            log file. Default is to only output to stdout.
+            Toggle for logging. If True, will output to stdout and generate a log file.
+            Default is to only output to stdout.
         loglevel : {"info", "debug"}, optional
             Toggle to set the logging level: "debug" will print out additional
             diagnostic information to the log and stdout. (Default "info")
         trigger_name : str
             Optional name of a sub-run - useful when testing different trigger
             parameters, for example.
 
     Attributes
     ----------
     mad_window_length : float, optional
         Length of window within which to calculate the Median Average
         Deviation. Default: 3600 seconds (1 hour).
     mad_multiplier : float, optional
-        A scaling factor for the MAD output to make the calculated MAD factor
-        a consistent estimation of the standard deviation of the distribution.
+        A scaling factor for the MAD output to make the calculated MAD factor a
+        consistent estimation of the standard deviation of the distribution.
         Default: 1.4826, which is the appropriate scaling factor for a normal
         distribution.
     marginal_window : float, optional
-        Half-width of window centred on the maximum coalescence time. The
-        4-D coalescence functioned is marginalised over time across this window
-        such that the earthquake location and associated uncertainty can be
-        appropriately calculated. It should be an estimate of the time
-        uncertainty in the earthquake origin time, which itself is some
-        combination of the expected spatial uncertainty and uncertainty in the
-        seismic velocity model used. Default: 2 seconds.
+        Half-width of window centred on the maximum coalescence time. The 4-D
+        coalescence functioned is marginalised over time across this window such that
+        the earthquake location and associated uncertainty can be appropriately
+        calculated. It should be an estimate of the time uncertainty in the earthquake
+        origin time, which itself is some combination of the expected spatial
+        uncertainty and uncertainty in the seismic velocity model used.
+        Default: 2 seconds.
     min_event_interval : float, optional
-        Minimum time interval between triggered events. Must be at least twice
-        the marginal window. Default: 4 seconds.
+        Minimum time interval between triggered events. Must be at least twice the
+        marginal window. Default: 4 seconds.
     normalise_coalescence : bool, optional
-        If True, triggering is performed on the maximum coalescence normalised
-        by the mean coalescence value in the 3-D grid. Default: False.
+        If True, triggering is performed on the maximum coalescence normalised by the
+        mean coalescence value in the 3-D grid. Default: False.
     pad : float, optional
-        Additional time padding to ensure events close to the starttime/endtime
-        are not cut off and missed. Default: 120 seconds.
+        Additional time padding to ensure events close to the starttime/endtime are not
+        cut off and missed. Default: 120 seconds.
     plot_trigger_summary : bool, optional
         Plot triggering through time for each batched segment. Default: True.
     run : :class:`~quakemigrate.io.core.Run` object
         Light class encapsulating i/o path information for a given run.
     static_threshold : float, optional
         Static threshold value above which to trigger candidate events.
     threshold_method : str, optional
-        Toggle between a "static" threshold and a "dynamic" threshold, based on
-        the Median Average Deviation. Default: "static".
+        Toggle between a "static" threshold and a "dynamic" threshold, based on the
+        Median Average Deviation. Default: "static".
     xy_files : str, optional
-        Path to comma-separated value file (.csv) containing a series of
-        coordinate files to plot. Columns: ["File", "Color", "Linewidth",
-        "Linestyle"], where "File" is the absolute path to the file containing
-        the coordinates to be plotted. E.g:
-        "/home/user/volcano_outlines.csv,black,0.5,-". Each .csv coordinate
-        file should contain coordinates only, with columns: ["Longitude",
-        "Latitude"]. E.g.: "-17.5,64.8". Lines pre-pended with ``#`` will be
-        treated as a comment - this can be used to include references. See the
+        Path to comma-separated value file (.csv) containing a series of coordinate
+        files to plot. Columns: ["File", "Color", "Linewidth", "Linestyle"], where
+        "File" is the absolute path to the file containing the coordinates to be
+        plotted. E.g: "/home/user/volcano_outlines.csv,black,0.5,-". Each .csv
+        coordinate file should contain coordinates only, with columns: ["Longitude",
+        "Latitude"]. E.g.: "-17.5,64.8". Lines pre-pended with ``#`` will be treated as
+        a comment - this can be used to include references. See the
         Volcanotectonic_Iceland example XY_files for a template.\n
         .. note:: Do not include a header line in either file.
     plot_all_stns : bool, optional
-        If true, plot all stations used for detect. Otherwise, only plot
-        stations which for which some data was available during the trigger
-        time window. NOTE: if no station availability data is found, all
-        stations in the LUT will be plotted. (Default: True)
+        If true, plot all stations used for detect. Otherwise, only plot stations which
+        for which some data was available during the trigger time window. NOTE: if no
+        station availability data is found, all stations in the LUT will be plotted.
+        (Default: True)
 
     Methods
     -------
     trigger(starttime, endtime, region=None, interactive_plot=False)
         Trigger candidate earthquakes from decimated detect scan results.
 
     Raises
@@ -153,55 +171,64 @@
 
     def __init__(self, lut, run_path, run_name, **kwargs):
         """Instantiate the Trigger object."""
 
         self.lut = lut
 
         # --- Organise i/o and logging ---
-        self.run = Run(run_path, run_name, kwargs.get("trigger_name", ""),
-                       "trigger", loglevel=kwargs.get("loglevel", "info"))
+        self.run = Run(
+            run_path,
+            run_name,
+            kwargs.get("trigger_name", ""),
+            "trigger",
+            loglevel=kwargs.get("loglevel", "info"),
+        )
         self.run.logger(kwargs.get("log", False))
 
         # --- Grab Trigger parameters or set defaults ---
         self.threshold_method = kwargs.get("threshold_method", "static")
         if self.threshold_method == "static":
             self.static_threshold = kwargs.get("static_threshold", 1.5)
         elif self.threshold_method == "dynamic":
-            self.mad_window_length = kwargs.get("mad_window_length", 3600.)
-            self.mad_multiplier = kwargs.get("mad_multiplier", 1.)
+            self.mad_window_length = kwargs.get("mad_window_length", 3600.0)
+            self.mad_multiplier = kwargs.get("mad_multiplier", 1.0)
         else:
             raise util.InvalidTriggerThresholdMethodException
-        self.marginal_window = kwargs.get("marginal_window", 2.)
-        self.min_event_interval = kwargs.get("min_event_interval", 4.)
+        self.marginal_window = kwargs.get("marginal_window", 2.0)
+        self.min_event_interval = kwargs.get("min_event_interval", 4.0)
         if kwargs.get("minimum_repeat"):
             self.minimum_repeat = kwargs.get("minimum_repeat")
         self.normalise_coalescence = kwargs.get("normalise_coalescence", False)
-        self.pad = kwargs.get("pad", 120.)
+        self.pad = kwargs.get("pad", 120.0)
 
         # --- Plotting toggles and parameters ---
         self.plot_trigger_summary = kwargs.get("plot_trigger_summary", True)
         self.xy_files = kwargs.get("xy_files")
         self.plot_all_stns = kwargs.get("plot_all_stns", True)
 
     def __str__(self):
         """Return short summary string of the Trigger object."""
 
-        out = ("\tTrigger parameters:\n"
-               f"\t\tPre/post pad = {self.pad} s\n"
-               f"\t\tMarginal window = {self.marginal_window} s\n"
-               f"\t\tMinimum event interval  = {self.min_event_interval} s\n\n"
-               f"\t\tTriggering from the ")
+        out = (
+            "\tTrigger parameters:\n"
+            f"\t\tPre/post pad = {self.pad} s\n"
+            f"\t\tMarginal window = {self.marginal_window} s\n"
+            f"\t\tMinimum event interval  = {self.min_event_interval} s\n\n"
+            f"\t\tTriggering from the "
+        )
         out += "normalised " if self.normalise_coalescence else ""
         out += "maximum coalescence trace.\n\n"
         out += f"\t\tTrigger threshold method: {self.threshold_method}\n"
         if self.threshold_method == "static":
             out += f"\t\tStatic threshold = {self.static_threshold}\n"
         elif self.threshold_method == "dynamic":
-            out += (f"\t\tMAD Window     = {self.mad_window_length}\n"
-                    f"\t\tMAD Multiplier = {self.mad_multiplier}\n")
+            out += (
+                f"\t\tMAD Window     = {self.mad_window_length}\n"
+                f"\t\tMAD Multiplier = {self.mad_multiplier}\n"
+            )
 
         return out
 
     def trigger(self, starttime, endtime, region=None, interactive_plot=False):
         """
         Trigger candidate earthquakes from decimated scan data.
 
@@ -210,16 +237,16 @@
         starttime : str
             Timestamp from which to trigger events.
         endtime : str
             Timestamp up to which to trigger events.
         region : list of floats, optional
             Only retain triggered events located within this region. Format is:
                 [Xmin, Ymin, Zmin, Xmax, Ymax, Zmax]
-            As longitude / latitude / depth (units corresponding to the lookup
-            table grid projection; in positive-down frame).
+            As longitude / latitude / depth (units corresponding to the lookup table
+            grid projection; in positive-down frame).
         interactive_plot : bool, optional
             Toggles whether to produce an interactive plot. Default: False.
 
         Raises
         ------
         TimeSpanException
             If `starttime` is after `endtime`.
@@ -255,135 +282,146 @@
         batchstart : `obspy.UTCDateTime` object
             Timestamp from which to trigger events.
         batchend : `obspy.UTCDateTime` object
             Timestamp up to which to trigger events.
         region : list of floats
             Only retain triggered events located within this region. Format is:
                 [Xmin, Ymin, Zmin, Xmax, Ymax, Zmax]
-            As longitude / latitude / depth (units corresponding to the lookup
-            table grid projection; in positive-down frame).
+            As longitude / latitude / depth (units corresponding to the lookup table
+            grid projection; in positive-down frame).
         interactive_plot : bool
             Toggles whether to produce an interactive plot. Default: False.
 
         """
 
         logging.info("\tReading in .scanmseed...")
-        data, stats = read_scanmseed(self.run, batchstart, batchend, self.pad,
-                                     self.lut.unit_conversion_factor)
+        data, stats = read_scanmseed(
+            self.run, batchstart, batchend, self.pad, self.lut.unit_conversion_factor
+        )
 
         logging.info("\n\tTriggering events...")
         trigger_on = "COA_N" if self.normalise_coalescence else "COA"
         threshold = self._get_threshold(data[trigger_on], stats.sampling_rate)
-        candidate_events = self._identify_candidates(data, trigger_on,
-                                                     threshold)
+        candidate_events = self._identify_candidates(data, trigger_on, threshold)
 
         if candidate_events.empty:
-            logging.info("\tNo events triggered at this threshold - try a "
-                         "lower detection threshold.")
+            logging.info(
+                "\tNo events triggered at this threshold - try a lower detection "
+                "threshold."
+            )
             events = candidate_events
             discarded = candidate_events
         else:
             refined_events = self._refine_candidates(candidate_events)
             logging.debug(refined_events)
-            events = self._filter_events(refined_events, batchstart, batchend,
-                                         region)
+            events = self._filter_events(refined_events, batchstart, batchend, region)
             logging.debug(events)
-            discarded = refined_events[~refined_events.index.isin(events.index)].dropna()
+            discarded = refined_events[
+                ~refined_events.index.isin(events.index)
+            ].dropna()
             logging.debug(discarded)
-            logging.info(f"\n\t\t{len(events)} event(s) triggered within the "
-                         f"specified region between {batchstart} \n\t\tand "
-                         f"{batchend}")
+            logging.info(
+                f"\n\t\t{len(events)} event(s) triggered within the specified region "
+                f"between {batchstart} \n\t\tand {batchend}"
+            )
             logging.info("\n\tWriting triggered events to file...")
             write_triggered_events(self.run, events, batchstart)
 
         if self.plot_trigger_summary:
             logging.info("\n\tPlotting trigger summary...")
-            trigger_summary(events, batchstart, batchend, self.run,
-                            self.marginal_window, self.min_event_interval,
-                            threshold, self.normalise_coalescence, self.lut,
-                            data, region, discarded,
-                            interactive=interactive_plot,
-                            xy_files=self.xy_files,
-                            plot_all_stns=self.plot_all_stns)
+            trigger_summary(
+                events,
+                batchstart,
+                batchend,
+                self.run,
+                self.marginal_window,
+                self.min_event_interval,
+                threshold,
+                self.normalise_coalescence,
+                self.lut,
+                data,
+                region,
+                discarded,
+                interactive=interactive_plot,
+                xy_files=self.xy_files,
+                plot_all_stns=self.plot_all_stns,
+            )
 
     @util.timeit()
     def _get_threshold(self, scandata, sampling_rate):
         """
         Determine the threshold to use when triggering candidate events.
 
         Parameters
         ----------
         scandata : `pandas.Series` object
-            (Normalised) coalescence values for which to calculate the
-            threshold.
+            (Normalised) coalescence values for which to calculate the threshold.
         sampling_rate : int
             Number of samples per second of the coalescence scan data.
 
         Returns
         -------
         threshold : `numpy.ndarray` object
             Array of threshold values.
 
         """
 
         if self.threshold_method == "dynamic":
             # Split the data in window_length chunks
             breaks = np.arange(len(scandata))
-            breaks = breaks[breaks % int(self.mad_window_length
-                                         * sampling_rate) == 0][1:]
+            breaks = breaks[breaks % int(self.mad_window_length * sampling_rate) == 0][
+                1:
+            ]
             chunks = np.split(scandata.values, breaks)
 
             # Calculate the mad and median values
-            mad_values = \
-                np.asarray([util.calculate_mad(chunk) for chunk in chunks])
+            mad_values = np.asarray([util.calculate_mad(chunk) for chunk in chunks])
             median_values = np.asarray([np.median(chunk) for chunk in chunks])
             mad_trace = chunks2trace(mad_values, (len(chunks), len(chunks[0])))
-            median_trace = chunks2trace(median_values, (len(chunks),
-                                                        len(chunks[0])))
-            mad_trace = mad_trace[:len(scandata)]
-            median_trace = median_trace[:len(scandata)]
+            median_trace = chunks2trace(median_values, (len(chunks), len(chunks[0])))
+            mad_trace = mad_trace[: len(scandata)]
+            median_trace = median_trace[: len(scandata)]
 
             # Set the dynamic threshold
             threshold = median_trace + (mad_trace * self.mad_multiplier)
         else:
             # Set static threshold
             threshold = np.zeros_like(scandata) + self.static_threshold
 
         return threshold
 
     @util.timeit()
     def _identify_candidates(self, scandata, trigger_on, threshold):
         """
-        Identify distinct periods of time for which the maximum (normalised)
-        coalescence trace exceeds the chosen threshold.
+        Identify distinct periods of time for which the maximum (normalised) coalescence
+        trace exceeds the chosen threshold.
 
         Parameters
         ----------
         scandata : `pandas.DataFrame` object
             Data output by detect() -- decimated scan.
             Columns: ["DT", "COA", "COA_N", "X", "Y", "Z"] - X/Y/Z as lon/lat/
-            z-units corresponding to the units of the lookup table grid
-            projection.
+            z-units corresponding to the units of the lookup table grid projection.
         trigger_on : str
             Specifies the maximum coalescence data on which to trigger events.
         threshold : `numpy.ndarray` object
             Array of threshold values.
 
         Returns
         -------
         triggers : `pandas.DataFrame` object
-            Candidate events exceeding some threshold. Columns: ["EventNum",
-            "CoaTime", "TRIG_COA", "COA_X", "COA_Y", "COA_Z", "MinTime",
-            "MaxTime", "COA", "COA_NORM"]
+            Candidate events exceeding some threshold. Columns: ["EventNum", "CoaTime",
+            "TRIG_COA", "COA_X", "COA_Y", "COA_Z", "MinTime",  "MaxTime", "COA",
+            "COA_NORM"]
 
         """
 
-        # Switch between user-facing minimum event interval definition (minimum
-        # interval between event triggers) and internal definition (extra
-        # buffer on top of marginal window within which events cannot overlap)
+        # Switch between user-facing minimum event interval definition (minimum interval
+        # between event triggers) and internal definition (extra buffer on top of
+        # marginal window within which events cannot overlap)
         min_event_interval = self.min_event_interval - self.marginal_window
 
         thresholded = scandata[scandata[trigger_on] >= threshold]
         r = np.arange(len(thresholded))
         candidates = [d for _, d in thresholded.groupby(thresholded.index - r)]
 
         triggers = pd.DataFrame(columns=CANDIDATES_COLS)
@@ -400,158 +438,174 @@
             # If last sample above threshold is within the marginal window
             if (candidate["DT"].iloc[-1] - peak["DT"]) < self.marginal_window:
                 max_dt = peak["DT"] + self.min_event_interval
             # Otherwise just add the minimum event interval
             else:
                 max_dt = candidate["DT"].iloc[-1] + min_event_interval
 
-            trigger = pd.Series([i, peak["DT"], peak[trigger_on],
-                                 peak["X"], peak["Y"], peak["Z"],
-                                 min_dt, max_dt, peak["COA"], peak["COA_N"]],
-                                index=CANDIDATES_COLS)
-
-            triggers = pd.concat([triggers, trigger.to_frame().T.convert_dtypes()],
-                                 ignore_index=True)
+            trigger = pd.Series(
+                [
+                    i,
+                    peak["DT"],
+                    peak[trigger_on],
+                    peak["X"],
+                    peak["Y"],
+                    peak["Z"],
+                    min_dt,
+                    max_dt,
+                    peak["COA"],
+                    peak["COA_N"],
+                ],
+                index=CANDIDATES_COLS,
+            )
+
+            triggers = pd.concat(
+                [triggers, trigger.to_frame().T.convert_dtypes()], ignore_index=True
+            )
 
         return triggers
 
     @util.timeit()
     def _refine_candidates(self, candidate_events):
         """
-        Merge candidate events for which the marginal windows overlap with the
-        minimum inter-event time.
+        Merge candidate events for which the marginal windows overlap with the minimum
+        inter-event time.
 
         Parameters
         ----------
         candidate_events : `pandas.DataFrame` object
             Candidate events corresponding to periods of time in which the
-            coalescence signal exceeds some threshold. Columns: ["EventNum",
-            "CoaTime", "TRIG_COA", "COA_X", "COA_Y", "COA_Z", "MinTime",
-            "MaxTime", "COA", "COA_NORM"]
+            coalescence signal exceeds some threshold. Columns: ["EventNum", "CoaTime",
+            "TRIG_COA", "COA_X", "COA_Y", "COA_Z", "MinTime", "MaxTime", "COA",
+            "COA_NORM"]
 
         Returns
         -------
         events : `pandas.DataFrame` object
             Merged events with some minimum inter-event spacing in time.
-            Columns: ["EventID", "CoaTime", "TRIG_COA", "COA_X", "COA_Y",
-                       "COA_Z", "MinTime", "MaxTime", "COA", "COA_NORM"].
+            Columns: ["EventID", "CoaTime", "TRIG_COA", "COA_X", "COA_Y", "COA_Z",
+            "MinTime", "MaxTime", "COA", "COA_NORM"].
 
         """
 
-        # Iterate pairwise (event1, event2) over the candidate events to
-        # identify overlaps between:
+        # Iterate pairwise (event1, event2) over the candidate events to identify
+        # overlaps between:
         #   - event1 marginal window and event2 minimum window position
         #   - event2 marginal window and event1 maximum window position
         event_count = 1
         for i, event1 in candidate_events.iterrows():
             candidate_events.loc[i, "EventNum"] = event_count
             if i + 1 == len(candidate_events):
                 continue
-            event2 = candidate_events.iloc[i+1]
-            if all([event1["MaxTime"] < \
-                        event2["CoaTime"] - self.marginal_window,
-                    event2["MinTime"] > \
-                        event1["CoaTime"] + self.marginal_window]):
+            event2 = candidate_events.iloc[i + 1]
+            if all(
+                [
+                    event1["MaxTime"] < event2["CoaTime"] - self.marginal_window,
+                    event2["MinTime"] > event1["CoaTime"] + self.marginal_window,
+                ]
+            ):
                 event_count += 1
 
         # Split into DataFrames by event number
-        merged_candidates = [d for _, d in candidate_events.groupby(
-            candidate_events["EventNum"])]
+        merged_candidates = [
+            d for _, d in candidate_events.groupby(candidate_events["EventNum"])
+        ]
 
         # Update the min/max window times and build final event DataFrame
         refined_events = pd.DataFrame(columns=REFINED_EVENTS_COLS)
         for i, candidate in enumerate(merged_candidates):
-            logging.debug(f"\t    Triggered event {i+1} of "
-                          f"{len(merged_candidates)}")
+            logging.debug(f"\t    Triggered event {i+1} of {len(merged_candidates)}")
             event = candidate.loc[candidate["TRIG_COA"].idxmax()].copy()
             event["MinTime"] = candidate["MinTime"].min()
             event["MaxTime"] = candidate["MaxTime"].max()
 
             # Add unique identifier
             event_uid = str(event["CoaTime"])
             for char_ in ["-", ":", ".", " ", "Z", "T"]:
                 event_uid = event_uid.replace(char_, "")
             event_uid = event_uid[:17].ljust(17, "0")
             event["EventID"] = event_uid
 
-            refined_events = pd.concat([refined_events,
-                                        event.to_frame().T.convert_dtypes()],
-                                       ignore_index=True)
+            refined_events = pd.concat(
+                [refined_events, event.to_frame().T.convert_dtypes()], ignore_index=True
+            )
 
         return refined_events
 
     @util.timeit()
     def _filter_events(self, events, starttime, endtime, region):
         """
-        Remove events within the padding time and/or within a specific
-        geographical region. Also adds a unique event identifier based on the
-        coalescence time.
+        Remove events within the padding time and/or within a specific geographical
+        region. Also adds a unique event identifier based on the coalescence time.
 
         Parameters
         ----------
         events : `pandas.DataFrame` object
-            Refined set of events to be filtered. Columns: ["EventID",
-            "CoaTime", "TRIG_COA", "COA_X", "COA_Y", "COA_Z", "MinTime",
-            "MaxTime", "COA", "COA_NORM"].
+            Refined set of events to be filtered. Columns: ["EventID", "CoaTime",
+            "TRIG_COA", "COA_X", "COA_Y", "COA_Z", "MinTime", "MaxTime", "COA",
+            "COA_NORM"].
         starttime : `obspy.UTCDateTime` object
             Timestamp from which to trigger events.
         endtime : `obspy.UTCDateTime` object
             Timestamp up to which to trigger events.
         region : list of floats
             Only retain triggered events located within this region. Format is:
                 [Xmin, Ymin, Zmin, Xmax, Ymax, Zmax]
-            As longitude / latitude / depth (units corresponding to the lookup
-            table grid projection; in positive-down frame).
+            As longitude / latitude / depth (units corresponding to the lookup table
+            grid projection; in positive-down frame).
 
         Returns
         -------
         events : `pandas.DataFrame` object
-            Final set of triggered events. Columns: ["EventID", "CoaTime",
-            "TRIG_COA", "COA_X", "COA_Y", "COA_Z", "MinTime", "MaxTime", "COA",
-            "COA_NORM"].
+            Final set of triggered events. Columns: ["EventID", "CoaTime", "TRIG_COA",
+            "COA_X", "COA_Y", "COA_Z", "MinTime", "MaxTime", "COA", "COA_NORM"].
 
         """
 
         # Remove events which occur in the pre-pad and post-pad:
-        events = events.loc[(events["CoaTime"] >= starttime) &
-                            (events["CoaTime"] < endtime), :].copy()
+        events = events.loc[
+            (events["CoaTime"] >= starttime) & (events["CoaTime"] < endtime), :
+        ].copy()
 
         if region is not None:
-            events = events.loc[(events["COA_X"] >= region[0]) &
-                                (events["COA_Y"] >= region[1]) &
-                                (events["COA_Z"] >= region[2]) &
-                                (events["COA_X"] <= region[3]) &
-                                (events["COA_Y"] <= region[4]) &
-                                (events["COA_Z"] <= region[5]), :].copy()
+            events = events.loc[
+                (events["COA_X"] >= region[0])
+                & (events["COA_Y"] >= region[1])
+                & (events["COA_Z"] >= region[2])
+                & (events["COA_X"] <= region[3])
+                & (events["COA_Y"] <= region[4])
+                & (events["COA_Z"] <= region[5]),
+                :,
+            ].copy()
 
         return events
 
     @property
     def min_event_interval(self):
         """Get and set the minimum event interval."""
 
         return self._min_event_interval
 
     @min_event_interval.setter
     def min_event_interval(self, value):
         if value < 2 * self.marginal_window:
-            msg = "\tMinimum event interval must be >= 2 * marginal window."
-            raise ValueError(msg)
+            raise ValueError("\tMinimum event interval must be >= 2 * marginal window.")
         else:
             self._min_event_interval = value
 
     # --- Deprecation/Future handling ---
     @property
     def minimum_repeat(self):
         """Handler for deprecated attribute name 'minimum_repeat'."""
 
         return self._min_event_interval
 
     @minimum_repeat.setter
     def minimum_repeat(self, value):
         if value < 2 * self.marginal_window:
-            msg = "\tMinimum repeat must be >= 2 * marginal window."
-            raise ValueError(msg)
-        print("FutureWarning: Parameter name has changed - continuing.")
-        print("To remove this message, change:")
-        print("\t'minimum_repeat' -> 'min_event_interval'")
+            raise ValueError("\tMinimum repeat must be >= 2 * marginal window.")
+        print(
+            "FutureWarning: Parameter name has changed - continuing.\n"
+            "To remove this message, change:\n"
+            "\t'minimum_repeat' -> 'min_event_interval'"
+        )
         self._min_event_interval = value
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quakemigrate-1.0.1/quakemigrate/util.py` & `quakemigrate-1.0.2/quakemigrate/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 Module that supplies various utility functions and classes.
 
 :copyright:
-    2020 - 2021, QuakeMigrate developers.
+    2020–2023, QuakeMigrate developers.
 :license:
     GNU General Public License, Version 3
     (https://www.gnu.org/licenses/gpl-3.0.html)
 
 """
 
 import logging
@@ -19,15 +19,15 @@
 from itertools import tee
 
 import matplotlib.ticker as ticker
 import numpy as np
 from obspy import Trace, Stream
 
 
-log_spacer = "="*110
+log_spacer = "=" * 110
 
 
 def make_directories(run, subdir=None):
     """
     Make run directory, and optionally make subdirectories within it.
 
     Parameters
@@ -49,48 +49,48 @@
 def gaussian_1d(x, a, b, c):
     """
     Create a 1-dimensional Gaussian function.
 
     Parameters
     ----------
     x : array-like
-        Array of x values
+        Array of x values.
     a : float / int
-        Amplitude (height of Gaussian)
+        Amplitude (height of Gaussian).
     b : float / int
-        Mean (centre of Gaussian)
+        Mean (centre of Gaussian).
     c : float / int
-        Sigma (width of Gaussian)
+        Sigma (width of Gaussian).
 
     Returns
     -------
     f : function
         1-dimensional Gaussian function
 
     """
 
-    f = a * np.exp(-1. * ((x - b) ** 2) / (2 * (c ** 2)))
+    f = a * np.exp(-1.0 * ((x - b) ** 2) / (2 * (c**2)))
 
     return f
 
 
 def gaussian_3d(nx, ny, nz, sgm):
     """
     Create a 3-dimensional Gaussian function.
 
     Parameters
     ----------
     nx : array-like
-        Array of x values
+        Array of x values.
     ny : array-like
-        Array of y values
+        Array of y values.
     nz : array-like
-        Array of z values
+        Array of z values.
     sgm : float / int
-        Sigma (width of gaussian in all directions)
+        Sigma (width of gaussian in all directions).
 
     Returns
     -------
     f : function
         3-dimensional Gaussian function
 
     """
@@ -103,17 +103,19 @@
     z = np.linspace(-nz2, nz2, nz)
     ix, iy, iz = np.meshgrid(x, y, z, indexing="ij")
 
     if np.isscalar(sgm):
         sgm = np.repeat(sgm, 3)
     sx, sy, sz = sgm
 
-    f = np.exp(- (ix * ix) / (2 * sx * sx)
-               - (iy * iy) / (2 * sy * sy)
-               - (iz * iz) / (2 * sz * sz))
+    f = np.exp(
+        -(ix * ix) / (2 * sx * sx)
+        - (iy * iy) / (2 * sy * sy)
+        - (iz * iz) / (2 * sz * sz)
+    )
 
     return f
 
 
 def logger(logstem, log, loglevel="info"):
     """
     Simple logger that will output to both a log file and stdout.
@@ -122,78 +124,75 @@
     ----------
     logstem : str
         Filestem for log file.
     log : bool
         Toggle for logging - default is to only print information to stdout.
         If True, will also create a log file.
     loglevel : str, optional
-        Toggle for logging level - default is to print only "info" messages to
-        log. To print more detailed "debug" messages, set to "debug".
+        Toggle for logging level - default is to print only "info" messages to log.
+        To print more detailed "debug" messages, set to "debug".
 
     """
 
     level = logging.DEBUG if loglevel == "debug" else logging.INFO
 
     if log:
         now = datetime.now().strftime("%Y-%m-%d_%H-%M-%S")
         logfile = logstem.parent / f"{logstem.name}_{now}"
         logfile.parent.mkdir(exist_ok=True, parents=True)
-        handlers = [logging.FileHandler(str(logfile.with_suffix(".log"))),
-                    logging.StreamHandler(sys.stdout)]
+        handlers = [
+            logging.FileHandler(str(logfile.with_suffix(".log"))),
+            logging.StreamHandler(sys.stdout),
+        ]
     else:
         handlers = [logging.StreamHandler(sys.stdout)]
 
-    logging.basicConfig(level=level,
-                        format="%(message)s",
-                        handlers=handlers)
-                        # format="%(asctime)s [%(levelname)s] %(message)s",
+    logging.basicConfig(level=level, format="%(message)s", handlers=handlers)
 
 
 def time2sample(time, sampling_rate):
     """
-    Utility function to convert from seconds and sampling rate to number of
-    samples.
+    Utility function to convert from seconds and sampling rate to number of samples.
 
     Parameters
     ----------
     time : float
-        Time to convert
+        Time to convert.
     sampling_rate : int
-        Sampling rate of input data/sampling rate at which to compute
-        the coalescence function.
+        Sampling rate of input data/sampling rate at which to compute the coalescence
+        function.
 
     Returns
     -------
     out : int
-        Time that correpsonds to an integer number of samples at a specific
-        sampling rate.
+        Time that correpsonds to an integer number of samples at a specific sampling
+        rate.
 
     """
 
-    return int(round(time*int(sampling_rate)))
+    return int(round(time * int(sampling_rate)))
 
 
 def calculate_mad(x, scale=1.4826):
     """
     Calculates the Median Absolute Deviation (MAD) of the input array x.
 
     Parameters
     ----------
     x : array-like
         Input data.
     scale : float, optional
-        A scaling factor for the MAD output to make the calculated MAD factor
-        a consistent estimation of the standard deviation of the distribution.
+        A scaling factor for the MAD output to make the calculated MAD factor a
+        consistent estimation of the standard deviation of the distribution.
 
     Returns
     -------
     scaled_mad : array-like
-        Array of scaled mean absolute deviation values for the input array, x,
-        scaled to provide an estimation of the standard deviation of the
-        distribution.
+        Array of scaled mean absolute deviation values for the input array, x, scaled
+        to provide an estimation of the standard deviation of the distribution.
 
     """
 
     x = np.asarray(x)
 
     if not x.size:
         return np.nan
@@ -206,238 +205,242 @@
     mad = np.median(np.abs(x - med), axis=0)
 
     return scale * mad
 
 
 class DateFormatter(ticker.Formatter):
     """
-    Extend the `matplotlib.ticker.Formatter` class to allow for millisecond
-    precision when formatting a tick (in days since the epoch) with a
-    `datetime.datetime.strftime` format string.
+    Extend the `matplotlib.ticker.Formatter` class to allow for millisecond precision
+    when formatting a tick (in days since the epoch) with a `datetime.datetime.strftime`
+    format string.
+
+    Parameters
+    ----------
+    fmt : str
+        `datetime.datetime.strftime` format string.
+    precision : int
+        Degree of precision to which to report sub-second time intervals.
 
     """
 
     def __init__(self, fmt, precision=3):
-        """
-        Parameters
-        ----------
-        fmt : str
-            `datetime.datetime.strftime` format string.
-        precision : int
-            Degree of precision to which to report sub-second time intervals.
-
-        """
+        """Instantiate the DateFormatter object."""
 
         from matplotlib.dates import num2date
 
         self.num2date = num2date
         self.fmt = fmt
         self.precision = precision
 
     def __call__(self, x, pos=0):
         if x == 0:
-            raise ValueError("DateFormatter found a value of x=0, which is "
-                             "an illegal date; this usually occurs because "
-                             "you have not informed the axis that it is "
-                             "plotting dates, e.g., with ax.xaxis_date()")
+            raise ValueError(
+                "DateFormatter found a value of x=0, which is an illegal date; this "
+                "usually occurs because you have not informed the axis that it is "
+                "plotting dates, e.g., with 'ax.xaxis_date()'"
+            )
 
         dt = self.num2date(x)
-        ms = dt.strftime("%f")[:self.precision]
+        ms = dt.strftime("%f")[: self.precision]
 
         return dt.strftime(self.fmt).format(ms=ms)
 
 
 def trim2sample(time, sampling_rate):
     """
-    Utility function to ensure time padding results in a time that is an
-    integer number of samples.
+    Utility function to ensure time padding results in a time that is an integer number
+    of samples.
 
     Parameters
     ----------
     time : float
         Time to trim.
     sampling_rate : int
-        Sampling rate of input data/sampling rate at which to compute
-        the coalescence function.
+        Sampling rate of input data/sampling rate at which to compute the coalescence
+        function.
 
     Returns
     -------
     out : int
-        Time that correpsonds to an integer number of samples at a specific
-        sampling rate.
+        Time that correpsonds to an integer number of samples at a specific sampling
+        rate.
 
     """
 
     return int(np.ceil(time * sampling_rate) / sampling_rate * 1000) / 1000
 
 
-def wa_response(convert='DIS2DIS', obspy_def=True):
+def wa_response(convert="DIS2DIS", obspy_def=True):
     """
     Generate a Wood Anderson response dictionary.
 
     Parameters
     ----------
-    convert : {'DIS2DIS', 'VEL2VEL', ‘VEL2DIS'}
-        Type of output to convert between; determines the number of complex
-        zeros used.
+    convert : {'DIS2DIS', 'VEL2VEL', 'VEL2DIS'}
+        Type of output to convert between; determines the number of complex zeros used.
     obspy_def : bool, optional
         Use the ObsPy definition of the Wood Anderson response (Default).
         Otherwise, use the IRIS/SAC definition.
 
     Returns
     -------
     WOODANDERSON : dict
-        Poles, zeros, sensitivity and gain of the Wood-Anderson torsion
-        seismograph.
+        Poles, zeros, sensitivity and gain of the Wood-Anderson torsion seismograph.
 
     """
 
     if obspy_def:
         # Create Wood-Anderson response - ObsPy values
-        woodanderson = {"poles": [-6.283185 - 4.712j,
-                                  -6.283185 + 4.712j],
-                        "zeros": [0j],
-                        "sensitivity": 2080,
-                        "gain": 1.}
+        woodanderson = {
+            "poles": [-6.283185 - 4.712j, -6.283185 + 4.712j],
+            "zeros": [0j],
+            "sensitivity": 2080,
+            "gain": 1.0,
+        }
     else:
         # Create Wood Anderson response - different to the ObsPy values
         # http://www.iris.washington.edu/pipermail/sac-help/2013-March/001430.html
-        woodanderson = {"poles": [-5.49779 + 5.60886j,
-                                  -5.49779 - 5.60886j],
-                        "zeros": [0j],
-                        "sensitivity": 2080,
-                        "gain": 1.}
+        woodanderson = {
+            "poles": [-5.49779 + 5.60886j, -5.49779 - 5.60886j],
+            "zeros": [0j],
+            "sensitivity": 2080,
+            "gain": 1.0,
+        }
 
-    if convert in ('DIS2DIS', 'VEL2VEL'):
+    if convert in ("DIS2DIS", "VEL2VEL"):
         # Add an extra zero to go from disp to disp or vel to vel.
-        woodanderson['zeros'].extend([0j])
+        woodanderson["zeros"].extend([0j])
 
     return woodanderson
 
 
 def shift_to_sample(stream, interpolate=False):
     """
-    Check whether any data in an `obspy.Stream` object is "off-sample" - i.e.
-    the data timestamps are *not* an integer number of samples after midnight.
-    If so, shift data to be "on-sample".
-
-    This can either be done by shifting the timestamps by a sub-sample time
-    interval, or interpolating the trace to the "on-sample" timestamps. The
-    latter has the benefit that it will not affect the timing of the data, but
-    will require additional computation time and some inevitable edge effects -
-    though for onset calculation these should be contained within the pad
-    windows. If you are using a sampling rate < 10 Hz, contact the QuakeMigrate
-    developers.
+    Check whether any data in an `obspy.Stream` object is "off-sample" - i.e. the data
+    timestamps are *not* an integer number of samples after midnight. If so, shift data
+    to be "on-sample".
+
+    This can either be done by shifting the timestamps by a sub-sample time interval, or
+    interpolating the trace to the "on-sample" timestamps. The latter has the benefit
+    that it will not affect the timing of the data, but will require additional
+    computation time and some inevitable edge effects - though for onset calculation
+    these should be contained within the pad windows. If you are using a sampling
+    rate < 10 Hz, contact the QuakeMigrate developers.
 
     Parameters
     ----------
     stream : `obspy.Stream` object
         Contains list of `obspy.Trace` objects for which to check the timing.
     interpolate : bool, optional
-        Whether to interpolate the data to correct the "off-sample" timing.
-        Otherwise, the metadata will simply be altered to shift the timestamps
-        "on-sample"; this will lead to a sub-sample timing offset.
+        Whether to interpolate the data to correct the "off-sample" timing. Otherwise,
+        the metadata will simply be altered to shift the timestamps "on-sample"; this
+        will lead to a sub-sample timing offset.
 
     Returns
     -------
     stream : `obspy.Stream` object
         Waveform data with all timestamps "on-sample".
 
     """
 
     # work on a copy
     stream = stream.copy()
 
     for tr in stream:
-        # Check if microsecond is divisible by sampling rate; only guaranteed
-        # to work for sampling rates of 1 Hz or less
-        delta = tr.stats.starttime.microsecond \
-            % (1e6 / tr.stats.sampling_rate)
+        # Check if microsecond is divisible by sampling rate; only guaranteed to work
+        # for sampling rates of 1 Hz or less
+        delta = tr.stats.starttime.microsecond % (1e6 / tr.stats.sampling_rate)
         if delta == 0:
-            if tr.stats.sampling_rate < 1.:
-                logging.warning(f"Trace\n\t{tr}\nhas a sampling rate less than"
-                                " 1 Hz, so off-sample data might not be "
-                                "corrected!")
+            if tr.stats.sampling_rate < 1.0:
+                logging.warning(
+                    f"Trace\n\t{tr}\nhas a sampling rate less than 1 Hz, so off-sample "
+                    "data might not be corrected!"
+                )
             continue
         else:
             # Calculate time shift to closest "on-sample" timestamp
-            time_shift = round(delta / 1e6 * tr.stats.sampling_rate) \
-                / tr.stats.sampling_rate - delta / 1e6
+            time_shift = (
+                round(delta / 1e6 * tr.stats.sampling_rate) / tr.stats.sampling_rate
+                - delta / 1e6
+            )
             if not interpolate:
-                logging.info(f"Trace\n\t{tr}\nhas off-sample data. Applying "
-                             f"{time_shift:+f} s shift to timing.")
+                logging.info(
+                    f"Trace\n\t{tr}\nhas off-sample data. Applying "
+                    f"{time_shift:+f} s shift to timing."
+                )
                 tr.stats.starttime += time_shift
                 logging.debug(f"Shifted trace: {tr}")
             else:
-                logging.info(f"Trace\n\t{tr}\nhas off-sample data. "
-                             f"Interpolating to apply a {time_shift:+f} s "
-                             "shift to timing.")
-                # Interpolate can only map between values contained within the
-                # original array. For negative time shift, shift by one sample
-                # so new starttime is within original array, and add constant
-                # value pad after interpolation.
+                logging.info(
+                    f"Trace\n\t{tr}\nhas off-sample data. "
+                    f"Interpolating to apply a {time_shift:+f} s "
+                    "shift to timing."
+                )
+                # Interpolate can only map between values contained within the original
+                # array. For negative time shift, shift by one sample so new starttime
+                # is within original array, and add constant value pad after
+                # interpolation.
                 new_starttime = tr.stats.starttime + time_shift
-                if time_shift < 0.:
+                if time_shift < 0.0:
                     new_starttime += tr.stats.delta
-                tr.interpolate(sampling_rate=tr.stats.sampling_rate,
-                               method="lanczos", a=20, starttime=new_starttime)
-                # Add constant-value pad at end if time_shift is positive,
-                # (last sample is dropped when interpolating for positive time
-                # shifts), else at start. If adding at start, also adjust start
-                # time.
-                if time_shift > 0.:
+                tr.interpolate(
+                    sampling_rate=tr.stats.sampling_rate,
+                    method="lanczos",
+                    a=20,
+                    starttime=new_starttime,
+                )
+                # Add constant-value pad at end if time_shift is positive, (last sample
+                # is dropped when interpolating for positive time shifts), else at
+                # start. If adding at start, also adjust start time.
+                if time_shift > 0.0:
                     tr.data = np.append(tr.data, tr.data[-1])
                 else:
                     tr.data = np.append(tr.data[0], tr.data)
                     tr.stats.starttime -= tr.stats.delta
                 logging.debug(f"Interpolated tr:\n\t{tr}")
 
     return stream
 
 
 def resample(stream, sampling_rate, resample, upfactor, starttime, endtime):
     """
     Resample data in an `obspy.Stream` object to the specified sampling rate.
 
-    By default, this function will only perform decimation of the data. If
-    necessary, and if the user specifies `resample = True` and an upfactor
-    to upsample by `upfactor = int`, data can also be upsampled and then,
-    if necessary, subsequently decimated to achieve the desired sampling
-    rate.
-
-    For example, for raw input data sampled at a mix of 40, 50 and 100 Hz,
-    to achieve a unified sampling rate of 50 Hz, the user would have to
-    specify an upfactor of 5; 40 Hz x 5 = 200 Hz, which can then be
-    decimated to 50 Hz.
+    By default, this function will only perform decimation of the data. If necessary,
+    and if the user specifies `resample = True` and an upfactor to upsample by
+    `upfactor = int`, data can also be upsampled and then, if necessary, subsequently
+    decimated to achieve the desired sampling rate.
+
+    For example, for raw input data sampled at a mix of 40, 50 and 100 Hz, to achieve a
+    unified sampling rate of 50 Hz, the user would have to specify an upfactor of 5;
+    40 Hz x 5 = 200 Hz, which can then be decimated to 50 Hz.
 
     NOTE: assumes any data with off-sample timing has been corrected with
-    :func:`~quakemigrate.util.shift_to_sample`. If not, the resulting traces
-    may not all contain the correct number of samples.
+    :func:`~quakemigrate.util.shift_to_sample`. If not, the resulting traces may not all
+    contain the correct number of samples.
 
-    NOTE: data will be detrended and a cosine taper applied before
-    decimation, in order to avoid edge effects when applying the lowpass
-    filter.
+    NOTE: data will be detrended and a cosine taper applied before decimation, in order
+    to avoid edge effects when applying the lowpass filter.
 
     Parameters
     ----------
     stream : `obspy.Stream` object
         Contains list of `obspy.Trace` objects to be decimated / resampled.
     resample : bool
-        If true, perform resampling of data which cannot be decimated
-        directly to the desired sampling rate.
+        If true, perform resampling of data which cannot be decimated directly to the
+        desired sampling rate.
     upfactor : int or None
-        Factor by which to upsample the data to enable it to be decimated
-        to the desired sampling rate, e.g. 40Hz -> 50Hz requires
-        upfactor = 5.
+        Factor by which to upsample the data to enable it to be decimated to the desired
+        sampling rate, e.g. 40Hz -> 50Hz requires upfactor = 5.
 
     Returns
     -------
     stream : `obspy.Stream` object
-        Contains list of resampled `obspy.Trace` objects at the chosen
-        sampling rate `sr`.
+        Contains list of resampled `obspy.Trace` objects at the chosen sampling rate
+        `sr`.
 
     """
 
     # Work on a copy of the stream
     stream = stream.copy()
 
     for trace in stream:
@@ -453,35 +456,36 @@
                     raise BadUpfactorException(trace)
                 stream.remove(trace)
                 trace = upsample(trace, upfactor, starttime, endtime)
                 if trace_sampling_rate != sampling_rate:
                     trace = decimate(trace, sampling_rate)
                 stream += trace
             else:
-                logging.info("Mismatched sampling rates - cannot decimate "
-                             f"data from\n\t{trace}.\n..to resample data, set "
-                             "resample = True and choose a suitable upfactor")
-
-    # Trim as a general safety net. NOTE: here we are using
-    # nearest_sample=False, as all data in the stream should now be at the
-    # desired sampling rate, and with any off-sample data having had it's
-    # timing shifted.
-    stream.trim(starttime=starttime-0.00001, endtime=endtime+0.00001,
-                nearest_sample=False)
+                logging.info(
+                    f"Mismatched sampling rates - cannot decimate data from\n\t{trace}"
+                    "\n...to resample data, set resample = True and choose a suitable "
+                    "upfactor"
+                )
+
+    # Trim as a general safety net. NOTE: here we are using 'nearest_sample=False', as
+    # all data in the stream should now be at the desired sampling rate, and with any
+    # off-sample data having had its timing shifted.
+    stream.trim(
+        starttime=starttime - 0.00001, endtime=endtime + 0.00001, nearest_sample=False
+    )
 
     return stream
 
 
 def decimate(trace, sampling_rate):
     """
     Decimate a trace to achieve the desired sampling rate, sr.
 
-    NOTE: data will be detrended and a cosine taper applied before
-    decimation, in order to avoid edge effects when applying the lowpass
-    filter before decimating.
+    NOTE: data will be detrended and a cosine taper applied before decimation, in order
+    to avoid edge effects when applying the lowpass filter before decimating.
 
     Parameters:
     -----------
     trace : `obspy.Trace` object
         Trace to be decimated.
     sampling_rate : int
         Output sampling rate.
@@ -493,36 +497,39 @@
 
     """
 
     # Work on a copy of the trace
     trace = trace.copy()
 
     # Detrend and apply cosine taper
-    trace.detrend('linear')
-    trace.detrend('demean')
-    trace.taper(type='cosine', max_percentage=0.05)
+    trace.detrend("linear")
+    trace.detrend("demean")
+    trace.taper(type="cosine", max_percentage=0.05)
 
     # Zero-phase Butterworth-lowpass filter at Nyquist frequency
-    trace.filter("lowpass", freq=float(sampling_rate) / 2.000001, corners=2,
-                 zerophase=True)
-    trace.decimate(factor=int(trace.stats.sampling_rate / sampling_rate),
-                   strict_length=False, no_filter=True)
+    trace.filter(
+        "lowpass", freq=float(sampling_rate) / 2.000001, corners=2, zerophase=True
+    )
+    trace.decimate(
+        factor=int(trace.stats.sampling_rate / sampling_rate),
+        strict_length=False,
+        no_filter=True,
+    )
 
     return trace
 
 
 def upsample(trace, upfactor, starttime, endtime):
     """
-    Upsample a data stream by a given factor, prior to decimation. The
-    upsampling is carried out by linear interpolation.
+    Upsample a data stream by a given factor, prior to decimation. The upsampling is
+    carried out by linear interpolation.
 
     NOTE: assumes any data with off-sample timing has been corrected with
-    :func:`~quakemigrate.util.shift_to_sample`. If not, the resulting traces
-    may not all contain the correct number of samples (and desired start
-    and end times).
+    :func:`~quakemigrate.util.shift_to_sample`. If not, the resulting traces may not all
+    contain the correct number of samples (and desired start and end times).
 
     Parameters
     ----------
     trace : `obspy.Trace` object
         Trace to be upsampled.
     upfactor : int
         Factor by which to upsample the data in trace.
@@ -535,75 +542,77 @@
     """
 
     data = trace.data
     # Fenceposts
     dnew = np.zeros((len(data) - 1) * upfactor + 1)
     dnew[::upfactor] = data
     for i in range(1, upfactor):
-        dnew[i::upfactor] = float(i)/upfactor*data[1:] \
-                        + float(upfactor - i)/upfactor*data[:-1]
-
-    # Check if start needs pad - if so pad with constant value (start value
-    # of original trace). Use inequality here to only apply padding to data at
-    # the start and end of the requested time window; not for other traces
-    # floating in the middle (in the case that there are gaps).
-    if 0. < trace.stats.starttime - starttime < trace.stats.delta:
-        logging.debug(f"Mismatched starttimes: {trace.stats.starttime}, "
-                      f"{starttime}")
+        dnew[i::upfactor] = (
+            float(i) / upfactor * data[1:] + float(upfactor - i) / upfactor * data[:-1]
+        )
+
+    # Check if start needs pad - if so pad with constant value (start value of original
+    # trace). Use inequality here to only apply padding to data at the start and end of
+    # the requested time window; not for other traces floating in the middle (in the
+    # case that there are gaps).
+    if 0.0 < trace.stats.starttime - starttime < trace.stats.delta:
+        logging.debug(f"Mismatched starttimes: {trace.stats.starttime}, {starttime}")
         # Calculate how many additional samples are needed
-        start_pad = np.round((trace.stats.starttime - starttime) \
-            * trace.stats.sampling_rate * upfactor)
+        start_pad = np.round(
+            (trace.stats.starttime - starttime) * trace.stats.sampling_rate * upfactor
+        )
         logging.debug(f"Start pad = {start_pad}")
         # Add padding data (constant value)
         start_fill = np.full(int(start_pad), trace.data[0], dtype=int)
         dnew = np.append(start_fill, dnew)
         # Calculate new starttime of trace
-        new_starttime = trace.stats.starttime - start_pad \
-            / (trace.stats.sampling_rate * upfactor)
+        new_starttime = trace.stats.starttime - start_pad / (
+            trace.stats.sampling_rate * upfactor
+        )
         logging.debug(f"New starttime = {new_starttime}")
     else:
         new_starttime = trace.stats.starttime
 
     # Ditto for end of trace
-    if 0. < endtime - trace.stats.endtime < trace.stats.delta:
+    if 0.0 < endtime - trace.stats.endtime < trace.stats.delta:
         logging.debug(f"Mismatched endtimes: {trace.stats.endtime}, {endtime}")
         # Calculate how many additional samples are needed
-        end_pad = np.round((endtime - trace.stats.endtime) \
-            * trace.stats.sampling_rate * upfactor)
+        end_pad = np.round(
+            (endtime - trace.stats.endtime) * trace.stats.sampling_rate * upfactor
+        )
         logging.debug(f"End pad = {end_pad}")
         # Add padding data (constant value)
         end_fill = np.full(int(end_pad), trace.data[-1], dtype=int)
         dnew = np.append(dnew, end_fill)
 
     out = Trace()
     out.data = dnew
     out.stats = trace.stats.copy()
     out.stats.npts = len(out.data)
     out.stats.starttime = new_starttime
     out.stats.sampling_rate = int(upfactor * trace.stats.sampling_rate)
     logging.debug(f"Raw upsampled trace:\n\t{out}")
 
-    # Trim to remove additional padding left from reading with
-    # nearest_sample=True at a variety of sampling rates.
-    # NOTE: here we are using nearest_sample=False, as all data in the stream
-    # should now be at a *multiple* of the desired sampling rate, and with any
-    # off-sample data having had it's timing shifted.
-    out.trim(starttime=starttime-0.00001, endtime=endtime+0.00001,
-             nearest_sample=False)
+    # Trim to remove additional padding left from reading with nearest_sample=True at a
+    # variety of sampling rates. NOTE: here we are using nearest_sample=False, as all
+    # data in the stream should now be at a *multiple* of the desired sampling rate, and
+    # with any off-sample data having had its timing shifted.
+    out.trim(
+        starttime=starttime - 0.00001, endtime=endtime + 0.00001, nearest_sample=False
+    )
     logging.debug(f"Trimmed upsampled trace:\n\t{out}")
 
     return out
 
 
 def merge_stream(stream):
     """
-    Merge all traces with contiguous data, or overlapping data which
-    exactly matches (== st._cleanup(); i.e. no clobber). Apply this on a
-    channel by channel basis so that if any individual merge fails then only
-    that channel will be omitted.
+    Merge all traces with contiguous data, or overlapping data which exactly matches
+    (== st._cleanup(); i.e. no clobber). Apply this on a channel by channel basis so
+    that if any individual merge fails then only that channel will be omitted.
 
     Parameters
     ----------
     stream : `obspy.Stream` object
         Stream to be merged.
 
     Returns
@@ -622,395 +631,374 @@
         warnings.filterwarnings("error")
         for seed_id in seed_ids:
             try:
                 stream_merged += stream.select(id=seed_id).merge(method=-1)
             except UserWarning as error_message:
                 logging.info(f"\t\t{error_message}")
                 logging.info(f"\t\t{stream.select(id=seed_id)}")
-                logging.info(
-                    "\t\tThis channel will not be used for onset calculation."
-                )
+                logging.info("\t\tThis channel will not be used for onset calculation.")
 
     return stream_merged
 
 
 def pairwise(iterable):
     """Utility to iterate over an iterable pairwise."""
 
     a, b = tee(iterable)
     next(b, None)
     return zip(a, b)
 
 
 def timeit(*args_, **kwargs_):
     """Function wrapper that measures the time elapsed during its execution."""
+
     def inner_function(func):
         @wraps(func)
         def wrapper(*args, **kwargs):
             ts = time.time()
             result = func(*args, **kwargs)
-            msg = " "*21 + f"Elapsed time: {time.time() - ts:6f} seconds."
+            msg = " " * 21 + f"Elapsed time: {time.time() - ts:6f} seconds."
             try:
                 if args_[0] == "info":
                     logging.info(msg)
             except IndexError:
                 logging.debug(msg)
             return result
+
         return wrapper
+
     return inner_function
 
 
 class StationFileHeaderException(Exception):
-    """Custom exception to handle incorrect header columns in station file"""
+    """Custom exception to handle incorrect header columns in station file."""
 
     def __init__(self):
-        msg = ("StationFileHeaderException: incorrect station file header - "
-               "use:\nLatitude, Longitude, Elevation, Name")
-        super().__init__(msg)
+        super().__init__(
+            "Incorrect station file header - use:\nLatitude, Longitude, Elevation, Name"
+        )
 
 
 class InvalidVelocityModelHeader(Exception):
-    """Custom exception to handle incorrect header columns in station file"""
+    """Custom exception to handle incorrect header columns in station file."""
 
     def __init__(self, key):
         super().__init__(f"Must include at least '{key}' in header.")
 
 
 class ArchiveFormatException(Exception):
     """Custom exception to handle case where Archive.format is not set."""
 
     def __init__(self):
-        msg = ("ArchiveFormatException: Archive format has not been set. Set "
-               "when making the Archive object with the kwarg "
-               "'archive_format=<path_structure>', or afterwards by using the "
-               "command 'Archive.path_structure(<path_structure>)'. To set a "
-               "custom format, use 'Archive.format = "
-               "custom/archive_{year}_{jday}/{day:02d}.{station}_structure' ")
-        super().__init__(msg)
+        super().__init__(
+            "Archive format has not been set. Set when making the Archive object with "
+            "the kwarg 'archive_format=<path_structure>', or afterwards with the "
+            "command 'Archive.path_structure(<path_structure>)'.\nTo set a custom "
+            "format, use 'Archive.format = "
+            "custom/archive_{year}_{jday}/{day:02d}.{station}_structure'."
+        )
 
 
 class ArchivePathStructureError(Exception):
-    """Custom exception to handle case where an invalid Archive path structure
-    is selected."""
+    """
+    Custom exception to handle case where an invalid Archive path structure is selected.
+    """
 
     def __init__(self, archive_format):
-        msg = ("ArchivePathStructureError: The archive path structure you have"
-               f" selected: '{archive_format}' is not a valid option! See the "
-               "documentation for quakemigrate.data.Archive.path_structure for"
-               " a complete list, or specify a custom format with Archive.form"
-               "at = custom/archive_{year}_{jday}/{day:02d}.{station}_structur"
-               "e")
-        super().__init__(msg)
+        super().__init__(
+            f"The archive path structure you have selected: '{archive_format}' is not "
+            "a valid option! See the documentation for "
+            "'quakemigrate.data.Archive.path_structure' for a complete list, or specify"
+            " a custom format with 'Archive.format = "
+            "custom/archive_{year}_{jday}/{day:02d}.{station}_structure'."
+        )
 
 
 class ArchiveEmptyException(Exception):
-    """Custom exception to handle empty archive"""
+    """Custom exception to handle empty archive."""
 
     def __init__(self):
-        msg = "ArchiveEmptyException: No data was available for this timestep."
-        super().__init__(msg)
+        super().__init__("No data was available for this timestep.")
 
         # Additional message printed to log
-        self.msg = ("\t\tNo files found in archive for this time period.")
+        self.msg = "\t\tNo files found in archive for this time period."
 
 
 class NoScanMseedDataException(Exception):
     """
     Custom exception to handle case when no .scanmseed files can be found by
-    read_coastream()
-
+    read_coastream().
     """
 
     def __init__(self):
-        msg = "NoScanMseedDataException: No .scanmseed data found."
-        super().__init__(msg)
+        super().__init__("No .scanmseed data found.")
 
 
 class NoStationAvailabilityDataException(Exception):
     """
-    Custom exception to handle case when no .StationAvailability files can be
-    found by read_availability()
-
+    Custom exception to handle case when no .StationAvailability files can be found by
+    read_availability().
     """
 
     def __init__(self):
-        msg = ("NoStationAvailabilityDataException: No .StationAvailability "
-               "files found.")
-        super().__init__(msg)
+        super().__init__("No .StationAvailability files found.")
 
 
 class DataAvailabilityException(Exception):
     """
-    Custom exception to handle case when all data for the selected stations did
-    not pass the data quality criteria specified by the user.
-
+    Custom exception to handle case when all data for the selected stations did not pass
+    the data quality criteria specified by the user.
     """
 
     def __init__(self):
-        msg = ("DataAvailabilityException: All data for this timestep did not "
-               "pass the specified data quality criteria.")
-        super().__init__(msg)
+        super().__init__(
+            "All data for this timestep did not pass the specified data quality "
+            "criteria."
+        )
 
         # Additional message printed to log
-        self.msg = ("\t\tAll data for this timestep failed to pass the"
-                    "\n\t\tspecified data quality criteria. This includes the"
-                    "\n\t\tpresence of gaps or overlaps, or the data not"
-                    "\n\t\tspanning the full time window.")
+        self.msg = (
+            "\t\tAll data for this timestep failed to pass the"
+            "\n\t\tspecified data quality criteria. This includes the"
+            "\n\t\tpresence of gaps or overlaps, or the data not"
+            "\n\t\tspanning the full time window."
+        )
 
 
 class DataGapException(Exception):
     """
-    Custom exception to handle case when no data is found for the selected
-    stations for a given timestep.
-
+    Custom exception to handle case when no data is found for the selected stations for
+    a given timestep.
     """
 
     def __init__(self):
-        msg = ("DataGapException: No data present in the archive for the"
-               "selected stations for this time window.")
-        super().__init__(msg)
+        super().__init__(
+            "No data present in the archive for theselected stations for this time "
+            "window."
+        )
 
         # Additional message printed to log
-        self.msg = ("\t\tNo data for the selected stations was found in the"
-                    "\n\t\tarchive for this time window.")
+        self.msg = (
+            "\t\tNo data for the selected stations was found in the"
+            "\n\t\tarchive for this time window."
+        )
 
 
 class ChannelNameException(Exception):
     """
-    Custom exception to handle case when waveform data header has channel names
-    which do not conform to the IRIS SEED standard.
-
+    Custom exception to handle case when waveform data header has channel names which do
+    not conform to the IRIS SEED standard.
     """
 
     def __init__(self, trace):
-        msg = ("ChannelNameException: Channel name header does not conform "
-               "to\nthe IRIS SEED standard - 3 characters; ending in 'Z' for\n"
-               "vertical and ending either 'E' & 'N' or '1' & '2' for\n"
-               "horizontal components.\n    Working on trace: {}".format(trace))
-        super().__init__(msg)
+        super().__init__(
+            "Channel name header does not conform to\nthe IRIS SEED standard - 3 "
+            "characters; ending in 'Z' for\nvertical and ending either 'E' & 'N' or "
+            f"'1' & '2' for\nhorizontal components.\n    Working on trace: {trace}"
+        )
 
 
 class NoOnsetPeak(Exception):
     """
-    Custom exception to handle case when no values in the onset function exceed
-    the threshold used for picking.
-
+    Custom exception to handle case when no values in the onset function exceed the
+    threshold used for picking.
     """
 
     def __init__(self, pick_threshold):
-        self.msg = ("\t\t    No onset signal exceeding pick threshold "
-                    f"({pick_threshold:5.3f}) - continuing.")
+        self.msg = (
+            "\t\t    No onset signal exceeding pick threshold "
+            f"({pick_threshold:5.3f}) - continuing."
+        )
         super().__init__(self.msg)
 
 
 class BadUpfactorException(Exception):
     """
-    Custom exception to handle case when the chosen upfactor does not create a
-    trace with a sampling rate that can be decimated to the target sampling
-    rate
-
+    Custom exception to handle case when the chosen upfactor does not create a trace
+    with a sampling rate that can be decimated to the target sampling rate.
     """
 
     def __init__(self, trace):
-        msg = ("BadUpfactorException: chosen upfactor cannot be decimated to\n"
-               "target sampling rate.\n    Working on trace: {}".format(trace))
-        super().__init__(msg)
+        super().__init__(
+            "Chosen upfactor cannot be decimated to\ntarget sampling rate."
+            f"\n    Working on trace: {trace}"
+        )
 
 
 class OnsetTypeError(Exception):
     """
-    Custom exception to handle case when the onset object passed to QuakeScan
-    is not of the default type defined in QuakeMigrate.
-
+    Custom exception to handle case when the onset object passed to QuakeScan is not of
+    the default type defined in QuakeMigrate.
     """
 
     def __init__(self):
-        msg = ("OnsetTypeError: The Onset object you have created does not "
-               "inherit from the required base class - see manual.")
-        super().__init__(msg)
+        super().__init__(
+            "The Onset object you have created does not inherit from the required base "
+            "class - see manual."
+        )
 
 
 class PickerTypeError(Exception):
     """
-    Custom exception to handle case when the phase picker object passed to
-    QuakeScan is not of the default type defined in QuakeMigrate.
-
+    Custom exception to handle case when the phase picker object passed to QuakeScan is
+    not of the default type defined in QuakeMigrate.
     """
 
     def __init__(self):
-        msg = ("PickerTypeError: The PhasePicker object you have created does "
-               "not inherit from the required base class - see manual.")
-        super().__init__(msg)
+        super().__init__(
+            "The PhasePicker object you have created does not inherit from the "
+            "required base class - see manual."
+        )
 
 
 class LUTPhasesException(Exception):
     """
-    Custom exception to handle the case when the look-up table does not
-    contain the traveltimes for the phases necessary for a given function.
-
+    Custom exception to handle the case when the look-up table does not contain the
+    traveltimes for the phases necessary for a given function.
     """
 
     def __init__(self, message):
-        msg = (f"LUTPhasesException: {message}")
-        super().__init__(msg)
+        super().__init__(message)
 
 
 class PickOrderException(Exception):
     """
-    Custom exception to handle the case when the pick for the P phase is later
-    than the pick for the S phase.
-
+    Custom exception to handle the case when the pick for the P phase is later than the
+    pick for the S phase.
     """
 
     def __init__(self, event_uid, station, p_pick, s_pick):
-        msg = ("PickOrderException: The P-phase arrival-time pick is later "
-               "than the S-phase arrival pick! Something has gone wrong. "
-               f"Event: {event_uid}, station: {station}, p_pick: {p_pick}, "
-               f"s_pick: {s_pick}. There is probably a bug with the picker.")
-        super().__init__(msg)
+        super().__init__(
+            "The P-phase arrival-time pick is later than the S-phase arrival pick! "
+            f"Something has gone wrong.\nEvent: {event_uid}, station: {station}, "
+            f"p_pick: {p_pick}, s_pick: {s_pick}. There is probably a bug with the "
+            "picker."
+        )
 
 
 class MagsTypeError(Exception):
     """
-    Custom exception to handle case when an object has been provided to
-    calculate magnitudes during locate, but it isn't supported.
-
+    Custom exception to handle case when an object has been provided to calculate
+    magnitudes during locate, but it isn't supported.
     """
 
     def __init__(self):
-        msg = ("MagsTypeError: The Mags object you have specified is not "
-               "supported: currently only "
-               "`quakemigrate.signal.local_mag.LocalMag` - see manual.")
-        super().__init__(msg)
+        super().__init__(
+            "The Mags object you have specified is not supported: currently only "
+            "`quakemigrate.signal.local_mag.LocalMag` - see manual."
+        )
 
 
 class NoTriggerFilesFound(Exception):
     """
-    Custom exception to handle case when no trigger files are found during
-    locate. This can occur for one of two reasons - an entirely invalid time
-    period was used (i.e. one that does not overlap at all with a period of
-    time for which there exists TriggeredEvents.csv files) or an invalid run
-    name was provided.
-
+    Custom exception to handle case when no trigger files are found during locate. This
+    can occur for one of two reasons - an entirely invalid time period was used (i.e.
+    one that does not overlap at all with a period of time for which there exists
+    TriggeredEvents.csv files) or an invalid run name was provided.
     """
 
     def __init__(self):
-        msg = ("NoTriggerFilesFound: Double check you have supplied a valid "
-               "run name and a time period for which you have run detect.")
-        super().__init__(msg)
+        super().__init__(
+            "Double check you have supplied a valid run name and a time period for "
+            "which you have run detect."
+        )
 
 
 class ResponseNotFoundError(Exception):
     """
-    Custom exception to handle the case where the provided response inventory
-    doesn't contain the response information for a trace.
+    Custom exception to handle the case where the provided response inventory doesn't
+    contain the response information for a trace.
 
     Parameters
     ----------
     e : str
-        Error message from ObsPy `Inventory.get_response()`
+        Error message from ObsPy `Inventory.get_response()`.
     tr_id : str
-        ID string for the Trace for which the response cannot be found
+        ID string for the Trace for which the response cannot be found.
 
     """
 
     def __init__(self, e, tr_id):
-        msg = (f"ResponseNotFoundError: {e} -- skipping {tr_id}")
-        super().__init__(msg)
+        super().__init__(f"{e} -- skipping {tr_id}")
 
 
 class ResponseRemovalError(Exception):
     """
-    Custom exception to handle the case where the response removal was not
-    successful.
+    Custom exception to handle the case where the response removal was not successful.
 
     Parameters
     ----------
     e : str
-        Error message from ObsPy `Trace.remove_response()` or
-        `Trace.simulate()`
+        Error message from ObsPy `Trace.remove_response()` or `Trace.simulate()`.
     tr_id : str
-        ID string for the Trace for which the response cannot be removed
+        ID string for the Trace for which the response cannot be removed.
 
     """
 
     def __init__(self, e, tr_id):
-        msg = (f"ResponseRemovalError: {e} -- skipping {tr_id}")
-        super().__init__(msg)
+        super().__init__(f"{e} -- skipping {tr_id}")
 
 
 class NyquistException(Exception):
     """
-    Custom exception to handle the case where the specified filter has a
-    lowpass corner above the signal Nyquist frequency.
+    Custom exception to handle the case where the specified filter has a lowpass corner
+    above the signal Nyquist frequency.
 
     Parameters
     ----------
     freqmax : float
-        Specified lowpass frequency for filter
+        Specified lowpass frequency for filter.
     f_nyquist : float
-        Nyquist frequency for the relevant waveform data
+        Nyquist frequency for the relevant waveform data.
     tr_id : str
-        ID string for the Trace
+        ID string for the Trace.
 
     """
 
     def __init__(self, freqmax, f_nyquist, tr_id):
-        msg = (f"    NyquistException: Selected bandpass_highcut {freqmax} "
-               f"Hz is at or above the Nyquist frequency ({f_nyquist} Hz) "
-               f"for trace {tr_id}. ")
-        super().__init__(msg)
+        super().__init__(
+            f"    Selected bandpass_highcut {freqmax} Hz is at or above the Nyquist "
+            f"frequency ({f_nyquist} Hz) for trace {tr_id}. "
+        )
 
 
 class PeakToTroughError(Exception):
     """
-    Custom exception to handle case when amplitude._peak_to_trough_amplitude
-    encounters an anomalous set of peaks and troughs, so can't calculate an
-    amplitude.
-
+    Custom exception to handle case when amplitude._peak_to_trough_amplitude encounters
+    an anomalous set of peaks and troughs, so can't calculate an amplitude.
     """
 
     def __init__(self, err):
-        msg = (f"PeakToTroughError: {err}")
-        super().__init__(msg)
+        super().__init__(err)
 
         # Additional message printed to log
-        self.msg = (err)
+        self.msg = err
 
 
 class TimeSpanException(Exception):
     """
-    Custom exception to handle case when the user has submitted a start time
-    that is after the end time.
-
+    Custom exception to handle case when the user has submitted a start time that is
+    after the end time.
     """
 
     def __init__(self):
-        msg = ("TimeSpanException: The start time specified is after the end"
-               " time.")
-        super().__init__(msg)
+        super().__init__("The start time specified is after the end time.")
 
 
 class InvalidTriggerThresholdMethodException(Exception):
     """
-    Custom exception to handle case when the user has not selected a valid
-    trigger threshold method.
-
+    Custom exception to handle case when the user has not selected a valid trigger
+    threshold method.
     """
 
     def __init__(self):
-        msg = ("InvalidTriggerThresholdMethodException: Only 'static' or "
-               "'dynamic' thresholds are supported.")
-        super().__init__(msg)
+        super().__init__("Only 'static' or 'dynamic' thresholds are supported.")
 
 
 class InvalidPickThresholdMethodException(Exception):
     """
-    Custom exception to handle case when the user has not selected a valid
-    pick threshold method.
-
+    Custom exception to handle case when the user has not selected a valid pick
+    threshold method.
     """
 
     def __init__(self):
-        msg = ("InvalidPickThresholdMethodException: Only 'percentile' or "
-               "'MAD' thresholds are supported.")
-        super().__init__(msg)
+        super().__init__("Only 'percentile' or 'MAD' thresholds are supported.")
```

### Comparing `quakemigrate-1.0.1/quakemigrate.egg-info/PKG-INFO` & `quakemigrate-1.0.2/quakemigrate.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quakemigrate
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python package for automatic earthquake detection and location using waveform migration and stacking.
 Author-email: The QuakeMigrate Development Team <quakemigrate.developers@gmail.com>, Tom Winder <tom.winder@esc.cam.ac.uk>, Conor Bacon <cbacon@ldeo.columbia.edu>
 Maintainer-email: Tom Winder <tom.winder@esc.cam.ac.uk>, Conor Bacon <cbacon@ldeo.columbia.edu>
 License: GPLv3
 Project-URL: GitHub, https://github.com/QuakeMigrate/QuakeMigrate
 Project-URL: Issues, https://github.com/QuakeMigrate/QuakeMigrate/issues
 Keywords: seismic event detection,seismic event location,waveform migration,array,seismic,seismology,earthquake,seismic waves,waveform,processing
@@ -68,15 +68,15 @@
 
 <p align="center">
 <img src="https://github.com/QuakeMigrate/QuakeMigrate/raw/master/docs/img/QMlogoBig.png", width="80%">
 </p>
 
 Key Features
 ------------
-QuakeMigrate uses a waveform migration and stacking algorithm to search for coherent seismic phase arrivals across a network of instruments. It produces—from raw data—catalogues of earthquakes with locations, origin times, phase arrival picks, and local magnitude estimates, as well as well as rigorous estimates of the associated uncertainties.
+QuakeMigrate uses a waveform migration and stacking algorithm to search for coherent seismic phase arrivals across a network of instruments. It produces—from raw data—catalogues of earthquakes with locations, origin times, phase arrival picks, and local magnitude estimates, as well as rigorous estimates of the associated uncertainties.
 
 The package has been built with a modular architecture, providing the potential for extension and adaptation at numerous entry points. This includes, but is not limited to:
 * the calculation or import of traveltime grids
 * the choice of algorithm used to identify phase arrivals (for example by kurtosis, cross-covariance analysis between multiple components, machine learning techniques and more)
 * the stacking function used to combine onset functions
 * the algorithm used to perform phase picking
 
@@ -121,24 +121,22 @@
 
 ```console
 Winder, T., Bacon, C.A., Smith, J.D., Hudson, T.S., Drew, J., and White, R.S. QuakeMigrate: a Python Package for Automatic Earthquake Detection and Location Using Waveform Migration and Stacking. (to be submitted to Seismica).
 ```
 
 Contributing to QuakeMigrate
 ----------------------------
-Contributions to QuakeMigrate are welcomed. The first stop should be to reach out, either directly or—preferably—via the GitHub Issues panel, to discuss the proposed changes. Next, simply fork the QuakeMigrate repository, make your changes/add your new contribution, then make a [pull request](https://help.github.com/articles/about-pull-requests/).
+Contributions to QuakeMigrate are welcomed. Whether you have identified a bug or would like to request a new feature, your first stop should be to reach out, either directly or—preferably—via the GitHub Issues panel, to discuss the proposed changes. Once we have had a chance to scope out the proposed changes you can proceed with making your contribution following the instructions in our [contributions guidelines](https://github.com/QuakeMigrate/QuakeMigrate/blob/master/CONTRIBUTING.md).
 
 Bug reports, suggestions for new features and enhancements, and even links to projects that have made use of QuakeMigrate are most welcome.
 
-See our [contributions page](https://github.com/QuakeMigrate/QuakeMigrate/blob/master/CONTRIBUTING.md) for more information.
-
 Contact
 -------
 You can contact us directly at: quakemigrate.developers@gmail.com
 
 Any additional comments/questions can be directed to:
 * **Tom Winder** - tom.winder@esc.cam.ac.uk
 * **Conor Bacon** - conor.bacon@cantab.net
 
 License
 -------
-This package is written and maintained by the QuakeMigrate developers, Copyright QuakeMigrate developers 2023. It is distributed under the GPLv3 License. Please see the [LICENSE](LICENSE) file for a complete description of the rights and freedoms that this provides the user.
+This package is written and maintained by the QuakeMigrate developers, Copyright QuakeMigrate developers 2020–2023. It is distributed under the GPLv3 License. Please see the [LICENSE](LICENSE) file for a complete description of the rights and freedoms that this provides the user.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: quakemigrate Version: 1.0.1 Summary: A Python
+Metadata-Version: 2.1 Name: quakemigrate Version: 1.0.2 Summary: A Python
 package for automatic earthquake detection and location using waveform
 migration and stacking. Author-email: The QuakeMigrate Development Team
 developers@gmail.com>, Tom Winder
 winder@esc.cam.ac.uk>, Conor Bacon
 ldeo.columbia.edu> Maintainer-email: Tom Winder
 winder@esc.cam.ac.uk>, Conor Bacon
 ldeo.columbia.edu> License: GPLv3 Project-URL: GitHub, https://github.com/
@@ -29,39 +29,38 @@
     QuakeMigrate is a Python package for automatic earthquake detection and
                 location using waveform migration and stacking.
                                   width="80%">
 Key Features ------------ QuakeMigrate uses a waveform migration and stacking
 algorithm to search for coherent seismic phase arrivals across a network of
 instruments. It producesâfrom raw dataâcatalogues of earthquakes with
 locations, origin times, phase arrival picks, and local magnitude estimates, as
-well as well as rigorous estimates of the associated uncertainties. The package
-has been built with a modular architecture, providing the potential for
-extension and adaptation at numerous entry points. This includes, but is not
-limited to: * the calculation or import of traveltime grids * the choice of
-algorithm used to identify phase arrivals (for example by kurtosis, cross-
-covariance analysis between multiple components, machine learning techniques
-and more) * the stacking function used to combine onset functions * the
-algorithm used to perform phase picking Documentation ------------
-- Documentation for QuakeMigrate is hosted [here](https://
-quakemigrate.readthedocs.io/en/latest/index.html). Installation -----------
-- Detailed installation instructions can be found [here](https://
-quakemigrate.readthedocs.io/en/latest/installation.html). If you're comfortable
-with virtual environments and just want to get started, QuakeMigrate is
-available via the Python Package Index, and can be installed via pip:
-```console pip install quakemigrate ``` Usage ----- We are working on tutorials
-covering how each individual aspect of the package works, as well as example
-use cases where we provide substantive reasoning for the parameter choices
-used. These examples include applications to cryoseismicity and volcano
-seismology. This is a work in progress - [see our documentation for full
-details](https://quakemigrate.readthedocs.io/en/latest/tutorials.html). ###
-Examples you can run in your browser To quickly get a taste for how the
-software works, try out the two icequake examples hosted on Binder: * Icequakes
-at the Rutford Ice Stream, Antarctica [![badge](https://img.shields.io/badge/
-launch-Icequake%20Rutford%20notebook-579ACA.svg)](https://mybinder.org/v2/gh/
-QuakeMigrate/QuakeMigrate/
+well as rigorous estimates of the associated uncertainties. The package has
+been built with a modular architecture, providing the potential for extension
+and adaptation at numerous entry points. This includes, but is not limited to:
+* the calculation or import of traveltime grids * the choice of algorithm used
+to identify phase arrivals (for example by kurtosis, cross-covariance analysis
+between multiple components, machine learning techniques and more) * the
+stacking function used to combine onset functions * the algorithm used to
+perform phase picking Documentation ------------- Documentation for
+QuakeMigrate is hosted [here](https://quakemigrate.readthedocs.io/en/latest/
+index.html). Installation ------------ Detailed installation instructions can
+be found [here](https://quakemigrate.readthedocs.io/en/latest/
+installation.html). If you're comfortable with virtual environments and just
+want to get started, QuakeMigrate is available via the Python Package Index,
+and can be installed via pip: ```console pip install quakemigrate ``` Usage ---
+-- We are working on tutorials covering how each individual aspect of the
+package works, as well as example use cases where we provide substantive
+reasoning for the parameter choices used. These examples include applications
+to cryoseismicity and volcano seismology. This is a work in progress - [see our
+documentation for full details](https://quakemigrate.readthedocs.io/en/latest/
+tutorials.html). ### Examples you can run in your browser To quickly get a
+taste for how the software works, try out the two icequake examples hosted on
+Binder: * Icequakes at the Rutford Ice Stream, Antarctica [![badge](https://
+img.shields.io/badge/launch-Icequake%20Rutford%20notebook-579ACA.svg)](https://
+mybinder.org/v2/gh/QuakeMigrate/QuakeMigrate/
 master?filepath=examples%2FIcequake_Rutford%2Ficequakes_rutford.ipynb) *
 Icequakes at the SkeiÃ°arÃ¡rjÃ¶kull outlet glacier, Iceland [![badge](https://
 img.shields.io/badge/launch-Icequake%20Iceland%20notebook-E66581.svg)](https://
 mybinder.org/v2/gh/QuakeMigrate/QuakeMigrate/
 master?filepath=examples%2FIcequake_Iceland%2Ficequakes_iceland.ipynb) And for
 a more comprehensive demonstration of the options available, see the [template
 scripts](examples/template_scripts). Citation -------- If you use this package
@@ -71,22 +70,23 @@
 Earthquake Detection and Location. In AGU Fall Meeting 2020. AGU. ``` as well
 as the relevant version of the source code on [Zenodo](https://doi.org/10.5281/
 zenodo.4442749). We hope to have a publication coming out soon: ```console
 Winder, T., Bacon, C.A., Smith, J.D., Hudson, T.S., Drew, J., and White, R.S.
 QuakeMigrate: a Python Package for Automatic Earthquake Detection and Location
 Using Waveform Migration and Stacking. (to be submitted to Seismica). ```
 Contributing to QuakeMigrate ---------------------------- Contributions to
-QuakeMigrate are welcomed. The first stop should be to reach out, either
-directly orâpreferablyâvia the GitHub Issues panel, to discuss the proposed
-changes. Next, simply fork the QuakeMigrate repository, make your changes/add
-your new contribution, then make a [pull request](https://help.github.com/
-articles/about-pull-requests/). Bug reports, suggestions for new features and
-enhancements, and even links to projects that have made use of QuakeMigrate are
-most welcome. See our [contributions page](https://github.com/QuakeMigrate/
-QuakeMigrate/blob/master/CONTRIBUTING.md) for more information. Contact ------
-- You can contact us directly at: quakemigrate.developers@gmail.com Any
-additional comments/questions can be directed to: * **Tom Winder** -
-tom.winder@esc.cam.ac.uk * **Conor Bacon** - conor.bacon@cantab.net License ---
----- This package is written and maintained by the QuakeMigrate developers,
-Copyright QuakeMigrate developers 2023. It is distributed under the GPLv3
-License. Please see the [LICENSE](LICENSE) file for a complete description of
-the rights and freedoms that this provides the user.
+QuakeMigrate are welcomed. Whether you have identified a bug or would like to
+request a new feature, your first stop should be to reach out, either directly
+orâpreferablyâvia the GitHub Issues panel, to discuss the proposed changes.
+Once we have had a chance to scope out the proposed changes you can proceed
+with making your contribution following the instructions in our [contributions
+guidelines](https://github.com/QuakeMigrate/QuakeMigrate/blob/master/
+CONTRIBUTING.md). Bug reports, suggestions for new features and enhancements,
+and even links to projects that have made use of QuakeMigrate are most welcome.
+Contact ------- You can contact us directly at:
+quakemigrate.developers@gmail.com Any additional comments/questions can be
+directed to: * **Tom Winder** - tom.winder@esc.cam.ac.uk * **Conor Bacon** -
+conor.bacon@cantab.net License ------- This package is written and maintained
+by the QuakeMigrate developers, Copyright QuakeMigrate developers 2020â2023.
+It is distributed under the GPLv3 License. Please see the [LICENSE](LICENSE)
+file for a complete description of the rights and freedoms that this provides
+the user.
```

### Comparing `quakemigrate-1.0.1/quakemigrate.egg-info/SOURCES.txt` & `quakemigrate-1.0.2/quakemigrate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quakemigrate-1.0.1/setup.py` & `quakemigrate-1.0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,14 @@
 # -*- coding: utf-8 -*-
 """
-A Python package for automatic earthquake detection and location using waveform
-migration and stacking.
-
-QuakeMigrate is a Python package for automatic earthquake detection and
-location using waveform migration and stacking. It can be used to produce
-catalogues of earthquakes, including hypocentres, origin times, phase arrival
-picks, and local magnitude estimates, as well as rigorous estimates of the
-associated uncertainties.
-
-The package has been built with a modular architecture, providing the potential
-for extension and adaptation at numerous entry points.
+QuakeMigrate: A Python package for automatic earthquake detection and location using
+waveform migration and stacking.
 
 :copyright:
-    2020-2022, QuakeMigrate developers.
+    2020–2023, QuakeMigrate developers.
 :license:
     GNU General Public License, Version 3
     (https://www.gnu.org/licenses/gpl-3.0.html)
 
 """
 
 import os
@@ -26,26 +17,14 @@
 import shutil
 import sys
 
 from distutils.ccompiler import get_default_compiler
 from setuptools import Extension, setup
 
 
-# The minimum python version which can be used to run QuakeMigrate
-MIN_PYTHON_VERSION = (3, 8)
-
-# Fail fast if the user is on an unsupported version of Python.
-if sys.version_info < MIN_PYTHON_VERSION:
-    msg = (
-        f"QuakeMigrate requires python version >= {MIN_PYTHON_VERSION}"
-        f" you are using python version {sys.version_info}"
-    )
-    print(msg, file=sys.stderr)
-    sys.exit(1)
-
 # Check if we are on RTD and don't build extensions if we are.
 READ_THE_DOCS = os.environ.get("READTHEDOCS", None) == "True"
 if READ_THE_DOCS:
     try:
         environ = os.environb
     except AttributeError:
         environ = os.environ
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quakemigrate-1.0.1/tests/test_benchmarks.py` & `quakemigrate-1.0.2/tests/test_benchmarks.py`

 * *Files identical despite different names*

### Comparing `quakemigrate-1.0.1/tests/test_import.py` & `quakemigrate-1.0.2/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `quakemigrate-1.0.1/tests/test_util.py` & `quakemigrate-1.0.2/tests/test_util.py`

 * *Files identical despite different names*

