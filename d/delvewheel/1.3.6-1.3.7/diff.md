# Comparing `tmp/delvewheel-1.3.6.tar.gz` & `tmp/delvewheel-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delvewheel-1.3.6.tar", last modified: Tue Apr 18 13:53:35 2023, max compression
+gzip compressed data, was "delvewheel-1.3.7.tar", last modified: Tue May 16 15:22:27 2023, max compression
```

## Comparing `delvewheel-1.3.6.tar` & `delvewheel-1.3.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 13:53:35.003922 delvewheel-1.3.6/
--rw-rw-rw-   0        0        0     1073 2023-04-18 13:53:04.000000 delvewheel-1.3.6/LICENSE
--rw-rw-rw-   0        0        0    10121 2023-04-18 13:53:35.003922 delvewheel-1.3.6/PKG-INFO
--rw-rw-rw-   0        0        0     9001 2023-04-18 13:53:04.000000 delvewheel-1.3.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 13:53:34.988566 delvewheel-1.3.6/delvewheel/
--rw-rw-rw-   0        0        0        0 2023-04-18 13:53:04.000000 delvewheel-1.3.6/delvewheel/__init__.py
--rw-rw-rw-   0        0        0     5169 2023-04-18 13:53:04.000000 delvewheel-1.3.6/delvewheel/__main__.py
--rw-rw-rw-   0        0        0   138556 2023-04-18 13:53:04.000000 delvewheel-1.3.6/delvewheel/_dll_list.py
--rw-rw-rw-   0        0        0    32890 2023-04-18 13:53:04.000000 delvewheel-1.3.6/delvewheel/_dll_utils.py
--rw-rw-rw-   0        0        0       23 2023-04-18 13:53:04.000000 delvewheel-1.3.6/delvewheel/_version.py
--rw-rw-rw-   0        0        0    41066 2023-04-18 13:53:04.000000 delvewheel-1.3.6/delvewheel/_wheel_repair.py
-drwxrwxrwx   0        0        0        0 2023-04-18 13:53:35.003922 delvewheel-1.3.6/delvewheel.egg-info/
--rw-rw-rw-   0        0        0    10121 2023-04-18 13:53:34.000000 delvewheel-1.3.6/delvewheel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      394 2023-04-18 13:53:34.000000 delvewheel-1.3.6/delvewheel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 13:53:34.000000 delvewheel-1.3.6/delvewheel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-04-18 13:53:34.000000 delvewheel-1.3.6/delvewheel.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-04-18 13:53:34.000000 delvewheel-1.3.6/delvewheel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-18 13:53:34.000000 delvewheel-1.3.6/delvewheel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      117 2023-04-18 13:53:04.000000 delvewheel-1.3.6/pyproject.toml
--rw-rw-rw-   0        0        0     1214 2023-04-18 13:53:35.003922 delvewheel-1.3.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-16 15:22:27.239392 delvewheel-1.3.7/
+-rw-rw-rw-   0        0        0     1073 2023-05-16 15:21:43.000000 delvewheel-1.3.7/LICENSE
+-rw-rw-rw-   0        0        0    10414 2023-05-16 15:22:27.239392 delvewheel-1.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0     9294 2023-05-16 15:21:43.000000 delvewheel-1.3.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 15:22:27.239392 delvewheel-1.3.7/delvewheel/
+-rw-rw-rw-   0        0        0        0 2023-05-16 15:21:43.000000 delvewheel-1.3.7/delvewheel/__init__.py
+-rw-rw-rw-   0        0        0     5169 2023-05-16 15:21:43.000000 delvewheel-1.3.7/delvewheel/__main__.py
+-rw-rw-rw-   0        0        0   138609 2023-05-16 15:21:43.000000 delvewheel-1.3.7/delvewheel/_dll_list.py
+-rw-rw-rw-   0        0        0    32890 2023-05-16 15:21:43.000000 delvewheel-1.3.7/delvewheel/_dll_utils.py
+-rw-rw-rw-   0        0        0       23 2023-05-16 15:21:43.000000 delvewheel-1.3.7/delvewheel/_version.py
+-rw-rw-rw-   0        0        0    38757 2023-05-16 15:21:43.000000 delvewheel-1.3.7/delvewheel/_wheel_repair.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:22:27.239392 delvewheel-1.3.7/delvewheel.egg-info/
+-rw-rw-rw-   0        0        0    10414 2023-05-16 15:22:27.000000 delvewheel-1.3.7/delvewheel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2023-05-16 15:22:27.000000 delvewheel-1.3.7/delvewheel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 15:22:27.000000 delvewheel-1.3.7/delvewheel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-05-16 15:22:27.000000 delvewheel-1.3.7/delvewheel.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-05-16 15:22:27.000000 delvewheel-1.3.7/delvewheel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-16 15:22:27.000000 delvewheel-1.3.7/delvewheel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      117 2023-05-16 15:21:43.000000 delvewheel-1.3.7/pyproject.toml
+-rw-rw-rw-   0        0        0     1214 2023-05-16 15:22:27.239392 delvewheel-1.3.7/setup.cfg
```

### Comparing `delvewheel-1.3.6/LICENSE` & `delvewheel-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `delvewheel-1.3.6/PKG-INFO` & `delvewheel-1.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delvewheel
-Version: 1.3.6
+Version: 1.3.7
 Summary: Self-contained wheels for Windows
 Home-page: https://github.com/adang1345/delvewheel
 Author: Aohan Dang
 Author-email: adang1345@gmail.com
 License: MIT
 Platform: Windows
 Classifier: License :: OSI Approved :: MIT License
@@ -96,8 +96,8 @@
 
 - `delvewheel` reads DLL file headers to determine which libraries a wheel depends on. DLLs that are loaded at runtime using `ctypes`/`cffi` (from Python) or `LoadLibrary` (from C/C++) will be missed. You can, however, specify additional DLLs to vendor into the wheel using the `--add-dll` option. If you elect to do this, it is your responsibility to ensure that the additional DLL is found at load time.
 - Wheels created using `delvewheel` are not guaranteed to work on systems older than Windows 7 SP1. If you intend to create a wheel for an old Windows system, you should test the resultant wheel thoroughly. If it turns out that getting the wheel to work on an older system simply requires an extra DLL, you can use the `--add-dll` flag to vendor additional DLLs into the wheel.
 - To avoid DLL hell, we mangle the file names of most DLLs that are vendored into the wheel. This way, a Python process that tries loading a vendored DLL does not end up using a different DLL with the same name. Due to a limitation in how name-mangling is performed, `delvewheel` is unable to name-mangle DLLs whose dependents contain insufficient internal padding to fit the mangled names and contain trailing data at the end of the binary. An exception will be raised if such a DLL is encountered. Commonly, trailing data consist of symbols that can be safely removed using the GNU `strip` utility, although there exist situations where the data must be present for the DLL to function properly. To remove the trailing data, execute `strip -s EXAMPLE.dll` or use the `--strip` flag. To keep the trailing data and skip name mangling, use the `--no-mangle` or `--no-mangle-all` flag.
 - Any DLL containing an Authenticode signature will have its signature cleared if its dependencies are name-mangled.
 - `delvewheel` cannot repair a wheel that contains extension modules targeting more than one CPU architecture (e.g. both `win32` and `win_amd64`). You should create a separate wheel for each CPU architecture and repair each individually.
 - `delvewheel` creates or patches `__init__.py` in each top-level package so that the DLLs are loaded properly during import. This will cause issues if you have a top-level namespace package that requires `__init__.py` to be absent to function properly.
-- Support for delay-load DLLs is limited. Delay-load DLLs are vendored into the wheel, but depending on the environment, errors may occur when they are loaded at runtime. If your project requires better support for delay-load DLLs, then file an issue.
+- If your project has a [delay-load DLL dependency](https://learn.microsoft.com/en-us/cpp/build/reference/linker-support-for-delay-loaded-dlls), you must use a custom delay-load import hook when building the DLL that has the delay-load dependency. This ensures that the directory containing the vendored DLLs is included in the DLL search path when delay-loading. For convenience, we provide a suitable hook for Microsoft Visual C/C++ at [delayload/delayhook.c](delayload/delayhook.c). Add the file to your C/C++ project when building your DLL.
```

### Comparing `delvewheel-1.3.6/README.md` & `delvewheel-1.3.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -68,8 +68,8 @@
 
 - `delvewheel` reads DLL file headers to determine which libraries a wheel depends on. DLLs that are loaded at runtime using `ctypes`/`cffi` (from Python) or `LoadLibrary` (from C/C++) will be missed. You can, however, specify additional DLLs to vendor into the wheel using the `--add-dll` option. If you elect to do this, it is your responsibility to ensure that the additional DLL is found at load time.
 - Wheels created using `delvewheel` are not guaranteed to work on systems older than Windows 7 SP1. If you intend to create a wheel for an old Windows system, you should test the resultant wheel thoroughly. If it turns out that getting the wheel to work on an older system simply requires an extra DLL, you can use the `--add-dll` flag to vendor additional DLLs into the wheel.
 - To avoid DLL hell, we mangle the file names of most DLLs that are vendored into the wheel. This way, a Python process that tries loading a vendored DLL does not end up using a different DLL with the same name. Due to a limitation in how name-mangling is performed, `delvewheel` is unable to name-mangle DLLs whose dependents contain insufficient internal padding to fit the mangled names and contain trailing data at the end of the binary. An exception will be raised if such a DLL is encountered. Commonly, trailing data consist of symbols that can be safely removed using the GNU `strip` utility, although there exist situations where the data must be present for the DLL to function properly. To remove the trailing data, execute `strip -s EXAMPLE.dll` or use the `--strip` flag. To keep the trailing data and skip name mangling, use the `--no-mangle` or `--no-mangle-all` flag.
 - Any DLL containing an Authenticode signature will have its signature cleared if its dependencies are name-mangled.
 - `delvewheel` cannot repair a wheel that contains extension modules targeting more than one CPU architecture (e.g. both `win32` and `win_amd64`). You should create a separate wheel for each CPU architecture and repair each individually.
 - `delvewheel` creates or patches `__init__.py` in each top-level package so that the DLLs are loaded properly during import. This will cause issues if you have a top-level namespace package that requires `__init__.py` to be absent to function properly.
-- Support for delay-load DLLs is limited. Delay-load DLLs are vendored into the wheel, but depending on the environment, errors may occur when they are loaded at runtime. If your project requires better support for delay-load DLLs, then file an issue.
+- If your project has a [delay-load DLL dependency](https://learn.microsoft.com/en-us/cpp/build/reference/linker-support-for-delay-loaded-dlls), you must use a custom delay-load import hook when building the DLL that has the delay-load dependency. This ensures that the directory containing the vendored DLLs is included in the DLL search path when delay-loading. For convenience, we provide a suitable hook for Microsoft Visual C/C++ at [delayload/delayhook.c](delayload/delayhook.c). Add the file to your C/C++ project when building your DLL.
```

### Comparing `delvewheel-1.3.6/delvewheel/__main__.py` & `delvewheel-1.3.7/delvewheel/__main__.py`

 * *Files identical despite different names*

### Comparing `delvewheel-1.3.6/delvewheel/_dll_list.py` & `delvewheel-1.3.7/delvewheel/_dll_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,14 +82,15 @@
     'cp39-win32': {'vcruntime140.dll'},
     'cp39-win_amd64': {'vcruntime140.dll', 'vcruntime140_1.dll'},
     'cp39-win_arm64': {'vcruntime140.dll', 'vcruntime140_1.dll'},
     'pypy39_pp73-win_amd64': {'vcruntime140.dll'},
     'cp310-win32': {'vcruntime140.dll'},
     'cp310-win_amd64': {'vcruntime140.dll', 'vcruntime140_1.dll'},
     'cp310-win_arm64': {'vcruntime140.dll', 'vcruntime140_1.dll'},
+    'pypy310_pp73-win_amd64': {'vcruntime140.dll'},
     'cp311-win32': {'vcruntime140.dll'},
     'cp311-win_amd64': {'vcruntime140.dll', 'vcruntime140_1.dll'},
     'cp311-win_arm64': {'vcruntime140.dll', 'vcruntime140_1.dll'},
     'cp312-win32': {'vcruntime140.dll'},
     'cp312-win_amd64': {'vcruntime140.dll', 'vcruntime140_1.dll'},
     'cp312-win_arm64': {'vcruntime140.dll', 'vcruntime140_1.dll'},
 }
```

### Comparing `delvewheel-1.3.6/delvewheel/_dll_utils.py` & `delvewheel-1.3.7/delvewheel/_dll_utils.py`

 * *Files identical despite different names*

### Comparing `delvewheel-1.3.6/delvewheel/_wheel_repair.py` & `delvewheel-1.3.7/delvewheel/_wheel_repair.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,28 +42,27 @@
 {0}# start delvewheel patch
 def _delvewheel_init_patch_{1}():
     import ctypes
     import os
     import platform
     import sys
     libs_dir = os.path.abspath(os.path.join(os.path.dirname(__file__), os.pardir, {2!r}))
-    is_pyinstaller = getattr(sys, 'frozen', False) and hasattr(sys, '_MEIPASS')
     is_conda_cpython = platform.python_implementation() == 'CPython' and (hasattr(ctypes.pythonapi, 'Anaconda_GetVersion') or 'packaged by conda-forge' in sys.version)
     if sys.version_info[:2] >= (3, 8) and not is_conda_cpython or sys.version_info[:2] >= (3, 10):
-        if not is_pyinstaller or os.path.isdir(libs_dir):
+        if os.path.isdir(libs_dir):
             os.add_dll_directory(libs_dir)
     else:
         load_order_filepath = os.path.join(libs_dir, {3!r})
-        if not is_pyinstaller or os.path.isfile(load_order_filepath):
+        if os.path.isfile(load_order_filepath):
             with open(os.path.join(libs_dir, {3!r})) as file:
                 load_order = file.read().split()
             for lib in load_order:
                 lib_path = os.path.join(os.path.join(libs_dir, lib))
-                if not is_pyinstaller or os.path.isfile(lib_path):
-                    ctypes.WinDLL(lib_path)
+                if os.path.isfile(lib_path) and not ctypes.windll.kernel32.LoadLibraryExW(ctypes.c_wchar_p(lib_path), None, 0x00000008):
+                    raise OSError('Error loading {{}}; {{}}'.format(lib, ctypes.FormatError()))
 
 
 _delvewheel_init_patch_{1}()
 del _delvewheel_init_patch_{1}
 # end delvewheel patch
 
 """
@@ -81,16 +80,15 @@
 _patch_init_template_v2 = """
 
 {0}# start delvewheel patch
 def _delvewheel_init_patch_{1}():
     import os
     import sys
     libs_dir = os.path.abspath(os.path.join(os.path.dirname(__file__), os.pardir, {2!r}))
-    is_pyinstaller = getattr(sys, 'frozen', False) and hasattr(sys, '_MEIPASS')
-    if not is_pyinstaller or os.path.isdir(libs_dir):
+    if os.path.isdir(libs_dir):
         os.add_dll_directory(libs_dir)
 
 
 _delvewheel_init_patch_{1}()
 del _delvewheel_init_patch_{1}
 # end delvewheel patch
 
@@ -622,68 +620,37 @@
                 lib_path = os.path.join(libs_dir, lib_name)
                 needed = _dll_utils.get_direct_mangleable_needed(lib_path, self._no_dlls, no_mangles, self._verbose)
                 _dll_utils.replace_needed(lib_path, needed, name_mangler, strip, self._verbose, self._test)
                 if lib_name.lower() in name_mangler:
                     os.rename(lib_path, os.path.join(libs_dir, name_mangler[lib_name.lower()]))
 
         if self._min_supported_python is None or self._min_supported_python < (3, 10):
-            # Perform topological sort to determine the order that DLLs must be
-            # loaded at runtime. We first construct a directed graph where the
-            # vertices are the vendored DLLs and an edge represents a "depends-
-            # on" relationship. We perform a topological sort of this graph.
-            # The reverse of this topological sort then tells us what order we
-            # need to load the DLLs so that all dependencies of a DLL are
-            # loaded before that DLL is loaded.
-            print('calculating DLL load order')
+            # Create .load-order file containing list of DLLs to load during
+            # import. Contrary to what the filename suggests, the DLLs are not
+            # listed in any particular order. In an older version of
+            # delvewheel, the DLLs needed to be listed in a particular order,
+            # and the old filename has been kept to maintain backward
+            # compatibility with re-bundling tools such as PyInstaller.
             for dependency_name in dependency_names.copy():
                 # dependency_name is NOT lowercased
                 if dependency_name.lower() in name_mangler:
                     dependency_names.remove(dependency_name)
                     dependency_names.add(name_mangler[dependency_name.lower()])
-
-            # map from lowercased DLL name to its original case
-            dependency_name_casemap = {dependency_name.lower(): dependency_name for dependency_name in dependency_names}
-
-            graph = {}  # map each lowercased DLL name to a lowercased set of its vendored direct dependencies
-            for dll_name in dependency_names:
-                # dll_name is NOT lowercased
-                dll_path = os.path.join(libs_dir, dll_name)
-                # In this context, delay-loaded DLL dependencies are not true
-                # dependencies because they are not necessary to get the DLL to
-                # load initially. More importantly, we may get circular
-                # dependencies if we were to consider delay-loaded DLLs as true
-                # dependencies. For example, there exist versions of
-                # concrt140.dll and msvcp140.dll such that concrt140.dll lists
-                # msvcp140.dll in its import table, while msvcp140.dll lists
-                # concrt140.dll in its delay import table.
-                graph[dll_name.lower()] = _dll_utils.get_direct_needed(dll_path, False, True, self._verbose) & set(dependency_name_casemap.keys())
-            rev_dll_load_order = []
-            no_incoming_edge = {dll_name_lower for dll_name_lower in dependency_name_casemap.keys() if not any(dll_name_lower in value for value in graph.values())}
-            while no_incoming_edge:
-                dll_name_lower = no_incoming_edge.pop()
-                rev_dll_load_order.append(dependency_name_casemap[dll_name_lower])
-                while graph[dll_name_lower]:
-                    dependent_dll_name = graph[dll_name_lower].pop()
-                    if not any(dependent_dll_name in value for value in graph.values()):
-                        no_incoming_edge.add(dependent_dll_name)
-            if any(graph.values()):
-                graph_leftover = {k: v for k, v in graph.items() if v}
-                raise RuntimeError(f'Dependent DLLs have a circular dependency: {graph_leftover}')
             # If the wheel contains a top-level extension module, then the
             # load-order file will be installed directly into site-packages. To
             # avoid conflicts with load-order files from other distributions,
             # include the distribution name and version in the load-order
             # filename. Do this regardless of whether the wheel actually
             # contains a top-level extension module.
             load_order_filename = f'.load-order-{self._distribution_name}-{self._version}'
             load_order_filepath = os.path.join(libs_dir, load_order_filename)
             if os.path.exists(load_order_filepath):
                 raise FileExistsError(f'{os.path.relpath(load_order_filepath, self._extract_dir)} already exists')
             with open(os.path.join(libs_dir, load_order_filename), 'w', newline='\n') as file:
-                file.write('\n'.join(reversed(rev_dll_load_order)))
+                file.write('\n'.join(dependency_names))
                 file.write('\n')
         else:
             load_order_filename = None
 
         # Create or patch top-level __init__.py in each package to load
         # dependent DLLs from correct location at runtime.
         #
```

### Comparing `delvewheel-1.3.6/delvewheel.egg-info/PKG-INFO` & `delvewheel-1.3.7/delvewheel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delvewheel
-Version: 1.3.6
+Version: 1.3.7
 Summary: Self-contained wheels for Windows
 Home-page: https://github.com/adang1345/delvewheel
 Author: Aohan Dang
 Author-email: adang1345@gmail.com
 License: MIT
 Platform: Windows
 Classifier: License :: OSI Approved :: MIT License
@@ -96,8 +96,8 @@
 
 - `delvewheel` reads DLL file headers to determine which libraries a wheel depends on. DLLs that are loaded at runtime using `ctypes`/`cffi` (from Python) or `LoadLibrary` (from C/C++) will be missed. You can, however, specify additional DLLs to vendor into the wheel using the `--add-dll` option. If you elect to do this, it is your responsibility to ensure that the additional DLL is found at load time.
 - Wheels created using `delvewheel` are not guaranteed to work on systems older than Windows 7 SP1. If you intend to create a wheel for an old Windows system, you should test the resultant wheel thoroughly. If it turns out that getting the wheel to work on an older system simply requires an extra DLL, you can use the `--add-dll` flag to vendor additional DLLs into the wheel.
 - To avoid DLL hell, we mangle the file names of most DLLs that are vendored into the wheel. This way, a Python process that tries loading a vendored DLL does not end up using a different DLL with the same name. Due to a limitation in how name-mangling is performed, `delvewheel` is unable to name-mangle DLLs whose dependents contain insufficient internal padding to fit the mangled names and contain trailing data at the end of the binary. An exception will be raised if such a DLL is encountered. Commonly, trailing data consist of symbols that can be safely removed using the GNU `strip` utility, although there exist situations where the data must be present for the DLL to function properly. To remove the trailing data, execute `strip -s EXAMPLE.dll` or use the `--strip` flag. To keep the trailing data and skip name mangling, use the `--no-mangle` or `--no-mangle-all` flag.
 - Any DLL containing an Authenticode signature will have its signature cleared if its dependencies are name-mangled.
 - `delvewheel` cannot repair a wheel that contains extension modules targeting more than one CPU architecture (e.g. both `win32` and `win_amd64`). You should create a separate wheel for each CPU architecture and repair each individually.
 - `delvewheel` creates or patches `__init__.py` in each top-level package so that the DLLs are loaded properly during import. This will cause issues if you have a top-level namespace package that requires `__init__.py` to be absent to function properly.
-- Support for delay-load DLLs is limited. Delay-load DLLs are vendored into the wheel, but depending on the environment, errors may occur when they are loaded at runtime. If your project requires better support for delay-load DLLs, then file an issue.
+- If your project has a [delay-load DLL dependency](https://learn.microsoft.com/en-us/cpp/build/reference/linker-support-for-delay-loaded-dlls), you must use a custom delay-load import hook when building the DLL that has the delay-load dependency. This ensures that the directory containing the vendored DLLs is included in the DLL search path when delay-loading. For convenience, we provide a suitable hook for Microsoft Visual C/C++ at [delayload/delayhook.c](delayload/delayhook.c). Add the file to your C/C++ project when building your DLL.
```

### Comparing `delvewheel-1.3.6/setup.cfg` & `delvewheel-1.3.7/setup.cfg`

 * *Files identical despite different names*

