# Comparing `tmp/dbpoolpy-0.6.5.tar.gz` & `tmp/dbpoolpy-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/root/user/proj/dbpoolpy/dist/.tmp-o2gaufso/dbpoolpy-0.6.5.tar", last modified: Tue Dec 20 07:09:28 2022, max compression
+gzip compressed data, was "/mnt/e/jiutian/pyproj/dbpoolpy/dist/.tmp-srw9na__/dbpoolpy-0.6.6.tar", last modified: Tue May 16 04:37:50 2023, max compression
```

## Comparing `dbpoolpy-0.6.5.tar` & `dbpoolpy-0.6.6.tar`

### file list

```diff
@@ -1,35 +1,53 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 07:09:28.427567 dbpoolpy-0.6.5/
--rw-r--r--   0 root         (0) root         (0)     1064 2021-07-08 06:56:01.000000 dbpoolpy-0.6.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)      397 2022-12-20 07:09:28.428565 dbpoolpy-0.6.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13156 2022-12-07 10:55:42.000000 dbpoolpy-0.6.5/README.md
--rw-r--r--   0 root         (0) root         (0)       90 2021-07-08 04:50:17.000000 dbpoolpy-0.6.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      747 2022-12-20 07:09:28.431567 dbpoolpy-0.6.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      152 2022-03-04 05:11:41.000000 dbpoolpy-0.6.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 07:09:28.193559 dbpoolpy-0.6.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 07:09:28.277564 dbpoolpy-0.6.5/src/dbpoolpy/
--rw-r--r--   0 root         (0) root         (0)      403 2022-12-07 10:41:22.000000 dbpoolpy-0.6.5/src/dbpoolpy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 07:09:28.341563 dbpoolpy-0.6.5/src/dbpoolpy/config/
--rw-r--r--   0 root         (0) root         (0)    10663 2021-09-03 10:40:36.000000 dbpoolpy-0.6.5/src/dbpoolpy/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-03 10:39:50.000000 dbpoolpy-0.6.5/src/dbpoolpy/config/custom_settings.py
--rw-r--r--   0 root         (0) root         (0)      233 2022-12-07 10:37:58.000000 dbpoolpy-0.6.5/src/dbpoolpy/config/default_settings.py
--rw-r--r--   0 root         (0) root         (0)    14155 2021-09-03 10:31:52.000000 dbpoolpy-0.6.5/src/dbpoolpy/config/functional.py
--rw-r--r--   0 root         (0) root         (0)      732 2022-12-07 10:37:56.000000 dbpoolpy-0.6.5/src/dbpoolpy/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 07:09:28.392570 dbpoolpy-0.6.5/src/dbpoolpy/dbconnect/
--rw-r--r--   0 root         (0) root         (0)     3762 2022-08-02 03:25:55.000000 dbpoolpy-0.6.5/src/dbpoolpy/dbconnect/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2293 2022-08-02 04:18:13.000000 dbpoolpy-0.6.5/src/dbpoolpy/dbconnect/mysql.py
--rw-r--r--   0 root         (0) root         (0)      594 2022-04-16 04:34:02.000000 dbpoolpy-0.6.5/src/dbpoolpy/dbconnect/postgresql.py
--rw-r--r--   0 root         (0) root         (0)     2565 2022-01-21 09:38:31.000000 dbpoolpy-0.6.5/src/dbpoolpy/dbconnect/simple.py
--rw-r--r--   0 root         (0) root         (0)      270 2022-04-16 04:33:56.000000 dbpoolpy-0.6.5/src/dbpoolpy/dbconnect/sqlite3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 07:09:28.423574 dbpoolpy-0.6.5/src/dbpoolpy/dbhelper/
--rw-r--r--   0 root         (0) root         (0)    23412 2022-07-27 14:58:20.000000 dbpoolpy-0.6.5/src/dbpoolpy/dbhelper/__init__.py
--rw-r--r--   0 root         (0) root         (0)      645 2022-01-21 13:35:26.000000 dbpoolpy-0.6.5/src/dbpoolpy/dbhelper/mysql.py
--rw-r--r--   0 root         (0) root         (0)      976 2022-01-21 13:36:33.000000 dbpoolpy-0.6.5/src/dbpoolpy/dbhelper/postgresql.py
--rw-r--r--   0 root         (0) root         (0)       99 2022-01-21 13:34:18.000000 dbpoolpy-0.6.5/src/dbpoolpy/dbhelper/sqlite3.py
--rw-r--r--   0 root         (0) root         (0)    10097 2022-12-07 10:36:58.000000 dbpoolpy-0.6.5/src/dbpoolpy/dbpool.py
--rw-r--r--   0 root         (0) root         (0)     7822 2022-12-07 09:23:02.000000 dbpoolpy-0.6.5/src/dbpoolpy/table.py
--rw-r--r--   0 root         (0) root         (0)     5108 2022-12-07 10:37:01.000000 dbpoolpy-0.6.5/src/dbpoolpy/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 07:09:28.312563 dbpoolpy-0.6.5/src/dbpoolpy.egg-info/
--rw-r--r--   0 root         (0) root         (0)      397 2022-12-20 07:09:28.000000 dbpoolpy-0.6.5/src/dbpoolpy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      763 2022-12-20 07:09:28.000000 dbpoolpy-0.6.5/src/dbpoolpy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-20 07:09:28.000000 dbpoolpy-0.6.5/src/dbpoolpy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2022-12-20 07:09:28.000000 dbpoolpy-0.6.5/src/dbpoolpy.egg-info/top_level.txt
+drwxrwxrwx   0 zsq       (1000) zsq       (1000)        0 2023-05-16 04:37:50.250159 dbpoolpy-0.6.6/
+drwxrwxrwx   0 zsq       (1000) zsq       (1000)        0 2023-05-16 04:37:49.674936 dbpoolpy-0.6.6/.gitee/
+-rwxrwxrwx   0 zsq       (1000) zsq       (1000)       79 2023-05-16 03:22:18.000000 dbpoolpy-0.6.6/.gitee/ISSUE_TEMPLATE.zh-CN.md
+-rwxrwxrwx   0 zsq       (1000) zsq       (1000)      182 2023-05-16 03:22:18.000000 dbpoolpy-0.6.6/.gitee/PULL_REQUEST_TEMPLATE.zh-CN.md
+-rwxrwxrwx   0 zsq       (1000) zsq       (1000)     1388 2023-05-16 03:22:18.000000 dbpoolpy-0.6.6/.gitignore
+-rwxrwxrwx   0 zsq       (1000) zsq       (1000)     4726 2023-05-16 03:37:59.000000 dbpoolpy-0.6.6/CHANGES.rst
+-rwxrwxrwx   0 zsq       (1000) zsq       (1000)     1064 2023-05-16 03:22:18.000000 dbpoolpy-0.6.6/LICENSE
+-rwxrwxrwx   0 zsq       (1000) zsq       (1000)      397 2023-05-16 04:37:50.251159 dbpoolpy-0.6.6/PKG-INFO
+-rwxrwxrwx   0 zsq       (1000) zsq       (1000)      872 2023-05-16 03:22:18.000000 dbpoolpy-0.6.6/README.en.md
+-rwxrwxrwx   0 zsq       (1000) zsq       (1000)    13187 2023-05-16 03:22:18.000000 dbpoolpy-0.6.6/README.md
+drwxrwxrwx   0 zsq       (1000) zsq       (1000)        0 2023-05-16 04:37:49.511412 dbpoolpy-0.6.6/example/
+drwxrwxrwx   0 zsq       (1000) zsq       (1000)        0 2023-05-16 04:37:49.691936 dbpoolpy-0.6.6/example/db/
+-rwxrwxrwx   0 zsq       (1000) zsq       (1000)      558 2023-05-16 03:22:19.000000 dbpoolpy-0.6.6/example/db/__init__.py
+-rwxrwxrwx   0 zsq       (1000) zsq       (1000)       90 2023-05-16 03:22:19.000000 dbpoolpy-0.6.6/pyproject.toml
+-rwxrwxrwx   0 zsq       (1000) zsq       (1000)      626 2023-05-16 03:22:19.000000 dbpoolpy-0.6.6/requestments.txt
+drwxrwxrwx   0 zsq       (1000) zsq       (1000)        0 2023-05-16 04:37:49.707936 dbpoolpy-0.6.6/script/
+-rwxrwxrwx   0 zsq       (1000) zsq       (1000)      645 2023-05-16 03:22:19.000000 dbpoolpy-0.6.6/script/postgresql_test.py
+-rwxrwxrwx   0 zsq       (1000) zsq       (1000)      747 2023-05-16 04:37:50.256159 dbpoolpy-0.6.6/setup.cfg
+-rwxrwxrwx   0 zsq       (1000) zsq       (1000)      152 2023-05-16 03:22:19.000000 dbpoolpy-0.6.6/setup.py
+drwxrwxrwx   0 zsq       (1000) zsq       (1000)        0 2023-05-16 04:37:49.522412 dbpoolpy-0.6.6/src/
+drwxrwxrwx   0 zsq       (1000) zsq       (1000)        0 2023-05-16 04:37:49.801160 dbpoolpy-0.6.6/src/dbpoolpy/
+-rwxrwxrwx   0 zsq       (1000) zsq       (1000)      403 2023-05-16 03:38:11.000000 dbpoolpy-0.6.6/src/dbpoolpy/__init__.py
+drwxrwxrwx   0 zsq       (1000) zsq       (1000)        0 2023-05-16 04:37:49.966161 dbpoolpy-0.6.6/src/dbpoolpy/config/
+-rwxrwxrwx   0 zsq       (1000) zsq       (1000)    10663 2023-05-16 03:22:18.000000 dbpoolpy-0.6.6/src/dbpoolpy/config/__init__.py
+-rwxrwxrwx   0 zsq       (1000) zsq       (1000)        0 2023-05-16 03:22:18.000000 dbpoolpy-0.6.6/src/dbpoolpy/config/custom_settings.py
+-rwxrwxrwx   0 zsq       (1000) zsq       (1000)      233 2023-05-16 03:22:18.000000 dbpoolpy-0.6.6/src/dbpoolpy/config/default_settings.py
+-rwxrwxrwx   0 zsq       (1000) zsq       (1000)    14155 2023-05-16 03:22:18.000000 dbpoolpy-0.6.6/src/dbpoolpy/config/functional.py
+-rwxrwxrwx   0 zsq       (1000) zsq       (1000)      732 2023-05-16 03:22:18.000000 dbpoolpy-0.6.6/src/dbpoolpy/constants.py
+drwxrwxrwx   0 zsq       (1000) zsq       (1000)        0 2023-05-16 04:37:50.082161 dbpoolpy-0.6.6/src/dbpoolpy/dbconnect/
+-rwxrwxrwx   0 zsq       (1000) zsq       (1000)     3762 2023-05-16 03:22:18.000000 dbpoolpy-0.6.6/src/dbpoolpy/dbconnect/__init__.py
+-rwxrwxrwx   0 zsq       (1000) zsq       (1000)     2293 2023-05-16 03:22:18.000000 dbpoolpy-0.6.6/src/dbpoolpy/dbconnect/mysql.py
+-rwxrwxrwx   0 zsq       (1000) zsq       (1000)      594 2023-05-16 03:22:18.000000 dbpoolpy-0.6.6/src/dbpoolpy/dbconnect/postgresql.py
+-rwxrwxrwx   0 zsq       (1000) zsq       (1000)     2565 2023-05-16 03:22:18.000000 dbpoolpy-0.6.6/src/dbpoolpy/dbconnect/simple.py
+-rwxrwxrwx   0 zsq       (1000) zsq       (1000)      270 2023-05-16 03:22:18.000000 dbpoolpy-0.6.6/src/dbpoolpy/dbconnect/sqlite3.py
+drwxrwxrwx   0 zsq       (1000) zsq       (1000)        0 2023-05-16 04:37:50.174159 dbpoolpy-0.6.6/src/dbpoolpy/dbhelper/
+-rwxrwxrwx   0 zsq       (1000) zsq       (1000)    23649 2023-05-16 04:36:27.000000 dbpoolpy-0.6.6/src/dbpoolpy/dbhelper/__init__.py
+-rwxrwxrwx   0 zsq       (1000) zsq       (1000)      645 2023-05-16 03:22:18.000000 dbpoolpy-0.6.6/src/dbpoolpy/dbhelper/mysql.py
+-rwxrwxrwx   0 zsq       (1000) zsq       (1000)      976 2023-05-16 03:22:18.000000 dbpoolpy-0.6.6/src/dbpoolpy/dbhelper/postgresql.py
+-rwxrwxrwx   0 zsq       (1000) zsq       (1000)       99 2023-05-16 03:22:18.000000 dbpoolpy-0.6.6/src/dbpoolpy/dbhelper/sqlite3.py
+-rwxrwxrwx   0 zsq       (1000) zsq       (1000)    10097 2023-05-16 03:22:18.000000 dbpoolpy-0.6.6/src/dbpoolpy/dbpool.py
+-rwxrwxrwx   0 zsq       (1000) zsq       (1000)     8097 2023-05-16 04:36:28.000000 dbpoolpy-0.6.6/src/dbpoolpy/table.py
+-rwxrwxrwx   0 zsq       (1000) zsq       (1000)     5108 2023-05-16 03:22:18.000000 dbpoolpy-0.6.6/src/dbpoolpy/utils.py
+drwxrwxrwx   0 zsq       (1000) zsq       (1000)        0 2023-05-16 04:37:49.875158 dbpoolpy-0.6.6/src/dbpoolpy.egg-info/
+-rwxrwxrwx   0 zsq       (1000) zsq       (1000)      397 2023-05-16 04:37:49.000000 dbpoolpy-0.6.6/src/dbpoolpy.egg-info/PKG-INFO
+-rwxrwxrwx   0 zsq       (1000) zsq       (1000)     1059 2023-05-16 04:37:49.000000 dbpoolpy-0.6.6/src/dbpoolpy.egg-info/SOURCES.txt
+-rwxrwxrwx   0 zsq       (1000) zsq       (1000)        1 2023-05-16 04:37:49.000000 dbpoolpy-0.6.6/src/dbpoolpy.egg-info/dependency_links.txt
+-rwxrwxrwx   0 zsq       (1000) zsq       (1000)        9 2023-05-16 04:37:49.000000 dbpoolpy-0.6.6/src/dbpoolpy.egg-info/top_level.txt
+drwxrwxrwx   0 zsq       (1000) zsq       (1000)        0 2023-05-16 04:37:50.234158 dbpoolpy-0.6.6/tests/
+-rwxrwxrwx   0 zsq       (1000) zsq       (1000)     1222 2023-05-16 03:22:19.000000 dbpoolpy-0.6.6/tests/dbhelper_test.py
+-rwxrwxrwx   0 zsq       (1000) zsq       (1000)    10519 2023-05-16 03:22:19.000000 dbpoolpy-0.6.6/tests/mysql_dbpool_test.py
+-rwxrwxrwx   0 zsq       (1000) zsq       (1000)     9262 2023-05-16 03:22:19.000000 dbpoolpy-0.6.6/tests/postgresql_dbpool_test.py
+-rwxrwxrwx   0 zsq       (1000) zsq       (1000)     8639 2023-05-16 03:22:19.000000 dbpoolpy-0.6.6/tests/sqlite_dbpool_test.py
+-rwxrwxrwx   0 zsq       (1000) zsq       (1000)    36864 2023-05-16 03:22:19.000000 dbpoolpy-0.6.6/testsqlite3.db
```

### Comparing `dbpoolpy-0.6.5/LICENSE` & `dbpoolpy-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dbpoolpy-0.6.5/README.md` & `dbpoolpy-0.6.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 ```python
 import pymysql
 from dbpoolpy import init_pool 
 from dbpoolpy import Select, Update, Insert, Delete
 
 DATABASE = {
-    'dbcon1':  {
+    'dbcon1':  {              # 连接池名称
         'engine': pymysql,    # 取数据库所使用的插件：mysql使用pymysql, SQLite3使用python自带的sqlite3, PostgreSQL使用psycopg2
         'database': 'imlf',   # 默认连接的数据库
         'host': '',           # 数据库地址
         'port': 51000,        # 数据库端口
         'user': 'atpdev',     # 数据库用户名
         'password': '',       # 数据库的密码
         'charset': 'utf8',    # 字符集类型
```

### Comparing `dbpoolpy-0.6.5/setup.cfg` & `dbpoolpy-0.6.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `dbpoolpy-0.6.5/src/dbpoolpy/config/__init__.py` & `dbpoolpy-0.6.6/src/dbpoolpy/config/__init__.py`

 * *Files identical despite different names*

### Comparing `dbpoolpy-0.6.5/src/dbpoolpy/config/functional.py` & `dbpoolpy-0.6.6/src/dbpoolpy/config/functional.py`

 * *Files identical despite different names*

### Comparing `dbpoolpy-0.6.5/src/dbpoolpy/constants.py` & `dbpoolpy-0.6.6/src/dbpoolpy/constants.py`

 * *Files identical despite different names*

### Comparing `dbpoolpy-0.6.5/src/dbpoolpy/dbconnect/__init__.py` & `dbpoolpy-0.6.6/src/dbpoolpy/dbconnect/__init__.py`

 * *Files identical despite different names*

### Comparing `dbpoolpy-0.6.5/src/dbpoolpy/dbconnect/mysql.py` & `dbpoolpy-0.6.6/src/dbpoolpy/dbconnect/mysql.py`

 * *Files identical despite different names*

### Comparing `dbpoolpy-0.6.5/src/dbpoolpy/dbconnect/postgresql.py` & `dbpoolpy-0.6.6/src/dbpoolpy/dbconnect/postgresql.py`

 * *Files identical despite different names*

### Comparing `dbpoolpy-0.6.5/src/dbpoolpy/dbconnect/simple.py` & `dbpoolpy-0.6.6/src/dbpoolpy/dbconnect/simple.py`

 * *Files identical despite different names*

### Comparing `dbpoolpy-0.6.5/src/dbpoolpy/dbhelper/__init__.py` & `dbpoolpy-0.6.6/src/dbpoolpy/dbhelper/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -297,15 +297,20 @@
         assert page > 0 and isinstance(page, int)
         assert size > 0 and isinstance(size, int)
         sql = self.sql(fill_args=False)
         assert sql.find('limit') == -1, ValueError("page不能自定义limit")
 
         # 生成sql
         count_sql = self._count_sql(sql)
-        sql += ' limit %s,%s' % ((page - 1) * size, size)
+        count_sql = count_sql.split("ORDER")[0]
+        count_sql = count_sql.split("order")[0]
+        if self._dbo.__dbtype__ == DBTYPE.POSTGRESQL:
+            sql += ' limit %s offset %s' % (size, (page - 1) * size)
+        else:
+            sql += ' limit %s,%s' % ((page - 1) * size, size)
 
         # 获取数据
         count_data = self._dbo.get(count_sql, self._where_args or None, isdict=True)
         page_data = self._dbo.query(sql, self._where_args or None, isdict=isdict)
         pages = ceil(count_data["total"] / size)
 
         return Page(
```

### Comparing `dbpoolpy-0.6.5/src/dbpoolpy/dbhelper/mysql.py` & `dbpoolpy-0.6.6/src/dbpoolpy/dbhelper/mysql.py`

 * *Files identical despite different names*

### Comparing `dbpoolpy-0.6.5/src/dbpoolpy/dbhelper/postgresql.py` & `dbpoolpy-0.6.6/src/dbpoolpy/dbhelper/postgresql.py`

 * *Files identical despite different names*

### Comparing `dbpoolpy-0.6.5/src/dbpoolpy/dbpool.py` & `dbpoolpy-0.6.6/src/dbpoolpy/dbpool.py`

 * *Files identical despite different names*

### Comparing `dbpoolpy-0.6.5/src/dbpoolpy/table.py` & `dbpoolpy-0.6.6/src/dbpoolpy/table.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from math import ceil
 from collections import namedtuple
+from dbpoolpy.constants import DBTYPE
 from dbpoolpy.dbpool import acquire, release
 from dbpoolpy.dbhelper import SelectHelper, InsertHelper, UpdateHelper, DeleteHelper
 
 Page = namedtuple("Page", ["total", "pages", "page", "size", "data"])
 
 def with_dbo(func):
     def _(self, *args, **kwargs):
@@ -81,15 +82,20 @@
         assert page > 0 and isinstance(page, int)
         assert size > 0 and isinstance(size, int)
         sql = self.sql(is_auto_close=False, fill_args=False)
         assert sql.find('limit') == -1, ValueError("page不能自定义limit")
 
         # 生成sql
         count_sql = self._count_sql(sql)
-        sql += ' limit %s,%s' % ((page - 1) * size, size)
+        count_sql = count_sql.split("ORDER")[0]
+        count_sql = count_sql.split("order")[0]
+        if self._dbo.__dbtype__ == DBTYPE.POSTGRESQL:
+            sql += ' limit %s offset %s' % (size, (page - 1) * size)
+        else:
+            sql += ' limit %s,%s' % ((page - 1) * size, size)
 
         # 获取数据
         count_data = self._dbo.get(count_sql, self._where_args or None, isdict=True)
         page_data = self._dbo.query(sql, self._where_args or None, isdict=isdict)
         pages = ceil(count_data["total"] / size)
 
         return Page(
```

### Comparing `dbpoolpy-0.6.5/src/dbpoolpy/utils.py` & `dbpoolpy-0.6.6/src/dbpoolpy/utils.py`

 * *Files identical despite different names*

### Comparing `dbpoolpy-0.6.5/src/dbpoolpy.egg-info/SOURCES.txt` & `dbpoolpy-0.6.6/src/dbpoolpy.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,21 @@
+.gitignore
+CHANGES.rst
 LICENSE
+README.en.md
 README.md
 pyproject.toml
+requestments.txt
 setup.cfg
 setup.py
+testsqlite3.db
+.gitee/ISSUE_TEMPLATE.zh-CN.md
+.gitee/PULL_REQUEST_TEMPLATE.zh-CN.md
+example/db/__init__.py
+script/postgresql_test.py
 src/dbpoolpy/__init__.py
 src/dbpoolpy/constants.py
 src/dbpoolpy/dbpool.py
 src/dbpoolpy/table.py
 src/dbpoolpy/utils.py
 src/dbpoolpy.egg-info/PKG-INFO
 src/dbpoolpy.egg-info/SOURCES.txt
@@ -20,8 +29,12 @@
 src/dbpoolpy/dbconnect/mysql.py
 src/dbpoolpy/dbconnect/postgresql.py
 src/dbpoolpy/dbconnect/simple.py
 src/dbpoolpy/dbconnect/sqlite3.py
 src/dbpoolpy/dbhelper/__init__.py
 src/dbpoolpy/dbhelper/mysql.py
 src/dbpoolpy/dbhelper/postgresql.py
-src/dbpoolpy/dbhelper/sqlite3.py
+src/dbpoolpy/dbhelper/sqlite3.py
+tests/dbhelper_test.py
+tests/mysql_dbpool_test.py
+tests/postgresql_dbpool_test.py
+tests/sqlite_dbpool_test.py
```

