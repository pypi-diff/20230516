# Comparing `tmp/drb-driver-odata-1.1.0.tar.gz` & `tmp/drb-driver-odata-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drb-driver-odata-1.1.0.tar", last modified: Wed Dec 28 11:05:28 2022, max compression
+gzip compressed data, was "drb-driver-odata-1.2.0.tar", last modified: Tue May 16 07:59:06 2023, max compression
```

## Comparing `drb-driver-odata-1.1.0.tar` & `drb-driver-odata-1.2.0.tar`

### file list

```diff
@@ -1,31 +1,48 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-28 11:05:28.166759 drb-driver-odata-1.1.0/
--rw-rw-rw-   0 root         (0) root         (0)       60 2022-12-19 16:43:54.000000 drb-driver-odata-1.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5204 2022-12-28 11:05:28.166759 drb-driver-odata-1.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4747 2022-12-20 08:38:10.000000 drb-driver-odata-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-28 11:05:28.158759 drb-driver-odata-1.1.0/drb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-28 11:05:28.158759 drb-driver-odata-1.1.0/drb/drivers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-28 11:05:28.166759 drb-driver-odata-1.1.0/drb/drivers/odata/
--rw-rw-rw-   0 root         (0) root         (0)      732 2022-12-28 10:44:07.000000 drb-driver-odata-1.1.0/drb/drivers/odata/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2022-12-28 11:05:28.166759 drb-driver-odata-1.1.0/drb/drivers/odata/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     1961 2022-12-19 16:43:54.000000 drb-driver-odata-1.1.0/drb/drivers/odata/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     1527 2022-12-19 16:43:54.000000 drb-driver-odata-1.1.0/drb/drivers/odata/odata_node.py
--rw-rw-rw-   0 root         (0) root         (0)    13571 2022-12-19 16:43:54.000000 drb-driver-odata-1.1.0/drb/drivers/odata/odata_nodes.py
--rw-rw-rw-   0 root         (0) root         (0)    29906 2022-12-19 16:43:54.000000 drb-driver-odata-1.1.0/drb/drivers/odata/odata_services_nodes.py
--rw-rw-rw-   0 root         (0) root         (0)     9077 2022-12-19 16:43:54.000000 drb-driver-odata-1.1.0/drb/drivers/odata/odata_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-28 11:05:28.162759 drb-driver-odata-1.1.0/drb/exceptions/
--rw-rw-rw-   0 root         (0) root         (0)       99 2022-12-19 16:43:54.000000 drb-driver-odata-1.1.0/drb/exceptions/odata.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-28 11:05:28.158759 drb-driver-odata-1.1.0/drb/topics/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-28 11:05:28.162759 drb-driver-odata-1.1.0/drb/topics/odata/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 16:43:54.000000 drb-driver-odata-1.1.0/drb/topics/odata/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      187 2022-12-19 16:43:54.000000 drb-driver-odata-1.1.0/drb/topics/odata/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-28 11:05:28.162759 drb-driver-odata-1.1.0/drb_driver_odata.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5204 2022-12-28 11:05:28.000000 drb-driver-odata-1.1.0/drb_driver_odata.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      623 2022-12-28 11:05:28.000000 drb-driver-odata-1.1.0/drb_driver_odata.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-28 11:05:28.000000 drb-driver-odata-1.1.0/drb_driver_odata.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-12-28 11:05:28.000000 drb-driver-odata-1.1.0/drb_driver_odata.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       75 2022-12-28 11:05:28.000000 drb-driver-odata-1.1.0/drb_driver_odata.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2022-12-28 11:05:28.000000 drb-driver-odata-1.1.0/drb_driver_odata.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       75 2022-12-19 16:43:54.000000 drb-driver-odata-1.1.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      212 2022-12-28 11:05:28.166759 drb-driver-odata-1.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1125 2022-12-19 16:43:54.000000 drb-driver-odata-1.1.0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    83607 2022-12-19 16:43:54.000000 drb-driver-odata-1.1.0/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 07:59:06.096801 drb-driver-odata-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-01-19 12:50:34.000000 drb-driver-odata-1.2.0/LICENCE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       60 2022-12-19 16:43:54.000000 drb-driver-odata-1.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    23132 2023-05-16 07:59:06.096801 drb-driver-odata-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    22747 2023-05-15 09:10:40.000000 drb-driver-odata-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 07:59:05.940799 drb-driver-odata-1.2.0/drb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 07:59:05.936799 drb-driver-odata-1.2.0/drb/drivers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 07:59:06.096801 drb-driver-odata-1.2.0/drb/drivers/odata/
+-rw-rw-rw-   0 root         (0) root         (0)     1162 2023-03-16 14:59:25.000000 drb-driver-odata-1.2.0/drb/drivers/odata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-05-16 07:59:06.100802 drb-driver-odata-1.2.0/drb/drivers/odata/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)    12146 2023-03-21 16:22:48.000000 drb-driver-odata-1.2.0/drb/drivers/odata/expression.py
+-rw-rw-rw-   0 root         (0) root         (0)     2008 2023-05-11 08:47:12.000000 drb-driver-odata-1.2.0/drb/drivers/odata/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1733 2023-05-11 08:47:12.000000 drb-driver-odata-1.2.0/drb/drivers/odata/odata_node.py
+-rw-rw-rw-   0 root         (0) root         (0)    10936 2023-05-11 08:47:12.000000 drb-driver-odata-1.2.0/drb/drivers/odata/odata_nodes.py
+-rw-rw-rw-   0 root         (0) root         (0)    30221 2023-03-16 15:55:06.000000 drb-driver-odata-1.2.0/drb/drivers/odata/odata_services_nodes.py
+-rw-rw-rw-   0 root         (0) root         (0)     9618 2023-05-11 08:47:12.000000 drb-driver-odata-1.2.0/drb/drivers/odata/odata_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 07:59:06.076801 drb-driver-odata-1.2.0/drb/exceptions/
+-rw-rw-rw-   0 root         (0) root         (0)       99 2022-12-19 16:43:54.000000 drb-driver-odata-1.2.0/drb/exceptions/odata.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 07:59:05.940799 drb-driver-odata-1.2.0/drb/topics/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 07:59:06.080801 drb-driver-odata-1.2.0/drb/topics/odata/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 16:43:54.000000 drb-driver-odata-1.2.0/drb/topics/odata/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 07:59:06.080801 drb-driver-odata-1.2.0/drb_driver_odata.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    23132 2023-05-16 07:59:05.000000 drb-driver-odata-1.2.0/drb_driver_odata.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1049 2023-05-16 07:59:05.000000 drb-driver-odata-1.2.0/drb_driver_odata.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 07:59:05.000000 drb-driver-odata-1.2.0/drb_driver_odata.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2023-05-16 07:59:05.000000 drb-driver-odata-1.2.0/drb_driver_odata.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 07:59:05.000000 drb-driver-odata-1.2.0/drb_driver_odata.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       90 2023-05-16 07:59:05.000000 drb-driver-odata-1.2.0/drb_driver_odata.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-16 07:59:05.000000 drb-driver-odata-1.2.0/drb_driver_odata.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-03-16 15:55:06.000000 drb-driver-odata-1.2.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       92 2023-05-11 08:47:12.000000 drb-driver-odata-1.2.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      954 2023-05-16 07:59:06.096801 drb-driver-odata-1.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-03-16 15:55:06.000000 drb-driver-odata-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 07:59:06.096801 drb-driver-odata-1.2.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2780 2022-12-19 16:43:54.000000 drb-driver-odata-1.2.0/tests/test_attribute_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     1999 2023-05-11 08:47:12.000000 drb-driver-odata-1.2.0/tests/test_authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)    20544 2023-03-21 16:22:48.000000 drb-driver-odata-1.2.0/tests/test_expression.py
+-rw-rw-rw-   0 root         (0) root         (0)     1699 2023-05-11 08:47:12.000000 drb-driver-odata-1.2.0/tests/test_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     4768 2023-05-11 08:47:12.000000 drb-driver-odata-1.2.0/tests/test_odata_dias_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     4288 2022-12-19 16:43:54.000000 drb-driver-odata-1.2.0/tests/test_odata_service_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     5745 2023-05-11 08:47:12.000000 drb-driver-odata-1.2.0/tests/test_odata_svc_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     6882 2022-12-19 16:43:54.000000 drb-driver-odata-1.2.0/tests/test_odata_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4811 2023-05-11 08:47:12.000000 drb-driver-odata-1.2.0/tests/test_orders.py
+-rw-rw-rw-   0 root         (0) root         (0)     6686 2023-03-16 14:59:25.000000 drb-driver-odata-1.2.0/tests/test_predicate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1854 2022-12-19 16:43:54.000000 drb-driver-odata-1.2.0/tests/test_product_attribute_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     4233 2023-05-11 08:47:12.000000 drb-driver-odata-1.2.0/tests/test_product_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     1803 2023-05-11 08:47:12.000000 drb-driver-odata-1.2.0/tests/test_signature.py
+-rw-rw-rw-   0 root         (0) root         (0)    83607 2022-12-19 16:43:54.000000 drb-driver-odata-1.2.0/versioneer.py
```

### Comparing `drb-driver-odata-1.1.0/drb/drivers/odata/factory.py` & `drb-driver-odata-1.2.0/drb/drivers/odata/factory.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import io
 import json
+import keyring
 
+from requests.auth import HTTPBasicAuth
 from drb.core import DrbFactory, DrbNode
 from drb.drivers.http import DrbHttpNode
 from drb.drivers.json import JsonNode
 from drb.exceptions.core import DrbFactoryException
-from drb.utils import keyringconnection
-
-
 from .odata_node import OdataNode
 from .odata_nodes import ODataProductNode
 from .odata_services_nodes import ODataServiceNodeDhus, \
     ODataServiceNodeDias, ODataServiceNodeCSC
 from .odata_utils import ODataServiceType, ODataUtils
 
 
@@ -28,18 +27,21 @@
             req = node.get_impl(io.BytesIO).read().decode()
             json_node = JsonNode(json.loads(req))
             return [ODataProductNode(source=node.path.original_path,
                                      auth=node.auth,
                                      data=e.value
                                      ) for e in json_node['value', :]]
         final_url = node.path.name.replace('+odata', '')
-        auth = None
-        if keyringconnection.kr_check(final_url):
-            auth = keyringconnection.kr_get_auth(final_url)
+
+        auth = keyring.get_keyring().get_credential(final_url, None)
+        if auth is not None:
+            auth = HTTPBasicAuth(auth.username, auth.password)
+
         service_type = ODataUtils.get_type_odata_svc(final_url, auth)
         if service_type == ODataServiceType.CSC:
             return ODataServiceNodeCSC(final_url, auth)
         if service_type == ODataServiceType.DHUS:
             return ODataServiceNodeDhus(final_url, auth)
         if service_type == ODataServiceType.ONDA_DIAS:
             return ODataServiceNodeDias(final_url, auth)
+
         raise DrbFactoryException(f'Unsupported Odata service: {final_url}')
```

### Comparing `drb-driver-odata-1.1.0/drb/drivers/odata/odata_node.py` & `drb-driver-odata-1.2.0/drb/drivers/odata/odata_node.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import abc
-
+import keyring
 from drb.nodes.abstract_node import AbstractNode
-from requests.auth import AuthBase
+from requests.auth import AuthBase, HTTPBasicAuth
 from typing import Optional
-from drb.utils.keyringconnection import kr_get_auth, kr_check
 
 
 class OdataNode(AbstractNode, abc.ABC):
     """
     Common ODataNode interface
     """
 
@@ -29,23 +28,31 @@
     def get_auth(self) -> Optional[AuthBase]:
         """
         Returns the associated authentication required to access to the OData
         service.
         :returns: an authentication compatible with requests library.
         :rtype: AuthBase
         """
-        if self.__auth is not None:
-            return self.__auth
-        if kr_check(self._original_service_url):
-            return kr_get_auth(self._original_service_url)
+        if self.__auth is None:
+            auth = keyring.get_keyring().get_credential(
+                self._original_service_url, None)
+            if auth is not None:
+                self.__auth = HTTPBasicAuth(auth.username, auth.password)
+        return self.__auth
 
     @property
     @abc.abstractmethod
     def type_service(self):
         raise NotImplementedError
 
     def __eq__(self, other):
         return isinstance(other, OdataNode) and \
             self._service_url == other._service_url
 
     def __hash__(self):
         return hash(self._service_url)
+
+    def __setitem__(self, key, value):
+        raise NotImplementedError
+
+    def __delitem__(self, key):
+        raise NotImplementedError
```

### Comparing `drb-driver-odata-1.1.0/drb/drivers/odata/odata_services_nodes.py` & `drb-driver-odata-1.2.0/drb/drivers/odata/odata_services_nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,18 @@
         raise NotImplementedError
 
     @property
     def orders(self):
         raise NotImplementedError
 
     @property
+    def orders_eta(self):
+        raise NotImplementedError
+
+    @property
     def name(self) -> str:
         return self._service_url
 
     @property
     def value(self) -> Optional[Any]:
         return None
 
@@ -219,14 +223,18 @@
         return 'Id'
 
     @property
     def order(self) -> str:
         return 'OData.CSC.Order'
 
     @property
+    def orders_eta(self) -> str:
+        return 'EstimatedDate'
+
+    @property
     def filter_keyword(self) -> str:
         return '$filter'
 
     @property
     def is_count_accepted_in_request(self) -> bool:
         return True
 
@@ -297,14 +305,18 @@
         return 'Id'
 
     @property
     def order(self) -> str:
         raise NotImplementedError
 
     @property
+    def orders_eta(self) -> str:
+        raise NotImplementedError
+
+    @property
     def filter_keyword(self) -> str:
         return '$filter'
 
     @property
     def is_count_accepted_in_request(self) -> bool:
         return True
 
@@ -447,14 +459,18 @@
         return 'id'
 
     @property
     def order(self) -> str:
         return 'Ens.Order'
 
     @property
+    def orders_eta(self) -> str:
+        return 'EstimatedTime'
+
+    @property
     def filter_keyword(self) -> str:
         return '$search'
 
     @property
     def is_count_accepted_in_request(self) -> bool:
         return False
```

### Comparing `drb-driver-odata-1.1.0/drb/drivers/odata/odata_utils.py` & `drb-driver-odata-1.2.0/drb/drivers/odata/odata_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from drb.drivers.http import DrbHttpNode
 from drb.exceptions.core import DrbException
 from requests.auth import AuthBase
 from typing import List
 from defusedxml import ElementTree
 from defusedxml.ElementTree import ParseError
 
-
+from .expression import Expression
 from .odata_node import OdataNode
 from ...exceptions.odata import OdataRequestException
 
 
 class ODataServiceType(Enum):
     UNKNOWN = 0
     CSC = 1
@@ -195,14 +195,16 @@
         node = DrbHttpNode(url, auth=odata.get_auth())
         if start is None or end is None:
             return node.get_impl(io.BytesIO)
         return node.get_impl(io.BytesIO, start=start, end=end)
 
     @staticmethod
     def launch_order(odata: OdataNode, prd_uuid: str, order: str):
+        if not isinstance(prd_uuid, str):
+            raise TypeError
         url = f'{odata.get_service_url()}/' \
               f'{odata.format_product(prd_uuid)}/{order}'
         node = DrbHttpNode.post(url,
                                 auth=odata.get_auth())
         return node
 
     @staticmethod
@@ -220,30 +222,39 @@
 
 class ODataQueryPredicate(Predicate):
     """
     This predicate allowing to customize an OData query request.
     Customizable OData query elements: filter, search, orderby.
 
     Keyword Arguments:
-        filter (str): the OData filter query element
+        filter (str | Expression): the OData filter query element
         search (str): the OData search query element
         order (str): the OData orderby query element
     """
 
     def __init__(self, **kwargs):
         self.__filter = kwargs['filter'] if 'filter' in kwargs.keys() else None
         self.__search = kwargs['search'] if 'search' in kwargs.keys() else None
         self.__order = kwargs['order'] if 'order' in kwargs.keys() else None
 
     @property
     def filter(self) -> str:
+        if isinstance(self.__filter, Expression):
+            return self.__filter.evaluate()
         return self.__filter
 
     @property
     def order(self) -> str:
+        if isinstance(self.__order, tuple):
+            return f"{self.__order[0].evaluate()} {self.__order[1].evaluate()}"
+        if isinstance(self.__order, list):
+            order = ''
+            for o in self.__order:
+                order += f"{o[0].evaluate()} {o[1].evaluate()} "
+            return order[:len(order)-1]
         return self.__order
 
     @property
     def search(self) -> str:
         return self.__search
 
     def matches(self, key) -> bool:
```

### Comparing `drb-driver-odata-1.1.0/versioneer.py` & `drb-driver-odata-1.2.0/versioneer.py`

 * *Files identical despite different names*

