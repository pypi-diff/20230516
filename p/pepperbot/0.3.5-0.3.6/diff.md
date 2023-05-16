# Comparing `tmp/pepperbot-0.3.5.tar.gz` & `tmp/pepperbot-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepperbot-0.3.5.tar", last modified: Mon May  8 13:11:47 2023, max compression
+gzip compressed data, was "pepperbot-0.3.6.tar", last modified: Tue May 16 05:16:16 2023, max compression
```

## Comparing `pepperbot-0.3.5.tar` & `pepperbot-0.3.6.tar`

### file list

```diff
@@ -1,86 +1,89 @@
--rw-r--r--   0        0        0     1084 2021-03-30 09:01:51.964858 pepperbot-0.3.5/LICENSE
--rw-r--r--   0        0        0     4722 2023-05-08 13:06:57.517071 pepperbot-0.3.5/README.md
--rw-r--r--   0        0        0      273 2023-04-10 16:48:13.652944 pepperbot-0.3.5/cli/__init__.py
--rw-r--r--   0        0        0      631 2023-05-08 13:03:35.795139 pepperbot-0.3.5/pepperbot/__init__.py
--rw-r--r--   0        0        0     2819 2023-04-15 23:10:33.259712 pepperbot-0.3.5/pepperbot/adapters/keaimao/__init__.py
--rw-r--r--   0        0        0     5722 2023-04-20 11:08:26.809253 pepperbot-0.3.5/pepperbot/adapters/keaimao/api/__init__.py
--rw-r--r--   0        0        0     2636 2023-04-15 23:07:16.981274 pepperbot-0.3.5/pepperbot/adapters/keaimao/event/__init__.py
--rw-r--r--   0        0        0    21222 2022-04-13 12:45:33.068068 pepperbot-0.3.5/pepperbot/adapters/keaimao/event/records/EventFriendMsg.js
--rw-r--r--   0        0        0    10263 2022-02-20 09:58:20.299888 pepperbot-0.3.5/pepperbot/adapters/keaimao/event/records/EventGroupMessage.js
--rw-r--r--   0        0        0     6524 2023-04-16 02:25:50.305638 pepperbot-0.3.5/pepperbot/adapters/onebot/__init__.py
--rw-r--r--   0        0        0    25015 2023-05-08 12:20:06.549164 pepperbot-0.3.5/pepperbot/adapters/onebot/api/__init__.py
--rw-r--r--   0        0        0    11305 2023-04-20 11:07:29.210764 pepperbot-0.3.5/pepperbot/adapters/onebot/event/__init__.py
--rw-r--r--   0        0        0       67 2023-04-14 16:22:16.875389 pepperbot-0.3.5/pepperbot/adapters/onebot/models/__init__.py
--rw-r--r--   0        0        0      696 2023-04-14 16:01:58.086198 pepperbot-0.3.5/pepperbot/adapters/onebot/models/group.py
--rw-r--r--   0        0        0      572 2022-02-20 09:58:20.311051 pepperbot-0.3.5/pepperbot/adapters/onebot/models/message.py
--rw-r--r--   0        0        0     1395 2023-04-14 16:22:28.359913 pepperbot-0.3.5/pepperbot/adapters/onebot/models/user.py
--rw-r--r--   0        0        0     9174 2023-04-19 05:26:45.684428 pepperbot-0.3.5/pepperbot/adapters/telegram/__init__.py
--rw-r--r--   0        0        0     2931 2023-04-20 11:10:48.986337 pepperbot-0.3.5/pepperbot/adapters/telegram/api/__init__.py
--rw-r--r--   0        0        0     4663 2023-04-19 05:22:27.264737 pepperbot-0.3.5/pepperbot/adapters/telegram/event/__init__.py
--rw-r--r--   0        0        0      900 2023-04-14 17:09:33.793304 pepperbot-0.3.5/pepperbot/adapters/universal/__init__.py
--rw-r--r--   0        0        0     2709 2023-04-20 11:10:48.986337 pepperbot-0.3.5/pepperbot/adapters/universal/api/__init__.py
--rw-r--r--   0        0        0     3245 2023-04-15 23:11:30.691877 pepperbot-0.3.5/pepperbot/adapters/universal/event/__init__.py
--rw-r--r--   0        0        0      766 2023-04-10 15:18:25.547755 pepperbot-0.3.5/pepperbot/config.py
--rw-r--r--   0        0        0        0 2022-02-20 09:58:20.315950 pepperbot-0.3.5/pepperbot/core/__init__.py
--rw-r--r--   0        0        0     2796 2023-04-14 15:03:07.150287 pepperbot-0.3.5/pepperbot/core/api/api_caller.py
--rw-r--r--   0        0        0      835 2022-02-20 09:58:20.317490 pepperbot-0.3.5/pepperbot/core/api/decorators.py
--rw-r--r--   0        0        0        0 2022-02-20 09:58:20.319000 pepperbot-0.3.5/pepperbot/core/event/__init__.py
--rw-r--r--   0        0        0     1514 2023-04-16 00:04:42.470521 pepperbot-0.3.5/pepperbot/core/event/base_adapter.py
--rw-r--r--   0        0        0    22212 2023-05-08 12:20:20.126205 pepperbot-0.3.5/pepperbot/core/event/handle.py
--rw-r--r--   0        0        0     1642 2023-04-19 05:27:57.642248 pepperbot-0.3.5/pepperbot/core/event/universal.py
--rw-r--r--   0        0        0     3020 2022-05-04 06:33:33.296283 pepperbot-0.3.5/pepperbot/core/event/utils.py
--rw-r--r--   0        0        0      931 2022-05-03 12:01:53.466811 pepperbot-0.3.5/pepperbot/core/message/base.py
--rw-r--r--   0        0        0    11258 2023-05-07 12:55:09.643864 pepperbot-0.3.5/pepperbot/core/message/chain.py
--rw-r--r--   0        0        0    16761 2023-05-07 08:29:43.324781 pepperbot-0.3.5/pepperbot/core/message/segment.py
--rw-r--r--   0        0        0       84 2023-04-22 12:37:07.245598 pepperbot-0.3.5/pepperbot/core/route/__init__.py
--rw-r--r--   0        0        0     5435 2023-05-08 12:03:14.378466 pepperbot-0.3.5/pepperbot/core/route/available/__init__.py
--rw-r--r--   0        0        0     1359 2023-04-22 15:10:40.463249 pepperbot-0.3.5/pepperbot/core/route/available/decorators.py
--rw-r--r--   0        0        0     4624 2023-05-08 12:21:33.482763 pepperbot-0.3.5/pepperbot/core/route/cache.py
--rw-r--r--   0        0        0      326 2022-02-20 09:58:20.368067 pepperbot-0.3.5/pepperbot/core/route/hook.py
--rw-r--r--   0        0        0     6520 2023-04-20 12:02:43.500740 pepperbot-0.3.5/pepperbot/core/route/parse.py
--rw-r--r--   0        0        0     1812 2023-05-08 12:21:46.168927 pepperbot-0.3.5/pepperbot/core/route/utils.py
--rw-r--r--   0        0        0    15411 2023-05-08 12:58:11.471224 pepperbot-0.3.5/pepperbot/core/route/validate.py
--rw-r--r--   0        0        0     1165 2023-04-20 10:22:17.059555 pepperbot-0.3.5/pepperbot/exceptions.py
--rw-r--r--   0        0        0        0 2022-02-20 09:58:20.371633 pepperbot-0.3.5/pepperbot/extensions/__init__.py
--rw-r--r--   0        0        0     2146 2022-07-12 14:55:41.437631 pepperbot-0.3.5/pepperbot/extensions/action/__init__.py
--rw-r--r--   0        0        0     1323 2022-02-20 09:58:20.372621 pepperbot-0.3.5/pepperbot/extensions/action/action.py
--rw-r--r--   0        0        0     9917 2022-02-20 09:58:20.372621 pepperbot-0.3.5/pepperbot/extensions/action/chain.py
--rw-r--r--   0        0        0     2813 2022-02-20 09:58:20.373773 pepperbot-0.3.5/pepperbot/extensions/action/decorators.py
--rw-r--r--   0        0        0     2413 2022-02-20 09:58:20.374299 pepperbot-0.3.5/pepperbot/extensions/action/runner.py
--rw-r--r--   0        0        0     5383 2023-05-08 12:38:58.821743 pepperbot-0.3.5/pepperbot/extensions/command/__init__.py
--rw-r--r--   0        0        0    29929 2023-05-08 12:41:31.503505 pepperbot-0.3.5/pepperbot/extensions/command/handle.py
--rw-r--r--   0        0        0     1377 2023-05-07 08:19:44.268892 pepperbot-0.3.5/pepperbot/extensions/command/node.py
--rw-r--r--   0        0        0      532 2023-05-07 08:20:17.196776 pepperbot-0.3.5/pepperbot/extensions/command/parser.py
--rw-r--r--   0        0        0    25012 2023-05-08 12:58:08.158417 pepperbot-0.3.5/pepperbot/extensions/command/pattern.py
--rw-r--r--   0        0        0     2491 2023-04-20 11:29:18.885191 pepperbot-0.3.5/pepperbot/extensions/command/sender.py
--rw-r--r--   0        0        0     7978 2023-05-07 13:22:49.683674 pepperbot-0.3.5/pepperbot/extensions/command/utils.py
--rw-r--r--   0        0        0     2093 2023-05-08 12:46:01.677718 pepperbot-0.3.5/pepperbot/extensions/log/__init__.py
--rw-r--r--   0        0        0      103 2023-04-07 14:00:53.161961 pepperbot-0.3.5/pepperbot/extensions/scheduler/__init__.py
--rw-r--r--   0        0        0     8449 2023-05-07 03:22:34.908784 pepperbot-0.3.5/pepperbot/initial.py
--rw-r--r--   0        0        0       79 2022-02-20 09:58:20.384843 pepperbot-0.3.5/pepperbot/store/__init__.py
--rw-r--r--   0        0        0     8636 2023-05-08 12:46:56.141148 pepperbot-0.3.5/pepperbot/store/command.py
--rw-r--r--   0        0        0     2421 2023-04-22 14:42:16.694644 pepperbot-0.3.5/pepperbot/store/event.py
--rw-r--r--   0        0        0    14722 2023-05-08 12:47:55.793372 pepperbot-0.3.5/pepperbot/store/meta.py
--rw-r--r--   0        0        0     2426 2023-04-12 14:36:34.483507 pepperbot-0.3.5/pepperbot/store/orm.py
--rw-r--r--   0        0        0     1750 2023-05-02 21:52:09.236997 pepperbot-0.3.5/pepperbot/types.py
--rw-r--r--   0        0        0        0 2021-05-20 10:22:56.350973 pepperbot-0.3.5/pepperbot/utils/__init__.py
--rw-r--r--   0        0        0     5637 2023-05-08 12:48:51.085527 pepperbot-0.3.5/pepperbot/utils/common.py
--rw-r--r--   0        0        0     1880 2023-05-08 13:11:47.810059 pepperbot-0.3.5/pyproject.toml
--rw-r--r--   0        0        0      144 2023-05-07 11:36:54.700923 pepperbot-0.3.5/tests/__init__.py
--rw-r--r--   0        0        0    12274 2023-05-08 12:43:16.485834 pepperbot-0.3.5/tests/command/test_cli_argument.py
--rw-r--r--   0        0        0     1499 2023-05-08 12:43:24.446692 pepperbot-0.3.5/tests/command/test_lifecycle.py
--rw-r--r--   0        0        0       87 2023-05-08 12:45:36.722837 pepperbot-0.3.5/tests/command/test_match.py
--rw-r--r--   0        0        0     5980 2023-05-07 12:54:47.433922 pepperbot-0.3.5/tests/command/test_merge.py
--rw-r--r--   0        0        0      400 2023-05-08 08:42:50.259215 pepperbot-0.3.5/tests/command/test_parameters.py
--rw-r--r--   0        0        0    15309 2023-05-08 12:45:06.857956 pepperbot-0.3.5/tests/command/test_sub_command.py
--rw-r--r--   0        0        0      619 2023-05-07 06:37:24.188198 pepperbot-0.3.5/tests/command/test_types.py
--rw-r--r--   0        0        0       28 2023-05-08 12:43:01.486316 pepperbot-0.3.5/tests/command/test_validate.py
--rw-r--r--   0        0        0     2481 2023-05-07 12:24:32.582530 pepperbot-0.3.5/tests/conftest.py
--rw-r--r--   0        0        0      867 2023-05-07 13:50:57.563104 pepperbot-0.3.5/tests/core/test_available.py
--rw-r--r--   0        0        0      214 2023-05-07 13:46:15.996945 pepperbot-0.3.5/tests/core/test_dispatch.py
--rw-r--r--   0        0        0        0 2023-05-07 09:54:19.845047 pepperbot-0.3.5/tests/core/test_route.py
--rw-r--r--   0        0        0     1818 2023-05-07 10:00:48.212139 pepperbot-0.3.5/tests/message/test_chain.py
--rw-r--r--   0        0        0       87 2023-05-07 09:56:20.249411 pepperbot-0.3.5/tests/message/test_segment.py
--rw-r--r--   0        0        0     2640 2021-05-20 11:42:38.152329 pepperbot-0.3.5/tests/tree.py
--rw-r--r--   0        0        0     1096 2023-05-08 07:29:48.570650 pepperbot-0.3.5/tests/utils.py
--rw-r--r--   0        0        0     5859 1970-01-01 00:00:00.000000 pepperbot-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1084 2021-03-30 09:01:51.964858 pepperbot-0.3.6/LICENSE
+-rw-r--r--   0        0        0     5077 2023-05-14 17:17:06.935125 pepperbot-0.3.6/README.md
+-rw-r--r--   0        0        0      273 2023-04-10 16:48:13.652944 pepperbot-0.3.6/cli/__init__.py
+-rw-r--r--   0        0        0      631 2023-05-08 13:03:35.795139 pepperbot-0.3.6/pepperbot/__init__.py
+-rw-r--r--   0        0        0     2825 2023-05-16 04:59:02.717759 pepperbot-0.3.6/pepperbot/adapters/keaimao/__init__.py
+-rw-r--r--   0        0        0     5722 2023-04-20 11:08:26.809253 pepperbot-0.3.6/pepperbot/adapters/keaimao/api/__init__.py
+-rw-r--r--   0        0        0     2649 2023-05-16 04:58:38.717680 pepperbot-0.3.6/pepperbot/adapters/keaimao/event/__init__.py
+-rw-r--r--   0        0        0    21222 2022-04-13 12:45:33.068068 pepperbot-0.3.6/pepperbot/adapters/keaimao/event/records/EventFriendMsg.js
+-rw-r--r--   0        0        0    10263 2022-02-20 09:58:20.299888 pepperbot-0.3.6/pepperbot/adapters/keaimao/event/records/EventGroupMessage.js
+-rw-r--r--   0        0        0     6530 2023-05-16 05:00:29.791248 pepperbot-0.3.6/pepperbot/adapters/onebot/__init__.py
+-rw-r--r--   0        0        0    25015 2023-05-16 04:59:35.810685 pepperbot-0.3.6/pepperbot/adapters/onebot/api/__init__.py
+-rw-r--r--   0        0        0     8909 2023-05-16 05:00:03.992500 pepperbot-0.3.6/pepperbot/adapters/onebot/event/__init__.py
+-rw-r--r--   0        0        0       67 2023-04-14 16:22:16.875389 pepperbot-0.3.6/pepperbot/adapters/onebot/models/__init__.py
+-rw-r--r--   0        0        0      696 2023-04-14 16:01:58.086198 pepperbot-0.3.6/pepperbot/adapters/onebot/models/group.py
+-rw-r--r--   0        0        0      572 2022-02-20 09:58:20.311051 pepperbot-0.3.6/pepperbot/adapters/onebot/models/message.py
+-rw-r--r--   0        0        0     1395 2023-04-14 16:22:28.359913 pepperbot-0.3.6/pepperbot/adapters/onebot/models/user.py
+-rw-r--r--   0        0        0     9195 2023-05-16 04:58:11.180375 pepperbot-0.3.6/pepperbot/adapters/telegram/__init__.py
+-rw-r--r--   0        0        0     2931 2023-04-20 11:10:48.986337 pepperbot-0.3.6/pepperbot/adapters/telegram/api/__init__.py
+-rw-r--r--   0        0        0     4663 2023-04-19 05:22:27.264737 pepperbot-0.3.6/pepperbot/adapters/telegram/event/__init__.py
+-rw-r--r--   0        0        0     1064 2023-05-16 05:00:52.564864 pepperbot-0.3.6/pepperbot/adapters/universal/__init__.py
+-rw-r--r--   0        0        0     2709 2023-04-20 11:10:48.986337 pepperbot-0.3.6/pepperbot/adapters/universal/api/__init__.py
+-rw-r--r--   0        0        0     3245 2023-04-15 23:11:30.691877 pepperbot-0.3.6/pepperbot/adapters/universal/event/__init__.py
+-rw-r--r--   0        0        0      766 2023-04-10 15:18:25.547755 pepperbot-0.3.6/pepperbot/config.py
+-rw-r--r--   0        0        0        0 2022-02-20 09:58:20.315950 pepperbot-0.3.6/pepperbot/core/__init__.py
+-rw-r--r--   0        0        0     2802 2023-05-16 04:51:12.572119 pepperbot-0.3.6/pepperbot/core/api/api_caller.py
+-rw-r--r--   0        0        0      835 2022-02-20 09:58:20.317490 pepperbot-0.3.6/pepperbot/core/api/decorators.py
+-rw-r--r--   0        0        0        0 2022-02-20 09:58:20.319000 pepperbot-0.3.6/pepperbot/core/event/__init__.py
+-rw-r--r--   0        0        0     1514 2023-05-16 04:57:25.719150 pepperbot-0.3.6/pepperbot/core/event/base_adapter.py
+-rw-r--r--   0        0        0    22264 2023-05-14 07:05:01.550490 pepperbot-0.3.6/pepperbot/core/event/handle.py
+-rw-r--r--   0        0        0     1648 2023-05-16 05:01:18.429996 pepperbot-0.3.6/pepperbot/core/event/universal.py
+-rw-r--r--   0        0        0     3020 2022-05-04 06:33:33.296283 pepperbot-0.3.6/pepperbot/core/event/utils.py
+-rw-r--r--   0        0        0      931 2022-05-03 12:01:53.466811 pepperbot-0.3.6/pepperbot/core/message/base.py
+-rw-r--r--   0        0        0    11258 2023-05-07 12:55:09.643864 pepperbot-0.3.6/pepperbot/core/message/chain.py
+-rw-r--r--   0        0        0    16761 2023-05-07 08:29:43.324781 pepperbot-0.3.6/pepperbot/core/message/segment.py
+-rw-r--r--   0        0        0       84 2023-04-22 12:37:07.245598 pepperbot-0.3.6/pepperbot/core/route/__init__.py
+-rw-r--r--   0        0        0     5435 2023-05-08 12:03:14.378466 pepperbot-0.3.6/pepperbot/core/route/available/__init__.py
+-rw-r--r--   0        0        0     1359 2023-04-22 15:10:40.463249 pepperbot-0.3.6/pepperbot/core/route/available/decorators.py
+-rw-r--r--   0        0        0     4444 2023-05-09 13:46:28.690963 pepperbot-0.3.6/pepperbot/core/route/cache.py
+-rw-r--r--   0        0        0      326 2022-02-20 09:58:20.368067 pepperbot-0.3.6/pepperbot/core/route/hook.py
+-rw-r--r--   0        0        0     6520 2023-04-20 12:02:43.500740 pepperbot-0.3.6/pepperbot/core/route/parse.py
+-rw-r--r--   0        0        0     1812 2023-05-08 12:21:46.168927 pepperbot-0.3.6/pepperbot/core/route/utils.py
+-rw-r--r--   0        0        0    15923 2023-05-16 05:04:55.304440 pepperbot-0.3.6/pepperbot/core/route/validate.py
+-rw-r--r--   0        0        0     1165 2023-04-20 10:22:17.059555 pepperbot-0.3.6/pepperbot/exceptions.py
+-rw-r--r--   0        0        0        0 2022-02-20 09:58:20.371633 pepperbot-0.3.6/pepperbot/extensions/__init__.py
+-rw-r--r--   0        0        0     2146 2022-07-12 14:55:41.437631 pepperbot-0.3.6/pepperbot/extensions/action/__init__.py
+-rw-r--r--   0        0        0     1323 2022-02-20 09:58:20.372621 pepperbot-0.3.6/pepperbot/extensions/action/action.py
+-rw-r--r--   0        0        0     9917 2022-02-20 09:58:20.372621 pepperbot-0.3.6/pepperbot/extensions/action/chain.py
+-rw-r--r--   0        0        0     2813 2022-02-20 09:58:20.373773 pepperbot-0.3.6/pepperbot/extensions/action/decorators.py
+-rw-r--r--   0        0        0     2413 2022-02-20 09:58:20.374299 pepperbot-0.3.6/pepperbot/extensions/action/runner.py
+-rw-r--r--   0        0        0     5403 2023-05-10 10:28:59.173753 pepperbot-0.3.6/pepperbot/extensions/command/__init__.py
+-rw-r--r--   0        0        0     1756 2023-05-10 10:33:38.549803 pepperbot-0.3.6/pepperbot/extensions/command/constant.py
+-rw-r--r--   0        0        0    16554 2023-05-16 05:04:00.576694 pepperbot-0.3.6/pepperbot/extensions/command/handle.py
+-rw-r--r--   0        0        0     2372 2023-05-09 13:47:27.145829 pepperbot-0.3.6/pepperbot/extensions/command/node.py
+-rw-r--r--   0        0        0      532 2023-05-07 08:20:17.196776 pepperbot-0.3.6/pepperbot/extensions/command/parser.py
+-rw-r--r--   0        0        0    26875 2023-05-14 07:26:25.926670 pepperbot-0.3.6/pepperbot/extensions/command/pattern.py
+-rw-r--r--   0        0        0     2491 2023-04-20 11:29:18.885191 pepperbot-0.3.6/pepperbot/extensions/command/sender.py
+-rw-r--r--   0        0        0     6643 2023-05-16 04:31:24.292113 pepperbot-0.3.6/pepperbot/extensions/command/timeout.py
+-rw-r--r--   0        0        0    12905 2023-05-16 05:04:34.175837 pepperbot-0.3.6/pepperbot/extensions/command/utils.py
+-rw-r--r--   0        0        0     2093 2023-05-08 12:46:01.677718 pepperbot-0.3.6/pepperbot/extensions/log/__init__.py
+-rw-r--r--   0        0        0      103 2023-04-07 14:00:53.161961 pepperbot-0.3.6/pepperbot/extensions/scheduler/__init__.py
+-rw-r--r--   0        0        0     8993 2023-05-14 15:12:16.283731 pepperbot-0.3.6/pepperbot/initial.py
+-rw-r--r--   0        0        0       79 2022-02-20 09:58:20.384843 pepperbot-0.3.6/pepperbot/store/__init__.py
+-rw-r--r--   0        0        0     9348 2023-05-16 04:56:06.308978 pepperbot-0.3.6/pepperbot/store/command.py
+-rw-r--r--   0        0        0     2427 2023-05-16 04:51:51.987867 pepperbot-0.3.6/pepperbot/store/event.py
+-rw-r--r--   0        0        0    14722 2023-05-16 04:56:28.944146 pepperbot-0.3.6/pepperbot/store/meta.py
+-rw-r--r--   0        0        0     2953 2023-05-09 13:59:16.374374 pepperbot-0.3.6/pepperbot/store/orm.py
+-rw-r--r--   0        0        0     1750 2023-05-02 21:52:09.236997 pepperbot-0.3.6/pepperbot/types.py
+-rw-r--r--   0        0        0        0 2021-05-20 10:22:56.350973 pepperbot-0.3.6/pepperbot/utils/__init__.py
+-rw-r--r--   0        0        0     5919 2023-05-16 05:11:49.201533 pepperbot-0.3.6/pepperbot/utils/common.py
+-rw-r--r--   0        0        0     1889 2023-05-16 05:16:16.135024 pepperbot-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0      117 2023-05-14 14:28:09.576125 pepperbot-0.3.6/tests/.env
+-rw-r--r--   0        0        0      149 2023-05-14 13:14:09.503220 pepperbot-0.3.6/tests/__init__.py
+-rw-r--r--   0        0        0    12411 2023-05-14 14:08:58.369335 pepperbot-0.3.6/tests/command/test_cli_argument.py
+-rw-r--r--   0        0        0    14400 2023-05-14 14:09:12.598323 pepperbot-0.3.6/tests/command/test_lifecycle.py
+-rw-r--r--   0        0        0      146 2023-05-14 12:55:38.262467 pepperbot-0.3.6/tests/command/test_match.py
+-rw-r--r--   0        0        0     5980 2023-05-07 12:54:47.433922 pepperbot-0.3.6/tests/command/test_merge.py
+-rw-r--r--   0        0        0      334 2023-05-14 12:58:22.365119 pepperbot-0.3.6/tests/command/test_parameters.py
+-rw-r--r--   0        0        0    26473 2023-05-14 14:09:30.504063 pepperbot-0.3.6/tests/command/test_sub_command.py
+-rw-r--r--   0        0        0      667 2023-05-14 12:56:39.030933 pepperbot-0.3.6/tests/command/test_types.py
+-rw-r--r--   0        0        0      585 2023-05-14 13:00:23.123882 pepperbot-0.3.6/tests/command/test_validate.py
+-rw-r--r--   0        0        0     2349 2023-05-14 15:33:55.936185 pepperbot-0.3.6/tests/conftest.py
+-rw-r--r--   0        0        0      775 2023-05-14 13:02:04.308930 pepperbot-0.3.6/tests/core/test_available.py
+-rw-r--r--   0        0        0      875 2023-05-13 16:49:27.289917 pepperbot-0.3.6/tests/core/test_dispatch.py
+-rw-r--r--   0        0        0     1379 2023-05-14 13:14:52.555206 pepperbot-0.3.6/tests/core/test_route.py
+-rw-r--r--   0        0        0     2305 2023-05-14 14:20:30.082636 pepperbot-0.3.6/tests/message/test_chain.py
+-rw-r--r--   0        0        0      501 2023-05-14 14:34:57.784528 pepperbot-0.3.6/tests/message/test_segment.py
+-rw-r--r--   0        0        0     2640 2021-05-20 11:42:38.152329 pepperbot-0.3.6/tests/tree.py
+-rw-r--r--   0        0        0     1096 2023-05-08 07:29:48.570650 pepperbot-0.3.6/tests/utils.py
+-rw-r--r--   0        0        0     6206 1970-01-01 00:00:00.000000 pepperbot-0.3.6/PKG-INFO
```

### Comparing `pepperbot-0.3.5/LICENSE` & `pepperbot-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.5/README.md` & `pepperbot-0.3.6/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 <p align="center">
 <a href="https://ssmjae.github.io/PepperBot/">文档</a> ·
 <a href="https://jq.qq.com/?_wv=1027&k=EPhcRRib">QQ交流群</a>  
 </p>
 
 <p align="center">
 <img src="./archive/coverage-badge.svg" />
+<img src="https://badge.fury.io/py/pepperbot.svg" />
+<img src="https://img.shields.io/badge/python-3.8+-blue.svg" />
+<img src="https://static.pepy.tech/badge/pepperbot/month" />
+
 </p>
 
 ## 生而跨平台
 
 - QQ 基于 `Onebot`，`Mirai`(待实现)、`OPQ`(待实现)
 - 微信基于`可爱猫`
 - Telegram基于`Pyrogram`
@@ -48,23 +52,24 @@
 - 基于 python3.6 之后的类型注解，提供了完全的类型提示
 - 大部分可以自动获取的参数，都会自动获取，不需要每次手动提供了
 - 只会动态注入用到的参数，没必要每次写一长串用不到的参数了！
 - 文档中，均有可直接复制使用的代码片段，快速开发
 
 ## 测试文档全
 
-- 通过元编程(AST 之类)手段，对编写的各种代码进行规则检查，并输出易于理解的错误信息，将问题消灭在框架启动之前
+- 自带linter
+  - 通过元编程(AST 之类)手段，对编写的各种代码进行规则检查，并输出易于理解的错误信息，将问题消灭在框架启动之前
 - 文档比较全
 - 测试覆盖比较全面
 - 大量官方示例/指令
 - 来自作者的 QA(加群以获取)
 
 ## 安装
 
-目前只能3.10及以上，因为用了点新特性，之后会恢复对3.8的支持
+TODO 目前只能3.10及以上，因为用了点新特性，之后会恢复对3.8的支持
 
 ```bash
 pip install pepperbot
 ```
 
 ## 使用
 
@@ -112,12 +117,14 @@
                 Text("没人"),
                 Image("http://123.jpg"),
             )
 ```
 
 ## 生态
 
+[插件市场](https://ssmjae.github.io/PepperBot/market/)
+
 ### 可以记忆上下文的GPT群聊机器人
 
-[PepperBot-GPT]( )
+[pepperbot-ai-query](https://github.com/SSmJaE/PepperBot/tree/master/capabilities/pepperbot_gpt_example )
 
 ### 通过GPT，自动检测群聊中的广告信息
```

#### html2text {}

```diff
@@ -1,12 +1,14 @@
                             ****** PepperBot ******
                              [./archive/icon.png]
 ä¸ä¸ªç¬¦åç´è§çè·¨ç¤¾äº¤å¹³å°æºå¨äººæ¡æ¶ï¼è½»æ¾å°å¨å¹³å°é´ä¼ éæ¶æ¯ï¼æ¯æQQãå¾®ä¿¡ãTelegram
                              ææ¡£ Â· QQäº¤æµç¾¤
-                        [./archive/coverage-badge.svg]
+[./archive/coverage-badge.svg] [https://badge.fury.io/py/pepperbot.svg] [https:
+ //img.shields.io/badge/python-3.8+-blue.svg] [https://static.pepy.tech/badge/
+                               pepperbot/month]
 ## çèè·¨å¹³å° - QQ åºäº `Onebot`ï¼`Mirai`(å¾å®ç°)ã`OPQ`(å¾å®ç°)
 - å¾®ä¿¡åºäº`å¯ç±ç«` - Telegramåºäº`Pyrogram` -
 æä¾äºè·¨å¹³å°ãæç¨çæ¶æ¯ç±»å(çæ®µ) -
 éç¨äºä»¶ï¼æ¯å¦ç¾¤æ¶æ¯ãç§èæ¶æ¯ç­ï¼æä¾äºç»ä¸çæ¥å£ï¼åªéè¦åä¸æ¬¡ä»£ç ï¼å°±å¯ä»¥æ ç¼åºç¨å°åä¸ªå¹³å°ä¸ï¼è·¨å¹³å°çæ¶æ¯ä¼ éä»æªå¦æ­¤è½»æ¾éæ
 - å¯ä»¥è·¨ç¾¤ãè·¨å¹³å°å±äº«æä»¤(çç¶æ)ï¼æèå¨å±éå®ç¨æ·
 (ä¸ç®¡ç¨æ·æ¯éè¿ç¾¤èè¿æ¯ç§è) ## æ§è½ä¹å¤ç¨ -
 åºå±åºäºå¼æ­¥ç Sanic æ¡æ¶ï¼ç®åæä¸å®çæç python web
@@ -25,18 +27,18 @@
 [ ] `fastAPI`é£æ ¼ç**ä¾èµæ³¨å¥** ## æ¥å£åè¯­ä¹ - API
 ç¬¦åç´è§ï¼ç´è§ï¼æµçå°ææ³æ³æ å°å°ä»£ç ä¸ - åºäº python3.6
 ä¹åçç±»åæ³¨è§£ï¼æä¾äºå®å¨çç±»åæç¤º -
 å¤§é¨åå¯ä»¥èªå¨è·åçåæ°ï¼é½ä¼èªå¨è·åï¼ä¸éè¦æ¯æ¬¡æå¨æä¾äº
 -
 åªä¼å¨ææ³¨å¥ç¨å°çåæ°ï¼æ²¡å¿è¦æ¯æ¬¡åä¸é¿ä¸²ç¨ä¸å°çåæ°äºï¼
 - ææ¡£ä¸­ï¼åæå¯ç´æ¥å¤å¶ä½¿ç¨çä»£ç çæ®µï¼å¿«éå¼å ##
-æµè¯ææ¡£å¨ - éè¿åç¼ç¨(AST
+æµè¯ææ¡£å¨ - èªå¸¦linter - éè¿åç¼ç¨(AST
 ä¹ç±»)ææ®µï¼å¯¹ç¼åçåç§ä»£ç è¿è¡è§åæ£æ¥ï¼å¹¶è¾åºæäºçè§£çéè¯¯ä¿¡æ¯ï¼å°é®é¢æ¶ç­å¨æ¡æ¶å¯å¨ä¹å
 - ææ¡£æ¯è¾å¨ - æµè¯è¦çæ¯è¾å¨é¢ - å¤§éå®æ¹ç¤ºä¾/æä»¤ -
-æ¥èªä½èç QA(å ç¾¤ä»¥è·å) ## å®è£
+æ¥èªä½èç QA(å ç¾¤ä»¥è·å) ## å®è£ TODO
 ç®ååªè½3.10åä»¥ä¸ï¼å ä¸ºç¨äºç¹æ°ç¹æ§ï¼ä¹åä¼æ¢å¤å¯¹3.8çæ¯æ
 ```bash pip install pepperbot ``` ## ä½¿ç¨ [å·ä½ä½¿ç¨è§ææ¡£](https://
 ssmjae.github.io/PepperBot/) ## ç¤ºä¾ å­è¡ä»£ç å®ç°æ¶æ¯äºè½¬ ```py
 class WhateverNameYouWant: async def group_message(self, bot:
 UniversalGroupBot, chain: MessageChain): if bot.onebot: #
 è½¬åqqæ¶æ¯è³å¾®ä¿¡ãTG await bot.arbitrary.keaimao.group_message
 ("19521241254@chatroom", *chain.segments) await
@@ -52,9 +54,11 @@
 å¯ä»¥ç´æ¥âæ¤åæ¶æ¯âï¼ç¬¦åç´è§ if "è¸¢åºæ" ==
 chain.pure_text: await sender.kickout() # å¯ä»¥ç´æ¥è¸¢åºåè¨ç¾¤å #
 ä¹å¯ä»¥å¯¹æ¶æ¯é¾è¿è¡inæä½ï¼ç¸å½äºin chain.pure_text if
 "ç¦è¨æ" in chain: await sender.ban(10) # å¯ä»¥ç´æ¥ç¦è¨åè¨ç¾¤å if
 chain.regex("æäºº(å¨|å|å|å¨å).?"): # åéä¸æ¡ç¾¤æ¶æ¯ #
 æ¥åä»»æä¸ªåæ°ï¼å¿é¡»æ¯åæ³çæ¶æ¯çæ®µï¼æ¯å¦Textï¼Faceï¼Image
 await bot.group_message( Text("æ²¡äºº"), Image("http://123.jpg"), ) ``` ##
-çæ ### å¯ä»¥è®°å¿ä¸ä¸æçGPTç¾¤èæºå¨äºº [PepperBot-GPT]( ) ###
-éè¿GPTï¼èªå¨æ£æµç¾¤èä¸­çå¹¿åä¿¡æ¯
+çæ [æä»¶å¸åº](https://ssmjae.github.io/PepperBot/market/) ###
+å¯ä»¥è®°å¿ä¸ä¸æçGPTç¾¤èæºå¨äºº [pepperbot-ai-query](https://
+github.com/SSmJaE/PepperBot/tree/master/capabilities/pepperbot_gpt_example )
+### éè¿GPTï¼èªå¨æ£æµç¾¤èä¸­çå¹¿åä¿¡æ¯
```

### Comparing `pepperbot-0.3.5/pepperbot/__init__.py` & `pepperbot-0.3.6/pepperbot/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.5/pepperbot/adapters/keaimao/__init__.py` & `pepperbot-0.3.6/pepperbot/adapters/keaimao/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from typing import Dict, Optional, cast
+from typing import Dict, List, Optional, cast
 
 from pepperbot.adapters.keaimao.event import KeaimaoEvent
 from pepperbot.core.event.base_adapter import BaseAdapter
 from pepperbot.exceptions import EventHandleError
 from pepperbot.store.event import ProtocolEvent, filter_event_by_type
 from pepperbot.types import T_ConversationType
 from pepperbot.utils.common import get_own_attributes
 
 own_attributes = get_own_attributes(KeaimaoEvent)
 
-events: list[ProtocolEvent] = [getattr(KeaimaoEvent, attr) for attr in own_attributes]
+events: List[ProtocolEvent] = [getattr(KeaimaoEvent, attr) for attr in own_attributes]
 
 
 class KeaimaoAdapter(BaseAdapter):
     kwargs_mapping = {
         cast(str, event.protocol_event_name): event.keyword_arguments
         for event in events
     }
```

### Comparing `pepperbot-0.3.5/pepperbot/adapters/keaimao/api/__init__.py` & `pepperbot-0.3.6/pepperbot/adapters/keaimao/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.5/pepperbot/adapters/keaimao/event/__init__.py` & `pepperbot-0.3.6/pepperbot/adapters/keaimao/event/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # https://www.kancloud.cn/yangtaott/dsaw/1179271
 
-from typing import Dict
+from typing import Dict, Union
 
 from pydantic import root_validator
 from pepperbot.adapters.keaimao.api import KeaimaoGroupBot, KeaimaoPrivateBot
 from pepperbot.core.message.chain import MessageChain, chain_factory
 from pepperbot.store.event import EventHandlerKwarg, ProtocolEvent
 
 raw_event = EventHandlerKwarg(
     name="raw_event",
-    type_=Dict | dict,
+    type_=Union[Dict, dict],
     value=lambda raw_event: raw_event,
 )
 
 group_bot = EventHandlerKwarg(
     name="bot",
     type_=KeaimaoGroupBot,
     value=lambda bot: bot,
```

### Comparing `pepperbot-0.3.5/pepperbot/adapters/keaimao/event/records/EventFriendMsg.js` & `pepperbot-0.3.6/pepperbot/adapters/keaimao/event/records/EventFriendMsg.js`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.5/pepperbot/adapters/keaimao/event/records/EventGroupMessage.js` & `pepperbot-0.3.6/pepperbot/adapters/keaimao/event/records/EventGroupMessage.js`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.5/pepperbot/adapters/onebot/__init__.py` & `pepperbot-0.3.6/pepperbot/adapters/onebot/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, Optional, cast
+from typing import Dict, List, Optional, cast
 
 import arrow
 from pepperbot.adapters.onebot.event import OnebotV11Event
 from pepperbot.core.event.base_adapter import BaseAdapter
 from pepperbot.exceptions import EventHandleError
 from pepperbot.extensions.log import logger
 from pepperbot.store.event import ProtocolEvent, filter_event_by_type
@@ -10,15 +10,15 @@
 from pepperbot.store.orm import get_metadata
 from pepperbot.types import T_ConversationType
 from pepperbot.utils.common import get_own_attributes
 
 
 own_attributes = get_own_attributes(OnebotV11Event)
 
-events: list[ProtocolEvent] = [getattr(OnebotV11Event, attr) for attr in own_attributes]
+events: List[ProtocolEvent] = [getattr(OnebotV11Event, attr) for attr in own_attributes]
 
 
 class OnebotV11Adapter(BaseAdapter):
     kwargs_mapping = {
         cast(str, event.protocol_event_name): event.keyword_arguments
         for event in events
     }
```

### Comparing `pepperbot-0.3.5/pepperbot/adapters/onebot/api/__init__.py` & `pepperbot-0.3.6/pepperbot/adapters/onebot/api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,15 +178,15 @@
             "mark_msg_as_read",
             **{
                 "message_id": message_id,
             },
         )
 
     @staticmethod
-    async def get_forward_msg(message_id: str) -> list[dict[str, Any]]:
+    async def get_forward_msg(message_id: str) -> List[Dict[str, Any]]:
         """
         获取合并转发内容
 
         https://docs.go-cqhttp.org/api/#获取合并转发内容
 
         Args:
             message_id (str): 消息 ID
@@ -205,15 +205,15 @@
                 "message_id": message_id,
             },
         )
         messages = resp.get("data", {}).get("messages", [])
         return messages
 
     @staticmethod
-    async def send_group_forward_msg(group_id: int, messages: list[dict]) -> dict:
+    async def send_group_forward_msg(group_id: int, messages: List[dict]) -> dict:
         """
         发送合并转发 ( 群聊 )
 
         https://docs.go-cqhttp.org/api/#发送合并转发-群聊-
 
         Args:
             group_id (int): 群号
@@ -229,15 +229,15 @@
             **{
                 "group_id": group_id,
                 "messages": messages,
             },
         )
 
     @staticmethod
-    async def send_private_forward_msg(user_id: int, messages: list[dict]) -> dict:
+    async def send_private_forward_msg(user_id: int, messages: List[dict]) -> dict:
         """
         发送合并转发 ( 好友 )
 
         Args:
             user_id (int): 好友 QQ 号
             messages (List[dict]): 自定义转发消息, 具体看 CQcode
```

### Comparing `pepperbot-0.3.5/pepperbot/adapters/onebot/event/__init__.py` & `pepperbot-0.3.6/pepperbot/adapters/onebot/event/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict
+from typing import Dict, Union
 
 from pydantic import root_validator
 
 from pepperbot.adapters.onebot.api import (
     OnebotV11API,
     OnebotV11GroupBot,
     OnebotV11PrivateBot,
@@ -22,15 +22,15 @@
     from pepperbot.core.message.chain import chain_factory
 
     return chain_factory(event_meta)
 
 
 raw_event = EventHandlerKwarg(
     name="raw_event",
-    type_=Dict | dict,
+    type_=Union[Dict, dict],
     value=lambda raw_event: raw_event,
 )
 group_bot = EventHandlerKwarg(
     name="bot",
     type_=OnebotV11GroupBot,
     value=lambda bot: bot,
 )
@@ -239,91 +239,7 @@
         ),
     )
     been_friend_poked = OnebotV11ProtocolEvent(
         event_type=("private",),
         raw_event_name="friend_poked",
         description="好友戳一戳",
     )
-
-
-# RELATIONS = {
-#     "group": {
-#         "GroupMessage": [
-#             GroupEvent.group_message,
-#             GroupEvent.group_anonymous_essage,
-#         ],
-#         "GroupNotice": [
-#             GroupEvent.group_notice,
-#             GroupEvent.group_message_been_withdraw,
-#             GroupEvent.group_admin_change,
-#             GroupEvent.group_ban_change,
-#             GroupEvent.group_honor_change,
-#             GroupEvent.member_increased,
-#             GroupEvent.member_declined,
-#             GroupEvent.new_file_uploaded,
-#             GroupEvent.been_group_poked,
-#         ],
-#         "GroupRequest": [
-#             GroupEvent.add_group,
-#             GroupEvent.been_invited,
-#         ],
-#     },
-#     "private": {
-#         "FriendMessage": [
-#             GroupEvent.friend_message,
-#             GroupEvent.temp_message,
-#         ],
-#         "FriendRequest": [
-#             GroupEvent.been_added,
-#         ],
-#         "FriendNotice": [
-#             GroupEvent.been_friend_poked,
-#             GroupEvent.friend_message_been_withdraw,
-#         ],
-#     },
-# }
-
-
-# def get_parent_level(bottomGroupEvent: Union[str, Any]):
-#     for key, value in RELATIONS["group"].items():
-#         if bottomGroupEvent in value:
-#             return key
-
-#     raise Exception("无效事件")
-
-
-# GROUP_EVENTS: List[str] = []
-
-# for _, subTypes in RELATIONS["group"].items():
-#     GROUP_EVENTS.extend(subTypes)
-
-# GROUP_EVENTS_WITH_LIFECYCLE = [*GROUP_EVENTS]
-# for event in GROUP_EVENTS:
-#     GROUP_EVENTS_WITH_LIFECYCLE.append("before_" + event)
-#     GROUP_EVENTS_WITH_LIFECYCLE.append("after_" + event)
-
-
-# def is_group_event(event: str) -> bool:
-#     return event in GROUP_EVENTS
-
-
-# def is_valid_group_method(methodName: str):
-#     return methodName in GROUP_EVENTS_WITH_LIFECYCLE
-
-
-# FRIEND_EVENTS: List[str] = []
-
-# for _, subTypes in RELATIONS["friend"].items():
-#     FRIEND_EVENTS.extend(subTypes)
-
-# FRIEND_EVENTS_WITH_LIFECYCLE = [*FRIEND_EVENTS]
-# for event in GROUP_EVENTS:
-#     FRIEND_EVENTS_WITH_LIFECYCLE.append("before_" + event)
-#     FRIEND_EVENTS_WITH_LIFECYCLE.append("after_" + event)
-
-
-# def is_friend_event(event: str) -> bool:
-#     return event in FRIEND_EVENTS
-
-
-# def is_valid_friend_method(methodName: str):
-#     return methodName in FRIEND_EVENTS_WITH_LIFECYCLE
```

### Comparing `pepperbot-0.3.5/pepperbot/adapters/onebot/models/group.py` & `pepperbot-0.3.6/pepperbot/adapters/onebot/models/group.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.5/pepperbot/adapters/onebot/models/message.py` & `pepperbot-0.3.6/pepperbot/adapters/onebot/models/message.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.5/pepperbot/adapters/onebot/models/user.py` & `pepperbot-0.3.6/pepperbot/adapters/onebot/models/user.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.5/pepperbot/adapters/telegram/__init__.py` & `pepperbot-0.3.6/pepperbot/adapters/telegram/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Callable, Dict, Optional, cast
+from typing import Any, Callable, Dict, List, Optional, Union, cast
 
 from devtools import debug
 from pepperbot.adapters.telegram.event import TelegramEvent
 from pepperbot.core.event.base_adapter import BaseAdapter
 from pepperbot.exceptions import EventHandleError
 from pepperbot.extensions.log import debug_log, logger
 from pepperbot.store.event import ProtocolEvent, filter_event_by_type
@@ -20,15 +20,15 @@
 from pyrogram.handlers.message_handler import MessageHandler
 from pyrogram.handlers.raw_update_handler import RawUpdateHandler
 from pyrogram.types import CallbackQuery, ChatEventFilter, Message
 
 
 own_attributes = get_own_attributes(TelegramEvent)
 
-events: list[ProtocolEvent] = [getattr(TelegramEvent, attr) for attr in own_attributes]
+events: List[ProtocolEvent] = [getattr(TelegramEvent, attr) for attr in own_attributes]
 
 
 class TelegramAdapter(BaseAdapter):
     kwargs_mapping = {
         cast(str, event.protocol_event_name): event.keyword_arguments
         for event in events
     }
@@ -102,15 +102,15 @@
 
     @staticmethod
     def get_user_id(raw_event: Dict, mode: T_ConversationType):
         callback_object = raw_event["callback_object"]
 
         # debug_log(callback_object)
 
-        user_id: Optional[int | str] = None
+        user_id: Optional[Union[int, str]] = None
 
         if isinstance(callback_object, CallbackQuery):
             user_id = callback_object.from_user.id
 
         elif isinstance(callback_object, Message):
             user_id = callback_object.from_user.id
 
@@ -220,15 +220,15 @@
     avoid circlely import caused by `handle_event`
 
     pass `handle_event` as parameter to avoid multiple times import
     """
 
     async def wrapper(client, callback_object, *args):
         try:
-            debug(*args)
+            # debug(*args)
             return await handler(client, callback_object, handle_event, *args)
 
         except ContinuePropagation:
             raise ContinuePropagation
 
         except Exception as e:
             logger.exception(e)
```

### Comparing `pepperbot-0.3.5/pepperbot/adapters/telegram/api/__init__.py` & `pepperbot-0.3.6/pepperbot/adapters/telegram/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.5/pepperbot/adapters/telegram/event/__init__.py` & `pepperbot-0.3.6/pepperbot/adapters/telegram/event/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.5/pepperbot/adapters/universal/api/__init__.py` & `pepperbot-0.3.6/pepperbot/adapters/universal/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.5/pepperbot/adapters/universal/event/__init__.py` & `pepperbot-0.3.6/pepperbot/adapters/universal/event/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.5/pepperbot/config.py` & `pepperbot-0.3.6/pepperbot/config.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.5/pepperbot/core/api/api_caller.py` & `pepperbot-0.3.6/pepperbot/core/api/api_caller.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any
+from typing import Any, Dict
 import httpx
 from pepperbot.config import global_config
 from pepperbot.exceptions import BackendApiError, InitializationError
 from pepperbot.extensions.log import debug_log, logger
 from pepperbot.types import T_BotProtocol, T_WebProtocol
 from devtools import debug
 
@@ -43,15 +43,15 @@
         self.client.close()
 
         # todo 没有找到在del中调用AsyncClient.aclose的方法
         # self.client.aclose().__await__()
 
     def to_onebot(
         self, action: str, kwargs: dict = {}, *, direct=True
-    ) -> dict[str, Any]:
+    ) -> Dict[str, Any]:
         """direct时，直接返回["data"]"""
 
         # debug_log(kwargs)
         httpx_result = self.client.post(
             f"http://{self.host}:{self.port}/{action}",
             json=kwargs,
         )
@@ -75,15 +75,15 @@
             logger.exception(exception)
             raise exception
 
         except Exception as exception:
             logger.exception("无法序列化协议端返回的数据，请检查是否正确配置了对应的ip、端口、协议")
             raise exception
 
-    def to_keaimao(self, action: str, kwargs={}) -> dict[str, Any]:
+    def to_keaimao(self, action: str, kwargs={}) -> Dict[str, Any]:
         kwargs["event"] = action
 
         debug(kwargs)
 
         return self.client.post(f"http://{self.host}:{self.port}", json=kwargs).json()
 
     async def __call__(self, action: str, **kwargs):
```

### Comparing `pepperbot-0.3.5/pepperbot/core/api/decorators.py` & `pepperbot-0.3.6/pepperbot/core/api/decorators.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.5/pepperbot/core/event/base_adapter.py` & `pepperbot-0.3.6/pepperbot/core/event/base_adapter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from typing import Dict, List, Sequence
 from pepperbot.store.event import EventHandlerKwarg, ProtocolEvent
 
 from pepperbot.types import T_ConversationType
 
 
 class BaseAdapter:
-    kwargs_mapping: dict[str, Sequence[EventHandlerKwarg]]
+    kwargs_mapping: Dict[str, Sequence[EventHandlerKwarg]]
 
     all_events: List[ProtocolEvent]
-    all_event_names: list[str]
+    all_event_names: List[str]
 
     meta_events: List[ProtocolEvent]
-    meta_event_names: list[str]
+    meta_event_names: List[str]
     notice_events: List[ProtocolEvent]
-    notice_event_names: list[str]
+    notice_event_names: List[str]
     request_events: List[ProtocolEvent]
-    request_event_names: list[str]
+    request_event_names: List[str]
     message_events: List[ProtocolEvent]
-    message_event_names: list[str]
+    message_event_names: List[str]
 
     private_events: List[ProtocolEvent]
     group_events: List[ProtocolEvent]
     channel_events = List[ProtocolEvent]
 
     @staticmethod
     def get_event(raw_event: Dict) -> ProtocolEvent:
```

### Comparing `pepperbot-0.3.5/pepperbot/core/event/handle.py` & `pepperbot-0.3.6/pepperbot/core/event/handle.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
+import json
 from collections import defaultdict
 from itertools import groupby
-import json
 from typing import (
     Any,
     Callable,
     DefaultDict,
     Dict,
     Iterator,
     List,
@@ -33,38 +33,38 @@
 from pepperbot.core.event.universal import (
     COMMAND_TRIGGER_EVENTS,
     UNIVERSAL_PROTOCOL_EVENT_MAPPING,
 )
 from pepperbot.core.event.utils import skip_current_onebot_event
 from pepperbot.core.route.available import check_available
 from pepperbot.exceptions import EventHandleError, StopPropagation
-from pepperbot.extensions.command.handle import (
+from pepperbot.extensions.command.handle import run_class_command
+from pepperbot.extensions.command.utils import (
     find_first_available_command,
     has_running_command,
-    run_class_command,
 )
 from pepperbot.extensions.log import debug_log, logger
 from pepperbot.store.event import (
     EventDispatchMetadata,
     EventHandlerKwarg,
     EventMetadata,
     PropagationConfig,
 )
 from pepperbot.store.meta import (
     LAST_ONEBOT_HEARTBEAT_TIME,
+    bot_instances,
+    class_command_config_mapping,
+    class_command_mapping,
+    class_handler_mapping,
     get_bot_id,
     get_onebot_caller,
     initial_bot_info,
     onebot_event_meta,
     route_mapping,
-    class_command_config_mapping,
-    class_handler_mapping,
     route_validator_mapping,
-    bot_instances,
-    class_command_mapping,
 )
 from pepperbot.store.orm import get_metadata, set_metadata
 from pepperbot.types import (
     BaseBot,
     T_BotProtocol,
     T_ConversationType,
     T_DispatchHandler,
@@ -134,15 +134,15 @@
     )
     event_dispatch_metadata.has_running_command = has_running
     debug_log(has_running)
     debug_log(disordered_class_command_handler)
 
     if has_running:
         # 这个是全局的，不管有多少个propagation group，只要有一个指令在运行，就不会再执行其他指令
-        logger.info(f"存在运行中的指令 <lc>{disordered_class_command_handler[3]}</lc>，继续执行该指令")
+        logger.info(f"存在运行中的指令 <lc>{disordered_class_command_handler[4]}</lc>，继续执行该指令")
         disordered_handlers.add(disordered_class_command_handler)
         event_dispatch_metadata.command_dispatch_handler = (
             disordered_class_command_handler
         )
 
     else:
         disordered_handlers |= disordered_class_command_handlers
@@ -408,15 +408,15 @@
         protocol, mode, source_id, "class_handlers"
     )
 
     debug_log(class_handler_names, "所有可用class_handler")
 
     if not class_handler_names:
         logger.info(
-            f"<lc>{event_meta.conversation_type}</lc> 模式的 <lc>{event_meta.source_id}</lc> 尚未注册class_handler"
+            f"<lc>{event_meta.conversation_type}</lc> 模式的 <lc>{event_meta.source_id}</lc> 尚未注册 <lc>class_handler</lc>"
         )
         return set()
 
     disordered_handlers: Set[T_DispatchHandler] = set()
 
     for class_handler_name in class_handler_names:
         class_handler_cache = class_handler_mapping[class_handler_name]
```

### Comparing `pepperbot-0.3.5/pepperbot/core/event/universal.py` & `pepperbot-0.3.6/pepperbot/core/event/universal.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from typing import Type
+from typing import List, Type
 from pepperbot.adapters.keaimao import KeaimaoAdapter
 from pepperbot.adapters.keaimao.event import KeaimaoEvent
 from pepperbot.adapters.onebot import OnebotV11Adapter
 from pepperbot.adapters.onebot.event import OnebotV11Event
 from pepperbot.adapters.telegram import TelegramAdapter
 from pepperbot.adapters.telegram.event import TelegramEvent
 from pepperbot.adapters.universal import UniversalAdapter
 from pepperbot.adapters.universal.event import UniversalEvent
 from pepperbot.core.event.base_adapter import BaseAdapter
 
 
-available_adapters: list[Type[BaseAdapter]] = [
+available_adapters: List[Type[BaseAdapter]] = [
     UniversalAdapter,
     OnebotV11Adapter,
     KeaimaoAdapter,
     TelegramAdapter,
 ]
 
 ALL_PROTOCOL_EVENT_NAMES = [
```

### Comparing `pepperbot-0.3.5/pepperbot/core/event/utils.py` & `pepperbot-0.3.6/pepperbot/core/event/utils.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.5/pepperbot/core/message/base.py` & `pepperbot-0.3.6/pepperbot/core/message/base.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.5/pepperbot/core/message/chain.py` & `pepperbot-0.3.6/pepperbot/core/message/chain.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.5/pepperbot/core/message/segment.py` & `pepperbot-0.3.6/pepperbot/core/message/segment.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.5/pepperbot/core/route/available/__init__.py` & `pepperbot-0.3.6/pepperbot/core/route/available/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.5/pepperbot/core/route/available/decorators.py` & `pepperbot-0.3.6/pepperbot/core/route/available/decorators.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.5/pepperbot/core/route/cache.py` & `pepperbot-0.3.6/pepperbot/core/route/cache.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from argparse import ArgumentParser
-from typing import Callable, Dict
+from typing import Callable, Dict, List
 
 from devtools import debug
 
 from pepperbot.extensions.command.handle import LIFECYCLE_WITHOUT_PATTERNS
 from pepperbot.extensions.command.node import build_command_tree
-from pepperbot.extensions.command.parser import CustomArgumentParser
 from pepperbot.extensions.command.pattern import (
-    build_sub_parsers,
-    construct_overall_help_message,
+    build_sub_parsers_for_multi_nodes,
 )
 from pepperbot.store.command import (
     ClassCommandCache,
     ClassCommandConfigCache,
     ClassCommandMethodCache,
     CommandConfig,
 )
@@ -67,14 +65,15 @@
     """同一个commandClass，就实例化一次"""
 
     class_command_instance = class_command()  # type: ignore
 
     command_method_mapping = {}
 
     with_pattern_methods = set()
+    """ 可以有cli arguments的method """
 
     relations_cache = command_relations_cache[command_name]
 
     for method in get_own_methods(class_command_instance):
         method_name = method.__name__
 
         if method_name not in LIFECYCLE_WITHOUT_PATTERNS:
@@ -84,40 +83,35 @@
 
     parsers: Dict[str, ArgumentParser] = {}
     """ 这里放的是.add_subparsers.add_parser()返回的对象 """
 
     parser_handles = {}
     """ 这里放的是add_subparsers()返回的对象，而不是parser对象 """
 
-    root_node = build_command_tree(relations_cache)
+    root_nodes = build_command_tree(relations_cache, with_pattern_methods)
 
-    main_parser = CustomArgumentParser(prog=command_name, add_help=False)
+    class_command_cache = ClassCommandCache(
+        class_instance=class_command_instance,
+        command_method_mapping=command_method_mapping,
+    )
 
-    build_sub_parsers(
-        root_node,
-        main_parser,
+    build_sub_parsers_for_multi_nodes(
+        root_nodes,
         parser_handles,
         parsers,
         relations_cache,
+        command_name,
+        class_command_cache,
         command_method_mapping,
     )
 
     # debug(parsers)
     # debug(parser_handles)
 
-    help_message = construct_overall_help_message(
-        command_name, root_node, command_method_mapping
-    )
-
-    class_command_mapping[command_name] = ClassCommandCache(
-        class_instance=class_command_instance,
-        command_method_mapping=command_method_mapping,
-        parser=main_parser,
-        help_message=help_message,
-    )
+    class_command_mapping[command_name] = class_command_cache
 
 
 def cache_class_command_config(command_name: str, command_config: CommandConfig):
     # TODO 验证一下
     # TODO 相关的文档，怎么避免意外创建多个command config
     class_command_config_mapping[command_config.config_id] = ClassCommandConfigCache(
         class_command_name=command_name,
```

### Comparing `pepperbot-0.3.5/pepperbot/core/route/parse.py` & `pepperbot-0.3.6/pepperbot/core/route/parse.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.5/pepperbot/core/route/utils.py` & `pepperbot-0.3.6/pepperbot/core/route/utils.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.5/pepperbot/core/route/validate.py` & `pepperbot-0.3.6/pepperbot/core/route/validate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,31 @@
-from ast import Call
 import ast
 import inspect
-import keyword
 import re
 import textwrap
 from typing import Any, Callable, Dict, List, Sequence, Set, Union, get_args, get_origin
 
 from devtools import debug
+
 from pepperbot.adapters.keaimao import KeaimaoAdapter
-from pepperbot.adapters.keaimao.event import KeaimaoEvent
 from pepperbot.adapters.onebot import OnebotV11Adapter
-from pepperbot.adapters.onebot.event import OnebotV11Event
 from pepperbot.adapters.telegram import TelegramAdapter
-from pepperbot.adapters.telegram.event import TelegramEvent
 from pepperbot.adapters.universal import UniversalAdapter
-from pepperbot.adapters.universal.event import UniversalEvent
 from pepperbot.core.event.universal import ALL_PROTOCOL_EVENT_NAMES
 from pepperbot.exceptions import InitializationError
-from pepperbot.extensions.command.handle import (
-    COMMAND_DEFAULT_KWARGS,
-    LIFECYCLE_WITHOUT_PATTERNS,
+from pepperbot.extensions.command.constant import (
     COMMAND_COMMON_KWARGS,
+    COMMAND_DEFAULT_KWARGS,
 )
+from pepperbot.extensions.command.handle import LIFECYCLE_WITHOUT_PATTERNS
 from pepperbot.store.command import PATTERN_ARG_TYPES, TemporaryPatternArg
 from pepperbot.store.event import EventHandlerKwarg
+from pepperbot.store.meta import command_relations_cache
 from pepperbot.types import COMMAND_CONFIG
 from pepperbot.utils.common import get_own_methods
-from pepperbot.store.meta import command_relations_cache
 
 
 def is_valid_class_handler(class_handler: object):
     for method in get_own_methods(class_handler):
         method_name = method.__name__
 
         is_class_handler_method_name_valid(method_name)
@@ -189,27 +184,28 @@
 
         is_class_command_method_return_valid(
             method, method_name, method_names, sub_command_method_names, common_prefix
         )
 
     # 先通过上面的验证，此时的方法一定有返回值，并且只返回了一个值
     involved_method_names = get_all_returned_identifiers(methods)
+    involved_method_names.add("initial")  # initial方法也需要验证
 
     # 只验证被返回的方法，其他的方法不需要验证
     for method_name in involved_method_names:
         method = method_mapping[method_name]
         is_class_command_method_args_valid(method, method_name, common_prefix)
 
     return True
 
 
 def is_class_command_method_args_valid(
     method: Callable, method_name: str, common_prefix: str
 ):
-    common_prefix += f"{method_name}方法"
+    common_prefix += f"方法 {method_name} "
 
     signature = inspect.signature(method)
 
     for arg_name, p in signature.parameters.items():
         # self
         if arg_name == "self":
             continue
@@ -256,17 +252,34 @@
 
         # pattern args
         if isinstance(p.default, TemporaryPatternArg):
             # no pattern in lifecycle hooks
             if method_name in LIFECYCLE_WITHOUT_PATTERNS:
                 raise InitializationError(common_prefix + f"这些生命周期不应支持pattern")
 
-            if p.annotation not in PATTERN_ARG_TYPES or p.annotation is Any:
+            # 考虑到Optional、List的情况
+            element_type = get_args(p.annotation)
+
+            # TODO 优化一下判断optional、list的逻辑，和pattern里的add_arguments一起
+            if element_type:
+                if container_type := get_origin(element_type[0]) is list:
+                    element_type = get_args(element_type[0])[0]
+                else:
+                    element_type = element_type[0]
+
+            else:  # 没有container
+                element_type = p.annotation
+
+            # debug(element_type)
+
+            if element_type not in PATTERN_ARG_TYPES and element_type is not Any:
                 raise InitializationError(
-                    common_prefix + f"仅支持str, bool, int, float和所有消息类型"
+                    common_prefix
+                    + f"仅支持str, bool, int, float和所有消息类型，或者Any"
+                    + f"，而你提供了 {element_type}"
                 )
 
 
 def get_ids_from_single_return(elt):
     if isinstance(elt, (ast.Name,)):
         return [elt.id]
 
@@ -351,15 +364,15 @@
                     ids=get_ids(node.value),
                 )
             )
 
     return return_statements
 
 
-def get_all_returned_identifiers(f_list: list[Callable]):
+def get_all_returned_identifiers(f_list: List[Callable]):
     identifiers: Set[str] = set()
 
     for f in f_list:
         return_statements = get_return_identifiers(f)
 
         for info in return_statements:
             ids = info["ids"]
```

### Comparing `pepperbot-0.3.5/pepperbot/exceptions.py` & `pepperbot-0.3.6/pepperbot/exceptions.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.5/pepperbot/extensions/action/__init__.py` & `pepperbot-0.3.6/pepperbot/extensions/action/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.5/pepperbot/extensions/action/action.py` & `pepperbot-0.3.6/pepperbot/extensions/action/action.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.5/pepperbot/extensions/action/chain.py` & `pepperbot-0.3.6/pepperbot/extensions/action/chain.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.5/pepperbot/extensions/action/decorators.py` & `pepperbot-0.3.6/pepperbot/extensions/action/decorators.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.5/pepperbot/extensions/action/runner.py` & `pepperbot-0.3.6/pepperbot/extensions/action/runner.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.5/pepperbot/extensions/command/__init__.py` & `pepperbot-0.3.6/pepperbot/extensions/command/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 )
 from pepperbot.store.meta import SubCommandRelation, command_relations_cache
 from pepperbot.types import COMMAND_CONFIG, BaseClassCommand, F
 from pepperbot.utils.common import get_class_name_from_method
 
 __all__ = (
     "as_command",
+    "sub_command",
     "CLIArgument",
     "CLIOption",
 )
 
 
 def as_command(
     *args,
```

### Comparing `pepperbot-0.3.5/pepperbot/extensions/command/node.py` & `pepperbot-0.3.6/pepperbot/extensions/command/node.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,76 @@
-from typing import Dict, Optional
+from typing import Dict, Iterable, List, Optional
+
+from devtools import debug
 
 from pepperbot.store.meta import SubCommandRelation
 
 
 class CommandNode:
     def __init__(self, name: str):
         self.name = name
         self.parent: Optional["CommandNode"] = None
         self.children = []
 
+    def __repr__(self):
+        return f"<CommandNode {self.name}>"
+
 
-def build_command_tree(relations_cache: Dict[str, SubCommandRelation]):
+def build_command_tree(
+    relations_cache: Dict[str, SubCommandRelation], with_pattern_methods: Iterable[str]
+):
     """构造出nest command的层级关系
 
-    - a, b, c, d, e, f, g
+    - a, b, c, d, e, f, g, h, i, j
 
     =>
 
-    - a
+    - a(initial)
         - b
             - d
             - e
         - c
             - f
             - g
+    - h(非initial、非sub command，另一个根command)
+        - i
+        - j
     """
 
     node_dict: Dict[str, CommandNode] = {}
 
-    node_dict["initial"] = CommandNode("initial")
+    root_command_method_names: List[str] = []
+
+    sub_command_method_names = list(relations_cache.keys())
+    for method_name in with_pattern_methods:
+        if method_name not in sub_command_method_names:  # 是根command
+            # node_dict["initial"] = CommandNode("initial")
+            node_dict[method_name] = CommandNode(method_name)
+            root_command_method_names.append(method_name)
 
     for method_name in relations_cache:
         node_dict[method_name] = CommandNode(method_name)
 
     for method_name, command_node in node_dict.items():
-        if method_name == "initial":
+        if method_name in root_command_method_names:
             continue
 
         sub_command_relation = relations_cache[method_name]
         parent_method_name = sub_command_relation["parent_method_name"]
 
         if parent_method_name:
             parent_command_node = node_dict[parent_method_name]
             parent_command_node.children.append(command_node)
             command_node.parent = parent_command_node
 
         else:
+            # 只有initial的sub command会走到这里
+            # 如果是其他的根command，会在上面的if中continue
             node_dict["initial"].children.append(command_node)
             command_node.parent = node_dict["initial"]
 
-    return node_dict["initial"]
+    root_command_nodes: List[CommandNode] = []
+    for root_command_name in root_command_method_names:
+        root_command_node = node_dict[root_command_name]
+        root_command_nodes.append(root_command_node)
+
+    return root_command_nodes
```

### Comparing `pepperbot-0.3.5/pepperbot/extensions/command/parser.py` & `pepperbot-0.3.6/pepperbot/extensions/command/parser.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.5/pepperbot/extensions/command/pattern.py` & `pepperbot-0.3.6/pepperbot/extensions/command/pattern.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from devtools import debug
 
 from pepperbot.core.message.chain import MessageChain, T_SegmentInstance
 from pepperbot.core.message.segment import T_SegmentClass, Text
 from pepperbot.exceptions import InitializationError, PatternFormatError
 from pepperbot.extensions.command.node import CommandNode
-from pepperbot.extensions.command.parser import CustomHelpAction
+from pepperbot.extensions.command.parser import CustomArgumentParser, CustomHelpAction
 from pepperbot.extensions.command.utils import merge_adjacent_text_segments
 from pepperbot.store.command import (
     ARGPARSE_CALLED_METHOD,
     ARGPARSE_HELP,
     DOWNGRADE_PATTERN,
     DOWNGRADE_PATTERN_FORMAT,
     FALSE_TEXTS,
@@ -278,20 +278,22 @@
 
 def construct_sub_command_help_message(
     command_name: str, pattern_args: OrderedDict[str, _PatternArg]
 ) -> str:
     return f"Usage: {command_name} [OPTIONS] [ARGS]..."
 
 
-def construct_overall_help_message(
+def construct_root_command_help_message(
     command_name: str,
     root_node: CommandNode,
     command_method_mapping: Dict[str, ClassCommandMethodCache],
 ) -> str:
-    return f"Usage: {command_name} [OPTIONS] [ARGS]..."
+    """针对根command，帮助信息包含其所有的sub command，树形展示"""
+
+    return f"Usage: {command_name}{':'+root_node.name if root_node.name != 'initial' else ''} [OPTIONS] [ARGS]..."
 
 
 def add_arguments(parser: ArgumentParser, method: Callable):
     # signature可以获取到被装饰器装饰过的函数的真实参数签名
     signature = inspect.signature(method)
 
     # debug(signature.parameters)
@@ -402,50 +404,46 @@
             help_message=p.default.kwargs.get("help", None),
             is_option=p.default.cls == "CLIOption",
             name=match_names[0],
             short_name=p.default.kwargs.get("short_name", None),
             multiple=multiple,
         )
 
-        pattern_args[match_names[0]] = pattern_arg
+        pattern_args[arg_name] = pattern_arg
 
     return pattern_args
 
 
 def get_command_stack(node: CommandNode):
     stack: List[str] = []
 
     while node:
         stack.append(node.name)
         node = node.parent  # type: ignore
 
     return stack[::-1]
 
 
-def build_sub_parsers(
+def build_sub_parsers_for_single_node(
     node: CommandNode,
-    main_parser: ArgumentParser,
     parser_handles: Dict[str, _SubParsersAction],
     parsers: Dict[str, ArgumentParser],
     relations_cache: Dict[str, SubCommandRelation],
+    command_name: str,
+    class_command_cache: ClassCommandCache,
     command_method_mapping: Dict[str, ClassCommandMethodCache],
+    root_parser: ArgumentParser,
 ):
-    """
-    一个指令中，只允许一个top parser
-
-    技术上来说，可以实现多个top parser，实现起来不复杂，但是想一想，都觉得可维护性太差了
-    """
-
     method_name = node.name
 
     # 判断是几级command，如果是第一级，那么就是main_parser，如果是第二级，那么就是sub_parser
     # 都需要保证，上一级的sub parser，已经存在
     if not node.parent:  # initial
-        parser = main_parser
-        command_final_name = "initial"
+        parser = root_parser
+        command_final_name = method_name
 
     else:
         sub_command_relation = relations_cache[method_name]
         command_final_name = sub_command_relation["command_final_name"]
 
         parent_command_name = node.parent.name
         handle = parser_handles[parent_command_name]
@@ -466,38 +464,90 @@
 
     class_command_method_cache = command_method_mapping[method_name]
     method = class_command_method_cache.method
 
     pattern_args = add_arguments(parser, method)
 
     class_command_method_cache.pattern_args = pattern_args
-    class_command_method_cache.help_message = construct_sub_command_help_message(
-        command_final_name, pattern_args
-    )
 
+    if not node.parent:
+        help_message = construct_root_command_help_message(
+            command_name, node, command_method_mapping
+        )
+
+    else:
+        help_message = construct_sub_command_help_message(
+            command_final_name, pattern_args
+        )
+
+    class_command_method_cache.help_message = help_message
     class_command_method_cache.command_stack = get_command_stack(node)
+    class_command_method_cache.is_root = node.parent is None
+
+    if not node.parent:
+        class_command_method_cache.parser = parser
+
+    class_command_cache.method_name_parser_mapping[method_name] = root_parser
 
     # 有sub_command再创建，不然，无法实现multi positional arguments，会直接尝试解析sub command
     if node.children:
         # 需要在add_subparser之前，先把所有的argument都添加进去
         # 先加参数，再加sub_command也不行，因为sub_command的本质，就是一个可选的位置参数，argparse无法解析
         handle = parser.add_subparsers(required=False)
         parser_handles[method_name] = handle
 
         for child in node.children:
-            build_sub_parsers(
+            build_sub_parsers_for_single_node(
                 child,
-                main_parser,
                 parser_handles,
                 parsers,
                 relations_cache,
+                command_name,
+                class_command_cache,
                 command_method_mapping,
+                root_parser,
             )
 
 
+def build_sub_parsers_for_multi_nodes(
+    root_nodes: List[CommandNode],
+    parser_handles: Dict[str, _SubParsersAction],
+    parsers: Dict[str, ArgumentParser],
+    relations_cache: Dict[str, SubCommandRelation],
+    command_name: str,
+    class_command_cache: ClassCommandCache,
+    command_method_mapping: Dict[str, ClassCommandMethodCache],
+):
+    """
+    一个指令中，允许多个top parser
+
+    虽然实现多个top parser，但是只是为了，让非initial、非sub_command的method，也能使用命令行参数
+
+    对于nest command，一个指令还是只建议实现一个，否则会很难维护
+
+    """
+
+    for root_node in root_nodes:
+        root_parser = CustomArgumentParser(
+            prog=f"{command_name}_{root_node.name}",
+            add_help=False,
+        )
+
+        build_sub_parsers_for_single_node(
+            root_node,
+            parser_handles,
+            parsers,
+            relations_cache,
+            command_name,
+            class_command_cache,
+            command_method_mapping,
+            root_parser,
+        )
+
+
 # def get_pattern_results(
 #     compressed_patterns: List[
 #         Union[List[Tuple[str, GT_PatternArg]], Tuple[str, GT_PatternArg]]
 #     ],
 #     compressed_segments: List[T_SegmentInstance],
 # ):
 #     pattern_result: OrderedDict[str, T_PatternArgInstance] = OrderedDict()
@@ -520,15 +570,15 @@
 
 #                 pattern_result[arg_name] = convert_base_type(
 #                     arg_name,
 #                     arg_type,
 #                     text_without_type,
 #                 )
 
-#         # todo 支持pydantic的Field，比如gt,lt,对输出的报错信息，转为PatternFormotError
+#         # todo 支持pydantic的Field，比如gt,lt,对输出的报错信息，转为PatternFormatError
 #         # 最好能找到，pydantic中是怎么使用ModelField进行字段验证的，只是使用就好了
 #         # snap: int = Field(
 #         #     42,
 #         #     title="The Snap",
 #         #     description="this is the value of snap",
 #         #     gt=30,
 #         #     lt=50,
@@ -563,15 +613,15 @@
 #     pass
 
 
 async def parse_pattern(
     event_metadata: EventMetadata,
     class_command_cache: ClassCommandCache,
     cache: ClassCommandMethodCache,
-    method_name,
+    method_name: str,
     command_kwargs: Dict[str, Any],
     command_name: str,
     status: ClassCommandStatus,
 ):
     """
     根据签名中的PatternArg，自动解析参数，并转换为对应类型，自动注入函数调用中
 
@@ -590,29 +640,32 @@
     alias: str = command_kwargs["alias"]
     context: Dict = command_kwargs["context"]
 
     # TODO 性能优化
     # if not cache.compressed_patterns:
     #     return method_name,{}
 
-    main_parser = class_command_cache.parser
+    # 需要根据当前的method_name，判断用哪个parser来解析
+    parser = class_command_cache.method_name_parser_mapping[method_name]
 
     # message_chain转为str(json.dumps，不带空格)，去掉prefix
     prefix_with_alias = prefix + alias
     # compressed_segments = merge_adjacent_text_segments(chain.segments)
     chain_str = await downgrade_segment_to_str(chain.segments, event_metadata.protocol)
     without_prefix = chain_str.replace(prefix_with_alias, "", 1).strip()
 
     # debug(chain_str)
     # debug(without_prefix)
 
     splitted_args = without_prefix.split()
 
     try:
-        args = main_parser.parse_args(splitted_args)
+        # args = parser.parse_args(splitted_args)
+        args, unknown_args = parser.parse_known_args(splitted_args)
+
         args_dict = vars(args)
 
         # debug(args_dict)
 
         # 考虑到alias(command_final_name)的问题
         target_method = args_dict[ARGPARSE_CALLED_METHOD]
```

### Comparing `pepperbot-0.3.5/pepperbot/extensions/command/sender.py` & `pepperbot-0.3.6/pepperbot/extensions/command/sender.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.5/pepperbot/extensions/log/__init__.py` & `pepperbot-0.3.6/pepperbot/extensions/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.5/pepperbot/initial.py` & `pepperbot-0.3.6/pepperbot/initial.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,26 +10,26 @@
 from pepperbot.core.route.utils import (
     create_bot_routes,
     create_web_routes,
     http_receiver,
     websocket_receiver,
 )
 from pepperbot.exceptions import InitializationError
-from pepperbot.extensions.command.handle import check_command_timeout
+from pepperbot.extensions.command.timeout import check_command_timeout
 from pepperbot.extensions.log import debug_log, logger
 from pepperbot.extensions.scheduler import async_scheduler
-from pepperbot.store.orm import engine, metadata, set_metadata
 from pepperbot.store.meta import (
     DEFAULT_URI,
     BotRoute,
+    api_callers,
     clean_bot_instances,
     output_config,
-    api_callers,
     register_routes,
 )
+from pepperbot.store.orm import database, engine, metadata, set_metadata
 from pepperbot.types import BOT_PROTOCOLS, T_BotProtocol, T_WebProtocol
 
 # from dotenv import load_dotenv
 # import os
 
 sanic_app = Sanic("PepperBot")
 
@@ -75,27 +75,32 @@
         if bot_protocol not in BOT_PROTOCOLS:
             raise InitializationError(f"尚不支持的机器人协议 {bot_protocol}")
 
         if receive_uri:
             uri = receive_uri
         else:
             if receive_protocol == "http":
-                # TODO lambda重名问题，动态创建
-                request_handler = lambda request: http_receiver(request, bot_protocol)
                 uri = DEFAULT_URI[bot_protocol] + "/http"
 
             elif receive_protocol == "websocket":
-                request_handler = lambda request, ws: websocket_receiver(
-                    request, ws, bot_protocol
-                )
                 uri = DEFAULT_URI[bot_protocol] + "/ws"
 
             else:
                 raise InitializationError(f"未知通信协议 {receive_protocol}")
 
+        if receive_protocol == "http":
+            # TODO lambda重名问题，动态创建
+            # 这个此时是receive_uri重复，可以在文档中说明
+            request_handler = lambda request: http_receiver(request, bot_protocol)
+
+        elif receive_protocol == "websocket":
+            request_handler = lambda request, ws: websocket_receiver(
+                request, ws, bot_protocol
+            )
+
         create_web_routes(
             sanic_app,
             receive_protocol=receive_protocol,
             uri=uri,
             request_handler=request_handler,
         )
 
@@ -149,42 +154,51 @@
         global async_create_telegram_handler
         async_create_telegram_handler = create_client_under_async_context
 
     def register_plugin(self) -> None:
         pass
 
     def apply_routes(self, routes: Iterable[BotRoute]):
-        create_bot_routes([*routes, *register_routes])
+        try:
+            create_bot_routes([*routes, *register_routes])
+
+        except InitializationError as e:  # 不显示整个traceback，只显示错误信息就行了
+            logger.error(e)
+            exit(1)
 
     def share_state_command(self):
         pass
 
     @staticmethod
     async def main_process_start(app, loop):
         """
         https://sanic.dev/en/guide/basics/listeners.html#asgi-mode
 
         If you are running your application with an ASGI server, main_process_start and main_process_stop will be ignored
         """
 
-
         # TODO 在各adapter初始化完成之后，再获取
         # 所以需要实现一个hook，after_adapter_init
 
         # main process、worker process都需要读取.env
         # 主动读取一次，这样即使用户定义的BaseSetting中没有制定env_file，也能读取到
         # load_dotenv()  # take environment variables from .env.
         logger.success(
             f"PepperBot successfully load .env config \n {pformat(global_config)}"
         )
 
         logger.success(f"PepperBot successfully create bot routes")
         # output_config()
         # debug(per_worker)
 
+        # https://collerek.github.io/ormar/fastapi/#database-connection
+        if "sqlite" not in global_config.database.url:
+            if not database.is_connected:
+                await database.connect()
+
         # 必须放到最后，等model都定义好了再执行
         # note that this has to be the same metadata that is used in ormar Models definition
         metadata.create_all(engine)
         # TODO 主动获取bot info
         await set_metadata("has_initial_bot_info", False)
         # 保证过期(无效)的command status一定被清理，不会干扰has_running_command的判断
         await check_command_timeout()
```

### Comparing `pepperbot-0.3.5/pepperbot/store/command.py` & `pepperbot-0.3.6/pepperbot/store/command.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,17 +17,19 @@
     Sequence,
     Tuple,
     Type,
     TypeVar,
     Union,
     cast,
 )
+import typing
 from uuid import uuid4
 
 import ormar
+from apscheduler.job import Job
 from pydantic import BaseModel, Field
 from typing_extensions import get_args
 
 # if TYPE_CHECKING:
 # field "chain" not yet prepared so type is still a ForwardRef, you might need to call HistoryItem.update_forward_refs().
 # pydantic需要用到
 from pepperbot.core.message.chain import MessageChain
@@ -198,32 +200,61 @@
 
 
 class ClassCommandMethodCache(BaseModel):
     class Config:
         arbitrary_types_allowed = True
 
     method: Callable
-    pattern_args: OrderedDict[str, _PatternArg] = OrderedDict()
+    pattern_args: typing.OrderedDict[str, _PatternArg] = Field(
+        default_factory=OrderedDict
+    )
     help_message: Optional[str] = None
-    """ sub command的help message """
+    """ command的help message """
     command_stack: List[str] = []
-    """ 对于nest command来说，就是从initial => sub command => sub sub command的顺序，
-    用于处理argparse的解析结果 """
+    """ 对于nest， root command => sub command => sub sub command的顺序
+
+    用于处理argparse的解析结果 
+    
+    至少包含自己
+    """
+
+    is_root: bool = False
+    """ 是否是root command """
+    parser: Optional[ArgumentParser] = None
+    """ 如果是root command，就是自己的parser"""
 
 
 class ClassCommandCache(BaseModel):
     class Config:
         arbitrary_types_allowed = True
 
     class_instance: Any
     command_method_mapping: Dict[str, ClassCommandMethodCache] = {}
     """ key为方法名，value为实例化后的方法 """
-    parser: ArgumentParser
-    help_message: Optional[str] = None
-    """ 存储help message，此处为总览"""
+
+    method_name_parser_mapping: Dict[str, ArgumentParser] = {}
+    """ key为方法名，value为parser 
+
+    - a(initial)
+        - b
+            - d
+            - e
+        - c
+            - f
+            - g
+    - h(非initial、非sub command，另一个根command)
+        - i
+        - j
+    
+    
+    则b、d、e、c、f、g的parser都是a的parser
+    而i、j的parser是h的parser
+
+    需要包含a、h自己的对应
+    """
 
 
 DOWNGRADE_PATTERN_FORMAT = "__{type_}:{id_}__"
 DOWNGRADE_PATTERN = re.compile(r"__(\w+):(.*)__")
 
 
 class ClassCommandConfigCache(BaseModel):
@@ -252,15 +283,15 @@
     class Meta:
         tablename = "class_command_status"
         database = database
         metadata = metadata
 
     id: int = cast(int, ormar.Integer(primary_key=True))
 
-    command_name = cast(str, ormar.String(max_length=50))
+    command_name: str = cast(str, ormar.String(max_length=50))
     config_id: str = cast(str, ormar.String(max_length=50))
     protocol: T_BotProtocol = cast(T_BotProtocol, ormar.String(max_length=50))
     conversation_type: str = cast(str, ormar.String(max_length=50))
     conversation_id: str = cast(str, ormar.String(max_length=50))
     user_id: str = cast(str, ormar.String(max_length=50))
 
     pointer: str = cast(str, ormar.String(max_length=50, default="initial"))
@@ -272,7 +303,14 @@
     )
     context: bytes = ormar.LargeBinary(max_length=100000, default=pickle.dumps({}))
 
     """ 用户定义，method之间的消息传递方式 """
     last_updated_time: float = cast(float, ormar.Float(default=time.time))
     """ 用来判断timeout """
     timeout: int = cast(int, ormar.Integer())
+
+
+command_timeout_jobs: Dict[int, Job] = {}
+""" 
+
+{ command_status_id : job }
+ """
```

### Comparing `pepperbot-0.3.5/pepperbot/store/event.py` & `pepperbot-0.3.6/pepperbot/store/event.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Literal, Optional, Sequence, Set
+from typing import Any, List, Literal, Optional, Sequence, Set
 from pydantic import BaseModel
 
 from pepperbot.types import T_BotProtocol, T_ConversationType, T_DispatchHandler
 
 
 class EventHandlerKwarg(BaseModel):
     name: str
@@ -36,15 +36,15 @@
 
     def __hash__(self):
         return hash(self.protocol_event_name)
 
 
 def filter_event_by_type(
     events: Sequence[ProtocolEvent], target_event_types: Sequence[T_EventType]
-) -> list[ProtocolEvent]:
+) -> List[ProtocolEvent]:
     results: Set[ProtocolEvent] = set()
 
     for event in events:
         for event_type in event.event_type:
             if event_type in target_event_types:
                 results.add(event)
```

### Comparing `pepperbot-0.3.5/pepperbot/store/meta.py` & `pepperbot-0.3.6/pepperbot/store/meta.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
 """每个worker进程都需要独立进行的初始化工作"""
 
 
 register_routes: List[BotRoute] = []
 """ 通过register装饰器注册的class_handler """
 
 route_mapping: Dict[
-    tuple[
+    Tuple[
         Union[T_BotProtocol, Literal["validator"]],
         T_ConversationType,
         str,
         T_HandlerType,
     ],
     Set[str],
 ] = defaultdict(set)
```

### Comparing `pepperbot-0.3.5/pepperbot/store/orm.py` & `pepperbot-0.3.6/pepperbot/store/orm.py`

 * *Files 10% similar despite different names*

```diff
@@ -81,7 +81,30 @@
     await set_value_from(Metadata, key, value)
 
 
 async def set_value(key: str, value: Any) -> None:
     """设置键值对形式的数据"""
 
     await set_value_from(Share, key, value)
+
+
+async def delete_value_from(model: Type[ormar.Model], key: str) -> None:
+    """删除键值对形式的数据"""
+
+    try:
+        column = await model.objects.get(key=key)
+        await column.delete()
+
+    except ormar.NoMatch:
+        pass
+
+
+async def delete_metadata(key: str) -> None:
+    """删除键值对形式的数据"""
+
+    await delete_value_from(Metadata, key)
+
+
+async def delete_value(key: str) -> None:
+    """删除键值对形式的数据"""
+
+    await delete_value_from(Share, key)
```

### Comparing `pepperbot-0.3.5/pepperbot/types.py` & `pepperbot-0.3.6/pepperbot/types.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.5/pepperbot/utils/common.py` & `pepperbot-0.3.6/pepperbot/utils/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import asyncio
+import contextvars
+import functools
 import inspect
 from inspect import iscoroutine
 from types import FunctionType
 from typing import Any, Callable, Coroutine, Dict, List, Union, cast
 
 from devtools import debug
 from pydantic import BaseModel
@@ -40,14 +42,21 @@
     """从method上获取class name"""
 
     # debug(method.__qualname__)
 
     return method.__qualname__.split(".")[0]
 
 
+async def to_thread(func, /, *args, **kwargs):
+    loop = asyncio.get_running_loop()
+    ctx = contextvars.copy_context()
+    func_call = functools.partial(ctx.run, func, *args, **kwargs)
+    return await loop.run_in_executor(None, func_call)
+
+
 async def await_or_sync(obj: Union[Any, FunctionType], *args, **kwargs) -> Any:
     """
     针对bound method，iscoroutine和isawaitable对bound method无效
 
     判断__func__也不行
     """
 
@@ -62,15 +71,15 @@
     ):
         # debug("coroutine")
         result = await obj(*args, **kwargs)  # type: ignore
         return result
     else:
         if callable(obj):
             # debug("sync")
-            result = await asyncio.to_thread(obj, *args, **kwargs)
+            result = await to_thread(obj, *args, **kwargs)
             # loop = asyncio.get_event_loop()
             # with_kwargs = functools.partial(functionOrCoroutine, *args, **kwargs)
 
             # result = await loop.run_in_executor(None, with_kwargs)
             return result
         else:
             return None
```

### Comparing `pepperbot-0.3.5/pyproject.toml` & `pepperbot-0.3.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -38,16 +38,16 @@
     "qq",
     "type-annotations",
     "type-hint",
     "wechat",
 ]
 name = "pepperbot"
 readme = "README.md"
-requires-python = ">=3.10"
-version = "0.3.5"
+requires-python = ">=3.8"
+version = "0.3.6"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 documentation = "https://SSmJaE.github.io/PepperBot"
 homepage = "https://github.com/SSmJaE/PepperBot"
@@ -70,13 +70,13 @@
     "pytest-asyncio>=0.21.0",
     "pytest-cov>=4.0.0",
     "pytest-mock>=3.10.0",
     "pytest>=7.2.2",
 ]
 
 [tool.pdm.scripts]
-badge = "pytest --cov-report xml --cov-branch --cov=pepperbot ./tests/command/test_parse.py && deactive && genbadge coverage -i ./coverage.xml "
+badge = "pytest --cov-report xml --cov-branch --cov=pepperbot ./tests -l -v && genbadge coverage -i ./coverage.xml -o ./archive/coverage-badge.svg "
 run = "python private/run.py"
-test = "pytest --cov-report html --cov-branch --cov=pepperbot ./tests"
+test = "pytest --cov-report html --cov-branch --cov=pepperbot ./tests -l -v"
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
```

### Comparing `pepperbot-0.3.5/tests/command/test_cli_argument.py` & `pepperbot-0.3.6/tests/command/test_cli_argument.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pepperbot.core.event.handle import handle_event
 from pepperbot.core.message.segment import Image, Text
 from pepperbot.extensions.command import as_command
 from pepperbot.extensions.command.sender import CommandSender
 from pepperbot.initial import PepperBot
 from pepperbot.store.command import CLIArgument
 from pepperbot.store.meta import BotRoute
-from tests.conftest import results
+from tests.conftest import api_results
 from tests.utils import fake_group_event
 
 
 @as_command(
     need_prefix=True,
     prefixes=["/"],
     include_class_name=True,
@@ -117,14 +117,15 @@
 
     bot.register_adapter(
         bot_protocol="onebot",
         receive_protocol="http",
         backend_protocol="http",
         backend_host="127.0.0.1",
         backend_port=5700,
+        receive_uri=f"/test_cli_argument/",
     )
 
     bot.apply_routes(
         [
             BotRoute(
                 commands=(
                     PositionalBaseType,
@@ -165,16 +166,16 @@
                     },
                 },
             ),
         )
 
         # debug(results)
 
-        action = results[0][0]
-        content = results[0][1]["message"][0]["data"]["text"]
+        action = api_results[0][0]
+        content = api_results[0][1]["message"][0]["data"]["text"]
 
         assert action == "send_group_msg" and content == "test"
 
     async def test_positional_segment_type(self):
         """测试segment类型的位置参数"""
 
         file_path = "https://i0.hdslb.com/1.jpg"
@@ -188,16 +189,16 @@
                         "text": "/PositionalSegmentType",
                     },
                 },
                 Image(file_path),
             ),
         )
 
-        action = results[0][0]
-        content = results[0][1]["message"][0]["data"]["text"]
+        action = api_results[0][0]
+        content = api_results[0][1]["message"][0]["data"]["text"]
 
         assert action == "send_group_msg" and content == file_path
 
     async def test_positional_any_type_base(self):
         """测试Any类型的位置参数"""
 
         await handle_event(
@@ -210,16 +211,16 @@
                     },
                 },
             ),
         )
 
         # debug(results)
 
-        action = results[0][0]
-        content = results[0][1]["message"][0]["data"]["text"]
+        action = api_results[0][0]
+        content = api_results[0][1]["message"][0]["data"]["text"]
 
         assert action == "send_group_msg" and content == "str"
 
     async def test_positional_any_type_segment(self):
         file_path = "https://i0.hdslb.com/1.jpg"
 
         await handle_event(
@@ -231,16 +232,16 @@
                         "text": "/PositionalAnyType",
                     },
                 },
                 Image(file_path),
             ),
         )
 
-        action = results[0][0]
-        content = results[0][1]["message"][0]["data"]["text"]
+        action = api_results[0][0]
+        content = api_results[0][1]["message"][0]["data"]["text"]
 
         assert action == "send_group_msg" and content == "Image"
 
     async def test_positional_wrong_type(self):
         """测试错误类型的位置参数"""
 
         await handle_event(
@@ -252,16 +253,16 @@
                         "text": "/PositionalBaseType",
                     },
                 },
                 Image("https://i0.hdslb.com/1.jpg"),
             ),
         )
 
-        action = results[0][0]
-        content = results[0][1]["message"][0]["data"]["text"]
+        action = api_results[0][0]
+        content = api_results[0][1]["message"][0]["data"]["text"]
 
         assert action == "send_group_msg" and "参数解析失败" in content
 
     async def test_multi_positional_base_type(self):
         strings = ["1", "2", "3", "4", "5"]
         space_joined = " ".join(strings)
 
@@ -273,16 +274,16 @@
                     "data": {
                         "text": f"/MultiPositionalBaseType {space_joined}",
                     },
                 },
             ),
         )
 
-        action = results[0][0]
-        content = results[0][1]["message"][0]["data"]["text"]
+        action = api_results[0][0]
+        content = api_results[0][1]["message"][0]["data"]["text"]
 
         assert action == "send_group_msg" and content == space_joined
 
     async def test_multi_positional_segment_type(self):
         segments = [
             Image("https://i0.hdslb.com/1.jpg"),
             Image("https://i0.hdslb.com/2.jpg"),
@@ -301,16 +302,16 @@
                         "text": f"/MultiPositionalSegmentType",
                     },
                 },
                 *segments,
             ),
         )
 
-        action = results[0][0]
-        content = results[0][1]["message"][0]["data"]["text"]
+        action = api_results[0][0]
+        content = api_results[0][1]["message"][0]["data"]["text"]
 
         assert action == "send_group_msg" and content == space_joined
 
     @pytest.mark.parametrize("argument", ["", "123"], ids=["empty", "not_empty"])
     async def test_optional_positional(self, argument):
         await handle_event(
             "onebot",
@@ -320,16 +321,16 @@
                     "data": {
                         "text": f"/OptionalPositionalSingle {argument}",
                     },
                 },
             ),
         )
 
-        action = results[0][0]
-        content = results[0][1]["message"][0]["data"]["text"]
+        action = api_results[0][0]
+        content = api_results[0][1]["message"][0]["data"]["text"]
 
         assert (
             action == "send_group_msg" and content == "None"
             if argument == ""
             else argument
         )
 
@@ -349,16 +350,16 @@
                     },
                 },
             ),
         )
 
         # debug(results)
 
-        action = results[0][0]
-        content = results[0][1]["message"][0]["data"]["text"]
+        action = api_results[0][0]
+        content = api_results[0][1]["message"][0]["data"]["text"]
 
         assert (
             action == "send_group_msg" and content == "None"
             if argument == [""]
             else space_joined
         )
 
@@ -376,16 +377,16 @@
                     "data": {
                         "text": f"/DefaultPositionalSingle {argument}",
                     },
                 },
             ),
         )
 
-        action = results[0][0]
-        content = results[0][1]["message"][0]["data"]["text"]
+        action = api_results[0][0]
+        content = api_results[0][1]["message"][0]["data"]["text"]
 
         assert (
             action == "send_group_msg" and content == default
             if argument == ""
             else argument
         )
 
@@ -405,16 +406,16 @@
                     "data": {
                         "text": f"/DefaultPositionalMulti {space_joined}",
                     },
                 },
             ),
         )
 
-        action = results[0][0]
-        content = results[0][1]["message"][0]["data"]["text"]
+        action = api_results[0][0]
+        content = api_results[0][1]["message"][0]["data"]["text"]
 
         assert action == "send_group_msg" and content == space_joined
 
     # single multi empty not_empty
     async def test_required_optional(self):
         pass
```

### Comparing `pepperbot-0.3.5/tests/command/test_merge.py` & `pepperbot-0.3.6/tests/command/test_merge.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.5/tests/conftest.py` & `pepperbot-0.3.6/tests/conftest.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,18 @@
 import asyncio
 import contextlib
 import pytest
 
-from typing import Any
-from devtools import debug
+from typing import Any, Optional, cast
 import pytest
-from pytest_mock import MockerFixture
-from capabilities.pepperbot_gpt_example.src.config import GPTExampleConfig
-from capabilities.pepperbot_gpt_example.src.main import GPTExample, GPTManage
-from pepperbot.core.api.api_caller import ApiCaller
-from pepperbot.core.event.handle import handle_event
-from pepperbot.core.message.segment import Image
-from pepperbot.extensions.command import as_command
-from pepperbot.initial import PepperBot
-from pepperbot.store.meta import BotRoute, get_onebot_caller, onebot_event_meta
-from pepperbot.store.orm import engine, metadata, set_metadata
+from pepperbot.store.meta import onebot_event_meta
+from pepperbot.store.orm import engine, metadata, database
 from pepperbot.config import global_config
 import os
-import sys
+
 
 from unittest.mock import patch
 
 # 可以直接import tests.conftest
 # base_dir = os.path.dirname(os.path.abspath(__file__))
 # sys.path.append(base_dir)
 
@@ -33,28 +24,41 @@
     loop = policy.new_event_loop()
     yield loop
     loop.close()
 
 
 @pytest.fixture(scope="session", autouse=True)
 async def setup_test_environment():
-    global_config.logger.level = 10
     # debug(global_config)
 
+    global_config.logger.level = 10
+
     onebot_event_meta.has_skip_buffered_event = True
 
-    db_path = global_config.database.url.split("///")[1]
-    if os.path.exists(db_path):
-        os.remove(db_path)
+    db_path: Optional[str] = None
+
+    if "sqlite" in global_config.database.url:
+        db_path = global_config.database.url.split("///")[1]
+        if os.path.exists(db_path):
+            os.remove(db_path)
+
+    else:
+        if not database.is_connected:
+            await database.connect()
 
     metadata.create_all(engine)
 
     yield
 
-    os.remove(db_path)
+    if "sqlite" in global_config.database.url:
+        os.remove(cast(str, db_path))
+
+    else:
+        if database.is_connected:
+            await database.disconnect()
 
 
 @pytest.fixture(scope="function")
 async def reset_database():
     yield
 
     # 清空数据库
@@ -63,23 +67,24 @@
         for table in reversed(metadata.sorted_tables):
             con.execute(table.delete())
         trans.commit()
 
     # metadata.drop_all(engine)
 
 
-results = []
+api_results = []
 
 
 def new_caller(self, action: str, kwargs: dict[str, Any]):
-    results.append((action, kwargs))
-
     if action == "get_login_info":
         return {"user_id": "123456789", "nickname": "测试机器人"}
 
+    else:
+        api_results.append((action, kwargs))
+
 
 @pytest.fixture(scope="class")
 def patch_api_caller():
     with patch(
         "pepperbot.core.api.api_caller.ApiCaller.to_onebot",
         new=new_caller,
         # create=True,
@@ -87,8 +92,8 @@
         yield patched
 
 
 @pytest.fixture(scope="function")
 def reset_api_results():
     yield
 
-    results.clear()
+    api_results.clear()
```

### Comparing `pepperbot-0.3.5/tests/core/test_available.py` & `pepperbot-0.3.6/tests/core/test_available.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,8 @@
 class TestAvailable:
-    async def test_root_validator(self):
-        """测试根验证器"""
-        pass
-
     async def test_class_handler(self):
         """测试类处理器"""
         pass
 
     async def test_class_command(self):
         """测试类命令"""
         pass
```

### Comparing `pepperbot-0.3.5/tests/message/test_chain.py` & `pepperbot-0.3.6/tests/message/test_chain.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import pytest
 from pepperbot.core.message.chain import MessageChain
 from pepperbot.core.message.segment import *
 
 
 mock_event = {
     "message_id": 12345,
     "message": [
@@ -9,41 +10,56 @@
         {"type": "text", "data": {"text": "word word"}},
         {"type": "text", "data": {"text": "word word2"}},
     ],
 }
 mock_event2 = {"message_id": 7238908, "message": []}
 
 chain = MessageChain("onebot", "group", mock_event, "123456789", "987654321")
+
+
 chain2 = MessageChain("onebot", "group", mock_event2, "123456789", "987654321")
 
-assert chain != chain2
 
-#
-assert chain.pure_text == "word wordword word2", "pure_text应只包含Text类型的内容"
-# 字符串可以直接in
-assert "word" in chain
-# 只取pure_text
-assert "123" not in chain
-# 可以判断是否指定类型
-assert Text in chain
-assert chain.has(Text) == True
-# 可以判断是否指定类型的实例
-assert Text("word2") not in chain
-assert Text("word word") in chain
-assert chain.has(Text("word word")) == True
-assert chain.has(Text("word word1")) == False
-assert chain.has(OnebotFace(123)) == True
-assert chain.has(OnebotFace(124)) == False
-assert chain.has(OnebotFace(123)) == True, "如果从后端传入的数据未经过Pydantic类型转换"
-# 快捷方式
-assert chain.has_and_first(Text) == (True, Text("word word"))
-assert chain.has_and_last(Text) == (True, Text("word word2"))
-assert chain.has_and_all(Text) == (True, [Text("word word"), Text("word word2")])
-# 获取所有指定类型实例
-assert chain.onebot_faces == [OnebotFace(123)]
-assert chain.text == [Text("word word"), Text("word word2")]
-# 按index取Segment
-assert chain[1] == Text("word word")
-
-# 可以直接判断实例
-assert Text("word word") == Text("word word")
-assert Text("word word") != Text("word word2")
+@pytest.fixture(scope="class")
+async def construct_chain():
+    await chain.construct()
+    await chain2.construct()
+
+
+@pytest.mark.usefixtures("construct_chain")
+class TestMessageChain:
+    async def test_chain_equal(self):
+        assert chain != chain2
+
+    async def test_pure_text(self):
+        assert chain.pure_text == "word wordword word2", "pure_text应只包含Text类型的内容"
+
+    async def test_has_item(self):
+        # 字符串可以直接in
+        assert "word" in chain
+        # 只取pure_text
+        assert "123" not in chain
+        # 可以判断是否指定类型
+        assert Text in chain
+        assert chain.has(Text) == True
+        # 可以判断是否指定类型的实例
+        assert Text("word2") not in chain
+        assert Text("word word") in chain
+        assert chain.has(Text("word word")) == True
+        assert chain.has(Text("word word1")) == False
+        assert chain.has(OnebotFace(123)) == True
+        assert chain.has(OnebotFace(124)) == False
+        assert chain.has(OnebotFace(123)) == True, "如果从后端传入的数据未经过Pydantic类型转换"
+        # 快捷方式
+        assert chain.has_and_first(Text) == (True, Text("word word"))
+        assert chain.has_and_last(Text) == (True, Text("word word2"))
+        assert chain.has_and_all(Text) == (
+            True,
+            [Text("word word"), Text("word word2")],
+        )
+
+    async def test_get_items(self):
+        # 获取所有指定类型实例
+        assert chain.onebot_faces == [OnebotFace(123)]
+        assert chain.text == [Text("word word"), Text("word word2")]
+        # 按index取Segment
+        assert chain[1] == Text("word word")
```

### Comparing `pepperbot-0.3.5/tests/tree.py` & `pepperbot-0.3.6/tests/tree.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.5/tests/utils.py` & `pepperbot-0.3.6/tests/utils.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.5/PKG-INFO` & `pepperbot-0.3.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pepperbot
-Version: 0.3.5
+Version: 0.3.6
 Summary: An intuitive multi-platform bot framework, easily forward messages among platforms, support QQ, WeChat, Telegram. 一个符合直觉的跨社交平台机器人框架，轻松地在平台间传递消息，支持QQ、微信、Telegram
 Keywords: Telegram async asyncio bot chinese cqhttp cross-platform framework keaimao onebot pydantic pyrogram python qq type-annotations type-hint wechat
 Home-page: https://github.com/SSmJaE/PepperBot
 Author-Email: SSmJaE <ssmjae327@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python
 Project-URL: Documentation, https://SSmJaE.github.io/PepperBot
 Project-URL: Homepage, https://github.com/SSmJaE/PepperBot
 Project-URL: Repository, https://github.com/SSmJaE/PepperBot
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Requires-Dist: Pyrogram>=2.0.102
 Requires-Dist: TgCrypto>=1.2.5
 Requires-Dist: apscheduler>=3
 Requires-Dist: arrow>=1.2.3
 Requires-Dist: better-exceptions>=0.3.3
 Requires-Dist: devtools>=0.10.0
 Requires-Dist: httpx>=0.23.3
@@ -36,14 +36,18 @@
 <p align="center">
 <a href="https://ssmjae.github.io/PepperBot/">文档</a> ·
 <a href="https://jq.qq.com/?_wv=1027&k=EPhcRRib">QQ交流群</a>  
 </p>
 
 <p align="center">
 <img src="./archive/coverage-badge.svg" />
+<img src="https://badge.fury.io/py/pepperbot.svg" />
+<img src="https://img.shields.io/badge/python-3.8+-blue.svg" />
+<img src="https://static.pepy.tech/badge/pepperbot/month" />
+
 </p>
 
 ## 生而跨平台
 
 - QQ 基于 `Onebot`，`Mirai`(待实现)、`OPQ`(待实现)
 - 微信基于`可爱猫`
 - Telegram基于`Pyrogram`
@@ -76,23 +80,24 @@
 - 基于 python3.6 之后的类型注解，提供了完全的类型提示
 - 大部分可以自动获取的参数，都会自动获取，不需要每次手动提供了
 - 只会动态注入用到的参数，没必要每次写一长串用不到的参数了！
 - 文档中，均有可直接复制使用的代码片段，快速开发
 
 ## 测试文档全
 
-- 通过元编程(AST 之类)手段，对编写的各种代码进行规则检查，并输出易于理解的错误信息，将问题消灭在框架启动之前
+- 自带linter
+  - 通过元编程(AST 之类)手段，对编写的各种代码进行规则检查，并输出易于理解的错误信息，将问题消灭在框架启动之前
 - 文档比较全
 - 测试覆盖比较全面
 - 大量官方示例/指令
 - 来自作者的 QA(加群以获取)
 
 ## 安装
 
-目前只能3.10及以上，因为用了点新特性，之后会恢复对3.8的支持
+TODO 目前只能3.10及以上，因为用了点新特性，之后会恢复对3.8的支持
 
 ```bash
 pip install pepperbot
 ```
 
 ## 使用
 
@@ -140,12 +145,14 @@
                 Text("没人"),
                 Image("http://123.jpg"),
             )
 ```
 
 ## 生态
 
+[插件市场](https://ssmjae.github.io/PepperBot/market/)
+
 ### 可以记忆上下文的GPT群聊机器人
 
-[PepperBot-GPT]( )
+[pepperbot-ai-query](https://github.com/SSmJaE/PepperBot/tree/master/capabilities/pepperbot_gpt_example )
 
 ### 通过GPT，自动检测群聊中的广告信息
```

