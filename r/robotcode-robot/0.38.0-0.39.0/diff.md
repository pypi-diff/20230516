# Comparing `tmp/robotcode_robot-0.38.0.tar.gz` & `tmp/robotcode_robot-0.39.0.tar.gz`

## Comparing `robotcode_robot-0.38.0.tar` & `robotcode_robot-0.39.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.38.0/src/robotcode/robot/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_robot-0.38.0/src/robotcode/robot/__version__.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_robot-0.38.0/src/robotcode/robot/py.typed
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 robotcode_robot-0.38.0/src/robotcode/robot/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.38.0/src/robotcode/robot/config/__init__.py
--rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 robotcode_robot-0.38.0/src/robotcode/robot/config/loader.py
--rw-r--r--   0        0        0    78347 2020-02-02 00:00:00.000000 robotcode_robot-0.38.0/src/robotcode/robot/config/model.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 robotcode_robot-0.38.0/src/robotcode/robot/config/utils.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_robot-0.38.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_robot-0.38.0/LICENSE.txt
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 robotcode_robot-0.38.0/README.md
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 robotcode_robot-0.38.0/pyproject.toml
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 robotcode_robot-0.38.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.39.0/src/robotcode/robot/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_robot-0.39.0/src/robotcode/robot/__version__.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_robot-0.39.0/src/robotcode/robot/py.typed
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 robotcode_robot-0.39.0/src/robotcode/robot/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.39.0/src/robotcode/robot/config/__init__.py
+-rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 robotcode_robot-0.39.0/src/robotcode/robot/config/loader.py
+-rw-r--r--   0        0        0    78409 2020-02-02 00:00:00.000000 robotcode_robot-0.39.0/src/robotcode/robot/config/model.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 robotcode_robot-0.39.0/src/robotcode/robot/config/utils.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_robot-0.39.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_robot-0.39.0/LICENSE.txt
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 robotcode_robot-0.39.0/README.md
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 robotcode_robot-0.39.0/pyproject.toml
+-rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 robotcode_robot-0.39.0/PKG-INFO
```

### Comparing `robotcode_robot-0.38.0/src/robotcode/robot/config/loader.py` & `robotcode_robot-0.39.0/src/robotcode/robot/config/loader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
 from enum import Enum
 from pathlib import Path
-from typing import Optional, Sequence, Tuple, Union
+from typing import Any, Optional, Sequence, Tuple, Union
 
 from robotcode.core.dataclasses import from_dict
 
 if sys.version_info >= (3, 11):
     import tomllib
 else:
     import tomli as tomllib
@@ -30,33 +30,50 @@
 class ConfigType(str, Enum):
     PYPROJECT_TOML = PYPROJECT_TOML
     ROBOT_TOML = ROBOT_TOML
     LOCAL_ROBOT_TOML = LOCAL_ROBOT_TOML
     CUSTOM_TOML = ".toml"
 
 
+class ConfigValueError(ValueError):
+    def __init__(self, path: Path, *args: Any, **kwargs: Any) -> None:
+        super().__init__(*args, **kwargs)
+        self.path = path
+
+
+class ConfigTypeError(TypeError):
+    def __init__(self, path: Path, *args: Any, **kwargs: Any) -> None:
+        super().__init__(*args, **kwargs)
+        self.path = path
+
+
 def loads_config_from_robot_toml(__s: str) -> RobotConfig:
     dict_data = tomllib.loads(__s)
     return from_dict(dict_data, RobotConfig)
 
 
 def loads_config_from_pyproject_toml(__s: str) -> RobotConfig:
     dict_data = tomllib.loads(__s)
 
     return from_dict(dict_data.get("tool", {}).get("robot", {}), RobotConfig)
 
 
 def _load_config_data_from_path(__path: Path) -> RobotConfig:
-    if __path.name == PYPROJECT_TOML:
-        return loads_config_from_pyproject_toml(__path.read_text("utf-8"))
-
-    if __path.name == ROBOT_TOML or __path.name == LOCAL_ROBOT_TOML:
-        return loads_config_from_robot_toml(__path.read_text("utf-8"))
-
-    raise ValueError(f"Unknown config file type: {__path.name}")
+    try:
+        if __path.name == PYPROJECT_TOML:
+            return loads_config_from_pyproject_toml(__path.read_text("utf-8"))
+
+        if __path.name == ROBOT_TOML or __path.name == LOCAL_ROBOT_TOML or __path.suffix == ".toml":
+            return loads_config_from_robot_toml(__path.read_text("utf-8"))
+        raise TypeError("Unknown config file type.")
+
+    except ValueError as e:
+        raise ConfigValueError(__path, f'Parsing "{__path}" failed: {e}') from e
+    except TypeError as e:
+        raise ConfigTypeError(__path, f'Parsing "{__path}" failed: {e}') from e
 
 
 def load_config_from_path(*__paths: Union[Path, Tuple[Path, ConfigType]]) -> RobotConfig:
     result = RobotConfig()
 
     for __path in __paths:
         result.add_options(_load_config_data_from_path(__path if isinstance(__path, Path) else __path[0]))
```

### Comparing `robotcode_robot-0.38.0/src/robotcode/robot/config/model.py` & `robotcode_robot-0.39.0/src/robotcode/robot/config/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,14 +136,17 @@
 @dataclass
 class StringExpression(Expression):
     """Expression to evaluate to a string."""
 
     def evaluate(self) -> str:
         return str(super().evaluate())
 
+    def __str__(self) -> str:
+        return self.evaluate()
+
 
 @dataclass
 class Condition:
     """Condition to evaluate."""
 
     if_: str = field(
         description="""\
```

### Comparing `robotcode_robot-0.38.0/src/robotcode/robot/config/utils.py` & `robotcode_robot-0.39.0/src/robotcode/robot/config/utils.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.38.0/.gitignore` & `robotcode_robot-0.39.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.38.0/LICENSE.txt` & `robotcode_robot-0.39.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.38.0/README.md` & `robotcode_robot-0.39.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.38.0/pyproject.toml` & `robotcode_robot-0.39.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dependencies = [
   "robotframework>=4.1.0",
   "tomli>=1.1.0; python_version < '3.11'",
-  "robotcode-core==0.38.0",
+  "robotcode-core==0.39.0",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://robotcode.io"
 Donate = "https://github.com/sponsors/d-biehl"
 Documentation = "https://github.com/d-biehl/robotcode#readme"
```

### Comparing `robotcode_robot-0.38.0/PKG-INFO` & `robotcode_robot-0.39.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-robot
-Version: 0.38.0
+Version: 0.39.0
 Summary: Support classes for RobotCode for handling Robot Framework projects.
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-core==0.38.0
+Requires-Dist: robotcode-core==0.39.0
 Requires-Dist: robotframework>=4.1.0
 Requires-Dist: tomli>=1.1.0; python_version < '3.11'
 Description-Content-Type: text/markdown
 
 # robotcode-robot
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-robot.svg)](https://pypi.org/project/robotcode-robot)
```

