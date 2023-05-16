# Comparing `tmp/baseblock-0.2.22.tar.gz` & `tmp/baseblock-0.2.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baseblock-0.2.22.tar", max compression
+gzip compressed data, was "baseblock-0.2.23.tar", max compression
```

## Comparing `baseblock-0.2.22.tar` & `baseblock-0.2.23.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      509 2022-11-01 19:40:10.480205 baseblock-0.2.22/baseblock/__init__.py
--rw-r--r--   0        0        0     1665 2023-03-31 18:06:04.643612 baseblock-0.2.22/baseblock/base_object.py
--rw-r--r--   0        0        0     2206 2022-11-01 19:40:21.549334 baseblock-0.2.22/baseblock/common_utils.py
--rw-r--r--   0        0        0     3400 2022-11-01 19:40:24.233178 baseblock-0.2.22/baseblock/crypto_base.py
--rw-r--r--   0        0        0    17009 2022-11-29 00:36:47.898866 baseblock-0.2.22/baseblock/enforce_type.py
--rw-r--r--   0        0        0     6749 2023-01-10 20:33:14.114247 baseblock-0.2.22/baseblock/env_io.py
--rw-r--r--   0        0        0    25397 2023-02-07 00:55:29.559730 baseblock-0.2.22/baseblock/file_io.py
--rw-r--r--   0        0        0     1918 2022-11-01 19:40:37.387998 baseblock-0.2.22/baseblock/service_event_generator.py
--rw-r--r--   0        0        0     2320 2022-11-01 19:40:10.479705 baseblock-0.2.22/baseblock/stopwatch.py
--rw-r--r--   0        0        0     5147 2023-01-27 20:32:24.092475 baseblock-0.2.22/baseblock/text_matcher.py
--rw-r--r--   0        0        0    29945 2023-01-26 05:18:13.221964 baseblock-0.2.22/baseblock/text_utils.py
--rw-r--r--   0        0        0     1364 2022-11-01 19:40:49.507564 baseblock-0.2.22/baseblock/time_helper.py
--rw-r--r--   0        0        0     1344 2023-03-31 18:00:22.922736 baseblock-0.2.22/pyproject.toml
--rw-r--r--   0        0        0      506 2022-10-20 17:03:08.598380 baseblock-0.2.22/README.md
--rw-r--r--   0        0        0     1237 2023-03-31 18:06:51.071933 baseblock-0.2.22/setup.py
--rw-r--r--   0        0        0     1364 2023-03-31 18:06:51.072432 baseblock-0.2.22/PKG-INFO
+-rw-r--r--   0        0        0      509 2022-11-01 19:40:10.480205 baseblock-0.2.23/baseblock/__init__.py
+-rw-r--r--   0        0        0     1665 2023-03-31 18:06:04.643612 baseblock-0.2.23/baseblock/base_object.py
+-rw-r--r--   0        0        0     2206 2022-11-01 19:40:21.549334 baseblock-0.2.23/baseblock/common_utils.py
+-rw-r--r--   0        0        0     3400 2022-11-01 19:40:24.233178 baseblock-0.2.23/baseblock/crypto_base.py
+-rw-r--r--   0        0        0    17519 2023-05-16 05:48:05.464931 baseblock-0.2.23/baseblock/enforce_type.py
+-rw-r--r--   0        0        0     6749 2023-01-10 20:33:14.114247 baseblock-0.2.23/baseblock/env_io.py
+-rw-r--r--   0        0        0    25397 2023-02-07 00:55:29.559730 baseblock-0.2.23/baseblock/file_io.py
+-rw-r--r--   0        0        0     1918 2022-11-01 19:40:37.387998 baseblock-0.2.23/baseblock/service_event_generator.py
+-rw-r--r--   0        0        0     2320 2022-11-01 19:40:10.479705 baseblock-0.2.23/baseblock/stopwatch.py
+-rw-r--r--   0        0        0     5147 2023-01-27 20:32:24.092475 baseblock-0.2.23/baseblock/text_matcher.py
+-rw-r--r--   0        0        0    29945 2023-01-26 05:18:13.221964 baseblock-0.2.23/baseblock/text_utils.py
+-rw-r--r--   0        0        0     1364 2022-11-01 19:40:49.507564 baseblock-0.2.23/baseblock/time_helper.py
+-rw-r--r--   0        0        0     1344 2023-05-16 03:21:11.641161 baseblock-0.2.23/pyproject.toml
+-rw-r--r--   0        0        0      506 2022-10-20 17:03:08.598380 baseblock-0.2.23/README.md
+-rw-r--r--   0        0        0     1237 2023-05-16 05:49:06.863304 baseblock-0.2.23/setup.py
+-rw-r--r--   0        0        0     1364 2023-05-16 05:49:06.863804 baseblock-0.2.23/PKG-INFO
```

### Comparing `baseblock-0.2.22/baseblock/base_object.py` & `baseblock-0.2.23/baseblock/base_object.py`

 * *Files identical despite different names*

### Comparing `baseblock-0.2.22/baseblock/common_utils.py` & `baseblock-0.2.23/baseblock/common_utils.py`

 * *Files identical despite different names*

### Comparing `baseblock-0.2.22/baseblock/crypto_base.py` & `baseblock-0.2.23/baseblock/crypto_base.py`

 * *Files identical despite different names*

### Comparing `baseblock-0.2.22/baseblock/enforce_type.py` & `baseblock-0.2.23/baseblock/enforce_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -456,14 +456,29 @@
             return True
 
         if not _is_list_of_strings():
             raise DataTypeNotExpectedError(actual_value=value,
                                            expected_type='List[str]')
 
     @classmethod
+    def is_list_of_list_of_dicts(cls,
+                                 value: object) -> None:
+        """ This is a highly specialized data type checker
+
+        Args:
+            value (object): True if this is a list of dict elements
+        """
+
+        if type(value) != list:
+            raise DataTypeNotExpectedError(actual_value=value,
+                                           expected_type='List[List[Dict]]')
+
+        [Enforcer.is_list_of_dicts(x) for x in value]
+
+    @classmethod
     def is_list_of_tuples(cls,
                           value: object) -> None:
         """ This is a highly specialized data type checker
 
         Args:
             value (object): True if this is a list of tuple elements
         """
```

### Comparing `baseblock-0.2.22/baseblock/env_io.py` & `baseblock-0.2.23/baseblock/env_io.py`

 * *Files identical despite different names*

### Comparing `baseblock-0.2.22/baseblock/file_io.py` & `baseblock-0.2.23/baseblock/file_io.py`

 * *Files identical despite different names*

### Comparing `baseblock-0.2.22/baseblock/service_event_generator.py` & `baseblock-0.2.23/baseblock/service_event_generator.py`

 * *Files identical despite different names*

### Comparing `baseblock-0.2.22/baseblock/stopwatch.py` & `baseblock-0.2.23/baseblock/stopwatch.py`

 * *Files identical despite different names*

### Comparing `baseblock-0.2.22/baseblock/text_matcher.py` & `baseblock-0.2.23/baseblock/text_matcher.py`

 * *Files identical despite different names*

### Comparing `baseblock-0.2.22/baseblock/text_utils.py` & `baseblock-0.2.23/baseblock/text_utils.py`

 * *Files identical despite different names*

### Comparing `baseblock-0.2.22/baseblock/time_helper.py` & `baseblock-0.2.23/baseblock/time_helper.py`

 * *Files identical despite different names*

### Comparing `baseblock-0.2.22/pyproject.toml` & `baseblock-0.2.23/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   "Craig Trim <craigtrim@gmail.com>",
 ]
 
 description = "Base Block of Common Enterprise Python Utilities"
 license = "MIT"
 name = "baseblock"
 readme = "README.md"
-version = "0.2.22"
+version = "0.2.23"
 
 keywords = ["utility", "helper", "text", "matching"]
 repository = "https://github.com/craigtrim/climate-bot"
 
 classifiers = [
   "Development Status :: 4 - Beta",
   "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `baseblock-0.2.22/setup.py` & `baseblock-0.2.23/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['PyYAML==6.0', 'cryptography==38.0.1', 'unicodedata2']
 
 setup_kwargs = {
     'name': 'baseblock',
-    'version': '0.2.22',
+    'version': '0.2.23',
     'description': 'Base Block of Common Enterprise Python Utilities',
     'long_description': '# Base Block (baseblock)\n\nBase Block of Common Enterprise Python Utilities\n\n\n## Crypto Base\nUsage\n```python\nfrom baseblock import CryptoBase\n\nkey = CryptoBase.generate_private_key()\n```\n\nThe `key` is used to both encrypt and decrypt text, like this:\n```python\ninput_text = "Hello, World!"\n\ncrypt = CryptoBase(key)\n\nx = crypt.encrypt_str(input_text)\ny = crypt.decrypt_str(x)\n\nassert input_text == y\n```\n\nThe key can also be stored in the environment under **BASEBLOCK_CRYPTO_KEY**.\n',
     'author': 'Craig Trim',
     'author_email': 'craigtrim@gmail.com',
     'maintainer': 'Craig Trim',
     'maintainer_email': 'craigtrim@gmail.com',
     'url': 'https://github.com/craigtrim/climate-bot',
```

### Comparing `baseblock-0.2.22/PKG-INFO` & `baseblock-0.2.23/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baseblock
-Version: 0.2.22
+Version: 0.2.23
 Summary: Base Block of Common Enterprise Python Utilities
 Home-page: https://github.com/craigtrim/climate-bot
 License: MIT
 Keywords: utility,helper,text,matching
 Author: Craig Trim
 Author-email: craigtrim@gmail.com
 Maintainer: Craig Trim
```

