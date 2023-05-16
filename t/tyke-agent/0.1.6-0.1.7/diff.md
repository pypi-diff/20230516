# Comparing `tmp/tyke-agent-0.1.6.tar.gz` & `tmp/tyke-agent-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tyke-agent-0.1.6.tar", last modified: Fri Dec  9 10:53:36 2022, max compression
+gzip compressed data, was "tyke-agent-0.1.7.tar", last modified: Tue May 16 04:36:37 2023, max compression
```

## Comparing `tyke-agent-0.1.6.tar` & `tyke-agent-0.1.7.tar`

### file list

```diff
@@ -1,65 +1,99 @@
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2022-12-09 10:53:36.560960 tyke-agent-0.1.6/
--rw-rw-r--   0 bhaskar    (501) staff       (20)    11357 2022-08-25 14:02:53.000000 tyke-agent-0.1.6/LICENSE
--rw-r--r--   0 bhaskar    (501) staff       (20)     2856 2022-12-09 10:53:36.560797 tyke-agent-0.1.6/PKG-INFO
--rw-rw-r--   0 bhaskar    (501) staff       (20)     2382 2022-11-17 04:52:00.000000 tyke-agent-0.1.6/README.md
--rw-rw-r--   0 bhaskar    (501) staff       (20)      106 2022-08-25 14:02:53.000000 tyke-agent-0.1.6/pyproject.toml
--rw-r--r--   0 bhaskar    (501) staff       (20)       38 2022-12-09 10:53:36.560995 tyke-agent-0.1.6/setup.cfg
--rw-rw-r--   0 bhaskar    (501) staff       (20)     2326 2022-12-01 18:38:35.000000 tyke-agent-0.1.6/setup.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2022-12-09 10:53:36.549317 tyke-agent-0.1.6/src/
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2022-12-09 10:53:36.551449 tyke-agent-0.1.6/src/tyke/
--rw-rw-r--   0 bhaskar    (501) staff       (20)      354 2022-10-22 15:56:27.000000 tyke-agent-0.1.6/src/tyke/__init__.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2022-12-09 10:53:36.552584 tyke-agent-0.1.6/src/tyke/agent/
--rw-rw-r--   0 bhaskar    (501) staff       (20)     9316 2022-10-25 05:16:51.000000 tyke-agent-0.1.6/src/tyke/agent/__init__.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2022-12-09 10:53:36.553433 tyke-agent-0.1.6/src/tyke/agent/autoinstrumentation/
--rw-rw-r--   0 bhaskar    (501) staff       (20)        0 2022-08-25 14:02:53.000000 tyke-agent-0.1.6/src/tyke/agent/autoinstrumentation/__init__.py
--rw-rw-r--   0 bhaskar    (501) staff       (20)      625 2022-10-22 16:49:39.000000 tyke-agent-0.1.6/src/tyke/agent/autoinstrumentation/sitecustomize.py
--rw-rw-r--   0 bhaskar    (501) staff       (20)     2125 2022-10-22 15:55:10.000000 tyke-agent-0.1.6/src/tyke/agent/autoinstrumentation/tyke_instrument.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2022-12-09 10:53:36.554744 tyke-agent-0.1.6/src/tyke/agent/config/
--rw-rw-r--   0 bhaskar    (501) staff       (20)     7552 2022-10-25 03:02:38.000000 tyke-agent-0.1.6/src/tyke/agent/config/__init__.py
--rw-r--r--   0 bhaskar    (501) staff       (20)     4658 2022-11-30 14:36:51.000000 tyke-agent-0.1.6/src/tyke/agent/config/config_pb2.py
--rw-rw-r--   0 bhaskar    (501) staff       (20)      847 2022-08-25 14:02:53.000000 tyke-agent-0.1.6/src/tyke/agent/config/default.py
--rw-rw-r--   0 bhaskar    (501) staff       (20)     5838 2022-10-22 15:56:27.000000 tyke-agent-0.1.6/src/tyke/agent/config/environment.py
--rw-rw-r--   0 bhaskar    (501) staff       (20)      913 2022-10-25 03:02:41.000000 tyke-agent-0.1.6/src/tyke/agent/config/file.py
--rw-rw-r--   0 bhaskar    (501) staff       (20)      462 2022-10-25 02:36:21.000000 tyke-agent-0.1.6/src/tyke/agent/constants.py
--rw-rw-r--   0 bhaskar    (501) staff       (20)     1240 2022-10-22 15:56:27.000000 tyke-agent-0.1.6/src/tyke/agent/custom_logger.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2022-12-09 10:53:36.555215 tyke-agent-0.1.6/src/tyke/agent/filter/
--rw-rw-r--   0 bhaskar    (501) staff       (20)      951 2022-08-25 14:02:53.000000 tyke-agent-0.1.6/src/tyke/agent/filter/__init__.py
--rw-rw-r--   0 bhaskar    (501) staff       (20)     1353 2022-10-22 15:56:27.000000 tyke-agent-0.1.6/src/tyke/agent/filter/registry.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2022-12-09 10:53:36.555489 tyke-agent-0.1.6/src/tyke/agent/init/
--rw-rw-r--   0 bhaskar    (501) staff       (20)     8927 2022-10-22 15:56:25.000000 tyke-agent-0.1.6/src/tyke/agent/init/__init__.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2022-12-09 10:53:36.555988 tyke-agent-0.1.6/src/tyke/agent/instrumentation/
--rw-rw-r--   0 bhaskar    (501) staff       (20)    13041 2022-12-09 09:41:41.000000 tyke-agent-0.1.6/src/tyke/agent/instrumentation/__init__.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2022-12-09 10:53:36.556197 tyke-agent-0.1.6/src/tyke/agent/instrumentation/aiohttp/
--rw-rw-r--   0 bhaskar    (501) staff       (20)     7670 2022-10-25 02:36:48.000000 tyke-agent-0.1.6/src/tyke/agent/instrumentation/aiohttp/__init__.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2022-12-09 10:53:36.556836 tyke-agent-0.1.6/src/tyke/agent/instrumentation/aws_lambda/
--rw-rw-r--   0 bhaskar    (501) staff       (20)     9227 2022-10-22 16:49:39.000000 tyke-agent-0.1.6/src/tyke/agent/instrumentation/aws_lambda/__init__.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2022-12-09 10:53:36.557171 tyke-agent-0.1.6/src/tyke/agent/instrumentation/boto/
--rw-rw-r--   0 bhaskar    (501) staff       (20)      488 2022-10-22 16:49:39.000000 tyke-agent-0.1.6/src/tyke/agent/instrumentation/boto/__init__.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2022-12-09 10:53:36.557364 tyke-agent-0.1.6/src/tyke/agent/instrumentation/botocore/
--rw-rw-r--   0 bhaskar    (501) staff       (20)      511 2022-10-22 16:49:39.000000 tyke-agent-0.1.6/src/tyke/agent/instrumentation/botocore/__init__.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2022-12-09 10:53:36.557735 tyke-agent-0.1.6/src/tyke/agent/instrumentation/django/
--rw-rw-r--   0 bhaskar    (501) staff       (20)     3201 2022-10-31 06:05:42.000000 tyke-agent-0.1.6/src/tyke/agent/instrumentation/django/__init__.py
--rw-rw-r--   0 bhaskar    (501) staff       (20)     3455 2022-10-26 19:28:45.000000 tyke-agent-0.1.6/src/tyke/agent/instrumentation/django/django_auto_instrumentation_compat.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2022-12-09 10:53:36.558103 tyke-agent-0.1.6/src/tyke/agent/instrumentation/fast_api/
--rw-rw-r--   0 bhaskar    (501) staff       (20)     8052 2022-10-25 02:36:53.000000 tyke-agent-0.1.6/src/tyke/agent/instrumentation/fast_api/__init__.py
--rw-rw-r--   0 bhaskar    (501) staff       (20)     2816 2022-10-22 15:56:26.000000 tyke-agent-0.1.6/src/tyke/agent/instrumentation/fast_api/fast_api_auto_instrumentation_compat.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2022-12-09 10:53:36.558312 tyke-agent-0.1.6/src/tyke/agent/instrumentation/flask/
--rw-rw-r--   0 bhaskar    (501) staff       (20)     7903 2022-10-25 02:37:00.000000 tyke-agent-0.1.6/src/tyke/agent/instrumentation/flask/__init__.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2022-12-09 10:53:36.558552 tyke-agent-0.1.6/src/tyke/agent/instrumentation/grpc/
--rw-rw-r--   0 bhaskar    (501) staff       (20)    11626 2022-10-25 02:37:01.000000 tyke-agent-0.1.6/src/tyke/agent/instrumentation/grpc/__init__.py
--rw-rw-r--   0 bhaskar    (501) staff       (20)     4344 2022-10-22 15:56:27.000000 tyke-agent-0.1.6/src/tyke/agent/instrumentation/instrumentation_definitions.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2022-12-09 10:53:36.558806 tyke-agent-0.1.6/src/tyke/agent/instrumentation/mysql/
--rw-rw-r--   0 bhaskar    (501) staff       (20)      483 2022-10-22 16:49:39.000000 tyke-agent-0.1.6/src/tyke/agent/instrumentation/mysql/__init__.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2022-12-09 10:53:36.559049 tyke-agent-0.1.6/src/tyke/agent/instrumentation/postgresql/
--rw-rw-r--   0 bhaskar    (501) staff       (20)      503 2022-10-22 16:49:39.000000 tyke-agent-0.1.6/src/tyke/agent/instrumentation/postgresql/__init__.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2022-12-09 10:53:36.559398 tyke-agent-0.1.6/src/tyke/agent/instrumentation/requests/
--rw-rw-r--   0 bhaskar    (501) staff       (20)     3238 2022-12-02 13:46:43.000000 tyke-agent-0.1.6/src/tyke/agent/instrumentation/requests/__init__.py
--rw-rw-r--   0 bhaskar    (501) staff       (20)      502 2022-10-25 04:51:53.000000 tyke-agent-0.1.6/src/tyke/env_var_settings.py
--rw-rw-r--   0 bhaskar    (501) staff       (20)       92 2022-12-09 10:29:54.000000 tyke-agent-0.1.6/src/tyke/version.py
-drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2022-12-09 10:53:36.560570 tyke-agent-0.1.6/src/tyke_agent.egg-info/
--rw-r--r--   0 bhaskar    (501) staff       (20)     2856 2022-12-09 10:53:36.000000 tyke-agent-0.1.6/src/tyke_agent.egg-info/PKG-INFO
--rw-r--r--   0 bhaskar    (501) staff       (20)     1671 2022-12-09 10:53:36.000000 tyke-agent-0.1.6/src/tyke_agent.egg-info/SOURCES.txt
--rw-r--r--   0 bhaskar    (501) staff       (20)        1 2022-12-09 10:53:36.000000 tyke-agent-0.1.6/src/tyke_agent.egg-info/dependency_links.txt
--rw-r--r--   0 bhaskar    (501) staff       (20)       87 2022-12-09 10:53:36.000000 tyke-agent-0.1.6/src/tyke_agent.egg-info/entry_points.txt
--rw-r--r--   0 bhaskar    (501) staff       (20)      840 2022-12-09 10:53:36.000000 tyke-agent-0.1.6/src/tyke_agent.egg-info/requires.txt
--rw-r--r--   0 bhaskar    (501) staff       (20)        5 2022-12-09 10:53:36.000000 tyke-agent-0.1.6/src/tyke_agent.egg-info/top_level.txt
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.714450 tyke-agent-0.1.7/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)    11348 2023-05-11 10:33:50.000000 tyke-agent-0.1.7/LICENSE
+-rw-r--r--   0 bhaskar    (501) staff       (20)     2975 2023-05-16 04:36:37.714275 tyke-agent-0.1.7/PKG-INFO
+-rw-rw-r--   0 bhaskar    (501) staff       (20)     2501 2023-05-16 04:33:41.000000 tyke-agent-0.1.7/README.md
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      106 2022-08-25 14:02:53.000000 tyke-agent-0.1.7/pyproject.toml
+-rw-r--r--   0 bhaskar    (501) staff       (20)       38 2023-05-16 04:36:37.714488 tyke-agent-0.1.7/setup.cfg
+-rw-rw-r--   0 bhaskar    (501) staff       (20)     3251 2023-05-11 14:13:14.000000 tyke-agent-0.1.7/setup.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.696226 tyke-agent-0.1.7/src/
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.698463 tyke-agent-0.1.7/src/tyke/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      354 2022-10-22 15:56:27.000000 tyke-agent-0.1.7/src/tyke/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.699494 tyke-agent-0.1.7/src/tyke/agent/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)    13249 2023-05-16 03:46:27.000000 tyke-agent-0.1.7/src/tyke/agent/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.700209 tyke-agent-0.1.7/src/tyke/agent/autoinstrumentation/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)        0 2022-08-25 14:02:53.000000 tyke-agent-0.1.7/src/tyke/agent/autoinstrumentation/__init__.py
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      625 2022-10-22 16:49:39.000000 tyke-agent-0.1.7/src/tyke/agent/autoinstrumentation/sitecustomize.py
+-rw-rw-r--   0 bhaskar    (501) staff       (20)     2125 2022-10-22 15:55:10.000000 tyke-agent-0.1.7/src/tyke/agent/autoinstrumentation/tyke_instrument.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.701517 tyke-agent-0.1.7/src/tyke/agent/config/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)     7552 2022-10-25 03:02:38.000000 tyke-agent-0.1.7/src/tyke/agent/config/__init__.py
+-rw-r--r--   0 bhaskar    (501) staff       (20)     4658 2022-11-30 14:36:51.000000 tyke-agent-0.1.7/src/tyke/agent/config/config_pb2.py
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      847 2022-08-25 14:02:53.000000 tyke-agent-0.1.7/src/tyke/agent/config/default.py
+-rw-rw-r--   0 bhaskar    (501) staff       (20)     5838 2022-10-22 15:56:27.000000 tyke-agent-0.1.7/src/tyke/agent/config/environment.py
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      913 2022-10-25 03:02:41.000000 tyke-agent-0.1.7/src/tyke/agent/config/file.py
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      462 2022-10-25 02:36:21.000000 tyke-agent-0.1.7/src/tyke/agent/constants.py
+-rw-rw-r--   0 bhaskar    (501) staff       (20)     1240 2022-10-22 15:56:27.000000 tyke-agent-0.1.7/src/tyke/agent/custom_logger.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.701903 tyke-agent-0.1.7/src/tyke/agent/filter/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      951 2022-08-25 14:02:53.000000 tyke-agent-0.1.7/src/tyke/agent/filter/__init__.py
+-rw-rw-r--   0 bhaskar    (501) staff       (20)     1353 2022-10-22 15:56:27.000000 tyke-agent-0.1.7/src/tyke/agent/filter/registry.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.702065 tyke-agent-0.1.7/src/tyke/agent/init/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)     8927 2022-10-22 15:56:25.000000 tyke-agent-0.1.7/src/tyke/agent/init/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.702826 tyke-agent-0.1.7/src/tyke/agent/instrumentation/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)    13041 2022-12-09 09:41:41.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.703131 tyke-agent-0.1.7/src/tyke/agent/instrumentation/aiohttp/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)     7670 2022-10-25 02:36:48.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/aiohttp/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.704006 tyke-agent-0.1.7/src/tyke/agent/instrumentation/aiopg/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      457 2023-05-11 12:39:26.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/aiopg/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.704374 tyke-agent-0.1.7/src/tyke/agent/instrumentation/asyncpg/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      589 2023-05-11 12:00:36.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/asyncpg/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.704675 tyke-agent-0.1.7/src/tyke/agent/instrumentation/aws_lambda/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)     9227 2022-10-22 16:49:39.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/aws_lambda/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.704985 tyke-agent-0.1.7/src/tyke/agent/instrumentation/boto/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      488 2022-10-22 16:49:39.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/boto/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.705325 tyke-agent-0.1.7/src/tyke/agent/instrumentation/botocore/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      511 2022-10-22 16:49:39.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/botocore/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.705542 tyke-agent-0.1.7/src/tyke/agent/instrumentation/celery/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      441 2023-05-11 12:39:40.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/celery/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.705858 tyke-agent-0.1.7/src/tyke/agent/instrumentation/confluent_kafka/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      513 2023-05-11 12:40:05.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/confluent_kafka/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.706874 tyke-agent-0.1.7/src/tyke/agent/instrumentation/django/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)     3201 2022-10-31 06:05:42.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/django/__init__.py
+-rw-rw-r--   0 bhaskar    (501) staff       (20)     3455 2022-10-26 19:28:45.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/django/django_auto_instrumentation_compat.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.707178 tyke-agent-0.1.7/src/tyke/agent/instrumentation/elasticsearch/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      508 2023-05-11 12:40:23.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/elasticsearch/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.707997 tyke-agent-0.1.7/src/tyke/agent/instrumentation/fast_api/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)     8052 2022-10-25 02:36:53.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/fast_api/__init__.py
+-rw-rw-r--   0 bhaskar    (501) staff       (20)     2816 2022-10-22 15:56:26.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/fast_api/fast_api_auto_instrumentation_compat.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.708286 tyke-agent-0.1.7/src/tyke/agent/instrumentation/flask/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)     7903 2022-10-25 02:37:00.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/flask/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.708518 tyke-agent-0.1.7/src/tyke/agent/instrumentation/grpc/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)    11626 2022-10-25 02:37:01.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/grpc/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.708701 tyke-agent-0.1.7/src/tyke/agent/instrumentation/httpx/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      448 2023-05-11 12:38:34.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/httpx/__init__.py
+-rw-rw-r--   0 bhaskar    (501) staff       (20)     7625 2023-05-16 03:44:42.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/instrumentation_definitions.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.709012 tyke-agent-0.1.7/src/tyke/agent/instrumentation/kafka_python/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      456 2023-05-11 12:40:49.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/kafka_python/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.709275 tyke-agent-0.1.7/src/tyke/agent/instrumentation/method/
+-rw-r--r--   0 bhaskar    (501) staff       (20)     1635 2023-05-11 16:45:11.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/method/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.709528 tyke-agent-0.1.7/src/tyke/agent/instrumentation/mysql/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      436 2023-05-11 12:38:55.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/mysql/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.709806 tyke-agent-0.1.7/src/tyke/agent/instrumentation/postgresql/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      565 2023-05-11 12:41:38.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/postgresql/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.710090 tyke-agent-0.1.7/src/tyke/agent/instrumentation/postgresql_binary/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      726 2023-05-15 18:31:15.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/postgresql_binary/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.710345 tyke-agent-0.1.7/src/tyke/agent/instrumentation/pymongo/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      448 2023-05-11 12:41:17.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/pymongo/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.710640 tyke-agent-0.1.7/src/tyke/agent/instrumentation/pymysql/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      447 2023-05-11 12:38:46.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/pymysql/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.710881 tyke-agent-0.1.7/src/tyke/agent/instrumentation/redis/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      435 2023-05-11 12:38:39.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/redis/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.711191 tyke-agent-0.1.7/src/tyke/agent/instrumentation/remoulade/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      459 2023-05-11 12:45:19.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/remoulade/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.711508 tyke-agent-0.1.7/src/tyke/agent/instrumentation/requests/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)     3238 2023-01-05 13:32:00.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/requests/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.711780 tyke-agent-0.1.7/src/tyke/agent/instrumentation/sklearn/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      447 2023-05-11 12:46:52.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/sklearn/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.712087 tyke-agent-0.1.7/src/tyke/agent/instrumentation/sqlalchemy/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      465 2023-05-11 12:48:09.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/sqlalchemy/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.712386 tyke-agent-0.1.7/src/tyke/agent/instrumentation/urllib/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      441 2023-05-11 14:12:39.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/urllib/__init__.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.713013 tyke-agent-0.1.7/src/tyke/agent/instrumentation/urllib3/
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      447 2023-05-11 14:11:23.000000 tyke-agent-0.1.7/src/tyke/agent/instrumentation/urllib3/__init__.py
+-rw-rw-r--   0 bhaskar    (501) staff       (20)      502 2022-10-25 04:51:53.000000 tyke-agent-0.1.7/src/tyke/env_var_settings.py
+-rw-rw-r--   0 bhaskar    (501) staff       (20)       92 2023-05-11 15:06:08.000000 tyke-agent-0.1.7/src/tyke/version.py
+drwxr-xr-x   0 bhaskar    (501) staff       (20)        0 2023-05-16 04:36:37.714082 tyke-agent-0.1.7/src/tyke_agent.egg-info/
+-rw-r--r--   0 bhaskar    (501) staff       (20)     2975 2023-05-16 04:36:37.000000 tyke-agent-0.1.7/src/tyke_agent.egg-info/PKG-INFO
+-rw-r--r--   0 bhaskar    (501) staff       (20)     2563 2023-05-16 04:36:37.000000 tyke-agent-0.1.7/src/tyke_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 bhaskar    (501) staff       (20)        1 2023-05-16 04:36:37.000000 tyke-agent-0.1.7/src/tyke_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 bhaskar    (501) staff       (20)       87 2023-05-16 04:36:37.000000 tyke-agent-0.1.7/src/tyke_agent.egg-info/entry_points.txt
+-rw-r--r--   0 bhaskar    (501) staff       (20)     1589 2023-05-16 04:36:37.000000 tyke-agent-0.1.7/src/tyke_agent.egg-info/requires.txt
+-rw-r--r--   0 bhaskar    (501) staff       (20)        5 2023-05-16 04:36:37.000000 tyke-agent-0.1.7/src/tyke_agent.egg-info/top_level.txt
```

### Comparing `tyke-agent-0.1.6/LICENSE` & `tyke-agent-0.1.7/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright [yyyy] [name of copyright owner]
+   Copyright [2023] [TykeVision,Inc]
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `tyke-agent-0.1.6/PKG-INFO` & `tyke-agent-0.1.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: tyke-agent
-Version: 0.1.6
+Version: 0.1.7
 Summary: Tyke Python Agent
 Home-page: https://tyke.ai
 Author: TykeVision
 Author-email: tech@tyke.ai
 Project-URL: Bug Tracker, https://github.com/tykevision/python-agent/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Tyke Python Agent
 
-Python agent provides instrumentation for collecting relevant data to be processed by [Tyke](https://www.tyke.ai/).
+Tyke Python agent provides instrumentation for collecting traces data to be processed by [Tyke](https://tyke.ai/).
 
 This agent supports these frameworks and adds following capabilities:
 
 - capture request and response headers
 - capture request and response bodies
 - capture SQL queries
 - tracing context propagation
@@ -28,17 +28,18 @@
 
 | Library | Description | Supported Library Versions|
 |------|-------------| ---------------|
 | [flask](https://flask.palletsprojects.com/en/1.1.x/api)|A micro web framework written in Python.| 1.\*, 2.\*|
 | [django](https://docs.djangoproject.com/)|Python web framework | 1.10+|
 | [grpc](https://grpc.github.io/grpc/python/)|Python GRPC library.| 1.27+|
 | [mysql-connector](https://dev.mysql.com/doc/connector-python/en/)| Python MySQL database client library.| 8.\*|
-| [psycopg2/postgresql](https://www.psycopg.org/docs/)|Python Postgresql database client library. | 2.7.3.1+ |
+| [psycopg2/psycopg2-binary/postgresql](https://www.psycopg.org/docs/)|Python Postgresql database client library. | 2.7.3.1+ |
 | [requests](https://docs.python-requests.org/en/master/)|Python HTTP client library.| 2.\*|
 | [aiohttp](https://docs.aiohttp.org/en/stable/)|Python async HTTP client library.| 3.\*|
+| [pymongo](https://pymongo.readthedocs.io/en/stable/)|Python mongodb pymongo library.| >= 3.1+, < 5.0|
 
 ## Getting started
 
 ## Instrumentation
 
 Instrumentation requires editing your code to initialize an agent, and registering any applicable modules to be instrumented.
```

### Comparing `tyke-agent-0.1.6/README.md` & `tyke-agent-0.1.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Tyke Python Agent
 
-Python agent provides instrumentation for collecting relevant data to be processed by [Tyke](https://www.tyke.ai/).
+Tyke Python agent provides instrumentation for collecting traces data to be processed by [Tyke](https://tyke.ai/).
 
 This agent supports these frameworks and adds following capabilities:
 
 - capture request and response headers
 - capture request and response bodies
 - capture SQL queries
 - tracing context propagation
@@ -13,17 +13,18 @@
 
 | Library | Description | Supported Library Versions|
 |------|-------------| ---------------|
 | [flask](https://flask.palletsprojects.com/en/1.1.x/api)|A micro web framework written in Python.| 1.\*, 2.\*|
 | [django](https://docs.djangoproject.com/)|Python web framework | 1.10+|
 | [grpc](https://grpc.github.io/grpc/python/)|Python GRPC library.| 1.27+|
 | [mysql-connector](https://dev.mysql.com/doc/connector-python/en/)| Python MySQL database client library.| 8.\*|
-| [psycopg2/postgresql](https://www.psycopg.org/docs/)|Python Postgresql database client library. | 2.7.3.1+ |
+| [psycopg2/psycopg2-binary/postgresql](https://www.psycopg.org/docs/)|Python Postgresql database client library. | 2.7.3.1+ |
 | [requests](https://docs.python-requests.org/en/master/)|Python HTTP client library.| 2.\*|
 | [aiohttp](https://docs.aiohttp.org/en/stable/)|Python async HTTP client library.| 3.\*|
+| [pymongo](https://pymongo.readthedocs.io/en/stable/)|Python mongodb pymongo library.| >= 3.1+, < 5.0|
 
 ## Getting started
 
 ## Instrumentation
 
 Instrumentation requires editing your code to initialize an agent, and registering any applicable modules to be instrumented.
```

### Comparing `tyke-agent-0.1.6/setup.py` & `tyke-agent-0.1.7/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -46,14 +46,30 @@
         "opentelemetry-instrumentation-flask==0.35b0",
         "opentelemetry-instrumentation-mysql==0.35b0",
         "opentelemetry-instrumentation-psycopg2==0.35b0",
         "opentelemetry-instrumentation-requests==0.35b0",
         "opentelemetry-instrumentation-grpc==0.35b0",
         "opentelemetry-instrumentation-django==0.35b0",
         "opentelemetry-instrumentation-aws-lambda==0.35b0",
+        "opentelemetry-instrumentation-pymongo==0.35b0",
+        "opentelemetry-instrumentation-celery==0.35b0",
+        "opentelemetry-instrumentation-asyncpg==0.35b0",
+        "opentelemetry-instrumentation-asgi==0.35b0",
+        "opentelemetry-instrumentation-aiopg==0.35b0",
+        "opentelemetry-instrumentation-confluent-kafka==0.35b0",
+        "opentelemetry-instrumentation-kafka-python==0.35b0",
+        "opentelemetry-instrumentation-elasticsearch==0.35b0",
+        "opentelemetry-instrumentation-httpx==0.35b0",
+        "opentelemetry-instrumentation-pymysql==0.35b0",
+        "opentelemetry-instrumentation-redis==0.35b0",
+        "opentelemetry-instrumentation-remoulade==0.35b0",
+        "opentelemetry-instrumentation-sklearn==0.35b0",
+        "opentelemetry-instrumentation-sqlalchemy==0.35b0",
+        "opentelemetry-instrumentation-urllib3==0.35b0",
+        "opentelemetry-instrumentation-urllib==0.35b0",
         "opentelemetry-propagator-b3==1.14.0",
         "opentelemetry-sdk==1.14.0",
         "opentelemetry-util-http==0.35b0",
         "deprecated==1.2.12",
         "google>=3.0.0",
         "pyyaml",
         "protobuf>=3.20.1"
```

### Comparing `tyke-agent-0.1.6/src/tyke/agent/__init__.py` & `tyke-agent-0.1.7/src/tyke/agent/instrumentation/flask/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,206 +1,188 @@
-'''Main entry point for Tyke agent module.'''
-import os
+'''Tyke flask instrumentor module wrapper.''' # pylint: disable=R0401
 import sys
-import threading
+import os.path
+import logging
+import inspect
 import traceback
-from contextlib import contextmanager
+import json
+import flask
+from opentelemetry.instrumentation.flask import (
+    _InstrumentedFlask,
+    FlaskInstrumentor,
+    _ENVIRON_SPAN_KEY,
+)
+from werkzeug.exceptions import Forbidden
+
+from tyke.agent import constants  # pylint: disable=R0801
+from tyke.agent.filter.registry import Registry, TYPE_HTTP
+from tyke.agent.instrumentation import BaseInstrumentorWrapper
 
-from deprecated import deprecated
-import opentelemetry.trace as ot
-
-from tyke.agent.instrumentation.instrumentation_definitions import SUPPORTED_LIBRARIES, \
-    get_instrumentation_wrapper, REQUESTS_KEY, GRPC_CLIENT_KEY, DJANGO_KEY, MYSQL_KEY, GRPC_SERVER_KEY, \
-    POSTGRESQL_KEY, AIOHTTP_CLIENT_KEY, FLASK_KEY, LAMBDA,FAST_API_KEY, _uninstrument_all
-from tyke.env_var_settings import get_env_value
-from tyke.agent.init import AgentInit
 from tyke.agent.config import AgentConfig
-from tyke.agent import constants
-from tyke.agent import custom_logger
-from tyke.version import __version__
-# The Tyke Python Agent class
-
-logger = custom_logger.get_custom_logger(__name__)
-
-
-class Agent:
-    '''Top-level entry point for Tyke agent.'''
-    _instance = None
-    _singleton_lock = threading.Lock()
-
-    def __new__(cls):
-        '''constructor'''
-        if cls._instance is None:
-            with cls._singleton_lock:
-                logger.debug('Creating Agent')
-                logger.debug('Python version: %s', sys.version)
-                logger.debug('Tyke Agent version: %s', __version__)
-                cls._instance = super(Agent, cls).__new__(cls)
-                cls._instance._initialized = False
-        else:
-            logger.debug('Using existing Agent.')
-        return cls._instance
 
-    def __init__(self):
-        '''Initializer'''
-        self._initialized = False
-        if not self._initialized:  # pylint: disable=E0203:
-            logger.debug('Initializing Agent.')
-            if not self.is_enabled():
-                return
-            try:
-                self._config = AgentConfig()
-                self._init = AgentInit(self._config)
-                self._initialized = True
-            except Exception as err:  # pylint: disable=W0703
-                logger.error('Failed to initialize Agent: exception=%s, stacktrace=%s',
-                             err,
-                             traceback.format_exc())
-
-    @contextmanager
-    def edit_config(self):
-        """Used by end users to modify the config"""
+# Initialize logger
+logger = logging.getLogger(__name__)  # pylint: disable=C0103
+
+# Per request pre-handler
+def _tyke_before_request(flask_wrapper):
+    '''This function is invoked by flask to set the handler'''
+    def tyke_before_request() -> None:
+        '''Tyke before_request() method'''
+        logger.debug('Entering _tyke_before_request().')
         try:
-            # need to explicitly set this as None when modifying the config via code
-            # to regenerate Trace Provider with new options
-            ot._TRACER_PROVIDER = None  # pylint:disable=W0212
-            agent_config = self._config.agent_config
-            yield agent_config
-            self._config.agent_config = agent_config
-        finally:
-            self._init.apply_config(self._config)
-
-    def instrument(self, app=None, skip_libraries=None, auto_instrument=False):
-        '''used to register applicable instrumentation wrappers'''
-        if skip_libraries is None:
-            skip_libraries = []
-        if not self.is_initialized():
-            logger.debug('agent is not initialized, not instrumenting')
-            return
-
-        for library_key in SUPPORTED_LIBRARIES:
-            if library_key in skip_libraries:
-                logger.debug('not attempting to instrument %s', library_key)
-                continue
-
-            self._instrument(library_key, app, auto_instrument)
-
-    def _instrument(self, library_key, app=None, auto_instrument=False):
-        """only used to allow the deprecated register_x library methods to still work"""
-        wrapper_instance = get_instrumentation_wrapper(library_key)
-        if wrapper_instance is None:
-            return
-
-        # Flask is a special case compared to rest of instrumentation
-        # using tyke-instrument we can replace flask class def before app is initialized
-        # however during code based instr we wrap the existing app
-        # since replacing class def after app is initialized doesnt have an effect
-        # the user has to pass the app in to agent.instrument()
-        # we could resolve this edge case by instead having users directly add the middleware
-        # ex: app = Flask();
-        # app = TykeMiddleware(App) => this in turn does agent.instrument()
-        # + we have ref to app
-        if library_key == FLASK_KEY and app is not None:
-            wrapper_instance.with_app(app)
-
-        # since ht sitecustomize pushes the agent to the front of the load path django instrumentation will error
-        # when using autoinstrumentation since we need the django app settings loaded to add middleware
-        #
-        # in order to resolve this if we detect django we wrap the wsgi/asgi app getter
-        # and instrument as soon as the app is retrieved(since settings have to be configured
-        # before returning loaded app)
-        if library_key == DJANGO_KEY and auto_instrument is True:
-            from tyke.agent.instrumentation.django.django_auto_instrumentation_compat import \
-                add_django_auto_instr_wrappers  # pylint: disable=C0415
-            add_django_auto_instr_wrappers(self, wrapper_instance)
-            return
-
-        # For FastAPI we need a handle to the user app before we can instrument fast & inject middleware
-        # to make things easier for the user always add the below instrumentation wrappers
-        # when FastAPI calls `.setup` take the app and then add instrumentation
-        if library_key == FAST_API_KEY:
-            from tyke.agent.instrumentation.fast_api.fast_api_auto_instrumentation_compat import \
-                add_fast_api_auto_instr_wrappers # pylint: disable=C0415
-            add_fast_api_auto_instr_wrappers(self, wrapper_instance)
-            return
-
-        if library_key == LAMBDA and '_HANDLER' not in os.environ:
-            return
-
-        self.register_library(library_key, wrapper_instance)
-
-    def register_library(self, library_name, wrapper_instance):
-        """will configure settings on an instrumentation wrapper + apply"""
-        logger.debug('attempting to register library instrumentation: %s', library_name)
+            # Read span from flask "environment". The global flask.request
+            # object keeps track of which request belong to the currently
+            # active thread. See
+            #   https://flask.palletsprojects.com/en/1.1.x/api/#flask.request
+            span = flask.request.environ.get(_ENVIRON_SPAN_KEY)
+            # Pull request headers
+            # for now, assuming single threaded mode (multiple python processes)
+            request_headers = flask.request.headers
+            # Pull message body
+            request_body = flask.request.data       # same
+
+            span.update_name(str(flask.request.method) + ' ' + str(flask.request.url_rule))
+
+            # Call base request handler
+            flask_wrapper.generic_request_handler(request_headers, request_body, span)
+
+            block_result = Registry().apply_filters(span,
+                                                    flask.request.url,
+                                                    flask.request.headers,
+                                                    flask.request.data,
+                                                    TYPE_HTTP)
+            if block_result:
+                logger.debug('should block evaluated to true, aborting with 403')
+                flask.abort(403)
+
+        except Forbidden as forbidden_error:
+            raise forbidden_error
+
+        except Exception as err:  # pylint: disable=W0703
+            logger.error(constants.INST_RUNTIME_EXCEPTION_MSSG,
+                         'flask before_request handler',
+                         err,
+                         traceback.format_exc())
+            # Not rethrowing to avoid causing runtime errors for Flask.
+    return tyke_before_request
+
+# Per request post-handler
+def _tyke_after_request(flask_wrapper) -> flask.wrappers.Response:
+    '''This function is invoked by flask to set the handler'''
+    def tyke_after_request(response):
+        '''Tyke after_request method.'''
+        try:
+            logger.debug('Entering _tyke_after_request().')
+            # Read span from flask "environment"
+            span = flask.request.environ.get(_ENVIRON_SPAN_KEY)
+            # Pull response headers
+            response_headers = response.headers
+
+            response_body = ""
+            # dont extract response content if body is a file
+            if not response.direct_passthrough:
+                response_body = response.data
+
+            # Call base response handler
+            flask_wrapper.generic_response_handler(
+                response_headers, response_body, span)
+            return response
+        except Exception as err:  # pylint: disable=W0703
+            logger.error(constants.INST_RUNTIME_EXCEPTION_MSSG,
+                         'flask after_request handler',
+                         err,
+                         traceback.format_exc())
+            # Not rethrowing to avoid causing runtime errors for Flask.
+            return response
+
+    return tyke_after_request
+
+class _TykeInstrumentedFlask(_InstrumentedFlask, BaseInstrumentorWrapper):
+    """Tyke Wrapper class around OTel _InstrumentedFlask. This replaces
+    the flask.Flask class definition."""
+
+    def __init__(self, *args, **kwargs):
+        _InstrumentedFlask.__init__(self, *args, **kwargs)
+        BaseInstrumentorWrapper.__init__(self)
+        self.before_request(_tyke_before_request(self))
+        self.after_request(_tyke_after_request(self))
+        config: AgentConfig = AgentConfig()
+        self.set_process_request_headers(config.agent_config.data_capture.http_headers.request)
+        self.set_process_request_body(config.agent_config.data_capture.http_body.request)
+        self.set_process_response_headers(config.agent_config.data_capture.http_headers.response)
+        self.set_process_response_body(config.agent_config.data_capture.http_body.response)
+        self.set_body_max_size(config.agent_config.data_capture.body_max_size_bytes)
+
+# Main Flask Instrumentor Wrapper class.
+class FlaskInstrumentorWrapper(FlaskInstrumentor, BaseInstrumentorWrapper):
+    '''Tyke wrapper around OTel Flask instrumentor class'''
+
+    def __init__(self):
+        logger.debug('Entering FlaskInstrumentorWrapper constructor.')
+        super().__init__()
+        self._app = None
+
+    def with_app(self, app=None):
+        """when instrumenting via code we need to instrument
+        the app directly, this is conditionally called from agent.instrument"""
+        self._app = app
+
+    def instrument(self, **kwargs):
+        if self._app:
+            # code based instrumentation
+            before_hook = _tyke_before_request(self)
+            after_hook = _tyke_after_request(self)
+            FlaskInstrumentorWrapper.instrument_app(self._app)
+            self._app.before_request(before_hook)
+            self._app.after_request(after_hook)
+        else:
+            # auto instrumentation
+            super().instrument()
+
+
+    def _instrument(self, **kwargs):
+        '''Override OTel method that sets up global flask instrumentation'''
+        self._original_flask = flask.Flask # pylint: disable = W0201
+        name_callback = kwargs.get("name_callback")
+        tracer_provider = kwargs.get("tracer_provider")
+        if callable(name_callback):
+            _TykeInstrumentedFlask.name_callback = name_callback
+        _TykeInstrumentedFlask._tracer_provider = tracer_provider # pylint: disable=W0212
+        flask.Flask = _TykeInstrumentedFlask
+
+    # Initialize instrumentation wrapper
+    @staticmethod
+    def instrument_app(app, request_hook=None, response_hook=None, tracer_provider=None, excluded_urls=None):  # pylint:disable=W0221,W0613
+        '''Initialize instrumentation'''
+        logger.debug('Entering FlaskInstrumentorWrapper.instument_app().')
         try:
-            self._init.init_library_instrumentation(library_name, wrapper_instance)
+
+            # Call parent class's initialization
+            FlaskInstrumentor.instrument_app(app, request_hook, response_hook)
+
         except Exception as err:  # pylint: disable=W0703
-            logger.debug(constants.EXCEPTION_MESSAGE, library_name, err, traceback.format_exc())
+            logger.error("""An error occurred initializing flask otel
+                            instrumentor: exception=%s, stacktrace=%s""",
+                         err,
+                         traceback.format_exc())
+            raise err
+
+    # Teardown instrumentation wrapper
+    @staticmethod
+    def uninstrument_app(app) -> None:
+        '''Disable instrumentation'''
+        logger.debug('Entering FlaskInstrumentorWrapper.uninstrument_app()')
+        try:
+            # Call parent's teardown logic
+            super().uninstrument_app(app)  # pylint: disable=E1101
 
-    def register_processor(self, processor) -> None:  # pylint: disable=R1710
-        '''Add additional span exporters + processors'''
-        logger.debug('Entering Agent.register_processor().')
-        logger.debug("initialized %s", self.is_initialized())
-        if not self.is_initialized():
-            return None
-        return self._init.register_processor(processor)
-
-    def is_enabled(self) -> bool:  # pylint: disable=R0201
-        '''Is agent enabled?'''
-        enabled = get_env_value('ENABLED')
-        if enabled:
-            if enabled.lower() == 'false':
-                logger.debug("ENABLED is disabled.")
-                return False
-        return True
-
-    def is_initialized(self) -> bool:  # pylint: disable=R0201
-        '''Is agent initialized - if an agent fails to init we should let the app continue'''
-        if not self.is_enabled():
-            return False
-        if not self._initialized:
-            return False
-        return True
-
-    # These methods are deprecated and replaced by a single call to `agent_instance.instrument()`
-    AGENT_INSTRUMENT_INSTEAD = "You should use agent.instrument() instead"
-    AGENT_INSTRUMENT_VERSION = '0.1.0'
-
-    @deprecated(version=AGENT_INSTRUMENT_VERSION, reason=AGENT_INSTRUMENT_INSTEAD)
-    def register_requests(self):
-        """just a proxy to support deprecated method for instrumenting requests"""
-        self._instrument(REQUESTS_KEY)
-
-    @deprecated(version=AGENT_INSTRUMENT_VERSION, reason=AGENT_INSTRUMENT_INSTEAD)
-    def register_grpc_client(self):
-        """just a proxy to support deprecated method for instrumenting grpc_client"""
-        self._instrument(GRPC_CLIENT_KEY)
-
-    @deprecated(version=AGENT_INSTRUMENT_VERSION, reason=AGENT_INSTRUMENT_INSTEAD)
-    def register_django(self):
-        """just a proxy to support deprecated method for instrumenting django"""
-        self._instrument(DJANGO_KEY)
-
-    @deprecated(version=AGENT_INSTRUMENT_VERSION, reason=AGENT_INSTRUMENT_INSTEAD)
-    def register_mysql(self):
-        """just a proxy to support deprecated method for instrumenting mysql"""
-        self._instrument(MYSQL_KEY)
-
-    @deprecated(version=AGENT_INSTRUMENT_VERSION, reason=AGENT_INSTRUMENT_INSTEAD)
-    def register_grpc_server(self):
-        """just a proxy to support deprecated method for instrumenting grpc server"""
-        self._instrument(GRPC_SERVER_KEY)
-
-    @deprecated(version=AGENT_INSTRUMENT_VERSION, reason=AGENT_INSTRUMENT_INSTEAD)
-    def register_postgresql(self):
-        """just a proxy to support deprecated method for instrumenting postgresql"""
-        self._instrument(POSTGRESQL_KEY)
-
-    @deprecated(version=AGENT_INSTRUMENT_VERSION, reason=AGENT_INSTRUMENT_INSTEAD)
-    def register_aiohttp_client(self):
-        """just a proxy to support deprecated method for instrumenting aiohttp"""
-        self._instrument(AIOHTTP_CLIENT_KEY)
-
-    @deprecated(version=AGENT_INSTRUMENT_VERSION, reason=AGENT_INSTRUMENT_INSTEAD)
-    def register_flask_app(self, app=None):
-        """just a proxy to support deprecated method for instrumenting flask"""
-        self._instrument(FLASK_KEY, app)
+        except Exception as err:  # pylint: disable=W0703
+            logger.error("""An error occurred while shutting down flask otel
+                         instrumentor: exception=%s, stacktrace=%s""",
+                         err,
+                         traceback.format_exc())
+            raise err
+
+    # retrieve flask app
+    def get_app(self) -> flask.Flask:
+        '''Return the flask app object.'''
+        return self._app
```

### Comparing `tyke-agent-0.1.6/src/tyke/agent/autoinstrumentation/sitecustomize.py` & `tyke-agent-0.1.7/src/tyke/agent/autoinstrumentation/sitecustomize.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.6/src/tyke/agent/autoinstrumentation/tyke_instrument.py` & `tyke-agent-0.1.7/src/tyke/agent/autoinstrumentation/tyke_instrument.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.6/src/tyke/agent/config/__init__.py` & `tyke-agent-0.1.7/src/tyke/agent/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.6/src/tyke/agent/config/config_pb2.py` & `tyke-agent-0.1.7/src/tyke/agent/config/config_pb2.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.6/src/tyke/agent/config/default.py` & `tyke-agent-0.1.7/src/tyke/agent/config/default.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.6/src/tyke/agent/config/environment.py` & `tyke-agent-0.1.7/src/tyke/agent/config/environment.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.6/src/tyke/agent/config/file.py` & `tyke-agent-0.1.7/src/tyke/agent/config/file.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.6/src/tyke/agent/custom_logger.py` & `tyke-agent-0.1.7/src/tyke/agent/custom_logger.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.6/src/tyke/agent/filter/__init__.py` & `tyke-agent-0.1.7/src/tyke/agent/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.6/src/tyke/agent/filter/registry.py` & `tyke-agent-0.1.7/src/tyke/agent/filter/registry.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.6/src/tyke/agent/init/__init__.py` & `tyke-agent-0.1.7/src/tyke/agent/init/__init__.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.6/src/tyke/agent/instrumentation/__init__.py` & `tyke-agent-0.1.7/src/tyke/agent/instrumentation/__init__.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.6/src/tyke/agent/instrumentation/aiohttp/__init__.py` & `tyke-agent-0.1.7/src/tyke/agent/instrumentation/aiohttp/__init__.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.6/src/tyke/agent/instrumentation/aws_lambda/__init__.py` & `tyke-agent-0.1.7/src/tyke/agent/instrumentation/aws_lambda/__init__.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.6/src/tyke/agent/instrumentation/django/__init__.py` & `tyke-agent-0.1.7/src/tyke/agent/instrumentation/django/__init__.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.6/src/tyke/agent/instrumentation/django/django_auto_instrumentation_compat.py` & `tyke-agent-0.1.7/src/tyke/agent/instrumentation/django/django_auto_instrumentation_compat.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.6/src/tyke/agent/instrumentation/fast_api/__init__.py` & `tyke-agent-0.1.7/src/tyke/agent/instrumentation/fast_api/__init__.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.6/src/tyke/agent/instrumentation/fast_api/fast_api_auto_instrumentation_compat.py` & `tyke-agent-0.1.7/src/tyke/agent/instrumentation/fast_api/fast_api_auto_instrumentation_compat.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.6/src/tyke/agent/instrumentation/grpc/__init__.py` & `tyke-agent-0.1.7/src/tyke/agent/instrumentation/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.6/src/tyke/agent/instrumentation/requests/__init__.py` & `tyke-agent-0.1.7/src/tyke/agent/instrumentation/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `tyke-agent-0.1.6/src/tyke_agent.egg-info/PKG-INFO` & `tyke-agent-0.1.7/src/tyke_agent.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: tyke-agent
-Version: 0.1.6
+Version: 0.1.7
 Summary: Tyke Python Agent
 Home-page: https://tyke.ai
 Author: TykeVision
 Author-email: tech@tyke.ai
 Project-URL: Bug Tracker, https://github.com/tykevision/python-agent/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Tyke Python Agent
 
-Python agent provides instrumentation for collecting relevant data to be processed by [Tyke](https://www.tyke.ai/).
+Tyke Python agent provides instrumentation for collecting traces data to be processed by [Tyke](https://tyke.ai/).
 
 This agent supports these frameworks and adds following capabilities:
 
 - capture request and response headers
 - capture request and response bodies
 - capture SQL queries
 - tracing context propagation
@@ -28,17 +28,18 @@
 
 | Library | Description | Supported Library Versions|
 |------|-------------| ---------------|
 | [flask](https://flask.palletsprojects.com/en/1.1.x/api)|A micro web framework written in Python.| 1.\*, 2.\*|
 | [django](https://docs.djangoproject.com/)|Python web framework | 1.10+|
 | [grpc](https://grpc.github.io/grpc/python/)|Python GRPC library.| 1.27+|
 | [mysql-connector](https://dev.mysql.com/doc/connector-python/en/)| Python MySQL database client library.| 8.\*|
-| [psycopg2/postgresql](https://www.psycopg.org/docs/)|Python Postgresql database client library. | 2.7.3.1+ |
+| [psycopg2/psycopg2-binary/postgresql](https://www.psycopg.org/docs/)|Python Postgresql database client library. | 2.7.3.1+ |
 | [requests](https://docs.python-requests.org/en/master/)|Python HTTP client library.| 2.\*|
 | [aiohttp](https://docs.aiohttp.org/en/stable/)|Python async HTTP client library.| 3.\*|
+| [pymongo](https://pymongo.readthedocs.io/en/stable/)|Python mongodb pymongo library.| >= 3.1+, < 5.0|
 
 ## Getting started
 
 ## Instrumentation
 
 Instrumentation requires editing your code to initialize an agent, and registering any applicable modules to be instrumented.
```

