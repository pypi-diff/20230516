# Comparing `tmp/bohrium_openapi_python_sdk-0.0.1.tar.gz` & `tmp/bohrium_openapi_python_sdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bohrium_openapi_python_sdk-0.0.1.tar", last modified: Tue May 16 07:40:03 2023, max compression
+gzip compressed data, was "bohrium_openapi_python_sdk-0.0.2.tar", last modified: Tue May 16 08:20:29 2023, max compression
```

## Comparing `bohrium_openapi_python_sdk-0.0.1.tar` & `bohrium_openapi_python_sdk-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,14 @@
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-16 07:40:03.304494 bohrium_openapi_python_sdk-0.0.1/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      220 2023-05-16 07:40:03.304244 bohrium_openapi_python_sdk-0.0.1/PKG-INFO
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       56 2023-05-16 07:10:39.000000 bohrium_openapi_python_sdk-0.0.1/README.md
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-16 07:40:03.302324 bohrium_openapi_python_sdk-0.0.1/bohrium_openapi_python_sdk.egg-info/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      220 2023-05-16 07:40:03.000000 bohrium_openapi_python_sdk-0.0.1/bohrium_openapi_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      321 2023-05-16 07:40:03.000000 bohrium_openapi_python_sdk-0.0.1/bohrium_openapi_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        1 2023-05-16 07:40:03.000000 bohrium_openapi_python_sdk-0.0.1/bohrium_openapi_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       11 2023-05-16 07:40:03.000000 bohrium_openapi_python_sdk-0.0.1/bohrium_openapi_python_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-16 07:40:03.302676 bohrium_openapi_python_sdk-0.0.1/python-sdk/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      123 2023-05-16 07:22:01.000000 bohrium_openapi_python_sdk-0.0.1/python-sdk/__init__.py
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-16 07:40:03.303190 bohrium_openapi_python_sdk-0.0.1/python-sdk/auth/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-16 07:14:57.000000 bohrium_openapi_python_sdk-0.0.1/python-sdk/auth/__init__.py
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-16 07:40:03.303812 bohrium_openapi_python_sdk-0.0.1/python-sdk/node/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-16 07:15:29.000000 bohrium_openapi_python_sdk-0.0.1/python-sdk/node/__init__.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      123 2023-05-16 07:16:57.000000 bohrium_openapi_python_sdk-0.0.1/python-sdk/node/main.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       38 2023-05-16 07:40:03.304567 bohrium_openapi_python_sdk-0.0.1/setup.cfg
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      358 2023-05-16 07:33:08.000000 bohrium_openapi_python_sdk-0.0.1/setup.py
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-16 08:20:29.103470 bohrium_openapi_python_sdk-0.0.2/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      220 2023-05-16 08:20:29.103042 bohrium_openapi_python_sdk-0.0.2/PKG-INFO
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       56 2023-05-16 07:10:39.000000 bohrium_openapi_python_sdk-0.0.2/README.md
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-16 08:20:29.101729 bohrium_openapi_python_sdk-0.0.2/bohrium_openapi_python_sdk.egg-info/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      220 2023-05-16 08:20:29.000000 bohrium_openapi_python_sdk-0.0.2/bohrium_openapi_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      299 2023-05-16 08:20:29.000000 bohrium_openapi_python_sdk-0.0.2/bohrium_openapi_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        1 2023-05-16 08:20:29.000000 bohrium_openapi_python_sdk-0.0.2/bohrium_openapi_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       84 2023-05-16 08:20:29.000000 bohrium_openapi_python_sdk-0.0.2/bohrium_openapi_python_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        4 2023-05-16 08:20:29.000000 bohrium_openapi_python_sdk-0.0.2/bohrium_openapi_python_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-16 08:20:29.102599 bohrium_openapi_python_sdk-0.0.2/sdk/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      123 2023-05-16 07:22:01.000000 bohrium_openapi_python_sdk-0.0.2/sdk/__init__.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      123 2023-05-16 07:16:57.000000 bohrium_openapi_python_sdk-0.0.2/sdk/node.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       38 2023-05-16 08:20:29.103564 bohrium_openapi_python_sdk-0.0.2/setup.cfg
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      514 2023-05-16 08:20:22.000000 bohrium_openapi_python_sdk-0.0.2/setup.py
```

