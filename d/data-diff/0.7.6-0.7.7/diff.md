# Comparing `tmp/data_diff-0.7.6.tar.gz` & `tmp/data_diff-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_diff-0.7.6.tar", max compression
+gzip compressed data, was "data_diff-0.7.7.tar", max compression
```

## Comparing `data_diff-0.7.6.tar` & `data_diff-0.7.7.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0     1053 2023-04-03 18:06:26.931220 data_diff-0.7.6/LICENSE
--rw-r--r--   0        0        0     2696 2023-05-11 19:39:43.703801 data_diff-0.7.6/README.md
--rw-r--r--   0        0        0     8429 2023-04-21 21:58:08.193898 data_diff-0.7.6/data_diff/__init__.py
--rw-r--r--   0        0        0    16024 2023-05-05 21:08:17.222127 data_diff-0.7.6/data_diff/__main__.py
--rw-r--r--   0        0        0      108 2023-04-14 15:23:33.906548 data_diff-0.7.6/data_diff/cloud/__init__.py
--rw-r--r--   0        0        0    11594 2023-04-21 21:58:08.194331 data_diff-0.7.6/data_diff/cloud/data_source.py
--rw-r--r--   0        0        0     9335 2023-05-11 19:39:43.704637 data_diff-0.7.6/data_diff/cloud/datafold_api.py
--rw-r--r--   0        0        0     4044 2023-04-03 18:06:26.931568 data_diff-0.7.6/data_diff/config.py
--rw-r--r--   0        0        0      493 2023-04-21 21:58:08.194615 data_diff-0.7.6/data_diff/databases/__init__.py
--rw-r--r--   0        0        0     1353 2023-04-21 21:58:08.194720 data_diff-0.7.6/data_diff/databases/_connect.py
--rw-r--r--   0        0        0      174 2023-04-21 21:58:08.194816 data_diff-0.7.6/data_diff/databases/base.py
--rw-r--r--   0        0        0      257 2023-04-21 21:58:08.195148 data_diff-0.7.6/data_diff/databases/bigquery.py
--rw-r--r--   0        0        0      271 2023-04-21 21:58:08.195281 data_diff-0.7.6/data_diff/databases/clickhouse.py
--rw-r--r--   0        0        0      271 2023-04-21 21:58:08.195390 data_diff-0.7.6/data_diff/databases/databricks.py
--rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195511 data_diff-0.7.6/data_diff/databases/duckdb.py
--rw-r--r--   0        0        0      236 2023-04-21 21:58:08.195617 data_diff-0.7.6/data_diff/databases/mysql.py
--rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195713 data_diff-0.7.6/data_diff/databases/oracle.py
--rw-r--r--   0        0        0      275 2023-04-21 21:58:08.195827 data_diff-0.7.6/data_diff/databases/postgresql.py
--rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195918 data_diff-0.7.6/data_diff/databases/presto.py
--rw-r--r--   0        0        0      257 2023-04-21 21:58:08.196013 data_diff-0.7.6/data_diff/databases/redshift.py
--rw-r--r--   0        0        0      264 2023-04-21 21:58:08.196109 data_diff-0.7.6/data_diff/databases/snowflake.py
--rw-r--r--   0        0        0      236 2023-04-21 21:58:08.196196 data_diff-0.7.6/data_diff/databases/trino.py
--rw-r--r--   0        0        0      250 2023-04-21 21:58:08.196288 data_diff-0.7.6/data_diff/databases/vertica.py
--rw-r--r--   0        0        0    13326 2023-05-11 19:39:43.704995 data_diff-0.7.6/data_diff/dbt.py
--rw-r--r--   0        0        0    17697 2023-05-11 19:39:43.705201 data_diff-0.7.6/data_diff/dbt_parser.py
--rw-r--r--   0        0        0    14376 2023-04-21 21:58:08.196773 data_diff-0.7.6/data_diff/diff_tables.py
--rw-r--r--   0        0        0     9333 2023-05-05 21:08:17.222755 data_diff-0.7.6/data_diff/hashdiff_tables.py
--rw-r--r--   0        0        0     1477 2023-04-03 18:06:26.932667 data_diff-0.7.6/data_diff/info_tree.py
--rw-r--r--   0        0        0    14768 2023-04-21 21:58:08.197074 data_diff-0.7.6/data_diff/joindiff_tables.py
--rw-r--r--   0        0        0     7557 2023-04-03 18:06:26.932827 data_diff-0.7.6/data_diff/lexicographic_space.py
--rw-r--r--   0        0        0     1783 2023-04-03 18:06:26.932897 data_diff-0.7.6/data_diff/parse_time.py
--rw-r--r--   0        0        0     1404 2023-04-21 21:58:08.197181 data_diff-0.7.6/data_diff/query_utils.py
--rw-r--r--   0        0        0       76 2023-04-21 21:58:08.197422 data_diff-0.7.6/data_diff/sqeleton/__init__.py
--rw-r--r--   0        0        0      279 2023-04-21 21:58:08.197521 data_diff-0.7.6/data_diff/sqeleton/__main__.py
--rw-r--r--   0        0        0      264 2023-05-05 21:08:17.222879 data_diff-0.7.6/data_diff/sqeleton/abcs/__init__.py
--rw-r--r--   0        0        0      409 2023-04-21 21:58:08.197743 data_diff-0.7.6/data_diff/sqeleton/abcs/compiler.py
--rw-r--r--   0        0        0    11118 2023-05-05 21:08:17.223038 data_diff-0.7.6/data_diff/sqeleton/abcs/database_types.py
--rw-r--r--   0        0        0     6989 2023-05-05 21:08:17.223166 data_diff-0.7.6/data_diff/sqeleton/abcs/mixins.py
--rw-r--r--   0        0        0     2425 2023-04-21 21:58:08.198003 data_diff-0.7.6/data_diff/sqeleton/bound_exprs.py
--rw-r--r--   0        0        0      554 2023-04-21 21:58:08.198154 data_diff-0.7.6/data_diff/sqeleton/databases/__init__.py
--rw-r--r--   0        0        0     9131 2023-04-21 21:58:08.198249 data_diff-0.7.6/data_diff/sqeleton/databases/_connect.py
--rw-r--r--   0        0        0    20140 2023-05-11 19:39:43.705453 data_diff-0.7.6/data_diff/sqeleton/databases/base.py
--rw-r--r--   0        0        0    10135 2023-05-05 21:08:17.223531 data_diff-0.7.6/data_diff/sqeleton/databases/bigquery.py
--rw-r--r--   0        0        0     6642 2023-04-21 21:58:08.198608 data_diff-0.7.6/data_diff/sqeleton/databases/clickhouse.py
--rw-r--r--   0        0        0     6959 2023-04-21 21:58:08.198702 data_diff-0.7.6/data_diff/sqeleton/databases/databricks.py
--rw-r--r--   0        0        0     6093 2023-04-21 21:58:08.198787 data_diff-0.7.6/data_diff/sqeleton/databases/duckdb.py
--rw-r--r--   0        0        0      910 2023-04-21 21:58:08.198859 data_diff-0.7.6/data_diff/sqeleton/databases/mssql.py
--rw-r--r--   0        0        0     4438 2023-04-21 21:58:08.198940 data_diff-0.7.6/data_diff/sqeleton/databases/mysql.py
--rw-r--r--   0        0        0     6550 2023-05-05 21:08:17.223666 data_diff-0.7.6/data_diff/sqeleton/databases/oracle.py
--rw-r--r--   0        0        0     5551 2023-05-05 21:08:17.223788 data_diff-0.7.6/data_diff/sqeleton/databases/postgresql.py
--rw-r--r--   0        0        0     6112 2023-04-21 21:58:08.199200 data_diff-0.7.6/data_diff/sqeleton/databases/presto.py
--rw-r--r--   0        0        0     6312 2023-05-05 21:08:17.223928 data_diff-0.7.6/data_diff/sqeleton/databases/redshift.py
--rw-r--r--   0        0        0     7742 2023-04-21 21:58:08.199375 data_diff-0.7.6/data_diff/sqeleton/databases/snowflake.py
--rw-r--r--   0        0        0     1297 2023-04-21 21:58:08.199477 data_diff-0.7.6/data_diff/sqeleton/databases/trino.py
--rw-r--r--   0        0        0     5426 2023-04-21 21:58:08.199590 data_diff-0.7.6/data_diff/sqeleton/databases/vertica.py
--rw-r--r--   0        0        0      464 2023-04-21 21:58:08.199708 data_diff-0.7.6/data_diff/sqeleton/queries/__init__.py
--rw-r--r--   0        0        0     5291 2023-04-21 21:58:08.199788 data_diff-0.7.6/data_diff/sqeleton/queries/api.py
--rw-r--r--   0        0        0    30750 2023-05-05 21:08:17.224381 data_diff-0.7.6/data_diff/sqeleton/queries/ast_classes.py
--rw-r--r--   0        0        0      367 2023-04-21 21:58:08.200018 data_diff-0.7.6/data_diff/sqeleton/queries/base.py
--rw-r--r--   0        0        0     2605 2023-04-21 21:58:08.200096 data_diff-0.7.6/data_diff/sqeleton/queries/compiler.py
--rw-r--r--   0        0        0     1985 2023-04-21 21:58:08.200163 data_diff-0.7.6/data_diff/sqeleton/queries/extras.py
--rw-r--r--   0        0        0     1404 2023-04-21 21:58:08.200227 data_diff-0.7.6/data_diff/sqeleton/query_utils.py
--rw-r--r--   0        0        0     1981 2023-04-21 21:58:08.200332 data_diff-0.7.6/data_diff/sqeleton/repl.py
--rw-r--r--   0        0        0      737 2023-04-21 21:58:08.200391 data_diff-0.7.6/data_diff/sqeleton/schema.py
--rw-r--r--   0        0        0     8907 2023-04-21 21:58:08.200481 data_diff-0.7.6/data_diff/sqeleton/utils.py
--rw-r--r--   0        0        0    10884 2023-04-21 21:58:08.200617 data_diff-0.7.6/data_diff/table_segment.py
--rw-r--r--   0        0        0     2651 2023-04-03 18:06:26.933183 data_diff-0.7.6/data_diff/thread_utils.py
--rw-r--r--   0        0        0     4121 2023-04-15 23:11:48.035287 data_diff-0.7.6/data_diff/tracking.py
--rw-r--r--   0        0        0     5247 2023-05-05 21:08:17.224565 data_diff-0.7.6/data_diff/utils.py
--rw-r--r--   0        0        0       22 2023-05-11 19:39:43.705598 data_diff-0.7.6/data_diff/version.py
--rwxr-xr-x   0        0        0     2816 2023-05-11 19:39:43.706580 data_diff-0.7.6/pyproject.toml
--rw-r--r--   0        0        0     5304 1970-01-01 00:00:00.000000 data_diff-0.7.6/PKG-INFO
+-rw-r--r--   0        0        0     1053 2023-04-03 18:06:26.931220 data_diff-0.7.7/LICENSE
+-rw-r--r--   0        0        0     2696 2023-05-11 19:39:43.703801 data_diff-0.7.7/README.md
+-rw-r--r--   0        0        0     8429 2023-04-21 21:58:08.193898 data_diff-0.7.7/data_diff/__init__.py
+-rw-r--r--   0        0        0    16024 2023-05-05 21:08:17.222127 data_diff-0.7.7/data_diff/__main__.py
+-rw-r--r--   0        0        0      126 2023-05-15 21:10:13.082463 data_diff-0.7.7/data_diff/cloud/__init__.py
+-rw-r--r--   0        0        0    11594 2023-04-21 21:58:08.194331 data_diff-0.7.7/data_diff/cloud/data_source.py
+-rw-r--r--   0        0        0    10067 2023-05-15 21:10:13.082649 data_diff-0.7.7/data_diff/cloud/datafold_api.py
+-rw-r--r--   0        0        0     4044 2023-04-03 18:06:26.931568 data_diff-0.7.7/data_diff/config.py
+-rw-r--r--   0        0        0      493 2023-04-21 21:58:08.194615 data_diff-0.7.7/data_diff/databases/__init__.py
+-rw-r--r--   0        0        0     1353 2023-04-21 21:58:08.194720 data_diff-0.7.7/data_diff/databases/_connect.py
+-rw-r--r--   0        0        0      174 2023-04-21 21:58:08.194816 data_diff-0.7.7/data_diff/databases/base.py
+-rw-r--r--   0        0        0      257 2023-04-21 21:58:08.195148 data_diff-0.7.7/data_diff/databases/bigquery.py
+-rw-r--r--   0        0        0      271 2023-04-21 21:58:08.195281 data_diff-0.7.7/data_diff/databases/clickhouse.py
+-rw-r--r--   0        0        0      271 2023-04-21 21:58:08.195390 data_diff-0.7.7/data_diff/databases/databricks.py
+-rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195511 data_diff-0.7.7/data_diff/databases/duckdb.py
+-rw-r--r--   0        0        0      236 2023-04-21 21:58:08.195617 data_diff-0.7.7/data_diff/databases/mysql.py
+-rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195713 data_diff-0.7.7/data_diff/databases/oracle.py
+-rw-r--r--   0        0        0      275 2023-04-21 21:58:08.195827 data_diff-0.7.7/data_diff/databases/postgresql.py
+-rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195918 data_diff-0.7.7/data_diff/databases/presto.py
+-rw-r--r--   0        0        0      257 2023-04-21 21:58:08.196013 data_diff-0.7.7/data_diff/databases/redshift.py
+-rw-r--r--   0        0        0      264 2023-04-21 21:58:08.196109 data_diff-0.7.7/data_diff/databases/snowflake.py
+-rw-r--r--   0        0        0      236 2023-04-21 21:58:08.196196 data_diff-0.7.7/data_diff/databases/trino.py
+-rw-r--r--   0        0        0      250 2023-04-21 21:58:08.196288 data_diff-0.7.7/data_diff/databases/vertica.py
+-rw-r--r--   0        0        0    14233 2023-05-15 21:10:13.082842 data_diff-0.7.7/data_diff/dbt.py
+-rw-r--r--   0        0        0    18122 2023-05-15 21:10:13.083057 data_diff-0.7.7/data_diff/dbt_parser.py
+-rw-r--r--   0        0        0    14376 2023-04-21 21:58:08.196773 data_diff-0.7.7/data_diff/diff_tables.py
+-rw-r--r--   0        0        0     9333 2023-05-05 21:08:17.222755 data_diff-0.7.7/data_diff/hashdiff_tables.py
+-rw-r--r--   0        0        0     1477 2023-04-03 18:06:26.932667 data_diff-0.7.7/data_diff/info_tree.py
+-rw-r--r--   0        0        0    14768 2023-04-21 21:58:08.197074 data_diff-0.7.7/data_diff/joindiff_tables.py
+-rw-r--r--   0        0        0     7557 2023-04-03 18:06:26.932827 data_diff-0.7.7/data_diff/lexicographic_space.py
+-rw-r--r--   0        0        0     1783 2023-04-03 18:06:26.932897 data_diff-0.7.7/data_diff/parse_time.py
+-rw-r--r--   0        0        0     1404 2023-04-21 21:58:08.197181 data_diff-0.7.7/data_diff/query_utils.py
+-rw-r--r--   0        0        0       76 2023-04-21 21:58:08.197422 data_diff-0.7.7/data_diff/sqeleton/__init__.py
+-rw-r--r--   0        0        0      279 2023-04-21 21:58:08.197521 data_diff-0.7.7/data_diff/sqeleton/__main__.py
+-rw-r--r--   0        0        0      264 2023-05-05 21:08:17.222879 data_diff-0.7.7/data_diff/sqeleton/abcs/__init__.py
+-rw-r--r--   0        0        0      409 2023-04-21 21:58:08.197743 data_diff-0.7.7/data_diff/sqeleton/abcs/compiler.py
+-rw-r--r--   0        0        0    11118 2023-05-05 21:08:17.223038 data_diff-0.7.7/data_diff/sqeleton/abcs/database_types.py
+-rw-r--r--   0        0        0     6989 2023-05-05 21:08:17.223166 data_diff-0.7.7/data_diff/sqeleton/abcs/mixins.py
+-rw-r--r--   0        0        0     2425 2023-04-21 21:58:08.198003 data_diff-0.7.7/data_diff/sqeleton/bound_exprs.py
+-rw-r--r--   0        0        0      554 2023-04-21 21:58:08.198154 data_diff-0.7.7/data_diff/sqeleton/databases/__init__.py
+-rw-r--r--   0        0        0     9245 2023-05-15 21:10:13.083663 data_diff-0.7.7/data_diff/sqeleton/databases/_connect.py
+-rw-r--r--   0        0        0    20140 2023-05-11 19:39:43.705453 data_diff-0.7.7/data_diff/sqeleton/databases/base.py
+-rw-r--r--   0        0        0    10135 2023-05-05 21:08:17.223531 data_diff-0.7.7/data_diff/sqeleton/databases/bigquery.py
+-rw-r--r--   0        0        0     6642 2023-04-21 21:58:08.198608 data_diff-0.7.7/data_diff/sqeleton/databases/clickhouse.py
+-rw-r--r--   0        0        0     6959 2023-04-21 21:58:08.198702 data_diff-0.7.7/data_diff/sqeleton/databases/databricks.py
+-rw-r--r--   0        0        0     6093 2023-04-21 21:58:08.198787 data_diff-0.7.7/data_diff/sqeleton/databases/duckdb.py
+-rw-r--r--   0        0        0      910 2023-04-21 21:58:08.198859 data_diff-0.7.7/data_diff/sqeleton/databases/mssql.py
+-rw-r--r--   0        0        0     4438 2023-04-21 21:58:08.198940 data_diff-0.7.7/data_diff/sqeleton/databases/mysql.py
+-rw-r--r--   0        0        0     6550 2023-05-05 21:08:17.223666 data_diff-0.7.7/data_diff/sqeleton/databases/oracle.py
+-rw-r--r--   0        0        0     5551 2023-05-05 21:08:17.223788 data_diff-0.7.7/data_diff/sqeleton/databases/postgresql.py
+-rw-r--r--   0        0        0     6112 2023-04-21 21:58:08.199200 data_diff-0.7.7/data_diff/sqeleton/databases/presto.py
+-rw-r--r--   0        0        0     6312 2023-05-05 21:08:17.223928 data_diff-0.7.7/data_diff/sqeleton/databases/redshift.py
+-rw-r--r--   0        0        0     7742 2023-04-21 21:58:08.199375 data_diff-0.7.7/data_diff/sqeleton/databases/snowflake.py
+-rw-r--r--   0        0        0     1297 2023-04-21 21:58:08.199477 data_diff-0.7.7/data_diff/sqeleton/databases/trino.py
+-rw-r--r--   0        0        0     5426 2023-04-21 21:58:08.199590 data_diff-0.7.7/data_diff/sqeleton/databases/vertica.py
+-rw-r--r--   0        0        0      464 2023-04-21 21:58:08.199708 data_diff-0.7.7/data_diff/sqeleton/queries/__init__.py
+-rw-r--r--   0        0        0     5291 2023-04-21 21:58:08.199788 data_diff-0.7.7/data_diff/sqeleton/queries/api.py
+-rw-r--r--   0        0        0    30750 2023-05-05 21:08:17.224381 data_diff-0.7.7/data_diff/sqeleton/queries/ast_classes.py
+-rw-r--r--   0        0        0      367 2023-04-21 21:58:08.200018 data_diff-0.7.7/data_diff/sqeleton/queries/base.py
+-rw-r--r--   0        0        0     2605 2023-04-21 21:58:08.200096 data_diff-0.7.7/data_diff/sqeleton/queries/compiler.py
+-rw-r--r--   0        0        0     1985 2023-04-21 21:58:08.200163 data_diff-0.7.7/data_diff/sqeleton/queries/extras.py
+-rw-r--r--   0        0        0     1404 2023-04-21 21:58:08.200227 data_diff-0.7.7/data_diff/sqeleton/query_utils.py
+-rw-r--r--   0        0        0     1981 2023-04-21 21:58:08.200332 data_diff-0.7.7/data_diff/sqeleton/repl.py
+-rw-r--r--   0        0        0      737 2023-04-21 21:58:08.200391 data_diff-0.7.7/data_diff/sqeleton/schema.py
+-rw-r--r--   0        0        0     8907 2023-04-21 21:58:08.200481 data_diff-0.7.7/data_diff/sqeleton/utils.py
+-rw-r--r--   0        0        0    10884 2023-04-21 21:58:08.200617 data_diff-0.7.7/data_diff/table_segment.py
+-rw-r--r--   0        0        0     2651 2023-04-03 18:06:26.933183 data_diff-0.7.7/data_diff/thread_utils.py
+-rw-r--r--   0        0        0     4322 2023-05-15 21:10:13.084169 data_diff-0.7.7/data_diff/tracking.py
+-rw-r--r--   0        0        0     5646 2023-05-15 21:10:13.084338 data_diff-0.7.7/data_diff/utils.py
+-rw-r--r--   0        0        0       22 2023-05-15 22:24:21.626159 data_diff-0.7.7/data_diff/version.py
+-rwxr-xr-x   0        0        0     2831 2023-05-15 22:24:21.626341 data_diff-0.7.7/pyproject.toml
+-rw-r--r--   0        0        0     5332 1970-01-01 00:00:00.000000 data_diff-0.7.7/PKG-INFO
```

### Comparing `data_diff-0.7.6/LICENSE` & `data_diff-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.6/README.md` & `data_diff-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.6/data_diff/__init__.py` & `data_diff-0.7.7/data_diff/__init__.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.6/data_diff/__main__.py` & `data_diff-0.7.7/data_diff/__main__.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.6/data_diff/cloud/data_source.py` & `data_diff-0.7.7/data_diff/cloud/data_source.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.6/data_diff/cloud/datafold_api.py` & `data_diff-0.7.7/data_diff/cloud/datafold_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,14 +103,20 @@
     pk_columns: List[str]
     filter1: Optional[str] = None
     filter2: Optional[str] = None
     include_columns: Optional[List[str]]
     exclude_columns: Optional[List[str]]
 
 
+class TCloudApiOrgMeta(pydantic.BaseModel):
+    org_id: int
+    org_name: str
+    user_id: int
+
+
 class TSummaryResultPrimaryKeyStats(pydantic.BaseModel):
     total_rows: Tuple[int, int]
     nulls: Tuple[int, int]
     dupes: Tuple[int, int]
     exclusives: Tuple[int, int]
     distincts: Tuple[int, int]
 
@@ -130,14 +136,16 @@
 
 
 class TSummaryResultSchemaStats(pydantic.BaseModel):
     columns_mismatched: Tuple[int, int]
     column_type_mismatches: int
     column_reorders: int
     column_counts: Tuple[int, int]
+    column_type_differs: List[str]
+    exclusive_columns: Tuple[List[str], List[str]]
 
 
 class TCloudApiDataDiffSummaryResult(pydantic.BaseModel):
     status: str
     pks: Optional[TSummaryResultPrimaryKeyStats]
     values: Optional[TSummaryResultValueStats]
     schema_: Optional[TSummaryResultSchemaStats]
@@ -194,14 +202,19 @@
         return rv
 
     def get_data_sources(self) -> List[TCloudApiDataSource]:
         rv = self.make_get_request(url="api/v1/data_sources")
         rv.raise_for_status()
         return [TCloudApiDataSource(**item) for item in rv.json()]
 
+    def get_data_source(self, data_source_id: int) -> TCloudApiDataSource:
+        rv = self.make_get_request(url=f"api/v1/data_sources/{data_source_id}")
+        rv.raise_for_status()
+        return TCloudApiDataSource(**rv.json())
+
     def create_data_source(self, config: TDsConfig) -> TCloudApiDataSource:
         payload = config.dict()
         if config.type == "bigquery":
             json_string = payload["options"]["jsonKeyFile"].encode("utf-8")
             payload["options"]["jsonKeyFile"] = base64.b64encode(json_string).decode("utf-8")
         rv = self.make_post_request(url="api/v1/data_sources", payload=payload)
         return TCloudApiDataSource(**rv.json())
@@ -265,7 +278,14 @@
                     outcome=item["result"]["outcome"],
                 )
                 if item["result"] is not None
                 else None,
             )
             for item in rv.json()["results"]
         ]
+
+    def get_org_meta(self) -> TCloudApiOrgMeta:
+        response = self.make_get_request(f"api/v1/organization/meta")
+        response_json = response.json()
+        return TCloudApiOrgMeta(
+            org_id=response_json["org_id"], org_name=response_json["org_name"], user_id=response_json["user_id"]
+        )
```

### Comparing `data_diff-0.7.6/data_diff/config.py` & `data_diff-0.7.7/data_diff/config.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.6/data_diff/databases/_connect.py` & `data_diff-0.7.7/data_diff/databases/_connect.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.6/data_diff/dbt.py` & `data_diff-0.7.7/data_diff/dbt.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,20 +2,26 @@
 import time
 import webbrowser
 import pydantic
 import rich
 from rich.prompt import Confirm
 
 from typing import List, Optional, Dict
-from .utils import dbt_diff_string_template, getLogger
+from .utils import (
+    dbt_diff_string_template,
+    getLogger,
+    columns_added_template,
+    columns_removed_template,
+    no_differences_template,
+)
 from pathlib import Path
 
 import keyring
 
-from .cloud import DatafoldAPI, TCloudApiDataDiff, get_or_create_data_source
+from .cloud import DatafoldAPI, TCloudApiDataDiff, TCloudApiOrgMeta, get_or_create_data_source
 from .dbt_parser import DbtParser, PROJECT_FILE
 
 
 logger = getLogger(__name__)
 
 
 from .tracking import (
@@ -68,14 +74,15 @@
         )
 
     if is_cloud:
         api = _initialize_api()
         # exit so the user can set the key
         if not api:
             return
+        org_meta = api.get_org_meta()
 
         if datasource_id is None:
             rich.print("[red]Data source ID not found in dbt_project.yml")
             is_create_data_source = Confirm.ask("Would you like to create a new data source?")
             if is_create_data_source:
                 datasource_id = get_or_create_data_source(api=api, dbt_parser=dbt_parser)
                 rich.print(f'To use the data source in next runs, please, update your "{PROJECT_FILE}" with a block:')
@@ -85,27 +92,30 @@
                     "https://docs.datafold.com/os_diff/dbt_integration/#configure-a-data-source\n"
                 )
             else:
                 raise ValueError(
                     "Datasource ID not found, include it as a dbt variable in the dbt_project.yml. "
                     "\nvars:\n data_diff:\n   datasource_id: 1234"
                 )
+
+        data_source = api.get_data_source(datasource_id)
+        dbt_parser.set_casing_policy_for(connection_type=data_source.type)
         rich.print("[green][bold]\nDiffs in progress...[/][/]\n")
 
     else:
         dbt_parser.set_connection()
 
     for model in models:
         diff_vars = _get_diff_vars(
             dbt_parser, config_prod_database, config_prod_schema, config_prod_custom_schema, model
         )
 
         if diff_vars.primary_keys:
             if is_cloud:
-                diff_thread = run_as_daemon(_cloud_diff, diff_vars, datasource_id, api)
+                diff_thread = run_as_daemon(_cloud_diff, diff_vars, datasource_id, api, org_meta)
                 diff_threads.append(diff_thread)
             else:
                 _local_diff(diff_vars)
         else:
             rich.print(
                 _diff_output_base(".".join(diff_vars.dev_path), ".".join(diff_vars.prod_path))
                 + "Skipped due to unknown primary key. Add uniqueness tests, meta, or tags.\n"
@@ -168,15 +178,14 @@
         where_filter=datadiff_model_config.where_filter,
         include_columns=datadiff_model_config.include_columns,
         exclude_columns=datadiff_model_config.exclude_columns,
     )
 
 
 def _local_diff(diff_vars: TDiffVars) -> None:
-    column_diffs_str = ""
     dev_qualified_str = ".".join(diff_vars.dev_path)
     prod_qualified_str = ".".join(diff_vars.prod_path)
     diff_output_str = _diff_output_base(dev_qualified_str, prod_qualified_str)
 
     table1 = connect_to_table(diff_vars.connection, dev_qualified_str, tuple(diff_vars.primary_keys), diff_vars.threads)
     table2 = connect_to_table(
         diff_vars.connection, prod_qualified_str, tuple(diff_vars.primary_keys), diff_vars.threads
@@ -189,22 +198,22 @@
     except Exception as ex:
         logger.debug(ex)
         diff_output_str += "[red]New model or no access to prod table.[/] \n"
         rich.print(diff_output_str)
         return
 
     column_set = set(table1_columns).intersection(table2_columns)
-    table1_diff = set(table1_columns).difference(table2_columns)
-    table2_diff = set(table2_columns).difference(table1_columns)
+    columns_added = set(table1_columns).difference(table2_columns)
+    columns_removed = set(table2_columns).difference(table1_columns)
 
-    if table1_diff:
-        column_diffs_str += f"Column(s) added: {table1_diff}\n"
+    if columns_added:
+        diff_output_str += columns_added_template(columns_added)
 
-    if table2_diff:
-        column_diffs_str += f"Column(s) removed: {table2_diff}\n"
+    if columns_removed:
+        diff_output_str += columns_removed_template(columns_removed)
 
     column_set = column_set - set(diff_vars.primary_keys)
 
     if diff_vars.include_columns:
         column_set = {x for x in column_set if x.upper() in [y.upper() for y in diff_vars.include_columns]}
 
     if diff_vars.exclude_columns:
@@ -218,18 +227,18 @@
         threaded=True,
         algorithm=Algorithm.JOINDIFF,
         extra_columns=extra_columns,
         where=diff_vars.where_filter,
     )
 
     if list(diff):
-        diff_output_str += f"{column_diffs_str}{diff.get_stats_string(is_dbt=True)} \n"
+        diff_output_str += f"{diff.get_stats_string(is_dbt=True)} \n"
         rich.print(diff_output_str)
     else:
-        diff_output_str += f"{column_diffs_str}[bold][green]No row differences[/][/] \n"
+        diff_output_str += no_differences_template()
         rich.print(diff_output_str)
 
 
 def _initialize_api() -> Optional[DatafoldAPI]:
     datafold_host = os.environ.get("DATAFOLD_HOST")
     if datafold_host is None:
         datafold_host = "https://app.datafold.com"
@@ -256,15 +265,15 @@
         keyring.set_password("data-diff", "DATAFOLD_API_KEY", api_key)
     except Exception as e:
         rich.print(f"[red]Failed when saving the API key to the system keyring service. Reason: {e}")
 
     return DatafoldAPI(api_key=api_key, host=datafold_host)
 
 
-def _cloud_diff(diff_vars: TDiffVars, datasource_id: int, api: DatafoldAPI) -> None:
+def _cloud_diff(diff_vars: TDiffVars, datasource_id: int, api: DatafoldAPI, org_meta: TCloudApiOrgMeta) -> None:
     diff_output_str = _diff_output_base(".".join(diff_vars.dev_path), ".".join(diff_vars.prod_path))
     payload = TCloudApiDataDiff(
         data_source1_id=datasource_id,
         data_source2_id=datasource_id,
         table1=diff_vars.prod_path,
         table2=diff_vars.dev_path,
         pk_columns=diff_vars.primary_keys,
@@ -297,28 +306,40 @@
 
         rows_updated = diff_results.values.rows_with_differences
         total_rows = diff_results.values.total_rows
         rows_unchanged = int(total_rows) - int(rows_updated)
         diff_percent_list = {
             x.column_name: str(x.match) + "%" for x in diff_results.values.columns_diff_stats if x.match != 100.0
         }
+        columns_added = diff_results.schema_.exclusive_columns[1]
+        columns_removed = diff_results.schema_.exclusive_columns[0]
+        column_type_changes = diff_results.schema_.column_type_differs
+
+        if columns_added:
+            diff_output_str += columns_added_template(columns_added)
+
+        if columns_removed:
+            diff_output_str += columns_removed_template(columns_removed)
+
+        if column_type_changes:
+            diff_output_str += "Type change: " + str(column_type_changes) + "\n"
 
         if any([rows_added_count, rows_removed_count, rows_updated]):
             diff_output = dbt_diff_string_template(
                 rows_added_count,
                 rows_removed_count,
                 rows_updated,
                 str(rows_unchanged),
                 diff_percent_list,
                 "Value Match Percent:",
             )
-            diff_output_str += f"{diff_url}\n {diff_output} \n"
+            diff_output_str += f"\n{diff_url}\n {diff_output} \n"
             rich.print(diff_output_str)
         else:
-            diff_output_str += f"{diff_url}\n [green]No row differences[/] \n"
+            diff_output_str += f"\n{diff_url}\n{no_differences_template()}\n"
             rich.print(diff_output_str)
 
     except BaseException as ex:  # Catch KeyboardInterrupt too
         error = ex
     finally:
         # we don't currently have much of this information
         # but I imagine a future iteration of this _cloud method
@@ -332,14 +353,17 @@
                 data_source_2_type="",
                 table1_count=0,
                 table2_count=0,
                 diff_count=0,
                 error=err_message,
                 diff_id=diff_id,
                 is_cloud=True,
+                org_id=org_meta.org_id,
+                org_name=org_meta.org_name,
+                user_id=org_meta.user_id,
             )
             send_event_json(event_json)
 
         if error:
             rich.print(diff_output_str)
             if diff_id:
                 diff_url = f"{api.host}/datadiffs/{diff_id}/overview"
```

### Comparing `data_diff-0.7.6/data_diff/dbt_parser.py` & `data_diff-0.7.7/data_diff/dbt_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,29 +234,29 @@
         )
         conn_type = conn_type.lower()
 
         return credentials, conn_type
 
     def set_connection(self):
         credentials, conn_type = self.get_connection_creds()
+        self.set_casing_policy_for(conn_type)
 
         if conn_type == "snowflake":
             conn_info = {
                 "driver": conn_type,
                 "user": credentials.get("user"),
                 "account": credentials.get("account"),
                 "database": credentials.get("database"),
                 "warehouse": credentials.get("warehouse"),
                 "role": credentials.get("role"),
                 "schema": credentials.get("schema"),
                 "insecure_mode": credentials.get("insecure_mode", False),
                 "client_session_keep_alive": credentials.get("client_session_keep_alive", False),
             }
             self.threads = credentials.get("threads")
-            self.requires_upper = True
 
             if credentials.get("private_key_path") is not None:
                 if credentials.get("password") is not None:
                     raise Exception("Cannot use password and key at the same time")
                 conn_info["key"] = credentials.get("private_key_path")
                 conn_info["private_key_passphrase"] = credentials.get("private_key_passphrase")
             elif credentials.get("authenticator") is not None:
@@ -401,7 +401,15 @@
             definition = definition[7:-1]  # Removes concat( and )
             columns = definition.split(",")
         else:
             columns = definition.split("||")
 
         stripped_columns = [col.strip('" ()') for col in columns]
         return stripped_columns
+
+    def set_casing_policy_for(self, connection_type: str):
+        """
+        Set casing policy for identifiers: database, schema, table, column, etc.
+        Correct policy depends on the type of the database, because some databases (e.g. Snowflake)
+        use upper case identifiers by default, while others (e.g. Postgres) use lower case.
+        """
+        self.requires_upper = connection_type == "snowflake"
```

### Comparing `data_diff-0.7.6/data_diff/diff_tables.py` & `data_diff-0.7.7/data_diff/diff_tables.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.6/data_diff/hashdiff_tables.py` & `data_diff-0.7.7/data_diff/hashdiff_tables.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.6/data_diff/info_tree.py` & `data_diff-0.7.7/data_diff/info_tree.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.6/data_diff/joindiff_tables.py` & `data_diff-0.7.7/data_diff/joindiff_tables.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.6/data_diff/lexicographic_space.py` & `data_diff-0.7.7/data_diff/lexicographic_space.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.6/data_diff/parse_time.py` & `data_diff-0.7.7/data_diff/parse_time.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.6/data_diff/query_utils.py` & `data_diff-0.7.7/data_diff/query_utils.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.6/data_diff/sqeleton/abcs/database_types.py` & `data_diff-0.7.7/data_diff/sqeleton/abcs/database_types.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.6/data_diff/sqeleton/abcs/mixins.py` & `data_diff-0.7.7/data_diff/sqeleton/abcs/mixins.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.6/data_diff/sqeleton/bound_exprs.py` & `data_diff-0.7.7/data_diff/sqeleton/bound_exprs.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.6/data_diff/sqeleton/databases/__init__.py` & `data_diff-0.7.7/data_diff/sqeleton/databases/__init__.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.6/data_diff/sqeleton/databases/_connect.py` & `data_diff-0.7.7/data_diff/sqeleton/databases/_connect.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,16 +178,19 @@
 
             if scheme == "snowflake":
                 kw["account"] = dsn.host
                 assert not dsn.port
                 kw["user"] = dsn.user
                 kw["password"] = dsn.password
             else:
-                kw["host"] = dsn.host
-                kw["port"] = dsn.port
+                if scheme == "oracle":
+                    kw["host"] = dsn.hostloc
+                else:
+                    kw["host"] = dsn.host
+                    kw["port"] = dsn.port
                 kw["user"] = dsn.user
                 if dsn.password:
                     kw["password"] = dsn.password
 
         kw = {k: v for k, v in kw.items() if v is not None}
 
         if issubclass(cls, ThreadedDatabase):
```

### Comparing `data_diff-0.7.6/data_diff/sqeleton/databases/base.py` & `data_diff-0.7.7/data_diff/sqeleton/databases/base.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.6/data_diff/sqeleton/databases/bigquery.py` & `data_diff-0.7.7/data_diff/sqeleton/databases/bigquery.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.6/data_diff/sqeleton/databases/clickhouse.py` & `data_diff-0.7.7/data_diff/sqeleton/databases/clickhouse.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.6/data_diff/sqeleton/databases/databricks.py` & `data_diff-0.7.7/data_diff/sqeleton/databases/databricks.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.6/data_diff/sqeleton/databases/duckdb.py` & `data_diff-0.7.7/data_diff/sqeleton/databases/duckdb.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.6/data_diff/sqeleton/databases/mssql.py` & `data_diff-0.7.7/data_diff/sqeleton/databases/mssql.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.6/data_diff/sqeleton/databases/mysql.py` & `data_diff-0.7.7/data_diff/sqeleton/databases/mysql.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.6/data_diff/sqeleton/databases/oracle.py` & `data_diff-0.7.7/data_diff/sqeleton/databases/oracle.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.6/data_diff/sqeleton/databases/postgresql.py` & `data_diff-0.7.7/data_diff/sqeleton/databases/postgresql.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.6/data_diff/sqeleton/databases/presto.py` & `data_diff-0.7.7/data_diff/sqeleton/databases/presto.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.6/data_diff/sqeleton/databases/redshift.py` & `data_diff-0.7.7/data_diff/sqeleton/databases/redshift.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.6/data_diff/sqeleton/databases/snowflake.py` & `data_diff-0.7.7/data_diff/sqeleton/databases/snowflake.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.6/data_diff/sqeleton/databases/trino.py` & `data_diff-0.7.7/data_diff/sqeleton/databases/trino.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.6/data_diff/sqeleton/databases/vertica.py` & `data_diff-0.7.7/data_diff/sqeleton/databases/vertica.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.6/data_diff/sqeleton/queries/api.py` & `data_diff-0.7.7/data_diff/sqeleton/queries/api.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.6/data_diff/sqeleton/queries/ast_classes.py` & `data_diff-0.7.7/data_diff/sqeleton/queries/ast_classes.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.6/data_diff/sqeleton/queries/compiler.py` & `data_diff-0.7.7/data_diff/sqeleton/queries/compiler.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.6/data_diff/sqeleton/queries/extras.py` & `data_diff-0.7.7/data_diff/sqeleton/queries/extras.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.6/data_diff/sqeleton/query_utils.py` & `data_diff-0.7.7/data_diff/sqeleton/query_utils.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.6/data_diff/sqeleton/repl.py` & `data_diff-0.7.7/data_diff/sqeleton/repl.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.6/data_diff/sqeleton/schema.py` & `data_diff-0.7.7/data_diff/sqeleton/schema.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.6/data_diff/sqeleton/utils.py` & `data_diff-0.7.7/data_diff/sqeleton/utils.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.6/data_diff/table_segment.py` & `data_diff-0.7.7/data_diff/table_segment.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.6/data_diff/thread_utils.py` & `data_diff-0.7.7/data_diff/thread_utils.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.6/data_diff/tracking.py` & `data_diff-0.7.7/data_diff/tracking.py`

 * *Files 4% similar despite different names*

```diff
@@ -112,14 +112,17 @@
     data_source_2_type: str,
     table1_count: int,
     table2_count: int,
     diff_count: int,
     error: Optional[str],
     diff_id: Optional[int] = None,
     is_cloud: bool = False,
+    org_id: Optional[int] = None,
+    org_name: Optional[str] = None,
+    user_id: Optional[int] = None,
 ):
     return {
         "event": "os_diff_run_end",
         "properties": {
             "distinct_id": get_anonymous_id(),
             "token": TOKEN,
             "time": time(),
@@ -134,14 +137,17 @@
             "data_diff_version:": __version__,
             "entrypoint_name": entrypoint_name,
             "is_cloud": is_cloud,
             "diff_id": diff_id,
             "dbt_user_id": dbt_user_id,
             "dbt_version": dbt_version,
             "dbt_project_id": dbt_project_id,
+            "org_id": org_id,
+            "org_name": org_name,
+            "user_id": user_id,
         },
     }
 
 
 def send_event_json(event_json):
     if not g_tracking_enabled:
         raise RuntimeError("Won't send; tracking is disabled!")
```

### Comparing `data_diff-0.7.6/data_diff/utils.py` & `data_diff-0.7.7/data_diff/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -152,20 +152,34 @@
         return json.loads(a) == json.loads(b)
     except (ValueError, TypeError, json.decoder.JSONDecodeError):  # not valid jsons
         return False
 
 
 def diffs_are_equiv_jsons(diff: list, json_cols: dict):
     overriden_diff_cols = set()
-    if (len(diff) != 2) or ({diff[0][0], diff[1][0]} != {'+', '-'}):
+    if (len(diff) != 2) or ({diff[0][0], diff[1][0]} != {"+", "-"}):
         return False, overriden_diff_cols
     match = True
     for i, (col_a, col_b) in enumerate(safezip(diff[0][1][1:], diff[1][1][1:])):  # index 0 is extra_columns first elem
         # we only attempt to parse columns of JSON type, but we still need to check if non-json columns don't match
         match = col_a == col_b
         if not match and (i in json_cols):
             if _jsons_equiv(col_a, col_b):
                 overriden_diff_cols.add(json_cols[i])
                 match = True
         if not match:
             break
     return match, overriden_diff_cols
+
+
+def columns_removed_template(table2_set_diff) -> str:
+    columns_removed = "Column(s) removed: " + str(table2_set_diff) + "\n"
+    return columns_removed
+
+
+def columns_added_template(table1_set_diff) -> str:
+    columns_added = "Column(s) added: " + str(table1_set_diff) + "\n"
+    return columns_added
+
+
+def no_differences_template() -> str:
+    return "[bold][green]No row differences[/][/]\n"
```

### Comparing `data_diff-0.7.6/pyproject.toml` & `data_diff-0.7.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "data-diff"
-version = "0.7.6"
+version = "0.7.7"
 description = "Command-line tool and Python library to efficiently diff rows across two different databases."
 authors = ["Datafold <data-diff@datafold.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/datafold/data-diff"
 documentation = ""
 classifiers = [
@@ -43,14 +43,15 @@
 dbt-artifacts-parser = {version="^0.3.0"}
 dbt-core = {version="^1.0.0"}
 keyring = "*"
 tabulate = "^0.9.0"
 preql = {version="^0.2.19", optional=true}
 cx_Oracle = {version="*", optional=true}
 vertica-python = {version="*", optional=true}
+urllib3 = "<2"
 
 [tool.poetry.dev-dependencies]
 parameterized = "*"
 unittest-parallel = "*"
 preql = "^0.2.19"
 mysql-connector-python = "*"
 psycopg2 = "*"
```

### Comparing `data_diff-0.7.6/PKG-INFO` & `data_diff-0.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-diff
-Version: 0.7.6
+Version: 0.7.7
 Summary: Command-line tool and Python library to efficiently diff rows across two different databases.
 Home-page: https://github.com/datafold/data-diff
 License: MIT
 Author: Datafold
 Author-email: data-diff@datafold.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -52,14 +52,15 @@
 Requires-Dist: psycopg2 ; extra == "postgresql" or extra == "redshift"
 Requires-Dist: rich
 Requires-Dist: runtype (>=0.2.6,<0.3.0)
 Requires-Dist: snowflake-connector-python (>=2.7.2,<3.0.0) ; extra == "snowflake"
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: trino (>=0.314.0,<0.315.0) ; extra == "trino"
+Requires-Dist: urllib3 (<2)
 Requires-Dist: vertica-python ; extra == "vertica"
 Project-URL: Repository, https://github.com/datafold/data-diff
 Description-Content-Type: text/markdown
 
 <p align="center">
     <img alt="Datafold" src="https://user-images.githubusercontent.com/1799931/196497110-d3de1113-a97f-4322-b531-026d859b867a.png" width="50%" />
 </p>
```

