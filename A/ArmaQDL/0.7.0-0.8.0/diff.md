# Comparing `tmp/armaqdl-0.7.0.tar.gz` & `tmp/armaqdl-0.8.0.tar.gz`

## Comparing `armaqdl-0.7.0.tar` & `armaqdl-0.8.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 armaqdl-0.7.0/.editorconfig
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 armaqdl-0.7.0/.flake8
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 armaqdl-0.7.0/.gitattributes
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 armaqdl-0.7.0/armaqdl/__init__.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 armaqdl-0.7.0/armaqdl/__main__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 armaqdl-0.7.0/armaqdl/_version.py
--rw-r--r--   0        0        0    15915 2020-02-02 00:00:00.000000 armaqdl-0.7.0/armaqdl/armaqdl.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 armaqdl-0.7.0/armaqdl/config.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 armaqdl-0.7.0/armaqdl/const.py
--rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 armaqdl-0.7.0/armaqdl/update.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 armaqdl-0.7.0/config/settings.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 armaqdl-0.7.0/tests/__init__.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 armaqdl-0.7.0/tests/test_commands.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 armaqdl-0.7.0/tests/test_config.py
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 armaqdl-0.7.0/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 armaqdl-0.7.0/LICENSE
--rw-r--r--   0        0        0     6808 2020-02-02 00:00:00.000000 armaqdl-0.7.0/README.md
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 armaqdl-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     7791 2020-02-02 00:00:00.000000 armaqdl-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 armaqdl-0.8.0/.editorconfig
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 armaqdl-0.8.0/.flake8
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 armaqdl-0.8.0/.gitattributes
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 armaqdl-0.8.0/armaqdl/__init__.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 armaqdl-0.8.0/armaqdl/__main__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 armaqdl-0.8.0/armaqdl/_version.py
+-rw-r--r--   0        0        0    16500 2020-02-02 00:00:00.000000 armaqdl-0.8.0/armaqdl/armaqdl.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 armaqdl-0.8.0/armaqdl/config.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 armaqdl-0.8.0/armaqdl/const.py
+-rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 armaqdl-0.8.0/armaqdl/update.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 armaqdl-0.8.0/config/settings.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 armaqdl-0.8.0/tests/__init__.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 armaqdl-0.8.0/tests/test_commands.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 armaqdl-0.8.0/tests/test_config.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 armaqdl-0.8.0/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 armaqdl-0.8.0/LICENSE
+-rw-r--r--   0        0        0     6808 2020-02-02 00:00:00.000000 armaqdl-0.8.0/README.md
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 armaqdl-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     7791 2020-02-02 00:00:00.000000 armaqdl-0.8.0/PKG-INFO
```

### Comparing `armaqdl-0.7.0/armaqdl/armaqdl.py` & `armaqdl-0.8.0/armaqdl/armaqdl.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,40 +17,57 @@
 
 
 VERBOSE = False
 DRY = False
 SETTINGS = None
 
 
-def find_arma(executable=True):
+def find_arma():
     path = None
 
     if os.name == "nt":
         try:
             k = winreg.OpenKey(winreg.HKEY_LOCAL_MACHINE, r"SOFTWARE\WOW6432Node\Bohemia Interactive\Arma 3")
             path = winreg.EnumValue(k, 1)[1]
             winreg.CloseKey(k)
         except OSError as e:
             print(f"Error! Could not find Arma path in registry.\n{e}")
             return None
 
         path = Path(path)
 
-        if executable:
-            path = path / "arma3_x64.exe"
-
         if not path.exists():
             return None
     else:
         # Linux support does not exist, this is just for testing
         path = Path()
 
     return path
 
 
+def find_arma_exe(executable):
+    executable = executable.replace("\\", "/").replace("//", "/")  # Support single backwards slashes on Windows
+
+    if "/" in executable:
+        # Absolute
+        path = Path(executable)
+    else:
+        # Relative to the Arma 3 directory
+        path = find_arma()
+        if not path:
+            return None
+
+        path /= f"{executable}.exe"
+
+    if not path.exists():
+        return None
+
+    return path
+
+
 def open_last_rpt():
     if os.name == "nt":
         log_open_delay = SETTINGS.get('log', {}).get('open_delay', 3)
         print(f"Opening last log in {log_open_delay}s ...")
         if not DRY:
             time.sleep(log_open_delay)
 
@@ -253,15 +270,15 @@
     return path
 
 
 def process_mission_server(mission):
     if not mission:
         return ""
 
-    arma_path = find_arma(executable=False)
+    arma_path = find_arma()
     if not arma_path:
         return ""
 
     # Remove "/mission.sqm"
     if mission.name == "mission.sqm":
         mission = mission.parent
 
@@ -365,15 +382,15 @@
 
 def run_arma(arma_path, params):
     process_cmd = [arma_path] + params
 
     if VERBOSE:
         print(f"Process command: {process_cmd}")
 
-    print("Running ...")
+    print(f"Running {arma_path.stem} ...")
     if not DRY:
         # Don't wait for process to finish (Popen() instead of run())
         subprocess.Popen(process_cmd)
 
 
 def main():
     # Generate new config
@@ -400,14 +417,16 @@
     parser.add_argument("-ne", "--no-errors", action="store_true", help="hide script errors")
     parser.add_argument("-nd", "--no-debug", action="store_true", help="disable debug mode")
     parser.add_argument("-np", "--no-pause", action="store_true", help="don't pause on focus loss")
     parser.add_argument("-c", "--check-signatures", action="store_true", help="check signatures")
     parser.add_argument("-f", "--fullscreen", action="store_true")
     parser.add_argument("-par", "--parameters", nargs="+", type=str,
                         help="other parameters to pass directly (use with '=' to pass '-<arg>')")
+    parser.add_argument("-e", "--executable", default="arma3_x64", type=str,
+                        help="Arma executable to launch (relative to Arma directory without .exe or absolute with .exe)")
 
     parser.add_argument("-b", "--build", metavar="TOOL", nargs="?", const="b", type=str,
                         help="build mods (auto-determine tool if unspecified)")
     parser.add_argument("-nl", "--no-log", action="store_true", help="don't open last log")
 
     parser.add_argument("--config", default=config.CONFIG_DIR, type=Path, help="load config from specified folder")
     parser.add_argument("--list", action="store_true", help="list active config locations and build tools")
@@ -458,15 +477,15 @@
     if "none" in args.mods:
         print("Warning! Launching without any mods (vanilla!)")
     elif not args.mods:
         print("Empty mod paths - use 'none' to launch without any mods (vanilla).")
         return 0
 
     # Arma path
-    arma_path = find_arma(executable=True)
+    arma_path = find_arma_exe(executable=args.executable)
     if not arma_path:
         print("Error! Invalid Arma path.")
         return 2
 
     # Mods
     param_mods = process_mods(args.mods, args.build)
     if param_mods is None:
```

### Comparing `armaqdl-0.7.0/armaqdl/config.py` & `armaqdl-0.8.0/armaqdl/config.py`

 * *Files identical despite different names*

### Comparing `armaqdl-0.7.0/armaqdl/update.py` & `armaqdl-0.8.0/armaqdl/update.py`

 * *Files identical despite different names*

### Comparing `armaqdl-0.7.0/config/settings.toml` & `armaqdl-0.8.0/config/settings.toml`

 * *Files identical despite different names*

### Comparing `armaqdl-0.7.0/tests/test_commands.py` & `armaqdl-0.8.0/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `armaqdl-0.7.0/tests/test_config.py` & `armaqdl-0.8.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `armaqdl-0.7.0/.gitignore` & `armaqdl-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `armaqdl-0.7.0/LICENSE` & `armaqdl-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `armaqdl-0.7.0/README.md` & `armaqdl-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `armaqdl-0.7.0/pyproject.toml` & `armaqdl-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `armaqdl-0.7.0/PKG-INFO` & `armaqdl-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ArmaQDL
-Version: 0.7.0
+Version: 0.8.0
 Summary: Python program for quick launching various mod development configurations for Arma through a simple CLI.
 Project-URL: Homepage, https://github.com/jonpas/Arma-QDL
 Project-URL: Bug Tracker, https://github.com/jonpas/Arma-QDL/issues
 Author-email: Jonpas <jonpas33@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Environment :: Console
```

