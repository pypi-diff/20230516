# Comparing `tmp/python-barn-0.7.0.tar.gz` & `tmp/python-barn-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-barn-0.7.0.tar", last modified: Tue May 16 18:02:31 2023, max compression
+gzip compressed data, was "python-barn-0.8.0.tar", last modified: Tue May 16 21:52:14 2023, max compression
```

## Comparing `python-barn-0.7.0.tar` & `python-barn-0.8.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:02:31.115624 python-barn-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-16 18:02:31.115624 python-barn-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-05-16 18:02:19.000000 python-barn-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:02:31.111624 python-barn-0.7.0/python_barn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-16 18:02:31.000000 python-barn-0.7.0/python_barn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-16 18:02:31.000000 python-barn-0.7.0/python_barn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 18:02:31.000000 python-barn-0.7.0/python_barn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 18:02:31.000000 python-barn-0.7.0/python_barn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 18:02:31.000000 python-barn-0.7.0/python_barn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-16 18:02:31.000000 python-barn-0.7.0/python_barn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 18:02:31.115624 python-barn-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-16 18:02:19.000000 python-barn-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:02:31.111624 python-barn-0.7.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-16 18:02:19.000000 python-barn-0.7.0/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:02:31.115624 python-barn-0.7.0/src/actions/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-16 18:02:19.000000 python-barn-0.7.0/src/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-16 18:02:19.000000 python-barn-0.7.0/src/actions/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-16 18:02:19.000000 python-barn-0.7.0/src/actions/execute_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-16 18:02:19.000000 python-barn-0.7.0/src/actions/init.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-16 18:02:19.000000 python-barn-0.7.0/src/actions/install.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-16 18:02:19.000000 python-barn-0.7.0/src/actions/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-16 18:02:19.000000 python-barn-0.7.0/src/actions/show.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-05-16 18:02:19.000000 python-barn-0.7.0/src/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-05-16 18:02:19.000000 python-barn-0.7.0/src/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-16 18:02:19.000000 python-barn-0.7.0/src/logging_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:52:14.452464 python-barn-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-16 21:52:14.452464 python-barn-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-05-16 21:52:00.000000 python-barn-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:52:14.448463 python-barn-0.8.0/python_barn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-16 21:52:14.000000 python-barn-0.8.0/python_barn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-16 21:52:14.000000 python-barn-0.8.0/python_barn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 21:52:14.000000 python-barn-0.8.0/python_barn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 21:52:14.000000 python-barn-0.8.0/python_barn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 21:52:14.000000 python-barn-0.8.0/python_barn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-16 21:52:14.000000 python-barn-0.8.0/python_barn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 21:52:14.452464 python-barn-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-16 21:52:00.000000 python-barn-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:52:14.448463 python-barn-0.8.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-16 21:52:00.000000 python-barn-0.8.0/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:52:14.452464 python-barn-0.8.0/src/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-16 21:52:00.000000 python-barn-0.8.0/src/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-16 21:52:00.000000 python-barn-0.8.0/src/actions/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-16 21:52:00.000000 python-barn-0.8.0/src/actions/execute_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-16 21:52:00.000000 python-barn-0.8.0/src/actions/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-16 21:52:00.000000 python-barn-0.8.0/src/actions/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-16 21:52:00.000000 python-barn-0.8.0/src/actions/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-16 21:52:00.000000 python-barn-0.8.0/src/actions/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-05-16 21:52:00.000000 python-barn-0.8.0/src/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8673 2023-05-16 21:52:00.000000 python-barn-0.8.0/src/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-16 21:52:00.000000 python-barn-0.8.0/src/logging_utils.py
```

### Comparing `python-barn-0.7.0/PKG-INFO` & `python-barn-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-barn
-Version: 0.7.0
+Version: 0.8.0
 Summary: A wrapper for pip, to give better utils to python projects dependency management
 Home-page: https://github.com/JacopoMadaluni/barn
 Author: Jacopo Madaluni
 Author-email: jacopo.madaluni@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `python-barn-0.7.0/README.md` & `python-barn-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `python-barn-0.7.0/python_barn.egg-info/PKG-INFO` & `python-barn-0.8.0/python_barn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-barn
-Version: 0.7.0
+Version: 0.8.0
 Summary: A wrapper for pip, to give better utils to python projects dependency management
 Home-page: https://github.com/JacopoMadaluni/barn
 Author: Jacopo Madaluni
 Author-email: jacopo.madaluni@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `python-barn-0.7.0/setup.py` & `python-barn-0.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="python-barn",
-    version="0.7.0",
+    version="0.8.0",
     packages=find_packages(),
     entry_points={
         "console_scripts": [
             "barn=src.cli:main",
         ],
     },
     package_data={
```

### Comparing `python-barn-0.7.0/src/actions/add.py` & `python-barn-0.8.0/src/actions/add.py`

 * *Files identical despite different names*

### Comparing `python-barn-0.7.0/src/actions/execute_script.py` & `python-barn-0.8.0/src/actions/execute_script.py`

 * *Files identical despite different names*

### Comparing `python-barn-0.7.0/src/actions/init.py` & `python-barn-0.8.0/src/actions/init.py`

 * *Files identical despite different names*

### Comparing `python-barn-0.7.0/src/actions/install.py` & `python-barn-0.8.0/src/actions/install.py`

 * *Files identical despite different names*

### Comparing `python-barn-0.7.0/src/cli.py` & `python-barn-0.8.0/src/cli.py`

 * *Files identical despite different names*

### Comparing `python-barn-0.7.0/src/core.py` & `python-barn-0.8.0/src/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,14 +18,22 @@
 else:
     logger.setLevel(logging.WARNING)
 
 class IndentedYamlDumper(yaml.Dumper):
     def increase_indent(self, flow=False, indentless=False):
         return super(IndentedYamlDumper, self).increase_indent(flow, False)
     
+def str_presenter(dumper, data):
+  if len(data.splitlines()) > 1:  # check for multiline string
+    return dumper.represent_scalar('tag:yaml.org,2002:str', data, style='|')
+  return dumper.represent_scalar('tag:yaml.org,2002:str', data)
+
+yaml.add_representer(str, str_presenter)
+# to use with safe_dump:
+yaml.representer.SafeRepresenter.add_representer(str, str_presenter)
 
 class Context:
     def __init__(self, root_dir: Path=None, is_initialized=False):
         if root_dir is None:
             raise ValueError("Critical error: context is missing project base directory.")
         self.root_dir = root_dir
         self.is_initialized = is_initialized
@@ -93,16 +101,16 @@
         stdout, exit_code = self.__run_command(
             f'source {self.activate_path} && {command}'
         )
 
         return stdout, exit_code
     
     def setup_bash_function_capabilities(self, name: str, command: str):
-        trailing_sc = ";" if command.strip()[-1] != ";" else ""
-        function_declaration = "function "+ name + " { " + command + trailing_sc + ' }'
+        trailing_sc = " " if command.strip()[-1] != ";" else ""
+        function_declaration = "function "+ name + "() { \n" + command + trailing_sc + '\n}'
         logger.debug(f"Setting up function: {function_declaration}")
         _, exit_code = self.__run_command(
             function_declaration
         )
         if exit_code == 0:
             self.bash_functions_declarations[name] = function_declaration
         return exit_code
@@ -154,42 +162,42 @@
 
         return yaml_content
     
     def add_dependency_to_project_yaml(self, package, version=None, is_url=False):
         yaml_content = self.get_project_config()
         if is_url:
             new_entry = {
-                package: f"N/A"
+                package: "N/A"
             }
         else:
             new_entry = {
                 package: version
             }
             
         if "dependencies" not in yaml_content:
             yaml_content["dependencies"] = []
 
         dependencies: list[any] = yaml_content["dependencies"]
         if new_entry not in dependencies:
             yaml_content["dependencies"].append(new_entry)
+            logger.debug(yaml_content)
             with open(self.project_yaml_path, 'w') as yaml_file:
                 yaml.dump(yaml_content, yaml_file, Dumper=IndentedYamlDumper, default_flow_style=False, indent=2, sort_keys=False)
 
     def remove_dependency_from_project_yaml(self, package):
         yaml_content = self.get_project_config()
 
         dependencies: list[any] = yaml_content["dependencies"]
         for index, dependency in enumerate(dependencies):
             if package in dependency:
                 del dependencies[index]
                 break
         
         yaml_content["dependencies"] = dependencies
-        
-            
+
         with open(self.project_yaml_path, 'w') as yaml_file:
             yaml.dump(yaml_content, yaml_file, Dumper=IndentedYamlDumper, default_flow_style=False, indent=2, sort_keys=False)
 
     def split_package_version(self, requirement: str):
         pattern = r'([a-zA-Z0-9-_]+)([<>=~!]+[0-9.a-zA-Z]+)?'
         match = re.match(pattern, requirement)
         if match:
```

### Comparing `python-barn-0.7.0/src/logging_utils.py` & `python-barn-0.8.0/src/logging_utils.py`

 * *Files identical despite different names*

