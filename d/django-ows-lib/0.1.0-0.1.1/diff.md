# Comparing `tmp/django-ows-lib-0.1.0.tar.gz` & `tmp/django-ows-lib-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-ows-lib-0.1.0.tar", last modified: Mon May 15 09:59:35 2023, max compression
+gzip compressed data, was "django-ows-lib-0.1.1.tar", last modified: Mon May 15 12:51:34 2023, max compression
```

## Comparing `django-ows-lib-0.1.0.tar` & `django-ows-lib-0.1.1.tar`

### file list

```diff
@@ -1,77 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:35.271652 django-ows-lib-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-15 09:59:35.271652 django-ows-lib-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:35.267652 django-ows-lib-0.1.0/django_ows_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-15 09:59:35.000000 django-ows-lib-0.1.0/django_ows_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-15 09:59:35.000000 django-ows-lib-0.1.0/django_ows_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 09:59:35.000000 django-ows-lib-0.1.0/django_ows_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-15 09:59:35.000000 django-ows-lib-0.1.0/django_ows_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 09:59:35.000000 django-ows-lib-0.1.0/django_ows_lib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:35.267652 django-ows-lib-0.1.0/ows_lib/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/ows_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:35.267652 django-ows-lib-0.1.0/ows_lib/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/ows_lib/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:35.267652 django-ows-lib-0.1.0/ows_lib/client/csw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/ows_lib/client/csw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/ows_lib/client/csw/csw202.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/ows_lib/client/csw/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/ows_lib/client/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/ows_lib/client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/ows_lib/client/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    10393 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/ows_lib/client/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:35.267652 django-ows-lib-0.1.0/ows_lib/client/wfs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/ows_lib/client/wfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/ows_lib/client/wfs/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/ows_lib/client/wfs/wfs200.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:35.267652 django-ows-lib-0.1.0/ows_lib/client/wms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/ows_lib/client/wms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/ows_lib/client/wms/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/ows_lib/client/wms/wms111.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/ows_lib/client/wms/wms130.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:35.267652 django-ows-lib-0.1.0/ows_lib/models/
--rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/ows_lib/models/ogc_request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:35.271652 django-ows-lib-0.1.0/ows_lib/xml_mapper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/ows_lib/xml_mapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:35.271652 django-ows-lib-0.1.0/ows_lib/xml_mapper/capabilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/ows_lib/xml_mapper/capabilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:35.271652 django-ows-lib-0.1.0/ows_lib/xml_mapper/capabilities/csw/
--rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/ows_lib/xml_mapper/capabilities/csw/csw202.py
--rw-r--r--   0 runner    (1001) docker     (123)    10682 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/ows_lib/xml_mapper/capabilities/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:35.271652 django-ows-lib-0.1.0/ows_lib/xml_mapper/capabilities/wfs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/ows_lib/xml_mapper/capabilities/wfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/ows_lib/xml_mapper/capabilities/wfs/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     9680 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/ows_lib/xml_mapper/capabilities/wfs/wfs200.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:35.271652 django-ows-lib-0.1.0/ows_lib/xml_mapper/capabilities/wms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/ows_lib/xml_mapper/capabilities/wms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10451 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/ows_lib/xml_mapper/capabilities/wms/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/ows_lib/xml_mapper/capabilities/wms/wms111.py
--rw-r--r--   0 runner    (1001) docker     (123)     9336 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/ows_lib/xml_mapper/capabilities/wms/wms130.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/ows_lib/xml_mapper/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:35.271652 django-ows-lib-0.1.0/ows_lib/xml_mapper/gml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/ows_lib/xml_mapper/gml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/ows_lib/xml_mapper/gml/gml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:35.271652 django-ows-lib-0.1.0/ows_lib/xml_mapper/iso_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/ows_lib/xml_mapper/iso_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16776 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/ows_lib/xml_mapper/iso_metadata/iso_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/ows_lib/xml_mapper/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/ows_lib/xml_mapper/namespaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/ows_lib/xml_mapper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:35.271652 django-ows-lib-0.1.0/ows_lib/xml_mapper/xml_requests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/ows_lib/xml_mapper/xml_requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/ows_lib/xml_mapper/xml_requests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:35.271652 django-ows-lib-0.1.0/ows_lib/xml_mapper/xml_requests/wfs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/ows_lib/xml_mapper/xml_requests/wfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/ows_lib/xml_mapper/xml_requests/wfs/get_feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:35.271652 django-ows-lib-0.1.0/ows_lib/xml_mapper/xml_responses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/ows_lib/xml_mapper/xml_responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/ows_lib/xml_mapper/xml_responses/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:35.271652 django-ows-lib-0.1.0/ows_lib/xml_mapper/xml_responses/csw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/ows_lib/xml_mapper/xml_responses/csw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/ows_lib/xml_mapper/xml_responses/csw/get_records.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:35.271652 django-ows-lib-0.1.0/ows_lib/xml_mapper/xml_responses/wfs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/ows_lib/xml_mapper/xml_responses/wfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/ows_lib/xml_mapper/xml_responses/wfs/describe_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/ows_lib/xml_mapper/xml_responses/wfs/feature_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 09:59:35.271652 django-ows-lib-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-15 09:59:34.000000 django-ows-lib-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:51:34.086248 django-ows-lib-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-15 12:51:34.086248 django-ows-lib-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:51:34.082248 django-ows-lib-0.1.1/django_ows_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-15 12:51:34.000000 django-ows-lib-0.1.1/django_ows_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-15 12:51:34.000000 django-ows-lib-0.1.1/django_ows_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 12:51:34.000000 django-ows-lib-0.1.1/django_ows_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-15 12:51:34.000000 django-ows-lib-0.1.1/django_ows_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 12:51:34.000000 django-ows-lib-0.1.1/django_ows_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:51:34.082248 django-ows-lib-0.1.1/ows_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:51:34.082248 django-ows-lib-0.1.1/ows_lib/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:51:34.082248 django-ows-lib-0.1.1/ows_lib/client/csw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/client/csw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/client/csw/csw202.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/client/csw/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/client/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/client/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10353 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/client/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:51:34.082248 django-ows-lib-0.1.1/ows_lib/client/wfs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/client/wfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/client/wfs/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/client/wfs/wfs200.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:51:34.082248 django-ows-lib-0.1.1/ows_lib/client/wms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/client/wms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/client/wms/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/client/wms/wms111.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/client/wms/wms130.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:51:34.082248 django-ows-lib-0.1.1/ows_lib/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/models/ogc_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:51:34.082248 django-ows-lib-0.1.1/ows_lib/xml_mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/xml_mapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:51:34.082248 django-ows-lib-0.1.1/ows_lib/xml_mapper/capabilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/xml_mapper/capabilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:51:34.082248 django-ows-lib-0.1.1/ows_lib/xml_mapper/capabilities/csw/
+-rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/xml_mapper/capabilities/csw/csw202.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/xml_mapper/capabilities/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:51:34.082248 django-ows-lib-0.1.1/ows_lib/xml_mapper/capabilities/wfs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/xml_mapper/capabilities/wfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/xml_mapper/capabilities/wfs/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9680 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/xml_mapper/capabilities/wfs/wfs200.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:51:34.082248 django-ows-lib-0.1.1/ows_lib/xml_mapper/capabilities/wms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/xml_mapper/capabilities/wms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/xml_mapper/capabilities/wms/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/xml_mapper/capabilities/wms/wms111.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9336 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/xml_mapper/capabilities/wms/wms130.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/xml_mapper/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/xml_mapper/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:51:34.082248 django-ows-lib-0.1.1/ows_lib/xml_mapper/gml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/xml_mapper/gml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/xml_mapper/gml/gml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:51:34.082248 django-ows-lib-0.1.1/ows_lib/xml_mapper/iso_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/xml_mapper/iso_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16896 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/xml_mapper/iso_metadata/iso_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/xml_mapper/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/xml_mapper/namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/xml_mapper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:51:34.082248 django-ows-lib-0.1.1/ows_lib/xml_mapper/xml_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/xml_mapper/xml_requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/xml_mapper/xml_requests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:51:34.082248 django-ows-lib-0.1.1/ows_lib/xml_mapper/xml_requests/wfs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/xml_mapper/xml_requests/wfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8615 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/xml_mapper/xml_requests/wfs/get_feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:51:34.082248 django-ows-lib-0.1.1/ows_lib/xml_mapper/xml_responses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/xml_mapper/xml_responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/xml_mapper/xml_responses/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:51:34.082248 django-ows-lib-0.1.1/ows_lib/xml_mapper/xml_responses/csw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/xml_mapper/xml_responses/csw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/xml_mapper/xml_responses/csw/get_records.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:51:34.082248 django-ows-lib-0.1.1/ows_lib/xml_mapper/xml_responses/wfs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/xml_mapper/xml_responses/wfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/xml_mapper/xml_responses/wfs/describe_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/ows_lib/xml_mapper/xml_responses/wfs/feature_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 12:51:34.086248 django-ows-lib-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-15 12:51:33.000000 django-ows-lib-0.1.1/setup.py
```

### Comparing `django-ows-lib-0.1.0/LICENSE` & `django-ows-lib-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.1.0/PKG-INFO` & `django-ows-lib-0.1.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ows-lib
-Version: 0.1.0
+Version: 0.1.1
 Summary: Well layered ows lib with a client implementation to communicate with ogc services with django based objects, including xml mapper classes to serialize and deserialize ows xml files, such as capabilities.
 Home-page: https://github.com/mrmap-community/django-ows-lib
 Author: mrmap-community
 Author-email: jonas.kiefer@live.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -28,14 +28,24 @@
     :target: https://django-ows-lib.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 .. image:: https://badge.fury.io/py/django-ows-lib.svg
     :target: https://pypi.org/project/django-ows-lib/
     :alt: PyPi version
 
+.. image:: https://sonarcloud.io/api/project_badges/measure?project=mrmap-community_django-ows-lib&metric=coverage
+    :target: https://sonarcloud.io/project/overview?id=mrmap-community_django-ows-lib
+    :alt: Coverage
+
+.. image:: https://sonarcloud.io/api/project_badges/measure?project=mrmap-community_django-ows-lib&metric=alert_status
+    :target: https://sonarcloud.io/project/overview?id=mrmap-community_django-ows-lib
+    :alt: Quality Gate
+
+
+
 django-ows-lib
 ==============
 
 Well layered ows lib with a client implementation to communicate with ogc services with django based objects, 
 including xml mapper classes to serialize and deserialize ows xml files, such as capabilities.
 
 Features
```

### Comparing `django-ows-lib-0.1.0/django_ows_lib.egg-info/PKG-INFO` & `django-ows-lib-0.1.1/django_ows_lib.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ows-lib
-Version: 0.1.0
+Version: 0.1.1
 Summary: Well layered ows lib with a client implementation to communicate with ogc services with django based objects, including xml mapper classes to serialize and deserialize ows xml files, such as capabilities.
 Home-page: https://github.com/mrmap-community/django-ows-lib
 Author: mrmap-community
 Author-email: jonas.kiefer@live.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -28,14 +28,24 @@
     :target: https://django-ows-lib.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 .. image:: https://badge.fury.io/py/django-ows-lib.svg
     :target: https://pypi.org/project/django-ows-lib/
     :alt: PyPi version
 
+.. image:: https://sonarcloud.io/api/project_badges/measure?project=mrmap-community_django-ows-lib&metric=coverage
+    :target: https://sonarcloud.io/project/overview?id=mrmap-community_django-ows-lib
+    :alt: Coverage
+
+.. image:: https://sonarcloud.io/api/project_badges/measure?project=mrmap-community_django-ows-lib&metric=alert_status
+    :target: https://sonarcloud.io/project/overview?id=mrmap-community_django-ows-lib
+    :alt: Quality Gate
+
+
+
 django-ows-lib
 ==============
 
 Well layered ows lib with a client implementation to communicate with ogc services with django based objects, 
 including xml mapper classes to serialize and deserialize ows xml files, such as capabilities.
 
 Features
```

### Comparing `django-ows-lib-0.1.0/django_ows_lib.egg-info/SOURCES.txt` & `django-ows-lib-0.1.1/django_ows_lib.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 ows_lib/client/wfs/wfs200.py
 ows_lib/client/wms/__init__.py
 ows_lib/client/wms/mixins.py
 ows_lib/client/wms/wms111.py
 ows_lib/client/wms/wms130.py
 ows_lib/models/ogc_request.py
 ows_lib/xml_mapper/__init__.py
+ows_lib/xml_mapper/consts.py
 ows_lib/xml_mapper/exceptions.py
 ows_lib/xml_mapper/mixins.py
 ows_lib/xml_mapper/namespaces.py
 ows_lib/xml_mapper/utils.py
 ows_lib/xml_mapper/capabilities/__init__.py
 ows_lib/xml_mapper/capabilities/mixins.py
 ows_lib/xml_mapper/capabilities/csw/csw202.py
```

### Comparing `django-ows-lib-0.1.0/ows_lib/client/csw/mixins.py` & `django-ows-lib-0.1.1/ows_lib/client/csw/mixins.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.1.0/ows_lib/client/enums.py` & `django-ows-lib-0.1.1/ows_lib/client/enums.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.1.0/ows_lib/client/exceptions.py` & `django-ows-lib-0.1.1/ows_lib/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.1.0/ows_lib/client/mixins.py` & `django-ows-lib-0.1.1/ows_lib/client/mixins.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.1.0/ows_lib/client/utils.py` & `django-ows-lib-0.1.1/ows_lib/client/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     * The coordinate reference system of the bbox by default is WGS84 (EPSG:4326). IF the bbox param provides a
     crsuri value this coordinate reference system shall be used instead.
 
     :return: the bbox parsed from the get_dict or an empty polygon if something went wrong.
     :rtype: :class:`django.contrib.gis.geos.polygon.Polygon`
     """
     try:
-        major_version, minor_version, fix_version = get_dict["version"].split(
+        major_version, minor_version, _ = get_dict["version"].split(
             ".")
         major_version = int(major_version)
         minor_version = int(minor_version)
         bbox = get_dict["bbox"]
         srid = get_dict.get("srs", None)
         if not srid:
             srid = get_dict.get("srsname", None)
@@ -61,15 +61,15 @@
             max_y = float(max_y)
         else:
             bbox_values = bbox.split(",")
             registry = Registry()
             if len(bbox_values) == 4:
                 epsg_sr = registry.get(srid=4326)
             elif len(bbox_values) == 5:
-                authority, srid = get_epsg_srid(bbox_values[4])
+                _, srid = get_epsg_srid(bbox_values[4])
                 epsg_sr = registry.get(srid=srid)
             else:
                 raise NotImplementedError(
                     "multiple dimension crs is not implemented.")
             min_x = float(bbox_values[0])
             min_y = float(bbox_values[1])
             max_x = float(bbox_values[2])
@@ -110,15 +110,15 @@
         * **OGC WMS 1.3.0**: EXAMPLE EPSG:4326 refers to WGS 84 geographic latitude, then longitude. That is, in
             this CRS the x axis corresponds to latitude, and the y axis to longitude. (see 6.7.3.3)
 
     :return: the bbox parsed from the get_dict or an empty polygon if something went wrong.
     :rtype: :class:`django.contrib.gis.geos.polygon.Polygon`
     """
     try:
-        major_version, minor_version, fix_version = get_dict["version"].split(
+        _, minor_version, _ = get_dict["version"].split(
             ".")
         minor_version = int(minor_version)
         srid = get_dict.get("srs", None)
         if not srid:
             srid = get_dict.get("crs", None)
             if not srid:
                 raise MissingCrsParam
```

### Comparing `django-ows-lib-0.1.0/ows_lib/client/wfs/mixins.py` & `django-ows-lib-0.1.1/ows_lib/client/wfs/mixins.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.1.0/ows_lib/client/wms/mixins.py` & `django-ows-lib-0.1.1/ows_lib/client/wms/mixins.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.1.0/ows_lib/models/ogc_request.py` & `django-ows-lib-0.1.1/ows_lib/models/ogc_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,15 +194,16 @@
         This function analyzes the given request by its method and operation. 
         If it is a get request, the get feature operation for example will be converted to an postable xml object.
 
         :return: The mapped xml object
         :rtype: XmlObject
         """
         if not self._xml_request:
-            if self.is_get_feature_request:
+            # TODO: implement the xml request generation for other requests too.
+            if self.is_get_feature_request:  # NOSONAR: See todo above
                 # FIXME: depending on version, different xml mapper are needed...
                 if self.is_post:
                     self._xml_request: GetFeatureRequest = load_xmlobject_from_string(
                         string=self.data, xmlclass=GetFeatureRequest)
                 elif self.is_get:
                     # we construct a xml get feature request to post it with a filter
                     queries: List[Query] = []
```

### Comparing `django-ows-lib-0.1.0/ows_lib/xml_mapper/capabilities/csw/csw202.py` & `django-ows-lib-0.1.1/ows_lib/xml_mapper/capabilities/csw/csw202.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.1.0/ows_lib/xml_mapper/capabilities/mixins.py` & `django-ows-lib-0.1.1/ows_lib/xml_mapper/capabilities/mixins.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,15 +165,15 @@
     def name(self, value: str) -> None:
         self._name = value
 
 
 class OGCServiceMixin:
     """Abstract class for all OGCService xml mappers,
     which implements functionality for global usage."""
-    _operation_urls: CallbackList = []
+    _operation_urls: CallbackList = CallbackList([], None)
 
     @property
     def _possible_operations(self):
         raise NotImplementedError
 
     @property
     def operation_urls(self) -> List[OperationUrl]:
```

### Comparing `django-ows-lib-0.1.0/ows_lib/xml_mapper/capabilities/wfs/mixins.py` & `django-ows-lib-0.1.1/ows_lib/xml_mapper/capabilities/wfs/mixins.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.1.0/ows_lib/xml_mapper/capabilities/wfs/wfs200.py` & `django-ows-lib-0.1.1/ows_lib/xml_mapper/capabilities/wfs/wfs200.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.1.0/ows_lib/xml_mapper/capabilities/wms/mixins.py` & `django-ows-lib-0.1.1/ows_lib/xml_mapper/capabilities/wms/mixins.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         if self.resolution:
             attr.update({"resolution": self.resolution})
         return attr
 
 
 class TimeDimensionMixin:
     # cache variable to store the parsed extent value
-    _time_extents: CallbackList = None
+    _time_extents: CallbackList = CallbackList([], None)
 
     @property
     def time_extents(self):
         if not self._time_extents:
             self.__parse_extent()
         return self._time_extents
```

### Comparing `django-ows-lib-0.1.0/ows_lib/xml_mapper/capabilities/wms/wms111.py` & `django-ows-lib-0.1.1/ows_lib/xml_mapper/capabilities/wms/wms111.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.1.0/ows_lib/xml_mapper/capabilities/wms/wms130.py` & `django-ows-lib-0.1.1/ows_lib/xml_mapper/capabilities/wms/wms130.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.1.0/ows_lib/xml_mapper/iso_metadata/iso_metadata.py` & `django-ows-lib-0.1.1/ows_lib/xml_mapper/iso_metadata/iso_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import urllib
 
 from django.contrib.gis.geos import MultiPolygon
 from django.contrib.gis.geos import Polygon as GeosPolygon
 from eulxml import xmlmap
+
 from ows_lib.xml_mapper.gml.gml import Gml
 from ows_lib.xml_mapper.mixins import CustomXmlObject
-from ows_lib.xml_mapper.namespaces import GCO_NAMESPACE, GMD_NAMESPACE, GML_3_1_1_NAMESPACE, SRV_NAMESPACE
+from ows_lib.xml_mapper.namespaces import (GCO_NAMESPACE, GMD_NAMESPACE,
+                                           GML_3_1_1_NAMESPACE, SRV_NAMESPACE)
 
 
 class Keyword(CustomXmlObject, xmlmap.XmlObject):
     ROOT_NS = GMD_NAMESPACE
     ROOT_NAME = "keyword"
     ROOT_NAMESPACES = dict([("gmd", GMD_NAMESPACE),
                             ("gco", GCO_NAMESPACE)])
 
     keyword = xmlmap.StringField(xpath="gco:CharacterString")
 
 
 class Category(CustomXmlObject, xmlmap.XmlObject):
-    # todo:
+    # TODO: Add xml specific information like root_ns, root_name, and namespaces list
 
     category = xmlmap.StringField(xpath=".")
 
 
 class Dimension(CustomXmlObject, xmlmap.XmlObject):
     ROOT_NS = GMD_NAMESPACE
     ROOT_NAME = "extent"
```

### Comparing `django-ows-lib-0.1.0/ows_lib/xml_mapper/mixins.py` & `django-ows-lib-0.1.1/ows_lib/xml_mapper/mixins.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,42 +4,48 @@
 from eulxml import xmlmap
 from eulxml.xmlmap import XmlObject
 from lxml.etree import XPathEvalError
 
 
 class CallbackList(list):
 
-    def __init__(self, iterable, callback: Callable, *args, **kwargs) -> None:
+    def __init__(self, iterable, callback: Callable = None, *args, **kwargs) -> None:
         super().__init__(iterable, *args, **kwargs)
         self.callback = callback
 
     def append(self, item) -> None:
         super().append(item)
-        self.callback(list_operation="append", items=item)
+        if self.callback:
+            self.callback(list_operation="append", items=item)
 
     def extend(self, items) -> None:
         super().extend(items)
-        self.callback(list_operation="extend", items=items)
+        if self.callback:
+            self.callback(list_operation="extend", items=items)
 
-    def pop(self, __index):
-        operation_url_to_pop = self[__index]
-        super().pop(__index)
-        self.callback(list_operation="pop", items=operation_url_to_pop)
+    def pop(self, index):
+        operation_url_to_pop = self[index]
+        super().pop(index)
+        if self.callback:
+            self.callback(list_operation="pop", items=operation_url_to_pop)
 
     def clear(self) -> None:
         super().clear()
-        self.callback(list_operation="clear")
+        if self.callback:
+            self.callback(list_operation="clear")
 
-    def insert(self, __index, __object) -> None:
-        super().insert(__index, __object)
-        self.callback(list_operation="insert", items=__object)
-
-    def remove(self, __value) -> None:
-        super().remove(__value)
-        self.callback(list_operation="remove", items=__value)
+    def insert(self, index, obj) -> None:
+        super().insert(index, obj)
+        if self.callback:
+            self.callback(list_operation="insert", items=obj)
+
+    def remove(self, value) -> None:
+        super().remove(value)
+        if self.callback:
+            self.callback(list_operation="remove", items=value)
 
 
 class CustomXmlObject(XmlObject):
     """ Custom Xml Object class which implements some generic functions to get the db model class and all relevant field content
         as dict.
     """
```

### Comparing `django-ows-lib-0.1.0/ows_lib/xml_mapper/namespaces.py` & `django-ows-lib-0.1.1/ows_lib/xml_mapper/namespaces.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.1.0/ows_lib/xml_mapper/utils.py` & `django-ows-lib-0.1.1/ows_lib/xml_mapper/utils.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.1.0/ows_lib/xml_mapper/xml_requests/wfs/get_feature.py` & `django-ows-lib-0.1.1/ows_lib/xml_mapper/xml_requests/wfs/get_feature.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import List
 
 from django.contrib.gis.geos import GEOSGeometry
 from django.contrib.gis.geos import Polygon as GeosPolygon
 from eulxml.xmlmap import (NodeField, NodeListField, StringField,
                            StringListField, XmlObject)
 
+from ows_lib.xml_mapper.consts import FES_AND, FES_OR, FES_WITHIN
 from ows_lib.xml_mapper.namespaces import (FES_2_0_NAMEPSACE,
                                            GML_3_2_2_NAMESPACE,
                                            WFS_2_0_0_NAMESPACE)
 
 
 class PolygonFilter(XmlObject):
     ROOT_NS = GML_3_2_2_NAMESPACE
@@ -65,47 +66,47 @@
     ROOT_NS = FES_2_0_NAMEPSACE
     ROOT_NAME = "Or"
     ROOT_NAMESPACES = {
         "fes": FES_2_0_NAMEPSACE,
     }
 
     within_conditions = NodeListField(
-        xpath="./fes:Within", node_class=WithinCondition)
-    or_conditions = NodeListField(xpath="./fes:Or", node_class="self")
+        xpath=FES_WITHIN, node_class=WithinCondition)
+    or_conditions = NodeListField(xpath=FES_OR, node_class="self")
     # FIXME: and_conditions are also possible
 
 
 class AndCondition(XmlObject):
     ROOT_NS = FES_2_0_NAMEPSACE
     ROOT_NAME = "And"
     ROOT_NAMESPACES = {
         "fes": FES_2_0_NAMEPSACE,
     }
 
     within_conditions = NodeListField(
-        xpath="./fes:Within", node_class=WithinCondition)
-    and_conditions = NodeListField(xpath="./fes:And", node_class="self")
-    or_conditions = NodeListField(xpath="./fes:Or", node_class=OrCondition)
+        xpath=FES_WITHIN, node_class=WithinCondition)
+    and_conditions = NodeListField(xpath=FES_AND, node_class="self")
+    or_conditions = NodeListField(xpath=FES_OR, node_class=OrCondition)
 
 
 class Filter(XmlObject):
     ROOT_NS = FES_2_0_NAMEPSACE
     ROOT_NAME = "Filter"
     XSD_SCHEMA = "http://schemas.opengis.net/filter/2.0/filter.xsd"
     ROOT_NAMESPACES = {
         "fes": FES_2_0_NAMEPSACE,
         "gml": GML_3_2_2_NAMESPACE
     }
 
     ressource_ids = StringListField(xpath="./fes:ResourceId/@rid")
 
-    and_condition = NodeField(xpath="./fes:And", node_class=AndCondition)
-    or_condition = NodeField(xpath="./fes:Or", node_class=OrCondition)
+    and_condition = NodeField(xpath=FES_AND, node_class=AndCondition)
+    or_condition = NodeField(xpath=FES_OR, node_class=OrCondition)
     within_conditions = NodeListField(
-        xpath="./fes:Within", node_class=WithinCondition)
+        xpath=FES_WITHIN, node_class=WithinCondition)
 
 
 class Query(XmlObject):
     ROOT_NS = WFS_2_0_0_NAMESPACE
     ROOT_NAME = "Query"
     XSD_SCHEMA = "http://schemas.opengis.net/wfs/2.0/wfs.xsd"
     ROOT_NAMESPACES = {
```

### Comparing `django-ows-lib-0.1.0/ows_lib/xml_mapper/xml_responses/csw/get_records.py` & `django-ows-lib-0.1.1/ows_lib/xml_mapper/xml_responses/csw/get_records.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.1.0/ows_lib/xml_mapper/xml_responses/wfs/describe_feature.py` & `django-ows-lib-0.1.1/ows_lib/xml_mapper/xml_responses/wfs/describe_feature.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.1.0/ows_lib/xml_mapper/xml_responses/wfs/feature_collection.py` & `django-ows-lib-0.1.1/ows_lib/xml_mapper/xml_responses/wfs/feature_collection.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.1.0/setup.py` & `django-ows-lib-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,23 @@
 description = 'Well layered ows lib with a client implementation to communicate with ogc services with django based objects, including xml mapper classes to serialize and deserialize ows xml files, such as capabilities.'
 url = 'https://github.com/mrmap-community/django-ows-lib'
 author = 'mrmap-community'
 author_email = 'jonas.kiefer@live.com'
 license = 'MIT'
 
 
+REQUIREMENTS = [
+    "django>=3.0,<4.3",
+    "django-axis-order==0.1.0",
+    "eulxml==1.1.3",
+    "isodate==0.6.1",
+    "camel-converter==3.0.0",
+    "requests>=2.23.0,<2.30.0"
+]
+
 with open("README.rst", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 def get_version(package):
     """
     Return package version as listed in `__version__` in `init.py`.
@@ -36,17 +45,15 @@
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author=author,
     author_email=author_email,
     packages=[p for p in find_namespace_packages(
         exclude=('tests*',)) if p.startswith(package)],
     include_package_data=True,
-    install_requires=[
-        "django>=3.0,<4.3",
-    ],
+    install_requires=REQUIREMENTS,
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
```

