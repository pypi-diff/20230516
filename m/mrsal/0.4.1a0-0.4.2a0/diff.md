# Comparing `tmp/mrsal-0.4.1a0.tar.gz` & `tmp/mrsal-0.4.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrsal-0.4.1a0.tar", max compression
+gzip compressed data, was "mrsal-0.4.2a0.tar", max compression
```

## Comparing `mrsal-0.4.1a0.tar` & `mrsal-0.4.2a0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35148 2022-09-08 10:55:29.050700 mrsal-0.4.1a0/LICENSE.txt
--rw-r--r--   0        0        0     8649 2023-04-26 07:22:55.916971 mrsal-0.4.1a0/README.md
--rw-r--r--   0        0        0        0 2022-08-17 10:39:13.102254 mrsal-0.4.1a0/mrsal/__init__.py
--rw-r--r--   0        0        0        0 2022-08-17 10:39:13.102254 mrsal-0.4.1a0/mrsal/config/__init__.py
--rw-r--r--   0        0        0     1175 2023-02-16 07:01:55.359449 mrsal-0.4.1a0/mrsal/config/config.py
--rw-r--r--   0        0        0      286 2023-04-26 07:24:07.167406 mrsal-0.4.1a0/mrsal/config/exceptions.py
--rw-r--r--   0        0        0     2431 2022-08-17 10:39:13.102254 mrsal-0.4.1a0/mrsal/config/logging.py
--rw-r--r--   0        0        0    30718 2023-04-26 09:46:44.007212 mrsal-0.4.1a0/mrsal/mrsal.py
--rw-r--r--   0        0        0      666 2023-04-26 09:54:36.335948 mrsal-0.4.1a0/pyproject.toml
--rw-r--r--   0        0        0     9371 1970-01-01 00:00:00.000000 mrsal-0.4.1a0/PKG-INFO
+-rw-r--r--   0        0        0    35148 2022-09-08 10:55:29.050700 mrsal-0.4.2a0/LICENSE.txt
+-rw-r--r--   0        0        0     8728 2023-04-26 10:08:10.924995 mrsal-0.4.2a0/README.md
+-rw-r--r--   0        0        0        0 2022-08-17 10:39:13.102254 mrsal-0.4.2a0/mrsal/__init__.py
+-rw-r--r--   0        0        0        0 2022-08-17 10:39:13.102254 mrsal-0.4.2a0/mrsal/config/__init__.py
+-rw-r--r--   0        0        0     1175 2023-02-16 07:01:55.359449 mrsal-0.4.2a0/mrsal/config/config.py
+-rw-r--r--   0        0        0      286 2023-04-26 07:24:07.167406 mrsal-0.4.2a0/mrsal/config/exceptions.py
+-rw-r--r--   0        0        0     2431 2022-08-17 10:39:13.102254 mrsal-0.4.2a0/mrsal/config/logging.py
+-rw-r--r--   0        0        0    30718 2023-04-26 09:46:44.007212 mrsal-0.4.2a0/mrsal/mrsal.py
+-rw-r--r--   0        0        0      666 2023-04-26 10:09:06.743901 mrsal-0.4.2a0/pyproject.toml
+-rw-r--r--   0        0        0     9450 1970-01-01 00:00:00.000000 mrsal-0.4.2a0/PKG-INFO
```

### Comparing `mrsal-0.4.1a0/LICENSE.txt` & `mrsal-0.4.2a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mrsal-0.4.1a0/README.md` & `mrsal-0.4.2a0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -135,14 +135,15 @@
 
 mrsal.start_consumer(
         queue='friendship_queue',
         callback=consumer_callback_with_delivery_info,
         callback_args=(test_config.HOST, 'friendship_queue'),
         inactivity_timeout=1,
         requeue=False,
+        fast_setup=True,
         callback_with_delivery_info=True
     )
 ```
 
 Done! Your first message of friendship has been sent to the friendship queue on the exchange of friendship.
 
 
@@ -184,14 +185,15 @@
     # Start concurrent consumers
     mrsal.start_concurrence_consumer(total_threads=NUM_THREADS, queue=QUEUE_EMERGENCY,
                                      callback=consumer_callback_with_delivery_info,
                                      callback_args=(test_config.HOST, QUEUE_EMERGENCY),
                                      exchange=EXCHANGE, exchange_type=EXCHANGE_TYPE,
                                      routing_key=ROUTING_KEY,
                                      inactivity_timeout=INACTIVITY_TIMEOUT,
+                                     fast_setup=True,
                                      callback_with_delivery_info=True)
     print(f"Concurrent consumers are done")
 
     mrsal.close_connection()
 
 def consumer_callback_with_delivery_info(host_param: str, queue_param: str, method_frame: pika.spec.Basic.Deliver, properties: pika.spec.BasicProperties, message_param: str):
     time.sleep(5)
```

### Comparing `mrsal-0.4.1a0/mrsal/config/config.py` & `mrsal-0.4.2a0/mrsal/config/config.py`

 * *Files identical despite different names*

### Comparing `mrsal-0.4.1a0/mrsal/config/logging.py` & `mrsal-0.4.2a0/mrsal/config/logging.py`

 * *Files identical despite different names*

### Comparing `mrsal-0.4.1a0/mrsal/mrsal.py` & `mrsal-0.4.2a0/mrsal/mrsal.py`

 * *Files identical despite different names*

### Comparing `mrsal-0.4.1a0/pyproject.toml` & `mrsal-0.4.2a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mrsal"
-version = "0.4.1-alpha"
+version = "0.4.2-alpha"
 description = "Mrsal is a simple to use message broker abstraction on top of RabbitMQ and Pika."
 authors = ["Raafat <rafatzahran90@gmail.com>", "Jon E Nesvold <jnesvold@pm.me>"]
 maintainers = ["Raafat <rafatzahran90@gmail.com>", "Jon E Nesvold <jnesvold@pm.me>"]
 keywords = ["RabbitMQ", "Pika", "Mrsal"]
 readme = "README.md"
 license = ""
```

### Comparing `mrsal-0.4.1a0/PKG-INFO` & `mrsal-0.4.2a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrsal
-Version: 0.4.1a0
+Version: 0.4.2a0
 Summary: Mrsal is a simple to use message broker abstraction on top of RabbitMQ and Pika.
 Keywords: RabbitMQ,Pika,Mrsal
 Author: Raafat
 Author-email: rafatzahran90@gmail.com
 Maintainer: Raafat
 Maintainer-email: rafatzahran90@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -155,14 +155,15 @@
 
 mrsal.start_consumer(
         queue='friendship_queue',
         callback=consumer_callback_with_delivery_info,
         callback_args=(test_config.HOST, 'friendship_queue'),
         inactivity_timeout=1,
         requeue=False,
+        fast_setup=True,
         callback_with_delivery_info=True
     )
 ```
 
 Done! Your first message of friendship has been sent to the friendship queue on the exchange of friendship.
 
 
@@ -204,14 +205,15 @@
     # Start concurrent consumers
     mrsal.start_concurrence_consumer(total_threads=NUM_THREADS, queue=QUEUE_EMERGENCY,
                                      callback=consumer_callback_with_delivery_info,
                                      callback_args=(test_config.HOST, QUEUE_EMERGENCY),
                                      exchange=EXCHANGE, exchange_type=EXCHANGE_TYPE,
                                      routing_key=ROUTING_KEY,
                                      inactivity_timeout=INACTIVITY_TIMEOUT,
+                                     fast_setup=True,
                                      callback_with_delivery_info=True)
     print(f"Concurrent consumers are done")
 
     mrsal.close_connection()
 
 def consumer_callback_with_delivery_info(host_param: str, queue_param: str, method_frame: pika.spec.Basic.Deliver, properties: pika.spec.BasicProperties, message_param: str):
     time.sleep(5)
```

