# Comparing `tmp/pyxdi-0.6.3.tar.gz` & `tmp/pyxdi-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxdi-0.6.3.tar", max compression
+gzip compressed data, was "pyxdi-0.7.0.tar", max compression
```

## Comparing `pyxdi-0.6.3.tar` & `pyxdi-0.7.0.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0     1069 2023-02-14 18:16:50.284355 pyxdi-0.6.3/LICENSE
--rw-r--r--   0        0        0     1352 2023-04-05 18:56:37.235297 pyxdi-0.6.3/README.md
--rw-r--r--   0        0        0     1380 2023-04-29 18:43:08.409486 pyxdi-0.6.3/pyproject.toml
--rw-r--r--   0        0        0      246 2023-03-24 15:06:03.633072 pyxdi-0.6.3/pyxdi/__init__.py
--rw-r--r--   0        0        0    30084 2023-04-29 18:42:44.646420 pyxdi-0.6.3/pyxdi/core.py
--rw-r--r--   0        0        0     1589 2023-03-23 19:35:30.931349 pyxdi-0.6.3/pyxdi/decorators.py
--rw-r--r--   0        0        0      218 2023-02-27 20:19:45.206653 pyxdi-0.6.3/pyxdi/exceptions.py
--rw-r--r--   0        0        0        0 2023-03-24 15:06:03.633484 pyxdi-0.6.3/pyxdi/ext/__init__.py
--rw-r--r--   0        0        0     2502 2023-04-03 07:18:04.638926 pyxdi-0.6.3/pyxdi/ext/fastapi.py
--rw-r--r--   0        0        0        0 2023-03-24 15:06:03.633846 pyxdi-0.6.3/pyxdi/ext/starlette/__init__.py
--rw-r--r--   0        0        0      635 2023-03-24 15:06:03.633960 pyxdi-0.6.3/pyxdi/ext/starlette/middleware.py
--rw-r--r--   0        0        0        0 2023-02-14 18:16:50.285713 pyxdi-0.6.3/pyxdi/py.typed
--rw-r--r--   0        0        0      149 2023-03-25 12:38:39.922067 pyxdi-0.6.3/pyxdi/types.py
--rw-r--r--   0        0        0      262 2023-04-03 07:18:04.639410 pyxdi-0.6.3/pyxdi/utils.py
--rw-r--r--   0        0        0     2290 1970-01-01 00:00:00.000000 pyxdi-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-02-14 18:16:50.284355 pyxdi-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1635 2023-05-16 11:55:56.046789 pyxdi-0.7.0/README.md
+-rw-r--r--   0        0        0     1667 2023-05-16 12:55:03.253417 pyxdi-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      239 2023-05-16 11:55:56.049371 pyxdi-0.7.0/pyxdi/__init__.py
+-rw-r--r--   0        0        0    30760 2023-05-16 11:55:56.049921 pyxdi-0.7.0/pyxdi/core.py
+-rw-r--r--   0        0        0     2464 2023-05-16 11:55:56.050184 pyxdi-0.7.0/pyxdi/decorators.py
+-rw-r--r--   0        0        0      263 2023-05-16 11:55:56.050387 pyxdi-0.7.0/pyxdi/exceptions.py
+-rw-r--r--   0        0        0        0 2023-03-24 15:06:03.633484 pyxdi-0.7.0/pyxdi/ext/__init__.py
+-rw-r--r--   0        0        0     2768 2023-05-16 11:55:56.050777 pyxdi-0.7.0/pyxdi/ext/fastapi.py
+-rw-r--r--   0        0        0        0 2023-03-24 15:06:03.633846 pyxdi-0.7.0/pyxdi/ext/starlette/__init__.py
+-rw-r--r--   0        0        0      635 2023-03-24 15:06:03.633960 pyxdi-0.7.0/pyxdi/ext/starlette/middleware.py
+-rw-r--r--   0        0        0        0 2023-02-14 18:16:50.285713 pyxdi-0.7.0/pyxdi/py.typed
+-rw-r--r--   0        0        0     1846 2023-05-16 12:54:50.100696 pyxdi-0.7.0/pyxdi/utils.py
+-rw-r--r--   0        0        0     2627 1970-01-01 00:00:00.000000 pyxdi-0.7.0/PKG-INFO
```

### Comparing `pyxdi-0.6.3/LICENSE` & `pyxdi-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxdi-0.6.3/README.md` & `pyxdi-0.7.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -15,24 +15,33 @@
 
 ---
 
 ## Requirements
 
 Python 3.7+
 
-and requires [anyio](https://github.com/agronholm/anyio)
+and optional dependencies:
+
+* [anyio](https://github.com/agronholm/anyio) (for supporting synchronous resources with an asynchronous runtime)
+* [lazy-object-proxy](https://github.com/ionelmc/python-lazy-object-proxy) (for supporting lazy injections)
 
 ## Installation
 
 Install using `pip`:
 
 ```shell
 pip install pyxdi
 ```
 
+or with all dependencies (anyio, lazy-object-proxy)
+
+```shell
+pip install pyxdi[all]
+```
+
 or using `poetry`:
 
 ```shell
 poetry add pyxdi
 ```
 
 ## Quick Example
```

### Comparing `pyxdi-0.6.3/pyxdi/core.py` & `pyxdi-0.7.0/pyxdi/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,63 +1,69 @@
 from __future__ import annotations
 
-import sys
 import contextlib
-import functools
 import importlib
 import inspect
 import logging
 import pkgutil
 import typing as t
 import uuid
 from collections import defaultdict
 from contextvars import ContextVar
 from dataclasses import dataclass
-from functools import cached_property, partial
+from functools import cached_property, wraps
 from types import ModuleType, TracebackType
 
+from typing_extensions import Annotated, ParamSpec
+
 try:
     from types import NoneType
 except ImportError:
     NoneType = type(None)  # type: ignore[assignment,misc]
 
-import anyio
 
 from .exceptions import (
     AnnotationError,
     InvalidScope,
     ProviderError,
     ScopeMismatch,
     UnknownDependency,
 )
-from .types import InterfaceT, ProviderObj, Scope
-from .utils import get_qualname
-
-SUPPORT_SIGNATURE_EVAL_STR = sys.version_info > (3, 9)
+from .utils import (
+    get_full_qualname,
+    get_signature,
+    is_builtin_type,
+    make_lazy,
+    run_async,
+)
 
-logger = logging.getLogger(__name__)
+Scope = t.Literal["transient", "singleton", "request"]
+T = t.TypeVar("T", bound=t.Any)
+P = ParamSpec("P")
 
 ALLOWED_SCOPES: t.Dict[Scope, t.List[Scope]] = {
     "singleton": ["singleton"],
     "request": ["request", "singleton"],
     "transient": ["transient", "singleton", "request"],
 }
 
+logger = logging.getLogger(__name__)
+
 
 @dataclass(frozen=True)
 class Provider:
-    obj: ProviderObj
+    obj: t.Callable[..., t.Any]
     scope: Scope
 
     def __str__(self) -> str:
         return self.name
 
     @cached_property
     def name(self) -> str:
-        return get_qualname(self.obj)
+        return get_full_qualname(self.obj)
 
     @cached_property
     def is_class(self) -> bool:
         return inspect.isclass(self.obj)
 
     @cached_property
     def is_function(self) -> bool:
@@ -87,71 +93,83 @@
     scope: Scope
 
 
 @dataclass(frozen=True)
 class ScannedDependency:
     member: t.Any
     module: ModuleType
+    lazy: t.Optional[bool] = None
 
 
-class DependencyMark:
+class _DependencyMark:
     __slots__ = ()
 
 
-def Dependency() -> t.Any:  # noqa
-    return DependencyMark()
+dep = t.cast(t.Any, _DependencyMark())
+
+
+def named(tp: t.Type[T], name: str) -> Annotated[t.Type[T], str]:
+    """
+    Cast annotated type helper.
+    """
+    return t.cast(Annotated[t.Type[T], str], Annotated[tp, name])
 
 
 @dataclass(frozen=True)
 class UnresolvedDependency:
     parameter_name: str
     obj: t.Callable[..., t.Any]
 
 
 class PyxDI:
     def __init__(
         self,
         *,
         default_scope: Scope = "singleton",
         auto_register: bool = False,
+        lazy_inject: bool = False,
     ) -> None:
         self._default_scope = default_scope
         self._auto_register = auto_register
+        self._lazy_inject = lazy_inject
         self._providers: t.Dict[t.Type[t.Any], Provider] = {}
         self._singleton_context = ScopedContext("singleton", self)
         self._request_context_var: ContextVar[t.Optional[ScopedContext]] = ContextVar(
             "request_context", default=None
         )
         self._unresolved_providers: t.Dict[
             t.Type[t.Any], t.List[UnresolvedProvider]
         ] = defaultdict(list)
         self._unresolved_dependencies: t.Dict[t.Type[t.Any], UnresolvedDependency] = {}
-        self._signature_cache: t.Dict[t.Callable[..., t.Any], inspect.Signature] = {}
 
     @property
     def default_scope(self) -> Scope:
         return self._default_scope
 
     @property
     def auto_register(self) -> bool:
         return self._auto_register
 
     @property
+    def lazy_inject(self) -> bool:
+        return self._lazy_inject
+
+    @property
     def providers(self) -> t.Dict[t.Type[t.Any], Provider]:
         return self._providers
 
     # Provider
 
     def has_provider(self, interface: t.Type[t.Any]) -> bool:
         return interface in self._providers
 
     def register_provider(
         self,
         interface: t.Type[t.Any],
-        obj: ProviderObj,
+        obj: t.Callable[..., t.Any],
         *,
         scope: t.Optional[Scope] = None,
         override: bool = False,
         ignore: bool = False,
     ) -> Provider:
         provider = Provider(obj=obj, scope=scope or self.default_scope)
 
@@ -173,29 +191,30 @@
                 logger.info(
                     f"Ignoring the `{provider}` provider as it "
                     "has already been registered."
                 )
                 return registered_provider
 
             raise ProviderError(
-                f"The provider interface `{get_qualname(interface)}` "
+                f"The provider interface `{get_full_qualname(interface)}` "
                 "already registered."
             )
 
         self._validate_provider_scope(provider)
         self._validate_provider_type(provider)
         self._validate_provider_match_scopes(interface, provider)
 
         self._providers[interface] = provider
         return provider
 
     def unregister_provider(self, interface: t.Type[t.Any]) -> None:
         if not self.has_provider(interface):
             raise ProviderError(
-                f"The provider interface `{get_qualname(interface)}` not registered."
+                "The provider interface "
+                f"`{get_full_qualname(interface)}` not registered."
             )
 
         provider = self.get_provider(interface)
 
         # Cleanup scoped context instance
         try:
             scoped_context = self._get_scoped_context(provider.scope)
@@ -211,21 +230,21 @@
         self._unresolved_dependencies.pop(interface, None)
 
     def get_provider(self, interface: t.Type[t.Any]) -> Provider:
         try:
             return self._providers[interface]
         except KeyError as exc:
             raise ProviderError(
-                f"The provider interface for `{get_qualname(interface)}` has not been "
-                "registered. Please ensure that the provider interface is properly "
-                "registered before attempting to use it."
+                f"The provider interface for `{get_full_qualname(interface)}` has "
+                "not been registered. Please ensure that the provider interface is "
+                "properly registered before attempting to use it."
             ) from exc
 
     def singleton(
-        self, interface: t.Type[InterfaceT], instance: t.Any, *, override: bool = False
+        self, interface: t.Type[T], instance: t.Any, *, override: bool = False
     ) -> Provider:
         return self.register_provider(
             interface, lambda: instance, scope="singleton", override=override
         )
 
     # Validators
     def _validate_provider_scope(self, provider: Provider) -> None:
@@ -258,15 +277,15 @@
     def _validate_provider_match_scopes(
         self, interface: t.Type[t.Any], provider: Provider
     ) -> None:
         related_providers = []
 
         obj, scope = provider.obj, provider.scope
 
-        for parameter in self._get_signature(obj).parameters.values():
+        for parameter in get_signature(obj).parameters.values():
             if parameter.annotation is inspect._empty:  # noqa
                 raise AnnotationError(
                     f"Missing provider `{provider}` "
                     f"dependency `{parameter.name}` annotation."
                 )
             try:
                 sub_provider = self.get_provider(parameter.annotation)
@@ -288,15 +307,15 @@
             if direct:
                 left_scope, right_scope = related_provider.scope, scope
             else:
                 left_scope, right_scope = scope, related_provider.scope
             allowed_scopes = ALLOWED_SCOPES.get(right_scope) or []
             if left_scope not in allowed_scopes:
                 raise ScopeMismatch(
-                    f"The provider `{get_qualname(obj)}` with a {scope} scope was "
+                    f"The provider `{get_full_qualname(obj)}` with a {scope} scope was "
                     f"attempted to be registered with the provider "
                     f"`{related_provider}` with a `{related_provider.scope}` scope, "
                     f"which is not allowed. Please ensure that all providers are "
                     f"registered with matching scopes."
                 )
 
     def validate(self) -> None:
@@ -304,18 +323,18 @@
             errors = []
             for (
                 unresolved_interface,
                 unresolved_providers,
             ) in self._unresolved_providers.items():
                 for unresolved_provider in unresolved_providers:
                     parameter_name = unresolved_provider.parameter_name
-                    provider_name = get_qualname(unresolved_provider.provider.obj)
+                    provider_name = get_full_qualname(unresolved_provider.provider.obj)
                     errors.append(
                         f"- `{provider_name}` has unknown `{parameter_name}: "
-                        f"{get_qualname(unresolved_interface)}` parameter"
+                        f"{get_full_qualname(unresolved_interface)}` parameter"
                     )
             message = "\n".join(errors)
             raise UnknownDependency(
                 "The following unknown provided dependencies were detected:"
                 f"\n{message}."
             )
         if self._unresolved_dependencies:
@@ -324,16 +343,16 @@
                 unresolved_interface,
                 dependency,
             ) in self._unresolved_dependencies.items():
                 if inspect.isclass(unresolved_interface) and self.auto_register:
                     continue
                 parameter_name = dependency.parameter_name
                 errors.append(
-                    f"- `{get_qualname(dependency.obj)}` has unknown "
-                    f"`{parameter_name}: {get_qualname(unresolved_interface)}` "
+                    f"- `{get_full_qualname(dependency.obj)}` has unknown "
+                    f"`{parameter_name}: {get_full_qualname(unresolved_interface)}` "
                     f"injected parameter"
                 )
             if not errors:
                 return
             message = "\n".join(errors)
             raise UnknownDependency(
                 "The following unknown injected dependencies were detected:"
@@ -391,35 +410,35 @@
                 "the request context is properly initialized before attempting "
                 "to use it."
             )
         return request_context
 
     # Instance
 
-    def get(self, interface: t.Type[InterfaceT]) -> InterfaceT:
+    def get(self, interface: t.Type[T]) -> T:
         try:
             provider = self.get_provider(interface)
-        except ProviderError as exc:
-            if self.auto_register and inspect.isclass(interface):
-                try:
-                    self._get_signature(interface)
-                except ValueError:
-                    raise exc
+        except ProviderError:
+            if (
+                self.auto_register
+                and inspect.isclass(interface)
+                and not is_builtin_type(interface)
+            ):
                 scope = getattr(interface, "__pyxdi_scope__", self._default_scope)
                 provider = self.register_provider(interface, interface, scope=scope)
             else:
                 raise
 
         scoped_context = self._get_scoped_context(provider.scope)
         if scoped_context:
             return scoped_context.get(interface)
 
-        return t.cast(InterfaceT, self.create_instance(provider))
+        return t.cast(T, self.create_instance(provider))
 
-    def has(self, interface: t.Type[InterfaceT]) -> bool:
+    def has(self, interface: t.Type[T]) -> bool:
         try:
             provider = self.get_provider(interface)
         except ProviderError:
             return False
         scoped_context = self._get_scoped_context(provider.scope)
         if scoped_context:
             return scoped_context.has(interface)
@@ -430,17 +449,15 @@
             return self._singleton_context
         elif scope == "request":
             request_context = self._get_request_context()
             return request_context
         return None
 
     @contextlib.contextmanager
-    def override(
-        self, interface: t.Type[InterfaceT], instance: t.Any
-    ) -> t.Iterator[None]:
+    def override(self, interface: t.Type[T], instance: t.Any) -> t.Iterator[None]:
         origin_instance: t.Optional[t.Any] = None
         origin_provider: t.Optional[Provider] = None
         scope = self.default_scope
 
         if self.has_provider(interface):
             origin_provider = self.get_provider(interface)
             if origin_provider.is_async_resource and not self.has(interface):
@@ -497,90 +514,112 @@
             )
         args, kwargs = self._get_provider_arguments(provider)
         return provider.obj(*args, **kwargs)
 
     # Decorators
 
     @t.overload
-    def provider(
-        self,
-        func: None = ...,
-        *,
-        scope: t.Optional[Scope] = None,
-        override: bool = False,
-        ignore: bool = False,
-    ) -> t.Callable[..., t.Any]:
+    def provider(self, func: t.Callable[P, T]) -> t.Callable[P, T]:
         ...
 
     @t.overload
     def provider(
         self,
-        func: ProviderObj,
         *,
         scope: t.Optional[Scope] = None,
         override: bool = False,
         ignore: bool = False,
-    ) -> t.Callable[[ProviderObj], t.Any]:
+    ) -> t.Callable[[t.Callable[P, T]], t.Callable[P, T]]:
         ...
 
     def provider(
         self,
-        func: t.Union[ProviderObj, None] = None,
-        *,
-        scope: t.Optional[Scope] = None,
-        override: bool = False,
-        ignore: bool = False,
-    ) -> t.Union[ProviderObj, t.Callable[[Provider], t.Any]]:
-        decorator = self._provider_decorator(
-            scope=scope, override=override, ignore=ignore
-        )
-        if func is None:
-            return decorator
-        return decorator(func)  # type: ignore[no-any-return]
-
-    def _provider_decorator(
-        self,
+        func: t.Optional[t.Callable[P, T]] = None,
         *,
         scope: t.Optional[Scope] = None,
         override: bool = False,
         ignore: bool = False,
-    ) -> t.Callable[[ProviderObj], t.Any]:
-        def register_provider(func: ProviderObj) -> t.Any:
+    ) -> t.Union[t.Callable[P, T], t.Callable[[t.Callable[P, T]], t.Callable[P, T]]]:
+        def decorator(func: t.Callable[P, T]) -> t.Callable[P, T]:
             interface = self._get_provider_annotation(func)
             self.register_provider(
                 interface,
                 func,
                 scope=scope,
                 override=override,
                 ignore=ignore,
             )
             return func
 
-        return register_provider
+        if func is None:
+            return decorator
+        return decorator(func)
+
+    @t.overload
+    def inject(self, obj: t.Callable[P, T]) -> t.Callable[P, T]:
+        ...
+
+    @t.overload
+    def inject(
+        self, obj: t.Callable[P, t.Awaitable[T]]
+    ) -> t.Callable[P, t.Awaitable[T]]:
+        ...
 
-    def inject(self, obj: t.Callable[..., t.Any]) -> t.Callable[..., t.Any]:
-        injected_params = self._get_injectable_params(obj)
+    @t.overload
+    def inject(
+        self, *, lazy: t.Optional[bool] = None
+    ) -> t.Callable[
+        [t.Callable[P, t.Union[T, t.Awaitable[T]]]],
+        t.Callable[P, t.Union[T, t.Awaitable[T]]],
+    ]:
+        ...
 
-        if inspect.iscoroutinefunction(obj):
+    def inject(
+        self,
+        obj: t.Union[t.Callable[P, t.Union[T, t.Awaitable[T]]], None] = None,
+        lazy: t.Optional[bool] = None,
+    ) -> t.Union[
+        t.Callable[
+            [t.Callable[P, t.Union[T, t.Awaitable[T]]]],
+            t.Callable[P, t.Union[T, t.Awaitable[T]]],
+        ],
+        t.Callable[P, t.Union[T, t.Awaitable[T]]],
+    ]:
+        lazy = self.lazy_inject if lazy is None else lazy
+
+        def decorator(
+            obj: t.Callable[P, t.Union[T, t.Awaitable[T]]]
+        ) -> t.Callable[P, t.Union[T, t.Awaitable[T]]]:
+            injected_params = self._get_injectable_params(obj)
 
-            @functools.wraps(obj)
-            async def awrapped(*args: t.Any, **kwargs: t.Any) -> t.Any:
+            def _inject_kwargs(**kwargs: P.kwargs) -> t.Dict[str, t.Any]:
                 for name, annotation in injected_params.items():
-                    kwargs[name] = self.get(annotation)
-                return await obj(*args, **kwargs)
+                    if lazy:
+                        kwargs[name] = make_lazy(self.get, annotation)
+                    else:
+                        kwargs[name] = self.get(annotation)
+                return kwargs
+
+            if inspect.iscoroutinefunction(obj):
 
-            return awrapped
+                @wraps(obj)
+                async def awrapped(*args: P.args, **kwargs: P.kwargs) -> T:
+                    return t.cast(T, await obj(*args, **_inject_kwargs(**kwargs)))
 
-        @functools.wraps(obj)
-        def wrapped(*args: t.Any, **kwargs: t.Any) -> t.Any:
-            for name, annotation in injected_params.items():
-                kwargs[name] = self.get(annotation)
-            return obj(*args, **kwargs)
+                return awrapped
 
-        return wrapped
+            @wraps(obj)
+            def wrapped(*args: P.args, **kwargs: P.kwargs) -> T:
+                return t.cast(T, obj(*args, **_inject_kwargs(**kwargs)))
+
+            return wrapped
+
+        if obj is None:
+            return decorator
+        return decorator(obj)
 
     # Scanner
 
     def scan(
         self,
         /,
         packages: t.Union[
@@ -603,22 +642,23 @@
                 package, tags=tags
             )
             scanned_providers.extend(_scanned_providers)
             scanned_dependencies.extend(_scanned_dependencies)
 
         for scanned_provider in scanned_providers:
             self.provider(
-                func=scanned_provider.member,
                 scope=scanned_provider.scope,
                 override=False,
                 ignore=True,
-            )
+            )(scanned_provider.member)
 
         for scanned_dependency in scanned_dependencies:
-            decorator = self.inject(scanned_dependency.member)
+            decorator = self.inject(lazy=scanned_dependency.lazy)(
+                scanned_dependency.member
+            )
             setattr(
                 scanned_dependency.module,
                 scanned_dependency.member.__name__,
                 decorator,
             )
 
     def _scan_package(
@@ -678,135 +718,126 @@
             if provided:
                 scope = provided["scope"]
                 scanned_providers.append(ScannedProvider(member=member, scope=scope))
                 continue
 
             injected = getattr(member, "__pyxdi_inject__", None)
             if injected:
+                lazy = injected["lazy"]
                 scanned_dependencies.append(
-                    self._scanned_dependency(member=member, module=module)
+                    self._scanned_dependency(member=member, module=module, lazy=lazy)
                 )
                 continue
 
             # Get by pyxdi.dep mark
             if inspect.isclass(member):
-                signature = self._get_signature(member.__init__)
+                signature = get_signature(member.__init__)
             else:
-                signature = self._get_signature(member)
+                signature = get_signature(member)
             for parameter in signature.parameters.values():
-                if isinstance(parameter.default, DependencyMark):
+                if isinstance(parameter.default, _DependencyMark):
                     scanned_dependencies.append(
                         self._scanned_dependency(member=member, module=module)
                     )
                     continue
 
         return scanned_providers, scanned_dependencies
 
     def _scanned_dependency(
-        self, member: t.Any, module: ModuleType
+        self, member: t.Any, module: ModuleType, lazy: t.Optional[bool] = None
     ) -> ScannedDependency:
         if hasattr(member, "__wrapped__"):
             member = member.__wrapped__
-        return ScannedDependency(member=member, module=module)
+        return ScannedDependency(member=member, module=module, lazy=lazy)
 
     # Inspection
 
-    def _get_provider_annotation(self, obj: ProviderObj) -> t.Any:
-        annotation = self._get_signature(obj).return_annotation
+    def _get_provider_annotation(self, obj: t.Callable[..., t.Any]) -> t.Any:
+        annotation = get_signature(obj).return_annotation
 
         if annotation is inspect._empty:  # noqa
             raise AnnotationError(
-                f"Missing `{get_qualname(obj)}` provider return annotation."
+                f"Missing `{get_full_qualname(obj)}` provider return annotation."
             )
 
         origin = t.get_origin(annotation) or annotation
         args = t.get_args(annotation)
 
         # Supported generic types
-        if origin in (list, dict, tuple):
+        if origin in (list, dict, tuple, Annotated):
             if args:
                 return annotation
             else:
                 raise AnnotationError(
-                    f"Cannot use `{get_qualname(obj)}` generic type annotation "
+                    f"Cannot use `{get_full_qualname(obj)}` generic type annotation "
                     "without actual type."
                 )
 
         try:
             return args[0]
         except IndexError:
             return annotation
 
     def _get_provider_arguments(
         self, provider: Provider
     ) -> t.Tuple[t.List[t.Any], t.Dict[str, t.Any]]:
         args = []
         kwargs = {}
-        signature = self._get_signature(provider.obj)
+        signature = get_signature(provider.obj)
         for parameter in signature.parameters.values():
             instance = self.get(parameter.annotation)
             if parameter.kind == parameter.POSITIONAL_ONLY:
                 args.append(instance)
             else:
                 kwargs[parameter.name] = instance
         return args, kwargs
 
     def _get_injectable_params(self, obj: t.Callable[..., t.Any]) -> t.Dict[str, t.Any]:
         injectable_params = {}
-        for parameter in self._get_signature(obj).parameters.values():
-            if not isinstance(parameter.default, DependencyMark):
+        for parameter in get_signature(obj).parameters.values():
+            if not isinstance(parameter.default, _DependencyMark):
                 continue
 
             annotation = parameter.annotation
             if annotation is inspect._empty:  # noqa
                 raise AnnotationError(
-                    f"Missing `{get_qualname(obj)}` parameter annotation."
+                    f"Missing `{get_full_qualname(obj)}` parameter annotation."
                 )
 
             if (
                 not self.has_provider(annotation)
                 and annotation not in self._unresolved_providers
                 and annotation not in self._unresolved_dependencies
             ):
                 self._unresolved_dependencies[annotation] = UnresolvedDependency(
                     parameter_name=parameter.name, obj=obj
                 )
 
             injectable_params[parameter.name] = annotation
         return injectable_params
 
-    def _get_signature(self, obj: t.Callable[..., t.Any]) -> inspect.Signature:
-        signature = self._signature_cache.get(obj)
-        if signature is None:
-            signature_kwargs: t.Dict[str, t.Any] = {}
-            if SUPPORT_SIGNATURE_EVAL_STR:
-                signature_kwargs["eval_str"] = True
-            signature = inspect.signature(obj, **signature_kwargs)
-            self._signature_cache[obj] = signature
-        return signature
-
 
 class ScopedContext:
     def __init__(self, scope: Scope, root: PyxDI) -> None:
         self._scope = scope
         self._root = root
         self._instances: t.Dict[t.Type[t.Any], t.Any] = {}
         self._stack = contextlib.ExitStack()
         self._async_stack = contextlib.AsyncExitStack()
 
-    def get(self, interface: t.Type[InterfaceT]) -> InterfaceT:
+    def get(self, interface: t.Type[T]) -> T:
         instance = self._instances.get(interface)
         if instance is None:
             provider = self._root.get_provider(interface)
             if provider.is_resource:
                 instance = self._root.create_resource(provider, stack=self._stack)
             else:
                 instance = self._root.create_instance(provider)
             self._instances[interface] = instance
-        return t.cast(InterfaceT, instance)
+        return t.cast(T, instance)
 
     def set(self, interface: t.Type[t.Any], instance: t.Any) -> None:
         self._instances[interface] = instance
         self._root.register_provider(
             interface, lambda: interface, scope=self._scope, override=True
         )
 
@@ -830,27 +861,27 @@
 
     def close(self) -> None:
         self._stack.close()
 
     async def astart(self) -> None:
         for interface, provider in self._iter_providers():
             if provider.is_resource:
-                instance = await anyio.to_thread.run_sync(
-                    partial(self._root.create_resource, provider, stack=self._stack)
+                instance = await run_async(
+                    self._root.create_resource, provider, stack=self._stack
                 )
                 self.set(interface, instance)
             elif provider.is_async_resource:
                 instance = await self._root.acreate_resource(
                     provider, stack=self._async_stack
                 )
                 self.set(interface, instance)
 
     async def aclose(self) -> None:
         await self._async_stack.aclose()
-        await anyio.to_thread.run_sync(self._stack.close)
+        await run_async(self._stack.close)
 
     def __enter__(self) -> ScopedContext:
         self.start()
         return self
 
     def __exit__(
         self,
```

### Comparing `pyxdi-0.6.3/pyxdi/ext/fastapi.py` & `pyxdi-0.7.0/pyxdi/ext/fastapi.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from fastapi import params
 from fastapi.dependencies.models import Dependant
 from fastapi.routing import APIRoute
 from starlette.requests import Request
 
 import pyxdi
 from pyxdi.ext.starlette.middleware import RequestScopedMiddleware
+from pyxdi.utils import get_signature, make_lazy
 
 __all__ = ["RequestScopedMiddleware", "install", "get_di", "Inject"]
 
 
 def install(app: fastapi.FastAPI, di: pyxdi.PyxDI) -> None:
     app.state.di = di  # noqa
 
@@ -23,15 +24,15 @@
             continue
         for dependant in iter_dependencies(route.dependant):
             if dependant.cache_key not in patched:
                 patched.append(dependant.cache_key)
                 call, *params = dependant.cache_key
                 if not call:
                     continue  # pragma: no cover
-                for param in inspect.signature(call, eval_str=True).parameters.values():
+                for param in get_signature(call).parameters.values():
                     if isinstance(param.default, InjectParam):
                         if param.annotation is inspect._empty:  # noqa
                             raise TypeError(
                                 f"The endpoint for the `{route.methods} {route.path}` "
                                 "route is missing a type annotation for the "
                                 f"`{param.name}` parameter. Please add a type "
                                 "annotation to the parameter to resolve this issue."
@@ -41,34 +42,38 @@
 
 
 def get_di(request: Request) -> pyxdi.PyxDI:
     return t.cast(pyxdi.PyxDI, request.app.state.di)
 
 
 class InjectParam(params.Depends):
-    def __init__(self) -> None:
+    def __init__(self, lazy: t.Optional[bool] = None) -> None:
         super().__init__(dependency=self._dependency, use_cache=True)
         self._interface: t.Any = None
+        self._lazy = lazy
 
     @property
     def interface(self) -> t.Any:
         if self._interface is None:
             raise TypeError("Interface is not set.")
         return self._interface
 
     @interface.setter
     def interface(self, val: t.Any) -> None:
         self._interface = val
 
     def _dependency(self, di: pyxdi.PyxDI = fastapi.Depends(get_di)) -> t.Any:
+        lazy = di.lazy_inject if self._lazy is None else self._lazy
+        if lazy:
+            return make_lazy(di.get, self.interface)
         return di.get(self.interface)
 
 
-def Inject() -> t.Any:  # noqa
-    return InjectParam()
+def Inject(*, lazy: t.Optional[bool] = None) -> t.Any:  # noqa
+    return InjectParam(lazy=lazy)
 
 
 def iter_dependencies(dependant: Dependant) -> t.Iterator[Dependant]:
     yield dependant
     if dependant.dependencies:
         for sub_dependant in dependant.dependencies:
             yield from iter_dependencies(sub_dependant)
```

### Comparing `pyxdi-0.6.3/pyxdi/ext/starlette/middleware.py` & `pyxdi-0.7.0/pyxdi/ext/starlette/middleware.py`

 * *Files identical despite different names*

### Comparing `pyxdi-0.6.3/PKG-INFO` & `pyxdi-0.7.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: pyxdi
-Version: 0.6.3
+Version: 0.7.0
 Summary: Dependency Injection library
 Home-page: https://github.com/antonrh/pyxdi
 License: MIT
 Keywords: dependency injection,dependencies,di,async,asyncio,application
 Author: Anton Ruhlov
 Author-email: antonruhlov@gmail.com
-Requires-Python: >=3.7,<3.12
+Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: all
 Provides-Extra: docs
-Requires-Dist: anyio (>=3.6.2,<4.0.0)
+Requires-Dist: anyio (>=3.6.2,<4.0.0) ; extra == "all"
+Requires-Dist: lazy-object-proxy (>=1.9.0,<2.0.0) ; extra == "all"
 Requires-Dist: mkdocs (>=1.4.2,<2.0.0) ; extra == "docs"
 Requires-Dist: mkdocs-material (>=9.0.12,<10.0.0) ; extra == "docs"
 Project-URL: Repository, https://github.com/antonrh/pyxdi
 Description-Content-Type: text/markdown
 
 # PyxDI
 
@@ -39,24 +40,33 @@
 
 ---
 
 ## Requirements
 
 Python 3.7+
 
-and requires [anyio](https://github.com/agronholm/anyio)
+and optional dependencies:
+
+* [anyio](https://github.com/agronholm/anyio) (for supporting synchronous resources with an asynchronous runtime)
+* [lazy-object-proxy](https://github.com/ionelmc/python-lazy-object-proxy) (for supporting lazy injections)
 
 ## Installation
 
 Install using `pip`:
 
 ```shell
 pip install pyxdi
 ```
 
+or with all dependencies (anyio, lazy-object-proxy)
+
+```shell
+pip install pyxdi[all]
+```
+
 or using `poetry`:
 
 ```shell
 poetry add pyxdi
 ```
 
 ## Quick Example
```

