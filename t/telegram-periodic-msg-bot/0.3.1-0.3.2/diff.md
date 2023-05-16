# Comparing `tmp/telegram_periodic_msg_bot-0.3.1.tar.gz` & `tmp/telegram_periodic_msg_bot-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegram_periodic_msg_bot-0.3.1.tar", last modified: Wed Sep 28 08:48:43 2022, max compression
+gzip compressed data, was "telegram_periodic_msg_bot-0.3.2.tar", last modified: Tue May 16 21:52:12 2023, max compression
```

## Comparing `telegram_periodic_msg_bot-0.3.1.tar` & `telegram_periodic_msg_bot-0.3.2.tar`

### file list

```diff
@@ -1,63 +1,68 @@
-drwxrwxrwx   0        0        0        0 2022-09-28 08:48:43.581946 telegram_periodic_msg_bot-0.3.1/
--rw-rw-rw-   0        0        0     1085 2021-06-09 13:22:24.000000 telegram_periodic_msg_bot-0.3.1/LICENSE
--rw-rw-rw-   0        0        0       26 2021-10-20 11:44:31.000000 telegram_periodic_msg_bot-0.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0     9390 2022-09-28 08:48:43.581946 telegram_periodic_msg_bot-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     8381 2021-12-09 21:54:39.000000 telegram_periodic_msg_bot-0.3.1/README.md
--rw-rw-rw-   0        0        0       45 2021-10-20 12:15:41.000000 telegram_periodic_msg_bot-0.3.1/requirements.txt
--rw-rw-rw-   0        0        0      111 2022-09-28 08:48:43.584945 telegram_periodic_msg_bot-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     2217 2021-10-20 12:17:11.000000 telegram_periodic_msg_bot-0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-09-28 08:48:43.463737 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/
--rw-rw-rw-   0        0        0      148 2021-09-28 14:11:55.000000 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/__init__.py
--rw-rw-rw-   0        0        0       28 2022-09-28 08:38:25.000000 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/_version.py
-drwxrwxrwx   0        0        0        0 2022-09-28 08:48:43.494737 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/bot/
--rw-rw-rw-   0        0        0        0 2021-11-30 15:43:37.000000 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/bot/__init__.py
--rw-rw-rw-   0        0        0     5115 2022-09-28 08:21:34.000000 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/bot/bot_base.py
--rw-rw-rw-   0        0        0     1989 2022-09-28 08:21:34.000000 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/bot/bot_config.py
--rw-rw-rw-   0        0        0     5242 2022-09-28 08:21:34.000000 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/bot/bot_config_cfg.py
--rw-rw-rw-   0        0        0     9633 2022-09-28 08:21:34.000000 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/bot/bot_handlers_cfg.py
-drwxrwxrwx   0        0        0        0 2022-09-28 08:48:43.507735 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/command/
--rw-rw-rw-   0        0        0        0 2021-11-30 15:43:37.000000 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/command/__init__.py
--rw-rw-rw-   0        0        0     5568 2022-09-28 08:37:05.000000 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/command/command_base.py
--rw-rw-rw-   0        0        0     4060 2022-09-28 08:36:07.000000 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/command/command_data.py
--rw-rw-rw-   0        0        0     4954 2022-09-28 08:21:34.000000 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/command/command_dispatcher.py
--rw-rw-rw-   0        0        0    15012 2022-09-28 08:21:34.000000 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/command/commands.py
-drwxrwxrwx   0        0        0        0 2022-09-28 08:48:43.514737 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/config/
--rw-rw-rw-   0        0        0        0 2021-11-30 15:43:37.000000 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/config/__init__.py
--rw-rw-rw-   0        0        0     5076 2022-09-28 08:21:34.000000 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/config/config_loader.py
--rw-rw-rw-   0        0        0     2520 2021-11-28 13:12:28.000000 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/config/configurable_object.py
-drwxrwxrwx   0        0        0        0 2022-09-28 08:48:43.517736 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/lang/
--rw-rw-rw-   0        0        0     6841 2021-12-09 21:52:07.000000 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/lang/lang_en.xml
-drwxrwxrwx   0        0        0        0 2022-09-28 08:48:43.520736 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/logger/
--rw-rw-rw-   0        0        0        0 2021-11-30 15:43:37.000000 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/logger/__init__.py
--rw-rw-rw-   0        0        0     4688 2022-09-28 08:21:34.000000 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/logger/logger.py
-drwxrwxrwx   0        0        0        0 2022-09-28 08:48:43.530737 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/message/
--rw-rw-rw-   0        0        0        0 2021-11-30 15:43:37.000000 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/message/__init__.py
--rw-rw-rw-   0        0        0     2388 2022-09-28 08:33:33.000000 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/message/message_deleter.py
--rw-rw-rw-   0        0        0     4669 2022-09-28 08:21:34.000000 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/message/message_dispatcher.py
--rw-rw-rw-   0        0        0     3783 2022-09-28 08:32:39.000000 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/message/message_sender.py
-drwxrwxrwx   0        0        0        0 2022-09-28 08:48:43.538947 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/misc/
--rw-rw-rw-   0        0        0        0 2021-11-30 15:43:37.000000 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/misc/__init__.py
--rw-rw-rw-   0        0        0     4264 2022-09-28 08:31:31.000000 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/misc/chat_members.py
--rw-rw-rw-   0        0        0     2933 2022-09-28 08:37:13.000000 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/misc/helpers.py
-drwxrwxrwx   0        0        0        0 2022-09-28 08:48:43.559946 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/periodic_msg/
--rw-rw-rw-   0        0        0        0 2021-11-30 15:43:37.000000 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/periodic_msg/__init__.py
--rw-rw-rw-   0        0        0     4223 2022-09-28 08:21:34.000000 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/periodic_msg/periodic_msg_job.py
--rw-rw-rw-   0        0        0     2423 2022-09-28 08:31:01.000000 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/periodic_msg/periodic_msg_parser.py
--rw-rw-rw-   0        0        0    15176 2022-09-28 08:21:34.000000 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/periodic_msg/periodic_msg_scheduler.py
--rw-rw-rw-   0        0        0     2737 2022-09-28 08:21:34.000000 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/periodic_msg/periodic_msg_sender.py
--rw-rw-rw-   0        0        0     2131 2021-11-30 20:21:55.000000 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/periodic_msg_bot.py
-drwxrwxrwx   0        0        0        0 2022-09-28 08:48:43.564945 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/translator/
--rw-rw-rw-   0        0        0        0 2021-11-30 15:43:37.000000 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/translator/__init__.py
--rw-rw-rw-   0        0        0     3708 2022-09-28 08:21:34.000000 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/translator/translation_loader.py
-drwxrwxrwx   0        0        0        0 2022-09-28 08:48:43.578946 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/utils/
--rw-rw-rw-   0        0        0        0 2021-11-30 15:43:37.000000 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/utils/__init__.py
--rw-rw-rw-   0        0        0     1731 2021-11-21 22:10:52.000000 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/utils/key_value_converter.py
--rw-rw-rw-   0        0        0     3343 2022-09-28 08:36:40.000000 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/utils/pyrogram_wrapper.py
--rw-rw-rw-   0        0        0     1744 2021-10-18 14:20:33.000000 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/utils/utils.py
--rw-rw-rw-   0        0        0     2576 2022-09-28 08:21:34.000000 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/utils/wrapped_list.py
-drwxrwxrwx   0        0        0        0 2022-09-28 08:48:43.483737 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot.egg-info/
--rw-rw-rw-   0        0        0     9390 2022-09-28 08:48:42.000000 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2173 2022-09-28 08:48:43.000000 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-28 08:48:42.000000 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2022-09-28 08:48:43.000000 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2022-09-28 08:48:43.000000 telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 21:52:12.128078 telegram_periodic_msg_bot-0.3.2/
+-rw-rw-rw-   0        0        0     1085 2021-06-09 13:22:24.000000 telegram_periodic_msg_bot-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0       26 2021-10-20 11:44:31.000000 telegram_periodic_msg_bot-0.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     9526 2023-05-16 21:52:12.128078 telegram_periodic_msg_bot-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8465 2022-09-29 12:33:20.000000 telegram_periodic_msg_bot-0.3.2/README.md
+-rw-rw-rw-   0        0        0       52 2022-10-07 12:53:29.000000 telegram_periodic_msg_bot-0.3.2/requirements.txt
+-rw-rw-rw-   0        0        0      111 2023-05-16 21:52:12.131586 telegram_periodic_msg_bot-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     2268 2023-05-07 20:48:19.000000 telegram_periodic_msg_bot-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:52:11.931672 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/
+-rw-rw-rw-   0        0        0      148 2021-09-28 14:11:55.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/__init__.py
+-rw-rw-rw-   0        0        0       28 2023-05-16 21:03:22.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/_version.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:52:11.980700 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/bot/
+-rw-rw-rw-   0        0        0        0 2021-11-30 15:43:37.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/bot/__init__.py
+-rw-rw-rw-   0        0        0     5126 2022-11-14 20:57:33.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/bot/bot_base.py
+-rw-rw-rw-   0        0        0     5255 2022-11-14 20:55:08.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/bot/bot_config.py
+-rw-rw-rw-   0        0        0     1853 2022-11-14 20:58:52.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/bot/bot_config_types.py
+-rw-rw-rw-   0        0        0     9666 2022-11-14 20:55:08.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/bot/bot_handlers_config.py
+-rw-rw-rw-   0        0        0     1516 2022-11-14 20:21:22.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/bot/bot_handlers_config_typing.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:52:12.002889 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/command/
+-rw-rw-rw-   0        0        0        0 2021-11-30 15:43:37.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/command/__init__.py
+-rw-rw-rw-   0        0        0     5674 2023-05-16 21:00:49.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/command/command_base.py
+-rw-rw-rw-   0        0        0     4060 2022-09-28 08:36:07.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/command/command_data.py
+-rw-rw-rw-   0        0        0     4930 2022-09-28 09:34:18.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/command/command_dispatcher.py
+-rw-rw-rw-   0        0        0    15018 2022-11-14 20:53:58.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/command/commands.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:52:12.035686 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/config/
+-rw-rw-rw-   0        0        0        0 2021-11-21 22:10:52.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/config/__init__.py
+-rw-rw-rw-   0        0        0     1923 2022-11-14 20:57:58.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/config/config_file_sections_loader.py
+-rw-rw-rw-   0        0        0     1339 2022-11-14 19:43:03.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/config/config_loader_ex.py
+-rw-rw-rw-   0        0        0     2201 2022-11-14 20:50:16.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/config/config_object.py
+-rw-rw-rw-   0        0        0     4105 2022-11-14 20:58:07.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/config/config_section_loader.py
+-rw-rw-rw-   0        0        0     2190 2022-11-14 20:58:10.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/config/config_sections_loader.py
+-rw-rw-rw-   0        0        0     1319 2022-11-14 15:20:40.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/config/config_typing.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:52:12.039699 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/lang/
+-rw-rw-rw-   0        0        0     6852 2023-05-06 18:01:43.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/lang/lang_en.xml
+drwxrwxrwx   0        0        0        0 2023-05-16 21:52:12.046509 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/logger/
+-rw-rw-rw-   0        0        0        0 2021-11-30 15:43:37.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/logger/__init__.py
+-rw-rw-rw-   0        0        0     4670 2022-11-14 20:53:58.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/logger/logger.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:52:12.066445 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/message/
+-rw-rw-rw-   0        0        0        0 2021-11-30 15:43:37.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/message/__init__.py
+-rw-rw-rw-   0        0        0     2388 2022-09-28 08:33:33.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/message/message_deleter.py
+-rw-rw-rw-   0        0        0     4645 2022-09-28 09:34:18.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/message/message_dispatcher.py
+-rw-rw-rw-   0        0        0     3783 2022-09-28 08:32:39.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/message/message_sender.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:52:12.074009 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/misc/
+-rw-rw-rw-   0        0        0        0 2021-11-30 15:43:37.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/misc/__init__.py
+-rw-rw-rw-   0        0        0     4270 2022-11-22 15:43:06.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/misc/chat_members.py
+-rw-rw-rw-   0        0        0     2933 2022-09-28 08:37:13.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/misc/helpers.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:52:12.094606 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/periodic_msg/
+-rw-rw-rw-   0        0        0        0 2021-11-30 15:43:37.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/periodic_msg/__init__.py
+-rw-rw-rw-   0        0        0     4223 2022-09-28 08:21:34.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/periodic_msg/periodic_msg_job.py
+-rw-rw-rw-   0        0        0     2405 2022-11-14 20:53:57.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/periodic_msg/periodic_msg_parser.py
+-rw-rw-rw-   0        0        0    15158 2022-11-14 20:53:58.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/periodic_msg/periodic_msg_scheduler.py
+-rw-rw-rw-   0        0        0     2737 2022-09-28 08:21:34.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/periodic_msg/periodic_msg_sender.py
+-rw-rw-rw-   0        0        0     2011 2022-11-14 20:57:49.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/periodic_msg_bot.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:52:12.101607 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/translator/
+-rw-rw-rw-   0        0        0        0 2021-11-30 15:43:37.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/translator/__init__.py
+-rw-rw-rw-   0        0        0     3708 2022-09-28 08:21:34.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/translator/translation_loader.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:52:12.124081 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/utils/
+-rw-rw-rw-   0        0        0        0 2021-11-30 15:43:37.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/utils/__init__.py
+-rw-rw-rw-   0        0        0     1731 2021-11-21 22:10:52.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/utils/key_value_converter.py
+-rw-rw-rw-   0        0        0     3343 2022-09-28 08:36:40.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/utils/pyrogram_wrapper.py
+-rw-rw-rw-   0        0        0     1744 2021-10-18 14:20:33.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/utils/utils.py
+-rw-rw-rw-   0        0        0     2576 2023-05-06 12:57:23.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/utils/wrapped_list.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:52:11.947701 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot.egg-info/
+-rw-rw-rw-   0        0        0     9526 2023-05-16 21:52:11.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2466 2023-05-16 21:52:11.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 21:52:11.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-16 21:52:11.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-05-16 21:52:11.000000 telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot.egg-info/top_level.txt
```

### Comparing `telegram_periodic_msg_bot-0.3.1/LICENSE` & `telegram_periodic_msg_bot-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `telegram_periodic_msg_bot-0.3.1/PKG-INFO` & `telegram_periodic_msg_bot-0.3.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: telegram_periodic_msg_bot
-Version: 0.3.1
+Version: 0.3.2
 Summary: Telegram bot for sending periodic messages
 Home-page: https://github.com/ebellocchia/telegram_periodic_msg_bot
-Download-URL: https://github.com/ebellocchia/telegram_periodic_msg_bot/archive/v0.3.1.tar.gz
+Download-URL: https://github.com/ebellocchia/telegram_periodic_msg_bot/archive/v0.3.2.tar.gz
 Author: Emanuele Bellocchia
 Author-email: ebellocchia@gmail.com
 Maintainer: Emanuele Bellocchia
 Maintainer-email: ebellocchia@gmail.com
 License: MIT
 Keywords: telegram,bot,telegram bot,periodic messages
 Platform: any
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -69,67 +70,74 @@
 
 An example of configuration file is provided in the *app/conf* folder.\
 The list of all possible fields that can be set is shown below.
 
 |Name|Description|
 |---|---|
 |**[pyrogram]**|Configuration for pyrogram|
-|session_name|Session name of your choice|
-|api_id|API ID from [https://my.telegram.org/apps](https://my.telegram.org/apps)|
-|api_hash|API hash from [https://my.telegram.org/apps](https://my.telegram.org/apps)|
-|bot_token|Bot token from BotFather|
+|`session_name`|Session name of your choice|
+|`api_id`|API ID from [https://my.telegram.org/apps](https://my.telegram.org/apps)|
+|`api_hash`|API hash from [https://my.telegram.org/apps](https://my.telegram.org/apps)|
+|`bot_token`|Bot token from BotFather|
 |**[app]**|Configuration for app|
-|app_is_test_mode|True to activate test mode false otherwise|
-|app_lang_file|Language file in XML format (default: English)|
+|`app_is_test_mode`|True to activate test mode false otherwise|
+|`app_lang_file`|Language file in XML format (default: English)|
 |**[task]**|Configuration for tasks|
-|tasks_max_num|Maximum number of running tasks (totally, in all groups). Default: 20.|
+|`tasks_max_num`|Maximum number of running tasks (totally, in all groups). Default: 20.|
 |**[message]**|Configuration for message|
-|message_max_len|Maximum message length in characters. Default: 4000.|
+|`message_max_len`|Maximum message length in characters. Default: 4000.|
 |**[logging]**|Configuration for logging|
-|log_level|Log level, same of python logging (*DEBUG*, *INFO*, *WARNING*, *ERROR*, *CRITICAL*). Default: *INFO*.|
-|log_console_enabled|True to enable logging to console, false otherwise (default: true)|
-|log_file_enabled|True to enable logging to file, false otherwise (default: false). If false, all the next fields will be skipped.|
-|log_file_name|Log file name|
-|log_file_use_rotating|True for using a rotating log file, false otherwise|
-|log_file_max_bytes|Maximum size in bytes for a log file. When reached, a new log file is created up to *log_file_backup_cnt*.. Valid only if log_file_use_rotating is true.|
-|log_file_backup_cnt|Maximum number of log files. Valid only if log_file_use_rotating is true.|
-|log_file_append|True to append to log file, false to start from a new file each time. Valid only if log_file_use_rotating is false.|
+|`log_level`|Log level, same of python logging (`DEBUG`, `INFO`, `WARNING`, `ERROR`, `CRITICAL`). Default: `INFO`.|
+|`log_console_enabled`|True to enable logging to console, false otherwise (default: `true`)|
+|`log_file_enabled`|True to enable logging to file, false otherwise (default: `false`). If false, all the next fields will be skipped.|
+|`log_file_name`|Log file name|
+|`log_file_use_rotating`|True for using a rotating log file, false otherwise|
+|`log_file_max_bytes`|Maximum size in bytes for a log file. When reached, a new log file is created up to `log_file_backup_cnt`. Valid only if `log_file_use_rotating` is true.|
+|`log_file_backup_cnt`|Maximum number of log files. Valid only if `log_file_use_rotating` is true.|
+|`log_file_append`|True to append to log file, false to start from a new file each time. Valid only if `log_file_use_rotating` is false.|
 
 ## Supported Commands
 
 List of supported commands:
-- **/help**: show this message
-- **/alive**: show if bot is active
-- **/msgbot_set_test_mode true/false**: enable/disable test mode
-- **/msgbot_is_test_mode**: show if test mode is enabled
-- **/msgbot_version**: show bot version
-- **/msgbot_task_start *MSG_ID PERIOD_HOURS [START_HOUR] MSG***: start a message task in the current chat. If the task *MSG_ID* already exists in the current chat, an error message will be shown. To start it again, it shall be stopped with the *msgbot_task_stop* command.
-    - *MSG_ID*: Message ID
-    - *PERIOD_HOURS*: Task period in hours, it shall be between 1 and 24
-    - *START_HOUR* (optional): Task start hour, it shall be between 0 and 23. Default value: 0.
-    - *MSG*: Message to be sent periodically, it shall be on a new line
-- **/msgbot_task_stop *MSG_ID***: stop the specified message task in the current chat. If the task *MSG_ID* does not exist in the current chat, an error message will be shown.
-    - *MSG_ID*: CoinGecko *ID*
-- **/msgbot_task_stop_all**: stop all message tasks in the current chat
-- **/msgbot_task_pause *MSG_ID***: pause the specified message task in the current chat. If the task *MSG_ID* does not exist in the current chat, an error message will be shown.
-    - *MSG_ID*: Message ID
-- **/msgbot_task_resume *MSG_ID***: resume the specified message task in the current chat. If the task *MSG_ID* does not exist in the current chat, an error message will be shown.
-    - *MSG_ID*: Message ID
-- **/msgbot_task_get *MSG_ID***: show the message set for the specified message task in the current chat.
-    - *MSG_ID*: Message ID
-- **/msgbot_task_set *MSG_ID MSG***: set the message of the specified message task in the current chat
-    - *MSG_ID*: Message ID
-    - *MSG*: Message to be sent periodically, it shall be on a new line
-- **/msgbot_task_delete_last_msg *MSG_ID true/false***: enable/disable the deletion of last messages for the specified message task in the current chat. If the task *MSG_ID* does not exist in the current chat, an error message will be shown.
-    - *MSG_ID*: Message ID
-    - *flag*: true or false
-- **/msgbot_task_info**: show the list of active message tasks in the current chat
+- `help`: show this message
+- `alive`: show if bot is active
+- `msgbot_set_test_mode true/false`: enable/disable test mode
+- `msgbot_is_test_mode`: show if test mode is enabled
+- `msgbot_version`: show bot version
+- `msgbot_task_start MSG_ID PERIOD_HOURS [START_HOUR] MSG`: start a message task in the current chat. If the task `MSG_ID` already exists in the current chat, an error message will be shown. To start it again, it shall be stopped with the `msgbot_task_stop` command.\
+Parameters:
+    - `MSG_ID`: Message ID
+    - `PERIOD_HOURS`: Task period in hours, it shall be between 1 and 24
+    - `START_HOUR` (optional): Task start hour, it shall be between 0 and 23. Default value: 0.
+    - `MSG`: Message to be sent periodically, it shall be on a new line
+- `msgbot_task_stop MSG_ID`: stop the specified message task in the current chat. If the task `MSG_ID` does not exist in the current chat, an error message will be shown.\
+Parameters:
+    - `MSG_ID`: CoinGecko *ID*
+- `msgbot_task_stop_all`: stop all message tasks in the current chat
+- `msgbot_task_pause MSG_ID`: pause the specified message task in the current chat. If the task `MSG_ID` does not exist in the current chat, an error message will be shown.\
+Parameters:
+    - `MSG_ID`: Message ID
+- `msgbot_task_resume MSG_ID`: resume the specified message task in the current chat. If the task `MSG_ID` does not exist in the current chat, an error message will be shown.\
+Parameters:
+    - `MSG_ID`: Message ID
+- `msgbot_task_get MSG_ID`: show the message set for the specified message task in the current chat.\
+Parameters:
+    - `MSG_ID`: Message ID
+- `msgbot_task_set MSG_ID MSG`: set the message of the specified message task in the current chat.\
+Parameters:
+    - `MSG_ID`: Message ID
+    - `MSG`: Message to be sent periodically, it shall be on a new line
+- `msgbot_task_delete_last_msg MSG_ID true/false`: enable/disable the deletion of last messages for the specified message task in the current chat. If the task `MSG_ID` does not exist in the current chat, an error message will be shown.\
+Parameters:
+    - `MSG_ID`: Message ID
+    - `flag`: true or false
+- `msgbot_task_info`: show the list of active message tasks in the current chat
 
 Messages can contain HTML tags if needed (e.g. for bold/italic text), while Markdown tags are not supported.\
-By default, a message task will delete the last sent message when sending a new one. This can be enabled/disabled with the *msgbot_task_delete_last_msg* command.
+By default, a message task will delete the last sent message when sending a new one. This can be enabled/disabled with the `msgbot_task_delete_last_msg` command.
 
 The task period starts from the specified starting hour (be sure to set the correct time on the VPS), for example:
 - A task period of 8 hours starting from 00:00 will send the message at: 00:00, 08:00 and 16:00
 - A task period of 6 hours starting from 08:00 will send the message at: 08:00, 14:00, 20:00 and 02:00
 
 **Examples**
 
@@ -174,13 +182,13 @@
 ## Test Mode
 
 During test mode, the bot will work as usual but the task period will be applied in minutes instead of hours. This allows to quickly check if it is working.
 
 ## Translation
 
 The messages sent by the bot on Telegram can be translated into different languages (the default language is English) by providing a custom XML file.\
-The XML file path is specified in the configuration file (*app_lang_file* field).\
+The XML file path is specified in the configuration file (`app_lang_file` field).\
 An example XML file in italian is provided in the folder *app/lang*.
 
 # License
 
 This software is available under the MIT license.
```

### Comparing `telegram_periodic_msg_bot-0.3.1/README.md` & `telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+Metadata-Version: 2.1
+Name: telegram-periodic-msg-bot
+Version: 0.3.2
+Summary: Telegram bot for sending periodic messages
+Home-page: https://github.com/ebellocchia/telegram_periodic_msg_bot
+Download-URL: https://github.com/ebellocchia/telegram_periodic_msg_bot/archive/v0.3.2.tar.gz
+Author: Emanuele Bellocchia
+Author-email: ebellocchia@gmail.com
+Maintainer: Emanuele Bellocchia
+Maintainer-email: ebellocchia@gmail.com
+License: MIT
+Keywords: telegram,bot,telegram bot,periodic messages
+Platform: any
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Telegram Periodic Message Bot
 
 [![PyPI version](https://badge.fury.io/py/telegram-periodic-msg-bot.svg)](https://badge.fury.io/py/telegram-periodic-msg-bot)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/d1cc7c1692de4939a23e626981923e83)](https://www.codacy.com/gh/ebellocchia/telegram_periodic_msg_bot/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=ebellocchia/telegram_periodic_msg_bot&amp;utm_campaign=Badge_Grade)
 [![CodeFactor](https://www.codefactor.io/repository/github/ebellocchia/telegram_periodic_msg_bot/badge)](https://www.codefactor.io/repository/github/ebellocchia/telegram_periodic_msg_bot)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://raw.githubusercontent.com/ebellocchia/bip_utils/master/LICENSE)
 
@@ -44,67 +70,74 @@
 
 An example of configuration file is provided in the *app/conf* folder.\
 The list of all possible fields that can be set is shown below.
 
 |Name|Description|
 |---|---|
 |**[pyrogram]**|Configuration for pyrogram|
-|session_name|Session name of your choice|
-|api_id|API ID from [https://my.telegram.org/apps](https://my.telegram.org/apps)|
-|api_hash|API hash from [https://my.telegram.org/apps](https://my.telegram.org/apps)|
-|bot_token|Bot token from BotFather|
+|`session_name`|Session name of your choice|
+|`api_id`|API ID from [https://my.telegram.org/apps](https://my.telegram.org/apps)|
+|`api_hash`|API hash from [https://my.telegram.org/apps](https://my.telegram.org/apps)|
+|`bot_token`|Bot token from BotFather|
 |**[app]**|Configuration for app|
-|app_is_test_mode|True to activate test mode false otherwise|
-|app_lang_file|Language file in XML format (default: English)|
+|`app_is_test_mode`|True to activate test mode false otherwise|
+|`app_lang_file`|Language file in XML format (default: English)|
 |**[task]**|Configuration for tasks|
-|tasks_max_num|Maximum number of running tasks (totally, in all groups). Default: 20.|
+|`tasks_max_num`|Maximum number of running tasks (totally, in all groups). Default: 20.|
 |**[message]**|Configuration for message|
-|message_max_len|Maximum message length in characters. Default: 4000.|
+|`message_max_len`|Maximum message length in characters. Default: 4000.|
 |**[logging]**|Configuration for logging|
-|log_level|Log level, same of python logging (*DEBUG*, *INFO*, *WARNING*, *ERROR*, *CRITICAL*). Default: *INFO*.|
-|log_console_enabled|True to enable logging to console, false otherwise (default: true)|
-|log_file_enabled|True to enable logging to file, false otherwise (default: false). If false, all the next fields will be skipped.|
-|log_file_name|Log file name|
-|log_file_use_rotating|True for using a rotating log file, false otherwise|
-|log_file_max_bytes|Maximum size in bytes for a log file. When reached, a new log file is created up to *log_file_backup_cnt*.. Valid only if log_file_use_rotating is true.|
-|log_file_backup_cnt|Maximum number of log files. Valid only if log_file_use_rotating is true.|
-|log_file_append|True to append to log file, false to start from a new file each time. Valid only if log_file_use_rotating is false.|
+|`log_level`|Log level, same of python logging (`DEBUG`, `INFO`, `WARNING`, `ERROR`, `CRITICAL`). Default: `INFO`.|
+|`log_console_enabled`|True to enable logging to console, false otherwise (default: `true`)|
+|`log_file_enabled`|True to enable logging to file, false otherwise (default: `false`). If false, all the next fields will be skipped.|
+|`log_file_name`|Log file name|
+|`log_file_use_rotating`|True for using a rotating log file, false otherwise|
+|`log_file_max_bytes`|Maximum size in bytes for a log file. When reached, a new log file is created up to `log_file_backup_cnt`. Valid only if `log_file_use_rotating` is true.|
+|`log_file_backup_cnt`|Maximum number of log files. Valid only if `log_file_use_rotating` is true.|
+|`log_file_append`|True to append to log file, false to start from a new file each time. Valid only if `log_file_use_rotating` is false.|
 
 ## Supported Commands
 
 List of supported commands:
-- **/help**: show this message
-- **/alive**: show if bot is active
-- **/msgbot_set_test_mode true/false**: enable/disable test mode
-- **/msgbot_is_test_mode**: show if test mode is enabled
-- **/msgbot_version**: show bot version
-- **/msgbot_task_start *MSG_ID PERIOD_HOURS [START_HOUR] MSG***: start a message task in the current chat. If the task *MSG_ID* already exists in the current chat, an error message will be shown. To start it again, it shall be stopped with the *msgbot_task_stop* command.
-    - *MSG_ID*: Message ID
-    - *PERIOD_HOURS*: Task period in hours, it shall be between 1 and 24
-    - *START_HOUR* (optional): Task start hour, it shall be between 0 and 23. Default value: 0.
-    - *MSG*: Message to be sent periodically, it shall be on a new line
-- **/msgbot_task_stop *MSG_ID***: stop the specified message task in the current chat. If the task *MSG_ID* does not exist in the current chat, an error message will be shown.
-    - *MSG_ID*: CoinGecko *ID*
-- **/msgbot_task_stop_all**: stop all message tasks in the current chat
-- **/msgbot_task_pause *MSG_ID***: pause the specified message task in the current chat. If the task *MSG_ID* does not exist in the current chat, an error message will be shown.
-    - *MSG_ID*: Message ID
-- **/msgbot_task_resume *MSG_ID***: resume the specified message task in the current chat. If the task *MSG_ID* does not exist in the current chat, an error message will be shown.
-    - *MSG_ID*: Message ID
-- **/msgbot_task_get *MSG_ID***: show the message set for the specified message task in the current chat.
-    - *MSG_ID*: Message ID
-- **/msgbot_task_set *MSG_ID MSG***: set the message of the specified message task in the current chat
-    - *MSG_ID*: Message ID
-    - *MSG*: Message to be sent periodically, it shall be on a new line
-- **/msgbot_task_delete_last_msg *MSG_ID true/false***: enable/disable the deletion of last messages for the specified message task in the current chat. If the task *MSG_ID* does not exist in the current chat, an error message will be shown.
-    - *MSG_ID*: Message ID
-    - *flag*: true or false
-- **/msgbot_task_info**: show the list of active message tasks in the current chat
+- `help`: show this message
+- `alive`: show if bot is active
+- `msgbot_set_test_mode true/false`: enable/disable test mode
+- `msgbot_is_test_mode`: show if test mode is enabled
+- `msgbot_version`: show bot version
+- `msgbot_task_start MSG_ID PERIOD_HOURS [START_HOUR] MSG`: start a message task in the current chat. If the task `MSG_ID` already exists in the current chat, an error message will be shown. To start it again, it shall be stopped with the `msgbot_task_stop` command.\
+Parameters:
+    - `MSG_ID`: Message ID
+    - `PERIOD_HOURS`: Task period in hours, it shall be between 1 and 24
+    - `START_HOUR` (optional): Task start hour, it shall be between 0 and 23. Default value: 0.
+    - `MSG`: Message to be sent periodically, it shall be on a new line
+- `msgbot_task_stop MSG_ID`: stop the specified message task in the current chat. If the task `MSG_ID` does not exist in the current chat, an error message will be shown.\
+Parameters:
+    - `MSG_ID`: CoinGecko *ID*
+- `msgbot_task_stop_all`: stop all message tasks in the current chat
+- `msgbot_task_pause MSG_ID`: pause the specified message task in the current chat. If the task `MSG_ID` does not exist in the current chat, an error message will be shown.\
+Parameters:
+    - `MSG_ID`: Message ID
+- `msgbot_task_resume MSG_ID`: resume the specified message task in the current chat. If the task `MSG_ID` does not exist in the current chat, an error message will be shown.\
+Parameters:
+    - `MSG_ID`: Message ID
+- `msgbot_task_get MSG_ID`: show the message set for the specified message task in the current chat.\
+Parameters:
+    - `MSG_ID`: Message ID
+- `msgbot_task_set MSG_ID MSG`: set the message of the specified message task in the current chat.\
+Parameters:
+    - `MSG_ID`: Message ID
+    - `MSG`: Message to be sent periodically, it shall be on a new line
+- `msgbot_task_delete_last_msg MSG_ID true/false`: enable/disable the deletion of last messages for the specified message task in the current chat. If the task `MSG_ID` does not exist in the current chat, an error message will be shown.\
+Parameters:
+    - `MSG_ID`: Message ID
+    - `flag`: true or false
+- `msgbot_task_info`: show the list of active message tasks in the current chat
 
 Messages can contain HTML tags if needed (e.g. for bold/italic text), while Markdown tags are not supported.\
-By default, a message task will delete the last sent message when sending a new one. This can be enabled/disabled with the *msgbot_task_delete_last_msg* command.
+By default, a message task will delete the last sent message when sending a new one. This can be enabled/disabled with the `msgbot_task_delete_last_msg` command.
 
 The task period starts from the specified starting hour (be sure to set the correct time on the VPS), for example:
 - A task period of 8 hours starting from 00:00 will send the message at: 00:00, 08:00 and 16:00
 - A task period of 6 hours starting from 08:00 will send the message at: 08:00, 14:00, 20:00 and 02:00
 
 **Examples**
 
@@ -149,13 +182,13 @@
 ## Test Mode
 
 During test mode, the bot will work as usual but the task period will be applied in minutes instead of hours. This allows to quickly check if it is working.
 
 ## Translation
 
 The messages sent by the bot on Telegram can be translated into different languages (the default language is English) by providing a custom XML file.\
-The XML file path is specified in the configuration file (*app_lang_file* field).\
+The XML file path is specified in the configuration file (`app_lang_file` field).\
 An example XML file in italian is provided in the folder *app/lang*.
 
 # License
 
 This software is available under the MIT license.
```

### Comparing `telegram_periodic_msg_bot-0.3.1/setup.py` & `telegram_periodic_msg_bot-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     keywords="telegram, bot, telegram bot, periodic messages",
     platforms=["any"],
     classifiers=[
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Intended Audience :: Developers",
     ],
     python_requires=">=3.7",
 )
```

### Comparing `telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/bot/bot_base.py` & `telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/bot/bot_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,60 +17,52 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
 #
 # Imports
 #
-from typing import Any, Dict, List
+from typing import Any
 
 import pyrogram
 from pyrogram import Client
 
-from telegram_periodic_msg_bot.bot.bot_config import BotConfig, BotConfigTypes
+from telegram_periodic_msg_bot.bot.bot_config_types import BotConfigTypes
+from telegram_periodic_msg_bot.bot.bot_handlers_config_typing import BotHandlersConfigType
 from telegram_periodic_msg_bot.command.command_dispatcher import CommandDispatcher, CommandTypes
-from telegram_periodic_msg_bot.config.config_loader import ConfigCfgType, ConfigLoader
-from telegram_periodic_msg_bot.config.configurable_object import ConfigurableObject
+from telegram_periodic_msg_bot.config.config_file_sections_loader import ConfigFileSectionsLoader
+from telegram_periodic_msg_bot.config.config_object import ConfigObject
+from telegram_periodic_msg_bot.config.config_typing import ConfigSectionsType
 from telegram_periodic_msg_bot.logger.logger import Logger
 from telegram_periodic_msg_bot.message.message_dispatcher import MessageDispatcher, MessageTypes
 from telegram_periodic_msg_bot.translator.translation_loader import TranslationLoader
 
 
 #
-# Types
-#
-
-# Handlers configuration type
-HandlersCfgType = Dict[Any, List[Dict[str, Any]]]
-
-
-#
 # Classes
 #
 
 
 # Bot base class
 class BotBase:
 
-    config: ConfigurableObject
+    config: ConfigObject
     logger: Logger
     translator: TranslationLoader
     client: pyrogram.Client
     cmd_dispatcher: CommandDispatcher
     msg_dispatcher: MessageDispatcher
 
     # Constructor
     def __init__(self,
                  config_file: str,
-                 config_cfg: ConfigCfgType,
-                 handlers_cfg: HandlersCfgType) -> None:
+                 config_sections: ConfigSectionsType,
+                 handlers_config: BotHandlersConfigType) -> None:
         # Load configuration
-        config_ldr = ConfigLoader(BotConfig(), config_cfg)
-        config_ldr.Load(config_file)
-        self.config = config_ldr.GetLoadedObject()
+        self.config = ConfigFileSectionsLoader.Load(config_file, config_sections)
         # Initialize logger
         self.logger = Logger(self.config)
         # Initialize translations
         self.translator = TranslationLoader(self.logger)
         self.translator.Load(self.config.GetValue(BotConfigTypes.APP_LANG_FILE))
         # Initialize client
         self.client = Client(
@@ -79,30 +71,30 @@
             api_hash=self.config.GetValue(BotConfigTypes.API_HASH),
             bot_token=self.config.GetValue(BotConfigTypes.BOT_TOKEN)
         )
         # Initialize helper classes
         self.cmd_dispatcher = CommandDispatcher(self.config, self.logger, self.translator)
         self.msg_dispatcher = MessageDispatcher(self.config, self.logger, self.translator)
         # Setup handlers
-        self._SetupHandlers(handlers_cfg)
+        self._SetupHandlers(handlers_config)
         # Log
         self.logger.GetLogger().info("Bot initialization completed")
 
     # Run bot
     def Run(self) -> None:
         # Print
         self.logger.GetLogger().info("Bot started!\n")
         # Run client
         self.client.run()
 
     # Setup handlers
     def _SetupHandlers(self,
-                       handlers_cfg: HandlersCfgType) -> None:
+                       handlers_config: BotHandlersConfigType) -> None:
         # Add all configured handlers
-        for curr_hnd_type, curr_hnd_cfg in handlers_cfg.items():
+        for curr_hnd_type, curr_hnd_cfg in handlers_config.items():
             for handler_cfg in curr_hnd_cfg:
                 self.client.add_handler(
                     # Little "hack" to keep a local scope for current configuration
                     (
                         lambda curr_type=curr_hnd_type, curr_cfg=handler_cfg:
                             curr_type(lambda client, message: curr_cfg["callback"](self, client, message),
                                       curr_cfg["filters"])
```

### Comparing `telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/bot/bot_config.py` & `telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/bot/bot_config_types.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,24 +19,24 @@
 # THE SOFTWARE.
 
 #
 # Imports
 #
 from enum import auto, unique
 
-from telegram_periodic_msg_bot.config.configurable_object import ConfigurableObject, ConfigurableTypes
+from telegram_periodic_msg_bot.config.config_object import ConfigTypes
 
 
 #
 # Enumerations
 #
 
 # Bot configuration types
 @unique
-class BotConfigTypes(ConfigurableTypes):
+class BotConfigTypes(ConfigTypes):
     API_ID = auto()
     API_HASH = auto()
     BOT_TOKEN = auto()
     SESSION_NAME = auto()
     # App
     APP_TEST_MODE = auto()
     APP_LANG_FILE = auto()
@@ -49,16 +49,7 @@
     LOG_CONSOLE_ENABLED = auto()
     LOG_FILE_ENABLED = auto()
     LOG_FILE_NAME = auto()
     LOG_FILE_USE_ROTATING = auto()
     LOG_FILE_APPEND = auto()
     LOG_FILE_MAX_BYTES = auto()
     LOG_FILE_BACKUP_CNT = auto()
-
-
-#
-# Classes
-#
-
-# Bot configuration class
-class BotConfig(ConfigurableObject):
-    pass
```

### Comparing `telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/bot/bot_config_cfg.py` & `telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/bot/bot_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 # THE SOFTWARE.
 
 #
 # Imports
 #
 import logging
 
-from telegram_periodic_msg_bot.bot.bot_config import BotConfigTypes
-from telegram_periodic_msg_bot.config.config_loader import ConfigCfgType
+from telegram_periodic_msg_bot.bot.bot_config_types import BotConfigTypes
+from telegram_periodic_msg_bot.config.config_typing import ConfigSectionsType
 from telegram_periodic_msg_bot.utils.key_value_converter import KeyValueConverter
 from telegram_periodic_msg_bot.utils.utils import Utils
 
 
 #
 # Variables
 #
@@ -40,15 +40,15 @@
     "WARNING": logging.WARNING,
     "ERROR": logging.ERROR,
     "CRITICAL": logging.CRITICAL,
 })
 
 
 # Bot configuration
-BotConfigCfg: ConfigCfgType = {
+BotConfig: ConfigSectionsType = {
     # Pyrogram
     "pyrogram": [
         {
             "type": BotConfigTypes.API_ID,
             "name": "api_id",
         },
         {
```

### Comparing `telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/bot/bot_handlers_cfg.py` & `telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/bot/bot_handlers_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,25 +20,25 @@
 
 #
 # Imports
 #
 from pyrogram import filters
 from pyrogram.handlers import MessageHandler
 
-from telegram_periodic_msg_bot.bot.bot_base import HandlersCfgType
+from telegram_periodic_msg_bot.bot.bot_handlers_config_typing import BotHandlersConfigType
 from telegram_periodic_msg_bot.command.command_dispatcher import CommandTypes
 from telegram_periodic_msg_bot.message.message_dispatcher import MessageTypes
 
 
 #
 # Classes
 #
 
 # Bot handlers configuration
-BotHandlersCfg: HandlersCfgType = {
+BotHandlersConfig: BotHandlersConfigType = {
     # Handlers for MessageHandler
     MessageHandler: [
 
         #
         # Generic commands
         #
```

### Comparing `telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/command/command_base.py` & `telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/command/command_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from abc import ABC, abstractmethod
 from typing import Any
 
 import pyrogram
 from pyrogram.errors import RPCError
 
 from telegram_periodic_msg_bot.command.command_data import CommandData
-from telegram_periodic_msg_bot.config.configurable_object import ConfigurableObject
+from telegram_periodic_msg_bot.config.config_object import ConfigObject
 from telegram_periodic_msg_bot.logger.logger import Logger
 from telegram_periodic_msg_bot.message.message_sender import MessageSender
 from telegram_periodic_msg_bot.misc.chat_members import ChatMembersGetter
 from telegram_periodic_msg_bot.misc.helpers import ChatHelper, UserHelper
 from telegram_periodic_msg_bot.translator.translation_loader import TranslationLoader
 
 
@@ -42,25 +42,25 @@
 
 #
 # Generic command base class
 #
 class CommandBase(ABC):
 
     client: pyrogram.Client
-    config: ConfigurableObject
+    config: ConfigObject
     logger: Logger
     translator: TranslationLoader
     message: pyrogram.types.Message
     cmd_data: CommandData
     message_sender: MessageSender
 
     # Constructor
     def __init__(self,
                  client: pyrogram.Client,
-                 config: ConfigurableObject,
+                 config: ConfigObject,
                  logger: Logger,
                  translator: TranslationLoader) -> None:
         self.client = client
         self.config = config
         self.logger = logger
         self.translator = translator
         # Helper classes
@@ -111,30 +111,34 @@
 
     # Get if user is anonymous
     def _IsUserAnonymous(self) -> bool:
         return self.cmd_data.User() is None
 
     # Get if user is authorized
     def _IsUserAuthorized(self) -> bool:
+        # In channels only admins can write, so we consider the user authorized since there is no way to know the specific user
+        # This is a limitation for channels only
+        if self._IsChannel():
+            return True
+
+        # Anonymous user
         cmd_user = self.cmd_data.User()
         if cmd_user is None:
             return False
-
-        # In channels only admins can write, so we consider the user authorized since there is no way to know the specific user
-        # This is a limitation for channels only
+        # Private chat is always authorized
         if ChatHelper.IsPrivateChat(self.cmd_data.Chat(), cmd_user):
             return True
-
+        # Check if admin
         admin_members = ChatMembersGetter(self.client).GetAdmins(self.cmd_data.Chat())
         return any((cmd_user.id == member.user.id for member in admin_members if member.user is not None))
 
     # Get if chat is private
     def _IsPrivateChat(self) -> bool:
         cmd_user = self.cmd_data.User()
-        if self._IsChannel() or cmd_user is None:
+        if cmd_user is None:
             return False
         return ChatHelper.IsPrivateChat(self.cmd_data.Chat(), cmd_user)
 
     # Log command
     def __LogCommand(self) -> None:
         self.logger.GetLogger().info(f"Command: {self.cmd_data.Name()}")
         self.logger.GetLogger().info(f"Executed by user: {UserHelper.GetNameOrId(self.cmd_data.User())}")
```

### Comparing `telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/command/command_data.py` & `telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/command/command_data.py`

 * *Files identical despite different names*

### Comparing `telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/command/command_dispatcher.py` & `telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/command/command_dispatcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 from telegram_periodic_msg_bot.command.command_base import CommandBase
 from telegram_periodic_msg_bot.command.commands import (
     AliveCmd, HelpCmd, IsTestModeCmd, MessageTaskDeleteLastMsgCmd, MessageTaskGetCmd, MessageTaskInfoCmd,
     MessageTaskPauseCmd, MessageTaskResumeCmd, MessageTaskSetCmd, MessageTaskStartCmd, MessageTaskStopAllCmd,
     MessageTaskStopCmd, SetTestModeCmd, VersionCmd
 )
-from telegram_periodic_msg_bot.config.configurable_object import ConfigurableObject
+from telegram_periodic_msg_bot.config.config_object import ConfigObject
 from telegram_periodic_msg_bot.logger.logger import Logger
 from telegram_periodic_msg_bot.translator.translation_loader import TranslationLoader
 
 
 #
 # Enumerations
 #
@@ -86,21 +86,21 @@
         CommandTypes.MESSAGE_TASK_INFO_CMD: MessageTaskInfoCmd,
     }
 
 
 # Command dispatcher class
 class CommandDispatcher:
 
-    config: ConfigurableObject
+    config: ConfigObject
     logger: Logger
     translator: TranslationLoader
 
     # Constructor
     def __init__(self,
-                 config: ConfigurableObject,
+                 config: ConfigObject,
                  logger: Logger,
                  translator: TranslationLoader) -> None:
         self.config = config
         self.logger = logger
         self.translator = translator
 
     # Dispatch command
```

### Comparing `telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/command/commands.py` & `telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/command/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 #
 # Imports
 #
 from typing import Any, Callable
 
 from telegram_periodic_msg_bot._version import __version__
-from telegram_periodic_msg_bot.bot.bot_config import BotConfigTypes
+from telegram_periodic_msg_bot.bot.bot_config_types import BotConfigTypes
 from telegram_periodic_msg_bot.command.command_base import CommandBase
 from telegram_periodic_msg_bot.command.command_data import CommandParameterError
 from telegram_periodic_msg_bot.misc.helpers import UserHelper
 from telegram_periodic_msg_bot.periodic_msg.periodic_msg_parser import (
     PeriodicMsgParserInvalidError, PeriodicMsgParserTooLongError
 )
 from telegram_periodic_msg_bot.periodic_msg.periodic_msg_scheduler import (
```

### Comparing `telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/config/config_loader.py` & `telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/config/config_section_loader.py`

 * *Files 25% similar despite different names*

```diff
@@ -18,125 +18,82 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
 #
 # Imports
 #
 import configparser
-from typing import Any, Dict, List
 
-from telegram_periodic_msg_bot.config.configurable_object import ConfigurableObject
-
-
-#
-# Types
-#
-FieldCfgType = Dict[str, Any]
-FieldsCfgType = List[FieldCfgType]
-ConfigCfgType = Dict[str, FieldsCfgType]
+from telegram_periodic_msg_bot.config.config_loader_ex import ConfigFieldNotExistentError, ConfigFieldValueError
+from telegram_periodic_msg_bot.config.config_object import ConfigObject
+from telegram_periodic_msg_bot.config.config_typing import ConfigFieldType, ConfigSectionType
 
 
 #
 # Classes
 #
 
-# Configuration load not existent error class
-class ConfigLoadNotExistentError(Exception):
-    pass
-
+# Configuration section loader class
+class ConfigSectionLoader:
 
-# Configuration load value error class
-class ConfigLoadValueError(Exception):
-    pass
-
-
-# Configuration loader class
-class ConfigLoader:
-
-    config_cfg: ConfigCfgType
-    config_obj: ConfigurableObject
+    config_parser: configparser.ConfigParser
 
     # Constructor
     def __init__(self,
-                 config_obj: ConfigurableObject,
-                 config_cfg: ConfigCfgType) -> None:
-        self.config_cfg = config_cfg
-        self.config_obj = config_obj
-
-    # Load configuration
-    def Load(self,
-             config_file: str) -> None:
-        # Read file
-        config_parser = configparser.ConfigParser()
-        config_parser.read(config_file)
-
-        print(f"\nLoading configuration file {config_file}...\n")
-        # Load sections
-        self.__LoadSections(config_parser)
-        # New line
-
-    # Get object
-    def GetLoadedObject(self) -> ConfigurableObject:
-        return self.config_obj
-
-    # Load sections
-    def __LoadSections(self,
-                       config_parser: configparser.ConfigParser) -> None:
-        # For each section
-        for section, fields in self.config_cfg.items():
-            # Print section
-            print(f"Section [{section}]")
-            # Load fields
-            self.__LoadFields(section, fields, config_parser)
-
-    # Load fields
-    def __LoadFields(self,
-                     section: str,
-                     fields: FieldsCfgType,
-                     config_parser: configparser.ConfigParser) -> None:
+                 config_parser: configparser.ConfigParser) -> None:
+        self.config_parser = config_parser
+
+    # Load section
+    def LoadSection(self,
+                    config_obj: ConfigObject,
+                    section_name: str,
+                    section: ConfigSectionType) -> None:
         # For each field
-        for field in fields:
+        for field in section:
             # Load if needed
-            if self.__FieldShallBeLoaded(field):
+            if self.__FieldShallBeLoaded(config_obj, field):
                 # Set field value and print it
-                self.__SetFieldValue(section, field, config_parser)
-                self.__PrintFieldValue(field)
+                self.__SetFieldValue(config_obj, section_name, field)
+                self.__PrintFieldValue(config_obj, field)
+            # Otherwise set the default value
             else:
                 if "def_val" in field:
-                    self.config_obj.SetValue(field["type"], field["def_val"])
+                    config_obj.SetValue(field["type"], field["def_val"])
 
     # Get if field shall be loaded
-    def __FieldShallBeLoaded(self,
-                             field: FieldCfgType) -> bool:
-        return field["load_if"](self.config_obj) if "load_if" in field else True
+    @staticmethod
+    def __FieldShallBeLoaded(config_obj: ConfigObject,
+                             field: ConfigFieldType) -> bool:
+        return field["load_if"](config_obj) if "load_if" in field else True
 
     # Set field value
     def __SetFieldValue(self,
+                        config_obj: ConfigObject,
                         section: str,
-                        field: FieldCfgType,
-                        config_parser: configparser.ConfigParser) -> None:
+                        field: ConfigFieldType) -> None:
         try:
-            field_val = config_parser[section][field["name"]]
+            field_val = self.config_parser[section][field["name"]]
         # Field not present, set default value if specified
         except KeyError as ex:
             if "def_val" not in field:
-                raise ConfigLoadNotExistentError(f"Configuration field \"{field['name']}\" not found") from ex
+                raise ConfigFieldNotExistentError(f"Configuration field \"{field['name']}\" not found") from ex
             field_val = field["def_val"]
         else:
             # Convert value if needed
             if "conv_fct" in field:
                 field_val = field["conv_fct"](field_val)
 
         # Validate value if needed
-        if "valid_if" in field and not field["valid_if"](self.config_obj, field_val):
-            raise ConfigLoadValueError(f"Value '{field_val}' is not valid for field \"{field['name']}\"")
+        if "valid_if" in field and not field["valid_if"](config_obj, field_val):
+            raise ConfigFieldValueError(f"Value '{field_val}' is not valid for field \"{field['name']}\"")
 
         # Set value
-        self.config_obj.SetValue(field["type"], field_val)
+        config_obj.SetValue(field["type"], field_val)
 
     # Print field value
-    def __PrintFieldValue(self,
-                          field: FieldCfgType) -> None:
+    @staticmethod
+    def __PrintFieldValue(config_obj: ConfigObject,
+                          field: ConfigFieldType) -> None:
         if "print_fct" in field:
-            print(f"- {field['name']}: {field['print_fct'](self.config_obj.GetValue(field['type']))}")
+            print(f"- {field['name']}: {field['print_fct'](config_obj.GetValue(field['type']))}")
         else:
-            print(f"- {field['name']}: {self.config_obj.GetValue(field['type'])}")
+            print(f"- {field['name']}: {config_obj.GetValue(field['type'])}")
```

### Comparing `telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/config/configurable_object.py` & `telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/config/config_object.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,56 +25,44 @@
 from typing import Any, Dict
 
 
 #
 # Enumerations
 #
 
-# Configurable types
-class ConfigurableTypes(Enum):
+# Configuration types
+class ConfigTypes(Enum):
     pass
 
 
 #
 # Classes
 #
 
-# Configurable object class
-class ConfigurableObject:
+# Configuration object class
+class ConfigObject:
 
-    config: Dict[ConfigurableTypes, Any]
+    config: Dict[ConfigTypes, Any]
 
     # Constructor
     def __init__(self) -> None:
         self.config = {}
 
     # Get value
     def GetValue(self,
-                 config_type: ConfigurableTypes) -> Any:
-        if not isinstance(config_type, ConfigurableTypes):
-            raise TypeError("BotConfig type is not an enumerative of ConfigurableTypes")
-
+                 config_type: ConfigTypes) -> Any:
+        if not isinstance(config_type, ConfigTypes):
+            raise TypeError("BotConfig type is not an enumerative of ConfigTypes")
         return self.config[config_type]
 
     # Set value
     def SetValue(self,
-                 config_type: ConfigurableTypes,
+                 config_type: ConfigTypes,
                  value: Any) -> None:
-        if not isinstance(config_type, ConfigurableTypes):
-            raise TypeError("BotConfig type is not an enumerative of ConfigurableTypes")
-
+        if not isinstance(config_type, ConfigTypes):
+            raise TypeError("BotConfig type is not an enumerative of ConfigTypes")
         self.config[config_type] = value
 
     # Get if value is set
     def IsValueSet(self,
-                   config_type: ConfigurableTypes) -> bool:
+                   config_type: ConfigTypes) -> bool:
         return config_type in self.config
-
-    # Convert to string
-    def ToString(self) -> str:
-        return "\n".join(
-            f"{field}: {val}" for field, val in self.config.values()
-        )
-
-    # Convert to string
-    def __str__(self) -> str:
-        return self.ToString()
```

### Comparing `telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/lang/lang_en.xml` & `telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/lang/lang_en.xml`

 * *Files 1% similar despite different names*

#### Comparing `telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/lang/lang_en.xml` & `telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/lang/lang_en.xml`

```diff
@@ -1,13 +1,13 @@
 <?xml version="1.0" encoding="utf-8"?>
 <translation>
   <!-- Help command message -->
   <sentence id="HELP_CMD">**HELP**
 Hi {name},
-welcome to the Telegram Price Bot.
+welcome to the Telegram Periodic Message Bot.
 
 ℹ️ Here is the list of supported commands.
 
 🔘 **/help** : show this message
 🔘 **/alive** : show if bot is active
 🔘 **/msgbot_set_test_mode** __true/false__ : enable/disable test mode
 🔘 **/msgbot_is_test_mode** : show if test mode is enabled
```

### Comparing `telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/logger/logger.py` & `telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/logger/logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 # Imports
 #
 import logging
 import logging.handlers
 import os
 from typing import Union
 
-from telegram_periodic_msg_bot.bot.bot_config import BotConfigTypes
-from telegram_periodic_msg_bot.config.configurable_object import ConfigurableObject
+from telegram_periodic_msg_bot.bot.bot_config_types import BotConfigTypes
+from telegram_periodic_msg_bot.config.config_object import ConfigObject
 
 
 #
 # Classes
 #
 
 # Constants for logger class
@@ -42,20 +42,20 @@
     LOG_CONSOLE_FORMAT: str = "%(asctime)-15s %(levelname)s - %(message)s"
     LOG_FILE_FORMAT: str = "%(asctime)-15s %(levelname)s - [%(name)s.%(funcName)s:%(lineno)d] %(message)s"
 
 
 # Logger class
 class Logger:
 
-    config: ConfigurableObject
+    config: ConfigObject
     logger: logging.Logger
 
     # Constructor
     def __init__(self,
-                 config: ConfigurableObject) -> None:
+                 config: ConfigObject) -> None:
         self.config = config
         self.logger = logging.getLogger(LoggerConst.LOGGER_NAME)
         self.__Init()
 
     # Get logger
     def GetLogger(self) -> logging.Logger:
         return self.logger
```

### Comparing `telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/message/message_deleter.py` & `telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/message/message_deleter.py`

 * *Files identical despite different names*

### Comparing `telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/message/message_dispatcher.py` & `telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/message/message_dispatcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # Imports
 #
 from enum import Enum, auto, unique
 from typing import Any
 
 import pyrogram
 
-from telegram_periodic_msg_bot.config.configurable_object import ConfigurableObject
+from telegram_periodic_msg_bot.config.config_object import ConfigObject
 from telegram_periodic_msg_bot.logger.logger import Logger
 from telegram_periodic_msg_bot.message.message_sender import MessageSender
 from telegram_periodic_msg_bot.translator.translation_loader import TranslationLoader
 
 
 #
 # Enumerations
@@ -47,21 +47,21 @@
 #
 # Classes
 #
 
 # Message dispatcher class
 class MessageDispatcher:
 
-    config: ConfigurableObject
+    config: ConfigObject
     logger: Logger
     translator: TranslationLoader
 
     # Constructor
     def __init__(self,
-                 config: ConfigurableObject,
+                 config: ConfigObject,
                  logger: Logger,
                  translator: TranslationLoader) -> None:
         self.config = config
         self.logger = logger
         self.translator = translator
 
     # Dispatch command
```

### Comparing `telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/message/message_sender.py` & `telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/message/message_sender.py`

 * *Files identical despite different names*

### Comparing `telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/misc/chat_members.py` & `telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/misc/chat_members.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
     # Get the list of chat members by applying the specified filter
     def FilterMembers(self,
                       chat: pyrogram.types.Chat,
                       filter_fct: Optional[Callable[[pyrogram.types.ChatMember], bool]] = None,
                       filter_str: str = "all") -> ChatMembersList:
         # Get members
-        filtered_members = PyrogramWrapper.GetChatMembers(self.client, chat, filter_str)
+        filtered_members = list(PyrogramWrapper.GetChatMembers(self.client, chat, filter_str))
         # Filter them if necessary
         if filter_fct is not None:
             filtered_members = list(filter(filter_fct, filtered_members))   # type: ignore
         # Order filtered members
         filtered_members.sort(      # type: ignore
             key=lambda member: member.user.username.lower() if member.user.username is not None else str(member.user.id)
         )
```

### Comparing `telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/misc/helpers.py` & `telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/misc/helpers.py`

 * *Files identical despite different names*

### Comparing `telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/periodic_msg/periodic_msg_job.py` & `telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/periodic_msg/periodic_msg_job.py`

 * *Files identical despite different names*

### Comparing `telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/periodic_msg/periodic_msg_parser.py` & `telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/periodic_msg/periodic_msg_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 # THE SOFTWARE.
 
 #
 # Imports
 #
 import pyrogram
 
-from telegram_periodic_msg_bot.bot.bot_config import BotConfigTypes
-from telegram_periodic_msg_bot.config.configurable_object import ConfigurableObject
+from telegram_periodic_msg_bot.bot.bot_config_types import BotConfigTypes
+from telegram_periodic_msg_bot.config.config_object import ConfigObject
 
 
 #
 # Classes
 #
 
 # Invalid message error
@@ -40,19 +40,19 @@
 class PeriodicMsgParserTooLongError(Exception):
     pass
 
 
 # Periodic message parser class
 class PeriodicMsgParser:
 
-    config: ConfigurableObject
+    config: ConfigObject
 
     # Constructor
     def __init__(self,
-                 config: ConfigurableObject) -> None:
+                 config: ConfigObject) -> None:
         self.config = config
 
     # Parse message
     def Parse(self,
               message: pyrogram.types.Message) -> str:
         if message.text is None:
             raise PeriodicMsgParserInvalidError()
```

### Comparing `telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/periodic_msg/periodic_msg_scheduler.py` & `telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/periodic_msg/periodic_msg_scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 # Imports
 #
 from typing import Dict
 
 import pyrogram
 from apscheduler.schedulers.background import BackgroundScheduler
 
-from telegram_periodic_msg_bot.bot.bot_config import BotConfigTypes
-from telegram_periodic_msg_bot.config.configurable_object import ConfigurableObject
+from telegram_periodic_msg_bot.bot.bot_config_types import BotConfigTypes
+from telegram_periodic_msg_bot.config.config_object import ConfigObject
 from telegram_periodic_msg_bot.logger.logger import Logger
 from telegram_periodic_msg_bot.misc.helpers import ChatHelper
 from telegram_periodic_msg_bot.periodic_msg.periodic_msg_job import PeriodicMsgJob, PeriodicMsgJobData
 from telegram_periodic_msg_bot.periodic_msg.periodic_msg_parser import PeriodicMsgParser
 from telegram_periodic_msg_bot.translator.translation_loader import TranslationLoader
 from telegram_periodic_msg_bot.utils.wrapped_list import WrappedList
 
@@ -105,24 +105,24 @@
         return self.ToString()
 
 
 # Periodic message scheduler class
 class PeriodicMsgScheduler:
 
     client: pyrogram.Client
-    config: ConfigurableObject
+    config: ConfigObject
     logger: Logger
     translator: TranslationLoader
     jobs: Dict[int, Dict[str, PeriodicMsgJob]]
     scheduler: BackgroundScheduler
 
     # Constructor
     def __init__(self,
                  client: pyrogram.Client,
-                 config: ConfigurableObject,
+                 config: ConfigObject,
                  logger: Logger,
                  translator: TranslationLoader) -> None:
         self.client = client
         self.config = config
         self.logger = logger
         self.translator = translator
         self.jobs = {}
```

### Comparing `telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/periodic_msg/periodic_msg_sender.py` & `telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/periodic_msg/periodic_msg_sender.py`

 * *Files identical despite different names*

### Comparing `telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/periodic_msg_bot.py` & `telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/periodic_msg_bot.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
 #
 # Imports
 #
 from telegram_periodic_msg_bot.bot.bot_base import BotBase
-from telegram_periodic_msg_bot.bot.bot_config_cfg import BotConfigCfg
-from telegram_periodic_msg_bot.bot.bot_handlers_cfg import BotHandlersCfg
+from telegram_periodic_msg_bot.bot.bot_config import BotConfig
+from telegram_periodic_msg_bot.bot.bot_handlers_config import BotHandlersConfig
 from telegram_periodic_msg_bot.periodic_msg.periodic_msg_scheduler import PeriodicMsgScheduler
 
 
 #
 # Classes
 #
 
@@ -35,15 +35,19 @@
 class PeriodicMsgBot(BotBase):
 
     periodic_msg_scheduler: PeriodicMsgScheduler
 
     # Constructor
     def __init__(self,
                  config_file: str) -> None:
-        super().__init__(config_file,
-                         BotConfigCfg,
-                         BotHandlersCfg)
+        super().__init__(
+            config_file,
+            BotConfig,
+            BotHandlersConfig
+        )
         # Initialize periodic message scheduler
-        self.periodic_msg_scheduler = PeriodicMsgScheduler(self.client,
-                                                           self.config,
-                                                           self.logger,
-                                                           self.translator)
+        self.periodic_msg_scheduler = PeriodicMsgScheduler(
+            self.client,
+            self.config,
+            self.logger,
+            self.translator
+        )
```

### Comparing `telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/translator/translation_loader.py` & `telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/translator/translation_loader.py`

 * *Files identical despite different names*

### Comparing `telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/utils/key_value_converter.py` & `telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/utils/key_value_converter.py`

 * *Files identical despite different names*

### Comparing `telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/utils/pyrogram_wrapper.py` & `telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/utils/pyrogram_wrapper.py`

 * *Files identical despite different names*

### Comparing `telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/utils/utils.py` & `telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/utils/utils.py`

 * *Files identical despite different names*

### Comparing `telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot/utils/wrapped_list.py` & `telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot/utils/wrapped_list.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
-import typing
-
 #
 # Imports
 #
+import typing
+
 from abc import ABC
 from typing import Iterator, List
 
 
 #
 # Classes
 #
```

### Comparing `telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot.egg-info/PKG-INFO` & `telegram_periodic_msg_bot-0.3.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,7 @@
-Metadata-Version: 2.1
-Name: telegram-periodic-msg-bot
-Version: 0.3.1
-Summary: Telegram bot for sending periodic messages
-Home-page: https://github.com/ebellocchia/telegram_periodic_msg_bot
-Download-URL: https://github.com/ebellocchia/telegram_periodic_msg_bot/archive/v0.3.1.tar.gz
-Author: Emanuele Bellocchia
-Author-email: ebellocchia@gmail.com
-Maintainer: Emanuele Bellocchia
-Maintainer-email: ebellocchia@gmail.com
-License: MIT
-Keywords: telegram,bot,telegram bot,periodic messages
-Platform: any
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Telegram Periodic Message Bot
 
 [![PyPI version](https://badge.fury.io/py/telegram-periodic-msg-bot.svg)](https://badge.fury.io/py/telegram-periodic-msg-bot)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/d1cc7c1692de4939a23e626981923e83)](https://www.codacy.com/gh/ebellocchia/telegram_periodic_msg_bot/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=ebellocchia/telegram_periodic_msg_bot&amp;utm_campaign=Badge_Grade)
 [![CodeFactor](https://www.codefactor.io/repository/github/ebellocchia/telegram_periodic_msg_bot/badge)](https://www.codefactor.io/repository/github/ebellocchia/telegram_periodic_msg_bot)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://raw.githubusercontent.com/ebellocchia/bip_utils/master/LICENSE)
 
@@ -69,67 +44,74 @@
 
 An example of configuration file is provided in the *app/conf* folder.\
 The list of all possible fields that can be set is shown below.
 
 |Name|Description|
 |---|---|
 |**[pyrogram]**|Configuration for pyrogram|
-|session_name|Session name of your choice|
-|api_id|API ID from [https://my.telegram.org/apps](https://my.telegram.org/apps)|
-|api_hash|API hash from [https://my.telegram.org/apps](https://my.telegram.org/apps)|
-|bot_token|Bot token from BotFather|
+|`session_name`|Session name of your choice|
+|`api_id`|API ID from [https://my.telegram.org/apps](https://my.telegram.org/apps)|
+|`api_hash`|API hash from [https://my.telegram.org/apps](https://my.telegram.org/apps)|
+|`bot_token`|Bot token from BotFather|
 |**[app]**|Configuration for app|
-|app_is_test_mode|True to activate test mode false otherwise|
-|app_lang_file|Language file in XML format (default: English)|
+|`app_is_test_mode`|True to activate test mode false otherwise|
+|`app_lang_file`|Language file in XML format (default: English)|
 |**[task]**|Configuration for tasks|
-|tasks_max_num|Maximum number of running tasks (totally, in all groups). Default: 20.|
+|`tasks_max_num`|Maximum number of running tasks (totally, in all groups). Default: 20.|
 |**[message]**|Configuration for message|
-|message_max_len|Maximum message length in characters. Default: 4000.|
+|`message_max_len`|Maximum message length in characters. Default: 4000.|
 |**[logging]**|Configuration for logging|
-|log_level|Log level, same of python logging (*DEBUG*, *INFO*, *WARNING*, *ERROR*, *CRITICAL*). Default: *INFO*.|
-|log_console_enabled|True to enable logging to console, false otherwise (default: true)|
-|log_file_enabled|True to enable logging to file, false otherwise (default: false). If false, all the next fields will be skipped.|
-|log_file_name|Log file name|
-|log_file_use_rotating|True for using a rotating log file, false otherwise|
-|log_file_max_bytes|Maximum size in bytes for a log file. When reached, a new log file is created up to *log_file_backup_cnt*.. Valid only if log_file_use_rotating is true.|
-|log_file_backup_cnt|Maximum number of log files. Valid only if log_file_use_rotating is true.|
-|log_file_append|True to append to log file, false to start from a new file each time. Valid only if log_file_use_rotating is false.|
+|`log_level`|Log level, same of python logging (`DEBUG`, `INFO`, `WARNING`, `ERROR`, `CRITICAL`). Default: `INFO`.|
+|`log_console_enabled`|True to enable logging to console, false otherwise (default: `true`)|
+|`log_file_enabled`|True to enable logging to file, false otherwise (default: `false`). If false, all the next fields will be skipped.|
+|`log_file_name`|Log file name|
+|`log_file_use_rotating`|True for using a rotating log file, false otherwise|
+|`log_file_max_bytes`|Maximum size in bytes for a log file. When reached, a new log file is created up to `log_file_backup_cnt`. Valid only if `log_file_use_rotating` is true.|
+|`log_file_backup_cnt`|Maximum number of log files. Valid only if `log_file_use_rotating` is true.|
+|`log_file_append`|True to append to log file, false to start from a new file each time. Valid only if `log_file_use_rotating` is false.|
 
 ## Supported Commands
 
 List of supported commands:
-- **/help**: show this message
-- **/alive**: show if bot is active
-- **/msgbot_set_test_mode true/false**: enable/disable test mode
-- **/msgbot_is_test_mode**: show if test mode is enabled
-- **/msgbot_version**: show bot version
-- **/msgbot_task_start *MSG_ID PERIOD_HOURS [START_HOUR] MSG***: start a message task in the current chat. If the task *MSG_ID* already exists in the current chat, an error message will be shown. To start it again, it shall be stopped with the *msgbot_task_stop* command.
-    - *MSG_ID*: Message ID
-    - *PERIOD_HOURS*: Task period in hours, it shall be between 1 and 24
-    - *START_HOUR* (optional): Task start hour, it shall be between 0 and 23. Default value: 0.
-    - *MSG*: Message to be sent periodically, it shall be on a new line
-- **/msgbot_task_stop *MSG_ID***: stop the specified message task in the current chat. If the task *MSG_ID* does not exist in the current chat, an error message will be shown.
-    - *MSG_ID*: CoinGecko *ID*
-- **/msgbot_task_stop_all**: stop all message tasks in the current chat
-- **/msgbot_task_pause *MSG_ID***: pause the specified message task in the current chat. If the task *MSG_ID* does not exist in the current chat, an error message will be shown.
-    - *MSG_ID*: Message ID
-- **/msgbot_task_resume *MSG_ID***: resume the specified message task in the current chat. If the task *MSG_ID* does not exist in the current chat, an error message will be shown.
-    - *MSG_ID*: Message ID
-- **/msgbot_task_get *MSG_ID***: show the message set for the specified message task in the current chat.
-    - *MSG_ID*: Message ID
-- **/msgbot_task_set *MSG_ID MSG***: set the message of the specified message task in the current chat
-    - *MSG_ID*: Message ID
-    - *MSG*: Message to be sent periodically, it shall be on a new line
-- **/msgbot_task_delete_last_msg *MSG_ID true/false***: enable/disable the deletion of last messages for the specified message task in the current chat. If the task *MSG_ID* does not exist in the current chat, an error message will be shown.
-    - *MSG_ID*: Message ID
-    - *flag*: true or false
-- **/msgbot_task_info**: show the list of active message tasks in the current chat
+- `help`: show this message
+- `alive`: show if bot is active
+- `msgbot_set_test_mode true/false`: enable/disable test mode
+- `msgbot_is_test_mode`: show if test mode is enabled
+- `msgbot_version`: show bot version
+- `msgbot_task_start MSG_ID PERIOD_HOURS [START_HOUR] MSG`: start a message task in the current chat. If the task `MSG_ID` already exists in the current chat, an error message will be shown. To start it again, it shall be stopped with the `msgbot_task_stop` command.\
+Parameters:
+    - `MSG_ID`: Message ID
+    - `PERIOD_HOURS`: Task period in hours, it shall be between 1 and 24
+    - `START_HOUR` (optional): Task start hour, it shall be between 0 and 23. Default value: 0.
+    - `MSG`: Message to be sent periodically, it shall be on a new line
+- `msgbot_task_stop MSG_ID`: stop the specified message task in the current chat. If the task `MSG_ID` does not exist in the current chat, an error message will be shown.\
+Parameters:
+    - `MSG_ID`: CoinGecko *ID*
+- `msgbot_task_stop_all`: stop all message tasks in the current chat
+- `msgbot_task_pause MSG_ID`: pause the specified message task in the current chat. If the task `MSG_ID` does not exist in the current chat, an error message will be shown.\
+Parameters:
+    - `MSG_ID`: Message ID
+- `msgbot_task_resume MSG_ID`: resume the specified message task in the current chat. If the task `MSG_ID` does not exist in the current chat, an error message will be shown.\
+Parameters:
+    - `MSG_ID`: Message ID
+- `msgbot_task_get MSG_ID`: show the message set for the specified message task in the current chat.\
+Parameters:
+    - `MSG_ID`: Message ID
+- `msgbot_task_set MSG_ID MSG`: set the message of the specified message task in the current chat.\
+Parameters:
+    - `MSG_ID`: Message ID
+    - `MSG`: Message to be sent periodically, it shall be on a new line
+- `msgbot_task_delete_last_msg MSG_ID true/false`: enable/disable the deletion of last messages for the specified message task in the current chat. If the task `MSG_ID` does not exist in the current chat, an error message will be shown.\
+Parameters:
+    - `MSG_ID`: Message ID
+    - `flag`: true or false
+- `msgbot_task_info`: show the list of active message tasks in the current chat
 
 Messages can contain HTML tags if needed (e.g. for bold/italic text), while Markdown tags are not supported.\
-By default, a message task will delete the last sent message when sending a new one. This can be enabled/disabled with the *msgbot_task_delete_last_msg* command.
+By default, a message task will delete the last sent message when sending a new one. This can be enabled/disabled with the `msgbot_task_delete_last_msg` command.
 
 The task period starts from the specified starting hour (be sure to set the correct time on the VPS), for example:
 - A task period of 8 hours starting from 00:00 will send the message at: 00:00, 08:00 and 16:00
 - A task period of 6 hours starting from 08:00 will send the message at: 08:00, 14:00, 20:00 and 02:00
 
 **Examples**
 
@@ -174,13 +156,13 @@
 ## Test Mode
 
 During test mode, the bot will work as usual but the task period will be applied in minutes instead of hours. This allows to quickly check if it is working.
 
 ## Translation
 
 The messages sent by the bot on Telegram can be translated into different languages (the default language is English) by providing a custom XML file.\
-The XML file path is specified in the configuration file (*app_lang_file* field).\
+The XML file path is specified in the configuration file (`app_lang_file` field).\
 An example XML file in italian is provided in the folder *app/lang*.
 
 # License
 
 This software is available under the MIT license.
```

### Comparing `telegram_periodic_msg_bot-0.3.1/telegram_periodic_msg_bot.egg-info/SOURCES.txt` & `telegram_periodic_msg_bot-0.3.2/telegram_periodic_msg_bot.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -11,24 +11,29 @@
 telegram_periodic_msg_bot.egg-info/SOURCES.txt
 telegram_periodic_msg_bot.egg-info/dependency_links.txt
 telegram_periodic_msg_bot.egg-info/requires.txt
 telegram_periodic_msg_bot.egg-info/top_level.txt
 telegram_periodic_msg_bot/bot/__init__.py
 telegram_periodic_msg_bot/bot/bot_base.py
 telegram_periodic_msg_bot/bot/bot_config.py
-telegram_periodic_msg_bot/bot/bot_config_cfg.py
-telegram_periodic_msg_bot/bot/bot_handlers_cfg.py
+telegram_periodic_msg_bot/bot/bot_config_types.py
+telegram_periodic_msg_bot/bot/bot_handlers_config.py
+telegram_periodic_msg_bot/bot/bot_handlers_config_typing.py
 telegram_periodic_msg_bot/command/__init__.py
 telegram_periodic_msg_bot/command/command_base.py
 telegram_periodic_msg_bot/command/command_data.py
 telegram_periodic_msg_bot/command/command_dispatcher.py
 telegram_periodic_msg_bot/command/commands.py
 telegram_periodic_msg_bot/config/__init__.py
-telegram_periodic_msg_bot/config/config_loader.py
-telegram_periodic_msg_bot/config/configurable_object.py
+telegram_periodic_msg_bot/config/config_file_sections_loader.py
+telegram_periodic_msg_bot/config/config_loader_ex.py
+telegram_periodic_msg_bot/config/config_object.py
+telegram_periodic_msg_bot/config/config_section_loader.py
+telegram_periodic_msg_bot/config/config_sections_loader.py
+telegram_periodic_msg_bot/config/config_typing.py
 telegram_periodic_msg_bot/lang/lang_en.xml
 telegram_periodic_msg_bot/logger/__init__.py
 telegram_periodic_msg_bot/logger/logger.py
 telegram_periodic_msg_bot/message/__init__.py
 telegram_periodic_msg_bot/message/message_deleter.py
 telegram_periodic_msg_bot/message/message_dispatcher.py
 telegram_periodic_msg_bot/message/message_sender.py
```

