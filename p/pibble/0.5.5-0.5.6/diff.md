# Comparing `tmp/pibble-0.5.5.tar.gz` & `tmp/pibble-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pibble-0.5.5.tar", last modified: Fri May 12 19:56:44 2023, max compression
+gzip compressed data, was "pibble-0.5.6.tar", last modified: Tue May 16 17:44:22 2023, max compression
```

## Comparing `pibble-0.5.5.tar` & `pibble-0.5.6.tar`

### file list

```diff
@@ -1,214 +1,214 @@
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.216298 pibble-0.5.5/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6444 2023-05-12 19:56:44.216298 pibble-0.5.5/PKG-INFO
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5919 2023-05-12 19:56:44.000000 pibble-0.5.5/README.md
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.204299 pibble-0.5.5/pibble/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     9049 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/__main__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.208299 pibble-0.5.5/pibble/api/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3374 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.208299 pibble-0.5.5/pibble/api/client/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/client/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.208299 pibble-0.5.5/pibble/api/client/apachethrift/
--rw-------   0 benjamin  (1000) benjamin  (1000)     6195 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/client/apachethrift/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1865 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/client/apachethrift/wrapper.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1340 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/client/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.208299 pibble-0.5.5/pibble/api/client/file/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/client/file/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    14230 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/client/file/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     9726 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/client/file/ftp.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    11561 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/client/file/hdfs.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    12782 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/client/file/local.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    19652 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/client/file/sftp.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4132 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/client/googlerpc.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.208299 pibble-0.5.5/pibble/api/client/webservice/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/client/webservice/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4728 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/client/webservice/apachethrift.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    16837 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/client/webservice/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2312 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/client/webservice/jsonapi.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.208299 pibble-0.5.5/pibble/api/client/webservice/rpc/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/client/webservice/rpc/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    11386 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/client/webservice/rpc/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4766 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/client/webservice/rpc/jsonrpc.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    10690 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/client/webservice/rpc/xmlrpc.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     6689 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/client/webservice/soap.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     7333 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/client/webservice/wrapper.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      631 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/client/wrapper.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4087 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/configuration.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     6101 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/exceptions.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.208299 pibble-0.5.5/pibble/api/helpers/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/helpers/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    15706 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/helpers/apachethrift.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    20612 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/helpers/authentication.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    24691 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/helpers/googlerpc.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    13415 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/helpers/store.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    13868 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/helpers/wrappers.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.208299 pibble-0.5.5/pibble/api/meta/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/meta/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     9492 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/meta/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2952 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/meta/helpers.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.208299 pibble-0.5.5/pibble/api/middleware/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/middleware/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.208299 pibble-0.5.5/pibble/api/middleware/apachethrift/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/middleware/apachethrift/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1176 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/middleware/apachethrift/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1276 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/middleware/apachethrift/screening.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      167 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/middleware/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.208299 pibble-0.5.5/pibble/api/middleware/database/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/middleware/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3033 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/middleware/database/orm.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.208299 pibble-0.5.5/pibble/api/middleware/file/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/middleware/file/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      454 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/middleware/file/temp.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.208299 pibble-0.5.5/pibble/api/middleware/googlerpc/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/middleware/googlerpc/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2976 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/middleware/googlerpc/authentication.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1176 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/middleware/googlerpc/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1028 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/middleware/googlerpc/metadata.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3703 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/middleware/screening.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.208299 pibble-0.5.5/pibble/api/middleware/webservice/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/middleware/webservice/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.212298 pibble-0.5.5/pibble/api/middleware/webservice/authentication/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/middleware/webservice/authentication/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     5161 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/middleware/webservice/authentication/basic.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4338 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/middleware/webservice/authentication/bearer.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    13472 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/middleware/webservice/authentication/digest.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2134 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/middleware/webservice/authentication/header.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    17704 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/middleware/webservice/authentication/oauth.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1623 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/middleware/webservice/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3256 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/middleware/webservice/limit.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1908 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/middleware/webservice/screening.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.212298 pibble-0.5.5/pibble/api/protocol/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/protocol/__init__.py
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)    19486 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/protocol/apachethrift.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.212298 pibble-0.5.5/pibble/api/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/server/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2451 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/server/apachethrift.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2080 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/server/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.212298 pibble-0.5.5/pibble/api/server/file/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/server/file/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1419 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/server/file/ftp.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    15640 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/server/file/sftp.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     5453 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/server/googlerpc.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.212298 pibble-0.5.5/pibble/api/server/webservice/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/server/webservice/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2296 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/server/webservice/apachethrift.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     7311 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/server/webservice/awslambda.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    39095 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/server/webservice/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.212298 pibble-0.5.5/pibble/api/server/webservice/drivers/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/server/webservice/drivers/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1489 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/server/webservice/drivers/driver_cherrypy.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2228 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/server/webservice/drivers/driver_gunicorn.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1078 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/server/webservice/drivers/driver_werkzeug.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    15947 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/server/webservice/handler.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3164 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/server/webservice/jsonapi.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      969 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/server/webservice/orm.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.212298 pibble-0.5.5/pibble/api/server/webservice/rpc/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/server/webservice/rpc/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4150 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/server/webservice/rpc/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     6457 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/server/webservice/rpc/jsonrpc.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    12004 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/server/webservice/rpc/xmlrpc.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    16962 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/server/webservice/soap.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.212298 pibble-0.5.5/pibble/api/server/webservice/template/
--rw-------   0 benjamin  (1000) benjamin  (1000)     9717 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/server/webservice/template/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     9201 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/server/webservice/template/extensions.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     9770 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/api/server/webservice/template/loader.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.212298 pibble-0.5.5/pibble/database/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.000000 pibble-0.5.5/pibble/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     7797 2023-05-12 19:56:44.000000 pibble-0.5.5/pibble/database/dedupe.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    10529 2023-05-12 19:56:44.000000 pibble-0.5.5/pibble/database/engine.py
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)      306 2023-05-12 19:56:44.000000 pibble-0.5.5/pibble/database/exceptions.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    28331 2023-05-12 19:56:44.000000 pibble-0.5.5/pibble/database/orm.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2694 2023-05-12 19:56:44.000000 pibble-0.5.5/pibble/database/util.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.212298 pibble-0.5.5/pibble/ext/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/ext/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.212298 pibble-0.5.5/pibble/ext/cms/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/ext/cms/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.212298 pibble-0.5.5/pibble/ext/cms/database/
--rw-------   0 benjamin  (1000) benjamin  (1000)      721 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/ext/cms/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      124 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/ext/cms/database/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3129 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/ext/cms/database/interface.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1434 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/ext/cms/database/menu.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2531 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/ext/cms/database/view.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1366 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/ext/cms/middleware.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.212298 pibble-0.5.5/pibble/ext/cms/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/ext/cms/server/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     6660 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/ext/cms/server/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3012 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/ext/cms/server/extension.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.212298 pibble-0.5.5/pibble/ext/dam/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/ext/dam/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.212298 pibble-0.5.5/pibble/ext/dam/database/
--rw-------   0 benjamin  (1000) benjamin  (1000)      229 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/ext/dam/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      117 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/ext/dam/database/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1110 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/ext/dam/database/files.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.212298 pibble-0.5.5/pibble/ext/dam/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/ext/dam/server/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      494 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/ext/dam/server/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.212298 pibble-0.5.5/pibble/ext/rest/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/ext/rest/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.216298 pibble-0.5.5/pibble/ext/rest/database/
--rw-------   0 benjamin  (1000) benjamin  (1000)      103 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/ext/rest/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)       94 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/ext/rest/database/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.216298 pibble-0.5.5/pibble/ext/rest/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/ext/rest/server/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    15662 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/ext/rest/server/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     7244 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/ext/rest/server/user.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.216298 pibble-0.5.5/pibble/ext/session/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/ext/session/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.216298 pibble-0.5.5/pibble/ext/session/database/
--rw-------   0 benjamin  (1000) benjamin  (1000)      260 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/ext/session/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      172 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/ext/session/database/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      776 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/ext/session/database/session.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.216298 pibble-0.5.5/pibble/ext/session/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/ext/session/server/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     5087 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/ext/session/server/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.216298 pibble-0.5.5/pibble/ext/user/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/ext/user/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.216298 pibble-0.5.5/pibble/ext/user/client/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/ext/user/client/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      985 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/ext/user/client/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.216298 pibble-0.5.5/pibble/ext/user/database/
--rw-------   0 benjamin  (1000) benjamin  (1000)      933 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/ext/user/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      860 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/ext/user/database/authentication.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      103 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/ext/user/database/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      720 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/ext/user/database/notification.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     5865 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/ext/user/database/permission.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      611 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/ext/user/database/user.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.216298 pibble-0.5.5/pibble/ext/user/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/ext/user/server/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    24935 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/ext/user/server/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.216298 pibble-0.5.5/pibble/hooks/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/hooks/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     6037 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/hooks/aws.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.216298 pibble-0.5.5/pibble/media/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/media/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    10388 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/media/thumbnail.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.216298 pibble-0.5.5/pibble/resources/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/resources/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    10655 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/resources/retriever.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.216298 pibble-0.5.5/pibble/scripts/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/scripts/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1909 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/scripts/importcheck.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1726 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/scripts/templatefiles.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2732 2023-05-12 19:56:44.000000 pibble-0.5.5/pibble/setup.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.216298 pibble-0.5.5/pibble/util/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.000000 pibble-0.5.5/pibble/util/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     8357 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/util/encryption.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    16171 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/util/files.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    32884 2023-05-12 19:56:44.000000 pibble-0.5.5/pibble/util/helpers.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      563 2023-05-12 19:56:44.000000 pibble-0.5.5/pibble/util/imaging.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     6330 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/util/log.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1701 2023-05-12 19:56:44.000000 pibble-0.5.5/pibble/util/numeric.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    27424 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/util/strings.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.216298 pibble-0.5.5/pibble/web/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/web/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3227 2023-05-12 19:56:43.000000 pibble-0.5.5/pibble/web/scraper.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-12 19:56:44.204299 pibble-0.5.5/pibble.egg-info/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6444 2023-05-12 19:56:44.000000 pibble-0.5.5/pibble.egg-info/PKG-INFO
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5627 2023-05-12 19:56:44.000000 pibble-0.5.5/pibble.egg-info/SOURCES.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        1 2023-05-12 19:56:44.000000 pibble-0.5.5/pibble.egg-info/dependency_links.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       48 2023-05-12 19:56:44.000000 pibble-0.5.5/pibble.egg-info/entry_points.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1936 2023-05-12 19:56:44.000000 pibble-0.5.5/pibble.egg-info/requires.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        7 2023-05-12 19:56:44.000000 pibble-0.5.5/pibble.egg-info/top_level.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       38 2023-05-12 19:56:44.216298 pibble-0.5.5/setup.cfg
--rw-------   0 benjamin  (1000) benjamin  (1000)     2732 2023-05-12 19:56:44.000000 pibble-0.5.5/setup.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.846976 pibble-0.5.6/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6444 2023-05-16 17:44:22.846976 pibble-0.5.6/PKG-INFO
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5919 2023-05-16 17:44:22.000000 pibble-0.5.6/README.md
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.834976 pibble-0.5.6/pibble/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     9049 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/__main__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.834976 pibble-0.5.6/pibble/api/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3374 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.834976 pibble-0.5.6/pibble/api/client/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/client/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.834976 pibble-0.5.6/pibble/api/client/apachethrift/
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6195 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/client/apachethrift/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1865 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/client/apachethrift/wrapper.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1340 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/client/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.834976 pibble-0.5.6/pibble/api/client/file/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/client/file/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    14230 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/client/file/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     9726 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/client/file/ftp.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    11561 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/client/file/hdfs.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    12782 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/client/file/local.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    19652 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/client/file/sftp.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4132 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/client/googlerpc.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.838976 pibble-0.5.6/pibble/api/client/webservice/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/client/webservice/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4728 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/client/webservice/apachethrift.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    16837 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/client/webservice/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2312 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/client/webservice/jsonapi.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.838976 pibble-0.5.6/pibble/api/client/webservice/rpc/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/client/webservice/rpc/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    11386 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/client/webservice/rpc/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4766 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/client/webservice/rpc/jsonrpc.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    10690 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/client/webservice/rpc/xmlrpc.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6689 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/client/webservice/soap.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     7333 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/client/webservice/wrapper.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      631 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/client/wrapper.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4087 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/configuration.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6101 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/exceptions.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.838976 pibble-0.5.6/pibble/api/helpers/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/helpers/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    15706 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/helpers/apachethrift.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    20612 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/helpers/authentication.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    24691 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/helpers/googlerpc.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    13415 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/helpers/store.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    13868 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/helpers/wrappers.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.838976 pibble-0.5.6/pibble/api/meta/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/meta/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     9492 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/meta/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2952 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/meta/helpers.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.838976 pibble-0.5.6/pibble/api/middleware/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.838976 pibble-0.5.6/pibble/api/middleware/apachethrift/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/apachethrift/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1176 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/apachethrift/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1276 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/apachethrift/screening.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      167 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.838976 pibble-0.5.6/pibble/api/middleware/database/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/database/__init__.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2841 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/database/orm.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.838976 pibble-0.5.6/pibble/api/middleware/file/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/file/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      454 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/file/temp.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.838976 pibble-0.5.6/pibble/api/middleware/googlerpc/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/googlerpc/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2976 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/googlerpc/authentication.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1176 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/googlerpc/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1028 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/googlerpc/metadata.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3703 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/screening.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.838976 pibble-0.5.6/pibble/api/middleware/webservice/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/webservice/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.838976 pibble-0.5.6/pibble/api/middleware/webservice/authentication/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/webservice/authentication/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     5161 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/webservice/authentication/basic.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4338 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/webservice/authentication/bearer.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    13472 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/webservice/authentication/digest.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2134 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/webservice/authentication/header.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    17704 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/webservice/authentication/oauth.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1623 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/webservice/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3256 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/webservice/limit.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1908 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/webservice/screening.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.838976 pibble-0.5.6/pibble/api/protocol/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/protocol/__init__.py
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)    19486 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/protocol/apachethrift.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.838976 pibble-0.5.6/pibble/api/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2451 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/apachethrift.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2080 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/server/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.838976 pibble-0.5.6/pibble/api/server/file/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/file/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1419 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/file/ftp.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    15640 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/file/sftp.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     5453 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/server/googlerpc.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.842976 pibble-0.5.6/pibble/api/server/webservice/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/webservice/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2296 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/webservice/apachethrift.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     7311 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/webservice/awslambda.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    38922 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/webservice/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.842976 pibble-0.5.6/pibble/api/server/webservice/drivers/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/webservice/drivers/__init__.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1489 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/webservice/drivers/driver_cherrypy.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2229 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/webservice/drivers/driver_gunicorn.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1078 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/webservice/drivers/driver_werkzeug.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    15947 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/webservice/handler.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3164 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/webservice/jsonapi.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      969 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/webservice/orm.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.842976 pibble-0.5.6/pibble/api/server/webservice/rpc/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/webservice/rpc/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4149 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/webservice/rpc/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6457 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/webservice/rpc/jsonrpc.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    12004 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/webservice/rpc/xmlrpc.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    16963 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/webservice/soap.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.842976 pibble-0.5.6/pibble/api/server/webservice/template/
+-rw-------   0 benjamin  (1000) benjamin  (1000)     9717 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/webservice/template/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     9201 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/webservice/template/extensions.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     9770 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/webservice/template/loader.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.842976 pibble-0.5.6/pibble/database/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     7797 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/database/dedupe.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    10593 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/database/engine.py
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)      306 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/database/exceptions.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    28607 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/database/orm.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2694 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/database/util.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.842976 pibble-0.5.6/pibble/ext/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.842976 pibble-0.5.6/pibble/ext/cms/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/cms/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.842976 pibble-0.5.6/pibble/ext/cms/database/
+-rw-------   0 benjamin  (1000) benjamin  (1000)      721 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/cms/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      124 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/cms/database/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3129 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/cms/database/interface.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1434 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/cms/database/menu.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2531 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/cms/database/view.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1366 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/cms/middleware.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.842976 pibble-0.5.6/pibble/ext/cms/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/cms/server/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6660 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/cms/server/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3012 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/cms/server/extension.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.842976 pibble-0.5.6/pibble/ext/dam/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/dam/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.842976 pibble-0.5.6/pibble/ext/dam/database/
+-rw-------   0 benjamin  (1000) benjamin  (1000)      229 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/dam/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      117 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/dam/database/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1110 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/dam/database/files.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.842976 pibble-0.5.6/pibble/ext/dam/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/dam/server/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      494 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/dam/server/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.842976 pibble-0.5.6/pibble/ext/rest/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/rest/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.842976 pibble-0.5.6/pibble/ext/rest/database/
+-rw-------   0 benjamin  (1000) benjamin  (1000)      103 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/rest/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)       94 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/rest/database/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.842976 pibble-0.5.6/pibble/ext/rest/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/rest/server/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    15664 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/rest/server/base.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     7245 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/rest/server/user.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.842976 pibble-0.5.6/pibble/ext/session/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/session/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.842976 pibble-0.5.6/pibble/ext/session/database/
+-rw-------   0 benjamin  (1000) benjamin  (1000)      260 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/ext/session/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      172 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/ext/session/database/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      776 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/ext/session/database/session.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.842976 pibble-0.5.6/pibble/ext/session/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/session/server/__init__.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5087 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/ext/session/server/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.842976 pibble-0.5.6/pibble/ext/user/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/ext/user/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.842976 pibble-0.5.6/pibble/ext/user/client/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/ext/user/client/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      985 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/ext/user/client/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.846976 pibble-0.5.6/pibble/ext/user/database/
+-rw-------   0 benjamin  (1000) benjamin  (1000)      933 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/ext/user/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      860 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/ext/user/database/authentication.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      103 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/ext/user/database/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      720 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/ext/user/database/notification.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     5865 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/ext/user/database/permission.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      611 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/ext/user/database/user.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.846976 pibble-0.5.6/pibble/ext/user/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/ext/user/server/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    24936 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/ext/user/server/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.846976 pibble-0.5.6/pibble/hooks/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/hooks/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6037 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/hooks/aws.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.846976 pibble-0.5.6/pibble/media/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/media/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    10388 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/media/thumbnail.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.846976 pibble-0.5.6/pibble/resources/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/resources/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    10655 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/resources/retriever.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.846976 pibble-0.5.6/pibble/scripts/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/scripts/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1909 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/scripts/importcheck.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1726 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/scripts/templatefiles.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2732 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/setup.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.846976 pibble-0.5.6/pibble/util/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/util/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     8357 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/util/encryption.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    16171 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/util/files.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    32914 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/util/helpers.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      563 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/util/imaging.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6330 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/util/log.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1701 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/util/numeric.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    27424 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/util/strings.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.846976 pibble-0.5.6/pibble/web/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/web/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3227 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/web/scraper.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.834976 pibble-0.5.6/pibble.egg-info/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6444 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble.egg-info/PKG-INFO
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5627 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble.egg-info/SOURCES.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        1 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble.egg-info/dependency_links.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       48 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble.egg-info/entry_points.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1936 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble.egg-info/requires.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        7 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble.egg-info/top_level.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       38 2023-05-16 17:44:22.846976 pibble-0.5.6/setup.cfg
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2732 2023-05-16 17:44:22.000000 pibble-0.5.6/setup.py
```

### Comparing `pibble-0.5.5/PKG-INFO` & `pibble-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pibble
-Version: 0.5.5
+Version: 0.5.6
 Summary: A framework for developing webapps quickly and easily using Python
 Author: Benjamin Paine
 Author-email: painebenjamin@gmail.com
 License: gpl-3.0
 Description-Content-Type: text/markdown
 Provides-Extra: mysql
 Provides-Extra: postgresql
```

### Comparing `pibble-0.5.5/README.md` & `pibble-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/__main__.py` & `pibble-0.5.6/pibble/__main__.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/base.py` & `pibble-0.5.6/pibble/api/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/client/apachethrift/__init__.py` & `pibble-0.5.6/pibble/api/client/apachethrift/__init__.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/client/apachethrift/wrapper.py` & `pibble-0.5.6/pibble/api/client/apachethrift/wrapper.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/client/base.py` & `pibble-0.5.6/pibble/api/client/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/client/file/base.py` & `pibble-0.5.6/pibble/api/client/file/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/client/file/ftp.py` & `pibble-0.5.6/pibble/api/client/file/ftp.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/client/file/hdfs.py` & `pibble-0.5.6/pibble/api/client/file/hdfs.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/client/file/local.py` & `pibble-0.5.6/pibble/api/client/file/local.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/client/file/sftp.py` & `pibble-0.5.6/pibble/api/client/file/sftp.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/client/googlerpc.py` & `pibble-0.5.6/pibble/api/client/googlerpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/client/webservice/apachethrift.py` & `pibble-0.5.6/pibble/api/client/webservice/apachethrift.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/client/webservice/base.py` & `pibble-0.5.6/pibble/api/client/webservice/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/client/webservice/jsonapi.py` & `pibble-0.5.6/pibble/api/client/webservice/jsonapi.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/client/webservice/rpc/base.py` & `pibble-0.5.6/pibble/api/client/webservice/rpc/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/client/webservice/rpc/jsonrpc.py` & `pibble-0.5.6/pibble/api/client/webservice/rpc/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/client/webservice/rpc/xmlrpc.py` & `pibble-0.5.6/pibble/api/client/webservice/rpc/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/client/webservice/soap.py` & `pibble-0.5.6/pibble/api/client/webservice/soap.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/client/webservice/wrapper.py` & `pibble-0.5.6/pibble/api/client/webservice/wrapper.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/client/wrapper.py` & `pibble-0.5.6/pibble/api/client/wrapper.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/configuration.py` & `pibble-0.5.6/pibble/api/configuration.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/exceptions.py` & `pibble-0.5.6/pibble/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/helpers/apachethrift.py` & `pibble-0.5.6/pibble/api/helpers/apachethrift.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/helpers/authentication.py` & `pibble-0.5.6/pibble/api/helpers/authentication.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/helpers/googlerpc.py` & `pibble-0.5.6/pibble/api/helpers/googlerpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/helpers/store.py` & `pibble-0.5.6/pibble/api/helpers/store.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/helpers/wrappers.py` & `pibble-0.5.6/pibble/api/helpers/wrappers.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/meta/base.py` & `pibble-0.5.6/pibble/api/meta/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/meta/helpers.py` & `pibble-0.5.6/pibble/api/meta/helpers.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/middleware/apachethrift/base.py` & `pibble-0.5.6/pibble/api/middleware/apachethrift/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/middleware/apachethrift/screening.py` & `pibble-0.5.6/pibble/api/middleware/apachethrift/screening.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/middleware/database/orm.py` & `pibble-0.5.6/pibble/api/middleware/database/orm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import Optional, Union
 
 from webob import Request as WebobRequest, Response as WebobResponse
 from requests import Request as RequestsRequest, Response as RequestsResponse
 from pibble.api.helpers.wrappers import RequestWrapper, ResponseWrapper
 from pibble.api.middleware.base import APIMiddlewareBase
-from pibble.api.exceptions import ConfigurationError
 from pibble.database.orm import ORM, ORMBuilder, ORMSession
 from pibble.util.log import logger
 
 
 class ORMMiddlewareBase(APIMiddlewareBase):
     """
     A client/server with an ORM attached to it.
@@ -29,19 +28,17 @@
             )
 
     @property
     def database(self) -> ORMSession:
         """
         Getter for the database ensures we only instantiate when we need it.
         """
-        if not hasattr(self, "orm"):
-            raise ConfigurationError("No ORM present, but database requested.")
         if not hasattr(self, "_database"):
             logger.debug("Database requested, connecting to ORM")
-            self._database = self.orm.session(expire_on_commit=False)
+            self._database = self.orm.session()
         return self._database
 
     @database.deleter
     def database(self) -> None:
         """
         Only remove the database if necessary.
         """
```

### Comparing `pibble-0.5.5/pibble/api/middleware/googlerpc/authentication.py` & `pibble-0.5.6/pibble/api/middleware/googlerpc/authentication.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/middleware/googlerpc/base.py` & `pibble-0.5.6/pibble/api/middleware/googlerpc/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/middleware/googlerpc/metadata.py` & `pibble-0.5.6/pibble/api/middleware/googlerpc/metadata.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/middleware/screening.py` & `pibble-0.5.6/pibble/api/middleware/screening.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/middleware/webservice/authentication/basic.py` & `pibble-0.5.6/pibble/api/middleware/webservice/authentication/basic.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/middleware/webservice/authentication/bearer.py` & `pibble-0.5.6/pibble/api/middleware/webservice/authentication/bearer.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/middleware/webservice/authentication/digest.py` & `pibble-0.5.6/pibble/api/middleware/webservice/authentication/digest.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/middleware/webservice/authentication/header.py` & `pibble-0.5.6/pibble/api/middleware/webservice/authentication/header.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/middleware/webservice/authentication/oauth.py` & `pibble-0.5.6/pibble/api/middleware/webservice/authentication/oauth.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/middleware/webservice/base.py` & `pibble-0.5.6/pibble/api/middleware/webservice/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/middleware/webservice/limit.py` & `pibble-0.5.6/pibble/api/middleware/webservice/limit.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/middleware/webservice/screening.py` & `pibble-0.5.6/pibble/api/middleware/webservice/screening.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/protocol/apachethrift.py` & `pibble-0.5.6/pibble/api/protocol/apachethrift.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/server/apachethrift.py` & `pibble-0.5.6/pibble/api/server/apachethrift.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/server/base.py` & `pibble-0.5.6/pibble/api/server/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/server/file/ftp.py` & `pibble-0.5.6/pibble/api/server/file/ftp.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/server/file/sftp.py` & `pibble-0.5.6/pibble/api/server/file/sftp.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/server/googlerpc.py` & `pibble-0.5.6/pibble/api/server/googlerpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/server/webservice/apachethrift.py` & `pibble-0.5.6/pibble/api/server/webservice/apachethrift.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from pibble.api.exceptions import ApacheThriftError
 from pibble.api.helpers.apachethrift import (
     ApacheThriftService,
     ApacheThriftServerHandler,
 )
 
 
-
 class ApacheThriftWebServer(WebServiceAPIServerBase):
     """
     A webservice for handling thrift services.
 
     What this achieves is simple; there is an underlying layer of a thrift processor, which is called when
     receiving a POST request. This is less performant than a raw thrift server (due to HTTP overhead), but
     still more performant than other web services due to binary encoding.
@@ -29,14 +28,15 @@
     One of the following:
       A.
         1. `thrift.service` The compiled thrift module, or a string to resolve.
       B.
         1. `thrift.compile` The thrift IDL.
         2. `thrift.service` The service name.
     """
+
     handlers = WebServiceAPIHandlerRegistry()
 
     def on_configure(self) -> None:
         self.thrift = ApacheThriftService(self.configuration, True)
         self.processor = self.thrift.service.Processor(
             ApacheThriftServerHandler(self, self.thrift.interface, self.thrift.handler)
         )
```

### Comparing `pibble-0.5.5/pibble/api/server/webservice/awslambda.py` & `pibble-0.5.6/pibble/api/server/webservice/awslambda.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/server/webservice/base.py` & `pibble-0.5.6/pibble/api/server/webservice/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 
 import io
 import os
-import re
 import logging
 import mimetypes
 
 from traceback import format_exc
 
 from typing import (
     Optional,
@@ -19,15 +18,15 @@
     Dict,
     cast,
     TYPE_CHECKING,
 )
 
 from webob import Request, Response
 
-from pibble.util.strings import decode, truncate
+from pibble.util.strings import decode
 from pibble.util.log import logger
 from pibble.util.helpers import CompressedIterator
 from pibble.util.files import FileIterator
 from pibble.api.server.base import APIServerBase
 from pibble.api.server.webservice.handler import (
     WebServiceAPIHandlerRegistry,
     WebServiceAPIHandler,
@@ -58,16 +57,14 @@
     #
     # Since we called 'from __future__ import annotations' at the top, we're
     # able to use these classes as annotations **at any time**, even when they
     # wouldn't be available at runtime. That means these are all valid
     # type to notate, and will be appropriately checked when necessary. Neat!
     from _typeshed.wsgi import StartResponse, WSGIEnvironment, WSGIApplication
 
-TEXT_CONTENT_TYPE = re.compile(r"^(text|application).*$")
-
 
 class WebServiceAPIServerBase(APIServerBase):
     """
     A web service API base, useful for extension or mixins.
 
     To add functionality to the web service, use a :class:`pibble.api.server.webservice.handler.WebServiceAPIHandlerRegistry` to register methods and paths.
     """
@@ -126,20 +123,31 @@
         """
         Runs all ``register_handlers()`` methods.
 
         Used for middleware that registers handlers.
         """
         for cls in reversed(type(self).mro()):
             cls_mro = cls.mro()
-            if WebServiceAPIServerBase in cls_mro or WebServiceAPIMiddlewareBase in cls_mro:
+            if (
+                WebServiceAPIServerBase in cls_mro
+                or WebServiceAPIMiddlewareBase in cls_mro
+            ):
                 if hasattr(cls, "get_handlers") and "get_handlers" in cls.__dict__:
-                    logger.debug("Registering handlers in class {0} with 'get_handlers()'".format(cls.__name__))
+                    logger.debug(
+                        "Registering handlers in class {0} with 'get_handlers()'".format(
+                            cls.__name__
+                        )
+                    )
                     self.class_handlers.append(cls.get_handlers())
                 elif hasattr(cls, "handlers") and "handlers" in cls.__dict__:
-                    logger.debug("Registering handlers in class {0} with 'handlers'".format(cls.__name__))
+                    logger.debug(
+                        "Registering handlers in class {0} with 'handlers'".format(
+                            cls.__name__
+                        )
+                    )
                     self.class_handlers.append(cls.handlers)
 
     def prepare_all(
         self,
         request: Optional[Union[Request, RequestWrapper]] = None,
         response: Optional[Union[Response, ResponseWrapper]] = None,
         handler: Optional[
@@ -397,22 +405,14 @@
         self.prepare_all(request, response, handler)
         if logger.level == logging.DEBUG:
             logger.debug("Sending headers:")
             for header_name in response.headers:
                 logger.debug(
                     "{0}: {1}".format(header_name, response.headers[header_name])
                 )
-            if response.headers.get(
-                "Content-Encoding", None
-            ) is None and TEXT_CONTENT_TYPE.match(
-                str(response.headers.get("Content-Type", "text"))
-            ):
-                logger.debug(
-                    "Sending text: {0}".format(truncate(response.text, length=100))
-                )
         return response
 
     def wsgi(self) -> WSGIApplication:
         """
         Returns an "application" function, almost all wsgi servers expect this.
 
         :return function: The application to pass into your wsgi server of choice.
```

### Comparing `pibble-0.5.5/pibble/api/server/webservice/drivers/driver_cherrypy.py` & `pibble-0.5.6/pibble/api/server/webservice/drivers/driver_cherrypy.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/server/webservice/drivers/driver_gunicorn.py` & `pibble-0.5.6/pibble/api/server/webservice/drivers/driver_gunicorn.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 ) -> None:
     """
     Runs the gunicorn application synchronously.
     """
     options = {
         "bind": f"{host:s}:{port:d}",
         "workers": cpu_count() * 2 + 1 if workers is None else workers,
-        "worker_class": "gthread"
+        "worker_class": "gthread",
     }
 
     if secure and cert is not None and key is not None:
         options["keyfile"] = key
         options["certfile"] = cert
         logger.info(
             f"Loading SSL certificate chain from keyfile {key:s}, certfile {cert:s}"
```

### Comparing `pibble-0.5.5/pibble/api/server/webservice/drivers/driver_werkzeug.py` & `pibble-0.5.6/pibble/api/server/webservice/drivers/driver_werkzeug.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/server/webservice/handler.py` & `pibble-0.5.6/pibble/api/server/webservice/handler.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/server/webservice/jsonapi.py` & `pibble-0.5.6/pibble/api/server/webservice/jsonapi.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/server/webservice/orm.py` & `pibble-0.5.6/pibble/api/server/webservice/orm.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/server/webservice/rpc/base.py` & `pibble-0.5.6/pibble/api/server/webservice/rpc/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,23 +5,22 @@
 from pibble.api.exceptions import (
     UnsupportedMethodError,
     ConfigurationError,
 )
 from typing import Type, Optional, Union, List, Dict
 
 
-
 class RPCServerBase(MethodBasedWebServiceAPIServerBase):
     """
     A base server for RPC classes.
 
     This will handle function registration and dispatching. Inherited classes are responsible for parsing and formatting requests and responses.
     """
-    handlers = WebServiceAPIHandlerRegistry()
 
+    handlers = WebServiceAPIHandlerRegistry()
 
     def __init__(self) -> None:
         super(RPCServerBase, self).__init__()
         self.register_introspection_functions()
 
     def register_introspection_functions(self) -> None:
         """
```

### Comparing `pibble-0.5.5/pibble/api/server/webservice/rpc/jsonrpc.py` & `pibble-0.5.6/pibble/api/server/webservice/rpc/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/server/webservice/rpc/xmlrpc.py` & `pibble-0.5.6/pibble/api/server/webservice/rpc/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/server/webservice/soap.py` & `pibble-0.5.6/pibble/api/server/webservice/soap.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 
     Note that the socket will still listen on <server.host>.
 
     Optional Configuration:
       - `server.hostname`: The hostname of the server. Defaults to loopback - '127.0.0.1'.
       - `server.name`: The name of the service. Defaults to "SOAPServer".
     """
+
     handlers = WebServiceAPIHandlerRegistry()
 
     @staticmethod
     def get_type(obj: Type) -> str:
         """
         Takes a python type and turns it into the xsd equivalent.
         """
```

### Comparing `pibble-0.5.5/pibble/api/server/webservice/template/__init__.py` & `pibble-0.5.6/pibble/api/server/webservice/template/__init__.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/server/webservice/template/extensions.py` & `pibble-0.5.6/pibble/api/server/webservice/template/extensions.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/api/server/webservice/template/loader.py` & `pibble-0.5.6/pibble/api/server/webservice/template/loader.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/database/dedupe.py` & `pibble-0.5.6/pibble/database/dedupe.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/database/engine.py` & `pibble-0.5.6/pibble/database/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,18 @@
         """
         Builds the actual SQLAlchemy engine.
         """
         conn_string = URL(**{**self.connection_params, **{"database": database_name}})
         logger.info(
             "Creating SQLAlchemy engine using connection string {0}".format(conn_string)
         )
-        self.engines[database_name] = sqlalchemy.create_engine(conn_string)
+        self.engines[database_name] = sqlalchemy.create_engine(
+            conn_string, 
+            pool_reset_on_return=None, 
+        )
         if "pyodbc" in self.connection_params["drivername"]:
             if pyodbc is None:
                 raise OSError(
                     "Failed to import PyODBC. This server/container likely needs ODBC configuration."
                 )
 
             def decode_sketchy_utf16(raw_bytes: bytes) -> str:
```

### Comparing `pibble-0.5.5/pibble/database/orm.py` & `pibble-0.5.6/pibble/database/orm.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,32 +18,32 @@
 
 from typing import Optional, Type, Iterator, Any, Callable, Union, List, Dict, cast
 
 from sqlalchemy import Column, Integer, String, Sequence, ForeignKey
 
 from sqlalchemy.exc import InvalidRequestError
 
-from sqlalchemy.orm import sessionmaker, relationship, Query
+from sqlalchemy.orm import sessionmaker, scoped_session, relationship, Query
 from sqlalchemy.orm.session import Session
-from sqlalchemy.orm.state import InstanceState
-from sqlalchemy.orm.attributes import InstrumentedAttribute
-from sqlalchemy.orm.collections import InstrumentedList
+from sqlalchemy.orm.attributes import InstrumentedAttribute, ScalarAttributeImpl
 
 from sqlalchemy.engine import Dialect, Engine
 from sqlalchemy.ext.declarative import declarative_base
 
 FILE_CHUNK_SIZE = 1000
 
-class ORMQuery(Query): # type: ignore
+
+class ORMQuery(Query):  # type: ignore
     """
     A wrapper around a query which permits retrying.
     """
+
     def __init__(self, orm_session: ORMSession, arg: Any) -> None:
         self.orm_session = orm_session
-        super(ORMQuery, self).__init__(arg, session = orm_session.session)
+        super(ORMQuery, self).__init__(arg, session=orm_session.session)
 
     def reset_retry(self) -> None:
         """
         Resets the retry counter.
         """
         if hasattr(self, "_retried"):
             del self._retried
@@ -63,15 +63,17 @@
         """
         try:
             result = super(ORMQuery, self)._iter()
             return result
         except Exception as ex:
             if not self.can_retry():
                 raise
-            logger.info("Received exception {0}, retrying query.".format(type(ex).__name__))
+            logger.info(
+                "Received exception {0}, retrying query.".format(type(ex).__name__)
+            )
             logger.debug(str(ex))
             self.orm_session.reset()
             self.session = self.orm_session.session
             return self._iter()
 
 
 class ORMSession:
@@ -83,15 +85,19 @@
     Should not be instantiated manually. Call ORM.session() to instantiate.
 
     :param session Session: The SQLALchemy session to wrap around.
     :param kwargs
     """
 
     def __init__(
-        self, orm: ORM, session: Session, autocommit: Optional[bool] = False, **kwargs: Any
+        self,
+        orm: ORM,
+        session: Session,
+        autocommit: Optional[bool] = False,
+        **kwargs: Any,
     ):
         self.orm = orm
         self.session = session
         self.autocommit = autocommit
 
     def commit(self) -> None:
         """
@@ -106,25 +112,29 @@
     def close(self) -> None:
         """
         Closes the session, logs and ignores errors.
         """
         try:
             self.session.close()
         except Exception as ex:
-            logger.warning("Received {0} during close, ignoring.".format(type(ex).__name__))
+            logger.warning(
+                "Received {0} during close, ignoring.".format(type(ex).__name__)
+            )
             logger.debug(str(ex))
 
     def rollback(self) -> None:
         """
         Rolls back the session, logs and ignores errors.
         """
         try:
             self.session.rollback()
         except Exception as ex:
-            logger.warning("Received {0} during rollback, ignoring.".format(type(ex).__name__))
+            logger.warning(
+                "Received {0} during rollback, ignoring.".format(type(ex).__name__)
+            )
             logger.debug(str(ex))
 
     def get(self) -> Session:
         """
         Retrieves the underlying session.
         """
         return self.session
@@ -156,16 +166,14 @@
     def __enter__(self) -> ORMSession:
         return self
 
     def __exit__(self, *args: Any) -> None:
         try:
             if self.autocommit:
                 self.commit()
-            else:
-                self.rollback()
         finally:
             self.close()
 
 
 class ORMSolidifiedObject:
     """
     A small way to "solidify" an object.
@@ -277,33 +285,44 @@
         """
         existing_columns: List[str] = []
         existing_columns.extend(getattr(cls, "__default_hidden_columns__", []))
         existing_columns.extend(columns)
         setattr(cls, "__default_hidden_columns__", existing_columns)
 
     @staticmethod
-    def _is_sqlalchemy_data(value: Any) -> bool:
+    def _is_simple_data(value: Any) -> bool:
         """
-        A way to differentiate between sqlalchemy metadata and columnar data.
+        A way to differentiate between columnar data and other data.
+        Actually reads inheritence to ensure the object inherits from a 'primitive' type.
         """
-        return isinstance(value, InstrumentedList) or isinstance(value, InstanceState)
+        return type(value).mro()[-2] in [
+            str,
+            int,
+            float,
+            complex,
+            bool,
+            bytes,
+            bytearray,
+            memoryview,
+            type(None),
+        ]
 
-    def get_attributes(self) -> dict:
+    def get_attributes(self) -> Dict[str, Any]:
         """
         Returns the dictionary of columns (attributes) for formatting.
         """
-        return dict(
-            [
-                (k, self.__dict__[k])
-                for k in self.__dict__
-                if not k.startswith("__")
-                and not ORMObjectBase._is_sqlalchemy_data(self.__dict__[k])
-                and type(self).mro()[1] != type(self.__dict__[k]).mro()[1]
-            ]
-        )
+        attribute_dict: Dict[str, Any] = {}
+        for k in dir(self):
+            v = getattr(self, k, None)
+            v_static = getattr(type(self), k, None)
+            v_impl_type = type(getattr(v_static, "impl", None))
+            if v_impl_type is ScalarAttributeImpl:
+                attribute_dict[k] = v
+
+        return attribute_dict
 
     def see(self, *args: ORMObjectBase) -> None:
         """
         Includes an object in formatting, as a 'see-also' mechanic.
         """
         included = getattr(self, "__see_also__", [])
         setattr(self, "__see_also__", included + list(args))
@@ -596,15 +615,15 @@
 
     def session(
         self, test: bool = True, retry: bool = True, **kwargs: Any
     ) -> ORMSession:
         """
         Gets a SQLAlchemy session, and wraps it in an ORMSession.
         """
-        session = self.sessionmaker(**kwargs)
+        session = scoped_session(self.sessionmaker, **kwargs)
         if test:
             try:
                 assert session.execute("SELECT 1").fetchone()[0] == 1
             except:
                 if retry:
                     self.sessionmaker = sessionmaker(self.engine)
                     return self.session(test=True, retry=False, **kwargs)
```

### Comparing `pibble-0.5.5/pibble/database/util.py` & `pibble-0.5.6/pibble/database/util.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/ext/cms/database/__init__.py` & `pibble-0.5.6/pibble/ext/cms/database/__init__.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/ext/cms/database/interface.py` & `pibble-0.5.6/pibble/ext/cms/database/interface.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/ext/cms/database/menu.py` & `pibble-0.5.6/pibble/ext/cms/database/menu.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/ext/cms/database/view.py` & `pibble-0.5.6/pibble/ext/cms/database/view.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/ext/cms/middleware.py` & `pibble-0.5.6/pibble/ext/cms/middleware.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/ext/cms/server/base.py` & `pibble-0.5.6/pibble/ext/cms/server/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/ext/cms/server/extension.py` & `pibble-0.5.6/pibble/ext/cms/server/extension.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/ext/dam/database/files.py` & `pibble-0.5.6/pibble/ext/dam/database/files.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/ext/rest/server/base.py` & `pibble-0.5.6/pibble/ext/rest/server/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 from webob import Request, Response
 
 from typing import Any, Callable, List
 
 DEFAULT_LIMIT = 100
 
+
 class RESTExtensionServerBase(ORMWebServiceAPIServer):
     """
     Using the JSON web service and ORM extensions, provide a configurable
     interface to create HTTP handlers that follow JSON-REST standards.
 
     This requires the use of an ORM, so the configuration for the ORMBuilder
     is also required. See `pibble.database.orm.ORMBuilder`.
@@ -46,14 +47,15 @@
                   would correspond to the primary key(s) identifying a parent object.
           scope:  optional, sort of. This should be passed in to make a complete REST configuration,
                   and should correspond to the primary key of the object. This is necessary
                   for the REST server to conform to standards, as this creates unique endpoints
                   for all objects (and enables the use of DELETE and PUT endpoints, as well as
                   GET on a single object.)
     """
+
     handlers = WebServiceAPIHandlerRegistry()
 
     def paginate_object(
         self,
         request: Request,
         response: Response,
         session: ORMSession,
```

### Comparing `pibble-0.5.5/pibble/ext/rest/server/user.py` & `pibble-0.5.6/pibble/ext/rest/server/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from pibble.ext.user.server.base import (
     UserExtensionServer,
     UserExtensionHandlerRegistry,
 )
 from pibble.ext.rest.server.base import RESTExtensionServerBase
 from pibble.ext.user.database import *
 
+
 class UserRESTExtensionServerBase(UserExtensionServer, RESTExtensionServerBase):
     handlers = UserExtensionHandlerRegistry()
 
     def grant_permission_to_group(
         self, permission: Permission, user_permission_group: UserPermissionGroup
     ) -> None:
         """
```

### Comparing `pibble-0.5.5/pibble/ext/session/database/session.py` & `pibble-0.5.6/pibble/ext/session/database/session.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/ext/session/server/base.py` & `pibble-0.5.6/pibble/ext/session/server/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/ext/user/client/base.py` & `pibble-0.5.6/pibble/ext/user/client/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/ext/user/database/__init__.py` & `pibble-0.5.6/pibble/ext/user/database/__init__.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/ext/user/database/authentication.py` & `pibble-0.5.6/pibble/ext/user/database/authentication.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/ext/user/database/notification.py` & `pibble-0.5.6/pibble/ext/user/database/notification.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/ext/user/database/permission.py` & `pibble-0.5.6/pibble/ext/user/database/permission.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/ext/user/database/user.py` & `pibble-0.5.6/pibble/ext/user/database/user.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/ext/user/server/base.py` & `pibble-0.5.6/pibble/ext/user/server/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -566,14 +566,15 @@
         return cast(AuthenticationToken, token)
 
 
 class UserExtensionServer(UserExtensionServerBase):
     """
     This base class defines default handlers, if desired.
     """
+
     handlers = UserExtensionHandlerRegistry()
 
     @handlers.format()
     @handlers.methods("POST")
     @handlers.path("^/login$")
     def login(self, request: Request, response: Response) -> AuthenticationToken:
         return super(UserExtensionServer, self).login(request, response)
```

### Comparing `pibble-0.5.5/pibble/hooks/aws.py` & `pibble-0.5.6/pibble/hooks/aws.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/media/thumbnail.py` & `pibble-0.5.6/pibble/media/thumbnail.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/resources/retriever.py` & `pibble-0.5.6/pibble/resources/retriever.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/scripts/importcheck.py` & `pibble-0.5.6/pibble/scripts/importcheck.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/scripts/templatefiles.py` & `pibble-0.5.6/pibble/scripts/templatefiles.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/setup.py` & `pibble-0.5.6/pibble/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from setuptools import setup, find_packages
 
 package_name = "pibble"
 version_major = "0"
 version_minor = "5"
-version_patch = "5"
+version_patch = "6"
 
 install_requires = [
     "bcrypt>=4.0,<4.1",
     "boto3>=1.26,<2.0",
     "chardet>=5.1,<5.2",
     "click>=8.0,<9.0",
     "configparser>=5.3,<5.4",
```

### Comparing `pibble-0.5.5/pibble/util/encryption.py` & `pibble-0.5.6/pibble/util/encryption.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/util/files.py` & `pibble-0.5.6/pibble/util/files.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/util/helpers.py` & `pibble-0.5.6/pibble/util/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,17 @@
                         f"Cannot import module {module_name}. Tried {checked_paths} from {cwd}. {ex}"
                     )
             active = module
             for qualified_part in qualified_split[1:]:
                 active = getattr(active, qualified_part)
             return active
         else:
-            return local.get(qualified_name, getattr(sys.modules[__name__], qualified_name))
+            return local.get(
+                qualified_name, getattr(sys.modules[__name__], qualified_name)
+            )
     except (KeyError, AttributeError) as ex:
         raise ImportError(
             "Cannot resolve name '{0}': {1}({2})".format(
                 qualified_name, type(ex).__name__, str(ex)
             )
         )
```

### Comparing `pibble-0.5.5/pibble/util/imaging.py` & `pibble-0.5.6/pibble/util/imaging.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/util/log.py` & `pibble-0.5.6/pibble/util/log.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/util/numeric.py` & `pibble-0.5.6/pibble/util/numeric.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/util/strings.py` & `pibble-0.5.6/pibble/util/strings.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble/web/scraper.py` & `pibble-0.5.6/pibble/web/scraper.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble.egg-info/PKG-INFO` & `pibble-0.5.6/pibble.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pibble
-Version: 0.5.5
+Version: 0.5.6
 Summary: A framework for developing webapps quickly and easily using Python
 Author: Benjamin Paine
 Author-email: painebenjamin@gmail.com
 License: gpl-3.0
 Description-Content-Type: text/markdown
 Provides-Extra: mysql
 Provides-Extra: postgresql
```

### Comparing `pibble-0.5.5/pibble.egg-info/SOURCES.txt` & `pibble-0.5.6/pibble.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/pibble.egg-info/requires.txt` & `pibble-0.5.6/pibble.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pibble-0.5.5/setup.py` & `pibble-0.5.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from setuptools import setup, find_packages
 
 package_name = "pibble"
 version_major = "0"
 version_minor = "5"
-version_patch = "5"
+version_patch = "6"
 
 install_requires = [
     "bcrypt>=4.0,<4.1",
     "boto3>=1.26,<2.0",
     "chardet>=5.1,<5.2",
     "click>=8.0,<9.0",
     "configparser>=5.3,<5.4",
```

