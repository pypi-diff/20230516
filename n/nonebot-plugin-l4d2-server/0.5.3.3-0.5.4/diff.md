# Comparing `tmp/nonebot_plugin_l4d2_server-0.5.3.3.tar.gz` & `tmp/nonebot_plugin_l4d2_server-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_l4d2_server-0.5.3.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_l4d2_server-0.5.4.tar", max compression
```

## Comparing `nonebot_plugin_l4d2_server-0.5.3.3.tar` & `nonebot_plugin_l4d2_server-0.5.4.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0    35149 2023-05-16 02:17:23.780502 nonebot_plugin_l4d2_server-0.5.3.3/LICENSE
--rw-r--r--   0        0        0    11200 2023-05-16 02:17:23.780502 nonebot_plugin_l4d2_server-0.5.3.3/README.md
--rw-r--r--   0        0        0    17490 2023-05-16 02:17:23.784502 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/__init__.py
--rw-r--r--   0        0        0   158357 2023-05-16 02:17:23.784502 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
--rw-r--r--   0        0        0   631630 2023-05-16 02:17:23.784502 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
--rw-r--r--   0        0        0   405369 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
--rw-r--r--   0        0        0     1590 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
--rw-r--r--   0        0        0   242997 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
--rw-r--r--   0        0        0     2135 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
--rw-r--r--   0        0        0     6135 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
--rw-r--r--   0        0        0     6170 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
--rw-r--r--   0        0        0     1523 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
--rw-r--r--   0        0        0     5506 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg
--rw-r--r--   0        0        0     2408 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg
--rw-r--r--   0        0        0     7874 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
--rw-r--r--   0        0        0      486 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/w.svg
--rw-r--r--   0        0        0     8734 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
--rw-r--r--   0        0        0     1610 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
--rw-r--r--   0        0        0     3010 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
--rw-r--r--   0        0        0     1694 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_anne/server.py
--rw-r--r--   0        0        0      359 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
--rw-r--r--   0        0        0     3252 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
--rw-r--r--   0        0        0      468 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_data/config.py
--rw-r--r--   0        0        0        0 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_data/database.py
--rw-r--r--   0        0        0     3232 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_data/players.py
--rw-r--r--   0        0        0     1295 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
--rw-r--r--   0        0        0     4097 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
--rw-r--r--   0        0        0     1906 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
--rw-r--r--   0        0        0     2688 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_file/remote.py
--rw-r--r--   0        0        0     4061 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
--rw-r--r--   0        0        0     4007 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_image/download.py
--rw-r--r--   0        0        0     1038 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
--rw-r--r--   0        0        0     9524 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_image/image.py
--rw-r--r--   0        0        0      936 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
--rw-r--r--   0        0        0     3799 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_image/steam.py
--rw-r--r--   0        0        0     1387 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
--rw-r--r--   0        0        0     4398 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_push/__init__.py
--rw-r--r--   0        0        0     3791 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
--rw-r--r--   0        0        0     1157 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_queries/api.py
--rw-r--r--   0        0        0     1191 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
--rw-r--r--   0        0        0    10837 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
--rw-r--r--   0        0        0     1615 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
--rw-r--r--   0        0        0        0 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_server/index.py
--rw-r--r--   0        0        0     1248 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
--rw-r--r--   0        0        0     1359 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
--rw-r--r--   0        0        0     4114 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_update/__init__.py
--rw-r--r--   0        0        0     1179 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py
--rw-r--r--   0        0        0     2024 2023-05-16 02:17:23.792502 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_update/restart.py
--rw-r--r--   0        0        0     1968 2023-05-16 02:17:23.792502 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_update/update.py
--rw-r--r--   0        0        0     8871 2023-05-16 02:17:23.792502 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_utils/command.py
--rw-r--r--   0        0        0     6070 2023-05-16 02:17:23.792502 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_utils/config.py
--rw-r--r--   0        0        0     1620 2023-05-16 02:17:23.792502 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_utils/message.py
--rw-r--r--   0        0        0      337 2023-05-16 02:17:23.792502 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_utils/rule.py
--rw-r--r--   0        0        0      992 2023-05-16 02:17:23.792502 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_utils/seach.py
--rw-r--r--   0        0        0     2133 2023-05-16 02:17:23.792502 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py
--rw-r--r--   0        0        0     8630 2023-05-16 02:17:23.792502 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_utils/utils.py
--rw-r--r--   0        0        0     8575 2023-05-16 02:17:23.792502 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_web/web.py
--rw-r--r--   0        0        0    14159 2023-05-16 02:17:23.792502 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
--rw-r--r--   0        0        0     1434 2023-05-16 02:17:23.792502 nonebot_plugin_l4d2_server-0.5.3.3/pyproject.toml
--rw-r--r--   0        0        0    13037 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.5.3.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-16 03:39:20.222840 nonebot_plugin_l4d2_server-0.5.4/LICENSE
+-rw-r--r--   0        0        0    11200 2023-05-16 03:39:20.222840 nonebot_plugin_l4d2_server-0.5.4/README.md
+-rw-r--r--   0        0        0    17493 2023-05-16 03:39:20.226840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/__init__.py
+-rw-r--r--   0        0        0   158357 2023-05-16 03:39:20.226840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
+-rw-r--r--   0        0        0   631630 2023-05-16 03:39:20.230840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
+-rw-r--r--   0        0        0   405369 2023-05-16 03:39:20.230840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
+-rw-r--r--   0        0        0     1590 2023-05-16 03:39:20.230840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
+-rw-r--r--   0        0        0   242997 2023-05-16 03:39:20.230840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
+-rw-r--r--   0        0        0     2135 2023-05-16 03:39:20.230840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
+-rw-r--r--   0        0        0     6135 2023-05-16 03:39:20.230840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
+-rw-r--r--   0        0        0     6170 2023-05-16 03:39:20.230840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
+-rw-r--r--   0        0        0     1523 2023-05-16 03:39:20.230840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
+-rw-r--r--   0        0        0     5506 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg
+-rw-r--r--   0        0        0     2408 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg
+-rw-r--r--   0        0        0     7874 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
+-rw-r--r--   0        0        0      486 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/w.svg
+-rw-r--r--   0        0        0     8734 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
+-rw-r--r--   0        0        0     1610 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
+-rw-r--r--   0        0        0     3010 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
+-rw-r--r--   0        0        0     1694 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_anne/server.py
+-rw-r--r--   0        0        0      359 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
+-rw-r--r--   0        0        0     3252 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
+-rw-r--r--   0        0        0      468 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_data/config.py
+-rw-r--r--   0        0        0        0 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_data/database.py
+-rw-r--r--   0        0        0     3232 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_data/players.py
+-rw-r--r--   0        0        0     1295 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
+-rw-r--r--   0        0        0     4097 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
+-rw-r--r--   0        0        0     1906 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
+-rw-r--r--   0        0        0     2688 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_file/remote.py
+-rw-r--r--   0        0        0     4061 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
+-rw-r--r--   0        0        0     4007 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_image/download.py
+-rw-r--r--   0        0        0     1038 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
+-rw-r--r--   0        0        0     9524 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_image/image.py
+-rw-r--r--   0        0        0      936 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
+-rw-r--r--   0        0        0     3799 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_image/steam.py
+-rw-r--r--   0        0        0     1387 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
+-rw-r--r--   0        0        0     5429 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_push/__init__.py
+-rw-r--r--   0        0        0     3791 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
+-rw-r--r--   0        0        0     1157 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_queries/api.py
+-rw-r--r--   0        0        0     1191 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
+-rw-r--r--   0        0        0    10837 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
+-rw-r--r--   0        0        0     1615 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_server/index.py
+-rw-r--r--   0        0        0     1248 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
+-rw-r--r--   0        0        0     1359 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
+-rw-r--r--   0        0        0     4114 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_update/__init__.py
+-rw-r--r--   0        0        0     1179 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py
+-rw-r--r--   0        0        0     2024 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_update/restart.py
+-rw-r--r--   0        0        0     1968 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_update/update.py
+-rw-r--r--   0        0        0     8862 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_utils/command.py
+-rw-r--r--   0        0        0     6198 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_utils/config.py
+-rw-r--r--   0        0        0     1620 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_utils/message.py
+-rw-r--r--   0        0        0      337 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_utils/rule.py
+-rw-r--r--   0        0        0      992 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_utils/seach.py
+-rw-r--r--   0        0        0     2133 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py
+-rw-r--r--   0        0        0     8907 2023-05-16 03:39:20.238841 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_utils/utils.py
+-rw-r--r--   0        0        0     8575 2023-05-16 03:39:20.238841 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_web/web.py
+-rw-r--r--   0        0        0    14159 2023-05-16 03:39:20.238841 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
+-rw-r--r--   0        0        0     1432 2023-05-16 03:39:20.238841 nonebot_plugin_l4d2_server-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0    13035 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.5.4/PKG-INFO
```

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/LICENSE` & `nonebot_plugin_l4d2_server-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/README.md` & `nonebot_plugin_l4d2_server-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 from nonebot.matcher import Matcher
 from nonebot.typing import T_State
 from nonebot.params import CommandArg,ArgPlainText,RegexGroup,Arg
 from nonebot import get_driver, require
 from nonebot.plugin import PluginMetadata
 
 
-from l4d2_utils.config import *
-from l4d2_utils.utils import *
-from l4d2_utils.command import *
+from .l4d2_utils.config import *
+from .l4d2_utils.utils import *
+from .l4d2_utils.command import *
 from .l4d2_image.steam import url_to_byte,url_to_byte_name
 
 from .l4d2_data import sq_L4D2
 from .l4d2_push import *
 from .l4d2_image.vtfs import img_to_vtf
 from .l4d2_queries.ohter import load_josn
 from .l4d2_queries.qqgroup import write_json
```

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_anne/server.py` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_anne/server.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_data/__init__.py` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_data/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_data/players.py` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_data/players.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_data/serverip.py` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_data/serverip.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_file/__init__.py` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_file/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_file/remote.py` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_file/remote.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_image/__init__.py` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_image/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_image/download.py` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_image/download.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_image/image.py` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_image/image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_image/steam.py` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_image/steam.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_push/__init__.py` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_push/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,125 +1,144 @@
 from pathlib import Path
+import re
 from typing import Dict,List,Union
 try:
-    import ujson
+    import ujson as json
 except:
     import json
 
+from nonebot.log import logger
 from nonebot import get_driver,on_command,get_bot
 from nonebot import require
 from nonebot.permission import SUPERUSER
-from nonebot.params import RawCommand
+from nonebot.params import CommandArg
 from nonebot.matcher import Matcher
-from nonebot.adapters.onebot.v11 import GroupMessageEvent,MessageSegment
+from nonebot.adapters.onebot.v11 import GroupMessageEvent,MessageSegment,Message
 from nonebot.adapters.onebot.v11.permission import (
     GROUP_ADMIN,
     GROUP_OWNER,
 )
 require("nonebot_plugin_apscheduler")
 from nonebot_plugin_apscheduler import scheduler
 
 from ..l4d2_utils.command import get_ip_to_mes
+from ..l4d2_utils.utils import extract_last_digit
+from ..l4d2_utils.config import l4_config
 
 driver = get_driver()
 sch_json = Path('data/L4D2/scheduler.json')
-add_rss = on_command('l4_rss',aliases={'求生添加定时'},priority= 30,permission= SUPERUSER| GROUP_ADMIN | GROUP_OWNER)
-del_rss = on_command('l4_rss',aliases={'求生删除定时'},priority= 30,permission= SUPERUSER| GROUP_ADMIN | GROUP_OWNER)
+if not sch_json.exists():
+    with sch_json.open('w') as f:
+        json.dump({}, f ,ensure_ascii=False)
+        
+add_rss = on_command('add_rss',aliases={'求生定时添加'},priority= 30,permission= SUPERUSER| GROUP_ADMIN | GROUP_OWNER)
+del_rss = on_command('del_rss',aliases={'求生定时删除'},priority= 30,permission= SUPERUSER| GROUP_ADMIN | GROUP_OWNER)
 
 @add_rss.handle()
-async def _(event:GroupMessageEvent , matcher:Matcher ,msg: str = RawCommand()):
+async def _(event:GroupMessageEvent , matcher:Matcher ,args: Message = CommandArg()):
     group_id = event.group_id
-    push_msg =  await get_ip_to_mes(msg)
-    if push_msg == "服务器无响应":
-        await matcher.finish(f'无响应的服务器，请检查')
+    msg = args.extract_plain_text()
+    command,message = await extract_last_digit(msg)
+    push_msg =  await get_ip_to_mes(msg= message,  command= command)
+    if push_msg in ["服务器无响应" ,None] :
+        await matcher.finish('无响应的服务器，请检查')
     else:
         return_msg = await add_or_update_data(group_id,msg)
+        print(return_msg)
+        if isinstance(push_msg , bytes):
+            await matcher.send(MessageSegment.image(push_msg))
+        else:
+            await matcher.send(push_msg)
         if return_msg == 'add':
-            await matcher.finish(f'已添加群定时任务【{msg}】10次')
-        elif return_msg == 'update':
-            await matcher.finish(f'已更新群定时任务【{msg}】10次')
+            await matcher.send(f'已添加群定时任务【{msg}】10次')
+        elif return_msg in ['update','change']:
+            await matcher.send(f'已更新群定时任务【{msg}】10次')
 
 @del_rss.handle()
-async def _(msg:str , event:GroupMessageEvent , matcher:Matcher):
+async def _(event:GroupMessageEvent , matcher:Matcher):
     group_id = event.group_id
-    await add_or_update_data(group_id,msg , ad_mode= 'del')
-    await matcher.finish(f'已删除群定时任务')
+    await add_or_update_data(group_id, '' , ad_mode= 'del')
+    await matcher.finish('已删除群定时任务')
 
 
 
-async def add_or_update_data(group_id, some_str :str = '',ad_mode :str = 'add'):
+async def add_or_update_data(group_id:int, some_str :str = '',ad_mode :str = 'add'):
     """添加或者删除定时任务
     mode == [new,update,del,change]
     """
+    group_id = str(group_id)
     sch_json = Path('data/L4D2/scheduler.json')
     if ad_mode == 'add':
         if sch_json.exists():
-            with sch_json.open() as f:
+            with sch_json.open(encoding='utf-8') as f:
                 scheduler_data = json.load(f)
             try:
                 times , old_msg = scheduler_data[group_id]
-                scheduler_data[group_id] = [10, some_str]
+                scheduler_data[group_id] = [l4_config.l4_push_times, some_str]
                 if old_msg == some_str:
                     mode = 'update' 
                 else:
                     mode = 'change'
             except:
-                scheduler_data[group_id] = [10, some_str]
+                scheduler_data[group_id] = [l4_config.l4_push_times, some_str]
+                mode = 'new'
 
         else:
-            scheduler_data = {group_id: [10, some_str]}
+            scheduler_data = {group_id: [l4_config.l4_push_times, some_str]}
             mode = 'new'
             
-        with sch_json.open('w') as f:
-            json.dump(scheduler_data, f)
+        with sch_json.open('w',encoding='utf-8') as f:
+            json.dump(scheduler_data, f ,ensure_ascii=False)
     
     else:
         if sch_json.exists():
             with sch_json.open() as f:
                 scheduler_data = json.load(f)
             try:
                 times , old_msg = scheduler_data[group_id]  
                 scheduler_data[group_id] = [0, old_msg]
             except:      
                 scheduler_data[group_id] = [0, some_str]
         else:
             scheduler_data = {group_id: [0, some_str]}
         mode = 'del'
             
-        with sch_json.open('w') as f:
-            json.dump(scheduler_data, f)   
+        with sch_json.open('w',encoding='utf-8') as f:
+            json.dump(scheduler_data, f ,ensure_ascii=False)  
             
     return mode
 
 async def rss_ip():
     sch_json = Path('data/L4D2/scheduler.json')
     
     if sch_json.exists():
         with sch_json.open(encoding='utf-8') as f:
-            scheduler_data:Dict[int,List[Union[int,str]]] = json.load(f)
+            scheduler_data:Dict[str,List[Union[int,str]]] = json.load(f)
             
             for key, value in scheduler_data.items():
-                recipient_id = key
+                recipient_id = int(key)
                 count = value[0]
                 msg = value[-1]
                 
                 if count > 0:
                     await send_message(recipient_id, msg)
                     count -= 1
                 
                 scheduler_data[key][0] = count  # 更新次数
                 
         with sch_json.open(mode='w',encoding='utf-8') as f:
-            json.dump(scheduler_data, f)
+            json.dump(scheduler_data, f ,ensure_ascii=False)
         
 async def send_message(recipient_id :int, msg :str):
     # 执行发送消息的操作，参数可以根据需要进行传递和使用
-    push_msg =  await get_ip_to_mes(msg)
-    if isinstance(msg ,bytes):
+    command,message = await extract_last_digit(msg)
+    push_msg =  await get_ip_to_mes(msg= message,  command= command)
+    if isinstance(push_msg ,bytes):
         await get_bot().send_group_msg(group_id=recipient_id, message=MessageSegment.image(push_msg))
-    elif msg and isinstance(msg ,str):
-        await get_bot().send_group_msg(group_id=recipient_id, message=msg)
-    
-    
+    elif msg and isinstance(push_msg ,str):
+        await get_bot().send_group_msg(group_id=recipient_id, message=push_msg)
     
-scheduler.add_job(rss_ip, "cron", minute=3, id="rss_ip")
+@driver.on_bot_connect
+async def _():    
+    logger.success('已成功启动求生定时推送')
+    scheduler.add_job(rss_ip, "interval", minutes=l4_config.l4_push_interval, id="rss_ip")
```

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_queries/api.py` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_queries/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_server/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_server/rcon.py` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_server/rcon.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_server/workshop.py` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_server/workshop.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_update/__init__.py` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_update/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_update/restart.py` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_update/restart.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_update/update.py` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_update/update.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_utils/command.py` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_utils/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,15 +181,15 @@
             matchers[get_ip.plugin_name] = []
         matchers[get_ip.plugin_name].append(get_ip)
         if start:
             command = command.replace(start,'')
         if command == 'anne':
             command = '云'
         msg:str = args.extract_plain_text()
-        push_msg = await get_ip_to_mes(msg, command, matcher)
+        push_msg = await get_ip_to_mes(msg, command)
         if isinstance(msg ,bytes):
             await matcher.finish(MessageSegment.image(push_msg))
         elif msg and isinstance(msg ,str):
             await matcher.finish(push_msg)
                 
 async def get_ip_to_mes(msg:str ,command: str = ''):   
     if not msg:
```

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_utils/config.py` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_utils/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,16 @@
                                 alias='后台管理token密钥')
     l4_master: List[str] = Field(['114514919'], alias='求生地图全局管理员qq')
     # l4_ip:bool = Field(False, alias='查询地图是否显示ip')
     l4_font: str = Field('simsun.ttc', alias='字体')
     l4_only:bool = Field(False, alias='下载地图是是否阻碍其他指令')
     l4_tag: List[str] = Field(['呆呆','橘'], alias='查服的名')
     l4_key: str = Field('q1145149191810', alias='key')
+    l4_push_interval: int = Field(3, alias='定时任务间隔')
+    l4_push_times: int = Field(10, alias='定时任务次数')
     group_config: Dict[int, L4d2GroupConfig] = Field({}, alias='分群配置')
 
     def update(self, **kwargs):
         for key, value in kwargs.items():
             if key in self.__fields__:
                 self.__setattr__(key, value)
```

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_utils/message.py` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_utils/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_utils/seach.py` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_utils/seach.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_utils/utils.py` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -290,8 +290,18 @@
     )
 
 def register_menu(*args, **kwargs):
     def decorator(f):
         register_menu_func(*args, **kwargs)
         return f
 
-    return decorator
+    return decorator
+
+
+async def extract_last_digit(msg: str) -> tuple[str, str]:
+    "分离str和数字"
+    for i in range(len(msg) - 1, -1, -1):
+        if msg[i].isdigit():
+            last_digit = msg[i]
+            new_msg = msg[:i]
+            return new_msg, last_digit
+    return msg, ''
```

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_web/web.py` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_web/web.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_web/webUI.py` & `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_web/webUI.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/pyproject.toml` & `nonebot_plugin_l4d2_server-0.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-l4d2-server"
-version = "0.5.3.3"
+version = "0.5.4"
 description = "L4D2 server related operations plugin for NoneBot2"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 repository = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 keywords = ["steam", "game", "l4d2", "nonebot2", "plugin"]
```

### Comparing `nonebot_plugin_l4d2_server-0.5.3.3/PKG-INFO` & `nonebot_plugin_l4d2_server-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-l4d2-server
-Version: 0.5.3.3
+Version: 0.5.4
 Summary: L4D2 server related operations plugin for NoneBot2
 Home-page: https://github.com/Agnes4m/nonebot_plugin_l4d2_server
 License: GPLv3
 Keywords: steam,game,l4d2,nonebot2,plugin
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.9,<4.0
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.5.3.3
-Summary: L4D2 server related operations plugin for NoneBot2 Home-page: https://
+Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.5.4 Summary:
+L4D2 server related operations plugin for NoneBot2 Home-page: https://
 github.com/Agnes4m/nonebot_plugin_l4d2_server License: GPLv3 Keywords:
 steam,game,l4d2,nonebot2,plugin Author: Agnes_Digital Author-email:
 Z735803792@163.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
```

