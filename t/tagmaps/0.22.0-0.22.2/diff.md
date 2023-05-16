# Comparing `tmp/tagmaps-0.22.0.tar.gz` & `tmp/tagmaps-0.22.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tagmaps-0.22.0.tar", last modified: Wed May 10 09:28:24 2023, max compression
+gzip compressed data, was "tagmaps-0.22.2.tar", last modified: Tue May 16 06:26:17 2023, max compression
```

## Comparing `tagmaps-0.22.0.tar` & `tagmaps-0.22.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-10 09:28:24.395638 tagmaps-0.22.0/
--rw-r--r--   0 alex      (1000) alex      (1000)     8161 2023-05-10 09:27:59.000000 tagmaps-0.22.0/CHANGELOG.md
--rwxrwxrwx   0 alex      (1000) alex      (1000)    34940 2019-01-29 10:06:07.000000 tagmaps-0.22.0/LICENSE.md
--rw-rw-rw-   0 alex      (1000) alex      (1000)      164 2023-05-10 08:39:17.000000 tagmaps-0.22.0/MANIFEST.in
--rw-r--r--   0 alex      (1000) alex      (1000)    11727 2023-05-10 09:28:24.379823 tagmaps-0.22.0/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)    11570 2022-11-28 06:40:14.000000 tagmaps-0.22.0/README.md
--rw-r--r--   0 alex      (1000) alex      (1000)     2262 2023-05-10 08:37:55.000000 tagmaps-0.22.0/pyproject.toml
--rw-r--r--   0 alex      (1000) alex      (1000)       38 2023-05-10 09:28:24.395638 tagmaps-0.22.0/setup.cfg
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-10 09:28:24.122882 tagmaps-0.22.0/src/
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-10 09:28:24.211315 tagmaps-0.22.0/src/tagmaps/
--rw-rw-r--   0 alex      (1000) alex      (1000)      620 2021-02-18 12:42:56.000000 tagmaps-0.22.0/src/tagmaps/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5914 2022-07-27 08:37:55.000000 tagmaps-0.22.0/src/tagmaps/__main__.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-10 09:28:24.328506 tagmaps-0.22.0/src/tagmaps/classes/
--rw-rw-rw-   0 alex      (1000) alex      (1000)       33 2020-05-12 11:15:53.000000 tagmaps-0.22.0/src/tagmaps/classes/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    17469 2023-05-10 07:50:24.000000 tagmaps-0.22.0/src/tagmaps/classes/alpha_shapes.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    41054 2022-01-18 09:22:06.000000 tagmaps-0.22.0/src/tagmaps/classes/cluster.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    17232 2022-07-27 08:37:55.000000 tagmaps-0.22.0/src/tagmaps/classes/compile_output.py
--rw-r--r--   0 alex      (1000) alex      (1000)    23633 2022-11-28 06:40:14.000000 tagmaps-0.22.0/src/tagmaps/classes/interface.py
--rw-rw-rw-   0 alex      (1000) alex      (1000)    17745 2021-02-18 09:36:00.000000 tagmaps-0.22.0/src/tagmaps/classes/load_data.py
--rw-r--r--   0 alex      (1000) alex      (1000)    10479 2023-05-10 07:55:05.000000 tagmaps-0.22.0/src/tagmaps/classes/plotting.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    32505 2021-02-18 12:42:56.000000 tagmaps-0.22.0/src/tagmaps/classes/prepare_data.py
--rw-rw-rw-   0 alex      (1000) alex      (1000)     9578 2020-08-25 07:19:19.000000 tagmaps-0.22.0/src/tagmaps/classes/shared_structure.py
--rw-r--r--   0 alex      (1000) alex      (1000)    21911 2022-11-28 06:40:14.000000 tagmaps-0.22.0/src/tagmaps/classes/utils.py
--rwxrwxrwx   0 alex      (1000) alex      (1000)       75 2019-02-25 08:56:16.000000 tagmaps-0.22.0/src/tagmaps/classes/write_output.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-10 09:28:24.346148 tagmaps-0.22.0/src/tagmaps/config/
--rw-rw-rw-   0 alex      (1000) alex      (1000)       39 2020-05-12 11:15:53.000000 tagmaps-0.22.0/src/tagmaps/config/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    26041 2022-07-27 08:37:55.000000 tagmaps-0.22.0/src/tagmaps/config/config.py
--rwxrwxrwx   0 alex      (1000) alex      (1000)    31972 2017-12-21 09:44:59.000000 tagmaps-0.22.0/src/tagmaps/matplotlibrc
--rw-rw-r--   0 alex      (1000) alex      (1000)    19100 2022-07-27 08:37:55.000000 tagmaps-0.22.0/src/tagmaps/tagmaps_.py
--rw-r--r--   0 alex      (1000) alex      (1000)       46 2023-05-10 09:27:59.000000 tagmaps-0.22.0/src/tagmaps/version.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-10 09:28:24.234563 tagmaps-0.22.0/src/tagmaps.egg-info/
--rw-r--r--   0 alex      (1000) alex      (1000)    11727 2023-05-10 09:28:24.000000 tagmaps-0.22.0/src/tagmaps.egg-info/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)      885 2023-05-10 09:28:24.000000 tagmaps-0.22.0/src/tagmaps.egg-info/SOURCES.txt
--rw-r--r--   0 alex      (1000) alex      (1000)        1 2023-05-10 09:28:24.000000 tagmaps-0.22.0/src/tagmaps.egg-info/dependency_links.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       50 2023-05-10 09:28:24.000000 tagmaps-0.22.0/src/tagmaps.egg-info/entry_points.txt
--rw-r--r--   0 alex      (1000) alex      (1000)      149 2023-05-10 09:28:24.000000 tagmaps-0.22.0/src/tagmaps.egg-info/requires.txt
--rw-r--r--   0 alex      (1000) alex      (1000)        8 2023-05-10 09:28:24.000000 tagmaps-0.22.0/src/tagmaps.egg-info/top_level.txt
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-10 09:28:24.369274 tagmaps-0.22.0/tests/
--rw-rw-rw-   0 alex      (1000) alex      (1000)      626 2019-10-28 10:10:50.000000 tagmaps-0.22.0/tests/test_all.py
--rwxrwxrwx   0 alex      (1000) alex      (1000)     3271 2019-02-22 14:26:36.000000 tagmaps-0.22.0/tests/test_emoji.py
--rwxrwxrwx   0 alex      (1000) alex      (1000)      934 2019-01-29 10:06:07.000000 tagmaps-0.22.0/tests/test_post.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-16 06:26:17.341355 tagmaps-0.22.2/
+-rw-r--r--   0 alex      (1000) alex      (1000)     8506 2023-05-16 06:25:42.000000 tagmaps-0.22.2/CHANGELOG.md
+-rwxrwxrwx   0 alex      (1000) alex      (1000)    34940 2019-01-29 10:06:07.000000 tagmaps-0.22.2/LICENSE.md
+-rw-rw-rw-   0 alex      (1000) alex      (1000)      164 2023-05-10 08:39:17.000000 tagmaps-0.22.2/MANIFEST.in
+-rw-r--r--   0 alex      (1000) alex      (1000)    12279 2023-05-16 06:26:17.320066 tagmaps-0.22.2/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)    12128 2023-05-16 06:25:37.000000 tagmaps-0.22.2/README.md
+-rw-r--r--   0 alex      (1000) alex      (1000)     2195 2023-05-16 06:25:37.000000 tagmaps-0.22.2/pyproject.toml
+-rw-r--r--   0 alex      (1000) alex      (1000)       38 2023-05-16 06:26:17.341740 tagmaps-0.22.2/setup.cfg
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-16 06:26:16.848250 tagmaps-0.22.2/src/
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-16 06:26:16.988852 tagmaps-0.22.2/src/tagmaps/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      620 2021-02-18 12:42:56.000000 tagmaps-0.22.2/src/tagmaps/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5914 2022-07-27 08:37:55.000000 tagmaps-0.22.2/src/tagmaps/__main__.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-16 06:26:17.243393 tagmaps-0.22.2/src/tagmaps/classes/
+-rw-rw-rw-   0 alex      (1000) alex      (1000)       33 2020-05-12 11:15:53.000000 tagmaps-0.22.2/src/tagmaps/classes/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    17469 2023-05-10 07:50:24.000000 tagmaps-0.22.2/src/tagmaps/classes/alpha_shapes.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    41054 2022-01-18 09:22:06.000000 tagmaps-0.22.2/src/tagmaps/classes/cluster.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    17232 2022-07-27 08:37:55.000000 tagmaps-0.22.2/src/tagmaps/classes/compile_output.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    23633 2022-11-28 06:40:14.000000 tagmaps-0.22.2/src/tagmaps/classes/interface.py
+-rw-rw-rw-   0 alex      (1000) alex      (1000)    17745 2021-02-18 09:36:00.000000 tagmaps-0.22.2/src/tagmaps/classes/load_data.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    10479 2023-05-10 07:55:05.000000 tagmaps-0.22.2/src/tagmaps/classes/plotting.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    32505 2021-02-18 12:42:56.000000 tagmaps-0.22.2/src/tagmaps/classes/prepare_data.py
+-rw-rw-rw-   0 alex      (1000) alex      (1000)     9578 2020-08-25 07:19:19.000000 tagmaps-0.22.2/src/tagmaps/classes/shared_structure.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    21911 2022-11-28 06:40:14.000000 tagmaps-0.22.2/src/tagmaps/classes/utils.py
+-rwxrwxrwx   0 alex      (1000) alex      (1000)       75 2019-02-25 08:56:16.000000 tagmaps-0.22.2/src/tagmaps/classes/write_output.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-16 06:26:17.276984 tagmaps-0.22.2/src/tagmaps/config/
+-rw-rw-rw-   0 alex      (1000) alex      (1000)       39 2020-05-12 11:15:53.000000 tagmaps-0.22.2/src/tagmaps/config/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    26041 2022-07-27 08:37:55.000000 tagmaps-0.22.2/src/tagmaps/config/config.py
+-rwxrwxrwx   0 alex      (1000) alex      (1000)    31972 2017-12-21 09:44:59.000000 tagmaps-0.22.2/src/tagmaps/matplotlibrc
+-rw-rw-r--   0 alex      (1000) alex      (1000)    19100 2022-07-27 08:37:55.000000 tagmaps-0.22.2/src/tagmaps/tagmaps_.py
+-rw-r--r--   0 alex      (1000) alex      (1000)       46 2023-05-16 06:25:42.000000 tagmaps-0.22.2/src/tagmaps/version.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-16 06:26:17.019317 tagmaps-0.22.2/src/tagmaps.egg-info/
+-rwxrwxrwx   0 alex      (1000) alex      (1000)    12279 2023-05-16 06:26:16.000000 tagmaps-0.22.2/src/tagmaps.egg-info/PKG-INFO
+-rwxrwxrwx   0 alex      (1000) alex      (1000)      885 2023-05-16 06:26:16.000000 tagmaps-0.22.2/src/tagmaps.egg-info/SOURCES.txt
+-rwxrwxrwx   0 alex      (1000) alex      (1000)        1 2023-05-16 06:26:16.000000 tagmaps-0.22.2/src/tagmaps.egg-info/dependency_links.txt
+-rwxrwxrwx   0 alex      (1000) alex      (1000)       50 2023-05-16 06:26:16.000000 tagmaps-0.22.2/src/tagmaps.egg-info/entry_points.txt
+-rwxrwxrwx   0 alex      (1000) alex      (1000)      110 2023-05-16 06:26:16.000000 tagmaps-0.22.2/src/tagmaps.egg-info/requires.txt
+-rwxrwxrwx   0 alex      (1000) alex      (1000)        8 2023-05-16 06:26:16.000000 tagmaps-0.22.2/src/tagmaps.egg-info/top_level.txt
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-16 06:26:17.316745 tagmaps-0.22.2/tests/
+-rw-r--r--   0 alex      (1000) alex      (1000)      627 2023-05-16 06:25:37.000000 tagmaps-0.22.2/tests/test_all.py
+-rwxrwxrwx   0 alex      (1000) alex      (1000)     3271 2019-02-22 14:26:36.000000 tagmaps-0.22.2/tests/test_emoji.py
+-rwxrwxrwx   0 alex      (1000) alex      (1000)      934 2019-01-29 10:06:07.000000 tagmaps-0.22.2/tests/test_post.py
```

### Comparing `tagmaps-0.22.0/CHANGELOG.md` & `tagmaps-0.22.2/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.22.2 (2023-05-16)
+
+
+## v0.22.1 (2023-05-16)
+### Documentation
+* Restructure Developers section ([`ae93e68`](https://github.com/Sieboldianus/TagMaps/commit/ae93e686040d23e75117fcd1053ede7502da4bdb))
+* Add high-level update to changelog ([`6a1bc1f`](https://github.com/Sieboldianus/TagMaps/commit/6a1bc1f9db9355ff6ba1efd99cac9a1b510945d1))
+
 ## v0.22.0 (2023-05-10)
 ### Feature
 * Migrate project to pyproject.toml only ([`fc79efd`](https://github.com/Sieboldianus/TagMaps/commit/fc79efd653c982dc0db20e8a7f64110c152c037d))
 
 ### Documentation
 * Add basic description of project structure and release-flow for developers to documentation ([`f7e77db`](https://github.com/Sieboldianus/TagMaps/commit/f7e77db0754a70d4e92dafdd3ec9f19c4024a394))
 * Add purpose as docstring to environment.yml ([`5583627`](https://github.com/Sieboldianus/TagMaps/commit/558362784de10c360d88ed0be10ca5939c29bc38))
```

### Comparing `tagmaps-0.22.0/LICENSE.md` & `tagmaps-0.22.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.0/PKG-INFO` & `tagmaps-0.22.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: tagmaps
-Version: 0.22.0
+Version: 0.22.2
 Summary: Tag Clustering for Tag Maps
 Author-email: Alexander Dunkel <alexander.dunkel@tu-dresden.de>
 License: GNU GPLv3 or any higher
 Project-URL: Homepage, https://github.com/Sieboldianus/TagMaps
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-[![PyPI version](https://ad.vgiscience.org/tagmaps/pypi.svg)](https://pypi.org/project/tagmaps/) [![pylint](https://ad.vgiscience.org/tagmaps/pylint.svg)](https://github.com/Sieboldianus/TagMaps) [![pipeline](https://ad.vgiscience.org/tagmaps/pipeline.svg)](https://github.com/Sieboldianus/TagMaps) [![Conda Version](https://img.shields.io/conda/vn/conda-forge/tagmaps.svg)](https://anaconda.org/conda-forge/tagmaps) [![Conda Pipeline](https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/tagmaps-feedstock?branchName=master)](https://dev.azure.com/conda-forge/feedstock-builds/_build?definitionId=6736&_a=summary) [![Documentation](https://ad.vgiscience.org/tagmaps/documentation.svg)](https://ad.vgiscience.org/tagmaps/docs/)
+[![PyPI version](https://ad.vgiscience.org/tagmaps/pypi.svg)](https://pypi.org/project/tagmaps/) [![pylint](https://ad.vgiscience.org/tagmaps/pylint.svg)](https://github.com/Sieboldianus/TagMaps) [![pipeline](https://gitlab.vgiscience.de/ad/tagmaps/badges/master/pipeline.svg)](https://github.com/Sieboldianus/TagMaps) [![Conda Version](https://img.shields.io/conda/vn/conda-forge/tagmaps.svg)](https://anaconda.org/conda-forge/tagmaps) [![Conda Pipeline](https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/tagmaps-feedstock?branchName=master)](https://dev.azure.com/conda-forge/feedstock-builds/_build?definitionId=6736&_a=summary) [![Documentation](https://ad.vgiscience.org/tagmaps/documentation.svg)](https://ad.vgiscience.org/tagmaps/docs/)
 
 
 # Tag Maps
 
 Spatio-Temporal Tag and Photo Location Clustering for generating Tag Maps
 
 **Tag Maps** are similar to Tag Clouds, but Tag Maps use the spatial information that is attached to geotagged photographs, in addition to tag frequency, to visualize tags on a map.
@@ -68,29 +68,29 @@
 
 **Some background**:
 
 Tag Maps package can be used with any tagged & spatially referenced data, but it has been specifically developed with Social Media data in mind (Flickr, Twitter etc.).
 There are two ways to load input data:
 
 1. Unfiltered raw data
-   - Use `tagmaps.add_record(record)` where record is of type `PostStructure` (see [shared_structure.py](/tagmaps/classes/shared_structure.py))
-   - How you clean up data totally depends on the type, have a look at LoadData class in [load_data.py](/tagmaps/classes/load_data.py) for Twitter and  Flickr cleanup
+   - Use `tagmaps.add_record(record)` where record is of type `PostStructure` (see [shared_structure.py](src/tagmaps/classes/shared_structure.py))
+   - How you clean up data totally depends on the type, have a look at LoadData class in [load_data.py](src/tagmaps/classes/load_data.py) for Twitter and  Flickr cleanup
 2. Filtered data
    - the result from 1 is a `UserPostLocation` (UPL), which is a reference of type 'CleanedPost'. A UPL means that all posts of a single user at a single coordinate are merged,
      e.g. a reduced list of terms, tags and emoji based on global occurrence (i.e. no duplicates).
 
 3. The filtered data that is used for tagmaps can be exported using `tagmaps.write_cleaned_data()`.
    Since this will remove all terms/tags/emoji that do not appear in the top 1000 (e.g.) occurring global list of terms,
    this will produce a highly pseudonymized set of information, with only collectively relevant terms remaining.
    The default value (1000) can be adjusted using the `max_items` argument, e.g. the smaller max_items, the higher is the effect of anonymization/generalization.
 
 ## Code
 
 The code has been completely refactored in January 2019, but there are still some missing pieces.
-Particularly the API (that is: `import tagmaps`) is still in an early stage. See method main() in [**main**.py](/tagmaps/__main__.py)
+Particularly the API (that is: `import tagmaps`) is still in an early stage. See method main() in [**main**.py](src/tagmaps/__main__.py)
 for examples on how to use tag maps package.
 
 ## Resources
 
 - Check out [this album on Flickr](https://www.flickr.com/photos/64974314@N08/albums/72157628868173205) with some more Tag Maps examples
 - There's also an semi-interactive interface to explore some Tag Maps [here](http://maps.alexanderdunkel.com/)
 - Check out my blog [here](http://blog.alexanderdunkel.com/) with some background information
@@ -131,14 +131,20 @@
 
 GNU GPLv3
 
 ## Changelog & Download
 
 This is a high-level summary of version progress. See [CHANGELOG.md](CHANGELOG.md) for a full list of changes.
 
+2022-05-10: **TagMaps v0.22.0**
+
+- the project has finally migrated to a `pyproject.toml`-only based packaging system, as described in the [declarative config (pyproject.toml)](https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html)
+- structure now follows the [src-layout](https://setuptools.pypa.io/en/latest/userguide/package_discovery.html#src-layout).
+- fiona was pinned to `1.8.22` in conda until [#213](https://github.com/conda-forge/fiona-feedstock/issues/213) (Windows installations only) is solved
+
 2022-07-27: **TagMaps v0.21.0**
 
 - Add export to Mapnik ([`9db0d0d`](https://github.com/Sieboldianus/TagMaps/commit/9db0d0dc0a266f9eef7c3aac5bf663337c096f80)), enable with `--mapnik_export`
 - See a [jupyter lab notebook](https://ad.vgiscience.org/tagmaps-mapnik-jupyter/01_mapnik-tagmaps.html) that illustrates visualization of tag map data in [Mapnik](https://mapnik.org/)
 
 2021-02-22: **TagMaps v0.20.10**
```

### Comparing `tagmaps-0.22.0/README.md` & `tagmaps-0.22.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![PyPI version](https://ad.vgiscience.org/tagmaps/pypi.svg)](https://pypi.org/project/tagmaps/) [![pylint](https://ad.vgiscience.org/tagmaps/pylint.svg)](https://github.com/Sieboldianus/TagMaps) [![pipeline](https://ad.vgiscience.org/tagmaps/pipeline.svg)](https://github.com/Sieboldianus/TagMaps) [![Conda Version](https://img.shields.io/conda/vn/conda-forge/tagmaps.svg)](https://anaconda.org/conda-forge/tagmaps) [![Conda Pipeline](https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/tagmaps-feedstock?branchName=master)](https://dev.azure.com/conda-forge/feedstock-builds/_build?definitionId=6736&_a=summary) [![Documentation](https://ad.vgiscience.org/tagmaps/documentation.svg)](https://ad.vgiscience.org/tagmaps/docs/)
+[![PyPI version](https://ad.vgiscience.org/tagmaps/pypi.svg)](https://pypi.org/project/tagmaps/) [![pylint](https://ad.vgiscience.org/tagmaps/pylint.svg)](https://github.com/Sieboldianus/TagMaps) [![pipeline](https://gitlab.vgiscience.de/ad/tagmaps/badges/master/pipeline.svg)](https://github.com/Sieboldianus/TagMaps) [![Conda Version](https://img.shields.io/conda/vn/conda-forge/tagmaps.svg)](https://anaconda.org/conda-forge/tagmaps) [![Conda Pipeline](https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/tagmaps-feedstock?branchName=master)](https://dev.azure.com/conda-forge/feedstock-builds/_build?definitionId=6736&_a=summary) [![Documentation](https://ad.vgiscience.org/tagmaps/documentation.svg)](https://ad.vgiscience.org/tagmaps/docs/)
 
 
 # Tag Maps
 
 Spatio-Temporal Tag and Photo Location Clustering for generating Tag Maps
 
 **Tag Maps** are similar to Tag Clouds, but Tag Maps use the spatial information that is attached to geotagged photographs, in addition to tag frequency, to visualize tags on a map.
@@ -57,29 +57,29 @@
 
 **Some background**:
 
 Tag Maps package can be used with any tagged & spatially referenced data, but it has been specifically developed with Social Media data in mind (Flickr, Twitter etc.).
 There are two ways to load input data:
 
 1. Unfiltered raw data
-   - Use `tagmaps.add_record(record)` where record is of type `PostStructure` (see [shared_structure.py](/tagmaps/classes/shared_structure.py))
-   - How you clean up data totally depends on the type, have a look at LoadData class in [load_data.py](/tagmaps/classes/load_data.py) for Twitter and  Flickr cleanup
+   - Use `tagmaps.add_record(record)` where record is of type `PostStructure` (see [shared_structure.py](src/tagmaps/classes/shared_structure.py))
+   - How you clean up data totally depends on the type, have a look at LoadData class in [load_data.py](src/tagmaps/classes/load_data.py) for Twitter and  Flickr cleanup
 2. Filtered data
    - the result from 1 is a `UserPostLocation` (UPL), which is a reference of type 'CleanedPost'. A UPL means that all posts of a single user at a single coordinate are merged,
      e.g. a reduced list of terms, tags and emoji based on global occurrence (i.e. no duplicates).
 
 3. The filtered data that is used for tagmaps can be exported using `tagmaps.write_cleaned_data()`.
    Since this will remove all terms/tags/emoji that do not appear in the top 1000 (e.g.) occurring global list of terms,
    this will produce a highly pseudonymized set of information, with only collectively relevant terms remaining.
    The default value (1000) can be adjusted using the `max_items` argument, e.g. the smaller max_items, the higher is the effect of anonymization/generalization.
 
 ## Code
 
 The code has been completely refactored in January 2019, but there are still some missing pieces.
-Particularly the API (that is: `import tagmaps`) is still in an early stage. See method main() in [**main**.py](/tagmaps/__main__.py)
+Particularly the API (that is: `import tagmaps`) is still in an early stage. See method main() in [**main**.py](src/tagmaps/__main__.py)
 for examples on how to use tag maps package.
 
 ## Resources
 
 - Check out [this album on Flickr](https://www.flickr.com/photos/64974314@N08/albums/72157628868173205) with some more Tag Maps examples
 - There's also an semi-interactive interface to explore some Tag Maps [here](http://maps.alexanderdunkel.com/)
 - Check out my blog [here](http://blog.alexanderdunkel.com/) with some background information
@@ -120,14 +120,20 @@
 
 GNU GPLv3
 
 ## Changelog & Download
 
 This is a high-level summary of version progress. See [CHANGELOG.md](CHANGELOG.md) for a full list of changes.
 
+2022-05-10: **TagMaps v0.22.0**
+
+- the project has finally migrated to a `pyproject.toml`-only based packaging system, as described in the [declarative config (pyproject.toml)](https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html)
+- structure now follows the [src-layout](https://setuptools.pypa.io/en/latest/userguide/package_discovery.html#src-layout).
+- fiona was pinned to `1.8.22` in conda until [#213](https://github.com/conda-forge/fiona-feedstock/issues/213) (Windows installations only) is solved
+
 2022-07-27: **TagMaps v0.21.0**
 
 - Add export to Mapnik ([`9db0d0d`](https://github.com/Sieboldianus/TagMaps/commit/9db0d0dc0a266f9eef7c3aac5bf663337c096f80)), enable with `--mapnik_export`
 - See a [jupyter lab notebook](https://ad.vgiscience.org/tagmaps-mapnik-jupyter/01_mapnik-tagmaps.html) that illustrates visualization of tag map data in [Mapnik](https://mapnik.org/)
 
 2021-02-22: **TagMaps v0.20.10**
```

### Comparing `tagmaps-0.22.0/pyproject.toml` & `tagmaps-0.22.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,24 @@
 [project]
 name = "tagmaps"
 authors = [{name = "Alexander Dunkel", email = "alexander.dunkel@tu-dresden.de"}]
 license = {text = "GNU GPLv3 or any higher"}
 description = "Tag Clustering for Tag Maps"
 requires-python = ">=3.7"
 dependencies = [
-    "fiona==1.8.22",
+    "fiona",
     "shapely",
     "pandas>=0.24.2",
     "pyproj>=2.0.0",
     "numpy",
     "matplotlib>=3.0.0",
     "emoji>=2.0.0",
-    "cython",
     "hdbscan>=0.8.20",
-    "gdal>3.4.1",
     "seaborn",
-    "regex",
     "scipy",
-    "joblib",
 ]
 dynamic = ["version"]
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
```

### Comparing `tagmaps-0.22.0/src/tagmaps/__init__.py` & `tagmaps-0.22.2/src/tagmaps/__init__.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.0/src/tagmaps/__main__.py` & `tagmaps-0.22.2/src/tagmaps/__main__.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.0/src/tagmaps/classes/alpha_shapes.py` & `tagmaps-0.22.2/src/tagmaps/classes/alpha_shapes.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.0/src/tagmaps/classes/cluster.py` & `tagmaps-0.22.2/src/tagmaps/classes/cluster.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.0/src/tagmaps/classes/compile_output.py` & `tagmaps-0.22.2/src/tagmaps/classes/compile_output.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.0/src/tagmaps/classes/interface.py` & `tagmaps-0.22.2/src/tagmaps/classes/interface.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.0/src/tagmaps/classes/load_data.py` & `tagmaps-0.22.2/src/tagmaps/classes/load_data.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.0/src/tagmaps/classes/plotting.py` & `tagmaps-0.22.2/src/tagmaps/classes/plotting.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.0/src/tagmaps/classes/prepare_data.py` & `tagmaps-0.22.2/src/tagmaps/classes/prepare_data.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.0/src/tagmaps/classes/shared_structure.py` & `tagmaps-0.22.2/src/tagmaps/classes/shared_structure.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.0/src/tagmaps/classes/utils.py` & `tagmaps-0.22.2/src/tagmaps/classes/utils.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.0/src/tagmaps/config/config.py` & `tagmaps-0.22.2/src/tagmaps/config/config.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.0/src/tagmaps/matplotlibrc` & `tagmaps-0.22.2/src/tagmaps/matplotlibrc`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.0/src/tagmaps/tagmaps_.py` & `tagmaps-0.22.2/src/tagmaps/tagmaps_.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.0/src/tagmaps.egg-info/PKG-INFO` & `tagmaps-0.22.2/src/tagmaps.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: tagmaps
-Version: 0.22.0
+Version: 0.22.2
 Summary: Tag Clustering for Tag Maps
 Author-email: Alexander Dunkel <alexander.dunkel@tu-dresden.de>
 License: GNU GPLv3 or any higher
 Project-URL: Homepage, https://github.com/Sieboldianus/TagMaps
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-[![PyPI version](https://ad.vgiscience.org/tagmaps/pypi.svg)](https://pypi.org/project/tagmaps/) [![pylint](https://ad.vgiscience.org/tagmaps/pylint.svg)](https://github.com/Sieboldianus/TagMaps) [![pipeline](https://ad.vgiscience.org/tagmaps/pipeline.svg)](https://github.com/Sieboldianus/TagMaps) [![Conda Version](https://img.shields.io/conda/vn/conda-forge/tagmaps.svg)](https://anaconda.org/conda-forge/tagmaps) [![Conda Pipeline](https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/tagmaps-feedstock?branchName=master)](https://dev.azure.com/conda-forge/feedstock-builds/_build?definitionId=6736&_a=summary) [![Documentation](https://ad.vgiscience.org/tagmaps/documentation.svg)](https://ad.vgiscience.org/tagmaps/docs/)
+[![PyPI version](https://ad.vgiscience.org/tagmaps/pypi.svg)](https://pypi.org/project/tagmaps/) [![pylint](https://ad.vgiscience.org/tagmaps/pylint.svg)](https://github.com/Sieboldianus/TagMaps) [![pipeline](https://gitlab.vgiscience.de/ad/tagmaps/badges/master/pipeline.svg)](https://github.com/Sieboldianus/TagMaps) [![Conda Version](https://img.shields.io/conda/vn/conda-forge/tagmaps.svg)](https://anaconda.org/conda-forge/tagmaps) [![Conda Pipeline](https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/tagmaps-feedstock?branchName=master)](https://dev.azure.com/conda-forge/feedstock-builds/_build?definitionId=6736&_a=summary) [![Documentation](https://ad.vgiscience.org/tagmaps/documentation.svg)](https://ad.vgiscience.org/tagmaps/docs/)
 
 
 # Tag Maps
 
 Spatio-Temporal Tag and Photo Location Clustering for generating Tag Maps
 
 **Tag Maps** are similar to Tag Clouds, but Tag Maps use the spatial information that is attached to geotagged photographs, in addition to tag frequency, to visualize tags on a map.
@@ -68,29 +68,29 @@
 
 **Some background**:
 
 Tag Maps package can be used with any tagged & spatially referenced data, but it has been specifically developed with Social Media data in mind (Flickr, Twitter etc.).
 There are two ways to load input data:
 
 1. Unfiltered raw data
-   - Use `tagmaps.add_record(record)` where record is of type `PostStructure` (see [shared_structure.py](/tagmaps/classes/shared_structure.py))
-   - How you clean up data totally depends on the type, have a look at LoadData class in [load_data.py](/tagmaps/classes/load_data.py) for Twitter and  Flickr cleanup
+   - Use `tagmaps.add_record(record)` where record is of type `PostStructure` (see [shared_structure.py](src/tagmaps/classes/shared_structure.py))
+   - How you clean up data totally depends on the type, have a look at LoadData class in [load_data.py](src/tagmaps/classes/load_data.py) for Twitter and  Flickr cleanup
 2. Filtered data
    - the result from 1 is a `UserPostLocation` (UPL), which is a reference of type 'CleanedPost'. A UPL means that all posts of a single user at a single coordinate are merged,
      e.g. a reduced list of terms, tags and emoji based on global occurrence (i.e. no duplicates).
 
 3. The filtered data that is used for tagmaps can be exported using `tagmaps.write_cleaned_data()`.
    Since this will remove all terms/tags/emoji that do not appear in the top 1000 (e.g.) occurring global list of terms,
    this will produce a highly pseudonymized set of information, with only collectively relevant terms remaining.
    The default value (1000) can be adjusted using the `max_items` argument, e.g. the smaller max_items, the higher is the effect of anonymization/generalization.
 
 ## Code
 
 The code has been completely refactored in January 2019, but there are still some missing pieces.
-Particularly the API (that is: `import tagmaps`) is still in an early stage. See method main() in [**main**.py](/tagmaps/__main__.py)
+Particularly the API (that is: `import tagmaps`) is still in an early stage. See method main() in [**main**.py](src/tagmaps/__main__.py)
 for examples on how to use tag maps package.
 
 ## Resources
 
 - Check out [this album on Flickr](https://www.flickr.com/photos/64974314@N08/albums/72157628868173205) with some more Tag Maps examples
 - There's also an semi-interactive interface to explore some Tag Maps [here](http://maps.alexanderdunkel.com/)
 - Check out my blog [here](http://blog.alexanderdunkel.com/) with some background information
@@ -131,14 +131,20 @@
 
 GNU GPLv3
 
 ## Changelog & Download
 
 This is a high-level summary of version progress. See [CHANGELOG.md](CHANGELOG.md) for a full list of changes.
 
+2022-05-10: **TagMaps v0.22.0**
+
+- the project has finally migrated to a `pyproject.toml`-only based packaging system, as described in the [declarative config (pyproject.toml)](https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html)
+- structure now follows the [src-layout](https://setuptools.pypa.io/en/latest/userguide/package_discovery.html#src-layout).
+- fiona was pinned to `1.8.22` in conda until [#213](https://github.com/conda-forge/fiona-feedstock/issues/213) (Windows installations only) is solved
+
 2022-07-27: **TagMaps v0.21.0**
 
 - Add export to Mapnik ([`9db0d0d`](https://github.com/Sieboldianus/TagMaps/commit/9db0d0dc0a266f9eef7c3aac5bf663337c096f80)), enable with `--mapnik_export`
 - See a [jupyter lab notebook](https://ad.vgiscience.org/tagmaps-mapnik-jupyter/01_mapnik-tagmaps.html) that illustrates visualization of tag map data in [Mapnik](https://mapnik.org/)
 
 2021-02-22: **TagMaps v0.20.10**
```

### Comparing `tagmaps-0.22.0/src/tagmaps.egg-info/SOURCES.txt` & `tagmaps-0.22.2/src/tagmaps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.0/tests/test_all.py` & `tagmaps-0.22.2/tests/test_all.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Run Integration test for TagMaps
 
 
 This will check complete process of main() as if
-evoked with tagmaps --autoMode --maxItems 50
+invoked with tagmaps --autoMode --maxItems 50
 """
 
 import sys
 import os
 import traceback
 from pathlib import Path
 from tagmaps.__main__ import main as tm_main
@@ -21,9 +21,9 @@
         tm_main()
         sys.exit(0)
     except Exception:
         traceback.print_exc()
         sys.exit(1)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     tagmaps_system_integration_test()
```

### Comparing `tagmaps-0.22.0/tests/test_emoji.py` & `tagmaps-0.22.2/tests/test_emoji.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.0/tests/test_post.py` & `tagmaps-0.22.2/tests/test_post.py`

 * *Files identical despite different names*

