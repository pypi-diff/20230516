# Comparing `tmp/buenavista-0.2.3.tar.gz` & `tmp/buenavista-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buenavista-0.2.3.tar", last modified: Tue May 16 19:22:54 2023, max compression
+gzip compressed data, was "buenavista-0.3.0.tar", last modified: Tue May 16 19:42:03 2023, max compression
```

## Comparing `buenavista-0.2.3.tar` & `buenavista-0.3.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-16 19:22:54.661987 buenavista-0.2.3/
--rw-r--r--   0 jwills     (501) staff       (20)    11357 2022-12-17 04:32:44.000000 buenavista-0.2.3/LICENSE
--rw-r--r--   0 jwills     (501) staff       (20)     1910 2023-05-16 19:22:54.661812 buenavista-0.2.3/PKG-INFO
--rw-r--r--   0 jwills     (501) staff       (20)     1575 2023-05-10 16:04:37.000000 buenavista-0.2.3/README.md
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-16 19:22:54.655926 buenavista-0.2.3/buenavista/
--rw-r--r--   0 jwills     (501) staff       (20)        0 2022-12-27 19:08:41.000000 buenavista-0.2.3/buenavista/__init__.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-16 19:22:54.659474 buenavista-0.2.3/buenavista/backends/
--rw-r--r--   0 jwills     (501) staff       (20)        0 2023-01-13 04:28:53.000000 buenavista-0.2.3/buenavista/backends/__init__.py
--rw-r--r--   0 jwills     (501) staff       (20)     7551 2023-05-16 18:18:50.000000 buenavista-0.2.3/buenavista/backends/duckdb.py
--rw-r--r--   0 jwills     (501) staff       (20)     3359 2023-05-10 21:05:33.000000 buenavista-0.2.3/buenavista/backends/postgres.py
--rw-r--r--   0 jwills     (501) staff       (20)     4192 2023-05-16 19:22:05.000000 buenavista-0.2.3/buenavista/bv_dialects.py
--rw-r--r--   0 jwills     (501) staff       (20)     3148 2023-04-25 23:01:34.000000 buenavista-0.2.3/buenavista/core.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-16 19:22:54.660327 buenavista-0.2.3/buenavista/examples/
--rw-r--r--   0 jwills     (501) staff       (20)     3996 2023-05-16 19:22:05.000000 buenavista-0.2.3/buenavista/examples/duckdb_http.py
--rw-r--r--   0 jwills     (501) staff       (20)     1472 2023-05-10 21:05:33.000000 buenavista-0.2.3/buenavista/examples/duckdb_postgres.py
--rw-r--r--   0 jwills     (501) staff       (20)      428 2023-03-10 16:36:56.000000 buenavista-0.2.3/buenavista/examples/postgres_proxy.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-16 19:22:54.661496 buenavista-0.2.3/buenavista/http/
--rw-r--r--   0 jwills     (501) staff       (20)        0 2023-03-21 18:23:57.000000 buenavista-0.2.3/buenavista/http/__init__.py
--rw-r--r--   0 jwills     (501) staff       (20)     3247 2023-04-03 05:42:19.000000 buenavista-0.2.3/buenavista/http/context.py
--rw-r--r--   0 jwills     (501) staff       (20)     4339 2023-05-16 18:18:50.000000 buenavista-0.2.3/buenavista/http/main.py
--rw-r--r--   0 jwills     (501) staff       (20)     2227 2023-03-09 18:25:32.000000 buenavista-0.2.3/buenavista/http/schemas.py
--rw-r--r--   0 jwills     (501) staff       (20)     1709 2023-03-09 18:25:32.000000 buenavista-0.2.3/buenavista/http/type_mapping.py
--rw-r--r--   0 jwills     (501) staff       (20)    20676 2023-05-10 16:04:37.000000 buenavista-0.2.3/buenavista/postgres.py
--rw-r--r--   0 jwills     (501) staff       (20)     1840 2023-04-25 17:26:47.000000 buenavista-0.2.3/buenavista/rewrite.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-16 19:22:54.659042 buenavista-0.2.3/buenavista.egg-info/
--rw-r--r--   0 jwills     (501) staff       (20)     1910 2023-05-16 19:22:54.000000 buenavista-0.2.3/buenavista.egg-info/PKG-INFO
--rw-r--r--   0 jwills     (501) staff       (20)      652 2023-05-16 19:22:54.000000 buenavista-0.2.3/buenavista.egg-info/SOURCES.txt
--rw-r--r--   0 jwills     (501) staff       (20)        1 2023-05-16 19:22:54.000000 buenavista-0.2.3/buenavista.egg-info/dependency_links.txt
--rw-r--r--   0 jwills     (501) staff       (20)       83 2023-05-16 19:22:54.000000 buenavista-0.2.3/buenavista.egg-info/requires.txt
--rw-r--r--   0 jwills     (501) staff       (20)       11 2023-05-16 19:22:54.000000 buenavista-0.2.3/buenavista.egg-info/top_level.txt
--rw-r--r--   0 jwills     (501) staff       (20)       38 2023-05-16 19:22:54.662025 buenavista-0.2.3/setup.cfg
--rw-r--r--   0 jwills     (501) staff       (20)     1022 2023-05-16 19:22:28.000000 buenavista-0.2.3/setup.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-16 19:42:03.690891 buenavista-0.3.0/
+-rw-r--r--   0 jwills     (501) staff       (20)    11357 2022-12-17 04:32:44.000000 buenavista-0.3.0/LICENSE
+-rw-r--r--   0 jwills     (501) staff       (20)     1910 2023-05-16 19:42:03.690781 buenavista-0.3.0/PKG-INFO
+-rw-r--r--   0 jwills     (501) staff       (20)     1575 2023-05-10 16:04:37.000000 buenavista-0.3.0/README.md
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-16 19:42:03.687748 buenavista-0.3.0/buenavista/
+-rw-r--r--   0 jwills     (501) staff       (20)        0 2022-12-27 19:08:41.000000 buenavista-0.3.0/buenavista/__init__.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-16 19:42:03.688902 buenavista-0.3.0/buenavista/backends/
+-rw-r--r--   0 jwills     (501) staff       (20)        0 2023-01-13 04:28:53.000000 buenavista-0.3.0/buenavista/backends/__init__.py
+-rw-r--r--   0 jwills     (501) staff       (20)     7551 2023-05-16 18:18:50.000000 buenavista-0.3.0/buenavista/backends/duckdb.py
+-rw-r--r--   0 jwills     (501) staff       (20)     3359 2023-05-10 21:05:33.000000 buenavista-0.3.0/buenavista/backends/postgres.py
+-rw-r--r--   0 jwills     (501) staff       (20)     4192 2023-05-16 19:22:05.000000 buenavista-0.3.0/buenavista/bv_dialects.py
+-rw-r--r--   0 jwills     (501) staff       (20)     3148 2023-04-25 23:01:34.000000 buenavista-0.3.0/buenavista/core.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-16 19:42:03.689533 buenavista-0.3.0/buenavista/examples/
+-rw-r--r--   0 jwills     (501) staff       (20)     3957 2023-05-16 19:24:36.000000 buenavista-0.3.0/buenavista/examples/duckdb_http.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1472 2023-05-10 21:05:33.000000 buenavista-0.3.0/buenavista/examples/duckdb_postgres.py
+-rw-r--r--   0 jwills     (501) staff       (20)      428 2023-03-10 16:36:56.000000 buenavista-0.3.0/buenavista/examples/postgres_proxy.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-16 19:42:03.690512 buenavista-0.3.0/buenavista/http/
+-rw-r--r--   0 jwills     (501) staff       (20)        0 2023-03-21 18:23:57.000000 buenavista-0.3.0/buenavista/http/__init__.py
+-rw-r--r--   0 jwills     (501) staff       (20)     3247 2023-04-03 05:42:19.000000 buenavista-0.3.0/buenavista/http/context.py
+-rw-r--r--   0 jwills     (501) staff       (20)     4339 2023-05-16 18:18:50.000000 buenavista-0.3.0/buenavista/http/main.py
+-rw-r--r--   0 jwills     (501) staff       (20)     2227 2023-03-09 18:25:32.000000 buenavista-0.3.0/buenavista/http/schemas.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1709 2023-03-09 18:25:32.000000 buenavista-0.3.0/buenavista/http/type_mapping.py
+-rw-r--r--   0 jwills     (501) staff       (20)    20676 2023-05-10 16:04:37.000000 buenavista-0.3.0/buenavista/postgres.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1840 2023-04-25 17:26:47.000000 buenavista-0.3.0/buenavista/rewrite.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-16 19:42:03.688475 buenavista-0.3.0/buenavista.egg-info/
+-rw-r--r--   0 jwills     (501) staff       (20)     1910 2023-05-16 19:42:03.000000 buenavista-0.3.0/buenavista.egg-info/PKG-INFO
+-rw-r--r--   0 jwills     (501) staff       (20)      652 2023-05-16 19:42:03.000000 buenavista-0.3.0/buenavista.egg-info/SOURCES.txt
+-rw-r--r--   0 jwills     (501) staff       (20)        1 2023-05-16 19:42:03.000000 buenavista-0.3.0/buenavista.egg-info/dependency_links.txt
+-rw-r--r--   0 jwills     (501) staff       (20)       83 2023-05-16 19:42:03.000000 buenavista-0.3.0/buenavista.egg-info/requires.txt
+-rw-r--r--   0 jwills     (501) staff       (20)       11 2023-05-16 19:42:03.000000 buenavista-0.3.0/buenavista.egg-info/top_level.txt
+-rw-r--r--   0 jwills     (501) staff       (20)       38 2023-05-16 19:42:03.690920 buenavista-0.3.0/setup.cfg
+-rw-r--r--   0 jwills     (501) staff       (20)     1022 2023-05-16 19:25:34.000000 buenavista-0.3.0/setup.py
```

### Comparing `buenavista-0.2.3/LICENSE` & `buenavista-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `buenavista-0.2.3/PKG-INFO` & `buenavista-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buenavista
-Version: 0.2.3
+Version: 0.3.0
 Summary: Programmable Presto and Postgres Proxies
 Home-page: https://github.com/jwills/buenavista
 Author: Josh Wills
 Author-email: joshwills+bv@gmail.com
 License: Apache
 Description-Content-Type: text/markdown
 Provides-Extra: duckdb
```

### Comparing `buenavista-0.2.3/README.md` & `buenavista-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `buenavista-0.2.3/buenavista/backends/duckdb.py` & `buenavista-0.3.0/buenavista/backends/duckdb.py`

 * *Files identical despite different names*

### Comparing `buenavista-0.2.3/buenavista/backends/postgres.py` & `buenavista-0.3.0/buenavista/backends/postgres.py`

 * *Files identical despite different names*

### Comparing `buenavista-0.2.3/buenavista/bv_dialects.py` & `buenavista-0.3.0/buenavista/bv_dialects.py`

 * *Files identical despite different names*

### Comparing `buenavista-0.2.3/buenavista/core.py` & `buenavista-0.3.0/buenavista/core.py`

 * *Files identical despite different names*

### Comparing `buenavista-0.2.3/buenavista/examples/duckdb_http.py` & `buenavista-0.3.0/buenavista/examples/duckdb_http.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     return "LIKE " + token.replace(escape, "")
 
 
 class DuckDBHTTPRewriter(rewrite.Rewriter):
     def rewrite(self, sql: str) -> str:
         sql = super().rewrite(sql)
         sql = ESCAPE_PATTERN.sub(_escape_replace, sql)
-        print("Rewritten to %s" % sql)
         return sql
 
 
 rewriter = DuckDBHTTPRewriter(bv_dialects.BVTrino(), bv_dialects.BVDuckDB())
 
 
 @rewriter.relation("system.jdbc.tables")
```

### Comparing `buenavista-0.2.3/buenavista/examples/duckdb_postgres.py` & `buenavista-0.3.0/buenavista/examples/duckdb_postgres.py`

 * *Files identical despite different names*

### Comparing `buenavista-0.2.3/buenavista/http/context.py` & `buenavista-0.3.0/buenavista/http/context.py`

 * *Files identical despite different names*

### Comparing `buenavista-0.2.3/buenavista/http/main.py` & `buenavista-0.3.0/buenavista/http/main.py`

 * *Files identical despite different names*

### Comparing `buenavista-0.2.3/buenavista/http/schemas.py` & `buenavista-0.3.0/buenavista/http/schemas.py`

 * *Files identical despite different names*

### Comparing `buenavista-0.2.3/buenavista/http/type_mapping.py` & `buenavista-0.3.0/buenavista/http/type_mapping.py`

 * *Files identical despite different names*

### Comparing `buenavista-0.2.3/buenavista/postgres.py` & `buenavista-0.3.0/buenavista/postgres.py`

 * *Files identical despite different names*

### Comparing `buenavista-0.2.3/buenavista/rewrite.py` & `buenavista-0.3.0/buenavista/rewrite.py`

 * *Files identical despite different names*

### Comparing `buenavista-0.2.3/buenavista.egg-info/PKG-INFO` & `buenavista-0.3.0/buenavista.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buenavista
-Version: 0.2.3
+Version: 0.3.0
 Summary: Programmable Presto and Postgres Proxies
 Home-page: https://github.com/jwills/buenavista
 Author: Josh Wills
 Author-email: joshwills+bv@gmail.com
 License: Apache
 Description-Content-Type: text/markdown
 Provides-Extra: duckdb
```

### Comparing `buenavista-0.2.3/buenavista.egg-info/SOURCES.txt` & `buenavista-0.3.0/buenavista.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `buenavista-0.2.3/setup.py` & `buenavista-0.3.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md")) as f:
     long_description = f.read()
 
 package_name = "buenavista"
-package_version = "0.2.3"
+package_version = "0.3.0"
 
 description = """Programmable Presto and Postgres Proxies"""
 
 setup(
     name=package_name,
     version=package_version,
     description=description,
```

