# Comparing `tmp/python-barn-0.5.1.tar.gz` & `tmp/python-barn-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-barn-0.5.1.tar", last modified: Fri May  5 22:14:53 2023, max compression
+gzip compressed data, was "python-barn-0.6.0.tar", last modified: Tue May 16 15:06:29 2023, max compression
```

## Comparing `python-barn-0.5.1.tar` & `python-barn-0.6.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:14:53.152416 python-barn-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-05 22:14:53.152416 python-barn-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 22:14:35.000000 python-barn-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:14:53.152416 python-barn-0.5.1/python_barn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-05 22:14:53.000000 python-barn-0.5.1/python_barn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-05 22:14:53.000000 python-barn-0.5.1/python_barn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 22:14:53.000000 python-barn-0.5.1/python_barn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 22:14:53.000000 python-barn-0.5.1/python_barn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 22:14:53.000000 python-barn-0.5.1/python_barn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-05 22:14:53.000000 python-barn-0.5.1/python_barn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 22:14:53.152416 python-barn-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-05 22:14:35.000000 python-barn-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:14:53.152416 python-barn-0.5.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-05 22:14:35.000000 python-barn-0.5.1/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:14:53.152416 python-barn-0.5.1/src/actions/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-05 22:14:35.000000 python-barn-0.5.1/src/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-05 22:14:35.000000 python-barn-0.5.1/src/actions/add.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-05 22:14:35.000000 python-barn-0.5.1/src/actions/execute_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-05 22:14:35.000000 python-barn-0.5.1/src/actions/init.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-05 22:14:35.000000 python-barn-0.5.1/src/actions/install.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-05 22:14:35.000000 python-barn-0.5.1/src/actions/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-05 22:14:35.000000 python-barn-0.5.1/src/actions/show.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-05 22:14:35.000000 python-barn-0.5.1/src/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7077 2023-05-05 22:14:35.000000 python-barn-0.5.1/src/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:06:29.543465 python-barn-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-16 15:06:29.543465 python-barn-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-05-16 15:06:17.000000 python-barn-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:06:29.539465 python-barn-0.6.0/python_barn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-16 15:06:29.000000 python-barn-0.6.0/python_barn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-16 15:06:29.000000 python-barn-0.6.0/python_barn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 15:06:29.000000 python-barn-0.6.0/python_barn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 15:06:29.000000 python-barn-0.6.0/python_barn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 15:06:29.000000 python-barn-0.6.0/python_barn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-16 15:06:29.000000 python-barn-0.6.0/python_barn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 15:06:29.543465 python-barn-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-16 15:06:17.000000 python-barn-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:06:29.539465 python-barn-0.6.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-16 15:06:17.000000 python-barn-0.6.0/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:06:29.539465 python-barn-0.6.0/src/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-16 15:06:17.000000 python-barn-0.6.0/src/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-16 15:06:17.000000 python-barn-0.6.0/src/actions/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-16 15:06:17.000000 python-barn-0.6.0/src/actions/execute_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-16 15:06:17.000000 python-barn-0.6.0/src/actions/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-16 15:06:17.000000 python-barn-0.6.0/src/actions/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-16 15:06:17.000000 python-barn-0.6.0/src/actions/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-16 15:06:17.000000 python-barn-0.6.0/src/actions/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-05-16 15:06:17.000000 python-barn-0.6.0/src/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-05-16 15:06:17.000000 python-barn-0.6.0/src/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-16 15:06:17.000000 python-barn-0.6.0/src/logging_utils.py
```

### Comparing `python-barn-0.5.1/setup.py` & `python-barn-0.6.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="python-barn",
-    version="0.5.1",
+    version="0.6.0",
     packages=find_packages(),
     entry_points={
         "console_scripts": [
             "barn=src.cli:main",
         ],
     },
     package_data={
@@ -15,15 +15,15 @@
     install_requires=[
         # Add your package dependencies here, e.g. 'numpy>=1.14.0'
         "PyYAML==6.0"
     ],
     author="Jacopo Madaluni",
     author_email="jacopo.madaluni@gmail.com",
     description="A wrapper for pip, to give better utils to python projects dependency management",
-    long_description=open("README.md").read(),
+    long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/JacopoMadaluni/barn",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.9",
```

### Comparing `python-barn-0.5.1/src/actions/add.py` & `python-barn-0.6.0/src/actions/add.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+from logging import Logger
 from src.core import barn_action, Context
 
 def add_from_url(url: str, context: Context):
     stdout, exit_code = context.run_command_in_context(f"pip install {url}")
     if exit_code == 0:
         context.run_command_in_context("pip freeze > barn.lock")
         context.add_dependency_to_project_yaml(url, None, is_url=True)
     else:
         print(f"Error installing {url}")
 
 @barn_action
-def add(requirement: str, context: Context=None):
+def add(requirement: str, context: Context=None, logger: Logger=None):
 
     if requirement.startswith("git+https://") or requirement.startswith("git+ssh://"):
         add_from_url(requirement, context)
         return
     
     package_name, package_version = context.split_package_version(requirement)
```

### Comparing `python-barn-0.5.1/src/actions/init.py` & `python-barn-0.6.0/src/actions/init.py`

 * *Files identical despite different names*

### Comparing `python-barn-0.5.1/src/cli.py` & `python-barn-0.6.0/src/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,16 +28,19 @@
     subparsers = parser.add_subparsers(dest='command')
 
     # Add 'install' command
     subparsers.add_parser('install')
 
     # Add 'add' command
     add_parser = subparsers.add_parser('add')
-    add_parser.add_argument("requirement", help="The name of package to add, versioning is also supported")
-    
+    add_parser.add_argument(
+        "requirement",
+        help="The name of package to add, versioning is also supported"
+    )
+
     remove_parser = subparsers.add_parser('remove')
     remove_parser.add_argument("package_name", help="The name of package to add, versioning is also supported")
 
     show_parser = subparsers.add_parser('show')
     show_parser.add_argument("-v", "--verbose", help="extra text", action='store_true')
     show_parser.add_argument("package_name", help="The name of package to show")
     show_parser.add_argument("-f", "--files", help="Show the full list of files", action='store_true')
@@ -45,16 +48,16 @@
     # subparsers.add_parser('test')
 
     # Parse the arguments
  
     args, unknown_args = parser.parse_known_args()
 
     exit_code = 0
-    if len(unknown_args) > 0:
-        _, exit_code = execute_script(unknown_args[0])
+    if len(unknown_args) and args.command is None > 0:
+        _, exit_code = execute_script(unknown_args[0], unknown_args[1:])
     # If no command is given, print help and exit
     elif args.command is None:
         _, exit_code = install()
     elif args.command == 'show':
         _, exit_code = show(args.package_name, verbose=args.verbose, files=args.files)
     elif args.command == 'install':
         _, exit_code = install()
@@ -70,10 +73,7 @@
             # Do whatever here
             context.add_dependency_to_project_yaml("test", "1.0.0")
         test_action()
     else:
         print("Unknown command: " + args.command)
 
     sys.exit(exit_code)
-
-# if __name__ == "__main__":
-#     main()
```

### Comparing `python-barn-0.5.1/src/core.py` & `python-barn-0.6.0/src/core.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,26 @@
 import os
 from pathlib import Path
 import subprocess
 import yaml
 import pty
 import re
+import logging
 from typing import List, Dict
+from .logging_utils import CustomFormatter
 
+logger = logging.getLogger()
+ch = logging.StreamHandler()
+ch.setLevel(logging.DEBUG)
+ch.setFormatter(CustomFormatter())
+logger.addHandler(ch)
+if int(os.environ.get('BARN_DEBUG', 0)) == 1:
+    logger.setLevel(logging.DEBUG)
+else:
+    logger.setLevel(logging.WARNING)
 
 class IndentedYamlDumper(yaml.Dumper):
     def increase_indent(self, flow=False, indentless=False):
         return super(IndentedYamlDumper, self).increase_indent(flow, False)
     
 
 class Context:
@@ -20,25 +31,30 @@
         self.is_initialized = is_initialized
         self.activate_path = self.root_dir / "python_modules" / "bin" / "activate"
 
         self.lock_file_exists = os.path.exists(self.root_dir / "barn.lock")
 
         self.project_yaml_path = self.root_dir / "project.yaml"
 
+        self.bash_functions_declarations = {
+
+        }
+
 
 
     def __repr__(self) -> str:
         repr = f"""
         Root: {self.root_dir}
         Initialized: {self.is_initialized}
         Activate path: {self.activate_path}"
         """
         return repr
 
     def __run_command(self, command, mute=False):
+        logger.debug(f"Executing: {command}")
         master_fd, slave_fd = pty.openpty()
         process = subprocess.Popen(
             command,
             executable="/bin/bash",
             shell=True,
             stdin=slave_fd,
             stdout=slave_fd,
@@ -76,14 +92,30 @@
 
         stdout, exit_code = self.__run_command(
             f'source {self.activate_path} && {command}'
         )
 
         return stdout, exit_code
     
+    def setup_bash_function_capabilities(self, name: str, command: str):
+        trailing_sc = ";" if command.strip()[-1] != ";" else ""
+        function_declaration = "function "+ name + " { " + command + trailing_sc + ' }'
+        logger.debug(f"Setting up function: {function_declaration}")
+        _, exit_code = self.__run_command(
+            function_declaration
+        )
+        if exit_code == 0:
+            self.bash_functions_declarations[name] = function_declaration
+        return exit_code
+    
+    def run_function_in_context(self, name: str, args: str):
+        declaration = self.bash_functions_declarations[name]
+        script_to_execute = f"{declaration} && {name} {args}"
+        return self.run_command_in_context(script_to_execute)
+
     def run_command_on_global(self, command: str):
         stdout, exit_code = self.__run_command(
             f'{command}'
         )
         return stdout, exit_code
     
     def get_project_dependencies(self) -> List[Dict[str, str]]:
@@ -201,19 +233,20 @@
             return current_dir / "project.yaml"
         current_dir = current_dir.parent
     
     raise Exception("Barn could not find a project context to use. Are you in a project directory?")
 
 
 
+
 def barn_action(action):
     project_yaml = find_project_yaml()
     root_dir = project_yaml.parent
     is_initialized = is_env_initialized(root_dir)
     context = Context(
         root_dir=root_dir,
         is_initialized=is_initialized
     )
     def wrapper(*args, **kwargs):
-        return action(*args, **kwargs, context=context)
+        return action(*args, **kwargs, context=context, logger=logger)
 
     return wrapper
```

