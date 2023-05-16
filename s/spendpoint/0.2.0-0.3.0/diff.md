# Comparing `tmp/spendpoint-0.2.0.tar.gz` & `tmp/spendpoint-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spendpoint-0.2.0.tar", last modified: Tue Apr  4 11:08:02 2023, max compression
+gzip compressed data, was "spendpoint-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `spendpoint-0.2.0.tar` & `spendpoint-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,28 @@
--rw-r--r--   0        0        0      103 2023-04-04 10:46:28.100041 spendpoint-0.2.0/.dockerignore
--rw-r--r--   0        0        0      274 2023-04-04 10:46:28.100041 spendpoint-0.2.0/.editorconfig
--rw-r--r--   0        0        0      114 2023-04-04 10:46:28.100041 spendpoint-0.2.0/.gitignore
--rw-r--r--   0        0        0     1826 2023-04-04 10:46:28.100041 spendpoint-0.2.0/.gitlab-ci.yml
--rw-r--r--   0        0        0      178 2023-04-04 10:46:28.100041 spendpoint-0.2.0/AUTHORS.rst
--rw-r--r--   0        0        0      387 2023-04-04 10:46:28.100041 spendpoint-0.2.0/Dockerfile
--rw-r--r--   0        0        0      375 2023-04-04 10:46:28.100041 spendpoint-0.2.0/HISTORY.rst
--rw-r--r--   0        0        0     1081 2023-04-04 10:46:28.100041 spendpoint-0.2.0/LICENSE
--rw-r--r--   0        0        0      486 2023-04-04 10:46:28.100041 spendpoint-0.2.0/README.rst
--rw-r--r--   0        0        0     1054 2023-04-04 10:46:28.104042 spendpoint-0.2.0/docs/templates/pyproject.toml
--rw-r--r--   0        0        0     1203 2023-04-04 10:46:28.104042 spendpoint-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      513 2023-04-04 10:46:28.104042 spendpoint-0.2.0/requirements.txt
--rw-r--r--   0        0        0      178 2023-04-04 10:46:28.104042 spendpoint-0.2.0/spendpoint/__init__.py
--rw-r--r--   0        0        0       92 2023-04-04 10:46:28.104042 spendpoint-0.2.0/spendpoint/__main__.py
--rw-r--r--   0        0        0     1670 2023-04-04 10:46:28.104042 spendpoint-0.2.0/spendpoint/bridge.py
--rw-r--r--   0        0        0     8861 2023-04-04 10:46:28.104042 spendpoint-0.2.0/spendpoint/endpoint.py
--rw-r--r--   0        0        0      766 2023-04-04 10:46:28.104042 spendpoint-0.2.0/spendpoint/main.py
--rw-r--r--   0        0        0     4088 2023-04-04 10:46:28.104042 spendpoint-0.2.0/spendpoint/service.py
--rw-r--r--   0        0        0     3271 2023-04-04 10:46:28.104042 spendpoint-0.2.0/tasks.py
--rw-r--r--   0        0        0        0 2023-04-04 10:57:35.360218 spendpoint-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0       57 2023-04-04 10:46:28.104042 spendpoint-0.2.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-04-04 10:57:35.360218 spendpoint-0.2.0/tests/fixtures/__init__.py
--rw-r--r--   0        0        0      116 2023-04-04 10:46:28.104042 spendpoint-0.2.0/tests/fixtures/state.py
--rw-r--r--   0        0        0     2590 2023-04-04 10:46:28.104042 spendpoint-0.2.0/tests/test_query_endpoint.py
--rw-r--r--   0        0        0     1939 1970-01-01 00:00:00.000000 spendpoint-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      103 2023-04-04 10:46:28.100041 spendpoint-0.3.0/.dockerignore
+-rw-r--r--   0        0        0      274 2023-04-04 10:46:28.100041 spendpoint-0.3.0/.editorconfig
+-rw-r--r--   0        0        0      121 2023-05-16 13:05:47.269693 spendpoint-0.3.0/.gitignore
+-rw-r--r--   0        0        0     2346 2023-05-16 13:05:47.269693 spendpoint-0.3.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0      178 2023-04-04 10:46:28.100041 spendpoint-0.3.0/AUTHORS.rst
+-rw-r--r--   0        0        0      387 2023-04-04 10:46:28.100041 spendpoint-0.3.0/Dockerfile
+-rw-r--r--   0        0        0      408 2023-05-16 18:43:41.012519 spendpoint-0.3.0/HISTORY.rst
+-rw-r--r--   0        0        0     1081 2023-04-04 10:46:28.100041 spendpoint-0.3.0/LICENSE
+-rw-r--r--   0        0        0      957 2023-05-16 18:43:41.012519 spendpoint-0.3.0/README.rst
+-rw-r--r--   0        0        0      495 2023-05-16 18:43:41.012519 spendpoint-0.3.0/data/configuration.toml
+-rw-r--r--   0        0        0      315 2023-05-16 13:05:47.269693 spendpoint-0.3.0/default.nix
+-rw-r--r--   0        0        0     1054 2023-04-04 10:46:28.104042 spendpoint-0.3.0/docs/templates/pyproject.toml
+-rw-r--r--   0        0        0     1236 2023-05-16 18:43:41.012519 spendpoint-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      560 2023-05-16 18:43:41.012519 spendpoint-0.3.0/requirements.txt
+-rw-r--r--   0        0        0      178 2023-05-16 18:43:41.016519 spendpoint-0.3.0/spendpoint/__init__.py
+-rw-r--r--   0        0        0      776 2023-05-16 18:43:41.016519 spendpoint-0.3.0/spendpoint/__main__.py
+-rw-r--r--   0        0        0     1492 2023-05-16 18:43:41.016519 spendpoint-0.3.0/spendpoint/bridge.py
+-rw-r--r--   0        0        0      569 2023-05-16 18:43:41.016519 spendpoint-0.3.0/spendpoint/configuration.py
+-rw-r--r--   0        0        0     8767 2023-05-16 18:43:41.016519 spendpoint-0.3.0/spendpoint/endpoint.py
+-rw-r--r--   0        0        0      691 2023-05-16 18:43:41.016519 spendpoint-0.3.0/spendpoint/main.py
+-rw-r--r--   0        0        0     4334 2023-05-16 18:43:41.016519 spendpoint-0.3.0/spendpoint/service.py
+-rw-r--r--   0        0        0     3266 2023-05-16 13:05:47.269693 spendpoint-0.3.0/tasks.py
+-rw-r--r--   0        0        0        0 2023-05-16 18:55:31.614071 spendpoint-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0       57 2023-04-04 10:46:28.104042 spendpoint-0.3.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-05-16 18:55:31.614071 spendpoint-0.3.0/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0      116 2023-04-04 10:46:28.104042 spendpoint-0.3.0/tests/fixtures/state.py
+-rw-r--r--   0        0        0     2590 2023-04-04 10:46:28.104042 spendpoint-0.3.0/tests/test_query_endpoint.py
+-rw-r--r--   0        0        0     2459 1970-01-01 00:00:00.000000 spendpoint-0.3.0/PKG-INFO
```

### Comparing `spendpoint-0.2.0/LICENSE` & `spendpoint-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spendpoint-0.2.0/docs/templates/pyproject.toml` & `spendpoint-0.3.0/docs/templates/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spendpoint-0.2.0/requirements.txt` & `spendpoint-0.3.0/requirements.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # SpEndPoint
+toml              ~= 0.10.2
 arklog            ~= 0.5.1
-rdflib            ~= 6.2.0
-pandas            ~= 1.5.3
-fastapi           ~= 0.94.0
-pyarrow           ~= 11.0.0
-requests          ~= 2.28.2
-starlette         ~= 0.26.0.post1
+rdflib            ~= 6.3.2
+pandas            ~= 2.0.1
+dacite            ~= 1.8.1
+fastapi           ~= 0.95.2
+pyarrow           ~= 12.0.0
+requests          ~= 2.30.0
+starlette         ~= 0.27
 python-magic      ~= 0.4.27
-uvicorn[standard] ~= 0.21.0
+uvicorn[standard] ~= 0.22.0
 # Test
-pytest        ~= 7.2.2
+pytest        ~= 7.3.1
 sparqlwrapper ~= 2.0.0
 # Doc
-sphinx ~= 6.1.3
+sphinx ~= 7.0.1
 # Dev
-tox      ~= 4.4.7
-pip      ~= 23.0.1
-flit     ~= 3.8.0
+tox      ~= 4.5.1
+pip      ~= 23.1.2
+flit     ~= 3.9.0
 twine    ~= 4.0.2
-numpy    ~= 1.24.2
-invoke   ~= 2.0.0
+numpy    ~= 1.24.3
+invoke   ~= 2.1.2
 jinja2   ~= 3.1.2
 flake8   ~= 6.0.0
-coverage ~= 7.2.1
+coverage ~= 7.2.5
```

### Comparing `spendpoint-0.2.0/spendpoint/bridge.py` & `spendpoint-0.3.0/spendpoint/bridge.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,29 +3,24 @@
 import requests
 from rdflib import Graph
 from typing import Union
 
 arklog.set_config_logging()
 
 
-def fetch_outliers(
-        file_name: str = "rotation.csv",
-        column: Union[str, int] = 2,
-        iri: str = "<http://ua.be/drivetrain/description/artifacts/artifacts#drivetrain-sensor-data-v1>"
-    ) -> Graph:
+def fetch_outliers(file_name: str, column: Union[str, int], iri: str, outlier_service_url: str) -> Graph:
     """"""
-    outlier_service_url = "http://127.0.0.1:9090/api/csv/outlier"
     try:
         column = column if isinstance(column, int) else int(column)
     except ValueError as e:
         logging.error(f"Column '{column}' is not parseable to an integer.")
         raise
     parameters = {"iri": iri, "column" : column, "file" : file_name}
     try:
-        outliers_result = requests.post(outlier_service_url, json=parameters, timeout=5)
+        outliers_result = requests.post(outlier_service_url, json=parameters, timeout=60)
         outliers_result.raise_for_status()
     except requests.exceptions.InvalidSchema as e:
         logging.error(f"Invalid schema for '{outlier_service_url}'.")
         raise
     except requests.exceptions.ConnectTimeout as e:
         logging.error(f"Request for '{outlier_service_url}' timed out.")
         raise
```

### Comparing `spendpoint-0.2.0/spendpoint/endpoint.py` & `spendpoint-0.3.0/spendpoint/endpoint.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 # Copied and modified from https://pypi.org/project/rdflib-endpoint/
 
 import logging
 import re
 import arklog
 import rdflib
-from typing import Any, Callable, Dict, List, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 from urllib import parse
 from fastapi import FastAPI, Query, Request, Response
 from fastapi.responses import JSONResponse
 from rdflib import ConjunctiveGraph, Dataset, Graph, Literal, URIRef
 from rdflib.plugins.sparql import prepareQuery
 from rdflib.plugins.sparql.evaluate import evalPart
 from rdflib.plugins.sparql.evalutils import _eval
 from rdflib.plugins.sparql.parserutils import CompValue
 from rdflib.plugins.sparql.sparql import QueryContext, SPARQLError
 
+from spendpoint import service
+
 arklog.set_config_logging()
 
 
 class SparqlEndpoint(FastAPI):
     """SPARQL endpoint for services and storage of heterogeneous data."""
 
     @staticmethod
@@ -53,21 +55,21 @@
             return "application/xml"
         if operation == "Construct Query" and (self.is_json_mime_type(output_mime_type) or self.is_csv_mime_type(output_mime_type)):
             return "text/turtle"
         if operation == "Construct Query" and output_mime_type == "application/xml":
             return "application/rdf+xml"
         return output_mime_type
 
-    def __init__(self, *args: Any, title: str, description: str, version: str, functions: Dict[str, Callable[..., Any]], graph: Union[Graph, ConjunctiveGraph, Dataset] = ConjunctiveGraph(), **kwargs: Any):
+    def __init__(self, *args: Any, title: str, description: str, version: str, configuration, graph: Union[Graph, ConjunctiveGraph, Dataset] = ConjunctiveGraph(), **kwargs: Any):
         """"""
         self.graph = graph
-        self.functions = functions
         self.title = title
         self.description = description
         self.version = version
+        self.configuration = configuration
         super().__init__(*args, title=title, description=description, version=version, **kwargs)
         logging.debug(self.description)
         rdflib.plugins.sparql.CUSTOM_EVALS["evalCustomFunctions"] = self.eval_custom_functions
         api_responses: Optional[Dict[Union[int, str], Dict[str, Any]]] = {
             200: {
                 "description": "SPARQL query results",
                 "content": {
@@ -162,20 +164,18 @@
             raise NotImplementedError()
 
         query_results = []
         logging.debug("Custom evaluation.")
         for eval_part in evalPart(ctx, part.p):
             # Checks if the function is a URI (custom function)
             if hasattr(part.expr, "iri"):
-                # Iterate through the custom functions passed in the constructor
-                for function_uri, custom_function in self.functions.items():
+                for conf_service in self.configuration.services:
                     # Check if URI correspond to a registered custom function
-                    if part.expr.iri == URIRef(function_uri):
-                        # Execute each function
-                        query_results, ctx, part, eval_part = custom_function(query_results, ctx, part, eval_part)
+                    if part.expr.iri == URIRef(conf_service.namespace):
+                        query_results, ctx, part, eval_part = getattr(service, conf_service.call)(query_results, ctx, part, eval_part, conf_service)
             else:
                 # For built-in SPARQL functions (that are not URIs)
                 evaluation: List[Any] = [_eval(part.expr, eval_part.forget(ctx, _except=part._vars))]
                 if isinstance(evaluation[0], SPARQLError):
                     raise evaluation[0]
                 # Append results for built-in SPARQL functions
                 for result in evaluation:
```

### Comparing `spendpoint-0.2.0/spendpoint/service.py` & `spendpoint-0.3.0/spendpoint/service.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 @dataclass(init=True, repr=True, order=False, frozen=True)
 class Outlier:
     iri: str
     value: str
 
-def outlier_service(query_results, ctx, part, eval_part):
+def outlier_service(query_results, ctx, part, eval_part, service_configuration):
     """
 
     Example query:
     PREFIX xsd: <http://www.w3.org/2001/XMLSchema#>
     PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
     PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
     PREFIX dtf:  <https://ontology.rys.app/dt/function/>
@@ -35,34 +35,36 @@
       }
     }
 
     :param query_results:
     :param ctx:
     :param part:
     :param eval_part:
+    :param service_configuration:
     :return:
     """
-    logging.debug(f"Outlier service.")
+    logging.debug(f"Outlier service '{service_configuration.namespace}'.")
     file_name = str(_eval(part.expr.expr[0], eval_part.forget(ctx, _except=part.expr._vars)))
     column = str(_eval(part.expr.expr[1], eval_part.forget(ctx, _except=part.expr._vars)))
     iri = str(_eval(part.expr.expr[2], eval_part.forget(ctx, _except=part.expr._vars)))
     logging.info(f"Looking for outlier in '{file_name}' at column '{column}' for '{iri}'.")
-    outlier_graph = fetch_outliers(file_name, column, iri)
+    outlier_graph = fetch_outliers(file_name, column, iri, service_configuration.endpoint)
     for stmt in outlier_graph:
         query_results.append(eval_part.merge({
             part.var: stmt[0],
             rdflib.term.Variable(part.var + "_relation") : stmt[1],
             rdflib.term.Variable(part.var + "_value") : stmt[2],
         }))
+    logging.debug(f"{query_results=}")
     return query_results, ctx, part, eval_part
 
 
-def conversion_service(query_results, ctx, part, eval_part):
+def conversion_service(query_results, ctx, part, eval_part, service_configuration):
     """"""
-    logging.debug(f"Conversion service.")
+    logging.debug(f"Conversion service '{service_configuration.namespace}'.")
     input_file_name = str(_eval(part.expr.expr[0], eval_part.forget(ctx, _except=part.expr._vars)))
     output_file_name = str(_eval(part.expr.expr[1], eval_part.forget(ctx, _except=part.expr._vars)))
     data_dir = Path(__file__).resolve().parent.parent / Path("data")
     input_file_path = data_dir / Path(input_file_name)
     output_file_path = data_dir / Path(output_file_name)
     success = False
     start_time = timer()
@@ -78,15 +80,15 @@
         rdflib.term.Variable(part.var + "_duration") : Literal(end_time - start_time, datatype=XSD.duration),
         rdflib.term.Variable(part.var + "_success") : Literal(success),
     }))
     return query_results, ctx, part, eval_part
 
 
 
-def example_service(query_results, ctx, part, eval_part):
+def example_service(query_results, ctx, part, eval_part, service_configuration):
     """"""
     logging.debug(f"{query_results=}")
     logging.debug(f"{ctx=}")
     logging.debug(f"{part=}")
     logging.debug(f"{eval_part=}")
 
     file_name = str(_eval(part.expr.expr[0], eval_part.forget(ctx, _except=part.expr._vars)))
```

### Comparing `spendpoint-0.2.0/tasks.py` & `spendpoint-0.3.0/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,16 @@
     c.run("python3 -m unittest discover tests 'test_*' -v")
 
 
 @task(name="migrate")
 def migrate_requirements(c):
     """Copy requirements from the requirements.txt file to pyproject.toml."""
     lines = Path("requirements.txt").read_text().split("\n")
-    requirements = {"spendpoint": [], "test": [], "doc": [], "dev": []}
     current = "spendpoint"
+    requirements = {current: [], "test": [], "doc": [], "dev": []}
     for line in lines:
         if line.startswith("#"):
             candidate = line[1:].lower().strip()
             if candidate in requirements.keys():
                 current = candidate
                 continue
         if line.strip() == "":
```

### Comparing `spendpoint-0.2.0/tests/test_query_endpoint.py` & `spendpoint-0.3.0/tests/test_query_endpoint.py`

 * *Files identical despite different names*

### Comparing `spendpoint-0.2.0/PKG-INFO` & `spendpoint-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 Metadata-Version: 2.1
 Name: spendpoint
-Version: 0.2.0
+Version: 0.3.0
 Summary: SPARQL endpoint for ontologies.
 Keywords: spendpoint
 Author-email: Arkadiusz Michał Ryś <Arkadiusz.Michal.Rys@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
+Requires-Dist: toml~=0.10.2
 Requires-Dist: arklog~=0.5.1
-Requires-Dist: rdflib~=6.2.0
-Requires-Dist: pandas~=1.5.3
-Requires-Dist: fastapi~=0.94.0
-Requires-Dist: pyarrow~=11.0.0
-Requires-Dist: requests~=2.28.2
-Requires-Dist: starlette~=0.26.0.post1
+Requires-Dist: rdflib~=6.3.2
+Requires-Dist: pandas~=2.0.1
+Requires-Dist: dacite~=1.8.1
+Requires-Dist: fastapi~=0.95.2
+Requires-Dist: pyarrow~=12.0.0
+Requires-Dist: requests~=2.30.0
+Requires-Dist: starlette~=0.27
 Requires-Dist: python-magic~=0.4.27
-Requires-Dist: uvicorn[standard]~=0.21.0
-Requires-Dist: tox~=4.4.7 ; extra == "dev"
-Requires-Dist: pip~=23.0.1 ; extra == "dev"
-Requires-Dist: flit~=3.8.0 ; extra == "dev"
+Requires-Dist: uvicorn[standard]~=0.22.0
+Requires-Dist: tox~=4.5.1 ; extra == "dev"
+Requires-Dist: pip~=23.1.2 ; extra == "dev"
+Requires-Dist: flit~=3.9.0 ; extra == "dev"
 Requires-Dist: twine~=4.0.2 ; extra == "dev"
-Requires-Dist: numpy~=1.24.2 ; extra == "dev"
-Requires-Dist: invoke~=2.0.0 ; extra == "dev"
+Requires-Dist: numpy~=1.24.3 ; extra == "dev"
+Requires-Dist: invoke~=2.1.2 ; extra == "dev"
 Requires-Dist: jinja2~=3.1.2 ; extra == "dev"
 Requires-Dist: flake8~=6.0.0 ; extra == "dev"
-Requires-Dist: coverage~=7.2.1 ; extra == "dev"
-Requires-Dist: sphinx~=6.1.3 ; extra == "doc"
-Requires-Dist: pytest~=7.2.2 ; extra == "test"
+Requires-Dist: coverage~=7.2.5 ; extra == "dev"
+Requires-Dist: sphinx~=7.0.1 ; extra == "doc"
+Requires-Dist: pytest~=7.3.1 ; extra == "test"
 Requires-Dist: sparqlwrapper~=2.0.0 ; extra == "test"
 Project-URL: source, https://git.rys.one/dtdesign/spendpoint
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: test
 
 ##########
@@ -48,21 +50,31 @@
 
 .. code-block::
 
    dtf:outlier
    dtf:example
    dtf:conversion
 
+The outlier service relies on `another endpoint <https://msdl.uantwerpen.be/git/lucasalbertins/DTDesign/src/main/tools/typeOperations>`_ which needs to be set up and accessible.
+
 Installation
 ------------
 
 ..
    .. code-block:: shell
 
       pip install spendpoint
 
    or
 
 .. code-block:: shell
 
    pip install --index-url https://pip:glpat-m8mNfhxZAUnWvy7rLS1x@git.rys.one/api/v4/projects/262/packages/pypi/simple --no-deps spendpoint
 
+Configuration
+-------------
+
+A configuration file at `data/configuration.toml` holds all user configurable data.
+You can set the `host` and `port` the server will listen on.
+A more advanced use is to import extra services.
+These services need to be defined in the `service.py` file as well.
+
```

