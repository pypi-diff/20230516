# Comparing `tmp/sinetstream-1.7.0.tar.gz` & `tmp/sinetstream-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinetstream-1.7.0.tar", last modified: Fri Sep 16 07:09:24 2022, max compression
+gzip compressed data, was "sinetstream-1.8.0.tar", last modified: Tue May 16 06:32:29 2023, max compression
```

## Comparing `sinetstream-1.7.0.tar` & `sinetstream-1.8.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2022-09-16 07:09:24.825436 sinetstream-1.7.0/
--rw-rw-r--   0 koie      (1004) koie      (1004)     3625 2022-09-16 07:09:24.825436 sinetstream-1.7.0/PKG-INFO
--rw-rw-r--   0 koie      (1004) koie      (1004)     2446 2022-09-15 07:30:59.000000 sinetstream-1.7.0/README.md
--rw-rw-r--   0 koie      (1004) koie      (1004)     1428 2022-09-16 07:09:24.825436 sinetstream-1.7.0/setup.cfg
--rw-rw-r--   0 koie      (1004) koie      (1004)       39 2022-09-15 07:30:59.000000 sinetstream-1.7.0/setup.py
-drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2022-09-16 07:09:24.813436 sinetstream-1.7.0/src/
-drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2022-09-16 07:09:24.821436 sinetstream-1.7.0/src/sinetstream/
--rw-rw-r--   0 koie      (1004) koie      (1004)     1686 2022-09-15 07:30:59.000000 sinetstream-1.7.0/src/sinetstream/__init__.py
--rw-rw-r--   0 koie      (1004) koie      (1004)     1169 2022-09-15 07:30:59.000000 sinetstream-1.7.0/src/sinetstream/__main__.py
--rw-rw-r--   0 koie      (1004) koie      (1004)    28081 2022-09-15 07:30:59.000000 sinetstream-1.7.0/src/sinetstream/api.py
--rw-rw-r--   0 koie      (1004) koie      (1004)     2759 2022-09-15 07:30:59.000000 sinetstream-1.7.0/src/sinetstream/compression.py
--rw-rw-r--   0 koie      (1004) koie      (1004)    11484 2022-09-15 07:30:59.000000 sinetstream-1.7.0/src/sinetstream/config_client.py
--rw-rw-r--   0 koie      (1004) koie      (1004)     9012 2022-09-15 07:30:59.000000 sinetstream-1.7.0/src/sinetstream/configs.py
--rw-rw-r--   0 koie      (1004) koie      (1004)    11450 2022-09-15 07:30:59.000000 sinetstream-1.7.0/src/sinetstream/crypto.py
--rw-rw-r--   0 koie      (1004) koie      (1004)     1403 2022-09-15 07:30:59.000000 sinetstream-1.7.0/src/sinetstream/error.py
--rw-rw-r--   0 koie      (1004) koie      (1004)     3215 2022-09-15 07:30:59.000000 sinetstream-1.7.0/src/sinetstream/marshal.py
--rw-rw-r--   0 koie      (1004) koie      (1004)     4488 2022-09-15 07:30:59.000000 sinetstream-1.7.0/src/sinetstream/spi.py
--rw-rw-r--   0 koie      (1004) koie      (1004)     2502 2022-09-15 07:30:59.000000 sinetstream-1.7.0/src/sinetstream/utils.py
--rw-rw-r--   0 koie      (1004) koie      (1004)     1741 2022-09-15 07:30:59.000000 sinetstream-1.7.0/src/sinetstream/value_type.py
-drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2022-09-16 07:09:24.821436 sinetstream-1.7.0/src/sinetstream.egg-info/
--rw-rw-r--   0 koie      (1004) koie      (1004)     3625 2022-09-16 07:09:24.000000 sinetstream-1.7.0/src/sinetstream.egg-info/PKG-INFO
--rw-rw-r--   0 koie      (1004) koie      (1004)      586 2022-09-16 07:09:24.000000 sinetstream-1.7.0/src/sinetstream.egg-info/SOURCES.txt
--rw-rw-r--   0 koie      (1004) koie      (1004)        1 2022-09-16 07:09:24.000000 sinetstream-1.7.0/src/sinetstream.egg-info/dependency_links.txt
--rw-rw-r--   0 koie      (1004) koie      (1004)        1 2022-09-16 07:07:20.000000 sinetstream-1.7.0/src/sinetstream.egg-info/not-zip-safe
--rw-rw-r--   0 koie      (1004) koie      (1004)       61 2022-09-16 07:09:24.000000 sinetstream-1.7.0/src/sinetstream.egg-info/requires.txt
--rw-rw-r--   0 koie      (1004) koie      (1004)       12 2022-09-16 07:09:24.000000 sinetstream-1.7.0/src/sinetstream.egg-info/top_level.txt
+drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-05-16 06:32:29.654585 sinetstream-1.8.0/
+-rw-rw-r--   0 koie      (1004) koie      (1004)     2914 2023-05-16 06:32:29.654585 sinetstream-1.8.0/PKG-INFO
+-rw-rw-r--   0 koie      (1004) koie      (1004)     2446 2023-01-12 00:12:25.000000 sinetstream-1.8.0/README.md
+-rw-rw-r--   0 koie      (1004) koie      (1004)     1435 2023-05-16 06:32:29.654585 sinetstream-1.8.0/setup.cfg
+-rw-rw-r--   0 koie      (1004) koie      (1004)       39 2023-01-12 00:12:25.000000 sinetstream-1.8.0/setup.py
+drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-05-16 06:32:29.630585 sinetstream-1.8.0/src/
+drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-05-16 06:32:29.642585 sinetstream-1.8.0/src/sinetstream/
+-rw-rw-r--   0 koie      (1004) koie      (1004)     1686 2023-01-12 00:12:25.000000 sinetstream-1.8.0/src/sinetstream/__init__.py
+-rw-rw-r--   0 koie      (1004) koie      (1004)     1169 2023-01-12 00:12:25.000000 sinetstream-1.8.0/src/sinetstream/__main__.py
+-rw-rw-r--   0 koie      (1004) koie      (1004)    28081 2023-01-12 00:12:25.000000 sinetstream-1.8.0/src/sinetstream/api.py
+-rw-rw-r--   0 koie      (1004) koie      (1004)     2759 2023-01-12 00:12:25.000000 sinetstream-1.8.0/src/sinetstream/compression.py
+-rw-rw-r--   0 koie      (1004) koie      (1004)    11484 2023-05-16 06:28:20.000000 sinetstream-1.8.0/src/sinetstream/config_client.py
+-rw-rw-r--   0 koie      (1004) koie      (1004)     9012 2023-05-16 06:28:20.000000 sinetstream-1.8.0/src/sinetstream/configs.py
+-rw-rw-r--   0 koie      (1004) koie      (1004)    11450 2023-01-12 00:12:25.000000 sinetstream-1.8.0/src/sinetstream/crypto.py
+-rw-rw-r--   0 koie      (1004) koie      (1004)     1403 2023-01-12 00:12:25.000000 sinetstream-1.8.0/src/sinetstream/error.py
+-rw-rw-r--   0 koie      (1004) koie      (1004)     3215 2023-01-12 00:12:25.000000 sinetstream-1.8.0/src/sinetstream/marshal.py
+-rw-rw-r--   0 koie      (1004) koie      (1004)     4488 2023-01-12 00:12:25.000000 sinetstream-1.8.0/src/sinetstream/spi.py
+-rw-rw-r--   0 koie      (1004) koie      (1004)     2502 2023-01-12 00:12:25.000000 sinetstream-1.8.0/src/sinetstream/utils.py
+-rw-rw-r--   0 koie      (1004) koie      (1004)     1741 2023-01-12 00:12:25.000000 sinetstream-1.8.0/src/sinetstream/value_type.py
+drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-05-16 06:32:29.654585 sinetstream-1.8.0/src/sinetstream.egg-info/
+-rw-rw-r--   0 koie      (1004) koie      (1004)     2914 2023-05-16 06:32:28.000000 sinetstream-1.8.0/src/sinetstream.egg-info/PKG-INFO
+-rw-rw-r--   0 koie      (1004) koie      (1004)      586 2023-05-16 06:32:29.000000 sinetstream-1.8.0/src/sinetstream.egg-info/SOURCES.txt
+-rw-rw-r--   0 koie      (1004) koie      (1004)        1 2023-05-16 06:32:28.000000 sinetstream-1.8.0/src/sinetstream.egg-info/dependency_links.txt
+-rw-rw-r--   0 koie      (1004) koie      (1004)        1 2023-01-12 00:15:50.000000 sinetstream-1.8.0/src/sinetstream.egg-info/not-zip-safe
+-rw-rw-r--   0 koie      (1004) koie      (1004)       61 2023-05-16 06:32:28.000000 sinetstream-1.8.0/src/sinetstream.egg-info/requires.txt
+-rw-rw-r--   0 koie      (1004) koie      (1004)       12 2023-05-16 06:32:28.000000 sinetstream-1.8.0/src/sinetstream.egg-info/top_level.txt
```

### Comparing `sinetstream-1.7.0/PKG-INFO` & `sinetstream-1.8.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,101 +1,100 @@
 Metadata-Version: 2.1
 Name: sinetstream
-Version: 1.7.0
+Version: 1.8.0
 Summary: Library for operating messaging systems such as Apache Kafka and MQTT with the same API.
 Home-page: https://github.com/nii-gakunin-cloud/sinetstream
 License: Apache License, Version 2.0
-Description: <!--
-        Copyright (C) 2020 National Institute of Informatics
-        
-        Licensed to the Apache Software Foundation (ASF) under one
-        or more contributor license agreements.  See the NOTICE file
-        distributed with this work for additional information
-        regarding copyright ownership.  The ASF licenses this file
-        to you under the Apache License, Version 2.0 (the
-        "License"); you may not use this file except in compliance
-        with the License.  You may obtain a copy of the License at
-        
-          http://www.apache.org/licenses/LICENSE-2.0
-        
-        Unless required by applicable law or agreed to in writing,
-        software distributed under the License is distributed on an
-        "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
-        KIND, either express or implied.  See the License for the
-        specific language governing permissions and limitations
-        under the License.
-        -->
-        
-        [日本語](README.md)
-        
-        # SINETStream python
-        
-        ## Directory structure
-        
-        * src/
-            * Implementation of SINETStream for Python
-        * tests/
-            * Unit test
-        * sample/
-            * Sample program
-        * plugins/
-            * broker/
-                * kafka/
-                    * Kafka Plugin for SINETStream
-                * mqtt
-                    * MQTT Plugin for SINETStream
-            * value_type/
-                * image/
-                    * Plugin for handling image as message
-        * README.md
-        
-        ## Build procedure
-        
-        Execute the following command to build the SINETStream TAR file.
-        
-        ```
-        $ python3 setup.py bdist_wheel
-        $ cd plugins/broker/kafka
-        $ python3 setup.py bdist_wheel
-        $ cd ../mqtt
-        $ python3 setup.py bdist_wheel
-        $ cd ../../value_type/image
-        $ python3 setup.py bdist_wheel
-        ```
-        
-        If the build is successful, the following WHL file will be created.
-        
-        ```
-        ./dist/sinetstream-1.1.0-py3-none-any.whl
-        ./plugins/broker/kafka/dist/sinetstream_kafka-1.1.0-py3-none-any.whl
-        ./plugins/broker/mqtt/dist/sinetstream_mqtt-1.1.0-py3-none-any.whl
-        ./plugins/value_type/image/dist/sinetstream_type_image-1.1.0-py3-none-any.whl
-        ```
-        
-        ## Install
-        
-        You can also use the packages registered in pypi.
-        
-        ```
-        pip3 install --user sinetstream-kafka sinetstream-mqtt
-        ```
-        
-        If you want to handle image as message, please install the image plugin as follows.
-        
-        ```
-        pip3 install --user sinetstream-type-image
-        ```
-        
-        ## Dependent libraries
-        
-        * [kafka-python](https://kafka-python.readthedocs.io/en/master/)
-        * [mqtt client](https://www.eclipse.org/paho/clients/python/docs/)
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Japanese
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+
+<!--
+Copyright (C) 2020 National Institute of Informatics
+
+Licensed to the Apache Software Foundation (ASF) under one
+or more contributor license agreements.  See the NOTICE file
+distributed with this work for additional information
+regarding copyright ownership.  The ASF licenses this file
+to you under the Apache License, Version 2.0 (the
+"License"); you may not use this file except in compliance
+with the License.  You may obtain a copy of the License at
+
+  http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing,
+software distributed under the License is distributed on an
+"AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+KIND, either express or implied.  See the License for the
+specific language governing permissions and limitations
+under the License.
+-->
+
+[日本語](README.md)
+
+# SINETStream python
+
+## Directory structure
+
+* src/
+    * Implementation of SINETStream for Python
+* tests/
+    * Unit test
+* sample/
+    * Sample program
+* plugins/
+    * broker/
+        * kafka/
+            * Kafka Plugin for SINETStream
+        * mqtt
+            * MQTT Plugin for SINETStream
+    * value_type/
+        * image/
+            * Plugin for handling image as message
+* README.md
+
+## Build procedure
+
+Execute the following command to build the SINETStream TAR file.
+
+```
+$ python3 setup.py bdist_wheel
+$ cd plugins/broker/kafka
+$ python3 setup.py bdist_wheel
+$ cd ../mqtt
+$ python3 setup.py bdist_wheel
+$ cd ../../value_type/image
+$ python3 setup.py bdist_wheel
+```
+
+If the build is successful, the following WHL file will be created.
+
+```
+./dist/sinetstream-1.1.0-py3-none-any.whl
+./plugins/broker/kafka/dist/sinetstream_kafka-1.1.0-py3-none-any.whl
+./plugins/broker/mqtt/dist/sinetstream_mqtt-1.1.0-py3-none-any.whl
+./plugins/value_type/image/dist/sinetstream_type_image-1.1.0-py3-none-any.whl
+```
+
+## Install
+
+You can also use the packages registered in pypi.
+
+```
+pip3 install --user sinetstream-kafka sinetstream-mqtt
+```
+
+If you want to handle image as message, please install the image plugin as follows.
+
+```
+pip3 install --user sinetstream-type-image
+```
+
+## Dependent libraries
+
+* [kafka-python](https://kafka-python.readthedocs.io/en/master/)
+* [mqtt client](https://www.eclipse.org/paho/clients/python/docs/)
```

### Comparing `sinetstream-1.7.0/README.md` & `sinetstream-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `sinetstream-1.7.0/setup.cfg` & `sinetstream-1.8.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sinetstream
-version = 1.7.0
+version = 1.8.0
 description = Library for operating messaging systems such as Apache Kafka and MQTT with the same API.
 long_description = file: README.en.md
 long_description_content_type = text/markdown
 url = https://github.com/nii-gakunin-cloud/sinetstream
 license = Apache License, Version 2.0
 license_files = 
 	../LICENSE
@@ -29,15 +29,15 @@
 	requests
 	zstandard
 tests_require = 
 	pytest
 	pytest-cov
 	pytest-flake8
 	pytest-timeout
-	pytest-html
+	pytest-html==3.2.0
 	requests_mock
 	flake8>=4.0.0,<5.0.0  # workaround: https://github.com/tholo/pytest-flake8/issues/87
 setup_requires = 
 	pytest-runner
 python_requires = >= 3.7
 
 [options.packages.find]
```

### Comparing `sinetstream-1.7.0/src/sinetstream/__init__.py` & `sinetstream-1.8.0/src/sinetstream/__init__.py`

 * *Files identical despite different names*

### Comparing `sinetstream-1.7.0/src/sinetstream/__main__.py` & `sinetstream-1.8.0/src/sinetstream/__main__.py`

 * *Files identical despite different names*

### Comparing `sinetstream-1.7.0/src/sinetstream/api.py` & `sinetstream-1.8.0/src/sinetstream/api.py`

 * *Files identical despite different names*

### Comparing `sinetstream-1.7.0/src/sinetstream/compression.py` & `sinetstream-1.8.0/src/sinetstream/compression.py`

 * *Files identical despite different names*

### Comparing `sinetstream-1.7.0/src/sinetstream/config_client.py` & `sinetstream-1.8.0/src/sinetstream/config_client.py`

 * *Files identical despite different names*

### Comparing `sinetstream-1.7.0/src/sinetstream/configs.py` & `sinetstream-1.8.0/src/sinetstream/configs.py`

 * *Files identical despite different names*

### Comparing `sinetstream-1.7.0/src/sinetstream/crypto.py` & `sinetstream-1.8.0/src/sinetstream/crypto.py`

 * *Files identical despite different names*

### Comparing `sinetstream-1.7.0/src/sinetstream/error.py` & `sinetstream-1.8.0/src/sinetstream/error.py`

 * *Files identical despite different names*

### Comparing `sinetstream-1.7.0/src/sinetstream/marshal.py` & `sinetstream-1.8.0/src/sinetstream/marshal.py`

 * *Files identical despite different names*

### Comparing `sinetstream-1.7.0/src/sinetstream/spi.py` & `sinetstream-1.8.0/src/sinetstream/spi.py`

 * *Files identical despite different names*

### Comparing `sinetstream-1.7.0/src/sinetstream/utils.py` & `sinetstream-1.8.0/src/sinetstream/utils.py`

 * *Files identical despite different names*

### Comparing `sinetstream-1.7.0/src/sinetstream/value_type.py` & `sinetstream-1.8.0/src/sinetstream/value_type.py`

 * *Files identical despite different names*

### Comparing `sinetstream-1.7.0/src/sinetstream.egg-info/PKG-INFO` & `sinetstream-1.8.0/src/sinetstream.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,101 +1,100 @@
 Metadata-Version: 2.1
 Name: sinetstream
-Version: 1.7.0
+Version: 1.8.0
 Summary: Library for operating messaging systems such as Apache Kafka and MQTT with the same API.
 Home-page: https://github.com/nii-gakunin-cloud/sinetstream
 License: Apache License, Version 2.0
-Description: <!--
-        Copyright (C) 2020 National Institute of Informatics
-        
-        Licensed to the Apache Software Foundation (ASF) under one
-        or more contributor license agreements.  See the NOTICE file
-        distributed with this work for additional information
-        regarding copyright ownership.  The ASF licenses this file
-        to you under the Apache License, Version 2.0 (the
-        "License"); you may not use this file except in compliance
-        with the License.  You may obtain a copy of the License at
-        
-          http://www.apache.org/licenses/LICENSE-2.0
-        
-        Unless required by applicable law or agreed to in writing,
-        software distributed under the License is distributed on an
-        "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
-        KIND, either express or implied.  See the License for the
-        specific language governing permissions and limitations
-        under the License.
-        -->
-        
-        [日本語](README.md)
-        
-        # SINETStream python
-        
-        ## Directory structure
-        
-        * src/
-            * Implementation of SINETStream for Python
-        * tests/
-            * Unit test
-        * sample/
-            * Sample program
-        * plugins/
-            * broker/
-                * kafka/
-                    * Kafka Plugin for SINETStream
-                * mqtt
-                    * MQTT Plugin for SINETStream
-            * value_type/
-                * image/
-                    * Plugin for handling image as message
-        * README.md
-        
-        ## Build procedure
-        
-        Execute the following command to build the SINETStream TAR file.
-        
-        ```
-        $ python3 setup.py bdist_wheel
-        $ cd plugins/broker/kafka
-        $ python3 setup.py bdist_wheel
-        $ cd ../mqtt
-        $ python3 setup.py bdist_wheel
-        $ cd ../../value_type/image
-        $ python3 setup.py bdist_wheel
-        ```
-        
-        If the build is successful, the following WHL file will be created.
-        
-        ```
-        ./dist/sinetstream-1.1.0-py3-none-any.whl
-        ./plugins/broker/kafka/dist/sinetstream_kafka-1.1.0-py3-none-any.whl
-        ./plugins/broker/mqtt/dist/sinetstream_mqtt-1.1.0-py3-none-any.whl
-        ./plugins/value_type/image/dist/sinetstream_type_image-1.1.0-py3-none-any.whl
-        ```
-        
-        ## Install
-        
-        You can also use the packages registered in pypi.
-        
-        ```
-        pip3 install --user sinetstream-kafka sinetstream-mqtt
-        ```
-        
-        If you want to handle image as message, please install the image plugin as follows.
-        
-        ```
-        pip3 install --user sinetstream-type-image
-        ```
-        
-        ## Dependent libraries
-        
-        * [kafka-python](https://kafka-python.readthedocs.io/en/master/)
-        * [mqtt client](https://www.eclipse.org/paho/clients/python/docs/)
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Japanese
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+
+<!--
+Copyright (C) 2020 National Institute of Informatics
+
+Licensed to the Apache Software Foundation (ASF) under one
+or more contributor license agreements.  See the NOTICE file
+distributed with this work for additional information
+regarding copyright ownership.  The ASF licenses this file
+to you under the Apache License, Version 2.0 (the
+"License"); you may not use this file except in compliance
+with the License.  You may obtain a copy of the License at
+
+  http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing,
+software distributed under the License is distributed on an
+"AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+KIND, either express or implied.  See the License for the
+specific language governing permissions and limitations
+under the License.
+-->
+
+[日本語](README.md)
+
+# SINETStream python
+
+## Directory structure
+
+* src/
+    * Implementation of SINETStream for Python
+* tests/
+    * Unit test
+* sample/
+    * Sample program
+* plugins/
+    * broker/
+        * kafka/
+            * Kafka Plugin for SINETStream
+        * mqtt
+            * MQTT Plugin for SINETStream
+    * value_type/
+        * image/
+            * Plugin for handling image as message
+* README.md
+
+## Build procedure
+
+Execute the following command to build the SINETStream TAR file.
+
+```
+$ python3 setup.py bdist_wheel
+$ cd plugins/broker/kafka
+$ python3 setup.py bdist_wheel
+$ cd ../mqtt
+$ python3 setup.py bdist_wheel
+$ cd ../../value_type/image
+$ python3 setup.py bdist_wheel
+```
+
+If the build is successful, the following WHL file will be created.
+
+```
+./dist/sinetstream-1.1.0-py3-none-any.whl
+./plugins/broker/kafka/dist/sinetstream_kafka-1.1.0-py3-none-any.whl
+./plugins/broker/mqtt/dist/sinetstream_mqtt-1.1.0-py3-none-any.whl
+./plugins/value_type/image/dist/sinetstream_type_image-1.1.0-py3-none-any.whl
+```
+
+## Install
+
+You can also use the packages registered in pypi.
+
+```
+pip3 install --user sinetstream-kafka sinetstream-mqtt
+```
+
+If you want to handle image as message, please install the image plugin as follows.
+
+```
+pip3 install --user sinetstream-type-image
+```
+
+## Dependent libraries
+
+* [kafka-python](https://kafka-python.readthedocs.io/en/master/)
+* [mqtt client](https://www.eclipse.org/paho/clients/python/docs/)
```

### Comparing `sinetstream-1.7.0/src/sinetstream.egg-info/SOURCES.txt` & `sinetstream-1.8.0/src/sinetstream.egg-info/SOURCES.txt`

 * *Files identical despite different names*

