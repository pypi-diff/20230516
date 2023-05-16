# Comparing `tmp/udata-search-service-2.0.1.dev241.tar.gz` & `tmp/udata_search_service-2.0.1.dev246.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "udata-search-service-2.0.1.dev241.tar", last modified: Thu May  4 12:12:59 2023, max compression
+gzip compressed data, was "udata_search_service-2.0.1.dev246.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `udata-search-service-2.0.1.dev241.tar` & `udata_search_service-2.0.1.dev246.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     2409 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/.circleci/config.yml
--rw-r--r--   0        0        0      763 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/.gitignore
--rw-r--r--   0        0        0     1579 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/CHANGELOG.md
--rw-r--r--   0        0        0      173 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/Dockerfiles/Dockerfile.app
--rw-r--r--   0        0        0      494 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/Makefile
--rw-r--r--   0        0        0     3776 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/README.md
--rw-r--r--   0        0        0      394 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/bumpr.rc
--rw-r--r--   0        0        0      329 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/docker-compose.test.yml
--rw-r--r--   0        0        0      560 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/docker-compose.yml
--rw-r--r--   0        0        0    18532 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/docs/udata-search-service-schema.png
--rw-r--r--   0        0        0      831 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/tests/__init__.py
--rw-r--r--   0        0        0      769 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/tests/conftest.py
--rw-r--r--   0        0        0    27860 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/tests/test_api.py
--rw-r--r--   0        0        0     6164 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/tests/test_consumers.py
--rw-r--r--   0        0        0    13254 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/tests/test_search_client.py
--rw-r--r--   0        0        0      202 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/udata_search_service/__init__.py
--rw-r--r--   0        0        0      807 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/udata_search_service/app.py
--rw-r--r--   0        0        0      703 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/udata_search_service/config.py
--rw-r--r--   0        0        0      767 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/udata_search_service/container.py
--rw-r--r--   0        0        0        0 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/udata_search_service/domain/__init__.py
--rw-r--r--   0        0        0     2666 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/udata_search_service/domain/entities.py
--rw-r--r--   0        0        0     2501 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/udata_search_service/domain/factories.py
--rw-r--r--   0        0        0     1343 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/udata_search_service/domain/interfaces.py
--rw-r--r--   0        0        0        0 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/udata_search_service/infrastructure/__init__.py
--rw-r--r--   0        0        0     2641 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/udata_search_service/infrastructure/consumers.py
--rw-r--r--   0        0        0     2063 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/udata_search_service/infrastructure/migrate.py
--rw-r--r--   0        0        0    15953 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/udata_search_service/infrastructure/search_clients.py
--rw-r--r--   0        0        0     5699 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/udata_search_service/infrastructure/services.py
--rw-r--r--   0        0        0     1402 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/udata_search_service/infrastructure/utils.py
--rw-r--r--   0        0        0        0 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/udata_search_service/presentation/__init__.py
--rw-r--r--   0        0        0    14252 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/udata_search_service/presentation/api.py
--rw-r--r--   0        0        0      952 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/udata_search_service/presentation/commands.py
--rw-r--r--   0        0        0       76 2023-05-04 12:09:11.000000 udata-search-service-2.0.1.dev241/udata_search_service/wsgi.py
--rw-r--r--   0        0        0     4510 1970-01-01 00:00:00.000000 udata-search-service-2.0.1.dev241/PKG-INFO
+-rw-r--r--   0        0        0     2409 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/.circleci/config.yml
+-rw-r--r--   0        0        0      763 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/.gitignore
+-rw-r--r--   0        0        0     1708 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/CHANGELOG.md
+-rw-r--r--   0        0        0      173 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/Dockerfiles/Dockerfile.app
+-rw-r--r--   0        0        0      494 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/Makefile
+-rw-r--r--   0        0        0     3776 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/README.md
+-rw-r--r--   0        0        0      394 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/bumpr.rc
+-rw-r--r--   0        0        0      329 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/docker-compose.test.yml
+-rw-r--r--   0        0        0      560 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/docker-compose.yml
+-rw-r--r--   0        0        0    18532 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/docs/udata-search-service-schema.png
+-rw-r--r--   0        0        0      831 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/tests/__init__.py
+-rw-r--r--   0        0        0      769 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/tests/conftest.py
+-rw-r--r--   0        0        0    27878 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/tests/test_api.py
+-rw-r--r--   0        0        0     6164 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/tests/test_consumers.py
+-rw-r--r--   0        0        0    13254 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/tests/test_search_client.py
+-rw-r--r--   0        0        0      202 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/udata_search_service/__init__.py
+-rw-r--r--   0        0        0      807 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/udata_search_service/app.py
+-rw-r--r--   0        0        0      703 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/udata_search_service/config.py
+-rw-r--r--   0        0        0      767 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/udata_search_service/container.py
+-rw-r--r--   0        0        0        0 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/udata_search_service/domain/__init__.py
+-rw-r--r--   0        0        0     2666 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/udata_search_service/domain/entities.py
+-rw-r--r--   0        0        0     2513 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/udata_search_service/domain/factories.py
+-rw-r--r--   0        0        0     1343 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/udata_search_service/domain/interfaces.py
+-rw-r--r--   0        0        0        0 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/udata_search_service/infrastructure/__init__.py
+-rw-r--r--   0        0        0     2641 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/udata_search_service/infrastructure/consumers.py
+-rw-r--r--   0        0        0     2063 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/udata_search_service/infrastructure/migrate.py
+-rw-r--r--   0        0        0    15956 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/udata_search_service/infrastructure/search_clients.py
+-rw-r--r--   0        0        0     5699 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/udata_search_service/infrastructure/services.py
+-rw-r--r--   0        0        0     1402 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/udata_search_service/infrastructure/utils.py
+-rw-r--r--   0        0        0        0 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/udata_search_service/presentation/__init__.py
+-rw-r--r--   0        0        0    14252 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/udata_search_service/presentation/api.py
+-rw-r--r--   0        0        0      952 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/udata_search_service/presentation/commands.py
+-rw-r--r--   0        0        0       76 2023-05-16 07:52:51.000000 udata_search_service-2.0.1.dev246/udata_search_service/wsgi.py
+-rw-r--r--   0        0        0     4510 1970-01-01 00:00:00.000000 udata_search_service-2.0.1.dev246/PKG-INFO
```

### Comparing `udata-search-service-2.0.1.dev241/.circleci/config.yml` & `udata_search_service-2.0.1.dev246/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `udata-search-service-2.0.1.dev241/.gitignore` & `udata_search_service-2.0.1.dev246/.gitignore`

 * *Files identical despite different names*

### Comparing `udata-search-service-2.0.1.dev241/CHANGELOG.md` & `udata_search_service-2.0.1.dev246/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 
 ## Current (in progress)
 
 - Add `last_update` field to dataset entity. All datasets need to be reindexed to take last_update into account [#40](https://github.com/opendatateam/udata-search-service/pull/40)
+- Use `datetime.utcnow` to make sure to handle utc datetimes [#42](https://github.com/opendatateam/udata-search-service/pull/42)
 
 ## 2.0.0 (2023-01-09)
 
 - Use redpanda instead of Kafka [#34](https://github.com/opendatateam/udata-search-service/pull/34)
 - Remove Kafka integration and use HTTP calls instead [#35](https://github.com/opendatateam/udata-search-service/pull/35)
 
 ## 1.0.3 (2022-07-11)
```

### Comparing `udata-search-service-2.0.1.dev241/README.md` & `udata_search_service-2.0.1.dev246/README.md`

 * *Files identical despite different names*

### Comparing `udata-search-service-2.0.1.dev241/docker-compose.yml` & `udata_search_service-2.0.1.dev246/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `udata-search-service-2.0.1.dev241/docs/udata-search-service-schema.png` & `udata_search_service-2.0.1.dev246/docs/udata-search-service-schema.png`

 * *Files identical despite different names*

### Comparing `udata-search-service-2.0.1.dev241/pyproject.toml` & `udata_search_service-2.0.1.dev246/pyproject.toml`

 * *Files identical despite different names*

### Comparing `udata-search-service-2.0.1.dev241/tests/conftest.py` & `udata_search_service-2.0.1.dev246/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `udata-search-service-2.0.1.dev241/tests/test_api.py` & `udata_search_service-2.0.1.dev246/tests/test_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     assert dataset_search_after_delete_resp.json['previous_page'] is None
     assert dataset_search_after_delete_resp.json['page_size'] == 20
     assert dataset_search_after_delete_resp.json['total_pages'] == 1
     assert dataset_search_after_delete_resp.json['total'] == 0
 
 
 def test_api_dataset_index_on_another_index(app, client, search_client, faker):
-    now = datetime.datetime.now().strftime('%Y-%m-%d-%H-%M')
+    now = datetime.datetime.utcnow().strftime('%Y-%m-%d-%H-%M')
     index_name = f"test-dataset-{now}"
     if not search_client.es.indices.exists(index=f"{app.config['UDATA_INSTANCE_NAME']}-{index_name}"):
         search_client.es.indices.create(index=f"{app.config['UDATA_INSTANCE_NAME']}-{index_name}")
 
     dataset = {
         'id': faker.md5(),
         'title': faker.sentence(),
@@ -197,15 +197,15 @@
     assert organization_search_after_delete_resp.json['previous_page'] is None
     assert organization_search_after_delete_resp.json['page_size'] == 20
     assert organization_search_after_delete_resp.json['total_pages'] == 1
     assert organization_search_after_delete_resp.json['total'] == 0
 
 
 def test_api_org_index_on_another_index(app, client, search_client, faker):
-    now = datetime.datetime.now().strftime('%Y-%m-%d-%H-%M')
+    now = datetime.datetime.utcnow().strftime('%Y-%m-%d-%H-%M')
     index_name = f"test-organization-{now}"
     if not search_client.es.indices.exists(index=f"{app.config['UDATA_INSTANCE_NAME']}-{index_name}"):
         search_client.es.indices.create(index=f"{app.config['UDATA_INSTANCE_NAME']}-{index_name}")
 
     org = {
         'id': faker.md5(),
         'name': faker.company(),
@@ -301,15 +301,15 @@
     assert reuse_search_after_delete_resp.json['previous_page'] is None
     assert reuse_search_after_delete_resp.json['page_size'] == 20
     assert reuse_search_after_delete_resp.json['total_pages'] == 1
     assert reuse_search_after_delete_resp.json['total'] == 0
 
 
 def test_api_reuse_index_on_another_index(app, client, search_client, faker):
-    now = datetime.datetime.now().strftime('%Y-%m-%d-%H-%M')
+    now = datetime.datetime.utcnow().strftime('%Y-%m-%d-%H-%M')
     index_name = f"test-reuse-{now}"
     if not search_client.es.indices.exists(index=f"{app.config['UDATA_INSTANCE_NAME']}-{index_name}"):
         search_client.es.indices.create(index=f"{app.config['UDATA_INSTANCE_NAME']}-{index_name}")
 
     reuse = {
         'id': faker.md5(),
         'title': faker.sentence(),
@@ -450,28 +450,28 @@
     assert '/api/1/reuses/?page=1&page_size=2' in reuse_resp.json['previous_page']
     assert reuse_resp.json['page_size'] == 2
     assert reuse_resp.json['total_pages'] == 2
     assert reuse_resp.json['total'] == 4
 
 
 def test_api_create_index(app, client, search_client, faker):
-    now = datetime.datetime.now().strftime('%Y-%m-%d-%H-%M')
+    now = datetime.datetime.utcnow().strftime('%Y-%m-%d-%H-%M')
     index_name = f"test-dataset-{now}"
 
     payload = {
         'index': index_name
     }
     set_alias_resp = client.post(url_for('api.create_index'), json=payload)
     assert set_alias_resp.status_code == 200
 
     assert search_client.es.indices.exists(index=f"{app.config['UDATA_INSTANCE_NAME']}-{index_name}")
 
 
 def test_api_set_index_alias(app, client, search_client, faker):
-    now = datetime.datetime.now().strftime('%Y-%m-%d-%H-%M')
+    now = datetime.datetime.utcnow().strftime('%Y-%m-%d-%H-%M')
     index_name = f"{app.config['UDATA_INSTANCE_NAME']}-dataset-{now}"
 
     if not search_client.es.indices.exists(index=index_name):
         search_client.es.indices.create(index=index_name)
 
     payload = {
         'index_suffix_name': now,
@@ -484,15 +484,15 @@
 
     assert search_client.es.indices.exists_alias(name=index_alias)
     alias_keys = list(search_client.es.indices.get_alias(name=index_alias))
 
     assert alias_keys[0] == index_name
 
 
-    now = datetime.datetime.now().strftime('%Y-%m-%d-%H-%M')
+    now = datetime.datetime.utcnow().strftime('%Y-%m-%d-%H-%M')
 
     for index in ['dataset', 'reuse', 'organization']:
         index_name = f"{app.config['UDATA_INSTANCE_NAME']}-{index}-{now}"
         if not search_client.es.indices.exists(index=index_name):
             search_client.es.indices.create(index=index_name)
 
     payload = {
```

### Comparing `udata-search-service-2.0.1.dev241/tests/test_consumers.py` & `udata_search_service-2.0.1.dev246/tests/test_consumers.py`

 * *Files identical despite different names*

### Comparing `udata-search-service-2.0.1.dev241/tests/test_search_client.py` & `udata_search_service-2.0.1.dev246/tests/test_search_client.py`

 * *Files identical despite different names*

### Comparing `udata-search-service-2.0.1.dev241/udata_search_service/app.py` & `udata_search_service-2.0.1.dev246/udata_search_service/app.py`

 * *Files identical despite different names*

### Comparing `udata-search-service-2.0.1.dev241/udata_search_service/config.py` & `udata_search_service-2.0.1.dev246/udata_search_service/config.py`

 * *Files identical despite different names*

### Comparing `udata-search-service-2.0.1.dev241/udata_search_service/container.py` & `udata_search_service-2.0.1.dev246/udata_search_service/container.py`

 * *Files identical despite different names*

### Comparing `udata-search-service-2.0.1.dev241/udata_search_service/domain/entities.py` & `udata_search_service-2.0.1.dev246/udata_search_service/domain/entities.py`

 * *Files identical despite different names*

### Comparing `udata-search-service-2.0.1.dev241/udata_search_service/domain/factories.py` & `udata_search_service-2.0.1.dev246/udata_search_service/domain/factories.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,16 @@
         model = Dataset
 
     id = factory.Faker('md5')
     title = factory.Faker('sentence')
     description = factory.Faker('text')
     acronym = factory.Faker('company_suffix')
     url = factory.Faker('url')
-    created_at = factory.LazyFunction(datetime.datetime.now)
-    last_update = factory.LazyFunction(datetime.datetime.now)
+    created_at = factory.LazyFunction(datetime.datetime.utcnow)
+    last_update = factory.LazyFunction(datetime.datetime.utcnow)
     orga_sp = 4
     orga_followers = factory.Faker('random_int')
     views = factory.Faker('random_int')
     followers = factory.Faker('random_int')
     reuses = factory.Faker('random_int')
     featured = factory.Faker('random_int')
     resources_count = factory.Faker('random_int', min=1, max=15)
@@ -42,30 +42,30 @@
         model = Organization
 
     id = factory.Faker('md5')
     name = factory.Faker('company')
     description = factory.Faker('text')
     url = factory.Faker('url')
     orga_sp = 4
-    created_at = factory.LazyFunction(datetime.datetime.now)
+    created_at = factory.LazyFunction(datetime.datetime.utcnow)
     followers = factory.Faker('random_int')
     datasets = factory.Faker('random_int')
     views = factory.Faker('random_int')
     reuses = factory.Faker('random_int')
 
 
 class ReuseFactory(factory.Factory):
     class Meta:
         model = Reuse
 
     id = factory.Faker('md5')
     title = factory.Faker('sentence')
     description = factory.Faker('text')
     url = factory.Faker('url')
-    created_at = factory.LazyFunction(datetime.datetime.now)
+    created_at = factory.LazyFunction(datetime.datetime.utcnow)
     orga_followers = factory.Faker('random_int')
     views = factory.Faker('random_int')
     followers = factory.Faker('random_int')
     datasets = factory.Faker('random_int')
     featured = factory.Faker('random_int')
     organization = factory.Faker('md5')
     organization_name = factory.Faker('company')
```

### Comparing `udata-search-service-2.0.1.dev241/udata_search_service/domain/interfaces.py` & `udata_search_service-2.0.1.dev246/udata_search_service/domain/interfaces.py`

 * *Files identical despite different names*

### Comparing `udata-search-service-2.0.1.dev241/udata_search_service/infrastructure/consumers.py` & `udata_search_service-2.0.1.dev246/udata_search_service/infrastructure/consumers.py`

 * *Files identical despite different names*

### Comparing `udata-search-service-2.0.1.dev241/udata_search_service/infrastructure/migrate.py` & `udata_search_service-2.0.1.dev246/udata_search_service/infrastructure/migrate.py`

 * *Files identical despite different names*

### Comparing `udata-search-service-2.0.1.dev241/udata_search_service/infrastructure/search_clients.py` & `udata_search_service-2.0.1.dev246/udata_search_service/infrastructure/search_clients.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
         self.es = connections.create_connection(hosts=[url])
 
     def init_indices(self) -> None:
         '''
         Create templates based on Document mappings and map patterns.
         Create time-based index matchin the template patterns.
         '''
-        suffix_name = '-' + datetime.now().strftime('%Y-%m-%d-%H-%M')
+        suffix_name = '-' + datetime.utcnow().strftime('%Y-%m-%d-%H-%M')
 
         SearchableDataset.init_index(self.es, suffix_name)
         SearchableReuse.init_index(self.es, suffix_name)
         SearchableOrganization.init_index(self.es, suffix_name)
 
     def clean_indices(self) -> None:
         '''
```

### Comparing `udata-search-service-2.0.1.dev241/udata_search_service/infrastructure/services.py` & `udata_search_service-2.0.1.dev246/udata_search_service/infrastructure/services.py`

 * *Files identical despite different names*

### Comparing `udata-search-service-2.0.1.dev241/udata_search_service/infrastructure/utils.py` & `udata_search_service-2.0.1.dev246/udata_search_service/infrastructure/utils.py`

 * *Files identical despite different names*

### Comparing `udata-search-service-2.0.1.dev241/udata_search_service/presentation/api.py` & `udata_search_service-2.0.1.dev246/udata_search_service/presentation/api.py`

 * *Files identical despite different names*

### Comparing `udata-search-service-2.0.1.dev241/udata_search_service/presentation/commands.py` & `udata_search_service-2.0.1.dev246/udata_search_service/presentation/commands.py`

 * *Files identical despite different names*

### Comparing `udata-search-service-2.0.1.dev241/PKG-INFO` & `udata_search_service-2.0.1.dev246/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: udata-search-service
-Version: 2.0.1.dev241
+Version: 2.0.1.dev246
 Summary: udata search service
 Author-email: Opendata Team <opendatateam@data.gouv.fr>
 Description-Content-Type: text/markdown
 Requires-Dist: dependency-injector==4.36.0
 Requires-Dist: elasticsearch==7.15.0
 Requires-Dist: elasticsearch_dsl==7.4.0
 Requires-Dist: factory-boy==3.2.1
```

