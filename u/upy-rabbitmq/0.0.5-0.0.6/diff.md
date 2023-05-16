# Comparing `tmp/upy-rabbitmq-0.0.5.tar.gz` & `tmp/upy-rabbitmq-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upy-rabbitmq-0.0.5.tar", last modified: Mon Mar 28 03:16:16 2022, max compression
+gzip compressed data, was "upy-rabbitmq-0.0.6.tar", last modified: Tue May 16 00:48:51 2023, max compression
```

## Comparing `upy-rabbitmq-0.0.5.tar` & `upy-rabbitmq-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 fernandocelmer  (1000) fernandocelmer  (1000)        0 2022-03-28 03:16:16.562461 upy-rabbitmq-0.0.5/
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)     2419 2022-03-28 03:16:16.562461 upy-rabbitmq-0.0.5/PKG-INFO
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)     1690 2022-03-28 03:14:22.000000 upy-rabbitmq-0.0.5/README.md
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)      138 2022-03-28 03:16:16.562461 upy-rabbitmq-0.0.5/setup.cfg
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)     1152 2022-03-28 03:14:03.000000 upy-rabbitmq-0.0.5/setup.py
-drwxrwxr-x   0 fernandocelmer  (1000) fernandocelmer  (1000)        0 2022-03-28 03:16:16.562461 upy-rabbitmq-0.0.5/upy_rabbitmq/
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)       97 2022-03-28 03:15:34.000000 upy-rabbitmq-0.0.5/upy_rabbitmq/__init__.py
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)     1137 2022-03-28 03:14:00.000000 upy-rabbitmq-0.0.5/upy_rabbitmq/base.py
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)      648 2022-03-28 03:14:00.000000 upy-rabbitmq-0.0.5/upy_rabbitmq/client.py
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)      522 2022-03-28 03:14:00.000000 upy-rabbitmq-0.0.5/upy_rabbitmq/worker.py
-drwxrwxr-x   0 fernandocelmer  (1000) fernandocelmer  (1000)        0 2022-03-28 03:16:16.562461 upy-rabbitmq-0.0.5/upy_rabbitmq.egg-info/
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)     2419 2022-03-28 03:16:16.000000 upy-rabbitmq-0.0.5/upy_rabbitmq.egg-info/PKG-INFO
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)      334 2022-03-28 03:16:16.000000 upy-rabbitmq-0.0.5/upy_rabbitmq.egg-info/SOURCES.txt
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)        1 2022-03-28 03:16:16.000000 upy-rabbitmq-0.0.5/upy_rabbitmq.egg-info/dependency_links.txt
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)        1 2022-01-08 05:41:39.000000 upy-rabbitmq-0.0.5/upy_rabbitmq.egg-info/not-zip-safe
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)       12 2022-03-28 03:16:16.000000 upy-rabbitmq-0.0.5/upy_rabbitmq.egg-info/requires.txt
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)       13 2022-03-28 03:16:16.000000 upy-rabbitmq-0.0.5/upy_rabbitmq.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:48:51.550221 upy-rabbitmq-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-16 00:48:51.554221 upy-rabbitmq-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-05-16 00:48:30.000000 upy-rabbitmq-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-16 00:48:51.554221 upy-rabbitmq-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-16 00:48:30.000000 upy-rabbitmq-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:48:51.550221 upy-rabbitmq-0.0.6/upy_rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-16 00:48:30.000000 upy-rabbitmq-0.0.6/upy_rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-16 00:48:30.000000 upy-rabbitmq-0.0.6/upy_rabbitmq/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-16 00:48:30.000000 upy-rabbitmq-0.0.6/upy_rabbitmq/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-16 00:48:30.000000 upy-rabbitmq-0.0.6/upy_rabbitmq/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-16 00:48:30.000000 upy-rabbitmq-0.0.6/upy_rabbitmq/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:48:51.550221 upy-rabbitmq-0.0.6/upy_rabbitmq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-16 00:48:51.000000 upy-rabbitmq-0.0.6/upy_rabbitmq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-16 00:48:51.000000 upy-rabbitmq-0.0.6/upy_rabbitmq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 00:48:51.000000 upy-rabbitmq-0.0.6/upy_rabbitmq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 00:48:51.000000 upy-rabbitmq-0.0.6/upy_rabbitmq.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-16 00:48:51.000000 upy-rabbitmq-0.0.6/upy_rabbitmq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-16 00:48:51.000000 upy-rabbitmq-0.0.6/upy_rabbitmq.egg-info/top_level.txt
```

### Comparing `upy-rabbitmq-0.0.5/PKG-INFO` & `upy-rabbitmq-0.0.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,94 +1,116 @@
 Metadata-Version: 2.1
 Name: upy-rabbitmq
-Version: 0.0.5
+Version: 0.0.6
 Summary: Basic RabbitMQ
 Home-page: https://github.com/UpyExplorer/upy-rabbitmq
 Author: Fernando Celmer
 Author-email: email@fernandocelmer.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # upy-rabbitmq
 
+![GitHub Org's stars](https://img.shields.io/github/stars/UpyExplorer?label=LinuxProfile&style=flat-square)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/upy-rabbitmq)
 ![PyPI - License](https://img.shields.io/pypi/l/upy-rabbitmq)
 ![PyPI](https://img.shields.io/pypi/v/upy-rabbitmq)
 ![GitHub last commit](https://img.shields.io/github/last-commit/UpyExplorer/upy-rabbitmq)
-![GitHub followers](https://img.shields.io/github/followers/UpyExplorer?label=UpyExplorer&style=social)
-<br>
+
+---
+
+- **Documentation**: [https://github.com/UpyExplorer/upy-rabbitmq](https://github.com/UpyExplorer/upy-rabbitmq)
+- **Source Code**: [https://github.com/UpyExplorer/upy-rabbitmq](https://github.com/UpyExplorer/upy-rabbitmq)
+
+---
 
 ## How to install?
-```python
 
+```python
 pip install upy-rabbitmq
-
 ```
-<!-- CONFIG -->
+
 ## Config
 
 Add an environment variation called **RABBITMQ_URL** in your project's .env file.
 
 ```
-
 RABBITMQ_URL=amqp://user:password@remote.server.com:port//vhost
+```
+
+## Callback Class
+> callback.py
+
+```python
+
+import time
+from upy_rabbitmq.callback import CallbackProcess
 
+class MyCallBack(CallbackProcess):
+
+    def process(self):
+        time.sleep(5)
+        print(self.body.decode())
 ```
+
 ## Start Queue
+> worker.py
 
 ```python
 
 from upy_rabbitmq.worker import UpyMQWorker
 
 worker = UpyMQWorker()
 worker.start_queue(
     key="key",
-    callback=callback
+    callback=MyCallBack
 )
 ```
+
 ## New Task
+> client.py
 
 ```python
-
-from upy_rabbitmq.worker import UpyMQClient
+from upy_rabbitmq.client import UpyMQClient
 
 client = UpyMQClient()
 client.new_task(
     key="key",
     message="Hello"
 )
 ```
-<!-- CONTRIBUTING -->
+
 ## Contributing
 
 Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
 
 1. Fork the Project
 2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
 3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
 4. Push to the Branch (`git push origin feature/AmazingFeature`)
 5. Open a Pull Request
 
-<!-- LICENSE -->
-## License
-
-Distributed under the MIT License. See `LICENSE` for more information.
-
-<!-- CONTACT -->
-## Contact
+## Commit Style
 
-Fernando Celmer- email@fernandocelmer.com
-
-Project Link: [https://github.com/UpyExplorer/upy-rabbitmq](https://github.com/UpyExplorer/upy-rabbitmq)
+- ⚙️ FEATURE
+- 📝 PEP8
+- 📌 ISSUE
+- 🪲 BUG
+- 📘 DOCS
+- 📦 PyPI
+- ❤️️ TEST
+- ⬆️ CI/CD
+- ⚠️ SECURITY
 
+## License
 
+Distributed under the MIT License. See `LICENSE` for more information.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `upy-rabbitmq-0.0.5/README.md` & `upy-rabbitmq-0.0.6/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,71 +1,96 @@
 # upy-rabbitmq
 
+![GitHub Org's stars](https://img.shields.io/github/stars/UpyExplorer?label=LinuxProfile&style=flat-square)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/upy-rabbitmq)
 ![PyPI - License](https://img.shields.io/pypi/l/upy-rabbitmq)
 ![PyPI](https://img.shields.io/pypi/v/upy-rabbitmq)
 ![GitHub last commit](https://img.shields.io/github/last-commit/UpyExplorer/upy-rabbitmq)
-![GitHub followers](https://img.shields.io/github/followers/UpyExplorer?label=UpyExplorer&style=social)
-<br>
+
+---
+
+- **Documentation**: [https://github.com/UpyExplorer/upy-rabbitmq](https://github.com/UpyExplorer/upy-rabbitmq)
+- **Source Code**: [https://github.com/UpyExplorer/upy-rabbitmq](https://github.com/UpyExplorer/upy-rabbitmq)
+
+---
 
 ## How to install?
-```python
 
+```python
 pip install upy-rabbitmq
-
 ```
-<!-- CONFIG -->
+
 ## Config
 
 Add an environment variation called **RABBITMQ_URL** in your project's .env file.
 
 ```
-
 RABBITMQ_URL=amqp://user:password@remote.server.com:port//vhost
+```
+
+## Callback Class
+> callback.py
+
+```python
 
+import time
+from upy_rabbitmq.callback import CallbackProcess
+
+class MyCallBack(CallbackProcess):
+
+    def process(self):
+        time.sleep(5)
+        print(self.body.decode())
 ```
+
 ## Start Queue
+> worker.py
 
 ```python
 
 from upy_rabbitmq.worker import UpyMQWorker
 
 worker = UpyMQWorker()
 worker.start_queue(
     key="key",
-    callback=callback
+    callback=MyCallBack
 )
 ```
+
 ## New Task
+> client.py
 
 ```python
-
-from upy_rabbitmq.worker import UpyMQClient
+from upy_rabbitmq.client import UpyMQClient
 
 client = UpyMQClient()
 client.new_task(
     key="key",
     message="Hello"
 )
 ```
-<!-- CONTRIBUTING -->
+
 ## Contributing
 
 Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
 
 1. Fork the Project
 2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
 3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
 4. Push to the Branch (`git push origin feature/AmazingFeature`)
 5. Open a Pull Request
 
-<!-- LICENSE -->
-## License
-
-Distributed under the MIT License. See `LICENSE` for more information.
+## Commit Style
 
-<!-- CONTACT -->
-## Contact
+- ⚙️ FEATURE
+- 📝 PEP8
+- 📌 ISSUE
+- 🪲 BUG
+- 📘 DOCS
+- 📦 PyPI
+- ❤️️ TEST
+- ⬆️ CI/CD
+- ⚠️ SECURITY
 
-Fernando Celmer- email@fernandocelmer.com
+## License
 
-Project Link: [https://github.com/UpyExplorer/upy-rabbitmq](https://github.com/UpyExplorer/upy-rabbitmq)
+Distributed under the MIT License. See `LICENSE` for more information.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `upy-rabbitmq-0.0.5/setup.py` & `upy-rabbitmq-0.0.6/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-import setuptools
+from setuptools import setup
 import upy_rabbitmq
 
 version = upy_rabbitmq.__version__
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-setuptools.setup(
+
+setup(
     name="upy-rabbitmq",
     version=version,
     author="Fernando Celmer",
     author_email="email@fernandocelmer.com",
     description="Basic RabbitMQ",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/UpyExplorer/upy-rabbitmq",
     packages=[
         'upy_rabbitmq',
     ],
     include_package_data=True,
     install_requires=[
-        'pika>=1.2.0'
+        'pika==1.3.1',
+        'python-dotenv==1.0.0'
     ],
     classifiers=[
         "Operating System :: OS Independent",
         "License :: OSI Approved :: MIT License",
         'Intended Audience :: Developers',
         'Natural Language :: English',
-        "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     python_requires=">=3.6",
     zip_safe=False
 )
```

### Comparing `upy-rabbitmq-0.0.5/upy_rabbitmq/client.py` & `upy-rabbitmq-0.0.6/upy_rabbitmq/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 """
 Module Client
 """
 
 import pika
 from upy_rabbitmq.base import UpyRabbitMQ
 
+
 class UpyMQClient(UpyRabbitMQ):
     """Class responsible for producing new messages
     """
 
-    def new_task(self, key, message, exchange=None):
+    def new_task(self, key: str, message: str, exchange: str = ""):
         """New Task
         """
-        exchange = exchange or ""
         channel = self.channel_initialize()
 
         channel.queue_declare(queue=key, durable=True)
         channel.basic_publish(
             exchange=exchange,
             routing_key=key,
             body=message,
```

### Comparing `upy-rabbitmq-0.0.5/upy_rabbitmq/worker.py` & `upy-rabbitmq-0.0.6/upy_rabbitmq/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
 Module Worker
 """
 
 from upy_rabbitmq.base import UpyRabbitMQ
 
+
 class UpyMQWorker(UpyRabbitMQ):
     """Class responsible for orchestrating and initiating work processes
     """
 
     def start_queue(self, key, callback):
         """Start Queue
         """
```

### Comparing `upy-rabbitmq-0.0.5/upy_rabbitmq.egg-info/PKG-INFO` & `upy-rabbitmq-0.0.6/upy_rabbitmq.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,94 +1,116 @@
 Metadata-Version: 2.1
 Name: upy-rabbitmq
-Version: 0.0.5
+Version: 0.0.6
 Summary: Basic RabbitMQ
 Home-page: https://github.com/UpyExplorer/upy-rabbitmq
 Author: Fernando Celmer
 Author-email: email@fernandocelmer.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # upy-rabbitmq
 
+![GitHub Org's stars](https://img.shields.io/github/stars/UpyExplorer?label=LinuxProfile&style=flat-square)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/upy-rabbitmq)
 ![PyPI - License](https://img.shields.io/pypi/l/upy-rabbitmq)
 ![PyPI](https://img.shields.io/pypi/v/upy-rabbitmq)
 ![GitHub last commit](https://img.shields.io/github/last-commit/UpyExplorer/upy-rabbitmq)
-![GitHub followers](https://img.shields.io/github/followers/UpyExplorer?label=UpyExplorer&style=social)
-<br>
+
+---
+
+- **Documentation**: [https://github.com/UpyExplorer/upy-rabbitmq](https://github.com/UpyExplorer/upy-rabbitmq)
+- **Source Code**: [https://github.com/UpyExplorer/upy-rabbitmq](https://github.com/UpyExplorer/upy-rabbitmq)
+
+---
 
 ## How to install?
-```python
 
+```python
 pip install upy-rabbitmq
-
 ```
-<!-- CONFIG -->
+
 ## Config
 
 Add an environment variation called **RABBITMQ_URL** in your project's .env file.
 
 ```
-
 RABBITMQ_URL=amqp://user:password@remote.server.com:port//vhost
+```
+
+## Callback Class
+> callback.py
+
+```python
+
+import time
+from upy_rabbitmq.callback import CallbackProcess
 
+class MyCallBack(CallbackProcess):
+
+    def process(self):
+        time.sleep(5)
+        print(self.body.decode())
 ```
+
 ## Start Queue
+> worker.py
 
 ```python
 
 from upy_rabbitmq.worker import UpyMQWorker
 
 worker = UpyMQWorker()
 worker.start_queue(
     key="key",
-    callback=callback
+    callback=MyCallBack
 )
 ```
+
 ## New Task
+> client.py
 
 ```python
-
-from upy_rabbitmq.worker import UpyMQClient
+from upy_rabbitmq.client import UpyMQClient
 
 client = UpyMQClient()
 client.new_task(
     key="key",
     message="Hello"
 )
 ```
-<!-- CONTRIBUTING -->
+
 ## Contributing
 
 Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
 
 1. Fork the Project
 2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
 3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
 4. Push to the Branch (`git push origin feature/AmazingFeature`)
 5. Open a Pull Request
 
-<!-- LICENSE -->
-## License
-
-Distributed under the MIT License. See `LICENSE` for more information.
-
-<!-- CONTACT -->
-## Contact
+## Commit Style
 
-Fernando Celmer- email@fernandocelmer.com
-
-Project Link: [https://github.com/UpyExplorer/upy-rabbitmq](https://github.com/UpyExplorer/upy-rabbitmq)
+- ⚙️ FEATURE
+- 📝 PEP8
+- 📌 ISSUE
+- 🪲 BUG
+- 📘 DOCS
+- 📦 PyPI
+- ❤️️ TEST
+- ⬆️ CI/CD
+- ⚠️ SECURITY
 
+## License
 
+Distributed under the MIT License. See `LICENSE` for more information.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

