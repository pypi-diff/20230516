# Comparing `tmp/PostgreSQL-Audit-0.9.2.tar.gz` & `tmp/PostgreSQL-Audit-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PostgreSQL-Audit-0.9.2.tar", last modified: Wed Dec 13 15:35:18 2017, max compression
+gzip compressed data, was "dist/PostgreSQL-Audit-0.9.3.tar", last modified: Sun May 13 19:14:45 2018, max compression
```

## Comparing `PostgreSQL-Audit-0.9.2.tar` & `PostgreSQL-Audit-0.9.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2017-12-13 15:35:18.000000 PostgreSQL-Audit-0.9.2/
--rw-r--r--   0 konsta     (501) staff       (20)     4112 2017-12-13 15:28:01.000000 PostgreSQL-Audit-0.9.2/CHANGES.rst
--rw-r--r--   0 konsta     (501) staff       (20)     2864 2017-09-06 07:47:44.000000 PostgreSQL-Audit-0.9.2/conftest.py
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2017-12-13 15:35:18.000000 PostgreSQL-Audit-0.9.2/docs/
--rw-r--r--   0 konsta     (501) staff       (20)     6148 2015-04-14 14:43:41.000000 PostgreSQL-Audit-0.9.2/docs/.DS_Store
--rw-r--r--   0 konsta     (501) staff       (20)     8595 2015-03-02 15:10:29.000000 PostgreSQL-Audit-0.9.2/docs/conf.py
--rw-r--r--   0 konsta     (501) staff       (20)     3791 2016-01-09 19:29:09.000000 PostgreSQL-Audit-0.9.2/docs/flask.rst
--rw-r--r--   0 konsta     (501) staff       (20)      129 2015-04-13 11:12:05.000000 PostgreSQL-Audit-0.9.2/docs/index.rst
--rw-rw-r--   0 konsta     (501) staff       (20)     1276 2015-07-30 09:29:58.000000 PostgreSQL-Audit-0.9.2/docs/installation.rst
--rw-r--r--   0 konsta     (501) staff       (20)     6721 2015-03-02 15:03:29.000000 PostgreSQL-Audit-0.9.2/docs/make.bat
--rw-r--r--   0 konsta     (501) staff       (20)     6802 2015-03-02 15:03:29.000000 PostgreSQL-Audit-0.9.2/docs/Makefile
--rw-r--r--   0 konsta     (501) staff       (20)     1074 2016-03-27 11:59:43.000000 PostgreSQL-Audit-0.9.2/docs/migrations.rst
--rw-r--r--   0 konsta     (501) staff       (20)     4636 2017-09-06 13:59:15.000000 PostgreSQL-Audit-0.9.2/docs/sqlalchemy.rst
--rw-r--r--   0 konsta     (501) staff       (20)     1301 2015-02-08 14:13:07.000000 PostgreSQL-Audit-0.9.2/LICENSE
--rw-r--r--   0 konsta     (501) staff       (20)      297 2016-01-13 14:50:06.000000 PostgreSQL-Audit-0.9.2/MANIFEST.in
--rw-r--r--   0 konsta     (501) staff       (20)     1143 2017-12-13 15:35:18.000000 PostgreSQL-Audit-0.9.2/PKG-INFO
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2017-12-13 15:35:18.000000 PostgreSQL-Audit-0.9.2/postgresql_audit/
--rw-r--r--   0 konsta     (501) staff       (20)      347 2017-12-13 15:28:06.000000 PostgreSQL-Audit-0.9.2/postgresql_audit/__init__.py
--rw-r--r--   0 konsta     (501) staff       (20)    13803 2017-12-13 15:26:59.000000 PostgreSQL-Audit-0.9.2/postgresql_audit/base.py
--rw-r--r--   0 konsta     (501) staff       (20)      922 2017-09-06 13:59:15.000000 PostgreSQL-Audit-0.9.2/postgresql_audit/expressions.py
--rw-r--r--   0 konsta     (501) staff       (20)     1731 2016-09-12 15:20:55.000000 PostgreSQL-Audit-0.9.2/postgresql_audit/flask.py
--rw-r--r--   0 konsta     (501) staff       (20)     8738 2017-09-06 13:59:15.000000 PostgreSQL-Audit-0.9.2/postgresql_audit/migrations.py
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2017-12-13 15:35:18.000000 PostgreSQL-Audit-0.9.2/postgresql_audit/templates/
--rw-r--r--   0 konsta     (501) staff       (20)     1111 2017-10-10 10:19:18.000000 PostgreSQL-Audit-0.9.2/postgresql_audit/templates/audit_table_func.sql
--rw-r--r--   0 konsta     (501) staff       (20)     2110 2017-10-10 10:12:47.000000 PostgreSQL-Audit-0.9.2/postgresql_audit/templates/create_activity.sql
--rw-r--r--   0 konsta     (501) staff       (20)       79 2016-08-03 11:49:12.000000 PostgreSQL-Audit-0.9.2/postgresql_audit/templates/create_schema.sql
--rw-r--r--   0 konsta     (501) staff       (20)       35 2016-01-13 14:50:06.000000 PostgreSQL-Audit-0.9.2/postgresql_audit/templates/drop_schema.sql
--rw-r--r--   0 konsta     (501) staff       (20)      465 2017-12-13 15:26:59.000000 PostgreSQL-Audit-0.9.2/postgresql_audit/templates/operators.sql
--rw-r--r--   0 konsta     (501) staff       (20)      580 2017-12-13 15:26:59.000000 PostgreSQL-Audit-0.9.2/postgresql_audit/templates/operators_pre100.sql
--rw-r--r--   0 konsta     (501) staff       (20)     1093 2017-10-10 10:15:36.000000 PostgreSQL-Audit-0.9.2/postgresql_audit/templates/operators_pre95.sql
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2017-12-13 15:35:18.000000 PostgreSQL-Audit-0.9.2/PostgreSQL_Audit.egg-info/
--rw-r--r--   0 konsta     (501) staff       (20)        1 2017-12-13 15:35:18.000000 PostgreSQL-Audit-0.9.2/PostgreSQL_Audit.egg-info/dependency_links.txt
--rw-r--r--   0 konsta     (501) staff       (20)        1 2015-02-17 12:06:12.000000 PostgreSQL-Audit-0.9.2/PostgreSQL_Audit.egg-info/not-zip-safe
--rw-r--r--   0 konsta     (501) staff       (20)       47 2015-11-10 07:27:17.000000 PostgreSQL-Audit-0.9.2/PostgreSQL_Audit.egg-info/pbr.json
--rw-r--r--   0 konsta     (501) staff       (20)     1143 2017-12-13 15:35:18.000000 PostgreSQL-Audit-0.9.2/PostgreSQL_Audit.egg-info/PKG-INFO
--rw-r--r--   0 konsta     (501) staff       (20)       43 2017-12-13 15:35:18.000000 PostgreSQL-Audit-0.9.2/PostgreSQL_Audit.egg-info/requires.txt
--rw-r--r--   0 konsta     (501) staff       (20)     1187 2017-12-13 15:35:18.000000 PostgreSQL-Audit-0.9.2/PostgreSQL_Audit.egg-info/SOURCES.txt
--rw-r--r--   0 konsta     (501) staff       (20)       17 2017-12-13 15:35:18.000000 PostgreSQL-Audit-0.9.2/PostgreSQL_Audit.egg-info/top_level.txt
--rw-r--r--   0 konsta     (501) staff       (20)     3345 2016-03-27 11:59:42.000000 PostgreSQL-Audit-0.9.2/README.rst
--rw-r--r--   0 konsta     (501) staff       (20)       59 2017-12-13 15:35:18.000000 PostgreSQL-Audit-0.9.2/setup.cfg
--rw-r--r--   0 konsta     (501) staff       (20)     1770 2017-03-27 13:18:37.000000 PostgreSQL-Audit-0.9.2/setup.py
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2017-12-13 15:35:18.000000 PostgreSQL-Audit-0.9.2/tests/
--rw-r--r--   0 konsta     (501) staff       (20)        0 2015-04-13 18:47:56.000000 PostgreSQL-Audit-0.9.2/tests/__init__.py
--rw-r--r--   0 konsta     (501) staff       (20)     5435 2017-09-06 13:59:15.000000 PostgreSQL-Audit-0.9.2/tests/test_custom_schema.py
--rw-r--r--   0 konsta     (501) staff       (20)     5844 2016-09-12 15:20:55.000000 PostgreSQL-Audit-0.9.2/tests/test_flask_integration.py
--rw-r--r--   0 konsta     (501) staff       (20)     2936 2017-09-06 13:59:15.000000 PostgreSQL-Audit-0.9.2/tests/test_json_functions.py
--rw-r--r--   0 konsta     (501) staff       (20)     5875 2017-09-06 13:59:15.000000 PostgreSQL-Audit-0.9.2/tests/test_migration_functions.py
--rw-r--r--   0 konsta     (501) staff       (20)     1612 2017-12-13 15:26:59.000000 PostgreSQL-Audit-0.9.2/tests/test_operators.py
--rw-r--r--   0 konsta     (501) staff       (20)     1919 2017-09-06 13:59:15.000000 PostgreSQL-Audit-0.9.2/tests/test_sql_files.py
--rw-r--r--   0 konsta     (501) staff       (20)    10894 2017-09-06 13:59:15.000000 PostgreSQL-Audit-0.9.2/tests/test_sqlalchemy_integration.py
--rw-r--r--   0 konsta     (501) staff       (20)      333 2016-01-13 14:50:06.000000 PostgreSQL-Audit-0.9.2/tests/utils.py
+drwxr-xr-x   0 konsta     (501) staff       (20)        0 2018-05-13 19:14:45.000000 PostgreSQL-Audit-0.9.3/
+-rw-r--r--   0 konsta     (501) staff       (20)     4251 2018-05-13 19:05:13.000000 PostgreSQL-Audit-0.9.3/CHANGES.rst
+-rw-r--r--   0 konsta     (501) staff       (20)     2864 2017-09-06 07:47:44.000000 PostgreSQL-Audit-0.9.3/conftest.py
+drwxr-xr-x   0 konsta     (501) staff       (20)        0 2018-05-13 19:14:45.000000 PostgreSQL-Audit-0.9.3/docs/
+-rw-r--r--   0 konsta     (501) staff       (20)     6148 2015-04-14 14:43:41.000000 PostgreSQL-Audit-0.9.3/docs/.DS_Store
+-rw-r--r--   0 konsta     (501) staff       (20)     8595 2015-03-02 15:10:29.000000 PostgreSQL-Audit-0.9.3/docs/conf.py
+-rw-r--r--   0 konsta     (501) staff       (20)     3791 2016-01-09 19:29:09.000000 PostgreSQL-Audit-0.9.3/docs/flask.rst
+-rw-r--r--   0 konsta     (501) staff       (20)      129 2015-04-13 11:12:05.000000 PostgreSQL-Audit-0.9.3/docs/index.rst
+-rw-rw-r--   0 konsta     (501) staff       (20)     1276 2015-07-30 09:29:58.000000 PostgreSQL-Audit-0.9.3/docs/installation.rst
+-rw-r--r--   0 konsta     (501) staff       (20)     6721 2015-03-02 15:03:29.000000 PostgreSQL-Audit-0.9.3/docs/make.bat
+-rw-r--r--   0 konsta     (501) staff       (20)     6802 2015-03-02 15:03:29.000000 PostgreSQL-Audit-0.9.3/docs/Makefile
+-rw-r--r--   0 konsta     (501) staff       (20)     1074 2016-03-27 11:59:43.000000 PostgreSQL-Audit-0.9.3/docs/migrations.rst
+-rw-r--r--   0 konsta     (501) staff       (20)     4636 2017-09-06 13:59:15.000000 PostgreSQL-Audit-0.9.3/docs/sqlalchemy.rst
+-rw-r--r--   0 konsta     (501) staff       (20)     1301 2015-02-08 14:13:07.000000 PostgreSQL-Audit-0.9.3/LICENSE
+-rw-r--r--   0 konsta     (501) staff       (20)      297 2016-01-13 14:50:06.000000 PostgreSQL-Audit-0.9.3/MANIFEST.in
+-rw-r--r--   0 konsta     (501) staff       (20)     1093 2018-05-13 19:14:45.000000 PostgreSQL-Audit-0.9.3/PKG-INFO
+drwxr-xr-x   0 konsta     (501) staff       (20)        0 2018-05-13 19:14:45.000000 PostgreSQL-Audit-0.9.3/postgresql_audit/
+-rw-r--r--   0 konsta     (501) staff       (20)      347 2018-05-13 19:03:14.000000 PostgreSQL-Audit-0.9.3/postgresql_audit/__init__.py
+-rw-r--r--   0 konsta     (501) staff       (20)    13825 2018-04-09 18:43:18.000000 PostgreSQL-Audit-0.9.3/postgresql_audit/base.py
+-rw-r--r--   0 konsta     (501) staff       (20)      922 2017-09-06 13:59:15.000000 PostgreSQL-Audit-0.9.3/postgresql_audit/expressions.py
+-rw-r--r--   0 konsta     (501) staff       (20)     1731 2016-09-12 15:20:55.000000 PostgreSQL-Audit-0.9.3/postgresql_audit/flask.py
+-rw-r--r--   0 konsta     (501) staff       (20)     8738 2017-09-06 13:59:15.000000 PostgreSQL-Audit-0.9.3/postgresql_audit/migrations.py
+drwxr-xr-x   0 konsta     (501) staff       (20)        0 2018-05-13 19:14:45.000000 PostgreSQL-Audit-0.9.3/postgresql_audit/templates/
+-rw-r--r--   0 konsta     (501) staff       (20)     1111 2017-10-10 10:19:18.000000 PostgreSQL-Audit-0.9.3/postgresql_audit/templates/audit_table_func.sql
+-rw-r--r--   0 konsta     (501) staff       (20)     2129 2018-04-09 18:43:18.000000 PostgreSQL-Audit-0.9.3/postgresql_audit/templates/create_activity.sql
+-rw-r--r--   0 konsta     (501) staff       (20)       79 2016-08-03 11:49:12.000000 PostgreSQL-Audit-0.9.3/postgresql_audit/templates/create_schema.sql
+-rw-r--r--   0 konsta     (501) staff       (20)       35 2016-01-13 14:50:06.000000 PostgreSQL-Audit-0.9.3/postgresql_audit/templates/drop_schema.sql
+-rw-r--r--   0 konsta     (501) staff       (20)      465 2017-12-13 15:26:59.000000 PostgreSQL-Audit-0.9.3/postgresql_audit/templates/operators.sql
+-rw-r--r--   0 konsta     (501) staff       (20)      580 2017-12-13 15:26:59.000000 PostgreSQL-Audit-0.9.3/postgresql_audit/templates/operators_pre100.sql
+-rw-r--r--   0 konsta     (501) staff       (20)     1093 2017-10-10 10:15:36.000000 PostgreSQL-Audit-0.9.3/postgresql_audit/templates/operators_pre95.sql
+drwxr-xr-x   0 konsta     (501) staff       (20)        0 2018-05-13 19:14:45.000000 PostgreSQL-Audit-0.9.3/PostgreSQL_Audit.egg-info/
+-rw-r--r--   0 konsta     (501) staff       (20)        1 2018-05-13 19:14:45.000000 PostgreSQL-Audit-0.9.3/PostgreSQL_Audit.egg-info/dependency_links.txt
+-rw-r--r--   0 konsta     (501) staff       (20)        1 2015-02-17 12:06:12.000000 PostgreSQL-Audit-0.9.3/PostgreSQL_Audit.egg-info/not-zip-safe
+-rw-r--r--   0 konsta     (501) staff       (20)       47 2015-11-10 07:27:17.000000 PostgreSQL-Audit-0.9.3/PostgreSQL_Audit.egg-info/pbr.json
+-rw-r--r--   0 konsta     (501) staff       (20)     1093 2018-05-13 19:14:45.000000 PostgreSQL-Audit-0.9.3/PostgreSQL_Audit.egg-info/PKG-INFO
+-rw-r--r--   0 konsta     (501) staff       (20)       43 2018-05-13 19:14:45.000000 PostgreSQL-Audit-0.9.3/PostgreSQL_Audit.egg-info/requires.txt
+-rw-r--r--   0 konsta     (501) staff       (20)     1187 2018-05-13 19:14:45.000000 PostgreSQL-Audit-0.9.3/PostgreSQL_Audit.egg-info/SOURCES.txt
+-rw-r--r--   0 konsta     (501) staff       (20)       17 2018-05-13 19:14:45.000000 PostgreSQL-Audit-0.9.3/PostgreSQL_Audit.egg-info/top_level.txt
+-rw-r--r--   0 konsta     (501) staff       (20)     3345 2016-03-27 11:59:42.000000 PostgreSQL-Audit-0.9.3/README.rst
+-rw-r--r--   0 konsta     (501) staff       (20)       59 2018-05-13 19:14:45.000000 PostgreSQL-Audit-0.9.3/setup.cfg
+-rw-r--r--   0 konsta     (501) staff       (20)     1721 2018-05-13 19:05:16.000000 PostgreSQL-Audit-0.9.3/setup.py
+drwxr-xr-x   0 konsta     (501) staff       (20)        0 2018-05-13 19:14:45.000000 PostgreSQL-Audit-0.9.3/tests/
+-rw-r--r--   0 konsta     (501) staff       (20)        0 2015-04-13 18:47:56.000000 PostgreSQL-Audit-0.9.3/tests/__init__.py
+-rw-r--r--   0 konsta     (501) staff       (20)     5435 2017-09-06 13:59:15.000000 PostgreSQL-Audit-0.9.3/tests/test_custom_schema.py
+-rw-r--r--   0 konsta     (501) staff       (20)     5844 2016-09-12 15:20:55.000000 PostgreSQL-Audit-0.9.3/tests/test_flask_integration.py
+-rw-r--r--   0 konsta     (501) staff       (20)     2936 2017-09-06 13:59:15.000000 PostgreSQL-Audit-0.9.3/tests/test_json_functions.py
+-rw-r--r--   0 konsta     (501) staff       (20)     5875 2017-09-06 13:59:15.000000 PostgreSQL-Audit-0.9.3/tests/test_migration_functions.py
+-rw-r--r--   0 konsta     (501) staff       (20)     1612 2017-12-13 15:26:59.000000 PostgreSQL-Audit-0.9.3/tests/test_operators.py
+-rw-r--r--   0 konsta     (501) staff       (20)     1919 2017-09-06 13:59:15.000000 PostgreSQL-Audit-0.9.3/tests/test_sql_files.py
+-rw-r--r--   0 konsta     (501) staff       (20)    10894 2017-09-06 13:59:15.000000 PostgreSQL-Audit-0.9.3/tests/test_sqlalchemy_integration.py
+-rw-r--r--   0 konsta     (501) staff       (20)      333 2016-01-13 14:50:06.000000 PostgreSQL-Audit-0.9.3/tests/utils.py
```

### Comparing `PostgreSQL-Audit-0.9.2/CHANGES.rst` & `PostgreSQL-Audit-0.9.3/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 Changelog
 ---------
 
 Here you can see the full list of changes between each PostgreSQL-Audit release.
 
 
+0.9.3 (2018-05-13)
+^^^^^^^^^^^^^^^^^^
+
+- Force timestamps to use UTC as timezone (#30, courtesy of quantus)
+- Dropped Python 3.3 support
+
+
 0.9.2 (2017-12-13)
 ^^^^^^^^^^^^^^^^^^
 
 - Added PostgreSQL 10 support
 
 
 0.9.1 (2017-10-10)
```

### Comparing `PostgreSQL-Audit-0.9.2/conftest.py` & `PostgreSQL-Audit-0.9.3/conftest.py`

 * *Files identical despite different names*

### Comparing `PostgreSQL-Audit-0.9.2/docs/.DS_Store` & `PostgreSQL-Audit-0.9.3/docs/.DS_Store`

 * *Files identical despite different names*

### Comparing `PostgreSQL-Audit-0.9.2/docs/conf.py` & `PostgreSQL-Audit-0.9.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `PostgreSQL-Audit-0.9.2/docs/flask.rst` & `PostgreSQL-Audit-0.9.3/docs/flask.rst`

 * *Files identical despite different names*

### Comparing `PostgreSQL-Audit-0.9.2/docs/installation.rst` & `PostgreSQL-Audit-0.9.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `PostgreSQL-Audit-0.9.2/docs/make.bat` & `PostgreSQL-Audit-0.9.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `PostgreSQL-Audit-0.9.2/docs/Makefile` & `PostgreSQL-Audit-0.9.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `PostgreSQL-Audit-0.9.2/docs/migrations.rst` & `PostgreSQL-Audit-0.9.3/docs/migrations.rst`

 * *Files identical despite different names*

### Comparing `PostgreSQL-Audit-0.9.2/docs/sqlalchemy.rst` & `PostgreSQL-Audit-0.9.3/docs/sqlalchemy.rst`

 * *Files identical despite different names*

### Comparing `PostgreSQL-Audit-0.9.2/LICENSE` & `PostgreSQL-Audit-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PostgreSQL-Audit-0.9.2/PKG-INFO` & `PostgreSQL-Audit-0.9.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: PostgreSQL-Audit
-Version: 0.9.2
+Version: 0.9.3
 Summary: Versioning and auditing extension for PostgreSQL and SQLAlchemy.
 Home-page: https://github.com/kvesteri/postgresql-audit
 Author: Konsta Vesterinen
 Author-email: konsta@fastmonkeys.com
 License: BSD
 Description: 
         PostgreSQL-Audit
@@ -17,13 +17,12 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `PostgreSQL-Audit-0.9.2/postgresql_audit/base.py` & `PostgreSQL-Audit-0.9.3/postgresql_audit/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,15 +270,15 @@
                 RuntimeWarning
             )
             return
 
         values = convert_callables(self.get_transaction_values())
         if values:
             values['native_transaction_id'] = sa.func.txid_current()
-            values['issued_at'] = sa.func.now()
+            values['issued_at'] = sa.text("now() AT TIME ZONE 'UTC'")
             stmt = (
                 table
                 .insert()
                 .values(**values)
             )
             session.execute(stmt)
```

### Comparing `PostgreSQL-Audit-0.9.2/postgresql_audit/expressions.py` & `PostgreSQL-Audit-0.9.3/postgresql_audit/expressions.py`

 * *Files identical despite different names*

### Comparing `PostgreSQL-Audit-0.9.2/postgresql_audit/flask.py` & `PostgreSQL-Audit-0.9.3/postgresql_audit/flask.py`

 * *Files identical despite different names*

### Comparing `PostgreSQL-Audit-0.9.2/postgresql_audit/migrations.py` & `PostgreSQL-Audit-0.9.3/postgresql_audit/migrations.py`

 * *Files identical despite different names*

### Comparing `PostgreSQL-Audit-0.9.2/postgresql_audit/templates/audit_table_func.sql` & `PostgreSQL-Audit-0.9.3/postgresql_audit/templates/audit_table_func.sql`

 * *Files identical despite different names*

### Comparing `PostgreSQL-Audit-0.9.2/postgresql_audit/templates/create_activity.sql` & `PostgreSQL-Audit-0.9.3/postgresql_audit/templates/create_activity.sql`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     audit_row ${schema_prefix}activity;
     excluded_cols text[] = ARRAY[]::text[];
 BEGIN
     audit_row.id = nextval('${schema_prefix}activity_id_seq');
     audit_row.schema_name = TG_TABLE_SCHEMA::text;
     audit_row.table_name = TG_TABLE_NAME::text;
     audit_row.relid = TG_RELID;
-    audit_row.issued_at = statement_timestamp();
+    audit_row.issued_at = statement_timestamp() AT TIME ZONE 'UTC';
     audit_row.native_transaction_id = txid_current();
     audit_row.transaction_id = (
         SELECT id
         FROM ${schema_prefix}transaction
         WHERE
             native_transaction_id = txid_current() AND
             issued_at >= (NOW() - INTERVAL '1 day')
```

### Comparing `PostgreSQL-Audit-0.9.2/postgresql_audit/templates/operators_pre100.sql` & `PostgreSQL-Audit-0.9.3/postgresql_audit/templates/operators_pre100.sql`

 * *Files identical despite different names*

### Comparing `PostgreSQL-Audit-0.9.2/postgresql_audit/templates/operators_pre95.sql` & `PostgreSQL-Audit-0.9.3/postgresql_audit/templates/operators_pre95.sql`

 * *Files identical despite different names*

### Comparing `PostgreSQL-Audit-0.9.2/PostgreSQL_Audit.egg-info/PKG-INFO` & `PostgreSQL-Audit-0.9.3/PostgreSQL_Audit.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: PostgreSQL-Audit
-Version: 0.9.2
+Version: 0.9.3
 Summary: Versioning and auditing extension for PostgreSQL and SQLAlchemy.
 Home-page: https://github.com/kvesteri/postgresql-audit
 Author: Konsta Vesterinen
 Author-email: konsta@fastmonkeys.com
 License: BSD
 Description: 
         PostgreSQL-Audit
@@ -17,13 +17,12 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `PostgreSQL-Audit-0.9.2/PostgreSQL_Audit.egg-info/SOURCES.txt` & `PostgreSQL-Audit-0.9.3/PostgreSQL_Audit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PostgreSQL-Audit-0.9.2/README.rst` & `PostgreSQL-Audit-0.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `PostgreSQL-Audit-0.9.2/setup.py` & `PostgreSQL-Audit-0.9.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,14 @@
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.3',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
         'Topic :: Software Development :: Libraries :: Python Modules'
     ]
 )
```

### Comparing `PostgreSQL-Audit-0.9.2/tests/test_custom_schema.py` & `PostgreSQL-Audit-0.9.3/tests/test_custom_schema.py`

 * *Files identical despite different names*

### Comparing `PostgreSQL-Audit-0.9.2/tests/test_flask_integration.py` & `PostgreSQL-Audit-0.9.3/tests/test_flask_integration.py`

 * *Files identical despite different names*

### Comparing `PostgreSQL-Audit-0.9.2/tests/test_json_functions.py` & `PostgreSQL-Audit-0.9.3/tests/test_json_functions.py`

 * *Files identical despite different names*

### Comparing `PostgreSQL-Audit-0.9.2/tests/test_migration_functions.py` & `PostgreSQL-Audit-0.9.3/tests/test_migration_functions.py`

 * *Files identical despite different names*

### Comparing `PostgreSQL-Audit-0.9.2/tests/test_operators.py` & `PostgreSQL-Audit-0.9.3/tests/test_operators.py`

 * *Files identical despite different names*

### Comparing `PostgreSQL-Audit-0.9.2/tests/test_sql_files.py` & `PostgreSQL-Audit-0.9.3/tests/test_sql_files.py`

 * *Files identical despite different names*

### Comparing `PostgreSQL-Audit-0.9.2/tests/test_sqlalchemy_integration.py` & `PostgreSQL-Audit-0.9.3/tests/test_sqlalchemy_integration.py`

 * *Files identical despite different names*

