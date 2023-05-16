# Comparing `tmp/amqp_workers-0.1.1.tar.gz` & `tmp/amqp_workers-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amqp_workers-0.1.1.tar", max compression
+gzip compressed data, was "amqp_workers-0.1.2.tar", max compression
```

## Comparing `amqp_workers-0.1.1.tar` & `amqp_workers-0.1.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0        0 2023-04-27 01:38:48.372295 amqp_workers-0.1.1/amqpworker/__init__.py
--rw-r--r--   0        0        0     8274 2023-05-08 09:50:20.919904 amqp_workers-0.1.1/amqpworker/app.py
--rw-r--r--   0        0        0      899 2023-04-27 00:37:11.054428 amqp_workers-0.1.1/amqpworker/bucket.py
--rw-r--r--   0        0        0     1108 2023-04-28 03:13:55.374031 amqp_workers-0.1.1/amqpworker/conf.py
--rw-r--r--   0        0        0     5247 2023-04-27 04:04:35.910995 amqp_workers-0.1.1/amqpworker/connections.py
--rw-r--r--   0        0        0     9263 2023-05-12 00:55:25.860622 amqp_workers-0.1.1/amqpworker/consumer.py
--rw-r--r--   0        0        0      867 2023-04-27 02:02:41.661122 amqp_workers-0.1.1/amqpworker/decorators.py
--rw-r--r--   0        0        0        0 2023-04-27 00:37:11.056429 amqp_workers-0.1.1/amqpworker/easyqueue/__init__.py
--rw-r--r--   0        0        0     2300 2023-04-27 06:31:02.852491 amqp_workers-0.1.1/amqpworker/easyqueue/connection.py
--rw-r--r--   0        0        0      415 2023-04-27 00:37:11.056929 amqp_workers-0.1.1/amqpworker/easyqueue/exceptions.py
--rw-r--r--   0        0        0     2660 2023-05-11 08:31:00.365632 amqp_workers-0.1.1/amqpworker/easyqueue/message.py
--rw-r--r--   0        0        0    12224 2023-05-11 08:31:00.389109 amqp_workers-0.1.1/amqpworker/easyqueue/queue.py
--rw-r--r--   0        0        0      652 2023-04-28 02:06:33.017336 amqp_workers-0.1.1/amqpworker/entrypoints.py
--rw-r--r--   0        0        0      220 2023-04-27 00:37:11.058429 amqp_workers-0.1.1/amqpworker/exceptions.py
--rw-r--r--   0        0        0      918 2023-04-28 02:06:33.010338 amqp_workers-0.1.1/amqpworker/options.py
--rw-r--r--   0        0        0      102 2023-04-27 03:25:18.698414 amqp_workers-0.1.1/amqpworker/rabbitmq/__init__.py
--rw-r--r--   0        0        0     1217 2023-04-28 02:06:33.068336 amqp_workers-0.1.1/amqpworker/rabbitmq/entrypoints.py
--rw-r--r--   0        0        0     2040 2023-04-27 08:36:53.107610 amqp_workers-0.1.1/amqpworker/rabbitmq/message.py
--rw-r--r--   0        0        0     3815 2023-04-28 02:06:33.060333 amqp_workers-0.1.1/amqpworker/routes.py
--rw-r--r--   0        0        0     6701 2023-04-28 00:01:14.997514 amqp_workers-0.1.1/amqpworker/scheduled/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 01:46:21.379571 amqp_workers-0.1.1/amqpworker/signals/__init__.py
--rw-r--r--   0        0        0     1023 2023-04-27 01:53:14.068404 amqp_workers-0.1.1/amqpworker/signals/base.py
--rw-r--r--   0        0        0        0 2023-04-27 01:49:26.864472 amqp_workers-0.1.1/amqpworker/signals/handlers/__init__.py
--rw-r--r--   0        0        0      288 2023-04-27 02:02:41.649901 amqp_workers-0.1.1/amqpworker/signals/handlers/base.py
--rw-r--r--   0        0        0     1613 2023-04-28 01:28:30.030083 amqp_workers-0.1.1/amqpworker/signals/handlers/rabbitmq.py
--rw-r--r--   0        0        0        0 2023-04-27 00:37:11.071433 amqp_workers-0.1.1/amqpworker/types/__init__.py
--rw-r--r--   0        0        0     1611 2023-04-27 03:21:21.484561 amqp_workers-0.1.1/amqpworker/types/registry.py
--rw-r--r--   0        0        0     1688 2023-04-27 03:25:18.733914 amqp_workers-0.1.1/amqpworker/typing/__init__.py
--rw-r--r--   0        0        0      208 2023-04-27 05:43:33.253806 amqp_workers-0.1.1/amqpworker/utils.py
--rw-r--r--   0        0        0     1131 2023-05-08 08:02:08.608402 amqp_workers-0.1.1/LICENSE
--rw-r--r--   0        0        0      974 2023-05-12 01:53:10.320022 amqp_workers-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2970 2023-05-11 09:30:42.780253 amqp_workers-0.1.1/README.md
--rw-r--r--   0        0        0     3776 1970-01-01 00:00:00.000000 amqp_workers-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-27 01:38:48.372295 amqp_workers-0.1.2/amqpworker/__init__.py
+-rw-r--r--   0        0        0     8274 2023-05-08 09:50:20.919904 amqp_workers-0.1.2/amqpworker/app.py
+-rw-r--r--   0        0        0      899 2023-04-27 00:37:11.054428 amqp_workers-0.1.2/amqpworker/bucket.py
+-rw-r--r--   0        0        0     1108 2023-04-28 03:13:55.374031 amqp_workers-0.1.2/amqpworker/conf.py
+-rw-r--r--   0        0        0     5247 2023-04-27 04:04:35.910995 amqp_workers-0.1.2/amqpworker/connections.py
+-rw-r--r--   0        0        0     9263 2023-05-12 00:55:25.860622 amqp_workers-0.1.2/amqpworker/consumer.py
+-rw-r--r--   0        0        0      867 2023-04-27 02:02:41.661122 amqp_workers-0.1.2/amqpworker/decorators.py
+-rw-r--r--   0        0        0        0 2023-04-27 00:37:11.056429 amqp_workers-0.1.2/amqpworker/easyqueue/__init__.py
+-rw-r--r--   0        0        0     2300 2023-04-27 06:31:02.852491 amqp_workers-0.1.2/amqpworker/easyqueue/connection.py
+-rw-r--r--   0        0        0      415 2023-04-27 00:37:11.056929 amqp_workers-0.1.2/amqpworker/easyqueue/exceptions.py
+-rw-r--r--   0        0        0     2660 2023-05-11 08:31:00.365632 amqp_workers-0.1.2/amqpworker/easyqueue/message.py
+-rw-r--r--   0        0        0    12224 2023-05-11 08:31:00.389109 amqp_workers-0.1.2/amqpworker/easyqueue/queue.py
+-rw-r--r--   0        0        0      652 2023-04-28 02:06:33.017336 amqp_workers-0.1.2/amqpworker/entrypoints.py
+-rw-r--r--   0        0        0      220 2023-04-27 00:37:11.058429 amqp_workers-0.1.2/amqpworker/exceptions.py
+-rw-r--r--   0        0        0      918 2023-04-28 02:06:33.010338 amqp_workers-0.1.2/amqpworker/options.py
+-rw-r--r--   0        0        0      102 2023-04-27 03:25:18.698414 amqp_workers-0.1.2/amqpworker/rabbitmq/__init__.py
+-rw-r--r--   0        0        0     1217 2023-04-28 02:06:33.068336 amqp_workers-0.1.2/amqpworker/rabbitmq/entrypoints.py
+-rw-r--r--   0        0        0     2040 2023-04-27 08:36:53.107610 amqp_workers-0.1.2/amqpworker/rabbitmq/message.py
+-rw-r--r--   0        0        0     3815 2023-04-28 02:06:33.060333 amqp_workers-0.1.2/amqpworker/routes.py
+-rw-r--r--   0        0        0     6701 2023-04-28 00:01:14.997514 amqp_workers-0.1.2/amqpworker/scheduled/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 01:46:21.379571 amqp_workers-0.1.2/amqpworker/signals/__init__.py
+-rw-r--r--   0        0        0     1023 2023-04-27 01:53:14.068404 amqp_workers-0.1.2/amqpworker/signals/base.py
+-rw-r--r--   0        0        0        0 2023-04-27 01:49:26.864472 amqp_workers-0.1.2/amqpworker/signals/handlers/__init__.py
+-rw-r--r--   0        0        0      288 2023-04-27 02:02:41.649901 amqp_workers-0.1.2/amqpworker/signals/handlers/base.py
+-rw-r--r--   0        0        0     1613 2023-04-28 01:28:30.030083 amqp_workers-0.1.2/amqpworker/signals/handlers/rabbitmq.py
+-rw-r--r--   0        0        0        0 2023-04-27 00:37:11.071433 amqp_workers-0.1.2/amqpworker/types/__init__.py
+-rw-r--r--   0        0        0     1611 2023-04-27 03:21:21.484561 amqp_workers-0.1.2/amqpworker/types/registry.py
+-rw-r--r--   0        0        0     1688 2023-04-27 03:25:18.733914 amqp_workers-0.1.2/amqpworker/typing/__init__.py
+-rw-r--r--   0        0        0      208 2023-04-27 05:43:33.253806 amqp_workers-0.1.2/amqpworker/utils.py
+-rw-r--r--   0        0        0     1131 2023-05-08 08:02:08.608402 amqp_workers-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1046 2023-05-16 04:17:03.386393 amqp_workers-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2970 2023-05-11 09:30:42.780253 amqp_workers-0.1.2/README.md
+-rw-r--r--   0        0        0     3848 1970-01-01 00:00:00.000000 amqp_workers-0.1.2/PKG-INFO
```

### Comparing `amqp_workers-0.1.1/amqpworker/app.py` & `amqp_workers-0.1.2/amqpworker/app.py`

 * *Files identical despite different names*

### Comparing `amqp_workers-0.1.1/amqpworker/bucket.py` & `amqp_workers-0.1.2/amqpworker/bucket.py`

 * *Files identical despite different names*

### Comparing `amqp_workers-0.1.1/amqpworker/conf.py` & `amqp_workers-0.1.2/amqpworker/conf.py`

 * *Files identical despite different names*

### Comparing `amqp_workers-0.1.1/amqpworker/connections.py` & `amqp_workers-0.1.2/amqpworker/connections.py`

 * *Files identical despite different names*

### Comparing `amqp_workers-0.1.1/amqpworker/consumer.py` & `amqp_workers-0.1.2/amqpworker/consumer.py`

 * *Files identical despite different names*

### Comparing `amqp_workers-0.1.1/amqpworker/decorators.py` & `amqp_workers-0.1.2/amqpworker/decorators.py`

 * *Files identical despite different names*

### Comparing `amqp_workers-0.1.1/amqpworker/easyqueue/connection.py` & `amqp_workers-0.1.2/amqpworker/easyqueue/connection.py`

 * *Files identical despite different names*

### Comparing `amqp_workers-0.1.1/amqpworker/easyqueue/message.py` & `amqp_workers-0.1.2/amqpworker/easyqueue/message.py`

 * *Files identical despite different names*

### Comparing `amqp_workers-0.1.1/amqpworker/easyqueue/queue.py` & `amqp_workers-0.1.2/amqpworker/easyqueue/queue.py`

 * *Files identical despite different names*

### Comparing `amqp_workers-0.1.1/amqpworker/entrypoints.py` & `amqp_workers-0.1.2/amqpworker/entrypoints.py`

 * *Files identical despite different names*

### Comparing `amqp_workers-0.1.1/amqpworker/options.py` & `amqp_workers-0.1.2/amqpworker/options.py`

 * *Files identical despite different names*

### Comparing `amqp_workers-0.1.1/amqpworker/rabbitmq/entrypoints.py` & `amqp_workers-0.1.2/amqpworker/rabbitmq/entrypoints.py`

 * *Files identical despite different names*

### Comparing `amqp_workers-0.1.1/amqpworker/rabbitmq/message.py` & `amqp_workers-0.1.2/amqpworker/rabbitmq/message.py`

 * *Files identical despite different names*

### Comparing `amqp_workers-0.1.1/amqpworker/routes.py` & `amqp_workers-0.1.2/amqpworker/routes.py`

 * *Files identical despite different names*

### Comparing `amqp_workers-0.1.1/amqpworker/scheduled/__init__.py` & `amqp_workers-0.1.2/amqpworker/scheduled/__init__.py`

 * *Files identical despite different names*

### Comparing `amqp_workers-0.1.1/amqpworker/signals/base.py` & `amqp_workers-0.1.2/amqpworker/signals/base.py`

 * *Files identical despite different names*

### Comparing `amqp_workers-0.1.1/amqpworker/signals/handlers/rabbitmq.py` & `amqp_workers-0.1.2/amqpworker/signals/handlers/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `amqp_workers-0.1.1/amqpworker/types/registry.py` & `amqp_workers-0.1.2/amqpworker/types/registry.py`

 * *Files identical despite different names*

### Comparing `amqp_workers-0.1.1/amqpworker/typing/__init__.py` & `amqp_workers-0.1.2/amqpworker/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `amqp_workers-0.1.1/LICENSE` & `amqp_workers-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `amqp_workers-0.1.1/pyproject.toml` & `amqp_workers-0.1.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "amqp-workers"
-version = "0.1.1"
-description = ""
+version = "0.1.2"
+description = "amqp-worker is a Python-based multi-threaded RabbitMQ consumer framework"
 authors = ["JimZhang <zzl22100048@gmail.com>"]
 readme = "README.md"
 packages = [{include = "amqpworker"}]
 repository = "https://git.loom.run/Coder/amqp-worker"
 keywords = ["amqp", "rabbitmq"]
 license = "MIT"
```

### Comparing `amqp_workers-0.1.1/README.md` & `amqp_workers-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `amqp_workers-0.1.1/PKG-INFO` & `amqp_workers-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: amqp-workers
-Version: 0.1.1
-Summary: 
+Version: 0.1.2
+Summary: amqp-worker is a Python-based multi-threaded RabbitMQ consumer framework
 Home-page: https://git.loom.run/Coder/amqp-worker
 License: MIT
 Keywords: amqp,rabbitmq
 Author: JimZhang
 Author-email: zzl22100048@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

