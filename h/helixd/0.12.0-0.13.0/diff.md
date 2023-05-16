# Comparing `tmp/helixd-0.12.0.tar.gz` & `tmp/helixd-0.13.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helixd-0.12.0.tar", last modified: Mon May 15 15:47:43 2023, max compression
+gzip compressed data, was "helixd-0.13.0.tar", last modified: Tue May 16 15:02:02 2023, max compression
```

## Comparing `helixd-0.12.0.tar` & `helixd-0.13.0.tar`

### file list

```diff
@@ -1,19 +1,16 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 15:47:43.136738 helixd-0.12.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1061 2023-04-15 11:18:20.000000 helixd-0.12.0/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      716 2023-05-15 15:47:43.136738 helixd-0.12.0/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 15:47:43.136738 helixd-0.12.0/helixd/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10555 2023-05-15 15:44:24.000000 helixd-0.12.0/helixd/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 15:47:43.136738 helixd-0.12.0/helixd.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      716 2023-05-15 15:47:43.000000 helixd-0.12.0/helixd.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      258 2023-05-15 15:47:43.000000 helixd-0.12.0/helixd.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-15 15:47:43.000000 helixd-0.12.0/helixd.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       34 2023-05-15 15:47:43.000000 helixd-0.12.0/helixd.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        7 2023-05-15 15:47:43.000000 helixd-0.12.0/helixd.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 15:47:43.136738 helixd-0.12.0/scripts/
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)       52 2023-04-15 11:18:20.000000 helixd-0.12.0/scripts/helixd
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-15 15:47:43.136738 helixd-0.12.0/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      958 2023-05-15 15:46:54.000000 helixd-0.12.0/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 15:47:43.136738 helixd-0.12.0/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3478 2023-04-15 11:18:20.000000 helixd-0.12.0/tests/test_cli.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13834 2023-05-15 15:44:24.000000 helixd-0.12.0/tests/test_client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2727 2023-04-15 11:18:20.000000 helixd-0.12.0/tests/test_stack.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 15:02:02.285746 helixd-0.13.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1061 2023-04-15 11:18:20.000000 helixd-0.13.0/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      716 2023-05-16 15:02:02.285746 helixd-0.13.0/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 15:02:02.285746 helixd-0.13.0/helixd/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9625 2023-05-16 14:48:15.000000 helixd-0.13.0/helixd/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 15:02:02.285746 helixd-0.13.0/helixd.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      716 2023-05-16 15:02:02.000000 helixd-0.13.0/helixd.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      225 2023-05-16 15:02:02.000000 helixd-0.13.0/helixd.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-16 15:02:02.000000 helixd-0.13.0/helixd.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-05-16 15:02:02.000000 helixd-0.13.0/helixd.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        7 2023-05-16 15:02:02.000000 helixd-0.13.0/helixd.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-16 15:02:02.285746 helixd-0.13.0/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      890 2023-05-16 14:58:41.000000 helixd-0.13.0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 15:02:02.285746 helixd-0.13.0/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9933 2023-05-16 14:46:48.000000 helixd-0.13.0/tests/test_client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2727 2023-04-15 11:18:20.000000 helixd-0.13.0/tests/test_stack.py
```

### Comparing `helixd-0.12.0/LICENSE` & `helixd-0.13.0/LICENSE`

 * *Files identical despite different names*

### Comparing `helixd-0.12.0/PKG-INFO` & `helixd-0.13.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helixd
-Version: 0.12.0
+Version: 0.13.0
 Summary: Minimalist LXD API client
 Home-page: https://zebr0.io/projects/helixd
 Download-URL: https://gitlab.com/zebr0/helixd
 Author: Thomas JOUANNOT
 Author-email: mazerty@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
```

### Comparing `helixd-0.12.0/helixd/__init__.py` & `helixd-0.13.0/helixd/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 import enum
 import string
 import time
-from typing import Optional, List
 
-import kivalu
 import requests
 import requests_unixsocket
-import yaml
 
 KEY_DEFAULT = "lxd-stack"
 URL_DEFAULT = "http+unix://%2Fvar%2Fsnap%2Flxd%2Fcommon%2Flxd%2Funix.socket"
 
 
 class ResourceType(enum.Enum):
     """
@@ -83,45 +80,42 @@
     def exists(self, config: dict, resource_type: ResourceType) -> bool:
         """
         :param config: the resource's configuration
         :param resource_type: the resource's type
         :return: whether the resource exists or not
         """
 
-        resource_path = resource_type.path(config) + "/" + config.get("name")
-
-        print("checking existence", resource_path)
         try:
-            self.session.get(self.url + resource_path)
+            self.session.get(self.url + resource_type.path(config) + "/" + config.get("name"))
             return True
         except requests.HTTPError:
             return False
 
-    def create(self, config: dict, resource_type: ResourceType) -> None:
+    def create(self, config: dict, resource_type: ResourceType = ResourceType.INSTANCES) -> None:
         """
         Creates a resource if it doesn't exist.
         The required configuration depends on the resource's type (see helixd.Client).
 
         :param config: the resource's desired configuration
-        :param resource_type: the resource's type
+        :param resource_type: the resource's type, defaults to INSTANCES
         """
 
         type_path = resource_type.path(config)
         resource_path = type_path + "/" + config.get("name")
 
         if not self.exists(config, resource_type):
             print("creating", resource_path)
             self.session.post(self.url + type_path, json=config)
 
-    def delete(self, config: dict, resource_type: ResourceType) -> None:
+    def delete(self, config: dict, resource_type: ResourceType = ResourceType.INSTANCES) -> None:
         """
         Deletes a resource if it exists.
 
         :param config: the resource's configuration
-        :param resource_type: the resource's type
+        :param resource_type: the resource's type, defaults to INSTANCES
         """
 
         resource_path = resource_type.path(config) + "/" + config.get("name")
 
         if self.exists(config, resource_type):
             print(f"deleting", resource_path)
             self.session.delete(self.url + resource_path)
@@ -131,49 +125,48 @@
         :param config: the resource's configuration
         :param resource_type: the resource's type, defaults to INSTANCES
         :return: whether the resource is running or not
         """
 
         resource_path = resource_type.path(config) + "/" + config.get("name")
 
-        print("checking status", resource_path)
         return self.session.get(self.url + resource_path).json().get("metadata").get("status") == "Running"
 
     def start(self, config: dict, resource_type: ResourceType = ResourceType.INSTANCES) -> None:
         """
         Starts a resource if it's not running.
 
         :param config: the resource's configuration
-        :param resource_type: the resource's type
+        :param resource_type: the resource's type, defaults to INSTANCES
         """
 
         resource_path = resource_type.path(config) + "/" + config.get("name")
 
         if not self.is_running(config, resource_type):
             print("starting", resource_path)
             self.session.put(self.url + resource_path + "/state", json={"action": "start"})
 
     def stop(self, config: dict, resource_type: ResourceType = ResourceType.INSTANCES) -> None:
         """
         Stops a resource if it's running.
 
         :param config: the resource's configuration
-        :param resource_type: the resource's type
+        :param resource_type: the resource's type, defaults to INSTANCES
         """
 
         resource_path = resource_type.path(config) + "/" + config.get("name")
 
         if self.exists(config, resource_type) and self.is_running(config, resource_type):
             print("stopping", resource_path)
             self.session.put(self.url + resource_path + "/state", json={"action": "stop"})
 
     def get_ip_address(self, config: dict, resource_type: ResourceType = ResourceType.INSTANCES, device: str = "eth0", family: str = "inet", attempts: int = 10, delay: float = 0.3) -> str:
         """
         :param config: the resource's configuration
-        :param resource_type: the resource's type
+        :param resource_type: the resource's type, defaults to INSTANCES
         :param device: the resource's network device, defaults to eth0
         :param family: the address' family, i.e. inet for IPv4 or inet6 for IPv6, defaults to inet
         :param attempts: maximum number of attempts
         :param delay: delay between two attempts
         :return: the IP address or None if not found
         """
 
@@ -226,29 +219,7 @@
 
         :param stack: the stack as a dictionary
         """
 
         for resource_type in [ResourceType.INSTANCES]:
             for config in stack.get(resource_type.name()) or []:
                 self.stop(config, resource_type)
-
-
-# todo: remove once rollin is functional
-def main(args: Optional[List[str]] = None) -> None:
-    argparser = kivalu.build_argument_parser()
-    argparser.add_argument("command", choices=["create", "delete", "start", "stop"])
-    argparser.add_argument("key", nargs="?", default=KEY_DEFAULT)
-    argparser.add_argument("--lxd-url", default=URL_DEFAULT)
-    args = argparser.parse_args(args)
-
-    value = kivalu.Client(**vars(args)).get(args.key)
-    if not value:
-        print(f"key '{args.key}' not found on server {args.url}")
-        exit(1)
-
-    stack = yaml.load(value, Loader=yaml.BaseLoader)
-    if not isinstance(stack, dict):
-        print(f"key '{args.key}' on server {args.url} is not a proper yaml or json dictionary")
-        exit(1)
-
-    # creates a Client and calls the function corresponding to the given command
-    getattr(Client(args.lxd_url), args.command + "_stack")(stack)
```

### Comparing `helixd-0.12.0/helixd.egg-info/PKG-INFO` & `helixd-0.13.0/helixd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helixd
-Version: 0.12.0
+Version: 0.13.0
 Summary: Minimalist LXD API client
 Home-page: https://zebr0.io/projects/helixd
 Download-URL: https://gitlab.com/zebr0/helixd
 Author: Thomas JOUANNOT
 Author-email: mazerty@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
```

### Comparing `helixd-0.12.0/setup.py` & `helixd-0.13.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 import setuptools
 
 setuptools.setup(
     name="helixd",
-    version="0.12.0",
+    version="0.13.0",
     description="Minimalist LXD API client",
     long_description="TODO",
     long_description_content_type="text/markdown",
     author="Thomas JOUANNOT",
     author_email="mazerty@gmail.com",
     url="https://zebr0.io/projects/helixd",
     download_url="https://gitlab.com/zebr0/helixd",
     packages=["helixd"],
-    scripts=["scripts/helixd"],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Intended Audience :: System Administrators",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: POSIX",
         "Programming Language :: Python :: 3",
         "Topic :: System"
     ],
     license="MIT",
     install_requires=[
-        "kivalu",
-        "PyYAML",
         "requests-unixsocket"
     ]
 )
```

### Comparing `helixd-0.12.0/tests/test_client.py` & `helixd-0.13.0/tests/test_client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,122 +1,76 @@
 import subprocess
 import time
 
 import pytest
 
 from helixd import ResourceType
 
-EXISTS_STORAGE_POOL_OUTPUT = """
-checking existence /1.0/storage-pools/test-storage-pool
-checking existence /1.0/storage-pools/test-storage-pool
-""".lstrip()
-
 
-def test_exists_storage_pool(client, capsys):
+def test_exists_storage_pool(client):
     config = {"name": "test-storage-pool"}
 
     assert not client.exists(config, ResourceType.STORAGE_POOLS)
     subprocess.run("lxc storage create test-storage-pool dir", shell=True)
     assert client.exists(config, ResourceType.STORAGE_POOLS)
 
-    assert capsys.readouterr().out == EXISTS_STORAGE_POOL_OUTPUT
-
-
-EXISTS_VOLUME_OUTPUT = """
-checking existence /1.0/storage-pools/test-storage-pool/volumes/custom/test-volume
-checking existence /1.0/storage-pools/test-storage-pool/volumes/custom/test-volume
-checking existence /1.0/storage-pools/test-storage-pool/volumes/custom/test-volume
-""".lstrip()
-
 
-def test_exists_volume(client, capsys):
+def test_exists_volume(client):
     # first, checking for a volume without a storage pool shouldn't fail
     config = {"name": "test-volume", "parent": "test-storage-pool"}
     assert not client.exists(config, ResourceType.VOLUMES)
 
     subprocess.run("lxc storage create test-storage-pool dir", shell=True)  # given
 
     assert not client.exists(config, ResourceType.VOLUMES)
     subprocess.run("lxc storage volume create test-storage-pool test-volume", shell=True)
     assert client.exists(config, ResourceType.VOLUMES)
 
-    assert capsys.readouterr().out == EXISTS_VOLUME_OUTPUT
-
-
-EXISTS_NETWORK_OUTPUT = """
-checking existence /1.0/networks/test-network
-checking existence /1.0/networks/test-network
-""".lstrip()
-
 
-def test_exists_network(client, capsys):
+def test_exists_network(client):
     config = {"name": "test-network"}
 
     assert not client.exists(config, ResourceType.NETWORKS)
     subprocess.run("lxc network create test-network", shell=True)
     assert client.exists(config, ResourceType.NETWORKS)
 
-    assert capsys.readouterr().out == EXISTS_NETWORK_OUTPUT
 
-
-EXISTS_PROFILE_OUTPUT = """
-checking existence /1.0/profiles/test-profile
-checking existence /1.0/profiles/test-profile
-""".lstrip()
-
-
-def test_exists_profile(client, capsys):
+def test_exists_profile(client):
     config = {"name": "test-profile"}
 
     assert not client.exists(config, ResourceType.PROFILES)
     subprocess.run("lxc profile create test-profile", shell=True)
     assert client.exists(config, ResourceType.PROFILES)
 
-    assert capsys.readouterr().out == EXISTS_PROFILE_OUTPUT
-
 
-EXISTS_INSTANCE_OUTPUT = """
-checking existence /1.0/instances/test-instance
-checking existence /1.0/instances/test-instance
-""".lstrip()
-
-
-def test_exists_instance(client, capsys):
+def test_exists_instance(client):
     config = {"name": "test-instance"}
 
     assert not client.exists(config, ResourceType.INSTANCES)
     subprocess.run("lxc launch test-instance --empty", shell=True)
     assert client.exists(config, ResourceType.INSTANCES)
 
-    assert capsys.readouterr().out == EXISTS_INSTANCE_OUTPUT
-
 
 CREATE_STORAGE_POOL_OUTPUT = """
-checking existence /1.0/storage-pools/test-storage-pool
 creating /1.0/storage-pools/test-storage-pool
-checking existence /1.0/storage-pools/test-storage-pool
-checking existence /1.0/storage-pools/test-storage-pool
 """.lstrip()
 
 
 def test_create_storage_pool(client, capsys):
     config = {"name": "test-storage-pool", "driver": "dir"}
 
     client.create(config, ResourceType.STORAGE_POOLS)
     assert client.exists(config, ResourceType.STORAGE_POOLS)
     client.create(config, ResourceType.STORAGE_POOLS)  # idempotent
 
     assert capsys.readouterr().out == CREATE_STORAGE_POOL_OUTPUT
 
 
 CREATE_VOLUME_OUTPUT = """
-checking existence /1.0/storage-pools/test-storage-pool/volumes/custom/test-volume
 creating /1.0/storage-pools/test-storage-pool/volumes/custom/test-volume
-checking existence /1.0/storage-pools/test-storage-pool/volumes/custom/test-volume
-checking existence /1.0/storage-pools/test-storage-pool/volumes/custom/test-volume
 """.lstrip()
 
 
 def test_create_volume(client, capsys):
     subprocess.run("lxc storage create test-storage-pool dir", shell=True)  # given
 
     config = {"name": "test-volume", "parent": "test-storage-pool"}
@@ -125,74 +79,61 @@
     assert client.exists(config, ResourceType.VOLUMES)
     client.create(config, ResourceType.VOLUMES)  # idempotent
 
     assert capsys.readouterr().out == CREATE_VOLUME_OUTPUT
 
 
 CREATE_NETWORK_OUTPUT = """
-checking existence /1.0/networks/test-network
 creating /1.0/networks/test-network
-checking existence /1.0/networks/test-network
-checking existence /1.0/networks/test-network
 """.lstrip()
 
 
 def test_create_network(client, capsys):
     config = {"name": "test-network"}
 
     client.create(config, ResourceType.NETWORKS)
     assert client.exists(config, ResourceType.NETWORKS)
     client.create(config, ResourceType.NETWORKS)  # idempotent
 
     assert capsys.readouterr().out == CREATE_NETWORK_OUTPUT
 
 
 CREATE_PROFILE_OUTPUT = """
-checking existence /1.0/profiles/test-profile
 creating /1.0/profiles/test-profile
-checking existence /1.0/profiles/test-profile
-checking existence /1.0/profiles/test-profile
 """.lstrip()
 
 
 def test_create_profile(client, capsys):
     config = {"name": "test-profile"}
 
     client.create(config, ResourceType.PROFILES)
     assert client.exists(config, ResourceType.PROFILES)
     client.create(config, ResourceType.PROFILES)  # idempotent
 
     assert capsys.readouterr().out == CREATE_PROFILE_OUTPUT
 
 
 CREATE_INSTANCE_OUTPUT = """
-checking existence /1.0/instances/test-instance
 creating /1.0/instances/test-instance
-checking existence /1.0/instances/test-instance
-checking existence /1.0/instances/test-instance
 """.lstrip()
 
 
 def test_create_instance(client, capsys):
     config = {"name": "test-instance", "source": {"type": "none"}}
 
     client.create(config, ResourceType.INSTANCES)
     assert client.exists(config, ResourceType.INSTANCES)
     client.create(config, ResourceType.INSTANCES)  # idempotent
 
     assert capsys.readouterr().out == CREATE_INSTANCE_OUTPUT
 
 
 DELETE_STORAGE_POOL_OUTPUT = """
-checking existence /1.0/storage-pools/test-storage-pool
 creating /1.0/storage-pools/test-storage-pool
-checking existence /1.0/storage-pools/test-storage-pool
 deleting /1.0/storage-pools/test-storage-pool
-checking existence /1.0/storage-pools/test-storage-pool
-checking existence /1.0/storage-pools/test-storage-pool
 """.lstrip()
 
 
 def test_delete_storage_pool(client, capsys):
     config = {"name": "test-storage-pool", "driver": "dir"}
 
     client.create(config, ResourceType.STORAGE_POOLS)  # given
@@ -201,20 +142,16 @@
     assert not client.exists(config, ResourceType.STORAGE_POOLS)
     client.delete(config, ResourceType.STORAGE_POOLS)  # idempotent
 
     assert capsys.readouterr().out == DELETE_STORAGE_POOL_OUTPUT
 
 
 DELETE_VOLUME_OUTPUT = """
-checking existence /1.0/storage-pools/test-storage-pool/volumes/custom/test-volume
 creating /1.0/storage-pools/test-storage-pool/volumes/custom/test-volume
-checking existence /1.0/storage-pools/test-storage-pool/volumes/custom/test-volume
 deleting /1.0/storage-pools/test-storage-pool/volumes/custom/test-volume
-checking existence /1.0/storage-pools/test-storage-pool/volumes/custom/test-volume
-checking existence /1.0/storage-pools/test-storage-pool/volumes/custom/test-volume
 """.lstrip()
 
 
 def test_delete_volume(client, capsys):
     # given
     subprocess.run("lxc storage create test-storage-pool dir", shell=True)
     config = {"name": "test-volume", "parent": "test-storage-pool"}
@@ -224,20 +161,16 @@
     assert not client.exists(config, ResourceType.VOLUMES)
     client.delete(config, ResourceType.VOLUMES)  # idempotent
 
     assert capsys.readouterr().out == DELETE_VOLUME_OUTPUT
 
 
 DELETE_NETWORK_OUTPUT = """
-checking existence /1.0/networks/test-network
 creating /1.0/networks/test-network
-checking existence /1.0/networks/test-network
 deleting /1.0/networks/test-network
-checking existence /1.0/networks/test-network
-checking existence /1.0/networks/test-network
 """.lstrip()
 
 
 def test_delete_network(client, capsys):
     config = {"name": "test-network"}
 
     client.create(config, ResourceType.NETWORKS)  # given
@@ -246,20 +179,16 @@
     assert not client.exists(config, ResourceType.NETWORKS)
     client.delete(config, ResourceType.NETWORKS)  # idempotent
 
     assert capsys.readouterr().out == DELETE_NETWORK_OUTPUT
 
 
 DELETE_PROFILE_OUTPUT = """
-checking existence /1.0/profiles/test-profile
 creating /1.0/profiles/test-profile
-checking existence /1.0/profiles/test-profile
 deleting /1.0/profiles/test-profile
-checking existence /1.0/profiles/test-profile
-checking existence /1.0/profiles/test-profile
 """.lstrip()
 
 
 def test_delete_profile(client, capsys):
     config = {"name": "test-profile"}
 
     client.create(config, ResourceType.PROFILES)  # given
@@ -268,20 +197,16 @@
     assert not client.exists(config, ResourceType.PROFILES)
     client.delete(config, ResourceType.PROFILES)  # idempotent
 
     assert capsys.readouterr().out == DELETE_PROFILE_OUTPUT
 
 
 DELETE_INSTANCE_OUTPUT = """
-checking existence /1.0/instances/test-instance
 creating /1.0/instances/test-instance
-checking existence /1.0/instances/test-instance
 deleting /1.0/instances/test-instance
-checking existence /1.0/instances/test-instance
-checking existence /1.0/instances/test-instance
 """.lstrip()
 
 
 def test_delete_instance(client, capsys):
     config = {"name": "test-instance", "source": {"type": "none"}}
 
     client.create(config, ResourceType.INSTANCES)  # given
@@ -302,18 +227,15 @@
         "server": "https://images.linuxcontainers.org",
         "protocol": "simplestreams",
         "alias": "ubuntu/20.04"
     }
 }
 
 IS_RUNNING_OUTPUT = """
-checking existence /1.0/instances/test-instance
 creating /1.0/instances/test-instance
-checking status /1.0/instances/test-instance
-checking status /1.0/instances/test-instance
 """.lstrip()
 
 
 def test_is_running(client, capsys):
     client.create(TEST_INSTANCE_CONFIG, ResourceType.INSTANCES)
 
     assert not client.is_running(TEST_INSTANCE_CONFIG)
@@ -321,21 +243,16 @@
     time.sleep(0.2)
     assert client.is_running(TEST_INSTANCE_CONFIG)
 
     assert capsys.readouterr().out == IS_RUNNING_OUTPUT
 
 
 START_OUTPUT = """
-checking status /1.0/instances/test-instance
-checking existence /1.0/instances/test-instance
 creating /1.0/instances/test-instance
-checking status /1.0/instances/test-instance
 starting /1.0/instances/test-instance
-checking status /1.0/instances/test-instance
-checking status /1.0/instances/test-instance
 """.lstrip()
 
 
 def test_start(client, capsys):
     # first, trying to start a non-existent instance should fail
     with pytest.raises(Exception):
         client.start(TEST_INSTANCE_CONFIG, ResourceType.INSTANCES)
@@ -347,25 +264,17 @@
     assert client.is_running(TEST_INSTANCE_CONFIG)
     client.start(TEST_INSTANCE_CONFIG, ResourceType.INSTANCES)  # idempotent
 
     assert capsys.readouterr().out == START_OUTPUT
 
 
 STOP_OUTPUT = """
-checking existence /1.0/instances/test-instance
-checking existence /1.0/instances/test-instance
 creating /1.0/instances/test-instance
-checking status /1.0/instances/test-instance
 starting /1.0/instances/test-instance
-checking existence /1.0/instances/test-instance
-checking status /1.0/instances/test-instance
 stopping /1.0/instances/test-instance
-checking status /1.0/instances/test-instance
-checking existence /1.0/instances/test-instance
-checking status /1.0/instances/test-instance
 """.lstrip()
 
 
 def test_stop(client, capsys):
     # first, trying to stop a non-existent instance shouldn't fail
     client.stop(TEST_INSTANCE_CONFIG, ResourceType.INSTANCES)
```

### Comparing `helixd-0.12.0/tests/test_stack.py` & `helixd-0.13.0/tests/test_stack.py`

 * *Files identical despite different names*

