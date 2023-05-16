# Comparing `tmp/coordinate-projector-0.0.7.tar.gz` & `tmp/coordinate_projector-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coordinate-projector-0.0.7.tar", max compression
+gzip compressed data, was "coordinate_projector-0.0.8.tar", max compression
```

## Comparing `coordinate-projector-0.0.7.tar` & `coordinate_projector-0.0.8.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1084 2023-03-14 09:43:44.118018 coordinate-projector-0.0.7/LICENSE
--rw-r--r--   0        0        0     1687 2023-03-14 09:43:44.118018 coordinate-projector-0.0.7/README.md
--rw-r--r--   0        0        0     1246 2023-03-14 09:43:44.118018 coordinate-projector-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      217 2023-03-14 09:43:44.118018 coordinate-projector-0.0.7/src/coordinate_projector/__init__.py
--rw-r--r--   0        0        0     2615 2023-03-14 09:43:44.118018 coordinate-projector-0.0.7/src/coordinate_projector/datetime_parser.py
--rw-r--r--   0        0        0    11664 2023-03-14 09:43:44.118018 coordinate-projector-0.0.7/src/coordinate_projector/projections.json
--rw-r--r--   0        0        0      288 2023-03-14 09:43:44.118018 coordinate-projector-0.0.7/src/coordinate_projector/projections.py
--rw-r--r--   0        0        0     1404 2023-03-14 09:43:44.118018 coordinate-projector-0.0.7/src/coordinate_projector/projector.py
--rw-r--r--   0        0        0        0 2023-03-14 09:43:44.118018 coordinate-projector-0.0.7/src/coordinate_projector/py.typed
--rw-r--r--   0        0        0     2586 2023-03-14 09:43:56.264996 coordinate-projector-0.0.7/setup.py
--rw-r--r--   0        0        0     2611 2023-03-14 09:43:56.265372 coordinate-projector-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-05-16 08:39:53.489438 coordinate_projector-0.0.8/LICENSE
+-rw-r--r--   0        0        0     1687 2023-05-16 08:39:53.489438 coordinate_projector-0.0.8/README.md
+-rw-r--r--   0        0        0     1239 2023-05-16 08:39:53.489438 coordinate_projector-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      217 2023-05-16 08:39:53.489438 coordinate_projector-0.0.8/src/coordinate_projector/__init__.py
+-rw-r--r--   0        0        0     2615 2023-05-16 08:39:53.489438 coordinate_projector-0.0.8/src/coordinate_projector/datetime_parser.py
+-rw-r--r--   0        0        0    11664 2023-05-16 08:39:53.489438 coordinate_projector-0.0.8/src/coordinate_projector/projections.json
+-rw-r--r--   0        0        0      288 2023-05-16 08:39:53.489438 coordinate_projector-0.0.8/src/coordinate_projector/projections.py
+-rw-r--r--   0        0        0     1403 2023-05-16 08:39:53.489438 coordinate_projector-0.0.8/src/coordinate_projector/projector.py
+-rw-r--r--   0        0        0        0 2023-05-16 08:39:53.489438 coordinate_projector-0.0.8/src/coordinate_projector/py.typed
+-rw-r--r--   0        0        0     2708 1970-01-01 00:00:00.000000 coordinate_projector-0.0.8/PKG-INFO
```

### Comparing `coordinate-projector-0.0.7/LICENSE` & `coordinate_projector-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `coordinate-projector-0.0.7/README.md` & `coordinate_projector-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `coordinate-projector-0.0.7/pyproject.toml` & `coordinate_projector-0.0.8/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   | build
   | dist
 )/
 '''
 
 [tool.poetry]
 name = "coordinate-projector"
-version = "0.0.7"
+version = "0.0.8"
 description = "Project points from one projection to another using pyproj"
 license = "MIT"
 authors = ["Helge Smebye", "Jostein Leira <jostein@leira.net>"]
 maintainers = ["Jostein Leira <jostein@leira.net>"]
 readme = "README.md"
 homepage = "https://github.com/norwegian-geotechnical-institute/coordinate-projector"
 repository = "https://github.com/norwegian-geotechnical-institute/coordinate-projector"
@@ -31,26 +31,26 @@
 ]
 packages = [
     { include = "coordinate_projector", from="src" },
 ]
 
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.11"
-pyproj = "^3.3.0"
+python = ">=3.9,<4"
+pyproj = "^3.5.0"
 python-dateutil = "^2.8.2"
-types-python-dateutil = "^2.8.9"
+types-python-dateutil = "^2.8.19"
 timezonefinder = "*"
 
 
 [tool.poetry.dev-dependencies]
 black = "*"
 pytest = "*"
 pytest-cov = "*"
 mypy = "*"
 bandit = "*"
 safety = "*"
-pip-licenses = "^3.5.4"
+pip-licenses = "*"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `coordinate-projector-0.0.7/src/coordinate_projector/datetime_parser.py` & `coordinate_projector-0.0.8/src/coordinate_projector/datetime_parser.py`

 * *Files identical despite different names*

### Comparing `coordinate-projector-0.0.7/src/coordinate_projector/projections.json` & `coordinate_projector-0.0.8/src/coordinate_projector/projections.json`

 * *Files identical despite different names*

### Comparing `coordinate-projector-0.0.7/src/coordinate_projector/projector.py` & `coordinate_projector-0.0.8/src/coordinate_projector/projector.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 class Projector:
     @staticmethod
     def get_supported_projections() -> Dict:
         return projections
 
     @staticmethod
     def _get_transformer(from_srid: int, to_srid: int) -> Transformer:
-
         global _transformers
 
         if transformer := _transformers.get(f"{from_srid}-{to_srid}"):
             return transformer
 
         from_def_desc: Optional[Dict] = projections.get(str(from_srid))
         if not from_def_desc:
```

### Comparing `coordinate-projector-0.0.7/setup.py` & `coordinate_projector-0.0.8/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,109 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: coordinate-projector
+Version: 0.0.8
+Summary: Project points from one projection to another using pyproj
+Home-page: https://github.com/norwegian-geotechnical-institute/coordinate-projector
+License: MIT
+Author: Helge Smebye
+Maintainer: Jostein Leira
+Maintainer-email: jostein@leira.net
+Requires-Python: >=3.9,<4
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering :: GIS
+Requires-Dist: pyproj (>=3.5.0,<4.0.0)
+Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
+Requires-Dist: timezonefinder
+Requires-Dist: types-python-dateutil (>=2.8.19,<3.0.0)
+Project-URL: Repository, https://github.com/norwegian-geotechnical-institute/coordinate-projector
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+# Coordinate Projector
 
-packages = \
-['coordinate_projector']
+[![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['pyproj>=3.3.0,<4.0.0',
- 'python-dateutil>=2.8.2,<3.0.0',
- 'timezonefinder',
- 'types-python-dateutil>=2.8.9,<3.0.0']
-
-setup_kwargs = {
-    'name': 'coordinate-projector',
-    'version': '0.0.7',
-    'description': 'Project points from one projection to another using pyproj',
-    'long_description': '# Coordinate Projector\n\n[![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)\n\nThis is the Norwegian Geotechnical Institute (NGI) Python package for projecting coordinates. \nIt is a small shim on top of the library [pyproj](https://github.com/pyproj4/pyproj) that again is an interface to \n [PROJ](https://proj.org/).  \n\nReferences:\n\nLatest releases see [CHANGES.md](CHANGES.md)\n\n# Installation (end user) \n\n```bash\n\npip install coordinate-projector\n\n```\n\n## Basic usage\n\n### Project a point\n\n```python\nfrom coordinate_projector import Projector\n\nprojector = Projector()\n \nfrom_srid = "4326"\nto_srid = "3857"\n\n# Paris Lat(48.8589506) Lon(2.2768485) EPSG:4326\nfrom_east, from_north = 2.2768485, 48.8589506 \n\nprojected_east, projected_north = projector.transform(from_srid, to_srid, from_east, from_north)\n\n# Paris Lat(6250962.06) Lon(253457.62) EPSG:3857 is in metres - 2D projection\nassert abs(projected_east - 253457.62) <= 0.01\nassert abs(projected_north - 6250962.06) <= 0.01 \n\nprint(f"{projected_east=}, {projected_north=}")\n# projected_east=253457.6156334287, projected_north=6250962.062720417\n```\n\n# Getting Started developing\n\n1. Software dependencies\n\n   - Python 3.9 or higher\n   - Poetry\n   - black code formatter\n\n2. Clone this repository\n\n3. Install\n\n   `poetry install`\n\n\n\n# Build and Test\n\nRun in the project root folder: \n\n    poetry shell pytest \n\nBuild the package wheel: \n\n    poetry build\n\n# Publish\n\n# TODOs\n\n- Handle lines\n- Handle polygons\n\n# Contribute\n\nPlease start by adding an issue before submitting any pull requests.\n\n',
-    'author': 'Helge Smebye',
-    'author_email': None,
-    'maintainer': 'Jostein Leira',
-    'maintainer_email': 'jostein@leira.net',
-    'url': 'https://github.com/norwegian-geotechnical-institute/coordinate-projector',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<3.11',
-}
+This is the Norwegian Geotechnical Institute (NGI) Python package for projecting coordinates. 
+It is a small shim on top of the library [pyproj](https://github.com/pyproj4/pyproj) that again is an interface to 
+ [PROJ](https://proj.org/).  
+
+References:
+
+Latest releases see [CHANGES.md](CHANGES.md)
+
+# Installation (end user) 
+
+```bash
+
+pip install coordinate-projector
+
+```
+
+## Basic usage
+
+### Project a point
+
+```python
+from coordinate_projector import Projector
+
+projector = Projector()
+ 
+from_srid = "4326"
+to_srid = "3857"
+
+# Paris Lat(48.8589506) Lon(2.2768485) EPSG:4326
+from_east, from_north = 2.2768485, 48.8589506 
+
+projected_east, projected_north = projector.transform(from_srid, to_srid, from_east, from_north)
+
+# Paris Lat(6250962.06) Lon(253457.62) EPSG:3857 is in metres - 2D projection
+assert abs(projected_east - 253457.62) <= 0.01
+assert abs(projected_north - 6250962.06) <= 0.01 
+
+print(f"{projected_east=}, {projected_north=}")
+# projected_east=253457.6156334287, projected_north=6250962.062720417
+```
+
+# Getting Started developing
+
+1. Software dependencies
+
+   - Python 3.9 or higher
+   - Poetry
+   - black code formatter
+
+2. Clone this repository
+
+3. Install
+
+   `poetry install`
+
+
+
+# Build and Test
+
+Run in the project root folder: 
+
+    poetry shell pytest 
+
+Build the package wheel: 
+
+    poetry build
+
+# Publish
+
+# TODOs
+
+- Handle lines
+- Handle polygons
+
+# Contribute
+
+Please start by adding an issue before submitting any pull requests.
 
 
-setup(**setup_kwargs)
```

