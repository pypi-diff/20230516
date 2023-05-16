# Comparing `tmp/py_nvidia_cumulus-0.0.3.tar.gz` & `tmp/py_nvidia_cumulus-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "py_nvidia_cumulus-0.0.4.tar", max compression
```

## Comparing `py_nvidia_cumulus-0.0.3.tar` & `py_nvidia_cumulus-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,9 @@
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 py_nvidia_cumulus-0.0.3/Makefile
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 py_nvidia_cumulus-0.0.3/requirements.txt
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 py_nvidia_cumulus-0.0.3/cumulus/__init__.py
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 py_nvidia_cumulus-0.0.3/cumulus/api.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 py_nvidia_cumulus-0.0.3/cumulus/base.py
--rw-r--r--   0        0        0     9505 2020-02-02 00:00:00.000000 py_nvidia_cumulus-0.0.3/cumulus/models.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 py_nvidia_cumulus-0.0.3/cumulus/util.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 py_nvidia_cumulus-0.0.3/tests/test_api.py
--rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 py_nvidia_cumulus-0.0.3/tests/test_base.py
--rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 py_nvidia_cumulus-0.0.3/tests/test_models.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 py_nvidia_cumulus-0.0.3/.gitignore
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 py_nvidia_cumulus-0.0.3/LICENSE
--rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 py_nvidia_cumulus-0.0.3/README.md
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 py_nvidia_cumulus-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 py_nvidia_cumulus-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-05-16 15:35:12.958070 py_nvidia_cumulus-0.0.4/LICENSE
+-rw-r--r--   0        0        0     3819 2023-05-16 15:35:12.958070 py_nvidia_cumulus-0.0.4/README.md
+-rw-r--r--   0        0        0       39 2023-05-16 15:35:12.958070 py_nvidia_cumulus-0.0.4/cumulus/__init__.py
+-rw-r--r--   0        0        0     2173 2023-05-16 15:35:12.958070 py_nvidia_cumulus-0.0.4/cumulus/api.py
+-rw-r--r--   0        0        0     3078 2023-05-16 15:35:12.958070 py_nvidia_cumulus-0.0.4/cumulus/base.py
+-rw-r--r--   0        0        0     9499 2023-05-16 15:35:12.958070 py_nvidia_cumulus-0.0.4/cumulus/models.py
+-rw-r--r--   0        0        0      156 2023-05-16 15:35:12.958070 py_nvidia_cumulus-0.0.4/cumulus/util.py
+-rw-r--r--   0        0        0      661 2023-05-16 15:35:12.958070 py_nvidia_cumulus-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4604 1970-01-01 00:00:00.000000 py_nvidia_cumulus-0.0.4/PKG-INFO
```

### Comparing `py_nvidia_cumulus-0.0.3/cumulus/api.py` & `py_nvidia_cumulus-0.0.4/cumulus/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from requests import Session
 from .base import Request
 from .models import (Revision, Root,
                      Router, Platform, Bridge,
                      Mlag, Evpn, Qos,
                      Interface, Service, System,
                      Vrf, Nve, Acl, AAA,
-                     Bridge, Evpn, User, Role)
+                     User, Role)
 
 
 class Cumulus:
     """
     A thin wrapper around Cumulus API endpoints
-    :param str url: a URL to the Cumulus host in the format <protocol>://<host>:<port>
-    :param tuple auth: Cumulus host authentication details in the format ('user', 'pass')
+    :param str url: a URL to the Cumulus host
+        in the format <protocol>://<host>:<port>
+    :param tuple auth: Cumulus host authentication details
+        in the format ('user', 'pass')
 
     >>> api = Cumulus(url="http://127.0.0.1:8765",
                       auth=("user", "password"))
     """
 
     def __init__(self, url: str, auth: tuple, http_session=Session()) -> None:
         self.url = self._format_url(url)
```

### Comparing `py_nvidia_cumulus-0.0.3/cumulus/base.py` & `py_nvidia_cumulus-0.0.4/cumulus/base.py`

 * *Files identical despite different names*

### Comparing `py_nvidia_cumulus-0.0.3/cumulus/models.py` & `py_nvidia_cumulus-0.0.4/cumulus/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         Get object configuration on a specific path
         :param target_path: a path to the configuration part
             relative to the endpoint
         :param endpoint_params: any params accepted by the endpoint
 
         >>> api.interface.get('lo')
         {'ifindex': 1, 'ip': {'address': {'127.0.0.1/8': {}, '::1/128': {}}},
-        'link': {'mac': '00:00:00:00:00:00', 'mtu': 65536, 'state': {'up': {}}, ...}
+        'link': {'mac': '00:00:00:00:00:00', 'mtu': 65536, ...}
         >>> api.interface.get('lo/ip/address')
         {'127.0.0.1/8': {}, '::1/128': {}}
         >>> api.bridge.get('domain/br_default')
         ...
         """
         url = self._make_path(target_path)
 
@@ -72,15 +72,16 @@
         :param rev: the branch on which to update configuration
         :param data: the payload to send to the endpoint
         :param target_path: a path to the configuration part
             relative to the endpoint
         :param endpoint_params: any params accepted by the endpoint
 
         >>> api.revision.create()
-        {'1': {'state': 'pending', 'transition': {'issue': {}, 'progress': ''}}}
+        {'1': {'state': 'pending',
+               'transition': {'issue': {}, 'progress': ''}}}
         >>> api.interface.patch(rev=api.revision.rev,
                                 data=data,
                                 target_path="lo/ip")
         {'address': {'10.10.10.4/32': {}}}
         >>> api.revision.apply()
         {'state': 'apply', 'transition': {'issue': {}, 'progress': ''}}
         >>> api.revision.is_applied()
```

### Comparing `py_nvidia_cumulus-0.0.3/README.md` & `py_nvidia_cumulus-0.0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,56 @@
 # py-nvidia-cumulus
 Unofficial Python API client for [Nvidia Cumulus Linux](https://docs.nvidia.com/networking-ethernet-software/cumulus-linux-54/pdf/).
 
-## Installation
+## 📖 General information
+The client aims to provide a thin wrapper over the [Cumulus OpenAPI specification](https://docs.nvidia.com/networking-ethernet-software/cumulus-linux-54/api/index.html).<br>
+Therefore, it abstracts endpoints in a Pythonic fashion.
+
+## 🛠 Installation
 
 To install the package, run the following command:
 ```
 pip install py-nvidia-cumulus
 ```
 
-## Quick Start
+To install the package locally, clone this repository and run the following command:
+```
+pip install .
+```
+
+## 🚀 Quickstart
 
 To start using the client, instantiate the Cumulus class with the host and authentication details
 ```python
 from cumulus import Cumulus
 
 nv = Cumulus(
     url="https://127.0.0.1:8765",
     auth=("cumulus", "password")
 )
 # nv.http_session = requests.Session() # set your own session if necessary
 nv.http_session.verify = False # disable SSL verification if necessary
 ```
 
-The client aims to provide a thin wrapper over the [Cumulus OpenAPI specification](https://docs.nvidia.com/networking-ethernet-software/cumulus-linux-53/api/index.html).<br>
-Therefore, it abstracts endpoints in pythonic fashion.
-
-## Examples
+## 📄 Examples
 
 1. Get the IP address of an interface relative to the OpenAPI endpoint
 ```python
 # Instantiate the Cumulus class first
 loopback = nv.interface.get('lo/ip/address')
 print(loopback) # {'127.0.0.1/8': {}, '::1/128': {}}
 ```
 2. Update interface configuration relative to the OpenAPI endpoint:
 ```python
 # Instantiate the Cumulus class first
 nv.revision.create() # create a revision
-# patch an interface by provisiong the created revision ID, new data, and path to the object
+# patch an interface by providing the created revision ID, new data, and path to the object
 nv.interface.patch(rev=nv.revision.rev,
-                    data={"10.255.255.2/32": {}},
-                    target_path="lo/ip/address")
+                   data={"10.255.255.2/32": {}},
+                   target_path="lo/ip/address")
 nv.revision.apply() # apply the changes
 nv.revision.is_applied() # watch the switch to make sure the changes were applied successfully
 ```
 
 3. Here is a more complex example on how to deploy the entire switch configuration using the `root` endpoint.
 We will also see how to get the diff between the current revision and the one we are applying.
 ```python
@@ -85,12 +91,18 @@
     url="https://127.0.0.1:8765",
     auth=("cumulus", "password")
 )
 programming = BaseModel(client=nv, endpoint="system/forwarding/programming")
 print(programming.get(endpoint_params={"rev": "applied"}))
 ```
 
-## Tests
-To execute a set of unit tests, run the following command in the root of the project
-```bash
-make test
-```
+## 🏷️ Versioning
+
+We use [SemVer](http://semver.org/) for versioning.
+To see the available versions, check the [PyPI page](https://pypi.org/project/py-nvidia-cumulus/#history) or [tags in this repository](https://github.com/NCCloud/py-nvidia-cumulus/tags).
+
+## 🤝 Contribution
+
+We welcome contributions, issues, and feature requests!
+Also, please refer to our [contribution guidelines](https://github.com/NCCloud/py-nvidia-cumulus/blob/main/.github/CONTRIBUTING.md) for details.
+
+Made with <span style="color: #e25555;">&hearts;</span> by [Namecheap Cloud Team](https://github.com/NCCloud)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `py_nvidia_cumulus-0.0.3/PKG-INFO` & `py_nvidia_cumulus-0.0.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,63 +1,76 @@
 Metadata-Version: 2.1
 Name: py-nvidia-cumulus
-Version: 0.0.3
-Summary: A Python API Client for Nvidia Cumulus
-Author-email: Oleg Neichev <oleg.neichev@gmail.com>
-License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
+Version: 0.0.4
+Summary: Python API Client for Nvidia Cumulus
+Home-page: https://github.com/NCCloud/py-nvidia-cumulus
+License: Apache-2.0
+Author: Namecheap Cloud
+Author-email: cloud@namecheap.com
+Requires-Python: >=3.8.1,<4.0.0
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3
-Requires-Dist: requests
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Requires-Dist: requests (>=2.30.0,<3.0.0)
+Project-URL: Repository, https://github.com/NCCloud/py-nvidia-cumulus
 Description-Content-Type: text/markdown
 
 # py-nvidia-cumulus
 Unofficial Python API client for [Nvidia Cumulus Linux](https://docs.nvidia.com/networking-ethernet-software/cumulus-linux-54/pdf/).
 
-## Installation
+## 📖 General information
+The client aims to provide a thin wrapper over the [Cumulus OpenAPI specification](https://docs.nvidia.com/networking-ethernet-software/cumulus-linux-54/api/index.html).<br>
+Therefore, it abstracts endpoints in a Pythonic fashion.
+
+## 🛠 Installation
 
 To install the package, run the following command:
 ```
 pip install py-nvidia-cumulus
 ```
 
-## Quick Start
+To install the package locally, clone this repository and run the following command:
+```
+pip install .
+```
+
+## 🚀 Quickstart
 
 To start using the client, instantiate the Cumulus class with the host and authentication details
 ```python
 from cumulus import Cumulus
 
 nv = Cumulus(
     url="https://127.0.0.1:8765",
     auth=("cumulus", "password")
 )
 # nv.http_session = requests.Session() # set your own session if necessary
 nv.http_session.verify = False # disable SSL verification if necessary
 ```
 
-The client aims to provide a thin wrapper over the [Cumulus OpenAPI specification](https://docs.nvidia.com/networking-ethernet-software/cumulus-linux-53/api/index.html).<br>
-Therefore, it abstracts endpoints in pythonic fashion.
-
-## Examples
+## 📄 Examples
 
 1. Get the IP address of an interface relative to the OpenAPI endpoint
 ```python
 # Instantiate the Cumulus class first
 loopback = nv.interface.get('lo/ip/address')
 print(loopback) # {'127.0.0.1/8': {}, '::1/128': {}}
 ```
 2. Update interface configuration relative to the OpenAPI endpoint:
 ```python
 # Instantiate the Cumulus class first
 nv.revision.create() # create a revision
-# patch an interface by provisiong the created revision ID, new data, and path to the object
+# patch an interface by providing the created revision ID, new data, and path to the object
 nv.interface.patch(rev=nv.revision.rev,
-                    data={"10.255.255.2/32": {}},
-                    target_path="lo/ip/address")
+                   data={"10.255.255.2/32": {}},
+                   target_path="lo/ip/address")
 nv.revision.apply() # apply the changes
 nv.revision.is_applied() # watch the switch to make sure the changes were applied successfully
 ```
 
 3. Here is a more complex example on how to deploy the entire switch configuration using the `root` endpoint.
 We will also see how to get the diff between the current revision and the one we are applying.
 ```python
@@ -98,12 +111,19 @@
     url="https://127.0.0.1:8765",
     auth=("cumulus", "password")
 )
 programming = BaseModel(client=nv, endpoint="system/forwarding/programming")
 print(programming.get(endpoint_params={"rev": "applied"}))
 ```
 
-## Tests
-To execute a set of unit tests, run the following command in the root of the project
-```bash
-make test
-```
+## 🏷️ Versioning
+
+We use [SemVer](http://semver.org/) for versioning.
+To see the available versions, check the [PyPI page](https://pypi.org/project/py-nvidia-cumulus/#history) or [tags in this repository](https://github.com/NCCloud/py-nvidia-cumulus/tags).
+
+## 🤝 Contribution
+
+We welcome contributions, issues, and feature requests!
+Also, please refer to our [contribution guidelines](https://github.com/NCCloud/py-nvidia-cumulus/blob/main/.github/CONTRIBUTING.md) for details.
+
+Made with <span style="color: #e25555;">&hearts;</span> by [Namecheap Cloud Team](https://github.com/NCCloud)
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

