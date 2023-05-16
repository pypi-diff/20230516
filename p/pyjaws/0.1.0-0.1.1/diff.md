# Comparing `tmp/pyjaws-0.1.0.tar.gz` & `tmp/pyjaws-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjaws-0.1.0.tar", last modified: Sun May 14 13:49:26 2023, max compression
+gzip compressed data, was "pyjaws-0.1.1.tar", last modified: Tue May 16 11:10:34 2023, max compression
```

## Comparing `pyjaws-0.1.0.tar` & `pyjaws-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 13:49:26.547489 pyjaws-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-05-14 13:49:26.547489 pyjaws-0.1.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 13:49:26.543489 pyjaws-0.1.0/pyjaws/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-14 13:49:15.000000 pyjaws-0.1.0/pyjaws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 13:49:26.547489 pyjaws-0.1.0/pyjaws/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 13:49:15.000000 pyjaws-0.1.0/pyjaws/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-05-14 13:49:15.000000 pyjaws-0.1.0/pyjaws/api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-14 13:49:15.000000 pyjaws-0.1.0/pyjaws/api/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-14 13:49:15.000000 pyjaws-0.1.0/pyjaws/api/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 13:49:26.547489 pyjaws-0.1.0/pyjaws/api/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 13:49:26.547489 pyjaws-0.1.0/pyjaws/api/templates/macros/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-14 13:49:15.000000 pyjaws-0.1.0/pyjaws/api/templates/macros/cluster.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-14 13:49:15.000000 pyjaws-0.1.0/pyjaws/api/templates/macros/task.j2
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-14 13:49:15.000000 pyjaws-0.1.0/pyjaws/api/templates/workflow.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 13:49:26.547489 pyjaws-0.1.0/pyjaws/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 13:49:15.000000 pyjaws-0.1.0/pyjaws/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-14 13:49:15.000000 pyjaws-0.1.0/pyjaws/client/entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 13:49:26.547489 pyjaws-0.1.0/pyjaws.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-05-14 13:49:26.000000 pyjaws-0.1.0/pyjaws.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-14 13:49:26.000000 pyjaws-0.1.0/pyjaws.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 13:49:26.000000 pyjaws-0.1.0/pyjaws.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-14 13:49:26.000000 pyjaws-0.1.0/pyjaws.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-14 13:49:26.000000 pyjaws-0.1.0/pyjaws.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-14 13:49:26.000000 pyjaws-0.1.0/pyjaws.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-14 13:49:15.000000 pyjaws-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 13:49:26.547489 pyjaws-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-14 13:49:15.000000 pyjaws-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:10:34.388727 pyjaws-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-05-16 11:10:34.388727 pyjaws-0.1.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:10:34.384726 pyjaws-0.1.1/pyjaws/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-16 11:10:19.000000 pyjaws-0.1.1/pyjaws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:10:34.384726 pyjaws-0.1.1/pyjaws/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:10:19.000000 pyjaws-0.1.1/pyjaws/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-05-16 11:10:19.000000 pyjaws-0.1.1/pyjaws/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-16 11:10:19.000000 pyjaws-0.1.1/pyjaws/api/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-16 11:10:19.000000 pyjaws-0.1.1/pyjaws/api/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-16 11:10:19.000000 pyjaws-0.1.1/pyjaws/api/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:10:34.384726 pyjaws-0.1.1/pyjaws/api/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:10:34.384726 pyjaws-0.1.1/pyjaws/api/templates/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-16 11:10:19.000000 pyjaws-0.1.1/pyjaws/api/templates/macros/cluster.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-16 11:10:19.000000 pyjaws-0.1.1/pyjaws/api/templates/macros/task.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-16 11:10:19.000000 pyjaws-0.1.1/pyjaws/api/templates/workflow.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:10:34.388727 pyjaws-0.1.1/pyjaws/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:10:19.000000 pyjaws-0.1.1/pyjaws/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-16 11:10:19.000000 pyjaws-0.1.1/pyjaws/client/entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:10:34.384726 pyjaws-0.1.1/pyjaws.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-05-16 11:10:34.000000 pyjaws-0.1.1/pyjaws.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-16 11:10:34.000000 pyjaws-0.1.1/pyjaws.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 11:10:34.000000 pyjaws-0.1.1/pyjaws.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-16 11:10:34.000000 pyjaws-0.1.1/pyjaws.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-16 11:10:34.000000 pyjaws-0.1.1/pyjaws.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-16 11:10:34.000000 pyjaws-0.1.1/pyjaws.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-16 11:10:19.000000 pyjaws-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 11:10:34.388727 pyjaws-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-16 11:10:19.000000 pyjaws-0.1.1/setup.py
```

### Comparing `pyjaws-0.1.0/PKG-INFO` & `pyjaws-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: pyjaws
-Version: 0.1.0
+Version: 0.1.1
 Author: Rafael Pierre
 Description-Content-Type: text/markdown
 
 # PyJaws: A Pythonic Way to Define Databricks Jobs and Workflows
 
 <p align="center">
         <img src="https://raw.githubusercontent.com/rafaelpierre/pyjaws/main/img/pyjaws.png" class="align-center" />
     </a>
 </p>
 
 <hr />
 
-[![pypi](https://img.shields.io/badge/pypi-0.0.9-brightgreen?style=for-the-badge)](https://pypi.org/project/pyjaws/) ![black](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge) ![ruff](https://img.shields.io/badge/lint-ruff-gold?style=for-the-badge) ![cov](https://raw.githubusercontent.com/rafaelpierre/pyjaws/main/img/coverage.svg) ![databricks](https://img.shields.io/badge/Databricks-FF3621.svg?style=for-the-badge&logo=Databricks&logoColor=white) ![Jinja](https://img.shields.io/badge/jinja-white.svg?style=for-the-badge&logo=jinja&logoColor=black)
+[![pypi](https://img.shields.io/badge/pypi-0.1.0-brightgreen?style=for-the-badge)](https://pypi.org/project/pyjaws/) ![black](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge) ![ruff](https://img.shields.io/badge/lint-ruff-gold?style=for-the-badge) ![cov](https://raw.githubusercontent.com/rafaelpierre/pyjaws/main/img/coverage.svg) ![databricks](https://img.shields.io/badge/Databricks-FF3621.svg?style=for-the-badge&logo=Databricks&logoColor=white) ![Jinja](https://img.shields.io/badge/jinja-white.svg?style=for-the-badge&logo=jinja&logoColor=black)
 
 <hr />
 
 * **PyJaws** enables declaring [Databricks Jobs and Workflows](https://docs.databricks.com/workflows/index.html) as Python code, allowing for:
-   * Code Linting
-   * Formatting
-   * Parameter Validation
-   * Modularity and reusability
+  * Code Linting
+  * Formatting
+  * Parameter Validation
+  * Modularity and reusability
 * In addition to those, **PyJaws** also provides some nice features such as [cycle detection](https://networkx.org/documentation/stable/reference/algorithms/cycles.html) out of the box.
 
 Folks who have used Python-based orchestration tools such as [Apache Airflow](https://airflow.apache.org/), [Luigi](https://luigi.readthedocs.io/en/stable/) and [Mage](https://pypi.org/project/mage-ai/) will be familiar with the concepts and the API if **PyJaws**.
 
 * **PyJaws** leverages some existing libraries in order to allow for **modularisation**, **reusability** and **validation**, such as:
-    * [Click](https://click.palletsprojects.com/en/8.1.x/) - for providing a rich CLI functionality
-    * [Pydantic](https://docs.pydantic.dev/latest/) - for efficient parameter validation
-    * [NetworkX](https://networkx.org/) - for Graph and Cycle Detection features
-    * [Jinja2](https://jinja.palletsprojects.com/en/3.1.x/) - for templating
+  * [Click](https://click.palletsprojects.com/en/8.1.x/) - for providing a rich CLI functionality
+  * [Pydantic](https://docs.pydantic.dev/latest/) - for efficient parameter validation
+  * [NetworkX](https://networkx.org/) - for Graph and Cycle Detection features
+  * [Jinja2](https://jinja.palletsprojects.com/en/3.1.x/) - for templating
 
 ## Documentation
 
 * Work in progress. Stay tuned!
 
 ## Development & Testing
 
@@ -63,17 +63,17 @@
 
 ### Sample Job Definition
 
 ```python
 from pyjaws.api.base import (
     Cluster,
     Runtime,
-    Task,
     Workflow
 )
+from pyjaws.api.tasks import PythonWheelTask
 
 cluster = Cluster(
     job_cluster_key = "ai_cluster",
     spark_version = Runtime.DBR_13_ML,
     num_workers = 2,
     node_type_id = "Standard_DS3_v2",
     cluster_log_conf = {
@@ -82,26 +82,26 @@
         }
     }
 )
 
 
 # Create a Task object.
 
-ingest_task = Task(
+ingest_task = PythonWheelTask(
     key = "ingest",
     cluster = cluster,
     entrypoint = "iot",
     task_name = "ingest",
     parameters = [
         f"my_parameter_value",
         "--output-table", "my_table"
     ]
 )
 
-transform_task = Task(
+transform_task = PythonWheelTask(
     key = "transform",
     cluster = cluster,
     entrypoint = "iot",
     task_name = "ingest",
     dependencies = [ingest_task],
     parameters = [
         f"my_parameter_value2",
```

### Comparing `pyjaws-0.1.0/pyjaws/api/base.py` & `pyjaws-0.1.1/pyjaws/api/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,30 +55,26 @@
         return self.job_cluster_key
 
     @property
     def cluster_log_conf_str(self) -> str:
         return json.dumps(self.cluster_log_conf)
 
 
-class Task(BaseModel):
+class BaseTask(BaseModel):
     """
     Base class for Husk Databricks Workflow Task.
     Params:
         key: Task key.
         existing_cluster_id: Cluster ID for running the task.
         libraries: List of Python libraries to be installed.
     """
 
     key: str
-    package_name: str
-    entrypoint: str
-    task_name: str
     cluster: Cluster
-    parameters: List[str] = []
-    dependencies: Optional[List[Task]] = None
+    dependencies: Optional[List[BaseTask]] = None
     libraries: Optional[List[dict]] = None
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
     def __str__(self):
         return self.key
@@ -92,15 +88,15 @@
         tasks: List of Workflow Tasks.
     """
 
     class Config:
         arbitrary_types_allowed = True
 
     name: str
-    tasks: List[Task]
+    tasks: List[BaseTask]
     tags: Optional[dict] = {}
     graph: nx.Graph = None
     schedule: Optional[str]
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
```

### Comparing `pyjaws-0.1.0/pyjaws/api/jobs.py` & `pyjaws-0.1.1/pyjaws/api/jobs.py`

 * *Files identical despite different names*

### Comparing `pyjaws-0.1.0/pyjaws/api/templates/macros/cluster.j2` & `pyjaws-0.1.1/pyjaws/api/templates/macros/cluster.j2`

 * *Files identical despite different names*

### Comparing `pyjaws-0.1.0/pyjaws/api/templates/workflow.j2` & `pyjaws-0.1.1/pyjaws/api/templates/workflow.j2`

 * *Files identical despite different names*

### Comparing `pyjaws-0.1.0/pyjaws/client/entrypoint.py` & `pyjaws-0.1.1/pyjaws/client/entrypoint.py`

 * *Files identical despite different names*

### Comparing `pyjaws-0.1.0/pyjaws.egg-info/PKG-INFO` & `pyjaws-0.1.1/pyjaws.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: pyjaws
-Version: 0.1.0
+Version: 0.1.1
 Author: Rafael Pierre
 Description-Content-Type: text/markdown
 
 # PyJaws: A Pythonic Way to Define Databricks Jobs and Workflows
 
 <p align="center">
         <img src="https://raw.githubusercontent.com/rafaelpierre/pyjaws/main/img/pyjaws.png" class="align-center" />
     </a>
 </p>
 
 <hr />
 
-[![pypi](https://img.shields.io/badge/pypi-0.0.9-brightgreen?style=for-the-badge)](https://pypi.org/project/pyjaws/) ![black](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge) ![ruff](https://img.shields.io/badge/lint-ruff-gold?style=for-the-badge) ![cov](https://raw.githubusercontent.com/rafaelpierre/pyjaws/main/img/coverage.svg) ![databricks](https://img.shields.io/badge/Databricks-FF3621.svg?style=for-the-badge&logo=Databricks&logoColor=white) ![Jinja](https://img.shields.io/badge/jinja-white.svg?style=for-the-badge&logo=jinja&logoColor=black)
+[![pypi](https://img.shields.io/badge/pypi-0.1.0-brightgreen?style=for-the-badge)](https://pypi.org/project/pyjaws/) ![black](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge) ![ruff](https://img.shields.io/badge/lint-ruff-gold?style=for-the-badge) ![cov](https://raw.githubusercontent.com/rafaelpierre/pyjaws/main/img/coverage.svg) ![databricks](https://img.shields.io/badge/Databricks-FF3621.svg?style=for-the-badge&logo=Databricks&logoColor=white) ![Jinja](https://img.shields.io/badge/jinja-white.svg?style=for-the-badge&logo=jinja&logoColor=black)
 
 <hr />
 
 * **PyJaws** enables declaring [Databricks Jobs and Workflows](https://docs.databricks.com/workflows/index.html) as Python code, allowing for:
-   * Code Linting
-   * Formatting
-   * Parameter Validation
-   * Modularity and reusability
+  * Code Linting
+  * Formatting
+  * Parameter Validation
+  * Modularity and reusability
 * In addition to those, **PyJaws** also provides some nice features such as [cycle detection](https://networkx.org/documentation/stable/reference/algorithms/cycles.html) out of the box.
 
 Folks who have used Python-based orchestration tools such as [Apache Airflow](https://airflow.apache.org/), [Luigi](https://luigi.readthedocs.io/en/stable/) and [Mage](https://pypi.org/project/mage-ai/) will be familiar with the concepts and the API if **PyJaws**.
 
 * **PyJaws** leverages some existing libraries in order to allow for **modularisation**, **reusability** and **validation**, such as:
-    * [Click](https://click.palletsprojects.com/en/8.1.x/) - for providing a rich CLI functionality
-    * [Pydantic](https://docs.pydantic.dev/latest/) - for efficient parameter validation
-    * [NetworkX](https://networkx.org/) - for Graph and Cycle Detection features
-    * [Jinja2](https://jinja.palletsprojects.com/en/3.1.x/) - for templating
+  * [Click](https://click.palletsprojects.com/en/8.1.x/) - for providing a rich CLI functionality
+  * [Pydantic](https://docs.pydantic.dev/latest/) - for efficient parameter validation
+  * [NetworkX](https://networkx.org/) - for Graph and Cycle Detection features
+  * [Jinja2](https://jinja.palletsprojects.com/en/3.1.x/) - for templating
 
 ## Documentation
 
 * Work in progress. Stay tuned!
 
 ## Development & Testing
 
@@ -63,17 +63,17 @@
 
 ### Sample Job Definition
 
 ```python
 from pyjaws.api.base import (
     Cluster,
     Runtime,
-    Task,
     Workflow
 )
+from pyjaws.api.tasks import PythonWheelTask
 
 cluster = Cluster(
     job_cluster_key = "ai_cluster",
     spark_version = Runtime.DBR_13_ML,
     num_workers = 2,
     node_type_id = "Standard_DS3_v2",
     cluster_log_conf = {
@@ -82,26 +82,26 @@
         }
     }
 )
 
 
 # Create a Task object.
 
-ingest_task = Task(
+ingest_task = PythonWheelTask(
     key = "ingest",
     cluster = cluster,
     entrypoint = "iot",
     task_name = "ingest",
     parameters = [
         f"my_parameter_value",
         "--output-table", "my_table"
     ]
 )
 
-transform_task = Task(
+transform_task = PythonWheelTask(
     key = "transform",
     cluster = cluster,
     entrypoint = "iot",
     task_name = "ingest",
     dependencies = [ingest_task],
     parameters = [
         f"my_parameter_value2",
```

### Comparing `pyjaws-0.1.0/pyproject.toml` & `pyjaws-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyjaws-0.1.0/setup.py` & `pyjaws-0.1.1/setup.py`

 * *Files identical despite different names*

