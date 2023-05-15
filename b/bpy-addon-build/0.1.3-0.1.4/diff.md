# Comparing `tmp/bpy_addon_build-0.1.3.tar.gz` & `tmp/bpy_addon_build-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpy_addon_build-0.1.3.tar", max compression
+gzip compressed data, was "bpy_addon_build-0.1.4.tar", max compression
```

## Comparing `bpy_addon_build-0.1.3.tar` & `bpy_addon_build-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     4752 2023-05-15 22:51:02.597515 bpy_addon_build-0.1.3/bpy_addon_build/__init__.py
--rw-r--r--   0        0        0      983 2023-05-15 22:32:57.594935 bpy_addon_build-0.1.3/bpy_addon_build/actions.py
--rw-r--r--   0        0        0     1032 2023-05-15 22:50:43.257758 bpy_addon_build-0.1.3/bpy_addon_build/yaml_conf.py
--rw-r--r--   0        0        0      548 2023-05-15 22:51:57.480130 bpy_addon_build-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      730 1970-01-01 00:00:00.000000 bpy_addon_build-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     4752 2023-05-15 22:51:02.597515 bpy_addon_build-0.1.4/bpy_addon_build/__init__.py
+-rw-r--r--   0        0        0      961 2023-05-15 22:58:06.911116 bpy_addon_build-0.1.4/bpy_addon_build/actions.py
+-rw-r--r--   0        0        0     1021 2023-05-15 22:53:04.112538 bpy_addon_build-0.1.4/bpy_addon_build/yaml_conf.py
+-rw-r--r--   0        0        0      548 2023-05-15 23:05:22.479973 bpy_addon_build-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      730 1970-01-01 00:00:00.000000 bpy_addon_build-0.1.4/PKG-INFO
```

### Comparing `bpy_addon_build-0.1.3/bpy_addon_build/__init__.py` & `bpy_addon_build-0.1.4/bpy_addon_build/__init__.py`

 * *Files identical despite different names*

### Comparing `bpy_addon_build-0.1.3/bpy_addon_build/actions.py` & `bpy_addon_build-0.1.4/bpy_addon_build/actions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import subprocess
 import shlex
 from typing import List
 from pathlib import Path
 import shutil
 import re
 
+
 # Execute an action
 def execute_action(action: str, inter_dir: Path):
     extracted_str = re.search("\((.+?)\)", action)
     if not extracted_str:
         print(
             f"[bold red]Invalid action: {action}, perhaps you forgot parenthesis?[/bold red]"
         )
@@ -23,9 +24,8 @@
         files: List[str] = extracted_str.group(1).split("->")
         src: Path = Path(files[0].replace('"', "")).expanduser()
         dst: Path = inter_dir / Path(files[1].replace('"', ""))
         shutil.copy2(src, dst)
 
     if "execute_sh" in action:
         command = shlex.split(extracted_str.group(1))
-        print(command)
         subprocess.call(command, shell=True, cwd=inter_dir)
```

### Comparing `bpy_addon_build-0.1.3/bpy_addon_build/yaml_conf.py` & `bpy_addon_build-0.1.4/bpy_addon_build/yaml_conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from dataclasses import dataclass
 from typing import Dict, List, Optional, TextIO
 from pathlib import Path
 import yaml
 import rich
 
+
 @dataclass
 class BpyBuildYaml:
     addon_folder: Path
     build_name: str
     install_versions: Optional[List[str]]
     during_build: Optional[Dict[str, List[str]]]
 
@@ -15,15 +16,15 @@
         file_data = yaml.safe_load(file)
         if "addon_folder" not in file_data:
             print("[bold red]You need to specify the addon_folder![/bold red]")
             quit()
         if "build_name" not in file_data:
             print("[bold red]You need to specify the build name![/bold red]")
             quit()
-            
+
         self.addon_folder = file_path.parents[0] / Path(file_data["addon_folder"])
         self.build_name = file_data["build_name"]
 
         if "install_versions" in file_data:
             self.install_versions = file_data["install_versions"]
 
         if "during_build" in file_data:
```

### Comparing `bpy_addon_build-0.1.3/pyproject.toml` & `bpy_addon_build-0.1.4/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bpy-addon-build"
-version = "0.1.3"
+version = "0.1.4"
 description = "A build system to make building and testing Blender addons 10 times easier"
 authors = ["StandingPad"]
 license = "MIT"
 homepage = "https://github.com/StandingPadAnimations/bpy-build"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `bpy_addon_build-0.1.3/PKG-INFO` & `bpy_addon_build-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpy-addon-build
-Version: 0.1.3
+Version: 0.1.4
 Summary: A build system to make building and testing Blender addons 10 times easier
 Home-page: https://github.com/StandingPadAnimations/bpy-build
 License: MIT
 Author: StandingPad
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

