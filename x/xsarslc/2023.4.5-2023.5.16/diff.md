# Comparing `tmp/xsarslc-2023.4.5.tar.gz` & `tmp/xsarslc-2023.5.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xsarslc-2023.4.5.tar", last modified: Wed Apr  5 11:10:57 2023, max compression
+gzip compressed data, was "xsarslc-2023.5.16.tar", last modified: Tue May 16 13:34:43 2023, max compression
```

## Comparing `xsarslc-2023.4.5.tar` & `xsarslc-2023.5.16.tar`

### file list

```diff
@@ -1,100 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 11:10:57.144501 xsarslc-2023.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 11:10:57.128500 xsarslc-2023.4.5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 11:10:57.128500 xsarslc-2023.4.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-05 11:10:57.144501 xsarslc-2023.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 11:10:57.132500 xsarslc-2023.4.5/auxdata/
--rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/auxdata/S1A_IRs_IW1_HH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/auxdata/S1A_IRs_IW1_HV.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50600 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/auxdata/S1A_IRs_IW1_VH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50600 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/auxdata/S1A_IRs_IW1_VV.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/auxdata/S1A_IRs_IW2_VH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/auxdata/S1A_IRs_IW2_VV.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/auxdata/S1A_IRs_IW3_HH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/auxdata/S1A_IRs_IW3_HV.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/auxdata/S1A_IRs_IW3_VH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/auxdata/S1A_IRs_IW3_VV.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/auxdata/S1B_IRs_IW1_HH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/auxdata/S1B_IRs_IW1_HV.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50456 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/auxdata/S1B_IRs_IW1_VH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50456 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/auxdata/S1B_IRs_IW1_VV.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/auxdata/S1B_IRs_IW2_HH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/auxdata/S1B_IRs_IW2_HV.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50742 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/auxdata/S1B_IRs_IW2_VH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50742 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/auxdata/S1B_IRs_IW2_VV.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/auxdata/S1B_IRs_IW3_VH.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/auxdata/S1B_IRs_IW3_VV.nc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 11:10:57.124500 xsarslc-2023.4.5/ci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 11:10:57.132500 xsarslc-2023.4.5/ci/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/ci/requirements/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/ci/requirements/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 11:10:57.136500 xsarslc-2023.4.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/ATBD.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14602 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/ATBD_L1BSLC.tex
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 11:10:57.124500 xsarslc-2023.4.5/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 11:10:57.136500 xsarslc-2023.4.5/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/_static/css/xsarslc.css
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/basic_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    10850 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/crossspectra.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/cutoff.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 11:10:57.136500 xsarslc-2023.4.5/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/examples/default_impulseResponse_files_IW.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8498 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/examples/example_IW_compute_and_correct_from_impulse_response.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    14606 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/examples/example_WV_compute_and_correct_from_impulse_response.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/examples/intro.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/examples/xspec_IW_intra_and_inter_burst.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/examples/xspec_WV_example.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 11:10:57.140501 xsarslc-2023.4.5/docs/figures/
--rw-r--r--   0 runner    (1001) docker     (123)   422190 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/figures/NIRAN_NRCS_VH.png
--rw-r--r--   0 runner    (1001) docker     (123)   447722 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/figures/NIRAN_NRCS_vv.png
--rw-r--r--   0 runner    (1001) docker     (123)    75773 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/figures/S1_azimuth_IR_IW_VV.png
--rw-r--r--   0 runner    (1001) docker     (123)    31463 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/figures/S1_azimuth_IR_WV_VV.png
--rw-r--r--   0 runner    (1001) docker     (123)    97138 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/figures/S1_range_IR_IW_VV.png
--rw-r--r--   0 runner    (1001) docker     (123)    27568 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/figures/S1_range_IR_WV_VV.png
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/figures/index
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/normalizedvariance.rst
--rw-r--r--   0 runner    (1001) docker     (123)    59687 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/oceanspectrumSAR.png
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/docs/sigma0.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/requirements_doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 11:10:57.144501 xsarslc-2023.4.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 11:10:57.140501 xsarslc-2023.4.5/xsarslc/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/xsarslc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/xsarslc/burst.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/xsarslc/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/xsarslc/get_config_infos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/xsarslc/get_test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    11979 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/xsarslc/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 11:10:57.144501 xsarslc-2023.4.5/xsarslc/processing/
--rw-r--r--   0 runner    (1001) docker     (123)    12974 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/xsarslc/processing/HR_tiles.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/xsarslc/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/xsarslc/processing/deramping.py
--rw-r--r--   0 runner    (1001) docker     (123)    21873 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/xsarslc/processing/impulseResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)    22652 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/xsarslc/processing/interburst.py
--rw-r--r--   0 runner    (1001) docker     (123)    30041 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/xsarslc/processing/intraburst.py
--rw-r--r--   0 runner    (1001) docker     (123)    26717 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/xsarslc/processing/xspectra.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 11:10:57.144501 xsarslc-2023.4.5/xsarslc/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/xsarslc/scripts/L1B_xspectra_IW_SLC_IFR.py
--rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/xsarslc/scripts/L1B_xspectra_WV_SLC_IFR.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/xsarslc/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19993 2023-04-05 11:10:37.000000 xsarslc-2023.4.5/xsarslc/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 11:10:57.144501 xsarslc-2023.4.5/xsarslc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-05 11:10:57.000000 xsarslc-2023.4.5/xsarslc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-05 11:10:57.000000 xsarslc-2023.4.5/xsarslc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 11:10:57.000000 xsarslc-2023.4.5/xsarslc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-05 11:10:57.000000 xsarslc-2023.4.5/xsarslc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-05 11:10:57.000000 xsarslc-2023.4.5/xsarslc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-05 11:10:57.000000 xsarslc-2023.4.5/xsarslc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:34:43.449299 xsarslc-2023.5.16/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:34:43.433299 xsarslc-2023.5.16/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:34:43.433299 xsarslc-2023.5.16/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-16 13:34:43.449299 xsarslc-2023.5.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:34:43.437299 xsarslc-2023.5.16/auxdata/
+-rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/auxdata/S1A_IRs_IW1_HH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/auxdata/S1A_IRs_IW1_HV.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50600 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/auxdata/S1A_IRs_IW1_VH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50600 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/auxdata/S1A_IRs_IW1_VV.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/auxdata/S1A_IRs_IW2_VH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/auxdata/S1A_IRs_IW2_VV.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/auxdata/S1A_IRs_IW3_HH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/auxdata/S1A_IRs_IW3_HV.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/auxdata/S1A_IRs_IW3_VH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/auxdata/S1A_IRs_IW3_VV.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/auxdata/S1B_IRs_IW1_HH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/auxdata/S1B_IRs_IW1_HV.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50456 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/auxdata/S1B_IRs_IW1_VH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50456 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/auxdata/S1B_IRs_IW1_VV.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/auxdata/S1B_IRs_IW2_HH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/auxdata/S1B_IRs_IW2_HV.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50742 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/auxdata/S1B_IRs_IW2_VH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50742 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/auxdata/S1B_IRs_IW2_VV.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/auxdata/S1B_IRs_IW3_VH.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50314 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/auxdata/S1B_IRs_IW3_VV.nc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:34:43.433299 xsarslc-2023.5.16/ci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:34:43.437299 xsarslc-2023.5.16/ci/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/ci/requirements/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/ci/requirements/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:34:43.441299 xsarslc-2023.5.16/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/ATBD.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14602 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/ATBD_L1BSLC.tex
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:34:43.433299 xsarslc-2023.5.16/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:34:43.441299 xsarslc-2023.5.16/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/_static/css/xsarslc.css
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/basic_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10850 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/crossspectra.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/cutoff.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:34:43.441299 xsarslc-2023.5.16/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/examples/default_impulseResponse_files_IW.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8498 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/examples/example_IW_compute_and_correct_from_impulse_response.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    14606 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/examples/example_WV_compute_and_correct_from_impulse_response.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/examples/intro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/examples/xspec_IW_intra_and_inter_burst.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/examples/xspec_WV_example.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:34:43.445299 xsarslc-2023.5.16/docs/figures/
+-rw-r--r--   0 runner    (1001) docker     (123)   422190 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/figures/NIRAN_NRCS_VH.png
+-rw-r--r--   0 runner    (1001) docker     (123)   447722 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/figures/NIRAN_NRCS_vv.png
+-rw-r--r--   0 runner    (1001) docker     (123)    75773 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/figures/S1_azimuth_IR_IW_VV.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31463 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/figures/S1_azimuth_IR_WV_VV.png
+-rw-r--r--   0 runner    (1001) docker     (123)    97138 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/figures/S1_range_IR_IW_VV.png
+-rw-r--r--   0 runner    (1001) docker     (123)    27568 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/figures/S1_range_IR_WV_VV.png
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/figures/index
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/normalizedvariance.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    59687 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/oceanspectrumSAR.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/docs/sigma0.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/requirements_doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:34:43.449299 xsarslc-2023.5.16/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:34:43.445299 xsarslc-2023.5.16/xsarslc/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/xsarslc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/xsarslc/burst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/xsarslc/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/xsarslc/get_config_infos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/xsarslc/get_test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12447 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/xsarslc/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:34:43.445299 xsarslc-2023.5.16/xsarslc/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)    12974 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/xsarslc/processing/HR_tiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/xsarslc/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/xsarslc/processing/deramping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21873 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/xsarslc/processing/impulseResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23075 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/xsarslc/processing/interburst.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30553 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/xsarslc/processing/intraburst.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28917 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/xsarslc/processing/xspectra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:34:43.445299 xsarslc-2023.5.16/xsarslc/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    10241 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/xsarslc/scripts/L1B_xspectra_EW_SLC_IFR.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/xsarslc/scripts/L1B_xspectra_IW_SLC_IFR.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/xsarslc/scripts/L1B_xspectra_WV_SLC_IFR.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/xsarslc/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20138 2023-05-16 13:34:27.000000 xsarslc-2023.5.16/xsarslc/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:34:43.445299 xsarslc-2023.5.16/xsarslc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-16 13:34:43.000000 xsarslc-2023.5.16/xsarslc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-16 13:34:43.000000 xsarslc-2023.5.16/xsarslc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:34:43.000000 xsarslc-2023.5.16/xsarslc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-16 13:34:43.000000 xsarslc-2023.5.16/xsarslc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-16 13:34:43.000000 xsarslc-2023.5.16/xsarslc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 13:34:43.000000 xsarslc-2023.5.16/xsarslc.egg-info/top_level.txt
```

### Comparing `xsarslc-2023.4.5/.github/workflows/publish.yml` & `xsarslc-2023.5.16/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/.gitignore` & `xsarslc-2023.5.16/.gitignore`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/.pre-commit-config.yaml` & `xsarslc-2023.5.16/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/LICENSE` & `xsarslc-2023.5.16/LICENSE`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/PKG-INFO` & `xsarslc-2023.5.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xsarslc
-Version: 2023.4.5
+Version: 2023.5.16
 Summary: Python library to compute cross spectra from SAR image
 Author: Frederic Nouguier
 License: GPL-3.0
 Keywords: SAR,wave,reseach,cross-spectra
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `xsarslc-2023.4.5/auxdata/S1A_IRs_IW1_HH.nc` & `xsarslc-2023.5.16/auxdata/S1A_IRs_IW1_HH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/auxdata/S1A_IRs_IW1_HV.nc` & `xsarslc-2023.5.16/auxdata/S1A_IRs_IW1_HV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/auxdata/S1A_IRs_IW1_VH.nc` & `xsarslc-2023.5.16/auxdata/S1A_IRs_IW1_VH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/auxdata/S1A_IRs_IW1_VV.nc` & `xsarslc-2023.5.16/auxdata/S1A_IRs_IW1_VV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/auxdata/S1A_IRs_IW2_VH.nc` & `xsarslc-2023.5.16/auxdata/S1A_IRs_IW2_VH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/auxdata/S1A_IRs_IW2_VV.nc` & `xsarslc-2023.5.16/auxdata/S1A_IRs_IW2_VV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/auxdata/S1A_IRs_IW3_HH.nc` & `xsarslc-2023.5.16/auxdata/S1A_IRs_IW3_HH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/auxdata/S1A_IRs_IW3_HV.nc` & `xsarslc-2023.5.16/auxdata/S1A_IRs_IW3_HV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/auxdata/S1A_IRs_IW3_VH.nc` & `xsarslc-2023.5.16/auxdata/S1A_IRs_IW3_VH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/auxdata/S1A_IRs_IW3_VV.nc` & `xsarslc-2023.5.16/auxdata/S1A_IRs_IW3_VV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/auxdata/S1B_IRs_IW1_HH.nc` & `xsarslc-2023.5.16/auxdata/S1B_IRs_IW1_HH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/auxdata/S1B_IRs_IW1_HV.nc` & `xsarslc-2023.5.16/auxdata/S1B_IRs_IW1_HV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/auxdata/S1B_IRs_IW1_VH.nc` & `xsarslc-2023.5.16/auxdata/S1B_IRs_IW1_VH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/auxdata/S1B_IRs_IW1_VV.nc` & `xsarslc-2023.5.16/auxdata/S1B_IRs_IW1_VV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/auxdata/S1B_IRs_IW2_HH.nc` & `xsarslc-2023.5.16/auxdata/S1B_IRs_IW2_HH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/auxdata/S1B_IRs_IW2_HV.nc` & `xsarslc-2023.5.16/auxdata/S1B_IRs_IW2_HV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/auxdata/S1B_IRs_IW2_VH.nc` & `xsarslc-2023.5.16/auxdata/S1B_IRs_IW2_VH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/auxdata/S1B_IRs_IW2_VV.nc` & `xsarslc-2023.5.16/auxdata/S1B_IRs_IW2_VV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/auxdata/S1B_IRs_IW3_VH.nc` & `xsarslc-2023.5.16/auxdata/S1B_IRs_IW3_VH.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/auxdata/S1B_IRs_IW3_VV.nc` & `xsarslc-2023.5.16/auxdata/S1B_IRs_IW3_VV.nc`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/docs/ATBD.rst` & `xsarslc-2023.5.16/docs/ATBD.rst`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/docs/ATBD_L1BSLC.tex` & `xsarslc-2023.5.16/docs/ATBD_L1BSLC.tex`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/docs/Makefile` & `xsarslc-2023.5.16/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/docs/basic_api.rst` & `xsarslc-2023.5.16/docs/basic_api.rst`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/docs/conf.py` & `xsarslc-2023.5.16/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/docs/crossspectra.rst` & `xsarslc-2023.5.16/docs/crossspectra.rst`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/docs/cutoff.rst` & `xsarslc-2023.5.16/docs/cutoff.rst`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/docs/examples/default_impulseResponse_files_IW.ipynb` & `xsarslc-2023.5.16/docs/examples/default_impulseResponse_files_IW.ipynb`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/docs/examples/example_IW_compute_and_correct_from_impulse_response.ipynb` & `xsarslc-2023.5.16/docs/examples/example_IW_compute_and_correct_from_impulse_response.ipynb`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/docs/examples/example_WV_compute_and_correct_from_impulse_response.ipynb` & `xsarslc-2023.5.16/docs/examples/example_WV_compute_and_correct_from_impulse_response.ipynb`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/docs/examples/xspec_IW_intra_and_inter_burst.ipynb` & `xsarslc-2023.5.16/docs/examples/xspec_IW_intra_and_inter_burst.ipynb`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/docs/examples/xspec_WV_example.ipynb` & `xsarslc-2023.5.16/docs/examples/xspec_WV_example.ipynb`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/docs/figures/NIRAN_NRCS_VH.png` & `xsarslc-2023.5.16/docs/figures/NIRAN_NRCS_VH.png`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/docs/figures/NIRAN_NRCS_vv.png` & `xsarslc-2023.5.16/docs/figures/NIRAN_NRCS_vv.png`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/docs/figures/S1_azimuth_IR_IW_VV.png` & `xsarslc-2023.5.16/docs/figures/S1_azimuth_IR_IW_VV.png`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/docs/figures/S1_azimuth_IR_WV_VV.png` & `xsarslc-2023.5.16/docs/figures/S1_azimuth_IR_WV_VV.png`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/docs/figures/S1_range_IR_IW_VV.png` & `xsarslc-2023.5.16/docs/figures/S1_range_IR_IW_VV.png`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/docs/figures/S1_range_IR_WV_VV.png` & `xsarslc-2023.5.16/docs/figures/S1_range_IR_WV_VV.png`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/docs/index.rst` & `xsarslc-2023.5.16/docs/index.rst`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/docs/installing.rst` & `xsarslc-2023.5.16/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/docs/normalizedvariance.rst` & `xsarslc-2023.5.16/docs/normalizedvariance.rst`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/docs/oceanspectrumSAR.png` & `xsarslc-2023.5.16/docs/oceanspectrumSAR.png`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/docs/sigma0.rst` & `xsarslc-2023.5.16/docs/sigma0.rst`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/pyproject.toml` & `xsarslc-2023.5.16/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -40,8 +40,9 @@
 skip_gitignore = true
 float_to_top = true
 default_section = "THIRDPARTY"
 known_first_party = "xsarslc"
 
 [project.scripts]
 L1B_xspectra_IW_SLC_IFR = "xsarslc.scripts.L1B_xspectra_IW_SLC_IFR:main"
-L1B_xspectra_WV_SLC_IFR = "xsarslc.scripts.L1B_xspectra_WV_SLC_IFR:main"
+L1B_xspectra_WV_SLC_IFR = "xsarslc.scripts.L1B_xspectra_WV_SLC_IFR:main"
+L1B_xspectra_EW_SLC_IFR = "xsarslc.scripts.L1B_xspectra_EW_SLC_IFR:main"
```

### Comparing `xsarslc-2023.4.5/xsarslc/burst.py` & `xsarslc-2023.5.16/xsarslc/burst.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/xsarslc/config.yml` & `xsarslc-2023.5.16/xsarslc/config.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # default data dir for tests and examples
 data_dir: /tmp
 product_version: 1.5
-default_outputdir_iw: '/home/datawork-cersat-public/project/sarwave/data/products/tests/iw/slc/l1b'
-default_outputdir_wv: '/home/datawork-cersat-public/project/sarwave/data/products/tests/wv/slc/l1b'
-default_landmask_dir: '/home1/datahome/agrouaze/.local/share/cartopy/'
+default_outputdir_iw: './data/products/tests/iw/slc/l1b'
+default_outputdir_ew: './data/products/tests/ew/slc/l1b'
+default_outputdir_wv: './data/products/tests/wv/slc/l1b'
+default_landmask_dir: '~/.local/share/cartopy/'
 xspec_configs:
   tiles20km:
     tile_width_intra:
       sample: 20000
       line: 20000
     tile_overlap_intra:
       sample: 0
```

### Comparing `xsarslc-2023.4.5/xsarslc/get_config_infos.py` & `xsarslc-2023.5.16/xsarslc/get_config_infos.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/xsarslc/get_test_files.py` & `xsarslc-2023.5.16/xsarslc/get_test_files.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/xsarslc/interface.py` & `xsarslc-2023.5.16/xsarslc/interface.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,19 +26,20 @@
     import datatree
     dt = datatree.open_datatree(file_path)
     L1B = dt[xspectra+'burst'].ds
     tiles = get_tiles_from_L1B_SLC(L1B)
     low_res_tiles = list()
     for mytile in tiles:
         mytile.load()
-        incidence = mytile['incidence']
-        if not np.isnan(incidence): # incidence is set at "Nan" when no data available in tile (ex: not on waters)
+        if not mytile['land_flag']:
+            incidence = mytile['incidence']
             spacing = {'sample':mytile['sampleSpacing']/np.sin(np.radians(incidence)), 'line':mytile['lineSpacing']}
             low_res_tiles.append(compute_low_res_tiles(mytile, spacing = spacing, posting = posting, tile_width=tile_width, window=window, **kwargs))
     res = xr.combine_by_coords([t.expand_dims(['burst', 'tile_sample', 'tile_line']) for t in low_res_tiles])
+    res['land_flag'] = res['land_flag'].fillna(1).astype(bool)
     attrs = L1B.attrs.copy()
     attr_to_rm = ['comment','azimuth_time_interval','periodo_width_sample','periodo_width_line','periodo_overlap_sample','periodo_overlap_line']
     [attrs.pop(k,None) for k in attr_to_rm]
     res.attrs.update(attrs)
     return res
 
 def compute_low_res_tiles(tile, spacing, posting, tile_width, resolution=None, window = 'GAUSSIAN'):
@@ -97,17 +98,16 @@
     corner_lon = tile['corner_longitude'].interp(c_sample = decimated['sample'][[0,-1]], c_line = decimated['line'][[0,-1]]).rename({'range':'c_range', 'azimuth':'c_azimuth'})
     decimated = decimated.drop_vars(['line','sample'])
     decimated.attrs.update(sigma0.attrs)
     corner_lat = corner_lat.drop_vars(['line','sample', 'c_line', 'c_sample'])
     corner_lon = corner_lon.drop_vars(['line','sample', 'c_line', 'c_sample'])
     range_spacing = xr.DataArray(posting['sample'], attrs={'units':'m', 'long_name':'ground range spacing'}, name='range_spacing')
     azimuth_spacing = xr.DataArray(posting['line'], attrs={'units':'m', 'long_name':'azimuth spacing'}, name='azimuth_spacing')
-    heading = tile['ground_heading']
-    incidence = tile['incidence']
-    decimated = xr.merge([decimated.to_dataset(),corner_lat.to_dataset(), corner_lon.to_dataset(), range_spacing.to_dataset(), azimuth_spacing.to_dataset(), heading.to_dataset(), incidence.to_dataset()])
+    added_variables = [tile[v].to_dataset() for v in ['incidence','ground_heading','land_flag']] # add variables from L1B to output
+    decimated = xr.merge([decimated.to_dataset(),corner_lat.to_dataset(), corner_lon.to_dataset(), range_spacing.to_dataset(), azimuth_spacing.to_dataset(), *added_variables])
     decimated = decimated.transpose('azimuth', 'range', 'c_azimuth', 'c_range', ...)
     return decimated
 
 def get_tiles_from_L1B_SLC(L1B, polarization=None):
     """
     Return list of tiles (sigma0) based on L1B informations. Open original SLC file, extract DN and calibrate sigma0
     Args:
@@ -127,23 +127,28 @@
     DN = dt['measurement']['digital_number'].sel(pol=polarization)
     sigma0_lut = dt['calibration']['sigma0_lut'].sel(pol=polarization)
     range_noise_lut = dt['noise_range'].ds['noise_lut'].sel(pol=polarization)
     azimuth_noise_lut = dt['noise_azimuth'].ds['noise_lut'].sel(pol=polarization)
     sample_spacing = dt['measurement']['sampleSpacing']
     line_spacing = dt['measurement']['lineSpacing']
     DN_tiles = new_get_tiles(DN, tiles_index)
-    
-    noise = (azimuth_noise_lut.interp_like(DN, assume_sorted=True))*(range_noise_lut.interp_like(DN, assume_sorted=True))
+
     sigma0 = list()
     for DN in DN_tiles:
+        range_noise_lut_mytile = range_noise_lut.interp_like(DN, assume_sorted=True)
+        if np.any(np.isnan(range_noise_lut_mytile)):
+            mid_burst_line = int(dt['bursts']['linesPerBurst'].item()*(DN['burst'].item()+0.5))
+            range_noise_lut_mytile = range_noise_lut.sel(line=mid_burst_line, method='nearest').drop_vars('line') # taking closest line
+            range_noise_lut_mytile = range_noise_lut_mytile.interp_like(DN, assume_sorted=True)
+        noise = (azimuth_noise_lut.interp_like(DN, assume_sorted=True))*range_noise_lut_mytile
         calibrated_DN = ((np.abs(DN)**2-noise)/((sigma0_lut.interp_like(DN, assume_sorted=True))**2)).rename('sigma0')
         calibrated_DN.attrs.update({'long_name': 'calibrated sigma0', 'units': 'linear'})
         tile_coords = {'burst':calibrated_DN['burst'], 'tile_line':calibrated_DN['tile_line'], 'tile_sample':calibrated_DN['tile_sample']}
         calibrated_DN = calibrated_DN.assign_coords({'longitude':L1B['longitude'].sel(tile_coords).item(),'latitude':L1B['latitude'].sel(tile_coords).item()})
-        added_variables = [L1B[v].sel(tile_coords).to_dataset() for v in ['incidence','corner_longitude', 'corner_latitude', 'ground_heading']] # add variables from L1B to output
+        added_variables = [L1B[v].sel(tile_coords).to_dataset() for v in ['incidence','corner_longitude', 'corner_latitude', 'ground_heading','land_flag']] # add variables from L1B to output
         calibrated_DN = xr.merge([calibrated_DN,*added_variables, sample_spacing.to_dataset(), line_spacing.to_dataset()])
         calibrated_DN = calibrated_DN.assign_coords({'c_sample':L1B.sel(tile_coords)['corner_sample'].data, 'c_line':L1B.sel(tile_coords)['corner_line'].data})
         sigma0.append(calibrated_DN)
     return sigma0
 
 def get_tiles_index_from_L1B_SLC(L1B):
     """
```

### Comparing `xsarslc-2023.4.5/xsarslc/processing/HR_tiles.py` & `xsarslc-2023.5.16/xsarslc/processing/HR_tiles.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/xsarslc/processing/deramping.py` & `xsarslc-2023.5.16/xsarslc/processing/deramping.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/xsarslc/processing/impulseResponse.py` & `xsarslc-2023.5.16/xsarslc/processing/impulseResponse.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/xsarslc/processing/interburst.py` & `xsarslc-2023.5.16/xsarslc/processing/interburst.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         lowpass_width (dict): width for low pass filtering [m]. Dict of form {dim_name (str): width (float)}
         landmask (optional) : If provided, land mask passed to is_ocean(). Otherwise xspectra are calculated by default
         IR_path (str, optional) : a path to the Impulse Response file
     Keyword Args:
         kwargs: keyword arguments passed to compute_interburst_xspectrum()
     """
     from xsarslc.tools import get_tiles, get_corner_tile, get_middle_tile, is_ocean, FullResolutionInterpolation, haversine
-    from xsarslc.processing.xspectra import compute_modulation, compute_azimuth_cutoff, compute_normalized_variance, compute_mean_sigma0
+    from xsarslc.processing.xspectra import compute_modulation, compute_azimuth_cutoff, compute_normalized_variance, compute_mean_sigma0_interp, compute_mean_sigma0_closest
 
     # ------------------ preprocessing --------------
     azitime_interval = burst0.attrs['azimuth_time_interval']
     azimuth_spacing = float(burst0['lineSpacing'])
 
     # -------- find overlapping burst portion -----------
 
@@ -205,24 +205,26 @@
         azimuth_spacing = float(sub['lineSpacing'])
 
 
         mod0 = compute_modulation(np.abs(sub0['digital_number']), lowpass_width=lowpass_width,
                                   spacing={'sample': ground_spacing, 'line': azimuth_spacing})
         # ------------- nv ------------
         nv = compute_normalized_variance(mod0)
-        # ------------- mean sigma0 ------------
-        sigma0 = compute_mean_sigma0(sub0['digital_number'], calibration['sigma0_lut'], noise_range['noise_lut'], noise_azimuth['noise_lut'])
+        # ------------- mean sigma0 and nesz ------------
+        sigma0, nesz = compute_mean_sigma0_interp(sub0['digital_number'], calibration['sigma0_lut'], noise_range['noise_lut'], noise_azimuth['noise_lut'])
+        if not np.isfinite(sigma0): # should only append in IW mode. Case when line are badly indexed in noise-range LUT
+            sigma0, nesz = compute_mean_sigma0_closest(sub0['digital_number'], burst['linesPerBurst'], calibration['sigma0_lut'], noise_range['noise_lut'], noise_azimuth['noise_lut'])
         # ------------- mean incidence ------------
         mean_incidence = xr.DataArray(mean_incidence, name='incidence', attrs={'long_name':'incidence at tile middle', 'units':'degree'})
         # ------------- heading ------------
         _,heading = haversine(float(corner_lons.sel(mytile)[{'c_line': 0, 'c_sample': 0}]), float(corner_lats.sel(mytile)[{'c_line': 0, 'c_sample': 0}]), float(corner_lons.sel(mytile)[{'c_line': 1, 'c_sample': 0}]), float(corner_lats.sel(mytile)[{'c_line': 1, 'c_sample': 0}]))
         ground_heading = xr.DataArray(float(heading), name='ground_heading', attrs={'long_name':'ground heading', 'units':'degree', 'convention':'from North clockwise'})
 
         # ---------------- part of the variables to be added to the final dataset ----------------------
-        variables_list+=[mean_incidence.to_dataset(), nv.to_dataset(), sigma0.to_dataset(), ground_heading.to_dataset()]
+        variables_list+=[mean_incidence.to_dataset(), nv.to_dataset(), sigma0.to_dataset(), nesz.to_dataset(), ground_heading.to_dataset()]
 
         if water_only:
 
             periodo_spacing = {'sample': ground_spacing, 'line': azimuth_spacing}
             nperseg_periodo = {d: int(np.rint(periodo_width[d] / periodo_spacing[d])) for d in tile_width.keys()}
             noverlap_periodo = {d: int(np.rint(periodo_overlap[d] / periodo_spacing[d])) for d in tile_width.keys()}
 
@@ -248,16 +250,17 @@
             dist1 = (sub1[{'line': sub1.sizes['line'] // 2}]['line'] - sub1['linesPerBurst'] * sub1[
                 'burst']) * azimuth_spacing  # distance from begining of the burst
             tau = (sub1['sensingTime'] - sub0['sensingTime']) / np.timedelta64(1, 's') + (
                         dist1 - dist0) / scan_velocity  # The division by timedelta64(1,s) is to convert in seconds
             tau = xr.DataArray(float(tau), name='tau', attrs={'long_name': 'delay between two successive acquisitions', 'units': 's'})
             # ------------- cut-off --------------
             xs_cut = xspecs_m.swap_dims({'freq_sample': 'k_rg', 'freq_line': 'k_az'})
-            cutoff = compute_azimuth_cutoff(xs_cut)
-            variables_list+=[xspecs_m, tau.to_dataset(), cutoff.to_dataset()]
+            cutoff, cutoff_error = compute_azimuth_cutoff(xs_cut)
+
+            variables_list+=[xspecs_m, tau.to_dataset(), cutoff.to_dataset(), cutoff_error.to_dataset()]
 
         # ------------- concatenate all variables ------------
         xs.append(xr.merge(variables_list))
 
 
     Nfreqs = [x.sizes['freq_sample'] if 'freq_sample' in x.dims else np.nan for x in xs if 'freq_sample' in x.dims]
     if np.any(np.isfinite(Nfreqs)):
@@ -279,18 +282,19 @@
     xs = xs.assign_coords({'longitude': middle_lons,
                            'latitude': middle_lats})  # This line also ensures adding line/sample coordinates too !! DO NOT REMOVE
     xs.attrs.update(burst.attrs)
     xs.attrs.update({'tile_width_' + d: k for d, k in tile_width.items()})
     xs.attrs.update({'tile_overlap_' + d: k for d, k in tile_overlap.items()})
     xs.attrs.update({'periodo_width_' + d: k for d, k in periodo_width.items()})
     xs.attrs.update({'periodo_overlap_' + d: k for d, k in periodo_overlap.items()})
-
-    landflag = xr.combine_by_coords([l.expand_dims(['tile_sample', 'tile_line']) for l in landflag])['land_flag'] if landflag else xr.DataArray(np.nan, name='land_mask')
-    landflag.attrs.update({'long_name': 'land flag', 'convention': 'True if land is present'})
-    xs = xr.merge([xs, landflag.to_dataset(), overlap_corner_lons.to_dataset(), overlap_corner_lats.to_dataset()], join = 'inner')
+    if landflag:
+        landflag = xr.combine_by_coords([l.expand_dims(['tile_sample', 'tile_line']) for l in landflag])['land_flag']
+        landflag.attrs.update({'long_name': 'land flag', 'convention': 'True if land is present'})
+        xs = xr.merge([xs, landflag.to_dataset()])    
+    xs = xr.merge([xs,overlap_corner_lons.to_dataset(), overlap_corner_lats.to_dataset()], join = 'inner')
     return xs
 
 
 def compute_interburst_xspectrum(mod0, mod1, mean_incidence, slant_spacing, azimuth_spacing, azimuth_dim='line',
                                  nperseg={'sample': 512, 'line': None}, noverlap={'sample': 256, 'line': 0},**kwargs):
     """
     Compute cross spectrum between mod0 and mod1 using a 2D Welch method (periodograms).
```

### Comparing `xsarslc-2023.4.5/xsarslc/processing/intraburst.py` & `xsarslc-2023.5.16/xsarslc/processing/intraburst.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         landmask (optional) : If provided, land mask passed to is_ocean(). Otherwise xspectra are calculated by default
         IR_path (str, optional) : a path to the Impulse Response file
     Keyword Args:
         landmask (optional) : If provided, land mask passed to is_ocean(). Otherwise xspectra are calculated by default
         kwargs: keyword arguments passed to compute_intraburst_xspectrum()
     """
     from xsarslc.tools import get_tiles, get_corner_tile, get_middle_tile, is_ocean, FullResolutionInterpolation, haversine
-    from xsarslc.processing.xspectra import compute_modulation, compute_azimuth_cutoff, compute_normalized_variance, compute_mean_sigma0
+    from xsarslc.processing.xspectra import compute_modulation, compute_azimuth_cutoff, compute_normalized_variance, compute_mean_sigma0_interp, compute_mean_sigma0_closest
 
 
 
     # burst.load()
 
     # ------------------ preprocessing --------------
     azitime_interval = burst.attrs['azimuth_time_interval']
@@ -185,25 +185,27 @@
 
         DN = sub['digital_number'] if sub.swath=='WV' else sub['deramped_digital_number']
         mod = compute_modulation(DN, lowpass_width=lowpass_width,
                                  spacing={'sample': ground_spacing, 'line': azimuth_spacing})
             
         # ------------- nv ------------
         nv = compute_normalized_variance(mod)
-        # ------------- mean sigma0 ------------
-        sigma0 = compute_mean_sigma0(DN, calibration['sigma0_lut'], noise_range['noise_lut'], noise_azimuth['noise_lut'])
+        # ------------- mean sigma0 and nesz ------------
+        sigma0, nesz = compute_mean_sigma0_interp(DN, calibration['sigma0_lut'], noise_range['noise_lut'], noise_azimuth['noise_lut'])
+        if not np.isfinite(sigma0): # should only append in IW mode. Case when line are badly indexed in noise-range LUT
+            sigma0, nesz = compute_mean_sigma0_closest(DN, burst['linesPerBurst'], calibration['sigma0_lut'], noise_range['noise_lut'], noise_azimuth['noise_lut'])
         # ------------- mean incidence ------------
         mean_incidence = xr.DataArray(mean_incidence, name='incidence', attrs={'long_name':'incidence at tile middle', 'units':'degree'})
         # ------------- heading ------------
         # heding below is computed on one border of the tile. It should be evaluated at the middle of the tile (maybe)    
         _,heading = haversine(float(corner_lons.sel(mytile)[{'c_line': 0, 'c_sample': 0}]), float(corner_lats.sel(mytile)[{'c_line': 0, 'c_sample': 0}]), float(corner_lons.sel(mytile)[{'c_line': 1, 'c_sample': 0}]), float(corner_lats.sel(mytile)[{'c_line': 1, 'c_sample': 0}]))
         ground_heading = xr.DataArray(float(heading), name='ground_heading', attrs={'long_name':'ground heading', 'units':'degree', 'convention':'from North clockwise'})
         
         # ---------------- part of the variables to be added to the final dataset ----------------------
-        variables_list+=[mean_incidence.to_dataset(), nv.to_dataset(), sigma0.to_dataset(), ground_heading.to_dataset()]
+        variables_list+=[mean_incidence.to_dataset(), nv.to_dataset(), sigma0.to_dataset(), nesz.to_dataset(), ground_heading.to_dataset()]
 
         if water_only:
             periodo_spacing = {'sample': ground_spacing, 'line': azimuth_spacing}
             nperseg_periodo = {d: int(np.rint(periodo_width[d] / periodo_spacing[d])) for d in tile_width.keys()}
             noverlap_periodo = {d: int(np.rint(periodo_overlap[d] / periodo_spacing[d])) for d in tile_width.keys()}
 
             if np.any([sub.sizes[d] < nperseg_periodo[d] for d in ['line', 'sample']]):
@@ -229,18 +231,19 @@
                 tau = float(xspecs_m.attrs.pop('tau'))
                 tau = xr.DataArray(float(tau), name='tau', attrs={'long_name': 'delay between two successive looks', 'units': 's'})
 
                 # ------------- cut-off ------------
                 cutoff_tau = [str(i) + 'tau' for i in [3, 2, 1, 0] if str(i) + 'tau' in xspecs_m.dims][0]  # tau used to compute azimuthal cutoff
                 xs_cut = xspecs_m['xspectra_' + cutoff_tau].mean(dim=cutoff_tau).swap_dims(
                     {'freq_sample': 'k_rg', 'freq_line': 'k_az'})
-                cutoff = compute_azimuth_cutoff(xs_cut)
+                cutoff, cutoff_error = compute_azimuth_cutoff(xs_cut)
                 cutoff.attrs.update({'long_name':cutoff.attrs['long_name']+' ('+cutoff_tau+')'})
+                cutoff_error.attrs.update({'long_name':cutoff_error.attrs['long_name']+' ('+cutoff_tau+')'})
 
-                variables_list+=[xspecs_m, xspecs_v, tau.to_dataset(), cutoff.to_dataset()]
+                variables_list+=[xspecs_m, xspecs_v, tau.to_dataset(), cutoff.to_dataset(), cutoff_error.to_dataset()]
         # ------------- concatenate all variables ------------
         xs.append(xr.merge(variables_list))
 
 
     Nfreqs = [x.sizes['freq_sample'] if 'freq_sample' in x.dims else np.nan for x in xs if 'freq_sample' in x.dims]
     if np.any(np.isfinite(Nfreqs)):
         # -------Returned xspecs have different shape in range (to keep same dk). Lines below only select common portions of xspectra-----
@@ -263,17 +266,20 @@
                            'latitude': middle_lats})  # This line also ensures adding line/sample coordinates too !! DO NOT REMOVE
     xs.attrs.update(burst.attrs)
     xs.attrs.update({'tile_width_' + d: k for d, k in tile_width.items()})
     xs.attrs.update({'tile_overlap_' + d: k for d, k in tile_overlap.items()})
     xs.attrs.update({'periodo_width_' + d: k for d, k in periodo_width.items()})
     xs.attrs.update({'periodo_overlap_' + d: k for d, k in periodo_overlap.items()})
 
-    landflag = xr.combine_by_coords([l.expand_dims(['tile_sample', 'tile_line']) for l in landflag])['land_flag'] if landflag else xr.DataArray(np.nan, name='land_mask')
-    landflag.attrs.update({'long_name': 'land flag', 'convention': 'True if land is present'})
-    xs = xr.merge([xs, landflag.to_dataset(), burst_corner_lons.to_dataset(), burst_corner_lats.to_dataset()], join = 'inner')
+    if landflag:
+        landflag = xr.combine_by_coords([l.expand_dims(['tile_sample', 'tile_line']) for l in landflag])['land_flag']
+        landflag.attrs.update({'long_name': 'land flag', 'convention': 'True if land is present'})
+        xs = xr.merge([xs, landflag.to_dataset()])   
+
+    xs = xr.merge([xs,burst_corner_lons.to_dataset(), burst_corner_lats.to_dataset()], join = 'inner')
     return xs
 
 
 
 def compute_intraburst_xspectrum(slc, mean_incidence, slant_spacing, azimuth_spacing, synthetic_duration,
                                  azimuth_dim='line', nperseg={'sample': 512, 'line': 512},
                                  noverlap={'sample': 256, 'line': 256}, IR_path=None, **kwargs):
```

### Comparing `xsarslc-2023.4.5/xsarslc/processing/xspectra.py` & `xsarslc-2023.5.16/xsarslc/processing/xspectra.py`

 * *Files 8% similar despite different names*

```diff
@@ -117,16 +117,15 @@
     xspectra = tile_burst_to_xspectra(burst, dt['geolocation_annotation'], dt['orbit'], dt['calibration'],
                                       dt['noise_range'], dt['noise_azimuth'], tile_width, tile_overlap, landmask=landmask, IR_path=IR_path, **kwargs)
     xspectra = xspectra.drop(
         ['tile_line', 'tile_sample'])  # dropping coordinate is important to not artificially multiply the dimensions
     if xspectra.sizes['tile_line'] == xspectra.sizes[
         'tile_sample'] == 1:  # In WV mode, it will probably be only one tile
         xspectra = xspectra.squeeze(['tile_line', 'tile_sample'])
-    dims_to_transpose = [d for d in ['tile_line', 'tile_sample', 'freq_line', 'freq_sample'] if
-                         d in xspectra.dims]  # for homogeneous order of dimensions with intraburst
+    xspectra = xs_formatting(xspectra)
     return xspectra
 
 
 def compute_IW_subswath_intraburst_xspectra(dt, polarization, periodo_width={'sample': 2000, 'line': 2000},
                                             periodo_overlap={'sample': 1000 ,'line': 1000},
                                             tile_width={'sample': 20.e3, 'line': 20.e3},
                                             tile_overlap={'sample': 10.e3, 'line': 10.e3}, landmask=None, IR_path=None, **kwargs):
@@ -198,18 +197,15 @@
     dims_not_align = set()
     for x in xspectra:
         dims_not_align=dims_not_align.union(set(x.dims))
     dims_not_align = dims_not_align-set(['tile_sample', 'tile_line'])
     xspectra = xr.align(*xspectra, exclude=dims_not_align, join='outer') # tile sample/line are aligned (thanks to their coordinate value) to avoid bug in combine_by_coords below
     xspectra = xr.combine_by_coords([x.drop(['tile_sample', 'tile_line']).reset_coords(['line','sample','longitude','latitude']).expand_dims('burst') for x in xspectra], combine_attrs='drop_conflicts')
     xspectra = xspectra.assign_coords({d:xspectra[d] for d in ['line','sample','longitude','latitude'] if d in xspectra}) # reseting and reassigning theses variables avoid some bug in combine_by_coords with missing variables between datasets
-    dims_to_transpose = [d for d in ['burst', 'tile_line', 'tile_sample', 'freq_line', 'freq_sample'] if
-                         d in xspectra.dims]  # for homogeneous order of dimensions with interburst
-    xspectra = xspectra.transpose(*dims_to_transpose, ...)
-
+    xspectra = xs_formatting(xspectra)
     return xspectra
 
 
 def compute_IW_subswath_interburst_xspectra(dt, polarization, periodo_width={'sample': 2000, 'line': 1200},
                                             periodo_overlap={'sample': 1000 ,'line': 600},
                                             tile_width={'sample': 20.e3, 'line': 1.5e3},
                                             tile_overlap={'sample': 10.e3, 'line': 0.75e3}, landmask=None, IR_path=None, **kwargs):
@@ -291,18 +287,35 @@
     dims_not_align = set()
     for x in xspectra:
         dims_not_align=dims_not_align.union(set(x.dims))
     dims_not_align = dims_not_align-set(['tile_sample', 'tile_line'])
     xspectra = xr.align(*xspectra, exclude=dims_not_align, join='outer') # tile sample/line are aligned (thanks to their coordinate value) to avoid bug in combine_by_coords below
     xspectra = xr.combine_by_coords([x.drop(['tile_sample', 'tile_line']).reset_coords(['line','sample','longitude','latitude']).expand_dims('burst') for x in xspectra], combine_attrs='drop_conflicts')
     xspectra = xspectra.assign_coords({d:xspectra[d] for d in ['line','sample','longitude','latitude'] if d in xspectra}) # reseting and reassigning theses variables avoid some bug in combine_by_coords with missing variables between datasets
+    xspectra = xs_formatting(xspectra)
+    return xspectra
+
+
+def xs_formatting(xspectra):
+    """
+    Format final returned xspectra. Transposing dimensions, checking data type, ...
+    Args:
+        xspectra (xarray.Dataset): xspectra to format
+    Return:
+        (xarray.Dataset): formatted xspectra
+
+    """
     dims_to_transpose = [d for d in ['burst', 'tile_line', 'tile_sample', 'freq_line', 'freq_sample'] if
                          d in xspectra.dims]  # for homogeneous order of dimensions with intraburst
     xspectra = xspectra.transpose(*dims_to_transpose, ...)
-
+    if 'land_flag' in xspectra:
+        xspectra['land_flag'] = xspectra['land_flag'].astype(bool)
+    if 'corner_line' in xspectra:
+        xspectra['corner_line'] = xspectra['corner_line'].astype(int)
+        xspectra['corner_sample'] = xspectra['corner_sample'].astype(int)
     return xspectra
 
 
 def compute_modulation(ds, lowpass_width, spacing):
     """
     Compute modulation map (sig0/low_pass_filtered_sig0)
 
@@ -357,25 +370,28 @@
     elif definition == 'drfab':
         coVRm = np.real(coV).sel(rg=0.0)
     else:
         raise ValueError("Unknow definition '{}' for azimuth cutoff. It must be 'drfab' or 'ipf'".format(definition))
     coVRm /= coVRm.max()
     coVfit = coVRm.where(np.abs(coVRm.az) < 500, drop=True)
 
+
     def fit_gauss(x, a, l):
         return a * np.exp(-(np.pi * x / l) ** 2)
 
     try:
-        p, r = curve_fit(fit_gauss, coVfit.az, coVfit.data, p0=[1., 227.])
+        p, pcov = curve_fit(fit_gauss, coVfit.az, coVfit.data, p0=[1., 227.])
         cutoff = p[1]
+        relat_err = np.abs((np.sqrt(np.diag(pcov))/p)[1])
     except:
-        cutoff = np.nan
+        cutoff, relat_err = np.nan, np.nan
 
     cutoff = xr.DataArray(float(cutoff), name='azimuth_cutoff', attrs={'long_name': 'Azimuthal cut-off', 'units': 'm'})
-    return cutoff
+    cutoff_error = xr.DataArray(float(relat_err), name='azimuth_cutoff_error', attrs={'long_name': 'normalized azimuthal cut-off error std'})
+    return cutoff, cutoff_error
 
 
 def compute_normalized_variance(modulation):
     """
     compute normalized variance from modulation of digital numbers
     Args:
         modulation (xarray): output from compute_modulation()
@@ -385,33 +401,67 @@
     detected_mod = np.abs(modulation) ** 2.
     nv = detected_mod.var(dim=['line', 'sample']) / ((detected_mod.mean(dim=['line', 'sample'])) ** 2)
     nv = nv.rename('normalized_variance')
     nv.attrs.update({'long_name': 'normalized variance', 'units': ''})
     return nv
 
 
-def compute_mean_sigma0(DN, sigma0_lut, range_noise_lut, azimuth_noise_lut):
+def compute_mean_sigma0_interp(DN, sigma0_lut, range_noise_lut, azimuth_noise_lut):
     """
-    compute mean calibrated sigma0
+    Compute mean calibrated sigma0 and mean noise equivalent sigma0. This is a version doing interpolation over the LUT instead of taking closest LUT
     Args:
         DN (xarray): digital number
         sigma0_lut (xarray) : calibration LUT of dataset
     Return:
         (xarray): calibrated mean sigma0 (single value)
+        (xarray): noise equivalent sigma0 (single value)
     """
     polarization = DN.pol.item()
     sigma0_lut = sigma0_lut.sel(pol=polarization)
     range_noise_lut = range_noise_lut.sel(pol=polarization)
     azimuth_noise_lut = azimuth_noise_lut.sel(pol=polarization)
     noise = (azimuth_noise_lut.interp_like(DN, assume_sorted=True)) * (
         range_noise_lut.interp_like(DN, assume_sorted=True))
-    sigma0 = (np.abs(DN) ** 2 - noise) / ((sigma0_lut.interp_like(DN, assume_sorted=True)) ** 2)
+    
+    calib = (sigma0_lut.interp_like(DN, assume_sorted=True)) ** 2
+    sigma0 = (np.abs(DN) ** 2 - noise) / calib
+    sigma0 = sigma0.mean(dim=['line', 'sample']).rename('sigma0')
+    sigma0.attrs.update({'long_name': 'calibrated sigma0', 'units': 'linear'})
+
+    nesz = (noise / calib).mean(dim=['line', 'sample']).rename('nesz')
+    nesz.attrs.update({'long_name': 'noise-equivalent sigma zero', 'units': 'linear'})
+
+    return sigma0, nesz
+
+def compute_mean_sigma0_closest(DN, linesPerBurst, sigma0_lut, range_noise_lut, azimuth_noise_lut):
+    """
+    Compute mean calibrated sigma0 and mean noise equivalent sigma0. This version uses closest line of the burst
+    Args:
+        DN (xarray): digital number
+        sigma0_lut (xarray) : calibration LUT of dataset
+    Return:
+        (xarray): calibrated mean sigma0 (single value)
+        (xarray): noise equivalent sigma0 (single value)
+    """
+    polarization = DN.pol.item()
+    sigma0_lut = sigma0_lut.sel(pol=polarization)
+    mid_burst_line = int(linesPerBurst*(DN['burst'].item()+0.5))
+    range_noise_lut = range_noise_lut.sel(pol=polarization).sel(line=mid_burst_line, method='nearest').drop_vars('line') # taking closest line
+    azimuth_noise_lut = azimuth_noise_lut.sel(pol=polarization)
+    noise = (azimuth_noise_lut.interp_like(DN, assume_sorted=True)) * (
+        range_noise_lut.interp_like(DN, assume_sorted=True))
+    
+    calib = (sigma0_lut.interp_like(DN, assume_sorted=True)) ** 2
+    sigma0 = (np.abs(DN) ** 2 - noise) / calib
     sigma0 = sigma0.mean(dim=['line', 'sample']).rename('sigma0')
     sigma0.attrs.update({'long_name': 'calibrated sigma0', 'units': 'linear'})
-    return sigma0
+
+    nesz = (noise / calib).mean(dim=['line', 'sample']).rename('nesz')
+    nesz.attrs.update({'long_name': 'noise-equivalent sigma zero', 'units': 'linear'})
+    return sigma0, nesz
 
 
 def symmetrize_xspectrum(xs, dim_range='k_rg', dim_azimuth='k_az'):
     """
     Symmetrize half-xspectrum around origin point. For correct behaviour, xs has to be complex and assumed to contain only positive wavenumbers in range.
     
     Args:
```

### Comparing `xsarslc-2023.4.5/xsarslc/scripts/L1B_xspectra_IW_SLC_IFR.py` & `xsarslc-2023.5.16/xsarslc/scripts/L1B_xspectra_IW_SLC_IFR.py`

 * *Files identical despite different names*

### Comparing `xsarslc-2023.4.5/xsarslc/scripts/L1B_xspectra_WV_SLC_IFR.py` & `xsarslc-2023.5.16/xsarslc/scripts/L1B_xspectra_WV_SLC_IFR.py`

 * *Files 7% similar despite different names*

```diff
@@ -148,14 +148,16 @@
                                               periodo_width_intra=periodo_width_intra,
                                               periodo_overlap_intra=periodo_overlap_intra,
                                               IR_path=IR_path, dev=dev, landmask=landmask)
     # xs = xs0.swap_dims({'freq_line': 'k_az', 'freq_sample': 'k_rg'})
     # xs = xspectra.symmetrize_xspectrum(xs, dim_range='k_rg', dim_azimuth='k_az')
     xs = netcdf_compliant(xs0)  # to split complex128 variables into real and imag part
     xs = xs.drop('pol')
+    var2drop = ['var_xspectra_0tau','var_xspectra_1tau','var_xspectra_2tau','xspectra_0tau_Re','xspectra_0tau_Im','xspectra_1tau_Re','xspectra_1tau_Im']
+    xs = xs.drop_vars(var2drop)
     if 'spatial_ref' in xs:
         xs = xs.drop('spatial_ref')
     if xs:
         logging.info('xspec ready for %s', slc_wv_path)
         logging.debug('one_subswath_xspectrum = %s', xs)
         xs.attrs['version_xsar'] = xsar.__version__
         xs.attrs['version_xsarslc'] = xsarslc.__version__
```

### Comparing `xsarslc-2023.4.5/xsarslc/tools.py` & `xsarslc-2023.5.16/xsarslc/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,16 +20,16 @@
     Returns:
         (xarray.DataArray): interpolated values of field at provided (lines, samples) coordinates
     """
     from scipy.interpolate import RectBivariateSpline
     geolocated_lines = line2geolocline(lines, geolocation_annotation, azimuthTimeInterval)  # Find geolocated lines
     LR_field = geolocation_annotation[field]  # Low resolution field
     field_interpolator = RectBivariateSpline(LR_field['line'].data, LR_field['sample'].data,
-                                             LR_field.transpose('line', 'sample').data, kx=1,
-                                             ky=1)  # interpolator of low resolution field
+                                             LR_field.transpose('line', 'sample').data, kx=3,
+                                             ky=3)  # interpolator of low resolution field
     out = from_HDresampler(geolocated_lines, samples, field_interpolator).rename(field)
     out.attrs.update(LR_field.attrs)
     return out
 
 
 def line2geolocline(lines, geolocation_annotation, azimuth_time_interval):
     """
@@ -60,14 +60,15 @@
         line=i_ref).data  # line number of the first line of reference burst is updated for the overlapping parts
 
     az_ref2 = aziTime.isel(line=i_ref + 1, sample=0).data
     l_ref2 = geolines.isel(line=i_ref + 1).data
     delta = (az_ref2 - az_ref) / (
             l_ref2 - l_ref)  # rate of azimuth time variation VS line number in the low resolution geolocation annotation
     geoloc_lines = l_ref + (az - az_ref) / delta
+    geoloc_lines = np.where(i_ref!=geolines.sizes['line'] - 2, geoloc_lines,lines.data) # Ensuring lines and geolines match on last burst only !
     if isinstance(lines, xr.DataArray):
         geoloc_lines = xr.DataArray(geoloc_lines, dims=lines.dims, coords=lines.coords).rename('geolocated_line')
 
     return geoloc_lines
 
 
 def from_HDresampler(geoloc_lines, samples, HD_resampler):
```

### Comparing `xsarslc-2023.4.5/xsarslc.egg-info/PKG-INFO` & `xsarslc-2023.5.16/xsarslc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xsarslc
-Version: 2023.4.5
+Version: 2023.5.16
 Summary: Python library to compute cross spectra from SAR image
 Author: Frederic Nouguier
 License: GPL-3.0
 Keywords: SAR,wave,reseach,cross-spectra
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `xsarslc-2023.4.5/xsarslc.egg-info/SOURCES.txt` & `xsarslc-2023.5.16/xsarslc.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -74,10 +74,11 @@
 xsarslc/processing/HR_tiles.py
 xsarslc/processing/__init__.py
 xsarslc/processing/deramping.py
 xsarslc/processing/impulseResponse.py
 xsarslc/processing/interburst.py
 xsarslc/processing/intraburst.py
 xsarslc/processing/xspectra.py
+xsarslc/scripts/L1B_xspectra_EW_SLC_IFR.py
 xsarslc/scripts/L1B_xspectra_IW_SLC_IFR.py
 xsarslc/scripts/L1B_xspectra_WV_SLC_IFR.py
 xsarslc/scripts/__init__.py
```

