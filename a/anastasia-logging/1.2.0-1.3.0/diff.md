# Comparing `tmp/anastasia_logging-1.2.0.tar.gz` & `tmp/anastasia_logging-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anastasia_logging-1.2.0.tar", max compression
+gzip compressed data, was "anastasia_logging-1.3.0.tar", max compression
```

## Comparing `anastasia_logging-1.2.0.tar` & `anastasia_logging-1.3.0.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0     5908 2023-05-15 22:04:49.293092 anastasia_logging-1.2.0/README.md
--rw-r--r--   0        0        0     9601 2023-05-15 22:17:53.887196 anastasia_logging-1.2.0/anastasia_logging/__init__.py
--rw-r--r--   0        0        0       35 2023-05-09 14:56:24.294304 anastasia_logging-1.2.0/anastasia_logging/codes/__init__.py
--rw-r--r--   0        0        0      879 2023-05-09 16:53:34.979124 anastasia_logging-1.2.0/anastasia_logging/codes/standard.py
--rw-r--r--   0        0        0       92 2023-05-08 16:28:55.501019 anastasia_logging-1.2.0/anastasia_logging/codes/standard_errors.py
--rw-r--r--   0        0        0       55 2023-05-08 16:28:55.505019 anastasia_logging-1.2.0/anastasia_logging/codes/standard_info.py
--rw-r--r--   0        0        0      118 2023-05-08 16:28:55.505019 anastasia_logging-1.2.0/anastasia_logging/codes/standard_warning.py
--rw-r--r--   0        0        0       47 2023-05-09 20:12:08.106577 anastasia_logging-1.2.0/anastasia_logging/env/__init__.py
--rw-r--r--   0        0        0      553 2023-05-09 20:13:45.495205 anastasia_logging-1.2.0/anastasia_logging/env/env_variables.py
--rw-r--r--   0        0        0    13736 2023-05-15 22:36:46.978032 anastasia_logging-1.2.0/anastasia_logging/logger.py
--rw-r--r--   0        0        0      285 2023-05-15 22:41:22.467111 anastasia_logging-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     6351 1970-01-01 00:00:00.000000 anastasia_logging-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     6171 2023-05-16 18:44:03.254943 anastasia_logging-1.3.0/README.md
+-rw-r--r--   0        0        0    12541 2023-05-16 19:03:05.770304 anastasia_logging-1.3.0/anastasia_logging/__init__.py
+-rw-r--r--   0        0        0       35 2023-05-09 14:56:24.294304 anastasia_logging-1.3.0/anastasia_logging/codes/__init__.py
+-rw-r--r--   0        0        0     1200 2023-05-16 19:06:41.059173 anastasia_logging-1.3.0/anastasia_logging/codes/standard.py
+-rw-r--r--   0        0        0       59 2023-05-16 19:04:35.614812 anastasia_logging-1.3.0/anastasia_logging/codes/standard_critical.py
+-rw-r--r--   0        0        0       56 2023-05-16 19:03:57.198623 anastasia_logging-1.3.0/anastasia_logging/codes/standard_debug.py
+-rw-r--r--   0        0        0       92 2023-05-08 16:28:55.501019 anastasia_logging-1.3.0/anastasia_logging/codes/standard_errors.py
+-rw-r--r--   0        0        0       55 2023-05-08 16:28:55.505019 anastasia_logging-1.3.0/anastasia_logging/codes/standard_info.py
+-rw-r--r--   0        0        0      118 2023-05-08 16:28:55.505019 anastasia_logging-1.3.0/anastasia_logging/codes/standard_warning.py
+-rw-r--r--   0        0        0       47 2023-05-09 20:12:08.106577 anastasia_logging-1.3.0/anastasia_logging/env/__init__.py
+-rw-r--r--   0        0        0      553 2023-05-16 19:09:23.183169 anastasia_logging-1.3.0/anastasia_logging/env/env_variables.py
+-rw-r--r--   0        0        0    17527 2023-05-16 19:00:15.432605 anastasia_logging-1.3.0/anastasia_logging/logger.py
+-rw-r--r--   0        0        0      285 2023-05-16 18:44:41.226247 anastasia_logging-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6614 1970-01-01 00:00:00.000000 anastasia_logging-1.3.0/PKG-INFO
```

### Comparing `anastasia_logging-1.2.0/README.md` & `anastasia_logging-1.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 logger.warning("I am a very usefull warning")
 
 OUTPUT => I am a very usefull warning
 ```
 
 Have you noticed in the first import logging example that appears the word *root* in the output console? This is because when you use ```import logging``` directly, a default Logger class is instanciated with name *root* along with default configurations.
 
-This repository contains a class called **AnastasiaLogger**, which inherits from Logger class and standarize logging definitions and has some improvments over information (*.info()*), warning (*.warning()*) and error (*.error()*) methods.
+This repository contains a class called **AnastasiaLogger**, which inherits from Logger class and standarize logging definitions and has some improvments over debugging (```.debug()```), information (```.info()```), warning (```.warning()```), error (```.error()```), critical (```.critical()```) and fatal (```.fatal()```) methods.
 
 ```
 from anastasia_logging import AnastasiaLogger
 
 logger = AnastasiaLogger()
 logger.warning("I am a very usefull warning")
 
@@ -97,15 +97,15 @@
 |    2XX   	|   Mathematical related    |
 |    3XX   	|        AI related         |
 |    4XX   	|     Resources related 	|
 |    5XX   	| Operative System related 	|
 |    6XX   	|       API related         |
 |    7XX   	|       AWS related         |
 
-Methods info(), warning() and error() can be declared with a code as parameter in order to extended log with a code description.
+Methods ```debug()```, ```info()```, ```warning()```, ```error()```, ```critical()``` and ```fatal()``` can be declared with a code as parameter in order to extended log with a code description.
 
 ```
 import anastasia_logging as logging
 
 logging.warning("I am a dataset warning", 100)
 
 OUTPUT => 2023-05-08 11:55:27 UTC/GMT-0400 | [ANASTASIA-JOB] WARNING: <W100> I am a dataset warning
@@ -123,14 +123,20 @@
 logging.print("Some prints to show")
 
 OUTPUT => 2023-05-08 11:55:27 UTC/GMT-0400 | [ANASTASIA-JOB] PRINT: Some prints to show
 ```
 
 ## **3. Versioning** ##
 
+### v1.3.0 ###
+
+* Features:
+
+    * Functions ```critical```, ```fatal``` and ```debug``` incorporated
+
 ### v1.2.0 ###
 
 * Features:
 
     * Function ```print``` incorporated
     * Functions ```info```, ```warning```, ```error``` and ```print``` can return the formatted message for further usage
```

### Comparing `anastasia_logging-1.2.0/anastasia_logging/__init__.py` & `anastasia_logging-1.3.0/anastasia_logging/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -131,14 +131,59 @@
 
     if not save_log:
         filename = None
 
     logging.basicConfig(filename=filename, format=format, datefmt=datefmt, level=level)
     logging.info("Root logging modified with AnastasiaLogger structure")
 
+def debug(msg: Optional[str] = None, code: Optional[int] = None, save_log: bool = False, return_formatted_msg: bool = False, *args, **kwargs) -> Optional[str]:
+    """
+    Inherited from logging.debug function with additional properties
+
+    Attributes
+    ----------
+
+    msg : Optional[str], default=None
+        Name identification of logger instance
+
+    code : Optional[int], default=None
+        Code assignation to add, if msg is not declared then it will search for default debug codes
+
+    save_log : bool, default=False
+        Force to save log file, predefined with log_path attribute
+
+    return_formatted_msg : bool = False
+        If True, return the formatted message for further usage as a string
+
+    *args, **kwargs inherited from logging.debug function
+
+    Returns
+    -------
+
+    formatted_msg : Optional[str]
+        Message formatted with logger definitions
+
+    Notes
+    -----
+
+    Base codes standards:
+
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
+    return anastasia_logger.debug(msg=msg, code=code, save_log=save_log, return_formatted_msg=return_formatted_msg, *args, **kwargs)
+
 def info(msg: Optional[str] = None, code: Optional[int] = None, save_log: bool = False, return_formatted_msg: bool = False, *args, **kwargs) -> Optional[str]:
     """
     Inherited from logging.info function with additional properties
 
     Attributes
     ----------
 
@@ -269,14 +314,64 @@
     - 6XX = API related
     - 7XX = AWS related
 
     """
     
     return anastasia_logger.error(msg=msg, code=code, raise_type=raise_type, save_log=save_log, return_formatted_msg=return_formatted_msg, *args, **kwargs)
 
+def critical(msg: Optional[str] = None, code: Optional[int] = None, raise_type: Optional[type] = None, save_log: bool = False, return_formatted_msg: bool = False, *args, **kwargs) -> Optional[str]:
+    """
+    Inherited from logging.critical function with additional properties
+
+    Attributes
+    ----------
+
+    msg : Optional[str], default=None
+        Name identification of logger instance
+
+    code : Optional[int], default=None
+        Code assignation to add, if msg is not declared then it will search for default critical codes
+
+    raise_type : Optional[type], default=None
+        Raise any type with message content as text description and terminating python script execution, if None then no python type will be raised
+
+    save_log : bool, default=False
+        Force to save log file, predefined with log_path attribute
+
+    return_formatted_msg : bool = False
+        If True, return the formatted message for further usage as a string
+
+    *args, **kwargs inherited from logging.critical function
+
+    Returns
+    -------
+
+    formatted_msg : str
+            Message formatted with logger definitions
+
+    Notes
+    -----
+
+    Base codes standards:
+
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
+    return anastasia_logger.critical(msg=msg, code=code, raise_type=raise_type, save_log=save_log, return_formatted_msg=return_formatted_msg, *args, **kwargs)
+
+fatal = critical # fatal = critical in base logging implementation
+
 def print(msg: Optional[str] = None, code: Optional[int] = None, return_formatted_msg: bool = False, *args, **kwargs) -> Optional[str]:
     """
     Show in console a required message with logger format, doesn't register in contained handlers (just for console view, like a normal python print). 
 
     Attributes
     ----------
```

### Comparing `anastasia_logging-1.2.0/anastasia_logging/codes/standard.py` & `anastasia_logging-1.3.0/anastasia_logging/codes/standard.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from typing import Dict
 from dataclasses import dataclass, field
 
-from anastasia_logging.codes.standard_errors import _STANDARD_ERROR_CODES
-from anastasia_logging.codes.standard_warning import _STANDARD_WARNING_CODES
+from anastasia_logging.codes.standard_debug import _STANDARD_DEBUG_CODES
 from anastasia_logging.codes.standard_info import _STANDARD_INFO_CODES
+from anastasia_logging.codes.standard_warning import _STANDARD_WARNING_CODES
+from anastasia_logging.codes.standard_errors import _STANDARD_ERROR_CODES
+from anastasia_logging.codes.standard_critical import _STANDARD_CRITICAL_CODES
+
 
 @dataclass
 class StandardCodes:
     """
 
     Standard Codifications
 
@@ -20,10 +23,12 @@
     - 4XX = Resources related
     - 5XX = Operative System (OS) related
     - 6XX = API related
     - 7XX = AWS related
 
     """
 
-    ERROR: Dict[int, str] = field(default_factory=lambda: _STANDARD_ERROR_CODES)
+    DEBUG: Dict[int, str] = field(default_factory=lambda: _STANDARD_DEBUG_CODES)
+    INFO: Dict[int, str] = field(default_factory=lambda: _STANDARD_INFO_CODES)
     WARNING: Dict[int, str] = field(default_factory=lambda: _STANDARD_WARNING_CODES)
-    INFO: Dict[int, str] = field(default_factory=lambda: _STANDARD_INFO_CODES)
+    ERROR: Dict[int, str] = field(default_factory=lambda: _STANDARD_ERROR_CODES)
+    CRITICAL: Dict[int, str] = field(default_factory=lambda: _STANDARD_CRITICAL_CODES)
```

### Comparing `anastasia_logging-1.2.0/anastasia_logging/env/env_variables.py` & `anastasia_logging-1.3.0/anastasia_logging/env/env_variables.py`

 * *Files identical despite different names*

### Comparing `anastasia_logging-1.2.0/anastasia_logging/logger.py` & `anastasia_logging-1.3.0/anastasia_logging/logger.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import time
 
 from typing import Optional
 from logging import getLogger, _levelToName
 from logging import Logger, Formatter, FileHandler, StreamHandler
-from logging import INFO, WARNING, ERROR, DEBUG, CRITICAL, FATAL 
+from logging import DEBUG, INFO, WARNING, ERROR, DEBUG, CRITICAL, FATAL 
 
 from anastasia_logging.codes import StandardCodes
 from anastasia_logging.env import EnvironmentVariables
 
 PRINT = -1
 
 
@@ -102,20 +102,24 @@
         Returns
         -------
 
         standard_codes : dict
             Dict with codes and default descriptions
 
         """
-        if level == INFO:
+        if level == DEBUG:
+            return self.standard_codes.DEBUG
+        elif level == INFO:
             return self.standard_codes.INFO
         elif level == WARNING:
             return self.standard_codes.WARNING
         elif level == ERROR:
             return self.standard_codes.ERROR
+        elif level == CRITICAL or level == FATAL:
+            return self.standard_codes.CRITICAL
         elif level == PRINT:
             return {}
         else:
             val = "Level detected doesn't exists or is not implemented"
             self.error(val)
             raise ValueError(val)
         
@@ -132,26 +136,24 @@
         Returns
         -------
 
         str : str
             Letter representing level severity
 
         """
-        if level == INFO:
+        if level == DEBUG:
+            return "D"
+        elif level == INFO:
             return "I"
         elif level == WARNING:
             return "W"
         elif level == ERROR:
             return "E"
-        elif level == DEBUG:
-            return "D"
-        elif level == CRITICAL:
+        elif level == CRITICAL or level == FATAL:
             return "C"
-        elif level == FATAL:
-            return "F"
         elif level == PRINT:
             return "P"
         else:
             val = "Level detected doesn't exists or is not implemented"
             self.error(val)
             raise ValueError(val)
         
@@ -192,15 +194,69 @@
                 msg = f"<{self._initial_severity_tag_code(level)}{code}> " + msg
             else:
                 val = "Code is not a number"
                 self.error(val)
                 raise ValueError(val)
             
         return msg
-        
+
+    def debug(self, msg: Optional[str] = None, code: Optional[int] = None, save_log: bool = False, return_formatted_msg: bool = False, *args, **kwargs) -> Optional[str]:
+        """
+        Inherited from logging.debug function with additional properties
+
+        Attributes
+        ----------
+
+        msg : Optional[str], default=None
+            Name identification of logger instance
+
+        code : Optional[int], default=None
+            Code assignation to add, if msg is not declared then it will search for default debug codes
+
+        save_log : bool, default=False
+            Force to save log file, predefined with log_path attribute
+
+        return_formatted_msg : bool = False
+            If True, return the formatted message for further usage as a string
+
+        *args, **kwargs inherited from logging.debug function
+
+        Returns
+        -------
+
+        formatted_msg : Optional[str]
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
+
+        msg = self._check_code_msg(DEBUG, msg, code)
+
+        if save_log:
+            self._initial_filehandler(self.log_path)
+
+        if self.isEnabledFor(DEBUG):
+            self._log(DEBUG, msg, args, **kwargs)
+
+        if return_formatted_msg:
+            return self._getprint(msg=msg, level=DEBUG, *args, **kwargs)
+
     def info(self, msg: Optional[str] = None, code: Optional[int] = None, save_log: bool = False, return_formatted_msg: bool = False, *args, **kwargs) -> Optional[str]:
         """
         Inherited from logging.info function with additional properties
 
         Attributes
         ----------
 
@@ -360,15 +416,77 @@
             self._log(ERROR, msg, args, **kwargs)
 
         if isinstance(raise_type, type):
             raise raise_type(msg)
         
         if return_formatted_msg:
             return self._getprint(msg=msg, level=ERROR, *args, **kwargs)
+        
+    def critical(self, msg: Optional[str] = None, code: Optional[int] = None, raise_type: Optional[type] = None, save_log: bool = False, return_formatted_msg: bool = False, *args, **kwargs) -> Optional[str]:
+        """
+        Inherited from logging.critical function with additional properties
+
+        Attributes
+        ----------
+
+        msg : Optional[str], default=None
+            Name identification of logger instance
+
+        code : Optional[int], default=None
+            Code assignation to add, if msg is not declared then it will search for default critical codes
+
+        raise_type : Optional[type], default=None
+            Raise any type with message content as text description and terminating python script execution, if None then no python type will be raised
+
+        save_log : bool, default=False
+            Force to save log file, predefined with log_path attribute
+
+        return_formatted_msg : bool = False
+            If True, return the formatted message for further usage as a string
+
+        *args, **kwargs inherited from logging.critical function
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
+
+        msg = self._check_code_msg(CRITICAL, msg, code)
+
+        if save_log:
+            self._initial_filehandler(self.log_path)
+
+        if self.isEnabledFor(CRITICAL):
+            self._log(CRITICAL, msg, args, **kwargs)
+
+        if isinstance(raise_type, type):
+            raise raise_type(msg)
+        
+        if return_formatted_msg:
+            return self._getprint(msg=msg, level=CRITICAL, *args, **kwargs)
     
+    fatal = critical # fatal = critical in base logging implementation
+
     def print(self, msg: Optional[str] = None, code: Optional[int] = None, return_formatted_msg: bool = False, *args, **kwargs) -> Optional[str]:
         """
         Show in console a required message with logger format, doesn't register in contained handlers (just for console view, like a normal python print). 
 
         Attributes
         ----------
```

### Comparing `anastasia_logging-1.2.0/PKG-INFO` & `anastasia_logging-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anastasia-logging
-Version: 1.2.0
+Version: 1.3.0
 Summary: Anastasia Logging Standarization
 Author: anastasiaai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -48,15 +48,15 @@
 logger.warning("I am a very usefull warning")
 
 OUTPUT => I am a very usefull warning
 ```
 
 Have you noticed in the first import logging example that appears the word *root* in the output console? This is because when you use ```import logging``` directly, a default Logger class is instanciated with name *root* along with default configurations.
 
-This repository contains a class called **AnastasiaLogger**, which inherits from Logger class and standarize logging definitions and has some improvments over information (*.info()*), warning (*.warning()*) and error (*.error()*) methods.
+This repository contains a class called **AnastasiaLogger**, which inherits from Logger class and standarize logging definitions and has some improvments over debugging (```.debug()```), information (```.info()```), warning (```.warning()```), error (```.error()```), critical (```.critical()```) and fatal (```.fatal()```) methods.
 
 ```
 from anastasia_logging import AnastasiaLogger
 
 logger = AnastasiaLogger()
 logger.warning("I am a very usefull warning")
 
@@ -110,15 +110,15 @@
 |    2XX   	|   Mathematical related    |
 |    3XX   	|        AI related         |
 |    4XX   	|     Resources related 	|
 |    5XX   	| Operative System related 	|
 |    6XX   	|       API related         |
 |    7XX   	|       AWS related         |
 
-Methods info(), warning() and error() can be declared with a code as parameter in order to extended log with a code description.
+Methods ```debug()```, ```info()```, ```warning()```, ```error()```, ```critical()``` and ```fatal()``` can be declared with a code as parameter in order to extended log with a code description.
 
 ```
 import anastasia_logging as logging
 
 logging.warning("I am a dataset warning", 100)
 
 OUTPUT => 2023-05-08 11:55:27 UTC/GMT-0400 | [ANASTASIA-JOB] WARNING: <W100> I am a dataset warning
@@ -136,14 +136,20 @@
 logging.print("Some prints to show")
 
 OUTPUT => 2023-05-08 11:55:27 UTC/GMT-0400 | [ANASTASIA-JOB] PRINT: Some prints to show
 ```
 
 ## **3. Versioning** ##
 
+### v1.3.0 ###
+
+* Features:
+
+    * Functions ```critical```, ```fatal``` and ```debug``` incorporated
+
 ### v1.2.0 ###
 
 * Features:
 
     * Function ```print``` incorporated
     * Functions ```info```, ```warning```, ```error``` and ```print``` can return the formatted message for further usage
```

