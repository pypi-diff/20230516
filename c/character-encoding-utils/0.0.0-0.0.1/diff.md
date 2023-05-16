# Comparing `tmp/character-encoding-utils-0.0.0.tar.gz` & `tmp/character-encoding-utils-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "character-encoding-utils-0.0.0.tar", last modified: Wed May 10 07:08:14 2023, max compression
+gzip compressed data, was "character-encoding-utils-0.0.1.tar", last modified: Tue May 16 05:06:23 2023, max compression
```

## Comparing `character-encoding-utils-0.0.0.tar` & `character-encoding-utils-0.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:08:14.217747 character-encoding-utils-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-10 07:07:52.000000 character-encoding-utils-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-10 07:08:14.217747 character-encoding-utils-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-10 07:07:52.000000 character-encoding-utils-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-10 07:07:52.000000 character-encoding-utils-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 07:08:14.217747 character-encoding-utils-0.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:08:14.213747 character-encoding-utils-0.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:08:14.217747 character-encoding-utils-0.0.0/src/character_encoding_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 07:07:52.000000 character-encoding-utils-0.0.0/src/character_encoding_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 07:07:52.000000 character-encoding-utils-0.0.0/src/character_encoding_utils/big5.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 07:07:52.000000 character-encoding-utils-0.0.0/src/character_encoding_utils/gb2312.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 07:07:52.000000 character-encoding-utils-0.0.0/src/character_encoding_utils/ksx1001.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 07:07:52.000000 character-encoding-utils-0.0.0/src/character_encoding_utils/shiftjis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:08:14.217747 character-encoding-utils-0.0.0/src/character_encoding_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-10 07:08:14.000000 character-encoding-utils-0.0.0/src/character_encoding_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-10 07:08:14.000000 character-encoding-utils-0.0.0/src/character_encoding_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 07:08:14.000000 character-encoding-utils-0.0.0/src/character_encoding_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-10 07:08:14.000000 character-encoding-utils-0.0.0/src/character_encoding_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:08:14.217747 character-encoding-utils-0.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-10 07:07:52.000000 character-encoding-utils-0.0.0/tests/test_big5.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-10 07:07:52.000000 character-encoding-utils-0.0.0/tests/test_gb2312.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-10 07:07:52.000000 character-encoding-utils-0.0.0/tests/test_ksx1001.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-10 07:07:52.000000 character-encoding-utils-0.0.0/tests/test_shiftjis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:06:23.670114 character-encoding-utils-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-16 05:06:04.000000 character-encoding-utils-0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-16 05:06:23.670114 character-encoding-utils-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-16 05:06:04.000000 character-encoding-utils-0.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-16 05:06:04.000000 character-encoding-utils-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 05:06:23.670114 character-encoding-utils-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:06:23.662114 character-encoding-utils-0.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:06:23.666113 character-encoding-utils-0.0.1/src/character_encoding_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 05:06:04.000000 character-encoding-utils-0.0.1/src/character_encoding_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-05-16 05:06:04.000000 character-encoding-utils-0.0.1/src/character_encoding_utils/big5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-05-16 05:06:04.000000 character-encoding-utils-0.0.1/src/character_encoding_utils/gb2312.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-05-16 05:06:04.000000 character-encoding-utils-0.0.1/src/character_encoding_utils/ksx1001.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-05-16 05:06:04.000000 character-encoding-utils-0.0.1/src/character_encoding_utils/shiftjis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:06:23.670114 character-encoding-utils-0.0.1/src/character_encoding_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-16 05:06:23.000000 character-encoding-utils-0.0.1/src/character_encoding_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-16 05:06:23.000000 character-encoding-utils-0.0.1/src/character_encoding_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 05:06:23.000000 character-encoding-utils-0.0.1/src/character_encoding_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-16 05:06:23.000000 character-encoding-utils-0.0.1/src/character_encoding_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:06:23.670114 character-encoding-utils-0.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-16 05:06:04.000000 character-encoding-utils-0.0.1/tests/test_big5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-05-16 05:06:04.000000 character-encoding-utils-0.0.1/tests/test_gb2312.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-05-16 05:06:04.000000 character-encoding-utils-0.0.1/tests/test_ksx1001.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-05-16 05:06:04.000000 character-encoding-utils-0.0.1/tests/test_shiftjis.py
```

### Comparing `character-encoding-utils-0.0.0/LICENSE` & `character-encoding-utils-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `character-encoding-utils-0.0.0/PKG-INFO` & `character-encoding-utils-0.0.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: character-encoding-utils
-Version: 0.0.0
+Version: 0.0.1
 Summary: Some character encoding utils.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/character-encoding-utils
 Project-URL: source, https://github.com/TakWolf/character-encoding-utils
 Project-URL: issues, https://github.com/TakWolf/character-encoding-utils/issues
@@ -20,25 +20,59 @@
 
 [![PyPI](https://img.shields.io/pypi/v/character-encoding-utils)](https://pypi.org/project/character-encoding-utils/)
 
 Some [character encoding](https://en.wikipedia.org/wiki/Character_encoding) utils.
 
 Now support:
 
-- [GB 2312](https://en.wikipedia.org/wiki/GB_2312)
+- [GB2312](https://en.wikipedia.org/wiki/GB_2312)
 - [Big5](https://en.wikipedia.org/wiki/Big5)
-- [Shift JIS](https://en.wikipedia.org/wiki/Shift_JIS)
-- [KS X 1001](https://en.wikipedia.org/wiki/KS_X_1001)
+- [Shift-JIS](https://en.wikipedia.org/wiki/Shift_JIS)
+- [KS-X-1001](https://en.wikipedia.org/wiki/KS_X_1001)
 
 ## Installation
 
 ```commandline
 pip install character-encoding-utils
 ```
 
 ## Usage
 
-TODO
+### GB2312
+
+```python
+from character_encoding_utils import gb2312
+
+bs = gb2312.encode('abc中国')
+assert gb2312.decode(bs) == 'abc中国'
+```
+
+### Big5
+
+```python
+from character_encoding_utils import big5
+
+bs = big5.encode('abc中國')
+assert big5.decode(bs) == 'abc中國'
+```
+
+### Shift-JIS
+
+```python
+from character_encoding_utils import shiftjis
+
+bs =  shiftjis.encode('abc日本')
+assert shiftjis.decode(bs) == 'abc日本'
+```
+
+### KS-X-1001
+
+```python
+from character_encoding_utils import ksx1001
+
+bs = ksx1001.encode('abc가쳰')
+assert ksx1001.decode(bs) == 'abc가쳰'
+```
 
 ## License
 
 Under the [MIT license](LICENSE).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `character-encoding-utils-0.0.0/pyproject.toml` & `character-encoding-utils-0.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "character-encoding-utils"
-version = "0.0.0"
+version = "0.0.1"
 description = "Some character encoding utils."
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.10"
 authors = [
     { name = "TakWolf" },
 ]
```

### Comparing `character-encoding-utils-0.0.0/src/character_encoding_utils.egg-info/PKG-INFO` & `character-encoding-utils-0.0.1/src/character_encoding_utils.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: character-encoding-utils
-Version: 0.0.0
+Version: 0.0.1
 Summary: Some character encoding utils.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/character-encoding-utils
 Project-URL: source, https://github.com/TakWolf/character-encoding-utils
 Project-URL: issues, https://github.com/TakWolf/character-encoding-utils/issues
@@ -20,25 +20,59 @@
 
 [![PyPI](https://img.shields.io/pypi/v/character-encoding-utils)](https://pypi.org/project/character-encoding-utils/)
 
 Some [character encoding](https://en.wikipedia.org/wiki/Character_encoding) utils.
 
 Now support:
 
-- [GB 2312](https://en.wikipedia.org/wiki/GB_2312)
+- [GB2312](https://en.wikipedia.org/wiki/GB_2312)
 - [Big5](https://en.wikipedia.org/wiki/Big5)
-- [Shift JIS](https://en.wikipedia.org/wiki/Shift_JIS)
-- [KS X 1001](https://en.wikipedia.org/wiki/KS_X_1001)
+- [Shift-JIS](https://en.wikipedia.org/wiki/Shift_JIS)
+- [KS-X-1001](https://en.wikipedia.org/wiki/KS_X_1001)
 
 ## Installation
 
 ```commandline
 pip install character-encoding-utils
 ```
 
 ## Usage
 
-TODO
+### GB2312
+
+```python
+from character_encoding_utils import gb2312
+
+bs = gb2312.encode('abc中国')
+assert gb2312.decode(bs) == 'abc中国'
+```
+
+### Big5
+
+```python
+from character_encoding_utils import big5
+
+bs = big5.encode('abc中國')
+assert big5.decode(bs) == 'abc中國'
+```
+
+### Shift-JIS
+
+```python
+from character_encoding_utils import shiftjis
+
+bs =  shiftjis.encode('abc日本')
+assert shiftjis.decode(bs) == 'abc日本'
+```
+
+### KS-X-1001
+
+```python
+from character_encoding_utils import ksx1001
+
+bs = ksx1001.encode('abc가쳰')
+assert ksx1001.decode(bs) == 'abc가쳰'
+```
 
 ## License
 
 Under the [MIT license](LICENSE).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `character-encoding-utils-0.0.0/src/character_encoding_utils.egg-info/SOURCES.txt` & `character-encoding-utils-0.0.1/src/character_encoding_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

