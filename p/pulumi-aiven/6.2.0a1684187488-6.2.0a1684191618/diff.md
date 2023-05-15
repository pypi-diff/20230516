# Comparing `tmp/pulumi_aiven-6.2.0a1684187488.tar.gz` & `tmp/pulumi_aiven-6.2.0a1684191618.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_aiven-6.2.0a1684187488.tar", last modified: Mon May 15 21:56:01 2023, max compression
+gzip compressed data, was "pulumi_aiven-6.2.0a1684191618.tar", last modified: Mon May 15 23:04:58 2023, max compression
```

## Comparing `pulumi_aiven-6.2.0a1684187488.tar` & `pulumi_aiven-6.2.0a1684191618.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:56:01.262941 pulumi_aiven-6.2.0a1684187488/
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-15 21:56:01.262941 pulumi_aiven-6.2.0a1684187488/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:56:01.262941 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/
--rw-r--r--   0 runner    (1001) docker     (123)    14532 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   596286 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    14130 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/account.py
--rw-r--r--   0 runner    (1001) docker     (123)    36913 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/account_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/account_team.py
--rw-r--r--   0 runner    (1001) docker     (123)    17027 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/account_team_member.py
--rw-r--r--   0 runner    (1001) docker     (123)    12601 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/account_team_project.py
--rw-r--r--   0 runner    (1001) docker     (123)    15297 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/aws_privatelink.py
--rw-r--r--   0 runner    (1001) docker     (123)    18483 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/aws_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    18159 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/azure_privatelink.py
--rw-r--r--   0 runner    (1001) docker     (123)    15298 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/azure_privatelink_connection_approval.py
--rw-r--r--   0 runner    (1001) docker     (123)    24958 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/azure_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    29700 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/billing_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    73507 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/cassandra.py
--rw-r--r--   0 runner    (1001) docker     (123)    19136 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/cassandra_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    73170 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (123)    17227 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/clickhouse_database.py
--rw-r--r--   0 runner    (1001) docker     (123)    26602 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/clickhouse_grant.py
--rw-r--r--   0 runner    (1001) docker     (123)    13649 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/clickhouse_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    16414 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/clickhouse_user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:56:01.262941 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    26197 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    73192 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/flink.py
--rw-r--r--   0 runner    (1001) docker     (123)    17471 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/flink_application.py
--rw-r--r--   0 runner    (1001) docker     (123)    30205 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/flink_application_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15247 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/gcp_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    12455 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_account_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_account_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_account_team_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_account_team_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_aws_privatelink.py
--rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_aws_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7847 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_azure_privatelink.py
--rw-r--r--   0 runner    (1001) docker     (123)    10842 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_azure_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9636 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_billing_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    21868 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_cassanda.py
--rw-r--r--   0 runner    (1001) docker     (123)    21536 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_cassandra.py
--rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_cassandra_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    21612 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_clickhouse_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     7467 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_clickhouse_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     9126 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    21292 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_flink.py
--rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_flink_application.py
--rw-r--r--   0 runner    (1001) docker     (123)    11003 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_flink_application_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_gcp_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    21396 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_grafana.py
--rw-r--r--   0 runner    (1001) docker     (123)    21473 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_influx_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_influxdb_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_influxdb_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    22261 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_kafka_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)    21768 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_kafka_connect.py
--rw-r--r--   0 runner    (1001) docker     (123)    10310 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_kafka_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    22037 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_kafka_mirror_maker.py
--rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_kafka_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_kafka_schema_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_kafka_schema_registry_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_kafka_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7982 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_kafka_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    21715 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_m3_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21228 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_m3_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_m3db_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_mirror_maker_replication_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    21304 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_my_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     6836 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_mysql_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_mysql_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    21605 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_open_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_open_search_acl_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_open_search_acl_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_opensearch_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    21117 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_pg.py
--rw-r--r--   0 runner    (1001) docker     (123)     7965 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_pg_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_pg_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_project_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_project_vpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    21271 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_redis_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_service_component.py
--rw-r--r--   0 runner    (1001) docker     (123)    17872 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_service_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    15737 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_service_integration_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_transit_gateway_vpc_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)    74761 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/grafana.py
--rw-r--r--   0 runner    (1001) docker     (123)    73222 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/influx_db.py
--rw-r--r--   0 runner    (1001) docker     (123)    16389 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/influxdb_database.py
--rw-r--r--   0 runner    (1001) docker     (123)    19094 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/influxdb_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    78050 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)    20003 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/kafka_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)    76154 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/kafka_connect.py
--rw-r--r--   0 runner    (1001) docker     (123)    24756 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/kafka_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    76710 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/kafka_mirror_maker.py
--rw-r--r--   0 runner    (1001) docker     (123)    22353 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/kafka_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    14423 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/kafka_schema_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    19784 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/kafka_schema_registry_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)    24119 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/kafka_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)    18632 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/kafka_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    75554 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/m3_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)    74440 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/m3_db.py
--rw-r--r--   0 runner    (1001) docker     (123)    16448 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/m3db_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    37020 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/mirror_maker_replication_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    75063 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/my_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)    17313 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/mysql_database.py
--rw-r--r--   0 runner    (1001) docker     (123)    21287 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/mysql_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    74183 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/open_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    18457 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/open_search_acl_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    22319 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/open_search_acl_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    16700 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/opensearch_user.py
--rw-r--r--   0 runner    (1001) docker     (123)   892539 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    71601 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/pg.py
--rw-r--r--   0 runner    (1001) docker     (123)    22840 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/pg_database.py
--rw-r--r--   0 runner    (1001) docker     (123)    21818 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/pg_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    39073 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    13742 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/project_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/project_vpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    74559 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)    29938 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/redis_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    53125 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/service_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    53402 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/service_integration_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    14185 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/static_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)    22097 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven/transit_gateway_vpc_attachment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:56:01.262941 pulumi_aiven-6.2.0a1684187488/pulumi_aiven.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-15 21:56:01.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-05-15 21:56:01.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 21:56:01.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 21:56:01.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-15 21:56:01.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-15 21:56:01.000000 pulumi_aiven-6.2.0a1684187488/pulumi_aiven.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 21:56:01.262941 pulumi_aiven-6.2.0a1684187488/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-15 21:56:00.000000 pulumi_aiven-6.2.0a1684187488/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:04:58.661153 pulumi_aiven-6.2.0a1684191618/
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-15 23:04:58.661153 pulumi_aiven-6.2.0a1684191618/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:04:58.661153 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/
+-rw-r--r--   0 runner    (1001) docker     (123)    14532 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   594789 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14130 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36913 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/account_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/account_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17027 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/account_team_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12601 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/account_team_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15297 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/aws_privatelink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18483 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/aws_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18159 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/azure_privatelink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15298 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/azure_privatelink_connection_approval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24958 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/azure_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29700 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/billing_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74463 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/cassandra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19426 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/cassandra_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74126 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17227 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/clickhouse_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26558 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/clickhouse_grant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13649 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/clickhouse_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16426 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/clickhouse_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:04:58.661153 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26197 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74148 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/flink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17471 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/flink_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30205 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/flink_application_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15247 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/gcp_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12455 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_account_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_account_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_account_team_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_account_team_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_aws_privatelink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8722 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_aws_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_azure_privatelink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10842 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_azure_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9636 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_billing_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21970 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_cassanda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21638 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_cassandra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_cassandra_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21714 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_clickhouse_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7663 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_clickhouse_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21394 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_flink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_flink_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_flink_application_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_gcp_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21498 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_grafana.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21575 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_influx_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_influxdb_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_influxdb_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22363 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8889 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_kafka_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21870 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_kafka_connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10488 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_kafka_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22139 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_kafka_mirror_maker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_kafka_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_kafka_schema_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_kafka_schema_registry_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_kafka_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7982 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_kafka_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21817 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_m3_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21330 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_m3_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_m3db_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13264 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_mirror_maker_replication_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21406 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_my_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_mysql_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_mysql_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21707 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_open_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_open_search_acl_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8824 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_open_search_acl_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_opensearch_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21219 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_pg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_pg_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_pg_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_project_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_project_vpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21373 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_redis_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10493 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_service_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17978 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_service_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15415 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_service_integration_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_transit_gateway_vpc_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75717 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/grafana.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74178 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/influx_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16389 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/influxdb_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19380 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/influxdb_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79009 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20003 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/kafka_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77110 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/kafka_connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24756 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/kafka_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77666 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/kafka_mirror_maker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22353 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/kafka_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14423 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/kafka_schema_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19784 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/kafka_schema_registry_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24119 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/kafka_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18906 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/kafka_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76510 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/m3_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75396 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/m3_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16718 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/m3db_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37020 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/mirror_maker_replication_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76019 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/my_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17313 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/mysql_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21561 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/mysql_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75139 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/open_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18457 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/open_search_acl_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22685 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/open_search_acl_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16994 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/opensearch_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)   890191 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72557 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/pg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22840 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/pg_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21818 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/pg_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39073 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13742 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/project_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/project_vpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    75515 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30212 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/redis_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53125 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/service_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52318 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/service_integration_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14185 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/static_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22097 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven/transit_gateway_vpc_attachment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:04:58.661153 pulumi_aiven-6.2.0a1684191618/pulumi_aiven.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/pulumi_aiven.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 23:04:58.661153 pulumi_aiven-6.2.0a1684191618/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-15 23:04:58.000000 pulumi_aiven-6.2.0a1684191618/setup.py
```

### Comparing `pulumi_aiven-6.2.0a1684187488/PKG-INFO` & `pulumi_aiven-6.2.0a1684191618/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_aiven
-Version: 6.2.0a1684187488
+Version: 6.2.0a1684191618
 Summary: A Pulumi package for creating and managing Aiven cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-aiven
 Keywords: pulumi aiven
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_aiven-6.2.0a1684187488/README.md` & `pulumi_aiven-6.2.0a1684191618/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/__init__.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/_inputs.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/_inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,14 +140,15 @@
     'OpenSearchOpensearchUserConfigIndexTemplateArgs',
     'OpenSearchOpensearchUserConfigIpFilterObjectArgs',
     'OpenSearchOpensearchUserConfigOpensearchArgs',
     'OpenSearchOpensearchUserConfigOpensearchDashboardsArgs',
     'OpenSearchOpensearchUserConfigPrivateAccessArgs',
     'OpenSearchOpensearchUserConfigPrivatelinkAccessArgs',
     'OpenSearchOpensearchUserConfigPublicAccessArgs',
+    'OpenSearchOpensearchUserConfigSamlArgs',
     'OpenSearchServiceIntegrationArgs',
     'OpenSearchTagArgs',
     'PgComponentArgs',
     'PgPgArgs',
     'PgPgUserConfigArgs',
     'PgPgUserConfigIpFilterObjectArgs',
     'PgPgUserConfigMigrationArgs',
@@ -188,15 +189,14 @@
     'ServiceIntegrationEndpointExternalGoogleCloudLoggingUserConfigArgs',
     'ServiceIntegrationEndpointExternalKafkaUserConfigArgs',
     'ServiceIntegrationEndpointExternalOpensearchLogsUserConfigArgs',
     'ServiceIntegrationEndpointExternalSchemaRegistryUserConfigArgs',
     'ServiceIntegrationEndpointJolokiaUserConfigArgs',
     'ServiceIntegrationEndpointPrometheusUserConfigArgs',
     'ServiceIntegrationEndpointRsyslogUserConfigArgs',
-    'ServiceIntegrationEndpointSignalfxUserConfigArgs',
     'ServiceIntegrationExternalAwsCloudwatchMetricsUserConfigArgs',
     'ServiceIntegrationExternalAwsCloudwatchMetricsUserConfigDroppedMetricArgs',
     'ServiceIntegrationExternalAwsCloudwatchMetricsUserConfigExtraMetricArgs',
     'ServiceIntegrationKafkaConnectUserConfigArgs',
     'ServiceIntegrationKafkaConnectUserConfigKafkaConnectArgs',
     'ServiceIntegrationKafkaLogsUserConfigArgs',
     'ServiceIntegrationKafkaMirrormakerUserConfigArgs',
@@ -4262,86 +4262,64 @@
 class KafkaKafkaArgs:
     def __init__(__self__, *,
                  access_cert: Optional[pulumi.Input[str]] = None,
                  access_key: Optional[pulumi.Input[str]] = None,
                  connect_uri: Optional[pulumi.Input[str]] = None,
                  rest_uri: Optional[pulumi.Input[str]] = None,
                  schema_registry_uri: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] access_cert: The Kafka client certificate
-        :param pulumi.Input[str] access_key: The Kafka client certificate key
-        :param pulumi.Input[str] connect_uri: The Kafka Connect URI, if any
-        :param pulumi.Input[str] rest_uri: The Kafka REST URI, if any
-        :param pulumi.Input[str] schema_registry_uri: The Schema Registry URI, if any
-        """
         if access_cert is not None:
             pulumi.set(__self__, "access_cert", access_cert)
         if access_key is not None:
             pulumi.set(__self__, "access_key", access_key)
         if connect_uri is not None:
             pulumi.set(__self__, "connect_uri", connect_uri)
         if rest_uri is not None:
             pulumi.set(__self__, "rest_uri", rest_uri)
         if schema_registry_uri is not None:
             pulumi.set(__self__, "schema_registry_uri", schema_registry_uri)
 
     @property
     @pulumi.getter(name="accessCert")
     def access_cert(self) -> Optional[pulumi.Input[str]]:
-        """
-        The Kafka client certificate
-        """
         return pulumi.get(self, "access_cert")
 
     @access_cert.setter
     def access_cert(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "access_cert", value)
 
     @property
     @pulumi.getter(name="accessKey")
     def access_key(self) -> Optional[pulumi.Input[str]]:
-        """
-        The Kafka client certificate key
-        """
         return pulumi.get(self, "access_key")
 
     @access_key.setter
     def access_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "access_key", value)
 
     @property
     @pulumi.getter(name="connectUri")
     def connect_uri(self) -> Optional[pulumi.Input[str]]:
-        """
-        The Kafka Connect URI, if any
-        """
         return pulumi.get(self, "connect_uri")
 
     @connect_uri.setter
     def connect_uri(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "connect_uri", value)
 
     @property
     @pulumi.getter(name="restUri")
     def rest_uri(self) -> Optional[pulumi.Input[str]]:
-        """
-        The Kafka REST URI, if any
-        """
         return pulumi.get(self, "rest_uri")
 
     @rest_uri.setter
     def rest_uri(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "rest_uri", value)
 
     @property
     @pulumi.getter(name="schemaRegistryUri")
     def schema_registry_uri(self) -> Optional[pulumi.Input[str]]:
-        """
-        The Schema Registry URI, if any
-        """
         return pulumi.get(self, "schema_registry_uri")
 
     @schema_registry_uri.setter
     def schema_registry_uri(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "schema_registry_uri", value)
 
 
@@ -8879,14 +8857,15 @@
                  opensearch_dashboards: Optional[pulumi.Input['OpenSearchOpensearchUserConfigOpensearchDashboardsArgs']] = None,
                  opensearch_version: Optional[pulumi.Input[str]] = None,
                  private_access: Optional[pulumi.Input['OpenSearchOpensearchUserConfigPrivateAccessArgs']] = None,
                  privatelink_access: Optional[pulumi.Input['OpenSearchOpensearchUserConfigPrivatelinkAccessArgs']] = None,
                  project_to_fork_from: Optional[pulumi.Input[str]] = None,
                  public_access: Optional[pulumi.Input['OpenSearchOpensearchUserConfigPublicAccessArgs']] = None,
                  recovery_basebackup_name: Optional[pulumi.Input[str]] = None,
+                 saml: Optional[pulumi.Input['OpenSearchOpensearchUserConfigSamlArgs']] = None,
                  service_to_fork_from: Optional[pulumi.Input[str]] = None,
                  static_ips: Optional[pulumi.Input[bool]] = None):
         """
         :param pulumi.Input[str] additional_backup_regions: Additional Cloud Regions for Backup Replication.
         :param pulumi.Input[str] custom_domain: Serve the web frontend using a custom CNAME pointing to the Aiven DNS name.
         :param pulumi.Input[bool] disable_replication_factor_adjustment: Disable automatic replication factor adjustment for multi-node services. By default, Aiven ensures all indexes are replicated at least to two nodes. Note: Due to potential data loss in case of losing a service node, this setting can no longer be activated.
         :param pulumi.Input[Sequence[pulumi.Input['OpenSearchOpensearchUserConfigIndexPatternArgs']]] index_patterns: Index patterns.
@@ -8900,14 +8879,15 @@
         :param pulumi.Input['OpenSearchOpensearchUserConfigOpensearchDashboardsArgs'] opensearch_dashboards: OpenSearch Dashboards settings.
         :param pulumi.Input[str] opensearch_version: OpenSearch major version.
         :param pulumi.Input['OpenSearchOpensearchUserConfigPrivateAccessArgs'] private_access: Allow access to selected service ports from private networks.
         :param pulumi.Input['OpenSearchOpensearchUserConfigPrivatelinkAccessArgs'] privatelink_access: Allow access to selected service components through Privatelink.
         :param pulumi.Input[str] project_to_fork_from: Name of another project to fork a service from. This has effect only when a new service is being created.
         :param pulumi.Input['OpenSearchOpensearchUserConfigPublicAccessArgs'] public_access: Allow access to selected service ports from the public Internet.
         :param pulumi.Input[str] recovery_basebackup_name: Name of the basebackup to restore in forked service.
+        :param pulumi.Input['OpenSearchOpensearchUserConfigSamlArgs'] saml: OpenSearch SAML configuration.
         :param pulumi.Input[str] service_to_fork_from: Name of another service to fork from. This has effect only when a new service is being created.
         :param pulumi.Input[bool] static_ips: Use static public IP addresses.
         """
         if additional_backup_regions is not None:
             pulumi.set(__self__, "additional_backup_regions", additional_backup_regions)
         if custom_domain is not None:
             pulumi.set(__self__, "custom_domain", custom_domain)
@@ -8948,14 +8928,16 @@
             pulumi.set(__self__, "privatelink_access", privatelink_access)
         if project_to_fork_from is not None:
             pulumi.set(__self__, "project_to_fork_from", project_to_fork_from)
         if public_access is not None:
             pulumi.set(__self__, "public_access", public_access)
         if recovery_basebackup_name is not None:
             pulumi.set(__self__, "recovery_basebackup_name", recovery_basebackup_name)
+        if saml is not None:
+            pulumi.set(__self__, "saml", saml)
         if service_to_fork_from is not None:
             pulumi.set(__self__, "service_to_fork_from", service_to_fork_from)
         if static_ips is not None:
             pulumi.set(__self__, "static_ips", static_ips)
 
     @property
     @pulumi.getter(name="additionalBackupRegions")
@@ -9170,14 +9152,26 @@
         return pulumi.get(self, "recovery_basebackup_name")
 
     @recovery_basebackup_name.setter
     def recovery_basebackup_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "recovery_basebackup_name", value)
 
     @property
+    @pulumi.getter
+    def saml(self) -> Optional[pulumi.Input['OpenSearchOpensearchUserConfigSamlArgs']]:
+        """
+        OpenSearch SAML configuration.
+        """
+        return pulumi.get(self, "saml")
+
+    @saml.setter
+    def saml(self, value: Optional[pulumi.Input['OpenSearchOpensearchUserConfigSamlArgs']]):
+        pulumi.set(self, "saml", value)
+
+    @property
     @pulumi.getter(name="serviceToForkFrom")
     def service_to_fork_from(self) -> Optional[pulumi.Input[str]]:
         """
         Name of another service to fork from. This has effect only when a new service is being created.
         """
         return pulumi.get(self, "service_to_fork_from")
 
@@ -9862,14 +9856,87 @@
 
     @prometheus.setter
     def prometheus(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "prometheus", value)
 
 
 @pulumi.input_type
+class OpenSearchOpensearchUserConfigSamlArgs:
+    def __init__(__self__, *,
+                 enabled: pulumi.Input[bool],
+                 idp_entity_id: pulumi.Input[str],
+                 idp_metadata_url: pulumi.Input[str],
+                 sp_entity_id: pulumi.Input[str],
+                 roles_key: Optional[pulumi.Input[str]] = None,
+                 subject_key: Optional[pulumi.Input[str]] = None):
+        pulumi.set(__self__, "enabled", enabled)
+        pulumi.set(__self__, "idp_entity_id", idp_entity_id)
+        pulumi.set(__self__, "idp_metadata_url", idp_metadata_url)
+        pulumi.set(__self__, "sp_entity_id", sp_entity_id)
+        if roles_key is not None:
+            pulumi.set(__self__, "roles_key", roles_key)
+        if subject_key is not None:
+            pulumi.set(__self__, "subject_key", subject_key)
+
+    @property
+    @pulumi.getter
+    def enabled(self) -> pulumi.Input[bool]:
+        return pulumi.get(self, "enabled")
+
+    @enabled.setter
+    def enabled(self, value: pulumi.Input[bool]):
+        pulumi.set(self, "enabled", value)
+
+    @property
+    @pulumi.getter(name="idpEntityId")
+    def idp_entity_id(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "idp_entity_id")
+
+    @idp_entity_id.setter
+    def idp_entity_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "idp_entity_id", value)
+
+    @property
+    @pulumi.getter(name="idpMetadataUrl")
+    def idp_metadata_url(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "idp_metadata_url")
+
+    @idp_metadata_url.setter
+    def idp_metadata_url(self, value: pulumi.Input[str]):
+        pulumi.set(self, "idp_metadata_url", value)
+
+    @property
+    @pulumi.getter(name="spEntityId")
+    def sp_entity_id(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "sp_entity_id")
+
+    @sp_entity_id.setter
+    def sp_entity_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "sp_entity_id", value)
+
+    @property
+    @pulumi.getter(name="rolesKey")
+    def roles_key(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "roles_key")
+
+    @roles_key.setter
+    def roles_key(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "roles_key", value)
+
+    @property
+    @pulumi.getter(name="subjectKey")
+    def subject_key(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "subject_key")
+
+    @subject_key.setter
+    def subject_key(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subject_key", value)
+
+
+@pulumi.input_type
 class OpenSearchServiceIntegrationArgs:
     def __init__(__self__, *,
                  integration_type: pulumi.Input[str],
                  source_service_name: pulumi.Input[str]):
         """
         :param pulumi.Input[str] integration_type: Type of the service integration. The only supported value at the moment is `read_replica`
         :param pulumi.Input[str] source_service_name: Name of the source service
@@ -12824,15 +12891,15 @@
     def pshard_stats_enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "pshard_stats_enabled", value)
 
 
 @pulumi.input_type
 class ServiceIntegrationEndpointDatadogUserConfigArgs:
     def __init__(__self__, *,
-                 datadog_api_key: Optional[pulumi.Input[str]] = None,
+                 datadog_api_key: pulumi.Input[str],
                  datadog_tags: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceIntegrationEndpointDatadogUserConfigDatadogTagArgs']]]] = None,
                  disable_consumer_stats: Optional[pulumi.Input[bool]] = None,
                  kafka_consumer_check_instances: Optional[pulumi.Input[int]] = None,
                  kafka_consumer_stats_timeout: Optional[pulumi.Input[int]] = None,
                  max_partition_contexts: Optional[pulumi.Input[int]] = None,
                  site: Optional[pulumi.Input[str]] = None):
         """
@@ -12840,16 +12907,15 @@
         :param pulumi.Input[Sequence[pulumi.Input['ServiceIntegrationEndpointDatadogUserConfigDatadogTagArgs']]] datadog_tags: Custom tags provided by user.
         :param pulumi.Input[bool] disable_consumer_stats: Disable consumer group metrics.
         :param pulumi.Input[int] kafka_consumer_check_instances: Number of separate instances to fetch kafka consumer statistics with.
         :param pulumi.Input[int] kafka_consumer_stats_timeout: Number of seconds that datadog will wait to get consumer statistics from brokers.
         :param pulumi.Input[int] max_partition_contexts: Maximum number of partition contexts to send.
         :param pulumi.Input[str] site: Datadog intake site. Defaults to datadoghq.com.
         """
-        if datadog_api_key is not None:
-            pulumi.set(__self__, "datadog_api_key", datadog_api_key)
+        pulumi.set(__self__, "datadog_api_key", datadog_api_key)
         if datadog_tags is not None:
             pulumi.set(__self__, "datadog_tags", datadog_tags)
         if disable_consumer_stats is not None:
             pulumi.set(__self__, "disable_consumer_stats", disable_consumer_stats)
         if kafka_consumer_check_instances is not None:
             pulumi.set(__self__, "kafka_consumer_check_instances", kafka_consumer_check_instances)
         if kafka_consumer_stats_timeout is not None:
@@ -12857,22 +12923,22 @@
         if max_partition_contexts is not None:
             pulumi.set(__self__, "max_partition_contexts", max_partition_contexts)
         if site is not None:
             pulumi.set(__self__, "site", site)
 
     @property
     @pulumi.getter(name="datadogApiKey")
-    def datadog_api_key(self) -> Optional[pulumi.Input[str]]:
+    def datadog_api_key(self) -> pulumi.Input[str]:
         """
         Datadog API key.
         """
         return pulumi.get(self, "datadog_api_key")
 
     @datadog_api_key.setter
-    def datadog_api_key(self, value: Optional[pulumi.Input[str]]):
+    def datadog_api_key(self, value: pulumi.Input[str]):
         pulumi.set(self, "datadog_api_key", value)
 
     @property
     @pulumi.getter(name="datadogTags")
     def datadog_tags(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ServiceIntegrationEndpointDatadogUserConfigDatadogTagArgs']]]]:
         """
         Custom tags provided by user.
@@ -12971,178 +13037,193 @@
     def comment(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "comment", value)
 
 
 @pulumi.input_type
 class ServiceIntegrationEndpointExternalAwsCloudwatchLogsUserConfigArgs:
     def __init__(__self__, *,
-                 access_key: Optional[pulumi.Input[str]] = None,
-                 log_group_name: Optional[pulumi.Input[str]] = None,
-                 region: Optional[pulumi.Input[str]] = None,
-                 secret_key: Optional[pulumi.Input[str]] = None):
+                 access_key: pulumi.Input[str],
+                 region: pulumi.Input[str],
+                 secret_key: pulumi.Input[str],
+                 log_group_name: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] access_key: AWS access key. Required permissions are logs:CreateLogGroup, logs:CreateLogStream, logs:PutLogEvents and logs:DescribeLogStreams.
-        :param pulumi.Input[str] log_group_name: AWS CloudWatch log group name.
         :param pulumi.Input[str] region: AWS region.
         :param pulumi.Input[str] secret_key: AWS secret key.
+        :param pulumi.Input[str] log_group_name: AWS CloudWatch log group name.
         """
-        if access_key is not None:
-            pulumi.set(__self__, "access_key", access_key)
+        pulumi.set(__self__, "access_key", access_key)
+        pulumi.set(__self__, "region", region)
+        pulumi.set(__self__, "secret_key", secret_key)
         if log_group_name is not None:
             pulumi.set(__self__, "log_group_name", log_group_name)
-        if region is not None:
-            pulumi.set(__self__, "region", region)
-        if secret_key is not None:
-            pulumi.set(__self__, "secret_key", secret_key)
 
     @property
     @pulumi.getter(name="accessKey")
-    def access_key(self) -> Optional[pulumi.Input[str]]:
+    def access_key(self) -> pulumi.Input[str]:
         """
         AWS access key. Required permissions are logs:CreateLogGroup, logs:CreateLogStream, logs:PutLogEvents and logs:DescribeLogStreams.
         """
         return pulumi.get(self, "access_key")
 
     @access_key.setter
-    def access_key(self, value: Optional[pulumi.Input[str]]):
+    def access_key(self, value: pulumi.Input[str]):
         pulumi.set(self, "access_key", value)
 
     @property
-    @pulumi.getter(name="logGroupName")
-    def log_group_name(self) -> Optional[pulumi.Input[str]]:
-        """
-        AWS CloudWatch log group name.
-        """
-        return pulumi.get(self, "log_group_name")
-
-    @log_group_name.setter
-    def log_group_name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "log_group_name", value)
-
-    @property
     @pulumi.getter
-    def region(self) -> Optional[pulumi.Input[str]]:
+    def region(self) -> pulumi.Input[str]:
         """
         AWS region.
         """
         return pulumi.get(self, "region")
 
     @region.setter
-    def region(self, value: Optional[pulumi.Input[str]]):
+    def region(self, value: pulumi.Input[str]):
         pulumi.set(self, "region", value)
 
     @property
     @pulumi.getter(name="secretKey")
-    def secret_key(self) -> Optional[pulumi.Input[str]]:
+    def secret_key(self) -> pulumi.Input[str]:
         """
         AWS secret key.
         """
         return pulumi.get(self, "secret_key")
 
     @secret_key.setter
-    def secret_key(self, value: Optional[pulumi.Input[str]]):
+    def secret_key(self, value: pulumi.Input[str]):
         pulumi.set(self, "secret_key", value)
 
+    @property
+    @pulumi.getter(name="logGroupName")
+    def log_group_name(self) -> Optional[pulumi.Input[str]]:
+        """
+        AWS CloudWatch log group name.
+        """
+        return pulumi.get(self, "log_group_name")
+
+    @log_group_name.setter
+    def log_group_name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "log_group_name", value)
+
 
 @pulumi.input_type
 class ServiceIntegrationEndpointExternalAwsCloudwatchMetricsUserConfigArgs:
     def __init__(__self__, *,
-                 access_key: Optional[pulumi.Input[str]] = None,
-                 namespace: Optional[pulumi.Input[str]] = None,
-                 region: Optional[pulumi.Input[str]] = None,
-                 secret_key: Optional[pulumi.Input[str]] = None):
+                 access_key: pulumi.Input[str],
+                 namespace: pulumi.Input[str],
+                 region: pulumi.Input[str],
+                 secret_key: pulumi.Input[str]):
         """
         :param pulumi.Input[str] access_key: AWS access key. Required permissions are cloudwatch:PutMetricData.
         :param pulumi.Input[str] namespace: AWS CloudWatch Metrics Namespace.
         :param pulumi.Input[str] region: AWS region.
         :param pulumi.Input[str] secret_key: AWS secret key.
         """
-        if access_key is not None:
-            pulumi.set(__self__, "access_key", access_key)
-        if namespace is not None:
-            pulumi.set(__self__, "namespace", namespace)
-        if region is not None:
-            pulumi.set(__self__, "region", region)
-        if secret_key is not None:
-            pulumi.set(__self__, "secret_key", secret_key)
+        pulumi.set(__self__, "access_key", access_key)
+        pulumi.set(__self__, "namespace", namespace)
+        pulumi.set(__self__, "region", region)
+        pulumi.set(__self__, "secret_key", secret_key)
 
     @property
     @pulumi.getter(name="accessKey")
-    def access_key(self) -> Optional[pulumi.Input[str]]:
+    def access_key(self) -> pulumi.Input[str]:
         """
         AWS access key. Required permissions are cloudwatch:PutMetricData.
         """
         return pulumi.get(self, "access_key")
 
     @access_key.setter
-    def access_key(self, value: Optional[pulumi.Input[str]]):
+    def access_key(self, value: pulumi.Input[str]):
         pulumi.set(self, "access_key", value)
 
     @property
     @pulumi.getter
-    def namespace(self) -> Optional[pulumi.Input[str]]:
+    def namespace(self) -> pulumi.Input[str]:
         """
         AWS CloudWatch Metrics Namespace.
         """
         return pulumi.get(self, "namespace")
 
     @namespace.setter
-    def namespace(self, value: Optional[pulumi.Input[str]]):
+    def namespace(self, value: pulumi.Input[str]):
         pulumi.set(self, "namespace", value)
 
     @property
     @pulumi.getter
-    def region(self) -> Optional[pulumi.Input[str]]:
+    def region(self) -> pulumi.Input[str]:
         """
         AWS region.
         """
         return pulumi.get(self, "region")
 
     @region.setter
-    def region(self, value: Optional[pulumi.Input[str]]):
+    def region(self, value: pulumi.Input[str]):
         pulumi.set(self, "region", value)
 
     @property
     @pulumi.getter(name="secretKey")
-    def secret_key(self) -> Optional[pulumi.Input[str]]:
+    def secret_key(self) -> pulumi.Input[str]:
         """
         AWS secret key.
         """
         return pulumi.get(self, "secret_key")
 
     @secret_key.setter
-    def secret_key(self, value: Optional[pulumi.Input[str]]):
+    def secret_key(self, value: pulumi.Input[str]):
         pulumi.set(self, "secret_key", value)
 
 
 @pulumi.input_type
 class ServiceIntegrationEndpointExternalElasticsearchLogsUserConfigArgs:
     def __init__(__self__, *,
+                 index_prefix: pulumi.Input[str],
+                 url: pulumi.Input[str],
                  ca: Optional[pulumi.Input[str]] = None,
                  index_days_max: Optional[pulumi.Input[int]] = None,
-                 index_prefix: Optional[pulumi.Input[str]] = None,
-                 timeout: Optional[pulumi.Input[float]] = None,
-                 url: Optional[pulumi.Input[str]] = None):
+                 timeout: Optional[pulumi.Input[float]] = None):
         """
+        :param pulumi.Input[str] index_prefix: Elasticsearch index prefix. The default value is `logs`.
+        :param pulumi.Input[str] url: Elasticsearch connection URL.
         :param pulumi.Input[str] ca: PEM encoded CA certificate.
         :param pulumi.Input[int] index_days_max: Maximum number of days of logs to keep. The default value is `3`.
-        :param pulumi.Input[str] index_prefix: Elasticsearch index prefix. The default value is `logs`.
         :param pulumi.Input[float] timeout: Elasticsearch request timeout limit. The default value is `10.0`.
-        :param pulumi.Input[str] url: Elasticsearch connection URL.
         """
+        pulumi.set(__self__, "index_prefix", index_prefix)
+        pulumi.set(__self__, "url", url)
         if ca is not None:
             pulumi.set(__self__, "ca", ca)
         if index_days_max is not None:
             pulumi.set(__self__, "index_days_max", index_days_max)
-        if index_prefix is not None:
-            pulumi.set(__self__, "index_prefix", index_prefix)
         if timeout is not None:
             pulumi.set(__self__, "timeout", timeout)
-        if url is not None:
-            pulumi.set(__self__, "url", url)
+
+    @property
+    @pulumi.getter(name="indexPrefix")
+    def index_prefix(self) -> pulumi.Input[str]:
+        """
+        Elasticsearch index prefix. The default value is `logs`.
+        """
+        return pulumi.get(self, "index_prefix")
+
+    @index_prefix.setter
+    def index_prefix(self, value: pulumi.Input[str]):
+        pulumi.set(self, "index_prefix", value)
+
+    @property
+    @pulumi.getter
+    def url(self) -> pulumi.Input[str]:
+        """
+        Elasticsearch connection URL.
+        """
+        return pulumi.get(self, "url")
+
+    @url.setter
+    def url(self, value: pulumi.Input[str]):
+        pulumi.set(self, "url", value)
 
     @property
     @pulumi.getter
     def ca(self) -> Optional[pulumi.Input[str]]:
         """
         PEM encoded CA certificate.
         """
@@ -13161,160 +13242,143 @@
         return pulumi.get(self, "index_days_max")
 
     @index_days_max.setter
     def index_days_max(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "index_days_max", value)
 
     @property
-    @pulumi.getter(name="indexPrefix")
-    def index_prefix(self) -> Optional[pulumi.Input[str]]:
-        """
-        Elasticsearch index prefix. The default value is `logs`.
-        """
-        return pulumi.get(self, "index_prefix")
-
-    @index_prefix.setter
-    def index_prefix(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "index_prefix", value)
-
-    @property
     @pulumi.getter
     def timeout(self) -> Optional[pulumi.Input[float]]:
         """
         Elasticsearch request timeout limit. The default value is `10.0`.
         """
         return pulumi.get(self, "timeout")
 
     @timeout.setter
     def timeout(self, value: Optional[pulumi.Input[float]]):
         pulumi.set(self, "timeout", value)
 
-    @property
-    @pulumi.getter
-    def url(self) -> Optional[pulumi.Input[str]]:
-        """
-        Elasticsearch connection URL.
-        """
-        return pulumi.get(self, "url")
-
-    @url.setter
-    def url(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "url", value)
-
 
 @pulumi.input_type
 class ServiceIntegrationEndpointExternalGoogleCloudLoggingUserConfigArgs:
     def __init__(__self__, *,
-                 log_id: Optional[pulumi.Input[str]] = None,
-                 project_id: Optional[pulumi.Input[str]] = None,
-                 service_account_credentials: Optional[pulumi.Input[str]] = None):
+                 log_id: pulumi.Input[str],
+                 project_id: pulumi.Input[str],
+                 service_account_credentials: pulumi.Input[str]):
         """
         :param pulumi.Input[str] log_id: Google Cloud Logging log id.
         :param pulumi.Input[str] project_id: GCP project id.
         :param pulumi.Input[str] service_account_credentials: This is a JSON object with the fields documented in https://cloud.google.com/iam/docs/creating-managing-service-account-keys .
         """
-        if log_id is not None:
-            pulumi.set(__self__, "log_id", log_id)
-        if project_id is not None:
-            pulumi.set(__self__, "project_id", project_id)
-        if service_account_credentials is not None:
-            pulumi.set(__self__, "service_account_credentials", service_account_credentials)
+        pulumi.set(__self__, "log_id", log_id)
+        pulumi.set(__self__, "project_id", project_id)
+        pulumi.set(__self__, "service_account_credentials", service_account_credentials)
 
     @property
     @pulumi.getter(name="logId")
-    def log_id(self) -> Optional[pulumi.Input[str]]:
+    def log_id(self) -> pulumi.Input[str]:
         """
         Google Cloud Logging log id.
         """
         return pulumi.get(self, "log_id")
 
     @log_id.setter
-    def log_id(self, value: Optional[pulumi.Input[str]]):
+    def log_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "log_id", value)
 
     @property
     @pulumi.getter(name="projectId")
-    def project_id(self) -> Optional[pulumi.Input[str]]:
+    def project_id(self) -> pulumi.Input[str]:
         """
         GCP project id.
         """
         return pulumi.get(self, "project_id")
 
     @project_id.setter
-    def project_id(self, value: Optional[pulumi.Input[str]]):
+    def project_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "project_id", value)
 
     @property
     @pulumi.getter(name="serviceAccountCredentials")
-    def service_account_credentials(self) -> Optional[pulumi.Input[str]]:
+    def service_account_credentials(self) -> pulumi.Input[str]:
         """
         This is a JSON object with the fields documented in https://cloud.google.com/iam/docs/creating-managing-service-account-keys .
         """
         return pulumi.get(self, "service_account_credentials")
 
     @service_account_credentials.setter
-    def service_account_credentials(self, value: Optional[pulumi.Input[str]]):
+    def service_account_credentials(self, value: pulumi.Input[str]):
         pulumi.set(self, "service_account_credentials", value)
 
 
 @pulumi.input_type
 class ServiceIntegrationEndpointExternalKafkaUserConfigArgs:
     def __init__(__self__, *,
-                 bootstrap_servers: Optional[pulumi.Input[str]] = None,
+                 bootstrap_servers: pulumi.Input[str],
+                 security_protocol: pulumi.Input[str],
                  sasl_mechanism: Optional[pulumi.Input[str]] = None,
                  sasl_plain_password: Optional[pulumi.Input[str]] = None,
                  sasl_plain_username: Optional[pulumi.Input[str]] = None,
-                 security_protocol: Optional[pulumi.Input[str]] = None,
                  ssl_ca_cert: Optional[pulumi.Input[str]] = None,
                  ssl_client_cert: Optional[pulumi.Input[str]] = None,
                  ssl_client_key: Optional[pulumi.Input[str]] = None,
                  ssl_endpoint_identification_algorithm: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] bootstrap_servers: Bootstrap servers.
+        :param pulumi.Input[str] security_protocol: Security protocol.
         :param pulumi.Input[str] sasl_mechanism: The list of SASL mechanisms enabled in the Kafka server.
         :param pulumi.Input[str] sasl_plain_password: Password for SASL PLAIN mechanism in the Kafka server.
         :param pulumi.Input[str] sasl_plain_username: Username for SASL PLAIN mechanism in the Kafka server.
-        :param pulumi.Input[str] security_protocol: Security protocol.
         :param pulumi.Input[str] ssl_ca_cert: PEM-encoded CA certificate.
         :param pulumi.Input[str] ssl_client_cert: PEM-encoded client certificate.
         :param pulumi.Input[str] ssl_client_key: PEM-encoded client key.
         :param pulumi.Input[str] ssl_endpoint_identification_algorithm: The endpoint identification algorithm to validate server hostname using server certificate.
         """
-        if bootstrap_servers is not None:
-            pulumi.set(__self__, "bootstrap_servers", bootstrap_servers)
+        pulumi.set(__self__, "bootstrap_servers", bootstrap_servers)
+        pulumi.set(__self__, "security_protocol", security_protocol)
         if sasl_mechanism is not None:
             pulumi.set(__self__, "sasl_mechanism", sasl_mechanism)
         if sasl_plain_password is not None:
             pulumi.set(__self__, "sasl_plain_password", sasl_plain_password)
         if sasl_plain_username is not None:
             pulumi.set(__self__, "sasl_plain_username", sasl_plain_username)
-        if security_protocol is not None:
-            pulumi.set(__self__, "security_protocol", security_protocol)
         if ssl_ca_cert is not None:
             pulumi.set(__self__, "ssl_ca_cert", ssl_ca_cert)
         if ssl_client_cert is not None:
             pulumi.set(__self__, "ssl_client_cert", ssl_client_cert)
         if ssl_client_key is not None:
             pulumi.set(__self__, "ssl_client_key", ssl_client_key)
         if ssl_endpoint_identification_algorithm is not None:
             pulumi.set(__self__, "ssl_endpoint_identification_algorithm", ssl_endpoint_identification_algorithm)
 
     @property
     @pulumi.getter(name="bootstrapServers")
-    def bootstrap_servers(self) -> Optional[pulumi.Input[str]]:
+    def bootstrap_servers(self) -> pulumi.Input[str]:
         """
         Bootstrap servers.
         """
         return pulumi.get(self, "bootstrap_servers")
 
     @bootstrap_servers.setter
-    def bootstrap_servers(self, value: Optional[pulumi.Input[str]]):
+    def bootstrap_servers(self, value: pulumi.Input[str]):
         pulumi.set(self, "bootstrap_servers", value)
 
     @property
+    @pulumi.getter(name="securityProtocol")
+    def security_protocol(self) -> pulumi.Input[str]:
+        """
+        Security protocol.
+        """
+        return pulumi.get(self, "security_protocol")
+
+    @security_protocol.setter
+    def security_protocol(self, value: pulumi.Input[str]):
+        pulumi.set(self, "security_protocol", value)
+
+    @property
     @pulumi.getter(name="saslMechanism")
     def sasl_mechanism(self) -> Optional[pulumi.Input[str]]:
         """
         The list of SASL mechanisms enabled in the Kafka server.
         """
         return pulumi.get(self, "sasl_mechanism")
 
@@ -13343,26 +13407,14 @@
         return pulumi.get(self, "sasl_plain_username")
 
     @sasl_plain_username.setter
     def sasl_plain_username(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "sasl_plain_username", value)
 
     @property
-    @pulumi.getter(name="securityProtocol")
-    def security_protocol(self) -> Optional[pulumi.Input[str]]:
-        """
-        Security protocol.
-        """
-        return pulumi.get(self, "security_protocol")
-
-    @security_protocol.setter
-    def security_protocol(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "security_protocol", value)
-
-    @property
     @pulumi.getter(name="sslCaCert")
     def ssl_ca_cert(self) -> Optional[pulumi.Input[str]]:
         """
         PEM-encoded CA certificate.
         """
         return pulumi.get(self, "ssl_ca_cert")
 
@@ -13406,36 +13458,58 @@
     def ssl_endpoint_identification_algorithm(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ssl_endpoint_identification_algorithm", value)
 
 
 @pulumi.input_type
 class ServiceIntegrationEndpointExternalOpensearchLogsUserConfigArgs:
     def __init__(__self__, *,
+                 index_prefix: pulumi.Input[str],
+                 url: pulumi.Input[str],
                  ca: Optional[pulumi.Input[str]] = None,
                  index_days_max: Optional[pulumi.Input[int]] = None,
-                 index_prefix: Optional[pulumi.Input[str]] = None,
-                 timeout: Optional[pulumi.Input[float]] = None,
-                 url: Optional[pulumi.Input[str]] = None):
+                 timeout: Optional[pulumi.Input[float]] = None):
         """
+        :param pulumi.Input[str] index_prefix: OpenSearch index prefix. The default value is `logs`.
+        :param pulumi.Input[str] url: OpenSearch connection URL.
         :param pulumi.Input[str] ca: PEM encoded CA certificate.
         :param pulumi.Input[int] index_days_max: Maximum number of days of logs to keep. The default value is `3`.
-        :param pulumi.Input[str] index_prefix: OpenSearch index prefix. The default value is `logs`.
         :param pulumi.Input[float] timeout: OpenSearch request timeout limit. The default value is `10.0`.
-        :param pulumi.Input[str] url: OpenSearch connection URL.
         """
+        pulumi.set(__self__, "index_prefix", index_prefix)
+        pulumi.set(__self__, "url", url)
         if ca is not None:
             pulumi.set(__self__, "ca", ca)
         if index_days_max is not None:
             pulumi.set(__self__, "index_days_max", index_days_max)
-        if index_prefix is not None:
-            pulumi.set(__self__, "index_prefix", index_prefix)
         if timeout is not None:
             pulumi.set(__self__, "timeout", timeout)
-        if url is not None:
-            pulumi.set(__self__, "url", url)
+
+    @property
+    @pulumi.getter(name="indexPrefix")
+    def index_prefix(self) -> pulumi.Input[str]:
+        """
+        OpenSearch index prefix. The default value is `logs`.
+        """
+        return pulumi.get(self, "index_prefix")
+
+    @index_prefix.setter
+    def index_prefix(self, value: pulumi.Input[str]):
+        pulumi.set(self, "index_prefix", value)
+
+    @property
+    @pulumi.getter
+    def url(self) -> pulumi.Input[str]:
+        """
+        OpenSearch connection URL.
+        """
+        return pulumi.get(self, "url")
+
+    @url.setter
+    def url(self, value: pulumi.Input[str]):
+        pulumi.set(self, "url", value)
 
     @property
     @pulumi.getter
     def ca(self) -> Optional[pulumi.Input[str]]:
         """
         PEM encoded CA certificate.
         """
@@ -13454,85 +13528,71 @@
         return pulumi.get(self, "index_days_max")
 
     @index_days_max.setter
     def index_days_max(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "index_days_max", value)
 
     @property
-    @pulumi.getter(name="indexPrefix")
-    def index_prefix(self) -> Optional[pulumi.Input[str]]:
-        """
-        OpenSearch index prefix. The default value is `logs`.
-        """
-        return pulumi.get(self, "index_prefix")
-
-    @index_prefix.setter
-    def index_prefix(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "index_prefix", value)
-
-    @property
     @pulumi.getter
     def timeout(self) -> Optional[pulumi.Input[float]]:
         """
         OpenSearch request timeout limit. The default value is `10.0`.
         """
         return pulumi.get(self, "timeout")
 
     @timeout.setter
     def timeout(self, value: Optional[pulumi.Input[float]]):
         pulumi.set(self, "timeout", value)
 
-    @property
-    @pulumi.getter
-    def url(self) -> Optional[pulumi.Input[str]]:
-        """
-        OpenSearch connection URL.
-        """
-        return pulumi.get(self, "url")
-
-    @url.setter
-    def url(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "url", value)
-
 
 @pulumi.input_type
 class ServiceIntegrationEndpointExternalSchemaRegistryUserConfigArgs:
     def __init__(__self__, *,
-                 authentication: Optional[pulumi.Input[str]] = None,
+                 authentication: pulumi.Input[str],
+                 url: pulumi.Input[str],
                  basic_auth_password: Optional[pulumi.Input[str]] = None,
-                 basic_auth_username: Optional[pulumi.Input[str]] = None,
-                 url: Optional[pulumi.Input[str]] = None):
+                 basic_auth_username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] authentication: Authentication method.
+        :param pulumi.Input[str] url: Schema Registry URL.
         :param pulumi.Input[str] basic_auth_password: Basic authentication password.
         :param pulumi.Input[str] basic_auth_username: Basic authentication user name.
-        :param pulumi.Input[str] url: Schema Registry URL.
         """
-        if authentication is not None:
-            pulumi.set(__self__, "authentication", authentication)
+        pulumi.set(__self__, "authentication", authentication)
+        pulumi.set(__self__, "url", url)
         if basic_auth_password is not None:
             pulumi.set(__self__, "basic_auth_password", basic_auth_password)
         if basic_auth_username is not None:
             pulumi.set(__self__, "basic_auth_username", basic_auth_username)
-        if url is not None:
-            pulumi.set(__self__, "url", url)
 
     @property
     @pulumi.getter
-    def authentication(self) -> Optional[pulumi.Input[str]]:
+    def authentication(self) -> pulumi.Input[str]:
         """
         Authentication method.
         """
         return pulumi.get(self, "authentication")
 
     @authentication.setter
-    def authentication(self, value: Optional[pulumi.Input[str]]):
+    def authentication(self, value: pulumi.Input[str]):
         pulumi.set(self, "authentication", value)
 
     @property
+    @pulumi.getter
+    def url(self) -> pulumi.Input[str]:
+        """
+        Schema Registry URL.
+        """
+        return pulumi.get(self, "url")
+
+    @url.setter
+    def url(self, value: pulumi.Input[str]):
+        pulumi.set(self, "url", value)
+
+    @property
     @pulumi.getter(name="basicAuthPassword")
     def basic_auth_password(self) -> Optional[pulumi.Input[str]]:
         """
         Basic authentication password.
         """
         return pulumi.get(self, "basic_auth_password")
 
@@ -13548,26 +13608,14 @@
         """
         return pulumi.get(self, "basic_auth_username")
 
     @basic_auth_username.setter
     def basic_auth_username(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "basic_auth_username", value)
 
-    @property
-    @pulumi.getter
-    def url(self) -> Optional[pulumi.Input[str]]:
-        """
-        Schema Registry URL.
-        """
-        return pulumi.get(self, "url")
-
-    @url.setter
-    def url(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "url", value)
-
 
 @pulumi.input_type
 class ServiceIntegrationEndpointJolokiaUserConfigArgs:
     def __init__(__self__, *,
                  basic_auth_password: Optional[pulumi.Input[str]] = None,
                  basic_auth_username: Optional[pulumi.Input[str]] = None):
         """
@@ -13642,52 +13690,96 @@
     def basic_auth_username(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "basic_auth_username", value)
 
 
 @pulumi.input_type
 class ServiceIntegrationEndpointRsyslogUserConfigArgs:
     def __init__(__self__, *,
+                 format: pulumi.Input[str],
+                 port: pulumi.Input[int],
+                 server: pulumi.Input[str],
+                 tls: pulumi.Input[bool],
                  ca: Optional[pulumi.Input[str]] = None,
                  cert: Optional[pulumi.Input[str]] = None,
-                 format: Optional[pulumi.Input[str]] = None,
                  key: Optional[pulumi.Input[str]] = None,
                  logline: Optional[pulumi.Input[str]] = None,
-                 port: Optional[pulumi.Input[int]] = None,
-                 sd: Optional[pulumi.Input[str]] = None,
-                 server: Optional[pulumi.Input[str]] = None,
-                 tls: Optional[pulumi.Input[bool]] = None):
+                 sd: Optional[pulumi.Input[str]] = None):
         """
+        :param pulumi.Input[str] format: message format. The default value is `rfc5424`.
+        :param pulumi.Input[int] port: rsyslog server port. The default value is `514`.
+        :param pulumi.Input[str] server: rsyslog server IP address or hostname.
+        :param pulumi.Input[bool] tls: Require TLS. The default value is `true`.
         :param pulumi.Input[str] ca: PEM encoded CA certificate.
         :param pulumi.Input[str] cert: PEM encoded client certificate.
-        :param pulumi.Input[str] format: message format. The default value is `rfc5424`.
         :param pulumi.Input[str] key: PEM encoded client key.
         :param pulumi.Input[str] logline: custom syslog message format.
-        :param pulumi.Input[int] port: rsyslog server port. The default value is `514`.
         :param pulumi.Input[str] sd: Structured data block for log message.
-        :param pulumi.Input[str] server: rsyslog server IP address or hostname.
-        :param pulumi.Input[bool] tls: Require TLS. The default value is `true`.
         """
+        pulumi.set(__self__, "format", format)
+        pulumi.set(__self__, "port", port)
+        pulumi.set(__self__, "server", server)
+        pulumi.set(__self__, "tls", tls)
         if ca is not None:
             pulumi.set(__self__, "ca", ca)
         if cert is not None:
             pulumi.set(__self__, "cert", cert)
-        if format is not None:
-            pulumi.set(__self__, "format", format)
         if key is not None:
             pulumi.set(__self__, "key", key)
         if logline is not None:
             pulumi.set(__self__, "logline", logline)
-        if port is not None:
-            pulumi.set(__self__, "port", port)
         if sd is not None:
             pulumi.set(__self__, "sd", sd)
-        if server is not None:
-            pulumi.set(__self__, "server", server)
-        if tls is not None:
-            pulumi.set(__self__, "tls", tls)
+
+    @property
+    @pulumi.getter
+    def format(self) -> pulumi.Input[str]:
+        """
+        message format. The default value is `rfc5424`.
+        """
+        return pulumi.get(self, "format")
+
+    @format.setter
+    def format(self, value: pulumi.Input[str]):
+        pulumi.set(self, "format", value)
+
+    @property
+    @pulumi.getter
+    def port(self) -> pulumi.Input[int]:
+        """
+        rsyslog server port. The default value is `514`.
+        """
+        return pulumi.get(self, "port")
+
+    @port.setter
+    def port(self, value: pulumi.Input[int]):
+        pulumi.set(self, "port", value)
+
+    @property
+    @pulumi.getter
+    def server(self) -> pulumi.Input[str]:
+        """
+        rsyslog server IP address or hostname.
+        """
+        return pulumi.get(self, "server")
+
+    @server.setter
+    def server(self, value: pulumi.Input[str]):
+        pulumi.set(self, "server", value)
+
+    @property
+    @pulumi.getter
+    def tls(self) -> pulumi.Input[bool]:
+        """
+        Require TLS. The default value is `true`.
+        """
+        return pulumi.get(self, "tls")
+
+    @tls.setter
+    def tls(self, value: pulumi.Input[bool]):
+        pulumi.set(self, "tls", value)
 
     @property
     @pulumi.getter
     def ca(self) -> Optional[pulumi.Input[str]]:
         """
         PEM encoded CA certificate.
         """
@@ -13707,26 +13799,14 @@
 
     @cert.setter
     def cert(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cert", value)
 
     @property
     @pulumi.getter
-    def format(self) -> Optional[pulumi.Input[str]]:
-        """
-        message format. The default value is `rfc5424`.
-        """
-        return pulumi.get(self, "format")
-
-    @format.setter
-    def format(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "format", value)
-
-    @property
-    @pulumi.getter
     def key(self) -> Optional[pulumi.Input[str]]:
         """
         PEM encoded client key.
         """
         return pulumi.get(self, "key")
 
     @key.setter
@@ -13743,115 +13823,24 @@
 
     @logline.setter
     def logline(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "logline", value)
 
     @property
     @pulumi.getter
-    def port(self) -> Optional[pulumi.Input[int]]:
-        """
-        rsyslog server port. The default value is `514`.
-        """
-        return pulumi.get(self, "port")
-
-    @port.setter
-    def port(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "port", value)
-
-    @property
-    @pulumi.getter
     def sd(self) -> Optional[pulumi.Input[str]]:
         """
         Structured data block for log message.
         """
         return pulumi.get(self, "sd")
 
     @sd.setter
     def sd(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "sd", value)
 
-    @property
-    @pulumi.getter
-    def server(self) -> Optional[pulumi.Input[str]]:
-        """
-        rsyslog server IP address or hostname.
-        """
-        return pulumi.get(self, "server")
-
-    @server.setter
-    def server(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "server", value)
-
-    @property
-    @pulumi.getter
-    def tls(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Require TLS. The default value is `true`.
-        """
-        return pulumi.get(self, "tls")
-
-    @tls.setter
-    def tls(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "tls", value)
-
-
-@pulumi.input_type
-class ServiceIntegrationEndpointSignalfxUserConfigArgs:
-    def __init__(__self__, *,
-                 enabled_metrics: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 signalfx_api_key: Optional[pulumi.Input[str]] = None,
-                 signalfx_realm: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] enabled_metrics: list of metrics to send.
-        :param pulumi.Input[str] signalfx_api_key: SignalFX API key.
-        :param pulumi.Input[str] signalfx_realm: SignalFX realm. The default value is `us0`.
-        """
-        if enabled_metrics is not None:
-            pulumi.set(__self__, "enabled_metrics", enabled_metrics)
-        if signalfx_api_key is not None:
-            pulumi.set(__self__, "signalfx_api_key", signalfx_api_key)
-        if signalfx_realm is not None:
-            pulumi.set(__self__, "signalfx_realm", signalfx_realm)
-
-    @property
-    @pulumi.getter(name="enabledMetrics")
-    def enabled_metrics(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        list of metrics to send.
-        """
-        return pulumi.get(self, "enabled_metrics")
-
-    @enabled_metrics.setter
-    def enabled_metrics(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "enabled_metrics", value)
-
-    @property
-    @pulumi.getter(name="signalfxApiKey")
-    def signalfx_api_key(self) -> Optional[pulumi.Input[str]]:
-        """
-        SignalFX API key.
-        """
-        return pulumi.get(self, "signalfx_api_key")
-
-    @signalfx_api_key.setter
-    def signalfx_api_key(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "signalfx_api_key", value)
-
-    @property
-    @pulumi.getter(name="signalfxRealm")
-    def signalfx_realm(self) -> Optional[pulumi.Input[str]]:
-        """
-        SignalFX realm. The default value is `us0`.
-        """
-        return pulumi.get(self, "signalfx_realm")
-
-    @signalfx_realm.setter
-    def signalfx_realm(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "signalfx_realm", value)
-
 
 @pulumi.input_type
 class ServiceIntegrationExternalAwsCloudwatchMetricsUserConfigArgs:
     def __init__(__self__, *,
                  dropped_metrics: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceIntegrationExternalAwsCloudwatchMetricsUserConfigDroppedMetricArgs']]]] = None,
                  extra_metrics: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceIntegrationExternalAwsCloudwatchMetricsUserConfigExtraMetricArgs']]]] = None):
         """
@@ -14017,31 +14006,30 @@
     def status_storage_topic(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "status_storage_topic", value)
 
 
 @pulumi.input_type
 class ServiceIntegrationKafkaLogsUserConfigArgs:
     def __init__(__self__, *,
-                 kafka_topic: Optional[pulumi.Input[str]] = None):
+                 kafka_topic: pulumi.Input[str]):
         """
         :param pulumi.Input[str] kafka_topic: Topic name.
         """
-        if kafka_topic is not None:
-            pulumi.set(__self__, "kafka_topic", kafka_topic)
+        pulumi.set(__self__, "kafka_topic", kafka_topic)
 
     @property
     @pulumi.getter(name="kafkaTopic")
-    def kafka_topic(self) -> Optional[pulumi.Input[str]]:
+    def kafka_topic(self) -> pulumi.Input[str]:
         """
         Topic name.
         """
         return pulumi.get(self, "kafka_topic")
 
     @kafka_topic.setter
-    def kafka_topic(self, value: Optional[pulumi.Input[str]]):
+    def kafka_topic(self, value: pulumi.Input[str]):
         pulumi.set(self, "kafka_topic", value)
 
 
 @pulumi.input_type
 class ServiceIntegrationKafkaMirrormakerUserConfigArgs:
     def __init__(__self__, *,
                  cluster_alias: Optional[pulumi.Input[str]] = None,
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/_utilities.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/account.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/account.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/account_authentication.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/account_authentication.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/account_team.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/account_team.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/account_team_member.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/account_team_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/account_team_project.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/account_team_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/aws_privatelink.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/aws_privatelink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/aws_vpc_peering_connection.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/aws_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/azure_privatelink.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/azure_privatelink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/azure_privatelink_connection_approval.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/azure_privatelink_connection_approval.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/azure_vpc_peering_connection.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/azure_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/billing_group.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/billing_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/cassandra.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/cassandra.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,17 @@
         if additional_disk_space is not None:
             pulumi.set(__self__, "additional_disk_space", additional_disk_space)
         if cassandra_user_config is not None:
             pulumi.set(__self__, "cassandra_user_config", cassandra_user_config)
         if cloud_name is not None:
             pulumi.set(__self__, "cloud_name", cloud_name)
         if disk_space is not None:
+            warnings.warn("""This will be removed in v5.0.0 and replaced with additional_disk_space instead.""", DeprecationWarning)
+            pulumi.log.warn("""disk_space is deprecated: This will be removed in v5.0.0 and replaced with additional_disk_space instead.""")
+        if disk_space is not None:
             pulumi.set(__self__, "disk_space", disk_space)
         if maintenance_window_dow is not None:
             pulumi.set(__self__, "maintenance_window_dow", maintenance_window_dow)
         if maintenance_window_time is not None:
             pulumi.set(__self__, "maintenance_window_time", maintenance_window_time)
         if plan is not None:
             pulumi.set(__self__, "plan", plan)
@@ -310,14 +313,17 @@
         if cassandras is not None:
             pulumi.set(__self__, "cassandras", cassandras)
         if cloud_name is not None:
             pulumi.set(__self__, "cloud_name", cloud_name)
         if components is not None:
             pulumi.set(__self__, "components", components)
         if disk_space is not None:
+            warnings.warn("""This will be removed in v5.0.0 and replaced with additional_disk_space instead.""", DeprecationWarning)
+            pulumi.log.warn("""disk_space is deprecated: This will be removed in v5.0.0 and replaced with additional_disk_space instead.""")
+        if disk_space is not None:
             pulumi.set(__self__, "disk_space", disk_space)
         if disk_space_cap is not None:
             pulumi.set(__self__, "disk_space_cap", disk_space_cap)
         if disk_space_default is not None:
             pulumi.set(__self__, "disk_space_default", disk_space_default)
         if disk_space_step is not None:
             pulumi.set(__self__, "disk_space_step", disk_space_step)
@@ -823,14 +829,17 @@
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = CassandraArgs.__new__(CassandraArgs)
 
             __props__.__dict__["additional_disk_space"] = additional_disk_space
             __props__.__dict__["cassandra_user_config"] = cassandra_user_config
             __props__.__dict__["cloud_name"] = cloud_name
+            if disk_space is not None and not opts.urn:
+                warnings.warn("""This will be removed in v5.0.0 and replaced with additional_disk_space instead.""", DeprecationWarning)
+                pulumi.log.warn("""disk_space is deprecated: This will be removed in v5.0.0 and replaced with additional_disk_space instead.""")
             __props__.__dict__["disk_space"] = disk_space
             __props__.__dict__["maintenance_window_dow"] = maintenance_window_dow
             __props__.__dict__["maintenance_window_time"] = maintenance_window_time
             __props__.__dict__["plan"] = plan
             if project is None and not opts.urn:
                 raise TypeError("Missing required property 'project'")
             __props__.__dict__["project"] = project
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/cassandra_user.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/cassandra_user.py`

 * *Files 4% similar despite different names*

```diff
@@ -222,14 +222,20 @@
         foo = aiven.CassandraUser("foo",
             service_name=aiven_cassandra["bar"]["service_name"],
             project="my-project",
             username="user-1",
             password="Test$1234")
         ```
 
+        ## Import
+
+        ```sh
+         $ pulumi import aiven:index/cassandraUser:CassandraUser foo project/service_name/username
+        ```
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] password: The password of the Cassandra User.
         :param pulumi.Input[str] project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] username: The actual name of the Cassandra User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
@@ -251,14 +257,20 @@
         foo = aiven.CassandraUser("foo",
             service_name=aiven_cassandra["bar"]["service_name"],
             project="my-project",
             username="user-1",
             password="Test$1234")
         ```
 
+        ## Import
+
+        ```sh
+         $ pulumi import aiven:index/cassandraUser:CassandraUser foo project/service_name/username
+        ```
+
         :param str resource_name: The name of the resource.
         :param CassandraUserArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(CassandraUserArgs, pulumi.ResourceOptions, *args, **kwargs)
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/clickhouse.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/clickhouse.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,17 @@
         if additional_disk_space is not None:
             pulumi.set(__self__, "additional_disk_space", additional_disk_space)
         if clickhouse_user_config is not None:
             pulumi.set(__self__, "clickhouse_user_config", clickhouse_user_config)
         if cloud_name is not None:
             pulumi.set(__self__, "cloud_name", cloud_name)
         if disk_space is not None:
+            warnings.warn("""This will be removed in v5.0.0 and replaced with additional_disk_space instead.""", DeprecationWarning)
+            pulumi.log.warn("""disk_space is deprecated: This will be removed in v5.0.0 and replaced with additional_disk_space instead.""")
+        if disk_space is not None:
             pulumi.set(__self__, "disk_space", disk_space)
         if maintenance_window_dow is not None:
             pulumi.set(__self__, "maintenance_window_dow", maintenance_window_dow)
         if maintenance_window_time is not None:
             pulumi.set(__self__, "maintenance_window_time", maintenance_window_time)
         if plan is not None:
             pulumi.set(__self__, "plan", plan)
@@ -310,14 +313,17 @@
         if clickhouses is not None:
             pulumi.set(__self__, "clickhouses", clickhouses)
         if cloud_name is not None:
             pulumi.set(__self__, "cloud_name", cloud_name)
         if components is not None:
             pulumi.set(__self__, "components", components)
         if disk_space is not None:
+            warnings.warn("""This will be removed in v5.0.0 and replaced with additional_disk_space instead.""", DeprecationWarning)
+            pulumi.log.warn("""disk_space is deprecated: This will be removed in v5.0.0 and replaced with additional_disk_space instead.""")
+        if disk_space is not None:
             pulumi.set(__self__, "disk_space", disk_space)
         if disk_space_cap is not None:
             pulumi.set(__self__, "disk_space_cap", disk_space_cap)
         if disk_space_default is not None:
             pulumi.set(__self__, "disk_space_default", disk_space_default)
         if disk_space_step is not None:
             pulumi.set(__self__, "disk_space_step", disk_space_step)
@@ -811,14 +817,17 @@
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ClickhouseArgs.__new__(ClickhouseArgs)
 
             __props__.__dict__["additional_disk_space"] = additional_disk_space
             __props__.__dict__["clickhouse_user_config"] = clickhouse_user_config
             __props__.__dict__["cloud_name"] = cloud_name
+            if disk_space is not None and not opts.urn:
+                warnings.warn("""This will be removed in v5.0.0 and replaced with additional_disk_space instead.""", DeprecationWarning)
+                pulumi.log.warn("""disk_space is deprecated: This will be removed in v5.0.0 and replaced with additional_disk_space instead.""")
             __props__.__dict__["disk_space"] = disk_space
             __props__.__dict__["maintenance_window_dow"] = maintenance_window_dow
             __props__.__dict__["maintenance_window_time"] = maintenance_window_time
             __props__.__dict__["plan"] = plan
             if project is None and not opts.urn:
                 raise TypeError("Missing required property 'project'")
             __props__.__dict__["project"] = project
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/clickhouse_database.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/clickhouse_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/clickhouse_grant.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/clickhouse_grant.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,20 +260,19 @@
             project=clickhouse.project,
             service_name=clickhouse.service_name,
             role=demo_clickhouse_role.role,
             privilege_grants=[
                 aiven.ClickhouseGrantPrivilegeGrantArgs(
                     privilege="INSERT",
                     database=demodb.name,
-                    table="*",
+                    table="demo-table",
                 ),
                 aiven.ClickhouseGrantPrivilegeGrantArgs(
                     privilege="SELECT",
                     database=demodb.name,
-                    table="*",
                 ),
             ])
         demo_clickhouse_user = aiven.ClickhouseUser("demoClickhouseUser",
             project=clickhouse.project,
             service_name=clickhouse.service_name,
             username="demo-user")
         demo_user_grant = aiven.ClickhouseGrant("demo-user-grant",
@@ -329,20 +328,19 @@
             project=clickhouse.project,
             service_name=clickhouse.service_name,
             role=demo_clickhouse_role.role,
             privilege_grants=[
                 aiven.ClickhouseGrantPrivilegeGrantArgs(
                     privilege="INSERT",
                     database=demodb.name,
-                    table="*",
+                    table="demo-table",
                 ),
                 aiven.ClickhouseGrantPrivilegeGrantArgs(
                     privilege="SELECT",
                     database=demodb.name,
-                    table="*",
                 ),
             ])
         demo_clickhouse_user = aiven.ClickhouseUser("demoClickhouseUser",
             project=clickhouse.project,
             service_name=clickhouse.service_name,
             username="demo-user")
         demo_user_grant = aiven.ClickhouseGrant("demo-user-grant",
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/clickhouse_role.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/clickhouse_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/clickhouse_user.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/clickhouse_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
             service_name=aiven_clickhouse["myservice"]["service_name"],
             username="<USERNAME>")
         ```
 
         ## Import
 
         ```sh
-         $ pulumi import aiven:index/clickhouseUser:ClickhouseUser ch-user project/service_name/id
+         $ pulumi import aiven:index/clickhouseUser:ClickhouseUser ch-user project/service_name/username
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] username: The actual name of the Clickhouse user. This property cannot be changed, doing so forces recreation of the resource.
@@ -224,15 +224,15 @@
             service_name=aiven_clickhouse["myservice"]["service_name"],
             username="<USERNAME>")
         ```
 
         ## Import
 
         ```sh
-         $ pulumi import aiven:index/clickhouseUser:ClickhouseUser ch-user project/service_name/id
+         $ pulumi import aiven:index/clickhouseUser:ClickhouseUser ch-user project/service_name/username
         ```
 
         :param str resource_name: The name of the resource.
         :param ClickhouseUserArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/config/vars.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/connection_pool.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/connection_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/flink.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/flink.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,17 @@
         pulumi.set(__self__, "project", project)
         pulumi.set(__self__, "service_name", service_name)
         if additional_disk_space is not None:
             pulumi.set(__self__, "additional_disk_space", additional_disk_space)
         if cloud_name is not None:
             pulumi.set(__self__, "cloud_name", cloud_name)
         if disk_space is not None:
+            warnings.warn("""This will be removed in v5.0.0 and replaced with additional_disk_space instead.""", DeprecationWarning)
+            pulumi.log.warn("""disk_space is deprecated: This will be removed in v5.0.0 and replaced with additional_disk_space instead.""")
+        if disk_space is not None:
             pulumi.set(__self__, "disk_space", disk_space)
         if flink is not None:
             pulumi.set(__self__, "flink", flink)
         if flink_user_config is not None:
             pulumi.set(__self__, "flink_user_config", flink_user_config)
         if maintenance_window_dow is not None:
             pulumi.set(__self__, "maintenance_window_dow", maintenance_window_dow)
@@ -322,14 +325,17 @@
         if additional_disk_space is not None:
             pulumi.set(__self__, "additional_disk_space", additional_disk_space)
         if cloud_name is not None:
             pulumi.set(__self__, "cloud_name", cloud_name)
         if components is not None:
             pulumi.set(__self__, "components", components)
         if disk_space is not None:
+            warnings.warn("""This will be removed in v5.0.0 and replaced with additional_disk_space instead.""", DeprecationWarning)
+            pulumi.log.warn("""disk_space is deprecated: This will be removed in v5.0.0 and replaced with additional_disk_space instead.""")
+        if disk_space is not None:
             pulumi.set(__self__, "disk_space", disk_space)
         if disk_space_cap is not None:
             pulumi.set(__self__, "disk_space_cap", disk_space_cap)
         if disk_space_default is not None:
             pulumi.set(__self__, "disk_space_default", disk_space_default)
         if disk_space_step is not None:
             pulumi.set(__self__, "disk_space_step", disk_space_step)
@@ -835,14 +841,17 @@
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = FlinkArgs.__new__(FlinkArgs)
 
             __props__.__dict__["additional_disk_space"] = additional_disk_space
             __props__.__dict__["cloud_name"] = cloud_name
+            if disk_space is not None and not opts.urn:
+                warnings.warn("""This will be removed in v5.0.0 and replaced with additional_disk_space instead.""", DeprecationWarning)
+                pulumi.log.warn("""disk_space is deprecated: This will be removed in v5.0.0 and replaced with additional_disk_space instead.""")
             __props__.__dict__["disk_space"] = disk_space
             __props__.__dict__["flink"] = flink
             __props__.__dict__["flink_user_config"] = flink_user_config
             __props__.__dict__["maintenance_window_dow"] = maintenance_window_dow
             __props__.__dict__["maintenance_window_time"] = maintenance_window_time
             __props__.__dict__["plan"] = plan
             if project is None and not opts.urn:
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/flink_application.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/flink_application.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/flink_application_version.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/flink_application_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/gcp_vpc_peering_connection.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/gcp_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_account.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_account_authentication.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_account_authentication.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_account_team.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_account_team.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_account_team_member.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_account_team_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_account_team_project.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_account_team_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_aws_privatelink.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_aws_privatelink.py`

 * *Files 11% similar despite different names*

```diff
@@ -112,16 +112,16 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    foo = aiven.get_aws_privatelink(project=data["aiven_project"]["foo"]["project"],
-        service_name=aiven_kafka["bar"]["service_name"])
+    foo = aiven.get_aws_privatelink(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference))
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
     __args__ = dict()
@@ -148,16 +148,16 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    foo = aiven.get_aws_privatelink(project=data["aiven_project"]["foo"]["project"],
-        service_name=aiven_kafka["bar"]["service_name"])
+    foo = aiven.get_aws_privatelink(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference))
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
     ...
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_aws_vpc_peering_connection.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_aws_vpc_peering_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,15 +138,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    foo = aiven.get_aws_vpc_peering_connection(vpc_id=data["aiven_project_vpc"]["vpc"]["id"],
+    foo = aiven.get_aws_vpc_peering_connection(vpc_id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         aws_account_id="XXXXX",
         aws_vpc_id="XXXXX")
     ```
 
 
     :param str aws_account_id: AWS account ID. This property cannot be changed, doing so forces recreation of the resource.
     :param str aws_vpc_id: AWS VPC ID. This property cannot be changed, doing so forces recreation of the resource.
@@ -183,15 +183,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    foo = aiven.get_aws_vpc_peering_connection(vpc_id=data["aiven_project_vpc"]["vpc"]["id"],
+    foo = aiven.get_aws_vpc_peering_connection(vpc_id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         aws_account_id="XXXXX",
         aws_vpc_id="XXXXX")
     ```
 
 
     :param str aws_account_id: AWS account ID. This property cannot be changed, doing so forces recreation of the resource.
     :param str aws_vpc_id: AWS VPC ID. This property cannot be changed, doing so forces recreation of the resource.
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_azure_privatelink.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_azure_privatelink.py`

 * *Files 10% similar despite different names*

```diff
@@ -136,16 +136,16 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    foo = aiven.get_azure_privatelink(project=data["aiven_project"]["foo"]["project"],
-        service_name=aiven_kafka["bar"]["service_name"])
+    foo = aiven.get_azure_privatelink(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference))
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
     __args__ = dict()
@@ -174,16 +174,16 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    foo = aiven.get_azure_privatelink(project=data["aiven_project"]["foo"]["project"],
-        service_name=aiven_kafka["bar"]["service_name"])
+    foo = aiven.get_azure_privatelink(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference))
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
     ...
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_azure_vpc_peering_connection.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_azure_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_billing_group.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_billing_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_cassanda.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_cassanda.py`

 * *Files 1% similar despite different names*

```diff
@@ -379,15 +379,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    bar = aiven.get_cassandra(project=data["aiven_project"]["foo"]["project"],
+    bar = aiven.get_cassandra(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         service_name="<SERVICE_NAME>")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
@@ -438,15 +438,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    bar = aiven.get_cassandra(project=data["aiven_project"]["foo"]["project"],
+    bar = aiven.get_cassandra(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         service_name="<SERVICE_NAME>")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_cassandra.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_cassandra.py`

 * *Files 1% similar despite different names*

```diff
@@ -377,15 +377,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    bar = aiven.get_cassandra(project=data["aiven_project"]["foo"]["project"],
+    bar = aiven.get_cassandra(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         service_name="<SERVICE_NAME>")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
@@ -435,15 +435,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    bar = aiven.get_cassandra(project=data["aiven_project"]["foo"]["project"],
+    bar = aiven.get_cassandra(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         service_name="<SERVICE_NAME>")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_cassandra_user.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_cassandra_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_clickhouse.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_clickhouse.py`

 * *Files 1% similar despite different names*

```diff
@@ -377,15 +377,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    clickhouse = aiven.get_clickhouse(project=data["aiven_project"]["pr1"]["project"],
+    clickhouse = aiven.get_clickhouse(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         service_name="<SERVICE_NAME>")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
@@ -435,15 +435,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    clickhouse = aiven.get_clickhouse(project=data["aiven_project"]["pr1"]["project"],
+    clickhouse = aiven.get_clickhouse(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         service_name="<SERVICE_NAME>")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_clickhouse_database.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_influxdb_user.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,57 +6,82 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
-    'GetClickhouseDatabaseResult',
-    'AwaitableGetClickhouseDatabaseResult',
-    'get_clickhouse_database',
-    'get_clickhouse_database_output',
+    'GetInfluxdbUserResult',
+    'AwaitableGetInfluxdbUserResult',
+    'get_influxdb_user',
+    'get_influxdb_user_output',
 ]
 
 @pulumi.output_type
-class GetClickhouseDatabaseResult:
+class GetInfluxdbUserResult:
     """
-    A collection of values returned by getClickhouseDatabase.
+    A collection of values returned by getInfluxdbUser.
     """
-    def __init__(__self__, id=None, name=None, project=None, service_name=None, termination_protection=None):
+    def __init__(__self__, access_cert=None, access_key=None, id=None, password=None, project=None, service_name=None, type=None, username=None):
+        if access_cert and not isinstance(access_cert, str):
+            raise TypeError("Expected argument 'access_cert' to be a str")
+        pulumi.set(__self__, "access_cert", access_cert)
+        if access_key and not isinstance(access_key, str):
+            raise TypeError("Expected argument 'access_key' to be a str")
+        pulumi.set(__self__, "access_key", access_key)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
-        if name and not isinstance(name, str):
-            raise TypeError("Expected argument 'name' to be a str")
-        pulumi.set(__self__, "name", name)
+        if password and not isinstance(password, str):
+            raise TypeError("Expected argument 'password' to be a str")
+        pulumi.set(__self__, "password", password)
         if project and not isinstance(project, str):
             raise TypeError("Expected argument 'project' to be a str")
         pulumi.set(__self__, "project", project)
         if service_name and not isinstance(service_name, str):
             raise TypeError("Expected argument 'service_name' to be a str")
         pulumi.set(__self__, "service_name", service_name)
-        if termination_protection and not isinstance(termination_protection, bool):
-            raise TypeError("Expected argument 'termination_protection' to be a bool")
-        pulumi.set(__self__, "termination_protection", termination_protection)
+        if type and not isinstance(type, str):
+            raise TypeError("Expected argument 'type' to be a str")
+        pulumi.set(__self__, "type", type)
+        if username and not isinstance(username, str):
+            raise TypeError("Expected argument 'username' to be a str")
+        pulumi.set(__self__, "username", username)
+
+    @property
+    @pulumi.getter(name="accessCert")
+    def access_cert(self) -> str:
+        """
+        Access certificate for the user if applicable for the service in question
+        """
+        return pulumi.get(self, "access_cert")
+
+    @property
+    @pulumi.getter(name="accessKey")
+    def access_key(self) -> str:
+        """
+        Access certificate key for the user if applicable for the service in question
+        """
+        return pulumi.get(self, "access_key")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
-    def name(self) -> str:
+    def password(self) -> str:
         """
-        The name of the Clickhouse database. This property cannot be changed, doing so forces recreation of the resource.
+        The password of the InfluxDB User.
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def project(self) -> str:
         """
         Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
@@ -67,88 +92,105 @@
     def service_name(self) -> str:
         """
         Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
         return pulumi.get(self, "service_name")
 
     @property
-    @pulumi.getter(name="terminationProtection")
-    def termination_protection(self) -> bool:
-        return pulumi.get(self, "termination_protection")
+    @pulumi.getter
+    def type(self) -> str:
+        """
+        Type of the user account. Tells whether the user is the primary account or a regular account.
+        """
+        return pulumi.get(self, "type")
+
+    @property
+    @pulumi.getter
+    def username(self) -> str:
+        """
+        The actual name of the InfluxDB User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+        """
+        return pulumi.get(self, "username")
 
 
-class AwaitableGetClickhouseDatabaseResult(GetClickhouseDatabaseResult):
+class AwaitableGetInfluxdbUserResult(GetInfluxdbUserResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetClickhouseDatabaseResult(
+        return GetInfluxdbUserResult(
+            access_cert=self.access_cert,
+            access_key=self.access_key,
             id=self.id,
-            name=self.name,
+            password=self.password,
             project=self.project,
             service_name=self.service_name,
-            termination_protection=self.termination_protection)
+            type=self.type,
+            username=self.username)
 
 
-def get_clickhouse_database(name: Optional[str] = None,
-                            project: Optional[str] = None,
-                            service_name: Optional[str] = None,
-                            opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetClickhouseDatabaseResult:
+def get_influxdb_user(project: Optional[str] = None,
+                      service_name: Optional[str] = None,
+                      username: Optional[str] = None,
+                      opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetInfluxdbUserResult:
     """
-    The Clickhouse database data source provides information about the existing Aiven Clickhouse Database.
+    The InfluxDB User data source provides information about the existing Aiven InfluxDB User.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    clickhouse_db = aiven.get_clickhouse_database(project=aiven_clickhouse["ch"]["project"],
-        service_name=aiven_clickhouse["ch"]["service_name"],
-        name="my-ch-db")
+    user = aiven.get_influxdb_user(project="my-project",
+        service_name="my-service",
+        username="user1")
     ```
 
 
-    :param str name: The name of the Clickhouse database. This property cannot be changed, doing so forces recreation of the resource.
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+    :param str username: The actual name of the InfluxDB User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
     __args__ = dict()
-    __args__['name'] = name
     __args__['project'] = project
     __args__['serviceName'] = service_name
+    __args__['username'] = username
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('aiven:index/getClickhouseDatabase:getClickhouseDatabase', __args__, opts=opts, typ=GetClickhouseDatabaseResult).value
+    __ret__ = pulumi.runtime.invoke('aiven:index/getInfluxdbUser:getInfluxdbUser', __args__, opts=opts, typ=GetInfluxdbUserResult).value
 
-    return AwaitableGetClickhouseDatabaseResult(
+    return AwaitableGetInfluxdbUserResult(
+        access_cert=__ret__.access_cert,
+        access_key=__ret__.access_key,
         id=__ret__.id,
-        name=__ret__.name,
+        password=__ret__.password,
         project=__ret__.project,
         service_name=__ret__.service_name,
-        termination_protection=__ret__.termination_protection)
+        type=__ret__.type,
+        username=__ret__.username)
 
 
-@_utilities.lift_output_func(get_clickhouse_database)
-def get_clickhouse_database_output(name: Optional[pulumi.Input[str]] = None,
-                                   project: Optional[pulumi.Input[str]] = None,
-                                   service_name: Optional[pulumi.Input[str]] = None,
-                                   opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetClickhouseDatabaseResult]:
+@_utilities.lift_output_func(get_influxdb_user)
+def get_influxdb_user_output(project: Optional[pulumi.Input[str]] = None,
+                             service_name: Optional[pulumi.Input[str]] = None,
+                             username: Optional[pulumi.Input[str]] = None,
+                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetInfluxdbUserResult]:
     """
-    The Clickhouse database data source provides information about the existing Aiven Clickhouse Database.
+    The InfluxDB User data source provides information about the existing Aiven InfluxDB User.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    clickhouse_db = aiven.get_clickhouse_database(project=aiven_clickhouse["ch"]["project"],
-        service_name=aiven_clickhouse["ch"]["service_name"],
-        name="my-ch-db")
+    user = aiven.get_influxdb_user(project="my-project",
+        service_name="my-service",
+        username="user1")
     ```
 
 
-    :param str name: The name of the Clickhouse database. This property cannot be changed, doing so forces recreation of the resource.
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+    :param str username: The actual name of the InfluxDB User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
     ...
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_clickhouse_user.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_clickhouse_user.py`

 * *Files 16% similar despite different names*

```diff
@@ -125,16 +125,16 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    ch_user = aiven.get_clickhouse_user(project=aiven_project["myproject"]["project"],
-        service_name=aiven_clickhouse["myservice"]["service_name"],
+    ch_user = aiven.get_clickhouse_user(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         username="<USERNAME>")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str username: The actual name of the Clickhouse user. This property cannot be changed, doing so forces recreation of the resource.
@@ -166,16 +166,16 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    ch_user = aiven.get_clickhouse_user(project=aiven_project["myproject"]["project"],
-        service_name=aiven_clickhouse["myservice"]["service_name"],
+    ch_user = aiven.get_clickhouse_user(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         username="<USERNAME>")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str username: The actual name of the Clickhouse user. This property cannot be changed, doing so forces recreation of the resource.
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_connection_pool.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_connection_pool.py`

 * *Files 16% similar despite different names*

```diff
@@ -149,16 +149,16 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    mytestpool = aiven.get_connection_pool(project=aiven_project["myproject"]["project"],
-        service_name=aiven_pg["mypg"]["service_name"],
+    mytestpool = aiven.get_connection_pool(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         pool_name="mypool")
     ```
 
 
     :param str pool_name: The name of the created pool. This property cannot be changed, doing so forces recreation of the resource.
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
@@ -192,16 +192,16 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    mytestpool = aiven.get_connection_pool(project=aiven_project["myproject"]["project"],
-        service_name=aiven_pg["mypg"]["service_name"],
+    mytestpool = aiven.get_connection_pool(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         pool_name="mypool")
     ```
 
 
     :param str pool_name: The name of the created pool. This property cannot be changed, doing so forces recreation of the resource.
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_flink.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_flink.py`

 * *Files 2% similar despite different names*

```diff
@@ -377,15 +377,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    flink = aiven.get_flink(project=data["aiven_project"]["pr1"]["project"],
+    flink = aiven.get_flink(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         service_name="<SERVICE_NAME>")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
@@ -435,15 +435,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    flink = aiven.get_flink(project=data["aiven_project"]["pr1"]["project"],
+    flink = aiven.get_flink(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         service_name="<SERVICE_NAME>")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_flink_application.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_flink_application.py`

 * *Files 4% similar despite different names*

```diff
@@ -149,15 +149,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    app1 = aiven.get_flink_application(project=data["aiven_project"]["pr1"]["project"],
+    app1 = aiven.get_flink_application(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         service_name="<SERVICE_NAME>",
         name="<APPLICATION_NAME>")
     ```
 
 
     :param str name: Application name
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
@@ -192,15 +192,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    app1 = aiven.get_flink_application(project=data["aiven_project"]["pr1"]["project"],
+    app1 = aiven.get_flink_application(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         service_name="<SERVICE_NAME>",
         name="<APPLICATION_NAME>")
     ```
 
 
     :param str name: Application name
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_flink_application_version.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_flink_application_version.py`

 * *Files 4% similar despite different names*

```diff
@@ -199,15 +199,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    app1 = aiven.get_flink_application_version(project=data["aiven_project"]["pr1"]["project"],
+    app1 = aiven.get_flink_application_version(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         service_name="<SERVICE_NAME>",
         application_id="<APPLICATION_ID>",
         application_version_id="<APPLICATION_VERSION_ID>")
     ```
 
 
     :param str application_id: Application ID
@@ -250,15 +250,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    app1 = aiven.get_flink_application_version(project=data["aiven_project"]["pr1"]["project"],
+    app1 = aiven.get_flink_application_version(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         service_name="<SERVICE_NAME>",
         application_id="<APPLICATION_ID>",
         application_version_id="<APPLICATION_VERSION_ID>")
     ```
 
 
     :param str application_id: Application ID
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_gcp_vpc_peering_connection.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_gcp_vpc_peering_connection.py`

 * *Files 12% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    foo = aiven.get_gcp_vpc_peering_connection(vpc_id=data["aiven_project_vpc"]["vpc"]["id"],
+    foo = aiven.get_gcp_vpc_peering_connection(vpc_id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         gcp_project_id="xxxx",
         peer_vpc="xxxx")
     ```
 
 
     :param str gcp_project_id: GCP project ID. This property cannot be changed, doing so forces recreation of the resource.
     :param str peer_vpc: GCP VPC network name. This property cannot be changed, doing so forces recreation of the resource.
@@ -166,15 +166,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    foo = aiven.get_gcp_vpc_peering_connection(vpc_id=data["aiven_project_vpc"]["vpc"]["id"],
+    foo = aiven.get_gcp_vpc_peering_connection(vpc_id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         gcp_project_id="xxxx",
         peer_vpc="xxxx")
     ```
 
 
     :param str gcp_project_id: GCP project ID. This property cannot be changed, doing so forces recreation of the resource.
     :param str peer_vpc: GCP VPC network name. This property cannot be changed, doing so forces recreation of the resource.
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_grafana.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_grafana.py`

 * *Files 1% similar despite different names*

```diff
@@ -377,15 +377,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    gr1 = aiven.get_grafana(project=data["aiven_project"]["ps1"]["project"],
+    gr1 = aiven.get_grafana(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         service_name="my-gr1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
@@ -435,15 +435,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    gr1 = aiven.get_grafana(project=data["aiven_project"]["ps1"]["project"],
+    gr1 = aiven.get_grafana(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         service_name="my-gr1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_influx_db.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_influx_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -377,15 +377,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    inf1 = aiven.get_influx_db(project=data["aiven_project"]["pr1"]["project"],
+    inf1 = aiven.get_influx_db(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         service_name="my-inf1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
@@ -435,15 +435,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    inf1 = aiven.get_influx_db(project=data["aiven_project"]["pr1"]["project"],
+    inf1 = aiven.get_influx_db(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         service_name="my-inf1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_influxdb_database.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_influxdb_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_influxdb_user.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_pg_user.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,38 +6,41 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
-    'GetInfluxdbUserResult',
-    'AwaitableGetInfluxdbUserResult',
-    'get_influxdb_user',
-    'get_influxdb_user_output',
+    'GetPgUserResult',
+    'AwaitableGetPgUserResult',
+    'get_pg_user',
+    'get_pg_user_output',
 ]
 
 @pulumi.output_type
-class GetInfluxdbUserResult:
+class GetPgUserResult:
     """
-    A collection of values returned by getInfluxdbUser.
+    A collection of values returned by getPgUser.
     """
-    def __init__(__self__, access_cert=None, access_key=None, id=None, password=None, project=None, service_name=None, type=None, username=None):
+    def __init__(__self__, access_cert=None, access_key=None, id=None, password=None, pg_allow_replication=None, project=None, service_name=None, type=None, username=None):
         if access_cert and not isinstance(access_cert, str):
             raise TypeError("Expected argument 'access_cert' to be a str")
         pulumi.set(__self__, "access_cert", access_cert)
         if access_key and not isinstance(access_key, str):
             raise TypeError("Expected argument 'access_key' to be a str")
         pulumi.set(__self__, "access_key", access_key)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
         if password and not isinstance(password, str):
             raise TypeError("Expected argument 'password' to be a str")
         pulumi.set(__self__, "password", password)
+        if pg_allow_replication and not isinstance(pg_allow_replication, bool):
+            raise TypeError("Expected argument 'pg_allow_replication' to be a bool")
+        pulumi.set(__self__, "pg_allow_replication", pg_allow_replication)
         if project and not isinstance(project, str):
             raise TypeError("Expected argument 'project' to be a str")
         pulumi.set(__self__, "project", project)
         if service_name and not isinstance(service_name, str):
             raise TypeError("Expected argument 'service_name' to be a str")
         pulumi.set(__self__, "service_name", service_name)
         if type and not isinstance(type, str):
@@ -47,23 +50,23 @@
             raise TypeError("Expected argument 'username' to be a str")
         pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="accessCert")
     def access_cert(self) -> str:
         """
-        Access certificate for the user if applicable for the service in question
+        Access certificate for the user
         """
         return pulumi.get(self, "access_cert")
 
     @property
     @pulumi.getter(name="accessKey")
     def access_key(self) -> str:
         """
-        Access certificate key for the user if applicable for the service in question
+        Access certificate key for the user
         """
         return pulumi.get(self, "access_key")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
@@ -71,19 +74,27 @@
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def password(self) -> str:
         """
-        The password of the InfluxDB User.
+        The password of the PG User ( not applicable for all services ).
         """
         return pulumi.get(self, "password")
 
     @property
+    @pulumi.getter(name="pgAllowReplication")
+    def pg_allow_replication(self) -> bool:
+        """
+        Defines whether replication is allowed. This property cannot be changed, doing so forces recreation of the resource.
+        """
+        return pulumi.get(self, "pg_allow_replication")
+
+    @property
     @pulumi.getter
     def project(self) -> str:
         """
         Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
         return pulumi.get(self, "project")
 
@@ -103,94 +114,96 @@
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def username(self) -> str:
         """
-        The actual name of the InfluxDB User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+        The actual name of the PG User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
         return pulumi.get(self, "username")
 
 
-class AwaitableGetInfluxdbUserResult(GetInfluxdbUserResult):
+class AwaitableGetPgUserResult(GetPgUserResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetInfluxdbUserResult(
+        return GetPgUserResult(
             access_cert=self.access_cert,
             access_key=self.access_key,
             id=self.id,
             password=self.password,
+            pg_allow_replication=self.pg_allow_replication,
             project=self.project,
             service_name=self.service_name,
             type=self.type,
             username=self.username)
 
 
-def get_influxdb_user(project: Optional[str] = None,
-                      service_name: Optional[str] = None,
-                      username: Optional[str] = None,
-                      opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetInfluxdbUserResult:
+def get_pg_user(project: Optional[str] = None,
+                service_name: Optional[str] = None,
+                username: Optional[str] = None,
+                opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPgUserResult:
     """
-    The InfluxDB User data source provides information about the existing Aiven InfluxDB User.
+    The PG User data source provides information about the existing Aiven PG User.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    user = aiven.get_influxdb_user(project="my-project",
+    user = aiven.get_pg_user(project="my-project",
         service_name="my-service",
         username="user1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
-    :param str username: The actual name of the InfluxDB User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+    :param str username: The actual name of the PG User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
     __args__ = dict()
     __args__['project'] = project
     __args__['serviceName'] = service_name
     __args__['username'] = username
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('aiven:index/getInfluxdbUser:getInfluxdbUser', __args__, opts=opts, typ=GetInfluxdbUserResult).value
+    __ret__ = pulumi.runtime.invoke('aiven:index/getPgUser:getPgUser', __args__, opts=opts, typ=GetPgUserResult).value
 
-    return AwaitableGetInfluxdbUserResult(
+    return AwaitableGetPgUserResult(
         access_cert=__ret__.access_cert,
         access_key=__ret__.access_key,
         id=__ret__.id,
         password=__ret__.password,
+        pg_allow_replication=__ret__.pg_allow_replication,
         project=__ret__.project,
         service_name=__ret__.service_name,
         type=__ret__.type,
         username=__ret__.username)
 
 
-@_utilities.lift_output_func(get_influxdb_user)
-def get_influxdb_user_output(project: Optional[pulumi.Input[str]] = None,
-                             service_name: Optional[pulumi.Input[str]] = None,
-                             username: Optional[pulumi.Input[str]] = None,
-                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetInfluxdbUserResult]:
+@_utilities.lift_output_func(get_pg_user)
+def get_pg_user_output(project: Optional[pulumi.Input[str]] = None,
+                       service_name: Optional[pulumi.Input[str]] = None,
+                       username: Optional[pulumi.Input[str]] = None,
+                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPgUserResult]:
     """
-    The InfluxDB User data source provides information about the existing Aiven InfluxDB User.
+    The PG User data source provides information about the existing Aiven PG User.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    user = aiven.get_influxdb_user(project="my-project",
+    user = aiven.get_pg_user(project="my-project",
         service_name="my-service",
         username="user1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
-    :param str username: The actual name of the InfluxDB User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+    :param str username: The actual name of the PG User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
     ...
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_kafka.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_kafka.py`

 * *Files 2% similar despite different names*

```diff
@@ -401,15 +401,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    kafka1 = aiven.get_kafka(project=data["aiven_project"]["pr1"]["project"],
+    kafka1 = aiven.get_kafka(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         service_name="my-kafka1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
@@ -461,15 +461,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    kafka1 = aiven.get_kafka(project=data["aiven_project"]["pr1"]["project"],
+    kafka1 = aiven.get_kafka(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         service_name="my-kafka1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_kafka_acl.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_kafka_acl.py`

 * *Files 4% similar despite different names*

```diff
@@ -127,16 +127,16 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    mytestacl = aiven.get_kafka_acl(project=aiven_project["myproject"]["project"],
-        service_name=aiven_kafka["mykafka"]["service_name"],
+    mytestacl = aiven.get_kafka_acl(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         topic="<TOPIC_NAME_PATTERN>",
         permission="<PERMISSON>",
         username="<USERNAME_PATTERN>")
     ```
 
 
     :param str permission: Kafka permission to grant. The possible values are `admin`, `read`, `readwrite` and `write`. This property cannot be changed, doing so forces recreation of the resource.
@@ -176,16 +176,16 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    mytestacl = aiven.get_kafka_acl(project=aiven_project["myproject"]["project"],
-        service_name=aiven_kafka["mykafka"]["service_name"],
+    mytestacl = aiven.get_kafka_acl(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         topic="<TOPIC_NAME_PATTERN>",
         permission="<PERMISSON>",
         username="<USERNAME_PATTERN>")
     ```
 
 
     :param str permission: Kafka permission to grant. The possible values are `admin`, `read`, `readwrite` and `write`. This property cannot be changed, doing so forces recreation of the resource.
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_kafka_connect.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_kafka_connect.py`

 * *Files 1% similar despite different names*

```diff
@@ -377,15 +377,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    kc1 = aiven.get_kafka_connect(project=data["aiven_project"]["pr1"]["project"],
+    kc1 = aiven.get_kafka_connect(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         service_name="my-kc1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
@@ -435,15 +435,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    kc1 = aiven.get_kafka_connect(project=data["aiven_project"]["pr1"]["project"],
+    kc1 = aiven.get_kafka_connect(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         service_name="my-kc1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_kafka_connector.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_kafka_connector.py`

 * *Files 5% similar despite different names*

```diff
@@ -186,16 +186,16 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    kafka_es_con1 = aiven.get_kafka_connector(project=aiven_project["kafka-con-project1"]["project"],
-        service_name=aiven_kafka["kafka-service1"]["service_name"],
+    kafka_es_con1 = aiven.get_kafka_connector(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         connector_name="kafka-es-con1")
     ```
 
 
     :param str connector_name: The kafka connector name. This property cannot be changed, doing so forces recreation of the resource.
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
@@ -232,16 +232,16 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    kafka_es_con1 = aiven.get_kafka_connector(project=aiven_project["kafka-con-project1"]["project"],
-        service_name=aiven_kafka["kafka-service1"]["service_name"],
+    kafka_es_con1 = aiven.get_kafka_connector(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         connector_name="kafka-es-con1")
     ```
 
 
     :param str connector_name: The kafka connector name. This property cannot be changed, doing so forces recreation of the resource.
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_kafka_mirror_maker.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_kafka_mirror_maker.py`

 * *Files 2% similar despite different names*

```diff
@@ -377,15 +377,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    mm1 = aiven.get_kafka_mirror_maker(project=data["aiven_project"]["pr1"]["project"],
+    mm1 = aiven.get_kafka_mirror_maker(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         service_name="my-mm1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
@@ -435,15 +435,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    mm1 = aiven.get_kafka_mirror_maker(project=data["aiven_project"]["pr1"]["project"],
+    mm1 = aiven.get_kafka_mirror_maker(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         service_name="my-mm1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_kafka_schema.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_kafka_schema_configuration.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
-    'GetKafkaSchemaResult',
-    'AwaitableGetKafkaSchemaResult',
-    'get_kafka_schema',
-    'get_kafka_schema_output',
+    'GetKafkaSchemaConfigurationResult',
+    'AwaitableGetKafkaSchemaConfigurationResult',
+    'get_kafka_schema_configuration',
+    'get_kafka_schema_configuration_output',
 ]
 
 @pulumi.output_type
-class GetKafkaSchemaResult:
+class GetKafkaSchemaConfigurationResult:
     """
-    A collection of values returned by getKafkaSchema.
+    A collection of values returned by getKafkaSchemaConfiguration.
     """
     def __init__(__self__, compatibility_level=None, id=None, project=None, schema=None, schema_type=None, service_name=None, subject_name=None, version=None):
         if compatibility_level and not isinstance(compatibility_level, str):
             raise TypeError("Expected argument 'compatibility_level' to be a str")
         pulumi.set(__self__, "compatibility_level", compatibility_level)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
@@ -108,87 +108,86 @@
     def version(self) -> int:
         """
         Kafka Schema configuration version.
         """
         return pulumi.get(self, "version")
 
 
-class AwaitableGetKafkaSchemaResult(GetKafkaSchemaResult):
+class AwaitableGetKafkaSchemaConfigurationResult(GetKafkaSchemaConfigurationResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetKafkaSchemaResult(
+        return GetKafkaSchemaConfigurationResult(
             compatibility_level=self.compatibility_level,
             id=self.id,
             project=self.project,
             schema=self.schema,
             schema_type=self.schema_type,
             service_name=self.service_name,
             subject_name=self.subject_name,
             version=self.version)
 
 
-def get_kafka_schema(project: Optional[str] = None,
-                     service_name: Optional[str] = None,
-                     subject_name: Optional[str] = None,
-                     opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetKafkaSchemaResult:
+def get_kafka_schema_configuration(project: Optional[str] = None,
+                                   service_name: Optional[str] = None,
+                                   opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetKafkaSchemaConfigurationResult:
     """
-    The Kafka Schema data source provides information about the existing Aiven Kafka Schema.
+    The Kafka Schema Configuration data source provides information about the existing Aiven Kafka Schema Configuration.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    config = aiven.get_kafka_schema_configuration(project=aiven_project["kafka-schemas-project1"]["project"],
-        service_name=aiven_kafka["kafka-service1"]["service_name"])
+    config = aiven.KafkaSchemaConfiguration("config",
+        project=aiven_project["kafka-schemas-project1"]["project"],
+        service_name=aiven_kafka["kafka-service1"]["service_name"],
+        compatibility_level="BACKWARD")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
-    :param str subject_name: The Kafka Schema Subject name. This property cannot be changed, doing so forces recreation of the resource.
     """
     __args__ = dict()
     __args__['project'] = project
     __args__['serviceName'] = service_name
-    __args__['subjectName'] = subject_name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('aiven:index/getKafkaSchema:getKafkaSchema', __args__, opts=opts, typ=GetKafkaSchemaResult).value
+    __ret__ = pulumi.runtime.invoke('aiven:index/getKafkaSchemaConfiguration:getKafkaSchemaConfiguration', __args__, opts=opts, typ=GetKafkaSchemaConfigurationResult).value
 
-    return AwaitableGetKafkaSchemaResult(
+    return AwaitableGetKafkaSchemaConfigurationResult(
         compatibility_level=__ret__.compatibility_level,
         id=__ret__.id,
         project=__ret__.project,
         schema=__ret__.schema,
         schema_type=__ret__.schema_type,
         service_name=__ret__.service_name,
         subject_name=__ret__.subject_name,
         version=__ret__.version)
 
 
-@_utilities.lift_output_func(get_kafka_schema)
-def get_kafka_schema_output(project: Optional[pulumi.Input[str]] = None,
-                            service_name: Optional[pulumi.Input[str]] = None,
-                            subject_name: Optional[pulumi.Input[str]] = None,
-                            opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetKafkaSchemaResult]:
+@_utilities.lift_output_func(get_kafka_schema_configuration)
+def get_kafka_schema_configuration_output(project: Optional[pulumi.Input[str]] = None,
+                                          service_name: Optional[pulumi.Input[str]] = None,
+                                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetKafkaSchemaConfigurationResult]:
     """
-    The Kafka Schema data source provides information about the existing Aiven Kafka Schema.
+    The Kafka Schema Configuration data source provides information about the existing Aiven Kafka Schema Configuration.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    config = aiven.get_kafka_schema_configuration(project=aiven_project["kafka-schemas-project1"]["project"],
-        service_name=aiven_kafka["kafka-service1"]["service_name"])
+    config = aiven.KafkaSchemaConfiguration("config",
+        project=aiven_project["kafka-schemas-project1"]["project"],
+        service_name=aiven_kafka["kafka-service1"]["service_name"],
+        compatibility_level="BACKWARD")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
-    :param str subject_name: The Kafka Schema Subject name. This property cannot be changed, doing so forces recreation of the resource.
     """
     ...
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_kafka_schema_configuration.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_kafka_topic.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,190 +4,204 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
+from . import outputs
 
 __all__ = [
-    'GetKafkaSchemaConfigurationResult',
-    'AwaitableGetKafkaSchemaConfigurationResult',
-    'get_kafka_schema_configuration',
-    'get_kafka_schema_configuration_output',
+    'GetKafkaTopicResult',
+    'AwaitableGetKafkaTopicResult',
+    'get_kafka_topic',
+    'get_kafka_topic_output',
 ]
 
 @pulumi.output_type
-class GetKafkaSchemaConfigurationResult:
+class GetKafkaTopicResult:
     """
-    A collection of values returned by getKafkaSchemaConfiguration.
+    A collection of values returned by getKafkaTopic.
     """
-    def __init__(__self__, compatibility_level=None, id=None, project=None, schema=None, schema_type=None, service_name=None, subject_name=None, version=None):
-        if compatibility_level and not isinstance(compatibility_level, str):
-            raise TypeError("Expected argument 'compatibility_level' to be a str")
-        pulumi.set(__self__, "compatibility_level", compatibility_level)
+    def __init__(__self__, configs=None, id=None, partitions=None, project=None, replication=None, service_name=None, tags=None, termination_protection=None, topic_name=None):
+        if configs and not isinstance(configs, list):
+            raise TypeError("Expected argument 'configs' to be a list")
+        pulumi.set(__self__, "configs", configs)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
+        if partitions and not isinstance(partitions, int):
+            raise TypeError("Expected argument 'partitions' to be a int")
+        pulumi.set(__self__, "partitions", partitions)
         if project and not isinstance(project, str):
             raise TypeError("Expected argument 'project' to be a str")
         pulumi.set(__self__, "project", project)
-        if schema and not isinstance(schema, str):
-            raise TypeError("Expected argument 'schema' to be a str")
-        pulumi.set(__self__, "schema", schema)
-        if schema_type and not isinstance(schema_type, str):
-            raise TypeError("Expected argument 'schema_type' to be a str")
-        pulumi.set(__self__, "schema_type", schema_type)
+        if replication and not isinstance(replication, int):
+            raise TypeError("Expected argument 'replication' to be a int")
+        pulumi.set(__self__, "replication", replication)
         if service_name and not isinstance(service_name, str):
             raise TypeError("Expected argument 'service_name' to be a str")
         pulumi.set(__self__, "service_name", service_name)
-        if subject_name and not isinstance(subject_name, str):
-            raise TypeError("Expected argument 'subject_name' to be a str")
-        pulumi.set(__self__, "subject_name", subject_name)
-        if version and not isinstance(version, int):
-            raise TypeError("Expected argument 'version' to be a int")
-        pulumi.set(__self__, "version", version)
+        if tags and not isinstance(tags, list):
+            raise TypeError("Expected argument 'tags' to be a list")
+        pulumi.set(__self__, "tags", tags)
+        if termination_protection and not isinstance(termination_protection, bool):
+            raise TypeError("Expected argument 'termination_protection' to be a bool")
+        pulumi.set(__self__, "termination_protection", termination_protection)
+        if topic_name and not isinstance(topic_name, str):
+            raise TypeError("Expected argument 'topic_name' to be a str")
+        pulumi.set(__self__, "topic_name", topic_name)
 
     @property
-    @pulumi.getter(name="compatibilityLevel")
-    def compatibility_level(self) -> str:
+    @pulumi.getter
+    def configs(self) -> Sequence['outputs.GetKafkaTopicConfigResult']:
         """
-        Kafka Schemas compatibility level. The possible values are `BACKWARD`, `BACKWARD_TRANSITIVE`, `FORWARD`, `FORWARD_TRANSITIVE`, `FULL`, `FULL_TRANSITIVE` and `NONE`.
+        Kafka topic configuration
         """
-        return pulumi.get(self, "compatibility_level")
+        return pulumi.get(self, "configs")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
-    def project(self) -> str:
+    def partitions(self) -> int:
         """
-        Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+        The number of partitions to create in the topic.
         """
-        return pulumi.get(self, "project")
+        return pulumi.get(self, "partitions")
 
     @property
     @pulumi.getter
-    def schema(self) -> str:
+    def project(self) -> str:
         """
-        Kafka Schema configuration should be a valid Avro Schema JSON format.
+        Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
-        return pulumi.get(self, "schema")
+        return pulumi.get(self, "project")
 
     @property
-    @pulumi.getter(name="schemaType")
-    def schema_type(self) -> str:
+    @pulumi.getter
+    def replication(self) -> int:
         """
-        Kafka Schema type JSON or AVRO
+        The replication factor for the topic.
         """
-        return pulumi.get(self, "schema_type")
+        return pulumi.get(self, "replication")
 
     @property
     @pulumi.getter(name="serviceName")
     def service_name(self) -> str:
         """
         Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
         return pulumi.get(self, "service_name")
 
     @property
-    @pulumi.getter(name="subjectName")
-    def subject_name(self) -> str:
+    @pulumi.getter
+    def tags(self) -> Sequence['outputs.GetKafkaTopicTagResult']:
         """
-        The Kafka Schema Subject name. This property cannot be changed, doing so forces recreation of the resource.
+        Kafka Topic tag.
         """
-        return pulumi.get(self, "subject_name")
+        return pulumi.get(self, "tags")
 
     @property
-    @pulumi.getter
-    def version(self) -> int:
+    @pulumi.getter(name="terminationProtection")
+    def termination_protection(self) -> bool:
+        return pulumi.get(self, "termination_protection")
+
+    @property
+    @pulumi.getter(name="topicName")
+    def topic_name(self) -> str:
         """
-        Kafka Schema configuration version.
+        The name of the topic. This property cannot be changed, doing so forces recreation of the resource.
         """
-        return pulumi.get(self, "version")
+        return pulumi.get(self, "topic_name")
 
 
-class AwaitableGetKafkaSchemaConfigurationResult(GetKafkaSchemaConfigurationResult):
+class AwaitableGetKafkaTopicResult(GetKafkaTopicResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetKafkaSchemaConfigurationResult(
-            compatibility_level=self.compatibility_level,
+        return GetKafkaTopicResult(
+            configs=self.configs,
             id=self.id,
+            partitions=self.partitions,
             project=self.project,
-            schema=self.schema,
-            schema_type=self.schema_type,
+            replication=self.replication,
             service_name=self.service_name,
-            subject_name=self.subject_name,
-            version=self.version)
+            tags=self.tags,
+            termination_protection=self.termination_protection,
+            topic_name=self.topic_name)
 
 
-def get_kafka_schema_configuration(project: Optional[str] = None,
-                                   service_name: Optional[str] = None,
-                                   opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetKafkaSchemaConfigurationResult:
+def get_kafka_topic(project: Optional[str] = None,
+                    service_name: Optional[str] = None,
+                    topic_name: Optional[str] = None,
+                    opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetKafkaTopicResult:
     """
-    The Kafka Schema Configuration data source provides information about the existing Aiven Kafka Schema Configuration.
+    The Kafka Topic data source provides information about the existing Aiven Kafka Topic.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    config = aiven.KafkaSchemaConfiguration("config",
-        project=aiven_project["kafka-schemas-project1"]["project"],
-        service_name=aiven_kafka["kafka-service1"]["service_name"],
-        compatibility_level="BACKWARD")
+    mytesttopic = aiven.get_kafka_topic(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+        topic_name="<TOPIC_NAME>")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+    :param str topic_name: The name of the topic. This property cannot be changed, doing so forces recreation of the resource.
     """
     __args__ = dict()
     __args__['project'] = project
     __args__['serviceName'] = service_name
+    __args__['topicName'] = topic_name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('aiven:index/getKafkaSchemaConfiguration:getKafkaSchemaConfiguration', __args__, opts=opts, typ=GetKafkaSchemaConfigurationResult).value
+    __ret__ = pulumi.runtime.invoke('aiven:index/getKafkaTopic:getKafkaTopic', __args__, opts=opts, typ=GetKafkaTopicResult).value
 
-    return AwaitableGetKafkaSchemaConfigurationResult(
-        compatibility_level=__ret__.compatibility_level,
+    return AwaitableGetKafkaTopicResult(
+        configs=__ret__.configs,
         id=__ret__.id,
+        partitions=__ret__.partitions,
         project=__ret__.project,
-        schema=__ret__.schema,
-        schema_type=__ret__.schema_type,
+        replication=__ret__.replication,
         service_name=__ret__.service_name,
-        subject_name=__ret__.subject_name,
-        version=__ret__.version)
+        tags=__ret__.tags,
+        termination_protection=__ret__.termination_protection,
+        topic_name=__ret__.topic_name)
 
 
-@_utilities.lift_output_func(get_kafka_schema_configuration)
-def get_kafka_schema_configuration_output(project: Optional[pulumi.Input[str]] = None,
-                                          service_name: Optional[pulumi.Input[str]] = None,
-                                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetKafkaSchemaConfigurationResult]:
+@_utilities.lift_output_func(get_kafka_topic)
+def get_kafka_topic_output(project: Optional[pulumi.Input[str]] = None,
+                           service_name: Optional[pulumi.Input[str]] = None,
+                           topic_name: Optional[pulumi.Input[str]] = None,
+                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetKafkaTopicResult]:
     """
-    The Kafka Schema Configuration data source provides information about the existing Aiven Kafka Schema Configuration.
+    The Kafka Topic data source provides information about the existing Aiven Kafka Topic.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    config = aiven.KafkaSchemaConfiguration("config",
-        project=aiven_project["kafka-schemas-project1"]["project"],
-        service_name=aiven_kafka["kafka-service1"]["service_name"],
-        compatibility_level="BACKWARD")
+    mytesttopic = aiven.get_kafka_topic(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+        topic_name="<TOPIC_NAME>")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+    :param str topic_name: The name of the topic. This property cannot be changed, doing so forces recreation of the resource.
     """
     ...
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_kafka_schema_registry_acl.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_kafka_schema_registry_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_kafka_topic.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_kafka_user.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,204 +4,193 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
-from . import outputs
 
 __all__ = [
-    'GetKafkaTopicResult',
-    'AwaitableGetKafkaTopicResult',
-    'get_kafka_topic',
-    'get_kafka_topic_output',
+    'GetKafkaUserResult',
+    'AwaitableGetKafkaUserResult',
+    'get_kafka_user',
+    'get_kafka_user_output',
 ]
 
 @pulumi.output_type
-class GetKafkaTopicResult:
+class GetKafkaUserResult:
     """
-    A collection of values returned by getKafkaTopic.
+    A collection of values returned by getKafkaUser.
     """
-    def __init__(__self__, configs=None, id=None, partitions=None, project=None, replication=None, service_name=None, tags=None, termination_protection=None, topic_name=None):
-        if configs and not isinstance(configs, list):
-            raise TypeError("Expected argument 'configs' to be a list")
-        pulumi.set(__self__, "configs", configs)
+    def __init__(__self__, access_cert=None, access_key=None, id=None, password=None, project=None, service_name=None, type=None, username=None):
+        if access_cert and not isinstance(access_cert, str):
+            raise TypeError("Expected argument 'access_cert' to be a str")
+        pulumi.set(__self__, "access_cert", access_cert)
+        if access_key and not isinstance(access_key, str):
+            raise TypeError("Expected argument 'access_key' to be a str")
+        pulumi.set(__self__, "access_key", access_key)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
-        if partitions and not isinstance(partitions, int):
-            raise TypeError("Expected argument 'partitions' to be a int")
-        pulumi.set(__self__, "partitions", partitions)
+        if password and not isinstance(password, str):
+            raise TypeError("Expected argument 'password' to be a str")
+        pulumi.set(__self__, "password", password)
         if project and not isinstance(project, str):
             raise TypeError("Expected argument 'project' to be a str")
         pulumi.set(__self__, "project", project)
-        if replication and not isinstance(replication, int):
-            raise TypeError("Expected argument 'replication' to be a int")
-        pulumi.set(__self__, "replication", replication)
         if service_name and not isinstance(service_name, str):
             raise TypeError("Expected argument 'service_name' to be a str")
         pulumi.set(__self__, "service_name", service_name)
-        if tags and not isinstance(tags, list):
-            raise TypeError("Expected argument 'tags' to be a list")
-        pulumi.set(__self__, "tags", tags)
-        if termination_protection and not isinstance(termination_protection, bool):
-            raise TypeError("Expected argument 'termination_protection' to be a bool")
-        pulumi.set(__self__, "termination_protection", termination_protection)
-        if topic_name and not isinstance(topic_name, str):
-            raise TypeError("Expected argument 'topic_name' to be a str")
-        pulumi.set(__self__, "topic_name", topic_name)
+        if type and not isinstance(type, str):
+            raise TypeError("Expected argument 'type' to be a str")
+        pulumi.set(__self__, "type", type)
+        if username and not isinstance(username, str):
+            raise TypeError("Expected argument 'username' to be a str")
+        pulumi.set(__self__, "username", username)
 
     @property
-    @pulumi.getter
-    def configs(self) -> Sequence['outputs.GetKafkaTopicConfigResult']:
+    @pulumi.getter(name="accessCert")
+    def access_cert(self) -> str:
         """
-        Kafka topic configuration
+        Access certificate for the user
         """
-        return pulumi.get(self, "configs")
+        return pulumi.get(self, "access_cert")
+
+    @property
+    @pulumi.getter(name="accessKey")
+    def access_key(self) -> str:
+        """
+        Access certificate key for the user
+        """
+        return pulumi.get(self, "access_key")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
-    def partitions(self) -> int:
+    def password(self) -> str:
         """
-        The number of partitions to create in the topic.
+        The password of the Kafka User.
         """
-        return pulumi.get(self, "partitions")
+        return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def project(self) -> str:
         """
         Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
         return pulumi.get(self, "project")
 
     @property
-    @pulumi.getter
-    def replication(self) -> int:
-        """
-        The replication factor for the topic.
-        """
-        return pulumi.get(self, "replication")
-
-    @property
     @pulumi.getter(name="serviceName")
     def service_name(self) -> str:
         """
         Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
         return pulumi.get(self, "service_name")
 
     @property
     @pulumi.getter
-    def tags(self) -> Sequence['outputs.GetKafkaTopicTagResult']:
+    def type(self) -> str:
         """
-        Kafka Topic tag.
+        Type of the user account. Tells whether the user is the primary account or a regular account.
         """
-        return pulumi.get(self, "tags")
+        return pulumi.get(self, "type")
 
     @property
-    @pulumi.getter(name="terminationProtection")
-    def termination_protection(self) -> bool:
-        return pulumi.get(self, "termination_protection")
-
-    @property
-    @pulumi.getter(name="topicName")
-    def topic_name(self) -> str:
+    @pulumi.getter
+    def username(self) -> str:
         """
-        The name of the topic. This property cannot be changed, doing so forces recreation of the resource.
+        The actual name of the Kafka User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
-        return pulumi.get(self, "topic_name")
+        return pulumi.get(self, "username")
 
 
-class AwaitableGetKafkaTopicResult(GetKafkaTopicResult):
+class AwaitableGetKafkaUserResult(GetKafkaUserResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetKafkaTopicResult(
-            configs=self.configs,
+        return GetKafkaUserResult(
+            access_cert=self.access_cert,
+            access_key=self.access_key,
             id=self.id,
-            partitions=self.partitions,
+            password=self.password,
             project=self.project,
-            replication=self.replication,
             service_name=self.service_name,
-            tags=self.tags,
-            termination_protection=self.termination_protection,
-            topic_name=self.topic_name)
+            type=self.type,
+            username=self.username)
 
 
-def get_kafka_topic(project: Optional[str] = None,
-                    service_name: Optional[str] = None,
-                    topic_name: Optional[str] = None,
-                    opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetKafkaTopicResult:
+def get_kafka_user(project: Optional[str] = None,
+                   service_name: Optional[str] = None,
+                   username: Optional[str] = None,
+                   opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetKafkaUserResult:
     """
-    The Kafka Topic data source provides information about the existing Aiven Kafka Topic.
+    The Kafka User data source provides information about the existing Aiven Kafka User.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    mytesttopic = aiven.get_kafka_topic(project=aiven_project["myproject"]["project"],
-        service_name=aiven_kafka["myservice"]["service_name"],
-        topic_name="<TOPIC_NAME>")
+    user = aiven.get_kafka_user(project="my-project",
+        service_name="my-service",
+        username="user1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
-    :param str topic_name: The name of the topic. This property cannot be changed, doing so forces recreation of the resource.
+    :param str username: The actual name of the Kafka User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
     __args__ = dict()
     __args__['project'] = project
     __args__['serviceName'] = service_name
-    __args__['topicName'] = topic_name
+    __args__['username'] = username
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('aiven:index/getKafkaTopic:getKafkaTopic', __args__, opts=opts, typ=GetKafkaTopicResult).value
+    __ret__ = pulumi.runtime.invoke('aiven:index/getKafkaUser:getKafkaUser', __args__, opts=opts, typ=GetKafkaUserResult).value
 
-    return AwaitableGetKafkaTopicResult(
-        configs=__ret__.configs,
+    return AwaitableGetKafkaUserResult(
+        access_cert=__ret__.access_cert,
+        access_key=__ret__.access_key,
         id=__ret__.id,
-        partitions=__ret__.partitions,
+        password=__ret__.password,
         project=__ret__.project,
-        replication=__ret__.replication,
         service_name=__ret__.service_name,
-        tags=__ret__.tags,
-        termination_protection=__ret__.termination_protection,
-        topic_name=__ret__.topic_name)
+        type=__ret__.type,
+        username=__ret__.username)
 
 
-@_utilities.lift_output_func(get_kafka_topic)
-def get_kafka_topic_output(project: Optional[pulumi.Input[str]] = None,
-                           service_name: Optional[pulumi.Input[str]] = None,
-                           topic_name: Optional[pulumi.Input[str]] = None,
-                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetKafkaTopicResult]:
+@_utilities.lift_output_func(get_kafka_user)
+def get_kafka_user_output(project: Optional[pulumi.Input[str]] = None,
+                          service_name: Optional[pulumi.Input[str]] = None,
+                          username: Optional[pulumi.Input[str]] = None,
+                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetKafkaUserResult]:
     """
-    The Kafka Topic data source provides information about the existing Aiven Kafka Topic.
+    The Kafka User data source provides information about the existing Aiven Kafka User.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    mytesttopic = aiven.get_kafka_topic(project=aiven_project["myproject"]["project"],
-        service_name=aiven_kafka["myservice"]["service_name"],
-        topic_name="<TOPIC_NAME>")
+    user = aiven.get_kafka_user(project="my-project",
+        service_name="my-service",
+        username="user1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
-    :param str topic_name: The name of the topic. This property cannot be changed, doing so forces recreation of the resource.
+    :param str username: The actual name of the Kafka User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
     ...
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_kafka_user.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_m3db_user.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,32 +6,26 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
-    'GetKafkaUserResult',
-    'AwaitableGetKafkaUserResult',
-    'get_kafka_user',
-    'get_kafka_user_output',
+    'GetM3dbUserResult',
+    'AwaitableGetM3dbUserResult',
+    'get_m3db_user',
+    'get_m3db_user_output',
 ]
 
 @pulumi.output_type
-class GetKafkaUserResult:
+class GetM3dbUserResult:
     """
-    A collection of values returned by getKafkaUser.
+    A collection of values returned by getM3dbUser.
     """
-    def __init__(__self__, access_cert=None, access_key=None, id=None, password=None, project=None, service_name=None, type=None, username=None):
-        if access_cert and not isinstance(access_cert, str):
-            raise TypeError("Expected argument 'access_cert' to be a str")
-        pulumi.set(__self__, "access_cert", access_cert)
-        if access_key and not isinstance(access_key, str):
-            raise TypeError("Expected argument 'access_key' to be a str")
-        pulumi.set(__self__, "access_key", access_key)
+    def __init__(__self__, id=None, password=None, project=None, service_name=None, type=None, username=None):
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
         if password and not isinstance(password, str):
             raise TypeError("Expected argument 'password' to be a str")
         pulumi.set(__self__, "password", password)
         if project and not isinstance(project, str):
@@ -44,42 +38,26 @@
             raise TypeError("Expected argument 'type' to be a str")
         pulumi.set(__self__, "type", type)
         if username and not isinstance(username, str):
             raise TypeError("Expected argument 'username' to be a str")
         pulumi.set(__self__, "username", username)
 
     @property
-    @pulumi.getter(name="accessCert")
-    def access_cert(self) -> str:
-        """
-        Access certificate for the user
-        """
-        return pulumi.get(self, "access_cert")
-
-    @property
-    @pulumi.getter(name="accessKey")
-    def access_key(self) -> str:
-        """
-        Access certificate key for the user
-        """
-        return pulumi.get(self, "access_key")
-
-    @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def password(self) -> str:
         """
-        The password of the Kafka User.
+        The password of the M3DB User.
         """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def project(self) -> str:
         """
@@ -103,94 +81,90 @@
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def username(self) -> str:
         """
-        The actual name of the Kafka User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+        The actual name of the M3DB User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
         return pulumi.get(self, "username")
 
 
-class AwaitableGetKafkaUserResult(GetKafkaUserResult):
+class AwaitableGetM3dbUserResult(GetM3dbUserResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetKafkaUserResult(
-            access_cert=self.access_cert,
-            access_key=self.access_key,
+        return GetM3dbUserResult(
             id=self.id,
             password=self.password,
             project=self.project,
             service_name=self.service_name,
             type=self.type,
             username=self.username)
 
 
-def get_kafka_user(project: Optional[str] = None,
-                   service_name: Optional[str] = None,
-                   username: Optional[str] = None,
-                   opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetKafkaUserResult:
+def get_m3db_user(project: Optional[str] = None,
+                  service_name: Optional[str] = None,
+                  username: Optional[str] = None,
+                  opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetM3dbUserResult:
     """
-    The Kafka User data source provides information about the existing Aiven Kafka User.
+    The M3DB User data source provides information about the existing Aiven M3DB User.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    user = aiven.get_kafka_user(project="my-project",
+    user = aiven.get_m3db_user(project="my-project",
         service_name="my-service",
         username="user1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
-    :param str username: The actual name of the Kafka User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+    :param str username: The actual name of the M3DB User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
     __args__ = dict()
     __args__['project'] = project
     __args__['serviceName'] = service_name
     __args__['username'] = username
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('aiven:index/getKafkaUser:getKafkaUser', __args__, opts=opts, typ=GetKafkaUserResult).value
+    __ret__ = pulumi.runtime.invoke('aiven:index/getM3dbUser:getM3dbUser', __args__, opts=opts, typ=GetM3dbUserResult).value
 
-    return AwaitableGetKafkaUserResult(
-        access_cert=__ret__.access_cert,
-        access_key=__ret__.access_key,
+    return AwaitableGetM3dbUserResult(
         id=__ret__.id,
         password=__ret__.password,
         project=__ret__.project,
         service_name=__ret__.service_name,
         type=__ret__.type,
         username=__ret__.username)
 
 
-@_utilities.lift_output_func(get_kafka_user)
-def get_kafka_user_output(project: Optional[pulumi.Input[str]] = None,
-                          service_name: Optional[pulumi.Input[str]] = None,
-                          username: Optional[pulumi.Input[str]] = None,
-                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetKafkaUserResult]:
+@_utilities.lift_output_func(get_m3db_user)
+def get_m3db_user_output(project: Optional[pulumi.Input[str]] = None,
+                         service_name: Optional[pulumi.Input[str]] = None,
+                         username: Optional[pulumi.Input[str]] = None,
+                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetM3dbUserResult]:
     """
-    The Kafka User data source provides information about the existing Aiven Kafka User.
+    The M3DB User data source provides information about the existing Aiven M3DB User.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    user = aiven.get_kafka_user(project="my-project",
+    user = aiven.get_m3db_user(project="my-project",
         service_name="my-service",
         username="user1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
-    :param str username: The actual name of the Kafka User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+    :param str username: The actual name of the M3DB User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
     ...
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_m3_aggregator.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_m3_aggregator.py`

 * *Files 1% similar despite different names*

```diff
@@ -377,15 +377,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    m3a = aiven.get_m3_aggregator(project=data["aiven_project"]["foo"]["project"],
+    m3a = aiven.get_m3_aggregator(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         service_name="my-m3a")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
@@ -435,15 +435,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    m3a = aiven.get_m3_aggregator(project=data["aiven_project"]["foo"]["project"],
+    m3a = aiven.get_m3_aggregator(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         service_name="my-m3a")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_m3_db.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_m3_db.py`

 * *Files 1% similar despite different names*

```diff
@@ -377,15 +377,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    m3 = aiven.get_m3_db(project=data["aiven_project"]["foo"]["project"],
+    m3 = aiven.get_m3_db(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         service_name="my-m3db")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
@@ -435,15 +435,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    m3 = aiven.get_m3_db(project=data["aiven_project"]["foo"]["project"],
+    m3 = aiven.get_m3_db(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         service_name="my-m3db")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_m3db_user.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_opensearch_user.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
-    'GetM3dbUserResult',
-    'AwaitableGetM3dbUserResult',
-    'get_m3db_user',
-    'get_m3db_user_output',
+    'GetOpensearchUserResult',
+    'AwaitableGetOpensearchUserResult',
+    'get_opensearch_user',
+    'get_opensearch_user_output',
 ]
 
 @pulumi.output_type
-class GetM3dbUserResult:
+class GetOpensearchUserResult:
     """
-    A collection of values returned by getM3dbUser.
+    A collection of values returned by getOpensearchUser.
     """
     def __init__(__self__, id=None, password=None, project=None, service_name=None, type=None, username=None):
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
         if password and not isinstance(password, str):
             raise TypeError("Expected argument 'password' to be a str")
@@ -49,15 +49,15 @@
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def password(self) -> str:
         """
-        The password of the M3DB User.
+        The password of the Opensearch User.
         """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def project(self) -> str:
         """
@@ -81,90 +81,90 @@
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def username(self) -> str:
         """
-        The actual name of the M3DB User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+        The actual name of the Opensearch User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
         return pulumi.get(self, "username")
 
 
-class AwaitableGetM3dbUserResult(GetM3dbUserResult):
+class AwaitableGetOpensearchUserResult(GetOpensearchUserResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetM3dbUserResult(
+        return GetOpensearchUserResult(
             id=self.id,
             password=self.password,
             project=self.project,
             service_name=self.service_name,
             type=self.type,
             username=self.username)
 
 
-def get_m3db_user(project: Optional[str] = None,
-                  service_name: Optional[str] = None,
-                  username: Optional[str] = None,
-                  opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetM3dbUserResult:
+def get_opensearch_user(project: Optional[str] = None,
+                        service_name: Optional[str] = None,
+                        username: Optional[str] = None,
+                        opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetOpensearchUserResult:
     """
-    The M3DB User data source provides information about the existing Aiven M3DB User.
+    The Opensearch User data source provides information about the existing Aiven Cassandra User.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    user = aiven.get_m3db_user(project="my-project",
+    user = aiven.get_opensearch_user(project="my-project",
         service_name="my-service",
         username="user1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
-    :param str username: The actual name of the M3DB User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+    :param str username: The actual name of the Opensearch User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
     __args__ = dict()
     __args__['project'] = project
     __args__['serviceName'] = service_name
     __args__['username'] = username
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('aiven:index/getM3dbUser:getM3dbUser', __args__, opts=opts, typ=GetM3dbUserResult).value
+    __ret__ = pulumi.runtime.invoke('aiven:index/getOpensearchUser:getOpensearchUser', __args__, opts=opts, typ=GetOpensearchUserResult).value
 
-    return AwaitableGetM3dbUserResult(
+    return AwaitableGetOpensearchUserResult(
         id=__ret__.id,
         password=__ret__.password,
         project=__ret__.project,
         service_name=__ret__.service_name,
         type=__ret__.type,
         username=__ret__.username)
 
 
-@_utilities.lift_output_func(get_m3db_user)
-def get_m3db_user_output(project: Optional[pulumi.Input[str]] = None,
-                         service_name: Optional[pulumi.Input[str]] = None,
-                         username: Optional[pulumi.Input[str]] = None,
-                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetM3dbUserResult]:
+@_utilities.lift_output_func(get_opensearch_user)
+def get_opensearch_user_output(project: Optional[pulumi.Input[str]] = None,
+                               service_name: Optional[pulumi.Input[str]] = None,
+                               username: Optional[pulumi.Input[str]] = None,
+                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetOpensearchUserResult]:
     """
-    The M3DB User data source provides information about the existing Aiven M3DB User.
+    The Opensearch User data source provides information about the existing Aiven Cassandra User.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    user = aiven.get_m3db_user(project="my-project",
+    user = aiven.get_opensearch_user(project="my-project",
         service_name="my-service",
         username="user1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
-    :param str username: The actual name of the M3DB User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+    :param str username: The actual name of the Opensearch User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
     ...
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_mirror_maker_replication_flow.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_mirror_maker_replication_flow.py`

 * *Files 9% similar despite different names*

```diff
@@ -198,18 +198,18 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    f1 = aiven.get_mirror_maker_replication_flow(project=aiven_project["kafka-mm-project1"]["project"],
-        service_name=aiven_kafka["mm"]["service_name"],
-        source_cluster=aiven_kafka["source"]["service_name"],
-        target_cluster=aiven_kafka["target"]["service_name"])
+    f1 = aiven.get_mirror_maker_replication_flow(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+        source_cluster=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+        target_cluster=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference))
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str source_cluster: Source cluster alias. Maximum length: `128`.
     :param str target_cluster: Target cluster alias. Maximum length: `128`.
@@ -249,18 +249,18 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    f1 = aiven.get_mirror_maker_replication_flow(project=aiven_project["kafka-mm-project1"]["project"],
-        service_name=aiven_kafka["mm"]["service_name"],
-        source_cluster=aiven_kafka["source"]["service_name"],
-        target_cluster=aiven_kafka["target"]["service_name"])
+    f1 = aiven.get_mirror_maker_replication_flow(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+        source_cluster=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+        target_cluster=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference))
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str source_cluster: Source cluster alias. Maximum length: `128`.
     :param str target_cluster: Target cluster alias. Maximum length: `128`.
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_my_sql.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_my_sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -377,15 +377,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    mysql1 = aiven.get_my_sql(project=data["aiven_project"]["foo"]["project"],
+    mysql1 = aiven.get_my_sql(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         service_name="my-mysql1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
@@ -435,15 +435,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    mysql1 = aiven.get_my_sql(project=data["aiven_project"]["foo"]["project"],
+    mysql1 = aiven.get_my_sql(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         service_name="my-mysql1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_mysql_database.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_mysql_database.py`

 * *Files 12% similar despite different names*

```diff
@@ -98,16 +98,16 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    mydatabase = aiven.get_mysql_database(project=aiven_project["myproject"]["project"],
-        service_name=aiven_mysql["mymysql"]["service_name"],
+    mydatabase = aiven.get_mysql_database(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         database_name="<DATABASE_NAME>")
     ```
 
 
     :param str database_name: The name of the service database. This property cannot be changed, doing so forces recreation of the resource.
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
@@ -137,16 +137,16 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    mydatabase = aiven.get_mysql_database(project=aiven_project["myproject"]["project"],
-        service_name=aiven_mysql["mymysql"]["service_name"],
+    mydatabase = aiven.get_mysql_database(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         database_name="<DATABASE_NAME>")
     ```
 
 
     :param str database_name: The name of the service database. This property cannot be changed, doing so forces recreation of the resource.
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_mysql_user.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_mysql_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_open_search.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_open_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -377,15 +377,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    os1 = aiven.get_open_search(project=data["aiven_project"]["pr1"]["project"],
+    os1 = aiven.get_open_search(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         service_name="my-os1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
@@ -435,15 +435,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    os1 = aiven.get_open_search(project=data["aiven_project"]["pr1"]["project"],
+    os1 = aiven.get_open_search(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         service_name="my-os1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_open_search_acl_config.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_open_search_acl_config.py`

 * *Files 15% similar despite different names*

```diff
@@ -100,16 +100,16 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    os_acl_config = aiven.get_open_search_acl_config(project=aiven_project["os-project"]["project"],
-        service_name=aiven_opensearch["os"]["service_name"])
+    os_acl_config = aiven.get_open_search_acl_config(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference))
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
     __args__ = dict()
@@ -135,16 +135,16 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    os_acl_config = aiven.get_open_search_acl_config(project=aiven_project["os-project"]["project"],
-        service_name=aiven_opensearch["os"]["service_name"])
+    os_acl_config = aiven.get_open_search_acl_config(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference))
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
     ...
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_open_search_acl_rule.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_open_search_acl_rule.py`

 * *Files 4% similar despite different names*

```diff
@@ -115,16 +115,16 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    os_acl_rule = aiven.get_open_search_acl_rule(project=aiven_opensearch_acl_config["os_acls_config"]["project"],
-        service_name=aiven_opensearch_acl_config["os_acls_config"]["service_name"],
+    os_acl_rule = aiven.get_open_search_acl_rule(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         username="<USERNAME>",
         index="<INDEX>")
     ```
 
 
     :param str index: The index pattern for this ACL entry. Maximum length: `249`. This property cannot be changed, doing so forces recreation of the resource.
     :param str permission: The permissions for this ACL entry. The possible values are `deny`, `admin`, `read`, `readwrite` and `write`.
@@ -162,16 +162,16 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    os_acl_rule = aiven.get_open_search_acl_rule(project=aiven_opensearch_acl_config["os_acls_config"]["project"],
-        service_name=aiven_opensearch_acl_config["os_acls_config"]["service_name"],
+    os_acl_rule = aiven.get_open_search_acl_rule(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         username="<USERNAME>",
         index="<INDEX>")
     ```
 
 
     :param str index: The index pattern for this ACL entry. Maximum length: `249`. This property cannot be changed, doing so forces recreation of the resource.
     :param str permission: The permissions for this ACL entry. The possible values are `deny`, `admin`, `read`, `readwrite` and `write`.
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_opensearch_user.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_clickhouse_database.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,60 +6,57 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
-    'GetOpensearchUserResult',
-    'AwaitableGetOpensearchUserResult',
-    'get_opensearch_user',
-    'get_opensearch_user_output',
+    'GetClickhouseDatabaseResult',
+    'AwaitableGetClickhouseDatabaseResult',
+    'get_clickhouse_database',
+    'get_clickhouse_database_output',
 ]
 
 @pulumi.output_type
-class GetOpensearchUserResult:
+class GetClickhouseDatabaseResult:
     """
-    A collection of values returned by getOpensearchUser.
+    A collection of values returned by getClickhouseDatabase.
     """
-    def __init__(__self__, id=None, password=None, project=None, service_name=None, type=None, username=None):
+    def __init__(__self__, id=None, name=None, project=None, service_name=None, termination_protection=None):
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
-        if password and not isinstance(password, str):
-            raise TypeError("Expected argument 'password' to be a str")
-        pulumi.set(__self__, "password", password)
+        if name and not isinstance(name, str):
+            raise TypeError("Expected argument 'name' to be a str")
+        pulumi.set(__self__, "name", name)
         if project and not isinstance(project, str):
             raise TypeError("Expected argument 'project' to be a str")
         pulumi.set(__self__, "project", project)
         if service_name and not isinstance(service_name, str):
             raise TypeError("Expected argument 'service_name' to be a str")
         pulumi.set(__self__, "service_name", service_name)
-        if type and not isinstance(type, str):
-            raise TypeError("Expected argument 'type' to be a str")
-        pulumi.set(__self__, "type", type)
-        if username and not isinstance(username, str):
-            raise TypeError("Expected argument 'username' to be a str")
-        pulumi.set(__self__, "username", username)
+        if termination_protection and not isinstance(termination_protection, bool):
+            raise TypeError("Expected argument 'termination_protection' to be a bool")
+        pulumi.set(__self__, "termination_protection", termination_protection)
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
-    def password(self) -> str:
+    def name(self) -> str:
         """
-        The password of the Opensearch User.
+        The name of the Clickhouse database. This property cannot be changed, doing so forces recreation of the resource.
         """
-        return pulumi.get(self, "password")
+        return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def project(self) -> str:
         """
         Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
@@ -70,101 +67,88 @@
     def service_name(self) -> str:
         """
         Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
         return pulumi.get(self, "service_name")
 
     @property
-    @pulumi.getter
-    def type(self) -> str:
-        """
-        Type of the user account. Tells whether the user is the primary account or a regular account.
-        """
-        return pulumi.get(self, "type")
-
-    @property
-    @pulumi.getter
-    def username(self) -> str:
-        """
-        The actual name of the Opensearch User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
-        """
-        return pulumi.get(self, "username")
+    @pulumi.getter(name="terminationProtection")
+    def termination_protection(self) -> bool:
+        return pulumi.get(self, "termination_protection")
 
 
-class AwaitableGetOpensearchUserResult(GetOpensearchUserResult):
+class AwaitableGetClickhouseDatabaseResult(GetClickhouseDatabaseResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetOpensearchUserResult(
+        return GetClickhouseDatabaseResult(
             id=self.id,
-            password=self.password,
+            name=self.name,
             project=self.project,
             service_name=self.service_name,
-            type=self.type,
-            username=self.username)
+            termination_protection=self.termination_protection)
 
 
-def get_opensearch_user(project: Optional[str] = None,
-                        service_name: Optional[str] = None,
-                        username: Optional[str] = None,
-                        opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetOpensearchUserResult:
+def get_clickhouse_database(name: Optional[str] = None,
+                            project: Optional[str] = None,
+                            service_name: Optional[str] = None,
+                            opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetClickhouseDatabaseResult:
     """
-    The Opensearch User data source provides information about the existing Aiven Cassandra User.
+    The Clickhouse database data source provides information about the existing Aiven Clickhouse Database.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    user = aiven.get_opensearch_user(project="my-project",
-        service_name="my-service",
-        username="user1")
+    clickhouse_db = aiven.get_clickhouse_database(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+        name="my-ch-db")
     ```
 
 
+    :param str name: The name of the Clickhouse database. This property cannot be changed, doing so forces recreation of the resource.
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
-    :param str username: The actual name of the Opensearch User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
     __args__ = dict()
+    __args__['name'] = name
     __args__['project'] = project
     __args__['serviceName'] = service_name
-    __args__['username'] = username
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('aiven:index/getOpensearchUser:getOpensearchUser', __args__, opts=opts, typ=GetOpensearchUserResult).value
+    __ret__ = pulumi.runtime.invoke('aiven:index/getClickhouseDatabase:getClickhouseDatabase', __args__, opts=opts, typ=GetClickhouseDatabaseResult).value
 
-    return AwaitableGetOpensearchUserResult(
+    return AwaitableGetClickhouseDatabaseResult(
         id=__ret__.id,
-        password=__ret__.password,
+        name=__ret__.name,
         project=__ret__.project,
         service_name=__ret__.service_name,
-        type=__ret__.type,
-        username=__ret__.username)
+        termination_protection=__ret__.termination_protection)
 
 
-@_utilities.lift_output_func(get_opensearch_user)
-def get_opensearch_user_output(project: Optional[pulumi.Input[str]] = None,
-                               service_name: Optional[pulumi.Input[str]] = None,
-                               username: Optional[pulumi.Input[str]] = None,
-                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetOpensearchUserResult]:
+@_utilities.lift_output_func(get_clickhouse_database)
+def get_clickhouse_database_output(name: Optional[pulumi.Input[str]] = None,
+                                   project: Optional[pulumi.Input[str]] = None,
+                                   service_name: Optional[pulumi.Input[str]] = None,
+                                   opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetClickhouseDatabaseResult]:
     """
-    The Opensearch User data source provides information about the existing Aiven Cassandra User.
+    The Clickhouse database data source provides information about the existing Aiven Clickhouse Database.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    user = aiven.get_opensearch_user(project="my-project",
-        service_name="my-service",
-        username="user1")
+    clickhouse_db = aiven.get_clickhouse_database(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+        name="my-ch-db")
     ```
 
 
+    :param str name: The name of the Clickhouse database. This property cannot be changed, doing so forces recreation of the resource.
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
-    :param str username: The actual name of the Opensearch User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
     ...
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_pg.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_pg.py`

 * *Files 1% similar despite different names*

```diff
@@ -377,15 +377,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    pg = aiven.get_pg(project=data["aiven_project"]["pr1"]["project"],
+    pg = aiven.get_pg(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         service_name="my-pg1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
@@ -435,15 +435,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    pg = aiven.get_pg(project=data["aiven_project"]["pr1"]["project"],
+    pg = aiven.get_pg(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         service_name="my-pg1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_pg_database.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_pg_database.py`

 * *Files 11% similar despite different names*

```diff
@@ -122,16 +122,16 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    mydatabase = aiven.get_pg_database(project=aiven_project["myproject"]["project"],
-        service_name=aiven_pg["mypg"]["service_name"],
+    mydatabase = aiven.get_pg_database(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         database_name="<DATABASE_NAME>")
     ```
 
 
     :param str database_name: The name of the service database. This property cannot be changed, doing so forces recreation of the resource.
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
@@ -163,16 +163,16 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    mydatabase = aiven.get_pg_database(project=aiven_project["myproject"]["project"],
-        service_name=aiven_pg["mypg"]["service_name"],
+    mydatabase = aiven.get_pg_database(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         database_name="<DATABASE_NAME>")
     ```
 
 
     :param str database_name: The name of the service database. This property cannot be changed, doing so forces recreation of the resource.
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_pg_user.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_redis_user.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,101 +6,112 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
-    'GetPgUserResult',
-    'AwaitableGetPgUserResult',
-    'get_pg_user',
-    'get_pg_user_output',
+    'GetRedisUserResult',
+    'AwaitableGetRedisUserResult',
+    'get_redis_user',
+    'get_redis_user_output',
 ]
 
 @pulumi.output_type
-class GetPgUserResult:
+class GetRedisUserResult:
     """
-    A collection of values returned by getPgUser.
+    A collection of values returned by getRedisUser.
     """
-    def __init__(__self__, access_cert=None, access_key=None, id=None, password=None, pg_allow_replication=None, project=None, service_name=None, type=None, username=None):
-        if access_cert and not isinstance(access_cert, str):
-            raise TypeError("Expected argument 'access_cert' to be a str")
-        pulumi.set(__self__, "access_cert", access_cert)
-        if access_key and not isinstance(access_key, str):
-            raise TypeError("Expected argument 'access_key' to be a str")
-        pulumi.set(__self__, "access_key", access_key)
+    def __init__(__self__, id=None, password=None, project=None, redis_acl_categories=None, redis_acl_channels=None, redis_acl_commands=None, redis_acl_keys=None, service_name=None, type=None, username=None):
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
         if password and not isinstance(password, str):
             raise TypeError("Expected argument 'password' to be a str")
         pulumi.set(__self__, "password", password)
-        if pg_allow_replication and not isinstance(pg_allow_replication, bool):
-            raise TypeError("Expected argument 'pg_allow_replication' to be a bool")
-        pulumi.set(__self__, "pg_allow_replication", pg_allow_replication)
         if project and not isinstance(project, str):
             raise TypeError("Expected argument 'project' to be a str")
         pulumi.set(__self__, "project", project)
+        if redis_acl_categories and not isinstance(redis_acl_categories, list):
+            raise TypeError("Expected argument 'redis_acl_categories' to be a list")
+        pulumi.set(__self__, "redis_acl_categories", redis_acl_categories)
+        if redis_acl_channels and not isinstance(redis_acl_channels, list):
+            raise TypeError("Expected argument 'redis_acl_channels' to be a list")
+        pulumi.set(__self__, "redis_acl_channels", redis_acl_channels)
+        if redis_acl_commands and not isinstance(redis_acl_commands, list):
+            raise TypeError("Expected argument 'redis_acl_commands' to be a list")
+        pulumi.set(__self__, "redis_acl_commands", redis_acl_commands)
+        if redis_acl_keys and not isinstance(redis_acl_keys, list):
+            raise TypeError("Expected argument 'redis_acl_keys' to be a list")
+        pulumi.set(__self__, "redis_acl_keys", redis_acl_keys)
         if service_name and not isinstance(service_name, str):
             raise TypeError("Expected argument 'service_name' to be a str")
         pulumi.set(__self__, "service_name", service_name)
         if type and not isinstance(type, str):
             raise TypeError("Expected argument 'type' to be a str")
         pulumi.set(__self__, "type", type)
         if username and not isinstance(username, str):
             raise TypeError("Expected argument 'username' to be a str")
         pulumi.set(__self__, "username", username)
 
     @property
-    @pulumi.getter(name="accessCert")
-    def access_cert(self) -> str:
+    @pulumi.getter
+    def id(self) -> str:
         """
-        Access certificate for the user
+        The provider-assigned unique ID for this managed resource.
         """
-        return pulumi.get(self, "access_cert")
+        return pulumi.get(self, "id")
 
     @property
-    @pulumi.getter(name="accessKey")
-    def access_key(self) -> str:
+    @pulumi.getter
+    def password(self) -> str:
         """
-        Access certificate key for the user
+        The password of the Redis User.
         """
-        return pulumi.get(self, "access_key")
+        return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
-    def id(self) -> str:
+    def project(self) -> str:
         """
-        The provider-assigned unique ID for this managed resource.
+        Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
-        return pulumi.get(self, "id")
+        return pulumi.get(self, "project")
 
     @property
-    @pulumi.getter
-    def password(self) -> str:
+    @pulumi.getter(name="redisAclCategories")
+    def redis_acl_categories(self) -> Sequence[str]:
         """
-        The password of the PG User ( not applicable for all services ).
+        Defines command category rules. The field is required with`redis_acl_commands` and `redis_acl_keys`. This property cannot be changed, doing so forces recreation of the resource.
         """
-        return pulumi.get(self, "password")
+        return pulumi.get(self, "redis_acl_categories")
 
     @property
-    @pulumi.getter(name="pgAllowReplication")
-    def pg_allow_replication(self) -> bool:
+    @pulumi.getter(name="redisAclChannels")
+    def redis_acl_channels(self) -> Sequence[str]:
         """
-        Defines whether replication is allowed. This property cannot be changed, doing so forces recreation of the resource.
+        Defines the permitted pub/sub channel patterns. This property cannot be changed, doing so forces recreation of the resource.
         """
-        return pulumi.get(self, "pg_allow_replication")
+        return pulumi.get(self, "redis_acl_channels")
 
     @property
-    @pulumi.getter
-    def project(self) -> str:
+    @pulumi.getter(name="redisAclCommands")
+    def redis_acl_commands(self) -> Sequence[str]:
         """
-        Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+        Defines rules for individual commands. The field is required with`redis_acl_categories` and `redis_acl_keys`. This property cannot be changed, doing so forces recreation of the resource.
         """
-        return pulumi.get(self, "project")
+        return pulumi.get(self, "redis_acl_commands")
+
+    @property
+    @pulumi.getter(name="redisAclKeys")
+    def redis_acl_keys(self) -> Sequence[str]:
+        """
+        Defines key access rules. The field is required with`redis_acl_categories` and `redis_acl_keys`. This property cannot be changed, doing so forces recreation of the resource.
+        """
+        return pulumi.get(self, "redis_acl_keys")
 
     @property
     @pulumi.getter(name="serviceName")
     def service_name(self) -> str:
         """
         Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
@@ -114,96 +125,98 @@
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def username(self) -> str:
         """
-        The actual name of the PG User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+        The actual name of the Redis User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
         return pulumi.get(self, "username")
 
 
-class AwaitableGetPgUserResult(GetPgUserResult):
+class AwaitableGetRedisUserResult(GetRedisUserResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetPgUserResult(
-            access_cert=self.access_cert,
-            access_key=self.access_key,
+        return GetRedisUserResult(
             id=self.id,
             password=self.password,
-            pg_allow_replication=self.pg_allow_replication,
             project=self.project,
+            redis_acl_categories=self.redis_acl_categories,
+            redis_acl_channels=self.redis_acl_channels,
+            redis_acl_commands=self.redis_acl_commands,
+            redis_acl_keys=self.redis_acl_keys,
             service_name=self.service_name,
             type=self.type,
             username=self.username)
 
 
-def get_pg_user(project: Optional[str] = None,
-                service_name: Optional[str] = None,
-                username: Optional[str] = None,
-                opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPgUserResult:
+def get_redis_user(project: Optional[str] = None,
+                   service_name: Optional[str] = None,
+                   username: Optional[str] = None,
+                   opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetRedisUserResult:
     """
-    The PG User data source provides information about the existing Aiven PG User.
+    The Redis User data source provides information about the existing Aiven Redis User.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    user = aiven.get_pg_user(project="my-project",
+    user = aiven.get_redis_user(project="my-project",
         service_name="my-service",
         username="user1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
-    :param str username: The actual name of the PG User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+    :param str username: The actual name of the Redis User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
     __args__ = dict()
     __args__['project'] = project
     __args__['serviceName'] = service_name
     __args__['username'] = username
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('aiven:index/getPgUser:getPgUser', __args__, opts=opts, typ=GetPgUserResult).value
+    __ret__ = pulumi.runtime.invoke('aiven:index/getRedisUser:getRedisUser', __args__, opts=opts, typ=GetRedisUserResult).value
 
-    return AwaitableGetPgUserResult(
-        access_cert=__ret__.access_cert,
-        access_key=__ret__.access_key,
+    return AwaitableGetRedisUserResult(
         id=__ret__.id,
         password=__ret__.password,
-        pg_allow_replication=__ret__.pg_allow_replication,
         project=__ret__.project,
+        redis_acl_categories=__ret__.redis_acl_categories,
+        redis_acl_channels=__ret__.redis_acl_channels,
+        redis_acl_commands=__ret__.redis_acl_commands,
+        redis_acl_keys=__ret__.redis_acl_keys,
         service_name=__ret__.service_name,
         type=__ret__.type,
         username=__ret__.username)
 
 
-@_utilities.lift_output_func(get_pg_user)
-def get_pg_user_output(project: Optional[pulumi.Input[str]] = None,
-                       service_name: Optional[pulumi.Input[str]] = None,
-                       username: Optional[pulumi.Input[str]] = None,
-                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPgUserResult]:
+@_utilities.lift_output_func(get_redis_user)
+def get_redis_user_output(project: Optional[pulumi.Input[str]] = None,
+                          service_name: Optional[pulumi.Input[str]] = None,
+                          username: Optional[pulumi.Input[str]] = None,
+                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRedisUserResult]:
     """
-    The PG User data source provides information about the existing Aiven PG User.
+    The Redis User data source provides information about the existing Aiven Redis User.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    user = aiven.get_pg_user(project="my-project",
+    user = aiven.get_redis_user(project="my-project",
         service_name="my-service",
         username="user1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
-    :param str username: The actual name of the PG User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+    :param str username: The actual name of the Redis User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
     ...
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_project.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_project_user.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_project_user.py`

 * *Files 8% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    mytestuser = aiven.get_project_user(project=aiven_project["myproject"]["project"],
+    mytestuser = aiven.get_project_user(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         email="john.doe@example.com")
     ```
 
 
     :param str email: Email address of the user. This property cannot be changed, doing so forces recreation of the resource.
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
@@ -135,15 +135,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    mytestuser = aiven.get_project_user(project=aiven_project["myproject"]["project"],
+    mytestuser = aiven.get_project_user(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         email="john.doe@example.com")
     ```
 
 
     :param str email: Email address of the user. This property cannot be changed, doing so forces recreation of the resource.
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_project_vpc.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_project_vpc.py`

 * *Files 16% similar despite different names*

```diff
@@ -113,17 +113,17 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    myvpc = aiven.get_project_vpc(project=aiven_project["myproject"]["project"],
+    myvpc = aiven.get_project_vpc(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         cloud_name="google-europe-west1")
-    myvpc_id = aiven.get_project_vpc(vpc_id=aiven_project_vpc["vpc"]["id"])
+    myvpc_id = aiven.get_project_vpc(vpc_id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference))
     ```
 
 
     :param str cloud_name: Defines where the cloud provider and region where the service is hosted in. See the Service resource for additional information.
     :param str project: Identifies the project this resource belongs to.
     :param str vpc_id: ID of the VPC. This can be used to filter out the specific VPC if there are more than one datasource returned.
     """
@@ -153,17 +153,17 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    myvpc = aiven.get_project_vpc(project=aiven_project["myproject"]["project"],
+    myvpc = aiven.get_project_vpc(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         cloud_name="google-europe-west1")
-    myvpc_id = aiven.get_project_vpc(vpc_id=aiven_project_vpc["vpc"]["id"])
+    myvpc_id = aiven.get_project_vpc(vpc_id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference))
     ```
 
 
     :param str cloud_name: Defines where the cloud provider and region where the service is hosted in. See the Service resource for additional information.
     :param str project: Identifies the project this resource belongs to.
     :param str vpc_id: ID of the VPC. This can be used to filter out the specific VPC if there are more than one datasource returned.
     """
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_redis.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_redis.py`

 * *Files 1% similar despite different names*

```diff
@@ -377,15 +377,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    redis1 = aiven.get_redis(project=data["aiven_project"]["pr1"]["project"],
+    redis1 = aiven.get_redis(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         service_name="my-redis1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
@@ -435,15 +435,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    redis1 = aiven.get_redis(project=data["aiven_project"]["pr1"]["project"],
+    redis1 = aiven.get_redis(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         service_name="my-redis1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_redis_user.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_transit_gateway_vpc_attachment.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,217 +6,204 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
-    'GetRedisUserResult',
-    'AwaitableGetRedisUserResult',
-    'get_redis_user',
-    'get_redis_user_output',
+    'GetTransitGatewayVpcAttachmentResult',
+    'AwaitableGetTransitGatewayVpcAttachmentResult',
+    'get_transit_gateway_vpc_attachment',
+    'get_transit_gateway_vpc_attachment_output',
 ]
 
 @pulumi.output_type
-class GetRedisUserResult:
+class GetTransitGatewayVpcAttachmentResult:
     """
-    A collection of values returned by getRedisUser.
+    A collection of values returned by getTransitGatewayVpcAttachment.
     """
-    def __init__(__self__, id=None, password=None, project=None, redis_acl_categories=None, redis_acl_channels=None, redis_acl_commands=None, redis_acl_keys=None, service_name=None, type=None, username=None):
+    def __init__(__self__, id=None, peer_cloud_account=None, peer_region=None, peer_vpc=None, peering_connection_id=None, state=None, state_info=None, user_peer_network_cidrs=None, vpc_id=None):
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
-        if password and not isinstance(password, str):
-            raise TypeError("Expected argument 'password' to be a str")
-        pulumi.set(__self__, "password", password)
-        if project and not isinstance(project, str):
-            raise TypeError("Expected argument 'project' to be a str")
-        pulumi.set(__self__, "project", project)
-        if redis_acl_categories and not isinstance(redis_acl_categories, list):
-            raise TypeError("Expected argument 'redis_acl_categories' to be a list")
-        pulumi.set(__self__, "redis_acl_categories", redis_acl_categories)
-        if redis_acl_channels and not isinstance(redis_acl_channels, list):
-            raise TypeError("Expected argument 'redis_acl_channels' to be a list")
-        pulumi.set(__self__, "redis_acl_channels", redis_acl_channels)
-        if redis_acl_commands and not isinstance(redis_acl_commands, list):
-            raise TypeError("Expected argument 'redis_acl_commands' to be a list")
-        pulumi.set(__self__, "redis_acl_commands", redis_acl_commands)
-        if redis_acl_keys and not isinstance(redis_acl_keys, list):
-            raise TypeError("Expected argument 'redis_acl_keys' to be a list")
-        pulumi.set(__self__, "redis_acl_keys", redis_acl_keys)
-        if service_name and not isinstance(service_name, str):
-            raise TypeError("Expected argument 'service_name' to be a str")
-        pulumi.set(__self__, "service_name", service_name)
-        if type and not isinstance(type, str):
-            raise TypeError("Expected argument 'type' to be a str")
-        pulumi.set(__self__, "type", type)
-        if username and not isinstance(username, str):
-            raise TypeError("Expected argument 'username' to be a str")
-        pulumi.set(__self__, "username", username)
+        if peer_cloud_account and not isinstance(peer_cloud_account, str):
+            raise TypeError("Expected argument 'peer_cloud_account' to be a str")
+        pulumi.set(__self__, "peer_cloud_account", peer_cloud_account)
+        if peer_region and not isinstance(peer_region, str):
+            raise TypeError("Expected argument 'peer_region' to be a str")
+        pulumi.set(__self__, "peer_region", peer_region)
+        if peer_vpc and not isinstance(peer_vpc, str):
+            raise TypeError("Expected argument 'peer_vpc' to be a str")
+        pulumi.set(__self__, "peer_vpc", peer_vpc)
+        if peering_connection_id and not isinstance(peering_connection_id, str):
+            raise TypeError("Expected argument 'peering_connection_id' to be a str")
+        pulumi.set(__self__, "peering_connection_id", peering_connection_id)
+        if state and not isinstance(state, str):
+            raise TypeError("Expected argument 'state' to be a str")
+        pulumi.set(__self__, "state", state)
+        if state_info and not isinstance(state_info, dict):
+            raise TypeError("Expected argument 'state_info' to be a dict")
+        pulumi.set(__self__, "state_info", state_info)
+        if user_peer_network_cidrs and not isinstance(user_peer_network_cidrs, list):
+            raise TypeError("Expected argument 'user_peer_network_cidrs' to be a list")
+        pulumi.set(__self__, "user_peer_network_cidrs", user_peer_network_cidrs)
+        if vpc_id and not isinstance(vpc_id, str):
+            raise TypeError("Expected argument 'vpc_id' to be a str")
+        pulumi.set(__self__, "vpc_id", vpc_id)
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
-    @pulumi.getter
-    def password(self) -> str:
+    @pulumi.getter(name="peerCloudAccount")
+    def peer_cloud_account(self) -> str:
         """
-        The password of the Redis User.
+        AWS account ID or GCP project ID of the peered VPC. This property cannot be changed, doing so forces recreation of the resource.
         """
-        return pulumi.get(self, "password")
+        return pulumi.get(self, "peer_cloud_account")
 
     @property
-    @pulumi.getter
-    def project(self) -> str:
+    @pulumi.getter(name="peerRegion")
+    def peer_region(self) -> str:
         """
-        Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+        AWS region of the peered VPC (if not in the same region as Aiven VPC)
         """
-        return pulumi.get(self, "project")
+        return pulumi.get(self, "peer_region")
 
     @property
-    @pulumi.getter(name="redisAclCategories")
-    def redis_acl_categories(self) -> Sequence[str]:
+    @pulumi.getter(name="peerVpc")
+    def peer_vpc(self) -> str:
         """
-        Defines command category rules. The field is required with`redis_acl_commands` and `redis_acl_keys`. This property cannot be changed, doing so forces recreation of the resource.
+        Transit gateway ID. This property cannot be changed, doing so forces recreation of the resource.
         """
-        return pulumi.get(self, "redis_acl_categories")
+        return pulumi.get(self, "peer_vpc")
 
     @property
-    @pulumi.getter(name="redisAclChannels")
-    def redis_acl_channels(self) -> Sequence[str]:
+    @pulumi.getter(name="peeringConnectionId")
+    def peering_connection_id(self) -> str:
         """
-        Defines the permitted pub/sub channel patterns. This property cannot be changed, doing so forces recreation of the resource.
+        Cloud provider identifier for the peering connection if available
         """
-        return pulumi.get(self, "redis_acl_channels")
+        return pulumi.get(self, "peering_connection_id")
 
     @property
-    @pulumi.getter(name="redisAclCommands")
-    def redis_acl_commands(self) -> Sequence[str]:
-        """
-        Defines rules for individual commands. The field is required with`redis_acl_categories` and `redis_acl_keys`. This property cannot be changed, doing so forces recreation of the resource.
-        """
-        return pulumi.get(self, "redis_acl_commands")
-
-    @property
-    @pulumi.getter(name="redisAclKeys")
-    def redis_acl_keys(self) -> Sequence[str]:
+    @pulumi.getter
+    def state(self) -> str:
         """
-        Defines key access rules. The field is required with`redis_acl_categories` and `redis_acl_keys`. This property cannot be changed, doing so forces recreation of the resource.
+        State of the peering connection
         """
-        return pulumi.get(self, "redis_acl_keys")
+        return pulumi.get(self, "state")
 
     @property
-    @pulumi.getter(name="serviceName")
-    def service_name(self) -> str:
+    @pulumi.getter(name="stateInfo")
+    def state_info(self) -> Mapping[str, Any]:
         """
-        Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+        State-specific help or error information
         """
-        return pulumi.get(self, "service_name")
+        return pulumi.get(self, "state_info")
 
     @property
-    @pulumi.getter
-    def type(self) -> str:
+    @pulumi.getter(name="userPeerNetworkCidrs")
+    def user_peer_network_cidrs(self) -> Sequence[str]:
         """
-        Type of the user account. Tells whether the user is the primary account or a regular account.
+        List of private IPv4 ranges to route through the peering connection
         """
-        return pulumi.get(self, "type")
+        return pulumi.get(self, "user_peer_network_cidrs")
 
     @property
-    @pulumi.getter
-    def username(self) -> str:
+    @pulumi.getter(name="vpcId")
+    def vpc_id(self) -> str:
         """
-        The actual name of the Redis User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+        The VPC the peering connection belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
-        return pulumi.get(self, "username")
+        return pulumi.get(self, "vpc_id")
 
 
-class AwaitableGetRedisUserResult(GetRedisUserResult):
+class AwaitableGetTransitGatewayVpcAttachmentResult(GetTransitGatewayVpcAttachmentResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetRedisUserResult(
+        return GetTransitGatewayVpcAttachmentResult(
             id=self.id,
-            password=self.password,
-            project=self.project,
-            redis_acl_categories=self.redis_acl_categories,
-            redis_acl_channels=self.redis_acl_channels,
-            redis_acl_commands=self.redis_acl_commands,
-            redis_acl_keys=self.redis_acl_keys,
-            service_name=self.service_name,
-            type=self.type,
-            username=self.username)
-
-
-def get_redis_user(project: Optional[str] = None,
-                   service_name: Optional[str] = None,
-                   username: Optional[str] = None,
-                   opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetRedisUserResult:
+            peer_cloud_account=self.peer_cloud_account,
+            peer_region=self.peer_region,
+            peer_vpc=self.peer_vpc,
+            peering_connection_id=self.peering_connection_id,
+            state=self.state,
+            state_info=self.state_info,
+            user_peer_network_cidrs=self.user_peer_network_cidrs,
+            vpc_id=self.vpc_id)
+
+
+def get_transit_gateway_vpc_attachment(peer_cloud_account: Optional[str] = None,
+                                       peer_vpc: Optional[str] = None,
+                                       vpc_id: Optional[str] = None,
+                                       opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetTransitGatewayVpcAttachmentResult:
     """
-    The Redis User data source provides information about the existing Aiven Redis User.
+    The Transit Gateway VPC Attachment resource allows the creation and management Transit Gateway VPC Attachment VPC peering connection between Aiven and AWS.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    user = aiven.get_redis_user(project="my-project",
-        service_name="my-service",
-        username="user1")
+    attachment = aiven.get_transit_gateway_vpc_attachment(vpc_id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+        peer_cloud_account="<PEER_ACCOUNT_ID>",
+        peer_vpc="google-project1")
     ```
 
 
-    :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
-    :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
-    :param str username: The actual name of the Redis User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+    :param str peer_cloud_account: AWS account ID or GCP project ID of the peered VPC. This property cannot be changed, doing so forces recreation of the resource.
+    :param str peer_vpc: Transit gateway ID. This property cannot be changed, doing so forces recreation of the resource.
+    :param str vpc_id: The VPC the peering connection belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
     __args__ = dict()
-    __args__['project'] = project
-    __args__['serviceName'] = service_name
-    __args__['username'] = username
+    __args__['peerCloudAccount'] = peer_cloud_account
+    __args__['peerVpc'] = peer_vpc
+    __args__['vpcId'] = vpc_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('aiven:index/getRedisUser:getRedisUser', __args__, opts=opts, typ=GetRedisUserResult).value
+    __ret__ = pulumi.runtime.invoke('aiven:index/getTransitGatewayVpcAttachment:getTransitGatewayVpcAttachment', __args__, opts=opts, typ=GetTransitGatewayVpcAttachmentResult).value
 
-    return AwaitableGetRedisUserResult(
+    return AwaitableGetTransitGatewayVpcAttachmentResult(
         id=__ret__.id,
-        password=__ret__.password,
-        project=__ret__.project,
-        redis_acl_categories=__ret__.redis_acl_categories,
-        redis_acl_channels=__ret__.redis_acl_channels,
-        redis_acl_commands=__ret__.redis_acl_commands,
-        redis_acl_keys=__ret__.redis_acl_keys,
-        service_name=__ret__.service_name,
-        type=__ret__.type,
-        username=__ret__.username)
-
-
-@_utilities.lift_output_func(get_redis_user)
-def get_redis_user_output(project: Optional[pulumi.Input[str]] = None,
-                          service_name: Optional[pulumi.Input[str]] = None,
-                          username: Optional[pulumi.Input[str]] = None,
-                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRedisUserResult]:
+        peer_cloud_account=__ret__.peer_cloud_account,
+        peer_region=__ret__.peer_region,
+        peer_vpc=__ret__.peer_vpc,
+        peering_connection_id=__ret__.peering_connection_id,
+        state=__ret__.state,
+        state_info=__ret__.state_info,
+        user_peer_network_cidrs=__ret__.user_peer_network_cidrs,
+        vpc_id=__ret__.vpc_id)
+
+
+@_utilities.lift_output_func(get_transit_gateway_vpc_attachment)
+def get_transit_gateway_vpc_attachment_output(peer_cloud_account: Optional[pulumi.Input[str]] = None,
+                                              peer_vpc: Optional[pulumi.Input[str]] = None,
+                                              vpc_id: Optional[pulumi.Input[str]] = None,
+                                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetTransitGatewayVpcAttachmentResult]:
     """
-    The Redis User data source provides information about the existing Aiven Redis User.
+    The Transit Gateway VPC Attachment resource allows the creation and management Transit Gateway VPC Attachment VPC peering connection between Aiven and AWS.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    user = aiven.get_redis_user(project="my-project",
-        service_name="my-service",
-        username="user1")
+    attachment = aiven.get_transit_gateway_vpc_attachment(vpc_id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+        peer_cloud_account="<PEER_ACCOUNT_ID>",
+        peer_vpc="google-project1")
     ```
 
 
-    :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
-    :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
-    :param str username: The actual name of the Redis User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+    :param str peer_cloud_account: AWS account ID or GCP project ID of the peered VPC. This property cannot be changed, doing so forces recreation of the resource.
+    :param str peer_vpc: Transit gateway ID. This property cannot be changed, doing so forces recreation of the resource.
+    :param str vpc_id: The VPC the peering connection belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
     ...
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_service_component.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_service_component.py`

 * *Files 4% similar despite different names*

```diff
@@ -167,16 +167,16 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    sc1 = aiven.get_service_component(project=aiven_kafka["project1"]["project"],
-        service_name=aiven_kafka["service1"]["service_name"],
+    sc1 = aiven.get_service_component(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         component="kafka",
         route="dynamic",
         kafka_authentication_method="certificate")
     ```
 
 
     :param str component: Service component name
@@ -227,16 +227,16 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    sc1 = aiven.get_service_component(project=aiven_kafka["project1"]["project"],
-        service_name=aiven_kafka["service1"]["service_name"],
+    sc1 = aiven.get_service_component(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         component="kafka",
         route="dynamic",
         kafka_authentication_method="certificate")
     ```
 
 
     :param str component: Service component name
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_service_integration.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_service_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -249,15 +249,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    myintegration = aiven.get_service_integration(project=aiven_project["myproject"]["project"],
+    myintegration = aiven.get_service_integration(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         destination_service_name="<DESTINATION_SERVICE_NAME>",
         integration_type="datadog",
         source_service_name="<SOURCE_SERVICE_NAME>")
     ```
 
 
     :param str destination_service_name: Destination service for the integration (if any)
@@ -306,15 +306,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    myintegration = aiven.get_service_integration(project=aiven_project["myproject"]["project"],
+    myintegration = aiven.get_service_integration(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         destination_service_name="<DESTINATION_SERVICE_NAME>",
         integration_type="datadog",
         source_service_name="<SOURCE_SERVICE_NAME>")
     ```
 
 
     :param str destination_service_name: Destination service for the integration (if any)
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/get_service_integration_endpoint.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/get_service_integration_endpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ]
 
 @pulumi.output_type
 class GetServiceIntegrationEndpointResult:
     """
     A collection of values returned by getServiceIntegrationEndpoint.
     """
-    def __init__(__self__, datadog_user_configs=None, endpoint_config=None, endpoint_name=None, endpoint_type=None, external_aws_cloudwatch_logs_user_configs=None, external_aws_cloudwatch_metrics_user_configs=None, external_elasticsearch_logs_user_configs=None, external_google_cloud_logging_user_configs=None, external_kafka_user_configs=None, external_opensearch_logs_user_configs=None, external_schema_registry_user_configs=None, id=None, jolokia_user_configs=None, project=None, prometheus_user_configs=None, rsyslog_user_configs=None, signalfx_user_configs=None):
+    def __init__(__self__, datadog_user_configs=None, endpoint_config=None, endpoint_name=None, endpoint_type=None, external_aws_cloudwatch_logs_user_configs=None, external_aws_cloudwatch_metrics_user_configs=None, external_elasticsearch_logs_user_configs=None, external_google_cloud_logging_user_configs=None, external_kafka_user_configs=None, external_opensearch_logs_user_configs=None, external_schema_registry_user_configs=None, id=None, jolokia_user_configs=None, project=None, prometheus_user_configs=None, rsyslog_user_configs=None):
         if datadog_user_configs and not isinstance(datadog_user_configs, list):
             raise TypeError("Expected argument 'datadog_user_configs' to be a list")
         pulumi.set(__self__, "datadog_user_configs", datadog_user_configs)
         if endpoint_config and not isinstance(endpoint_config, dict):
             raise TypeError("Expected argument 'endpoint_config' to be a dict")
         pulumi.set(__self__, "endpoint_config", endpoint_config)
         if endpoint_name and not isinstance(endpoint_name, str):
@@ -67,17 +67,14 @@
         pulumi.set(__self__, "project", project)
         if prometheus_user_configs and not isinstance(prometheus_user_configs, list):
             raise TypeError("Expected argument 'prometheus_user_configs' to be a list")
         pulumi.set(__self__, "prometheus_user_configs", prometheus_user_configs)
         if rsyslog_user_configs and not isinstance(rsyslog_user_configs, list):
             raise TypeError("Expected argument 'rsyslog_user_configs' to be a list")
         pulumi.set(__self__, "rsyslog_user_configs", rsyslog_user_configs)
-        if signalfx_user_configs and not isinstance(signalfx_user_configs, list):
-            raise TypeError("Expected argument 'signalfx_user_configs' to be a list")
-        pulumi.set(__self__, "signalfx_user_configs", signalfx_user_configs)
 
     @property
     @pulumi.getter(name="datadogUserConfigs")
     def datadog_user_configs(self) -> Sequence['outputs.GetServiceIntegrationEndpointDatadogUserConfigResult']:
         """
         Datadog user configurable settings
         """
@@ -99,15 +96,15 @@
         """
         return pulumi.get(self, "endpoint_name")
 
     @property
     @pulumi.getter(name="endpointType")
     def endpoint_type(self) -> str:
         """
-        Type of the service integration endpoint
+        Type of the service integration endpoint. Possible values: `datadog`, `prometheus`, `rsyslog`, `external_elasticsearch_logs`, `external_opensearch_logs`, `external_aws_cloudwatch_logs`, `external_google_cloud_logging`, `external_kafka`, `jolokia`, `external_schema_registry`, `external_aws_cloudwatch_metrics`
         """
         return pulumi.get(self, "endpoint_type")
 
     @property
     @pulumi.getter(name="externalAwsCloudwatchLogsUserConfigs")
     def external_aws_cloudwatch_logs_user_configs(self) -> Sequence['outputs.GetServiceIntegrationEndpointExternalAwsCloudwatchLogsUserConfigResult']:
         """
@@ -199,22 +196,14 @@
     @pulumi.getter(name="rsyslogUserConfigs")
     def rsyslog_user_configs(self) -> Sequence['outputs.GetServiceIntegrationEndpointRsyslogUserConfigResult']:
         """
         Rsyslog user configurable settings
         """
         return pulumi.get(self, "rsyslog_user_configs")
 
-    @property
-    @pulumi.getter(name="signalfxUserConfigs")
-    def signalfx_user_configs(self) -> Sequence['outputs.GetServiceIntegrationEndpointSignalfxUserConfigResult']:
-        """
-        Signalfx user configurable settings
-        """
-        return pulumi.get(self, "signalfx_user_configs")
-
 
 class AwaitableGetServiceIntegrationEndpointResult(GetServiceIntegrationEndpointResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
         return GetServiceIntegrationEndpointResult(
@@ -229,31 +218,30 @@
             external_kafka_user_configs=self.external_kafka_user_configs,
             external_opensearch_logs_user_configs=self.external_opensearch_logs_user_configs,
             external_schema_registry_user_configs=self.external_schema_registry_user_configs,
             id=self.id,
             jolokia_user_configs=self.jolokia_user_configs,
             project=self.project,
             prometheus_user_configs=self.prometheus_user_configs,
-            rsyslog_user_configs=self.rsyslog_user_configs,
-            signalfx_user_configs=self.signalfx_user_configs)
+            rsyslog_user_configs=self.rsyslog_user_configs)
 
 
 def get_service_integration_endpoint(endpoint_name: Optional[str] = None,
                                      project: Optional[str] = None,
                                      opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetServiceIntegrationEndpointResult:
     """
     The Service Integration Endpoint data source provides information about the existing Aiven Service Integration Endpoint.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    myendpoint = aiven.get_service_integration_endpoint(project=aiven_project["myproject"]["project"],
+    myendpoint = aiven.get_service_integration_endpoint(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         endpoint_name="<ENDPOINT_NAME>")
     ```
 
 
     :param str endpoint_name: Name of the service integration endpoint
     :param str project: Project the service integration endpoint belongs to
     """
@@ -275,16 +263,15 @@
         external_kafka_user_configs=__ret__.external_kafka_user_configs,
         external_opensearch_logs_user_configs=__ret__.external_opensearch_logs_user_configs,
         external_schema_registry_user_configs=__ret__.external_schema_registry_user_configs,
         id=__ret__.id,
         jolokia_user_configs=__ret__.jolokia_user_configs,
         project=__ret__.project,
         prometheus_user_configs=__ret__.prometheus_user_configs,
-        rsyslog_user_configs=__ret__.rsyslog_user_configs,
-        signalfx_user_configs=__ret__.signalfx_user_configs)
+        rsyslog_user_configs=__ret__.rsyslog_user_configs)
 
 
 @_utilities.lift_output_func(get_service_integration_endpoint)
 def get_service_integration_endpoint_output(endpoint_name: Optional[pulumi.Input[str]] = None,
                                             project: Optional[pulumi.Input[str]] = None,
                                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetServiceIntegrationEndpointResult]:
     """
@@ -292,15 +279,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    myendpoint = aiven.get_service_integration_endpoint(project=aiven_project["myproject"]["project"],
+    myendpoint = aiven.get_service_integration_endpoint(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         endpoint_name="<ENDPOINT_NAME>")
     ```
 
 
     :param str endpoint_name: Name of the service integration endpoint
     :param str project: Project the service integration endpoint belongs to
     """
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/grafana.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/grafana.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,17 @@
         """
         pulumi.set(__self__, "project", project)
         if additional_disk_space is not None:
             pulumi.set(__self__, "additional_disk_space", additional_disk_space)
         if cloud_name is not None:
             pulumi.set(__self__, "cloud_name", cloud_name)
         if disk_space is not None:
+            warnings.warn("""This will be removed in v5.0.0 and replaced with additional_disk_space instead.""", DeprecationWarning)
+            pulumi.log.warn("""disk_space is deprecated: This will be removed in v5.0.0 and replaced with additional_disk_space instead.""")
+        if disk_space is not None:
             pulumi.set(__self__, "disk_space", disk_space)
         if grafana_user_config is not None:
             pulumi.set(__self__, "grafana_user_config", grafana_user_config)
         if maintenance_window_dow is not None:
             pulumi.set(__self__, "maintenance_window_dow", maintenance_window_dow)
         if maintenance_window_time is not None:
             pulumi.set(__self__, "maintenance_window_time", maintenance_window_time)
@@ -369,14 +372,17 @@
         if additional_disk_space is not None:
             pulumi.set(__self__, "additional_disk_space", additional_disk_space)
         if cloud_name is not None:
             pulumi.set(__self__, "cloud_name", cloud_name)
         if components is not None:
             pulumi.set(__self__, "components", components)
         if disk_space is not None:
+            warnings.warn("""This will be removed in v5.0.0 and replaced with additional_disk_space instead.""", DeprecationWarning)
+            pulumi.log.warn("""disk_space is deprecated: This will be removed in v5.0.0 and replaced with additional_disk_space instead.""")
+        if disk_space is not None:
             pulumi.set(__self__, "disk_space", disk_space)
         if disk_space_cap is not None:
             pulumi.set(__self__, "disk_space_cap", disk_space_cap)
         if disk_space_default is not None:
             pulumi.set(__self__, "disk_space_default", disk_space_default)
         if disk_space_step is not None:
             pulumi.set(__self__, "disk_space_step", disk_space_step)
@@ -925,14 +931,17 @@
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = GrafanaArgs.__new__(GrafanaArgs)
 
             __props__.__dict__["additional_disk_space"] = additional_disk_space
             __props__.__dict__["cloud_name"] = cloud_name
+            if disk_space is not None and not opts.urn:
+                warnings.warn("""This will be removed in v5.0.0 and replaced with additional_disk_space instead.""", DeprecationWarning)
+                pulumi.log.warn("""disk_space is deprecated: This will be removed in v5.0.0 and replaced with additional_disk_space instead.""")
             __props__.__dict__["disk_space"] = disk_space
             __props__.__dict__["grafana_user_config"] = grafana_user_config
             __props__.__dict__["maintenance_window_dow"] = maintenance_window_dow
             __props__.__dict__["maintenance_window_time"] = maintenance_window_time
             __props__.__dict__["plan"] = plan
             if project is None and not opts.urn:
                 raise TypeError("Missing required property 'project'")
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/influx_db.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/influx_db.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,17 @@
         pulumi.set(__self__, "project", project)
         pulumi.set(__self__, "service_name", service_name)
         if additional_disk_space is not None:
             pulumi.set(__self__, "additional_disk_space", additional_disk_space)
         if cloud_name is not None:
             pulumi.set(__self__, "cloud_name", cloud_name)
         if disk_space is not None:
+            warnings.warn("""This will be removed in v5.0.0 and replaced with additional_disk_space instead.""", DeprecationWarning)
+            pulumi.log.warn("""disk_space is deprecated: This will be removed in v5.0.0 and replaced with additional_disk_space instead.""")
+        if disk_space is not None:
             pulumi.set(__self__, "disk_space", disk_space)
         if influxdb_user_config is not None:
             pulumi.set(__self__, "influxdb_user_config", influxdb_user_config)
         if maintenance_window_dow is not None:
             pulumi.set(__self__, "maintenance_window_dow", maintenance_window_dow)
         if maintenance_window_time is not None:
             pulumi.set(__self__, "maintenance_window_time", maintenance_window_time)
@@ -306,14 +309,17 @@
         if additional_disk_space is not None:
             pulumi.set(__self__, "additional_disk_space", additional_disk_space)
         if cloud_name is not None:
             pulumi.set(__self__, "cloud_name", cloud_name)
         if components is not None:
             pulumi.set(__self__, "components", components)
         if disk_space is not None:
+            warnings.warn("""This will be removed in v5.0.0 and replaced with additional_disk_space instead.""", DeprecationWarning)
+            pulumi.log.warn("""disk_space is deprecated: This will be removed in v5.0.0 and replaced with additional_disk_space instead.""")
+        if disk_space is not None:
             pulumi.set(__self__, "disk_space", disk_space)
         if disk_space_cap is not None:
             pulumi.set(__self__, "disk_space_cap", disk_space_cap)
         if disk_space_default is not None:
             pulumi.set(__self__, "disk_space_default", disk_space_default)
         if disk_space_step is not None:
             pulumi.set(__self__, "disk_space_step", disk_space_step)
@@ -820,14 +826,17 @@
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = InfluxDbArgs.__new__(InfluxDbArgs)
 
             __props__.__dict__["additional_disk_space"] = additional_disk_space
             __props__.__dict__["cloud_name"] = cloud_name
+            if disk_space is not None and not opts.urn:
+                warnings.warn("""This will be removed in v5.0.0 and replaced with additional_disk_space instead.""", DeprecationWarning)
+                pulumi.log.warn("""disk_space is deprecated: This will be removed in v5.0.0 and replaced with additional_disk_space instead.""")
             __props__.__dict__["disk_space"] = disk_space
             __props__.__dict__["influxdb_user_config"] = influxdb_user_config
             __props__.__dict__["maintenance_window_dow"] = maintenance_window_dow
             __props__.__dict__["maintenance_window_time"] = maintenance_window_time
             __props__.__dict__["plan"] = plan
             if project is None and not opts.urn:
                 raise TypeError("Missing required property 'project'")
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/influxdb_database.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/influxdb_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/influxdb_user.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/influxdb_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,14 +222,20 @@
         foo = aiven.InfluxdbUser("foo",
             service_name=aiven_influxdb["bar"]["service_name"],
             project="my-project",
             username="user-1",
             password="Test$1234")
         ```
 
+        ## Import
+
+        ```sh
+         $ pulumi import aiven:index/influxdbUser:InfluxdbUser foo project/service_name/username
+        ```
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] password: The password of the InfluxDB User.
         :param pulumi.Input[str] project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] username: The actual name of the InfluxDB User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
@@ -251,14 +257,20 @@
         foo = aiven.InfluxdbUser("foo",
             service_name=aiven_influxdb["bar"]["service_name"],
             project="my-project",
             username="user-1",
             password="Test$1234")
         ```
 
+        ## Import
+
+        ```sh
+         $ pulumi import aiven:index/influxdbUser:InfluxdbUser foo project/service_name/username
+        ```
+
         :param str resource_name: The name of the resource.
         :param InfluxdbUserArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(InfluxdbUserArgs, pulumi.ResourceOptions, *args, **kwargs)
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/kafka.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/kafka.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     def __init__(__self__, *,
                  project: pulumi.Input[str],
                  service_name: pulumi.Input[str],
                  additional_disk_space: Optional[pulumi.Input[str]] = None,
                  cloud_name: Optional[pulumi.Input[str]] = None,
                  default_acl: Optional[pulumi.Input[bool]] = None,
                  disk_space: Optional[pulumi.Input[str]] = None,
-                 kafka: Optional[pulumi.Input['KafkaKafkaArgs']] = None,
                  kafka_user_config: Optional[pulumi.Input['KafkaKafkaUserConfigArgs']] = None,
                  karapace: Optional[pulumi.Input[bool]] = None,
                  maintenance_window_dow: Optional[pulumi.Input[str]] = None,
                  maintenance_window_time: Optional[pulumi.Input[str]] = None,
                  plan: Optional[pulumi.Input[str]] = None,
                  project_vpc_id: Optional[pulumi.Input[str]] = None,
                  service_integrations: Optional[pulumi.Input[Sequence[pulumi.Input['KafkaServiceIntegrationArgs']]]] = None,
@@ -37,15 +36,14 @@
         The set of arguments for constructing a Kafka resource.
         :param pulumi.Input[str] project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
         :param pulumi.Input[str] additional_disk_space: Additional disk space. Possible values depend on the service type, the cloud provider and the project. Therefore, reducing will result in the service rebalancing.
         :param pulumi.Input[str] cloud_name: Defines where the cloud provider and region where the service is hosted in. This can be changed freely after service is created. Changing the value will trigger a potentially lengthy migration process for the service. Format is cloud provider name (`aws`, `azure`, `do` `google`, `upcloud`, etc.), dash, and the cloud provider specific region name. These are documented on each Cloud provider's own support articles, like [here for Google](https://cloud.google.com/compute/docs/regions-zones/) and [here for AWS](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Concepts.RegionsAndAvailabilityZones.html).
         :param pulumi.Input[bool] default_acl: Create default wildcard Kafka ACL
         :param pulumi.Input[str] disk_space: Service disk space. Possible values depend on the service type, the cloud provider and the project. Therefore, reducing will result in the service rebalancing.
-        :param pulumi.Input['KafkaKafkaArgs'] kafka: Kafka server provided values
         :param pulumi.Input['KafkaKafkaUserConfigArgs'] kafka_user_config: Kafka user configurable settings
         :param pulumi.Input[bool] karapace: Switch the service to use Karapace for schema registry and REST proxy
         :param pulumi.Input[str] maintenance_window_dow: Day of week when maintenance operations should be performed. One monday, tuesday, wednesday, etc.
         :param pulumi.Input[str] maintenance_window_time: Time of day when maintenance operations should be performed. UTC time in HH:mm:ss format.
         :param pulumi.Input[str] plan: Defines what kind of computing resources are allocated for the service. It can be changed after creation, though there are some restrictions when going to a smaller plan such as the new plan must have sufficient amount of disk space to store all current data and switching to a plan with fewer nodes might not be supported. The basic plan names are `hobbyist`, `startup-x`, `business-x` and `premium-x` where `x` is (roughly) the amount of memory on each node (also other attributes like number of CPUs and amount of disk space varies but naming is based on memory). The available options can be seem from the [Aiven pricing page](https://aiven.io/pricing).
         :param pulumi.Input[str] project_vpc_id: Specifies the VPC the service should run in. If the value is not set the service is not run inside a VPC. When set, the value should be given as a reference to set up dependencies correctly and the VPC must be in the same cloud and region as the service itself. Project can be freely moved to and from VPC after creation but doing so triggers migration to new servers so the operation can take significant amount of time to complete if the service has a lot of data.
         :param pulumi.Input[Sequence[pulumi.Input['KafkaServiceIntegrationArgs']]] service_integrations: Service integrations to specify when creating a service. Not applied after initial service creation
@@ -58,20 +56,24 @@
         if additional_disk_space is not None:
             pulumi.set(__self__, "additional_disk_space", additional_disk_space)
         if cloud_name is not None:
             pulumi.set(__self__, "cloud_name", cloud_name)
         if default_acl is not None:
             pulumi.set(__self__, "default_acl", default_acl)
         if disk_space is not None:
+            warnings.warn("""This will be removed in v5.0.0 and replaced with additional_disk_space instead.""", DeprecationWarning)
+            pulumi.log.warn("""disk_space is deprecated: This will be removed in v5.0.0 and replaced with additional_disk_space instead.""")
+        if disk_space is not None:
             pulumi.set(__self__, "disk_space", disk_space)
-        if kafka is not None:
-            pulumi.set(__self__, "kafka", kafka)
         if kafka_user_config is not None:
             pulumi.set(__self__, "kafka_user_config", kafka_user_config)
         if karapace is not None:
+            warnings.warn("""Usage of this field is discouraged.""", DeprecationWarning)
+            pulumi.log.warn("""karapace is deprecated: Usage of this field is discouraged.""")
+        if karapace is not None:
             pulumi.set(__self__, "karapace", karapace)
         if maintenance_window_dow is not None:
             pulumi.set(__self__, "maintenance_window_dow", maintenance_window_dow)
         if maintenance_window_time is not None:
             pulumi.set(__self__, "maintenance_window_time", maintenance_window_time)
         if plan is not None:
             pulumi.set(__self__, "plan", plan)
@@ -155,26 +157,14 @@
         return pulumi.get(self, "disk_space")
 
     @disk_space.setter
     def disk_space(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "disk_space", value)
 
     @property
-    @pulumi.getter
-    def kafka(self) -> Optional[pulumi.Input['KafkaKafkaArgs']]:
-        """
-        Kafka server provided values
-        """
-        return pulumi.get(self, "kafka")
-
-    @kafka.setter
-    def kafka(self, value: Optional[pulumi.Input['KafkaKafkaArgs']]):
-        pulumi.set(self, "kafka", value)
-
-    @property
     @pulumi.getter(name="kafkaUserConfig")
     def kafka_user_config(self) -> Optional[pulumi.Input['KafkaKafkaUserConfigArgs']]:
         """
         Kafka user configurable settings
         """
         return pulumi.get(self, "kafka_user_config")
 
@@ -299,16 +289,16 @@
                  components: Optional[pulumi.Input[Sequence[pulumi.Input['KafkaComponentArgs']]]] = None,
                  default_acl: Optional[pulumi.Input[bool]] = None,
                  disk_space: Optional[pulumi.Input[str]] = None,
                  disk_space_cap: Optional[pulumi.Input[str]] = None,
                  disk_space_default: Optional[pulumi.Input[str]] = None,
                  disk_space_step: Optional[pulumi.Input[str]] = None,
                  disk_space_used: Optional[pulumi.Input[str]] = None,
-                 kafka: Optional[pulumi.Input['KafkaKafkaArgs']] = None,
                  kafka_user_config: Optional[pulumi.Input['KafkaKafkaUserConfigArgs']] = None,
+                 kafkas: Optional[pulumi.Input[Sequence[pulumi.Input['KafkaKafkaArgs']]]] = None,
                  karapace: Optional[pulumi.Input[bool]] = None,
                  maintenance_window_dow: Optional[pulumi.Input[str]] = None,
                  maintenance_window_time: Optional[pulumi.Input[str]] = None,
                  plan: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None,
                  project_vpc_id: Optional[pulumi.Input[str]] = None,
                  service_host: Optional[pulumi.Input[str]] = None,
@@ -330,16 +320,16 @@
         :param pulumi.Input[Sequence[pulumi.Input['KafkaComponentArgs']]] components: Service component information objects
         :param pulumi.Input[bool] default_acl: Create default wildcard Kafka ACL
         :param pulumi.Input[str] disk_space: Service disk space. Possible values depend on the service type, the cloud provider and the project. Therefore, reducing will result in the service rebalancing.
         :param pulumi.Input[str] disk_space_cap: The maximum disk space of the service, possible values depend on the service type, the cloud provider and the project.
         :param pulumi.Input[str] disk_space_default: The default disk space of the service, possible values depend on the service type, the cloud provider and the project. Its also the minimum value for `disk_space`
         :param pulumi.Input[str] disk_space_step: The default disk space step of the service, possible values depend on the service type, the cloud provider and the project. `disk_space` needs to increment from `disk_space_default` by increments of this size.
         :param pulumi.Input[str] disk_space_used: Disk space that service is currently using
-        :param pulumi.Input['KafkaKafkaArgs'] kafka: Kafka server provided values
         :param pulumi.Input['KafkaKafkaUserConfigArgs'] kafka_user_config: Kafka user configurable settings
+        :param pulumi.Input[Sequence[pulumi.Input['KafkaKafkaArgs']]] kafkas: Kafka server provided values
         :param pulumi.Input[bool] karapace: Switch the service to use Karapace for schema registry and REST proxy
         :param pulumi.Input[str] maintenance_window_dow: Day of week when maintenance operations should be performed. One monday, tuesday, wednesday, etc.
         :param pulumi.Input[str] maintenance_window_time: Time of day when maintenance operations should be performed. UTC time in HH:mm:ss format.
         :param pulumi.Input[str] plan: Defines what kind of computing resources are allocated for the service. It can be changed after creation, though there are some restrictions when going to a smaller plan such as the new plan must have sufficient amount of disk space to store all current data and switching to a plan with fewer nodes might not be supported. The basic plan names are `hobbyist`, `startup-x`, `business-x` and `premium-x` where `x` is (roughly) the amount of memory on each node (also other attributes like number of CPUs and amount of disk space varies but naming is based on memory). The available options can be seem from the [Aiven pricing page](https://aiven.io/pricing).
         :param pulumi.Input[str] project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] project_vpc_id: Specifies the VPC the service should run in. If the value is not set the service is not run inside a VPC. When set, the value should be given as a reference to set up dependencies correctly and the VPC must be in the same cloud and region as the service itself. Project can be freely moved to and from VPC after creation but doing so triggers migration to new servers so the operation can take significant amount of time to complete if the service has a lot of data.
         :param pulumi.Input[str] service_host: The hostname of the service.
@@ -360,27 +350,33 @@
         if cloud_name is not None:
             pulumi.set(__self__, "cloud_name", cloud_name)
         if components is not None:
             pulumi.set(__self__, "components", components)
         if default_acl is not None:
             pulumi.set(__self__, "default_acl", default_acl)
         if disk_space is not None:
+            warnings.warn("""This will be removed in v5.0.0 and replaced with additional_disk_space instead.""", DeprecationWarning)
+            pulumi.log.warn("""disk_space is deprecated: This will be removed in v5.0.0 and replaced with additional_disk_space instead.""")
+        if disk_space is not None:
             pulumi.set(__self__, "disk_space", disk_space)
         if disk_space_cap is not None:
             pulumi.set(__self__, "disk_space_cap", disk_space_cap)
         if disk_space_default is not None:
             pulumi.set(__self__, "disk_space_default", disk_space_default)
         if disk_space_step is not None:
             pulumi.set(__self__, "disk_space_step", disk_space_step)
         if disk_space_used is not None:
             pulumi.set(__self__, "disk_space_used", disk_space_used)
-        if kafka is not None:
-            pulumi.set(__self__, "kafka", kafka)
         if kafka_user_config is not None:
             pulumi.set(__self__, "kafka_user_config", kafka_user_config)
+        if kafkas is not None:
+            pulumi.set(__self__, "kafkas", kafkas)
+        if karapace is not None:
+            warnings.warn("""Usage of this field is discouraged.""", DeprecationWarning)
+            pulumi.log.warn("""karapace is deprecated: Usage of this field is discouraged.""")
         if karapace is not None:
             pulumi.set(__self__, "karapace", karapace)
         if maintenance_window_dow is not None:
             pulumi.set(__self__, "maintenance_window_dow", maintenance_window_dow)
         if maintenance_window_time is not None:
             pulumi.set(__self__, "maintenance_window_time", maintenance_window_time)
         if plan is not None:
@@ -519,39 +515,39 @@
         return pulumi.get(self, "disk_space_used")
 
     @disk_space_used.setter
     def disk_space_used(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "disk_space_used", value)
 
     @property
-    @pulumi.getter
-    def kafka(self) -> Optional[pulumi.Input['KafkaKafkaArgs']]:
-        """
-        Kafka server provided values
-        """
-        return pulumi.get(self, "kafka")
-
-    @kafka.setter
-    def kafka(self, value: Optional[pulumi.Input['KafkaKafkaArgs']]):
-        pulumi.set(self, "kafka", value)
-
-    @property
     @pulumi.getter(name="kafkaUserConfig")
     def kafka_user_config(self) -> Optional[pulumi.Input['KafkaKafkaUserConfigArgs']]:
         """
         Kafka user configurable settings
         """
         return pulumi.get(self, "kafka_user_config")
 
     @kafka_user_config.setter
     def kafka_user_config(self, value: Optional[pulumi.Input['KafkaKafkaUserConfigArgs']]):
         pulumi.set(self, "kafka_user_config", value)
 
     @property
     @pulumi.getter
+    def kafkas(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['KafkaKafkaArgs']]]]:
+        """
+        Kafka server provided values
+        """
+        return pulumi.get(self, "kafkas")
+
+    @kafkas.setter
+    def kafkas(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['KafkaKafkaArgs']]]]):
+        pulumi.set(self, "kafkas", value)
+
+    @property
+    @pulumi.getter
     def karapace(self) -> Optional[pulumi.Input[bool]]:
         """
         Switch the service to use Karapace for schema registry and REST proxy
         """
         return pulumi.get(self, "karapace")
 
     @karapace.setter
@@ -768,15 +764,14 @@
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  additional_disk_space: Optional[pulumi.Input[str]] = None,
                  cloud_name: Optional[pulumi.Input[str]] = None,
                  default_acl: Optional[pulumi.Input[bool]] = None,
                  disk_space: Optional[pulumi.Input[str]] = None,
-                 kafka: Optional[pulumi.Input[pulumi.InputType['KafkaKafkaArgs']]] = None,
                  kafka_user_config: Optional[pulumi.Input[pulumi.InputType['KafkaKafkaUserConfigArgs']]] = None,
                  karapace: Optional[pulumi.Input[bool]] = None,
                  maintenance_window_dow: Optional[pulumi.Input[str]] = None,
                  maintenance_window_time: Optional[pulumi.Input[str]] = None,
                  plan: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None,
                  project_vpc_id: Optional[pulumi.Input[str]] = None,
@@ -826,15 +821,14 @@
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] additional_disk_space: Additional disk space. Possible values depend on the service type, the cloud provider and the project. Therefore, reducing will result in the service rebalancing.
         :param pulumi.Input[str] cloud_name: Defines where the cloud provider and region where the service is hosted in. This can be changed freely after service is created. Changing the value will trigger a potentially lengthy migration process for the service. Format is cloud provider name (`aws`, `azure`, `do` `google`, `upcloud`, etc.), dash, and the cloud provider specific region name. These are documented on each Cloud provider's own support articles, like [here for Google](https://cloud.google.com/compute/docs/regions-zones/) and [here for AWS](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Concepts.RegionsAndAvailabilityZones.html).
         :param pulumi.Input[bool] default_acl: Create default wildcard Kafka ACL
         :param pulumi.Input[str] disk_space: Service disk space. Possible values depend on the service type, the cloud provider and the project. Therefore, reducing will result in the service rebalancing.
-        :param pulumi.Input[pulumi.InputType['KafkaKafkaArgs']] kafka: Kafka server provided values
         :param pulumi.Input[pulumi.InputType['KafkaKafkaUserConfigArgs']] kafka_user_config: Kafka user configurable settings
         :param pulumi.Input[bool] karapace: Switch the service to use Karapace for schema registry and REST proxy
         :param pulumi.Input[str] maintenance_window_dow: Day of week when maintenance operations should be performed. One monday, tuesday, wednesday, etc.
         :param pulumi.Input[str] maintenance_window_time: Time of day when maintenance operations should be performed. UTC time in HH:mm:ss format.
         :param pulumi.Input[str] plan: Defines what kind of computing resources are allocated for the service. It can be changed after creation, though there are some restrictions when going to a smaller plan such as the new plan must have sufficient amount of disk space to store all current data and switching to a plan with fewer nodes might not be supported. The basic plan names are `hobbyist`, `startup-x`, `business-x` and `premium-x` where `x` is (roughly) the amount of memory on each node (also other attributes like number of CPUs and amount of disk space varies but naming is based on memory). The available options can be seem from the [Aiven pricing page](https://aiven.io/pricing).
         :param pulumi.Input[str] project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] project_vpc_id: Specifies the VPC the service should run in. If the value is not set the service is not run inside a VPC. When set, the value should be given as a reference to set up dependencies correctly and the VPC must be in the same cloud and region as the service itself. Project can be freely moved to and from VPC after creation but doing so triggers migration to new servers so the operation can take significant amount of time to complete if the service has a lot of data.
@@ -903,15 +897,14 @@
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  additional_disk_space: Optional[pulumi.Input[str]] = None,
                  cloud_name: Optional[pulumi.Input[str]] = None,
                  default_acl: Optional[pulumi.Input[bool]] = None,
                  disk_space: Optional[pulumi.Input[str]] = None,
-                 kafka: Optional[pulumi.Input[pulumi.InputType['KafkaKafkaArgs']]] = None,
                  kafka_user_config: Optional[pulumi.Input[pulumi.InputType['KafkaKafkaUserConfigArgs']]] = None,
                  karapace: Optional[pulumi.Input[bool]] = None,
                  maintenance_window_dow: Optional[pulumi.Input[str]] = None,
                  maintenance_window_time: Optional[pulumi.Input[str]] = None,
                  plan: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None,
                  project_vpc_id: Optional[pulumi.Input[str]] = None,
@@ -928,17 +921,22 @@
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = KafkaArgs.__new__(KafkaArgs)
 
             __props__.__dict__["additional_disk_space"] = additional_disk_space
             __props__.__dict__["cloud_name"] = cloud_name
             __props__.__dict__["default_acl"] = default_acl
+            if disk_space is not None and not opts.urn:
+                warnings.warn("""This will be removed in v5.0.0 and replaced with additional_disk_space instead.""", DeprecationWarning)
+                pulumi.log.warn("""disk_space is deprecated: This will be removed in v5.0.0 and replaced with additional_disk_space instead.""")
             __props__.__dict__["disk_space"] = disk_space
-            __props__.__dict__["kafka"] = kafka
             __props__.__dict__["kafka_user_config"] = kafka_user_config
+            if karapace is not None and not opts.urn:
+                warnings.warn("""Usage of this field is discouraged.""", DeprecationWarning)
+                pulumi.log.warn("""karapace is deprecated: Usage of this field is discouraged.""")
             __props__.__dict__["karapace"] = karapace
             __props__.__dict__["maintenance_window_dow"] = maintenance_window_dow
             __props__.__dict__["maintenance_window_time"] = maintenance_window_time
             __props__.__dict__["plan"] = plan
             if project is None and not opts.urn:
                 raise TypeError("Missing required property 'project'")
             __props__.__dict__["project"] = project
@@ -951,14 +949,15 @@
             __props__.__dict__["tags"] = tags
             __props__.__dict__["termination_protection"] = termination_protection
             __props__.__dict__["components"] = None
             __props__.__dict__["disk_space_cap"] = None
             __props__.__dict__["disk_space_default"] = None
             __props__.__dict__["disk_space_step"] = None
             __props__.__dict__["disk_space_used"] = None
+            __props__.__dict__["kafkas"] = None
             __props__.__dict__["service_host"] = None
             __props__.__dict__["service_password"] = None
             __props__.__dict__["service_port"] = None
             __props__.__dict__["service_type"] = None
             __props__.__dict__["service_uri"] = None
             __props__.__dict__["service_username"] = None
             __props__.__dict__["state"] = None
@@ -979,16 +978,16 @@
             components: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['KafkaComponentArgs']]]]] = None,
             default_acl: Optional[pulumi.Input[bool]] = None,
             disk_space: Optional[pulumi.Input[str]] = None,
             disk_space_cap: Optional[pulumi.Input[str]] = None,
             disk_space_default: Optional[pulumi.Input[str]] = None,
             disk_space_step: Optional[pulumi.Input[str]] = None,
             disk_space_used: Optional[pulumi.Input[str]] = None,
-            kafka: Optional[pulumi.Input[pulumi.InputType['KafkaKafkaArgs']]] = None,
             kafka_user_config: Optional[pulumi.Input[pulumi.InputType['KafkaKafkaUserConfigArgs']]] = None,
+            kafkas: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['KafkaKafkaArgs']]]]] = None,
             karapace: Optional[pulumi.Input[bool]] = None,
             maintenance_window_dow: Optional[pulumi.Input[str]] = None,
             maintenance_window_time: Optional[pulumi.Input[str]] = None,
             plan: Optional[pulumi.Input[str]] = None,
             project: Optional[pulumi.Input[str]] = None,
             project_vpc_id: Optional[pulumi.Input[str]] = None,
             service_host: Optional[pulumi.Input[str]] = None,
@@ -1015,16 +1014,16 @@
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['KafkaComponentArgs']]]] components: Service component information objects
         :param pulumi.Input[bool] default_acl: Create default wildcard Kafka ACL
         :param pulumi.Input[str] disk_space: Service disk space. Possible values depend on the service type, the cloud provider and the project. Therefore, reducing will result in the service rebalancing.
         :param pulumi.Input[str] disk_space_cap: The maximum disk space of the service, possible values depend on the service type, the cloud provider and the project.
         :param pulumi.Input[str] disk_space_default: The default disk space of the service, possible values depend on the service type, the cloud provider and the project. Its also the minimum value for `disk_space`
         :param pulumi.Input[str] disk_space_step: The default disk space step of the service, possible values depend on the service type, the cloud provider and the project. `disk_space` needs to increment from `disk_space_default` by increments of this size.
         :param pulumi.Input[str] disk_space_used: Disk space that service is currently using
-        :param pulumi.Input[pulumi.InputType['KafkaKafkaArgs']] kafka: Kafka server provided values
         :param pulumi.Input[pulumi.InputType['KafkaKafkaUserConfigArgs']] kafka_user_config: Kafka user configurable settings
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['KafkaKafkaArgs']]]] kafkas: Kafka server provided values
         :param pulumi.Input[bool] karapace: Switch the service to use Karapace for schema registry and REST proxy
         :param pulumi.Input[str] maintenance_window_dow: Day of week when maintenance operations should be performed. One monday, tuesday, wednesday, etc.
         :param pulumi.Input[str] maintenance_window_time: Time of day when maintenance operations should be performed. UTC time in HH:mm:ss format.
         :param pulumi.Input[str] plan: Defines what kind of computing resources are allocated for the service. It can be changed after creation, though there are some restrictions when going to a smaller plan such as the new plan must have sufficient amount of disk space to store all current data and switching to a plan with fewer nodes might not be supported. The basic plan names are `hobbyist`, `startup-x`, `business-x` and `premium-x` where `x` is (roughly) the amount of memory on each node (also other attributes like number of CPUs and amount of disk space varies but naming is based on memory). The available options can be seem from the [Aiven pricing page](https://aiven.io/pricing).
         :param pulumi.Input[str] project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] project_vpc_id: Specifies the VPC the service should run in. If the value is not set the service is not run inside a VPC. When set, the value should be given as a reference to set up dependencies correctly and the VPC must be in the same cloud and region as the service itself. Project can be freely moved to and from VPC after creation but doing so triggers migration to new servers so the operation can take significant amount of time to complete if the service has a lot of data.
         :param pulumi.Input[str] service_host: The hostname of the service.
@@ -1049,16 +1048,16 @@
         __props__.__dict__["components"] = components
         __props__.__dict__["default_acl"] = default_acl
         __props__.__dict__["disk_space"] = disk_space
         __props__.__dict__["disk_space_cap"] = disk_space_cap
         __props__.__dict__["disk_space_default"] = disk_space_default
         __props__.__dict__["disk_space_step"] = disk_space_step
         __props__.__dict__["disk_space_used"] = disk_space_used
-        __props__.__dict__["kafka"] = kafka
         __props__.__dict__["kafka_user_config"] = kafka_user_config
+        __props__.__dict__["kafkas"] = kafkas
         __props__.__dict__["karapace"] = karapace
         __props__.__dict__["maintenance_window_dow"] = maintenance_window_dow
         __props__.__dict__["maintenance_window_time"] = maintenance_window_time
         __props__.__dict__["plan"] = plan
         __props__.__dict__["project"] = project
         __props__.__dict__["project_vpc_id"] = project_vpc_id
         __props__.__dict__["service_host"] = service_host
@@ -1144,31 +1143,31 @@
     def disk_space_used(self) -> pulumi.Output[str]:
         """
         Disk space that service is currently using
         """
         return pulumi.get(self, "disk_space_used")
 
     @property
-    @pulumi.getter
-    def kafka(self) -> pulumi.Output['outputs.KafkaKafka']:
-        """
-        Kafka server provided values
-        """
-        return pulumi.get(self, "kafka")
-
-    @property
     @pulumi.getter(name="kafkaUserConfig")
     def kafka_user_config(self) -> pulumi.Output[Optional['outputs.KafkaKafkaUserConfig']]:
         """
         Kafka user configurable settings
         """
         return pulumi.get(self, "kafka_user_config")
 
     @property
     @pulumi.getter
+    def kafkas(self) -> pulumi.Output[Sequence['outputs.KafkaKafka']]:
+        """
+        Kafka server provided values
+        """
+        return pulumi.get(self, "kafkas")
+
+    @property
+    @pulumi.getter
     def karapace(self) -> pulumi.Output[Optional[bool]]:
         """
         Switch the service to use Karapace for schema registry and REST proxy
         """
         return pulumi.get(self, "karapace")
 
     @property
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/kafka_acl.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/kafka_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/kafka_connect.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/kafka_connect.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,17 @@
         pulumi.set(__self__, "project", project)
         pulumi.set(__self__, "service_name", service_name)
         if additional_disk_space is not None:
             pulumi.set(__self__, "additional_disk_space", additional_disk_space)
         if cloud_name is not None:
             pulumi.set(__self__, "cloud_name", cloud_name)
         if disk_space is not None:
+            warnings.warn("""This will be removed in v5.0.0 and replaced with additional_disk_space instead.""", DeprecationWarning)
+            pulumi.log.warn("""disk_space is deprecated: This will be removed in v5.0.0 and replaced with additional_disk_space instead.""")
+        if disk_space is not None:
             pulumi.set(__self__, "disk_space", disk_space)
         if kafka_connect_user_config is not None:
             pulumi.set(__self__, "kafka_connect_user_config", kafka_connect_user_config)
         if maintenance_window_dow is not None:
             pulumi.set(__self__, "maintenance_window_dow", maintenance_window_dow)
         if maintenance_window_time is not None:
             pulumi.set(__self__, "maintenance_window_time", maintenance_window_time)
@@ -368,14 +371,17 @@
         if additional_disk_space is not None:
             pulumi.set(__self__, "additional_disk_space", additional_disk_space)
         if cloud_name is not None:
             pulumi.set(__self__, "cloud_name", cloud_name)
         if components is not None:
             pulumi.set(__self__, "components", components)
         if disk_space is not None:
+            warnings.warn("""This will be removed in v5.0.0 and replaced with additional_disk_space instead.""", DeprecationWarning)
+            pulumi.log.warn("""disk_space is deprecated: This will be removed in v5.0.0 and replaced with additional_disk_space instead.""")
+        if disk_space is not None:
             pulumi.set(__self__, "disk_space", disk_space)
         if disk_space_cap is not None:
             pulumi.set(__self__, "disk_space_cap", disk_space_cap)
         if disk_space_default is not None:
             pulumi.set(__self__, "disk_space_default", disk_space_default)
         if disk_space_step is not None:
             pulumi.set(__self__, "disk_space_step", disk_space_step)
@@ -930,14 +936,17 @@
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = KafkaConnectArgs.__new__(KafkaConnectArgs)
 
             __props__.__dict__["additional_disk_space"] = additional_disk_space
             __props__.__dict__["cloud_name"] = cloud_name
+            if disk_space is not None and not opts.urn:
+                warnings.warn("""This will be removed in v5.0.0 and replaced with additional_disk_space instead.""", DeprecationWarning)
+                pulumi.log.warn("""disk_space is deprecated: This will be removed in v5.0.0 and replaced with additional_disk_space instead.""")
             __props__.__dict__["disk_space"] = disk_space
             __props__.__dict__["kafka_connect_user_config"] = kafka_connect_user_config
             __props__.__dict__["maintenance_window_dow"] = maintenance_window_dow
             __props__.__dict__["maintenance_window_time"] = maintenance_window_time
             __props__.__dict__["plan"] = plan
             if project is None and not opts.urn:
                 raise TypeError("Missing required property 'project'")
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/kafka_connector.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/kafka_connector.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/kafka_mirror_maker.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/kafka_mirror_maker.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,17 @@
         pulumi.set(__self__, "project", project)
         pulumi.set(__self__, "service_name", service_name)
         if additional_disk_space is not None:
             pulumi.set(__self__, "additional_disk_space", additional_disk_space)
         if cloud_name is not None:
             pulumi.set(__self__, "cloud_name", cloud_name)
         if disk_space is not None:
+            warnings.warn("""This will be removed in v5.0.0 and replaced with additional_disk_space instead.""", DeprecationWarning)
+            pulumi.log.warn("""disk_space is deprecated: This will be removed in v5.0.0 and replaced with additional_disk_space instead.""")
+        if disk_space is not None:
             pulumi.set(__self__, "disk_space", disk_space)
         if kafka_mirrormaker_user_config is not None:
             pulumi.set(__self__, "kafka_mirrormaker_user_config", kafka_mirrormaker_user_config)
         if maintenance_window_dow is not None:
             pulumi.set(__self__, "maintenance_window_dow", maintenance_window_dow)
         if maintenance_window_time is not None:
             pulumi.set(__self__, "maintenance_window_time", maintenance_window_time)
@@ -368,14 +371,17 @@
         if additional_disk_space is not None:
             pulumi.set(__self__, "additional_disk_space", additional_disk_space)
         if cloud_name is not None:
             pulumi.set(__self__, "cloud_name", cloud_name)
         if components is not None:
             pulumi.set(__self__, "components", components)
         if disk_space is not None:
+            warnings.warn("""This will be removed in v5.0.0 and replaced with additional_disk_space instead.""", DeprecationWarning)
+            pulumi.log.warn("""disk_space is deprecated: This will be removed in v5.0.0 and replaced with additional_disk_space instead.""")
+        if disk_space is not None:
             pulumi.set(__self__, "disk_space", disk_space)
         if disk_space_cap is not None:
             pulumi.set(__self__, "disk_space_cap", disk_space_cap)
         if disk_space_default is not None:
             pulumi.set(__self__, "disk_space_default", disk_space_default)
         if disk_space_step is not None:
             pulumi.set(__self__, "disk_space_step", disk_space_step)
@@ -926,14 +932,17 @@
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = KafkaMirrorMakerArgs.__new__(KafkaMirrorMakerArgs)
 
             __props__.__dict__["additional_disk_space"] = additional_disk_space
             __props__.__dict__["cloud_name"] = cloud_name
+            if disk_space is not None and not opts.urn:
+                warnings.warn("""This will be removed in v5.0.0 and replaced with additional_disk_space instead.""", DeprecationWarning)
+                pulumi.log.warn("""disk_space is deprecated: This will be removed in v5.0.0 and replaced with additional_disk_space instead.""")
             __props__.__dict__["disk_space"] = disk_space
             __props__.__dict__["kafka_mirrormaker_user_config"] = kafka_mirrormaker_user_config
             __props__.__dict__["maintenance_window_dow"] = maintenance_window_dow
             __props__.__dict__["maintenance_window_time"] = maintenance_window_time
             __props__.__dict__["plan"] = plan
             if project is None and not opts.urn:
                 raise TypeError("Missing required property 'project'")
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/kafka_schema.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/kafka_schema.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/kafka_schema_configuration.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/kafka_schema_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/kafka_schema_registry_acl.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/kafka_schema_registry_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/kafka_topic.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/kafka_topic.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/kafka_user.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/kafka_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,14 +222,20 @@
         foo = aiven.KafkaUser("foo",
             service_name=aiven_kafka["bar"]["service_name"],
             project="my-project",
             username="user-1",
             password="Test$1234")
         ```
 
+        ## Import
+
+        ```sh
+         $ pulumi import aiven:index/kafkaUser:KafkaUser foo project/service_name/username
+        ```
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] password: The password of the Kafka User.
         :param pulumi.Input[str] project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] username: The actual name of the Kafka User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
@@ -251,14 +257,20 @@
         foo = aiven.KafkaUser("foo",
             service_name=aiven_kafka["bar"]["service_name"],
             project="my-project",
             username="user-1",
             password="Test$1234")
         ```
 
+        ## Import
+
+        ```sh
+         $ pulumi import aiven:index/kafkaUser:KafkaUser foo project/service_name/username
+        ```
+
         :param str resource_name: The name of the resource.
         :param KafkaUserArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(KafkaUserArgs, pulumi.ResourceOptions, *args, **kwargs)
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/m3_aggregator.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/m3_aggregator.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,17 @@
         pulumi.set(__self__, "project", project)
         pulumi.set(__self__, "service_name", service_name)
         if additional_disk_space is not None:
             pulumi.set(__self__, "additional_disk_space", additional_disk_space)
         if cloud_name is not None:
             pulumi.set(__self__, "cloud_name", cloud_name)
         if disk_space is not None:
+            warnings.warn("""This will be removed in v5.0.0 and replaced with additional_disk_space instead.""", DeprecationWarning)
+            pulumi.log.warn("""disk_space is deprecated: This will be removed in v5.0.0 and replaced with additional_disk_space instead.""")
+        if disk_space is not None:
             pulumi.set(__self__, "disk_space", disk_space)
         if m3aggregator_user_config is not None:
             pulumi.set(__self__, "m3aggregator_user_config", m3aggregator_user_config)
         if maintenance_window_dow is not None:
             pulumi.set(__self__, "maintenance_window_dow", maintenance_window_dow)
         if maintenance_window_time is not None:
             pulumi.set(__self__, "maintenance_window_time", maintenance_window_time)
@@ -368,14 +371,17 @@
         if additional_disk_space is not None:
             pulumi.set(__self__, "additional_disk_space", additional_disk_space)
         if cloud_name is not None:
             pulumi.set(__self__, "cloud_name", cloud_name)
         if components is not None:
             pulumi.set(__self__, "components", components)
         if disk_space is not None:
+            warnings.warn("""This will be removed in v5.0.0 and replaced with additional_disk_space instead.""", DeprecationWarning)
+            pulumi.log.warn("""disk_space is deprecated: This will be removed in v5.0.0 and replaced with additional_disk_space instead.""")
+        if disk_space is not None:
             pulumi.set(__self__, "disk_space", disk_space)
         if disk_space_cap is not None:
             pulumi.set(__self__, "disk_space_cap", disk_space_cap)
         if disk_space_default is not None:
             pulumi.set(__self__, "disk_space_default", disk_space_default)
         if disk_space_step is not None:
             pulumi.set(__self__, "disk_space_step", disk_space_step)
@@ -920,14 +926,17 @@
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = M3AggregatorArgs.__new__(M3AggregatorArgs)
 
             __props__.__dict__["additional_disk_space"] = additional_disk_space
             __props__.__dict__["cloud_name"] = cloud_name
+            if disk_space is not None and not opts.urn:
+                warnings.warn("""This will be removed in v5.0.0 and replaced with additional_disk_space instead.""", DeprecationWarning)
+                pulumi.log.warn("""disk_space is deprecated: This will be removed in v5.0.0 and replaced with additional_disk_space instead.""")
             __props__.__dict__["disk_space"] = disk_space
             __props__.__dict__["m3aggregator_user_config"] = m3aggregator_user_config
             __props__.__dict__["maintenance_window_dow"] = maintenance_window_dow
             __props__.__dict__["maintenance_window_time"] = maintenance_window_time
             __props__.__dict__["plan"] = plan
             if project is None and not opts.urn:
                 raise TypeError("Missing required property 'project'")
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/m3_db.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/m3_db.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,14 +70,17 @@
         pulumi.set(__self__, "project", project)
         pulumi.set(__self__, "service_name", service_name)
         if additional_disk_space is not None:
             pulumi.set(__self__, "additional_disk_space", additional_disk_space)
         if cloud_name is not None:
             pulumi.set(__self__, "cloud_name", cloud_name)
         if disk_space is not None:
+            warnings.warn("""This will be removed in v5.0.0 and replaced with additional_disk_space instead.""", DeprecationWarning)
+            pulumi.log.warn("""disk_space is deprecated: This will be removed in v5.0.0 and replaced with additional_disk_space instead.""")
+        if disk_space is not None:
             pulumi.set(__self__, "disk_space", disk_space)
         if m3db_user_config is not None:
             pulumi.set(__self__, "m3db_user_config", m3db_user_config)
         if maintenance_window_dow is not None:
             pulumi.set(__self__, "maintenance_window_dow", maintenance_window_dow)
         if maintenance_window_time is not None:
             pulumi.set(__self__, "maintenance_window_time", maintenance_window_time)
@@ -368,14 +371,17 @@
         if additional_disk_space is not None:
             pulumi.set(__self__, "additional_disk_space", additional_disk_space)
         if cloud_name is not None:
             pulumi.set(__self__, "cloud_name", cloud_name)
         if components is not None:
             pulumi.set(__self__, "components", components)
         if disk_space is not None:
+            warnings.warn("""This will be removed in v5.0.0 and replaced with additional_disk_space instead.""", DeprecationWarning)
+            pulumi.log.warn("""disk_space is deprecated: This will be removed in v5.0.0 and replaced with additional_disk_space instead.""")
+        if disk_space is not None:
             pulumi.set(__self__, "disk_space", disk_space)
         if disk_space_cap is not None:
             pulumi.set(__self__, "disk_space_cap", disk_space_cap)
         if disk_space_default is not None:
             pulumi.set(__self__, "disk_space_default", disk_space_default)
         if disk_space_step is not None:
             pulumi.set(__self__, "disk_space_step", disk_space_step)
@@ -928,14 +934,17 @@
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = M3DbArgs.__new__(M3DbArgs)
 
             __props__.__dict__["additional_disk_space"] = additional_disk_space
             __props__.__dict__["cloud_name"] = cloud_name
+            if disk_space is not None and not opts.urn:
+                warnings.warn("""This will be removed in v5.0.0 and replaced with additional_disk_space instead.""", DeprecationWarning)
+                pulumi.log.warn("""disk_space is deprecated: This will be removed in v5.0.0 and replaced with additional_disk_space instead.""")
             __props__.__dict__["disk_space"] = disk_space
             __props__.__dict__["m3db_user_config"] = m3db_user_config
             __props__.__dict__["maintenance_window_dow"] = maintenance_window_dow
             __props__.__dict__["maintenance_window_time"] = maintenance_window_time
             __props__.__dict__["plan"] = plan
             if project is None and not opts.urn:
                 raise TypeError("Missing required property 'project'")
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/m3db_user.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/m3db_user.py`

 * *Files 3% similar despite different names*

```diff
@@ -190,14 +190,20 @@
         foo = aiven.M3dbUser("foo",
             service_name=aiven_m3db["bar"]["service_name"],
             project="my-project",
             username="user-1",
             password="Test$1234")
         ```
 
+        ## Import
+
+        ```sh
+         $ pulumi import aiven:index/m3dbUser:M3dbUser foo project/service_name/username
+        ```
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] password: The password of the M3DB User.
         :param pulumi.Input[str] project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] username: The actual name of the M3DB User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
@@ -219,14 +225,20 @@
         foo = aiven.M3dbUser("foo",
             service_name=aiven_m3db["bar"]["service_name"],
             project="my-project",
             username="user-1",
             password="Test$1234")
         ```
 
+        ## Import
+
+        ```sh
+         $ pulumi import aiven:index/m3dbUser:M3dbUser foo project/service_name/username
+        ```
+
         :param str resource_name: The name of the resource.
         :param M3dbUserArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(M3dbUserArgs, pulumi.ResourceOptions, *args, **kwargs)
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/mirror_maker_replication_flow.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/mirror_maker_replication_flow.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/my_sql.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/my_sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,17 @@
         pulumi.set(__self__, "project", project)
         pulumi.set(__self__, "service_name", service_name)
         if additional_disk_space is not None:
             pulumi.set(__self__, "additional_disk_space", additional_disk_space)
         if cloud_name is not None:
             pulumi.set(__self__, "cloud_name", cloud_name)
         if disk_space is not None:
+            warnings.warn("""This will be removed in v5.0.0 and replaced with additional_disk_space instead.""", DeprecationWarning)
+            pulumi.log.warn("""disk_space is deprecated: This will be removed in v5.0.0 and replaced with additional_disk_space instead.""")
+        if disk_space is not None:
             pulumi.set(__self__, "disk_space", disk_space)
         if maintenance_window_dow is not None:
             pulumi.set(__self__, "maintenance_window_dow", maintenance_window_dow)
         if maintenance_window_time is not None:
             pulumi.set(__self__, "maintenance_window_time", maintenance_window_time)
         if mysql_user_config is not None:
             pulumi.set(__self__, "mysql_user_config", mysql_user_config)
@@ -368,14 +371,17 @@
         if additional_disk_space is not None:
             pulumi.set(__self__, "additional_disk_space", additional_disk_space)
         if cloud_name is not None:
             pulumi.set(__self__, "cloud_name", cloud_name)
         if components is not None:
             pulumi.set(__self__, "components", components)
         if disk_space is not None:
+            warnings.warn("""This will be removed in v5.0.0 and replaced with additional_disk_space instead.""", DeprecationWarning)
+            pulumi.log.warn("""disk_space is deprecated: This will be removed in v5.0.0 and replaced with additional_disk_space instead.""")
+        if disk_space is not None:
             pulumi.set(__self__, "disk_space", disk_space)
         if disk_space_cap is not None:
             pulumi.set(__self__, "disk_space_cap", disk_space_cap)
         if disk_space_default is not None:
             pulumi.set(__self__, "disk_space_default", disk_space_default)
         if disk_space_step is not None:
             pulumi.set(__self__, "disk_space_step", disk_space_step)
@@ -934,14 +940,17 @@
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = MySqlArgs.__new__(MySqlArgs)
 
             __props__.__dict__["additional_disk_space"] = additional_disk_space
             __props__.__dict__["cloud_name"] = cloud_name
+            if disk_space is not None and not opts.urn:
+                warnings.warn("""This will be removed in v5.0.0 and replaced with additional_disk_space instead.""", DeprecationWarning)
+                pulumi.log.warn("""disk_space is deprecated: This will be removed in v5.0.0 and replaced with additional_disk_space instead.""")
             __props__.__dict__["disk_space"] = disk_space
             __props__.__dict__["maintenance_window_dow"] = maintenance_window_dow
             __props__.__dict__["maintenance_window_time"] = maintenance_window_time
             __props__.__dict__["mysql_user_config"] = mysql_user_config
             __props__.__dict__["plan"] = plan
             if project is None and not opts.urn:
                 raise TypeError("Missing required property 'project'")
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/mysql_database.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/mysql_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/mysql_user.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/mysql_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -255,14 +255,20 @@
         foo = aiven.MysqlUser("foo",
             service_name=aiven_mysql["bar"]["service_name"],
             project="my-project",
             username="user-1",
             password="Test$1234")
         ```
 
+        ## Import
+
+        ```sh
+         $ pulumi import aiven:index/mysqlUser:MysqlUser foo project/service_name/username
+        ```
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] authentication: Authentication details. The possible values are `caching_sha2_password` and `mysql_native_password`.
         :param pulumi.Input[str] password: The password of the MySQL User ( not applicable for all services ).
         :param pulumi.Input[str] project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] username: The actual name of the MySQL User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
@@ -285,14 +291,20 @@
         foo = aiven.MysqlUser("foo",
             service_name=aiven_mysql["bar"]["service_name"],
             project="my-project",
             username="user-1",
             password="Test$1234")
         ```
 
+        ## Import
+
+        ```sh
+         $ pulumi import aiven:index/mysqlUser:MysqlUser foo project/service_name/username
+        ```
+
         :param str resource_name: The name of the resource.
         :param MysqlUserArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(MysqlUserArgs, pulumi.ResourceOptions, *args, **kwargs)
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/open_search.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/open_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,14 +50,17 @@
         pulumi.set(__self__, "project", project)
         pulumi.set(__self__, "service_name", service_name)
         if additional_disk_space is not None:
             pulumi.set(__self__, "additional_disk_space", additional_disk_space)
         if cloud_name is not None:
             pulumi.set(__self__, "cloud_name", cloud_name)
         if disk_space is not None:
+            warnings.warn("""This will be removed in v5.0.0 and replaced with additional_disk_space instead.""", DeprecationWarning)
+            pulumi.log.warn("""disk_space is deprecated: This will be removed in v5.0.0 and replaced with additional_disk_space instead.""")
+        if disk_space is not None:
             pulumi.set(__self__, "disk_space", disk_space)
         if maintenance_window_dow is not None:
             pulumi.set(__self__, "maintenance_window_dow", maintenance_window_dow)
         if maintenance_window_time is not None:
             pulumi.set(__self__, "maintenance_window_time", maintenance_window_time)
         if opensearch_user_config is not None:
             pulumi.set(__self__, "opensearch_user_config", opensearch_user_config)
@@ -306,14 +309,17 @@
         if additional_disk_space is not None:
             pulumi.set(__self__, "additional_disk_space", additional_disk_space)
         if cloud_name is not None:
             pulumi.set(__self__, "cloud_name", cloud_name)
         if components is not None:
             pulumi.set(__self__, "components", components)
         if disk_space is not None:
+            warnings.warn("""This will be removed in v5.0.0 and replaced with additional_disk_space instead.""", DeprecationWarning)
+            pulumi.log.warn("""disk_space is deprecated: This will be removed in v5.0.0 and replaced with additional_disk_space instead.""")
+        if disk_space is not None:
             pulumi.set(__self__, "disk_space", disk_space)
         if disk_space_cap is not None:
             pulumi.set(__self__, "disk_space_cap", disk_space_cap)
         if disk_space_default is not None:
             pulumi.set(__self__, "disk_space_default", disk_space_default)
         if disk_space_step is not None:
             pulumi.set(__self__, "disk_space_step", disk_space_step)
@@ -832,14 +838,17 @@
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = OpenSearchArgs.__new__(OpenSearchArgs)
 
             __props__.__dict__["additional_disk_space"] = additional_disk_space
             __props__.__dict__["cloud_name"] = cloud_name
+            if disk_space is not None and not opts.urn:
+                warnings.warn("""This will be removed in v5.0.0 and replaced with additional_disk_space instead.""", DeprecationWarning)
+                pulumi.log.warn("""disk_space is deprecated: This will be removed in v5.0.0 and replaced with additional_disk_space instead.""")
             __props__.__dict__["disk_space"] = disk_space
             __props__.__dict__["maintenance_window_dow"] = maintenance_window_dow
             __props__.__dict__["maintenance_window_time"] = maintenance_window_time
             __props__.__dict__["opensearch_user_config"] = opensearch_user_config
             __props__.__dict__["plan"] = plan
             if project is None and not opts.urn:
                 raise TypeError("Missing required property 'project'")
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/open_search_acl_config.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/open_search_acl_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/open_search_acl_rule.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/open_search_acl_rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -239,21 +239,24 @@
             {
                 "username": os_user2.username,
                 "index": "index7",
                 "permission": "readwrite",
             },
         ]
         os_acl_rule = []
-        for range in [{"key": k, "value": v} for [k, v] in enumerate({i: v for i, v in acl_rules})]:
-            os_acl_rule.append(aiven.OpenSearchAclRule(f"osAclRule-{range['key']}",
-                project=os_acls_config.project,
-                service_name=os_acls_config.service_name,
-                username=range["value"]["username"],
-                index=range["value"]["index"],
-                permission=range["value"]["permission"]))
+        def create_os_acl_rule(range_body):
+            for range in [{"key": k, "value": v} for [k, v] in enumerate(range_body)]:
+                os_acl_rule.append(aiven.OpenSearchAclRule(f"osAclRule-{range['key']}",
+                    project=os_acls_config.project,
+                    service_name=os_acls_config.service_name,
+                    username=range["value"]["username"],
+                    index=range["value"]["index"],
+                    permission=range["value"]["permission"]))
+
+        pulumi.Output.all({i: v for i, v in acl_rules}).apply(lambda resolved_outputs: create_os_acl_rule(resolved_outputs[0]))
         ```
 
         ## Import
 
         ```sh
          $ pulumi import aiven:index/openSearchAclRule:OpenSearchAclRule os_acl_rule project/service_name/username/index
         ```
@@ -318,21 +321,24 @@
             {
                 "username": os_user2.username,
                 "index": "index7",
                 "permission": "readwrite",
             },
         ]
         os_acl_rule = []
-        for range in [{"key": k, "value": v} for [k, v] in enumerate({i: v for i, v in acl_rules})]:
-            os_acl_rule.append(aiven.OpenSearchAclRule(f"osAclRule-{range['key']}",
-                project=os_acls_config.project,
-                service_name=os_acls_config.service_name,
-                username=range["value"]["username"],
-                index=range["value"]["index"],
-                permission=range["value"]["permission"]))
+        def create_os_acl_rule(range_body):
+            for range in [{"key": k, "value": v} for [k, v] in enumerate(range_body)]:
+                os_acl_rule.append(aiven.OpenSearchAclRule(f"osAclRule-{range['key']}",
+                    project=os_acls_config.project,
+                    service_name=os_acls_config.service_name,
+                    username=range["value"]["username"],
+                    index=range["value"]["index"],
+                    permission=range["value"]["permission"]))
+
+        pulumi.Output.all({i: v for i, v in acl_rules}).apply(lambda resolved_outputs: create_os_acl_rule(resolved_outputs[0]))
         ```
 
         ## Import
 
         ```sh
          $ pulumi import aiven:index/openSearchAclRule:OpenSearchAclRule os_acl_rule project/service_name/username/index
         ```
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/opensearch_user.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/opensearch_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,14 +190,20 @@
         foo = aiven.OpensearchUser("foo",
             service_name=aiven_opensearch["bar"]["service_name"],
             project="my-project",
             username="user-1",
             password="Test$1234")
         ```
 
+        ## Import
+
+        ```sh
+         $ pulumi import aiven:index/opensearchUser:OpensearchUser foo project/service_name/username
+        ```
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] password: The password of the Opensearch User.
         :param pulumi.Input[str] project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] username: The actual name of the Opensearch User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
@@ -219,14 +225,20 @@
         foo = aiven.OpensearchUser("foo",
             service_name=aiven_opensearch["bar"]["service_name"],
             project="my-project",
             username="user-1",
             password="Test$1234")
         ```
 
+        ## Import
+
+        ```sh
+         $ pulumi import aiven:index/opensearchUser:OpensearchUser foo project/service_name/username
+        ```
+
         :param str resource_name: The name of the resource.
         :param OpensearchUserArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(OpensearchUserArgs, pulumi.ResourceOptions, *args, **kwargs)
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/outputs.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,14 +141,15 @@
     'OpenSearchOpensearchUserConfigIndexTemplate',
     'OpenSearchOpensearchUserConfigIpFilterObject',
     'OpenSearchOpensearchUserConfigOpensearch',
     'OpenSearchOpensearchUserConfigOpensearchDashboards',
     'OpenSearchOpensearchUserConfigPrivateAccess',
     'OpenSearchOpensearchUserConfigPrivatelinkAccess',
     'OpenSearchOpensearchUserConfigPublicAccess',
+    'OpenSearchOpensearchUserConfigSaml',
     'OpenSearchServiceIntegration',
     'OpenSearchTag',
     'PgComponent',
     'PgPg',
     'PgPgUserConfig',
     'PgPgUserConfigIpFilterObject',
     'PgPgUserConfigMigration',
@@ -189,15 +190,14 @@
     'ServiceIntegrationEndpointExternalGoogleCloudLoggingUserConfig',
     'ServiceIntegrationEndpointExternalKafkaUserConfig',
     'ServiceIntegrationEndpointExternalOpensearchLogsUserConfig',
     'ServiceIntegrationEndpointExternalSchemaRegistryUserConfig',
     'ServiceIntegrationEndpointJolokiaUserConfig',
     'ServiceIntegrationEndpointPrometheusUserConfig',
     'ServiceIntegrationEndpointRsyslogUserConfig',
-    'ServiceIntegrationEndpointSignalfxUserConfig',
     'ServiceIntegrationExternalAwsCloudwatchMetricsUserConfig',
     'ServiceIntegrationExternalAwsCloudwatchMetricsUserConfigDroppedMetric',
     'ServiceIntegrationExternalAwsCloudwatchMetricsUserConfigExtraMetric',
     'ServiceIntegrationKafkaConnectUserConfig',
     'ServiceIntegrationKafkaConnectUserConfigKafkaConnect',
     'ServiceIntegrationKafkaLogsUserConfig',
     'ServiceIntegrationKafkaMirrormakerUserConfig',
@@ -343,14 +343,15 @@
     'GetOpenSearchOpensearchUserConfigIndexTemplateResult',
     'GetOpenSearchOpensearchUserConfigIpFilterObjectResult',
     'GetOpenSearchOpensearchUserConfigOpensearchResult',
     'GetOpenSearchOpensearchUserConfigOpensearchDashboardsResult',
     'GetOpenSearchOpensearchUserConfigPrivateAccessResult',
     'GetOpenSearchOpensearchUserConfigPrivatelinkAccessResult',
     'GetOpenSearchOpensearchUserConfigPublicAccessResult',
+    'GetOpenSearchOpensearchUserConfigSamlResult',
     'GetOpenSearchServiceIntegrationResult',
     'GetOpenSearchTagResult',
     'GetPgComponentResult',
     'GetPgPgResult',
     'GetPgPgUserConfigResult',
     'GetPgPgUserConfigIpFilterObjectResult',
     'GetPgPgUserConfigMigrationResult',
@@ -391,15 +392,14 @@
     'GetServiceIntegrationEndpointExternalGoogleCloudLoggingUserConfigResult',
     'GetServiceIntegrationEndpointExternalKafkaUserConfigResult',
     'GetServiceIntegrationEndpointExternalOpensearchLogsUserConfigResult',
     'GetServiceIntegrationEndpointExternalSchemaRegistryUserConfigResult',
     'GetServiceIntegrationEndpointJolokiaUserConfigResult',
     'GetServiceIntegrationEndpointPrometheusUserConfigResult',
     'GetServiceIntegrationEndpointRsyslogUserConfigResult',
-    'GetServiceIntegrationEndpointSignalfxUserConfigResult',
     'GetServiceIntegrationExternalAwsCloudwatchMetricsUserConfigResult',
     'GetServiceIntegrationExternalAwsCloudwatchMetricsUserConfigDroppedMetricResult',
     'GetServiceIntegrationExternalAwsCloudwatchMetricsUserConfigExtraMetricResult',
     'GetServiceIntegrationKafkaConnectUserConfigResult',
     'GetServiceIntegrationKafkaConnectUserConfigKafkaConnectResult',
     'GetServiceIntegrationKafkaLogsUserConfigResult',
     'GetServiceIntegrationKafkaMirrormakerUserConfigResult',
@@ -4291,70 +4291,48 @@
 
     def __init__(__self__, *,
                  access_cert: Optional[str] = None,
                  access_key: Optional[str] = None,
                  connect_uri: Optional[str] = None,
                  rest_uri: Optional[str] = None,
                  schema_registry_uri: Optional[str] = None):
-        """
-        :param str access_cert: The Kafka client certificate
-        :param str access_key: The Kafka client certificate key
-        :param str connect_uri: The Kafka Connect URI, if any
-        :param str rest_uri: The Kafka REST URI, if any
-        :param str schema_registry_uri: The Schema Registry URI, if any
-        """
         if access_cert is not None:
             pulumi.set(__self__, "access_cert", access_cert)
         if access_key is not None:
             pulumi.set(__self__, "access_key", access_key)
         if connect_uri is not None:
             pulumi.set(__self__, "connect_uri", connect_uri)
         if rest_uri is not None:
             pulumi.set(__self__, "rest_uri", rest_uri)
         if schema_registry_uri is not None:
             pulumi.set(__self__, "schema_registry_uri", schema_registry_uri)
 
     @property
     @pulumi.getter(name="accessCert")
     def access_cert(self) -> Optional[str]:
-        """
-        The Kafka client certificate
-        """
         return pulumi.get(self, "access_cert")
 
     @property
     @pulumi.getter(name="accessKey")
     def access_key(self) -> Optional[str]:
-        """
-        The Kafka client certificate key
-        """
         return pulumi.get(self, "access_key")
 
     @property
     @pulumi.getter(name="connectUri")
     def connect_uri(self) -> Optional[str]:
-        """
-        The Kafka Connect URI, if any
-        """
         return pulumi.get(self, "connect_uri")
 
     @property
     @pulumi.getter(name="restUri")
     def rest_uri(self) -> Optional[str]:
-        """
-        The Kafka REST URI, if any
-        """
         return pulumi.get(self, "rest_uri")
 
     @property
     @pulumi.getter(name="schemaRegistryUri")
     def schema_registry_uri(self) -> Optional[str]:
-        """
-        The Schema Registry URI, if any
-        """
         return pulumi.get(self, "schema_registry_uri")
 
 
 @pulumi.output_type
 class KafkaKafkaUserConfig(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -8540,14 +8518,15 @@
                  opensearch_dashboards: Optional['outputs.OpenSearchOpensearchUserConfigOpensearchDashboards'] = None,
                  opensearch_version: Optional[str] = None,
                  private_access: Optional['outputs.OpenSearchOpensearchUserConfigPrivateAccess'] = None,
                  privatelink_access: Optional['outputs.OpenSearchOpensearchUserConfigPrivatelinkAccess'] = None,
                  project_to_fork_from: Optional[str] = None,
                  public_access: Optional['outputs.OpenSearchOpensearchUserConfigPublicAccess'] = None,
                  recovery_basebackup_name: Optional[str] = None,
+                 saml: Optional['outputs.OpenSearchOpensearchUserConfigSaml'] = None,
                  service_to_fork_from: Optional[str] = None,
                  static_ips: Optional[bool] = None):
         """
         :param str additional_backup_regions: Additional Cloud Regions for Backup Replication.
         :param str custom_domain: Serve the web frontend using a custom CNAME pointing to the Aiven DNS name.
         :param bool disable_replication_factor_adjustment: Disable automatic replication factor adjustment for multi-node services. By default, Aiven ensures all indexes are replicated at least to two nodes. Note: Due to potential data loss in case of losing a service node, this setting can no longer be activated.
         :param Sequence['OpenSearchOpensearchUserConfigIndexPatternArgs'] index_patterns: Index patterns.
@@ -8561,14 +8540,15 @@
         :param 'OpenSearchOpensearchUserConfigOpensearchDashboardsArgs' opensearch_dashboards: OpenSearch Dashboards settings.
         :param str opensearch_version: OpenSearch major version.
         :param 'OpenSearchOpensearchUserConfigPrivateAccessArgs' private_access: Allow access to selected service ports from private networks.
         :param 'OpenSearchOpensearchUserConfigPrivatelinkAccessArgs' privatelink_access: Allow access to selected service components through Privatelink.
         :param str project_to_fork_from: Name of another project to fork a service from. This has effect only when a new service is being created.
         :param 'OpenSearchOpensearchUserConfigPublicAccessArgs' public_access: Allow access to selected service ports from the public Internet.
         :param str recovery_basebackup_name: Name of the basebackup to restore in forked service.
+        :param 'OpenSearchOpensearchUserConfigSamlArgs' saml: OpenSearch SAML configuration.
         :param str service_to_fork_from: Name of another service to fork from. This has effect only when a new service is being created.
         :param bool static_ips: Use static public IP addresses.
         """
         if additional_backup_regions is not None:
             pulumi.set(__self__, "additional_backup_regions", additional_backup_regions)
         if custom_domain is not None:
             pulumi.set(__self__, "custom_domain", custom_domain)
@@ -8600,14 +8580,16 @@
             pulumi.set(__self__, "privatelink_access", privatelink_access)
         if project_to_fork_from is not None:
             pulumi.set(__self__, "project_to_fork_from", project_to_fork_from)
         if public_access is not None:
             pulumi.set(__self__, "public_access", public_access)
         if recovery_basebackup_name is not None:
             pulumi.set(__self__, "recovery_basebackup_name", recovery_basebackup_name)
+        if saml is not None:
+            pulumi.set(__self__, "saml", saml)
         if service_to_fork_from is not None:
             pulumi.set(__self__, "service_to_fork_from", service_to_fork_from)
         if static_ips is not None:
             pulumi.set(__self__, "static_ips", static_ips)
 
     @property
     @pulumi.getter(name="additionalBackupRegions")
@@ -8750,14 +8732,22 @@
     def recovery_basebackup_name(self) -> Optional[str]:
         """
         Name of the basebackup to restore in forked service.
         """
         return pulumi.get(self, "recovery_basebackup_name")
 
     @property
+    @pulumi.getter
+    def saml(self) -> Optional['outputs.OpenSearchOpensearchUserConfigSaml']:
+        """
+        OpenSearch SAML configuration.
+        """
+        return pulumi.get(self, "saml")
+
+    @property
     @pulumi.getter(name="serviceToForkFrom")
     def service_to_fork_from(self) -> Optional[str]:
         """
         Name of another service to fork from. This has effect only when a new service is being created.
         """
         return pulumi.get(self, "service_to_fork_from")
 
@@ -9417,14 +9407,88 @@
     @property
     @pulumi.getter
     def prometheus(self) -> Optional[bool]:
         return pulumi.get(self, "prometheus")
 
 
 @pulumi.output_type
+class OpenSearchOpensearchUserConfigSaml(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "idpEntityId":
+            suggest = "idp_entity_id"
+        elif key == "idpMetadataUrl":
+            suggest = "idp_metadata_url"
+        elif key == "spEntityId":
+            suggest = "sp_entity_id"
+        elif key == "rolesKey":
+            suggest = "roles_key"
+        elif key == "subjectKey":
+            suggest = "subject_key"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in OpenSearchOpensearchUserConfigSaml. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        OpenSearchOpensearchUserConfigSaml.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        OpenSearchOpensearchUserConfigSaml.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 enabled: bool,
+                 idp_entity_id: str,
+                 idp_metadata_url: str,
+                 sp_entity_id: str,
+                 roles_key: Optional[str] = None,
+                 subject_key: Optional[str] = None):
+        pulumi.set(__self__, "enabled", enabled)
+        pulumi.set(__self__, "idp_entity_id", idp_entity_id)
+        pulumi.set(__self__, "idp_metadata_url", idp_metadata_url)
+        pulumi.set(__self__, "sp_entity_id", sp_entity_id)
+        if roles_key is not None:
+            pulumi.set(__self__, "roles_key", roles_key)
+        if subject_key is not None:
+            pulumi.set(__self__, "subject_key", subject_key)
+
+    @property
+    @pulumi.getter
+    def enabled(self) -> bool:
+        return pulumi.get(self, "enabled")
+
+    @property
+    @pulumi.getter(name="idpEntityId")
+    def idp_entity_id(self) -> str:
+        return pulumi.get(self, "idp_entity_id")
+
+    @property
+    @pulumi.getter(name="idpMetadataUrl")
+    def idp_metadata_url(self) -> str:
+        return pulumi.get(self, "idp_metadata_url")
+
+    @property
+    @pulumi.getter(name="spEntityId")
+    def sp_entity_id(self) -> str:
+        return pulumi.get(self, "sp_entity_id")
+
+    @property
+    @pulumi.getter(name="rolesKey")
+    def roles_key(self) -> Optional[str]:
+        return pulumi.get(self, "roles_key")
+
+    @property
+    @pulumi.getter(name="subjectKey")
+    def subject_key(self) -> Optional[str]:
+        return pulumi.get(self, "subject_key")
+
+
+@pulumi.output_type
 class OpenSearchServiceIntegration(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "integrationType":
             suggest = "integration_type"
         elif key == "sourceServiceName":
@@ -12065,15 +12129,15 @@
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
         ServiceIntegrationEndpointDatadogUserConfig.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
-                 datadog_api_key: Optional[str] = None,
+                 datadog_api_key: str,
                  datadog_tags: Optional[Sequence['outputs.ServiceIntegrationEndpointDatadogUserConfigDatadogTag']] = None,
                  disable_consumer_stats: Optional[bool] = None,
                  kafka_consumer_check_instances: Optional[int] = None,
                  kafka_consumer_stats_timeout: Optional[int] = None,
                  max_partition_contexts: Optional[int] = None,
                  site: Optional[str] = None):
         """
@@ -12081,16 +12145,15 @@
         :param Sequence['ServiceIntegrationEndpointDatadogUserConfigDatadogTagArgs'] datadog_tags: Custom tags provided by user.
         :param bool disable_consumer_stats: Disable consumer group metrics.
         :param int kafka_consumer_check_instances: Number of separate instances to fetch kafka consumer statistics with.
         :param int kafka_consumer_stats_timeout: Number of seconds that datadog will wait to get consumer statistics from brokers.
         :param int max_partition_contexts: Maximum number of partition contexts to send.
         :param str site: Datadog intake site. Defaults to datadoghq.com.
         """
-        if datadog_api_key is not None:
-            pulumi.set(__self__, "datadog_api_key", datadog_api_key)
+        pulumi.set(__self__, "datadog_api_key", datadog_api_key)
         if datadog_tags is not None:
             pulumi.set(__self__, "datadog_tags", datadog_tags)
         if disable_consumer_stats is not None:
             pulumi.set(__self__, "disable_consumer_stats", disable_consumer_stats)
         if kafka_consumer_check_instances is not None:
             pulumi.set(__self__, "kafka_consumer_check_instances", kafka_consumer_check_instances)
         if kafka_consumer_stats_timeout is not None:
@@ -12098,15 +12161,15 @@
         if max_partition_contexts is not None:
             pulumi.set(__self__, "max_partition_contexts", max_partition_contexts)
         if site is not None:
             pulumi.set(__self__, "site", site)
 
     @property
     @pulumi.getter(name="datadogApiKey")
-    def datadog_api_key(self) -> Optional[str]:
+    def datadog_api_key(self) -> str:
         """
         Datadog API key.
         """
         return pulumi.get(self, "datadog_api_key")
 
     @property
     @pulumi.getter(name="datadogTags")
@@ -12180,82 +12243,79 @@
 @pulumi.output_type
 class ServiceIntegrationEndpointExternalAwsCloudwatchLogsUserConfig(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "accessKey":
             suggest = "access_key"
-        elif key == "logGroupName":
-            suggest = "log_group_name"
         elif key == "secretKey":
             suggest = "secret_key"
+        elif key == "logGroupName":
+            suggest = "log_group_name"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in ServiceIntegrationEndpointExternalAwsCloudwatchLogsUserConfig. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
         ServiceIntegrationEndpointExternalAwsCloudwatchLogsUserConfig.__key_warning(key)
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
         ServiceIntegrationEndpointExternalAwsCloudwatchLogsUserConfig.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
-                 access_key: Optional[str] = None,
-                 log_group_name: Optional[str] = None,
-                 region: Optional[str] = None,
-                 secret_key: Optional[str] = None):
+                 access_key: str,
+                 region: str,
+                 secret_key: str,
+                 log_group_name: Optional[str] = None):
         """
         :param str access_key: AWS access key. Required permissions are logs:CreateLogGroup, logs:CreateLogStream, logs:PutLogEvents and logs:DescribeLogStreams.
-        :param str log_group_name: AWS CloudWatch log group name.
         :param str region: AWS region.
         :param str secret_key: AWS secret key.
+        :param str log_group_name: AWS CloudWatch log group name.
         """
-        if access_key is not None:
-            pulumi.set(__self__, "access_key", access_key)
+        pulumi.set(__self__, "access_key", access_key)
+        pulumi.set(__self__, "region", region)
+        pulumi.set(__self__, "secret_key", secret_key)
         if log_group_name is not None:
             pulumi.set(__self__, "log_group_name", log_group_name)
-        if region is not None:
-            pulumi.set(__self__, "region", region)
-        if secret_key is not None:
-            pulumi.set(__self__, "secret_key", secret_key)
 
     @property
     @pulumi.getter(name="accessKey")
-    def access_key(self) -> Optional[str]:
+    def access_key(self) -> str:
         """
         AWS access key. Required permissions are logs:CreateLogGroup, logs:CreateLogStream, logs:PutLogEvents and logs:DescribeLogStreams.
         """
         return pulumi.get(self, "access_key")
 
     @property
-    @pulumi.getter(name="logGroupName")
-    def log_group_name(self) -> Optional[str]:
-        """
-        AWS CloudWatch log group name.
-        """
-        return pulumi.get(self, "log_group_name")
-
-    @property
     @pulumi.getter
-    def region(self) -> Optional[str]:
+    def region(self) -> str:
         """
         AWS region.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="secretKey")
-    def secret_key(self) -> Optional[str]:
+    def secret_key(self) -> str:
         """
         AWS secret key.
         """
         return pulumi.get(self, "secret_key")
 
+    @property
+    @pulumi.getter(name="logGroupName")
+    def log_group_name(self) -> Optional[str]:
+        """
+        AWS CloudWatch log group name.
+        """
+        return pulumi.get(self, "log_group_name")
+
 
 @pulumi.output_type
 class ServiceIntegrationEndpointExternalAwsCloudwatchMetricsUserConfig(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "accessKey":
@@ -12271,110 +12331,120 @@
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
         ServiceIntegrationEndpointExternalAwsCloudwatchMetricsUserConfig.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
-                 access_key: Optional[str] = None,
-                 namespace: Optional[str] = None,
-                 region: Optional[str] = None,
-                 secret_key: Optional[str] = None):
+                 access_key: str,
+                 namespace: str,
+                 region: str,
+                 secret_key: str):
         """
         :param str access_key: AWS access key. Required permissions are cloudwatch:PutMetricData.
         :param str namespace: AWS CloudWatch Metrics Namespace.
         :param str region: AWS region.
         :param str secret_key: AWS secret key.
         """
-        if access_key is not None:
-            pulumi.set(__self__, "access_key", access_key)
-        if namespace is not None:
-            pulumi.set(__self__, "namespace", namespace)
-        if region is not None:
-            pulumi.set(__self__, "region", region)
-        if secret_key is not None:
-            pulumi.set(__self__, "secret_key", secret_key)
+        pulumi.set(__self__, "access_key", access_key)
+        pulumi.set(__self__, "namespace", namespace)
+        pulumi.set(__self__, "region", region)
+        pulumi.set(__self__, "secret_key", secret_key)
 
     @property
     @pulumi.getter(name="accessKey")
-    def access_key(self) -> Optional[str]:
+    def access_key(self) -> str:
         """
         AWS access key. Required permissions are cloudwatch:PutMetricData.
         """
         return pulumi.get(self, "access_key")
 
     @property
     @pulumi.getter
-    def namespace(self) -> Optional[str]:
+    def namespace(self) -> str:
         """
         AWS CloudWatch Metrics Namespace.
         """
         return pulumi.get(self, "namespace")
 
     @property
     @pulumi.getter
-    def region(self) -> Optional[str]:
+    def region(self) -> str:
         """
         AWS region.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="secretKey")
-    def secret_key(self) -> Optional[str]:
+    def secret_key(self) -> str:
         """
         AWS secret key.
         """
         return pulumi.get(self, "secret_key")
 
 
 @pulumi.output_type
 class ServiceIntegrationEndpointExternalElasticsearchLogsUserConfig(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
-        if key == "indexDaysMax":
-            suggest = "index_days_max"
-        elif key == "indexPrefix":
+        if key == "indexPrefix":
             suggest = "index_prefix"
+        elif key == "indexDaysMax":
+            suggest = "index_days_max"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in ServiceIntegrationEndpointExternalElasticsearchLogsUserConfig. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
         ServiceIntegrationEndpointExternalElasticsearchLogsUserConfig.__key_warning(key)
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
         ServiceIntegrationEndpointExternalElasticsearchLogsUserConfig.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
+                 index_prefix: str,
+                 url: str,
                  ca: Optional[str] = None,
                  index_days_max: Optional[int] = None,
-                 index_prefix: Optional[str] = None,
-                 timeout: Optional[float] = None,
-                 url: Optional[str] = None):
+                 timeout: Optional[float] = None):
         """
+        :param str index_prefix: Elasticsearch index prefix. The default value is `logs`.
+        :param str url: Elasticsearch connection URL.
         :param str ca: PEM encoded CA certificate.
         :param int index_days_max: Maximum number of days of logs to keep. The default value is `3`.
-        :param str index_prefix: Elasticsearch index prefix. The default value is `logs`.
         :param float timeout: Elasticsearch request timeout limit. The default value is `10.0`.
-        :param str url: Elasticsearch connection URL.
         """
+        pulumi.set(__self__, "index_prefix", index_prefix)
+        pulumi.set(__self__, "url", url)
         if ca is not None:
             pulumi.set(__self__, "ca", ca)
         if index_days_max is not None:
             pulumi.set(__self__, "index_days_max", index_days_max)
-        if index_prefix is not None:
-            pulumi.set(__self__, "index_prefix", index_prefix)
         if timeout is not None:
             pulumi.set(__self__, "timeout", timeout)
-        if url is not None:
-            pulumi.set(__self__, "url", url)
+
+    @property
+    @pulumi.getter(name="indexPrefix")
+    def index_prefix(self) -> str:
+        """
+        Elasticsearch index prefix. The default value is `logs`.
+        """
+        return pulumi.get(self, "index_prefix")
+
+    @property
+    @pulumi.getter
+    def url(self) -> str:
+        """
+        Elasticsearch connection URL.
+        """
+        return pulumi.get(self, "url")
 
     @property
     @pulumi.getter
     def ca(self) -> Optional[str]:
         """
         PEM encoded CA certificate.
         """
@@ -12385,37 +12455,21 @@
     def index_days_max(self) -> Optional[int]:
         """
         Maximum number of days of logs to keep. The default value is `3`.
         """
         return pulumi.get(self, "index_days_max")
 
     @property
-    @pulumi.getter(name="indexPrefix")
-    def index_prefix(self) -> Optional[str]:
-        """
-        Elasticsearch index prefix. The default value is `logs`.
-        """
-        return pulumi.get(self, "index_prefix")
-
-    @property
     @pulumi.getter
     def timeout(self) -> Optional[float]:
         """
         Elasticsearch request timeout limit. The default value is `10.0`.
         """
         return pulumi.get(self, "timeout")
 
-    @property
-    @pulumi.getter
-    def url(self) -> Optional[str]:
-        """
-        Elasticsearch connection URL.
-        """
-        return pulumi.get(self, "url")
-
 
 @pulumi.output_type
 class ServiceIntegrationEndpointExternalGoogleCloudLoggingUserConfig(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "logId":
@@ -12433,69 +12487,66 @@
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
         ServiceIntegrationEndpointExternalGoogleCloudLoggingUserConfig.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
-                 log_id: Optional[str] = None,
-                 project_id: Optional[str] = None,
-                 service_account_credentials: Optional[str] = None):
+                 log_id: str,
+                 project_id: str,
+                 service_account_credentials: str):
         """
         :param str log_id: Google Cloud Logging log id.
         :param str project_id: GCP project id.
         :param str service_account_credentials: This is a JSON object with the fields documented in https://cloud.google.com/iam/docs/creating-managing-service-account-keys .
         """
-        if log_id is not None:
-            pulumi.set(__self__, "log_id", log_id)
-        if project_id is not None:
-            pulumi.set(__self__, "project_id", project_id)
-        if service_account_credentials is not None:
-            pulumi.set(__self__, "service_account_credentials", service_account_credentials)
+        pulumi.set(__self__, "log_id", log_id)
+        pulumi.set(__self__, "project_id", project_id)
+        pulumi.set(__self__, "service_account_credentials", service_account_credentials)
 
     @property
     @pulumi.getter(name="logId")
-    def log_id(self) -> Optional[str]:
+    def log_id(self) -> str:
         """
         Google Cloud Logging log id.
         """
         return pulumi.get(self, "log_id")
 
     @property
     @pulumi.getter(name="projectId")
-    def project_id(self) -> Optional[str]:
+    def project_id(self) -> str:
         """
         GCP project id.
         """
         return pulumi.get(self, "project_id")
 
     @property
     @pulumi.getter(name="serviceAccountCredentials")
-    def service_account_credentials(self) -> Optional[str]:
+    def service_account_credentials(self) -> str:
         """
         This is a JSON object with the fields documented in https://cloud.google.com/iam/docs/creating-managing-service-account-keys .
         """
         return pulumi.get(self, "service_account_credentials")
 
 
 @pulumi.output_type
 class ServiceIntegrationEndpointExternalKafkaUserConfig(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "bootstrapServers":
             suggest = "bootstrap_servers"
+        elif key == "securityProtocol":
+            suggest = "security_protocol"
         elif key == "saslMechanism":
             suggest = "sasl_mechanism"
         elif key == "saslPlainPassword":
             suggest = "sasl_plain_password"
         elif key == "saslPlainUsername":
             suggest = "sasl_plain_username"
-        elif key == "securityProtocol":
-            suggest = "security_protocol"
         elif key == "sslCaCert":
             suggest = "ssl_ca_cert"
         elif key == "sslClientCert":
             suggest = "ssl_client_cert"
         elif key == "sslClientKey":
             suggest = "ssl_client_key"
         elif key == "sslEndpointIdentificationAlgorithm":
@@ -12509,62 +12560,68 @@
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
         ServiceIntegrationEndpointExternalKafkaUserConfig.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
-                 bootstrap_servers: Optional[str] = None,
+                 bootstrap_servers: str,
+                 security_protocol: str,
                  sasl_mechanism: Optional[str] = None,
                  sasl_plain_password: Optional[str] = None,
                  sasl_plain_username: Optional[str] = None,
-                 security_protocol: Optional[str] = None,
                  ssl_ca_cert: Optional[str] = None,
                  ssl_client_cert: Optional[str] = None,
                  ssl_client_key: Optional[str] = None,
                  ssl_endpoint_identification_algorithm: Optional[str] = None):
         """
         :param str bootstrap_servers: Bootstrap servers.
+        :param str security_protocol: Security protocol.
         :param str sasl_mechanism: The list of SASL mechanisms enabled in the Kafka server.
         :param str sasl_plain_password: Password for SASL PLAIN mechanism in the Kafka server.
         :param str sasl_plain_username: Username for SASL PLAIN mechanism in the Kafka server.
-        :param str security_protocol: Security protocol.
         :param str ssl_ca_cert: PEM-encoded CA certificate.
         :param str ssl_client_cert: PEM-encoded client certificate.
         :param str ssl_client_key: PEM-encoded client key.
         :param str ssl_endpoint_identification_algorithm: The endpoint identification algorithm to validate server hostname using server certificate.
         """
-        if bootstrap_servers is not None:
-            pulumi.set(__self__, "bootstrap_servers", bootstrap_servers)
+        pulumi.set(__self__, "bootstrap_servers", bootstrap_servers)
+        pulumi.set(__self__, "security_protocol", security_protocol)
         if sasl_mechanism is not None:
             pulumi.set(__self__, "sasl_mechanism", sasl_mechanism)
         if sasl_plain_password is not None:
             pulumi.set(__self__, "sasl_plain_password", sasl_plain_password)
         if sasl_plain_username is not None:
             pulumi.set(__self__, "sasl_plain_username", sasl_plain_username)
-        if security_protocol is not None:
-            pulumi.set(__self__, "security_protocol", security_protocol)
         if ssl_ca_cert is not None:
             pulumi.set(__self__, "ssl_ca_cert", ssl_ca_cert)
         if ssl_client_cert is not None:
             pulumi.set(__self__, "ssl_client_cert", ssl_client_cert)
         if ssl_client_key is not None:
             pulumi.set(__self__, "ssl_client_key", ssl_client_key)
         if ssl_endpoint_identification_algorithm is not None:
             pulumi.set(__self__, "ssl_endpoint_identification_algorithm", ssl_endpoint_identification_algorithm)
 
     @property
     @pulumi.getter(name="bootstrapServers")
-    def bootstrap_servers(self) -> Optional[str]:
+    def bootstrap_servers(self) -> str:
         """
         Bootstrap servers.
         """
         return pulumi.get(self, "bootstrap_servers")
 
     @property
+    @pulumi.getter(name="securityProtocol")
+    def security_protocol(self) -> str:
+        """
+        Security protocol.
+        """
+        return pulumi.get(self, "security_protocol")
+
+    @property
     @pulumi.getter(name="saslMechanism")
     def sasl_mechanism(self) -> Optional[str]:
         """
         The list of SASL mechanisms enabled in the Kafka server.
         """
         return pulumi.get(self, "sasl_mechanism")
 
@@ -12581,22 +12638,14 @@
     def sasl_plain_username(self) -> Optional[str]:
         """
         Username for SASL PLAIN mechanism in the Kafka server.
         """
         return pulumi.get(self, "sasl_plain_username")
 
     @property
-    @pulumi.getter(name="securityProtocol")
-    def security_protocol(self) -> Optional[str]:
-        """
-        Security protocol.
-        """
-        return pulumi.get(self, "security_protocol")
-
-    @property
     @pulumi.getter(name="sslCaCert")
     def ssl_ca_cert(self) -> Optional[str]:
         """
         PEM-encoded CA certificate.
         """
         return pulumi.get(self, "ssl_ca_cert")
 
@@ -12626,53 +12675,67 @@
 
 
 @pulumi.output_type
 class ServiceIntegrationEndpointExternalOpensearchLogsUserConfig(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
-        if key == "indexDaysMax":
-            suggest = "index_days_max"
-        elif key == "indexPrefix":
+        if key == "indexPrefix":
             suggest = "index_prefix"
+        elif key == "indexDaysMax":
+            suggest = "index_days_max"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in ServiceIntegrationEndpointExternalOpensearchLogsUserConfig. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
         ServiceIntegrationEndpointExternalOpensearchLogsUserConfig.__key_warning(key)
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
         ServiceIntegrationEndpointExternalOpensearchLogsUserConfig.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
+                 index_prefix: str,
+                 url: str,
                  ca: Optional[str] = None,
                  index_days_max: Optional[int] = None,
-                 index_prefix: Optional[str] = None,
-                 timeout: Optional[float] = None,
-                 url: Optional[str] = None):
+                 timeout: Optional[float] = None):
         """
+        :param str index_prefix: OpenSearch index prefix. The default value is `logs`.
+        :param str url: OpenSearch connection URL.
         :param str ca: PEM encoded CA certificate.
         :param int index_days_max: Maximum number of days of logs to keep. The default value is `3`.
-        :param str index_prefix: OpenSearch index prefix. The default value is `logs`.
         :param float timeout: OpenSearch request timeout limit. The default value is `10.0`.
-        :param str url: OpenSearch connection URL.
         """
+        pulumi.set(__self__, "index_prefix", index_prefix)
+        pulumi.set(__self__, "url", url)
         if ca is not None:
             pulumi.set(__self__, "ca", ca)
         if index_days_max is not None:
             pulumi.set(__self__, "index_days_max", index_days_max)
-        if index_prefix is not None:
-            pulumi.set(__self__, "index_prefix", index_prefix)
         if timeout is not None:
             pulumi.set(__self__, "timeout", timeout)
-        if url is not None:
-            pulumi.set(__self__, "url", url)
+
+    @property
+    @pulumi.getter(name="indexPrefix")
+    def index_prefix(self) -> str:
+        """
+        OpenSearch index prefix. The default value is `logs`.
+        """
+        return pulumi.get(self, "index_prefix")
+
+    @property
+    @pulumi.getter
+    def url(self) -> str:
+        """
+        OpenSearch connection URL.
+        """
+        return pulumi.get(self, "url")
 
     @property
     @pulumi.getter
     def ca(self) -> Optional[str]:
         """
         PEM encoded CA certificate.
         """
@@ -12683,37 +12746,21 @@
     def index_days_max(self) -> Optional[int]:
         """
         Maximum number of days of logs to keep. The default value is `3`.
         """
         return pulumi.get(self, "index_days_max")
 
     @property
-    @pulumi.getter(name="indexPrefix")
-    def index_prefix(self) -> Optional[str]:
-        """
-        OpenSearch index prefix. The default value is `logs`.
-        """
-        return pulumi.get(self, "index_prefix")
-
-    @property
     @pulumi.getter
     def timeout(self) -> Optional[float]:
         """
         OpenSearch request timeout limit. The default value is `10.0`.
         """
         return pulumi.get(self, "timeout")
 
-    @property
-    @pulumi.getter
-    def url(self) -> Optional[str]:
-        """
-        OpenSearch connection URL.
-        """
-        return pulumi.get(self, "url")
-
 
 @pulumi.output_type
 class ServiceIntegrationEndpointExternalSchemaRegistryUserConfig(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "basicAuthPassword":
@@ -12729,42 +12776,48 @@
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
         ServiceIntegrationEndpointExternalSchemaRegistryUserConfig.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
-                 authentication: Optional[str] = None,
+                 authentication: str,
+                 url: str,
                  basic_auth_password: Optional[str] = None,
-                 basic_auth_username: Optional[str] = None,
-                 url: Optional[str] = None):
+                 basic_auth_username: Optional[str] = None):
         """
         :param str authentication: Authentication method.
+        :param str url: Schema Registry URL.
         :param str basic_auth_password: Basic authentication password.
         :param str basic_auth_username: Basic authentication user name.
-        :param str url: Schema Registry URL.
         """
-        if authentication is not None:
-            pulumi.set(__self__, "authentication", authentication)
+        pulumi.set(__self__, "authentication", authentication)
+        pulumi.set(__self__, "url", url)
         if basic_auth_password is not None:
             pulumi.set(__self__, "basic_auth_password", basic_auth_password)
         if basic_auth_username is not None:
             pulumi.set(__self__, "basic_auth_username", basic_auth_username)
-        if url is not None:
-            pulumi.set(__self__, "url", url)
 
     @property
     @pulumi.getter
-    def authentication(self) -> Optional[str]:
+    def authentication(self) -> str:
         """
         Authentication method.
         """
         return pulumi.get(self, "authentication")
 
     @property
+    @pulumi.getter
+    def url(self) -> str:
+        """
+        Schema Registry URL.
+        """
+        return pulumi.get(self, "url")
+
+    @property
     @pulumi.getter(name="basicAuthPassword")
     def basic_auth_password(self) -> Optional[str]:
         """
         Basic authentication password.
         """
         return pulumi.get(self, "basic_auth_password")
 
@@ -12772,22 +12825,14 @@
     @pulumi.getter(name="basicAuthUsername")
     def basic_auth_username(self) -> Optional[str]:
         """
         Basic authentication user name.
         """
         return pulumi.get(self, "basic_auth_username")
 
-    @property
-    @pulumi.getter
-    def url(self) -> Optional[str]:
-        """
-        Schema Registry URL.
-        """
-        return pulumi.get(self, "url")
-
 
 @pulumi.output_type
 class ServiceIntegrationEndpointJolokiaUserConfig(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "basicAuthPassword":
@@ -12884,188 +12929,120 @@
         """
         return pulumi.get(self, "basic_auth_username")
 
 
 @pulumi.output_type
 class ServiceIntegrationEndpointRsyslogUserConfig(dict):
     def __init__(__self__, *,
+                 format: str,
+                 port: int,
+                 server: str,
+                 tls: bool,
                  ca: Optional[str] = None,
                  cert: Optional[str] = None,
-                 format: Optional[str] = None,
                  key: Optional[str] = None,
                  logline: Optional[str] = None,
-                 port: Optional[int] = None,
-                 sd: Optional[str] = None,
-                 server: Optional[str] = None,
-                 tls: Optional[bool] = None):
+                 sd: Optional[str] = None):
         """
+        :param str format: message format. The default value is `rfc5424`.
+        :param int port: rsyslog server port. The default value is `514`.
+        :param str server: rsyslog server IP address or hostname.
+        :param bool tls: Require TLS. The default value is `true`.
         :param str ca: PEM encoded CA certificate.
         :param str cert: PEM encoded client certificate.
-        :param str format: message format. The default value is `rfc5424`.
         :param str key: PEM encoded client key.
         :param str logline: custom syslog message format.
-        :param int port: rsyslog server port. The default value is `514`.
         :param str sd: Structured data block for log message.
-        :param str server: rsyslog server IP address or hostname.
-        :param bool tls: Require TLS. The default value is `true`.
         """
+        pulumi.set(__self__, "format", format)
+        pulumi.set(__self__, "port", port)
+        pulumi.set(__self__, "server", server)
+        pulumi.set(__self__, "tls", tls)
         if ca is not None:
             pulumi.set(__self__, "ca", ca)
         if cert is not None:
             pulumi.set(__self__, "cert", cert)
-        if format is not None:
-            pulumi.set(__self__, "format", format)
         if key is not None:
             pulumi.set(__self__, "key", key)
         if logline is not None:
             pulumi.set(__self__, "logline", logline)
-        if port is not None:
-            pulumi.set(__self__, "port", port)
         if sd is not None:
             pulumi.set(__self__, "sd", sd)
-        if server is not None:
-            pulumi.set(__self__, "server", server)
-        if tls is not None:
-            pulumi.set(__self__, "tls", tls)
-
-    @property
-    @pulumi.getter
-    def ca(self) -> Optional[str]:
-        """
-        PEM encoded CA certificate.
-        """
-        return pulumi.get(self, "ca")
 
     @property
     @pulumi.getter
-    def cert(self) -> Optional[str]:
-        """
-        PEM encoded client certificate.
-        """
-        return pulumi.get(self, "cert")
-
-    @property
-    @pulumi.getter
-    def format(self) -> Optional[str]:
+    def format(self) -> str:
         """
         message format. The default value is `rfc5424`.
         """
         return pulumi.get(self, "format")
 
     @property
     @pulumi.getter
-    def key(self) -> Optional[str]:
+    def port(self) -> int:
         """
-        PEM encoded client key.
+        rsyslog server port. The default value is `514`.
         """
-        return pulumi.get(self, "key")
+        return pulumi.get(self, "port")
 
     @property
     @pulumi.getter
-    def logline(self) -> Optional[str]:
+    def server(self) -> str:
         """
-        custom syslog message format.
+        rsyslog server IP address or hostname.
         """
-        return pulumi.get(self, "logline")
+        return pulumi.get(self, "server")
 
     @property
     @pulumi.getter
-    def port(self) -> Optional[int]:
+    def tls(self) -> bool:
         """
-        rsyslog server port. The default value is `514`.
+        Require TLS. The default value is `true`.
         """
-        return pulumi.get(self, "port")
+        return pulumi.get(self, "tls")
 
     @property
     @pulumi.getter
-    def sd(self) -> Optional[str]:
+    def ca(self) -> Optional[str]:
         """
-        Structured data block for log message.
+        PEM encoded CA certificate.
         """
-        return pulumi.get(self, "sd")
+        return pulumi.get(self, "ca")
 
     @property
     @pulumi.getter
-    def server(self) -> Optional[str]:
+    def cert(self) -> Optional[str]:
         """
-        rsyslog server IP address or hostname.
+        PEM encoded client certificate.
         """
-        return pulumi.get(self, "server")
+        return pulumi.get(self, "cert")
 
     @property
     @pulumi.getter
-    def tls(self) -> Optional[bool]:
-        """
-        Require TLS. The default value is `true`.
-        """
-        return pulumi.get(self, "tls")
-
-
-@pulumi.output_type
-class ServiceIntegrationEndpointSignalfxUserConfig(dict):
-    @staticmethod
-    def __key_warning(key: str):
-        suggest = None
-        if key == "enabledMetrics":
-            suggest = "enabled_metrics"
-        elif key == "signalfxApiKey":
-            suggest = "signalfx_api_key"
-        elif key == "signalfxRealm":
-            suggest = "signalfx_realm"
-
-        if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in ServiceIntegrationEndpointSignalfxUserConfig. Access the value via the '{suggest}' property getter instead.")
-
-    def __getitem__(self, key: str) -> Any:
-        ServiceIntegrationEndpointSignalfxUserConfig.__key_warning(key)
-        return super().__getitem__(key)
-
-    def get(self, key: str, default = None) -> Any:
-        ServiceIntegrationEndpointSignalfxUserConfig.__key_warning(key)
-        return super().get(key, default)
-
-    def __init__(__self__, *,
-                 enabled_metrics: Optional[Sequence[str]] = None,
-                 signalfx_api_key: Optional[str] = None,
-                 signalfx_realm: Optional[str] = None):
-        """
-        :param Sequence[str] enabled_metrics: list of metrics to send.
-        :param str signalfx_api_key: SignalFX API key.
-        :param str signalfx_realm: SignalFX realm. The default value is `us0`.
-        """
-        if enabled_metrics is not None:
-            pulumi.set(__self__, "enabled_metrics", enabled_metrics)
-        if signalfx_api_key is not None:
-            pulumi.set(__self__, "signalfx_api_key", signalfx_api_key)
-        if signalfx_realm is not None:
-            pulumi.set(__self__, "signalfx_realm", signalfx_realm)
-
-    @property
-    @pulumi.getter(name="enabledMetrics")
-    def enabled_metrics(self) -> Optional[Sequence[str]]:
+    def key(self) -> Optional[str]:
         """
-        list of metrics to send.
+        PEM encoded client key.
         """
-        return pulumi.get(self, "enabled_metrics")
+        return pulumi.get(self, "key")
 
     @property
-    @pulumi.getter(name="signalfxApiKey")
-    def signalfx_api_key(self) -> Optional[str]:
+    @pulumi.getter
+    def logline(self) -> Optional[str]:
         """
-        SignalFX API key.
+        custom syslog message format.
         """
-        return pulumi.get(self, "signalfx_api_key")
+        return pulumi.get(self, "logline")
 
     @property
-    @pulumi.getter(name="signalfxRealm")
-    def signalfx_realm(self) -> Optional[str]:
+    @pulumi.getter
+    def sd(self) -> Optional[str]:
         """
-        SignalFX realm. The default value is `us0`.
+        Structured data block for log message.
         """
-        return pulumi.get(self, "signalfx_realm")
+        return pulumi.get(self, "sd")
 
 
 @pulumi.output_type
 class ServiceIntegrationExternalAwsCloudwatchMetricsUserConfig(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
@@ -13264,24 +13241,23 @@
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
         ServiceIntegrationKafkaLogsUserConfig.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
-                 kafka_topic: Optional[str] = None):
+                 kafka_topic: str):
         """
         :param str kafka_topic: Topic name.
         """
-        if kafka_topic is not None:
-            pulumi.set(__self__, "kafka_topic", kafka_topic)
+        pulumi.set(__self__, "kafka_topic", kafka_topic)
 
     @property
     @pulumi.getter(name="kafkaTopic")
-    def kafka_topic(self) -> Optional[str]:
+    def kafka_topic(self) -> str:
         """
         Topic name.
         """
         return pulumi.get(self, "kafka_topic")
 
 
 @pulumi.output_type
@@ -19582,14 +19558,15 @@
                  opensearch_dashboards: Optional['outputs.GetOpenSearchOpensearchUserConfigOpensearchDashboardsResult'] = None,
                  opensearch_version: Optional[str] = None,
                  private_access: Optional['outputs.GetOpenSearchOpensearchUserConfigPrivateAccessResult'] = None,
                  privatelink_access: Optional['outputs.GetOpenSearchOpensearchUserConfigPrivatelinkAccessResult'] = None,
                  project_to_fork_from: Optional[str] = None,
                  public_access: Optional['outputs.GetOpenSearchOpensearchUserConfigPublicAccessResult'] = None,
                  recovery_basebackup_name: Optional[str] = None,
+                 saml: Optional['outputs.GetOpenSearchOpensearchUserConfigSamlResult'] = None,
                  service_to_fork_from: Optional[str] = None,
                  static_ips: Optional[bool] = None):
         """
         :param 'GetOpenSearchOpensearchUserConfigOpensearchArgs' opensearch: Opensearch server provided values
         :param bool static_ips: Static IPs that are going to be associated with this service. Please assign a value using the 'toset' function. Once a static ip resource is in the 'assigned' state it cannot be unbound from the node again
         """
         if additional_backup_regions is not None:
@@ -19624,14 +19601,16 @@
             pulumi.set(__self__, "privatelink_access", privatelink_access)
         if project_to_fork_from is not None:
             pulumi.set(__self__, "project_to_fork_from", project_to_fork_from)
         if public_access is not None:
             pulumi.set(__self__, "public_access", public_access)
         if recovery_basebackup_name is not None:
             pulumi.set(__self__, "recovery_basebackup_name", recovery_basebackup_name)
+        if saml is not None:
+            pulumi.set(__self__, "saml", saml)
         if service_to_fork_from is not None:
             pulumi.set(__self__, "service_to_fork_from", service_to_fork_from)
         if static_ips is not None:
             pulumi.set(__self__, "static_ips", static_ips)
 
     @property
     @pulumi.getter(name="additionalBackupRegions")
@@ -19723,14 +19702,19 @@
 
     @property
     @pulumi.getter(name="recoveryBasebackupName")
     def recovery_basebackup_name(self) -> Optional[str]:
         return pulumi.get(self, "recovery_basebackup_name")
 
     @property
+    @pulumi.getter
+    def saml(self) -> Optional['outputs.GetOpenSearchOpensearchUserConfigSamlResult']:
+        return pulumi.get(self, "saml")
+
+    @property
     @pulumi.getter(name="serviceToForkFrom")
     def service_to_fork_from(self) -> Optional[str]:
         return pulumi.get(self, "service_to_fork_from")
 
     @property
     @pulumi.getter(name="staticIps")
     def static_ips(self) -> Optional[bool]:
@@ -20200,14 +20184,63 @@
     @property
     @pulumi.getter
     def prometheus(self) -> Optional[bool]:
         return pulumi.get(self, "prometheus")
 
 
 @pulumi.output_type
+class GetOpenSearchOpensearchUserConfigSamlResult(dict):
+    def __init__(__self__, *,
+                 enabled: bool,
+                 idp_entity_id: str,
+                 idp_metadata_url: str,
+                 sp_entity_id: str,
+                 roles_key: Optional[str] = None,
+                 subject_key: Optional[str] = None):
+        pulumi.set(__self__, "enabled", enabled)
+        pulumi.set(__self__, "idp_entity_id", idp_entity_id)
+        pulumi.set(__self__, "idp_metadata_url", idp_metadata_url)
+        pulumi.set(__self__, "sp_entity_id", sp_entity_id)
+        if roles_key is not None:
+            pulumi.set(__self__, "roles_key", roles_key)
+        if subject_key is not None:
+            pulumi.set(__self__, "subject_key", subject_key)
+
+    @property
+    @pulumi.getter
+    def enabled(self) -> bool:
+        return pulumi.get(self, "enabled")
+
+    @property
+    @pulumi.getter(name="idpEntityId")
+    def idp_entity_id(self) -> str:
+        return pulumi.get(self, "idp_entity_id")
+
+    @property
+    @pulumi.getter(name="idpMetadataUrl")
+    def idp_metadata_url(self) -> str:
+        return pulumi.get(self, "idp_metadata_url")
+
+    @property
+    @pulumi.getter(name="spEntityId")
+    def sp_entity_id(self) -> str:
+        return pulumi.get(self, "sp_entity_id")
+
+    @property
+    @pulumi.getter(name="rolesKey")
+    def roles_key(self) -> Optional[str]:
+        return pulumi.get(self, "roles_key")
+
+    @property
+    @pulumi.getter(name="subjectKey")
+    def subject_key(self) -> Optional[str]:
+        return pulumi.get(self, "subject_key")
+
+
+@pulumi.output_type
 class GetOpenSearchServiceIntegrationResult(dict):
     def __init__(__self__, *,
                  integration_type: str,
                  source_service_name: str):
         pulumi.set(__self__, "integration_type", integration_type)
         pulumi.set(__self__, "source_service_name", source_service_name)
 
@@ -22065,23 +22098,22 @@
     def pshard_stats_enabled(self) -> Optional[bool]:
         return pulumi.get(self, "pshard_stats_enabled")
 
 
 @pulumi.output_type
 class GetServiceIntegrationEndpointDatadogUserConfigResult(dict):
     def __init__(__self__, *,
-                 datadog_api_key: Optional[str] = None,
+                 datadog_api_key: str,
                  datadog_tags: Optional[Sequence['outputs.GetServiceIntegrationEndpointDatadogUserConfigDatadogTagResult']] = None,
                  disable_consumer_stats: Optional[bool] = None,
                  kafka_consumer_check_instances: Optional[int] = None,
                  kafka_consumer_stats_timeout: Optional[int] = None,
                  max_partition_contexts: Optional[int] = None,
                  site: Optional[str] = None):
-        if datadog_api_key is not None:
-            pulumi.set(__self__, "datadog_api_key", datadog_api_key)
+        pulumi.set(__self__, "datadog_api_key", datadog_api_key)
         if datadog_tags is not None:
             pulumi.set(__self__, "datadog_tags", datadog_tags)
         if disable_consumer_stats is not None:
             pulumi.set(__self__, "disable_consumer_stats", disable_consumer_stats)
         if kafka_consumer_check_instances is not None:
             pulumi.set(__self__, "kafka_consumer_check_instances", kafka_consumer_check_instances)
         if kafka_consumer_stats_timeout is not None:
@@ -22089,15 +22121,15 @@
         if max_partition_contexts is not None:
             pulumi.set(__self__, "max_partition_contexts", max_partition_contexts)
         if site is not None:
             pulumi.set(__self__, "site", site)
 
     @property
     @pulumi.getter(name="datadogApiKey")
-    def datadog_api_key(self) -> Optional[str]:
+    def datadog_api_key(self) -> str:
         return pulumi.get(self, "datadog_api_key")
 
     @property
     @pulumi.getter(name="datadogTags")
     def datadog_tags(self) -> Optional[Sequence['outputs.GetServiceIntegrationEndpointDatadogUserConfigDatadogTagResult']]:
         return pulumi.get(self, "datadog_tags")
 
@@ -22146,196 +22178,187 @@
     def comment(self) -> Optional[str]:
         return pulumi.get(self, "comment")
 
 
 @pulumi.output_type
 class GetServiceIntegrationEndpointExternalAwsCloudwatchLogsUserConfigResult(dict):
     def __init__(__self__, *,
-                 access_key: Optional[str] = None,
-                 log_group_name: Optional[str] = None,
-                 region: Optional[str] = None,
-                 secret_key: Optional[str] = None):
-        if access_key is not None:
-            pulumi.set(__self__, "access_key", access_key)
+                 access_key: str,
+                 region: str,
+                 secret_key: str,
+                 log_group_name: Optional[str] = None):
+        pulumi.set(__self__, "access_key", access_key)
+        pulumi.set(__self__, "region", region)
+        pulumi.set(__self__, "secret_key", secret_key)
         if log_group_name is not None:
             pulumi.set(__self__, "log_group_name", log_group_name)
-        if region is not None:
-            pulumi.set(__self__, "region", region)
-        if secret_key is not None:
-            pulumi.set(__self__, "secret_key", secret_key)
 
     @property
     @pulumi.getter(name="accessKey")
-    def access_key(self) -> Optional[str]:
+    def access_key(self) -> str:
         return pulumi.get(self, "access_key")
 
     @property
-    @pulumi.getter(name="logGroupName")
-    def log_group_name(self) -> Optional[str]:
-        return pulumi.get(self, "log_group_name")
-
-    @property
     @pulumi.getter
-    def region(self) -> Optional[str]:
+    def region(self) -> str:
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="secretKey")
-    def secret_key(self) -> Optional[str]:
+    def secret_key(self) -> str:
         return pulumi.get(self, "secret_key")
 
+    @property
+    @pulumi.getter(name="logGroupName")
+    def log_group_name(self) -> Optional[str]:
+        return pulumi.get(self, "log_group_name")
+
 
 @pulumi.output_type
 class GetServiceIntegrationEndpointExternalAwsCloudwatchMetricsUserConfigResult(dict):
     def __init__(__self__, *,
-                 access_key: Optional[str] = None,
-                 namespace: Optional[str] = None,
-                 region: Optional[str] = None,
-                 secret_key: Optional[str] = None):
-        if access_key is not None:
-            pulumi.set(__self__, "access_key", access_key)
-        if namespace is not None:
-            pulumi.set(__self__, "namespace", namespace)
-        if region is not None:
-            pulumi.set(__self__, "region", region)
-        if secret_key is not None:
-            pulumi.set(__self__, "secret_key", secret_key)
+                 access_key: str,
+                 namespace: str,
+                 region: str,
+                 secret_key: str):
+        pulumi.set(__self__, "access_key", access_key)
+        pulumi.set(__self__, "namespace", namespace)
+        pulumi.set(__self__, "region", region)
+        pulumi.set(__self__, "secret_key", secret_key)
 
     @property
     @pulumi.getter(name="accessKey")
-    def access_key(self) -> Optional[str]:
+    def access_key(self) -> str:
         return pulumi.get(self, "access_key")
 
     @property
     @pulumi.getter
-    def namespace(self) -> Optional[str]:
+    def namespace(self) -> str:
         return pulumi.get(self, "namespace")
 
     @property
     @pulumi.getter
-    def region(self) -> Optional[str]:
+    def region(self) -> str:
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="secretKey")
-    def secret_key(self) -> Optional[str]:
+    def secret_key(self) -> str:
         return pulumi.get(self, "secret_key")
 
 
 @pulumi.output_type
 class GetServiceIntegrationEndpointExternalElasticsearchLogsUserConfigResult(dict):
     def __init__(__self__, *,
+                 index_prefix: str,
+                 url: str,
                  ca: Optional[str] = None,
                  index_days_max: Optional[int] = None,
-                 index_prefix: Optional[str] = None,
-                 timeout: Optional[float] = None,
-                 url: Optional[str] = None):
+                 timeout: Optional[float] = None):
+        pulumi.set(__self__, "index_prefix", index_prefix)
+        pulumi.set(__self__, "url", url)
         if ca is not None:
             pulumi.set(__self__, "ca", ca)
         if index_days_max is not None:
             pulumi.set(__self__, "index_days_max", index_days_max)
-        if index_prefix is not None:
-            pulumi.set(__self__, "index_prefix", index_prefix)
         if timeout is not None:
             pulumi.set(__self__, "timeout", timeout)
-        if url is not None:
-            pulumi.set(__self__, "url", url)
+
+    @property
+    @pulumi.getter(name="indexPrefix")
+    def index_prefix(self) -> str:
+        return pulumi.get(self, "index_prefix")
+
+    @property
+    @pulumi.getter
+    def url(self) -> str:
+        return pulumi.get(self, "url")
 
     @property
     @pulumi.getter
     def ca(self) -> Optional[str]:
         return pulumi.get(self, "ca")
 
     @property
     @pulumi.getter(name="indexDaysMax")
     def index_days_max(self) -> Optional[int]:
         return pulumi.get(self, "index_days_max")
 
     @property
-    @pulumi.getter(name="indexPrefix")
-    def index_prefix(self) -> Optional[str]:
-        return pulumi.get(self, "index_prefix")
-
-    @property
     @pulumi.getter
     def timeout(self) -> Optional[float]:
         return pulumi.get(self, "timeout")
 
-    @property
-    @pulumi.getter
-    def url(self) -> Optional[str]:
-        return pulumi.get(self, "url")
-
 
 @pulumi.output_type
 class GetServiceIntegrationEndpointExternalGoogleCloudLoggingUserConfigResult(dict):
     def __init__(__self__, *,
-                 log_id: Optional[str] = None,
-                 project_id: Optional[str] = None,
-                 service_account_credentials: Optional[str] = None):
-        if log_id is not None:
-            pulumi.set(__self__, "log_id", log_id)
-        if project_id is not None:
-            pulumi.set(__self__, "project_id", project_id)
-        if service_account_credentials is not None:
-            pulumi.set(__self__, "service_account_credentials", service_account_credentials)
+                 log_id: str,
+                 project_id: str,
+                 service_account_credentials: str):
+        pulumi.set(__self__, "log_id", log_id)
+        pulumi.set(__self__, "project_id", project_id)
+        pulumi.set(__self__, "service_account_credentials", service_account_credentials)
 
     @property
     @pulumi.getter(name="logId")
-    def log_id(self) -> Optional[str]:
+    def log_id(self) -> str:
         return pulumi.get(self, "log_id")
 
     @property
     @pulumi.getter(name="projectId")
-    def project_id(self) -> Optional[str]:
+    def project_id(self) -> str:
         return pulumi.get(self, "project_id")
 
     @property
     @pulumi.getter(name="serviceAccountCredentials")
-    def service_account_credentials(self) -> Optional[str]:
+    def service_account_credentials(self) -> str:
         return pulumi.get(self, "service_account_credentials")
 
 
 @pulumi.output_type
 class GetServiceIntegrationEndpointExternalKafkaUserConfigResult(dict):
     def __init__(__self__, *,
-                 bootstrap_servers: Optional[str] = None,
+                 bootstrap_servers: str,
+                 security_protocol: str,
                  sasl_mechanism: Optional[str] = None,
                  sasl_plain_password: Optional[str] = None,
                  sasl_plain_username: Optional[str] = None,
-                 security_protocol: Optional[str] = None,
                  ssl_ca_cert: Optional[str] = None,
                  ssl_client_cert: Optional[str] = None,
                  ssl_client_key: Optional[str] = None,
                  ssl_endpoint_identification_algorithm: Optional[str] = None):
-        if bootstrap_servers is not None:
-            pulumi.set(__self__, "bootstrap_servers", bootstrap_servers)
+        pulumi.set(__self__, "bootstrap_servers", bootstrap_servers)
+        pulumi.set(__self__, "security_protocol", security_protocol)
         if sasl_mechanism is not None:
             pulumi.set(__self__, "sasl_mechanism", sasl_mechanism)
         if sasl_plain_password is not None:
             pulumi.set(__self__, "sasl_plain_password", sasl_plain_password)
         if sasl_plain_username is not None:
             pulumi.set(__self__, "sasl_plain_username", sasl_plain_username)
-        if security_protocol is not None:
-            pulumi.set(__self__, "security_protocol", security_protocol)
         if ssl_ca_cert is not None:
             pulumi.set(__self__, "ssl_ca_cert", ssl_ca_cert)
         if ssl_client_cert is not None:
             pulumi.set(__self__, "ssl_client_cert", ssl_client_cert)
         if ssl_client_key is not None:
             pulumi.set(__self__, "ssl_client_key", ssl_client_key)
         if ssl_endpoint_identification_algorithm is not None:
             pulumi.set(__self__, "ssl_endpoint_identification_algorithm", ssl_endpoint_identification_algorithm)
 
     @property
     @pulumi.getter(name="bootstrapServers")
-    def bootstrap_servers(self) -> Optional[str]:
+    def bootstrap_servers(self) -> str:
         return pulumi.get(self, "bootstrap_servers")
 
     @property
+    @pulumi.getter(name="securityProtocol")
+    def security_protocol(self) -> str:
+        return pulumi.get(self, "security_protocol")
+
+    @property
     @pulumi.getter(name="saslMechanism")
     def sasl_mechanism(self) -> Optional[str]:
         return pulumi.get(self, "sasl_mechanism")
 
     @property
     @pulumi.getter(name="saslPlainPassword")
     def sasl_plain_password(self) -> Optional[str]:
@@ -22343,19 +22366,14 @@
 
     @property
     @pulumi.getter(name="saslPlainUsername")
     def sasl_plain_username(self) -> Optional[str]:
         return pulumi.get(self, "sasl_plain_username")
 
     @property
-    @pulumi.getter(name="securityProtocol")
-    def security_protocol(self) -> Optional[str]:
-        return pulumi.get(self, "security_protocol")
-
-    @property
     @pulumi.getter(name="sslCaCert")
     def ssl_ca_cert(self) -> Optional[str]:
         return pulumi.get(self, "ssl_ca_cert")
 
     @property
     @pulumi.getter(name="sslClientCert")
     def ssl_client_cert(self) -> Optional[str]:
@@ -22371,92 +22389,88 @@
     def ssl_endpoint_identification_algorithm(self) -> Optional[str]:
         return pulumi.get(self, "ssl_endpoint_identification_algorithm")
 
 
 @pulumi.output_type
 class GetServiceIntegrationEndpointExternalOpensearchLogsUserConfigResult(dict):
     def __init__(__self__, *,
+                 index_prefix: str,
+                 url: str,
                  ca: Optional[str] = None,
                  index_days_max: Optional[int] = None,
-                 index_prefix: Optional[str] = None,
-                 timeout: Optional[float] = None,
-                 url: Optional[str] = None):
+                 timeout: Optional[float] = None):
+        pulumi.set(__self__, "index_prefix", index_prefix)
+        pulumi.set(__self__, "url", url)
         if ca is not None:
             pulumi.set(__self__, "ca", ca)
         if index_days_max is not None:
             pulumi.set(__self__, "index_days_max", index_days_max)
-        if index_prefix is not None:
-            pulumi.set(__self__, "index_prefix", index_prefix)
         if timeout is not None:
             pulumi.set(__self__, "timeout", timeout)
-        if url is not None:
-            pulumi.set(__self__, "url", url)
+
+    @property
+    @pulumi.getter(name="indexPrefix")
+    def index_prefix(self) -> str:
+        return pulumi.get(self, "index_prefix")
+
+    @property
+    @pulumi.getter
+    def url(self) -> str:
+        return pulumi.get(self, "url")
 
     @property
     @pulumi.getter
     def ca(self) -> Optional[str]:
         return pulumi.get(self, "ca")
 
     @property
     @pulumi.getter(name="indexDaysMax")
     def index_days_max(self) -> Optional[int]:
         return pulumi.get(self, "index_days_max")
 
     @property
-    @pulumi.getter(name="indexPrefix")
-    def index_prefix(self) -> Optional[str]:
-        return pulumi.get(self, "index_prefix")
-
-    @property
     @pulumi.getter
     def timeout(self) -> Optional[float]:
         return pulumi.get(self, "timeout")
 
-    @property
-    @pulumi.getter
-    def url(self) -> Optional[str]:
-        return pulumi.get(self, "url")
-
 
 @pulumi.output_type
 class GetServiceIntegrationEndpointExternalSchemaRegistryUserConfigResult(dict):
     def __init__(__self__, *,
-                 authentication: Optional[str] = None,
+                 authentication: str,
+                 url: str,
                  basic_auth_password: Optional[str] = None,
-                 basic_auth_username: Optional[str] = None,
-                 url: Optional[str] = None):
-        if authentication is not None:
-            pulumi.set(__self__, "authentication", authentication)
+                 basic_auth_username: Optional[str] = None):
+        pulumi.set(__self__, "authentication", authentication)
+        pulumi.set(__self__, "url", url)
         if basic_auth_password is not None:
             pulumi.set(__self__, "basic_auth_password", basic_auth_password)
         if basic_auth_username is not None:
             pulumi.set(__self__, "basic_auth_username", basic_auth_username)
-        if url is not None:
-            pulumi.set(__self__, "url", url)
 
     @property
     @pulumi.getter
-    def authentication(self) -> Optional[str]:
+    def authentication(self) -> str:
         return pulumi.get(self, "authentication")
 
     @property
+    @pulumi.getter
+    def url(self) -> str:
+        return pulumi.get(self, "url")
+
+    @property
     @pulumi.getter(name="basicAuthPassword")
     def basic_auth_password(self) -> Optional[str]:
         return pulumi.get(self, "basic_auth_password")
 
     @property
     @pulumi.getter(name="basicAuthUsername")
     def basic_auth_username(self) -> Optional[str]:
         return pulumi.get(self, "basic_auth_username")
 
-    @property
-    @pulumi.getter
-    def url(self) -> Optional[str]:
-        return pulumi.get(self, "url")
-
 
 @pulumi.output_type
 class GetServiceIntegrationEndpointJolokiaUserConfigResult(dict):
     def __init__(__self__, *,
                  basic_auth_password: Optional[str] = None,
                  basic_auth_username: Optional[str] = None):
         if basic_auth_password is not None:
@@ -22495,115 +22509,82 @@
     def basic_auth_username(self) -> Optional[str]:
         return pulumi.get(self, "basic_auth_username")
 
 
 @pulumi.output_type
 class GetServiceIntegrationEndpointRsyslogUserConfigResult(dict):
     def __init__(__self__, *,
+                 format: str,
+                 port: int,
+                 server: str,
+                 tls: bool,
                  ca: Optional[str] = None,
                  cert: Optional[str] = None,
-                 format: Optional[str] = None,
                  key: Optional[str] = None,
                  logline: Optional[str] = None,
-                 port: Optional[int] = None,
-                 sd: Optional[str] = None,
-                 server: Optional[str] = None,
-                 tls: Optional[bool] = None):
+                 sd: Optional[str] = None):
+        pulumi.set(__self__, "format", format)
+        pulumi.set(__self__, "port", port)
+        pulumi.set(__self__, "server", server)
+        pulumi.set(__self__, "tls", tls)
         if ca is not None:
             pulumi.set(__self__, "ca", ca)
         if cert is not None:
             pulumi.set(__self__, "cert", cert)
-        if format is not None:
-            pulumi.set(__self__, "format", format)
         if key is not None:
             pulumi.set(__self__, "key", key)
         if logline is not None:
             pulumi.set(__self__, "logline", logline)
-        if port is not None:
-            pulumi.set(__self__, "port", port)
         if sd is not None:
             pulumi.set(__self__, "sd", sd)
-        if server is not None:
-            pulumi.set(__self__, "server", server)
-        if tls is not None:
-            pulumi.set(__self__, "tls", tls)
 
     @property
     @pulumi.getter
-    def ca(self) -> Optional[str]:
-        return pulumi.get(self, "ca")
+    def format(self) -> str:
+        return pulumi.get(self, "format")
 
     @property
     @pulumi.getter
-    def cert(self) -> Optional[str]:
-        return pulumi.get(self, "cert")
+    def port(self) -> int:
+        return pulumi.get(self, "port")
 
     @property
     @pulumi.getter
-    def format(self) -> Optional[str]:
-        return pulumi.get(self, "format")
+    def server(self) -> str:
+        return pulumi.get(self, "server")
 
     @property
     @pulumi.getter
-    def key(self) -> Optional[str]:
-        return pulumi.get(self, "key")
+    def tls(self) -> bool:
+        return pulumi.get(self, "tls")
 
     @property
     @pulumi.getter
-    def logline(self) -> Optional[str]:
-        return pulumi.get(self, "logline")
+    def ca(self) -> Optional[str]:
+        return pulumi.get(self, "ca")
 
     @property
     @pulumi.getter
-    def port(self) -> Optional[int]:
-        return pulumi.get(self, "port")
+    def cert(self) -> Optional[str]:
+        return pulumi.get(self, "cert")
 
     @property
     @pulumi.getter
-    def sd(self) -> Optional[str]:
-        return pulumi.get(self, "sd")
+    def key(self) -> Optional[str]:
+        return pulumi.get(self, "key")
 
     @property
     @pulumi.getter
-    def server(self) -> Optional[str]:
-        return pulumi.get(self, "server")
+    def logline(self) -> Optional[str]:
+        return pulumi.get(self, "logline")
 
     @property
     @pulumi.getter
-    def tls(self) -> Optional[bool]:
-        return pulumi.get(self, "tls")
-
-
-@pulumi.output_type
-class GetServiceIntegrationEndpointSignalfxUserConfigResult(dict):
-    def __init__(__self__, *,
-                 enabled_metrics: Optional[Sequence[str]] = None,
-                 signalfx_api_key: Optional[str] = None,
-                 signalfx_realm: Optional[str] = None):
-        if enabled_metrics is not None:
-            pulumi.set(__self__, "enabled_metrics", enabled_metrics)
-        if signalfx_api_key is not None:
-            pulumi.set(__self__, "signalfx_api_key", signalfx_api_key)
-        if signalfx_realm is not None:
-            pulumi.set(__self__, "signalfx_realm", signalfx_realm)
-
-    @property
-    @pulumi.getter(name="enabledMetrics")
-    def enabled_metrics(self) -> Optional[Sequence[str]]:
-        return pulumi.get(self, "enabled_metrics")
-
-    @property
-    @pulumi.getter(name="signalfxApiKey")
-    def signalfx_api_key(self) -> Optional[str]:
-        return pulumi.get(self, "signalfx_api_key")
-
-    @property
-    @pulumi.getter(name="signalfxRealm")
-    def signalfx_realm(self) -> Optional[str]:
-        return pulumi.get(self, "signalfx_realm")
+    def sd(self) -> Optional[str]:
+        return pulumi.get(self, "sd")
 
 
 @pulumi.output_type
 class GetServiceIntegrationExternalAwsCloudwatchMetricsUserConfigResult(dict):
     def __init__(__self__, *,
                  dropped_metrics: Optional[Sequence['outputs.GetServiceIntegrationExternalAwsCloudwatchMetricsUserConfigDroppedMetricResult']] = None,
                  extra_metrics: Optional[Sequence['outputs.GetServiceIntegrationExternalAwsCloudwatchMetricsUserConfigExtraMetricResult']] = None):
@@ -22710,21 +22691,20 @@
     def status_storage_topic(self) -> Optional[str]:
         return pulumi.get(self, "status_storage_topic")
 
 
 @pulumi.output_type
 class GetServiceIntegrationKafkaLogsUserConfigResult(dict):
     def __init__(__self__, *,
-                 kafka_topic: Optional[str] = None):
-        if kafka_topic is not None:
-            pulumi.set(__self__, "kafka_topic", kafka_topic)
+                 kafka_topic: str):
+        pulumi.set(__self__, "kafka_topic", kafka_topic)
 
     @property
     @pulumi.getter(name="kafkaTopic")
-    def kafka_topic(self) -> Optional[str]:
+    def kafka_topic(self) -> str:
         return pulumi.get(self, "kafka_topic")
 
 
 @pulumi.output_type
 class GetServiceIntegrationKafkaMirrormakerUserConfigResult(dict):
     def __init__(__self__, *,
                  cluster_alias: Optional[str] = None,
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/pg.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/pg.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,17 @@
         """
         pulumi.set(__self__, "project", project)
         if additional_disk_space is not None:
             pulumi.set(__self__, "additional_disk_space", additional_disk_space)
         if cloud_name is not None:
             pulumi.set(__self__, "cloud_name", cloud_name)
         if disk_space is not None:
+            warnings.warn("""This will be removed in v5.0.0 and replaced with additional_disk_space instead.""", DeprecationWarning)
+            pulumi.log.warn("""disk_space is deprecated: This will be removed in v5.0.0 and replaced with additional_disk_space instead.""")
+        if disk_space is not None:
             pulumi.set(__self__, "disk_space", disk_space)
         if maintenance_window_dow is not None:
             pulumi.set(__self__, "maintenance_window_dow", maintenance_window_dow)
         if maintenance_window_time is not None:
             pulumi.set(__self__, "maintenance_window_time", maintenance_window_time)
         if pg is not None:
             pulumi.set(__self__, "pg", pg)
@@ -323,14 +326,17 @@
         if additional_disk_space is not None:
             pulumi.set(__self__, "additional_disk_space", additional_disk_space)
         if cloud_name is not None:
             pulumi.set(__self__, "cloud_name", cloud_name)
         if components is not None:
             pulumi.set(__self__, "components", components)
         if disk_space is not None:
+            warnings.warn("""This will be removed in v5.0.0 and replaced with additional_disk_space instead.""", DeprecationWarning)
+            pulumi.log.warn("""disk_space is deprecated: This will be removed in v5.0.0 and replaced with additional_disk_space instead.""")
+        if disk_space is not None:
             pulumi.set(__self__, "disk_space", disk_space)
         if disk_space_cap is not None:
             pulumi.set(__self__, "disk_space_cap", disk_space_cap)
         if disk_space_default is not None:
             pulumi.set(__self__, "disk_space_default", disk_space_default)
         if disk_space_step is not None:
             pulumi.set(__self__, "disk_space_step", disk_space_step)
@@ -800,14 +806,17 @@
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = PgArgs.__new__(PgArgs)
 
             __props__.__dict__["additional_disk_space"] = additional_disk_space
             __props__.__dict__["cloud_name"] = cloud_name
+            if disk_space is not None and not opts.urn:
+                warnings.warn("""This will be removed in v5.0.0 and replaced with additional_disk_space instead.""", DeprecationWarning)
+                pulumi.log.warn("""disk_space is deprecated: This will be removed in v5.0.0 and replaced with additional_disk_space instead.""")
             __props__.__dict__["disk_space"] = disk_space
             __props__.__dict__["maintenance_window_dow"] = maintenance_window_dow
             __props__.__dict__["maintenance_window_time"] = maintenance_window_time
             __props__.__dict__["pg"] = pg
             __props__.__dict__["pg_user_config"] = pg_user_config
             __props__.__dict__["plan"] = plan
             if project is None and not opts.urn:
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/pg_database.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/pg_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/pg_user.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/pg_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/project.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/project.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/project_user.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/project_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/project_vpc.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/project_vpc.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/provider.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/redis.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/redis.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,17 @@
         pulumi.set(__self__, "project", project)
         pulumi.set(__self__, "service_name", service_name)
         if additional_disk_space is not None:
             pulumi.set(__self__, "additional_disk_space", additional_disk_space)
         if cloud_name is not None:
             pulumi.set(__self__, "cloud_name", cloud_name)
         if disk_space is not None:
+            warnings.warn("""This will be removed in v5.0.0 and replaced with additional_disk_space instead.""", DeprecationWarning)
+            pulumi.log.warn("""disk_space is deprecated: This will be removed in v5.0.0 and replaced with additional_disk_space instead.""")
+        if disk_space is not None:
             pulumi.set(__self__, "disk_space", disk_space)
         if maintenance_window_dow is not None:
             pulumi.set(__self__, "maintenance_window_dow", maintenance_window_dow)
         if maintenance_window_time is not None:
             pulumi.set(__self__, "maintenance_window_time", maintenance_window_time)
         if plan is not None:
             pulumi.set(__self__, "plan", plan)
@@ -368,14 +371,17 @@
         if additional_disk_space is not None:
             pulumi.set(__self__, "additional_disk_space", additional_disk_space)
         if cloud_name is not None:
             pulumi.set(__self__, "cloud_name", cloud_name)
         if components is not None:
             pulumi.set(__self__, "components", components)
         if disk_space is not None:
+            warnings.warn("""This will be removed in v5.0.0 and replaced with additional_disk_space instead.""", DeprecationWarning)
+            pulumi.log.warn("""disk_space is deprecated: This will be removed in v5.0.0 and replaced with additional_disk_space instead.""")
+        if disk_space is not None:
             pulumi.set(__self__, "disk_space", disk_space)
         if disk_space_cap is not None:
             pulumi.set(__self__, "disk_space_cap", disk_space_cap)
         if disk_space_default is not None:
             pulumi.set(__self__, "disk_space_default", disk_space_default)
         if disk_space_step is not None:
             pulumi.set(__self__, "disk_space_step", disk_space_step)
@@ -926,14 +932,17 @@
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = RedisArgs.__new__(RedisArgs)
 
             __props__.__dict__["additional_disk_space"] = additional_disk_space
             __props__.__dict__["cloud_name"] = cloud_name
+            if disk_space is not None and not opts.urn:
+                warnings.warn("""This will be removed in v5.0.0 and replaced with additional_disk_space instead.""", DeprecationWarning)
+                pulumi.log.warn("""disk_space is deprecated: This will be removed in v5.0.0 and replaced with additional_disk_space instead.""")
             __props__.__dict__["disk_space"] = disk_space
             __props__.__dict__["maintenance_window_dow"] = maintenance_window_dow
             __props__.__dict__["maintenance_window_time"] = maintenance_window_time
             __props__.__dict__["plan"] = plan
             if project is None and not opts.urn:
                 raise TypeError("Missing required property 'project'")
             __props__.__dict__["project"] = project
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/redis_user.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/redis_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -322,14 +322,20 @@
         foo = aiven.RedisUser("foo",
             service_name=aiven_redis["bar"]["service_name"],
             project="my-project",
             username="user-1",
             password="Test$1234")
         ```
 
+        ## Import
+
+        ```sh
+         $ pulumi import aiven:index/redisUser:RedisUser foo project/service_name/username
+        ```
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] password: The password of the Redis User.
         :param pulumi.Input[str] project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] redis_acl_categories: Defines command category rules. The field is required with`redis_acl_commands` and `redis_acl_keys`. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] redis_acl_channels: Defines the permitted pub/sub channel patterns. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] redis_acl_commands: Defines rules for individual commands. The field is required with`redis_acl_categories` and `redis_acl_keys`. This property cannot be changed, doing so forces recreation of the resource.
@@ -355,14 +361,20 @@
         foo = aiven.RedisUser("foo",
             service_name=aiven_redis["bar"]["service_name"],
             project="my-project",
             username="user-1",
             password="Test$1234")
         ```
 
+        ## Import
+
+        ```sh
+         $ pulumi import aiven:index/redisUser:RedisUser foo project/service_name/username
+        ```
+
         :param str resource_name: The name of the resource.
         :param RedisUserArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(RedisUserArgs, pulumi.ResourceOptions, *args, **kwargs)
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/service_integration.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/service_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/service_integration_endpoint.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/service_integration_endpoint.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,33 +25,31 @@
                  external_elasticsearch_logs_user_config: Optional[pulumi.Input['ServiceIntegrationEndpointExternalElasticsearchLogsUserConfigArgs']] = None,
                  external_google_cloud_logging_user_config: Optional[pulumi.Input['ServiceIntegrationEndpointExternalGoogleCloudLoggingUserConfigArgs']] = None,
                  external_kafka_user_config: Optional[pulumi.Input['ServiceIntegrationEndpointExternalKafkaUserConfigArgs']] = None,
                  external_opensearch_logs_user_config: Optional[pulumi.Input['ServiceIntegrationEndpointExternalOpensearchLogsUserConfigArgs']] = None,
                  external_schema_registry_user_config: Optional[pulumi.Input['ServiceIntegrationEndpointExternalSchemaRegistryUserConfigArgs']] = None,
                  jolokia_user_config: Optional[pulumi.Input['ServiceIntegrationEndpointJolokiaUserConfigArgs']] = None,
                  prometheus_user_config: Optional[pulumi.Input['ServiceIntegrationEndpointPrometheusUserConfigArgs']] = None,
-                 rsyslog_user_config: Optional[pulumi.Input['ServiceIntegrationEndpointRsyslogUserConfigArgs']] = None,
-                 signalfx_user_config: Optional[pulumi.Input['ServiceIntegrationEndpointSignalfxUserConfigArgs']] = None):
+                 rsyslog_user_config: Optional[pulumi.Input['ServiceIntegrationEndpointRsyslogUserConfigArgs']] = None):
         """
         The set of arguments for constructing a ServiceIntegrationEndpoint resource.
         :param pulumi.Input[str] endpoint_name: Name of the service integration endpoint
-        :param pulumi.Input[str] endpoint_type: Type of the service integration endpoint
+        :param pulumi.Input[str] endpoint_type: Type of the service integration endpoint. Possible values: `datadog`, `prometheus`, `rsyslog`, `external_elasticsearch_logs`, `external_opensearch_logs`, `external_aws_cloudwatch_logs`, `external_google_cloud_logging`, `external_kafka`, `jolokia`, `external_schema_registry`, `external_aws_cloudwatch_metrics`
         :param pulumi.Input[str] project: Project the service integration endpoint belongs to
         :param pulumi.Input['ServiceIntegrationEndpointDatadogUserConfigArgs'] datadog_user_config: Datadog user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointExternalAwsCloudwatchLogsUserConfigArgs'] external_aws_cloudwatch_logs_user_config: ExternalAwsCloudwatchLogs user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointExternalAwsCloudwatchMetricsUserConfigArgs'] external_aws_cloudwatch_metrics_user_config: ExternalAwsCloudwatchMetrics user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointExternalElasticsearchLogsUserConfigArgs'] external_elasticsearch_logs_user_config: ExternalElasticsearchLogs user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointExternalGoogleCloudLoggingUserConfigArgs'] external_google_cloud_logging_user_config: ExternalGoogleCloudLogging user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointExternalKafkaUserConfigArgs'] external_kafka_user_config: ExternalKafka user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointExternalOpensearchLogsUserConfigArgs'] external_opensearch_logs_user_config: ExternalOpensearchLogs user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointExternalSchemaRegistryUserConfigArgs'] external_schema_registry_user_config: ExternalSchemaRegistry user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointJolokiaUserConfigArgs'] jolokia_user_config: Jolokia user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointPrometheusUserConfigArgs'] prometheus_user_config: Prometheus user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointRsyslogUserConfigArgs'] rsyslog_user_config: Rsyslog user configurable settings
-        :param pulumi.Input['ServiceIntegrationEndpointSignalfxUserConfigArgs'] signalfx_user_config: Signalfx user configurable settings
         """
         pulumi.set(__self__, "endpoint_name", endpoint_name)
         pulumi.set(__self__, "endpoint_type", endpoint_type)
         pulumi.set(__self__, "project", project)
         if datadog_user_config is not None:
             pulumi.set(__self__, "datadog_user_config", datadog_user_config)
         if external_aws_cloudwatch_logs_user_config is not None:
@@ -70,16 +68,14 @@
             pulumi.set(__self__, "external_schema_registry_user_config", external_schema_registry_user_config)
         if jolokia_user_config is not None:
             pulumi.set(__self__, "jolokia_user_config", jolokia_user_config)
         if prometheus_user_config is not None:
             pulumi.set(__self__, "prometheus_user_config", prometheus_user_config)
         if rsyslog_user_config is not None:
             pulumi.set(__self__, "rsyslog_user_config", rsyslog_user_config)
-        if signalfx_user_config is not None:
-            pulumi.set(__self__, "signalfx_user_config", signalfx_user_config)
 
     @property
     @pulumi.getter(name="endpointName")
     def endpoint_name(self) -> pulumi.Input[str]:
         """
         Name of the service integration endpoint
         """
@@ -89,15 +85,15 @@
     def endpoint_name(self, value: pulumi.Input[str]):
         pulumi.set(self, "endpoint_name", value)
 
     @property
     @pulumi.getter(name="endpointType")
     def endpoint_type(self) -> pulumi.Input[str]:
         """
-        Type of the service integration endpoint
+        Type of the service integration endpoint. Possible values: `datadog`, `prometheus`, `rsyslog`, `external_elasticsearch_logs`, `external_opensearch_logs`, `external_aws_cloudwatch_logs`, `external_google_cloud_logging`, `external_kafka`, `jolokia`, `external_schema_registry`, `external_aws_cloudwatch_metrics`
         """
         return pulumi.get(self, "endpoint_type")
 
     @endpoint_type.setter
     def endpoint_type(self, value: pulumi.Input[str]):
         pulumi.set(self, "endpoint_type", value)
 
@@ -241,26 +237,14 @@
         """
         return pulumi.get(self, "rsyslog_user_config")
 
     @rsyslog_user_config.setter
     def rsyslog_user_config(self, value: Optional[pulumi.Input['ServiceIntegrationEndpointRsyslogUserConfigArgs']]):
         pulumi.set(self, "rsyslog_user_config", value)
 
-    @property
-    @pulumi.getter(name="signalfxUserConfig")
-    def signalfx_user_config(self) -> Optional[pulumi.Input['ServiceIntegrationEndpointSignalfxUserConfigArgs']]:
-        """
-        Signalfx user configurable settings
-        """
-        return pulumi.get(self, "signalfx_user_config")
-
-    @signalfx_user_config.setter
-    def signalfx_user_config(self, value: Optional[pulumi.Input['ServiceIntegrationEndpointSignalfxUserConfigArgs']]):
-        pulumi.set(self, "signalfx_user_config", value)
-
 
 @pulumi.input_type
 class _ServiceIntegrationEndpointState:
     def __init__(__self__, *,
                  datadog_user_config: Optional[pulumi.Input['ServiceIntegrationEndpointDatadogUserConfigArgs']] = None,
                  endpoint_config: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  endpoint_name: Optional[pulumi.Input[str]] = None,
@@ -271,34 +255,32 @@
                  external_google_cloud_logging_user_config: Optional[pulumi.Input['ServiceIntegrationEndpointExternalGoogleCloudLoggingUserConfigArgs']] = None,
                  external_kafka_user_config: Optional[pulumi.Input['ServiceIntegrationEndpointExternalKafkaUserConfigArgs']] = None,
                  external_opensearch_logs_user_config: Optional[pulumi.Input['ServiceIntegrationEndpointExternalOpensearchLogsUserConfigArgs']] = None,
                  external_schema_registry_user_config: Optional[pulumi.Input['ServiceIntegrationEndpointExternalSchemaRegistryUserConfigArgs']] = None,
                  jolokia_user_config: Optional[pulumi.Input['ServiceIntegrationEndpointJolokiaUserConfigArgs']] = None,
                  project: Optional[pulumi.Input[str]] = None,
                  prometheus_user_config: Optional[pulumi.Input['ServiceIntegrationEndpointPrometheusUserConfigArgs']] = None,
-                 rsyslog_user_config: Optional[pulumi.Input['ServiceIntegrationEndpointRsyslogUserConfigArgs']] = None,
-                 signalfx_user_config: Optional[pulumi.Input['ServiceIntegrationEndpointSignalfxUserConfigArgs']] = None):
+                 rsyslog_user_config: Optional[pulumi.Input['ServiceIntegrationEndpointRsyslogUserConfigArgs']] = None):
         """
         Input properties used for looking up and filtering ServiceIntegrationEndpoint resources.
         :param pulumi.Input['ServiceIntegrationEndpointDatadogUserConfigArgs'] datadog_user_config: Datadog user configurable settings
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] endpoint_config: Integration endpoint specific backend configuration
         :param pulumi.Input[str] endpoint_name: Name of the service integration endpoint
-        :param pulumi.Input[str] endpoint_type: Type of the service integration endpoint
+        :param pulumi.Input[str] endpoint_type: Type of the service integration endpoint. Possible values: `datadog`, `prometheus`, `rsyslog`, `external_elasticsearch_logs`, `external_opensearch_logs`, `external_aws_cloudwatch_logs`, `external_google_cloud_logging`, `external_kafka`, `jolokia`, `external_schema_registry`, `external_aws_cloudwatch_metrics`
         :param pulumi.Input['ServiceIntegrationEndpointExternalAwsCloudwatchLogsUserConfigArgs'] external_aws_cloudwatch_logs_user_config: ExternalAwsCloudwatchLogs user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointExternalAwsCloudwatchMetricsUserConfigArgs'] external_aws_cloudwatch_metrics_user_config: ExternalAwsCloudwatchMetrics user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointExternalElasticsearchLogsUserConfigArgs'] external_elasticsearch_logs_user_config: ExternalElasticsearchLogs user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointExternalGoogleCloudLoggingUserConfigArgs'] external_google_cloud_logging_user_config: ExternalGoogleCloudLogging user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointExternalKafkaUserConfigArgs'] external_kafka_user_config: ExternalKafka user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointExternalOpensearchLogsUserConfigArgs'] external_opensearch_logs_user_config: ExternalOpensearchLogs user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointExternalSchemaRegistryUserConfigArgs'] external_schema_registry_user_config: ExternalSchemaRegistry user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointJolokiaUserConfigArgs'] jolokia_user_config: Jolokia user configurable settings
         :param pulumi.Input[str] project: Project the service integration endpoint belongs to
         :param pulumi.Input['ServiceIntegrationEndpointPrometheusUserConfigArgs'] prometheus_user_config: Prometheus user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointRsyslogUserConfigArgs'] rsyslog_user_config: Rsyslog user configurable settings
-        :param pulumi.Input['ServiceIntegrationEndpointSignalfxUserConfigArgs'] signalfx_user_config: Signalfx user configurable settings
         """
         if datadog_user_config is not None:
             pulumi.set(__self__, "datadog_user_config", datadog_user_config)
         if endpoint_config is not None:
             pulumi.set(__self__, "endpoint_config", endpoint_config)
         if endpoint_name is not None:
             pulumi.set(__self__, "endpoint_name", endpoint_name)
@@ -322,16 +304,14 @@
             pulumi.set(__self__, "jolokia_user_config", jolokia_user_config)
         if project is not None:
             pulumi.set(__self__, "project", project)
         if prometheus_user_config is not None:
             pulumi.set(__self__, "prometheus_user_config", prometheus_user_config)
         if rsyslog_user_config is not None:
             pulumi.set(__self__, "rsyslog_user_config", rsyslog_user_config)
-        if signalfx_user_config is not None:
-            pulumi.set(__self__, "signalfx_user_config", signalfx_user_config)
 
     @property
     @pulumi.getter(name="datadogUserConfig")
     def datadog_user_config(self) -> Optional[pulumi.Input['ServiceIntegrationEndpointDatadogUserConfigArgs']]:
         """
         Datadog user configurable settings
         """
@@ -365,15 +345,15 @@
     def endpoint_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "endpoint_name", value)
 
     @property
     @pulumi.getter(name="endpointType")
     def endpoint_type(self) -> Optional[pulumi.Input[str]]:
         """
-        Type of the service integration endpoint
+        Type of the service integration endpoint. Possible values: `datadog`, `prometheus`, `rsyslog`, `external_elasticsearch_logs`, `external_opensearch_logs`, `external_aws_cloudwatch_logs`, `external_google_cloud_logging`, `external_kafka`, `jolokia`, `external_schema_registry`, `external_aws_cloudwatch_metrics`
         """
         return pulumi.get(self, "endpoint_type")
 
     @endpoint_type.setter
     def endpoint_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "endpoint_type", value)
 
@@ -505,26 +485,14 @@
         """
         return pulumi.get(self, "rsyslog_user_config")
 
     @rsyslog_user_config.setter
     def rsyslog_user_config(self, value: Optional[pulumi.Input['ServiceIntegrationEndpointRsyslogUserConfigArgs']]):
         pulumi.set(self, "rsyslog_user_config", value)
 
-    @property
-    @pulumi.getter(name="signalfxUserConfig")
-    def signalfx_user_config(self) -> Optional[pulumi.Input['ServiceIntegrationEndpointSignalfxUserConfigArgs']]:
-        """
-        Signalfx user configurable settings
-        """
-        return pulumi.get(self, "signalfx_user_config")
-
-    @signalfx_user_config.setter
-    def signalfx_user_config(self, value: Optional[pulumi.Input['ServiceIntegrationEndpointSignalfxUserConfigArgs']]):
-        pulumi.set(self, "signalfx_user_config", value)
-
 
 class ServiceIntegrationEndpoint(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  datadog_user_config: Optional[pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointDatadogUserConfigArgs']]] = None,
@@ -537,36 +505,34 @@
                  external_kafka_user_config: Optional[pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalKafkaUserConfigArgs']]] = None,
                  external_opensearch_logs_user_config: Optional[pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalOpensearchLogsUserConfigArgs']]] = None,
                  external_schema_registry_user_config: Optional[pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalSchemaRegistryUserConfigArgs']]] = None,
                  jolokia_user_config: Optional[pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointJolokiaUserConfigArgs']]] = None,
                  project: Optional[pulumi.Input[str]] = None,
                  prometheus_user_config: Optional[pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointPrometheusUserConfigArgs']]] = None,
                  rsyslog_user_config: Optional[pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointRsyslogUserConfigArgs']]] = None,
-                 signalfx_user_config: Optional[pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointSignalfxUserConfigArgs']]] = None,
                  __props__=None):
         """
         The Service Integration Endpoint resource allows the creation and management of Aiven Service Integration Endpoints.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointDatadogUserConfigArgs']] datadog_user_config: Datadog user configurable settings
         :param pulumi.Input[str] endpoint_name: Name of the service integration endpoint
-        :param pulumi.Input[str] endpoint_type: Type of the service integration endpoint
+        :param pulumi.Input[str] endpoint_type: Type of the service integration endpoint. Possible values: `datadog`, `prometheus`, `rsyslog`, `external_elasticsearch_logs`, `external_opensearch_logs`, `external_aws_cloudwatch_logs`, `external_google_cloud_logging`, `external_kafka`, `jolokia`, `external_schema_registry`, `external_aws_cloudwatch_metrics`
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalAwsCloudwatchLogsUserConfigArgs']] external_aws_cloudwatch_logs_user_config: ExternalAwsCloudwatchLogs user configurable settings
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalAwsCloudwatchMetricsUserConfigArgs']] external_aws_cloudwatch_metrics_user_config: ExternalAwsCloudwatchMetrics user configurable settings
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalElasticsearchLogsUserConfigArgs']] external_elasticsearch_logs_user_config: ExternalElasticsearchLogs user configurable settings
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalGoogleCloudLoggingUserConfigArgs']] external_google_cloud_logging_user_config: ExternalGoogleCloudLogging user configurable settings
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalKafkaUserConfigArgs']] external_kafka_user_config: ExternalKafka user configurable settings
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalOpensearchLogsUserConfigArgs']] external_opensearch_logs_user_config: ExternalOpensearchLogs user configurable settings
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalSchemaRegistryUserConfigArgs']] external_schema_registry_user_config: ExternalSchemaRegistry user configurable settings
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointJolokiaUserConfigArgs']] jolokia_user_config: Jolokia user configurable settings
         :param pulumi.Input[str] project: Project the service integration endpoint belongs to
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointPrometheusUserConfigArgs']] prometheus_user_config: Prometheus user configurable settings
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointRsyslogUserConfigArgs']] rsyslog_user_config: Rsyslog user configurable settings
-        :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointSignalfxUserConfigArgs']] signalfx_user_config: Signalfx user configurable settings
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ServiceIntegrationEndpointArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -598,15 +564,14 @@
                  external_kafka_user_config: Optional[pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalKafkaUserConfigArgs']]] = None,
                  external_opensearch_logs_user_config: Optional[pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalOpensearchLogsUserConfigArgs']]] = None,
                  external_schema_registry_user_config: Optional[pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalSchemaRegistryUserConfigArgs']]] = None,
                  jolokia_user_config: Optional[pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointJolokiaUserConfigArgs']]] = None,
                  project: Optional[pulumi.Input[str]] = None,
                  prometheus_user_config: Optional[pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointPrometheusUserConfigArgs']]] = None,
                  rsyslog_user_config: Optional[pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointRsyslogUserConfigArgs']]] = None,
-                 signalfx_user_config: Optional[pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointSignalfxUserConfigArgs']]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
@@ -628,15 +593,14 @@
             __props__.__dict__["external_schema_registry_user_config"] = external_schema_registry_user_config
             __props__.__dict__["jolokia_user_config"] = jolokia_user_config
             if project is None and not opts.urn:
                 raise TypeError("Missing required property 'project'")
             __props__.__dict__["project"] = project
             __props__.__dict__["prometheus_user_config"] = prometheus_user_config
             __props__.__dict__["rsyslog_user_config"] = rsyslog_user_config
-            __props__.__dict__["signalfx_user_config"] = signalfx_user_config
             __props__.__dict__["endpoint_config"] = None
         super(ServiceIntegrationEndpoint, __self__).__init__(
             'aiven:index/serviceIntegrationEndpoint:ServiceIntegrationEndpoint',
             resource_name,
             __props__,
             opts)
 
@@ -654,39 +618,37 @@
             external_google_cloud_logging_user_config: Optional[pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalGoogleCloudLoggingUserConfigArgs']]] = None,
             external_kafka_user_config: Optional[pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalKafkaUserConfigArgs']]] = None,
             external_opensearch_logs_user_config: Optional[pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalOpensearchLogsUserConfigArgs']]] = None,
             external_schema_registry_user_config: Optional[pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalSchemaRegistryUserConfigArgs']]] = None,
             jolokia_user_config: Optional[pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointJolokiaUserConfigArgs']]] = None,
             project: Optional[pulumi.Input[str]] = None,
             prometheus_user_config: Optional[pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointPrometheusUserConfigArgs']]] = None,
-            rsyslog_user_config: Optional[pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointRsyslogUserConfigArgs']]] = None,
-            signalfx_user_config: Optional[pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointSignalfxUserConfigArgs']]] = None) -> 'ServiceIntegrationEndpoint':
+            rsyslog_user_config: Optional[pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointRsyslogUserConfigArgs']]] = None) -> 'ServiceIntegrationEndpoint':
         """
         Get an existing ServiceIntegrationEndpoint resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointDatadogUserConfigArgs']] datadog_user_config: Datadog user configurable settings
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] endpoint_config: Integration endpoint specific backend configuration
         :param pulumi.Input[str] endpoint_name: Name of the service integration endpoint
-        :param pulumi.Input[str] endpoint_type: Type of the service integration endpoint
+        :param pulumi.Input[str] endpoint_type: Type of the service integration endpoint. Possible values: `datadog`, `prometheus`, `rsyslog`, `external_elasticsearch_logs`, `external_opensearch_logs`, `external_aws_cloudwatch_logs`, `external_google_cloud_logging`, `external_kafka`, `jolokia`, `external_schema_registry`, `external_aws_cloudwatch_metrics`
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalAwsCloudwatchLogsUserConfigArgs']] external_aws_cloudwatch_logs_user_config: ExternalAwsCloudwatchLogs user configurable settings
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalAwsCloudwatchMetricsUserConfigArgs']] external_aws_cloudwatch_metrics_user_config: ExternalAwsCloudwatchMetrics user configurable settings
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalElasticsearchLogsUserConfigArgs']] external_elasticsearch_logs_user_config: ExternalElasticsearchLogs user configurable settings
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalGoogleCloudLoggingUserConfigArgs']] external_google_cloud_logging_user_config: ExternalGoogleCloudLogging user configurable settings
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalKafkaUserConfigArgs']] external_kafka_user_config: ExternalKafka user configurable settings
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalOpensearchLogsUserConfigArgs']] external_opensearch_logs_user_config: ExternalOpensearchLogs user configurable settings
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalSchemaRegistryUserConfigArgs']] external_schema_registry_user_config: ExternalSchemaRegistry user configurable settings
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointJolokiaUserConfigArgs']] jolokia_user_config: Jolokia user configurable settings
         :param pulumi.Input[str] project: Project the service integration endpoint belongs to
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointPrometheusUserConfigArgs']] prometheus_user_config: Prometheus user configurable settings
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointRsyslogUserConfigArgs']] rsyslog_user_config: Rsyslog user configurable settings
-        :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointSignalfxUserConfigArgs']] signalfx_user_config: Signalfx user configurable settings
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ServiceIntegrationEndpointState.__new__(_ServiceIntegrationEndpointState)
 
         __props__.__dict__["datadog_user_config"] = datadog_user_config
         __props__.__dict__["endpoint_config"] = endpoint_config
@@ -699,15 +661,14 @@
         __props__.__dict__["external_kafka_user_config"] = external_kafka_user_config
         __props__.__dict__["external_opensearch_logs_user_config"] = external_opensearch_logs_user_config
         __props__.__dict__["external_schema_registry_user_config"] = external_schema_registry_user_config
         __props__.__dict__["jolokia_user_config"] = jolokia_user_config
         __props__.__dict__["project"] = project
         __props__.__dict__["prometheus_user_config"] = prometheus_user_config
         __props__.__dict__["rsyslog_user_config"] = rsyslog_user_config
-        __props__.__dict__["signalfx_user_config"] = signalfx_user_config
         return ServiceIntegrationEndpoint(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="datadogUserConfig")
     def datadog_user_config(self) -> pulumi.Output[Optional['outputs.ServiceIntegrationEndpointDatadogUserConfig']]:
         """
         Datadog user configurable settings
@@ -730,15 +691,15 @@
         """
         return pulumi.get(self, "endpoint_name")
 
     @property
     @pulumi.getter(name="endpointType")
     def endpoint_type(self) -> pulumi.Output[str]:
         """
-        Type of the service integration endpoint
+        Type of the service integration endpoint. Possible values: `datadog`, `prometheus`, `rsyslog`, `external_elasticsearch_logs`, `external_opensearch_logs`, `external_aws_cloudwatch_logs`, `external_google_cloud_logging`, `external_kafka`, `jolokia`, `external_schema_registry`, `external_aws_cloudwatch_metrics`
         """
         return pulumi.get(self, "endpoint_type")
 
     @property
     @pulumi.getter(name="externalAwsCloudwatchLogsUserConfig")
     def external_aws_cloudwatch_logs_user_config(self) -> pulumi.Output[Optional['outputs.ServiceIntegrationEndpointExternalAwsCloudwatchLogsUserConfig']]:
         """
@@ -822,15 +783,7 @@
     @pulumi.getter(name="rsyslogUserConfig")
     def rsyslog_user_config(self) -> pulumi.Output[Optional['outputs.ServiceIntegrationEndpointRsyslogUserConfig']]:
         """
         Rsyslog user configurable settings
         """
         return pulumi.get(self, "rsyslog_user_config")
 
-    @property
-    @pulumi.getter(name="signalfxUserConfig")
-    def signalfx_user_config(self) -> pulumi.Output[Optional['outputs.ServiceIntegrationEndpointSignalfxUserConfig']]:
-        """
-        Signalfx user configurable settings
-        """
-        return pulumi.get(self, "signalfx_user_config")
-
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/static_ip.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/static_ip.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven/transit_gateway_vpc_attachment.py` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven/transit_gateway_vpc_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven.egg-info/PKG-INFO` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-aiven
-Version: 6.2.0a1684187488
+Version: 6.2.0a1684191618
 Summary: A Pulumi package for creating and managing Aiven cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-aiven
 Keywords: pulumi aiven
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_aiven-6.2.0a1684187488/pulumi_aiven.egg-info/SOURCES.txt` & `pulumi_aiven-6.2.0a1684191618/pulumi_aiven.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.2.0a1684187488/setup.py` & `pulumi_aiven-6.2.0a1684191618/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "6.2.0a1684187488"
-PLUGIN_VERSION = "6.2.0-alpha.1684187488+cd871e36"
+VERSION = "6.2.0a1684191618"
+PLUGIN_VERSION = "6.2.0-alpha.1684191618+d324a45d"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'aiven', PLUGIN_VERSION])
         except OSError as error:
```

