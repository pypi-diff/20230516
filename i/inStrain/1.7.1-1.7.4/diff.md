# Comparing `tmp/inStrain-1.7.1.tar.gz` & `tmp/inStrain-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/inStrain-1.7.1.tar", last modified: Sat Feb 25 02:21:32 2023, max compression
+gzip compressed data, was "inStrain-1.7.4.tar", last modified: Tue May 16 19:27:49 2023, max compression
```

## Comparing `inStrain-1.7.1.tar` & `inStrain-1.7.4.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-02-25 02:21:32.500838 inStrain-1.7.1/
--rw-r--r--   0 mattolm    (501) staff       (20)      296 2023-02-25 02:21:32.500687 inStrain-1.7.1/PKG-INFO
--rw-r--r--   0 mattolm    (501) staff       (20)     1416 2023-02-21 01:15:19.000000 inStrain-1.7.1/README.md
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-02-25 02:21:32.493346 inStrain-1.7.1/bin/
--rwxr-xr-x   0 mattolm    (501) staff       (20)      962 2021-01-21 18:18:24.000000 inStrain-1.7.1/bin/inStrain
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-02-25 02:21:32.493811 inStrain-1.7.1/docker/
--rw-r--r--   0 mattolm    (501) staff       (20)        0 2021-01-21 18:18:24.000000 inStrain-1.7.1/docker/__init__.py
--rwxr-xr-x   0 mattolm    (501) staff       (20)     1688 2021-01-21 18:18:24.000000 inStrain-1.7.1/docker/job_utils.py
--rwxr-xr-x   0 mattolm    (501) staff       (20)    10928 2022-06-10 19:12:50.000000 inStrain-1.7.1/docker/run_instrain.py
--rwxr-xr-x   0 mattolm    (501) staff       (20)     5153 2021-01-21 18:18:24.000000 inStrain-1.7.1/docker/s3_utils.py
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-02-25 02:21:32.496163 inStrain-1.7.1/inStrain/
--rwxr-xr-x   0 mattolm    (501) staff       (20)    31954 2023-02-24 17:32:05.000000 inStrain-1.7.1/inStrain/GeneProfile.py
--rwxr-xr-x   0 mattolm    (501) staff       (20)    42757 2023-02-21 01:15:04.000000 inStrain-1.7.1/inStrain/SNVprofile.py
--rwxr-xr-x   0 mattolm    (501) staff       (20)       34 2021-01-21 18:18:24.000000 inStrain-1.7.1/inStrain/__init__.py
--rw-r--r--   0 mattolm    (501) staff       (20)       22 2023-02-25 01:49:54.000000 inStrain-1.7.1/inStrain/_version.py
--rw-r--r--   0 mattolm    (501) staff       (20)    23220 2023-02-21 01:15:04.000000 inStrain-1.7.1/inStrain/argumentParser.py
--rw-r--r--   0 mattolm    (501) staff       (20)    25579 2022-06-10 19:12:50.000000 inStrain-1.7.1/inStrain/compare_controller.py
--rw-r--r--   0 mattolm    (501) staff       (20)     4897 2021-01-21 18:18:24.000000 inStrain-1.7.1/inStrain/compare_greedy.py
--rw-r--r--   0 mattolm    (501) staff       (20)     8480 2023-02-25 01:32:59.000000 inStrain-1.7.1/inStrain/compare_utils.py
--rw-r--r--   0 mattolm    (501) staff       (20)    17782 2023-02-21 01:15:04.000000 inStrain-1.7.1/inStrain/controller.py
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-02-25 02:21:32.497501 inStrain-1.7.1/inStrain/deprecated/
--rw-r--r--   0 mattolm    (501) staff       (20)     2257 2023-02-24 18:53:38.000000 inStrain-1.7.1/inStrain/deprecated/DEPRECATEDmapping_plots.py
--rw-r--r--   0 mattolm    (501) staff       (20)    34343 2021-02-12 01:00:32.000000 inStrain-1.7.1/inStrain/deprecated/__init__.py
--rw-r--r--   0 mattolm    (501) staff       (20)    22971 2021-01-21 18:18:24.000000 inStrain-1.7.1/inStrain/deprecated/deprecated_filter_reads.py
--rwxr-xr-x   0 mattolm    (501) staff       (20)     9651 2021-01-21 18:18:24.000000 inStrain-1.7.1/inStrain/deprecated/deprecated_gene_statistics.py
--rw-r--r--   0 mattolm    (501) staff       (20)    58073 2023-02-25 01:32:59.000000 inStrain-1.7.1/inStrain/deprecated/plottingUtilities.py
--rwxr-xr-x   0 mattolm    (501) staff       (20)    35695 2023-02-25 01:48:27.000000 inStrain-1.7.1/inStrain/filter_reads.py
--rw-r--r--   0 mattolm    (501) staff       (20)    34180 2023-02-25 01:41:50.000000 inStrain-1.7.1/inStrain/genomeUtilities.py
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-02-25 02:21:32.497662 inStrain-1.7.1/inStrain/helper_files/
--rw-r--r--   0 mattolm    (501) staff       (20)  1256610 2021-01-21 18:18:24.000000 inStrain-1.7.1/inStrain/helper_files/NullModel.txt
--rw-r--r--   0 mattolm    (501) staff       (20)     8957 2021-02-12 01:00:32.000000 inStrain-1.7.1/inStrain/irep_utilities.py
--rw-r--r--   0 mattolm    (501) staff       (20)    38401 2021-03-26 21:19:02.000000 inStrain-1.7.1/inStrain/logUtils.py
--rw-r--r--   0 mattolm    (501) staff       (20)    11844 2023-02-21 01:15:04.000000 inStrain-1.7.1/inStrain/parse_annotations.py
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-02-25 02:21:32.499536 inStrain-1.7.1/inStrain/plotting/
--rw-r--r--   0 mattolm    (501) staff       (20)     2524 2023-02-24 18:53:38.000000 inStrain-1.7.1/inStrain/plotting/SNV_plots.py
--rw-r--r--   0 mattolm    (501) staff       (20)      662 2021-02-12 01:00:32.000000 inStrain-1.7.1/inStrain/plotting/__init__.py
--rw-r--r--   0 mattolm    (501) staff       (20)     9260 2023-02-25 01:38:35.000000 inStrain-1.7.1/inStrain/plotting/compare_plots.py
--rw-r--r--   0 mattolm    (501) staff       (20)     2548 2021-02-12 01:00:32.000000 inStrain-1.7.1/inStrain/plotting/gene_plots.py
--rw-r--r--   0 mattolm    (501) staff       (20)     6638 2023-02-24 18:50:29.000000 inStrain-1.7.1/inStrain/plotting/linkage_plots.py
--rw-r--r--   0 mattolm    (501) staff       (20)     9075 2023-02-25 00:47:19.000000 inStrain-1.7.1/inStrain/plotting/mapping_plots.py
--rw-r--r--   0 mattolm    (501) staff       (20)     5332 2023-02-25 00:49:14.000000 inStrain-1.7.1/inStrain/plotting/plotting_controller.py
--rw-r--r--   0 mattolm    (501) staff       (20)    18444 2023-02-24 18:53:38.000000 inStrain-1.7.1/inStrain/plotting/positional_plots.py
--rw-r--r--   0 mattolm    (501) staff       (20)     2831 2021-02-12 01:00:32.000000 inStrain-1.7.1/inStrain/plotting/utilities.py
--rwxr-xr-x   0 mattolm    (501) staff       (20)    20710 2023-02-25 01:32:59.000000 inStrain-1.7.1/inStrain/polymorpher.py
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-02-25 02:21:32.500386 inStrain-1.7.1/inStrain/profile/
--rw-r--r--   0 mattolm    (501) staff       (20)      636 2021-01-21 18:18:24.000000 inStrain-1.7.1/inStrain/profile/__init__.py
--rw-r--r--   0 mattolm    (501) staff       (20)     5822 2021-02-12 01:00:32.000000 inStrain-1.7.1/inStrain/profile/fasta.py
--rw-r--r--   0 mattolm    (501) staff       (20)     9115 2021-01-21 18:18:24.000000 inStrain-1.7.1/inStrain/profile/linkage.py
--rw-r--r--   0 mattolm    (501) staff       (20)    15636 2021-01-21 18:18:24.000000 inStrain-1.7.1/inStrain/profile/profile_controller.py
--rw-r--r--   0 mattolm    (501) staff       (20)    32820 2023-02-24 18:17:07.000000 inStrain-1.7.1/inStrain/profile/profile_utilities.py
--rw-r--r--   0 mattolm    (501) staff       (20)     3144 2021-02-17 23:42:47.000000 inStrain-1.7.1/inStrain/profile/samtools_ops.py
--rw-r--r--   0 mattolm    (501) staff       (20)    10361 2021-02-12 01:00:32.000000 inStrain-1.7.1/inStrain/profile/snv_utilities.py
--rwxr-xr-x   0 mattolm    (501) staff       (20)     5332 2021-02-12 01:00:32.000000 inStrain-1.7.1/inStrain/quickProfile.py
--rwxr-xr-x   0 mattolm    (501) staff       (20)    16916 2022-06-10 19:12:50.000000 inStrain-1.7.1/inStrain/readComparer.py
--rw-r--r--   0 mattolm    (501) staff       (20)     2629 2023-02-25 01:49:24.000000 inStrain-1.7.1/inStrain/utils.py
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-02-25 02:21:32.496866 inStrain-1.7.1/inStrain.egg-info/
--rw-r--r--   0 mattolm    (501) staff       (20)      296 2023-02-25 02:21:32.000000 inStrain-1.7.1/inStrain.egg-info/PKG-INFO
--rw-r--r--   0 mattolm    (501) staff       (20)     1555 2023-02-25 02:21:32.000000 inStrain-1.7.1/inStrain.egg-info/SOURCES.txt
--rw-r--r--   0 mattolm    (501) staff       (20)        1 2023-02-25 02:21:32.000000 inStrain-1.7.1/inStrain.egg-info/dependency_links.txt
--rw-r--r--   0 mattolm    (501) staff       (20)        1 2023-02-25 02:21:32.000000 inStrain-1.7.1/inStrain.egg-info/not-zip-safe
--rw-r--r--   0 mattolm    (501) staff       (20)      113 2023-02-25 02:21:32.000000 inStrain-1.7.1/inStrain.egg-info/requires.txt
--rw-r--r--   0 mattolm    (501) staff       (20)       16 2023-02-25 02:21:32.000000 inStrain-1.7.1/inStrain.egg-info/top_level.txt
--rw-r--r--   0 mattolm    (501) staff       (20)       38 2023-02-25 02:21:32.500882 inStrain-1.7.1/setup.cfg
--rw-r--r--   0 mattolm    (501) staff       (20)     1051 2023-02-25 02:18:49.000000 inStrain-1.7.1/setup.py
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-02-25 02:21:32.500506 inStrain-1.7.1/test/
--rwxr-xr-x   0 mattolm    (501) staff       (20)     1213 2022-06-10 19:12:50.000000 inStrain-1.7.1/test/test_suite.py
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-05-16 19:27:49.548183 inStrain-1.7.4/
+-rw-r--r--   0 mattolm    (501) staff       (20)     1065 2021-03-26 22:19:41.000000 inStrain-1.7.4/LICENSE
+-rw-r--r--   0 mattolm    (501) staff       (20)      279 2023-05-16 19:27:49.548042 inStrain-1.7.4/PKG-INFO
+-rw-r--r--   0 mattolm    (501) staff       (20)     1416 2023-02-21 01:15:19.000000 inStrain-1.7.4/README.md
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-05-16 19:27:49.534676 inStrain-1.7.4/bin/
+-rwxr-xr-x   0 mattolm    (501) staff       (20)      962 2021-01-21 18:18:24.000000 inStrain-1.7.4/bin/inStrain
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-05-16 19:27:49.535484 inStrain-1.7.4/docker/
+-rw-r--r--   0 mattolm    (501) staff       (20)        0 2021-01-21 18:18:24.000000 inStrain-1.7.4/docker/__init__.py
+-rwxr-xr-x   0 mattolm    (501) staff       (20)     1688 2021-01-21 18:18:24.000000 inStrain-1.7.4/docker/job_utils.py
+-rwxr-xr-x   0 mattolm    (501) staff       (20)    10928 2022-06-10 19:12:50.000000 inStrain-1.7.4/docker/run_instrain.py
+-rwxr-xr-x   0 mattolm    (501) staff       (20)     5153 2021-01-21 18:18:24.000000 inStrain-1.7.4/docker/s3_utils.py
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-05-16 19:27:49.539683 inStrain-1.7.4/inStrain/
+-rwxr-xr-x   0 mattolm    (501) staff       (20)    31954 2023-02-24 17:32:05.000000 inStrain-1.7.4/inStrain/GeneProfile.py
+-rwxr-xr-x   0 mattolm    (501) staff       (20)    42757 2023-05-16 19:21:51.000000 inStrain-1.7.4/inStrain/SNVprofile.py
+-rwxr-xr-x   0 mattolm    (501) staff       (20)       34 2021-01-21 18:18:24.000000 inStrain-1.7.4/inStrain/__init__.py
+-rw-r--r--   0 mattolm    (501) staff       (20)       22 2023-05-16 19:27:09.000000 inStrain-1.7.4/inStrain/_version.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    23220 2023-02-21 01:15:04.000000 inStrain-1.7.4/inStrain/argumentParser.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    25579 2022-06-10 19:12:50.000000 inStrain-1.7.4/inStrain/compare_controller.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     4897 2021-01-21 18:18:24.000000 inStrain-1.7.4/inStrain/compare_greedy.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     8480 2023-02-25 01:32:59.000000 inStrain-1.7.4/inStrain/compare_utils.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    17782 2023-02-21 01:15:04.000000 inStrain-1.7.4/inStrain/controller.py
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-05-16 19:27:49.542398 inStrain-1.7.4/inStrain/deprecated/
+-rw-r--r--   0 mattolm    (501) staff       (20)     2257 2023-02-24 18:53:38.000000 inStrain-1.7.4/inStrain/deprecated/DEPRECATEDmapping_plots.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    34343 2021-02-12 01:00:32.000000 inStrain-1.7.4/inStrain/deprecated/__init__.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    22971 2021-01-21 18:18:24.000000 inStrain-1.7.4/inStrain/deprecated/deprecated_filter_reads.py
+-rwxr-xr-x   0 mattolm    (501) staff       (20)     9651 2021-01-21 18:18:24.000000 inStrain-1.7.4/inStrain/deprecated/deprecated_gene_statistics.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    58073 2023-02-25 01:32:59.000000 inStrain-1.7.4/inStrain/deprecated/plottingUtilities.py
+-rwxr-xr-x   0 mattolm    (501) staff       (20)    35695 2023-02-25 01:48:27.000000 inStrain-1.7.4/inStrain/filter_reads.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    34180 2023-02-25 01:41:50.000000 inStrain-1.7.4/inStrain/genomeUtilities.py
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-05-16 19:27:49.543129 inStrain-1.7.4/inStrain/helper_files/
+-rw-r--r--   0 mattolm    (501) staff       (20)  1256610 2021-01-21 18:18:24.000000 inStrain-1.7.4/inStrain/helper_files/NullModel.txt
+-rw-r--r--   0 mattolm    (501) staff       (20)     8957 2021-02-12 01:00:32.000000 inStrain-1.7.4/inStrain/irep_utilities.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    38401 2021-03-26 21:19:02.000000 inStrain-1.7.4/inStrain/logUtils.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    15400 2023-05-16 19:23:03.000000 inStrain-1.7.4/inStrain/parse_annotations.py
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-05-16 19:27:49.546339 inStrain-1.7.4/inStrain/plotting/
+-rw-r--r--   0 mattolm    (501) staff       (20)     2524 2023-02-24 18:53:38.000000 inStrain-1.7.4/inStrain/plotting/SNV_plots.py
+-rw-r--r--   0 mattolm    (501) staff       (20)      662 2021-02-12 01:00:32.000000 inStrain-1.7.4/inStrain/plotting/__init__.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     9260 2023-02-25 01:38:35.000000 inStrain-1.7.4/inStrain/plotting/compare_plots.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     2548 2021-02-12 01:00:32.000000 inStrain-1.7.4/inStrain/plotting/gene_plots.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     6638 2023-02-24 18:50:29.000000 inStrain-1.7.4/inStrain/plotting/linkage_plots.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     9075 2023-02-25 00:47:19.000000 inStrain-1.7.4/inStrain/plotting/mapping_plots.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     5332 2023-02-25 00:49:14.000000 inStrain-1.7.4/inStrain/plotting/plotting_controller.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    18444 2023-02-24 18:53:38.000000 inStrain-1.7.4/inStrain/plotting/positional_plots.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     2831 2021-02-12 01:00:32.000000 inStrain-1.7.4/inStrain/plotting/utilities.py
+-rwxr-xr-x   0 mattolm    (501) staff       (20)    20710 2023-02-25 01:32:59.000000 inStrain-1.7.4/inStrain/polymorpher.py
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-05-16 19:27:49.547484 inStrain-1.7.4/inStrain/profile/
+-rw-r--r--   0 mattolm    (501) staff       (20)      636 2021-01-21 18:18:24.000000 inStrain-1.7.4/inStrain/profile/__init__.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     5822 2021-02-12 01:00:32.000000 inStrain-1.7.4/inStrain/profile/fasta.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     9115 2021-01-21 18:18:24.000000 inStrain-1.7.4/inStrain/profile/linkage.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    15636 2021-01-21 18:18:24.000000 inStrain-1.7.4/inStrain/profile/profile_controller.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    32820 2023-02-24 18:17:07.000000 inStrain-1.7.4/inStrain/profile/profile_utilities.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     3144 2021-02-17 23:42:47.000000 inStrain-1.7.4/inStrain/profile/samtools_ops.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    10361 2021-02-12 01:00:32.000000 inStrain-1.7.4/inStrain/profile/snv_utilities.py
+-rwxr-xr-x   0 mattolm    (501) staff       (20)     5332 2021-02-12 01:00:32.000000 inStrain-1.7.4/inStrain/quickProfile.py
+-rwxr-xr-x   0 mattolm    (501) staff       (20)    16916 2022-06-10 19:12:50.000000 inStrain-1.7.4/inStrain/readComparer.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     2629 2023-02-25 01:49:24.000000 inStrain-1.7.4/inStrain/utils.py
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-05-16 19:27:49.540746 inStrain-1.7.4/inStrain.egg-info/
+-rw-r--r--   0 mattolm    (501) staff       (20)      279 2023-05-16 19:27:49.000000 inStrain-1.7.4/inStrain.egg-info/PKG-INFO
+-rw-r--r--   0 mattolm    (501) staff       (20)     1563 2023-05-16 19:27:49.000000 inStrain-1.7.4/inStrain.egg-info/SOURCES.txt
+-rw-r--r--   0 mattolm    (501) staff       (20)        1 2023-05-16 19:27:49.000000 inStrain-1.7.4/inStrain.egg-info/dependency_links.txt
+-rw-r--r--   0 mattolm    (501) staff       (20)        1 2023-02-25 02:21:32.000000 inStrain-1.7.4/inStrain.egg-info/not-zip-safe
+-rw-r--r--   0 mattolm    (501) staff       (20)      113 2023-05-16 19:27:49.000000 inStrain-1.7.4/inStrain.egg-info/requires.txt
+-rw-r--r--   0 mattolm    (501) staff       (20)       16 2023-05-16 19:27:49.000000 inStrain-1.7.4/inStrain.egg-info/top_level.txt
+-rw-r--r--   0 mattolm    (501) staff       (20)       38 2023-05-16 19:27:49.548223 inStrain-1.7.4/setup.cfg
+-rw-r--r--   0 mattolm    (501) staff       (20)     1051 2023-02-25 02:18:49.000000 inStrain-1.7.4/setup.py
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-05-16 19:27:49.547728 inStrain-1.7.4/test/
+-rwxr-xr-x   0 mattolm    (501) staff       (20)     1213 2022-06-10 19:12:50.000000 inStrain-1.7.4/test/test_suite.py
```

### Comparing `inStrain-1.7.1/README.md` & `inStrain-1.7.4/README.md`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.1/bin/inStrain` & `inStrain-1.7.4/bin/inStrain`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.1/docker/job_utils.py` & `inStrain-1.7.4/docker/job_utils.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.1/docker/run_instrain.py` & `inStrain-1.7.4/docker/run_instrain.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.1/docker/s3_utils.py` & `inStrain-1.7.4/docker/s3_utils.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.1/inStrain/GeneProfile.py` & `inStrain-1.7.4/inStrain/GeneProfile.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.1/inStrain/SNVprofile.py` & `inStrain-1.7.4/inStrain/SNVprofile.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.1/inStrain/argumentParser.py` & `inStrain-1.7.4/inStrain/argumentParser.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.1/inStrain/compare_controller.py` & `inStrain-1.7.4/inStrain/compare_controller.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.1/inStrain/compare_greedy.py` & `inStrain-1.7.4/inStrain/compare_greedy.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.1/inStrain/compare_utils.py` & `inStrain-1.7.4/inStrain/compare_utils.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.1/inStrain/controller.py` & `inStrain-1.7.4/inStrain/controller.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.1/inStrain/deprecated/DEPRECATEDmapping_plots.py` & `inStrain-1.7.4/inStrain/deprecated/DEPRECATEDmapping_plots.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.1/inStrain/deprecated/__init__.py` & `inStrain-1.7.4/inStrain/deprecated/__init__.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.1/inStrain/deprecated/deprecated_filter_reads.py` & `inStrain-1.7.4/inStrain/deprecated/deprecated_filter_reads.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.1/inStrain/deprecated/deprecated_gene_statistics.py` & `inStrain-1.7.4/inStrain/deprecated/deprecated_gene_statistics.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.1/inStrain/deprecated/plottingUtilities.py` & `inStrain-1.7.4/inStrain/deprecated/plottingUtilities.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.1/inStrain/filter_reads.py` & `inStrain-1.7.4/inStrain/filter_reads.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.1/inStrain/genomeUtilities.py` & `inStrain-1.7.4/inStrain/genomeUtilities.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.1/inStrain/helper_files/NullModel.txt` & `inStrain-1.7.4/inStrain/helper_files/NullModel.txt`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.1/inStrain/irep_utilities.py` & `inStrain-1.7.4/inStrain/irep_utilities.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.1/inStrain/logUtils.py` & `inStrain-1.7.4/inStrain/logUtils.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.1/inStrain/parse_annotations.py` & `inStrain-1.7.4/inStrain/parse_annotations.py`

 * *Files 16% similar despite different names*

```diff
@@ -116,18 +116,18 @@
 
     def gene_calculations_wrapper(self):
         # Calculate summary stats
         sdb = calculate_gene_sum_stats(self.gene_tables, self.names, **self.kwargs)
         self.totals_db = sdb
 
         # Calculate annotation counts
-        s2a2vals = calculate_annotation_counts(self.gene_tables, self.names, **self.kwargs)
+        s2a2g2vals = calculate_annotation_counts2(self.gene_tables, self.names, **self.kwargs)
 
         # Create tables
-        metric2table = create_annotation_tables(sdb, s2a2vals, **self.kwargs)
+        metric2table = create_annotation_tables2(sdb, s2a2g2vals, **self.kwargs)
         self.metric2tables = metric2table
 
     def store_results(self):
         # Store raw data
         if self.kwargs.get('store_rawdata', False):
             self.OD.store('gene2anno', self.gene2anno, 'dictionary', 'Dictionary of genes 2 annotations')
 
@@ -157,44 +157,14 @@
 See documentation for output descriptions - https://instrain.readthedocs.io/en/latest/
 
 $$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$
                 """.format(Sprofile.get_location('output'), \
                            Sprofile.get_location('log'))
         logging.info(message)
 
-# def load_annotation_table(locs):
-#     """
-#     Load the annotation table
-#
-#     Input can either be a list of file locations or just 1 file location
-#     """
-#     gene2annos = {}
-#
-#     if type(locs) != type([]):
-#         locs = [locs]
-#
-#     for loc in locs:
-#         adb = pd.read_csv(loc, sep=',', dtype='string')
-#
-#         # Validate table
-#         for c in ['gene', 'anno']:
-#             if c not in list(adb.columns):
-#                 m = f"The required column {c} is not in your annotation table {loc}!"
-#                 print(m)
-#                 logging.error(m)
-#                 raise Exception(m)
-#
-#         # Store annos
-#         for gene, db in adb.groupby('gene'):
-#             if gene not in gene2annos:
-#                 gene2annos[gene] = set()
-#             gene2annos[gene] = gene2annos[gene].union(set(db['anno']))
-#
-#     return gene2annos
-
 def load_annotation_table2(locs):
     """
     Load the annotation table
 
     Input can either be a list of file locations or just 1 file location
     """
     gene2annos = {}
@@ -262,65 +232,168 @@
 
         table['bases_mapped_to_genes'].append(int(db['mb'].sum()))
         table['detected_annotations'].append(sum([len(a) for a in db['annos'] if a == a]))
         table['detected_genes_with_anno'].append(len(db[~db['annos'].isna()]))
 
     return pd.DataFrame(table)
 
-def calculate_annotation_counts(gdbs, names, **kwargs):
+# def calculate_annotation_counts(gdbs, names, **kwargs):
+#     """
+#     Create sample2accession2values
+#     """
+#     s2a2vals = {}
+#     for db, name in tqdm(zip(gdbs, names), total=len(names), desc='Calculating anno metrics'):
+#         # Create "accession to values"
+#         # values = [genomes, # genes, # bases]
+#         a2vals = {}
+#         for i, row in db[~db['annos'].isna()].iterrows():
+#             kos = row['annos']
+#             if 'genome' in row:
+#                 genome = row['genome']
+#             else:
+#                 genome = None
+#             for k in kos:
+#                 if k in a2vals:
+#                     a2vals[k][0] = a2vals[k][0].union(set([genome]))
+#                     a2vals[k][1] += 1
+#                     a2vals[k][2] += row['mb']
+#                 else:
+#                     a2vals[k] = [set([genome]), 1, row['mb']]
+#         s2a2vals[name] = a2vals
+#     return s2a2vals
+
+def calculate_annotation_counts2(gdbs, names, **kwargs):
     """
-    Create sample2accession2values
+    Create sample2accession2genome2values
     """
-    s2a2vals = {}
+    s2a2g2vals = {}
     for db, name in tqdm(zip(gdbs, names), total=len(names), desc='Calculating anno metrics'):
-        # Create "accession to values"
+        # Create "accession to genome to values"
         # values = [genomes, # genes, # bases]
-        a2vals = {}
+        a2g2vals = {}
         for i, row in db[~db['annos'].isna()].iterrows():
             kos = row['annos']
             if 'genome' in row:
-                genome = row['genome']
+                g = row['genome']
             else:
-                genome = None
+                g = None
             for k in kos:
-                if k in a2vals:
-                    a2vals[k][0] = a2vals[k][0].union(set([genome]))
-                    a2vals[k][1] += 1
-                    a2vals[k][2] += row['mb']
+
+                if k not in a2g2vals:
+                    a2g2vals[k] = {}
+
+                if g in a2g2vals[k]:
+                    a2g2vals[k][g][0] = a2g2vals[k][g][0].union(set([g]))
+                    a2g2vals[k][g][1] += 1
+                    a2g2vals[k][g][2] += row['mb']
                 else:
-                    a2vals[k] = [set([genome]), 1, row['mb']]
-        s2a2vals[name] = a2vals
-    return s2a2vals
+                    a2g2vals[k][g] = [set([g]), 1, row['mb']]
+        s2a2g2vals[name] = a2g2vals
+    return s2a2g2vals
 
-def create_annotation_tables(sdb, s2a2vals, **kwargs):
+# def create_annotation_tables(sdb, s2a2vals, **kwargs):
+#     """
+#     Create the actual tables that can be used for stats and whatnot
+#     """
+#     if 'detected_genomes' in set(sdb.columns):
+#         METRICS = ['genes', 'bases', 'genomes']
+#     else:
+#         METRICS = ['genes', 'bases']
+#
+#     metric2table = {}
+#     for metric in METRICS:
+#         metric2table[metric] = defaultdict(list)
+#
+#     TOTAL_KOS = set()
+#     for s, a2vals in s2a2vals.items():
+#         TOTAL_KOS = TOTAL_KOS.union(set(a2vals.keys()))
+#
+#     for sample, a2vals in s2a2vals.items():
+#         for metric in METRICS:
+#             metric2table[metric]['sample'].append(sample)
+#
+#         for KO in sorted(list(TOTAL_KOS)):
+#             if KO in a2vals:
+#                 genomes = len(a2vals[KO][0])
+#                 genes = a2vals[KO][1]
+#                 bases = a2vals[KO][2]
+#             else:
+#                 genomes = 0
+#                 genes = 0
+#                 bases = 0
+#
+#             for metric in METRICS:
+#                 if metric == 'genes':
+#                     val = genes
+#                 elif metric == 'bases':
+#                     val = bases
+#                 elif metric == 'genomes':
+#                     val = genomes
+#                 else:
+#                     assert False
+#                 metric2table[metric][KO].append(val)
+#
+#     for metric in METRICS:
+#         metric2table[metric] = pd.DataFrame(metric2table[metric])
+#
+#     # Calculate the percentage metrics
+#     for metric in METRICS:
+#         if metric == 'genes':
+#             s2norm = sdb.set_index('sample')['detected_genes'].to_dict()
+#         elif metric == 'bases':
+#             s2norm = sdb.set_index('sample')['bases_mapped_to_genes'].to_dict()
+#         elif metric == 'genomes':
+#             s2norm = sdb.set_index('sample')['detected_genomes'].to_dict()
+#         else:
+#             assert False
+#
+#         db = metric2table[metric].copy()
+#         for d in TOTAL_KOS:
+#             db[d] = [x / s2norm[s] for x, s in zip(db[d], db['sample'])]
+#
+#         metric2table[metric + '_fraction'] = db
+#
+#     # Calculate the long-form table
+#     table = defaultdict(list)
+#     for sample, a2vals in s2a2vals.items():
+#         for a, vals in a2vals.items():
+#             table['sample'].append(sample)
+#             table['anno'].append(a)
+#             for name, thing in zip(['genomes', 'genes', 'bases'], vals):
+#                 table[name].append(thing)
+#     metric2table["long_data"] = pd.DataFrame(table)
+#
+#     return metric2table
+
+def create_annotation_tables2(sdb, s2a2g2vals, **kwargs):
     """
     Create the actual tables that can be used for stats and whatnot
     """
     if 'detected_genomes' in set(sdb.columns):
         METRICS = ['genes', 'bases', 'genomes']
     else:
         METRICS = ['genes', 'bases']
 
     metric2table = {}
     for metric in METRICS:
         metric2table[metric] = defaultdict(list)
 
     TOTAL_KOS = set()
-    for s, a2vals in s2a2vals.items():
-        TOTAL_KOS = TOTAL_KOS.union(set(a2vals.keys()))
+    for s, a2g2vals in s2a2g2vals.items():
+        TOTAL_KOS = TOTAL_KOS.union(set(a2g2vals.keys()))
 
-    for sample, a2vals in s2a2vals.items():
+    for sample, a2g2vals in s2a2g2vals.items():
         for metric in METRICS:
             metric2table[metric]['sample'].append(sample)
 
         for KO in sorted(list(TOTAL_KOS)):
-            if KO in a2vals:
-                genomes = len(a2vals[KO][0])
-                genes = a2vals[KO][1]
-                bases = a2vals[KO][2]
+            if KO in a2g2vals:
+                genomes = len(a2g2vals[KO].keys())
+                genes = sum([a2vals[1] for g, a2vals in a2g2vals[KO].items()])
+                bases = sum([a2vals[2] for g, a2vals in a2g2vals[KO].items()])
             else:
                 genomes = 0
                 genes = 0
                 bases = 0
 
             for metric in METRICS:
                 if metric == 'genes':
@@ -345,22 +418,49 @@
         elif metric == 'genomes':
             s2norm = sdb.set_index('sample')['detected_genomes'].to_dict()
         else:
             assert False
 
         db = metric2table[metric].copy()
         for d in TOTAL_KOS:
-            db[d] = [x / s2norm[s] for x, s in zip(db[d], db['sample'])]
+            if s2norm[s] == 0:
+                db[d] = 0
+            else:
+                db[d] = [x / s2norm[s] for x, s in zip(db[d], db['sample'])]
 
         metric2table[metric + '_fraction'] = db
 
     # Calculate the long-form table
     table = defaultdict(list)
-    for sample, a2vals in s2a2vals.items():
-        for a, vals in a2vals.items():
-            table['sample'].append(sample)
-            table['anno'].append(a)
-            for name, thing in zip(['genomes', 'genes', 'bases'], vals):
-                table[name].append(thing)
+    for sample, a2g2vals in s2a2g2vals.items():
+        for a, g2vals in a2g2vals.items():
+            for g, vals in g2vals.items():
+                table['sample'].append(sample)
+                table['anno'].append(a)
+                table['genome'].append(g)
+                for name, thing in zip(['genomes', 'genes', 'bases'], vals):
+                    if name == 'genomes':
+                        continue
+                    table[name].append(thing)
     metric2table["long_data"] = pd.DataFrame(table)
 
-    return metric2table
+    return metric2table
+
+def load_s2a2g2vals(loc):
+    """
+    Create s2a2g2vals from long_data
+    """
+
+    s2a2g2vals = {}
+    bdb = pd.read_csv(loc)
+    for i, row in bdb.iterrows():
+        s = row['sample']
+        g = row['genome']
+        a = row['anno']
+
+        if s not in s2a2g2vals:
+            s2a2g2vals[s] = {}
+        if a not in s2a2g2vals[s]:
+            s2a2g2vals[s][a] = {}
+        s2a2g2vals[s][a][g] = [set([g]), row['genes'], row['bases']]
+
+    return s2a2g2vals
```

### Comparing `inStrain-1.7.1/inStrain/plotting/SNV_plots.py` & `inStrain-1.7.4/inStrain/plotting/SNV_plots.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.1/inStrain/plotting/__init__.py` & `inStrain-1.7.4/inStrain/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.1/inStrain/plotting/compare_plots.py` & `inStrain-1.7.4/inStrain/plotting/compare_plots.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.1/inStrain/plotting/gene_plots.py` & `inStrain-1.7.4/inStrain/plotting/gene_plots.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.1/inStrain/plotting/linkage_plots.py` & `inStrain-1.7.4/inStrain/plotting/linkage_plots.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.1/inStrain/plotting/mapping_plots.py` & `inStrain-1.7.4/inStrain/plotting/mapping_plots.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.1/inStrain/plotting/plotting_controller.py` & `inStrain-1.7.4/inStrain/plotting/plotting_controller.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.1/inStrain/plotting/positional_plots.py` & `inStrain-1.7.4/inStrain/plotting/positional_plots.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.1/inStrain/plotting/utilities.py` & `inStrain-1.7.4/inStrain/plotting/utilities.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.1/inStrain/polymorpher.py` & `inStrain-1.7.4/inStrain/polymorpher.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.1/inStrain/profile/__init__.py` & `inStrain-1.7.4/inStrain/profile/__init__.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.1/inStrain/profile/fasta.py` & `inStrain-1.7.4/inStrain/profile/fasta.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.1/inStrain/profile/linkage.py` & `inStrain-1.7.4/inStrain/profile/linkage.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.1/inStrain/profile/profile_controller.py` & `inStrain-1.7.4/inStrain/profile/profile_controller.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.1/inStrain/profile/profile_utilities.py` & `inStrain-1.7.4/inStrain/profile/profile_utilities.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.1/inStrain/profile/samtools_ops.py` & `inStrain-1.7.4/inStrain/profile/samtools_ops.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.1/inStrain/profile/snv_utilities.py` & `inStrain-1.7.4/inStrain/profile/snv_utilities.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.1/inStrain/quickProfile.py` & `inStrain-1.7.4/inStrain/quickProfile.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.1/inStrain/readComparer.py` & `inStrain-1.7.4/inStrain/readComparer.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.1/inStrain/utils.py` & `inStrain-1.7.4/inStrain/utils.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.1/inStrain.egg-info/SOURCES.txt` & `inStrain-1.7.4/inStrain.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 bin/inStrain
 docker/__init__.py
 docker/job_utils.py
 docker/run_instrain.py
 docker/s3_utils.py
```

### Comparing `inStrain-1.7.1/setup.py` & `inStrain-1.7.4/setup.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.1/test/test_suite.py` & `inStrain-1.7.4/test/test_suite.py`

 * *Files identical despite different names*

