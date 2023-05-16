# Comparing `tmp/pyrsm-0.8.1.4.tar.gz` & `tmp/pyrsm-0.8.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrsm-0.8.1.4.tar", last modified: Tue May 16 07:43:35 2023, max compression
+gzip compressed data, was "pyrsm-0.8.1.5.tar", last modified: Tue May 16 19:44:31 2023, max compression
```

## Comparing `pyrsm-0.8.1.4.tar` & `pyrsm-0.8.1.5.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-16 07:43:35.266203 pyrsm-0.8.1.4/
--rw-r--r--   0 root         (0) staff       (20)    34523 2022-03-19 20:23:12.000000 pyrsm-0.8.1.4/LICENSE
--rw-r--r--   0 root         (0) staff       (20)      243 2023-05-16 06:57:58.000000 pyrsm-0.8.1.4/MANIFEST.in
--rw-r--r--   0 root         (0) staff       (20)      594 2023-05-16 07:43:35.266284 pyrsm-0.8.1.4/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     2625 2023-03-25 21:31:10.000000 pyrsm-0.8.1.4/README.md
--rw-r--r--   0 root         (0) staff       (20)       80 2022-02-19 01:02:39.000000 pyrsm-0.8.1.4/pyproject.toml
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-16 07:43:35.258380 pyrsm-0.8.1.4/pyrsm/
--rw-r--r--   0 root         (0) staff       (20)      314 2023-05-16 07:41:53.000000 pyrsm-0.8.1.4/pyrsm/__init__.py
--rw-r--r--   0 root         (0) staff       (20)    54279 2023-05-15 06:31:28.000000 pyrsm-0.8.1.4/pyrsm/basics.py
--rw-r--r--   0 root         (0) staff       (20)     2843 2023-01-31 17:36:18.000000 pyrsm-0.8.1.4/pyrsm/bins.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-16 07:43:35.259482 pyrsm-0.8.1.4/pyrsm/data/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.1.4/pyrsm/data/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-16 07:43:35.260063 pyrsm-0.8.1.4/pyrsm/data/basics/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.1.4/pyrsm/data/basics/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     6996 2022-02-13 01:24:09.000000 pyrsm-0.8.1.4/pyrsm/data/basics/consider.pkl
--rw-r--r--   0 root         (0) staff       (20)    13754 2022-02-13 01:24:09.000000 pyrsm-0.8.1.4/pyrsm/data/basics/demand_uk.pkl
--rw-r--r--   0 root         (0) staff       (20)     5508 2022-02-13 01:24:09.000000 pyrsm-0.8.1.4/pyrsm/data/basics/newspaper.pkl
--rw-r--r--   0 root         (0) staff       (20)     8545 2022-02-13 01:24:09.000000 pyrsm-0.8.1.4/pyrsm/data/basics/salary.pkl
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-16 07:43:35.260895 pyrsm-0.8.1.4/pyrsm/data/data/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.1.4/pyrsm/data/data/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     1620 2022-02-13 01:24:09.000000 pyrsm-0.8.1.4/pyrsm/data/data/avengers.pkl
--rw-r--r--   0 root         (0) staff       (20)   207435 2022-02-13 01:24:09.000000 pyrsm-0.8.1.4/pyrsm/data/data/diamonds.pkl
--rw-r--r--   0 root         (0) staff       (20)     1557 2022-02-13 01:24:09.000000 pyrsm-0.8.1.4/pyrsm/data/data/publishers.pkl
--rw-r--r--   0 root         (0) staff       (20)     1660 2022-02-13 01:24:09.000000 pyrsm-0.8.1.4/pyrsm/data/data/superheroes.pkl
--rw-r--r--   0 root         (0) staff       (20)    69129 2022-02-13 01:24:09.000000 pyrsm-0.8.1.4/pyrsm/data/data/titanic.pkl
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-16 07:43:35.261154 pyrsm-0.8.1.4/pyrsm/data/design/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.1.4/pyrsm/data/design/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     3414 2022-02-13 01:24:09.000000 pyrsm-0.8.1.4/pyrsm/data/design/rndnames.pkl
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-16 07:43:35.263165 pyrsm-0.8.1.4/pyrsm/data/model/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.1.4/pyrsm/data/model/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     8197 2022-02-13 01:24:09.000000 pyrsm-0.8.1.4/pyrsm/data/model/catalog.pkl
--rw-r--r--   0 root         (0) staff       (20)    41039 2022-02-13 01:24:09.000000 pyrsm-0.8.1.4/pyrsm/data/model/direct_marketing.pkl
--rw-r--r--   0 root         (0) staff       (20)   342723 2022-02-13 01:24:09.000000 pyrsm-0.8.1.4/pyrsm/data/model/dvd.pkl
--rw-r--r--   0 root         (0) staff       (20)     4468 2022-02-13 01:24:09.000000 pyrsm-0.8.1.4/pyrsm/data/model/houseprices.pkl
--rw-r--r--   0 root         (0) staff       (20)    33206 2022-02-13 01:24:09.000000 pyrsm-0.8.1.4/pyrsm/data/model/ideal.pkl
--rw-r--r--   0 root         (0) staff       (20)   126402 2022-02-13 01:24:09.000000 pyrsm-0.8.1.4/pyrsm/data/model/ketchup.pkl
--rw-r--r--   0 root         (0) staff       (20)      315 2022-02-13 01:24:09.000000 pyrsm-0.8.1.4/pyrsm/data/model/movie_contract.pkl
--rw-r--r--   0 root         (0) staff       (20)     3123 2022-02-13 01:24:09.000000 pyrsm-0.8.1.4/pyrsm/data/model/ratings.pkl
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-16 07:43:35.264650 pyrsm-0.8.1.4/pyrsm/data/multivariate/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.1.4/pyrsm/data/multivariate/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     3125 2022-02-13 01:24:09.000000 pyrsm-0.8.1.4/pyrsm/data/multivariate/carpet.pkl
--rw-r--r--   0 root         (0) staff       (20)     2423 2022-02-13 01:24:09.000000 pyrsm-0.8.1.4/pyrsm/data/multivariate/city.pkl
--rw-r--r--   0 root         (0) staff       (20)     3923 2022-02-13 01:24:09.000000 pyrsm-0.8.1.4/pyrsm/data/multivariate/city2.pkl
--rw-r--r--   0 root         (0) staff       (20)     2625 2022-02-13 01:24:09.000000 pyrsm-0.8.1.4/pyrsm/data/multivariate/computer.pkl
--rw-r--r--   0 root         (0) staff       (20)     3442 2022-02-13 01:24:09.000000 pyrsm-0.8.1.4/pyrsm/data/multivariate/movie.pkl
--rw-r--r--   0 root         (0) staff       (20)     2994 2022-02-13 01:24:09.000000 pyrsm-0.8.1.4/pyrsm/data/multivariate/mp3.pkl
--rw-r--r--   0 root         (0) staff       (20)     3278 2022-02-13 01:24:09.000000 pyrsm-0.8.1.4/pyrsm/data/multivariate/retailers.pkl
--rw-r--r--   0 root         (0) staff       (20)     2357 2022-02-13 01:24:09.000000 pyrsm-0.8.1.4/pyrsm/data/multivariate/shopping.pkl
--rw-r--r--   0 root         (0) staff       (20)     4872 2022-02-13 01:24:09.000000 pyrsm-0.8.1.4/pyrsm/data/multivariate/toothpaste.pkl
--rw-r--r--   0 root         (0) staff       (20)     3678 2022-02-13 01:24:09.000000 pyrsm-0.8.1.4/pyrsm/data/multivariate/tpbrands.pkl
--rw-r--r--   0 root         (0) staff       (20)     1966 2023-01-26 08:23:23.000000 pyrsm-0.8.1.4/pyrsm/example_data.py
--rw-r--r--   0 root         (0) staff       (20)     5271 2023-05-07 05:21:24.000000 pyrsm-0.8.1.4/pyrsm/logit.py
--rw-r--r--   0 root         (0) staff       (20)    25101 2023-05-15 06:38:12.000000 pyrsm-0.8.1.4/pyrsm/model.py
--rw-r--r--   0 root         (0) staff       (20)     2214 2023-05-15 20:48:14.000000 pyrsm-0.8.1.4/pyrsm/notebook.py
--rw-r--r--   0 root         (0) staff       (20)    37519 2023-04-16 05:51:16.000000 pyrsm-0.8.1.4/pyrsm/perf.py
--rw-r--r--   0 root         (0) staff       (20)     1835 2022-02-13 01:24:09.000000 pyrsm-0.8.1.4/pyrsm/props.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-16 07:43:35.265003 pyrsm-0.8.1.4/pyrsm/radiant/
--rw-r--r--   0 root         (0) staff       (20)       23 2023-05-15 21:34:35.000000 pyrsm-0.8.1.4/pyrsm/radiant/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     9489 2023-05-15 05:18:12.000000 pyrsm-0.8.1.4/pyrsm/radiant/logit.py
--rw-r--r--   0 root         (0) staff       (20)    10625 2023-05-16 07:42:58.000000 pyrsm-0.8.1.4/pyrsm/radiant/regress.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-16 07:43:35.265268 pyrsm-0.8.1.4/pyrsm/radiant/www/
--rw-r--r--   0 root         (0) staff       (20)      230 2023-05-11 03:12:37.000000 pyrsm-0.8.1.4/pyrsm/radiant/www/copy.js
--rw-r--r--   0 root         (0) staff       (20)     3597 2023-05-11 03:12:22.000000 pyrsm-0.8.1.4/pyrsm/radiant/www/style.css
--rw-r--r--   0 root         (0) staff       (20)     7156 2023-05-16 00:00:23.000000 pyrsm-0.8.1.4/pyrsm/regress.py
--rw-r--r--   0 root         (0) staff       (20)     5411 2023-03-27 22:17:11.000000 pyrsm-0.8.1.4/pyrsm/stats.py
--rw-r--r--   0 root         (0) staff       (20)    10313 2023-05-14 21:06:56.000000 pyrsm-0.8.1.4/pyrsm/utils.py
--rw-r--r--   0 root         (0) staff       (20)    22540 2023-05-15 06:30:36.000000 pyrsm-0.8.1.4/pyrsm/visualize.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-16 07:43:35.259348 pyrsm-0.8.1.4/pyrsm.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      594 2023-05-16 07:43:35.000000 pyrsm-0.8.1.4/pyrsm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     1772 2023-05-16 07:43:35.000000 pyrsm-0.8.1.4/pyrsm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-05-16 07:43:35.000000 pyrsm-0.8.1.4/pyrsm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)      160 2023-05-16 07:43:35.000000 pyrsm-0.8.1.4/pyrsm.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)        6 2023-05-16 07:43:35.000000 pyrsm-0.8.1.4/pyrsm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)      968 2023-05-16 07:43:35.266602 pyrsm-0.8.1.4/setup.cfg
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-16 07:43:35.266098 pyrsm-0.8.1.4/tests/
--rw-r--r--   0 root         (0) staff       (20)      722 2023-05-16 05:24:37.000000 pyrsm-0.8.1.4/tests/test_basics.py
--rw-r--r--   0 root         (0) staff       (20)     1072 2023-03-05 06:28:28.000000 pyrsm-0.8.1.4/tests/test_bins.py
--rw-r--r--   0 root         (0) staff       (20)      794 2023-05-16 05:39:55.000000 pyrsm-0.8.1.4/tests/test_example_data.py
--rw-r--r--   0 root         (0) staff       (20)     2756 2023-01-21 01:15:24.000000 pyrsm-0.8.1.4/tests/test_perf.py
--rw-r--r--   0 root         (0) staff       (20)      615 2023-05-16 05:41:07.000000 pyrsm-0.8.1.4/tests/test_regression.py
--rw-r--r--   0 root         (0) staff       (20)     2036 2023-03-05 06:38:03.000000 pyrsm-0.8.1.4/tests/test_stats.py
--rw-r--r--   0 root         (0) staff       (20)     1979 2022-02-13 01:24:09.000000 pyrsm-0.8.1.4/tests/test_utils.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-16 19:44:31.364157 pyrsm-0.8.1.5/
+-rw-r--r--   0 root         (0) staff       (20)    34523 2022-03-19 20:23:12.000000 pyrsm-0.8.1.5/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)      243 2023-05-16 06:57:58.000000 pyrsm-0.8.1.5/MANIFEST.in
+-rw-r--r--   0 root         (0) staff       (20)      594 2023-05-16 19:44:31.364232 pyrsm-0.8.1.5/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     2625 2023-05-16 19:42:31.000000 pyrsm-0.8.1.5/README.md
+-rw-r--r--   0 root         (0) staff       (20)       80 2022-02-19 01:02:39.000000 pyrsm-0.8.1.5/pyproject.toml
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-16 19:44:31.348087 pyrsm-0.8.1.5/pyrsm/
+-rw-r--r--   0 root         (0) staff       (20)      314 2023-05-16 19:44:03.000000 pyrsm-0.8.1.5/pyrsm/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)    54279 2023-05-15 06:31:28.000000 pyrsm-0.8.1.5/pyrsm/basics.py
+-rw-r--r--   0 root         (0) staff       (20)     2843 2023-01-31 17:36:18.000000 pyrsm-0.8.1.5/pyrsm/bins.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-16 19:44:31.348761 pyrsm-0.8.1.5/pyrsm/data/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.1.5/pyrsm/data/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-16 19:44:31.349818 pyrsm-0.8.1.5/pyrsm/data/basics/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.1.5/pyrsm/data/basics/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     6996 2022-02-13 01:24:09.000000 pyrsm-0.8.1.5/pyrsm/data/basics/consider.pkl
+-rw-r--r--   0 root         (0) staff       (20)    13754 2022-02-13 01:24:09.000000 pyrsm-0.8.1.5/pyrsm/data/basics/demand_uk.pkl
+-rw-r--r--   0 root         (0) staff       (20)     5508 2022-02-13 01:24:09.000000 pyrsm-0.8.1.5/pyrsm/data/basics/newspaper.pkl
+-rw-r--r--   0 root         (0) staff       (20)     8545 2022-02-13 01:24:09.000000 pyrsm-0.8.1.5/pyrsm/data/basics/salary.pkl
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-16 19:44:31.351181 pyrsm-0.8.1.5/pyrsm/data/data/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.1.5/pyrsm/data/data/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     1620 2022-02-13 01:24:09.000000 pyrsm-0.8.1.5/pyrsm/data/data/avengers.pkl
+-rw-r--r--   0 root         (0) staff       (20)   207435 2022-02-13 01:24:09.000000 pyrsm-0.8.1.5/pyrsm/data/data/diamonds.pkl
+-rw-r--r--   0 root         (0) staff       (20)     1557 2022-02-13 01:24:09.000000 pyrsm-0.8.1.5/pyrsm/data/data/publishers.pkl
+-rw-r--r--   0 root         (0) staff       (20)     1660 2022-02-13 01:24:09.000000 pyrsm-0.8.1.5/pyrsm/data/data/superheroes.pkl
+-rw-r--r--   0 root         (0) staff       (20)    69129 2022-02-13 01:24:09.000000 pyrsm-0.8.1.5/pyrsm/data/data/titanic.pkl
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-16 19:44:31.351685 pyrsm-0.8.1.5/pyrsm/data/design/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.1.5/pyrsm/data/design/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     3414 2022-02-13 01:24:09.000000 pyrsm-0.8.1.5/pyrsm/data/design/rndnames.pkl
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-16 19:44:31.358149 pyrsm-0.8.1.5/pyrsm/data/model/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.1.5/pyrsm/data/model/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     8197 2022-02-13 01:24:09.000000 pyrsm-0.8.1.5/pyrsm/data/model/catalog.pkl
+-rw-r--r--   0 root         (0) staff       (20)    41039 2022-02-13 01:24:09.000000 pyrsm-0.8.1.5/pyrsm/data/model/direct_marketing.pkl
+-rw-r--r--   0 root         (0) staff       (20)   342723 2022-02-13 01:24:09.000000 pyrsm-0.8.1.5/pyrsm/data/model/dvd.pkl
+-rw-r--r--   0 root         (0) staff       (20)     4468 2022-02-13 01:24:09.000000 pyrsm-0.8.1.5/pyrsm/data/model/houseprices.pkl
+-rw-r--r--   0 root         (0) staff       (20)    33206 2022-02-13 01:24:09.000000 pyrsm-0.8.1.5/pyrsm/data/model/ideal.pkl
+-rw-r--r--   0 root         (0) staff       (20)   126402 2022-02-13 01:24:09.000000 pyrsm-0.8.1.5/pyrsm/data/model/ketchup.pkl
+-rw-r--r--   0 root         (0) staff       (20)      315 2022-02-13 01:24:09.000000 pyrsm-0.8.1.5/pyrsm/data/model/movie_contract.pkl
+-rw-r--r--   0 root         (0) staff       (20)     3123 2022-02-13 01:24:09.000000 pyrsm-0.8.1.5/pyrsm/data/model/ratings.pkl
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-16 19:44:31.359963 pyrsm-0.8.1.5/pyrsm/data/multivariate/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.1.5/pyrsm/data/multivariate/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     3125 2022-02-13 01:24:09.000000 pyrsm-0.8.1.5/pyrsm/data/multivariate/carpet.pkl
+-rw-r--r--   0 root         (0) staff       (20)     2423 2022-02-13 01:24:09.000000 pyrsm-0.8.1.5/pyrsm/data/multivariate/city.pkl
+-rw-r--r--   0 root         (0) staff       (20)     3923 2022-02-13 01:24:09.000000 pyrsm-0.8.1.5/pyrsm/data/multivariate/city2.pkl
+-rw-r--r--   0 root         (0) staff       (20)     2625 2022-02-13 01:24:09.000000 pyrsm-0.8.1.5/pyrsm/data/multivariate/computer.pkl
+-rw-r--r--   0 root         (0) staff       (20)     3442 2022-02-13 01:24:09.000000 pyrsm-0.8.1.5/pyrsm/data/multivariate/movie.pkl
+-rw-r--r--   0 root         (0) staff       (20)     2994 2022-02-13 01:24:09.000000 pyrsm-0.8.1.5/pyrsm/data/multivariate/mp3.pkl
+-rw-r--r--   0 root         (0) staff       (20)     3278 2022-02-13 01:24:09.000000 pyrsm-0.8.1.5/pyrsm/data/multivariate/retailers.pkl
+-rw-r--r--   0 root         (0) staff       (20)     2357 2022-02-13 01:24:09.000000 pyrsm-0.8.1.5/pyrsm/data/multivariate/shopping.pkl
+-rw-r--r--   0 root         (0) staff       (20)     4872 2022-02-13 01:24:09.000000 pyrsm-0.8.1.5/pyrsm/data/multivariate/toothpaste.pkl
+-rw-r--r--   0 root         (0) staff       (20)     3678 2022-02-13 01:24:09.000000 pyrsm-0.8.1.5/pyrsm/data/multivariate/tpbrands.pkl
+-rw-r--r--   0 root         (0) staff       (20)     1966 2023-01-26 08:23:23.000000 pyrsm-0.8.1.5/pyrsm/example_data.py
+-rw-r--r--   0 root         (0) staff       (20)     5271 2023-05-07 05:21:24.000000 pyrsm-0.8.1.5/pyrsm/logit.py
+-rw-r--r--   0 root         (0) staff       (20)    25101 2023-05-15 06:38:12.000000 pyrsm-0.8.1.5/pyrsm/model.py
+-rw-r--r--   0 root         (0) staff       (20)     2214 2023-05-15 20:48:14.000000 pyrsm-0.8.1.5/pyrsm/notebook.py
+-rw-r--r--   0 root         (0) staff       (20)    37519 2023-04-16 05:51:16.000000 pyrsm-0.8.1.5/pyrsm/perf.py
+-rw-r--r--   0 root         (0) staff       (20)     1835 2022-02-13 01:24:09.000000 pyrsm-0.8.1.5/pyrsm/props.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-16 19:44:31.360382 pyrsm-0.8.1.5/pyrsm/radiant/
+-rw-r--r--   0 root         (0) staff       (20)       23 2023-05-15 21:34:35.000000 pyrsm-0.8.1.5/pyrsm/radiant/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     9489 2023-05-15 05:18:12.000000 pyrsm-0.8.1.5/pyrsm/radiant/logit.py
+-rw-r--r--   0 root         (0) staff       (20)    10769 2023-05-16 19:43:32.000000 pyrsm-0.8.1.5/pyrsm/radiant/regress.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-16 19:44:31.360775 pyrsm-0.8.1.5/pyrsm/radiant/www/
+-rw-r--r--   0 root         (0) staff       (20)      230 2023-05-11 03:12:37.000000 pyrsm-0.8.1.5/pyrsm/radiant/www/copy.js
+-rw-r--r--   0 root         (0) staff       (20)     3597 2023-05-11 03:12:22.000000 pyrsm-0.8.1.5/pyrsm/radiant/www/style.css
+-rw-r--r--   0 root         (0) staff       (20)     7156 2023-05-16 00:00:23.000000 pyrsm-0.8.1.5/pyrsm/regress.py
+-rw-r--r--   0 root         (0) staff       (20)     5411 2023-03-27 22:17:11.000000 pyrsm-0.8.1.5/pyrsm/stats.py
+-rw-r--r--   0 root         (0) staff       (20)    10313 2023-05-14 21:06:56.000000 pyrsm-0.8.1.5/pyrsm/utils.py
+-rw-r--r--   0 root         (0) staff       (20)    22540 2023-05-15 06:30:36.000000 pyrsm-0.8.1.5/pyrsm/visualize.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-16 19:44:31.348653 pyrsm-0.8.1.5/pyrsm.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)      594 2023-05-16 19:44:31.000000 pyrsm-0.8.1.5/pyrsm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     1772 2023-05-16 19:44:31.000000 pyrsm-0.8.1.5/pyrsm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-05-16 19:44:31.000000 pyrsm-0.8.1.5/pyrsm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)      176 2023-05-16 19:44:31.000000 pyrsm-0.8.1.5/pyrsm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)        6 2023-05-16 19:44:31.000000 pyrsm-0.8.1.5/pyrsm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)      985 2023-05-16 19:44:31.364568 pyrsm-0.8.1.5/setup.cfg
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-16 19:44:31.363911 pyrsm-0.8.1.5/tests/
+-rw-r--r--   0 root         (0) staff       (20)      722 2023-05-16 05:24:37.000000 pyrsm-0.8.1.5/tests/test_basics.py
+-rw-r--r--   0 root         (0) staff       (20)     1072 2023-03-05 06:28:28.000000 pyrsm-0.8.1.5/tests/test_bins.py
+-rw-r--r--   0 root         (0) staff       (20)      794 2023-05-16 05:39:55.000000 pyrsm-0.8.1.5/tests/test_example_data.py
+-rw-r--r--   0 root         (0) staff       (20)     2756 2023-01-21 01:15:24.000000 pyrsm-0.8.1.5/tests/test_perf.py
+-rw-r--r--   0 root         (0) staff       (20)      615 2023-05-16 05:41:07.000000 pyrsm-0.8.1.5/tests/test_regression.py
+-rw-r--r--   0 root         (0) staff       (20)     2036 2023-03-05 06:38:03.000000 pyrsm-0.8.1.5/tests/test_stats.py
+-rw-r--r--   0 root         (0) staff       (20)     1979 2022-02-13 01:24:09.000000 pyrsm-0.8.1.5/tests/test_utils.py
```

### Comparing `pyrsm-0.8.1.4/LICENSE` & `pyrsm-0.8.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/PKG-INFO` & `pyrsm-0.8.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrsm
-Version: 0.8.1.4
+Version: 0.8.1.5
 Summary: Python functions for Customer Analytics at the Rady School of Management (RSM)
 Author: Vincent Nijs <vnijs@ucsd.edu>, Vikram Jambulapati <vikjam@ucsd.edu>, Suhas Goutham <sgoutham@ucsd.edu>, Raghav Prasad <rprasad@ucsd.edu>
 Author-email: vnijs@ucsd.edu
 License: AGPL-3.0-only
 Project-URL: Bug Reports, https://github.com/vnijs/pyrsm/issues
 Project-URL: Source, https://github.com/vnijs/pyrsm
 Description-Content-Type: text/markdown
```

### Comparing `pyrsm-0.8.1.4/README.md` & `pyrsm-0.8.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 Python functions and classes for Customer Analytics at the Rady School of Management (RSM), University of California, San Diego (UCSD)
 
 ## Install instructions
 
 If you have python and pip3 install you can use the below to install the latest version of `pyrsm`:
 
-`pip3 install --user 'pyrsm>=0.7.9'`
+`pip3 install --user 'pyrsm>=0.8.1'`
 
 or 
 
-`conda install 'pyrsm>=0.7.9'`
+`conda install 'pyrsm>=0.8.1'`
 
 ## Example notebooks
 
 ### Data
 
 * [Load example datasets](examples/load-example-data.ipynb)
 * [Save and load notebook state files](examples/save-load-state.ipynb)
```

### Comparing `pyrsm-0.8.1.4/pyrsm/basics.py` & `pyrsm-0.8.1.5/pyrsm/basics.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/pyrsm/bins.py` & `pyrsm-0.8.1.5/pyrsm/bins.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/pyrsm/data/basics/consider.pkl` & `pyrsm-0.8.1.5/pyrsm/data/basics/consider.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/pyrsm/data/basics/demand_uk.pkl` & `pyrsm-0.8.1.5/pyrsm/data/basics/demand_uk.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/pyrsm/data/basics/newspaper.pkl` & `pyrsm-0.8.1.5/pyrsm/data/basics/newspaper.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/pyrsm/data/basics/salary.pkl` & `pyrsm-0.8.1.5/pyrsm/data/basics/salary.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/pyrsm/data/data/avengers.pkl` & `pyrsm-0.8.1.5/pyrsm/data/data/avengers.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/pyrsm/data/data/diamonds.pkl` & `pyrsm-0.8.1.5/pyrsm/data/data/diamonds.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/pyrsm/data/data/publishers.pkl` & `pyrsm-0.8.1.5/pyrsm/data/data/publishers.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/pyrsm/data/data/superheroes.pkl` & `pyrsm-0.8.1.5/pyrsm/data/data/superheroes.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/pyrsm/data/data/titanic.pkl` & `pyrsm-0.8.1.5/pyrsm/data/data/titanic.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/pyrsm/data/design/rndnames.pkl` & `pyrsm-0.8.1.5/pyrsm/data/design/rndnames.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/pyrsm/data/model/catalog.pkl` & `pyrsm-0.8.1.5/pyrsm/data/model/catalog.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/pyrsm/data/model/direct_marketing.pkl` & `pyrsm-0.8.1.5/pyrsm/data/model/direct_marketing.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/pyrsm/data/model/dvd.pkl` & `pyrsm-0.8.1.5/pyrsm/data/model/dvd.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/pyrsm/data/model/houseprices.pkl` & `pyrsm-0.8.1.5/pyrsm/data/model/houseprices.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/pyrsm/data/model/ideal.pkl` & `pyrsm-0.8.1.5/pyrsm/data/model/ideal.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/pyrsm/data/model/ketchup.pkl` & `pyrsm-0.8.1.5/pyrsm/data/model/ketchup.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/pyrsm/data/model/ratings.pkl` & `pyrsm-0.8.1.5/pyrsm/data/model/ratings.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/pyrsm/data/multivariate/carpet.pkl` & `pyrsm-0.8.1.5/pyrsm/data/multivariate/carpet.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/pyrsm/data/multivariate/city.pkl` & `pyrsm-0.8.1.5/pyrsm/data/multivariate/city.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/pyrsm/data/multivariate/city2.pkl` & `pyrsm-0.8.1.5/pyrsm/data/multivariate/city2.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/pyrsm/data/multivariate/computer.pkl` & `pyrsm-0.8.1.5/pyrsm/data/multivariate/computer.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/pyrsm/data/multivariate/movie.pkl` & `pyrsm-0.8.1.5/pyrsm/data/multivariate/movie.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/pyrsm/data/multivariate/mp3.pkl` & `pyrsm-0.8.1.5/pyrsm/data/multivariate/mp3.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/pyrsm/data/multivariate/retailers.pkl` & `pyrsm-0.8.1.5/pyrsm/data/multivariate/retailers.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/pyrsm/data/multivariate/shopping.pkl` & `pyrsm-0.8.1.5/pyrsm/data/multivariate/shopping.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/pyrsm/data/multivariate/toothpaste.pkl` & `pyrsm-0.8.1.5/pyrsm/data/multivariate/toothpaste.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/pyrsm/data/multivariate/tpbrands.pkl` & `pyrsm-0.8.1.5/pyrsm/data/multivariate/tpbrands.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/pyrsm/example_data.py` & `pyrsm-0.8.1.5/pyrsm/example_data.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/pyrsm/logit.py` & `pyrsm-0.8.1.5/pyrsm/logit.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/pyrsm/model.py` & `pyrsm-0.8.1.5/pyrsm/model.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/pyrsm/notebook.py` & `pyrsm-0.8.1.5/pyrsm/notebook.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/pyrsm/perf.py` & `pyrsm-0.8.1.5/pyrsm/perf.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/pyrsm/props.py` & `pyrsm-0.8.1.5/pyrsm/props.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/pyrsm/radiant/logit.py` & `pyrsm-0.8.1.5/pyrsm/radiant/logit.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/pyrsm/radiant/regress.py` & `pyrsm-0.8.1.5/pyrsm/radiant/regress.py`

 * *Files 5% similar despite different names*

```diff
@@ -128,14 +128,16 @@
             cmd = black.format_str(code, mode=black.Mode())
             try:
                 pyperclip.copy(cmd)
             except pyperclip.PyperclipException:
                 pass
             cmd = f"""<pre><details><summary>Code</summary>{cmd}</details></pre>"""
             return ui.HTML(cmd)
+            # needs syntax highlighting but ui.markdown doesn't provide that yet
+            # return ui.markdown(f"""```python\n{cmd}\n```""")
 
         @reactive.Calc
         def load_data():
             return (
                 self.datasets[input.datasets()],
                 input.datasets(),
                 f"{input.datasets()} = pd.read_pickle('{input.datasets()}.pkl')",
```

### Comparing `pyrsm-0.8.1.4/pyrsm/radiant/www/style.css` & `pyrsm-0.8.1.5/pyrsm/radiant/www/style.css`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/pyrsm/regress.py` & `pyrsm-0.8.1.5/pyrsm/regress.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/pyrsm/stats.py` & `pyrsm-0.8.1.5/pyrsm/stats.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/pyrsm/utils.py` & `pyrsm-0.8.1.5/pyrsm/utils.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/pyrsm/visualize.py` & `pyrsm-0.8.1.5/pyrsm/visualize.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/pyrsm.egg-info/PKG-INFO` & `pyrsm-0.8.1.5/pyrsm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrsm
-Version: 0.8.1.4
+Version: 0.8.1.5
 Summary: Python functions for Customer Analytics at the Rady School of Management (RSM)
 Author: Vincent Nijs <vnijs@ucsd.edu>, Vikram Jambulapati <vikjam@ucsd.edu>, Suhas Goutham <sgoutham@ucsd.edu>, Raghav Prasad <rprasad@ucsd.edu>
 Author-email: vnijs@ucsd.edu
 License: AGPL-3.0-only
 Project-URL: Bug Reports, https://github.com/vnijs/pyrsm/issues
 Project-URL: Source, https://github.com/vnijs/pyrsm
 Description-Content-Type: text/markdown
```

### Comparing `pyrsm-0.8.1.4/pyrsm.egg-info/SOURCES.txt` & `pyrsm-0.8.1.5/pyrsm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/setup.cfg` & `pyrsm-0.8.1.5/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 	seaborn>=0.9.0
 	matplotlib>=3.1.1
 	statsmodels>=0.10.1
 	scipy>=1.4.1
 	scikit-learn>=1.0.2
 	IPython>=8.0.1
 	shiny>=0.3.3
+	uvicorn>=0.20.0
 	pyperclip>=1.8.2
 
 [options.packages.find]
 exclude = 
 	*.tests
 	*.tests.*
 	tests.*
```

### Comparing `pyrsm-0.8.1.4/tests/test_basics.py` & `pyrsm-0.8.1.5/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/tests/test_bins.py` & `pyrsm-0.8.1.5/tests/test_bins.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/tests/test_example_data.py` & `pyrsm-0.8.1.5/tests/test_example_data.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/tests/test_perf.py` & `pyrsm-0.8.1.5/tests/test_perf.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/tests/test_regression.py` & `pyrsm-0.8.1.5/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/tests/test_stats.py` & `pyrsm-0.8.1.5/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.1.4/tests/test_utils.py` & `pyrsm-0.8.1.5/tests/test_utils.py`

 * *Files identical despite different names*

