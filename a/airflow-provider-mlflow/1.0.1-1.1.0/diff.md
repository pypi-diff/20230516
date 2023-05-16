# Comparing `tmp/airflow-provider-mlflow-1.0.1.tar.gz` & `tmp/airflow-provider-mlflow-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow-provider-mlflow-1.0.1.tar", last modified: Tue Apr 11 19:05:15 2023, max compression
+gzip compressed data, was "airflow-provider-mlflow-1.1.0.tar", last modified: Tue May 16 18:00:21 2023, max compression
```

## Comparing `airflow-provider-mlflow-1.0.1.tar` & `airflow-provider-mlflow-1.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:05:15.552349 airflow-provider-mlflow-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-11 19:05:06.000000 airflow-provider-mlflow-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-04-11 19:05:15.552349 airflow-provider-mlflow-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-04-11 19:05:06.000000 airflow-provider-mlflow-1.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:05:15.552349 airflow-provider-mlflow-1.0.1/airflow_provider_mlflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-04-11 19:05:15.000000 airflow-provider-mlflow-1.0.1/airflow_provider_mlflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-11 19:05:15.000000 airflow-provider-mlflow-1.0.1/airflow_provider_mlflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 19:05:15.000000 airflow-provider-mlflow-1.0.1/airflow_provider_mlflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 19:05:15.000000 airflow-provider-mlflow-1.0.1/airflow_provider_mlflow.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-11 19:05:15.000000 airflow-provider-mlflow-1.0.1/airflow_provider_mlflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-11 19:05:15.000000 airflow-provider-mlflow-1.0.1/airflow_provider_mlflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:05:15.552349 airflow-provider-mlflow-1.0.1/mlflow_provider/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-11 19:05:06.000000 airflow-provider-mlflow-1.0.1/mlflow_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 19:05:06.000000 airflow-provider-mlflow-1.0.1/mlflow_provider/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:05:15.552349 airflow-provider-mlflow-1.0.1/mlflow_provider/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 19:05:06.000000 airflow-provider-mlflow-1.0.1/mlflow_provider/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-11 19:05:06.000000 airflow-provider-mlflow-1.0.1/mlflow_provider/hooks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-04-11 19:05:06.000000 airflow-provider-mlflow-1.0.1/mlflow_provider/hooks/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-04-11 19:05:06.000000 airflow-provider-mlflow-1.0.1/mlflow_provider/hooks/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-11 19:05:06.000000 airflow-provider-mlflow-1.0.1/mlflow_provider/hooks/pyfunc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:05:15.552349 airflow-provider-mlflow-1.0.1/mlflow_provider/operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 19:05:06.000000 airflow-provider-mlflow-1.0.1/mlflow_provider/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-04-11 19:05:06.000000 airflow-provider-mlflow-1.0.1/mlflow_provider/operators/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-04-11 19:05:06.000000 airflow-provider-mlflow-1.0.1/mlflow_provider/operators/pyfunc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16596 2023-04-11 19:05:06.000000 airflow-provider-mlflow-1.0.1/mlflow_provider/operators/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-11 19:05:15.552349 airflow-provider-mlflow-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 19:05:06.000000 airflow-provider-mlflow-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:00:21.446771 airflow-provider-mlflow-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-16 18:00:09.000000 airflow-provider-mlflow-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-16 18:00:21.446771 airflow-provider-mlflow-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-16 18:00:09.000000 airflow-provider-mlflow-1.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:00:21.442771 airflow-provider-mlflow-1.1.0/airflow_provider_mlflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-16 18:00:21.000000 airflow-provider-mlflow-1.1.0/airflow_provider_mlflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-16 18:00:21.000000 airflow-provider-mlflow-1.1.0/airflow_provider_mlflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 18:00:21.000000 airflow-provider-mlflow-1.1.0/airflow_provider_mlflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 18:00:21.000000 airflow-provider-mlflow-1.1.0/airflow_provider_mlflow.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 18:00:21.000000 airflow-provider-mlflow-1.1.0/airflow_provider_mlflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 18:00:21.000000 airflow-provider-mlflow-1.1.0/airflow_provider_mlflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:00:21.442771 airflow-provider-mlflow-1.1.0/mlflow_provider/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-16 18:00:09.000000 airflow-provider-mlflow-1.1.0/mlflow_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:00:09.000000 airflow-provider-mlflow-1.1.0/mlflow_provider/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:00:21.446771 airflow-provider-mlflow-1.1.0/mlflow_provider/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:00:09.000000 airflow-provider-mlflow-1.1.0/mlflow_provider/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-05-16 18:00:09.000000 airflow-provider-mlflow-1.1.0/mlflow_provider/hooks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-05-16 18:00:09.000000 airflow-provider-mlflow-1.1.0/mlflow_provider/hooks/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-05-16 18:00:09.000000 airflow-provider-mlflow-1.1.0/mlflow_provider/hooks/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-16 18:00:09.000000 airflow-provider-mlflow-1.1.0/mlflow_provider/hooks/pyfunc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:00:21.446771 airflow-provider-mlflow-1.1.0/mlflow_provider/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:00:09.000000 airflow-provider-mlflow-1.1.0/mlflow_provider/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-16 18:00:09.000000 airflow-provider-mlflow-1.1.0/mlflow_provider/operators/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-05-16 18:00:09.000000 airflow-provider-mlflow-1.1.0/mlflow_provider/operators/pyfunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16596 2023-05-16 18:00:09.000000 airflow-provider-mlflow-1.1.0/mlflow_provider/operators/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-16 18:00:21.446771 airflow-provider-mlflow-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 18:00:09.000000 airflow-provider-mlflow-1.1.0/setup.py
```

### Comparing `airflow-provider-mlflow-1.0.1/LICENSE` & `airflow-provider-mlflow-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow-provider-mlflow-1.0.1/PKG-INFO` & `airflow-provider-mlflow-1.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-provider-mlflow
-Version: 1.0.1
+Version: 1.1.0
 Summary: Apache Airflow provider for MLflow
 Home-page: https://github.com/astronomer/airflow-provider-mlflow
 Author: Faisal Hoda
 Author-email: faisal@astronomer.io
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/astronomer/airflow-provider-mlflow
 Project-URL: Homepage, https://github.com/astronomer/airflow-provider-mlflow
@@ -24,14 +24,27 @@
 Requires-Python: >=3.8
 Provides-Extra: dev
 License-File: LICENSE
 
 MLflow Provider Package for Apache Airflow
 ==========================================
 
+.. image:: https://badge.fury.io/py/airflow-provider-mlflow.svg
+    :target: https://badge.fury.io/py/airflow-provider-mlflow
+    :alt: PyPI Version
+.. image:: https://img.shields.io/pypi/pyversions/airflow-provider-mlflow
+    :target: https://img.shields.io/pypi/pyversions/airflow-provider-mlflow
+    :alt: PyPI - Python Version
+.. image:: https://readthedocs.org/projects/airflow-provider-mlflow/badge/?version=latest
+    :target: https://airflow-provider-mlflow.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+.. image:: https://img.shields.io/pypi/l/astronomer-providers?color=blue
+    :target: https://img.shields.io/pypi/l/astronomer-providers?color=blue
+    :alt: PyPI - License
+
 An `Apache Airflow <https://airflow.apache.org/>`_ provider to interact with MLflow using Operators and Hooks for the following:
 
 - Registry
 - Deployments
 - Pyfunc
 
 https://mlflow.org/docs/latest/index.html
```

### Comparing `airflow-provider-mlflow-1.0.1/airflow_provider_mlflow.egg-info/PKG-INFO` & `airflow-provider-mlflow-1.1.0/airflow_provider_mlflow.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-provider-mlflow
-Version: 1.0.1
+Version: 1.1.0
 Summary: Apache Airflow provider for MLflow
 Home-page: https://github.com/astronomer/airflow-provider-mlflow
 Author: Faisal Hoda
 Author-email: faisal@astronomer.io
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/astronomer/airflow-provider-mlflow
 Project-URL: Homepage, https://github.com/astronomer/airflow-provider-mlflow
@@ -24,14 +24,27 @@
 Requires-Python: >=3.8
 Provides-Extra: dev
 License-File: LICENSE
 
 MLflow Provider Package for Apache Airflow
 ==========================================
 
+.. image:: https://badge.fury.io/py/airflow-provider-mlflow.svg
+    :target: https://badge.fury.io/py/airflow-provider-mlflow
+    :alt: PyPI Version
+.. image:: https://img.shields.io/pypi/pyversions/airflow-provider-mlflow
+    :target: https://img.shields.io/pypi/pyversions/airflow-provider-mlflow
+    :alt: PyPI - Python Version
+.. image:: https://readthedocs.org/projects/airflow-provider-mlflow/badge/?version=latest
+    :target: https://airflow-provider-mlflow.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+.. image:: https://img.shields.io/pypi/l/astronomer-providers?color=blue
+    :target: https://img.shields.io/pypi/l/astronomer-providers?color=blue
+    :alt: PyPI - License
+
 An `Apache Airflow <https://airflow.apache.org/>`_ provider to interact with MLflow using Operators and Hooks for the following:
 
 - Registry
 - Deployments
 - Pyfunc
 
 https://mlflow.org/docs/latest/index.html
```

### Comparing `airflow-provider-mlflow-1.0.1/airflow_provider_mlflow.egg-info/SOURCES.txt` & `airflow-provider-mlflow-1.1.0/airflow_provider_mlflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `airflow-provider-mlflow-1.0.1/mlflow_provider/hooks/base.py` & `airflow-provider-mlflow-1.1.0/mlflow_provider/hooks/base.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-mlflow-1.0.1/mlflow_provider/hooks/client.py` & `airflow-provider-mlflow-1.1.0/mlflow_provider/hooks/client.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-mlflow-1.0.1/mlflow_provider/hooks/deployment.py` & `airflow-provider-mlflow-1.1.0/mlflow_provider/hooks/deployment.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-mlflow-1.0.1/mlflow_provider/hooks/pyfunc.py` & `airflow-provider-mlflow-1.1.0/mlflow_provider/hooks/pyfunc.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-mlflow-1.0.1/mlflow_provider/operators/deployment.py` & `airflow-provider-mlflow-1.1.0/mlflow_provider/operators/deployment.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-mlflow-1.0.1/mlflow_provider/operators/pyfunc.py` & `airflow-provider-mlflow-1.1.0/mlflow_provider/operators/pyfunc.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,18 +3,16 @@
 from tempfile import TemporaryDirectory
 from typing import Any, Dict, Union, List, Sequence
 
 from numpy import ndarray
 from pandas.core.frame import DataFrame
 from pandas.core.series import Series
 from airflow.exceptions import AirflowException
-from airflow.hooks.base import BaseHook
 from airflow.operators.python import _BasePythonVirtualenvOperator
 from airflow.utils import python_virtualenv
-from airflow.utils.decorators import apply_defaults
 from scipy.sparse import csc_matrix, csr_matrix
 
 from mlflow_provider.hooks.pyfunc import MLflowPyfuncHook
 
 
 def _model_load_and_predict(
         host,
@@ -114,45 +112,42 @@
         'data',
         "op_args", "op_kwargs"
     )
     template_fields_renderers = {"op_args": "py", "op_kwargs": "py"}
     template_ext = ()
     ui_color = '#f4a460'
 
-    @apply_defaults
     def __init__(
             self,
             *,
             mlflow_conn_id: str = 'mlflow_default',
             model_uri: str,
             suppress_warnings: bool = False,
             dst_path: str | None = None,
             data: Union[DataFrame, Series, ndarray, csc_matrix, csr_matrix, List[Any], Dict[str, Any]],
-            # python_callable: Optional[Callable] = _model_load_and_predict,
             **kwargs: Any
     ) -> None:
         self.requirements = None
         self.system_site_packages = False
         self.mlflow_conn_id = mlflow_conn_id
         self.model_uri = model_uri
         self.suppress_warnings = suppress_warnings
         self.dst_path = dst_path
         self.data = data
-        self.conn = BaseHook.get_connection(self.mlflow_conn_id)
         if kwargs.get('xcom_push') is not None:
             raise AirflowException(
                 "'xcom_push' was deprecated, use 'BaseOperator.do_xcom_push' instead")
         super().__init__(
             python_callable=_model_load_and_predict,
             use_dill=False,
             op_args=None,
             op_kwargs={
-                'host':self.conn.host,
-                'login':self.conn.login,
-                'password':self.conn.password,
+                "host": f"{{{{ conn.{self.mlflow_conn_id}.host }}}}",
+                "login": f"{{{{ conn.{self.mlflow_conn_id}.login }}}}",
+                "password": f"{{{{ conn.{self.mlflow_conn_id}.password }}}}",
                 'model_uri':self.model_uri,
                 'suppress_warnings':self.suppress_warnings,
                 'dst_path':self.dst_path,
                 'data':self.data,
             },
             string_args=None,
             templates_dict=None,
```

### Comparing `airflow-provider-mlflow-1.0.1/mlflow_provider/operators/registry.py` & `airflow-provider-mlflow-1.1.0/mlflow_provider/operators/registry.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-mlflow-1.0.1/setup.cfg` & `airflow-provider-mlflow-1.1.0/setup.cfg`

 * *Files identical despite different names*

