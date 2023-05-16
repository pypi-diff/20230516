# Comparing `tmp/google-cloud-automlops-1.1.0.tar.gz` & `tmp/google-cloud-automlops-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-automlops-1.1.0.tar", last modified: Mon May  1 20:18:52 2023, max compression
+gzip compressed data, was "google-cloud-automlops-1.1.1.tar", last modified: Tue May 16 17:39:33 2023, max compression
```

## Comparing `google-cloud-automlops-1.1.0.tar` & `google-cloud-automlops-1.1.1.tar`

### file list

```diff
@@ -1,20 +1,54 @@
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-01 20:18:52.525854 google-cloud-automlops-1.1.0/
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-01 20:18:52.524621 google-cloud-automlops-1.1.0/AutoMLOps/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    43608 2023-05-01 20:16:21.000000 google-cloud-automlops-1.1.0/AutoMLOps/AutoMLOps.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      702 2023-02-07 20:59:28.000000 google-cloud-automlops-1.1.0/AutoMLOps/AutoMLOps_test.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     9741 2023-05-01 20:16:21.000000 google-cloud-automlops-1.1.0/AutoMLOps/BuilderUtils.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    19465 2023-05-01 20:16:21.000000 google-cloud-automlops-1.1.0/AutoMLOps/CloudRunBuilder.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    10765 2023-05-01 20:16:21.000000 google-cloud-automlops-1.1.0/AutoMLOps/ComponentBuilder.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    13155 2023-05-01 20:16:21.000000 google-cloud-automlops-1.1.0/AutoMLOps/PipelineBuilder.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     1199 2023-05-01 20:16:21.000000 google-cloud-automlops-1.1.0/AutoMLOps/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    11357 2023-01-13 20:01:02.000000 google-cloud-automlops-1.1.0/LICENSE
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    14181 2023-05-01 20:18:52.525651 google-cloud-automlops-1.1.0/PKG-INFO
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    13312 2023-05-01 20:16:21.000000 google-cloud-automlops-1.1.0/README.md
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-01 20:18:52.525435 google-cloud-automlops-1.1.0/google_cloud_automlops.egg-info/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    14181 2023-05-01 20:18:52.000000 google-cloud-automlops-1.1.0/google_cloud_automlops.egg-info/PKG-INFO
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      442 2023-05-01 20:18:52.000000 google-cloud-automlops-1.1.0/google_cloud_automlops.egg-info/SOURCES.txt
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)        1 2023-05-01 20:18:52.000000 google-cloud-automlops-1.1.0/google_cloud_automlops.egg-info/dependency_links.txt
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)       79 2023-05-01 20:18:52.000000 google-cloud-automlops-1.1.0/google_cloud_automlops.egg-info/requires.txt
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)       10 2023-05-01 20:18:52.000000 google-cloud-automlops-1.1.0/google_cloud_automlops.egg-info/top_level.txt
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)       38 2023-05-01 20:18:52.525910 google-cloud-automlops-1.1.0/setup.cfg
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     1910 2023-05-01 20:16:21.000000 google-cloud-automlops-1.1.0/setup.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-16 17:39:33.211176 google-cloud-automlops-1.1.1/
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-16 17:39:33.200431 google-cloud-automlops-1.1.1/AutoMLOps/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    15403 2023-05-16 14:47:23.000000 google-cloud-automlops-1.1.1/AutoMLOps/AutoMLOps.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     1199 2023-05-12 15:42:26.000000 google-cloud-automlops-1.1.1/AutoMLOps/__init__.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-16 17:39:33.200853 google-cloud-automlops-1.1.1/AutoMLOps/deployments/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-15 14:44:02.000000 google-cloud-automlops-1.1.1/AutoMLOps/deployments/__init__.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-16 17:39:33.201602 google-cloud-automlops-1.1.1/AutoMLOps/deployments/cloudbuild/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-15 14:44:07.000000 google-cloud-automlops-1.1.1/AutoMLOps/deployments/cloudbuild/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     2258 2023-05-12 20:14:34.000000 google-cloud-automlops-1.1.1/AutoMLOps/deployments/cloudbuild/builder.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-16 17:39:33.202142 google-cloud-automlops-1.1.1/AutoMLOps/deployments/cloudbuild/constructs/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)        0 2023-05-10 19:53:15.000000 google-cloud-automlops-1.1.1/AutoMLOps/deployments/cloudbuild/constructs/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     9302 2023-05-15 18:22:07.000000 google-cloud-automlops-1.1.1/AutoMLOps/deployments/cloudbuild/constructs/scripts.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-16 17:39:33.202879 google-cloud-automlops-1.1.1/AutoMLOps/frameworks/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-15 14:43:10.000000 google-cloud-automlops-1.1.1/AutoMLOps/frameworks/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     2271 2023-05-12 18:33:19.000000 google-cloud-automlops-1.1.1/AutoMLOps/frameworks/base.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-16 17:39:33.203927 google-cloud-automlops-1.1.1/AutoMLOps/frameworks/kfp/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-15 14:43:27.000000 google-cloud-automlops-1.1.1/AutoMLOps/frameworks/kfp/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    11973 2023-05-12 20:11:24.000000 google-cloud-automlops-1.1.1/AutoMLOps/frameworks/kfp/builder.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-16 17:39:33.205923 google-cloud-automlops-1.1.1/AutoMLOps/frameworks/kfp/constructs/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-15 14:43:45.000000 google-cloud-automlops-1.1.1/AutoMLOps/frameworks/kfp/constructs/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    20675 2023-05-12 18:34:14.000000 google-cloud-automlops-1.1.1/AutoMLOps/frameworks/kfp/constructs/cloudrun.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     3421 2023-05-12 18:34:54.000000 google-cloud-automlops-1.1.1/AutoMLOps/frameworks/kfp/constructs/component.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     8842 2023-05-12 18:37:02.000000 google-cloud-automlops-1.1.1/AutoMLOps/frameworks/kfp/constructs/pipeline.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    31558 2023-05-15 18:21:03.000000 google-cloud-automlops-1.1.1/AutoMLOps/frameworks/kfp/constructs/scripts.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     8702 2023-05-12 18:55:25.000000 google-cloud-automlops-1.1.1/AutoMLOps/frameworks/kfp/scaffold.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-16 17:39:33.207291 google-cloud-automlops-1.1.1/AutoMLOps/utils/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-15 18:34:44.000000 google-cloud-automlops-1.1.1/AutoMLOps/utils/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     3231 2023-05-16 15:37:55.000000 google-cloud-automlops-1.1.1/AutoMLOps/utils/constants.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     9583 2023-05-10 20:13:43.000000 google-cloud-automlops-1.1.1/AutoMLOps/utils/utils.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    11357 2023-01-13 20:01:02.000000 google-cloud-automlops-1.1.1/LICENSE
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    14196 2023-05-16 17:39:33.211001 google-cloud-automlops-1.1.1/PKG-INFO
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    13327 2023-05-11 17:20:14.000000 google-cloud-automlops-1.1.1/README.md
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-16 17:39:33.208212 google-cloud-automlops-1.1.1/google_cloud_automlops.egg-info/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    14196 2023-05-16 17:39:33.000000 google-cloud-automlops-1.1.1/google_cloud_automlops.egg-info/PKG-INFO
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     1265 2023-05-16 17:39:33.000000 google-cloud-automlops-1.1.1/google_cloud_automlops.egg-info/SOURCES.txt
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)        1 2023-05-16 17:39:33.000000 google-cloud-automlops-1.1.1/google_cloud_automlops.egg-info/dependency_links.txt
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)       79 2023-05-16 17:39:33.000000 google-cloud-automlops-1.1.1/google_cloud_automlops.egg-info/requires.txt
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)       16 2023-05-16 17:39:33.000000 google-cloud-automlops-1.1.1/google_cloud_automlops.egg-info/top_level.txt
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)       38 2023-05-16 17:39:33.211225 google-cloud-automlops-1.1.1/setup.cfg
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     1949 2023-05-12 18:42:41.000000 google-cloud-automlops-1.1.1/setup.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-16 17:39:33.208356 google-cloud-automlops-1.1.1/tests/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-15 18:34:44.000000 google-cloud-automlops-1.1.1/tests/__init__.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-16 17:39:33.209048 google-cloud-automlops-1.1.1/tests/unit/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      702 2023-02-07 20:59:28.000000 google-cloud-automlops-1.1.1/tests/unit/AutoMLOps_test.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-15 18:22:39.000000 google-cloud-automlops-1.1.1/tests/unit/__init__.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-16 17:39:33.209424 google-cloud-automlops-1.1.1/tests/unit/deployments/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-15 18:22:44.000000 google-cloud-automlops-1.1.1/tests/unit/deployments/__init__.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-16 17:39:33.209799 google-cloud-automlops-1.1.1/tests/unit/frameworks/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-15 18:22:57.000000 google-cloud-automlops-1.1.1/tests/unit/frameworks/__init__.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-16 17:39:33.210113 google-cloud-automlops-1.1.1/tests/unit/frameworks/kfp/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-15 18:23:03.000000 google-cloud-automlops-1.1.1/tests/unit/frameworks/kfp/__init__.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-16 17:39:33.210660 google-cloud-automlops-1.1.1/tests/unit/utils/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-15 18:23:13.000000 google-cloud-automlops-1.1.1/tests/unit/utils/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    11516 2023-05-15 19:11:22.000000 google-cloud-automlops-1.1.1/tests/unit/utils/utils_test.py
```

### Comparing `google-cloud-automlops-1.1.0/AutoMLOps/AutoMLOps_test.py` & `google-cloud-automlops-1.1.1/tests/unit/AutoMLOps_test.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.0/AutoMLOps/BuilderUtils.py` & `google-cloud-automlops-1.1.1/AutoMLOps/utils/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,35 +23,15 @@
 import subprocess
 
 import itertools
 import textwrap
 from typing import Callable
 import yaml
 
-TMPFILES_DIR = '.tmpfiles'
-IMPORTS_TMPFILE = f'{TMPFILES_DIR}/imports.py'
-CELL_TMPFILE = f'{TMPFILES_DIR}/cell.py'
-PIPELINE_TMPFILE = f'{TMPFILES_DIR}/pipeline_scaffold.py'
-PARAMETER_VALUES_PATH = 'pipelines/runtime_parameters/pipeline_parameter_values.json'
-PIPELINE_JOB_SPEC_PATH = 'scripts/pipeline_spec/pipeline_job.json'
-LICENSE = (
-    '# Licensed under the Apache License, Version 2.0 (the "License");\n'
-    '# you may not use this file except in compliance with the License.\n'
-    '# You may obtain a copy of the License at\n'
-    '#\n'
-    '#     http://www.apache.org/licenses/LICENSE-2.0\n'
-    '#\n'
-    '# Unless required by applicable law or agreed to in writing, software\n'
-    '# distributed under the License is distributed on an "AS IS" BASIS,\n'
-    '# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.\n'
-    '# See the License for the specific language governing permissions and\n'
-    '# limitations under the License.\n'
-    '#\n'
-    '# DISCLAIMER: This code is generated as part of the AutoMLOps output.\n'
-    '\n')
+from AutoMLOps.utils.constants import TMPFILES_DIR
 
 def make_dirs(directories: list):
     """Makes directories with the specified names.
 
     Args:
         directories: Path of the directories to make.
     """
@@ -201,17 +181,19 @@
         command: The string of the command to execute.
         to_null: Determines where to send output.
     Raises:
         Exception: If an error occurs in executing the script.
     """
     stdout = subprocess.DEVNULL if to_null else None
     try:
-        subprocess.run([command], shell=True, check=True,
-            stdout=stdout,
-            stderr=subprocess.STDOUT)
+        subprocess.run([command],
+                       shell=True,
+                       check=True,
+                       stdout=stdout,
+                       stderr=subprocess.STDOUT)
     except subprocess.CalledProcessError as err:
         raise RuntimeError(f'Error executing process. {err}') from err
 
 def validate_schedule(schedule_pattern: str, run_local: str):
     """Validates that the inputted schedule parameter.
 
     Args:
@@ -248,15 +230,15 @@
         dict: 'Dict'
     }
     for param in params:
         try:
             param['type'] = python_kfp_types_mapper[param['type']]
         except KeyError as err:
             raise ValueError(f'Unsupported python type - we only support '
-                            f'primitive types at this time. {err}') from err
+                             f'primitive types at this time. {err}') from err
     return params
 
 def get_function_source_definition(func: Callable) -> str:
     """Returns a formatted list of parameters.
 
     Args:
         func: The python function to create a component from. The function
@@ -275,7 +257,28 @@
                                             source_code_lines)
     if not source_code_lines:
         raise ValueError(
             f'Failed to dedent and clean up the source of function "{func.__name__}". '
             f'It is probably not properly indented.')
 
     return '\n'.join(source_code_lines)
+
+def format_spec_dict(job_spec: dict) -> str:
+    """Takes in a job spec dictionary and removes the quotes around the component op name. 
+    e.g. 'component_spec': 'train_model' becomes 'component_spec': train_model.
+    This is necessary to in order for the op to be callable within the Python code.
+
+    Args:
+        job_spec: Dictionary with job spec info.
+
+    Returns:
+        str: Python formatted dictionary code.
+    """
+    quote = '\''
+    left_bracket = '{'
+    right_bracket = '}'
+    newline = '\n'
+
+    return (
+        f'''{left_bracket}\n'''
+        f'''    {f'{newline}    '.join(f"   {quote}{k}{quote}: {quote if k != 'component_spec' else ''}{v}{quote if k != 'component_spec' else ''}," for k, v in job_spec.items())}{newline}'''
+        f'''    {right_bracket}\n''')
```

### Comparing `google-cloud-automlops-1.1.0/AutoMLOps/CloudRunBuilder.py` & `google-cloud-automlops-1.1.1/AutoMLOps/frameworks/kfp/constructs/cloudrun.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,384 +8,393 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Builds cloud_run files."""
+"""Code strings for a kfp cloud run instance."""
 
-# pylint: disable=C0103
 # pylint: disable=line-too-long
 
-from AutoMLOps import BuilderUtils
-
-def formalize(top_lvl_name: str,
-              defaults_file: str,):
-    """Constructs and writes a Dockerfile, requirements.txt, and
-       main.py to the cloud_run/run_pipeline directory. Also
-       constructs and writes a main.py, requirements.txt, and
-       pipeline_parameter_values.json to the
-       cloud_run/queueing_svc directory.
-
-    Args:
-        top_lvl_name: Top directory name.
-        defaults_file: Path to the default config variables yaml.
-    """
-    BuilderUtils.make_dirs([top_lvl_name + 'cloud_run',
-                            top_lvl_name + 'cloud_run/run_pipeline',
-                            top_lvl_name + 'cloud_run/queueing_svc'])
-    create_dockerfile(top_lvl_name)
-    create_requirements(top_lvl_name)
-    create_mains(top_lvl_name, defaults_file)
-    # copy runtime parameters over to queueing_svc dir
-    BuilderUtils.execute_process(f'''cp -r {top_lvl_name + BuilderUtils.PARAMETER_VALUES_PATH} {top_lvl_name + 'cloud_run/queueing_svc'}''', to_null=False)
-
-def create_dockerfile(top_lvl_name: str):
-    """Writes a Dockerfile to the cloud_run/run_pipeline directory.
-
-    Args:
-        top_lvl_name: Top directory name.
-    """
-    cloudrun_base = top_lvl_name + 'cloud_run/run_pipeline'
-    dockerfile = (BuilderUtils.LICENSE +
-        'FROM python:3.9-slim\n'
-        '\n'
-        '# Allow statements and log messages to immediately appear in the Knative logs\n'
-        'ENV PYTHONUNBUFFERED True\n'
-        '\n'
-        '# Copy local code to the container image.\n'
-        'ENV APP_HOME /app\n'
-        'WORKDIR $APP_HOME\n'
-        'COPY ./ ./\n'
-        '\n'
-        '# Upgrade pip\n'
-        'RUN python -m pip install --upgrade pip\n'
-        '# Install requirements\n'
-        'RUN pip install --no-cache-dir -r /app/cloud_run/run_pipeline/requirements.txt\n'
-        '# Compile pipeline spec\n'
-        'RUN ./scripts/build_pipeline_spec.sh\n'
-        '# Change Directories\n'
-        'WORKDIR "/app/cloud_run/run_pipeline"\n'
-        '# Run flask api server\n'
-        'CMD exec gunicorn --bind :$PORT --workers 1 --threads 8 --timeout 0 main:app\n'
-    )
-    BuilderUtils.write_file(f'{cloudrun_base}/Dockerfile', dockerfile, 'w')
-
-def create_requirements(top_lvl_name: str):
-    """Writes a requirements.txt to the cloud_run/run_pipeline
-       directory, and a requirements.txt to the cloud_run/queueing_svc
-       directory.
-
-    Args:
-        top_lvl_name: Top directory name.
-    """
-    cloudrun_base = top_lvl_name + 'cloud_run/run_pipeline'
-    queueing_svc_base = top_lvl_name + 'cloud_run/queueing_svc'
-    cloud_run_reqs = (
-        'kfp\n'
-        'google-cloud-aiplatform\n'
-        'google-cloud-pipeline-components\n'
-        'Flask\n'
-        'gunicorn\n'
-        'pyyaml\n'
-    )
-    queueing_svc_reqs = (
-        'google-cloud\n'
-        'google-cloud-tasks\n'
-        'google-api-python-client\n'
-        'google-cloud-run\n'
-        'google-cloud-scheduler\n'
-    )
-    BuilderUtils.write_file(f'{cloudrun_base}/requirements.txt', cloud_run_reqs, 'w')
-    BuilderUtils.write_file(f'{queueing_svc_base}/requirements.txt', queueing_svc_reqs, 'w')
-
-def create_mains(top_lvl_name: str,
-                 defaults_file: str):
-    """Writes a main.py to the cloud_run/run_pipeline
-       directory. This file contains code for running
-       a flask service that will act as a pipeline
-       runner service. Also writes a main.py to
-       the cloud_run/queueing_svc directory. This file
-       contains code for submitting a job to the cloud
-       runner service, and creating a cloud scheduler job.
-
-    Args:
-        top_lvl_name: Top directory name.
-        defaults_file: Path to the default config variables yaml.
-    """
-    defaults = BuilderUtils.read_yaml_file(defaults_file)
-    cloudrun_base = top_lvl_name + 'cloud_run/run_pipeline'
-    queueing_svc_base = top_lvl_name + 'cloud_run/queueing_svc'
-    left_bracket = '{'
-    right_bracket = '}'
-    cloud_run_code = (BuilderUtils.LICENSE +
-        f'''"""Cloud Run to run pipeline spec"""\n'''
-        f'''import logging\n'''
-        f'''import os\n'''
-        f'''from typing import Tuple\n'''
-        f'\n'
-        f'''import flask\n'''
-        f'''from google.cloud import aiplatform\n'''
-        f'''import yaml\n'''
-        f'\n'
-        f'''app = flask.Flask(__name__)\n'''
-        f'\n'
-        f'''logger = logging.getLogger()\n'''
-        f'''log_level = os.environ.get('LOG_LEVEL', 'INFO')\n'''
-        f'''logger.setLevel(log_level)\n'''
-        f'\n'
-        f'''CONFIG_FILE = '../../configs/defaults.yaml'\n'''
-        f'''PIPELINE_SPEC_PATH_LOCAL = '../../scripts/pipeline_spec/pipeline_job.json'\n'''
-        f'\n'
-        f'''@app.route('/', methods=['POST'])\n'''
-        f'''def process_request() -> flask.Response:\n'''
-        f'''    """HTTP web service to trigger pipeline execution.\n'''
-        f'\n'
-        f'''    Returns:\n'''
-        f'''        The response text, or any set of values that can be turned into a\n'''
-        f'''        Response object using `make_response`\n'''
-        f'''        <https://flask.palletsprojects.com/en/1.1.x/api/#flask.make_response>.\n'''
-        f'''    """\n'''
-        f'''    content_type = flask.request.headers['content-type']\n'''
-        f'''    if content_type == 'application/json':\n'''
-        f'''        request_json = flask.request.json\n'''
-        f'\n'
-        f'''        logging.debug('JSON Recieved:')\n'''
-        f'''        logging.debug(request_json)\n'''
-        f'\n'
-        f'''        with open(CONFIG_FILE, 'r', encoding='utf-8') as config_file:\n'''
-        f'''            config = yaml.load(config_file, Loader=yaml.FullLoader)\n'''
-        f'\n'
-        f'''        logging.debug('Calling run_pipeline()')\n'''
-        f'''        dashboard_uri, resource_name = run_pipeline(\n'''
-        f'''            project_id=config['gcp']['project_id'],\n'''
-        f'''            pipeline_root=config['pipelines']['pipeline_storage_path'],\n'''
-        f'''            pipeline_runner_sa=config['gcp']['pipeline_runner_service_account'],\n'''
-        f'''            pipeline_params=request_json,\n'''
-        f'''            pipeline_spec_path=PIPELINE_SPEC_PATH_LOCAL)\n'''
-        f'''        return flask.make_response({left_bracket}\n'''
-        f'''            'dashboard_uri': dashboard_uri,\n'''
-        f'''            'resource_name': resource_name\n'''
-        f'''        {right_bracket}, 200)\n'''
-        f'\n'
-        f'''    else:\n'''
-        f'''        raise ValueError(f'Unknown content type: {left_bracket}content_type{right_bracket}')\n'''
-        f'\n'
-        f'''def run_pipeline(\n'''
-        f'''    project_id: str,\n'''
-        f'''    pipeline_root: str,\n'''
-        f'''    pipeline_runner_sa: str,\n'''
-        f'''    pipeline_params: dict,\n'''
-        f'''    pipeline_spec_path: str,\n'''
-        f'''    display_name: str = 'mlops-pipeline-run',\n'''
-        f'''    enable_caching: bool = False) -> Tuple[str, str]:\n'''
-        f'''    """Executes a pipeline run.\n'''
-        f'\n'
-        f'''    Args:\n'''
-        f'''        project_id: The project_id.\n'''
-        f'''        pipeline_root: GCS location of the pipeline runs metadata.\n'''
-        f'''        pipeline_runner_sa: Service Account to runner PipelineJobs.\n'''
-        f'''        pipeline_params: Pipeline parameters values.\n'''
-        f'''        pipeline_spec_path: Location of the pipeline spec JSON.\n'''
-        f'''        display_name: Name to call the pipeline.\n'''
-        f'''        enable_caching: Should caching be enabled (Boolean)\n'''
-        f'''    """\n'''
-        f'''    logging.debug('Pipeline Parms Configured:')\n'''
-        f'''    logging.debug(pipeline_params)\n'''
-        f'\n'
-        f'''    aiplatform.init(project=project_id)\n'''
-        f'''    job = aiplatform.PipelineJob(\n'''
-        f'''        display_name = display_name,\n'''
-        f'''        template_path = pipeline_spec_path,\n'''
-        f'''        pipeline_root = pipeline_root,\n'''
-        f'''        parameter_values = pipeline_params,\n'''
-        f'''        enable_caching = enable_caching)\n'''
-        f'''    logging.debug('AI Platform job built. Submitting...')\n'''
-        f'''    job.submit(service_account=pipeline_runner_sa)\n'''
-        f'''    logging.debug('Job sent!')\n'''
-        f'''    dashboard_uri = job._dashboard_uri()\n'''
-        f'''    resource_name = job.resource_name\n'''
-        f'''    return dashboard_uri, resource_name\n'''
-        f'\n'
-        f'''if __name__ == '__main__':\n'''
-        f'''    app.run(debug=True, host='0.0.0.0', port=int(os.environ.get('PORT', 8080)))\n''')
-
-    queueing_svc_code = (BuilderUtils.LICENSE +
-        f'''"""Submit pipeline job using Cloud Tasks and create Cloud Scheduler Job."""\n'''
-        f'''import argparse\n'''
-        f'''import json\n'''
-        f'\n'
-        f'''from google.cloud import run_v2\n'''
-        f'''from google.cloud import scheduler_v1\n'''
-        f'''from google.cloud import tasks_v2\n'''
-        f'\n'
-        f'''CLOUD_RUN_LOCATION = '{defaults['gcp']['cloud_run_location']}'\n'''
-        f'''CLOUD_RUN_NAME = '{defaults['gcp']['cloud_run_name']}'\n'''
-        f'''CLOUD_TASKS_QUEUE_LOCATION = '{defaults['gcp']['cloud_tasks_queue_location']}'\n'''
-        f'''CLOUD_TASKS_QUEUE_NAME = '{defaults['gcp']['cloud_tasks_queue_name']}'\n'''
-        f'''PARAMETER_VALUES_PATH = 'queueing_svc/pipeline_parameter_values.json'\n'''
-        f'''PIPELINE_RUNNER_SA = '{defaults['gcp']['pipeline_runner_service_account']}'\n'''
-        f'''PROJECT_ID = '{defaults['gcp']['project_id']}'\n'''
-        f'''SCHEDULE_LOCATION = '{defaults['gcp']['cloud_schedule_location']}'\n'''
-        f'''SCHEDULE_NAME = '{defaults['gcp']['cloud_schedule_name']}'\n'''
-        f'''SCHEDULE_PATTERN = '{defaults['gcp']['cloud_schedule_pattern']}'\n'''
-        f'\n'
-        f'''def get_runner_svc_uri(\n'''
-        f'''    cloud_run_location: str,\n'''
-        f'''    cloud_run_name: str,\n'''
-        f'''    project_id: str):\n'''
-        f'''    """Fetches the uri for the given cloud run instance.\n'''
-        f'\n'
-        f'''    Args:\n'''
-        f'''        cloud_run_location: The location of the cloud runner service.\n'''
-        f'''        cloud_run_name: The name of the cloud runner service.\n'''
-        f'''        project_id: The project ID.\n'''
-        f'''    Returns:\n'''
-        f'''        str: Uri of the Cloud Run instance.\n'''
-        f'''    """\n'''
-        f'''    client = run_v2.ServicesClient()\n'''
-        f'''    parent = client.service_path(project_id, cloud_run_location, cloud_run_name)\n'''
-        f'''    request = run_v2.GetServiceRequest(name=parent)\n'''
-        f'''    response = client.get_service(request=request)\n'''
-        f'''    return response.uri\n'''
-        f'\n'
-        f'''def get_json_bytes(file_path: str):\n'''
-        f'''    """Reads a json file at the specified path and returns as bytes.\n'''
-        f'\n'
-        f'''    Args:\n'''
-        f'''        file_path: Path of the json file.\n'''
-        f'''    Returns:\n'''
-        f'''        bytes: Encode bytes of the file.\n'''
-        f'''    """\n'''
-        f'''    try:\n'''
-        f'''        with open(file_path, 'r', encoding='utf-8') as file:\n'''
-        f'''            data = json.load(file)\n'''
-        f'''        file.close()\n'''
-        f'''    except OSError as err:\n'''
-        f'''        raise Exception(f'Error reading json file. {left_bracket}err{right_bracket}') from err\n'''
-        f'''    return json.dumps(data).encode()\n'''
-        f'\n'
-        f'''def create_cloud_task(\n'''
-        f'''    cloud_tasks_queue_location: str,\n'''
-        f'''    cloud_tasks_queue_name: str,\n'''
-        f'''    parameter_values_path: str,\n'''
-        f'''    pipeline_runner_sa: str,\n'''
-        f'''    project_id: str,\n'''
-        f'''    runner_svc_uri: str):\n'''
-        f'''    """Create a task to the queue with the runtime parameters.\n'''
-        f'\n'
-        f'''    Args:\n'''
-        f'''        cloud_run_location: The location of the cloud runner service.\n'''
-        f'''        cloud_run_name: The name of the cloud runner service.\n'''
-        f'''        cloud_tasks_queue_location: The location of the cloud tasks queue.\n'''
-        f'''        cloud_tasks_queue_name: The name of the cloud tasks queue.\n'''
-        f'''        parameter_values_path: Path to json pipeline params.\n'''
-        f'''        pipeline_runner_sa: Service Account to runner PipelineJobs.\n'''
-        f'''        project_id: The project ID.\n'''
-        f'''        runner_svc_uri: Uri of the Cloud Run instance.\n'''
-        f'''    """\n'''
-        f'''    client = tasks_v2.CloudTasksClient()\n'''
-        f'''    parent = client.queue_path(project_id, cloud_tasks_queue_location, cloud_tasks_queue_name)\n'''
-        f'''    task = {left_bracket}\n'''
-        f'''        'http_request': {left_bracket}\n'''
-        f'''            'http_method': tasks_v2.HttpMethod.POST,\n'''
-        f'''            'url': runner_svc_uri,\n'''
-        f'''            'oidc_token': {left_bracket}\n'''
-        f'''                'service_account_email': pipeline_runner_sa,\n'''
-        f'''                'audience': runner_svc_uri\n'''
-        f'''            {right_bracket},\n'''
-        f'''            'headers': {left_bracket}\n'''
-        f'''               'Content-Type': 'application/json'\n'''
-        f'''            {right_bracket}\n'''
-        f'''        {right_bracket}\n'''
-        f'''    {right_bracket}\n'''
-        f'''    task['http_request']['body'] = get_json_bytes(parameter_values_path)\n'''
-        f'''    response = client.create_task(request={left_bracket}'parent': parent, 'task': task{right_bracket})\n'''
-        f'''    print(f'Created task {left_bracket}response.name{right_bracket}')\n'''
-        f'\n'
-        f'''def create_cloud_scheduler_job(\n'''
-        f'''    parameter_values_path: str,\n'''
-        f'''    pipeline_runner_sa: str,\n'''
-        f'''    project_id: str,\n'''
-        f'''    runner_svc_uri: str,\n'''
-        f'''    schedule_location: str,\n'''
-        f'''    schedule_name: str,\n'''
-        f'''    schedule_pattern: str):\n'''
-        f'''    """Creates a scheduled pipeline job.\n'''
-        f'\n'
-        f'''    Args:\n'''
-        f'''        parameter_values_path: Path to json pipeline params.\n'''
-        f'''        pipeline_runner_sa: Service Account to runner PipelineJobs.\n'''
-        f'''        project_id: The project ID.\n'''
-        f'''        runner_svc_uri: Uri of the Cloud Run instance.\n'''
-        f'''        schedule_location: The location of the scheduler resource.\n'''
-        f'''        schedule_name: The name of the scheduler resource.\n'''
-        f'''        schedule_pattern: Cron formatted value used to create a Scheduled retrain job.\n'''
-        f'''    """\n'''
-        f'''    client = scheduler_v1.CloudSchedulerClient()\n'''
-        f'''    parent = f'projects/{left_bracket}project_id{right_bracket}/locations/{left_bracket}schedule_location{right_bracket}'\n'''
-        f'''    name = f'{left_bracket}parent{right_bracket}/jobs/{left_bracket}schedule_name{right_bracket}'\n'''
-        f'\n'
-        f'''    request = scheduler_v1.ListJobsRequest(parent=parent)\n'''
-        f'''    page_result = client.list_jobs(request=request)\n'''
-        f'''    for response in page_result:\n'''
-        f'''        if response.name == name:\n'''
-        f'''            print(f'Cloud Scheduler {left_bracket}schedule_name{right_bracket} resource already exists in '\n'''
-        f'''                  f'project {left_bracket}project_id{right_bracket}.')\n'''
-        f'''            return\n'''
-        f'\n'
-        f'''    oidc_token = scheduler_v1.OidcToken(\n'''
-        f'''        service_account_email=pipeline_runner_sa,\n'''
-        f'''        audience=runner_svc_uri)\n'''
-        f'\n'
-        f'''    target = scheduler_v1.HttpTarget(\n'''
-        f'''       uri=runner_svc_uri,\n'''
-        f'''        http_method=scheduler_v1.HttpMethod(1), # HTTP POST\n'''
-        f'''        headers={left_bracket}'Content-Type': 'application/json'{right_bracket},\n'''
-        f'''        body=get_json_bytes(parameter_values_path),\n'''
-        f'''        oidc_token=oidc_token)\n'''
-        f'\n'
-        f'''    job = scheduler_v1.Job(\n'''
-        f'''       name=f'{left_bracket}parent{right_bracket}/jobs/{left_bracket}schedule_name{right_bracket}',\n'''
-        f'''        description='AutoMLOps cloud scheduled run.',\n'''
-        f'''        http_target=target,\n'''
-        f'''        schedule=schedule_pattern)\n'''
-        f'\n'
-        f'''    request = scheduler_v1.CreateJobRequest(\n'''
-        f'''        parent=parent,\n'''
-        f'''        job=job)\n'''
-        f'\n'
-        f'''    response = client.create_job(request=request)\n'''
-        f'''    print(response)\n'''
-        f'\n'
-        f'''if __name__ == '__main__':\n'''
-        f'''    parser = argparse.ArgumentParser()\n'''
-        f'''    parser.add_argument('--setting', type=str,\n'''
-        f'''                       help='The config file for setting default values.')\n'''
-        f'''    args = parser.parse_args()\n'''
-        f'\n'
-        f'''    uri = get_runner_svc_uri(\n'''
-        f'''        cloud_run_location=CLOUD_RUN_LOCATION,\n'''
-        f'''        cloud_run_name=CLOUD_RUN_NAME,\n'''
-        f'''        project_id=PROJECT_ID)\n'''
-        f'\n'
-        f'''    if args.setting == 'queue_job':\n'''
-        f'''        create_cloud_task(\n'''
-        f'''            cloud_tasks_queue_location=CLOUD_TASKS_QUEUE_LOCATION,\n'''
-        f'''            cloud_tasks_queue_name=CLOUD_TASKS_QUEUE_NAME,\n'''
-        f'''            parameter_values_path=PARAMETER_VALUES_PATH,\n'''
-        f'''            pipeline_runner_sa=PIPELINE_RUNNER_SA,\n'''
-        f'''            project_id=PROJECT_ID,\n'''
-        f'''            runner_svc_uri=uri)\n'''
-        f'\n'
-        f'''    if args.setting == 'schedule_job':\n'''
-        f'''        create_cloud_scheduler_job(\n'''
-        f'''            parameter_values_path=PARAMETER_VALUES_PATH,\n'''
-        f'''            pipeline_runner_sa=PIPELINE_RUNNER_SA,\n'''
-        f'''            project_id=PROJECT_ID,\n'''
-        f'''            runner_svc_uri=uri,\n'''
-        f'''            schedule_location=SCHEDULE_LOCATION,\n'''
-        f'''            schedule_name=SCHEDULE_NAME,\n'''
-        f'''            schedule_pattern=SCHEDULE_PATTERN)\n''')
-    BuilderUtils.write_file(f'{cloudrun_base}/main.py', cloud_run_code, 'w')
-    BuilderUtils.write_file(f'{queueing_svc_base}/main.py', queueing_svc_code, 'w')
+from AutoMLOps.utils.utils import read_yaml_file
+from AutoMLOps.utils.constants import (
+    GENERATED_LICENSE,
+    LEFT_BRACKET,
+    RIGHT_BRACKET
+)
+
+class KfpCloudRun():
+    """Generates files related to cloud runner service."""
+    def __init__(self, defaults_file: str):
+        """Instantiate Cloud Run scripts object with all necessary attributes.
+
+        Args:
+            defaults_file (str): Path to the default config variables yaml.
+        """
+
+        # Parse defaults file for hidden class attributes
+        defaults = read_yaml_file(defaults_file)
+        self.__project_id = defaults['gcp']['project_id']
+        self.__pipeline_runner_service_account = defaults['gcp']['pipeline_runner_service_account']
+        self.__cloud_tasks_queue_location = defaults['gcp']['cloud_tasks_queue_location']
+        self.__cloud_tasks_queue_name = defaults['gcp']['cloud_tasks_queue_name']
+        self.__cloud_run_name = defaults['gcp']['cloud_run_name']
+        self.__cloud_run_location = defaults['gcp']['cloud_run_location']
+        self.__cloud_schedule_pattern = defaults['gcp']['cloud_schedule_pattern']
+        self.__cloud_schedule_location = defaults['gcp']['cloud_schedule_location']
+        self.__cloud_schedule_name = defaults['gcp']['cloud_schedule_name']
+
+        # Set generated scripts as public attributes
+        self.dockerfile = self._create_dockerfile()
+        self.cloudrun_base_reqs = self._create_cloudrun_base_reqs()
+        self.queueing_svc_reqs = self._create_queuing_svc_reqs()
+        self.cloudrun_base = self._create_cloudrun_base()
+        self.queueing_svc = self._create_queueing_svc()
+
+    def _create_dockerfile(self):
+        """Returns text for a Dockerfile that will be added to the cloudrun/run_pipeline directory.
+
+        Returns:
+            str: Dockerfile text.
+        """
+        return (
+            GENERATED_LICENSE +
+            'FROM python:3.9-slim\n'
+            '\n'
+            '# Allow statements and log messages to immediately appear in the Knative logs\n'
+            'ENV PYTHONUNBUFFERED True\n'
+            '\n'
+            '# Copy local code to the container image.\n'
+            'ENV APP_HOME /app\n'
+            'WORKDIR $APP_HOME\n'
+            'COPY ./ ./\n'
+            '\n'
+            '# Upgrade pip\n'
+            'RUN python -m pip install --upgrade pip\n'
+            '# Install requirements\n'
+            'RUN pip install --no-cache-dir -r /app/cloud_run/run_pipeline/requirements.txt\n'
+            '# Compile pipeline spec\n'
+            'RUN ./scripts/build_pipeline_spec.sh\n'
+            '# Change Directories\n'
+            'WORKDIR "/app/cloud_run/run_pipeline"\n'
+            '# Run flask api server\n'
+            'CMD exec gunicorn --bind :$PORT --workers 1 --threads 8 --timeout 0 main:app\n'
+        )
+
+    def _create_cloudrun_base_reqs(self):
+        """Returns the text of a cloudrun base requirements file to be written to the cloud_run/run_pipeline directory.
+
+        Returns:
+            str: Package requirements for cloudrun base.
+        """
+        return (
+            'kfp\n'
+            'google-cloud-aiplatform\n'
+            'google-cloud-pipeline-components\n'
+            'Flask\n'
+            'gunicorn\n'
+            'pyyaml\n'
+        )
+
+    def _create_queuing_svc_reqs(self):
+        """Returns the text of a queueing svc requirements file to be written to the cloud_run/queueing_svc directory.
+
+        Returns:
+            str: Package requirements for queueing svc.
+        """
+        return (
+            'google-cloud\n'
+            'google-cloud-tasks\n'
+            'google-api-python-client\n'
+            'google-cloud-run\n'
+            'google-cloud-scheduler\n'
+        )
+
+    def _create_cloudrun_base(self):
+        """Creates content for a main.py to be written to the cloud_run/run_pipeline
+        directory. This file contains code for running a flask service that will act as
+        a pipeline runner service.
+
+        Returns:
+            str: Content of cloudrun main.py.
+        """
+        return (
+            GENERATED_LICENSE +
+            f'''"""Cloud Run to run pipeline spec"""\n'''
+            f'''import logging\n'''
+            f'''import os\n'''
+            f'''from typing import Tuple\n'''
+            f'\n'
+            f'''import flask\n'''
+            f'''from google.cloud import aiplatform\n'''
+            f'''import yaml\n'''
+            f'\n'
+            f'''app = flask.Flask(__name__)\n'''
+            f'\n'
+            f'''logger = logging.getLogger()\n'''
+            f'''log_level = os.environ.get('LOG_LEVEL', 'INFO')\n'''
+            f'''logger.setLevel(log_level)\n'''
+            f'\n'
+            f'''CONFIG_FILE = '../../configs/defaults.yaml'\n'''
+            f'''PIPELINE_SPEC_PATH_LOCAL = '../../scripts/pipeline_spec/pipeline_job.json'\n'''
+            f'\n'
+            f'''@app.route('/', methods=['POST'])\n'''
+            f'''def process_request() -> flask.Response:\n'''
+            f'''    """HTTP web service to trigger pipeline execution.\n'''
+            f'\n'
+            f'''    Returns:\n'''
+            f'''        The response text, or any set of values that can be turned into a\n'''
+            f'''        Response object using `make_response`\n'''
+            f'''        <https://flask.palletsprojects.com/en/1.1.x/api/#flask.make_response>.\n'''
+            f'''    """\n'''
+            f'''    content_type = flask.request.headers['content-type']\n'''
+            f'''    if content_type == 'application/json':\n'''
+            f'''        request_json = flask.request.json\n'''
+            f'\n'
+            f'''        logging.debug('JSON Recieved:')\n'''
+            f'''        logging.debug(request_json)\n'''
+            f'\n'
+            f'''        with open(CONFIG_FILE, 'r', encoding='utf-8') as config_file:\n'''
+            f'''            config = yaml.load(config_file, Loader=yaml.FullLoader)\n'''
+            f'\n'
+            f'''        logging.debug('Calling run_pipeline()')\n'''
+            f'''        dashboard_uri, resource_name = run_pipeline(\n'''
+            f'''            project_id=config['gcp']['project_id'],\n'''
+            f'''            pipeline_root=config['pipelines']['pipeline_storage_path'],\n'''
+            f'''            pipeline_runner_sa=config['gcp']['pipeline_runner_service_account'],\n'''
+            f'''            pipeline_params=request_json,\n'''
+            f'''            pipeline_spec_path=PIPELINE_SPEC_PATH_LOCAL)\n'''
+            f'''        return flask.make_response({LEFT_BRACKET}\n'''
+            f'''            'dashboard_uri': dashboard_uri,\n'''
+            f'''            'resource_name': resource_name\n'''
+            f'''        {RIGHT_BRACKET}, 200)\n'''
+            f'\n'
+            f'''    else:\n'''
+            f'''        raise ValueError(f'Unknown content type: {LEFT_BRACKET}content_type{RIGHT_BRACKET}')\n'''
+            f'\n'
+            f'''def run_pipeline(\n'''
+            f'''    project_id: str,\n'''
+            f'''    pipeline_root: str,\n'''
+            f'''    pipeline_runner_sa: str,\n'''
+            f'''    pipeline_params: dict,\n'''
+            f'''    pipeline_spec_path: str,\n'''
+            f'''    display_name: str = 'mlops-pipeline-run',\n'''
+            f'''    enable_caching: bool = False) -> Tuple[str, str]:\n'''
+            f'''    """Executes a pipeline run.\n'''
+            f'\n'
+            f'''    Args:\n'''
+            f'''        project_id: The project_id.\n'''
+            f'''        pipeline_root: GCS location of the pipeline runs metadata.\n'''
+            f'''        pipeline_runner_sa: Service Account to runner PipelineJobs.\n'''
+            f'''        pipeline_params: Pipeline parameters values.\n'''
+            f'''        pipeline_spec_path: Location of the pipeline spec JSON.\n'''
+            f'''        display_name: Name to call the pipeline.\n'''
+            f'''        enable_caching: Should caching be enabled (Boolean)\n'''
+            f'''    """\n'''
+            f'''    logging.debug('Pipeline Parms Configured:')\n'''
+            f'''    logging.debug(pipeline_params)\n'''
+            f'\n'
+            f'''    aiplatform.init(project=project_id)\n'''
+            f'''    job = aiplatform.PipelineJob(\n'''
+            f'''        display_name = display_name,\n'''
+            f'''        template_path = pipeline_spec_path,\n'''
+            f'''        pipeline_root = pipeline_root,\n'''
+            f'''        parameter_values = pipeline_params,\n'''
+            f'''        enable_caching = enable_caching)\n'''
+            f'''    logging.debug('AI Platform job built. Submitting...')\n'''
+            f'''    job.submit(service_account=pipeline_runner_sa)\n'''
+            f'''    logging.debug('Job sent!')\n'''
+            f'''    dashboard_uri = job._dashboard_uri()\n'''
+            f'''    resource_name = job.resource_name\n'''
+            f'''    return dashboard_uri, resource_name\n'''
+            f'\n'
+            f'''if __name__ == '__main__':\n'''
+            f'''    app.run(debug=True, host='0.0.0.0', port=int(os.environ.get('PORT', 8080)))\n'''
+        )
+
+    def _create_queueing_svc(self):
+        """Creates content for a main.py to be written to the cloud_run/queueing_svc
+        directory. This file contains code for submitting a job to the cloud runner
+        service, and creating a cloud scheduler job.
+
+        Returns:
+            str: Content of queueing svc main.py.
+        """
+        return (
+            GENERATED_LICENSE +
+            f'''"""Submit pipeline job using Cloud Tasks and create Cloud Scheduler Job."""\n'''
+            f'''import argparse\n'''
+            f'''import json\n'''
+            f'\n'
+            f'''from google.cloud import run_v2\n'''
+            f'''from google.cloud import scheduler_v1\n'''
+            f'''from google.cloud import tasks_v2\n'''
+            f'\n'
+            f'''CLOUD_RUN_LOCATION = '{self.__cloud_run_location}'\n'''
+            f'''CLOUD_RUN_NAME = '{self.__cloud_run_name}'\n'''
+            f'''CLOUD_TASKS_QUEUE_LOCATION = '{self.__cloud_tasks_queue_location}'\n'''
+            f'''CLOUD_TASKS_QUEUE_NAME = '{self.__cloud_tasks_queue_name}'\n'''
+            f'''PARAMETER_VALUES_PATH = 'queueing_svc/pipeline_parameter_values.json'\n'''
+            f'''PIPELINE_RUNNER_SA = '{self.__pipeline_runner_service_account}'\n'''
+            f'''PROJECT_ID = '{self.__project_id}'\n'''
+            f'''SCHEDULE_LOCATION = '{self.__cloud_schedule_location}'\n'''
+            f'''SCHEDULE_PATTERN = '{self.__cloud_schedule_pattern}'\n'''
+            f'''SCHEDULE_NAME = '{self.__cloud_schedule_name}'\n'''
+            f'\n'
+            f'''def get_runner_svc_uri(\n'''
+            f'''    cloud_run_location: str,\n'''
+            f'''    cloud_run_name: str,\n'''
+            f'''    project_id: str):\n'''
+            f'''    """Fetches the uri for the given cloud run instance.\n'''
+            f'\n'
+            f'''    Args:\n'''
+            f'''        cloud_run_location: The location of the cloud runner service.\n'''
+            f'''        cloud_run_name: The name of the cloud runner service.\n'''
+            f'''        project_id: The project ID.\n'''
+            f'''    Returns:\n'''
+            f'''        str: Uri of the Cloud Run instance.\n'''
+            f'''    """\n'''
+            f'''    client = run_v2.ServicesClient()\n'''
+            f'''    parent = client.service_path(project_id, cloud_run_location, cloud_run_name)\n'''
+            f'''    request = run_v2.GetServiceRequest(name=parent)\n'''
+            f'''    response = client.get_service(request=request)\n'''
+            f'''    return response.uri\n'''
+            f'\n'
+            f'''def get_json_bytes(file_path: str):\n'''
+            f'''    """Reads a json file at the specified path and returns as bytes.\n'''
+            f'\n'
+            f'''    Args:\n'''
+            f'''        file_path: Path of the json file.\n'''
+            f'''    Returns:\n'''
+            f'''        bytes: Encode bytes of the file.\n'''
+            f'''    """\n'''
+            f'''    try:\n'''
+            f'''        with open(file_path, 'r', encoding='utf-8') as file:\n'''
+            f'''            data = json.load(file)\n'''
+            f'''        file.close()\n'''
+            f'''    except OSError as err:\n'''
+            f'''        raise Exception(f'Error reading json file. {LEFT_BRACKET}err{RIGHT_BRACKET}') from err\n'''
+            f'''    return json.dumps(data).encode()\n'''
+            f'\n'
+            f'''def create_cloud_task(\n'''
+            f'''    cloud_tasks_queue_location: str,\n'''
+            f'''    cloud_tasks_queue_name: str,\n'''
+            f'''    parameter_values_path: str,\n'''
+            f'''    pipeline_runner_sa: str,\n'''
+            f'''    project_id: str,\n'''
+            f'''    runner_svc_uri: str):\n'''
+            f'''    """Create a task to the queue with the runtime parameters.\n'''
+            f'\n'
+            f'''    Args:\n'''
+            f'''        cloud_run_location: The location of the cloud runner service.\n'''
+            f'''        cloud_run_name: The name of the cloud runner service.\n'''
+            f'''        cloud_tasks_queue_location: The location of the cloud tasks queue.\n'''
+            f'''        cloud_tasks_queue_name: The name of the cloud tasks queue.\n'''
+            f'''        parameter_values_path: Path to json pipeline params.\n'''
+            f'''        pipeline_runner_sa: Service Account to runner PipelineJobs.\n'''
+            f'''        project_id: The project ID.\n'''
+            f'''        runner_svc_uri: Uri of the Cloud Run instance.\n'''
+            f'''    """\n'''
+            f'''    client = tasks_v2.CloudTasksClient()\n'''
+            f'''    parent = client.queue_path(project_id, cloud_tasks_queue_location, cloud_tasks_queue_name)\n'''
+            f'''    task = {LEFT_BRACKET}\n'''
+            f'''        'http_request': {LEFT_BRACKET}\n'''
+            f'''            'http_method': tasks_v2.HttpMethod.POST,\n'''
+            f'''            'url': runner_svc_uri,\n'''
+            f'''            'oidc_token': {LEFT_BRACKET}\n'''
+            f'''                'service_account_email': pipeline_runner_sa,\n'''
+            f'''                'audience': runner_svc_uri\n'''
+            f'''            {RIGHT_BRACKET},\n'''
+            f'''            'headers': {LEFT_BRACKET}\n'''
+            f'''               'Content-Type': 'application/json'\n'''
+            f'''            {RIGHT_BRACKET}\n'''
+            f'''        {RIGHT_BRACKET}\n'''
+            f'''    {RIGHT_BRACKET}\n'''
+            f'''    task['http_request']['body'] = get_json_bytes(parameter_values_path)\n'''
+            f'''    response = client.create_task(request={LEFT_BRACKET}'parent': parent, 'task': task{RIGHT_BRACKET})\n'''
+            f'''    print(f'Created task {LEFT_BRACKET}response.name{RIGHT_BRACKET}')\n'''
+            f'\n'
+            f'''def create_cloud_scheduler_job(\n'''
+            f'''    parameter_values_path: str,\n'''
+            f'''    pipeline_runner_sa: str,\n'''
+            f'''    project_id: str,\n'''
+            f'''    runner_svc_uri: str,\n'''
+            f'''    schedule_location: str,\n'''
+            f'''    schedule_name: str,\n'''
+            f'''    schedule_pattern: str):\n'''
+            f'''    """Creates a scheduled pipeline job.\n'''
+            f'\n'
+            f'''    Args:\n'''
+            f'''        parameter_values_path: Path to json pipeline params.\n'''
+            f'''        pipeline_runner_sa: Service Account to runner PipelineJobs.\n'''
+            f'''        project_id: The project ID.\n'''
+            f'''        runner_svc_uri: Uri of the Cloud Run instance.\n'''
+            f'''        schedule_location: The location of the scheduler resource.\n'''
+            f'''        schedule_name: The name of the scheduler resource.\n'''
+            f'''        schedule_pattern: Cron formatted value used to create a Scheduled retrain job.\n'''
+            f'''    """\n'''
+            f'''    client = scheduler_v1.CloudSchedulerClient()\n'''
+            f'''    parent = f'projects/{LEFT_BRACKET}project_id{RIGHT_BRACKET}/locations/{LEFT_BRACKET}schedule_location{RIGHT_BRACKET}'\n'''
+            f'''    name = f'{LEFT_BRACKET}parent{RIGHT_BRACKET}/jobs/{LEFT_BRACKET}schedule_name{RIGHT_BRACKET}'\n'''
+            f'\n'
+            f'''    request = scheduler_v1.ListJobsRequest(parent=parent)\n'''
+            f'''    page_result = client.list_jobs(request=request)\n'''
+            f'''    for response in page_result:\n'''
+            f'''        if response.name == name:\n'''
+            f'''            print(f'Cloud Scheduler {LEFT_BRACKET}schedule_name{RIGHT_BRACKET} resource already exists in '\n'''
+            f'''                  f'project {LEFT_BRACKET}project_id{RIGHT_BRACKET}.')\n'''
+            f'''            return\n'''
+            f'\n'
+            f'''    oidc_token = scheduler_v1.OidcToken(\n'''
+            f'''        service_account_email=pipeline_runner_sa,\n'''
+            f'''        audience=runner_svc_uri)\n'''
+            f'\n'
+            f'''    target = scheduler_v1.HttpTarget(\n'''
+            f'''       uri=runner_svc_uri,\n'''
+            f'''        http_method=scheduler_v1.HttpMethod(1), # HTTP POST\n'''
+            f'''        headers={LEFT_BRACKET}'Content-Type': 'application/json'{RIGHT_BRACKET},\n'''
+            f'''        body=get_json_bytes(parameter_values_path),\n'''
+            f'''        oidc_token=oidc_token)\n'''
+            f'\n'
+            f'''    job = scheduler_v1.Job(\n'''
+            f'''       name=f'{LEFT_BRACKET}parent{RIGHT_BRACKET}/jobs/{LEFT_BRACKET}schedule_name{RIGHT_BRACKET}',\n'''
+            f'''        description='AutoMLOps cloud scheduled run.',\n'''
+            f'''        http_target=target,\n'''
+            f'''        schedule=schedule_pattern)\n'''
+            f'\n'
+            f'''    request = scheduler_v1.CreateJobRequest(\n'''
+            f'''        parent=parent,\n'''
+            f'''        job=job)\n'''
+            f'\n'
+            f'''    response = client.create_job(request=request)\n'''
+            f'''    print(response)\n'''
+            f'\n'
+            f'''if __name__ == '__main__':\n'''
+            f'''    parser = argparse.ArgumentParser()\n'''
+            f'''    parser.add_argument('--setting', type=str,\n'''
+            f'''                       help='The config file for setting default values.')\n'''
+            f'''    args = parser.parse_args()\n'''
+            f'\n'
+            f'''    uri = get_runner_svc_uri(\n'''
+            f'''        cloud_run_location=CLOUD_RUN_LOCATION,\n'''
+            f'''        cloud_run_name=CLOUD_RUN_NAME,\n'''
+            f'''        project_id=PROJECT_ID)\n'''
+            f'\n'
+            f'''    if args.setting == 'queue_job':\n'''
+            f'''        create_cloud_task(\n'''
+            f'''            cloud_tasks_queue_location=CLOUD_TASKS_QUEUE_LOCATION,\n'''
+            f'''            cloud_tasks_queue_name=CLOUD_TASKS_QUEUE_NAME,\n'''
+            f'''            parameter_values_path=PARAMETER_VALUES_PATH,\n'''
+            f'''            pipeline_runner_sa=PIPELINE_RUNNER_SA,\n'''
+            f'''            project_id=PROJECT_ID,\n'''
+            f'''            runner_svc_uri=uri)\n'''
+            f'\n'
+            f'''    if args.setting == 'schedule_job':\n'''
+            f'''        create_cloud_scheduler_job(\n'''
+            f'''            parameter_values_path=PARAMETER_VALUES_PATH,\n'''
+            f'''            pipeline_runner_sa=PIPELINE_RUNNER_SA,\n'''
+            f'''            project_id=PROJECT_ID,\n'''
+            f'''            runner_svc_uri=uri,\n'''
+            f'''            schedule_location=SCHEDULE_LOCATION,\n'''
+            f'''            schedule_name=SCHEDULE_NAME,\n'''
+            f'''            schedule_pattern=SCHEDULE_PATTERN)\n''')
```

### Comparing `google-cloud-automlops-1.1.0/AutoMLOps/PipelineBuilder.py` & `google-cloud-automlops-1.1.1/AutoMLOps/frameworks/kfp/constructs/pipeline.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,284 +8,170 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Builds pipeline files."""
+"""Code strings for a kfp pipeline."""
 
-# pylint: disable=C0103
 # pylint: disable=line-too-long
 
-import json
-from typing import Callable, Dict, List, Optional
+from typing import Dict, List
 
-from AutoMLOps import BuilderUtils
-
-DEFAULT_PIPELINE_NAME = 'automlops-pipeline'
-
-def formalize(custom_training_job_specs: List[Dict],
-              defaults_file: str,
-              pipeline_parameter_values: dict,
-              top_lvl_name: str):
-    """Constructs and writes pipeline.py, pipeline_runner.py, and pipeline_parameter_values.json files.
-        pipeline.py: Generates a Kubeflow pipeline spec from custom components.
-        pipeline_runner.py: Sends a PipelineJob to Vertex AI using pipeline spec.
-        pipeline_parameter_values.json: Provides runtime parameters for the PipelineJob.
-
-    Args:
-        custom_training_job_specs: Specifies the specs to run the training job with.
-        defaults_file: Path to the default config variables yaml.
-        pipeline_parameter_values: Dictionary of runtime parameters for the PipelineJob.
-        top_lvl_name: Top directory name.
-    Raises:
-        Exception: If an error is encountered reading/writing to a file.
-    """
-    defaults = BuilderUtils.read_yaml_file(defaults_file)
-    pipeline_file = top_lvl_name + 'pipelines/pipeline.py'
-    pipeline_runner_file = top_lvl_name + 'pipelines/pipeline_runner.py'
-    pipeline_params_file = top_lvl_name + BuilderUtils.PARAMETER_VALUES_PATH
-    # construct pipeline.py
-    pipeline_imports = get_pipeline_imports(custom_training_job_specs, defaults['gcp']['project_id'])
-    pipeline_argparse = get_pipeline_argparse()
-    try:
-        with open(pipeline_file, 'r+', encoding='utf-8') as file:
-            pipeline_scaffold = file.read()
-            file.seek(0, 0)
-            file.write(BuilderUtils.LICENSE)
-            file.write(pipeline_imports)
-            for line in pipeline_scaffold.splitlines():
-                file.write('    ' + line + '\n')
-            file.write(pipeline_argparse)
-        file.close()
-    except OSError as err:
-        raise OSError(f'Error interacting with file. {err}') from err
-    # construct pipeline_runner.py
-    BuilderUtils.write_file(pipeline_runner_file, get_pipeline_runner(), 'w+')
-    # construct pipeline_parameter_values.json
-    serialized_params = json.dumps(pipeline_parameter_values, indent=4)
-    BuilderUtils.write_file(pipeline_params_file, serialized_params, 'w+')
-
-def get_pipeline_imports(custom_training_job_specs: List[Dict], project_id: str) -> str:
-    """Generates python code that imports modules and loads all custom components.
-    Args:
-        custom_training_job_specs: Specifies the specs to run the training job with.
-        project_id: The project_id to run the pipeline. 
-
-    Returns:
-        str: Python pipeline_imports code.
-    """
-    components_list = BuilderUtils.get_components_list(full_path=False)
-    gcpc_imports = (
-        'from functools import partial\n'
-        'from google_cloud_pipeline_components.v1.custom_job import create_custom_training_job_op_from_component\n')
-    quote = '\''
-    newline_tab = '\n    '
-    return (
-        f'''import argparse\n'''
-        f'''import os\n'''
-        f'''{gcpc_imports if custom_training_job_specs else ''}'''
-        f'''import kfp\n'''
-        f'''from kfp.v2 import compiler, dsl\n'''
-        f'''from kfp.v2.dsl import *\n'''
-        f'''from typing import *\n'''
-        f'''import yaml\n'''
-        f'\n'
-        f'''def load_custom_component(component_name: str):\n'''
-        f'''    component_path = os.path.join('components',\n'''
-        f'''                                component_name,\n'''
-        f'''                              'component.yaml')\n'''
-        f'''    return kfp.components.load_component_from_file(component_path)\n'''
-        f'\n'
-        f'''def create_training_pipeline(pipeline_job_spec_path: str):\n'''
-        f'''    {newline_tab.join(f'{component} = load_custom_component(component_name={quote}{component}{quote})' for component in components_list)}\n'''
-        f'\n'
-        f'''{get_custom_job_specs(custom_training_job_specs, project_id)}''')
-
-def get_custom_job_specs(custom_training_job_specs: List[Dict], project_id: str) -> str:
-    """Generates python code that creates a custom training op from the specified component.
-    Args:
-        custom_training_job_specs: Specifies the specs to run the training job with.
-        project_id: The project_id to run the pipeline. 
-
-    Returns:
-        str: Python custom training op code.
-    """
-    quote = '\''
-    newline_tab = '\n    '
-    output_string = '' if not custom_training_job_specs else (
-            f'''    {newline_tab.join(f'{spec["component_spec"]}_custom_training_job_specs = {format_spec_dict(spec)}' for spec in custom_training_job_specs)}'''
+from AutoMLOps.utils.utils import get_components_list, format_spec_dict
+from AutoMLOps.utils.constants import GENERATED_LICENSE
+from AutoMLOps.frameworks.base import Pipeline
+
+class KfpPipeline(Pipeline):
+    """Child class that generates files related to kfp pipelines."""
+    def __init__(self, custom_training_job_specs: List[Dict], defaults_file: str):
+        """Instantiate Pipeline scripts object with all necessary attributes.
+
+        Args:
+            custom_training_job_specs (List[Dict]): Specifies the specs to run the training job with.
+            defaults_file (str): Path to the default config variables yaml.
+        """
+        super().__init__(custom_training_job_specs, defaults_file)
+        self.pipeline_imports = self._get_pipeline_imports()
+        self.pipeline_argparse = self._get_pipeline_argparse()
+        self.pipeline_runner = self._get_pipeline_runner()
+
+    def _get_pipeline_imports(self):
+        """Generates python code that imports modules and loads all custom components.
+
+        Returns:
+            str: Python pipeline_imports code.
+        """
+        components_list = get_components_list(full_path=False)
+        gcpc_imports = (
+            'from functools import partial\n'
+            'from google_cloud_pipeline_components.v1.custom_job import create_custom_training_job_op_from_component\n')
+        quote = '\''
+        newline_tab = '\n    '
+
+        # If there is a custom training job specified, write those to feed to pipeline imports
+        if not self._custom_training_job_specs:
+            custom_specs = ''
+        else:
+            custom_specs = (
+                f'''    {newline_tab.join(f'{spec["component_spec"]}_custom_training_job_specs = {format_spec_dict(spec)}' for spec in self._custom_training_job_specs)}'''
+                f'\n'
+                f'''    {newline_tab.join(f'{spec["component_spec"]}_job_op = create_custom_training_job_op_from_component(**{spec["component_spec"]}_custom_training_job_specs)' for spec in self._custom_training_job_specs)}'''
+                f'\n'
+                f'''    {newline_tab.join(f'{spec["component_spec"]} = partial({spec["component_spec"]}_job_op, project={quote}{self._project_id}{quote})' for spec in self._custom_training_job_specs)}'''        
+                f'\n')
+
+        # Return standard code and customized specs
+        return (
+            f'''import argparse\n'''
+            f'''import os\n'''
+            f'''{gcpc_imports if self._custom_training_job_specs else ''}'''
+            f'''import kfp\n'''
+            f'''from kfp.v2 import compiler, dsl\n'''
+            f'''from kfp.v2.dsl import *\n'''
+            f'''from typing import *\n'''
+            f'''import yaml\n'''
+            f'\n'
+            f'''def load_custom_component(component_name: str):\n'''
+            f'''    component_path = os.path.join('components',\n'''
+            f'''                                component_name,\n'''
+            f'''                              'component.yaml')\n'''
+            f'''    return kfp.components.load_component_from_file(component_path)\n'''
             f'\n'
-            f'''    {newline_tab.join(f'{spec["component_spec"]}_job_op = create_custom_training_job_op_from_component(**{spec["component_spec"]}_custom_training_job_specs)' for spec in custom_training_job_specs)}'''
+            f'''def create_training_pipeline(pipeline_job_spec_path: str):\n'''
+            f'''    {newline_tab.join(f'{component} = load_custom_component(component_name={quote}{component}{quote})' for component in components_list)}\n'''
             f'\n'
-            f'''    {newline_tab.join(f'{spec["component_spec"]} = partial({spec["component_spec"]}_job_op, project={quote}{project_id}{quote})' for spec in custom_training_job_specs)}'''        
-            f'\n')
-    return output_string
-
-def format_spec_dict(job_spec: dict) -> str:
-    """Takes in a job spec dictionary and removes the quotes around the component op name. 
-       e.g. 'component_spec': 'train_model' becomes 'component_spec': train_model.
-       This is necessary to in order for the op to be callable within the Python code.
-
-    Args:
-        job_spec: Dictionary with job spec info.
-
-    Returns:
-        str: Python formatted dictionary code.
-    """
-    quote = '\''
-    left_bracket = '{'
-    right_bracket = '}'
-    newline = '\n'
-
-    return (
-        f'''{left_bracket}\n'''
-        f'''    {f'{newline}    '.join(f"   {quote}{k}{quote}: {quote if k != 'component_spec' else ''}{v}{quote if k != 'component_spec' else ''}," for k, v in job_spec.items())}{newline}'''
-        f'''    {right_bracket}\n''')
-
-def get_pipeline_argparse() -> str:
-    """Generates python code that loads default pipeline parameters from the defaults config_file.
-
-    Returns:
-        str: Python pipeline_argparse code.
-    """
-    return (
-        '''if __name__ == '__main__':\n'''
-        '''    parser = argparse.ArgumentParser()\n'''
-        '''    parser.add_argument('--config', type=str,\n'''
-        '''                       help='The config file for setting default values.')\n'''
-        '\n'
-        '''    args = parser.parse_args()\n'''
-        '\n'
-        '''    with open(args.config, 'r', encoding='utf-8') as config_file:\n'''
-        '''        config = yaml.load(config_file, Loader=yaml.FullLoader)\n'''
-        '\n'
-        '''    pipeline = create_training_pipeline(\n'''
-        '''        pipeline_job_spec_path=config['pipelines']['pipeline_job_spec_path'])\n''')
-
-def get_pipeline_runner() -> str:
-    """Generates python code that sends a PipelineJob to Vertex AI.
-
-    Returns:
-        str: Python pipeline_runner code.
-    """
-    return (BuilderUtils.LICENSE +
-        '''import argparse\n'''
-        '''import json\n'''
-        '''import logging\n'''
-        '''import os\n'''
-        '''import yaml\n'''
-        '\n'
-        '''from google.cloud import aiplatform\n'''
-        '\n'
-        '''logger = logging.getLogger()\n'''
-        '''log_level = os.environ.get('LOG_LEVEL', 'INFO')\n'''
-        '''logger.setLevel(log_level)\n'''
-        '\n'
-        '''def run_pipeline(\n'''
-        '''    project_id: str,\n'''
-        '''    pipeline_root: str,\n'''
-        '''    pipeline_runner_sa: str,\n'''
-        '''    parameter_values_path: str,\n'''
-        '''    pipeline_spec_path: str,\n'''
-        '''    display_name: str = 'mlops-pipeline-run',\n'''
-        '''    enable_caching: bool = False):\n'''
-        '''    """Executes a pipeline run.\n'''
-        '\n'
-        '''    Args:\n'''
-        '''        project_id: The project_id.\n'''
-        '''        pipeline_root: GCS location of the pipeline runs metadata.\n'''
-        '''        pipeline_runner_sa: Service Account to runner PipelineJobs.\n'''
-        '''        parameter_values_path: Location of parameter values JSON.\n'''
-        '''        pipeline_spec_path: Location of the pipeline spec JSON.\n'''
-        '''        display_name: Name to call the pipeline.\n'''
-        '''        enable_caching: Should caching be enabled (Boolean)\n'''
-        '''    """\n'''
-        '''    with open(parameter_values_path, 'r') as file:\n'''
-        '''        try:\n'''
-        '''            pipeline_params = json.load(file)\n'''
-        '''        except ValueError as exc:\n'''
-        '''            print(exc)\n'''
-        '''    logging.debug('Pipeline Parms Configured:')\n'''
-        '''    logging.debug(pipeline_params)\n'''
-        '\n'
-        '''    aiplatform.init(project=project_id)\n'''
-        '''    job = aiplatform.PipelineJob(\n'''
-        '''        display_name = display_name,\n'''
-        '''        template_path = pipeline_spec_path,\n'''
-        '''        pipeline_root = pipeline_root,\n'''
-        '''        parameter_values = pipeline_params,\n'''
-        '''        enable_caching = enable_caching)\n'''
-        '''    logging.debug('AI Platform job built. Submitting...')\n'''
-        '''    job.submit(service_account=pipeline_runner_sa)\n'''
-        '''    logging.debug('Job sent!')\n'''
-        '\n'
-        '''if __name__ == '__main__':\n'''
-        '''    parser = argparse.ArgumentParser()\n'''
-        '''    parser.add_argument('--config', type=str,\n'''
-        '''                        help='The config file for setting default values.')\n'''
-        '''    args = parser.parse_args()\n'''
-        '\n'
-        '''    with open(args.config, 'r', encoding='utf-8') as config_file:\n'''
-        '''        config = yaml.load(config_file, Loader=yaml.FullLoader)\n'''
-        '\n'
-        '''    run_pipeline(project_id=config['gcp']['project_id'],\n'''
-        '''                 pipeline_root=config['pipelines']['pipeline_storage_path'],\n'''
-        '''                 pipeline_runner_sa=config['gcp']['pipeline_runner_service_account'],\n'''
-        '''                 parameter_values_path=config['pipelines']['parameter_values_path'],\n'''
-        '''                 pipeline_spec_path=config['pipelines']['pipeline_job_spec_path']) \n''')
-
-def create_pipeline_scaffold(func: Optional[Callable] = None,
-                             *,
-                             name: Optional[str] = None,
-                             description: Optional[str] = None):
-    """Creates a temporary pipeline scaffold which will
-       be used by the formalize function.
-
-    Args:
-        func: The python function to create a pipeline from. The function
-            should have type annotations for all its arguments, indicating how
-            it is intended to be used (e.g. as an input/output Artifact object,
-            a plain parameter, or a path to a file).
-        name: The name of the pipeline.
-        description: Short description of what the pipeline does.
-    """
-    pipeline_scaffold = (get_pipeline_decorator(name, description) +
-                         BuilderUtils.get_function_source_definition(func) +
-                         get_compile_step(func.__name__))
-    BuilderUtils.make_dirs([BuilderUtils.TMPFILES_DIR]) # if it doesn't already exist
-    BuilderUtils.write_file(BuilderUtils.PIPELINE_TMPFILE, pipeline_scaffold, 'w')
-
-def get_pipeline_decorator(name: Optional[str] = None,
-                           description: Optional[str] = None):
-    """Creates the kfp pipeline decorator.
-
-    Args:
-        name: The name of the pipeline.
-        description: Short description of what the pipeline does.
-
-    Returns:
-        str: Python compile function call.
-    """
-    default_name = DEFAULT_PIPELINE_NAME if not name else name
-    name_str = f'''(\n    name='{default_name}',\n'''
-    desc_str = f'''    description='{description}',\n''' if description else ''
-    ending_str = ')\n'
-    return '@dsl.pipeline' + name_str + desc_str + ending_str
-
-def get_compile_step(func_name: str):
-    """Creates the compile function call.
-
-    Args:
-        func_name: The name of the pipeline function.
-
-    Returns:
-        str: Python compile function call.
-    """
-    return (
-        f'\n'
-        f'compiler.Compiler().compile(\n'
-        f'    pipeline_func={func_name},\n'
-        f'    package_path=pipeline_job_spec_path)\n'
-        f'\n'
-    )
+            f'''{custom_specs}''')
+
+    def _get_pipeline_argparse(self):
+        """Generates python code that loads default pipeline parameters from the defaults config_file.
+
+        Returns:
+            str: Python pipeline_argparse code.
+        """
+        return (
+            '''if __name__ == '__main__':\n'''
+            '''    parser = argparse.ArgumentParser()\n'''
+            '''    parser.add_argument('--config', type=str,\n'''
+            '''                       help='The config file for setting default values.')\n'''
+            '\n'
+            '''    args = parser.parse_args()\n'''
+            '\n'
+            '''    with open(args.config, 'r', encoding='utf-8') as config_file:\n'''
+            '''        config = yaml.load(config_file, Loader=yaml.FullLoader)\n'''
+            '\n'
+            '''    pipeline = create_training_pipeline(\n'''
+            '''        pipeline_job_spec_path=config['pipelines']['pipeline_job_spec_path'])\n''')
+
+    def _get_pipeline_runner(self):
+        """Generates python code that sends a PipelineJob to Vertex AI.
+
+        Returns:
+            str: Python pipeline_runner code.
+        """
+        return (
+            GENERATED_LICENSE +
+            '''import argparse\n'''
+            '''import json\n'''
+            '''import logging\n'''
+            '''import os\n'''
+            '''import yaml\n'''
+            '\n'
+            '''from google.cloud import aiplatform\n'''
+            '\n'
+            '''logger = logging.getLogger()\n'''
+            '''log_level = os.environ.get('LOG_LEVEL', 'INFO')\n'''
+            '''logger.setLevel(log_level)\n'''
+            '\n'
+            '''def run_pipeline(\n'''
+            '''    project_id: str,\n'''
+            '''    pipeline_root: str,\n'''
+            '''    pipeline_runner_sa: str,\n'''
+            '''    parameter_values_path: str,\n'''
+            '''    pipeline_spec_path: str,\n'''
+            '''    display_name: str = 'mlops-pipeline-run',\n'''
+            '''    enable_caching: bool = False):\n'''
+            '''    """Executes a pipeline run.\n'''
+            '\n'
+            '''    Args:\n'''
+            '''        project_id: The project_id.\n'''
+            '''        pipeline_root: GCS location of the pipeline runs metadata.\n'''
+            '''        pipeline_runner_sa: Service Account to runner PipelineJobs.\n'''
+            '''        parameter_values_path: Location of parameter values JSON.\n'''
+            '''        pipeline_spec_path: Location of the pipeline spec JSON.\n'''
+            '''        display_name: Name to call the pipeline.\n'''
+            '''        enable_caching: Should caching be enabled (Boolean)\n'''
+            '''    """\n'''
+            '''    with open(parameter_values_path, 'r') as file:\n'''
+            '''        try:\n'''
+            '''            pipeline_params = json.load(file)\n'''
+            '''        except ValueError as exc:\n'''
+            '''            print(exc)\n'''
+            '''    logging.debug('Pipeline Parms Configured:')\n'''
+            '''    logging.debug(pipeline_params)\n'''
+            '\n'
+            '''    aiplatform.init(project=project_id)\n'''
+            '''    job = aiplatform.PipelineJob(\n'''
+            '''        display_name = display_name,\n'''
+            '''        template_path = pipeline_spec_path,\n'''
+            '''        pipeline_root = pipeline_root,\n'''
+            '''        parameter_values = pipeline_params,\n'''
+            '''        enable_caching = enable_caching)\n'''
+            '''    logging.debug('AI Platform job built. Submitting...')\n'''
+            '''    job.submit(service_account=pipeline_runner_sa)\n'''
+            '''    logging.debug('Job sent!')\n'''
+            '\n'
+            '''if __name__ == '__main__':\n'''
+            '''    parser = argparse.ArgumentParser()\n'''
+            '''    parser.add_argument('--config', type=str,\n'''
+            '''                        help='The config file for setting default values.')\n'''
+            '''    args = parser.parse_args()\n'''
+            '\n'
+            '''    with open(args.config, 'r', encoding='utf-8') as config_file:\n'''
+            '''        config = yaml.load(config_file, Loader=yaml.FullLoader)\n'''
+            '\n'
+            '''    run_pipeline(project_id=config['gcp']['project_id'],\n'''
+            '''                 pipeline_root=config['pipelines']['pipeline_storage_path'],\n'''
+            '''                 pipeline_runner_sa=config['gcp']['pipeline_runner_service_account'],\n'''
+            '''                 parameter_values_path=config['pipelines']['parameter_values_path'],\n'''
+            '''                 pipeline_spec_path=config['pipelines']['pipeline_job_spec_path']) \n''')
```

### Comparing `google-cloud-automlops-1.1.0/AutoMLOps/__init__.py` & `google-cloud-automlops-1.1.1/AutoMLOps/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,10 +19,10 @@
 import, with the end goal of becoming a Jupyter plugin to Vertex
 Workbench managed notebooks. The tool will generate yaml-component
 definitions, complete with Dockerfiles and requirements.txts for all
 Kubeflow components defined in a notebook. It will also generate a
 series of directories to support the creation of Vertex Pipelines.
 """
 # pylint: disable=invalid-name
-__version__ = '1.1.0'
+__version__ = '1.1.1'
 __author__ = 'Sean Rastatter'
 __credits__ = 'Google'
```

### Comparing `google-cloud-automlops-1.1.0/LICENSE` & `google-cloud-automlops-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.0/PKG-INFO` & `google-cloud-automlops-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-automlops
-Version: 1.1.0
+Version: 1.1.1
 Summary: AutoMLOps is a service that generates a production-style         MLOps pipeline from Jupyter Notebooks.
 Home-page: https://github.com/GoogleCloudPlatform/automlops
 Author: Sean Rastatter
 Author-email: srastatter@google.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -247,15 +247,15 @@
 
 # Contributors
 
 [Sean Rastatter](mailto:srastatter@google.com): Technical Lead
 
 [Tony DiLoreto](mailto:tonydiloreto@google.com): Project Manager
 
-[Allegra Noto](mailto:allegranoto@google.com): Engineer
+[Allegra Noto](mailto:allegranoto@google.com): Senior Project Engineer
 
 # Disclaimer
 
 **This is not an officially supported Google product.**
 
 Copyright 2023 Google LLC. All Rights Reserved.
```

### Comparing `google-cloud-automlops-1.1.0/README.md` & `google-cloud-automlops-1.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -226,15 +226,15 @@
 
 # Contributors
 
 [Sean Rastatter](mailto:srastatter@google.com): Technical Lead
 
 [Tony DiLoreto](mailto:tonydiloreto@google.com): Project Manager
 
-[Allegra Noto](mailto:allegranoto@google.com): Engineer
+[Allegra Noto](mailto:allegranoto@google.com): Senior Project Engineer
 
 # Disclaimer
 
 **This is not an officially supported Google product.**
 
 Copyright 2023 Google LLC. All Rights Reserved.
```

### Comparing `google-cloud-automlops-1.1.0/google_cloud_automlops.egg-info/PKG-INFO` & `google-cloud-automlops-1.1.1/google_cloud_automlops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-automlops
-Version: 1.1.0
+Version: 1.1.1
 Summary: AutoMLOps is a service that generates a production-style         MLOps pipeline from Jupyter Notebooks.
 Home-page: https://github.com/GoogleCloudPlatform/automlops
 Author: Sean Rastatter
 Author-email: srastatter@google.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -247,15 +247,15 @@
 
 # Contributors
 
 [Sean Rastatter](mailto:srastatter@google.com): Technical Lead
 
 [Tony DiLoreto](mailto:tonydiloreto@google.com): Project Manager
 
-[Allegra Noto](mailto:allegranoto@google.com): Engineer
+[Allegra Noto](mailto:allegranoto@google.com): Senior Project Engineer
 
 # Disclaimer
 
 **This is not an officially supported Google product.**
 
 Copyright 2023 Google LLC. All Rights Reserved.
```

### Comparing `google-cloud-automlops-1.1.0/setup.py` & `google-cloud-automlops-1.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,31 +8,32 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Setup AutoMLOps modules"""
+from setuptools import find_packages
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as file:
     readme_contents = file.read()
 
 setup(
     name='google-cloud-automlops',
-    version='1.1.0',
+    version='1.1.1',
     description='AutoMLOps is a service that generates a production-style \
         MLOps pipeline from Jupyter Notebooks.',
     long_description=readme_contents,
     long_description_content_type='text/markdown',
     url='https://github.com/GoogleCloudPlatform/automlops',
     author='Sean Rastatter',
     author_email='srastatter@google.com',
     license='Apache-2.0',
-    packages=['AutoMLOps'],
+    packages=find_packages(),
     install_requires=['docopt==0.6.2',
                       'docstring-parser==0.15',
                       'pipreqs==0.4.11',
                       'PyYAML==5.4.1',
                       'yarg==0.1.9'],
     classifiers=[
         'Development Status :: 4 - Beta',
```

