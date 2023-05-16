# Comparing `tmp/udata_search_service-2.0.1.dev246.tar.gz` & `tmp/udata_search_service-2.0.2.dev250.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "udata_search_service-2.0.1.dev246.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "udata_search_service-2.0.2.dev250.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `udata_search_service-2.0.1.dev246.tar` & `udata_search_service-2.0.2.dev250.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     2409 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/.circleci/config.yml
--rw-r--r--   0        0        0      763 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/.gitignore
--rw-r--r--   0        0        0     1708 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/CHANGELOG.md
--rw-r--r--   0        0        0      173 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/Dockerfiles/Dockerfile.app
--rw-r--r--   0        0        0      494 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/Makefile
--rw-r--r--   0        0        0     3776 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/README.md
--rw-r--r--   0        0        0      394 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/bumpr.rc
--rw-r--r--   0        0        0      329 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/docker-compose.test.yml
--rw-r--r--   0        0        0      560 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/docker-compose.yml
--rw-r--r--   0        0        0    18532 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/docs/udata-search-service-schema.png
--rw-r--r--   0        0        0      831 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/tests/__init__.py
--rw-r--r--   0        0        0      769 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/tests/conftest.py
--rw-r--r--   0        0        0    27878 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/tests/test_api.py
--rw-r--r--   0        0        0     6164 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/tests/test_consumers.py
--rw-r--r--   0        0        0    13254 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/tests/test_search_client.py
--rw-r--r--   0        0        0      202 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/udata_search_service/__init__.py
--rw-r--r--   0        0        0      807 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/udata_search_service/app.py
--rw-r--r--   0        0        0      703 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/udata_search_service/config.py
--rw-r--r--   0        0        0      767 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/udata_search_service/container.py
--rw-r--r--   0        0        0        0 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/udata_search_service/domain/__init__.py
--rw-r--r--   0        0        0     2666 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/udata_search_service/domain/entities.py
--rw-r--r--   0        0        0     2513 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/udata_search_service/domain/factories.py
--rw-r--r--   0        0        0     1343 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/udata_search_service/domain/interfaces.py
--rw-r--r--   0        0        0        0 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/udata_search_service/infrastructure/__init__.py
--rw-r--r--   0        0        0     2641 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/udata_search_service/infrastructure/consumers.py
--rw-r--r--   0        0        0     2063 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/udata_search_service/infrastructure/migrate.py
--rw-r--r--   0        0        0    15956 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/udata_search_service/infrastructure/search_clients.py
--rw-r--r--   0        0        0     5699 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/udata_search_service/infrastructure/services.py
--rw-r--r--   0        0        0     1402 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/udata_search_service/infrastructure/utils.py
--rw-r--r--   0        0        0        0 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/udata_search_service/presentation/__init__.py
--rw-r--r--   0        0        0    14252 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/udata_search_service/presentation/api.py
--rw-r--r--   0        0        0      952 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/udata_search_service/presentation/commands.py
--rw-r--r--   0        0        0       76 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/udata_search_service/wsgi.py
--rw-r--r--   0        0        0     4510 1970-01-01 00:00:00.000000 udata_search_service-2.0.1.dev246/PKG-INFO
+-rw-r--r--   0        0        0     2409 2023-05-16 12:53:52.000000 udata_search_service-2.0.2.dev250/.circleci/config.yml
+-rw-r--r--   0        0        0      763 2023-05-16 12:53:52.000000 udata_search_service-2.0.2.dev250/.gitignore
+-rw-r--r--   0        0        0     1746 2023-05-16 12:53:52.000000 udata_search_service-2.0.2.dev250/CHANGELOG.md
+-rw-r--r--   0        0        0      173 2023-05-16 12:53:52.000000 udata_search_service-2.0.2.dev250/Dockerfiles/Dockerfile.app
+-rw-r--r--   0        0        0      494 2023-05-16 12:53:52.000000 udata_search_service-2.0.2.dev250/Makefile
+-rw-r--r--   0        0        0     3776 2023-05-16 12:53:52.000000 udata_search_service-2.0.2.dev250/README.md
+-rw-r--r--   0        0        0      394 2023-05-16 12:53:52.000000 udata_search_service-2.0.2.dev250/bumpr.rc
+-rw-r--r--   0        0        0      329 2023-05-16 12:53:52.000000 udata_search_service-2.0.2.dev250/docker-compose.test.yml
+-rw-r--r--   0        0        0      560 2023-05-16 12:53:52.000000 udata_search_service-2.0.2.dev250/docker-compose.yml
+-rw-r--r--   0        0        0    18532 2023-05-16 12:53:52.000000 udata_search_service-2.0.2.dev250/docs/udata-search-service-schema.png
+-rw-r--r--   0        0        0      831 2023-05-16 12:53:52.000000 udata_search_service-2.0.2.dev250/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-16 12:53:52.000000 udata_search_service-2.0.2.dev250/tests/__init__.py
+-rw-r--r--   0        0        0      769 2023-05-16 12:53:52.000000 udata_search_service-2.0.2.dev250/tests/conftest.py
+-rw-r--r--   0        0        0    27878 2023-05-16 12:53:52.000000 udata_search_service-2.0.2.dev250/tests/test_api.py
+-rw-r--r--   0        0        0     6164 2023-05-16 12:53:52.000000 udata_search_service-2.0.2.dev250/tests/test_consumers.py
+-rw-r--r--   0        0        0    13254 2023-05-16 12:53:52.000000 udata_search_service-2.0.2.dev250/tests/test_search_client.py
+-rw-r--r--   0        0        0      202 2023-05-16 12:53:52.000000 udata_search_service-2.0.2.dev250/udata_search_service/__init__.py
+-rw-r--r--   0        0        0      807 2023-05-16 12:53:52.000000 udata_search_service-2.0.2.dev250/udata_search_service/app.py
+-rw-r--r--   0        0        0      703 2023-05-16 12:53:52.000000 udata_search_service-2.0.2.dev250/udata_search_service/config.py
+-rw-r--r--   0        0        0      767 2023-05-16 12:53:52.000000 udata_search_service-2.0.2.dev250/udata_search_service/container.py
+-rw-r--r--   0        0        0        0 2023-05-16 12:53:52.000000 udata_search_service-2.0.2.dev250/udata_search_service/domain/__init__.py
+-rw-r--r--   0        0        0     2666 2023-05-16 12:53:52.000000 udata_search_service-2.0.2.dev250/udata_search_service/domain/entities.py
+-rw-r--r--   0        0        0     2513 2023-05-16 12:53:52.000000 udata_search_service-2.0.2.dev250/udata_search_service/domain/factories.py
+-rw-r--r--   0        0        0     1343 2023-05-16 12:53:52.000000 udata_search_service-2.0.2.dev250/udata_search_service/domain/interfaces.py
+-rw-r--r--   0        0        0        0 2023-05-16 12:53:52.000000 udata_search_service-2.0.2.dev250/udata_search_service/infrastructure/__init__.py
+-rw-r--r--   0        0        0     2641 2023-05-16 12:53:52.000000 udata_search_service-2.0.2.dev250/udata_search_service/infrastructure/consumers.py
+-rw-r--r--   0        0        0     2063 2023-05-16 12:53:52.000000 udata_search_service-2.0.2.dev250/udata_search_service/infrastructure/migrate.py
+-rw-r--r--   0        0        0    15956 2023-05-16 12:53:52.000000 udata_search_service-2.0.2.dev250/udata_search_service/infrastructure/search_clients.py
+-rw-r--r--   0        0        0     5699 2023-05-16 12:53:52.000000 udata_search_service-2.0.2.dev250/udata_search_service/infrastructure/services.py
+-rw-r--r--   0        0        0     1402 2023-05-16 12:53:52.000000 udata_search_service-2.0.2.dev250/udata_search_service/infrastructure/utils.py
+-rw-r--r--   0        0        0        0 2023-05-16 12:53:52.000000 udata_search_service-2.0.2.dev250/udata_search_service/presentation/__init__.py
+-rw-r--r--   0        0        0    14252 2023-05-16 12:53:52.000000 udata_search_service-2.0.2.dev250/udata_search_service/presentation/api.py
+-rw-r--r--   0        0        0      952 2023-05-16 12:53:52.000000 udata_search_service-2.0.2.dev250/udata_search_service/presentation/commands.py
+-rw-r--r--   0        0        0       76 2023-05-16 12:53:52.000000 udata_search_service-2.0.2.dev250/udata_search_service/wsgi.py
+-rw-r--r--   0        0        0     4510 1970-01-01 00:00:00.000000 udata_search_service-2.0.2.dev250/PKG-INFO
```

### Comparing `udata_search_service-2.0.1.dev246/.circleci/config.yml` & `udata_search_service-2.0.2.dev250/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `udata_search_service-2.0.1.dev246/.gitignore` & `udata_search_service-2.0.2.dev250/.gitignore`

 * *Files identical despite different names*

### Comparing `udata_search_service-2.0.1.dev246/CHANGELOG.md` & `udata_search_service-2.0.2.dev250/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 ## Current (in progress)
 
+- Nothing yet
+
+## 2.0.1 (2023-05-16)
+
 - Add `last_update` field to dataset entity. All datasets need to be reindexed to take last_update into account [#40](https://github.com/opendatateam/udata-search-service/pull/40)
 - Use `datetime.utcnow` to make sure to handle utc datetimes [#42](https://github.com/opendatateam/udata-search-service/pull/42)
 
 ## 2.0.0 (2023-01-09)
 
 - Use redpanda instead of Kafka [#34](https://github.com/opendatateam/udata-search-service/pull/34)
 - Remove Kafka integration and use HTTP calls instead [#35](https://github.com/opendatateam/udata-search-service/pull/35)
```

### Comparing `udata_search_service-2.0.1.dev246/README.md` & `udata_search_service-2.0.2.dev250/README.md`

 * *Files identical despite different names*

### Comparing `udata_search_service-2.0.1.dev246/docker-compose.yml` & `udata_search_service-2.0.2.dev250/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `udata_search_service-2.0.1.dev246/docs/udata-search-service-schema.png` & `udata_search_service-2.0.2.dev250/docs/udata-search-service-schema.png`

 * *Files identical despite different names*

### Comparing `udata_search_service-2.0.1.dev246/pyproject.toml` & `udata_search_service-2.0.2.dev250/pyproject.toml`

 * *Files identical despite different names*

### Comparing `udata_search_service-2.0.1.dev246/tests/conftest.py` & `udata_search_service-2.0.2.dev250/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `udata_search_service-2.0.1.dev246/tests/test_api.py` & `udata_search_service-2.0.2.dev250/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `udata_search_service-2.0.1.dev246/tests/test_consumers.py` & `udata_search_service-2.0.2.dev250/tests/test_consumers.py`

 * *Files identical despite different names*

### Comparing `udata_search_service-2.0.1.dev246/tests/test_search_client.py` & `udata_search_service-2.0.2.dev250/tests/test_search_client.py`

 * *Files identical despite different names*

### Comparing `udata_search_service-2.0.1.dev246/udata_search_service/app.py` & `udata_search_service-2.0.2.dev250/udata_search_service/app.py`

 * *Files identical despite different names*

### Comparing `udata_search_service-2.0.1.dev246/udata_search_service/config.py` & `udata_search_service-2.0.2.dev250/udata_search_service/config.py`

 * *Files identical despite different names*

### Comparing `udata_search_service-2.0.1.dev246/udata_search_service/container.py` & `udata_search_service-2.0.2.dev250/udata_search_service/container.py`

 * *Files identical despite different names*

### Comparing `udata_search_service-2.0.1.dev246/udata_search_service/domain/entities.py` & `udata_search_service-2.0.2.dev250/udata_search_service/domain/entities.py`

 * *Files identical despite different names*

### Comparing `udata_search_service-2.0.1.dev246/udata_search_service/domain/factories.py` & `udata_search_service-2.0.2.dev250/udata_search_service/domain/factories.py`

 * *Files identical despite different names*

### Comparing `udata_search_service-2.0.1.dev246/udata_search_service/domain/interfaces.py` & `udata_search_service-2.0.2.dev250/udata_search_service/domain/interfaces.py`

 * *Files identical despite different names*

### Comparing `udata_search_service-2.0.1.dev246/udata_search_service/infrastructure/consumers.py` & `udata_search_service-2.0.2.dev250/udata_search_service/infrastructure/consumers.py`

 * *Files identical despite different names*

### Comparing `udata_search_service-2.0.1.dev246/udata_search_service/infrastructure/migrate.py` & `udata_search_service-2.0.2.dev250/udata_search_service/infrastructure/migrate.py`

 * *Files identical despite different names*

### Comparing `udata_search_service-2.0.1.dev246/udata_search_service/infrastructure/search_clients.py` & `udata_search_service-2.0.2.dev250/udata_search_service/infrastructure/search_clients.py`

 * *Files identical despite different names*

### Comparing `udata_search_service-2.0.1.dev246/udata_search_service/infrastructure/services.py` & `udata_search_service-2.0.2.dev250/udata_search_service/infrastructure/services.py`

 * *Files identical despite different names*

### Comparing `udata_search_service-2.0.1.dev246/udata_search_service/infrastructure/utils.py` & `udata_search_service-2.0.2.dev250/udata_search_service/infrastructure/utils.py`

 * *Files identical despite different names*

### Comparing `udata_search_service-2.0.1.dev246/udata_search_service/presentation/api.py` & `udata_search_service-2.0.2.dev250/udata_search_service/presentation/api.py`

 * *Files identical despite different names*

### Comparing `udata_search_service-2.0.1.dev246/udata_search_service/presentation/commands.py` & `udata_search_service-2.0.2.dev250/udata_search_service/presentation/commands.py`

 * *Files identical despite different names*

### Comparing `udata_search_service-2.0.1.dev246/PKG-INFO` & `udata_search_service-2.0.2.dev250/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: udata-search-service
-Version: 2.0.1.dev246
+Version: 2.0.2.dev250
 Summary: udata search service
 Author-email: Opendata Team <opendatateam@data.gouv.fr>
 Description-Content-Type: text/markdown
 Requires-Dist: dependency-injector==4.36.0
 Requires-Dist: elasticsearch==7.15.0
 Requires-Dist: elasticsearch_dsl==7.4.0
 Requires-Dist: factory-boy==3.2.1
```

