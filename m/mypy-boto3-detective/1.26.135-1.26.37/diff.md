# Comparing `tmp/mypy-boto3-detective-1.26.135.tar.gz` & `tmp/mypy-boto3-detective-1.26.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-detective-1.26.135.tar", last modified: Tue May 16 19:32:46 2023, max compression
+gzip compressed data, was "mypy-boto3-detective-1.26.37.tar", last modified: Fri Dec 23 20:32:30 2022, max compression
```

## Comparing `mypy-boto3-detective-1.26.135.tar` & `mypy-boto3-detective-1.26.37.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:32:46.156726 mypy-boto3-detective-1.26.135/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-16 19:32:02.000000 mypy-boto3-detective-1.26.135/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14011 2023-05-16 19:32:46.152726 mypy-boto3-detective-1.26.135/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12514 2023-05-16 19:32:02.000000 mypy-boto3-detective-1.26.135/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:32:46.144725 mypy-boto3-detective-1.26.135/mypy_boto3_detective/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-16 19:32:02.000000 mypy-boto3-detective-1.26.135/mypy_boto3_detective/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-16 19:32:02.000000 mypy-boto3-detective-1.26.135/mypy_boto3_detective/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-16 19:32:02.000000 mypy-boto3-detective-1.26.135/mypy_boto3_detective/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16651 2023-05-16 19:32:03.000000 mypy-boto3-detective-1.26.135/mypy_boto3_detective/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16621 2023-05-16 19:32:02.000000 mypy-boto3-detective-1.26.135/mypy_boto3_detective/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8400 2023-05-16 19:32:03.000000 mypy-boto3-detective-1.26.135/mypy_boto3_detective/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8398 2023-05-16 19:32:03.000000 mypy-boto3-detective-1.26.135/mypy_boto3_detective/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 19:32:02.000000 mypy-boto3-detective-1.26.135/mypy_boto3_detective/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14268 2023-05-16 19:32:03.000000 mypy-boto3-detective-1.26.135/mypy_boto3_detective/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14259 2023-05-16 19:32:03.000000 mypy-boto3-detective-1.26.135/mypy_boto3_detective/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-16 19:32:02.000000 mypy-boto3-detective-1.26.135/mypy_boto3_detective/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:32:46.152726 mypy-boto3-detective-1.26.135/mypy_boto3_detective.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14011 2023-05-16 19:32:45.000000 mypy-boto3-detective-1.26.135/mypy_boto3_detective.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-16 19:32:46.000000 mypy-boto3-detective-1.26.135/mypy_boto3_detective.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 19:32:45.000000 mypy-boto3-detective-1.26.135/mypy_boto3_detective.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 19:32:45.000000 mypy-boto3-detective-1.26.135/mypy_boto3_detective.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-16 19:32:45.000000 mypy-boto3-detective-1.26.135/mypy_boto3_detective.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-16 19:32:45.000000 mypy-boto3-detective-1.26.135/mypy_boto3_detective.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 19:32:46.156726 mypy-boto3-detective-1.26.135/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-16 19:32:02.000000 mypy-boto3-detective-1.26.135/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 20:32:30.580941 mypy-boto3-detective-1.26.37/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-23 20:32:13.000000 mypy-boto3-detective-1.26.37/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14027 2022-12-23 20:32:30.580941 mypy-boto3-detective-1.26.37/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12532 2022-12-23 20:32:13.000000 mypy-boto3-detective-1.26.37/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 20:32:30.576941 mypy-boto3-detective-1.26.37/mypy_boto3_detective/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2022-12-23 20:32:13.000000 mypy-boto3-detective-1.26.37/mypy_boto3_detective/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2022-12-23 20:32:13.000000 mypy-boto3-detective-1.26.37/mypy_boto3_detective/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2022-12-23 20:32:13.000000 mypy-boto3-detective-1.26.37/mypy_boto3_detective/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16652 2022-12-23 20:32:13.000000 mypy-boto3-detective-1.26.37/mypy_boto3_detective/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16622 2022-12-23 20:32:13.000000 mypy-boto3-detective-1.26.37/mypy_boto3_detective/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8224 2022-12-23 20:32:13.000000 mypy-boto3-detective-1.26.37/mypy_boto3_detective/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8222 2022-12-23 20:32:13.000000 mypy-boto3-detective-1.26.37/mypy_boto3_detective/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-23 20:32:13.000000 mypy-boto3-detective-1.26.37/mypy_boto3_detective/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14268 2022-12-23 20:32:14.000000 mypy-boto3-detective-1.26.37/mypy_boto3_detective/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14259 2022-12-23 20:32:14.000000 mypy-boto3-detective-1.26.37/mypy_boto3_detective/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-23 20:32:13.000000 mypy-boto3-detective-1.26.37/mypy_boto3_detective/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 20:32:30.580941 mypy-boto3-detective-1.26.37/mypy_boto3_detective.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14027 2022-12-23 20:32:30.000000 mypy-boto3-detective-1.26.37/mypy_boto3_detective.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2022-12-23 20:32:30.000000 mypy-boto3-detective-1.26.37/mypy_boto3_detective.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-23 20:32:30.000000 mypy-boto3-detective-1.26.37/mypy_boto3_detective.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-23 20:32:30.000000 mypy-boto3-detective-1.26.37/mypy_boto3_detective.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-23 20:32:30.000000 mypy-boto3-detective-1.26.37/mypy_boto3_detective.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2022-12-23 20:32:30.000000 mypy-boto3-detective-1.26.37/mypy_boto3_detective.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-23 20:32:30.580941 mypy-boto3-detective-1.26.37/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2022-12-23 20:32:13.000000 mypy-boto3-detective-1.26.37/setup.py
```

### Comparing `mypy-boto3-detective-1.26.135/LICENSE` & `mypy-boto3-detective-1.26.37/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2022 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-detective-1.26.135/PKG-INFO` & `mypy-boto3-detective-1.26.37/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-detective
-Version: 1.26.135
-Summary: Type annotations for boto3.Detective 1.26.135 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.37
+Summary: Type annotations for boto3.Detective 1.26.37 service generated with mypy-boto3-builder 7.12.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_detective/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-detective"></a>
 
 # mypy-boto3-detective
 
 [![PyPI - mypy-boto3-detective](https://img.shields.io/pypi/v/mypy-boto3-detective.svg?color=blue)](https://pypi.org/project/mypy-boto3-detective)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-detective.svg?color=blue)](https://pypi.org/project/mypy-boto3-detective)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_detective/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-detective?color=blue)](https://pypistats.org/packages/mypy-boto3-detective)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Detective 1.26.135](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective)
+[boto3.Detective 1.26.37](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-detective docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_detective/).
 
 See how it helps to find and fix potential bugs:
 
@@ -362,42 +362,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-detective-1.26.135/README.md` & `mypy-boto3-detective-1.26.37/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-detective"></a>
 
 # mypy-boto3-detective
 
 [![PyPI - mypy-boto3-detective](https://img.shields.io/pypi/v/mypy-boto3-detective.svg?color=blue)](https://pypi.org/project/mypy-boto3-detective)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-detective.svg?color=blue)](https://pypi.org/project/mypy-boto3-detective)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_detective/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-detective?color=blue)](https://pypistats.org/packages/mypy-boto3-detective)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Detective 1.26.135](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective)
+[boto3.Detective 1.26.37](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-detective docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_detective/).
 
 See how it helps to find and fix potential bugs:
 
@@ -330,42 +330,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-detective-1.26.135/mypy_boto3_detective/client.py` & `mypy-boto3-detective-1.26.37/mypy_boto3_detective/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -290,15 +290,15 @@
         """
 
     def start_monitoring_member(
         self, *, GraphArn: str, AccountId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Sends a request to enable data ingest for a member account that has a status of
-        `ACCEPTED_BUT_DISABLED`.
+        `ACCEPTED_BUT_DISABLED` .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.start_monitoring_member)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_detective/client/#start_monitoring_member)
         """
 
     def tag_resource(self, *, ResourceArn: str, Tags: Mapping[str, str]) -> Dict[str, Any]:
         """
```

### Comparing `mypy-boto3-detective-1.26.135/mypy_boto3_detective/client.pyi` & `mypy-boto3-detective-1.26.37/mypy_boto3_detective/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -264,15 +264,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_detective/client/#reject_invitation)
         """
     def start_monitoring_member(
         self, *, GraphArn: str, AccountId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Sends a request to enable data ingest for a member account that has a status of
-        `ACCEPTED_BUT_DISABLED`.
+        `ACCEPTED_BUT_DISABLED` .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.start_monitoring_member)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_detective/client/#start_monitoring_member)
         """
     def tag_resource(self, *, ResourceArn: str, Tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Applies tag values to a behavior graph.
```

### Comparing `mypy-boto3-detective-1.26.135/mypy_boto3_detective/literals.py` & `mypy-boto3-detective-1.26.37/mypy_boto3_detective/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
 
 DatasourcePackageIngestStateType = Literal["DISABLED", "STARTED", "STOPPED"]
-DatasourcePackageType = Literal["ASFF_SECURITYHUB_FINDING", "DETECTIVE_CORE", "EKS_AUDIT"]
+DatasourcePackageType = Literal["DETECTIVE_CORE", "EKS_AUDIT"]
 InvitationTypeType = Literal["INVITATION", "ORGANIZATION"]
 MemberDisabledReasonType = Literal["VOLUME_TOO_HIGH", "VOLUME_UNKNOWN"]
 MemberStatusType = Literal[
     "ACCEPTED_BUT_DISABLED", "ENABLED", "INVITED", "VERIFICATION_FAILED", "VERIFICATION_IN_PROGRESS"
 ]
 DetectiveServiceName = Literal["detective"]
 ServiceName = Literal[
@@ -79,26 +79,24 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
-    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
-    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -184,15 +182,14 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
-    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -203,20 +200,18 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
-    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
     "kinesis-video-webrtc-storage",
     "kinesisanalytics",
@@ -273,15 +268,14 @@
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
-    "osis",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
@@ -363,20 +357,18 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
-    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-detective-1.26.135/mypy_boto3_detective/literals.pyi` & `mypy-boto3-detective-1.26.37/mypy_boto3_detective/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "DetectiveServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
 DatasourcePackageIngestStateType = Literal["DISABLED", "STARTED", "STOPPED"]
-DatasourcePackageType = Literal["ASFF_SECURITYHUB_FINDING", "DETECTIVE_CORE", "EKS_AUDIT"]
+DatasourcePackageType = Literal["DETECTIVE_CORE", "EKS_AUDIT"]
 InvitationTypeType = Literal["INVITATION", "ORGANIZATION"]
 MemberDisabledReasonType = Literal["VOLUME_TOO_HIGH", "VOLUME_UNKNOWN"]
 MemberStatusType = Literal[
     "ACCEPTED_BUT_DISABLED", "ENABLED", "INVITED", "VERIFICATION_FAILED", "VERIFICATION_IN_PROGRESS"
 ]
 DetectiveServiceName = Literal["detective"]
 ServiceName = Literal[
@@ -77,26 +77,24 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
-    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
-    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -182,15 +180,14 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
-    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -201,20 +198,18 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
-    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
     "kinesis-video-webrtc-storage",
     "kinesisanalytics",
@@ -271,15 +266,14 @@
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
-    "osis",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
@@ -361,20 +355,18 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
-    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-detective-1.26.135/mypy_boto3_detective/type_defs.py` & `mypy-boto3-detective-1.26.37/mypy_boto3_detective/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-detective-1.26.135/mypy_boto3_detective/type_defs.pyi` & `mypy-boto3-detective-1.26.37/mypy_boto3_detective/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-detective-1.26.135/mypy_boto3_detective.egg-info/PKG-INFO` & `mypy-boto3-detective-1.26.37/mypy_boto3_detective.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-detective
-Version: 1.26.135
-Summary: Type annotations for boto3.Detective 1.26.135 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.37
+Summary: Type annotations for boto3.Detective 1.26.37 service generated with mypy-boto3-builder 7.12.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_detective/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-detective"></a>
 
 # mypy-boto3-detective
 
 [![PyPI - mypy-boto3-detective](https://img.shields.io/pypi/v/mypy-boto3-detective.svg?color=blue)](https://pypi.org/project/mypy-boto3-detective)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-detective.svg?color=blue)](https://pypi.org/project/mypy-boto3-detective)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_detective/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-detective?color=blue)](https://pypistats.org/packages/mypy-boto3-detective)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Detective 1.26.135](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective)
+[boto3.Detective 1.26.37](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-detective docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_detective/).
 
 See how it helps to find and fix potential bugs:
 
@@ -362,42 +362,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-detective-1.26.135/mypy_boto3_detective.egg-info/SOURCES.txt` & `mypy-boto3-detective-1.26.37/mypy_boto3_detective.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-detective-1.26.135/setup.py` & `mypy-boto3-detective-1.26.37/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-detective.
 """
-from pathlib import Path
+from os.path import abspath, dirname
 
 from setuptools import setup
 
-LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
+LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-detective",
-    version="1.26.135",
+    version="1.26.37",
     packages=["mypy_boto3_detective"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Detective 1.26.135 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.Detective 1.26.37 service generated with mypy-boto3-builder"
+        " 7.12.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -45,11 +45,11 @@
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_detective/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        'typing-extensions>=4.1.0; python_version<"3.9"',
+        "typing-extensions>=4.1.0",
     ],
     zip_safe=False,
 )
```

