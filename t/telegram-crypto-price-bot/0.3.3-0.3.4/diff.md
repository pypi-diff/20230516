# Comparing `tmp/telegram_crypto_price_bot-0.3.3.tar.gz` & `tmp/telegram_crypto_price_bot-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegram_crypto_price_bot-0.3.3.tar", last modified: Fri Dec 16 12:22:55 2022, max compression
+gzip compressed data, was "telegram_crypto_price_bot-0.3.4.tar", last modified: Tue May 16 21:50:44 2023, max compression
```

## Comparing `telegram_crypto_price_bot-0.3.3.tar` & `telegram_crypto_price_bot-0.3.4.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxrwxrwx   0        0        0        0 2022-12-16 12:22:55.220534 telegram_crypto_price_bot-0.3.3/
--rw-rw-rw-   0        0        0     1085 2021-06-09 13:22:24.000000 telegram_crypto_price_bot-0.3.3/LICENSE
--rw-rw-rw-   0        0        0       26 2021-10-20 11:44:31.000000 telegram_crypto_price_bot-0.3.3/MANIFEST.in
--rw-rw-rw-   0        0        0    12799 2022-12-16 12:22:55.220534 telegram_crypto_price_bot-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0    11742 2022-09-29 12:35:36.000000 telegram_crypto_price_bot-0.3.3/README.md
--rw-rw-rw-   0        0        0       77 2022-10-07 12:38:47.000000 telegram_crypto_price_bot-0.3.3/requirements.txt
--rw-rw-rw-   0        0        0      111 2022-12-16 12:22:55.223544 telegram_crypto_price_bot-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0     2268 2021-10-20 12:15:01.000000 telegram_crypto_price_bot-0.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2022-12-16 12:22:54.964661 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/
--rw-rw-rw-   0        0        0      135 2021-09-17 22:04:56.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/__init__.py
--rw-rw-rw-   0        0        0       28 2022-12-16 12:21:38.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/_version.py
-drwxrwxrwx   0        0        0        0 2022-12-16 12:22:55.016244 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/bot/
--rw-rw-rw-   0        0        0        0 2021-12-09 22:03:30.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/bot/__init__.py
--rw-rw-rw-   0        0        0     5127 2022-11-14 20:26:36.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/bot/bot_base.py
--rw-rw-rw-   0        0        0    10275 2022-11-14 20:09:37.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/bot/bot_config.py
--rw-rw-rw-   0        0        0     2372 2022-11-14 20:08:09.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/bot/bot_config_types.py
--rw-rw-rw-   0        0        0     9581 2022-11-14 20:24:26.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/bot/bot_handlers_config.py
--rw-rw-rw-   0        0        0     1516 2022-11-14 20:21:22.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/bot/bot_handlers_config_typing.py
-drwxrwxrwx   0        0        0        0 2022-12-16 12:22:55.028743 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/chart_info/
--rw-rw-rw-   0        0        0        0 2021-12-09 22:03:30.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/chart_info/__init__.py
--rw-rw-rw-   0        0        0     2292 2022-09-27 21:57:11.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/chart_info/chart_info.py
--rw-rw-rw-   0        0        0     8679 2022-11-14 20:09:37.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/chart_info/chart_info_file_saver.py
-drwxrwxrwx   0        0        0        0 2022-12-16 12:22:55.039261 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/coin_info/
--rw-rw-rw-   0        0        0        0 2021-11-30 15:43:37.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/coin_info/__init__.py
--rw-rw-rw-   0        0        0     4486 2022-09-28 09:30:57.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/coin_info/coin_info_job.py
--rw-rw-rw-   0        0        0    15092 2022-11-14 20:09:37.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/coin_info/coin_info_scheduler.py
-drwxrwxrwx   0        0        0        0 2022-12-16 12:22:55.045776 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/coingecko/
--rw-rw-rw-   0        0        0        0 2021-11-30 15:43:37.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/coingecko/__init__.py
--rw-rw-rw-   0        0        0     2409 2022-09-27 21:57:11.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/coingecko/coingecko_price_api.py
-drwxrwxrwx   0        0        0        0 2022-12-16 12:22:55.067809 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/command/
--rw-rw-rw-   0        0        0        0 2021-11-30 15:43:37.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/command/__init__.py
--rw-rw-rw-   0        0        0     5524 2022-10-07 12:42:45.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/command/command_base.py
--rw-rw-rw-   0        0        0     4060 2022-09-28 07:54:31.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/command/command_data.py
--rw-rw-rw-   0        0        0     4913 2022-09-28 09:30:56.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/command/command_dispatcher.py
--rw-rw-rw-   0        0        0    14950 2022-11-14 20:09:37.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/command/commands.py
-drwxrwxrwx   0        0        0        0 2022-12-16 12:22:55.103354 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/config/
--rw-rw-rw-   0        0        0        0 2021-11-21 22:10:52.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/config/__init__.py
--rw-rw-rw-   0        0        0     1923 2022-11-14 20:01:32.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/config/config_file_sections_loader.py
--rw-rw-rw-   0        0        0     1339 2022-11-14 19:43:03.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/config/config_loader_ex.py
--rw-rw-rw-   0        0        0     2201 2022-11-14 20:50:16.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/config/config_object.py
--rw-rw-rw-   0        0        0     4105 2022-11-14 20:01:42.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/config/config_section_loader.py
--rw-rw-rw-   0        0        0     2190 2022-11-14 20:01:48.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/config/config_sections_loader.py
--rw-rw-rw-   0        0        0     1319 2022-11-14 15:20:40.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/config/config_typing.py
-drwxrwxrwx   0        0        0        0 2022-12-16 12:22:55.130896 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/info_message_sender/
--rw-rw-rw-   0        0        0        0 2021-12-09 22:03:30.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/info_message_sender/__init__.py
--rw-rw-rw-   0        0        0     3043 2022-09-28 09:30:57.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/info_message_sender/chart_info_message_sender.py
--rw-rw-rw-   0        0        0     3599 2022-12-15 22:12:19.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/info_message_sender/chart_price_info_message_sender.py
--rw-rw-rw-   0        0        0     4972 2022-11-14 20:09:37.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/info_message_sender/coin_info_message_sender.py
--rw-rw-rw-   0        0        0     3103 2022-09-27 21:57:11.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/info_message_sender/info_message_sender_base.py
--rw-rw-rw-   0        0        0     2580 2022-09-28 09:30:56.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/info_message_sender/price_info_message_sender.py
-drwxrwxrwx   0        0        0        0 2022-12-16 12:22:55.133893 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/lang/
--rw-rw-rw-   0        0        0     6848 2022-12-15 22:16:07.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/lang/lang_en.xml
-drwxrwxrwx   0        0        0        0 2022-12-16 12:22:55.141410 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/logger/
--rw-rw-rw-   0        0        0        0 2021-12-09 22:03:30.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/logger/__init__.py
--rw-rw-rw-   0        0        0     4670 2022-11-14 20:09:37.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/logger/logger.py
-drwxrwxrwx   0        0        0        0 2022-12-16 12:22:55.158447 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/message/
--rw-rw-rw-   0        0        0        0 2021-12-09 22:03:30.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/message/__init__.py
--rw-rw-rw-   0        0        0     2388 2022-09-27 21:57:11.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/message/message_deleter.py
--rw-rw-rw-   0        0        0     4643 2022-09-28 09:30:56.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/message/message_dispatcher.py
--rw-rw-rw-   0        0        0     4081 2022-12-15 22:09:31.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/message/message_sender.py
-drwxrwxrwx   0        0        0        0 2022-12-16 12:22:55.175959 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/misc/
--rw-rw-rw-   0        0        0        0 2021-12-09 22:03:30.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/misc/__init__.py
--rw-rw-rw-   0        0        0     4270 2022-11-22 15:42:50.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/misc/chat_members.py
--rw-rw-rw-   0        0        0     3713 2022-09-27 21:57:11.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/misc/formatters.py
--rw-rw-rw-   0        0        0     2933 2022-09-28 08:57:50.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/misc/helpers.py
--rw-rw-rw-   0        0        0     1916 2022-11-14 20:26:24.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/price_bot.py
-drwxrwxrwx   0        0        0        0 2022-12-16 12:22:55.187472 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/price_info/
--rw-rw-rw-   0        0        0        0 2021-12-09 22:03:30.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/price_info/__init__.py
--rw-rw-rw-   0        0        0     3854 2022-09-27 21:57:11.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/price_info/price_info.py
--rw-rw-rw-   0        0        0     5444 2022-12-15 22:15:08.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/price_info/price_info_builder.py
-drwxrwxrwx   0        0        0        0 2022-12-16 12:22:55.195992 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/translation/
--rw-rw-rw-   0        0        0        0 2021-12-09 22:03:30.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/translation/__init__.py
--rw-rw-rw-   0        0        0     3708 2022-09-27 21:57:11.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/translation/translation_loader.py
-drwxrwxrwx   0        0        0        0 2022-12-16 12:22:55.217026 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/utils/
--rw-rw-rw-   0        0        0        0 2021-12-09 22:03:30.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/utils/__init__.py
--rw-rw-rw-   0        0        0     3343 2022-09-28 07:55:19.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/utils/pyrogram_wrapper.py
--rw-rw-rw-   0        0        0     2367 2022-12-15 21:33:21.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/utils/utils.py
--rw-rw-rw-   0        0        0     2576 2022-09-27 21:57:11.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/utils/wrapped_list.py
-drwxrwxrwx   0        0        0        0 2022-12-16 12:22:54.985688 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot.egg-info/
--rw-rw-rw-   0        0        0    12799 2022-12-16 12:22:54.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3177 2022-12-16 12:22:54.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-16 12:22:54.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2022-12-16 12:22:54.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2022-12-16 12:22:54.000000 telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 21:50:44.465541 telegram_crypto_price_bot-0.3.4/
+-rw-rw-rw-   0        0        0     1085 2021-06-09 13:22:24.000000 telegram_crypto_price_bot-0.3.4/LICENSE
+-rw-rw-rw-   0        0        0       26 2021-10-20 11:44:31.000000 telegram_crypto_price_bot-0.3.4/MANIFEST.in
+-rw-rw-rw-   0        0        0    12851 2023-05-16 21:50:44.465541 telegram_crypto_price_bot-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0    11742 2022-09-29 12:35:36.000000 telegram_crypto_price_bot-0.3.4/README.md
+-rw-rw-rw-   0        0        0       77 2022-10-07 12:38:47.000000 telegram_crypto_price_bot-0.3.4/requirements.txt
+-rw-rw-rw-   0        0        0      111 2023-05-16 21:50:44.471576 telegram_crypto_price_bot-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     2319 2023-05-07 20:48:25.000000 telegram_crypto_price_bot-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:50:44.133708 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/
+-rw-rw-rw-   0        0        0      135 2021-09-17 22:04:56.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/__init__.py
+-rw-rw-rw-   0        0        0       28 2023-05-16 21:03:30.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/_version.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:50:44.187154 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/bot/
+-rw-rw-rw-   0        0        0        0 2021-12-09 22:03:30.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/bot/__init__.py
+-rw-rw-rw-   0        0        0     5127 2022-11-14 20:26:36.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/bot/bot_base.py
+-rw-rw-rw-   0        0        0    10275 2022-11-14 20:09:37.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/bot/bot_config.py
+-rw-rw-rw-   0        0        0     2372 2022-11-14 20:08:09.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/bot/bot_config_types.py
+-rw-rw-rw-   0        0        0     9581 2022-11-14 20:24:26.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/bot/bot_handlers_config.py
+-rw-rw-rw-   0        0        0     1516 2022-11-14 20:21:22.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/bot/bot_handlers_config_typing.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:50:44.206075 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/chart_info/
+-rw-rw-rw-   0        0        0        0 2021-12-09 22:03:30.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/chart_info/__init__.py
+-rw-rw-rw-   0        0        0     2292 2022-09-27 21:57:11.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/chart_info/chart_info.py
+-rw-rw-rw-   0        0        0     8679 2022-11-14 20:09:37.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/chart_info/chart_info_file_saver.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:50:44.222305 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/coin_info/
+-rw-rw-rw-   0        0        0        0 2021-11-30 15:43:37.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/coin_info/__init__.py
+-rw-rw-rw-   0        0        0     4486 2022-09-28 09:30:57.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/coin_info/coin_info_job.py
+-rw-rw-rw-   0        0        0    15092 2022-11-14 20:09:37.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/coin_info/coin_info_scheduler.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:50:44.230810 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/coingecko/
+-rw-rw-rw-   0        0        0        0 2021-11-30 15:43:37.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/coingecko/__init__.py
+-rw-rw-rw-   0        0        0     2409 2022-09-27 21:57:11.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/coingecko/coingecko_price_api.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:50:44.252339 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/command/
+-rw-rw-rw-   0        0        0        0 2021-11-30 15:43:37.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/command/__init__.py
+-rw-rw-rw-   0        0        0     5675 2023-05-16 21:02:38.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/command/command_base.py
+-rw-rw-rw-   0        0        0     4060 2022-09-28 07:54:31.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/command/command_data.py
+-rw-rw-rw-   0        0        0     4913 2022-09-28 09:30:56.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/command/command_dispatcher.py
+-rw-rw-rw-   0        0        0    14950 2022-11-14 20:09:37.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/command/commands.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:50:44.304180 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/config/
+-rw-rw-rw-   0        0        0        0 2021-11-21 22:10:52.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/config/__init__.py
+-rw-rw-rw-   0        0        0     1923 2022-11-14 20:01:32.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/config/config_file_sections_loader.py
+-rw-rw-rw-   0        0        0     1339 2022-11-14 19:43:03.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/config/config_loader_ex.py
+-rw-rw-rw-   0        0        0     2201 2022-11-14 20:50:16.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/config/config_object.py
+-rw-rw-rw-   0        0        0     4105 2022-11-14 20:01:42.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/config/config_section_loader.py
+-rw-rw-rw-   0        0        0     2190 2022-11-14 20:01:48.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/config/config_sections_loader.py
+-rw-rw-rw-   0        0        0     1319 2022-11-14 15:20:40.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/config/config_typing.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:50:44.343517 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/info_message_sender/
+-rw-rw-rw-   0        0        0        0 2021-12-09 22:03:30.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/info_message_sender/__init__.py
+-rw-rw-rw-   0        0        0     3043 2022-09-28 09:30:57.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/info_message_sender/chart_info_message_sender.py
+-rw-rw-rw-   0        0        0     3599 2022-12-15 22:12:19.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/info_message_sender/chart_price_info_message_sender.py
+-rw-rw-rw-   0        0        0     4972 2022-11-14 20:09:37.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/info_message_sender/coin_info_message_sender.py
+-rw-rw-rw-   0        0        0     3103 2022-09-27 21:57:11.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/info_message_sender/info_message_sender_base.py
+-rw-rw-rw-   0        0        0     2580 2022-09-28 09:30:56.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/info_message_sender/price_info_message_sender.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:50:44.349518 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/lang/
+-rw-rw-rw-   0        0        0     6848 2022-12-15 22:16:07.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/lang/lang_en.xml
+drwxrwxrwx   0        0        0        0 2023-05-16 21:50:44.357584 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/logger/
+-rw-rw-rw-   0        0        0        0 2021-12-09 22:03:30.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/logger/__init__.py
+-rw-rw-rw-   0        0        0     4670 2022-11-14 20:09:37.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/logger/logger.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:50:44.385176 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/message/
+-rw-rw-rw-   0        0        0        0 2021-12-09 22:03:30.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/message/__init__.py
+-rw-rw-rw-   0        0        0     2388 2022-09-27 21:57:11.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/message/message_deleter.py
+-rw-rw-rw-   0        0        0     4643 2022-09-28 09:30:56.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/message/message_dispatcher.py
+-rw-rw-rw-   0        0        0     4081 2022-12-15 22:09:31.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/message/message_sender.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:50:44.414663 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/misc/
+-rw-rw-rw-   0        0        0        0 2021-12-09 22:03:30.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/misc/__init__.py
+-rw-rw-rw-   0        0        0     4270 2022-11-22 15:42:50.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/misc/chat_members.py
+-rw-rw-rw-   0        0        0     3713 2022-09-27 21:57:11.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/misc/formatters.py
+-rw-rw-rw-   0        0        0     2933 2022-09-28 08:57:50.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/misc/helpers.py
+-rw-rw-rw-   0        0        0     1916 2022-11-14 20:26:24.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/price_bot.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:50:44.430688 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/price_info/
+-rw-rw-rw-   0        0        0        0 2021-12-09 22:03:30.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/price_info/__init__.py
+-rw-rw-rw-   0        0        0     3854 2022-09-27 21:57:11.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/price_info/price_info.py
+-rw-rw-rw-   0        0        0     5444 2022-12-15 22:15:08.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/price_info/price_info_builder.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:50:44.438822 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/translation/
+-rw-rw-rw-   0        0        0        0 2021-12-09 22:03:30.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/translation/__init__.py
+-rw-rw-rw-   0        0        0     3708 2022-09-27 21:57:11.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/translation/translation_loader.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:50:44.460447 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/utils/
+-rw-rw-rw-   0        0        0        0 2021-12-09 22:03:30.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/utils/__init__.py
+-rw-rw-rw-   0        0        0     3343 2022-09-28 07:55:19.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/utils/pyrogram_wrapper.py
+-rw-rw-rw-   0        0        0     2367 2022-12-15 21:33:21.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/utils/utils.py
+-rw-rw-rw-   0        0        0     2576 2023-05-06 12:58:13.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/utils/wrapped_list.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:50:44.150823 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot.egg-info/
+-rw-rw-rw-   0        0        0    12851 2023-05-16 21:50:43.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3177 2023-05-16 21:50:43.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 21:50:43.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2023-05-16 21:50:43.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-05-16 21:50:43.000000 telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot.egg-info/top_level.txt
```

### Comparing `telegram_crypto_price_bot-0.3.3/LICENSE` & `telegram_crypto_price_bot-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `telegram_crypto_price_bot-0.3.3/PKG-INFO` & `telegram_crypto_price_bot-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: telegram_crypto_price_bot
-Version: 0.3.3
+Version: 0.3.4
 Summary: Telegram bot for displaying cryptocurrencies price
 Home-page: https://github.com/ebellocchia/telegram_crypto_price_bot
-Download-URL: https://github.com/ebellocchia/telegram_crypto_price_bot/archive/v0.3.3.tar.gz
+Download-URL: https://github.com/ebellocchia/telegram_crypto_price_bot/archive/v0.3.4.tar.gz
 Author: Emanuele Bellocchia
 Author-email: ebellocchia@gmail.com
 Maintainer: Emanuele Bellocchia
 Maintainer-email: ebellocchia@gmail.com
 License: MIT
 Keywords: telegram,bot,telegram bot,crypto,crypto prices,cryptocurrency,cryptocurrency prices
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
```

### Comparing `telegram_crypto_price_bot-0.3.3/README.md` & `telegram_crypto_price_bot-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `telegram_crypto_price_bot-0.3.3/setup.py` & `telegram_crypto_price_bot-0.3.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     keywords="telegram, bot, telegram bot, crypto, crypto prices, cryptocurrency, cryptocurrency prices",
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

### Comparing `telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/bot/bot_base.py` & `telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/bot/bot_base.py`

 * *Files identical despite different names*

### Comparing `telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/bot/bot_config.py` & `telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/bot/bot_config.py`

 * *Files identical despite different names*

### Comparing `telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/bot/bot_config_types.py` & `telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/bot/bot_config_types.py`

 * *Files identical despite different names*

### Comparing `telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/bot/bot_handlers_config.py` & `telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/bot/bot_handlers_config.py`

 * *Files identical despite different names*

### Comparing `telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/bot/bot_handlers_config_typing.py` & `telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/bot/bot_handlers_config_typing.py`

 * *Files identical despite different names*

### Comparing `telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/chart_info/chart_info.py` & `telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/chart_info/chart_info.py`

 * *Files identical despite different names*

### Comparing `telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/chart_info/chart_info_file_saver.py` & `telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/chart_info/chart_info_file_saver.py`

 * *Files identical despite different names*

### Comparing `telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/coin_info/coin_info_job.py` & `telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/coin_info/coin_info_job.py`

 * *Files identical despite different names*

### Comparing `telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/coin_info/coin_info_scheduler.py` & `telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/coin_info/coin_info_scheduler.py`

 * *Files identical despite different names*

### Comparing `telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/coingecko/coingecko_price_api.py` & `telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/coingecko/coingecko_price_api.py`

 * *Files identical despite different names*

### Comparing `telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/command/command_base.py` & `telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/command/command_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -111,23 +111,27 @@
 
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
         if cmd_user is None:
```

### Comparing `telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/command/command_data.py` & `telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/command/command_data.py`

 * *Files identical despite different names*

### Comparing `telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/command/command_dispatcher.py` & `telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/command/command_dispatcher.py`

 * *Files identical despite different names*

### Comparing `telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/command/commands.py` & `telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/command/commands.py`

 * *Files identical despite different names*

### Comparing `telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/config/config_file_sections_loader.py` & `telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/config/config_file_sections_loader.py`

 * *Files identical despite different names*

### Comparing `telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/config/config_loader_ex.py` & `telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/config/config_loader_ex.py`

 * *Files identical despite different names*

### Comparing `telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/config/config_object.py` & `telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/config/config_object.py`

 * *Files identical despite different names*

### Comparing `telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/config/config_section_loader.py` & `telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/config/config_section_loader.py`

 * *Files identical despite different names*

### Comparing `telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/config/config_sections_loader.py` & `telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/config/config_sections_loader.py`

 * *Files identical despite different names*

### Comparing `telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/config/config_typing.py` & `telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/config/config_typing.py`

 * *Files identical despite different names*

### Comparing `telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/info_message_sender/chart_info_message_sender.py` & `telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/info_message_sender/chart_info_message_sender.py`

 * *Files identical despite different names*

### Comparing `telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/info_message_sender/chart_price_info_message_sender.py` & `telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/info_message_sender/chart_price_info_message_sender.py`

 * *Files identical despite different names*

### Comparing `telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/info_message_sender/coin_info_message_sender.py` & `telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/info_message_sender/coin_info_message_sender.py`

 * *Files identical despite different names*

### Comparing `telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/info_message_sender/info_message_sender_base.py` & `telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/info_message_sender/info_message_sender_base.py`

 * *Files identical despite different names*

### Comparing `telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/info_message_sender/price_info_message_sender.py` & `telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/info_message_sender/price_info_message_sender.py`

 * *Files identical despite different names*

### Comparing `telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/lang/lang_en.xml` & `telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/lang/lang_en.xml`

 * *Files identical despite different names*

### Comparing `telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/logger/logger.py` & `telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/logger/logger.py`

 * *Files identical despite different names*

### Comparing `telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/message/message_deleter.py` & `telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/message/message_deleter.py`

 * *Files identical despite different names*

### Comparing `telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/message/message_dispatcher.py` & `telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/message/message_dispatcher.py`

 * *Files identical despite different names*

### Comparing `telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/message/message_sender.py` & `telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/message/message_sender.py`

 * *Files identical despite different names*

### Comparing `telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/misc/chat_members.py` & `telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/misc/chat_members.py`

 * *Files identical despite different names*

### Comparing `telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/misc/formatters.py` & `telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/misc/formatters.py`

 * *Files identical despite different names*

### Comparing `telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/misc/helpers.py` & `telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/misc/helpers.py`

 * *Files identical despite different names*

### Comparing `telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/price_bot.py` & `telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/price_bot.py`

 * *Files identical despite different names*

### Comparing `telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/price_info/price_info.py` & `telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/price_info/price_info.py`

 * *Files identical despite different names*

### Comparing `telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/price_info/price_info_builder.py` & `telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/price_info/price_info_builder.py`

 * *Files identical despite different names*

### Comparing `telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/translation/translation_loader.py` & `telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/translation/translation_loader.py`

 * *Files identical despite different names*

### Comparing `telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/utils/pyrogram_wrapper.py` & `telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/utils/pyrogram_wrapper.py`

 * *Files identical despite different names*

### Comparing `telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/utils/utils.py` & `telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/utils/utils.py`

 * *Files identical despite different names*

### Comparing `telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot/utils/wrapped_list.py` & `telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot/utils/wrapped_list.py`

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

### Comparing `telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot.egg-info/PKG-INFO` & `telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: telegram-crypto-price-bot
-Version: 0.3.3
+Version: 0.3.4
 Summary: Telegram bot for displaying cryptocurrencies price
 Home-page: https://github.com/ebellocchia/telegram_crypto_price_bot
-Download-URL: https://github.com/ebellocchia/telegram_crypto_price_bot/archive/v0.3.3.tar.gz
+Download-URL: https://github.com/ebellocchia/telegram_crypto_price_bot/archive/v0.3.4.tar.gz
 Author: Emanuele Bellocchia
 Author-email: ebellocchia@gmail.com
 Maintainer: Emanuele Bellocchia
 Maintainer-email: ebellocchia@gmail.com
 License: MIT
 Keywords: telegram,bot,telegram bot,crypto,crypto prices,cryptocurrency,cryptocurrency prices
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
```

### Comparing `telegram_crypto_price_bot-0.3.3/telegram_crypto_price_bot.egg-info/SOURCES.txt` & `telegram_crypto_price_bot-0.3.4/telegram_crypto_price_bot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

