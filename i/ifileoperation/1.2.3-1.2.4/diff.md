# Comparing `tmp/ifileoperation-1.2.3.tar.gz` & `tmp/ifileoperation-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifileoperation-1.2.3.tar", last modified: Sun Mar  5 20:19:00 2023, max compression
+gzip compressed data, was "ifileoperation-1.2.4.tar", last modified: Tue May 16 03:42:13 2023, max compression
```

## Comparing `ifileoperation-1.2.3.tar` & `ifileoperation-1.2.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-03-05 20:19:00.969073 ifileoperation-1.2.3/
--rw-rw-rw-   0        0        0     1514 2023-01-21 01:14:44.000000 ifileoperation-1.2.3/LICENSE
--rw-rw-rw-   0        0        0    10719 2023-03-05 20:19:00.968073 ifileoperation-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     9745 2023-02-06 21:24:02.000000 ifileoperation-1.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-03-05 20:19:00.941548 ifileoperation-1.2.3/ifileoperation/
--rw-rw-rw-   0        0        0      118 2023-03-05 20:10:00.000000 ifileoperation-1.2.3/ifileoperation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-05 20:19:00.961069 ifileoperation-1.2.3/ifileoperation/com/
--rw-rw-rw-   0        0        0      123 2023-01-23 23:38:57.000000 ifileoperation-1.2.3/ifileoperation/com/__init__.py
--rw-rw-rw-   0        0        0     2796 2023-03-05 20:09:21.000000 ifileoperation-1.2.3/ifileoperation/com/common.py
--rw-rw-rw-   0        0        0      354 2023-01-23 23:38:57.000000 ifileoperation-1.2.3/ifileoperation/com/fileoperation.py
--rw-rw-rw-   0        0        0     9918 2023-01-24 21:26:33.000000 ifileoperation-1.2.3/ifileoperation/com/fileoperationprogresssink.py
--rw-rw-rw-   0        0        0     2153 2023-01-24 21:00:56.000000 ifileoperation-1.2.3/ifileoperation/com/filesysbinddata.py
-drwxrwxrwx   0        0        0        0 2023-03-05 20:19:00.966073 ifileoperation-1.2.3/ifileoperation/com/interfaces/
--rw-rw-rw-   0        0        0      130 2023-01-23 23:38:57.000000 ifileoperation-1.2.3/ifileoperation/com/interfaces/__init__.py
--rw-rw-rw-   0        0        0     3311 2023-01-23 23:38:57.000000 ifileoperation-1.2.3/ifileoperation/com/interfaces/ifileoperation.py
--rw-rw-rw-   0        0        0     4293 2023-01-24 21:26:33.000000 ifileoperation-1.2.3/ifileoperation/com/interfaces/ifileoperationprogresssink.py
--rw-rw-rw-   0        0        0      798 2023-01-23 23:38:57.000000 ifileoperation-1.2.3/ifileoperation/com/interfaces/ifilesysbinddata.py
--rw-rw-rw-   0        0        0     1185 2023-01-24 21:26:34.000000 ifileoperation-1.2.3/ifileoperation/com/interfaces/ishellitem.py
--rw-rw-rw-   0        0        0     1903 2023-03-05 20:08:17.000000 ifileoperation-1.2.3/ifileoperation/errors.py
--rw-rw-rw-   0        0        0    10690 2023-03-05 19:23:31.000000 ifileoperation-1.2.3/ifileoperation/fileoperator.py
--rw-rw-rw-   0        0        0    12219 2023-03-05 19:09:03.000000 ifileoperation-1.2.3/ifileoperation/flags.py
-drwxrwxrwx   0        0        0        0 2023-03-05 20:19:00.956551 ifileoperation-1.2.3/ifileoperation.egg-info/
--rw-rw-rw-   0        0        0    10719 2023-03-05 20:19:00.000000 ifileoperation-1.2.3/ifileoperation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      783 2023-03-05 20:19:00.000000 ifileoperation-1.2.3/ifileoperation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-05 20:19:00.000000 ifileoperation-1.2.3/ifileoperation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-03-05 20:19:00.000000 ifileoperation-1.2.3/ifileoperation.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-03-05 20:19:00.000000 ifileoperation-1.2.3/ifileoperation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1714 2023-01-24 21:00:56.000000 ifileoperation-1.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-05 20:19:00.969073 ifileoperation-1.2.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-05 20:19:00.967072 ifileoperation-1.2.3/tests/
--rw-rw-rw-   0        0        0       30 2023-02-01 10:05:05.000000 ifileoperation-1.2.3/tests/test_ifileoperation.py
+drwxrwxrwx   0        0        0        0 2023-05-16 03:42:13.706300 ifileoperation-1.2.4/
+-rw-rw-rw-   0        0        0     1514 2023-01-21 01:14:44.000000 ifileoperation-1.2.4/LICENSE
+-rw-rw-rw-   0        0        0    10719 2023-05-16 03:42:13.704970 ifileoperation-1.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     9745 2023-02-06 21:24:02.000000 ifileoperation-1.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 03:42:13.625270 ifileoperation-1.2.4/ifileoperation/
+-rw-rw-rw-   0        0        0      118 2023-05-16 01:34:52.000000 ifileoperation-1.2.4/ifileoperation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 03:42:13.672236 ifileoperation-1.2.4/ifileoperation/com/
+-rw-rw-rw-   0        0        0      123 2023-01-23 23:38:57.000000 ifileoperation-1.2.4/ifileoperation/com/__init__.py
+-rw-rw-rw-   0        0        0     2796 2023-05-16 01:33:55.000000 ifileoperation-1.2.4/ifileoperation/com/common.py
+-rw-rw-rw-   0        0        0      354 2023-01-23 23:38:57.000000 ifileoperation-1.2.4/ifileoperation/com/fileoperation.py
+-rw-rw-rw-   0        0        0     9918 2023-01-24 21:26:33.000000 ifileoperation-1.2.4/ifileoperation/com/fileoperationprogresssink.py
+-rw-rw-rw-   0        0        0     2153 2023-01-24 21:00:56.000000 ifileoperation-1.2.4/ifileoperation/com/filesysbinddata.py
+drwxrwxrwx   0        0        0        0 2023-05-16 03:42:13.699455 ifileoperation-1.2.4/ifileoperation/com/interfaces/
+-rw-rw-rw-   0        0        0      130 2023-01-23 23:38:57.000000 ifileoperation-1.2.4/ifileoperation/com/interfaces/__init__.py
+-rw-rw-rw-   0        0        0     3311 2023-01-23 23:38:57.000000 ifileoperation-1.2.4/ifileoperation/com/interfaces/ifileoperation.py
+-rw-rw-rw-   0        0        0     4293 2023-01-24 21:26:33.000000 ifileoperation-1.2.4/ifileoperation/com/interfaces/ifileoperationprogresssink.py
+-rw-rw-rw-   0        0        0      798 2023-01-23 23:38:57.000000 ifileoperation-1.2.4/ifileoperation/com/interfaces/ifilesysbinddata.py
+-rw-rw-rw-   0        0        0     1185 2023-01-24 21:26:34.000000 ifileoperation-1.2.4/ifileoperation/com/interfaces/ishellitem.py
+-rw-rw-rw-   0        0        0     1903 2023-05-16 01:33:55.000000 ifileoperation-1.2.4/ifileoperation/errors.py
+-rw-rw-rw-   0        0        0    11034 2023-05-16 01:45:06.000000 ifileoperation-1.2.4/ifileoperation/fileoperator.py
+-rw-rw-rw-   0        0        0    12219 2023-05-16 01:33:55.000000 ifileoperation-1.2.4/ifileoperation/flags.py
+drwxrwxrwx   0        0        0        0 2023-05-16 03:42:13.643261 ifileoperation-1.2.4/ifileoperation.egg-info/
+-rw-rw-rw-   0        0        0    10719 2023-05-16 03:42:13.000000 ifileoperation-1.2.4/ifileoperation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      783 2023-05-16 03:42:13.000000 ifileoperation-1.2.4/ifileoperation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 03:42:13.000000 ifileoperation-1.2.4/ifileoperation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-05-16 03:42:13.000000 ifileoperation-1.2.4/ifileoperation.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-16 03:42:13.000000 ifileoperation-1.2.4/ifileoperation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1714 2023-01-24 21:00:56.000000 ifileoperation-1.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-16 03:42:13.706300 ifileoperation-1.2.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-16 03:42:13.703959 ifileoperation-1.2.4/tests/
+-rw-rw-rw-   0        0        0      849 2023-05-16 01:34:17.000000 ifileoperation-1.2.4/tests/test_ifileoperation.py
```

### Comparing `ifileoperation-1.2.3/LICENSE` & `ifileoperation-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ifileoperation-1.2.3/PKG-INFO` & `ifileoperation-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifileoperation
-Version: 1.2.3
+Version: 1.2.4
 Summary: Python wrapper for using Win32's IFileOperation for manipulating the filesystem.
 Author: lojack5
 License: BSD 3-Clause
 Project-URL: Homepage, https://github.com/lojack5/IFileOperation
 Project-URL: Bug Tracker, https://github.com/lojack5/IFileOperation/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `ifileoperation-1.2.3/README.md` & `ifileoperation-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `ifileoperation-1.2.3/ifileoperation/com/common.py` & `ifileoperation-1.2.4/ifileoperation/com/common.py`

 * *Files identical despite different names*

### Comparing `ifileoperation-1.2.3/ifileoperation/com/fileoperationprogresssink.py` & `ifileoperation-1.2.4/ifileoperation/com/fileoperationprogresssink.py`

 * *Files identical despite different names*

### Comparing `ifileoperation-1.2.3/ifileoperation/com/filesysbinddata.py` & `ifileoperation-1.2.4/ifileoperation/com/filesysbinddata.py`

 * *Files identical despite different names*

### Comparing `ifileoperation-1.2.3/ifileoperation/com/interfaces/ifileoperation.py` & `ifileoperation-1.2.4/ifileoperation/com/interfaces/ifileoperation.py`

 * *Files identical despite different names*

### Comparing `ifileoperation-1.2.3/ifileoperation/com/interfaces/ifileoperationprogresssink.py` & `ifileoperation-1.2.4/ifileoperation/com/interfaces/ifileoperationprogresssink.py`

 * *Files identical despite different names*

### Comparing `ifileoperation-1.2.3/ifileoperation/com/interfaces/ifilesysbinddata.py` & `ifileoperation-1.2.4/ifileoperation/com/interfaces/ifilesysbinddata.py`

 * *Files identical despite different names*

### Comparing `ifileoperation-1.2.3/ifileoperation/com/interfaces/ishellitem.py` & `ifileoperation-1.2.4/ifileoperation/com/interfaces/ishellitem.py`

 * *Files identical despite different names*

### Comparing `ifileoperation-1.2.3/ifileoperation/errors.py` & `ifileoperation-1.2.4/ifileoperation/errors.py`

 * *Files identical despite different names*

### Comparing `ifileoperation-1.2.3/ifileoperation/fileoperator.py` & `ifileoperation-1.2.4/ifileoperation/fileoperator.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,16 @@
     'FileOperator',
 ]
 
 from os import PathLike, fspath
 from pathlib import Path
 from typing import Iterable, TypeAlias
 
+import pythoncom
+
 from .com import (
     FileOperation,
     FileOperationProgressSink,
     convert_exceptions,
     parse_filename,
 )
 from .errors import IFileOperationError, UnexpectedError
@@ -106,15 +108,14 @@
         | FileOperationFlags.NO_CONFIRM_MKDIR
         | FileOperationFlags.SHOWELEVATIONPROMPT
     )
     """Flags to suppress all dialogs (as if Yes to All was selected), except for a UAC
     prompt if necessary.  If errors occur, the operation will fail immediately.
     """
 
-    @convert_exceptions
     def __init__(
         self,
         parent=None,
         flags: FileOperationFlags | None = DEFAULT_FLAGS,
         *,
         commit_on_exit: bool = False,
     ):
@@ -126,43 +127,52 @@
 
         :param parent: A HANDLE to the window that should own any dialog boxes that are
             displayed. Also supports wx.Window instances.
         :param flags: The FileOperationFlags to use for the operations.
         :param commit_on_exit: If True (default: False), `commit` will be performed
             automatically when the with block is exited if no exceptions were raised.
         """
-        self.ifo = FileOperation()
-        self.sink = ProgressSink()
-        self.sink_cookie = self.ifo.Advise(self.sink.com_ptr)
+        self.entered = False
         if parent is not None:
             try:
                 parent = parent.GetHandle()  # wx.Window
             except AttributeError:
                 pass
-        if parent is not None:
-            self.ifo.SetOwnerWindow(parent)
-        if flags is not None:
-            self.ifo.SetOperationFlags(int(flags))
+        self._parent = parent
+        self._flags = flags
         self.commit_on_exit = commit_on_exit
-        self.entered = False
-        self._operations_queued = False
 
+    @convert_exceptions
     def __enter__(self):
         if self.entered:
             raise IFileOperationError(f'{type(self).__name__} is not reentrant')
         else:
             self.entered = True
+            pythoncom.CoInitializeEx(pythoncom.COINIT_APARTMENTTHREADED)
+            self.ifo = FileOperation()
+            self.sink = ProgressSink()
+            self.sink_cookie = self.ifo.Advise(self.sink.com_ptr)
+            if self._parent is not None:
+                self.ifo.SetOwnerWindow(self._parent)
+            if self._flags is not None:
+                self.ifo.SetOperationFlags(int(self._flags))
+            self._operations_queued = False
             return self
 
+    @convert_exceptions
     def __exit__(self, exc_type, exc_value, exc_traceback):
         if self.commit_on_exit and not exc_type:
             self.commit()
             self.ifo.Unadvise(self.sink_cookie)
+        pythoncom.CoUninitialize()
         # Delete the IFileOperation instance, so reentrance will raise an error
         del self.ifo
+        del self.sink
+        del self.sink_cookie
+        self.entered = False
 
     @convert_exceptions
     def move_file(
         self, source: StrPath, destination: StrPath, new_name: str | None = None
     ) -> None:
         """Schedule to move a file from `source` to `destination`.  Optionally rename
         the file in the process. NOTE: Windows performs a move to a different logical
```

### Comparing `ifileoperation-1.2.3/ifileoperation/flags.py` & `ifileoperation-1.2.4/ifileoperation/flags.py`

 * *Files identical despite different names*

### Comparing `ifileoperation-1.2.3/ifileoperation.egg-info/PKG-INFO` & `ifileoperation-1.2.4/ifileoperation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifileoperation
-Version: 1.2.3
+Version: 1.2.4
 Summary: Python wrapper for using Win32's IFileOperation for manipulating the filesystem.
 Author: lojack5
 License: BSD 3-Clause
 Project-URL: Homepage, https://github.com/lojack5/IFileOperation
 Project-URL: Bug Tracker, https://github.com/lojack5/IFileOperation/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `ifileoperation-1.2.3/ifileoperation.egg-info/SOURCES.txt` & `ifileoperation-1.2.4/ifileoperation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ifileoperation-1.2.3/pyproject.toml` & `ifileoperation-1.2.4/pyproject.toml`

 * *Files identical despite different names*

