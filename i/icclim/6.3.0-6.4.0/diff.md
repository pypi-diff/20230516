# Comparing `tmp/icclim-6.3.0.tar.gz` & `tmp/icclim-6.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icclim-6.3.0.tar", last modified: Tue Apr 25 15:25:06 2023, max compression
+gzip compressed data, was "icclim-6.4.0.tar", last modified: Tue May 16 05:39:20 2023, max compression
```

## Comparing `icclim-6.3.0.tar` & `icclim-6.4.0.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        0 2023-04-25 15:25:06.092923 icclim-6.3.0/
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)    11358 2022-12-20 08:56:54.000000 icclim-6.3.0/LICENSE
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      222 2022-12-20 08:56:54.000000 icclim-6.3.0/MANIFEST.in
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     4534 2023-04-25 15:25:06.094137 icclim-6.3.0/PKG-INFO
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     3831 2022-12-20 08:56:54.000000 icclim-6.3.0/README.rst
-drwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        0 2023-04-25 15:25:04.146831 icclim-6.3.0/doc/
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      639 2022-12-20 08:56:54.000000 icclim-6.3.0/doc/Makefile
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      765 2022-12-20 08:56:54.000000 icclim-6.3.0/doc/make.bat
-drwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        0 2023-04-25 15:25:04.193623 icclim-6.3.0/doc/source/
-drwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        0 2023-04-25 15:25:04.198166 icclim-6.3.0/doc/source/_static/
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)    42702 2022-12-20 08:56:54.000000 icclim-6.3.0/doc/source/_static/chunks.png
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     3186 2022-12-20 08:56:54.000000 icclim-6.3.0/doc/source/conf.py
-drwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        0 2023-04-25 15:25:04.265579 icclim-6.3.0/doc/source/dev/
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      890 2022-12-20 08:56:54.000000 icclim-6.3.0/doc/source/dev/ci.rst
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)       47 2022-12-20 08:56:54.000000 icclim-6.3.0/doc/source/dev/contributing.rst
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      207 2022-12-20 08:56:54.000000 icclim-6.3.0/doc/source/dev/index.rst
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     2270 2022-12-20 08:56:54.000000 icclim-6.3.0/doc/source/dev/release_process.rst
-drwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        0 2023-04-25 15:25:04.363171 icclim-6.3.0/doc/source/explanation/
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      485 2022-12-20 08:56:54.000000 icclim-6.3.0/doc/source/explanation/4.2.x_installation.rst
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)    18547 2022-12-20 08:56:54.000000 icclim-6.3.0/doc/source/explanation/climate_indices.rst
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      251 2022-12-20 08:56:54.000000 icclim-6.3.0/doc/source/explanation/index.rst
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     3616 2022-12-20 08:56:54.000000 icclim-6.3.0/doc/source/explanation/xclim_and_icclim.rst
-drwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        0 2023-04-25 15:25:04.558905 icclim-6.3.0/doc/source/how_to/
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)    29218 2022-12-20 08:56:54.000000 icclim-6.3.0/doc/source/how_to/dask.rst
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      589 2022-12-20 08:56:54.000000 icclim-6.3.0/doc/source/how_to/index.rst
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     1240 2022-12-20 08:56:54.000000 icclim-6.3.0/doc/source/how_to/notebooks.rst
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     7382 2022-12-20 08:56:54.000000 icclim-6.3.0/doc/source/how_to/ocgis.rst
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)    15192 2022-12-20 08:56:54.000000 icclim-6.3.0/doc/source/how_to/recipes_custom.rst
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     6935 2022-12-20 08:56:54.000000 icclim-6.3.0/doc/source/how_to/recipes_ecad.rst
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     8994 2022-12-20 08:56:54.000000 icclim-6.3.0/doc/source/how_to/recipes_generic.rst
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     2102 2022-12-20 08:56:54.000000 icclim-6.3.0/doc/source/index.rst
-drwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        0 2023-04-25 15:25:04.828601 icclim-6.3.0/doc/source/references/
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)    10456 2022-12-20 08:56:54.000000 icclim-6.3.0/doc/source/references/custom_indices.rst
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     1615 2022-12-20 08:56:54.000000 icclim-6.3.0/doc/source/references/ecad_functions_api.rst
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)       85 2022-12-20 08:56:54.000000 icclim-6.3.0/doc/source/references/frequency.rst
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     1619 2022-12-20 08:56:54.000000 icclim-6.3.0/doc/source/references/generic_functions_api.rst
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)    18267 2022-12-20 08:56:54.000000 icclim-6.3.0/doc/source/references/icclim_index_api.rst
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      530 2022-12-20 08:56:54.000000 icclim-6.3.0/doc/source/references/index.rst
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     5598 2022-12-20 08:56:54.000000 icclim-6.3.0/doc/source/references/output_metadata.rst
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)    17581 2023-04-25 15:24:39.000000 icclim-6.3.0/doc/source/references/release_notes.rst
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      299 2022-12-20 08:56:54.000000 icclim-6.3.0/doc/source/references/threshold.rst
-drwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        0 2023-04-25 15:25:04.881574 icclim-6.3.0/doc/source/tutorials/
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      237 2022-12-20 08:56:54.000000 icclim-6.3.0/doc/source/tutorials/index.rst
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     1229 2022-12-20 08:56:54.000000 icclim-6.3.0/doc/source/tutorials/installation.rst
-drwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        0 2023-04-25 15:25:05.067152 icclim-6.3.0/icclim/
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      520 2022-12-20 08:56:54.000000 icclim-6.3.0/icclim/__init__.py
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)   334504 2023-04-11 13:19:13.000000 icclim-6.3.0/icclim/_generated_api.py
-drwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        0 2023-04-25 15:25:05.158983 icclim-6.3.0/icclim/ecad/
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        0 2022-12-20 08:56:54.000000 icclim-6.3.0/icclim/ecad/__init__.py
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)    28468 2022-12-20 08:56:54.000000 icclim-6.3.0/icclim/ecad/ecad_indices.py
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     4292 2022-12-20 08:56:54.000000 icclim-6.3.0/icclim/ecad/xclim_binding.py
-drwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        0 2023-04-25 15:25:05.339419 icclim-6.3.0/icclim/generic_indices/
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        0 2022-12-20 08:56:54.000000 icclim-6.3.0/icclim/generic_indices/__init__.py
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)    44631 2023-04-25 15:09:39.000000 icclim-6.3.0/icclim/generic_indices/generic_indicators.py
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     9508 2022-12-20 08:56:54.000000 icclim-6.3.0/icclim/generic_indices/generic_templates.py
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     7845 2022-12-20 08:56:54.000000 icclim-6.3.0/icclim/generic_indices/standard_variable.py
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)    40401 2023-04-25 15:09:39.000000 icclim-6.3.0/icclim/generic_indices/threshold.py
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     5085 2022-12-20 08:56:54.000000 icclim-6.3.0/icclim/generic_indices/threshold_templates.py
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      478 2022-12-20 08:56:54.000000 icclim-6.3.0/icclim/icclim_exceptions.py
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     5957 2022-12-20 08:56:54.000000 icclim-6.3.0/icclim/icclim_logger.py
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      876 2022-12-20 08:56:54.000000 icclim-6.3.0/icclim/icclim_types.py
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)    30820 2022-12-20 08:56:54.000000 icclim-6.3.0/icclim/main.py
-drwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        0 2023-04-25 15:25:05.608137 icclim-6.3.0/icclim/models/
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      105 2022-12-20 08:56:54.000000 icclim-6.3.0/icclim/models/__init__.py
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     2627 2022-12-20 08:56:54.000000 icclim-6.3.0/icclim/models/cf_calendar.py
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)    11282 2023-04-11 13:19:13.000000 icclim-6.3.0/icclim/models/climate_variable.py
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     3289 2023-04-11 13:19:13.000000 icclim-6.3.0/icclim/models/constants.py
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)    17259 2022-12-20 08:56:54.000000 icclim-6.3.0/icclim/models/frequency.py
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      214 2022-12-20 08:56:54.000000 icclim-6.3.0/icclim/models/global_metadata.py
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     1925 2022-12-20 08:56:54.000000 icclim-6.3.0/icclim/models/index_config.py
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     1630 2022-12-20 08:56:54.000000 icclim-6.3.0/icclim/models/index_group.py
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      997 2022-12-20 08:56:54.000000 icclim-6.3.0/icclim/models/logical_link.py
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      546 2022-12-20 08:56:54.000000 icclim-6.3.0/icclim/models/netcdf_version.py
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     2480 2022-12-20 08:56:54.000000 icclim-6.3.0/icclim/models/operator.py
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      446 2022-12-20 08:56:54.000000 icclim-6.3.0/icclim/models/quantile_interpolation.py
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     1810 2022-12-20 08:56:54.000000 icclim-6.3.0/icclim/models/registry.py
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     2588 2022-12-20 08:56:54.000000 icclim-6.3.0/icclim/models/standard_index.py
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      863 2022-12-20 08:56:54.000000 icclim-6.3.0/icclim/models/user_index_dict.py
-drwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        0 2023-04-25 15:25:05.677657 icclim-6.3.0/icclim/pre_processing/
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        0 2022-12-20 08:56:54.000000 icclim-6.3.0/icclim/pre_processing/__init__.py
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      764 2022-12-20 08:56:54.000000 icclim-6.3.0/icclim/pre_processing/in_file_dictionary.py
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)    14655 2023-04-11 12:52:34.000000 icclim-6.3.0/icclim/pre_processing/input_parsing.py
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     8306 2022-12-20 08:56:54.000000 icclim-6.3.0/icclim/pre_processing/rechunk.py
-drwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        0 2023-04-25 15:25:06.060233 icclim-6.3.0/icclim/tests/
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        0 2022-12-20 08:56:54.000000 icclim-6.3.0/icclim/tests/__init__.py
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     2524 2022-12-20 08:56:54.000000 icclim-6.3.0/icclim/tests/test_cf_calendar.py
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      835 2022-12-20 08:56:54.000000 icclim-6.3.0/icclim/tests/test_ecad_indices.py
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     5753 2022-12-20 08:56:54.000000 icclim-6.3.0/icclim/tests/test_frequency.py
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)    13360 2022-12-20 08:56:54.000000 icclim-6.3.0/icclim/tests/test_generated_api.py
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      932 2022-12-20 08:56:54.000000 icclim-6.3.0/icclim/tests/test_index_group.py
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     6654 2023-02-15 09:31:22.000000 icclim-6.3.0/icclim/tests/test_input_parsing.py
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)    33580 2023-04-25 15:09:39.000000 icclim-6.3.0/icclim/tests/test_main.py
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     2845 2022-12-20 08:56:54.000000 icclim-6.3.0/icclim/tests/test_rechunk.py
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)    11082 2023-02-15 09:31:22.000000 icclim-6.3.0/icclim/tests/test_threshold.py
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)    10327 2022-12-20 08:56:54.000000 icclim-6.3.0/icclim/tests/test_user_index.py
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     1103 2023-04-25 15:09:39.000000 icclim-6.3.0/icclim/tests/testing_utils.py
-drwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        0 2023-04-25 15:25:06.080883 icclim-6.3.0/icclim/user_indices/
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        0 2022-12-20 08:56:54.000000 icclim-6.3.0/icclim/user_indices/__init__.py
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      973 2022-12-20 08:56:54.000000 icclim-6.3.0/icclim/user_indices/calc_operation.py
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     1730 2023-01-30 13:21:59.000000 icclim-6.3.0/icclim/utils.py
-drwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        0 2023-04-25 15:25:05.110473 icclim-6.3.0/icclim.egg-info/
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     4534 2023-04-25 15:25:02.000000 icclim-6.3.0/icclim.egg-info/PKG-INFO
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     2760 2023-04-25 15:25:03.000000 icclim-6.3.0/icclim.egg-info/SOURCES.txt
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        1 2023-04-25 15:25:02.000000 icclim-6.3.0/icclim.egg-info/dependency_links.txt
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      167 2023-04-25 15:25:02.000000 icclim-6.3.0/icclim.egg-info/requires.txt
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        7 2023-04-25 15:25:02.000000 icclim-6.3.0/icclim.egg-info/top_level.txt
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      559 2023-04-25 15:25:06.109383 icclim-6.3.0/setup.cfg
--rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     1249 2023-04-25 15:09:39.000000 icclim-6.3.0/setup.py
+drwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        0 2023-05-16 05:39:20.647176 icclim-6.4.0/
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)    11358 2022-12-20 08:56:54.000000 icclim-6.4.0/LICENSE
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      222 2022-12-20 08:56:54.000000 icclim-6.4.0/MANIFEST.in
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     4534 2023-05-16 05:39:20.651227 icclim-6.4.0/PKG-INFO
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     3831 2022-12-20 08:56:54.000000 icclim-6.4.0/README.rst
+drwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        0 2023-05-16 05:39:18.396832 icclim-6.4.0/doc/
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      639 2022-12-20 08:56:54.000000 icclim-6.4.0/doc/Makefile
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      765 2022-12-20 08:56:54.000000 icclim-6.4.0/doc/make.bat
+drwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        0 2023-05-16 05:39:18.444294 icclim-6.4.0/doc/source/
+drwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        0 2023-05-16 05:39:18.449467 icclim-6.4.0/doc/source/_static/
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)    42702 2022-12-20 08:56:54.000000 icclim-6.4.0/doc/source/_static/chunks.png
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     3186 2022-12-20 08:56:54.000000 icclim-6.4.0/doc/source/conf.py
+drwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        0 2023-05-16 05:39:18.523068 icclim-6.4.0/doc/source/dev/
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      890 2022-12-20 08:56:54.000000 icclim-6.4.0/doc/source/dev/ci.rst
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)       47 2022-12-20 08:56:54.000000 icclim-6.4.0/doc/source/dev/contributing.rst
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      207 2022-12-20 08:56:54.000000 icclim-6.4.0/doc/source/dev/index.rst
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     2270 2022-12-20 08:56:54.000000 icclim-6.4.0/doc/source/dev/release_process.rst
+drwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        0 2023-05-16 05:39:18.633956 icclim-6.4.0/doc/source/explanation/
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      485 2022-12-20 08:56:54.000000 icclim-6.4.0/doc/source/explanation/4.2.x_installation.rst
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)    18547 2022-12-20 08:56:54.000000 icclim-6.4.0/doc/source/explanation/climate_indices.rst
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      251 2022-12-20 08:56:54.000000 icclim-6.4.0/doc/source/explanation/index.rst
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     3616 2022-12-20 08:56:54.000000 icclim-6.4.0/doc/source/explanation/xclim_and_icclim.rst
+drwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        0 2023-05-16 05:39:18.846463 icclim-6.4.0/doc/source/how_to/
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)    29218 2022-12-20 08:56:54.000000 icclim-6.4.0/doc/source/how_to/dask.rst
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      589 2022-12-20 08:56:54.000000 icclim-6.4.0/doc/source/how_to/index.rst
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     1240 2022-12-20 08:56:54.000000 icclim-6.4.0/doc/source/how_to/notebooks.rst
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     7382 2022-12-20 08:56:54.000000 icclim-6.4.0/doc/source/how_to/ocgis.rst
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)    15192 2022-12-20 08:56:54.000000 icclim-6.4.0/doc/source/how_to/recipes_custom.rst
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     6935 2022-12-20 08:56:54.000000 icclim-6.4.0/doc/source/how_to/recipes_ecad.rst
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     8994 2022-12-20 08:56:54.000000 icclim-6.4.0/doc/source/how_to/recipes_generic.rst
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     2102 2022-12-20 08:56:54.000000 icclim-6.4.0/doc/source/index.rst
+drwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        0 2023-05-16 05:39:19.124338 icclim-6.4.0/doc/source/references/
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)    10456 2022-12-20 08:56:54.000000 icclim-6.4.0/doc/source/references/custom_indices.rst
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     1615 2022-12-20 08:56:54.000000 icclim-6.4.0/doc/source/references/ecad_functions_api.rst
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)       85 2022-12-20 08:56:54.000000 icclim-6.4.0/doc/source/references/frequency.rst
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     1619 2022-12-20 08:56:54.000000 icclim-6.4.0/doc/source/references/generic_functions_api.rst
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)    18267 2022-12-20 08:56:54.000000 icclim-6.4.0/doc/source/references/icclim_index_api.rst
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      530 2022-12-20 08:56:54.000000 icclim-6.4.0/doc/source/references/index.rst
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     5598 2022-12-20 08:56:54.000000 icclim-6.4.0/doc/source/references/output_metadata.rst
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)    17712 2023-05-16 05:37:50.000000 icclim-6.4.0/doc/source/references/release_notes.rst
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      299 2022-12-20 08:56:54.000000 icclim-6.4.0/doc/source/references/threshold.rst
+drwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        0 2023-05-16 05:39:19.156869 icclim-6.4.0/doc/source/tutorials/
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      237 2022-12-20 08:56:54.000000 icclim-6.4.0/doc/source/tutorials/index.rst
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     1229 2022-12-20 08:56:54.000000 icclim-6.4.0/doc/source/tutorials/installation.rst
+drwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        0 2023-05-16 05:39:19.526513 icclim-6.4.0/icclim/
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      520 2022-12-20 08:56:54.000000 icclim-6.4.0/icclim/__init__.py
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)   334504 2023-04-11 13:19:13.000000 icclim-6.4.0/icclim/_generated_api.py
+drwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        0 2023-05-16 05:39:19.613349 icclim-6.4.0/icclim/ecad/
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        0 2022-12-20 08:56:54.000000 icclim-6.4.0/icclim/ecad/__init__.py
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)    28468 2022-12-20 08:56:54.000000 icclim-6.4.0/icclim/ecad/ecad_indices.py
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     4292 2022-12-20 08:56:54.000000 icclim-6.4.0/icclim/ecad/xclim_binding.py
+drwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        0 2023-05-16 05:39:19.831648 icclim-6.4.0/icclim/generic_indices/
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        0 2022-12-20 08:56:54.000000 icclim-6.4.0/icclim/generic_indices/__init__.py
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)    44631 2023-04-25 15:09:39.000000 icclim-6.4.0/icclim/generic_indices/generic_indicators.py
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     9508 2022-12-20 08:56:54.000000 icclim-6.4.0/icclim/generic_indices/generic_templates.py
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     7845 2022-12-20 08:56:54.000000 icclim-6.4.0/icclim/generic_indices/standard_variable.py
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)    40401 2023-04-25 15:09:39.000000 icclim-6.4.0/icclim/generic_indices/threshold.py
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     5085 2022-12-20 08:56:54.000000 icclim-6.4.0/icclim/generic_indices/threshold_templates.py
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      478 2022-12-20 08:56:54.000000 icclim-6.4.0/icclim/icclim_exceptions.py
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     5957 2022-12-20 08:56:54.000000 icclim-6.4.0/icclim/icclim_logger.py
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      876 2022-12-20 08:56:54.000000 icclim-6.4.0/icclim/icclim_types.py
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)    30820 2022-12-20 08:56:54.000000 icclim-6.4.0/icclim/main.py
+drwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        0 2023-05-16 05:39:20.191576 icclim-6.4.0/icclim/models/
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      105 2022-12-20 08:56:54.000000 icclim-6.4.0/icclim/models/__init__.py
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     2627 2022-12-20 08:56:54.000000 icclim-6.4.0/icclim/models/cf_calendar.py
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)    11282 2023-04-11 13:19:13.000000 icclim-6.4.0/icclim/models/climate_variable.py
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     3289 2023-05-16 05:37:50.000000 icclim-6.4.0/icclim/models/constants.py
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)    17259 2022-12-20 08:56:54.000000 icclim-6.4.0/icclim/models/frequency.py
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      214 2022-12-20 08:56:54.000000 icclim-6.4.0/icclim/models/global_metadata.py
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     1925 2022-12-20 08:56:54.000000 icclim-6.4.0/icclim/models/index_config.py
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     1630 2022-12-20 08:56:54.000000 icclim-6.4.0/icclim/models/index_group.py
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      997 2022-12-20 08:56:54.000000 icclim-6.4.0/icclim/models/logical_link.py
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      546 2022-12-20 08:56:54.000000 icclim-6.4.0/icclim/models/netcdf_version.py
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     2480 2022-12-20 08:56:54.000000 icclim-6.4.0/icclim/models/operator.py
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      446 2022-12-20 08:56:54.000000 icclim-6.4.0/icclim/models/quantile_interpolation.py
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     1810 2022-12-20 08:56:54.000000 icclim-6.4.0/icclim/models/registry.py
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     2588 2022-12-20 08:56:54.000000 icclim-6.4.0/icclim/models/standard_index.py
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      863 2022-12-20 08:56:54.000000 icclim-6.4.0/icclim/models/user_index_dict.py
+drwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        0 2023-05-16 05:39:20.291987 icclim-6.4.0/icclim/pre_processing/
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        0 2022-12-20 08:56:54.000000 icclim-6.4.0/icclim/pre_processing/__init__.py
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      764 2022-12-20 08:56:54.000000 icclim-6.4.0/icclim/pre_processing/in_file_dictionary.py
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)    14655 2023-04-11 12:52:34.000000 icclim-6.4.0/icclim/pre_processing/input_parsing.py
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     8306 2022-12-20 08:56:54.000000 icclim-6.4.0/icclim/pre_processing/rechunk.py
+drwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        0 2023-05-16 05:39:20.623890 icclim-6.4.0/icclim/tests/
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        0 2022-12-20 08:56:54.000000 icclim-6.4.0/icclim/tests/__init__.py
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     2524 2022-12-20 08:56:54.000000 icclim-6.4.0/icclim/tests/test_cf_calendar.py
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      835 2022-12-20 08:56:54.000000 icclim-6.4.0/icclim/tests/test_ecad_indices.py
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     5753 2022-12-20 08:56:54.000000 icclim-6.4.0/icclim/tests/test_frequency.py
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)    13360 2022-12-20 08:56:54.000000 icclim-6.4.0/icclim/tests/test_generated_api.py
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      932 2022-12-20 08:56:54.000000 icclim-6.4.0/icclim/tests/test_index_group.py
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     6654 2023-02-15 09:31:22.000000 icclim-6.4.0/icclim/tests/test_input_parsing.py
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)    33580 2023-04-25 15:09:39.000000 icclim-6.4.0/icclim/tests/test_main.py
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     2845 2022-12-20 08:56:54.000000 icclim-6.4.0/icclim/tests/test_rechunk.py
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)    11082 2023-02-15 09:31:22.000000 icclim-6.4.0/icclim/tests/test_threshold.py
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)    10327 2022-12-20 08:56:54.000000 icclim-6.4.0/icclim/tests/test_user_index.py
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     1103 2023-04-25 15:09:39.000000 icclim-6.4.0/icclim/tests/testing_utils.py
+drwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        0 2023-05-16 05:39:20.645109 icclim-6.4.0/icclim/user_indices/
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        0 2022-12-20 08:56:54.000000 icclim-6.4.0/icclim/user_indices/__init__.py
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      973 2022-12-20 08:56:54.000000 icclim-6.4.0/icclim/user_indices/calc_operation.py
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     1730 2023-01-30 13:21:59.000000 icclim-6.4.0/icclim/utils.py
+drwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        0 2023-05-16 05:39:19.551319 icclim-6.4.0/icclim.egg-info/
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     4534 2023-05-16 05:39:17.000000 icclim-6.4.0/icclim.egg-info/PKG-INFO
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     2760 2023-05-16 05:39:17.000000 icclim-6.4.0/icclim.egg-info/SOURCES.txt
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        1 2023-05-16 05:39:17.000000 icclim-6.4.0/icclim.egg-info/dependency_links.txt
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      173 2023-05-16 05:39:17.000000 icclim-6.4.0/icclim.egg-info/requires.txt
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)        7 2023-05-16 05:39:17.000000 icclim-6.4.0/icclim.egg-info/top_level.txt
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)      559 2023-05-16 05:39:20.653079 icclim-6.4.0/setup.cfg
+-rwxrwxrwx   0 aaoun     (1000) aaoun     (1000)     1256 2023-05-16 05:37:50.000000 icclim-6.4.0/setup.py
```

### Comparing `icclim-6.3.0/LICENSE` & `icclim-6.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/PKG-INFO` & `icclim-6.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icclim
-Version: 6.3.0
+Version: 6.4.0
 Summary: Python library for climate indices calculation
 Home-page: https://github.com/cerfacs-globc/icclim
 Author: Christian P.
 Author-email: christian.page@cerfacs.fr
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `icclim-6.3.0/README.rst` & `icclim-6.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/doc/Makefile` & `icclim-6.4.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/doc/make.bat` & `icclim-6.4.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/doc/source/_static/chunks.png` & `icclim-6.4.0/doc/source/_static/chunks.png`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/doc/source/conf.py` & `icclim-6.4.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/doc/source/dev/ci.rst` & `icclim-6.4.0/doc/source/dev/ci.rst`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/doc/source/dev/release_process.rst` & `icclim-6.4.0/doc/source/dev/release_process.rst`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/doc/source/explanation/climate_indices.rst` & `icclim-6.4.0/doc/source/explanation/climate_indices.rst`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/doc/source/explanation/xclim_and_icclim.rst` & `icclim-6.4.0/doc/source/explanation/xclim_and_icclim.rst`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/doc/source/how_to/dask.rst` & `icclim-6.4.0/doc/source/how_to/dask.rst`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/doc/source/how_to/index.rst` & `icclim-6.4.0/doc/source/how_to/index.rst`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/doc/source/how_to/notebooks.rst` & `icclim-6.4.0/doc/source/how_to/notebooks.rst`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/doc/source/how_to/ocgis.rst` & `icclim-6.4.0/doc/source/how_to/ocgis.rst`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/doc/source/how_to/recipes_custom.rst` & `icclim-6.4.0/doc/source/how_to/recipes_custom.rst`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/doc/source/how_to/recipes_ecad.rst` & `icclim-6.4.0/doc/source/how_to/recipes_ecad.rst`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/doc/source/how_to/recipes_generic.rst` & `icclim-6.4.0/doc/source/how_to/recipes_generic.rst`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/doc/source/index.rst` & `icclim-6.4.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/doc/source/references/custom_indices.rst` & `icclim-6.4.0/doc/source/references/custom_indices.rst`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/doc/source/references/ecad_functions_api.rst` & `icclim-6.4.0/doc/source/references/ecad_functions_api.rst`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/doc/source/references/generic_functions_api.rst` & `icclim-6.4.0/doc/source/references/generic_functions_api.rst`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/doc/source/references/icclim_index_api.rst` & `icclim-6.4.0/doc/source/references/icclim_index_api.rst`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/doc/source/references/index.rst` & `icclim-6.4.0/doc/source/references/index.rst`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/doc/source/references/output_metadata.rst` & `icclim-6.4.0/doc/source/references/output_metadata.rst`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/doc/source/references/release_notes.rst` & `icclim-6.4.0/doc/source/references/release_notes.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Release history
 ===============
 
+6.4.0
+-----
+
+* [maint] Upgrade to xclim 0.43 (released on 09/05/2023).
+* [maint] Change how xclim is pinned to allow patch changes.
+
+
 6.3.0
 -----
 * [maint] Upgrade to xclim 0.42 (released on 04/04/2023).
-
 * [fix] **BREAKING CHANGE** The indicators based on the difference between two variables (ecad: DTR, ETR, vDTR and anomaly) gave wrong values due to a bad unit conversion of the output.
   This was for example the case when the input variables are in Kelvin, the difference between the two variables is still in Kelvin but it cannot be converted to degree Celsius with the ususal `+273.15`.
   To workaround this issue, we first convert inputs to the expected output unit and then we compute the index.
-
 * [fix] **BREAKING CHANGE** Indices based on both a percentile threshold and a `threshold_min_value` (for ecad: r75p, r75pTOT, r95p, r95pTOT, r99p, r99pTOT)
   are now computing the exceedance rate on values above `threshold_min_value` as well. Previously this `threshold_min_value` was used to compute the percentile and the total (for rxxpTOT indices)
   but not the exceedance rate.
 
 6.2.0
 -----
 * [maint] Upgrade and adapt to xclim 0.40.
   Moved PercentileDataArray from xclim to icclim.
   Adapted the unit cenversion to use the hydro context.
-
 * [fix] Pin xclim to exact 0.40 to avoid breaking changes.
 
 
 6.1.5
 -----
 * [fix] Bug fix: not assuming longitude and latitude are lon and lat with respect to output metadata. Fix needed to work on E-OBS and other datasets.
```

### Comparing `icclim-6.3.0/doc/source/tutorials/installation.rst` & `icclim-6.4.0/doc/source/tutorials/installation.rst`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/icclim/__init__.py` & `icclim-6.4.0/icclim/__init__.py`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/icclim/_generated_api.py` & `icclim-6.4.0/icclim/_generated_api.py`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/icclim/ecad/ecad_indices.py` & `icclim-6.4.0/icclim/ecad/ecad_indices.py`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/icclim/ecad/xclim_binding.py` & `icclim-6.4.0/icclim/ecad/xclim_binding.py`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/icclim/generic_indices/generic_indicators.py` & `icclim-6.4.0/icclim/generic_indices/generic_indicators.py`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/icclim/generic_indices/generic_templates.py` & `icclim-6.4.0/icclim/generic_indices/generic_templates.py`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/icclim/generic_indices/standard_variable.py` & `icclim-6.4.0/icclim/generic_indices/standard_variable.py`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/icclim/generic_indices/threshold.py` & `icclim-6.4.0/icclim/generic_indices/threshold.py`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/icclim/generic_indices/threshold_templates.py` & `icclim-6.4.0/icclim/generic_indices/threshold_templates.py`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/icclim/icclim_logger.py` & `icclim-6.4.0/icclim/icclim_logger.py`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/icclim/icclim_types.py` & `icclim-6.4.0/icclim/icclim_types.py`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/icclim/main.py` & `icclim-6.4.0/icclim/main.py`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/icclim/models/cf_calendar.py` & `icclim-6.4.0/icclim/models/cf_calendar.py`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/icclim/models/climate_variable.py` & `icclim-6.4.0/icclim/models/climate_variable.py`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/icclim/models/constants.py` & `icclim-6.4.0/icclim/models/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 # fmt: off
 # flake8: noqa
 
-ICCLIM_VERSION = "6.3.0"
+ICCLIM_VERSION = "6.4.0"
 
 # placeholders for user_index
 PERCENTILE_THRESHOLD_STAMP = "p"
 WET_DAY_THRESHOLD = 1  # 1mm
 USER_INDEX_PRECIPITATION_STAMP = "p"
 USER_INDEX_TEMPERATURE_STAMP = "t"
```

### Comparing `icclim-6.3.0/icclim/models/frequency.py` & `icclim-6.4.0/icclim/models/frequency.py`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/icclim/models/index_config.py` & `icclim-6.4.0/icclim/models/index_config.py`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/icclim/models/index_group.py` & `icclim-6.4.0/icclim/models/index_group.py`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/icclim/models/logical_link.py` & `icclim-6.4.0/icclim/models/logical_link.py`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/icclim/models/netcdf_version.py` & `icclim-6.4.0/icclim/models/netcdf_version.py`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/icclim/models/operator.py` & `icclim-6.4.0/icclim/models/operator.py`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/icclim/models/registry.py` & `icclim-6.4.0/icclim/models/registry.py`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/icclim/models/standard_index.py` & `icclim-6.4.0/icclim/models/standard_index.py`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/icclim/models/user_index_dict.py` & `icclim-6.4.0/icclim/models/user_index_dict.py`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/icclim/pre_processing/in_file_dictionary.py` & `icclim-6.4.0/icclim/pre_processing/in_file_dictionary.py`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/icclim/pre_processing/input_parsing.py` & `icclim-6.4.0/icclim/pre_processing/input_parsing.py`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/icclim/pre_processing/rechunk.py` & `icclim-6.4.0/icclim/pre_processing/rechunk.py`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/icclim/tests/test_cf_calendar.py` & `icclim-6.4.0/icclim/tests/test_cf_calendar.py`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/icclim/tests/test_ecad_indices.py` & `icclim-6.4.0/icclim/tests/test_ecad_indices.py`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/icclim/tests/test_frequency.py` & `icclim-6.4.0/icclim/tests/test_frequency.py`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/icclim/tests/test_generated_api.py` & `icclim-6.4.0/icclim/tests/test_generated_api.py`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/icclim/tests/test_index_group.py` & `icclim-6.4.0/icclim/tests/test_index_group.py`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/icclim/tests/test_input_parsing.py` & `icclim-6.4.0/icclim/tests/test_input_parsing.py`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/icclim/tests/test_main.py` & `icclim-6.4.0/icclim/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/icclim/tests/test_rechunk.py` & `icclim-6.4.0/icclim/tests/test_rechunk.py`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/icclim/tests/test_threshold.py` & `icclim-6.4.0/icclim/tests/test_threshold.py`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/icclim/tests/test_user_index.py` & `icclim-6.4.0/icclim/tests/test_user_index.py`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/icclim/tests/testing_utils.py` & `icclim-6.4.0/icclim/tests/testing_utils.py`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/icclim/user_indices/calc_operation.py` & `icclim-6.4.0/icclim/user_indices/calc_operation.py`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/icclim/utils.py` & `icclim-6.4.0/icclim/utils.py`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/icclim.egg-info/PKG-INFO` & `icclim-6.4.0/icclim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icclim
-Version: 6.3.0
+Version: 6.4.0
 Summary: Python library for climate indices calculation
 Home-page: https://github.com/cerfacs-globc/icclim
 Author: Christian P.
 Author-email: christian.page@cerfacs.fr
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `icclim-6.3.0/icclim.egg-info/SOURCES.txt` & `icclim-6.4.0/icclim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/setup.cfg` & `icclim-6.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `icclim-6.3.0/setup.py` & `icclim-6.4.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 MINIMAL_REQUIREMENTS = [
     "numpy>=1.16",
     "xarray>=2022.6",
-    "xclim==0.42",
+    "xclim>=0.43, <0.44",
     "cf_xarray>=0.7.4",
     "cftime>=1.4.1",
     "dask[array]",
     "netCDF4>=1.5.7",
     "pyyaml",
     "psutil",
     "zarr",
@@ -17,15 +17,15 @@
     "fsspec",
     "pandas>=1.3",
     "dateparser",
 ]
 
 setup(
     name="icclim",
-    version="6.3.0",
+    version="6.4.0",
     packages=find_packages(),
     author="Christian P.",
     author_email="christian.page@cerfacs.fr",
     description="Python library for climate indices calculation",
     long_description=open("README.rst").read(),
     long_description_content_type="text/x-rst",
     include_package_data=True,
```

