# Comparing `tmp/apache-airflow-providers-amazon-8.0.0rc3.tar.gz` & `tmp/apache-airflow-providers-amazon-8.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-amazon-8.0.0rc3.tar", last modified: Wed Apr 26 09:36:03 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-amazon-8.1.0rc1.tar", last modified: Tue May 16 15:52:50 2023, max compression
```

## Comparing `apache-airflow-providers-amazon-8.0.0rc3.tar` & `apache-airflow-providers-amazon-8.1.0rc1.tar`

### file list

```diff
@@ -1,169 +1,173 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:36:03.000000 apache-airflow-providers-amazon-8.0.0rc3/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-amazon-8.0.0rc3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1219 2023-04-26 09:35:58.000000 apache-airflow-providers-amazon-8.0.0rc3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-amazon-8.0.0rc3/NOTICE
--rw-r--r--   0 root         (0) root         (0)    57184 2023-04-26 09:36:03.000000 apache-airflow-providers-amazon-8.0.0rc3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    55363 2023-04-26 09:35:58.000000 apache-airflow-providers-amazon-8.0.0rc3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:36:01.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:36:01.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:36:01.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:36:01.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1731 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:36:02.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4856 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/appflow.py
--rw-r--r--   0 root         (0) root         (0)    12240 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/athena.py
--rw-r--r--   0 root         (0) root         (0)    45461 2023-04-26 05:04:56.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/base_aws.py
--rw-r--r--   0 root         (0) root         (0)    20629 2023-04-13 08:25:21.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/batch_client.py
--rw-r--r--   0 root         (0) root         (0)     2511 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/batch_waiters.json
--rw-r--r--   0 root         (0) root         (0)     9697 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/batch_waiters.py
--rw-r--r--   0 root         (0) root         (0)     3376 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/cloud_formation.py
--rw-r--r--   0 root         (0) root         (0)    14133 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/datasync.py
--rw-r--r--   0 root         (0) root         (0)     7906 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/dms.py
--rw-r--r--   0 root         (0) root         (0)     2668 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/dynamodb.py
--rw-r--r--   0 root         (0) root         (0)     7641 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/ec2.py
--rw-r--r--   0 root         (0) root         (0)     3702 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/ecr.py
--rw-r--r--   0 root         (0) root         (0)     9194 2023-03-06 20:52:28.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/ecs.py
--rw-r--r--   0 root         (0) root         (0)    23957 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/eks.py
--rw-r--r--   0 root         (0) root         (0)    12114 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py
--rw-r--r--   0 root         (0) root         (0)    20348 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/emr.py
--rw-r--r--   0 root         (0) root         (0)     3518 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/glacier.py
--rw-r--r--   0 root         (0) root         (0)    13816 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/glue.py
--rw-r--r--   0 root         (0) root         (0)     7611 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/glue_catalog.py
--rw-r--r--   0 root         (0) root         (0)     8895 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/glue_crawler.py
--rw-r--r--   0 root         (0) root         (0)     1993 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/kinesis.py
--rw-r--r--   0 root         (0) root         (0)     8008 2023-02-24 18:53:47.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/lambda_function.py
--rw-r--r--   0 root         (0) root         (0)     4823 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/logs.py
--rw-r--r--   0 root         (0) root         (0)     7219 2023-04-07 12:28:57.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/quicksight.py
--rw-r--r--   0 root         (0) root         (0)    15272 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/rds.py
--rw-r--r--   0 root         (0) root         (0)    13108 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/redshift_cluster.py
--rw-r--r--   0 root         (0) root         (0)     7720 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/redshift_data.py
--rw-r--r--   0 root         (0) root         (0)     5020 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/redshift_sql.py
--rw-r--r--   0 root         (0) root         (0)    42450 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/s3.py
--rw-r--r--   0 root         (0) root         (0)    56676 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     2692 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/secrets_manager.py
--rw-r--r--   0 root         (0) root         (0)     4143 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/ses.py
--rw-r--r--   0 root         (0) root         (0)     3461 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/sns.py
--rw-r--r--   0 root         (0) root         (0)     3119 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/sqs.py
--rw-r--r--   0 root         (0) root         (0)     2449 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/ssm.py
--rw-r--r--   0 root         (0) root         (0)     3072 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/step_function.py
--rw-r--r--   0 root         (0) root         (0)     1817 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/sts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:36:02.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/links/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/links/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2940 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/links/base_aws.py
--rw-r--r--   0 root         (0) root         (0)     1767 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/links/batch.py
--rw-r--r--   0 root         (0) root         (0)     1416 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/links/emr.py
--rw-r--r--   0 root         (0) root         (0)     1228 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/links/glue.py
--rw-r--r--   0 root         (0) root         (0)     1607 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/links/logs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:36:02.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/log/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5072 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py
--rw-r--r--   0 root         (0) root         (0)     9635 2023-03-10 19:31:58.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/log/s3_task_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:36:02.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19677 2023-03-06 20:52:28.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/appflow.py
--rw-r--r--   0 root         (0) root         (0)     6141 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/athena.py
--rw-r--r--   0 root         (0) root         (0)    15828 2023-04-13 08:25:21.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/batch.py
--rw-r--r--   0 root         (0) root         (0)     3633 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/cloud_formation.py
--rw-r--r--   0 root         (0) root         (0)    18419 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/datasync.py
--rw-r--r--   0 root         (0) root         (0)    10715 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/dms.py
--rw-r--r--   0 root         (0) root         (0)     9589 2023-03-10 19:31:58.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/ec2.py
--rw-r--r--   0 root         (0) root         (0)    29018 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/ecs.py
--rw-r--r--   0 root         (0) root         (0)    31753 2023-04-14 11:39:41.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/eks.py
--rw-r--r--   0 root         (0) root         (0)    50180 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/emr.py
--rw-r--r--   0 root         (0) root         (0)     3705 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/glacier.py
--rw-r--r--   0 root         (0) root         (0)     7471 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/glue.py
--rw-r--r--   0 root         (0) root         (0)     3306 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/glue_crawler.py
--rw-r--r--   0 root         (0) root         (0)     7755 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/lambda_function.py
--rw-r--r--   0 root         (0) root         (0)     3972 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/quicksight.py
--rw-r--r--   0 root         (0) root         (0)    29868 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/rds.py
--rw-r--r--   0 root         (0) root         (0)    28991 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/redshift_cluster.py
--rw-r--r--   0 root         (0) root         (0)     5559 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/redshift_data.py
--rw-r--r--   0 root         (0) root         (0)    29966 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/s3.py
--rw-r--r--   0 root         (0) root         (0)    49835 2023-03-01 07:06:45.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     2959 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/sns.py
--rw-r--r--   0 root         (0) root         (0)     3563 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/sqs.py
--rw-r--r--   0 root         (0) root         (0)     4469 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/step_function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:36:02.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/secrets/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15533 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/secrets/secrets_manager.py
--rw-r--r--   0 root         (0) root         (0)     8503 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/secrets/systems_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:36:02.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3120 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/athena.py
--rw-r--r--   0 root         (0) root         (0)     7384 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/batch.py
--rw-r--r--   0 root         (0) root         (0)     4163 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/cloud_formation.py
--rw-r--r--   0 root         (0) root         (0)     3998 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/dms.py
--rw-r--r--   0 root         (0) root         (0)     3915 2023-04-19 10:00:26.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/dynamodb.py
--rw-r--r--   0 root         (0) root         (0)     2674 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/ec2.py
--rw-r--r--   0 root         (0) root         (0)     7203 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/ecs.py
--rw-r--r--   0 root         (0) root         (0)     9786 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/eks.py
--rw-r--r--   0 root         (0) root         (0)    18505 2023-04-21 10:05:41.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/emr.py
--rw-r--r--   0 root         (0) root         (0)     4129 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/glacier.py
--rw-r--r--   0 root         (0) root         (0)     3428 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/glue.py
--rw-r--r--   0 root         (0) root         (0)     3732 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py
--rw-r--r--   0 root         (0) root         (0)     2963 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/glue_crawler.py
--rw-r--r--   0 root         (0) root         (0)     3064 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/lambda_function.py
--rw-r--r--   0 root         (0) root         (0)     3641 2023-04-07 12:28:57.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/quicksight.py
--rw-r--r--   0 root         (0) root         (0)     6447 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/rds.py
--rw-r--r--   0 root         (0) root         (0)     2637 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/redshift_cluster.py
--rw-r--r--   0 root         (0) root         (0)    11650 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/s3.py
--rw-r--r--   0 root         (0) root         (0)    13057 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     9584 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/sqs.py
--rw-r--r--   0 root         (0) root         (0)     3400 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/step_function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:36:02.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2768 2023-03-15 08:58:48.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/base.py
--rw-r--r--   0 root         (0) root         (0)     5843 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     4410 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/exasol_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     6435 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/ftp_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     7676 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/gcs_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     4701 2023-04-21 10:05:41.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py
--rw-r--r--   0 root         (0) root         (0)     9042 2023-04-21 10:05:41.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/google_api_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     4172 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py
--rw-r--r--   0 root         (0) root         (0)     4248 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     4158 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/local_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     5863 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/mongo_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     8108 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/redshift_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     2966 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/s3_to_ftp.py
--rw-r--r--   0 root         (0) root         (0)     8268 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/s3_to_redshift.py
--rw-r--r--   0 root         (0) root         (0)     3191 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/s3_to_sftp.py
--rw-r--r--   0 root         (0) root         (0)     4620 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/s3_to_sql.py
--rw-r--r--   0 root         (0) root         (0)     5679 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     3679 2023-04-07 12:28:57.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/sftp_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     8475 2023-04-19 10:00:26.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/sql_to_s3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:36:02.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/triggers/
--rw-r--r--   0 root         (0) root         (0)      787 2023-03-14 06:24:40.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5579 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/triggers/redshift_cluster.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:36:03.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/utils/
--rw-r--r--   0 root         (0) root         (0)     2215 2023-03-06 20:52:28.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20348 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/utils/connection_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     2561 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/utils/eks_get_token.py
--rw-r--r--   0 root         (0) root         (0)     1853 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/utils/emailer.py
--rw-r--r--   0 root         (0) root         (0)      972 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/utils/rds.py
--rw-r--r--   0 root         (0) root         (0)     1913 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/utils/redshift.py
--rw-r--r--   0 root         (0) root         (0)     1040 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/utils/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     1701 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/utils/tags.py
--rw-r--r--   0 root         (0) root         (0)     3583 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/utils/waiter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:36:03.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/waiters/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/waiters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/waiters/appflow.json
--rw-r--r--   0 root         (0) root         (0)     1853 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/waiters/base_waiter.py
--rw-r--r--   0 root         (0) root         (0)     2720 2023-03-02 08:17:44.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/waiters/ecs.json
--rw-r--r--   0 root         (0) root         (0)      659 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/waiters/eks.json
--rw-r--r--   0 root         (0) root         (0)      430 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/waiters/emr-serverless.json
--rw-r--r--   0 root         (0) root         (0)     2559 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/waiters/emr.json
--rw-r--r--   0 root         (0) root         (0)    36833 2023-04-26 09:35:58.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:36:03.000000 apache-airflow-providers-amazon-8.0.0rc3/apache_airflow_providers_amazon.egg-info/
--rw-r--r--   0 root         (0) root         (0)    57184 2023-04-26 09:36:01.000000 apache-airflow-providers-amazon-8.0.0rc3/apache_airflow_providers_amazon.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7264 2023-04-26 09:36:01.000000 apache-airflow-providers-amazon-8.0.0rc3/apache_airflow_providers_amazon.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 09:36:01.000000 apache-airflow-providers-amazon-8.0.0rc3/apache_airflow_providers_amazon.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-04-26 09:36:01.000000 apache-airflow-providers-amazon-8.0.0rc3/apache_airflow_providers_amazon.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 09:36:01.000000 apache-airflow-providers-amazon-8.0.0rc3/apache_airflow_providers_amazon.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      784 2023-04-26 09:36:01.000000 apache-airflow-providers-amazon-8.0.0rc3/apache_airflow_providers_amazon.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-26 09:36:01.000000 apache-airflow-providers-amazon-8.0.0rc3/apache_airflow_providers_amazon.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5246 2023-04-07 12:28:58.000000 apache-airflow-providers-amazon-8.0.0rc3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2083 2023-04-26 09:36:03.000000 apache-airflow-providers-amazon-8.0.0rc3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2363 2023-04-26 09:35:57.000000 apache-airflow-providers-amazon-8.0.0rc3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-amazon-8.1.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1219 2023-05-16 15:52:48.000000 apache-airflow-providers-amazon-8.1.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-amazon-8.1.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    59663 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    57842 2023-05-16 15:52:48.000000 apache-airflow-providers-amazon-8.1.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/
+-rw-r--r--   0 root         (0) root         (0)     1389 2023-05-16 15:39:21.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1731 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4856 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/appflow.py
+-rw-r--r--   0 root         (0) root         (0)    12240 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/athena.py
+-rw-r--r--   0 root         (0) root         (0)    45981 2023-05-12 08:38:07.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/base_aws.py
+-rw-r--r--   0 root         (0) root         (0)    20625 2023-05-15 07:14:11.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/batch_client.py
+-rw-r--r--   0 root         (0) root         (0)     2511 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/batch_waiters.json
+-rw-r--r--   0 root         (0) root         (0)     9697 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/batch_waiters.py
+-rw-r--r--   0 root         (0) root         (0)     3376 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/cloud_formation.py
+-rw-r--r--   0 root         (0) root         (0)    14133 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/datasync.py
+-rw-r--r--   0 root         (0) root         (0)     7906 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/dms.py
+-rw-r--r--   0 root         (0) root         (0)     2668 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/dynamodb.py
+-rw-r--r--   0 root         (0) root         (0)     7921 2023-05-15 07:14:11.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/ec2.py
+-rw-r--r--   0 root         (0) root         (0)     3702 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/ecr.py
+-rw-r--r--   0 root         (0) root         (0)     9194 2023-03-06 20:52:28.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/ecs.py
+-rw-r--r--   0 root         (0) root         (0)    23957 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/eks.py
+-rw-r--r--   0 root         (0) root         (0)    12114 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py
+-rw-r--r--   0 root         (0) root         (0)    20465 2023-05-03 19:47:07.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/emr.py
+-rw-r--r--   0 root         (0) root         (0)     3518 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/glacier.py
+-rw-r--r--   0 root         (0) root         (0)    14759 2023-04-30 16:30:42.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/glue.py
+-rw-r--r--   0 root         (0) root         (0)     7611 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/glue_catalog.py
+-rw-r--r--   0 root         (0) root         (0)     8895 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/glue_crawler.py
+-rw-r--r--   0 root         (0) root         (0)     1993 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/kinesis.py
+-rw-r--r--   0 root         (0) root         (0)     8008 2023-02-24 18:53:47.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/lambda_function.py
+-rw-r--r--   0 root         (0) root         (0)     4823 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/logs.py
+-rw-r--r--   0 root         (0) root         (0)     7219 2023-04-07 12:28:57.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/quicksight.py
+-rw-r--r--   0 root         (0) root         (0)    15272 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/rds.py
+-rw-r--r--   0 root         (0) root         (0)    13287 2023-05-03 19:47:07.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/redshift_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     7720 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/redshift_data.py
+-rw-r--r--   0 root         (0) root         (0)     7072 2023-05-03 19:47:07.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/redshift_sql.py
+-rw-r--r--   0 root         (0) root         (0)    43170 2023-05-12 08:38:07.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/s3.py
+-rw-r--r--   0 root         (0) root         (0)    56676 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     2692 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/secrets_manager.py
+-rw-r--r--   0 root         (0) root         (0)     4143 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/ses.py
+-rw-r--r--   0 root         (0) root         (0)     3461 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/sns.py
+-rw-r--r--   0 root         (0) root         (0)     3119 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/sqs.py
+-rw-r--r--   0 root         (0) root         (0)     2449 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/ssm.py
+-rw-r--r--   0 root         (0) root         (0)     3072 2023-05-04 19:22:39.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/step_function.py
+-rw-r--r--   0 root         (0) root         (0)     1817 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/sts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/links/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/links/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2943 2023-05-04 19:17:30.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/links/base_aws.py
+-rw-r--r--   0 root         (0) root         (0)     1767 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/links/batch.py
+-rw-r--r--   0 root         (0) root         (0)     2401 2023-05-04 19:17:30.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/links/emr.py
+-rw-r--r--   0 root         (0) root         (0)     1228 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/links/glue.py
+-rw-r--r--   0 root         (0) root         (0)     1607 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/links/logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/log/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5072 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py
+-rw-r--r--   0 root         (0) root         (0)     9635 2023-03-10 19:31:58.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/log/s3_task_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19677 2023-03-06 20:52:28.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/appflow.py
+-rw-r--r--   0 root         (0) root         (0)     6141 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/athena.py
+-rw-r--r--   0 root         (0) root         (0)    16635 2023-05-15 07:14:11.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/batch.py
+-rw-r--r--   0 root         (0) root         (0)     3633 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/cloud_formation.py
+-rw-r--r--   0 root         (0) root         (0)    18419 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/datasync.py
+-rw-r--r--   0 root         (0) root         (0)    10715 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/dms.py
+-rw-r--r--   0 root         (0) root         (0)     9589 2023-03-10 19:31:58.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/ec2.py
+-rw-r--r--   0 root         (0) root         (0)    29018 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/ecs.py
+-rw-r--r--   0 root         (0) root         (0)    31814 2023-05-03 19:47:07.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/eks.py
+-rw-r--r--   0 root         (0) root         (0)    53336 2023-05-12 22:41:38.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/emr.py
+-rw-r--r--   0 root         (0) root         (0)     3705 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/glacier.py
+-rw-r--r--   0 root         (0) root         (0)     7471 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/glue.py
+-rw-r--r--   0 root         (0) root         (0)     3306 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/glue_crawler.py
+-rw-r--r--   0 root         (0) root         (0)     7755 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/lambda_function.py
+-rw-r--r--   0 root         (0) root         (0)     3972 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/quicksight.py
+-rw-r--r--   0 root         (0) root         (0)    29868 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/rds.py
+-rw-r--r--   0 root         (0) root         (0)    29124 2023-05-03 19:47:07.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/redshift_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     5559 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/redshift_data.py
+-rw-r--r--   0 root         (0) root         (0)    29966 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/s3.py
+-rw-r--r--   0 root         (0) root         (0)    55195 2023-05-12 08:38:07.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     2959 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/sns.py
+-rw-r--r--   0 root         (0) root         (0)     3563 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/sqs.py
+-rw-r--r--   0 root         (0) root         (0)     4583 2023-05-05 08:06:03.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/step_function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/secrets/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15628 2023-05-03 19:47:07.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/secrets/secrets_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8503 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/secrets/systems_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3120 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/athena.py
+-rw-r--r--   0 root         (0) root         (0)     7384 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/batch.py
+-rw-r--r--   0 root         (0) root         (0)     4163 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/cloud_formation.py
+-rw-r--r--   0 root         (0) root         (0)     3998 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/dms.py
+-rw-r--r--   0 root         (0) root         (0)     3915 2023-04-19 10:00:26.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/dynamodb.py
+-rw-r--r--   0 root         (0) root         (0)     3658 2023-05-15 07:14:11.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/ec2.py
+-rw-r--r--   0 root         (0) root         (0)     7203 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/ecs.py
+-rw-r--r--   0 root         (0) root         (0)     9786 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/eks.py
+-rw-r--r--   0 root         (0) root         (0)    19390 2023-05-04 19:17:30.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/emr.py
+-rw-r--r--   0 root         (0) root         (0)     4129 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/glacier.py
+-rw-r--r--   0 root         (0) root         (0)     3332 2023-04-30 16:30:42.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/glue.py
+-rw-r--r--   0 root         (0) root         (0)     3732 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py
+-rw-r--r--   0 root         (0) root         (0)     2963 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/glue_crawler.py
+-rw-r--r--   0 root         (0) root         (0)     3064 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/lambda_function.py
+-rw-r--r--   0 root         (0) root         (0)     3641 2023-04-07 12:28:57.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/quicksight.py
+-rw-r--r--   0 root         (0) root         (0)     6447 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/rds.py
+-rw-r--r--   0 root         (0) root         (0)     2637 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/redshift_cluster.py
+-rw-r--r--   0 root         (0) root         (0)    11650 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/s3.py
+-rw-r--r--   0 root         (0) root         (0)    13057 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     9584 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/sqs.py
+-rw-r--r--   0 root         (0) root         (0)     3400 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/step_function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2848 2023-05-03 19:47:07.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/base.py
+-rw-r--r--   0 root         (0) root         (0)     7703 2023-05-12 08:38:07.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     4410 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/exasol_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     6435 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/ftp_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     7676 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/gcs_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     4701 2023-04-21 10:05:41.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py
+-rw-r--r--   0 root         (0) root         (0)     9042 2023-04-21 10:05:41.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/google_api_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     4172 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py
+-rw-r--r--   0 root         (0) root         (0)     4248 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     4158 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/local_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     6007 2023-05-16 07:40:59.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/mongo_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     8108 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/redshift_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     2966 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/s3_to_ftp.py
+-rw-r--r--   0 root         (0) root         (0)     8286 2023-05-05 08:06:03.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/s3_to_redshift.py
+-rw-r--r--   0 root         (0) root         (0)     3191 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/s3_to_sftp.py
+-rw-r--r--   0 root         (0) root         (0)     4620 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/s3_to_sql.py
+-rw-r--r--   0 root         (0) root         (0)     5679 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     3679 2023-04-07 12:28:57.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/sftp_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     8475 2023-04-19 10:00:26.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/sql_to_s3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/triggers/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-03-14 06:24:40.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3006 2023-05-15 07:14:11.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/triggers/ec2.py
+-rw-r--r--   0 root         (0) root         (0)     5579 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/triggers/redshift_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     3853 2023-05-12 08:38:07.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/triggers/sagemaker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/utils/
+-rw-r--r--   0 root         (0) root         (0)     2215 2023-03-06 20:52:28.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20488 2023-05-03 19:47:07.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/utils/connection_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     2561 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/utils/eks_get_token.py
+-rw-r--r--   0 root         (0) root         (0)     1853 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/utils/emailer.py
+-rw-r--r--   0 root         (0) root         (0)      972 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/utils/rds.py
+-rw-r--r--   0 root         (0) root         (0)     1913 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/utils/redshift.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/utils/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     1701 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/utils/tags.py
+-rw-r--r--   0 root         (0) root         (0)     3583 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/utils/waiter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/waiters/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/waiters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/waiters/appflow.json
+-rw-r--r--   0 root         (0) root         (0)     1853 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/waiters/base_waiter.py
+-rw-r--r--   0 root         (0) root         (0)      895 2023-05-12 08:38:07.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/waiters/dynamodb.json
+-rw-r--r--   0 root         (0) root         (0)     2720 2023-03-02 08:17:44.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/waiters/ecs.json
+-rw-r--r--   0 root         (0) root         (0)      659 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/waiters/eks.json
+-rw-r--r--   0 root         (0) root         (0)      430 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/waiters/emr-serverless.json
+-rw-r--r--   0 root         (0) root         (0)     2559 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/waiters/emr.json
+-rw-r--r--   0 root         (0) root         (0)     2699 2023-05-12 08:38:07.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/waiters/sagemaker.json
+-rw-r--r--   0 root         (0) root         (0)    36891 2023-05-16 15:52:48.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/apache_airflow_providers_amazon.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    59663 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/apache_airflow_providers_amazon.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7463 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/apache_airflow_providers_amazon.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/apache_airflow_providers_amazon.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/apache_airflow_providers_amazon.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/apache_airflow_providers_amazon.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      806 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/apache_airflow_providers_amazon.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/apache_airflow_providers_amazon.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-amazon-8.1.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2106 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2363 2023-05-16 15:52:48.000000 apache-airflow-providers-amazon-8.1.0rc1/setup.py
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/LICENSE` & `apache-airflow-providers-amazon-8.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/MANIFEST.in` & `apache-airflow-providers-amazon-8.1.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/PKG-INFO` & `apache-airflow-providers-amazon-8.1.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-amazon
-Version: 8.0.0rc3
+Version: 8.1.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-amazon package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.0.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.1.0/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -60,28 +60,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-amazon``
 
-Release: ``8.0.0rc3``
+Release: ``8.1.0rc1``
 
 
 Amazon integration (including `Amazon Web Services (AWS) <https://aws.amazon.com/>`__).
 
 
 Provider package
 ----------------
 
 This is a provider package for ``amazon`` provider. All classes for this provider package
 are in ``airflow.providers.amazon`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.0.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.1.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -91,25 +91,26 @@
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
-``apache-airflow``                       ``>=2.3.0``
+``apache-airflow``                       ``>=2.4.0``
 ``apache-airflow-providers-common-sql``  ``>=1.3.1``
 ``boto3``                                ``>=1.24.0``
 ``asgiref``
 ``watchtower``                           ``~=2.0.1``
 ``jsonpath_ng``                          ``>=1.5.3``
 ``redshift_connector``                   ``>=2.0.888``
 ``sqlalchemy_redshift``                  ``>=0.8.6``
 ``mypy-boto3-rds``                       ``>=1.24.0``
 ``mypy-boto3-redshift-data``             ``>=1.24.0``
 ``mypy-boto3-appflow``                   ``>=1.24.0``
+``mypy-boto3-s3``                        ``>=1.24.0``
 =======================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
 Those are dependencies that might be needed in order to use all the features of the package.
 You need to install the specified provider packages in order to use them.
@@ -158,14 +159,62 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+8.1.0
+.....
+
+.. note::
+  This release of provider is only available for Airflow 2.4+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
+
+Features
+~~~~~~~~
+
+* ``DynamoDBToS3Operator - Add a feature to export the table to a point in time. (#31142)``
+* ``Add deferrable param in SageMakerTransformOperator (#31063)``
+* ``Add deferrable param in SageMakerTrainingOperator (#31042)``
+* ``Add deferrable param in SageMakerProcessingOperator (#31062)``
+* ``Add IAM authentication to Amazon Redshift Connection by AWS Connection (#28187)``
+* ``'StepFunctionStartExecutionOperator': get logs in case of failure (#31072)``
+* ``Add on_kill to EMR Serverless Job Operator (#31169)``
+* ``Add Deferrable Mode for EC2StateSensor (#31130)``
+
+Bug Fixes
+~~~~~~~~~
+
+* ``bigfix: EMRHook  Loop through paginated response to check for cluster id (#29732)``
+
+Misc
+~~~~
+
+* ``Bump minimum Airflow version in providers (#30917)``
+* ``Add template field to S3ToRedshiftOperator (#30781)``
+* ``Add extras links to some more EMR Operators and Sensors (#31032)``
+* ``Add retries to S3 delete_bucket (#31192)``
+* ``Add tags param in RedshiftCreateClusterSnapshotOperator (#31006)``
+* ``improve/fix glue job logs printing (#30886)``
+* ``Import aiobotocore only if deferrable is true (#31094)``
+* ``Update return types of 'get_key' methods on 'S3Hook' (#30923)``
+* ``Support 'shareIdentifier' in BatchOperator (#30829)``
+* ``BaseAWS - Override client when resource_type is user to get custom waiters (#30897)``
+* ``Add future-compatible mongo Hook typing (#31289)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Move TaskInstanceKey to a separate file (#31033)``
+   * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
+   * ``DynamoDBToS3Operator - Add feature to export table to a point in time (#30501)``
+   * ``Revert "DynamoDBToS3Operator - Add feature to export table to a point in time (#30501)" (#31139)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Bring back detection of implicit single-line string concatenation (#31270)``
+
 8.0.0
 ......
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
 .. warning::
@@ -480,16 +529,17 @@
    appropriate section above if needed. Do not delete the lines(!):
    * ``System Test for EMR (AIP-47) (#27286)``
    * ``Prepare for follow-up release for November providers (#27774)``
 
 6.1.0
 .....
 
-This release of provider is only available for Airflow 2.3+ as explained in the
-`Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/README.md#support-for-providers>`_.
+.. note::
+  This release of provider is only available for Airflow 2.3+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Misc
 ~~~~
 
 * ``Move min airflow version to 2.3.0 for all providers (#27196)``
 * ``Replace urlparse with urlsplit (#27389)``
 
@@ -720,16 +770,17 @@
 
 4.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
-* This release of provider is only available for Airflow 2.2+ as explained in the Apache Airflow
-  providers support policy https://github.com/apache/airflow/blob/main/README.md#support-for-providers
+.. note::
+  This release of provider is only available for Airflow 2.2+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Features
 ~~~~~~~~
 
 * ``Add partition related methods to GlueCatalogHook: (#23857)``
 * ``Add support for associating  custom tags to job runs submitted via EmrContainerOperator (#23769)``
 * ``Add number of node params only for single-node cluster in RedshiftCreateClusterOperator (#23839)``
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/README.rst` & `apache-airflow-providers-amazon-8.1.0rc1/apache_airflow_providers_amazon.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,52 @@
+Metadata-Version: 2.1
+Name: apache-airflow-providers-amazon
+Version: 8.1.0rc1
+Summary: Provider for Apache Airflow. Implements apache-airflow-providers-amazon package
+Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
+Author: Apache Software Foundation
+Author-email: dev@airflow.apache.org
+License: Apache License 2.0
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.1.0/
+Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
+Project-URL: Source Code, https://github.com/apache/airflow
+Project-URL: Slack Chat, https://s.apache.org/airflow-slack
+Project-URL: Twitter, https://twitter.com/ApacheAirflow
+Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: System Administrators
+Classifier: Framework :: Apache Airflow
+Classifier: Framework :: Apache Airflow :: Provider
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: System :: Monitoring
+Requires-Python: ~=3.7
+Description-Content-Type: text/x-rst
+Provides-Extra: apache.hive
+Provides-Extra: cncf.kubernetes
+Provides-Extra: common.sql
+Provides-Extra: exasol
+Provides-Extra: ftp
+Provides-Extra: google
+Provides-Extra: imap
+Provides-Extra: mongo
+Provides-Extra: salesforce
+Provides-Extra: ssh
+Provides-Extra: pandas
+Provides-Extra: aiobotocore
+License-File: LICENSE
+License-File: NOTICE
+
 
 .. Licensed to the Apache Software Foundation (ASF) under one
    or more contributor license agreements.  See the NOTICE file
    distributed with this work for additional information
    regarding copyright ownership.  The ASF licenses this file
    to you under the Apache License, Version 2.0 (the
    "License"); you may not use this file except in compliance
@@ -15,28 +60,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-amazon``
 
-Release: ``8.0.0rc3``
+Release: ``8.1.0rc1``
 
 
 Amazon integration (including `Amazon Web Services (AWS) <https://aws.amazon.com/>`__).
 
 
 Provider package
 ----------------
 
 This is a provider package for ``amazon`` provider. All classes for this provider package
 are in ``airflow.providers.amazon`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.0.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.1.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -46,25 +91,26 @@
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
-``apache-airflow``                       ``>=2.3.0``
+``apache-airflow``                       ``>=2.4.0``
 ``apache-airflow-providers-common-sql``  ``>=1.3.1``
 ``boto3``                                ``>=1.24.0``
 ``asgiref``
 ``watchtower``                           ``~=2.0.1``
 ``jsonpath_ng``                          ``>=1.5.3``
 ``redshift_connector``                   ``>=2.0.888``
 ``sqlalchemy_redshift``                  ``>=0.8.6``
 ``mypy-boto3-rds``                       ``>=1.24.0``
 ``mypy-boto3-redshift-data``             ``>=1.24.0``
 ``mypy-boto3-appflow``                   ``>=1.24.0``
+``mypy-boto3-s3``                        ``>=1.24.0``
 =======================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
 Those are dependencies that might be needed in order to use all the features of the package.
 You need to install the specified provider packages in order to use them.
@@ -113,14 +159,62 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+8.1.0
+.....
+
+.. note::
+  This release of provider is only available for Airflow 2.4+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
+
+Features
+~~~~~~~~
+
+* ``DynamoDBToS3Operator - Add a feature to export the table to a point in time. (#31142)``
+* ``Add deferrable param in SageMakerTransformOperator (#31063)``
+* ``Add deferrable param in SageMakerTrainingOperator (#31042)``
+* ``Add deferrable param in SageMakerProcessingOperator (#31062)``
+* ``Add IAM authentication to Amazon Redshift Connection by AWS Connection (#28187)``
+* ``'StepFunctionStartExecutionOperator': get logs in case of failure (#31072)``
+* ``Add on_kill to EMR Serverless Job Operator (#31169)``
+* ``Add Deferrable Mode for EC2StateSensor (#31130)``
+
+Bug Fixes
+~~~~~~~~~
+
+* ``bigfix: EMRHook  Loop through paginated response to check for cluster id (#29732)``
+
+Misc
+~~~~
+
+* ``Bump minimum Airflow version in providers (#30917)``
+* ``Add template field to S3ToRedshiftOperator (#30781)``
+* ``Add extras links to some more EMR Operators and Sensors (#31032)``
+* ``Add retries to S3 delete_bucket (#31192)``
+* ``Add tags param in RedshiftCreateClusterSnapshotOperator (#31006)``
+* ``improve/fix glue job logs printing (#30886)``
+* ``Import aiobotocore only if deferrable is true (#31094)``
+* ``Update return types of 'get_key' methods on 'S3Hook' (#30923)``
+* ``Support 'shareIdentifier' in BatchOperator (#30829)``
+* ``BaseAWS - Override client when resource_type is user to get custom waiters (#30897)``
+* ``Add future-compatible mongo Hook typing (#31289)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Move TaskInstanceKey to a separate file (#31033)``
+   * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
+   * ``DynamoDBToS3Operator - Add feature to export table to a point in time (#30501)``
+   * ``Revert "DynamoDBToS3Operator - Add feature to export table to a point in time (#30501)" (#31139)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Bring back detection of implicit single-line string concatenation (#31270)``
+
 8.0.0
 ......
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
 .. warning::
@@ -435,16 +529,17 @@
    appropriate section above if needed. Do not delete the lines(!):
    * ``System Test for EMR (AIP-47) (#27286)``
    * ``Prepare for follow-up release for November providers (#27774)``
 
 6.1.0
 .....
 
-This release of provider is only available for Airflow 2.3+ as explained in the
-`Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/README.md#support-for-providers>`_.
+.. note::
+  This release of provider is only available for Airflow 2.3+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Misc
 ~~~~
 
 * ``Move min airflow version to 2.3.0 for all providers (#27196)``
 * ``Replace urlparse with urlsplit (#27389)``
 
@@ -675,16 +770,17 @@
 
 4.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
-* This release of provider is only available for Airflow 2.2+ as explained in the Apache Airflow
-  providers support policy https://github.com/apache/airflow/blob/main/README.md#support-for-providers
+.. note::
+  This release of provider is only available for Airflow 2.2+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Features
 ~~~~~~~~
 
 * ``Add partition related methods to GlueCatalogHook: (#23857)``
 * ``Add support for associating  custom tags to job runs submitted via EmrContainerOperator (#23769)``
 * ``Add number of node params only for single-node cluster in RedshiftCreateClusterOperator (#23839)``
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/__init__.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/__init__.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/exceptions.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/exceptions.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/__init__.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/links/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/appflow.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/appflow.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/athena.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/athena.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/base_aws.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/base_aws.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,15 +190,14 @@
 
     def _create_basic_session(self, session_kwargs: dict[str, Any]) -> boto3.session.Session:
         return boto3.session.Session(**session_kwargs)
 
     def _create_session_with_assume_role(
         self, session_kwargs: dict[str, Any], deferrable: bool = False
     ) -> boto3.session.Session:
-        from aiobotocore.session import get_session as async_get_session
 
         if self.conn.assume_role_method == "assume_role_with_web_identity":
             # Deferred credentials have no initial credentials
             credential_fetcher = self._get_web_identity_credential_fetcher()
             credentials = botocore.credentials.DeferredRefreshableCredentials(
                 method="assume-role-with-web-identity",
                 refresh_using=credential_fetcher.fetch_credentials,
@@ -208,15 +207,20 @@
             # Refreshable credentials do have initial credentials
             credentials = botocore.credentials.RefreshableCredentials.create_from_metadata(
                 metadata=self._refresh_credentials(),
                 refresh_using=self._refresh_credentials,
                 method="sts-assume-role",
             )
 
-        session = async_get_session() if deferrable else botocore.session.get_session()
+        if deferrable:
+            from aiobotocore.session import get_session as async_get_session
+
+            session = async_get_session()
+        else:
+            session = botocore.session.get_session()
 
         session._credentials = credentials
         session.set_config_variable("region", self.basic_session.region_name)
 
         return boto3.session.Session(botocore_session=session, **session_kwargs)
 
     def _refresh_credentials(self) -> dict[str, Any]:
@@ -837,14 +841,24 @@
         """
         from airflow.providers.amazon.aws.waiters.base_waiter import BaseBotoWaiter
 
         if deferrable and not client:
             raise ValueError("client must be provided for a deferrable waiter.")
         client = client or self.conn
         if self.waiter_path and (waiter_name in self._list_custom_waiters()):
+            # Currently, the custom waiter doesn't work with resource_type, only client_type is supported.
+            if self.resource_type:
+                credentials = self.get_credentials()
+                client = boto3.client(
+                    self.resource_type,
+                    region_name=self.region_name,
+                    aws_access_key_id=credentials.access_key,
+                    aws_secret_access_key=credentials.secret_key,
+                )
+
             # Technically if waiter_name is in custom_waiters then self.waiter_path must
             # exist but MyPy doesn't like the fact that self.waiter_path could be None.
             with open(self.waiter_path) as config_file:
                 config = json.loads(config_file.read())
 
             config = self._apply_parameters_value(config, waiter_name, parameters)
             return BaseBotoWaiter(client=client, model_config=config, deferrable=deferrable).waiter(
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/batch_client.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/batch_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -415,15 +415,15 @@
 
     def get_job_awslogs_info(self, job_id: str) -> dict[str, str] | None:
         all_info = self.get_job_all_awslogs_info(job_id)
         if not all_info:
             return None
         if len(all_info) > 1:
             self.log.warning(
-                f"AWS Batch job ({job_id}) has more than one log stream, " f"only returning the first one."
+                f"AWS Batch job ({job_id}) has more than one log stream, only returning the first one."
             )
         return all_info[0]
 
     def get_job_all_awslogs_info(self, job_id: str) -> list[dict[str, str]]:
         """
         Parse job description to extract AWS CloudWatch information.
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/batch_waiters.json` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/batch_waiters.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/batch_waiters.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/batch_waiters.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/cloud_formation.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/cloud_formation.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/datasync.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/datasync.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/dms.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/dms.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/dynamodb.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/dynamodb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/ec2.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/ec2.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,14 +162,19 @@
         Get list of instance ids, optionally applying filters to fetch selective instances
 
         :param filters: List of filters to specify instances to get
         :return: List of instance ids
         """
         return [instance["InstanceId"] for instance in self.get_instances(filters=filters)]
 
+    async def get_instance_state_async(self, instance_id: str) -> str:
+        async with self.async_conn as client:
+            response = await client.describe_instances(InstanceIds=[instance_id])
+            return response["Reservations"][0]["Instances"][0]["State"]["Name"]
+
     def get_instance_state(self, instance_id: str) -> str:
         """
         Get EC2 instance state by id and return it.
 
         :param instance_id: id of the AWS EC2 instance
         :return: current state of the instance
         """
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/ecr.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/ecr.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/ecs.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/ecs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/eks.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/eks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/emr.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/emr.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,19 +63,23 @@
         .. seealso::
             - :external+boto3:py:meth:`EMR.Client.list_clusters`
 
         :param emr_cluster_name: Name of a cluster to find
         :param cluster_states: State(s) of cluster to find
         :return: id of the EMR cluster
         """
-        response = self.get_conn().list_clusters(ClusterStates=cluster_states)
-
-        matching_clusters = list(
-            filter(lambda cluster: cluster["Name"] == emr_cluster_name, response["Clusters"])
+        response_iterator = (
+            self.get_conn().get_paginator("list_clusters").paginate(ClusterStates=cluster_states)
         )
+        matching_clusters = [
+            cluster
+            for page in response_iterator
+            for cluster in page["Clusters"]
+            if cluster["Name"] == emr_cluster_name
+        ]
 
         if len(matching_clusters) == 1:
             cluster_id = matching_clusters[0]["Id"]
             self.log.info("Found cluster name = %s id = %s", emr_cluster_name, cluster_id)
             return cluster_id
         elif len(matching_clusters) > 1:
             raise AirflowException(f"More than one cluster found for name {emr_cluster_name}")
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/glacier.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/glacier.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/glue.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/glue.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,24 +16,21 @@
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 import time
 
 import boto3
+from botocore.exceptions import ClientError
 
 from airflow.exceptions import AirflowException
 from airflow.providers.amazon.aws.hooks.base_aws import AwsBaseHook
 
 DEFAULT_LOG_SUFFIX = "output"
-FAILURE_LOG_SUFFIX = "error"
-# A filter value of ' ' translates to "match all".
-# see: https://docs.aws.amazon.com/AmazonCloudWatch/latest/logs/FilterAndPatternSyntax.html
-DEFAULT_LOG_FILTER = " "
-FAILURE_LOG_FILTER = "?ERROR ?Exception"
+ERROR_LOG_SUFFIX = "error"
 
 
 class GlueJobHook(AwsBaseHook):
     """
     Interact with AWS Glue.
     Provide thick wrapper around :external+boto3:py:class:`boto3.client("glue") <Glue.Client>`.
 
@@ -54,14 +51,21 @@
 
     .. seealso::
         - :class:`airflow.providers.amazon.aws.hooks.base_aws.AwsBaseHook`
     """
 
     JOB_POLL_INTERVAL = 6  # polls job status after every JOB_POLL_INTERVAL seconds
 
+    class LogContinuationTokens:
+        """Used to hold the continuation tokens when reading logs from both streams Glue Jobs write to."""
+
+        def __init__(self):
+            self.output_stream_continuation: str | None = None
+            self.error_stream_continuation: str | None = None
+
     def __init__(
         self,
         s3_bucket: str | None = None,
         job_name: str | None = None,
         desc: str | None = None,
         concurrent_run_limit: int = 1,
         script_location: str | None = None,
@@ -190,96 +194,106 @@
         job_run = self.conn.get_job_run(JobName=job_name, RunId=run_id, PredecessorsIncluded=True)
         return job_run["JobRun"]["JobRunState"]
 
     def print_job_logs(
         self,
         job_name: str,
         run_id: str,
-        job_failed: bool = False,
-        next_token: str | None = None,
-    ) -> str | None:
-        """Prints the batch of logs to the Airflow task log and returns nextToken."""
-        log_client = boto3.client("logs")
-        response = {}
+        continuation_tokens: LogContinuationTokens,
+    ):
+        """
+        Prints the latest job logs to the Airflow task log and updates the continuation tokens.
 
-        filter_pattern = FAILURE_LOG_FILTER if job_failed else DEFAULT_LOG_FILTER
-        log_group_prefix = self.conn.get_job_run(JobName=job_name, RunId=run_id)["JobRun"]["LogGroupName"]
-        log_group_suffix = FAILURE_LOG_SUFFIX if job_failed else DEFAULT_LOG_SUFFIX
-        log_group_name = f"{log_group_prefix}/{log_group_suffix}"
+        :param continuation_tokens: the tokens where to resume from when reading logs.
+            The object gets updated with the new tokens by this method.
+        """
+        log_client = boto3.client("logs")
+        paginator = log_client.get_paginator("filter_log_events")
 
-        try:
-            if next_token:
-                response = log_client.filter_log_events(
-                    logGroupName=log_group_name,
+        def display_logs_from(log_group: str, continuation_token: str | None) -> str | None:
+            """Internal method to mutualize iteration over the 2 different log streams glue jobs write to"""
+            fetched_logs = []
+            next_token = continuation_token
+            try:
+                for response in paginator.paginate(
+                    logGroupName=log_group,
                     logStreamNames=[run_id],
-                    filterPattern=filter_pattern,
-                    nextToken=next_token,
-                )
+                    PaginationConfig={"StartingToken": continuation_token},
+                ):
+                    fetched_logs.extend([event["message"] for event in response["events"]])
+                    # if the response is empty there is no nextToken in it
+                    next_token = response.get("nextToken") or next_token
+            except ClientError as e:
+                if e.response["Error"]["Code"] == "ResourceNotFoundException":
+                    # we land here when the log groups/streams don't exist yet
+                    self.log.warning(
+                        "No new Glue driver logs so far.\nIf this persists, check the CloudWatch dashboard "
+                        f"at: https://{self.conn_region_name}.console.aws.amazon.com/cloudwatch/home"
+                    )
+                else:
+                    raise
+
+            if len(fetched_logs):
+                # Add a tab to indent those logs and distinguish them from airflow logs.
+                # Log lines returned already contain a newline character at the end.
+                messages = "\t".join(fetched_logs)
+                self.log.info("Glue Job Run %s Logs:\n\t%s", log_group, messages)
             else:
-                response = log_client.filter_log_events(
-                    logGroupName=log_group_name,
-                    logStreamNames=[run_id],
-                    filterPattern=filter_pattern,
-                )
-            if len(response["events"]):
-                messages = "\t".join([event["message"] for event in response["events"]])
-                self.log.info("Glue Job Run Logs:\n\t%s", messages)
-
-        except log_client.exceptions.ResourceNotFoundException:
-            self.log.warning(
-                "No new Glue driver logs found. This might be because there are no new logs, "
-                "or might be an error.\nIf the error persists, check the CloudWatch dashboard "
-                f"at: https://{self.conn_region_name}.console.aws.amazon.com/cloudwatch/home"
-            )
+                self.log.info("No new log from the Glue Job in %s", log_group)
+            return next_token
 
-        # If no new log events are available, filter_log_events will return None.
-        # In that case, check the same token again next pass.
-        return response.get("nextToken") or next_token
+        log_group_prefix = self.conn.get_job_run(JobName=job_name, RunId=run_id)["JobRun"]["LogGroupName"]
+        log_group_default = f"{log_group_prefix}/{DEFAULT_LOG_SUFFIX}"
+        log_group_error = f"{log_group_prefix}/{ERROR_LOG_SUFFIX}"
+
+        # one would think that the error log group would contain only errors, but it actually contains
+        # a lot of interesting logs too, so it's valuable to have both
+        continuation_tokens.output_stream_continuation = display_logs_from(
+            log_group_default, continuation_tokens.output_stream_continuation
+        )
+        continuation_tokens.error_stream_continuation = display_logs_from(
+            log_group_error, continuation_tokens.error_stream_continuation
+        )
 
     def job_completion(self, job_name: str, run_id: str, verbose: bool = False) -> dict[str, str]:
         """
         Waits until Glue job with job_name completes or fails and return final state if finished.
         Raises AirflowException when the job failed.
 
         :param job_name: unique job name per AWS account
         :param run_id: The job-run ID of the predecessor job run
         :param verbose: If True, more Glue Job Run logs show in the Airflow Task Logs.  (default: False)
         :return: Dict of JobRunState and JobRunId
         """
         failed_states = ["FAILED", "TIMEOUT"]
         finished_states = ["SUCCEEDED", "STOPPED"]
-        next_log_token = None
-        job_failed = False
-
+        next_log_tokens = self.LogContinuationTokens()
         while True:
-            try:
-                job_run_state = self.get_job_state(job_name, run_id)
-                if job_run_state in finished_states:
-                    self.log.info("Exiting Job %s Run State: %s", run_id, job_run_state)
-                    return {"JobRunState": job_run_state, "JobRunId": run_id}
-                if job_run_state in failed_states:
-                    job_failed = True
-                    job_error_message = f"Exiting Job {run_id} Run State: {job_run_state}"
-                    self.log.info(job_error_message)
-                    raise AirflowException(job_error_message)
-                else:
-                    self.log.info(
-                        "Polling for AWS Glue Job %s current run state with status %s",
-                        job_name,
-                        job_run_state,
-                    )
-                    time.sleep(self.JOB_POLL_INTERVAL)
-            finally:
-                if verbose:
-                    next_log_token = self.print_job_logs(
-                        job_name=job_name,
-                        run_id=run_id,
-                        job_failed=job_failed,
-                        next_token=next_log_token,
-                    )
+            if verbose:
+                self.print_job_logs(
+                    job_name=job_name,
+                    run_id=run_id,
+                    continuation_tokens=next_log_tokens,
+                )
+
+            job_run_state = self.get_job_state(job_name, run_id)
+            if job_run_state in finished_states:
+                self.log.info("Exiting Job %s Run State: %s", run_id, job_run_state)
+                return {"JobRunState": job_run_state, "JobRunId": run_id}
+            if job_run_state in failed_states:
+                job_error_message = f"Exiting Job {run_id} Run State: {job_run_state}"
+                self.log.info(job_error_message)
+                raise AirflowException(job_error_message)
+            else:
+                self.log.info(
+                    "Polling for AWS Glue Job %s current run state with status %s",
+                    job_name,
+                    job_run_state,
+                )
+                time.sleep(self.JOB_POLL_INTERVAL)
 
     def has_job(self, job_name) -> bool:
         """
         Checks if the job already exists.
 
         .. seealso::
             - :external+boto3:py:meth:`Glue.Client.get_job`
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/glue_catalog.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/glue_catalog.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/glue_crawler.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/glue_crawler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/kinesis.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/kinesis.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/lambda_function.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/lambda_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/logs.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/logs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/quicksight.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/quicksight.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/rds.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/rds.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/redshift_cluster.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/redshift_cluster.py`

 * *Files 5% similar despite different names*

```diff
@@ -152,31 +152,39 @@
         """
         response = self.get_conn().restore_from_cluster_snapshot(
             ClusterIdentifier=cluster_identifier, SnapshotIdentifier=snapshot_identifier
         )
         return response["Cluster"] if response["Cluster"] else None
 
     def create_cluster_snapshot(
-        self, snapshot_identifier: str, cluster_identifier: str, retention_period: int = -1
+        self,
+        snapshot_identifier: str,
+        cluster_identifier: str,
+        retention_period: int = -1,
+        tags: list[Any] | None = None,
     ) -> str:
         """
         Creates a snapshot of a cluster
 
         .. seealso::
             - :external+boto3:py:meth:`Redshift.Client.create_cluster_snapshot`
 
         :param snapshot_identifier: unique identifier for a snapshot of a cluster
         :param cluster_identifier: unique identifier of a cluster
         :param retention_period: The number of days that a manual snapshot is retained.
             If the value is -1, the manual snapshot is retained indefinitely.
+        :param tags: A list of tag instances
         """
+        if tags is None:
+            tags = []
         response = self.get_conn().create_cluster_snapshot(
             SnapshotIdentifier=snapshot_identifier,
             ClusterIdentifier=cluster_identifier,
             ManualSnapshotRetentionPeriod=retention_period,
+            Tags=tags,
         )
         return response["Snapshot"] if response["Snapshot"] else None
 
     def get_cluster_snapshot_status(self, snapshot_identifier: str):
         """
         Return Redshift cluster snapshot status. If cluster snapshot not found return ``None``
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/redshift_data.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/redshift_data.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/s3.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/s3.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,27 +29,31 @@
 from copy import deepcopy
 from datetime import datetime
 from functools import wraps
 from inspect import signature
 from io import BytesIO
 from pathlib import Path
 from tempfile import NamedTemporaryFile, gettempdir
-from typing import Any, Callable, TypeVar, cast
+from time import sleep
+from typing import TYPE_CHECKING, Any, Callable, TypeVar, cast
 from urllib.parse import urlsplit
 from uuid import uuid4
 
-from boto3.s3.transfer import S3Transfer, TransferConfig
+from boto3.s3.transfer import TransferConfig
 from botocore.exceptions import ClientError
 
-from airflow.exceptions import AirflowException
+from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
 from airflow.providers.amazon.aws.exceptions import S3HookUriParseFailure
 from airflow.providers.amazon.aws.hooks.base_aws import AwsBaseHook
 from airflow.providers.amazon.aws.utils.tags import format_tags
 from airflow.utils.helpers import chunks
 
+if TYPE_CHECKING:
+    from mypy_boto3_s3.service_resource import Object as S3ResourceObject
+
 T = TypeVar("T", bound=Callable)
 
 logger = logging.getLogger(__name__)
 
 
 def provide_bucket_name(func: T) -> T:
     """
@@ -70,15 +74,15 @@
             if "bucket_name" in self.service_config:
                 bound_args.arguments["bucket_name"] = self.service_config["bucket_name"]
             elif self.conn_config and self.conn_config.schema:
                 warnings.warn(
                     "s3 conn_type, and the associated schema field, is deprecated."
                     " Please use aws conn_type instead, and specify `bucket_name`"
                     " in `service_config.s3` within `extras`.",
-                    DeprecationWarning,
+                    AirflowProviderDeprecationWarning,
                     stacklevel=2,
                 )
                 bound_args.arguments["bucket_name"] = self.conn_config.schema
 
         return func(*bound_args.args, **bound_args.kwargs)
 
     return cast(T, wrapper)
@@ -517,15 +521,15 @@
         :return: True if the key exists and False if not.
         """
         obj = self.head_object(key, bucket_name)
         return obj is not None
 
     @unify_bucket_name_and_key
     @provide_bucket_name
-    def get_key(self, key: str, bucket_name: str | None = None) -> S3Transfer:
+    def get_key(self, key: str, bucket_name: str | None = None) -> S3ResourceObject:
         """
         Returns a :py:class:`S3.Object`.
 
         .. seealso::
             - :external+boto3:py:meth:`S3.ServiceResource.Object`
 
         :param key: the path to the key
@@ -622,15 +626,15 @@
             is not None
         )
 
     @unify_bucket_name_and_key
     @provide_bucket_name
     def get_wildcard_key(
         self, wildcard_key: str, bucket_name: str | None = None, delimiter: str = ""
-    ) -> S3Transfer:
+    ) -> S3ResourceObject | None:
         """
         Returns a boto3.s3.Object object matching the wildcard expression
 
         :param wildcard_key: the path to the key
         :param bucket_name: the name of the bucket
         :param delimiter: the delimiter marks key hierarchy
         :return: the key object from the bucket or None if none has been found.
@@ -884,29 +888,41 @@
         copy_source = {"Bucket": source_bucket_name, "Key": source_bucket_key, "VersionId": source_version_id}
         response = self.get_conn().copy_object(
             Bucket=dest_bucket_name, Key=dest_bucket_key, CopySource=copy_source, ACL=acl_policy
         )
         return response
 
     @provide_bucket_name
-    def delete_bucket(self, bucket_name: str, force_delete: bool = False) -> None:
+    def delete_bucket(self, bucket_name: str, force_delete: bool = False, max_retries: int = 5) -> None:
         """
         To delete s3 bucket, delete all s3 bucket objects and then delete the bucket.
 
         .. seealso::
             - :external+boto3:py:meth:`S3.Client.delete_bucket`
 
         :param bucket_name: Bucket name
         :param force_delete: Enable this to delete bucket even if not empty
+        :param max_retries: A bucket must be empty to be deleted.  If force_delete is true,
+            then retries may help prevent a race condition between deleting objects in the
+            bucket and trying to delete the bucket.
         :return: None
         """
+        tries_remaining = max_retries + 1
         if force_delete:
-            bucket_keys = self.list_keys(bucket_name=bucket_name)
-            if bucket_keys:
+            while tries_remaining:
+                bucket_keys = self.list_keys(bucket_name=bucket_name)
+                if not bucket_keys:
+                    break
+                if tries_remaining <= max_retries:
+                    # Avoid first loop
+                    sleep(500)
+
                 self.delete_objects(bucket=bucket_name, keys=bucket_keys)
+                tries_remaining -= 1
+
         self.conn.delete_bucket(Bucket=bucket_name)
 
     def delete_objects(self, bucket: str, keys: str | list) -> None:
         """
         Delete keys from the bucket.
 
         .. seealso::
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/sagemaker.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/sagemaker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/secrets_manager.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/ses.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/ses.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/sns.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/sns.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/sqs.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/sqs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/ssm.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/ssm.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/step_function.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/step_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/sts.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/sts.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/links/__init__.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/log/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/links/base_aws.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/links/base_aws.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from typing import TYPE_CHECKING, ClassVar
 
 from airflow.models import BaseOperatorLink, XCom
 
 if TYPE_CHECKING:
     from airflow.models import BaseOperator
-    from airflow.models.taskinstance import TaskInstanceKey
+    from airflow.models.taskinstancekey import TaskInstanceKey
     from airflow.utils.context import Context
 
 
 BASE_AWS_CONSOLE_LINK = "https://console.{aws_domain}"
 
 
 class BaseAwsLink(BaseOperatorLink):
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/links/batch.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/links/batch.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/links/emr.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/links/glue.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,21 +15,15 @@
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 from airflow.providers.amazon.aws.links.base_aws import BASE_AWS_CONSOLE_LINK, BaseAwsLink
 
 
-class EmrClusterLink(BaseAwsLink):
-    """Helper class for constructing AWS EMR Cluster Link"""
+class GlueJobRunDetailsLink(BaseAwsLink):
+    """Helper class for constructing AWS Glue Job Run Details Link"""
 
-    name = "EMR Cluster"
-    key = "emr_cluster"
-    format_str = BASE_AWS_CONSOLE_LINK + "/emr/home?region={region_name}#/clusterDetails/{job_flow_id}"
-
-
-class EmrLogsLink(BaseAwsLink):
-    """Helper class for constructing AWS EMR Logs Link"""
-
-    name = "EMR Cluster Logs"
-    key = "emr_logs"
-    format_str = BASE_AWS_CONSOLE_LINK + "/s3/buckets/{log_uri}?region={region_name}&prefix={job_flow_id}/"
+    name = "AWS Glue Job Run Details"
+    key = "glue_job_run_details"
+    format_str = (
+        BASE_AWS_CONSOLE_LINK + "/gluestudio/home?region={region_name}#/job/{job_name}/run/{job_run_id}"
+    )
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/links/glue.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/links/logs.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,18 +12,31 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
+from urllib.parse import quote_plus
+
 from airflow.providers.amazon.aws.links.base_aws import BASE_AWS_CONSOLE_LINK, BaseAwsLink
 
 
-class GlueJobRunDetailsLink(BaseAwsLink):
-    """Helper class for constructing AWS Glue Job Run Details Link"""
+class CloudWatchEventsLink(BaseAwsLink):
+    """Helper class for constructing AWS CloudWatch Events Link"""
 
-    name = "AWS Glue Job Run Details"
-    key = "glue_job_run_details"
+    name = "CloudWatch Events"
+    key = "cloudwatch_events"
     format_str = (
-        BASE_AWS_CONSOLE_LINK + "/gluestudio/home?region={region_name}#/job/{job_name}/run/{job_run_id}"
+        BASE_AWS_CONSOLE_LINK
+        + "/cloudwatch/home?region={awslogs_region}#logsV2:log-groups/log-group/{awslogs_group}"
+        + "/log-events/{awslogs_stream_name}"
     )
+
+    def format_link(self, **kwargs) -> str:
+        for field in ("awslogs_stream_name", "awslogs_group"):
+            if field in kwargs:
+                kwargs[field] = quote_plus(kwargs[field])
+            else:
+                return ""
+
+        return super().format_link(**kwargs)
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/links/logs.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/utils/tags.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,31 +12,27 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
-from urllib.parse import quote_plus
+from typing import Any
 
-from airflow.providers.amazon.aws.links.base_aws import BASE_AWS_CONSOLE_LINK, BaseAwsLink
 
-
-class CloudWatchEventsLink(BaseAwsLink):
-    """Helper class for constructing AWS CloudWatch Events Link"""
-
-    name = "CloudWatch Events"
-    key = "cloudwatch_events"
-    format_str = (
-        BASE_AWS_CONSOLE_LINK
-        + "/cloudwatch/home?region={awslogs_region}#logsV2:log-groups/log-group/{awslogs_group}"
-        + "/log-events/{awslogs_stream_name}"
-    )
-
-    def format_link(self, **kwargs) -> str:
-        for field in ("awslogs_stream_name", "awslogs_group"):
-            if field in kwargs:
-                kwargs[field] = quote_plus(kwargs[field])
-            else:
-                return ""
-
-        return super().format_link(**kwargs)
+def format_tags(source: Any, *, key_label: str = "Key", value_label: str = "Value"):
+    """
+    If given a dictionary, formats it as an array of objects with a key and a value field to be passed to boto
+    calls that expect this format.
+    Else, assumes that it's already in the right format and returns it as is. We do not validate
+    the format here since it's done by boto anyway, and the error would not be clearer if thrown from here.
+
+    :param source: a dict from which keys and values are read
+    :param key_label: optional, the label to use for keys if not "Key"
+    :param value_label: optional, the label to use for values if not "Value"
+    """
+    if source is None:
+        return []
+    elif isinstance(source, dict):
+        return [{key_label: kvp[0], value_label: kvp[1]} for kvp in source.items()]
+    else:
+        return source
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/log/__init__.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/log/s3_task_handler.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/log/s3_task_handler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/__init__.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/appflow.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/appflow.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/athena.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/athena.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/batch.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/batch.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 """
 from __future__ import annotations
 
 import warnings
 from typing import TYPE_CHECKING, Any, Sequence
 
 from airflow.compat.functools import cached_property
-from airflow.exceptions import AirflowException
+from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
 from airflow.models import BaseOperator
 from airflow.providers.amazon.aws.hooks.batch_client import BatchClientHook
 from airflow.providers.amazon.aws.links.batch import (
     BatchJobDefinitionLink,
     BatchJobDetailsLink,
     BatchJobQueueLink,
 )
@@ -54,14 +54,19 @@
 
     :param job_name: the name for the job that will run on AWS Batch (templated)
     :param job_definition: the job definition name on AWS Batch
     :param job_queue: the queue name on AWS Batch
     :param overrides: DEPRECATED, use container_overrides instead with the same value.
     :param container_overrides: the `containerOverrides` parameter for boto3 (templated)
     :param node_overrides: the `nodeOverrides` parameter for boto3 (templated)
+    :param share_identifier: The share identifier for the job. Don't specify this parameter if the job queue
+        doesn't have a scheduling policy.
+    :param scheduling_priority_override: The scheduling priority for the job.
+        Jobs with a higher scheduling priority are scheduled before jobs with a lower scheduling priority.
+        This overrides any scheduling priority in the job definition
     :param array_properties: the `arrayProperties` parameter for boto3
     :param parameters: the `parameters` for boto3 (templated)
     :param job_id: the job ID, usually unknown (None) until the
         submit_job operation gets the jobId defined by AWS Batch
     :param waiters: an :py:class:`.BatchWaiters` object (see note below);
         if None, polling is used with max_retries and status_retries.
     :param max_retries: exponential back-off retries, 4200 = 48 hours;
@@ -122,14 +127,16 @@
         job_name: str,
         job_definition: str,
         job_queue: str,
         overrides: dict | None = None,  # deprecated
         container_overrides: dict | None = None,
         array_properties: dict | None = None,
         node_overrides: dict | None = None,
+        share_identifier: str | None = None,
+        scheduling_priority_override: int | None = None,
         parameters: dict | None = None,
         job_id: str | None = None,
         waiters: Any | None = None,
         max_retries: int | None = None,
         status_retries: int | None = None,
         aws_conn_id: str | None = None,
         region_name: str | None = None,
@@ -152,19 +159,21 @@
                 raise AirflowException(
                     "'container_overrides' replaces the 'overrides' parameter. "
                     "You cannot specify both. Please remove assignation to the deprecated 'overrides'."
                 )
             self.container_overrides = overrides
             warnings.warn(
                 "Parameter `overrides` is deprecated, Please use `container_overrides` instead.",
-                DeprecationWarning,
+                AirflowProviderDeprecationWarning,
                 stacklevel=2,
             )
 
         self.node_overrides = node_overrides
+        self.share_identifier = share_identifier
+        self.scheduling_priority_override = scheduling_priority_override
         self.array_properties = array_properties
         self.parameters = parameters or {}
         self.waiters = waiters
         self.tags = tags or {}
         self.wait_for_completion = wait_for_completion
 
         # params for hook
@@ -223,14 +232,16 @@
             "jobQueue": self.job_queue,
             "jobDefinition": self.job_definition,
             "arrayProperties": self.array_properties,
             "parameters": self.parameters,
             "tags": self.tags,
             "containerOverrides": self.container_overrides,
             "nodeOverrides": self.node_overrides,
+            "shareIdentifier": self.share_identifier,
+            "schedulingPriorityOverride": self.scheduling_priority_override,
         }
 
         try:
             response = self.hook.client.submit_job(**trim_none_values(args))
         except Exception as e:
             self.log.error(
                 "AWS Batch job failed submission - job definition: %s - on queue %s",
@@ -299,15 +310,15 @@
             self.log.info("AWS Batch job (%s) CloudWatch Events details found. Links to logs:", self.job_id)
             link_builder = CloudWatchEventsLink()
             for log in awslogs:
                 self.log.info(link_builder.format_link(**log))
             if len(awslogs) > 1:
                 # there can be several log streams on multi-node jobs
                 self.log.warning(
-                    "out of all those logs, we can only link to one in the UI. " "Using the first one."
+                    "out of all those logs, we can only link to one in the UI. Using the first one."
                 )
 
             CloudWatchEventsLink.persist(
                 context=context,
                 operator=self,
                 region_name=self.hook.conn_region_name,
                 aws_partition=self.hook.conn_partition,
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/cloud_formation.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/cloud_formation.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/datasync.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/datasync.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/dms.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/dms.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/ec2.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/ec2.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/ecs.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/ecs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/eks.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/eks.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 import warnings
 from ast import literal_eval
 from typing import TYPE_CHECKING, Any, List, Sequence, cast
 
 from botocore.exceptions import ClientError, WaiterError
 
-from airflow import AirflowException
+from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
 from airflow.models import BaseOperator
 from airflow.providers.amazon.aws.hooks.eks import EksHook
 
 try:
     from airflow.providers.cncf.kubernetes.operators.pod import KubernetesPodOperator
 except ImportError:
     # preserve backward compatibility for older versions of cncf.kubernetes provider
@@ -687,15 +687,15 @@
     ) -> None:
         if is_delete_operator_pod is None:
             warnings.warn(
                 f"You have not set parameter `is_delete_operator_pod` in class {self.__class__.__name__}. "
                 "Currently the default for this parameter is `False` but in a future release the default "
                 "will be changed to `True`. To ensure pods are not deleted in the future you will need to "
                 "set `is_delete_operator_pod=False` explicitly.",
-                DeprecationWarning,
+                AirflowProviderDeprecationWarning,
                 stacklevel=2,
             )
             is_delete_operator_pod = False
 
         self.cluster_name = cluster_name
         self.in_cluster = in_cluster
         self.namespace = namespace
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/emr.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/emr.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,18 +18,18 @@
 from __future__ import annotations
 
 import ast
 import warnings
 from typing import TYPE_CHECKING, Any, Sequence
 from uuid import uuid4
 
-from airflow.exceptions import AirflowException
+from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
 from airflow.models import BaseOperator
 from airflow.providers.amazon.aws.hooks.emr import EmrContainerHook, EmrHook, EmrServerlessHook
-from airflow.providers.amazon.aws.links.emr import EmrClusterLink
+from airflow.providers.amazon.aws.links.emr import EmrClusterLink, EmrLogsLink, get_log_uri
 from airflow.providers.amazon.aws.utils.waiter import waiter
 from airflow.utils.helpers import exactly_one, prune_dict
 from airflow.utils.types import NOTSET, ArgNotSet
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
@@ -64,15 +64,18 @@
         "cluster_states",
         "steps",
         "execution_role_arn",
     )
     template_ext: Sequence[str] = (".json",)
     template_fields_renderers = {"steps": "json"}
     ui_color = "#f9c915"
-    operator_extra_links = (EmrClusterLink(),)
+    operator_extra_links = (
+        EmrClusterLink(),
+        EmrLogsLink(),
+    )
 
     def __init__(
         self,
         *,
         job_flow_id: str | None = None,
         job_flow_name: str | None = None,
         cluster_states: list[str] | None = None,
@@ -115,14 +118,22 @@
         EmrClusterLink.persist(
             context=context,
             operator=self,
             region_name=emr_hook.conn_region_name,
             aws_partition=emr_hook.conn_partition,
             job_flow_id=job_flow_id,
         )
+        EmrLogsLink.persist(
+            context=context,
+            operator=self,
+            region_name=emr_hook.conn_region_name,
+            aws_partition=emr_hook.conn_partition,
+            job_flow_id=self.job_flow_id,
+            log_uri=get_log_uri(emr_client=emr_hook.conn, job_flow_id=job_flow_id),
+        )
 
         self.log.info("Adding steps to %s", job_flow_id)
 
         # steps may arrive as a string representing a list
         # e.g. if we used XCom or a file then: steps="[{ step1 }, { step2 }]"
         steps = self.steps
         if isinstance(steps, str):
@@ -482,15 +493,15 @@
         self.tags = tags
         self.job_id: str | None = None
 
         if max_tries:
             warnings.warn(
                 f"Parameter `{self.__class__.__name__}.max_tries` is deprecated and will be removed "
                 "in a future release.  Please use method `max_polling_attempts` instead.",
-                DeprecationWarning,
+                AirflowProviderDeprecationWarning,
                 stacklevel=2,
             )
             if max_polling_attempts and max_polling_attempts != max_tries:
                 raise Exception("max_polling_attempts must be the same value as max_tries")
             else:
                 self.max_polling_attempts = max_tries
 
@@ -593,15 +604,18 @@
         "job_flow_overrides",
         "waiter_delay",
         "waiter_max_attempts",
     )
     template_ext: Sequence[str] = (".json",)
     template_fields_renderers = {"job_flow_overrides": "json"}
     ui_color = "#f9c915"
-    operator_extra_links = (EmrClusterLink(),)
+    operator_extra_links = (
+        EmrClusterLink(),
+        EmrLogsLink(),
+    )
 
     def __init__(
         self,
         *,
         aws_conn_id: str = "aws_default",
         emr_conn_id: str | None = "emr_default",
         job_flow_overrides: str | dict[str, Any] | None = None,
@@ -667,14 +681,23 @@
             EmrClusterLink.persist(
                 context=context,
                 operator=self,
                 region_name=self._emr_hook.conn_region_name,
                 aws_partition=self._emr_hook.conn_partition,
                 job_flow_id=self._job_flow_id,
             )
+            if self._job_flow_id:
+                EmrLogsLink.persist(
+                    context=context,
+                    operator=self,
+                    region_name=self._emr_hook.conn_region_name,
+                    aws_partition=self._emr_hook.conn_partition,
+                    job_flow_id=self._job_flow_id,
+                    log_uri=get_log_uri(emr_client=self._emr_hook.conn, job_flow_id=self._job_flow_id),
+                )
 
             if self.wait_for_completion:
                 self._emr_hook.get_waiter("job_flow_waiting").wait(
                     ClusterId=self._job_flow_id,
                     WaiterConfig=prune_dict(
                         {
                             "Delay": self.waiter_delay,
@@ -708,15 +731,18 @@
     :param aws_conn_id: aws connection to uses
     :param do_xcom_push: if True, cluster_id is pushed to XCom with key cluster_id.
     """
 
     template_fields: Sequence[str] = ("cluster_id", "step_concurrency_level")
     template_ext: Sequence[str] = ()
     ui_color = "#f9c915"
-    operator_extra_links = (EmrClusterLink(),)
+    operator_extra_links = (
+        EmrClusterLink(),
+        EmrLogsLink(),
+    )
 
     def __init__(
         self, *, cluster_id: str, step_concurrency_level: int, aws_conn_id: str = "aws_default", **kwargs
     ):
         super().__init__(**kwargs)
         self.aws_conn_id = aws_conn_id
         self.cluster_id = cluster_id
@@ -732,14 +758,22 @@
         EmrClusterLink.persist(
             context=context,
             operator=self,
             region_name=emr_hook.conn_region_name,
             aws_partition=emr_hook.conn_partition,
             job_flow_id=self.cluster_id,
         )
+        EmrLogsLink.persist(
+            context=context,
+            operator=self,
+            region_name=emr_hook.conn_region_name,
+            aws_partition=emr_hook.conn_partition,
+            job_flow_id=self.cluster_id,
+            log_uri=get_log_uri(emr_client=emr_hook.conn, job_flow_id=self.cluster_id),
+        )
 
         self.log.info("Modifying cluster %s", self.cluster_id)
         response = emr.modify_cluster(
             ClusterId=self.cluster_id, StepConcurrencyLevel=self.step_concurrency_level
         )
 
         if response["ResponseMetadata"]["HTTPStatusCode"] != 200:
@@ -760,15 +794,18 @@
     :param job_flow_id: id of the JobFlow to terminate. (templated)
     :param aws_conn_id: aws connection to uses
     """
 
     template_fields: Sequence[str] = ("job_flow_id",)
     template_ext: Sequence[str] = ()
     ui_color = "#f9c915"
-    operator_extra_links = (EmrClusterLink(),)
+    operator_extra_links = (
+        EmrClusterLink(),
+        EmrLogsLink(),
+    )
 
     def __init__(self, *, job_flow_id: str, aws_conn_id: str = "aws_default", **kwargs):
         super().__init__(**kwargs)
         self.job_flow_id = job_flow_id
         self.aws_conn_id = aws_conn_id
 
     def execute(self, context: Context) -> None:
@@ -778,14 +815,22 @@
         EmrClusterLink.persist(
             context=context,
             operator=self,
             region_name=emr_hook.conn_region_name,
             aws_partition=emr_hook.conn_partition,
             job_flow_id=self.job_flow_id,
         )
+        EmrLogsLink.persist(
+            context=context,
+            operator=self,
+            region_name=emr_hook.conn_region_name,
+            aws_partition=emr_hook.conn_partition,
+            job_flow_id=self.job_flow_id,
+            log_uri=get_log_uri(emr_client=emr, job_flow_id=self.job_flow_id),
+        )
 
         self.log.info("Terminating JobFlow %s", self.job_flow_id)
         response = emr.terminate_job_flows(JobFlowIds=[self.job_flow_id])
 
         if not response["ResponseMetadata"]["HTTPStatusCode"] == 200:
             raise AirflowException(f"JobFlow termination failed: {response}")
         else:
@@ -840,15 +885,15 @@
         self.client_request_token = client_request_token or str(uuid4())
 
     @cached_property
     def hook(self) -> EmrServerlessHook:
         """Create and return an EmrServerlessHook."""
         return EmrServerlessHook(aws_conn_id=self.aws_conn_id)
 
-    def execute(self, context: Context):
+    def execute(self, context: Context) -> str | None:
         response = self.hook.conn.create_application(
             clientToken=self.client_request_token,
             releaseLabel=self.release_label,
             type=self.job_type,
             **self.config,
         )
         application_id = response["applicationId"]
@@ -945,24 +990,25 @@
         self.job_driver = job_driver
         self.configuration_overrides = configuration_overrides
         self.wait_for_completion = wait_for_completion
         self.config = config or {}
         self.name = name or self.config.pop("name", f"emr_serverless_job_airflow_{uuid4()}")
         self.waiter_countdown = waiter_countdown
         self.waiter_check_interval_seconds = waiter_check_interval_seconds
+        self.job_id: str | None = None
         super().__init__(**kwargs)
 
         self.client_request_token = client_request_token or str(uuid4())
 
     @cached_property
     def hook(self) -> EmrServerlessHook:
         """Create and return an EmrServerlessHook."""
         return EmrServerlessHook(aws_conn_id=self.aws_conn_id)
 
-    def execute(self, context: Context) -> dict:
+    def execute(self, context: Context) -> str | None:
         self.log.info("Starting job on Application: %s", self.application_id)
 
         app_state = self.hook.conn.get_application(applicationId=self.application_id)["application"]["state"]
         if app_state not in EmrServerlessHook.APPLICATION_SUCCESS_STATES:
             self.hook.conn.start_application(applicationId=self.application_id)
 
             waiter(
@@ -986,32 +1032,64 @@
             name=self.name,
             **self.config,
         )
 
         if response["ResponseMetadata"]["HTTPStatusCode"] != 200:
             raise AirflowException(f"EMR serverless job failed to start: {response}")
 
-        self.log.info("EMR serverless job started: %s", response["jobRunId"])
+        self.job_id = response["jobRunId"]
+        self.log.info("EMR serverless job started: %s", self.job_id)
         if self.wait_for_completion:
             # This should be replaced with a boto waiter when available.
             waiter(
                 get_state_callable=self.hook.conn.get_job_run,
                 get_state_args={
                     "applicationId": self.application_id,
-                    "jobRunId": response["jobRunId"],
+                    "jobRunId": self.job_id,
                 },
                 parse_response=["jobRun", "state"],
                 desired_state=EmrServerlessHook.JOB_SUCCESS_STATES,
                 failure_states=EmrServerlessHook.JOB_FAILURE_STATES,
                 object_type="job",
                 action="run",
                 countdown=self.waiter_countdown,
                 check_interval_seconds=self.waiter_check_interval_seconds,
             )
-        return response["jobRunId"]
+        return self.job_id
+
+    def on_kill(self) -> None:
+        """Cancel the submitted job run"""
+        if self.job_id:
+            self.log.info("Stopping job run with jobId - %s", self.job_id)
+            response = self.hook.conn.cancel_job_run(applicationId=self.application_id, jobRunId=self.job_id)
+            http_status_code = (
+                response.get("ResponseMetadata", {}).get("HTTPStatusCode") if response else None
+            )
+            if http_status_code is None or http_status_code != 200:
+                self.log.error("Unable to request query cancel on EMR Serverless. Exiting")
+                return
+            self.log.info(
+                "Polling EMR Serverless for query with id %s to reach final state",
+                self.job_id,
+            )
+            # This should be replaced with a boto waiter when available.
+            waiter(
+                get_state_callable=self.hook.conn.get_job_run,
+                get_state_args={
+                    "applicationId": self.application_id,
+                    "jobRunId": self.job_id,
+                },
+                parse_response=["jobRun", "state"],
+                desired_state=EmrServerlessHook.JOB_TERMINAL_STATES,
+                failure_states=set(),
+                object_type="job",
+                action="cancelled",
+                countdown=self.waiter_countdown,
+                check_interval_seconds=self.waiter_check_interval_seconds,
+            )
 
 
 class EmrServerlessStopApplicationOperator(BaseOperator):
     """
     Operator to stop an EMR Serverless application
 
     .. seealso::
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/glacier.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/glacier.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/glue.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/glue_crawler.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/glue_crawler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/lambda_function.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/lambda_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/quicksight.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/quicksight.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/rds.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/rds.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/redshift_cluster.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/redshift_cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -294,14 +294,15 @@
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:RedshiftCreateClusterSnapshotOperator`
 
     :param snapshot_identifier: A unique identifier for the snapshot that you are requesting
     :param cluster_identifier: The cluster identifier for which you want a snapshot
     :param retention_period: The number of days that a manual snapshot is retained.
         If the value is -1, the manual snapshot is retained indefinitely.
+    :parma tags: A list of tag instances
     :param wait_for_completion: Whether wait for the cluster snapshot to be in ``available`` state
     :param poll_interval: Time (in seconds) to wait between two consecutive calls to check state
     :param max_attempt: The maximum number of attempts to be made to check the state
     :param aws_conn_id: The Airflow connection used for AWS credentials.
         The default connection id is ``aws_default``
     """
 
@@ -312,24 +313,26 @@
 
     def __init__(
         self,
         *,
         snapshot_identifier: str,
         cluster_identifier: str,
         retention_period: int = -1,
+        tags: list[Any] | None = None,
         wait_for_completion: bool = False,
         poll_interval: int = 15,
         max_attempt: int = 20,
         aws_conn_id: str = "aws_default",
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.snapshot_identifier = snapshot_identifier
         self.cluster_identifier = cluster_identifier
         self.retention_period = retention_period
+        self.tags = tags
         self.wait_for_completion = wait_for_completion
         self.poll_interval = poll_interval
         self.max_attempt = max_attempt
         self.redshift_hook = RedshiftHook(aws_conn_id=aws_conn_id)
 
     def execute(self, context: Context) -> Any:
         cluster_state = self.redshift_hook.cluster_status(cluster_identifier=self.cluster_identifier)
@@ -339,14 +342,15 @@
                 f"Redshift cluster current state is {cluster_state}"
             )
 
         self.redshift_hook.create_cluster_snapshot(
             cluster_identifier=self.cluster_identifier,
             snapshot_identifier=self.snapshot_identifier,
             retention_period=self.retention_period,
+            tags=self.tags,
         )
 
         if self.wait_for_completion:
             self.redshift_hook.get_conn().get_waiter("snapshot_available").wait(
                 ClusterIdentifier=self.cluster_identifier,
                 WaiterConfig={
                     "Delay": self.poll_interval,
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/redshift_data.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/redshift_data.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/s3.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/sagemaker.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/sagemaker.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,18 +20,19 @@
 import time
 import warnings
 from typing import TYPE_CHECKING, Any, Callable, Sequence
 
 from botocore.exceptions import ClientError
 
 from airflow.compat.functools import cached_property
-from airflow.exceptions import AirflowException
+from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
 from airflow.models import BaseOperator
 from airflow.providers.amazon.aws.hooks.base_aws import AwsBaseHook
 from airflow.providers.amazon.aws.hooks.sagemaker import SageMakerHook
+from airflow.providers.amazon.aws.triggers.sagemaker import SageMakerTrigger
 from airflow.providers.amazon.aws.utils import trim_none_values
 from airflow.providers.amazon.aws.utils.sagemaker import ApprovalStatus
 from airflow.providers.amazon.aws.utils.tags import format_tags
 from airflow.utils.json import AirflowJsonEncoder
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
@@ -167,52 +168,60 @@
         For details of the configuration parameter see :py:meth:`SageMaker.Client.create_processing_job`
     :param aws_conn_id: The AWS connection ID to use.
     :param wait_for_completion: If wait is set to True, the time interval, in seconds,
         that the operation waits to check the status of the processing job.
     :param print_log: if the operator should print the cloudwatch log during processing
     :param check_interval: if wait is set to be true, this is the time interval
         in seconds which the operator will check the status of the processing job
+    :param max_attempts: Number of times to poll for query state before returning the current state,
+        defaults to None.
     :param max_ingestion_time: If wait is set to True, the operation fails if the processing job
         doesn't finish within max_ingestion_time seconds. If you set this parameter to None,
         the operation does not timeout.
     :param action_if_job_exists: Behaviour if the job name already exists. Possible options are "timestamp"
         (default), "increment" (deprecated) and "fail".
+    :param deferrable: Run operator in the deferrable mode. This is only effective if wait_for_completion is
+        set to True.
     :return Dict: Returns The ARN of the processing job created in Amazon SageMaker.
     """
 
     def __init__(
         self,
         *,
         config: dict,
         aws_conn_id: str = DEFAULT_CONN_ID,
         wait_for_completion: bool = True,
         print_log: bool = True,
         check_interval: int = CHECK_INTERVAL_SECOND,
+        max_attempts: int | None = None,
         max_ingestion_time: int | None = None,
         action_if_job_exists: str = "timestamp",
+        deferrable: bool = False,
         **kwargs,
     ):
         super().__init__(config=config, aws_conn_id=aws_conn_id, **kwargs)
         if action_if_job_exists not in ("increment", "fail", "timestamp"):
             raise AirflowException(
                 f"Argument action_if_job_exists accepts only 'timestamp', 'increment' and 'fail'. \
                 Provided value: '{action_if_job_exists}'."
             )
         if action_if_job_exists == "increment":
             warnings.warn(
                 "Action 'increment' on job name conflict has been deprecated for performance reasons."
                 "The alternative to 'fail' is now 'timestamp'.",
-                DeprecationWarning,
+                AirflowProviderDeprecationWarning,
                 stacklevel=2,
             )
         self.action_if_job_exists = action_if_job_exists
         self.wait_for_completion = wait_for_completion
         self.print_log = print_log
         self.check_interval = check_interval
+        self.max_attempts = max_attempts or 60
         self.max_ingestion_time = max_ingestion_time
+        self.deferrable = deferrable
 
     def _create_integer_fields(self) -> None:
         """Set fields which should be cast to integers."""
         self.integer_fields: list[list[str] | list[list[str]]] = [
             ["ProcessingResources", "ClusterConfig", "InstanceCount"],
             ["ProcessingResources", "ClusterConfig", "VolumeSizeInGB"],
         ]
@@ -230,22 +239,53 @@
 
         self.config["ProcessingJobName"] = self._get_unique_job_name(
             self.config["ProcessingJobName"],
             self.action_if_job_exists == "fail",
             self.hook.describe_processing_job,
         )
 
+        if self.deferrable and not self.wait_for_completion:
+            self.log.warning(
+                "Setting deferrable to True does not have effect when wait_for_completion is set to False."
+            )
+
+        wait_for_completion = self.wait_for_completion
+        if self.deferrable and self.wait_for_completion:
+            # Set wait_for_completion to False so that it waits for the status in the deferred task.
+            wait_for_completion = False
+
         response = self.hook.create_processing_job(
             self.config,
-            wait_for_completion=self.wait_for_completion,
+            wait_for_completion=wait_for_completion,
             check_interval=self.check_interval,
             max_ingestion_time=self.max_ingestion_time,
         )
         if response["ResponseMetadata"]["HTTPStatusCode"] != 200:
             raise AirflowException(f"Sagemaker Processing Job creation failed: {response}")
+
+        if self.deferrable and self.wait_for_completion:
+            self.defer(
+                timeout=self.execution_timeout,
+                trigger=SageMakerTrigger(
+                    job_name=self.config["ProcessingJobName"],
+                    job_type="Processing",
+                    poke_interval=self.check_interval,
+                    max_attempts=self.max_attempts,
+                    aws_conn_id=self.aws_conn_id,
+                ),
+                method_name="execute_complete",
+            )
+
+        return {"Processing": serialize(self.hook.describe_processing_job(self.config["ProcessingJobName"]))}
+
+    def execute_complete(self, context, event=None):
+        if event["status"] != "success":
+            raise AirflowException(f"Error while running job: {event}")
+        else:
+            self.log.info(event["message"])
         return {"Processing": serialize(self.hook.describe_processing_job(self.config["ProcessingJobName"]))}
 
 
 class SageMakerEndpointConfigOperator(SageMakerBaseOperator):
     """
     Creates an endpoint configuration that Amazon SageMaker hosting
     services uses to deploy models. In the configuration, you identify
@@ -449,14 +489,16 @@
         For details of the configuration parameter of model_config, See:
         :py:meth:`SageMaker.Client.create_model`
 
     :param aws_conn_id: The AWS connection ID to use.
     :param wait_for_completion: Set to True to wait until the transform job finishes.
     :param check_interval: If wait is set to True, the time interval, in seconds,
         that this operation waits to check the status of the transform job.
+    :param max_attempts: Number of times to poll for query state before returning the current state,
+        defaults to None.
     :param max_ingestion_time: If wait is set to True, the operation fails
         if the transform job doesn't finish within max_ingestion_time seconds. If you
         set this parameter to None, the operation does not timeout.
     :param check_if_job_exists: If set to true, then the operator will check whether a transform job
         already exists for the name in the config.
     :param action_if_job_exists: Behaviour if the job name already exists. Possible options are "timestamp"
         (default), "increment" (deprecated) and "fail".
@@ -467,38 +509,42 @@
     def __init__(
         self,
         *,
         config: dict,
         aws_conn_id: str = DEFAULT_CONN_ID,
         wait_for_completion: bool = True,
         check_interval: int = CHECK_INTERVAL_SECOND,
+        max_attempts: int | None = None,
         max_ingestion_time: int | None = None,
         check_if_job_exists: bool = True,
         action_if_job_exists: str = "timestamp",
+        deferrable: bool = False,
         **kwargs,
     ):
         super().__init__(config=config, aws_conn_id=aws_conn_id, **kwargs)
         self.wait_for_completion = wait_for_completion
         self.check_interval = check_interval
+        self.max_attempts = max_attempts or 60
         self.max_ingestion_time = max_ingestion_time
         self.check_if_job_exists = check_if_job_exists
         if action_if_job_exists in ("increment", "fail", "timestamp"):
             if action_if_job_exists == "increment":
                 warnings.warn(
                     "Action 'increment' on job name conflict has been deprecated for performance reasons."
                     "The alternative to 'fail' is now 'timestamp'.",
-                    DeprecationWarning,
+                    AirflowProviderDeprecationWarning,
                     stacklevel=2,
                 )
             self.action_if_job_exists = action_if_job_exists
         else:
             raise AirflowException(
                 f"Argument action_if_job_exists accepts only 'timestamp', 'increment' and 'fail'. \
                 Provided value: '{action_if_job_exists}'."
             )
+        self.deferrable = deferrable
 
     def _create_integer_fields(self) -> None:
         """Set fields which should be cast to integers."""
         self.integer_fields: list[list[str]] = [
             ["Transform", "TransformResources", "InstanceCount"],
             ["Transform", "MaxConcurrentTransforms"],
             ["Transform", "MaxPayloadInMB"],
@@ -529,29 +575,62 @@
 
         model_config = self.config.get("Model")
         if model_config:
             self.log.info("Creating SageMaker Model %s for transform job", model_config["ModelName"])
             self.hook.create_model(model_config)
 
         self.log.info("Creating SageMaker transform Job %s.", transform_config["TransformJobName"])
+
+        if self.deferrable and not self.wait_for_completion:
+            self.log.warning(
+                "Setting deferrable to True does not have effect when wait_for_completion is set to False."
+            )
+
+        wait_for_completion = self.wait_for_completion
+        if self.deferrable and self.wait_for_completion:
+            # Set wait_for_completion to False so that it waits for the status in the deferred task.
+            wait_for_completion = False
+
         response = self.hook.create_transform_job(
             transform_config,
-            wait_for_completion=self.wait_for_completion,
+            wait_for_completion=wait_for_completion,
             check_interval=self.check_interval,
             max_ingestion_time=self.max_ingestion_time,
         )
         if response["ResponseMetadata"]["HTTPStatusCode"] != 200:
             raise AirflowException(f"Sagemaker transform Job creation failed: {response}")
-        else:
-            return {
-                "Model": serialize(self.hook.describe_model(transform_config["ModelName"])),
-                "Transform": serialize(
-                    self.hook.describe_transform_job(transform_config["TransformJobName"])
+
+        if self.deferrable and self.wait_for_completion:
+            self.defer(
+                timeout=self.execution_timeout,
+                trigger=SageMakerTrigger(
+                    job_name=transform_config["TransformJobName"],
+                    job_type="Transform",
+                    poke_interval=self.check_interval,
+                    max_attempts=self.max_attempts,
+                    aws_conn_id=self.aws_conn_id,
                 ),
-            }
+                method_name="execute_complete",
+            )
+
+        return {
+            "Model": serialize(self.hook.describe_model(transform_config["ModelName"])),
+            "Transform": serialize(self.hook.describe_transform_job(transform_config["TransformJobName"])),
+        }
+
+    def execute_complete(self, context, event=None):
+        if event["status"] != "success":
+            raise AirflowException(f"Error while running job: {event}")
+        else:
+            self.log.info(event["message"])
+        transform_config = self.config.get("Transform", self.config)
+        return {
+            "Model": serialize(self.hook.describe_model(transform_config["ModelName"])),
+            "Transform": serialize(self.hook.describe_transform_job(transform_config["TransformJobName"])),
+        }
 
 
 class SageMakerTuningOperator(SageMakerBaseOperator):
     """
     Starts a hyperparameter tuning job. A hyperparameter tuning job finds the
     best version of a model by running many training jobs on your dataset using
     the algorithm you choose and values for hyperparameters within ranges that
@@ -679,58 +758,66 @@
         For details of the configuration parameter see :py:meth:`SageMaker.Client.create_training_job`
     :param aws_conn_id: The AWS connection ID to use.
     :param wait_for_completion: If wait is set to True, the time interval, in seconds,
         that the operation waits to check the status of the training job.
     :param print_log: if the operator should print the cloudwatch log during training
     :param check_interval: if wait is set to be true, this is the time interval
         in seconds which the operator will check the status of the training job
+    :param max_attempts: Number of times to poll for query state before returning the current state,
+        defaults to None.
     :param max_ingestion_time: If wait is set to True, the operation fails if the training job
         doesn't finish within max_ingestion_time seconds. If you set this parameter to None,
         the operation does not timeout.
     :param check_if_job_exists: If set to true, then the operator will check whether a training job
         already exists for the name in the config.
     :param action_if_job_exists: Behaviour if the job name already exists. Possible options are "timestamp"
         (default), "increment" (deprecated) and "fail".
         This is only relevant if check_if_job_exists is True.
+    :param deferrable: Run operator in the deferrable mode. This is only effective if wait_for_completion is
+        set to True.
     :return Dict: Returns The ARN of the training job created in Amazon SageMaker.
     """
 
     def __init__(
         self,
         *,
         config: dict,
         aws_conn_id: str = DEFAULT_CONN_ID,
         wait_for_completion: bool = True,
         print_log: bool = True,
         check_interval: int = CHECK_INTERVAL_SECOND,
+        max_attempts: int | None = None,
         max_ingestion_time: int | None = None,
         check_if_job_exists: bool = True,
         action_if_job_exists: str = "timestamp",
+        deferrable: bool = False,
         **kwargs,
     ):
         super().__init__(config=config, aws_conn_id=aws_conn_id, **kwargs)
         self.wait_for_completion = wait_for_completion
         self.print_log = print_log
         self.check_interval = check_interval
+        self.max_attempts = max_attempts or 60
         self.max_ingestion_time = max_ingestion_time
         self.check_if_job_exists = check_if_job_exists
         if action_if_job_exists in {"timestamp", "increment", "fail"}:
             if action_if_job_exists == "increment":
                 warnings.warn(
                     "Action 'increment' on job name conflict has been deprecated for performance reasons."
                     "The alternative to 'fail' is now 'timestamp'.",
-                    DeprecationWarning,
+                    AirflowProviderDeprecationWarning,
                     stacklevel=2,
                 )
             self.action_if_job_exists = action_if_job_exists
         else:
             raise AirflowException(
                 f"Argument action_if_job_exists accepts only 'timestamp', 'increment' and 'fail'. \
                 Provided value: '{action_if_job_exists}'."
             )
+        self.deferrable = deferrable
 
     def expand_role(self) -> None:
         """Expands an IAM role name into an ARN."""
         if "RoleArn" in self.config:
             hook = AwsBaseHook(self.aws_conn_id, client_type="iam")
             self.config["RoleArn"] = hook.expand_role(self.config["RoleArn"])
 
@@ -749,25 +836,58 @@
             self.config["TrainingJobName"] = self._get_unique_job_name(
                 self.config["TrainingJobName"],
                 self.action_if_job_exists == "fail",
                 self.hook.describe_training_job,
             )
 
         self.log.info("Creating SageMaker training job %s.", self.config["TrainingJobName"])
+
+        if self.deferrable and not self.wait_for_completion:
+            self.log.warning(
+                "Setting deferrable to True does not have effect when wait_for_completion is set to False."
+            )
+
+        wait_for_completion = self.wait_for_completion
+        if self.deferrable and self.wait_for_completion:
+            # Set wait_for_completion to False so that it waits for the status in the deferred task.
+            wait_for_completion = False
+
         response = self.hook.create_training_job(
             self.config,
-            wait_for_completion=self.wait_for_completion,
+            wait_for_completion=wait_for_completion,
             print_log=self.print_log,
             check_interval=self.check_interval,
             max_ingestion_time=self.max_ingestion_time,
         )
         if response["ResponseMetadata"]["HTTPStatusCode"] != 200:
             raise AirflowException(f"Sagemaker Training Job creation failed: {response}")
+
+        if self.deferrable and self.wait_for_completion:
+            self.defer(
+                timeout=self.execution_timeout,
+                trigger=SageMakerTrigger(
+                    job_name=self.config["TrainingJobName"],
+                    job_type="Training",
+                    poke_interval=self.check_interval,
+                    max_attempts=self.max_attempts,
+                    aws_conn_id=self.aws_conn_id,
+                ),
+                method_name="execute_complete",
+            )
+
+        result = {"Training": serialize(self.hook.describe_training_job(self.config["TrainingJobName"]))}
+        return result
+
+    def execute_complete(self, context, event=None):
+        if event["status"] != "success":
+            raise AirflowException(f"Error while running job: {event}")
         else:
-            return {"Training": serialize(self.hook.describe_training_job(self.config["TrainingJobName"]))}
+            self.log.info(event["message"])
+        result = {"Training": serialize(self.hook.describe_training_job(self.config["TrainingJobName"]))}
+        return result
 
 
 class SageMakerDeleteModelOperator(SageMakerBaseOperator):
     """
     Deletes a SageMaker model.
 
     .. seealso::
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/sns.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/sns.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/sqs.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/sqs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/step_function.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/step_function.py`

 * *Files 12% similar despite different names*

```diff
@@ -109,12 +109,16 @@
         self.aws_conn_id = aws_conn_id
         self.region_name = region_name
 
     def execute(self, context: Context):
         hook = StepFunctionHook(aws_conn_id=self.aws_conn_id, region_name=self.region_name)
 
         execution_status = hook.describe_execution(self.execution_arn)
-        execution_output = json.loads(execution_status["output"]) if "output" in execution_status else None
+        response = None
+        if "output" in execution_status:
+            response = json.loads(execution_status["output"])
+        elif "error" in execution_status:
+            response = json.loads(execution_status["error"])
 
         self.log.info("Got State Machine Execution output for %s", self.execution_arn)
 
-        return execution_output
+        return response
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/secrets/__init__.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/secrets/secrets_manager.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/secrets/secrets_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import json
 import re
 import warnings
 from typing import Any
 from urllib.parse import unquote
 
 from airflow.compat.functools import cached_property
+from airflow.exceptions import AirflowProviderDeprecationWarning
 from airflow.providers.amazon.aws.utils import trim_none_values
 from airflow.secrets import BaseSecretsBackend
 from airflow.utils.log.logging_mixin import LoggingMixin
 
 
 class SecretsManagerBackend(BaseSecretsBackend, LoggingMixin):
     """
@@ -145,25 +146,25 @@
         self.sep = sep
 
         if kwargs.pop("full_url_mode", None) is not None:
             warnings.warn(
                 "The `full_url_mode` kwarg is deprecated. Going forward, the `SecretsManagerBackend`"
                 " will support both URL-encoded and JSON-encoded secrets at the same time. The encoding"
                 " of the secret will be determined automatically.",
-                DeprecationWarning,
+                AirflowProviderDeprecationWarning,
                 stacklevel=2,
             )
 
         if kwargs.get("are_secret_values_urlencoded") is not None:
             warnings.warn(
                 "The `secret_values_are_urlencoded` is deprecated. This kwarg only exists to assist in"
                 " migrating away from URL-encoding secret values for JSON secrets."
                 " To remove this warning, make sure your JSON secrets are *NOT* URL-encoded, and then"
                 " remove this kwarg from backend_kwargs.",
-                DeprecationWarning,
+                AirflowProviderDeprecationWarning,
                 stacklevel=2,
             )
             self.are_secret_values_urlencoded = kwargs.pop("are_secret_values_urlencoded", None)
         else:
             self.are_secret_values_urlencoded = False
 
         self.extra_conn_words = extra_conn_words or {}
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/secrets/systems_manager.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/secrets/systems_manager.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/__init__.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/athena.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/athena.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/batch.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/batch.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/cloud_formation.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/cloud_formation.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/dms.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/dms.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/dynamodb.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/dynamodb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/ec2.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/ec2.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,18 +13,20 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Sequence
+from typing import TYPE_CHECKING, Any, Sequence
 
 from airflow.compat.functools import cached_property
+from airflow.exceptions import AirflowException
 from airflow.providers.amazon.aws.hooks.ec2 import EC2Hook
+from airflow.providers.amazon.aws.triggers.ec2 import EC2StateSensorTrigger
 from airflow.sensors.base import BaseSensorOperator
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class EC2InstanceStateSensor(BaseSensorOperator):
@@ -35,39 +37,62 @@
     .. seealso::
         For more information on how to use this sensor, take a look at the guide:
         :ref:`howto/sensor:EC2InstanceStateSensor`
 
     :param target_state: target state of instance
     :param instance_id: id of the AWS EC2 instance
     :param region_name: (optional) aws region name associated with the client
+    :param deferrable: if True, the sensor will run in deferrable mode
     """
 
     template_fields: Sequence[str] = ("target_state", "instance_id", "region_name")
     ui_color = "#cc8811"
     ui_fgcolor = "#ffffff"
     valid_states = ["running", "stopped", "terminated"]
 
     def __init__(
         self,
         *,
         target_state: str,
         instance_id: str,
         aws_conn_id: str = "aws_default",
         region_name: str | None = None,
+        deferrable: bool = False,
         **kwargs,
     ):
         if target_state not in self.valid_states:
             raise ValueError(f"Invalid target_state: {target_state}")
         super().__init__(**kwargs)
         self.target_state = target_state
         self.instance_id = instance_id
         self.aws_conn_id = aws_conn_id
         self.region_name = region_name
+        self.deferrable = deferrable
+
+    def execute(self, context: Context) -> Any:
+        if self.deferrable:
+            self.defer(
+                trigger=EC2StateSensorTrigger(
+                    instance_id=self.instance_id,
+                    target_state=self.target_state,
+                    aws_conn_id=self.aws_conn_id,
+                    region_name=self.region_name,
+                    poll_interval=int(self.poke_interval),
+                ),
+                method_name="execute_complete",
+            )
+        else:
+            super().execute(context=context)
 
     @cached_property
     def hook(self):
         return EC2Hook(aws_conn_id=self.aws_conn_id, region_name=self.region_name)
 
     def poke(self, context: Context):
         instance_state = self.hook.get_instance_state(instance_id=self.instance_id)
         self.log.info("instance state: %s", instance_state)
         return instance_state == self.target_state
+
+    def execute_complete(self, context, event=None):
+        if event["status"] != "success":
+            raise AirflowException(f"Error: {event}")
+        return
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/ecs.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/ecs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/eks.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/eks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/emr.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/emr.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,16 +19,15 @@
 
 from typing import TYPE_CHECKING, Any, Iterable, Sequence
 
 from deprecated import deprecated
 
 from airflow.exceptions import AirflowException
 from airflow.providers.amazon.aws.hooks.emr import EmrContainerHook, EmrHook, EmrServerlessHook
-from airflow.providers.amazon.aws.hooks.s3 import S3Hook
-from airflow.providers.amazon.aws.links.emr import EmrLogsLink
+from airflow.providers.amazon.aws.links.emr import EmrClusterLink, EmrLogsLink, get_log_uri
 from airflow.sensors.base import BaseSensorOperator
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 from airflow.compat.functools import cached_property
 
@@ -381,15 +380,18 @@
         job flow reaches any of these states
     :param failed_states: the failure states, sensor fails when
         job flow reaches any of these states
     """
 
     template_fields: Sequence[str] = ("job_flow_id", "target_states", "failed_states")
     template_ext: Sequence[str] = ()
-    operator_extra_links = (EmrLogsLink(),)
+    operator_extra_links = (
+        EmrClusterLink(),
+        EmrLogsLink(),
+    )
 
     def __init__(
         self,
         *,
         job_flow_id: str,
         target_states: Iterable[str] | None = None,
         failed_states: Iterable[str] | None = None,
@@ -408,22 +410,29 @@
             https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.describe_cluster
 
         :return: response
         """
         emr_client = self.hook.conn
         self.log.info("Poking cluster %s", self.job_flow_id)
         response = emr_client.describe_cluster(ClusterId=self.job_flow_id)
-        log_uri = S3Hook.parse_s3_url(response["Cluster"]["LogUri"])
+
+        EmrClusterLink.persist(
+            context=context,
+            operator=self,
+            region_name=self.hook.conn_region_name,
+            aws_partition=self.hook.conn_partition,
+            job_flow_id=self.job_flow_id,
+        )
         EmrLogsLink.persist(
             context=context,
             operator=self,
             region_name=self.hook.conn_region_name,
             aws_partition=self.hook.conn_partition,
             job_flow_id=self.job_flow_id,
-            log_uri="/".join(log_uri),
+            log_uri=get_log_uri(cluster=response),
         )
         return response
 
     @staticmethod
     def state_from_response(response: dict[str, Any]) -> str:
         """
         Get state from response dictionary.
@@ -468,14 +477,18 @@
         step reaches any of these states
     :param failed_states: the failure states, sensor fails when
         step reaches any of these states
     """
 
     template_fields: Sequence[str] = ("job_flow_id", "step_id", "target_states", "failed_states")
     template_ext: Sequence[str] = ()
+    operator_extra_links = (
+        EmrClusterLink(),
+        EmrLogsLink(),
+    )
 
     def __init__(
         self,
         *,
         job_flow_id: str,
         step_id: str,
         target_states: Iterable[str] | None = None,
@@ -496,15 +509,33 @@
             https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.describe_step
 
         :return: response
         """
         emr_client = self.hook.conn
 
         self.log.info("Poking step %s on cluster %s", self.step_id, self.job_flow_id)
-        return emr_client.describe_step(ClusterId=self.job_flow_id, StepId=self.step_id)
+        response = emr_client.describe_step(ClusterId=self.job_flow_id, StepId=self.step_id)
+
+        EmrClusterLink.persist(
+            context=context,
+            operator=self,
+            region_name=self.hook.conn_region_name,
+            aws_partition=self.hook.conn_partition,
+            job_flow_id=self.job_flow_id,
+        )
+        EmrLogsLink.persist(
+            context=context,
+            operator=self,
+            region_name=self.hook.conn_region_name,
+            aws_partition=self.hook.conn_partition,
+            job_flow_id=self.job_flow_id,
+            log_uri=get_log_uri(emr_client=emr_client, job_flow_id=self.job_flow_id),
+        )
+
+        return response
 
     @staticmethod
     def state_from_response(response: dict[str, Any]) -> str:
         """
         Get state from response dictionary.
 
         :param response: response from AWS API
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/glacier.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/glacier.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/glue.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/glue.py`

 * *Files 9% similar despite different names*

```diff
@@ -56,37 +56,34 @@
         super().__init__(**kwargs)
         self.job_name = job_name
         self.run_id = run_id
         self.verbose = verbose
         self.aws_conn_id = aws_conn_id
         self.success_states: list[str] = ["SUCCEEDED"]
         self.errored_states: list[str] = ["FAILED", "STOPPED", "TIMEOUT"]
-        self.next_log_token: str | None = None
+        self.next_log_tokens = GlueJobHook.LogContinuationTokens()
 
     @cached_property
     def hook(self):
         return GlueJobHook(aws_conn_id=self.aws_conn_id)
 
     def poke(self, context: Context):
         self.log.info("Poking for job run status :for Glue Job %s and ID %s", self.job_name, self.run_id)
         job_state = self.hook.get_job_state(job_name=self.job_name, run_id=self.run_id)
-        job_failed = False
 
         try:
             if job_state in self.success_states:
                 self.log.info("Exiting Job %s Run State: %s", self.run_id, job_state)
                 return True
             elif job_state in self.errored_states:
-                job_failed = True
                 job_error_message = "Exiting Job %s Run State: %s", self.run_id, job_state
                 self.log.info(job_error_message)
                 raise AirflowException(job_error_message)
             else:
                 return False
         finally:
             if self.verbose:
-                self.next_log_token = self.hook.print_job_logs(
+                self.hook.print_job_logs(
                     job_name=self.job_name,
                     run_id=self.run_id,
-                    job_failed=job_failed,
-                    next_token=self.next_log_token,
+                    continuation_tokens=self.next_log_tokens,
                 )
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/glue_crawler.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/glue_crawler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/lambda_function.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/lambda_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/quicksight.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/quicksight.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/rds.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/rds.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/redshift_cluster.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/s3.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/sagemaker.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/sagemaker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/sqs.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/sqs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/step_function.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/step_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/__init__.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/waiters/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/base.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 # under the License.
 """This module contains base AWS to AWS transfer operator"""
 from __future__ import annotations
 
 import warnings
 from typing import Sequence
 
+from airflow.exceptions import AirflowProviderDeprecationWarning
 from airflow.models import BaseOperator
 from airflow.providers.amazon.aws.hooks.base_aws import AwsBaseHook
 from airflow.utils.types import NOTSET, ArgNotSet
 
 _DEPRECATION_MSG = (
     "The aws_conn_id parameter has been deprecated. Use the source_aws_conn_id parameter instead."
 )
@@ -56,14 +57,14 @@
         source_aws_conn_id: str | None = AwsBaseHook.default_conn_name,
         dest_aws_conn_id: str | None | ArgNotSet = NOTSET,
         aws_conn_id: str | None | ArgNotSet = NOTSET,
         **kwargs,
     ) -> None:
         super().__init__(**kwargs)
         if not isinstance(aws_conn_id, ArgNotSet):
-            warnings.warn(_DEPRECATION_MSG, DeprecationWarning, stacklevel=3)
+            warnings.warn(_DEPRECATION_MSG, AirflowProviderDeprecationWarning, stacklevel=3)
             self.source_aws_conn_id = aws_conn_id
         else:
             self.source_aws_conn_id = source_aws_conn_id
         self.dest_aws_conn_id = (
             self.source_aws_conn_id if isinstance(dest_aws_conn_id, ArgNotSet) else dest_aws_conn_id
         )
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py`

 * *Files 23% similar despite different names*

```diff
@@ -19,20 +19,22 @@
 This module contains operators to replicate records from
 DynamoDB table to S3.
 """
 from __future__ import annotations
 
 import json
 from copy import copy
+from datetime import datetime
 from decimal import Decimal
 from os.path import getsize
 from tempfile import NamedTemporaryFile
 from typing import IO, TYPE_CHECKING, Any, Callable, Sequence
 from uuid import uuid4
 
+from airflow.compat.functools import cached_property
 from airflow.providers.amazon.aws.hooks.base_aws import AwsBaseHook
 from airflow.providers.amazon.aws.hooks.dynamodb import DynamoDBHook
 from airflow.providers.amazon.aws.hooks.s3 import S3Hook
 from airflow.providers.amazon.aws.transfers.base import AwsToAwsBaseOperator
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
@@ -83,14 +85,18 @@
 
     :param dynamodb_table_name: Dynamodb table to replicate data from
     :param s3_bucket_name: S3 bucket to replicate data to
     :param file_size: Flush file to s3 if file size >= file_size
     :param dynamodb_scan_kwargs: kwargs pass to <https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.scan>
     :param s3_key_prefix: Prefix of s3 object key
     :param process_func: How we transforms a dynamodb item to bytes. By default we dump the json
+    :param export_time: Time in the past from which to export table data, counted in seconds from the start of
+     the Unix epoch. The table export will be a snapshot of the table's state at this point in time.
+    :param export_format: The format for the exported data. Valid values for ExportFormat are DYNAMODB_JSON
+     or ION.
     """
 
     template_fields: Sequence[str] = (
         *AwsToAwsBaseOperator.template_fields,
         "s3_bucket_name",
         "s3_key_prefix",
         "dynamodb_table_name",
@@ -105,28 +111,63 @@
         *,
         dynamodb_table_name: str,
         s3_bucket_name: str,
         file_size: int,
         dynamodb_scan_kwargs: dict[str, Any] | None = None,
         s3_key_prefix: str = "",
         process_func: Callable[[dict[str, Any]], bytes] = _convert_item_to_json_bytes,
+        export_time: datetime | None = None,
+        export_format: str = "DYNAMODB_JSON",
         **kwargs,
     ) -> None:
         super().__init__(**kwargs)
         self.file_size = file_size
         self.process_func = process_func
         self.dynamodb_table_name = dynamodb_table_name
         self.dynamodb_scan_kwargs = dynamodb_scan_kwargs
         self.s3_bucket_name = s3_bucket_name
         self.s3_key_prefix = s3_key_prefix
+        self.export_time = export_time
+        self.export_format = export_format
 
-    def execute(self, context: Context) -> None:
-        hook = DynamoDBHook(aws_conn_id=self.source_aws_conn_id)
-        table = hook.get_conn().Table(self.dynamodb_table_name)
+        if self.export_time and self.export_time > datetime.now():
+            raise ValueError("The export_time parameter cannot be a future time.")
+
+    @cached_property
+    def hook(self):
+        """Create DynamoDBHook"""
+        return DynamoDBHook(aws_conn_id=self.source_aws_conn_id)
 
+    def execute(self, context: Context) -> None:
+        if self.export_time:
+            self._export_table_to_point_in_time()
+        else:
+            self._export_entire_data()
+
+    def _export_table_to_point_in_time(self):
+        """
+        Export data from start of epoc till `export_time`. Table export will be a snapshot of the table's
+         state at this point in time.
+        """
+        client = self.hook.conn.meta.client
+        table_description = client.describe_table(TableName=self.dynamodb_table_name)
+        response = client.export_table_to_point_in_time(
+            TableArn=table_description.get("Table", {}).get("TableArn"),
+            ExportTime=self.export_time,
+            S3Bucket=self.s3_bucket_name,
+            S3Prefix=self.s3_key_prefix,
+            ExportFormat=self.export_format,
+        )
+        waiter = self.hook.get_waiter("export_table")
+        export_arn = response.get("ExportDescription", {}).get("ExportArn")
+        waiter.wait(ExportArn=export_arn)
+
+    def _export_entire_data(self):
+        """Export all data from the table."""
+        table = self.hook.get_conn().Table(self.dynamodb_table_name)
         scan_kwargs = copy(self.dynamodb_scan_kwargs) if self.dynamodb_scan_kwargs else {}
         err = None
         f: IO[Any]
         with NamedTemporaryFile() as f:
             try:
                 f = self._scan_dynamodb_and_upload_to_s3(f, scan_kwargs, table)
             except Exception as e:
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/exasol_to_s3.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/exasol_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/ftp_to_s3.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/ftp_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/gcs_to_s3.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/gcs_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/google_api_to_s3.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/google_api_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/local_to_s3.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/local_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/mongo_to_s3.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/mongo_to_s3.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 # under the License.
 from __future__ import annotations
 
 import json
 from typing import TYPE_CHECKING, Any, Iterable, Sequence, cast
 
 from bson import json_util
+from pymongo.command_cursor import CommandCursor
+from pymongo.cursor import Cursor
 
 from airflow.models import BaseOperator
 from airflow.providers.amazon.aws.hooks.s3 import S3Hook
 from airflow.providers.mongo.hooks.mongo import MongoHook
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
@@ -92,27 +94,28 @@
 
     def execute(self, context: Context):
         """Is written to depend on transform method"""
         s3_conn = S3Hook(self.aws_conn_id)
 
         # Grab collection and execute query according to whether or not it is a pipeline
         if self.is_pipeline:
-            results = MongoHook(self.mongo_conn_id).aggregate(
+            results: CommandCursor[Any] | Cursor = MongoHook(self.mongo_conn_id).aggregate(
                 mongo_collection=self.mongo_collection,
                 aggregate_query=cast(list, self.mongo_query),
                 mongo_db=self.mongo_db,
                 allowDiskUse=self.allow_disk_use,
             )
 
         else:
             results = MongoHook(self.mongo_conn_id).find(
                 mongo_collection=self.mongo_collection,
                 query=cast(dict, self.mongo_query),
                 projection=self.mongo_projection,
                 mongo_db=self.mongo_db,
+                find_one=False,
             )
 
         # Performs transform then stringifies the docs results into json format
         docs_str = self._stringify(self.transform(results))
 
         s3_conn.load_string(
             string_data=docs_str,
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/redshift_to_s3.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/redshift_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/s3_to_ftp.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/s3_to_ftp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/s3_to_redshift.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/s3_to_redshift.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,14 +72,15 @@
         "s3_bucket",
         "s3_key",
         "schema",
         "table",
         "column_list",
         "copy_options",
         "redshift_conn_id",
+        "method",
     )
     template_ext: Sequence[str] = ()
     ui_color = "#99e699"
 
     def __init__(
         self,
         *,
@@ -109,17 +110,14 @@
         self.column_list = column_list
         self.copy_options = copy_options or []
         self.autocommit = autocommit
         self.method = method
         self.upsert_keys = upsert_keys
         self.redshift_data_api_kwargs = redshift_data_api_kwargs
 
-        if self.method not in AVAILABLE_METHODS:
-            raise AirflowException(f"Method not found! Available methods: {AVAILABLE_METHODS}")
-
         if self.redshift_data_api_kwargs:
             for arg in ["sql", "parameters"]:
                 if arg in self.redshift_data_api_kwargs.keys():
                     raise AirflowException(f"Cannot include param '{arg}' in Redshift Data API kwargs")
 
     def _build_copy_query(self, copy_destination: str, credentials_block: str, copy_options: str) -> str:
         column_names = "(" + ", ".join(self.column_list) + ")" if self.column_list else ""
@@ -128,14 +126,17 @@
                     FROM 's3://{self.s3_bucket}/{self.s3_key}'
                     credentials
                     '{credentials_block}'
                     {copy_options};
         """
 
     def execute(self, context: Context) -> None:
+        if self.method not in AVAILABLE_METHODS:
+            raise AirflowException(f"Method not found! Available methods: {AVAILABLE_METHODS}")
+
         redshift_hook: RedshiftDataHook | RedshiftSQLHook
         if self.redshift_data_api_kwargs:
             redshift_hook = RedshiftDataHook(aws_conn_id=self.redshift_conn_id)
         else:
             redshift_hook = RedshiftSQLHook(redshift_conn_id=self.redshift_conn_id)
         conn = S3Hook.get_connection(conn_id=self.aws_conn_id)
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/s3_to_sftp.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/s3_to_sftp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/s3_to_sql.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/s3_to_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/sftp_to_s3.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/sftp_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/sql_to_s3.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/sql_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/triggers/__init__.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/triggers/redshift_cluster.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/triggers/redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/utils/__init__.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/utils/connection_wrapper.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/utils/connection_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from copy import deepcopy
 from dataclasses import MISSING, InitVar, dataclass, field, fields
 from typing import TYPE_CHECKING, Any
 
 from botocore.config import Config
 
 from airflow.compat.functools import cached_property
-from airflow.exceptions import AirflowException
+from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
 from airflow.providers.amazon.aws.utils import trim_none_values
 from airflow.utils.log.logging_mixin import LoggingMixin
 from airflow.utils.log.secrets_masker import mask_secret
 from airflow.utils.types import NOTSET, ArgNotSet
 
 if TYPE_CHECKING:
     from airflow.models.connection import Connection  # Avoid circular imports.
@@ -164,15 +164,15 @@
         self.extra_config = deepcopy(conn.extra_dejson)
 
         if self.conn_type.lower() == "s3":
             warnings.warn(
                 f"{self.conn_repr} has connection type 's3', "
                 "which has been replaced by connection type 'aws'. "
                 "Please update your connection to have `conn_type='aws'`.",
-                DeprecationWarning,
+                AirflowProviderDeprecationWarning,
                 stacklevel=2,
             )
         elif self.conn_type != "aws":
             warnings.warn(
                 f"{self.conn_repr} expected connection type 'aws', got {self.conn_type!r}. "
                 "This connection might not work correctly. "
                 "Please use Amazon Web Services Connection type.",
@@ -182,15 +182,15 @@
 
         extra = deepcopy(conn.extra_dejson)
         session_kwargs = extra.get("session_kwargs", {})
         if session_kwargs:
             warnings.warn(
                 "'session_kwargs' in extra config is deprecated and will be removed in a future releases. "
                 f"Please specify arguments passed to boto3 Session directly in {self.conn_repr} extra.",
-                DeprecationWarning,
+                AirflowProviderDeprecationWarning,
                 stacklevel=2,
             )
 
         # Retrieve initial connection credentials
         init_credentials = self._get_credentials(**extra)
         self.aws_access_key_id, self.aws_secret_access_key, self.aws_session_token = init_credentials
 
@@ -238,24 +238,24 @@
             self.log.debug("Retrieving botocore config=%s from %s extra.", config_kwargs, self.conn_repr)
             self.botocore_config = Config(**config_kwargs)
 
         if conn.host:
             warnings.warn(
                 f"Host {conn.host} specified in the connection is not used."
                 " Please, set it on extra['endpoint_url'] instead",
-                DeprecationWarning,
+                AirflowProviderDeprecationWarning,
                 stacklevel=2,
             )
 
         self.endpoint_url = extra.get("host")
         if self.endpoint_url:
             warnings.warn(
                 "extra['host'] is deprecated and will be removed in a future release."
                 " Please set extra['endpoint_url'] instead",
-                DeprecationWarning,
+                AirflowProviderDeprecationWarning,
                 stacklevel=2,
             )
         else:
             self.endpoint_url = extra.get("endpoint_url")
 
         # Retrieve Assume Role Configuration
         assume_role_configs = self._get_assume_role_configs(**extra)
@@ -381,15 +381,15 @@
         if role_arn:
             self.log.debug("Retrieving role_arn=%r from %s extra.", role_arn, self.conn_repr)
         elif aws_account_id and aws_iam_role:
             warnings.warn(
                 "Constructing 'role_arn' from extra['aws_account_id'] and extra['aws_iam_role'] is deprecated"
                 f" and will be removed in a future releases."
                 f" Please set 'role_arn' in {self.conn_repr} extra.",
-                DeprecationWarning,
+                AirflowProviderDeprecationWarning,
                 stacklevel=3,
             )
             role_arn = f"arn:aws:iam::{aws_account_id}:role/{aws_iam_role}"
             self.log.debug(
                 "Constructions role_arn=%r from %s extra['aws_account_id'] and extra['aws_iam_role'].",
                 role_arn,
                 self.conn_repr,
@@ -409,15 +409,15 @@
         self.log.debug("Retrieve assume_role_method=%r from %s.", assume_role_method, self.conn_repr)
 
         assume_role_kwargs = assume_role_kwargs or {}
         if "ExternalId" not in assume_role_kwargs and external_id:
             warnings.warn(
                 "'external_id' in extra config is deprecated and will be removed in a future releases. "
                 f"Please set 'ExternalId' in 'assume_role_kwargs' in {self.conn_repr} extra.",
-                DeprecationWarning,
+                AirflowProviderDeprecationWarning,
                 stacklevel=3,
             )
             assume_role_kwargs["ExternalId"] = external_id
 
         return role_arn, assume_role_method, assume_role_kwargs
 
 
@@ -432,15 +432,15 @@
     :param config_format: config type. One of "boto", "s3cmd" or "aws".
         Defaults to "boto"
     :param profile: profile name in AWS type config file
     """
     warnings.warn(
         "Use local credentials file is never documented and well tested. "
         "Obtain credentials by this way deprecated and will be removed in a future releases.",
-        DeprecationWarning,
+        AirflowProviderDeprecationWarning,
         stacklevel=4,
     )
 
     import configparser
 
     config = configparser.ConfigParser()
     try:
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/utils/eks_get_token.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/utils/eks_get_token.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/utils/emailer.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/utils/emailer.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/utils/rds.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/utils/rds.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/utils/redshift.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/utils/redshift.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/utils/sagemaker.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/utils/sagemaker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/utils/waiter.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/utils/waiter.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/waiters/appflow.json` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/waiters/appflow.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/waiters/base_waiter.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/waiters/base_waiter.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/waiters/ecs.json` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/waiters/ecs.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/waiters/eks.json` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/waiters/eks.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/waiters/emr.json` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/waiters/emr.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/get_provider_info.py` & `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/get_provider_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-amazon",
         "name": "Amazon",
         "description": "Amazon integration (including `Amazon Web Services (AWS) <https://aws.amazon.com/>`__).\n",
         "suspended": False,
         "versions": [
+            "8.1.0",
             "8.0.0",
             "7.4.1",
             "7.4.0",
             "7.3.0",
             "7.2.1",
             "7.2.0",
             "7.1.0",
@@ -59,25 +60,26 @@
             "1.4.0",
             "1.3.0",
             "1.2.0",
             "1.1.0",
             "1.0.0",
         ],
         "dependencies": [
-            "apache-airflow>=2.3.0",
+            "apache-airflow>=2.4.0",
             "apache-airflow-providers-common-sql>=1.3.1",
             "boto3>=1.24.0",
             "asgiref",
             "watchtower~=2.0.1",
             "jsonpath_ng>=1.5.3",
             "redshift_connector>=2.0.888",
             "sqlalchemy_redshift>=0.8.6",
             "mypy-boto3-rds>=1.24.0",
             "mypy-boto3-redshift-data>=1.24.0",
             "mypy-boto3-appflow>=1.24.0",
+            "mypy-boto3-s3>=1.24.0",
         ],
         "integrations": [
             {
                 "integration-name": "Amazon Athena",
                 "external-doc-url": "https://aws.amazon.com/athena/",
                 "logo": "/integration-logos/aws/Amazon-Athena_light-bg@4x.png",
                 "how-to-guide": ["/docs/apache-airflow-providers-amazon/operators/athena.rst"],
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/apache_airflow_providers_amazon.egg-info/PKG-INFO` & `apache-airflow-providers-amazon-8.1.0rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,52 +1,7 @@
-Metadata-Version: 2.1
-Name: apache-airflow-providers-amazon
-Version: 8.0.0rc3
-Summary: Provider for Apache Airflow. Implements apache-airflow-providers-amazon package
-Home-page: https://airflow.apache.org/
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Author: Apache Software Foundation
-Author-email: dev@airflow.apache.org
-License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.0.0/
-Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
-Project-URL: Source Code, https://github.com/apache/airflow
-Project-URL: Slack Chat, https://s.apache.org/airflow-slack
-Project-URL: Twitter, https://twitter.com/ApacheAirflow
-Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: System Administrators
-Classifier: Framework :: Apache Airflow
-Classifier: Framework :: Apache Airflow :: Provider
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: System :: Monitoring
-Requires-Python: ~=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: apache.hive
-Provides-Extra: cncf.kubernetes
-Provides-Extra: common.sql
-Provides-Extra: exasol
-Provides-Extra: ftp
-Provides-Extra: google
-Provides-Extra: imap
-Provides-Extra: mongo
-Provides-Extra: salesforce
-Provides-Extra: ssh
-Provides-Extra: pandas
-Provides-Extra: aiobotocore
-License-File: LICENSE
-License-File: NOTICE
-
 
 .. Licensed to the Apache Software Foundation (ASF) under one
    or more contributor license agreements.  See the NOTICE file
    distributed with this work for additional information
    regarding copyright ownership.  The ASF licenses this file
    to you under the Apache License, Version 2.0 (the
    "License"); you may not use this file except in compliance
@@ -60,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-amazon``
 
-Release: ``8.0.0rc3``
+Release: ``8.1.0rc1``
 
 
 Amazon integration (including `Amazon Web Services (AWS) <https://aws.amazon.com/>`__).
 
 
 Provider package
 ----------------
 
 This is a provider package for ``amazon`` provider. All classes for this provider package
 are in ``airflow.providers.amazon`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.0.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.1.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -91,25 +46,26 @@
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
-``apache-airflow``                       ``>=2.3.0``
+``apache-airflow``                       ``>=2.4.0``
 ``apache-airflow-providers-common-sql``  ``>=1.3.1``
 ``boto3``                                ``>=1.24.0``
 ``asgiref``
 ``watchtower``                           ``~=2.0.1``
 ``jsonpath_ng``                          ``>=1.5.3``
 ``redshift_connector``                   ``>=2.0.888``
 ``sqlalchemy_redshift``                  ``>=0.8.6``
 ``mypy-boto3-rds``                       ``>=1.24.0``
 ``mypy-boto3-redshift-data``             ``>=1.24.0``
 ``mypy-boto3-appflow``                   ``>=1.24.0``
+``mypy-boto3-s3``                        ``>=1.24.0``
 =======================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
 Those are dependencies that might be needed in order to use all the features of the package.
 You need to install the specified provider packages in order to use them.
@@ -158,14 +114,62 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+8.1.0
+.....
+
+.. note::
+  This release of provider is only available for Airflow 2.4+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
+
+Features
+~~~~~~~~
+
+* ``DynamoDBToS3Operator - Add a feature to export the table to a point in time. (#31142)``
+* ``Add deferrable param in SageMakerTransformOperator (#31063)``
+* ``Add deferrable param in SageMakerTrainingOperator (#31042)``
+* ``Add deferrable param in SageMakerProcessingOperator (#31062)``
+* ``Add IAM authentication to Amazon Redshift Connection by AWS Connection (#28187)``
+* ``'StepFunctionStartExecutionOperator': get logs in case of failure (#31072)``
+* ``Add on_kill to EMR Serverless Job Operator (#31169)``
+* ``Add Deferrable Mode for EC2StateSensor (#31130)``
+
+Bug Fixes
+~~~~~~~~~
+
+* ``bigfix: EMRHook  Loop through paginated response to check for cluster id (#29732)``
+
+Misc
+~~~~
+
+* ``Bump minimum Airflow version in providers (#30917)``
+* ``Add template field to S3ToRedshiftOperator (#30781)``
+* ``Add extras links to some more EMR Operators and Sensors (#31032)``
+* ``Add retries to S3 delete_bucket (#31192)``
+* ``Add tags param in RedshiftCreateClusterSnapshotOperator (#31006)``
+* ``improve/fix glue job logs printing (#30886)``
+* ``Import aiobotocore only if deferrable is true (#31094)``
+* ``Update return types of 'get_key' methods on 'S3Hook' (#30923)``
+* ``Support 'shareIdentifier' in BatchOperator (#30829)``
+* ``BaseAWS - Override client when resource_type is user to get custom waiters (#30897)``
+* ``Add future-compatible mongo Hook typing (#31289)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Move TaskInstanceKey to a separate file (#31033)``
+   * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
+   * ``DynamoDBToS3Operator - Add feature to export table to a point in time (#30501)``
+   * ``Revert "DynamoDBToS3Operator - Add feature to export table to a point in time (#30501)" (#31139)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Bring back detection of implicit single-line string concatenation (#31270)``
+
 8.0.0
 ......
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
 .. warning::
@@ -480,16 +484,17 @@
    appropriate section above if needed. Do not delete the lines(!):
    * ``System Test for EMR (AIP-47) (#27286)``
    * ``Prepare for follow-up release for November providers (#27774)``
 
 6.1.0
 .....
 
-This release of provider is only available for Airflow 2.3+ as explained in the
-`Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/README.md#support-for-providers>`_.
+.. note::
+  This release of provider is only available for Airflow 2.3+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Misc
 ~~~~
 
 * ``Move min airflow version to 2.3.0 for all providers (#27196)``
 * ``Replace urlparse with urlsplit (#27389)``
 
@@ -720,16 +725,17 @@
 
 4.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
-* This release of provider is only available for Airflow 2.2+ as explained in the Apache Airflow
-  providers support policy https://github.com/apache/airflow/blob/main/README.md#support-for-providers
+.. note::
+  This release of provider is only available for Airflow 2.2+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Features
 ~~~~~~~~
 
 * ``Add partition related methods to GlueCatalogHook: (#23857)``
 * ``Add support for associating  custom tags to job runs submitted via EmrContainerOperator (#23769)``
 * ``Add number of node params only for single-node cluster in RedshiftCreateClusterOperator (#23839)``
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/apache_airflow_providers_amazon.egg-info/SOURCES.txt` & `apache-airflow-providers-amazon-8.1.0rc1/apache_airflow_providers_amazon.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -122,31 +122,35 @@
 airflow/providers/amazon/aws/transfers/s3_to_redshift.py
 airflow/providers/amazon/aws/transfers/s3_to_sftp.py
 airflow/providers/amazon/aws/transfers/s3_to_sql.py
 airflow/providers/amazon/aws/transfers/salesforce_to_s3.py
 airflow/providers/amazon/aws/transfers/sftp_to_s3.py
 airflow/providers/amazon/aws/transfers/sql_to_s3.py
 airflow/providers/amazon/aws/triggers/__init__.py
+airflow/providers/amazon/aws/triggers/ec2.py
 airflow/providers/amazon/aws/triggers/redshift_cluster.py
+airflow/providers/amazon/aws/triggers/sagemaker.py
 airflow/providers/amazon/aws/utils/__init__.py
 airflow/providers/amazon/aws/utils/connection_wrapper.py
 airflow/providers/amazon/aws/utils/eks_get_token.py
 airflow/providers/amazon/aws/utils/emailer.py
 airflow/providers/amazon/aws/utils/rds.py
 airflow/providers/amazon/aws/utils/redshift.py
 airflow/providers/amazon/aws/utils/sagemaker.py
 airflow/providers/amazon/aws/utils/tags.py
 airflow/providers/amazon/aws/utils/waiter.py
 airflow/providers/amazon/aws/waiters/__init__.py
 airflow/providers/amazon/aws/waiters/appflow.json
 airflow/providers/amazon/aws/waiters/base_waiter.py
+airflow/providers/amazon/aws/waiters/dynamodb.json
 airflow/providers/amazon/aws/waiters/ecs.json
 airflow/providers/amazon/aws/waiters/eks.json
 airflow/providers/amazon/aws/waiters/emr-serverless.json
 airflow/providers/amazon/aws/waiters/emr.json
+airflow/providers/amazon/aws/waiters/sagemaker.json
 apache_airflow_providers_amazon.egg-info/PKG-INFO
 apache_airflow_providers_amazon.egg-info/SOURCES.txt
 apache_airflow_providers_amazon.egg-info/dependency_links.txt
 apache_airflow_providers_amazon.egg-info/entry_points.txt
 apache_airflow_providers_amazon.egg-info/not-zip-safe
 apache_airflow_providers_amazon.egg-info/requires.txt
 apache_airflow_providers_amazon.egg-info/top_level.txt
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/apache_airflow_providers_amazon.egg-info/requires.txt` & `apache-airflow-providers-amazon-8.1.0rc1/apache_airflow_providers_amazon.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 apache-airflow-providers-common-sql>=1.3.1.dev0
-apache-airflow>=2.3.0.dev0
+apache-airflow>=2.4.0.dev0
 asgiref
 boto3>=1.24.0
 jsonpath_ng>=1.5.3
 mypy-boto3-appflow>=1.24.0
 mypy-boto3-rds>=1.24.0
 mypy-boto3-redshift-data>=1.24.0
+mypy-boto3-s3>=1.24.0
 redshift_connector>=2.0.888
 sqlalchemy_redshift>=0.8.6
 watchtower~=2.0.1
 
 [aiobotocore]
 aiobotocore[boto3]>=2.2.0
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/pyproject.toml` & `apache-airflow-providers-amazon-8.1.0rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,16 @@
 target-version = "py37"
 
 extend-select = [
     "I", # Missing required import (auto-fixable)
     "UP", # Pyupgrade
     "RUF100", # Unused noqa (auto-fixable)
 
+    # implicit single-line string concatenation
+    "ISC001",
     # We ignore more pydocstyle than we enable, so be more selective at what we enable
     "D101",
     "D106",
     "D2",
     "D3",
     # "D401", # Not enabled by ruff, but we don't want it
     "D402",
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/setup.cfg` & `apache-airflow-providers-amazon-8.1.0rc1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.0.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.1.0/
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
@@ -43,29 +43,30 @@
 python_requires = ~=3.7
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
 	apache-airflow-providers-common-sql>=1.3.1.dev0
-	apache-airflow>=2.3.0.dev0
+	apache-airflow>=2.4.0.dev0
 	asgiref
 	boto3>=1.24.0
 	jsonpath_ng>=1.5.3
 	mypy-boto3-appflow>=1.24.0
 	mypy-boto3-rds>=1.24.0
 	mypy-boto3-redshift-data>=1.24.0
+	mypy-boto3-s3>=1.24.0
 	redshift_connector>=2.0.888
 	sqlalchemy_redshift>=0.8.6
 	watchtower~=2.0.1
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.amazon.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.amazon
 
 [egg_info]
-tag_build = rc3
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc3/setup.py` & `apache-airflow-providers-amazon-8.1.0rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-amazon package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "8.0.0"
+version = "8.1.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-amazon setup."""
     setup(
         version=version,
         extras_require={
```

