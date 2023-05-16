# Comparing `tmp/pysradb-2.0.1.tar.gz` & `tmp/pysradb-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysradb-2.0.1.tar", last modified: Sat Mar 18 22:40:38 2023, max compression
+gzip compressed data, was "pysradb-2.0.2.tar", last modified: Sun Apr  9 16:25:51 2023, max compression
```

## Comparing `pysradb-2.0.1.tar` & `pysradb-2.0.2.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxrwxr-x   0 saket     (1000) saket     (1000)        0 2023-03-18 22:40:38.949769 pysradb-2.0.1/
--rw-rw-r--   0 saket     (1000) saket     (1000)      382 2023-03-18 22:39:30.000000 pysradb-2.0.1/AUTHORS.rst
--rw-rw-r--   0 saket     (1000) saket     (1000)     3596 2023-03-18 22:39:30.000000 pysradb-2.0.1/CONTRIBUTING.rst
--rw-rw-r--   0 saket     (1000) saket     (1000)     9260 2023-03-18 22:39:57.000000 pysradb-2.0.1/HISTORY.rst
--rw-rw-r--   0 saket     (1000) saket     (1000)     1520 2023-03-18 22:39:30.000000 pysradb-2.0.1/LICENSE
--rw-rw-r--   0 saket     (1000) saket     (1000)      348 2023-03-18 22:39:30.000000 pysradb-2.0.1/MANIFEST.in
--rw-rw-r--   0 saket     (1000) saket     (1000)    28589 2023-03-18 22:40:38.949769 pysradb-2.0.1/PKG-INFO
--rw-rw-r--   0 saket     (1000) saket     (1000)    18355 2023-03-18 22:39:57.000000 pysradb-2.0.1/README.rst
-drwxrwxr-x   0 saket     (1000) saket     (1000)        0 2023-03-18 22:40:38.933769 pysradb-2.0.1/docs/
--rw-rw-r--   0 saket     (1000) saket     (1000)      608 2023-03-18 22:39:30.000000 pysradb-2.0.1/docs/Makefile
-drwxrwxr-x   0 saket     (1000) saket     (1000)        0 2023-03-18 22:40:38.937769 pysradb-2.0.1/docs/_static/
--rw-rw-r--   0 saket     (1000) saket     (1000)    35323 2023-03-18 22:39:30.000000 pysradb-2.0.1/docs/_static/e1.png
--rw-rw-r--   0 saket     (1000) saket     (1000)    58243 2023-03-18 22:39:30.000000 pysradb-2.0.1/docs/_static/e2.png
--rw-rw-r--   0 saket     (1000) saket     (1000)    27031 2023-03-18 22:39:30.000000 pysradb-2.0.1/docs/_static/e3.png
--rw-rw-r--   0 saket     (1000) saket     (1000)    27736 2023-03-18 22:39:30.000000 pysradb-2.0.1/docs/_static/pysradb_v3.png
--rw-rw-r--   0 saket     (1000) saket     (1000)       28 2023-03-18 22:39:30.000000 pysradb-2.0.1/docs/authors.rst
--rw-rw-r--   0 saket     (1000) saket     (1000)    15534 2023-03-18 22:39:30.000000 pysradb-2.0.1/docs/case_studies.rst
--rw-rw-r--   0 saket     (1000) saket     (1000)     9781 2023-03-18 22:39:30.000000 pysradb-2.0.1/docs/cmdline.rst
-drwxrwxr-x   0 saket     (1000) saket     (1000)        0 2023-03-18 22:40:38.937769 pysradb-2.0.1/docs/commands/
--rw-rw-r--   0 saket     (1000) saket     (1000)      815 2023-03-18 22:39:30.000000 pysradb-2.0.1/docs/commands/download.rst
--rw-rw-r--   0 saket     (1000) saket     (1000)     1652 2023-03-18 22:39:30.000000 pysradb-2.0.1/docs/commands/gse-to-gsm.rst
--rw-rw-r--   0 saket     (1000) saket     (1000)     1935 2023-03-18 22:39:30.000000 pysradb-2.0.1/docs/commands/gse-to-srp.rst
--rw-rw-r--   0 saket     (1000) saket     (1000)     2751 2023-03-18 22:39:30.000000 pysradb-2.0.1/docs/commands/metadata.rst
--rw-rw-r--   0 saket     (1000) saket     (1000)   125097 2023-03-18 22:39:30.000000 pysradb-2.0.1/docs/commands/search.rst
--rw-rw-r--   0 saket     (1000) saket     (1000)     1456 2023-03-18 22:39:30.000000 pysradb-2.0.1/docs/commands/srp-to-gse.rst
--rw-rw-r--   0 saket     (1000) saket     (1000)     2436 2023-03-18 22:39:30.000000 pysradb-2.0.1/docs/commands/srp-to-srr.rst
--rw-rw-r--   0 saket     (1000) saket     (1000)     1752 2023-03-18 22:39:30.000000 pysradb-2.0.1/docs/commands/srp-to-srs.rst
--rw-rw-r--   0 saket     (1000) saket     (1000)     2459 2023-03-18 22:39:30.000000 pysradb-2.0.1/docs/commands/srp-to-srx.rst
--rw-rw-r--   0 saket     (1000) saket     (1000)     1674 2023-03-18 22:39:30.000000 pysradb-2.0.1/docs/commands/srr-to-srs.rst
--rw-rw-r--   0 saket     (1000) saket     (1000)     1535 2023-03-18 22:39:30.000000 pysradb-2.0.1/docs/commands/srr-to-srx.rst
--rw-rw-r--   0 saket     (1000) saket     (1000)     1361 2023-03-18 22:39:30.000000 pysradb-2.0.1/docs/commands/srs-to-srx.rst
--rw-rw-r--   0 saket     (1000) saket     (1000)     1381 2023-03-18 22:39:30.000000 pysradb-2.0.1/docs/commands/srx-to-srr.rst
--rw-rw-r--   0 saket     (1000) saket     (1000)     1370 2023-03-18 22:39:30.000000 pysradb-2.0.1/docs/commands/srx-to-srs.rst
--rw-rw-r--   0 saket     (1000) saket     (1000)      396 2023-03-18 22:39:30.000000 pysradb-2.0.1/docs/commands.rst
--rw-rw-r--   0 saket     (1000) saket     (1000)     6001 2023-03-18 22:39:30.000000 pysradb-2.0.1/docs/conf.py
--rw-rw-r--   0 saket     (1000) saket     (1000)       33 2023-03-18 22:39:30.000000 pysradb-2.0.1/docs/contributing.rst
--rw-rw-r--   0 saket     (1000) saket     (1000)       28 2023-03-18 22:39:30.000000 pysradb-2.0.1/docs/history.rst
--rw-rw-r--   0 saket     (1000) saket     (1000)    21032 2023-03-18 22:39:30.000000 pysradb-2.0.1/docs/index.rst
--rw-rw-r--   0 saket     (1000) saket     (1000)     1623 2023-03-18 22:39:30.000000 pysradb-2.0.1/docs/installation.rst
--rw-rw-r--   0 saket     (1000) saket     (1000)      769 2023-03-18 22:39:30.000000 pysradb-2.0.1/docs/make.bat
--rw-rw-r--   0 saket     (1000) saket     (1000)       58 2023-03-18 22:39:30.000000 pysradb-2.0.1/docs/modules.rst
--rw-rw-r--   0 saket     (1000) saket     (1000)     1640 2023-03-18 22:39:30.000000 pysradb-2.0.1/docs/pysradb.rst
--rw-rw-r--   0 saket     (1000) saket     (1000)    13150 2023-03-18 22:39:30.000000 pysradb-2.0.1/docs/python-api-usage.rst
--rw-rw-r--   0 saket     (1000) saket     (1000)    62700 2023-03-18 22:39:30.000000 pysradb-2.0.1/docs/quickstart.rst
-drwxrwxr-x   0 saket     (1000) saket     (1000)        0 2023-03-18 22:40:38.937769 pysradb-2.0.1/pysradb/
--rw-rw-r--   0 saket     (1000) saket     (1000)      365 2023-03-18 22:39:57.000000 pysradb-2.0.1/pysradb/__init__.py
--rw-rw-r--   0 saket     (1000) saket     (1000)     4089 2023-03-18 22:39:30.000000 pysradb-2.0.1/pysradb/basedb.py
--rw-rw-r--   0 saket     (1000) saket     (1000)    44751 2023-03-18 22:39:30.000000 pysradb-2.0.1/pysradb/cli.py
--rw-rw-r--   0 saket     (1000) saket     (1000)     4949 2023-03-18 22:39:30.000000 pysradb-2.0.1/pysradb/download.py
--rw-rw-r--   0 saket     (1000) saket     (1000)      778 2023-03-18 22:39:30.000000 pysradb-2.0.1/pysradb/exceptions.py
--rw-rw-r--   0 saket     (1000) saket     (1000)     7987 2023-03-18 22:39:30.000000 pysradb-2.0.1/pysradb/filter_attrs.py
--rw-rw-r--   0 saket     (1000) saket     (1000)     5176 2023-03-18 22:39:30.000000 pysradb-2.0.1/pysradb/geodb.py
--rw-rw-r--   0 saket     (1000) saket     (1000)     3551 2023-03-18 22:39:30.000000 pysradb-2.0.1/pysradb/geoweb.py
--rw-rw-r--   0 saket     (1000) saket     (1000)    71756 2023-03-18 22:39:30.000000 pysradb-2.0.1/pysradb/search.py
--rw-rw-r--   0 saket     (1000) saket     (1000)    48559 2023-03-18 22:39:57.000000 pysradb-2.0.1/pysradb/sradb.py
--rw-rw-r--   0 saket     (1000) saket     (1000)    37694 2023-03-18 22:39:57.000000 pysradb-2.0.1/pysradb/sraweb.py
--rw-rw-r--   0 saket     (1000) saket     (1000)   386928 2023-03-18 22:39:30.000000 pysradb-2.0.1/pysradb/taxid2name.py
--rw-rw-r--   0 saket     (1000) saket     (1000)     7539 2023-03-18 22:39:30.000000 pysradb-2.0.1/pysradb/utils.py
-drwxrwxr-x   0 saket     (1000) saket     (1000)        0 2023-03-18 22:40:38.937769 pysradb-2.0.1/pysradb.egg-info/
--rw-rw-r--   0 saket     (1000) saket     (1000)    28589 2023-03-18 22:40:38.000000 pysradb-2.0.1/pysradb.egg-info/PKG-INFO
--rw-rw-r--   0 saket     (1000) saket     (1000)     2542 2023-03-18 22:40:38.000000 pysradb-2.0.1/pysradb.egg-info/SOURCES.txt
--rw-rw-r--   0 saket     (1000) saket     (1000)        1 2023-03-18 22:40:38.000000 pysradb-2.0.1/pysradb.egg-info/dependency_links.txt
--rw-rw-r--   0 saket     (1000) saket     (1000)       51 2023-03-18 22:40:38.000000 pysradb-2.0.1/pysradb.egg-info/entry_points.txt
--rw-rw-r--   0 saket     (1000) saket     (1000)        1 2023-03-18 22:40:37.000000 pysradb-2.0.1/pysradb.egg-info/not-zip-safe
--rw-rw-r--   0 saket     (1000) saket     (1000)       94 2023-03-18 22:40:38.000000 pysradb-2.0.1/pysradb.egg-info/requires.txt
--rw-rw-r--   0 saket     (1000) saket     (1000)        8 2023-03-18 22:40:38.000000 pysradb-2.0.1/pysradb.egg-info/top_level.txt
--rw-rw-r--   0 saket     (1000) saket     (1000)       94 2023-03-18 22:39:30.000000 pysradb-2.0.1/requirements.txt
--rw-rw-r--   0 saket     (1000) saket     (1000)      709 2023-03-18 22:40:38.949769 pysradb-2.0.1/setup.cfg
--rw-rw-r--   0 saket     (1000) saket     (1000)     1695 2023-03-18 22:39:57.000000 pysradb-2.0.1/setup.py
-drwxrwxr-x   0 saket     (1000) saket     (1000)        0 2023-03-18 22:40:38.941769 pysradb-2.0.1/tests/
--rw-rw-r--   0 saket     (1000) saket     (1000)      901 2023-03-18 22:39:30.000000 pysradb-2.0.1/tests/_test_geodb.py
--rw-rw-r--   0 saket     (1000) saket     (1000)     3335 2023-03-18 22:39:30.000000 pysradb-2.0.1/tests/_test_pcli.py
--rw-rw-r--   0 saket     (1000) saket     (1000)     6102 2023-03-18 22:39:30.000000 pysradb-2.0.1/tests/_test_sradb.py
--rw-rw-r--   0 saket     (1000) saket     (1000)      626 2023-03-18 22:39:30.000000 pysradb-2.0.1/tests/conftest.py
-drwxrwxr-x   0 saket     (1000) saket     (1000)        0 2023-03-18 22:40:38.933769 pysradb-2.0.1/tests/data/
-drwxrwxr-x   0 saket     (1000) saket     (1000)        0 2023-03-18 22:40:38.949769 pysradb-2.0.1/tests/data/test_search/
--rw-rw-r--   0 saket     (1000) saket     (1000)      784 2023-03-18 22:39:30.000000 pysradb-2.0.1/tests/data/test_search/ena_search_test1.txt
--rw-rw-r--   0 saket     (1000) saket     (1000)    10994 2023-03-18 22:39:30.000000 pysradb-2.0.1/tests/data/test_search/ena_test_verbosity_0.csv
--rw-rw-r--   0 saket     (1000) saket     (1000)   821724 2023-03-18 22:39:30.000000 pysradb-2.0.1/tests/data/test_search/ena_test_verbosity_0.json
--rw-rw-r--   0 saket     (1000) saket     (1000)   132839 2023-03-18 22:39:30.000000 pysradb-2.0.1/tests/data/test_search/ena_test_verbosity_1.csv
--rw-rw-r--   0 saket     (1000) saket     (1000)   821724 2023-03-18 22:39:30.000000 pysradb-2.0.1/tests/data/test_search/ena_test_verbosity_1.json
--rw-rw-r--   0 saket     (1000) saket     (1000)   415835 2023-03-18 22:39:30.000000 pysradb-2.0.1/tests/data/test_search/ena_test_verbosity_2.csv
--rw-rw-r--   0 saket     (1000) saket     (1000)   821724 2023-03-18 22:39:30.000000 pysradb-2.0.1/tests/data/test_search/ena_test_verbosity_2.json
--rw-rw-r--   0 saket     (1000) saket     (1000)  2188813 2023-03-18 22:39:30.000000 pysradb-2.0.1/tests/data/test_search/ena_test_verbosity_3.csv
--rw-rw-r--   0 saket     (1000) saket     (1000)  4334941 2023-03-18 22:39:30.000000 pysradb-2.0.1/tests/data/test_search/ena_test_verbosity_3.json
--rw-rw-r--   0 saket     (1000) saket     (1000)      857 2023-03-18 22:39:30.000000 pysradb-2.0.1/tests/data/test_search/geo_search_test1.txt
--rw-rw-r--   0 saket     (1000) saket     (1000)       19 2023-03-18 22:39:30.000000 pysradb-2.0.1/tests/data/test_search/sra_search_test1.txt
--rw-rw-r--   0 saket     (1000) saket     (1000)   648777 2023-03-18 22:39:30.000000 pysradb-2.0.1/tests/data/test_search/sra_test.xml
--rw-rw-r--   0 saket     (1000) saket     (1000)       25 2023-03-18 22:39:30.000000 pysradb-2.0.1/tests/data/test_search/sra_test_2_verbosity_0.csv
--rw-rw-r--   0 saket     (1000) saket     (1000)       76 2023-03-18 22:39:30.000000 pysradb-2.0.1/tests/data/test_search/sra_test_2_verbosity_1.csv
--rw-rw-r--   0 saket     (1000) saket     (1000)      516 2023-03-18 22:39:30.000000 pysradb-2.0.1/tests/data/test_search/sra_test_2_verbosity_2.csv
--rw-rw-r--   0 saket     (1000) saket     (1000)     9398 2023-03-18 22:39:30.000000 pysradb-2.0.1/tests/data/test_search/sra_test_2_verbosity_3.csv
--rw-rw-r--   0 saket     (1000) saket     (1000)    10356 2023-03-18 22:39:30.000000 pysradb-2.0.1/tests/data/test_search/sra_test_ERS3331676.xml
--rw-rw-r--   0 saket     (1000) saket     (1000)     1033 2023-03-18 22:39:30.000000 pysradb-2.0.1/tests/data/test_search/sra_test_verbosity_0.csv
--rw-rw-r--   0 saket     (1000) saket     (1000)     6333 2023-03-18 22:39:30.000000 pysradb-2.0.1/tests/data/test_search/sra_test_verbosity_1.csv
--rw-rw-r--   0 saket     (1000) saket     (1000)    20039 2023-03-18 22:39:30.000000 pysradb-2.0.1/tests/data/test_search/sra_test_verbosity_2.csv
--rw-rw-r--   0 saket     (1000) saket     (1000)   329879 2023-03-18 22:39:30.000000 pysradb-2.0.1/tests/data/test_search/sra_test_verbosity_3.csv
--rw-rw-r--   0 saket     (1000) saket     (1000)       14 2023-03-18 22:39:30.000000 pysradb-2.0.1/tests/data/test_search/sra_uids.txt
--rw-rw-r--   0 saket     (1000) saket     (1000)     1162 2023-03-18 22:39:30.000000 pysradb-2.0.1/tests/test_geoweb.py
--rw-rw-r--   0 saket     (1000) saket     (1000)    31360 2023-03-18 22:39:30.000000 pysradb-2.0.1/tests/test_search.py
--rw-rw-r--   0 saket     (1000) saket     (1000)      572 2023-03-18 22:39:30.000000 pysradb-2.0.1/tests/test_sradb.py
--rw-rw-r--   0 saket     (1000) saket     (1000)     7898 2023-03-18 22:39:57.000000 pysradb-2.0.1/tests/test_sraweb.py
--rw-rw-r--   0 saket     (1000) saket     (1000)      547 2023-03-18 22:39:30.000000 pysradb-2.0.1/tests/test_utils.py
+drwxrwxr-x   0 saket     (1000) saket     (1000)        0 2023-04-09 16:25:51.364595 pysradb-2.0.2/
+-rw-rw-r--   0 saket     (1000) saket     (1000)      382 2023-03-18 22:39:30.000000 pysradb-2.0.2/AUTHORS.rst
+-rw-rw-r--   0 saket     (1000) saket     (1000)     3596 2023-03-18 22:39:30.000000 pysradb-2.0.2/CONTRIBUTING.rst
+-rw-rw-r--   0 saket     (1000) saket     (1000)     9542 2023-04-09 16:23:52.000000 pysradb-2.0.2/HISTORY.rst
+-rw-rw-r--   0 saket     (1000) saket     (1000)     1520 2023-03-18 22:39:30.000000 pysradb-2.0.2/LICENSE
+-rw-rw-r--   0 saket     (1000) saket     (1000)      348 2023-03-18 22:39:30.000000 pysradb-2.0.2/MANIFEST.in
+-rw-rw-r--   0 saket     (1000) saket     (1000)    28873 2023-04-09 16:25:51.364595 pysradb-2.0.2/PKG-INFO
+-rw-rw-r--   0 saket     (1000) saket     (1000)    18357 2023-04-03 02:51:47.000000 pysradb-2.0.2/README.rst
+drwxrwxr-x   0 saket     (1000) saket     (1000)        0 2023-04-09 16:25:51.352595 pysradb-2.0.2/docs/
+-rw-rw-r--   0 saket     (1000) saket     (1000)      608 2023-03-18 22:39:30.000000 pysradb-2.0.2/docs/Makefile
+drwxrwxr-x   0 saket     (1000) saket     (1000)        0 2023-04-09 16:25:51.352595 pysradb-2.0.2/docs/_static/
+-rw-rw-r--   0 saket     (1000) saket     (1000)    35323 2023-03-18 22:39:30.000000 pysradb-2.0.2/docs/_static/e1.png
+-rw-rw-r--   0 saket     (1000) saket     (1000)    58243 2023-03-18 22:39:30.000000 pysradb-2.0.2/docs/_static/e2.png
+-rw-rw-r--   0 saket     (1000) saket     (1000)    27031 2023-03-18 22:39:30.000000 pysradb-2.0.2/docs/_static/e3.png
+-rw-rw-r--   0 saket     (1000) saket     (1000)    27736 2023-03-18 22:39:30.000000 pysradb-2.0.2/docs/_static/pysradb_v3.png
+-rw-rw-r--   0 saket     (1000) saket     (1000)       28 2023-03-18 22:39:30.000000 pysradb-2.0.2/docs/authors.rst
+-rw-rw-r--   0 saket     (1000) saket     (1000)    15534 2023-03-18 22:39:30.000000 pysradb-2.0.2/docs/case_studies.rst
+-rw-rw-r--   0 saket     (1000) saket     (1000)     9781 2023-03-18 22:39:30.000000 pysradb-2.0.2/docs/cmdline.rst
+drwxrwxr-x   0 saket     (1000) saket     (1000)        0 2023-04-09 16:25:51.352595 pysradb-2.0.2/docs/commands/
+-rw-rw-r--   0 saket     (1000) saket     (1000)      815 2023-03-18 22:39:30.000000 pysradb-2.0.2/docs/commands/download.rst
+-rw-rw-r--   0 saket     (1000) saket     (1000)     1652 2023-03-18 22:39:30.000000 pysradb-2.0.2/docs/commands/gse-to-gsm.rst
+-rw-rw-r--   0 saket     (1000) saket     (1000)     1935 2023-03-18 22:39:30.000000 pysradb-2.0.2/docs/commands/gse-to-srp.rst
+-rw-rw-r--   0 saket     (1000) saket     (1000)     2751 2023-03-18 22:39:30.000000 pysradb-2.0.2/docs/commands/metadata.rst
+-rw-rw-r--   0 saket     (1000) saket     (1000)   125097 2023-03-18 22:39:30.000000 pysradb-2.0.2/docs/commands/search.rst
+-rw-rw-r--   0 saket     (1000) saket     (1000)     1456 2023-03-18 22:39:30.000000 pysradb-2.0.2/docs/commands/srp-to-gse.rst
+-rw-rw-r--   0 saket     (1000) saket     (1000)     2436 2023-03-18 22:39:30.000000 pysradb-2.0.2/docs/commands/srp-to-srr.rst
+-rw-rw-r--   0 saket     (1000) saket     (1000)     1752 2023-03-18 22:39:30.000000 pysradb-2.0.2/docs/commands/srp-to-srs.rst
+-rw-rw-r--   0 saket     (1000) saket     (1000)     2459 2023-03-18 22:39:30.000000 pysradb-2.0.2/docs/commands/srp-to-srx.rst
+-rw-rw-r--   0 saket     (1000) saket     (1000)     1674 2023-03-18 22:39:30.000000 pysradb-2.0.2/docs/commands/srr-to-srs.rst
+-rw-rw-r--   0 saket     (1000) saket     (1000)     1535 2023-03-18 22:39:30.000000 pysradb-2.0.2/docs/commands/srr-to-srx.rst
+-rw-rw-r--   0 saket     (1000) saket     (1000)     1361 2023-03-18 22:39:30.000000 pysradb-2.0.2/docs/commands/srs-to-srx.rst
+-rw-rw-r--   0 saket     (1000) saket     (1000)     1381 2023-03-18 22:39:30.000000 pysradb-2.0.2/docs/commands/srx-to-srr.rst
+-rw-rw-r--   0 saket     (1000) saket     (1000)     1370 2023-03-18 22:39:30.000000 pysradb-2.0.2/docs/commands/srx-to-srs.rst
+-rw-rw-r--   0 saket     (1000) saket     (1000)      396 2023-03-18 22:39:30.000000 pysradb-2.0.2/docs/commands.rst
+-rw-rw-r--   0 saket     (1000) saket     (1000)     6001 2023-03-18 22:39:30.000000 pysradb-2.0.2/docs/conf.py
+-rw-rw-r--   0 saket     (1000) saket     (1000)       33 2023-03-18 22:39:30.000000 pysradb-2.0.2/docs/contributing.rst
+-rw-rw-r--   0 saket     (1000) saket     (1000)       28 2023-03-18 22:39:30.000000 pysradb-2.0.2/docs/history.rst
+-rw-rw-r--   0 saket     (1000) saket     (1000)    21032 2023-03-18 22:39:30.000000 pysradb-2.0.2/docs/index.rst
+-rw-rw-r--   0 saket     (1000) saket     (1000)     1623 2023-03-18 22:39:30.000000 pysradb-2.0.2/docs/installation.rst
+-rw-rw-r--   0 saket     (1000) saket     (1000)      769 2023-03-18 22:39:30.000000 pysradb-2.0.2/docs/make.bat
+-rw-rw-r--   0 saket     (1000) saket     (1000)       58 2023-03-18 22:39:30.000000 pysradb-2.0.2/docs/modules.rst
+-rw-rw-r--   0 saket     (1000) saket     (1000)     1640 2023-03-18 22:39:30.000000 pysradb-2.0.2/docs/pysradb.rst
+-rw-rw-r--   0 saket     (1000) saket     (1000)    13150 2023-03-18 22:39:30.000000 pysradb-2.0.2/docs/python-api-usage.rst
+-rw-rw-r--   0 saket     (1000) saket     (1000)    62700 2023-03-18 22:39:30.000000 pysradb-2.0.2/docs/quickstart.rst
+drwxrwxr-x   0 saket     (1000) saket     (1000)        0 2023-04-09 16:25:51.352595 pysradb-2.0.2/pysradb/
+-rw-rw-r--   0 saket     (1000) saket     (1000)      365 2023-04-09 16:24:32.000000 pysradb-2.0.2/pysradb/__init__.py
+-rw-rw-r--   0 saket     (1000) saket     (1000)     4089 2023-03-18 22:39:30.000000 pysradb-2.0.2/pysradb/basedb.py
+-rw-rw-r--   0 saket     (1000) saket     (1000)    44751 2023-03-18 22:39:30.000000 pysradb-2.0.2/pysradb/cli.py
+-rw-rw-r--   0 saket     (1000) saket     (1000)     4949 2023-03-18 22:39:30.000000 pysradb-2.0.2/pysradb/download.py
+-rw-rw-r--   0 saket     (1000) saket     (1000)      778 2023-03-18 22:39:30.000000 pysradb-2.0.2/pysradb/exceptions.py
+-rw-rw-r--   0 saket     (1000) saket     (1000)     7987 2023-03-18 22:39:30.000000 pysradb-2.0.2/pysradb/filter_attrs.py
+-rw-rw-r--   0 saket     (1000) saket     (1000)     5176 2023-03-18 22:39:30.000000 pysradb-2.0.2/pysradb/geodb.py
+-rw-rw-r--   0 saket     (1000) saket     (1000)     3551 2023-03-18 22:39:30.000000 pysradb-2.0.2/pysradb/geoweb.py
+-rw-rw-r--   0 saket     (1000) saket     (1000)    71756 2023-04-09 16:13:04.000000 pysradb-2.0.2/pysradb/search.py
+-rw-rw-r--   0 saket     (1000) saket     (1000)    48559 2023-03-18 22:39:57.000000 pysradb-2.0.2/pysradb/sradb.py
+-rw-rw-r--   0 saket     (1000) saket     (1000)    39719 2023-04-09 04:18:53.000000 pysradb-2.0.2/pysradb/sraweb.py
+-rw-rw-r--   0 saket     (1000) saket     (1000)   386928 2023-03-18 22:39:30.000000 pysradb-2.0.2/pysradb/taxid2name.py
+-rw-rw-r--   0 saket     (1000) saket     (1000)     7539 2023-03-18 22:39:30.000000 pysradb-2.0.2/pysradb/utils.py
+drwxrwxr-x   0 saket     (1000) saket     (1000)        0 2023-04-09 16:25:51.352595 pysradb-2.0.2/pysradb.egg-info/
+-rw-rw-r--   0 saket     (1000) saket     (1000)    28873 2023-04-09 16:25:51.000000 pysradb-2.0.2/pysradb.egg-info/PKG-INFO
+-rw-rw-r--   0 saket     (1000) saket     (1000)     2542 2023-04-09 16:25:51.000000 pysradb-2.0.2/pysradb.egg-info/SOURCES.txt
+-rw-rw-r--   0 saket     (1000) saket     (1000)        1 2023-04-09 16:25:51.000000 pysradb-2.0.2/pysradb.egg-info/dependency_links.txt
+-rw-rw-r--   0 saket     (1000) saket     (1000)       51 2023-04-09 16:25:51.000000 pysradb-2.0.2/pysradb.egg-info/entry_points.txt
+-rw-rw-r--   0 saket     (1000) saket     (1000)        1 2023-04-09 16:25:50.000000 pysradb-2.0.2/pysradb.egg-info/not-zip-safe
+-rw-rw-r--   0 saket     (1000) saket     (1000)       94 2023-04-09 16:25:51.000000 pysradb-2.0.2/pysradb.egg-info/requires.txt
+-rw-rw-r--   0 saket     (1000) saket     (1000)        8 2023-04-09 16:25:51.000000 pysradb-2.0.2/pysradb.egg-info/top_level.txt
+-rw-rw-r--   0 saket     (1000) saket     (1000)       94 2023-03-18 22:39:30.000000 pysradb-2.0.2/requirements.txt
+-rw-rw-r--   0 saket     (1000) saket     (1000)      709 2023-04-09 16:25:51.364595 pysradb-2.0.2/setup.cfg
+-rw-rw-r--   0 saket     (1000) saket     (1000)     1695 2023-04-09 16:24:32.000000 pysradb-2.0.2/setup.py
+drwxrwxr-x   0 saket     (1000) saket     (1000)        0 2023-04-09 16:25:51.356595 pysradb-2.0.2/tests/
+-rw-rw-r--   0 saket     (1000) saket     (1000)      901 2023-03-18 22:39:30.000000 pysradb-2.0.2/tests/_test_geodb.py
+-rw-rw-r--   0 saket     (1000) saket     (1000)     3335 2023-03-18 22:39:30.000000 pysradb-2.0.2/tests/_test_pcli.py
+-rw-rw-r--   0 saket     (1000) saket     (1000)     6102 2023-03-18 22:39:30.000000 pysradb-2.0.2/tests/_test_sradb.py
+-rw-rw-r--   0 saket     (1000) saket     (1000)      626 2023-03-18 22:39:30.000000 pysradb-2.0.2/tests/conftest.py
+drwxrwxr-x   0 saket     (1000) saket     (1000)        0 2023-04-09 16:25:51.348595 pysradb-2.0.2/tests/data/
+drwxrwxr-x   0 saket     (1000) saket     (1000)        0 2023-04-09 16:25:51.364595 pysradb-2.0.2/tests/data/test_search/
+-rw-rw-r--   0 saket     (1000) saket     (1000)      784 2023-03-18 22:39:30.000000 pysradb-2.0.2/tests/data/test_search/ena_search_test1.txt
+-rw-rw-r--   0 saket     (1000) saket     (1000)    10994 2023-03-18 22:39:30.000000 pysradb-2.0.2/tests/data/test_search/ena_test_verbosity_0.csv
+-rw-rw-r--   0 saket     (1000) saket     (1000)   821724 2023-03-18 22:39:30.000000 pysradb-2.0.2/tests/data/test_search/ena_test_verbosity_0.json
+-rw-rw-r--   0 saket     (1000) saket     (1000)   132839 2023-03-18 22:39:30.000000 pysradb-2.0.2/tests/data/test_search/ena_test_verbosity_1.csv
+-rw-rw-r--   0 saket     (1000) saket     (1000)   821724 2023-03-18 22:39:30.000000 pysradb-2.0.2/tests/data/test_search/ena_test_verbosity_1.json
+-rw-rw-r--   0 saket     (1000) saket     (1000)   415835 2023-03-18 22:39:30.000000 pysradb-2.0.2/tests/data/test_search/ena_test_verbosity_2.csv
+-rw-rw-r--   0 saket     (1000) saket     (1000)   821724 2023-03-18 22:39:30.000000 pysradb-2.0.2/tests/data/test_search/ena_test_verbosity_2.json
+-rw-rw-r--   0 saket     (1000) saket     (1000)  2188813 2023-03-18 22:39:30.000000 pysradb-2.0.2/tests/data/test_search/ena_test_verbosity_3.csv
+-rw-rw-r--   0 saket     (1000) saket     (1000)  4334941 2023-03-18 22:39:30.000000 pysradb-2.0.2/tests/data/test_search/ena_test_verbosity_3.json
+-rw-rw-r--   0 saket     (1000) saket     (1000)      857 2023-03-18 22:39:30.000000 pysradb-2.0.2/tests/data/test_search/geo_search_test1.txt
+-rw-rw-r--   0 saket     (1000) saket     (1000)       19 2023-03-18 22:39:30.000000 pysradb-2.0.2/tests/data/test_search/sra_search_test1.txt
+-rw-rw-r--   0 saket     (1000) saket     (1000)   648777 2023-03-18 22:39:30.000000 pysradb-2.0.2/tests/data/test_search/sra_test.xml
+-rw-rw-r--   0 saket     (1000) saket     (1000)       25 2023-03-18 22:39:30.000000 pysradb-2.0.2/tests/data/test_search/sra_test_2_verbosity_0.csv
+-rw-rw-r--   0 saket     (1000) saket     (1000)       76 2023-03-18 22:39:30.000000 pysradb-2.0.2/tests/data/test_search/sra_test_2_verbosity_1.csv
+-rw-rw-r--   0 saket     (1000) saket     (1000)      516 2023-03-18 22:39:30.000000 pysradb-2.0.2/tests/data/test_search/sra_test_2_verbosity_2.csv
+-rw-rw-r--   0 saket     (1000) saket     (1000)     9398 2023-03-18 22:39:30.000000 pysradb-2.0.2/tests/data/test_search/sra_test_2_verbosity_3.csv
+-rw-rw-r--   0 saket     (1000) saket     (1000)    10356 2023-03-18 22:39:30.000000 pysradb-2.0.2/tests/data/test_search/sra_test_ERS3331676.xml
+-rw-rw-r--   0 saket     (1000) saket     (1000)     1033 2023-03-18 22:39:30.000000 pysradb-2.0.2/tests/data/test_search/sra_test_verbosity_0.csv
+-rw-rw-r--   0 saket     (1000) saket     (1000)     6333 2023-03-18 22:39:30.000000 pysradb-2.0.2/tests/data/test_search/sra_test_verbosity_1.csv
+-rw-rw-r--   0 saket     (1000) saket     (1000)    20039 2023-03-18 22:39:30.000000 pysradb-2.0.2/tests/data/test_search/sra_test_verbosity_2.csv
+-rw-rw-r--   0 saket     (1000) saket     (1000)   329879 2023-03-18 22:39:30.000000 pysradb-2.0.2/tests/data/test_search/sra_test_verbosity_3.csv
+-rw-rw-r--   0 saket     (1000) saket     (1000)       14 2023-03-18 22:39:30.000000 pysradb-2.0.2/tests/data/test_search/sra_uids.txt
+-rw-rw-r--   0 saket     (1000) saket     (1000)     1162 2023-03-18 22:39:30.000000 pysradb-2.0.2/tests/test_geoweb.py
+-rw-rw-r--   0 saket     (1000) saket     (1000)    31386 2023-04-09 16:13:25.000000 pysradb-2.0.2/tests/test_search.py
+-rw-rw-r--   0 saket     (1000) saket     (1000)      572 2023-03-18 22:39:30.000000 pysradb-2.0.2/tests/test_sradb.py
+-rw-rw-r--   0 saket     (1000) saket     (1000)     8379 2023-04-09 04:13:51.000000 pysradb-2.0.2/tests/test_sraweb.py
+-rw-rw-r--   0 saket     (1000) saket     (1000)      547 2023-03-18 22:39:30.000000 pysradb-2.0.2/tests/test_utils.py
```

### Comparing `pysradb-2.0.1/CONTRIBUTING.rst` & `pysradb-2.0.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/HISTORY.rst` & `pysradb-2.0.2/HISTORY.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 #######
 History
 #######
 
 ******************
+2.0.2 (2023-04-09)
+******************
+
+* Fix for `gse-to-srp` to handle cases where a project is missing but SRXs
+  are returned (`#186 <https://github.com/saketkc/pysradb/issues/186>`)
+* Fix gse-to-gsm (`#187 <https://github.com/saketkc/pysradb/issues/187>`) 
+
+
+******************
 2.0.1 (2023-03-18)
 ******************
 
 * Fix for `pysradb download` - using `public_url`
 * Fix for SRX -> SRR and related conversions (`#183 <https://github.com/saketkc/pysradb/pull/183>`)
```

### Comparing `pysradb-2.0.1/LICENSE` & `pysradb-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/PKG-INFO` & `pysradb-2.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysradb
-Version: 2.0.1
+Version: 2.0.2
 Summary: A Python package for interacting with SRAdb and downloading datasets from SRA/ENA/GEO
 Home-page: https://github.com/saketkc/pysradb
 Author: Saket Choudhary
 Author-email: saketkc@gmail.com
 License: BSD license
 Keywords: pysradb
 Classifier: Development Status :: 5 - Production/Stable
@@ -69,15 +69,15 @@
 
    $ pysradb
     usage: pysradb [-h] [--version] [--citation]
                    {metadata,download,search,gse-to-gsm,gse-to-srp,gsm-to-gse,gsm-to-srp,gsm-to-srr,gsm-to-srs,gsm-to-srx,srp-to-gse,srp-to-srr,srp-to-srs,srp-to-srx,srr-to-gsm,srr-to-srp,srr-to-srs,srr-to-srx,srs-to-gsm,srs-to-srx,srx-to-srp,srx-to-srr,srx-to-srs}
                    ...
 
     pysradb: Query NGS metadata and data from NCBI Sequence Read Archive.
-    version: 2.0
+    version: 2.0.1
     Citation: 10.12688/f1000research.18676.1
 
     optional arguments:
       -h, --help            show this help message and exit
       --version             show program's version number and exit
       --citation            how to cite
 
@@ -367,14 +367,23 @@
 
 
 #######
 History
 #######
 
 ******************
+2.0.2 (2023-04-09)
+******************
+
+* Fix for `gse-to-srp` to handle cases where a project is missing but SRXs
+  are returned (`#186 <https://github.com/saketkc/pysradb/issues/186>`)
+* Fix gse-to-gsm (`#187 <https://github.com/saketkc/pysradb/issues/187>`) 
+
+
+******************
 2.0.1 (2023-03-18)
 ******************
 
 * Fix for `pysradb download` - using `public_url`
 * Fix for SRX -> SRR and related conversions (`#183 <https://github.com/saketkc/pysradb/pull/183>`)
```

### Comparing `pysradb-2.0.1/README.rst` & `pysradb-2.0.2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
    $ pysradb
     usage: pysradb [-h] [--version] [--citation]
                    {metadata,download,search,gse-to-gsm,gse-to-srp,gsm-to-gse,gsm-to-srp,gsm-to-srr,gsm-to-srs,gsm-to-srx,srp-to-gse,srp-to-srr,srp-to-srs,srp-to-srx,srr-to-gsm,srr-to-srp,srr-to-srs,srr-to-srx,srs-to-gsm,srs-to-srx,srx-to-srp,srx-to-srr,srx-to-srs}
                    ...
 
     pysradb: Query NGS metadata and data from NCBI Sequence Read Archive.
-    version: 2.0
+    version: 2.0.1
     Citation: 10.12688/f1000research.18676.1
 
     optional arguments:
       -h, --help            show this help message and exit
       --version             show program's version number and exit
       --citation            how to cite
```

### Comparing `pysradb-2.0.1/docs/Makefile` & `pysradb-2.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/docs/_static/e1.png` & `pysradb-2.0.2/docs/_static/e1.png`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/docs/_static/e2.png` & `pysradb-2.0.2/docs/_static/e2.png`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/docs/_static/e3.png` & `pysradb-2.0.2/docs/_static/e3.png`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/docs/_static/pysradb_v3.png` & `pysradb-2.0.2/docs/_static/pysradb_v3.png`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/docs/case_studies.rst` & `pysradb-2.0.2/docs/case_studies.rst`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/docs/cmdline.rst` & `pysradb-2.0.2/docs/cmdline.rst`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/docs/commands/download.rst` & `pysradb-2.0.2/docs/commands/download.rst`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/docs/commands/gse-to-gsm.rst` & `pysradb-2.0.2/docs/commands/gse-to-gsm.rst`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/docs/commands/gse-to-srp.rst` & `pysradb-2.0.2/docs/commands/gse-to-srp.rst`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/docs/commands/metadata.rst` & `pysradb-2.0.2/docs/commands/metadata.rst`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/docs/commands/search.rst` & `pysradb-2.0.2/docs/commands/search.rst`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/docs/commands/srp-to-gse.rst` & `pysradb-2.0.2/docs/commands/srp-to-gse.rst`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/docs/commands/srp-to-srr.rst` & `pysradb-2.0.2/docs/commands/srp-to-srr.rst`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/docs/commands/srp-to-srs.rst` & `pysradb-2.0.2/docs/commands/srp-to-srs.rst`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/docs/commands/srp-to-srx.rst` & `pysradb-2.0.2/docs/commands/srp-to-srx.rst`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/docs/commands/srr-to-srs.rst` & `pysradb-2.0.2/docs/commands/srr-to-srs.rst`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/docs/commands/srr-to-srx.rst` & `pysradb-2.0.2/docs/commands/srr-to-srx.rst`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/docs/commands/srs-to-srx.rst` & `pysradb-2.0.2/docs/commands/srs-to-srx.rst`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/docs/commands/srx-to-srr.rst` & `pysradb-2.0.2/docs/commands/srx-to-srr.rst`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/docs/commands/srx-to-srs.rst` & `pysradb-2.0.2/docs/commands/srx-to-srs.rst`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/docs/conf.py` & `pysradb-2.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/docs/index.rst` & `pysradb-2.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/docs/installation.rst` & `pysradb-2.0.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/docs/make.bat` & `pysradb-2.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/docs/pysradb.rst` & `pysradb-2.0.2/docs/pysradb.rst`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/docs/python-api-usage.rst` & `pysradb-2.0.2/docs/python-api-usage.rst`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/docs/quickstart.rst` & `pysradb-2.0.2/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/pysradb/basedb.py` & `pysradb-2.0.2/pysradb/basedb.py`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/pysradb/cli.py` & `pysradb-2.0.2/pysradb/cli.py`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/pysradb/download.py` & `pysradb-2.0.2/pysradb/download.py`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/pysradb/exceptions.py` & `pysradb-2.0.2/pysradb/exceptions.py`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/pysradb/filter_attrs.py` & `pysradb-2.0.2/pysradb/filter_attrs.py`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/pysradb/geodb.py` & `pysradb-2.0.2/pysradb/geodb.py`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/pysradb/geoweb.py` & `pysradb-2.0.2/pysradb/geoweb.py`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/pysradb/search.py` & `pysradb-2.0.2/pysradb/search.py`

 * *Files 0% similar despite different names*

```diff
@@ -1206,17 +1206,17 @@
     def _merge_selected_columns(self, regex):
         columns = list(self.df.filter(regex=regex, axis=1).columns)
         if not columns:
             series = pd.Series(dtype="object")
         elif len(columns) == 1:
             series = self.df[columns[0]]
         else:
-            series = self.df[columns[0]].append(
-                [self.df[c] for c in columns[1:]], ignore_index=True
-            )
+            series = self.df[columns[0]]
+            for c in columns[1:]:
+                series = pd.concat([series, self.df[c]])
         return series[~pd.isna(series)]
 
 
 class EnaSearch(QuerySearch):
     """Subclass of QuerySearch that implements search via querying ENA API
```

### Comparing `pysradb-2.0.1/pysradb/sradb.py` & `pysradb-2.0.2/pysradb/sradb.py`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/pysradb/sraweb.py` & `pysradb-2.0.2/pysradb/sraweb.py`

 * *Files 4% similar despite different names*

```diff
@@ -726,25 +726,29 @@
                 gse_records.append(record)
         if not len(gse_records):
             print("No results found for {}".format(gse))
             return None
         return pd.DataFrame(gse_records)
 
     def gse_to_gsm(self, gse, **kwargs):
+        if isinstance(gse, str):
+            gse = [gse]
         gse_df = self.fetch_gds_results(gse, **kwargs)
         gse_df = gse_df.rename(
             columns={
                 "accession": "experiment_alias",
                 "SRA": "experiment_accession",
                 "title": "experiment_title",
                 "summary": "sample_attribute",
             }
         )
         # TODO: Fix for multiple GSEs?
         gse_df["study_alias"] = ""
+        if len(gse) == 1:
+            study_alias = gse[0]
         for index, row in gse_df.iterrows():
             if row.entrytype == "GSE":
                 study_alias = row["experiment_accession"]
             # If GSM is ecnountered, apply it the
             # previously encountered GSE
             elif row.entrytype == "GSM":
                 gse_df.loc[index, "study_alias"] = study_alias
@@ -752,20 +756,46 @@
         if kwargs and kwargs["detailed"] == True:
             return gse_df
         return gse_df[
             ["study_alias", "experiment_alias", "experiment_accession"]
         ].drop_duplicates()
 
     def gse_to_srp(self, gse, **kwargs):
+        if isinstance(gse, str):
+            gse = [gse]
         gse_df = self.fetch_gds_results(gse, **kwargs)
-        gse_df = gse_df[gse_df.entrytype == "GSE"]
         gse_df = gse_df.rename(
             columns={"accession": "study_alias", "SRA": "study_accession"}
         )
-        return gse_df[["study_alias", "study_accession"]].drop_duplicates()
+        gse_df_subset = None
+        if "GSE" in gse_df.entrytype.unique():
+            gse_df_subset = gse_df[gse_df.entrytype == "GSE"]
+            common_gses = set(gse_df.study_alias.unique()).intersection(gse)
+            if len(common_gses) < len(gse):
+                gse_df_subset = None
+        if gse_df_subset is None:
+            # sometimes SRX ids ar ereturned instead of an entire project
+            # see https://github.com/saketkc/pysradb/issues/186
+            # GSE: GSE209835; SRP =SRP388275
+            gse_df_subset_gse = gse_df[gse_df.entrytype == "GSE"]
+            gse_of_interest = list(set(gse).difference(gse_df.study_alias.unique()))
+            gse_df_subset_other = gse_df[gse_df.entrytype != "GSE"]
+            srx = gse_df_subset_other.study_accession.tolist()
+            srp_df = self.srx_to_srp(srx)
+            srp_unique = list(
+                set(srp_df.study_accession.unique()).difference(
+                    gse_df_subset_gse.study_accession.tolist()
+                )
+            )
+            new_gse_df = pd.DataFrame(
+                {"study_alias": gse_of_interest, "study_accession": srp_unique}
+            )
+            gse_df_subset = pd.concat([gse_df_subset_gse, new_gse_df])
+
+        return gse_df_subset[["study_alias", "study_accession"]].drop_duplicates()
 
     def gsm_to_srp(self, gsm, **kwargs):
         gsm_df = self.fetch_gds_results(gsm, **kwargs)
         gsm_df = gsm_df[gsm_df.entrytype == "GSE"]
         gsm_df = gsm_df.rename(
             columns={"accession": "experiment_alias", "SRA": "study_accession"}
         )
@@ -815,18 +845,34 @@
             columns={"accession": "study_alias", "SRA": "study_accession"}
         )
         return gsm_df[["study_alias", "study_accession"]]
 
     def srp_to_gse(self, srp, **kwargs):
         """Get GSE for a SRP"""
         srp_df = self.fetch_gds_results(srp, **kwargs)
-        srp_df = srp_df[srp_df.entrytype == "GSE"]
+        if srp_df is None:
+            srp_df = pd.DataFrame(
+                {"study_alias": [], "study_accession": [], "entrytype": []}
+            )
+
         srp_df = srp_df.rename(
             columns={"accession": "study_alias", "SRA": "study_accession"}
         )
+        srp_df_gse = srp_df[srp_df.entrytype == "GSE"]
+        missing_srp = list(set(srp).difference(srp_df_gse.study_accession.tolist()))
+        srp_df_nongse = srp_df[srp_df.entrytype != "GSE"]
+        if srp_df_nongse.shape[0] >= 1:
+            srp_df_nongse = pd.DataFrame(
+                {
+                    "study_accession": missing_srp,
+                    "study_alias": [pd.NA] * len(missing_srp),
+                    "entrytpe": ["GSE"] * len(missing_srp),
+                }
+            )
+        srp_df = pd.concat([srp_df_gse, srp_df_nongse])
         return srp_df[["study_accession", "study_alias"]].drop_duplicates()
 
     def srp_to_srr(self, srp, **kwargs):
         """Get SRR for a SRP"""
         srp_df = self.sra_metadata(srp, **kwargs)
         return _order_first(srp_df, ["study_accession", "run_accession"])
```

### Comparing `pysradb-2.0.1/pysradb/taxid2name.py` & `pysradb-2.0.2/pysradb/taxid2name.py`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/pysradb/utils.py` & `pysradb-2.0.2/pysradb/utils.py`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/pysradb.egg-info/PKG-INFO` & `pysradb-2.0.2/pysradb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysradb
-Version: 2.0.1
+Version: 2.0.2
 Summary: A Python package for interacting with SRAdb and downloading datasets from SRA/ENA/GEO
 Home-page: https://github.com/saketkc/pysradb
 Author: Saket Choudhary
 Author-email: saketkc@gmail.com
 License: BSD license
 Keywords: pysradb
 Classifier: Development Status :: 5 - Production/Stable
@@ -69,15 +69,15 @@
 
    $ pysradb
     usage: pysradb [-h] [--version] [--citation]
                    {metadata,download,search,gse-to-gsm,gse-to-srp,gsm-to-gse,gsm-to-srp,gsm-to-srr,gsm-to-srs,gsm-to-srx,srp-to-gse,srp-to-srr,srp-to-srs,srp-to-srx,srr-to-gsm,srr-to-srp,srr-to-srs,srr-to-srx,srs-to-gsm,srs-to-srx,srx-to-srp,srx-to-srr,srx-to-srs}
                    ...
 
     pysradb: Query NGS metadata and data from NCBI Sequence Read Archive.
-    version: 2.0
+    version: 2.0.1
     Citation: 10.12688/f1000research.18676.1
 
     optional arguments:
       -h, --help            show this help message and exit
       --version             show program's version number and exit
       --citation            how to cite
 
@@ -367,14 +367,23 @@
 
 
 #######
 History
 #######
 
 ******************
+2.0.2 (2023-04-09)
+******************
+
+* Fix for `gse-to-srp` to handle cases where a project is missing but SRXs
+  are returned (`#186 <https://github.com/saketkc/pysradb/issues/186>`)
+* Fix gse-to-gsm (`#187 <https://github.com/saketkc/pysradb/issues/187>`) 
+
+
+******************
 2.0.1 (2023-03-18)
 ******************
 
 * Fix for `pysradb download` - using `public_url`
 * Fix for SRX -> SRR and related conversions (`#183 <https://github.com/saketkc/pysradb/pull/183>`)
```

### Comparing `pysradb-2.0.1/pysradb.egg-info/SOURCES.txt` & `pysradb-2.0.2/pysradb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/setup.cfg` & `pysradb-2.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 2.0.1
+current_version = 2.0.2
 commit = True
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\-(?P<release>[a-z]+)(?P<build>\d+))?
 serialize = 
 	{major}.{minor}.{patch}-{release}{build}
 	{major}.{minor}.{patch}
```

### Comparing `pysradb-2.0.1/setup.py` & `pysradb-2.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,10 +42,10 @@
     name="pysradb",
     packages=["pysradb"],
     python_requires=">=3.7",
     setup_requires=requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/saketkc/pysradb",
-    version="2.0.1",
+    version="2.0.2",
     zip_safe=False,
 )
```

### Comparing `pysradb-2.0.1/tests/_test_geodb.py` & `pysradb-2.0.2/tests/_test_geodb.py`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/tests/_test_pcli.py` & `pysradb-2.0.2/tests/_test_pcli.py`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/tests/_test_sradb.py` & `pysradb-2.0.2/tests/_test_sradb.py`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/tests/conftest.py` & `pysradb-2.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/tests/data/test_search/ena_search_test1.txt` & `pysradb-2.0.2/tests/data/test_search/ena_search_test1.txt`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/tests/data/test_search/ena_test_verbosity_0.csv` & `pysradb-2.0.2/tests/data/test_search/ena_test_verbosity_0.csv`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/tests/data/test_search/ena_test_verbosity_0.json` & `pysradb-2.0.2/tests/data/test_search/ena_test_verbosity_0.json`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/tests/data/test_search/ena_test_verbosity_1.csv` & `pysradb-2.0.2/tests/data/test_search/ena_test_verbosity_1.csv`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/tests/data/test_search/ena_test_verbosity_1.json` & `pysradb-2.0.2/tests/data/test_search/ena_test_verbosity_1.json`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/tests/data/test_search/ena_test_verbosity_2.csv` & `pysradb-2.0.2/tests/data/test_search/ena_test_verbosity_2.csv`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/tests/data/test_search/ena_test_verbosity_2.json` & `pysradb-2.0.2/tests/data/test_search/ena_test_verbosity_2.json`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/tests/data/test_search/ena_test_verbosity_3.csv` & `pysradb-2.0.2/tests/data/test_search/ena_test_verbosity_3.csv`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/tests/data/test_search/ena_test_verbosity_3.json` & `pysradb-2.0.2/tests/data/test_search/ena_test_verbosity_3.json`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/tests/data/test_search/geo_search_test1.txt` & `pysradb-2.0.2/tests/data/test_search/geo_search_test1.txt`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/tests/data/test_search/sra_test.xml` & `pysradb-2.0.2/tests/data/test_search/sra_test.xml`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/tests/data/test_search/sra_test_2_verbosity_2.csv` & `pysradb-2.0.2/tests/data/test_search/sra_test_2_verbosity_2.csv`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/tests/data/test_search/sra_test_2_verbosity_3.csv` & `pysradb-2.0.2/tests/data/test_search/sra_test_2_verbosity_3.csv`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/tests/data/test_search/sra_test_ERS3331676.xml` & `pysradb-2.0.2/tests/data/test_search/sra_test_ERS3331676.xml`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/tests/data/test_search/sra_test_verbosity_0.csv` & `pysradb-2.0.2/tests/data/test_search/sra_test_verbosity_0.csv`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/tests/data/test_search/sra_test_verbosity_1.csv` & `pysradb-2.0.2/tests/data/test_search/sra_test_verbosity_1.csv`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/tests/data/test_search/sra_test_verbosity_2.csv` & `pysradb-2.0.2/tests/data/test_search/sra_test_verbosity_2.csv`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/tests/data/test_search/sra_test_verbosity_3.csv` & `pysradb-2.0.2/tests/data/test_search/sra_test_verbosity_3.csv`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/tests/test_geoweb.py` & `pysradb-2.0.2/tests/test_geoweb.py`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/tests/test_search.py` & `pysradb-2.0.2/tests/test_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -1172,16 +1172,17 @@
 def missing_query_test_geo(empty_search_inputs_geo):
     for empty_search_input in empty_search_inputs_geo:
         with pytest.raises(MissingQueryException):
             QuerySearch(*empty_search_input)
 
 
 def test_geo_search_1():
-    instance = GeoSearch(3, 1000, geo_query="ferret")
+    instance = GeoSearch(3, 1000, geo_query="human")
     instance.search()
+    df = instance.get_df()
     df = instance.get_df()["experiment_accession"].to_list()
     assert len(df) > 10
     # with open("./tests/data/test_search/geo_search_test1.txt", "r") as f:
     #    expected_accessions = f.read().splitlines()
 
     # assert len(set(expected_accessions).intersection(df)) > 1
```

### Comparing `pysradb-2.0.1/tests/test_sradb.py` & `pysradb-2.0.2/tests/test_sradb.py`

 * *Files identical despite different names*

### Comparing `pysradb-2.0.1/tests/test_sraweb.py` & `pysradb-2.0.2/tests/test_sraweb.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,48 +111,61 @@
 
 def test_gse_to_gsm(sraweb_connection):
     """Test if gse is converted to gsm correctly"""
     df = sraweb_connection.gse_to_gsm("GSE56924", detailed=False)
     assert df.shape[0] == 96
 
 
+def test_gse_to_gsm2(sraweb_connection):
+    """Test for gse to gsm"""
+    df = sraweb_connection.gse_to_gsm("GSE200028", detailed=False)
+    assert df.shape[0] == 15
+
+
 def test_gse_to_gsm1(sraweb_connection):
     """Test if gse_to_gsm works without passing `detailed` parameter"""
     df = sraweb_connection.gse_to_gsm("GSE63858")
     assert list(sorted(df["experiment_alias"])) == ["GSM1558530", "GSM1558531"]
 
 
 def test_gse_to_srp(sraweb_connection):
     """Test if gse is converted to srp correctly"""
     df = sraweb_connection.gse_to_srp("GSE63858")
     assert df["study_accession"][0] == "SRP050548"
 
 
+def test_gse_to_srp2(sraweb_connection):
+    """Test if gse is converted to srp correctly"""
+    df = sraweb_connection.gse_to_srp(["GSE168880", "GSE209835"])
+    assert df["study_accession"].tolist()[0] == "SRP310566"
+    assert df["study_accession"].tolist()[1] == "SRP388275"
+
+
 def test_gsm_to_srp(sraweb_connection):
     """Test if gsm is converted to srp correctly"""
     df = sraweb_connection.gsm_to_srp("GSM1371490")
-    assert df["study_accession"][0] == "SRP041298"
+    assert df["study_accession"].tolist()[0] == "SRP041298"
 
 
 def test_gsm_to_gse(sraweb_connection):
     """Test if gsm is converted to gse correctly"""
     df = sraweb_connection.gsm_to_gse("GSM1371490")
-    assert df["study_alias"][0] == "GSE56924"
+    assert df["study_alias"].tolist()[0] == "GSE56924"
 
 
 def test_gsm_to_srr(sraweb_connection):
     """Test if gsm is converted to srr correctly"""
     df = sraweb_connection.gsm_to_srr("GSM1371489")
-    assert df["run_accession"][0] == "SRR1257271"
+    assert df["run_accession"].tolist()[0] == "SRR1257271"
 
 
 def test_gsm_to_srs(sraweb_connection):
     """Test if gsm is converted to srs correctly"""
     df = sraweb_connection.gsm_to_srs("GSM1371469")
-    assert df["sample_accession"][0] == "SRS594838"
+    assert df["sample_accession"].tolist()[0] == "SRS594838"
 
 
 def test_gsm_to_srx(sraweb_connection):
     """Test if gsm is converted to srx correctly"""
     df = sraweb_connection.gsm_to_srx("GSM1371454")
     assert list(df["experiment_accession"]) == ["SRX522468"]
 
@@ -185,15 +198,15 @@
     df = sraweb_connection.srr_to_srx("SRR057514")
     assert list(df["experiment_accession"]) == ["SRX021967"]
 
 
 def test_srs_to_gsm(sraweb_connection):
     """Test if srs is converted to gsm correctly"""
     df = sraweb_connection.srs_to_gsm("SRS079386")
-    assert list(df["experiment_alias"]) == ["GSM546921"]
+    assert df["experiment_alias"][0] == "GSM546921"
 
 
 def test_srs_to_srx(sraweb_connection):
     """Test if srs is converted to srx correctly"""
     df = sraweb_connection.srs_to_srx("SRS594838")
     assert list(df["experiment_accession"]) == ["SRX522483"]
```

### Comparing `pysradb-2.0.1/tests/test_utils.py` & `pysradb-2.0.2/tests/test_utils.py`

 * *Files identical despite different names*

