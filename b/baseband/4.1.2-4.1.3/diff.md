# Comparing `tmp/baseband-4.1.2.tar.gz` & `tmp/baseband-4.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baseband-4.1.2.tar", last modified: Tue Dec 20 23:32:22 2022, max compression
+gzip compressed data, was "baseband-4.1.3.tar", last modified: Tue May 16 09:47:34 2023, max compression
```

## Comparing `baseband-4.1.2.tar` & `baseband-4.1.3.tar`

### file list

```diff
@@ -1,205 +1,206 @@
-drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2022-12-20 23:32:22.515203 baseband-4.1.2/
-drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2022-12-20 23:32:22.491201 baseband-4.1.2/.github/
-drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2022-12-20 23:32:22.495201 baseband-4.1.2/.github/workflows/
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     2398 2022-12-20 23:17:17.000000 baseband-4.1.2/.github/workflows/ci_cron_monthly.yml
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     2142 2022-12-20 23:26:01.000000 baseband-4.1.2/.github/workflows/ci_workflows.yml
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)      719 2020-12-14 22:27:09.000000 baseband-4.1.2/.gitignore
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)      170 2022-12-20 23:17:17.000000 baseband-4.1.2/.readthedocs.yml
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)      120 2020-12-14 22:27:09.000000 baseband-4.1.2/.rtd-environment.yml
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     1243 2021-11-29 22:19:55.000000 baseband-4.1.2/.zenodo.json
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     1081 2022-11-17 00:41:25.000000 baseband-4.1.2/AUTHORS.rst
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    14061 2022-12-20 23:31:02.000000 baseband-4.1.2/CHANGES.rst
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)       94 2020-07-14 20:59:29.000000 baseband-4.1.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)      196 2020-07-14 20:59:29.000000 baseband-4.1.2/CONTRIBUTING.md
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    35141 2020-07-14 20:59:29.000000 baseband-4.1.2/LICENSE
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)      346 2021-11-29 22:19:55.000000 baseband-4.1.2/MANIFEST.in
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     2551 2022-12-20 23:32:22.515203 baseband-4.1.2/PKG-INFO
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     2030 2021-11-29 22:19:55.000000 baseband-4.1.2/README.rst
-drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2022-12-20 23:32:22.495201 baseband-4.1.2/baseband/
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)      699 2022-12-20 23:17:17.000000 baseband-4.1.2/baseband/__init__.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)      613 2021-11-29 22:19:55.000000 baseband-4.1.2/baseband/_astropy_init.py
-drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2022-12-20 23:32:22.495201 baseband-4.1.2/baseband/base/
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     1065 2020-12-14 22:27:09.000000 baseband-4.1.2/baseband/base/__init__.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    72042 2022-12-20 23:09:23.000000 baseband-4.1.2/baseband/base/base.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     5359 2020-12-14 22:27:09.000000 baseband-4.1.2/baseband/base/encoding.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    22583 2021-12-01 18:28:57.000000 baseband-4.1.2/baseband/base/file_info.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     8072 2020-12-14 22:27:09.000000 baseband-4.1.2/baseband/base/frame.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    22862 2022-12-20 23:20:16.000000 baseband-4.1.2/baseband/base/header.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     4704 2021-12-02 18:32:59.000000 baseband-4.1.2/baseband/base/offsets.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    13670 2022-12-20 23:23:34.000000 baseband-4.1.2/baseband/base/payload.py
-drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2022-12-20 23:32:22.499202 baseband-4.1.2/baseband/base/tests/
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)        0 2020-12-14 22:27:09.000000 baseband-4.1.2/baseband/base/tests/__init__.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    29684 2022-12-20 23:23:53.000000 baseband-4.1.2/baseband/base/tests/test_base.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     1782 2020-12-14 22:27:09.000000 baseband-4.1.2/baseband/base/tests/test_file_info.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     3566 2020-12-14 22:27:09.000000 baseband-4.1.2/baseband/base/tests/test_header_parser.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     2296 2021-12-02 18:32:59.000000 baseband-4.1.2/baseband/base/tests/test_offsets.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     7066 2020-12-14 22:27:09.000000 baseband-4.1.2/baseband/base/tests/test_opener.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     4429 2022-12-20 23:23:53.000000 baseband-4.1.2/baseband/base/tests/test_utils.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     8373 2022-12-20 23:09:23.000000 baseband-4.1.2/baseband/base/utils.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     1758 2020-12-14 22:27:09.000000 baseband-4.1.2/baseband/conftest.py
-drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2022-12-20 23:32:22.499202 baseband-4.1.2/baseband/dada/
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)      299 2020-12-14 22:27:09.000000 baseband-4.1.2/baseband/dada/__init__.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    18464 2020-12-14 22:27:09.000000 baseband-4.1.2/baseband/dada/base.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     1825 2020-12-14 22:27:09.000000 baseband-4.1.2/baseband/dada/frame.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    16148 2022-12-20 23:20:16.000000 baseband-4.1.2/baseband/dada/header.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     1307 2020-12-14 22:27:09.000000 baseband-4.1.2/baseband/dada/payload.py
-drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2022-12-20 23:32:22.499202 baseband-4.1.2/baseband/dada/tests/
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)        0 2020-06-25 18:31:10.000000 baseband-4.1.2/baseband/dada/tests/__init__.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    35054 2022-12-20 23:23:53.000000 baseband-4.1.2/baseband/dada/tests/test_dada.py
-drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2022-12-20 23:32:22.503202 baseband-4.1.2/baseband/data/
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)      257 2020-06-25 18:34:28.000000 baseband-4.1.2/baseband/data/README.rst
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     5662 2022-12-20 23:19:03.000000 baseband-4.1.2/baseband/data/__init__.py
-drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2022-12-20 23:32:22.503202 baseband-4.1.2/baseband/data/gsb/
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)        0 2020-07-14 20:59:29.000000 baseband-4.1.2/baseband/data/gsb/__init__.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    40960 2020-07-14 20:59:29.000000 baseband-4.1.2/baseband/data/gsb/sample_gsb_phased.Pol-L1.dat
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    40960 2020-07-14 20:59:29.000000 baseband-4.1.2/baseband/data/gsb/sample_gsb_phased.Pol-L2.dat
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    40960 2020-07-14 20:59:29.000000 baseband-4.1.2/baseband/data/gsb/sample_gsb_phased.Pol-R1.dat
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    40960 2020-07-14 20:59:29.000000 baseband-4.1.2/baseband/data/gsb/sample_gsb_phased.Pol-R2.dat
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)      694 2020-07-14 20:59:29.000000 baseband-4.1.2/baseband/data/gsb/sample_gsb_phased.timestamp
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    40960 2020-07-14 20:59:29.000000 baseband-4.1.2/baseband/data/gsb/sample_gsb_rawdump.dat
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)      329 2020-07-14 20:59:29.000000 baseband-4.1.2/baseband/data/gsb/sample_gsb_rawdump.timestamp
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    68096 2020-06-19 20:13:31.000000 baseband-4.1.2/baseband/data/sample.dada
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)   384000 2018-07-05 15:53:52.000000 baseband-4.1.2/baseband/data/sample.m4
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    40064 2018-07-05 15:53:52.000000 baseband-4.1.2/baseband/data/sample.m5b
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    80512 2020-07-14 20:59:29.000000 baseband-4.1.2/baseband/data/sample.vdif
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)   102124 2020-07-14 20:59:29.000000 baseband-4.1.2/baseband/data/sample_16track.m4
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)   170000 2019-11-28 14:05:22.000000 baseband-4.1.2/baseband/data/sample_32track.m4
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)   180000 2020-07-14 20:59:29.000000 baseband-4.1.2/baseband/data/sample_32track_fanout2.m4
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)   327680 2020-12-14 22:27:09.000000 baseband-4.1.2/baseband/data/sample_64track_fanout2_ft.m4
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    10560 2018-07-05 15:53:52.000000 baseband-4.1.2/baseband/data/sample_arochime.vdif
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    16064 2020-12-14 22:27:09.000000 baseband-4.1.2/baseband/data/sample_bps1.vdif
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    50320 2020-07-14 20:59:29.000000 baseband-4.1.2/baseband/data/sample_drao_corrupted.vdif
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    32768 2022-12-20 23:19:03.000000 baseband-4.1.2/baseband/data/sample_meerkat.dada
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     5440 2018-07-05 15:53:52.000000 baseband-4.1.2/baseband/data/sample_mwa.vdif
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    91136 2020-12-14 22:27:09.000000 baseband-4.1.2/baseband/data/sample_puppi.raw
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    80512 2020-07-14 20:59:29.000000 baseband-4.1.2/baseband/data/sample_vlbi.vdif
-drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2022-12-20 23:32:22.503202 baseband-4.1.2/baseband/gsb/
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)      315 2020-12-14 22:27:09.000000 baseband-4.1.2/baseband/gsb/__init__.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    25864 2020-12-15 17:58:53.000000 baseband-4.1.2/baseband/gsb/base.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     7134 2020-12-14 22:27:09.000000 baseband-4.1.2/baseband/gsb/file_info.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     5671 2020-12-14 22:27:09.000000 baseband-4.1.2/baseband/gsb/frame.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    12136 2020-12-14 22:27:09.000000 baseband-4.1.2/baseband/gsb/header.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     5147 2020-12-14 22:27:09.000000 baseband-4.1.2/baseband/gsb/payload.py
-drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2022-12-20 23:32:22.507202 baseband-4.1.2/baseband/gsb/tests/
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)        0 2020-06-25 18:31:10.000000 baseband-4.1.2/baseband/gsb/tests/__init__.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    52111 2022-12-20 23:23:53.000000 baseband-4.1.2/baseband/gsb/tests/test_gsb.py
-drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2022-12-20 23:32:22.507202 baseband-4.1.2/baseband/guppi/
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)      308 2020-12-14 22:27:09.000000 baseband-4.1.2/baseband/guppi/__init__.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    15724 2020-12-14 22:27:09.000000 baseband-4.1.2/baseband/guppi/base.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     1266 2020-12-14 22:27:09.000000 baseband-4.1.2/baseband/guppi/file_info.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     1841 2020-12-14 22:27:09.000000 baseband-4.1.2/baseband/guppi/frame.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    14236 2022-12-20 23:20:16.000000 baseband-4.1.2/baseband/guppi/header.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     8160 2020-12-14 22:27:09.000000 baseband-4.1.2/baseband/guppi/payload.py
-drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2022-12-20 23:32:22.507202 baseband-4.1.2/baseband/guppi/tests/
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)        0 2020-12-14 22:27:09.000000 baseband-4.1.2/baseband/guppi/tests/__init__.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    36319 2022-12-20 23:23:53.000000 baseband-4.1.2/baseband/guppi/tests/test_guppi.py
-drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2022-12-20 23:32:22.507202 baseband-4.1.2/baseband/helpers/
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)        0 2020-07-14 20:59:29.000000 baseband-4.1.2/baseband/helpers/__init__.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    15050 2020-12-14 22:27:09.000000 baseband-4.1.2/baseband/helpers/sequentialfile.py
-drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2022-12-20 23:32:22.507202 baseband-4.1.2/baseband/helpers/tests/
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)        0 2020-07-14 20:59:29.000000 baseband-4.1.2/baseband/helpers/tests/__init__.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    13512 2022-12-20 23:23:53.000000 baseband-4.1.2/baseband/helpers/tests/test_sequentialfile.py
-drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2022-12-20 23:32:22.507202 baseband-4.1.2/baseband/io/
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     9485 2022-12-20 23:20:16.000000 baseband-4.1.2/baseband/io/__init__.py
-drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2022-12-20 23:32:22.507202 baseband-4.1.2/baseband/mark4/
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)      425 2022-12-20 23:19:55.000000 baseband-4.1.2/baseband/mark4/__init__.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    17351 2021-12-02 18:32:59.000000 baseband-4.1.2/baseband/mark4/base.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     4324 2020-12-14 22:27:09.000000 baseband-4.1.2/baseband/mark4/file_info.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    10992 2020-12-14 22:27:09.000000 baseband-4.1.2/baseband/mark4/frame.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    31255 2022-12-20 23:20:16.000000 baseband-4.1.2/baseband/mark4/header.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    18271 2020-12-14 22:27:09.000000 baseband-4.1.2/baseband/mark4/payload.py
-drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2022-12-20 23:32:22.507202 baseband-4.1.2/baseband/mark4/tests/
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)        0 2020-06-25 18:31:10.000000 baseband-4.1.2/baseband/mark4/tests/__init__.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     6806 2020-12-14 22:27:09.000000 baseband-4.1.2/baseband/mark4/tests/test_corrupt_files.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    56921 2021-12-02 18:32:59.000000 baseband-4.1.2/baseband/mark4/tests/test_mark4.py
-drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2022-12-20 23:32:22.507202 baseband-4.1.2/baseband/mark5b/
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)      422 2022-12-20 23:19:55.000000 baseband-4.1.2/baseband/mark5b/__init__.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    17900 2021-12-02 18:32:59.000000 baseband-4.1.2/baseband/mark5b/base.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     2905 2021-12-02 18:32:59.000000 baseband-4.1.2/baseband/mark5b/file_info.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     5051 2020-12-14 22:27:09.000000 baseband-4.1.2/baseband/mark5b/frame.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    11962 2022-12-20 23:09:33.000000 baseband-4.1.2/baseband/mark5b/header.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     4349 2020-12-14 22:27:09.000000 baseband-4.1.2/baseband/mark5b/payload.py
-drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2022-12-20 23:32:22.511203 baseband-4.1.2/baseband/mark5b/tests/
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)        0 2020-06-25 18:31:10.000000 baseband-4.1.2/baseband/mark5b/tests/__init__.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    12417 2022-12-20 23:23:53.000000 baseband-4.1.2/baseband/mark5b/tests/test_corrupt_files.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    41332 2022-12-20 23:09:33.000000 baseband-4.1.2/baseband/mark5b/tests/test_mark5b.py
-drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2022-12-20 23:32:22.511203 baseband-4.1.2/baseband/tasks/
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     2653 2022-12-20 23:30:37.000000 baseband-4.1.2/baseband/tasks/__init__.py
-drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2022-12-20 23:32:22.511203 baseband-4.1.2/baseband/tests/
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)       94 2020-12-14 22:27:09.000000 baseband-4.1.2/baseband/tests/__init__.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    19399 2020-12-14 22:27:09.000000 baseband-4.1.2/baseband/tests/test_conversion.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     5228 2021-12-02 17:13:38.000000 baseband-4.1.2/baseband/tests/test_core.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     6177 2022-12-20 23:30:37.000000 baseband-4.1.2/baseband/tests/test_entry_points.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     7445 2021-12-02 18:32:59.000000 baseband-4.1.2/baseband/tests/test_file_info.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     1792 2020-12-14 22:27:09.000000 baseband-4.1.2/baseband/tests/test_sequential_baseband.py
-drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2022-12-20 23:32:22.511203 baseband-4.1.2/baseband/vdif/
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)      537 2020-12-14 22:27:09.000000 baseband-4.1.2/baseband/vdif/__init__.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    37822 2022-12-20 23:11:32.000000 baseband-4.1.2/baseband/vdif/base.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     1863 2020-12-14 22:27:09.000000 baseband-4.1.2/baseband/vdif/file_info.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    19352 2022-12-20 23:11:28.000000 baseband-4.1.2/baseband/vdif/frame.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    33714 2022-12-20 23:11:28.000000 baseband-4.1.2/baseband/vdif/header.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     6695 2020-12-14 22:27:09.000000 baseband-4.1.2/baseband/vdif/payload.py
-drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2022-12-20 23:32:22.511203 baseband-4.1.2/baseband/vdif/tests/
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)        0 2020-06-25 18:31:10.000000 baseband-4.1.2/baseband/vdif/tests/__init__.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    14558 2020-12-14 22:27:09.000000 baseband-4.1.2/baseband/vdif/tests/test_corrupt_files.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    73706 2022-12-20 23:11:28.000000 baseband-4.1.2/baseband/vdif/tests/test_vdif.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)      337 2022-12-20 23:32:22.000000 baseband-4.1.2/baseband/version.py
-drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2022-12-20 23:32:22.495201 baseband-4.1.2/baseband.egg-info/
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     2551 2022-12-20 23:32:22.000000 baseband-4.1.2/baseband.egg-info/PKG-INFO
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     4545 2022-12-20 23:32:22.000000 baseband-4.1.2/baseband.egg-info/SOURCES.txt
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)        1 2022-12-20 23:32:22.000000 baseband-4.1.2/baseband.egg-info/dependency_links.txt
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)      146 2022-12-20 23:32:22.000000 baseband-4.1.2/baseband.egg-info/entry_points.txt
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)        1 2022-12-20 23:32:22.000000 baseband-4.1.2/baseband.egg-info/not-zip-safe
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)      205 2022-12-20 23:32:22.000000 baseband-4.1.2/baseband.egg-info/requires.txt
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)        9 2022-12-20 23:32:22.000000 baseband-4.1.2/baseband.egg-info/top_level.txt
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)       13 2020-12-14 22:27:09.000000 baseband-4.1.2/codecov.yml
-drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2022-12-20 23:32:22.511203 baseband-4.1.2/docs/
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     4581 2018-07-05 15:53:52.000000 baseband-4.1.2/docs/Makefile
-drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2022-12-20 23:32:22.491201 baseband-4.1.2/docs/_templates/
-drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2022-12-20 23:32:22.511203 baseband-4.1.2/docs/_templates/autosummary/
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)      250 2020-06-25 18:34:35.000000 baseband-4.1.2/docs/_templates/autosummary/base.rst
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)      251 2020-06-25 18:34:35.000000 baseband-4.1.2/docs/_templates/autosummary/class.rst
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)      252 2020-06-25 18:34:35.000000 baseband-4.1.2/docs/_templates/autosummary/module.rst
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)       47 2020-12-14 22:27:09.000000 baseband-4.1.2/docs/authors_for_sphinx.rst
-drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2022-12-20 23:32:22.511203 baseband-4.1.2/docs/base/
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)      494 2020-12-14 22:27:09.000000 baseband-4.1.2/docs/base/index.rst
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)       89 2020-12-14 22:27:09.000000 baseband-4.1.2/docs/changelog.rst
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     7827 2020-12-14 22:27:09.000000 baseband-4.1.2/docs/conf.py
-drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2022-12-20 23:32:22.515203 baseband-4.1.2/docs/dada/
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     2793 2020-12-14 22:27:09.000000 baseband-4.1.2/docs/dada/header.rst
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     4110 2020-12-14 22:27:09.000000 baseband-4.1.2/docs/dada/index.rst
-drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2022-12-20 23:32:22.515203 baseband-4.1.2/docs/data/
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)      121 2020-12-14 22:27:09.000000 baseband-4.1.2/docs/data/index.rst
-drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2022-12-20 23:32:22.515203 baseband-4.1.2/docs/gsb/
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    12046 2022-12-20 23:09:23.000000 baseband-4.1.2/docs/gsb/index.rst
-drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2022-12-20 23:32:22.515203 baseband-4.1.2/docs/guppi/
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     6515 2020-12-14 22:27:09.000000 baseband-4.1.2/docs/guppi/index.rst
-drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2022-12-20 23:32:22.515203 baseband-4.1.2/docs/helpers/
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     3365 2020-12-14 22:27:09.000000 baseband-4.1.2/docs/helpers/index.rst
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     3486 2022-12-20 23:09:19.000000 baseband-4.1.2/docs/index.rst
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     3596 2020-12-15 17:58:53.000000 baseband-4.1.2/docs/install.rst
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)      281 2020-12-14 22:27:09.000000 baseband-4.1.2/docs/license.rst
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     4549 2020-12-14 22:27:09.000000 baseband-4.1.2/docs/make.bat
-drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2022-12-20 23:32:22.515203 baseband-4.1.2/docs/mark4/
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     7291 2020-12-14 22:27:09.000000 baseband-4.1.2/docs/mark4/index.rst
-drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2022-12-20 23:32:22.515203 baseband-4.1.2/docs/mark5b/
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     4703 2020-12-14 22:27:09.000000 baseband-4.1.2/docs/mark5b/index.rst
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     1066 2020-12-14 22:27:09.000000 baseband-4.1.2/docs/nitpick-exceptions
-drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2022-12-20 23:32:22.515203 baseband-4.1.2/docs/tutorials/
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    99173 2020-12-14 22:27:09.000000 baseband-4.1.2/docs/tutorials/VDIFHeader.png
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     7149 2020-12-14 22:27:09.000000 baseband-4.1.2/docs/tutorials/getting_started.rst
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     2314 2020-12-14 22:27:09.000000 baseband-4.1.2/docs/tutorials/glossary.rst
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)      922 2020-12-14 22:27:09.000000 baseband-4.1.2/docs/tutorials/glossary_substitutions.rst
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    20795 2021-11-29 22:19:55.000000 baseband-4.1.2/docs/tutorials/new_edv.rst
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     1314 2022-12-20 23:09:19.000000 baseband-4.1.2/docs/tutorials/new_format.rst
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     1053 2020-12-15 18:34:29.000000 baseband-4.1.2/docs/tutorials/performance_tips.rst
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     9606 2021-11-29 22:19:55.000000 baseband-4.1.2/docs/tutorials/release_procedure.rst
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)    30494 2022-12-20 23:09:23.000000 baseband-4.1.2/docs/tutorials/using_baseband.rst
-drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2022-12-20 23:32:22.515203 baseband-4.1.2/docs/vdif/
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     8458 2021-11-29 22:19:55.000000 baseband-4.1.2/docs/vdif/index.rst
-drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2022-12-20 23:32:22.515203 baseband-4.1.2/licenses/
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)      405 2020-07-14 20:59:29.000000 baseband-4.1.2/licenses/README.rst
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)      134 2020-12-14 22:27:09.000000 baseband-4.1.2/pyproject.toml
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     2475 2022-12-20 23:32:22.515203 baseband-4.1.2/setup.cfg
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     2006 2020-12-14 22:27:09.000000 baseband-4.1.2/setup.py
--rw-r--r--   0 mhvk      (1000) mhvk      (1000)     2141 2022-12-20 23:30:51.000000 baseband-4.1.2/tox.ini
+drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2023-05-16 09:47:34.619050 baseband-4.1.3/
+drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2023-05-16 09:47:34.591050 baseband-4.1.3/.github/
+drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2023-05-16 09:47:34.595050 baseband-4.1.3/.github/workflows/
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     2398 2023-05-16 09:43:23.000000 baseband-4.1.3/.github/workflows/ci_cron_monthly.yml
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     2105 2023-05-16 09:45:05.000000 baseband-4.1.3/.github/workflows/ci_workflows.yml
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)      719 2023-05-16 09:33:25.000000 baseband-4.1.3/.gitignore
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)      170 2023-05-16 09:43:23.000000 baseband-4.1.3/.readthedocs.yml
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)      120 2023-05-16 09:33:25.000000 baseband-4.1.3/.rtd-environment.yml
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     1361 2023-05-16 09:45:38.000000 baseband-4.1.3/.zenodo.json
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     1116 2023-05-16 09:45:38.000000 baseband-4.1.3/AUTHORS.rst
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    14258 2023-05-16 09:45:54.000000 baseband-4.1.3/CHANGES.rst
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)       94 2020-07-14 20:59:29.000000 baseband-4.1.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)      196 2020-07-14 20:59:29.000000 baseband-4.1.3/CONTRIBUTING.md
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    35141 2020-07-14 20:59:29.000000 baseband-4.1.3/LICENSE
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)      346 2023-05-16 09:33:25.000000 baseband-4.1.3/MANIFEST.in
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     2551 2023-05-16 09:47:34.619050 baseband-4.1.3/PKG-INFO
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     2030 2023-05-16 09:33:25.000000 baseband-4.1.3/README.rst
+drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2023-05-16 09:47:34.595050 baseband-4.1.3/baseband/
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)      699 2023-05-16 09:43:23.000000 baseband-4.1.3/baseband/__init__.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)      613 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/_astropy_init.py
+drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2023-05-16 09:47:34.599050 baseband-4.1.3/baseband/base/
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     1065 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/base/__init__.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    72042 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/base/base.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     5359 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/base/encoding.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    22583 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/base/file_info.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     8072 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/base/frame.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    22862 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/base/header.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     4704 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/base/offsets.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    13670 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/base/payload.py
+drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2023-05-16 09:47:34.599050 baseband-4.1.3/baseband/base/tests/
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)        0 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/base/tests/__init__.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    29684 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/base/tests/test_base.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     1782 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/base/tests/test_file_info.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     3566 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/base/tests/test_header_parser.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     2296 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/base/tests/test_offsets.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     7066 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/base/tests/test_opener.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     4429 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/base/tests/test_utils.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     8373 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/base/utils.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     1758 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/conftest.py
+drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2023-05-16 09:47:34.599050 baseband-4.1.3/baseband/dada/
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)      299 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/dada/__init__.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    18464 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/dada/base.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     1825 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/dada/frame.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    16148 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/dada/header.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     1307 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/dada/payload.py
+drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2023-05-16 09:47:34.599050 baseband-4.1.3/baseband/dada/tests/
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)        0 2020-06-25 18:31:10.000000 baseband-4.1.3/baseband/dada/tests/__init__.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    35054 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/dada/tests/test_dada.py
+drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2023-05-16 09:47:34.603050 baseband-4.1.3/baseband/data/
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)      257 2020-06-25 18:34:28.000000 baseband-4.1.3/baseband/data/README.rst
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     5984 2023-05-16 09:45:18.000000 baseband-4.1.3/baseband/data/__init__.py
+drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2023-05-16 09:47:34.607050 baseband-4.1.3/baseband/data/gsb/
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)        0 2020-07-14 20:59:29.000000 baseband-4.1.3/baseband/data/gsb/__init__.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    40960 2020-07-14 20:59:29.000000 baseband-4.1.3/baseband/data/gsb/sample_gsb_phased.Pol-L1.dat
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    40960 2020-07-14 20:59:29.000000 baseband-4.1.3/baseband/data/gsb/sample_gsb_phased.Pol-L2.dat
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    40960 2020-07-14 20:59:29.000000 baseband-4.1.3/baseband/data/gsb/sample_gsb_phased.Pol-R1.dat
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    40960 2020-07-14 20:59:29.000000 baseband-4.1.3/baseband/data/gsb/sample_gsb_phased.Pol-R2.dat
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)      694 2020-07-14 20:59:29.000000 baseband-4.1.3/baseband/data/gsb/sample_gsb_phased.timestamp
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    40960 2020-07-14 20:59:29.000000 baseband-4.1.3/baseband/data/gsb/sample_gsb_rawdump.dat
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)      329 2020-07-14 20:59:29.000000 baseband-4.1.3/baseband/data/gsb/sample_gsb_rawdump.timestamp
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    68096 2020-06-19 20:13:31.000000 baseband-4.1.3/baseband/data/sample.dada
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)   384000 2018-07-05 15:53:52.000000 baseband-4.1.3/baseband/data/sample.m4
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    40064 2018-07-05 15:53:52.000000 baseband-4.1.3/baseband/data/sample.m5b
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    80512 2020-07-14 20:59:29.000000 baseband-4.1.3/baseband/data/sample.vdif
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)   102124 2020-07-14 20:59:29.000000 baseband-4.1.3/baseband/data/sample_16track.m4
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)   170000 2019-11-28 14:05:22.000000 baseband-4.1.3/baseband/data/sample_32track.m4
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)   180000 2020-07-14 20:59:29.000000 baseband-4.1.3/baseband/data/sample_32track_fanout2.m4
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)   327680 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/data/sample_64track_fanout2_ft.m4
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    10560 2018-07-05 15:53:52.000000 baseband-4.1.3/baseband/data/sample_arochime.vdif
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    16064 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/data/sample_bps1.vdif
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    50320 2020-07-14 20:59:29.000000 baseband-4.1.3/baseband/data/sample_drao_corrupted.vdif
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    32768 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/data/sample_meerkat.dada
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     5440 2018-07-05 15:53:52.000000 baseband-4.1.3/baseband/data/sample_mwa.vdif
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    91136 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/data/sample_puppi.raw
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    14240 2023-05-16 09:45:18.000000 baseband-4.1.3/baseband/data/sample_vegas.raw
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    80512 2020-07-14 20:59:29.000000 baseband-4.1.3/baseband/data/sample_vlbi.vdif
+drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2023-05-16 09:47:34.607050 baseband-4.1.3/baseband/gsb/
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)      315 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/gsb/__init__.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    25864 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/gsb/base.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     7134 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/gsb/file_info.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     5671 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/gsb/frame.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    12136 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/gsb/header.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     5147 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/gsb/payload.py
+drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2023-05-16 09:47:34.607050 baseband-4.1.3/baseband/gsb/tests/
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)        0 2020-06-25 18:31:10.000000 baseband-4.1.3/baseband/gsb/tests/__init__.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    52111 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/gsb/tests/test_gsb.py
+drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2023-05-16 09:47:34.607050 baseband-4.1.3/baseband/guppi/
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)      308 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/guppi/__init__.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    15724 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/guppi/base.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     1266 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/guppi/file_info.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     1841 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/guppi/frame.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    14339 2023-05-16 09:45:18.000000 baseband-4.1.3/baseband/guppi/header.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     8160 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/guppi/payload.py
+drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2023-05-16 09:47:34.607050 baseband-4.1.3/baseband/guppi/tests/
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)        0 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/guppi/tests/__init__.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    36795 2023-05-16 09:45:18.000000 baseband-4.1.3/baseband/guppi/tests/test_guppi.py
+drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2023-05-16 09:47:34.607050 baseband-4.1.3/baseband/helpers/
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)        0 2020-07-14 20:59:29.000000 baseband-4.1.3/baseband/helpers/__init__.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    15050 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/helpers/sequentialfile.py
+drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2023-05-16 09:47:34.607050 baseband-4.1.3/baseband/helpers/tests/
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)        0 2020-07-14 20:59:29.000000 baseband-4.1.3/baseband/helpers/tests/__init__.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    13512 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/helpers/tests/test_sequentialfile.py
+drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2023-05-16 09:47:34.607050 baseband-4.1.3/baseband/io/
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     9485 2023-05-16 09:43:23.000000 baseband-4.1.3/baseband/io/__init__.py
+drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2023-05-16 09:47:34.611050 baseband-4.1.3/baseband/mark4/
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)      425 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/mark4/__init__.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    17351 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/mark4/base.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     4324 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/mark4/file_info.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    10992 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/mark4/frame.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    31255 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/mark4/header.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    18271 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/mark4/payload.py
+drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2023-05-16 09:47:34.611050 baseband-4.1.3/baseband/mark4/tests/
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)        0 2020-06-25 18:31:10.000000 baseband-4.1.3/baseband/mark4/tests/__init__.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     6806 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/mark4/tests/test_corrupt_files.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    56921 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/mark4/tests/test_mark4.py
+drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2023-05-16 09:47:34.611050 baseband-4.1.3/baseband/mark5b/
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)      422 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/mark5b/__init__.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    17900 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/mark5b/base.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     2905 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/mark5b/file_info.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     5051 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/mark5b/frame.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    11962 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/mark5b/header.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     4349 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/mark5b/payload.py
+drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2023-05-16 09:47:34.611050 baseband-4.1.3/baseband/mark5b/tests/
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)        0 2020-06-25 18:31:10.000000 baseband-4.1.3/baseband/mark5b/tests/__init__.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    12417 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/mark5b/tests/test_corrupt_files.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    41332 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/mark5b/tests/test_mark5b.py
+drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2023-05-16 09:47:34.611050 baseband-4.1.3/baseband/tasks/
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     2653 2023-05-16 09:43:23.000000 baseband-4.1.3/baseband/tasks/__init__.py
+drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2023-05-16 09:47:34.611050 baseband-4.1.3/baseband/tests/
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)       94 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/tests/__init__.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    19399 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/tests/test_conversion.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     5228 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/tests/test_core.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     6177 2023-05-16 09:43:23.000000 baseband-4.1.3/baseband/tests/test_entry_points.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     7445 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/tests/test_file_info.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     1792 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/tests/test_sequential_baseband.py
+drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2023-05-16 09:47:34.615050 baseband-4.1.3/baseband/vdif/
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)      537 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/vdif/__init__.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    37822 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/vdif/base.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     1863 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/vdif/file_info.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    19352 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/vdif/frame.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    33714 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/vdif/header.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     6695 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/vdif/payload.py
+drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2023-05-16 09:47:34.615050 baseband-4.1.3/baseband/vdif/tests/
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)        0 2020-06-25 18:31:10.000000 baseband-4.1.3/baseband/vdif/tests/__init__.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    14558 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/vdif/tests/test_corrupt_files.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    73706 2023-05-16 09:33:25.000000 baseband-4.1.3/baseband/vdif/tests/test_vdif.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)      337 2023-05-16 09:47:34.000000 baseband-4.1.3/baseband/version.py
+drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2023-05-16 09:47:34.599050 baseband-4.1.3/baseband.egg-info/
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     2551 2023-05-16 09:47:34.000000 baseband-4.1.3/baseband.egg-info/PKG-INFO
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     4576 2023-05-16 09:47:34.000000 baseband-4.1.3/baseband.egg-info/SOURCES.txt
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)        1 2023-05-16 09:47:34.000000 baseband-4.1.3/baseband.egg-info/dependency_links.txt
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)      146 2023-05-16 09:47:34.000000 baseband-4.1.3/baseband.egg-info/entry_points.txt
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)        1 2023-05-16 09:47:34.000000 baseband-4.1.3/baseband.egg-info/not-zip-safe
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)      188 2023-05-16 09:47:34.000000 baseband-4.1.3/baseband.egg-info/requires.txt
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)        9 2023-05-16 09:47:34.000000 baseband-4.1.3/baseband.egg-info/top_level.txt
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)       13 2023-05-16 09:33:25.000000 baseband-4.1.3/codecov.yml
+drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2023-05-16 09:47:34.615050 baseband-4.1.3/docs/
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     4581 2018-07-05 15:53:52.000000 baseband-4.1.3/docs/Makefile
+drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2023-05-16 09:47:34.591050 baseband-4.1.3/docs/_templates/
+drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2023-05-16 09:47:34.615050 baseband-4.1.3/docs/_templates/autosummary/
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)      250 2020-06-25 18:34:35.000000 baseband-4.1.3/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)      251 2020-06-25 18:34:35.000000 baseband-4.1.3/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)      252 2020-06-25 18:34:35.000000 baseband-4.1.3/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)       47 2023-05-16 09:33:25.000000 baseband-4.1.3/docs/authors_for_sphinx.rst
+drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2023-05-16 09:47:34.615050 baseband-4.1.3/docs/base/
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)      494 2023-05-16 09:33:25.000000 baseband-4.1.3/docs/base/index.rst
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)       89 2023-05-16 09:33:25.000000 baseband-4.1.3/docs/changelog.rst
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     7827 2023-05-16 09:33:25.000000 baseband-4.1.3/docs/conf.py
+drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2023-05-16 09:47:34.615050 baseband-4.1.3/docs/dada/
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     2793 2023-05-16 09:33:25.000000 baseband-4.1.3/docs/dada/header.rst
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     4110 2023-05-16 09:33:25.000000 baseband-4.1.3/docs/dada/index.rst
+drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2023-05-16 09:47:34.615050 baseband-4.1.3/docs/data/
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)      121 2023-05-16 09:33:25.000000 baseband-4.1.3/docs/data/index.rst
+drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2023-05-16 09:47:34.615050 baseband-4.1.3/docs/gsb/
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    12046 2023-05-16 09:33:25.000000 baseband-4.1.3/docs/gsb/index.rst
+drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2023-05-16 09:47:34.615050 baseband-4.1.3/docs/guppi/
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     6515 2023-05-16 09:33:25.000000 baseband-4.1.3/docs/guppi/index.rst
+drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2023-05-16 09:47:34.615050 baseband-4.1.3/docs/helpers/
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     3365 2023-05-16 09:33:25.000000 baseband-4.1.3/docs/helpers/index.rst
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     3486 2023-05-16 09:33:25.000000 baseband-4.1.3/docs/index.rst
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     3596 2023-05-16 09:33:25.000000 baseband-4.1.3/docs/install.rst
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)      281 2023-05-16 09:33:25.000000 baseband-4.1.3/docs/license.rst
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     4549 2023-05-16 09:33:25.000000 baseband-4.1.3/docs/make.bat
+drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2023-05-16 09:47:34.615050 baseband-4.1.3/docs/mark4/
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     7291 2023-05-16 09:33:25.000000 baseband-4.1.3/docs/mark4/index.rst
+drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2023-05-16 09:47:34.615050 baseband-4.1.3/docs/mark5b/
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     4703 2023-05-16 09:33:25.000000 baseband-4.1.3/docs/mark5b/index.rst
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     1066 2023-05-16 09:33:25.000000 baseband-4.1.3/docs/nitpick-exceptions
+drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2023-05-16 09:47:34.619050 baseband-4.1.3/docs/tutorials/
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    99173 2023-05-16 09:33:25.000000 baseband-4.1.3/docs/tutorials/VDIFHeader.png
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     7149 2023-05-16 09:33:25.000000 baseband-4.1.3/docs/tutorials/getting_started.rst
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     2314 2023-05-16 09:33:25.000000 baseband-4.1.3/docs/tutorials/glossary.rst
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)      922 2023-05-16 09:33:25.000000 baseband-4.1.3/docs/tutorials/glossary_substitutions.rst
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    20795 2023-05-16 09:33:25.000000 baseband-4.1.3/docs/tutorials/new_edv.rst
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     1314 2023-05-16 09:33:25.000000 baseband-4.1.3/docs/tutorials/new_format.rst
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     1053 2023-05-16 09:33:25.000000 baseband-4.1.3/docs/tutorials/performance_tips.rst
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     9606 2023-05-16 09:33:25.000000 baseband-4.1.3/docs/tutorials/release_procedure.rst
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)    30494 2023-05-16 09:33:25.000000 baseband-4.1.3/docs/tutorials/using_baseband.rst
+drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2023-05-16 09:47:34.619050 baseband-4.1.3/docs/vdif/
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     8458 2023-05-16 09:33:25.000000 baseband-4.1.3/docs/vdif/index.rst
+drwxr-xr-x   0 mhvk      (1000) mhvk      (1000)        0 2023-05-16 09:47:34.619050 baseband-4.1.3/licenses/
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)      405 2020-07-14 20:59:29.000000 baseband-4.1.3/licenses/README.rst
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)      134 2023-05-16 09:33:25.000000 baseband-4.1.3/pyproject.toml
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     2457 2023-05-16 09:47:34.619050 baseband-4.1.3/setup.cfg
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     2006 2023-05-16 09:33:25.000000 baseband-4.1.3/setup.py
+-rw-r--r--   0 mhvk      (1000) mhvk      (1000)     2141 2023-05-16 09:44:48.000000 baseband-4.1.3/tox.ini
```

### Comparing `baseband-4.1.2/.github/workflows/ci_cron_monthly.yml` & `baseband-4.1.3/.github/workflows/ci_cron_monthly.yml`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/.github/workflows/ci_workflows.yml` & `baseband-4.1.3/.github/workflows/ci_workflows.yml`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
       fail-fast: true
       matrix:
         include:
 
           - name: Test basics and coverage on 3.10
             python: "3.10"
             toxenv: py310-test-cov
-            toxposargs: --open-files
 
           - name: Code style checks
             python: "3.x"
             toxenv: codestyle
 
     steps:
     - uses: actions/checkout@v3
```

### Comparing `baseband-4.1.2/.gitignore` & `baseband-4.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/.zenodo.json` & `baseband-4.1.3/.zenodo.json`

 * *Files 9% similar despite different names*

```diff
@@ -31,48 +31,56 @@
 000001e0: 6974 7920 6f66 2054 6f72 6f6e 746f 222c  ity of Toronto",
 000001f0: 0a20 2020 2020 2020 2020 2020 2022 6e61  .            "na
 00000200: 6d65 223a 2022 5265 6265 6363 6120 4c69  me": "Rebecca Li
 00000210: 6e22 0a20 2020 2020 2020 207d 2c0a 2020  n".        },.  
 00000220: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
 00000230: 2020 2020 2261 6666 696c 6961 7469 6f6e      "affiliation
 00000240: 223a 2022 556e 6976 6572 7369 7479 206f  ": "University o
-00000250: 6620 546f 726f 6e74 6f22 2c0a 2020 2020  f Toronto",.    
-00000260: 2020 2020 2020 2020 226e 616d 6522 3a20          "name": 
-00000270: 224e 696b 6869 6c20 4d61 6861 6a61 6e22  "Nikhil Mahajan"
-00000280: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
-00000290: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
-000002a0: 2020 2261 6666 696c 6961 7469 6f6e 223a    "affiliation":
-000002b0: 2022 4475 626c 696e 2049 6e73 7469 7475   "Dublin Institu
-000002c0: 7465 2066 6f72 2041 6476 616e 6365 6420  te for Advanced 
-000002d0: 5374 7564 6965 7322 2c0a 2020 2020 2020  Studies",.      
-000002e0: 2020 2020 2020 226e 616d 6522 3a20 2244        "name": "D
-000002f0: 6176 6964 204d 634b 656e 6e61 220a 2020  avid McKenna".  
-00000300: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00000310: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
-00000320: 6166 6669 6c69 6174 696f 6e22 3a20 224d  affiliation": "M
-00000330: 6178 2d50 6c61 6e6b 2d49 6e73 7469 7475  ax-Plank-Institu
-00000340: 7420 665c 7530 3066 6372 2052 6164 696f  t f\u00fcr Radio
-00000350: 6173 7472 6f6e 6f6d 6965 222c 0a20 2020  astronomie",.   
-00000360: 2020 2020 2020 2020 2022 6e61 6d65 223a           "name":
-00000370: 2022 526f 6265 7274 204d 6169 6e22 0a20   "Robert Main". 
-00000380: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-00000390: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
-000003a0: 2261 6666 696c 6961 7469 6f6e 223a 2022  "affiliation": "
-000003b0: 4361 6c69 666f 726e 6961 2049 6e73 7469  California Insti
-000003c0: 7475 7465 206f 6620 5465 6368 6e6f 6c6f  tute of Technolo
-000003d0: 6779 222c 0a20 2020 2020 2020 2020 2020  gy",.           
-000003e0: 2022 6e61 6d65 223a 2022 4461 6e61 2053   "name": "Dana S
-000003f0: 696d 6172 6422 0a20 2020 2020 2020 207d  imard".        }
-00000400: 2c0a 2020 2020 2020 2020 7b0a 2020 2020  ,.        {.    
-00000410: 2020 2020 2020 2020 2261 6666 696c 6961          "affilia
-00000420: 7469 6f6e 223a 2022 5543 2042 6572 6b65  tion": "UC Berke
-00000430: 6c65 7922 2c0a 2020 2020 2020 2020 2020  ley",.          
-00000440: 2020 226e 616d 6522 3a20 2247 656f 7267    "name": "Georg
-00000450: 6520 5374 6569 6e22 0a20 2020 2020 2020  e Stein".       
-00000460: 207d 2c0a 2020 2020 2020 2020 7b0a 2020   },.        {.  
-00000470: 2020 2020 2020 2020 2020 2261 6666 696c            "affil
-00000480: 6961 7469 6f6e 223a 2022 556e 6976 6572  iation": "Univer
-00000490: 7369 7479 206f 6620 546f 726f 6e74 6f22  sity of Toronto"
-000004a0: 2c0a 2020 2020 2020 2020 2020 2020 226e  ,.            "n
-000004b0: 616d 6522 3a20 2252 696b 2076 616e 204c  ame": "Rik van L
-000004c0: 6965 7368 6f75 7422 0a20 2020 2020 2020  ieshout".       
-000004d0: 207d 0a20 2020 205d 0a7d 0a               }.    ].}.
+00000250: 6620 4361 6c69 666f 726e 6961 2061 7420  f California at 
+00000260: 4c6f 7320 416e 6765 6c65 7322 2c0a 2020  Los Angeles",.  
+00000270: 2020 2020 2020 2020 2020 226e 616d 6522            "name"
+00000280: 3a20 224a 6561 6e2d 4c75 6320 4d61 7267  : "Jean-Luc Marg
+00000290: 6f74 220a 2020 2020 2020 2020 7b0a 2020  ot".        {.  
+000002a0: 2020 2020 2020 2020 2020 2261 6666 696c            "affil
+000002b0: 6961 7469 6f6e 223a 2022 556e 6976 6572  iation": "Univer
+000002c0: 7369 7479 206f 6620 546f 726f 6e74 6f22  sity of Toronto"
+000002d0: 2c0a 2020 2020 2020 2020 2020 2020 226e  ,.            "n
+000002e0: 616d 6522 3a20 224e 696b 6869 6c20 4d61  ame": "Nikhil Ma
+000002f0: 6861 6a61 6e22 0a20 2020 2020 2020 207d  hajan".        }
+00000300: 2c0a 2020 2020 2020 2020 7b0a 2020 2020  ,.        {.    
+00000310: 2020 2020 2020 2020 2261 6666 696c 6961          "affilia
+00000320: 7469 6f6e 223a 2022 4475 626c 696e 2049  tion": "Dublin I
+00000330: 6e73 7469 7475 7465 2066 6f72 2041 6476  nstitute for Adv
+00000340: 616e 6365 6420 5374 7564 6965 7322 2c0a  anced Studies",.
+00000350: 2020 2020 2020 2020 2020 2020 226e 616d              "nam
+00000360: 6522 3a20 2244 6176 6964 204d 634b 656e  e": "David McKen
+00000370: 6e61 220a 2020 2020 2020 2020 7d2c 0a20  na".        },. 
+00000380: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+00000390: 2020 2020 2022 6166 6669 6c69 6174 696f       "affiliatio
+000003a0: 6e22 3a20 224d 6178 2d50 6c61 6e6b 2d49  n": "Max-Plank-I
+000003b0: 6e73 7469 7475 7420 665c 7530 3066 6372  nstitut f\u00fcr
+000003c0: 2052 6164 696f 6173 7472 6f6e 6f6d 6965   Radioastronomie
+000003d0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+000003e0: 6e61 6d65 223a 2022 526f 6265 7274 204d  name": "Robert M
+000003f0: 6169 6e22 0a20 2020 2020 2020 207d 2c0a  ain".        },.
+00000400: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+00000410: 2020 2020 2020 2261 6666 696c 6961 7469        "affiliati
+00000420: 6f6e 223a 2022 4361 6c69 666f 726e 6961  on": "California
+00000430: 2049 6e73 7469 7475 7465 206f 6620 5465   Institute of Te
+00000440: 6368 6e6f 6c6f 6779 222c 0a20 2020 2020  chnology",.     
+00000450: 2020 2020 2020 2022 6e61 6d65 223a 2022         "name": "
+00000460: 4461 6e61 2053 696d 6172 6422 0a20 2020  Dana Simard".   
+00000470: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00000480: 7b0a 2020 2020 2020 2020 2020 2020 2261  {.            "a
+00000490: 6666 696c 6961 7469 6f6e 223a 2022 5543  ffiliation": "UC
+000004a0: 2042 6572 6b65 6c65 7922 2c0a 2020 2020   Berkeley",.    
+000004b0: 2020 2020 2020 2020 226e 616d 6522 3a20          "name": 
+000004c0: 2247 656f 7267 6520 5374 6569 6e22 0a20  "George Stein". 
+000004d0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+000004e0: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
+000004f0: 2261 6666 696c 6961 7469 6f6e 223a 2022  "affiliation": "
+00000500: 556e 6976 6572 7369 7479 206f 6620 546f  University of To
+00000510: 726f 6e74 6f22 2c0a 2020 2020 2020 2020  ronto",.        
+00000520: 2020 2020 226e 616d 6522 3a20 2252 696b      "name": "Rik
+00000530: 2076 616e 204c 6965 7368 6f75 7422 0a20   van Lieshout". 
+00000540: 2020 2020 2020 207d 0a20 2020 205d 0a7d         }.    ].}
+00000550: 0a                                       .
```

### Comparing `baseband-4.1.2/AUTHORS.rst` & `baseband-4.1.3/AUTHORS.rst`

 * *Files 11% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 Other contributors (alphabetical)
 =================================
 
 * Shaoguang Guo (@shaoguangleo)
 * Rebecca Lin (@00rebe)
 * Nikhil Mahajan (@theXYZT)
 * Robert Main (@ramain)
+* Jean-Luc Margot (@jeanlucmargot)
 * David McKenna (@David-McKenna)
 * Dana Simard (@danasimard)
 * George Stein (@georgestein)
 * Rik van Lieshout (@rikvl)
 
 If you have contributed to Baseband but are not listed above, please send one
 of the authors an e-mail, or `open a pull request for this page
```

### Comparing `baseband-4.1.2/CHANGES.rst` & `baseband-4.1.3/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+4.1.3 (2023-05-16)
+==================
+
+Bug Fixes
+---------
+
+- GUPPI files written by the VEGAS backend, which, oddly, writes
+  numbers as strings with quotes around them, can now be read. [#515]
+
+
 4.1.2 (2022-12-20)
 ==================
 
 Bug Fixes
 ---------
 
 - DADA files such as those produced with Meerkat, in which the header ends
```

### Comparing `baseband-4.1.2/LICENSE` & `baseband-4.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/PKG-INFO` & `baseband-4.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baseband
-Version: 4.1.2
+Version: 4.1.3
 Summary: A package for radio baseband I/O
 Home-page: https://github.com/mhvk/baseband
 Author: Marten H. van Kerkwijk, Chenchong Zhu
 Author-email: mhvk@astro.utoronto.ca
 License: GNU GPL v3+
 Project-URL: Documentation, https://baseband.readthedocs.io
 Project-URL: Source, https://github.com/mhvk/baseband
```

### Comparing `baseband-4.1.2/README.rst` & `baseband-4.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/__init__.py` & `baseband-4.1.3/baseband/__init__.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/_astropy_init.py` & `baseband-4.1.3/baseband/_astropy_init.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/base/__init__.py` & `baseband-4.1.3/baseband/base/__init__.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/base/base.py` & `baseband-4.1.3/baseband/base/base.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/base/encoding.py` & `baseband-4.1.3/baseband/base/encoding.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/base/file_info.py` & `baseband-4.1.3/baseband/base/file_info.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/base/frame.py` & `baseband-4.1.3/baseband/base/frame.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/base/header.py` & `baseband-4.1.3/baseband/base/header.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/base/offsets.py` & `baseband-4.1.3/baseband/base/offsets.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/base/payload.py` & `baseband-4.1.3/baseband/base/payload.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/base/tests/test_base.py` & `baseband-4.1.3/baseband/base/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/base/tests/test_file_info.py` & `baseband-4.1.3/baseband/base/tests/test_file_info.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/base/tests/test_header_parser.py` & `baseband-4.1.3/baseband/base/tests/test_header_parser.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/base/tests/test_offsets.py` & `baseband-4.1.3/baseband/base/tests/test_offsets.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/base/tests/test_opener.py` & `baseband-4.1.3/baseband/base/tests/test_opener.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/base/tests/test_utils.py` & `baseband-4.1.3/baseband/base/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/base/utils.py` & `baseband-4.1.3/baseband/base/utils.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/conftest.py` & `baseband-4.1.3/baseband/conftest.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/dada/base.py` & `baseband-4.1.3/baseband/dada/base.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/dada/frame.py` & `baseband-4.1.3/baseband/dada/frame.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/dada/header.py` & `baseband-4.1.3/baseband/dada/header.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/dada/payload.py` & `baseband-4.1.3/baseband/dada/payload.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/dada/tests/test_dada.py` & `baseband-4.1.3/baseband/dada/tests/test_dada.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/data/__init__.py` & `baseband-4.1.3/baseband/data/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,14 +116,23 @@
 """GUPPI/PUPPI sample, npol=2, nchan=4.
 
 Created from the first four frames of a 2018-01-14 Arecibo observation of
 J1810+1744, with payload shortened to 8192 samples (with 512 overlap),
 equivalent to 1024 complete samples (with 64 overlap).
 """
 
+SAMPLE_VEGAS = _full_path('sample_vegas.raw')
+r"""VEGAS sample, npol=2, obsnchan=32.
+
+Created from a Green Bank Telescope observation of TOI 1898
+dd if=vegas_59332_80137_Jade_1898_1_0001.0000.raw \
+   of=sample_vegas.raw bs=80 count=178
+Initial frame is >50 MB and truncated.  For tests of header functionality only.
+"""
+
 SAMPLE_GSB_RAWDUMP_HEADER = _full_path('gsb/sample_gsb_rawdump.timestamp')
 """GSB rawdump header sample.
 
 First 10 header entries of node 5 rawdump data from 2015-04-27 GMRT
 observations of the Crab pulsar.
 """
```

### Comparing `baseband-4.1.2/baseband/data/gsb/sample_gsb_phased.Pol-L1.dat` & `baseband-4.1.3/baseband/data/gsb/sample_gsb_phased.Pol-L1.dat`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/data/gsb/sample_gsb_phased.Pol-L2.dat` & `baseband-4.1.3/baseband/data/gsb/sample_gsb_phased.Pol-L2.dat`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/data/gsb/sample_gsb_phased.Pol-R1.dat` & `baseband-4.1.3/baseband/data/gsb/sample_gsb_phased.Pol-R1.dat`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/data/gsb/sample_gsb_phased.Pol-R2.dat` & `baseband-4.1.3/baseband/data/gsb/sample_gsb_phased.Pol-R2.dat`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/data/gsb/sample_gsb_phased.timestamp` & `baseband-4.1.3/baseband/data/gsb/sample_gsb_phased.timestamp`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/data/gsb/sample_gsb_rawdump.dat` & `baseband-4.1.3/baseband/data/gsb/sample_gsb_rawdump.dat`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/data/sample.dada` & `baseband-4.1.3/baseband/data/sample.dada`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/data/sample.m4` & `baseband-4.1.3/baseband/data/sample.m4`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/data/sample.m5b` & `baseband-4.1.3/baseband/data/sample.m5b`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/data/sample.vdif` & `baseband-4.1.3/baseband/data/sample.vdif`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/data/sample_16track.m4` & `baseband-4.1.3/baseband/data/sample_16track.m4`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/data/sample_32track.m4` & `baseband-4.1.3/baseband/data/sample_32track.m4`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/data/sample_32track_fanout2.m4` & `baseband-4.1.3/baseband/data/sample_32track_fanout2.m4`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/data/sample_64track_fanout2_ft.m4` & `baseband-4.1.3/baseband/data/sample_64track_fanout2_ft.m4`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/data/sample_arochime.vdif` & `baseband-4.1.3/baseband/data/sample_arochime.vdif`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/data/sample_bps1.vdif` & `baseband-4.1.3/baseband/data/sample_bps1.vdif`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/data/sample_drao_corrupted.vdif` & `baseband-4.1.3/baseband/data/sample_drao_corrupted.vdif`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/data/sample_meerkat.dada` & `baseband-4.1.3/baseband/data/sample_meerkat.dada`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/data/sample_mwa.vdif` & `baseband-4.1.3/baseband/data/sample_mwa.vdif`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/data/sample_puppi.raw` & `baseband-4.1.3/baseband/data/sample_puppi.raw`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/data/sample_vlbi.vdif` & `baseband-4.1.3/baseband/data/sample_vlbi.vdif`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/gsb/base.py` & `baseband-4.1.3/baseband/gsb/base.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/gsb/file_info.py` & `baseband-4.1.3/baseband/gsb/file_info.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/gsb/frame.py` & `baseband-4.1.3/baseband/gsb/frame.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/gsb/header.py` & `baseband-4.1.3/baseband/gsb/header.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/gsb/payload.py` & `baseband-4.1.3/baseband/gsb/payload.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/gsb/tests/test_gsb.py` & `baseband-4.1.3/baseband/gsb/tests/test_gsb.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/guppi/base.py` & `baseband-4.1.3/baseband/guppi/base.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/guppi/file_info.py` & `baseband-4.1.3/baseband/guppi/file_info.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/guppi/frame.py` & `baseband-4.1.3/baseband/guppi/frame.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/guppi/header.py` & `baseband-4.1.3/baseband/guppi/header.py`

 * *Files 9% similar despite different names*

```diff
@@ -211,15 +211,15 @@
     def nbytes(self):
         """Size of the header in bytes."""
         return (len(self) + 1) * 80
 
     @property
     def payload_nbytes(self):
         """Size of the payload in bytes."""
-        return self['BLOCSIZE']
+        return int(self['BLOCSIZE'])
 
     @payload_nbytes.setter
     def payload_nbytes(self, payloadsize):
         self['BLOCSIZE'] = payloadsize
 
     @property
     def frame_nbytes(self):
@@ -229,38 +229,38 @@
     @frame_nbytes.setter
     def frame_nbytes(self, frame_nbytes):
         self.payload_nbytes = frame_nbytes - self.nbytes
 
     @property
     def bps(self):
         """Bits per elementary sample."""
-        return self['NBITS']
+        return int(self['NBITS'])
 
     @bps.setter
     def bps(self, bps):
         self['NBITS'] = bps
 
     @property
     def complex_data(self):
         """Whether the data are complex."""
-        return self['OBSNCHAN'] != 1
+        return int(self['OBSNCHAN']) != 1
 
     @property
     def npol(self):
         """Number of polarisations."""
-        return self['NPOL'] // (2 if self.complex_data else 1)
+        return int(self['NPOL']) // (2 if self.complex_data else 1)
 
     @npol.setter
     def npol(self, npol):
         self['NPOL'] = npol * (2 if self.complex_data else 1)
 
     @property
     def nchan(self):
         """Number of channels."""
-        return self['OBSNCHAN']
+        return int(self['OBSNCHAN'])
 
     @nchan.setter
     def nchan(self, nchan):
         self['OBSNCHAN'] = operator.index(nchan)
 
     @property
     def sample_shape(self):
@@ -274,36 +274,36 @@
         self.nchan = sample_shape[1]
         self.npol = sample_shape[0]
 
     @property
     def _bpcs(self):
         """Bits per complete sample."""
         # NPOL includes factor of 2 for real/complex components.
-        return self['OBSNCHAN'] * self['NPOL'] * self.bps
+        return int(self['OBSNCHAN']) * int(self['NPOL']) * self.bps
 
     @property
     def sample_rate(self):
         """Number of complete samples per second.
 
         Can be set with a negative quantity to set `sideband`.  Overlap samples
         are not included in the rate.
         """
-        return (1. / self['TBIN']) * u.Hz
+        return (1. / float(self['TBIN'])) * u.Hz
 
     @sample_rate.setter
     def sample_rate(self, sample_rate):
         self['TBIN'] = 1. / abs(sample_rate.to_value(u.Hz))
-        bw = (sample_rate.to_value(u.MHz) * self['OBSNCHAN']
+        bw = (sample_rate.to_value(u.MHz) * int(self['OBSNCHAN'])
               / (1 if self.complex_data else 2))
         self['OBSBW'] = bw
 
     @property
     def sideband(self):
         """True if upper sideband."""
-        return self['OBSBW'] > 0
+        return float(self['OBSBW']) > 0
 
     @sideband.setter
     def sideband(self, sideband):
         self['OBSBW'] = (1 if sideband else -1) * abs(self['OBSBW'])
 
     @property
     def channels_first(self):
@@ -330,30 +330,31 @@
                                                      self.samples_per_frame))
             self.payload_nbytes = old_payload_nbytes
             raise exc
 
     @property
     def overlap(self):
         """Number of complete samples that overlap with the next frame."""
-        return self['OVERLAP']
+        return int(self['OVERLAP'])
 
     @overlap.setter
     def overlap(self, overlap):
         self['OVERLAP'] = operator.index(overlap)
 
     @property
     def offset(self):
         """Offset from start of observation in units of time."""
         # PKTIDX only counts valid packets, not overlap ones.
         return ((self['PKTIDX'] * self['PKTSIZE'] * 8 // self._bpcs)
-                * self['TBIN']) * u.s
+                * float(self['TBIN'])) * u.s
 
     @offset.setter
     def offset(self, offset):
-        self['PKTIDX'] = int((offset / (self['TBIN'] * u.s) / self['PKTSIZE']
+        self['PKTIDX'] = int((offset / (float(self['TBIN']) * u.s)
+                              / self['PKTSIZE']
                               * ((self._bpcs + 7) // 8)).to(u.one).round())
 
     @property
     def start_time(self):
         """Start time of the observation."""
         return (Time(self['STT_IMJD'], scale='utc', format='mjd')
                 + TimeDelta(self['STT_SMJD'], self['STT_OFFS'], format='sec'))
```

### Comparing `baseband-4.1.2/baseband/guppi/payload.py` & `baseband-4.1.3/baseband/guppi/payload.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/guppi/tests/test_guppi.py` & `baseband-4.1.3/baseband/guppi/tests/test_guppi.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import numpy as np
 from astropy import units as u
 from astropy.time import Time
 
 from ... import guppi
 from ...helpers import sequentialfile as sf
 from ..base import GUPPIFileNameSequencer
-from ...data import SAMPLE_PUPPI as SAMPLE_FILE
+from ...data import SAMPLE_PUPPI as SAMPLE_FILE, SAMPLE_VEGAS
 
 
 class TestGUPPI:
     def setup_class(cls):
         with open(SAMPLE_FILE, 'rb') as fh:
             cls.header = guppi.GUPPIHeader.fromfile(fh)
             cls.payload = guppi.GUPPIPayload.fromfile(fh, cls.header,
@@ -823,7 +823,20 @@
     def test_header_extraction(self):
         # Follow Nikhil's J1810 Arecibo observation file naming scheme:
         # puppi_58132_J1810+1744_2176.0000.raw, etc.
         template = 'puppi_{stt_imjd}_{src_name}_{scannum}.{file_nr:04d}.raw'
         fns = GUPPIFileNameSequencer(template, self.header)
         assert fns[0] == 'puppi_58132_J1810+1744_2176.0000.raw'
         assert fns[29] == 'puppi_58132_J1810+1744_2176.0029.raw'
+
+
+def test_vegas_header_keywords():
+    with guppi.open(SAMPLE_VEGAS, 'rs') as fh:
+        assert fh.header0.payload_nbytes == 132186112
+        assert fh.header0.bps == 8
+        assert fh.header0.complex_data
+        assert fh.header0.npol == 2
+        assert fh.header0.nchan == 32
+        assert fh.header0.sample_rate == 3125000.0 * u.Hz
+        assert not fh.header0.sideband
+        assert fh.header0.overlap == 512
+        assert fh.header0.offset == 0.
```

### Comparing `baseband-4.1.2/baseband/helpers/sequentialfile.py` & `baseband-4.1.3/baseband/helpers/sequentialfile.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/helpers/tests/test_sequentialfile.py` & `baseband-4.1.3/baseband/helpers/tests/test_sequentialfile.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/io/__init__.py` & `baseband-4.1.3/baseband/io/__init__.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/mark4/base.py` & `baseband-4.1.3/baseband/mark4/base.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/mark4/file_info.py` & `baseband-4.1.3/baseband/mark4/file_info.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/mark4/frame.py` & `baseband-4.1.3/baseband/mark4/frame.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/mark4/header.py` & `baseband-4.1.3/baseband/mark4/header.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/mark4/payload.py` & `baseband-4.1.3/baseband/mark4/payload.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/mark4/tests/test_corrupt_files.py` & `baseband-4.1.3/baseband/mark4/tests/test_corrupt_files.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/mark4/tests/test_mark4.py` & `baseband-4.1.3/baseband/mark4/tests/test_mark4.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/mark5b/base.py` & `baseband-4.1.3/baseband/mark5b/base.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/mark5b/file_info.py` & `baseband-4.1.3/baseband/mark5b/file_info.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/mark5b/frame.py` & `baseband-4.1.3/baseband/mark5b/frame.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/mark5b/header.py` & `baseband-4.1.3/baseband/mark5b/header.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/mark5b/payload.py` & `baseband-4.1.3/baseband/mark5b/payload.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/mark5b/tests/test_corrupt_files.py` & `baseband-4.1.3/baseband/mark5b/tests/test_corrupt_files.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/mark5b/tests/test_mark5b.py` & `baseband-4.1.3/baseband/mark5b/tests/test_mark5b.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/tasks/__init__.py` & `baseband-4.1.3/baseband/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/tests/test_conversion.py` & `baseband-4.1.3/baseband/tests/test_conversion.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/tests/test_core.py` & `baseband-4.1.3/baseband/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/tests/test_entry_points.py` & `baseband-4.1.3/baseband/tests/test_entry_points.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/tests/test_file_info.py` & `baseband-4.1.3/baseband/tests/test_file_info.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/tests/test_sequential_baseband.py` & `baseband-4.1.3/baseband/tests/test_sequential_baseband.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/vdif/__init__.py` & `baseband-4.1.3/baseband/vdif/__init__.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/vdif/base.py` & `baseband-4.1.3/baseband/vdif/base.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/vdif/file_info.py` & `baseband-4.1.3/baseband/vdif/file_info.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/vdif/frame.py` & `baseband-4.1.3/baseband/vdif/frame.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/vdif/header.py` & `baseband-4.1.3/baseband/vdif/header.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/vdif/payload.py` & `baseband-4.1.3/baseband/vdif/payload.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/vdif/tests/test_corrupt_files.py` & `baseband-4.1.3/baseband/vdif/tests/test_corrupt_files.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband/vdif/tests/test_vdif.py` & `baseband-4.1.3/baseband/vdif/tests/test_vdif.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/baseband.egg-info/PKG-INFO` & `baseband-4.1.3/baseband.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baseband
-Version: 4.1.2
+Version: 4.1.3
 Summary: A package for radio baseband I/O
 Home-page: https://github.com/mhvk/baseband
 Author: Marten H. van Kerkwijk, Chenchong Zhu
 Author-email: mhvk@astro.utoronto.ca
 License: GNU GPL v3+
 Project-URL: Documentation, https://baseband.readthedocs.io
 Project-URL: Source, https://github.com/mhvk/baseband
```

### Comparing `baseband-4.1.2/baseband.egg-info/SOURCES.txt` & `baseband-4.1.3/baseband.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 baseband/data/sample_64track_fanout2_ft.m4
 baseband/data/sample_arochime.vdif
 baseband/data/sample_bps1.vdif
 baseband/data/sample_drao_corrupted.vdif
 baseband/data/sample_meerkat.dada
 baseband/data/sample_mwa.vdif
 baseband/data/sample_puppi.raw
+baseband/data/sample_vegas.raw
 baseband/data/sample_vlbi.vdif
 baseband/data/gsb/__init__.py
 baseband/data/gsb/sample_gsb_phased.Pol-L1.dat
 baseband/data/gsb/sample_gsb_phased.Pol-L2.dat
 baseband/data/gsb/sample_gsb_phased.Pol-R1.dat
 baseband/data/gsb/sample_gsb_phased.Pol-R2.dat
 baseband/data/gsb/sample_gsb_phased.timestamp
```

### Comparing `baseband-4.1.2/docs/Makefile` & `baseband-4.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/docs/conf.py` & `baseband-4.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/docs/dada/header.rst` & `baseband-4.1.3/docs/dada/header.rst`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/docs/dada/index.rst` & `baseband-4.1.3/docs/dada/index.rst`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/docs/gsb/index.rst` & `baseband-4.1.3/docs/gsb/index.rst`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/docs/guppi/index.rst` & `baseband-4.1.3/docs/guppi/index.rst`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/docs/helpers/index.rst` & `baseband-4.1.3/docs/helpers/index.rst`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/docs/index.rst` & `baseband-4.1.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/docs/install.rst` & `baseband-4.1.3/docs/install.rst`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/docs/make.bat` & `baseband-4.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/docs/mark4/index.rst` & `baseband-4.1.3/docs/mark4/index.rst`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/docs/mark5b/index.rst` & `baseband-4.1.3/docs/mark5b/index.rst`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/docs/nitpick-exceptions` & `baseband-4.1.3/docs/nitpick-exceptions`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/docs/tutorials/VDIFHeader.png` & `baseband-4.1.3/docs/tutorials/VDIFHeader.png`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/docs/tutorials/getting_started.rst` & `baseband-4.1.3/docs/tutorials/getting_started.rst`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/docs/tutorials/glossary.rst` & `baseband-4.1.3/docs/tutorials/glossary.rst`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/docs/tutorials/glossary_substitutions.rst` & `baseband-4.1.3/docs/tutorials/glossary_substitutions.rst`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/docs/tutorials/new_edv.rst` & `baseband-4.1.3/docs/tutorials/new_edv.rst`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/docs/tutorials/new_format.rst` & `baseband-4.1.3/docs/tutorials/new_format.rst`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/docs/tutorials/performance_tips.rst` & `baseband-4.1.3/docs/tutorials/performance_tips.rst`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/docs/tutorials/release_procedure.rst` & `baseband-4.1.3/docs/tutorials/release_procedure.rst`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/docs/tutorials/using_baseband.rst` & `baseband-4.1.3/docs/tutorials/using_baseband.rst`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/docs/vdif/index.rst` & `baseband-4.1.3/docs/vdif/index.rst`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/setup.cfg` & `baseband-4.1.3/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 
 [options.extras_require]
 all = 
 	baseband-tasks[all]
 test = 
 	pytest-astropy-header
 	pytest-doctestplus
-	pytest-openfiles
 cov = 
 	pytest-cov
 docs = 
 	sphinx-astropy
 
 [options.package_data]
 baseband = data/*, data/gsb/*
```

### Comparing `baseband-4.1.2/setup.py` & `baseband-4.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `baseband-4.1.2/tox.ini` & `baseband-4.1.3/tox.ini`

 * *Files identical despite different names*

