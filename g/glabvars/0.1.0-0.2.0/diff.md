# Comparing `tmp/glabvars-0.1.0.tar.gz` & `tmp/glabvars-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glabvars-0.1.0.tar", last modified: Fri May 12 13:04:23 2023, max compression
+gzip compressed data, was "glabvars-0.2.0.tar", last modified: Tue May 16 13:22:37 2023, max compression
```

## Comparing `glabvars-0.1.0.tar` & `glabvars-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxr-x   0 wouter    (1000) wouter    (1000)        0 2023-05-12 13:04:23.617553 glabvars-0.1.0/
--rw-rw-r--   0 wouter    (1000) wouter    (1000)     1519 2023-05-12 12:25:44.000000 glabvars-0.1.0/LICENSE
--rw-rw-r--   0 wouter    (1000) wouter    (1000)     4407 2023-05-12 13:04:23.617553 glabvars-0.1.0/PKG-INFO
--rw-rw-r--   0 wouter    (1000) wouter    (1000)     1611 2023-05-12 12:55:09.000000 glabvars-0.1.0/README.md
--rw-rw-r--   0 wouter    (1000) wouter    (1000)     1397 2023-05-12 12:43:39.000000 glabvars-0.1.0/pyproject.toml
--rw-rw-r--   0 wouter    (1000) wouter    (1000)       38 2023-05-12 13:04:23.617553 glabvars-0.1.0/setup.cfg
-drwxrwxr-x   0 wouter    (1000) wouter    (1000)        0 2023-05-12 13:04:23.617553 glabvars-0.1.0/src/
--rw-rw-r--   0 wouter    (1000) wouter    (1000)        0 2023-05-12 12:27:14.000000 glabvars-0.1.0/src/__init__.py
--rw-rw-r--   0 wouter    (1000) wouter    (1000)     6216 2023-05-12 12:58:32.000000 glabvars-0.1.0/src/app.py
-drwxrwxr-x   0 wouter    (1000) wouter    (1000)        0 2023-05-12 13:04:23.617553 glabvars-0.1.0/src/glabvars.egg-info/
--rw-rw-r--   0 wouter    (1000) wouter    (1000)     4407 2023-05-12 13:04:23.000000 glabvars-0.1.0/src/glabvars.egg-info/PKG-INFO
--rw-rw-r--   0 wouter    (1000) wouter    (1000)      299 2023-05-12 13:04:23.000000 glabvars-0.1.0/src/glabvars.egg-info/SOURCES.txt
--rw-rw-r--   0 wouter    (1000) wouter    (1000)        1 2023-05-12 13:04:23.000000 glabvars-0.1.0/src/glabvars.egg-info/dependency_links.txt
--rw-rw-r--   0 wouter    (1000) wouter    (1000)       37 2023-05-12 13:04:23.000000 glabvars-0.1.0/src/glabvars.egg-info/entry_points.txt
--rw-rw-r--   0 wouter    (1000) wouter    (1000)       17 2023-05-12 13:04:23.000000 glabvars-0.1.0/src/glabvars.egg-info/requires.txt
--rw-rw-r--   0 wouter    (1000) wouter    (1000)       19 2023-05-12 13:04:23.000000 glabvars-0.1.0/src/glabvars.egg-info/top_level.txt
-drwxrwxr-x   0 wouter    (1000) wouter    (1000)        0 2023-05-12 13:04:23.617553 glabvars-0.1.0/src/tests/
--rw-rw-r--   0 wouter    (1000) wouter    (1000)      443 2023-05-12 12:40:20.000000 glabvars-0.1.0/src/tests/test_app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 13:22:37.650036 glabvars-0.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1519 2023-05-16 13:22:20.000000 glabvars-0.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4890 2023-05-16 13:22:37.650036 glabvars-0.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2094 2023-05-16 13:22:20.000000 glabvars-0.2.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1402 2023-05-16 13:22:20.000000 glabvars-0.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-16 13:22:37.650036 glabvars-0.2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 13:22:37.648036 glabvars-0.2.0/src/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 13:22:20.000000 glabvars-0.2.0/src/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7488 2023-05-16 13:22:20.000000 glabvars-0.2.0/src/app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 13:22:37.649036 glabvars-0.2.0/src/glabvars.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4890 2023-05-16 13:22:37.000000 glabvars-0.2.0/src/glabvars.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      331 2023-05-16 13:22:37.000000 glabvars-0.2.0/src/glabvars.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 13:22:37.000000 glabvars-0.2.0/src/glabvars.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-05-16 13:22:37.000000 glabvars-0.2.0/src/glabvars.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-05-16 13:22:37.000000 glabvars-0.2.0/src/glabvars.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-05-16 13:22:37.000000 glabvars-0.2.0/src/glabvars.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-05-16 13:22:20.000000 glabvars-0.2.0/src/targets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 13:22:37.649036 glabvars-0.2.0/src/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      443 2023-05-16 13:22:20.000000 glabvars-0.2.0/src/tests/test_app.py
+-rw-rw-rw-   0 root         (0) root         (0)      589 2023-05-16 13:22:20.000000 glabvars-0.2.0/src/variables.py
```

### Comparing `glabvars-0.1.0/LICENSE` & `glabvars-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `glabvars-0.1.0/PKG-INFO` & `glabvars-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glabvars
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Python wrapper for retrieving Gitlab CI/CD variables
 Author-email: Wouter Donders <wouter@42analytics.eu>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, 42Analytics
         All rights reserved.
         
@@ -67,14 +67,24 @@
 Run the `glabvars` CLI app inside a git repository with a Gitlab remote.
 The application can return a YAML configuration string for `gitlab-ci-local` to `stdout`.
 You can pipe this output to `.gitlab-ci-local-variables.yml` so that `gitlab-ci-local` can use the variables.
 ```shell
 glabvars --target gcl > .gitlab-ci-local-variables.yml
 ```
 
+# Output targets
+
+## Gitlab-CI-Local: `gcl`
+When passing `--target gcl`, `glabvars` will output to `stdout` a YAML configuration file that can be used by `gitlab-ci-local`.
+
+## Environment: `env`
+When passing `--target env`, `glabvars` will output `.env` files and file-type variable files.
+These files are postfixed with `.<environment_scope>` if the `environment_scope` of a CI/CD variable is not `'*'`. These files are written in the `--env-path` directory (default: `.gitlab`)
+
+
 # Installation
 Install with `pip` to install globally:
 
 ```shell
 pip install glabvars
 ```
```

### Comparing `glabvars-0.1.0/README.md` & `glabvars-0.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -14,14 +14,24 @@
 Run the `glabvars` CLI app inside a git repository with a Gitlab remote.
 The application can return a YAML configuration string for `gitlab-ci-local` to `stdout`.
 You can pipe this output to `.gitlab-ci-local-variables.yml` so that `gitlab-ci-local` can use the variables.
 ```shell
 glabvars --target gcl > .gitlab-ci-local-variables.yml
 ```
 
+# Output targets
+
+## Gitlab-CI-Local: `gcl`
+When passing `--target gcl`, `glabvars` will output to `stdout` a YAML configuration file that can be used by `gitlab-ci-local`.
+
+## Environment: `env`
+When passing `--target env`, `glabvars` will output `.env` files and file-type variable files.
+These files are postfixed with `.<environment_scope>` if the `environment_scope` of a CI/CD variable is not `'*'`. These files are written in the `--env-path` directory (default: `.gitlab`)
+
+
 # Installation
 Install with `pip` to install globally:
 
 ```shell
 pip install glabvars
 ```
```

### Comparing `glabvars-0.1.0/pyproject.toml` & `glabvars-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 [tool.pdm.dev-dependencies]
 dev = [
     "pre-commit>=3.3.1",
     "pytest>=7.3.1",
 ]
 
+[tool.tox]
+legacy_tox_ini = "[tox]\nenvlist = py39, py310, py311, py312\nisolated_build = True\n[testenv]\ncommands = pytest\n"
+
 [project]
 name = "glabvars"
-version = "0.1.0"
+version = "0.2.0"
 description = "A Python wrapper for retrieving Gitlab CI/CD variables"
 authors = [
     { name = "Wouter Donders", email = "wouter@42analytics.eu" },
 ]
 dependencies = [
     "pydantic>=1.10.7",
 ]
 requires-python = ">=3.9"
 readme = "README.md"
-license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: BSD License",
 ]
 
+[project.license]
+file = "LICENSE"
+
 [project.urls]
 Homepage = "https://42analytics.eu"
 Documentations = "https://gitlab.com/42analytics1/public/glabvars"
 Source = "https://gitlab.com/42analytics1/public/glabvars"
 Download = "https://gitlab.com/42analytics1/public/glabvars/-/packages"
 Tracker = "https://gitlab.com/42analytics1/public/glabvars/-/issues"
 
@@ -41,16 +46,7 @@
 
 [build-system]
 requires = [
     "setuptools>=61",
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
-
-[tool.tox]
-legacy_tox_ini = """
-[tox]
-envlist = py39, py310, py311, py312
-isolated_build = True
-[testenv]
-commands = pytest
-"""
```

### Comparing `glabvars-0.1.0/src/app.py` & `glabvars-0.2.0/src/app.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,15 @@
 import argparse
 import logging
 import subprocess
-from pydantic import BaseModel, parse_raw_as
-
-
-class GLVariable(BaseModel):
-    """Gitlab CI variable"""
-
-    key: str
-    value: str
-    protected: bool
-    variable_type: str = "env_var"
-    masked: bool
-    raw: bool
-    environment_scope: str
-
-    @property
-    def gcl_type(self):
-        """Type string to be used in YAML config"""
-        return "variable" if self.variable_type == "env_var" else "file"
-
-
-class GCLVariable(BaseModel):
-    """Gitlab-CI-Local variable"""
-
-    type: str
-    values: dict[str, str]
-
-
-class GLGroup(BaseModel):
-    """Gitlab group"""
-
-    id: int
-    full_path: str
+from typing import Iterable
+from pydantic import parse_raw_as
+from variables import GCLVariable, GLGroup, GLVariable
+from targets import Target
+from pathlib import Path
 
 
 def convert_to_gcl(ci_variables: list[GLVariable]):
     """Collect CI variables into a new structure."""
     gcl_variables: dict[str, GCLVariable] = {}
     for ci_variable in ci_variables:
         environment_values = {ci_variable.environment_scope: ci_variable.value}
@@ -116,15 +89,17 @@
 
     return parse_raw_as(list[GLVariable], process.stdout)
 
 
 def export_project_variables() -> list[GLVariable]:
     """Export project variables"""
     process = subprocess.run(
-        ["glab", "variable", "export"], stderr=subprocess.PIPE, stdout=subprocess.PIPE
+        ["glab", "variable", "export", "-R", "42analytics1/experiments/gitlab-to-gcl"],
+        stderr=subprocess.PIPE,
+        stdout=subprocess.PIPE,
     )
     return export_variables(process)
 
 
 def export_group_variables(group_path: str) -> list[GLVariable]:
     """Export group variables"""
     process = subprocess.run(
@@ -145,19 +120,44 @@
 
     return sorted(
         parse_raw_as(list[GLGroup], process.stdout),
         key=lambda x: len(x.full_path.split("/")),
     )
 
 
-def main(target: str):
-    if target != "gcl":
-        logging.error(f"Target {target} is not supported.")
-        exit(999)
+def convert_to_env(env_path: Path, gl_variables: Iterable[GLVariable]) -> None:
+    """Return GL variables"""
+
+    filenames = set()
 
+    for gl_variable in gl_variables:
+        if gl_variable.gcl_type == "variable":
+            # The .env file to write to is '.env[.<environment_scope>]', where the scope
+            # is added if the scope is anything other than '*'
+            filename = ".env"
+            if gl_variable.environment_scope != "*":
+                filename = f"{filename}.{gl_variable.environment_scope}"
+
+            file_access = "w" if filename not in filenames else "a"
+            with open(env_path / filename, file_access) as f:
+                f.write(f"{gl_variable.key}='{gl_variable.value}'\n")
+
+            # Add the filename
+            filenames.add(filename)
+
+        elif gl_variable.gcl_type == "file":
+            # Write the contents of file-type variables to a file
+            filename = f"{gl_variable.key.lower()}"
+            if gl_variable.environment_scope != "*":
+                filename = f"{filename}.{gl_variable.environment_scope}"
+            with open(env_path / filename, "w") as f:
+                f.write(gl_variable.value)
+
+
+def main(target: Target, env_path: Path):
     if not is_glab_installed():
         # ERROR CODE 1: Gitlab CLI (`glab`) is not installed or found on PATH
         exit(1)
 
     if not is_glab_authenticated():
         # ERROR CODE 2: Gitlab CLI (`glab`) is not authenticated
         exit(2)
@@ -169,26 +169,46 @@
         group_variables = export_group_variables(group_path=project_group.full_path)
         gl_variables.extend(group_variables)
 
     # Obtain variables
     project_variables = export_project_variables()
     gl_variables.extend(project_variables)
 
-    gcl_variables = convert_to_gcl(gl_variables)
-    print_to_stdout(gcl_variables)
+    match target:
+        case Target.GCL:
+            gcl_variables = convert_to_gcl(gl_variables)
+            print_to_stdout(gcl_variables)
+        case Target.ENV:
+            if not env_path.exists():
+                env_path.mkdir(parents=True)
+
+            convert_to_env(env_path=env_path, gl_variables=gl_variables)
+        case _:
+            raise NotImplementedError()
 
 
 def cli():
     """Main function"""
     parser = argparse.ArgumentParser(
         description="Retrieve Gitlab CI variables and output yaml configuration contents for gitlab-ci-local"  # noqa: E501
     )
     parser.add_argument(
-        "-t", "--target", default="gcl", help="CI/CD variable export target"
+        "-t",
+        "--target",
+        type=Target,
+        default="env",
+        help="CI/CD variable export target",
+    )
+    parser.add_argument(
+        "-e",
+        "--env-path",
+        type=Path,
+        default=".gitlab",
+        help="Output path when --target ENV is passed",
     )
     arguments = parser.parse_args()
 
-    main(target=arguments.target)
+    main(target=arguments.target, env_path=arguments.env_path)
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `glabvars-0.1.0/src/glabvars.egg-info/PKG-INFO` & `glabvars-0.2.0/src/glabvars.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glabvars
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Python wrapper for retrieving Gitlab CI/CD variables
 Author-email: Wouter Donders <wouter@42analytics.eu>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, 42Analytics
         All rights reserved.
         
@@ -67,14 +67,24 @@
 Run the `glabvars` CLI app inside a git repository with a Gitlab remote.
 The application can return a YAML configuration string for `gitlab-ci-local` to `stdout`.
 You can pipe this output to `.gitlab-ci-local-variables.yml` so that `gitlab-ci-local` can use the variables.
 ```shell
 glabvars --target gcl > .gitlab-ci-local-variables.yml
 ```
 
+# Output targets
+
+## Gitlab-CI-Local: `gcl`
+When passing `--target gcl`, `glabvars` will output to `stdout` a YAML configuration file that can be used by `gitlab-ci-local`.
+
+## Environment: `env`
+When passing `--target env`, `glabvars` will output `.env` files and file-type variable files.
+These files are postfixed with `.<environment_scope>` if the `environment_scope` of a CI/CD variable is not `'*'`. These files are written in the `--env-path` directory (default: `.gitlab`)
+
+
 # Installation
 Install with `pip` to install globally:
 
 ```shell
 pip install glabvars
 ```
```

