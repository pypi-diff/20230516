# Comparing `tmp/cloud-governance-1.1.97.tar.gz` & `tmp/cloud-governance-1.1.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud-governance-1.1.97.tar", last modified: Mon May 15 09:22:34 2023, max compression
+gzip compressed data, was "cloud-governance-1.1.98.tar", last modified: Tue May 16 18:38:37 2023, max compression
```

## Comparing `cloud-governance-1.1.97.tar` & `cloud-governance-1.1.98.tar`

### file list

```diff
@@ -1,219 +1,226 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.087942 cloud-governance-1.1.97/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14803 2023-05-15 09:22:34.087942 cloud-governance-1.1.97/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14122 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.071942 cloud-governance-1.1.97/cloud_governance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.071942 cloud-governance-1.1.97/cloud_governance/cloud_resource_orchestration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/cloud_resource_orchestration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.071942 cloud-governance-1.1.97/cloud_governance/cloud_resource_orchestration/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/cloud_resource_orchestration/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.071942 cloud-governance-1.1.97/cloud_governance/cloud_resource_orchestration/aws/long_run/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/cloud_resource_orchestration/aws/long_run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/cloud_resource_orchestration/aws/long_run/ec2_long_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/cloud_resource_orchestration/aws/long_run/monitor_in_progress_issues.py
--rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/cloud_resource_orchestration/aws/long_run/monitor_long_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     6380 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/cloud_resource_orchestration/aws/long_run/tag_long_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.075942 cloud-governance-1.1.97/cloud_governance/cloud_resource_orchestration/aws/short_run/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/cloud_resource_orchestration/aws/short_run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/cloud_resource_orchestration/aws/short_run/ec2_short_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.075942 cloud-governance-1.1.97/cloud_governance/cloud_resource_orchestration/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/cloud_resource_orchestration/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11864 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/cloud_resource_orchestration/common/ec2_monitor_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.075942 cloud-governance-1.1.97/cloud_governance/cloud_resource_orchestration/monitor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/cloud_resource_orchestration/monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/cloud_resource_orchestration/monitor/cloud_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.075942 cloud-governance-1.1.97/cloud_governance/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.075942 cloud-governance-1.1.97/cloud_governance/common/clouds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/clouds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.075942 cloud-governance-1.1.97/cloud_governance/common/clouds/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/clouds/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.075942 cloud-governance-1.1.97/cloud_governance/common/clouds/aws/cloudtrail/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/clouds/aws/cloudtrail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13416 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/clouds/aws/cloudtrail/cloudtrail_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.075942 cloud-governance-1.1.97/cloud_governance/common/clouds/aws/cloudwatch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/clouds/aws/cloudwatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/clouds/aws/cloudwatch/cloudwatch_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.075942 cloud-governance-1.1.97/cloud_governance/common/clouds/aws/cost_explorer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/clouds/aws/cost_explorer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/clouds/aws/cost_explorer/cost_explorer_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.075942 cloud-governance-1.1.97/cloud_governance/common/clouds/aws/dynamodb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/clouds/aws/dynamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/clouds/aws/dynamodb/dynamodb_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.075942 cloud-governance-1.1.97/cloud_governance/common/clouds/aws/ec2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/clouds/aws/ec2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17897 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/clouds/aws/ec2/ec2_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.075942 cloud-governance-1.1.97/cloud_governance/common/clouds/aws/iam/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/clouds/aws/iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/clouds/aws/iam/iam_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.075942 cloud-governance-1.1.97/cloud_governance/common/clouds/aws/price/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/clouds/aws/price/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/clouds/aws/price/price.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/clouds/aws/price/resources_pricing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.075942 cloud-governance-1.1.97/cloud_governance/common/clouds/aws/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/clouds/aws/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11967 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/clouds/aws/s3/s3_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.075942 cloud-governance-1.1.97/cloud_governance/common/clouds/aws/sts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/clouds/aws/sts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/clouds/aws/sts/sts_oprations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.075942 cloud-governance-1.1.97/cloud_governance/common/clouds/aws/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/clouds/aws/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/clouds/aws/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.075942 cloud-governance-1.1.97/cloud_governance/common/clouds/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/clouds/azure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.075942 cloud-governance-1.1.97/cloud_governance/common/clouds/azure/cost_management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/clouds/azure/cost_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/clouds/azure/cost_management/cost_management_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.075942 cloud-governance-1.1.97/cloud_governance/common/clouds/azure/subscriptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/clouds/azure/subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/clouds/azure/subscriptions/azure_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.075942 cloud-governance-1.1.97/cloud_governance/common/clouds/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/clouds/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/clouds/gcp/google_account.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.075942 cloud-governance-1.1.97/cloud_governance/common/clouds/ibm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/clouds/ibm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.075942 cloud-governance-1.1.97/cloud_governance/common/clouds/ibm/account/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/clouds/ibm/account/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/clouds/ibm/account/ibm_account.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.075942 cloud-governance-1.1.97/cloud_governance/common/clouds/ibm/classic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/clouds/ibm/classic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/clouds/ibm/classic/classic_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.075942 cloud-governance-1.1.97/cloud_governance/common/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/elasticsearch/elastic_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/elasticsearch/elasticsearch_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/elasticsearch/elasticsearch_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.079942 cloud-governance-1.1.97/cloud_governance/common/google_drive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/google_drive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/google_drive/google_drive_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/google_drive/upload_to_gsheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.079942 cloud-governance-1.1.97/cloud_governance/common/jira/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/jira/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9020 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/jira/jira.py
--rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/jira/jira_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.079942 cloud-governance-1.1.97/cloud_governance/common/ldap/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/ldap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/ldap/ldap_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.079942 cloud-governance-1.1.97/cloud_governance/common/logger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/logger/init_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/logger/logger_time_stamp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.079942 cloud-governance-1.1.97/cloud_governance/common/mails/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/mails/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/mails/gmail.py
--rw-r--r--   0 runner    (1001) docker     (123)    12254 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/mails/mail_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/mails/postfix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.079942 cloud-governance-1.1.97/cloud_governance/common/tool/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/common/tool/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.079942 cloud-governance-1.1.97/cloud_governance/main/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16723 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/main/environment_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/main/environment_variables_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10656 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/main/es_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)    16025 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/main/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.079942 cloud-governance-1.1.97/cloud_governance/policy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.079942 cloud-governance-1.1.97/cloud_governance/policy/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/aws/cost_billing_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/aws/cost_explorer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15631 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/aws/cost_explorer_payer_billings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/aws/cost_over_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/aws/ebs_in_use.py
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/aws/ebs_unattached.py
--rw-r--r--   0 runner    (1001) docker     (123)     9741 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/aws/ec2_idle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/aws/ec2_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8141 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/aws/ec2_stop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/aws/empty_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/aws/ip_unattached.py
--rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/aws/monthly_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/aws/s3_inactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/aws/skipped_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/aws/unused_nat_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    51727 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/aws/zombie_cluster_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/aws/zombie_snapshots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.079942 cloud-governance-1.1.97/cloud_governance/policy/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/azure/cost_billing_reports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.079942 cloud-governance-1.1.97/cloud_governance/policy/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14218 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/gcp/cost_billing_reports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.083942 cloud-governance-1.1.97/cloud_governance/policy/ibm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/ibm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/ibm/cost_billing_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/ibm/ibm_cost_over_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/ibm/ibm_cost_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/ibm/tag_baremetal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/ibm/tag_vm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.083942 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.083942 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.083942 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/cost_expenditure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/cost_expenditure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/cost_expenditure/cost_report_policies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.083942 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/cloudtrail_to_dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/upload_data_to_dynamodb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.083942 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/tag_cluster/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/tag_cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/tag_cluster/remove_cluster_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/tag_cluster/run_tag_cluster_resouces.py
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)    41938 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_resouces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.083942 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/tag_non_cluster/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/tag_non_cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9494 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/tag_non_cluster/non_cluster_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/tag_non_cluster/remove_non_cluster_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/tag_non_cluster/run_tag_non_cluster_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    12945 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/tag_non_cluster/tag_non_cluster_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/tag_non_cluster/update_na_tag_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.083942 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/tag_user/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/tag_user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/tag_user/iam_user_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/tag_user/remove_user_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/tag_user/run_tag_iam_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    10510 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/tag_user/tag_iam_user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.083942 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/zombie_cluster/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/zombie_cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27642 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_ec2_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_iam_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_s3_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/zombie_cluster/run_zombie_cluster_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/zombie_cluster/validate_zombies.py
--rw-r--r--   0 runner    (1001) docker     (123)    14370 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/zombie_cluster/zombie_cluster_common_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.083942 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17153 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/run_zombie_non_cluster_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/zombie_non_cluster_polices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.083942 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/azure/azure_policy_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.083942 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/gcp/gcp_policy_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.083942 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/gitleaks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/gitleaks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/gitleaks/gitleaks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.087942 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/ibm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/ibm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.087942 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/ibm/ibm_operations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/ibm/ibm_operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_policy_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.087942 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/ibm/tagging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/ibm/tagging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/cloud_governance/policy/policy_operations/ibm/tagging/tagging_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:22:34.071942 cloud-governance-1.1.97/cloud_governance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14803 2023-05-15 09:22:33.000000 cloud-governance-1.1.97/cloud_governance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-05-15 09:22:34.000000 cloud-governance-1.1.97/cloud_governance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 09:22:33.000000 cloud-governance-1.1.97/cloud_governance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 09:22:33.000000 cloud-governance-1.1.97/cloud_governance.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-15 09:22:34.000000 cloud-governance-1.1.97/cloud_governance.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-15 09:22:34.000000 cloud-governance-1.1.97/cloud_governance.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-15 09:22:34.087942 cloud-governance-1.1.97/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-15 09:22:15.000000 cloud-governance-1.1.97/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.163784 cloud-governance-1.1.98/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14803 2023-05-16 18:38:37.163784 cloud-governance-1.1.98/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14122 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.143784 cloud-governance-1.1.98/cloud_governance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.147784 cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.147784 cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.147784 cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/aws/long_run/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/aws/long_run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/aws/long_run/ec2_long_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/aws/long_run/monitor_in_progress_issues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/aws/long_run/monitor_long_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6380 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/aws/long_run/tag_long_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.147784 cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/aws/short_run/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/aws/short_run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/aws/short_run/ec2_short_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.147784 cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11864 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/common/ec2_monitor_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.147784 cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/monitor/cloud_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.147784 cloud-governance-1.1.98/cloud_governance/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.147784 cloud-governance-1.1.98/cloud_governance/common/clouds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.147784 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.147784 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/cloudtrail/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/cloudtrail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13416 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/cloudtrail/cloudtrail_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.147784 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/cloudwatch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/cloudwatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/cloudwatch/cloudwatch_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.147784 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/cost_explorer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/cost_explorer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/cost_explorer/cost_explorer_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.147784 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/dynamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/dynamodb/dynamodb_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.147784 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/ec2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18246 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/ec2/ec2_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.147784 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/iam/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/iam/iam_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.147784 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/price/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/price/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/price/price.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/price/resources_pricing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.147784 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12090 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/s3/s3_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.151784 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/sts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/sts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/sts/sts_oprations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.151784 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.151784 cloud-governance-1.1.98/cloud_governance/common/clouds/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/azure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.151784 cloud-governance-1.1.98/cloud_governance/common/clouds/azure/cost_management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/azure/cost_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/azure/cost_management/cost_management_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.151784 cloud-governance-1.1.98/cloud_governance/common/clouds/azure/subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/azure/subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/azure/subscriptions/azure_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.151784 cloud-governance-1.1.98/cloud_governance/common/clouds/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/gcp/google_account.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.151784 cloud-governance-1.1.98/cloud_governance/common/clouds/ibm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/ibm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.151784 cloud-governance-1.1.98/cloud_governance/common/clouds/ibm/account/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/ibm/account/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/ibm/account/ibm_account.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.151784 cloud-governance-1.1.98/cloud_governance/common/clouds/ibm/classic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/ibm/classic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/ibm/classic/classic_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.151784 cloud-governance-1.1.98/cloud_governance/common/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/elasticsearch/elastic_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/elasticsearch/elasticsearch_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/elasticsearch/elasticsearch_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.151784 cloud-governance-1.1.98/cloud_governance/common/google_drive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/google_drive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/google_drive/google_drive_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/google_drive/upload_to_gsheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.151784 cloud-governance-1.1.98/cloud_governance/common/jira/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/jira/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9020 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/jira/jira.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/jira/jira_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.151784 cloud-governance-1.1.98/cloud_governance/common/ldap/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/ldap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/ldap/ldap_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.151784 cloud-governance-1.1.98/cloud_governance/common/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/logger/init_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/logger/logger_time_stamp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.151784 cloud-governance-1.1.98/cloud_governance/common/mails/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/mails/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/mails/gmail.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16489 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/mails/mail_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/mails/postfix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.151784 cloud-governance-1.1.98/cloud_governance/common/tool/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/tool/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.155784 cloud-governance-1.1.98/cloud_governance/main/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18195 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/main/environment_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/main/environment_variables_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10656 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/main/es_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16636 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/main/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/main/main_common_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.155784 cloud-governance-1.1.98/cloud_governance/policy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.155784 cloud-governance-1.1.98/cloud_governance/policy/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/aws/cost_billing_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/aws/cost_explorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15608 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/aws/cost_explorer_payer_billings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/aws/cost_over_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/aws/ebs_in_use.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/aws/ebs_unattached.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9741 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/aws/ec2_idle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/aws/ec2_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/aws/ec2_stop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/aws/empty_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/aws/ip_unattached.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/aws/monthly_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/aws/s3_inactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/aws/skipped_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/aws/unused_nat_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51727 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/aws/zombie_cluster_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/aws/zombie_snapshots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.155784 cloud-governance-1.1.98/cloud_governance/policy/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/azure/cost_billing_reports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.155784 cloud-governance-1.1.98/cloud_governance/policy/common_policies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/common_policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/common_policies/send_aggregated_alerts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.155784 cloud-governance-1.1.98/cloud_governance/policy/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14218 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/gcp/cost_billing_reports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.155784 cloud-governance-1.1.98/cloud_governance/policy/ibm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/ibm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/ibm/cost_billing_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/ibm/ibm_cost_over_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/ibm/ibm_cost_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/ibm/tag_baremetal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/ibm/tag_vm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.155784 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.155784 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.155784 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/cost_expenditure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/cost_expenditure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/cost_expenditure/cost_report_policies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.159784 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/cloudtrail_to_dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/upload_data_to_dynamodb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.159784 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_cluster/remove_cluster_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_cluster/run_tag_cluster_resouces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41938 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_resouces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.159784 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_non_cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_non_cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9494 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_non_cluster/non_cluster_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_non_cluster/remove_non_cluster_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_non_cluster/run_tag_non_cluster_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12945 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_non_cluster/tag_non_cluster_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_non_cluster/update_na_tag_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.159784 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_user/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_user/iam_user_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_user/remove_user_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_user/run_tag_iam_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10510 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_user/tag_iam_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.159784 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/zombie_cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/zombie_cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27642 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_ec2_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_iam_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_s3_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/zombie_cluster/run_zombie_cluster_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/zombie_cluster/validate_zombies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14301 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/zombie_cluster/zombie_cluster_common_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.159784 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17153 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/run_zombie_non_cluster_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/zombie_non_cluster_polices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.159784 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/azure/azure_policy_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.159784 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/gcp/gcp_policy_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.159784 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/gitleaks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/gitleaks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/gitleaks/gitleaks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.159784 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/ibm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/ibm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.159784 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/ibm/ibm_operations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/ibm/ibm_operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_policy_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.163784 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/ibm/tagging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/ibm/tagging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/ibm/tagging/tagging_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.163784 cloud-governance-1.1.98/cloud_governance/policy/policy_runners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_runners/common_policy_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.147784 cloud-governance-1.1.98/cloud_governance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14803 2023-05-16 18:38:37.000000 cloud-governance-1.1.98/cloud_governance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9637 2023-05-16 18:38:37.000000 cloud-governance-1.1.98/cloud_governance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 18:38:37.000000 cloud-governance-1.1.98/cloud_governance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 18:38:37.000000 cloud-governance-1.1.98/cloud_governance.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-16 18:38:37.000000 cloud-governance-1.1.98/cloud_governance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 18:38:37.000000 cloud-governance-1.1.98/cloud_governance.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-16 18:38:37.163784 cloud-governance-1.1.98/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/setup.py
```

### Comparing `cloud-governance-1.1.97/LICENSE` & `cloud-governance-1.1.98/LICENSE`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/PKG-INFO` & `cloud-governance-1.1.98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-governance
-Version: 1.1.97
+Version: 1.1.98
 Summary: Cloud Governance Tool
 Home-page: https://github.com/redhat-performance/cloud-governance
 Author: Red Hat
 Author-email: ebattat@redhat.com, athiruma@redhat.com
 License: Apache License 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cloud-governance-1.1.97/README.md` & `cloud-governance-1.1.98/README.md`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/cloud_resource_orchestration/aws/long_run/ec2_long_run.py` & `cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/aws/long_run/ec2_long_run.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/cloud_resource_orchestration/aws/long_run/monitor_in_progress_issues.py` & `cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/aws/long_run/monitor_in_progress_issues.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/cloud_resource_orchestration/aws/long_run/monitor_long_run.py` & `cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/aws/long_run/monitor_long_run.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/cloud_resource_orchestration/aws/long_run/tag_long_run.py` & `cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/aws/long_run/tag_long_run.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/cloud_resource_orchestration/common/ec2_monitor_operations.py` & `cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/common/ec2_monitor_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/cloud_resource_orchestration/monitor/cloud_monitor.py` & `cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/monitor/cloud_monitor.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/common/clouds/aws/cloudtrail/cloudtrail_operations.py` & `cloud-governance-1.1.98/cloud_governance/common/clouds/aws/cloudtrail/cloudtrail_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/common/clouds/aws/cloudwatch/cloudwatch_operations.py` & `cloud-governance-1.1.98/cloud_governance/common/clouds/aws/cloudwatch/cloudwatch_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/common/clouds/aws/cost_explorer/cost_explorer_operations.py` & `cloud-governance-1.1.98/cloud_governance/common/clouds/aws/cost_explorer/cost_explorer_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/common/clouds/aws/dynamodb/dynamodb_operations.py` & `cloud-governance-1.1.98/cloud_governance/common/clouds/aws/dynamodb/dynamodb_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/common/clouds/aws/ec2/ec2_operations.py` & `cloud-governance-1.1.98/cloud_governance/common/clouds/aws/ec2/ec2_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -512,7 +512,17 @@
         if tags:
             for tag in tags:
                 key = tag.get('Key').lower().replace("_", '').replace("-", '')
                 if key == tag_name.lower():
                     return tag.get('Value')
         return default_value
 
+    def get_active_regions(self):
+        """
+        This method return active regions in aws account
+        :return:
+        """
+        responses = self.ec2_client.describe_regions()['Regions']
+        active_regions = []
+        for region in responses:
+            active_regions.append(region.get('RegionName'))
+        return active_regions
```

### Comparing `cloud-governance-1.1.97/cloud_governance/common/clouds/aws/iam/iam_operations.py` & `cloud-governance-1.1.98/cloud_governance/common/clouds/aws/iam/iam_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/common/clouds/aws/price/price.py` & `cloud-governance-1.1.98/cloud_governance/common/clouds/aws/price/price.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/common/clouds/aws/price/resources_pricing.py` & `cloud-governance-1.1.98/cloud_governance/common/clouds/aws/price/resources_pricing.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/common/clouds/aws/s3/s3_operations.py` & `cloud-governance-1.1.98/cloud_governance/common/clouds/aws/s3/s3_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -222,28 +222,30 @@
         except ClientError as err:
             raise
         except Exception:
             raise
 
     @logger_time_stamp
     @typeguard.typechecked
-    def get_last_objects(self, bucket: str, logs_bucket_key: str, policy: str):
+    def get_last_objects(self, bucket: str, logs_bucket_key: str = '', policy: str = '', key_prefix: str = ''):
         """
         This method return last object per policy, only path without file name
         @param logs_bucket_key:
         @param bucket:
         @param policy:
+        @param key_prefix:
         @return:
         """
         try:
-            if '_' in policy:
-                policy = policy.replace('_', '-')
-            date_key = (datetime.datetime.now() - datetime.timedelta(days=1)).strftime("%Y/%m/%d")
-            objs = self.__s3_client.list_objects_v2(Bucket=bucket,
-                                                    Prefix=f'{logs_bucket_key}/{policy}/{date_key}')['Contents']
+            if not key_prefix:
+                if '_' in policy:
+                    policy = policy.replace('_', '-')
+                date_key = (datetime.datetime.now() - datetime.timedelta(days=1)).strftime("%Y/%m/%d")
+                key_prefix = f'{logs_bucket_key}/{policy}/{date_key}'
+            objs = self.__s3_client.list_objects_v2(Bucket=bucket, Prefix=key_prefix)['Contents']
         except:
             return None
         get_last_modified_key = lambda obj: int(obj['LastModified'].strftime('%s'))
         full_path = [obj['Key'] for obj in sorted(objs, key=get_last_modified_key)][-1]
         return os.path.dirname(full_path)
 
     @staticmethod
@@ -298,24 +300,25 @@
         @param policy:
         @return:
         """
         return self.get_last_objects(bucket=self.__bucket,
                                      logs_bucket_key=f'{self.__logs_bucket_key}/{self.__region}',
                                      policy=policy)
 
-    def get_last_s3_policy_content(self, policy: str, file_name: str):
+    def get_last_s3_policy_content(self, policy: str = '', file_name: str = '', s3_file_path: str = None):
         """
         This method return last policy content
         @return:
         """
         with tempfile.TemporaryDirectory() as temp_local_directory:
             local_file = temp_local_directory + '/' + file_name + '.gz'
-            if self.__get_s3_latest_policy_file(policy=policy):
-                latest_policy_path = self.__get_s3_latest_policy_file(policy=policy)
-                self.download_file(bucket=self.__bucket,
-                                   key=str(latest_policy_path),
-                                   download_file=file_name + '.gz',
-                                   file_name_path=local_file)
-                # gzip
-                os.system(f"gzip -d {local_file}")
-                with open(os.path.join(temp_local_directory, file_name)) as f:
-                    return f.read()
+            if not s3_file_path:
+                if self.__get_s3_latest_policy_file(policy=policy):
+                    s3_file_path = self.__get_s3_latest_policy_file(policy=policy)
+            self.download_file(bucket=self.__bucket,
+                               key=str(s3_file_path),
+                               download_file=file_name + '.gz',
+                               file_name_path=local_file)
+            # gzip
+            os.system(f"gzip -d {local_file}")
+            with open(os.path.join(temp_local_directory, file_name)) as f:
+                return f.read()
```

### Comparing `cloud-governance-1.1.97/cloud_governance/common/clouds/aws/utils/utils.py` & `cloud-governance-1.1.98/cloud_governance/common/clouds/aws/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/common/clouds/azure/cost_management/cost_management_operations.py` & `cloud-governance-1.1.98/cloud_governance/common/clouds/azure/cost_management/cost_management_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/common/clouds/azure/subscriptions/azure_operations.py` & `cloud-governance-1.1.98/cloud_governance/common/clouds/azure/subscriptions/azure_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/common/clouds/gcp/google_account.py` & `cloud-governance-1.1.98/cloud_governance/common/clouds/gcp/google_account.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/common/clouds/ibm/account/ibm_account.py` & `cloud-governance-1.1.98/cloud_governance/common/clouds/ibm/account/ibm_account.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/common/clouds/ibm/classic/classic_operations.py` & `cloud-governance-1.1.98/cloud_governance/common/clouds/ibm/classic/classic_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/common/elasticsearch/elastic_upload.py` & `cloud-governance-1.1.98/cloud_governance/common/elasticsearch/elastic_upload.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/common/elasticsearch/elasticsearch_operations.py` & `cloud-governance-1.1.98/cloud_governance/common/elasticsearch/elasticsearch_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/common/google_drive/google_drive_operations.py` & `cloud-governance-1.1.98/cloud_governance/common/google_drive/google_drive_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/common/google_drive/upload_to_gsheet.py` & `cloud-governance-1.1.98/cloud_governance/common/google_drive/upload_to_gsheet.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/common/jira/jira.py` & `cloud-governance-1.1.98/cloud_governance/common/jira/jira.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/common/jira/jira_operations.py` & `cloud-governance-1.1.98/cloud_governance/common/jira/jira_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/common/ldap/ldap_search.py` & `cloud-governance-1.1.98/cloud_governance/common/ldap/ldap_search.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/common/logger/logger_time_stamp.py` & `cloud-governance-1.1.98/cloud_governance/common/logger/logger_time_stamp.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,21 +20,22 @@
         @param args:
         @param kwargs:
         @return: prefix + input method + suffix
         """
         time_start = time.time()
         date_time_start = datetime.datetime.now().strftime(datetime_format)
         try:
-            logger.info(f'Method name: {method.__name__} {kwargs} , Start time: {date_time_start} ')
+            logger.warn(f'Method name: {method.__name__} , Start time: {date_time_start} ')
+            logger.info(f'Method name: {method.__name__} {kwargs}')
             result = method(*args, **kwargs)
             time_end = time.time()
             date_time_end = datetime.datetime.now().strftime(datetime_format)
             total_time = time_end - time_start
             total_time_str = f'Total time: {round(total_time, 2)} sec'
-            logger.info(f'Method name: {method.__name__} , End time: {date_time_end} , {total_time_str}')
+            logger.warn(f'Method name: {method.__name__} , End time: {date_time_end} , {total_time_str}')
         except Exception as err:
             time_end = time.time()
             total_time = time_end - time_start
             date_time_end = datetime.datetime.now().strftime(datetime_format)
             logger.error(f'Method name: {method.__name__} , End time with errors: {date_time_end} , Total time: {round(total_time, 2)} sec')
             raise err  # Exception(method.__name__, err)
```

### Comparing `cloud-governance-1.1.97/cloud_governance/common/mails/gmail.py` & `cloud-governance-1.1.98/cloud_governance/common/mails/gmail.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/common/mails/mail_message.py` & `cloud-governance-1.1.98/cloud_governance/common/mails/mail_message.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,37 @@
-
+from cloud_governance.common.ldap.ldap_search import LdapSearch
+from cloud_governance.common.logger.logger_time_stamp import logger_time_stamp
 from cloud_governance.main.environment_variables import environment_variables
 
 
 class MailMessage:
-    RESTRICTION = 'Do not reply this email. If you need more clarification, please reach out to us in the CoreOS slack channel - #perf-dept-public-clouds.'
+
+    RESTRICTION = 'Do not reply this email. If you need more information, please reach out to us in the slack channel - #perf-dept-public-clouds.'
+    FOOTER = '<div style="color:gray">---<br />Thanks, <br />Cloud GovernanceTeam</div>'
 
     def __init__(self):
         self.__environment_variables_dict = environment_variables.environment_variables_dict
-        self.account = self.__environment_variables_dict.get('account', '')
+        self.account = self.__environment_variables_dict.get('account', '').upper()
         self.policy = self.__environment_variables_dict.get('policy', '')
         self.region = self.__environment_variables_dict.get('AWS_DEFAULT_REGION', '')
+        self.__LDAP_HOST_NAME = self.__environment_variables_dict.get('LDAP_HOST_NAME')
+        self.__ldap_search = LdapSearch(ldap_host_name=self.__LDAP_HOST_NAME)
+        self.__public_cloud_name = self.__environment_variables_dict.get('PUBLIC_CLOUD_NAME')
+
+    def get_user_display_name(self, user_name: str):
+        """
+        This method return user details from ldap
+        :param user_name:
+        :return:
+        """
+        user_details = self.__ldap_search.get_user_details(user_name=user_name)
+        if user_details:
+            return user_details.get('displayName')
+        else:
+            return None
 
     def ec2_stop(self, name: str, days: int, image_id: str, delete_instance_days: int, instance_name: str,
                  resource_id: str, stopped_time: str, ec2_type: str, **kwargs):
         extra_purse = ''
         if kwargs.get("extra_purse"):
             extra_purse = f', Cost {round(kwargs.get("extra_purse"), 3)} $ '
         subject = f'cloud-governance alert: ec2-stop'
@@ -272,7 +290,74 @@
                         --<br/>
                         Best Regards,<br/>
                         Cloud-governance Team<br/>
                     </address>
                 </div>
         """.strip()
         return subject, body
+
+    def filter_resources_on_days(self, resources: dict):
+        """
+        This method return the resources based on the days
+        :param resources:
+        :param days:
+        :return:
+        """
+        resources_by_days = {}
+        for policy_name, resource_data in resources.items():
+            for region_name, policy_region_data in resource_data.items():
+                for data_item in policy_region_data:
+                    resources_by_days.setdefault(data_item.get('Days'), []).append(data_item)
+        return resources_by_days
+
+    def get_data_in_html_table_format(self, resources: dict):
+        """
+        This method return user policy alerts in HTML table format
+        :param resources:
+        :return:
+        """
+        html_table_format = '<table width="auto" border="2" style="border-collapse: collapse;padding: 10px;border: 2px solid black;">'
+        html_style_value = "border-collapse: collapse;padding: 10px;border: 2px solid black;"
+        html_style = f'style="{html_style_value}"'
+        html_style_color = f'style="color:red;{html_style_value}"'
+        td_left, td_right = f'<td align="left" {html_style}>', '</td>'
+        td_left_color = f'<td align="left" {html_style_color}>'
+        th_left, th_right = f'<th align="left" {html_style}>', '</th>'
+        tr_left, tr_right = f'<tr {html_style}>', '</tr>'
+        thead_values = ['Policy', 'Region', 'ResourceId', 'Name', 'Action', 'DeletedDay']
+        html_table_format += '<thead>' + tr_left + ''.join([f'{th_left}{value}{th_right}' for value in thead_values]) + f'{tr_right}</thead><tbody>'
+        for days, resource_data in resources.items():
+            resource_data = sorted(resource_data, key=lambda item: (item.get('Policy'), item.get('Region')))
+            for resource in resource_data:
+                td_data = [resource.get(th_value) for th_value in thead_values]
+                if 'Deleted' == resource.get('Action'):
+                    html_table_format += f"""{tr_left }{''.join([f'{td_left_color}{value}{td_right}' for value in td_data])}{tr_right}"""
+                else:
+                    html_table_format += f"""{tr_left}{''.join([f'{td_left}{value}{td_right}' for value in td_data])}{tr_right}"""
+        html_table_format += '</tbody></table>'
+        return html_table_format
+
+    def get_agg_policies_mail_message(self, user: str, user_resources: dict):
+        """
+        This method return the message for the aggregated alert of all policies
+        :param user:
+        :param user_resources:
+        :return:
+        """
+        display_name = self.get_user_display_name(user_name=user)
+        resources_by_days = self.filter_resources_on_days(resources=user_resources)
+        table_data = self.get_data_in_html_table_format(resources=resources_by_days)
+        display_name = display_name if display_name else user
+        subject = f'Cloud Governance: Policy Alerts'
+        body = f"""
+        <div>
+            <p>Hi {display_name},</p>
+        </div>
+        <div>
+            <p>You can find below your unused resources in the {self.__public_cloud_name} account ({self.account}).</p>
+            <p>If you want to keep them, please add "Policy=Not_Delete" or "Policy=skip" tag for each resource</p>
+            {table_data}
+        </div>
+        <p>{self.RESTRICTION}</p>
+        {self.FOOTER}
+"""
+        return subject, body
```

### Comparing `cloud-governance-1.1.97/cloud_governance/common/mails/postfix.py` & `cloud-governance-1.1.98/cloud_governance/common/mails/postfix.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         self.__environment_variables_dict = environment_variables.environment_variables_dict
         self.reply_to = self.__environment_variables_dict.get('REPLY_TO', 'dev-null@redhat.com')
         self.__es_host = self.__environment_variables_dict.get('es_host', '')
         self.__policy = self.__environment_variables_dict.get('policy', '')
         self.__es_port = self.__environment_variables_dict.get('es_port', '')
         self.__account = self.__environment_variables_dict.get('account', '')
         self.__policy_output = self.__environment_variables_dict.get('policy_output', '')
+        self.__default_admins = self.__environment_variables_dict.get('DEFAULT_ADMINS')
         self.bucket_name, self.key = self.get_bucket_name()
         self.__es_index = 'cloud-governance-mail-messages'
         if self.__es_host:
             self.__es_operations = ElasticSearchOperations(es_host=self.__es_host, es_port=self.__es_port)
         if self.__policy_output:
             self.__s3_operations = S3Operations(region_name='us-east-1')
 
@@ -49,14 +50,15 @@
             key = targets[3]
         else:
             bucket_name = self.__policy_output
         return bucket_name, key
 
     @logger_time_stamp
     def send_email_postfix(self, subject: str, to: any, cc: list, content: str, **kwargs):
+        cc.extend(self.__default_admins)
         msg = MIMEMultipart('alternative')
         msg["Subject"] = subject
         msg["From"] = "%s <%s>" % (
             'cloud-governance',
             "@".join(["noreply-cloud-governance", 'redhat.com']),
         )
         if isinstance(to, str):
```

### Comparing `cloud-governance-1.1.97/cloud_governance/main/environment_variables.py` & `cloud-governance-1.1.98/cloud_governance/main/environment_variables.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import argparse
 import os
+from ast import literal_eval
 
 import boto3
 
 from cloud_governance.main.environment_variables_exceptions import ParseFailed
 
 
 class EnvironmentVariables:
@@ -33,14 +34,19 @@
 
         ##################################################################################################
         # dynamic parameters - configure for local run
         # parameters for running policies
         self._environment_variables_dict['account'] = EnvironmentVariables.get_env('account', '').upper()
         self._environment_variables_dict['AWS_DEFAULT_REGION'] = EnvironmentVariables.get_env('AWS_DEFAULT_REGION', '')
 
+        self._environment_variables_dict['log_level'] = EnvironmentVariables.get_env('log_level', 'INFO')
+        self._environment_variables_dict['PRINT_LOGS'] = EnvironmentVariables.get_boolean_from_environment('PRINT_LOGS', True)
+        if not self._environment_variables_dict['AWS_DEFAULT_REGION']:
+            self._environment_variables_dict['AWS_DEFAULT_REGION'] = 'us-east-2'
+
         if EnvironmentVariables.get_env('AWS_ACCESS_KEY_ID', '') and EnvironmentVariables.get_env('AWS_SECRET_ACCESS_KEY', ''):
             self._environment_variables_dict['account'] = self.get_aws_account_alias_name().upper()
 
         self._environment_variables_dict['policy'] = EnvironmentVariables.get_env('policy', '')
 
         self._environment_variables_dict['aws_non_cluster_policies'] = ['ec2_idle', 'ec2_stop', 'ec2_run', 'ebs_in_use',
                                                                         'ebs_unattached', 's3_inactive',
@@ -162,14 +168,26 @@
         if self._environment_variables_dict.get('GCP_DATABASE_TABLE_NAME'):
             self._environment_variables_dict['PUBLIC_CLOUD_NAME'] = 'GCP'
 
         self._environment_variables_dict['EMAIL_ALERT'] = EnvironmentVariables.get_boolean_from_environment('EMAIL_ALERT', True)
         self._environment_variables_dict['MANAGER_EMAIL_ALERT'] = EnvironmentVariables.get_boolean_from_environment('MANAGER_EMAIL_ALERT', True)
         self._environment_variables_dict['UPDATE_TAG_BULKS'] = int(EnvironmentVariables.get_env('UPDATE_TAG_BULKS', '20'))
 
+        # policies aggregate alert
+        self._environment_variables_dict['BUCKET_NAME'] = EnvironmentVariables.get_env('BUCKET_NAME')
+        self._environment_variables_dict['BUCKET_KEY'] = EnvironmentVariables.get_env('BUCKET_KEY')
+        self._environment_variables_dict['MAIL_ALERT_DAYS'] = literal_eval(EnvironmentVariables.get_env('MAIL_ALERT_DAYS', '[]'))
+        self._environment_variables_dict['POLICY_ACTIONS_DAYS'] = literal_eval(EnvironmentVariables.get_env('POLICY_ACTIONS_DAYS', '[]'))
+        self._environment_variables_dict['DEFAULT_ADMINS'] = literal_eval(EnvironmentVariables.get_env('DEFAULT_ADMINS', '[]'))
+        self._environment_variables_dict['KERBEROS_USERS'] = literal_eval(EnvironmentVariables.get_env('KERBEROS_USERS', '[]'))
+        self._environment_variables_dict['POLICIES_TO_ALERT'] = literal_eval(EnvironmentVariables.get_env('POLICIES_TO_ALERT', '[]'))
+        if self._environment_variables_dict.get('policy') in ['send_aggregated_alerts']:
+            self._environment_variables_dict['COMMON_POLICIES'] = True
+
+
     @staticmethod
     def to_bool(arg, def_val: bool = None):
         if isinstance(arg, bool):
             return arg
         if isinstance(arg, (int, float)):
             return arg != 0
         if isinstance(arg, str):
```

### Comparing `cloud-governance-1.1.97/cloud_governance/main/es_uploader.py` & `cloud-governance-1.1.98/cloud_governance/main/es_uploader.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/main/main.py` & `cloud-governance-1.1.98/cloud_governance/main/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import typeguard
 from ast import literal_eval  # str to dict
 import boto3  # regions
 
 from cloud_governance.cloud_resource_orchestration.monitor.cloud_monitor import CloudMonitor
+from cloud_governance.main.main_common_operations import run_common_policies
 from cloud_governance.policy.policy_operations.aws.cost_expenditure.cost_report_policies import CostReportPolicies
 from cloud_governance.policy.policy_operations.azure.azure_policy_runner import AzurePolicyRunner
 from cloud_governance.common.logger.logger_time_stamp import logger_time_stamp, logger
 from cloud_governance.policy.policy_operations.aws.tag_cluster.run_tag_cluster_resouces import tag_cluster_resource, \
     remove_cluster_resources_tags
 from cloud_governance.policy.policy_operations.aws.tag_non_cluster.run_tag_non_cluster_resources import tag_non_cluster_resource, \
     remove_tag_non_cluster_resource, tag_na_resources
@@ -191,130 +192,133 @@
     upload_data_es = environment_variables_dict.get('upload_data_es', '')
     es_host = environment_variables_dict.get('es_host', '')
     es_port = environment_variables_dict.get('es_port', '')
     es_index = environment_variables_dict.get('es_index', '')
     es_doc_type = environment_variables_dict.get('es_doc_type', '')
     bucket = environment_variables_dict.get('bucket', '')
 
-    non_cluster_polices_runner = None
-    is_non_cluster_polices_runner = policy in environment_variables_dict.get('aws_non_cluster_policies')
-    if is_non_cluster_polices_runner:
-        non_cluster_polices_runner = ZombieNonClusterPolicies()
-
-    ibm_classic_infrastructure_policy_runner = None
-    is_tag_ibm_classic_infrastructure_runner = policy in environment_variables_dict.get('ibm_policies')
-    if not is_tag_ibm_classic_infrastructure_runner:
-        if environment_variables_dict.get('PUBLIC_CLOUD_NAME') and environment_variables_dict.get('PUBLIC_CLOUD_NAME').upper() == 'IBM':
-            is_tag_ibm_classic_infrastructure_runner = policy in environment_variables_dict.get('cost_policies')
-    if is_tag_ibm_classic_infrastructure_runner:
-        ibm_classic_infrastructure_policy_runner = IBMPolicyRunner()
-
-    is_cost_explorer_policies_runner = ''
-    if environment_variables_dict.get('PUBLIC_CLOUD_NAME') == 'AWS':
-        cost_explorer_policies_runner = None
-        is_cost_explorer_policies_runner = policy in environment_variables_dict.get('cost_policies')
-        if is_cost_explorer_policies_runner:
-            cost_explorer_policies_runner = CostReportPolicies()
-
-    is_azure_policy_runner = ''
-    if environment_variables_dict.get('PUBLIC_CLOUD_NAME') and environment_variables_dict.get('PUBLIC_CLOUD_NAME').upper() == 'AZURE':
-        azure_cost_policy_runner = None
-        is_azure_policy_runner = policy in environment_variables_dict.get('cost_policies')
-        if is_azure_policy_runner:
-            azure_cost_policy_runner = AzurePolicyRunner()
-
-    # cloud_resource_orchestration lon_run/short_run
-    is_cloud_management = False
-    if environment_variables_dict.get('MANAGEMENT'):
-        is_cloud_management = True
-
-    is_gcp_policy_runner = ''
-    if environment_variables_dict.get('PUBLIC_CLOUD_NAME') and environment_variables_dict.get('PUBLIC_CLOUD_NAME').upper() == 'GCP':
-        gcp_cost_policy_runner = None
-        is_gcp_policy_runner = policy in environment_variables_dict.get('cost_policies')
-        if is_gcp_policy_runner:
-            gcp_cost_policy_runner = GcpPolicyRunner()
-
-    @logger_time_stamp
-    def run_non_cluster_polices_runner():
-        """
-        This method run the aws non-cluster policies
-        @return:
-        """
-        non_cluster_polices_runner.run()
-
-    def run_tag_ibm_classic_infrastructure_runner():
-        """
-        This method run the IBM policies
-        @return:
-        """
-        ibm_classic_infrastructure_policy_runner.run()
-
-    @logger_time_stamp
-    def run_cost_explorer_policies_runner():
-        """
-        This method run the aws cost_explorer policies
-        @return:
-        """
-        cost_explorer_policies_runner.run()
-
-    @logger_time_stamp
-    def run_azure_policy_runner():
-        """
-        This method run the azure policies
-        @return:
-        """
-        azure_cost_policy_runner.run()
-
-    @logger_time_stamp
-    def run_gcp_policy_runner():
-        """
-        This method run the gcp policies
-        """
-        gcp_cost_policy_runner.run()
-
-    # 1. ELK Uploader
-    if upload_data_es:
-        input_data = {'es_host': es_host,
-                      'es_port': int(es_port),
-                      'es_index': es_index,
-                      'es_doc_type': es_doc_type,
-                      'es_add_items': {'account': account},
-                      'bucket': bucket,
-                      'logs_bucket_key': 'logs',
-                      's3_file_name': 'resources.json',
-                      'region': region_env,
-                      'policy': policy,
-                      }
-        elk_uploader = ESUploader(**input_data)
-        elk_uploader.upload_to_es(account=account)
-    # 2. POLICY
-    elif is_non_cluster_polices_runner:
-        run_non_cluster_polices_runner()
-    elif is_tag_ibm_classic_infrastructure_runner:
-        run_tag_ibm_classic_infrastructure_runner()
-    elif is_cost_explorer_policies_runner:
-        run_cost_explorer_policies_runner()
-    elif is_azure_policy_runner:
-        run_azure_policy_runner()
-    elif is_cloud_management:
-        run_cloud_management()
-    elif is_gcp_policy_runner:
-        run_gcp_policy_runner()
+    if environment_variables_dict.get('COMMON_POLICIES'):
+        run_common_policies()
     else:
-        if not policy:
-            logger.exception(f'Missing Policy name: "{policy}"')
-            raise Exception(f'Missing Policy name: "{policy}"')
-        if region_env == 'all':
-            # must be set for boto3 client default region
-            # environment_variables_dict['AWS_DEFAULT_REGION'] = 'us-east-2'
-            ec2 = boto3.client('ec2')
-            regions_data = ec2.describe_regions()
-            for region in regions_data['Regions']:
-                # logger.info(f"region: {region['RegionName']}")
-                environment_variables_dict['AWS_DEFAULT_REGION'] = region['RegionName']
-                run_policy(account=account, policy=policy, region=region['RegionName'], dry_run=dry_run)
+        non_cluster_polices_runner = None
+        is_non_cluster_polices_runner = policy in environment_variables_dict.get('aws_non_cluster_policies')
+        if is_non_cluster_polices_runner:
+            non_cluster_polices_runner = ZombieNonClusterPolicies()
+
+        ibm_classic_infrastructure_policy_runner = None
+        is_tag_ibm_classic_infrastructure_runner = policy in environment_variables_dict.get('ibm_policies')
+        if not is_tag_ibm_classic_infrastructure_runner:
+            if environment_variables_dict.get('PUBLIC_CLOUD_NAME') and environment_variables_dict.get('PUBLIC_CLOUD_NAME').upper() == 'IBM':
+                is_tag_ibm_classic_infrastructure_runner = policy in environment_variables_dict.get('cost_policies')
+        if is_tag_ibm_classic_infrastructure_runner:
+            ibm_classic_infrastructure_policy_runner = IBMPolicyRunner()
+
+        is_cost_explorer_policies_runner = ''
+        if environment_variables_dict.get('PUBLIC_CLOUD_NAME') == 'AWS':
+            cost_explorer_policies_runner = None
+            is_cost_explorer_policies_runner = policy in environment_variables_dict.get('cost_policies')
+            if is_cost_explorer_policies_runner:
+                cost_explorer_policies_runner = CostReportPolicies()
+
+        is_azure_policy_runner = ''
+        if environment_variables_dict.get('PUBLIC_CLOUD_NAME') and environment_variables_dict.get('PUBLIC_CLOUD_NAME').upper() == 'AZURE':
+            azure_cost_policy_runner = None
+            is_azure_policy_runner = policy in environment_variables_dict.get('cost_policies')
+            if is_azure_policy_runner:
+                azure_cost_policy_runner = AzurePolicyRunner()
+
+        # cloud_resource_orchestration lon_run/short_run
+        is_cloud_management = False
+        if environment_variables_dict.get('MANAGEMENT'):
+            is_cloud_management = True
+
+        is_gcp_policy_runner = ''
+        if environment_variables_dict.get('PUBLIC_CLOUD_NAME') and environment_variables_dict.get('PUBLIC_CLOUD_NAME').upper() == 'GCP':
+            gcp_cost_policy_runner = None
+            is_gcp_policy_runner = policy in environment_variables_dict.get('cost_policies')
+            if is_gcp_policy_runner:
+                gcp_cost_policy_runner = GcpPolicyRunner()
+
+        @logger_time_stamp
+        def run_non_cluster_polices_runner():
+            """
+            This method run the aws non-cluster policies
+            @return:
+            """
+            non_cluster_polices_runner.run()
+
+        def run_tag_ibm_classic_infrastructure_runner():
+            """
+            This method run the IBM policies
+            @return:
+            """
+            ibm_classic_infrastructure_policy_runner.run()
+
+        @logger_time_stamp
+        def run_cost_explorer_policies_runner():
+            """
+            This method run the aws cost_explorer policies
+            @return:
+            """
+            cost_explorer_policies_runner.run()
+
+        @logger_time_stamp
+        def run_azure_policy_runner():
+            """
+            This method run the azure policies
+            @return:
+            """
+            azure_cost_policy_runner.run()
+
+        @logger_time_stamp
+        def run_gcp_policy_runner():
+            """
+            This method run the gcp policies
+            """
+            gcp_cost_policy_runner.run()
+
+        # 1. ELK Uploader
+        if upload_data_es:
+            input_data = {'es_host': es_host,
+                          'es_port': int(es_port),
+                          'es_index': es_index,
+                          'es_doc_type': es_doc_type,
+                          'es_add_items': {'account': account},
+                          'bucket': bucket,
+                          'logs_bucket_key': 'logs',
+                          's3_file_name': 'resources.json',
+                          'region': region_env,
+                          'policy': policy,
+                          }
+            elk_uploader = ESUploader(**input_data)
+            elk_uploader.upload_to_es(account=account)
+        # 2. POLICY
+        elif is_non_cluster_polices_runner:
+            run_non_cluster_polices_runner()
+        elif is_tag_ibm_classic_infrastructure_runner:
+            run_tag_ibm_classic_infrastructure_runner()
+        elif is_cost_explorer_policies_runner:
+            run_cost_explorer_policies_runner()
+        elif is_azure_policy_runner:
+            run_azure_policy_runner()
+        elif is_cloud_management:
+            run_cloud_management()
+        elif is_gcp_policy_runner:
+            run_gcp_policy_runner()
         else:
-            run_policy(account=account, policy=policy, region=region_env, dry_run=dry_run)
+            if not policy:
+                logger.exception(f'Missing Policy name: "{policy}"')
+                raise Exception(f'Missing Policy name: "{policy}"')
+            if region_env == 'all':
+                # must be set for boto3 client default region
+                # environment_variables_dict['AWS_DEFAULT_REGION'] = 'us-east-2'
+                ec2 = boto3.client('ec2')
+                regions_data = ec2.describe_regions()
+                for region in regions_data['Regions']:
+                    # logger.info(f"region: {region['RegionName']}")
+                    environment_variables_dict['AWS_DEFAULT_REGION'] = region['RegionName']
+                    run_policy(account=account, policy=policy, region=region['RegionName'], dry_run=dry_run)
+            else:
+                run_policy(account=account, policy=policy, region=region_env, dry_run=dry_run)
 
 
 main()
```

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/aws/cost_billing_reports.py` & `cloud-governance-1.1.98/cloud_governance/policy/aws/cost_billing_reports.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/aws/cost_explorer.py` & `cloud-governance-1.1.98/cloud_governance/policy/aws/cost_explorer.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/aws/cost_explorer_payer_billings.py` & `cloud-governance-1.1.98/cloud_governance/policy/aws/cost_explorer_payer_billings.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,15 +171,14 @@
             for idx, usage in cost_center_usage_accounts.items():
                 account = usage['Account']
                 cost_usage_data.setdefault(account, {}).update({idx: usage})
         self.get_linked_accounts_forecast(linked_account_usage=cost_usage_data)
         self.upload_data_elastic_search(linked_account_usage=cost_usage_data)
         return cost_usage_data
 
-    @logger_time_stamp
     def upload_data_elastic_search(self, linked_account_usage: dict):
         """This method uploads the data to elastic search"""
         for account, monthly_cost in linked_account_usage.items():
             monthly_account_cost = []
             for month, cost in monthly_cost.items():
                 monthly_account_cost.append(cost)
             self.elastic_upload.es_upload_data(items=monthly_account_cost, set_index='index_id')
```

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/aws/cost_over_usage.py` & `cloud-governance-1.1.98/cloud_governance/policy/aws/cost_over_usage.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/aws/ebs_in_use.py` & `cloud-governance-1.1.98/cloud_governance/policy/aws/ebs_in_use.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/aws/ebs_unattached.py` & `cloud-governance-1.1.98/cloud_governance/policy/aws/ebs_unattached.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,13 +48,14 @@
                                                                              resource_id='VolumeId',
                                                                              resource_type='CreateVolume',
                                                                              resource=volume,
                                                                              empty_days=last_detached_days,
                                                                              days_to_delete_resource=self.DAYS_TO_DELETE_RESOURCE,
                                                                              extra_purse=ebs_cost, delta_cost=delta_cost)
                         if unattached_volumes:
-                            unattached_volumes_data.append([volume.get('VolumeId'),
-                                                            self._get_tag_name_from_tags(tags=volume.get('Tags'), tag_name='Name'),
-                                                            self._get_tag_name_from_tags(tags=volume.get('Tags'), tag_name='User'),
-                                                            str(last_detached_days),
-                                                            self._get_tag_name_from_tags(tags=volume.get('Tags'), tag_name='Policy')])
+                            unattached_volumes_data.append({'ResourceId': volume.get('VolumeId'),
+                                                            'Name': self._get_tag_name_from_tags(tags=volume.get('Tags'), tag_name='Name'),
+                                                            'User': self._get_tag_name_from_tags(tags=volume.get('Tags'), tag_name='User'),
+                                                            'Days': str(last_detached_days),
+                                                            'Skip': self._get_tag_name_from_tags(tags=volume.get('Tags'), tag_name='Policy')
+                                                            })
         return unattached_volumes_data
```

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/aws/ec2_idle.py` & `cloud-governance-1.1.98/cloud_governance/policy/aws/ec2_idle.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/aws/ec2_run.py` & `cloud-governance-1.1.98/cloud_governance/policy/aws/ec2_run.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/aws/ec2_stop.py` & `cloud-governance-1.1.98/cloud_governance/policy/aws/ec2_stop.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,18 +67,20 @@
                                             days=days, ec2_type=resource.get("InstanceType"), instance_id=instance_id, admins=self._admins,
                                             message_type='notify-admin', stop_cost=stop_cost, delta_charge=delta_charge)
                     if sign(days, instance_days):
                         if days >= delete_instance_days:
                             stopped_instance_tags[instance_id] = resource.get('Tags')
                             ec2_types[instance_id] = resource.get('InstanceType')
                             block_device_mappings[instance_id] = resource.get('BlockDeviceMappings')
-                        stopped_instances.append([resource.get('InstanceId'), self._get_tag_name_from_tags(tags=resource.get('Tags'), tag_name='Name'),
-                                                  self._get_tag_name_from_tags(tags=resource.get('Tags'), tag_name='User'), str(resource.get('LaunchTime')),
-                                                  self._get_tag_name_from_tags(tags=resource.get('Tags'), tag_name='Policy')
-                                                  ])
+                        stopped_instances.append({
+                            'ResourceId': resource.get('InstanceId'),
+                            'Name': self._get_tag_name_from_tags(tags=resource.get('Tags'), tag_name='Name'),
+                            'User': self._get_tag_name_from_tags(tags=resource.get('Tags'), tag_name='User'),
+                            'LaunchTime': str(resource.get('LaunchTime')),
+                            'Policy': self._get_tag_name_from_tags(tags=resource.get('Tags'), tag_name='Policy')})
         if self._dry_run == "no":
             for instance_id, tags in stopped_instance_tags.items():
                 if self._get_policy_value(tags=tags) not in ('NOTDELETE', 'SKIP'):
                     tags.append({'Key': 'Policy', 'Value': 'backup'})
                     tag_specifications = [{'ResourceType': 'image', 'Tags': tags}]
                     if sign == ge:
                         tag_specifications.append({'ResourceType': 'snapshot', 'Tags': tags})
```

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/aws/empty_roles.py` & `cloud-governance-1.1.98/cloud_governance/policy/aws/empty_roles.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,19 @@
                     if not role_inline_policies.get('PolicyNames') and not role_attached_policies.get('AttachedPolicies'):
                         role_empty = True
                         if not self._get_tag_name_from_tags(tags=tags, tag_name='Name'):
                             tags.append({'Key': 'Name', 'Value': role_name})
                         empty_days = self._get_resource_last_used_days(tags=tags)
                         empty_role = self._check_resource_and_delete(resource_name='IAM Role', resource_id='RoleName', resource_type='CreateRole', resource=get_role, empty_days=empty_days, days_to_delete_resource=self.DAYS_TO_DELETE_RESOURCE, tags=tags)
                         if empty_role:
-                            zombie_roles.append([empty_role.get('RoleName'), self._get_tag_name_from_tags(tags=tags, tag_name='User'), self._get_policy_value(tags=tags), empty_days])
+                            zombie_roles.append({
+                                'ResourceId': empty_role.get('RoleName'),
+                                'Name': empty_role.get('RoleName'),
+                                'User': self._get_tag_name_from_tags(tags=tags, tag_name='User'),
+                                'Skip': self._get_policy_value(tags=tags),
+                                'Days': empty_days})
                     else:
                         empty_days = 0
                     self._update_resource_tags(resource_id=role_name, tags=tags, left_out_days=empty_days, resource_left_out=role_empty)
             except Exception as err:
                 logger.info(f'Error occur:{role_name}, {err}')
         return zombie_roles
```

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/aws/ip_unattached.py` & `cloud-governance-1.1.98/cloud_governance/policy/aws/ip_unattached.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,17 @@
                                                                  resource_id='AllocationId',
                                                                  resource_type='AllocateAddress',
                                                                  resource=address,
                                                                  empty_days=unused_days,
                                                                  days_to_delete_resource=self.DAYS_TO_DELETE_RESOURCE, tags=tags,
                                                                  extra_purse=eip_cost, delta_cost=delta_cost)
                     if zombie_eip:
-                        zombie_addresses.append([address.get('AllocationId'), self._get_tag_name_from_tags(tags=tags),
-                                                 self._get_tag_name_from_tags(tags=tags, tag_name='User'), address.get('PublicIp'),
-                                                 self._get_policy_value(tags=tags), unused_days])
+                        zombie_addresses.append({'ResourceId': address.get('AllocationId'),
+                                                 'Name': self._get_tag_name_from_tags(tags=tags),
+                                                 'User': self._get_tag_name_from_tags(tags=tags, tag_name='User'),
+                                                 'PublicIp': address.get('PublicIp'),
+                                                 'Skip': self._get_policy_value(tags=tags),
+                                                 'Days': unused_days})
                 else:
                     unused_days = 0
                 self._update_resource_tags(resource_id=address.get('AllocationId'), tags=tags, left_out_days=unused_days, resource_left_out=ip_no_used)
         return zombie_addresses
```

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/aws/monthly_report.py` & `cloud-governance-1.1.98/cloud_governance/policy/aws/monthly_report.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/aws/s3_inactive.py` & `cloud-governance-1.1.98/cloud_governance/policy/aws/s3_inactive.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,14 +45,14 @@
                         empty_days = self._get_resource_last_used_days(tags=tags)
                         bucket_empty = True
                         if not self._get_tag_name_from_tags(tags=tags, tag_name='User'):
                             region = self._s3_client.get_bucket_location(Bucket=bucket_name)['LocationConstraint']
                             self._cloudtrail.set_cloudtrail(region_name=region)
                         empty_bucket = self._check_resource_and_delete(resource_name='S3 Bucket', resource_id='Name', resource_type='CreateBucket', resource=bucket, empty_days=empty_days, days_to_delete_resource=self.DAYS_TO_DELETE_RESOURCE, tags=tags)
                         if empty_bucket:
-                            empty_buckets.append([bucket.get('Name'), self._get_tag_name_from_tags(tags=tags, tag_name='User'), str(bucket.get('CreationDate')), str(empty_days), self._get_policy_value(tags=tags)])
+                            empty_buckets.append({'ResourceId': bucket.get('Name'), 'Name': bucket.get('Name'), 'User': self._get_tag_name_from_tags(tags=tags, tag_name='User'), 'Date': str(bucket.get('CreationDate')), 'Days': str(empty_days), 'Skip': self._get_policy_value(tags=tags)})
                 else:
                     empty_days = 0
                 self._update_resource_tags(resource_id=bucket_name, tags=tags, left_out_days=empty_days, resource_left_out=bucket_empty)
             except Exception as err:
                 logger.info(f'{err}, {bucket.get("Name")}')
         return empty_buckets
```

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/aws/skipped_resources.py` & `cloud-governance-1.1.98/cloud_governance/policy/aws/skipped_resources.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/aws/unused_nat_gateway.py` & `cloud-governance-1.1.98/cloud_governance/policy/aws/unused_nat_gateway.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,16 @@
     def __check_cloud_watch_logs(self, resource_id: str, days: int = UNUSED_DAYS):
         """
         This method returns weather the NatGateway is used in last input days
         :param resource_id:
         :param days:
         :return:
         """
+        if days == 0:
+            days = 1
         end_time = datetime.datetime.utcnow()
         start_time = end_time - datetime.timedelta(days=days)
         response = self._cloudwatch.get_metric_data(start_time=start_time, end_time=end_time, resource_id=resource_id,
                                                     resource_type='NatGatewayId', namespace=self.NAMESPACE,
                                                     metric_names={'ActiveConnectionCount': 'Count'},
                                                     statistic='Average')['MetricDataResults'][0]
         for value in response.get('Values'):
```

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/aws/zombie_cluster_resource.py` & `cloud-governance-1.1.98/cloud_governance/policy/aws/zombie_cluster_resource.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/aws/zombie_snapshots.py` & `cloud-governance-1.1.98/cloud_governance/policy/aws/zombie_snapshots.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,18 +47,19 @@
                                                                           resource_id='SnapshotId',
                                                                           resource_type='CreateSnapshot',
                                                                           resource=snapshot,
                                                                           empty_days=unused_days,
                                                                           days_to_delete_resource=self.DAYS_TO_DELETE_RESOURCE,
                                                                           tags=tags)
                         if zombie_snapshot:
-                            zombie_snapshots.append([snapshot.get('SnapshotId'),
-                                                     self._get_tag_name_from_tags(tags=tags),
-                                                     self._get_tag_name_from_tags(tags=tags, tag_name='User'),
-                                                     f'{str(snapshot.get("VolumeSize"))}Gb',
-                                                     self._get_policy_value(tags=snapshot.get('Tags')), str(unused_days)
-                                                     ])
+                            zombie_snapshots.append({'ResourceId': snapshot.get('SnapshotId'),
+                                                     'Name': self._get_tag_name_from_tags(tags=tags),
+                                                     'User': self._get_tag_name_from_tags(tags=tags, tag_name='User'),
+                                                     'Size': f'{str(snapshot.get("VolumeSize"))}Gb',
+                                                     'Skip': self._get_policy_value(tags=snapshot.get('Tags')),
+                                                     'Days': str(unused_days)
+                            })
                     else:
                         unused_days = 0
                     self._update_resource_tags(resource_id=snapshot_id, tags=tags, left_out_days=unused_days,
                                                resource_left_out=not found)
         return zombie_snapshots
```

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/azure/cost_billing_reports.py` & `cloud-governance-1.1.98/cloud_governance/policy/azure/cost_billing_reports.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/gcp/cost_billing_reports.py` & `cloud-governance-1.1.98/cloud_governance/policy/gcp/cost_billing_reports.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/ibm/cost_billing_reports.py` & `cloud-governance-1.1.98/cloud_governance/policy/ibm/cost_billing_reports.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/ibm/ibm_cost_over_usage.py` & `cloud-governance-1.1.98/cloud_governance/policy/ibm/ibm_cost_over_usage.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/ibm/ibm_cost_report.py` & `cloud-governance-1.1.98/cloud_governance/policy/ibm/ibm_cost_report.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/ibm/tag_baremetal.py` & `cloud-governance-1.1.98/cloud_governance/policy/ibm/tag_baremetal.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/ibm/tag_vm.py` & `cloud-governance-1.1.98/cloud_governance/policy/ibm/tag_vm.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/cost_expenditure/cost_report_policies.py` & `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/cost_expenditure/cost_report_policies.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/cloudtrail_to_dynamodb.py` & `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/cloudtrail_to_dynamodb.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/upload_data_to_dynamodb.py` & `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/upload_data_to_dynamodb.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/tag_cluster/remove_cluster_tags.py` & `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_cluster/remove_cluster_tags.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/tag_cluster/run_tag_cluster_resouces.py` & `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_cluster/run_tag_cluster_resouces.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_operations.py` & `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_resouces.py` & `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_resouces.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/tag_non_cluster/non_cluster_operations.py` & `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_non_cluster/non_cluster_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/tag_non_cluster/remove_non_cluster_tags.py` & `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_non_cluster/remove_non_cluster_tags.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/tag_non_cluster/run_tag_non_cluster_resources.py` & `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_non_cluster/run_tag_non_cluster_resources.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/tag_non_cluster/tag_non_cluster_resources.py` & `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_non_cluster/tag_non_cluster_resources.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/tag_non_cluster/update_na_tag_resources.py` & `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_non_cluster/update_na_tag_resources.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/tag_user/iam_user_tags.py` & `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_user/iam_user_tags.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/tag_user/remove_user_tags.py` & `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_user/remove_user_tags.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/tag_user/run_tag_iam_user.py` & `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_user/run_tag_iam_user.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/tag_user/tag_iam_user.py` & `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_user/tag_iam_user.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_ec2_resources.py` & `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_ec2_resources.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_iam_resources.py` & `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_iam_resources.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_s3_resources.py` & `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_s3_resources.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/zombie_cluster/run_zombie_cluster_resources.py` & `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/zombie_cluster/run_zombie_cluster_resources.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/zombie_cluster/validate_zombies.py` & `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/zombie_cluster/validate_zombies.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/zombie_cluster/zombie_cluster_common_methods.py` & `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/zombie_cluster/zombie_cluster_common_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,15 +185,14 @@
         cluster_delete_days = self.get_tag_name_from_tags(tags=tags, tag_name='ClusterDeleteDays')
         if not cluster_delete_days:
             cluster_delete_days = 1
         else:
             cluster_delete_days = int(cluster_delete_days) + 1
         return cluster_delete_days
 
-    @logger_time_stamp
     def trigger_mail(self, tags: list, resource_id: str, days: int, resources: list, message_type: str):
         """
         This method send triggering mail
         @param message_type:
         @param resources:
         @param days:
         @param tags:
@@ -251,15 +250,14 @@
             if cluster_tag in cluster_left_out_days:
                 if cluster_tag in notify_tag_data:
                     notify_data.setdefault(cluster_tag, []).append({func_name: notify_tag_data[cluster_tag]})
                 if cluster_tag in delete_tag_data:
                     delete_data.setdefault(cluster_tag, []).append({func_name: delete_tag_data[cluster_tag]})
         return notify_data, delete_data, cluster_data
 
-    @logger_time_stamp
     def send_mails_to_cluster_user(self, notify_data: dict, delete_data: dict, cluster_data: dict):
         """
         This method send mail to the user to notify cluster status
         @param cluster_data:
         @param notify_data:
         @param delete_data:
         @return:
@@ -271,15 +269,14 @@
                                   days=self.DAYS_TO_TRIGGER_RESOURCE_MAIL,
                                   resources=resource_ids, message_type='notification')
             for cluster_tag, resource_ids in delete_data.items():
                 self.update_resource_tags(tags=cluster_data[cluster_tag], tag_name='Name', tag_value=cluster_tag)
                 self.trigger_mail(tags=cluster_data[cluster_tag], resource_id=cluster_tag,
                                   days=self.DAYS_TO_DELETE_RESOURCE, resources=resource_ids, message_type='delete')
 
-    @logger_time_stamp
     def _check_zombie_cluster_deleted_days(self, resources: dict, cluster_left_out_days: dict, zombie: str, cluster_tag: str):
         """
         This method check the cluster delete days and return the clusters
         @param resources:
         @param cluster_left_out_days:
         @return:
         """
```

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/run_zombie_non_cluster_policies.py` & `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/run_zombie_non_cluster_policies.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,15 +231,15 @@
                 self._s3_client.delete_bucket(Bucket=resource_id)
             elif self._policy == 'empty_roles':
                 self._iam_client.delete_role(RoleName=resource_id)
             elif self._policy == 'ebs_unattached':
                 self._ec2_client.delete_volume(VolumeId=resource_id)
             elif self._policy == 'ip_unattached':
                 self._ec2_client.release_address(AllocationId=resource_id)
-            elif self._policy == 'nat_gateway_unused':
+            elif self._policy == 'unused_nat_gateway':
                 self._ec2_client.delete_nat_gateway(NatGatewayId=resource_id)
             elif self._policy == 'zombie_snapshots':
                 self._ec2_client.delete_snapshot(SnapshotId=resource_id)
             logger.info(f'{self._policy} deleted: {resource_id}')
         except Exception as err:
             logger.info(f'Exception raised: {err}: {resource_id}')
 
@@ -287,15 +287,15 @@
             if self._get_tag_name_from_tags(tags=tags, tag_name='LastUsedDay') or resource_left_out:
                 tags = self._update_tag_value(tags=tags, tag_name='LastUsedDay', tag_value=str(left_out_days))
                 try:
                     if self._policy == 's3_inactive':
                         self._s3_client.put_bucket_tagging(Bucket=resource_id, Tagging={'TagSet': tags})
                     elif self._policy == 'empty_roles':
                         self._iam_client.tag_role(RoleName=resource_id, Tags=tags)
-                    elif self._policy in ('ip_unattached', 'nat_gateway_unused', 'zombie_snapshots'):
+                    elif self._policy in ('ip_unattached', 'unused_nat_gateway', 'zombie_snapshots'):
                         self._ec2_client.create_tags(Resources=[resource_id], Tags=tags)
                 except Exception as err:
                     logger.info(f'Exception raised: {err}: {resource_id}')
 
     def _organise_instance_data(self, resources: list):
         """
         This method convert all datetime into string
```

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/zombie_non_cluster_polices.py` & `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/zombie_non_cluster_polices.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,12 +23,12 @@
                 response = cls[1]().run()
                 if isinstance(response, str):
                     logger.info(f'key: {cls[0]}, Response: {response}')
                 else:
                     logger.info(f'key: {cls[0]}, count: {len(response)}, {response}')
                     policy_result = response
                     if self._policy_output:
-                        if self._policy not in ('ec2_idle', 'ebs_in_use', 'ec2_run', 'unused_nat_gateway'):
-                            beautify_data = self._beautify_upload_data(upload_resource_data=response)
-                            policy_result = {'count': len(beautify_data), self._policy: beautify_data}
+                        # if self._policy not in ('ec2_idle', 'ebs_in_use', 'ec2_run', 's3_inactive', 'zombie_snapshots', 'nat_gateway_unused'):
+                        #     beautify_data = self._beautify_upload_data(upload_resource_data=response)
+                        #     policy_result = {'count': len(beautify_data), self._policy: beautify_data}
                         logger.info(policy_result)
                         self._s3operations.save_results_to_s3(policy=self._policy.replace('_', '-'), policy_output=self._policy_output, policy_result=policy_result)
```

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/policy_operations/azure/azure_policy_runner.py` & `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/azure/azure_policy_runner.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/policy_operations/gcp/gcp_policy_runner.py` & `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/gcp/gcp_policy_runner.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/policy_operations/gitleaks/gitleaks.py` & `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/gitleaks/gitleaks.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_operations.py` & `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_policy_runner.py` & `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_policy_runner.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance/policy/policy_operations/ibm/tagging/tagging_operations.py` & `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/ibm/tagging/tagging_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/cloud_governance.egg-info/PKG-INFO` & `cloud-governance-1.1.98/cloud_governance.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-governance
-Version: 1.1.97
+Version: 1.1.98
 Summary: Cloud Governance Tool
 Home-page: https://github.com/redhat-performance/cloud-governance
 Author: Red Hat
 Author-email: ebattat@redhat.com, athiruma@redhat.com
 License: Apache License 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cloud-governance-1.1.97/cloud_governance.egg-info/SOURCES.txt` & `cloud-governance-1.1.98/cloud_governance.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -81,14 +81,15 @@
 cloud_governance/common/tool/__init__.py
 cloud_governance/common/tool/tool.py
 cloud_governance/main/__init__.py
 cloud_governance/main/environment_variables.py
 cloud_governance/main/environment_variables_exceptions.py
 cloud_governance/main/es_uploader.py
 cloud_governance/main/main.py
+cloud_governance/main/main_common_operations.py
 cloud_governance/policy/__init__.py
 cloud_governance/policy/aws/__init__.py
 cloud_governance/policy/aws/cost_billing_reports.py
 cloud_governance/policy/aws/cost_explorer.py
 cloud_governance/policy/aws/cost_explorer_payer_billings.py
 cloud_governance/policy/aws/cost_over_usage.py
 cloud_governance/policy/aws/ebs_in_use.py
@@ -102,14 +103,16 @@
 cloud_governance/policy/aws/s3_inactive.py
 cloud_governance/policy/aws/skipped_resources.py
 cloud_governance/policy/aws/unused_nat_gateway.py
 cloud_governance/policy/aws/zombie_cluster_resource.py
 cloud_governance/policy/aws/zombie_snapshots.py
 cloud_governance/policy/azure/__init__.py
 cloud_governance/policy/azure/cost_billing_reports.py
+cloud_governance/policy/common_policies/__init__.py
+cloud_governance/policy/common_policies/send_aggregated_alerts.py
 cloud_governance/policy/gcp/__init__.py
 cloud_governance/policy/gcp/cost_billing_reports.py
 cloud_governance/policy/ibm/__init__.py
 cloud_governance/policy/ibm/cost_billing_reports.py
 cloud_governance/policy/ibm/ibm_cost_over_usage.py
 cloud_governance/policy/ibm/ibm_cost_report.py
 cloud_governance/policy/ibm/tag_baremetal.py
@@ -154,8 +157,10 @@
 cloud_governance/policy/policy_operations/gitleaks/__init__.py
 cloud_governance/policy/policy_operations/gitleaks/gitleaks.py
 cloud_governance/policy/policy_operations/ibm/__init__.py
 cloud_governance/policy/policy_operations/ibm/ibm_operations/__init__.py
 cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_operations.py
 cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_policy_runner.py
 cloud_governance/policy/policy_operations/ibm/tagging/__init__.py
-cloud_governance/policy/policy_operations/ibm/tagging/tagging_operations.py
+cloud_governance/policy/policy_operations/ibm/tagging/tagging_operations.py
+cloud_governance/policy/policy_runners/__init__.py
+cloud_governance/policy/policy_runners/common_policy_runner.py
```

### Comparing `cloud-governance-1.1.97/cloud_governance.egg-info/requires.txt` & `cloud-governance-1.1.98/cloud_governance.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.97/setup.py` & `cloud-governance-1.1.98/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from codecs import open
 from os import path
 from setuptools import setup, find_packages
 
 
-__version__ = '1.1.97'
+__version__ = '1.1.98'
 
 
 here = path.abspath(path.dirname(__file__))
 
 
 if path.isfile(path.join(here, 'README.md')):
     with open(path.join(here, 'README.md'), encoding='utf-8') as f:
```

