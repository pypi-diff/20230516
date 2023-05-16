# Comparing `tmp/xgrid-0.0.2.tar.gz` & `tmp/xgrid-0.0.3.tar.gz`

## Comparing `xgrid-0.0.2.tar` & `xgrid-0.0.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 xgrid-0.0.2/requirements.txt
--rw-r--r--   0        0        0     9144 2020-02-02 00:00:00.000000 xgrid-0.0.2/test.py
--rw-r--r--   0        0        0     8574 2020-02-02 00:00:00.000000 xgrid-0.0.2/examples/cavity.py
--rw-r--r--   0        0        0   455424 2020-02-02 00:00:00.000000 xgrid-0.0.2/imgs/cavity.gif
--rw-r--r--   0        0        0   181643 2020-02-02 00:00:00.000000 xgrid-0.0.2/imgs/cavity.png
--rw-r--r--   0        0        0   181637 2020-02-02 00:00:00.000000 xgrid-0.0.2/imgs/cavityref.png
--rw-r--r--   0        0        0    18194 2020-02-02 00:00:00.000000 xgrid-0.0.2/imgs/convection_1d.png
--rw-r--r--   0        0        0    14277 2020-02-02 00:00:00.000000 xgrid-0.0.2/imgs/convection_1d_nonlinear.png
--rw-r--r--   0        0        0    12678 2020-02-02 00:00:00.000000 xgrid-0.0.2/imgs/convection_2d.png
--rw-r--r--   0        0        0    16467 2020-02-02 00:00:00.000000 xgrid-0.0.2/imgs/diffusion_1d.png
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 xgrid-0.0.2/xgrid/__init__.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 xgrid-0.0.2/xgrid/lang/__init__.py
--rw-r--r--   0        0        0    18300 2020-02-02 00:00:00.000000 xgrid-0.0.2/xgrid/lang/generator.py
--rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 xgrid-0.0.2/xgrid/lang/operator.py
--rw-r--r--   0        0        0    27541 2020-02-02 00:00:00.000000 xgrid-0.0.2/xgrid/lang/parser.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 xgrid-0.0.2/xgrid/lang/ir/__init__.py
--rw-r--r--   0        0        0     4498 2020-02-02 00:00:00.000000 xgrid-0.0.2/xgrid/lang/ir/expression.py
--rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 xgrid-0.0.2/xgrid/lang/ir/statement.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 xgrid-0.0.2/xgrid/lang/ir/visitor.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 xgrid-0.0.2/xgrid/util/__init__.py
--rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 xgrid-0.0.2/xgrid/util/console.py
--rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 xgrid-0.0.2/xgrid/util/ffi.py
--rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 xgrid-0.0.2/xgrid/util/init.py
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 xgrid-0.0.2/xgrid/util/logging.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 xgrid-0.0.2/xgrid/util/typing/__init__.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 xgrid-0.0.2/xgrid/util/typing/annotation.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 xgrid-0.0.2/xgrid/util/typing/reference.py
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 xgrid-0.0.2/xgrid/util/typing/value.py
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 xgrid-0.0.2/xgrid/xgrid/__init__.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 xgrid-0.0.2/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 xgrid-0.0.2/LICENSE
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 xgrid-0.0.2/README.md
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 xgrid-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 xgrid-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 xgrid-0.0.3/requirements.txt
+-rw-r--r--   0        0        0     9144 2020-02-02 00:00:00.000000 xgrid-0.0.3/test.py
+-rw-r--r--   0        0        0     8574 2020-02-02 00:00:00.000000 xgrid-0.0.3/examples/cavity.py
+-rw-r--r--   0        0        0   455424 2020-02-02 00:00:00.000000 xgrid-0.0.3/imgs/cavity.gif
+-rw-r--r--   0        0        0   181643 2020-02-02 00:00:00.000000 xgrid-0.0.3/imgs/cavity.png
+-rw-r--r--   0        0        0   181637 2020-02-02 00:00:00.000000 xgrid-0.0.3/imgs/cavityref.png
+-rw-r--r--   0        0        0    18194 2020-02-02 00:00:00.000000 xgrid-0.0.3/imgs/convection_1d.png
+-rw-r--r--   0        0        0    14277 2020-02-02 00:00:00.000000 xgrid-0.0.3/imgs/convection_1d_nonlinear.png
+-rw-r--r--   0        0        0    12678 2020-02-02 00:00:00.000000 xgrid-0.0.3/imgs/convection_2d.png
+-rw-r--r--   0        0        0    16467 2020-02-02 00:00:00.000000 xgrid-0.0.3/imgs/diffusion_1d.png
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 xgrid-0.0.3/xgrid/__init__.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 xgrid-0.0.3/xgrid/lang/__init__.py
+-rw-r--r--   0        0        0    18300 2020-02-02 00:00:00.000000 xgrid-0.0.3/xgrid/lang/generator.py
+-rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 xgrid-0.0.3/xgrid/lang/operator.py
+-rw-r--r--   0        0        0    27541 2020-02-02 00:00:00.000000 xgrid-0.0.3/xgrid/lang/parser.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 xgrid-0.0.3/xgrid/lang/ir/__init__.py
+-rw-r--r--   0        0        0     4498 2020-02-02 00:00:00.000000 xgrid-0.0.3/xgrid/lang/ir/expression.py
+-rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 xgrid-0.0.3/xgrid/lang/ir/statement.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 xgrid-0.0.3/xgrid/lang/ir/visitor.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 xgrid-0.0.3/xgrid/util/__init__.py
+-rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 xgrid-0.0.3/xgrid/util/console.py
+-rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 xgrid-0.0.3/xgrid/util/ffi.py
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 xgrid-0.0.3/xgrid/util/init.py
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 xgrid-0.0.3/xgrid/util/logging.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 xgrid-0.0.3/xgrid/util/typing/__init__.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 xgrid-0.0.3/xgrid/util/typing/annotation.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 xgrid-0.0.3/xgrid/util/typing/reference.py
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 xgrid-0.0.3/xgrid/util/typing/value.py
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 xgrid-0.0.3/xgrid/xgrid/__init__.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 xgrid-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 xgrid-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 xgrid-0.0.3/README.md
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 xgrid-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 xgrid-0.0.3/PKG-INFO
```

### Comparing `xgrid-0.0.2/requirements.txt` & `xgrid-0.0.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.2/test.py` & `xgrid-0.0.3/test.py`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.2/examples/cavity.py` & `xgrid-0.0.3/examples/cavity.py`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.2/imgs/cavity.gif` & `xgrid-0.0.3/imgs/cavity.gif`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.2/imgs/cavity.png` & `xgrid-0.0.3/imgs/cavity.png`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.2/imgs/cavityref.png` & `xgrid-0.0.3/imgs/cavityref.png`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.2/imgs/convection_1d.png` & `xgrid-0.0.3/imgs/convection_1d.png`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.2/imgs/convection_1d_nonlinear.png` & `xgrid-0.0.3/imgs/convection_1d_nonlinear.png`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.2/imgs/convection_2d.png` & `xgrid-0.0.3/imgs/convection_2d.png`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.2/imgs/diffusion_1d.png` & `xgrid-0.0.3/imgs/diffusion_1d.png`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.2/xgrid/__init__.py` & `xgrid-0.0.3/xgrid/__init__.py`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.2/xgrid/lang/generator.py` & `xgrid-0.0.3/xgrid/lang/generator.py`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.2/xgrid/lang/operator.py` & `xgrid-0.0.3/xgrid/lang/operator.py`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.2/xgrid/lang/parser.py` & `xgrid-0.0.3/xgrid/lang/parser.py`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.2/xgrid/lang/ir/__init__.py` & `xgrid-0.0.3/xgrid/lang/ir/__init__.py`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.2/xgrid/lang/ir/expression.py` & `xgrid-0.0.3/xgrid/lang/ir/expression.py`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.2/xgrid/lang/ir/statement.py` & `xgrid-0.0.3/xgrid/lang/ir/statement.py`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.2/xgrid/lang/ir/visitor.py` & `xgrid-0.0.3/xgrid/lang/ir/visitor.py`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.2/xgrid/util/console.py` & `xgrid-0.0.3/xgrid/util/console.py`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.2/xgrid/util/ffi.py` & `xgrid-0.0.3/xgrid/util/ffi.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         self.logger.info(
             f"compiler initialized with cacheroot = '{self.cacheroot}', cc = '{self.cc}'")
 
     def compile(self, source: str, cflags: Iterable[str] = []):
         args = [self.cc, "-shared"]
 
         if sys.platform != "win32":
-            args.append("-fpic")
+            args.extend(["-fpic", "-lm"])
 
         args.extend(cflags)
 
         source = f"// {' '.join(args)}\n" + source
 
         name = os.path.join(self.cacheroot, md5(
             source.encode()).hexdigest() + ".c")
```

### Comparing `xgrid-0.0.2/xgrid/util/init.py` & `xgrid-0.0.3/xgrid/util/init.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,16 +25,14 @@
         flags = []
 
         if self.parallel:
             flags.append("-fopenmp")
 
         flags.append(f"-O{self.opt_level}")
 
-        flags.append(f"-lm")
-
         return flags
 
     @property
     def fsize(self):
         return 4 if self.precision == "float" else 8
 
 
@@ -54,18 +52,15 @@
         logger.fail(
             f"Minimum Python 3.10 is required, current version is {sys.version_info}")
 
     if sys.platform == "win32":
         import shutil
 
         if not any(filter(shutil.which, cc)):
-            solutions = ["    1. LLVM (https://llvm.org/)",
-                         "    2. MinGW-w64 (https://www.mingw-w64.org/)",
-                         "    3. MSYS2 (https://www.msys2.org/)",
-                         "    4. Cygwin (https://www.cygwin.com/)"]
+            solutions = ["    LLVM (https://llvm.org/) + MSVC"]
             logger.fail(
                 f"Failed to find cc within {cc}, possible solutions are:", *solutions)
 
     _config = Configuration(parallel, cc, cacheroot,
                             comment, overstep, opt_level, precision)
 
     logger.info(f"initialized with configuration: {_config}")
```

### Comparing `xgrid-0.0.2/xgrid/util/logging.py` & `xgrid-0.0.3/xgrid/util/logging.py`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.2/xgrid/util/typing/annotation.py` & `xgrid-0.0.3/xgrid/util/typing/annotation.py`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.2/xgrid/util/typing/reference.py` & `xgrid-0.0.3/xgrid/util/typing/reference.py`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.2/xgrid/util/typing/value.py` & `xgrid-0.0.3/xgrid/util/typing/value.py`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.2/xgrid/xgrid/__init__.py` & `xgrid-0.0.3/xgrid/xgrid/__init__.py`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.2/LICENSE` & `xgrid-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.2/README.md` & `xgrid-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.2/pyproject.toml` & `xgrid-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "xgrid"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="yhl1219", email="yhliu2000@outlook.com" },
 ]
 description = "Domain-specific language for developing partial differential equation solvers"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `xgrid-0.0.2/PKG-INFO` & `xgrid-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xgrid
-Version: 0.0.2
+Version: 0.0.3
 Summary: Domain-specific language for developing partial differential equation solvers
 Project-URL: Homepage, https://github.com/yhl1219/xgrid
 Project-URL: Bug Tracker, https://github.com/yhl1219/xgrid/issues
 Author-email: yhl1219 <yhliu2000@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

