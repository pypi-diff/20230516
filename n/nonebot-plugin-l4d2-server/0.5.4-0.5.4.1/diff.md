# Comparing `tmp/nonebot_plugin_l4d2_server-0.5.4.tar.gz` & `tmp/nonebot_plugin_l4d2_server-0.5.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_l4d2_server-0.5.4.tar", max compression
+gzip compressed data, was "nonebot_plugin_l4d2_server-0.5.4.1.tar", max compression
```

## Comparing `nonebot_plugin_l4d2_server-0.5.4.tar` & `nonebot_plugin_l4d2_server-0.5.4.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0    35149 2023-05-16 03:39:20.222840 nonebot_plugin_l4d2_server-0.5.4/LICENSE
--rw-r--r--   0        0        0    11200 2023-05-16 03:39:20.222840 nonebot_plugin_l4d2_server-0.5.4/README.md
--rw-r--r--   0        0        0    17493 2023-05-16 03:39:20.226840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/__init__.py
--rw-r--r--   0        0        0   158357 2023-05-16 03:39:20.226840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
--rw-r--r--   0        0        0   631630 2023-05-16 03:39:20.230840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
--rw-r--r--   0        0        0   405369 2023-05-16 03:39:20.230840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
--rw-r--r--   0        0        0     1590 2023-05-16 03:39:20.230840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
--rw-r--r--   0        0        0   242997 2023-05-16 03:39:20.230840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
--rw-r--r--   0        0        0     2135 2023-05-16 03:39:20.230840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
--rw-r--r--   0        0        0     6135 2023-05-16 03:39:20.230840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
--rw-r--r--   0        0        0     6170 2023-05-16 03:39:20.230840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
--rw-r--r--   0        0        0     1523 2023-05-16 03:39:20.230840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
--rw-r--r--   0        0        0     5506 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg
--rw-r--r--   0        0        0     2408 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg
--rw-r--r--   0        0        0     7874 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
--rw-r--r--   0        0        0      486 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/w.svg
--rw-r--r--   0        0        0     8734 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
--rw-r--r--   0        0        0     1610 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
--rw-r--r--   0        0        0     3010 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
--rw-r--r--   0        0        0     1694 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_anne/server.py
--rw-r--r--   0        0        0      359 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
--rw-r--r--   0        0        0     3252 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
--rw-r--r--   0        0        0      468 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_data/config.py
--rw-r--r--   0        0        0        0 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_data/database.py
--rw-r--r--   0        0        0     3232 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_data/players.py
--rw-r--r--   0        0        0     1295 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
--rw-r--r--   0        0        0     4097 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
--rw-r--r--   0        0        0     1906 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
--rw-r--r--   0        0        0     2688 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_file/remote.py
--rw-r--r--   0        0        0     4061 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
--rw-r--r--   0        0        0     4007 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_image/download.py
--rw-r--r--   0        0        0     1038 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
--rw-r--r--   0        0        0     9524 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_image/image.py
--rw-r--r--   0        0        0      936 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
--rw-r--r--   0        0        0     3799 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_image/steam.py
--rw-r--r--   0        0        0     1387 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
--rw-r--r--   0        0        0     5429 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_push/__init__.py
--rw-r--r--   0        0        0     3791 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
--rw-r--r--   0        0        0     1157 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_queries/api.py
--rw-r--r--   0        0        0     1191 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
--rw-r--r--   0        0        0    10837 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
--rw-r--r--   0        0        0     1615 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
--rw-r--r--   0        0        0        0 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_server/index.py
--rw-r--r--   0        0        0     1248 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
--rw-r--r--   0        0        0     1359 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
--rw-r--r--   0        0        0     4114 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_update/__init__.py
--rw-r--r--   0        0        0     1179 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py
--rw-r--r--   0        0        0     2024 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_update/restart.py
--rw-r--r--   0        0        0     1968 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_update/update.py
--rw-r--r--   0        0        0     8862 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_utils/command.py
--rw-r--r--   0        0        0     6198 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_utils/config.py
--rw-r--r--   0        0        0     1620 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_utils/message.py
--rw-r--r--   0        0        0      337 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_utils/rule.py
--rw-r--r--   0        0        0      992 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_utils/seach.py
--rw-r--r--   0        0        0     2133 2023-05-16 03:39:20.234840 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py
--rw-r--r--   0        0        0     8907 2023-05-16 03:39:20.238841 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_utils/utils.py
--rw-r--r--   0        0        0     8575 2023-05-16 03:39:20.238841 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_web/web.py
--rw-r--r--   0        0        0    14159 2023-05-16 03:39:20.238841 nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
--rw-r--r--   0        0        0     1432 2023-05-16 03:39:20.238841 nonebot_plugin_l4d2_server-0.5.4/pyproject.toml
--rw-r--r--   0        0        0    13035 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-16 05:04:13.955801 nonebot_plugin_l4d2_server-0.5.4.1/LICENSE
+-rw-r--r--   0        0        0    11415 2023-05-16 05:04:13.955801 nonebot_plugin_l4d2_server-0.5.4.1/README.md
+-rw-r--r--   0        0        0    17493 2023-05-16 05:04:13.955801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/__init__.py
+-rw-r--r--   0        0        0   158357 2023-05-16 05:04:13.959801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
+-rw-r--r--   0        0        0   631630 2023-05-16 05:04:13.959801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
+-rw-r--r--   0        0        0   405369 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
+-rw-r--r--   0        0        0     1590 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
+-rw-r--r--   0        0        0   242997 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
+-rw-r--r--   0        0        0     2135 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
+-rw-r--r--   0        0        0     6135 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
+-rw-r--r--   0        0        0     6170 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
+-rw-r--r--   0        0        0     1523 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
+-rw-r--r--   0        0        0     5506 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg
+-rw-r--r--   0        0        0     2408 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg
+-rw-r--r--   0        0        0     7874 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
+-rw-r--r--   0        0        0      486 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/w.svg
+-rw-r--r--   0        0        0     8734 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
+-rw-r--r--   0        0        0     1610 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
+-rw-r--r--   0        0        0     3010 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
+-rw-r--r--   0        0        0     1694 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_anne/server.py
+-rw-r--r--   0        0        0      359 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
+-rw-r--r--   0        0        0     3252 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
+-rw-r--r--   0        0        0      468 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_data/config.py
+-rw-r--r--   0        0        0        0 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_data/database.py
+-rw-r--r--   0        0        0     3232 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_data/players.py
+-rw-r--r--   0        0        0     1295 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
+-rw-r--r--   0        0        0     4097 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
+-rw-r--r--   0        0        0     1906 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
+-rw-r--r--   0        0        0     2688 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_file/remote.py
+-rw-r--r--   0        0        0     4148 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
+-rw-r--r--   0        0        0     4007 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_image/download.py
+-rw-r--r--   0        0        0     1038 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
+-rw-r--r--   0        0        0     9524 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_image/image.py
+-rw-r--r--   0        0        0      936 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
+-rw-r--r--   0        0        0     3799 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_image/steam.py
+-rw-r--r--   0        0        0     1387 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
+-rw-r--r--   0        0        0     5429 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_push/__init__.py
+-rw-r--r--   0        0        0     3791 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
+-rw-r--r--   0        0        0     1157 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_queries/api.py
+-rw-r--r--   0        0        0     1191 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
+-rw-r--r--   0        0        0    10855 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
+-rw-r--r--   0        0        0     1615 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_server/index.py
+-rw-r--r--   0        0        0     1248 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
+-rw-r--r--   0        0        0     1359 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
+-rw-r--r--   0        0        0     4114 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_update/__init__.py
+-rw-r--r--   0        0        0     1179 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py
+-rw-r--r--   0        0        0     2024 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_update/restart.py
+-rw-r--r--   0        0        0     1968 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_update/update.py
+-rw-r--r--   0        0        0     8892 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_utils/command.py
+-rw-r--r--   0        0        0     6212 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_utils/config.py
+-rw-r--r--   0        0        0     1620 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_utils/message.py
+-rw-r--r--   0        0        0      337 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_utils/rule.py
+-rw-r--r--   0        0        0      992 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_utils/seach.py
+-rw-r--r--   0        0        0     2133 2023-05-16 05:04:13.963801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py
+-rw-r--r--   0        0        0     8907 2023-05-16 05:04:13.967801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_utils/utils.py
+-rw-r--r--   0        0        0     8575 2023-05-16 05:04:13.967801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_web/web.py
+-rw-r--r--   0        0        0    14159 2023-05-16 05:04:13.967801 nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
+-rw-r--r--   0        0        0     1434 2023-05-16 05:04:13.967801 nonebot_plugin_l4d2_server-0.5.4.1/pyproject.toml
+-rw-r--r--   0        0        0    13252 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.5.4.1/PKG-INFO
```

### Comparing `nonebot_plugin_l4d2_server-0.5.4/LICENSE` & `nonebot_plugin_l4d2_server-0.5.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4/README.md` & `nonebot_plugin_l4d2_server-0.5.4.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
   <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">
   <br>
   <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>
 </div>
 
 <div align="center">
 
-# nonebot_plugin_l4d2_server
+# nonebot_plugin_l4d2_server 0.5
 
 _✨Nonebot & Left 4 Dead 2 server操作✨_
 <div align = "center">
         <a href="https://agnes4m.github.io/l4d2/" target="_blank">文档</a> &nbsp; · &nbsp;
         <a href="https://agnes4m.github.io/l4d2/reader/#%E5%8A%9F%E8%83%BD-%E6%8C%87%E4%BB%A4-%F0%9F%A4%94" target="_blank">指令列表</a> &nbsp; · &nbsp;
         <a href="https://agnes4m.github.io/l4d2/bug/">常见问题</a>
 </div><br>
@@ -54,22 +54,23 @@
 ## 数据结构
 
 bot所在文件夹下
 ```txt
 举例：
 └── data
     └── L4D2
-        ├── l4d2.yml
-        ├── l4d2.json
-        ├── sql
+        ├── l4d2.yml         # 配置文件
+        ├── l4d2.json        # ip文件
+        ├── scheduler.json   # 定时文件
+        ├── sql              # 数据库
         │   └── L4D2.db
-        ├── image
+        ├── image            # 头像缓存
         │   └── players
         │       └── ...
-        └── l4d2
+        └── l4d2             # 子ip文件
             ├── 关键词1.json
             ├── 关键词2.json
             └── ...
 ...
 ```
 
 新增一个json文件，格式如下,文件名与需要响应的指令一致
@@ -93,33 +94,36 @@
 ## 🌐 默认服务器
 
 由于不可抗力原因，暂时不使用在线的方式获取ip，有需求可以自行添加
 以下仅供参考本人使用的查询服务器
 
 | 指令 | 服务器 | op | 数量 |
 |:-----:|:----:|:----:|:----:|
-| 数码 | 爱丽数码想要涩涩 | 爱丽数码 | 5
-| 云 | anne电信服云服 | 东 | 19
+| 数码 | 爱丽数码想要涩涩 | 爱丽数码 | 4
+| 云 | anne电信服云服 | 东 | 21
 | 呆呆 | 呆呆的小窝 | 提莫大魔王 | 15
-| 橘 | 橘希实香的小窝 | 橘希实香 | 21
-| 竹 | 竹烨 | 竹烨oО柠檬茶 | 21
+| 橘 | 橘希实香的小窝 | 橘希实香 | 19
+| 竹 | 竹烨 | 竹烨oО柠檬茶 | 24
 | 音理 | 星空列车与白的旅行 | 音理 | 3
-| 尤 | 尤尤 | 晓音 | 3
+| 尤 | 尤尤 | 晓音 | 1
 | 鱼 | 飞鱼の小窝 | 飞鱼桑 | 3
 | 恋恋 | 恋氏集团雪糕制作研究中心 | 古明地恋 | 2
 | Air | Air | Air | 15
 | 3ks | 为人民服务 | DK | 14
 | 驴头 | 驴头服 | lvt | 4
 | 尸鬼 | 尸鬼狂潮 | ❀几❀ | 7
 
 ## 🔖 更新日志
 
 <details>
 <summary>展开/收起</summary>
 
+### 0.5.4--2022.5.16
+
+- 添加定时任务
 
 ### 0.5.3--2022.5.07
 
 - 新增`l4更新`和`l4重启`
 - 注释无效项（三方图查询）
 - 可以通过git clone 直接加载插件
```

#### html2text {}

```diff
@@ -1,44 +1,46 @@
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
-   # nonebot_plugin_l4d2_server _â¨Nonebot & Left 4 Dead 2 serveræä½â¨_
+ # nonebot_plugin_l4d2_server 0.5 _â¨Nonebot & Left 4 Dead 2 serveræä½â¨_
                 ææ¡£   Â·   æä»¤åè¡¨   Â·   å¸¸è§é®é¢
 
 [GitHub_stars] [GitHub_issues] [QQ_Chat_Group] [pypi] [pypi_download] [python]
                                    [NoneBot]
 ## é¡¶ç½®å¬å
 0.5.0ç ´åå¼æ´æ°ï¼ä¸åä½¿ç¨envéç½®ï¼éç¨webæ§å¶å°ç®¡ç
 åæ¶ä¸åæ¯æè¿ç¨æ¥è¯¢ï¼æ¹ä¸ºåªåè®¸æ¬å°æ¥è¯¢
 ææ¡£ææ¶æ²¡æ¶é´æ´æ°ozr ## ä¸»è¦åè½ - æ±çæå¡å¨-
 æ¬å°å¤è·¯å¾æä½ï¼ä¼ å°å¾ï¼ -
 æ¹éæ¥è¯¢æå®ipæå¡å¨ç¶æåç©å®¶ -
 åæå·¥åä¸è½½åå·æ¼å¶ä½ - webæ§å¶å° - [æ±ççµä¿¡æanne](https:
 //github.com/fantasylidong/CompetitiveWithAnne)[æ¥è¯¢~](https://sb.trygek.com/
 l4d_stats/ranking/index.php) ## æ°æ®ç»æ botæå¨æä»¶å¤¹ä¸ ```txt
-ä¸¾ä¾ï¼ âââ data âââ L4D2 âââ l4d2.yml âââ l4d2.json
-âââ sql â âââ L4D2.db âââ image â âââ players â
-âââ ... âââ l4d2 âââ å³é®è¯1.json âââ
-å³é®è¯2.json âââ ... ... ```
+ä¸¾ä¾ï¼ âââ data âââ L4D2 âââ l4d2.yml # éç½®æä»¶
+âââ l4d2.json # ipæä»¶ âââ scheduler.json # å®æ¶æä»¶
+âââ sql # æ°æ®åº â âââ L4D2.db âââ image # å¤´åç¼å­
+â âââ players â âââ ... âââ l4d2 # å­ipæä»¶ âââ
+å³é®è¯1.json âââ å³é®è¯2.json âââ ... ... ```
 æ°å¢ä¸ä¸ªjsonæä»¶ï¼æ ¼å¼å¦ä¸,æä»¶åä¸éè¦ååºçæä»¤ä¸è´
 `l4d2.json`å`å³é®è¯1.json`é½å¯ä»¥å è½½ { "åå": [ { "id": 1,
 "version": "æå½¹", "ip": "43.248.188.17:27031" }, { "id": 2, "version":
 "æå½¹", "ip": "43.248.188.17:27032" } ] } ## ð é»è®¤æå¡å¨
 ç±äºä¸å¯æååå ï¼ææ¶ä¸ä½¿ç¨å¨çº¿çæ¹å¼è·åipï¼æéæ±å¯ä»¥èªè¡æ·»å 
 ä»¥ä¸ä»ä¾åèæ¬äººä½¿ç¨çæ¥è¯¢æå¡å¨ | æä»¤ | æå¡å¨ | op |
 æ°é | |:-----:|:----:|:----:|:----:| | æ°ç  | ç±ä¸½æ°ç æ³è¦æ¶©æ¶© |
-ç±ä¸½æ°ç  | 5 | äº | anneçµä¿¡æäºæ | ä¸ | 19 | åå |
+ç±ä¸½æ°ç  | 4 | äº | anneçµä¿¡æäºæ | ä¸ | 21 | åå |
 ååçå°çª | æè«å¤§é­ç | 15 | æ© | æ©å¸å®é¦çå°çª |
-æ©å¸å®é¦ | 21 | ç«¹ | ç«¹ç¨ | ç«¹ç¨oÐæ æª¬è¶ | 21 | é³ç |
-æç©ºåè½¦ä¸ç½çæè¡ | é³ç | 3 | å°¤ | å°¤å°¤ | æé³ | 3 | é±¼ |
+æ©å¸å®é¦ | 19 | ç«¹ | ç«¹ç¨ | ç«¹ç¨oÐæ æª¬è¶ | 24 | é³ç |
+æç©ºåè½¦ä¸ç½çæè¡ | é³ç | 3 | å°¤ | å°¤å°¤ | æé³ | 1 | é±¼ |
 é£é±¼ã®å°çª | é£é±¼æ¡ | 3 | ææ | ææ°éå¢éªç³å¶ä½ç ç©¶ä¸­å¿
 | å¤æå°æ | 2 | Air | Air | Air | 15 | 3ks | ä¸ºäººæ°æå¡ | DK | 14 |
 é©´å¤´ | é©´å¤´æ | lvt | 4 | å°¸é¬¼ | å°¸é¬¼çæ½® | âå â | 7 ## ð
-æ´æ°æ¥å¿  å±å¼/æ¶èµ· ### 0.5.3--2022.5.07 -
-æ°å¢`l4æ´æ°`å`l4éå¯` - æ³¨éæ æé¡¹ï¼ä¸æ¹å¾æ¥è¯¢ï¼ -
-å¯ä»¥éè¿git clone ç´æ¥å è½½æä»¶ ### 0.5.2--2022.5.01 -
+æ´æ°æ¥å¿  å±å¼/æ¶èµ· ### 0.5.4--2022.5.16 - æ·»å å®æ¶ä»»å¡ ###
+0.5.3--2022.5.07 - æ°å¢`l4æ´æ°`å`l4éå¯` -
+æ³¨éæ æé¡¹ï¼ä¸æ¹å¾æ¥è¯¢ï¼ - å¯ä»¥éè¿git clone ç´æ¥å è½½æä»¶
+### 0.5.2--2022.5.01 -
 è§£å³äºmainådevåæ¯çä¸ä¸ªä¸¥ébugï¼ä¹è®¸æ²¡è§£å³ -
 æ¬å°åï¼æ´å¥½çæ·»å ,å é¤è¿ç¨åæ¯ -
 æå¡å¨å¿äºå¤ä»½ï¼å°½åæ¢æäºæ°æ®äº ### 0.5.0--2022.4.28 -
 éæconfigï¼å¹¶å¼ç¨envè®¾ç½® - ä½¿ç¨ç½é¡µæ§å¶å°æ¥æ§å¶éç½® -
 æ°å¢äºå¾å¤ä¸ä¼æ¥éçbug ### 0.4.9--2022.4 -
 ä¿®å¤h11çæ¬éè¯¯çbug -
 éåäºconfigï¼ä¸ä¸ªçæ¬æ­£å¼ä½¿ç¨yamlæ¿ä»£envè®¾ç½® -
```

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_anne/server.py` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_anne/server.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_data/__init__.py` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_data/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_data/players.py` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_data/players.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_data/serverip.py` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_data/serverip.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_file/__init__.py` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_file/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_file/remote.py` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_file/remote.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_image/__init__.py` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_image/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     template = env.get_template('anne.html')
     html = await template.render_async(data=msg_dict)
     pic = await html_to_pic(
                 html,
                 wait=0,
                 viewport={"width": 1100, "height": 800},
                 template_path=f"file://{template_path.absolute()}",)
-    print(type(pic))
     return pic
 
 
 async def dict_to_html(usr_id,DETAIL_MAP:dict,soup:BeautifulSoup):
     """输入qq、字典，获取新的msg替换html"""
     DETAIL_right = {}
     DETAIL_right['name'] = DETAIL_MAP['Steam 名字:']
@@ -80,15 +79,18 @@
             for player_info in sorted_players:
                 player_str = f"{player_info['name']} | {player_info['Duration']}"
                 players_list.append(player_str)
             while len(players_list) < 4:
                 players_list.append("")
             server_info['Players'] = players_list
     pic = await get_help_img(msg_list)
-
+    if pic:
+        logger.success('正在输出图片')
+    else:
+        logger.warning('我的图图呢')
     return pic
 
 
 async def get_help_img(plugins: List[dict]) -> Optional[bytes]:
     try:
         if l4_config.l4_style == 'black':
             template = env.get_template("help_dack.html")
```

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_image/download.py` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_image/download.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_image/image.py` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_image/image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_image/steam.py` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_image/steam.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_push/__init__.py` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_push/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_queries/api.py` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_queries/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,14 +77,15 @@
     else:
         result = {}
     return result
 
 
 async def qq_ip_queries_pic(msg: list,igr = False):
     result = await qq_ip_querie(msg,igr)
+    print(result)
     if 'msg_list' in result:
         pic = await server_ip_pic(result['msg_list'])
     else:
         pic = None
     return pic
```

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_server/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_server/rcon.py` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_server/rcon.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_server/workshop.py` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_server/workshop.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_update/__init__.py` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_update/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_update/restart.py` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_update/restart.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_update/update.py` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_update/update.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_utils/command.py` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_utils/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,22 +182,23 @@
         matchers[get_ip.plugin_name].append(get_ip)
         if start:
             command = command.replace(start,'')
         if command == 'anne':
             command = '云'
         msg:str = args.extract_plain_text()
         push_msg = await get_ip_to_mes(msg, command)
-        if isinstance(msg ,bytes):
+        if isinstance(push_msg ,bytes):
             await matcher.finish(MessageSegment.image(push_msg))
-        elif msg and isinstance(msg ,str):
+        elif msg and isinstance(push_msg ,str):
             await matcher.finish(push_msg)
                 
 async def get_ip_to_mes(msg:str ,command: str = ''):   
     if not msg:
         # 以图片输出全部当前
+        igr = False
         if command in gamemode_list:
             this_ips = [d for l in ALL_HOST.values() for d in l if d.get('version') == command]
             igr = True
         else:
             this_ips:list = ALL_HOST[command]
             igr = False
         if not this_ips:
```

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_utils/config.py` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_utils/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -145,24 +145,24 @@
 地图路径
 '''
 vpk_path = "left4dead2/addons"
 
 
 PLAYERSDATA = Path() / "data/L4D2/image/players"
 """用户数据路径"""
-TEXT_PATH = Path(__file__).parent / 'data/L4D2/image'
+TEXT_PATH = Path(__file__).parent.parent / 'data/L4D2/image'
 """图片存储路径"""
 TEXT_XPATH = Path() / 'data/L4D2/image'
 """内置图片路径"""
 
 
 
 PLAYERSDATA = Path() / "data/L4D2/sql"
 """数据库路径"""
-DATASQLITE = Path().parent / "data/L4D2/sql/L4D2.db"
+DATASQLITE = Path().parent.parent / "data/L4D2/sql/L4D2.db"
 """数据库！"""  
 
 table_data = ["L4d2_players","L4D2_server"]
 """数据库表"""
 L4d2_players_tag = ['qq', 'nickname', 'steamid']
 """数据库表1"""
 L4d2_server_tag = ['id','qqgroup', 'host', 'port', 'rcon']
```

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_utils/message.py` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_utils/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_utils/seach.py` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_utils/seach.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_utils/utils.py` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_utils/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_web/web.py` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_web/web.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4/nonebot_plugin_l4d2_server/l4d2_web/webUI.py` & `nonebot_plugin_l4d2_server-0.5.4.1/nonebot_plugin_l4d2_server/l4d2_web/webUI.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.4/pyproject.toml` & `nonebot_plugin_l4d2_server-0.5.4.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-l4d2-server"
-version = "0.5.4"
+version = "0.5.4.1"
 description = "L4D2 server related operations plugin for NoneBot2"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 repository = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 keywords = ["steam", "game", "l4d2", "nonebot2", "plugin"]
```

### Comparing `nonebot_plugin_l4d2_server-0.5.4/PKG-INFO` & `nonebot_plugin_l4d2_server-0.5.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-l4d2-server
-Version: 0.5.4
+Version: 0.5.4.1
 Summary: L4D2 server related operations plugin for NoneBot2
 Home-page: https://github.com/Agnes4m/nonebot_plugin_l4d2_server
 License: GPLv3
 Keywords: steam,game,l4d2,nonebot2,plugin
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.9,<4.0
@@ -46,15 +46,15 @@
   <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">
   <br>
   <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>
 </div>
 
 <div align="center">
 
-# nonebot_plugin_l4d2_server
+# nonebot_plugin_l4d2_server 0.5
 
 _✨Nonebot & Left 4 Dead 2 server操作✨_
 <div align = "center">
         <a href="https://agnes4m.github.io/l4d2/" target="_blank">文档</a> &nbsp; · &nbsp;
         <a href="https://agnes4m.github.io/l4d2/reader/#%E5%8A%9F%E8%83%BD-%E6%8C%87%E4%BB%A4-%F0%9F%A4%94" target="_blank">指令列表</a> &nbsp; · &nbsp;
         <a href="https://agnes4m.github.io/l4d2/bug/">常见问题</a>
 </div><br>
@@ -98,22 +98,23 @@
 ## 数据结构
 
 bot所在文件夹下
 ```txt
 举例：
 └── data
     └── L4D2
-        ├── l4d2.yml
-        ├── l4d2.json
-        ├── sql
+        ├── l4d2.yml         # 配置文件
+        ├── l4d2.json        # ip文件
+        ├── scheduler.json   # 定时文件
+        ├── sql              # 数据库
         │   └── L4D2.db
-        ├── image
+        ├── image            # 头像缓存
         │   └── players
         │       └── ...
-        └── l4d2
+        └── l4d2             # 子ip文件
             ├── 关键词1.json
             ├── 关键词2.json
             └── ...
 ...
 ```
 
 新增一个json文件，格式如下,文件名与需要响应的指令一致
@@ -137,33 +138,36 @@
 ## 🌐 默认服务器
 
 由于不可抗力原因，暂时不使用在线的方式获取ip，有需求可以自行添加
 以下仅供参考本人使用的查询服务器
 
 | 指令 | 服务器 | op | 数量 |
 |:-----:|:----:|:----:|:----:|
-| 数码 | 爱丽数码想要涩涩 | 爱丽数码 | 5
-| 云 | anne电信服云服 | 东 | 19
+| 数码 | 爱丽数码想要涩涩 | 爱丽数码 | 4
+| 云 | anne电信服云服 | 东 | 21
 | 呆呆 | 呆呆的小窝 | 提莫大魔王 | 15
-| 橘 | 橘希实香的小窝 | 橘希实香 | 21
-| 竹 | 竹烨 | 竹烨oО柠檬茶 | 21
+| 橘 | 橘希实香的小窝 | 橘希实香 | 19
+| 竹 | 竹烨 | 竹烨oО柠檬茶 | 24
 | 音理 | 星空列车与白的旅行 | 音理 | 3
-| 尤 | 尤尤 | 晓音 | 3
+| 尤 | 尤尤 | 晓音 | 1
 | 鱼 | 飞鱼の小窝 | 飞鱼桑 | 3
 | 恋恋 | 恋氏集团雪糕制作研究中心 | 古明地恋 | 2
 | Air | Air | Air | 15
 | 3ks | 为人民服务 | DK | 14
 | 驴头 | 驴头服 | lvt | 4
 | 尸鬼 | 尸鬼狂潮 | ❀几❀ | 7
 
 ## 🔖 更新日志
 
 <details>
 <summary>展开/收起</summary>
 
+### 0.5.4--2022.5.16
+
+- 添加定时任务
 
 ### 0.5.3--2022.5.07
 
 - 新增`l4更新`和`l4重启`
 - 注释无效项（三方图查询）
 - 可以通过git clone 直接加载插件
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.5.4 Summary:
-L4D2 server related operations plugin for NoneBot2 Home-page: https://
+Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.5.4.1
+Summary: L4D2 server related operations plugin for NoneBot2 Home-page: https://
 github.com/Agnes4m/nonebot_plugin_l4d2_server License: GPLv3 Keywords:
 steam,game,l4d2,nonebot2,plugin Author: Agnes_Digital Author-email:
 Z735803792@163.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
@@ -21,49 +21,51 @@
 (>=3.3.0,<4.0.0) Requires-Dist: pyunpack (>=0.3.0,<0.4.0) Requires-Dist:
 rarfile (>=4.0,<5.0) Requires-Dist: rcon (>=2.1.0,<3.0.0) Requires-Dist:
 ruamel.yaml (>=0.17.21,<0.18.0) Requires-Dist: srctools (>=2.3.9,<3.0.0)
 Project-URL: Repository, https://github.com/Agnes4m/nonebot_plugin_l4d2_server
 Description-Content-Type: text/markdown
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
-   # nonebot_plugin_l4d2_server _â¨Nonebot & Left 4 Dead 2 serveræä½â¨_
+ # nonebot_plugin_l4d2_server 0.5 _â¨Nonebot & Left 4 Dead 2 serveræä½â¨_
                 ææ¡£   Â·   æä»¤åè¡¨   Â·   å¸¸è§é®é¢
 
 [GitHub_stars] [GitHub_issues] [QQ_Chat_Group] [pypi] [pypi_download] [python]
                                    [NoneBot]
 ## é¡¶ç½®å¬å
 0.5.0ç ´åå¼æ´æ°ï¼ä¸åä½¿ç¨envéç½®ï¼éç¨webæ§å¶å°ç®¡ç
 åæ¶ä¸åæ¯æè¿ç¨æ¥è¯¢ï¼æ¹ä¸ºåªåè®¸æ¬å°æ¥è¯¢
 ææ¡£ææ¶æ²¡æ¶é´æ´æ°ozr ## ä¸»è¦åè½ - æ±çæå¡å¨-
 æ¬å°å¤è·¯å¾æä½ï¼ä¼ å°å¾ï¼ -
 æ¹éæ¥è¯¢æå®ipæå¡å¨ç¶æåç©å®¶ -
 åæå·¥åä¸è½½åå·æ¼å¶ä½ - webæ§å¶å° - [æ±ççµä¿¡æanne](https:
 //github.com/fantasylidong/CompetitiveWithAnne)[æ¥è¯¢~](https://sb.trygek.com/
 l4d_stats/ranking/index.php) ## æ°æ®ç»æ botæå¨æä»¶å¤¹ä¸ ```txt
-ä¸¾ä¾ï¼ âââ data âââ L4D2 âââ l4d2.yml âââ l4d2.json
-âââ sql â âââ L4D2.db âââ image â âââ players â
-âââ ... âââ l4d2 âââ å³é®è¯1.json âââ
-å³é®è¯2.json âââ ... ... ```
+ä¸¾ä¾ï¼ âââ data âââ L4D2 âââ l4d2.yml # éç½®æä»¶
+âââ l4d2.json # ipæä»¶ âââ scheduler.json # å®æ¶æä»¶
+âââ sql # æ°æ®åº â âââ L4D2.db âââ image # å¤´åç¼å­
+â âââ players â âââ ... âââ l4d2 # å­ipæä»¶ âââ
+å³é®è¯1.json âââ å³é®è¯2.json âââ ... ... ```
 æ°å¢ä¸ä¸ªjsonæä»¶ï¼æ ¼å¼å¦ä¸,æä»¶åä¸éè¦ååºçæä»¤ä¸è´
 `l4d2.json`å`å³é®è¯1.json`é½å¯ä»¥å è½½ { "åå": [ { "id": 1,
 "version": "æå½¹", "ip": "43.248.188.17:27031" }, { "id": 2, "version":
 "æå½¹", "ip": "43.248.188.17:27032" } ] } ## ð é»è®¤æå¡å¨
 ç±äºä¸å¯æååå ï¼ææ¶ä¸ä½¿ç¨å¨çº¿çæ¹å¼è·åipï¼æéæ±å¯ä»¥èªè¡æ·»å 
 ä»¥ä¸ä»ä¾åèæ¬äººä½¿ç¨çæ¥è¯¢æå¡å¨ | æä»¤ | æå¡å¨ | op |
 æ°é | |:-----:|:----:|:----:|:----:| | æ°ç  | ç±ä¸½æ°ç æ³è¦æ¶©æ¶© |
-ç±ä¸½æ°ç  | 5 | äº | anneçµä¿¡æäºæ | ä¸ | 19 | åå |
+ç±ä¸½æ°ç  | 4 | äº | anneçµä¿¡æäºæ | ä¸ | 21 | åå |
 ååçå°çª | æè«å¤§é­ç | 15 | æ© | æ©å¸å®é¦çå°çª |
-æ©å¸å®é¦ | 21 | ç«¹ | ç«¹ç¨ | ç«¹ç¨oÐæ æª¬è¶ | 21 | é³ç |
-æç©ºåè½¦ä¸ç½çæè¡ | é³ç | 3 | å°¤ | å°¤å°¤ | æé³ | 3 | é±¼ |
+æ©å¸å®é¦ | 19 | ç«¹ | ç«¹ç¨ | ç«¹ç¨oÐæ æª¬è¶ | 24 | é³ç |
+æç©ºåè½¦ä¸ç½çæè¡ | é³ç | 3 | å°¤ | å°¤å°¤ | æé³ | 1 | é±¼ |
 é£é±¼ã®å°çª | é£é±¼æ¡ | 3 | ææ | ææ°éå¢éªç³å¶ä½ç ç©¶ä¸­å¿
 | å¤æå°æ | 2 | Air | Air | Air | 15 | 3ks | ä¸ºäººæ°æå¡ | DK | 14 |
 é©´å¤´ | é©´å¤´æ | lvt | 4 | å°¸é¬¼ | å°¸é¬¼çæ½® | âå â | 7 ## ð
-æ´æ°æ¥å¿  å±å¼/æ¶èµ· ### 0.5.3--2022.5.07 -
-æ°å¢`l4æ´æ°`å`l4éå¯` - æ³¨éæ æé¡¹ï¼ä¸æ¹å¾æ¥è¯¢ï¼ -
-å¯ä»¥éè¿git clone ç´æ¥å è½½æä»¶ ### 0.5.2--2022.5.01 -
+æ´æ°æ¥å¿  å±å¼/æ¶èµ· ### 0.5.4--2022.5.16 - æ·»å å®æ¶ä»»å¡ ###
+0.5.3--2022.5.07 - æ°å¢`l4æ´æ°`å`l4éå¯` -
+æ³¨éæ æé¡¹ï¼ä¸æ¹å¾æ¥è¯¢ï¼ - å¯ä»¥éè¿git clone ç´æ¥å è½½æä»¶
+### 0.5.2--2022.5.01 -
 è§£å³äºmainådevåæ¯çä¸ä¸ªä¸¥ébugï¼ä¹è®¸æ²¡è§£å³ -
 æ¬å°åï¼æ´å¥½çæ·»å ,å é¤è¿ç¨åæ¯ -
 æå¡å¨å¿äºå¤ä»½ï¼å°½åæ¢æäºæ°æ®äº ### 0.5.0--2022.4.28 -
 éæconfigï¼å¹¶å¼ç¨envè®¾ç½® - ä½¿ç¨ç½é¡µæ§å¶å°æ¥æ§å¶éç½® -
 æ°å¢äºå¾å¤ä¸ä¼æ¥éçbug ### 0.4.9--2022.4 -
 ä¿®å¤h11çæ¬éè¯¯çbug -
 éåäºconfigï¼ä¸ä¸ªçæ¬æ­£å¼ä½¿ç¨yamlæ¿ä»£envè®¾ç½® -
```

