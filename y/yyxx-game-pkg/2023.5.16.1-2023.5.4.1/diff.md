# Comparing `tmp/yyxx_game_pkg-2023.5.16.1.tar.gz` & `tmp/yyxx_game_pkg-2023.5.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yyxx_game_pkg-2023.5.16.1.tar", max compression
+gzip compressed data, was "yyxx_game_pkg-2023.5.4.1.tar", max compression
```

## Comparing `yyxx_game_pkg-2023.5.16.1.tar` & `yyxx_game_pkg-2023.5.4.1.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0     3888 2023-05-16 03:53:46.549778 yyxx_game_pkg-2023.5.16.1/README.md
--rw-r--r--   0        0        0     1170 2023-05-16 03:53:57.465959 yyxx_game_pkg-2023.5.16.1/pyproject.toml
--rw-r--r--   0        0        0       68 2023-05-16 03:53:46.549778 yyxx_game_pkg-2023.5.16.1/tests/__init__.py
--rw-r--r--   0        0        0       83 2023-05-16 03:53:46.549778 yyxx_game_pkg-2023.5.16.1/tests/dbops/__init__.py
--rw-r--r--   0        0        0     1341 2023-05-16 03:53:46.549778 yyxx_game_pkg-2023.5.16.1/tests/dbops/mysql_op.py
--rw-r--r--   0        0        0       70 2023-05-16 03:53:46.549778 yyxx_game_pkg-2023.5.16.1/tests/dispatch/__init__.py
--rw-r--r--   0        0        0       70 2023-05-16 03:53:46.549778 yyxx_game_pkg-2023.5.16.1/tests/dispatch/config/__init__.py
--rw-r--r--   0        0        0     1228 2023-05-16 03:53:46.549778 yyxx_game_pkg-2023.5.16.1/tests/dispatch/config/celery_local_config.py
--rw-r--r--   0        0        0      660 2023-05-16 03:53:46.549778 yyxx_game_pkg-2023.5.16.1/tests/dispatch/rules/__init__.py
--rw-r--r--   0        0        0     1348 2023-05-16 03:53:46.549778 yyxx_game_pkg-2023.5.16.1/tests/dispatch/rules/rule_temp.py
--rw-r--r--   0        0        0      580 2023-05-16 03:53:46.549778 yyxx_game_pkg-2023.5.16.1/tests/dispatch/test_dispatch.py
--rw-r--r--   0        0        0       84 2023-05-16 03:53:46.549778 yyxx_game_pkg-2023.5.16.1/tests/helpers/__init__.py
--rw-r--r--   0        0        0      522 2023-05-16 03:53:46.549778 yyxx_game_pkg-2023.5.16.1/tests/helpers/test_mysql_helper.py
--rw-r--r--   0        0        0      455 2023-05-16 03:53:46.549778 yyxx_game_pkg-2023.5.16.1/tests/helpers/test_pika_helper.py
--rw-r--r--   0        0        0      481 2023-05-16 03:53:46.549778 yyxx_game_pkg-2023.5.16.1/tests/helpers/test_redis_helper.py
--rw-r--r--   0        0        0       70 2023-05-16 03:53:46.549778 yyxx_game_pkg-2023.5.16.1/tests/submit/__init__.py
--rw-r--r--   0        0        0       70 2023-05-16 03:53:46.549778 yyxx_game_pkg-2023.5.16.1/tests/submit/schedule_rule/__init__.py
--rw-r--r--   0        0        0       70 2023-05-16 03:53:46.553778 yyxx_game_pkg-2023.5.16.1/tests/submit/schedule_rule/schedule/__init__.py
--rw-r--r--   0        0        0       70 2023-05-16 03:53:46.553778 yyxx_game_pkg-2023.5.16.1/tests/submit/schedule_rule/schedule/statistic_task/__init__.py
--rw-r--r--   0        0        0      431 2023-05-16 03:53:46.553778 yyxx_game_pkg-2023.5.16.1/tests/submit/schedule_rule/schedule/statistic_task/schedule_statistic_collect_test.py
--rw-r--r--   0        0        0      413 2023-05-16 03:53:46.553778 yyxx_game_pkg-2023.5.16.1/tests/submit/schedule_rule/schedule/statistic_task/schedule_statistic_task_test.py
--rw-r--r--   0        0        0       70 2023-05-16 03:53:46.553778 yyxx_game_pkg-2023.5.16.1/tests/submit/schedule_rule/schedule/work_flow/__init__.py
--rw-r--r--   0        0        0     1217 2023-05-16 03:53:46.553778 yyxx_game_pkg-2023.5.16.1/tests/submit/schedule_rule/schedule/work_flow/schedule_work_flow_test.py
--rw-r--r--   0        0        0      305 2023-05-16 03:53:46.553778 yyxx_game_pkg-2023.5.16.1/tests/submit/submit.json
--rw-r--r--   0        0        0     1250 2023-05-16 03:53:46.553778 yyxx_game_pkg-2023.5.16.1/tests/submit/test_submit.py
--rw-r--r--   0        0        0      235 2023-05-16 03:53:46.553778 yyxx_game_pkg-2023.5.16.1/tests/test_ip2region.py
--rw-r--r--   0        0        0      513 2023-05-16 03:53:46.553778 yyxx_game_pkg-2023.5.16.1/tests/test_logger.py
--rw-r--r--   0        0        0      960 2023-05-16 03:53:46.553778 yyxx_game_pkg-2023.5.16.1/tests/test_xtrace.py
--rw-r--r--   0        0        0       81 2023-05-16 03:53:46.553778 yyxx_game_pkg-2023.5.16.1/tests/utils/__init__.py
--rw-r--r--   0        0        0       70 2023-05-16 03:53:46.553778 yyxx_game_pkg-2023.5.16.1/tests/xcelery/__init__.py
--rw-r--r--   0        0        0       70 2023-05-16 03:53:46.553778 yyxx_game_pkg-2023.5.16.1/tests/xcelery/config/__init__.py
--rw-r--r--   0        0        0     1226 2023-05-16 03:53:46.553778 yyxx_game_pkg-2023.5.16.1/tests/xcelery/config/celery_local_config.py
--rw-r--r--   0        0        0      747 2023-05-16 03:53:46.553778 yyxx_game_pkg-2023.5.16.1/tests/xcelery/task_register.py
--rw-r--r--   0        0        0      299 2023-05-16 03:53:46.553778 yyxx_game_pkg-2023.5.16.1/tests/xcelery/test_celery.py
--rw-r--r--   0        0        0       69 2023-05-16 03:53:46.553778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/__init__.py
--rw-r--r--   0        0        0       83 2023-05-16 03:53:46.553778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/dbops/__init__.py
--rw-r--r--   0        0        0     1331 2023-05-16 03:53:46.553778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/dbops/base.py
--rw-r--r--   0        0        0     1295 2023-05-16 03:53:46.553778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/dbops/ch_op.py
--rw-r--r--   0        0        0     5597 2023-05-16 03:53:46.553778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/dbops/das_api.py
--rw-r--r--   0        0        0     1911 2023-05-16 03:53:46.553778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/dbops/es_op.py
--rw-r--r--   0        0        0     1678 2023-05-16 03:53:46.553778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/dbops/hdfs_op.py
--rw-r--r--   0        0        0      979 2023-05-16 03:53:46.553778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/dbops/mongo_op.py
--rw-r--r--   0        0        0     3955 2023-05-16 03:53:46.553778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/dbops/mysql_op.py
--rw-r--r--   0        0        0       81 2023-05-16 03:53:46.553778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/helpers/__init__.py
--rw-r--r--   0        0        0     2408 2023-05-16 03:53:46.553778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/helpers/mysql_helper.py
--rw-r--r--   0        0        0     1266 2023-05-16 03:53:46.553778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/helpers/pika_helper.py
--rw-r--r--   0        0        0     2850 2023-05-16 03:53:46.553778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/helpers/redis_helper.py
--rw-r--r--   0        0        0       79 2023-05-16 03:53:46.553778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/ip2region/__init__.py
--rw-r--r--   0        0        0 11070130 2023-05-16 03:53:46.617778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/ip2region/ip2region.xdb
--rw-r--r--   0        0        0      604 2023-05-16 03:53:46.617778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/ip2region/ip_x.py
--rw-r--r--   0        0        0     5735 2023-05-16 03:53:46.617778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/ip2region/xdbSearcher.py
--rw-r--r--   0        0        0       81 2023-05-16 03:53:46.617778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/logger/__init__.py
--rw-r--r--   0        0        0     2326 2023-05-16 03:53:46.617778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/logger/config.py
--rw-r--r--   0        0        0     3467 2023-05-16 03:53:46.617778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/logger/handlers.py
--rw-r--r--   0        0        0     2154 2023-05-16 03:53:46.617778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/logger/log.py
--rw-r--r--   0        0        0       70 2023-05-16 03:53:46.617778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/stat/__init__.py
--rw-r--r--   0        0        0       68 2023-05-16 03:53:46.617778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/stat/dispatch/__init__.py
--rw-r--r--   0        0        0       70 2023-05-16 03:53:46.617778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/stat/dispatch/common/__init__.py
--rw-r--r--   0        0        0     1514 2023-05-16 03:53:46.617778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/stat/dispatch/common/common.py
--rw-r--r--   0        0        0       69 2023-05-16 03:53:46.617778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/stat/dispatch/core/__init__.py
--rw-r--r--   0        0        0      805 2023-05-16 03:53:46.617778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/stat/dispatch/core/manager.py
--rw-r--r--   0        0        0     1042 2023-05-16 03:53:46.617778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/stat/dispatch/core/structs.py
--rw-r--r--   0        0        0     5533 2023-05-16 03:53:46.617778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/stat/dispatch/core/workflows.py
--rw-r--r--   0        0        0      604 2023-05-16 03:53:46.617778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/stat/dispatch/dispatch.py
--rw-r--r--   0        0        0       70 2023-05-16 03:53:46.617778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/stat/dispatch/logic/__init__.py
--rw-r--r--   0        0        0     4402 2023-05-16 03:53:46.617778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/stat/dispatch/logic/task_logic.py
--rw-r--r--   0        0        0      809 2023-05-16 03:53:46.617778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/stat/dispatch/route.py
--rw-r--r--   0        0        0      677 2023-05-16 03:53:46.617778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/stat/dispatch/rules/__init__.py
--rw-r--r--   0        0        0      689 2023-05-16 03:53:46.617778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/stat/dispatch/rules/rule_base.py
--rw-r--r--   0        0        0     4270 2023-05-16 03:53:46.617778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/stat/dispatch/rules/rule_workflow.py
--rw-r--r--   0        0        0      667 2023-05-16 03:53:46.617778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/stat/log.py
--rw-r--r--   0        0        0       70 2023-05-16 03:53:46.617778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/stat/submit/__init__.py
--rw-r--r--   0        0        0       70 2023-05-16 03:53:46.617778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/stat/submit/logic/__init__.py
--rw-r--r--   0        0        0     5961 2023-05-16 03:53:46.617778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/stat/submit/logic/submit_logic.py
--rw-r--r--   0        0        0      987 2023-05-16 03:53:46.617778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/stat/submit/submit.py
--rw-r--r--   0        0        0       70 2023-05-16 03:53:46.617778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/stat/xcelery/__init__.py
--rw-r--r--   0        0        0     2206 2023-05-16 03:53:46.617778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/stat/xcelery/instance.py
--rw-r--r--   0        0        0     1183 2023-05-16 03:53:46.617778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/stat/xcelery/task_base.py
--rw-r--r--   0        0        0       83 2023-05-16 03:53:46.617778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/utils/__init__.py
--rw-r--r--   0        0        0     5652 2023-05-16 03:53:46.617778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/utils/decorator.py
--rw-r--r--   0        0        0     2845 2023-05-16 03:53:46.617778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/utils/profiler.py
--rw-r--r--   0        0        0     3068 2023-05-16 03:53:46.617778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/utils/xListStr.py
--rw-r--r--   0        0        0     7305 2023-05-16 03:53:46.617778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/utils/xdataframe.py
--rw-r--r--   0        0        0     6161 2023-05-16 03:53:46.617778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/utils/xdate.py
--rw-r--r--   0        0        0     3091 2023-05-16 03:53:46.617778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/utils/xhttp.py
--rw-r--r--   0        0        0      971 2023-05-16 03:53:46.617778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/utils/xmath.py
--rw-r--r--   0        0        0       69 2023-05-16 03:53:46.617778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/xtrace/__init__.py
--rw-r--r--   0        0        0     2858 2023-05-16 03:53:46.617778 yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/xtrace/helper.py
--rw-r--r--   0        0        0     5506 1970-01-01 00:00:00.000000 yyxx_game_pkg-2023.5.16.1/PKG-INFO
+-rw-r--r--   0        0        0     3888 2023-05-04 04:10:07.938087 yyxx_game_pkg-2023.5.4.1/README.md
+-rw-r--r--   0        0        0     1170 2023-05-04 04:10:20.550173 yyxx_game_pkg-2023.5.4.1/pyproject.toml
+-rw-r--r--   0        0        0       68 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/__init__.py
+-rw-r--r--   0        0        0       83 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/dbops/__init__.py
+-rw-r--r--   0        0        0     1341 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/dbops/mysql_op.py
+-rw-r--r--   0        0        0       70 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/dispatch/__init__.py
+-rw-r--r--   0        0        0       70 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/dispatch/config/__init__.py
+-rw-r--r--   0        0        0     1228 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/dispatch/config/celery_local_config.py
+-rw-r--r--   0        0        0      660 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/dispatch/rules/__init__.py
+-rw-r--r--   0        0        0     1348 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/dispatch/rules/rule_temp.py
+-rw-r--r--   0        0        0      580 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/dispatch/test_dispatch.py
+-rw-r--r--   0        0        0       84 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/helpers/__init__.py
+-rw-r--r--   0        0        0      522 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/helpers/test_mysql_helper.py
+-rw-r--r--   0        0        0      455 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/helpers/test_pika_helper.py
+-rw-r--r--   0        0        0      481 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/helpers/test_redis_helper.py
+-rw-r--r--   0        0        0       70 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/submit/__init__.py
+-rw-r--r--   0        0        0       70 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/submit/schedule_rule/__init__.py
+-rw-r--r--   0        0        0       70 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/submit/schedule_rule/schedule/__init__.py
+-rw-r--r--   0        0        0       70 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/submit/schedule_rule/schedule/statistic_task/__init__.py
+-rw-r--r--   0        0        0      431 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/submit/schedule_rule/schedule/statistic_task/schedule_statistic_collect_test.py
+-rw-r--r--   0        0        0      413 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/submit/schedule_rule/schedule/statistic_task/schedule_statistic_task_test.py
+-rw-r--r--   0        0        0       70 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/submit/schedule_rule/schedule/work_flow/__init__.py
+-rw-r--r--   0        0        0     1217 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/submit/schedule_rule/schedule/work_flow/schedule_work_flow_test.py
+-rw-r--r--   0        0        0      305 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/submit/submit.json
+-rw-r--r--   0        0        0     1250 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/submit/test_submit.py
+-rw-r--r--   0        0        0      235 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/test_ip2region.py
+-rw-r--r--   0        0        0      513 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/test_logger.py
+-rw-r--r--   0        0        0      960 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/test_xtrace.py
+-rw-r--r--   0        0        0       81 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/utils/__init__.py
+-rw-r--r--   0        0        0       70 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/xcelery/__init__.py
+-rw-r--r--   0        0        0       70 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/xcelery/config/__init__.py
+-rw-r--r--   0        0        0     1226 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/xcelery/config/celery_local_config.py
+-rw-r--r--   0        0        0      747 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/xcelery/task_register.py
+-rw-r--r--   0        0        0      299 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/xcelery/test_celery.py
+-rw-r--r--   0        0        0       69 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/__init__.py
+-rw-r--r--   0        0        0       83 2023-05-04 04:10:07.946087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/dbops/__init__.py
+-rw-r--r--   0        0        0     1331 2023-05-04 04:10:07.946087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/dbops/base.py
+-rw-r--r--   0        0        0     1295 2023-05-04 04:10:07.946087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/dbops/ch_op.py
+-rw-r--r--   0        0        0     5597 2023-05-04 04:10:07.946087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/dbops/das_api.py
+-rw-r--r--   0        0        0     1911 2023-05-04 04:10:07.946087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/dbops/es_op.py
+-rw-r--r--   0        0        0     1678 2023-05-04 04:10:07.946087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/dbops/hdfs_op.py
+-rw-r--r--   0        0        0      979 2023-05-04 04:10:07.946087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/dbops/mongo_op.py
+-rw-r--r--   0        0        0     3955 2023-05-04 04:10:07.946087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/dbops/mysql_op.py
+-rw-r--r--   0        0        0       81 2023-05-04 04:10:07.946087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/helpers/__init__.py
+-rw-r--r--   0        0        0     2408 2023-05-04 04:10:07.946087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/helpers/mysql_helper.py
+-rw-r--r--   0        0        0     1266 2023-05-04 04:10:07.946087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/helpers/pika_helper.py
+-rw-r--r--   0        0        0     2850 2023-05-04 04:10:07.946087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/helpers/redis_helper.py
+-rw-r--r--   0        0        0       79 2023-05-04 04:10:07.946087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/ip2region/__init__.py
+-rw-r--r--   0        0        0 11070130 2023-05-04 04:10:08.018087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/ip2region/ip2region.xdb
+-rw-r--r--   0        0        0      604 2023-05-04 04:10:08.018087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/ip2region/ip_x.py
+-rw-r--r--   0        0        0     5735 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/ip2region/xdbSearcher.py
+-rw-r--r--   0        0        0       81 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/logger/__init__.py
+-rw-r--r--   0        0        0     2326 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/logger/config.py
+-rw-r--r--   0        0        0     3467 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/logger/handlers.py
+-rw-r--r--   0        0        0     2154 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/logger/log.py
+-rw-r--r--   0        0        0       70 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/__init__.py
+-rw-r--r--   0        0        0       68 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/__init__.py
+-rw-r--r--   0        0        0       70 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/common/__init__.py
+-rw-r--r--   0        0        0     1514 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/common/common.py
+-rw-r--r--   0        0        0       69 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/core/__init__.py
+-rw-r--r--   0        0        0      805 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/core/manager.py
+-rw-r--r--   0        0        0     1042 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/core/structs.py
+-rw-r--r--   0        0        0     5533 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/core/workflows.py
+-rw-r--r--   0        0        0      604 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/dispatch.py
+-rw-r--r--   0        0        0       70 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/logic/__init__.py
+-rw-r--r--   0        0        0     4402 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/logic/task_logic.py
+-rw-r--r--   0        0        0      809 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/route.py
+-rw-r--r--   0        0        0      677 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/rules/__init__.py
+-rw-r--r--   0        0        0      689 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/rules/rule_base.py
+-rw-r--r--   0        0        0     4270 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/rules/rule_workflow.py
+-rw-r--r--   0        0        0      667 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/log.py
+-rw-r--r--   0        0        0       70 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/submit/__init__.py
+-rw-r--r--   0        0        0       70 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/submit/logic/__init__.py
+-rw-r--r--   0        0        0     5961 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/submit/logic/submit_logic.py
+-rw-r--r--   0        0        0      987 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/submit/submit.py
+-rw-r--r--   0        0        0       70 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/xcelery/__init__.py
+-rw-r--r--   0        0        0     2206 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/xcelery/instance.py
+-rw-r--r--   0        0        0     1183 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/xcelery/task_base.py
+-rw-r--r--   0        0        0       83 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/utils/__init__.py
+-rw-r--r--   0        0        0     5652 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/utils/decorator.py
+-rw-r--r--   0        0        0     2845 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/utils/profiler.py
+-rw-r--r--   0        0        0     3068 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/utils/xListStr.py
+-rw-r--r--   0        0        0     6099 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/utils/xdataframe.py
+-rw-r--r--   0        0        0     6161 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/utils/xdate.py
+-rw-r--r--   0        0        0     3091 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/utils/xhttp.py
+-rw-r--r--   0        0        0      971 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/utils/xmath.py
+-rw-r--r--   0        0        0       69 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/xtrace/__init__.py
+-rw-r--r--   0        0        0     2858 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/xtrace/helper.py
+-rw-r--r--   0        0        0     5505 1970-01-01 00:00:00.000000 yyxx_game_pkg-2023.5.4.1/PKG-INFO
```

### Comparing `yyxx_game_pkg-2023.5.16.1/README.md` & `yyxx_game_pkg-2023.5.4.1/README.md`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/pyproject.toml` & `yyxx_game_pkg-2023.5.4.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 equires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "yyxx-game-pkg"
-version = "v2023.05.16.001"
+version = "v2023.05.04.001"
 description = "yyxx game custom module"
 authors = [ "yyxx-game",]
 license = "MIT"
 homepage = "https://github.com/yyxxgame/yyxxgame-pkg"
 repository = "https://github.com/yyxxgame/yyxxgame-pkg"
 readme = "README.md"
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",]
```

### Comparing `yyxx_game_pkg-2023.5.16.1/tests/dbops/mysql_op.py` & `yyxx_game_pkg-2023.5.4.1/tests/dbops/mysql_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/tests/dispatch/config/celery_local_config.py` & `yyxx_game_pkg-2023.5.4.1/tests/dispatch/config/celery_local_config.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/tests/dispatch/rules/__init__.py` & `yyxx_game_pkg-2023.5.4.1/tests/dispatch/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/tests/dispatch/rules/rule_temp.py` & `yyxx_game_pkg-2023.5.4.1/tests/dispatch/rules/rule_temp.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/tests/dispatch/test_dispatch.py` & `yyxx_game_pkg-2023.5.4.1/tests/dispatch/test_dispatch.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/tests/helpers/test_mysql_helper.py` & `yyxx_game_pkg-2023.5.4.1/tests/helpers/test_mysql_helper.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/tests/submit/schedule_rule/schedule/work_flow/schedule_work_flow_test.py` & `yyxx_game_pkg-2023.5.4.1/tests/submit/schedule_rule/schedule/work_flow/schedule_work_flow_test.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/tests/submit/test_submit.py` & `yyxx_game_pkg-2023.5.4.1/tests/submit/test_submit.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/tests/test_logger.py` & `yyxx_game_pkg-2023.5.4.1/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/tests/test_xtrace.py` & `yyxx_game_pkg-2023.5.4.1/tests/test_xtrace.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/tests/xcelery/config/celery_local_config.py` & `yyxx_game_pkg-2023.5.4.1/tests/xcelery/config/celery_local_config.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/tests/xcelery/task_register.py` & `yyxx_game_pkg-2023.5.4.1/tests/xcelery/task_register.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/dbops/base.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/dbops/base.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/dbops/ch_op.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/dbops/ch_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/dbops/das_api.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/dbops/das_api.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/dbops/es_op.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/dbops/es_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/dbops/hdfs_op.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/dbops/hdfs_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/dbops/mongo_op.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/dbops/mongo_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/dbops/mysql_op.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/dbops/mysql_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/helpers/mysql_helper.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/helpers/mysql_helper.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/helpers/pika_helper.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/helpers/pika_helper.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/helpers/redis_helper.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/helpers/redis_helper.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/ip2region/ip2region.xdb` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/ip2region/ip2region.xdb`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/ip2region/ip_x.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/ip2region/ip_x.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/ip2region/xdbSearcher.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/ip2region/xdbSearcher.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/logger/config.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/logger/config.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/logger/handlers.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/logger/handlers.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/logger/log.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/logger/log.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/stat/dispatch/common/common.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/common/common.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/stat/dispatch/core/manager.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/core/manager.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/stat/dispatch/core/structs.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/core/structs.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/stat/dispatch/core/workflows.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/core/workflows.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/stat/dispatch/dispatch.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/dispatch.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/stat/dispatch/logic/task_logic.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/logic/task_logic.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/stat/dispatch/route.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/route.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/stat/dispatch/rules/__init__.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/stat/dispatch/rules/rule_base.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/rules/rule_base.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/stat/dispatch/rules/rule_workflow.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/rules/rule_workflow.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/stat/log.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/log.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/stat/submit/logic/submit_logic.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/submit/logic/submit_logic.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/stat/submit/submit.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/submit/submit.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/stat/xcelery/instance.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/xcelery/instance.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/stat/xcelery/task_base.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/xcelery/task_base.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/utils/decorator.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/utils/profiler.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/utils/xListStr.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/utils/xListStr.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/utils/xdataframe.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/utils/xdataframe.py`

 * *Files 23% similar despite different names*

```diff
@@ -218,53 +218,7 @@
     """填充{}到nan"""
     return {} if not isinstance(data, dict) and pd.isna(data) else data
 
 
 def fill_list(data):
     """填充[]到nan"""
     return [] if not isinstance(data, list) and pd.isna(data) else data
-
-
-def df_expand_labels(_df, key, bins, insert_zero=True):
-    """
-    # money_df ####
-    # player_id, money
-    # 19296,  8
-    # 21169,  8
-    # 24003,  98
-    # 25016,  2
-    # 25254,  2
-    money_df[["money_label", "label_rank"]] = df_expand_labels(
-        money_df, "money", bins=[0, 8, 41, 267, 500, 1000, 2000, 5000, 10000, 20000, 30000, 50000, 999999]
-    ) =>
-    # player_id, money, money_label, label_rank
-    # 19296,    8,  1-8,    8
-    # 21169,    8,  1-8,    8
-    # 24003,    98, 1-8,    8
-    # 25016,    2,  1-8,    8
-    # 25254,    2,  42-267, 267
-    insert_zero : 是否在bins最前面插入0
-    :return:
-    """
-
-    def prefix_bins(_bins):
-        _bins = sorted(map(int, _bins))
-        if insert_zero and _bins[0] != 0:
-            _bins.insert(0, 0)
-        return _bins
-
-    bins = prefix_bins(bins)
-    concat = "-"
-
-    def cut_bins(row):
-        val = row[key]
-        if not val:
-            return val
-
-        if val > bins[-1]:
-            val = bins[-1]
-
-        position = bisect_left(bins, val)
-        labels = f"{bins[position - 1] + 1}{concat}{bins[position]}"
-        return labels, bins[position]
-
-    return _df.apply(cut_bins, axis=1, result_type="expand")
```

### Comparing `yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/utils/xdate.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/utils/xdate.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/utils/xhttp.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/utils/xhttp.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/utils/xmath.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/utils/xmath.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/yyxx_game_pkg/xtrace/helper.py` & `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/xtrace/helper.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.16.1/PKG-INFO` & `yyxx_game_pkg-2023.5.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yyxx-game-pkg
-Version: 2023.5.16.1
+Version: 2023.5.4.1
 Summary: yyxx game custom module
 Home-page: https://github.com/yyxxgame/yyxxgame-pkg
 License: MIT
 Author: yyxx-game
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yyxx-game-pkg Version: 2023.5.16.1 Summary: yyxx
+Metadata-Version: 2.1 Name: yyxx-game-pkg Version: 2023.5.4.1 Summary: yyxx
 game custom module Home-page: https://github.com/yyxxgame/yyxxgame-pkg License:
 MIT Author: yyxx-game Requires-Python: >=3.8,<4 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3
```

