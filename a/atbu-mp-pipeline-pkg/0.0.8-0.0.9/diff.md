# Comparing `tmp/atbu-mp-pipeline-pkg-0.0.8.tar.gz` & `tmp/atbu-mp-pipeline-pkg-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atbu-mp-pipeline-pkg-0.0.8.tar", last modified: Fri Jul 29 22:07:13 2022, max compression
+gzip compressed data, was "atbu-mp-pipeline-pkg-0.0.9.tar", last modified: Tue May 16 05:32:46 2023, max compression
```

## Comparing `atbu-mp-pipeline-pkg-0.0.8.tar` & `atbu-mp-pipeline-pkg-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxrwx   0        0        0        0 2022-07-29 22:07:13.841163 atbu-mp-pipeline-pkg-0.0.8/
--rw-rw-rw-   0        0        0    11560 2022-06-01 12:51:37.000000 atbu-mp-pipeline-pkg-0.0.8/LICENSE
--rw-rw-rw-   0        0        0    15122 2022-07-29 22:07:13.840151 atbu-mp-pipeline-pkg-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0    14415 2022-06-12 01:08:10.000000 atbu-mp-pipeline-pkg-0.0.8/README.md
--rw-rw-rw-   0        0        0      110 2022-06-01 12:51:37.000000 atbu-mp-pipeline-pkg-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-07-29 22:07:13.841163 atbu-mp-pipeline-pkg-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1839 2022-07-29 21:09:22.000000 atbu-mp-pipeline-pkg-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-07-29 22:07:13.784824 atbu-mp-pipeline-pkg-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2022-07-29 22:07:13.783813 atbu-mp-pipeline-pkg-0.0.8/src/atbu/
-drwxrwxrwx   0        0        0        0 2022-07-29 22:07:13.809816 atbu-mp-pipeline-pkg-0.0.8/src/atbu/mp_pipeline/
--rw-rw-rw-   0        0        0        2 2022-06-01 12:51:37.000000 atbu-mp-pipeline-pkg-0.0.8/src/atbu/mp_pipeline/__init__.py
--rw-rw-rw-   0        0        0     3092 2022-06-10 00:39:13.000000 atbu-mp-pipeline-pkg-0.0.8/src/atbu/mp_pipeline/exception.py
--rw-rw-rw-   0        0        0    16356 2022-07-29 21:08:16.000000 atbu-mp-pipeline-pkg-0.0.8/src/atbu/mp_pipeline/mp_global.py
--rw-rw-rw-   0        0        0     1601 2022-06-21 02:49:51.000000 atbu-mp-pipeline-pkg-0.0.8/src/atbu/mp_pipeline/mp_helper.py
--rw-rw-rw-   0        0        0    58671 2022-06-13 10:25:25.000000 atbu-mp-pipeline-pkg-0.0.8/src/atbu/mp_pipeline/mp_pipeline.py
-drwxrwxrwx   0        0        0        0 2022-07-29 22:07:13.833846 atbu-mp-pipeline-pkg-0.0.8/src/atbu_mp_pipeline_pkg.egg-info/
--rw-rw-rw-   0        0        0    15122 2022-07-29 22:07:13.000000 atbu-mp-pipeline-pkg-0.0.8/src/atbu_mp_pipeline_pkg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      451 2022-07-29 22:07:13.000000 atbu-mp-pipeline-pkg-0.0.8/src/atbu_mp_pipeline_pkg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-29 22:07:13.000000 atbu-mp-pipeline-pkg-0.0.8/src/atbu_mp_pipeline_pkg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2022-07-29 22:07:13.000000 atbu-mp-pipeline-pkg-0.0.8/src/atbu_mp_pipeline_pkg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2022-07-29 22:07:13.000000 atbu-mp-pipeline-pkg-0.0.8/src/atbu_mp_pipeline_pkg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 05:32:46.192066 atbu-mp-pipeline-pkg-0.0.9/
+-rw-rw-rw-   0        0        0    11560 2022-06-01 12:51:37.000000 atbu-mp-pipeline-pkg-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0    15122 2023-05-16 05:32:46.192066 atbu-mp-pipeline-pkg-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    14415 2022-06-12 01:08:10.000000 atbu-mp-pipeline-pkg-0.0.9/README.md
+-rw-rw-rw-   0        0        0      110 2022-06-01 12:51:37.000000 atbu-mp-pipeline-pkg-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-16 05:32:46.193065 atbu-mp-pipeline-pkg-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1839 2023-05-16 05:30:11.000000 atbu-mp-pipeline-pkg-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 05:32:46.149067 atbu-mp-pipeline-pkg-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-05-16 05:32:46.149067 atbu-mp-pipeline-pkg-0.0.9/src/atbu/
+drwxrwxrwx   0        0        0        0 2023-05-16 05:32:46.162065 atbu-mp-pipeline-pkg-0.0.9/src/atbu/mp_pipeline/
+-rw-rw-rw-   0        0        0        2 2022-06-01 12:51:37.000000 atbu-mp-pipeline-pkg-0.0.9/src/atbu/mp_pipeline/__init__.py
+-rw-rw-rw-   0        0        0     3092 2022-06-10 00:39:13.000000 atbu-mp-pipeline-pkg-0.0.9/src/atbu/mp_pipeline/exception.py
+-rw-rw-rw-   0        0        0    16960 2022-10-11 23:13:15.000000 atbu-mp-pipeline-pkg-0.0.9/src/atbu/mp_pipeline/mp_global.py
+-rw-rw-rw-   0        0        0     1601 2022-06-21 02:49:51.000000 atbu-mp-pipeline-pkg-0.0.9/src/atbu/mp_pipeline/mp_helper.py
+-rw-rw-rw-   0        0        0    58671 2022-06-13 10:25:25.000000 atbu-mp-pipeline-pkg-0.0.9/src/atbu/mp_pipeline/mp_pipeline.py
+drwxrwxrwx   0        0        0        0 2023-05-16 05:32:46.186068 atbu-mp-pipeline-pkg-0.0.9/src/atbu_mp_pipeline_pkg.egg-info/
+-rw-rw-rw-   0        0        0    15122 2023-05-16 05:32:46.000000 atbu-mp-pipeline-pkg-0.0.9/src/atbu_mp_pipeline_pkg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      477 2023-05-16 05:32:46.000000 atbu-mp-pipeline-pkg-0.0.9/src/atbu_mp_pipeline_pkg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 05:32:46.000000 atbu-mp-pipeline-pkg-0.0.9/src/atbu_mp_pipeline_pkg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-05-16 05:32:46.000000 atbu-mp-pipeline-pkg-0.0.9/src/atbu_mp_pipeline_pkg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-16 05:32:46.000000 atbu-mp-pipeline-pkg-0.0.9/src/atbu_mp_pipeline_pkg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 05:32:46.187066 atbu-mp-pipeline-pkg-0.0.9/tests/
+-rw-rw-rw-   0        0        0    14045 2022-09-27 22:38:11.000000 atbu-mp-pipeline-pkg-0.0.9/tests/test_mp_pipeline.py
```

### Comparing `atbu-mp-pipeline-pkg-0.0.8/LICENSE` & `atbu-mp-pipeline-pkg-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `atbu-mp-pipeline-pkg-0.0.8/PKG-INFO` & `atbu-mp-pipeline-pkg-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atbu-mp-pipeline-pkg
-Version: 0.0.8
+Version: 0.0.9
 Summary: ATBU atbu.mp_pipeline package, a multiprocessing work item pipeline.
 Home-page: https://github.com/AshleyT3/atbu-mp-pipeline
 Author: Ashley R. Thomas
 Author-email: ashley.r.thomas.701@gmail.com
 Project-URL: Bug Tracker, https://github.com/AshleyT3/atbu-mp-pipeline/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `atbu-mp-pipeline-pkg-0.0.8/README.md` & `atbu-mp-pipeline-pkg-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `atbu-mp-pipeline-pkg-0.0.8/setup.py` & `atbu-mp-pipeline-pkg-0.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 # read the contents of your README file
 this_dir = Path(__file__).parent.absolute()
 readme_md_path = this_dir / "README.md"
 long_description = readme_md_path.read_text()
 
 setuptools.setup(
     name="atbu-mp-pipeline-pkg",
-    version="0.0.8",
+    version="0.0.9",
     author="Ashley R. Thomas",
     author_email="ashley.r.thomas.701@gmail.com",
     description= (
         "ATBU atbu.mp_pipeline package, a multiprocessing work item pipeline."
     ),
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `atbu-mp-pipeline-pkg-0.0.8/src/atbu/mp_pipeline/exception.py` & `atbu-mp-pipeline-pkg-0.0.9/src/atbu/mp_pipeline/exception.py`

 * *Files identical despite different names*

### Comparing `atbu-mp-pipeline-pkg-0.0.8/src/atbu/mp_pipeline/mp_global.py` & `atbu-mp-pipeline-pkg-0.0.9/src/atbu/mp_pipeline/mp_global.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 import threading
 from typing import Callable
 
 
 from atbu.common.exception import (
     QueueListenerNotStarted,
     QueueListenerAlreadyStarted,
+    InvalidStateError,
 )
 
 from .exception import (
     GlobalContextNotSet,
 )
 
 
@@ -69,15 +70,15 @@
             f"t_name={current_thread.getName()} cp.pid={current_process.pid} "
             f"c_p={str(current_process)} c_t={str(current_thread)}"
         )
 
 
 class _MultiprocessGlobalContext:
     """Initialize a global context instance.
-    
+
     MP global context. WARNING: Do not add any member
     variables that cannot be pickled, or generally avoid
     doing so if sharing is not needed.
 
     Args:
         logging_queue (:obj:`multiprocessing.Queue`): A multiprocessing
             shared process queue.
@@ -385,14 +386,15 @@
     ]
     for l in all_loggers:
         for h in l.handlers:
             if h in _CREATED_LOGGING_HANDLERS:
                 l.handlers.remove(h)
                 _untrack_logging_handler(h)
 
+_LAST_INITIALIZE_ARGS = None
 
 def initialize_logging(
     logfile,
     loglevel,
     verbosity_level,
     log_console_detail
 ):
@@ -419,14 +421,16 @@
             output.
 
     Raises:
         GlobalContextNotSet: The `global_init` or subprocess initialization
             function :func:`get_process_pool_exec_init_func` was not
             specified/called.
     """
+    global _LAST_INITIALIZE_ARGS
+    _LAST_INITIALIZE_ARGS = locals()
     if not _GLOBAL_CONTEXT:
         raise GlobalContextNotSet()
     file_log_level = logging.DEBUG
     console_log_level = logging.INFO
     _GLOBAL_CONTEXT.global_logging_level = logging.INFO
     _GLOBAL_CONTEXT.global_verbosity_level = 0
     if loglevel is not None:
@@ -474,14 +478,28 @@
 
     This is often called as part of process exit/cleanup.
     """
     _stop_global_queue_listener()
     remove_created_logging_handlers()
 
 
+def reinitialize_logging():
+    """Reinitialize logging after using switch_to_non_queued_logging().
+
+    Raises:
+        InvalidStateError: Raised if initialize_logging() has never been called.
+    """
+    if _LAST_INITIALIZE_ARGS is None:
+        raise InvalidStateError(
+            "The initialize_logging() function must be called at least once "
+            "before reinitialize_logging() can be used."
+        )
+    initialize_logging(**_LAST_INITIALIZE_ARGS)
+
+
 def initialize_logging_basic():
     """Setup basic logging without having to specify any detailed
     setup parameters.
 
     Command line arguments often specify the details of the type of
     logging/verbosity desired by a user. In such cases, this can be
     used early during app statrtup until such time as full logging
```

### Comparing `atbu-mp-pipeline-pkg-0.0.8/src/atbu/mp_pipeline/mp_helper.py` & `atbu-mp-pipeline-pkg-0.0.9/src/atbu/mp_pipeline/mp_helper.py`

 * *Files identical despite different names*

### Comparing `atbu-mp-pipeline-pkg-0.0.8/src/atbu/mp_pipeline/mp_pipeline.py` & `atbu-mp-pipeline-pkg-0.0.9/src/atbu/mp_pipeline/mp_pipeline.py`

 * *Files identical despite different names*

### Comparing `atbu-mp-pipeline-pkg-0.0.8/src/atbu_mp_pipeline_pkg.egg-info/PKG-INFO` & `atbu-mp-pipeline-pkg-0.0.9/src/atbu_mp_pipeline_pkg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atbu-mp-pipeline-pkg
-Version: 0.0.8
+Version: 0.0.9
 Summary: ATBU atbu.mp_pipeline package, a multiprocessing work item pipeline.
 Home-page: https://github.com/AshleyT3/atbu-mp-pipeline
 Author: Ashley R. Thomas
 Author-email: ashley.r.thomas.701@gmail.com
 Project-URL: Bug Tracker, https://github.com/AshleyT3/atbu-mp-pipeline/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

