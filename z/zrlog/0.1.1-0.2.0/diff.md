# Comparing `tmp/zrlog-0.1.1.tar.gz` & `tmp/zrlog-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\repo-work\zirconium_logs\dist\tmpeof53mg6\zrlog-0.1.1.tar", last modified: Mon Jul  4 18:09:17 2022, max compression
+gzip compressed data, was "zrlog-0.2.0.tar", last modified: Tue May 16 14:03:35 2023, max compression
```

## Comparing `zrlog-0.1.1.tar` & `zrlog-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-07-04 18:09:17.020395 zrlog-0.1.1/
--rw-rw-rw-   0        0        0     1069 2022-06-30 16:51:47.000000 zrlog-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     3851 2022-07-04 18:09:17.020395 zrlog-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3294 2022-07-04 18:07:34.000000 zrlog-0.1.1/README.md
--rw-rw-rw-   0        0        0       88 2022-06-30 17:15:44.000000 zrlog-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0      763 2022-07-04 18:09:17.022387 zrlog-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-07-04 18:09:16.985984 zrlog-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2022-07-04 18:09:17.010357 zrlog-0.1.1/src/zrlog/
--rw-rw-rw-   0        0        0       57 2022-07-04 18:00:26.000000 zrlog-0.1.1/src/zrlog/__init__.py
--rw-rw-rw-   0        0        0      969 2022-07-04 17:23:43.000000 zrlog-0.1.1/src/zrlog/logger.py
--rw-rw-rw-   0        0        0     4626 2022-07-04 18:06:41.000000 zrlog-0.1.1/src/zrlog/logs.py
-drwxrwxrwx   0        0        0        0 2022-07-04 18:09:17.018394 zrlog-0.1.1/src/zrlog.egg-info/
--rw-rw-rw-   0        0        0     3851 2022-07-04 18:09:16.000000 zrlog-0.1.1/src/zrlog.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2022-07-04 18:09:16.000000 zrlog-0.1.1/src/zrlog.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-04 18:09:16.000000 zrlog-0.1.1/src/zrlog.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2022-07-04 18:09:16.000000 zrlog-0.1.1/src/zrlog.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-07-04 18:09:16.000000 zrlog-0.1.1/src/zrlog.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 14:03:35.411049 zrlog-0.2.0/
+-rw-rw-rw-   0        0        0     1069 2023-05-16 13:38:24.000000 zrlog-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     5167 2023-05-16 14:03:35.411049 zrlog-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4608 2023-05-16 14:01:40.000000 zrlog-0.2.0/README.md
+-rw-rw-rw-   0        0        0       88 2023-05-16 13:38:24.000000 zrlog-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0      763 2023-05-16 14:03:35.413049 zrlog-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-16 14:03:35.395049 zrlog-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-16 14:03:35.404049 zrlog-0.2.0/src/zrlog/
+-rw-rw-rw-   0        0        0       57 2023-05-16 13:45:41.000000 zrlog-0.2.0/src/zrlog/__init__.py
+-rw-rw-rw-   0        0        0      969 2023-05-16 13:38:24.000000 zrlog-0.2.0/src/zrlog/logger.py
+-rw-rw-rw-   0        0        0     4710 2023-05-16 14:00:09.000000 zrlog-0.2.0/src/zrlog/logs.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:03:35.410049 zrlog-0.2.0/src/zrlog.egg-info/
+-rw-rw-rw-   0        0        0     5167 2023-05-16 14:03:35.000000 zrlog-0.2.0/src/zrlog.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-05-16 14:03:35.000000 zrlog-0.2.0/src/zrlog.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 14:03:35.000000 zrlog-0.2.0/src/zrlog.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-05-16 14:03:35.000000 zrlog-0.2.0/src/zrlog.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-16 14:03:35.000000 zrlog-0.2.0/src/zrlog.egg-info/top_level.txt
```

### Comparing `zrlog-0.1.1/LICENSE` & `zrlog-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zrlog-0.1.1/PKG-INFO` & `zrlog-0.2.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,108 +1,133 @@
-Metadata-Version: 2.1
-Name: zrlog
-Version: 0.1.1
-Summary: Logging with Zirconium-based configuration and supports audit logging
-Home-page: https://github.com/turnbullerin/zrlog
-Author: Erin Turnbull
-Author-email: erin.a.turnbull@gmail.com
-Project-URL: Bug Tracker, https://github.com/turnbullerin/zrlog/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Zirconium Logging (ZrLog)
 This package adds logging support using the Zirconium configuration tool and TOML, with an extension for supporting
 logging audit events.
 
 
 ## Defining Logging Parameters
 Configuration for the logging module can be added in TOML under the `logging` key. The entries correspond to those 
 supported by `logging.config.dictConfig()` with a few additions to support audit logging. For example:
 
-    # .logging.toml (or your own app configuration file that you've registered) 
-    [logging]
-    version = 1
-
-    [logging.root]
-    level = "INFO"
-    handlers = ["console"]
-
-    [logging.handlers.console]
-    class = "logging.StreamHandler"
-    formatter = "brief"
-    level = "WARNING"
-    stream = "ext://sys.stdout"
-
-    [logging.formatters.brief]
-    format = "%(message)s [%(levelname)s]"
-
+```toml 
+# .logging.toml (or your own app configuration file that you've registered) 
+[logging]
+version = 1
+
+[logging.root]
+level = "INFO"
+handlers = ["console"]
+
+[logging.handlers.console]
+class = "logging.StreamHandler"
+formatter = "brief"
+level = "WARNING"
+stream = "ext://sys.stdout"
+
+[logging.formatters.brief]
+format = "%(message)s [%(levelname)s]"
+```
 
 Of note, if you want to change a specific logger (which often have dots in the name), you must quote the key:
 
-    [logging.loggers."module.foo.bar"]
-    level = "WARNING"
-
+```toml 
+[logging.loggers."module.foo.bar"]
+level = "WARNING"
+```
 
 ## Setting up logging
 
 Logging can be initialized at the appropriate place in your code. This should be AFTER you have registered all your
 configuration with Zirconium but before you want to do any logging.
 
-    import zrlog
-    zrlog.init_logging()
+```python 
+import zrlog
+zrlog.init_logging()
+```
+
+For test cases, configuration is often not done until the test case level, but you can use the `no_config` parameter
+to tell ZrLog to ignore the configuration.
+
+```python
+import zrlog
+zrlog.init_logging(no_config=True)
+```
 
 
 ## Additional Logging Levels
 This package adds three additional levels of logging:
 
-- audit(), which is intended to be used only with the Python auditing system as described below. The logging level is 
+- `audit()`, which is intended to be used only with the Python auditing system as described below. The logging level is 
   set to 1.
-- trace(), which is intended to be even more detailed than debug(). The logging level is set to 5.
-- out(), which is ranked between INFO and WARNING and is intended to be used to log user output for command-line 
-  applications. The logging level is set to 25.
+- `trace()`, which is intended to be even more detailed than debug(). The logging level is set to 5.
+- `out()`, which is ranked between INFO and WARNING and is intended to be used to log user output for command-line 
+  applications or key events that need to be tracked for auditing purposes. The logging level is set to 25.
+
+These are configured as methods on the `getLogger()` class as well as on `logging` itself for the root logger. Putting
+these together with existing levels, we recommend the following usages:
+
+| Level | Meaning |
+| --- | --- |
+| critical | An error so severe has occurred that the system may now crash. |
+| error | An error has occurred and something that was expected to happen did not happen. |
+| warning | Something unexpected happen or a problem may occur in the future. |
+| out | Something expected has happened that needs to be tracked in a production environment (e.g. user login). |
+| info | Something expected has happened that does not need tracking but can be useful to confirm normal operation. |
+| debug | Additional detail for debugging an issue |
+| trace | Even more detail for debugging an issue |
+| audit | Python auditing output only |
 
-These are configured as methods on the `getLogger()` class as well as on `logging` itself for the root logger.
 
 
 ## Logging Audit Events
 This package provides a system for turning `sys.audit()` events into log records using a thread-based queue. This is 
 necessary because audit events don't play nicely with the logging subsystem, leading to inconsistent errors if the
 logger `log()` method is called directly from the audit hook. Audit logging must be enabled specifically by setting
-the with_audit flag:
+the `with_audit` flag:
 
-    # .logging.toml
-    [logging]
-    with_audit = true
+```toml
+# .logging.toml
+[logging]
+with_audit = true
+```
 
 While the default level is "AUDIT", you can change this to any of the logging level prefixes by specifying the 
 audit_level:
 
-    # .logging.toml
-    [logging]
-    with_audit = true
-    audit_level = "INFO"
+```toml
+# .logging.toml
+[logging]
+with_audit = true
+audit_level = "INFO"
+```
 
-One specific event can cause further problems: sys._getframe() is called repeatedly from the logging subsystem in Python
+One specific event can cause further problems: `sys._getframe()` is called repeatedly from the logging subsystem in Python
 (in 3.8 at least). These audit events are NOT logged by default, but logging of them can be enabled by turning off the
 `omit_logging_frames` flag.
 
-    # .logging.toml
-    [logging]
-    with_audit = true
-    omit_logging_frames = false
+```toml
+# .logging.toml
+[logging]
+with_audit = true
+omit_logging_frames = false
+```
 
-Audit events are logged at the AUDIT level which is below TRACE; your logger and handler must be set to that level to 
+Audit events are logged (by default) at the AUDIT level which is below TRACE; your logger and handler must be set to that level to 
 see these events:
 
-    [logging.root]
-    level = "AUDIT"
-    handlers = ["console"]
-
-    [logging.handlers.console]
-    class = "logging.StreamHandler"
-    formatter = "brief"
-    level = "AUDIT"
-    stream = "ext://sys.stdout"
+```toml
+[logging.root]
+level = "AUDIT"
+handlers = ["console"]
+
+[logging.handlers.console]
+class = "logging.StreamHandler"
+formatter = "brief"
+level = "AUDIT"
+stream = "ext://sys.stdout"
+```
+
+## Change Log
+
+### version 0.2.0
+- Updated the audit handling thread to use a `threading.Event` to end itself rather than a boolean flag.
+- Added the `no_config` flag, mostly to be used in test suites to ensure everything still works properly.
+- Several documentation cleanup items
```

### Comparing `zrlog-0.1.1/setup.cfg` & `zrlog-0.2.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 207a 726c 6f67 0d0a 7665 7273 696f   = zrlog..versio
-00000020: 6e20 3d20 302e 312e 310d 0a61 7574 686f  n = 0.1.1..autho
+00000020: 6e20 3d20 302e 322e 300d 0a61 7574 686f  n = 0.2.0..autho
 00000030: 7220 3d20 4572 696e 2054 7572 6e62 756c  r = Erin Turnbul
 00000040: 6c0d 0a61 7574 686f 725f 656d 6169 6c20  l..author_email 
 00000050: 3d20 6572 696e 2e61 2e74 7572 6e62 756c  = erin.a.turnbul
 00000060: 6c40 676d 6169 6c2e 636f 6d0d 0a64 6573  l@gmail.com..des
 00000070: 6372 6970 7469 6f6e 203d 204c 6f67 6769  cription = Loggi
 00000080: 6e67 2077 6974 6820 5a69 7263 6f6e 6975  ng with Zirconiu
 00000090: 6d2d 6261 7365 6420 636f 6e66 6967 7572  m-based configur
```

### Comparing `zrlog-0.1.1/src/zrlog/logger.py` & `zrlog-0.2.0/src/zrlog/logger.py`

 * *Files identical despite different names*

### Comparing `zrlog-0.1.1/src/zrlog/logs.py` & `zrlog-0.2.0/src/zrlog/logs.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,49 +21,47 @@
             using the logging subsystem itself and clutter up the logs)
         :type omit_logging_frames: bool
     """
 
     def __init__(self, omit_logging_frames=True, log_level="AUDIT"):
         self._write_queue = queue.SimpleQueue()
         self.omit_logging_frames = omit_logging_frames
-        self._halt = False
+        self._halt = threading.Event()
         self.log = logging.getLogger("sys.audit")
         self._log_level_cb = self.log.audit
         if (not log_level == "AUDIT") and hasattr(self.log, log_level.lower()):
             self._log_level_cb = getattr(self.log, log_level.lower())
         self.lock = threading.Lock()
         super().__init__()
         self.daemon = True
 
     def halt(self):
         """ Stops the thread by setting the _halt flag and then joining. """
-        self._halt = True
+        self._halt.set()
         self.join()
 
     def audit_hook(self, action, info):
         """ Audit hook for sys.addaudithook() that queues the message to be sent. """
-        if not self._halt:
+        if not self._halt.is_set():
             s = "{}: {}".format(action, ";".join(str(x) for x in info))
             # sys._getframe is called a lot when logging, so this prevents a lot of junk from the logging module
             if (not self.omit_logging_frames) or not (action == "sys._getframe" and ("logging\\\\__init__.py" in s or "logging/__init__.py" in s)):
                 self._write_queue.put(s)
-            #self.log.audit(s)
 
     def run(self):
-        """ Implementation of run() """
-        while True:
+        """ Implement of run() """
+        while not self._halt.is_set():
             try:
-                nxt = self._write_queue.get(True, 0.1)
-                self._log_level_cb(nxt)
+                self._log_level_cb(self._write_queue.get(False))
             except queue.Empty as ex:
-                # Check for _halt here to make sure that the queue is empty when we halt
-                if self._halt:
-                    break
+                pass
                 # Give ourselves a bit of a break
-                time.sleep(0.01)
+                self._halt.wait(0.1)
+        while not self._write_queue.empty():
+            self._log_level_cb(self._write_queue.get(False))
 
 
 @zr.configure
 def config_logging(config: zr.ApplicationConfig):
     """ Configuration for zirconium """
     config.register_file("~/.logging.toml")
     config.register_file("./.logging.toml")
@@ -79,32 +77,33 @@
     method_name = level_name.lower()
     logging.addLevelName(level_no, level_name)
     setattr(logging, level_name, level_no)
     setattr(logging, method_name, log_at_level)
 
 
 @injector.inject
-def init_logging(config: zr.ApplicationConfig):
+def init_logging(no_config: bool = False, config: zr.ApplicationConfig = None):
     """ Initializes logging from the configuration file as well as adding our custom levels and, if specified, audit
         output
     """
-    # Audit is for the sys.audit(), if enabled
+    #Audit is for the sys.audit(), if enabled
     _add_logging_level("AUDIT", 1)
     # Trace is a lower level than debug for even more information
     _add_logging_level("TRACE", 5)
     # Out is a level higher than info but lower than warning for what a CLI user might want to see
     _add_logging_level("OUT", 25)
     # Import is done here in case something else has overridden the default logging class
     from .logger import ImprovedLogger
     logging.setLoggerClass(ImprovedLogger)
-    if "logging" in config:
+    if (not no_config) and "logging" in config:
         # Load our logging configuration
         logging.config.dictConfig(config["logging"])
         # If we want to include audit events, set up the logging for them
         if config.as_bool(("logging", "with_audit"), False) and sys.version_info.major >= 3 and sys.version_info.minor >= 8:
             audit_logger = AuditLog(
                 config.as_bool(("logging", "omit_logging_frames"), True),
                 config.as_str(("logging", "audit_level"), "AUDIT")
             )
             audit_logger.start()
             sys.addaudithook(audit_logger.audit_hook)
             atexit.register(audit_logger.halt)
+    logging.getLogger("zrlog").debug("Zirconium-based logging initialized")
```

