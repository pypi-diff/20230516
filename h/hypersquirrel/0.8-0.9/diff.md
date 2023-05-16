# Comparing `tmp/hypersquirrel-0.8.tar.gz` & `tmp/hypersquirrel-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypersquirrel-0.8.tar", last modified: Sat Oct  9 08:13:48 2021, max compression
+gzip compressed data, was "hypersquirrel-0.9.tar", last modified: Thu Nov 18 00:15:36 2021, max compression
```

## Comparing `hypersquirrel-0.8.tar` & `hypersquirrel-0.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 08:13:48.637275 hypersquirrel-0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2021-10-09 08:13:34.000000 hypersquirrel-0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      730 2021-10-09 08:13:48.633275 hypersquirrel-0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      381 2021-10-09 08:13:34.000000 hypersquirrel-0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 08:13:48.629275 hypersquirrel-0.8/hypersquirrel/
--rw-r--r--   0 runner    (1001) docker     (121)       89 2021-10-09 08:13:34.000000 hypersquirrel-0.8/hypersquirrel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-09 08:13:34.000000 hypersquirrel-0.8/hypersquirrel/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1013 2021-10-09 08:13:34.000000 hypersquirrel-0.8/hypersquirrel/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 08:13:48.633275 hypersquirrel-0.8/hypersquirrel/scraper/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-09 08:13:34.000000 hypersquirrel-0.8/hypersquirrel/scraper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      547 2021-10-09 08:13:34.000000 hypersquirrel-0.8/hypersquirrel/scraper/buondua.py
--rw-r--r--   0 runner    (1001) docker     (121)      861 2021-10-09 08:13:34.000000 hypersquirrel-0.8/hypersquirrel/scraper/cosplayporntube.py
--rw-r--r--   0 runner    (1001) docker     (121)     1166 2021-10-09 08:13:34.000000 hypersquirrel-0.8/hypersquirrel/scraper/drts.py
--rw-r--r--   0 runner    (1001) docker     (121)     1539 2021-10-09 08:13:34.000000 hypersquirrel-0.8/hypersquirrel/scraper/ehen.py
--rw-r--r--   0 runner    (1001) docker     (121)     1274 2021-10-09 08:13:34.000000 hypersquirrel-0.8/hypersquirrel/scraper/fseg.py
--rw-r--r--   0 runner    (1001) docker     (121)      344 2021-10-09 08:13:34.000000 hypersquirrel-0.8/hypersquirrel/scraper/googleimagesearch.py
--rw-r--r--   0 runner    (1001) docker     (121)     1942 2021-10-09 08:13:34.000000 hypersquirrel-0.8/hypersquirrel/scraper/hcos.py
--rw-r--r--   0 runner    (1001) docker     (121)     1010 2021-10-09 08:13:34.000000 hypersquirrel-0.8/hypersquirrel/scraper/hnlg.py
--rw-r--r--   0 runner    (1001) docker     (121)      994 2021-10-09 08:13:34.000000 hypersquirrel-0.8/hypersquirrel/scraper/lgbb.py
--rw-r--r--   0 runner    (1001) docker     (121)     1167 2021-10-09 08:13:34.000000 hypersquirrel-0.8/hypersquirrel/scraper/nh.py
--rw-r--r--   0 runner    (1001) docker     (121)     1083 2021-10-09 08:13:34.000000 hypersquirrel-0.8/hypersquirrel/scraper/nlgs.py
--rw-r--r--   0 runner    (1001) docker     (121)      462 2021-10-09 08:13:34.000000 hypersquirrel-0.8/hypersquirrel/scraper/opendir.py
--rw-r--r--   0 runner    (1001) docker     (121)      816 2021-10-09 08:13:34.000000 hypersquirrel-0.8/hypersquirrel/scraper/reddit.py
--rw-r--r--   0 runner    (1001) docker     (121)      686 2021-10-09 08:13:34.000000 hypersquirrel-0.8/hypersquirrel/scraper/sb.py
--rw-r--r--   0 runner    (1001) docker     (121)      826 2021-10-09 08:13:34.000000 hypersquirrel-0.8/hypersquirrel/scraper/sbgx.py
--rw-r--r--   0 runner    (1001) docker     (121)      607 2021-10-09 08:13:34.000000 hypersquirrel-0.8/hypersquirrel/scraper/v2ph.py
--rw-r--r--   0 runner    (1001) docker     (121)     2473 2021-10-09 08:13:34.000000 hypersquirrel-0.8/hypersquirrel/scraper/vg.py
--rw-r--r--   0 runner    (1001) docker     (121)      850 2021-10-09 08:13:34.000000 hypersquirrel-0.8/hypersquirrel/scraper/xh.py
--rw-r--r--   0 runner    (1001) docker     (121)     1515 2021-10-09 08:13:34.000000 hypersquirrel-0.8/hypersquirrel/scraper/xv.py
--rw-r--r--   0 runner    (1001) docker     (121)     1664 2021-10-09 08:13:34.000000 hypersquirrel-0.8/hypersquirrel/scraper/youtubeapi.py
--rw-r--r--   0 runner    (1001) docker     (121)     3185 2021-10-09 08:13:34.000000 hypersquirrel-0.8/hypersquirrel/scraperfactory.py
--rw-r--r--   0 runner    (1001) docker     (121)      369 2021-10-09 08:13:34.000000 hypersquirrel-0.8/hypersquirrel/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 08:13:48.633275 hypersquirrel-0.8/hypersquirrel/watchlist/
--rw-r--r--   0 runner    (1001) docker     (121)      833 2021-10-09 08:13:34.000000 hypersquirrel-0.8/hypersquirrel/watchlist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 08:13:48.633275 hypersquirrel-0.8/hypersquirrel/watchlist/decorator/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-09 08:13:34.000000 hypersquirrel-0.8/hypersquirrel/watchlist/decorator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      125 2021-10-09 08:13:34.000000 hypersquirrel-0.8/hypersquirrel/watchlist/decorator/maxitems.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 08:13:48.633275 hypersquirrel-0.8/hypersquirrel/watchlist/validator/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-09 08:13:34.000000 hypersquirrel-0.8/hypersquirrel/watchlist/validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      136 2021-10-09 08:13:34.000000 hypersquirrel-0.8/hypersquirrel/watchlist/validator/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      329 2021-10-09 08:13:34.000000 hypersquirrel-0.8/hypersquirrel/watchlist/validator/paged.py
--rw-r--r--   0 runner    (1001) docker     (121)      884 2021-10-09 08:13:34.000000 hypersquirrel-0.8/hypersquirrel/watchlist/validatorfactory.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 08:13:48.633275 hypersquirrel-0.8/hypersquirrel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      730 2021-10-09 08:13:48.000000 hypersquirrel-0.8/hypersquirrel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1304 2021-10-09 08:13:48.000000 hypersquirrel-0.8/hypersquirrel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-09 08:13:48.000000 hypersquirrel-0.8/hypersquirrel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       51 2021-10-09 08:13:48.000000 hypersquirrel-0.8/hypersquirrel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2021-10-09 08:13:48.000000 hypersquirrel-0.8/hypersquirrel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-09 08:13:48.637275 hypersquirrel-0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      609 2021-10-09 08:13:35.000000 hypersquirrel-0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 00:15:36.771202 hypersquirrel-0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1068 2021-11-18 00:15:26.000000 hypersquirrel-0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      730 2021-11-18 00:15:36.771202 hypersquirrel-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      381 2021-11-18 00:15:26.000000 hypersquirrel-0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 00:15:36.767202 hypersquirrel-0.9/hypersquirrel/
+-rw-r--r--   0 runner    (1001) docker     (121)       89 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1013 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 00:15:36.767202 hypersquirrel-0.9/hypersquirrel/scraper/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/scraper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      547 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/scraper/buondua.py
+-rw-r--r--   0 runner    (1001) docker     (121)      861 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/scraper/cosplayporntube.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1166 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/scraper/drts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1539 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/scraper/ehen.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1274 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/scraper/fseg.py
+-rw-r--r--   0 runner    (1001) docker     (121)      344 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/scraper/googleimagesearch.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1942 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/scraper/hcos.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1010 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/scraper/hnlg.py
+-rw-r--r--   0 runner    (1001) docker     (121)      994 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/scraper/lgbb.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1167 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/scraper/nh.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1083 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/scraper/nlgs.py
+-rw-r--r--   0 runner    (1001) docker     (121)      462 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/scraper/opendir.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1117 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/scraper/reddit.py
+-rw-r--r--   0 runner    (1001) docker     (121)      686 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/scraper/sb.py
+-rw-r--r--   0 runner    (1001) docker     (121)      826 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/scraper/sbgx.py
+-rw-r--r--   0 runner    (1001) docker     (121)      607 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/scraper/v2ph.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2473 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/scraper/vg.py
+-rw-r--r--   0 runner    (1001) docker     (121)      850 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/scraper/xh.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1515 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/scraper/xv.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1664 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/scraper/youtubeapi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3185 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/scraperfactory.py
+-rw-r--r--   0 runner    (1001) docker     (121)      369 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 00:15:36.767202 hypersquirrel-0.9/hypersquirrel/watchlist/
+-rw-r--r--   0 runner    (1001) docker     (121)      833 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/watchlist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 00:15:36.771202 hypersquirrel-0.9/hypersquirrel/watchlist/decorator/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/watchlist/decorator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      125 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/watchlist/decorator/maxitems.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 00:15:36.771202 hypersquirrel-0.9/hypersquirrel/watchlist/validator/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/watchlist/validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      136 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/watchlist/validator/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)      329 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/watchlist/validator/paged.py
+-rw-r--r--   0 runner    (1001) docker     (121)      884 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/watchlist/validatorfactory.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 00:15:36.767202 hypersquirrel-0.9/hypersquirrel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      730 2021-11-18 00:15:36.000000 hypersquirrel-0.9/hypersquirrel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1304 2021-11-18 00:15:36.000000 hypersquirrel-0.9/hypersquirrel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-18 00:15:36.000000 hypersquirrel-0.9/hypersquirrel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       51 2021-11-18 00:15:36.000000 hypersquirrel-0.9/hypersquirrel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2021-11-18 00:15:36.000000 hypersquirrel-0.9/hypersquirrel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-18 00:15:36.771202 hypersquirrel-0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      609 2021-11-18 00:15:27.000000 hypersquirrel-0.9/setup.py
```

### Comparing `hypersquirrel-0.8/LICENSE` & `hypersquirrel-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hypersquirrel-0.8/PKG-INFO` & `hypersquirrel-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypersquirrel
-Version: 0.8
+Version: 0.9
 Summary: Scrapes posts from various websites
 Home-page: UNKNOWN
 Author: vka
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `hypersquirrel-0.8/hypersquirrel/entry.py` & `hypersquirrel-0.9/hypersquirrel/entry.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-0.8/hypersquirrel/scraper/buondua.py` & `hypersquirrel-0.9/hypersquirrel/scraper/buondua.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-0.8/hypersquirrel/scraper/cosplayporntube.py` & `hypersquirrel-0.9/hypersquirrel/scraper/cosplayporntube.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-0.8/hypersquirrel/scraper/drts.py` & `hypersquirrel-0.9/hypersquirrel/scraper/drts.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-0.8/hypersquirrel/scraper/ehen.py` & `hypersquirrel-0.9/hypersquirrel/scraper/ehen.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-0.8/hypersquirrel/scraper/fseg.py` & `hypersquirrel-0.9/hypersquirrel/scraper/fseg.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-0.8/hypersquirrel/scraper/hcos.py` & `hypersquirrel-0.9/hypersquirrel/scraper/hcos.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-0.8/hypersquirrel/scraper/hnlg.py` & `hypersquirrel-0.9/hypersquirrel/scraper/hnlg.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-0.8/hypersquirrel/scraper/lgbb.py` & `hypersquirrel-0.9/hypersquirrel/scraper/lgbb.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-0.8/hypersquirrel/scraper/nh.py` & `hypersquirrel-0.9/hypersquirrel/scraper/nh.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-0.8/hypersquirrel/scraper/nlgs.py` & `hypersquirrel-0.9/hypersquirrel/scraper/nlgs.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-0.8/hypersquirrel/scraper/sb.py` & `hypersquirrel-0.9/hypersquirrel/scraper/sb.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-0.8/hypersquirrel/scraper/sbgx.py` & `hypersquirrel-0.9/hypersquirrel/scraper/sbgx.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-0.8/hypersquirrel/scraper/v2ph.py` & `hypersquirrel-0.9/hypersquirrel/scraper/v2ph.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-0.8/hypersquirrel/scraper/vg.py` & `hypersquirrel-0.9/hypersquirrel/scraper/vg.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-0.8/hypersquirrel/scraper/xh.py` & `hypersquirrel-0.9/hypersquirrel/scraper/xh.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-0.8/hypersquirrel/scraper/xv.py` & `hypersquirrel-0.9/hypersquirrel/scraper/xv.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-0.8/hypersquirrel/scraper/youtubeapi.py` & `hypersquirrel-0.9/hypersquirrel/scraper/youtubeapi.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-0.8/hypersquirrel/scraperfactory.py` & `hypersquirrel-0.9/hypersquirrel/scraperfactory.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-0.8/hypersquirrel/watchlist/__init__.py` & `hypersquirrel-0.9/hypersquirrel/watchlist/__init__.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-0.8/hypersquirrel/watchlist/validatorfactory.py` & `hypersquirrel-0.9/hypersquirrel/watchlist/validatorfactory.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-0.8/hypersquirrel.egg-info/PKG-INFO` & `hypersquirrel-0.9/hypersquirrel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypersquirrel
-Version: 0.8
+Version: 0.9
 Summary: Scrapes posts from various websites
 Home-page: UNKNOWN
 Author: vka
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `hypersquirrel-0.8/hypersquirrel.egg-info/SOURCES.txt` & `hypersquirrel-0.9/hypersquirrel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hypersquirrel-0.8/setup.py` & `hypersquirrel-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hypersquirrel",
-    version="0.8",
+    version="0.9",
     author="vka",
     description="Scrapes posts from various websites",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(exclude=("test",)),
     classifiers=[
         "Programming Language :: Python :: 3",
```

