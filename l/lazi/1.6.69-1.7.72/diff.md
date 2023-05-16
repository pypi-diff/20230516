# Comparing `tmp/lazi-1.6.69.tar.gz` & `tmp/lazi-1.7.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazi-1.6.69.tar", max compression
+gzip compressed data, was "lazi-1.7.72.tar", max compression
```

## Comparing `lazi-1.6.69.tar` & `lazi-1.7.72.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    34523 2023-05-10 08:04:21.503726 lazi-1.6.69/LICENSE
--rw-r--r--   0        0        0     2012 2023-05-16 03:17:42.603835 lazi-1.6.69/README.md
--rw-r--r--   0        0        0      169 2023-05-16 03:17:42.603835 lazi-1.6.69/lazi/auto.py
--rw-r--r--   0        0        0      284 2023-05-12 07:30:19.063612 lazi-1.6.69/lazi/conf/auto.py
--rw-r--r--   0        0        0     1238 2023-05-16 03:15:31.114120 lazi-1.6.69/lazi/conf/base.py
--rw-r--r--   0        0        0     4738 2023-05-15 22:42:51.727662 lazi-1.6.69/lazi/conf/conf.py
--rw-r--r--   0        0        0       99 2023-05-15 22:42:51.727662 lazi-1.6.69/lazi/conf/test.py
--rw-r--r--   0        0        0      375 2023-05-16 03:17:42.603835 lazi-1.6.69/lazi/core/__init__.py
--rw-r--r--   0        0        0     3339 2023-05-16 03:17:42.603835 lazi-1.6.69/lazi/core/finder.py
--rw-r--r--   0        0        0     3533 2023-05-16 03:17:42.607835 lazi-1.6.69/lazi/core/loader.py
--rw-r--r--   0        0        0     4127 2023-05-16 03:17:42.607835 lazi-1.6.69/lazi/core/module.py
--rw-r--r--   0        0        0     1756 2023-05-15 22:42:51.727662 lazi-1.6.69/lazi/core/spec.py
--rw-r--r--   0        0        0       46 2023-05-12 00:02:04.162155 lazi-1.6.69/lazi/util/__init__.py
--rw-r--r--   0        0        0      448 2023-05-15 22:42:51.727662 lazi-1.6.69/lazi/util/debug.py
--rw-r--r--   0        0        0      146 2023-05-15 22:42:51.727662 lazi-1.6.69/lazi/util/functional.py
--rw-r--r--   0        0        0        0 2023-05-15 22:42:51.727662 lazi-1.6.69/lazi/util/util.py
--rw-r--r--   0        0        0     1555 2023-05-16 03:18:18.516303 lazi-1.6.69/pyproject.toml
--rw-r--r--   0        0        0      203 2023-05-15 22:42:51.727662 lazi-1.6.69/tests/standalone/sa_array.py
--rw-r--r--   0        0        0      273 2023-05-15 22:42:51.727662 lazi-1.6.69/tests/standalone/sa_pygments.py
--rw-r--r--   0        0        0      380 2023-05-15 22:42:51.727662 lazi-1.6.69/tests/test_array.py
--rw-r--r--   0        0        0      901 2023-05-15 22:42:51.727662 lazi-1.6.69/tests/test_django.py
--rw-r--r--   0        0        0      810 2023-05-15 22:42:51.727662 lazi-1.6.69/tests/test_pygments.py
--rw-r--r--   0        0        0      775 2023-05-15 22:42:51.727662 lazi-1.6.69/tests/test_requests.py
--rw-r--r--   0        0        0     2795 2023-05-15 22:42:51.727662 lazi-1.6.69/tests/test_rich.py
--rw-r--r--   0        0        0     3107 1970-01-01 00:00:00.000000 lazi-1.6.69/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-10 08:04:21.503726 lazi-1.7.72/LICENSE
+-rw-r--r--   0        0        0     1913 2023-05-16 03:20:51.902303 lazi-1.7.72/README.md
+-rw-r--r--   0        0        0      169 2023-05-16 03:17:42.603835 lazi-1.7.72/lazi/auto.py
+-rw-r--r--   0        0        0      284 2023-05-12 07:30:19.063612 lazi-1.7.72/lazi/conf/auto.py
+-rw-r--r--   0        0        0     1154 2023-05-16 03:26:57.047060 lazi-1.7.72/lazi/conf/base.py
+-rw-r--r--   0        0        0     4738 2023-05-15 22:42:51.727662 lazi-1.7.72/lazi/conf/conf.py
+-rw-r--r--   0        0        0       99 2023-05-15 22:42:51.727662 lazi-1.7.72/lazi/conf/test.py
+-rw-r--r--   0        0        0      375 2023-05-16 03:17:42.603835 lazi-1.7.72/lazi/core/__init__.py
+-rw-r--r--   0        0        0     3339 2023-05-16 03:17:42.603835 lazi-1.7.72/lazi/core/finder.py
+-rw-r--r--   0        0        0     3533 2023-05-16 03:17:42.607835 lazi-1.7.72/lazi/core/loader.py
+-rw-r--r--   0        0        0     2907 2023-05-16 03:32:57.095748 lazi-1.7.72/lazi/core/module.py
+-rw-r--r--   0        0        0     1756 2023-05-15 22:42:51.727662 lazi-1.7.72/lazi/core/spec.py
+-rw-r--r--   0        0        0       46 2023-05-12 00:02:04.162155 lazi-1.7.72/lazi/util/__init__.py
+-rw-r--r--   0        0        0      448 2023-05-15 22:42:51.727662 lazi-1.7.72/lazi/util/debug.py
+-rw-r--r--   0        0        0      146 2023-05-15 22:42:51.727662 lazi-1.7.72/lazi/util/functional.py
+-rw-r--r--   0        0        0        0 2023-05-15 22:42:51.727662 lazi-1.7.72/lazi/util/util.py
+-rw-r--r--   0        0        0     1555 2023-05-16 03:34:03.788625 lazi-1.7.72/pyproject.toml
+-rw-r--r--   0        0        0      203 2023-05-15 22:42:51.727662 lazi-1.7.72/tests/standalone/sa_array.py
+-rw-r--r--   0        0        0      273 2023-05-15 22:42:51.727662 lazi-1.7.72/tests/standalone/sa_pygments.py
+-rw-r--r--   0        0        0      380 2023-05-15 22:42:51.727662 lazi-1.7.72/tests/test_array.py
+-rw-r--r--   0        0        0      901 2023-05-15 22:42:51.727662 lazi-1.7.72/tests/test_django.py
+-rw-r--r--   0        0        0      810 2023-05-15 22:42:51.727662 lazi-1.7.72/tests/test_pygments.py
+-rw-r--r--   0        0        0      775 2023-05-15 22:42:51.727662 lazi-1.7.72/tests/test_requests.py
+-rw-r--r--   0        0        0     2795 2023-05-15 22:42:51.727662 lazi-1.7.72/tests/test_rich.py
+-rw-r--r--   0        0        0     3008 1970-01-01 00:00:00.000000 lazi-1.7.72/PKG-INFO
```

### Comparing `lazi-1.6.69/LICENSE` & `lazi-1.7.72/LICENSE`

 * *Files identical despite different names*

### Comparing `lazi-1.6.69/README.md` & `lazi-1.7.72/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 ```shell
 poetry add lazi
 ```
 ```shell
 DEBUG_TRACING=1 python3
 ```
 ```pycon
-# (lazi-py3.11) lazi λ DEBUG_TRACING=1 python
-Python 3.11.2 (main, Mar 13 2023, 12:18:29) [GCC 12.2.0] on linux
+Python 3.11.2
 >>> import lazi.auto
 [140402520740240] +Finder refs:0 inst:0 sys:5
 >>> from django import test
 [140402520858096] <get> LAZY django[.test]
 [140402518572896] <set> LAZY django.utils[.version] [140402518571056]
 [140402518571056] <get> LAZY django.utils.version[.get_version]
 [140402518606128] <get> LAZY django.utils.regex_helper[._lazy_re_compile]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `lazi-1.6.69/lazi/conf/base.py` & `lazi-1.7.72/lazi/conf/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,13 +8,12 @@
 DEBUG_TRACING: int = 0                  # Enable debug traces.
 
 LAZI_AUTO_INSTALL: bool = True          # Automatically install when importing lazi.auto.
 CORE_AUTO_INSTALL: bool = False         # Automatically install when importing lazi.core.
 FORCE_LOAD_MODULE: bool = False         # Immediately call exec_module() on imported modules.
 NO_STDLIB_MODULES: bool = True          # Disable loader hooking for stdlib modules.
 DISABLE_LOAD_HOOK: bool = False         # Disable all loader hooks.
-NO_DICT_LAZY_ATTR: bool = True          # Trigger exec_module() on __dict__ access.
 
 CONF_NO_CACHING: bool | None = None     # Disable caching of conf vars.
 #                                         - None: Use the default caching behavior, which will disable
 #                                                 caching if `lazi.core` is already present in sys.modules
 #                                                 when lazi.conf.conf is imported.
```

### Comparing `lazi-1.6.69/lazi/conf/conf.py` & `lazi-1.7.72/lazi/conf/conf.py`

 * *Files identical despite different names*

### Comparing `lazi-1.6.69/lazi/core/finder.py` & `lazi-1.7.72/lazi/core/finder.py`

 * *Files identical despite different names*

### Comparing `lazi-1.6.69/lazi/core/loader.py` & `lazi-1.7.72/lazi/core/loader.py`

 * *Files identical despite different names*

### Comparing `lazi-1.6.69/lazi/core/spec.py` & `lazi-1.7.72/lazi/core/spec.py`

 * *Files identical despite different names*

### Comparing `lazi-1.6.69/pyproject.toml` & `lazi-1.7.72/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lazi"
-version = "1.6.69"
+version = "1.7.72"
 description = "A lightweight and extensible way to implement lazy imports globally."
 authors = ["Phillip Sitbon <phillip.sitbon@gmail.com>"]
 readme = "README.md"
 license = "AGPLv3"
 repository = "https://github.com/sitbon/lazi"
 classifiers= [
     "Environment :: Web Environment",
```

### Comparing `lazi-1.6.69/tests/test_django.py` & `lazi-1.7.72/tests/test_django.py`

 * *Files identical despite different names*

### Comparing `lazi-1.6.69/tests/test_pygments.py` & `lazi-1.7.72/tests/test_pygments.py`

 * *Files identical despite different names*

### Comparing `lazi-1.6.69/tests/test_requests.py` & `lazi-1.7.72/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `lazi-1.6.69/tests/test_rich.py` & `lazi-1.7.72/tests/test_rich.py`

 * *Files identical despite different names*

### Comparing `lazi-1.6.69/PKG-INFO` & `lazi-1.7.72/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazi
-Version: 1.6.69
+Version: 1.7.72
 Summary: A lightweight and extensible way to implement lazy imports globally.
 Home-page: https://github.com/sitbon/lazi
 License: AGPLv3
 Author: Phillip Sitbon
 Author-email: phillip.sitbon@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Environment :: Web Environment
@@ -37,16 +37,15 @@
 ```shell
 poetry add lazi
 ```
 ```shell
 DEBUG_TRACING=1 python3
 ```
 ```pycon
-# (lazi-py3.11) lazi λ DEBUG_TRACING=1 python
-Python 3.11.2 (main, Mar 13 2023, 12:18:29) [GCC 12.2.0] on linux
+Python 3.11.2
 >>> import lazi.auto
 [140402520740240] +Finder refs:0 inst:0 sys:5
 >>> from django import test
 [140402520858096] <get> LAZY django[.test]
 [140402518572896] <set> LAZY django.utils[.version] [140402518571056]
 [140402518571056] <get> LAZY django.utils.version[.get_version]
 [140402518606128] <get> LAZY django.utils.regex_helper[._lazy_re_compile]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

