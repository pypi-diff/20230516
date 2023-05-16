# Comparing `tmp/polario-0.2.2.tar.gz` & `tmp/polario-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polario-0.2.2.tar", max compression
+gzip compressed data, was "polario-0.2.3.tar", max compression
```

## Comparing `polario-0.2.2.tar` & `polario-0.2.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-04-23 17:52:08.816507 polario-0.2.2/LICENSE
--rw-r--r--   0        0        0      694 2023-04-23 17:52:08.816507 polario-0.2.2/README.md
--rw-r--r--   0        0        0      106 2023-04-23 17:52:08.816507 polario-0.2.2/polario/__init__.py
--rw-r--r--   0        0        0    11443 2023-04-23 17:52:08.816507 polario-0.2.2/polario/dataset.py
--rw-r--r--   0        0        0     1644 2023-04-23 17:52:08.816507 polario-0.2.2/polario/main.py
--rw-r--r--   0        0        0        0 2023-04-23 17:52:08.816507 polario-0.2.2/polario/py.typed
--rw-r--r--   0        0        0      997 2023-04-23 17:52:29.460622 polario-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1507 1970-01-01 00:00:00.000000 polario-0.2.2/setup.py
--rw-r--r--   0        0        0     1440 1970-01-01 00:00:00.000000 polario-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-16 08:52:06.081131 polario-0.2.3/LICENSE
+-rw-r--r--   0        0        0      694 2023-05-16 08:52:06.081131 polario-0.2.3/README.md
+-rw-r--r--   0        0        0      106 2023-05-16 08:52:06.081131 polario-0.2.3/polario/__init__.py
+-rw-r--r--   0        0        0    11498 2023-05-16 08:52:06.085131 polario-0.2.3/polario/dataset.py
+-rw-r--r--   0        0        0     1644 2023-05-16 08:52:06.085131 polario-0.2.3/polario/main.py
+-rw-r--r--   0        0        0        0 2023-05-16 08:52:06.085131 polario-0.2.3/polario/py.typed
+-rw-r--r--   0        0        0      999 2023-05-16 08:52:33.645241 polario-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1489 1970-01-01 00:00:00.000000 polario-0.2.3/setup.py
+-rw-r--r--   0        0        0     1424 1970-01-01 00:00:00.000000 polario-0.2.3/PKG-INFO
```

### Comparing `polario-0.2.2/LICENSE` & `polario-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `polario-0.2.2/README.md` & `polario-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `polario-0.2.2/polario/dataset.py` & `polario-0.2.3/polario/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """The main dataset package"""
 from enum import Enum
 from functools import reduce
-from typing import Iterable, Optional, Sequence
+from typing import Iterable, Literal, Optional, Sequence
 from urllib.parse import urlsplit, urlunsplit
 from uuid import uuid4
 
 import fsspec
 import polars as pl
 import pyarrow as pa
 import pyarrow.dataset
@@ -213,15 +213,18 @@
         ]
         if wrong_columns:
             raise ValueError(
                 f"Partition columns must be of type string for dataset. Wrong columns are {wrong_columns}"
             )
 
     def update(
-        self, other_df: pl.DataFrame, on: Sequence[str], how: str = "left"
+        self,
+        other_df: pl.DataFrame,
+        on: Sequence[str],
+        how: Literal["left", "inner"] = "left",
     ) -> None:
         """Upsert the given dataframe into the dataset.
 
         This will partition the dataframe and for each partition, load the partition, merge
         the dataframe and write back to the dataset.
 
         Args:
```

### Comparing `polario-0.2.2/polario/main.py` & `polario-0.2.3/polario/main.py`

 * *Files identical despite different names*

### Comparing `polario-0.2.2/pyproject.toml` & `polario-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "polario"
-version = "0.2.2"
+version = "0.2.3"
 description = "Polars IO"
 authors = ["Bram Neijt <bram@neijt.nl>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://bneijt.github.io/polario/"
 repository = "https://github.com/bneijt/polario"
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-polars = "^0.16.8"
+polars = ">=0.16.8"
 fsspec = "^2023.1.0"
-pyarrow = "^11.0.0"
+pyarrow = ">=11.0.0"
 
 
 [tool.poetry.group.dev.dependencies]
 black = { version = "^23.1.0", allow-prereleases = true }
 mypy = "^1.0.1"
 pytest = "^7.2.1"
 pdoc = "^13.0.0"
```

### Comparing `polario-0.2.2/setup.py` & `polario-0.2.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,24 +4,22 @@
 packages = \
 ['polario']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['fsspec>=2023.1.0,<2024.0.0',
- 'polars>=0.16.8,<0.17.0',
- 'pyarrow>=11.0.0,<12.0.0']
+['fsspec>=2023.1.0,<2024.0.0', 'polars>=0.16.8', 'pyarrow>=11.0.0']
 
 entry_points = \
 {'console_scripts': ['polario = polario.main:main']}
 
 setup_kwargs = {
     'name': 'polario',
-    'version': '0.2.2',
+    'version': '0.2.3',
     'description': 'Polars IO',
     'long_description': 'Polars IO utility library\n=================\n\nHelpers to make it easier to read and write Hive partitioned parquet dataset with Polars.\n\nIt is meant to be a library to deal with datasets easily, but also contains a commandline interface\nwhich allows you to inspect parquet files and datasets more easily.\n\nDataset\n=======\nExample of use of `polario.dataset.HiveDataset`\n```python\n\nfrom polario.dataset import HiveDataset\nimport polars as pl\ndf = pl.from_dicts(\n        [\n            {"p1": 1, "v": 1},\n            {"p1": 2, "v": 1},\n        ]\n    )\n\nds = HiveDataset("file:///tmp/", partition_columns=["p1"])\n\nds.write(df)\n\nfor partition_df in ds.read_partitions():\n    print(partition_df)\n\n```\n',
     'author': 'Bram Neijt',
     'author_email': 'bram@neijt.nl',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://bneijt.github.io/polario/',
```

### Comparing `polario-0.2.2/PKG-INFO` & `polario-0.2.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: polario
-Version: 0.2.2
+Version: 0.2.3
 Summary: Polars IO
 Home-page: https://bneijt.github.io/polario/
 License: Apache-2.0
 Author: Bram Neijt
 Author-email: bram@neijt.nl
 Requires-Python: >=3.9,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fsspec (>=2023.1.0,<2024.0.0)
-Requires-Dist: polars (>=0.16.8,<0.17.0)
-Requires-Dist: pyarrow (>=11.0.0,<12.0.0)
+Requires-Dist: polars (>=0.16.8)
+Requires-Dist: pyarrow (>=11.0.0)
 Project-URL: Repository, https://github.com/bneijt/polario
 Description-Content-Type: text/markdown
 
 Polars IO utility library
 =================
 
 Helpers to make it easier to read and write Hive partitioned parquet dataset with Polars.
```

