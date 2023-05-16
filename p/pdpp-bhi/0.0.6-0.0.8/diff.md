# Comparing `tmp/pdpp-bhi-0.0.6.tar.gz` & `tmp/pdpp-bhi-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdpp-bhi-0.0.6.tar", last modified: Thu Apr 20 16:33:29 2023, max compression
+gzip compressed data, was "pdpp-bhi-0.0.8.tar", last modified: Wed Apr 26 05:58:56 2023, max compression
```

## Comparing `pdpp-bhi-0.0.6.tar` & `pdpp-bhi-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:33:29.159834 pdpp-bhi-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-20 16:33:29.159834 pdpp-bhi-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 16:33:18.000000 pdpp-bhi-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:33:29.159834 pdpp-bhi-0.0.6/pdpp_bhi/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 16:33:18.000000 pdpp-bhi-0.0.6/pdpp_bhi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-04-20 16:33:18.000000 pdpp-bhi-0.0.6/pdpp_bhi/pdpp_bhi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:33:29.159834 pdpp-bhi-0.0.6/pdpp_bhi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-20 16:33:29.000000 pdpp-bhi-0.0.6/pdpp_bhi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-20 16:33:29.000000 pdpp-bhi-0.0.6/pdpp_bhi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 16:33:29.000000 pdpp-bhi-0.0.6/pdpp_bhi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-20 16:33:29.000000 pdpp-bhi-0.0.6/pdpp_bhi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-20 16:33:29.000000 pdpp-bhi-0.0.6/pdpp_bhi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 16:33:29.159834 pdpp-bhi-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-20 16:33:18.000000 pdpp-bhi-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:58:56.532029 pdpp-bhi-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-26 05:58:56.532029 pdpp-bhi-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 05:58:38.000000 pdpp-bhi-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:58:56.532029 pdpp-bhi-0.0.8/pdpp_bhi/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 05:58:38.000000 pdpp-bhi-0.0.8/pdpp_bhi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8335 2023-04-26 05:58:38.000000 pdpp-bhi-0.0.8/pdpp_bhi/pdpp_bhi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:58:56.532029 pdpp-bhi-0.0.8/pdpp_bhi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-26 05:58:56.000000 pdpp-bhi-0.0.8/pdpp_bhi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-26 05:58:56.000000 pdpp-bhi-0.0.8/pdpp_bhi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 05:58:56.000000 pdpp-bhi-0.0.8/pdpp_bhi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-26 05:58:56.000000 pdpp-bhi-0.0.8/pdpp_bhi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-26 05:58:56.000000 pdpp-bhi-0.0.8/pdpp_bhi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 05:58:56.532029 pdpp-bhi-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-26 05:58:38.000000 pdpp-bhi-0.0.8/setup.py
```

### Comparing `pdpp-bhi-0.0.6/pdpp_bhi/pdpp_bhi.py` & `pdpp-bhi-0.0.8/pdpp_bhi/pdpp_bhi.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,15 +138,15 @@
         self._status = 'finished'
     
     def score(self, return_result=False):
         if not self._status == 'finished':
             raise Exception('You must run a full iteration of `iter_test()` first to score.')
         
         merged = self.predictions.merge(self.target, on='prediction_id')
-        merged = merged.dropna(subset='target_rating')
+        merged = merged.dropna(subset=['target_rating'])
 
         scores = {'total': smape_p1(merged.target_rating, merged.rating)}
         for idx in range(1, 5):
             sub_df = merged[merged.prediction_id.str.contains(f'updrs_{idx}')]
             scores[f'updrs_{idx}'] = smape_p1(sub_df.target_rating, sub_df.rating)
         
         if not return_result:
```

### Comparing `pdpp-bhi-0.0.6/setup.py` & `pdpp-bhi-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pdpp-bhi",
     packages=find_packages(exclude=[]),
     include_package_data=True,
-    version="0.0.6",
+    version="0.0.8",
     license="MIT",
     description="PDPP - BHI",
     author="Dohoon Lee",
     author_email="dohlee.bioinfo@gmail.com",
     long_description_content_type="text/markdown",
     url="https://github.com/dohlee/pdpp",
     keywords=[
```

