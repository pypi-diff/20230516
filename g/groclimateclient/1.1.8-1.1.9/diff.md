# Comparing `tmp/groclimateclient-1.1.8.tar.gz` & `tmp/groclimateclient-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "groclimateclient-1.1.8.tar", max compression
+gzip compressed data, was "groclimateclient-1.1.9.tar", max compression
```

## Comparing `groclimateclient-1.1.8.tar` & `groclimateclient-1.1.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2023-05-02 20:23:28.721809 groclimateclient-1.1.8/LICENSE
--rw-r--r--   0        0        0      158 2023-05-02 20:23:28.721908 groclimateclient-1.1.8/README.md
--rw-r--r--   0        0        0     3243 2023-05-02 20:23:28.722091 groclimateclient-1.1.8/groclimateclient/CONTRIBUTING.md
--rw-r--r--   0        0        0       60 2023-05-02 20:23:28.722188 groclimateclient-1.1.8/groclimateclient/__init__.py
--rw-r--r--   0        0        0    16450 2023-05-02 20:23:28.722539 groclimateclient-1.1.8/groclimateclient/climate_client.py
--rw-r--r--   0        0        0    13745 2023-05-02 20:23:28.722706 groclimateclient-1.1.8/groclimateclient/constants.py
--rw-r--r--   0        0        0      706 2023-05-02 20:27:41.848894 groclimateclient-1.1.8/pyproject.toml
--rw-r--r--   0        0        0      946 1970-01-01 00:00:00.000000 groclimateclient-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1073 2022-09-01 19:43:38.683704 groclimateclient-1.1.9/LICENSE
+-rw-r--r--   0        0        0      158 2022-09-01 19:43:38.683785 groclimateclient-1.1.9/README.md
+-rw-r--r--   0        0        0     3421 2023-05-16 13:55:53.607861 groclimateclient-1.1.9/groclimateclient/CONTRIBUTING.md
+-rw-r--r--   0        0        0       60 2022-09-01 19:43:38.684016 groclimateclient-1.1.9/groclimateclient/__init__.py
+-rw-r--r--   0        0        0    16450 2022-09-01 19:43:38.684366 groclimateclient-1.1.9/groclimateclient/climate_client.py
+-rw-r--r--   0        0        0    13835 2023-05-16 13:55:53.608193 groclimateclient-1.1.9/groclimateclient/constants.py
+-rw-r--r--   0        0        0      706 2023-05-16 13:58:15.425605 groclimateclient-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0      946 1970-01-01 00:00:00.000000 groclimateclient-1.1.9/PKG-INFO
```

### Comparing `groclimateclient-1.1.8/LICENSE` & `groclimateclient-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `groclimateclient-1.1.8/groclimateclient/CONTRIBUTING.md` & `groclimateclient-1.1.9/groclimateclient/CONTRIBUTING.md`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,31 @@
 We use Poetry to manage packaging for the client library. Using Poetry for
 development is encouraged. See [Poetry docs](https://python-poetry.org/docs/)
 for full installation instructions.
 
 Here's the tl;dr for OS X and Linux:
 
 ```sh
-curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python -
+curl -sSL https://install.python-poetry.org | python3 -
 ```
 
 In case you need to `uninstall` poetry
 ```sh
-curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python - --uninstall
+curl -sSL https://install.python-poetry.org | python3 - --uninstall
 ```
 
+You will either need to add poetry to your $PATH or replace all below instances of `poetry` with:
+`~/Library/Application\ Support/pypoetry/venv/bin/poetry`
+
 ## Get the client library
 
 Clone the repo:
 
 ```sh
-git clone git@bitbucket.org:grointelligence/api-onboarding.git
+git clone git@github.com:grointelligence/api-onboarding.git
 cd gro-climate-client
 ```
 
 Install dependencies as well as a local editable copy of the library:
 
 ```sh
 poetry install
@@ -69,18 +72,18 @@
 To publish to PyPI, you'll need credentials. Using [PyPI API
 tokens](https://pypi.org/help/#apitoken) is recommended, like so:
 
 ```sh
 poetry publish --username __token__ --password <pypi-token-value-here>
 ```
 
-You can find pypi-token in shared [Gro Dev Ops Passwords](https://docs.google.com/spreadsheets/d/19urWvXdmZB36ZO5eg3Q-qqfHIxMcOl4_xeLJ-3Ugjqk/edit?usp=sharing):
+You can find pypi-token in shared [Gro Ops Passwords](https://docs.google.com/spreadsheets/d/19G8u229adwani2TR9iJ7CQ60EOftlW4EzziFy5fOyGc/edit#gid=0)
 
 You can also publish with the username and password for the [gro-intelligence
-account on PyPA](https://pypi.org/user/gro-intelligence/).
+account on PyPA](https://pypi.org/user/gro-intelligence/) (found in [Gro Ops Passwords](https://docs.google.com/spreadsheets/d/19G8u229adwani2TR9iJ7CQ60EOftlW4EzziFy5fOyGc/edit#gid=0)).
 
 ### Publishing to TestPyPI
 
 You'll need to first configure the repository:
 
 - configure the repository (only need to do this once): `poetry config
   repositories.testpypi https://test.pypi.org/legacy/`
@@ -88,12 +91,12 @@
   POETRY_REPOSITORIES_TESTPYPI_URL=https://test.pypi.org/legacy/`
 
 Then add `-r testpypi` to the publish command:
 
 ```sh
 poetry publish -r testpypi --username __token__ --password <pypi-token-value-here>
 ```
-Similarly, pypi-token can be found in [Gro Dev Ops Passwords](https://docs.google.com/spreadsheets/d/19urWvXdmZB36ZO5eg3Q-qqfHIxMcOl4_xeLJ-3Ugjqk/edit?usp=sharing):
+Similarly, pypi-token can be found in [Gro Ops Passwords](https://docs.google.com/spreadsheets/d/19G8u229adwani2TR9iJ7CQ60EOftlW4EzziFy5fOyGc/edit#gid=0):
 
 ### Conda package details
 
 Not supported yet
```

### Comparing `groclimateclient-1.1.8/groclimateclient/climate_client.py` & `groclimateclient-1.1.9/groclimateclient/climate_client.py`

 * *Files identical despite different names*

### Comparing `groclimateclient-1.1.8/groclimateclient/constants.py` & `groclimateclient-1.1.9/groclimateclient/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,14 +163,15 @@
     23834: "Tropical cyclones within 50 km, Saffir-Simpson Category 3-5",
     23835: "Tropical cyclones within 50 km, Saffir-Simpson Category 4-5",
     23836: "Tropical cyclones within 50 km, Saffir-Simpson Category 5",
     25884: "Ocean",
     25885: "Sea surface",
     26971: "Heat stress",
     26968: "Water stress",
+    27257: "Observed fire",
 }
 
 CLIMATE_METRICS = {
     1585211: "Aspect",
     1585297: "Atmospheric Greenhouse Gas Concentration",
     1585297: "Atmospheric Greenhouse Gas Concentration, Seasonally Corrected",
     1553109: "Availability in soil (amount of substance)",
@@ -262,14 +263,15 @@
     15854066: "Maximum water stress index (percent)",
     15854080: "Minimum water stress index (percent)",
     15854094: "Weighted mean water stress index (percent)",
     15854688: "Actual water stress score (number)",
     15854109: "Maximum water stress score (number)",
     15854123: "Minimum water stress score (number)",
     15854137: "Weighted mean water stress score (number)",
+    15854153: "Area with detected fire, % of total",
 }
 
 CLIMATE_SOURCES = [
     3,
     20,
     22,
     26,
@@ -317,9 +319,10 @@
     322,
     323,
     324,
     325,
     326,
     327,
     343,
+    344,
 ]
 CMIP6_SOURCES = [178, 189, 190, 191, 192, 300, 301, 302, 303, 304, 305, 306, 307, 308, 309]
```

### Comparing `groclimateclient-1.1.8/pyproject.toml` & `groclimateclient-1.1.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "groclimateclient"
 # Note: we use poetry-dynamic-versioning to set the version from git tags.
-version = "1.1.8"
+version = "1.1.9"
 description = "Python client library for accessing Gro Intelligence's climate data"
 authors = ["Gro Intelligence developers <dev@gro-intelligence.com>"]
 readme = "README.md"
 homepage = "https://www.gro-intelligence.com"
 repository = ""
 documentation = ""
 license = "MIT"
```

### Comparing `groclimateclient-1.1.8/PKG-INFO` & `groclimateclient-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: groclimateclient
-Version: 1.1.8
+Version: 1.1.9
 Summary: Python client library for accessing Gro Intelligence's climate data
 Home-page: https://www.gro-intelligence.com
 License: MIT
 Author: Gro Intelligence developers
 Author-email: dev@gro-intelligence.com
 Requires-Python: >=3.6.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

