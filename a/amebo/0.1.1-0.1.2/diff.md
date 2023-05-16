# Comparing `tmp/amebo-0.1.1.tar.gz` & `tmp/amebo-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amebo-0.1.1.tar", max compression
+gzip compressed data, was "amebo-0.1.2.tar", max compression
```

## Comparing `amebo-0.1.1.tar` & `amebo-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     6224 2023-05-14 15:13:57.906136 amebo-0.1.1/README.md
--rw-r--r--   0        0        0     2544 2023-04-05 09:41:47.811252 amebo-0.1.1/amebo.py
--rw-r--r--   0        0        0      511 2023-05-16 05:03:33.018779 amebo-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     6968 1970-01-01 00:00:00.000000 amebo-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     6314 2023-05-16 05:08:20.824236 amebo-0.1.2/README.md
+-rw-r--r--   0        0        0     2544 2023-04-05 09:41:47.811252 amebo-0.1.2/amebo.py
+-rw-r--r--   0        0        0      511 2023-05-16 05:07:01.705318 amebo-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     7058 1970-01-01 00:00:00.000000 amebo-0.1.2/PKG-INFO
```

### Comparing `amebo-0.1.1/README.md` & `amebo-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # AMEBO
 
 Amebo is the simplest pubsub server to use, deploy, understand or maintain. It was
 built to enable communication between applications i.e. microservices or
-modules (if you are using monoliths), and can
-serve as a full blown replacement for Kafka, RabbitMQ, SQS/SNS.
+modules (if you are using monoliths), and hopes to be able to serve as a small
+but capable and simpler alternative to Kafka, RabbitMQ, SQS/SNS.
+
+**STILL IN DEVELOPMENT: NOT READY FOR Production Use**
 
 &nbsp;
 
 ## How It Works
 ---
 Amebo has only 4 concepts (first class objects) to understand or master.
```

#### html2text {}

```diff
@@ -1,28 +1,29 @@
 # AMEBO Amebo is the simplest pubsub server to use, deploy, understand or
 maintain. It was built to enable communication between applications i.e.
-microservices or modules (if you are using monoliths), and can serve as a full
-blown replacement for Kafka, RabbitMQ, SQS/SNS.   ## How It Works --- Amebo has
-only 4 concepts (first class objects) to understand or master.   ### 1.
-Microservices/Modules --- These are applications or modules you register on
-amebo - they send and receive events ;-) ### 2. Events --- Something that can
-happen in an application, they are registered on Amebo by Microservices/Modules
-### 3. Actions --- A HTTP request sent to Amebo to signal an event (action on
-event) has occured. Usually has a payload that is forwarded by Amebo to all
-applications subscribed to the offending event ### 4. Subscribers --- HTTP
-endpoints registered to watch specific/particular events (by Microservices/
-Modules)   ## GETTING STARTED This assumes you have [installed](https://
-github.com/tersoo/amebo) Amebo on your machine. Amebo requires [Python3.6+]
-(https://www.python.org/downloads) ```sh # the easy path pip install amebo
-amebo --workers 2 --address 0.0.0.0:8701 # the hardway (manual installation)
-BUT not the only way... Sorry, I couldn't resist the pun ;-) git clone https://
-github.com/tersoo/amebo mv amebo /to/a/directory/of/your/choosing export
-$PATH=$PATH:/to/a/directory/of/your/choosing/amebo # add amebo location to your
-path ambeo -w 2 -a 0.0.0.0:8701 ```   ## 1st : Tell Amebo about all your
-microservices or applications --- `endpoint: /v1/microservices`
+microservices or modules (if you are using monoliths), and hopes to be able to
+serve as a small but capable and simpler alternative to Kafka, RabbitMQ, SQS/
+SNS. **STILL IN DEVELOPMENT: NOT READY FOR Production Use**   ## How It Works -
+-- Amebo has only 4 concepts (first class objects) to understand or master.  
+### 1. Microservices/Modules --- These are applications or modules you register
+on amebo - they send and receive events ;-) ### 2. Events --- Something that
+can happen in an application, they are registered on Amebo by Microservices/
+Modules ### 3. Actions --- A HTTP request sent to Amebo to signal an event
+(action on event) has occured. Usually has a payload that is forwarded by Amebo
+to all applications subscribed to the offending event ### 4. Subscribers --
+- HTTP endpoints registered to watch specific/particular events (by
+Microservices/Modules)   ## GETTING STARTED This assumes you have [installed]
+(https://github.com/tersoo/amebo) Amebo on your machine. Amebo requires
+[Python3.6+](https://www.python.org/downloads) ```sh # the easy path pip
+install amebo amebo --workers 2 --address 0.0.0.0:8701 # the hardway (manual
+installation) BUT not the only way... Sorry, I couldn't resist the pun ;-) git
+clone https://github.com/tersoo/amebo mv amebo /to/a/directory/of/your/choosing
+export $PATH=$PATH:/to/a/directory/of/your/choosing/amebo # add amebo location
+to your path ambeo -w 2 -a 0.0.0.0:8701 ```   ## 1st : Tell Amebo about all
+your microservices or applications --- `endpoint: /v1/microservices`
 Schema                                 Example Payload
 ```json { "$schema": "", "type":
 "object", "properties":
 { "microservice": {"type": "string"},  ```json { "microservice": "customers",
 "passkey": {"type": "string",          "passkey": "some-super-duper-secret-of-
 "format": "ipv4 | ipv6 | hostname |    the-module-or-microservice",
 idn-hostname"}, "location": {"type":   "location": "http://0.0.0.0:3300" } ```
```

### Comparing `amebo-0.1.1/amebo.py` & `amebo-0.1.2/amebo.py`

 * *Files identical despite different names*

### Comparing `amebo-0.1.1/PKG-INFO` & `amebo-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amebo
-Version: 0.1.1
+Version: 0.1.2
 Summary: HTTP Event Notifications Server - Asynchronous Communication Engine
 License: MIT
 Author: Tersoo
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -20,16 +20,18 @@
 Requires-Dist: uvicorn (==0.14.0)
 Description-Content-Type: text/markdown
 
 # AMEBO
 
 Amebo is the simplest pubsub server to use, deploy, understand or maintain. It was
 built to enable communication between applications i.e. microservices or
-modules (if you are using monoliths), and can
-serve as a full blown replacement for Kafka, RabbitMQ, SQS/SNS.
+modules (if you are using monoliths), and hopes to be able to serve as a small
+but capable and simpler alternative to Kafka, RabbitMQ, SQS/SNS.
+
+**STILL IN DEVELOPMENT: NOT READY FOR Production Use**
 
 &nbsp;
 
 ## How It Works
 ---
 Amebo has only 4 concepts (first class objects) to understand or master.
```

#### html2text {}

```diff
@@ -1,38 +1,39 @@
-Metadata-Version: 2.1 Name: amebo Version: 0.1.1 Summary: HTTP Event
+Metadata-Version: 2.1 Name: amebo Version: 0.1.2 Summary: HTTP Event
 Notifications Server - Asynchronous Communication Engine License: MIT Author:
 Tersoo Requires-Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: httpx
 (==0.23.3) Requires-Dist: jinja2 (==3.1.2) Requires-Dist: jsonschema (==4.17.3)
 Requires-Dist: orjson (==3.8.9) Requires-Dist: pydantic (==1.10.7) Requires-
 Dist: pyjwt (==2.7.0) Requires-Dist: routerling (==0.5.1) Requires-Dist:
 uvicorn (==0.14.0) Description-Content-Type: text/markdown # AMEBO Amebo is the
 simplest pubsub server to use, deploy, understand or maintain. It was built to
 enable communication between applications i.e. microservices or modules (if you
-are using monoliths), and can serve as a full blown replacement for Kafka,
-RabbitMQ, SQS/SNS.   ## How It Works --- Amebo has only 4 concepts (first class
-objects) to understand or master.   ### 1. Microservices/Modules --- These are
-applications or modules you register on amebo - they send and receive events ;-
-) ### 2. Events --- Something that can happen in an application, they are
-registered on Amebo by Microservices/Modules ### 3. Actions --- A HTTP request
-sent to Amebo to signal an event (action on event) has occured. Usually has a
-payload that is forwarded by Amebo to all applications subscribed to the
-offending event ### 4. Subscribers --- HTTP endpoints registered to watch
-specific/particular events (by Microservices/Modules)   ## GETTING STARTED This
-assumes you have [installed](https://github.com/tersoo/amebo) Amebo on your
-machine. Amebo requires [Python3.6+](https://www.python.org/downloads) ```sh #
-the easy path pip install amebo amebo --workers 2 --address 0.0.0.0:8701 # the
-hardway (manual installation) BUT not the only way... Sorry, I couldn't resist
-the pun ;-) git clone https://github.com/tersoo/amebo mv amebo /to/a/directory/
-of/your/choosing export $PATH=$PATH:/to/a/directory/of/your/choosing/amebo #
-add amebo location to your path ambeo -w 2 -a 0.0.0.0:8701 ```   ## 1st : Tell
-Amebo about all your microservices or applications --- `endpoint: /v1/
-microservices`
+are using monoliths), and hopes to be able to serve as a small but capable and
+simpler alternative to Kafka, RabbitMQ, SQS/SNS. **STILL IN DEVELOPMENT: NOT
+READY FOR Production Use**   ## How It Works --- Amebo has only 4 concepts
+(first class objects) to understand or master.   ### 1. Microservices/Modules -
+-- These are applications or modules you register on amebo - they send and
+receive events ;-) ### 2. Events --- Something that can happen in an
+application, they are registered on Amebo by Microservices/Modules ### 3.
+Actions --- A HTTP request sent to Amebo to signal an event (action on event)
+has occured. Usually has a payload that is forwarded by Amebo to all
+applications subscribed to the offending event ### 4. Subscribers --- HTTP
+endpoints registered to watch specific/particular events (by Microservices/
+Modules)   ## GETTING STARTED This assumes you have [installed](https://
+github.com/tersoo/amebo) Amebo on your machine. Amebo requires [Python3.6+]
+(https://www.python.org/downloads) ```sh # the easy path pip install amebo
+amebo --workers 2 --address 0.0.0.0:8701 # the hardway (manual installation)
+BUT not the only way... Sorry, I couldn't resist the pun ;-) git clone https://
+github.com/tersoo/amebo mv amebo /to/a/directory/of/your/choosing export
+$PATH=$PATH:/to/a/directory/of/your/choosing/amebo # add amebo location to your
+path ambeo -w 2 -a 0.0.0.0:8701 ```   ## 1st : Tell Amebo about all your
+microservices or applications --- `endpoint: /v1/microservices`
 Schema                                 Example Payload
 ```json { "$schema": "", "type":
 "object", "properties":
 { "microservice": {"type": "string"},  ```json { "microservice": "customers",
 "passkey": {"type": "string",          "passkey": "some-super-duper-secret-of-
 "format": "ipv4 | ipv6 | hostname |    the-module-or-microservice",
 idn-hostname"}, "location": {"type":   "location": "http://0.0.0.0:3300" } ```
```

