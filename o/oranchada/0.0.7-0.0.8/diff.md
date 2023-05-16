# Comparing `tmp/oranchada-0.0.7.tar.gz` & `tmp/oranchada-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oranchada-0.0.7.tar", last modified: Thu May  4 12:48:05 2023, max compression
+gzip compressed data, was "oranchada-0.0.8.tar", last modified: Tue May 16 00:02:25 2023, max compression
```

## Comparing `oranchada-0.0.7.tar` & `oranchada-0.0.8.tar`

### file list

```diff
@@ -1,67 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:48:05.424214 oranchada-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-04 12:47:53.000000 oranchada-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-04 12:47:53.000000 oranchada-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-04 12:48:05.420214 oranchada-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-04 12:47:53.000000 oranchada-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-04 12:47:53.000000 oranchada-0.0.7/README.pypi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:48:05.408214 oranchada-0.0.7/oranchada.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-04 12:48:05.000000 oranchada-0.0.7/oranchada.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-04 12:48:05.000000 oranchada-0.0.7/oranchada.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 12:48:05.000000 oranchada-0.0.7/oranchada.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-04 12:48:05.000000 oranchada-0.0.7/oranchada.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-04 12:48:05.000000 oranchada-0.0.7/oranchada.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 12:48:05.000000 oranchada-0.0.7/oranchada.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-04 12:48:05.000000 oranchada-0.0.7/oranchada.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-04 12:48:05.000000 oranchada-0.0.7/oranchada.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:48:05.408214 oranchada-0.0.7/orangecontrib/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:48:05.408214 oranchada-0.0.7/orangecontrib/oranchada/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:48:05.412214 oranchada-0.0.7/orangecontrib/oranchada/base_widget/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/base_widget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/base_widget/arithmetic_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/base_widget/base_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/base_widget/creator_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/base_widget/filter_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/base_widget/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:48:05.412214 oranchada-0.0.7/orangecontrib/oranchada/processings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/processings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/processings/add_baseline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/processings/add_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/processings/gen_spe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:48:05.412214 oranchada-0.0.7/orangecontrib/oranchada/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/tests/process_spectra_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:48:05.416214 oranchada-0.0.7/orangecontrib/oranchada/widgets_easy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_easy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_easy/gen_noisy_spe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:48:05.416214 oranchada-0.0.7/orangecontrib/oranchada/widgets_easy/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_easy/icons/spectra.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:48:05.420214 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/add_baseline.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/add_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/arithmetics_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/arithmetics_subtract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/find_peaks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/fit_peaks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/gen_spe.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/hht_sharpening.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:48:05.420214 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/icons/spectra.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/load_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/load_file_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/load_test_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/merger.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/moving_minimum.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/process_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/raman_shift_to_wavelength.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/remove_spikes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/resample_NUDFT.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/set_xaxis.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/wavelength_to_raman_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/xaxis_fine_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 12:48:05.424214 oranchada-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-05-04 12:47:53.000000 oranchada-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:25.339974 oranchada-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-16 00:02:14.000000 oranchada-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-16 00:02:14.000000 oranchada-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-16 00:02:25.339974 oranchada-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-05-16 00:02:14.000000 oranchada-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-16 00:02:14.000000 oranchada-0.0.8/README.pypi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:25.331974 oranchada-0.0.8/oranchada.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-16 00:02:25.000000 oranchada-0.0.8/oranchada.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-05-16 00:02:25.000000 oranchada-0.0.8/oranchada.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 00:02:25.000000 oranchada-0.0.8/oranchada.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-16 00:02:25.000000 oranchada-0.0.8/oranchada.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-16 00:02:25.000000 oranchada-0.0.8/oranchada.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 00:02:25.000000 oranchada-0.0.8/oranchada.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-16 00:02:25.000000 oranchada-0.0.8/oranchada.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-16 00:02:25.000000 oranchada-0.0.8/oranchada.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:25.331974 oranchada-0.0.8/orangecontrib/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:25.331974 oranchada-0.0.8/orangecontrib/oranchada/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:25.331974 oranchada-0.0.8/orangecontrib/oranchada/base_widget/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/base_widget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/base_widget/arithmetic_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/base_widget/base_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/base_widget/creator_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/base_widget/filter_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/base_widget/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:25.331974 oranchada-0.0.8/orangecontrib/oranchada/processings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/processings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/processings/add_baseline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/processings/add_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/processings/gen_spe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:25.335974 oranchada-0.0.8/orangecontrib/oranchada/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/tests/process_spectra_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:25.335974 oranchada-0.0.8/orangecontrib/oranchada/widgets_easy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_easy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_easy/gen_noisy_spe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:25.335974 oranchada-0.0.8/orangecontrib/oranchada/widgets_easy/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_easy/icons/spectra.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:25.339974 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/add_baseline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/add_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/arithmetics_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/arithmetics_subtract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/find_peaks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/fit_peaks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/gen_spe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/hdr_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/hht_sharpening.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:25.339974 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/icons/spectra.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/load_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/load_file_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/load_test_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/moving_minimum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/process_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/raman_shift_to_wavelength.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/remove_spikes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/resample_NUDFT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/set_xaxis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/wavelength_to_raman_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7609 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/xaxis_fine_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 00:02:25.339974 oranchada-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-05-16 00:02:14.000000 oranchada-0.0.8/setup.py
```

### Comparing `oranchada-0.0.7/LICENSE` & `oranchada-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.7/PKG-INFO` & `oranchada-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oranchada
-Version: 0.0.7
+Version: 0.0.8
 Summary: Orange add-on for Raman spectroscopy
 Home-page: https://github.com/h2020charisma/oranchada
 Author: IDEAconsult Ltd.
 Author-email: dev-charisma@ideaconsult.net
 License: MIT
 Keywords: Raman,oranchada,orange3 add-on,spectroscopy
 Classifier: Development Status :: 4 - Beta
```

### Comparing `oranchada-0.0.7/oranchada.egg-info/PKG-INFO` & `oranchada-0.0.8/oranchada.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oranchada
-Version: 0.0.7
+Version: 0.0.8
 Summary: Orange add-on for Raman spectroscopy
 Home-page: https://github.com/h2020charisma/oranchada
 Author: IDEAconsult Ltd.
 Author-email: dev-charisma@ideaconsult.net
 License: MIT
 Keywords: Raman,oranchada,orange3 add-on,spectroscopy
 Classifier: Development Status :: 4 - Beta
```

### Comparing `oranchada-0.0.7/oranchada.egg-info/SOURCES.txt` & `oranchada-0.0.8/oranchada.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 orangecontrib/oranchada/widgets_pro/add_baseline.py
 orangecontrib/oranchada/widgets_pro/add_noise.py
 orangecontrib/oranchada/widgets_pro/arithmetics_add.py
 orangecontrib/oranchada/widgets_pro/arithmetics_subtract.py
 orangecontrib/oranchada/widgets_pro/find_peaks.py
 orangecontrib/oranchada/widgets_pro/fit_peaks.py
 orangecontrib/oranchada/widgets_pro/gen_spe.py
+orangecontrib/oranchada/widgets_pro/hdr_merge.py
 orangecontrib/oranchada/widgets_pro/hht_sharpening.py
 orangecontrib/oranchada/widgets_pro/load_file.py
 orangecontrib/oranchada/widgets_pro/load_file_names.py
 orangecontrib/oranchada/widgets_pro/load_test_spectra.py
 orangecontrib/oranchada/widgets_pro/merger.py
 orangecontrib/oranchada/widgets_pro/moving_minimum.py
 orangecontrib/oranchada/widgets_pro/normalize.py
```

### Comparing `oranchada-0.0.7/orangecontrib/oranchada/base_widget/base_widget.py` & `oranchada-0.0.8/orangecontrib/oranchada/base_widget/base_widget.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.7/orangecontrib/oranchada/base_widget/filter_widget.py` & `oranchada-0.0.8/orangecontrib/oranchada/base_widget/filter_widget.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.7/orangecontrib/oranchada/processings/add_baseline.py` & `oranchada-0.0.8/orangecontrib/oranchada/processings/add_baseline.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.7/orangecontrib/oranchada/processings/add_noise.py` & `oranchada-0.0.8/orangecontrib/oranchada/processings/add_noise.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.7/orangecontrib/oranchada/processings/gen_spe.py` & `oranchada-0.0.8/orangecontrib/oranchada/processings/gen_spe.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.7/orangecontrib/oranchada/tests/process_spectra_test.py` & `oranchada-0.0.8/orangecontrib/oranchada/tests/process_spectra_test.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.7/orangecontrib/oranchada/widgets_easy/gen_noisy_spe.py` & `oranchada-0.0.8/orangecontrib/oranchada/widgets_easy/gen_noisy_spe.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.7/orangecontrib/oranchada/widgets_easy/icons/spectra.svg` & `oranchada-0.0.8/orangecontrib/oranchada/widgets_easy/icons/spectra.svg`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/add_baseline.py` & `oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/add_baseline.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/add_noise.py` & `oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/add_noise.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/arithmetics_add.py` & `oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/arithmetics_add.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/arithmetics_subtract.py` & `oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/arithmetics_subtract.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/find_peaks.py` & `oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/find_peaks.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/fit_peaks.py` & `oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/fit_peaks.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/gen_spe.py` & `oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/gen_spe.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/hht_sharpening.py` & `oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/hht_sharpening.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/icons/spectra.svg` & `oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/icons/spectra.svg`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/load_file.py` & `oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/load_file.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/load_file_names.py` & `oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/load_file_names.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/load_test_spectra.py` & `oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/load_test_spectra.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/merger.py` & `oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/merger.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/moving_minimum.py` & `oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/moving_minimum.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/normalize.py` & `oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/normalize.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/process_spectra.py` & `oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/process_spectra.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/raman_shift_to_wavelength.py` & `oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/raman_shift_to_wavelength.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/remove_spikes.py` & `oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/remove_spikes.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/resample_NUDFT.py` & `oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/resample_NUDFT.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/select.py` & `oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/select.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/set_xaxis.py` & `oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/set_xaxis.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/wavelength_to_raman_shift.py` & `oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/wavelength_to_raman_shift.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/xaxis_fine_calibration.py` & `oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/xaxis_fine_calibration.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,24 +14,26 @@
 
     predefined_deltas = Setting('Ne WL D3.3')
     deltas = Setting('')
     poly_order = Setting('poly3')
     should_fit = Setting(False)
     prominence = Setting(3.)
     wlen = Setting(200)
+    min_peak_width = Setting(2)
     should_auto_proc = Setting(False)
     n_iters = Setting(1)
 
     def __init__(self):
         super().__init__()
         box = gui.widgetBox(self.controlArea, self.name)
 
         gui.doubleSpin(box, self, 'prominence', 0, 50000, decimals=2, step=1, callback=self.auto_process,
                        label='Prominence [×σ]')
         gui.spin(box, self, 'wlen', 0, 50000, step=1, callback=self.auto_process, label='wlen')
+        gui.spin(box, self, 'min_peak_width', 1, 5000, callback=self.auto_process, label='Min peak width')
 
         gui.checkBox(box, self, "should_fit", "Should fit", callback=self.auto_process)
 
         gui.comboBox(box, self, 'poly_order', sendSelectedValue=True,
                      items=['poly0', 'poly1', 'poly2', 'poly3', 'poly4', 'RBF thin-plate-spline'],
                      callback=self.auto_process
                      )
@@ -86,19 +88,26 @@
         self.out_spe = list()
         if len(self.in_spe) > 1:
             raise ValueError(f'Expects a single spectrum input. {len(self.in_spe)} found')
         for spe in self.in_spe:
             for iter in range(self.n_iters):
                 if self.poly_order == 'RBF thin-plate-spline':
                     spe = spe.xcal_fine_RBF(ref=self.deltas_dict, should_fit=self.should_fit,
-                                            find_peaks_kw=dict(prominence=spe.y_noise*self.prominence, wlen=self.wlen)
+                                            find_peaks_kw=dict(prominence=spe.y_noise*self.prominence,
+                                                               wlen=self.wlen,
+                                                               width=self.min_peak_width,
+                                                               )
                                             )
                 else:
                     spe = spe.xcal_fine(ref=self.deltas_dict, poly_order=poly_order_num, should_fit=self.should_fit,
-                                        find_peaks_kw=dict(prominence=spe.y_noise*self.prominence, wlen=self.wlen))
+                                        find_peaks_kw=dict(prominence=spe.y_noise*self.prominence,
+                                                           wlen=self.wlen,
+                                                           width=self.min_peak_width,
+                                                           )
+                                        )
             self.out_spe.append(spe)
         self.send_outputs()
 
     def custom_plot(self, ax):
         if not self.in_spe:
             return
         self.in_spe[0].plot(ax=self.axes[0])
```

### Comparing `oranchada-0.0.7/setup.py` & `oranchada-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from os import path, walk
 
 from setuptools import find_packages, setup
 
 NAME = 'oranchada'
 
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 
 DESCRIPTION = 'Orange add-on for Raman spectroscopy'
 README_FILE = path.join(path.dirname(__file__), 'README.pypi')
 LONG_DESCRIPTION = open(README_FILE, 'r', encoding='utf-8').read()
 LONG_DESCRIPTION_CONTENT_TYPE = 'text/markdown'
 URL = 'https://github.com/h2020charisma/oranchada'
 AUTHOR = 'IDEAconsult Ltd.'
@@ -38,15 +38,15 @@
 
 INSTALL_REQUIRES = [
     'Orange3>=3.31.0',
     'numpy>=1.18.0',
     'orange-canvas-core>=0.1.24',
     'orange-widget-base>=4.16.1',
     'pip>=9.0',  # same as for Orange 3.28
-    'ramanchada2~=0.0.5',
+    'ramanchada2~=0.0.6',
     'setuptools>=36.3',  # same as for Orange 3.28
     # 'AnyQt>=0.0.6',
     # 'bottleneck',
     # 'colorcet',
     # 'extranormal3 >=0.0.3',
     # 'h5py',
     # 'lmfit>=1.0.2',
```

