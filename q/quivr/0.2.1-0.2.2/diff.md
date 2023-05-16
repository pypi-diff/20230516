# Comparing `tmp/quivr-0.2.1.tar.gz` & `tmp/quivr-0.2.2.tar.gz`

## Comparing `quivr-0.2.1.tar` & `quivr-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 quivr-0.2.1/quivr/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 quivr-0.2.1/quivr/__version__.py
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 quivr-0.2.1/quivr/concat.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 quivr-0.2.1/quivr/defragment.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 quivr-0.2.1/quivr/errors.py
--rw-r--r--   0        0        0    22772 2020-02-02 00:00:00.000000 quivr-0.2.1/quivr/fields.py
--rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 quivr-0.2.1/quivr/indexing.py
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 quivr-0.2.1/quivr/matrix.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 quivr-0.2.1/quivr/py.typed
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 quivr-0.2.1/quivr/schemagraph.py
--rw-r--r--   0        0        0    17108 2020-02-02 00:00:00.000000 quivr-0.2.1/quivr/tables.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 quivr-0.2.1/.gitignore
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 quivr-0.2.1/LICENSE
--rw-r--r--   0        0        0     7894 2020-02-02 00:00:00.000000 quivr-0.2.1/README.md
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 quivr-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     8292 2020-02-02 00:00:00.000000 quivr-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 quivr-0.2.2/quivr/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 quivr-0.2.2/quivr/__version__.py
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 quivr-0.2.2/quivr/concat.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 quivr-0.2.2/quivr/defragment.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 quivr-0.2.2/quivr/errors.py
+-rw-r--r--   0        0        0    22772 2020-02-02 00:00:00.000000 quivr-0.2.2/quivr/fields.py
+-rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 quivr-0.2.2/quivr/indexing.py
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 quivr-0.2.2/quivr/matrix.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 quivr-0.2.2/quivr/py.typed
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 quivr-0.2.2/quivr/schemagraph.py
+-rw-r--r--   0        0        0    18425 2020-02-02 00:00:00.000000 quivr-0.2.2/quivr/tables.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 quivr-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 quivr-0.2.2/LICENSE
+-rw-r--r--   0        0        0     7894 2020-02-02 00:00:00.000000 quivr-0.2.2/README.md
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 quivr-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     8292 2020-02-02 00:00:00.000000 quivr-0.2.2/PKG-INFO
```

### Comparing `quivr-0.2.1/quivr/__init__.py` & `quivr-0.2.2/quivr/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,17 +30,18 @@
     UInt8Field,
     UInt16Field,
     UInt32Field,
     UInt64Field,
 )
 from .indexing import StringIndex
 from .matrix import MatrixArray, MatrixExtensionType
+from .tables import Table
 
 __all__ = [
-    "TableBase",
+    "Table",
     "MatrixArray",
     "MatrixExtensionType",
     "concatenate",
     "StringIndex",
     "Field",
     "SubTableField" "Int8Field",
     "Int16Field",
```

### Comparing `quivr-0.2.1/quivr/concat.py` & `quivr-0.2.2/quivr/concat.py`

 * *Files identical despite different names*

### Comparing `quivr-0.2.1/quivr/fields.py` & `quivr-0.2.2/quivr/fields.py`

 * *Files identical despite different names*

### Comparing `quivr-0.2.1/quivr/indexing.py` & `quivr-0.2.2/quivr/indexing.py`

 * *Files identical despite different names*

### Comparing `quivr-0.2.1/quivr/matrix.py` & `quivr-0.2.2/quivr/matrix.py`

 * *Files identical despite different names*

### Comparing `quivr-0.2.1/quivr/schemagraph.py` & `quivr-0.2.2/quivr/schemagraph.py`

 * *Files identical despite different names*

### Comparing `quivr-0.2.1/quivr/tables.py` & `quivr-0.2.2/quivr/tables.py`

 * *Files 5% similar despite different names*

```diff
@@ -94,28 +94,62 @@
 
         Each keyword argument corresponds to a field in the Table.
 
         The keys should correspond to the field names, and the values
         can be a list, numpy array, pyarrow array, or Table instance.
         """
         arrays = []
-        for column_name in cls.schema.names:
+        size = None
+
+        # We don't know the size of the table until we've found a
+        # field in the schema which corresponds to a kwarg with data.
+        # Therefore, we need to keep track of which columns are empty
+        # *before* we've discovered the size of the table so we can
+        # populate them with nulls later.
+        empty_columns = []
+
+        for i, field in enumerate(cls.schema):
+            column_name = field.name
             if column_name not in kwargs:
-                raise ValueError(f"Missing column {column_name}")
+                if not field.nullable:
+                    raise ValueError(f"Missing non-nullable column {column_name}")
+                else:
+                    if size is not None:
+                        arrays.append(pa.nulls(size, type=cls.schema[i].type))
+                    else:
+                        # We'll have to wait until we get to a non-None column
+                        # to figure out the size.
+                        empty_columns.append(i)
+                        arrays.append(None)
+                    continue
+
             value = kwargs[column_name]
+            if size is None:
+                size = len(value)
+            elif len(value) != size:
+                raise ValueError(
+                    f"Column {column_name} has wrong length {len(value)} (first column has length {size})"
+                )
+
             if isinstance(value, Table):
                 arrays.append(value.to_structarray())
             elif isinstance(value, pa.Array):
                 arrays.append(value)
             elif isinstance(value, np.ndarray):
                 arrays.append(pa.array(value))
             elif isinstance(value, list):
                 arrays.append(pa.array(value))
             else:
                 raise TypeError(f"Unsupported type for {column_name}: {type(value)}")
+
+        if size is None:
+            raise ValueError("No data provided")
+
+        for idx in empty_columns:
+            arrays[idx] = pa.nulls(size, type=cls.schema[idx].type)
         return cls.from_arrays(arrays)
 
     @classmethod
     def from_arrays(cls, arrays: list[pa.array]) -> Self:
         """Create a Table object from a list of arrays.
 
         Args:
```

### Comparing `quivr-0.2.1/LICENSE` & `quivr-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quivr-0.2.1/README.md` & `quivr-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `quivr-0.2.1/pyproject.toml` & `quivr-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `quivr-0.2.1/PKG-INFO` & `quivr-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quivr
-Version: 0.2.1
+Version: 0.2.2
 Summary: Container library for working with tabular Arrow data
 Project-URL: Source, https://github.com/spenczar/quivr
 Author-email: Spencer Nelson <spencer@spencerwnelson.com>
 License-File: LICENSE
 Requires-Python: >=3.11
 Requires-Dist: mmh3
 Requires-Dist: numpy
```

