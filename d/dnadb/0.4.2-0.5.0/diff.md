# Comparing `tmp/dnadb-0.4.2.tar.gz` & `tmp/dnadb-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnadb-0.4.2.tar", last modified: Mon May 15 03:37:00 2023, max compression
+gzip compressed data, was "dnadb-0.5.0.tar", last modified: Tue May 16 01:20:49 2023, max compression
```

## Comparing `dnadb-0.4.2.tar` & `dnadb-0.5.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-15 03:37:00.287145 dnadb-0.4.2/
--rw-r--r--   0 dwl2x     (1000) users      (100)     1070 2023-03-27 04:24:58.000000 dnadb-0.4.2/LICENSE
--rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-05-15 03:37:00.287145 dnadb-0.4.2/PKG-INFO
--rw-r--r--   0 dwl2x     (1000) users      (100)       43 2023-03-27 04:27:38.000000 dnadb-0.4.2/README.md
--rw-r--r--   0 dwl2x     (1000) users      (100)      742 2023-05-15 03:35:15.000000 dnadb-0.4.2/pyproject.toml
--rw-r--r--   0 dwl2x     (1000) users      (100)       38 2023-05-15 03:37:00.287145 dnadb-0.4.2/setup.cfg
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-15 03:37:00.287145 dnadb-0.4.2/src/
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-15 03:37:00.287145 dnadb-0.4.2/src/dnadb/
--rw-r--r--   0 dwl2x     (1000) users      (100)       22 2023-05-15 03:36:19.000000 dnadb-0.4.2/src/dnadb/__init__.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-15 03:37:00.287145 dnadb-0.4.2/src/dnadb/datasets/
--rw-r--r--   0 dwl2x     (1000) users      (100)      255 2023-03-27 05:49:34.000000 dnadb-0.4.2/src/dnadb/datasets/__init__.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     7303 2023-05-14 15:51:22.000000 dnadb-0.4.2/src/dnadb/datasets/dataset.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     1392 2023-04-03 19:22:40.000000 dnadb-0.4.2/src/dnadb/datasets/greengenes.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-15 03:37:00.287145 dnadb-0.4.2/src/dnadb/datasets/silva/
--rw-r--r--   0 dwl2x     (1000) users      (100)     5538 2023-05-14 21:04:53.000000 dnadb-0.4.2/src/dnadb/datasets/silva/__init__.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     6022 2023-05-15 03:13:49.000000 dnadb-0.4.2/src/dnadb/datasets/silva/taxonomy_map.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     2234 2023-05-10 12:52:14.000000 dnadb-0.4.2/src/dnadb/db.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     4815 2023-05-11 20:35:23.000000 dnadb-0.4.2/src/dnadb/dna.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     5208 2023-05-11 01:32:34.000000 dnadb-0.4.2/src/dnadb/fasta.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     5969 2023-05-11 01:44:43.000000 dnadb-0.4.2/src/dnadb/fastq.py
--rw-r--r--   0 dwl2x     (1000) users      (100)        0 2023-05-09 22:29:41.000000 dnadb-0.4.2/src/dnadb/otu.py
--rw-r--r--   0 dwl2x     (1000) users      (100)    19190 2023-05-15 01:07:27.000000 dnadb-0.4.2/src/dnadb/taxonomy.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     1473 2023-04-01 17:43:32.000000 dnadb-0.4.2/src/dnadb/utils.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-15 03:37:00.287145 dnadb-0.4.2/src/dnadb.egg-info/
--rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-05-15 03:37:00.000000 dnadb-0.4.2/src/dnadb.egg-info/PKG-INFO
--rw-r--r--   0 dwl2x     (1000) users      (100)      519 2023-05-15 03:37:00.000000 dnadb-0.4.2/src/dnadb.egg-info/SOURCES.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)        1 2023-05-15 03:37:00.000000 dnadb-0.4.2/src/dnadb.egg-info/dependency_links.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)       64 2023-05-15 03:37:00.000000 dnadb-0.4.2/src/dnadb.egg-info/requires.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)        6 2023-05-15 03:37:00.000000 dnadb-0.4.2/src/dnadb.egg-info/top_level.txt
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-16 01:20:49.209688 dnadb-0.5.0/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1070 2023-03-27 04:24:58.000000 dnadb-0.5.0/LICENSE
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-05-16 01:20:49.209688 dnadb-0.5.0/PKG-INFO
+-rw-r--r--   0 dwl2x     (1000) users      (100)       43 2023-03-27 04:27:38.000000 dnadb-0.5.0/README.md
+-rw-r--r--   0 dwl2x     (1000) users      (100)      742 2023-05-15 22:10:37.000000 dnadb-0.5.0/pyproject.toml
+-rw-r--r--   0 dwl2x     (1000) users      (100)       38 2023-05-16 01:20:49.209688 dnadb-0.5.0/setup.cfg
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-16 01:20:49.205688 dnadb-0.5.0/src/
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-16 01:20:49.209688 dnadb-0.5.0/src/dnadb/
+-rw-r--r--   0 dwl2x     (1000) users      (100)       22 2023-05-15 22:10:42.000000 dnadb-0.5.0/src/dnadb/__init__.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-16 01:20:49.209688 dnadb-0.5.0/src/dnadb/datasets/
+-rw-r--r--   0 dwl2x     (1000) users      (100)      255 2023-03-27 05:49:34.000000 dnadb-0.5.0/src/dnadb/datasets/__init__.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     7303 2023-05-14 15:51:22.000000 dnadb-0.5.0/src/dnadb/datasets/dataset.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1392 2023-04-03 19:22:40.000000 dnadb-0.5.0/src/dnadb/datasets/greengenes.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-16 01:20:49.209688 dnadb-0.5.0/src/dnadb/datasets/silva/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     5538 2023-05-14 21:04:53.000000 dnadb-0.5.0/src/dnadb/datasets/silva/__init__.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     6022 2023-05-15 03:13:49.000000 dnadb-0.5.0/src/dnadb/datasets/silva/taxonomy_map.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     2234 2023-05-10 12:52:14.000000 dnadb-0.5.0/src/dnadb/db.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     4815 2023-05-11 20:35:23.000000 dnadb-0.5.0/src/dnadb/dna.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     5232 2023-05-15 04:51:39.000000 dnadb-0.5.0/src/dnadb/fasta.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     6017 2023-05-15 04:51:34.000000 dnadb-0.5.0/src/dnadb/fastq.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)        0 2023-05-09 22:29:41.000000 dnadb-0.5.0/src/dnadb/otu.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)    20115 2023-05-16 00:50:00.000000 dnadb-0.5.0/src/dnadb/taxonomy.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1473 2023-04-01 17:43:32.000000 dnadb-0.5.0/src/dnadb/utils.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-16 01:20:49.209688 dnadb-0.5.0/src/dnadb.egg-info/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-05-16 01:20:49.000000 dnadb-0.5.0/src/dnadb.egg-info/PKG-INFO
+-rw-r--r--   0 dwl2x     (1000) users      (100)      519 2023-05-16 01:20:49.000000 dnadb-0.5.0/src/dnadb.egg-info/SOURCES.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)        1 2023-05-16 01:20:49.000000 dnadb-0.5.0/src/dnadb.egg-info/dependency_links.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)       64 2023-05-16 01:20:49.000000 dnadb-0.5.0/src/dnadb.egg-info/requires.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)        6 2023-05-16 01:20:49.000000 dnadb-0.5.0/src/dnadb.egg-info/top_level.txt
```

### Comparing `dnadb-0.4.2/LICENSE` & `dnadb-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dnadb-0.4.2/PKG-INFO` & `dnadb-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnadb
-Version: 0.4.2
+Version: 0.5.0
 Summary: A library for handling DNA files.
 Author-email: David Ludwig <davidludwigii@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 DLii-Research
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dnadb-0.4.2/pyproject.toml` & `dnadb-0.5.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dnadb"
-version = "0.4.2"
+version = "0.5.0"
 authors = [
   { name="David Ludwig", email="davidludwigii@gmail.com" },
 ]
 description = "A library for handling DNA files."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `dnadb-0.4.2/src/dnadb/datasets/dataset.py` & `dnadb-0.5.0/src/dnadb/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.4.2/src/dnadb/datasets/greengenes.py` & `dnadb-0.5.0/src/dnadb/datasets/greengenes.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.4.2/src/dnadb/datasets/silva/__init__.py` & `dnadb-0.5.0/src/dnadb/datasets/silva/__init__.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.4.2/src/dnadb/datasets/silva/taxonomy_map.py` & `dnadb-0.5.0/src/dnadb/datasets/silva/taxonomy_map.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.4.2/src/dnadb/db.py` & `dnadb-0.5.0/src/dnadb/db.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.4.2/src/dnadb/dna.py` & `dnadb-0.5.0/src/dnadb/dna.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.4.2/src/dnadb/fasta.py` & `dnadb-0.5.0/src/dnadb/fasta.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from dataclasses import dataclass
 from functools import singledispatchmethod
 import io
-from lmdbm import Lmdb
 import numpy as np
 from pathlib import Path
 from typing import Generator, Iterable, Tuple, Union
 
 from .db import DbFactory, DbWrapper
 from .taxonomy import TaxonomyEntry
 from .utils import open_file
 
+_int_t = Union[int, np.int32, np.int64]
+
 @dataclass(frozen=True, order=True)
 class FastaEntry:
     """
     A container class to represent a FASTA entry
     """
     __slots__ = ("identifier", "sequence", "extra")
 
@@ -84,15 +85,15 @@
         super().__init__(fasta_db_path)
         self.length = np.frombuffer(self.db["length"], dtype=np.int32, count=1)[0]
 
     def __len__(self):
         return self.length
 
     @singledispatchmethod
-    def __contains__(self, sequence_index: int) -> bool:
+    def __contains__(self, sequence_index: _int_t) -> bool:
         return str(sequence_index) in self.db
 
     @__contains__.register
     def _(self, sequence_id: str) -> bool:
         return f"id_{sequence_id}" in self.db
 
     @__contains__.register
@@ -100,15 +101,15 @@
         return entry.identifier in self
 
     def __iter__(self):
         for i in range(len(self)):
             yield self[i]
 
     @singledispatchmethod
-    def __getitem__(self, sequence_index: int) -> FastaEntry:
+    def __getitem__(self, sequence_index: _int_t) -> FastaEntry:
         return FastaEntry.deserialize(self.db[str(sequence_index)])
 
     @__getitem__.register
     def _(self, sequence_id: str) -> FastaEntry:
         index = np.frombuffer(self.db[f"id_{sequence_id}"], dtype=np.int32, count=1)[0]
         return self[index]
```

### Comparing `dnadb-0.4.2/src/dnadb/fastq.py` & `dnadb-0.5.0/src/dnadb/fastq.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from dataclasses import dataclass
 import io
-from lmdbm import Lmdb
 import numpy as np
 import numpy.typing as npt
 from pathlib import Path
 from typing import Generator, Iterable, Tuple, Union
 
 from .db import DbFactory, DbWrapper
 from .utils import open_file
 
-def phred_encode(probabilities: npt.ArrayLike, encoding: int = 33) -> str:
+_int_t = Union[int, np.int32, np.int64]
+
+def phred_encode(probabilities: npt.ArrayLike, encoding: _int_t = 33) -> str:
     scores = (-10 * np.log10(np.array(probabilities))).astype(int)
     return ''.join((chr(score + encoding)) for score in scores)
 
 
-def phred_decode(qualities: str, encoding: int = 33) -> npt.NDArray[np.float64]:
+def phred_decode(qualities: str, encoding: _int_t = 33) -> npt.NDArray[np.float64]:
     scores = np.array([(ord(token) - encoding) for token in qualities])
     return 10**(scores / -10)
 
 
 @dataclass(frozen=True, order=True)
 class FastqHeader:
     """
@@ -34,22 +35,22 @@
         "read_type",
         "is_filtered",
         "control_number",
         "sequence_index"
     )
 
     instrument: str
-    run_number: int
+    run_number: _int_t
     flowcell_id: str
-    lane: int
-    tile: int
+    lane: _int_t
+    tile: _int_t
     pos: Tuple[int, int]
-    read_type: int
+    read_type: _int_t
     is_filtered: bool
-    control_number: int
+    control_number: _int_t
     sequence_index: str
 
     @classmethod
     def deserialize(cls, sequence_id: bytes):
         return cls.from_str(sequence_id.decode())
 
     @classmethod
@@ -127,15 +128,15 @@
         return f"{self.header_str}\n{self.sequence}\n+\n{self.quality_scores}"
 
 
 class FastqDbFactory(DbFactory):
     """
     A factory for creating LMDB-backed databases of FASTA entries.
     """
-    def __init__(self, path: Union[str, Path], chunk_size: int = 10000):
+    def __init__(self, path: Union[str, Path], chunk_size: _int_t = 10000):
         super().__init__(path, chunk_size)
         self.num_entries = np.int32(0)
 
     def write_entry(self, entry: FastqEntry):
         """
         Create a new FASTA LMDB database from a FASTA file.
         """
@@ -155,22 +156,22 @@
     def __init__(self, fastq_db_path: Union[str, Path]):
         super().__init__(fastq_db_path)
         self.length = np.frombuffer(self.db["length"], dtype=np.int32, count=1)[0]
 
     def __len__(self):
         return self.length
 
-    def __contains__(self, sequence_index: int) -> bool:
+    def __contains__(self, sequence_index: _int_t) -> bool:
         return str(sequence_index) in self.db
 
     def __iter__(self):
         for i in range(len(self)):
             yield self[i]
 
-    def __getitem__(self, sequence_index: int) -> FastqEntry:
+    def __getitem__(self, sequence_index: _int_t) -> FastqEntry:
         return FastqEntry.deserialize(self.db[str(sequence_index)])
 
 
 def entries(
     sequences: Union[io.TextIOBase, Iterable[FastqEntry], str, Path]
 ) -> Iterable[FastqEntry]:
     """
```

### Comparing `dnadb-0.4.2/src/dnadb/taxonomy.py` & `dnadb-0.5.0/src/dnadb/taxonomy.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from dataclasses import dataclass, field, replace
-from itertools import chain
+import heapq
 import io
+import json
 import numpy as np
 import numpy.typing as npt
 from pathlib import Path
 import re
-from sortedcontainers import SortedDict
 from typing import Dict, Generator, Iterable, List, Optional, Tuple, Union
 
 from .db import DbFactory, DbWrapper
 from .utils import open_file
 
+_int_t = Union[int, np.int32, np.int64]
+
 RANKS = ("Kingdom", "Phylum", "Class", "Order", "Family", "Genus", "Species")
 RANK_PREFIXES = ''.join(rank[0] for rank in RANKS).lower()
 
 # Utility Functions --------------------------------------------------------------------------------
 
 def split_taxonomy(taxonomy: str) -> Tuple[str, ...]:
     """
@@ -119,99 +121,111 @@
         for entry in entries:
             self.write_entry(entry)
 
     def before_close(self):
         self.write("length", self.num_entries.tobytes())
         super().before_close()
 
-
 class TaxonomyDb(DbWrapper):
     __slots__ = ("length",)
 
     def __init__(self, taxonomy_db_path: Union[str, Path]):
         super().__init__(taxonomy_db_path)
         self.length = np.frombuffer(self.db["length"], dtype=np.int32, count=1)[0]
 
-    def contains_id(self, fasta_identifier: str) -> bool:
+    def contains_fasta_id(self, fasta_identifier: str) -> bool:
         """
         Check if a FASTA identifier exists in the database.
         """
         return f">{fasta_identifier}" in self.db
 
     def contains_label(self, label: str) -> bool:
         """
         Check if a taxonomy label exists in the database.
         """
         return label in self.db
 
-    def count(self, label_index: int) -> int:
+    def count(self, label_index: _int_t) -> int:
         """
         Get the number of sequences with a given label index.
         """
         return int(np.frombuffer(self.db[f"count_{label_index}"], dtype=np.int32, count=1)[0])
 
     def counts(self) -> Generator[int, None, None]:
         """
         Get the number of sequences for each label index.
         """
         for i in range(self.length):
             yield self.count(i)
 
-    def id_to_index(self, fasta_identifier: str) -> int:
+    def fasta_id_with_label(self, label_index: _int_t, fasta_index: _int_t) -> str:
+        """
+        Get the FASTA identifier for a given label and index.
+        """
+        return self.db[f"{label_index}_{fasta_index}"].decode()
+
+    def fasta_ids_with_label(self, label_index: _int_t) -> Generator[str, None, None]:
+        """
+        Get the FASTA identifiers for a given label.
+        """
+        for i in range(self.count(label_index)):
+            yield self.fasta_id_with_label(label_index, i)
+
+    def fasta_id_to_index(self, fasta_identifier: str) -> int:
         """
         Get the taxonomy index for a given FASTA identifier.
         """
         return int(np.frombuffer(self.db[f">{fasta_identifier}"], dtype=np.int32, count=1)[0])
 
-    def id_to_label(self, fasta_identifier: str) -> str:
+    def fasta_id_to_label(self, fasta_identifier: str) -> str:
         """
         Get the taxonomy label for a given FASTA identifier.
         """
-        return self.label(self.id_to_index(fasta_identifier))
+        return self.label(self.fasta_id_to_index(fasta_identifier))
 
-    def label(self, index: int) -> str:
+    def label(self, label_index: _int_t) -> str:
         """
         Get the taxonomy label for a given index.
         """
-        return self.db[str(index)].decode()
+        return self.db[str(label_index)].decode()
 
     def labels(self) -> Generator[str, None, None]:
         """
         Get the taxonomy labels.
         """
         for i in range(self.length):
             yield self.label(i)
 
     def label_to_index(self, label: str) -> np.int32:
         """
         Get the taxonomy index for a given label.
         """
         return np.frombuffer(self.db[label], dtype=np.int32, count=1)[0]
 
-    # @cached_property
-    # def hierarchy(self):
-    #     return TaxonomyHierarchy.deserialize(self.db["hierarchy"])
-
     def __len__(self):
         return self.length
 
     def __iter__(self):
         for i in range(len(self)):
             yield self.db[str(i)].decode()
 
 # Taxonomy Hierarchy -------------------------------------------------------------------------------
 
 @dataclass(frozen=True, order=True)
 class Taxon:
     # __slots__ = ("name", "rank", "parent", "children")
-    name: str
     rank: int
-    parent: Optional["Taxon"] = field(default=None, hash=False)
+    name: str
+    parent: Optional["Taxon"] = field(default=None, repr=False)
     children: Dict[str, "Taxon"] = field(default_factory=dict, init=False, hash=False, repr=False)
 
+    def add_child(self, name: str):
+        assert name not in self, f"Attempted to add duplicate child taxon: {name}"
+        return Taxon(self.rank + 1, name, self)
+
     def __post_init__(self):
         if self.parent is not None:
             self.parent.children[self.name.casefold()] = self
 
     def __contains__(self, other: Union[str, "Taxon"]):
         if isinstance(other, Taxon):
             other = other.name
@@ -219,89 +233,78 @@
 
     def __iter__(self):
         yield from self.children.values()
 
     def __eq__(self, other: Union[str, "Taxon"]):
         if isinstance(other, str):
             return self.name.casefold() == other.casefold()
-        return self.rank == other.rank and self.name.casefold() == other.name.casefold()
+        return self.rank == other.rank \
+            and self.name.casefold() == other.name.casefold() \
+            and self.parent == other.parent
 
     def __getitem__(self, key: Union[str, "Taxon"]):
         if isinstance(key, Taxon):
             key = key.name
         return self.children[key.casefold()]
 
 class TaxonomyHierarchy:
 
-    class TaxonDict(SortedDict):
+    @classmethod
+    def deserialize(cls, hierarchy_json_bytes: Union[str, bytes, bytearray]) -> "TaxonomyHierarchy":
         """
-        A dictionary of Taxon instances with alphabetically-sorted, case-insensitive keys.
+        Deserialize a taxonomy hierarchy from a bytes object.
         """
-        def insert(self, taxon: Taxon):
-            """
-            Insert a Taxon instance into the dictionary using the Taxon's name as the key.
-            """
-            self[taxon.name] = taxon
-
-        def __contains__(self, key: Union[str, Taxon]) -> bool:
-            if isinstance(key, Taxon):
-                key = key.name
-            return super().__contains__(key.casefold())
-
-        def __getitem__(self, key: Union[str, Taxon]) -> Taxon:
-            if isinstance(key, Taxon):
-                key = key.name
-            return super().__getitem__(key.casefold())
-
-        def __setitem__(self, key: Union[str, Taxon], value: Taxon):
-            if isinstance(key, Taxon):
-                key = key.name
-            super().__setitem__(key.casefold(), value)
-
-        def __delitem__(self, key: Union[str, Taxon]):
-            if isinstance(key, Taxon):
-                key = key.name
-            super().__delitem__(key.casefold())
-
-        def keys(self) -> chain[str]:
-            return super().keys()
-
-        def values(self) -> chain[Taxon]:
-            return super().values()
+        def recursive_add(taxon_json: Dict, parent: Taxon):
+            taxon = parent.add_child(taxon_json["name"])
+            for child_json in taxon_json["children"]:
+                recursive_add(child_json, taxon)
+        hierarchy_json = json.loads(hierarchy_json_bytes)
+        hierarchy = cls(hierarchy_json["depth"])
+        for taxon_json in hierarchy_json["taxons"]:
+            recursive_add(taxon_json, hierarchy.taxon_tree_head)
+        return hierarchy
 
-        def __iter__(self) -> chain[str]:
-            return super().__iter__()
+    @classmethod
+    def from_dbs(cls, dbs: Iterable[TaxonomyDb], depth: int = 6) -> "TaxonomyHierarchy":
+        """
+        Create a taxonomy hierarchy from multiple taxonomy databases.
+        """
+        hierarchy = cls(depth)
+        for db in dbs:
+            hierarchy.add_taxonomies(db)
+        return hierarchy
 
     @classmethod
     def merged(
         cls,
         hierarchies: Iterable["TaxonomyHierarchy"],
         depth: Optional[int] = None
     ) -> "TaxonomyHierarchy":
         """
         Merge multiple taxonomy hierarchies into one.
         """
-        depth = depth if depth is not None else max(hierarchy.depth for hierarchy in hierarchies)
+        depth = depth if depth is not None else min(hierarchy.depth for hierarchy in hierarchies)
+        def recursive_insert(head: Taxon, taxon: Taxon):
+            if taxon.rank >= depth:
+                return
+            if taxon not in head:
+                head.add_child(taxon.name)
+            for child in taxon:
+                recursive_insert(head[taxon.name], child)
         merged = cls(depth)
         for hierarchy in hierarchies:
-            for taxon in hierarchy:
-                if taxon.rank >= depth:
-                    break
-                merged.taxons[taxon.rank][taxon.name] = Taxon(
-                    taxon.name,
-                    taxon.rank,
-                    parent=(merged.taxons[taxon.rank - 1][taxon.parent.name]
-                            if taxon.parent else None))
+            for child in hierarchy.taxon_tree_head:
+                recursive_insert(merged.taxon_tree_head, child)
         return merged
 
-    def __init__(self, depth: int):
+    def __init__(self, depth: int = 6):
         self.depth = depth
-        self.taxons = tuple(TaxonomyHierarchy.TaxonDict() for _ in range(depth))
-        self.__taxon_to_id_map: Optional[Tuple[Dict[Taxon, int], ...]] = None
-        self.__id_to_taxon_map: Optional[Tuple[Dict[int, Taxon], ...]] = None
+        self.taxon_tree_head = Taxon(-1, "_root_")
+        self._taxon_to_id_map: Optional[Tuple[Dict[Taxon, int], ...]] = None
+        self._id_to_taxon_map: Optional[Tuple[Dict[int, Taxon], ...]] = None
 
     def add_entries(self, entries: Iterable[TaxonomyEntry]):
         """
         Add taxonomy entries to the hierarchy.
 
         Args:
             entries (Iterable[TaxonomyEntry]): The taxonomy entries to add.
@@ -340,212 +343,248 @@
     def add_taxons(self, taxons: Tuple[str, ...]):
         """
         Add a taxonomy in the form of a taxon tuple to the hierarchy.
 
         Args:
             taxonomy (Tuple[str, ...]): The taxon tuple to add.
         """
-        taxons = taxons[:self.depth]
-        parent: Optional[Taxon] = None
-        for rank, name in enumerate(taxons):
-            if not self.has_taxon(name, rank):
-                self.__taxon_to_id_map = None
-                self.__id_to_taxon_map = None
-                self.taxons[rank].insert(Taxon(name, rank, parent))
-            parent = self.taxons[rank][name]
+        head = self.taxon_tree_head
+        for taxon in taxons[:self.depth]:
+            if taxon not in head:
+                self._id_to_taxon_map = None
+                self._taxon_to_id_map = None
+                head = head.add_child(taxon)
+            else:
+                head = head[taxon]
 
-    def has_entry(self, entry: TaxonomyEntry, strict: bool = False) -> bool:
+    def has_entry(self, entry: TaxonomyEntry) -> bool:
         """
         Check if the hierarchy has the given taxonomy.
 
         Args:
             entry (str): The taxonomy entry to check
-            strict (bool, optional): Ensure every taxon exists. Defaults to False.
 
         Returns:
             bool: The hierarchy contains the taxonomy.
         """
-        return self.has_taxonomy(entry.label, strict)
+        return self.has_taxonomy(entry.label)
 
-    def has_taxonomy(self, taxonomy: str, strict: bool = False) -> bool:
+    def has_taxonomy(self, taxonomy: str) -> bool:
         """
         Check if the hierarchy has the given taxonomy.
 
         Args:
             taxonomy (TaxonomyEntry): The taxonomy to check.
-            strict (bool, optional): Ensure every taxon exists. Defaults to False.
 
         Returns:
             bool: The hierarchy contains the taxonomy.
         """
-        if isinstance(taxonomy, TaxonomyEntry):
-            taxonomy = taxonomy.label
-        taxons = split_taxonomy(taxonomy)
-        return self.has_taxons(taxons, strict)
+        return self.has_taxons(split_taxonomy(taxonomy))
 
-    def has_taxon(self, taxon: str, rank: int) -> bool:
+    def has_taxons(self, taxons: Tuple[str, ...]) -> bool:
         """
-        Check if the given taxon is present within the hierarchy.
+        Determine if the given taxons are present in the hierarchy.
 
         Args:
-            taxon (str): The taxon name to check.
-            rank (int): The rank of the taxon.
+            taxons (Tuple[str, ...]): The taxon hierarchy to check.
 
         Returns:
-            bool: The taxon is present within the hierarchy.
-        """
-        return (rank < self.depth) and taxon.casefold() in self.taxons[rank]
-
-    def has_taxons(self, taxons: Tuple[str, ...], strict: bool = False) -> bool:
-        """
-        Check if the hierarchy has a list of taxons.
-
-        Note: When strict == False, a valid hierarchy is assumed.
+            bool: The presence of the taxons in the hierarchy.
         """
-        if len(taxons) > self.depth:
+        if len(taxons) > self.depth and taxons[self.depth] != "":
             return False
-        if not strict:
-            return self.has_taxon(taxons[-1], len(taxons) - 1)
-        return all(taxon.casefold() in self.taxons[rank] for rank, taxon in enumerate(taxons))
+        head = self.taxon_tree_head
+        for taxon in taxons[:self.depth]:
+            if taxon == "":
+                return True
+            if taxon not in head:
+                return False
+            head = head[taxon]
+        return True
 
-    def reduce_entry(self, entry: TaxonomyEntry, strict: bool = False) -> TaxonomyEntry:
+    def reduce_entry(self, entry: TaxonomyEntry) -> TaxonomyEntry:
         """
         Reduce the taxonomy to a valid known taxonomy label in the hierarchy.
 
         Args:
             entry (TaxonomyEntry): The taxonomy entry to reduce.
-            strict (bool, optional): Ensure every taxon exists. Defaults to False.
 
         Returns:
             TaxonomyEntry: A new TaxonomyEntry instance containing the reduced taxonomy label.
         """
-        return replace(entry, label=self.reduce_taxonomy(entry.label, strict))
+        return replace(entry, label=self.reduce_taxonomy(entry.label))
 
-    def reduce_taxonomy(self, taxonomy: str, strict: bool = False) -> str:
+    def reduce_taxonomy(self, taxonomy: str) -> str:
         """
         Reduce the taxonomy to a valid known taxonomy label in the hierarchy.
 
         Args:
             taxonomy (str): The taxonomy label to reduce (e.g. "k__Bacteria; ...").
-            strict (bool, optional): Ensure every taxon exists. Defaults to False.
 
         Returns:
             str: The reduced taxonomy label.
         """
-        return join_taxonomy(self.reduce_taxons(split_taxonomy(taxonomy), strict))
+        return join_taxonomy(self.reduce_taxons(split_taxonomy(taxonomy)))
 
-    def reduce_taxons(self, taxons: Tuple[str, ...], strict: bool = False) -> Tuple[str, ...]:
+    def reduce_taxons(self, taxons: Tuple[str, ...]) -> Tuple[str, ...]:
         """
         Reduce the taxonomy tuple to a valid known taxonomy in the hierarchy.
 
         Args:
             taxons (Tuple[str, ...]): The taxonomy tuple to reduce.
-            strict (bool, optional): Ensure every taxon exists. Defaults to False.
 
         Returns:
             Tuple[str, ...]: The reduced taxonomy tuple.
         """
-        taxons = taxons[:self.depth]
-        if strict:
-            for rank, taxon in enumerate(taxons):
-                if taxon not in self.taxons[rank]:
-                    return taxons[:rank]
-            return taxons
-        for i in range(len(taxons) - 1, -1, -1):
-            if taxons[i] in self.taxons[i]:
-                return taxons[:i + 1]
-        return tuple()
+        result = tuple()
+        head = self.taxon_tree_head
+        for taxon in taxons[:self.depth]:
+            if taxon not in head:
+                break
+            result += (taxon,)
+            head = head[taxon]
+        return result
 
-    def tokenize(self, taxonomy: str, pad: bool = False) -> npt.NDArray[np.int64]:
+    def tokenize(self, taxonomy: str, pad: bool = False) -> npt.NDArray[np.int32]:
         """
         Tokenize the taxonomy label into a a tuple of taxon integer IDs
 
         Args:
             taxonomy (str): The taxonomy label to tokenize (e.g. "k__Bacteria; ...").
             pad (bool): Pad the taxonomy with -1s to the depth of the hierarchy. Defaults to False.
 
         Returns:
-            Tuple[str, ...]: The tokenized taxonomy.
+            np.ndarray[np.int32]: The tokenized taxonomy.
         """
         return self.tokenize_taxons(split_taxonomy(taxonomy), pad)
 
-    def tokenize_taxons(self, taxons: Tuple[str, ...], pad: bool = False) -> npt.NDArray[np.int64]:
+    def tokenize_taxons(self, taxons: Tuple[str, ...], pad: bool = False) -> npt.NDArray[np.int32]:
         """
         Tokenize the taxonomy tuple into a a tuple of taxon integer IDs
 
         Args:
             taxons (Tuple[str, ...]): The taxonomy tuple to tokenize.
             pad (bool): Pad the taxonomy with -1s to the depth of the hierarchy. Defaults to False.
 
         Returns:
-            Tuple[str, ...]: The tokenized taxonomy.
+            np.ndarray[np.int32]: The tokenized taxonomy.
         """
-        result = np.empty(len(taxons), np.int64) if not pad else np.full(self.depth, -1, np.int64)
-        for rank, taxon in enumerate(taxons):
-            result[rank] = self.taxon_to_id_map[rank][self.taxons[rank][taxon]]
+        taxons = taxons[:self.depth] # todo should we trim silently or throw error?
+        result = np.empty(len(taxons), np.int32) if not pad else np.full(self.depth, -1, np.int32)
+        head = self.taxon_tree_head
+        for taxon in taxons:
+            head = head[taxon]
+            result[head.rank] = self.taxon_to_id_map[head.rank][head]
         return result
 
-    def detokenize(self, taxon_tokens: npt.NDArray[np.int64]) -> str:
+    def detokenize(self, taxon_tokens: npt.NDArray[np.int32]) -> str:
         """
         Detokenize the taxonomy tokens into a taxonomy label.
 
         Args:
             taxon_tokens (npt.NDArray[np.int64]): The taxonomy tokens.
 
         Returns:
             str: The detokenized taxonomy label.
         """
         return join_taxonomy(self.detokenize_taxons(taxon_tokens))
 
-    def detokenize_taxons(self, taxon_tokens: npt.NDArray[np.int64]) -> Tuple[str, ...]:
+    def detokenize_taxons(self, taxon_tokens: npt.NDArray[np.int32]) -> Tuple[str, ...]:
         """
         Detokenize the taxonomy tokens into a taxonomy tuple.
 
         Args:
             taxon_tokens (npt.NDArray[np.int64]): The taxonomy tokens.
 
         Returns:
             Tuple[str, ...]: The detokenized taxonomy tuple.
         """
         result = tuple()
+        token: np.int32
         for rank, token in enumerate(taxon_tokens):
             if token < 0:
                 break
             result += (self.id_to_taxon_map[rank][token].name,)
         return result
 
+    def serialize(self) -> bytes:
+        """
+        Serialize the taxonomy hierarchy as a JSON string.
+        """
+        def dfs_serialize(head: Taxon):
+            return {
+                "name": head.name,
+                "children": [dfs_serialize(child) for child in head]
+            }
+        taxons = []
+        for head in self.taxon_tree_head:
+            taxons.append(dfs_serialize(head))
+        return json.dumps({
+            "depth": self.depth,
+            "taxons": taxons
+        }).encode()
+
+    @property
+    def taxons(self) -> Tuple[Tuple[Taxon, ...], ...]:
+        """
+        A tuple of tuples of taxons at each rank in the hierarchy.
+        """
+        return tuple(tuple(taxons.keys()) for taxons in self.taxon_to_id_map)
+
+    @property
+    def taxon_counts(self) -> Tuple[int, ...]:
+        """
+        The number of taxons at each rank in the hierarchy.
+        """
+        return tuple(len(taxons) for taxons in self.taxon_to_id_map)
+
     @property
     def taxon_to_id_map(self) -> Tuple[Dict[Taxon, int], ...]:
         """
         A mapping of taxon instances to taxon IDs.
         """
-        if self.__taxon_to_id_map is None:
-            self.__taxon_to_id_map = tuple(
-                {taxon: i for i, taxon in enumerate(taxons.values())}
-                for taxons in self.taxons)
-        return self.__taxon_to_id_map
+        if self._taxon_to_id_map is None:
+            self._taxon_to_id_map = tuple({} for _ in range(self.depth))
+            for taxon in self:
+                self._taxon_to_id_map[taxon.rank][taxon] = len(self._taxon_to_id_map[taxon.rank])
+        return self._taxon_to_id_map
 
     @property
     def id_to_taxon_map(self) -> Tuple[Dict[int, Taxon], ...]:
         """
         A mapping of taxon IDs to Taxon instances.
         """
-        if self.__id_to_taxon_map is None:
-            self.__id_to_taxon_map = tuple(
-                {i: taxon for i, taxon in enumerate(taxons.values())}
-                for taxons in self.taxons)
-        return self.__id_to_taxon_map
+        if self._id_to_taxon_map is None:
+            self._id_to_taxon_map = tuple({} for _ in range(self.depth))
+            for taxon in self:
+                taxon_id = self.taxon_to_id_map[taxon.rank][taxon]
+                self._id_to_taxon_map[taxon.rank][taxon_id] = taxon
+        return self._id_to_taxon_map
+
+    def __eq__(self, other: "TaxonomyHierarchy"):
+        """
+        Check if two taxonomy hierarchies are equal.
+        """
+        for taxon, other_taxon in zip(self, other):
+            if taxon != other_taxon:
+                return False
+        return True
 
     def __iter__(self) -> Generator[Taxon, None, None]:
         """
-        Breadth-first iteration over the taxonomy hierarchy.
+        Breadth-first sorted iteration over the taxonomy hierarchy.
         """
-        for rank in range(self.depth):
-            yield from self.taxons[rank].values()
-
+        q: list[Taxon] = []
+        for child in self.taxon_tree_head:
+            heapq.heappush(q, child)
+        while len(q) > 0:
+            taxon = heapq.heappop(q)
+            yield taxon
+            for child in taxon:
+                heapq.heappush(q, child)
 
 def entries(
     taxonomy: Union[io.TextIOBase, Iterable[TaxonomyEntry], str, Path]
 ) -> Iterable[TaxonomyEntry]:
     """
     Create an iterator over a taxonomy file or iterable of taxonomy entries.
     """
```

### Comparing `dnadb-0.4.2/src/dnadb/utils.py` & `dnadb-0.5.0/src/dnadb/utils.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.4.2/src/dnadb.egg-info/PKG-INFO` & `dnadb-0.5.0/src/dnadb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnadb
-Version: 0.4.2
+Version: 0.5.0
 Summary: A library for handling DNA files.
 Author-email: David Ludwig <davidludwigii@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 DLii-Research
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dnadb-0.4.2/src/dnadb.egg-info/SOURCES.txt` & `dnadb-0.5.0/src/dnadb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

