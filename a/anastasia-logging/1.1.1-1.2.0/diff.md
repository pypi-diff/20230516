# Comparing `tmp/anastasia_logging-1.1.1.tar.gz` & `tmp/anastasia_logging-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anastasia_logging-1.1.1.tar", max compression
+gzip compressed data, was "anastasia_logging-1.2.0.tar", max compression
```

## Comparing `anastasia_logging-1.1.1.tar` & `anastasia_logging-1.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     5339 2023-05-10 14:54:15.919165 anastasia_logging-1.1.1/README.md
--rw-r--r--   0        0        0     7990 2023-05-10 14:47:36.159319 anastasia_logging-1.1.1/anastasia_logging/__init__.py
--rw-r--r--   0        0        0       35 2023-05-09 14:56:24.294304 anastasia_logging-1.1.1/anastasia_logging/codes/__init__.py
--rw-r--r--   0        0        0      879 2023-05-09 16:53:34.979124 anastasia_logging-1.1.1/anastasia_logging/codes/standard.py
--rw-r--r--   0        0        0       92 2023-05-08 16:28:55.501019 anastasia_logging-1.1.1/anastasia_logging/codes/standard_errors.py
--rw-r--r--   0        0        0       55 2023-05-08 16:28:55.505019 anastasia_logging-1.1.1/anastasia_logging/codes/standard_info.py
--rw-r--r--   0        0        0      118 2023-05-08 16:28:55.505019 anastasia_logging-1.1.1/anastasia_logging/codes/standard_warning.py
--rw-r--r--   0        0        0       47 2023-05-09 20:12:08.106577 anastasia_logging-1.1.1/anastasia_logging/env/__init__.py
--rw-r--r--   0        0        0      553 2023-05-09 20:13:45.495205 anastasia_logging-1.1.1/anastasia_logging/env/env_variables.py
--rw-r--r--   0        0        0    10259 2023-05-09 20:16:26.872345 anastasia_logging-1.1.1/anastasia_logging/logger.py
--rw-r--r--   0        0        0      285 2023-05-10 14:51:57.373439 anastasia_logging-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     5782 1970-01-01 00:00:00.000000 anastasia_logging-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     5908 2023-05-15 22:04:49.293092 anastasia_logging-1.2.0/README.md
+-rw-r--r--   0        0        0     9601 2023-05-15 22:17:53.887196 anastasia_logging-1.2.0/anastasia_logging/__init__.py
+-rw-r--r--   0        0        0       35 2023-05-09 14:56:24.294304 anastasia_logging-1.2.0/anastasia_logging/codes/__init__.py
+-rw-r--r--   0        0        0      879 2023-05-09 16:53:34.979124 anastasia_logging-1.2.0/anastasia_logging/codes/standard.py
+-rw-r--r--   0        0        0       92 2023-05-08 16:28:55.501019 anastasia_logging-1.2.0/anastasia_logging/codes/standard_errors.py
+-rw-r--r--   0        0        0       55 2023-05-08 16:28:55.505019 anastasia_logging-1.2.0/anastasia_logging/codes/standard_info.py
+-rw-r--r--   0        0        0      118 2023-05-08 16:28:55.505019 anastasia_logging-1.2.0/anastasia_logging/codes/standard_warning.py
+-rw-r--r--   0        0        0       47 2023-05-09 20:12:08.106577 anastasia_logging-1.2.0/anastasia_logging/env/__init__.py
+-rw-r--r--   0        0        0      553 2023-05-09 20:13:45.495205 anastasia_logging-1.2.0/anastasia_logging/env/env_variables.py
+-rw-r--r--   0        0        0    13736 2023-05-15 22:36:46.978032 anastasia_logging-1.2.0/anastasia_logging/logger.py
+-rw-r--r--   0        0        0      285 2023-05-15 22:41:22.467111 anastasia_logging-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6351 1970-01-01 00:00:00.000000 anastasia_logging-1.2.0/PKG-INFO
```

### Comparing `anastasia_logging-1.1.1/README.md` & `anastasia_logging-1.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 ## **Summary** ##
 
 1. About *logging* python library
 2. Enhancements and additional functionalities
     1. Log Output Standarization
     2. Predefined Parameters for AnastasiaLoggers from Environment Variables
     3. Code Tags Standarization
+    4. Print Functionality
 3. Versioning
 
 ## **1. About *logging* Python Library** ##
 
 This repository is based in python base log management library called [logging](https://docs.python.org/3/library/logging.html).
 
 Commonly, when this library is intended to be used, for a basic usage a simple logging import is recommended to be used in order to avoid additional settings in our internal scripts.
@@ -108,16 +109,35 @@
 logging.warning("I am a dataset warning", 100)
 
 OUTPUT => 2023-05-08 11:55:27 UTC/GMT-0400 | [ANASTASIA-JOB] WARNING: <W100> I am a dataset warning
 ```
 
 If a code is already predefined and no message is introduced, a default message will appear according to code declared.
 
+### **2.4 Print Functionality** ###
+
+For a easy visualization in console without interacting with an AnastasiaLogger, you can use ```print``` like a python built-in print call.
+
+```
+import anastasia_logging as logging
+
+logging.print("Some prints to show")
+
+OUTPUT => 2023-05-08 11:55:27 UTC/GMT-0400 | [ANASTASIA-JOB] PRINT: Some prints to show
+```
+
 ## **3. Versioning** ##
 
+### v1.2.0 ###
+
+* Features:
+
+    * Function ```print``` incorporated
+    * Functions ```info```, ```warning```, ```error``` and ```print``` can return the formatted message for further usage
+
 ### v1.1.1 ###
 
 * Fixes:
 
     * Function ```basicConfig``` was skipping predefined structures with tags and log streamhandlers
 
 ### v1.1.0 ###
```

### Comparing `anastasia_logging-1.1.1/anastasia_logging/__init__.py` & `anastasia_logging-1.2.0/anastasia_logging/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 
     if not save_log:
         filename = None
 
     logging.basicConfig(filename=filename, format=format, datefmt=datefmt, level=level)
     logging.info("Root logging modified with AnastasiaLogger structure")
 
-def info(msg: Optional[str] = None, code: Optional[int] = None, save_log: bool = False, *args, **kwargs) -> Optional[str]:
+def info(msg: Optional[str] = None, code: Optional[int] = None, save_log: bool = False, return_formatted_msg: bool = False, *args, **kwargs) -> Optional[str]:
     """
     Inherited from logging.info function with additional properties
 
     Attributes
     ----------
 
     msg : Optional[str], default=None
@@ -147,21 +147,24 @@
 
     code : Optional[int], default=None
         Code assignation to add, if msg is not declared then it will search for default info codes
 
     save_log : bool, default=False
         Force to save log file, predefined with log_path attribute
 
+    return_formatted_msg : bool = False
+        If True, return the formatted message for further usage as a string
+
     *args, **kwargs inherited from logging.info function
 
     Returns
     -------
 
-    return_value : Optional[str]
-        Log path where file was saved, none if save_log = False
+    formatted_msg : Optional[str]
+        Message formatted with logger definitions
 
     Notes
     -----
 
     Base codes standards:
 
     -   0 = Unindentified
@@ -171,19 +174,17 @@
     - 4XX = Resources related
     - 5XX = Operative System (OS) related
     - 6XX = API related
     - 7XX = AWS related
 
     """
 
-    return_value = anastasia_logger.info(msg=msg, code=code, save_log=save_log, *args, **kwargs)
-
-    return return_value
+    return anastasia_logger.info(msg=msg, code=code, save_log=save_log, return_formatted_msg=return_formatted_msg, *args, **kwargs)
 
-def warning(msg: Optional[str] = None, code: Optional[int] = None, save_log: bool = False, *args, **kwargs) -> Optional[str]:
+def warning(msg: Optional[str] = None, code: Optional[int] = None, save_log: bool = False, return_formatted_msg: bool = False, *args, **kwargs) -> Optional[str]:
     """
     Inherited from logging.warning function with additional properties
 
     Attributes
     ----------
 
     msg : Optional[str], default=None
@@ -191,21 +192,24 @@
 
     code : Optional[int], default=None
         Code assignation to add, if msg is not declared then it will search for default warning codes
 
     save_log : bool, default=False
         Force to save log file, predefined with log_path attribute
 
+    return_formatted_msg : bool = False
+        If True, return the formatted message for further usage as a string
+
     *args, **kwargs inherited from logging.warning function
 
     Returns
     -------
 
-    return_value : Optional[str]
-        Log path where file was saved, none if save_log = False
+    formatted_msg : str
+        Message formatted with logger definitions
 
     Notes
     -----
 
     Base codes standards:
 
     -   0 = Unindentified
@@ -215,19 +219,17 @@
     - 4XX = Resources related
     - 5XX = Operative System (OS) related
     - 6XX = API related
     - 7XX = AWS related
 
     """
 
-    return_value = anastasia_logger.warning(msg=msg, code=code, save_log=save_log, *args, **kwargs)
+    return anastasia_logger.warning(msg=msg, code=code, save_log=save_log, return_formatted_msg=return_formatted_msg, *args, **kwargs)
 
-    return return_value
-
-def error(msg: Optional[str] = None, code: Optional[int] = None, raise_type: Optional[type] = None, save_log: bool = False, *args, **kwargs) -> Optional[str]:
+def error(msg: Optional[str] = None, code: Optional[int] = None, raise_type: Optional[type] = None, save_log: bool = False, return_formatted_msg: bool = False, *args, **kwargs) -> Optional[str]:
     """
     Inherited from logging.error function with additional properties
 
     Attributes
     ----------
 
     msg : Optional[str], default=None
@@ -238,21 +240,24 @@
 
     raise_type : Optional[type], default=None
         Raise any type with message content as text description and terminating python script execution, if None then no python type will be raised
 
     save_log : bool, default=False
         Force to save log file, predefined with log_path attribute
 
+    return_formatted_msg : bool = False
+        If True, return the formatted message for further usage as a string
+
     *args, **kwargs inherited from logging.error function
 
     Returns
     -------
 
-    return_value : Optional[str]
-        Log path where file was saved, none if save_log = False
+    formatted_msg : str
+            Message formatted with logger definitions
 
     Notes
     -----
 
     Base codes standards:
 
     -   0 = Unindentified
@@ -261,12 +266,49 @@
     - 3XX = AI related
     - 4XX = Resources related
     - 5XX = Operative System (OS) related
     - 6XX = API related
     - 7XX = AWS related
 
     """
-
-    return_value = anastasia_logger.error(msg=msg, code=code, raise_type=raise_type, save_log=save_log, *args, **kwargs)
     
-    return return_value
+    return anastasia_logger.error(msg=msg, code=code, raise_type=raise_type, save_log=save_log, return_formatted_msg=return_formatted_msg, *args, **kwargs)
+
+def print(msg: Optional[str] = None, code: Optional[int] = None, return_formatted_msg: bool = False, *args, **kwargs) -> Optional[str]:
+    """
+    Show in console a required message with logger format, doesn't register in contained handlers (just for console view, like a normal python print). 
+
+    Attributes
+    ----------
+
+    msg : Optional[str], default=None
+        Name identification of logger instance
+
+    code : Optional[int], default=None
+        Code assignation to add, if msg is not declared then it will search for default error codes
+
+    return_formatted_msg : bool = False
+            If True, return the formatted message for further usage as a string
+
+    Returns
+    -------
+
+    formatted_msg : str
+        Message formatted with logger definitions
+
+    Notes
+    -----
+
+    Base codes standards:
 
+    -   0 = Unindentified
+    - 1XX = Data related
+    - 2XX = Mathematical related
+    - 3XX = AI related
+    - 4XX = Resources related
+    - 5XX = Operative System (OS) related
+    - 6XX = API related
+    - 7XX = AWS related
+
+    """
+    
+    return anastasia_logger.print(msg=msg, code=code, return_formatted_msg=return_formatted_msg, *args, **kwargs)
```

### Comparing `anastasia_logging-1.1.1/anastasia_logging/codes/standard.py` & `anastasia_logging-1.2.0/anastasia_logging/codes/standard.py`

 * *Files identical despite different names*

### Comparing `anastasia_logging-1.1.1/anastasia_logging/env/env_variables.py` & `anastasia_logging-1.2.0/anastasia_logging/env/env_variables.py`

 * *Files identical despite different names*

### Comparing `anastasia_logging-1.1.1/anastasia_logging/logger.py` & `anastasia_logging-1.2.0/anastasia_logging/logger.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,20 @@
+import time
+
 from typing import Optional
-from logging import getLogger
+from logging import getLogger, _levelToName
 from logging import Logger, Formatter, FileHandler, StreamHandler
 from logging import INFO, WARNING, ERROR, DEBUG, CRITICAL, FATAL 
 
 from anastasia_logging.codes import StandardCodes
 from anastasia_logging.env import EnvironmentVariables
 
+PRINT = -1
+
+
 class AnastasiaLogger(Logger):
 
     def __init__(self, name: Optional[str] = None, tag: Optional[str] = None, level: Optional[str] = None, save_log: Optional[bool] = None, log_path: Optional[str] = None):
         """
         Class wrapper from logging.Logger implementation
 
         Attributes
@@ -99,18 +104,20 @@
 
         standard_codes : dict
             Dict with codes and default descriptions
 
         """
         if level == INFO:
             return self.standard_codes.INFO
-        if level == WARNING:
+        elif level == WARNING:
             return self.standard_codes.WARNING
-        if level == ERROR:
+        elif level == ERROR:
             return self.standard_codes.ERROR
+        elif level == PRINT:
+            return {}
         else:
             val = "Level detected doesn't exists or is not implemented"
             self.error(val)
             raise ValueError(val)
         
     def _initial_severity_tag_code(self, level: int) -> str:
         """
@@ -137,14 +144,16 @@
             return "E"
         elif level == DEBUG:
             return "D"
         elif level == CRITICAL:
             return "C"
         elif level == FATAL:
             return "F"
+        elif level == PRINT:
+            return "P"
         else:
             val = "Level detected doesn't exists or is not implemented"
             self.error(val)
             raise ValueError(val)
         
     def _check_code_msg(self, level: int, msg: Optional[str] = None, code: Optional[int] = None) -> str:
         """
@@ -184,15 +193,15 @@
             else:
                 val = "Code is not a number"
                 self.error(val)
                 raise ValueError(val)
             
         return msg
         
-    def info(self, msg: Optional[str] = None, code: Optional[int] = None, save_log: bool = False, *args, **kwargs) -> Optional[str]:
+    def info(self, msg: Optional[str] = None, code: Optional[int] = None, save_log: bool = False, return_formatted_msg: bool = False, *args, **kwargs) -> Optional[str]:
         """
         Inherited from logging.info function with additional properties
 
         Attributes
         ----------
 
         msg : Optional[str], default=None
@@ -200,21 +209,24 @@
 
         code : Optional[int], default=None
             Code assignation to add, if msg is not declared then it will search for default info codes
 
         save_log : bool, default=False
             Force to save log file, predefined with log_path attribute
 
+        return_formatted_msg : bool = False
+            If True, return the formatted message for further usage as a string
+
         *args, **kwargs inherited from logging.info function
 
         Returns
         -------
 
-        return_value : Optional[str]
-            Log path where file was saved, none if save_log = False
+        formatted_msg : Optional[str]
+            Message formatted with logger definitions
 
         Notes
         -----
 
         Base codes standards:
 
         -   0 = Unindentified
@@ -226,25 +238,24 @@
         - 6XX = API related
         - 7XX = AWS related
 
         """
 
         msg = self._check_code_msg(INFO, msg, code)
 
-        return_value = None
         if save_log:
             self._initial_filehandler(self.log_path)
-            return_value = self.log_path
 
         if self.isEnabledFor(INFO):
             self._log(INFO, msg, args, **kwargs)
 
-        return return_value
+        if return_formatted_msg:
+            return self._getprint(msg=msg, level=INFO, *args, **kwargs)
 
-    def warning(self, msg: Optional[str] = None, code: Optional[int] = None, save_log: bool = False, *args, **kwargs) -> Optional[str]:
+    def warning(self, msg: Optional[str] = None, code: Optional[int] = None, save_log: bool = False, return_formatted_msg: bool = False, *args, **kwargs) -> Optional[str]:
         """
         Inherited from logging.warning function with additional properties
 
         Attributes
         ----------
 
         msg : Optional[str], default=None
@@ -252,21 +263,24 @@
 
         code : Optional[int], default=None
             Code assignation to add, if msg is not declared then it will search for default warning codes
 
         save_log : bool, default=False
             Force to save log file, predefined with log_path attribute
 
+        return_formatted_msg : bool = False
+            If True, return the formatted message for further usage as a string
+
         *args, **kwargs inherited from logging.warning function
 
         Returns
         -------
 
-        return_value : Optional[str]
-            Log path where file was saved, none if save_log = False
+        formatted_msg : str
+            Message formatted with logger definitions
 
         Notes
         -----
 
         Base codes standards:
 
         -   0 = Unindentified
@@ -278,25 +292,24 @@
         - 6XX = API related
         - 7XX = AWS related
 
         """
 
         msg = self._check_code_msg(WARNING, msg, code)
 
-        return_value = None
         if save_log:
             self._initial_filehandler(self.log_path)
-            return_value = self.log_path
 
         if self.isEnabledFor(WARNING):
             self._log(WARNING, msg, args, **kwargs)
 
-        return return_value
+        if return_formatted_msg:
+            return self._getprint(msg=msg, level=WARNING, *args, **kwargs)
 
-    def error(self, msg: Optional[str] = None, code: Optional[int] = None, raise_type: Optional[type] = None, save_log: bool = False, *args, **kwargs) -> Optional[str]:
+    def error(self, msg: Optional[str] = None, code: Optional[int] = None, raise_type: Optional[type] = None, save_log: bool = False, return_formatted_msg: bool = False, *args, **kwargs) -> Optional[str]:
         """
         Inherited from logging.error function with additional properties
 
         Attributes
         ----------
 
         msg : Optional[str], default=None
@@ -307,21 +320,24 @@
 
         raise_type : Optional[type], default=None
             Raise any type with message content as text description and terminating python script execution, if None then no python type will be raised
 
         save_log : bool, default=False
             Force to save log file, predefined with log_path attribute
 
+        return_formatted_msg : bool = False
+            If True, return the formatted message for further usage as a string
+
         *args, **kwargs inherited from logging.error function
 
         Returns
         -------
 
-        return_value : Optional[str]
-            Log path where file was saved, none if save_log = False
+        formatted_msg : str
+            Message formatted with logger definitions
 
         Notes
         -----
 
         Base codes standards:
 
         -   0 = Unindentified
@@ -333,19 +349,112 @@
         - 6XX = API related
         - 7XX = AWS related
 
         """
 
         msg = self._check_code_msg(ERROR, msg, code)
 
-        return_value = None
         if save_log:
             self._initial_filehandler(self.log_path)
-            return_value = self.log_path
 
         if self.isEnabledFor(ERROR):
             self._log(ERROR, msg, args, **kwargs)
 
         if isinstance(raise_type, type):
             raise raise_type(msg)
         
-        return return_value
+        if return_formatted_msg:
+            return self._getprint(msg=msg, level=ERROR, *args, **kwargs)
+    
+    def print(self, msg: Optional[str] = None, code: Optional[int] = None, return_formatted_msg: bool = False, *args, **kwargs) -> Optional[str]:
+        """
+        Show in console a required message with logger format, doesn't register in contained handlers (just for console view, like a normal python print). 
+
+        Attributes
+        ----------
+
+        msg : Optional[str], default=None
+            Name identification of logger instance
+
+        code : Optional[int], default=None
+            Code assignation to add, if msg is not declared then it will search for default error codes
+
+        return_formatted_msg : bool = False
+            If True, return the formatted message for further usage as a string
+
+        Returns
+        -------
+
+        formatted_msg : str
+            Message formatted with logger definitions
+
+        Notes
+        -----
+
+        Base codes standards:
+
+        -   0 = Unindentified
+        - 1XX = Data related
+        - 2XX = Mathematical related
+        - 3XX = AI related
+        - 4XX = Resources related
+        - 5XX = Operative System (OS) related
+        - 6XX = API related
+        - 7XX = AWS related
+
+        """
+        console_msg = self._getprint(msg=msg, code=code, level=PRINT, *args, **kwargs)
+        print(console_msg)
+
+        if return_formatted_msg:
+            return console_msg
+
+    def _getprint(self, level: int, msg: Optional[str] = None, code: Optional[int] = None, *args, **kwargs) -> str:
+        """
+        Obtain a string with an example of logger output contained from message. 
+
+        Attributes
+        ----------
+
+        msg : Optional[str], default=None
+            Name identification of logger instance
+
+        code : Optional[int], default=None
+            Code assignation to add, if msg is not declared then it will search for default error codes
+
+        Returns
+        -------
+
+        msg : str
+            Original message with logger format
+
+        Notes
+        -----
+
+        Base codes standards:
+
+        -   0 = Unindentified
+        - 1XX = Data related
+        - 2XX = Mathematical related
+        - 3XX = AI related
+        - 4XX = Resources related
+        - 5XX = Operative System (OS) related
+        - 6XX = API related
+        - 7XX = AWS related
+
+        """
+        fmt = self.formatter._fmt
+        datefmt = self.formatter.datefmt
+
+        asctime = time.strftime(datefmt)
+        fmt = fmt.replace("%(", "{").replace(")s", "}")
+        msg = self._check_code_msg(level, msg, code)
+        
+        if level == PRINT:
+            levelname = "PRINT"
+        elif level in [INFO, WARNING, ERROR, DEBUG, CRITICAL, FATAL]:
+            levelname = _levelToName[level]
+        else:
+            val = "Level detected doesn't exists or is not implemented"
+            self.error(val)
+
+        return fmt.format(asctime=asctime, levelname=levelname, message=msg)
```

### Comparing `anastasia_logging-1.1.1/PKG-INFO` & `anastasia_logging-1.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anastasia-logging
-Version: 1.1.1
+Version: 1.2.0
 Summary: Anastasia Logging Standarization
 Author: anastasiaai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -18,14 +18,15 @@
 ## **Summary** ##
 
 1. About *logging* python library
 2. Enhancements and additional functionalities
     1. Log Output Standarization
     2. Predefined Parameters for AnastasiaLoggers from Environment Variables
     3. Code Tags Standarization
+    4. Print Functionality
 3. Versioning
 
 ## **1. About *logging* Python Library** ##
 
 This repository is based in python base log management library called [logging](https://docs.python.org/3/library/logging.html).
 
 Commonly, when this library is intended to be used, for a basic usage a simple logging import is recommended to be used in order to avoid additional settings in our internal scripts.
@@ -121,16 +122,35 @@
 logging.warning("I am a dataset warning", 100)
 
 OUTPUT => 2023-05-08 11:55:27 UTC/GMT-0400 | [ANASTASIA-JOB] WARNING: <W100> I am a dataset warning
 ```
 
 If a code is already predefined and no message is introduced, a default message will appear according to code declared.
 
+### **2.4 Print Functionality** ###
+
+For a easy visualization in console without interacting with an AnastasiaLogger, you can use ```print``` like a python built-in print call.
+
+```
+import anastasia_logging as logging
+
+logging.print("Some prints to show")
+
+OUTPUT => 2023-05-08 11:55:27 UTC/GMT-0400 | [ANASTASIA-JOB] PRINT: Some prints to show
+```
+
 ## **3. Versioning** ##
 
+### v1.2.0 ###
+
+* Features:
+
+    * Function ```print``` incorporated
+    * Functions ```info```, ```warning```, ```error``` and ```print``` can return the formatted message for further usage
+
 ### v1.1.1 ###
 
 * Fixes:
 
     * Function ```basicConfig``` was skipping predefined structures with tags and log streamhandlers
 
 ### v1.1.0 ###
```

