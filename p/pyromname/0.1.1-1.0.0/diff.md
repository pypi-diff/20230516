# Comparing `tmp/pyromname-0.1.1.tar.gz` & `tmp/pyromname-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyromname-0.1.1.tar", max compression
+gzip compressed data, was "pyromname-1.0.0.tar", max compression
```

## Comparing `pyromname-0.1.1.tar` & `pyromname-1.0.0.tar`

### file list

```diff
@@ -1,9 +1,14 @@
--rw-r--r--   0        0        0      540 2023-03-20 21:26:38.985544 pyromname-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       22 2023-03-03 15:39:48.486029 pyromname-0.1.1/pyromname/__init__.py
--rw-r--r--   0        0        0     8913 2023-03-19 15:15:40.726311 pyromname-0.1.1/pyromname/cli.py
--rw-r--r--   0        0        0      669 2023-03-08 21:31:52.971045 pyromname-0.1.1/pyromname/crc.py
--rw-r--r--   0        0        0     5144 2023-03-08 23:10:38.371186 pyromname-0.1.1/pyromname/file.py
--rw-r--r--   0        0        0      975 2023-03-19 14:57:57.858345 pyromname-0.1.1/pyromname/io.py
--rw-r--r--   0        0        0     2095 2023-03-08 22:53:46.455162 pyromname-0.1.1/pyromname/rom_database.py
--rw-r--r--   0        0        0     3588 2023-03-03 16:27:24.682097 pyromname-0.1.1/pyromname/seven_zip.py
--rw-r--r--   0        0        0      471 1970-01-01 00:00:00.000000 pyromname-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      582 2023-05-15 20:37:05.131495 pyromname-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-15 20:17:27.028972 pyromname-1.0.0/pyromname/__init__.py
+-rw-r--r--   0        0        0    10545 2023-05-09 19:35:46.526561 pyromname-1.0.0/pyromname/cli.py
+-rw-r--r--   0        0        0      671 2023-05-15 20:17:27.084973 pyromname-1.0.0/pyromname/crc.py
+-rw-r--r--   0        0        0     6228 2023-05-15 20:17:27.996994 pyromname-1.0.0/pyromname/file.py
+-rw-r--r--   0        0        0      974 2023-05-15 20:17:27.212976 pyromname-1.0.0/pyromname/io.py
+-rw-r--r--   0        0        0     8556 2023-05-15 20:17:27.996994 pyromname-1.0.0/pyromname/renascene.py
+-rw-r--r--   0        0        0     2353 2023-05-15 22:02:08.572879 pyromname-1.0.0/pyromname/rom_database.py
+-rw-r--r--   0        0        0     1177 2023-05-15 21:41:05.822587 pyromname-1.0.0/pyromname/rom_database_3dsdb.py
+-rw-r--r--   0        0        0     1605 2023-05-15 21:44:30.227787 pyromname-1.0.0/pyromname/rom_database_dat.py
+-rw-r--r--   0        0        0     3588 2023-03-03 16:27:24.682097 pyromname-1.0.0/pyromname/seven_zip.py
+-rw-r--r--   0        0        0      560 2023-05-15 20:17:27.600985 pyromname-1.0.0/pyromname/ui.py
+-rw-r--r--   0        0        0     2190 2023-05-09 19:36:54.964083 pyromname-1.0.0/pyromname/zip.py
+-rw-r--r--   0        0        0      471 1970-01-01 00:00:00.000000 pyromname-1.0.0/PKG-INFO
```

### Comparing `pyromname-0.1.1/pyproject.toml` & `pyromname-1.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyromname"
-version = "0.1.1"
+version = "1.0.0"
 description = "pyromname is a command line tool to manage roms."
 authors = ["Mathieu <git@bigbisous.org>"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 colorama = "^0.4.6"
 defusedxml = "^0.7.1"
@@ -18,8 +18,9 @@
 pytest-cov = "^4.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-pyromname = "pyromname.cli:main"
+pyromname = "pyromname.cli:main"
+pyrenascene = "pyromname.renascene:main"
```

### Comparing `pyromname-0.1.1/pyromname/crc.py` & `pyromname-1.0.0/pyromname/crc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import zlib
 
 
 def crc_from_file(fname, fix_3ds_header=False):
-
     prev = 0
     data = b""
     with open(fname, "rb") as filep:
         #  Replace 0x48 bytes with 0xFF at position 4608
         if fix_3ds_header:
             upper = 0x1200 + 0x48
             lower = 0x1200
@@ -14,9 +13,9 @@
             lchunk = bytearray(chunk)
             lchunk[lower:upper] = [0xFF] * 0x48
             data = data + bytes(lchunk)
             prev = zlib.crc32(bytes(lchunk), prev)
 
         for chunk in iter(lambda: filep.read(4096), b""):
             prev = zlib.crc32(chunk, prev)
-            #data = data + chunk
-    return f"{prev & 0xFFFFFFFF:08X}" #, data
+            # data = data + chunk
+    return f"{prev & 0xFFFFFFFF:08X}"  # , data
```

### Comparing `pyromname-0.1.1/pyromname/file.py` & `pyromname-1.0.0/pyromname/file.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,22 +13,20 @@
 class FileException(Exception):
     def __init__(self, message):
         self.message = message
         super().__init__(message)
 
 
 class FileStatus(Enum):
-
     SUCCESS = (0,)
     PARTIAL_SUCCESS = (1,)
     FAILURE = 2
 
 
 class File:
-
     rom_database: pyromname.rom_database.RomDatabase
 
     def __init__(self, file):
         self.file = file
 
     @property
     @abc.abstractmethod
@@ -38,53 +36,76 @@
     @abc.abstractmethod
     def extract(
         self, destination_dir
     ) -> Tuple[FileStatus, List[Tuple[str, str, Tuple[str, str], str]]]:
         pass
 
     def check(self):
+        def normalize(string):
+            return (
+                string.replace("United Kingdom", "Europe")
+                .replace("Germany", "Europe")
+                .replace("Sega", "SEGA")
+                .replace(" (Not For Resale)", "")
+                .replace("(USA, Australia)", "(USA)")
+            )
+
         status, content = self.content
         if status == FileStatus.FAILURE:
-            return False
+            return FileStatus.FAILURE
         if len(content) != 1:
-            return False
-        for (filename, _, name_in_db) in content:
+            return FileStatus.FAILURE
+        perfect = False
+        for filename, _, name_in_db in content:
             if name_in_db:
                 name, _ = name_in_db
                 filename_only = os.path.basename(filename)
-                if name != filename_only:
-                    return False
+                if name == filename_only:
+                    perfect = True
+                elif normalize(name) == filename_only:
+                    print(f"{name} / {filename_only}")
+                    perfect = False
+                else:
+                    print(f"{name} / {filename_only}")
+                    print(f"{normalize(name)} / {filename_only}")
+                    return FileStatus.FAILURE
             else:
-                return False
+                return FileStatus.FAILURE
 
-        return True
+        return FileStatus.SUCCESS if perfect else FileStatus.PARTIAL_SUCCESS
 
 
 class SingleFile(File):
-
-    @functools.cached_property
-    def content(self):
+    def _content(self, fix_3ds_header=False):
         try:
-            crc = pyromname.crc.crc_from_file(self.file)
+            crc = pyromname.crc.crc_from_file(self.file, fix_3ds_header)
         except (IOError, OSError) as exception:
             raise FileException(f"Unable to read {self.file}") from exception
 
-        name_in_db = self.rom_database.name_by_crc(crc)
+        name_in_db = self.rom_database.name_by_crc(crc, self.file)
         if name_in_db:
             return (FileStatus.SUCCESS, [(self.file, crc, name_in_db)])
         else:
+            _, file_extension = os.path.splitext(self.file)
+            if file_extension == ".3ds" and not fix_3ds_header:
+                print("Try to fix header ...")
+                return self._content(True)
             return (FileStatus.FAILURE, [(self.file, crc, name_in_db)])
 
+    @functools.cached_property
+    def content(self):
+        return self._content()
+
     def extract(self, destination_dir):
-        result = [] # type: List[Tuple[str, str, str, str]]
+        result = []  # type: List[Tuple[str, str, str, str]]
         status, content = self.content
         if status == FileStatus.FAILURE:
             return (FileStatus.FAILURE, result)
         try:
-            for (filename, crc, name_in_db) in content:
+            for filename, crc, name_in_db in content:
                 if name_in_db:
                     name, _ = name_in_db
                     pyromname.io.copy_to_dir(filename, destination_dir, name)
                     result.append((filename, crc, name_in_db, name))
         except (IOError, OSError) as exception:
             raise FileException(f"Unable to read {self.file}") from exception
 
@@ -94,22 +115,22 @@
 class ArchiveFile(File):
     def __init__(self, file: str):
         self.archive = pyromname.seven_zip.SevenZip(file)
         super().__init__(file)
 
     @functools.cached_property
     def content(self):
-        result = [] # type: List[Tuple[str, str, str]]
+        result = []  # type: List[Tuple[str, str, str]]
         unknown_content = 0
         try:
             if not self.archive.test():
                 return FileStatus.FAILURE, result
 
-            for (filename, crc) in self.archive.content() or []:
-                name_in_db = self.rom_database.name_by_crc(crc)
+            for filename, crc in self.archive.content() or []:
+                name_in_db = self.rom_database.name_by_crc(crc, self.file)
                 result.append((filename, crc, name_in_db))
                 if not name_in_db:
                     unknown_content += 1
 
             if len(result) == 0 or unknown_content == len(result):
                 return (FileStatus.FAILURE, result)
             if unknown_content > 0:
@@ -118,30 +139,30 @@
                 return (FileStatus.SUCCESS, result)
         except pyromname.seven_zip.SevenZipException as exception:
             raise FileException(
                 f"{exception.message} ({exception.command})"
             ) from exception
 
     def extract(self, destination_dir):
-        result = [] # type: List[Tuple[str, str, str|None, str|None]]
+        result = []  # type: List[Tuple[str, str, str|None, str|None]]
         unknown_content = 0
         status, content = self.content
 
         try:
-            for (filename, crc, name_in_db) in content:
+            for filename, crc, name_in_db in content:
                 if name_in_db:
                     name, _ = name_in_db
                     if self.archive.extract_to_specific_filename(
                         filename, destination_dir, name
                     ):
                         result.append((filename, crc, name_in_db, name))
                     else:
                         result.append((filename, crc, name_in_db, None))
                         raise FileException(
-                            f"Unable to extract '{filename}' in {self.file}"            
+                            f"Unable to extract '{filename}' in {self.file}"
                         )
                 else:
                     result.append((filename, crc, None, None))
                     unknown_content += 1
         except pyromname.seven_zip.SevenZipException as exception:
             raise FileException(
                 f"{exception.message} ({exception.command})"
```

### Comparing `pyromname-0.1.1/pyromname/io.py` & `pyromname-1.0.0/pyromname/io.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,17 +11,18 @@
     destination_file = os.path.join(destination_dir, filename)
     if os.path.exists(destination_file):
         number = number + 1
         return get_destination_filename(destination_dir, destination_filename, number)
     else:
         return destination_file
 
+
 def get_original_filename(filename):
-    (name, ext) = os.path.splitext(filename)
-    return re.sub(f"(_\\d+){ext}", f"{ext}", filename)
+    (_, ext) = os.path.splitext(filename)
+    return re.sub(f"(_\\d+){ext}$", f"{ext}", filename)
 
 
 def move_to_dir(file, destination_dir, destination_filename):
     shutil.move(file, get_destination_filename(destination_dir, destination_filename))
 
 
 def copy_to_dir(file, destination_dir, destination_filename):
```

### Comparing `pyromname-0.1.1/pyromname/seven_zip.py` & `pyromname-1.0.0/pyromname/seven_zip.py`

 * *Files identical despite different names*

