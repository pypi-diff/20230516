# Comparing `tmp/skeletonkey-0.0.11.tar.gz` & `tmp/skeletonkey-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skeletonkey-0.0.11.tar", last modified: Fri Apr 28 02:06:21 2023, max compression
+gzip compressed data, was "skeletonkey-0.1.0.tar", last modified: Tue May 16 00:30:55 2023, max compression
```

## Comparing `skeletonkey-0.0.11.tar` & `skeletonkey-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 sizemol  (77241) grp.csci.Faculty (71145)        0 2023-04-28 02:06:21.565911 skeletonkey-0.0.11/
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     1071 2023-04-27 04:50:50.000000 skeletonkey-0.0.11/LICENSE
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     1667 2023-04-28 02:06:21.553910 skeletonkey-0.0.11/PKG-INFO
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     1176 2023-04-28 01:59:03.000000 skeletonkey-0.0.11/README.md
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)       38 2023-04-28 02:06:21.593912 skeletonkey-0.0.11/setup.cfg
--rw-rw-r--   0 sizemol  (77241) grp.csci.Faculty (71145)      718 2023-04-28 02:05:55.000000 skeletonkey-0.0.11/setup.py
-drwxr-xr-x   0 sizemol  (77241) grp.csci.Faculty (71145)        0 2023-04-28 02:06:21.045885 skeletonkey-0.0.11/skeletonkey/
--rw-rw-r--   0 sizemol  (77241) grp.csci.Faculty (71145)     5043 2023-04-28 01:55:09.000000 skeletonkey-0.0.11/skeletonkey/__init__.py
--rw-rw-r--   0 sizemol  (77241) grp.csci.Faculty (71145)     6367 2023-04-28 00:17:00.000000 skeletonkey-0.0.11/skeletonkey/utils.py
-drwxr-xr-x   0 sizemol  (77241) grp.csci.Faculty (71145)        0 2023-04-28 02:06:21.393902 skeletonkey-0.0.11/skeletonkey.egg-info/
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     1667 2023-04-28 02:06:20.000000 skeletonkey-0.0.11/skeletonkey.egg-info/PKG-INFO
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)      211 2023-04-28 02:06:20.000000 skeletonkey-0.0.11/skeletonkey.egg-info/SOURCES.txt
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)        1 2023-04-28 02:06:20.000000 skeletonkey-0.0.11/skeletonkey.egg-info/dependency_links.txt
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)       12 2023-04-28 02:06:20.000000 skeletonkey-0.0.11/skeletonkey.egg-info/top_level.txt
+drwxr-xr-x   0 sizemol  (77241) grp.csci.Faculty (71145)        0 2023-05-16 00:30:54.970136 skeletonkey-0.1.0/
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     1071 2023-05-01 03:35:36.000000 skeletonkey-0.1.0/LICENSE
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     4304 2023-05-16 00:30:54.950135 skeletonkey-0.1.0/PKG-INFO
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     3814 2023-05-01 05:00:51.000000 skeletonkey-0.1.0/README.md
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)       38 2023-05-16 00:30:54.986137 skeletonkey-0.1.0/setup.cfg
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)      717 2023-05-16 00:30:42.000000 skeletonkey-0.1.0/setup.py
+drwxr-xr-x   0 sizemol  (77241) grp.csci.Faculty (71145)        0 2023-05-16 00:30:54.502113 skeletonkey-0.1.0/skeletonkey/
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)      562 2023-05-01 04:36:26.000000 skeletonkey-0.1.0/skeletonkey/__init__.py
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     8060 2023-05-01 05:05:03.000000 skeletonkey-0.1.0/skeletonkey/config.py
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     4658 2023-05-01 04:36:26.000000 skeletonkey-0.1.0/skeletonkey/core.py
+drwxr-xr-x   0 sizemol  (77241) grp.csci.Faculty (71145)        0 2023-05-16 00:30:54.846130 skeletonkey-0.1.0/skeletonkey.egg-info/
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     4304 2023-05-16 00:30:52.000000 skeletonkey-0.1.0/skeletonkey.egg-info/PKG-INFO
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)      232 2023-05-16 00:30:52.000000 skeletonkey-0.1.0/skeletonkey.egg-info/SOURCES.txt
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)        1 2023-05-16 00:30:52.000000 skeletonkey-0.1.0/skeletonkey.egg-info/dependency_links.txt
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)       12 2023-05-16 00:30:52.000000 skeletonkey-0.1.0/skeletonkey.egg-info/top_level.txt
```

### Comparing `skeletonkey-0.0.11/LICENSE` & `skeletonkey-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skeletonkey-0.0.11/setup.py` & `skeletonkey-0.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="skeletonkey",
-    version="0.0.11",
+    version="0.1.0",
     description="A bare-bones configuration managment tool.",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sizemore0125/skeletonkey",
     author="Logan Sizemore",
     author_email="sizemore0125@gmail.com",
```

### Comparing `skeletonkey-0.0.11/skeletonkey/__init__.py` & `skeletonkey-0.1.0/skeletonkey/core.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,15 @@
-"""
-Author: Logan Sizemore
-Date: 4/27/23
-
-This code provides decorator for parsing and injecting configuration arguments into a main function 
-and an instantiate funtion that can dynamically instantiate classes with their configurations. 
-It facilitates the management of complex configurations for applications using YAML files and enables 
-the dynamic loading of classes and their arguments at runtime.
-"""
-
 import argparse
 import functools
 import inspect
 import os
 import sys
 from typing import Callable, Optional, Type, Any, Dict
 
-from .utils import open_yaml, load_yaml_config, add_args_from_dict, add_yaml_extension
+from .config import load_yaml_config, add_args_from_dict, add_yaml_extension, namespace_to_nested_namespace
 
 
 def get_config_dir_path(config_path: str) -> str:
     """
     Convert a given relative or absolute config file path to its absolute directory path.
 
     Args:
@@ -44,15 +34,14 @@
             config_path = config_path[len("../") :]
             path_from_main = os.path.dirname(path_from_main)
 
         # Create absolute path.
         config_path = os.path.join(path_from_main, config_path)
     return config_path
 
-
 def unlock(config_name: str, config_path: Optional[str] = None) -> Callable:
     """
     Create a decorator for parsing and injecting configuration arguments into a
     main function from a YAML file.
 
     Args:
         config_name (str): The name of the YAML configuration file.
@@ -74,14 +63,15 @@
 
     def _parse_config(main: Callable):
         @functools.wraps(main)
         def _inner_function():
             parser = argparse.ArgumentParser()
             add_args_from_dict(parser, config)
             args = parser.parse_args()
+            args = namespace_to_nested_namespace(args)
             main(args)
 
         return _inner_function
 
     return _parse_config
 
 
@@ -101,32 +91,32 @@
     module_name = ".".join(parts[:-1])
     class_name = parts[-1]
     module = __import__(module_name, fromlist=[class_name])
     class_obj = getattr(module, class_name)
     return class_obj
 
 
-def instantiate(kwargs: Dict[str, Any]) -> Any:
+def instantiate(namespace: argparse.Namespace) -> Any:
     """
     Instantiate a class object using a dictionary of keyword arguments.
     The dictionary should contain the keys "_kwargs_" and "_target_" to
     specify the class to instantiate and its arguments.
 
     Args:
-        kwargs (Dict[str, Any]): A dictionary containing the keys "_kwargs_"
-                                 and "_target_" to specify the class and its
-                                 arguments, along with any additional keyword
-                                 arguments for the class.
+        namespace (argparse.Namespace): A Namespace object containing the key "_kwargs_" 
+            to specify the class and its arguments, along with any additional keyword 
+            arguments for the class.
 
     Returns:
         Any: An instance of the specified class.
 
     Raises:
         AssertionError: If the class is missing specific parameters.
     """
+    kwargs = vars(namespace)
     target_keyword = "_target_"
     class_obj = import_class(kwargs[target_keyword])
     del kwargs[target_keyword]
 
     obj_parameters = list(inspect.signature(class_obj).parameters)
     valid_parameters = {k: v for k, v in kwargs.items() if k in obj_parameters}
     missing_parameters = [k for k in obj_parameters if k not in valid_parameters.keys()]
```

### Comparing `skeletonkey-0.0.11/skeletonkey/utils.py` & `skeletonkey-0.1.0/skeletonkey/config.py`

 * *Files 25% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 def load_yaml_config(config_path: str, config_name: str, default_keyword: str = "defaults") ->  dict:
     """
     Load a YAML configuration file and update it with default configurations.
 
     Args:
         path (str): The file path to the YAML configuration file.
         default_keyword (str): The keyword used to identify default configurations
-                               in the YAML file. Defaults to "defaults".
+            in the YAML file. Defaults to "defaults".
 
     Returns:
         dict: The updated configuration dictionary.
     """
     path = os.path.join(config_path, config_name)
     config = open_yaml(path)
     
@@ -142,24 +142,67 @@
             if isinstance(default_yaml, str):
                 default_yaml = add_yaml_extension(default_yaml)
                 default_config = open_yaml(os.path.join(config_path, default_yaml))
             elif isinstance(default_yaml, dict):
                 yaml_paths = get_default_yaml_paths_from_dict(default_yaml)
                 default_configs = [open_yaml(os.path.join(config_path, yaml_path)) for yaml_path in yaml_paths]
                 default_config = {key: value for config_dict in default_configs for key, value in config_dict.items()}
-            config.update(default_config)
+            config.update((key, value) for key, value in default_config.items() if key not in config)
 
     return config
 
-def add_args_from_dict(arg_parser: argparse.ArgumentParser, config: dict) -> None:
+def add_args_from_dict(arg_parser: argparse.ArgumentParser, config: dict, prefix='') -> None:
     """
     Add arguments to an ArgumentParser instance using key-value pairs from a 
-    configuration dictionary.
-
+    configuration dictionary. If the dictionary contains a nested dictionary, the
+    argument will be added as --key.key value.
     Args:
         arg_parser (argparse.ArgumentParser): The ArgumentParser instance to which
                                               arguments will be added.
         config (dict): A dictionary containing key-value pairs representing
                        the arguments and their default values.
+        prefix (str, optional): The prefix string for nested keys. Defaults to ''.
     """
     for key, value in config.items():
-        arg_parser.add_argument(f"--{key}", default=value, type=type(value))
+        if isinstance(value, dict):
+            add_args_from_dict(arg_parser, value, f'{prefix}{key}.')
+        else:
+            arg_parser.add_argument(f"--{prefix}{key}", default=value, type=type(value))
+
+
+def dict_to_namespace(dictionary: dict) -> argparse.Namespace:
+    """
+    Convert a dictionary to an argparse.Namespace object recursively.
+
+    Args:
+        dictionary (dict): The dictionary to be converted.
+
+    Returns:
+        argparse.Namespace: A Namespace object representing the input dictionary.
+    """
+    for key, value in dictionary.items():
+        if isinstance(value, dict):
+            dictionary[key] = dict_to_namespace(value)
+    return argparse.Namespace(**dictionary)
+
+
+def namespace_to_nested_namespace(namespace: argparse.Namespace) -> argparse.Namespace:
+    """
+    Convert an argparse.Namespace object with 'key1.keyn' formatted keys into a nested Namespace object.
+
+    Args:
+        namespace (argparse.Namespace): The Namespace object to be converted.
+
+    Returns:
+        argparse.Namespace: A nested Namespace representation of the input Namespace object.
+    """
+    nested_dict = {}
+    for key, value in vars(namespace).items():
+        keys = key.split(".")
+        current_dict = nested_dict
+        for sub_key in keys[:-1]:
+            if sub_key not in current_dict:
+                current_dict[sub_key] = {}
+            current_dict = current_dict[sub_key]
+        current_dict[keys[-1]] = value
+
+    return dict_to_namespace(nested_dict)
```

