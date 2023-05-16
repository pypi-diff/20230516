# Comparing `tmp/vss-tools-4.0rc2.tar.gz` & `tmp/vss-tools-4.1.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vss-tools-4.0rc2.tar", last modified: Tue May 16 07:21:18 2023, max compression
+gzip compressed data, was "vss-tools-4.1.dev5.tar", last modified: Mon May 15 13:28:48 2023, max compression
```

## Comparing `vss-tools-4.0rc2.tar` & `vss-tools-4.1.dev5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-05-16 07:21:18.484208 vss-tools-4.0rc2/
--rw-r--r--   0 erik      (1000) erik      (1000)    16725 2022-08-23 11:55:56.000000 vss-tools-4.0rc2/LICENSE
--rw-r--r--   0 erik      (1000) erik      (1000)      236 2023-05-16 07:21:18.484208 vss-tools-4.0rc2/PKG-INFO
--rw-r--r--   0 erik      (1000) erik      (1000)    11203 2023-05-16 07:16:04.000000 vss-tools-4.0rc2/README.md
--rw-r--r--   0 erik      (1000) erik      (1000)       90 2023-05-15 11:45:18.000000 vss-tools-4.0rc2/pyproject.toml
--rw-r--r--   0 erik      (1000) erik      (1000)       38 2023-05-16 07:21:18.484208 vss-tools-4.0rc2/setup.cfg
--rw-r--r--   0 erik      (1000) erik      (1000)     1386 2023-05-16 07:18:39.000000 vss-tools-4.0rc2/setup.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-05-16 07:21:18.480208 vss-tools-4.0rc2/vspec/
--rwxr-xr-x   0 erik      (1000) erik      (1000)    35008 2023-05-04 13:37:39.000000 vss-tools-4.0rc2/vspec/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)      379 2023-02-22 10:27:00.000000 vss-tools-4.0rc2/vspec/loggingconfig.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-05-16 07:21:18.484208 vss-tools-4.0rc2/vspec/model/
--rw-r--r--   0 erik      (1000) erik      (1000)        0 2022-08-23 11:55:56.000000 vss-tools-4.0rc2/vspec/model/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)     6254 2023-05-04 07:44:52.000000 vss-tools-4.0rc2/vspec/model/constants.py
--rw-r--r--   0 erik      (1000) erik      (1000)      734 2023-05-04 07:44:52.000000 vss-tools-4.0rc2/vspec/model/exceptions.py
--rw-r--r--   0 erik      (1000) erik      (1000)    18800 2023-05-04 13:37:39.000000 vss-tools-4.0rc2/vspec/model/vsstree.py
--rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-02-22 10:27:00.000000 vss-tools-4.0rc2/vspec/py.typed
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-05-16 07:21:18.484208 vss-tools-4.0rc2/vspec/utils/
--rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-02-22 10:27:00.000000 vss-tools-4.0rc2/vspec/utils/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)      662 2023-02-22 10:27:00.000000 vss-tools-4.0rc2/vspec/utils/stringstyle.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-05-16 07:21:18.484208 vss-tools-4.0rc2/vspec/vssexporters/
--rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-02-22 10:27:00.000000 vss-tools-4.0rc2/vspec/vssexporters/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)     4612 2023-05-16 07:16:04.000000 vss-tools-4.0rc2/vspec/vssexporters/vss2binary.py
--rw-r--r--   0 erik      (1000) erik      (1000)     2786 2023-05-04 07:44:52.000000 vss-tools-4.0rc2/vspec/vssexporters/vss2csv.py
--rw-r--r--   0 erik      (1000) erik      (1000)     9218 2023-05-16 07:15:44.000000 vss-tools-4.0rc2/vspec/vssexporters/vss2ddsidl.py
--rw-r--r--   0 erik      (1000) erik      (1000)     2497 2023-02-22 10:27:00.000000 vss-tools-4.0rc2/vspec/vssexporters/vss2franca.py
--rw-r--r--   0 erik      (1000) erik      (1000)     5029 2023-04-17 11:54:24.000000 vss-tools-4.0rc2/vspec/vssexporters/vss2graphql.py
--rw-r--r--   0 erik      (1000) erik      (1000)     3863 2023-05-04 07:44:52.000000 vss-tools-4.0rc2/vspec/vssexporters/vss2json.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)     5933 2023-05-04 13:37:39.000000 vss-tools-4.0rc2/vspec/vssexporters/vss2protobuf.py
--rw-r--r--   0 erik      (1000) erik      (1000)     3864 2023-05-04 07:44:52.000000 vss-tools-4.0rc2/vspec/vssexporters/vss2yaml.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)      355 2023-03-29 09:18:58.000000 vss-tools-4.0rc2/vspec2csv.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)      355 2022-08-23 11:55:56.000000 vss-tools-4.0rc2/vspec2ddsidl.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)      375 2022-08-23 11:55:56.000000 vss-tools-4.0rc2/vspec2franca.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)      354 2022-08-23 11:55:56.000000 vss-tools-4.0rc2/vspec2graphql.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)      357 2022-08-23 11:55:56.000000 vss-tools-4.0rc2/vspec2json.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)      185 2023-05-04 07:44:52.000000 vss-tools-4.0rc2/vspec2protobuf.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)     9867 2023-05-04 13:37:39.000000 vss-tools-4.0rc2/vspec2x.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)      357 2022-08-23 11:55:56.000000 vss-tools-4.0rc2/vspec2yaml.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-05-16 07:21:18.484208 vss-tools-4.0rc2/vss_tools.egg-info/
--rw-r--r--   0 erik      (1000) erik      (1000)      236 2023-05-16 07:21:18.000000 vss-tools-4.0rc2/vss_tools.egg-info/PKG-INFO
--rw-r--r--   0 erik      (1000) erik      (1000)      820 2023-05-16 07:21:18.000000 vss-tools-4.0rc2/vss_tools.egg-info/SOURCES.txt
--rw-r--r--   0 erik      (1000) erik      (1000)        1 2023-05-16 07:21:18.000000 vss-tools-4.0rc2/vss_tools.egg-info/dependency_links.txt
--rw-r--r--   0 erik      (1000) erik      (1000)       59 2023-05-16 07:21:18.000000 vss-tools-4.0rc2/vss_tools.egg-info/requires.txt
--rw-r--r--   0 erik      (1000) erik      (1000)        6 2023-05-16 07:21:18.000000 vss-tools-4.0rc2/vss_tools.egg-info/top_level.txt
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-05-15 13:28:48.108762 vss-tools-4.1.dev5/
+-rw-r--r--   0 erik      (1000) erik      (1000)    16725 2022-08-23 11:55:56.000000 vss-tools-4.1.dev5/LICENSE
+-rw-r--r--   0 erik      (1000) erik      (1000)      238 2023-05-15 13:28:48.108762 vss-tools-4.1.dev5/PKG-INFO
+-rw-r--r--   0 erik      (1000) erik      (1000)    11930 2023-05-15 12:18:48.000000 vss-tools-4.1.dev5/README.md
+-rw-r--r--   0 erik      (1000) erik      (1000)       90 2023-05-15 11:45:18.000000 vss-tools-4.1.dev5/pyproject.toml
+-rw-r--r--   0 erik      (1000) erik      (1000)       38 2023-05-15 13:28:48.108762 vss-tools-4.1.dev5/setup.cfg
+-rw-r--r--   0 erik      (1000) erik      (1000)     1380 2023-05-15 12:29:02.000000 vss-tools-4.1.dev5/setup.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-05-15 13:28:48.104762 vss-tools-4.1.dev5/vspec/
+-rwxr-xr-x   0 erik      (1000) erik      (1000)    35008 2023-05-04 13:37:39.000000 vss-tools-4.1.dev5/vspec/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)      379 2023-02-22 10:27:00.000000 vss-tools-4.1.dev5/vspec/loggingconfig.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-05-15 13:28:48.108762 vss-tools-4.1.dev5/vspec/model/
+-rw-r--r--   0 erik      (1000) erik      (1000)        0 2022-08-23 11:55:56.000000 vss-tools-4.1.dev5/vspec/model/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     6254 2023-05-04 07:44:52.000000 vss-tools-4.1.dev5/vspec/model/constants.py
+-rw-r--r--   0 erik      (1000) erik      (1000)      734 2023-05-04 07:44:52.000000 vss-tools-4.1.dev5/vspec/model/exceptions.py
+-rw-r--r--   0 erik      (1000) erik      (1000)    18800 2023-05-04 13:37:39.000000 vss-tools-4.1.dev5/vspec/model/vsstree.py
+-rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-02-22 10:27:00.000000 vss-tools-4.1.dev5/vspec/py.typed
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-05-15 13:28:48.108762 vss-tools-4.1.dev5/vspec/utils/
+-rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-02-22 10:27:00.000000 vss-tools-4.1.dev5/vspec/utils/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)      662 2023-02-22 10:27:00.000000 vss-tools-4.1.dev5/vspec/utils/stringstyle.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-05-15 13:28:48.108762 vss-tools-4.1.dev5/vspec/vssexporters/
+-rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-02-22 10:27:00.000000 vss-tools-4.1.dev5/vspec/vssexporters/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     4612 2023-05-15 09:35:05.000000 vss-tools-4.1.dev5/vspec/vssexporters/vss2binary.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     2786 2023-05-04 07:44:52.000000 vss-tools-4.1.dev5/vspec/vssexporters/vss2csv.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     8117 2023-05-15 09:11:01.000000 vss-tools-4.1.dev5/vspec/vssexporters/vss2ddsidl.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     2497 2023-02-22 10:27:00.000000 vss-tools-4.1.dev5/vspec/vssexporters/vss2franca.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     5029 2023-04-17 11:54:24.000000 vss-tools-4.1.dev5/vspec/vssexporters/vss2graphql.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     3863 2023-05-04 07:44:52.000000 vss-tools-4.1.dev5/vspec/vssexporters/vss2json.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)     5933 2023-05-04 13:37:39.000000 vss-tools-4.1.dev5/vspec/vssexporters/vss2protobuf.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     3864 2023-05-04 07:44:52.000000 vss-tools-4.1.dev5/vspec/vssexporters/vss2yaml.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)      355 2023-03-29 09:18:58.000000 vss-tools-4.1.dev5/vspec2csv.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)      355 2022-08-23 11:55:56.000000 vss-tools-4.1.dev5/vspec2ddsidl.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)      375 2022-08-23 11:55:56.000000 vss-tools-4.1.dev5/vspec2franca.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)      354 2022-08-23 11:55:56.000000 vss-tools-4.1.dev5/vspec2graphql.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)      357 2022-08-23 11:55:56.000000 vss-tools-4.1.dev5/vspec2json.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)      185 2023-05-04 07:44:52.000000 vss-tools-4.1.dev5/vspec2protobuf.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)     9867 2023-05-04 13:37:39.000000 vss-tools-4.1.dev5/vspec2x.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)      357 2022-08-23 11:55:56.000000 vss-tools-4.1.dev5/vspec2yaml.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-05-15 13:28:48.108762 vss-tools-4.1.dev5/vss_tools.egg-info/
+-rw-r--r--   0 erik      (1000) erik      (1000)      238 2023-05-15 13:28:48.000000 vss-tools-4.1.dev5/vss_tools.egg-info/PKG-INFO
+-rw-r--r--   0 erik      (1000) erik      (1000)      820 2023-05-15 13:28:48.000000 vss-tools-4.1.dev5/vss_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)        1 2023-05-15 13:28:48.000000 vss-tools-4.1.dev5/vss_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)       59 2023-05-15 13:28:48.000000 vss-tools-4.1.dev5/vss_tools.egg-info/requires.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)        6 2023-05-15 13:28:48.000000 vss-tools-4.1.dev5/vss_tools.egg-info/top_level.txt
```

### Comparing `vss-tools-4.0rc2/LICENSE` & `vss-tools-4.1.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `vss-tools-4.0rc2/README.md` & `vss-tools-4.1.dev5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -28,19 +28,19 @@
 | [vspec2x.py](vspec2x.py) | Parses and expands VSS into different text based output formats. Currently supports `json`, `yaml`,`csv`,`idl`  | Community Supported | Try `./vspec2x --help` or check [vspec2x documentation](docs/vspec2x.md) |
 [vspec2csv.py](vspec2csv.py) | Shortcut for [vspec2x.py](vspec2x.py) generating CSV output | Community Supported |  Check [vspec2x documentation](docs/vspec2x.md) |
 [vspec2ddsidl.py](vspec2ddsidl.py) | Shortcut for [vspec2x.py](vspec2x.py) generating DDS-IDL output | Community Supported | [VSS2DDSIDL Documentation](docs/VSS2DDSIDL.md). For general parameters check [vspec2x documentation](docs/vspec2x.md) |
 [vspec2json.py](vspec2json.py) |  Shortcut for [vspec2x.py](vspec2x.py) generating JSON output | Community Supported | Check [vspec2x documentation](docs/vspec2x.md) |
 [vspec2yaml.py](vspec2yaml.py) | Shortcut for [vspec2x.py](vspec2x.py) generating flattened YAML output | Community Supported | Check [vspec2x documentation](docs/vspec2x.md) |
 [vspec2binary.py](vspec2binary.py) | The binary toolset consists of a tool that translates the VSS YAML specification to the binary file format (see below), and two libraries that provides methods that are likely to be needed by a server that manages the VSS tree, one written in C, and one in Go | Community Supported | [vspec2binary Documentation](binary/README.md). For general parameters check [vspec2x documentation](docs/vspec2x.md) |
 [vspec2franca.py](vspec2franca.py) | Parses and expands a VSS and generates a Franca IDL specification | Community Supported | Check [vspec2x documentation](docs/vspec2x.md) |
-[vspec2c.py](obsolete/vspec2c.py) | The vspec2c tooling allows a vehicle signal specification to be translated from its source YAML file to native C code that has the entire specification encoded in it. | Obsolete (2022-11-01) | [Documentation](obsolete/vspec2c/README.md) |
-[vspec2ocf.py](obsolete/ocf/vspec2ocf.py) | Parses and expands a VSS and generates a OCF specification | Obsolete (2022-11-01) | - |
+[vspec2c.py](contrib/vspec2c.py) | The vspec2c tooling allows a vehicle signal specification to be translated from its source YAML file to native C code that has the entire specification encoded in it. | Obsolete (2022-11-01) | [Documentation](obsolete/vspec2c/README.md) |
+[vspec2ocf.py](contrib/ocf/vspec2ocf.py) | Parses and expands a VSS and generates a OCF specification | Obsolete (2022-11-01) | - |
 [vspec2protobuf.py](vspec2protobuf.py) | Parses and expands a VSS and generates a Protobuf specification | Contrib | - |
 [vspec2ttl.py](contrib/vspec2ttl/vspec2ttl.py) | Parses and expands a VSS and generates a TTL specification | Contrib  | - |
-[vspec2graphql.py](vspec2graphql.py) | Parses and expands a VSS and generates a GraphQL specification | Community Supported  | [Documentation](docs/VSS2GRAPHQL.md) |
+[vspec2graphql.py](contrib/vspec2graphql.py) | Parses and expands a VSS and generates a GraphQL specification | Community Supported  | [Documentation](docs/VSS2GRAPHQL.md) |
 
 ## Tool Architecture
 
 All current tools are based on common Python functionality in the `vspec` folder to read, parse and expand a Vehicle Signal Specification files(*.vspec files). As an example, if the standard [VSS root file](https://github.com/COVESA/vehicle_signal_specification/blob/master/spec/VehicleSignalSpecification.vspec) is given as input then the Python tooling will read all included files, do a validation of the content, expand any instances used and create an in-memory representation which then can be used by specialized tools to generate the wanted output.
 
 ## Getting started
 
@@ -137,25 +137,46 @@
 ```
 
 ## Pre-commit set up
 This repository is set up to use pre-commit hooks. After you clone the project, run `pre-commit install` to install pre-commit into your git hooks. pre-commit will now run on every commit. Every time you clone a project using pre-commit running pre-commit install should always be the first thing you do.
 
 ## Building and installing with Pip
 
-Vss-tools can be installed by Pip. If you just want the latest version this should be sufficient:
+*Note: This is still an experimental feature*
+
+Vss-tools can be be built and uploaded to pypi. Currently it is built and published to [TestPypPI](https://test.pypi.org/)
+only as shown below. Version used is hardcoded in [setup.py](setup.py].
+
+```sh
+git clean -fdx
+python -m build
+python -m twine upload --repository testpypi dist/*
+```
+
+Available versions can be found [here](https://test.pypi.org/project/vss-tools/).
+Currently only pre-releases exist, which means that `--pre` must be used to install it.
 
 ```sh
-pip install vss-tools
+pip install --pre --index-url -U https://test.pypi.org/simple/ vss-tools
 ```
 
-When installed tools like `vspec2x.py` shall be available on your path.
+As `--pre` is used you might need to also specify default repository to find dependencies like anytree.
 
-For more information see the [wiki](https://github.com/COVESA/vss-tools/wiki/PyPI-packing).
+```sh
+python -m pip install --pre --index-url https://test.pypi.org/simple/ --extra-index-url  https://pypi.org/simple/ vss-tools
+```
+
+After installation, tools like `vspec2x.py` shall be available on your path without the need of cloning the repository.
+For development purposes you can install directly from source:
+
+```sh
+pip install -e .
+```
 
 ### Pip versioning
 
 This is the versions types that may exist in PyPI for vss-tools and used for local pip install (`pip install -e .`)
 
 * X.Y or X.Y.Z - A released version.
-* X.Y.devN, N starting from 0 - Developer builds - may be published to PyPI if needed for testing purposes.
+* X.Y.devN, N starting from 0 - Developer builds - normally not published to PyPI.
 * X.YaN, N starting from 0 - Pre-releases, may be published to PyPI if needed for testing purposes.
 * X.YrcN, N starting from 0 - Release candidates, to be published around two weeks before a major/minor release.
```

### Comparing `vss-tools-4.0rc2/setup.py` & `vss-tools-4.1.dev5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 #!/usr/bin/env python3
 from setuptools import setup, find_packages
 
-
 # Proposed versioning mechanism
 #
 # General: - Use 3 numbers only if needed, i.e. do not use X.Y.0
 #          - Master branch should by default always have a dev-version, except for released commits
 #
 # * During development (in master), use X.Y.devN, use N==0 as starting point, only increase N if needed for pypi
 #   reasons, like if a maintainer has pushed 4.0.dev0 to pypi, then update to 4.0.dev1
 # * For release candidates use X.YrcN, use N==0 as starting point
-# * If needed (for bigger functionality, dependencies, .., create pre-releases like 4.1a0
-# * When working on patches just add a third number, like 4.1.1, 4.1.1.dev0, 4.1.1rc0 (if needed at all)
+# * If needed (for bigger functionality, dependencies, .., create pre-releases like 0.4a0
+# * When working on patches just add a third number, like 0.4.1.dev0, 0.4.1rc0 (if needed at all)
 #
 #
 
 setup(
     name='vss-tools',
     description='COVESA Vehicle Signal Specification tooling.',
-    version='4.0rc2',
+    version='4.1.dev5',
     url='https://github.com/COVESA/vss-tools',
     license='Mozilla Public License 2.0',
     packages=find_packages(exclude=('tests', 'contrib')),
     scripts=['vspec2csv.py', 'vspec2x.py', 'vspec2franca.py', 'vspec2json.py', 'vspec2ddsidl.py',
              'vspec2yaml.py', 'vspec2protobuf.py', 'vspec2graphql.py'],
     python_requires='>=3.8',
     install_requires=['pyyaml>=5.1', 'anytree>=2.8.0', 'deprecation>=2.1.0', 'graphql-core'],
```

### Comparing `vss-tools-4.0rc2/vspec/__init__.py` & `vss-tools-4.1.dev5/vspec/__init__.py`

 * *Files identical despite different names*

### Comparing `vss-tools-4.0rc2/vspec/model/constants.py` & `vss-tools-4.1.dev5/vspec/model/constants.py`

 * *Files identical despite different names*

### Comparing `vss-tools-4.0rc2/vspec/model/exceptions.py` & `vss-tools-4.1.dev5/vspec/model/exceptions.py`

 * *Files identical despite different names*

### Comparing `vss-tools-4.0rc2/vspec/model/vsstree.py` & `vss-tools-4.1.dev5/vspec/model/vsstree.py`

 * *Files identical despite different names*

### Comparing `vss-tools-4.0rc2/vspec/utils/stringstyle.py` & `vss-tools-4.1.dev5/vspec/utils/stringstyle.py`

 * *Files identical despite different names*

### Comparing `vss-tools-4.0rc2/vspec/vssexporters/vss2binary.py` & `vss-tools-4.1.dev5/vspec/vssexporters/vss2binary.py`

 * *Files identical despite different names*

### Comparing `vss-tools-4.0rc2/vspec/vssexporters/vss2csv.py` & `vss-tools-4.1.dev5/vspec/vssexporters/vss2csv.py`

 * *Files identical despite different names*

### Comparing `vss-tools-4.0rc2/vspec/vssexporters/vss2ddsidl.py` & `vss-tools-4.1.dev5/vspec/vssexporters/vss2ddsidl.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,204 +6,179 @@
 # All files and artifacts in this repository are licensed under the
 # provisions of the license provided by the LICENSE file in this repository.
 #
 #
 # Convert vspec files to DDS-IDL
 #
 
+from email.policy import default
+import sys
+import vspec
 import argparse
 import keyword
 
 from vspec.model.vsstree import VSSNode, VSSType
 
-
 def add_arguments(parser: argparse.ArgumentParser):
-    parser.description = "The DDS-IDL exporter"
-    parser.add_argument('--all-idl-features', action='store_true',
+   parser.description="The DDS-IDL exporter"
+   parser.add_argument('--all-idl-features', action='store_true',
                         help='Generate all features based on DDS IDL 4.2 specification')
 
-
 c_keywords = [
-    "auto", "break", "case", "char", "const", "continue", "default", "do", "double", "else", "enum", "extern", "float",
-    "for", "goto", "if", "int", "long", "register", "return", "short", "signed", "sizeof", "static", "struct", "switch",
-    "typedef", "union", "unsigned", "void", "volatile", "while"
+    "auto"   , "break", "case"    , "char", "const"   , "continue", "default", "do"   , "double", "else"  , "enum"  , "extern", "float",
+    "for"    , "goto" , "if"      , "int" , "long"    , "register",  "return", "short", "signed", "sizeof", "static", "struct", "switch",
+    "typedef","union" , "unsigned", "void", "volatile", "while"
     ]
 
-# Based on http://www.omg.org/spec/IDL/4.2/
-idl_keywords = [
-    "abstract", "any", "alias", "attribute", "bitfield", "bitmask", "bitset", "boolean", "case", "char", "component",
-    "connector", "const", "consumes", "context", "custom", "default", "double", "exception", "emits", "enum",
-    "eventtype", "factory", "FALSE", "finder", "fixed", "float", "getraises", "home", "import", "in", "inout",
-    "interface", "local", "long", "manages", "map", "mirrorport", "module", "multiple", "native", "Object", "octet",
-    "oneway", "out", "primarykey", "private", "port", "porttype", "provides", "public", "publishes", "raises",
-    "readonly", "setraises", "sequence", "short", "string", "struct", "supports", "switch", "TRUE", "truncatable",
-    "typedef", "typeid", "typename", "typeprefix", "unsigned", "union", "uses", "ValueBase", "valuetype", "void",
-    "wchar", "wstring", "int8", "uint8", "int16", "int32", "int64", "uint16", "uint32", "uint64"
+#Based on http://www.omg.org/spec/IDL/4.2/
+idl_keywords =[
+    "abstract" ,"any"      ,"alias" ,"attribute","bitfield" ,"bitmask"   ,"bitset"   ,"boolean","case"       ,"char"    ,"component","connector" ,"const" ,
+    "consumes" ,"context"  ,"custom","default"  ,"double"   ,"exception" ,"emits"    ,"enum"   ,"eventtype"  ,"factory" ,"FALSE"    ,"finder"    ,"fixed" ,
+    "float"    ,"getraises","home"  ,"import"   ,"in"       ,"inout"     ,"interface","local"  ,"long"       ,"manages" ,"map"      ,"mirrorport","module","multiple",
+    "native"   ,"Object"   ,"octet" ,"oneway"   ,"out"      ,"primarykey","private"  ,"port"   ,"porttype"   ,"provides","public"   ,"publishes" ,"raises","readonly",
+    "setraises","sequence" ,"short" ,"string"   ,"struct"   ,"supports"  ,"switch"   ,"TRUE"   ,"truncatable","typedef" ,"typeid"   ,"typename"  ,"typeprefix",
+    "unsigned" ,"union"    ,"uses"  ,"ValueBase","valuetype","void"      ,"wchar"    ,"wstring","int8"       ,"uint8"   ,"int16"    ,"int32"     ,
+    "int64"    ,"uint16"   ,"uint32","uint64"
     ]
 
-
 def getAllowedName(name):
-    if (
+    if(
         name.lower() in c_keywords
-        or name.lower() in idl_keywords
+        or name.lower() in idl_keywords 
         or keyword.iskeyword(name.lower)
     ):
         return "_"+name
     else:
         return name
 
-
-def get_allowed_enum_literal(name: str):
-    """
-    Check if this is is an allowed literal name, if not add prefix.
-
-    Background:
-
-    In VSS '123' is a perfectly fine string literal, usable as allowed value for a string.
-    The current exporter (this file) translated it previously to 123 which is not a valid DSS IDL literal.
-    Adding an underscore as prefix makes the generated IDL ok, but then gives problems if generating for example
-    Python code by Eclipse Cyclone DDS idlc Python Backend.
-    By that reason we now add a regular character instead.
-    """
-    if name[0].isdigit():
-        return "d" + name
-    return name
-
-
 idlFileBuffer = []
 
-dataTypesMap_covesa_dds = {"uint8": "octet",
-                           "int8": "octet",
-                           "uint16": "unsigned short",
-                           "int16": "short",
-                           "uint32": "unsigned long",
-                           "int32": "long",
-                           "uint64": "unsigned long long",
-                           "int64": "long long",
-                           "boolean": "boolean",
-                           "float": "float",
-                           "double": "double",
-                           "string": "string"
-                           }
-
+dataTypesMap_covesa_dds={"uint8": "octet",
+              "int8": "octet",
+              "uint16": "unsigned short",
+              "int16": "short",
+              "uint32": "unsigned long",
+              "int32": "long",
+              "uint64": "unsigned long long",
+              "int64": "long long",
+              "boolean": "boolean",
+              "float": "float",
+              "double": "double",
+              "string": "string"
+              }
 
-def export_node(node, generate_uuid, generate_all_idl_features):
+def export_node( node, generate_uuid,generate_all_idl_features):
     """
     This method is used to traverse VSS node and to create corresponding DDS IDL buffer string
     """
     global idlFileBuffer
     datatype = None
-    unit = None
-    min = None
-    max = None
-    defaultValue = None
-    allowedValues = None
-    arraysize = None
+    unit=None
+    min=None
+    max=None
+    defaultValue=None
+    allowedValues=None
+    arraysize=None
 
     if node.type == VSSType.BRANCH:
         idlFileBuffer.append("module "+getAllowedName(node.name))
         idlFileBuffer.append("{")
         for child in node.children:
-            export_node(child, generate_uuid, generate_all_idl_features)
+            export_node( child, generate_uuid,generate_all_idl_features)
         idlFileBuffer.append("};")
-        idlFileBuffer.append("")
+        idlFileBuffer.append("");
     else:
-        isEnumCreated = False
-        # check if there is a need to create enum (based on the usage of allowed values)
-        if node.allowed != "":
+        isEnumCreated=False
+        #check if there is a need to create enum (based on the usage of allowed values)
+        if node.allowed!="":
             """
             enum should be enclosed under module block to avoid namespec conflict
-            module name for enum is chosen as the node name +
+            module name for enum is chosen as the node name + 
             """
             if (node.datatype.value in ["string", "string[]"]):
                 idlFileBuffer.append("module "+getAllowedName(node.name)+"_M")
                 idlFileBuffer.append("{")
-                idlFileBuffer.append("enum " + getAllowedName(node.name) +
-                                     "Values{"+str(",".join(get_allowed_enum_literal(item) for item in node.allowed)) +
-                                     "};")
-                isEnumCreated = True
+                idlFileBuffer.append("enum "+getAllowedName(node.name)+"Values{"+str(",".join(node.allowed))+"};")
+                isEnumCreated=True
                 idlFileBuffer.append("};")
-                allowedValues = str(node.allowed)
+                allowedValues=str(node.allowed)
             else:
-                print(f"Warning: VSS2IDL can only handle allowed values for string type, "
-                      f"signal {node.name} has type {node.datatype.value}")
+                print(f"Warning: VSS2IDL can only handle allowed values for string type, signal {node.name} has type {node.datatype.value}")
 
         idlFileBuffer.append("struct "+getAllowedName(node.name))
         idlFileBuffer.append("{")
         if generate_uuid:
             idlFileBuffer.append("string uuid;")
-        # fetching value of datatype and obtaining the equivalent DDS type
+        #fetching value of datatype and obtaining the equivalent DDS type
         try:
             if str(node.datatype.value) in dataTypesMap_covesa_dds:
-                datatype = str(dataTypesMap_covesa_dds[str(node.datatype.value)])
+                datatype= str(dataTypesMap_covesa_dds[str(node.datatype.value)])
             elif '[' in str(node.datatype.value):
-                nodevalueArray = str(node.datatype.value).split("[", 1)
-                if str(nodevalueArray[0]) in dataTypesMap_covesa_dds:
-                    datatype = str(dataTypesMap_covesa_dds[str(nodevalueArray[0])])
-                    arraysize = '['+str(arraysize)+nodevalueArray[1]
+                nodevalueArray=str(node.datatype.value).split("[",1)
+                if str(nodevalueArray[0]) in dataTypesMap_covesa_dds :
+                    datatype= str(dataTypesMap_covesa_dds[str(nodevalueArray[0])])
+                    arraysize='['+str(arraysize)+nodevalueArray[1]
 
         except AttributeError:
             pass
-        # fetching value of unit
+        #fetching value of unit
         try:
-            unit = str(node.unit.value)
+            unit =str(node.unit.value)
         except AttributeError:
             pass
 
-        if node.min != "":
-            min = str(node.min)
-        if node.max != "":
-            max = str(node.max)
+        if node.min!="":
+            min=str(node.min)
+        if node.max!="":
+            max=str(node.max)
         if node.default != "":
-            defaultValue = node.default
-            if isinstance(defaultValue, str) and not isEnumCreated:
-                defaultValue = "\""+defaultValue+"\""
-
-        if datatype is not None:
-            # adding range if min and max are specified in vspec file
-            if min is not None and max is not None and generate_all_idl_features:
+            defaultValue=node.default
+            if isinstance(defaultValue,str) and isEnumCreated==False:
+                defaultValue="\""+defaultValue+"\""
+
+
+        if datatype !=None:
+            #adding range if min and max are specified in vspec file
+            if min!=None and max!=None and generate_all_idl_features:
                 idlFileBuffer.append("@range(min="+str(min)+" ,max="+str(max)+")")
 
-            if allowedValues is None:
-                if defaultValue is None:
-                    idlFileBuffer.append(("sequence<"+datatype+"> value" if (arraysize is not None) else
-                                          datatype+" value")+";")
+            if allowedValues == None:
+                if defaultValue==None:
+                    idlFileBuffer.append(("sequence<"+datatype+"> value" if arraysize!=None else datatype+" value")+";" )
                 else:
-                    # default values in IDL file are not accepted by CycloneDDS/FastDDS :
-                    # these values can be generated if --all-idl-features is set as True
-                    idlFileBuffer.append(("sequence<"+datatype+"> value" if arraysize is not None else
-                                          datatype + " value") +
-                                         ("  default " + str(defaultValue) if generate_all_idl_features else "") + ";")
+                    #default values in IDL file are not accepted by CycloneDDS/FastDDS : these values can be generated if --all-idl-features is set as True
+                    idlFileBuffer.append(("sequence<"+datatype+"> value" if arraysize!=None else datatype+" value")+
+                                        ("  default "+str(defaultValue) if generate_all_idl_features else "") +";")
             else:
-                # this is the case where allowed values are provided, accordingly contents are converted to enum
-                if defaultValue is None:
+                #this is the case where allowed values are provided, accordingly contents are converted to enum
+                if defaultValue==None:
                     idlFileBuffer.append(getAllowedName(node.name)+"_M::"+getAllowedName(node.name)+"Values value;")
                 else:
-                    # default values in IDL file are not accepted by CycloneDDS/FastDDS :
-                    # these values can be generated if --all-idl-features is set as True
-                    idlFileBuffer.append(getAllowedName(node.name) + "_M::"+getAllowedName(node.name) + "Values value" +
-                                         (" " + str(defaultValue) if generate_all_idl_features else "") + ";")
+                    #default values in IDL file are not accepted by CycloneDDS/FastDDS : these values can be generated if --all-idl-features is set as True
+                    idlFileBuffer.append(getAllowedName(node.name)+"_M::"+getAllowedName(node.name)+"Values value"+ (" "+str(defaultValue) if generate_all_idl_features else "")+";")
 
-        if unit is not None:
-            idlFileBuffer.append(("" if generate_all_idl_features else "//") + "const string unit=\"" + unit + "\";")
 
-        idlFileBuffer.append(("" if generate_all_idl_features else "//") + "const string type =\"" +
-                             str(node.type.value) + "\";")
+        if unit!=None:
+            idlFileBuffer.append(("" if generate_all_idl_features else "//")+"const string unit=\""+unit +"\";")
 
-        idlFileBuffer.append(("" if generate_all_idl_features else "//") + "const string description=\"" +
-                             node.description + "\";")
+
+
+        idlFileBuffer.append(("" if generate_all_idl_features else "//")+"const string type =\""+  str(node.type.value)+"\";")
+
+        idlFileBuffer.append(("" if generate_all_idl_features else "//")+"const string description=\""+  node.description+"\";")
         idlFileBuffer.append("};")
 
 
 def export_idl(file, root, generate_uuids=True, generate_all_idl_features=False):
     """This method is used to traverse through the root VSS node to build
        -> DDS IDL equivalent string buffer and to serialize it acccordingly into a file
     """
-    export_node(root, generate_uuids, generate_all_idl_features)
+    export_node( root, generate_uuids,generate_all_idl_features)
     file.write('\n'.join(idlFileBuffer))
     print("IDL file generated at location : "+file.name)
 
 
+
 def export(config: argparse.Namespace, root: VSSNode, print_uuid):
     print("Generating DDS-IDL output...")
-    idl_out = open(config.output_file, 'w')
-    export_idl(idl_out, root, print_uuid, config.all_idl_features)
+    idl_out=open(config.output_file,'w')
+    export_idl(idl_out, root, print_uuid, config.all_idl_features)
```

### Comparing `vss-tools-4.0rc2/vspec/vssexporters/vss2franca.py` & `vss-tools-4.1.dev5/vspec/vssexporters/vss2franca.py`

 * *Files identical despite different names*

### Comparing `vss-tools-4.0rc2/vspec/vssexporters/vss2graphql.py` & `vss-tools-4.1.dev5/vspec/vssexporters/vss2graphql.py`

 * *Files identical despite different names*

### Comparing `vss-tools-4.0rc2/vspec/vssexporters/vss2json.py` & `vss-tools-4.1.dev5/vspec/vssexporters/vss2json.py`

 * *Files identical despite different names*

### Comparing `vss-tools-4.0rc2/vspec/vssexporters/vss2protobuf.py` & `vss-tools-4.1.dev5/vspec/vssexporters/vss2protobuf.py`

 * *Files identical despite different names*

### Comparing `vss-tools-4.0rc2/vspec/vssexporters/vss2yaml.py` & `vss-tools-4.1.dev5/vspec/vssexporters/vss2yaml.py`

 * *Files identical despite different names*

### Comparing `vss-tools-4.0rc2/vspec2x.py` & `vss-tools-4.1.dev5/vspec2x.py`

 * *Files identical despite different names*

### Comparing `vss-tools-4.0rc2/vss_tools.egg-info/SOURCES.txt` & `vss-tools-4.1.dev5/vss_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

