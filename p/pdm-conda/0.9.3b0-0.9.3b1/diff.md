# Comparing `tmp/pdm_conda-0.9.3b0.tar.gz` & `tmp/pdm_conda-0.9.3b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm_conda-0.9.3b0.tar", last modified: Wed Apr 26 21:30:37 2023, max compression
+gzip compressed data, was "pdm_conda-0.9.3b1.tar", last modified: Wed Apr 26 21:47:52 2023, max compression
```

## Comparing `pdm_conda-0.9.3b0.tar` & `pdm_conda-0.9.3b1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1065 2022-12-16 23:52:20.043514 pdm_conda-0.9.3b0/LICENSE
--rw-r--r--   0        0        0     5701 2023-04-26 21:23:52.333777 pdm_conda-0.9.3b0/README.md
--rw-r--r--   0        0        0      110 2023-04-26 21:12:13.255162 pdm_conda-0.9.3b0/data/mapping_fixes.json
--rw-r--r--   0        0        0     1998 2023-04-26 21:30:37.087628 pdm_conda-0.9.3b0/pyproject.toml
--rw-r--r--   0        0        0      595 2023-04-26 21:30:00.405870 pdm_conda-0.9.3b0/src/pdm_conda/__init__.py
--rw-r--r--   0        0        0        0 2023-01-06 20:52:28.238706 pdm_conda-0.9.3b0/src/pdm_conda/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-01-06 20:52:59.837399 pdm_conda-0.9.3b0/src/pdm_conda/cli/commands/__init__.py
--rw-r--r--   0        0        0     3087 2023-04-19 19:04:02.150645 pdm_conda-0.9.3b0/src/pdm_conda/cli/commands/add.py
--rw-r--r--   0        0        0     1681 2023-04-19 16:32:57.025189 pdm_conda-0.9.3b0/src/pdm_conda/cli/commands/remove.py
--rw-r--r--   0        0        0     3009 2023-04-21 15:54:37.429042 pdm_conda-0.9.3b0/src/pdm_conda/cli/utils.py
--rw-r--r--   0        0        0    15836 2023-04-26 21:23:23.198612 pdm_conda-0.9.3b0/src/pdm_conda/conda.py
--rw-r--r--   0        0        0        0 2023-01-05 20:40:25.652497 pdm_conda-0.9.3b0/src/pdm_conda/installers/__init__.py
--rw-r--r--   0        0        0     2444 2023-04-26 21:20:39.055538 pdm_conda-0.9.3b0/src/pdm_conda/installers/manager.py
--rw-r--r--   0        0        0     2304 2023-04-26 21:18:03.786553 pdm_conda-0.9.3b0/src/pdm_conda/installers/synchronizers.py
--rw-r--r--   0        0        0     3343 2023-04-26 21:12:20.058679 pdm_conda-0.9.3b0/src/pdm_conda/mapping.py
--rw-r--r--   0        0        0        0 2023-01-02 22:45:44.891129 pdm_conda-0.9.3b0/src/pdm_conda/models/__init__.py
--rw-r--r--   0        0        0        0 2023-03-30 01:53:52.844040 pdm_conda-0.9.3b0/src/pdm_conda/models/__pycache__/candidates.cpython-310.pyc.281473776611248
--rw-r--r--   0        0        0     7575 2023-04-21 15:54:37.432253 pdm_conda-0.9.3b0/src/pdm_conda/models/candidates.py
--rw-r--r--   0        0        0     1818 2023-04-19 19:04:02.154757 pdm_conda-0.9.3b0/src/pdm_conda/models/conda.py
--rw-r--r--   0        0        0     8846 2023-04-26 21:15:12.881202 pdm_conda-0.9.3b0/src/pdm_conda/models/config.py
--rw-r--r--   0        0        0     3795 2023-04-26 21:19:38.356166 pdm_conda-0.9.3b0/src/pdm_conda/models/environment.py
--rw-r--r--   0        0        0     6740 2023-04-21 15:54:37.432966 pdm_conda-0.9.3b0/src/pdm_conda/models/repositories.py
--rw-r--r--   0        0        0    11368 2023-04-21 15:54:37.434138 pdm_conda-0.9.3b0/src/pdm_conda/models/requirements.py
--rw-r--r--   0        0        0     1123 2023-04-26 21:17:17.574104 pdm_conda-0.9.3b0/src/pdm_conda/models/setup.py
--rw-r--r--   0        0        0     8311 2023-04-19 19:04:02.158361 pdm_conda-0.9.3b0/src/pdm_conda/project.py
--rw-r--r--   0        0        0        0 2023-02-18 20:09:32.663574 pdm_conda-0.9.3b0/src/pdm_conda/resolver/__init__.py
--rw-r--r--   0        0        0     2418 2023-04-19 19:04:02.159092 pdm_conda-0.9.3b0/src/pdm_conda/resolver/providers.py
--rw-r--r--   0        0        0     8601 2023-04-19 19:04:02.159990 pdm_conda-0.9.3b0/src/pdm_conda/resolvers.py
--rw-r--r--   0        0        0      784 2023-01-10 16:37:32.674613 pdm_conda-0.9.3b0/src/pdm_conda/utils.py
--rw-r--r--   0        0        0     7549 1970-01-01 00:00:00.000000 pdm_conda-0.9.3b0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-12-16 23:52:20.043514 pdm_conda-0.9.3b1/LICENSE
+-rw-r--r--   0        0        0     5701 2023-04-26 21:23:52.333777 pdm_conda-0.9.3b1/README.md
+-rw-r--r--   0        0        0      110 2023-04-26 21:12:13.255162 pdm_conda-0.9.3b1/data/mapping_fixes.json
+-rw-r--r--   0        0        0     1998 2023-04-26 21:47:52.038888 pdm_conda-0.9.3b1/pyproject.toml
+-rw-r--r--   0        0        0      595 2023-04-26 21:47:36.532789 pdm_conda-0.9.3b1/src/pdm_conda/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-06 20:52:28.238706 pdm_conda-0.9.3b1/src/pdm_conda/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-06 20:52:59.837399 pdm_conda-0.9.3b1/src/pdm_conda/cli/commands/__init__.py
+-rw-r--r--   0        0        0     3087 2023-04-19 19:04:02.150645 pdm_conda-0.9.3b1/src/pdm_conda/cli/commands/add.py
+-rw-r--r--   0        0        0     1681 2023-04-19 16:32:57.025189 pdm_conda-0.9.3b1/src/pdm_conda/cli/commands/remove.py
+-rw-r--r--   0        0        0     3009 2023-04-21 15:54:37.429042 pdm_conda-0.9.3b1/src/pdm_conda/cli/utils.py
+-rw-r--r--   0        0        0    15836 2023-04-26 21:23:23.198612 pdm_conda-0.9.3b1/src/pdm_conda/conda.py
+-rw-r--r--   0        0        0        0 2023-01-05 20:40:25.652497 pdm_conda-0.9.3b1/src/pdm_conda/installers/__init__.py
+-rw-r--r--   0        0        0     2444 2023-04-26 21:20:39.055538 pdm_conda-0.9.3b1/src/pdm_conda/installers/manager.py
+-rw-r--r--   0        0        0     2304 2023-04-26 21:18:03.786553 pdm_conda-0.9.3b1/src/pdm_conda/installers/synchronizers.py
+-rw-r--r--   0        0        0     3420 2023-04-26 21:46:06.831344 pdm_conda-0.9.3b1/src/pdm_conda/mapping.py
+-rw-r--r--   0        0        0        0 2023-01-02 22:45:44.891129 pdm_conda-0.9.3b1/src/pdm_conda/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-30 01:53:52.844040 pdm_conda-0.9.3b1/src/pdm_conda/models/__pycache__/candidates.cpython-310.pyc.281473776611248
+-rw-r--r--   0        0        0     7575 2023-04-21 15:54:37.432253 pdm_conda-0.9.3b1/src/pdm_conda/models/candidates.py
+-rw-r--r--   0        0        0     1818 2023-04-19 19:04:02.154757 pdm_conda-0.9.3b1/src/pdm_conda/models/conda.py
+-rw-r--r--   0        0        0     8846 2023-04-26 21:15:12.881202 pdm_conda-0.9.3b1/src/pdm_conda/models/config.py
+-rw-r--r--   0        0        0     3795 2023-04-26 21:19:38.356166 pdm_conda-0.9.3b1/src/pdm_conda/models/environment.py
+-rw-r--r--   0        0        0     6740 2023-04-21 15:54:37.432966 pdm_conda-0.9.3b1/src/pdm_conda/models/repositories.py
+-rw-r--r--   0        0        0    11368 2023-04-21 15:54:37.434138 pdm_conda-0.9.3b1/src/pdm_conda/models/requirements.py
+-rw-r--r--   0        0        0     1123 2023-04-26 21:17:17.574104 pdm_conda-0.9.3b1/src/pdm_conda/models/setup.py
+-rw-r--r--   0        0        0     8311 2023-04-19 19:04:02.158361 pdm_conda-0.9.3b1/src/pdm_conda/project.py
+-rw-r--r--   0        0        0        0 2023-02-18 20:09:32.663574 pdm_conda-0.9.3b1/src/pdm_conda/resolver/__init__.py
+-rw-r--r--   0        0        0     2418 2023-04-19 19:04:02.159092 pdm_conda-0.9.3b1/src/pdm_conda/resolver/providers.py
+-rw-r--r--   0        0        0     8601 2023-04-19 19:04:02.159990 pdm_conda-0.9.3b1/src/pdm_conda/resolvers.py
+-rw-r--r--   0        0        0      784 2023-01-10 16:37:32.674613 pdm_conda-0.9.3b1/src/pdm_conda/utils.py
+-rw-r--r--   0        0        0     7549 1970-01-01 00:00:00.000000 pdm_conda-0.9.3b1/PKG-INFO
```

### Comparing `pdm_conda-0.9.3b0/LICENSE` & `pdm_conda-0.9.3b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.3b0/README.md` & `pdm_conda-0.9.3b1/README.md`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.3b0/pyproject.toml` & `pdm_conda-0.9.3b1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3 :: Only",
 ]
 dependencies = [
     "pdm~=2.4.0",
     "requests>=2.28.1",
 ]
-version = "0.9.3b0"
+version = "0.9.3b1"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Homepage = "https://github.com/macro128/pdm-conda"
 Changelog = "https://github.com/macro128/pdm-conda/blob/main/CHANGELOG.md"
```

### Comparing `pdm_conda-0.9.3b0/src/pdm_conda/__init__.py` & `pdm_conda-0.9.3b1/src/pdm_conda/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
     core.register_command(AddCommand)
     core.register_command(RemoveCommand)
 
     for name, config in CONFIGS:
         core.add_config(name, config)
 
 
-__version__ = "0.9.3b0"
+__version__ = "0.9.3b1"
```

### Comparing `pdm_conda-0.9.3b0/src/pdm_conda/cli/commands/add.py` & `pdm_conda-0.9.3b1/src/pdm_conda/cli/commands/add.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.3b0/src/pdm_conda/cli/commands/remove.py` & `pdm_conda-0.9.3b1/src/pdm_conda/cli/commands/remove.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.3b0/src/pdm_conda/cli/utils.py` & `pdm_conda-0.9.3b1/src/pdm_conda/cli/utils.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.3b0/src/pdm_conda/conda.py` & `pdm_conda-0.9.3b1/src/pdm_conda/conda.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.3b0/src/pdm_conda/installers/manager.py` & `pdm_conda-0.9.3b1/src/pdm_conda/installers/manager.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.3b0/src/pdm_conda/installers/synchronizers.py` & `pdm_conda-0.9.3b1/src/pdm_conda/installers/synchronizers.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.3b0/src/pdm_conda/mapping.py` & `pdm_conda-0.9.3b1/src/pdm_conda/mapping.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,17 +57,20 @@
 
     with dict_path.open() as f:
         return json.load(f)
 
 
 def get_mapping_fixes() -> dict:
     fixes = dict()
-    if (fixes_file := Path(__file__).parents[2] / "data/mapping_fixes.json").exists():
-        with fixes_file.open() as f:
-            fixes = json.load(f)
+    for path in Path(__file__).parents[:3]:
+        print(path)
+        if (fixes_file := path / "data/mapping_fixes.json").exists():
+            with fixes_file.open() as f:
+                fixes = json.load(f)
+                break
     return fixes
 
 
 @lru_cache
 def get_pypi_mapping() -> dict[str, str]:
     download_dir = os.getenv(DOWNLOAD_DIR_ENV_VAR)
     mapping = download_mapping(Path(str(download_dir)))
```

### Comparing `pdm_conda-0.9.3b0/src/pdm_conda/models/candidates.py` & `pdm_conda-0.9.3b1/src/pdm_conda/models/candidates.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.3b0/src/pdm_conda/models/conda.py` & `pdm_conda-0.9.3b1/src/pdm_conda/models/conda.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.3b0/src/pdm_conda/models/config.py` & `pdm_conda-0.9.3b1/src/pdm_conda/models/config.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.3b0/src/pdm_conda/models/environment.py` & `pdm_conda-0.9.3b1/src/pdm_conda/models/environment.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.3b0/src/pdm_conda/models/repositories.py` & `pdm_conda-0.9.3b1/src/pdm_conda/models/repositories.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.3b0/src/pdm_conda/models/requirements.py` & `pdm_conda-0.9.3b1/src/pdm_conda/models/requirements.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.3b0/src/pdm_conda/models/setup.py` & `pdm_conda-0.9.3b1/src/pdm_conda/models/setup.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.3b0/src/pdm_conda/project.py` & `pdm_conda-0.9.3b1/src/pdm_conda/project.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.3b0/src/pdm_conda/resolver/providers.py` & `pdm_conda-0.9.3b1/src/pdm_conda/resolver/providers.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.3b0/src/pdm_conda/resolvers.py` & `pdm_conda-0.9.3b1/src/pdm_conda/resolvers.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.3b0/src/pdm_conda/utils.py` & `pdm_conda-0.9.3b1/src/pdm_conda/utils.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.3b0/PKG-INFO` & `pdm_conda-0.9.3b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm-conda
-Version: 0.9.3b0
+Version: 0.9.3b1
 Summary: A PDM plugin to resolve/install/uninstall project dependencies with Conda
 Keywords: pdm plugin conda
 Author: Marcos Pastorini
 License: MIT License
         
         Copyright (c) 2022 macro128
```

