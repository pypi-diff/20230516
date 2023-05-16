# Comparing `tmp/dbt_superset_lineage-0.3.0.tar.gz` & `tmp/dbt_superset_lineage-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_superset_lineage-0.3.0.tar", max compression
+gzip compressed data, was "dbt_superset_lineage-0.3.1.tar", max compression
```

## Comparing `dbt_superset_lineage-0.3.0.tar` & `dbt_superset_lineage-0.3.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1062 2021-12-03 09:02:37.138885 dbt_superset_lineage-0.3.0/LICENSE.md
--rw-r--r--   0        0        0     4774 2023-03-28 19:49:49.244002 dbt_superset_lineage-0.3.0/README.md
--rw-r--r--   0        0        0     6148 2023-03-30 16:32:49.836101 dbt_superset_lineage-0.3.0/dbt_superset_lineage/.DS_Store
--rw-r--r--   0        0        0     4506 2023-04-03 14:26:54.290955 dbt_superset_lineage-0.3.0/dbt_superset_lineage/__init__.py
--rw-r--r--   0        0        0    14162 2023-04-03 20:24:19.463013 dbt_superset_lineage-0.3.0/dbt_superset_lineage/pull_dashboards.py
--rw-r--r--   0        0        0     8841 2023-04-03 20:24:19.465744 dbt_superset_lineage-0.3.0/dbt_superset_lineage/push_descriptions.py
--rw-r--r--   0        0        0     3370 2023-03-21 10:17:38.771099 dbt_superset_lineage-0.3.0/dbt_superset_lineage/superset_api.py
--rw-r--r--   0        0        0      642 2023-04-03 20:36:48.266666 dbt_superset_lineage-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     5735 1970-01-01 00:00:00.000000 dbt_superset_lineage-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2021-12-03 09:02:37.138885 dbt_superset_lineage-0.3.1/LICENSE.md
+-rw-r--r--   0        0        0     4774 2023-03-28 19:49:49.244002 dbt_superset_lineage-0.3.1/README.md
+-rw-r--r--   0        0        0     6148 2023-03-30 16:32:49.836101 dbt_superset_lineage-0.3.1/dbt_superset_lineage/.DS_Store
+-rw-r--r--   0        0        0     4506 2023-04-03 14:26:54.290955 dbt_superset_lineage-0.3.1/dbt_superset_lineage/__init__.py
+-rw-r--r--   0        0        0    14162 2023-04-03 20:24:19.463013 dbt_superset_lineage-0.3.1/dbt_superset_lineage/pull_dashboards.py
+-rw-r--r--   0        0        0     8842 2023-05-16 14:38:20.272268 dbt_superset_lineage-0.3.1/dbt_superset_lineage/push_descriptions.py
+-rw-r--r--   0        0        0     3370 2023-03-21 10:17:38.771099 dbt_superset_lineage-0.3.1/dbt_superset_lineage/superset_api.py
+-rw-r--r--   0        0        0      642 2023-05-16 14:38:58.519322 dbt_superset_lineage-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5735 1970-01-01 00:00:00.000000 dbt_superset_lineage-0.3.1/PKG-INFO
```

### Comparing `dbt_superset_lineage-0.3.0/LICENSE.md` & `dbt_superset_lineage-0.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dbt_superset_lineage-0.3.0/README.md` & `dbt_superset_lineage-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `dbt_superset_lineage-0.3.0/dbt_superset_lineage/.DS_Store` & `dbt_superset_lineage-0.3.1/dbt_superset_lineage/.DS_Store`

 * *Files identical despite different names*

### Comparing `dbt_superset_lineage-0.3.0/dbt_superset_lineage/__init__.py` & `dbt_superset_lineage-0.3.1/dbt_superset_lineage/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_superset_lineage-0.3.0/dbt_superset_lineage/pull_dashboards.py` & `dbt_superset_lineage-0.3.1/dbt_superset_lineage/pull_dashboards.py`

 * *Files identical despite different names*

### Comparing `dbt_superset_lineage-0.3.0/dbt_superset_lineage/push_descriptions.py` & `dbt_superset_lineage-0.3.1/dbt_superset_lineage/push_descriptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,15 +202,15 @@
         'id': col['id'],
         'description': col['description']
     } for col in dataset['columns']]
 
     if description_new != description_old or \
        not check_columns_equal(columns_new, columns_old):
         payload = {'description': description_new, 'columns': columns_new}
-        superset.request('PUT', f"/dataset/{dataset['id']}?override_columns=true", json=payload)
+        superset.request('PUT', f"/dataset/{dataset['id']}?override_columns=false", json=payload)
     else:
         logging.info("Skipping PUT execute request as nothing would be updated.")
 
 
 def main(dbt_project_dir, dbt_db_name,
          superset_url, superset_db_id, superset_refresh_columns,
          superset_access_token, superset_refresh_token):
```

### Comparing `dbt_superset_lineage-0.3.0/dbt_superset_lineage/superset_api.py` & `dbt_superset_lineage-0.3.1/dbt_superset_lineage/superset_api.py`

 * *Files identical despite different names*

### Comparing `dbt_superset_lineage-0.3.0/pyproject.toml` & `dbt_superset_lineage-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbt-superset-lineage"
-version = "0.3.0"
+version = "0.3.1"
 description = "Make dbt docs and Apache Superset talk to one another"
 authors = ["Michal Kolacek <mkolacek@slido.com>"]
 readme = "README.md"
 repository = "https://github.com/slidoapp/dbt-superset-lineage"
 
 [tool.poetry.scripts]
 dbt-superset-lineage = "dbt_superset_lineage.__init__:app"
```

### Comparing `dbt_superset_lineage-0.3.0/PKG-INFO` & `dbt_superset_lineage-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-superset-lineage
-Version: 0.3.0
+Version: 0.3.1
 Summary: Make dbt docs and Apache Superset talk to one another
 Home-page: https://github.com/slidoapp/dbt-superset-lineage
 Author: Michal Kolacek
 Author-email: mkolacek@slido.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-superset-lineage Version: 0.3.0 Summary: Make
+Metadata-Version: 2.1 Name: dbt-superset-lineage Version: 0.3.1 Summary: Make
 dbt docs and Apache Superset talk to one another Home-page: https://github.com/
 slidoapp/dbt-superset-lineage Author: Michal Kolacek Author-email:
 mkolacek@slido.com Requires-Python: >=3.8,<4.0 Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
 Dist: Markdown (>=3.3.6,<4.0.0) Requires-Dist: bs4 (>=0.0.1,<0.0.2) Requires-
```

