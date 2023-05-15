# Comparing `tmp/flytekitplugins-papermill-1.6.0b4.tar.gz` & `tmp/flytekitplugins-papermill-1.6.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-papermill-1.6.0b4.tar", last modified: Tue May  9 00:42:38 2023, max compression
+gzip compressed data, was "flytekitplugins-papermill-1.6.1b0.tar", last modified: Mon May 15 22:07:09 2023, max compression
```

## Comparing `flytekitplugins-papermill-1.6.0b4.tar` & `flytekitplugins-papermill-1.6.1b0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:38.888773 flytekitplugins-papermill-1.6.0b4/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-09 00:42:38.888773 flytekitplugins-papermill-1.6.0b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-09 00:42:15.000000 flytekitplugins-papermill-1.6.0b4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:38.888773 flytekitplugins-papermill-1.6.0b4/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:38.888773 flytekitplugins-papermill-1.6.0b4/flytekitplugins/papermill/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-09 00:42:15.000000 flytekitplugins-papermill-1.6.0b4/flytekitplugins/papermill/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12932 2023-05-09 00:42:15.000000 flytekitplugins-papermill-1.6.0b4/flytekitplugins/papermill/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:38.888773 flytekitplugins-papermill-1.6.0b4/flytekitplugins_papermill.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-09 00:42:38.000000 flytekitplugins-papermill-1.6.0b4/flytekitplugins_papermill.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-09 00:42:38.000000 flytekitplugins-papermill-1.6.0b4/flytekitplugins_papermill.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 00:42:38.000000 flytekitplugins-papermill-1.6.0b4/flytekitplugins_papermill.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 00:42:38.000000 flytekitplugins-papermill-1.6.0b4/flytekitplugins_papermill.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-09 00:42:38.000000 flytekitplugins-papermill-1.6.0b4/flytekitplugins_papermill.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 00:42:38.000000 flytekitplugins-papermill-1.6.0b4/flytekitplugins_papermill.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 00:42:38.888773 flytekitplugins-papermill-1.6.0b4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-09 00:42:30.000000 flytekitplugins-papermill-1.6.0b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:09.075792 flytekitplugins-papermill-1.6.1b0/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-15 22:07:09.075792 flytekitplugins-papermill-1.6.1b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-15 22:06:44.000000 flytekitplugins-papermill-1.6.1b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:09.071792 flytekitplugins-papermill-1.6.1b0/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:09.071792 flytekitplugins-papermill-1.6.1b0/flytekitplugins/papermill/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-15 22:06:44.000000 flytekitplugins-papermill-1.6.1b0/flytekitplugins/papermill/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15374 2023-05-15 22:06:44.000000 flytekitplugins-papermill-1.6.1b0/flytekitplugins/papermill/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:09.075792 flytekitplugins-papermill-1.6.1b0/flytekitplugins_papermill.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-15 22:07:09.000000 flytekitplugins-papermill-1.6.1b0/flytekitplugins_papermill.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-15 22:07:09.000000 flytekitplugins-papermill-1.6.1b0/flytekitplugins_papermill.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 22:07:09.000000 flytekitplugins-papermill-1.6.1b0/flytekitplugins_papermill.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 22:07:09.000000 flytekitplugins-papermill-1.6.1b0/flytekitplugins_papermill.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-15 22:07:09.000000 flytekitplugins-papermill-1.6.1b0/flytekitplugins_papermill.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 22:07:09.000000 flytekitplugins-papermill-1.6.1b0/flytekitplugins_papermill.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 22:07:09.075792 flytekitplugins-papermill-1.6.1b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-15 22:07:00.000000 flytekitplugins-papermill-1.6.1b0/setup.py
```

### Comparing `flytekitplugins-papermill-1.6.0b4/PKG-INFO` & `flytekitplugins-papermill-1.6.1b0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-papermill
-Version: 1.6.0b4
+Version: 1.6.1b0
 Summary: This is the flytekit papermill plugin
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-papermill-1.6.0b4/README.md` & `flytekitplugins-papermill-1.6.1b0/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-papermill-1.6.0b4/flytekitplugins/papermill/task.py` & `flytekitplugins-papermill-1.6.1b0/flytekitplugins/papermill/task.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 import json
 import logging
 import os
 import sys
+import tempfile
 import typing
 from typing import Any
 
 import nbformat
 import papermill as pm
+from flyteidl.core.literals_pb2 import Literal as _pb2_Literal
 from flyteidl.core.literals_pb2 import LiteralMap as _pb2_LiteralMap
 from google.protobuf import text_format as _text_format
 from nbconvert import HTMLExporter
 
-from flytekit import FlyteContext, PythonInstanceTask
+from flytekit import FlyteContext, PythonInstanceTask, StructuredDataset
 from flytekit.configuration import SerializationSettings
+from flytekit.core import utils
 from flytekit.core.context_manager import ExecutionParameters
 from flytekit.deck.deck import Deck
 from flytekit.extend import Interface, TaskPlugins, TypeEngine
 from flytekit.loggers import logger
 from flytekit.models import task as task_models
-from flytekit.models.literals import LiteralMap
-from flytekit.types.file import HTMLPage, PythonNotebook
+from flytekit.models.literals import Literal, LiteralMap
+from flytekit.types.directory import FlyteDirectory
+from flytekit.types.file import FlyteFile, HTMLPage, PythonNotebook
 
 T = typing.TypeVar("T")
 
 
 def _dummy_task_func():
     return None
 
 
+SAVE_AS_LITERAL = (FlyteFile, FlyteDirectory, StructuredDataset)
+
 PAPERMILL_TASK_PREFIX = "pm.nb"
 
 
 class NotebookTask(PythonInstanceTask[T]):
     """
     Simple Papermill based input output handling for a Python Jupyter notebook. This task should be used to wrap
     a Notebook that has 2 properties
@@ -251,34 +257,39 @@
         """
         TODO: Figure out how to share FlyteContext ExecutionParameters with the notebook kernel (as notebook kernel
              is executed in a separate python process)
         For Spark, the notebooks today need to use the new_session or just getOrCreate session and get a handle to the
         singleton
         """
         logger.info(f"Hijacking the call for task-type {self.task_type}, to call notebook.")
+        for k, v in kwargs.items():
+            if isinstance(v, SAVE_AS_LITERAL):
+                kwargs[k] = save_python_val_to_file(v)
+
         # Execute Notebook via Papermill.
         pm.execute_notebook(self._notebook_path, self.output_notebook_path, parameters=kwargs, log_output=self._stream_logs)  # type: ignore
 
         outputs = self.extract_outputs(self.output_notebook_path)
         self.render_nb_html(self.output_notebook_path, self.rendered_output_path)
 
         m = {}
         if outputs:
             m = outputs.literals
         output_list = []
+
         for k, type_v in self.python_interface.outputs.items():
             if k == self._IMPLICIT_OP_NOTEBOOK:
                 output_list.append(self.output_notebook_path)
             elif k == self._IMPLICIT_RENDERED_NOTEBOOK:
                 output_list.append(self.rendered_output_path)
             elif k in m:
                 v = TypeEngine.to_python_value(ctx=FlyteContext.current_context(), lv=m[k], expected_python_type=type_v)
                 output_list.append(v)
             else:
-                raise RuntimeError(f"Expected output {k} of type {v} not found in the notebook outputs")
+                raise TypeError(f"Expected output {k} of type {type_v} not found in the notebook outputs")
 
         return tuple(output_list)
 
     def post_execute(self, user_params: ExecutionParameters, rval: Any) -> Any:
         if self._render_deck:
             nb_deck = Deck(self._IMPLICIT_RENDERED_NOTEBOOK)
             with open(self.rendered_output_path, "r") as f:
@@ -303,7 +314,84 @@
     m = {}
     ctx = FlyteContext.current_context()
     for k, v in kwargs.items():
         expected = TypeEngine.to_literal_type(type(v))
         lit = TypeEngine.to_literal(ctx, python_type=type(v), python_val=v, expected=expected)
         m[k] = lit
     return LiteralMap(literals=m).to_flyte_idl()
+
+
+def save_python_val_to_file(input: Any) -> str:
+    """Save a python value to a local file as a Flyte literal.
+
+    Args:
+        input (Any): the python value
+
+    Returns:
+        str: the path to the file
+    """
+    ctx = FlyteContext.current_context()
+    expected = TypeEngine.to_literal_type(type(input))
+    lit = TypeEngine.to_literal(ctx, python_type=type(input), python_val=input, expected=expected)
+
+    tmp_file = tempfile.mktemp(suffix="bin")
+    utils.write_proto_to_file(lit.to_flyte_idl(), tmp_file)
+    return tmp_file
+
+
+def load_python_val_from_file(path: str, dtype: T) -> T:
+    """Loads a python value from a Flyte literal saved to a local file.
+
+    If the path matches the type, it is returned as is. This enables
+    reusing the parameters cell for local development.
+
+    Args:
+        path (str): path to the file
+        dtype (T): the type of the literal
+
+    Returns:
+        T: the python value of the literal
+    """
+    if isinstance(path, dtype):
+        return path
+
+    proto = utils.load_proto_from_file(_pb2_Literal, path)
+    lit = Literal.from_flyte_idl(proto)
+    ctx = FlyteContext.current_context()
+    python_value = TypeEngine.to_python_value(ctx, lit, dtype)
+    return python_value
+
+
+def load_flytefile(path: str) -> T:
+    """Loads a FlyteFile from a file.
+
+    Args:
+        path (str): path to the file
+
+    Returns:
+        T: the python value of the literal
+    """
+    return load_python_val_from_file(path=path, dtype=FlyteFile)
+
+
+def load_flytedirectory(path: str) -> T:
+    """Loads a FlyteDirectory from a file.
+
+    Args:
+        path (str): path to the file
+
+    Returns:
+        T: the python value of the literal
+    """
+    return load_python_val_from_file(path=path, dtype=FlyteDirectory)
+
+
+def load_structureddataset(path: str) -> T:
+    """Loads a StructuredDataset from a file.
+
+    Args:
+        path (str): path to the file
+
+    Returns:
+        T: the python value of the literal
+    """
+    return load_python_val_from_file(path=path, dtype=StructuredDataset)
```

### Comparing `flytekitplugins-papermill-1.6.0b4/flytekitplugins_papermill.egg-info/PKG-INFO` & `flytekitplugins-papermill-1.6.1b0/flytekitplugins_papermill.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-papermill
-Version: 1.6.0b4
+Version: 1.6.1b0
 Summary: This is the flytekit papermill plugin
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-papermill-1.6.0b4/setup.py` & `flytekitplugins-papermill-1.6.1b0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 plugin_requires = [
     "flytekit>=1.3.0b2,<2.0.0",
     "papermill>=1.2.0",
     "nbconvert>=6.0.7",
     "ipykernel>=5.0.0",
 ]
 
-__version__ = "1.6.0b4"
+__version__ = "1.6.1b0"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This is the flytekit papermill plugin",
```

