# Comparing `tmp/blaster-server-0.0.430b0.tar.gz` & `tmp/blaster-server-0.0.431.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blaster-server-0.0.430b0.tar", last modified: Mon May 15 15:19:26 2023, max compression
+gzip compressed data, was "blaster-server-0.0.431.tar", last modified: Tue May 16 19:14:01 2023, max compression
```

## Comparing `blaster-server-0.0.430b0.tar` & `blaster-server-0.0.431.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-15 15:19:26.503753 blaster-server-0.0.430b0/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1061 2019-07-03 19:03:00.000000 blaster-server-0.0.430b0/LICENSE.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       38 2022-11-07 18:47:07.000000 blaster-server-0.0.430b0/MANIFEST.in
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      851 2023-05-15 15:19:26.503753 blaster-server-0.0.430b0/PKG-INFO
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     2620 2022-11-14 12:45:11.000000 blaster-server-0.0.430b0/README.md
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2021-10-05 11:27:02.000000 blaster-server-0.0.430b0/__init__.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-15 15:19:26.499753 blaster-server-0.0.430b0/blaster/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      875 2023-01-09 13:10:46.000000 blaster-server-0.0.430b0/blaster/__init__.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-15 15:19:26.499753 blaster-server-0.0.430b0/blaster/cloud/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       51 2022-11-09 17:29:08.000000 blaster-server-0.0.430b0/blaster/cloud/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3215 2023-04-30 12:43:59.000000 blaster-server-0.0.430b0/blaster/cloud/analytics.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-15 15:19:26.499753 blaster-server-0.0.430b0/blaster/cloud/aws/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       78 2019-07-03 19:03:00.000000 blaster-server-0.0.430b0/blaster/cloud/aws/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1371 2022-12-01 11:30:06.000000 blaster-server-0.0.430b0/blaster/cloud/aws/ses_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5221 2023-05-10 23:46:29.000000 blaster-server-0.0.430b0/blaster/cloud/push_tasks.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5297 2023-05-06 07:07:21.000000 blaster-server-0.0.430b0/blaster/cloud/storage.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3828 2023-05-15 14:10:32.000000 blaster-server-0.0.430b0/blaster/config.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3715 2023-01-28 12:57:17.000000 blaster-server-0.0.430b0/blaster/connection_pool.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       99 2020-11-22 14:37:38.000000 blaster-server-0.0.430b0/blaster/constants.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5290 2023-05-15 14:09:30.000000 blaster-server-0.0.430b0/blaster/logging.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    62877 2023-05-10 08:42:24.000000 blaster-server-0.0.430b0/blaster/mongo_orm.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    15339 2023-05-15 15:18:23.000000 blaster-server-0.0.430b0/blaster/schema.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    36583 2023-04-18 10:02:10.000000 blaster-server-0.0.430b0/blaster/server.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    46443 2023-05-15 14:15:15.000000 blaster-server-0.0.430b0/blaster/tools.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-15 15:19:26.503753 blaster-server-0.0.430b0/blaster/utils/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2019-07-03 19:03:00.000000 blaster-server-0.0.430b0/blaster/utils/__init__.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-15 15:19:26.503753 blaster-server-0.0.430b0/blaster/utils/data/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    53078 2022-11-08 15:22:07.000000 blaster-server-0.0.430b0/blaster/utils/data/countries.json
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)   119011 2022-12-01 10:20:50.000000 blaster-server-0.0.430b0/blaster/utils/data/mime_types.json
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     7085 2023-05-14 10:13:13.000000 blaster-server-0.0.430b0/blaster/utils/data_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1951 2023-01-07 12:42:21.000000 blaster-server-0.0.430b0/blaster/utils/events.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     4812 2023-03-30 16:36:26.000000 blaster-server-0.0.430b0/blaster/utils/fork.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1076 2023-02-21 07:52:48.000000 blaster-server-0.0.430b0/blaster/utils/lat_long_utils.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     5564 2023-05-09 13:55:03.000000 blaster-server-0.0.430b0/blaster/utils/phone_number_utils.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     6773 2020-12-14 07:56:42.000000 blaster-server-0.0.430b0/blaster/utils/xss_html.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-15 15:19:26.503753 blaster-server-0.0.430b0/blaster/websocket/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1022 2019-07-03 19:03:00.000000 blaster-server-0.0.430b0/blaster/websocket/__init__.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    12874 2019-07-03 19:03:00.000000 blaster-server-0.0.430b0/blaster/websocket/_abnf.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    11136 2022-01-06 11:42:20.000000 blaster-server-0.0.430b0/blaster/websocket/_app.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    16360 2019-07-03 19:03:00.000000 blaster-server-0.0.430b0/blaster/websocket/_core.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     2141 2019-07-03 19:03:00.000000 blaster-server-0.0.430b0/blaster/websocket/_exceptions.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     4793 2019-07-03 19:03:00.000000 blaster-server-0.0.430b0/blaster/websocket/_handshake.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     7288 2019-07-03 19:03:00.000000 blaster-server-0.0.430b0/blaster/websocket/_http.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1870 2019-07-03 19:03:00.000000 blaster-server-0.0.430b0/blaster/websocket/_logging.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     3623 2019-07-03 19:03:00.000000 blaster-server-0.0.430b0/blaster/websocket/_socket.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1550 2019-07-03 19:03:00.000000 blaster-server-0.0.430b0/blaster/websocket/_ssl_compat.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     3670 2019-07-03 19:03:00.000000 blaster-server-0.0.430b0/blaster/websocket/_url.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     3632 2019-07-03 19:03:00.000000 blaster-server-0.0.430b0/blaster/websocket/_utils.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    12758 2021-10-03 12:23:56.000000 blaster-server-0.0.430b0/blaster/websocket/server.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-15 15:19:26.503753 blaster-server-0.0.430b0/blaster/websocket/tests/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2019-07-03 19:03:00.000000 blaster-server-0.0.430b0/blaster/websocket/tests/__init__.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    26115 2019-07-03 19:03:00.000000 blaster-server-0.0.430b0/blaster/websocket/tests/test_websocket.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-15 15:19:26.503753 blaster-server-0.0.430b0/blaster_server.egg-info/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      851 2023-05-15 15:19:26.000000 blaster-server-0.0.430b0/blaster_server.egg-info/PKG-INFO
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1682 2023-05-15 15:19:26.000000 blaster-server-0.0.430b0/blaster_server.egg-info/SOURCES.txt
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        1 2023-05-15 15:19:26.000000 blaster-server-0.0.430b0/blaster_server.egg-info/dependency_links.txt
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      221 2023-05-15 15:19:26.000000 blaster-server-0.0.430b0/blaster_server.egg-info/requires.txt
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       41 2023-05-15 15:19:26.000000 blaster-server-0.0.430b0/blaster_server.egg-info/top_level.txt
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-15 15:19:26.503753 blaster-server-0.0.430b0/examples/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2019-07-03 19:03:00.000000 blaster-server-0.0.430b0/examples/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      266 2022-01-06 11:42:20.000000 blaster-server-0.0.430b0/examples/fast_api_test.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      636 2019-07-03 19:03:00.000000 blaster-server-0.0.430b0/examples/gevent_wsgi_test.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      233 2021-10-04 14:48:01.000000 blaster-server-0.0.430b0/examples/meinheld_flask.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1743 2022-06-17 17:10:40.000000 blaster-server-0.0.430b0/examples/mongo_ormexample.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2386 2022-11-14 12:13:43.000000 blaster-server-0.0.430b0/examples/simple_examples.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1088 2019-07-03 19:03:00.000000 blaster-server-0.0.430b0/examples/test_chat_room.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      614 2021-02-24 01:34:32.000000 blaster-server-0.0.430b0/examples/tornado_hello_world.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      791 2021-02-24 01:20:44.000000 blaster-server-0.0.430b0/examples/wheezy_hello.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       79 2023-05-15 15:19:26.503753 blaster-server-0.0.430b0/setup.cfg
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1560 2023-05-15 14:58:42.000000 blaster-server-0.0.430b0/setup.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-15 15:19:26.503753 blaster-server-0.0.430b0/test/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2022-07-26 21:35:40.000000 blaster-server-0.0.430b0/test/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6851 2023-01-07 00:03:08.000000 blaster-server-0.0.430b0/test/test_mongo_orm.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      503 2022-11-07 18:31:41.000000 blaster-server-0.0.430b0/test/test_schema.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     5457 2022-12-09 21:19:51.000000 blaster-server-0.0.430b0/test/test_tools.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-16 18:26:08.000000 blaster-server-0.0.430b0/test/test_utils.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      615 2021-02-24 11:15:27.000000 blaster-server-0.0.430b0/test/timeit_snippets.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-16 19:14:01.247362 blaster-server-0.0.431/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1061 2019-07-03 19:03:00.000000 blaster-server-0.0.431/LICENSE.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       38 2022-11-07 18:47:07.000000 blaster-server-0.0.431/MANIFEST.in
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      849 2023-05-16 19:14:01.247362 blaster-server-0.0.431/PKG-INFO
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     2620 2022-11-14 12:45:11.000000 blaster-server-0.0.431/README.md
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2021-10-05 11:27:02.000000 blaster-server-0.0.431/__init__.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-16 19:14:01.243362 blaster-server-0.0.431/blaster/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      875 2023-01-09 13:10:46.000000 blaster-server-0.0.431/blaster/__init__.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-16 19:14:01.243362 blaster-server-0.0.431/blaster/cloud/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       51 2022-11-09 17:29:08.000000 blaster-server-0.0.431/blaster/cloud/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3215 2023-04-30 12:43:59.000000 blaster-server-0.0.431/blaster/cloud/analytics.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-16 19:14:01.247362 blaster-server-0.0.431/blaster/cloud/aws/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       78 2019-07-03 19:03:00.000000 blaster-server-0.0.431/blaster/cloud/aws/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1371 2022-12-01 11:30:06.000000 blaster-server-0.0.431/blaster/cloud/aws/ses_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5221 2023-05-10 23:46:29.000000 blaster-server-0.0.431/blaster/cloud/push_tasks.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5297 2023-05-06 07:07:21.000000 blaster-server-0.0.431/blaster/cloud/storage.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3828 2023-05-15 14:10:32.000000 blaster-server-0.0.431/blaster/config.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3715 2023-01-28 12:57:17.000000 blaster-server-0.0.431/blaster/connection_pool.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       99 2020-11-22 14:37:38.000000 blaster-server-0.0.431/blaster/constants.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5290 2023-05-15 14:09:30.000000 blaster-server-0.0.431/blaster/logging.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    62877 2023-05-10 08:42:24.000000 blaster-server-0.0.431/blaster/mongo_orm.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    15096 2023-05-16 19:07:33.000000 blaster-server-0.0.431/blaster/schema.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    36583 2023-04-18 10:02:10.000000 blaster-server-0.0.431/blaster/server.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    46443 2023-05-15 14:15:15.000000 blaster-server-0.0.431/blaster/tools.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-16 19:14:01.247362 blaster-server-0.0.431/blaster/utils/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2019-07-03 19:03:00.000000 blaster-server-0.0.431/blaster/utils/__init__.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-16 19:14:01.247362 blaster-server-0.0.431/blaster/utils/data/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    53078 2022-11-08 15:22:07.000000 blaster-server-0.0.431/blaster/utils/data/countries.json
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)   119011 2022-12-01 10:20:50.000000 blaster-server-0.0.431/blaster/utils/data/mime_types.json
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     7085 2023-05-14 10:13:13.000000 blaster-server-0.0.431/blaster/utils/data_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1951 2023-01-07 12:42:21.000000 blaster-server-0.0.431/blaster/utils/events.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     4812 2023-03-30 16:36:26.000000 blaster-server-0.0.431/blaster/utils/fork.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1076 2023-02-21 07:52:48.000000 blaster-server-0.0.431/blaster/utils/lat_long_utils.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     5564 2023-05-09 13:55:03.000000 blaster-server-0.0.431/blaster/utils/phone_number_utils.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     6773 2020-12-14 07:56:42.000000 blaster-server-0.0.431/blaster/utils/xss_html.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-16 19:14:01.247362 blaster-server-0.0.431/blaster/websocket/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1022 2019-07-03 19:03:00.000000 blaster-server-0.0.431/blaster/websocket/__init__.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    12874 2019-07-03 19:03:00.000000 blaster-server-0.0.431/blaster/websocket/_abnf.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    11136 2022-01-06 11:42:20.000000 blaster-server-0.0.431/blaster/websocket/_app.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    16360 2019-07-03 19:03:00.000000 blaster-server-0.0.431/blaster/websocket/_core.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     2141 2019-07-03 19:03:00.000000 blaster-server-0.0.431/blaster/websocket/_exceptions.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     4793 2019-07-03 19:03:00.000000 blaster-server-0.0.431/blaster/websocket/_handshake.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     7288 2019-07-03 19:03:00.000000 blaster-server-0.0.431/blaster/websocket/_http.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1870 2019-07-03 19:03:00.000000 blaster-server-0.0.431/blaster/websocket/_logging.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     3623 2019-07-03 19:03:00.000000 blaster-server-0.0.431/blaster/websocket/_socket.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1550 2019-07-03 19:03:00.000000 blaster-server-0.0.431/blaster/websocket/_ssl_compat.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     3670 2019-07-03 19:03:00.000000 blaster-server-0.0.431/blaster/websocket/_url.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     3632 2019-07-03 19:03:00.000000 blaster-server-0.0.431/blaster/websocket/_utils.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    12758 2021-10-03 12:23:56.000000 blaster-server-0.0.431/blaster/websocket/server.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-16 19:14:01.247362 blaster-server-0.0.431/blaster/websocket/tests/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2019-07-03 19:03:00.000000 blaster-server-0.0.431/blaster/websocket/tests/__init__.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    26115 2019-07-03 19:03:00.000000 blaster-server-0.0.431/blaster/websocket/tests/test_websocket.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-16 19:14:01.247362 blaster-server-0.0.431/blaster_server.egg-info/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      849 2023-05-16 19:14:01.000000 blaster-server-0.0.431/blaster_server.egg-info/PKG-INFO
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1682 2023-05-16 19:14:01.000000 blaster-server-0.0.431/blaster_server.egg-info/SOURCES.txt
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        1 2023-05-16 19:14:01.000000 blaster-server-0.0.431/blaster_server.egg-info/dependency_links.txt
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      221 2023-05-16 19:14:01.000000 blaster-server-0.0.431/blaster_server.egg-info/requires.txt
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       41 2023-05-16 19:14:01.000000 blaster-server-0.0.431/blaster_server.egg-info/top_level.txt
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-16 19:14:01.247362 blaster-server-0.0.431/examples/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2019-07-03 19:03:00.000000 blaster-server-0.0.431/examples/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      266 2022-01-06 11:42:20.000000 blaster-server-0.0.431/examples/fast_api_test.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      636 2019-07-03 19:03:00.000000 blaster-server-0.0.431/examples/gevent_wsgi_test.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      233 2021-10-04 14:48:01.000000 blaster-server-0.0.431/examples/meinheld_flask.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1743 2022-06-17 17:10:40.000000 blaster-server-0.0.431/examples/mongo_ormexample.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2386 2022-11-14 12:13:43.000000 blaster-server-0.0.431/examples/simple_examples.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1088 2019-07-03 19:03:00.000000 blaster-server-0.0.431/examples/test_chat_room.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      614 2021-02-24 01:34:32.000000 blaster-server-0.0.431/examples/tornado_hello_world.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      791 2021-02-24 01:20:44.000000 blaster-server-0.0.431/examples/wheezy_hello.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       79 2023-05-16 19:14:01.247362 blaster-server-0.0.431/setup.cfg
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1559 2023-05-16 19:07:33.000000 blaster-server-0.0.431/setup.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-16 19:14:01.247362 blaster-server-0.0.431/test/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2022-07-26 21:35:40.000000 blaster-server-0.0.431/test/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6851 2023-01-07 00:03:08.000000 blaster-server-0.0.431/test/test_mongo_orm.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1068 2023-05-16 19:13:33.000000 blaster-server-0.0.431/test/test_schema.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     5457 2022-12-09 21:19:51.000000 blaster-server-0.0.431/test/test_tools.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-16 18:26:08.000000 blaster-server-0.0.431/test/test_utils.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      615 2021-02-24 11:15:27.000000 blaster-server-0.0.431/test/timeit_snippets.py
```

### Comparing `blaster-server-0.0.430b0/LICENSE.txt` & `blaster-server-0.0.431/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.430b0/PKG-INFO` & `blaster-server-0.0.431/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaster-server
-Version: 0.0.430b0
+Version: 0.0.431
 Summary: Gevent based python server built from scratch for maximum performance
 Home-page: https://github.com/abhinavabcd/blaster
 Author: Abhinav Reddy
 Author-email: abhinavabcd@gmail.com
 License: MIT
 Download-URL: https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz
 Keywords: server,superfast,Like FastApi or Flask but 10x faster
```

### Comparing `blaster-server-0.0.430b0/README.md` & `blaster-server-0.0.431/README.md`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.430b0/blaster/__init__.py` & `blaster-server-0.0.431/blaster/__init__.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.430b0/blaster/cloud/analytics.py` & `blaster-server-0.0.431/blaster/cloud/analytics.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.430b0/blaster/cloud/aws/ses_utils.py` & `blaster-server-0.0.431/blaster/cloud/aws/ses_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.430b0/blaster/cloud/push_tasks.py` & `blaster-server-0.0.431/blaster/cloud/push_tasks.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.430b0/blaster/cloud/storage.py` & `blaster-server-0.0.431/blaster/cloud/storage.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.430b0/blaster/config.py` & `blaster-server-0.0.431/blaster/config.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.430b0/blaster/connection_pool.py` & `blaster-server-0.0.431/blaster/connection_pool.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.430b0/blaster/logging.py` & `blaster-server-0.0.431/blaster/logging.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.430b0/blaster/mongo_orm.py` & `blaster-server-0.0.431/blaster/mongo_orm.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.430b0/blaster/schema.py` & `blaster-server-0.0.431/blaster/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,20 +53,18 @@
 		if(self._min != _OBJ_END_):
 			_schema["minimum"] = self._min
 		if(self._max != _OBJ_END_):
 			_schema["maximum"] = self._max
 		if(self.one_of):
 			_schema["enum"] = list(self.one_of)
 
-	def validate(self, e, default=_OBJ_END_):
+	def validate(self, e):
 		if(e == None):
 			if(self._default != _OBJ_END_):
 				return self._default
-			if(default != _OBJ_END_):
-				return default
 			raise TypeError("should be int")
 		if(isinstance(e, str) and len(e) > 50):
 			raise TypeError("should be valid int")
 		e = self._type(e)
 		if(self._min != _OBJ_END_ and e < self._min):
 			raise TypeError("should be minlen {:d}".format(self._min))
 		if(self._max != _OBJ_END_ and e > self._max):
@@ -121,26 +119,29 @@
 		if(self.one_of):
 			_schema["enum"] = list(self.one_of)
 		if(regex):
 			_schema["pattern"] = regex
 		if(_fmt):
 			_schema["format"] = _fmt
 
-	def validate(self, e, default=_OBJ_END_):
+	def validate(self, e):
 		if(self.before):
 			e = (e != None) and self.before(e)
+		_default = self._default
 		if(e == None):
-			if(self._default != _OBJ_END_):
-				return self._default
-			if(default != _OBJ_END_):
-				return default
+			if(_default != _OBJ_END_):
+				return _default
 			raise TypeError("should be string")
 		if(not isinstance(e, str)):
 			e = str(e)
+		# e is a string now
 		if(len(e) < self.minlen):
+			if(not e):  # empty string allowed if minlen is 0 or default is set
+				if(_default != _OBJ_END_):
+					return _default
 			raise TypeError("should be minlen {:d}".format(self.minlen))
 		if(len(e) > self.maxlen):
 			e = e[:self.maxlen]
 		if(self.one_of and e not in self.one_of):
 			raise TypeError("should be one of {}".format(self.one_of))
 		if(self.regex and not self.regex.fullmatch(e)):
 			raise TypeError("did not match the pattern {}".format(self.one_of))
@@ -204,36 +205,34 @@
 		self._default = default
 		self._name = _name
 		self._schema_ = {
 			"type": "object",
 			"additionalProperties": schema(val_type)[0]
 		}
 
-	def validate(self, e, default=_OBJ_END_):
-		if(e == None):
+	def validate(self, e):
+		if(e == None or not isinstance(e, dict)):
 			if(self._default != _OBJ_END_):
-				return self._default
-			if(default != _OBJ_END_):
-				return default
+				return dict(self._default) if self._default != None else None
+			raise TypeError("should be a dict")
 
-		if(not isinstance(e, dict)):
-			return e
 		for k in list(e.keys()):
 			if(self.key_ype_validator(k) == None):
 				e.pop(k)
 				continue
 			e[k] = self.val_type_validator(e[k])
 		return e
 
 	def __getitem__(self, *kv):
 		return _Dict(
-			str if len(kv) < 2 else kv[-2], 
+			str if len(kv) < 2 else kv[-2],
 			str if len(kv) < 1 else kv[-1]
 		)
 
+
 class Object:
 	def __init__(self, default=_OBJ_END_, _required_=None, _name=None, **keys):
 		self._default = default
 		self._required = set(_required_) if _required_ else set()
 		self._name = _name
 
 		# instance specific: Ex: Object(a=Int, b=Str)
@@ -258,23 +257,18 @@
 
 	# validates Object(a=str, b=int, h=Test).validate({} or obj or string)
 	# validates ObjectClass.validate({} or )
 	def validate(self):
 		self.__class__.validate(self)  # resets internal dict
 
 	@classmethod
-	def validate(cls, obj):  # obj -> instance of dict, cls, str
-		if(isinstance(obj, dict)):
-			return cls.from_dict(obj)
-		elif(isinstance(obj, str)):
-			return cls.from_dict(json.loads(obj))
-
+	def validate(cls, obj, set_obj=None):  # obj -> instance of dict, cls, str
 		# regular class instance
 		# validate __dict__ of the instance inplace
-		e = obj.__dict__
+		e = obj.__dict__ if not isinstance(obj, dict) else obj
 		k = None
 		attr_value = None
 		try:
 			for k, attr_validation in cls._validations.items():
 				attr_value = e.get(k, _OBJ_END_)
 				if(attr_value != _OBJ_END_):
 					_validated_attr = attr_validation(attr_value)
@@ -283,44 +277,34 @@
 					_validated_attr = getattr(cls, k, None)
 
 				if(_validated_attr == None and k in cls._required):
 					raise TypeError("Field is required")
 
 				if(_validated_attr != attr_value):
 					e[k] = _validated_attr
+
+				if(set_obj):
+					setattr(set_obj, k, _validated_attr)
+
 			return obj
 		except Exception as ex:
 			raise TypeError({
 				"exception": (ex.args and ex.args[0]) or "Validation failed",
 				"key": k,
 				"value": attr_value,
 				"schema": cls._properties[k]
 			})
 
-	def from_dict(self, _dict: dict, default=_OBJ_END_):
-		return self.__class__.from_dict(_dict, default=default)
-
 	@classmethod
-	def from_dict(cls, _dict: dict, default=_OBJ_END_):
+	def from_dict(cls, _dict: dict):
 		ret = cls()
-		for _k, (k, _validator, _default) in cls._dict_key_to_object_key.items():
-			if((_v := _dict.get(_k, _OBJ_END_)) != _OBJ_END_):
-				# value exists
-				try:
-					setattr(ret, k, _validator(_v))
-				except Exception as ex:
-					raise Exception(f"key: {_k}/{k} failed validation: {_v} -> {ex}")
-			elif(_default != _OBJ_END_):
-				# key doesn't exists, if default exists it's set,
-				# else raises error with missing key
-				setattr(ret, k, _default)
-			elif(default != _OBJ_END_):
-				return default
-			else:
-				raise Exception(f"missing key: {_k}/{k}")
+		for _k, k in cls._dict_key_to_object_key.items():
+			if(_k in _dict):
+				_dict[_k] = _dict.pop(_k)
+		cls.validate(_dict, set_obj=ret)
 		return ret
 
 	def to_dict(self):
 		ret = {}
 		for k, attr_validation in self.__class__._validations.items():
 			ret[k] = getattr(self, k, None)
 		return ret
@@ -360,15 +344,15 @@
 	raise TypeError("Cannot be none")
 
 
 def array_validation(_type, arr, simple_types=None, complex_validations=None, mix=False, nullable=True):
 	# sequece
 	if(arr == None):
 		if(_type._default != _OBJ_END_):
-			return _type._default
+			return list(_type._default) if _type._default != None else None
 		if(nullable):
 			return None
 		raise TypeError("Cannot be none")
 	if(not isinstance(arr, list)):
 		arr = json.loads(arr)
 
 	filter_nones = False
@@ -409,15 +393,15 @@
 # List[str, int]-> anyOf int, str
 # List[[str, int]] -> oneOf int, str
 
 # Object(id=int, name=str)
 # Dict[str, int]
 
 # given any instance/class, returns schema, _validation function
-def schema(x):
+def schema(x, _default=_OBJ_END_):
 
 	if(isinstance(x, _Optional)):
 		_schema, _validator = schema(x._types[0])
 		return _schema, _validator
 	if(isinstance(x, _Required)):
 		_schema, _validator = schema(x._types[0])
 		_schema["required"] = True
@@ -434,15 +418,19 @@
 		x._validations = _validations = {}
 		x._properties = _properties = {}
 		x._property_types = {}
 		x._required = _required = set()
 		x._dict_key_to_object_key = {}  # used when converting json/dict to object
 
 		for k, _type in get_type_hints(x).items():
-			is_required = True
+
+			# pure type to instance of schema types
+			_default_value = x.__dict__.get(k, _OBJ_END_)  # declaration default
+			is_required = _default_value == _OBJ_END_
+
 			if(
 				_type.__module__ == 'typing'
 				and getattr(_type, "__origin__", None) == typing.Union
 				and getattr(_type, "__args__", None)
 			):
 				# union
 				_type = _type.__args__[0]
@@ -452,46 +440,23 @@
 				_type = _type._types[0]
 				is_required = False
 
 			elif(isinstance(_type, _Required)):
 				# required
 				_type = _type._types[0]
 
-			# pure type to instance of schema types
-			_default = x.__dict__.get(k, _OBJ_END_)  # declaration default
-			if(_type == int or _type == Int):
-				_type = Int(default=_default)
-
-			elif(_type == float):
-				_type = Float(default=_default)
-
-			elif(_type == str or _type == Str):
-				_type = Str(default=_default)
-
-			elif(_type == Array or _type == list):  # genric
-				# make a copy if default exists
-				_default_copy = list(_default) if (_default and _default != _OBJ_END_) else _default
-				_type = Array(None, default=_default_copy)
-
-			elif(_type == dict or _type == Dict):  # generic without any attributes
-				_default_copy = dict(_default) if (_default and _default != _OBJ_END_) else _default
-				_type = _Dict(None, None, default=_default_copy)
-
-			_schema_and_validation = schema(_type)
+			_schema_and_validation = schema(_type, _default=_default_value)
 			if(_schema_and_validation):
 				_properties[k], _validations[k] = _schema_and_validation
-				if(_default != _OBJ_END_):  # ? and not isinstance(_type, type)):
-					is_required = False
 
 				is_required and _required.add(k)
 				# keep track of propeties
 				x._property_types[k] = _type
-				dict_key = getattr(_type, "_name", None) or k
-				x._dict_key_to_object_key[dict_key] \
-					= (k, _validations[k], _default)
+				if(dict_key := getattr(_type, "_name", None)):
+					x._dict_key_to_object_key[dict_key] = k
 		# create schema
 		x._schema_ = ret = schema.defs[x.__name__] = {
 			"type": "object",
 		}
 		_title = getattr(x, "_title_", None)
 		_description = getattr(x, "_description_", None)
 		if(_title):
@@ -541,26 +506,61 @@
 			item_validation,
 			simple_types=tuple(simple_types),
 			complex_validations=complex_validations,
 			nullable=is_nullable
 		)
 
 	elif(isinstance(x, Str)):
+		if(_default != _OBJ_END_):
+			x._default = _default
+			x._schema_["default"] = _default
 		return x._schema_, x.validate
 
 	elif(isinstance(x, Int)):
+		if(_default != _OBJ_END_):
+			x._default = _default
+			x._schema_["default"] = _default
 		return x._schema_, x.validate
 
 	elif(isinstance(x, _Dict)):
+		if(_default != _OBJ_END_):
+			x._default = _default
+			x._schema_["default"] = _default
 		return x._schema_, x.validate
 
 	elif(isinstance(x, Array)):  # Array(_types)
+		if(_default != _OBJ_END_):
+			x._default = _default
+			x._schema_["default"] = _default
 		return x._schema_, x.validate
 
 	elif(isinstance(x, Object)):  # Object(id=Array)
+		if(_default != _OBJ_END_):
+			x._default = _default
+		return x._schema_, x.validate
+
+	elif(x == int or x == Int):
+		x = Int(default=_default)
+		return x._schema_, x.validate
+
+	elif(x == float):
+		x = Float(default=_default)
+		return x._schema_, x.validate
+
+	elif(x == str or x == Str):
+		x = Str(default=_default)
+		return x._schema_, x.validate
+
+	elif(x == Array or x == list):  # genric
+		# make a copy if default exists
+		x = Array(None, default=_default)
+		return x._schema_, x.validate
+
+	elif(x == dict or x == _Dict):  # generic without any attributes
+		x = _Dict(None, None, default=_default)
 		return x._schema_, x.validate
 
 	else:
 		return {"AnyValue": {}}, lambda x: x
 
 
 # Defs, that require schema to be defined
```

### Comparing `blaster-server-0.0.430b0/blaster/server.py` & `blaster-server-0.0.431/blaster/server.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.430b0/blaster/tools.py` & `blaster-server-0.0.431/blaster/tools.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.430b0/blaster/utils/data/countries.json` & `blaster-server-0.0.431/blaster/utils/data/countries.json`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.430b0/blaster/utils/data/mime_types.json` & `blaster-server-0.0.431/blaster/utils/data/mime_types.json`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.430b0/blaster/utils/data_utils.py` & `blaster-server-0.0.431/blaster/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.430b0/blaster/utils/events.py` & `blaster-server-0.0.431/blaster/utils/events.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.430b0/blaster/utils/fork.py` & `blaster-server-0.0.431/blaster/utils/fork.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.430b0/blaster/utils/lat_long_utils.py` & `blaster-server-0.0.431/blaster/utils/lat_long_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.430b0/blaster/utils/phone_number_utils.py` & `blaster-server-0.0.431/blaster/utils/phone_number_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.430b0/blaster/utils/xss_html.py` & `blaster-server-0.0.431/blaster/utils/xss_html.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.430b0/blaster/websocket/__init__.py` & `blaster-server-0.0.431/blaster/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.430b0/blaster/websocket/_abnf.py` & `blaster-server-0.0.431/blaster/websocket/_abnf.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.430b0/blaster/websocket/_app.py` & `blaster-server-0.0.431/blaster/websocket/_app.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.430b0/blaster/websocket/_core.py` & `blaster-server-0.0.431/blaster/websocket/_core.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.430b0/blaster/websocket/_exceptions.py` & `blaster-server-0.0.431/blaster/websocket/_exceptions.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.430b0/blaster/websocket/_handshake.py` & `blaster-server-0.0.431/blaster/websocket/_handshake.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.430b0/blaster/websocket/_http.py` & `blaster-server-0.0.431/blaster/websocket/_http.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.430b0/blaster/websocket/_logging.py` & `blaster-server-0.0.431/blaster/websocket/_logging.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.430b0/blaster/websocket/_socket.py` & `blaster-server-0.0.431/blaster/websocket/_socket.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.430b0/blaster/websocket/_ssl_compat.py` & `blaster-server-0.0.431/blaster/websocket/_ssl_compat.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.430b0/blaster/websocket/_url.py` & `blaster-server-0.0.431/blaster/websocket/_url.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.430b0/blaster/websocket/_utils.py` & `blaster-server-0.0.431/blaster/websocket/_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.430b0/blaster/websocket/server.py` & `blaster-server-0.0.431/blaster/websocket/server.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.430b0/blaster/websocket/tests/test_websocket.py` & `blaster-server-0.0.431/blaster/websocket/tests/test_websocket.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.430b0/blaster_server.egg-info/PKG-INFO` & `blaster-server-0.0.431/blaster_server.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaster-server
-Version: 0.0.430b0
+Version: 0.0.431
 Summary: Gevent based python server built from scratch for maximum performance
 Home-page: https://github.com/abhinavabcd/blaster
 Author: Abhinav Reddy
 Author-email: abhinavabcd@gmail.com
 License: MIT
 Download-URL: https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz
 Keywords: server,superfast,Like FastApi or Flask but 10x faster
```

### Comparing `blaster-server-0.0.430b0/blaster_server.egg-info/SOURCES.txt` & `blaster-server-0.0.431/blaster_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.430b0/examples/gevent_wsgi_test.py` & `blaster-server-0.0.431/examples/gevent_wsgi_test.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.430b0/examples/mongo_ormexample.py` & `blaster-server-0.0.431/examples/mongo_ormexample.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.430b0/examples/simple_examples.py` & `blaster-server-0.0.431/examples/simple_examples.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.430b0/examples/test_chat_room.py` & `blaster-server-0.0.431/examples/test_chat_room.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.430b0/examples/tornado_hello_world.py` & `blaster-server-0.0.431/examples/tornado_hello_world.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.430b0/examples/wheezy_hello.py` & `blaster-server-0.0.431/examples/wheezy_hello.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.430b0/setup.py` & `blaster-server-0.0.431/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
 	name='blaster-server',
 	packages=find_packages() + ["blaster/utils/data"],
-	version='0.0.430b',
+	version='0.0.431',
 	license='MIT',
 	description='Gevent based python server built from scratch for maximum performance',
 	author='Abhinav Reddy',                   # Type in your name
 	author_email='abhinavabcd@gmail.com',      # Type in your E-Mail
 	url='https://github.com/abhinavabcd/blaster',
 	download_url='https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz',
 	keywords=['server', 'superfast', 'Like FastApi or Flask but 10x faster'],
```

### Comparing `blaster-server-0.0.430b0/test/test_mongo_orm.py` & `blaster-server-0.0.431/test/test_mongo_orm.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.430b0/test/test_tools.py` & `blaster-server-0.0.431/test/test_tools.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.430b0/test/test_utils.py` & `blaster-server-0.0.431/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.430b0/test/timeit_snippets.py` & `blaster-server-0.0.431/test/timeit_snippets.py`

 * *Files identical despite different names*

