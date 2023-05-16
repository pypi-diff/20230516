# Comparing `tmp/bloboluni-1.1.0.tar.gz` & `tmp/bloboluni-2.0.0.tar.gz`

## Comparing `bloboluni-1.1.0.tar` & `bloboluni-2.0.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 bloboluni-1.1.0/GitVersion.yml
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 bloboluni-1.1.0/test.py
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 bloboluni-1.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bloboluni-1.1.0/bloboluni/__init__.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 bloboluni-1.1.0/bloboluni/serializers.py
--rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 bloboluni-1.1.0/bloboluni/storage.py
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 bloboluni-1.1.0/.gitignore
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 bloboluni-1.1.0/LICENSE
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 bloboluni-1.1.0/README.md
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 bloboluni-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 bloboluni-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 bloboluni-2.0.0/GitVersion.yml
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 bloboluni-2.0.0/test.py
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 bloboluni-2.0.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 bloboluni-2.0.0/bloboluni/__init__.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 bloboluni-2.0.0/bloboluni/serializers.py
+-rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 bloboluni-2.0.0/bloboluni/storage.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 bloboluni-2.0.0/.gitignore
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 bloboluni-2.0.0/LICENSE
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 bloboluni-2.0.0/README.md
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 bloboluni-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 bloboluni-2.0.0/PKG-INFO
```

### Comparing `bloboluni-1.1.0/test.py` & `bloboluni-2.0.0/test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from bloboluni.storage import BlobStorage, JsonSerializer
+from bloboluni import BlobStorage, JsonBlobStorage, JsonPickleBlobStorage
 import os, uuid
 from dotenv import load_dotenv
 load_dotenv()
 
 @dataclass
 class MyProfession:
     name: str
@@ -23,16 +23,15 @@
     def amethod(self):
         return "A method"
 
 if __name__ == "__main__":
     data = MyClass("blob", 30, MyProfession("Developer", "A developer"))
 
     connectionstring = os.environ["AZURE_STORAGE_CONNECTION_STRING"]
-    serializer = JsonSerializer()
-    storage = BlobStorage(connectionstring, "mycontainer", serializer)
+    storage = BlobStorage(connectionstring, "mycontainer")
     
     key = uuid.uuid4().hex
     blob = storage.get(key)
     assert blob is None
     storage.upsert(key, data)
     blob = storage.get(key)
     assert blob is not None
```

### Comparing `bloboluni-1.1.0/.github/workflows/python-publish.yml` & `bloboluni-2.0.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `bloboluni-1.1.0/bloboluni/serializers.py` & `bloboluni-2.0.0/bloboluni/serializers.py`

 * *Files identical despite different names*

### Comparing `bloboluni-1.1.0/bloboluni/storage.py` & `bloboluni-2.0.0/bloboluni/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from azure.storage.blob import BlobClient, ContainerClient
 from typing import Generic, TypeVar
 from .serializers import ISerializer, JsonSerializer, JsonPickleSerializer
 
 T = TypeVar('T')
     
 class BlobStorage(Generic[T]):
-    def __init__(self, connectionstring: str, container: str, serializer: ISerializer = None):
+    def __init__(self, connectionstring: str, container: str, serializer: ISerializer = JsonPickleSerializer()):
         self.connectionstring = connectionstring
         self.container = container
         self.serializer = serializer
         
     def get(self, key: str) -> None | T:
         '''Fetch a blob from the storage account. If the blob does not exist, None is returned. If a serializer is provided, the blob is deserialized before being returned.'''
         blob = BlobClient.from_connection_string(conn_str=self.connectionstring, container_name=self.container, blob_name=key)
```

### Comparing `bloboluni-1.1.0/.gitignore` & `bloboluni-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `bloboluni-1.1.0/LICENSE` & `bloboluni-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bloboluni-1.1.0/README.md` & `bloboluni-2.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 ## Installation
 ````
 pip install bloboluni
 ````
 
 ## Usage
 ````python
-from bloboluni.storage import JsonPickleBlobStorage
+from bloboluni import BlobStorage
 from mymodels import Person, Profession
 
 if __name__ == "__main__":
     alex = Person("Alex", 27, Profession("Developer", "A developer"))
 
     # Create a storage client
-    storage = JsonPickleBlobStorage(connectionstring="...", container="mycontainer")
+    storage = BlobStorage(connectionstring="...", container="mycontainer")
 
     # Store some data
     storage.upsert(key="Alex", alex)
 
     # Read some data
     sam = storage.get(key="Sam") # Returns instance of Person or None
```

### Comparing `bloboluni-1.1.0/pyproject.toml` & `bloboluni-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bloboluni"
-version = "1.1.0"
+version = "2.0.0"
 description = "A simple package for storing and retrieving blobs of data from Azure Blob Storage"
 authors = [
   { name = "Martin Moan", email = "martin.moan1@gmail.com" },
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
 classifiers = [
```

### Comparing `bloboluni-1.1.0/PKG-INFO` & `bloboluni-2.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bloboluni
-Version: 1.1.0
+Version: 2.0.0
 Summary: A simple package for storing and retrieving blobs of data from Azure Blob Storage
 Project-URL: Homepage, https://github.com/MartinMoan/blobstorage
 Project-URL: Bug Tracker, https://github.com/MartinMoan/blobstorage/issues
 Author-email: Martin Moan <martin.moan1@gmail.com>
 License: Copyright (c) 2023 Martin Hoff Moan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -41,22 +41,22 @@
 ## Installation
 ````
 pip install bloboluni
 ````
 
 ## Usage
 ````python
-from bloboluni.storage import JsonPickleBlobStorage
+from bloboluni import BlobStorage
 from mymodels import Person, Profession
 
 if __name__ == "__main__":
     alex = Person("Alex", 27, Profession("Developer", "A developer"))
 
     # Create a storage client
-    storage = JsonPickleBlobStorage(connectionstring="...", container="mycontainer")
+    storage = BlobStorage(connectionstring="...", container="mycontainer")
 
     # Store some data
     storage.upsert(key="Alex", alex)
 
     # Read some data
     sam = storage.get(key="Sam") # Returns instance of Person or None
```

