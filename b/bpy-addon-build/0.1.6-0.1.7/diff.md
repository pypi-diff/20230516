# Comparing `tmp/bpy_addon_build-0.1.6.tar.gz` & `tmp/bpy_addon_build-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpy_addon_build-0.1.6.tar", max compression
+gzip compressed data, was "bpy_addon_build-0.1.7.tar", max compression
```

## Comparing `bpy_addon_build-0.1.6.tar` & `bpy_addon_build-0.1.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     4770 2023-05-15 23:17:22.409369 bpy_addon_build-0.1.6/bpy_addon_build/__init__.py
--rw-r--r--   0        0        0     1162 2023-05-15 23:31:21.125187 bpy_addon_build-0.1.6/bpy_addon_build/actions.py
--rw-r--r--   0        0        0     1021 2023-05-15 23:16:32.883680 bpy_addon_build-0.1.6/bpy_addon_build/yaml_conf.py
--rw-r--r--   0        0        0      548 2023-05-15 23:23:43.445152 bpy_addon_build-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      730 1970-01-01 00:00:00.000000 bpy_addon_build-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     4770 2023-05-15 23:17:22.409369 bpy_addon_build-0.1.7/bpy_addon_build/__init__.py
+-rw-r--r--   0        0        0     1141 2023-05-15 23:40:10.223641 bpy_addon_build-0.1.7/bpy_addon_build/actions.py
+-rw-r--r--   0        0        0     1021 2023-05-15 23:16:32.883680 bpy_addon_build-0.1.7/bpy_addon_build/yaml_conf.py
+-rw-r--r--   0        0        0      548 2023-05-15 23:40:30.227513 bpy_addon_build-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      730 1970-01-01 00:00:00.000000 bpy_addon_build-0.1.7/PKG-INFO
```

### Comparing `bpy_addon_build-0.1.6/bpy_addon_build/__init__.py` & `bpy_addon_build-0.1.7/bpy_addon_build/__init__.py`

 * *Files identical despite different names*

### Comparing `bpy_addon_build-0.1.6/bpy_addon_build/actions.py` & `bpy_addon_build-0.1.7/bpy_addon_build/actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,9 +25,9 @@
         files: List[str] = extracted_str.group(1).split("->")
         src: Path = Path(files[0].replace('"', "")).expanduser()
         dst: Path = inter_dir / Path(files[1].replace('"', ""))
         shutil.copy2(src, dst)
 
     if "execute_sh" in action:
         command = shlex.split(extracted_str.group(1))
-        output = subprocess.run(command, shell=True, cwd=inter_dir, capture_output=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+        output = subprocess.run(command, shell=True, cwd=inter_dir, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
         console.print(output.stdout.decode("UTF-8"))
```

### Comparing `bpy_addon_build-0.1.6/bpy_addon_build/yaml_conf.py` & `bpy_addon_build-0.1.7/bpy_addon_build/yaml_conf.py`

 * *Files identical despite different names*

### Comparing `bpy_addon_build-0.1.6/pyproject.toml` & `bpy_addon_build-0.1.7/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bpy-addon-build"
-version = "0.1.6"
+version = "0.1.7"
 description = "A build system to make building and testing Blender addons 10 times easier"
 authors = ["StandingPad"]
 license = "MIT"
 homepage = "https://github.com/StandingPadAnimations/bpy-build"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `bpy_addon_build-0.1.6/PKG-INFO` & `bpy_addon_build-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpy-addon-build
-Version: 0.1.6
+Version: 0.1.7
 Summary: A build system to make building and testing Blender addons 10 times easier
 Home-page: https://github.com/StandingPadAnimations/bpy-build
 License: MIT
 Author: StandingPad
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

