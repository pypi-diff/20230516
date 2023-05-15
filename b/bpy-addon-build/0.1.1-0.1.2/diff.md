# Comparing `tmp/bpy_addon_build-0.1.1.tar.gz` & `tmp/bpy_addon_build-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpy_addon_build-0.1.1.tar", max compression
+gzip compressed data, was "bpy_addon_build-0.1.2.tar", max compression
```

## Comparing `bpy_addon_build-0.1.1.tar` & `bpy_addon_build-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     4757 2023-05-14 23:04:40.989141 bpy_addon_build-0.1.1/bpy_addon_build/__init__.py
--rw-r--r--   0        0        0      550 2023-05-14 22:58:32.318576 bpy_addon_build-0.1.1/bpy_addon_build/actions.py
--rw-r--r--   0        0        0      666 2023-05-14 20:30:55.184639 bpy_addon_build-0.1.1/bpy_addon_build/yaml_conf.py
--rw-r--r--   0        0        0      550 2023-05-14 23:06:12.276625 bpy_addon_build-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      634 1970-01-01 00:00:00.000000 bpy_addon_build-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     4752 2023-05-15 22:06:22.813351 bpy_addon_build-0.1.2/bpy_addon_build/__init__.py
+-rw-r--r--   0        0        0      983 2023-05-15 22:32:57.594935 bpy_addon_build-0.1.2/bpy_addon_build/actions.py
+-rw-r--r--   0        0        0      667 2023-05-15 22:08:56.424258 bpy_addon_build-0.1.2/bpy_addon_build/yaml_conf.py
+-rw-r--r--   0        0        0      548 2023-05-15 22:35:22.869802 bpy_addon_build-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      730 1970-01-01 00:00:00.000000 bpy_addon_build-0.1.2/PKG-INFO
```

### Comparing `bpy_addon_build-0.1.1/bpy_addon_build/__init__.py` & `bpy_addon_build-0.1.2/bpy_addon_build/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 import shutil
 import time
 from pathlib import Path
-from typing import Dict, List, Optional
+from typing import List, Optional
 from rich.console import Console
 from docopt import docopt
-from . import actions
 
+from . import actions
 from . import yaml_conf
 
 # Current working directory
 WORKING_DIR: Path = Path(os.getcwd())
 
 # All file paths on Windows, MacOS, and Linux based on the Blender Docs
 # We use ~ for user directories, and we expand these later on in the code
@@ -43,14 +43,15 @@
         return yaml_config
 
 
 # Main function
 def main():
     args = docopt(USAGE)
     bpy_build_yaml: Path = WORKING_DIR / Path("bpy-build.yaml")
+
     if not args["<file>"]:
         if bpy_build_yaml.exists():
             pass
         else:
             console.print(
                 "Can't find bpy-build.yaml, maybe pass it directly?", style="bold red"
             )
```

### Comparing `bpy_addon_build-0.1.1/bpy_addon_build/yaml_conf.py` & `bpy_addon_build-0.1.2/bpy_addon_build/yaml_conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from dataclasses import dataclass
-from typing import Dict, List, TextIO
+from typing import Dict, List, Optional, TextIO
 from pathlib import Path
 import yaml
 
 
 @dataclass
-class BpyBuildYaml(object):
+class BpyBuildYaml:
     addon_folder: Path
     build_name: str
     install_versions: List[str]
-    during_build: Dict[str, List[Dict[str, str]]]
+    during_build: Optional[Dict[str, List[str]]]
 
     def __init__(self, file: TextIO, file_path: Path):
         file_data = yaml.safe_load(file)
         self.addon_folder = file_path.parents[0] / Path(file_data["addon_folder"])
         self.build_name = file_data["build_name"]
         self.install_versions = file_data["install_versions"]
```

### Comparing `bpy_addon_build-0.1.1/pyproject.toml` & `bpy_addon_build-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "bpy-addon-build"
-version = "0.1.1"
+version = "0.1.2"
 description = "A build system to make building and testing Blender addons 10 times easier"
 authors = ["StandingPad"]
 license = "MIT"
 homepage = "https://github.com/StandingPadAnimations/bpy-build"
 
 [tool.poetry.dependencies]
-python = "^3.8.1"
+python = "^3.7"
 pyyaml = "^6.0"
 rich = "^13.3.5"
 docopt = "^0.6.2"
 
 [tool.poetry.dev-dependencies]
 black = "^23.3.0"
```

### Comparing `bpy_addon_build-0.1.1/PKG-INFO` & `bpy_addon_build-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: bpy-addon-build
-Version: 0.1.1
+Version: 0.1.2
 Summary: A build system to make building and testing Blender addons 10 times easier
 Home-page: https://github.com/StandingPadAnimations/bpy-build
 License: MIT
 Author: StandingPad
-Requires-Python: >=3.8.1,<4.0.0
+Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: docopt (>=0.6.2,<0.7.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: rich (>=13.3.5,<14.0.0)
```

