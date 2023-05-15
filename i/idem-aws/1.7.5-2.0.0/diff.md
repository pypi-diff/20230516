# Comparing `tmp/idem-aws-1.7.5.tar.gz` & `tmp/idem-aws-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idem-aws-1.7.5.tar", last modified: Fri May  5 18:38:41 2023, max compression
+gzip compressed data, was "idem-aws-2.0.0.tar", last modified: Mon May 15 22:32:09 2023, max compression
```

## Comparing `idem-aws-1.7.5.tar` & `idem-aws-2.0.0.tar`

### file list

```diff
@@ -1,696 +1,696 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.895220 idem-aws-1.7.5/
--rw-r--r--   0 root         (0) root         (0)    11342 2023-05-05 18:38:25.000000 idem-aws-1.7.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       54 2023-05-05 18:38:25.000000 idem-aws-1.7.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    11051 2023-05-05 18:38:41.895220 idem-aws-1.7.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9835 2023-05-05 18:38:25.000000 idem-aws-1.7.5/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.839216 idem-aws-1.7.5/idem_aws/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.829215 idem-aws-1.7.5/idem_aws/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.840216 idem-aws-1.7.5/idem_aws/acct/aws/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.840216 idem-aws-1.7.5/idem_aws/acct/aws/contracts/
--rw-r--r--   0 root         (0) root         (0)     1127 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/acct/aws/contracts/init.py
--rw-r--r--   0 root         (0) root         (0)     5506 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/acct/aws/gsuite.py
--rw-r--r--   0 root         (0) root         (0)     1618 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/acct/aws/iam.py
--rw-r--r--   0 root         (0) root         (0)     2213 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/acct/aws/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.840216 idem-aws-1.7.5/idem_aws/acct/metadata/
--rw-r--r--   0 root         (0) root         (0)      534 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/acct/metadata/aws.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.829215 idem-aws-1.7.5/idem_aws/autogen/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.840216 idem-aws-1.7.5/idem_aws/autogen/aws/
--rw-r--r--   0 root         (0) root         (0)     7082 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/autogen/aws/function.py
--rw-r--r--   0 root         (0) root         (0)     9947 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/autogen/aws/init.py
--rw-r--r--   0 root         (0) root         (0)     3023 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/autogen/aws/param.py
--rw-r--r--   0 root         (0) root         (0)     4731 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/autogen/aws/plugin.py
--rw-r--r--   0 root         (0) root         (0)      677 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/autogen/aws/possible_functions.py
--rw-r--r--   0 root         (0) root         (0)     3870 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/autogen/aws/resource.py
--rw-r--r--   0 root         (0) root         (0)     4045 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/autogen/aws/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.841216 idem-aws-1.7.5/idem_aws/autogen/aws/tag/
--rw-r--r--   0 root         (0) root         (0)     3401 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/autogen/aws/tag/plugin.py
--rw-r--r--   0 root         (0) root         (0)     4865 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/autogen/aws/tag/template.py
--rw-r--r--   0 root         (0) root         (0)    15883 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/autogen/aws/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.841216 idem-aws-1.7.5/idem_aws/autogen/aws/utils/
--rw-r--r--   0 root         (0) root         (0)     1361 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/autogen/aws/utils/plugin.py
--rw-r--r--   0 root         (0) root         (0)     1669 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/autogen/aws/utils/template.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.841216 idem-aws-1.7.5/idem_aws/esm/
--rw-r--r--   0 root         (0) root         (0)     8692 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/esm/aws.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.841216 idem-aws-1.7.5/idem_aws/esm/contracts/
--rw-r--r--   0 root         (0) root         (0)     1063 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/esm/contracts/aws.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.832215 idem-aws-1.7.5/idem_aws/exec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.841216 idem-aws-1.7.5/idem_aws/exec/aws/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.841216 idem-aws-1.7.5/idem_aws/exec/aws/acm/
--rw-r--r--   0 root         (0) root         (0)     2000 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/acm/certificate_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.842216 idem-aws-1.7.5/idem_aws/exec/aws/apigateway/
--rw-r--r--   0 root         (0) root         (0)     5430 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/apigateway/base_path_mapping.py
--rw-r--r--   0 root         (0) root         (0)     2600 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/apigateway/deployment.py
--rw-r--r--   0 root         (0) root         (0)     3322 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/apigateway/domain_name.py
--rw-r--r--   0 root         (0) root         (0)     1925 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/apigateway/integration.py
--rw-r--r--   0 root         (0) root         (0)     2971 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/apigateway/integration_response.py
--rw-r--r--   0 root         (0) root         (0)     1766 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/apigateway/method.py
--rw-r--r--   0 root         (0) root         (0)     2145 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/apigateway/method_response.py
--rw-r--r--   0 root         (0) root         (0)     1136 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/apigateway/resource.py
--rw-r--r--   0 root         (0) root         (0)     2435 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/apigateway/rest_api.py
--rw-r--r--   0 root         (0) root         (0)     2608 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/apigateway/stage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.843216 idem-aws-1.7.5/idem_aws/exec/aws/apigatewayv2/
--rw-r--r--   0 root         (0) root         (0)     3276 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/apigatewayv2/api.py
--rw-r--r--   0 root         (0) root         (0)     2069 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/apigatewayv2/authorizer.py
--rw-r--r--   0 root         (0) root         (0)     1890 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/apigatewayv2/domain_name.py
--rw-r--r--   0 root         (0) root         (0)     2184 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/apigatewayv2/integration.py
--rw-r--r--   0 root         (0) root         (0)     3761 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/apigatewayv2/route.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.843216 idem-aws-1.7.5/idem_aws/exec/aws/application_autoscaling/
--rw-r--r--   0 root         (0) root         (0)     3192 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/application_autoscaling/scalable_target.py
--rw-r--r--   0 root         (0) root         (0)     3395 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/application_autoscaling/scaling_policy.py
--rw-r--r--   0 root         (0) root         (0)     2846 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/arn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.843216 idem-aws-1.7.5/idem_aws/exec/aws/autoscaling/
--rw-r--r--   0 root         (0) root         (0)     3034 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/autoscaling/scaling_policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.843216 idem-aws-1.7.5/idem_aws/exec/aws/backup/
--rw-r--r--   0 root         (0) root         (0)     4661 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/backup/backup_vault.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.843216 idem-aws-1.7.5/idem_aws/exec/aws/budgets/
--rw-r--r--   0 root         (0) root         (0)     4105 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/budgets/budget.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.843216 idem-aws-1.7.5/idem_aws/exec/aws/cloudformation/
--rw-r--r--   0 root         (0) root         (0)     2285 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/cloudformation/stack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.844216 idem-aws-1.7.5/idem_aws/exec/aws/cloudfront/
--rw-r--r--   0 root         (0) root         (0)     4007 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/cloudfront/cache_policy.py
--rw-r--r--   0 root         (0) root         (0)     2697 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/cloudfront/distribution.py
--rw-r--r--   0 root         (0) root         (0)     4297 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/cloudfront/origin_request_policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.844216 idem-aws-1.7.5/idem_aws/exec/aws/cloudwatch/
--rw-r--r--   0 root         (0) root         (0)     3012 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/cloudwatch/log_group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.844216 idem-aws-1.7.5/idem_aws/exec/aws/cloudwatchlogs/
--rw-r--r--   0 root         (0) root         (0)     1528 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/cloudwatchlogs/resource_policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.844216 idem-aws-1.7.5/idem_aws/exec/aws/config/
--rw-r--r--   0 root         (0) root         (0)     4538 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/config/configuration_aggregator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.844216 idem-aws-1.7.5/idem_aws/exec/aws/costexplorer/
--rw-r--r--   0 root         (0) root         (0)     1660 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/costexplorer/cost_allocation_tag.py
--rw-r--r--   0 root         (0) root         (0)     1033 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.844216 idem-aws-1.7.5/idem_aws/exec/aws/docdb/
--rw-r--r--   0 root         (0) root         (0)     6138 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/docdb/db_cluster.py
--rw-r--r--   0 root         (0) root         (0)     7293 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/docdb/db_cluster_parameter_group.py
--rw-r--r--   0 root         (0) root         (0)     4887 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/docdb/db_subnet_group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.844216 idem-aws-1.7.5/idem_aws/exec/aws/dynamodb/
--rw-r--r--   0 root         (0) root         (0)     2434 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/dynamodb/table.py
--rw-r--r--   0 root         (0) root         (0)     2318 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/dynamodb/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.847216 idem-aws-1.7.5/idem_aws/exec/aws/ec2/
--rw-r--r--   0 root         (0) root         (0)     8697 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/ami.py
--rw-r--r--   0 root         (0) root         (0)     4290 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/availability_zones.py
--rw-r--r--   0 root         (0) root         (0)     4206 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/elastic_ip.py
--rw-r--r--   0 root         (0) root         (0)     3405 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/flow_log.py
--rw-r--r--   0 root         (0) root         (0)    22002 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/instance.py
--rw-r--r--   0 root         (0) root         (0)     3299 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/instance_type.py
--rw-r--r--   0 root         (0) root         (0)     1511 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/internet_gateway.py
--rw-r--r--   0 root         (0) root         (0)     2216 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/key_pair.py
--rw-r--r--   0 root         (0) root         (0)     7293 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/launch_template.py
--rw-r--r--   0 root         (0) root         (0)     8395 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/network_interface.py
--rw-r--r--   0 root         (0) root         (0)     4680 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/placement_group.py
--rw-r--r--   0 root         (0) root         (0)     5836 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/route.py
--rw-r--r--   0 root         (0) root         (0)     3579 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/route_table.py
--rw-r--r--   0 root         (0) root         (0)     3265 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/route_table_association.py
--rw-r--r--   0 root         (0) root         (0)     5108 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/security_group.py
--rw-r--r--   0 root         (0) root         (0)     4143 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/security_group_rule.py
--rw-r--r--   0 root         (0) root         (0)     4810 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/snapshot.py
--rw-r--r--   0 root         (0) root         (0)     4295 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/spot_instance_request.py
--rw-r--r--   0 root         (0) root         (0)     8595 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/subnet.py
--rw-r--r--   0 root         (0) root         (0)     4471 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/volume.py
--rw-r--r--   0 root         (0) root         (0)     4459 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/vpc.py
--rw-r--r--   0 root         (0) root         (0)     4081 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/vpc_endpoint.py
--rw-r--r--   0 root         (0) root         (0)     1952 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/vpc_peering_connection.py
--rw-r--r--   0 root         (0) root         (0)     2007 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/vpc_peering_connection_accepter.py
--rw-r--r--   0 root         (0) root         (0)     2048 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/vpc_peering_connection_options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.847216 idem-aws-1.7.5/idem_aws/exec/aws/ecr/
--rw-r--r--   0 root         (0) root         (0)     5183 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ecr/image.py
--rw-r--r--   0 root         (0) root         (0)     3195 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ecr/lifecycle_policy.py
--rw-r--r--   0 root         (0) root         (0)     5504 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ecr/repository.py
--rw-r--r--   0 root         (0) root         (0)     2750 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ecr/repository_policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.847216 idem-aws-1.7.5/idem_aws/exec/aws/eks/
--rw-r--r--   0 root         (0) root         (0)     1665 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/eks/cluster.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.848216 idem-aws-1.7.5/idem_aws/exec/aws/elasticache/
--rw-r--r--   0 root         (0) root         (0)     2934 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/elasticache/replication_group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.848216 idem-aws-1.7.5/idem_aws/exec/aws/elb/
--rw-r--r--   0 root         (0) root         (0)     3023 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/elb/elb_hosted_zone_id.py
--rw-r--r--   0 root         (0) root         (0)     3363 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/elb/load_balancer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.848216 idem-aws-1.7.5/idem_aws/exec/aws/elbv2/
--rw-r--r--   0 root         (0) root         (0)     3296 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/elbv2/listener.py
--rw-r--r--   0 root         (0) root         (0)     3346 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/elbv2/load_balancer.py
--rw-r--r--   0 root         (0) root         (0)     4861 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/elbv2/target_group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.848216 idem-aws-1.7.5/idem_aws/exec/aws/es/
--rw-r--r--   0 root         (0) root         (0)     2387 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/es/elasticsearch_domain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.848216 idem-aws-1.7.5/idem_aws/exec/aws/events/
--rw-r--r--   0 root         (0) root         (0)     5682 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/events/rule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.849216 idem-aws-1.7.5/idem_aws/exec/aws/guardduty/
--rw-r--r--   0 root         (0) root         (0)     2423 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/guardduty/detector.py
--rw-r--r--   0 root         (0) root         (0)     5618 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/guardduty/member.py
--rw-r--r--   0 root         (0) root         (0)     1814 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/guardduty/organization_admin_account.py
--rw-r--r--   0 root         (0) root         (0)     8637 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/guardduty/organization_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.850216 idem-aws-1.7.5/idem_aws/exec/aws/iam/
--rw-r--r--   0 root         (0) root         (0)     9324 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/iam/access_key.py
--rw-r--r--   0 root         (0) root         (0)     1128 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/iam/group.py
--rw-r--r--   0 root         (0) root         (0)     1199 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/iam/group_membership.py
--rw-r--r--   0 root         (0) root         (0)     2099 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/iam/group_policy_attachment.py
--rw-r--r--   0 root         (0) root         (0)     4749 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/iam/instance_profile.py
--rw-r--r--   0 root         (0) root         (0)     7709 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/iam/open_id_connect_provider.py
--rw-r--r--   0 root         (0) root         (0)     1842 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/iam/password_policy.py
--rw-r--r--   0 root         (0) root         (0)     6957 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/iam/policy.py
--rw-r--r--   0 root         (0) root         (0)     9723 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/iam/role.py
--rw-r--r--   0 root         (0) root         (0)     1218 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/iam/user.py
--rw-r--r--   0 root         (0) root         (0)     2945 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/iam/user_policy_attachment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.850216 idem-aws-1.7.5/idem_aws/exec/aws/kinesis/
--rw-r--r--   0 root         (0) root         (0)     2919 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/kinesis/stream.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.850216 idem-aws-1.7.5/idem_aws/exec/aws/kms/
--rw-r--r--   0 root         (0) root         (0)     3031 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/kms/key.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.850216 idem-aws-1.7.5/idem_aws/exec/aws/lambda_aws/
--rw-r--r--   0 root         (0) root         (0)     4863 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/lambda_aws/function_event_invoke_config.py
--rw-r--r--   0 root         (0) root         (0)     5632 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/lambda_aws/function_provisioned_concurrency_config.py
--rw-r--r--   0 root         (0) root         (0)       27 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/lambda_aws/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.850216 idem-aws-1.7.5/idem_aws/exec/aws/neptune/
--rw-r--r--   0 root         (0) root         (0)     7388 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/neptune/db_cluster_parameter_group.py
--rw-r--r--   0 root         (0) root         (0)     6621 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/neptune/db_instance.py
--rw-r--r--   0 root         (0) root         (0)     6854 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/neptune/db_parameter_group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.851216 idem-aws-1.7.5/idem_aws/exec/aws/organizations/
--rw-r--r--   0 root         (0) root         (0)     4486 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/organizations/account.py
--rw-r--r--   0 root         (0) root         (0)     2391 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/organizations/policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.851216 idem-aws-1.7.5/idem_aws/exec/aws/rds/
--rw-r--r--   0 root         (0) root         (0)     5996 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/rds/db_cluster.py
--rw-r--r--   0 root         (0) root         (0)     5001 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/rds/db_cluster_parameter_group.py
--rw-r--r--   0 root         (0) root         (0)     5971 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/rds/db_instance.py
--rw-r--r--   0 root         (0) root         (0)     6287 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/rds/db_parameter_group.py
--rw-r--r--   0 root         (0) root         (0)     4835 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/rds/db_subnet_group.py
--rw-r--r--   0 root         (0) root         (0)     2686 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/rds/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.851216 idem-aws-1.7.5/idem_aws/exec/aws/route53/
--rw-r--r--   0 root         (0) root         (0)     5251 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/route53/hosted_zone.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.852217 idem-aws-1.7.5/idem_aws/exec/aws/s3/
--rw-r--r--   0 root         (0) root         (0)     2659 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/s3/bucket.py
--rw-r--r--   0 root         (0) root         (0)     1518 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/s3/bucket_acl.py
--rw-r--r--   0 root         (0) root         (0)     1918 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/s3/bucket_lifecycle.py
--rw-r--r--   0 root         (0) root         (0)     1897 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/s3/bucket_logging.py
--rw-r--r--   0 root         (0) root         (0)     1982 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/s3/bucket_replication.py
--rw-r--r--   0 root         (0) root         (0)     1956 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/s3/bucket_website.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.852217 idem-aws-1.7.5/idem_aws/exec/aws/ses/
--rw-r--r--   0 root         (0) root         (0)     3203 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ses/domain_identity.py
--rw-r--r--   0 root         (0) root         (0)     4167 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ses/identity_notification_topic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.852217 idem-aws-1.7.5/idem_aws/exec/aws/sesv2/
--rw-r--r--   0 root         (0) root         (0)     4342 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/sesv2/event_destination.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.852217 idem-aws-1.7.5/idem_aws/exec/aws/sns/
--rw-r--r--   0 root         (0) root         (0)     3682 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/sns/subscription.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.852217 idem-aws-1.7.5/idem_aws/exec/aws/sqs/
--rw-r--r--   0 root         (0) root         (0)     4686 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/sqs/queue.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.852217 idem-aws-1.7.5/idem_aws/exec/aws/sts/
--rw-r--r--   0 root         (0) root         (0)     5261 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/sts/assume_role.py
--rw-r--r--   0 root         (0) root         (0)     1259 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/sts/caller_identity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.853217 idem-aws-1.7.5/idem_aws/exec/aws/wafv2/
--rw-r--r--   0 root         (0) root         (0)     4859 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/wafv2/ip_set.py
--rw-r--r--   0 root         (0) root         (0)     7041 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/wafv2/regex_pattern_set.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.853217 idem-aws-1.7.5/idem_aws/exec/boto3/
--rw-r--r--   0 root         (0) root         (0)      747 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/boto3/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.832215 idem-aws-1.7.5/idem_aws/reconcile/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.853217 idem-aws-1.7.5/idem_aws/reconcile/pending/
--rw-r--r--   0 root         (0) root         (0)     1004 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/reconcile/pending/aws.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.832215 idem-aws-1.7.5/idem_aws/states/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.853217 idem-aws-1.7.5/idem_aws/states/aws/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.853217 idem-aws-1.7.5/idem_aws/states/aws/acm/
--rw-r--r--   0 root         (0) root         (0)    28336 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/acm/certificate_manager.py
--rw-r--r--   0 root         (0) root         (0)    11133 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/acm/certificate_validation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.854217 idem-aws-1.7.5/idem_aws/states/aws/apigateway/
--rw-r--r--   0 root         (0) root         (0)    10257 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/apigateway/base_path_mapping.py
--rw-r--r--   0 root         (0) root         (0)    12091 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/apigateway/deployment.py
--rw-r--r--   0 root         (0) root         (0)    19520 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/apigateway/domain_name.py
--rw-r--r--   0 root         (0) root         (0)    15779 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/apigateway/integration.py
--rw-r--r--   0 root         (0) root         (0)    13752 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/apigateway/integration_response.py
--rw-r--r--   0 root         (0) root         (0)    12951 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/apigateway/method.py
--rw-r--r--   0 root         (0) root         (0)    12155 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/apigateway/method_response.py
--rw-r--r--   0 root         (0) root         (0)     9866 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/apigateway/resource.py
--rw-r--r--   0 root         (0) root         (0)    13732 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/apigateway/rest_api.py
--rw-r--r--   0 root         (0) root         (0)    13857 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/apigateway/stage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.855217 idem-aws-1.7.5/idem_aws/states/aws/apigatewayv2/
--rw-r--r--   0 root         (0) root         (0)    15354 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/apigatewayv2/api.py
--rw-r--r--   0 root         (0) root         (0)    16244 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/apigatewayv2/authorizer.py
--rw-r--r--   0 root         (0) root         (0)    15119 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/apigatewayv2/domain_name.py
--rw-r--r--   0 root         (0) root         (0)    22693 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/apigatewayv2/integration.py
--rw-r--r--   0 root         (0) root         (0)    14022 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/apigatewayv2/route.py
--rw-r--r--   0 root         (0) root         (0)    16913 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/apigatewayv2/stage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.855217 idem-aws-1.7.5/idem_aws/states/aws/application_autoscaling/
--rw-r--r--   0 root         (0) root         (0)    31855 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/application_autoscaling/scalable_target.py
--rw-r--r--   0 root         (0) root         (0)    45934 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/application_autoscaling/scaling_policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.856217 idem-aws-1.7.5/idem_aws/states/aws/autoscaling/
--rw-r--r--   0 root         (0) root         (0)    78777 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/autoscaling/auto_scaling_group.py
--rw-r--r--   0 root         (0) root         (0)    32523 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/autoscaling/launch_configuration.py
--rw-r--r--   0 root         (0) root         (0)    54968 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/autoscaling/scaling_policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.856217 idem-aws-1.7.5/idem_aws/states/aws/backup/
--rw-r--r--   0 root         (0) root         (0)     8985 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/backup/backup_vault.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.856217 idem-aws-1.7.5/idem_aws/states/aws/budgets/
--rw-r--r--   0 root         (0) root         (0)    25523 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/budgets/budget.py
--rw-r--r--   0 root         (0) root         (0)    16456 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/budgets/budget_action.py
--rw-r--r--   0 root         (0) root         (0)     1768 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/caller_identity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.856217 idem-aws-1.7.5/idem_aws/states/aws/cloudformation/
--rw-r--r--   0 root         (0) root         (0)    32414 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/cloudformation/stack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.857217 idem-aws-1.7.5/idem_aws/states/aws/cloudfront/
--rw-r--r--   0 root         (0) root         (0)    24459 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/cloudfront/cache_policy.py
--rw-r--r--   0 root         (0) root         (0)   116104 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/cloudfront/distribution.py
--rw-r--r--   0 root         (0) root         (0)    15501 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/cloudfront/origin_request_policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.857217 idem-aws-1.7.5/idem_aws/states/aws/cloudtrail/
--rw-r--r--   0 root         (0) root         (0)    37423 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/cloudtrail/trail.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.857217 idem-aws-1.7.5/idem_aws/states/aws/cloudwatch/
--rw-r--r--   0 root         (0) root         (0)    11420 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/cloudwatch/log_group.py
--rw-r--r--   0 root         (0) root         (0)    36077 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/cloudwatch/metric_alarm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.857217 idem-aws-1.7.5/idem_aws/states/aws/cloudwatchlogs/
--rw-r--r--   0 root         (0) root         (0)     8723 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/cloudwatchlogs/resource_policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.858217 idem-aws-1.7.5/idem_aws/states/aws/config/
--rwxr-xr-x   0 root         (0) root         (0)    11422 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/config/config_recorder.py
--rwxr-xr-x   0 root         (0) root         (0)     9512 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/config/config_recorder_status.py
--rw-r--r--   0 root         (0) root         (0)    10463 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/config/configuration_aggregator.py
--rwxr-xr-x   0 root         (0) root         (0)    12062 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/config/delivery_channel.py
--rw-r--r--   0 root         (0) root         (0)    21665 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/config/rule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.858217 idem-aws-1.7.5/idem_aws/states/aws/costexplorer/
--rw-r--r--   0 root         (0) root         (0)    18654 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/costexplorer/anomaly_monitor.py
--rw-r--r--   0 root         (0) root         (0)    10751 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/costexplorer/anomaly_subscription.py
--rw-r--r--   0 root         (0) root         (0)    28397 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/costexplorer/cost_category.py
--rw-r--r--   0 root         (0) root         (0)     1026 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.858217 idem-aws-1.7.5/idem_aws/states/aws/docdb/
--rw-r--r--   0 root         (0) root         (0)    28355 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/docdb/db_cluster.py
--rw-r--r--   0 root         (0) root         (0)    12967 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/docdb/db_cluster_parameter_group.py
--rw-r--r--   0 root         (0) root         (0)    11755 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/docdb/db_subnet_group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.859217 idem-aws-1.7.5/idem_aws/states/aws/dynamodb/
--rw-r--r--   0 root         (0) root         (0)    36228 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/dynamodb/table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.862217 idem-aws-1.7.5/idem_aws/states/aws/ec2/
--rw-r--r--   0 root         (0) root         (0)    22039 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/ami.py
--rw-r--r--   0 root         (0) root         (0)    15794 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/dhcp_option.py
--rw-r--r--   0 root         (0) root         (0)    10017 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/dhcp_option_association.py
--rw-r--r--   0 root         (0) root         (0)    13002 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/elastic_ip.py
--rw-r--r--   0 root         (0) root         (0)    12633 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/flow_log.py
--rw-r--r--   0 root         (0) root         (0)    40732 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/instance.py
--rw-r--r--   0 root         (0) root         (0)    12429 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/internet_gateway.py
--rw-r--r--   0 root         (0) root         (0)     9711 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/key_pair.py
--rw-r--r--   0 root         (0) root         (0)    73136 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/launch_template.py
--rw-r--r--   0 root         (0) root         (0)    17418 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/nat_gateway.py
--rw-r--r--   0 root         (0) root         (0)    12093 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/network_interface.py
--rw-r--r--   0 root         (0) root         (0)    10946 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/placement_group.py
--rw-r--r--   0 root         (0) root         (0)    14835 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/route.py
--rw-r--r--   0 root         (0) root         (0)    15623 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/route_table.py
--rw-r--r--   0 root         (0) root         (0)     8933 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/route_table_association.py
--rw-r--r--   0 root         (0) root         (0)    12947 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/security_group.py
--rw-r--r--   0 root         (0) root         (0)    17979 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/security_group_rule.py
--rw-r--r--   0 root         (0) root         (0)    10513 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/snapshot.py
--rw-r--r--   0 root         (0) root         (0)    36976 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/spot_instance_request.py
--rw-r--r--   0 root         (0) root         (0)    20046 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/subnet.py
--rw-r--r--   0 root         (0) root         (0)    17765 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/transit_gateway.py
--rw-r--r--   0 root         (0) root         (0)    16953 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/transit_gateway_vpc_attachment.py
--rw-r--r--   0 root         (0) root         (0)    15331 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/volume.py
--rw-r--r--   0 root         (0) root         (0)    20607 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/vpc.py
--rw-r--r--   0 root         (0) root         (0)    19294 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/vpc_endpoint.py
--rw-r--r--   0 root         (0) root         (0)    14516 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/vpc_peering_connection.py
--rw-r--r--   0 root         (0) root         (0)     9225 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/vpc_peering_connection_accepter.py
--rw-r--r--   0 root         (0) root         (0)     9871 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/vpc_peering_connection_options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.862217 idem-aws-1.7.5/idem_aws/states/aws/ecr/
--rw-r--r--   0 root         (0) root         (0)    11586 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ecr/lifecycle_policy.py
--rw-r--r--   0 root         (0) root         (0)    13319 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ecr/repository.py
--rw-r--r--   0 root         (0) root         (0)    11707 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ecr/repository_policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.863217 idem-aws-1.7.5/idem_aws/states/aws/efs/
--rw-r--r--   0 root         (0) root         (0)    25301 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/efs/file_system.py
--rw-r--r--   0 root         (0) root         (0)    22090 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/efs/mount_target.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.863217 idem-aws-1.7.5/idem_aws/states/aws/eks/
--rw-r--r--   0 root         (0) root         (0)    18084 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/eks/addon.py
--rw-r--r--   0 root         (0) root         (0)    29585 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/eks/cluster.py
--rw-r--r--   0 root         (0) root         (0)    17678 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/eks/fargate_profile.py
--rw-r--r--   0 root         (0) root         (0)    29787 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/eks/nodegroup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.863217 idem-aws-1.7.5/idem_aws/states/aws/elasticache/
--rw-r--r--   0 root         (0) root         (0)    16170 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/elasticache/cache_parameter_group.py
--rw-r--r--   0 root         (0) root         (0)    13492 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/elasticache/cache_subnet_group.py
--rw-r--r--   0 root         (0) root         (0)    51005 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/elasticache/replication_group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.864217 idem-aws-1.7.5/idem_aws/states/aws/elb/
--rw-r--r--   0 root         (0) root         (0)    19828 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/elb/load_balancer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.864217 idem-aws-1.7.5/idem_aws/states/aws/elbv2/
--rw-r--r--   0 root         (0) root         (0)    32920 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/elbv2/listener.py
--rw-r--r--   0 root         (0) root         (0)    24159 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/elbv2/load_balancer.py
--rw-r--r--   0 root         (0) root         (0)    30475 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/elbv2/target_group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.864217 idem-aws-1.7.5/idem_aws/states/aws/es/
--rw-r--r--   0 root         (0) root         (0)    36336 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/es/elasticsearch_domain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.864217 idem-aws-1.7.5/idem_aws/states/aws/events/
--rw-r--r--   0 root         (0) root         (0)    45263 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/events/rule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.865218 idem-aws-1.7.5/idem_aws/states/aws/guardduty/
--rw-r--r--   0 root         (0) root         (0)    15458 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/guardduty/detector.py
--rw-r--r--   0 root         (0) root         (0)    10351 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/guardduty/member.py
--rw-r--r--   0 root         (0) root         (0)     8768 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/guardduty/organization_admin_account.py
--rw-r--r--   0 root         (0) root         (0)     8981 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/guardduty/organization_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.866218 idem-aws-1.7.5/idem_aws/states/aws/iam/
--rw-r--r--   0 root         (0) root         (0)     9988 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/iam/access_key.py
--rw-r--r--   0 root         (0) root         (0)     8246 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/iam/group.py
--rw-r--r--   0 root         (0) root         (0)     8179 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/iam/group_membership.py
--rw-r--r--   0 root         (0) root         (0)     8776 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/iam/group_policy_attachment.py
--rw-r--r--   0 root         (0) root         (0)    14496 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/iam/instance_profile.py
--rw-r--r--   0 root         (0) root         (0)    18389 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/iam/open_id_connect_provider.py
--rw-r--r--   0 root         (0) root         (0)    12320 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/iam/password_policy.py
--rw-r--r--   0 root         (0) root         (0)    14613 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/iam/policy.py
--rw-r--r--   0 root         (0) root         (0)    22432 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/iam/role.py
--rw-r--r--   0 root         (0) root         (0)    14538 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/iam/role_policy.py
--rw-r--r--   0 root         (0) root         (0)    10537 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/iam/role_policy_attachment.py
--rw-r--r--   0 root         (0) root         (0)    15633 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/iam/service_linked_role.py
--rw-r--r--   0 root         (0) root         (0)    15522 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/iam/user.py
--rw-r--r--   0 root         (0) root         (0)    14080 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/iam/user_policy.py
--rw-r--r--   0 root         (0) root         (0)    11044 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/iam/user_policy_attachment.py
--rw-r--r--   0 root         (0) root         (0)    13341 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/iam/user_ssh_key.py
--rw-r--r--   0 root         (0) root         (0)      169 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.866218 idem-aws-1.7.5/idem_aws/states/aws/kinesis/
--rw-r--r--   0 root         (0) root         (0)    24114 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/kinesis/stream.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.867218 idem-aws-1.7.5/idem_aws/states/aws/kms/
--rw-r--r--   0 root         (0) root         (0)    10460 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/kms/alias.py
--rw-r--r--   0 root         (0) root         (0)    22629 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/kms/key.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.867218 idem-aws-1.7.5/idem_aws/states/aws/lambda_aws/
--rw-r--r--   0 root         (0) root         (0)    27963 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/lambda_aws/function.py
--rw-r--r--   0 root         (0) root         (0)    11651 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/lambda_aws/function_event_invoke_config.py
--rw-r--r--   0 root         (0) root         (0)    14029 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/lambda_aws/function_permission.py
--rw-r--r--   0 root         (0) root         (0)    10018 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/lambda_aws/function_provisioned_concurrency_config.py
--rw-r--r--   0 root         (0) root         (0)       27 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/lambda_aws/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.867218 idem-aws-1.7.5/idem_aws/states/aws/logs/
--rw-r--r--   0 root         (0) root         (0)    12064 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/logs/subscription_filter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.868218 idem-aws-1.7.5/idem_aws/states/aws/neptune/
--rw-r--r--   0 root         (0) root         (0)    32988 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/neptune/db_cluster.py
--rw-r--r--   0 root         (0) root         (0)    13936 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/neptune/db_cluster_parameter_group.py
--rw-r--r--   0 root         (0) root         (0)    37556 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/neptune/db_instance.py
--rw-r--r--   0 root         (0) root         (0)    12467 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/neptune/db_parameter_group.py
--rw-r--r--   0 root         (0) root         (0)    14288 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/neptune/db_subnet_group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.868218 idem-aws-1.7.5/idem_aws/states/aws/organizations/
--rw-r--r--   0 root         (0) root         (0)    17382 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/organizations/account.py
--rw-r--r--   0 root         (0) root         (0)     8251 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/organizations/organization.py
--rw-r--r--   0 root         (0) root         (0)    14288 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/organizations/organization_unit.py
--rw-r--r--   0 root         (0) root         (0)    13661 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/organizations/policy.py
--rw-r--r--   0 root         (0) root         (0)    11399 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/organizations/policy_attachment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.869218 idem-aws-1.7.5/idem_aws/states/aws/rds/
--rw-r--r--   0 root         (0) root         (0)    62077 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/rds/db_cluster.py
--rw-r--r--   0 root         (0) root         (0)    14695 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/rds/db_cluster_parameter_group.py
--rw-r--r--   0 root         (0) root         (0)    39434 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/rds/db_instance.py
--rw-r--r--   0 root         (0) root         (0)    13874 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/rds/db_parameter_group.py
--rw-r--r--   0 root         (0) root         (0)    14036 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/rds/db_subnet_group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.869218 idem-aws-1.7.5/idem_aws/states/aws/recursive_contracts/
--rw-r--r--   0 root         (0) root         (0)       98 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/recursive_contracts/allow_sync_sls_name_and_name_tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.870218 idem-aws-1.7.5/idem_aws/states/aws/route53/
--rw-r--r--   0 root         (0) root         (0)    19436 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/route53/hosted_zone.py
--rw-r--r--   0 root         (0) root         (0)    14158 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/route53/hosted_zone_association.py
--rw-r--r--   0 root         (0) root         (0)    12020 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/route53/resource_record.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.871218 idem-aws-1.7.5/idem_aws/states/aws/s3/
--rw-r--r--   0 root         (0) root         (0)    19835 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/s3/bucket.py
--rw-r--r--   0 root         (0) root         (0)    11122 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/s3/bucket_acl.py
--rw-r--r--   0 root         (0) root         (0)    12547 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/s3/bucket_encryption.py
--rw-r--r--   0 root         (0) root         (0)    26660 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/s3/bucket_lifecycle.py
--rw-r--r--   0 root         (0) root         (0)    14837 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/s3/bucket_logging.py
--rw-r--r--   0 root         (0) root         (0)    17615 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/s3/bucket_notification.py
--rw-r--r--   0 root         (0) root         (0)    11956 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/s3/bucket_policy.py
--rw-r--r--   0 root         (0) root         (0)    27930 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/s3/bucket_replication.py
--rw-r--r--   0 root         (0) root         (0)    10328 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/s3/bucket_versioning.py
--rw-r--r--   0 root         (0) root         (0)    22433 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/s3/bucket_website.py
--rw-r--r--   0 root         (0) root         (0)    12854 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/s3/public_access_block.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.871218 idem-aws-1.7.5/idem_aws/states/aws/ses/
--rw-r--r--   0 root         (0) root         (0)     6158 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ses/domain_identity.py
--rw-r--r--   0 root         (0) root         (0)    10385 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ses/identity_notification_topic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.871218 idem-aws-1.7.5/idem_aws/states/aws/sesv2/
--rw-r--r--   0 root         (0) root         (0)    14618 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/sesv2/event_destination.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.871218 idem-aws-1.7.5/idem_aws/states/aws/sns/
--rw-r--r--   0 root         (0) root         (0)    11622 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/sns/subscription.py
--rw-r--r--   0 root         (0) root         (0)    13240 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/sns/topic.py
--rw-r--r--   0 root         (0) root         (0)     8684 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/sns/topic_policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.871218 idem-aws-1.7.5/idem_aws/states/aws/sqs/
--rw-r--r--   0 root         (0) root         (0)    24692 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/sqs/queue.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.872218 idem-aws-1.7.5/idem_aws/states/aws/wafv2/
--rw-r--r--   0 root         (0) root         (0)     9933 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/wafv2/associate_web_acl.py
--rw-r--r--   0 root         (0) root         (0)    14712 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/wafv2/ip_set.py
--rw-r--r--   0 root         (0) root         (0)    12255 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/wafv2/regex_pattern_set.py
--rw-r--r--   0 root         (0) root         (0)   268538 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/wafv2/web_acl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.838215 idem-aws-1.7.5/idem_aws/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.874218 idem-aws-1.7.5/idem_aws/tool/aws/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.874218 idem-aws-1.7.5/idem_aws/tool/aws/acct/
--rw-r--r--   0 root         (0) root         (0)     1393 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/acct/assume_role.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.874218 idem-aws-1.7.5/idem_aws/tool/aws/acct/contracts/
--rw-r--r--   0 root         (0) root         (0)      159 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/acct/contracts/init.py
--rw-r--r--   0 root         (0) root         (0)      293 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/acct/esm.py
--rw-r--r--   0 root         (0) root         (0)      714 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/acct/init.py
--rw-r--r--   0 root         (0) root         (0)     1577 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/acct/key_name.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.874218 idem-aws-1.7.5/idem_aws/tool/aws/acm/
--rw-r--r--   0 root         (0) root         (0)     2485 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/acm/certificate_validation_utils.py
--rw-r--r--   0 root         (0) root         (0)     5339 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/acm/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     2625 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/acm/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.876218 idem-aws-1.7.5/idem_aws/tool/aws/apigateway/
--rw-r--r--   0 root         (0) root         (0)     3883 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/apigateway/base_path_mapping.py
--rw-r--r--   0 root         (0) root         (0)     3343 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/apigateway/deployment.py
--rw-r--r--   0 root         (0) root         (0)     8767 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/apigateway/domain_name.py
--rw-r--r--   0 root         (0) root         (0)     4535 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/apigateway/integration.py
--rw-r--r--   0 root         (0) root         (0)     5000 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/apigateway/integration_response.py
--rw-r--r--   0 root         (0) root         (0)     4226 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/apigateway/method.py
--rw-r--r--   0 root         (0) root         (0)     4250 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/apigateway/method_response.py
--rw-r--r--   0 root         (0) root         (0)     4087 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/apigateway/resource.py
--rw-r--r--   0 root         (0) root         (0)     7175 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/apigateway/rest_api.py
--rw-r--r--   0 root         (0) root         (0)     4417 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/apigateway/stage.py
--rw-r--r--   0 root         (0) root         (0)     2203 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/apigateway/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.876218 idem-aws-1.7.5/idem_aws/tool/aws/apigatewayv2/
--rw-r--r--   0 root         (0) root         (0)     5671 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/apigatewayv2/api.py
--rw-r--r--   0 root         (0) root         (0)     5125 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/apigatewayv2/authorizer.py
--rw-r--r--   0 root         (0) root         (0)     4842 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/apigatewayv2/domain_name.py
--rw-r--r--   0 root         (0) root         (0)     5187 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/apigatewayv2/integration.py
--rw-r--r--   0 root         (0) root         (0)     4793 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/apigatewayv2/route.py
--rw-r--r--   0 root         (0) root         (0)     4061 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/apigatewayv2/stage.py
--rw-r--r--   0 root         (0) root         (0)     2655 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/apigatewayv2/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.876218 idem-aws-1.7.5/idem_aws/tool/aws/application_autoscaling/
--rw-r--r--   0 root         (0) root         (0)     2724 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/application_autoscaling/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     1725 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/application_autoscaling/scalable_target.py
--rw-r--r--   0 root         (0) root         (0)     1907 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/application_autoscaling/scaling_policy.py
--rw-r--r--   0 root         (0) root         (0)     4099 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/arn_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.877218 idem-aws-1.7.5/idem_aws/tool/aws/autoscaling/
--rw-r--r--   0 root         (0) root         (0)     5561 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/autoscaling/auto_scaling_group_utils.py
--rw-r--r--   0 root         (0) root         (0)     4257 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/autoscaling/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     3367 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/autoscaling/scaling_policy.py
--rw-r--r--   0 root         (0) root         (0)     2946 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/autoscaling/tag.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/b64.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.877218 idem-aws-1.7.5/idem_aws/tool/aws/backup/
--rw-r--r--   0 root         (0) root         (0)     1042 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/backup/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     2452 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/backup/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.877218 idem-aws-1.7.5/idem_aws/tool/aws/budgets/
--rw-r--r--   0 root         (0) root         (0)     5249 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/budgets/budget.py
--rw-r--r--   0 root         (0) root         (0)     3415 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/budgets/budget_action.py
--rw-r--r--   0 root         (0) root         (0)     3563 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/budgets/conversion_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.877218 idem-aws-1.7.5/idem_aws/tool/aws/cloudformation/
--rw-r--r--   0 root         (0) root         (0)    18904 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/cloudformation/stack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.878219 idem-aws-1.7.5/idem_aws/tool/aws/cloudfront/
--rw-r--r--   0 root         (0) root         (0)     6468 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/cloudfront/cloudfront_utils.py
--rw-r--r--   0 root         (0) root         (0)     4860 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/cloudfront/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     7618 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/cloudfront/distribution.py
--rw-r--r--   0 root         (0) root         (0)     2010 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/cloudfront/distribution_utils.py
--rw-r--r--   0 root         (0) root         (0)     2416 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/cloudfront/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.878219 idem-aws-1.7.5/idem_aws/tool/aws/cloudtrail/
--rw-r--r--   0 root         (0) root         (0)     3966 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/cloudtrail/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)    13076 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/cloudtrail/trail.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.879219 idem-aws-1.7.5/idem_aws/tool/aws/cloudwatch/
--rw-r--r--   0 root         (0) root         (0)     3540 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/cloudwatch/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)      807 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/cloudwatch/log_group.py
--rw-r--r--   0 root         (0) root         (0)     4464 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/cloudwatch/metric_alarm.py
--rw-r--r--   0 root         (0) root         (0)     2033 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/cloudwatch/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.879219 idem-aws-1.7.5/idem_aws/tool/aws/cloudwatchlogs/
--rw-r--r--   0 root         (0) root         (0)      566 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/cloudwatchlogs/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     3193 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/comment_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.879219 idem-aws-1.7.5/idem_aws/tool/aws/config/
--rw-r--r--   0 root         (0) root         (0)     1511 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/config/config_utils.py
--rwxr-xr-x   0 root         (0) root         (0)     4483 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/config/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     2032 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/config/delivery_channel.py
--rw-r--r--   0 root         (0) root         (0)     2578 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/config/rule.py
--rw-r--r--   0 root         (0) root         (0)     2434 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/config/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.879219 idem-aws-1.7.5/idem_aws/tool/aws/costexplorer/
--rw-r--r--   0 root         (0) root         (0)     1024 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/costexplorer/anomaly_monitor.py
--rw-r--r--   0 root         (0) root         (0)     3078 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/costexplorer/anomaly_subscription.py
--rw-r--r--   0 root         (0) root         (0)     2953 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/costexplorer/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     4859 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/costexplorer/cost_category.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.880219 idem-aws-1.7.5/idem_aws/tool/aws/docdb/
--rw-r--r--   0 root         (0) root         (0)    12556 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/docdb/db_cluster.py
--rw-r--r--   0 root         (0) root         (0)     6638 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/docdb/db_cluster_parameter_group.py
--rw-r--r--   0 root         (0) root         (0)     2668 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/docdb/db_subnet_group.py
--rw-r--r--   0 root         (0) root         (0)     3183 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/docdb/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.880219 idem-aws-1.7.5/idem_aws/tool/aws/dynamodb/
--rw-r--r--   0 root         (0) root         (0)    15451 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/dynamodb/table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.882219 idem-aws-1.7.5/idem_aws/tool/aws/ec2/
--rw-r--r--   0 root         (0) root         (0)     3051 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/ami.py
--rw-r--r--   0 root         (0) root         (0)     2022 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/availability_zones.py
--rw-r--r--   0 root         (0) root         (0)    37442 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/dhcp_option_association_utils.py
--rw-r--r--   0 root         (0) root         (0)     1774 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/elastic_ip.py
--rw-r--r--   0 root         (0) root         (0)     1525 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/flow_log.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.882219 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/
--rw-r--r--   0 root         (0) root         (0)     1280 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/data.py
--rw-r--r--   0 root         (0) root         (0)     2910 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/key_pair.py
--rw-r--r--   0 root         (0) root         (0)    19910 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/state.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.884219 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/
--rw-r--r--   0 root         (0) root         (0)     4440 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/block_device_mappings.py
--rw-r--r--   0 root         (0) root         (0)     1813 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/bootstrap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.884219 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/contracts/
--rw-r--r--   0 root         (0) root         (0)      677 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/contracts/init.py
--rw-r--r--   0 root         (0) root         (0)     1191 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/disable_api_termination.py
--rw-r--r--   0 root         (0) root         (0)     1258 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/ebs_optimized.py
--rw-r--r--   0 root         (0) root         (0)     2287 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/iam_instance_profile_arn.py
--rw-r--r--   0 root         (0) root         (0)     8226 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/init.py
--rw-r--r--   0 root         (0) root         (0)     1227 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/instance_initiated_shutdown_behavior.py
--rw-r--r--   0 root         (0) root         (0)     1256 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/instance_type.py
--rw-r--r--   0 root         (0) root         (0)     1300 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/kernel_id.py
--rw-r--r--   0 root         (0) root         (0)     1154 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/monitoring_enabled.py
--rw-r--r--   0 root         (0) root         (0)     4123 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/network_interfaces.py
--rw-r--r--   0 root         (0) root         (0)     1656 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/placement.py
--rw-r--r--   0 root         (0) root         (0)     1119 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/private_ip_address.py
--rw-r--r--   0 root         (0) root         (0)     1313 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/ram_disk_id.py
--rw-r--r--   0 root         (0) root         (0)      214 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/running.py
--rw-r--r--   0 root         (0) root         (0)     1022 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/security_group_ids.py
--rw-r--r--   0 root         (0) root         (0)     1173 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/source_dest_check.py
--rw-r--r--   0 root         (0) root         (0)     1173 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/sriov_net_support.py
--rw-r--r--   0 root         (0) root         (0)     1799 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/tags.py
--rw-r--r--   0 root         (0) root         (0)     1281 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/user_data.py
--rw-r--r--   0 root         (0) root         (0)     4843 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/internet_gateway.py
--rw-r--r--   0 root         (0) root         (0)     1585 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/key_pair.py
--rw-r--r--   0 root         (0) root         (0)     3658 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/launch_template.py
--rw-r--r--   0 root         (0) root         (0)     3948 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/network_interface.py
--rw-r--r--   0 root         (0) root         (0)     1517 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/placement_group.py
--rw-r--r--   0 root         (0) root         (0)    12208 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/route_table.py
--rw-r--r--   0 root         (0) root         (0)     3924 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/security_group_rule.py
--rw-r--r--   0 root         (0) root         (0)     1801 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/snapshot.py
--rw-r--r--   0 root         (0) root         (0)     2779 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/spot_instance_request.py
--rw-r--r--   0 root         (0) root         (0)    14415 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/subnet.py
--rw-r--r--   0 root         (0) root         (0)     2752 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/tag.py
--rw-r--r--   0 root         (0) root         (0)     3821 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/transit_gateway.py
--rw-r--r--   0 root         (0) root         (0)     3043 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/transit_gateway_vpc_attachment.py
--rw-r--r--   0 root         (0) root         (0)     1745 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/volume.py
--rw-r--r--   0 root         (0) root         (0)     7822 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/vpc.py
--rw-r--r--   0 root         (0) root         (0)     8498 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/vpc_endpoint.py
--rw-r--r--   0 root         (0) root         (0)    10282 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/vpc_peering_connection_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.885219 idem-aws-1.7.5/idem_aws/tool/aws/ecr/
--rw-r--r--   0 root         (0) root         (0)     4995 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ecr/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     3190 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ecr/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.885219 idem-aws-1.7.5/idem_aws/tool/aws/efs/
--rw-r--r--   0 root         (0) root         (0)     2368 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/efs/file_system_utils.py
--rw-r--r--   0 root         (0) root         (0)      947 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/efs/mount_target_utils.py
--rw-r--r--   0 root         (0) root         (0)     1850 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/efs/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.885219 idem-aws-1.7.5/idem_aws/tool/aws/eks/
--rw-r--r--   0 root         (0) root         (0)     4881 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/eks/addon.py
--rw-r--r--   0 root         (0) root         (0)     9514 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/eks/cluster.py
--rw-r--r--   0 root         (0) root         (0)     5220 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/eks/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     4559 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/eks/eks_utils.py
--rw-r--r--   0 root         (0) root         (0)     7710 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/eks/nodegroup.py
--rw-r--r--   0 root         (0) root         (0)     1868 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/eks/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.886219 idem-aws-1.7.5/idem_aws/tool/aws/elasticache/
--rw-r--r--   0 root         (0) root         (0)     9303 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/elasticache/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)    20325 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/elasticache/elasticache_utils.py
--rw-r--r--   0 root         (0) root         (0)     1737 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/elasticache/parameters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.886219 idem-aws-1.7.5/idem_aws/tool/aws/elb/
--rw-r--r--   0 root         (0) root         (0)     1957 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/elb/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)    19196 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/elb/load_balancer.py
--rw-r--r--   0 root         (0) root         (0)     2429 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/elb/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.887219 idem-aws-1.7.5/idem_aws/tool/aws/elbv2/
--rw-r--r--   0 root         (0) root         (0)     7683 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/elbv2/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)    10904 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/elbv2/listener.py
--rw-r--r--   0 root         (0) root         (0)    10107 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/elbv2/load_balancer.py
--rw-r--r--   0 root         (0) root         (0)     2428 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/elbv2/tag.py
--rw-r--r--   0 root         (0) root         (0)    10958 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/elbv2/target_group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.887219 idem-aws-1.7.5/idem_aws/tool/aws/es/
--rw-r--r--   0 root         (0) root         (0)     9741 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/es/elasticsearch_domain.py
--rw-r--r--   0 root         (0) root         (0)     2511 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/es/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.887219 idem-aws-1.7.5/idem_aws/tool/aws/events/
--rw-r--r--   0 root         (0) root         (0)     1707 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/events/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     5958 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/events/rule.py
--rw-r--r--   0 root         (0) root         (0)     2752 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/events/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.888219 idem-aws-1.7.5/idem_aws/tool/aws/guardduty/
--rw-r--r--   0 root         (0) root         (0)     1048 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/guardduty/config_utils.py
--rw-r--r--   0 root         (0) root         (0)     3246 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/guardduty/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     7045 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/guardduty/detector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.889219 idem-aws-1.7.5/idem_aws/tool/aws/iam/
--rw-r--r--   0 root         (0) root         (0)    12738 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/iam/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     1649 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/iam/group.py
--rw-r--r--   0 root         (0) root         (0)     2324 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/iam/group_membership.py
--rw-r--r--   0 root         (0) root         (0)     2737 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/iam/password_policy.py
--rw-r--r--   0 root         (0) root         (0)     7466 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/iam/policy.py
--rw-r--r--   0 root         (0) root         (0)     1573 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/iam/role_policy_attachment.py
--rw-r--r--   0 root         (0) root         (0)     1251 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/iam/service_linked_role.py
--rw-r--r--   0 root         (0) root         (0)     3720 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/iam/user.py
--rw-r--r--   0 root         (0) root         (0)     1486 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/iam/user_ssh_key.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.889219 idem-aws-1.7.5/idem_aws/tool/aws/kinesis/
--rw-r--r--   0 root         (0) root         (0)     1976 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/kinesis/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)    21390 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/kinesis/stream.py
--rw-r--r--   0 root         (0) root         (0)     2362 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/kinesis/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.889219 idem-aws-1.7.5/idem_aws/tool/aws/kms/
--rw-r--r--   0 root         (0) root         (0)      999 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/kms/alias.py
--rw-r--r--   0 root         (0) root         (0)     3196 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/kms/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     3159 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/kms/key.py
--rw-r--r--   0 root         (0) root         (0)     2060 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/kms/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.890220 idem-aws-1.7.5/idem_aws/tool/aws/lambda_aws/
--rw-r--r--   0 root         (0) root         (0)     3194 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/lambda_aws/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)    16057 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/lambda_aws/function.py
--rw-r--r--   0 root         (0) root         (0)     4274 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/lambda_aws/function_event_invoke_config.py
--rw-r--r--   0 root         (0) root         (0)     2579 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/lambda_aws/function_permission.py
--rw-r--r--   0 root         (0) root         (0)     1680 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/lambda_aws/function_provisioned_concurrency_config.py
--rw-r--r--   0 root         (0) root         (0)       27 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/lambda_aws/init.py
--rw-r--r--   0 root         (0) root         (0)     2689 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/lambda_aws/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.890220 idem-aws-1.7.5/idem_aws/tool/aws/logs/
--rw-r--r--   0 root         (0) root         (0)     1336 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/logs/subscription_filter_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.891219 idem-aws-1.7.5/idem_aws/tool/aws/neptune/
--rw-r--r--   0 root         (0) root         (0)     8991 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/neptune/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)    12251 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/neptune/db_cluster.py
--rw-r--r--   0 root         (0) root         (0)     6385 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/neptune/db_cluster_parameter_group.py
--rw-r--r--   0 root         (0) root         (0)    11654 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/neptune/db_instance.py
--rw-r--r--   0 root         (0) root         (0)     6128 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/neptune/db_parameter_group.py
--rw-r--r--   0 root         (0) root         (0)     1546 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/neptune/db_subnet_group.py
--rw-r--r--   0 root         (0) root         (0)     3258 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/neptune/tag.py
--rw-r--r--   0 root         (0) root         (0)     2094 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/network_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.891219 idem-aws-1.7.5/idem_aws/tool/aws/organizations/
--rw-r--r--   0 root         (0) root         (0)     1795 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/organizations/account.py
--rw-r--r--   0 root         (0) root         (0)     4764 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/organizations/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     1656 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/organizations/policy_attachment.py
--rw-r--r--   0 root         (0) root         (0)     2704 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/organizations/tag.py
--rw-r--r--   0 root         (0) root         (0)     1496 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/parameters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.892220 idem-aws-1.7.5/idem_aws/tool/aws/rds/
--rw-r--r--   0 root         (0) root         (0)    12718 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/rds/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     5582 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/rds/parameters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.892220 idem-aws-1.7.5/idem_aws/tool/aws/route53/
--rw-r--r--   0 root         (0) root         (0)     5018 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/route53/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     1251 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/route53/hosted_zone_association.py
--rw-r--r--   0 root         (0) root         (0)     5900 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/route53/hosted_zone_utils.py
--rw-r--r--   0 root         (0) root         (0)     7422 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/route53/resource_record_utils.py
--rw-r--r--   0 root         (0) root         (0)     2663 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/route53/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.893220 idem-aws-1.7.5/idem_aws/tool/aws/s3/
--rw-r--r--   0 root         (0) root         (0)     1526 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/s3/bucket_acl.py
--rw-r--r--   0 root         (0) root         (0)     7925 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/s3/bucket_encryption.py
--rw-r--r--   0 root         (0) root         (0)     7403 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/s3/bucket_lifecycle.py
--rw-r--r--   0 root         (0) root         (0)     2440 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/s3/bucket_logging.py
--rw-r--r--   0 root         (0) root         (0)     2584 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/s3/bucket_replication.py
--rw-r--r--   0 root         (0) root         (0)     1050 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/s3/bucket_versioning.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/s3/bucket_website.py
--rw-r--r--   0 root         (0) root         (0)     9894 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/s3/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     3373 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/s3/s3_utils.py
--rw-r--r--   0 root         (0) root         (0)     1506 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/search_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.893220 idem-aws-1.7.5/idem_aws/tool/aws/ses/
--rw-r--r--   0 root         (0) root         (0)     1214 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ses/conversion_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.893220 idem-aws-1.7.5/idem_aws/tool/aws/sesv2/
--rw-r--r--   0 root         (0) root         (0)      563 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/sesv2/conversion_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.893220 idem-aws-1.7.5/idem_aws/tool/aws/sns/
--rw-r--r--   0 root         (0) root         (0)     3617 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/sns/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     7581 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/sns/sns_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.894220 idem-aws-1.7.5/idem_aws/tool/aws/sqs/
--rw-r--r--   0 root         (0) root         (0)     6482 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/sqs/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     5455 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/sqs/queue_utils.py
--rw-r--r--   0 root         (0) root         (0)     3760 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/state_comparison_utils.py
--rw-r--r--   0 root         (0) root         (0)      859 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/state_utils.py
--rw-r--r--   0 root         (0) root         (0)      526 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/string_utils.py
--rw-r--r--   0 root         (0) root         (0)     5900 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/tag_utils.py
--rw-r--r--   0 root         (0) root         (0)     1548 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/test_state_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.894220 idem-aws-1.7.5/idem_aws/tool/aws/wafv2/
--rw-r--r--   0 root         (0) root         (0)     6843 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/wafv2/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     3076 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/wafv2/ip_set_utils.py
--rw-r--r--   0 root         (0) root         (0)     1661 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/wafv2/regex_pattern_set.py
--rw-r--r--   0 root         (0) root         (0)     3822 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/wafv2/tag.py
--rw-r--r--   0 root         (0) root         (0)     2310 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/wafv2/web_acl.py
--rw-r--r--   0 root         (0) root         (0)     1050 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/waiter_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.895220 idem-aws-1.7.5/idem_aws/tool/boto3/
--rw-r--r--   0 root         (0) root         (0)     5000 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/boto3/client.py
--rw-r--r--   0 root         (0) root         (0)     5181 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/boto3/custom_waiter.py
--rw-r--r--   0 root         (0) root         (0)      429 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/boto3/exception.py
--rw-r--r--   0 root         (0) root         (0)      669 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/boto3/region.py
--rw-r--r--   0 root         (0) root         (0)     6270 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/boto3/resolve.py
--rw-r--r--   0 root         (0) root         (0)     5230 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/boto3/resource.py
--rw-r--r--   0 root         (0) root         (0)     1411 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/boto3/session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.895220 idem-aws-1.7.5/idem_aws/tool/heist/
--rw-r--r--   0 root         (0) root         (0)      906 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/heist/bootstrap.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-05 18:38:41.000000 idem-aws-1.7.5/idem_aws/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.839216 idem-aws-1.7.5/idem_aws.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11051 2023-05-05 18:38:41.000000 idem-aws-1.7.5/idem_aws.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    22825 2023-05-05 18:38:41.000000 idem-aws-1.7.5/idem_aws.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 18:38:41.000000 idem-aws-1.7.5/idem_aws.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      588 2023-05-05 18:38:41.000000 idem-aws-1.7.5/idem_aws.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-05 18:38:41.000000 idem-aws-1.7.5/idem_aws.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      365 2023-05-05 18:38:25.000000 idem-aws-1.7.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-05 18:38:41.895220 idem-aws-1.7.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3136 2023-05-05 18:38:25.000000 idem-aws-1.7.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.426671 idem-aws-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)    11342 2023-05-15 22:31:55.000000 idem-aws-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       54 2023-05-15 22:31:55.000000 idem-aws-2.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    11102 2023-05-15 22:32:09.426671 idem-aws-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9835 2023-05-15 22:31:55.000000 idem-aws-2.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.386671 idem-aws-2.0.0/idem_aws/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.378671 idem-aws-2.0.0/idem_aws/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.386671 idem-aws-2.0.0/idem_aws/acct/aws/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.386671 idem-aws-2.0.0/idem_aws/acct/aws/contracts/
+-rw-r--r--   0 root         (0) root         (0)     1127 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/acct/aws/contracts/init.py
+-rw-r--r--   0 root         (0) root         (0)     5506 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/acct/aws/gsuite.py
+-rw-r--r--   0 root         (0) root         (0)     1618 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/acct/aws/iam.py
+-rw-r--r--   0 root         (0) root         (0)     2213 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/acct/aws/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.386671 idem-aws-2.0.0/idem_aws/acct/metadata/
+-rw-r--r--   0 root         (0) root         (0)      534 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/acct/metadata/aws.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.378671 idem-aws-2.0.0/idem_aws/autogen/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.386671 idem-aws-2.0.0/idem_aws/autogen/aws/
+-rw-r--r--   0 root         (0) root         (0)     7082 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/autogen/aws/function.py
+-rw-r--r--   0 root         (0) root         (0)     9947 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/autogen/aws/init.py
+-rw-r--r--   0 root         (0) root         (0)     3023 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/autogen/aws/param.py
+-rw-r--r--   0 root         (0) root         (0)     4731 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/autogen/aws/plugin.py
+-rw-r--r--   0 root         (0) root         (0)      677 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/autogen/aws/possible_functions.py
+-rw-r--r--   0 root         (0) root         (0)     3870 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/autogen/aws/resource.py
+-rw-r--r--   0 root         (0) root         (0)     4045 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/autogen/aws/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.386671 idem-aws-2.0.0/idem_aws/autogen/aws/tag/
+-rw-r--r--   0 root         (0) root         (0)     3401 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/autogen/aws/tag/plugin.py
+-rw-r--r--   0 root         (0) root         (0)     4865 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/autogen/aws/tag/template.py
+-rw-r--r--   0 root         (0) root         (0)    15883 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/autogen/aws/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.386671 idem-aws-2.0.0/idem_aws/autogen/aws/utils/
+-rw-r--r--   0 root         (0) root         (0)     1361 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/autogen/aws/utils/plugin.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/autogen/aws/utils/template.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.386671 idem-aws-2.0.0/idem_aws/esm/
+-rw-r--r--   0 root         (0) root         (0)     8838 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/esm/aws.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.386671 idem-aws-2.0.0/idem_aws/esm/contracts/
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/esm/contracts/aws.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.382671 idem-aws-2.0.0/idem_aws/exec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.386671 idem-aws-2.0.0/idem_aws/exec/aws/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.386671 idem-aws-2.0.0/idem_aws/exec/aws/acm/
+-rw-r--r--   0 root         (0) root         (0)     2000 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/acm/certificate_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.386671 idem-aws-2.0.0/idem_aws/exec/aws/apigateway/
+-rw-r--r--   0 root         (0) root         (0)     5430 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/apigateway/base_path_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     2600 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/apigateway/deployment.py
+-rw-r--r--   0 root         (0) root         (0)     3322 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/apigateway/domain_name.py
+-rw-r--r--   0 root         (0) root         (0)     1925 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/apigateway/integration.py
+-rw-r--r--   0 root         (0) root         (0)     2971 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/apigateway/integration_response.py
+-rw-r--r--   0 root         (0) root         (0)     1766 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/apigateway/method.py
+-rw-r--r--   0 root         (0) root         (0)     2145 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/apigateway/method_response.py
+-rw-r--r--   0 root         (0) root         (0)     1136 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/apigateway/resource.py
+-rw-r--r--   0 root         (0) root         (0)     2435 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/apigateway/rest_api.py
+-rw-r--r--   0 root         (0) root         (0)     2608 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/apigateway/stage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.386671 idem-aws-2.0.0/idem_aws/exec/aws/apigatewayv2/
+-rw-r--r--   0 root         (0) root         (0)     3276 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/apigatewayv2/api.py
+-rw-r--r--   0 root         (0) root         (0)     2069 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/apigatewayv2/authorizer.py
+-rw-r--r--   0 root         (0) root         (0)     1890 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/apigatewayv2/domain_name.py
+-rw-r--r--   0 root         (0) root         (0)     2184 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/apigatewayv2/integration.py
+-rw-r--r--   0 root         (0) root         (0)     3761 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/apigatewayv2/route.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.390671 idem-aws-2.0.0/idem_aws/exec/aws/application_autoscaling/
+-rw-r--r--   0 root         (0) root         (0)     3192 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/application_autoscaling/scalable_target.py
+-rw-r--r--   0 root         (0) root         (0)     3395 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/application_autoscaling/scaling_policy.py
+-rw-r--r--   0 root         (0) root         (0)     2846 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/arn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.390671 idem-aws-2.0.0/idem_aws/exec/aws/autoscaling/
+-rw-r--r--   0 root         (0) root         (0)     3034 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/autoscaling/scaling_policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.390671 idem-aws-2.0.0/idem_aws/exec/aws/backup/
+-rw-r--r--   0 root         (0) root         (0)     4661 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/backup/backup_vault.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.390671 idem-aws-2.0.0/idem_aws/exec/aws/budgets/
+-rw-r--r--   0 root         (0) root         (0)     4105 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/budgets/budget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.390671 idem-aws-2.0.0/idem_aws/exec/aws/cloudformation/
+-rw-r--r--   0 root         (0) root         (0)     2285 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/cloudformation/stack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.390671 idem-aws-2.0.0/idem_aws/exec/aws/cloudfront/
+-rw-r--r--   0 root         (0) root         (0)     4007 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/cloudfront/cache_policy.py
+-rw-r--r--   0 root         (0) root         (0)     2697 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/cloudfront/distribution.py
+-rw-r--r--   0 root         (0) root         (0)     4297 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/cloudfront/origin_request_policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.390671 idem-aws-2.0.0/idem_aws/exec/aws/cloudwatch/
+-rw-r--r--   0 root         (0) root         (0)     3012 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/cloudwatch/log_group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.390671 idem-aws-2.0.0/idem_aws/exec/aws/cloudwatchlogs/
+-rw-r--r--   0 root         (0) root         (0)     1528 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/cloudwatchlogs/resource_policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.390671 idem-aws-2.0.0/idem_aws/exec/aws/config/
+-rw-r--r--   0 root         (0) root         (0)     4538 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/config/configuration_aggregator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.390671 idem-aws-2.0.0/idem_aws/exec/aws/costexplorer/
+-rw-r--r--   0 root         (0) root         (0)     1660 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/costexplorer/cost_allocation_tag.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.390671 idem-aws-2.0.0/idem_aws/exec/aws/docdb/
+-rw-r--r--   0 root         (0) root         (0)     6138 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/docdb/db_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     7293 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/docdb/db_cluster_parameter_group.py
+-rw-r--r--   0 root         (0) root         (0)     4887 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/docdb/db_subnet_group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.390671 idem-aws-2.0.0/idem_aws/exec/aws/dynamodb/
+-rw-r--r--   0 root         (0) root         (0)     2434 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/dynamodb/table.py
+-rw-r--r--   0 root         (0) root         (0)     2318 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/dynamodb/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.390671 idem-aws-2.0.0/idem_aws/exec/aws/ec2/
+-rw-r--r--   0 root         (0) root         (0)     8697 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/ec2/ami.py
+-rw-r--r--   0 root         (0) root         (0)     4290 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/ec2/availability_zones.py
+-rw-r--r--   0 root         (0) root         (0)     4206 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/ec2/elastic_ip.py
+-rw-r--r--   0 root         (0) root         (0)     3405 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/ec2/flow_log.py
+-rw-r--r--   0 root         (0) root         (0)    22002 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/ec2/instance.py
+-rw-r--r--   0 root         (0) root         (0)     3299 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/ec2/instance_type.py
+-rw-r--r--   0 root         (0) root         (0)     1511 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/ec2/internet_gateway.py
+-rw-r--r--   0 root         (0) root         (0)     2216 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/ec2/key_pair.py
+-rw-r--r--   0 root         (0) root         (0)     7293 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/ec2/launch_template.py
+-rw-r--r--   0 root         (0) root         (0)     8692 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/ec2/network_interface.py
+-rw-r--r--   0 root         (0) root         (0)     4680 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/ec2/placement_group.py
+-rw-r--r--   0 root         (0) root         (0)     5836 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/ec2/route.py
+-rw-r--r--   0 root         (0) root         (0)     3579 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/ec2/route_table.py
+-rw-r--r--   0 root         (0) root         (0)     3265 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/ec2/route_table_association.py
+-rw-r--r--   0 root         (0) root         (0)     5108 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/ec2/security_group.py
+-rw-r--r--   0 root         (0) root         (0)     4143 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/ec2/security_group_rule.py
+-rw-r--r--   0 root         (0) root         (0)     4810 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/ec2/snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     4295 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/ec2/spot_instance_request.py
+-rw-r--r--   0 root         (0) root         (0)     8595 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/ec2/subnet.py
+-rw-r--r--   0 root         (0) root         (0)     4471 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/ec2/volume.py
+-rw-r--r--   0 root         (0) root         (0)     4459 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/ec2/vpc.py
+-rw-r--r--   0 root         (0) root         (0)     4081 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/ec2/vpc_endpoint.py
+-rw-r--r--   0 root         (0) root         (0)     1952 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/ec2/vpc_peering_connection.py
+-rw-r--r--   0 root         (0) root         (0)     2007 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/ec2/vpc_peering_connection_accepter.py
+-rw-r--r--   0 root         (0) root         (0)     2048 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/ec2/vpc_peering_connection_options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.390671 idem-aws-2.0.0/idem_aws/exec/aws/ecr/
+-rw-r--r--   0 root         (0) root         (0)     5183 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/ecr/image.py
+-rw-r--r--   0 root         (0) root         (0)     3195 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/ecr/lifecycle_policy.py
+-rw-r--r--   0 root         (0) root         (0)     5504 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/ecr/repository.py
+-rw-r--r--   0 root         (0) root         (0)     2750 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/ecr/repository_policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.390671 idem-aws-2.0.0/idem_aws/exec/aws/eks/
+-rw-r--r--   0 root         (0) root         (0)     1665 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/eks/cluster.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.390671 idem-aws-2.0.0/idem_aws/exec/aws/elasticache/
+-rw-r--r--   0 root         (0) root         (0)     2934 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/elasticache/replication_group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.390671 idem-aws-2.0.0/idem_aws/exec/aws/elb/
+-rw-r--r--   0 root         (0) root         (0)     3023 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/elb/elb_hosted_zone_id.py
+-rw-r--r--   0 root         (0) root         (0)     3363 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/elb/load_balancer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.390671 idem-aws-2.0.0/idem_aws/exec/aws/elbv2/
+-rw-r--r--   0 root         (0) root         (0)     3296 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/elbv2/listener.py
+-rw-r--r--   0 root         (0) root         (0)     3346 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/elbv2/load_balancer.py
+-rw-r--r--   0 root         (0) root         (0)     4861 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/elbv2/target_group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.394671 idem-aws-2.0.0/idem_aws/exec/aws/es/
+-rw-r--r--   0 root         (0) root         (0)     2387 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/es/elasticsearch_domain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.394671 idem-aws-2.0.0/idem_aws/exec/aws/events/
+-rw-r--r--   0 root         (0) root         (0)     5682 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/events/rule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.394671 idem-aws-2.0.0/idem_aws/exec/aws/guardduty/
+-rw-r--r--   0 root         (0) root         (0)     2423 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/guardduty/detector.py
+-rw-r--r--   0 root         (0) root         (0)     5618 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/guardduty/member.py
+-rw-r--r--   0 root         (0) root         (0)     1814 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/guardduty/organization_admin_account.py
+-rw-r--r--   0 root         (0) root         (0)     8637 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/guardduty/organization_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.394671 idem-aws-2.0.0/idem_aws/exec/aws/iam/
+-rw-r--r--   0 root         (0) root         (0)     9324 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/iam/access_key.py
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/iam/group.py
+-rw-r--r--   0 root         (0) root         (0)     1199 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/iam/group_membership.py
+-rw-r--r--   0 root         (0) root         (0)     2099 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/iam/group_policy_attachment.py
+-rw-r--r--   0 root         (0) root         (0)     4749 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/iam/instance_profile.py
+-rw-r--r--   0 root         (0) root         (0)     7709 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/iam/open_id_connect_provider.py
+-rw-r--r--   0 root         (0) root         (0)     1842 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/iam/password_policy.py
+-rw-r--r--   0 root         (0) root         (0)     6957 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/iam/policy.py
+-rw-r--r--   0 root         (0) root         (0)     9723 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/iam/role.py
+-rw-r--r--   0 root         (0) root         (0)     1218 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/iam/user.py
+-rw-r--r--   0 root         (0) root         (0)     2945 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/iam/user_policy_attachment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.394671 idem-aws-2.0.0/idem_aws/exec/aws/kinesis/
+-rw-r--r--   0 root         (0) root         (0)     2919 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/kinesis/stream.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.394671 idem-aws-2.0.0/idem_aws/exec/aws/kms/
+-rw-r--r--   0 root         (0) root         (0)     3031 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/kms/key.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.394671 idem-aws-2.0.0/idem_aws/exec/aws/lambda_aws/
+-rw-r--r--   0 root         (0) root         (0)     4863 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/lambda_aws/function_event_invoke_config.py
+-rw-r--r--   0 root         (0) root         (0)     5632 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/lambda_aws/function_provisioned_concurrency_config.py
+-rw-r--r--   0 root         (0) root         (0)       27 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/lambda_aws/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.394671 idem-aws-2.0.0/idem_aws/exec/aws/neptune/
+-rw-r--r--   0 root         (0) root         (0)     7388 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/neptune/db_cluster_parameter_group.py
+-rw-r--r--   0 root         (0) root         (0)     6621 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/neptune/db_instance.py
+-rw-r--r--   0 root         (0) root         (0)     6854 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/neptune/db_parameter_group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.394671 idem-aws-2.0.0/idem_aws/exec/aws/organizations/
+-rw-r--r--   0 root         (0) root         (0)     4486 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/organizations/account.py
+-rw-r--r--   0 root         (0) root         (0)     2391 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/organizations/policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.394671 idem-aws-2.0.0/idem_aws/exec/aws/rds/
+-rw-r--r--   0 root         (0) root         (0)     5996 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/rds/db_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     5001 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/rds/db_cluster_parameter_group.py
+-rw-r--r--   0 root         (0) root         (0)     5971 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/rds/db_instance.py
+-rw-r--r--   0 root         (0) root         (0)     6287 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/rds/db_parameter_group.py
+-rw-r--r--   0 root         (0) root         (0)     4835 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/rds/db_subnet_group.py
+-rw-r--r--   0 root         (0) root         (0)     2686 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/rds/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.394671 idem-aws-2.0.0/idem_aws/exec/aws/route53/
+-rw-r--r--   0 root         (0) root         (0)     5251 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/route53/hosted_zone.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.394671 idem-aws-2.0.0/idem_aws/exec/aws/s3/
+-rw-r--r--   0 root         (0) root         (0)     2659 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/s3/bucket.py
+-rw-r--r--   0 root         (0) root         (0)     1518 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/s3/bucket_acl.py
+-rw-r--r--   0 root         (0) root         (0)     1918 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/s3/bucket_lifecycle.py
+-rw-r--r--   0 root         (0) root         (0)     1897 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/s3/bucket_logging.py
+-rw-r--r--   0 root         (0) root         (0)     1982 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/s3/bucket_replication.py
+-rw-r--r--   0 root         (0) root         (0)     1956 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/s3/bucket_website.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.394671 idem-aws-2.0.0/idem_aws/exec/aws/ses/
+-rw-r--r--   0 root         (0) root         (0)     3203 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/ses/domain_identity.py
+-rw-r--r--   0 root         (0) root         (0)     4167 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/ses/identity_notification_topic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.394671 idem-aws-2.0.0/idem_aws/exec/aws/sesv2/
+-rw-r--r--   0 root         (0) root         (0)     4342 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/sesv2/event_destination.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.394671 idem-aws-2.0.0/idem_aws/exec/aws/sns/
+-rw-r--r--   0 root         (0) root         (0)     3682 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/sns/subscription.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.394671 idem-aws-2.0.0/idem_aws/exec/aws/sqs/
+-rw-r--r--   0 root         (0) root         (0)     4686 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/sqs/queue.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.394671 idem-aws-2.0.0/idem_aws/exec/aws/sts/
+-rw-r--r--   0 root         (0) root         (0)     5261 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/sts/assume_role.py
+-rw-r--r--   0 root         (0) root         (0)     1259 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/sts/caller_identity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.394671 idem-aws-2.0.0/idem_aws/exec/aws/wafv2/
+-rw-r--r--   0 root         (0) root         (0)     4859 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/wafv2/ip_set.py
+-rw-r--r--   0 root         (0) root         (0)     7041 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/aws/wafv2/regex_pattern_set.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.394671 idem-aws-2.0.0/idem_aws/exec/boto3/
+-rw-r--r--   0 root         (0) root         (0)      747 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/exec/boto3/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.382671 idem-aws-2.0.0/idem_aws/reconcile/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.394671 idem-aws-2.0.0/idem_aws/reconcile/pending/
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/reconcile/pending/aws.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.382671 idem-aws-2.0.0/idem_aws/states/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.394671 idem-aws-2.0.0/idem_aws/states/aws/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.398671 idem-aws-2.0.0/idem_aws/states/aws/acm/
+-rw-r--r--   0 root         (0) root         (0)    28336 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/acm/certificate_manager.py
+-rw-r--r--   0 root         (0) root         (0)    11133 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/acm/certificate_validation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.398671 idem-aws-2.0.0/idem_aws/states/aws/apigateway/
+-rw-r--r--   0 root         (0) root         (0)    10257 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/apigateway/base_path_mapping.py
+-rw-r--r--   0 root         (0) root         (0)    12091 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/apigateway/deployment.py
+-rw-r--r--   0 root         (0) root         (0)    19520 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/apigateway/domain_name.py
+-rw-r--r--   0 root         (0) root         (0)    15779 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/apigateway/integration.py
+-rw-r--r--   0 root         (0) root         (0)    13752 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/apigateway/integration_response.py
+-rw-r--r--   0 root         (0) root         (0)    12951 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/apigateway/method.py
+-rw-r--r--   0 root         (0) root         (0)    12155 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/apigateway/method_response.py
+-rw-r--r--   0 root         (0) root         (0)     9866 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/apigateway/resource.py
+-rw-r--r--   0 root         (0) root         (0)    13732 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/apigateway/rest_api.py
+-rw-r--r--   0 root         (0) root         (0)    13857 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/apigateway/stage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.398671 idem-aws-2.0.0/idem_aws/states/aws/apigatewayv2/
+-rw-r--r--   0 root         (0) root         (0)    15354 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/apigatewayv2/api.py
+-rw-r--r--   0 root         (0) root         (0)    16244 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/apigatewayv2/authorizer.py
+-rw-r--r--   0 root         (0) root         (0)    15119 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/apigatewayv2/domain_name.py
+-rw-r--r--   0 root         (0) root         (0)    22693 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/apigatewayv2/integration.py
+-rw-r--r--   0 root         (0) root         (0)    14022 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/apigatewayv2/route.py
+-rw-r--r--   0 root         (0) root         (0)    16913 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/apigatewayv2/stage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.398671 idem-aws-2.0.0/idem_aws/states/aws/application_autoscaling/
+-rw-r--r--   0 root         (0) root         (0)    31855 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/application_autoscaling/scalable_target.py
+-rw-r--r--   0 root         (0) root         (0)    45934 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/application_autoscaling/scaling_policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.398671 idem-aws-2.0.0/idem_aws/states/aws/autoscaling/
+-rw-r--r--   0 root         (0) root         (0)    78777 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/autoscaling/auto_scaling_group.py
+-rw-r--r--   0 root         (0) root         (0)    32523 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/autoscaling/launch_configuration.py
+-rw-r--r--   0 root         (0) root         (0)    54968 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/autoscaling/scaling_policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.398671 idem-aws-2.0.0/idem_aws/states/aws/backup/
+-rw-r--r--   0 root         (0) root         (0)     8985 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/backup/backup_vault.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.398671 idem-aws-2.0.0/idem_aws/states/aws/budgets/
+-rw-r--r--   0 root         (0) root         (0)    25523 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/budgets/budget.py
+-rw-r--r--   0 root         (0) root         (0)    16456 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/budgets/budget_action.py
+-rw-r--r--   0 root         (0) root         (0)     1768 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/caller_identity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.398671 idem-aws-2.0.0/idem_aws/states/aws/cloudformation/
+-rw-r--r--   0 root         (0) root         (0)    32414 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/cloudformation/stack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.398671 idem-aws-2.0.0/idem_aws/states/aws/cloudfront/
+-rw-r--r--   0 root         (0) root         (0)    24459 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/cloudfront/cache_policy.py
+-rw-r--r--   0 root         (0) root         (0)   116104 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/cloudfront/distribution.py
+-rw-r--r--   0 root         (0) root         (0)    15501 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/cloudfront/origin_request_policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.398671 idem-aws-2.0.0/idem_aws/states/aws/cloudtrail/
+-rw-r--r--   0 root         (0) root         (0)    37423 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/cloudtrail/trail.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.398671 idem-aws-2.0.0/idem_aws/states/aws/cloudwatch/
+-rw-r--r--   0 root         (0) root         (0)    11420 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/cloudwatch/log_group.py
+-rw-r--r--   0 root         (0) root         (0)    36077 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/cloudwatch/metric_alarm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.398671 idem-aws-2.0.0/idem_aws/states/aws/cloudwatchlogs/
+-rw-r--r--   0 root         (0) root         (0)     8723 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/cloudwatchlogs/resource_policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.398671 idem-aws-2.0.0/idem_aws/states/aws/config/
+-rwxr-xr-x   0 root         (0) root         (0)    11422 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/config/config_recorder.py
+-rwxr-xr-x   0 root         (0) root         (0)     9512 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/config/config_recorder_status.py
+-rw-r--r--   0 root         (0) root         (0)    10463 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/config/configuration_aggregator.py
+-rwxr-xr-x   0 root         (0) root         (0)    12062 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/config/delivery_channel.py
+-rw-r--r--   0 root         (0) root         (0)    21665 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/config/rule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.398671 idem-aws-2.0.0/idem_aws/states/aws/costexplorer/
+-rw-r--r--   0 root         (0) root         (0)    18654 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/costexplorer/anomaly_monitor.py
+-rw-r--r--   0 root         (0) root         (0)    10751 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/costexplorer/anomaly_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    28397 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/costexplorer/cost_category.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.398671 idem-aws-2.0.0/idem_aws/states/aws/docdb/
+-rw-r--r--   0 root         (0) root         (0)    28355 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/docdb/db_cluster.py
+-rw-r--r--   0 root         (0) root         (0)    12967 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/docdb/db_cluster_parameter_group.py
+-rw-r--r--   0 root         (0) root         (0)    11755 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/docdb/db_subnet_group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.398671 idem-aws-2.0.0/idem_aws/states/aws/dynamodb/
+-rw-r--r--   0 root         (0) root         (0)    36228 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/dynamodb/table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.402671 idem-aws-2.0.0/idem_aws/states/aws/ec2/
+-rw-r--r--   0 root         (0) root         (0)    22039 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/ec2/ami.py
+-rw-r--r--   0 root         (0) root         (0)    15794 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/ec2/dhcp_option.py
+-rw-r--r--   0 root         (0) root         (0)    10017 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/ec2/dhcp_option_association.py
+-rw-r--r--   0 root         (0) root         (0)    13002 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/ec2/elastic_ip.py
+-rw-r--r--   0 root         (0) root         (0)    12633 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/ec2/flow_log.py
+-rw-r--r--   0 root         (0) root         (0)    40732 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/ec2/instance.py
+-rw-r--r--   0 root         (0) root         (0)    12429 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/ec2/internet_gateway.py
+-rw-r--r--   0 root         (0) root         (0)     9711 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/ec2/key_pair.py
+-rw-r--r--   0 root         (0) root         (0)    73136 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/ec2/launch_template.py
+-rw-r--r--   0 root         (0) root         (0)    17418 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/ec2/nat_gateway.py
+-rw-r--r--   0 root         (0) root         (0)    12093 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/ec2/network_interface.py
+-rw-r--r--   0 root         (0) root         (0)    10946 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/ec2/placement_group.py
+-rw-r--r--   0 root         (0) root         (0)    14835 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/ec2/route.py
+-rw-r--r--   0 root         (0) root         (0)    15623 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/ec2/route_table.py
+-rw-r--r--   0 root         (0) root         (0)     8933 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/ec2/route_table_association.py
+-rw-r--r--   0 root         (0) root         (0)    12947 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/ec2/security_group.py
+-rw-r--r--   0 root         (0) root         (0)    17979 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/ec2/security_group_rule.py
+-rw-r--r--   0 root         (0) root         (0)    10513 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/ec2/snapshot.py
+-rw-r--r--   0 root         (0) root         (0)    36976 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/ec2/spot_instance_request.py
+-rw-r--r--   0 root         (0) root         (0)    20046 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/ec2/subnet.py
+-rw-r--r--   0 root         (0) root         (0)    17765 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/ec2/transit_gateway.py
+-rw-r--r--   0 root         (0) root         (0)    16953 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/ec2/transit_gateway_vpc_attachment.py
+-rw-r--r--   0 root         (0) root         (0)    15331 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/ec2/volume.py
+-rw-r--r--   0 root         (0) root         (0)    20607 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/ec2/vpc.py
+-rw-r--r--   0 root         (0) root         (0)    19294 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/ec2/vpc_endpoint.py
+-rw-r--r--   0 root         (0) root         (0)    14516 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/ec2/vpc_peering_connection.py
+-rw-r--r--   0 root         (0) root         (0)     9225 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/ec2/vpc_peering_connection_accepter.py
+-rw-r--r--   0 root         (0) root         (0)     9871 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/ec2/vpc_peering_connection_options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.402671 idem-aws-2.0.0/idem_aws/states/aws/ecr/
+-rw-r--r--   0 root         (0) root         (0)    11586 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/ecr/lifecycle_policy.py
+-rw-r--r--   0 root         (0) root         (0)    13319 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/ecr/repository.py
+-rw-r--r--   0 root         (0) root         (0)    11707 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/ecr/repository_policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.402671 idem-aws-2.0.0/idem_aws/states/aws/efs/
+-rw-r--r--   0 root         (0) root         (0)    25301 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/efs/file_system.py
+-rw-r--r--   0 root         (0) root         (0)    22090 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/efs/mount_target.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.402671 idem-aws-2.0.0/idem_aws/states/aws/eks/
+-rw-r--r--   0 root         (0) root         (0)    18084 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/eks/addon.py
+-rw-r--r--   0 root         (0) root         (0)    29585 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/eks/cluster.py
+-rw-r--r--   0 root         (0) root         (0)    17678 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/eks/fargate_profile.py
+-rw-r--r--   0 root         (0) root         (0)    29787 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/eks/nodegroup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.402671 idem-aws-2.0.0/idem_aws/states/aws/elasticache/
+-rw-r--r--   0 root         (0) root         (0)    16170 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/elasticache/cache_parameter_group.py
+-rw-r--r--   0 root         (0) root         (0)    13492 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/elasticache/cache_subnet_group.py
+-rw-r--r--   0 root         (0) root         (0)    51005 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/elasticache/replication_group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.402671 idem-aws-2.0.0/idem_aws/states/aws/elb/
+-rw-r--r--   0 root         (0) root         (0)    19828 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/elb/load_balancer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.402671 idem-aws-2.0.0/idem_aws/states/aws/elbv2/
+-rw-r--r--   0 root         (0) root         (0)    32920 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/elbv2/listener.py
+-rw-r--r--   0 root         (0) root         (0)    24159 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/elbv2/load_balancer.py
+-rw-r--r--   0 root         (0) root         (0)    30475 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/elbv2/target_group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.402671 idem-aws-2.0.0/idem_aws/states/aws/es/
+-rw-r--r--   0 root         (0) root         (0)    36336 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/es/elasticsearch_domain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.402671 idem-aws-2.0.0/idem_aws/states/aws/events/
+-rw-r--r--   0 root         (0) root         (0)    45263 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/events/rule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.406671 idem-aws-2.0.0/idem_aws/states/aws/guardduty/
+-rw-r--r--   0 root         (0) root         (0)    15458 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/guardduty/detector.py
+-rw-r--r--   0 root         (0) root         (0)    10351 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/guardduty/member.py
+-rw-r--r--   0 root         (0) root         (0)     8768 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/guardduty/organization_admin_account.py
+-rw-r--r--   0 root         (0) root         (0)     8981 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/guardduty/organization_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.406671 idem-aws-2.0.0/idem_aws/states/aws/iam/
+-rw-r--r--   0 root         (0) root         (0)     9988 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/iam/access_key.py
+-rw-r--r--   0 root         (0) root         (0)     8246 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/iam/group.py
+-rw-r--r--   0 root         (0) root         (0)     8179 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/iam/group_membership.py
+-rw-r--r--   0 root         (0) root         (0)     8776 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/iam/group_policy_attachment.py
+-rw-r--r--   0 root         (0) root         (0)    14496 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/iam/instance_profile.py
+-rw-r--r--   0 root         (0) root         (0)    18389 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/iam/open_id_connect_provider.py
+-rw-r--r--   0 root         (0) root         (0)    12320 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/iam/password_policy.py
+-rw-r--r--   0 root         (0) root         (0)    14613 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/iam/policy.py
+-rw-r--r--   0 root         (0) root         (0)    22432 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/iam/role.py
+-rw-r--r--   0 root         (0) root         (0)    14538 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/iam/role_policy.py
+-rw-r--r--   0 root         (0) root         (0)    10537 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/iam/role_policy_attachment.py
+-rw-r--r--   0 root         (0) root         (0)    15633 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/iam/service_linked_role.py
+-rw-r--r--   0 root         (0) root         (0)    15522 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/iam/user.py
+-rw-r--r--   0 root         (0) root         (0)    14080 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/iam/user_policy.py
+-rw-r--r--   0 root         (0) root         (0)    11044 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/iam/user_policy_attachment.py
+-rw-r--r--   0 root         (0) root         (0)    13341 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/iam/user_ssh_key.py
+-rw-r--r--   0 root         (0) root         (0)      169 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.406671 idem-aws-2.0.0/idem_aws/states/aws/kinesis/
+-rw-r--r--   0 root         (0) root         (0)    24114 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/kinesis/stream.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.406671 idem-aws-2.0.0/idem_aws/states/aws/kms/
+-rw-r--r--   0 root         (0) root         (0)    10460 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/kms/alias.py
+-rw-r--r--   0 root         (0) root         (0)    22629 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/kms/key.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.406671 idem-aws-2.0.0/idem_aws/states/aws/lambda_aws/
+-rw-r--r--   0 root         (0) root         (0)    27963 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/lambda_aws/function.py
+-rw-r--r--   0 root         (0) root         (0)    11651 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/lambda_aws/function_event_invoke_config.py
+-rw-r--r--   0 root         (0) root         (0)    14029 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/lambda_aws/function_permission.py
+-rw-r--r--   0 root         (0) root         (0)    10018 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/lambda_aws/function_provisioned_concurrency_config.py
+-rw-r--r--   0 root         (0) root         (0)       27 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/lambda_aws/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.406671 idem-aws-2.0.0/idem_aws/states/aws/logs/
+-rw-r--r--   0 root         (0) root         (0)    12064 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/logs/subscription_filter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.406671 idem-aws-2.0.0/idem_aws/states/aws/neptune/
+-rw-r--r--   0 root         (0) root         (0)    32988 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/neptune/db_cluster.py
+-rw-r--r--   0 root         (0) root         (0)    13936 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/neptune/db_cluster_parameter_group.py
+-rw-r--r--   0 root         (0) root         (0)    37556 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/neptune/db_instance.py
+-rw-r--r--   0 root         (0) root         (0)    12467 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/neptune/db_parameter_group.py
+-rw-r--r--   0 root         (0) root         (0)    14288 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/neptune/db_subnet_group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.406671 idem-aws-2.0.0/idem_aws/states/aws/organizations/
+-rw-r--r--   0 root         (0) root         (0)    17382 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/organizations/account.py
+-rw-r--r--   0 root         (0) root         (0)     8251 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/organizations/organization.py
+-rw-r--r--   0 root         (0) root         (0)    14288 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/organizations/organization_unit.py
+-rw-r--r--   0 root         (0) root         (0)    13178 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/organizations/policy.py
+-rw-r--r--   0 root         (0) root         (0)    11399 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/organizations/policy_attachment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.406671 idem-aws-2.0.0/idem_aws/states/aws/rds/
+-rw-r--r--   0 root         (0) root         (0)    62077 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/rds/db_cluster.py
+-rw-r--r--   0 root         (0) root         (0)    14695 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/rds/db_cluster_parameter_group.py
+-rw-r--r--   0 root         (0) root         (0)    39434 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/rds/db_instance.py
+-rw-r--r--   0 root         (0) root         (0)    13874 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/rds/db_parameter_group.py
+-rw-r--r--   0 root         (0) root         (0)    14036 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/rds/db_subnet_group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.406671 idem-aws-2.0.0/idem_aws/states/aws/recursive_contracts/
+-rw-r--r--   0 root         (0) root         (0)       98 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/recursive_contracts/allow_sync_sls_name_and_name_tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.406671 idem-aws-2.0.0/idem_aws/states/aws/route53/
+-rw-r--r--   0 root         (0) root         (0)    19436 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/route53/hosted_zone.py
+-rw-r--r--   0 root         (0) root         (0)    14158 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/route53/hosted_zone_association.py
+-rw-r--r--   0 root         (0) root         (0)    12020 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/route53/resource_record.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.410671 idem-aws-2.0.0/idem_aws/states/aws/s3/
+-rw-r--r--   0 root         (0) root         (0)    19835 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/s3/bucket.py
+-rw-r--r--   0 root         (0) root         (0)    11122 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/s3/bucket_acl.py
+-rw-r--r--   0 root         (0) root         (0)    12547 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/s3/bucket_encryption.py
+-rw-r--r--   0 root         (0) root         (0)    26660 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/s3/bucket_lifecycle.py
+-rw-r--r--   0 root         (0) root         (0)    14837 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/s3/bucket_logging.py
+-rw-r--r--   0 root         (0) root         (0)    17615 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/s3/bucket_notification.py
+-rw-r--r--   0 root         (0) root         (0)    11941 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/s3/bucket_policy.py
+-rw-r--r--   0 root         (0) root         (0)    27930 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/s3/bucket_replication.py
+-rw-r--r--   0 root         (0) root         (0)    10328 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/s3/bucket_versioning.py
+-rw-r--r--   0 root         (0) root         (0)    22433 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/s3/bucket_website.py
+-rw-r--r--   0 root         (0) root         (0)    12854 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/s3/public_access_block.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.410671 idem-aws-2.0.0/idem_aws/states/aws/ses/
+-rw-r--r--   0 root         (0) root         (0)     6158 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/ses/domain_identity.py
+-rw-r--r--   0 root         (0) root         (0)    10385 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/ses/identity_notification_topic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.410671 idem-aws-2.0.0/idem_aws/states/aws/sesv2/
+-rw-r--r--   0 root         (0) root         (0)    14618 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/sesv2/event_destination.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.410671 idem-aws-2.0.0/idem_aws/states/aws/sns/
+-rw-r--r--   0 root         (0) root         (0)    11654 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/sns/subscription.py
+-rw-r--r--   0 root         (0) root         (0)    13240 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/sns/topic.py
+-rw-r--r--   0 root         (0) root         (0)     8686 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/sns/topic_policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.410671 idem-aws-2.0.0/idem_aws/states/aws/sqs/
+-rw-r--r--   0 root         (0) root         (0)    24692 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/sqs/queue.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.410671 idem-aws-2.0.0/idem_aws/states/aws/wafv2/
+-rw-r--r--   0 root         (0) root         (0)     9933 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/wafv2/associate_web_acl.py
+-rw-r--r--   0 root         (0) root         (0)    14712 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/wafv2/ip_set.py
+-rw-r--r--   0 root         (0) root         (0)    12255 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/wafv2/regex_pattern_set.py
+-rw-r--r--   0 root         (0) root         (0)   268538 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/states/aws/wafv2/web_acl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.386671 idem-aws-2.0.0/idem_aws/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.410671 idem-aws-2.0.0/idem_aws/tool/aws/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.410671 idem-aws-2.0.0/idem_aws/tool/aws/acct/
+-rw-r--r--   0 root         (0) root         (0)     1393 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/acct/assume_role.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.410671 idem-aws-2.0.0/idem_aws/tool/aws/acct/contracts/
+-rw-r--r--   0 root         (0) root         (0)      159 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/acct/contracts/init.py
+-rw-r--r--   0 root         (0) root         (0)      293 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/acct/esm.py
+-rw-r--r--   0 root         (0) root         (0)      714 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/acct/init.py
+-rw-r--r--   0 root         (0) root         (0)     1577 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/acct/key_name.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.410671 idem-aws-2.0.0/idem_aws/tool/aws/acm/
+-rw-r--r--   0 root         (0) root         (0)     2485 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/acm/certificate_validation_utils.py
+-rw-r--r--   0 root         (0) root         (0)     5339 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/acm/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2625 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/acm/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.414671 idem-aws-2.0.0/idem_aws/tool/aws/apigateway/
+-rw-r--r--   0 root         (0) root         (0)     3883 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/apigateway/base_path_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     3343 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/apigateway/deployment.py
+-rw-r--r--   0 root         (0) root         (0)     8767 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/apigateway/domain_name.py
+-rw-r--r--   0 root         (0) root         (0)     4535 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/apigateway/integration.py
+-rw-r--r--   0 root         (0) root         (0)     5000 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/apigateway/integration_response.py
+-rw-r--r--   0 root         (0) root         (0)     4226 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/apigateway/method.py
+-rw-r--r--   0 root         (0) root         (0)     4250 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/apigateway/method_response.py
+-rw-r--r--   0 root         (0) root         (0)     4087 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/apigateway/resource.py
+-rw-r--r--   0 root         (0) root         (0)     7175 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/apigateway/rest_api.py
+-rw-r--r--   0 root         (0) root         (0)     4417 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/apigateway/stage.py
+-rw-r--r--   0 root         (0) root         (0)     2203 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/apigateway/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.414671 idem-aws-2.0.0/idem_aws/tool/aws/apigatewayv2/
+-rw-r--r--   0 root         (0) root         (0)     5671 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/apigatewayv2/api.py
+-rw-r--r--   0 root         (0) root         (0)     5125 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/apigatewayv2/authorizer.py
+-rw-r--r--   0 root         (0) root         (0)     4842 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/apigatewayv2/domain_name.py
+-rw-r--r--   0 root         (0) root         (0)     5187 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/apigatewayv2/integration.py
+-rw-r--r--   0 root         (0) root         (0)     4793 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/apigatewayv2/route.py
+-rw-r--r--   0 root         (0) root         (0)     4061 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/apigatewayv2/stage.py
+-rw-r--r--   0 root         (0) root         (0)     2655 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/apigatewayv2/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.414671 idem-aws-2.0.0/idem_aws/tool/aws/application_autoscaling/
+-rw-r--r--   0 root         (0) root         (0)     2724 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/application_autoscaling/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1725 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/application_autoscaling/scalable_target.py
+-rw-r--r--   0 root         (0) root         (0)     1907 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/application_autoscaling/scaling_policy.py
+-rw-r--r--   0 root         (0) root         (0)     4099 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/arn_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.414671 idem-aws-2.0.0/idem_aws/tool/aws/autoscaling/
+-rw-r--r--   0 root         (0) root         (0)     5561 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/autoscaling/auto_scaling_group_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4257 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/autoscaling/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3367 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/autoscaling/scaling_policy.py
+-rw-r--r--   0 root         (0) root         (0)     2946 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/autoscaling/tag.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/b64.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.414671 idem-aws-2.0.0/idem_aws/tool/aws/backup/
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/backup/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2452 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/backup/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.414671 idem-aws-2.0.0/idem_aws/tool/aws/budgets/
+-rw-r--r--   0 root         (0) root         (0)     5249 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/budgets/budget.py
+-rw-r--r--   0 root         (0) root         (0)     3415 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/budgets/budget_action.py
+-rw-r--r--   0 root         (0) root         (0)     3563 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/budgets/conversion_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.414671 idem-aws-2.0.0/idem_aws/tool/aws/cloudformation/
+-rw-r--r--   0 root         (0) root         (0)    18904 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/cloudformation/stack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.414671 idem-aws-2.0.0/idem_aws/tool/aws/cloudfront/
+-rw-r--r--   0 root         (0) root         (0)     6468 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/cloudfront/cloudfront_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4860 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/cloudfront/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     7618 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/cloudfront/distribution.py
+-rw-r--r--   0 root         (0) root         (0)     2010 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/cloudfront/distribution_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2416 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/cloudfront/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.414671 idem-aws-2.0.0/idem_aws/tool/aws/cloudtrail/
+-rw-r--r--   0 root         (0) root         (0)     3966 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/cloudtrail/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)    13076 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/cloudtrail/trail.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.414671 idem-aws-2.0.0/idem_aws/tool/aws/cloudwatch/
+-rw-r--r--   0 root         (0) root         (0)     3540 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/cloudwatch/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)      807 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/cloudwatch/log_group.py
+-rw-r--r--   0 root         (0) root         (0)     4464 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/cloudwatch/metric_alarm.py
+-rw-r--r--   0 root         (0) root         (0)     2033 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/cloudwatch/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.414671 idem-aws-2.0.0/idem_aws/tool/aws/cloudwatchlogs/
+-rw-r--r--   0 root         (0) root         (0)      566 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/cloudwatchlogs/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3193 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/comment_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.414671 idem-aws-2.0.0/idem_aws/tool/aws/config/
+-rw-r--r--   0 root         (0) root         (0)     1511 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/config/config_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)     4483 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/config/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2032 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/config/delivery_channel.py
+-rw-r--r--   0 root         (0) root         (0)     2578 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/config/rule.py
+-rw-r--r--   0 root         (0) root         (0)     2434 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/config/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.414671 idem-aws-2.0.0/idem_aws/tool/aws/costexplorer/
+-rw-r--r--   0 root         (0) root         (0)     1024 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/costexplorer/anomaly_monitor.py
+-rw-r--r--   0 root         (0) root         (0)     3078 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/costexplorer/anomaly_subscription.py
+-rw-r--r--   0 root         (0) root         (0)     2953 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/costexplorer/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4859 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/costexplorer/cost_category.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.414671 idem-aws-2.0.0/idem_aws/tool/aws/docdb/
+-rw-r--r--   0 root         (0) root         (0)    12556 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/docdb/db_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     6638 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/docdb/db_cluster_parameter_group.py
+-rw-r--r--   0 root         (0) root         (0)     2668 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/docdb/db_subnet_group.py
+-rw-r--r--   0 root         (0) root         (0)     3183 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/docdb/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.414671 idem-aws-2.0.0/idem_aws/tool/aws/dynamodb/
+-rw-r--r--   0 root         (0) root         (0)    15451 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/dynamodb/table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.418671 idem-aws-2.0.0/idem_aws/tool/aws/ec2/
+-rw-r--r--   0 root         (0) root         (0)     3051 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ec2/ami.py
+-rw-r--r--   0 root         (0) root         (0)     2022 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ec2/availability_zones.py
+-rw-r--r--   0 root         (0) root         (0)    37825 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ec2/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ec2/dhcp_option_association_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1774 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ec2/elastic_ip.py
+-rw-r--r--   0 root         (0) root         (0)     1525 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ec2/flow_log.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.418671 idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/
+-rw-r--r--   0 root         (0) root         (0)     1280 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/data.py
+-rw-r--r--   0 root         (0) root         (0)     2910 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/key_pair.py
+-rw-r--r--   0 root         (0) root         (0)    19910 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/state.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.418671 idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/update/
+-rw-r--r--   0 root         (0) root         (0)     4440 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/update/block_device_mappings.py
+-rw-r--r--   0 root         (0) root         (0)     1813 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/update/bootstrap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.418671 idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/update/contracts/
+-rw-r--r--   0 root         (0) root         (0)      677 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/update/contracts/init.py
+-rw-r--r--   0 root         (0) root         (0)     1191 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/update/disable_api_termination.py
+-rw-r--r--   0 root         (0) root         (0)     1258 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/update/ebs_optimized.py
+-rw-r--r--   0 root         (0) root         (0)     2287 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/update/iam_instance_profile_arn.py
+-rw-r--r--   0 root         (0) root         (0)     8226 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/update/init.py
+-rw-r--r--   0 root         (0) root         (0)     1227 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/update/instance_initiated_shutdown_behavior.py
+-rw-r--r--   0 root         (0) root         (0)     1256 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/update/instance_type.py
+-rw-r--r--   0 root         (0) root         (0)     1300 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/update/kernel_id.py
+-rw-r--r--   0 root         (0) root         (0)     1154 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/update/monitoring_enabled.py
+-rw-r--r--   0 root         (0) root         (0)     4123 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/update/network_interfaces.py
+-rw-r--r--   0 root         (0) root         (0)     1656 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/update/placement.py
+-rw-r--r--   0 root         (0) root         (0)     1119 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/update/private_ip_address.py
+-rw-r--r--   0 root         (0) root         (0)     1313 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/update/ram_disk_id.py
+-rw-r--r--   0 root         (0) root         (0)      214 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/update/running.py
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/update/security_group_ids.py
+-rw-r--r--   0 root         (0) root         (0)     1173 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/update/source_dest_check.py
+-rw-r--r--   0 root         (0) root         (0)     1173 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/update/sriov_net_support.py
+-rw-r--r--   0 root         (0) root         (0)     1799 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/update/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1281 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/update/user_data.py
+-rw-r--r--   0 root         (0) root         (0)     4843 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ec2/internet_gateway.py
+-rw-r--r--   0 root         (0) root         (0)     1585 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ec2/key_pair.py
+-rw-r--r--   0 root         (0) root         (0)     3658 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ec2/launch_template.py
+-rw-r--r--   0 root         (0) root         (0)     3948 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ec2/network_interface.py
+-rw-r--r--   0 root         (0) root         (0)     1517 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ec2/placement_group.py
+-rw-r--r--   0 root         (0) root         (0)    12208 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ec2/route_table.py
+-rw-r--r--   0 root         (0) root         (0)     3924 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ec2/security_group_rule.py
+-rw-r--r--   0 root         (0) root         (0)     1801 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ec2/snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     2779 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ec2/spot_instance_request.py
+-rw-r--r--   0 root         (0) root         (0)    14415 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ec2/subnet.py
+-rw-r--r--   0 root         (0) root         (0)     2752 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ec2/tag.py
+-rw-r--r--   0 root         (0) root         (0)     3821 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ec2/transit_gateway.py
+-rw-r--r--   0 root         (0) root         (0)     3043 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ec2/transit_gateway_vpc_attachment.py
+-rw-r--r--   0 root         (0) root         (0)     1745 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ec2/volume.py
+-rw-r--r--   0 root         (0) root         (0)     7822 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ec2/vpc.py
+-rw-r--r--   0 root         (0) root         (0)     8498 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ec2/vpc_endpoint.py
+-rw-r--r--   0 root         (0) root         (0)    10282 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ec2/vpc_peering_connection_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.418671 idem-aws-2.0.0/idem_aws/tool/aws/ecr/
+-rw-r--r--   0 root         (0) root         (0)     4995 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ecr/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3190 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ecr/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.418671 idem-aws-2.0.0/idem_aws/tool/aws/efs/
+-rw-r--r--   0 root         (0) root         (0)     2368 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/efs/file_system_utils.py
+-rw-r--r--   0 root         (0) root         (0)      947 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/efs/mount_target_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1850 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/efs/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.418671 idem-aws-2.0.0/idem_aws/tool/aws/eks/
+-rw-r--r--   0 root         (0) root         (0)     4881 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/eks/addon.py
+-rw-r--r--   0 root         (0) root         (0)     9514 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/eks/cluster.py
+-rw-r--r--   0 root         (0) root         (0)     5220 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/eks/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4559 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/eks/eks_utils.py
+-rw-r--r--   0 root         (0) root         (0)     7710 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/eks/nodegroup.py
+-rw-r--r--   0 root         (0) root         (0)     1868 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/eks/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.422671 idem-aws-2.0.0/idem_aws/tool/aws/elasticache/
+-rw-r--r--   0 root         (0) root         (0)     9303 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/elasticache/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)    20325 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/elasticache/elasticache_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1737 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/elasticache/parameters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.422671 idem-aws-2.0.0/idem_aws/tool/aws/elb/
+-rw-r--r--   0 root         (0) root         (0)     1957 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/elb/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)    19196 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/elb/load_balancer.py
+-rw-r--r--   0 root         (0) root         (0)     2429 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/elb/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.422671 idem-aws-2.0.0/idem_aws/tool/aws/elbv2/
+-rw-r--r--   0 root         (0) root         (0)     7683 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/elbv2/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)    10904 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/elbv2/listener.py
+-rw-r--r--   0 root         (0) root         (0)    10107 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/elbv2/load_balancer.py
+-rw-r--r--   0 root         (0) root         (0)     2428 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/elbv2/tag.py
+-rw-r--r--   0 root         (0) root         (0)    10958 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/elbv2/target_group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.422671 idem-aws-2.0.0/idem_aws/tool/aws/es/
+-rw-r--r--   0 root         (0) root         (0)     9741 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/es/elasticsearch_domain.py
+-rw-r--r--   0 root         (0) root         (0)     2511 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/es/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.422671 idem-aws-2.0.0/idem_aws/tool/aws/events/
+-rw-r--r--   0 root         (0) root         (0)     1707 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/events/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     5958 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/events/rule.py
+-rw-r--r--   0 root         (0) root         (0)     2752 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/events/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.422671 idem-aws-2.0.0/idem_aws/tool/aws/guardduty/
+-rw-r--r--   0 root         (0) root         (0)     1048 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/guardduty/config_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3246 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/guardduty/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     7045 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/guardduty/detector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.422671 idem-aws-2.0.0/idem_aws/tool/aws/iam/
+-rw-r--r--   0 root         (0) root         (0)    12687 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/iam/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1649 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/iam/group.py
+-rw-r--r--   0 root         (0) root         (0)     2324 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/iam/group_membership.py
+-rw-r--r--   0 root         (0) root         (0)     2737 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/iam/password_policy.py
+-rw-r--r--   0 root         (0) root         (0)     7466 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/iam/policy.py
+-rw-r--r--   0 root         (0) root         (0)     1573 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/iam/role_policy_attachment.py
+-rw-r--r--   0 root         (0) root         (0)     1251 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/iam/service_linked_role.py
+-rw-r--r--   0 root         (0) root         (0)     3720 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/iam/user.py
+-rw-r--r--   0 root         (0) root         (0)     1486 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/iam/user_ssh_key.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.422671 idem-aws-2.0.0/idem_aws/tool/aws/kinesis/
+-rw-r--r--   0 root         (0) root         (0)     1976 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/kinesis/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)    21390 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/kinesis/stream.py
+-rw-r--r--   0 root         (0) root         (0)     2362 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/kinesis/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.422671 idem-aws-2.0.0/idem_aws/tool/aws/kms/
+-rw-r--r--   0 root         (0) root         (0)      999 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/kms/alias.py
+-rw-r--r--   0 root         (0) root         (0)     3196 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/kms/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3159 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/kms/key.py
+-rw-r--r--   0 root         (0) root         (0)     2060 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/kms/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.422671 idem-aws-2.0.0/idem_aws/tool/aws/lambda_aws/
+-rw-r--r--   0 root         (0) root         (0)     3194 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/lambda_aws/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)    16057 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/lambda_aws/function.py
+-rw-r--r--   0 root         (0) root         (0)     4274 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/lambda_aws/function_event_invoke_config.py
+-rw-r--r--   0 root         (0) root         (0)     2579 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/lambda_aws/function_permission.py
+-rw-r--r--   0 root         (0) root         (0)     1680 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/lambda_aws/function_provisioned_concurrency_config.py
+-rw-r--r--   0 root         (0) root         (0)       27 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/lambda_aws/init.py
+-rw-r--r--   0 root         (0) root         (0)     2689 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/lambda_aws/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.422671 idem-aws-2.0.0/idem_aws/tool/aws/logs/
+-rw-r--r--   0 root         (0) root         (0)     1336 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/logs/subscription_filter_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.422671 idem-aws-2.0.0/idem_aws/tool/aws/neptune/
+-rw-r--r--   0 root         (0) root         (0)     8991 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/neptune/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)    12251 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/neptune/db_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     6385 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/neptune/db_cluster_parameter_group.py
+-rw-r--r--   0 root         (0) root         (0)    11654 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/neptune/db_instance.py
+-rw-r--r--   0 root         (0) root         (0)     6128 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/neptune/db_parameter_group.py
+-rw-r--r--   0 root         (0) root         (0)     1546 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/neptune/db_subnet_group.py
+-rw-r--r--   0 root         (0) root         (0)     3258 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/neptune/tag.py
+-rw-r--r--   0 root         (0) root         (0)     2094 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/network_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.422671 idem-aws-2.0.0/idem_aws/tool/aws/organizations/
+-rw-r--r--   0 root         (0) root         (0)     1795 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/organizations/account.py
+-rw-r--r--   0 root         (0) root         (0)     4916 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/organizations/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1656 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/organizations/policy_attachment.py
+-rw-r--r--   0 root         (0) root         (0)     2704 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/organizations/tag.py
+-rw-r--r--   0 root         (0) root         (0)     1496 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/parameters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.426671 idem-aws-2.0.0/idem_aws/tool/aws/rds/
+-rw-r--r--   0 root         (0) root         (0)    12718 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/rds/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     5582 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/rds/parameters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.426671 idem-aws-2.0.0/idem_aws/tool/aws/route53/
+-rw-r--r--   0 root         (0) root         (0)     5018 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/route53/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1251 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/route53/hosted_zone_association.py
+-rw-r--r--   0 root         (0) root         (0)     5900 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/route53/hosted_zone_utils.py
+-rw-r--r--   0 root         (0) root         (0)     7422 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/route53/resource_record_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2663 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/route53/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.426671 idem-aws-2.0.0/idem_aws/tool/aws/s3/
+-rw-r--r--   0 root         (0) root         (0)     1526 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/s3/bucket_acl.py
+-rw-r--r--   0 root         (0) root         (0)     7925 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/s3/bucket_encryption.py
+-rw-r--r--   0 root         (0) root         (0)     7403 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/s3/bucket_lifecycle.py
+-rw-r--r--   0 root         (0) root         (0)     2440 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/s3/bucket_logging.py
+-rw-r--r--   0 root         (0) root         (0)     2584 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/s3/bucket_replication.py
+-rw-r--r--   0 root         (0) root         (0)     1050 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/s3/bucket_versioning.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/s3/bucket_website.py
+-rw-r--r--   0 root         (0) root         (0)     9894 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/s3/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3373 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/s3/s3_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1506 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/search_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.426671 idem-aws-2.0.0/idem_aws/tool/aws/ses/
+-rw-r--r--   0 root         (0) root         (0)     1214 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/ses/conversion_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.426671 idem-aws-2.0.0/idem_aws/tool/aws/sesv2/
+-rw-r--r--   0 root         (0) root         (0)      563 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/sesv2/conversion_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.426671 idem-aws-2.0.0/idem_aws/tool/aws/sns/
+-rw-r--r--   0 root         (0) root         (0)     3275 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/sns/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     7581 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/sns/sns_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.426671 idem-aws-2.0.0/idem_aws/tool/aws/sqs/
+-rw-r--r--   0 root         (0) root         (0)     6482 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/sqs/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     5455 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/sqs/queue_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3760 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/state_comparison_utils.py
+-rw-r--r--   0 root         (0) root         (0)      859 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/state_utils.py
+-rw-r--r--   0 root         (0) root         (0)      526 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/string_utils.py
+-rw-r--r--   0 root         (0) root         (0)     5900 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/tag_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1548 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/test_state_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.426671 idem-aws-2.0.0/idem_aws/tool/aws/wafv2/
+-rw-r--r--   0 root         (0) root         (0)     6843 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/wafv2/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3076 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/wafv2/ip_set_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1661 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/wafv2/regex_pattern_set.py
+-rw-r--r--   0 root         (0) root         (0)     3822 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/wafv2/tag.py
+-rw-r--r--   0 root         (0) root         (0)     2310 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/wafv2/web_acl.py
+-rw-r--r--   0 root         (0) root         (0)     1050 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/aws/waiter_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.426671 idem-aws-2.0.0/idem_aws/tool/boto3/
+-rw-r--r--   0 root         (0) root         (0)     5000 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/boto3/client.py
+-rw-r--r--   0 root         (0) root         (0)     5181 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/boto3/custom_waiter.py
+-rw-r--r--   0 root         (0) root         (0)      429 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/boto3/exception.py
+-rw-r--r--   0 root         (0) root         (0)      669 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/boto3/region.py
+-rw-r--r--   0 root         (0) root         (0)     6270 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/boto3/resolve.py
+-rw-r--r--   0 root         (0) root         (0)     5230 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/boto3/resource.py
+-rw-r--r--   0 root         (0) root         (0)     1411 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/boto3/session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.426671 idem-aws-2.0.0/idem_aws/tool/heist/
+-rw-r--r--   0 root         (0) root         (0)      906 2023-05-15 22:31:55.000000 idem-aws-2.0.0/idem_aws/tool/heist/bootstrap.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-15 22:32:08.000000 idem-aws-2.0.0/idem_aws/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 22:32:09.386671 idem-aws-2.0.0/idem_aws.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11102 2023-05-15 22:32:09.000000 idem-aws-2.0.0/idem_aws.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    22825 2023-05-15 22:32:09.000000 idem-aws-2.0.0/idem_aws.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 22:32:09.000000 idem-aws-2.0.0/idem_aws.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      608 2023-05-15 22:32:09.000000 idem-aws-2.0.0/idem_aws.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-15 22:32:09.000000 idem-aws-2.0.0/idem_aws.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      365 2023-05-15 22:31:55.000000 idem-aws-2.0.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 22:32:09.426671 idem-aws-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3186 2023-05-15 22:31:55.000000 idem-aws-2.0.0/setup.py
```

### Comparing `idem-aws-1.7.5/LICENSE` & `idem-aws-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/PKG-INFO` & `idem-aws-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: idem-aws
-Version: 1.7.5
+Version: 2.0.0
 Summary: AWS Cloud Provider for Idem
 Home-page: https://docs.idemproject.io/idem-aws/en/latest/index.html
 Author: VMware, Inc.
 Author-email: idemproject@vmware.com
 License: Apache Software License 2.0
 Project-URL: Code, https://gitlab.com/vmware/idem/idem-aws
 Project-URL: Issue tracker, https://gitlab.com/vmware/idem/idem-aws/issues
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: full
 Provides-Extra: bootstrap
 Provides-Extra: localstack
 Provides-Extra: google_auth
 Provides-Extra: autogen
 License-File: LICENSE
@@ -88,15 +89,15 @@
 
 Getting Started
 ===============
 
 Prerequisites
 -------------
 
-* Python 3.7+
+* Python 3.8+
 * git *(if installing from source, or contributing to the project)*
 
 Installation
 ------------
 
 .. note::
```

### Comparing `idem-aws-1.7.5/README.rst` & `idem-aws-2.0.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 Getting Started
 ===============
 
 Prerequisites
 -------------
 
-* Python 3.7+
+* Python 3.8+
 * git *(if installing from source, or contributing to the project)*
 
 Installation
 ------------
 
 .. note::
```

### Comparing `idem-aws-1.7.5/idem_aws/acct/aws/contracts/init.py` & `idem-aws-2.0.0/idem_aws/acct/aws/contracts/init.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/acct/aws/gsuite.py` & `idem-aws-2.0.0/idem_aws/acct/aws/gsuite.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/acct/aws/iam.py` & `idem-aws-2.0.0/idem_aws/acct/aws/iam.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/acct/aws/init.py` & `idem-aws-2.0.0/idem_aws/acct/aws/init.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/acct/metadata/aws.py` & `idem-aws-2.0.0/idem_aws/acct/metadata/aws.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/autogen/aws/function.py` & `idem-aws-2.0.0/idem_aws/autogen/aws/function.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/autogen/aws/init.py` & `idem-aws-2.0.0/idem_aws/autogen/aws/init.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/autogen/aws/param.py` & `idem-aws-2.0.0/idem_aws/autogen/aws/param.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/autogen/aws/plugin.py` & `idem-aws-2.0.0/idem_aws/autogen/aws/plugin.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/autogen/aws/possible_functions.py` & `idem-aws-2.0.0/idem_aws/autogen/aws/possible_functions.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/autogen/aws/resource.py` & `idem-aws-2.0.0/idem_aws/autogen/aws/resource.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/autogen/aws/service.py` & `idem-aws-2.0.0/idem_aws/autogen/aws/service.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/autogen/aws/tag/plugin.py` & `idem-aws-2.0.0/idem_aws/autogen/aws/tag/plugin.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/autogen/aws/tag/template.py` & `idem-aws-2.0.0/idem_aws/autogen/aws/tag/template.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/autogen/aws/template.py` & `idem-aws-2.0.0/idem_aws/autogen/aws/template.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/autogen/aws/utils/plugin.py` & `idem-aws-2.0.0/idem_aws/autogen/aws/utils/plugin.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/autogen/aws/utils/template.py` & `idem-aws-2.0.0/idem_aws/autogen/aws/utils/template.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/conf.py` & `idem-aws-2.0.0/idem_aws/conf.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/esm/aws.py` & `idem-aws-2.0.0/idem_aws/esm/aws.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import copy
 import json
 import pathlib
 from typing import Any
 from typing import Dict
 
 import botocore.exceptions
+from dict_tools.data import NamespaceDict
 
 
 def __init__(hub):
     hub.esm.aws.ACCT = ["aws"]
 
 
 async def get_state(hub, ctx) -> Dict[str, Any]:
@@ -96,14 +97,15 @@
     except Exception as e:
         hub.log.error(str(e))
         raise e
 
 
 async def generate_esm_profile(hub, ctx):
     esm_profile = ctx.acct.get("esm")
+    # If there was no esm profile in ACCT then get it purely from hub.OPT.extras.aws.esm
     if not esm_profile:
         if (
             "extras" in hub.OPT.acct
             and hub.OPT.acct.extras
             and "aws" in hub.OPT.acct.extras
         ):
             esm_profile = hub.OPT.acct.extras.aws.get("esm")
@@ -214,12 +216,12 @@
 
 
 def _populate_esm_ctx(esm_profile: dict, ctx: dict):
     # If esm has a region_name, we should use it when connecting to the dynamodb
     if esm_profile.get("region_name") is not None and esm_profile.get(
         "region_name"
     ) != ctx.get("acct", {}).get("region_name"):
-        esm_ctx = copy.deepcopy(ctx)
+        esm_ctx = NamespaceDict(copy.deepcopy(ctx))
         esm_ctx["acct"]["region_name"] = esm_profile.get("region_name")
         return esm_ctx
 
     return ctx
```

### Comparing `idem-aws-1.7.5/idem_aws/esm/contracts/aws.py` & `idem-aws-2.0.0/idem_aws/esm/contracts/aws.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/acm/certificate_manager.py` & `idem-aws-2.0.0/idem_aws/exec/aws/acm/certificate_manager.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/apigateway/base_path_mapping.py` & `idem-aws-2.0.0/idem_aws/exec/aws/apigateway/base_path_mapping.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/apigateway/deployment.py` & `idem-aws-2.0.0/idem_aws/exec/aws/apigateway/deployment.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/apigateway/domain_name.py` & `idem-aws-2.0.0/idem_aws/exec/aws/apigateway/domain_name.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/apigateway/integration.py` & `idem-aws-2.0.0/idem_aws/exec/aws/apigateway/integration.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/apigateway/integration_response.py` & `idem-aws-2.0.0/idem_aws/exec/aws/apigateway/integration_response.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/apigateway/method.py` & `idem-aws-2.0.0/idem_aws/exec/aws/apigateway/method.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/apigateway/method_response.py` & `idem-aws-2.0.0/idem_aws/exec/aws/apigateway/method_response.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/apigateway/resource.py` & `idem-aws-2.0.0/idem_aws/exec/aws/apigateway/resource.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/apigateway/rest_api.py` & `idem-aws-2.0.0/idem_aws/exec/aws/apigateway/rest_api.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/apigateway/stage.py` & `idem-aws-2.0.0/idem_aws/exec/aws/apigateway/stage.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/apigatewayv2/api.py` & `idem-aws-2.0.0/idem_aws/exec/aws/apigatewayv2/api.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/apigatewayv2/authorizer.py` & `idem-aws-2.0.0/idem_aws/exec/aws/apigatewayv2/authorizer.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/apigatewayv2/domain_name.py` & `idem-aws-2.0.0/idem_aws/exec/aws/apigatewayv2/domain_name.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/apigatewayv2/integration.py` & `idem-aws-2.0.0/idem_aws/exec/aws/apigatewayv2/integration.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/apigatewayv2/route.py` & `idem-aws-2.0.0/idem_aws/exec/aws/apigatewayv2/route.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/application_autoscaling/scalable_target.py` & `idem-aws-2.0.0/idem_aws/exec/aws/application_autoscaling/scalable_target.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/application_autoscaling/scaling_policy.py` & `idem-aws-2.0.0/idem_aws/exec/aws/application_autoscaling/scaling_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/arn.py` & `idem-aws-2.0.0/idem_aws/exec/aws/arn.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/autoscaling/scaling_policy.py` & `idem-aws-2.0.0/idem_aws/exec/aws/autoscaling/scaling_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/backup/backup_vault.py` & `idem-aws-2.0.0/idem_aws/exec/aws/backup/backup_vault.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/budgets/budget.py` & `idem-aws-2.0.0/idem_aws/exec/aws/budgets/budget.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/cloudformation/stack.py` & `idem-aws-2.0.0/idem_aws/exec/aws/cloudformation/stack.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/cloudfront/cache_policy.py` & `idem-aws-2.0.0/idem_aws/exec/aws/cloudfront/cache_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/cloudfront/distribution.py` & `idem-aws-2.0.0/idem_aws/exec/aws/cloudfront/distribution.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/cloudfront/origin_request_policy.py` & `idem-aws-2.0.0/idem_aws/exec/aws/cloudfront/origin_request_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/cloudwatch/log_group.py` & `idem-aws-2.0.0/idem_aws/exec/aws/cloudwatch/log_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/cloudwatchlogs/resource_policy.py` & `idem-aws-2.0.0/idem_aws/exec/aws/cloudwatchlogs/resource_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/config/configuration_aggregator.py` & `idem-aws-2.0.0/idem_aws/exec/aws/config/configuration_aggregator.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/costexplorer/cost_allocation_tag.py` & `idem-aws-2.0.0/idem_aws/exec/aws/costexplorer/cost_allocation_tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/data.py` & `idem-aws-2.0.0/idem_aws/exec/aws/data.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/docdb/db_cluster.py` & `idem-aws-2.0.0/idem_aws/exec/aws/docdb/db_cluster.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/docdb/db_cluster_parameter_group.py` & `idem-aws-2.0.0/idem_aws/exec/aws/docdb/db_cluster_parameter_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/docdb/db_subnet_group.py` & `idem-aws-2.0.0/idem_aws/exec/aws/docdb/db_subnet_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/dynamodb/table.py` & `idem-aws-2.0.0/idem_aws/exec/aws/dynamodb/table.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/dynamodb/tag.py` & `idem-aws-2.0.0/idem_aws/exec/aws/dynamodb/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/ec2/ami.py` & `idem-aws-2.0.0/idem_aws/exec/aws/ec2/ami.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/ec2/availability_zones.py` & `idem-aws-2.0.0/idem_aws/exec/aws/ec2/availability_zones.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/ec2/elastic_ip.py` & `idem-aws-2.0.0/idem_aws/exec/aws/ec2/elastic_ip.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/ec2/flow_log.py` & `idem-aws-2.0.0/idem_aws/exec/aws/ec2/flow_log.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/ec2/instance.py` & `idem-aws-2.0.0/idem_aws/exec/aws/ec2/instance.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/ec2/instance_type.py` & `idem-aws-2.0.0/idem_aws/exec/aws/ec2/instance_type.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/ec2/internet_gateway.py` & `idem-aws-2.0.0/idem_aws/exec/aws/ec2/internet_gateway.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/ec2/key_pair.py` & `idem-aws-2.0.0/idem_aws/exec/aws/ec2/key_pair.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/ec2/launch_template.py` & `idem-aws-2.0.0/idem_aws/exec/aws/ec2/launch_template.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/ec2/network_interface.py` & `idem-aws-2.0.0/idem_aws/exec/aws/ec2/network_interface.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,16 +40,23 @@
         )
     else:
         ret = await hub.exec.boto3.client.ec2.describe_network_interfaces(
             ctx,
             Filters=filters,
         )
 
-    # If there was an error in the call then report failure
     if not ret["result"]:
+        if "InvalidNetworkInterfaceID.NotFound" in str(ret["comment"]):
+            result["comment"].append(
+                hub.tool.aws.comment_utils.get_empty_comment(
+                    resource_type="aws.ec2.network_interface", name=name
+                )
+            )
+            result["comment"] += list(ret["comment"])
+            return result
         result["comment"] += list(ret["comment"])
         result["result"] = False
         return result
 
     present_states = hub.tool.aws.ec2.network_interface.convert_to_present(ret.ret)
 
     # If the resource can't be found but there were no results then "result" is True and "ret" is None
```

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/ec2/placement_group.py` & `idem-aws-2.0.0/idem_aws/exec/aws/ec2/placement_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/ec2/route.py` & `idem-aws-2.0.0/idem_aws/exec/aws/ec2/route.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/ec2/route_table.py` & `idem-aws-2.0.0/idem_aws/exec/aws/ec2/route_table.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/ec2/route_table_association.py` & `idem-aws-2.0.0/idem_aws/exec/aws/ec2/route_table_association.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/ec2/security_group.py` & `idem-aws-2.0.0/idem_aws/exec/aws/ec2/security_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/ec2/security_group_rule.py` & `idem-aws-2.0.0/idem_aws/exec/aws/ec2/security_group_rule.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/ec2/snapshot.py` & `idem-aws-2.0.0/idem_aws/exec/aws/ec2/snapshot.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/ec2/spot_instance_request.py` & `idem-aws-2.0.0/idem_aws/exec/aws/ec2/spot_instance_request.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/ec2/subnet.py` & `idem-aws-2.0.0/idem_aws/exec/aws/ec2/subnet.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/ec2/volume.py` & `idem-aws-2.0.0/idem_aws/exec/aws/ec2/volume.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/ec2/vpc.py` & `idem-aws-2.0.0/idem_aws/exec/aws/ec2/vpc.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/ec2/vpc_endpoint.py` & `idem-aws-2.0.0/idem_aws/exec/aws/ec2/vpc_endpoint.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/ec2/vpc_peering_connection.py` & `idem-aws-2.0.0/idem_aws/exec/aws/ec2/vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/ec2/vpc_peering_connection_accepter.py` & `idem-aws-2.0.0/idem_aws/exec/aws/ec2/vpc_peering_connection_accepter.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/ec2/vpc_peering_connection_options.py` & `idem-aws-2.0.0/idem_aws/exec/aws/ec2/vpc_peering_connection_options.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/ecr/image.py` & `idem-aws-2.0.0/idem_aws/exec/aws/ecr/image.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/ecr/lifecycle_policy.py` & `idem-aws-2.0.0/idem_aws/exec/aws/ecr/lifecycle_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/ecr/repository.py` & `idem-aws-2.0.0/idem_aws/exec/aws/ecr/repository.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/ecr/repository_policy.py` & `idem-aws-2.0.0/idem_aws/exec/aws/ecr/repository_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/eks/cluster.py` & `idem-aws-2.0.0/idem_aws/exec/aws/eks/cluster.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/elasticache/replication_group.py` & `idem-aws-2.0.0/idem_aws/exec/aws/elasticache/replication_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/elb/elb_hosted_zone_id.py` & `idem-aws-2.0.0/idem_aws/exec/aws/elb/elb_hosted_zone_id.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/elb/load_balancer.py` & `idem-aws-2.0.0/idem_aws/exec/aws/elb/load_balancer.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/elbv2/listener.py` & `idem-aws-2.0.0/idem_aws/exec/aws/elbv2/listener.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/elbv2/load_balancer.py` & `idem-aws-2.0.0/idem_aws/exec/aws/elbv2/load_balancer.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/elbv2/target_group.py` & `idem-aws-2.0.0/idem_aws/exec/aws/elbv2/target_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/es/elasticsearch_domain.py` & `idem-aws-2.0.0/idem_aws/exec/aws/es/elasticsearch_domain.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/events/rule.py` & `idem-aws-2.0.0/idem_aws/exec/aws/events/rule.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/guardduty/detector.py` & `idem-aws-2.0.0/idem_aws/exec/aws/guardduty/detector.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/guardduty/member.py` & `idem-aws-2.0.0/idem_aws/exec/aws/guardduty/member.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/guardduty/organization_admin_account.py` & `idem-aws-2.0.0/idem_aws/exec/aws/guardduty/organization_admin_account.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/guardduty/organization_configuration.py` & `idem-aws-2.0.0/idem_aws/exec/aws/guardduty/organization_configuration.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/iam/access_key.py` & `idem-aws-2.0.0/idem_aws/exec/aws/iam/access_key.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/iam/group.py` & `idem-aws-2.0.0/idem_aws/exec/aws/iam/group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/iam/group_membership.py` & `idem-aws-2.0.0/idem_aws/exec/aws/iam/group_membership.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/iam/group_policy_attachment.py` & `idem-aws-2.0.0/idem_aws/exec/aws/iam/group_policy_attachment.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/iam/instance_profile.py` & `idem-aws-2.0.0/idem_aws/exec/aws/iam/instance_profile.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/iam/open_id_connect_provider.py` & `idem-aws-2.0.0/idem_aws/exec/aws/iam/open_id_connect_provider.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/iam/password_policy.py` & `idem-aws-2.0.0/idem_aws/exec/aws/iam/password_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/iam/policy.py` & `idem-aws-2.0.0/idem_aws/exec/aws/iam/policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/iam/role.py` & `idem-aws-2.0.0/idem_aws/exec/aws/iam/role.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/iam/user.py` & `idem-aws-2.0.0/idem_aws/exec/aws/iam/user.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/iam/user_policy_attachment.py` & `idem-aws-2.0.0/idem_aws/exec/aws/iam/user_policy_attachment.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/kinesis/stream.py` & `idem-aws-2.0.0/idem_aws/exec/aws/kinesis/stream.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/kms/key.py` & `idem-aws-2.0.0/idem_aws/exec/aws/kms/key.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/lambda_aws/function_event_invoke_config.py` & `idem-aws-2.0.0/idem_aws/exec/aws/lambda_aws/function_event_invoke_config.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/lambda_aws/function_provisioned_concurrency_config.py` & `idem-aws-2.0.0/idem_aws/exec/aws/lambda_aws/function_provisioned_concurrency_config.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/neptune/db_cluster_parameter_group.py` & `idem-aws-2.0.0/idem_aws/exec/aws/neptune/db_cluster_parameter_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/neptune/db_instance.py` & `idem-aws-2.0.0/idem_aws/exec/aws/neptune/db_instance.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/neptune/db_parameter_group.py` & `idem-aws-2.0.0/idem_aws/exec/aws/neptune/db_parameter_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/organizations/account.py` & `idem-aws-2.0.0/idem_aws/exec/aws/organizations/account.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/organizations/policy.py` & `idem-aws-2.0.0/idem_aws/exec/aws/organizations/policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/rds/db_cluster.py` & `idem-aws-2.0.0/idem_aws/exec/aws/rds/db_cluster.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/rds/db_cluster_parameter_group.py` & `idem-aws-2.0.0/idem_aws/exec/aws/rds/db_cluster_parameter_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/rds/db_instance.py` & `idem-aws-2.0.0/idem_aws/exec/aws/rds/db_instance.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/rds/db_parameter_group.py` & `idem-aws-2.0.0/idem_aws/exec/aws/rds/db_parameter_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/rds/db_subnet_group.py` & `idem-aws-2.0.0/idem_aws/exec/aws/rds/db_subnet_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/rds/tag.py` & `idem-aws-2.0.0/idem_aws/exec/aws/rds/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/route53/hosted_zone.py` & `idem-aws-2.0.0/idem_aws/exec/aws/route53/hosted_zone.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/s3/bucket.py` & `idem-aws-2.0.0/idem_aws/exec/aws/s3/bucket.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/s3/bucket_acl.py` & `idem-aws-2.0.0/idem_aws/exec/aws/s3/bucket_acl.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/s3/bucket_lifecycle.py` & `idem-aws-2.0.0/idem_aws/exec/aws/s3/bucket_lifecycle.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/s3/bucket_logging.py` & `idem-aws-2.0.0/idem_aws/exec/aws/s3/bucket_logging.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/s3/bucket_replication.py` & `idem-aws-2.0.0/idem_aws/exec/aws/s3/bucket_replication.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/s3/bucket_website.py` & `idem-aws-2.0.0/idem_aws/exec/aws/s3/bucket_website.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/ses/domain_identity.py` & `idem-aws-2.0.0/idem_aws/exec/aws/ses/domain_identity.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/ses/identity_notification_topic.py` & `idem-aws-2.0.0/idem_aws/exec/aws/ses/identity_notification_topic.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/sesv2/event_destination.py` & `idem-aws-2.0.0/idem_aws/exec/aws/sesv2/event_destination.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/sns/subscription.py` & `idem-aws-2.0.0/idem_aws/exec/aws/sns/subscription.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/sqs/queue.py` & `idem-aws-2.0.0/idem_aws/exec/aws/sqs/queue.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/sts/assume_role.py` & `idem-aws-2.0.0/idem_aws/exec/aws/sts/assume_role.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/sts/caller_identity.py` & `idem-aws-2.0.0/idem_aws/exec/aws/sts/caller_identity.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/wafv2/ip_set.py` & `idem-aws-2.0.0/idem_aws/exec/aws/wafv2/ip_set.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/aws/wafv2/regex_pattern_set.py` & `idem-aws-2.0.0/idem_aws/exec/aws/wafv2/regex_pattern_set.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/exec/boto3/init.py` & `idem-aws-2.0.0/idem_aws/exec/boto3/init.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/reconcile/pending/aws.py` & `idem-aws-2.0.0/idem_aws/reconcile/pending/aws.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/acm/certificate_manager.py` & `idem-aws-2.0.0/idem_aws/states/aws/acm/certificate_manager.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/acm/certificate_validation.py` & `idem-aws-2.0.0/idem_aws/states/aws/acm/certificate_validation.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/apigateway/base_path_mapping.py` & `idem-aws-2.0.0/idem_aws/states/aws/apigateway/base_path_mapping.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/apigateway/deployment.py` & `idem-aws-2.0.0/idem_aws/states/aws/apigateway/deployment.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/apigateway/domain_name.py` & `idem-aws-2.0.0/idem_aws/states/aws/apigateway/domain_name.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/apigateway/integration.py` & `idem-aws-2.0.0/idem_aws/states/aws/apigateway/integration.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/apigateway/integration_response.py` & `idem-aws-2.0.0/idem_aws/states/aws/apigateway/integration_response.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/apigateway/method.py` & `idem-aws-2.0.0/idem_aws/states/aws/apigateway/method.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/apigateway/method_response.py` & `idem-aws-2.0.0/idem_aws/states/aws/apigateway/method_response.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/apigateway/resource.py` & `idem-aws-2.0.0/idem_aws/states/aws/apigateway/resource.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/apigateway/rest_api.py` & `idem-aws-2.0.0/idem_aws/states/aws/apigateway/rest_api.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/apigateway/stage.py` & `idem-aws-2.0.0/idem_aws/states/aws/apigateway/stage.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/apigatewayv2/api.py` & `idem-aws-2.0.0/idem_aws/states/aws/apigatewayv2/api.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/apigatewayv2/authorizer.py` & `idem-aws-2.0.0/idem_aws/states/aws/apigatewayv2/authorizer.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/apigatewayv2/domain_name.py` & `idem-aws-2.0.0/idem_aws/states/aws/apigatewayv2/domain_name.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/apigatewayv2/integration.py` & `idem-aws-2.0.0/idem_aws/states/aws/apigatewayv2/integration.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/apigatewayv2/route.py` & `idem-aws-2.0.0/idem_aws/states/aws/apigatewayv2/route.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/apigatewayv2/stage.py` & `idem-aws-2.0.0/idem_aws/states/aws/apigatewayv2/stage.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/application_autoscaling/scalable_target.py` & `idem-aws-2.0.0/idem_aws/states/aws/application_autoscaling/scalable_target.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/application_autoscaling/scaling_policy.py` & `idem-aws-2.0.0/idem_aws/states/aws/application_autoscaling/scaling_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/autoscaling/auto_scaling_group.py` & `idem-aws-2.0.0/idem_aws/states/aws/autoscaling/auto_scaling_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/autoscaling/launch_configuration.py` & `idem-aws-2.0.0/idem_aws/states/aws/autoscaling/launch_configuration.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/autoscaling/scaling_policy.py` & `idem-aws-2.0.0/idem_aws/states/aws/autoscaling/scaling_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/backup/backup_vault.py` & `idem-aws-2.0.0/idem_aws/states/aws/backup/backup_vault.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/budgets/budget.py` & `idem-aws-2.0.0/idem_aws/states/aws/budgets/budget.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/budgets/budget_action.py` & `idem-aws-2.0.0/idem_aws/states/aws/budgets/budget_action.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/caller_identity.py` & `idem-aws-2.0.0/idem_aws/states/aws/caller_identity.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/cloudformation/stack.py` & `idem-aws-2.0.0/idem_aws/states/aws/cloudformation/stack.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/cloudfront/cache_policy.py` & `idem-aws-2.0.0/idem_aws/states/aws/cloudfront/cache_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/cloudfront/distribution.py` & `idem-aws-2.0.0/idem_aws/states/aws/cloudfront/distribution.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/cloudfront/origin_request_policy.py` & `idem-aws-2.0.0/idem_aws/states/aws/cloudfront/origin_request_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/cloudtrail/trail.py` & `idem-aws-2.0.0/idem_aws/states/aws/cloudtrail/trail.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/cloudwatch/log_group.py` & `idem-aws-2.0.0/idem_aws/states/aws/cloudwatch/log_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/cloudwatch/metric_alarm.py` & `idem-aws-2.0.0/idem_aws/states/aws/cloudwatch/metric_alarm.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/cloudwatchlogs/resource_policy.py` & `idem-aws-2.0.0/idem_aws/states/aws/cloudwatchlogs/resource_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/config/config_recorder.py` & `idem-aws-2.0.0/idem_aws/states/aws/config/config_recorder.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/config/config_recorder_status.py` & `idem-aws-2.0.0/idem_aws/states/aws/config/config_recorder_status.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/config/configuration_aggregator.py` & `idem-aws-2.0.0/idem_aws/states/aws/config/configuration_aggregator.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/config/delivery_channel.py` & `idem-aws-2.0.0/idem_aws/states/aws/config/delivery_channel.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/config/rule.py` & `idem-aws-2.0.0/idem_aws/states/aws/config/rule.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/costexplorer/anomaly_monitor.py` & `idem-aws-2.0.0/idem_aws/states/aws/costexplorer/anomaly_monitor.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/costexplorer/anomaly_subscription.py` & `idem-aws-2.0.0/idem_aws/states/aws/costexplorer/anomaly_subscription.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/costexplorer/cost_category.py` & `idem-aws-2.0.0/idem_aws/states/aws/costexplorer/cost_category.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/data.py` & `idem-aws-2.0.0/idem_aws/states/aws/data.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/docdb/db_cluster.py` & `idem-aws-2.0.0/idem_aws/states/aws/docdb/db_cluster.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/docdb/db_cluster_parameter_group.py` & `idem-aws-2.0.0/idem_aws/states/aws/docdb/db_cluster_parameter_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/docdb/db_subnet_group.py` & `idem-aws-2.0.0/idem_aws/states/aws/docdb/db_subnet_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/dynamodb/table.py` & `idem-aws-2.0.0/idem_aws/states/aws/dynamodb/table.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/ec2/ami.py` & `idem-aws-2.0.0/idem_aws/states/aws/ec2/ami.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/ec2/dhcp_option.py` & `idem-aws-2.0.0/idem_aws/states/aws/ec2/dhcp_option.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/ec2/dhcp_option_association.py` & `idem-aws-2.0.0/idem_aws/states/aws/ec2/dhcp_option_association.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/ec2/elastic_ip.py` & `idem-aws-2.0.0/idem_aws/states/aws/ec2/elastic_ip.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/ec2/flow_log.py` & `idem-aws-2.0.0/idem_aws/states/aws/ec2/flow_log.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/ec2/instance.py` & `idem-aws-2.0.0/idem_aws/states/aws/ec2/instance.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/ec2/internet_gateway.py` & `idem-aws-2.0.0/idem_aws/states/aws/ec2/internet_gateway.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/ec2/key_pair.py` & `idem-aws-2.0.0/idem_aws/states/aws/ec2/key_pair.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/ec2/launch_template.py` & `idem-aws-2.0.0/idem_aws/states/aws/ec2/launch_template.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/ec2/nat_gateway.py` & `idem-aws-2.0.0/idem_aws/states/aws/ec2/nat_gateway.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/ec2/network_interface.py` & `idem-aws-2.0.0/idem_aws/states/aws/ec2/network_interface.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/ec2/placement_group.py` & `idem-aws-2.0.0/idem_aws/states/aws/ec2/placement_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/ec2/route.py` & `idem-aws-2.0.0/idem_aws/states/aws/ec2/route.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/ec2/route_table.py` & `idem-aws-2.0.0/idem_aws/states/aws/ec2/route_table.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/ec2/route_table_association.py` & `idem-aws-2.0.0/idem_aws/states/aws/ec2/route_table_association.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/ec2/security_group.py` & `idem-aws-2.0.0/idem_aws/states/aws/ec2/security_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/ec2/security_group_rule.py` & `idem-aws-2.0.0/idem_aws/states/aws/ec2/security_group_rule.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/ec2/snapshot.py` & `idem-aws-2.0.0/idem_aws/states/aws/ec2/snapshot.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/ec2/spot_instance_request.py` & `idem-aws-2.0.0/idem_aws/states/aws/ec2/spot_instance_request.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/ec2/subnet.py` & `idem-aws-2.0.0/idem_aws/states/aws/ec2/subnet.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/ec2/transit_gateway.py` & `idem-aws-2.0.0/idem_aws/states/aws/ec2/transit_gateway.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/ec2/transit_gateway_vpc_attachment.py` & `idem-aws-2.0.0/idem_aws/states/aws/ec2/transit_gateway_vpc_attachment.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/ec2/volume.py` & `idem-aws-2.0.0/idem_aws/states/aws/ec2/volume.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/ec2/vpc.py` & `idem-aws-2.0.0/idem_aws/states/aws/ec2/vpc.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/ec2/vpc_endpoint.py` & `idem-aws-2.0.0/idem_aws/states/aws/ec2/vpc_endpoint.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/ec2/vpc_peering_connection.py` & `idem-aws-2.0.0/idem_aws/states/aws/ec2/vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/ec2/vpc_peering_connection_accepter.py` & `idem-aws-2.0.0/idem_aws/states/aws/ec2/vpc_peering_connection_accepter.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/ec2/vpc_peering_connection_options.py` & `idem-aws-2.0.0/idem_aws/states/aws/ec2/vpc_peering_connection_options.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/ecr/lifecycle_policy.py` & `idem-aws-2.0.0/idem_aws/states/aws/ecr/lifecycle_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/ecr/repository.py` & `idem-aws-2.0.0/idem_aws/states/aws/ecr/repository.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/ecr/repository_policy.py` & `idem-aws-2.0.0/idem_aws/states/aws/ecr/repository_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/efs/file_system.py` & `idem-aws-2.0.0/idem_aws/states/aws/efs/file_system.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/efs/mount_target.py` & `idem-aws-2.0.0/idem_aws/states/aws/efs/mount_target.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/eks/addon.py` & `idem-aws-2.0.0/idem_aws/states/aws/eks/addon.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/eks/cluster.py` & `idem-aws-2.0.0/idem_aws/states/aws/eks/cluster.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/eks/fargate_profile.py` & `idem-aws-2.0.0/idem_aws/states/aws/eks/fargate_profile.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/eks/nodegroup.py` & `idem-aws-2.0.0/idem_aws/states/aws/eks/nodegroup.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/elasticache/cache_parameter_group.py` & `idem-aws-2.0.0/idem_aws/states/aws/elasticache/cache_parameter_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/elasticache/cache_subnet_group.py` & `idem-aws-2.0.0/idem_aws/states/aws/elasticache/cache_subnet_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/elasticache/replication_group.py` & `idem-aws-2.0.0/idem_aws/states/aws/elasticache/replication_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/elb/load_balancer.py` & `idem-aws-2.0.0/idem_aws/states/aws/elb/load_balancer.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/elbv2/listener.py` & `idem-aws-2.0.0/idem_aws/states/aws/elbv2/listener.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/elbv2/load_balancer.py` & `idem-aws-2.0.0/idem_aws/states/aws/elbv2/load_balancer.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/elbv2/target_group.py` & `idem-aws-2.0.0/idem_aws/states/aws/elbv2/target_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/es/elasticsearch_domain.py` & `idem-aws-2.0.0/idem_aws/states/aws/es/elasticsearch_domain.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/events/rule.py` & `idem-aws-2.0.0/idem_aws/states/aws/events/rule.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/guardduty/detector.py` & `idem-aws-2.0.0/idem_aws/states/aws/guardduty/detector.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/guardduty/member.py` & `idem-aws-2.0.0/idem_aws/states/aws/guardduty/member.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/guardduty/organization_admin_account.py` & `idem-aws-2.0.0/idem_aws/states/aws/guardduty/organization_admin_account.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/guardduty/organization_configuration.py` & `idem-aws-2.0.0/idem_aws/states/aws/guardduty/organization_configuration.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/iam/access_key.py` & `idem-aws-2.0.0/idem_aws/states/aws/iam/access_key.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/iam/group.py` & `idem-aws-2.0.0/idem_aws/states/aws/iam/group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/iam/group_membership.py` & `idem-aws-2.0.0/idem_aws/states/aws/iam/group_membership.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/iam/group_policy_attachment.py` & `idem-aws-2.0.0/idem_aws/states/aws/iam/group_policy_attachment.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/iam/instance_profile.py` & `idem-aws-2.0.0/idem_aws/states/aws/iam/instance_profile.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/iam/open_id_connect_provider.py` & `idem-aws-2.0.0/idem_aws/states/aws/iam/open_id_connect_provider.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/iam/password_policy.py` & `idem-aws-2.0.0/idem_aws/states/aws/iam/password_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/iam/policy.py` & `idem-aws-2.0.0/idem_aws/states/aws/iam/policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/iam/role.py` & `idem-aws-2.0.0/idem_aws/states/aws/iam/role.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/iam/role_policy.py` & `idem-aws-2.0.0/idem_aws/states/aws/iam/role_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/iam/role_policy_attachment.py` & `idem-aws-2.0.0/idem_aws/states/aws/iam/role_policy_attachment.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/iam/service_linked_role.py` & `idem-aws-2.0.0/idem_aws/states/aws/iam/service_linked_role.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/iam/user.py` & `idem-aws-2.0.0/idem_aws/states/aws/iam/user.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/iam/user_policy.py` & `idem-aws-2.0.0/idem_aws/states/aws/iam/user_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/iam/user_policy_attachment.py` & `idem-aws-2.0.0/idem_aws/states/aws/iam/user_policy_attachment.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/iam/user_ssh_key.py` & `idem-aws-2.0.0/idem_aws/states/aws/iam/user_ssh_key.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/kinesis/stream.py` & `idem-aws-2.0.0/idem_aws/states/aws/kinesis/stream.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/kms/alias.py` & `idem-aws-2.0.0/idem_aws/states/aws/kms/alias.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/kms/key.py` & `idem-aws-2.0.0/idem_aws/states/aws/kms/key.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/lambda_aws/function.py` & `idem-aws-2.0.0/idem_aws/states/aws/lambda_aws/function.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/lambda_aws/function_event_invoke_config.py` & `idem-aws-2.0.0/idem_aws/states/aws/lambda_aws/function_event_invoke_config.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/lambda_aws/function_permission.py` & `idem-aws-2.0.0/idem_aws/states/aws/lambda_aws/function_permission.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/lambda_aws/function_provisioned_concurrency_config.py` & `idem-aws-2.0.0/idem_aws/states/aws/lambda_aws/function_provisioned_concurrency_config.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/logs/subscription_filter.py` & `idem-aws-2.0.0/idem_aws/states/aws/logs/subscription_filter.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/neptune/db_cluster.py` & `idem-aws-2.0.0/idem_aws/states/aws/neptune/db_cluster.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/neptune/db_cluster_parameter_group.py` & `idem-aws-2.0.0/idem_aws/states/aws/neptune/db_cluster_parameter_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/neptune/db_instance.py` & `idem-aws-2.0.0/idem_aws/states/aws/neptune/db_instance.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/neptune/db_parameter_group.py` & `idem-aws-2.0.0/idem_aws/states/aws/neptune/db_parameter_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/neptune/db_subnet_group.py` & `idem-aws-2.0.0/idem_aws/states/aws/neptune/db_subnet_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/organizations/account.py` & `idem-aws-2.0.0/idem_aws/states/aws/organizations/account.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/organizations/organization.py` & `idem-aws-2.0.0/idem_aws/states/aws/organizations/organization.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/organizations/organization_unit.py` & `idem-aws-2.0.0/idem_aws/states/aws/organizations/organization_unit.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/organizations/policy.py` & `idem-aws-2.0.0/idem_aws/states/aws/organizations/policy.py`

 * *Files 6% similar despite different names*

```diff
@@ -107,14 +107,17 @@
 
     if isinstance(tags, List):
         tags = hub.tool.aws.tag_utils.convert_tag_list_to_dict(tags)
     change_dict = dict(Name=None, Description=None, Content=None)
 
     resource_updated = False
 
+    # Standardise on the json format
+    content = hub.tool.aws.state_comparison_utils.standardise_json(content)
+
     if before:
         result["comment"] = hub.tool.aws.comment_utils.already_exists_comment(
             resource_type="aws.organizations.policy", name=name
         )
         result["old_state"] = copy.deepcopy(before["ret"])
         plan_state = copy.deepcopy(result["old_state"])
 
@@ -124,15 +127,17 @@
 
             if before["ret"]["name"] != name:
                 change_dict["Name"] = name
 
             if before["ret"]["description"] != description:
                 change_dict["Description"] = description
 
-            if before["ret"]["content"] != content:
+            if not hub.tool.aws.state_comparison_utils.is_json_identical(
+                before["ret"]["content"], content
+            ):
                 change_dict["Content"] = content
 
             if any(value is not None for value in change_dict.values()):
 
                 if ctx.get("test", False):
                     plan_state["resource_id"] = resource_id
                     if change_dict.get("Name"):
@@ -160,17 +165,15 @@
                     if not update_policy_ret["result"]:
                         result["comment"] = (
                             result["comment"] + update_policy_ret["comment"]
                         )
                         result["result"] = update_policy_ret["result"]
                         return result
                     resource_updated = True
-                    result["comment"] = result["comment"] + (
-                        f"Updated aws.organizations.policy '{name}'",
-                    )
+                    result["comment"] += (f"Updated aws.organizations.policy '{name}'",)
 
             # Update tags
             if (tags is not None) and tags != result["old_state"].get("tags"):
                 update_ret = await hub.tool.aws.organizations.tag.update_tags(
                     ctx,
                     resource_id=resource_id,
                     old_tags=result["old_state"].get("tags"),
@@ -180,15 +183,15 @@
                 result["comment"] = result["comment"] + update_ret["comment"]
                 resource_updated = resource_updated or bool(update_ret["result"])
                 if ctx.get("test", False) and update_ret["ret"] is not None:
                     plan_state["tags"] = update_ret["ret"]
 
         except hub.tool.boto3.exception.ClientError as e:
             result["result"] = False
-            result["comment"] = result["comment"] + (f"{e.__class__.__name__}: {e}",)
+            result["comment"] += (f"{e.__class__.__name__}: {e}",)
 
     else:
         # Policy does not exist , create
         if ctx.get("test", False):
             result["new_state"] = hub.tool.aws.test_state_utils.generate_test_state(
                 enforced_state={},
                 desired_state={
@@ -352,40 +355,25 @@
 
         if list_policies["ret"]["Policies"]:
             list_all_policies.extend(list_policies["ret"]["Policies"])
 
     for policy in list_all_policies:
         policy_id = policy["Id"]
 
-        policy_ret = await hub.exec.boto3.client.organizations.describe_policy(
-            ctx, PolicyId=policy_id
+        policy_ret = await hub.exec.aws.organizations.policy.get(
+            ctx, resource_id=policy_id
         )
 
-        if not policy_ret and not policy_ret["ret"]:
-            hub.log.debug(
-                f"Could not describe '{policy_id}' with error: {policy_ret['comment']}"
+        if not policy_ret["result"]:
+            hub.log.info(
+                f"Failed to retrieve aws.organizations.policy with id {policy_id}"
             )
             continue
 
-        tags_ret = await hub.exec.boto3.client.organizations.list_tags_for_resource(
-            ctx, ResourceId=policy_id
-        )
-        if not tags_ret["result"]:
-            hub.log.debug(
-                f"Unable to list tags for resource {policy_id} with error: {tags_ret['comment']}"
-            )
-
-        translated_resource = (
-            hub.tool.aws.organizations.conversion_utils.convert_raw_policy_to_present(
-                policy_ret["ret"]["Policy"],
-                tags_ret["ret"]["Tags"] if tags_ret else None,
-            )
-        )
-
-        result[policy["Name"]] = {
+        result[policy_id] = {
             "aws.organizations.policy.present": [
                 {parameter_key: parameter_value}
-                for parameter_key, parameter_value in translated_resource.items()
+                for parameter_key, parameter_value in policy_ret["ret"].items()
             ]
         }
 
     return result
```

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/organizations/policy_attachment.py` & `idem-aws-2.0.0/idem_aws/states/aws/organizations/policy_attachment.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/rds/db_cluster.py` & `idem-aws-2.0.0/idem_aws/states/aws/rds/db_cluster.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/rds/db_cluster_parameter_group.py` & `idem-aws-2.0.0/idem_aws/states/aws/rds/db_cluster_parameter_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/rds/db_instance.py` & `idem-aws-2.0.0/idem_aws/states/aws/rds/db_instance.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/rds/db_parameter_group.py` & `idem-aws-2.0.0/idem_aws/states/aws/rds/db_parameter_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/rds/db_subnet_group.py` & `idem-aws-2.0.0/idem_aws/states/aws/rds/db_subnet_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/route53/hosted_zone.py` & `idem-aws-2.0.0/idem_aws/states/aws/route53/hosted_zone.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/route53/hosted_zone_association.py` & `idem-aws-2.0.0/idem_aws/states/aws/route53/hosted_zone_association.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/route53/resource_record.py` & `idem-aws-2.0.0/idem_aws/states/aws/route53/resource_record.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/s3/bucket.py` & `idem-aws-2.0.0/idem_aws/states/aws/s3/bucket.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/s3/bucket_acl.py` & `idem-aws-2.0.0/idem_aws/states/aws/s3/bucket_acl.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/s3/bucket_encryption.py` & `idem-aws-2.0.0/idem_aws/states/aws/s3/bucket_encryption.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/s3/bucket_lifecycle.py` & `idem-aws-2.0.0/idem_aws/states/aws/s3/bucket_lifecycle.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/s3/bucket_logging.py` & `idem-aws-2.0.0/idem_aws/states/aws/s3/bucket_logging.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/s3/bucket_notification.py` & `idem-aws-2.0.0/idem_aws/states/aws/s3/bucket_notification.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/s3/bucket_policy.py` & `idem-aws-2.0.0/idem_aws/states/aws/s3/bucket_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,19 +97,18 @@
     # Standardise on the json format
     policy = hub.tool.aws.state_comparison_utils.standardise_json(policy)
     # Get current bucket policy for the bucket
     if resource_id:
         before = await hub.exec.boto3.client.s3.get_bucket_policy(
             ctx, Bucket=bucket, ExpectedBucketOwner=expected_bucket_owner
         )
-        if before and not before["result"]:
+        if not before["result"] or not before["ret"]:
             result["comment"] = (
-                f"Failed to get existing Bucket policy '{name}'. Error : "
-                + before["comment"]
-            )
+                f"Failed to get existing Bucket policy '{name}'",
+            ) + before["comment"]
             result["result"] = before["result"]
             return result
 
         result[
             "old_state"
         ] = hub.tool.aws.s3.conversion_utils.convert_raw_bucket_policy_to_present(
             raw_resource=before["ret"], bucket=bucket, name=name
```

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/s3/bucket_replication.py` & `idem-aws-2.0.0/idem_aws/states/aws/s3/bucket_replication.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/s3/bucket_versioning.py` & `idem-aws-2.0.0/idem_aws/states/aws/s3/bucket_versioning.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/s3/bucket_website.py` & `idem-aws-2.0.0/idem_aws/states/aws/s3/bucket_website.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/s3/public_access_block.py` & `idem-aws-2.0.0/idem_aws/states/aws/s3/public_access_block.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/ses/domain_identity.py` & `idem-aws-2.0.0/idem_aws/states/aws/ses/domain_identity.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/ses/identity_notification_topic.py` & `idem-aws-2.0.0/idem_aws/states/aws/ses/identity_notification_topic.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/sesv2/event_destination.py` & `idem-aws-2.0.0/idem_aws/states/aws/sesv2/event_destination.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/sns/subscription.py` & `idem-aws-2.0.0/idem_aws/states/aws/sns/subscription.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,17 @@
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
     before = None
     resource_updated = False
     plan_state = None
     # Standardise JSON string format
     if attributes:
         for key, value in attributes.items():
-            attributes[key] = hub.tool.aws.sns.conversion_utils.standardise_json(value)
+            attributes[key] = hub.tool.aws.state_comparison_utils.standardise_json(
+                value
+            )
 
     if resource_id:
         resource = await hub.tool.boto3.resource.create(
             ctx, "sns", "Subscription", arn=resource_id
         )
         before = await hub.tool.boto3.resource.describe(resource)
```

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/sns/topic.py` & `idem-aws-2.0.0/idem_aws/states/aws/sns/topic.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/sns/topic_policy.py` & `idem-aws-2.0.0/idem_aws/states/aws/sns/topic_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
                 - resource_id: arn:aws:sns:eu-west-3:537227425989:test-topic-policy
     """
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
     resource_updated = False
     plan_state = None
 
     # Standardise JSON string format
-    policy = hub.tool.aws.sns.conversion_utils.standardise_json(policy)
+    policy = hub.tool.aws.state_comparison_utils.standardise_json(policy)
 
     before = await hub.exec.boto3.client.sns.get_topic_attributes(
         ctx, TopicArn=topic_arn
     )
     if before:
         result[
             "old_state"
```

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/sqs/queue.py` & `idem-aws-2.0.0/idem_aws/states/aws/sqs/queue.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/wafv2/associate_web_acl.py` & `idem-aws-2.0.0/idem_aws/states/aws/wafv2/associate_web_acl.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/wafv2/ip_set.py` & `idem-aws-2.0.0/idem_aws/states/aws/wafv2/ip_set.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/wafv2/regex_pattern_set.py` & `idem-aws-2.0.0/idem_aws/states/aws/wafv2/regex_pattern_set.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/states/aws/wafv2/web_acl.py` & `idem-aws-2.0.0/idem_aws/states/aws/wafv2/web_acl.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/acct/assume_role.py` & `idem-aws-2.0.0/idem_aws/tool/aws/acct/assume_role.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     """
     if "assume_role" not in raw_profile:
         return
 
     # Get new access credentials for the assumed role
     assume_role_obj = raw_profile.pop("assume_role", {})
 
-    ctx = dict_tools.data.NamespaceDict(acct=new_profile, test=False)
+    ctx = dict_tools.data.NamespaceDict(acct=raw_profile, test=False)
 
     try:
         credentials = await hub.exec.aws.sts.assume_role.credentials(
             ctx, **assume_role_obj
         )
     except Exception as e:
         raise ConnectionError(f"Failed to assume role: {e.__class__.__name__}:{e}")
```

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/acct/init.py` & `idem-aws-2.0.0/idem_aws/tool/aws/acct/init.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/acct/key_name.py` & `idem-aws-2.0.0/idem_aws/tool/aws/acct/key_name.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/acm/certificate_validation_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/acm/certificate_validation_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/acm/conversion_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/acm/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/acm/tag.py` & `idem-aws-2.0.0/idem_aws/tool/aws/acm/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/apigateway/base_path_mapping.py` & `idem-aws-2.0.0/idem_aws/tool/aws/apigateway/base_path_mapping.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/apigateway/deployment.py` & `idem-aws-2.0.0/idem_aws/tool/aws/apigateway/deployment.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/apigateway/domain_name.py` & `idem-aws-2.0.0/idem_aws/tool/aws/apigateway/domain_name.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/apigateway/integration.py` & `idem-aws-2.0.0/idem_aws/tool/aws/apigateway/integration.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/apigateway/integration_response.py` & `idem-aws-2.0.0/idem_aws/tool/aws/apigateway/integration_response.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/apigateway/method.py` & `idem-aws-2.0.0/idem_aws/tool/aws/apigateway/method.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/apigateway/method_response.py` & `idem-aws-2.0.0/idem_aws/tool/aws/apigateway/method_response.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/apigateway/resource.py` & `idem-aws-2.0.0/idem_aws/tool/aws/apigateway/resource.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/apigateway/rest_api.py` & `idem-aws-2.0.0/idem_aws/tool/aws/apigateway/rest_api.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/apigateway/stage.py` & `idem-aws-2.0.0/idem_aws/tool/aws/apigateway/stage.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/apigateway/tag.py` & `idem-aws-2.0.0/idem_aws/tool/aws/apigateway/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/apigatewayv2/api.py` & `idem-aws-2.0.0/idem_aws/tool/aws/apigatewayv2/api.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/apigatewayv2/authorizer.py` & `idem-aws-2.0.0/idem_aws/tool/aws/apigatewayv2/authorizer.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/apigatewayv2/domain_name.py` & `idem-aws-2.0.0/idem_aws/tool/aws/apigatewayv2/domain_name.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/apigatewayv2/integration.py` & `idem-aws-2.0.0/idem_aws/tool/aws/apigatewayv2/integration.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/apigatewayv2/route.py` & `idem-aws-2.0.0/idem_aws/tool/aws/apigatewayv2/route.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/apigatewayv2/stage.py` & `idem-aws-2.0.0/idem_aws/tool/aws/apigatewayv2/stage.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/apigatewayv2/tag.py` & `idem-aws-2.0.0/idem_aws/tool/aws/apigatewayv2/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/application_autoscaling/conversion_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/application_autoscaling/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/application_autoscaling/scalable_target.py` & `idem-aws-2.0.0/idem_aws/tool/aws/application_autoscaling/scalable_target.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/application_autoscaling/scaling_policy.py` & `idem-aws-2.0.0/idem_aws/tool/aws/application_autoscaling/scaling_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/arn_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/arn_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/autoscaling/auto_scaling_group_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/autoscaling/auto_scaling_group_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/autoscaling/conversion_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/autoscaling/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/autoscaling/scaling_policy.py` & `idem-aws-2.0.0/idem_aws/tool/aws/autoscaling/scaling_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/autoscaling/tag.py` & `idem-aws-2.0.0/idem_aws/tool/aws/autoscaling/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/backup/conversion_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/backup/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/backup/tag.py` & `idem-aws-2.0.0/idem_aws/tool/aws/backup/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/budgets/budget.py` & `idem-aws-2.0.0/idem_aws/tool/aws/budgets/budget.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/budgets/budget_action.py` & `idem-aws-2.0.0/idem_aws/tool/aws/budgets/budget_action.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/budgets/conversion_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/budgets/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/cloudformation/stack.py` & `idem-aws-2.0.0/idem_aws/tool/aws/cloudformation/stack.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/cloudfront/cloudfront_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/cloudfront/cloudfront_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/cloudfront/conversion_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/cloudfront/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/cloudfront/distribution.py` & `idem-aws-2.0.0/idem_aws/tool/aws/cloudfront/distribution.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/cloudfront/distribution_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/cloudfront/distribution_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/cloudfront/tag.py` & `idem-aws-2.0.0/idem_aws/tool/aws/cloudfront/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/cloudtrail/conversion_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/cloudtrail/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/cloudtrail/trail.py` & `idem-aws-2.0.0/idem_aws/tool/aws/cloudtrail/trail.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/cloudwatch/conversion_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/cloudwatch/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/cloudwatch/log_group.py` & `idem-aws-2.0.0/idem_aws/tool/aws/cloudwatch/log_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/cloudwatch/metric_alarm.py` & `idem-aws-2.0.0/idem_aws/tool/aws/cloudwatch/metric_alarm.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/cloudwatch/tag.py` & `idem-aws-2.0.0/idem_aws/tool/aws/cloudwatch/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/cloudwatchlogs/conversion_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/cloudwatchlogs/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/comment_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/comment_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/config/config_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/config/config_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/config/conversion_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/config/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/config/delivery_channel.py` & `idem-aws-2.0.0/idem_aws/tool/aws/config/delivery_channel.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/config/rule.py` & `idem-aws-2.0.0/idem_aws/tool/aws/config/rule.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/config/tag.py` & `idem-aws-2.0.0/idem_aws/tool/aws/config/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/costexplorer/anomaly_monitor.py` & `idem-aws-2.0.0/idem_aws/tool/aws/costexplorer/anomaly_monitor.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/costexplorer/anomaly_subscription.py` & `idem-aws-2.0.0/idem_aws/tool/aws/costexplorer/anomaly_subscription.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/costexplorer/conversion_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/costexplorer/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/costexplorer/cost_category.py` & `idem-aws-2.0.0/idem_aws/tool/aws/costexplorer/cost_category.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/docdb/db_cluster.py` & `idem-aws-2.0.0/idem_aws/tool/aws/docdb/db_cluster.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/docdb/db_cluster_parameter_group.py` & `idem-aws-2.0.0/idem_aws/tool/aws/docdb/db_cluster_parameter_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/docdb/db_subnet_group.py` & `idem-aws-2.0.0/idem_aws/tool/aws/docdb/db_subnet_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/docdb/tag.py` & `idem-aws-2.0.0/idem_aws/tool/aws/docdb/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/dynamodb/table.py` & `idem-aws-2.0.0/idem_aws/tool/aws/dynamodb/table.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ec2/ami.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ec2/ami.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ec2/availability_zones.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ec2/availability_zones.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ec2/conversion_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ec2/conversion_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -878,33 +878,38 @@
 ) -> Dict[str, Any]:
     if not raw_resource:
         return {}
 
     resource_translated = {
         "resource_id": raw_resource["VpcPeeringConnectionId"],
         "name": idem_resource_name,
-        "peer_allow_remote_vpc_dns_resolution": raw_resource["AccepterVpcInfo"][
-            "PeeringOptions"
-        ]["AllowDnsResolutionFromRemoteVpc"],
-        "peer_allow_classic_link_to_remote_vpc": raw_resource["AccepterVpcInfo"][
-            "PeeringOptions"
-        ]["AllowEgressFromLocalClassicLinkToRemoteVpc"],
-        "peer_allow_vpc_to_remote_classic_link": raw_resource["AccepterVpcInfo"][
-            "PeeringOptions"
-        ]["AllowEgressFromLocalVpcToRemoteClassicLink"],
-        "allow_remote_vpc_dns_resolution": raw_resource["RequesterVpcInfo"][
-            "PeeringOptions"
-        ]["AllowDnsResolutionFromRemoteVpc"],
-        "allow_classic_link_to_remote_vpc": raw_resource["RequesterVpcInfo"][
-            "PeeringOptions"
-        ]["AllowEgressFromLocalClassicLinkToRemoteVpc"],
-        "allow_vpc_to_remote_classic_link": raw_resource["RequesterVpcInfo"][
-            "PeeringOptions"
-        ]["AllowEgressFromLocalVpcToRemoteClassicLink"],
     }
+    # If acceptor or requestor vpc is from a different AWS account we do not get
+    # PeeringOptions from vpc in another AWS account.
+    if "PeeringOptions" in raw_resource["AccepterVpcInfo"]:
+        resource_translated["peer_allow_remote_vpc_dns_resolution"] = raw_resource[
+            "AccepterVpcInfo"
+        ]["PeeringOptions"]["AllowDnsResolutionFromRemoteVpc"]
+        resource_translated["peer_allow_classic_link_to_remote_vpc"] = raw_resource[
+            "AccepterVpcInfo"
+        ]["PeeringOptions"]["AllowEgressFromLocalClassicLinkToRemoteVpc"]
+        resource_translated["peer_allow_vpc_to_remote_classic_link"] = raw_resource[
+            "AccepterVpcInfo"
+        ]["PeeringOptions"]["AllowEgressFromLocalVpcToRemoteClassicLink"]
+
+    if "PeeringOptions" in raw_resource["RequesterVpcInfo"]:
+        resource_translated["allow_remote_vpc_dns_resolution"] = raw_resource[
+            "RequesterVpcInfo"
+        ]["PeeringOptions"]["AllowDnsResolutionFromRemoteVpc"]
+        resource_translated["allow_classic_link_to_remote_vpc"] = raw_resource[
+            "RequesterVpcInfo"
+        ]["PeeringOptions"]["AllowEgressFromLocalClassicLinkToRemoteVpc"]
+        resource_translated["allow_vpc_to_remote_classic_link"] = raw_resource[
+            "RequesterVpcInfo"
+        ]["PeeringOptions"]["AllowEgressFromLocalVpcToRemoteClassicLink"]
 
     return resource_translated
 
 
 def convert_raw_vpc_peering_connection_accepter_to_present(
     hub, raw_resource: Dict[str, Any], idem_resource_name: str
 ) -> Dict[str, Any]:
```

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ec2/dhcp_option_association_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ec2/dhcp_option_association_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ec2/elastic_ip.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ec2/elastic_ip.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ec2/flow_log.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ec2/flow_log.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/data.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/data.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/key_pair.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/key_pair.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/state.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/state.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/block_device_mappings.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/update/block_device_mappings.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/bootstrap.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/update/bootstrap.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/contracts/init.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/update/contracts/init.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/disable_api_termination.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/update/disable_api_termination.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/ebs_optimized.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/update/ebs_optimized.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/iam_instance_profile_arn.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/update/iam_instance_profile_arn.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/init.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/update/init.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/instance_initiated_shutdown_behavior.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/update/instance_initiated_shutdown_behavior.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/instance_type.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/update/instance_type.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/kernel_id.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/update/kernel_id.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/monitoring_enabled.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/update/monitoring_enabled.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/network_interfaces.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/update/network_interfaces.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/placement.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/update/placement.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/private_ip_address.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/update/private_ip_address.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/ram_disk_id.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/update/ram_disk_id.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/security_group_ids.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/update/security_group_ids.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/source_dest_check.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/update/source_dest_check.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/sriov_net_support.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/update/sriov_net_support.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/tags.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/update/tags.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/user_data.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ec2/instance/update/user_data.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ec2/internet_gateway.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ec2/internet_gateway.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ec2/key_pair.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ec2/key_pair.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ec2/launch_template.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ec2/launch_template.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ec2/network_interface.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ec2/network_interface.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ec2/placement_group.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ec2/placement_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ec2/route_table.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ec2/route_table.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ec2/security_group_rule.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ec2/security_group_rule.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ec2/snapshot.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ec2/snapshot.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ec2/spot_instance_request.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ec2/spot_instance_request.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ec2/subnet.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ec2/subnet.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ec2/tag.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ec2/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ec2/transit_gateway.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ec2/transit_gateway.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ec2/transit_gateway_vpc_attachment.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ec2/transit_gateway_vpc_attachment.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ec2/volume.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ec2/volume.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ec2/vpc.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ec2/vpc.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ec2/vpc_endpoint.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ec2/vpc_endpoint.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ec2/vpc_peering_connection_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ec2/vpc_peering_connection_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ecr/conversion_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ecr/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ecr/tag.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ecr/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/efs/file_system_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/efs/file_system_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/efs/mount_target_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/efs/mount_target_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/efs/tag.py` & `idem-aws-2.0.0/idem_aws/tool/aws/efs/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/eks/addon.py` & `idem-aws-2.0.0/idem_aws/tool/aws/eks/addon.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/eks/cluster.py` & `idem-aws-2.0.0/idem_aws/tool/aws/eks/cluster.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/eks/conversion_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/eks/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/eks/eks_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/eks/eks_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/eks/nodegroup.py` & `idem-aws-2.0.0/idem_aws/tool/aws/eks/nodegroup.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/eks/tag.py` & `idem-aws-2.0.0/idem_aws/tool/aws/eks/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/elasticache/conversion_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/elasticache/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/elasticache/elasticache_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/elasticache/elasticache_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/elasticache/parameters.py` & `idem-aws-2.0.0/idem_aws/tool/aws/elasticache/parameters.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/elb/conversion_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/elb/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/elb/load_balancer.py` & `idem-aws-2.0.0/idem_aws/tool/aws/elb/load_balancer.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/elb/tag.py` & `idem-aws-2.0.0/idem_aws/tool/aws/elb/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/elbv2/conversion_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/elbv2/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/elbv2/listener.py` & `idem-aws-2.0.0/idem_aws/tool/aws/elbv2/listener.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/elbv2/load_balancer.py` & `idem-aws-2.0.0/idem_aws/tool/aws/elbv2/load_balancer.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/elbv2/tag.py` & `idem-aws-2.0.0/idem_aws/tool/aws/elbv2/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/elbv2/target_group.py` & `idem-aws-2.0.0/idem_aws/tool/aws/elbv2/target_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/es/elasticsearch_domain.py` & `idem-aws-2.0.0/idem_aws/tool/aws/es/elasticsearch_domain.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/es/tag.py` & `idem-aws-2.0.0/idem_aws/tool/aws/es/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/events/conversion_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/events/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/events/rule.py` & `idem-aws-2.0.0/idem_aws/tool/aws/events/rule.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/events/tag.py` & `idem-aws-2.0.0/idem_aws/tool/aws/events/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/guardduty/config_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/guardduty/config_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/guardduty/conversion_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/guardduty/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/guardduty/detector.py` & `idem-aws-2.0.0/idem_aws/tool/aws/guardduty/detector.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/iam/conversion_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/iam/conversion_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import json
 from collections import OrderedDict
 from typing import Any
 from typing import Dict
 from typing import List
 
 
 def convert_raw_instance_profile_to_present(
@@ -52,15 +51,17 @@
 
     translated_resource = {}
     for parameter_raw, parameter_present in resource_parameters.items():
         if parameter_raw in raw_resource:
             translated_resource[parameter_present] = raw_resource.get(parameter_raw)
 
     if translated_resource.get("policy_document") is not None:
-        translated_resource["policy_document"] = _standardise_json(
+        translated_resource[
+            "policy_document"
+        ] = hub.tool.aws.state_comparison_utils.standardise_json(
             translated_resource.get("policy_document")
         )
 
     if translated_resource.get("tags") is not None:
         translated_resource["tags"] = hub.tool.aws.tag_utils.convert_tag_list_to_dict(
             translated_resource.get("tags")
         )
@@ -93,15 +94,17 @@
 
     if raw_resource.get("PermissionsBoundary"):
         translated_resource["permissions_boundary"] = raw_resource.get(
             "PermissionsBoundary"
         ).get("PermissionsBoundaryArn")
 
     if raw_resource.get("AssumeRolePolicyDocument", None):
-        translated_resource["assume_role_policy_document"] = _standardise_json(
+        translated_resource[
+            "assume_role_policy_document"
+        ] = hub.tool.aws.state_comparison_utils.standardise_json(
             raw_resource.get("AssumeRolePolicyDocument")
         )
 
     return translated_resource
 
 
 def convert_raw_role_policy_to_present(
@@ -120,15 +123,17 @@
         "resource_id": f"{raw_resource.get('RoleName')}-{raw_resource.get('PolicyName')}"
     }
     for parameter_raw, parameter_present in resource_parameters.items():
         if parameter_raw in raw_resource:
             translated_resource[parameter_present] = raw_resource.get(parameter_raw)
 
     if raw_resource.get("PolicyDocument"):
-        translated_resource["policy_document"] = _standardise_json(
+        translated_resource[
+            "policy_document"
+        ] = hub.tool.aws.state_comparison_utils.standardise_json(
             raw_resource.get("PolicyDocument")
         )
 
     return translated_resource
 
 
 def convert_raw_role_policy_attachment_to_present(
@@ -156,15 +161,17 @@
         "resource_id": f"{raw_resource.get('UserName')}-{raw_resource.get('PolicyName')}"
     }
     for parameter_raw, parameter_present in resource_parameters.items():
         if parameter_raw in raw_resource:
             translated_resource[parameter_present] = raw_resource.get(parameter_raw)
 
     if raw_resource.get("PolicyDocument"):
-        translated_resource["policy_document"] = _standardise_json(
+        translated_resource[
+            "policy_document"
+        ] = hub.tool.aws.state_comparison_utils.standardise_json(
             raw_resource.get("PolicyDocument")
         )
 
     return translated_resource
 
 
 def convert_raw_user_to_present(
@@ -250,25 +257,14 @@
     else:
         hub.log.warning(
             f"Could not get ssh public key body with ssh public key ID {idem_resource_name} with error"
         )
     return translated_resource
 
 
-def _standardise_json(value: str or Dict):
-    if value is None:
-        return None
-
-    if isinstance(value, str):
-        json_dict = json.loads(value)
-    else:
-        json_dict = value
-    return json.dumps(json_dict, separators=(", ", ": "), sort_keys=True)
-
-
 # NOTE: access_keys are different from other AWS objects, so we
 #  use convert_raw_access_key_to_camel_case to provide a semi-normal python representation
 #  and then convert_access_key_to_present takes that camel case representation
 #  and outputs in 'present' format.
 def convert_raw_access_key_to_camel_case(
     hub,
     access_key_raw: Dict[str, Any],
```

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/iam/group.py` & `idem-aws-2.0.0/idem_aws/tool/aws/iam/group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/iam/group_membership.py` & `idem-aws-2.0.0/idem_aws/tool/aws/iam/group_membership.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/iam/password_policy.py` & `idem-aws-2.0.0/idem_aws/tool/aws/iam/password_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/iam/policy.py` & `idem-aws-2.0.0/idem_aws/tool/aws/iam/policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/iam/role_policy_attachment.py` & `idem-aws-2.0.0/idem_aws/tool/aws/iam/role_policy_attachment.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/iam/service_linked_role.py` & `idem-aws-2.0.0/idem_aws/tool/aws/iam/service_linked_role.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/iam/user.py` & `idem-aws-2.0.0/idem_aws/tool/aws/iam/user.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/iam/user_ssh_key.py` & `idem-aws-2.0.0/idem_aws/tool/aws/iam/user_ssh_key.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/kinesis/conversion_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/kinesis/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/kinesis/stream.py` & `idem-aws-2.0.0/idem_aws/tool/aws/kinesis/stream.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/kinesis/tag.py` & `idem-aws-2.0.0/idem_aws/tool/aws/kinesis/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/kms/alias.py` & `idem-aws-2.0.0/idem_aws/tool/aws/kms/alias.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/kms/conversion_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/kms/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/kms/key.py` & `idem-aws-2.0.0/idem_aws/tool/aws/kms/key.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/kms/tag.py` & `idem-aws-2.0.0/idem_aws/tool/aws/kms/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/lambda_aws/conversion_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/lambda_aws/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/lambda_aws/function.py` & `idem-aws-2.0.0/idem_aws/tool/aws/lambda_aws/function.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/lambda_aws/function_event_invoke_config.py` & `idem-aws-2.0.0/idem_aws/tool/aws/lambda_aws/function_event_invoke_config.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/lambda_aws/function_permission.py` & `idem-aws-2.0.0/idem_aws/tool/aws/lambda_aws/function_permission.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/lambda_aws/function_provisioned_concurrency_config.py` & `idem-aws-2.0.0/idem_aws/tool/aws/lambda_aws/function_provisioned_concurrency_config.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/lambda_aws/tag.py` & `idem-aws-2.0.0/idem_aws/tool/aws/lambda_aws/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/logs/subscription_filter_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/logs/subscription_filter_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/neptune/conversion_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/neptune/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/neptune/db_cluster.py` & `idem-aws-2.0.0/idem_aws/tool/aws/neptune/db_cluster.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/neptune/db_cluster_parameter_group.py` & `idem-aws-2.0.0/idem_aws/tool/aws/neptune/db_cluster_parameter_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/neptune/db_instance.py` & `idem-aws-2.0.0/idem_aws/tool/aws/neptune/db_instance.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/neptune/db_parameter_group.py` & `idem-aws-2.0.0/idem_aws/tool/aws/neptune/db_parameter_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/neptune/db_subnet_group.py` & `idem-aws-2.0.0/idem_aws/tool/aws/neptune/db_subnet_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/neptune/tag.py` & `idem-aws-2.0.0/idem_aws/tool/aws/neptune/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/network_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/network_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/organizations/account.py` & `idem-aws-2.0.0/idem_aws/tool/aws/organizations/account.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/organizations/conversion_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/organizations/conversion_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,21 @@
     for camel_case_key, snake_case_key in describe_parameters.items():
         if policy["PolicySummary"].get(camel_case_key) is not None:
             translated_resource[snake_case_key] = policy["PolicySummary"].get(
                 camel_case_key
             )
         elif policy.get(camel_case_key) is not None:
             translated_resource[snake_case_key] = policy.get(camel_case_key)
+
+    translated_resource[
+        "content"
+    ] = hub.tool.aws.state_comparison_utils.standardise_json(
+        translated_resource["content"]
+    )
+
     if tags:
         if isinstance(tags, List):
             tags = hub.tool.aws.tag_utils.convert_tag_list_to_dict(tags)
         translated_resource["tags"] = tags
     return translated_resource
```

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/organizations/policy_attachment.py` & `idem-aws-2.0.0/idem_aws/tool/aws/organizations/policy_attachment.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/organizations/tag.py` & `idem-aws-2.0.0/idem_aws/tool/aws/organizations/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/parameters.py` & `idem-aws-2.0.0/idem_aws/tool/aws/parameters.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/rds/conversion_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/rds/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/rds/parameters.py` & `idem-aws-2.0.0/idem_aws/tool/aws/rds/parameters.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/route53/conversion_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/route53/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/route53/hosted_zone_association.py` & `idem-aws-2.0.0/idem_aws/tool/aws/route53/hosted_zone_association.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/route53/hosted_zone_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/route53/hosted_zone_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/route53/resource_record_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/route53/resource_record_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/route53/tag.py` & `idem-aws-2.0.0/idem_aws/tool/aws/route53/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/s3/bucket_acl.py` & `idem-aws-2.0.0/idem_aws/tool/aws/s3/bucket_acl.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/s3/bucket_encryption.py` & `idem-aws-2.0.0/idem_aws/tool/aws/s3/bucket_encryption.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/s3/bucket_lifecycle.py` & `idem-aws-2.0.0/idem_aws/tool/aws/s3/bucket_lifecycle.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/s3/bucket_logging.py` & `idem-aws-2.0.0/idem_aws/tool/aws/s3/bucket_logging.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/s3/bucket_replication.py` & `idem-aws-2.0.0/idem_aws/tool/aws/s3/bucket_replication.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/s3/bucket_versioning.py` & `idem-aws-2.0.0/idem_aws/tool/aws/s3/bucket_versioning.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/s3/bucket_website.py` & `idem-aws-2.0.0/idem_aws/tool/aws/s3/bucket_website.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/s3/conversion_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/s3/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/s3/s3_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/s3/s3_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/search_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/search_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/ses/conversion_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/ses/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/sesv2/conversion_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/sesv2/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/sns/conversion_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/sns/conversion_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """Util functions for converting raw attributes to present form and vice versa."""
-import json
 from collections import OrderedDict
-from json import JSONDecodeError
 from typing import Any
 from typing import Dict
 
 
 def convert_raw_subscription_to_present(
     hub, raw_resource: Dict[str, Any], idem_resource_name: str = None
 ) -> Dict[str, Any]:
@@ -33,15 +31,17 @@
         "RedrivePolicy",
     ]
 
     attributes = {}
     for param in attribute_params:
         value = raw_attributes.get(param, None)
         if value:
-            attributes[param] = standardise_json(hub, value)
+            attributes[param] = hub.tool.aws.state_comparison_utils.standardise_json(
+                value
+            )
     resource_translated["attributes"] = attributes
 
     return resource_translated
 
 
 def convert_raw_topic_to_present(
     hub,
@@ -82,26 +82,13 @@
     """Util functions to convert raw resource state to present input format for SNS topic_policy."""
     raw_attributes = raw_resource["ret"].get("Attributes")
     resource_id = raw_attributes.get("TopicArn") + "-policy"
     resource_translated = {
         "name": idem_resource_name,
         "resource_id": resource_id,
         "topic_arn": raw_attributes.get("TopicArn"),
-        "policy": standardise_json(hub, raw_attributes.get("Policy")),
+        "policy": hub.tool.aws.state_comparison_utils.standardise_json(
+            raw_attributes.get("Policy")
+        ),
     }
 
     return resource_translated
-
-
-def standardise_json(hub, value: str):
-    """Utils function for standardising the json string format for SNS resources."""
-    if value is None:
-        return None
-
-    if isinstance(value, str):
-        try:
-            json_dict = json.loads(value)
-        except JSONDecodeError:
-            json_dict = value
-    else:
-        json_dict = value
-    return json.dumps(json_dict, separators=(", ", ": "))
```

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/sns/sns_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/sns/sns_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/sqs/conversion_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/sqs/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/sqs/queue_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/sqs/queue_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/state_comparison_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/state_comparison_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/state_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/state_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/string_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/string_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/tag_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/tag_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/test_state_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/test_state_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/wafv2/conversion_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/wafv2/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/wafv2/ip_set_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/wafv2/ip_set_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/wafv2/regex_pattern_set.py` & `idem-aws-2.0.0/idem_aws/tool/aws/wafv2/regex_pattern_set.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/wafv2/tag.py` & `idem-aws-2.0.0/idem_aws/tool/aws/wafv2/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/wafv2/web_acl.py` & `idem-aws-2.0.0/idem_aws/tool/aws/wafv2/web_acl.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/aws/waiter_utils.py` & `idem-aws-2.0.0/idem_aws/tool/aws/waiter_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/boto3/client.py` & `idem-aws-2.0.0/idem_aws/tool/boto3/client.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/boto3/custom_waiter.py` & `idem-aws-2.0.0/idem_aws/tool/boto3/custom_waiter.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/boto3/region.py` & `idem-aws-2.0.0/idem_aws/tool/boto3/region.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/boto3/resolve.py` & `idem-aws-2.0.0/idem_aws/tool/boto3/resolve.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/boto3/resource.py` & `idem-aws-2.0.0/idem_aws/tool/boto3/resource.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/boto3/session.py` & `idem-aws-2.0.0/idem_aws/tool/boto3/session.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws/tool/heist/bootstrap.py` & `idem-aws-2.0.0/idem_aws/tool/heist/bootstrap.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws.egg-info/PKG-INFO` & `idem-aws-2.0.0/idem_aws.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: idem-aws
-Version: 1.7.5
+Version: 2.0.0
 Summary: AWS Cloud Provider for Idem
 Home-page: https://docs.idemproject.io/idem-aws/en/latest/index.html
 Author: VMware, Inc.
 Author-email: idemproject@vmware.com
 License: Apache Software License 2.0
 Project-URL: Code, https://gitlab.com/vmware/idem/idem-aws
 Project-URL: Issue tracker, https://gitlab.com/vmware/idem/idem-aws/issues
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: full
 Provides-Extra: bootstrap
 Provides-Extra: localstack
 Provides-Extra: google_auth
 Provides-Extra: autogen
 License-File: LICENSE
@@ -88,15 +89,15 @@
 
 Getting Started
 ===============
 
 Prerequisites
 -------------
 
-* Python 3.7+
+* Python 3.8+
 * git *(if installing from source, or contributing to the project)*
 
 Installation
 ------------
 
 .. note::
```

### Comparing `idem-aws-1.7.5/idem_aws.egg-info/SOURCES.txt` & `idem-aws-2.0.0/idem_aws.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.5/idem_aws.egg-info/requires.txt` & `idem-aws-2.0.0/idem_aws.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 acct<9.0.0,>=8.3.3
+dict-toolbox>=3.1.1
 boto3<1.27.0,>=1.25.0
 configparser<6.0.0,>=5.0.0
-idem<22.0.0,>=20.7.0
+idem<23.0.0,>=21.0.0
 pgpy<0.6.0,>=0.5.4
 deepdiff<6.0.0,>=5.8.0
 heist<7.0.0,>=6.1.0
 pycryptodomex<3.14.0,>=3.10
 pop-serial<2.0.0,>=1.1.0
 cryptography<38.0.0,>=37.0.4
 
@@ -15,24 +16,24 @@
 textwrap3
 tqdm
 
 [bootstrap]
 heist-salt<6.0.0,>=5.3.1
 
 [full]
-localstack
-msgpack
-localstack-client
-pop-create-idem==2.0.4
-textwrap3
-tqdm
 localstack-ext
 heist-salt<6.0.0,>=5.3.1
+localstack-client
+msgpack
+localstack
+tqdm
 aws-google-auth>=0.0.35
+pop-create-idem==2.0.4
 inflect
+textwrap3
 
 [google_auth]
 aws-google-auth>=0.0.35
 msgpack
 
 [localstack]
 localstack
```

### Comparing `idem-aws-1.7.5/setup.py` & `idem-aws-2.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,26 +77,27 @@
     },
     version=VERSION,
     install_requires=REQUIREMENTS,
     extras_require=REQUIREMENTS_EXTRA,
     description=DESC,
     long_description=LONG_DESC,
     long_description_content_type="text/x-rst",
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     license="Apache Software License 2.0",
     classifiers=[
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Intended Audience :: System Administrators",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
     ],
     packages=discover_packages(),
     cmdclass={"clean": Clean},
 )
```

