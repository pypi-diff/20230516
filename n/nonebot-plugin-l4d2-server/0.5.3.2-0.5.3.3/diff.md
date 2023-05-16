# Comparing `tmp/nonebot_plugin_l4d2_server-0.5.3.2.tar.gz` & `tmp/nonebot_plugin_l4d2_server-0.5.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_l4d2_server-0.5.3.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_l4d2_server-0.5.3.3.tar", max compression
```

## Comparing `nonebot_plugin_l4d2_server-0.5.3.2.tar` & `nonebot_plugin_l4d2_server-0.5.3.3.tar`

### file list

```diff
@@ -1,59 +1,60 @@
--rw-r--r--   0        0        0    35149 2023-05-13 14:22:26.242742 nonebot_plugin_l4d2_server-0.5.3.2/LICENSE
--rw-r--r--   0        0        0    11200 2023-05-13 14:22:26.242742 nonebot_plugin_l4d2_server-0.5.3.2/README.md
--rw-r--r--   0        0        0    17491 2023-05-13 14:22:26.242742 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/__init__.py
--rw-r--r--   0        0        0   158357 2023-05-13 14:22:26.242742 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
--rw-r--r--   0        0        0   631630 2023-05-13 14:22:26.246743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
--rw-r--r--   0        0        0   405369 2023-05-13 14:22:26.246743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
--rw-r--r--   0        0        0     1590 2023-05-13 14:22:26.246743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
--rw-r--r--   0        0        0   242997 2023-05-13 14:22:26.246743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
--rw-r--r--   0        0        0     2135 2023-05-13 14:22:26.246743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
--rw-r--r--   0        0        0     6135 2023-05-13 14:22:26.246743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
--rw-r--r--   0        0        0     6170 2023-05-13 14:22:26.246743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
--rw-r--r--   0        0        0     1523 2023-05-13 14:22:26.246743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
--rw-r--r--   0        0        0     5506 2023-05-13 14:22:26.250743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg
--rw-r--r--   0        0        0     2408 2023-05-13 14:22:26.250743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg
--rw-r--r--   0        0        0     7874 2023-05-13 14:22:26.250743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
--rw-r--r--   0        0        0      486 2023-05-13 14:22:26.250743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/w.svg
--rw-r--r--   0        0        0     8734 2023-05-13 14:22:26.250743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
--rw-r--r--   0        0        0     1610 2023-05-13 14:22:26.250743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
--rw-r--r--   0        0        0     3010 2023-05-13 14:22:26.250743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
--rw-r--r--   0        0        0     1694 2023-05-13 14:22:26.250743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_anne/server.py
--rw-r--r--   0        0        0      359 2023-05-13 14:22:26.250743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
--rw-r--r--   0        0        0     3252 2023-05-13 14:22:26.250743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
--rw-r--r--   0        0        0      468 2023-05-13 14:22:26.250743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_data/config.py
--rw-r--r--   0        0        0        0 2023-05-13 14:22:26.250743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_data/database.py
--rw-r--r--   0        0        0     3232 2023-05-13 14:22:26.250743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_data/players.py
--rw-r--r--   0        0        0     1295 2023-05-13 14:22:26.250743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
--rw-r--r--   0        0        0     4097 2023-05-13 14:22:26.250743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
--rw-r--r--   0        0        0     1906 2023-05-13 14:22:26.250743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
--rw-r--r--   0        0        0     2688 2023-05-13 14:22:26.250743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_file/remote.py
--rw-r--r--   0        0        0     4061 2023-05-13 14:22:26.250743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
--rw-r--r--   0        0        0     4007 2023-05-13 14:22:26.250743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_image/download.py
--rw-r--r--   0        0        0     1038 2023-05-13 14:22:26.250743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
--rw-r--r--   0        0        0     9524 2023-05-13 14:22:26.250743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_image/image.py
--rw-r--r--   0        0        0      936 2023-05-13 14:22:26.250743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
--rw-r--r--   0        0        0     3799 2023-05-13 14:22:26.250743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_image/steam.py
--rw-r--r--   0        0        0     1387 2023-05-13 14:22:26.250743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
--rw-r--r--   0        0        0     3791 2023-05-13 14:22:26.250743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
--rw-r--r--   0        0        0     1157 2023-05-13 14:22:26.250743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_queries/api.py
--rw-r--r--   0        0        0     1191 2023-05-13 14:22:26.250743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
--rw-r--r--   0        0        0    10837 2023-05-13 14:22:26.250743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
--rw-r--r--   0        0        0     1615 2023-05-13 14:22:26.250743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
--rw-r--r--   0        0        0        0 2023-05-13 14:22:26.250743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_server/index.py
--rw-r--r--   0        0        0     1248 2023-05-13 14:22:26.250743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
--rw-r--r--   0        0        0     1359 2023-05-13 14:22:26.250743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
--rw-r--r--   0        0        0     4114 2023-05-13 14:22:26.250743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_update/__init__.py
--rw-r--r--   0        0        0     1179 2023-05-13 14:22:26.250743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py
--rw-r--r--   0        0        0     2024 2023-05-13 14:22:26.250743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_update/restart.py
--rw-r--r--   0        0        0     1968 2023-05-13 14:22:26.250743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_update/update.py
--rw-r--r--   0        0        0     8693 2023-05-13 14:22:26.250743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_utils/command.py
--rw-r--r--   0        0        0     6070 2023-05-13 14:22:26.250743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_utils/config.py
--rw-r--r--   0        0        0     1620 2023-05-13 14:22:26.250743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_utils/message.py
--rw-r--r--   0        0        0      337 2023-05-13 14:22:26.250743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_utils/rule.py
--rw-r--r--   0        0        0      992 2023-05-13 14:22:26.250743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_utils/seach.py
--rw-r--r--   0        0        0     2133 2023-05-13 14:22:26.250743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py
--rw-r--r--   0        0        0     8630 2023-05-13 14:22:26.250743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_utils/utils.py
--rw-r--r--   0        0        0     8575 2023-05-13 14:22:26.250743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_web/web.py
--rw-r--r--   0        0        0    14159 2023-05-13 14:22:26.250743 nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
--rw-r--r--   0        0        0     1495 2023-05-13 14:22:26.250743 nonebot_plugin_l4d2_server-0.5.3.2/pyproject.toml
--rw-r--r--   0        0        0    13265 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.5.3.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-16 02:17:23.780502 nonebot_plugin_l4d2_server-0.5.3.3/LICENSE
+-rw-r--r--   0        0        0    11200 2023-05-16 02:17:23.780502 nonebot_plugin_l4d2_server-0.5.3.3/README.md
+-rw-r--r--   0        0        0    17490 2023-05-16 02:17:23.784502 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/__init__.py
+-rw-r--r--   0        0        0   158357 2023-05-16 02:17:23.784502 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
+-rw-r--r--   0        0        0   631630 2023-05-16 02:17:23.784502 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
+-rw-r--r--   0        0        0   405369 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
+-rw-r--r--   0        0        0     1590 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
+-rw-r--r--   0        0        0   242997 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
+-rw-r--r--   0        0        0     2135 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
+-rw-r--r--   0        0        0     6135 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
+-rw-r--r--   0        0        0     6170 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
+-rw-r--r--   0        0        0     1523 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
+-rw-r--r--   0        0        0     5506 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg
+-rw-r--r--   0        0        0     2408 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg
+-rw-r--r--   0        0        0     7874 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
+-rw-r--r--   0        0        0      486 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/w.svg
+-rw-r--r--   0        0        0     8734 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
+-rw-r--r--   0        0        0     1610 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
+-rw-r--r--   0        0        0     3010 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
+-rw-r--r--   0        0        0     1694 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_anne/server.py
+-rw-r--r--   0        0        0      359 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
+-rw-r--r--   0        0        0     3252 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
+-rw-r--r--   0        0        0      468 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_data/config.py
+-rw-r--r--   0        0        0        0 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_data/database.py
+-rw-r--r--   0        0        0     3232 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_data/players.py
+-rw-r--r--   0        0        0     1295 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
+-rw-r--r--   0        0        0     4097 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
+-rw-r--r--   0        0        0     1906 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
+-rw-r--r--   0        0        0     2688 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_file/remote.py
+-rw-r--r--   0        0        0     4061 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
+-rw-r--r--   0        0        0     4007 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_image/download.py
+-rw-r--r--   0        0        0     1038 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
+-rw-r--r--   0        0        0     9524 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_image/image.py
+-rw-r--r--   0        0        0      936 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
+-rw-r--r--   0        0        0     3799 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_image/steam.py
+-rw-r--r--   0        0        0     1387 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
+-rw-r--r--   0        0        0     4398 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_push/__init__.py
+-rw-r--r--   0        0        0     3791 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
+-rw-r--r--   0        0        0     1157 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_queries/api.py
+-rw-r--r--   0        0        0     1191 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
+-rw-r--r--   0        0        0    10837 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
+-rw-r--r--   0        0        0     1615 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_server/index.py
+-rw-r--r--   0        0        0     1248 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
+-rw-r--r--   0        0        0     1359 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
+-rw-r--r--   0        0        0     4114 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_update/__init__.py
+-rw-r--r--   0        0        0     1179 2023-05-16 02:17:23.788503 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py
+-rw-r--r--   0        0        0     2024 2023-05-16 02:17:23.792502 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_update/restart.py
+-rw-r--r--   0        0        0     1968 2023-05-16 02:17:23.792502 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_update/update.py
+-rw-r--r--   0        0        0     8871 2023-05-16 02:17:23.792502 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_utils/command.py
+-rw-r--r--   0        0        0     6070 2023-05-16 02:17:23.792502 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_utils/config.py
+-rw-r--r--   0        0        0     1620 2023-05-16 02:17:23.792502 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_utils/message.py
+-rw-r--r--   0        0        0      337 2023-05-16 02:17:23.792502 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_utils/rule.py
+-rw-r--r--   0        0        0      992 2023-05-16 02:17:23.792502 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_utils/seach.py
+-rw-r--r--   0        0        0     2133 2023-05-16 02:17:23.792502 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py
+-rw-r--r--   0        0        0     8630 2023-05-16 02:17:23.792502 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_utils/utils.py
+-rw-r--r--   0        0        0     8575 2023-05-16 02:17:23.792502 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_web/web.py
+-rw-r--r--   0        0        0    14159 2023-05-16 02:17:23.792502 nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
+-rw-r--r--   0        0        0     1434 2023-05-16 02:17:23.792502 nonebot_plugin_l4d2_server-0.5.3.3/pyproject.toml
+-rw-r--r--   0        0        0    13037 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.5.3.3/PKG-INFO
```

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/LICENSE` & `nonebot_plugin_l4d2_server-0.5.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/README.md` & `nonebot_plugin_l4d2_server-0.5.3.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,39 +17,39 @@
 from .l4d2_web import web,webUI
 
 from typing import Tuple,Union,List
 from time import sleep
 
 from nonebot.matcher import Matcher
 from nonebot.typing import T_State
-from nonebot.params import CommandArg,ArgPlainText,RegexGroup,Arg,RawCommand,CommandStart
+from nonebot.params import CommandArg,ArgPlainText,RegexGroup,Arg
 from nonebot import get_driver, require
 from nonebot.plugin import PluginMetadata
 
 
 from l4d2_utils.config import *
 from l4d2_utils.utils import *
 from l4d2_utils.command import *
 from .l4d2_image.steam import url_to_byte,url_to_byte_name
 
 from .l4d2_data import sq_L4D2
-
+from .l4d2_push import *
 from .l4d2_image.vtfs import img_to_vtf
 from .l4d2_queries.ohter import load_josn
 from .l4d2_queries.qqgroup import write_json
 from .l4d2_file import updown_l4d2_vpk,all_zip_to_one
 
-from l4d2_utils.txt_to_img import mode_txt_to_img
+from .l4d2_utils.txt_to_img import mode_txt_to_img
 # from .l4d2_server import RCONClient
 scheduler = require("nonebot_plugin_apscheduler").scheduler
 
 driver = get_driver()
 
 
-__version__ = "0.5.3.1"
+__version__ = "0.5.3"
 __plugin_meta__ = PluginMetadata(
     name="求生之路小助手",
     description='群内对有关求生之路的查询和操作',
     usage='求生服务器操作指令',
     extra={
         "version": __version__,
         "author": "Agnes4m <Z735803792@163.com>",
```

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_anne/server.py` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_anne/server.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_data/__init__.py` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_data/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_data/players.py` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_data/players.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_data/serverip.py` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_data/serverip.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_file/__init__.py` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_file/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_file/remote.py` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_file/remote.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_image/__init__.py` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_image/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_image/download.py` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_image/download.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_image/image.py` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_image/image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_image/steam.py` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_image/steam.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_queries/api.py` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_queries/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_server/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_server/rcon.py` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_server/rcon.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_server/workshop.py` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_server/workshop.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_update/__init__.py` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_update/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_update/restart.py` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_update/restart.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_update/update.py` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_update/update.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_utils/command.py` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_utils/command.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,17 +12,17 @@
     NoticeEvent,
     MessageEvent,
     Message,
     MessageSegment,
     GroupMessageEvent,
     )
 
-from .l4d2_anne.server import server_key,ANNE_IP
+from ..l4d2_anne.server import server_key,ANNE_IP
 from .config import *
-from .l4d2_queries.qqgroup import split_maohao
+from ..l4d2_queries.qqgroup import split_maohao
 # from .utils import qq_ip_queries_pic,json_server_to_tag_dict,get_anne_server_ip,get_tan_jian
 from .utils import *
 help_ = on_command('l4_help',aliases={'求生帮助'},priority=20,block=True)
 
 # 服务器
 # last_operation_time = nonebot.Config.parse_obj(nonebot.get_driver().config.dict()).SUPERUSERS
 
@@ -147,88 +147,100 @@
             ips = ALL_HOST['云']
             ip_anne_list = []
             for one_ip in ips:
                 host,port = split_maohao(one_ip['ip'])
                 ip_anne_list.append((one_ip['id'],host,port))
         except KeyError:
             pass
+        await get_read_ip(ip_anne_list)
+
+        
+    @tan_jian.handle()
+    async def _(matcher:Matcher,event:MessageEvent):
+        msg = await get_tan_jian(ip_anne_list,1)
+        await matcher.finish(msg)  
+        
+    @prison.handle()
+    async def _(matcher:Matcher,event:MessageEvent):
+        msg = await get_tan_jian(ip_anne_list,2)
+        await matcher.finish(msg)
+
+    @open_prison.handle()
+    async def _(matcher:Matcher,event:MessageEvent):
+
+        msg = await get_tan_jian(ip_anne_list,3)
+        await matcher.finish(msg)
+        
     
     
+async def get_read_ip(ip_anne_list):    
     get_ip = on_command('anne',aliases=server_key(),priority=80,block=True)
     @get_ip.handle()
     async def _(matcher:Matcher,start:str = CommandStart(),command: str = RawCommand(),args:Message = CommandArg()):
         global matchers
         if get_ip.plugin_name not in matchers:
             matchers[get_ip.plugin_name] = []
         matchers[get_ip.plugin_name].append(get_ip)
         if start:
             command = command.replace(start,'')
         if command == 'anne':
             command = '云'
         msg:str = args.extract_plain_text()
-        if not msg:
-            # 以图片输出全部当前
-            if command in gamemode_list:
-                this_ips = [d for l in ALL_HOST.values() for d in l if d.get('version') == command]
-                igr = True
-            else:
-                this_ips:list = ALL_HOST[command]
-                igr = False
-            if not this_ips:
-                matcher.finish('')
-            ip_list = []
-            for one_ip in this_ips:
-                host,port = split_maohao(one_ip['ip'])
-                ip_list.append((one_ip['id'],host,port))
-            img = await qq_ip_queries_pic(ip_list,igr)
-            if img:
-                await matcher.finish(MessageSegment.image(img)) 
-            else:
-                await matcher.finish("服务器无响应")
+        push_msg = await get_ip_to_mes(msg, command, matcher)
+        if isinstance(msg ,bytes):
+            await matcher.finish(MessageSegment.image(push_msg))
+        elif msg and isinstance(msg ,str):
+            await matcher.finish(push_msg)
+                
+async def get_ip_to_mes(msg:str ,command: str = ''):   
+    if not msg:
+        # 以图片输出全部当前
+        if command in gamemode_list:
+            this_ips = [d for l in ALL_HOST.values() for d in l if d.get('version') == command]
+            igr = True
+        else:
+            this_ips:list = ALL_HOST[command]
+            igr = False
+        if not this_ips:
+            return
+        ip_list = []
+        for one_ip in this_ips:
+            host,port = split_maohao(one_ip['ip'])
+            ip_list.append((one_ip['id'],host,port))
+        img = await qq_ip_queries_pic(ip_list,igr)
+        if img:
+            return img
         else:
-            if not msg[0].isdigit():
-                if any(mode in msg for mode in gamemode_list):
-                    pass
-                else:
-                    return
-            message = await json_server_to_tag_dict(command,msg)
-            if len(message) == 0:
-                # 关键词不匹配，忽略
+            return "服务器无响应"
+    else:
+        if not msg[0].isdigit():
+            if any(mode in msg for mode in gamemode_list):
+                pass
+            else:
                 return
-            ip = str(message['ip'])
-            logger.info(ip)
-            try:
-                msg= await get_anne_server_ip(ip)
-                await matcher.finish(msg)
-            except (OSError,asyncio.exceptions.TimeoutError):
-                await matcher.finish('服务器无响应')
+        message = await json_server_to_tag_dict(command,msg)
+        if len(message) == 0:
+            # 关键词不匹配，忽略
+            return
+        ip = str(message['ip'])
+        logger.info(ip)
+        try:
+            msg= await get_anne_server_ip(ip)
+            return  msg
+        except (OSError,asyncio.exceptions.TimeoutError):
+            return '服务器无响应'
     
            
-    @tan_jian.handle()
-    async def _(matcher:Matcher,event:MessageEvent):
-        msg = await get_tan_jian(ip_anne_list,1)
-        await matcher.finish(msg)  
-        
-    @prison.handle()
-    async def _(matcher:Matcher,event:MessageEvent):
-        msg = await get_tan_jian(ip_anne_list,2)
-        await matcher.finish(msg)
-
-    @open_prison.handle()
-    async def _(matcher:Matcher,event:MessageEvent):
 
-        msg = await get_tan_jian(ip_anne_list,3)
-        await matcher.finish(msg)
-        
     
     
 async def init():
     global matchers
     # print('启动辣')
-    from .l4d2_update import l4d_restart,l4d_update,get_update_log,driver
+    from ..l4d2_update import l4d_restart,l4d_update,get_update_log,driver
     await get_des_ip()
     
    
     
 @driver.on_bot_connect
 async def _():
     await init()
```

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_utils/config.py` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_utils/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_utils/message.py` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_utils/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_utils/seach.py` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_utils/seach.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_utils/utils.py` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_utils/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_web/web.py` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_web/web.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/nonebot_plugin_l4d2_server/l4d2_web/webUI.py` & `nonebot_plugin_l4d2_server-0.5.3.3/nonebot_plugin_l4d2_server/l4d2_web/webUI.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/pyproject.toml` & `nonebot_plugin_l4d2_server-0.5.3.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 [tool.poetry]
 name = "nonebot-plugin-l4d2-server"
-version = "0.5.3.2"
+version = "0.5.3.3"
 description = "L4D2 server related operations plugin for NoneBot2"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 repository = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 keywords = ["steam", "game", "l4d2", "nonebot2", "plugin"]
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Operating System :: OS Independent",
 ]
 include = [
     "LICENSE","README.md"
 ]
@@ -41,13 +40,12 @@
 rarfile = "^4.0"
 patool = "^1.12"
 python-a2s = "^1.3.0"
 amis-python = "^1.0.6"
 jieba = "^0.42.1"
 pandas = ">=1.5.2"
 python-jose = "^3.3.0"
-h11 = ">0.11.0"
 gitpython = ">=3.1.27"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_l4d2_server-0.5.3.2/PKG-INFO` & `nonebot_plugin_l4d2_server-0.5.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-l4d2-server
-Version: 0.5.3.2
+Version: 0.5.3.3
 Summary: L4D2 server related operations plugin for NoneBot2
 Home-page: https://github.com/Agnes4m/nonebot_plugin_l4d2_server
 License: GPLv3
 Keywords: steam,game,l4d2,nonebot2,plugin
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.9,<4.0
@@ -12,24 +12,19 @@
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
 Requires-Dist: amis-python (>=1.0.6,<2.0.0)
 Requires-Dist: asyncio (>=3.4.3)
 Requires-Dist: beautifulsoup4 (>=4.8.0)
 Requires-Dist: gitpython (>=3.1.27)
-Requires-Dist: h11 (>0.11.0)
 Requires-Dist: httpx (>=0.23.3,<0.24.0)
 Requires-Dist: jieba (>=0.42.1,<0.43.0)
 Requires-Dist: jinja2 (>=3.0.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.1.5)
 Requires-Dist: nonebot2 (>=2.0.0rc4,<3.0.0)
 Requires-Dist: nonebot_plugin_apscheduler (>=0.2.0,<0.3.0)
 Requires-Dist: nonebot_plugin_htmlrender (>=0.2.0.1,<0.3.0.0)
```

#### html2text {}

```diff
@@ -1,23 +1,20 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.5.3.2
+Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.5.3.3
 Summary: L4D2 server related operations plugin for NoneBot2 Home-page: https://
 github.com/Agnes4m/nonebot_plugin_l4d2_server License: GPLv3 Keywords:
 steam,game,l4d2,nonebot2,plugin Author: Agnes_Digital Author-email:
 Z735803792@163.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Requires-Dist: aiohttp
-(>=3.8.3,<4.0.0) Requires-Dist: amis-python (>=1.0.6,<2.0.0) Requires-Dist:
-asyncio (>=3.4.3) Requires-Dist: beautifulsoup4 (>=4.8.0) Requires-Dist:
-gitpython (>=3.1.27) Requires-Dist: h11 (>0.11.0) Requires-Dist: httpx
+Requires-Dist: aiohttp (>=3.8.3,<4.0.0) Requires-Dist: amis-python
+(>=1.0.6,<2.0.0) Requires-Dist: asyncio (>=3.4.3) Requires-Dist: beautifulsoup4
+(>=4.8.0) Requires-Dist: gitpython (>=3.1.27) Requires-Dist: httpx
 (>=0.23.3,<0.24.0) Requires-Dist: jieba (>=0.42.1,<0.43.0) Requires-Dist:
 jinja2 (>=3.0.0) Requires-Dist: nonebot-adapter-onebot (>=2.1.5) Requires-Dist:
 nonebot2 (>=2.0.0rc4,<3.0.0) Requires-Dist: nonebot_plugin_apscheduler
 (>=0.2.0,<0.3.0) Requires-Dist: nonebot_plugin_htmlrender (>=0.2.0.1,<0.3.0.0)
 Requires-Dist: nonebot_plugin_txt2img (>=0.3.0) Requires-Dist: pandas (>=1.5.2)
 Requires-Dist: patool (>=1.12,<2.0) Requires-Dist: pillow (>=9.3.0,<10.0.0)
 Requires-Dist: python-a2s (>=1.3.0,<2.0.0) Requires-Dist: python-jose
```

