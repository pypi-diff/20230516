# Comparing `tmp/pykebab-0.6.0.tar.gz` & `tmp/pykebab-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykebab-0.6.0.tar", max compression
+gzip compressed data, was "pykebab-0.6.1.tar", max compression
```

## Comparing `pykebab-0.6.0.tar` & `pykebab-0.6.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      821 2023-03-28 08:28:34.526031 pykebab-0.6.0/kebab/__init__.py
--rw-r--r--   0        0        0     3920 2023-03-28 08:28:34.526031 pykebab-0.6.0/kebab/aws.py
--rw-r--r--   0        0        0       40 2023-03-28 08:28:34.526031 pykebab-0.6.0/kebab/cli/__init__.py
--rw-r--r--   0        0        0     1801 2023-03-28 08:28:34.526031 pykebab-0.6.0/kebab/cli/cli.py
--rw-r--r--   0        0        0      798 2023-03-28 08:28:34.526031 pykebab-0.6.0/kebab/constants.py
--rw-r--r--   0        0        0       42 2023-03-28 08:28:34.526031 pykebab-0.6.0/kebab/exceptions.py
--rw-r--r--   0        0        0     2587 2023-03-28 08:28:34.526031 pykebab-0.6.0/kebab/k8s.py
--rw-r--r--   0        0        0      773 2023-03-28 08:28:34.526031 pykebab-0.6.0/kebab/loader.py
--rw-r--r--   0        0        0     2368 2023-03-28 08:28:34.526031 pykebab-0.6.0/kebab/magic.py
--rw-r--r--   0        0        0     2108 2023-03-28 08:28:34.526031 pykebab-0.6.0/kebab/openers.py
--rw-r--r--   0        0        0    19970 2023-03-28 08:28:34.526031 pykebab-0.6.0/kebab/sources.py
--rw-r--r--   0        0        0     4825 2023-03-28 08:28:34.526031 pykebab-0.6.0/kebab/utils.py
--rw-r--r--   0        0        0     1025 2023-03-28 08:28:34.526031 pykebab-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      889 1970-01-01 00:00:00.000000 pykebab-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      821 2022-11-06 03:32:21.214628 pykebab-0.6.1/kebab/__init__.py
+-rw-r--r--   0        0        0     3920 2022-11-06 03:32:21.214802 pykebab-0.6.1/kebab/aws.py
+-rw-r--r--   0        0        0       40 2022-11-06 03:32:21.214897 pykebab-0.6.1/kebab/cli/__init__.py
+-rw-r--r--   0        0        0     1801 2023-01-05 03:45:44.147407 pykebab-0.6.1/kebab/cli/cli.py
+-rw-r--r--   0        0        0      798 2023-02-03 08:02:22.409418 pykebab-0.6.1/kebab/constants.py
+-rw-r--r--   0        0        0       42 2022-11-06 03:32:21.215088 pykebab-0.6.1/kebab/exceptions.py
+-rw-r--r--   0        0        0     2587 2023-01-05 03:45:44.147717 pykebab-0.6.1/kebab/k8s.py
+-rw-r--r--   0        0        0      773 2023-03-28 07:51:19.037015 pykebab-0.6.1/kebab/loader.py
+-rw-r--r--   0        0        0     2368 2022-11-06 03:32:21.215294 pykebab-0.6.1/kebab/magic.py
+-rw-r--r--   0        0        0     2108 2023-03-25 11:13:55.662982 pykebab-0.6.1/kebab/openers.py
+-rw-r--r--   0        0        0    19971 2023-05-16 19:08:58.975736 pykebab-0.6.1/kebab/sources.py
+-rw-r--r--   0        0        0     4825 2023-01-05 03:45:44.148106 pykebab-0.6.1/kebab/utils.py
+-rw-r--r--   0        0        0     1025 2023-05-16 19:10:07.348057 pykebab-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      889 1970-01-01 00:00:00.000000 pykebab-0.6.1/PKG-INFO
```

### Comparing `pykebab-0.6.0/kebab/__init__.py` & `pykebab-0.6.1/kebab/__init__.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.6.0/kebab/aws.py` & `pykebab-0.6.1/kebab/aws.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.6.0/kebab/cli/cli.py` & `pykebab-0.6.1/kebab/cli/cli.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.6.0/kebab/constants.py` & `pykebab-0.6.1/kebab/constants.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.6.0/kebab/k8s.py` & `pykebab-0.6.1/kebab/k8s.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.6.0/kebab/loader.py` & `pykebab-0.6.1/kebab/loader.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.6.0/kebab/magic.py` & `pykebab-0.6.1/kebab/magic.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.6.0/kebab/openers.py` & `pykebab-0.6.1/kebab/openers.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.6.0/kebab/sources.py` & `pykebab-0.6.1/kebab/sources.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,15 @@
                 self._reload_timer
                 and threading.current_thread().ident != self._reload_timer.ident
             ):
                 _logger.debug(f"reload timer was already set for {self}")
                 self._reload_timer.args = (reload_interval_in_secs, False)
             else:
                 if not self._reload_timer:
-                    _logger.info(
+                    _logger.debug(
                         f"setting timer to reload per {reload_interval_in_secs} secs "
                         f"for {self} "
                     )
                 # noinspection PyTypeChecker
                 self._reload_timer = threading.Timer(
                     interval=reload_interval_in_secs,
                     function=self.reload,
```

### Comparing `pykebab-0.6.0/kebab/utils.py` & `pykebab-0.6.1/kebab/utils.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.6.0/pyproject.toml` & `pykebab-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pykebab"
-version = "0.6.0"
+version = "0.6.1"
 description = ""
 authors = ["Yangming Huang <leonmax@gmail.com>"]
 packages = [
     { include = "kebab" },
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `pykebab-0.6.0/PKG-INFO` & `pykebab-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykebab
-Version: 0.6.0
+Version: 0.6.1
 Summary: 
 Author: Yangming Huang
 Author-email: leonmax@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

