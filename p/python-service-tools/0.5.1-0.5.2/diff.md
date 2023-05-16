# Comparing `tmp/python-service-tools-0.5.1.tar.gz` & `tmp/python_service_tools-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-service-tools-0.5.1.tar", max compression
+gzip compressed data, was "python_service_tools-0.5.2.tar", max compression
```

## Comparing `python-service-tools-0.5.1.tar` & `python_service_tools-0.5.2.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0    11343 2022-05-02 13:19:59.599989 python-service-tools-0.5.1/LICENSE
--rw-r--r--   0        0        0     3976 2022-05-02 13:19:59.599989 python-service-tools-0.5.1/README.md
--rw-r--r--   0        0        0     1179 2022-05-02 13:19:59.603989 python-service-tools-0.5.1/pyproject.toml
--rw-r--r--   0        0        0        0 2022-05-02 13:19:59.603989 python-service-tools-0.5.1/src/servicetools/__init__.py
--rw-r--r--   0        0        0     1793 2022-05-02 13:19:59.603989 python-service-tools-0.5.1/src/servicetools/lazyactor.py
--rw-r--r--   0        0        0     4653 2022-05-02 13:19:59.603989 python-service-tools-0.5.1/src/servicetools/logging_config.py
--rw-r--r--   0        0        0     4016 2022-05-02 13:19:59.603989 python-service-tools-0.5.1/src/servicetools/middleware.py
--rw-r--r--   0        0        0      644 2022-05-02 13:19:59.603989 python-service-tools-0.5.1/src/servicetools/testing.py
--rw-r--r--   0        0        0     1168 2022-05-02 13:19:59.603989 python-service-tools-0.5.1/src/servicetools/timer.py
--rw-r--r--   0        0        0     4978 2022-05-02 13:23:18.217104 python-service-tools-0.5.1/setup.py
--rw-r--r--   0        0        0     4890 2022-05-02 13:23:18.217483 python-service-tools-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    11343 2023-05-16 19:48:39.599733 python_service_tools-0.5.2/LICENSE
+-rw-r--r--   0        0        0     3976 2023-05-16 19:48:39.599733 python_service_tools-0.5.2/README.md
+-rw-r--r--   0        0        0     1239 2023-05-16 19:48:39.603733 python_service_tools-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-16 19:48:39.603733 python_service_tools-0.5.2/src/servicetools/__init__.py
+-rw-r--r--   0        0        0     1793 2023-05-16 19:48:39.603733 python_service_tools-0.5.2/src/servicetools/lazyactor.py
+-rw-r--r--   0        0        0     5458 2023-05-16 19:48:39.603733 python_service_tools-0.5.2/src/servicetools/logging_config.py
+-rw-r--r--   0        0        0     4026 2023-05-16 19:48:39.603733 python_service_tools-0.5.2/src/servicetools/middleware.py
+-rw-r--r--   0        0        0      644 2023-05-16 19:48:39.603733 python_service_tools-0.5.2/src/servicetools/testing.py
+-rw-r--r--   0        0        0     1168 2023-05-16 19:48:39.603733 python_service_tools-0.5.2/src/servicetools/timer.py
+-rw-r--r--   0        0        0     4983 1970-01-01 00:00:00.000000 python_service_tools-0.5.2/PKG-INFO
```

### Comparing `python-service-tools-0.5.1/LICENSE` & `python_service_tools-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-service-tools-0.5.1/README.md` & `python_service_tools-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `python-service-tools-0.5.1/pyproject.toml` & `python_service_tools-0.5.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = 'python-service-tools'
-version = '0.5.1'
+version = '0.5.2'
 description = "Utilities for working with python services."
 authors = [
     "Alexander Costas <alexander.costas@mongodb.com>",
     "David Bradford <david.bradford@mongodb.com",
 ]
 license = "Apache-2.0"
 readme = "README.md"
@@ -16,25 +16,28 @@
 [tool.poetry.dependencies]
 python = "^3.7"
 python-json-logger = ">=0.1"
 structlog = ">=19"
 starlette = ">=0.13"
 dramatiq = {extras = ["rabbitmq", "watch"], version = ">=1.10"}
 pika = ">=1.2"
+typed-ast = "^1.5.4"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6"
-pytest-flake8 = "^1.0"
-black = "^20.8b1"
+pytest-flake8 = "<6.0"
+flake8 = "<5.0.0"
+black = "^22.3.0"
 pytest-black = "^0.3"
 pytest-mypy = "^0.7"
-mypy = "^0.782"
+mypy = "^1.2.0"
 pytest-cov = "^2.10"
 pytest-asyncio = "^0.14"
 pytest-pydocstyle = "^2.2"
+pydocstyle = "6.1.1"
 
 [tool.pytest.ini_options]
 addopts = "--flake8 --black --pydocstyle --mypy --cov=servicetools --cov-fail-under=90 --cov-branch --cov-report=term-missing"
 flake8-ignore = "W605 W503 W291 E203 E501 F821"
 
 [tool.black]
 line-length = 100
```

### Comparing `python-service-tools-0.5.1/src/servicetools/lazyactor.py` & `python_service_tools-0.5.2/src/servicetools/lazyactor.py`

 * *Files identical despite different names*

### Comparing `python-service-tools-0.5.1/src/servicetools/logging_config.py` & `python_service_tools-0.5.2/src/servicetools/logging_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-"""Default logging configuration for struclog."""
+"""Default logging configuration for structlog."""
 
 from enum import IntEnum, Enum, auto
 import logging
 import logging.config
 import sys
-from typing import Any, Dict, Iterable, Optional
+import threading
+from types import TracebackType
+from typing import Any, Dict, Iterable, Optional, Type
+from _thread import _ExceptHookArgs as ExceptHookArgs
 
 import structlog
 
 TEXT_LOG_FORMAT = "[%(levelname)s %(filename)s:%(funcName)s:%(lineno)s] %(message)s"
 VERBOSE_LEVELS = [logging.WARNING, logging.INFO, logging.DEBUG]
 
 
@@ -33,14 +36,33 @@
 
         :return: logging level.
         """
         v = self.value
         return VERBOSE_LEVELS[v] if v < len(VERBOSE_LEVELS) else VERBOSE_LEVELS[-1]
 
 
+def _log_uncaught_thread_exceptions(args: ExceptHookArgs) -> None:
+    """Handle logging uncaught exceptions in threads."""
+    _log_uncaught_exceptions(args.exc_type, args.exc_value, args.exc_traceback)
+
+
+def _log_uncaught_exceptions(
+    exception_class: Type[BaseException],
+    exception: Optional[BaseException] = None,
+    trace: Optional[TracebackType] = None,
+) -> None:
+    """Handle logging uncaught exceptions."""
+    log = structlog.get_logger()
+
+    log.critical(
+        "Uncaught exception",
+        exc_info=(exception_class, exception, trace),
+    )
+
+
 def default_logging(
     verbosity: int,
     log_format: LogFormat = LogFormat.TEXT,
     external_logs: Optional[Iterable[str]] = None,
     loggers_to_configure: Optional[Iterable[str]] = None,
 ) -> None:
     """
@@ -109,18 +131,22 @@
     # Unless the user specifies higher verbosity than we have levels, turn down the log level
     # for external libraries.
     if external_logs and verbosity < Verbosity.MAX:
         # Turn down logging for modules outside this project.
         for logger in external_logs:
             logging.getLogger(logger).setLevel(logging.WARNING)
 
+    # Log exceptions
+    sys.excepthook = _log_uncaught_exceptions
+    threading.excepthook = _log_uncaught_thread_exceptions
+
 
 def build_loggers_dictionary(
     loggers: Optional[Iterable[str]], logger_config: Dict[str, Any]
-) -> Dict[str, Dict]:
+) -> Dict[str, Any]:
     """
     Build a dictionary of loggers to configure.
 
     This will automatically include a default logger under `""`.
 
     :param loggers: List of log names to include in dictionary.
     :param logger_config: Configuration to use for logging.
```

### Comparing `python-service-tools-0.5.1/src/servicetools/middleware.py` & `python_service_tools-0.5.2/src/servicetools/middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     codes to ignore can be provided to not log certain error codes (for example,
     ignore all 404 errors).
     """
 
     def __init__(
         self,
         app: ASGIApp,
-        dispatch: DispatchFunction = None,
+        dispatch: Optional[DispatchFunction] = None,
         logger: Any = LOGGER,
         log_level: int = logging.INFO,
         ignored_status_codes: Optional[Set[int]] = None,
         include_request_in_failed_requests: Optional[bool] = False,
     ) -> None:
         """
         Create structlog request middleware.
```

### Comparing `python-service-tools-0.5.1/src/servicetools/testing.py` & `python_service_tools-0.5.2/src/servicetools/testing.py`

 * *Files identical despite different names*

### Comparing `python-service-tools-0.5.1/src/servicetools/timer.py` & `python_service_tools-0.5.2/src/servicetools/timer.py`

 * *Files identical despite different names*

### Comparing `python-service-tools-0.5.1/PKG-INFO` & `python_service_tools-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: python-service-tools
-Version: 0.5.1
+Version: 0.5.2
 Summary: Utilities for working with python services.
 Home-page: https://github.com/mongodb-labs/python-service-tools
 License: Apache-2.0
 Author: Alexander Costas
 Author-email: alexander.costas@mongodb.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dramatiq[rabbitmq,watch] (>=1.10)
 Requires-Dist: pika (>=1.2)
 Requires-Dist: python-json-logger (>=0.1)
 Requires-Dist: starlette (>=0.13)
 Requires-Dist: structlog (>=19)
+Requires-Dist: typed-ast (>=1.5.4,<2.0.0)
 Project-URL: Repository, https://github.com/mongodb-labs/python-service-tools
 Description-Content-Type: text/markdown
 
 # python-service-tools
 
 Utilities for working with python services.
```

