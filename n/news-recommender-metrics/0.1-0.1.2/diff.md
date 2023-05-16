# Comparing `tmp/news-recommender-metrics-0.1.tar.gz` & `tmp/news-recommender-metrics-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "news-recommender-metrics-0.1.tar", last modified: Thu May 11 12:34:16 2023, max compression
+gzip compressed data, was "news-recommender-metrics-0.1.2.tar", last modified: Tue May 16 08:26:07 2023, max compression
```

## Comparing `news-recommender-metrics-0.1.tar` & `news-recommender-metrics-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 12:34:16.116955 news-recommender-metrics-0.1/
--rw-rw-rw-   0        0        0     1092 2023-05-11 11:25:57.000000 news-recommender-metrics-0.1/LICENSE
--rw-rw-rw-   0        0        0      334 2023-05-11 12:34:16.110522 news-recommender-metrics-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      104 2023-05-11 11:25:57.000000 news-recommender-metrics-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-11 12:34:16.034873 news-recommender-metrics-0.1/news_recommender_metrics/
--rw-rw-rw-   0        0        0        0 2023-05-11 12:32:14.000000 news-recommender-metrics-0.1/news_recommender_metrics/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 12:34:16.099728 news-recommender-metrics-0.1/news_recommender_metrics.egg-info/
--rw-rw-rw-   0        0        0      334 2023-05-11 12:34:15.000000 news-recommender-metrics-0.1/news_recommender_metrics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-05-11 12:34:15.000000 news-recommender-metrics-0.1/news_recommender_metrics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 12:34:15.000000 news-recommender-metrics-0.1/news_recommender_metrics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-05-11 12:34:15.000000 news-recommender-metrics-0.1/news_recommender_metrics.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-11 12:34:16.118001 news-recommender-metrics-0.1/setup.cfg
--rw-rw-rw-   0        0        0      393 2023-05-11 11:53:26.000000 news-recommender-metrics-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 08:26:07.120692 news-recommender-metrics-0.1.2/
+-rw-rw-rw-   0        0        0     1092 2023-05-11 11:25:57.000000 news-recommender-metrics-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      336 2023-05-16 08:26:07.114862 news-recommender-metrics-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      104 2023-05-11 11:25:57.000000 news-recommender-metrics-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 08:26:07.037493 news-recommender-metrics-0.1.2/news_recommender_metrics/
+drwxrwxrwx   0        0        0        0 2023-05-16 08:26:07.086043 news-recommender-metrics-0.1.2/news_recommender_metrics/RADio/
+-rw-rw-rw-   0        0        0        0 2023-05-14 09:17:39.000000 news-recommender-metrics-0.1.2/news_recommender_metrics/RADio/__init__.py
+-rw-rw-rw-   0        0        0     2265 2023-05-16 08:20:45.000000 news-recommender-metrics-0.1.2/news_recommender_metrics/RADio/calibration.py
+-rw-rw-rw-   0        0        0      331 2023-05-16 08:20:45.000000 news-recommender-metrics-0.1.2/news_recommender_metrics/RADio/dart_metrics_abstract.py
+-rw-rw-rw-   0        0        0     2365 2023-05-14 09:30:23.000000 news-recommender-metrics-0.1.2/news_recommender_metrics/RADio/divergence_metrics.py
+-rw-rw-rw-   0        0        0       69 2023-05-16 08:25:17.000000 news-recommender-metrics-0.1.2/news_recommender_metrics/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 08:26:07.097033 news-recommender-metrics-0.1.2/news_recommender_metrics/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-16 08:21:40.000000 news-recommender-metrics-0.1.2/news_recommender_metrics/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 08:26:07.111737 news-recommender-metrics-0.1.2/news_recommender_metrics/utils/probability_mass_function/
+-rw-rw-rw-   0        0        0        0 2023-05-16 08:21:16.000000 news-recommender-metrics-0.1.2/news_recommender_metrics/utils/probability_mass_function/__init__.py
+-rw-rw-rw-   0        0        0      488 2023-05-16 08:20:45.000000 news-recommender-metrics-0.1.2/news_recommender_metrics/utils/probability_mass_function/probability_mass_function.py
+-rw-rw-rw-   0        0        0     1087 2023-05-16 08:20:45.000000 news-recommender-metrics-0.1.2/news_recommender_metrics/utils/probability_mass_function/rank_aware_probability_mass_function.py
+drwxrwxrwx   0        0        0        0 2023-05-16 08:26:07.071684 news-recommender-metrics-0.1.2/news_recommender_metrics.egg-info/
+-rw-rw-rw-   0        0        0      336 2023-05-16 08:26:06.000000 news-recommender-metrics-0.1.2/news_recommender_metrics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      748 2023-05-16 08:26:06.000000 news-recommender-metrics-0.1.2/news_recommender_metrics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 08:26:06.000000 news-recommender-metrics-0.1.2/news_recommender_metrics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-05-16 08:26:06.000000 news-recommender-metrics-0.1.2/news_recommender_metrics.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 08:26:07.120908 news-recommender-metrics-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      395 2023-05-16 08:24:56.000000 news-recommender-metrics-0.1.2/setup.py
```

### Comparing `news-recommender-metrics-0.1/LICENSE` & `news-recommender-metrics-0.1.2/LICENSE`

 * *Files identical despite different names*

