# Comparing `tmp/hatch_util-0.0.2.tar.gz` & `tmp/hatch_util-0.0.3.tar.gz`

## Comparing `hatch_util-0.0.2.tar` & `hatch_util-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hatch_util-0.0.2/requirements.txt
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 hatch_util-0.0.2/tox.ini
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 hatch_util-0.0.2/src/hatch_util/__about__.py
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 hatch_util-0.0.2/src/hatch_util/__init__.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 hatch_util-0.0.2/src/hatch_util/compose.py
--rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 hatch_util-0.0.2/src/hatch_util/convert.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 hatch_util-0.0.2/src/hatch_util/environ.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 hatch_util-0.0.2/src/hatch_util/hash_object.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 hatch_util-0.0.2/src/hatch_util/misc.py
--rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 hatch_util-0.0.2/src/hatch_util/parser_argument.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 hatch_util-0.0.2/src/hatch_util/period.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 hatch_util-0.0.2/src/hatch_util/string.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 hatch_util-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 hatch_util-0.0.2/tests/test_convert.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 hatch_util-0.0.2/tests/test_exist.py
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 hatch_util-0.0.2/tests/test_hash_object.py
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 hatch_util-0.0.2/tests/test_parsor.py
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 hatch_util-0.0.2/.gitignore
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 hatch_util-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 hatch_util-0.0.2/README.md
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 hatch_util-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 hatch_util-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hatch_util-0.0.3/requirements.txt
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 hatch_util-0.0.3/setup.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 hatch_util-0.0.3/tox.ini
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 hatch_util-0.0.3/src/hatch_util/__about__.py
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 hatch_util-0.0.3/src/hatch_util/__init__.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 hatch_util-0.0.3/src/hatch_util/compose.py
+-rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 hatch_util-0.0.3/src/hatch_util/convert.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 hatch_util-0.0.3/src/hatch_util/environ.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 hatch_util-0.0.3/src/hatch_util/hash_object.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 hatch_util-0.0.3/src/hatch_util/misc.py
+-rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 hatch_util-0.0.3/src/hatch_util/parser_argument.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 hatch_util-0.0.3/src/hatch_util/period.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 hatch_util-0.0.3/src/hatch_util/string.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 hatch_util-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 hatch_util-0.0.3/tests/test_convert.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 hatch_util-0.0.3/tests/test_exist.py
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 hatch_util-0.0.3/tests/test_hash_object.py
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 hatch_util-0.0.3/tests/test_parsor.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 hatch_util-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 hatch_util-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 hatch_util-0.0.3/README.md
+-rw-r--r--   0        0        0     3535 2020-02-02 00:00:00.000000 hatch_util-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 hatch_util-0.0.3/PKG-INFO
```

### Comparing `hatch_util-0.0.2/src/hatch_util/__init__.py` & `hatch_util-0.0.3/src/hatch_util/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch_util-0.0.2/src/hatch_util/convert.py` & `hatch_util-0.0.3/src/hatch_util/convert.py`

 * *Files identical despite different names*

### Comparing `hatch_util-0.0.2/src/hatch_util/parser_argument.py` & `hatch_util-0.0.3/src/hatch_util/parser_argument.py`

 * *Files identical despite different names*

### Comparing `hatch_util-0.0.2/tests/test_convert.py` & `hatch_util-0.0.3/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `hatch_util-0.0.2/tests/test_hash_object.py` & `hatch_util-0.0.3/tests/test_hash_object.py`

 * *Files identical despite different names*

### Comparing `hatch_util-0.0.2/tests/test_parsor.py` & `hatch_util-0.0.3/tests/test_parsor.py`

 * *Files identical despite different names*

### Comparing `hatch_util-0.0.2/.gitignore` & `hatch_util-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `hatch_util-0.0.2/LICENSE.txt` & `hatch_util-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hatch_util-0.0.2/README.md` & `hatch_util-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `hatch_util-0.0.2/pyproject.toml` & `hatch_util-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -162,8 +162,8 @@
   "/docs",
 ]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/hatch_util"]
 
 [tool.hatch.publish.index]
-disable = false
+disable = true
```

### Comparing `hatch_util-0.0.2/PKG-INFO` & `hatch_util-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hatch-util
-Version: 0.0.2
+Version: 0.0.3
 Summary: i-util contain functions so useful for processing data projects
 Project-URL: Documentation, https://github.com/unknown/hatch-util#readme
 Project-URL: Issues, https://github.com/unknown/hatch-util/issues
 Project-URL: Source, https://github.com/unknown/hatch-util
 Author-email: HuynhSieu <sieu.huynh@innotech.vn>
 License-Expression: MIT
 License-File: LICENSE.txt
```

