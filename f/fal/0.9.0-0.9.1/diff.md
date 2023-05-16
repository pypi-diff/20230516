# Comparing `tmp/fal-0.9.0.tar.gz` & `tmp/fal-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fal-0.9.0.tar", max compression
+gzip compressed data, was "fal-0.9.1.tar", max compression
```

## Comparing `fal-0.9.0.tar` & `fal-0.9.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0    11804 2023-05-12 18:03:34.238037 fal-0.9.0/README.md
--rw-r--r--   0        0        0     2617 2023-05-12 18:03:45.242026 fal-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      221 2023-05-12 18:03:34.246038 fal-0.9.0/src/fal/__init__.py
--rw-r--r--   0        0        0       21 2023-05-12 18:03:34.246038 fal-0.9.0/src/fal/cli/__init__.py
--rw-r--r--   0        0        0     8499 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/cli/args.py
--rw-r--r--   0        0        0     2120 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/cli/cli.py
--rw-r--r--   0        0        0     5469 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/cli/dbt_runner.py
--rw-r--r--   0        0        0     6159 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/cli/fal_runner.py
--rw-r--r--   0        0        0     4430 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/cli/flow_runner.py
--rw-r--r--   0        0        0       56 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/cli/model_generator/__init__.py
--rw-r--r--   0        0        0     5505 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/cli/model_generator/model_generator.py
--rw-r--r--   0        0        0     3180 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/cli/model_generator/module_check.py
--rw-r--r--   0        0        0     9742 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/cli/selectors.py
--rw-r--r--   0        0        0    12306 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/fal_script.py
--rw-r--r--   0        0        0        0 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/feature_store/__init__.py
--rw-r--r--   0        0        0      401 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/feature_store/feature.py
--rw-r--r--   0        0        0     8394 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/node_graph.py
--rw-r--r--   0        0        0        0 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/packages/__init__.py
--rw-r--r--   0        0        0     1603 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/packages/bridge.py
--rw-r--r--   0        0        0     5332 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/packages/dependency_analysis.py
--rw-r--r--   0        0        0      793 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/packages/environments/__init__.py
--rw-r--r--   0        0        0     9482 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/packages/environments/base.py
--rw-r--r--   0        0        0     4395 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/packages/environments/conda.py
--rw-r--r--   0        0        0     3369 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/packages/environments/virtual_env.py
--rw-r--r--   0        0        0     4776 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/packages/isolated_runner.py
--rw-r--r--   0        0        0        0 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/planner/__init__.py
--rw-r--r--   0        0        0     5635 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/planner/executor.py
--rw-r--r--   0        0        0     6475 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/planner/plan.py
--rw-r--r--   0        0        0     6761 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/planner/schedule.py
--rw-r--r--   0        0        0     9041 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/planner/tasks.py
--rw-r--r--   0        0        0        0 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/telemetry/__init__.py
--rw-r--r--   0        0        0    11416 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/telemetry/telemetry.py
--rw-r--r--   0        0        0     3043 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/typing.py
--rw-r--r--   0        0        0     1711 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/utils.py
--rw-r--r--   0        0        0        0 2023-05-12 18:03:34.250038 fal-0.9.0/src/faldbt/__init__.py
--rw-r--r--   0        0        0    24156 2023-05-12 18:03:34.250038 fal-0.9.0/src/faldbt/lib.py
--rw-r--r--   0        0        0     3273 2023-05-12 18:03:34.250038 fal-0.9.0/src/faldbt/logger.py
--rw-r--r--   0        0        0     1850 2023-05-12 18:03:34.250038 fal-0.9.0/src/faldbt/magics.py
--rw-r--r--   0        0        0     8806 2023-05-12 18:03:34.250038 fal-0.9.0/src/faldbt/parse.py
--rw-r--r--   0        0        0    26552 2023-05-12 18:03:34.250038 fal-0.9.0/src/faldbt/project.py
--rw-r--r--   0        0        0        0 2023-05-12 18:03:34.250038 fal-0.9.0/src/faldbt/utils/__init__.py
--rw-r--r--   0        0        0     1970 2023-05-12 18:03:34.250038 fal-0.9.0/src/faldbt/utils/yaml_helper.py
--rw-r--r--   0        0        0      317 2023-05-12 18:03:34.250038 fal-0.9.0/src/faldbt/version.py
--rw-r--r--   0        0        0       33 2023-05-12 18:03:34.250038 fal-0.9.0/tests/_fal_testing/__init__.py
--rw-r--r--   0        0        0     1786 2023-05-12 18:03:34.250038 fal-0.9.0/tests/_fal_testing/utils.py
--rw-r--r--   0        0        0    13990 1970-01-01 00:00:00.000000 fal-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0    11804 2023-05-16 14:16:33.206267 fal-0.9.1/README.md
+-rw-r--r--   0        0        0     2619 2023-05-16 14:16:48.306693 fal-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      221 2023-05-16 14:16:33.214268 fal-0.9.1/src/fal/__init__.py
+-rw-r--r--   0        0        0       21 2023-05-16 14:16:33.214268 fal-0.9.1/src/fal/cli/__init__.py
+-rw-r--r--   0        0        0     8499 2023-05-16 14:16:33.214268 fal-0.9.1/src/fal/cli/args.py
+-rw-r--r--   0        0        0     2120 2023-05-16 14:16:33.214268 fal-0.9.1/src/fal/cli/cli.py
+-rw-r--r--   0        0        0     5469 2023-05-16 14:16:33.214268 fal-0.9.1/src/fal/cli/dbt_runner.py
+-rw-r--r--   0        0        0     5815 2023-05-16 14:16:33.214268 fal-0.9.1/src/fal/cli/fal_runner.py
+-rw-r--r--   0        0        0     4430 2023-05-16 14:16:33.214268 fal-0.9.1/src/fal/cli/flow_runner.py
+-rw-r--r--   0        0        0       56 2023-05-16 14:16:33.214268 fal-0.9.1/src/fal/cli/model_generator/__init__.py
+-rw-r--r--   0        0        0     5505 2023-05-16 14:16:33.218268 fal-0.9.1/src/fal/cli/model_generator/model_generator.py
+-rw-r--r--   0        0        0     3180 2023-05-16 14:16:33.218268 fal-0.9.1/src/fal/cli/model_generator/module_check.py
+-rw-r--r--   0        0        0     9742 2023-05-16 14:16:33.218268 fal-0.9.1/src/fal/cli/selectors.py
+-rw-r--r--   0        0        0    12306 2023-05-16 14:16:33.218268 fal-0.9.1/src/fal/fal_script.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:16:33.218268 fal-0.9.1/src/fal/feature_store/__init__.py
+-rw-r--r--   0        0        0      401 2023-05-16 14:16:33.218268 fal-0.9.1/src/fal/feature_store/feature.py
+-rw-r--r--   0        0        0     8394 2023-05-16 14:16:33.218268 fal-0.9.1/src/fal/node_graph.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:16:33.218268 fal-0.9.1/src/fal/packages/__init__.py
+-rw-r--r--   0        0        0     1603 2023-05-16 14:16:33.218268 fal-0.9.1/src/fal/packages/bridge.py
+-rw-r--r--   0        0        0     5332 2023-05-16 14:16:33.218268 fal-0.9.1/src/fal/packages/dependency_analysis.py
+-rw-r--r--   0        0        0      793 2023-05-16 14:16:33.218268 fal-0.9.1/src/fal/packages/environments/__init__.py
+-rw-r--r--   0        0        0     9482 2023-05-16 14:16:33.218268 fal-0.9.1/src/fal/packages/environments/base.py
+-rw-r--r--   0        0        0     4395 2023-05-16 14:16:33.218268 fal-0.9.1/src/fal/packages/environments/conda.py
+-rw-r--r--   0        0        0     3369 2023-05-16 14:16:33.218268 fal-0.9.1/src/fal/packages/environments/virtual_env.py
+-rw-r--r--   0        0        0     4776 2023-05-16 14:16:33.218268 fal-0.9.1/src/fal/packages/isolated_runner.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:16:33.218268 fal-0.9.1/src/fal/planner/__init__.py
+-rw-r--r--   0        0        0     5635 2023-05-16 14:16:33.218268 fal-0.9.1/src/fal/planner/executor.py
+-rw-r--r--   0        0        0     6475 2023-05-16 14:16:33.218268 fal-0.9.1/src/fal/planner/plan.py
+-rw-r--r--   0        0        0     6761 2023-05-16 14:16:33.218268 fal-0.9.1/src/fal/planner/schedule.py
+-rw-r--r--   0        0        0     9041 2023-05-16 14:16:33.218268 fal-0.9.1/src/fal/planner/tasks.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:16:33.218268 fal-0.9.1/src/fal/telemetry/__init__.py
+-rw-r--r--   0        0        0    11416 2023-05-16 14:16:33.218268 fal-0.9.1/src/fal/telemetry/telemetry.py
+-rw-r--r--   0        0        0     3043 2023-05-16 14:16:33.218268 fal-0.9.1/src/fal/typing.py
+-rw-r--r--   0        0        0     1711 2023-05-16 14:16:33.218268 fal-0.9.1/src/fal/utils.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:16:33.218268 fal-0.9.1/src/faldbt/__init__.py
+-rw-r--r--   0        0        0    24563 2023-05-16 14:16:33.218268 fal-0.9.1/src/faldbt/lib.py
+-rw-r--r--   0        0        0     3273 2023-05-16 14:16:33.218268 fal-0.9.1/src/faldbt/logger.py
+-rw-r--r--   0        0        0     1850 2023-05-16 14:16:33.218268 fal-0.9.1/src/faldbt/magics.py
+-rw-r--r--   0        0        0     9057 2023-05-16 14:16:33.218268 fal-0.9.1/src/faldbt/parse.py
+-rw-r--r--   0        0        0    27131 2023-05-16 14:16:33.218268 fal-0.9.1/src/faldbt/project.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:16:33.218268 fal-0.9.1/src/faldbt/utils/__init__.py
+-rw-r--r--   0        0        0     1970 2023-05-16 14:16:33.218268 fal-0.9.1/src/faldbt/utils/yaml_helper.py
+-rw-r--r--   0        0        0      317 2023-05-16 14:16:33.218268 fal-0.9.1/src/faldbt/version.py
+-rw-r--r--   0        0        0       33 2023-05-16 14:16:33.218268 fal-0.9.1/tests/_fal_testing/__init__.py
+-rw-r--r--   0        0        0     1786 2023-05-16 14:16:33.218268 fal-0.9.1/tests/_fal_testing/utils.py
+-rw-r--r--   0        0        0    13992 1970-01-01 00:00:00.000000 fal-0.9.1/PKG-INFO
```

### Comparing `fal-0.9.0/README.md` & `fal-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `fal-0.9.0/pyproject.toml` & `fal-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fal"
-version = "0.9.0"
+version = "0.9.1"
 description = "fal allows you to run python scripts directly from your dbt project."
 homepage = "https://github.com/fal-ai/fal/blob/-/projects/fal"
 documentation = "https://docs.fal.ai"
 repository = "https://github.com/fal-ai/fal"
 readme = "README.md"
 authors = [ "Features & Labels <hello@fal.ai>" ]
 packages = [
@@ -32,15 +32,15 @@
 "backports.functools_lru_cache" = "^1.6.4"
 
 # Environment management related dependencies
 platformdirs = "^2.5.2"
 virtualenv = "^20.16.2"
 dill = "^0.3.5.1, <0.3.6"
 importlib-metadata = ">=4.12.0"
-packaging = "<22"
+packaging = ">20.9"
 
 # Adapters
 
 ## snowflake
 snowflake-connector-python = { version = "~=3.0", extras = ["pandas"], optional = true }
 
 ## bigquery
```

### Comparing `fal-0.9.0/src/fal/cli/args.py` & `fal-0.9.1/src/fal/cli/args.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.0/src/fal/cli/cli.py` & `fal-0.9.1/src/fal/cli/cli.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.0/src/fal/cli/dbt_runner.py` & `fal-0.9.1/src/fal/cli/dbt_runner.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.0/src/fal/cli/fal_runner.py` & `fal-0.9.1/src/fal/cli/fal_runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,29 @@
 import argparse
 from pathlib import Path
 from typing import Any, Dict, List
 
-from dbt.flags import get_flags, set_from_args
 from fal.planner.executor import parallel_executor
 from fal.planner.schedule import Scheduler
 from fal.planner.tasks import FalLocalHookTask, Status, TaskGroup
-from dbt.cli.resolvers import default_profiles_dir
 
 from fal.fal_script import FalScript, TimingType
 from faldbt.project import FAL, DbtModel, FalDbt, FalGeneralException
 
 
 def create_fal_dbt(
     args: argparse.Namespace, generated_models: Dict[str, Path] = {}
 ) -> FalDbt:
-    if args.profiles_dir is None:
-        args.profiles_dir = default_profiles_dir()
-
-    set_from_args(args, None)
-    flags = get_flags()
-    profiles_dir = flags.PROFILES_DIR
-
     real_state = None
     if hasattr(args, "state") and args.state is not None:
         real_state = args.state
 
     return FalDbt(
         args.project_dir,
-        profiles_dir,
+        args.profiles_dir,
         args.select,
         args.exclude,
         args.selector,
         args.threads,
         real_state,
         args.target,
         args.vars,
@@ -68,18 +59,20 @@
         _run_scripts(args, scripts, faldbt)
 
         post_hook_scripts = _get_hooks_for_model(models, faldbt, TimingType.POST)
         _run_scripts(args, post_hook_scripts, faldbt)
         _handle_global_scripts(args, global_scripts, faldbt, selector_flags)
 
 
-def _handle_global_scripts(args: argparse.Namespace,
-                           global_scripts: List[FalScript],
-                           faldbt: FalDbt,
-                           selector_flags: Any) -> None:
+def _handle_global_scripts(
+    args: argparse.Namespace,
+    global_scripts: List[FalScript],
+    faldbt: FalDbt,
+    selector_flags: Any,
+) -> None:
     scripts_flag = _scripts_flag(args)
     if not scripts_flag and not selector_flags:
         # run globals when no --script is passed and no selector is passed
         _run_scripts(args, global_scripts, faldbt)
     if (scripts_flag or selector_flags) and args.globals:
         _run_scripts(args, global_scripts, faldbt)
 
@@ -114,15 +107,15 @@
 
 def _select_scripts(
     args: argparse.Namespace, models: List[DbtModel], faldbt: FalDbt
 ) -> List[FalScript]:
     scripts = []
     scripts_flag = _scripts_flag(args)
     is_before = bool(args.before)
-    timing_type=TimingType.PRE if is_before else TimingType.POST
+    timing_type = TimingType.PRE if is_before else TimingType.POST
 
     for model in models:
         model_scripts = model.get_scripts(before=is_before)
         for path in model_scripts:
             if not scripts_flag:
                 # run all scripts when no --script is passed
                 scripts.append(FalScript(faldbt, model, path, timing_type=timing_type))
@@ -132,26 +125,24 @@
 
     return scripts
 
 
 def _get_global_scripts(faldbt: FalDbt, args: argparse.Namespace):
     scripts_flag = _scripts_flag(args)
     is_before = bool(args.before)
-    timing_type=TimingType.PRE if is_before else TimingType.POST
+    timing_type = TimingType.PRE if is_before else TimingType.POST
     return [
         FalScript(faldbt, None, path, timing_type=timing_type)
         for path in faldbt._global_script_paths["before" if is_before else "after"]
         if not scripts_flag or path in args.scripts
     ]
 
 
 def _get_models_with_keyword(faldbt: FalDbt) -> List[DbtModel]:
-    return list(
-        filter(lambda model: FAL in model.meta, faldbt.list_models())
-    )
+    return list(filter(lambda model: FAL in model.meta, faldbt.list_models()))
 
 
 def _get_filtered_models(faldbt: FalDbt, all, selected, before) -> List[DbtModel]:
     selected_ids = _models_ids(faldbt._compile_task._flattened_nodes)
     filtered_models: List[DbtModel] = []
 
     if (
```

### Comparing `fal-0.9.0/src/fal/cli/flow_runner.py` & `fal-0.9.1/src/fal/cli/flow_runner.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.0/src/fal/cli/model_generator/model_generator.py` & `fal-0.9.1/src/fal/cli/model_generator/model_generator.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.0/src/fal/cli/model_generator/module_check.py` & `fal-0.9.1/src/fal/cli/model_generator/module_check.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.0/src/fal/cli/selectors.py` & `fal-0.9.1/src/fal/cli/selectors.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.0/src/fal/fal_script.py` & `fal-0.9.1/src/fal/fal_script.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.0/src/fal/node_graph.py` & `fal-0.9.1/src/fal/node_graph.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.0/src/fal/packages/bridge.py` & `fal-0.9.1/src/fal/packages/bridge.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.0/src/fal/packages/dependency_analysis.py` & `fal-0.9.1/src/fal/packages/dependency_analysis.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.0/src/fal/packages/environments/__init__.py` & `fal-0.9.1/src/fal/packages/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.0/src/fal/packages/environments/base.py` & `fal-0.9.1/src/fal/packages/environments/base.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.0/src/fal/packages/environments/conda.py` & `fal-0.9.1/src/fal/packages/environments/conda.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.0/src/fal/packages/environments/virtual_env.py` & `fal-0.9.1/src/fal/packages/environments/virtual_env.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.0/src/fal/packages/isolated_runner.py` & `fal-0.9.1/src/fal/packages/isolated_runner.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.0/src/fal/planner/executor.py` & `fal-0.9.1/src/fal/planner/executor.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.0/src/fal/planner/plan.py` & `fal-0.9.1/src/fal/planner/plan.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.0/src/fal/planner/schedule.py` & `fal-0.9.1/src/fal/planner/schedule.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.0/src/fal/planner/tasks.py` & `fal-0.9.1/src/fal/planner/tasks.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.0/src/fal/telemetry/telemetry.py` & `fal-0.9.1/src/fal/telemetry/telemetry.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.0/src/fal/typing.py` & `fal-0.9.1/src/fal/typing.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.0/src/fal/utils.py` & `fal-0.9.1/src/fal/utils.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.0/src/faldbt/lib.py` & `fal-0.9.1/src/faldbt/lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # NOTE: INSPIRED IN https://github.com/dbt-labs/dbt-core/blob/43edc887f97e359b02b6317a9f91898d3d66652b/core/dbt/lib.py
 from contextlib import contextmanager
 import six
 from enum import Enum
 from dataclasses import dataclass
 from uuid import uuid4
-from typing import Iterator, List, Optional, Tuple
+from typing import Dict, Iterator, List, Optional, Tuple
 from urllib.parse import quote_plus
 import threading
 
 import dbt.flags as flags
 import dbt.adapters.factory as adapters_factory
 
 from dbt.contracts.connection import AdapterResponse
@@ -36,32 +36,53 @@
 class WriteModeEnum(Enum):
     APPEND = "append"
     OVERWRITE = "overwrite"
 
 
 @dataclass
 class FlagsArgs:
+    project_dir: str
     profiles_dir: str
+    threads: Optional[int]
+    profile: Optional[str]
+    target: Optional[str]
+    vars: Optional[Dict[str, str]]
     use_colors: Optional[bool]
 
 
-def initialize_dbt_flags(profiles_dir: str):
+def initialize_dbt_flags(
+    profiles_dir: str,
+    project_dir: str,
+    profile_target: Optional[str],
+    vars: Optional[dict],
+    threads: Optional[int],
+):
     """
     Initializes the flags module from dbt, since it's accessed from around their code.
     """
-    args = FlagsArgs(profiles_dir, None)
-    user_config = parse.get_dbt_user_config(profiles_dir)
+    args = FlagsArgs(
+        use_colors=None,
+        project_dir=project_dir,
+        profiles_dir=profiles_dir,
+        # TODO: accept profile flag too
+        profile=None,
+        target=profile_target,
+        vars=vars,
+        threads=threads,
+    )
 
-    flags.set_from_args(args, user_config)
+    flags.set_from_args(args, None)
 
     # Set invocation id
     import dbt.events.functions as events_functions
 
     events_functions.set_invocation_id()
 
+    return flags.get_flags()
+
 
 def register_adapters(config: RuntimeConfig):
     # HACK: to avoid 'Node package named <profile> not found'
     adapters_factory.reset_adapters()
     adapters_factory.register_adapter(config)
 
 
@@ -80,35 +101,30 @@
             profile_target=profile_target,
         )
     adapter: SQLAdapter = adapters_factory.get_adapter(config)  # type: ignore
 
     return adapter
 
 
-global _lock
-# RLock supports recursive locking by the same thread
-_lock = threading.RLock()
-
+# HACK: to avoid https://github.com/uqfoundation/dill/issues/321
+# When the lock is unpickled in the other thread, it is initialized as locked
+if hasattr(threading, "_PyRLock"):
+    _lock: threading.RLock = threading._PyRLock()  # type: ignore
+else:
+    _lock = threading.RLock()
 
 @contextmanager
 def _cache_lock(info: str = ""):
+    global _lock
+
     operationId = uuid4()
     LOGGER.debug("Locking  {} {}", operationId, info)
 
-    _lock.acquire()
-    LOGGER.debug("Acquired {}", operationId)
-
-    try:
+    with _lock:
         yield
-    except:
-        LOGGER.debug("Error during lock operation {}", operationId)
-        raise
-    finally:
-        _lock.release()
-        LOGGER.debug("Released {}", operationId)
 
 
 def _connection_name(prefix: str, obj, _hash: bool = True):
     # HACK: we need to include uniqueness (UUID4) to avoid clashes
     return f"{prefix}:{hash(str(obj)) if _hash else obj}:{uuid4()}"
```

### Comparing `fal-0.9.0/src/faldbt/logger.py` & `fal-0.9.1/src/faldbt/logger.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.0/src/faldbt/magics.py` & `fal-0.9.1/src/faldbt/magics.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.0/src/faldbt/parse.py` & `fal-0.9.1/src/faldbt/parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from dataclasses import dataclass
 import glob
 from pathlib import Path
 from typing import Any, List, Dict, Optional, Union, TYPE_CHECKING
 
 from dbt.contracts.project import Project as ProjectContract
 from dbt.config import RuntimeConfig, Project
-from dbt.config.utils import parse_cli_vars
+from dbt.config.utils import parse_cli_vars as dbt_parse_cli_vars
 from dbt.contracts.graph.manifest import Manifest
 from dbt.contracts.results import RunResultsArtifact, FreshnessExecutionResultArtifact
 from dbt.contracts.project import UserConfig
 from dbt.config.profile import read_user_config
 
 from dbt.exceptions import IncompatibleSchemaError, DbtRuntimeError
 
@@ -59,29 +59,28 @@
 def get_dbt_config(
     *,
     project_dir: str,
     profiles_dir: str,
     profile_target: Optional[str] = None,
     threads: Optional[int] = None,
     profile: Optional[str] = None,
-    vars: str = "{}",
+    args_vars: str = "{}",
 ) -> RuntimeConfig:
     # Construct a phony config
     import os
 
-    vars_dict = parse_cli_vars(vars)
-
+    vars = get_vars_dict(project_dir, args_vars)
     args = RuntimeArgs(
         project_dir=project_dir,
         profiles_dir=profiles_dir,
         threads=threads,
         single_threaded=False,
         profile=profile,
         target=profile_target,
-        vars=vars_dict,
+        vars=vars,
     )
 
     if project_dir and not "PYTEST_CURRENT_TEST" in os.environ:
         # HACK: initializing dbt-fal requires cwd to be project_dir
         # TODO: this doesn't work in pytest + Github Actions
         owd = os.getcwd()
         os.chdir(project_dir)
@@ -105,14 +104,23 @@
     # NOTE: This happens usually inside unit tests
     vars = (project_contract is not None and project_contract.vars) or {}
     cli_vars = parse_cli_vars(args_vars)
 
     # cli_vars have higher priority
     return {**vars, **cli_vars}
 
+def parse_cli_vars(args_vars: str) -> Dict[str, Any]:
+    if not args_vars:
+        return {}
+
+    try:
+        return dbt_parse_cli_vars(args_vars)
+    except DbtRuntimeError as exc:
+        raise FalParseError(exc)
+
 
 @cache_static
 def get_fal_models_dirs(project_dir: str, args_vars: str) -> List[str]:
     vars = get_vars_dict(project_dir, args_vars)
     model_paths = vars.get(FAL_MODELS_PATHS) or []
     if not model_paths:
         # None or empty list
```

### Comparing `fal-0.9.0/src/faldbt/project.py` & `fal-0.9.1/src/faldbt/project.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     TYPE_CHECKING,
 )
 from pathlib import Path
 from deprecation import deprecated
 
 import faldbt.version as version
 
+from dbt.cli.resolvers import default_profiles_dir
 from dbt.cli.main import dbtRunner, dbtRunnerResult
 
 from dbt.contracts.graph.nodes import (
     SourceDefinition,
     TestMetadata,
     GenericTestNode,
     SingularTestNode,
@@ -436,47 +437,66 @@
 @has_side_effects
 class FalDbt:
     """Holds the entire dbt project information."""
 
     # TODO: figure out a meaningful __repr__ for this class
     def __init__(
         self,
-        project_dir: str,
-        profiles_dir: str,
+        project_dir: Optional[str] = None,
+        profiles_dir: Optional[str] = None,
         select: List[str] = [],
         exclude: Tuple[str] = tuple(),
         selector: Optional[str] = None,
         threads: Optional[int] = None,
         state: Optional[str] = None,
         profile_target: Optional[str] = None,
         args_vars: str = "{}",
         generated_models: Dict[str, Path] = {},
     ):
         if not version.is_version_plus("1.0.0"):
             raise NotImplementedError(
                 f"dbt version {version.DBT_VCURRENT} is no longer supported, please upgrade to dbt 1.0.0 or above"
             )
 
-        self.project_dir = os.path.realpath(os.path.expanduser(project_dir))
-        self.profiles_dir = os.path.realpath(os.path.expanduser(profiles_dir))
+        if project_dir is None:
+            project_dir = os.getcwd()
+
+        if profiles_dir is None:
+            profiles_dir = str(default_profiles_dir())
+
+        project_dir = os.path.realpath(os.path.expanduser(project_dir))
+        profiles_dir = os.path.realpath(os.path.expanduser(profiles_dir))
+
+        vars = parse.parse_cli_vars(args_vars)
+
+        flags = lib.initialize_dbt_flags(
+            profiles_dir=profiles_dir,
+            project_dir=project_dir,
+            threads=threads,
+            profile_target=profile_target,
+            vars=vars,
+        )
+
+        self.project_dir = flags.PROJECT_DIR
+        self.profiles_dir = flags.PROFILES_DIR
+
         self._state = None
         if state is not None:
             self._state = Path(os.path.realpath(os.path.expanduser(state)))
 
         self.scripts_dir = parse.get_scripts_dir(self.project_dir, args_vars)
 
-        lib.initialize_dbt_flags(profiles_dir=self.profiles_dir)
 
         # Can be overwritten if profile_target is not None
         self._config = parse.get_dbt_config(
             project_dir=self.project_dir,
             profiles_dir=self.profiles_dir,
             profile_target=profile_target,
             threads=threads,
-            vars=args_vars
+            args_vars=args_vars,
         )
 
         self._run_results = DbtRunResult(
             parse.get_dbt_results(self.project_dir, self._config)
         )
 
         if self._run_results.native_run_result:
@@ -485,14 +505,15 @@
 
         if profile_target is not None:
             self._config = parse.get_dbt_config(
                 project_dir=self.project_dir,
                 profiles_dir=self.profiles_dir,
                 threads=threads,
                 profile_target=profile_target,
+                args_vars=args_vars,
             )
 
         lib.register_adapters(self._config)
 
         parse_result = self._dbt_invoke("parse")
         native_manifest: Manifest = parse_result.result # type: ignore
```

### Comparing `fal-0.9.0/src/faldbt/utils/yaml_helper.py` & `fal-0.9.1/src/faldbt/utils/yaml_helper.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.0/tests/_fal_testing/utils.py` & `fal-0.9.1/tests/_fal_testing/utils.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.0/PKG-INFO` & `fal-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fal
-Version: 0.9.0
+Version: 0.9.1
 Summary: fal allows you to run python scripts directly from your dbt project.
 Home-page: https://github.com/fal-ai/fal/blob/-/projects/fal
 Keywords: dbt,pandas
 Author: Features & Labels
 Author-email: hello@fal.ai
 Requires-Python: >=3.7.2,<3.11
 Classifier: Development Status :: 4 - Beta
@@ -32,15 +32,15 @@
 Requires-Dist: dill (>=0.3.5.1,<0.3.6)
 Requires-Dist: duckdb-engine (>=0.1.8,<0.2.0) ; extra == "duckdb"
 Requires-Dist: google-cloud-bigquery[pandas] (>=3.5.0,<3.6.0) ; extra == "bigquery"
 Requires-Dist: importlib-metadata (>=4.12.0)
 Requires-Dist: koldstart (>=0.6.16,<0.7.0) ; extra == "cloud"
 Requires-Dist: matplotlib (>=3.5.2,<4.0.0) ; extra == "dev"
 Requires-Dist: mock (>=4.0.3,<5.0.0) ; extra == "test"
-Requires-Dist: packaging (<22)
+Requires-Dist: packaging (>20.9)
 Requires-Dist: pandas (>=1.3.4,<2.0.0)
 Requires-Dist: platformdirs (>=2.5.2,<3.0.0)
 Requires-Dist: posthog (>=1.4.5,<2.0.0)
 Requires-Dist: pytest (>=5.2,<6.0) ; extra == "test"
 Requires-Dist: pytest-mock (>=3.7.0,<4.0.0) ; extra == "test"
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Requires-Dist: snowflake-connector-python[pandas] (>=3.0,<4.0) ; extra == "snowflake"
```

