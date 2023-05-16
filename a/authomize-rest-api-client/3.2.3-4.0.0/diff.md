# Comparing `tmp/authomize-rest-api-client-3.2.3.tar.gz` & `tmp/authomize-rest-api-client-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authomize-rest-api-client-3.2.3.tar", last modified: Thu May 11 10:53:46 2023, max compression
+gzip compressed data, was "authomize-rest-api-client-4.0.0.tar", last modified: Tue May 16 10:03:20 2023, max compression
```

## Comparing `authomize-rest-api-client-3.2.3.tar` & `authomize-rest-api-client-4.0.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 10:53:46.145251 authomize-rest-api-client-3.2.3/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-05-11 10:53:10.000000 authomize-rest-api-client-3.2.3/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      134 2023-05-11 10:53:10.000000 authomize-rest-api-client-3.2.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      251 2023-05-11 10:53:46.145251 authomize-rest-api-client-3.2.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2160 2023-05-11 10:53:10.000000 authomize-rest-api-client-3.2.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 10:53:46.141251 authomize-rest-api-client-3.2.3/authomize/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 10:53:46.141251 authomize-rest-api-client-3.2.3/authomize/rest_api_client/
--rw-r--r--   0 root         (0) root         (0)      627 2023-05-11 10:53:10.000000 authomize-rest-api-client-3.2.3/authomize/rest_api_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 10:53:46.141251 authomize-rest-api-client-3.2.3/authomize/rest_api_client/client/
--rw-r--r--   0 root         (0) root         (0)       81 2023-05-11 10:53:10.000000 authomize-rest-api-client-3.2.3/authomize/rest_api_client/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2631 2023-05-11 10:53:10.000000 authomize-rest-api-client-3.2.3/authomize/rest_api_client/client/base_client.py
--rw-r--r--   0 root         (0) root         (0)    10105 2023-05-11 10:53:10.000000 authomize-rest-api-client-3.2.3/authomize/rest_api_client/client/client.py
--rw-r--r--   0 root         (0) root         (0)    12633 2023-05-11 10:53:10.000000 authomize-rest-api-client-3.2.3/authomize/rest_api_client/client/connectors_client.py
--rw-r--r--   0 root         (0) root         (0)     1102 2023-05-11 10:53:10.000000 authomize-rest-api-client-3.2.3/authomize/rest_api_client/client/platform_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 10:53:46.141251 authomize-rest-api-client-3.2.3/authomize/rest_api_client/configuration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 10:53:10.000000 authomize-rest-api-client-3.2.3/authomize/rest_api_client/configuration/__init__.py
--rw-r--r--   0 root         (0) root         (0)      330 2023-05-11 10:53:10.000000 authomize-rest-api-client-3.2.3/authomize/rest_api_client/configuration/authomize_api_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 10:53:46.141251 authomize-rest-api-client-3.2.3/authomize/rest_api_client/generated/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 10:53:10.000000 authomize-rest-api-client-3.2.3/authomize/rest_api_client/generated/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 10:53:46.141251 authomize-rest-api-client-3.2.3/authomize/rest_api_client/generated/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 10:53:10.000000 authomize-rest-api-client-3.2.3/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    73614 2023-05-11 10:53:10.000000 authomize-rest-api-client-3.2.3/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 10:53:46.141251 authomize-rest-api-client-3.2.3/authomize/rest_api_client/generated/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 10:53:10.000000 authomize-rest-api-client-3.2.3/authomize/rest_api_client/generated/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24509 2023-05-11 10:53:10.000000 authomize-rest-api-client-3.2.3/authomize/rest_api_client/generated/external_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 10:53:46.145251 authomize-rest-api-client-3.2.3/authomize/rest_api_client/openapi/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 10:53:10.000000 authomize-rest-api-client-3.2.3/authomize/rest_api_client/openapi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 10:53:46.145251 authomize-rest-api-client-3.2.3/authomize/rest_api_client/openapi/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 10:53:10.000000 authomize-rest-api-client-3.2.3/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)   185721 2023-05-11 10:53:10.000000 authomize-rest-api-client-3.2.3/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 10:53:46.145251 authomize-rest-api-client-3.2.3/authomize/rest_api_client/openapi/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 10:53:10.000000 authomize-rest-api-client-3.2.3/authomize/rest_api_client/openapi/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    64900 2023-05-11 10:53:10.000000 authomize-rest-api-client-3.2.3/authomize/rest_api_client/openapi/external_rest_api/openapi.json
--rw-r--r--   0 root         (0) root         (0)       26 2023-05-11 10:53:10.000000 authomize-rest-api-client-3.2.3/authomize/rest_api_client/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 10:53:46.145251 authomize-rest-api-client-3.2.3/authomize_rest_api_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      251 2023-05-11 10:53:46.000000 authomize-rest-api-client-3.2.3/authomize_rest_api_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1356 2023-05-11 10:53:46.000000 authomize-rest-api-client-3.2.3/authomize_rest_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 10:53:46.000000 authomize-rest-api-client-3.2.3/authomize_rest_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      214 2023-05-11 10:53:46.000000 authomize-rest-api-client-3.2.3/authomize_rest_api_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-11 10:53:46.000000 authomize-rest-api-client-3.2.3/authomize_rest_api_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      336 2023-05-11 10:53:46.145251 authomize-rest-api-client-3.2.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1161 2023-05-11 10:53:44.000000 authomize-rest-api-client-3.2.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:03:20.656275 authomize-rest-api-client-4.0.0/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-05-16 10:02:55.000000 authomize-rest-api-client-4.0.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      134 2023-05-16 10:02:55.000000 authomize-rest-api-client-4.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      251 2023-05-16 10:03:20.656275 authomize-rest-api-client-4.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2160 2023-05-16 10:02:55.000000 authomize-rest-api-client-4.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:03:20.652275 authomize-rest-api-client-4.0.0/authomize/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:03:20.652275 authomize-rest-api-client-4.0.0/authomize/rest_api_client/
+-rw-r--r--   0 root         (0) root         (0)      627 2023-05-16 10:02:55.000000 authomize-rest-api-client-4.0.0/authomize/rest_api_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:03:20.652275 authomize-rest-api-client-4.0.0/authomize/rest_api_client/client/
+-rw-r--r--   0 root         (0) root         (0)       81 2023-05-16 10:02:55.000000 authomize-rest-api-client-4.0.0/authomize/rest_api_client/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2631 2023-05-16 10:02:55.000000 authomize-rest-api-client-4.0.0/authomize/rest_api_client/client/base_client.py
+-rw-r--r--   0 root         (0) root         (0)    10105 2023-05-16 10:02:55.000000 authomize-rest-api-client-4.0.0/authomize/rest_api_client/client/client.py
+-rw-r--r--   0 root         (0) root         (0)    12633 2023-05-16 10:02:55.000000 authomize-rest-api-client-4.0.0/authomize/rest_api_client/client/connectors_client.py
+-rw-r--r--   0 root         (0) root         (0)     1102 2023-05-16 10:02:55.000000 authomize-rest-api-client-4.0.0/authomize/rest_api_client/client/platform_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:03:20.652275 authomize-rest-api-client-4.0.0/authomize/rest_api_client/configuration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 10:02:55.000000 authomize-rest-api-client-4.0.0/authomize/rest_api_client/configuration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      330 2023-05-16 10:02:55.000000 authomize-rest-api-client-4.0.0/authomize/rest_api_client/configuration/authomize_api_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:03:20.652275 authomize-rest-api-client-4.0.0/authomize/rest_api_client/generated/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 10:02:55.000000 authomize-rest-api-client-4.0.0/authomize/rest_api_client/generated/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:03:20.656275 authomize-rest-api-client-4.0.0/authomize/rest_api_client/generated/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 10:02:55.000000 authomize-rest-api-client-4.0.0/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    73614 2023-05-16 10:02:55.000000 authomize-rest-api-client-4.0.0/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:03:20.656275 authomize-rest-api-client-4.0.0/authomize/rest_api_client/generated/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 10:02:55.000000 authomize-rest-api-client-4.0.0/authomize/rest_api_client/generated/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24501 2023-05-16 10:02:55.000000 authomize-rest-api-client-4.0.0/authomize/rest_api_client/generated/external_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:03:20.656275 authomize-rest-api-client-4.0.0/authomize/rest_api_client/openapi/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 10:02:55.000000 authomize-rest-api-client-4.0.0/authomize/rest_api_client/openapi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:03:20.656275 authomize-rest-api-client-4.0.0/authomize/rest_api_client/openapi/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 10:02:55.000000 authomize-rest-api-client-4.0.0/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   185721 2023-05-16 10:02:55.000000 authomize-rest-api-client-4.0.0/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:03:20.656275 authomize-rest-api-client-4.0.0/authomize/rest_api_client/openapi/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 10:02:55.000000 authomize-rest-api-client-4.0.0/authomize/rest_api_client/openapi/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    65008 2023-05-16 10:02:55.000000 authomize-rest-api-client-4.0.0/authomize/rest_api_client/openapi/external_rest_api/openapi.json
+-rw-r--r--   0 root         (0) root         (0)       26 2023-05-16 10:02:55.000000 authomize-rest-api-client-4.0.0/authomize/rest_api_client/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:03:20.656275 authomize-rest-api-client-4.0.0/authomize_rest_api_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      251 2023-05-16 10:03:20.000000 authomize-rest-api-client-4.0.0/authomize_rest_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1356 2023-05-16 10:03:20.000000 authomize-rest-api-client-4.0.0/authomize_rest_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 10:03:20.000000 authomize-rest-api-client-4.0.0/authomize_rest_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      214 2023-05-16 10:03:20.000000 authomize-rest-api-client-4.0.0/authomize_rest_api_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-16 10:03:20.000000 authomize-rest-api-client-4.0.0/authomize_rest_api_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      336 2023-05-16 10:03:20.656275 authomize-rest-api-client-4.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1161 2023-05-16 10:03:19.000000 authomize-rest-api-client-4.0.0/setup.py
```

### Comparing `authomize-rest-api-client-3.2.3/LICENSE.txt` & `authomize-rest-api-client-4.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.2.3/README.md` & `authomize-rest-api-client-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.2.3/authomize/rest_api_client/__init__.py` & `authomize-rest-api-client-4.0.0/authomize/rest_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.2.3/authomize/rest_api_client/client/base_client.py` & `authomize-rest-api-client-4.0.0/authomize/rest_api_client/client/base_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.2.3/authomize/rest_api_client/client/client.py` & `authomize-rest-api-client-4.0.0/authomize/rest_api_client/client/client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.2.3/authomize/rest_api_client/client/connectors_client.py` & `authomize-rest-api-client-4.0.0/authomize/rest_api_client/client/connectors_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.2.3/authomize/rest_api_client/client/platform_client.py` & `authomize-rest-api-client-4.0.0/authomize/rest_api_client/client/platform_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.2.3/authomize/rest_api_client/generated/connectors_rest_api/schemas.py` & `authomize-rest-api-client-4.0.0/authomize/rest_api_client/generated/connectors_rest_api/schemas.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.2.3/authomize/rest_api_client/generated/external_rest_api/schemas.py` & `authomize-rest-api-client-4.0.0/authomize/rest_api_client/generated/external_rest_api/schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  openapi.json
-#   timestamp: 2023-05-10T16:13:43+00:00
+#   timestamp: 2023-05-16T09:37:39+00:00
 
 from __future__ import annotations
 
 from datetime import datetime
 from enum import Enum
 from typing import List, Optional, Union
 
@@ -94,15 +94,15 @@
 
 
 class CampaignStatusFilter(BaseModel):
     class Config:
         extra = Extra.forbid
 
     field_in: Optional[List[CampaignStatus]] = Field(
-        default=None, alias='$in', description='In'
+        default=[], alias='$in', description='In'
     )
 
 
 class Ccm301Standard(Enum):
     AIS_04 = 'AIS-04'
     IAM_01 = 'IAM-01'
     IAM_02 = 'IAM-02'
@@ -256,15 +256,15 @@
 
 
 class IncidentsStatusFilter(BaseModel):
     class Config:
         extra = Extra.forbid
 
     field_in: Optional[List[EventStatusType]] = Field(
-        default=None, alias='$in', description='In'
+        default=[], alias='$in', description='In'
     )
 
 
 class IncidentsUpdatedAtFilter(BaseModel):
     class Config:
         extra = Extra.forbid
 
@@ -317,15 +317,15 @@
     A_8_2_3 = 'A.8.2.3'
     A_7_3_1 = 'A.7.3.1'
     A_8_1_4 = 'A.8.1.4'
 
 
 class MeResponse(BaseModel):
     version: Optional[str] = Field(
-        default='3.2.1', description='**version**', title='Version'
+        default='4.0.0', description='**version**', title='Version'
     )
     id: str = Field(..., description='**id**', title='Id')
     tenant: str = Field(..., description='**tenant**', title='Tenant')
 
 
 class NonPaginatedResponseSchemaCommentSchema(BaseModel):
     class Config:
@@ -474,15 +474,15 @@
 
 
 class CampaignPermissionDecisionFilter(BaseModel):
     class Config:
         extra = Extra.forbid
 
     field_in: Optional[List[Selection]] = Field(
-        default=None, alias='$in', description='In'
+        default=[], alias='$in', description='In'
     )
 
 
 class CampaignPermissionsSearchFilterBody(BaseModel):
     class Config:
         extra = Extra.forbid
 
@@ -563,15 +563,15 @@
 
 
 class IncidentsSeverityFilter(BaseModel):
     class Config:
         extra = Extra.forbid
 
     field_in: Optional[List[SeverityType]] = Field(
-        default=None, alias='$in', description='In'
+        default=[], alias='$in', description='In'
     )
 
 
 class IsoIec27001(BaseModel):
     values: List[IsoIec27001Standard] = Field(..., description='Values')
     id: Optional[str] = Field(default='isoIec27001', description='UniqueID', title='Id')
     name: Optional[str] = Field(
```

### Comparing `authomize-rest-api-client-3.2.3/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json` & `authomize-rest-api-client-4.0.0/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.2.3/authomize/rest_api_client/openapi/external_rest_api/openapi.json` & `authomize-rest-api-client-4.0.0/authomize/rest_api_client/openapi/external_rest_api/openapi.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9874880323223039%*

 * *Differences: {"'components'": "{'schemas': {'CampaignPermissionDecisionFilter': {'properties': {'$in': "*

 * *                 "{'default': []}}}, 'CampaignStatusFilter': {'properties': {'$in': {'default': "*

 * *                 "[]}}}, 'IncidentsSeverityFilter': {'properties': {'$in': {'default': []}}}, "*

 * *                 "'IncidentsStatusFilter': {'properties': {'$in': {'default': []}}}, 'MeResponse': "*

 * *                 "{'properties': {'version': {'default': '4.0.0'}}}}}",*

 * * "'info'": "{'version': '4.0.0'}"}*

```diff
@@ -130,14 +130,15 @@
                 "title": "CampaignExpansion",
                 "type": "string"
             },
             "CampaignPermissionDecisionFilter": {
                 "additionalProperties": false,
                 "properties": {
                     "$in": {
+                        "default": [],
                         "description": "In",
                         "items": {
                             "$ref": "#/components/schemas/Selection"
                         },
                         "type": "array"
                     }
                 },
@@ -257,14 +258,15 @@
                 ],
                 "title": "CampaignStatus"
             },
             "CampaignStatusFilter": {
                 "additionalProperties": false,
                 "properties": {
                     "$in": {
+                        "default": [],
                         "description": "In",
                         "items": {
                             "$ref": "#/components/schemas/CampaignStatus"
                         },
                         "type": "array"
                     }
                 },
@@ -858,28 +860,30 @@
                 "title": "IncidentsPolicyTempalteIdFilter",
                 "type": "object"
             },
             "IncidentsSeverityFilter": {
                 "additionalProperties": false,
                 "properties": {
                     "$in": {
+                        "default": [],
                         "description": "In",
                         "items": {
                             "$ref": "#/components/schemas/SeverityType"
                         },
                         "type": "array"
                     }
                 },
                 "title": "IncidentsSeverityFilter",
                 "type": "object"
             },
             "IncidentsStatusFilter": {
                 "additionalProperties": false,
                 "properties": {
                     "$in": {
+                        "default": [],
                         "description": "In",
                         "items": {
                             "$ref": "#/components/schemas/EventStatusType"
                         },
                         "type": "array"
                     }
                 },
@@ -1005,15 +1009,15 @@
                     },
                     "tenant": {
                         "description": "**tenant**",
                         "title": "Tenant",
                         "type": "string"
                     },
                     "version": {
-                        "default": "3.2.1",
+                        "default": "4.0.0",
                         "description": "**version**",
                         "title": "Version",
                         "type": "string"
                     }
                 },
                 "required": [
                     "id",
@@ -1734,15 +1738,15 @@
                 "type": "apiKey"
             }
         }
     },
     "info": {
         "description": "Authomize enables users to integrate your applications with Authomize via custom connectors.\n\nYou can use the APIs described in this document to create your connector.\n\nOnce data is uploaded and processed successfully, your custom connector will function in the same way as the connectors created by Authomize.\n\n## How does Authomize work?\nAuthomize works by gathering information about:\n\n\u00b7 individuals, teams and functions.\n\n\u00b7 apps, assets and accounts.\n\n\u00b7 all the relationships between them.\n\n![img.png](https://storagetry1.blob.core.windows.net/public/78d82650-71b0-4909-8444-022aab79add5.png)\n\n## Connector APIs\n\nAuthomize connector APIs enable pushing data into Authomize from external sources.\n\nThese APIs enable data extracted from outside applications (via application APIs) to be delivered to Authomize.\n\nA connector processes extracted application data to transform it into a format compatible with Authomize.\n\n![img_1.png](https://storagetry1.blob.core.windows.net/public/341bf6ef-2e5b-4284-b715-45105ffbf0f8.png)\n\n## Authentication\nTo Authenticate use the API Token, with the format: `Authorization: API_Token`.\n\nAn API Token is a token you provide when making API calls. \n\n\nThe API Token should be included in every request to the API in an `Authorization` header.\n```\ncurl -v -X POST \\n\n     -H \"Authorization: {API_Token}\" \\n\n     ...\n```\n\n## Limits\nRequests cannot exceed a size of 1MB.\n",
         "title": "Authomize API Reference",
-        "version": "3.2.1",
+        "version": "4.0.0",
         "x-logo": {
             "url": "https://static.authomize.com/public/icons/authomize-green.svg"
         }
     },
     "openapi": "3.0.2",
     "paths": {
         "/is_alive": {
```

### Comparing `authomize-rest-api-client-3.2.3/authomize_rest_api_client.egg-info/SOURCES.txt` & `authomize-rest-api-client-4.0.0/authomize_rest_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.2.3/setup.py` & `authomize-rest-api-client-4.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == '__main__':
     setup(
-        version='3.2.3',
+        version='4.0.0',
         name='authomize-rest-api-client',
         author='Authomize inc.',
         license='MIT',
         author_email='info@authomize.com',
         description='Authomize REST API Python Client',
         packages=find_namespace_packages(include=['authomize.*']),
         package_data={
```

