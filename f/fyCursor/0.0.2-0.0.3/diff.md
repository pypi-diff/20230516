# Comparing `tmp/fyCursor-0.0.2.tar.gz` & `tmp/fyCursor-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fyCursor-0.0.2.tar", last modified: Tue May 16 02:01:07 2023, max compression
+gzip compressed data, was "fyCursor-0.0.3.tar", last modified: Tue May 16 03:39:00 2023, max compression
```

## Comparing `fyCursor-0.0.2.tar` & `fyCursor-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 danielkay   (503) staff       (20)        0 2023-05-16 02:01:07.470669 fyCursor-0.0.2/
--rw-r--r--   0 danielkay   (503) staff       (20)     1062 2023-05-14 02:45:31.000000 fyCursor-0.0.2/LICENSE
--rw-r--r--   0 danielkay   (503) staff       (20)      294 2023-05-16 02:01:07.470512 fyCursor-0.0.2/PKG-INFO
--rw-r--r--   0 danielkay   (503) staff       (20)       59 2023-05-14 02:46:01.000000 fyCursor-0.0.2/README.md
-drwxr-xr-x   0 danielkay   (503) staff       (20)        0 2023-05-16 02:01:07.460049 fyCursor-0.0.2/fyCursor/
--rw-r--r--   0 danielkay   (503) staff       (20)      589 2023-05-16 01:33:40.000000 fyCursor-0.0.2/fyCursor/__init__.py
--rw-r--r--   0 danielkay   (503) staff       (20)     4510 2023-05-16 01:30:01.000000 fyCursor-0.0.2/fyCursor/core.py
-drwxr-xr-x   0 danielkay   (503) staff       (20)        0 2023-05-16 02:01:07.470123 fyCursor-0.0.2/fyCursor.egg-info/
--rw-r--r--   0 danielkay   (503) staff       (20)      294 2023-05-16 02:01:07.000000 fyCursor-0.0.2/fyCursor.egg-info/PKG-INFO
--rw-r--r--   0 danielkay   (503) staff       (20)      192 2023-05-16 02:01:07.000000 fyCursor-0.0.2/fyCursor.egg-info/SOURCES.txt
--rw-r--r--   0 danielkay   (503) staff       (20)        1 2023-05-16 02:01:07.000000 fyCursor-0.0.2/fyCursor.egg-info/dependency_links.txt
--rw-r--r--   0 danielkay   (503) staff       (20)        9 2023-05-16 02:01:07.000000 fyCursor-0.0.2/fyCursor.egg-info/top_level.txt
--rw-r--r--   0 danielkay   (503) staff       (20)       38 2023-05-16 02:01:07.470721 fyCursor-0.0.2/setup.cfg
--rw-r--r--   0 danielkay   (503) staff       (20)      698 2023-05-16 01:51:46.000000 fyCursor-0.0.2/setup.py
+drwxr-xr-x   0 danielkay   (503) staff       (20)        0 2023-05-16 03:39:00.255984 fyCursor-0.0.3/
+-rw-r--r--   0 danielkay   (503) staff       (20)     1062 2023-05-14 02:45:31.000000 fyCursor-0.0.3/LICENSE
+-rw-r--r--   0 danielkay   (503) staff       (20)      508 2023-05-16 03:39:00.255839 fyCursor-0.0.3/PKG-INFO
+-rw-r--r--   0 danielkay   (503) staff       (20)      272 2023-05-16 03:37:49.000000 fyCursor-0.0.3/README.md
+drwxr-xr-x   0 danielkay   (503) staff       (20)        0 2023-05-16 03:39:00.251340 fyCursor-0.0.3/fyCursor/
+-rw-r--r--   0 danielkay   (503) staff       (20)      590 2023-05-16 03:38:55.000000 fyCursor-0.0.3/fyCursor/__init__.py
+-rw-r--r--   0 danielkay   (503) staff       (20)     4015 2023-05-16 03:19:09.000000 fyCursor-0.0.3/fyCursor/core.py
+drwxr-xr-x   0 danielkay   (503) staff       (20)        0 2023-05-16 03:39:00.255598 fyCursor-0.0.3/fyCursor.egg-info/
+-rw-r--r--   0 danielkay   (503) staff       (20)      508 2023-05-16 03:39:00.000000 fyCursor-0.0.3/fyCursor.egg-info/PKG-INFO
+-rw-r--r--   0 danielkay   (503) staff       (20)      192 2023-05-16 03:39:00.000000 fyCursor-0.0.3/fyCursor.egg-info/SOURCES.txt
+-rw-r--r--   0 danielkay   (503) staff       (20)        1 2023-05-16 03:39:00.000000 fyCursor-0.0.3/fyCursor.egg-info/dependency_links.txt
+-rw-r--r--   0 danielkay   (503) staff       (20)        9 2023-05-16 03:39:00.000000 fyCursor-0.0.3/fyCursor.egg-info/top_level.txt
+-rw-r--r--   0 danielkay   (503) staff       (20)       38 2023-05-16 03:39:00.256032 fyCursor-0.0.3/setup.cfg
+-rw-r--r--   0 danielkay   (503) staff       (20)      698 2023-05-16 01:51:46.000000 fyCursor-0.0.3/setup.py
```

### Comparing `fyCursor-0.0.2/LICENSE` & `fyCursor-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fyCursor-0.0.2/fyCursor/__init__.py` & `fyCursor-0.0.3/fyCursor/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from fyCursor.core import connect, fyCursor
 
 __all__ = ["connect", "fyCursor"]
 __title__ = "fyCursor"
 
-__version__  = "0.0.2"
+__version__  = "0.0.3"
 
 __author__ = "felixyeahh"
 __author_email__ = "<felixyeah@outlook.com>"
 
 __license__ = "MIT"
 __copyright__ = "Copyright 2023 Baffu"
 
@@ -20,7 +20,8 @@
     __author__ = __author__
     __author_email__ = __author_email__
     __license__ = __license__
     __copyright__ = __copyright__
     __description__ = __description__
     __name__ = __name__
 
+
```

### Comparing `fyCursor-0.0.2/fyCursor/core.py` & `fyCursor-0.0.3/fyCursor/core.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,51 +1,32 @@
 import logging
+import sqlite3
 
-from sqlite3 import (
-    Cursor as _cur, 
-    Connection, 
-    ProgrammingError, 
-    connect as _connect
-)
-from typing import Union, Any, Type
+from typing import Union, Any, Type, Optional
 
 def connect(
     database: str, 
-    timeout: float = ..., 
-    detect_types: int = ..., 
-    isolation_level: str | None = ..., 
-    check_same_thread: bool = ..., 
-    factory: Type[Connection] | None = ..., 
-    cached_statements: int = ..., 
-    uri: bool = ...
 ) -> 'fyCursor':
 
-    connection = _connect(
+    connection = sqlite3.connect(
         database=database, 
-        timeout=timeout, 
-        detect_types=detect_types,
-        isolation_level=isolation_level, 
-        check_same_thread=check_same_thread,
-        factory=factory,
-        cached_statements=cached_statements, 
-        uri=uri
     )
     return connection.cursor(fyCursor) #type: ignore
     
 
-class fyCursor(_cur):
+class fyCursor(sqlite3.Cursor):
     """
     Custom `sqlite3.Cursor` that can be used without string query. \n
     I just hate query because it does not have any highlighting in IDE, yeah.
 
     https://github.com/felixyeahh/fyCursor
     """
     def __init__(
         self, 
-        __cursor: Connection, 
+        __cursor: sqlite3.Connection, 
         logger = None
     ) -> None:
         """
         Initialise a cursor.
 
         :param __cursor - sqlite3 connection
         :param logger - custom logger (Optional) 
@@ -73,15 +54,15 @@
 
         :returns: - self
 
         :raises: - `sqlite3.ProgrammingError` if you didn't use `fyCursor.update()` 
         or something similar before this statement
         """
         if not self._query:
-            raise ProgrammingError("You should use something before `add`")
+            raise sqlite3.ProgrammingError("You should use something before `add`")
         column = list(kwargs.keys())[0]
         value = list(kwargs.values())[0]
         self._query += f" SET {column} = {column} + {value}"
         return self
         
 
     def set(self, **kwargs) -> 'fyCursor':
@@ -90,15 +71,15 @@
 
         :returns: - self
 
         :raises: - `sqlite3.ProgrammingError` if you didn't use `fyCursor.update()` 
         or something similar before this statement
         """
         if not self._query:
-            raise ProgrammingError("You should use something before `set`")
+            raise sqlite3.ProgrammingError("You should use something before `set`")
 
         column = list(kwargs.keys())[0]
         value = str(list(kwargs.values())[0])
         self._query += f" SET {column} = {value}"
         return self
         
 
@@ -120,27 +101,27 @@
     def _from(self, table) -> 'fyCursor':
         self._query += f" FROM {table}"
         return self
 
 
     def where(self, **kwargs) -> 'fyCursor':
         if not self._query:
-            raise ProgrammingError("You should use something before `where`")
+            raise sqlite3.ProgrammingError("You should use something before `where`")
         self._query += f" WHERE {list(kwargs.keys())[0]} = \"{list(kwargs.values())[0]}\""
         return self
 
 
     def fetch(self, one: bool = False) -> Union[list, tuple[Any], None]:
         """
         fetch values from cursor query
         
         :param one - if `True` provided, the `cursor.fetchone()` function will be used
         """
         if not self._query:
-            raise ProgrammingError("Nothing to fetch")
+            raise sqlite3.ProgrammingError("Nothing to fetch")
         super().execute(self._query)
         super().connection.commit()
         return super().fetchone() if one else super().fetchall()        
 
 
     def one(self) -> Any:
         """
```

### Comparing `fyCursor-0.0.2/setup.py` & `fyCursor-0.0.3/setup.py`

 * *Files identical despite different names*

