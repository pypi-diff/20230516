# Comparing `tmp/wechat_api-0.1.0.tar.gz` & `tmp/wechat_api-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wechat_api-0.1.0.tar", last modified: Fri May  5 10:39:35 2023, max compression
+gzip compressed data, was "wechat_api-0.1.1.tar", last modified: Tue May 16 06:31:36 2023, max compression
```

## Comparing `wechat_api-0.1.0.tar` & `wechat_api-0.1.1.tar`

### file list

```diff
@@ -1,3 +1,26 @@
--rw-r--r--   0        0        0       18 2023-05-05 10:37:32.585358 wechat_api-0.1.0/README.md
--rw-r--r--   0        0        0      435 2023-05-05 10:39:35.981223 wechat_api-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      195 1970-01-01 00:00:00.000000 wechat_api-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       41 2023-05-16 06:25:51.254610 wechat_api-0.1.1/README.md
+-rw-r--r--   0        0        0      586 2023-05-16 06:31:36.417178 wechat_api-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      102 2023-05-16 06:18:26.129740 wechat_api-0.1.1/wechat_api/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:18:26.129740 wechat_api-0.1.1/wechat_api/aispeech.py
+-rw-r--r--   0        0        0     5637 2023-05-16 06:18:26.130740 wechat_api-0.1.1/wechat_api/base.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:18:26.130740 wechat_api-0.1.1/wechat_api/channels.py
+-rw-r--r--   0        0        0     1897 2023-05-16 06:18:26.131740 wechat_api-0.1.1/wechat_api/core.py
+-rw-r--r--   0        0        0     1154 2023-05-16 06:18:26.132127 wechat_api-0.1.1/wechat_api/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:18:26.132127 wechat_api-0.1.1/wechat_api/game.py
+-rw-r--r--   0        0        0    30509 2023-05-16 06:18:26.132127 wechat_api-0.1.1/wechat_api/mini.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:18:26.133137 wechat_api-0.1.1/wechat_api/models/__init__.py
+-rw-r--r--   0        0        0      409 2023-05-16 06:18:26.133137 wechat_api-0.1.1/wechat_api/models/base.py
+-rw-r--r--   0        0        0      503 2023-05-16 06:18:26.134136 wechat_api-0.1.1/wechat_api/models/mini.py
+-rw-r--r--   0        0        0     3047 2023-05-16 06:18:26.134136 wechat_api-0.1.1/wechat_api/models/pay.py
+-rw-r--r--   0        0        0      444 2023-05-16 06:18:26.134136 wechat_api-0.1.1/wechat_api/models/platform.py
+-rw-r--r--   0        0        0     1120 2023-05-16 06:18:26.135136 wechat_api-0.1.1/wechat_api/models/request.py
+-rw-r--r--   0        0        0     1861 2023-05-16 06:18:26.135611 wechat_api-0.1.1/wechat_api/models/state.py
+-rw-r--r--   0        0        0     1774 2023-05-16 06:18:26.135611 wechat_api-0.1.1/wechat_api/offi.py
+-rw-r--r--   0        0        0     6518 2023-05-16 06:18:26.136621 wechat_api-0.1.1/wechat_api/pay.py
+-rw-r--r--   0        0        0     1839 2023-05-16 06:18:26.136621 wechat_api-0.1.1/wechat_api/platform.py
+-rw-r--r--   0        0        0      264 2023-05-16 06:18:26.136621 wechat_api-0.1.1/wechat_api/state.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:18:26.136621 wechat_api-0.1.1/wechat_api/store.py
+-rw-r--r--   0        0        0     5958 2023-05-16 06:18:26.137621 wechat_api-0.1.1/wechat_api/tools.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:18:26.137621 wechat_api-0.1.1/wechat_api/work.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:18:26.137621 wechat_api-0.1.1/wechat_api/xwei.py
+-rw-r--r--   0        0        0      376 1970-01-01 00:00:00.000000 wechat_api-0.1.1/PKG-INFO
```

