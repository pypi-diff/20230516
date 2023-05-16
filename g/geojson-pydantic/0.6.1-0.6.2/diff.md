# Comparing `tmp/geojson-pydantic-0.6.1.tar.gz` & `tmp/geojson_pydantic-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geojson-pydantic-0.6.1.tar", last modified: Thu May 11 23:04:37 2023, max compression
+gzip compressed data, was "geojson_pydantic-0.6.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `geojson-pydantic-0.6.1.tar` & `geojson_pydantic-0.6.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      220 2023-05-11 23:04:25.778352 geojson-pydantic-0.6.1/.bumpversion.cfg
--rw-r--r--   0        0        0     1173 2023-05-11 23:04:25.778352 geojson-pydantic-0.6.1/.gitignore
--rw-r--r--   0        0        0      792 2023-05-11 23:04:25.778352 geojson-pydantic-0.6.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1073 2023-05-11 23:04:25.778352 geojson-pydantic-0.6.1/LICENSE
--rw-r--r--   0        0        0     6592 2023-05-11 23:04:25.778352 geojson-pydantic-0.6.1/README.md
--rw-r--r--   0        0        0      448 2023-05-11 23:04:25.778352 geojson-pydantic-0.6.1/geojson_pydantic/__init__.py
--rw-r--r--   0        0        0     2624 2023-05-11 23:04:25.778352 geojson-pydantic-0.6.1/geojson_pydantic/features.py
--rw-r--r--   0        0        0      705 2023-05-11 23:04:25.778352 geojson-pydantic-0.6.1/geojson_pydantic/geo_interface.py
--rw-r--r--   0        0        0    10811 2023-05-11 23:04:25.778352 geojson-pydantic-0.6.1/geojson_pydantic/geometries.py
--rw-r--r--   0        0        0        0 2023-05-11 23:04:25.778352 geojson-pydantic-0.6.1/geojson_pydantic/py.typed
--rw-r--r--   0        0        0      694 2023-05-11 23:04:25.778352 geojson-pydantic-0.6.1/geojson_pydantic/types.py
--rw-r--r--   0        0        0     2293 2023-05-11 23:04:25.778352 geojson-pydantic-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     7596 1970-01-01 00:00:00.000000 geojson-pydantic-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0      220 2023-05-16 21:47:04.019785 geojson_pydantic-0.6.2/.bumpversion.cfg
+-rw-r--r--   0        0        0     1173 2023-05-16 21:47:04.023785 geojson_pydantic-0.6.2/.gitignore
+-rw-r--r--   0        0        0      792 2023-05-16 21:47:04.023785 geojson_pydantic-0.6.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1073 2023-05-16 21:47:04.023785 geojson_pydantic-0.6.2/LICENSE
+-rw-r--r--   0        0        0     6592 2023-05-16 21:47:04.023785 geojson_pydantic-0.6.2/README.md
+-rw-r--r--   0        0        0      448 2023-05-16 21:47:04.023785 geojson_pydantic-0.6.2/geojson_pydantic/__init__.py
+-rw-r--r--   0        0        0     1906 2023-05-16 21:47:04.023785 geojson_pydantic-0.6.2/geojson_pydantic/features.py
+-rw-r--r--   0        0        0      705 2023-05-16 21:47:04.023785 geojson_pydantic-0.6.2/geojson_pydantic/geo_interface.py
+-rw-r--r--   0        0        0    10976 2023-05-16 21:47:04.023785 geojson_pydantic-0.6.2/geojson_pydantic/geometries.py
+-rw-r--r--   0        0        0        0 2023-05-16 21:47:04.023785 geojson_pydantic-0.6.2/geojson_pydantic/py.typed
+-rw-r--r--   0        0        0     1696 2023-05-16 21:47:04.023785 geojson_pydantic-0.6.2/geojson_pydantic/types.py
+-rw-r--r--   0        0        0     2293 2023-05-16 21:47:04.023785 geojson_pydantic-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     7596 1970-01-01 00:00:00.000000 geojson_pydantic-0.6.2/PKG-INFO
```

### Comparing `geojson-pydantic-0.6.1/.gitignore` & `geojson_pydantic-0.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `geojson-pydantic-0.6.1/.pre-commit-config.yaml` & `geojson_pydantic-0.6.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `geojson-pydantic-0.6.1/LICENSE` & `geojson_pydantic-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `geojson-pydantic-0.6.1/README.md` & `geojson_pydantic-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `geojson-pydantic-0.6.1/geojson_pydantic/geo_interface.py` & `geojson_pydantic-0.6.2/geojson_pydantic/geo_interface.py`

 * *Files identical despite different names*

### Comparing `geojson-pydantic-0.6.1/geojson_pydantic/geometries.py` & `geojson_pydantic-0.6.2/geojson_pydantic/geometries.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     LinearRing,
     LineStringCoords,
     MultiLineStringCoords,
     MultiPointCoords,
     MultiPolygonCoords,
     PolygonCoords,
     Position,
+    validate_bbox,
 )
 
 
 def _position_wkt_coordinates(coordinates: Position, force_z: bool = False) -> str:
     """Converts a Position to WKT Coordinates."""
     wkt_coordinates = " ".join(str(number) for number in coordinates)
     if force_z and len(coordinates) < 3:
@@ -103,14 +104,16 @@
             wkt += f"({self.__wkt_coordinates__(self.coordinates, force_z=has_z)})"
         else:
             # Otherwise it will be "EMPTY"
             wkt += " EMPTY"
 
         return wkt
 
+    _validate_bbox = validator("bbox", allow_reuse=True)(validate_bbox)
+
 
 class Point(_GeometryBase):
     """Point Model"""
 
     type: Literal["Point"]
     coordinates: Position
 
@@ -283,14 +286,16 @@
             if self.geometries
             else "EMPTY"
         )
         # If any of them contain `Z` add Z to the output wkt
         z = " Z " if "Z" in geometries else " "
         return f"{self.type.upper()}{z}{geometries}"
 
+    _validate_bbox = validator("bbox", allow_reuse=True)(validate_bbox)
+
     @validator("geometries")
     def check_geometries(cls, geometries: List) -> List:
         """Add warnings for conditions the spec does not explicitly forbid."""
         if len(geometries) == 1:
             warnings.warn(
                 "GeometryCollection should not be used for single geometries."
             )
```

### Comparing `geojson-pydantic-0.6.1/pyproject.toml` & `geojson_pydantic-0.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `geojson-pydantic-0.6.1/PKG-INFO` & `geojson_pydantic-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geojson-pydantic
-Version: 0.6.1
+Version: 0.6.2
 Summary: Pydantic data models for the GeoJSON spec.
 Keywords: geojson,Pydantic
 Author-email: Drew Bollinger <drew@developmentseed.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
```

