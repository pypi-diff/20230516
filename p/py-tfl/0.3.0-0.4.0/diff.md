# Comparing `tmp/py_tfl-0.3.0.tar.gz` & `tmp/py_tfl-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_tfl-0.3.0.tar", max compression
+gzip compressed data, was "py_tfl-0.4.0.tar", max compression
```

## Comparing `py_tfl-0.3.0.tar` & `py_tfl-0.4.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rw-r--r--   0        0        0     1068 2023-05-09 18:55:40.123287 py_tfl-0.3.0/LICENSE
--rw-r--r--   0        0        0     4316 2023-05-09 18:55:40.123287 py_tfl-0.3.0/README.md
--rw-r--r--   0        0        0     2346 2023-05-09 18:55:40.127288 py_tfl-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      121 2023-05-09 18:55:40.127288 py_tfl-0.3.0/tfl/__init__.py
--rw-r--r--   0        0        0       68 2023-05-09 18:55:40.127288 py_tfl-0.3.0/tfl/cli/__init__.py
--rw-r--r--   0        0        0     1345 2023-05-09 18:55:40.127288 py_tfl-0.3.0/tfl/cli/_async_typer.py
--rw-r--r--   0        0        0     2056 2023-05-09 18:55:40.127288 py_tfl-0.3.0/tfl/cli/main.py
--rw-r--r--   0        0        0        0 2023-05-09 18:55:40.127288 py_tfl-0.3.0/tfl/cli/py.typed
--rw-r--r--   0        0        0      359 2023-05-09 18:55:40.127288 py_tfl-0.3.0/tfl/clients/__init__.py
--rw-r--r--   0        0        0     4650 2023-05-09 18:55:40.127288 py_tfl-0.3.0/tfl/clients/_accident_stats_client.py
--rw-r--r--   0        0        0     4484 2023-05-09 18:55:40.127288 py_tfl-0.3.0/tfl/clients/_air_quality_client.py
--rw-r--r--   0        0        0     1696 2023-05-09 18:55:40.127288 py_tfl-0.3.0/tfl/clients/_auth.py
--rw-r--r--   0        0        0     5000 2023-05-09 18:55:40.127288 py_tfl-0.3.0/tfl/clients/_client.py
--rw-r--r--   0        0        0     4463 2023-05-09 18:55:40.127288 py_tfl-0.3.0/tfl/clients/_lift_disruptions_client.py
--rw-r--r--   0        0        0        0 2023-05-09 18:55:40.127288 py_tfl-0.3.0/tfl/clients/py.typed
--rw-r--r--   0        0        0        0 2023-05-09 18:55:40.127288 py_tfl-0.3.0/tfl/py.typed
--rw-r--r--   0        0        0     5490 1970-01-01 00:00:00.000000 py_tfl-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-16 18:51:49.957667 py_tfl-0.4.0/LICENSE
+-rw-r--r--   0        0        0     4409 2023-05-16 18:51:49.957667 py_tfl-0.4.0/README.md
+-rw-r--r--   0        0        0     2347 2023-05-16 18:51:49.961668 py_tfl-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      128 2023-05-16 18:51:49.961668 py_tfl-0.4.0/tfl/__init__.py
+-rw-r--r--   0        0        0       68 2023-05-16 18:51:49.961668 py_tfl-0.4.0/tfl/cli/__init__.py
+-rw-r--r--   0        0        0     1345 2023-05-16 18:51:49.961668 py_tfl-0.4.0/tfl/cli/_async_typer.py
+-rw-r--r--   0        0        0     2930 2023-05-16 18:51:49.961668 py_tfl-0.4.0/tfl/cli/main.py
+-rw-r--r--   0        0        0        0 2023-05-16 18:51:49.961668 py_tfl-0.4.0/tfl/cli/py.typed
+-rw-r--r--   0        0        0      415 2023-05-16 18:51:49.961668 py_tfl-0.4.0/tfl/clients/__init__.py
+-rw-r--r--   0        0        0     4650 2023-05-16 18:51:49.961668 py_tfl-0.4.0/tfl/clients/_accident_stats_client.py
+-rw-r--r--   0        0        0     4484 2023-05-16 18:51:49.961668 py_tfl-0.4.0/tfl/clients/_air_quality_client.py
+-rw-r--r--   0        0        0     1696 2023-05-16 18:51:49.961668 py_tfl-0.4.0/tfl/clients/_auth.py
+-rw-r--r--   0        0        0     5000 2023-05-16 18:51:49.961668 py_tfl-0.4.0/tfl/clients/_client.py
+-rw-r--r--   0        0        0     4913 2023-05-16 18:51:49.961668 py_tfl-0.4.0/tfl/clients/_crowding_client.py
+-rw-r--r--   0        0        0     4463 2023-05-16 18:51:49.961668 py_tfl-0.4.0/tfl/clients/_lift_disruptions_client.py
+-rw-r--r--   0        0        0        0 2023-05-16 18:51:49.961668 py_tfl-0.4.0/tfl/clients/py.typed
+-rw-r--r--   0        0        0      561 2023-05-16 18:51:49.961668 py_tfl-0.4.0/tfl/enums.py
+-rw-r--r--   0        0        0        0 2023-05-16 18:51:49.961668 py_tfl-0.4.0/tfl/py.typed
+-rw-r--r--   0        0        0     5583 1970-01-01 00:00:00.000000 py_tfl-0.4.0/PKG-INFO
```

### Comparing `py_tfl-0.3.0/LICENSE` & `py_tfl-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_tfl-0.3.0/README.md` & `py_tfl-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 call the API more than that, you'll need to subscribe to a "Product" which lets you bypass this limit with a
 subscription-key that you append to your requests.
 
 Currently, we support the following APIs:
 
 - [Accident Stats API](https://api-portal.tfl.gov.uk/api-details#api=AccidentStats&operation=AccidentStats_Get)
 - [Air Quality API](https://api-portal.tfl.gov.uk/api-details#api=AirQuality&operation=AirQuality_Get)
+- [Crowding API](https://api-portal.tfl.gov.uk/api-details#api=crowding&operation=dayofweek)
 - [Lift Disruptions API](https://api-portal.tfl.gov.uk/api-details#api=Disruptions-Lifts-v2&operation=get)
 
 The plan is to add support for all the TFL APIs. Contributions are welcome!
 
 ## Installation
 
 ```bash
```

### Comparing `py_tfl-0.3.0/pyproject.toml` & `py_tfl-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "py-tfl"
-version = "0.3.0"
+version = "0.4.0"
 description = "A Python package for the Transport for London (TFL) API."
 authors = ["Cellan Hall <hallcellan@gmail.com>"]
 readme = "README.md"
 packages = [
     {include = "tfl"},
 ]
 homepage = "https://ce11an.github.io/tfl/"
@@ -34,21 +34,21 @@
 python = ">=3.8, <3.12"
 httpx = "~=0.24.0"
 typer = {extras = ["all"], version = "~=0.9.0"}
 
 [tool.poetry.dev-dependencies]
 pre-commit = "~=3.3.1"
 black = "~=23.3.0"
-ruff = "~=0.0.263"
-mypy = "~=1.2.0"
+ruff = "~=0.0.267"
+mypy = "~=1.3.0"
 pytest = "~=7.3.1"
 pytest-cov = "~=4.0.0"
 pytest-httpx = "~=0.22.0"
 pytest-asyncio = "~=0.21.0"
-mkdocs-material = "~=9.1.9"
+mkdocs-material = "~=9.1.12"
 mkdocstrings = {extras = ["python"], version = "~=0.21.2"}
 
 [tool.black]
 line-length = 120
 color = true
 
 exclude = '''
```

### Comparing `py_tfl-0.3.0/tfl/cli/_async_typer.py` & `py_tfl-0.4.0/tfl/cli/_async_typer.py`

 * *Files identical despite different names*

### Comparing `py_tfl-0.3.0/tfl/cli/main.py` & `py_tfl-0.4.0/tfl/cli/main.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Optional
 
 import rich
 import typer
 from typing_extensions import Annotated
 
 import tfl
+import tfl.enums
 from tfl import cli, clients
 
 app = cli.AsyncTyper()
 
 
 def version_callback(version: bool) -> None:
     """Print the version of tfl."""
@@ -39,14 +40,34 @@
     async with clients.AccidentStatsClient(auth=tfl.clients.Auth(key=key) if key else None) as client:
         response = await client.get_accident_stats(year=year)
     rich.print(response.json())
     raise typer.Exit()
 
 
 @app.async_command()
+async def crowding(
+    naptan_code: Annotated[str, typer.Argument(help="The NAPTAN code of the station to get crowding for.")],
+    day: Annotated[
+        Optional[str],
+        typer.Argument(
+            help="The day to get crowding information for. The options are 'Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', "
+            "'Sun', 'Live'."
+        ),
+    ] = None,
+    key: Annotated[Optional[str], typer.Argument(envvar="TFL_API_KEY", help="TFL API key.")] = None,
+) -> None:
+    """Information about crowding levels within TFL stations."""
+    day = tfl.enums.DayOfWeekEnum(day) if day else None
+    async with clients.CrowdingClient(auth=tfl.clients.Auth(key=key) if key else None) as client:
+        response = await client.get_crowding(naptan_code=naptan_code, day=day)
+    rich.print(response.json())
+    raise typer.Exit()
+
+
+@app.async_command()
 async def air_quality(
     key: Annotated[Optional[str], typer.Argument(envvar="TFL_API_KEY", help="TFL API key.")] = None,
 ) -> None:
     """Get air quality data feed."""
     async with clients.AirQualityClient(auth=tfl.clients.Auth(key=key) if key else None) as client:
         response = await client.get_air_quality()
     rich.print(response.json())
```

### Comparing `py_tfl-0.3.0/tfl/clients/_accident_stats_client.py` & `py_tfl-0.4.0/tfl/clients/_accident_stats_client.py`

 * *Files identical despite different names*

### Comparing `py_tfl-0.3.0/tfl/clients/_air_quality_client.py` & `py_tfl-0.4.0/tfl/clients/_air_quality_client.py`

 * *Files identical despite different names*

### Comparing `py_tfl-0.3.0/tfl/clients/_auth.py` & `py_tfl-0.4.0/tfl/clients/_auth.py`

 * *Files identical despite different names*

### Comparing `py_tfl-0.3.0/tfl/clients/_client.py` & `py_tfl-0.4.0/tfl/clients/_client.py`

 * *Files identical despite different names*

### Comparing `py_tfl-0.3.0/tfl/clients/_lift_disruptions_client.py` & `py_tfl-0.4.0/tfl/clients/_lift_disruptions_client.py`

 * *Files identical despite different names*

### Comparing `py_tfl-0.3.0/PKG-INFO` & `py_tfl-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-tfl
-Version: 0.3.0
+Version: 0.4.0
 Summary: A Python package for the Transport for London (TFL) API.
 Home-page: https://ce11an.github.io/tfl/
 Author: Cellan Hall
 Author-email: hallcellan@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -46,14 +46,15 @@
 call the API more than that, you'll need to subscribe to a "Product" which lets you bypass this limit with a
 subscription-key that you append to your requests.
 
 Currently, we support the following APIs:
 
 - [Accident Stats API](https://api-portal.tfl.gov.uk/api-details#api=AccidentStats&operation=AccidentStats_Get)
 - [Air Quality API](https://api-portal.tfl.gov.uk/api-details#api=AirQuality&operation=AirQuality_Get)
+- [Crowding API](https://api-portal.tfl.gov.uk/api-details#api=crowding&operation=dayofweek)
 - [Lift Disruptions API](https://api-portal.tfl.gov.uk/api-details#api=Disruptions-Lifts-v2&operation=get)
 
 The plan is to add support for all the TFL APIs. Contributions are welcome!
 
 ## Installation
 
 ```bash
```

