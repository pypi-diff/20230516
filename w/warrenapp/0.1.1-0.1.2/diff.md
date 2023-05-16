# Comparing `tmp/warrenapp-0.1.1.tar.gz` & `tmp/warrenapp-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "warrenapp-0.1.1.tar", last modified: Mon May  8 18:57:45 2023, max compression
+gzip compressed data, was "warrenapp-0.1.2.tar", last modified: Tue May 16 17:30:55 2023, max compression
```

## Comparing `warrenapp-0.1.1.tar` & `warrenapp-0.1.2.tar`

### file list

```diff
@@ -1,56 +1,59 @@
-drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-08 18:57:45.562255 warrenapp-0.1.1/
--rw-r--r--   0 sweav     (1001) sweav     (1001)     1521 2023-05-04 20:41:15.000000 warrenapp-0.1.1/LICENSE
--rw-rw-r--   0 sweav     (1001) sweav     (1001)     3615 2023-05-08 18:57:45.558255 warrenapp-0.1.1/PKG-INFO
--rw-r--r--   0 sweav     (1001) sweav     (1001)     1405 2023-05-05 00:01:17.000000 warrenapp-0.1.1/README.md
--rw-r--r--   0 sweav     (1001) sweav     (1001)     1351 2023-05-08 18:35:34.000000 warrenapp-0.1.1/pyproject.toml
--rw-rw-r--   0 sweav     (1001) sweav     (1001)       38 2023-05-08 18:57:45.562255 warrenapp-0.1.1/setup.cfg
--rw-r--r--   0 sweav     (1001) sweav     (1001)      245 2023-05-04 23:54:39.000000 warrenapp-0.1.1/setup.py
-drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-08 18:57:45.554255 warrenapp-0.1.1/src/
-drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-08 18:57:45.554255 warrenapp-0.1.1/src/warrenapp/
--rw-r--r--   0 sweav     (1001) sweav     (1001)       24 2023-05-04 20:41:15.000000 warrenapp-0.1.1/src/warrenapp/__init__.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)      281 2023-05-04 23:54:00.000000 warrenapp-0.1.1/src/warrenapp/apps.py
-drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-08 18:57:45.554255 warrenapp-0.1.1/src/warrenapp/badelf_tools/
--rw-rw-r--   0 sweav     (1001) sweav     (1001)     4776 2023-05-08 18:36:02.000000 warrenapp-0.1.1/src/warrenapp/badelf_tools/acf.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)    20158 2023-05-04 20:41:15.000000 warrenapp-0.1.1/src/warrenapp/badelf_tools/badelf_algorithm_functions.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)    13809 2023-05-08 16:36:29.000000 warrenapp-0.1.1/src/warrenapp/badelf_tools/utilities.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)     5179 2023-05-08 18:36:04.000000 warrenapp-0.1.1/src/warrenapp/models.py
-drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-08 18:57:45.554255 warrenapp-0.1.1/src/warrenapp/workflows/
--rw-r--r--   0 sweav     (1001) sweav     (1001)     1394 2023-05-08 18:36:04.000000 warrenapp-0.1.1/src/warrenapp/workflows/__init__.py
-drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-08 18:57:45.558255 warrenapp-0.1.1/src/warrenapp/workflows/population_analysis/
--rw-r--r--   0 sweav     (1001) sweav     (1001)     1177 2023-05-08 18:36:04.000000 warrenapp-0.1.1/src/warrenapp/workflows/population_analysis/__init__.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)     1703 2023-05-08 18:36:02.000000 warrenapp-0.1.1/src/warrenapp/workflows/population_analysis/badelf_hse.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)     1387 2023-05-05 00:04:23.000000 warrenapp-0.1.1/src/warrenapp/workflows/population_analysis/badelf_pbe.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)     1712 2023-05-08 18:36:04.000000 warrenapp-0.1.1/src/warrenapp/workflows/population_analysis/bader_badelf_hse.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)     1350 2023-05-08 15:51:16.000000 warrenapp-0.1.1/src/warrenapp/workflows/population_analysis/bader_badelf_pbe.py
--rw-rw-r--   0 sweav     (1001) sweav     (1001)      931 2023-05-08 18:36:04.000000 warrenapp-0.1.1/src/warrenapp/workflows/population_analysis/bader_badelf_relaxation_hse.py
--rw-rw-r--   0 sweav     (1001) sweav     (1001)      874 2023-05-08 18:36:04.000000 warrenapp-0.1.1/src/warrenapp/workflows/population_analysis/bader_badelf_relaxation_pbe.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)     1595 2023-05-08 18:36:02.000000 warrenapp-0.1.1/src/warrenapp/workflows/population_analysis/bader_hse.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)     1401 2023-05-05 00:04:23.000000 warrenapp-0.1.1/src/warrenapp/workflows/population_analysis/bader_pbe.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)    15457 2023-05-08 15:20:27.000000 warrenapp-0.1.1/src/warrenapp/workflows/population_analysis/base.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)      903 2023-05-04 23:50:58.000000 warrenapp-0.1.1/src/warrenapp/workflows/population_analysis/elf_hse.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)      903 2023-05-04 23:50:58.000000 warrenapp-0.1.1/src/warrenapp/workflows/population_analysis/elf_pbe.py
--rw-rw-r--   0 sweav     (1001) sweav     (1001)     2171 2023-05-08 18:36:04.000000 warrenapp-0.1.1/src/warrenapp/workflows/population_analysis/relaxation_base.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)    13893 2023-05-05 00:04:23.000000 warrenapp-0.1.1/src/warrenapp/workflows/population_analysis/warren_badelf_v3_7.py
-drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-08 18:57:45.558255 warrenapp-0.1.1/src/warrenapp/workflows/relaxation/
--rw-r--r--   0 sweav     (1001) sweav     (1001)      296 2023-05-04 20:41:15.000000 warrenapp-0.1.1/src/warrenapp/workflows/relaxation/__init__.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)      624 2023-05-04 23:52:02.000000 warrenapp-0.1.1/src/warrenapp/workflows/relaxation/hse.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)      545 2023-05-04 23:52:02.000000 warrenapp-0.1.1/src/warrenapp/workflows/relaxation/hsesol.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)     4621 2023-05-05 00:04:23.000000 warrenapp-0.1.1/src/warrenapp/workflows/relaxation/pbe.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)      503 2023-05-04 23:52:02.000000 warrenapp-0.1.1/src/warrenapp/workflows/relaxation/pbe_metal.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)      443 2023-05-04 23:52:02.000000 warrenapp-0.1.1/src/warrenapp/workflows/relaxation/pbesol.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)      702 2023-05-04 23:52:02.000000 warrenapp-0.1.1/src/warrenapp/workflows/relaxation/scan.py
-drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-08 18:57:45.558255 warrenapp-0.1.1/src/warrenapp/workflows/static_energy/
--rw-r--r--   0 sweav     (1001) sweav     (1001)      364 2023-05-08 17:14:12.000000 warrenapp-0.1.1/src/warrenapp/workflows/static_energy/__init__.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)      431 2023-05-04 23:53:18.000000 warrenapp-0.1.1/src/warrenapp/workflows/static_energy/hse.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)      449 2023-05-04 23:53:18.000000 warrenapp-0.1.1/src/warrenapp/workflows/static_energy/hsesol.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)      764 2023-05-08 17:18:15.000000 warrenapp-0.1.1/src/warrenapp/workflows/static_energy/pbe.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)      474 2023-05-04 23:53:18.000000 warrenapp-0.1.1/src/warrenapp/workflows/static_energy/pbe_metal.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)      567 2023-05-08 18:34:55.000000 warrenapp-0.1.1/src/warrenapp/workflows/static_energy/pbesol.py
--rw-r--r--   0 sweav     (1001) sweav     (1001)      437 2023-05-04 23:53:18.000000 warrenapp-0.1.1/src/warrenapp/workflows/static_energy/scan.py
--rw-rw-r--   0 sweav     (1001) sweav     (1001)     2137 2023-05-08 18:36:04.000000 warrenapp-0.1.1/src/warrenapp/workflows/static_energy/seeded_hse.py
-drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-08 18:57:45.554255 warrenapp-0.1.1/src/warrenapp.egg-info/
--rw-rw-r--   0 sweav     (1001) sweav     (1001)     3615 2023-05-08 18:57:45.000000 warrenapp-0.1.1/src/warrenapp.egg-info/PKG-INFO
--rw-rw-r--   0 sweav     (1001) sweav     (1001)     2016 2023-05-08 18:57:45.000000 warrenapp-0.1.1/src/warrenapp.egg-info/SOURCES.txt
--rw-rw-r--   0 sweav     (1001) sweav     (1001)        1 2023-05-08 18:57:45.000000 warrenapp-0.1.1/src/warrenapp.egg-info/dependency_links.txt
--rw-rw-r--   0 sweav     (1001) sweav     (1001)        8 2023-05-08 18:57:45.000000 warrenapp-0.1.1/src/warrenapp.egg-info/requires.txt
--rw-rw-r--   0 sweav     (1001) sweav     (1001)       10 2023-05-08 18:57:45.000000 warrenapp-0.1.1/src/warrenapp.egg-info/top_level.txt
+drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-16 17:30:55.454624 warrenapp-0.1.2/
+-rw-r--r--   0 sweav     (1001) sweav     (1001)     1521 2023-05-04 20:41:15.000000 warrenapp-0.1.2/LICENSE
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)     3615 2023-05-16 17:30:55.454624 warrenapp-0.1.2/PKG-INFO
+-rw-r--r--   0 sweav     (1001) sweav     (1001)     1405 2023-05-05 00:01:17.000000 warrenapp-0.1.2/README.md
+-rw-r--r--   0 sweav     (1001) sweav     (1001)     1351 2023-05-16 17:24:45.000000 warrenapp-0.1.2/pyproject.toml
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)       38 2023-05-16 17:30:55.454624 warrenapp-0.1.2/setup.cfg
+-rw-r--r--   0 sweav     (1001) sweav     (1001)      245 2023-05-04 23:54:39.000000 warrenapp-0.1.2/setup.py
+drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-16 17:30:55.446624 warrenapp-0.1.2/src/
+drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-16 17:30:55.446624 warrenapp-0.1.2/src/warrenapp/
+-rw-r--r--   0 sweav     (1001) sweav     (1001)       24 2023-05-04 20:41:15.000000 warrenapp-0.1.2/src/warrenapp/__init__.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)      281 2023-05-04 23:54:00.000000 warrenapp-0.1.2/src/warrenapp/apps.py
+drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-16 17:30:55.446624 warrenapp-0.1.2/src/warrenapp/badelf_tools/
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)     4776 2023-05-08 18:36:02.000000 warrenapp-0.1.2/src/warrenapp/badelf_tools/acf.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)    20158 2023-05-04 20:41:15.000000 warrenapp-0.1.2/src/warrenapp/badelf_tools/badelf_algorithm_functions.py
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)    14535 2023-05-10 15:37:41.000000 warrenapp-0.1.2/src/warrenapp/badelf_tools/utilities.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)     5179 2023-05-08 18:36:04.000000 warrenapp-0.1.2/src/warrenapp/models.py
+drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-16 17:30:55.446624 warrenapp-0.1.2/src/warrenapp/workflows/
+-rw-r--r--   0 sweav     (1001) sweav     (1001)     1177 2023-05-16 17:24:13.000000 warrenapp-0.1.2/src/warrenapp/workflows/__init__.py
+drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-16 17:30:55.454624 warrenapp-0.1.2/src/warrenapp/workflows/nested_dft/
+-rw-r--r--   0 sweav     (1001) sweav     (1001)      187 2023-05-16 17:24:15.000000 warrenapp-0.1.2/src/warrenapp/workflows/nested_dft/__init__.py
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)      828 2023-05-16 17:24:15.000000 warrenapp-0.1.2/src/warrenapp/workflows/nested_dft/prepop_relaxation_static_hse.py
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)      816 2023-05-16 17:24:15.000000 warrenapp-0.1.2/src/warrenapp/workflows/nested_dft/prepop_relaxation_static_pbesol.py
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)     1778 2023-05-16 17:24:13.000000 warrenapp-0.1.2/src/warrenapp/workflows/nested_dft/relaxation_static_base.py
+drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-16 17:30:55.454624 warrenapp-0.1.2/src/warrenapp/workflows/population_analysis/
+-rw-r--r--   0 sweav     (1001) sweav     (1001)      752 2023-05-16 17:24:15.000000 warrenapp-0.1.2/src/warrenapp/workflows/population_analysis/__init__.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)      807 2023-05-16 17:24:15.000000 warrenapp-0.1.2/src/warrenapp/workflows/population_analysis/badelf_hse.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)      622 2023-05-16 17:24:15.000000 warrenapp-0.1.2/src/warrenapp/workflows/population_analysis/badelf_pbesol.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)      637 2023-05-16 17:24:15.000000 warrenapp-0.1.2/src/warrenapp/workflows/population_analysis/bader_badelf_hse.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)      650 2023-05-16 17:24:15.000000 warrenapp-0.1.2/src/warrenapp/workflows/population_analysis/bader_badelf_pbesol.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)      651 2023-05-16 17:24:15.000000 warrenapp-0.1.2/src/warrenapp/workflows/population_analysis/bader_hse.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)      742 2023-05-16 17:24:15.000000 warrenapp-0.1.2/src/warrenapp/workflows/population_analysis/bader_pbesol.py
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)    15145 2023-05-16 17:24:13.000000 warrenapp-0.1.2/src/warrenapp/workflows/population_analysis/base.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)      903 2023-05-04 23:50:58.000000 warrenapp-0.1.2/src/warrenapp/workflows/population_analysis/elf_hse.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)      921 2023-05-16 17:22:25.000000 warrenapp-0.1.2/src/warrenapp/workflows/population_analysis/elf_pbesol.py
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)     3958 2023-05-16 17:24:15.000000 warrenapp-0.1.2/src/warrenapp/workflows/population_analysis/prebader_badelf_dft.py
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)    14056 2023-05-16 17:24:13.000000 warrenapp-0.1.2/src/warrenapp/workflows/population_analysis/warren_badelf_v3_7.py
+drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-16 17:30:55.454624 warrenapp-0.1.2/src/warrenapp/workflows/relaxation/
+-rw-r--r--   0 sweav     (1001) sweav     (1001)      296 2023-05-04 20:41:15.000000 warrenapp-0.1.2/src/warrenapp/workflows/relaxation/__init__.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)      963 2023-05-16 17:24:13.000000 warrenapp-0.1.2/src/warrenapp/workflows/relaxation/hse.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)      545 2023-05-04 23:52:02.000000 warrenapp-0.1.2/src/warrenapp/workflows/relaxation/hsesol.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)     4621 2023-05-05 00:04:23.000000 warrenapp-0.1.2/src/warrenapp/workflows/relaxation/pbe.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)      503 2023-05-04 23:52:02.000000 warrenapp-0.1.2/src/warrenapp/workflows/relaxation/pbe_metal.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)      443 2023-05-04 23:52:02.000000 warrenapp-0.1.2/src/warrenapp/workflows/relaxation/pbesol.py
+-rw-r--r--   0 sweav     (1001) sweav     (1001)      702 2023-05-04 23:52:02.000000 warrenapp-0.1.2/src/warrenapp/workflows/relaxation/scan.py
+drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-16 17:30:55.454624 warrenapp-0.1.2/src/warrenapp/workflows/static_energy/
+-rw-r--r--   0 sweav     (1001) sweav     (1001)      364 2023-05-08 17:14:12.000000 warrenapp-0.1.2/src/warrenapp/workflows/static_energy/__init__.py
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)      874 2023-05-16 17:24:13.000000 warrenapp-0.1.2/src/warrenapp/workflows/static_energy/hse.py
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)      457 2023-05-16 17:24:13.000000 warrenapp-0.1.2/src/warrenapp/workflows/static_energy/hsesol.py
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)      772 2023-05-10 15:37:41.000000 warrenapp-0.1.2/src/warrenapp/workflows/static_energy/pbe.py
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)      482 2023-05-10 15:37:41.000000 warrenapp-0.1.2/src/warrenapp/workflows/static_energy/pbe_metal.py
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)      575 2023-05-10 15:37:41.000000 warrenapp-0.1.2/src/warrenapp/workflows/static_energy/pbesol.py
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)      445 2023-05-10 15:37:41.000000 warrenapp-0.1.2/src/warrenapp/workflows/static_energy/scan.py
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)     2136 2023-05-08 21:19:01.000000 warrenapp-0.1.2/src/warrenapp/workflows/static_energy/seeded_hse.py
+drwxrwxr-x   0 sweav     (1001) sweav     (1001)        0 2023-05-16 17:30:55.446624 warrenapp-0.1.2/src/warrenapp.egg-info/
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)     3615 2023-05-16 17:30:55.000000 warrenapp-0.1.2/src/warrenapp.egg-info/PKG-INFO
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)     2127 2023-05-16 17:30:55.000000 warrenapp-0.1.2/src/warrenapp.egg-info/SOURCES.txt
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)        1 2023-05-16 17:30:55.000000 warrenapp-0.1.2/src/warrenapp.egg-info/dependency_links.txt
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)        8 2023-05-16 17:30:55.000000 warrenapp-0.1.2/src/warrenapp.egg-info/requires.txt
+-rw-rw-r--   0 sweav     (1001) sweav     (1001)       10 2023-05-16 17:30:55.000000 warrenapp-0.1.2/src/warrenapp.egg-info/top_level.txt
```

### Comparing `warrenapp-0.1.1/LICENSE` & `warrenapp-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `warrenapp-0.1.1/PKG-INFO` & `warrenapp-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warrenapp
-Version: 0.1.1
+Version: 0.1.2
 Summary: The Warrenapp is an extension of the Simulated Materials Ecosystem (Simmate), a package designed to ease computational materials research. The WarrenApp adds several custom workflows and settings.
 Author-email: Sam Weaver <sweav@unc.edu>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Sam M. Weaver
         All rights reserved.
```

### Comparing `warrenapp-0.1.1/README.md` & `warrenapp-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `warrenapp-0.1.1/pyproject.toml` & `warrenapp-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 [build-system]
 requires = ["setuptools>=64.0.0", "wheel"]
 build-backend= "setuptools.build_meta"
 
 [project]
 name = "warrenapp"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = ["simmate"]
 description = "The Warrenapp is an extension of the Simulated Materials Ecosystem (Simmate), a package designed to ease computational materials research. The WarrenApp adds several custom workflows and settings."
 readme = "README.md"
 requires-python=">=3.10"
 authors = [{ name = "Sam Weaver", email = "sweav@unc.edu" }]
 license = { file = "LICENSE" }
```

### Comparing `warrenapp-0.1.1/src/warrenapp/badelf_tools/acf.py` & `warrenapp-0.1.2/src/warrenapp/badelf_tools/acf.py`

 * *Files identical despite different names*

### Comparing `warrenapp-0.1.1/src/warrenapp/badelf_tools/badelf_algorithm_functions.py` & `warrenapp-0.1.2/src/warrenapp/badelf_tools/badelf_algorithm_functions.py`

 * *Files identical despite different names*

### Comparing `warrenapp-0.1.1/src/warrenapp/badelf_tools/utilities.py` & `warrenapp-0.1.2/src/warrenapp/badelf_tools/utilities.py`

 * *Files 3% similar despite different names*

```diff
@@ -118,15 +118,15 @@
             """
         )
 
 
 def get_empties_from_bcf(
     directory: Path,
     structure: Structure,
-    min_charge: float = 0.1,
+    min_charge: float = 0.15,
 ):
     """
     Checks the BCF.dat output file from the Henkelman algorithm for charge
     maxima that are far from other atoms with large charges, and adds in "dummy"
     atoms at these sites. Returns a Structure object.
     """
     # Set the correct density file (CHGCAR or ELFCAR) to update depending on
@@ -206,14 +206,24 @@
     structure_empty = structure.copy()
     # sites_to_remove = []
     for charge_site in empty_sites:
         structure_empty.append(
             species="He", coords=charge_site, coords_are_cartesian=True
         )
 
+    # Sometimes the program finds two electride sites that are right next to
+    # eachother(maybe due to voxelation?). To account for this, we check through
+    # all of the sites in our structure and remove any that are close to eachother
+    # (within 0.3 angstrom. This is arbitrary and may need to be updated)
+    sites_to_remove = []
+    for site_index in range(len((structure_empty.sites))):
+        for other_site_index in range(site_index + 1, len(structure_empty.sites)):
+            if structure_empty.get_distance(site_index, other_site_index) < 0.3:
+                sites_to_remove.append(site_index)
+    structure_empty.remove_sites(sites_to_remove)
     return structure_empty
 
 
 # This function writes a file POSCAR_empty which contains the original structure
 # information from the POSCAR with the added lines for electride sites.
 def write_poscar_empty(directory: Path, structure_empty: Structure):
     """
@@ -314,26 +324,28 @@
             file.writelines(structure_lines)
             file.writelines(later_lines_to_keep)
 
 
 def get_density_file_empty(
     directory: Path,
     structure: Structure,
+    min_charge: float = 0.15,
     analysis_type: str = "badelf",
 ):
     """
     Checks the BCF.dat output file from the Henkelman algorithm for charge
     maxima that are far from other atoms with large charges, and adds in "dummy"
     atoms at these sites. This is meant to be used when searching for electrides
     or when working with known electrides.
     """
     # Get a structure object with empty atoms at electride sites
     structure_empty = get_empties_from_bcf(
         directory=directory,
         structure=structure,
+        min_charge=min_charge,
     )
 
     # Write the structure to a POSCAR_empty file. This must be in a specific format.
     # Here we take care of the formatting of lines 6 and on. The early lines
     # are handled in the replace_density_function function
     write_poscar_empty(directory=directory, structure_empty=structure_empty)
```

### Comparing `warrenapp-0.1.1/src/warrenapp/models.py` & `warrenapp-0.1.2/src/warrenapp/models.py`

 * *Files identical despite different names*

### Comparing `warrenapp-0.1.1/src/warrenapp/workflows/__init__.py` & `warrenapp-0.1.2/src/warrenapp/workflows/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 # -*- coding: utf-8 -*-
 
+from .nested_dft import (
+    Nested__Warren__RelaxationStaticHse,
+    Nested__Warren__RelaxationStaticPbesol,
+)
 from .population_analysis import (
     PopulationAnalysis__Warren__BadelfHse,
-    PopulationAnalysis__Warren__BadelfPbe,
+    PopulationAnalysis__Warren__BadelfPbesol,
     PopulationAnalysis__Warren__BaderBadelfHse,
-    PopulationAnalysis__Warren__BaderBadelfPbe,
-    PopulationAnalysis__Warren__BaderBadelfRelaxationHse,
-    PopulationAnalysis__Warren__BaderBadelfRelaxationPbe,
+    PopulationAnalysis__Warren__BaderBadelfPbesol,
     PopulationAnalysis__Warren__BaderHse,
-    PopulationAnalysis__Warren__BaderPbe,
+    PopulationAnalysis__Warren__BaderPbesol,
     PopulationAnalysis__Warren__ElfHse,
-    PopulationAnalysis__Warren__ElfPbe,
+    PopulationAnalysis__Warren__ElfPbesol,
     StaticEnergy__Warren__PrebadelfHse,
-    StaticEnergy__Warren__PrebadelfPbe,
-    StaticEnergy__Warren__PrebadelfSeededHse,
-    StaticEnergy__Warren__PrebaderbadelfHse,
-    StaticEnergy__Warren__PrebaderbadelfPbe,
-    StaticEnergy__Warren__PrebaderbadelfSeededHse,
+    StaticEnergy__Warren__PrebadelfPbesol,
     StaticEnergy__Warren__PrebaderHse,
-    StaticEnergy__Warren__PrebaderPbe,
-    StaticEnergy__Warren__PrebaderSeededHse,
+    StaticEnergy__Warren__PrebaderPbesol,
 )
 from .relaxation import (
     Relaxation__Warren__Hse,
     Relaxation__Warren__Hsesol,
     Relaxation__Warren__Pbe,
     Relaxation__Warren__PbeMetal,
     Relaxation__Warren__Pbesol,
```

### Comparing `warrenapp-0.1.1/src/warrenapp/workflows/population_analysis/bader_badelf_relaxation_hse.py` & `warrenapp-0.1.2/src/warrenapp/workflows/population_analysis/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,16 @@
 # -*- coding: utf-8 -*-
 
-from warrenapp.workflows.population_analysis import (
-    PopulationAnalysis__Warren__BaderBadelfHse,
+from .badelf_hse import PopulationAnalysis__Warren__BadelfHse
+from .badelf_pbesol import PopulationAnalysis__Warren__BadelfPbesol
+from .bader_badelf_hse import PopulationAnalysis__Warren__BaderBadelfHse
+from .bader_badelf_pbesol import PopulationAnalysis__Warren__BaderBadelfPbesol
+from .bader_hse import PopulationAnalysis__Warren__BaderHse
+from .bader_pbesol import PopulationAnalysis__Warren__BaderPbesol
+from .elf_hse import PopulationAnalysis__Warren__ElfHse
+from .elf_pbesol import PopulationAnalysis__Warren__ElfPbesol
+from .prebader_badelf_dft import (
+    StaticEnergy__Warren__PrebadelfHse,
+    StaticEnergy__Warren__PrebadelfPbesol,
+    StaticEnergy__Warren__PrebaderHse,
+    StaticEnergy__Warren__PrebaderPbesol,
 )
-from warrenapp.workflows.population_analysis.relaxation_base import (
-    BaderBadelfRelaxationBase,
-)
-from warrenapp.workflows.relaxation.pbesol import Relaxation__Warren__Pbesol
-
-
-# This workflow will run
-class PopulationAnalysis__Warren__BaderBadelfRelaxationHse(BaderBadelfRelaxationBase):
-    """
-    Runs a PBE quality structure relaxation, an HSE quality static energy
-    calculation (seeded with a PBE calculation), and a bader and badelf analysis.
-    """
-
-    population_analysis_workflow = PopulationAnalysis__Warren__BaderBadelfHse
-    # We use pbesol as our default relaxation functional because it doesn't take
-    # much more time than pbe and is considered to be more accurate for solids
-    # (Phys. Rev. Lett. 102, 039902 (2009))
-    relaxation_workflow = Relaxation__Warren__Pbesol
```

### Comparing `warrenapp-0.1.1/src/warrenapp/workflows/population_analysis/base.py` & `warrenapp-0.1.2/src/warrenapp/workflows/population_analysis/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,25 +58,28 @@
     """
 
     required_files = ["CHGCAR_sum_empty", "CHGCAR_empty"]
     database_table = WarrenPopulationAnalysis
     command = "bader CHGCAR_empty -ref CHGCAR_sum_empty > bader.out"
 
     @staticmethod
-    def setup(directory, **kwargs):
+    def setup(directory, min_charge, analysis_type="bader", **kwargs):
         required_files = ["CHGCAR_sum_empty", "CHGCAR_empty", "POSCAR"]
         # Set the structure for this run
         structure = Structure.from_file(directory / "POSCAR")
         # Parse the BCF.dat file for possible electride sites and create CHGCAR_empty
         # and CHGCAR_sum_empty if found
         try:
             check_required_files(directory=directory, required_files=required_files)
         except:
             get_density_file_empty(
-                directory=directory, structure=structure, analysis_type="bader"
+                directory=directory,
+                structure=structure,
+                analysis_type=analysis_type,
+                min_charge=min_charge,
             )
 
 
 # Workflow for running a badelf analysis to create a BCF.dat file that will
 # be used to find electride sites before running further bader or badelf
 # analyses.
 class PopulationAnalysis__Warren__BadelfInit(S3Workflow):
@@ -102,25 +105,28 @@
 
     required_files = ["CHGCAR_empty", "ELFCAR_empty"]
     use_database = False
 
     command = "bader CHGCAR_empty -ref ELFCAR_empty -p all_atom > bader.out"
 
     @staticmethod
-    def setup(directory, analysis_type, **kwargs):
+    def setup(directory, min_charge, analysis_type="bader", **kwargs):
         required_files = ["CHGCAR_empty", "ELFCAR_empty"]
         # Set the structure for this run
         structure = Structure.from_file(directory / "POSCAR")
         # Parse the BCF.dat file for possible electride sites and create CHGCAR_empty
         # and CHGCAR_sum_empty if found
         try:
             check_required_files(directory=directory, required_files=required_files)
         except:
             get_density_file_empty(
-                directory=directory, structure=structure, analysis_type=analysis_type
+                directory=directory,
+                structure=structure,
+                analysis_type=analysis_type,
+                min_charge=min_charge,
             )
 
 
 # The base workflow that all workflows that just run bader analysis are built
 # from. For these a static_energy workflow needs to be created and set. The
 # workflow can take in an extra parameter, find_empties, which can be set to
 # true when searching for electrides is desired.
@@ -139,14 +145,15 @@
     def run_config(
         cls,
         structure: Structure,
         command: str = None,
         source: dict = None,
         find_empties: bool = True,
         directory: Path = None,
+        min_charge: float = 0.15,
         **kwargs,
     ):
         if find_empties:
             # Run static energy calculation
             prebader_result = cls.static_energy_prebadelf.run(
                 structure=structure,
                 command=command,
@@ -160,15 +167,17 @@
             ).result()
             # Combine AECCAR0 and AECCAR2
             PopulationAnalysis__Bader__CombineChgcars.run(
                 directory=prebader_result.directory,
             ).result()
             # Find electride sites, place empty atoms, and run bader
             PopulationAnalysis__Warren__BaderEmpty.run(
-                structure=structure, directory=prebader_result.directory
+                structure=structure,
+                directory=prebader_result.directory,
+                min_charge=min_charge,
             )
 
         else:
             prebader_result = cls.static_energy_prebader.run(
                 structure=structure,
                 command=command,
                 source=source,
@@ -206,14 +215,15 @@
     def run_config(
         cls,
         structure: Structure,
         command: str = None,
         source: dict = None,
         find_empties: bool = False,
         directory: Path = None,
+        min_charge: float = 0.15,
         **kwargs,
     ):
         if find_empties:
             # Run static_energy calculation
             prebadelf_result = cls.static_energy_prebadelf.run(
                 structure=structure,
                 command=command,
@@ -224,15 +234,17 @@
             PopulationAnalysis__Warren__BadelfInit.run(
                 structure=structure,
                 directory=prebadelf_result.directory,
             ).result()
             # Find electride sites, place empty atoms, and generate chgcar
             # like files for each atomic site
             PopulationAnalysis__Warren__GetAtomChgcar.run(
-                directory=prebadelf_result.directory, analysis_type="badelf"
+                directory=prebadelf_result.directory,
+                analysis_type="badelf",
+                min_charge=min_charge,
             )
             # Run Warren lab version of BadELF algorithm
             PopulationAnalysis__Warren__BadelfIonicRadii.run(
                 directory=prebadelf_result.directory,
             )
 
         else:
@@ -271,14 +283,15 @@
     def run_config(
         cls,
         structure: Structure,
         command: str = None,
         source: dict = None,
         find_empties: bool = False,
         directory: Path = None,
+        min_charge: float = 0.15,
         **kwargs,
     ):
         # Define files that will be copied into badelf and bader subdirectories
         badelf_files = ["ACF.dat", "simmate_population_summary.csv"]
         bader_files = [
             "ACF.dat",
             "BCF.dat",
@@ -301,15 +314,17 @@
             PopulationAnalysis__Warren__BadelfInit.run(
                 structure=structure,
                 directory=directory,
             ).result()
             # Find electride sites, place empty atoms, and get atom charges
             # in CHGCAR format
             PopulationAnalysis__Warren__GetAtomChgcar.run(
-                directory=directory, analysis_type="both"
+                directory=directory,
+                analysis_type="both",
+                min_charge=min_charge,
             ).result()
             # Run Warren lab BadELF algorithm
             PopulationAnalysis__Warren__BadelfIonicRadii.run(directory=directory)
             # Create directories for badelf and bader results so that they
             # don't get overwritten
             Path(directory / "badelf").mkdir()
             Path(directory / "bader").mkdir()
@@ -317,15 +332,17 @@
             for file in badelf_files:
                 shutil.copy(directory / file, directory / "badelf")
             # shutil.copy(
             #     directory / "simmate_population_summary.csv", directory / "badelf"
             # )
             # Run bader analysis
             PopulationAnalysis__Warren__BaderEmpty.run(
-                structure=structure, directory=directory
+                structure=structure,
+                directory=directory,
+                min_charge=min_charge,
             ).result()
             # Copy bader results into bader
             for file in bader_files:
                 shutil.copy(directory / file, directory / "bader")
         else:
             prebadelf_result = cls.static_energy_prebadelf.run(
                 structure=structure,
@@ -357,27 +374,7 @@
             # Run bader
             PopulationAnalysis__Warren__Bader.run(
                 directory=directory,
             ).result()
             # Copy bader files
             for file in bader_files:
                 shutil.copy(directory / file, directory / "bader")
-
-
-# We want to define the settings that will be used when updating static energy
-# workflows for prebader or prebadelf DFT calculations. We do that here so
-# that we don't need to do it in every inheriting class.
-prebader_incar_settings = dict(
-    NGXF__density_a=10,
-    NGYF__density_b=10,
-    NGZF__density_c=10,
-    LAECHG=True,  # write core charge density to AECCAR0 and valence to AECCAR2
-)
-prebadelf_incar_settings = dict(
-    NGX__density_a=10,  # Note that these set the FFT grid while the pre-Bader task sets the
-    NGY__density_b=10,  # fine FFT grid (e.g. useds NGX instead of NGXF)
-    NGZ__density_c=10,
-    LELF=True,  # Writes the ELFCAR
-    NPAR=1,  # Must be set if LELF is set
-    PREC="Single",  # ensures CHGCAR grid matches ELFCAR grid
-    LAECHG=True,  # write core charge density to AECCAR0 and valence to AECCAR2
-)
```

### Comparing `warrenapp-0.1.1/src/warrenapp/workflows/population_analysis/elf_hse.py` & `warrenapp-0.1.2/src/warrenapp/workflows/population_analysis/elf_hse.py`

 * *Files identical despite different names*

### Comparing `warrenapp-0.1.1/src/warrenapp/workflows/population_analysis/elf_pbe.py` & `warrenapp-0.1.2/src/warrenapp/workflows/population_analysis/elf_pbesol.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*-
 
 from simmate.database.workflow_results import StaticEnergy
 
-from warrenapp.workflows.static_energy.pbe import StaticEnergy__Warren__Pbe
+from warrenapp.workflows.static_energy.pbesol import StaticEnergy__Warren__Pbesol
 
 
-class PopulationAnalysis__Warren__ElfPbe(StaticEnergy__Warren__Pbe):
+class PopulationAnalysis__Warren__ElfPbesol(StaticEnergy__Warren__Pbesol):
     """
-    Runs a static energy calculation under Warren lab PBE settings
+    Runs a static energy calculation under Warren lab Pbesol settings
     and also writes the electron localization function (to ELFCAR).
     """
 
-    incar = StaticEnergy__Warren__Pbe.incar.copy()
+    incar = StaticEnergy__Warren__Pbesol.incar.copy()
     incar.update(
         LELF=True,  # writes ELFCAR
         NPAR=1,  # must be set if LELF is set to True
         # BUG: if NPAR conflicts with INCAR_parallel_settings config this
         # fails and tells the user to specify a setting
     )
```

### Comparing `warrenapp-0.1.1/src/warrenapp/workflows/population_analysis/relaxation_base.py` & `warrenapp-0.1.2/src/warrenapp/workflows/nested_dft/relaxation_static_base.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,35 +2,35 @@
 
 from pathlib import Path
 
 from simmate.engine import Workflow
 from simmate.toolkit import Structure
 
 
-class BaderBadelfRelaxationBase(Workflow):
+class RelaxationStaticBase(Workflow):
     """
-    Base class for running a PBE quality relaxation followed by a static energy
-    and bader or badelf analysis.
+    Base class for running a relaxation followed by a static energy
+    calculation.
 
     This should NOT be run on its own. It is meant to be inherited from in
     other workflows.
     """
 
-    # We don't need to save anything from this parent workflow
+    # We don't want to save anything from the parent workflow, only the
+    # sub workflows (relaxation and static energy) so we set use_database=False
     use_database = False
     relaxation_workflow = None  # This will be defined in inheriting workflows
-    population_analysis_workflow = None  # This will be defined in inheriting workflows
+    static_energy_workflow = None  # This will be defined in inheriting workflows
 
     @classmethod
     def run_config(
         cls,
         structure: Structure,
         command: str = None,
         source: dict = None,
-        find_empties: bool = True,
         directory: Path = None,
         **kwargs,
     ):
         # run a relaxation at PBE quality
         relaxation_directory = directory / "relaxation"
         relaxation_result = cls.relaxation_workflow.run(
             structure=structure,
@@ -39,21 +39,15 @@
             directory=relaxation_directory,
         ).result()
 
         static_energy_directory = directory / "static_energy"
         # run a static energy and bader/badelf analysis using the same structure
         # as above.
         # !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
-        # I noticed that when I run these calculations sharing the same directory
-        # it just reruns the first calculation twice. For now I'm just moving
-        # everything to a new directory, but this shouldn't be the case. I'll
-        # contact Jack about it. This is even more cluttered with the HSE calculations
-        # which are seeded with a PBE calculation and require the same splitting
-        # of folders.
-        bader_result = cls.population_analysis_workflow.run(
+        # We need to make a new directory because only one vasp workflow can
+        # be run in each directory.
+        static_energy_result = cls.static_energy_workflow.run(
             structure=relaxation_result,
-            # copy_previous_directory = True,
             command=command,
             source=source,
-            find_empties=find_empties,
             directory=static_energy_directory,
-        ).result()
+        )
```

### Comparing `warrenapp-0.1.1/src/warrenapp/workflows/population_analysis/warren_badelf_v3_7.py` & `warrenapp-0.1.2/src/warrenapp/workflows/population_analysis/warren_badelf_v3_7.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,19 @@
         # that are within all bounding planes of a site belong to that site.
 
         # I go across the elf grid voxel-by-voxel.
         # For each voxel, I get its real space position.
         # I then test if it is within the planes in each site.
         # Only when it matches all the planes do I record it as belonging to a site.
 
+        # !!!!!!!!
+        # In this iteration, I'm going to try and treat voxels that may intersect
+        # 1 or more planes more rigorously
+        #!!!!!!!!!
+
         # The output, then, is a list of voxels (x,y,z position) that belong
         # to each site.
 
         # Then, this list of voxels is applied to the total charge density to
         # add up all the incremental charge.
 
         # create dictionaries for each site's coordinates, charge, min-distance
@@ -141,14 +146,18 @@
         # We need to get the charge on each electride site and get the coordinates that
         # belong to the electride. We first get a dataframe that indexes all of the
         # coordinates. We'll remove the electride coordinates from this later.
 
         a, b, c = lattice["grid_size"]
 
         # Create lists that contain the coordinates of each voxel and their charges
+
+        #!!!!
+        # Why did I do this instead of keeping everything in an array so that
+        # indexing is easier?
         voxel_coords = [idx for idx in itertools.product(range(a), range(b), range(c))]
         voxel_charges = [float(chg[idx[0], idx[1], idx[2]]) for idx in voxel_coords]
 
         # Create a dataframe that has each coordinate index and the charge as columns
         # Later we'll remove voxels that belong to electrides from this dataframe
         all_charge_coords = pd.DataFrame(voxel_coords, columns=["x", "y", "z"]).add(1)
         all_charge_coords["chg"] = voxel_charges
@@ -192,38 +201,37 @@
                 permutations_sorted.append(item)
         permutations_sorted.insert(0, permutations_sorted.pop(7))
 
         # open dask client. Find a available number of cores/threads and use
         # 90% of them. Only 1 thread per worker. We also suppress output to
         # the terminal and instead send to a dask.out file
         cpu_count = int(0.9 * len(psutil.Process().cpu_affinity()))
-        with redirect_stderr(None):
-            with LocalCluster(
-                n_workers=cpu_count,
-                threads_per_worker=1,
-                memory_limit="auto",
-                processes=True,
-            ) as cluster, Client(cluster) as client:
-                # put list of indices in dask dataframe. Partition with the same
-                # number of partitions as workers
-                ddf = dd.from_pandas(
-                    all_charge_coords,
-                    npartitions=cpu_count,
-                )
-
-                # site search for all voxel positions.
-                ddf["site"] = ddf.map_partitions(
-                    get_voxels_site_dask,
-                    results=results,
-                    permutations=permutations,
-                    lattice=lattice,
-                    electride_sites=electride_sites,
-                )
-                # run site search and save as pandas dataframe
-                pdf = ddf.compute()
+        with LocalCluster(
+            n_workers=cpu_count,
+            threads_per_worker=1,
+            memory_limit="auto",
+            processes=True,
+        ) as cluster, Client(cluster) as client:
+            # put list of indices in dask dataframe. Partition with the same
+            # number of partitions as workers
+            ddf = dd.from_pandas(
+                all_charge_coords,
+                npartitions=cpu_count,
+            )
+
+            # site search for all voxel positions.
+            ddf["site"] = ddf.map_partitions(
+                get_voxels_site_dask,
+                results=results,
+                permutations=permutations,
+                lattice=lattice,
+                electride_sites=electride_sites,
+            )
+            # run site search and save as pandas dataframe
+            pdf = ddf.compute()
 
         # Group the results by site. Sum the charges and count the total number
         # of voxels for each site. Apply charges and volumes to dictionaries.
         pdf_grouped = pdf.groupby(by="site")
         pdf_grouped_charge = pdf_grouped["chg"].sum()
         pdf_grouped_voxels = pdf_grouped["site"].size()
         for site in results_charge:
```

### Comparing `warrenapp-0.1.1/src/warrenapp/workflows/relaxation/hsesol.py` & `warrenapp-0.1.2/src/warrenapp/workflows/relaxation/hsesol.py`

 * *Files identical despite different names*

### Comparing `warrenapp-0.1.1/src/warrenapp/workflows/relaxation/pbe.py` & `warrenapp-0.1.2/src/warrenapp/workflows/relaxation/pbe.py`

 * *Files identical despite different names*

### Comparing `warrenapp-0.1.1/src/warrenapp/workflows/relaxation/scan.py` & `warrenapp-0.1.2/src/warrenapp/workflows/relaxation/scan.py`

 * *Files identical despite different names*

### Comparing `warrenapp-0.1.1/src/warrenapp/workflows/static_energy/pbe.py` & `warrenapp-0.1.2/src/warrenapp/workflows/static_energy/pbe.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 from warrenapp.workflows.relaxation.pbe import Relaxation__Warren__Pbe
 
-static_settings = dict(
+pbe_static_settings = dict(
     IBRION=-1,  # (optional) locks everything between ionic steps
     NSW=0,  # this is the main static energy setting
     #            LAECHG=True, # currently only set in population analysis
     LCHARG=True,
     LORBIT=11,
     LVHAR=True,
     LWAVE=True,
@@ -19,8 +19,8 @@
 class StaticEnergy__Warren__Pbe(Relaxation__Warren__Pbe):
     """
     Performs a static energy calculation based on the settings for Warren Lab
     PBE.
     """
 
     incar = Relaxation__Warren__Pbe.incar.copy()
-    incar.update(static_settings)
+    incar.update(pbe_static_settings)
```

### Comparing `warrenapp-0.1.1/src/warrenapp/workflows/static_energy/pbesol.py` & `warrenapp-0.1.2/src/warrenapp/workflows/static_energy/pbesol.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 
 from warrenapp.workflows.relaxation.pbesol import Relaxation__Warren__Pbesol
-from warrenapp.workflows.static_energy.pbe import static_settings
+from warrenapp.workflows.static_energy.pbe import pbe_static_settings
 
 
 class StaticEnergy__Warren__Pbesol(Relaxation__Warren__Pbesol):
     """
     Performs a static energy calculation based on the settings for Warren Lab
     PBEsol functional relaxation. This functional is generally considered to
     be more accurate for solids.
     (Phys. Rev. Lett. 102, 039902 (2009))
     """
 
     incar = Relaxation__Warren__Pbesol.incar.copy()
-    incar.update(static_settings)
+    incar.update(pbe_static_settings)
```

### Comparing `warrenapp-0.1.1/src/warrenapp/workflows/static_energy/seeded_hse.py` & `warrenapp-0.1.2/src/warrenapp/workflows/static_energy/seeded_hse.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,14 @@
         cls,
         structure: Structure,
         command: str = None,
         source: dict = None,
         directory: Path = None,
         **kwargs,
     ):
-
         # run the initial PBE calculation and save its results as a variable
         initial_directory = directory / "pbe_seed"
         initial_result = cls.initial_calculation.run(
             structure=structure,
             command=command,
             source=source,
             directory=initial_directory,
```

### Comparing `warrenapp-0.1.1/src/warrenapp.egg-info/PKG-INFO` & `warrenapp-0.1.2/src/warrenapp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warrenapp
-Version: 0.1.1
+Version: 0.1.2
 Summary: The Warrenapp is an extension of the Simulated Materials Ecosystem (Simmate), a package designed to ease computational materials research. The WarrenApp adds several custom workflows and settings.
 Author-email: Sam Weaver <sweav@unc.edu>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Sam M. Weaver
         All rights reserved.
```

### Comparing `warrenapp-0.1.1/src/warrenapp.egg-info/SOURCES.txt` & `warrenapp-0.1.2/src/warrenapp.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -10,27 +10,29 @@
 src/warrenapp.egg-info/dependency_links.txt
 src/warrenapp.egg-info/requires.txt
 src/warrenapp.egg-info/top_level.txt
 src/warrenapp/badelf_tools/acf.py
 src/warrenapp/badelf_tools/badelf_algorithm_functions.py
 src/warrenapp/badelf_tools/utilities.py
 src/warrenapp/workflows/__init__.py
+src/warrenapp/workflows/nested_dft/__init__.py
+src/warrenapp/workflows/nested_dft/prepop_relaxation_static_hse.py
+src/warrenapp/workflows/nested_dft/prepop_relaxation_static_pbesol.py
+src/warrenapp/workflows/nested_dft/relaxation_static_base.py
 src/warrenapp/workflows/population_analysis/__init__.py
 src/warrenapp/workflows/population_analysis/badelf_hse.py
-src/warrenapp/workflows/population_analysis/badelf_pbe.py
+src/warrenapp/workflows/population_analysis/badelf_pbesol.py
 src/warrenapp/workflows/population_analysis/bader_badelf_hse.py
-src/warrenapp/workflows/population_analysis/bader_badelf_pbe.py
-src/warrenapp/workflows/population_analysis/bader_badelf_relaxation_hse.py
-src/warrenapp/workflows/population_analysis/bader_badelf_relaxation_pbe.py
+src/warrenapp/workflows/population_analysis/bader_badelf_pbesol.py
 src/warrenapp/workflows/population_analysis/bader_hse.py
-src/warrenapp/workflows/population_analysis/bader_pbe.py
+src/warrenapp/workflows/population_analysis/bader_pbesol.py
 src/warrenapp/workflows/population_analysis/base.py
 src/warrenapp/workflows/population_analysis/elf_hse.py
-src/warrenapp/workflows/population_analysis/elf_pbe.py
-src/warrenapp/workflows/population_analysis/relaxation_base.py
+src/warrenapp/workflows/population_analysis/elf_pbesol.py
+src/warrenapp/workflows/population_analysis/prebader_badelf_dft.py
 src/warrenapp/workflows/population_analysis/warren_badelf_v3_7.py
 src/warrenapp/workflows/relaxation/__init__.py
 src/warrenapp/workflows/relaxation/hse.py
 src/warrenapp/workflows/relaxation/hsesol.py
 src/warrenapp/workflows/relaxation/pbe.py
 src/warrenapp/workflows/relaxation/pbe_metal.py
 src/warrenapp/workflows/relaxation/pbesol.py
```

