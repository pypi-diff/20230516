# Comparing `tmp/ssb_sgis-0.1.9.tar.gz` & `tmp/ssb_sgis-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_sgis-0.1.9.tar", max compression
+gzip compressed data, was "ssb_sgis-0.2.0.tar", max compression
```

## Comparing `ssb_sgis-0.1.9.tar` & `ssb_sgis-0.2.0.tar`

### file list

```diff
@@ -1,37 +1,39 @@
--rw-r--r--   0        0        0     1074 2023-04-18 12:55:23.109640 ssb_sgis-0.1.9/LICENSE
--rw-r--r--   0        0        0     7332 2023-04-18 12:55:38.209936 ssb_sgis-0.1.9/README.md
--rw-r--r--   0        0        0     2477 2023-04-18 12:55:38.213936 ssb_sgis-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     1854 2023-04-18 12:55:38.213936 ssb_sgis-0.1.9/src/sgis/__init__.py
--rw-r--r--   0        0        0     2634 2023-04-18 12:55:23.137640 ssb_sgis-0.1.9/src/sgis/dapla.py
--rw-r--r--   0        0        0      666 2023-04-18 12:55:23.137640 ssb_sgis-0.1.9/src/sgis/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-18 12:55:23.137640 ssb_sgis-0.1.9/src/sgis/geopandas_tools/__init__.py
--rw-r--r--   0        0        0     8776 2023-04-18 12:55:23.137640 ssb_sgis-0.1.9/src/sgis/geopandas_tools/buffer_dissolve_explode.py
--rw-r--r--   0        0        0    27637 2023-04-18 12:55:23.137640 ssb_sgis-0.1.9/src/sgis/geopandas_tools/general.py
--rw-r--r--   0        0        0     5480 2023-04-18 12:55:23.137640 ssb_sgis-0.1.9/src/sgis/geopandas_tools/geometry_types.py
--rw-r--r--   0        0        0    16647 2023-04-18 12:55:23.137640 ssb_sgis-0.1.9/src/sgis/geopandas_tools/neighbors.py
--rw-r--r--   0        0        0    14812 2023-04-18 12:55:38.213936 ssb_sgis-0.1.9/src/sgis/geopandas_tools/overlay.py
--rw-r--r--   0        0        0     6316 2023-04-18 12:55:23.137640 ssb_sgis-0.1.9/src/sgis/geopandas_tools/point_operations.py
--rw-r--r--   0        0        0     5046 2023-04-18 12:55:23.137640 ssb_sgis-0.1.9/src/sgis/geopandas_tools/polygon_operations.py
--rw-r--r--   0        0        0     2468 2023-04-18 12:55:23.137640 ssb_sgis-0.1.9/src/sgis/helpers.py
--rw-r--r--   0        0        0        0 2023-04-18 12:55:23.137640 ssb_sgis-0.1.9/src/sgis/maps/__init__.py
--rw-r--r--   0        0        0    19154 2023-04-18 12:55:23.137640 ssb_sgis-0.1.9/src/sgis/maps/explore.py
--rw-r--r--   0        0        0    20499 2023-04-18 12:55:23.137640 ssb_sgis-0.1.9/src/sgis/maps/legend.py
--rw-r--r--   0        0        0    16711 2023-04-18 12:55:23.137640 ssb_sgis-0.1.9/src/sgis/maps/map.py
--rw-r--r--   0        0        0    12875 2023-04-18 12:55:38.213936 ssb_sgis-0.1.9/src/sgis/maps/maps.py
--rw-r--r--   0        0        0    13848 2023-04-18 12:55:23.137640 ssb_sgis-0.1.9/src/sgis/maps/thematicmap.py
--rw-r--r--   0        0        0        0 2023-04-18 12:55:23.137640 ssb_sgis-0.1.9/src/sgis/networkanalysis/__init__.py
--rw-r--r--   0        0        0     6199 2023-04-18 12:55:38.213936 ssb_sgis-0.1.9/src/sgis/networkanalysis/_get_route.py
--rw-r--r--   0        0        0     2017 2023-04-18 12:55:38.213936 ssb_sgis-0.1.9/src/sgis/networkanalysis/_od_cost_matrix.py
--rw-r--r--   0        0        0     4182 2023-04-18 12:55:23.137640 ssb_sgis-0.1.9/src/sgis/networkanalysis/_points.py
--rw-r--r--   0        0        0     4487 2023-04-18 12:55:38.213936 ssb_sgis-0.1.9/src/sgis/networkanalysis/_service_area.py
--rw-r--r--   0        0        0    12639 2023-04-18 12:55:38.213936 ssb_sgis-0.1.9/src/sgis/networkanalysis/closing_network_holes.py
--rw-r--r--   0        0        0    12096 2023-04-18 12:55:38.213936 ssb_sgis-0.1.9/src/sgis/networkanalysis/cutting_lines.py
--rw-r--r--   0        0        0     9247 2023-04-18 12:55:38.213936 ssb_sgis-0.1.9/src/sgis/networkanalysis/directednetwork.py
--rw-r--r--   0        0        0     3438 2023-04-18 12:55:38.213936 ssb_sgis-0.1.9/src/sgis/networkanalysis/finding_isolated_networks.py
--rw-r--r--   0        0        0     8242 2023-04-18 12:55:38.213936 ssb_sgis-0.1.9/src/sgis/networkanalysis/network.py
--rw-r--r--   0        0        0    62946 2023-04-18 12:55:38.213936 ssb_sgis-0.1.9/src/sgis/networkanalysis/networkanalysis.py
--rw-r--r--   0        0        0    12439 2023-04-18 12:55:38.213936 ssb_sgis-0.1.9/src/sgis/networkanalysis/networkanalysisrules.py
--rw-r--r--   0        0        0     6740 2023-04-18 12:55:38.213936 ssb_sgis-0.1.9/src/sgis/networkanalysis/nodes.py
--rw-r--r--   0        0        0        0 2023-04-18 12:55:23.137640 ssb_sgis-0.1.9/src/sgis/py.typed
--rw-r--r--   0        0        0     3765 2023-04-18 12:55:23.137640 ssb_sgis-0.1.9/src/sgis/read_parquet.py
--rw-r--r--   0        0        0     8696 1970-01-01 00:00:00.000000 ssb_sgis-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-16 11:10:02.287542 ssb_sgis-0.2.0/LICENSE
+-rw-r--r--   0        0        0     7543 2023-05-16 11:10:02.287542 ssb_sgis-0.2.0/README.md
+-rw-r--r--   0        0        0     2539 2023-05-16 11:10:18.679628 ssb_sgis-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2230 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/__init__.py
+-rw-r--r--   0        0        0     3243 2023-05-16 11:10:18.679628 ssb_sgis-0.2.0/src/sgis/dapla.py
+-rw-r--r--   0        0        0      666 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/geopandas_tools/__init__.py
+-rw-r--r--   0        0        0     8028 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/geopandas_tools/buffer_dissolve_explode.py
+-rw-r--r--   0        0        0    23937 2023-05-16 11:10:18.679628 ssb_sgis-0.2.0/src/sgis/geopandas_tools/general.py
+-rw-r--r--   0        0        0     5480 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/geopandas_tools/geometry_types.py
+-rw-r--r--   0        0        0    14520 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/geopandas_tools/neighbors.py
+-rw-r--r--   0        0        0    11815 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/geopandas_tools/overlay.py
+-rw-r--r--   0        0        0     6888 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/geopandas_tools/point_operations.py
+-rw-r--r--   0        0        0    10556 2023-05-16 11:10:18.679628 ssb_sgis-0.2.0/src/sgis/geopandas_tools/polygon_operations.py
+-rw-r--r--   0        0        0     9722 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/geopandas_tools/to_geodataframe.py
+-rw-r--r--   0        0        0     2674 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/helpers.py
+-rw-r--r--   0        0        0        0 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/maps/__init__.py
+-rw-r--r--   0        0        0    20212 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/maps/explore.py
+-rw-r--r--   0        0        0     1938 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/maps/httpserver.py
+-rw-r--r--   0        0        0    20499 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/maps/legend.py
+-rw-r--r--   0        0        0    17556 2023-05-16 11:10:18.679628 ssb_sgis-0.2.0/src/sgis/maps/map.py
+-rw-r--r--   0        0        0    16124 2023-05-16 11:10:18.679628 ssb_sgis-0.2.0/src/sgis/maps/maps.py
+-rw-r--r--   0        0        0    14132 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/maps/thematicmap.py
+-rw-r--r--   0        0        0        0 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/networkanalysis/__init__.py
+-rw-r--r--   0        0        0     6218 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/networkanalysis/_get_route.py
+-rw-r--r--   0        0        0     2017 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/networkanalysis/_od_cost_matrix.py
+-rw-r--r--   0        0        0     4206 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/networkanalysis/_points.py
+-rw-r--r--   0        0        0     4487 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/networkanalysis/_service_area.py
+-rw-r--r--   0        0        0    12433 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/networkanalysis/closing_network_holes.py
+-rw-r--r--   0        0        0    11984 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/networkanalysis/cutting_lines.py
+-rw-r--r--   0        0        0     9375 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/networkanalysis/directednetwork.py
+-rw-r--r--   0        0        0     3359 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/networkanalysis/finding_isolated_networks.py
+-rw-r--r--   0        0        0     7686 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/networkanalysis/network.py
+-rw-r--r--   0        0        0    66761 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/networkanalysis/networkanalysis.py
+-rw-r--r--   0        0        0    12643 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/networkanalysis/networkanalysisrules.py
+-rw-r--r--   0        0        0     6740 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/networkanalysis/nodes.py
+-rw-r--r--   0        0        0        0 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/py.typed
+-rw-r--r--   0        0        0     3774 2023-05-16 11:10:02.319543 ssb_sgis-0.2.0/src/sgis/read_parquet.py
+-rw-r--r--   0        0        0     8831 1970-01-01 00:00:00.000000 ssb_sgis-0.2.0/PKG-INFO
```

### Comparing `ssb_sgis-0.1.9/LICENSE` & `ssb_sgis-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.9/README.md` & `ssb_sgis-0.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 [![PyPI](https://img.shields.io/pypi/v/ssb-sgis.svg)][pypi_]
 [![Status](https://img.shields.io/pypi/status/ssb-sgis.svg)][status]
 [![Python Version](https://img.shields.io/pypi/pyversions/ssb-sgis)][python version]
 [![License](https://img.shields.io/pypi/l/ssb-sgis)][license]
 
 [![Documentation](https://img.shields.io/badge/Documentation-GitHub_Pages-green.svg)](https://statisticsnorway.github.io/ssb-sgis/index.html)
 [![Tests](https://github.com/statisticsnorway/ssb-sgis/workflows/Tests/badge.svg)][tests]
-[![Coverage](https://sonarcloud.io/component_measures?id=statisticsnorway_ssb-gis-utils&metric=new_coverage&view=list)][coverage]
 
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
 
 [pypi_]: https://pypi.org/project/ssb-sgis/
 [status]: https://pypi.org/project/ssb-sgis/
 [python version]: https://pypi.org/project/ssb-sgis
@@ -24,73 +23,59 @@
 [black]: https://github.com/psf/black
 
 sgis builds on the geopandas package and provides functions that make it easier to do GIS in python.
 Features include network analysis, functions for exploring multiple GeoDataFrames in a layered interactive map,
 and vector operations like finding k-nearest neighbours, splitting lines by points, snapping and closing holes
 in polygons by size.
 
+To install, use one of:
+
+```shell
+poetry add ssb-sgis
+pip install ssb-sgis
+```
+
 ## Network analysis examples
 
 Preparing for network analysis:
 
 ```python
 import sgis as sg
-import pandas as pd
+
 
 roads = sg.read_parquet_url(
     "https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_oslo_2022.parquet"
 )
 
 connected_roads = sg.get_connected_components(roads).query("connected == 1")
 
 directed_roads = sg.make_directed_network(
     connected_roads,
     direction_col="oneway",
     direction_vals_bft=("B", "FT", "TF"),
     minute_cols=("drivetime_fw", "drivetime_bw"),
 )
 
-rules = sg.NetworkAnalysisRules(weight="minutes", directed=True)
+rules = sg.NetworkAnalysisRules(directed=True, weight="minutes")
 
 nwa = sg.NetworkAnalysis(network=directed_roads, rules=rules)
 
 nwa
 ```
 
     NetworkAnalysis(
-        network=DirectedNetwork(6364 km, percent_bidirectional=87),
+        network=Network(6364 km, percent_bidirectional=87),
         rules=NetworkAnalysisRules(weight=minutes, directed=True, search_tolerance=250, search_factor=0, split_lines=False, ...),
-        log=True, detailed_log=True,
+        log=True, detailed_log=False,
     )
 
-Get number of times each line segment was visited, with optional weighting.
-
-```python
-origins = points.iloc[:75]
-destinations = points.iloc[75:150]
-
-# creating uniform weights of 10
-od_pairs = pd.MultiIndex.from_product([origins.index, destinations.index])
-weights = pd.DataFrame(index=od_pairs)
-weights["weight"] = 10
-
-frequencies = nwa.get_route_frequencies(origins, destinations, weight_df=weights)
-
-# plot the results
-m = sg.ThematicMap(sg.buff(frequencies, 15), column="frequency", black=True)
-m.cmap = "plasma"
-m.title = "Number of times each road was used,\nweighted * 10"
-m.plot()
-```
-
-![png](docs/examples/network_analysis_examples_files/network_analysis_examples_5_0.png)
-
 Fast many-to-many travel times/distances.
 
 ```python
+points = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_oslo.parquet")
 od = nwa.od_cost_matrix(points, points)
 
 print(od)
 ```
 
             origin  destination    minutes
     0            0            0   0.000000
@@ -103,14 +88,36 @@
     999996     999          996  17.820664
     999997     999          997  10.288465
     999998     999          998  14.798257
     999999     999          999   0.000000
 
     [1000000 rows x 3 columns]
 
+Get number of times each line segment was visited, with optional weighting.
+
+```python
+origins = points.iloc[:100]
+destinations = points.iloc[100:200]
+
+# creating uniform weights of 10
+od_pairs = pd.MultiIndex.from_product([origins.index, destinations.index])
+weights = pd.DataFrame(index=od_pairs)
+weights["weight"] = 10
+
+frequencies = nwa.get_route_frequencies(origins, destinations, weight_df=weights)
+
+# plot the results
+m = sg.ThematicMap(sg.buff(frequencies, 15), column="frequency", black=True)
+m.cmap = "plasma"
+m.title = "Number of times each road was used,\nweighted * 10"
+m.plot()
+```
+
+![png](docs/examples/network_analysis_examples_files/network_analysis_examples_5_0.png)
+
 Get the area that can be reached within one or more breaks.
 
 ```python
 service_areas = nwa.service_area(
     points.iloc[[0]],
     breaks=np.arange(1, 11),
 )
@@ -135,14 +142,16 @@
 m.title = "Four fastest routes from A to B"
 m.legend.title = "Rank"
 m.plot()
 ```
 
 ![png](docs/examples/network_analysis_examples_files/network_analysis_examples_11_0.png)
 
+More network analysis examples can be found here: https://github.com/statisticsnorway/ssb-sgis/blob/main/docs/network_analysis_demo_template.md
+
 Road data for Norway can be downloaded here: https://kartkatalog.geonorge.no/metadata/nvdb-ruteplan-nettverksdatasett/8d0f9066-34f9-4423-be12-8e8523089313
 
 ## Developer information
 
 ### Git LFS
 
 The data in the testdata directory is stored with [Git LFS](https://git-lfs.com/).
```

### Comparing `ssb_sgis-0.1.9/pyproject.toml` & `ssb_sgis-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssb-sgis"
-version = "0.1.9"
+version = "0.2.0"
 description = "GIS functions used at Statistics Norway."
 authors = ["Statistics Norway <ort@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "sgis", from = "src"}]
 homepage = "https://github.com/statisticsnorway/ssb-sgis"
 repository = "https://github.com/statisticsnorway/ssb-sgis"
@@ -14,58 +14,59 @@
 ]
 
 [tool.poetry.urls]
 Changelog = "https://github.com/statisticsnorway/ssb-sgis/releases"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
-branca = "^0.6.0"
-folium = "^0.14.0"
-geopandas = "^0.12.2"
-igraph = "^0.10.4"
-mapclassify = "^2.5.0"
-matplotlib = "^3.7.0"
-networkx = "^3.0"
-numpy = "^1.24.2"
-pandas = "^1.5.3"
-pyarrow = "^11.0.0"
-requests = "^2.28.2"
-scikit-learn = "^1.2.1"
-shapely = "^2.0.1"
-xyzservices = "^2023.2.0"
-jenkspy = "^0.3.2"
+branca = ">=0.6.0"
+folium = ">=0.14.0"
+geopandas = ">=0.12.2"
+igraph = ">=0.10.4"
+mapclassify = ">=2.5.0"
+matplotlib = ">=3.7.0"
+networkx = ">=3.0"
+numpy = ">=1.24.2"
+pandas = ">=1.5.3"
+pyarrow = ">=11.0.0"
+requests = ">=2.28.2"
+scikit-learn = ">=1.2.1"
+shapely = ">=2.0.1"
+xyzservices = ">=2023.2.0"
+jenkspy = ">=0.3.2"
+ipython = ">=8.13.2"
 
 [tool.poetry.group.dev.dependencies]
-black = {extras = ["d", "jupyter"], version = "^23.1.0"}
-coverage = {extras = ["toml"], version = "^7.2.1"}
-darglint = "^1.8.1"
-deptry = "^0.8.0"
-flake8 = "^6.0.0"
-flake8-bandit = "^4.1.1"
-flake8-bugbear = "^23.2.13"
-flake8-docstrings = "^1.7.0"
-flake8-rst-docstrings = "^0.3.0"
-furo = "^2023.3.27"
-isort = "^5.12.0"
-jupyterlab = "^3.6.1"
-jupytext = "^1.14.5"
-mypy = "^1.0.1"
-myst-parser = {version = "^0.19.1"}
-pep8-naming = "^0.13.3"
-pre-commit = "^3.1.1"
-pre-commit-hooks = "^4.4.0"
-pyogrio = "^0.5.1"
-pytest = "^7.2.1"
-pytest-cov = "^4.0.0"
-pytest-mock = "^3.10.0"
-pyupgrade = "^3.3.1"
+black = {extras = ["d", "jupyter"], version = ">=23.1.0"}
+coverage = {extras = ["toml"], version = ">=7.2.1"}
+darglint = ">=1.8.1"
+deptry = ">=0.8.0"
+flake8 = ">=6.0.0"
+flake8-bandit = ">=4.1.1"
+flake8-bugbear = ">=23.2.13"
+flake8-docstrings = ">=1.7.0"
+flake8-rst-docstrings = ">=0.3.0"
+furo = ">=2023.3.27"
+isort = ">=5.12.0"
+jupyterlab = ">=3.6.1"
+jupytext = ">=1.14.5"
+mypy = ">=1.0.1"
+myst-parser = {version = ">=0.19.1"}
+pep8-naming = ">=0.13.3"
+pre-commit = ">=3.1.1"
+pre-commit-hooks = ">=4.4.0"
+pyogrio = ">=0.5.1"
+pytest = ">=7.2.1"
+pytest-cov = ">=4.0.0"
+pytest-mock = ">=3.10.0"
+pyupgrade = ">=3.3.1"
 sphinx = ">=6.1.3"
-sphinx-autobuild = "^2021.3.14"
-sphinx-autodoc-typehints = "^1.22"
-xdoctest = {extras = ["colors"], version = "^1.1.1"}
+sphinx-autobuild = ">=2021.3.14"
+sphinx-autodoc-typehints = ">=1.22"
+xdoctest = {extras = ["colors"], version = ">=1.1.1"}
 
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
 tests = ["tests", "*/tests"]
 
 [tool.coverage.run]
```

### Comparing `ssb_sgis-0.1.9/src/sgis/__init__.py` & `ssb_sgis-0.2.0/src/sgis/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,54 @@
 # flake8: noqa: F401
 from .geopandas_tools.buffer_dissolve_explode import (
     buff,
     buffdiss,
     buffdissexp,
-    buffexp,
     dissexp,
 )
 from .geopandas_tools.general import (
+    bounds_to_points,
+    bounds_to_polygon,
     clean_clip,
     clean_geoms,
     coordinate_array,
+    drop_inactive_geometry_columns,
+    make_grid,
+    make_grid_from_bbox,
+    make_ssb_grid,
     points_in_bounds,
     random_points,
     random_points_in_polygons,
-    to_gdf,
+    rename_geometry_if,
     to_lines,
     to_multipoint,
 )
 from .geopandas_tools.geometry_types import (
     get_geom_type,
     is_single_geom_type,
     to_single_geom_type,
 )
 from .geopandas_tools.neighbors import (
     get_all_distances,
     get_k_nearest_neighbors,
     get_neighbor_indices,
+    k_nearest_neighbors,
 )
-from .geopandas_tools.overlay import clean_shapely_overlay, overlay, overlay_update
+from .geopandas_tools.overlay import clean_overlay, overlay_update
 from .geopandas_tools.point_operations import snap_all, snap_within_distance
-from .geopandas_tools.polygon_operations import close_all_holes, close_small_holes
+from .geopandas_tools.polygon_operations import (
+    close_all_holes,
+    close_small_holes,
+    get_overlapping_polygon_indices,
+    get_overlapping_polygon_product,
+    get_overlapping_polygons,
+    get_polygon_clusters,
+)
+from .geopandas_tools.to_geodataframe import to_gdf
+from .maps.explore import Explore
 from .maps.legend import Legend
 from .maps.maps import clipmap, explore, qtm, samplemap
 from .maps.thematicmap import ThematicMap
 from .networkanalysis.closing_network_holes import (
     close_network_holes,
     close_network_holes_to_deadends,
 )
```

### Comparing `ssb_sgis-0.1.9/src/sgis/dapla.py` & `ssb_sgis-0.2.0/src/sgis/dapla.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Functions for reading and writing GeoDataFrames in Statistics Norway's GCS Dapla.
 """
 import os
+from pathlib import Path
 
+import dapla as dp
 import geopandas as gpd
 import pandas as pd
-from dapla import FileClient, details
 from geopandas import GeoDataFrame
 from geopandas.io.arrow import _geopandas_to_arrow
 from pyarrow import parquet
 
 
 def exists(path: str) -> bool:
     """Returns True if the path exists, and False if it doesn't.
@@ -18,61 +19,80 @@
     Args:
         path (str): The path to the file or directory.
 
     Returns:
         True if the path exists, False if not.
     """
     try:
-        details(path)
+        dp.details(path)
         return True
     except FileNotFoundError:
         return False
     except ModuleNotFoundError:
         return os.path.exists(path)
 
 
 def read_geopandas(path: str, **kwargs) -> GeoDataFrame:
-    """Reads geoparquet or other geodata* from a file on GCS.
+    """Reads geoparquet or other geodata from a file on GCS.
 
     Note:
-        Does not currently read shapelfiles or filegeodatabases.
+        Does not currently read shapefiles or filegeodatabases.
 
     Args:
         path: path to a file on Google Cloud Storage.
-        **kwargs: additional keyword arguments passed to geopandas' read_parquet
+        **kwargs: Additional keyword arguments passed to geopandas' read_parquet
             or read_file, depending on the file type.
 
      Returns:
          A GeoDataFrame.
     """
-    fs = FileClient.get_gcs_file_system()
+    fs = dp.FileClient.get_gcs_file_system()
 
-    if "parquet" in path:
-        with fs.open(path, mode="rb") as file:
-            return gpd.read_parquet(file, **kwargs)
-    else:
-        with fs.open(path, mode="rb") as file:
-            return gpd.read_file(file, **kwargs)
+    try:
+        if "parquet" in path:
+            with fs.open(path, mode="rb") as file:
+                return gpd.read_parquet(file, **kwargs)
+        else:
+            with fs.open(path, mode="rb") as file:
+                return gpd.read_file(file, **kwargs)
+    except FileNotFoundError as e:
+        parent = str(Path(path).parent)
+        if exists(parent):
+            print(
+                f"Didn't find the file {path}"
+                "\nHere are the files in the given parent directory:"
+            )
+            print(dp.FileClient().ls(parent))
+        raise e
 
 
 def write_geopandas(df: gpd.GeoDataFrame, gcs_path: str, **kwargs) -> None:
     """Writes a GeoDataFrame to the speficied format.
 
     Note:
         Does not currently write to shapelfile or filegeodatabase.
 
     Args:
-        df: The GeoDataFrame to write
+        df: The GeoDataFrame to write.
         gcs_path: The path to the file you want to write to.
-        **kwargs: additional keyword arguments passed to parquet.write_table
+        **kwargs: Additional keyword arguments passed to parquet.write_table
             (for parquet) or geopandas' to_file method (if not parquet).
     """
     pd.io.parquet.BaseImpl.validate_dataframe(df)
 
-    fs = FileClient.get_gcs_file_system()
+    if not len(df):
+        try:
+            dp.write_pandas(df, gcs_path, **kwargs)
+        except Exception:
+            dp.write_pandas(
+                df.drop(df._geometry_column_name, axis=1), gcs_path, **kwargs
+            )
+        return
+
+    fs = dp.FileClient.get_gcs_file_system()
 
     if ".parquet" in gcs_path:
         with fs.open(gcs_path, mode="wb") as buffer:
             table = _geopandas_to_arrow(df, index=df.index, schema_version=None)
             parquet.write_table(table, buffer, compression="snappy", **kwargs)
         return
```

### Comparing `ssb_sgis-0.1.9/src/sgis/exceptions.py` & `ssb_sgis-0.2.0/src/sgis/exceptions.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.9/src/sgis/geopandas_tools/buffer_dissolve_explode.py` & `ssb_sgis-0.2.0/src/sgis/geopandas_tools/buffer_dissolve_explode.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,53 @@
 """Functions that buffer, dissolve and/or explodes geometries while fixing geometries.
 
-Functions with the purpose of making the code cleaner when buffering, dissolving,
-exploding and repairing geometries. The functions are identical to doing buffer,
-dissolve and explode individually, except for the following:
+The functions do the same as the geopandas buffer, dissolve and explode methods, except
+for the following:
 
-- Geometries are always repaired after buffer and dissolve.
+- Geometries are made valid after buffer and dissolve.
 
-- The buffer resolution defaults to 50, while geopandas' default is 16.
+- The buffer resolution defaults to 50 (geopandas' default is 16).
 
-- The buff function returns a GeoDataFrame, the geopandas method returns a GeoSeries.
+- If 'by' is not specified, the index will be labeled 0, 1, …, n - 1 after exploded, instead of 0, 0, …, 0 as it will with the geopandas defaults.
+
+- index_parts is set to False, which will be the default in a future version of geopandas.
 
-- index_parts is set to False, which will be the default value in a future version of geopandas.
+- The buff function returns a GeoDataFrame, the geopandas method returns a GeoSeries.
 """
 
-from geopandas import GeoDataFrame
+from geopandas import GeoDataFrame, GeoSeries
+
+
+def _decide_ignore_index(kwargs: dict) -> tuple[dict, bool]:
+    if "ignore_index" in kwargs:
+        return kwargs, kwargs.pop("ignore_index")
+
+    if not kwargs.get("by", None):
+        return kwargs, True
 
+    if kwargs.get("as_index", True):
+        return kwargs, False
 
-IGNORE_INDEX_ERROR_MESSAGE = (
-    "Cannot set ignore_index. Set as_index=False to reset the index and keep "
-    "the 'by' columns. Or use reset_index(drop=True) to remove the 'by' "
-    "columns completely"
-)
+    return kwargs, True
 
 
 def buffdissexp(
     gdf: GeoDataFrame,
-    distance,
+    distance: int | float,
     *,
-    resolution=50,
+    resolution: int = 50,
     index_parts: bool = False,
     copy: bool = True,
     **dissolve_kwargs,
 ) -> GeoDataFrame:
     """Buffers and dissolves overlapping geometries.
 
     It takes a GeoDataFrame and buffer, fixes, dissolves, fixes and explodes geometries.
+    If the 'by' parameter is not specified, the index will labeled 0, 1, …, n - 1,
+    instead of 0, 0, …, 0. If 'by' is speficied, this will be the index.
 
     Args:
         gdf: the GeoDataFrame that will be buffered, dissolved and exploded.
         distance: the distance (meters, degrees, depending on the crs) to buffer
             the geometry by
         resolution: The number of segments used to approximate a quarter circle.
             Here defaults to 50, as opposed to the default 16 in geopandas.
@@ -47,38 +56,39 @@
         copy: Whether to copy the GeoDataFrame before buffering.
         **dissolve_kwargs: additional keyword arguments passed to geopandas' dissolve.
 
     Returns:
         A buffered GeoDataFrame where overlapping geometries are dissolved.
 
     """
-    if "ignore_index" in dissolve_kwargs:
-        raise ValueError(IGNORE_INDEX_ERROR_MESSAGE)
+    dissolve_kwargs, ignore_index = _decide_ignore_index(dissolve_kwargs)
 
-    geom_col = gdf._geometry_column_name
+    dissolved = buffdiss(
+        gdf,
+        distance,
+        resolution=resolution,
+        copy=copy,
+        **dissolve_kwargs,
+    )
 
-    buffered = buff(gdf, distance, resolution=resolution, copy=copy)
-
-    dissolved = buffered.dissolve(**dissolve_kwargs)
-
-    dissolved[geom_col] = dissolved.make_valid()
-
-    return dissolved.explode(index_parts=index_parts)
+    return dissolved.explode(index_parts=index_parts, ignore_index=ignore_index)
 
 
 def buffdiss(
     gdf: GeoDataFrame,
-    distance,
-    resolution=50,
+    distance: int | float,
+    resolution: int = 50,
     copy: bool = True,
     **dissolve_kwargs,
 ) -> GeoDataFrame:
     """Buffers and dissolves geometries.
 
     It takes a GeoDataFrame and buffer, fixes, dissolves and fixes geometries.
+    If the 'by' parameter is not specified, the index will labeled 0, 1, …, n - 1,
+    instead of 0, 0, …, 0. If 'by' is speficied, this will be the index.
 
     Args:
         gdf: the GeoDataFrame that will be
             buffered and dissolved.
         distance: the distance (meters, degrees, depending on the crs) to buffer
             the geometry by
         resolution: The number of segments used to approximate a quarter circle.
@@ -133,17 +143,14 @@
 
     >>> sg.buffdiss(points, 100, by="group", as_index=False)
       group                                           geometry    number
     0     a  MULTIPOLYGON (((258866.258 6648220.031, 258865...  0.323948
     1     b  MULTIPOLYGON (((258404.858 6647830.931, 258404...  0.687635
     2     d  MULTIPOLYGON (((258180.258 6647935.731, 258179...  0.580157
     """
-    if "ignore_index" in dissolve_kwargs:
-        raise ValueError(IGNORE_INDEX_ERROR_MESSAGE)
-
     geom_col = gdf._geometry_column_name
 
     buffered = buff(gdf, distance, resolution=resolution, copy=copy)
 
     dissolved = buffered.dissolve(**dissolve_kwargs)
 
     dissolved[geom_col] = dissolved.make_valid()
@@ -165,62 +172,27 @@
         index_parts: If False (default), the index after dissolve is respected. If
             True, an integer index level is added during explode.
         **dissolve_kwargs: additional keyword arguments passed to geopandas' dissolve.
 
     Returns:
         A GeoDataFrame where overlapping geometries are dissolved.
     """
-    if "ignore_index" in dissolve_kwargs:
-        raise ValueError(IGNORE_INDEX_ERROR_MESSAGE)
-
     geom_col = gdf._geometry_column_name
 
+    dissolve_kwargs, ignore_index = _decide_ignore_index(dissolve_kwargs)
+
     dissolved = gdf.dissolve(**dissolve_kwargs)
 
     dissolved[geom_col] = dissolved.make_valid()
 
-    return dissolved.explode(index_parts=index_parts)
-
-
-def buffexp(
-    gdf,
-    distance,
-    resolution=50,
-    index_parts: bool = False,
-    copy: bool = True,
-    **buffer_kwargs,
-):
-    """Buffers and explodes geometries.
-
-    It takes a GeoDataFrame and buffer, fixes and explodes geometries.
-
-    Args:
-        gdf: the GeoDataFrame that will be buffered, dissolved and exploded.
-        distance: the distance (meters, degrees, depending on the crs) to buffer
-            the geometry by
-        resolution: The number of segments used to approximate a quarter circle.
-            Here defaults to 50, as opposed to the default 16 in geopandas.
-        index_parts: If False (default), the index after dissolve is respected. If
-            True, an integer index level is added during explode.
-        copy: Whether to copy the GeoDataFrame before buffering.
-        **buffer_kwargs: additional keyword arguments passed to geopandas' buffer.
-
-    Returns:
-        A buffered GeoDataFrame where geometries are exploded.
-    """
-    if "ignore_index" in buffer_kwargs:
-        raise ValueError(IGNORE_INDEX_ERROR_MESSAGE)
-
-    return buff(
-        gdf, distance, resolution=resolution, copy=copy, **buffer_kwargs
-    ).explode(index_parts=index_parts)
+    return dissolved.explode(index_parts=index_parts, ignore_index=ignore_index)
 
 
 def buff(
-    gdf: GeoDataFrame,
+    gdf: GeoDataFrame | GeoSeries,
     distance: int | float,
     resolution: int = 50,
     copy: bool = True,
     **buffer_kwargs,
 ) -> GeoDataFrame:
     """Buffers a GeoDataFrame with high resolution and returns a new GeoDataFrame.
 
@@ -232,14 +204,18 @@
             Here defaults to 50, as opposed to the default 16 in geopandas.
         copy: Whether to copy the GeoDataFrame before buffering.
         **buffer_kwargs: additional keyword arguments passed to geopandas' buffer.
 
     Returns:
         A buffered GeoDataFrame.
     """
+
+    if isinstance(gdf, GeoSeries):
+        return gdf.buffer(distance, resolution=resolution, **buffer_kwargs).make_valid()
+
     geom_col = gdf._geometry_column_name
 
     if copy:
         gdf = gdf.copy()
 
     gdf[geom_col] = gdf.buffer(
         distance, resolution=resolution, **buffer_kwargs
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ssb_sgis-0.1.9/src/sgis/geopandas_tools/general.py` & `ssb_sgis-0.2.0/src/sgis/geopandas_tools/general.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,38 @@
-import numbers
 import warnings
-from collections.abc import Iterator, Sized
 
 import geopandas as gpd
 import numpy as np
 import pandas as pd
 from geopandas import GeoDataFrame, GeoSeries
 from geopandas.array import GeometryDtype
-from numpy.random import random as _np_random
-from pandas.api.types import is_dict_like
 from shapely import (
     Geometry,
+    box,
     force_2d,
     get_exterior_ring,
     get_interior_ring,
     get_num_interior_rings,
     get_parts,
-    wkb,
     wkt,
 )
-from shapely.geometry import LineString, Point
+from shapely.geometry import LineString, Point, Polygon
 from shapely.ops import unary_union
 
+from .geometry_types import to_single_geom_type
+from .to_geodataframe import to_gdf
+
 
 def coordinate_array(
-    gdf: GeoDataFrame,
+    gdf: GeoDataFrame | GeoSeries,
 ) -> np.ndarray[np.ndarray[float], np.ndarray[float]]:
-    """Creates a 2d ndarray of coordinates from a GeoDataFrame of points.
+    """Creates a 2d ndarray of coordinates from point geometries.
 
     Args:
-        gdf: GeoDataFrame of point geometries.
+        gdf: GeoDataFrame or GeoSeries of point geometries.
 
     Returns:
         np.ndarray of np.ndarrays of coordinates.
 
     Examples
     --------
     >>> from sgis import coordinate_array, random_points
@@ -47,16 +46,25 @@
     4  POINT (0.38046 0.87879)
     >>> coordinate_array(points)
     array([[0.59376221, 0.92577159],
         [0.34074678, 0.91650446],
         [0.74840912, 0.10626954],
         [0.00965935, 0.87867915],
         [0.38045827, 0.87878816]])
+    >>> coordinate_array(points.geometry)
+    array([[0.59376221, 0.92577159],
+        [0.34074678, 0.91650446],
+        [0.74840912, 0.10626954],
+        [0.00965935, 0.87867915],
+        [0.38045827, 0.87878816]])
     """
-    return np.array([(geom.x, geom.y) for geom in gdf.geometry])
+    if isinstance(gdf, GeoDataFrame):
+        return np.array([(geom.x, geom.y) for geom in gdf.geometry])
+    else:
+        return np.array([(geom.x, geom.y) for geom in gdf])
 
 
 def _push_geom_col(gdf: GeoDataFrame) -> GeoDataFrame:
     """Makes the geometry column the rightmost column in the GeoDataFrame.
 
     Args:
         gdf: GeoDataFrame.
@@ -74,19 +82,213 @@
             isinstance(gdf[col].dtype, GeometryDtype)
             and col != gdf._geometry_column_name
         ):
             gdf = gdf.drop(col, axis=1)
     return gdf
 
 
-def rename_geometry_if(gdf):
+def rename_geometry_if(gdf: GeoDataFrame) -> GeoDataFrame:
     geom_col = gdf._geometry_column_name
-    if geom_col == "geometry":
+    if geom_col == "geometry" and geom_col in gdf.columns:
         return gdf
-    return gdf.rename_geometry("geometry")
+    elif geom_col in gdf.columns:
+        return gdf.rename_geometry("geometry")
+
+    geom_cols = list(
+        {col for col in gdf.columns if isinstance(gdf[col].dtype, GeometryDtype)}
+    )
+    if len(geom_cols) == 1:
+        gdf._geometry_column_name = geom_cols[0]
+        return gdf.rename_geometry("geometry")
+
+    raise ValueError(
+        "There are multiple geometry columns and none are the active geometry"
+    )
+
+
+def make_grid_from_bbox(
+    minx: int | float,
+    miny: int | float,
+    maxx: int | float,
+    maxy: int | float,
+    *_,
+    gridsize: int | float,
+    crs,
+) -> GeoDataFrame:
+    """Creates a polygon grid from a bounding box.
+
+    Creates a GeoDataFrame of grid cells of a given size within the given
+    maxumum and mimimum x and y values.
+
+    Args:
+        minx: Minumum x coordinate.
+        miny: Minumum y coordinate.
+        maxx: Maximum x coordinate.
+        maxy: Maximum y coordinate.
+        gridsize: Length of the grid walls.
+        crs: Coordinate reference system.
+
+    Returns:
+        GeoDataFrame with grid geometries.
+    """
+    grid_cells1 = []
+    grid_cells2 = []
+    grid_cells3 = []
+    grid_cells4 = []
+    for x0 in np.arange(minx, maxx + gridsize, gridsize):
+        for y0 in np.arange(miny, maxy + gridsize, gridsize):
+            x1 = x0 - gridsize
+            y1 = y0 + gridsize
+            grid_cells1.append(x0)
+            grid_cells2.append(y0)
+            grid_cells3.append(x1)
+            grid_cells4.append(y1)
+
+    grid_cells = box(grid_cells1, grid_cells2, grid_cells3, grid_cells4)
+
+    return gpd.GeoDataFrame(grid_cells, columns=["geometry"], crs=crs)
+
+
+def make_grid(gdf: GeoDataFrame, gridsize: int | float) -> GeoDataFrame:
+    """Create a polygon grid around a GeoDataFrame.
+
+    Creates a GeoDataFrame of grid cells of a given size within the bounds of
+    a given GeoDataFrame.
+
+    Args:
+        gdf: A GeoDataFrame.
+        gridsize: Length of the grid walls.
+
+    Returns:
+        GeoDataFrame with grid polygons.
+    """
+    minx, miny, maxx, maxy = gdf.total_bounds
+    return make_grid_from_bbox(minx, miny, maxx, maxy, gridsize=gridsize, crs=gdf.crs)
+
+
+def make_ssb_grid(gdf: GeoDataFrame, gridsize: int = 1000) -> GeoDataFrame:
+    """Creates a polygon grid around a GeoDataFrame with an SSB id column.
+
+    Creates a grid that follows the grids produced by Statistics Norway.
+    The GeoDataFrame must have 25833 as crs (UTM 33 N).
+
+    Courtesy https://gis.stackexchange.com/questions/269243/creating-polygon-grid-using-geopandas
+
+    Args:
+        gdf: A GeoDataFrame.
+        gridsize: Size of the grid in meters.
+
+    Returns:
+        GeoDataFrame with grid geometries and a column 'SSBID'.
+
+    Raises:
+        ValueError: If the GeoDataFrame does not have 25833 as crs.
+    """
+    if gdf.crs != 25833:
+        raise ValueError(
+            "Geodataframe must have crs = 25833. Use df.set_crs(25833) to set "
+            "projection or df.to_crs(25833) for transforming."
+        )
+
+    minx, miny, maxx, maxy = gdf.total_bounds
+
+    # Adjust for SSB-grid
+    minx = int(minx / int(gridsize)) * int(gridsize)
+    miny = int(miny / int(gridsize)) * int(gridsize)
+
+    cols = list(np.arange(minx, maxx + gridsize, gridsize))
+    rows = list(np.arange(miny, maxy + gridsize, gridsize))
+
+    polygons = []
+    for x in cols[:-1]:
+        for y in rows[:-1]:
+            polygons.append(
+                Polygon(
+                    [
+                        (x, y),
+                        (x + gridsize, y),
+                        (x + gridsize, y + gridsize),
+                        (x, y + gridsize),
+                    ]
+                )
+            )
+
+    grid = gpd.GeoDataFrame({"geometry": polygons}, crs=25833)
+
+    # Make SSB-id
+    grid["ostc"] = (
+        (np.floor((grid.geometry.centroid.x + 2000000) / gridsize) * gridsize).apply(
+            int
+        )
+    ).apply(str)
+    grid["nordc"] = (
+        (np.floor((grid.geometry.centroid.y) / gridsize) * gridsize).apply(int)
+    ).apply(str)
+    grid["SSBID"] = grid["ostc"] + grid["nordc"]
+    grid = grid.drop(columns=["ostc", "nordc"])
+    return grid
+
+
+def add_grid_id(
+    gdf: GeoDataFrame, gridsize: int, out_column: str = "SSBID"
+) -> GeoDataFrame:
+    """Adds a grid ID column to a GeoDataFrame of points.
+
+    The GeoDataFrame must have 25833 as crs (UTM 33 N).
+
+    Args:
+        gdf: A GeoDataFrame.
+        gridsize: Size of the grid in meters.
+
+    Returns:
+        The input GeoDataFrame with a new grid id column.
+
+    Raises:
+        ValueError: If the GeoDataFrame does not have 25833 as crs.
+    """
+    if gdf.crs != 25833:
+        raise ValueError(
+            "Geodataframe must have crs = 25833. Use df.set_crs(25833) to set "
+            "projection or df.to_crs(25833) for transforming."
+        )
+    midlrdf = gdf.copy()
+    midlrdf["ostc"] = (
+        (np.floor((midlrdf.geometry.x + 2000000) / gridsize) * gridsize).apply(int)
+    ).apply(str)
+    midlrdf["nordc"] = (
+        (np.floor((midlrdf.geometry.y) / gridsize) * gridsize).apply(int)
+    ).apply(str)
+    midlrdf[out_column] = midlrdf["ostc"] + midlrdf["nordc"]
+    midlrdf = midlrdf.drop(columns=["nordc", "ostc"])
+    return midlrdf
+
+
+def bounds_to_polygon(gdf: GeoDataFrame) -> GeoDataFrame:
+    """Creates a box around the geometry in each row of a GeoDataFrame.
+
+    Args:
+        gdf: The GeoDataFrame.
+
+    Returns:
+        GeoDataFrame of box polygons with same length and index as 'gdf'.
+    """
+    bbox_each_row = [box(*arr) for arr in gdf.bounds.values]
+    return to_gdf(bbox_each_row, index=gdf.index, crs=gdf.crs)
+
+
+def bounds_to_points(gdf: GeoDataFrame) -> GeoDataFrame:
+    """Creates a 4-noded multipoint around the geometry in each row of a GeoDataFrame.
+
+    Args:
+        gdf: The GeoDataFrame.
+
+    Returns:
+        GeoDataFrame of multipoints with same length and index as 'gdf'.
+    """
+    return bounds_to_polygon(gdf).pipe(to_multipoint)
 
 
 def clean_geoms(
     gdf: GeoDataFrame | GeoSeries, ignore_index: bool = False
 ) -> GeoDataFrame | GeoSeries:
     """Fixes geometries and removes invalid, empty, NaN and None geometries.
 
@@ -210,15 +412,15 @@
 
     return GeoDataFrame(
         (Point(x, y) for x, y in zip(x, y, strict=True)), columns=["geometry"]
     )
 
 
 def random_points_in_polygons(
-    gdf: GeoDataFrame, n: int, ignore_index=False
+    gdf: GeoDataFrame | GeoSeries, n: int, ignore_index=False
 ) -> GeoDataFrame:
     """Creates n random points inside each polygon of a GeoDataFrame.
 
     Args:
         gdf: GeoDataFrame to use as mask for the points.
         n: Number of points to create per polygon in 'gdf'.
         ignore_index: If True, the resulting axis will be labeled 0, 1, …, n - 1.
@@ -263,14 +465,16 @@
     98  POINT (-0.39865 0.87135)
     98   POINT (0.03573 0.50788)
     99  POINT (-0.79089 0.57835)
     99   POINT (0.39838 1.50881)
     99   POINT (0.98383 0.77298)
     [300 rows x 1 columns]
     """
+    if not isinstance(gdf, GeoDataFrame):
+        gdf = to_gdf(gdf)
 
     if not all(gdf.geom_type.isin(["Polygon", "MultiPolygon"])):
         raise ValueError("Geometry types must be polygon.")
 
     if gdf.index.is_unique:
         gdf["temp_idx____"] = gdf.index
     else:
@@ -302,15 +506,19 @@
 
             overlapping_indices = overlapping_indices + tuple(overlapping.index.values)
 
             gdf__ = gdf.loc[~gdf["temp_idx____"].isin(overlapping_indices)]
             temp_idx____ = gdf__["temp_idx____"].values
             bounds = gdf__.bounds
 
-    all_points = all_points.sort_index().drop(["temp_idx____", "index_right"], axis=1)
+    all_points = all_points.sort_index()
+
+    all_points = all_points.loc[
+        :, ~all_points.columns.str.contains("temp_idx____|index_right")
+    ]
 
     if gdf.index.is_unique:
         gdf = gdf.drop("temp_idx____", axis=1)
         return all_points
 
     original_index = {
         temp_idx: idx for temp_idx, idx in zip(gdf.temp_idx____, gdf.index)
@@ -320,15 +528,15 @@
     all_points.index.name = None
 
     gdf = gdf.drop("temp_idx____", axis=1)
 
     return all_points
 
 
-def points_in_bounds(gdf: GeoDataFrame, n2: int):
+def points_in_bounds(gdf: GeoDataFrame | GeoSeries, n2: int):
     minx, miny, maxx, maxy = gdf.total_bounds
     xs = np.linspace(minx, maxx, num=n2)
     ys = np.linspace(miny, maxy, num=n2)
     x_coords, y_coords = np.meshgrid(xs, ys, indexing="ij")
     coords = np.concatenate((x_coords.reshape(-1, 1), y_coords.reshape(-1, 1)), axis=1)
     return to_gdf(coords, crs=gdf.crs)
 
@@ -417,14 +625,16 @@
         if copy:
             gdf = gdf.copy()
 
         gdf[gdf._geometry_column_name] = gdf[gdf._geometry_column_name].map(
             _shapely_geometry_to_lines
         )
 
+        gdf = to_single_geom_type(gdf, "line")
+
         lines.append(gdf)
 
     if len(lines) == 1:
         return lines[0]
 
     unioned = lines[0].overlay(lines[1], how="union", keep_geom_type=True)
 
@@ -432,30 +642,27 @@
         for line_gdf in lines[2:]:
             unioned = unioned.overlay(line_gdf, how="union", keep_geom_type=True)
 
     return unioned.explode(ignore_index=True)
 
 
 def to_multipoint(
-    gdf: GeoDataFrame | GeoSeries | Geometry, copy: bool = True
-) -> GeoDataFrame | GeoSeries | Geometry:
-    """Creates a multipoint geometry of any geometry object.
+    gdf: GeoDataFrame | GeoSeries, copy: bool = True
+) -> GeoDataFrame | GeoSeries:
+    """Creates multipoint geometries from GeoDataFrame or GeoSeries.
 
-    Takes a GeoDataFrame, GeoSeries or Shapely geometry and turns it into a MultiPoint.
-    If the input is a GeoDataFrame or GeoSeries, the rows and columns will be preserved,
-    but with a geometry column of MultiPoints.
+    Takes a GeoDataFrame or GeoSeries and turns it into a MultiPoint.
 
     Args:
-        gdf: The geometry to be converted to MultiPoint. Can be a GeoDataFrame,
-            GeoSeries or a shapely geometry.
+        gdf: The geometry to be converted to MultiPoint.
         copy: If True, the geometry will be copied. Defaults to True.
 
     Returns:
-        A GeoDataFrame with the geometry column as a MultiPoint, or Point if the
-        original geometry was a point.
+        A GeoDataFrame or GeoSeries with MultiPoint geometries. If the input type
+        if GeoDataFrame, the other columns will be preserved.
 
     Examples
     --------
     Let's create a GeoDataFrame with a point, a line and a polygon.
 
     >>> from sgis import to_multipoint, to_gdf
     >>> from shapely.geometry import LineString, Polygon
@@ -472,20 +679,18 @@
 
     >>> to_multipoint(gdf)
                                                 geometry
     0                            POINT (0.00000 0.00000)
     1      MULTIPOINT (1.00000 1.00000, 2.00000 2.00000)
     2  MULTIPOINT (3.00000 3.00000, 3.00000 4.00000, ...
     """
-    if copy and not isinstance(gdf, Geometry):
+    if copy:
         gdf = gdf.copy()
 
-    if isinstance(gdf, (GeoDataFrame, GeoSeries)) and gdf.is_empty.any():
-        raise ValueError("Cannot create multipoints from empty geometry.")
-    if isinstance(gdf, Geometry) and gdf.is_empty:
+    if gdf.is_empty.any():
         raise ValueError("Cannot create multipoints from empty geometry.")
 
     def _to_multipoint(gdf):
         koordinater = "".join(
             [x for x in gdf.wkt if x.isdigit() or x.isspace() or x == "." or x == ","]
         ).strip()
 
@@ -503,16 +708,18 @@
         )
 
     elif isinstance(gdf, gpd.GeoSeries):
         gdf = force_2d(gdf)
         gdf = gdf.apply(lambda x: _to_multipoint(x))
 
     else:
-        gdf = force_2d(gdf)
-        gdf = _to_multipoint(unary_union(gdf))
+        gdf = to_gdf(gdf)
+        gdf["geometry"] = (
+            gdf["geometry"].pipe(force_2d).apply(lambda x: _to_multipoint(x))
+        )
 
     return gdf
 
 
 def clean_clip(
     gdf: GeoDataFrame | GeoSeries,
     mask: GeoDataFrame | GeoSeries | Geometry,
@@ -540,305 +747,7 @@
 
     try:
         return gdf.clip(mask, **kwargs).pipe(clean_geoms)
     except Exception:
         gdf = clean_geoms(gdf)
         mask = clean_geoms(mask)
         return gdf.clip(mask, **kwargs).pipe(clean_geoms)
-
-
-def to_gdf(
-    geom: Geometry
-    | str
-    | bytes
-    | list
-    | tuple
-    | dict
-    | GeoSeries
-    | pd.Series
-    | pd.DataFrame
-    | Iterator,
-    crs: str | tuple[str] | None = None,
-    geometry: str | None = None,
-    **kwargs,
-) -> GeoDataFrame:
-    """Converts geometry-like objects to a GeoDataFrame.
-
-    Constructs a GeoDataFrame from any geometry-like object, or an interable of such.
-    Accepted types are string (wkt), byte (wkb), coordinate tuples, shapely geometries,
-    GeoSeries, Series/DataFrame. The index/keys will be preserved if the input type is
-    Series, DataFrame or dictionary.
-
-    Args:
-        geom: the object to be converted to a GeoDataFrame
-        crs: if None (default), it uses the crs of the GeoSeries if GeoSeries
-            is the input type. Otherwise, no crs is used.
-        geometry: name of column(s) containing the geometry-like values. Can be
-            ['x', 'y', 'z'] if coordinate columns, or e.g. 'geometry' if one column.
-            The resulting geometry column will always be named 'geometry'.
-        **kwargs: additional keyword arguments taken by the GeoDataFrame constructor.
-
-    Returns:
-        A GeoDataFrame with one column, the geometry column.
-
-    Raises:
-        TypeError: If geom is a GeoDataFrame.
-
-    Examples
-    --------
-    >>> from sgis import to_gdf
-    >>> coords = (10, 60)
-    >>> to_gdf(coords, crs=4326)
-                        geometry
-    0  POINT (10.00000 60.00000)
-
-    From wkt.
-
-    >>> wkt = "POINT (10 60)"
-    >>> to_gdf(wkt, crs=4326)
-                        geometry
-    0  POINT (10.00000 60.00000)
-
-    From DataFrame with x, y (optionally z) coordinate columns. Index and
-    columns are preserved.
-
-    >>> df = pd.DataFrame({"x": [10, 11], "y": [60, 59]}, index=[1,3])
-        x   y
-    1  10  60
-    3  11  59
-    >>> gdf = to_gdf(df, geometry=["x", "y"], crs=4326)
-    >>> gdf
-        x   y                   geometry
-    1  10  60  POINT (10.00000 60.00000)
-    3  11  59  POINT (11.00000 59.00000)
-
-    For DataFrame/dict with a geometry-like column, the geometry column can be
-    speficied with the geometry parameter, which is set to "geometry" by default.
-
-    >>> df = pd.DataFrame({"col": [1, 2], "geometry": ["point (10 60)", (11, 59)]})
-    >>> df
-       col       geometry
-    0    1  point (10 60)
-    1    2       (11, 59)
-    >>> gdf = to_gdf(df, crs=4326)
-    >>> gdf
-       col                   geometry
-    0    1  POINT (10.00000 60.00000)
-    1    2  POINT (11.00000 59.00000)
-
-    From Series or Series-like dictionary.
-
-    >>> d = {1: (10, 60), 3: (11, 59)}
-    >>> to_gdf(d)
-                        geometry
-    1  POINT (10.00000 60.00000)
-    3  POINT (11.00000 59.00000)
-
-    >>> from pandas import Series
-    >>> to_gdf(Series(d))
-                        geometry
-    1  POINT (10.00000 60.00000)
-    3  POINT (11.00000 59.00000)
-
-    Multiple coordinates will be converted to points, unless a line or polygon geometry
-    is constructed beforehand.
-
-    >>> coordslist = [(10, 60), (11, 59)]
-    >>> to_gdf(coordslist, crs=4326)
-                        geometry
-    0  POINT (10.00000 60.00000)
-    1  POINT (11.00000 59.00000)
-
-    >>> from shapely.geometry import LineString
-    >>> to_gdf(LineString(coordslist), crs=4326)
-                                                geometry
-    0  LINESTRING (10.00000 60.00000, 11.00000 59.00000)
-
-    From 2 or 3 dimensional array.
-
-    >>> arr = np.random.randint(100, size=(5, 3))
-    >>> to_gdf(arr)
-                             geometry
-    0  POINT Z (82.000 88.000 82.000)
-    1  POINT Z (70.000 92.000 20.000)
-    2   POINT Z (91.000 34.000 3.000)
-    3   POINT Z (1.000 50.000 77.000)
-    4  POINT Z (58.000 49.000 46.000)
-    """
-    if isinstance(geom, GeoDataFrame):
-        raise TypeError("'to_gdf' doesn't accept GeoDataFrames as input type.")
-
-    if isinstance(geom, GeoSeries):
-        if not crs:
-            crs = geom.crs
-        else:
-            geom = geom.to_crs(crs) if geom.crs else geom.set_crs(crs)
-
-        return GeoDataFrame({"geometry": geom}, geometry="geometry", crs=crs, **kwargs)
-
-    # first the iterators that get consumed by 'all' statements
-    if isinstance(geom, Iterator) and not isinstance(geom, Sized):
-        geom = GeoSeries(_make_shapely_geom(x) for x in geom)
-        return GeoDataFrame({"geometry": geom}, geometry="geometry", crs=crs, **kwargs)
-
-    # dataframes and dicts with geometry/xyz key(s)
-    geometry = "geometry" if not geometry else geometry
-    if _is_df_like(geom, geometry):
-        geom = geom.copy()
-        geom = _make_geomcol_df_like(geom, geometry, index=kwargs.get("index"))
-        if "geometry" in geom:
-            return GeoDataFrame(geom, geometry="geometry", crs=crs, **kwargs)
-        elif isinstance(geom, pd.DataFrame):
-            raise ValueError(f"Cannot find 'geometry' column {geometry!r}")
-
-    if is_dict_like(geom):
-        if isinstance(geom, dict):
-            geom = pd.Series(geom)
-        if "index" not in kwargs:
-            index_ = geom.index
-        else:
-            index_ = None
-        geom = GeoSeries(_make_shapely_geom(x) for x in geom)
-        gdf = GeoDataFrame({"geometry": geom}, geometry="geometry", crs=crs, **kwargs)
-        if index_ is not None:
-            gdf.index = index_
-        return gdf
-
-    # single geometry objects like wkt, wkb, shapely geometry or iterable of numbers
-    if _is_one_geometry(geom):
-        geom = GeoSeries(_make_shapely_geom(geom))
-        return GeoDataFrame({"geometry": geom}, geometry="geometry", crs=crs, **kwargs)
-
-        # single geometry objects like wkt, wkb, shapely geometry or iterable of numbers
-    if hasattr(geom, "__iter__"):
-        geom = GeoSeries(_make_shapely_geom(x) for x in geom)
-        return GeoDataFrame({"geometry": geom}, geometry="geometry", crs=crs, **kwargs)
-
-    raise TypeError(f"Got unexpected type {type(geom)}")
-
-
-def _is_one_geometry(geom) -> bool:
-    if (
-        isinstance(geom, (str, bytes, Geometry))
-        or all(isinstance(i, numbers.Number) for i in geom)
-        or not hasattr(geom, "__iter__")
-    ):
-        return True
-    return False
-
-
-def _is_df_like(geom, geometry: str | None) -> bool:
-    if not is_dict_like(geom):
-        return False
-
-    if len(geometry) == 1 and geometry[0] in geom:
-        return True
-
-    if len(geometry) == 2:
-        x, y = geometry
-        if x in geom and y in geom:
-            return True
-
-    elif len(geometry) == 3:
-        x, y, z = geometry
-        if x in geom and y in geom and z in geom:
-            return True
-
-    if geometry in geom:
-        return True
-
-    if len(geom.keys()) == 1:
-        return True
-
-
-def _make_geomcol_df_like(
-    geom: pd.DataFrame | dict,
-    geometry: str | tuple[str],
-    index: list | tuple | None,
-) -> pd.DataFrame | dict:
-    """Create GeoSeries column in DataFrame or dictionary that has a DataFrame structure
-    rather than a Series structure.
-
-    Use the same logic for DataFrame and dict, as long as the speficied 'geometry'
-    value or values (if x, y, z coordinate columns) are keys in the dictionary. If
-    not, nothing happens here, and the dict goes on to be treated as a Series where
-    keys are index and values the geometries.
-    """
-
-    if not index and hasattr(geom, "index"):
-        index = geom.index
-    elif index and hasattr(geom, "index"):
-        geom.index = index
-
-    if len(geometry) == 1 and geometry[0] in geom:
-        geometry = geometry[0]
-
-    if isinstance(geometry, (tuple, list)):
-        if len(geometry) == 2:
-            x, y = geometry
-            z = None
-        elif len(geometry) == 3:
-            x, y, z = geometry
-            z = geom[z]
-        else:
-            raise ValueError(
-                "geometry should be one geometry-like column or 2-3 x, y, z columns."
-            )
-        geom["geometry"] = gpd.GeoSeries.from_xy(x=geom[x], y=geom[y], z=z)
-    elif geometry in geom:
-        if not hasattr(geom[geometry], "__iter__"):
-            geom[geometry] = [geom[geometry]]
-        geom["geometry"] = GeoSeries(
-            map(_make_shapely_geom, geom[geometry]), index=index
-        )
-
-    elif isinstance(geom, pd.DataFrame) and len(geom.columns) == 1:
-        geometry = geom.columns[0]
-        geom["geometry"] = GeoSeries(
-            map(_make_shapely_geom, geom[geometry]), index=index
-        )
-
-    elif isinstance(geom, dict) and len(geom.keys()) == 1:
-        geometry = next(iter(geom))
-        geom["geometry"] = GeoSeries(
-            map(_make_shapely_geom, geom[geometry]), index=index
-        )
-
-    return geom
-
-
-def _make_shapely_geom(geom):
-    """Create shapely geometry from wkt, wkb or coordinate tuple.
-
-    Works recursively if the object is a nested iterable.
-    """
-    if isinstance(geom, str):
-        return wkt.loads(geom)
-
-    if isinstance(geom, bytes):
-        return wkb.loads(geom)
-
-    if isinstance(geom, Geometry):
-        return geom
-
-    if not hasattr(geom, "__iter__"):
-        raise ValueError(
-            f"Couldn't create shapely geometry from {geom} of type {type(geom)}"
-        )
-
-    if isinstance(geom, GeoSeries):
-        raise TypeError(
-            "to_gdf doesn't accept iterable of GeoSeries. Instead use: "
-            "pd.concat(to_gdf(geom) for geom in geoseries_iterable)"
-        )
-
-    if not any(isinstance(g, numbers.Number) for g in geom):
-        # we're likely dealing with a nested iterable, so let's
-        # recursively dig out way down to the coords/wkt/wkb
-        return unary_union([_make_shapely_geom(g) for g in geom])
-    elif len(geom) == 2 or len(geom) == 3:
-        return Point(geom)
-    else:
-        raise ValueError(
-            "If 'geom' is an iterable, each item should consist of "
-            "wkt, wkb or 2/3 coordinates (x, y, z)."
-        )
```

### Comparing `ssb_sgis-0.1.9/src/sgis/geopandas_tools/geometry_types.py` & `ssb_sgis-0.2.0/src/sgis/geopandas_tools/geometry_types.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.9/src/sgis/geopandas_tools/neighbors.py` & `ssb_sgis-0.2.0/src/sgis/geopandas_tools/neighbors.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,49 @@
-"""Get neighbors and K-nearest neighbors."""
-import warnings
+"""Get neighbors and K-nearest neighbors.
 
+The functions rely on the pandas index as identifiers for the geometries and their
+neighbors. This makes it easy to join or aggregate the results onto the input
+GeoDataFrames.
+
+The results of all functions will be identical with GeoDataFrame and GeoSeries as input
+types.
+"""
 import numpy as np
 from geopandas import GeoDataFrame, GeoSeries
 from pandas import DataFrame, Series
 from sklearn.neighbors import NearestNeighbors
 
 from .general import coordinate_array
+from .geometry_types import get_geom_type
 
 
 def get_neighbor_indices(
     gdf: GeoDataFrame | GeoSeries,
     neighbors: GeoDataFrame | GeoSeries,
     max_distance: int = 0,
     predicate: str = "intersects",
 ) -> Series:
-    """Returns a pandas Series of neighbor indices.
-
-    The returned Series will contain values of all indices of 'neighbors' for each row
-    in 'gdf'. will be the 'neighbours' indices. The Series index will be the 'gdf'
-    indices.
+    """Creates a pandas Series with the index of 'gdf' and values of 'neighbors'.
 
     Finds all the geometries in 'neighbors' that intersect with 'gdf' and returns a
-    list of the indices of the neighbors. Use set_index on the neighbors inside the
-    function call to get values from a column instead of the current index.
+    Series where the values are the 'neighbors' indices and the index is the indices of
+    'gdf'. Use set_index inside the function call to get values from a column instead of
+    the current index.
 
     Args:
-        gdf: GeoDataFrame or GeoSeries
-        neighbors: GeoDataFrame or GeoSeries
-        max_distance: The maximum distance between the two geometries. Defaults to 0.
+        gdf: GeoDataFrame or GeoSeries.
+        neighbors: GeoDataFrame or GeoSeries.
+        max_distance: The maximum distance between the geometries. Defaults to 0.
         predicate: Spatial predicate to use in sjoin. Defaults to "intersects", meaning
             the geometry itself and geometries within will be considered neighbors if
             they are part of the 'neighbors' GeoDataFrame.
 
     Returns:
-        A pandas Series with indices of the intersecting 'neighbors'. The Series'
-        index will follow the index of the 'gdf'.
+        A pandas Series with values of the intersecting 'neighbors' indices.
+        The Series' index will follow the index of 'gdf'.
 
     Raises:
         ValueError: If gdf and neighbors do not have the same coordinate reference
             system.
 
     Examples
     --------
@@ -90,123 +94,48 @@
 
     """
 
     if gdf.crs != neighbors.crs:
         raise ValueError(f"'crs' mismatch. Got {gdf.crs} and {neighbors.crs}")
 
     # buffer and keep only geometry column
-    if max_distance:
-        if gdf.crs == 4326:
-            warnings.warn(
-                "'gdf' has latlon crs, meaning the 'max_distance' paramter "
-                "will not be in meters, but degrees."
-            )
+    if max_distance and predicate != "nearest":
         gdf = gdf.buffer(max_distance).to_frame()
     else:
         gdf = gdf.geometry.to_frame()
 
     if predicate == "nearest":
-        joined = gdf.sjoin_nearest(neighbors, how="inner").rename(
-            columns={"index_right": "neighbor_index"}, errors="raise"
-        )
+        max_distance = None if max_distance == 0 else max_distance
+        joined = gdf.sjoin_nearest(
+            neighbors, how="inner", max_distance=max_distance
+        ).rename(columns={"index_right": "neighbor_index"}, errors="raise")
     else:
         joined = gdf.sjoin(neighbors, how="inner", predicate=predicate).rename(
             columns={"index_right": "neighbor_index"}, errors="raise"
         )
 
     return joined["neighbor_index"]
 
 
-def _get_unique_neighbor_indices(
-    gdf: GeoDataFrame | GeoSeries,
-    neighbors: GeoDataFrame | GeoSeries,
-    max_distance: int = 0,
-    predicate: str = "intersects",
-) -> list:
-    """Returns a list of the indices of a GeoDataFrame's neigbours.
-
-    Finds all the geometries in 'neighbors' that intersect with 'gdf' and returns a
-    list of the indices of the neighbors. Use set_index on the neighbors inside the
-    function call to get values from a column instead of the current index.
-
-    Args:
-        gdf: GeoDataFrame or GeoSeries
-        neighbors: GeoDataFrame or GeoSeries
-        max_distance: The maximum distance between the two geometries. Defaults to 0.
-        predicate: Spatial predicate to use in sjoin. Defaults to "intersects", meaning
-            the geometry itself and geometries within will be considered neighbors if
-            they are part of the 'neighbors' GeoDataFrame.
-
-    Returns:
-        A list of the indices of the intersecting neighbors.
-
-    Raises:
-        ValueError: If gdf and neighbors do not have the same coordinate reference
-            system.
-
-    Examples
-    --------
-    >>> from sgis import get_neighbor_indices, to_gdf
-    >>> points = to_gdf([(0, 0), (0.5, 0.5), (2, 2)])
-    >>> points
-                    geometry
-    0  POINT (0.00000 0.00000)
-    1  POINT (0.50000 0.50000)
-    2  POINT (2.00000 2.00000)
-
-    >>> p1 = points.iloc[[0]]
-    >>> get_neighbor_indices(p1, points)
-    [0]
-    >>> get_neighbor_indices(p1, points, max_distance=1)
-    [0, 1]
-    >>> get_neighbor_indices(p1, points, max_distance=3)
-    [0, 1, 2]
-
-    Using a column instead of the index.
-
-    >>> points["text"] = [*"abc"]
-    >>> get_neighbor_indices(p1, points.set_index("text"), max_distance=3)
-    ['a', 'b', 'c']
-    """
-
-    if gdf.crs != neighbors.crs:
-        raise ValueError(f"'crs' mismatch. Got {gdf.crs} and {neighbors.crs}")
-
-    id_col = "index_right"
-
-    # buffer and keep only geometry column
-    if max_distance:
-        if gdf.crs == 4326:
-            warnings.warn(
-                "'gdf' has latlon crs, meaning the 'max_distance' paramter "
-                "will not be in meters, but degrees."
-            )
-        gdf = gdf.buffer(max_distance).to_frame()
-    else:
-        gdf = gdf.geometry.to_frame()
-
-    joined = gdf.sjoin(neighbors, how="inner", predicate=predicate)
-
-    return [x for x in joined[id_col].unique()]
-
-
-def get_all_distances(gdf: GeoDataFrame, neighbors: GeoDataFrame) -> DataFrame:
+def get_all_distances(
+    gdf: GeoDataFrame | GeoSeries, neighbors: GeoDataFrame | GeoSeries
+) -> DataFrame:
     """Get distances from 'gdf' to all points in 'neighbors'.
 
-    Find the distance from each point in 'gdf' to each point in 'neighbors'. Preserves
-    the index of 'gdf' and adds column 'neighbor_index' with the indices of the
-    neighbors.
+    Find the distance from each point in 'gdf' to each point in 'neighbors'. Also
+    returns the indices of 'neighbors' (as the column 'neighbor_index') and 'gdf'
+    (as the index).
 
     Args:
-        gdf: a GeoDataFrame of points
-        neighbors: a GeoDataFrame of points
+        gdf: a GeoDataFrame of points.
+        neighbors: a GeoDataFrame of points.
 
     Returns:
-        DataFrame with distances and index values from the 'gdf'. Also includes the
-        column 'neighbor_index'.
+        DataFrame with the columns 'neighbor_index' and 'distance'. The index follows
+        the index of 'gdf'.
 
     Raises:
         ValueError: If the coordinate reference system of 'gdf' and 'neighbors' are
             not the same.
 
     Examples
     --------
@@ -293,39 +222,38 @@
         gdf=gdf,
         neighbors=neighbors,
         k=len(neighbors),
     )
 
 
 def get_k_nearest_neighbors(
-    gdf: GeoDataFrame,
-    neighbors: GeoDataFrame,
+    gdf: GeoDataFrame | GeoSeries,
+    neighbors: GeoDataFrame | GeoSeries,
     k: int,
     *,
     strict: bool = False,
 ) -> DataFrame:
     """Finds the k nearest neighbors for a GeoDataFrame of points.
 
     Uses the K-nearest neighbors algorithm method from scikit-learn to find the given
     number of neighbors for each point in 'gdf'. Identical points are considered
-    neighbors. Preserves the index of 'gdf' and adds 'neighbor_index' with the indices
-    of the neighbors.
+    neighbors. Preserves the index of 'gdf' and adds the column 'neighbor_index'
+    with the indices of the neighbors, as well as a column 'distance'.
 
     Args:
         gdf: a GeoDataFrame of points
         neighbors: a GeoDataFrame of points
         k: number of neighbors to find.
         strict: If False (default), no exception is raised if k is larger than the
             number of points in 'neighbors'. If True, 'k' must be less than or equal
             to the number of points in 'neighbors'.
 
     Returns:
-        A DataFrame with the distance from gdf to the k nearest neighbours. The
-        index follows the index of 'gdf' and a column 'neighbor_index' is added
-        as identifier for the 'neighbors'.
+        DataFrame with the columns 'neighbor_index' and 'distance'. The index follows
+        the index of 'gdf'.
 
     Raises:
         ValueError: If the coordinate reference system of 'gdf' and 'neighbors' are
             not the same.
 
     Examples
     --------
@@ -370,16 +298,16 @@
     99              e  0.157481
     99              d  0.177368
     99              d  0.184087
     99              b  0.202216
 
     [1000 rows x 2 columns]
 
-    The index from 'points' is preserved. Use join to get the distance and neighbor ids
-    onto the 'points' GeoDataFrame.
+    The index from 'points' is preserved. Use join to get the distance and neighbor
+    index onto the 'points' GeoDataFrame.
 
     >>> joined = points.join(distances)
     >>> joined["k"] = joined.groupby(level=0)["distance"].transform("rank")
     >>> joined
                        geometry neighbor_index  distance     k
     0   POINT (0.89067 0.75346)              e  0.049168   1.0
     0   POINT (0.89067 0.75346)              c  0.053592   2.0
@@ -414,14 +342,17 @@
     99  POINT (0.65910 0.16714)       0.143257      0.058453
 
     [100 rows x 3 columns]
     """
     if gdf.crs != neighbors.crs:
         raise ValueError("crs mismatch:", gdf.crs, "and", neighbors.crs)
 
+    if get_geom_type(gdf) != "point" or get_geom_type(neighbors) != "point":
+        raise ValueError("Geometries must be points.")
+
     # using the range index
     idx_dict_gdf = {i: col for i, col in zip(range(len(gdf)), gdf.index, strict=True)}
     id_dict_neighbors = {
         i: col for i, col in zip(range(len(neighbors)), neighbors.index, strict=True)
     }
 
     gdf_array = coordinate_array(gdf)
@@ -461,15 +392,17 @@
         k = k if len(to_array) >= k else len(to_array)
 
     nbr = NearestNeighbors(n_neighbors=k, algorithm="ball_tree").fit(to_array)
     dists, indices = nbr.kneighbors(from_array)
     return dists, indices
 
 
-def _get_edges(gdf: GeoDataFrame, indices: np.ndarray[int]) -> np.ndarray[tuple[int]]:
+def _get_edges(
+    gdf: GeoDataFrame | GeoSeries, indices: np.ndarray[int]
+) -> np.ndarray[tuple[int]]:
     """Takes a GeoDataFrame and array of indices, and returns a 2d array of edges.
 
     Args:
         gdf (GeoDataFrame): GeoDataFrame
         indices (np.ndarray[float]): a numpy array of the indices of the nearest
             neighbors for each point in the GeoDataFrame.
```

### Comparing `ssb_sgis-0.1.9/src/sgis/geopandas_tools/overlay.py` & `ssb_sgis-0.2.0/src/sgis/geopandas_tools/overlay.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,136 +1,26 @@
-"""Overlay function that avoids a nasty GEOSException from geopandas.overlay.
+"""Overlay function that avoids a GEOSException from geopandas.overlay.
 
-This module includes the function 'clean_shapely_overlay', which bypasses a
+This module includes the function 'clean_overlay', which bypasses a
 GEOSException from the regular geopandas.overlay. The function is a generalized
-version of the solution from GH 2792. The module also includes the 'overlay' function,
-which first tries a geopandas.overlay, and if it raises a GEOSException, tries
-'clean_shapely_overlay'.
-
-Both 'overlay' and 'clean_shapely_overlay' also include the overlay type "update",
-which can be specified in the "how" parameter, in addition to the five native geopandas
-how-s.
+version of the solution from GH 2792.
+
+'clean_overlay' also includes the overlay type "update", which can be specified in the
+"how" parameter, in addition to the five native geopandas how-s.
 """
 
 import geopandas as gpd
 import numpy as np
 import pandas as pd
 from geopandas import GeoDataFrame
-from shapely import GEOSException, STRtree, difference, intersection, union_all
+from pyproj import CRS
+from shapely import STRtree, difference, intersection, union_all
 
 from .general import _push_geom_col, clean_geoms
-from .geometry_types import get_geom_type, is_single_geom_type, to_single_geom_type
-
-
-def overlay(
-    df1: GeoDataFrame,
-    df2: GeoDataFrame,
-    how: str = "intersection",
-    keep_geom_type: bool = True,
-    geom_type: str | tuple[str, str] | None = None,
-    **kwargs,
-) -> GeoDataFrame:
-    """Overlay that bypasses a GEOSException raised by geopandas.overlay.
-
-    First fixes geometries and tries a regular geopandas.overlay. If it is
-    unsuccessful, tries a solution from GH 2792. This solution bypasses a
-    GEOSExceptions raised in the regular geopandas.overlay.
-
-    Like in geopandas, the default is to keep only the geometry type of df1. If
-    either 'df1' or 'df2' has mixed geometries, it will raise an
-    Exception if not 'geom_type' is specified. 'geom_type' can be a string or a tuple
-    of two strings for the geometry type of the left and right GeoDataFrame
-    respectfully.
-
-    Args:
-        df1: GeoDataFrame
-        df2: GeoDataFrame
-        how: Method of spatial overlay. Includes the 'update' method, plus the five
-            native geopandas methods 'intersection', 'union', 'identity',
-            'symmetric_difference' and 'difference'.
-        keep_geom_type: If True (default), return only geometries of the same
-            geometry type as df1 has, if False, return all resulting geometries.
-        geom_type: optionally specify what geometry type to keep before the overlay,
-            if there may be mixed geometry types. Either a string with one geom_type
-            or a tuple/list with geom_type for df1 and df2 respectfully.
-        **kwargs: Additional keyword arguments passed to geopandas.overlay
-
-    Returns:
-        GeoDataFrame with overlayed and fixed geometries and columns from both
-        GeoDataFrames.
-
-    Raises:
-        ValueError: If the geometries have mixed geometry types and 'geom_type' is not
-            specified.
-    """
-    # Allowed operations (includes 'update')
-    allowed_hows = [
-        "intersection",
-        "union",
-        "identity",
-        "symmetric_difference",
-        "difference",  # aka erase
-        "update",  # not in geopandas
-    ]
-    # Error Messages
-    if how not in allowed_hows:
-        raise ValueError(
-            f"'how' was {how!r} but is expected to be in {', '.join(allowed_hows)}"
-        )
-
-    if df1.crs != df2.crs:
-        raise ValueError(f"crs mismatch. Got {df1.crs} and {df2.crs}")
-
-    df1 = clean_geoms(df1)
-    df2 = clean_geoms(df2)
-
-    geom_type_left, geom_type_right = _get_geom_type_left_right(geom_type)
-
-    if geom_type_left:
-        df1 = to_single_geom_type(df1, geom_type=geom_type_left)
-    if geom_type_right:
-        df2 = to_single_geom_type(df2, geom_type=geom_type_right)
-
-    if not is_single_geom_type(df1):
-        raise ValueError(
-            "mixed geometry types in 'df1'. Specify 'geom_type' as "
-            "'polygon', 'line' or 'point'."
-        )
-    if not is_single_geom_type(df2):
-        raise ValueError(
-            "mixed geometry types in 'df2'. Specify 'geom_type' as "
-            "'polygon', 'line' or 'point'."
-        )
-
-    if keep_geom_type and not geom_type_left:
-        geom_type_left = get_geom_type(df1)
-
-    df1 = df1.loc[:, ~df1.columns.str.contains("index|level_")]
-    df2 = df2.loc[:, ~df2.columns.str.contains("index|level_")]
-
-    # determine what function to use
-    if how == "update":
-        overlayfunc = overlay_update
-    else:
-        overlayfunc = gpd.overlay
-        kwargs = kwargs | {"how": how}
-
-    try:
-        overlayed = overlayfunc(df1, df2, **kwargs)
-    except GEOSException as e:
-        if how == "update":
-            raise e
-        overlayed = clean_shapely_overlay(df1, df2, how=how)
-
-    overlayed = clean_geoms(overlayed)
-
-    if keep_geom_type:
-        overlayed = to_single_geom_type(overlayed, geom_type_left)
-
-    return overlayed.loc[:, ~overlayed.columns.str.contains("index|level_")]
+from .geometry_types import get_geom_type, to_single_geom_type
 
 
 def overlay_update(
     df1: GeoDataFrame,
     df2: GeoDataFrame,
     keep_geom_type: bool = True,
     geom_type: str | tuple[str, str] | None = None,
@@ -163,29 +53,20 @@
     df1 = clean_geoms(df1)
     if geom_type_left:
         df1 = to_single_geom_type(df1, geom_type_left)
     df2 = clean_geoms(df2)
     if geom_type_right:
         df2 = to_single_geom_type(df2, geom_type_right)
 
-    try:
-        overlayed = df1.overlay(df2, how="difference", **kwargs)
-    except GEOSException:
-        overlayed = clean_shapely_overlay(
-            df1,
-            df2,
-            how="difference",
-            keep_geom_type=keep_geom_type,
-            geom_type=geom_type,
-        )
+    overlayed = df1.overlay(df2[["geometry"]], how="difference", **kwargs)
     overlayed = overlayed.loc[:, ~overlayed.columns.str.contains("index|level_")]
     return pd.concat([overlayed, df2], ignore_index=True)
 
 
-def clean_shapely_overlay(
+def clean_overlay(
     df1: GeoDataFrame,
     df2: GeoDataFrame,
     how: str = "intersection",
     keep_geom_type: bool = True,
     geom_type: str | tuple[str, str] | None = None,
 ) -> GeoDataFrame:
     """Fixes and explodes geometries before doing a shapely overlay, then cleans up.
@@ -217,21 +98,27 @@
     # Allowed operations
     allowed_hows = [
         "intersection",
         "union",
         "identity",
         "symmetric_difference",
         "difference",  # aka erase
+        "update",
     ]
     # Error messages
     if how not in allowed_hows:
         raise ValueError(
             f"`how` was {how!r} but is expected to be in {', '.join(allowed_hows)}"
         )
 
+    if df1.crs != df2.crs:
+        raise ValueError(f"'crs' mismatch. Got {df1.crs} and {df2.crs}")
+
+    crs = df1.crs
+
     geom_type_left, geom_type_right = _get_geom_type_left_right(geom_type)
 
     if keep_geom_type and not geom_type_left:
         geom_type_left = get_geom_type(df1)
 
     df1 = clean_geoms(df1)
     df2 = clean_geoms(df2)
@@ -240,15 +127,19 @@
         df1 = to_single_geom_type(df1, geom_type_left)
     if geom_type_right:
         df2 = to_single_geom_type(df2, geom_type_right)
 
     df1 = df1.explode(ignore_index=True)
     df2 = df2.explode(ignore_index=True)
 
-    overlayed = _shapely_overlay(df1, df2, how=how).pipe(clean_geoms)
+    overlayed = (
+        _shapely_overlay(df1, df2, how=how, crs=crs)
+        .pipe(clean_geoms)
+        .pipe(_push_geom_col)
+    )
 
     if geom_type_left:
         overlayed = to_single_geom_type(overlayed, geom_type_left)
 
     return overlayed.reset_index(drop=True)
 
 
@@ -271,92 +162,111 @@
             )
     else:
         raise ValueError(
             "'geom_type' should be one or two strings for the left and right gdf"
         )
 
 
-def _shapely_overlay(df1: GeoDataFrame, df2: GeoDataFrame, how: str) -> GeoDataFrame:
+def _shapely_overlay(
+    df1: GeoDataFrame, df2: GeoDataFrame, how: str, crs: int | str | None | CRS
+) -> GeoDataFrame:
     tree = STRtree(df2.geometry.values)
     left, right = tree.query(df1.geometry.values, predicate="intersects")
 
     pairs = _get_intersects_pairs(df1, df2, left, right)
 
     if how == "intersection":
-        return _intersection(pairs)
+        overlayed = _intersection(pairs, crs=crs)
 
-    if how == "difference":
-        return _difference(pairs, df1, left)
+    elif how == "difference":
+        # don't add suffix on difference
+        return _difference(pairs, df1, left, crs=crs)
 
-    if how == "symmetric_difference":
-        return _symmetric_difference(pairs, df1, df2, left, right)
+    elif how == "symmetric_difference":
+        overlayed = _symmetric_difference(pairs, df1, df2, left, right, crs=crs)
 
-    if how == "identity":
-        return _identity(pairs, df1, left)
+    elif how == "identity":
+        overlayed = _identity(pairs, df1, df2, left, crs=crs)
 
-    if how == "union":
-        return _union(pairs, df1, df2, left, right)
+    elif how == "union":
+        overlayed = _union(pairs, df1, df2, left, right, crs=crs)
 
+    elif how == "update":
+        # don't add suffix on update
+        return _update(pairs, df1, df2, left=left, crs=crs)
 
-def _intersection(pairs: GeoDataFrame) -> GeoDataFrame:
+    overlayed = _add_suffix_left(overlayed, df1, df2)
+    return overlayed
+
+
+def _update(pairs, df1, df2, left, crs) -> GeoDataFrame:
+    overlayed = _difference(pairs, df1, left, crs=crs)
+    overlayed = overlayed.loc[:, ~overlayed.columns.str.contains("index|level_")]
+    return pd.concat([overlayed, df2], ignore_index=True)
+
+
+def _intersection(pairs, crs) -> GeoDataFrame:
     intersections = pairs.copy()
     intersections["geometry"] = intersection(
         intersections.geometry.values, intersections.geom_right.values
     )
-    intersections = intersections.drop(columns=["index_right", "geom_right"])
+    intersections = intersections.drop(["index_right", "geom_right"], axis=1)
+
+    if crs:
+        intersections = intersections.to_crs(crs)
     return intersections
 
 
-def _union(pairs, df1, df2, left, right):
+def _union(pairs, df1, df2, left, right, crs):
     merged = []
     if len(left):
-        intersections = _intersection(pairs)
+        intersections = _intersection(pairs, crs=crs)
         merged.append(intersections)
-    symmdiff = _symmetric_difference(pairs, df1, df2, left, right)
+    symmdiff = _symmetric_difference(pairs, df1, df2, left, right, crs=crs)
     merged.append(symmdiff)
-    crs = merged[0].crs
-    merged = [gdf.to_crs(crs) for gdf in merged]
+    if crs:
+        merged = [gdf.to_crs(crs) for gdf in merged]
     return pd.concat(merged, ignore_index=True).pipe(_push_geom_col)
 
 
-def _identity(pairs, df1, left):
+def _identity(pairs, df1, df2, left, crs):
     merged = []
     if len(left):
-        intersections = _intersection(pairs)
+        intersections = _intersection(pairs, crs=crs)
         merged.append(intersections)
-    diff = _difference(pairs, df1, left)
+    diff = _difference(pairs, df1, left, crs=crs)
     merged.append(diff)
-    crs = merged[0].crs
-    merged = [gdf.to_crs(crs) for gdf in merged]
+    if crs:
+        merged = [gdf.to_crs(crs) for gdf in merged]
     return pd.concat(merged, ignore_index=True).pipe(_push_geom_col)
 
 
-def _symmetric_difference(pairs, df1, df2, left, right):
+def _symmetric_difference(pairs, df1, df2, left, right, crs):
     merged = []
-    difference_left = _difference(pairs, df1, left)
+    difference_left = _difference(pairs, df1, left, crs=crs)
     merged.append(difference_left)
     if len(left):
         clip_right = _shapely_diffclip_right(pairs, df1, df2)
         merged.append(clip_right)
     diff_right = _add_from_right(df1, df2, right)
     merged.append(diff_right)
-    crs = merged[0].crs
-    merged = [gdf.to_crs(crs) for gdf in merged]
+    if crs:
+        merged = [gdf.to_crs(crs) for gdf in merged]
     return pd.concat(merged, ignore_index=True).pipe(_push_geom_col)
 
 
-def _difference(pairs, df1, left):
+def _difference(pairs, df1, left, crs):
     merged = []
     if len(left):
         clip_left = _shapely_diffclip_left(pairs, df1)
         merged.append(clip_left)
     diff_left = _add_from_left(df1, left)
     merged.append(diff_left)
-    crs = merged[0].crs
-    merged = [gdf.to_crs(crs) for gdf in merged]
+    if crs:
+        merged = [gdf.to_crs(crs) for gdf in merged]
     return pd.concat(merged, ignore_index=True).pipe(_push_geom_col)
 
 
 def _get_intersects_pairs(
     df1: GeoDataFrame, df2: GeoDataFrame, left: np.ndarray, right: np.ndarray
 ) -> GeoDataFrame:
     return pd.concat(
@@ -368,14 +278,26 @@
     ).join(
         df2.rename(columns={"geometry": "geom_right"}),
         on="index_right",
         rsuffix="_2",
     )
 
 
+def _add_suffix_left(overlayed, df1, df2):
+    """Separating this from _add_from_left, since this suffix is not needed in difference."""
+    return overlayed.rename(
+        columns={
+            c: f"{c}_1"
+            if c in df1.columns and c in df2.columns and c != "geometry"
+            else c
+            for c in overlayed.columns
+        }
+    )
+
+
 def _add_from_left(df1, left):
     return df1.take(np.setdiff1d(np.arange(len(df1)), left))
 
 
 def _add_from_right(
     df1: GeoDataFrame, df2: GeoDataFrame, right: np.ndarray
 ) -> GeoDataFrame:
```

### Comparing `ssb_sgis-0.1.9/src/sgis/geopandas_tools/point_operations.py` & `ssb_sgis-0.2.0/src/sgis/geopandas_tools/point_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 """Functions for point geometries."""
 
 import numpy as np
 import pandas as pd
 from geopandas import GeoDataFrame, GeoSeries
-from shapely import Geometry
 from shapely.ops import nearest_points, snap, unary_union
 
 from ..geopandas_tools.general import to_lines
 from ..geopandas_tools.geometry_types import get_geom_type, to_single_geom_type
 
 
 def snap_within_distance(
-    points: GeoDataFrame,
-    to: GeoDataFrame,
+    points: GeoDataFrame | GeoSeries,
+    to: GeoDataFrame | GeoSeries,
     max_distance: int | float,
     *,
     distance_col: str | None = None,
-) -> GeoDataFrame:
+) -> GeoDataFrame | GeoSeries:
     """Snaps points to nearest geometry if within given distance.
 
     It takes a GeoDataFrame of points and snaps them to the nearest geometry in a
-    second GeoDataFrame if the snap distance is less than 'max_distance'. Returns distance
-    column if specified.
+    second GeoDataFrame if the snap distance is less than 'max_distance'.
+    Adds a distance column if specified.
 
     Args:
         points: The GeoDataFrame of points to snap.
         to: The GeoDataFrame to snap to.
         max_distance: The maximum distance to snap to.
         distance_col: Name of column with the snap distance. Defaults to
             'snap_distance'. Set to None to not get any distance column. This will make
@@ -71,14 +70,24 @@
     0  POINT (0.00000 0.00000)          <NA>
     1  POINT (2.00000 2.00000)      1.414214
     >>> snap_within_distance(points, to, 3)
                     geometry snap_distance
     0  POINT (2.00000 2.00000)      2.828427
     1  POINT (2.00000 2.00000)      1.414214
     """
+
+    if isinstance(points, GeoSeries):
+        points = GeoDataFrame(points)
+        _was_geoseries = True
+    else:
+        _was_geoseries = False
+
+    if isinstance(to, GeoSeries):
+        to = GeoDataFrame(to)
+
     to = _polygons_to_lines(to)
 
     copied = points.copy()
 
     geom_col = points._geometry_column_name
     copied[geom_col] = _series_snap(
         points=copied[geom_col],
@@ -87,28 +96,30 @@
     )
 
     if distance_col:
         copied[distance_col] = copied.distance(points)
         copied[distance_col] = np.where(
             copied[distance_col] == 0, pd.NA, copied[distance_col]
         )
+    elif _was_geoseries:
+        return copied[geom_col]
 
     return copied
 
 
 def snap_all(
-    points: GeoDataFrame,
-    to: GeoDataFrame,
+    points: GeoDataFrame | GeoSeries,
+    to: GeoDataFrame | GeoSeries,
     *,
     distance_col: str | None = None,
-) -> GeoDataFrame:
+) -> GeoDataFrame | GeoSeries:
     """Snaps points to the nearest geometry.
 
     It takes a GeoDataFrame of points and snaps them to the nearest geometry in a
-    second GeoDataFrame. Returns distance column if specified.
+    second GeoDataFrame. Adds a distance column if specified.
 
     Args:
         points: The GeoDataFrame of points to snap.
         to: The GeoDataFrame to snap to.
         distance_col: Name of column with the snap distance. Defaults to None.
 
     Returns:
@@ -144,14 +155,24 @@
     Snap all points to closest geometry in 'to'.
 
     >>> snap_all(points, to)
                     geometry  snap_distance
     0  POINT (2.00000 2.00000)       2.828427
     1  POINT (2.00000 2.00000)       1.414214
     """
+
+    if isinstance(points, GeoSeries):
+        points = GeoDataFrame(points)
+        _was_geoseries = True
+    else:
+        _was_geoseries = False
+
+    if isinstance(to, GeoSeries):
+        to = GeoDataFrame(to)
+
     to = _polygons_to_lines(to)
 
     copied = points.copy()
 
     geom_col = points._geometry_column_name
     copied[geom_col] = _series_snap(
         points=copied[geom_col],
@@ -160,14 +181,16 @@
     )
 
     if distance_col:
         copied[distance_col] = copied.distance(points)
         copied[distance_col] = np.where(
             copied[distance_col] == 0, pd.NA, copied[distance_col]
         )
+    elif _was_geoseries:
+        return copied[geom_col]
 
     return copied
 
 
 def _polygons_to_lines(gdf):
     if get_geom_type(gdf) == "polygon":
         return to_lines(gdf)
@@ -177,15 +200,15 @@
         gdf_polys = to_lines(to_single_geom_type(gdf, "polygon"))
         return pd.concat([gdf_points, gdf_lines, gdf_polys])
     return gdf
 
 
 def _series_snap(
     points: GeoSeries,
-    to: GeoSeries | GeoDataFrame | Geometry,
+    to: GeoSeries | GeoDataFrame,
     max_distance: int | float | None = None,
 ) -> GeoSeries:
     def snapfunc(point, to):
         nearest = nearest_points(point, to)[1]
         if not max_distance:
             return nearest
         return snap(point, nearest, tolerance=max_distance)
```

### Comparing `ssb_sgis-0.1.9/src/sgis/helpers.py` & `ssb_sgis-0.2.0/src/sgis/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,22 @@
 
 
 def unit_is_metres(gdf: GeoDataFrame) -> bool:
     """Returns True if the crs unit is 'metre''."""
     return unit_is_meters(gdf)
 
 
+def unit_is_degrees(gdf: GeoDataFrame) -> bool:
+    """Returns True if the crs unit is 'metre''."""
+    unit = gdf.crs.axis_info[0].unit_name
+    if "degree" in unit:
+        return True
+    return False
+
+
 def get_name(var: object, n: int = 5) -> str | None:
     """Searches through the local variables down one level at a time."""
     frame = inspect.currentframe().f_back.f_back
 
     for _ in range(n):
         locals_ = frame.f_locals
```

### Comparing `ssb_sgis-0.1.9/src/sgis/maps/explore.py` & `ssb_sgis-0.2.0/src/sgis/maps/explore.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 import numpy as np
 import pandas as pd
 from geopandas import GeoDataFrame
 from shapely.geometry import LineString
 
 from ..geopandas_tools.general import clean_geoms, random_points_in_polygons
 from ..geopandas_tools.geometry_types import get_geom_type
+from ..geopandas_tools.to_geodataframe import to_gdf
+from .httpserver import run_html_server
 from .map import Map
 
 
 # the geopandas._explore raises a deprication warning. Ignoring for now.
 warnings.filterwarnings(
     action="ignore", category=matplotlib.MatplotlibDeprecationWarning
 )
@@ -60,39 +62,69 @@
 class Explore(Map):
     def __init__(
         self,
         *gdfs,
         column: str | None = None,
         popup: bool = True,
         max_zoom: int = 30,
-        show_in_browser: bool = False,
+        browser: bool = False,
         **kwargs,
     ):
+        self.browser = browser
+        if not self.browser and "show_in_browser" in kwargs:
+            self.browser = kwargs.pop("show_in_browser")
+        if not self.browser and "in_browser" in kwargs:
+            self.browser = kwargs.pop("in_browser")
+
         super().__init__(*gdfs, column=column, **kwargs)
+
         self.popup = popup
         self.max_zoom = max_zoom
-        self.show_in_browser = show_in_browser
 
         self._to_single_geom_type()
 
         if self._is_categorical:
             if len(self.gdfs) == 1:
                 self._split_categories()
         else:
             if not self._cmap:
                 self._cmap = "viridis"
             self.cmap_start = kwargs.pop("cmap_start", 0)
             self.cmap_stop = kwargs.pop("cmap_stop", 256)
 
-    def explore(self, column: str | None = None, **kwargs) -> None:
+    def explore(
+        self, column: str | None = None, center=None, size=None, **kwargs
+    ) -> None:
         if column:
             self._column = column
             self._update_column()
             kwargs.pop("column", None)
-        self.to_show = self._gdfs
+
+        if center is None:
+            self.to_show = self._gdfs
+            self._explore(**kwargs)
+            return
+
+        size = size if size else 1000
+
+        centerpoint = (
+            to_gdf(center, crs=self.crs)
+            if not isinstance(center, GeoDataFrame)
+            else center
+        )
+
+        gdfs: tuple[GeoDataFrame] = ()
+        for gdf in self._gdfs:
+            gdf = gdf.clip(centerpoint.buffer(size))
+            gdfs = gdfs + (gdf,)
+        self._gdfs = gdfs
+        self._gdf = pd.concat(gdfs, ignore_index=True)
+
+        self._get_unique_values()
+
         self._explore(**kwargs)
 
     def samplemap(
         self,
         size: int = 1000,
         column: str | None = None,
         sample_from_first: bool = True,
@@ -117,20 +149,24 @@
         if get_geom_type(sample) == "polygon":
             random_point = random_points_in_polygons(sample, 1)
 
         # if point or mixed geometries
         else:
             random_point = sample.centroid
 
+        self.center = (random_point.geometry.iloc[0].x, random_point.geometry.iloc[0].y)
+        print(f"center={self.center}, size={size}")
+
         gdfs: tuple[GeoDataFrame] = ()
         for gdf in self._gdfs:
             gdf = gdf.clip(random_point.buffer(size))
             gdfs = gdfs + (gdf,)
         self._gdfs = gdfs
         self._gdf = pd.concat(gdfs, ignore_index=True)
+        self._get_unique_values()
         self._explore(**kwargs)
 
     def clipmap(
         self,
         mask,
         column: str | None = None,
         **kwargs,
@@ -156,16 +192,16 @@
         self.kwargs = self.kwargs | kwargs
 
         if self._is_categorical:
             self._create_categorical_map()
         else:
             self._create_continous_map()
 
-        if self.show_in_browser:
-            self.map.show_in_browser()
+        if self.browser:
+            run_html_server(self.map._repr_html_())
         else:
             display(self.map)
 
     def _split_categories(self):
         new_gdfs, new_labels = [], []
         for cat in self._unique_values:
             gdf = self.gdf.loc[self.gdf[self.column] == cat]
@@ -189,15 +225,15 @@
             new_gdfs.append(gdf)
         self._gdfs = new_gdfs
         self._gdf = pd.concat(new_gdfs, ignore_index=True)
         self._nan_idx = self._gdf[self._column].isna()
 
     def _update_column(self):
         self._is_categorical = self._check_if_categorical()
-        self._fill_missings()
+        self._fillna_if_col_is_missing()
         self._gdf = pd.concat(self._gdfs, ignore_index=True)
 
     def _create_categorical_map(self):
         self._get_categorical_colors()
 
         self.map = self._explore_return(
             self._gdf,
@@ -289,15 +325,14 @@
             return tooltip
         return [col for col in gdf.columns if col not in COLS_TO_DROP]
 
     def _explore_return(
         self,
         df,
         return_: str,
-        column=None,
         color=None,
         attr=None,
         tiles="OpenStreetMap",
         tooltip=True,
         popup=False,
         highlight=True,
         width="100%",
```

### Comparing `ssb_sgis-0.1.9/src/sgis/maps/legend.py` & `ssb_sgis-0.2.0/src/sgis/maps/legend.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.9/src/sgis/maps/map.py` & `ssb_sgis-0.2.0/src/sgis/maps/map.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
         # need to get the object names of the gdfs before copying. Only getting,
         # not setting, labels. So the original gdfs don't get the label column.
         self.labels = labels
         if not self.labels:
             self._get_labels(gdfs)
 
-        self._gdfs: list[GeoDataFrame] = [gdf.copy() for gdf in gdfs]
+        self._gdfs: list[GeoDataFrame] = [gdf.reset_index(drop=True) for gdf in gdfs]
         self.kwargs = kwargs
 
         if not self.labels:
             self._set_labels()
 
         if not self._column:
             for gdf, label in zip(self._gdfs, self.labels, strict=True):
@@ -106,14 +106,17 @@
 
         self._fillna_if_col_is_missing()
 
         self._gdf = pd.concat(self._gdfs, ignore_index=True)
 
         self._nan_idx = self._gdf[self._column].isna()
 
+        self._get_unique_values()
+
+    def _get_unique_values(self):
         if not self._is_categorical:
             self._unique_values = self._get_unique_floats()
             if self._k > len(self._unique_values):
                 self._k = len(self._unique_values)
         else:
             self._unique_values = sorted(
                 list(self._gdf.loc[~self._nan_idx, self._column].unique())
@@ -134,27 +137,36 @@
 
         unique = array.reset_index(drop=True).drop_duplicates()
         as_int = self._array_to_large_int(unique)
         no_duplicates = as_int.drop_duplicates()
 
         return np.sort(np.array(unique.loc[no_duplicates.index]))
 
-    def _array_to_large_int(self, array: np.ndarray):
+    def _array_to_large_int(self, array):
         """Multiply values in float array, then convert to integer."""
+        if not isinstance(array, pd.Series):
+            array = pd.Series(array)
+
+        notna = array[array.notna()]
+        isna = array[array.isna()]
 
-        unique_multiplied = array * self._multiplier
+        unique_multiplied = (notna * self._multiplier).astype(np.int64)
 
-        return unique_multiplied.astype(np.int64)
+        return pd.concat([unique_multiplied, isna]).sort_index()
 
     def _get_multiplier(self, array: np.ndarray):
         """Find the number of zeros needed to push the max value of the array above
         +-1_000_000.
 
         Adding this as an attribute to use later in _classify_from_bins.
         """
+        if np.max(array) == 0:
+            self._multiplier: int = 1
+            return
+
         multiplier = 10
         max_ = np.max(array * multiplier)
 
         if self._max > 0:
             while max_ < 1_000_000:
                 multiplier *= 10
                 max_ = np.max(array * multiplier)
@@ -166,19 +178,23 @@
         self._multiplier: int = multiplier
 
     def _add_minmax_to_bins(self, bins: list[float | int]) -> list[float | int]:
         """If values are outside the bin range, add max and/or min values of array."""
         # make sure they are lists
         bins = [bin for bin in bins]
 
-        if min(bins) > 0 and min(self._gdf[self._column]) < min(bins):
-            bins = [min(self._gdf[self._column])] + bins
-
-        if min(bins) < 0 and min(self._gdf[self._column]) < min(bins):
-            bins = [min(self._gdf[self._column])] + bins
+        if min(bins) > 0 and min(self._gdf.loc[~self._nan_idx, self._column]) < min(
+            bins
+        ):
+            bins = [min(self._gdf.loc[~self._nan_idx, self._column])] + bins
+
+        if min(bins) < 0 and min(self._gdf.loc[~self._nan_idx, self._column]) < min(
+            bins
+        ):
+            bins = [min(self._gdf.loc[~self._nan_idx, self._column])] + bins
 
         if max(bins) > 0 and max(self._gdf[self._column]) > max(bins):
             bins = bins + [max(self._gdf[self._column])]
 
         if max(bins) < 0 and max(self._gdf[self._column]) < max(bins):
             bins = bins + [max(self._gdf[self._column])]
 
@@ -204,29 +220,31 @@
                 gdfs = gdfs + (arg,)
 
         return gdfs, column
 
     def _prepare_continous_map(self):
         """Create bins if not already done and adjust k if needed."""
 
+        default_scheme = "fisherjenks"
+
         if not hasattr(self, "scheme"):
-            self.scheme = self.kwargs.pop("scheme", "fisherjenks")
+            self.scheme = self.kwargs.pop("scheme", default_scheme)
 
         if self.scheme is None:
             return
 
         if not self.bins:
             self.bins = self._create_bins(self._gdf, self._column)
             if len(self.bins) <= self._k and len(self.bins) != len(self._unique_values):
                 warnings.warn(f"Could not create {self._k} classes.")
                 self._k = len(self.bins)
         else:
             self.bins = self._add_minmax_to_bins(self.bins)
-            if len(self._unique_values) > len(self.bins):
-                self._k = len(self.bins) - 1
+            if len(self._unique_values) <= len(self.bins):
+                self._k = len(self.bins)  # - 1
 
     def _get_labels(self, gdfs: tuple[GeoDataFrame]) -> None:
         """Putting the labels/names in a list before copying the gdfs."""
         self.labels: list[str] = []
         for i, gdf in enumerate(gdfs):
             if hasattr(gdf, "name"):
                 name = gdf.name
@@ -244,14 +262,15 @@
     def _to_common_crs_and_one_geom_col(self, gdfs: list[GeoDataFrame]):
         """Need common crs and max one geometry column."""
         crs_list = list({gdf.crs for gdf in gdfs if gdf.crs is not None})
         if crs_list:
             self.crs = crs_list[0]
         new_gdfs = []
         for gdf in gdfs:
+            gdf = gdf.reset_index(drop=True)
             gdf = drop_inactive_geometry_columns(gdf).pipe(rename_geometry_if)
             if crs_list:
                 try:
                     gdf = gdf.to_crs(self.crs)
                 except ValueError:
                     gdf = gdf.set_crs(self.crs)
             new_gdfs.append(gdf)
@@ -327,16 +346,19 @@
                 for i, category in enumerate(self._unique_values)
             }
 
         if any(self._nan_idx):
             self._gdf[self._column] = self._gdf[self._column].fillna(self.nan_label)
             self._categories_colors_dict[self.nan_label] = self.nan_color
 
+        new_gdfs = []
         for gdf in self._gdfs:
             gdf["color"] = gdf[self._column].map(self._categories_colors_dict)
+            new_gdfs.append(gdf)
+        self._gdfs = new_gdfs
 
         self._gdf["color"] = self._gdf[self._column].map(self._categories_colors_dict)
 
     def _create_bins(self, gdf: GeoDataFrame, column: str) -> np.ndarray:
         """Make bin list of length k + 1, or length of unique values.
 
         The returned bins sometimes have two almost identical
@@ -348,15 +370,15 @@
         n_classes = (
             self._k if len(self._unique_values) > self._k else len(self._unique_values)
         )
 
         if self._k == len(self._unique_values) - 1:
             n_classes = self._k - 1
 
-        if self.scheme == "fisherjenks":
+        if self.scheme == "jenks":
             bins = jenks_breaks(gdf.loc[~self._nan_idx, column], n_classes=n_classes)
         else:
             binning = classify(
                 np.asarray(gdf.loc[~self._nan_idx, column]),
                 scheme=self.scheme,
                 k=self._k,
             )
@@ -399,23 +421,30 @@
         ]
         if any(self._nan_idx):
             colors_ = colors_ + [self.nan_color]
         return np.array(colors_)
 
     def _classify_from_bins(self, gdf: GeoDataFrame, bins: np.ndarray) -> np.ndarray:
         """Place the column values into groups."""
+
+        # if equal lenght, convert to integer and check for equality
         if len(bins) == len(self._unique_values):
-            # if equal lenght, convert to integer and check for equality
+            if gdf[self._column].isna().all():
+                return np.repeat(len(bins), len(gdf))
+
             gdf["col_as_int"] = self._array_to_large_int(gdf[self._column])
             bins = self._array_to_large_int(self._unique_values)
             classified = np.searchsorted(bins, gdf["col_as_int"])
         else:
             if len(bins) == self._k + 1:
                 bins = bins[1:]
 
+            if gdf[self._column].isna().all():
+                return np.repeat(len(bins), len(gdf))
+
             classified = np.searchsorted(bins, gdf[self._column])
 
         return classified
 
     def _push_classification(self, classified: np.ndarray) -> np.ndarray:
         """Push classes downwards if gaps in classification sequence.
```

### Comparing `ssb_sgis-0.1.9/src/sgis/maps/maps.py` & `ssb_sgis-0.2.0/src/sgis/maps/maps.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,74 +1,108 @@
 """Interactive and static mapping of multiple GeoDataFrames.
 
 The main function is 'explore', which displays one of more GeoDataFrames together in an
 interactive map with layers that can be toggled on and off. The 'samplemap' and
 'clipmap' functions do the same, but displays a random and chosen area respectfully.
 
-The 'qtm' function shows a static map of one or more GeoDataFrames.
+The 'qtm' function shows a simple static map of one or more GeoDataFrames.
 """
+from numbers import Number
+
 from geopandas import GeoDataFrame, GeoSeries
 from shapely import Geometry
 
 from ..exceptions import NotInJupyterError
-from ..geopandas_tools.general import random_points_in_polygons
+from ..geopandas_tools.general import clean_clip, random_points_in_polygons, to_gdf
 from ..geopandas_tools.geometry_types import get_geom_type
 from ..helpers import make_namedict
 from .explore import Explore
 from .map import Map
 from .thematicmap import ThematicMap
 
 
-def _check_if_jupyter_is_needed(explore, show_in_browser):
-    if explore and not show_in_browser:
+def _check_if_jupyter_is_needed(explore, browser):
+    if explore and not browser:
         try:
             display
         except NameError as e:
             raise NotInJupyterError(
                 "Cannot display interactive map. Try setting "
-                "'show_in_browser' to True, or 'explore' to False."
+                "'browser' to True, or 'explore' to False."
             ) from e
 
 
+def _get_mask(kwargs: dict, crs) -> tuple[GeoDataFrame, dict | None, dict]:
+    masks = {
+        "bygdoy": (10.6976899, 59.9081695),
+        "Bygdoy": (10.6976899, 59.9081695),
+        "kongsvinger": (12.0035242, 60.1875279),
+        "Kongsvinger": (12.0035242, 60.1875279),
+        "stavanger": (5.6960601, 58.8946196),
+        "Stavanger": (5.6960601, 58.8946196),
+    }
+
+    if "size" in kwargs and kwargs["size"] is not None:
+        size = kwargs["size"]
+    else:
+        size = 1000
+
+    for key, value in kwargs.items():
+        if key in masks:
+            mask = masks[key]
+            kwargs.pop(key)
+            if isinstance(value, Number) and value > 1:
+                size = value
+            return to_gdf([mask], crs=4326).to_crs(crs).buffer(size), kwargs
+
+    return None, kwargs
+
+
 def explore(
     *gdfs: GeoDataFrame,
     column: str | None = None,
     labels: tuple[str] | None = None,
     max_zoom: int = 30,
-    show_in_browser: bool = False,
+    browser: bool = False,
+    smooth_factor: int | float = 1.5,
+    center: tuple[float, float] | None = None,
+    size: int | None = None,
     **kwargs,
 ) -> None:
     """Interactive map of GeoDataFrames with layers that can be toggled on/off.
 
     It takes all the given GeoDataFrames and displays them together in an
     interactive map with a common legend. If 'column' is not specified, each
     GeoDataFrame is given a unique color.
 
     If the column is of type string and only one GeoDataFrame is given, the unique
     values will be split into separate GeoDataFrames so that each value can be toggled
     on/off.
 
-    The coloring can be changed with the 'cmap' parameter. The default colormap is a
-    custom, strongly colored palette. If a numerical colum is given, the 'viridis'
-    palette is used.
-
     Note:
         The maximum zoom level only works on the OpenStreetMap background map.
 
     Args:
         *gdfs: one or more GeoDataFrames.
         column: The column to color the geometries by. Defaults to None, which means
             each GeoDataFrame will get a unique color.
         labels: By default, the GeoDataFrames will be labeled by their object names.
             Alternatively, labels can be specified as a tuple of strings with the same
             length as the number of gdfs.
         max_zoom: The maximum allowed level of zoom. Higher number means more zoom
             allowed. Defaults to 30, which is higher than the geopandas default.
-        show_in_browser: If False (default), the maps will be shown in Jupyter.
+        browser: If False (default), the maps will be shown in Jupyter.
             If True the maps will be opened in a browser folder.
+        smooth_factor: How much to simplify the geometries. 1 is the minimum,
+            5 is quite a lot of simplification.
+        center: Optional coordinate pair (x, y) to use as centerpoint for the map.
+            The geometries will then be clipped by a buffered circle around this point.
+            If 'size' is not given, 1000 will be used as the buffer distance.
+        size: The buffer distance. Only applies when center is specified. Defaults to
+            1000 if center is given.
         **kwargs: Keyword arguments to pass to geopandas.GeoDataFrame.explore, for
             instance 'cmap' to change the colors, 'scheme' to change how the data
             is grouped. This defaults to 'fisherjenkssampled' for numeric data.
 
     See also
     --------
     samplemap: same functionality, but shows only a random area of a given size.
@@ -86,42 +120,62 @@
 
     With additional arguments.
 
     >>> roads["meters"] = roads.length
     >>> points["meters"] = points.length
     >>> explore(roads, points, column="meters", cmap="plasma", max_zoom=60)
     """
+    mask, kwargs = _get_mask(kwargs | {"size": size}, crs=gdfs[0].crs)
+    kwargs.pop("size", None)
+    if mask is not None:
+        return clipmap(
+            *gdfs,
+            column=column,
+            mask=mask,
+            labels=labels,
+            browser=browser,
+            max_zoom=max_zoom,
+            **kwargs,
+        )
+
     m = Explore(
         *gdfs,
         column=column,
         labels=labels,
-        show_in_browser=show_in_browser,
+        browser=browser,
         max_zoom=max_zoom,
+        smooth_factor=smooth_factor,
         **kwargs,
     )
-    m.explore()
+
+    m.explore(center=center, size=size)
 
 
 def samplemap(
     *gdfs: GeoDataFrame,
     column: str | None = None,
     size: int = 1000,
     sample_from_first: bool = True,
     labels: tuple[str] | None = None,
     max_zoom: int = 30,
+    smooth_factor: int = 1.5,
     explore: bool = True,
-    show_in_browser: bool = False,
+    browser: bool = False,
     **kwargs,
 ) -> None:
     """Shows an interactive map of a random area of GeoDataFrames.
 
     It takes all the GeoDataFrames specified, takes a random sample point from the
     first, and shows all geometries within a given radius of this point. Otherwise
     works like the explore function.
 
+    To re-use the sample area, use the line that is printed in this function,
+    containing the size and centerpoint. This line can be copypasted directly
+    into the explore or clipmap functions.
+
     Note:
         The maximum zoom level only works on the OpenStreetMap background map.
 
     Args:
         *gdfs: one or more GeoDataFrames.
         column: The column to color the geometries by. Defaults to None, which means
             each GeoDataFrame will get a unique color.
@@ -130,17 +184,19 @@
         sample_from_first: If True (default), the sample point is taken form the
             first specified GeoDataFrame. If False, all GeoDataFrames are considered.
         labels: By default, the GeoDataFrames will be labeled by their object names.
             Alternatively, labels can be specified as a tuple of strings the same
             length as the number of gdfs.
         max_zoom: The maximum allowed level of zoom. Higher number means more zoom
             allowed. Defaults to 30, which is higher than the geopandas default.
+        smooth_factor: How much to simplify the geometries. 1 is the minimum,
+            5 is quite a lot of simplification.
         explore: If True (default), an interactive map will be displayed. If False,
             or not in Jupyter, a static plot will be shown.
-        show_in_browser: If False (default), the maps will be shown in Jupyter.
+        browser: If False (default), the maps will be shown in Jupyter.
             If True the maps will be opened in a browser folder.
         **kwargs: Keyword arguments to pass to geopandas.GeoDataFrame.explore, for
             instance 'cmap' to change the colors, 'scheme' to change how the data
             is grouped. This defaults to 'fisherjenkssampled' for numeric data.
 
     See also
     --------
@@ -158,29 +214,43 @@
     >>> samplemap(roads, points)
 
     Sample area with a radius of 5 kilometers.
 
     >>> samplemap(roads, points, size=5_000, column="meters")
 
     """
-    _check_if_jupyter_is_needed(explore, show_in_browser)
+    _check_if_jupyter_is_needed(explore, browser)
 
     if not size and isinstance(gdfs[-1], (float, int)):
         *gdfs, size = gdfs
 
+    mask, kwargs = _get_mask(kwargs | {"size": size}, crs=gdfs[0].crs)
+    kwargs.pop("size")
+
+    if mask is not None:
+        gdfs, column = Explore._separate_args(gdfs, column)
+        gdfs, kwargs = _prepare_clipmap(
+            *gdfs,
+            mask=mask,
+            labels=labels,
+            **kwargs,
+        )
+
     if explore:
         m = Explore(
             *gdfs,
             column=column,
             labels=labels,
-            show_in_browser=show_in_browser,
+            browser=browser,
             max_zoom=max_zoom,
+            smooth_factor=smooth_factor,
             **kwargs,
         )
         m.samplemap(size, sample_from_first=sample_from_first)
+
     else:
         m = Map(
             *gdfs,
             column=column,
             labels=labels,
             **kwargs,
         )
@@ -195,29 +265,64 @@
             sample["geometry"] = sample.buffer(1)
 
         if get_geom_type(sample) == "polygon":
             random_point = random_points_in_polygons(sample, 1)
 
         # if point or mixed geometries
         else:
-            random_point = sample.centroid.buffer
+            random_point = sample.centroid
+
+        center = (random_point.geometry.iloc[0].x, random_point.geometry.iloc[0].y)
+        print(f"center={center}, size={size}")
 
-        m._gdf = m._gdf.clip(random_point.buffer(size))
+        m._gdf = clean_clip(m._gdf, random_point.buffer(size))
 
         qtm(m._gdf, column=m.column, cmap=m._cmap, k=m.k)
 
 
+def _prepare_clipmap(*gdfs, mask, labels, **kwargs):
+    if mask is None:
+        mask, kwargs = _get_mask(kwargs, crs=gdfs[0].crs)
+        if mask is None and len(gdfs) > 1:
+            *gdfs, mask = gdfs
+        elif mask is None:
+            raise ValueError("Must speficy mask.")
+
+    # storing object names in dict here, since the names disappear after clip
+    if not labels:
+        namedict = make_namedict(gdfs)
+        kwargs["namedict"] = namedict
+
+    clipped: tuple[GeoDataFrame] = ()
+
+    if mask is not None:
+        for gdf in gdfs:
+            clipped_ = clean_clip(gdf, mask)
+            clipped = clipped + (clipped_,)
+
+    else:
+        for gdf in gdfs[:-1]:
+            clipped_ = clean_clip(gdf, gdfs[-1])
+            clipped = clipped + (clipped_,)
+
+    if not any(len(gdf) for gdf in clipped):
+        raise ValueError("None of the GeoDataFrames are within the mask extent.")
+
+    return clipped, kwargs
+
+
 def clipmap(
     *gdfs: GeoDataFrame,
     column: str | None = None,
-    mask: GeoDataFrame | GeoSeries | Geometry,
+    mask: GeoDataFrame | GeoSeries | Geometry = None,
     labels: tuple[str] | None = None,
     explore: bool = True,
     max_zoom: int = 30,
-    show_in_browser: bool = False,
+    smooth_factor: int = 1.5,
+    browser: bool = False,
     **kwargs,
 ) -> None:
     """Shows an interactive map of a of GeoDataFrames clipped to the mask extent.
 
     It takes all the GeoDataFrames specified, clips them to the extent of the mask,
     and displays the resulting geometries in an interactive map with a common legends.
     The layers can be toggled on and off.
@@ -233,62 +338,55 @@
         column: The column to color the geometries by. Defaults to None, which means
             each GeoDataFrame will get a unique color.
         labels: By default, the GeoDataFrames will be labeled by their object names.
             Alternatively, labels can be specified as a tuple of strings the same
             length as the number of gdfs.
         max_zoom: The maximum allowed level of zoom. Higher number means more zoom
             allowed. Defaults to 30, which is higher than the geopandas default.
+        smooth_factor: How much to simplify the geometries. 1 is the minimum,
+            5 is quite a lot of simplification.
         explore: If True (default), an interactive map will be displayed. If False,
             or not in Jupyter, a static plot will be shown.
-        show_in_browser: If False (default), the maps will be shown in Jupyter.
+        browser: If False (default), the maps will be shown in Jupyter.
             If True the maps will be opened in a browser folder.
         **kwargs: Keyword arguments to pass to geopandas.GeoDataFrame.explore, for
             instance 'cmap' to change the colors, 'scheme' to change how the data
             is grouped. This defaults to 'fisherjenkssampled' for numeric data.
 
     See also
     --------
     explore: same functionality, but shows the entire area of the geometries.
     samplemap: same functionality, but shows only a random area of a given size.
     """
 
-    _check_if_jupyter_is_needed(explore, show_in_browser)
+    _check_if_jupyter_is_needed(explore, browser)
 
     gdfs, column = Explore._separate_args(gdfs, column)
 
-    # storing object names in dict here, since the names disappear after clip
-    if not labels:
-        namedict = make_namedict(gdfs)
-        kwargs["namedict"] = namedict
-
-    clipped: tuple[GeoDataFrame] = ()
-
-    if mask is not None:
-        for gdf in gdfs:
-            clipped_ = gdf.clip(mask)
-            clipped = clipped + (clipped_,)
-
-    else:
-        for gdf in gdfs[:-1]:
-            clipped_ = gdf.clip(gdfs[-1])
-            clipped = clipped + (clipped_,)
+    clipped, kwargs = _prepare_clipmap(
+        *gdfs,
+        mask=mask,
+        labels=labels,
+        **kwargs,
+    )
 
-    if not any(len(gdf) for gdf in clipped):
-        raise ValueError("None of the GeoDataFrames are within the mask extent.")
+    center = kwargs.pop("center", None)
+    size = kwargs.pop("size", None)
 
     if explore:
         m = Explore(
             *clipped,
             column=column,
             labels=labels,
-            show_in_browser=show_in_browser,
+            browser=browser,
             max_zoom=max_zoom,
+            smooth_factor=smooth_factor,
             **kwargs,
         )
-        m.explore()
+        m.explore(center=center, size=size)
     else:
         m = Map(
             *gdfs,
             column=column,
             labels=labels,
             **kwargs,
         )
@@ -336,13 +434,15 @@
 
     m.title = title
 
     if k and len(m._unique_values) >= k:
         m.k = k
 
     if cmap:
-        m.cmap = cmap
+        m.change_cmap(
+            cmap, start=kwargs.pop("cmap_start", 0), stop=kwargs.pop("cmap_stop", 256)
+        )
 
     if not legend:
         m.legend = None
 
     m.plot(**kwargs)
```

### Comparing `ssb_sgis-0.1.9/src/sgis/maps/thematicmap.py` & `ssb_sgis-0.2.0/src/sgis/maps/thematicmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Creating static maps with geopandas and matplotlib."""
+"""Make static maps with geopandas and matplotlib."""
 import warnings
 
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from geopandas import GeoDataFrame
@@ -157,18 +157,19 @@
             kwargs.pop("column", None)
             kwargs["color"] = self.color
             self.legend = None
             include_legend = False
 
         elif self._is_categorical:
             kwargs = self._prepare_categorical_plot(kwargs)
-            self.legend._prepare_categorical_legend(
-                categories_colors=self._categories_colors_dict,
-                nan_label=self.nan_label,
-            )
+            if self.legend:
+                self.legend._prepare_categorical_legend(
+                    categories_colors=self._categories_colors_dict,
+                    nan_label=self.nan_label,
+                )
 
         else:
             kwargs = self._prepare_continous_plot(kwargs)
             if self.legend:
                 if not self.legend._rounding_has_been_set:
                     self.legend._rounding = self.legend._get_rounding(
                         array=self._gdf.loc[~self._nan_idx, self._column]
@@ -190,17 +191,14 @@
             return
 
         self._prepare_plot(**kwargs)
 
         if self.legend:
             self.ax = self.legend._actually_add_legend(ax=self.ax)
 
-        #        if self.legend:
-        #           self._actually_add_legend()
-
         self._gdf.plot(legend=include_legend, ax=self.ax, **kwargs)
 
     def save(self, path: str) -> None:
         """Save figure as image file.
 
         To be run after the plot method.
 
@@ -400,7 +398,15 @@
             return
         if not hasattr(self.legend, "_title_fontsize_has_been_set"):
             self.legend._title_fontsize = self._size * 1.2
         if not hasattr(self.legend, "_fontsize_has_been_set"):
             self.legend._fontsize = self._size
         if not hasattr(self.legend, "_markersize_has_been_set"):
             self.legend._markersize = self._size
+
+    def __setattr__(self, __name: str, __value) -> None:
+        if "legend_" in __name:
+            last_part = __name.split("legend_")[-1]
+            raise AttributeError(
+                f"Invalid attribute {__name!r}. Did you mean 'legend.{last_part}'?"
+            )
+        return super().__setattr__(__name, __value)
```

### Comparing `ssb_sgis-0.1.9/src/sgis/networkanalysis/_get_route.py` & `ssb_sgis-0.2.0/src/sgis/networkanalysis/_get_route.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,17 +36,15 @@
             line_ids["origin"] = ori_id
             line_ids["destination"] = des_id
             line_ids["multiplier"] = weight_df.loc[ori_id, des_id].iloc[0]
 
             resultlist.append(line_ids)
 
     summarised: pd.Series = (
-        pd.concat(resultlist, ignore_index=True)
-        .groupby("src_tgt_wt")["multiplier"]
-        .sum()
+        pd.concat(resultlist).groupby("src_tgt_wt")["multiplier"].sum()
     )
 
     roads["frequency"] = roads["src_tgt_wt"].map(summarised)
 
     roads_visited = roads.loc[roads.frequency.notna()].drop("src_tgt_wt", axis=1)
 
     return roads_visited
@@ -121,28 +119,33 @@
         warnings.warn(
             "No paths were found. Try larger search_tolerance or search_factor. "
             "Or close_network_holes() or remove_isolated()."
         )
         return pd.DataFrame(columns=["origin", "destination", weight, "geometry"])
 
     results: DataFrame = pd.concat(resultlist)
+
     assert list(results.columns) == ["origin", "destination", "k"], list(
         results.columns
     )
     lines: GeoDataFrame = _get_line_geometries(results, roads, weight)
 
     lines = lines.dissolve(
         by=["origin", "destination", "k"], aggfunc="sum", as_index=False
     )
 
     return lines[["origin", "destination", weight, "k", "geometry"]]
 
 
 def _loop_k_routes(
-    graph: Graph, ori_id: str, des_id: str, k: int, drop_middle_percent: int
+    graph: Graph,
+    ori_id: str,
+    des_id: str,
+    k: int,
+    drop_middle_percent: int,
 ) -> DataFrame:
     """Workaround for igraph's get_k_shortest_paths.
 
     igraph's get_k_shorest_paths doesn't seem to work (gives just the same path k
     times), so doing it manually. Run _get_one_route, then remove the edges in the
     middle of the route, given with drop_middle_percent, repeat k times.
     """
@@ -176,15 +179,15 @@
 
         to_be_dropped = edge_tuples[n_edges_to_keep:-n_edges_to_keep]
         graph.delete_edges(to_be_dropped)
 
     if lines:
         return pd.concat(lines)
     else:
-        return pd.DataFrame()
+        return pd.DataFrame(columns=["origin", "destination", "k"])
 
 
 def _get_line_geometries(
     line_ids: DataFrame, roads: GeoDataFrame, weight: str
 ) -> GeoDataFrame:
     road_mapper = roads.set_index(["src_tgt_wt"])[[weight, "geometry"]]
     line_ids = line_ids.join(road_mapper)
```

### Comparing `ssb_sgis-0.1.9/src/sgis/networkanalysis/_od_cost_matrix.py` & `ssb_sgis-0.2.0/src/sgis/networkanalysis/_od_cost_matrix.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.9/src/sgis/networkanalysis/_points.py` & `ssb_sgis-0.2.0/src/sgis/networkanalysis/_points.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import numpy as np
 from geopandas import GeoDataFrame
-from pandas import DataFrame
 
 from ..geopandas_tools.neighbors import get_k_nearest_neighbors
 from .networkanalysisrules import NetworkAnalysisRules
 
 
 """
 These are internal classes used in the NetworkAnalysis class. The classes used in
@@ -64,21 +63,22 @@
     def _make_edges(self, df, from_col, to_col):
         return [(f, t) for f, t in zip(df[from_col], df[to_col], strict=True)]
 
     def _get_edges_and_weights(
         self,
         nodes: GeoDataFrame,
         rules: NetworkAnalysisRules,
+        k: int,
         from_col: str,
         to_col: str,
     ):
         distances = get_k_nearest_neighbors(
             gdf=self.gdf.set_index("temp_idx"),
             neighbors=nodes.set_index("node_id"),
-            k=50,
+            k=k,
         )
 
         distances["distance_min"] = distances.groupby(level=0)["distance"].min()
 
         distances = distances.reset_index()
 
         search_factor_multiplier = 1 + rules.search_factor / 100
@@ -106,30 +106,32 @@
     ) -> None:
         super().__init__(points)
 
     def _get_edges_and_weights(
         self,
         nodes: GeoDataFrame,
         rules: NetworkAnalysisRules,
+        k: int,
         from_col="temp_idx",
         to_col="neighbor_index",
     ):
         """Note: opposite order as in Destinations."""
-        return super()._get_edges_and_weights(nodes, rules, from_col, to_col)
+        return super()._get_edges_and_weights(nodes, rules, k, from_col, to_col)
 
 
 class Destinations(Points):
     def __init__(
         self,
         points: GeoDataFrame,
     ) -> None:
         super().__init__(points)
 
     def _get_edges_and_weights(
         self,
         nodes: GeoDataFrame,
         rules: NetworkAnalysisRules,
+        k: int,
         from_col="neighbor_index",
         to_col="temp_idx",
     ):
         """Note: opposite order as in Origins."""
-        return super()._get_edges_and_weights(nodes, rules, from_col, to_col)
+        return super()._get_edges_and_weights(nodes, rules, k, from_col, to_col)
```

### Comparing `ssb_sgis-0.1.9/src/sgis/networkanalysis/_service_area.py` & `ssb_sgis-0.2.0/src/sgis/networkanalysis/_service_area.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.9/src/sgis/networkanalysis/closing_network_holes.py` & `ssb_sgis-0.2.0/src/sgis/networkanalysis/closing_network_holes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,14 @@
-"""Functions for line geometries.
-
-The module includes functions for cutting and splitting lines, cutting lines into
-pieces, filling holes in a network of lines, finding isolated network islands and
-creating unique node ids.
-
-The functions are also methods of the Network class, where some checks and
-preperation is done before each method is run, making sure the lines are correct.
-"""
+"""Functions for filling gaps in the network with straight lines."""
 
 import geopandas as gpd
 import numpy as np
 import pandas as pd
 from geopandas import GeoDataFrame
+from pandas import DataFrame
 from shapely import shortest_line
 
 from ..geopandas_tools.general import coordinate_array
 from ..geopandas_tools.neighbors import k_nearest_neighbors
 from .nodes import make_edge_wkt_cols, make_node_ids
 
 
@@ -199,15 +192,15 @@
 
 
 def _find_holes_all_lines(
     lines: GeoDataFrame,
     nodes: GeoDataFrame,
     max_distance: int | float,
     max_angle: int,
-):
+) -> GeoDataFrame | DataFrame:
     """Creates lines between deadends and closest node.
 
     Creates lines if distance is less than max_distance and angle less than max_angle.
 
     wkt: well-known text, e.g. "POINT (60 10)"
     """
     k = 50 if len(nodes) >= 50 else len(nodes)
@@ -229,15 +222,15 @@
     )
     deadends_source = no_dups.loc[no_dups.n_source == 1].rename(
         columns={"source_wkt": "wkt", "target_wkt": "wkt_other_end"}
     )
     deadends = pd.concat([deadends_source, deadends_target], ignore_index=True)
 
     if len(deadends) <= 1:
-        return []
+        return DataFrame()
 
     deadends_other_end = deadends.copy()
     deadends_other_end["geometry"] = gpd.GeoSeries.from_wkt(
         deadends_other_end["wkt_other_end"], crs=crs
     )
 
     deadends["geometry"] = gpd.GeoSeries.from_wkt(deadends["wkt"], crs=crs)
@@ -317,15 +310,17 @@
         return new_lines
 
     new_lines = make_edge_wkt_cols(new_lines)
 
     return new_lines
 
 
-def _find_holes_deadends(nodes: GeoDataFrame, max_distance: float | int):
+def _find_holes_deadends(
+    nodes: GeoDataFrame, max_distance: float | int
+) -> GeoDataFrame | DataFrame:
     """Creates lines between two deadends if between max_distance and min_dist.
 
     It takes a GeoDataFrame of nodes, chooses the deadends, and creates a straight line
     between the closest deadends if the distance is no greater than 'max_distance'.
 
     Args:
         nodes: the nodes of the network
@@ -339,15 +334,15 @@
     # deadends are nodes that appear only once
     deadends = nodes[nodes["n"] == 1]
 
     # have to reset index to be able to integrate with numpy/scikit-learn
     deadends = deadends.reset_index(drop=True)
 
     if len(deadends) <= 1:
-        return []
+        return pd.DataFrame()
 
     deadends_array = coordinate_array(deadends)
 
     dists, indices = k_nearest_neighbors(deadends_array, deadends_array, k=2)
 
     # choose the second column (the closest neighbour)
     dists = dists[:, 1]
```

### Comparing `ssb_sgis-0.1.9/src/sgis/networkanalysis/cutting_lines.py` & `ssb_sgis-0.2.0/src/sgis/networkanalysis/cutting_lines.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,21 @@
-"""Functions for line geometries.
-
-The module includes functions for cutting and splitting lines, cutting lines into
-pieces, filling holes in a network of lines, finding isolated network islands and
-creating unique node ids.
-
-The functions are also methods of the Network class, where some checks and
-preperation is done before each method is run, making sure the lines are correct.
-"""
+"""Cutting and splitting line geometries."""
 import warnings
 
 import numpy as np
 import pandas as pd
 from geopandas import GeoDataFrame
 from pandas import DataFrame, Series
 from shapely import force_2d
 from shapely.geometry import LineString, Point
 
 from ..geopandas_tools.buffer_dissolve_explode import buff
-from ..geopandas_tools.general import to_gdf
 from ..geopandas_tools.neighbors import get_k_nearest_neighbors
 from ..geopandas_tools.point_operations import snap_all, snap_within_distance
+from ..geopandas_tools.to_geodataframe import to_gdf
 from .nodes import make_edge_coords_cols
 
 
 def split_lines_by_nearest_point(
     gdf: GeoDataFrame,
     points: GeoDataFrame,
     max_distance: int | None = None,
@@ -40,15 +32,16 @@
         gdf: GeoDataFrame of lines that will be split.
         points: GeoDataFrame of points to split the lines with.
         max_distance: the maximum distance between the point and the line. Points
             further away than max_distance will not split any lines. Defaults to None.
 
     Returns:
         A GeoDataFrame with the same columns as the input lines, but with the lines
-        split at the closest point to the points.
+        split at the closest point to the points. If no lines are within 'max_distance'
+        from any points, 'gdf' is returned as it came.
 
     Raises:
         ValueError: If the crs of the input data differs.
 
     Examples
     --------
     >>> from sgis import read_parquet_url, split_lines_by_nearest_point
@@ -84,17 +77,21 @@
     if max_distance:
         snapped = snap_within_distance(points, gdf, max_distance=max_distance)
     else:
         snapped = snap_all(points, gdf)
 
     # find the lines that were snapped to (or are very close)
     snapped_buff = buff(snapped, BUFFDIST)
-    intersect = gdf.intersects(snapped_buff.unary_union)
-    relevant_lines = gdf.loc[intersect]
-    the_other_lines = gdf.loc[~intersect]
+    intersects = gdf.intersects(snapped_buff.unary_union)
+
+    relevant_lines = gdf.loc[intersects]
+    the_other_lines = gdf.loc[~intersects]
+
+    if max_distance and not len(relevant_lines):
+        return gdf
 
     # need consistent coordinate dimensions later
     # (doing it down here to not overwrite the original data)
     relevant_lines.geometry = force_2d(relevant_lines.geometry)
     snapped.geometry = force_2d(snapped.geometry)
 
     # split the lines with buffer + difference, since shaply.split usually doesn't work
@@ -113,19 +110,20 @@
 
     splitted_source = to_gdf(splitted["source_coords"], crs=gdf.crs)
     splitted_target = to_gdf(splitted["target_coords"], crs=gdf.crs)
 
     # find the nearest snapped point for each source and target of the lines
     snapped = snapped.set_index("point_coords")
     dists_source: DataFrame = get_k_nearest_neighbors(splitted_source, snapped, k=1)
-    dists_target: DataFrame = get_k_nearest_neighbors(splitted_target, snapped, k=1)
-
     dists_source = dists_source.loc[dists_source.distance <= BUFFDIST * 2]
+
+    dists_target: DataFrame = get_k_nearest_neighbors(splitted_target, snapped, k=1)
     dists_target = dists_target.loc[dists_target.distance <= BUFFDIST * 2]
 
+    # neighbor_index == point_coords (coordinate tuple)
     pointmapper_source: pd.Series = dists_source["neighbor_index"]
     pointmapper_target: pd.Series = dists_target["neighbor_index"]
 
     # now, we can finally replace the source/target coordinate with the coordinates of
     # the snapped points.
 
     # loop for each line where the source is the endpoint that was split
```

### Comparing `ssb_sgis-0.1.9/src/sgis/networkanalysis/directednetwork.py` & `ssb_sgis-0.2.0/src/sgis/networkanalysis/directednetwork.py`

 * *Files 14% similar despite different names*

```diff
@@ -54,31 +54,31 @@
     ...          ...                                                ...
     175620  0.007564  MULTILINESTRING Z ((268641.225 6651871.624 111...
     175621  0.020246  MULTILINESTRING Z ((268669.748 6651890.291 110...
     175622  0.036810  MULTILINESTRING Z ((268681.757 6651886.457 110...
     175623  0.003019  MULTILINESTRING Z ((268682.748 6651886.162 110...
     175624  0.036975  MULTILINESTRING Z ((268694.594 6651881.688 111...
     [175541 rows x 45 columns]
-
     """
+    gdf = gdf.loc[~((gdf.drivetime_fw == -1) & (gdf.drivetime_bw == -1))]
     return make_directed_network(
         gdf,
         direction_col="oneway",
         direction_vals_bft=("B", "FT", "TF"),
         minute_cols=("drivetime_fw", "drivetime_bw"),
     )
 
 
 def make_directed_network(
     gdf: GeoDataFrame,
     direction_col: str,
     direction_vals_bft: tuple[str, str, str],
     minute_cols: tuple[str, str] | str | None = None,
-    speed_col: str | None = None,
-    flat_speed: int | None = None,
+    speed_col_kmh: str | None = None,
+    flat_speed_kmh: int | None = None,
     reverse_tofrom: bool = True,
 ) -> GeoDataFrame:
     """Flips the line geometries of roads going backwards and in both directions.
 
     Args:
         gdf: GeoDataFrame of line geometries.
         direction_col: name of column specifying the direction of the line
@@ -87,42 +87,42 @@
             column. Must be in the order 'both directions', 'from', 'to'.
             E.g. ('B', 'F', 'T').
         minute_cols (optional): column or columns containing the number of minutes
             it takes to traverse the line. If one column name is given, this will
             be used for both directions. If tuple/list with two column names,
             the first column will be used as the minute column for the forward
             direction, and the second column for roads going backwards.
-        speed_col (optional): name of column with the road speed limit.
-        flat_speed (optional): Speed in kilometers per hour to use as the speed for
+        speed_col_kmh (optional): name of column with the road speed limit.
+        flat_speed_kmh (optional): Speed in kilometers per hour to use as the speed for
             all roads.
         reverse_tofrom: If the geometries of the lines going backwards
             (i.e. has the last value in 'direction_vals_bft'). Defaults to True.
 
     Returns:
         The Network class, with the network attribute updated with flipped
             geometries for lines going backwards and both directions.
-        Adds the column 'minutes' if either 'speed_col', 'minute_col' or
-            'flat_speed' is specified.
+        Adds the column 'minutes' if either 'speed_col_kmh', 'minute_col' or
+            'flat_speed_kmh' is specified.
 
     Raises:
-        ValueError: If 'flat_speed' or 'speed_col' is specified and the unit of the
-            coordinate reference system is not 'metre'
+        ValueError: If 'flat_speed_kmh' or 'speed_col_kmh' is specified and the unit of
+            the coordinate reference system is not 'metre'.
     """
-    _validate_minute_args(minute_cols, speed_col, flat_speed)
+    _validate_minute_args(minute_cols, speed_col_kmh, flat_speed_kmh)
     _validate_direction_args(gdf, direction_col, direction_vals_bft)
 
-    if (flat_speed or speed_col) and not unit_is_meters(gdf):
+    if (flat_speed_kmh or speed_col_kmh) and not unit_is_meters(gdf):
         raise ValueError(
             "The crs must have 'metre' as units when calculating minutes."
             "Change crs or calculate minutes manually."
         )
 
     b, f, t = direction_vals_bft
 
-    if minute_cols:
+    if minute_cols and minute_cols != "minutes" and minute_cols[0] != "minutes":
         gdf = gdf.drop("minutes", axis=1, errors="ignore")
 
     # select the directional and bidirectional rows.
     ft = gdf.loc[gdf[direction_col] == f]
     tf = gdf.loc[gdf[direction_col] == t]
     both_ways = gdf.loc[gdf[direction_col] == b]
     both_ways2 = both_ways.copy()
@@ -139,51 +139,46 @@
         # rename the two minute cols
         both_ways = both_ways.rename(columns={min_f: "minutes"}, errors="raise")
         both_ways2 = both_ways2.rename(columns={min_t: "minutes"}, errors="raise")
 
         ft = ft.rename(columns={min_f: "minutes"}, errors="raise")
         tf = tf.rename(columns={min_t: "minutes"}, errors="raise")
 
-        for gdf in [ft, tf, both_ways, both_ways2]:
-            if all(gdf["minutes"].fillna(0) <= 0):
-                raise ValueError("All values in minute col is NaN or less than 0.")
-
     both_ways2.geometry = reverse(both_ways2.geometry)
 
     if reverse_tofrom:
         tf.geometry = reverse(tf.geometry)
 
     gdf = pd.concat([both_ways, both_ways2, ft, tf], ignore_index=True)
 
-    gdf = gdf.drop([min_f, min_t], axis=1)
-
-    if speed_col:
-        _get_speed_from_col(gdf, speed_col)
+    if minute_cols and minute_cols != "minutes" and minute_cols[0] != "minutes":
+        gdf = gdf.drop([min_f, min_t], axis=1, errors="ignore")
 
-    if flat_speed:
-        gdf["minutes"] = gdf.length / flat_speed * 16.6666666667
+    if speed_col_kmh:
+        gdf = _get_speed_from_col(gdf, speed_col_kmh)
 
-    if "minutes" in gdf.columns:
-        gdf = gdf.loc[gdf["minutes"] >= 0]
+    if flat_speed_kmh:
+        meters_per_min = (flat_speed_kmh / 60) * 1000
+        gdf["minutes"] = gdf.length / meters_per_min
 
     return gdf
 
 
-def _validate_minute_args(minute_cols, speed_col, flat_speed):
-    if not minute_cols and not speed_col and not flat_speed:
+def _validate_minute_args(minute_cols, speed_col_kmh, flat_speed_kmh):
+    if not minute_cols and not speed_col_kmh and not flat_speed_kmh:
         warnings.warn(
             "Minute column will not be calculated when both 'minute_cols', "
-            "'speed_col' and 'flat_speed' is None",
+            "'speed_col_kmh' and 'flat_speed_kmh' is None",
             stacklevel=2,
         )
 
-    if sum([bool(minute_cols), bool(speed_col), bool(flat_speed)]) > 1:
+    if sum([bool(minute_cols), bool(speed_col_kmh), bool(flat_speed_kmh)]) > 1:
         raise ValueError(
-            "Can only calculate minutes from either 'speed_col', "
-            "'minute_cols' or 'flat_speed'."
+            "Can only calculate minutes from either 'speed_col_kmh', "
+            "'minute_cols' or 'flat_speed_kmh'."
         )
 
 
 def _validate_direction_args(gdf, direction_col, direction_vals_bft):
     if len(direction_vals_bft) != 3:
         raise ValueError(
             "'direction_vals_bft' should be tuple/list with values of directions "
@@ -204,14 +199,16 @@
         warnings.warn(
             f"The 'direction_vals_bft' should be in the order 'both ways', "
             f"'from', 'to'. Got {b, f, t}. Is this correct?",
             stacklevel=2,
         )
 
 
-def _get_speed_from_col(gdf, speed_col):
-    if len(gdf.loc[(gdf[speed_col].isna()) | (gdf[speed_col] == 0)]) > len(gdf) * 0.05:
+def _get_speed_from_col(gdf: GeoDataFrame, speed_col_kmh: str) -> GeoDataFrame:
+    if len(gdf.loc[(gdf[speed_col_kmh].isna()) | (gdf[speed_col_kmh] == 0)]):
         raise ValueError(
-            f"speed_col {speed_col!r} has a lot of missing or 0 values. Fill these "
-            "with appropriate values"
+            f"speed_col_kmh {speed_col_kmh!r} cannot have missing values or zeros"
         )
-    gdf["minutes"] = gdf.length / gdf[speed_col].astype(float) * 16.6666666667
+
+    gdf["minutes"] = gdf.length / (gdf[speed_col_kmh].astype(float) * 1000 / 60)
+
+    return gdf
```

### Comparing `ssb_sgis-0.1.9/src/sgis/networkanalysis/finding_isolated_networks.py` & `ssb_sgis-0.2.0/src/sgis/networkanalysis/finding_isolated_networks.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,9 @@
-"""Functions for line geometries.
+"""Functions for Finding network components in a GeoDataFrame of lines."""
 
-The module includes functions for cutting and splitting lines, cutting lines into
-pieces, filling holes in a network of lines, finding isolated network islands and
-creating unique node ids.
-
-The functions are also methods of the Network class, where some checks and
-preperation is done before each method is run, making sure the lines are correct.
-"""
 import networkx as nx
 from geopandas import GeoDataFrame
 
 from .nodes import make_node_ids
 
 
 def get_connected_components(gdf: GeoDataFrame) -> GeoDataFrame:
@@ -59,14 +52,18 @@
 
     largest_component = max(nx.connected_components(graph), key=len)
 
     largest_component_dict = {node_id: 1 for node_id in largest_component}
 
     gdf["connected"] = gdf.source.map(largest_component_dict).fillna(0)
 
+    gdf = gdf.drop(
+        ["source_wkt", "target_wkt", "source", "target", "n_source", "n_target"], axis=1
+    )
+
     return gdf
 
 
 def get_component_size(gdf: GeoDataFrame) -> GeoDataFrame:
     """Finds the size of each component in the network.
 
     Takes a GeoDataFrame of linea and creates the column "component_size", which
@@ -105,8 +102,12 @@
 
     componentsdict = {
         idx: len(component) for component in components for idx in component
     }
 
     gdf["component_size"] = gdf.source.map(componentsdict)
 
+    gdf = gdf.drop(
+        ["source_wkt", "target_wkt", "source", "target", "n_source", "n_target"], axis=1
+    )
+
     return gdf
```

### Comparing `ssb_sgis-0.1.9/src/sgis/networkanalysis/network.py` & `ssb_sgis-0.2.0/src/sgis/networkanalysis/network.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,41 +17,27 @@
 from ..geopandas_tools.geometry_types import to_single_geom_type
 from .nodes import make_node_ids
 
 
 class Network:
     """Class used in NetworkAnalysis."""
 
-    def __init__(
-        self,
-        gdf: GeoDataFrame,
-        *,
-        allow_degree_units: bool = False,
-    ):
+    def __init__(self, gdf: GeoDataFrame):
         """The lines are fixed, welded together rowwise and exploded. Creates node-ids.
 
         Raises:
             TypeError: If 'gdf' is not of type GeoDataFrame.
             ZeroLinesError: If 'gdf' has zero rows.
-            ValueError: If the coordinate reference system is in degree units and
-                allow_degree_units is False.
         """
         if not isinstance(gdf, GeoDataFrame):
             raise TypeError(f"'lines' should be GeoDataFrame, got {type(gdf)}")
 
         if not len(gdf):
             raise ZeroLinesError
 
-        if not allow_degree_units and gdf.crs.axis_info[0].unit_name == "degree":
-            raise ValueError(
-                "The crs cannot have degrees as unit. Change to a projected crs with "
-                "e.g. 'metre' as unit. If you really want to use an unprojected crs, "
-                "set 'allow_degree_units' to True."
-            )
-
         self.gdf = self._prepare_network(gdf)
 
         self._make_node_ids()
 
         self._percent_bidirectional = self._check_percent_bidirectional()
 
     def _make_node_ids(self) -> None:
```

### Comparing `ssb_sgis-0.1.9/src/sgis/networkanalysis/networkanalysis.py` & `ssb_sgis-0.2.0/src/sgis/networkanalysis/networkanalysis.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """Contains the NetworkAnalysis class.
 
-The class has five methods: od_cost_matrix, get_route, get_k_routes,
+The class has five analysis methods: od_cost_matrix, get_route, get_k_routes,
 get_route_frequencies and service_area.
 """
 
 
 from copy import copy, deepcopy
 from datetime import datetime
 from time import perf_counter
 
 import igraph
 import numpy as np
 import pandas as pd
 from geopandas import GeoDataFrame
 from igraph import Graph
-from pandas import DataFrame
+from pandas import DataFrame, MultiIndex
 
 from ..geopandas_tools.general import _push_geom_col
 from ._get_route import _get_k_routes, _get_route, _get_route_frequencies
 from ._od_cost_matrix import _od_cost_matrix
 from ._points import Destinations, Origins
 from ._service_area import _service_area
 from .cutting_lines import split_lines_by_nearest_point
@@ -55,16 +55,15 @@
             analysis run will be stored in the 'log' attribute.
         detailed_log: If True, the log DataFrame will include columns for
             all arguments passed to the analysis method, plus standard deviation and
             percentiles (25th, 50th, 75th) of the weight column in the results.
             Defaults to False.
 
     Attributes:
-        network: A Network instance that holds the lines and nodes (points) of the
-            GeoDataFrame of line geometries.
+        network: A Network instance that holds the lines and nodes (points).
         rules: NetworkAnalysisRules instance.
         log: A DataFrame with information about each analysis run.
 
     Examples
     --------
     Read example data.
 
@@ -120,14 +119,15 @@
         self._update_wkts()
         self.rules._update_rules()
 
         if log:
             self.log = DataFrame()
 
         self._graph_updated_count = 0
+        self._k_nearest_points = 50
 
     def _check_if_holes_are_nan(self):
         HOLES_ARE_NAN = (
             "Network holes have been filled by straigt lines, but the rows have "
             f"NaN values in the {self.rules.weight!r} column. Either remove NaNs "
             "or fill these values with a numeric value (e.g. 0)."
         )
@@ -138,28 +138,37 @@
 
     def od_cost_matrix(
         self,
         origins: GeoDataFrame,
         destinations: GeoDataFrame,
         *,
         rowwise: bool = False,
+        destination_count: int | None = None,
+        cutoff: int | float | None = None,
         lines: bool = False,
     ) -> DataFrame | GeoDataFrame:
         """Fast calculation of many-to-many travel costs.
 
         Finds the the lowest cost (minutes, meters, etc.) from a set of origins to a
         set of destinations. The index of the origins and destinations are used as
         values for the returned columns 'origins' and 'destinations'.
 
         Args:
             origins: GeoDataFrame of points from where the trips will originate
             destinations: GeoDataFrame of points from where the trips will terminate
             rowwise: if False (default), it will calculate the cost from each
                 origins to each destination. If true, it will calculate the cost from
                 origin 1 to destination 1, origin 2 to destination 2 and so on.
+            destination_count: number of closest destinations to keep for each origin.
+                If None (default), all trips will be included. The number of
+                destinations might be higher than the destination_count if trips have
+                equal cost.
+            cutoff: the maximum cost (weight) for the trips. Defaults to None,
+                meaning all rows will be included. NaNs will also be removed if cutoff
+                is specified.
             lines: if True, returns a geometry column with straight lines between
                 origin and destination. Defaults to False.
 
         Returns:
             A DataFrame with the weight column and the columns 'origin' and
             'destination', containing the indices of the origins and destinations
             GeoDataFrames. If lines is True, also returns a geometry column with
@@ -188,29 +197,32 @@
         4   POINT (272876.200 6652889.100)
         ..                             ...
         95  POINT (270348.000 6651899.400)
         96  POINT (264845.600 6649005.800)
         97  POINT (263162.000 6650732.200)
         98  POINT (272322.700 6653729.100)
         99  POINT (265622.800 6644644.200)
+        <BLANKLINE>
         [100 rows x 1 columns]
+
         >>> destinations = points.loc[100:199, ["geometry"]]
         >>> destinations
                                    geometry
         100  POINT (265997.900 6647899.400)
         101  POINT (263835.200 6648677.700)
         102  POINT (265764.000 6644063.900)
         103  POINT (265970.700 6651258.500)
         104  POINT (264624.300 6649937.700)
         ..                              ...
         195  POINT (258175.600 6653694.300)
         196  POINT (258772.200 6652487.600)
         197  POINT (273135.300 6653198.100)
         198  POINT (270582.300 6652163.800)
         199  POINT (264980.800 6647231.300)
+        <BLANKLINE>
         [100 rows x 1 columns]
 
         Travel time from 100 to 100 points.
 
         >>> od = nwa.od_cost_matrix(origins, destinations)
         >>> od
               origin  destination    minutes
@@ -221,94 +233,102 @@
         4          0          104   5.882124
         ...      ...          ...        ...
         9995      99          195  20.488644
         9996      99          196  16.721241
         9997      99          197  19.977029
         9998      99          198  15.233163
         9999      99          199   6.439002
+        <BLANKLINE>
         [10000 rows x 3 columns]
 
-        Join the results onto the 'origins' GeoDataFrame via the index.
+        Assign aggregated values onto the origins (or destinations).
+
+        >>> origins["minutes_min"] = od.groupby("origin")["minutes"].min()
+        >>> origins["minutes_mean"] = od.groupby("origin")["minutes"].mean()
+        >>> origins["n_missing"] = len(origins) - od.groupby("origin")["minutes"].count()
+        >>> origins
+                                  geometry  minutes_min  minutes_mean  n_missing
+        0   POINT (263122.700 6651184.900)     0.966702     11.628637          0
+        1   POINT (272456.100 6653369.500)     2.754545     16.084722          0
+        2   POINT (270082.300 6653032.700)     1.768334     15.304246          0
+        3   POINT (259804.800 6650339.700)     2.776873     14.044023          0
+        4   POINT (272876.200 6652889.100)     0.541074     17.565747          0
+        ..                             ...          ...           ...        ...
+        95  POINT (270348.000 6651899.400)     1.529400     15.427027          0
+        96  POINT (264845.600 6649005.800)     1.336207     11.239592          0
+        97  POINT (263162.000 6650732.200)     1.010721     11.904372          0
+        98  POINT (272322.700 6653729.100)     3.175472     17.579399          0
+        99  POINT (265622.800 6644644.200)     1.116209     12.185800          0
+        <BLANKLINE>
+        [100 rows x 4 columns]
 
-        >>> od = od.set_index("origin")
-        >>> joined = origins.join(od)
+        Join the results onto the 'origins' via the index.
+
+        >>> joined = origins.join(od.set_index("origin"))
         >>> joined
                                   geometry  destination    minutes
         0   POINT (263122.700 6651184.900)          100   8.765621
         0   POINT (263122.700 6651184.900)          101   6.383407
         0   POINT (263122.700 6651184.900)          102  13.482324
         0   POINT (263122.700 6651184.900)          103   6.410121
         0   POINT (263122.700 6651184.900)          104   5.882124
         ..                             ...          ...        ...
         99  POINT (265622.800 6644644.200)          195  20.488644
         99  POINT (265622.800 6644644.200)          196  16.721241
         99  POINT (265622.800 6644644.200)          197  19.977029
         99  POINT (265622.800 6644644.200)          198  15.233163
         99  POINT (265622.800 6644644.200)          199   6.439002
+        <BLANKLINE>
         [10000 rows x 3 columns]
 
-        Get travel times below 10 minutes.
+        Keep only travel times of 10 minutes or less. This is the same as using the
+        cutoff parameter.
 
-        >>> less_than_10_min = od.loc[od.minutes < 10]
-        >>> joined = origins.join(less_than_10_min)
+        >>> ten_min_or_less = od.loc[od.minutes <= 10]
+        >>> joined = origins.join(ten_min_or_less.set_index("origin"))
         >>> joined
                                   geometry  destination   minutes
         0   POINT (263122.700 6651184.900)        100.0  8.765621
         0   POINT (263122.700 6651184.900)        101.0  6.383407
         0   POINT (263122.700 6651184.900)        103.0  6.410121
         0   POINT (263122.700 6651184.900)        104.0  5.882124
         0   POINT (263122.700 6651184.900)        106.0  9.811828
         ..                             ...          ...       ...
         99  POINT (265622.800 6644644.200)        173.0  4.305523
         99  POINT (265622.800 6644644.200)        174.0  6.094040
         99  POINT (265622.800 6644644.200)        177.0  5.944194
         99  POINT (265622.800 6644644.200)        183.0  8.449906
         99  POINT (265622.800 6644644.200)        199.0  6.439002
+        <BLANKLINE>
         [2195 rows x 3 columns]
 
-        Get the three fastest routes from each origin.
+        Keep the three fastest times from each origin. This is the same as using the
+        destination_count parameter.
 
         >>> three_fastest = od.loc[od.groupby("origin")["minutes"].rank() <= 3]
-        >>> joined = origins.join(three_fastest)
+        >>> joined = origins.join(three_fastest.set_index("origin"))
         >>> joined
                                   geometry  destination   minutes
         0   POINT (263122.700 6651184.900)        135.0  0.966702
         0   POINT (263122.700 6651184.900)        175.0  2.202638
         0   POINT (263122.700 6651184.900)        188.0  2.931595
         1   POINT (272456.100 6653369.500)        171.0  2.918100
         1   POINT (272456.100 6653369.500)        184.0  2.754545
         ..                             ...          ...       ...
         98  POINT (272322.700 6653729.100)        184.0  3.175472
         98  POINT (272322.700 6653729.100)        189.0  3.179428
         99  POINT (265622.800 6644644.200)        102.0  1.648705
         99  POINT (265622.800 6644644.200)        134.0  1.116209
         99  POINT (265622.800 6644644.200)        156.0  1.368926
+        <BLANKLINE>
         [294 rows x 3 columns]
 
-        Assign aggregated values directly onto the origins.
-
-        >>> origins["minutes_mean"] = od.groupby("origin")["minutes"].mean()
-        >>> origins
-                                  geometry  minutes_mean
-        0   POINT (263122.700 6651184.900)     11.628637
-        1   POINT (272456.100 6653369.500)     16.084722
-        2   POINT (270082.300 6653032.700)     15.304246
-        3   POINT (259804.800 6650339.700)     14.044023
-        4   POINT (272876.200 6652889.100)     17.565747
-        ..                             ...           ...
-        95  POINT (270348.000 6651899.400)     15.427027
-        96  POINT (264845.600 6649005.800)     11.239592
-        97  POINT (263162.000 6650732.200)     11.904372
-        98  POINT (272322.700 6653729.100)     17.579399
-        99  POINT (265622.800 6644644.200)     12.185800
-        [100 rows x 2 columns]
-
         Use set_index to use column as identifier insted of the index.
 
-        >>> origins["areacode"] = np.random.choice(["0301", "4601", "3401"], len(origins))
+        >>> origins["areacode"] = np.random.choice(["0301", "3401"], len(origins))
         >>> od = nwa.od_cost_matrix(
         ...    origins.set_index("areacode"),
         ...    destinations
         ... )
         >>> od
              origin  destination    minutes
         0      0301          100   8.765621
@@ -318,14 +338,15 @@
         4      0301          104   5.882124
         ...     ...          ...        ...
         9995   3401          195  20.488644
         9996   3401          196  16.721241
         9997   3401          197  19.977029
         9998   3401          198  15.233163
         9999   3401          199   6.439002
+        <BLANKLINE>
         [10000 rows x 3 columns]
 
         Travel time from 1000 to 1000 points rowwise.
 
         >>> points_reversed = points.iloc[::-1]
         >>> od = nwa.od_cost_matrix(points, points_reversed, rowwise=True)
         >>> od
@@ -337,14 +358,15 @@
         4         4          995  16.521346
         ..      ...          ...        ...
         995     995            4  16.794610
         996     996            3   9.611700
         997     997            2  19.968743
         998     998            1   9.484374
         999     999            0  14.892648
+        <BLANKLINE>
         [1000 rows x 3 columns]
 
         """
         if self._log:
             time_ = perf_counter()
 
         self._prepare_network_analysis(origins, destinations, rowwise)
@@ -356,14 +378,22 @@
             origins=ori,
             destinations=des,
             weight=self.rules.weight,
             lines=lines,
             rowwise=rowwise,
         )
 
+        if cutoff is not None:
+            results = results.loc[results[self.rules.weight] <= cutoff]
+
+        if destination_count:
+            results = results.loc[
+                results.groupby("origin")[self.rules.weight].rank() <= destination_count
+            ]
+
         results["origin"] = results["origin"].map(self.origins.idx_dict)
         results["destination"] = results["destination"].map(self.destinations.idx_dict)
 
         if lines:
             results = _push_geom_col(results)
 
         if self.rules.split_lines:
@@ -417,17 +447,16 @@
             with a column with the number of times the line segment was used in the
             individual routes.
 
         Note:
             The resulting lines will keep all columns of the 'gdf' of the Network.
 
         Raises:
-            ValueError: If no paths were found.
             ValueError: If weight_df is not a DataFrame with one or three columns
-                that contain all indices of 'origins' and 'destinations'.
+                that contain weights and all indices of 'origins' and 'destinations'.
 
         Examples
         --------
         Create the NetworkAnalysis instance.
 
         >>> import sgis as sg
         >>> import pandas as pd
@@ -454,14 +483,15 @@
         153677  47999  75262        1.0  LINESTRING Z (268631.500 6652176.800 118.166, ...
         ...       ...    ...        ...                                                ...
         151465  73801  73802      103.0  LINESTRING Z (265368.600 6647142.900 131.660, ...
         151464  73800  73801      103.0  LINESTRING Z (265362.800 6647137.100 131.660, ...
         151466  73802  73632      103.0  LINESTRING Z (265371.400 6647147.900 131.660, ...
         151463  73799  73800      123.0  LINESTRING Z (265359.600 6647135.400 131.660, ...
         152170  74418  74246      130.0  LINESTRING Z (264579.835 6651954.573 113.209, ...
+        <BLANKLINE>
         [8556 rows x 4 columns]
 
         The frequencies can be weighted for each origin-destination pair by specifying
         'weight_df'. This can be a DataFrame with three columns, where the first two
         contain the indices of the origin and destination (in that order), and the
         third the number to multiply the frequency by. 'weight_df' can also be a
         DataFrame with a 2-leveled MultiIndex, where level 0 is the origin index and
@@ -484,14 +514,15 @@
         4         0           29      10
         ..      ...          ...     ...
         620      24           45      10
         621      24           46      10
         622      24           47      10
         623      24           48      10
         624      24           49      10
+        <BLANKLINE>
         [625 rows x 3 columns]
 
         All frequencies will now be multiplied by 10.
 
         >>> frequencies = nwa.get_route_frequencies(origins, destinations, weight_df, weight_df=weight_df)
         >>> frequencies[["source", "target", "frequency", "geometry"]]
                source target  frequency                                           geometry
@@ -502,14 +533,15 @@
         153677  47999  75262       10.0  LINESTRING Z (268631.500 6652176.800 118.166, ...
         ...       ...    ...        ...                                                ...
         151465  73801  73802     1030.0  LINESTRING Z (265368.600 6647142.900 131.660, ...
         151464  73800  73801     1030.0  LINESTRING Z (265362.800 6647137.100 131.660, ...
         151466  73802  73632     1030.0  LINESTRING Z (265371.400 6647147.900 131.660, ...
         151463  73799  73800     1230.0  LINESTRING Z (265359.600 6647135.400 131.660, ...
         152170  74418  74246     1300.0  LINESTRING Z (264579.835 6651954.573 113.209, ...
+        <BLANKLINE>
         [8556 rows x 4 columns]
 
         'weight_df' can also be a DataFrame with one column (the weight) and a
         MultiIndex.
 
         >>> weight_df = pd.DataFrame(index=od_pairs)
         >>> weight_df["weight"] = 10
@@ -522,26 +554,34 @@
            29      10
         ...       ...
         24 45      10
            46      10
            47      10
            48      10
            49      10
-
+        <BLANKLINE>
+        [625 rows x 1 columns]
         """
         if self._log:
             time_ = perf_counter()
 
         if weight_df is not None:
-            weight_df = self._prepare_weight_df(weight_df)
-            od_pairs = self._create_od_pairs(origins, destinations, rowwise=rowwise)
+            weight_df: DataFrame = self._prepare_weight_df(weight_df)
+            od_pairs: MultiIndex = self._create_od_pairs(
+                origins, destinations, rowwise=rowwise
+            )
             self._make_sure_unique(weight_df, od_pairs)
 
             weights_mapped = od_pairs.map(weight_df.iloc[:, 0])
             if default_weight:
+                if not weight_df.index.isin(od_pairs).all():
+                    raise ValueError(
+                        "All origin-destination indices in 'weight_df' must "
+                        "be in 'origins' and 'destinations'."
+                    )
                 weights_mapped = weights_mapped.fillna(default_weight)
             else:
                 self._make_sure_index_match(weight_df, od_pairs)
             weight_df = DataFrame(index=od_pairs)
             weight_df["weight"] = weights_mapped
 
         self._prepare_network_analysis(origins, destinations, rowwise)
@@ -592,36 +632,42 @@
 
     def get_route(
         self,
         origins: GeoDataFrame,
         destinations: GeoDataFrame,
         *,
         rowwise: bool = False,
+        destination_count: int | None = None,
+        cutoff: int | float | None = None,
     ) -> GeoDataFrame:
         """Returns the geometry of the low-cost route between origins and destinations.
 
         Finds the route with the lowest cost (minutes, meters, etc.) from a set of
         origins to a set of destinations. If the weight is meters, the shortest route
         will be found. If the weight is minutes, the fastest route will be found.
 
         Args:
             origins: GeoDataFrame of points from where the routes will originate
             destinations: GeoDataFrame of points from where the routes will terminate.
             rowwise: if False (default), it will calculate the cost from each
                 origins to each destination. If true, it will calculate the cost from
                 origin 1 to destination 1, origin 2 to destination 2 and so on.
+            destination_count: number of closest destinations to keep for each origin.
+                If None (default), all trips will be included. The number of
+                destinations might be higher than the destination_count if trips have
+                equal cost.
+            cutoff: the maximum cost (weight) for the trips. Defaults to None,
+                meaning all rows will be included. NaNs will also be removed if cutoff
+                is specified.
 
         Returns:
             A DataFrame with the geometry of the routes between origin and destination.
             Also returns a weight column and the columns 'origin' and 'destination',
             containing the indices of the origins and destinations GeoDataFrames.
 
-        Raises:
-            ValueError: if no paths were found.
-
         Examples
         --------
         Create the NetworkAnalysis instance.
 
         >>> import sgis as sg
         >>> roads = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_oslo_2022.parquet")
         >>> directed_roads = sg.remove_isolated(roads).pipe(sg.make_directed_network_norway)
@@ -642,14 +688,15 @@
         4         1            6  14.406460  MULTILINESTRING Z ((257034.948 6652685.595 156...
         ..      ...          ...        ...                                                ...
         992       1          996  10.858519  MULTILINESTRING Z ((266881.100 6647824.860 132...
         993       1          997   7.461032  MULTILINESTRING Z ((262623.190 6652506.640 79....
         994       1          998  10.698588  MULTILINESTRING Z ((263489.330 6645655.330 11....
         995       1          999  10.109855  MULTILINESTRING Z ((269217.997 6650654.895 166...
         996       1         1000  14.657289  MULTILINESTRING Z ((264475.675 6644245.782 114...
+        <BLANKLINE>
         [997 rows x 4 columns]
         """
         if self._log:
             time_ = perf_counter()
 
         self._prepare_network_analysis(origins, destinations, rowwise)
 
@@ -662,14 +709,22 @@
         results = _get_route(
             graph=self.graph,
             weight=self.rules.weight,
             roads=self.network.gdf,
             od_pairs=od_pairs,
         )
 
+        if cutoff is not None:
+            results = results.loc[results[self.rules.weight] <= cutoff]
+
+        if destination_count:
+            results = results.loc[
+                results.groupby("origin")[self.rules.weight].rank() <= destination_count
+            ]
+
         results["origin"] = results["origin"].map(self.origins.idx_dict)
         results["destination"] = results["destination"].map(self.destinations.idx_dict)
 
         if self.rules.split_lines:
             self._unsplit_network()
 
         if self._log:
@@ -686,15 +741,17 @@
     def get_k_routes(
         self,
         origins: GeoDataFrame,
         destinations: GeoDataFrame,
         *,
         k: int,
         drop_middle_percent: int,
-        rowwise=False,
+        rowwise: bool = False,
+        destination_count: int | None = None,
+        cutoff: int | float | None = None,
     ) -> GeoDataFrame:
         r"""Returns the geometry of 1 or more routes between origins and destinations.
 
         Finds the route with the lowest cost (minutes, meters, etc.) from a set of
         origins to a set of destinations. Then the middle part of the route is removed
         from the graph the new low-cost path is found. Repeats k times. If k=1, it is
         identical to the get_route method.
@@ -707,14 +764,21 @@
                 that should be removed from the graph before the next k route is
                 calculated. If set to 100, only the median edge will be removed.
                 If set to 0, all but the first and last edge will be removed. The
                 graph is copied for each od pair.
             rowwise: if False (default), it will calculate the cost from each
                 origins to each destination. If true, it will calculate the cost from
                 origin 1 to destination 1, origin 2 to destination 2 and so on.
+            destination_count: number of closest destinations to keep for each origin.
+                If None (default), all trips will be included. The number of
+                destinations might be higher than the destination_count if trips have
+                equal cost.
+            cutoff: the maximum cost (weight) for the trips. Defaults to None,
+                meaning all rows will be included. NaNs will also be removed if cutoff
+                is specified.
 
         Returns:
             A DataFrame with the geometry of the k routes between origin and
             destination. Also returns the column 'k', a weight column and the columns
             'origin' and 'destination', containing the indices of the origins and
             destinations GeoDataFrames.
 
@@ -722,15 +786,14 @@
             How many percent of the route to drop from the graph, will determine how
             many k routes will be found. If 100 percent of the route is dropped, it is
             very hard to find more than one path for each OD pair.
             If 'drop_middle_percent' is 1, the resulting routes might be very similar,
             depending on the layout of the network.
 
         Raises:
-            ValueError: if no paths were found.
             ValueError: if drop_middle_percent is not between 0 and 100.
 
         Examples
         --------
         Create the NetworkAnalysis instance.
 
         >>> import sgis as sg
@@ -811,14 +874,22 @@
             weight=self.rules.weight,
             roads=self.network.gdf,
             od_pairs=od_pairs,
             k=k,
             drop_middle_percent=drop_middle_percent,
         )
 
+        if cutoff is not None:
+            results = results.loc[results[self.rules.weight] <= cutoff]
+
+        if destination_count:
+            results = results.loc[
+                results.groupby("origin")[self.rules.weight].rank() <= destination_count
+            ]
+
         results["origin"] = results["origin"].map(self.origins.idx_dict)
         results["destination"] = results["destination"].map(self.destinations.idx_dict)
 
         if isinstance(results, GeoDataFrame):
             results = _push_geom_col(results)
 
         if self.rules.split_lines:
@@ -861,15 +932,15 @@
         Returns:
             A GeoDataFrame with one row per break per origin, with the origin index and
             a dissolved line geometry. If dissolve is False, it will return each line
             that is part of the service area.
 
         See also:
             precice_service_area: Equivelent method where lines are also cut to get
-                precice results.
+            precice results.
 
         Examples
         --------
         Create the NetworkAnalysis instance.
 
         >>> import sgis as sg
         >>> roads = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_oslo_2022.parquet")
@@ -937,15 +1008,15 @@
 
             # add missing rows as NaNs
             missing = self.origins.gdf.loc[
                 ~self.origins.gdf["temp_idx"].isin(results["origin"])
             ].rename(columns={"temp_idx": "origin"})[["origin"]]
 
             if len(missing):
-                missing["geometry"] = np.nan
+                missing["geometry"] = pd.NA
                 results = pd.concat([results, missing], ignore_index=True)
 
             results["origin"] = results["origin"].map(self.origins.idx_dict)
 
             results = _push_geom_col(results)
 
         if self.rules.split_lines:
@@ -1064,15 +1135,15 @@
 
             # add missing rows as NaNs
             missing = self.origins.gdf.loc[
                 ~self.origins.gdf["temp_idx"].isin(results["origin"])
             ].rename(columns={"temp_idx": "origin"})[["origin"]]
 
             if len(missing):
-                missing["geometry"] = np.nan
+                missing["geometry"] = pd.NA
                 results = pd.concat([results, missing], ignore_index=True)
 
             results["origin"] = results["origin"].map(self.origins.idx_dict)
             results = results.drop("origin", axis=1)
 
             results = _push_geom_col(results)
 
@@ -1111,67 +1182,67 @@
             raise ValueError(error_message)
 
         weight_df = weight_df.copy()
 
         if len(weight_df.columns) == 3:
             weight_df = weight_df.set_index(list(weight_df.columns[:2]))
 
-        if len(weight_df.columns) != 1 and isinstance(weight_df.index, pd.MultiIndex):
+        if len(weight_df.columns) != 1 and isinstance(weight_df.index, MultiIndex):
             raise ValueError(error_message)
 
         return weight_df
 
     @staticmethod
-    def _make_sure_unique(weight_df: DataFrame, od_pairs: pd.MultiIndex) -> None:
-        """Make sure this index matches the index of origins and destinations."""
+    def _make_sure_unique(weight_df: DataFrame, od_pairs: MultiIndex) -> None:
+        """It's nesseccary with unique index when using weight_df."""
         if not weight_df.index.is_unique:
             raise ValueError("'weight_df' must contain only unique OD combinations.")
 
         if not od_pairs.is_unique:
             raise ValueError(
                 "'origins' and 'destinations must contain only unique "
                 "indices when weight_df is specified."
             )
 
     @staticmethod
     def _make_sure_index_match(
         weight_df: DataFrame,
-        od_pairs: pd.MultiIndex,
+        od_pairs: MultiIndex,
     ):
         """Make sure this index matches the index of origins and destinations."""
         if not od_pairs.isin(weight_df.index).all():
             if not od_pairs.isin(weight_df.index).any():
                 raise ValueError(
                     "None of the origin-destination pair indices are in 'weight_df'."
                 )
             raise ValueError(
                 "Not all origin-destination pair indices are in 'weight_df'."
             )
 
     @staticmethod
     def _create_od_pairs(
         origins: GeoDataFrame, destinations: GeoDataFrame, rowwise: bool
-    ) -> pd.MultiIndex:
+    ) -> MultiIndex:
         """Get all OD combinaions without identical origin-destination geometry.
 
         Returns a MultiIndex to be iterated over in get_route, get_k_routes and
         get_route_frequencies. In get_route_frequencies, the MultiIndex is turned
         into a DataFrame with a weight column.
         """
         if rowwise:
-            od_pairs = pd.MultiIndex.from_arrays([origins.index, destinations.index])
+            od_pairs = MultiIndex.from_arrays([origins.index, destinations.index])
         else:
-            od_pairs = pd.MultiIndex.from_product([origins.index, destinations.index])
+            od_pairs = MultiIndex.from_product([origins.index, destinations.index])
 
         geoms_ori = od_pairs.get_level_values(0).map(origins.geometry)
         geoms_des = od_pairs.get_level_values(1).map(destinations.geometry)
         no_identical_geoms = od_pairs[geoms_ori != geoms_des]
 
         if not len(no_identical_geoms) and len(origins) and len(destinations):
-            raise ValueError("All origin-destination pairs have identical geometries")
+            raise ValueError("All origin-destination pairs have identical geometries.")
 
         return no_identical_geoms
 
     def _log_df_template(self, method: str, minutes_elapsed: float) -> DataFrame:
         """Creates a DataFrame with one row and the main columns.
 
         To be run after each network analysis.
@@ -1183,18 +1254,18 @@
         Returns:
             A one-row DataFrame with log info columns
         """
         data = {
             "endtime": pd.to_datetime(datetime.now()).floor("S").to_pydatetime(),
             "minutes_elapsed": minutes_elapsed,
             "method": method,
-            "origins_count": np.nan,
-            "destinations_count": np.nan,
-            "percent_missing": np.nan,
-            "cost_mean": np.nan,
+            "origins_count": pd.NA,
+            "destinations_count": pd.NA,
+            "percent_missing": pd.NA,
+            "cost_mean": pd.NA,
         }
         if self.rules.directed:
             data["percent_bidirectional"] = self.network.percent_bidirectional
 
         df = DataFrame(data, index=[0])
 
         if not self.detailed_log:
@@ -1240,15 +1311,15 @@
                     value = [str(x) for x in value]
                     value = ", ".join(value)
                 df[key] = value
 
         self.log = pd.concat([self.log, df], ignore_index=True)
 
     def _prepare_network_analysis(
-        self, origins, destinations=None, rowwise=False
+        self, origins, destinations=None, rowwise: bool = False
     ) -> None:
         """Prepares the weight column, node ids, origins, destinations and graph.
 
         Updates the graph only if it is not yet created and no parts of the analysis
         has changed. this method is run inside od_cost_matrix, get_route and
         service_area.
         """
@@ -1318,26 +1389,28 @@
         weights = list(self.network.gdf[self.rules.weight])
 
         self.network.gdf["src_tgt_wt"] = self.network._create_edge_ids(edges, weights)
 
         edges_start, weights_start = self.origins._get_edges_and_weights(
             nodes=self.network.nodes,
             rules=self.rules,
+            k=self._k_nearest_points,
         )
 
         edges = edges + edges_start
         weights = weights + weights_start
 
         if self.destinations is None:
             edge_ids = self.network._create_edge_ids(edges, weights)
             return edges, weights, edge_ids
 
         edges_end, weights_end = self.destinations._get_edges_and_weights(
             nodes=self.network.nodes,
             rules=self.rules,
+            k=self._k_nearest_points,
         )
 
         edges = edges + edges_end
         weights = weights + weights_end
 
         edge_ids = self.network._create_edge_ids(edges, weights)
 
@@ -1424,15 +1497,19 @@
 
         graph.es["weight"] = weights
         graph.es["src_tgt_wt"] = edge_ids
         graph.es["edge_tuples"] = edges
         graph.es["source"] = [edge[0] for edge in edges]
         graph.es["target"] = [edge[1] for edge in edges]
 
-        assert min(graph.es["weight"]) >= 0
+        if min(graph.es["weight"]) < 0:
+            n = sum([1 for w in graph.es["weight"] if w < 0])
+            raise ValueError(
+                f"The graph has been built with {n} negative weight values."
+            )
 
         return graph
 
     def _graph_is_up_to_date(self) -> bool:
         """Checks if the network or rules have changed.
 
         Returns False if the rules of the graphmaking has changed,
@@ -1500,15 +1577,15 @@
         if hasattr(breaks, "__iter__"):
             return list(sorted(list(breaks)))
 
         if isinstance(breaks, (int, float)):
             return [breaks]
 
         raise ValueError(
-            "'breaks' should not integer, float, string or an iterable of "
+            "'breaks' should be integer, float, string or an iterable of "
             f" one of these. Got {type(breaks)!r}"
         )
 
     def __repr__(self) -> str:
         """The print representation."""
         # drop the 'weight_to_nodes_' parameters in the repr of rules to avoid clutter
         rules = (
```

### Comparing `ssb_sgis-0.1.9/src/sgis/networkanalysis/networkanalysisrules.py` & `ssb_sgis-0.2.0/src/sgis/networkanalysis/networkanalysisrules.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """The NetworkAnalysisRules class sets the rules for the network analysis.
 
 The class is to be used as the 'rules' parameter in the NetworkAnalysis
 class.
 """
-import warnings
 from copy import copy, deepcopy
 from dataclasses import dataclass
 
 from geopandas import GeoDataFrame
 
 from ..helpers import unit_is_meters
 
@@ -52,15 +51,15 @@
     --------
     Read testdata.
 
     >>> import sgis as sg
     >>> roads = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_oslo_2022.parquet")
     >>> points = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_oslo.parquet")
 
-    Let's start by setting the default rules. 'weight' and 'directed' has noe default
+    Let's start by setting the default rules. 'weight' and 'directed' have no default
     values.
 
     >>> rules = sg.NetworkAnalysisRules(weight="minutes", directed=True)
     >>> directed_roads = sg.remove_isolated(roads).pipe(sg.make_directed_network_norway)
     >>> nwa = sg.NetworkAnalysis(network=directed_roads, rules=rules, detailed_log=False)
     >>> nwa
     NetworkAnalysis(
@@ -216,25 +215,28 @@
 
         # allow abbreviation of 'minutes' to be nice
         elif (
             self.weight == "min" or "minut" in self.weight and "minutes" in gdf.columns
         ):
             if self.nodedist_multiplier:
                 raise ValueError(
-                    "Cannot set 'nodedist_multiplier' when 'weight' is minutes."
+                    "Cannot set 'nodedist_multiplier' when 'weight' is minutes. "
+                    "Set 'nodedist_kmh' instead."
                 )
             self.weight = "minutes"
             gdf["minutes"] = gdf[self.weight]
+            self._check_for_nans(gdf, self.weight)
+            gdf = self._try_to_float(gdf, self.weight)
+            self._check_for_negative_values(gdf, self.weight)
             return gdf
 
         elif self.weight in gdf.columns:
-            gdf[self.weight] = gdf[self.weight].astype(float)
             self._check_for_nans(gdf, self.weight)
-            self._check_for_negative_values(gdf, self.weight)
             gdf = self._try_to_float(gdf, self.weight)
+            self._check_for_negative_values(gdf, self.weight)
             return gdf
 
         # at this point, the weight is wrong. Now to determine the error
         # message
 
         if "meter" in self.weight or "metre" in self.weight:
             raise ValueError(
@@ -269,15 +271,16 @@
 
     @staticmethod
     def _check_for_negative_values(df, col):
         """Remove negative values and give warning if there are any."""
         negative = sum(df[col] < 0)
         if negative:
             raise ValueError(
-                f": {negative} rows have {col!r} less than 0. Removing these " "rows.",
+                f"{negative} negative values found in the {col!r} column. Fill these "
+                "with a number greater than or equal to zero.",
             )
 
     @staticmethod
     def _try_to_float(df, col):
         """Try to convert weight column to float, raise ValueError if it fails."""
         try:
             df[col] = df[col].astype(float)
```

### Comparing `ssb_sgis-0.1.9/src/sgis/networkanalysis/nodes.py` & `ssb_sgis-0.2.0/src/sgis/networkanalysis/nodes.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.9/src/sgis/read_parquet.py` & `ssb_sgis-0.2.0/src/sgis/read_parquet.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from geopandas import GeoDataFrame
 
 
 def read_parquet_url(url: str) -> GeoDataFrame:
     """Reads geoparquet from a URL.
 
     Args:
-        url: url to a geoparquet file
+        url: URL containing a geoparquet file.
 
     Returns:
         A GeoDataFrame.
 
     Examples
     --------
     >>> from sgis import read_parquet_url
```

### Comparing `ssb_sgis-0.1.9/PKG-INFO` & `ssb_sgis-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: ssb-sgis
-Version: 0.1.9
+Version: 0.2.0
 Summary: GIS functions used at Statistics Norway.
 Home-page: https://github.com/statisticsnorway/ssb-sgis
 License: MIT
 Author: Statistics Norway
 Author-email: ort@ssb.no
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: GIS
-Requires-Dist: branca (>=0.6.0,<0.7.0)
-Requires-Dist: folium (>=0.14.0,<0.15.0)
-Requires-Dist: geopandas (>=0.12.2,<0.13.0)
-Requires-Dist: igraph (>=0.10.4,<0.11.0)
-Requires-Dist: jenkspy (>=0.3.2,<0.4.0)
-Requires-Dist: mapclassify (>=2.5.0,<3.0.0)
-Requires-Dist: matplotlib (>=3.7.0,<4.0.0)
-Requires-Dist: networkx (>=3.0,<4.0)
-Requires-Dist: numpy (>=1.24.2,<2.0.0)
-Requires-Dist: pandas (>=1.5.3,<2.0.0)
-Requires-Dist: pyarrow (>=11.0.0,<12.0.0)
-Requires-Dist: requests (>=2.28.2,<3.0.0)
-Requires-Dist: scikit-learn (>=1.2.1,<2.0.0)
-Requires-Dist: shapely (>=2.0.1,<3.0.0)
-Requires-Dist: xyzservices (>=2023.2.0,<2024.0.0)
+Requires-Dist: branca (>=0.6.0)
+Requires-Dist: folium (>=0.14.0)
+Requires-Dist: geopandas (>=0.12.2)
+Requires-Dist: igraph (>=0.10.4)
+Requires-Dist: ipython (>=8.13.2)
+Requires-Dist: jenkspy (>=0.3.2)
+Requires-Dist: mapclassify (>=2.5.0)
+Requires-Dist: matplotlib (>=3.7.0)
+Requires-Dist: networkx (>=3.0)
+Requires-Dist: numpy (>=1.24.2)
+Requires-Dist: pandas (>=1.5.3)
+Requires-Dist: pyarrow (>=11.0.0)
+Requires-Dist: requests (>=2.28.2)
+Requires-Dist: scikit-learn (>=1.2.1)
+Requires-Dist: shapely (>=2.0.1)
+Requires-Dist: xyzservices (>=2023.2.0)
 Project-URL: Changelog, https://github.com/statisticsnorway/ssb-sgis/releases
 Project-URL: Repository, https://github.com/statisticsnorway/ssb-sgis
 Description-Content-Type: text/markdown
 
 # ssb-sgis
 
 GIS Python tools used in [Statistics Norway](https://www.ssb.no/en).
@@ -39,15 +40,14 @@
 [![PyPI](https://img.shields.io/pypi/v/ssb-sgis.svg)][pypi_]
 [![Status](https://img.shields.io/pypi/status/ssb-sgis.svg)][status]
 [![Python Version](https://img.shields.io/pypi/pyversions/ssb-sgis)][python version]
 [![License](https://img.shields.io/pypi/l/ssb-sgis)][license]
 
 [![Documentation](https://img.shields.io/badge/Documentation-GitHub_Pages-green.svg)](https://statisticsnorway.github.io/ssb-sgis/index.html)
 [![Tests](https://github.com/statisticsnorway/ssb-sgis/workflows/Tests/badge.svg)][tests]
-[![Coverage](https://sonarcloud.io/component_measures?id=statisticsnorway_ssb-gis-utils&metric=new_coverage&view=list)][coverage]
 
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
 
 [pypi_]: https://pypi.org/project/ssb-sgis/
 [status]: https://pypi.org/project/ssb-sgis/
 [python version]: https://pypi.org/project/ssb-sgis
@@ -58,73 +58,59 @@
 [black]: https://github.com/psf/black
 
 sgis builds on the geopandas package and provides functions that make it easier to do GIS in python.
 Features include network analysis, functions for exploring multiple GeoDataFrames in a layered interactive map,
 and vector operations like finding k-nearest neighbours, splitting lines by points, snapping and closing holes
 in polygons by size.
 
+To install, use one of:
+
+```shell
+poetry add ssb-sgis
+pip install ssb-sgis
+```
+
 ## Network analysis examples
 
 Preparing for network analysis:
 
 ```python
 import sgis as sg
-import pandas as pd
+
 
 roads = sg.read_parquet_url(
     "https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_oslo_2022.parquet"
 )
 
 connected_roads = sg.get_connected_components(roads).query("connected == 1")
 
 directed_roads = sg.make_directed_network(
     connected_roads,
     direction_col="oneway",
     direction_vals_bft=("B", "FT", "TF"),
     minute_cols=("drivetime_fw", "drivetime_bw"),
 )
 
-rules = sg.NetworkAnalysisRules(weight="minutes", directed=True)
+rules = sg.NetworkAnalysisRules(directed=True, weight="minutes")
 
 nwa = sg.NetworkAnalysis(network=directed_roads, rules=rules)
 
 nwa
 ```
 
     NetworkAnalysis(
-        network=DirectedNetwork(6364 km, percent_bidirectional=87),
+        network=Network(6364 km, percent_bidirectional=87),
         rules=NetworkAnalysisRules(weight=minutes, directed=True, search_tolerance=250, search_factor=0, split_lines=False, ...),
-        log=True, detailed_log=True,
+        log=True, detailed_log=False,
     )
 
-Get number of times each line segment was visited, with optional weighting.
-
-```python
-origins = points.iloc[:75]
-destinations = points.iloc[75:150]
-
-# creating uniform weights of 10
-od_pairs = pd.MultiIndex.from_product([origins.index, destinations.index])
-weights = pd.DataFrame(index=od_pairs)
-weights["weight"] = 10
-
-frequencies = nwa.get_route_frequencies(origins, destinations, weight_df=weights)
-
-# plot the results
-m = sg.ThematicMap(sg.buff(frequencies, 15), column="frequency", black=True)
-m.cmap = "plasma"
-m.title = "Number of times each road was used,\nweighted * 10"
-m.plot()
-```
-
-![png](docs/examples/network_analysis_examples_files/network_analysis_examples_5_0.png)
-
 Fast many-to-many travel times/distances.
 
 ```python
+points = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_oslo.parquet")
 od = nwa.od_cost_matrix(points, points)
 
 print(od)
 ```
 
             origin  destination    minutes
     0            0            0   0.000000
@@ -137,14 +123,36 @@
     999996     999          996  17.820664
     999997     999          997  10.288465
     999998     999          998  14.798257
     999999     999          999   0.000000
 
     [1000000 rows x 3 columns]
 
+Get number of times each line segment was visited, with optional weighting.
+
+```python
+origins = points.iloc[:100]
+destinations = points.iloc[100:200]
+
+# creating uniform weights of 10
+od_pairs = pd.MultiIndex.from_product([origins.index, destinations.index])
+weights = pd.DataFrame(index=od_pairs)
+weights["weight"] = 10
+
+frequencies = nwa.get_route_frequencies(origins, destinations, weight_df=weights)
+
+# plot the results
+m = sg.ThematicMap(sg.buff(frequencies, 15), column="frequency", black=True)
+m.cmap = "plasma"
+m.title = "Number of times each road was used,\nweighted * 10"
+m.plot()
+```
+
+![png](docs/examples/network_analysis_examples_files/network_analysis_examples_5_0.png)
+
 Get the area that can be reached within one or more breaks.
 
 ```python
 service_areas = nwa.service_area(
     points.iloc[[0]],
     breaks=np.arange(1, 11),
 )
@@ -169,14 +177,16 @@
 m.title = "Four fastest routes from A to B"
 m.legend.title = "Rank"
 m.plot()
 ```
 
 ![png](docs/examples/network_analysis_examples_files/network_analysis_examples_11_0.png)
 
+More network analysis examples can be found here: https://github.com/statisticsnorway/ssb-sgis/blob/main/docs/network_analysis_demo_template.md
+
 Road data for Norway can be downloaded here: https://kartkatalog.geonorge.no/metadata/nvdb-ruteplan-nettverksdatasett/8d0f9066-34f9-4423-be12-8e8523089313
 
 ## Developer information
 
 ### Git LFS
 
 The data in the testdata directory is stored with [Git LFS](https://git-lfs.com/).
```

