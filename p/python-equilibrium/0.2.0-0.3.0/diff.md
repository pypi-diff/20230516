# Comparing `tmp/python_equilibrium-0.2.0.tar.gz` & `tmp/python_equilibrium-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_equilibrium-0.2.0.tar", max compression
+gzip compressed data, was "python_equilibrium-0.3.0.tar", max compression
```

## Comparing `python_equilibrium-0.2.0.tar` & `python_equilibrium-0.3.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      988 2023-04-29 15:23:39.604150 python_equilibrium-0.2.0/LICENSE
--rw-r--r--   0        0        0     1648 2023-05-15 12:17:20.303965 python_equilibrium-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       44 2023-05-15 12:17:20.303965 python_equilibrium-0.2.0/src/equilibrium/__init__.py
--rw-r--r--   0        0        0        0 2023-04-30 01:55:51.676435 python_equilibrium-0.2.0/src/equilibrium/py.typed
--rw-r--r--   0        0        0      741 2023-05-12 13:32:26.554091 python_equilibrium-0.2.0/src/equilibrium/resource/AdmissionController.py
--rw-r--r--   0        0        0     8497 2023-05-12 13:32:26.554091 python_equilibrium-0.2.0/src/equilibrium/resource/CrudResourceController.py
--rw-r--r--   0        0        0    12910 2023-05-12 13:32:26.554091 python_equilibrium-0.2.0/src/equilibrium/resource/JsonResourceStore.py
--rw-r--r--   0        0        0     8298 2023-05-12 13:32:26.554091 python_equilibrium-0.2.0/src/equilibrium/resource/JsonResourceStore_test.py
--rw-r--r--   0        0        0      616 2023-05-12 13:32:26.554091 python_equilibrium-0.2.0/src/equilibrium/resource/Namespace.py
--rw-r--r--   0        0        0    13234 2023-05-12 17:39:48.381669 python_equilibrium-0.2.0/src/equilibrium/resource/Resource.py
--rw-r--r--   0        0        0    15071 2023-05-12 17:39:31.274153 python_equilibrium-0.2.0/src/equilibrium/resource/ResourceContext.py
--rw-r--r--   0        0        0      500 2023-05-12 13:32:26.554091 python_equilibrium-0.2.0/src/equilibrium/resource/ResourceController.py
--rw-r--r--   0        0        0     4849 2023-05-12 13:32:26.554091 python_equilibrium-0.2.0/src/equilibrium/resource/ResourceStore.py
--rw-r--r--   0        0        0     2198 2023-05-12 13:32:26.582090 python_equilibrium-0.2.0/src/equilibrium/resource/Resource_test.py
--rw-r--r--   0        0        0     2088 2023-05-12 13:44:07.098245 python_equilibrium-0.2.0/src/equilibrium/resource/Service.py
--rw-r--r--   0        0        0      786 2023-05-12 14:13:31.848076 python_equilibrium-0.2.0/src/equilibrium/resource/__init__.py
--rw-r--r--   0        0        0     2031 2023-05-12 19:29:51.170583 python_equilibrium-0.2.0/src/equilibrium/rules/Cache.py
--rw-r--r--   0        0        0     3161 2023-05-12 19:29:51.170583 python_equilibrium-0.2.0/src/equilibrium/rules/Executor.py
--rw-r--r--   0        0        0      853 2023-05-12 20:59:56.505150 python_equilibrium-0.2.0/src/equilibrium/rules/HashSupport.py
--rw-r--r--   0        0        0     5223 2023-05-12 21:00:21.736435 python_equilibrium-0.2.0/src/equilibrium/rules/Params.py
--rw-r--r--   0        0        0      898 2023-05-12 19:42:53.092371 python_equilibrium-0.2.0/src/equilibrium/rules/Params_test.py
--rw-r--r--   0        0        0     3699 2023-05-15 12:11:03.698682 python_equilibrium-0.2.0/src/equilibrium/rules/Rule.py
--rw-r--r--   0        0        0      417 2023-05-12 19:29:51.170583 python_equilibrium-0.2.0/src/equilibrium/rules/Rule_test.py
--rw-r--r--   0        0        0     3111 2023-05-12 20:59:56.661146 python_equilibrium-0.2.0/src/equilibrium/rules/RulesEngine.py
--rw-r--r--   0        0        0     2682 2023-05-12 19:45:46.695447 python_equilibrium-0.2.0/src/equilibrium/rules/RulesEngine_test.py
--rw-r--r--   0        0        0     3054 2023-05-12 19:29:51.170583 python_equilibrium-0.2.0/src/equilibrium/rules/RulesGraph.py
--rw-r--r--   0        0        0     2639 2023-05-12 19:29:51.170583 python_equilibrium-0.2.0/src/equilibrium/rules/RulesGraph_test.py
--rw-r--r--   0        0        0      420 2023-05-12 14:30:48.998605 python_equilibrium-0.2.0/src/equilibrium/rules/Signature.py
--rw-r--r--   0        0        0      689 2023-05-12 19:29:51.170583 python_equilibrium-0.2.0/src/equilibrium/rules/__init__.py
--rw-r--r--   0        0        0     1415 2023-05-12 19:29:51.170583 python_equilibrium-0.2.0/src/equilibrium/rules/errors.py
--rw-r--r--   0        0        0      758 1970-01-01 00:00:00.000000 python_equilibrium-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      988 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1648 2023-05-16 21:42:27.224180 python_equilibrium-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-05-16 21:42:27.224180 python_equilibrium-0.3.0/src/equilibrium/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/src/equilibrium/py.typed
+-rw-r--r--   0        0        0      741 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/src/equilibrium/resource/AdmissionController.py
+-rw-r--r--   0        0        0     8497 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/src/equilibrium/resource/CrudResourceController.py
+-rw-r--r--   0        0        0    12910 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/src/equilibrium/resource/JsonResourceStore.py
+-rw-r--r--   0        0        0     8298 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/src/equilibrium/resource/JsonResourceStore_test.py
+-rw-r--r--   0        0        0      616 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/src/equilibrium/resource/Namespace.py
+-rw-r--r--   0        0        0    13234 2023-05-16 21:15:49.967795 python_equilibrium-0.3.0/src/equilibrium/resource/Resource.py
+-rw-r--r--   0        0        0    15490 2023-05-16 21:33:14.798476 python_equilibrium-0.3.0/src/equilibrium/resource/ResourceContext.py
+-rw-r--r--   0        0        0      500 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/src/equilibrium/resource/ResourceController.py
+-rw-r--r--   0        0        0     4849 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/src/equilibrium/resource/ResourceStore.py
+-rw-r--r--   0        0        0     2198 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/src/equilibrium/resource/Resource_test.py
+-rw-r--r--   0        0        0     3046 2023-05-16 21:27:19.982844 python_equilibrium-0.3.0/src/equilibrium/resource/Service.py
+-rw-r--r--   0        0        0      989 2023-05-16 21:27:24.034885 python_equilibrium-0.3.0/src/equilibrium/resource/__init__.py
+-rw-r--r--   0        0        0     2031 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/src/equilibrium/rules/Cache.py
+-rw-r--r--   0        0        0     3161 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/src/equilibrium/rules/Executor.py
+-rw-r--r--   0        0        0      853 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/src/equilibrium/rules/HashSupport.py
+-rw-r--r--   0        0        0     5223 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/src/equilibrium/rules/Params.py
+-rw-r--r--   0        0        0      898 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/src/equilibrium/rules/Params_test.py
+-rw-r--r--   0        0        0     3699 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/src/equilibrium/rules/Rule.py
+-rw-r--r--   0        0        0      417 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/src/equilibrium/rules/Rule_test.py
+-rw-r--r--   0        0        0     3111 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/src/equilibrium/rules/RulesEngine.py
+-rw-r--r--   0        0        0     2682 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/src/equilibrium/rules/RulesEngine_test.py
+-rw-r--r--   0        0        0     3054 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/src/equilibrium/rules/RulesGraph.py
+-rw-r--r--   0        0        0     2639 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/src/equilibrium/rules/RulesGraph_test.py
+-rw-r--r--   0        0        0      420 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/src/equilibrium/rules/Signature.py
+-rw-r--r--   0        0        0      689 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/src/equilibrium/rules/__init__.py
+-rw-r--r--   0        0        0     1415 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/src/equilibrium/rules/errors.py
+-rw-r--r--   0        0        0      758 1970-01-01 00:00:00.000000 python_equilibrium-0.3.0/PKG-INFO
```

### Comparing `python_equilibrium-0.2.0/LICENSE` & `python_equilibrium-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.2.0/pyproject.toml` & `python_equilibrium-0.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "python-equilibrium"
-version = "0.2.0"
+version = "0.3.0"
 description = ""
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 packages = [{ include = "equilibrium", from = "src" }]
 classifiers = []
 keywords = []
```

### Comparing `python_equilibrium-0.2.0/src/equilibrium/resource/AdmissionController.py` & `python_equilibrium-0.3.0/src/equilibrium/resource/AdmissionController.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.2.0/src/equilibrium/resource/CrudResourceController.py` & `python_equilibrium-0.3.0/src/equilibrium/resource/CrudResourceController.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.2.0/src/equilibrium/resource/JsonResourceStore.py` & `python_equilibrium-0.3.0/src/equilibrium/resource/JsonResourceStore.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.2.0/src/equilibrium/resource/JsonResourceStore_test.py` & `python_equilibrium-0.3.0/src/equilibrium/resource/JsonResourceStore_test.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.2.0/src/equilibrium/resource/Namespace.py` & `python_equilibrium-0.3.0/src/equilibrium/resource/Namespace.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.2.0/src/equilibrium/resource/Resource.py` & `python_equilibrium-0.3.0/src/equilibrium/resource/Resource.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.2.0/src/equilibrium/resource/ResourceContext.py` & `python_equilibrium-0.3.0/src/equilibrium/resource/ResourceContext.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,20 +149,26 @@
 
 
 class ServiceRegistry(Service.Provider):
     def __init__(self, resources: ResourceStore) -> None:
         self._resources = resources
         self._services: dict[Resource.Type, dict[Service.Id, Service]] = {}
 
-    def register(self, resource_type: Resource.Type | type[Resource.Spec], service: Service) -> None:
+    def register(self, service: Service, resource_type: Resource.Type | type[Resource.Spec] | None = None) -> None:
         """
-        Register a service to the controller for the given resource type.
+        Register a service to the controller for the given resource type. If no resource type is specified, the
+        service must have a resource type specified in its class definition. If no resource type is specified, a
+        `ValueError` is raised.
         """
 
-        if isinstance(resource_type, type):
+        if resource_type is None:
+            if service.RESOURCE_TYPE is None:
+                raise ValueError(f"Service {service!r} does not specify a resource type")
+            resource_type = service.RESOURCE_TYPE
+        elif isinstance(resource_type, type):
             resource_type = resource_type.TYPE
 
         service.resources = self._resources
         service.services = self
         services = self._services.setdefault(resource_type, {})
         if service.SERVICE_ID in services:
             raise ValueError(
```

### Comparing `python_equilibrium-0.2.0/src/equilibrium/resource/ResourceStore.py` & `python_equilibrium-0.3.0/src/equilibrium/resource/ResourceStore.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.2.0/src/equilibrium/resource/Resource_test.py` & `python_equilibrium-0.3.0/src/equilibrium/resource/Resource_test.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.2.0/src/equilibrium/resource/Service.py` & `python_equilibrium-0.3.0/src/equilibrium/resource/Service.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,42 +13,61 @@
     except ValueError:
         raise ValueError(f"Invalid serviceId: {s!r}")
 
 
 class Service(ABC):
     """
     Base class for services that can be registered to a context and retrieved by controllers. Services are pluggable
-    components that support various actions no resources.
+    components that support various actions no resources. The same service implementation can be registered multiple
+    types to support different resource types, but if that's not the case, the *resourceType* may be specified as part
+    of the class definition.
     """
 
     Id = NewType("Id", str)
     T = TypeVar("T", bound="Service")
 
     #: A globally unique identifier of the service type. The identifier is used to retrieve the service from the
     #: context. This must begin with an apiVersion and end with a kind, separated by a slash. The apiVersion and kind
     #: must be valid DNS subdomains.
     SERVICE_ID: ClassVar[Id]
 
+    #: The resource type that the service supports. This is used when the service is registered without explicitly
+    #: specifying the resource type to register it for. If this is None, the resource type to register the service for
+    #: must always be explicitly specified.
+    RESOURCE_TYPE: ClassVar[Resource.Type | None] = None
+
     #: Assigned to the service upon registration to the context.
     resources: ResourceStore
     services: Service.Provider
 
     class Provider(ABC):
         @abstractmethod
         def get(self, resource_type: Resource.Type, service_type: type[Service.T]) -> Service.T | None:
             ...
 
-    def __init_subclass__(cls, serviceId: str | None = None, **kwargs: Any) -> None:
+    def __init_subclass__(
+        cls,
+        serviceId: str | None = None,
+        resourceType: type[Resource.Spec] | Resource.Type | None = None,
+        **kwargs: Any,
+    ) -> None:
         # Check if any of the base classes is a subclass of the service. In this case, the `serviceId` is inherited
         # and must not be redefined.
         if any(issubclass(x, Service) and x is not Service for x in cls.__bases__):
             if serviceId is not None:
                 raise RuntimeError("Service implementation must not redefine serviceId")
             assert hasattr(cls, "SERVICE_ID"), "Service parent class should have a serviceId defined."
 
         else:
             if serviceId is None:
                 raise RuntimeError("Service subclass must define serviceId")
             validate_service_id(serviceId)
             cls.SERVICE_ID = cls.Id(serviceId)
 
+        if resourceType is not None:
+            if cls.RESOURCE_TYPE is not None:
+                raise RuntimeError("Service subclass must not redefine resourceType")
+            if isinstance(resourceType, type):
+                resourceType = resourceType.TYPE
+            cls.RESOURCE_TYPE = resourceType
+
         return super().__init_subclass__(**kwargs)
```

### Comparing `python_equilibrium-0.2.0/src/equilibrium/rules/Cache.py` & `python_equilibrium-0.3.0/src/equilibrium/rules/Cache.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.2.0/src/equilibrium/rules/Executor.py` & `python_equilibrium-0.3.0/src/equilibrium/rules/Executor.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.2.0/src/equilibrium/rules/HashSupport.py` & `python_equilibrium-0.3.0/src/equilibrium/rules/HashSupport.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.2.0/src/equilibrium/rules/Params.py` & `python_equilibrium-0.3.0/src/equilibrium/rules/Params.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.2.0/src/equilibrium/rules/Params_test.py` & `python_equilibrium-0.3.0/src/equilibrium/rules/Params_test.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.2.0/src/equilibrium/rules/Rule.py` & `python_equilibrium-0.3.0/src/equilibrium/rules/Rule.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.2.0/src/equilibrium/rules/RulesEngine.py` & `python_equilibrium-0.3.0/src/equilibrium/rules/RulesEngine.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.2.0/src/equilibrium/rules/RulesEngine_test.py` & `python_equilibrium-0.3.0/src/equilibrium/rules/RulesEngine_test.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.2.0/src/equilibrium/rules/RulesGraph.py` & `python_equilibrium-0.3.0/src/equilibrium/rules/RulesGraph.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.2.0/src/equilibrium/rules/RulesGraph_test.py` & `python_equilibrium-0.3.0/src/equilibrium/rules/RulesGraph_test.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.2.0/src/equilibrium/rules/__init__.py` & `python_equilibrium-0.3.0/src/equilibrium/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.2.0/src/equilibrium/rules/errors.py` & `python_equilibrium-0.3.0/src/equilibrium/rules/errors.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.2.0/PKG-INFO` & `python_equilibrium-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-equilibrium
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

