# Comparing `tmp/awswrangler-3.1.0.tar.gz` & `tmp/awswrangler-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awswrangler-3.1.0.tar", max compression
+gzip compressed data, was "awswrangler-3.1.1.tar", max compression
```

## Comparing `awswrangler-3.1.0.tar` & `awswrangler-3.1.1.tar`

### file list

```diff
@@ -1,145 +1,145 @@
--rw-r--r--   0        0        0    10142 2022-08-02 16:44:38.861100 awswrangler-3.1.0/LICENSE.txt
--rw-r--r--   0        0        0       92 2022-09-01 20:50:36.683640 awswrangler-3.1.0/NOTICE.txt
--rw-r--r--   0        0        0    19946 2023-05-15 16:32:46.970048 awswrangler-3.1.0/README.md
--rw-r--r--   0        0        0    17494 2022-08-02 16:44:38.861401 awswrangler-3.1.0/THIRD_PARTY.txt
--rw-r--r--   0        0        0     1405 2023-04-21 16:06:31.383067 awswrangler-3.1.0/awswrangler/__init__.py
--rw-r--r--   0        0        0      276 2023-05-15 16:32:46.971384 awswrangler-3.1.0/awswrangler/__metadata__.py
--rw-r--r--   0        0        0     4359 2023-04-25 15:43:59.617624 awswrangler-3.1.0/awswrangler/_arrow.py
--rw-r--r--   0        0        0    27916 2023-05-02 21:22:41.635980 awswrangler-3.1.0/awswrangler/_config.py
--rw-r--r--   0        0        0    31116 2023-04-25 15:43:59.618486 awswrangler-3.1.0/awswrangler/_data_types.py
--rw-r--r--   0        0        0    13202 2023-05-02 20:57:29.199914 awswrangler-3.1.0/awswrangler/_databases.py
--rw-r--r--   0        0        0     6169 2023-04-21 16:06:31.387129 awswrangler-3.1.0/awswrangler/_distributed.py
--rw-r--r--   0        0        0     2063 2023-04-21 16:06:31.388005 awswrangler-3.1.0/awswrangler/_executor.py
--rw-r--r--   0        0        0     6211 2023-04-21 16:06:31.388148 awswrangler-3.1.0/awswrangler/_sql_formatter.py
--rw-r--r--   0        0        0    28878 2023-04-25 15:43:59.619218 awswrangler-3.1.0/awswrangler/_utils.py
--rw-r--r--   0        0        0     1701 2023-04-21 16:06:31.390428 awswrangler-3.1.0/awswrangler/annotations.py
--rw-r--r--   0        0        0     1190 2023-05-05 17:01:05.124627 awswrangler-3.1.0/awswrangler/athena/__init__.py
--rw-r--r--   0        0        0     9301 2023-04-21 16:06:31.390689 awswrangler-3.1.0/awswrangler/athena/_cache.py
--rw-r--r--   0        0        0     9681 2023-05-05 17:01:05.124758 awswrangler-3.1.0/awswrangler/athena/_executions.py
--rw-r--r--   0        0        0     2148 2023-05-05 17:01:05.124846 awswrangler-3.1.0/awswrangler/athena/_executions.pyi
--rw-r--r--   0        0        0    54600 2023-05-15 16:32:46.972287 awswrangler-3.1.0/awswrangler/athena/_read.py
--rw-r--r--   0        0        0    11526 2023-05-05 17:01:05.125558 awswrangler-3.1.0/awswrangler/athena/_read.pyi
--rw-r--r--   0        0        0    41939 2023-05-05 17:01:05.126045 awswrangler-3.1.0/awswrangler/athena/_utils.py
--rw-r--r--   0        0        0     7073 2023-05-05 17:01:05.126400 awswrangler-3.1.0/awswrangler/athena/_write_iceberg.py
--rw-r--r--   0        0        0     2414 2023-01-17 17:33:17.175478 awswrangler-3.1.0/awswrangler/catalog/__init__.py
--rw-r--r--   0        0        0    14077 2023-04-21 16:06:31.392981 awswrangler-3.1.0/awswrangler/catalog/_add.py
--rw-r--r--   0        0        0    50455 2023-04-21 16:06:31.393727 awswrangler-3.1.0/awswrangler/catalog/_create.py
--rw-r--r--   0        0        0    11466 2023-04-21 16:06:31.393962 awswrangler-3.1.0/awswrangler/catalog/_definitions.py
--rw-r--r--   0        0        0     8236 2023-04-21 16:06:31.394534 awswrangler-3.1.0/awswrangler/catalog/_delete.py
--rw-r--r--   0        0        0    36053 2023-04-21 16:06:31.395286 awswrangler-3.1.0/awswrangler/catalog/_get.py
--rw-r--r--   0        0        0    11233 2023-04-21 16:06:31.395700 awswrangler-3.1.0/awswrangler/catalog/_utils.py
--rw-r--r--   0        0        0     1199 2022-08-02 16:44:38.863657 awswrangler-3.1.0/awswrangler/chime.py
--rw-r--r--   0        0        0    16592 2023-04-21 16:06:31.396720 awswrangler-3.1.0/awswrangler/cloudwatch.py
--rw-r--r--   0        0        0      141 2022-08-02 16:44:38.863831 awswrangler-3.1.0/awswrangler/data_api/__init__.py
--rw-r--r--   0        0        0     2841 2023-04-21 16:06:31.396849 awswrangler-3.1.0/awswrangler/data_api/_connector.py
--rw-r--r--   0        0        0     5723 2023-04-21 16:06:31.397250 awswrangler-3.1.0/awswrangler/data_api/rds.py
--rw-r--r--   0        0        0     9547 2023-04-21 16:06:31.397699 awswrangler-3.1.0/awswrangler/data_api/redshift.py
--rw-r--r--   0        0        0      377 2023-01-17 17:33:17.179381 awswrangler-3.1.0/awswrangler/data_quality/__init__.py
--rw-r--r--   0        0        0    13403 2023-04-21 16:06:31.398627 awswrangler-3.1.0/awswrangler/data_quality/_create.py
--rw-r--r--   0        0        0     1404 2023-04-21 16:06:31.398990 awswrangler-3.1.0/awswrangler/data_quality/_get.py
--rw-r--r--   0        0        0     6550 2023-04-21 16:06:31.399880 awswrangler-3.1.0/awswrangler/data_quality/_utils.py
--rw-r--r--   0        0        0       26 2023-04-21 16:06:31.399991 awswrangler-3.1.0/awswrangler/distributed/__init__.py
--rw-r--r--   0        0        0      237 2023-04-21 16:06:31.400247 awswrangler-3.1.0/awswrangler/distributed/ray/__init__.py
--rw-r--r--   0        0        0     6256 2023-04-21 16:06:31.400358 awswrangler-3.1.0/awswrangler/distributed/ray/_core.py
--rw-r--r--   0        0        0      931 2023-04-21 16:06:31.400648 awswrangler-3.1.0/awswrangler/distributed/ray/_core.pyi
--rw-r--r--   0        0        0     2121 2023-04-21 16:06:31.400948 awswrangler-3.1.0/awswrangler/distributed/ray/_executor.py
--rw-r--r--   0        0        0     4239 2023-05-10 17:40:59.248347 awswrangler-3.1.0/awswrangler/distributed/ray/_register.py
--rw-r--r--   0        0        0     2443 2023-04-21 16:06:31.401571 awswrangler-3.1.0/awswrangler/distributed/ray/_utils.py
--rw-r--r--   0        0        0     1013 2023-04-21 16:06:31.401685 awswrangler-3.1.0/awswrangler/distributed/ray/datasources/__init__.py
--rw-r--r--   0        0        0     2191 2023-04-21 16:06:31.401968 awswrangler-3.1.0/awswrangler/distributed/ray/datasources/arrow_csv_datasource.py
--rw-r--r--   0        0        0     1273 2023-04-21 16:06:31.402074 awswrangler-3.1.0/awswrangler/distributed/ray/datasources/arrow_json_datasource.py
--rw-r--r--   0        0        0     3323 2023-05-05 18:06:21.358459 awswrangler-3.1.0/awswrangler/distributed/ray/datasources/arrow_parquet_base_datasource.py
--rw-r--r--   0        0        0    18476 2023-05-10 17:40:59.248836 awswrangler-3.1.0/awswrangler/distributed/ray/datasources/arrow_parquet_datasource.py
--rw-r--r--   0        0        0     8991 2023-05-15 14:41:37.788540 awswrangler-3.1.0/awswrangler/distributed/ray/datasources/pandas_file_based_datasource.py
--rw-r--r--   0        0        0     5896 2023-05-01 20:36:12.635110 awswrangler-3.1.0/awswrangler/distributed/ray/datasources/pandas_text_datasource.py
--rw-r--r--   0        0        0      135 2023-04-21 16:06:31.402995 awswrangler-3.1.0/awswrangler/distributed/ray/modin/__init__.py
--rw-r--r--   0        0        0     2524 2023-04-21 16:06:31.403517 awswrangler-3.1.0/awswrangler/distributed/ray/modin/_core.py
--rw-r--r--   0        0        0      929 2023-04-21 16:06:31.403611 awswrangler-3.1.0/awswrangler/distributed/ray/modin/_data_types.py
--rw-r--r--   0        0        0     4126 2023-04-25 15:43:59.620007 awswrangler-3.1.0/awswrangler/distributed/ray/modin/_utils.py
--rw-r--r--   0        0        0       27 2023-04-21 16:06:31.403997 awswrangler-3.1.0/awswrangler/distributed/ray/modin/s3/__init__.py
--rw-r--r--   0        0        0     1912 2023-05-15 16:16:27.394845 awswrangler-3.1.0/awswrangler/distributed/ray/modin/s3/_read_parquet.py
--rw-r--r--   0        0        0     5507 2023-04-21 16:06:31.404564 awswrangler-3.1.0/awswrangler/distributed/ray/modin/s3/_read_text.py
--rw-r--r--   0        0        0     7306 2023-04-21 16:06:31.405287 awswrangler-3.1.0/awswrangler/distributed/ray/modin/s3/_write_dataset.py
--rw-r--r--   0        0        0     3065 2023-04-21 16:06:31.405385 awswrangler-3.1.0/awswrangler/distributed/ray/modin/s3/_write_parquet.py
--rw-r--r--   0        0        0     5479 2023-05-10 17:40:59.250548 awswrangler-3.1.0/awswrangler/distributed/ray/modin/s3/_write_text.py
--rw-r--r--   0        0        0       21 2023-04-21 16:06:31.405975 awswrangler-3.1.0/awswrangler/distributed/ray/s3/__init__.py
--rw-r--r--   0        0        0     2413 2023-04-21 16:06:31.406055 awswrangler-3.1.0/awswrangler/distributed/ray/s3/_list.py
--rw-r--r--   0        0        0     1005 2023-04-21 16:06:31.406314 awswrangler-3.1.0/awswrangler/distributed/ray/s3/_read_parquet.py
--rw-r--r--   0        0        0      484 2023-05-04 22:03:58.498637 awswrangler-3.1.0/awswrangler/dynamodb/__init__.py
--rw-r--r--   0        0        0     1545 2023-04-21 16:06:31.406985 awswrangler-3.1.0/awswrangler/dynamodb/_delete.py
--rw-r--r--   0        0        0    24958 2023-05-05 17:01:05.126808 awswrangler-3.1.0/awswrangler/dynamodb/_read.py
--rw-r--r--   0        0        0     9045 2023-05-05 17:01:05.126904 awswrangler-3.1.0/awswrangler/dynamodb/_read.pyi
--rw-r--r--   0        0        0     6978 2023-05-05 17:01:05.127213 awswrangler-3.1.0/awswrangler/dynamodb/_utils.py
--rw-r--r--   0        0        0     8406 2023-04-21 16:06:31.408377 awswrangler-3.1.0/awswrangler/dynamodb/_write.py
--rw-r--r--   0        0        0    44390 2023-05-05 17:01:05.127643 awswrangler-3.1.0/awswrangler/emr.py
--rw-r--r--   0        0        0     2756 2023-05-02 21:22:41.637450 awswrangler-3.1.0/awswrangler/exceptions.py
--rw-r--r--   0        0        0      682 2023-04-13 20:06:09.276287 awswrangler-3.1.0/awswrangler/lakeformation/__init__.py
--rw-r--r--   0        0        0    10941 2023-04-21 16:06:31.410840 awswrangler-3.1.0/awswrangler/lakeformation/_read.py
--rw-r--r--   0        0        0    13151 2023-04-21 16:06:31.411661 awswrangler-3.1.0/awswrangler/lakeformation/_utils.py
--rw-r--r--   0        0        0    20293 2023-05-10 17:43:52.854565 awswrangler-3.1.0/awswrangler/mysql.py
--rw-r--r--   0        0        0      570 2023-05-02 21:22:41.638164 awswrangler-3.1.0/awswrangler/neptune/__init__.py
--rw-r--r--   0        0        0    12730 2023-05-10 17:40:54.870838 awswrangler-3.1.0/awswrangler/neptune/_client.py
--rw-r--r--   0        0        0      923 2023-04-21 16:06:31.412767 awswrangler-3.1.0/awswrangler/neptune/_gremlin_init.py
--rw-r--r--   0        0        0     2685 2023-05-10 17:40:54.871069 awswrangler-3.1.0/awswrangler/neptune/_gremlin_parser.py
--rw-r--r--   0        0        0    22208 2023-05-10 17:40:54.871423 awswrangler-3.1.0/awswrangler/neptune/_neptune.py
--rw-r--r--   0        0        0     3748 2023-04-21 16:06:31.413536 awswrangler-3.1.0/awswrangler/neptune/_utils.py
--rw-r--r--   0        0        0      502 2023-01-30 20:05:15.832378 awswrangler-3.1.0/awswrangler/opensearch/__init__.py
--rw-r--r--   0        0        0     6480 2023-05-10 17:40:54.871644 awswrangler-3.1.0/awswrangler/opensearch/_read.py
--rw-r--r--   0        0        0    13764 2023-05-10 17:40:54.872112 awswrangler-3.1.0/awswrangler/opensearch/_utils.py
--rw-r--r--   0        0        0    21509 2023-05-10 17:40:54.872409 awswrangler-3.1.0/awswrangler/opensearch/_write.py
--rw-r--r--   0        0        0    20931 2023-05-10 17:43:52.855383 awswrangler-3.1.0/awswrangler/oracle.py
--rw-r--r--   0        0        0     1595 2023-04-25 15:43:59.622719 awswrangler-3.1.0/awswrangler/pandas/__init__.py
--rw-r--r--   0        0        0    20629 2023-05-10 17:43:52.856222 awswrangler-3.1.0/awswrangler/postgresql.py
--rw-r--r--   0        0        0       27 2022-08-02 16:44:38.866284 awswrangler-3.1.0/awswrangler/py.typed
--rw-r--r--   0        0        0     2219 2023-01-17 17:33:17.208660 awswrangler-3.1.0/awswrangler/quicksight/__init__.py
--rw-r--r--   0        0        0     1906 2023-04-21 16:06:31.416913 awswrangler-3.1.0/awswrangler/quicksight/_cancel.py
--rw-r--r--   0        0        0    15508 2023-05-15 16:16:15.071628 awswrangler-3.1.0/awswrangler/quicksight/_create.py
--rw-r--r--   0        0        0    11710 2023-04-21 16:06:31.417954 awswrangler-3.1.0/awswrangler/quicksight/_delete.py
--rw-r--r--   0        0        0     8660 2023-04-21 16:06:31.418387 awswrangler-3.1.0/awswrangler/quicksight/_describe.py
--rw-r--r--   0        0        0    23657 2023-05-15 14:19:50.276077 awswrangler-3.1.0/awswrangler/quicksight/_get_list.py
--rw-r--r--   0        0        0     1929 2023-05-15 15:20:02.815523 awswrangler-3.1.0/awswrangler/quicksight/_utils.py
--rw-r--r--   0        0        0      440 2023-05-10 17:40:59.251591 awswrangler-3.1.0/awswrangler/redshift/__init__.py
--rw-r--r--   0        0        0     8809 2023-05-10 17:40:59.251715 awswrangler-3.1.0/awswrangler/redshift/_connect.py
--rw-r--r--   0        0        0    18905 2023-05-10 17:40:59.251876 awswrangler-3.1.0/awswrangler/redshift/_read.py
--rw-r--r--   0        0        0     6086 2023-05-10 17:40:59.251990 awswrangler-3.1.0/awswrangler/redshift/_read.pyi
--rw-r--r--   0        0        0    15681 2023-05-10 17:40:59.252145 awswrangler-3.1.0/awswrangler/redshift/_utils.py
--rw-r--r--   0        0        0    28318 2023-05-10 17:40:59.252324 awswrangler-3.1.0/awswrangler/redshift/_write.py
--rw-r--r--   0        0        0     1789 2023-05-02 21:22:41.642687 awswrangler-3.1.0/awswrangler/s3/__init__.py
--rw-r--r--   0        0        0    10594 2023-04-21 16:06:31.421145 awswrangler-3.1.0/awswrangler/s3/_copy.py
--rw-r--r--   0        0        0     5289 2023-04-21 16:06:31.421784 awswrangler-3.1.0/awswrangler/s3/_delete.py
--rw-r--r--   0        0        0     9327 2023-04-21 16:06:31.422180 awswrangler-3.1.0/awswrangler/s3/_describe.py
--rw-r--r--   0        0        0     2633 2023-01-30 20:05:15.841405 awswrangler-3.1.0/awswrangler/s3/_download.py
--rw-r--r--   0        0        0    23146 2023-04-21 16:06:31.422841 awswrangler-3.1.0/awswrangler/s3/_fs.py
--rw-r--r--   0        0        0    15683 2023-04-21 16:06:31.423159 awswrangler-3.1.0/awswrangler/s3/_list.py
--rw-r--r--   0        0        0     3970 2023-04-21 16:06:31.423979 awswrangler-3.1.0/awswrangler/s3/_list.pyi
--rw-r--r--   0        0        0     5342 2023-04-21 16:06:31.424139 awswrangler-3.1.0/awswrangler/s3/_read.py
--rw-r--r--   0        0        0     3471 2023-05-02 21:22:41.643295 awswrangler-3.1.0/awswrangler/s3/_read_deltalake.py
--rw-r--r--   0        0        0     3277 2023-05-10 17:40:54.875396 awswrangler-3.1.0/awswrangler/s3/_read_excel.py
--rw-r--r--   0        0        0    36296 2023-05-15 16:32:46.973134 awswrangler-3.1.0/awswrangler/s3/_read_parquet.py
--rw-r--r--   0        0        0     9380 2023-05-05 17:01:05.128332 awswrangler-3.1.0/awswrangler/s3/_read_parquet.pyi
--rw-r--r--   0        0        0    26728 2023-05-15 16:32:46.973775 awswrangler-3.1.0/awswrangler/s3/_read_text.py
--rw-r--r--   0        0        0     7577 2023-05-05 17:01:05.129193 awswrangler-3.1.0/awswrangler/s3/_read_text.pyi
--rw-r--r--   0        0        0     4108 2023-04-21 16:06:31.426375 awswrangler-3.1.0/awswrangler/s3/_read_text_core.py
--rw-r--r--   0        0        0    11991 2023-05-02 21:22:41.644182 awswrangler-3.1.0/awswrangler/s3/_select.py
--rw-r--r--   0        0        0     2465 2023-04-21 16:06:31.426801 awswrangler-3.1.0/awswrangler/s3/_upload.py
--rw-r--r--   0        0        0     6205 2023-04-21 16:06:31.427634 awswrangler-3.1.0/awswrangler/s3/_wait.py
--rw-r--r--   0        0        0     4715 2023-04-21 16:06:31.428073 awswrangler-3.1.0/awswrangler/s3/_write.py
--rw-r--r--   0        0        0     1840 2023-04-21 16:06:31.428436 awswrangler-3.1.0/awswrangler/s3/_write_concurrent.py
--rw-r--r--   0        0        0    12694 2023-04-21 16:06:31.428881 awswrangler-3.1.0/awswrangler/s3/_write_dataset.py
--rw-r--r--   0        0        0     4087 2023-05-02 21:22:41.644400 awswrangler-3.1.0/awswrangler/s3/_write_deltalake.py
--rw-r--r--   0        0        0     3196 2023-05-10 17:40:54.875751 awswrangler-3.1.0/awswrangler/s3/_write_excel.py
--rw-r--r--   0        0        0    43262 2023-05-15 16:32:46.974626 awswrangler-3.1.0/awswrangler/s3/_write_parquet.py
--rw-r--r--   0        0        0    48588 2023-05-15 16:32:46.975422 awswrangler-3.1.0/awswrangler/s3/_write_text.py
--rw-r--r--   0        0        0     2018 2023-04-21 16:06:31.431108 awswrangler-3.1.0/awswrangler/secretsmanager.py
--rw-r--r--   0        0        0    17975 2023-05-10 17:43:52.856811 awswrangler-3.1.0/awswrangler/sqlserver.py
--rw-r--r--   0        0        0     1853 2023-04-21 16:06:31.432014 awswrangler-3.1.0/awswrangler/sts.py
--rw-r--r--   0        0        0      644 2023-05-10 17:40:59.253502 awswrangler-3.1.0/awswrangler/timestream/__init__.py
--rw-r--r--   0        0        0     4512 2023-05-10 17:40:59.255448 awswrangler-3.1.0/awswrangler/timestream/_create.py
--rw-r--r--   0        0        0     2491 2023-05-10 17:40:59.255770 awswrangler-3.1.0/awswrangler/timestream/_delete.py
--rw-r--r--   0        0        0     2603 2023-05-15 14:41:20.785245 awswrangler-3.1.0/awswrangler/timestream/_list.py
--rw-r--r--   0        0        0     5881 2023-05-10 17:40:59.256502 awswrangler-3.1.0/awswrangler/timestream/_read.py
--rw-r--r--   0        0        0      722 2023-05-10 17:40:59.256775 awswrangler-3.1.0/awswrangler/timestream/_read.pyi
--rw-r--r--   0        0        0    26397 2023-05-10 17:40:59.257401 awswrangler-3.1.0/awswrangler/timestream/_write.py
--rw-r--r--   0        0        0     8983 2023-05-02 21:22:41.646552 awswrangler-3.1.0/awswrangler/typing.py
--rw-r--r--   0        0        0     4786 2023-05-15 16:32:46.977245 awswrangler-3.1.0/pyproject.toml
--rw-r--r--   0        0        0    22545 1970-01-01 00:00:00.000000 awswrangler-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0    10142 2022-08-02 16:44:38.861100 awswrangler-3.1.1/LICENSE.txt
+-rw-r--r--   0        0        0       92 2022-09-01 20:50:36.683640 awswrangler-3.1.1/NOTICE.txt
+-rw-r--r--   0        0        0    19946 2023-05-16 00:05:56.635964 awswrangler-3.1.1/README.md
+-rw-r--r--   0        0        0    17494 2022-08-02 16:44:38.861401 awswrangler-3.1.1/THIRD_PARTY.txt
+-rw-r--r--   0        0        0     1405 2023-04-21 16:06:31.383067 awswrangler-3.1.1/awswrangler/__init__.py
+-rw-r--r--   0        0        0      276 2023-05-16 00:05:56.636826 awswrangler-3.1.1/awswrangler/__metadata__.py
+-rw-r--r--   0        0        0     4359 2023-04-25 15:43:59.617624 awswrangler-3.1.1/awswrangler/_arrow.py
+-rw-r--r--   0        0        0    27916 2023-05-02 21:22:41.635980 awswrangler-3.1.1/awswrangler/_config.py
+-rw-r--r--   0        0        0    31116 2023-04-25 15:43:59.618486 awswrangler-3.1.1/awswrangler/_data_types.py
+-rw-r--r--   0        0        0    13202 2023-05-02 20:57:29.199914 awswrangler-3.1.1/awswrangler/_databases.py
+-rw-r--r--   0        0        0     6169 2023-04-21 16:06:31.387129 awswrangler-3.1.1/awswrangler/_distributed.py
+-rw-r--r--   0        0        0     2063 2023-04-21 16:06:31.388005 awswrangler-3.1.1/awswrangler/_executor.py
+-rw-r--r--   0        0        0     6211 2023-04-21 16:06:31.388148 awswrangler-3.1.1/awswrangler/_sql_formatter.py
+-rw-r--r--   0        0        0    28878 2023-04-25 15:43:59.619218 awswrangler-3.1.1/awswrangler/_utils.py
+-rw-r--r--   0        0        0     1701 2023-04-21 16:06:31.390428 awswrangler-3.1.1/awswrangler/annotations.py
+-rw-r--r--   0        0        0     1190 2023-05-05 17:01:05.124627 awswrangler-3.1.1/awswrangler/athena/__init__.py
+-rw-r--r--   0        0        0     9301 2023-04-21 16:06:31.390689 awswrangler-3.1.1/awswrangler/athena/_cache.py
+-rw-r--r--   0        0        0     9681 2023-05-05 17:01:05.124758 awswrangler-3.1.1/awswrangler/athena/_executions.py
+-rw-r--r--   0        0        0     2148 2023-05-05 17:01:05.124846 awswrangler-3.1.1/awswrangler/athena/_executions.pyi
+-rw-r--r--   0        0        0    54600 2023-05-16 00:05:56.637451 awswrangler-3.1.1/awswrangler/athena/_read.py
+-rw-r--r--   0        0        0    11526 2023-05-05 17:01:05.125558 awswrangler-3.1.1/awswrangler/athena/_read.pyi
+-rw-r--r--   0        0        0    41939 2023-05-05 17:01:05.126045 awswrangler-3.1.1/awswrangler/athena/_utils.py
+-rw-r--r--   0        0        0     7073 2023-05-05 17:01:05.126400 awswrangler-3.1.1/awswrangler/athena/_write_iceberg.py
+-rw-r--r--   0        0        0     2414 2023-01-17 17:33:17.175478 awswrangler-3.1.1/awswrangler/catalog/__init__.py
+-rw-r--r--   0        0        0    14077 2023-04-21 16:06:31.392981 awswrangler-3.1.1/awswrangler/catalog/_add.py
+-rw-r--r--   0        0        0    50455 2023-04-21 16:06:31.393727 awswrangler-3.1.1/awswrangler/catalog/_create.py
+-rw-r--r--   0        0        0    11466 2023-04-21 16:06:31.393962 awswrangler-3.1.1/awswrangler/catalog/_definitions.py
+-rw-r--r--   0        0        0     8236 2023-04-21 16:06:31.394534 awswrangler-3.1.1/awswrangler/catalog/_delete.py
+-rw-r--r--   0        0        0    36053 2023-04-21 16:06:31.395286 awswrangler-3.1.1/awswrangler/catalog/_get.py
+-rw-r--r--   0        0        0    11233 2023-04-21 16:06:31.395700 awswrangler-3.1.1/awswrangler/catalog/_utils.py
+-rw-r--r--   0        0        0     1199 2022-08-02 16:44:38.863657 awswrangler-3.1.1/awswrangler/chime.py
+-rw-r--r--   0        0        0    16592 2023-04-21 16:06:31.396720 awswrangler-3.1.1/awswrangler/cloudwatch.py
+-rw-r--r--   0        0        0      141 2022-08-02 16:44:38.863831 awswrangler-3.1.1/awswrangler/data_api/__init__.py
+-rw-r--r--   0        0        0     2841 2023-04-21 16:06:31.396849 awswrangler-3.1.1/awswrangler/data_api/_connector.py
+-rw-r--r--   0        0        0     5723 2023-04-21 16:06:31.397250 awswrangler-3.1.1/awswrangler/data_api/rds.py
+-rw-r--r--   0        0        0     9547 2023-04-21 16:06:31.397699 awswrangler-3.1.1/awswrangler/data_api/redshift.py
+-rw-r--r--   0        0        0      377 2023-01-17 17:33:17.179381 awswrangler-3.1.1/awswrangler/data_quality/__init__.py
+-rw-r--r--   0        0        0    13403 2023-04-21 16:06:31.398627 awswrangler-3.1.1/awswrangler/data_quality/_create.py
+-rw-r--r--   0        0        0     1404 2023-04-21 16:06:31.398990 awswrangler-3.1.1/awswrangler/data_quality/_get.py
+-rw-r--r--   0        0        0     6550 2023-04-21 16:06:31.399880 awswrangler-3.1.1/awswrangler/data_quality/_utils.py
+-rw-r--r--   0        0        0       26 2023-04-21 16:06:31.399991 awswrangler-3.1.1/awswrangler/distributed/__init__.py
+-rw-r--r--   0        0        0      237 2023-04-21 16:06:31.400247 awswrangler-3.1.1/awswrangler/distributed/ray/__init__.py
+-rw-r--r--   0        0        0     6256 2023-04-21 16:06:31.400358 awswrangler-3.1.1/awswrangler/distributed/ray/_core.py
+-rw-r--r--   0        0        0      931 2023-04-21 16:06:31.400648 awswrangler-3.1.1/awswrangler/distributed/ray/_core.pyi
+-rw-r--r--   0        0        0     2121 2023-04-21 16:06:31.400948 awswrangler-3.1.1/awswrangler/distributed/ray/_executor.py
+-rw-r--r--   0        0        0     4239 2023-05-10 17:40:59.248347 awswrangler-3.1.1/awswrangler/distributed/ray/_register.py
+-rw-r--r--   0        0        0     2443 2023-04-21 16:06:31.401571 awswrangler-3.1.1/awswrangler/distributed/ray/_utils.py
+-rw-r--r--   0        0        0     1013 2023-04-21 16:06:31.401685 awswrangler-3.1.1/awswrangler/distributed/ray/datasources/__init__.py
+-rw-r--r--   0        0        0     2191 2023-04-21 16:06:31.401968 awswrangler-3.1.1/awswrangler/distributed/ray/datasources/arrow_csv_datasource.py
+-rw-r--r--   0        0        0     1273 2023-04-21 16:06:31.402074 awswrangler-3.1.1/awswrangler/distributed/ray/datasources/arrow_json_datasource.py
+-rw-r--r--   0        0        0     3323 2023-05-05 18:06:21.358459 awswrangler-3.1.1/awswrangler/distributed/ray/datasources/arrow_parquet_base_datasource.py
+-rw-r--r--   0        0        0    18476 2023-05-15 20:31:05.631250 awswrangler-3.1.1/awswrangler/distributed/ray/datasources/arrow_parquet_datasource.py
+-rw-r--r--   0        0        0     8991 2023-05-15 23:11:38.901422 awswrangler-3.1.1/awswrangler/distributed/ray/datasources/pandas_file_based_datasource.py
+-rw-r--r--   0        0        0     5896 2023-05-01 20:36:12.635110 awswrangler-3.1.1/awswrangler/distributed/ray/datasources/pandas_text_datasource.py
+-rw-r--r--   0        0        0      135 2023-04-21 16:06:31.402995 awswrangler-3.1.1/awswrangler/distributed/ray/modin/__init__.py
+-rw-r--r--   0        0        0     2524 2023-04-21 16:06:31.403517 awswrangler-3.1.1/awswrangler/distributed/ray/modin/_core.py
+-rw-r--r--   0        0        0      929 2023-04-21 16:06:31.403611 awswrangler-3.1.1/awswrangler/distributed/ray/modin/_data_types.py
+-rw-r--r--   0        0        0     4126 2023-04-25 15:43:59.620007 awswrangler-3.1.1/awswrangler/distributed/ray/modin/_utils.py
+-rw-r--r--   0        0        0       27 2023-04-21 16:06:31.403997 awswrangler-3.1.1/awswrangler/distributed/ray/modin/s3/__init__.py
+-rw-r--r--   0        0        0     1912 2023-05-15 18:43:51.641408 awswrangler-3.1.1/awswrangler/distributed/ray/modin/s3/_read_parquet.py
+-rw-r--r--   0        0        0     5507 2023-04-21 16:06:31.404564 awswrangler-3.1.1/awswrangler/distributed/ray/modin/s3/_read_text.py
+-rw-r--r--   0        0        0     7306 2023-04-21 16:06:31.405287 awswrangler-3.1.1/awswrangler/distributed/ray/modin/s3/_write_dataset.py
+-rw-r--r--   0        0        0     3065 2023-04-21 16:06:31.405385 awswrangler-3.1.1/awswrangler/distributed/ray/modin/s3/_write_parquet.py
+-rw-r--r--   0        0        0     5479 2023-05-15 20:31:05.633385 awswrangler-3.1.1/awswrangler/distributed/ray/modin/s3/_write_text.py
+-rw-r--r--   0        0        0       21 2023-04-21 16:06:31.405975 awswrangler-3.1.1/awswrangler/distributed/ray/s3/__init__.py
+-rw-r--r--   0        0        0     2413 2023-04-21 16:06:31.406055 awswrangler-3.1.1/awswrangler/distributed/ray/s3/_list.py
+-rw-r--r--   0        0        0     1005 2023-04-21 16:06:31.406314 awswrangler-3.1.1/awswrangler/distributed/ray/s3/_read_parquet.py
+-rw-r--r--   0        0        0      484 2023-05-04 22:03:58.498637 awswrangler-3.1.1/awswrangler/dynamodb/__init__.py
+-rw-r--r--   0        0        0     1545 2023-04-21 16:06:31.406985 awswrangler-3.1.1/awswrangler/dynamodb/_delete.py
+-rw-r--r--   0        0        0    24958 2023-05-05 17:01:05.126808 awswrangler-3.1.1/awswrangler/dynamodb/_read.py
+-rw-r--r--   0        0        0     9045 2023-05-05 17:01:05.126904 awswrangler-3.1.1/awswrangler/dynamodb/_read.pyi
+-rw-r--r--   0        0        0     6978 2023-05-05 17:01:05.127213 awswrangler-3.1.1/awswrangler/dynamodb/_utils.py
+-rw-r--r--   0        0        0     8406 2023-04-21 16:06:31.408377 awswrangler-3.1.1/awswrangler/dynamodb/_write.py
+-rw-r--r--   0        0        0    44390 2023-05-05 17:01:05.127643 awswrangler-3.1.1/awswrangler/emr.py
+-rw-r--r--   0        0        0     2756 2023-05-02 21:22:41.637450 awswrangler-3.1.1/awswrangler/exceptions.py
+-rw-r--r--   0        0        0      682 2023-04-13 20:06:09.276287 awswrangler-3.1.1/awswrangler/lakeformation/__init__.py
+-rw-r--r--   0        0        0    10941 2023-04-21 16:06:31.410840 awswrangler-3.1.1/awswrangler/lakeformation/_read.py
+-rw-r--r--   0        0        0    13151 2023-04-21 16:06:31.411661 awswrangler-3.1.1/awswrangler/lakeformation/_utils.py
+-rw-r--r--   0        0        0    20293 2023-05-15 23:11:38.902130 awswrangler-3.1.1/awswrangler/mysql.py
+-rw-r--r--   0        0        0      570 2023-05-02 21:22:41.638164 awswrangler-3.1.1/awswrangler/neptune/__init__.py
+-rw-r--r--   0        0        0    12730 2023-05-15 20:31:18.255917 awswrangler-3.1.1/awswrangler/neptune/_client.py
+-rw-r--r--   0        0        0      923 2023-04-21 16:06:31.412767 awswrangler-3.1.1/awswrangler/neptune/_gremlin_init.py
+-rw-r--r--   0        0        0     2685 2023-05-15 20:31:18.256245 awswrangler-3.1.1/awswrangler/neptune/_gremlin_parser.py
+-rw-r--r--   0        0        0    22208 2023-05-15 20:31:18.256641 awswrangler-3.1.1/awswrangler/neptune/_neptune.py
+-rw-r--r--   0        0        0     3748 2023-04-21 16:06:31.413536 awswrangler-3.1.1/awswrangler/neptune/_utils.py
+-rw-r--r--   0        0        0      502 2023-01-30 20:05:15.832378 awswrangler-3.1.1/awswrangler/opensearch/__init__.py
+-rw-r--r--   0        0        0     6480 2023-05-15 20:31:18.256995 awswrangler-3.1.1/awswrangler/opensearch/_read.py
+-rw-r--r--   0        0        0    13764 2023-05-15 20:31:18.257329 awswrangler-3.1.1/awswrangler/opensearch/_utils.py
+-rw-r--r--   0        0        0    21509 2023-05-15 20:31:18.257745 awswrangler-3.1.1/awswrangler/opensearch/_write.py
+-rw-r--r--   0        0        0    20931 2023-05-15 23:11:38.903127 awswrangler-3.1.1/awswrangler/oracle.py
+-rw-r--r--   0        0        0     1595 2023-05-15 23:11:28.066397 awswrangler-3.1.1/awswrangler/pandas/__init__.py
+-rw-r--r--   0        0        0    20629 2023-05-15 23:11:38.904222 awswrangler-3.1.1/awswrangler/postgresql.py
+-rw-r--r--   0        0        0       27 2022-08-02 16:44:38.866284 awswrangler-3.1.1/awswrangler/py.typed
+-rw-r--r--   0        0        0     2219 2023-01-17 17:33:17.208660 awswrangler-3.1.1/awswrangler/quicksight/__init__.py
+-rw-r--r--   0        0        0     1906 2023-04-21 16:06:31.416913 awswrangler-3.1.1/awswrangler/quicksight/_cancel.py
+-rw-r--r--   0        0        0    15508 2023-05-15 22:16:43.536525 awswrangler-3.1.1/awswrangler/quicksight/_create.py
+-rw-r--r--   0        0        0    11710 2023-04-21 16:06:31.417954 awswrangler-3.1.1/awswrangler/quicksight/_delete.py
+-rw-r--r--   0        0        0     8660 2023-04-21 16:06:31.418387 awswrangler-3.1.1/awswrangler/quicksight/_describe.py
+-rw-r--r--   0        0        0    23657 2023-05-15 14:19:50.276077 awswrangler-3.1.1/awswrangler/quicksight/_get_list.py
+-rw-r--r--   0        0        0     1929 2023-05-15 22:16:43.536932 awswrangler-3.1.1/awswrangler/quicksight/_utils.py
+-rw-r--r--   0        0        0      440 2023-05-10 17:40:59.251591 awswrangler-3.1.1/awswrangler/redshift/__init__.py
+-rw-r--r--   0        0        0     8809 2023-05-15 20:31:18.259025 awswrangler-3.1.1/awswrangler/redshift/_connect.py
+-rw-r--r--   0        0        0    18905 2023-05-15 20:31:18.259447 awswrangler-3.1.1/awswrangler/redshift/_read.py
+-rw-r--r--   0        0        0     6086 2023-05-10 17:40:59.251990 awswrangler-3.1.1/awswrangler/redshift/_read.pyi
+-rw-r--r--   0        0        0    15681 2023-05-15 20:31:18.259784 awswrangler-3.1.1/awswrangler/redshift/_utils.py
+-rw-r--r--   0        0        0    28318 2023-05-15 20:31:18.260094 awswrangler-3.1.1/awswrangler/redshift/_write.py
+-rw-r--r--   0        0        0     1789 2023-05-02 21:22:41.642687 awswrangler-3.1.1/awswrangler/s3/__init__.py
+-rw-r--r--   0        0        0    10594 2023-04-21 16:06:31.421145 awswrangler-3.1.1/awswrangler/s3/_copy.py
+-rw-r--r--   0        0        0     5289 2023-04-21 16:06:31.421784 awswrangler-3.1.1/awswrangler/s3/_delete.py
+-rw-r--r--   0        0        0     9327 2023-04-21 16:06:31.422180 awswrangler-3.1.1/awswrangler/s3/_describe.py
+-rw-r--r--   0        0        0     2633 2023-01-30 20:05:15.841405 awswrangler-3.1.1/awswrangler/s3/_download.py
+-rw-r--r--   0        0        0    23146 2023-04-21 16:06:31.422841 awswrangler-3.1.1/awswrangler/s3/_fs.py
+-rw-r--r--   0        0        0    15683 2023-04-21 16:06:31.423159 awswrangler-3.1.1/awswrangler/s3/_list.py
+-rw-r--r--   0        0        0     3970 2023-04-21 16:06:31.423979 awswrangler-3.1.1/awswrangler/s3/_list.pyi
+-rw-r--r--   0        0        0     5342 2023-04-21 16:06:31.424139 awswrangler-3.1.1/awswrangler/s3/_read.py
+-rw-r--r--   0        0        0     3471 2023-05-02 21:22:41.643295 awswrangler-3.1.1/awswrangler/s3/_read_deltalake.py
+-rw-r--r--   0        0        0     3277 2023-05-15 20:31:18.260401 awswrangler-3.1.1/awswrangler/s3/_read_excel.py
+-rw-r--r--   0        0        0    36296 2023-05-16 00:05:56.638034 awswrangler-3.1.1/awswrangler/s3/_read_parquet.py
+-rw-r--r--   0        0        0     9380 2023-05-05 17:01:05.128332 awswrangler-3.1.1/awswrangler/s3/_read_parquet.pyi
+-rw-r--r--   0        0        0    26728 2023-05-16 00:05:56.638491 awswrangler-3.1.1/awswrangler/s3/_read_text.py
+-rw-r--r--   0        0        0     7577 2023-05-05 17:01:05.129193 awswrangler-3.1.1/awswrangler/s3/_read_text.pyi
+-rw-r--r--   0        0        0     4108 2023-04-21 16:06:31.426375 awswrangler-3.1.1/awswrangler/s3/_read_text_core.py
+-rw-r--r--   0        0        0    11991 2023-05-02 21:22:41.644182 awswrangler-3.1.1/awswrangler/s3/_select.py
+-rw-r--r--   0        0        0     2465 2023-04-21 16:06:31.426801 awswrangler-3.1.1/awswrangler/s3/_upload.py
+-rw-r--r--   0        0        0     6205 2023-04-21 16:06:31.427634 awswrangler-3.1.1/awswrangler/s3/_wait.py
+-rw-r--r--   0        0        0     4715 2023-04-21 16:06:31.428073 awswrangler-3.1.1/awswrangler/s3/_write.py
+-rw-r--r--   0        0        0     1840 2023-04-21 16:06:31.428436 awswrangler-3.1.1/awswrangler/s3/_write_concurrent.py
+-rw-r--r--   0        0        0    12694 2023-04-21 16:06:31.428881 awswrangler-3.1.1/awswrangler/s3/_write_dataset.py
+-rw-r--r--   0        0        0     4087 2023-05-02 21:22:41.644400 awswrangler-3.1.1/awswrangler/s3/_write_deltalake.py
+-rw-r--r--   0        0        0     3196 2023-05-15 20:31:18.260647 awswrangler-3.1.1/awswrangler/s3/_write_excel.py
+-rw-r--r--   0        0        0    43262 2023-05-16 00:05:56.639011 awswrangler-3.1.1/awswrangler/s3/_write_parquet.py
+-rw-r--r--   0        0        0    48588 2023-05-16 00:05:56.639505 awswrangler-3.1.1/awswrangler/s3/_write_text.py
+-rw-r--r--   0        0        0     2018 2023-04-21 16:06:31.431108 awswrangler-3.1.1/awswrangler/secretsmanager.py
+-rw-r--r--   0        0        0    17975 2023-05-15 23:11:38.908565 awswrangler-3.1.1/awswrangler/sqlserver.py
+-rw-r--r--   0        0        0     1853 2023-04-21 16:06:31.432014 awswrangler-3.1.1/awswrangler/sts.py
+-rw-r--r--   0        0        0      644 2023-05-10 17:40:59.253502 awswrangler-3.1.1/awswrangler/timestream/__init__.py
+-rw-r--r--   0        0        0     4512 2023-05-10 17:40:59.255448 awswrangler-3.1.1/awswrangler/timestream/_create.py
+-rw-r--r--   0        0        0     2491 2023-05-10 17:40:59.255770 awswrangler-3.1.1/awswrangler/timestream/_delete.py
+-rw-r--r--   0        0        0     2603 2023-05-15 23:11:38.909361 awswrangler-3.1.1/awswrangler/timestream/_list.py
+-rw-r--r--   0        0        0     5881 2023-05-10 17:40:59.256502 awswrangler-3.1.1/awswrangler/timestream/_read.py
+-rw-r--r--   0        0        0      722 2023-05-10 17:40:59.256775 awswrangler-3.1.1/awswrangler/timestream/_read.pyi
+-rw-r--r--   0        0        0    26397 2023-05-15 20:31:05.639995 awswrangler-3.1.1/awswrangler/timestream/_write.py
+-rw-r--r--   0        0        0     8983 2023-05-02 21:22:41.646552 awswrangler-3.1.1/awswrangler/typing.py
+-rw-r--r--   0        0        0     4806 2023-05-16 00:05:56.640136 awswrangler-3.1.1/pyproject.toml
+-rw-r--r--   0        0        0    22585 1970-01-01 00:00:00.000000 awswrangler-3.1.1/PKG-INFO
```

### Comparing `awswrangler-3.1.0/LICENSE.txt` & `awswrangler-3.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/README.md` & `awswrangler-3.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 Easy integration with Athena, Glue, Redshift, Timestream, OpenSearch, Neptune, QuickSight, Chime, CloudWatchLogs, DynamoDB, EMR, SecretManager, PostgreSQL, MySQL, SQLServer and S3 (Parquet, CSV, JSON and EXCEL).
 
 ![AWS SDK for pandas](docs/source/_static/logo2.png?raw=true "AWS SDK for pandas")
 ![tracker](https://d3tiqpr4kkkomd.cloudfront.net/img/pixel.png?asset=GVOYN2BOOQ573LTVIHEW)
 
 > An [AWS Professional Service](https://aws.amazon.com/professional-services/) open source initiative | aws-proserve-opensource@amazon.com
 
-[![Release](https://img.shields.io/badge/3.1.0-brightgreen.svg)](https://pypi.org/project/awswrangler/)
+[![Release](https://img.shields.io/badge/3.1.1-brightgreen.svg)](https://pypi.org/project/awswrangler/)
 [![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.8%20%7C%203.9%20%7C%203.10-brightgreen.svg)](https://anaconda.org/conda-forge/awswrangler)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 ![Static Checking](https://github.com/aws/aws-sdk-pandas/workflows/Static%20Checking/badge.svg?branch=main)
 [![Documentation Status](https://readthedocs.org/projects/aws-sdk-pandas/badge/?version=latest)](https://aws-sdk-pandas.readthedocs.io/?badge=latest)
@@ -95,33 +95,33 @@
 """)
 
 ```
 
 ## At scale
 AWS SDK for pandas can also run your workflows at scale by leveraging [Modin](https://modin.readthedocs.io/en/stable/) and [Ray](https://www.ray.io/). Both projects aim to speed up data workloads by distributing processing over a cluster of workers.
 
-The quickest way to get started is to use AWS Glue with Ray. Read our [docs](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/scale.html), our [blog](https://aws.amazon.com/blogs/big-data/scale-aws-sdk-for-pandas-workloads-with-aws-glue-for-ray/), or head to our latest [tutorials](https://github.com/aws/aws-sdk-pandas/tree/main/tutorials) to discover even more features.
+The quickest way to get started is to use AWS Glue with Ray. Read our [docs](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/scale.html), our [blog](https://aws.amazon.com/blogs/big-data/scale-aws-sdk-for-pandas-workloads-with-aws-glue-for-ray/), or head to our latest [tutorials](https://github.com/aws/aws-sdk-pandas/tree/main/tutorials) to discover even more features.
 
 ## [Read The Docs](https://aws-sdk-pandas.readthedocs.io/)
 
-- [**What is AWS SDK for pandas?**](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/about.html)
-- [**Install**](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/install.html)
-  - [PyPi (pip)](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/install.html#pypi-pip)
-  - [Conda](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/install.html#conda)
-  - [AWS Lambda Layer](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/install.html#aws-lambda-layer)
-  - [AWS Glue Python Shell Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/install.html#aws-glue-python-shell-jobs)
-  - [AWS Glue PySpark Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/install.html#aws-glue-pyspark-jobs)
-  - [Amazon SageMaker Notebook](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/install.html#amazon-sagemaker-notebook)
-  - [Amazon SageMaker Notebook Lifecycle](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/install.html#amazon-sagemaker-notebook-lifecycle)
-  - [EMR](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/install.html#emr)
-  - [From source](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/install.html#from-source)
-- [**At scale**](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/scale.html)
-  - [Getting Started](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/scale.html#getting-started)
-  - [Supported APIs](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/scale.html#supported-apis)
-  - [Resources](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/scale.html#resources)
+- [**What is AWS SDK for pandas?**](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/about.html)
+- [**Install**](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/install.html)
+  - [PyPi (pip)](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/install.html#pypi-pip)
+  - [Conda](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/install.html#conda)
+  - [AWS Lambda Layer](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/install.html#aws-lambda-layer)
+  - [AWS Glue Python Shell Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/install.html#aws-glue-python-shell-jobs)
+  - [AWS Glue PySpark Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/install.html#aws-glue-pyspark-jobs)
+  - [Amazon SageMaker Notebook](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/install.html#amazon-sagemaker-notebook)
+  - [Amazon SageMaker Notebook Lifecycle](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/install.html#amazon-sagemaker-notebook-lifecycle)
+  - [EMR](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/install.html#emr)
+  - [From source](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/install.html#from-source)
+- [**At scale**](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/scale.html)
+  - [Getting Started](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/scale.html#getting-started)
+  - [Supported APIs](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/scale.html#supported-apis)
+  - [Resources](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/scale.html#resources)
 - [**Tutorials**](https://github.com/aws/aws-sdk-pandas/tree/main/tutorials)
   - [001 - Introduction](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/001%20-%20Introduction.ipynb)
   - [002 - Sessions](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/002%20-%20Sessions.ipynb)
   - [003 - Amazon S3](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/003%20-%20Amazon%20S3.ipynb)
   - [004 - Parquet Datasets](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/004%20-%20Parquet%20Datasets.ipynb)
   - [005 - Glue Catalog](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/005%20-%20Glue%20Catalog.ipynb)
   - [006 - Amazon Athena](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/006%20-%20Amazon%20Athena.ipynb)
@@ -154,39 +154,39 @@
   - [033 - Amazon Neptune](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/033%20-%20Amazon%20Neptune.ipynb)
   - [034 - Distributing Calls Using Ray](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/034%20-%20Distributing%20Calls%20using%20Ray.ipynb)
   - [035 - Distributing Calls on Ray Remote Cluster](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/035%20-%20Distributing%20Calls%20on%20Ray%20Remote%20Cluster.ipynb)
   - [036 - Distributing Calls with Glue Interactive Sessions on Ray](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/036%20-%20Distributing%20Calls%20with%20Glue%20Interactive%20Sessions%20on%20Ray.ipynb)
   - [037 - Glue Data Quality](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/037%20-%20Glue%20Data%20Quality.ipynb)
   - [038 - OpenSearch Serverless](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/038%20-%20OpenSearch%20Serverless.ipynb)
   - [039 - Athena Iceberg](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/039%20-%20Athena%20Iceberg.ipynb)
-- [**API Reference**](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html)
-  - [Amazon S3](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#amazon-s3)
-  - [AWS Glue Catalog](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#aws-glue-catalog)
-  - [Amazon Athena](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#amazon-athena)
-  - [AWS Lake Formation](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#aws-lake-formation)
-  - [Amazon Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#amazon-redshift)
-  - [PostgreSQL](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#postgresql)
-  - [MySQL](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#mysql)
-  - [SQL Server](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#sqlserver)
-  - [Oracle](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#oracle)
-  - [Data API Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#data-api-redshift)
-  - [Data API RDS](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#data-api-rds)
-  - [OpenSearch](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#opensearch)
-  - [AWS Glue Data Quality](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#aws-glue-data-quality)
-  - [Amazon Neptune](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#amazon-neptune)
-  - [DynamoDB](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#dynamodb)
-  - [Amazon Timestream](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#amazon-timestream)
-  - [Amazon EMR](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#amazon-emr)
-  - [Amazon CloudWatch Logs](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#amazon-cloudwatch-logs)
-  - [Amazon Chime](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#amazon-chime)
-  - [Amazon QuickSight](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#amazon-quicksight)
-  - [AWS STS](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#aws-sts)
-  - [AWS Secrets Manager](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#aws-secrets-manager)
-  - [Global Configurations](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#global-configurations)
-  - [Distributed - Ray](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#distributed-ray)
+- [**API Reference**](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html)
+  - [Amazon S3](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#amazon-s3)
+  - [AWS Glue Catalog](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#aws-glue-catalog)
+  - [Amazon Athena](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#amazon-athena)
+  - [AWS Lake Formation](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#aws-lake-formation)
+  - [Amazon Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#amazon-redshift)
+  - [PostgreSQL](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#postgresql)
+  - [MySQL](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#mysql)
+  - [SQL Server](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#sqlserver)
+  - [Oracle](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#oracle)
+  - [Data API Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#data-api-redshift)
+  - [Data API RDS](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#data-api-rds)
+  - [OpenSearch](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#opensearch)
+  - [AWS Glue Data Quality](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#aws-glue-data-quality)
+  - [Amazon Neptune](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#amazon-neptune)
+  - [DynamoDB](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#dynamodb)
+  - [Amazon Timestream](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#amazon-timestream)
+  - [Amazon EMR](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#amazon-emr)
+  - [Amazon CloudWatch Logs](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#amazon-cloudwatch-logs)
+  - [Amazon Chime](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#amazon-chime)
+  - [Amazon QuickSight](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#amazon-quicksight)
+  - [AWS STS](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#aws-sts)
+  - [AWS Secrets Manager](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#aws-secrets-manager)
+  - [Global Configurations](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#global-configurations)
+  - [Distributed - Ray](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#distributed-ray)
 - [**License**](https://github.com/aws/aws-sdk-pandas/blob/main/LICENSE.txt)
 - [**Contributing**](https://github.com/aws/aws-sdk-pandas/blob/main/CONTRIBUTING.md)
 
 ## Getting Help
 
 The best way to interact with our team is through GitHub. You can open an [issue](https://github.com/aws/aws-sdk-pandas/issues/new/choose) and choose from one of our templates for bug reports, feature requests...
 You may also find help on these community resources:
```

### Comparing `awswrangler-3.1.0/THIRD_PARTY.txt` & `awswrangler-3.1.1/THIRD_PARTY.txt`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/__init__.py` & `awswrangler-3.1.1/awswrangler/__init__.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/_arrow.py` & `awswrangler-3.1.1/awswrangler/_arrow.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/_config.py` & `awswrangler-3.1.1/awswrangler/_config.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/_data_types.py` & `awswrangler-3.1.1/awswrangler/_data_types.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/_databases.py` & `awswrangler-3.1.1/awswrangler/_databases.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/_distributed.py` & `awswrangler-3.1.1/awswrangler/_distributed.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/_executor.py` & `awswrangler-3.1.1/awswrangler/_executor.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/_sql_formatter.py` & `awswrangler-3.1.1/awswrangler/_sql_formatter.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/_utils.py` & `awswrangler-3.1.1/awswrangler/_utils.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/annotations.py` & `awswrangler-3.1.1/awswrangler/annotations.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/athena/__init__.py` & `awswrangler-3.1.1/awswrangler/athena/__init__.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/athena/_cache.py` & `awswrangler-3.1.1/awswrangler/athena/_cache.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/athena/_executions.py` & `awswrangler-3.1.1/awswrangler/athena/_executions.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/athena/_executions.pyi` & `awswrangler-3.1.1/awswrangler/athena/_executions.pyi`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/athena/_read.py` & `awswrangler-3.1.1/awswrangler/athena/_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -712,19 +712,19 @@
     s3_additional_kwargs: Optional[Dict[str, Any]] = None,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     """Execute any SQL query on AWS Athena and return the results as a Pandas DataFrame.
 
     **Related tutorial:**
 
-    - `Amazon Athena <https://aws-sdk-pandas.readthedocs.io/en/3.1.0/
+    - `Amazon Athena <https://aws-sdk-pandas.readthedocs.io/en/3.1.1/
       tutorials/006%20-%20Amazon%20Athena.html>`_
-    - `Athena Cache <https://aws-sdk-pandas.readthedocs.io/en/3.1.0/
+    - `Athena Cache <https://aws-sdk-pandas.readthedocs.io/en/3.1.1/
       tutorials/019%20-%20Athena%20Cache.html>`_
-    - `Global Configurations <https://aws-sdk-pandas.readthedocs.io/en/3.1.0/
+    - `Global Configurations <https://aws-sdk-pandas.readthedocs.io/en/3.1.1/
       tutorials/021%20-%20Global%20Configurations.html>`_
 
     **There are three approaches available through ctas_approach and unload_approach parameters:**
 
     **1** - ctas_approach=True (Default):
 
     Wrap the query with a CTAS and then reads the table data as parquet directly from s3.
@@ -780,15 +780,15 @@
     ----
     The resulting DataFrame (or every DataFrame in the returned Iterator for chunked queries) have a
     `query_metadata` attribute, which brings the query result metadata returned by
     `Boto3/Athena <https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services
     /athena.html#Athena.Client.get_query_execution>`_ .
 
     For a practical example check out the
-    `related tutorial <https://aws-sdk-pandas.readthedocs.io/en/3.1.0/
+    `related tutorial <https://aws-sdk-pandas.readthedocs.io/en/3.1.1/
     tutorials/024%20-%20Athena%20Query%20Metadata.html>`_!
 
 
     Note
     ----
     Valid encryption modes: [None, 'SSE_S3', 'SSE_KMS'].
 
@@ -1025,19 +1025,19 @@
     s3_additional_kwargs: Optional[Dict[str, Any]] = None,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     """Extract the full table AWS Athena and return the results as a Pandas DataFrame.
 
     **Related tutorial:**
 
-    - `Amazon Athena <https://aws-sdk-pandas.readthedocs.io/en/3.1.0/
+    - `Amazon Athena <https://aws-sdk-pandas.readthedocs.io/en/3.1.1/
       tutorials/006%20-%20Amazon%20Athena.html>`_
-    - `Athena Cache <https://aws-sdk-pandas.readthedocs.io/en/3.1.0/
+    - `Athena Cache <https://aws-sdk-pandas.readthedocs.io/en/3.1.1/
       tutorials/019%20-%20Athena%20Cache.html>`_
-    - `Global Configurations <https://aws-sdk-pandas.readthedocs.io/en/3.1.0/
+    - `Global Configurations <https://aws-sdk-pandas.readthedocs.io/en/3.1.1/
       tutorials/021%20-%20Global%20Configurations.html>`_
 
     **There are three approaches available through ctas_approach and unload_approach parameters:**
 
     **1** - ctas_approach=True (Default):
 
     Wrap the query with a CTAS and then reads the table data as parquet directly from s3.
@@ -1093,15 +1093,15 @@
     ----
     The resulting DataFrame (or every DataFrame in the returned Iterator for chunked queries) have a
     `query_metadata` attribute, which brings the query result metadata returned by
     `Boto3/Athena <https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services
     /athena.html#Athena.Client.get_query_execution>`_ .
 
     For a practical example check out the
-    `related tutorial <https://aws-sdk-pandas.readthedocs.io/en/3.1.0/
+    `related tutorial <https://aws-sdk-pandas.readthedocs.io/en/3.1.1/
     tutorials/024%20-%20Athena%20Query%20Metadata.html>`_!
 
 
     Note
     ----
     Valid encryption modes: [None, 'SSE_S3', 'SSE_KMS'].
```

### Comparing `awswrangler-3.1.0/awswrangler/athena/_read.pyi` & `awswrangler-3.1.1/awswrangler/athena/_read.pyi`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/athena/_utils.py` & `awswrangler-3.1.1/awswrangler/athena/_utils.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/athena/_write_iceberg.py` & `awswrangler-3.1.1/awswrangler/athena/_write_iceberg.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/catalog/__init__.py` & `awswrangler-3.1.1/awswrangler/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/catalog/_add.py` & `awswrangler-3.1.1/awswrangler/catalog/_add.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/catalog/_create.py` & `awswrangler-3.1.1/awswrangler/catalog/_create.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/catalog/_definitions.py` & `awswrangler-3.1.1/awswrangler/catalog/_definitions.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/catalog/_delete.py` & `awswrangler-3.1.1/awswrangler/catalog/_delete.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/catalog/_get.py` & `awswrangler-3.1.1/awswrangler/catalog/_get.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/catalog/_utils.py` & `awswrangler-3.1.1/awswrangler/catalog/_utils.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/chime.py` & `awswrangler-3.1.1/awswrangler/chime.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/cloudwatch.py` & `awswrangler-3.1.1/awswrangler/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/data_api/_connector.py` & `awswrangler-3.1.1/awswrangler/data_api/_connector.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/data_api/rds.py` & `awswrangler-3.1.1/awswrangler/data_api/rds.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/data_api/redshift.py` & `awswrangler-3.1.1/awswrangler/data_api/redshift.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/data_quality/_create.py` & `awswrangler-3.1.1/awswrangler/data_quality/_create.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/data_quality/_get.py` & `awswrangler-3.1.1/awswrangler/data_quality/_get.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/data_quality/_utils.py` & `awswrangler-3.1.1/awswrangler/data_quality/_utils.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/distributed/ray/_core.py` & `awswrangler-3.1.1/awswrangler/distributed/ray/_core.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/distributed/ray/_core.pyi` & `awswrangler-3.1.1/awswrangler/distributed/ray/_core.pyi`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/distributed/ray/_executor.py` & `awswrangler-3.1.1/awswrangler/distributed/ray/_executor.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/distributed/ray/_register.py` & `awswrangler-3.1.1/awswrangler/distributed/ray/_register.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/distributed/ray/_utils.py` & `awswrangler-3.1.1/awswrangler/distributed/ray/_utils.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/distributed/ray/datasources/__init__.py` & `awswrangler-3.1.1/awswrangler/distributed/ray/datasources/__init__.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/distributed/ray/datasources/arrow_csv_datasource.py` & `awswrangler-3.1.1/awswrangler/distributed/ray/datasources/arrow_csv_datasource.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/distributed/ray/datasources/arrow_json_datasource.py` & `awswrangler-3.1.1/awswrangler/distributed/ray/datasources/arrow_json_datasource.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/distributed/ray/datasources/arrow_parquet_base_datasource.py` & `awswrangler-3.1.1/awswrangler/distributed/ray/datasources/arrow_parquet_base_datasource.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/distributed/ray/datasources/arrow_parquet_datasource.py` & `awswrangler-3.1.1/awswrangler/distributed/ray/datasources/arrow_parquet_datasource.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/distributed/ray/datasources/pandas_file_based_datasource.py` & `awswrangler-3.1.1/awswrangler/distributed/ray/datasources/pandas_file_based_datasource.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/distributed/ray/datasources/pandas_text_datasource.py` & `awswrangler-3.1.1/awswrangler/distributed/ray/datasources/pandas_text_datasource.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/distributed/ray/modin/_core.py` & `awswrangler-3.1.1/awswrangler/distributed/ray/modin/_core.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/distributed/ray/modin/_data_types.py` & `awswrangler-3.1.1/awswrangler/distributed/ray/modin/_data_types.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/distributed/ray/modin/_utils.py` & `awswrangler-3.1.1/awswrangler/distributed/ray/modin/_utils.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/distributed/ray/modin/s3/_read_parquet.py` & `awswrangler-3.1.1/awswrangler/distributed/ray/modin/s3/_read_parquet.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/distributed/ray/modin/s3/_read_text.py` & `awswrangler-3.1.1/awswrangler/distributed/ray/modin/s3/_read_text.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/distributed/ray/modin/s3/_write_dataset.py` & `awswrangler-3.1.1/awswrangler/distributed/ray/modin/s3/_write_dataset.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/distributed/ray/modin/s3/_write_parquet.py` & `awswrangler-3.1.1/awswrangler/distributed/ray/modin/s3/_write_parquet.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/distributed/ray/modin/s3/_write_text.py` & `awswrangler-3.1.1/awswrangler/distributed/ray/modin/s3/_write_text.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/distributed/ray/s3/_list.py` & `awswrangler-3.1.1/awswrangler/distributed/ray/s3/_list.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/distributed/ray/s3/_read_parquet.py` & `awswrangler-3.1.1/awswrangler/distributed/ray/s3/_read_parquet.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/dynamodb/_delete.py` & `awswrangler-3.1.1/awswrangler/dynamodb/_delete.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/dynamodb/_read.py` & `awswrangler-3.1.1/awswrangler/dynamodb/_read.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/dynamodb/_read.pyi` & `awswrangler-3.1.1/awswrangler/dynamodb/_read.pyi`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/dynamodb/_utils.py` & `awswrangler-3.1.1/awswrangler/dynamodb/_utils.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/dynamodb/_write.py` & `awswrangler-3.1.1/awswrangler/dynamodb/_write.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/emr.py` & `awswrangler-3.1.1/awswrangler/emr.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/exceptions.py` & `awswrangler-3.1.1/awswrangler/exceptions.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/lakeformation/__init__.py` & `awswrangler-3.1.1/awswrangler/lakeformation/__init__.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/lakeformation/_read.py` & `awswrangler-3.1.1/awswrangler/lakeformation/_read.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/lakeformation/_utils.py` & `awswrangler-3.1.1/awswrangler/lakeformation/_utils.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/mysql.py` & `awswrangler-3.1.1/awswrangler/mysql.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/neptune/__init__.py` & `awswrangler-3.1.1/awswrangler/neptune/__init__.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/neptune/_client.py` & `awswrangler-3.1.1/awswrangler/neptune/_client.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/neptune/_gremlin_init.py` & `awswrangler-3.1.1/awswrangler/neptune/_gremlin_init.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/neptune/_gremlin_parser.py` & `awswrangler-3.1.1/awswrangler/neptune/_gremlin_parser.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/neptune/_neptune.py` & `awswrangler-3.1.1/awswrangler/neptune/_neptune.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/neptune/_utils.py` & `awswrangler-3.1.1/awswrangler/neptune/_utils.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/opensearch/_read.py` & `awswrangler-3.1.1/awswrangler/opensearch/_read.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/opensearch/_utils.py` & `awswrangler-3.1.1/awswrangler/opensearch/_utils.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/opensearch/_write.py` & `awswrangler-3.1.1/awswrangler/opensearch/_write.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/oracle.py` & `awswrangler-3.1.1/awswrangler/oracle.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/pandas/__init__.py` & `awswrangler-3.1.1/awswrangler/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/postgresql.py` & `awswrangler-3.1.1/awswrangler/postgresql.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/quicksight/__init__.py` & `awswrangler-3.1.1/awswrangler/quicksight/__init__.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/quicksight/_cancel.py` & `awswrangler-3.1.1/awswrangler/quicksight/_cancel.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/quicksight/_create.py` & `awswrangler-3.1.1/awswrangler/quicksight/_create.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/quicksight/_delete.py` & `awswrangler-3.1.1/awswrangler/quicksight/_delete.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/quicksight/_describe.py` & `awswrangler-3.1.1/awswrangler/quicksight/_describe.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/quicksight/_get_list.py` & `awswrangler-3.1.1/awswrangler/quicksight/_get_list.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/quicksight/_utils.py` & `awswrangler-3.1.1/awswrangler/quicksight/_utils.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/redshift/_connect.py` & `awswrangler-3.1.1/awswrangler/redshift/_connect.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/redshift/_read.py` & `awswrangler-3.1.1/awswrangler/redshift/_read.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/redshift/_read.pyi` & `awswrangler-3.1.1/awswrangler/redshift/_read.pyi`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/redshift/_utils.py` & `awswrangler-3.1.1/awswrangler/redshift/_utils.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/redshift/_write.py` & `awswrangler-3.1.1/awswrangler/redshift/_write.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/s3/__init__.py` & `awswrangler-3.1.1/awswrangler/s3/__init__.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/s3/_copy.py` & `awswrangler-3.1.1/awswrangler/s3/_copy.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/s3/_delete.py` & `awswrangler-3.1.1/awswrangler/s3/_delete.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/s3/_describe.py` & `awswrangler-3.1.1/awswrangler/s3/_describe.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/s3/_download.py` & `awswrangler-3.1.1/awswrangler/s3/_download.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/s3/_fs.py` & `awswrangler-3.1.1/awswrangler/s3/_fs.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/s3/_list.py` & `awswrangler-3.1.1/awswrangler/s3/_list.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/s3/_list.pyi` & `awswrangler-3.1.1/awswrangler/s3/_list.pyi`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/s3/_read.py` & `awswrangler-3.1.1/awswrangler/s3/_read.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/s3/_read_deltalake.py` & `awswrangler-3.1.1/awswrangler/s3/_read_deltalake.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/s3/_read_excel.py` & `awswrangler-3.1.1/awswrangler/s3/_read_excel.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/s3/_read_parquet.py` & `awswrangler-3.1.1/awswrangler/s3/_read_parquet.py`

 * *Files 0% similar despite different names*

```diff
@@ -425,15 +425,15 @@
     partition_filter : Callable[[Dict[str, str]], bool], optional
         Callback Function filters to apply on PARTITION columns (PUSH-DOWN filter).
         This function must receive a single argument (Dict[str, str]) where keys are partitions
         names and values are partitions values. Partitions values must be strings and the function
         must return a bool, True to read the partition or False to ignore it.
         Ignored if `dataset=False`.
         E.g ``lambda x: True if x["year"] == "2020" and x["month"] == "1" else False``
-        https://aws-data-wrangler.readthedocs.io/en/3.1.0/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
+        https://aws-data-wrangler.readthedocs.io/en/3.1.1/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
     columns : List[str], optional
         List of columns to read from the file(s).
     validate_schema : bool, default False
         Check that the schema is consistent across individual files.
     coerce_int96_timestamp_unit : str, optional
         Cast timestamps that are stored in INT96 format to a particular resolution (e.g. "ms").
         Setting to None is equivalent to "ns" and therefore INT96 timestamps are inferred as in nanoseconds.
@@ -650,15 +650,15 @@
     partition_filter: Optional[Callable[[Dict[str, str]], bool]]
         Callback Function filters to apply on PARTITION columns (PUSH-DOWN filter).
         This function must receive a single argument (Dict[str, str]) where keys are partitions
         names and values are partitions values. Partitions values must be strings and the function
         must return a bool, True to read the partition or False to ignore it.
         Ignored if `dataset=False`.
         E.g ``lambda x: True if x["year"] == "2020" and x["month"] == "1" else False``
-        https://aws-sdk-pandas.readthedocs.io/en/3.1.0/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.1.1/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
     columns : List[str], optional
         List of columns to read from the file(s).
     validate_schema : bool, default False
         Check that the schema is consistent across individual files.
     coerce_int96_timestamp_unit : str, optional
         Cast timestamps that are stored in INT96 format to a particular resolution (e.g. "ms").
         Setting to None is equivalent to "ns" and therefore INT96 timestamps are inferred as in nanoseconds.
```

### Comparing `awswrangler-3.1.0/awswrangler/s3/_read_parquet.pyi` & `awswrangler-3.1.1/awswrangler/s3/_read_parquet.pyi`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/s3/_read_text.py` & `awswrangler-3.1.1/awswrangler/s3/_read_text.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,15 +221,15 @@
     partition_filter : Optional[Callable[[Dict[str, str]], bool]]
         Callback Function filters to apply on PARTITION columns (PUSH-DOWN filter).
         This function MUST receive a single argument (Dict[str, str]) where keys are partitions
         names and values are partitions values. Partitions values will be always strings extracted from S3.
         This function MUST return a bool, True to read the partition or False to ignore it.
         Ignored if `dataset=False`.
         E.g ``lambda x: True if x["year"] == "2020" and x["month"] == "1" else False``
-        https://aws-sdk-pandas.readthedocs.io/en/3.1.0/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.1.1/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
     ray_args: typing.RaySettings, optional
         Parameters of the Ray Modin settings. Only used when distributed computing is used with Ray and Modin installed.
     pandas_kwargs :
         KEYWORD arguments forwarded to pandas.read_csv(). You can NOT pass `pandas_kwargs` explicitly, just add valid
         Pandas arguments in the function call and awswrangler will accept it.
         e.g. wr.s3.read_csv('s3://bucket/prefix/', sep='|', na_values=['null', 'none'], skip_blank_lines=True)
         https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.read_csv.html
@@ -377,15 +377,15 @@
     partition_filter: Optional[Callable[[Dict[str, str]], bool]]
         Callback Function filters to apply on PARTITION columns (PUSH-DOWN filter).
         This function MUST receive a single argument (Dict[str, str]) where keys are partitions
         names and values are partitions values. Partitions values will be always strings extracted from S3.
         This function MUST return a bool, True to read the partition or False to ignore it.
         Ignored if `dataset=False`.
         E.g ``lambda x: True if x["year"] == "2020" and x["month"] == "1" else False``
-        https://aws-sdk-pandas.readthedocs.io/en/3.1.0/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.1.1/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
     ray_args: typing.RaySettings, optional
         Parameters of the Ray Modin settings. Only used when distributed computing is used with Ray and Modin installed.
     pandas_kwargs:
         KEYWORD arguments forwarded to pandas.read_fwf(). You can NOT pass `pandas_kwargs` explicit, just add valid
         Pandas arguments in the function call and awswrangler will accept it.
         e.g. wr.s3.read_fwf(path='s3://bucket/prefix/', widths=[1, 3], names=["c0", "c1"])
         https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.read_fwf.html
@@ -537,15 +537,15 @@
     partition_filter: Optional[Callable[[Dict[str, str]], bool]]
         Callback Function filters to apply on PARTITION columns (PUSH-DOWN filter).
         This function MUST receive a single argument (Dict[str, str]) where keys are partitions
         names and values are partitions values. Partitions values will be always strings extracted from S3.
         This function MUST return a bool, True to read the partition or False to ignore it.
         Ignored if `dataset=False`.
         E.g ``lambda x: True if x["year"] == "2020" and x["month"] == "1" else False``
-        https://aws-sdk-pandas.readthedocs.io/en/3.1.0/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.1.1/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
     ray_args: typing.RaySettings, optional
         Parameters of the Ray Modin settings. Only used when distributed computing is used with Ray and Modin installed.
     pandas_kwargs:
         KEYWORD arguments forwarded to pandas.read_json(). You can NOT pass `pandas_kwargs` explicit, just add valid
         Pandas arguments in the function call and awswrangler will accept it.
         e.g. wr.s3.read_json('s3://bucket/prefix/', lines=True, keep_default_dates=True)
         https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.read_json.html
```

### Comparing `awswrangler-3.1.0/awswrangler/s3/_read_text.pyi` & `awswrangler-3.1.1/awswrangler/s3/_read_text.pyi`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/s3/_read_text_core.py` & `awswrangler-3.1.1/awswrangler/s3/_read_text_core.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/s3/_select.py` & `awswrangler-3.1.1/awswrangler/s3/_select.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/s3/_upload.py` & `awswrangler-3.1.1/awswrangler/s3/_upload.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/s3/_wait.py` & `awswrangler-3.1.1/awswrangler/s3/_wait.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/s3/_write.py` & `awswrangler-3.1.1/awswrangler/s3/_write.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/s3/_write_concurrent.py` & `awswrangler-3.1.1/awswrangler/s3/_write_concurrent.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/s3/_write_dataset.py` & `awswrangler-3.1.1/awswrangler/s3/_write_dataset.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/s3/_write_deltalake.py` & `awswrangler-3.1.1/awswrangler/s3/_write_deltalake.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/s3/_write_excel.py` & `awswrangler-3.1.1/awswrangler/s3/_write_excel.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/s3/_write_parquet.py` & `awswrangler-3.1.1/awswrangler/s3/_write_parquet.py`

 * *Files 0% similar despite different names*

```diff
@@ -318,26 +318,26 @@
     bucketing_info: Tuple[List[str], int], optional
         Tuple consisting of the column names used for bucketing as the first element and the number of buckets as the
         second element.
         Only `str`, `int` and `bool` are supported as column data types for bucketing.
     concurrent_partitioning: bool
         If True will increase the parallelism level during the partitions writing. It will decrease the
         writing time and increase the memory usage.
-        https://aws-sdk-pandas.readthedocs.io/en/3.1.0/tutorials/022%20-%20Writing%20Partitions%20Concurrently.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.1.1/tutorials/022%20-%20Writing%20Partitions%20Concurrently.html
     mode: str, optional
         ``append`` (Default), ``overwrite``, ``overwrite_partitions``. Only takes effect if dataset=True.
         For details check the related tutorial:
-        https://aws-sdk-pandas.readthedocs.io/en/3.1.0/tutorials/004%20-%20Parquet%20Datasets.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.1.1/tutorials/004%20-%20Parquet%20Datasets.html
     catalog_versioning : bool
         If True and `mode="overwrite"`, creates an archived version of the table catalog before updating it.
     schema_evolution : bool
         If True allows schema evolution (new or missing columns), otherwise a exception will be raised. True by default.
         (Only considered if dataset=True and mode in ("append", "overwrite_partitions"))
         Related tutorial:
-        https://aws-sdk-pandas.readthedocs.io/en/3.1.0/tutorials/014%20-%20Schema%20Evolution.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.1.1/tutorials/014%20-%20Schema%20Evolution.html
     database : str, optional
         Glue/Athena catalog: Database name.
     table : str, optional
         Glue/Athena catalog: Table name.
     glue_table_settings: dict (GlueTableSettings), optional
         Settings for writing to the Glue table.
     dtype : Dict[str, str], optional
```

### Comparing `awswrangler-3.1.0/awswrangler/s3/_write_text.py` & `awswrangler-3.1.1/awswrangler/s3/_write_text.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,26 +165,26 @@
     bucketing_info: Tuple[List[str], int], optional
         Tuple consisting of the column names used for bucketing as the first element and the number of buckets as the
         second element.
         Only `str`, `int` and `bool` are supported as column data types for bucketing.
     concurrent_partitioning: bool
         If True will increase the parallelism level during the partitions writing. It will decrease the
         writing time and increase the memory usage.
-        https://aws-sdk-pandas.readthedocs.io/en/3.1.0/tutorials/022%20-%20Writing%20Partitions%20Concurrently.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.1.1/tutorials/022%20-%20Writing%20Partitions%20Concurrently.html
     mode : str, optional
         ``append`` (Default), ``overwrite``, ``overwrite_partitions``. Only takes effect if dataset=True.
         For details check the related tutorial:
-        https://aws-sdk-pandas.readthedocs.io/en/3.1.0/stubs/awswrangler.s3.to_parquet.html#awswrangler.s3.to_parquet
+        https://aws-sdk-pandas.readthedocs.io/en/3.1.1/stubs/awswrangler.s3.to_parquet.html#awswrangler.s3.to_parquet
     catalog_versioning : bool
         If True and `mode="overwrite"`, creates an archived version of the table catalog before updating it.
     schema_evolution : bool
         If True allows schema evolution (new or missing columns), otherwise a exception will be raised.
         (Only considered if dataset=True and mode in ("append", "overwrite_partitions")). False by default.
         Related tutorial:
-        https://aws-sdk-pandas.readthedocs.io/en/3.1.0/tutorials/014%20-%20Schema%20Evolution.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.1.1/tutorials/014%20-%20Schema%20Evolution.html
     database : str, optional
         Glue/Athena catalog: Database name.
     table : str, optional
         Glue/Athena catalog: Table name.
     glue_table_settings: dict (GlueTableSettings), optional
         Settings for writing to the Glue table.
     dtype : Dict[str, str], optional
@@ -769,26 +769,26 @@
     bucketing_info: Tuple[List[str], int], optional
         Tuple consisting of the column names used for bucketing as the first element and the number of buckets as the
         second element.
         Only `str`, `int` and `bool` are supported as column data types for bucketing.
     concurrent_partitioning: bool
         If True will increase the parallelism level during the partitions writing. It will decrease the
         writing time and increase the memory usage.
-        https://aws-sdk-pandas.readthedocs.io/en/3.1.0/tutorials/022%20-%20Writing%20Partitions%20Concurrently.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.1.1/tutorials/022%20-%20Writing%20Partitions%20Concurrently.html
     mode : str, optional
         ``append`` (Default), ``overwrite``, ``overwrite_partitions``. Only takes effect if dataset=True.
         For details check the related tutorial:
-        https://aws-sdk-pandas.readthedocs.io/en/3.1.0/stubs/awswrangler.s3.to_parquet.html#awswrangler.s3.to_parquet
+        https://aws-sdk-pandas.readthedocs.io/en/3.1.1/stubs/awswrangler.s3.to_parquet.html#awswrangler.s3.to_parquet
     catalog_versioning : bool
         If True and `mode="overwrite"`, creates an archived version of the table catalog before updating it.
     schema_evolution : bool
         If True allows schema evolution (new or missing columns), otherwise a exception will be raised.
         (Only considered if dataset=True and mode in ("append", "overwrite_partitions"))
         Related tutorial:
-        https://aws-sdk-pandas.readthedocs.io/en/3.1.0/tutorials/014%20-%20Schema%20Evolution.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.1.1/tutorials/014%20-%20Schema%20Evolution.html
     database : str, optional
         Glue/Athena catalog: Database name.
     table : str, optional
         Glue/Athena catalog: Table name.
     glue_table_settings: dict (GlueTableSettings), optional
         Settings for writing to the Glue table.
     dtype : Dict[str, str], optional
```

### Comparing `awswrangler-3.1.0/awswrangler/secretsmanager.py` & `awswrangler-3.1.1/awswrangler/secretsmanager.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/sqlserver.py` & `awswrangler-3.1.1/awswrangler/sqlserver.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/sts.py` & `awswrangler-3.1.1/awswrangler/sts.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/timestream/__init__.py` & `awswrangler-3.1.1/awswrangler/timestream/__init__.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/timestream/_create.py` & `awswrangler-3.1.1/awswrangler/timestream/_create.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/timestream/_delete.py` & `awswrangler-3.1.1/awswrangler/timestream/_delete.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/timestream/_list.py` & `awswrangler-3.1.1/awswrangler/timestream/_list.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/timestream/_read.py` & `awswrangler-3.1.1/awswrangler/timestream/_read.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/timestream/_read.pyi` & `awswrangler-3.1.1/awswrangler/timestream/_read.pyi`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/timestream/_write.py` & `awswrangler-3.1.1/awswrangler/timestream/_write.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/awswrangler/typing.py` & `awswrangler-3.1.1/awswrangler/typing.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.0/pyproject.toml` & `awswrangler-3.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "awswrangler"
-version = "3.1.0"
+version = "3.1.1"
 description = "Pandas on AWS."
 authors = ["Amazon Web Services"]
 license = "Apache License 2.0"
 
 readme = "README.md"
 
 include = ["README.md", "LICENSE.txt", "NOTICE.txt", "THIRD_PARTY.txt", "awswrangler/py.typed"]
@@ -30,14 +30,15 @@
 # Required
 boto3 = "^1.20.32"
 botocore = "^1.23.32"
 pandas = ">=1.2.0,!=1.5.0,<3.0.0" # Exclusion per: https://github.com/aws/aws-sdk-pandas/issues/1678
 numpy = "^1.18"
 pyarrow = ">=7.0.0"
 typing-extensions = "^4.4.0"
+packaging = "^23.1"
 
 # Databases
 redshift-connector = { version = "^2.0.0", optional = true }
 pymysql = { version = "^1.0.0", optional = true }
 pg8000 = { version = "^1.29.0", optional = true }
 pyodbc = { version = "^4.0.0", optional = true }
 oracledb = { version = "^1.0.0", optional = true }
```

### Comparing `awswrangler-3.1.0/PKG-INFO` & `awswrangler-3.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awswrangler
-Version: 3.1.0
+Version: 3.1.1
 Summary: Pandas on AWS.
 Home-page: https://aws-sdk-pandas.readthedocs.io/
 License: Apache-2.0
 Keywords: pandas,aws
 Author: Amazon Web Services
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -38,14 +38,15 @@
 Requires-Dist: gremlinpython (>=3.6.2,<4.0.0) ; extra == "gremlin"
 Requires-Dist: jsonpath-ng (>=1.5.3,<2.0.0) ; extra == "opensearch"
 Requires-Dist: modin (>=0.20.1,<0.21.0) ; extra == "modin"
 Requires-Dist: numpy (>=1.18,<2.0)
 Requires-Dist: openpyxl (>=3.0.0,<4.0.0) ; extra == "openpyxl"
 Requires-Dist: opensearch-py (>=2.0.0,<3.0.0) ; extra == "opensearch"
 Requires-Dist: oracledb (>=1.0.0,<2.0.0) ; extra == "oracle"
+Requires-Dist: packaging (>=23.1,<24.0)
 Requires-Dist: pandas (>=1.2.0,!=1.5.0,<3.0.0)
 Requires-Dist: pg8000 (>=1.29.0,<2.0.0) ; extra == "postgres"
 Requires-Dist: progressbar2 (>=4.0.0,<5.0.0) ; extra == "progressbar"
 Requires-Dist: pyarrow (>=7.0.0)
 Requires-Dist: pymysql (>=1.0.0,<2.0.0) ; extra == "mysql"
 Requires-Dist: pyodbc (>=4.0.0,<5.0.0) ; extra == "sqlserver"
 Requires-Dist: ray[data,default] (>=2.0.0,<2.5.0) ; extra == "ray"
@@ -66,15 +67,15 @@
 Easy integration with Athena, Glue, Redshift, Timestream, OpenSearch, Neptune, QuickSight, Chime, CloudWatchLogs, DynamoDB, EMR, SecretManager, PostgreSQL, MySQL, SQLServer and S3 (Parquet, CSV, JSON and EXCEL).
 
 ![AWS SDK for pandas](docs/source/_static/logo2.png?raw=true "AWS SDK for pandas")
 ![tracker](https://d3tiqpr4kkkomd.cloudfront.net/img/pixel.png?asset=GVOYN2BOOQ573LTVIHEW)
 
 > An [AWS Professional Service](https://aws.amazon.com/professional-services/) open source initiative | aws-proserve-opensource@amazon.com
 
-[![Release](https://img.shields.io/badge/3.1.0-brightgreen.svg)](https://pypi.org/project/awswrangler/)
+[![Release](https://img.shields.io/badge/3.1.1-brightgreen.svg)](https://pypi.org/project/awswrangler/)
 [![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.8%20%7C%203.9%20%7C%203.10-brightgreen.svg)](https://anaconda.org/conda-forge/awswrangler)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 ![Static Checking](https://github.com/aws/aws-sdk-pandas/workflows/Static%20Checking/badge.svg?branch=main)
 [![Documentation Status](https://readthedocs.org/projects/aws-sdk-pandas/badge/?version=latest)](https://aws-sdk-pandas.readthedocs.io/?badge=latest)
@@ -154,33 +155,33 @@
 """)
 
 ```
 
 ## At scale
 AWS SDK for pandas can also run your workflows at scale by leveraging [Modin](https://modin.readthedocs.io/en/stable/) and [Ray](https://www.ray.io/). Both projects aim to speed up data workloads by distributing processing over a cluster of workers.
 
-The quickest way to get started is to use AWS Glue with Ray. Read our [docs](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/scale.html), our [blog](https://aws.amazon.com/blogs/big-data/scale-aws-sdk-for-pandas-workloads-with-aws-glue-for-ray/), or head to our latest [tutorials](https://github.com/aws/aws-sdk-pandas/tree/main/tutorials) to discover even more features.
+The quickest way to get started is to use AWS Glue with Ray. Read our [docs](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/scale.html), our [blog](https://aws.amazon.com/blogs/big-data/scale-aws-sdk-for-pandas-workloads-with-aws-glue-for-ray/), or head to our latest [tutorials](https://github.com/aws/aws-sdk-pandas/tree/main/tutorials) to discover even more features.
 
 ## [Read The Docs](https://aws-sdk-pandas.readthedocs.io/)
 
-- [**What is AWS SDK for pandas?**](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/about.html)
-- [**Install**](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/install.html)
-  - [PyPi (pip)](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/install.html#pypi-pip)
-  - [Conda](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/install.html#conda)
-  - [AWS Lambda Layer](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/install.html#aws-lambda-layer)
-  - [AWS Glue Python Shell Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/install.html#aws-glue-python-shell-jobs)
-  - [AWS Glue PySpark Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/install.html#aws-glue-pyspark-jobs)
-  - [Amazon SageMaker Notebook](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/install.html#amazon-sagemaker-notebook)
-  - [Amazon SageMaker Notebook Lifecycle](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/install.html#amazon-sagemaker-notebook-lifecycle)
-  - [EMR](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/install.html#emr)
-  - [From source](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/install.html#from-source)
-- [**At scale**](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/scale.html)
-  - [Getting Started](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/scale.html#getting-started)
-  - [Supported APIs](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/scale.html#supported-apis)
-  - [Resources](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/scale.html#resources)
+- [**What is AWS SDK for pandas?**](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/about.html)
+- [**Install**](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/install.html)
+  - [PyPi (pip)](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/install.html#pypi-pip)
+  - [Conda](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/install.html#conda)
+  - [AWS Lambda Layer](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/install.html#aws-lambda-layer)
+  - [AWS Glue Python Shell Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/install.html#aws-glue-python-shell-jobs)
+  - [AWS Glue PySpark Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/install.html#aws-glue-pyspark-jobs)
+  - [Amazon SageMaker Notebook](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/install.html#amazon-sagemaker-notebook)
+  - [Amazon SageMaker Notebook Lifecycle](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/install.html#amazon-sagemaker-notebook-lifecycle)
+  - [EMR](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/install.html#emr)
+  - [From source](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/install.html#from-source)
+- [**At scale**](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/scale.html)
+  - [Getting Started](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/scale.html#getting-started)
+  - [Supported APIs](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/scale.html#supported-apis)
+  - [Resources](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/scale.html#resources)
 - [**Tutorials**](https://github.com/aws/aws-sdk-pandas/tree/main/tutorials)
   - [001 - Introduction](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/001%20-%20Introduction.ipynb)
   - [002 - Sessions](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/002%20-%20Sessions.ipynb)
   - [003 - Amazon S3](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/003%20-%20Amazon%20S3.ipynb)
   - [004 - Parquet Datasets](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/004%20-%20Parquet%20Datasets.ipynb)
   - [005 - Glue Catalog](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/005%20-%20Glue%20Catalog.ipynb)
   - [006 - Amazon Athena](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/006%20-%20Amazon%20Athena.ipynb)
@@ -213,39 +214,39 @@
   - [033 - Amazon Neptune](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/033%20-%20Amazon%20Neptune.ipynb)
   - [034 - Distributing Calls Using Ray](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/034%20-%20Distributing%20Calls%20using%20Ray.ipynb)
   - [035 - Distributing Calls on Ray Remote Cluster](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/035%20-%20Distributing%20Calls%20on%20Ray%20Remote%20Cluster.ipynb)
   - [036 - Distributing Calls with Glue Interactive Sessions on Ray](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/036%20-%20Distributing%20Calls%20with%20Glue%20Interactive%20Sessions%20on%20Ray.ipynb)
   - [037 - Glue Data Quality](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/037%20-%20Glue%20Data%20Quality.ipynb)
   - [038 - OpenSearch Serverless](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/038%20-%20OpenSearch%20Serverless.ipynb)
   - [039 - Athena Iceberg](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/039%20-%20Athena%20Iceberg.ipynb)
-- [**API Reference**](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html)
-  - [Amazon S3](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#amazon-s3)
-  - [AWS Glue Catalog](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#aws-glue-catalog)
-  - [Amazon Athena](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#amazon-athena)
-  - [AWS Lake Formation](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#aws-lake-formation)
-  - [Amazon Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#amazon-redshift)
-  - [PostgreSQL](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#postgresql)
-  - [MySQL](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#mysql)
-  - [SQL Server](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#sqlserver)
-  - [Oracle](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#oracle)
-  - [Data API Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#data-api-redshift)
-  - [Data API RDS](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#data-api-rds)
-  - [OpenSearch](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#opensearch)
-  - [AWS Glue Data Quality](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#aws-glue-data-quality)
-  - [Amazon Neptune](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#amazon-neptune)
-  - [DynamoDB](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#dynamodb)
-  - [Amazon Timestream](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#amazon-timestream)
-  - [Amazon EMR](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#amazon-emr)
-  - [Amazon CloudWatch Logs](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#amazon-cloudwatch-logs)
-  - [Amazon Chime](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#amazon-chime)
-  - [Amazon QuickSight](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#amazon-quicksight)
-  - [AWS STS](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#aws-sts)
-  - [AWS Secrets Manager](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#aws-secrets-manager)
-  - [Global Configurations](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#global-configurations)
-  - [Distributed - Ray](https://aws-sdk-pandas.readthedocs.io/en/3.1.0/api.html#distributed-ray)
+- [**API Reference**](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html)
+  - [Amazon S3](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#amazon-s3)
+  - [AWS Glue Catalog](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#aws-glue-catalog)
+  - [Amazon Athena](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#amazon-athena)
+  - [AWS Lake Formation](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#aws-lake-formation)
+  - [Amazon Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#amazon-redshift)
+  - [PostgreSQL](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#postgresql)
+  - [MySQL](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#mysql)
+  - [SQL Server](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#sqlserver)
+  - [Oracle](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#oracle)
+  - [Data API Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#data-api-redshift)
+  - [Data API RDS](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#data-api-rds)
+  - [OpenSearch](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#opensearch)
+  - [AWS Glue Data Quality](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#aws-glue-data-quality)
+  - [Amazon Neptune](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#amazon-neptune)
+  - [DynamoDB](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#dynamodb)
+  - [Amazon Timestream](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#amazon-timestream)
+  - [Amazon EMR](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#amazon-emr)
+  - [Amazon CloudWatch Logs](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#amazon-cloudwatch-logs)
+  - [Amazon Chime](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#amazon-chime)
+  - [Amazon QuickSight](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#amazon-quicksight)
+  - [AWS STS](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#aws-sts)
+  - [AWS Secrets Manager](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#aws-secrets-manager)
+  - [Global Configurations](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#global-configurations)
+  - [Distributed - Ray](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#distributed-ray)
 - [**License**](https://github.com/aws/aws-sdk-pandas/blob/main/LICENSE.txt)
 - [**Contributing**](https://github.com/aws/aws-sdk-pandas/blob/main/CONTRIBUTING.md)
 
 ## Getting Help
 
 The best way to interact with our team is through GitHub. You can open an [issue](https://github.com/aws/aws-sdk-pandas/issues/new/choose) and choose from one of our templates for bug reports, feature requests...
 You may also find help on these community resources:
```

