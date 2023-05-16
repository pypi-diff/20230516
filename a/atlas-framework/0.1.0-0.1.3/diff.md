# Comparing `tmp/atlas-framework-0.1.0.tar.gz` & `tmp/atlas-framework-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlas-framework-0.1.0.tar", last modified: Mon Jan 30 18:37:24 2023, max compression
+gzip compressed data, was "atlas-framework-0.1.3.tar", last modified: Tue May 16 19:18:10 2023, max compression
```

## Comparing `atlas-framework-0.1.0.tar` & `atlas-framework-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,24 @@
-drwxr-xr-x   0 grantv     (501) staff       (20)        0 2023-01-30 18:37:24.890744 atlas-framework-0.1.0/
--rw-r--r--   0 grantv     (501) staff       (20)     1070 2023-01-30 18:34:34.000000 atlas-framework-0.1.0/LICENSE
--rw-r--r--   0 grantv     (501) staff       (20)     5287 2023-01-30 18:37:24.890401 atlas-framework-0.1.0/PKG-INFO
--rw-r--r--   0 grantv     (501) staff       (20)     4529 2023-01-30 18:29:52.000000 atlas-framework-0.1.0/README.md
-drwxr-xr-x   0 grantv     (501) staff       (20)        0 2023-01-30 18:37:24.885916 atlas-framework-0.1.0/atlas/
--rw-r--r--   0 grantv     (501) staff       (20)        0 2023-01-30 15:21:44.000000 atlas-framework-0.1.0/atlas/__init__.py
-drwxr-xr-x   0 grantv     (501) staff       (20)        0 2023-01-30 18:37:24.887337 atlas-framework-0.1.0/atlas/app/
--rw-r--r--   0 grantv     (501) staff       (20)     3034 2023-01-30 17:34:10.000000 atlas-framework-0.1.0/atlas/app/base.py
--rw-r--r--   0 grantv     (501) staff       (20)       60 2023-01-30 15:32:29.000000 atlas-framework-0.1.0/atlas/app/cli.py
--rw-r--r--   0 grantv     (501) staff       (20)       60 2023-01-30 15:32:43.000000 atlas-framework-0.1.0/atlas/app/gui.py
-drwxr-xr-x   0 grantv     (501) staff       (20)        0 2023-01-30 18:37:24.888129 atlas-framework-0.1.0/atlas/context/
--rw-r--r--   0 grantv     (501) staff       (20)     1913 2023-01-30 17:31:02.000000 atlas-framework-0.1.0/atlas/context/__init__.py
-drwxr-xr-x   0 grantv     (501) staff       (20)        0 2023-01-30 18:37:24.890025 atlas-framework-0.1.0/atlas_framework.egg-info/
--rw-r--r--   0 grantv     (501) staff       (20)     5287 2023-01-30 18:37:24.000000 atlas-framework-0.1.0/atlas_framework.egg-info/PKG-INFO
--rw-r--r--   0 grantv     (501) staff       (20)      322 2023-01-30 18:37:24.000000 atlas-framework-0.1.0/atlas_framework.egg-info/SOURCES.txt
--rw-r--r--   0 grantv     (501) staff       (20)        1 2023-01-30 18:37:24.000000 atlas-framework-0.1.0/atlas_framework.egg-info/dependency_links.txt
--rw-r--r--   0 grantv     (501) staff       (20)       98 2023-01-30 18:37:24.000000 atlas-framework-0.1.0/atlas_framework.egg-info/requires.txt
--rw-r--r--   0 grantv     (501) staff       (20)        6 2023-01-30 18:37:24.000000 atlas-framework-0.1.0/atlas_framework.egg-info/top_level.txt
--rw-r--r--   0 grantv     (501) staff       (20)     1054 2023-01-30 18:36:59.000000 atlas-framework-0.1.0/pyproject.toml
--rw-r--r--   0 grantv     (501) staff       (20)       38 2023-01-30 18:37:24.890852 atlas-framework-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:18:10.587477 atlas-framework-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-16 19:17:57.000000 atlas-framework-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-05-16 19:18:10.587477 atlas-framework-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-05-16 19:17:57.000000 atlas-framework-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-16 19:17:57.000000 atlas-framework-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 19:18:10.587477 atlas-framework-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:18:10.583477 atlas-framework-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:18:10.587477 atlas-framework-0.1.3/src/atlas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 19:17:57.000000 atlas-framework-0.1.3/src/atlas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:18:10.587477 atlas-framework-0.1.3/src/atlas/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-16 19:17:57.000000 atlas-framework-0.1.3/src/atlas/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-16 19:17:57.000000 atlas-framework-0.1.3/src/atlas/app/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-05-16 19:17:57.000000 atlas-framework-0.1.3/src/atlas/app/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:18:10.587477 atlas-framework-0.1.3/src/atlas/context/
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-16 19:17:57.000000 atlas-framework-0.1.3/src/atlas/context/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:18:10.587477 atlas-framework-0.1.3/src/atlas_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-05-16 19:18:10.000000 atlas-framework-0.1.3/src/atlas_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-16 19:18:10.000000 atlas-framework-0.1.3/src/atlas_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 19:18:10.000000 atlas-framework-0.1.3/src/atlas_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-16 19:18:10.000000 atlas-framework-0.1.3/src/atlas_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-16 19:18:10.000000 atlas-framework-0.1.3/src/atlas_framework.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:18:10.587477 atlas-framework-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-16 19:17:57.000000 atlas-framework-0.1.3/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-16 19:17:57.000000 atlas-framework-0.1.3/tests/test_context.py
```

### Comparing `atlas-framework-0.1.0/LICENSE` & `atlas-framework-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `atlas-framework-0.1.0/PKG-INFO` & `atlas-framework-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 Metadata-Version: 2.1
 Name: atlas-framework
-Version: 0.1.0
+Version: 0.1.3
 Summary: Class-based famework for quickly creating robust Python apps.
 Author-email: Grant Viklund <renderbox@gmail.com>
 Project-URL: Homepage, https://github.com/renderbox/atlas-framework
 Project-URL: Bug Tracker, https://github.com/renderbox/atlas-framework/issues
 Keywords: cli,app,application,framework
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: <3.12,>=3.9
+Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 Provides-Extra: docs
+Provides-Extra: pyside2
 License-File: LICENSE
 
 # Atlas App Framework
 
 This is a simple framework for creating Class based applications that can be run as a command line application or importated and run as a module. It's goal is to remove a lot of boiler plate that is typically done when writting CLI and GUI apps.
 
 ## Example
 
+You can run our sample app by checking out the repo, installing the packages and then using the following command line below. It's reconmended that you use a virtual environment and not install packages globally.
+
+```bash
+> python tests/sample_gui.py
+```
+
 Here is a simple CLI app to show how this all works.
 
 ```python
 from atlas.app.cli import CLIApp
 
 
 class SampleApp(CLIApp):
```

### Comparing `atlas-framework-0.1.0/README.md` & `atlas-framework-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # Atlas App Framework
 
 This is a simple framework for creating Class based applications that can be run as a command line application or importated and run as a module. It's goal is to remove a lot of boiler plate that is typically done when writting CLI and GUI apps.
 
 ## Example
 
+You can run our sample app by checking out the repo, installing the packages and then using the following command line below. It's reconmended that you use a virtual environment and not install packages globally.
+
+```bash
+> python tests/sample_gui.py
+```
+
 Here is a simple CLI app to show how this all works.
 
 ```python
 from atlas.app.cli import CLIApp
 
 
 class SampleApp(CLIApp):
```

### Comparing `atlas-framework-0.1.0/atlas/app/base.py` & `atlas-framework-0.1.3/src/atlas/app/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,16 @@
-from atlas.context import Context, camel_case_spaced
 import argparse
+from atlas.context import Context, camel_case_spaced
 
 
 class AppBase:
+    """
+    This is the development level base class and should not be subclassed directly.
+    Use the App Class one level above.
+    """
 
     ctx = None
     argparser = None
     description = "No Description set for this application"
     app_name = None  # Human Friendly Name like "App Base", default is class name
     epilog = None
     context_class = Context
@@ -36,29 +40,37 @@
 
     def add_argument(self, *args, **kwargs):
         """A wrapper around the arg parser to allow updates without breaking users code."""
         self.argparser.add_argument(*args, **kwargs)
 
     def parse_args(self):
         """parse args based on the input"""
-        return vars(self.argparser.parse_args())
+        parsed, extra_args = self.argparser.parse_known_args()
+        try:
+            self.arg_dict = vars(
+                parsed
+            )  # This can fail with unrecognized arguments in the app
+        except TypeError:
+            self.arg_dict = {}
+        return self.arg_dict
 
     # Create and set the Context object
     def set_context(self, ctx):
         """
         Set Context will set the context to one passed in or will generate one.  One is provided only if it is
         pre-generated somewhere else and passed in, like in the case of chaining App instances.
 
         Args:
             ctx (Context): Context Class or None
 
         Returns:
             Context: Instance of the Context Class
         """
-        self.ctx = ctx if ctx else self.context_class(args=self.parse_args())
+        args = self.parse_args()  # TODO: Handle extra args
+        self.ctx = ctx if ctx else self.context_class(args=args)
         return self.ctx
 
     def __call__(self, ctx=None):
         """
         This is the entry point to run the app.  It should not be overridden, and instead, just override the run()
         method.
 
@@ -81,19 +93,20 @@
         Returns:
             Context: The expected return context object.
         """
         return ctx
 
     def post(self):
         """
-        Called after the main run() method for any necessary cleanup or final steps.  This an entry point for a Mix-In Class.
+        Called after the main run() method for any necessary cleanup or final steps.  This an entry point for a Mix-In
+        Class.
         """
         pass
 
     def run(self, ctx):
         """Place where business logic is added in a subclassed app.
 
         Args:
             ctx (Context): Context Object to work with.
         """
         print("I do nothing yet except print my context.")
-        print(self.ctx)
+        print(ctx)
```

### Comparing `atlas-framework-0.1.0/atlas/context/__init__.py` & `atlas-framework-0.1.3/src/atlas/context/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,18 +24,19 @@
     multiple App classes.
     """
 
     # By default all keys will be reduced to lower_snake_case
     key_renamer = lower_snake_case
     config_parser = None
     include_env = True
+    gui_mode = False
 
-    def __init__(self, args=None, config=None, *pargs, **kwargs):
+    def __init__(self, *pargs, args=None, config=None, **kwargs):
         super().__init__(*pargs, **kwargs)
-        print("Generating Context")
+        # print("Generating Context")
         self.parse_config(config)
         self.parse_env()
         self.parse_args(args)
 
     def parse_config(self, config):
         """
         Provides a check to handle case where there is no parser set.
@@ -56,9 +57,9 @@
     def parse_args(self, args):
         self.args = args
         if self.args:
             self.update_context(**self.args)
 
     def update_context(self, **kwargs):
         """Updates the context with values and renames the key."""
-        for key in kwargs:
-            self[self.key_renamer(key)] = kwargs[key]
+        for key, value in kwargs.items():
+            self[self.key_renamer(key)] = value
```

### Comparing `atlas-framework-0.1.0/atlas_framework.egg-info/PKG-INFO` & `atlas-framework-0.1.3/src/atlas_framework.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 Metadata-Version: 2.1
 Name: atlas-framework
-Version: 0.1.0
+Version: 0.1.3
 Summary: Class-based famework for quickly creating robust Python apps.
 Author-email: Grant Viklund <renderbox@gmail.com>
 Project-URL: Homepage, https://github.com/renderbox/atlas-framework
 Project-URL: Bug Tracker, https://github.com/renderbox/atlas-framework/issues
 Keywords: cli,app,application,framework
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: <3.12,>=3.9
+Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 Provides-Extra: docs
+Provides-Extra: pyside2
 License-File: LICENSE
 
 # Atlas App Framework
 
 This is a simple framework for creating Class based applications that can be run as a command line application or importated and run as a module. It's goal is to remove a lot of boiler plate that is typically done when writting CLI and GUI apps.
 
 ## Example
 
+You can run our sample app by checking out the repo, installing the packages and then using the following command line below. It's reconmended that you use a virtual environment and not install packages globally.
+
+```bash
+> python tests/sample_gui.py
+```
+
 Here is a simple CLI app to show how this all works.
 
 ```python
 from atlas.app.cli import CLIApp
 
 
 class SampleApp(CLIApp):
```

### Comparing `atlas-framework-0.1.0/pyproject.toml` & `atlas-framework-0.1.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 build-backend = "setuptools.build_meta"
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 [project]
 name = "atlas-framework"
-version = "0.1.0"
+version = "0.1.3"
 authors = [
   { name="Grant Viklund", email="renderbox@gmail.com" },
 ]
 description = "Class-based famework for quickly creating robust Python apps."
 readme = "README.md"
-requires-python = ">=3.9,<3.12"
+requires-python = ">=3.8,<3.12"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
@@ -27,20 +27,48 @@
 
 [project.optional-dependencies]
 dev = [
     "ipython",
     "black",
     "flake8",
     "flake8-black",
+    "flake8-pyproject",
     "mypy",
     "bandit",
     "isort",
     "toml",
 ]
-test = ["coverage"]
+test = [
+    "coverage",
+    "pytest"
+]
 docs = [
-    'coverage',
+    "coverage",
+]
+pyside2 = [
+    "PySide2",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/renderbox/atlas-framework"
 "Bug Tracker" = "https://github.com/renderbox/atlas-framework/issues"
+
+# [tool.black]
+
+[tool.flake8]
+ignore = ['E231', 'E241']
+max-line-length = 120
+
+[tool.coverage.run]
+source = ["src"]
+
+[tool.pylint]
+max-line-length = 120
+disable = [
+    "C0103", # (invalid-name)
+    "C0114", # (missing-module-docstring)
+    "C0115", # (missing-class-docstring)
+    "C0116", # (missing-function-docstring)
+    "R0903", # (too-few-public-methods)
+    "R0913", # (too-many-arguments)
+    "W0105", # (pointless-string-statement)
+]
```

