# Comparing `tmp/pyrsm-0.8.0.tar.gz` & `tmp/pyrsm-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrsm-0.8.0.tar", last modified: Mon May 15 08:52:06 2023, max compression
+gzip compressed data, was "pyrsm-0.8.1.tar", last modified: Mon May 15 09:06:53 2023, max compression
```

## Comparing `pyrsm-0.8.0.tar` & `pyrsm-0.8.1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-15 08:52:06.661436 pyrsm-0.8.0/
--rw-r--r--   0 root         (0) staff       (20)    34523 2022-03-19 20:23:12.000000 pyrsm-0.8.0/LICENSE
--rw-r--r--   0 root         (0) staff       (20)      215 2023-03-25 21:03:06.000000 pyrsm-0.8.0/MANIFEST.in
--rw-r--r--   0 root         (0) staff       (20)      592 2023-05-15 08:52:06.661496 pyrsm-0.8.0/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     2625 2023-03-25 21:31:10.000000 pyrsm-0.8.0/README.md
--rw-r--r--   0 root         (0) staff       (20)       80 2022-02-19 01:02:39.000000 pyrsm-0.8.0/pyproject.toml
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-15 08:52:06.652379 pyrsm-0.8.0/pyrsm/
--rw-r--r--   0 root         (0) staff       (20)      289 2023-05-15 08:50:47.000000 pyrsm-0.8.0/pyrsm/__init__.py
--rw-r--r--   0 root         (0) staff       (20)    54279 2023-05-15 06:31:28.000000 pyrsm-0.8.0/pyrsm/basics.py
--rw-r--r--   0 root         (0) staff       (20)     2843 2023-01-31 17:36:18.000000 pyrsm-0.8.0/pyrsm/bins.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-15 08:52:06.653735 pyrsm-0.8.0/pyrsm/data/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-15 08:52:06.654812 pyrsm-0.8.0/pyrsm/data/basics/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/basics/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     6996 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/basics/consider.pkl
--rw-r--r--   0 root         (0) staff       (20)    13754 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/basics/demand_uk.pkl
--rw-r--r--   0 root         (0) staff       (20)     5508 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/basics/newspaper.pkl
--rw-r--r--   0 root         (0) staff       (20)     8545 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/basics/salary.pkl
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-15 08:52:06.655953 pyrsm-0.8.0/pyrsm/data/data/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/data/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     1620 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/data/avengers.pkl
--rw-r--r--   0 root         (0) staff       (20)   207435 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/data/diamonds.pkl
--rw-r--r--   0 root         (0) staff       (20)     1557 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/data/publishers.pkl
--rw-r--r--   0 root         (0) staff       (20)     1660 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/data/superheroes.pkl
--rw-r--r--   0 root         (0) staff       (20)    69129 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/data/titanic.pkl
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-15 08:52:06.656338 pyrsm-0.8.0/pyrsm/data/design/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/design/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     3414 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/design/rndnames.pkl
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-15 08:52:06.658713 pyrsm-0.8.0/pyrsm/data/model/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/model/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     8197 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/model/catalog.pkl
--rw-r--r--   0 root         (0) staff       (20)    41039 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/model/direct_marketing.pkl
--rw-r--r--   0 root         (0) staff       (20)   342723 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/model/dvd.pkl
--rw-r--r--   0 root         (0) staff       (20)     4468 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/model/houseprices.pkl
--rw-r--r--   0 root         (0) staff       (20)    33206 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/model/ideal.pkl
--rw-r--r--   0 root         (0) staff       (20)   126402 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/model/ketchup.pkl
--rw-r--r--   0 root         (0) staff       (20)      315 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/model/movie_contract.pkl
--rw-r--r--   0 root         (0) staff       (20)     3123 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/model/ratings.pkl
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-15 08:52:06.660472 pyrsm-0.8.0/pyrsm/data/multivariate/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/multivariate/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     3125 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/multivariate/carpet.pkl
--rw-r--r--   0 root         (0) staff       (20)     2423 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/multivariate/city.pkl
--rw-r--r--   0 root         (0) staff       (20)     3923 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/multivariate/city2.pkl
--rw-r--r--   0 root         (0) staff       (20)     2625 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/multivariate/computer.pkl
--rw-r--r--   0 root         (0) staff       (20)     3442 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/multivariate/movie.pkl
--rw-r--r--   0 root         (0) staff       (20)     2994 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/multivariate/mp3.pkl
--rw-r--r--   0 root         (0) staff       (20)     3278 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/multivariate/retailers.pkl
--rw-r--r--   0 root         (0) staff       (20)     2357 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/multivariate/shopping.pkl
--rw-r--r--   0 root         (0) staff       (20)     4872 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/multivariate/toothpaste.pkl
--rw-r--r--   0 root         (0) staff       (20)     3678 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/data/multivariate/tpbrands.pkl
--rw-r--r--   0 root         (0) staff       (20)     1966 2023-01-26 08:23:23.000000 pyrsm-0.8.0/pyrsm/example_data.py
--rw-r--r--   0 root         (0) staff       (20)     5271 2023-05-07 05:21:24.000000 pyrsm-0.8.0/pyrsm/logit.py
--rw-r--r--   0 root         (0) staff       (20)    25101 2023-05-15 06:38:12.000000 pyrsm-0.8.0/pyrsm/model.py
--rw-r--r--   0 root         (0) staff       (20)     2214 2023-02-28 23:28:31.000000 pyrsm-0.8.0/pyrsm/notebook.py
--rw-r--r--   0 root         (0) staff       (20)    37519 2023-04-16 05:51:16.000000 pyrsm-0.8.0/pyrsm/perf.py
--rw-r--r--   0 root         (0) staff       (20)     1835 2022-02-13 01:24:09.000000 pyrsm-0.8.0/pyrsm/props.py
--rw-r--r--   0 root         (0) staff       (20)     7406 2023-05-15 08:45:10.000000 pyrsm-0.8.0/pyrsm/regress.py
--rw-r--r--   0 root         (0) staff       (20)     5411 2023-03-27 22:17:11.000000 pyrsm-0.8.0/pyrsm/stats.py
--rw-r--r--   0 root         (0) staff       (20)    10313 2023-05-14 21:06:56.000000 pyrsm-0.8.0/pyrsm/utils.py
--rw-r--r--   0 root         (0) staff       (20)    22540 2023-05-15 06:30:36.000000 pyrsm-0.8.0/pyrsm/visualize.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-15 08:52:06.653575 pyrsm-0.8.0/pyrsm.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      592 2023-05-15 08:52:06.000000 pyrsm-0.8.0/pyrsm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     1644 2023-05-15 08:52:06.000000 pyrsm-0.8.0/pyrsm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-05-15 08:52:06.000000 pyrsm-0.8.0/pyrsm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)      143 2023-05-15 08:52:06.000000 pyrsm-0.8.0/pyrsm.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)        6 2023-05-15 08:52:06.000000 pyrsm-0.8.0/pyrsm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)      950 2023-05-15 08:52:06.661779 pyrsm-0.8.0/setup.cfg
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-15 08:52:06.661325 pyrsm-0.8.0/tests/
--rw-r--r--   0 root         (0) staff       (20)      722 2022-03-07 07:21:43.000000 pyrsm-0.8.0/tests/test_basics.py
--rw-r--r--   0 root         (0) staff       (20)     1072 2023-03-05 06:28:28.000000 pyrsm-0.8.0/tests/test_bins.py
--rw-r--r--   0 root         (0) staff       (20)      794 2023-01-31 08:59:01.000000 pyrsm-0.8.0/tests/test_example_data.py
--rw-r--r--   0 root         (0) staff       (20)     2756 2023-01-21 01:15:24.000000 pyrsm-0.8.0/tests/test_perf.py
--rw-r--r--   0 root         (0) staff       (20)      657 2023-05-07 05:28:57.000000 pyrsm-0.8.0/tests/test_regression.py
--rw-r--r--   0 root         (0) staff       (20)     2036 2023-03-05 06:38:03.000000 pyrsm-0.8.0/tests/test_stats.py
--rw-r--r--   0 root         (0) staff       (20)     1979 2022-02-13 01:24:09.000000 pyrsm-0.8.0/tests/test_utils.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-15 09:06:53.303319 pyrsm-0.8.1/
+-rw-r--r--   0 root         (0) staff       (20)    34523 2022-03-19 20:23:12.000000 pyrsm-0.8.1/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)      215 2023-03-25 21:03:06.000000 pyrsm-0.8.1/MANIFEST.in
+-rw-r--r--   0 root         (0) staff       (20)      592 2023-05-15 09:06:53.303388 pyrsm-0.8.1/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     2625 2023-03-25 21:31:10.000000 pyrsm-0.8.1/README.md
+-rw-r--r--   0 root         (0) staff       (20)       80 2022-02-19 01:02:39.000000 pyrsm-0.8.1/pyproject.toml
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-15 09:06:53.293278 pyrsm-0.8.1/pyrsm/
+-rw-r--r--   0 root         (0) staff       (20)      320 2023-05-15 09:06:28.000000 pyrsm-0.8.1/pyrsm/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)    54279 2023-05-15 06:31:28.000000 pyrsm-0.8.1/pyrsm/basics.py
+-rw-r--r--   0 root         (0) staff       (20)     2843 2023-01-31 17:36:18.000000 pyrsm-0.8.1/pyrsm/bins.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-15 09:06:53.293988 pyrsm-0.8.1/pyrsm/data/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.1/pyrsm/data/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-15 09:06:53.294985 pyrsm-0.8.1/pyrsm/data/basics/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.1/pyrsm/data/basics/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     6996 2022-02-13 01:24:09.000000 pyrsm-0.8.1/pyrsm/data/basics/consider.pkl
+-rw-r--r--   0 root         (0) staff       (20)    13754 2022-02-13 01:24:09.000000 pyrsm-0.8.1/pyrsm/data/basics/demand_uk.pkl
+-rw-r--r--   0 root         (0) staff       (20)     5508 2022-02-13 01:24:09.000000 pyrsm-0.8.1/pyrsm/data/basics/newspaper.pkl
+-rw-r--r--   0 root         (0) staff       (20)     8545 2022-02-13 01:24:09.000000 pyrsm-0.8.1/pyrsm/data/basics/salary.pkl
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-15 09:06:53.296378 pyrsm-0.8.1/pyrsm/data/data/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.1/pyrsm/data/data/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     1620 2022-02-13 01:24:09.000000 pyrsm-0.8.1/pyrsm/data/data/avengers.pkl
+-rw-r--r--   0 root         (0) staff       (20)   207435 2022-02-13 01:24:09.000000 pyrsm-0.8.1/pyrsm/data/data/diamonds.pkl
+-rw-r--r--   0 root         (0) staff       (20)     1557 2022-02-13 01:24:09.000000 pyrsm-0.8.1/pyrsm/data/data/publishers.pkl
+-rw-r--r--   0 root         (0) staff       (20)     1660 2022-02-13 01:24:09.000000 pyrsm-0.8.1/pyrsm/data/data/superheroes.pkl
+-rw-r--r--   0 root         (0) staff       (20)    69129 2022-02-13 01:24:09.000000 pyrsm-0.8.1/pyrsm/data/data/titanic.pkl
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-15 09:06:53.296879 pyrsm-0.8.1/pyrsm/data/design/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.1/pyrsm/data/design/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     3414 2022-02-13 01:24:09.000000 pyrsm-0.8.1/pyrsm/data/design/rndnames.pkl
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-15 09:06:53.300497 pyrsm-0.8.1/pyrsm/data/model/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.1/pyrsm/data/model/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     8197 2022-02-13 01:24:09.000000 pyrsm-0.8.1/pyrsm/data/model/catalog.pkl
+-rw-r--r--   0 root         (0) staff       (20)    41039 2022-02-13 01:24:09.000000 pyrsm-0.8.1/pyrsm/data/model/direct_marketing.pkl
+-rw-r--r--   0 root         (0) staff       (20)   342723 2022-02-13 01:24:09.000000 pyrsm-0.8.1/pyrsm/data/model/dvd.pkl
+-rw-r--r--   0 root         (0) staff       (20)     4468 2022-02-13 01:24:09.000000 pyrsm-0.8.1/pyrsm/data/model/houseprices.pkl
+-rw-r--r--   0 root         (0) staff       (20)    33206 2022-02-13 01:24:09.000000 pyrsm-0.8.1/pyrsm/data/model/ideal.pkl
+-rw-r--r--   0 root         (0) staff       (20)   126402 2022-02-13 01:24:09.000000 pyrsm-0.8.1/pyrsm/data/model/ketchup.pkl
+-rw-r--r--   0 root         (0) staff       (20)      315 2022-02-13 01:24:09.000000 pyrsm-0.8.1/pyrsm/data/model/movie_contract.pkl
+-rw-r--r--   0 root         (0) staff       (20)     3123 2022-02-13 01:24:09.000000 pyrsm-0.8.1/pyrsm/data/model/ratings.pkl
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-15 09:06:53.302281 pyrsm-0.8.1/pyrsm/data/multivariate/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.1/pyrsm/data/multivariate/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     3125 2022-02-13 01:24:09.000000 pyrsm-0.8.1/pyrsm/data/multivariate/carpet.pkl
+-rw-r--r--   0 root         (0) staff       (20)     2423 2022-02-13 01:24:09.000000 pyrsm-0.8.1/pyrsm/data/multivariate/city.pkl
+-rw-r--r--   0 root         (0) staff       (20)     3923 2022-02-13 01:24:09.000000 pyrsm-0.8.1/pyrsm/data/multivariate/city2.pkl
+-rw-r--r--   0 root         (0) staff       (20)     2625 2022-02-13 01:24:09.000000 pyrsm-0.8.1/pyrsm/data/multivariate/computer.pkl
+-rw-r--r--   0 root         (0) staff       (20)     3442 2022-02-13 01:24:09.000000 pyrsm-0.8.1/pyrsm/data/multivariate/movie.pkl
+-rw-r--r--   0 root         (0) staff       (20)     2994 2022-02-13 01:24:09.000000 pyrsm-0.8.1/pyrsm/data/multivariate/mp3.pkl
+-rw-r--r--   0 root         (0) staff       (20)     3278 2022-02-13 01:24:09.000000 pyrsm-0.8.1/pyrsm/data/multivariate/retailers.pkl
+-rw-r--r--   0 root         (0) staff       (20)     2357 2022-02-13 01:24:09.000000 pyrsm-0.8.1/pyrsm/data/multivariate/shopping.pkl
+-rw-r--r--   0 root         (0) staff       (20)     4872 2022-02-13 01:24:09.000000 pyrsm-0.8.1/pyrsm/data/multivariate/toothpaste.pkl
+-rw-r--r--   0 root         (0) staff       (20)     3678 2022-02-13 01:24:09.000000 pyrsm-0.8.1/pyrsm/data/multivariate/tpbrands.pkl
+-rw-r--r--   0 root         (0) staff       (20)     1966 2023-01-26 08:23:23.000000 pyrsm-0.8.1/pyrsm/example_data.py
+-rw-r--r--   0 root         (0) staff       (20)     5271 2023-05-07 05:21:24.000000 pyrsm-0.8.1/pyrsm/logit.py
+-rw-r--r--   0 root         (0) staff       (20)    25101 2023-05-15 06:38:12.000000 pyrsm-0.8.1/pyrsm/model.py
+-rw-r--r--   0 root         (0) staff       (20)     2214 2023-02-28 23:28:31.000000 pyrsm-0.8.1/pyrsm/notebook.py
+-rw-r--r--   0 root         (0) staff       (20)    37519 2023-04-16 05:51:16.000000 pyrsm-0.8.1/pyrsm/perf.py
+-rw-r--r--   0 root         (0) staff       (20)     1835 2022-02-13 01:24:09.000000 pyrsm-0.8.1/pyrsm/props.py
+-rw-r--r--   0 root         (0) staff       (20)     7401 2023-05-15 09:04:04.000000 pyrsm-0.8.1/pyrsm/regress.py
+-rw-r--r--   0 root         (0) staff       (20)     5411 2023-03-27 22:17:11.000000 pyrsm-0.8.1/pyrsm/stats.py
+-rw-r--r--   0 root         (0) staff       (20)    10313 2023-05-14 21:06:56.000000 pyrsm-0.8.1/pyrsm/utils.py
+-rw-r--r--   0 root         (0) staff       (20)    22540 2023-05-15 06:30:36.000000 pyrsm-0.8.1/pyrsm/visualize.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-15 09:06:53.293876 pyrsm-0.8.1/pyrsm.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)      592 2023-05-15 09:06:53.000000 pyrsm-0.8.1/pyrsm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     1644 2023-05-15 09:06:53.000000 pyrsm-0.8.1/pyrsm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-05-15 09:06:53.000000 pyrsm-0.8.1/pyrsm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)      143 2023-05-15 09:06:53.000000 pyrsm-0.8.1/pyrsm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)        6 2023-05-15 09:06:53.000000 pyrsm-0.8.1/pyrsm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)      950 2023-05-15 09:06:53.303680 pyrsm-0.8.1/setup.cfg
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-15 09:06:53.303192 pyrsm-0.8.1/tests/
+-rw-r--r--   0 root         (0) staff       (20)      722 2022-03-07 07:21:43.000000 pyrsm-0.8.1/tests/test_basics.py
+-rw-r--r--   0 root         (0) staff       (20)     1072 2023-03-05 06:28:28.000000 pyrsm-0.8.1/tests/test_bins.py
+-rw-r--r--   0 root         (0) staff       (20)      794 2023-01-31 08:59:01.000000 pyrsm-0.8.1/tests/test_example_data.py
+-rw-r--r--   0 root         (0) staff       (20)     2756 2023-01-21 01:15:24.000000 pyrsm-0.8.1/tests/test_perf.py
+-rw-r--r--   0 root         (0) staff       (20)      657 2023-05-07 05:28:57.000000 pyrsm-0.8.1/tests/test_regression.py
+-rw-r--r--   0 root         (0) staff       (20)     2036 2023-03-05 06:38:03.000000 pyrsm-0.8.1/tests/test_stats.py
+-rw-r--r--   0 root         (0) staff       (20)     1979 2022-02-13 01:24:09.000000 pyrsm-0.8.1/tests/test_utils.py
```

### Comparing `pyrsm-0.8.0/LICENSE` & `pyrsm-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/PKG-INFO` & `pyrsm-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrsm
-Version: 0.8.0
+Version: 0.8.1
 Summary: Python functions for Customer Analytics at the Rady School of Management (RSM)
 Author: Vincent Nijs <vnijs@ucsd.edu>, Vikram Jambulapati <vikjam@ucsd.edu>, Suhas Goutham <sgoutham@ucsd.edu>, Raghav Prasad <rprasad@ucsd.edu>
 Author-email: vnijs@ucsd.edu
 License: AGPL-3.0-only
 Project-URL: Bug Reports, https://github.com/vnijs/pyrsm/issues
 Project-URL: Source, https://github.com/vnijs/pyrsm
 Description-Content-Type: text/markdown
```

### Comparing `pyrsm-0.8.0/README.md` & `pyrsm-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/pyrsm/basics.py` & `pyrsm-0.8.1/pyrsm/basics.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/pyrsm/bins.py` & `pyrsm-0.8.1/pyrsm/bins.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/pyrsm/data/basics/consider.pkl` & `pyrsm-0.8.1/pyrsm/data/basics/consider.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/pyrsm/data/basics/demand_uk.pkl` & `pyrsm-0.8.1/pyrsm/data/basics/demand_uk.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/pyrsm/data/basics/newspaper.pkl` & `pyrsm-0.8.1/pyrsm/data/basics/newspaper.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/pyrsm/data/basics/salary.pkl` & `pyrsm-0.8.1/pyrsm/data/basics/salary.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/pyrsm/data/data/avengers.pkl` & `pyrsm-0.8.1/pyrsm/data/data/avengers.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/pyrsm/data/data/diamonds.pkl` & `pyrsm-0.8.1/pyrsm/data/data/diamonds.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/pyrsm/data/data/publishers.pkl` & `pyrsm-0.8.1/pyrsm/data/data/publishers.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/pyrsm/data/data/superheroes.pkl` & `pyrsm-0.8.1/pyrsm/data/data/superheroes.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/pyrsm/data/data/titanic.pkl` & `pyrsm-0.8.1/pyrsm/data/data/titanic.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/pyrsm/data/design/rndnames.pkl` & `pyrsm-0.8.1/pyrsm/data/design/rndnames.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/pyrsm/data/model/catalog.pkl` & `pyrsm-0.8.1/pyrsm/data/model/catalog.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/pyrsm/data/model/direct_marketing.pkl` & `pyrsm-0.8.1/pyrsm/data/model/direct_marketing.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/pyrsm/data/model/dvd.pkl` & `pyrsm-0.8.1/pyrsm/data/model/dvd.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/pyrsm/data/model/houseprices.pkl` & `pyrsm-0.8.1/pyrsm/data/model/houseprices.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/pyrsm/data/model/ideal.pkl` & `pyrsm-0.8.1/pyrsm/data/model/ideal.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/pyrsm/data/model/ketchup.pkl` & `pyrsm-0.8.1/pyrsm/data/model/ketchup.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/pyrsm/data/model/ratings.pkl` & `pyrsm-0.8.1/pyrsm/data/model/ratings.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/pyrsm/data/multivariate/carpet.pkl` & `pyrsm-0.8.1/pyrsm/data/multivariate/carpet.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/pyrsm/data/multivariate/city.pkl` & `pyrsm-0.8.1/pyrsm/data/multivariate/city.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/pyrsm/data/multivariate/city2.pkl` & `pyrsm-0.8.1/pyrsm/data/multivariate/city2.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/pyrsm/data/multivariate/computer.pkl` & `pyrsm-0.8.1/pyrsm/data/multivariate/computer.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/pyrsm/data/multivariate/movie.pkl` & `pyrsm-0.8.1/pyrsm/data/multivariate/movie.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/pyrsm/data/multivariate/mp3.pkl` & `pyrsm-0.8.1/pyrsm/data/multivariate/mp3.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/pyrsm/data/multivariate/retailers.pkl` & `pyrsm-0.8.1/pyrsm/data/multivariate/retailers.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/pyrsm/data/multivariate/shopping.pkl` & `pyrsm-0.8.1/pyrsm/data/multivariate/shopping.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/pyrsm/data/multivariate/toothpaste.pkl` & `pyrsm-0.8.1/pyrsm/data/multivariate/toothpaste.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/pyrsm/data/multivariate/tpbrands.pkl` & `pyrsm-0.8.1/pyrsm/data/multivariate/tpbrands.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/pyrsm/example_data.py` & `pyrsm-0.8.1/pyrsm/example_data.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/pyrsm/logit.py` & `pyrsm-0.8.1/pyrsm/logit.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/pyrsm/model.py` & `pyrsm-0.8.1/pyrsm/model.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/pyrsm/notebook.py` & `pyrsm-0.8.1/pyrsm/notebook.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/pyrsm/perf.py` & `pyrsm-0.8.1/pyrsm/perf.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/pyrsm/props.py` & `pyrsm-0.8.1/pyrsm/props.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/pyrsm/regress.py` & `pyrsm-0.8.1/pyrsm/regress.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import nest_asyncio
 import webbrowser
 import pandas as pd
 import statsmodels.formula.api as smf
 from typing import Optional
 from statsmodels.regression.linear_model import RegressionResults as rrs
 from shiny import App
-from pyrsm.radiant.regress import model_regress
+from .radiant.regress import model_regress
 from .utils import ifelse, format_nr, setdiff
 from .visualize import pred_plot_sm, vimp_plot_sm
 from .model import (
     sig_stars,
     model_fit,
     extract_evars,
     extract_rvar,
```

### Comparing `pyrsm-0.8.0/pyrsm/stats.py` & `pyrsm-0.8.1/pyrsm/stats.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/pyrsm/utils.py` & `pyrsm-0.8.1/pyrsm/utils.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/pyrsm/visualize.py` & `pyrsm-0.8.1/pyrsm/visualize.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/pyrsm.egg-info/PKG-INFO` & `pyrsm-0.8.1/pyrsm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrsm
-Version: 0.8.0
+Version: 0.8.1
 Summary: Python functions for Customer Analytics at the Rady School of Management (RSM)
 Author: Vincent Nijs <vnijs@ucsd.edu>, Vikram Jambulapati <vikjam@ucsd.edu>, Suhas Goutham <sgoutham@ucsd.edu>, Raghav Prasad <rprasad@ucsd.edu>
 Author-email: vnijs@ucsd.edu
 License: AGPL-3.0-only
 Project-URL: Bug Reports, https://github.com/vnijs/pyrsm/issues
 Project-URL: Source, https://github.com/vnijs/pyrsm
 Description-Content-Type: text/markdown
```

### Comparing `pyrsm-0.8.0/pyrsm.egg-info/SOURCES.txt` & `pyrsm-0.8.1/pyrsm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/setup.cfg` & `pyrsm-0.8.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/tests/test_basics.py` & `pyrsm-0.8.1/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/tests/test_bins.py` & `pyrsm-0.8.1/tests/test_bins.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/tests/test_example_data.py` & `pyrsm-0.8.1/tests/test_example_data.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/tests/test_perf.py` & `pyrsm-0.8.1/tests/test_perf.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/tests/test_regression.py` & `pyrsm-0.8.1/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/tests/test_stats.py` & `pyrsm-0.8.1/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.0/tests/test_utils.py` & `pyrsm-0.8.1/tests/test_utils.py`

 * *Files identical despite different names*

