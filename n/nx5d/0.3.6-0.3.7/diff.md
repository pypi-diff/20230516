# Comparing `tmp/nx5d-0.3.6.tar.gz` & `tmp/nx5d-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nx5d-0.3.6.tar", last modified: Mon May  1 16:15:32 2023, max compression
+gzip compressed data, was "nx5d-0.3.7.tar", last modified: Tue May 16 06:51:00 2023, max compression
```

## Comparing `nx5d-0.3.6.tar` & `nx5d-0.3.7.tar`

### file list

```diff
@@ -1,182 +1,225 @@
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-01 16:15:32.384182 nx5d-0.3.6/
--rw-r--r--   0 florin    (1000) florin    (1000)       72 2023-04-24 10:31:16.000000 nx5d-0.3.6/.gitignore
--rw-r--r--   0 florin    (1000) florin    (1000)     3261 2023-04-24 10:31:16.000000 nx5d-0.3.6/.gitlab-ci.yml
--rw-r--r--   0 florin    (1000) florin    (1000)      227 2023-03-30 12:37:15.000000 nx5d-0.3.6/.readthedocs.yaml
--rw-r--r--   0 florin    (1000) florin    (1000)    34916 2023-03-30 12:37:15.000000 nx5d-0.3.6/COPYING.md
--rw-r--r--   0 florin    (1000) florin    (1000)     3514 2023-05-01 16:15:32.384182 nx5d-0.3.6/PKG-INFO
--rw-r--r--   0 florin    (1000) florin    (1000)     2724 2023-03-30 12:37:15.000000 nx5d-0.3.6/README.md
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-01 16:15:32.360182 nx5d-0.3.6/doc/
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-01 16:15:32.361182 nx5d-0.3.6/doc/mkdocs/
--rw-r--r--   0 florin    (1000) florin    (1000)       11 2023-03-30 12:37:15.000000 nx5d-0.3.6/doc/mkdocs/about.md
--rw-r--r--   0 florin    (1000) florin    (1000)      147 2023-04-24 10:31:17.000000 nx5d-0.3.6/doc/mkdocs/api.md
--rw-r--r--   0 florin    (1000) florin    (1000)    27056 2023-04-25 08:54:47.000000 nx5d-0.3.6/doc/mkdocs/concepts.md
--rw-r--r--   0 florin    (1000) florin    (1000)     5970 2023-03-30 12:37:15.000000 nx5d-0.3.6/doc/mkdocs/frame.svg
--rw-r--r--   0 florin    (1000) florin    (1000)     2483 2023-04-25 08:54:47.000000 nx5d-0.3.6/doc/mkdocs/index.md
--rw-r--r--   0 florin    (1000) florin    (1000)    34916 2023-03-30 12:37:15.000000 nx5d-0.3.6/doc/mkdocs/license.md
--rw-r--r--   0 florin    (1000) florin    (1000)      723 2023-03-30 12:37:15.000000 nx5d-0.3.6/doc/mkdocs/module-nx.md
--rw-r--r--   0 florin    (1000) florin    (1000)    36207 2023-03-30 12:37:15.000000 nx5d-0.3.6/doc/mkdocs/scan.svg
--rw-r--r--   0 florin    (1000) florin    (1000)    25024 2023-03-30 12:37:15.000000 nx5d-0.3.6/doc/mkdocs/streak1.svg
--rw-r--r--   0 florin    (1000) florin    (1000)    11491 2023-03-30 12:37:15.000000 nx5d-0.3.6/doc/mkdocs/streak2.svg
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-01 16:15:32.361182 nx5d-0.3.6/doc/mkdocs/tutorials/
--rw-r--r--   0 florin    (1000) florin    (1000)      516 2023-03-30 12:37:15.000000 nx5d-0.3.6/doc/mkdocs/tutorials/index.md
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-01 16:15:32.362182 nx5d-0.3.6/doc/mkdocs/tutorials/kmc3-data-processing-howto/
--rw-r--r--   0 florin    (1000) florin    (1000)    44315 2023-03-30 12:37:15.000000 nx5d-0.3.6/doc/mkdocs/tutorials/kmc3-data-processing-howto/kmc3-data-processing-howto.md
--rw-r--r--   0 florin    (1000) florin    (1000)    19430 2023-03-30 12:37:15.000000 nx5d-0.3.6/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_0.png
--rw-r--r--   0 florin    (1000) florin    (1000)    25263 2023-03-30 12:37:15.000000 nx5d-0.3.6/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_1.png
--rw-r--r--   0 florin    (1000) florin    (1000)    23184 2023-03-30 12:37:15.000000 nx5d-0.3.6/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_2.png
--rw-r--r--   0 florin    (1000) florin    (1000)    13289 2023-03-30 12:37:15.000000 nx5d-0.3.6/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_33_0.png
--rw-r--r--   0 florin    (1000) florin    (1000)    16038 2023-03-30 12:37:15.000000 nx5d-0.3.6/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_52_1.png
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-01 16:15:32.362182 nx5d-0.3.6/doc/mkdocs/tutorials/scansource-howto/
--rw-r--r--   0 florin    (1000) florin    (1000)     8968 2023-03-30 12:37:15.000000 nx5d-0.3.6/doc/mkdocs/tutorials/scansource-howto/scansource-howto.md
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-01 16:15:32.363182 nx5d-0.3.6/doc/mkdocs/user-guide/
--rw-r--r--   0 florin    (1000) florin    (1000)      322 2023-04-24 10:31:17.000000 nx5d-0.3.6/doc/mkdocs/user-guide/index.md
--rw-r--r--   0 florin    (1000) florin    (1000)      513 2023-03-30 12:37:15.000000 nx5d-0.3.6/doc/mkdocs.yml
--rw-r--r--   0 florin    (1000) florin    (1000)      273 2023-03-30 12:37:15.000000 nx5d-0.3.6/mkdocs.yml
--rw-r--r--   0 florin    (1000) florin    (1000)      280 2023-03-30 12:37:15.000000 nx5d-0.3.6/pyproject.toml
--rw-r--r--   0 florin    (1000) florin    (1000)     2974 2023-03-30 12:37:15.000000 nx5d-0.3.6/scratch.org
--rw-r--r--   0 florin    (1000) florin    (1000)      946 2023-05-01 16:15:32.384182 nx5d-0.3.6/setup.cfg
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-01 16:15:32.357182 nx5d-0.3.6/src/
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-01 16:15:32.364182 nx5d-0.3.6/src/nx5d/
--rw-r--r--   0 florin    (1000) florin    (1000)      117 2023-03-30 12:37:15.000000 nx5d-0.3.6/src/nx5d/__init__.py
--rw-r--r--   0 florin    (1000) florin    (1000)      160 2023-05-01 16:15:32.000000 nx5d-0.3.6/src/nx5d/_version.py
--rwxr-xr-x   0 florin    (1000) florin    (1000)     7559 2023-03-30 12:37:15.000000 nx5d-0.3.6/src/nx5d/edf.py
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-01 16:15:32.366182 nx5d-0.3.6/src/nx5d/h5like/
--rw-r--r--   0 florin    (1000) florin    (1000)        0 2023-04-24 10:31:17.000000 nx5d-0.3.6/src/nx5d/h5like/__init__.py
--rw-r--r--   0 florin    (1000) florin    (1000)    12534 2023-05-01 15:31:12.000000 nx5d-0.3.6/src/nx5d/h5like/petra3.py
--rw-r--r--   0 florin    (1000) florin    (1000)     5686 2023-04-24 10:31:17.000000 nx5d-0.3.6/src/nx5d/h5like/pypod.py
--rw-r--r--   0 florin    (1000) florin    (1000)    10119 2023-05-01 15:16:41.000000 nx5d-0.3.6/src/nx5d/h5like/spec.py
--rw-r--r--   0 florin    (1000) florin    (1000)    11159 2023-05-01 15:49:22.000000 nx5d-0.3.6/src/nx5d/h5like/tools.py
--rw-r--r--   0 florin    (1000) florin    (1000)    31529 2023-04-24 10:31:17.000000 nx5d-0.3.6/src/nx5d/h5like/xfel.py
--rwxr-xr-x   0 florin    (1000) florin    (1000)    15796 2023-03-30 12:37:15.000000 nx5d-0.3.6/src/nx5d/nx.py
--rwxr-xr-x   0 florin    (1000) florin    (1000)     7585 2023-03-30 12:37:15.000000 nx5d-0.3.6/src/nx5d/runlog.py
--rw-r--r--   0 florin    (1000) florin    (1000)    14860 2023-05-01 15:16:41.000000 nx5d-0.3.6/src/nx5d/scan.py
--rw-r--r--   0 florin    (1000) florin    (1000)     7572 2023-04-24 10:31:17.000000 nx5d-0.3.6/src/nx5d/streaks.py
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-01 16:15:32.368182 nx5d-0.3.6/src/nx5d/xrd/
--rw-r--r--   0 florin    (1000) florin    (1000)      756 2023-03-30 12:37:15.000000 nx5d-0.3.6/src/nx5d/xrd/ColonelSandersFinest.py
--rw-r--r--   0 florin    (1000) florin    (1000)        0 2023-03-30 12:37:15.000000 nx5d-0.3.6/src/nx5d/xrd/__init__.py
--rwxr-xr-x   0 florin    (1000) florin    (1000)     4859 2023-03-30 12:37:15.000000 nx5d-0.3.6/src/nx5d/xrd/analysis.py
--rw-r--r--   0 florin    (1000) florin    (1000)      972 2023-03-30 12:37:15.000000 nx5d-0.3.6/src/nx5d/xrd/esrf_id09.py
--rw-r--r--   0 florin    (1000) florin    (1000)     1481 2023-03-30 12:37:15.000000 nx5d-0.3.6/src/nx5d/xrd/experiment-xpp.yml
--rw-r--r--   0 florin    (1000) florin    (1000)     4201 2023-03-30 12:37:15.000000 nx5d-0.3.6/src/nx5d/xrd/experiment.py
--rw-r--r--   0 florin    (1000) florin    (1000)     1939 2023-05-01 15:16:41.000000 nx5d-0.3.6/src/nx5d/xrd/kmc3.py
--rw-r--r--   0 florin    (1000) florin    (1000)      681 2023-05-01 15:51:21.000000 nx5d-0.3.6/src/nx5d/xrd/petra3.py
--rw-r--r--   0 florin    (1000) florin    (1000)     4316 2023-03-30 12:37:15.000000 nx5d-0.3.6/src/nx5d/xrd/roi.py
--rw-r--r--   0 florin    (1000) florin    (1000)    19835 2023-05-01 16:13:20.000000 nx5d-0.3.6/src/nx5d/xrd/signal.py
--rw-r--r--   0 florin    (1000) florin    (1000)      972 2023-04-24 10:31:17.000000 nx5d-0.3.6/src/nx5d/xrd/xfel.py
--rwxr-xr-x   0 florin    (1000) florin    (1000)     3960 2023-03-30 12:37:15.000000 nx5d-0.3.6/src/nx5d/xrd/xraytest.py
--rw-r--r--   0 florin    (1000) florin    (1000)    15899 2023-03-30 12:37:15.000000 nx5d-0.3.6/src/nx5d/xrd/xrd_helpers.py
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-01 16:15:32.365182 nx5d-0.3.6/src/nx5d.egg-info/
--rw-r--r--   0 florin    (1000) florin    (1000)     3514 2023-05-01 16:15:32.000000 nx5d-0.3.6/src/nx5d.egg-info/PKG-INFO
--rw-r--r--   0 florin    (1000) florin    (1000)     7817 2023-05-01 16:15:32.000000 nx5d-0.3.6/src/nx5d.egg-info/SOURCES.txt
--rw-r--r--   0 florin    (1000) florin    (1000)        1 2023-05-01 16:15:32.000000 nx5d-0.3.6/src/nx5d.egg-info/dependency_links.txt
--rw-r--r--   0 florin    (1000) florin    (1000)      157 2023-05-01 16:15:32.000000 nx5d-0.3.6/src/nx5d.egg-info/requires.txt
--rw-r--r--   0 florin    (1000) florin    (1000)        5 2023-05-01 16:15:32.000000 nx5d-0.3.6/src/nx5d.egg-info/top_level.txt
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-01 16:15:32.369182 nx5d-0.3.6/tests/
--rw-r--r--   0 florin    (1000) florin    (1000)        0 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/.gitignore
--rw-r--r--   0 florin    (1000) florin    (1000)     1167 2023-05-01 15:16:41.000000 nx5d-0.3.6/tests/fio_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)      961 2023-04-24 10:31:17.000000 nx5d-0.3.6/tests/pabst_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)     1559 2023-04-24 10:31:17.000000 nx5d-0.3.6/tests/pypod_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)     1342 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/runlog_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)      915 2023-05-01 15:16:41.000000 nx5d-0.3.6/tests/spec_test.py
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-01 16:15:32.358182 nx5d-0.3.6/tests/test_data/
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-01 16:15:32.369182 nx5d-0.3.6/tests/test_data/fioh5/
--rw-r--r--   0 florin    (1000) florin    (1000)    13611 2023-05-01 15:16:41.000000 nx5d-0.3.6/tests/test_data/fioh5/m3_2507_00342.fio
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-01 16:15:32.358182 nx5d-0.3.6/tests/test_data/fioh5/m3_2507_00744/
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-01 16:15:32.369182 nx5d-0.3.6/tests/test_data/fioh5/m3_2507_00744/lambda/
--rw-r--r--   0 florin    (1000) florin    (1000)   302228 2023-05-01 15:16:41.000000 nx5d-0.3.6/tests/test_data/fioh5/m3_2507_00744/lambda/m3_2507_00744_00000.nxs
--rw-r--r--   0 florin    (1000) florin    (1000)    13952 2023-05-01 15:16:41.000000 nx5d-0.3.6/tests/test_data/fioh5/m3_2507_00744.fio
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-01 16:15:32.376182 nx5d-0.3.6/tests/test_data/runfile/
--rw-r--r--   0 florin    (1000) florin    (1000)     5668 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/runfile/run04.log
--rw-r--r--   0 florin    (1000) florin    (1000)    10599 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/runfile/run105.log
--rw-r--r--   0 florin    (1000) florin    (1000)    10591 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/runfile/run105_brokendata1.log
--rw-r--r--   0 florin    (1000) florin    (1000)    10591 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/runfile/run105_brokendata2.log
--rw-r--r--   0 florin    (1000) florin    (1000)    10591 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/runfile/run105_brokenheader.log
--rw-r--r--   0 florin    (1000) florin    (1000)    10588 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/runfile/run105_simple.log
--rw-r--r--   0 florin    (1000) florin    (1000)     5668 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/runfile/short_run04.log
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/runfile/short_run04_0001.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/runfile/short_run04_0002.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/runfile/short_run04_0003.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/runfile/short_run04_0004.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/runfile/short_run04_0005.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/runfile/short_run04_0006.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/runfile/short_run04_0007.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/runfile/short_run04_0008.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/runfile/short_run04_0009.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/runfile/short_run04_0010.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/runfile/short_run04_0011.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/runfile/short_run04_0012.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/runfile/short_run04_0013.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/runfile/short_run04_0014.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/runfile/short_run04_0015.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/runfile/short_run04_0016.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/runfile/short_run04_0017.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/runfile/short_run04_0018.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/runfile/short_run04_0019.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/runfile/short_run04_0020.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/runfile/short_run04_0021.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/runfile/short_run04_0022.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/runfile/short_run04_0023.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/runfile/short_run04_0024.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/runfile/short_run04_0025.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/runfile/short_run04_0026.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/runfile/short_run04_0027.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/runfile/short_run04_0028.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/runfile/short_run04_0029.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/runfile/short_run04_0030.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/runfile/short_run04_0031.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/runfile/short_run04_0032.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/runfile/short_run04_0033.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/runfile/short_run04_0034.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/runfile/short_run04_0035.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/runfile/short_run04_0036.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/runfile/short_run04_0037.edf
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-01 16:15:32.358182 nx5d-0.3.6/tests/test_data/spech5/
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-01 16:15:32.376182 nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/
--rw-r--r--   0 florin    (1000) florin    (1000)  1374025 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/231-cw7-12083-roessle.spec
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-01 16:15:32.358182 nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-01 16:15:32.377182 nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00002/
--rw-r--r--   0 florin    (1000) florin    (1000)    32118 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00002/231-cw7-12083-roessle_2_0.tif
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-01 16:15:32.384182 nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/
--rw-r--r--   0 florin    (1000) florin    (1000)     2133 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_0.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2204 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_1.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3368 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_10.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3429 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_11.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3609 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_12.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3668 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_13.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3827 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_14.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4037 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_15.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4216 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_16.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4322 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_17.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4305 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_18.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4307 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_19.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2228 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_2.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4307 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_20.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4165 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_21.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3937 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_22.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3842 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_23.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3835 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_24.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3592 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_25.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3479 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_26.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3270 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_27.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3221 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_28.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3065 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_29.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2427 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_3.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2901 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_30.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2931 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_31.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2707 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_32.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2548 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_33.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2512 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_34.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2306 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_35.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2260 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_36.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2162 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_37.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2078 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_38.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2026 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_39.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2556 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_4.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2013 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_40.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2654 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_5.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2786 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_6.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2845 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_7.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3019 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_8.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3164 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_9.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3341 2023-04-24 10:31:17.000000 nx5d-0.3.6/tests/xfel_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)     1059 2023-03-30 12:37:15.000000 nx5d-0.3.6/tests/xrd_data_test.py
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.839137 nx5d-0.3.7/
+-rw-r--r--   0 florin    (1000) florin    (1000)       72 2023-04-13 14:23:04.000000 nx5d-0.3.7/.gitignore
+-rw-r--r--   0 florin    (1000) florin    (1000)     3261 2023-04-12 13:31:40.000000 nx5d-0.3.7/.gitlab-ci.yml
+-rw-r--r--   0 florin    (1000) florin    (1000)      227 2023-03-15 11:10:41.000000 nx5d-0.3.7/.readthedocs.yaml
+-rw-r--r--   0 florin    (1000) florin    (1000)    34916 2023-03-14 11:33:48.000000 nx5d-0.3.7/COPYING.md
+-rw-r--r--   0 florin    (1000) florin    (1000)     3514 2023-05-16 06:51:00.839137 nx5d-0.3.7/PKG-INFO
+-rw-r--r--   0 florin    (1000) florin    (1000)     2724 2023-03-27 10:49:57.000000 nx5d-0.3.7/README.md
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.817137 nx5d-0.3.7/doc/
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.818137 nx5d-0.3.7/doc/mkdocs/
+-rw-r--r--   0 florin    (1000) florin    (1000)       11 2023-03-15 10:15:42.000000 nx5d-0.3.7/doc/mkdocs/about.md
+-rw-r--r--   0 florin    (1000) florin    (1000)      147 2023-04-12 12:52:07.000000 nx5d-0.3.7/doc/mkdocs/api.md
+-rw-r--r--   0 florin    (1000) florin    (1000)    27056 2023-04-25 09:48:18.000000 nx5d-0.3.7/doc/mkdocs/concepts.md
+-rw-r--r--   0 florin    (1000) florin    (1000)     5970 2023-03-25 14:27:00.000000 nx5d-0.3.7/doc/mkdocs/frame.svg
+-rw-r--r--   0 florin    (1000) florin    (1000)     2483 2023-04-25 09:48:18.000000 nx5d-0.3.7/doc/mkdocs/index.md
+-rw-r--r--   0 florin    (1000) florin    (1000)    34916 2023-03-15 10:32:22.000000 nx5d-0.3.7/doc/mkdocs/license.md
+-rw-r--r--   0 florin    (1000) florin    (1000)      723 2023-03-27 10:50:49.000000 nx5d-0.3.7/doc/mkdocs/module-nx.md
+-rw-r--r--   0 florin    (1000) florin    (1000)    36207 2023-03-25 14:25:35.000000 nx5d-0.3.7/doc/mkdocs/scan.svg
+-rw-r--r--   0 florin    (1000) florin    (1000)    25024 2023-03-25 14:49:22.000000 nx5d-0.3.7/doc/mkdocs/streak1.svg
+-rw-r--r--   0 florin    (1000) florin    (1000)    11491 2023-03-25 14:49:37.000000 nx5d-0.3.7/doc/mkdocs/streak2.svg
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.818137 nx5d-0.3.7/doc/mkdocs/tutorials/
+-rw-r--r--   0 florin    (1000) florin    (1000)      516 2023-03-15 10:35:31.000000 nx5d-0.3.7/doc/mkdocs/tutorials/index.md
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.819137 nx5d-0.3.7/doc/mkdocs/tutorials/kmc3-data-processing-howto/
+-rw-------   0 florin    (1000) florin    (1000)    44315 2023-03-14 14:52:34.000000 nx5d-0.3.7/doc/mkdocs/tutorials/kmc3-data-processing-howto/kmc3-data-processing-howto.md
+-rw-------   0 florin    (1000) florin    (1000)    19430 2023-03-14 14:52:34.000000 nx5d-0.3.7/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_0.png
+-rw-------   0 florin    (1000) florin    (1000)    25263 2023-03-14 14:52:34.000000 nx5d-0.3.7/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_1.png
+-rw-------   0 florin    (1000) florin    (1000)    23184 2023-03-14 14:52:34.000000 nx5d-0.3.7/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_2.png
+-rw-------   0 florin    (1000) florin    (1000)    13289 2023-03-14 14:52:34.000000 nx5d-0.3.7/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_33_0.png
+-rw-------   0 florin    (1000) florin    (1000)    16038 2023-03-14 14:52:34.000000 nx5d-0.3.7/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_52_1.png
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.819137 nx5d-0.3.7/doc/mkdocs/tutorials/scansource-howto/
+-rw-r--r--   0 florin    (1000) florin    (1000)     8968 2023-03-14 12:31:08.000000 nx5d-0.3.7/doc/mkdocs/tutorials/scansource-howto/scansource-howto.md
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.819137 nx5d-0.3.7/doc/mkdocs/user-guide/
+-rw-r--r--   0 florin    (1000) florin    (1000)      322 2023-04-12 12:48:11.000000 nx5d-0.3.7/doc/mkdocs/user-guide/index.md
+-rw-r--r--   0 florin    (1000) florin    (1000)      513 2023-03-15 14:06:55.000000 nx5d-0.3.7/doc/mkdocs.yml
+-rw-r--r--   0 florin    (1000) florin    (1000)      273 2023-03-15 10:49:21.000000 nx5d-0.3.7/mkdocs.yml
+-rw-r--r--   0 florin    (1000) florin    (1000)      280 2023-03-14 11:33:48.000000 nx5d-0.3.7/pyproject.toml
+-rw-r--r--   0 florin    (1000) florin    (1000)     2974 2022-08-02 20:02:56.000000 nx5d-0.3.7/scratch.org
+-rw-r--r--   0 florin    (1000) florin    (1000)      946 2023-05-16 06:51:00.839137 nx5d-0.3.7/setup.cfg
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.815137 nx5d-0.3.7/src/
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.820137 nx5d-0.3.7/src/nx5d/
+-rw-r--r--   0 florin    (1000) florin    (1000)      117 2023-03-14 11:33:48.000000 nx5d-0.3.7/src/nx5d/__init__.py
+-rw-r--r--   0 florin    (1000) florin    (1000)      160 2023-05-16 06:51:00.000000 nx5d-0.3.7/src/nx5d/_version.py
+-rwxr-xr-x   0 florin    (1000) florin    (1000)     7559 2023-03-14 11:33:48.000000 nx5d-0.3.7/src/nx5d/edf.py
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.821137 nx5d-0.3.7/src/nx5d/h5like/
+-rw-r--r--   0 florin    (1000) florin    (1000)        0 2023-04-12 12:44:54.000000 nx5d-0.3.7/src/nx5d/h5like/__init__.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    12534 2023-05-16 06:50:26.000000 nx5d-0.3.7/src/nx5d/h5like/petra3.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     5686 2023-04-17 15:45:54.000000 nx5d-0.3.7/src/nx5d/h5like/pypod.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    11003 2023-05-16 06:50:26.000000 nx5d-0.3.7/src/nx5d/h5like/spec.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    11159 2023-05-16 06:50:26.000000 nx5d-0.3.7/src/nx5d/h5like/tools.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    31529 2023-04-13 15:04:17.000000 nx5d-0.3.7/src/nx5d/h5like/xfel.py
+-rwxr-xr-x   0 florin    (1000) florin    (1000)    15796 2023-03-14 11:33:48.000000 nx5d-0.3.7/src/nx5d/nx.py
+-rwxr-xr-x   0 florin    (1000) florin    (1000)     7585 2023-03-14 11:33:48.000000 nx5d-0.3.7/src/nx5d/runlog.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    14860 2023-04-27 14:19:57.000000 nx5d-0.3.7/src/nx5d/scan.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     7572 2023-04-17 15:45:54.000000 nx5d-0.3.7/src/nx5d/streaks.py
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.823137 nx5d-0.3.7/src/nx5d/xrd/
+-rw-r--r--   0 florin    (1000) florin    (1000)      756 2023-03-14 11:33:48.000000 nx5d-0.3.7/src/nx5d/xrd/ColonelSandersFinest.py
+-rw-r--r--   0 florin    (1000) florin    (1000)        0 2023-03-14 11:33:48.000000 nx5d-0.3.7/src/nx5d/xrd/__init__.py
+-rwxr-xr-x   0 florin    (1000) florin    (1000)     4859 2023-03-14 11:33:48.000000 nx5d-0.3.7/src/nx5d/xrd/analysis.py
+-rw-r--r--   0 florin    (1000) florin    (1000)      972 2023-03-14 11:33:48.000000 nx5d-0.3.7/src/nx5d/xrd/esrf_id09.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     1481 2023-03-14 11:33:48.000000 nx5d-0.3.7/src/nx5d/xrd/experiment-xpp.yml
+-rw-r--r--   0 florin    (1000) florin    (1000)     4201 2023-03-14 11:33:48.000000 nx5d-0.3.7/src/nx5d/xrd/experiment.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     1939 2023-04-27 14:16:35.000000 nx5d-0.3.7/src/nx5d/xrd/kmc3.py
+-rw-r--r--   0 florin    (1000) florin    (1000)      779 2023-05-16 06:50:26.000000 nx5d-0.3.7/src/nx5d/xrd/petra3.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     4316 2023-03-14 11:33:48.000000 nx5d-0.3.7/src/nx5d/xrd/roi.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    19952 2023-05-16 06:50:26.000000 nx5d-0.3.7/src/nx5d/xrd/signal.py
+-rw-r--r--   0 florin    (1000) florin    (1000)      972 2023-04-25 09:48:18.000000 nx5d-0.3.7/src/nx5d/xrd/xfel.py
+-rwxr-xr-x   0 florin    (1000) florin    (1000)     3960 2023-03-14 11:33:48.000000 nx5d-0.3.7/src/nx5d/xrd/xraytest.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    15899 2023-03-14 11:33:48.000000 nx5d-0.3.7/src/nx5d/xrd/xrd_helpers.py
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.821137 nx5d-0.3.7/src/nx5d.egg-info/
+-rw-r--r--   0 florin    (1000) florin    (1000)     3514 2023-05-16 06:51:00.000000 nx5d-0.3.7/src/nx5d.egg-info/PKG-INFO
+-rw-r--r--   0 florin    (1000) florin    (1000)    11943 2023-05-16 06:51:00.000000 nx5d-0.3.7/src/nx5d.egg-info/SOURCES.txt
+-rw-r--r--   0 florin    (1000) florin    (1000)        1 2023-05-16 06:51:00.000000 nx5d-0.3.7/src/nx5d.egg-info/dependency_links.txt
+-rw-r--r--   0 florin    (1000) florin    (1000)      157 2023-05-16 06:51:00.000000 nx5d-0.3.7/src/nx5d.egg-info/requires.txt
+-rw-r--r--   0 florin    (1000) florin    (1000)        5 2023-05-16 06:51:00.000000 nx5d-0.3.7/src/nx5d.egg-info/top_level.txt
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.823137 nx5d-0.3.7/tests/
+-rw-r--r--   0 florin    (1000) florin    (1000)        0 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/.gitignore
+-rw-r--r--   0 florin    (1000) florin    (1000)     1167 2023-04-27 15:21:20.000000 nx5d-0.3.7/tests/fio_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)      961 2023-04-17 15:45:54.000000 nx5d-0.3.7/tests/pabst_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     1559 2023-04-17 15:45:54.000000 nx5d-0.3.7/tests/pypod_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     1342 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/runlog_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     2219 2023-05-16 06:50:26.000000 nx5d-0.3.7/tests/spec_test.py
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.816137 nx5d-0.3.7/tests/test_data/
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.824137 nx5d-0.3.7/tests/test_data/fioh5/
+-rw-r--r--   0 florin    (1000) florin    (1000)    13611 2023-04-25 09:48:18.000000 nx5d-0.3.7/tests/test_data/fioh5/m3_2507_00342.fio
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.816137 nx5d-0.3.7/tests/test_data/fioh5/m3_2507_00744/
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.824137 nx5d-0.3.7/tests/test_data/fioh5/m3_2507_00744/lambda/
+-rw-r--r--   0 florin    (1000) florin    (1000)   302228 2023-04-25 10:50:01.000000 nx5d-0.3.7/tests/test_data/fioh5/m3_2507_00744/lambda/m3_2507_00744_00000.nxs
+-rw-r--r--   0 florin    (1000) florin    (1000)    13952 2023-04-25 09:48:18.000000 nx5d-0.3.7/tests/test_data/fioh5/m3_2507_00744.fio
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.828137 nx5d-0.3.7/tests/test_data/runfile/
+-rw-r--r--   0 florin    (1000) florin    (1000)     5668 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/run04.log
+-rw-r--r--   0 florin    (1000) florin    (1000)    10599 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/run105.log
+-rw-r--r--   0 florin    (1000) florin    (1000)    10591 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/run105_brokendata1.log
+-rw-r--r--   0 florin    (1000) florin    (1000)    10591 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/run105_brokendata2.log
+-rw-r--r--   0 florin    (1000) florin    (1000)    10591 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/run105_brokenheader.log
+-rw-r--r--   0 florin    (1000) florin    (1000)    10588 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/run105_simple.log
+-rw-r--r--   0 florin    (1000) florin    (1000)     5668 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04.log
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0001.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0002.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0003.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0004.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0005.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0006.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0007.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0008.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0009.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0010.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0011.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0012.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0013.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0014.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0015.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0016.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0017.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0018.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0019.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0020.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0021.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0022.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0023.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0024.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0025.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0026.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0027.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0028.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0029.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0030.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0031.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0032.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0033.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0034.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0035.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0036.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0037.edf
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.816137 nx5d-0.3.7/tests/test_data/spech5/
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.828137 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/
+-rw-r--r--   0 florin    (1000) florin    (1000)  1374025 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/231-cw7-12083-roessle.spec
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.816137 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.834137 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00002/
+-rw-r--r--   0 florin    (1000) florin    (1000)    32118 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00002/231-cw7-12083-roessle_2_0.tif
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.839137 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/
+-rw-r--r--   0 florin    (1000) florin    (1000)     2133 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_0.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2204 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_1.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3368 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_10.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3429 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_11.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3609 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_12.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3668 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_13.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3827 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_14.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4037 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_15.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4216 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_16.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4322 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_17.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4305 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_18.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4307 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_19.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2228 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_2.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4307 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_20.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4165 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_21.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3937 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_22.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3842 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_23.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3835 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_24.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3592 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_25.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3479 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_26.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3270 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_27.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3221 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_28.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3065 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_29.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2427 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_3.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2901 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_30.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2931 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_31.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2707 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_32.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2548 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_33.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2512 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_34.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2306 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_35.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2260 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_36.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2162 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_37.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2078 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_38.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2026 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_39.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2556 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_4.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2013 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_40.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2654 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_5.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2786 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_6.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2845 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_7.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3019 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_8.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3164 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_9.tif
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.829137 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/
+-rw-r--r--   0 florin    (1000) florin    (1000)  1374025 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/231-cw7-12083-roessle-missing.spec
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.816137 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.834137 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/
+-rw-r--r--   0 florin    (1000) florin    (1000)     2204 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_1.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3368 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_10.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3429 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_11.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3827 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_14.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4037 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_15.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4216 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_16.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4322 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_17.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4305 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_18.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4307 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_19.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2228 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_2.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4307 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_20.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4165 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_21.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3937 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_22.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3842 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_23.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3835 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_24.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3592 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_25.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3479 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_26.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3270 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_27.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3221 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_28.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3065 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_29.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2427 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_3.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2901 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_30.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2931 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_31.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2707 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_32.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2548 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_33.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2512 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_34.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2306 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_35.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2260 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_36.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2162 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_37.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2078 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_38.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2026 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_39.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2556 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_4.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2013 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_40.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2654 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_5.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2786 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_6.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2845 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_7.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3019 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_8.tif
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.839137 nx5d-0.3.7/tests/test_data/spech5/empty-spec/
+-rw-r--r--   0 florin    (1000) florin    (1000)     5209 2023-05-16 06:50:26.000000 nx5d-0.3.7/tests/test_data/spech5/empty-spec/empty-spec.spec
+-rw-r--r--   0 florin    (1000) florin    (1000)     3341 2023-04-13 14:23:04.000000 nx5d-0.3.7/tests/xfel_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     1059 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/xrd_data_test.py
```

### Comparing `nx5d-0.3.6/.gitlab-ci.yml` & `nx5d-0.3.7/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/COPYING.md` & `nx5d-0.3.7/COPYING.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/PKG-INFO` & `nx5d-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nx5d
-Version: 0.3.6
+Version: 0.3.7
 Summary: NX5 Duct Tape
 Author: Florin Boariu
 Author-email: florin.pt@rootshell.ro
 Project-URL: Source Code, https://gitlab.com/codedump2/nx5d
 Project-URL: Bug Tracker, https://gitlab.com/codedump2/nx5d/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `nx5d-0.3.6/README.md` & `nx5d-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/doc/mkdocs/concepts.md` & `nx5d-0.3.7/doc/mkdocs/concepts.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/doc/mkdocs/frame.svg` & `nx5d-0.3.7/doc/mkdocs/frame.svg`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/doc/mkdocs/index.md` & `nx5d-0.3.7/doc/mkdocs/index.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/doc/mkdocs/license.md` & `nx5d-0.3.7/doc/mkdocs/license.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/doc/mkdocs/module-nx.md` & `nx5d-0.3.7/doc/mkdocs/module-nx.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/doc/mkdocs/scan.svg` & `nx5d-0.3.7/doc/mkdocs/scan.svg`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/doc/mkdocs/streak1.svg` & `nx5d-0.3.7/doc/mkdocs/streak1.svg`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/doc/mkdocs/streak2.svg` & `nx5d-0.3.7/doc/mkdocs/streak2.svg`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/doc/mkdocs/tutorials/index.md` & `nx5d-0.3.7/doc/mkdocs/tutorials/index.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/doc/mkdocs/tutorials/kmc3-data-processing-howto/kmc3-data-processing-howto.md` & `nx5d-0.3.7/doc/mkdocs/tutorials/kmc3-data-processing-howto/kmc3-data-processing-howto.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_0.png` & `nx5d-0.3.7/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_0.png`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_1.png` & `nx5d-0.3.7/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_1.png`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_2.png` & `nx5d-0.3.7/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_2.png`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_33_0.png` & `nx5d-0.3.7/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_33_0.png`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_52_1.png` & `nx5d-0.3.7/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_52_1.png`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/doc/mkdocs/tutorials/scansource-howto/scansource-howto.md` & `nx5d-0.3.7/doc/mkdocs/tutorials/scansource-howto/scansource-howto.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/doc/mkdocs.yml` & `nx5d-0.3.7/doc/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/scratch.org` & `nx5d-0.3.7/scratch.org`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/setup.cfg` & `nx5d-0.3.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/src/nx5d/edf.py` & `nx5d-0.3.7/src/nx5d/edf.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/src/nx5d/h5like/petra3.py` & `nx5d-0.3.7/src/nx5d/h5like/petra3.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/src/nx5d/h5like/pypod.py` & `nx5d-0.3.7/src/nx5d/h5like/pypod.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/src/nx5d/h5like/spec.py` & `nx5d-0.3.7/src/nx5d/h5like/spec.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from silx.io.spech5 import SpecH5, SpecH5LazyNodeDataset, SpecH5NodeDataset
 from silx.io.commonh5 import Group as H5Group, SoftLink as H5SoftLink
 from h5py import File as H5File
 from os import path
 import tifffile
 import numpy as np
 
+import logging
+
 '''
 Provides a series of objects to mock an "ESRF dialect" of a HDF5-based Nexus
 data file for X-ray diffraction experiments for SPEC files.
 As an extra provision, detector data is loaded from external `.tiff` files
 with an easily computable path. This is typical for older installation of
 SPEC which couldn't handle and store large(-ish) 2D detector images.
 
@@ -64,21 +66,44 @@
     def __init__(self, *args, tiffPathFmt="{frameidx}.tiff", numFrames=0, **kwargs):
         super().__init__(*args, **kwargs)
         self._tiff_path_fmt = tiffPathFmt
         self._tiff_frames_no = int(numFrames)
 
 
     def _create_data(self):
-        #data = []
-        #for i in range(self._tiff_frames_no):
-        #    data.append( tifffile.imread(self._tiff_path_fmt.format(frameidx=i)) )
-        #return np.array(data)
-        return np.array([tifffile.imread(self._tiff_path_fmt.format(frameidx=i)) \
-                         for i in range(self._tiff_frames_no)])
-
+        data = []
+        shape = None
+        lasterr = None
+        missing = []
+        for i in range(self._tiff_frames_no):
+            try:
+                tiff = tifffile.imread(self._tiff_path_fmt.format(frameidx=i))
+                shape = tuple([s for s in tiff.shape])
+            except FileNotFoundError as e:
+                lasterr = e
+                if len(missing) == 0:
+                    logging.warning(str(e)+". Assuming bad frame, "
+                                    "similar errors will be suppressed.")
+                missing.append(i)
+                tiff = None
+            data.append(tiff)
+
+
+        # It happens a lot that individual files are missing, so
+        # we're just ignoring those and replace them with NaN arrays
+        # of the appropriate shape. But if we have no shape at this
+        # point, this means that _all_ TIFFs are missing. We
+        # want to get loud about that (don't we?...)
+        if shape is None:
+            logging.warning("Dataset had no frames at all.")
+            return np.array(np.NaN)
+        
+        return np.array([ (i if i is not None else np.full(shape, np.nan)) \
+                          for i in data])
+    
 
     def __getitem__(self, item):
         '''
         Apparently we can optimize this so that only a single file is
         loaded if not already initialized (...so we don't have to load
         the whole bunch for single-frame access). In that case, `item`
         is the index of the file, and all we have to do is plug it
```

### Comparing `nx5d-0.3.6/src/nx5d/h5like/tools.py` & `nx5d-0.3.7/src/nx5d/h5like/tools.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/src/nx5d/h5like/xfel.py` & `nx5d-0.3.7/src/nx5d/h5like/xfel.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/src/nx5d/nx.py` & `nx5d-0.3.7/src/nx5d/nx.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/src/nx5d/runlog.py` & `nx5d-0.3.7/src/nx5d/runlog.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/src/nx5d/scan.py` & `nx5d-0.3.7/src/nx5d/scan.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/src/nx5d/streaks.py` & `nx5d-0.3.7/src/nx5d/streaks.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/src/nx5d/xrd/ColonelSandersFinest.py` & `nx5d-0.3.7/src/nx5d/xrd/ColonelSandersFinest.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/src/nx5d/xrd/analysis.py` & `nx5d-0.3.7/src/nx5d/xrd/analysis.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/src/nx5d/xrd/esrf_id09.py` & `nx5d-0.3.7/src/nx5d/xrd/esrf_id09.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/src/nx5d/xrd/experiment-xpp.yml` & `nx5d-0.3.7/src/nx5d/xrd/experiment-xpp.yml`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/src/nx5d/xrd/experiment.py` & `nx5d-0.3.7/src/nx5d/xrd/experiment.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/src/nx5d/xrd/kmc3.py` & `nx5d-0.3.7/src/nx5d/xrd/kmc3.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/src/nx5d/xrd/roi.py` & `nx5d-0.3.7/src/nx5d/xrd/roi.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/src/nx5d/xrd/signal.py` & `nx5d-0.3.7/src/nx5d/xrd/signal.py`

 * *Files 2% similar despite different names*

```diff
@@ -274,21 +274,25 @@
 
     def __make_dataset(self, **dsets):
         ''' Creates an `xarray.Dataset` of data sets within `dsets`.
         The first dimension of all `dsets` is required to be the same.
         This is introduced as the first dimension in the `xarray` dataset,
         with the name "__index__".
         '''
-        
+
         tmp = next(iter(dsets.items()))
-        xdata = Dataset({'index': np.array(range(tmp[1].shape[0]))})
-        for k,p in dsets.items():
-            data = self.__arrayify(p, tmp[1].shape[0])
-            dims = ["index"] + ["%s_%d" % (k,i) for i in range(1,len(data.shape))]
-            xdata[k] = (dims, data)
+        try:
+            xdata = Dataset({'index': np.array(range(tmp[1].shape[0]))})
+            for k,p in dsets.items():
+                data = self.__arrayify(p, tmp[1].shape[0])
+                dims = ["index"] + ["%s_%d" % (k,i) for i in range(1,len(data.shape))]
+                xdata[k] = (dims, data)
+        except:
+            logging.error("Error with dataset: %r" % tmp)
+            raise
 
         return xdata
 
 
 
     def __2tuple(self, data, name=""):
         ''' Returns a 2-tuple (X, Y) from a variety of data sets:
```

### Comparing `nx5d-0.3.6/src/nx5d/xrd/xfel.py` & `nx5d-0.3.7/src/nx5d/xrd/xfel.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/src/nx5d/xrd/xraytest.py` & `nx5d-0.3.7/src/nx5d/xrd/xraytest.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/src/nx5d/xrd/xrd_helpers.py` & `nx5d-0.3.7/src/nx5d/xrd/xrd_helpers.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/src/nx5d.egg-info/PKG-INFO` & `nx5d-0.3.7/src/nx5d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nx5d
-Version: 0.3.6
+Version: 0.3.7
 Summary: NX5 Duct Tape
 Author: Florin Boariu
 Author-email: florin.pt@rootshell.ro
 Project-URL: Source Code, https://gitlab.com/codedump2/nx5d
 Project-URL: Bug Tracker, https://gitlab.com/codedump2/nx5d/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `nx5d-0.3.6/tests/fio_test.py` & `nx5d-0.3.7/tests/fio_test.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/pabst_test.py` & `nx5d-0.3.7/tests/pabst_test.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/pypod_test.py` & `nx5d-0.3.7/tests/pypod_test.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/runlog_test.py` & `nx5d-0.3.7/tests/runlog_test.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/fioh5/m3_2507_00342.fio` & `nx5d-0.3.7/tests/test_data/fioh5/m3_2507_00342.fio`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/fioh5/m3_2507_00744/lambda/m3_2507_00744_00000.nxs` & `nx5d-0.3.7/tests/test_data/fioh5/m3_2507_00744/lambda/m3_2507_00744_00000.nxs`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/fioh5/m3_2507_00744.fio` & `nx5d-0.3.7/tests/test_data/fioh5/m3_2507_00744.fio`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/runfile/run04.log` & `nx5d-0.3.7/tests/test_data/runfile/run04.log`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/runfile/run105.log` & `nx5d-0.3.7/tests/test_data/runfile/run105.log`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/runfile/run105_brokendata1.log` & `nx5d-0.3.7/tests/test_data/runfile/run105_brokendata1.log`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/runfile/run105_brokendata2.log` & `nx5d-0.3.7/tests/test_data/runfile/run105_brokendata2.log`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/runfile/run105_brokenheader.log` & `nx5d-0.3.7/tests/test_data/runfile/run105_brokenheader.log`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/runfile/run105_simple.log` & `nx5d-0.3.7/tests/test_data/runfile/run105_simple.log`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/runfile/short_run04.log` & `nx5d-0.3.7/tests/test_data/runfile/short_run04.log`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/runfile/short_run04_0001.edf` & `nx5d-0.3.7/tests/test_data/runfile/short_run04_0001.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/runfile/short_run04_0002.edf` & `nx5d-0.3.7/tests/test_data/runfile/short_run04_0002.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/runfile/short_run04_0003.edf` & `nx5d-0.3.7/tests/test_data/runfile/short_run04_0003.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/runfile/short_run04_0004.edf` & `nx5d-0.3.7/tests/test_data/runfile/short_run04_0004.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/runfile/short_run04_0005.edf` & `nx5d-0.3.7/tests/test_data/runfile/short_run04_0005.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/runfile/short_run04_0006.edf` & `nx5d-0.3.7/tests/test_data/runfile/short_run04_0006.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/runfile/short_run04_0007.edf` & `nx5d-0.3.7/tests/test_data/runfile/short_run04_0007.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/runfile/short_run04_0008.edf` & `nx5d-0.3.7/tests/test_data/runfile/short_run04_0008.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/runfile/short_run04_0009.edf` & `nx5d-0.3.7/tests/test_data/runfile/short_run04_0009.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/runfile/short_run04_0010.edf` & `nx5d-0.3.7/tests/test_data/runfile/short_run04_0010.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/runfile/short_run04_0011.edf` & `nx5d-0.3.7/tests/test_data/runfile/short_run04_0011.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/runfile/short_run04_0012.edf` & `nx5d-0.3.7/tests/test_data/runfile/short_run04_0012.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/runfile/short_run04_0013.edf` & `nx5d-0.3.7/tests/test_data/runfile/short_run04_0013.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/runfile/short_run04_0014.edf` & `nx5d-0.3.7/tests/test_data/runfile/short_run04_0014.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/runfile/short_run04_0015.edf` & `nx5d-0.3.7/tests/test_data/runfile/short_run04_0015.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/runfile/short_run04_0016.edf` & `nx5d-0.3.7/tests/test_data/runfile/short_run04_0016.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/runfile/short_run04_0017.edf` & `nx5d-0.3.7/tests/test_data/runfile/short_run04_0017.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/runfile/short_run04_0018.edf` & `nx5d-0.3.7/tests/test_data/runfile/short_run04_0018.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/runfile/short_run04_0019.edf` & `nx5d-0.3.7/tests/test_data/runfile/short_run04_0019.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/runfile/short_run04_0020.edf` & `nx5d-0.3.7/tests/test_data/runfile/short_run04_0020.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/runfile/short_run04_0021.edf` & `nx5d-0.3.7/tests/test_data/runfile/short_run04_0021.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/runfile/short_run04_0022.edf` & `nx5d-0.3.7/tests/test_data/runfile/short_run04_0022.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/runfile/short_run04_0023.edf` & `nx5d-0.3.7/tests/test_data/runfile/short_run04_0023.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/runfile/short_run04_0024.edf` & `nx5d-0.3.7/tests/test_data/runfile/short_run04_0024.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/runfile/short_run04_0025.edf` & `nx5d-0.3.7/tests/test_data/runfile/short_run04_0025.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/runfile/short_run04_0026.edf` & `nx5d-0.3.7/tests/test_data/runfile/short_run04_0026.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/runfile/short_run04_0027.edf` & `nx5d-0.3.7/tests/test_data/runfile/short_run04_0027.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/runfile/short_run04_0028.edf` & `nx5d-0.3.7/tests/test_data/runfile/short_run04_0028.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/runfile/short_run04_0029.edf` & `nx5d-0.3.7/tests/test_data/runfile/short_run04_0029.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/runfile/short_run04_0030.edf` & `nx5d-0.3.7/tests/test_data/runfile/short_run04_0030.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/runfile/short_run04_0031.edf` & `nx5d-0.3.7/tests/test_data/runfile/short_run04_0031.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/runfile/short_run04_0032.edf` & `nx5d-0.3.7/tests/test_data/runfile/short_run04_0032.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/runfile/short_run04_0033.edf` & `nx5d-0.3.7/tests/test_data/runfile/short_run04_0033.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/runfile/short_run04_0034.edf` & `nx5d-0.3.7/tests/test_data/runfile/short_run04_0034.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/runfile/short_run04_0035.edf` & `nx5d-0.3.7/tests/test_data/runfile/short_run04_0035.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/runfile/short_run04_0036.edf` & `nx5d-0.3.7/tests/test_data/runfile/short_run04_0036.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/runfile/short_run04_0037.edf` & `nx5d-0.3.7/tests/test_data/runfile/short_run04_0037.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/231-cw7-12083-roessle.spec` & `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/231-cw7-12083-roessle.spec`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00002/231-cw7-12083-roessle_2_0.tif` & `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00002/231-cw7-12083-roessle_2_0.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_0.tif` & `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_0.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_1.tif` & `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_1.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_10.tif` & `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_10.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_11.tif` & `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_11.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_12.tif` & `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_12.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_13.tif` & `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_13.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_14.tif` & `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_14.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_15.tif` & `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_15.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_16.tif` & `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_16.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_17.tif` & `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_17.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_18.tif` & `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_18.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_19.tif` & `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_19.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_2.tif` & `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_2.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_20.tif` & `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_20.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_21.tif` & `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_21.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_22.tif` & `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_22.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_23.tif` & `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_23.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_24.tif` & `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_24.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_25.tif` & `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_25.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_26.tif` & `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_26.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_27.tif` & `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_27.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_28.tif` & `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_28.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_29.tif` & `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_29.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_3.tif` & `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_3.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_30.tif` & `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_30.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_31.tif` & `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_31.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_32.tif` & `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_32.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_33.tif` & `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_33.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_34.tif` & `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_34.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_35.tif` & `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_35.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_36.tif` & `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_36.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_37.tif` & `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_37.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_38.tif` & `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_38.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_39.tif` & `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_39.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_4.tif` & `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_4.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_40.tif` & `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_40.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_5.tif` & `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_5.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_6.tif` & `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_6.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_7.tif` & `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_7.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_8.tif` & `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_8.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_9.tif` & `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_9.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/xfel_test.py` & `nx5d-0.3.7/tests/xfel_test.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.6/tests/xrd_data_test.py` & `nx5d-0.3.7/tests/xrd_data_test.py`

 * *Files identical despite different names*

