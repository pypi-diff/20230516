# Comparing `tmp/clean-notebook-0.1.8.tar.gz` & `tmp/clean-notebook-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clean-notebook-0.1.8.tar", last modified: Sun Mar 12 14:48:36 2023, max compression
+gzip compressed data, was "clean-notebook-0.1.9.tar", last modified: Tue Mar 14 08:18:26 2023, max compression
```

## Comparing `clean-notebook-0.1.8.tar` & `clean-notebook-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 14:48:36.115461 clean-notebook-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-03-12 14:48:36.115461 clean-notebook-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-03-12 14:48:18.000000 clean-notebook-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-03-12 14:48:18.000000 clean-notebook-0.1.8/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-12 14:48:36.115461 clean-notebook-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 14:48:36.115461 clean-notebook-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 14:48:36.115461 clean-notebook-0.1.8/src/clean_notebook/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-12 14:48:18.000000 clean-notebook-0.1.8/src/clean_notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-03-12 14:48:18.000000 clean-notebook-0.1.8/src/clean_notebook/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-03-12 14:48:18.000000 clean-notebook-0.1.8/src/clean_notebook/clean.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 14:48:36.115461 clean-notebook-0.1.8/src/clean_notebook.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-03-12 14:48:36.000000 clean-notebook-0.1.8/src/clean_notebook.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-03-12 14:48:36.000000 clean-notebook-0.1.8/src/clean_notebook.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-12 14:48:36.000000 clean-notebook-0.1.8/src/clean_notebook.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-12 14:48:36.000000 clean-notebook-0.1.8/src/clean_notebook.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-12 14:48:36.000000 clean-notebook-0.1.8/src/clean_notebook.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-12 14:48:36.000000 clean-notebook-0.1.8/src/clean_notebook.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 14:48:36.115461 clean-notebook-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-03-12 14:48:18.000000 clean-notebook-0.1.8/tests/test_clean_notebook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 08:18:26.445289 clean-notebook-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-03-14 08:18:26.445289 clean-notebook-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-03-14 08:18:06.000000 clean-notebook-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-03-14 08:18:06.000000 clean-notebook-0.1.9/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 08:18:26.445289 clean-notebook-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 08:18:26.441289 clean-notebook-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 08:18:26.445289 clean-notebook-0.1.9/src/clean_notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-14 08:18:06.000000 clean-notebook-0.1.9/src/clean_notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-03-14 08:18:06.000000 clean-notebook-0.1.9/src/clean_notebook/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-03-14 08:18:06.000000 clean-notebook-0.1.9/src/clean_notebook/clean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 08:18:26.445289 clean-notebook-0.1.9/src/clean_notebook.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-03-14 08:18:26.000000 clean-notebook-0.1.9/src/clean_notebook.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-03-14 08:18:26.000000 clean-notebook-0.1.9/src/clean_notebook.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 08:18:26.000000 clean-notebook-0.1.9/src/clean_notebook.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-14 08:18:26.000000 clean-notebook-0.1.9/src/clean_notebook.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-14 08:18:26.000000 clean-notebook-0.1.9/src/clean_notebook.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-14 08:18:26.000000 clean-notebook-0.1.9/src/clean_notebook.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 08:18:26.445289 clean-notebook-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-03-14 08:18:06.000000 clean-notebook-0.1.9/tests/test_clean_notebook.py
```

### Comparing `clean-notebook-0.1.8/PKG-INFO` & `clean-notebook-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clean-notebook
-Version: 0.1.8
+Version: 0.1.9
 Summary: A simple package to clean Jupyter notebooks
 Author: Simon Hansen
 Maintainer: Simon Hansen
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/hoxbro/clean_notebook
 Project-URL: Source, https://github.com/hoxbro/clean_notebook
 Keywords: clean,jupyter,notebook
```

### Comparing `clean-notebook-0.1.8/pyproject.toml` & `clean-notebook-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `clean-notebook-0.1.8/readme.md` & `clean-notebook-0.1.9/readme.md`

 * *Files identical despite different names*

### Comparing `clean-notebook-0.1.8/src/clean_notebook/__main__.py` & `clean-notebook-0.1.9/src/clean_notebook/__main__.py`

 * *Files identical despite different names*

### Comparing `clean-notebook-0.1.8/src/clean_notebook/clean.py` & `clean-notebook-0.1.9/src/clean_notebook/clean.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 def clean_notebook(
     paths: list[str | Path],
     *,
     dryrun: bool = False,
     keep_empty: bool = False,
     ignore: list[str] | None = None,
 ) -> None:
-    files = sorted(_get_files(paths))
-    for file in files:
+    for file in sorted(_get_files(paths)):
         clean_single_notebook(file, dryrun=dryrun, keep_empty=keep_empty, ignore=ignore)
 
 
 def find_line_ending(s: AnyStr) -> AnyStr:
     if isinstance(s, str):
         endings = ["\n", "\r", "\r\n"]
     elif isinstance(s, bytes):
@@ -42,16 +41,15 @@
     newline = find_line_ending(raw)
     nb = json.loads(raw)
 
     cleaned = False
     for cell in nb["cells"]:
         cleaned |= _update_value(cell, "outputs", [])
         cleaned |= _update_value(cell, "execution_count", None)
-        cell_metadata = _ignore(cell, ignore)
-        cleaned |= _update_value(cell, "metadata", cell_metadata)
+        cleaned |= _update_value(cell, "metadata", _ignore(cell, ignore))
         if not cell["source"] and not keep_empty:
             nb["cells"].remove(cell)
             cleaned = True
 
     if not nb["cells"]:
         print(f"Notebook '{file}' does not have any valid cells.")
         return True
@@ -80,14 +78,15 @@
 
 def _get_files(paths: list[str | Path]) -> Iterator[Path]:
     for path in map(Path, paths):
         if path.is_file() and path.suffix == ".ipynb":
             yield path
         if path.is_dir():
             for file in path.rglob("*.ipynb"):
-                yield file
+                if file.parent.name != ".ipynb_checkpoints":
+                    yield file
 
 
 def _ignore(cell: dict[str, Any], ignore: list[str] | None) -> dict[str, Any]:
     if "metadata" in cell and ignore:
         return {k: v for k, v in cell["metadata"].items() if k in ignore}
     return {}
```

### Comparing `clean-notebook-0.1.8/src/clean_notebook.egg-info/PKG-INFO` & `clean-notebook-0.1.9/src/clean_notebook.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clean-notebook
-Version: 0.1.8
+Version: 0.1.9
 Summary: A simple package to clean Jupyter notebooks
 Author: Simon Hansen
 Maintainer: Simon Hansen
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/hoxbro/clean_notebook
 Project-URL: Source, https://github.com/hoxbro/clean_notebook
 Keywords: clean,jupyter,notebook
```

### Comparing `clean-notebook-0.1.8/tests/test_clean_notebook.py` & `clean-notebook-0.1.9/tests/test_clean_notebook.py`

 * *Files identical despite different names*

