# Comparing `tmp/duckdbt-0.3.1.tar.gz` & `tmp/duckdbt-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckdbt-0.3.1.tar", last modified: Tue May  9 00:16:03 2023, max compression
+gzip compressed data, was "duckdbt-0.3.2.tar", last modified: Tue May 16 19:45:14 2023, max compression
```

## Comparing `duckdbt-0.3.1.tar` & `duckdbt-0.3.2.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-09 00:16:03.623397 duckdbt-0.3.1/
--rw-r--r--   0 jwills     (501) staff       (20)       53 2023-01-14 04:58:00.000000 duckdbt-0.3.1/MANIFEST.in
--rw-r--r--   0 jwills     (501) staff       (20)      302 2023-05-09 00:16:03.623286 duckdbt-0.3.1/PKG-INFO
--rw-r--r--   0 jwills     (501) staff       (20)       53 2023-05-08 20:57:22.000000 duckdbt-0.3.1/README.md
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-09 00:16:03.622033 duckdbt-0.3.1/duckdbt/
--rw-r--r--   0 jwills     (501) staff       (20)     1248 2023-05-08 20:17:37.000000 duckdbt-0.3.1/duckdbt/api.py
--rw-r--r--   0 jwills     (501) staff       (20)     1736 2023-05-08 20:17:37.000000 duckdbt-0.3.1/duckdbt/extensions.py
--rw-r--r--   0 jwills     (501) staff       (20)      696 2023-05-08 20:17:37.000000 duckdbt-0.3.1/duckdbt/ipython.py
--rw-r--r--   0 jwills     (501) staff       (20)     1786 2023-05-09 00:15:58.000000 duckdbt-0.3.1/duckdbt/load_db_profile.py
--rw-r--r--   0 jwills     (501) staff       (20)     1884 2023-05-08 20:17:37.000000 duckdbt-0.3.1/duckdbt/server.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-09 00:16:03.622990 duckdbt-0.3.1/duckdbt/static/
--rw-r--r--   0 jwills     (501) staff       (20)     1246 2023-01-14 04:58:00.000000 duckdbt-0.3.1/duckdbt/static/dashboard.css
--rw-r--r--   0 jwills     (501) staff       (20)     1406 2023-05-08 20:17:37.000000 duckdbt-0.3.1/duckdbt/static/favicon.ico
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-09 00:16:03.623122 duckdbt-0.3.1/duckdbt/templates/
--rw-r--r--   0 jwills     (501) staff       (20)     5332 2023-05-08 20:17:37.000000 duckdbt-0.3.1/duckdbt/templates/index.html
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-09 00:16:03.622636 duckdbt-0.3.1/duckdbt.egg-info/
--rw-r--r--   0 jwills     (501) staff       (20)      302 2023-05-09 00:16:03.000000 duckdbt-0.3.1/duckdbt.egg-info/PKG-INFO
--rw-r--r--   0 jwills     (501) staff       (20)      370 2023-05-09 00:16:03.000000 duckdbt-0.3.1/duckdbt.egg-info/SOURCES.txt
--rw-r--r--   0 jwills     (501) staff       (20)        1 2023-05-09 00:16:03.000000 duckdbt-0.3.1/duckdbt.egg-info/dependency_links.txt
--rw-r--r--   0 jwills     (501) staff       (20)       87 2023-05-09 00:16:03.000000 duckdbt-0.3.1/duckdbt.egg-info/requires.txt
--rw-r--r--   0 jwills     (501) staff       (20)        8 2023-05-09 00:16:03.000000 duckdbt-0.3.1/duckdbt.egg-info/top_level.txt
--rw-r--r--   0 jwills     (501) staff       (20)       38 2023-05-09 00:16:03.623430 duckdbt-0.3.1/setup.cfg
--rw-r--r--   0 jwills     (501) staff       (20)      951 2023-05-09 00:15:58.000000 duckdbt-0.3.1/setup.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-16 19:45:14.435883 duckdbt-0.3.2/
+-rw-r--r--   0 jwills     (501) staff       (20)       53 2023-01-14 04:58:00.000000 duckdbt-0.3.2/MANIFEST.in
+-rw-r--r--   0 jwills     (501) staff       (20)      302 2023-05-16 19:45:14.435758 duckdbt-0.3.2/PKG-INFO
+-rw-r--r--   0 jwills     (501) staff       (20)       53 2023-05-08 20:57:22.000000 duckdbt-0.3.2/README.md
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-16 19:45:14.434517 duckdbt-0.3.2/duckdbt/
+-rw-r--r--   0 jwills     (501) staff       (20)     1248 2023-05-08 20:17:37.000000 duckdbt-0.3.2/duckdbt/api.py
+-rw-r--r--   0 jwills     (501) staff       (20)      938 2023-05-16 19:23:48.000000 duckdbt-0.3.2/duckdbt/common.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1736 2023-05-08 20:17:37.000000 duckdbt-0.3.2/duckdbt/extensions.py
+-rw-r--r--   0 jwills     (501) staff       (20)      536 2023-05-16 19:23:48.000000 duckdbt-0.3.2/duckdbt/ipython.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1786 2023-05-09 00:15:58.000000 duckdbt-0.3.2/duckdbt/load_db_profile.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1165 2023-05-16 19:23:48.000000 duckdbt-0.3.2/duckdbt/server.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-16 19:45:14.435373 duckdbt-0.3.2/duckdbt/static/
+-rw-r--r--   0 jwills     (501) staff       (20)     1489 2023-05-16 19:23:48.000000 duckdbt-0.3.2/duckdbt/static/dashboard.css
+-rw-r--r--   0 jwills     (501) staff       (20)     1406 2023-05-08 20:17:37.000000 duckdbt-0.3.2/duckdbt/static/favicon.ico
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-16 19:45:14.435580 duckdbt-0.3.2/duckdbt/templates/
+-rw-r--r--   0 jwills     (501) staff       (20)     4910 2023-05-16 19:23:48.000000 duckdbt-0.3.2/duckdbt/templates/index.html
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-16 19:45:14.435072 duckdbt-0.3.2/duckdbt.egg-info/
+-rw-r--r--   0 jwills     (501) staff       (20)      302 2023-05-16 19:45:14.000000 duckdbt-0.3.2/duckdbt.egg-info/PKG-INFO
+-rw-r--r--   0 jwills     (501) staff       (20)      388 2023-05-16 19:45:14.000000 duckdbt-0.3.2/duckdbt.egg-info/SOURCES.txt
+-rw-r--r--   0 jwills     (501) staff       (20)        1 2023-05-16 19:45:14.000000 duckdbt-0.3.2/duckdbt.egg-info/dependency_links.txt
+-rw-r--r--   0 jwills     (501) staff       (20)       87 2023-05-16 19:45:14.000000 duckdbt-0.3.2/duckdbt.egg-info/requires.txt
+-rw-r--r--   0 jwills     (501) staff       (20)        8 2023-05-16 19:45:14.000000 duckdbt-0.3.2/duckdbt.egg-info/top_level.txt
+-rw-r--r--   0 jwills     (501) staff       (20)       38 2023-05-16 19:45:14.435914 duckdbt-0.3.2/setup.cfg
+-rw-r--r--   0 jwills     (501) staff       (20)      951 2023-05-16 19:44:44.000000 duckdbt-0.3.2/setup.py
```

### Comparing `duckdbt-0.3.1/duckdbt/api.py` & `duckdbt-0.3.2/duckdbt/api.py`

 * *Files identical despite different names*

### Comparing `duckdbt-0.3.1/duckdbt/extensions.py` & `duckdbt-0.3.2/duckdbt/extensions.py`

 * *Files identical despite different names*

### Comparing `duckdbt-0.3.1/duckdbt/load_db_profile.py` & `duckdbt-0.3.2/duckdbt/load_db_profile.py`

 * *Files identical despite different names*

### Comparing `duckdbt-0.3.1/duckdbt/static/dashboard.css` & `duckdbt-0.3.2/duckdbt/static/dashboard.css`

 * *Files 18% similar despite different names*

```diff
@@ -76,7 +76,26 @@
   border-color: rgba(255, 255, 255, .1);
 }
 
 .form-control-dark:focus {
   border-color: transparent;
   box-shadow: 0 0 0 3px rgba(255, 255, 255, .25);
 }
+
+.relation-item {
+  white-space: nowrap;
+  overflow: hidden;
+  text-overflow: ellipsis;
+}
+
+.relation-link {
+  display: block;
+  max-width: 100%;
+}
+
+.relation-link:hover {
+  text-decoration: none;
+}
+
+.relation-column {
+  padding-left: 1.5rem;
+}
```

### Comparing `duckdbt-0.3.1/duckdbt/static/favicon.ico` & `duckdbt-0.3.2/duckdbt/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `duckdbt-0.3.1/duckdbt/templates/index.html` & `duckdbt-0.3.2/duckdbt/templates/index.html`

 * *Files 5% similar despite different names*

```diff
@@ -2,37 +2,14 @@
   <head>
     <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-GLhlTQ8iRABdZLl6O3oVMWSktQOp6b7In1Zl3/Jr59b6EGGoI1aFkw7cmDA6j6gD" crossorigin="anonymous">
     <link href="https://cdn.jsdelivr.net/npm/codemirror@5.57.0/lib/codemirror.css" rel="stylesheet">
     <link href="/static/dashboard.css">
     <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/js/bootstrap.bundle.min.js" integrity="sha384-w76AqPfDkMBDXo30jS1Sgez6pr3x5MlQ1ZAGC+nuZB+EYdgRZgiwxhTBTkF7CXvN" crossorigin="anonymous"></script>
     <script src="https://cdn.jsdelivr.net/npm/codemirror@5.57.0/lib/codemirror.js"></script>
     <script src="https://cdn.jsdelivr.net/npm/codemirror@5.57.0/mode/sql/sql.js"></script>
-
-    <!-- thank you GPT-4 -->
-    <style>
-      .relation-item {
-        white-space: nowrap;
-        overflow: hidden;
-        text-overflow: ellipsis;
-      }
-
-      .relation-link {
-        display: block;
-        max-width: 100%;
-      }
-
-      .relation-link:hover {
-        text-decoration: none;
-      }
-
-      .relation-column {
-        padding-left: 1.5rem;
-      }
-    </style>
-
   </head>
 
   <body>
     <header class="navbar navbar-dark sticky-top bg-dark flex-md-nowrap p-0 shadow">
       <a class="navbar-brand col-md-3 col-lg-2 me-0 px-3 fs-6" href="#">DuckDBT</a>
     </header>
     
@@ -87,15 +64,14 @@
           </div>
         </main>
       </div>
     </div>
 
     <script>
       function toggleColumns(relation) {
-        console.log("Whats up");
         const columnsList = document.getElementById(relation + "-columns");
         if (columnsList.style.display === "none") {
           columnsList.style.display = "block";
         } else {
           columnsList.style.display = "none";
         }
       }
```

#### html2text {}

```diff
@@ -1,10 +1,9 @@
 
 
-
  DuckDBT
 * Tables *
     * {% for relation, columns in relations.items() %}
     * {{_relation_}}
           o_{%_for_column_in_columns_%}
           o_{{_column_}}
           o_{%_endfor_%}
```

### Comparing `duckdbt-0.3.1/setup.py` & `duckdbt-0.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md")) as f:
     long_description = f.read()
 
 package_name = "duckdbt"
 
 
-package_version = "0.3.1"
+package_version = "0.3.2"
 description = """The Modern Data Stack in a Python Package"""
 
 setup(
     name=package_name,
     version=package_version,
     description=description,
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Josh Wills",
     author_email="joshwills+duckdbt@gmail.com",
     url="https://github.com/jwills/duckdbt",
     packages=find_namespace_packages(include=["duckdbt", "duckdbt.*"]),
     include_package_data=True,
     install_requires=[
-        "buenavista[duckdb]~=0.2.1",
+        "buenavista[duckdb]~=0.3.0",
         "dbt-duckdb~=1.5.0",
         "duckdb~=0.7.0",
         "fastapi[all]",
         "psycopg2-binary",
     ],
 )
```

