# Comparing `tmp/tomcru-0.2.5.tar.gz` & `tmp/tomcru-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomcru-0.2.5.tar", max compression
+gzip compressed data, was "tomcru-0.2.6.tar", max compression
```

## Comparing `tomcru-0.2.5.tar` & `tomcru-0.2.6.tar`

### file list

```diff
@@ -1,110 +1,110 @@
--rw-r--r--   0        0        0     1065 2023-04-17 18:29:36.244599 tomcru-0.2.5/LICENSE
--rw-r--r--   0        0        0      183 2023-04-17 18:29:36.244599 tomcru-0.2.5/README.md
--rw-r--r--   0        0        0      632 2023-05-14 01:35:31.110041 tomcru-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      474 2023-04-29 11:53:00.162328 tomcru-0.2.5/tomcru/__init__.py
--rw-r--r--   0        0        0      885 2023-04-20 17:28:59.003207 tomcru-0.2.5/tomcru/appbuilders/envmapping.py
--rw-r--r--   0        0        0     1587 2023-04-29 18:55:53.024675 tomcru-0.2.5/tomcru/appbuilders/faas/InjectableAppBase.py
--rw-r--r--   0        0        0     2936 2023-04-29 11:52:43.934414 tomcru-0.2.5/tomcru/appbuilders/faas/sam_app/SamAppBuilder.py
--rw-r--r--   0        0        0       70 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/appbuilders/faas/sam_app/__init__.py
--rw-r--r--   0        0        0      848 2023-04-27 10:14:15.980656 tomcru-0.2.5/tomcru/appbuilders/faas/static_app/StaticAppBuilder.py
--rw-r--r--   0        0        0       79 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/appbuilders/faas/static_app/__init__.py
--rw-r--r--   0        0        0     9980 2023-04-29 12:03:31.807647 tomcru-0.2.5/tomcru/cfgparsers/BaseCfgParser.py
--rw-r--r--   0        0        0     3070 2023-04-29 01:53:19.641911 tomcru-0.2.5/tomcru/cfgparsers/EnvParser.py
--rw-r--r--   0        0        0     1144 2023-04-20 10:17:05.036609 tomcru-0.2.5/tomcru/cfgparsers/MergeCfgParser.py
--rw-r--r--   0        0        0     5090 2023-04-29 12:02:36.779844 tomcru-0.2.5/tomcru/cfgparsers/SwaggerCfgParser.py
--rw-r--r--   0        0        0      322 2023-04-23 19:46:42.543716 tomcru-0.2.5/tomcru/cfgparsers/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 19:28:55.917588 tomcru-0.2.5/tomcru/core/__init__.py
--rw-r--r--   0        0        0     3291 2023-04-29 12:02:24.479889 tomcru-0.2.5/tomcru/core/cfg/api.py
--rw-r--r--   0        0        0     1244 2023-04-29 11:52:34.470450 tomcru-0.2.5/tomcru/core/cfg/authorizers.py
--rw-r--r--   0        0        0     3716 2023-04-29 12:01:41.192048 tomcru-0.2.5/tomcru/core/cfg/integrations.py
--rw-r--r--   0        0        0     2041 2023-04-29 11:52:34.486450 tomcru-0.2.5/tomcru/core/cfg/proj.py
--rw-r--r--   0        0        0      670 2023-04-29 16:16:10.250867 tomcru-0.2.5/tomcru/core/modloader.py
--rw-r--r--   0        0        0      833 2023-04-25 19:30:27.561274 tomcru-0.2.5/tomcru/core/obj_store.py
--rw-r--r--   0        0        0     2989 2023-04-29 17:03:04.510715 tomcru-0.2.5/tomcru/core/project.py
--rw-r--r--   0        0        0     2227 2023-04-29 16:20:26.534540 tomcru-0.2.5/tomcru/core/servmgr.py
--rw-r--r--   0        0        0     3802 2023-05-07 01:20:10.626850 tomcru-0.2.5/tomcru/core/utils/MyMetaLoader.py
--rw-r--r--   0        0        0      104 2023-04-20 13:43:12.977618 tomcru-0.2.5/tomcru/core/utils/__init__.py
--rw-r--r--   0        0        0     1135 2023-04-20 13:44:18.245442 tomcru-0.2.5/tomcru/core/utils/toml_custom.py
--rw-r--r--   0        0        0     2462 2023-04-17 18:29:36.252599 tomcru-0.2.5/tomcru/core/utils/yaml_custom.py
--rw-r--r--   0        0        0       72 2023-05-05 20:11:13.811402 tomcru-0.2.5/tomcru/etc/proxies/aws-sdk/index.js
--rw-r--r--   0        0        0      261 2023-05-05 20:10:34.172421 tomcru-0.2.5/tomcru/etc/proxies/aws-sdk/package.json
--rw-r--r--   0        0        0      558 2023-05-05 23:50:53.045569 tomcru-0.2.5/tomcru/etc/proxies/aws-sdk/proxylib.js
--rw-r--r--   0        0        0      873 2023-05-06 16:59:17.798252 tomcru-0.2.5/tomcru/etc/proxies/aws-sdk/serv/ddb.js
--rw-r--r--   0        0        0      703 2023-05-06 16:12:42.134096 tomcru-0.2.5/tomcru/etc/proxies/t_proxy.js
--rw-r--r--   0        0        0      540 2023-04-25 19:12:49.028297 tomcru-0.2.5/tomcru/services/ServiceBase.py
--rw-r--r--   0        0        0        0 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/__init__.py
--rw-r--r--   0        0        0        0 2023-04-23 00:05:26.709577 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/__init__.py
--rw-r--r--   0        0        0     6799 2023-04-29 12:52:25.243899 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/api_shared/ApiGWBuilderBase.py
--rw-r--r--   0        0        0        0 2023-04-29 03:09:12.832374 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/api_shared/__init__.py
--rw-r--r--   0        0        0      835 2023-04-29 11:52:34.482450 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/api_shared/integration/ExternalLambdaAuthorizerIntegration.py
--rw-r--r--   0        0        0     2688 2023-05-01 08:08:53.636339 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/api_shared/integration/LambdaAuthorizerIntegration.py
--rw-r--r--   0        0        0     3318 2023-05-13 22:33:23.948162 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/api_shared/integration/OIDCAuthorizerIntegration.py
--rw-r--r--   0        0        0      711 2023-04-29 11:52:34.510450 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/api_shared/integration/TomcruApiGWHttpIntegration.py
--rw-r--r--   0        0        0      322 2023-04-29 03:05:19.325205 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/api_shared/integration/__init__.py
--rw-r--r--   0        0        0     4871 2023-05-01 09:27:22.908562 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/flask_b/ApiGWFlaskBuilder.py
--rw-r--r--   0        0        0       85 2023-04-21 15:34:30.512217 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/flask_b/__init__.py
--rw-r--r--   0        0        0      691 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/flask_b/controllers/EmeProxyController.py
--rw-r--r--   0        0        0      213 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/flask_b/controllers/HomeController.py
--rw-r--r--   0        0        0      236 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/flask_b/controllers/SwaggerController.py
--rw-r--r--   0        0        0     4019 2023-05-13 22:36:02.291646 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/flask_b/integration/LambdaIntegration.py
--rw-r--r--   0        0        0     1808 2023-05-13 22:27:41.433281 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/flask_b/integration/MockedIntegration.py
--rw-r--r--   0        0        0     2553 2023-04-29 11:52:43.966414 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/flask_b/integration/SwaggerIntegration.py
--rw-r--r--   0        0        0      148 2023-04-23 17:59:42.203687 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/flask_b/integration/__init__.py
--rw-r--r--   0        0        0      352 2023-04-21 15:34:30.504217 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/ws_b/ApiGWWebsocketBuilder.py
--rw-r--r--   0        0        0       97 2023-04-21 15:34:35.936203 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/ws_b/__init__.py
--rw-r--r--   0        0        0     2994 2023-04-29 11:52:43.946414 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/WsAppBuilder.py
--rw-r--r--   0        0        0       70 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/__init__.py
--rw-r--r--   0        0        0     1750 2023-04-29 11:53:00.170328 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/_jank.py
--rw-r--r--   0        0        0     3296 2023-04-29 11:52:34.474450 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/apps/EmeWsApp.py
--rw-r--r--   0        0        0     3510 2023-04-29 11:52:43.962414 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/LambdaIntegration.py
--rw-r--r--   0        0        0      185 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/TomcruApiGWWsIntegration.py
--rw-r--r--   0        0        0      686 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/WsEnRouteCachedAuthorizer.py
--rw-r--r--   0        0        0      853 2023-04-25 19:16:13.145908 tomcru-0.2.5/tomcru/services/aws/hosted/apigw_manager_b/ApiGWMgr.py
--rw-r--r--   0        0        0       58 2023-04-23 13:47:38.385293 tomcru-0.2.5/tomcru/services/aws/hosted/apigw_manager_b/__init__.py
--rw-r--r--   0        0        0     1477 2023-05-07 02:33:51.682008 tomcru-0.2.5/tomcru/services/aws/hosted/boto3_b/Boto3Builder.py
--rw-r--r--   0        0        0       70 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/hosted/boto3_b/__init__.py
--rw-r--r--   0        0        0      622 2023-05-03 19:16:05.271285 tomcru-0.2.5/tomcru/services/aws/hosted/boto3_b/boto3.py
--rw-r--r--   0        0        0     1782 2023-04-29 22:03:41.543858 tomcru-0.2.5/tomcru/services/aws/hosted/cloudfront/flask_b/CloudfrontFlaskBuilder.py
--rw-r--r--   0        0        0      100 2023-04-29 15:54:06.512215 tomcru-0.2.5/tomcru/services/aws/hosted/cloudfront/flask_b/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 18:57:16.415271 tomcru-0.2.5/tomcru/services/aws/hosted/ddb/__init__.py
--rw-r--r--   0        0        0      993 2023-05-04 12:19:56.412205 tomcru-0.2.5/tomcru/services/aws/hosted/ddb/proxy.py
--rw-r--r--   0        0        0     8695 2023-05-13 22:09:34.428940 tomcru-0.2.5/tomcru/services/aws/hosted/ddb/sqlalchemy_b/DDBSqlAlchemyTable.py
--rw-r--r--   0        0        0      971 2023-05-04 22:52:05.711536 tomcru-0.2.5/tomcru/services/aws/hosted/ddb/sqlalchemy_b/DynamoDBBuilder.py
--rw-r--r--   0        0        0     1134 2023-05-09 21:53:23.860126 tomcru-0.2.5/tomcru/services/aws/hosted/ddb/sqlalchemy_b/SqlAlchemyJSONType.py
--rw-r--r--   0        0        0       79 2023-04-20 17:41:37.808233 tomcru-0.2.5/tomcru/services/aws/hosted/ddb/sqlalchemy_b/__init__.py
--rw-r--r--   0        0        0      377 2023-05-09 21:44:42.921751 tomcru-0.2.5/tomcru/services/aws/hosted/ddb/sqlalchemy_b/boto3_proxy.py
--rw-r--r--   0        0        0     5436 2023-05-09 22:04:01.245469 tomcru-0.2.5/tomcru/services/aws/hosted/ddb/sqlalchemy_b/dal_ddb.py
--rw-r--r--   0        0        0     4400 2023-05-07 02:33:48.046038 tomcru-0.2.5/tomcru/services/aws/hosted/lambda_b/LambdaBuilder.py
--rw-r--r--   0        0        0      784 2023-05-01 08:27:27.476570 tomcru-0.2.5/tomcru/services/aws/hosted/lambda_b/LambdaHostedPyContext.py
--rw-r--r--   0        0        0       74 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/hosted/lambda_b/__init__.py
--rw-r--r--   0        0        0     5074 2023-05-13 17:44:03.162000 tomcru-0.2.5/tomcru/services/aws/hosted/lambda_b/proxy/Py2NodeLambdaProxy.py
--rw-r--r--   0        0        0     2585 2023-05-12 20:18:40.139204 tomcru-0.2.5/tomcru/services/aws/hosted/s3_b/S3AdapterLocal.py
--rw-r--r--   0        0        0      585 2023-05-09 23:34:07.782900 tomcru-0.2.5/tomcru/services/aws/hosted/s3_b/S3Service.py
--rw-r--r--   0        0        0       61 2023-04-25 22:42:25.629435 tomcru-0.2.5/tomcru/services/aws/hosted/s3_b/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/onpremise/__init__.py
--rw-r--r--   0        0        0     4043 2023-04-29 11:53:00.190328 tomcru-0.2.5/tomcru/services/aws/onpremise/model_checker/SwaggerResponseModelValidator.py
--rw-r--r--   0        0        0      121 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/onpremise/model_checker/__init__.py
--rw-r--r--   0        0        0      782 2023-04-29 11:52:34.530450 tomcru-0.2.5/tomcru/services/aws/onpremise/s3_static/S3StaticBuilder.py
--rw-r--r--   0        0        0       78 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/onpremise/s3_static/__init__.py
--rw-r--r--   0        0        0     7308 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/sam/_junk/SamTplBuilder.py
--rw-r--r--   0        0        0      841 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/sam/_junk/core.yaml
--rw-r--r--   0        0        0      855 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/sam/_junk/httpapi.yaml
--rw-r--r--   0        0        0      372 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/sam/_junk/integ_normal.yaml
--rw-r--r--   0        0        0      638 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/sam/_junk/integ_ws.yaml
--rw-r--r--   0        0        0      153 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/sam/_junk/lambda.yaml
--rw-r--r--   0        0        0      231 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/sam/_junk/layer.yaml
--rw-r--r--   0        0        0     4389 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/sam/_junk/template.yaml
--rw-r--r--   0        0        0     1027 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/sam/_junk/wsapi.yaml
--rw-r--r--   0        0        0     2101 2023-04-29 11:53:00.174328 tomcru-0.2.5/tomcru/services/aws/sam/lambda_b/LambdaBuilder.py
--rw-r--r--   0        0        0       74 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/sam/lambda_b/__init__.py
--rw-r--r--   0        0        0     1344 2023-04-29 11:53:00.154328 tomcru-0.2.5/tomcru/services/aws/sam/params_b/ParametersBuilder.py
--rw-r--r--   0        0        0       85 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/sam/params_b/__init__.py
--rw-r--r--   0        0        0     2725 2023-04-29 11:53:00.170328 tomcru-0.2.5/tomcru/services/aws/sam/spec_api_b/SwaggerApiTemplater.py
--rw-r--r--   0        0        0       91 2023-04-17 18:29:36.248599 tomcru-0.2.5/tomcru/services/aws/sam/spec_api_b/__init__.py
--rw-r--r--   0        0        0     1757 2023-04-29 11:52:34.502450 tomcru-0.2.5/tomcru/services/aws/sam/spec_api_b/authorizers/SAMLambdaAuthBuilder.py
--rw-r--r--   0        0        0      774 2023-04-29 11:52:34.470450 tomcru-0.2.5/tomcru/services/aws/sam/spec_api_b/authorizers/SAMOIDCAuthBuilder.py
--rw-r--r--   0        0        0      835 2023-04-29 11:52:43.962414 tomcru-0.2.5/tomcru/services/aws/sam/spec_api_b/integrations/SAMLambdaBuilder.py
--rw-r--r--   0        0        0     2266 2023-04-29 11:52:43.970414 tomcru-0.2.5/tomcru/services/general/eme2swagger/Eme2Swagger.py
--rw-r--r--   0        0        0       67 2023-04-17 18:29:36.252599 tomcru-0.2.5/tomcru/services/general/eme2swagger/__init__.py
--rw-r--r--   0        0        0     1047 1970-01-01 00:00:00.000000 tomcru-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-17 18:29:36.244599 tomcru-0.2.6/LICENSE
+-rw-r--r--   0        0        0      183 2023-04-17 18:29:36.244599 tomcru-0.2.6/README.md
+-rw-r--r--   0        0        0      632 2023-05-15 23:48:28.374215 tomcru-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      474 2023-04-29 11:53:00.162328 tomcru-0.2.6/tomcru/__init__.py
+-rw-r--r--   0        0        0      885 2023-04-20 17:28:59.003207 tomcru-0.2.6/tomcru/appbuilders/envmapping.py
+-rw-r--r--   0        0        0     1587 2023-04-29 18:55:53.024675 tomcru-0.2.6/tomcru/appbuilders/faas/InjectableAppBase.py
+-rw-r--r--   0        0        0     2936 2023-04-29 11:52:43.934414 tomcru-0.2.6/tomcru/appbuilders/faas/sam_app/SamAppBuilder.py
+-rw-r--r--   0        0        0       70 2023-04-17 18:29:36.248599 tomcru-0.2.6/tomcru/appbuilders/faas/sam_app/__init__.py
+-rw-r--r--   0        0        0      848 2023-04-27 10:14:15.980656 tomcru-0.2.6/tomcru/appbuilders/faas/static_app/StaticAppBuilder.py
+-rw-r--r--   0        0        0       79 2023-04-17 18:29:36.248599 tomcru-0.2.6/tomcru/appbuilders/faas/static_app/__init__.py
+-rw-r--r--   0        0        0     9980 2023-04-29 12:03:31.807647 tomcru-0.2.6/tomcru/cfgparsers/BaseCfgParser.py
+-rw-r--r--   0        0        0     3070 2023-04-29 01:53:19.641911 tomcru-0.2.6/tomcru/cfgparsers/EnvParser.py
+-rw-r--r--   0        0        0     1144 2023-04-20 10:17:05.036609 tomcru-0.2.6/tomcru/cfgparsers/MergeCfgParser.py
+-rw-r--r--   0        0        0     5042 2023-05-15 22:40:30.130155 tomcru-0.2.6/tomcru/cfgparsers/SwaggerCfgParser.py
+-rw-r--r--   0        0        0      322 2023-04-23 19:46:42.543716 tomcru-0.2.6/tomcru/cfgparsers/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 19:28:55.917588 tomcru-0.2.6/tomcru/core/__init__.py
+-rw-r--r--   0        0        0     3291 2023-04-29 12:02:24.479889 tomcru-0.2.6/tomcru/core/cfg/api.py
+-rw-r--r--   0        0        0     1164 2023-05-15 22:40:30.130155 tomcru-0.2.6/tomcru/core/cfg/authorizers.py
+-rw-r--r--   0        0        0     3716 2023-04-29 12:01:41.192048 tomcru-0.2.6/tomcru/core/cfg/integrations.py
+-rw-r--r--   0        0        0     2041 2023-04-29 11:52:34.486450 tomcru-0.2.6/tomcru/core/cfg/proj.py
+-rw-r--r--   0        0        0      670 2023-04-29 16:16:10.250867 tomcru-0.2.6/tomcru/core/modloader.py
+-rw-r--r--   0        0        0      833 2023-04-25 19:30:27.561274 tomcru-0.2.6/tomcru/core/obj_store.py
+-rw-r--r--   0        0        0     2989 2023-04-29 17:03:04.510715 tomcru-0.2.6/tomcru/core/project.py
+-rw-r--r--   0        0        0     2227 2023-04-29 16:20:26.534540 tomcru-0.2.6/tomcru/core/servmgr.py
+-rw-r--r--   0        0        0     3802 2023-05-07 01:20:10.626850 tomcru-0.2.6/tomcru/core/utils/MyMetaLoader.py
+-rw-r--r--   0        0        0      104 2023-04-20 13:43:12.977618 tomcru-0.2.6/tomcru/core/utils/__init__.py
+-rw-r--r--   0        0        0     1135 2023-04-20 13:44:18.245442 tomcru-0.2.6/tomcru/core/utils/toml_custom.py
+-rw-r--r--   0        0        0     2462 2023-04-17 18:29:36.252599 tomcru-0.2.6/tomcru/core/utils/yaml_custom.py
+-rw-r--r--   0        0        0       72 2023-05-05 20:11:13.811402 tomcru-0.2.6/tomcru/etc/proxies/aws-sdk/index.js
+-rw-r--r--   0        0        0      261 2023-05-05 20:10:34.172421 tomcru-0.2.6/tomcru/etc/proxies/aws-sdk/package.json
+-rw-r--r--   0        0        0      558 2023-05-05 23:50:53.045569 tomcru-0.2.6/tomcru/etc/proxies/aws-sdk/proxylib.js
+-rw-r--r--   0        0        0      873 2023-05-06 16:59:17.798252 tomcru-0.2.6/tomcru/etc/proxies/aws-sdk/serv/ddb.js
+-rw-r--r--   0        0        0      703 2023-05-06 16:12:42.134096 tomcru-0.2.6/tomcru/etc/proxies/t_proxy.js
+-rw-r--r--   0        0        0      540 2023-04-25 19:12:49.028297 tomcru-0.2.6/tomcru/services/ServiceBase.py
+-rw-r--r--   0        0        0        0 2023-04-17 18:29:36.248599 tomcru-0.2.6/tomcru/services/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 18:29:36.248599 tomcru-0.2.6/tomcru/services/aws/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-23 00:05:26.709577 tomcru-0.2.6/tomcru/services/aws/hosted/apigw/__init__.py
+-rw-r--r--   0        0        0     6799 2023-04-29 12:52:25.243899 tomcru-0.2.6/tomcru/services/aws/hosted/apigw/api_shared/ApiGWBuilderBase.py
+-rw-r--r--   0        0        0        0 2023-04-29 03:09:12.832374 tomcru-0.2.6/tomcru/services/aws/hosted/apigw/api_shared/__init__.py
+-rw-r--r--   0        0        0      835 2023-04-29 11:52:34.482450 tomcru-0.2.6/tomcru/services/aws/hosted/apigw/api_shared/integration/ExternalLambdaAuthorizerIntegration.py
+-rw-r--r--   0        0        0     2688 2023-05-01 08:08:53.636339 tomcru-0.2.6/tomcru/services/aws/hosted/apigw/api_shared/integration/LambdaAuthorizerIntegration.py
+-rw-r--r--   0        0        0     3233 2023-05-15 23:33:20.794748 tomcru-0.2.6/tomcru/services/aws/hosted/apigw/api_shared/integration/OIDCAuthorizerIntegration.py
+-rw-r--r--   0        0        0      711 2023-04-29 11:52:34.510450 tomcru-0.2.6/tomcru/services/aws/hosted/apigw/api_shared/integration/TomcruApiGWHttpIntegration.py
+-rw-r--r--   0        0        0      322 2023-04-29 03:05:19.325205 tomcru-0.2.6/tomcru/services/aws/hosted/apigw/api_shared/integration/__init__.py
+-rw-r--r--   0        0        0     4871 2023-05-01 09:27:22.908562 tomcru-0.2.6/tomcru/services/aws/hosted/apigw/flask_b/ApiGWFlaskBuilder.py
+-rw-r--r--   0        0        0       85 2023-04-21 15:34:30.512217 tomcru-0.2.6/tomcru/services/aws/hosted/apigw/flask_b/__init__.py
+-rw-r--r--   0        0        0      691 2023-04-17 18:29:36.248599 tomcru-0.2.6/tomcru/services/aws/hosted/apigw/flask_b/controllers/EmeProxyController.py
+-rw-r--r--   0        0        0      213 2023-04-17 18:29:36.248599 tomcru-0.2.6/tomcru/services/aws/hosted/apigw/flask_b/controllers/HomeController.py
+-rw-r--r--   0        0        0      236 2023-04-17 18:29:36.248599 tomcru-0.2.6/tomcru/services/aws/hosted/apigw/flask_b/controllers/SwaggerController.py
+-rw-r--r--   0        0        0     4019 2023-05-13 22:36:02.291646 tomcru-0.2.6/tomcru/services/aws/hosted/apigw/flask_b/integration/LambdaIntegration.py
+-rw-r--r--   0        0        0     1808 2023-05-13 22:27:41.433281 tomcru-0.2.6/tomcru/services/aws/hosted/apigw/flask_b/integration/MockedIntegration.py
+-rw-r--r--   0        0        0     2553 2023-04-29 11:52:43.966414 tomcru-0.2.6/tomcru/services/aws/hosted/apigw/flask_b/integration/SwaggerIntegration.py
+-rw-r--r--   0        0        0      148 2023-04-23 17:59:42.203687 tomcru-0.2.6/tomcru/services/aws/hosted/apigw/flask_b/integration/__init__.py
+-rw-r--r--   0        0        0      352 2023-04-21 15:34:30.504217 tomcru-0.2.6/tomcru/services/aws/hosted/apigw/ws_b/ApiGWWebsocketBuilder.py
+-rw-r--r--   0        0        0       97 2023-04-21 15:34:35.936203 tomcru-0.2.6/tomcru/services/aws/hosted/apigw/ws_b/__init__.py
+-rw-r--r--   0        0        0     2994 2023-04-29 11:52:43.946414 tomcru-0.2.6/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/WsAppBuilder.py
+-rw-r--r--   0        0        0       70 2023-04-17 18:29:36.248599 tomcru-0.2.6/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/__init__.py
+-rw-r--r--   0        0        0     1750 2023-04-29 11:53:00.170328 tomcru-0.2.6/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/_jank.py
+-rw-r--r--   0        0        0     3296 2023-04-29 11:52:34.474450 tomcru-0.2.6/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/apps/EmeWsApp.py
+-rw-r--r--   0        0        0     3510 2023-04-29 11:52:43.962414 tomcru-0.2.6/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/LambdaIntegration.py
+-rw-r--r--   0        0        0      185 2023-04-17 18:29:36.248599 tomcru-0.2.6/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/TomcruApiGWWsIntegration.py
+-rw-r--r--   0        0        0      686 2023-04-17 18:29:36.248599 tomcru-0.2.6/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/WsEnRouteCachedAuthorizer.py
+-rw-r--r--   0        0        0      853 2023-04-25 19:16:13.145908 tomcru-0.2.6/tomcru/services/aws/hosted/apigw_manager_b/ApiGWMgr.py
+-rw-r--r--   0        0        0       58 2023-04-23 13:47:38.385293 tomcru-0.2.6/tomcru/services/aws/hosted/apigw_manager_b/__init__.py
+-rw-r--r--   0        0        0     1477 2023-05-07 02:33:51.682008 tomcru-0.2.6/tomcru/services/aws/hosted/boto3_b/Boto3Builder.py
+-rw-r--r--   0        0        0       70 2023-04-17 18:29:36.248599 tomcru-0.2.6/tomcru/services/aws/hosted/boto3_b/__init__.py
+-rw-r--r--   0        0        0      622 2023-05-03 19:16:05.271285 tomcru-0.2.6/tomcru/services/aws/hosted/boto3_b/boto3.py
+-rw-r--r--   0        0        0     1782 2023-04-29 22:03:41.543858 tomcru-0.2.6/tomcru/services/aws/hosted/cloudfront/flask_b/CloudfrontFlaskBuilder.py
+-rw-r--r--   0        0        0      100 2023-04-29 15:54:06.512215 tomcru-0.2.6/tomcru/services/aws/hosted/cloudfront/flask_b/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 18:57:16.415271 tomcru-0.2.6/tomcru/services/aws/hosted/ddb/__init__.py
+-rw-r--r--   0        0        0      993 2023-05-04 12:19:56.412205 tomcru-0.2.6/tomcru/services/aws/hosted/ddb/proxy.py
+-rw-r--r--   0        0        0     8695 2023-05-13 22:09:34.428940 tomcru-0.2.6/tomcru/services/aws/hosted/ddb/sqlalchemy_b/DDBSqlAlchemyTable.py
+-rw-r--r--   0        0        0      971 2023-05-04 22:52:05.711536 tomcru-0.2.6/tomcru/services/aws/hosted/ddb/sqlalchemy_b/DynamoDBBuilder.py
+-rw-r--r--   0        0        0     1134 2023-05-09 21:53:23.860126 tomcru-0.2.6/tomcru/services/aws/hosted/ddb/sqlalchemy_b/SqlAlchemyJSONType.py
+-rw-r--r--   0        0        0       79 2023-04-20 17:41:37.808233 tomcru-0.2.6/tomcru/services/aws/hosted/ddb/sqlalchemy_b/__init__.py
+-rw-r--r--   0        0        0      377 2023-05-09 21:44:42.921751 tomcru-0.2.6/tomcru/services/aws/hosted/ddb/sqlalchemy_b/boto3_proxy.py
+-rw-r--r--   0        0        0     5436 2023-05-09 22:04:01.245469 tomcru-0.2.6/tomcru/services/aws/hosted/ddb/sqlalchemy_b/dal_ddb.py
+-rw-r--r--   0        0        0     4400 2023-05-07 02:33:48.046038 tomcru-0.2.6/tomcru/services/aws/hosted/lambda_b/LambdaBuilder.py
+-rw-r--r--   0        0        0      784 2023-05-01 08:27:27.476570 tomcru-0.2.6/tomcru/services/aws/hosted/lambda_b/LambdaHostedPyContext.py
+-rw-r--r--   0        0        0       74 2023-04-17 18:29:36.248599 tomcru-0.2.6/tomcru/services/aws/hosted/lambda_b/__init__.py
+-rw-r--r--   0        0        0     5074 2023-05-13 17:44:03.162000 tomcru-0.2.6/tomcru/services/aws/hosted/lambda_b/proxy/Py2NodeLambdaProxy.py
+-rw-r--r--   0        0        0     2585 2023-05-12 20:18:40.139204 tomcru-0.2.6/tomcru/services/aws/hosted/s3_b/S3AdapterLocal.py
+-rw-r--r--   0        0        0      585 2023-05-09 23:34:07.782900 tomcru-0.2.6/tomcru/services/aws/hosted/s3_b/S3Service.py
+-rw-r--r--   0        0        0       61 2023-04-25 22:42:25.629435 tomcru-0.2.6/tomcru/services/aws/hosted/s3_b/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 18:29:36.248599 tomcru-0.2.6/tomcru/services/aws/onpremise/__init__.py
+-rw-r--r--   0        0        0     4043 2023-04-29 11:53:00.190328 tomcru-0.2.6/tomcru/services/aws/onpremise/model_checker/SwaggerResponseModelValidator.py
+-rw-r--r--   0        0        0      121 2023-04-17 18:29:36.248599 tomcru-0.2.6/tomcru/services/aws/onpremise/model_checker/__init__.py
+-rw-r--r--   0        0        0      782 2023-04-29 11:52:34.530450 tomcru-0.2.6/tomcru/services/aws/onpremise/s3_static/S3StaticBuilder.py
+-rw-r--r--   0        0        0       78 2023-04-17 18:29:36.248599 tomcru-0.2.6/tomcru/services/aws/onpremise/s3_static/__init__.py
+-rw-r--r--   0        0        0     7308 2023-04-17 18:29:36.248599 tomcru-0.2.6/tomcru/services/aws/sam/_junk/SamTplBuilder.py
+-rw-r--r--   0        0        0      841 2023-04-17 18:29:36.248599 tomcru-0.2.6/tomcru/services/aws/sam/_junk/core.yaml
+-rw-r--r--   0        0        0      855 2023-04-17 18:29:36.248599 tomcru-0.2.6/tomcru/services/aws/sam/_junk/httpapi.yaml
+-rw-r--r--   0        0        0      372 2023-04-17 18:29:36.248599 tomcru-0.2.6/tomcru/services/aws/sam/_junk/integ_normal.yaml
+-rw-r--r--   0        0        0      638 2023-04-17 18:29:36.248599 tomcru-0.2.6/tomcru/services/aws/sam/_junk/integ_ws.yaml
+-rw-r--r--   0        0        0      153 2023-04-17 18:29:36.248599 tomcru-0.2.6/tomcru/services/aws/sam/_junk/lambda.yaml
+-rw-r--r--   0        0        0      231 2023-04-17 18:29:36.248599 tomcru-0.2.6/tomcru/services/aws/sam/_junk/layer.yaml
+-rw-r--r--   0        0        0     4389 2023-04-17 18:29:36.248599 tomcru-0.2.6/tomcru/services/aws/sam/_junk/template.yaml
+-rw-r--r--   0        0        0     1027 2023-04-17 18:29:36.248599 tomcru-0.2.6/tomcru/services/aws/sam/_junk/wsapi.yaml
+-rw-r--r--   0        0        0     2101 2023-04-29 11:53:00.174328 tomcru-0.2.6/tomcru/services/aws/sam/lambda_b/LambdaBuilder.py
+-rw-r--r--   0        0        0       74 2023-04-17 18:29:36.248599 tomcru-0.2.6/tomcru/services/aws/sam/lambda_b/__init__.py
+-rw-r--r--   0        0        0     1344 2023-04-29 11:53:00.154328 tomcru-0.2.6/tomcru/services/aws/sam/params_b/ParametersBuilder.py
+-rw-r--r--   0        0        0       85 2023-04-17 18:29:36.248599 tomcru-0.2.6/tomcru/services/aws/sam/params_b/__init__.py
+-rw-r--r--   0        0        0     2725 2023-04-29 11:53:00.170328 tomcru-0.2.6/tomcru/services/aws/sam/spec_api_b/SwaggerApiTemplater.py
+-rw-r--r--   0        0        0       91 2023-04-17 18:29:36.248599 tomcru-0.2.6/tomcru/services/aws/sam/spec_api_b/__init__.py
+-rw-r--r--   0        0        0     1757 2023-04-29 11:52:34.502450 tomcru-0.2.6/tomcru/services/aws/sam/spec_api_b/authorizers/SAMLambdaAuthBuilder.py
+-rw-r--r--   0        0        0      774 2023-04-29 11:52:34.470450 tomcru-0.2.6/tomcru/services/aws/sam/spec_api_b/authorizers/SAMOIDCAuthBuilder.py
+-rw-r--r--   0        0        0      835 2023-04-29 11:52:43.962414 tomcru-0.2.6/tomcru/services/aws/sam/spec_api_b/integrations/SAMLambdaBuilder.py
+-rw-r--r--   0        0        0     2266 2023-04-29 11:52:43.970414 tomcru-0.2.6/tomcru/services/general/eme2swagger/Eme2Swagger.py
+-rw-r--r--   0        0        0       67 2023-04-17 18:29:36.252599 tomcru-0.2.6/tomcru/services/general/eme2swagger/__init__.py
+-rw-r--r--   0        0        0     1047 1970-01-01 00:00:00.000000 tomcru-0.2.6/PKG-INFO
```

### Comparing `tomcru-0.2.5/LICENSE` & `tomcru-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/pyproject.toml` & `tomcru-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tomcru"
-version = "0.2.5"
+version = "0.2.6"
 description = "Serverless app framework"
 authors = ["Rajmund Csombordi <rajmund.csombordi@hotmail.com>"]
 readme = "README.md"
 packages = [{include = "tomcru"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `tomcru-0.2.5/tomcru/appbuilders/envmapping.py` & `tomcru-0.2.6/tomcru/appbuilders/envmapping.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/appbuilders/faas/InjectableAppBase.py` & `tomcru-0.2.6/tomcru/appbuilders/faas/InjectableAppBase.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/appbuilders/faas/sam_app/SamAppBuilder.py` & `tomcru-0.2.6/tomcru/appbuilders/faas/sam_app/SamAppBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/appbuilders/faas/static_app/StaticAppBuilder.py` & `tomcru-0.2.6/tomcru/appbuilders/faas/static_app/StaticAppBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/cfgparsers/BaseCfgParser.py` & `tomcru-0.2.6/tomcru/cfgparsers/BaseCfgParser.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/cfgparsers/EnvParser.py` & `tomcru-0.2.6/tomcru/cfgparsers/EnvParser.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/cfgparsers/MergeCfgParser.py` & `tomcru-0.2.6/tomcru/cfgparsers/MergeCfgParser.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/cfgparsers/SwaggerCfgParser.py` & `tomcru-0.2.6/tomcru/cfgparsers/SwaggerCfgParser.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,14 @@
 
             return TomcruApiLambdaAuthorizerEP(auth_id, lambda_id, group, _in, _name)
         elif spec['type'] == 'openIdConnect':
             # openapi3 doesn't allow in/name for openIdConnect, so authorization header is set static
 
             # oidc endpoint is going to be redundant because SAM also requires it
             endpoint = spec['openIdConnectUrl']
-            oidc_cfg = spec.pop('x-oidc')
+            # oidc_cfg = spec.pop('x-oidc')
 
-            return TomcruApiOIDCAuthorizerEP(auth_id, endpoint, oidc_cfg.get('audience'), oidc_cfg.get('scopes'))
+            return TomcruApiOIDCAuthorizerEP(auth_id, endpoint)
         elif spec['type'] == 'oauth2':
             raise NotImplementedError("we don't know how to implement this LOL")
         else:
             raise NotImplementedError("")
```

### Comparing `tomcru-0.2.5/tomcru/core/cfg/api.py` & `tomcru-0.2.6/tomcru/core/cfg/api.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/core/cfg/authorizers.py` & `tomcru-0.2.6/tomcru/core/cfg/authorizers.py`

 * *Files 17% similar despite different names*

```diff
@@ -28,20 +28,18 @@
 
     @property
     def lambda_id(self):
         return self.lambda_source+'/'+self.integ_id
 
 
 class TomcruApiOIDCAuthorizerEP(TomcruApiAuthorizerEP):
-    def __init__(self, auth_id, endpoint, audience, scopes):
+    def __init__(self, auth_id, endpoint):
         """
 
         :param auth_type:
         :param integ_id:
         """
         super().__init__(auth_id, 'oidc', endpoint)
-        self.audience = audience
-        self.scopes = scopes
 
     @property
     def endpoint_url(self):
         return self.integ_id
```

### Comparing `tomcru-0.2.5/tomcru/core/cfg/integrations.py` & `tomcru-0.2.6/tomcru/core/cfg/integrations.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/core/cfg/proj.py` & `tomcru-0.2.6/tomcru/core/cfg/proj.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/core/modloader.py` & `tomcru-0.2.6/tomcru/core/modloader.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/core/obj_store.py` & `tomcru-0.2.6/tomcru/core/obj_store.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/core/project.py` & `tomcru-0.2.6/tomcru/core/project.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/core/servmgr.py` & `tomcru-0.2.6/tomcru/core/servmgr.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/core/utils/MyMetaLoader.py` & `tomcru-0.2.6/tomcru/core/utils/MyMetaLoader.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/core/utils/toml_custom.py` & `tomcru-0.2.6/tomcru/core/utils/toml_custom.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/core/utils/yaml_custom.py` & `tomcru-0.2.6/tomcru/core/utils/yaml_custom.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/etc/proxies/aws-sdk/proxylib.js` & `tomcru-0.2.6/tomcru/etc/proxies/aws-sdk/proxylib.js`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/etc/proxies/aws-sdk/serv/ddb.js` & `tomcru-0.2.6/tomcru/etc/proxies/aws-sdk/serv/ddb.js`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/etc/proxies/t_proxy.js` & `tomcru-0.2.6/tomcru/etc/proxies/t_proxy.js`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/services/ServiceBase.py` & `tomcru-0.2.6/tomcru/services/ServiceBase.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/services/aws/hosted/apigw/api_shared/ApiGWBuilderBase.py` & `tomcru-0.2.6/tomcru/services/aws/hosted/apigw/api_shared/ApiGWBuilderBase.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/services/aws/hosted/apigw/api_shared/integration/ExternalLambdaAuthorizerIntegration.py` & `tomcru-0.2.6/tomcru/services/aws/hosted/apigw/api_shared/integration/ExternalLambdaAuthorizerIntegration.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/services/aws/hosted/apigw/api_shared/integration/LambdaAuthorizerIntegration.py` & `tomcru-0.2.6/tomcru/services/aws/hosted/apigw/api_shared/integration/LambdaAuthorizerIntegration.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/services/aws/hosted/apigw/api_shared/integration/OIDCAuthorizerIntegration.py` & `tomcru-0.2.6/tomcru/services/aws/hosted/apigw/api_shared/integration/OIDCAuthorizerIntegration.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 import requests
 
 from .TomcruApiGWHttpIntegration import TomcruApiGWAuthorizerIntegration
 from tomcru import TomcruApiOIDCAuthorizerEP
 
+
 class AWSOIDCException(Exception):
     pass
 
 
 class OIDCAuthorizerIntegration(TomcruApiGWAuthorizerIntegration):
 
     def __init__(self, cfg: TomcruApiOIDCAuthorizerEP, auth_cfg, env=None):
         super().__init__(cfg)
         self.env = env
 
-        self.oidc_ep = cfg.endpoint_url
-        self.audience = cfg.audience
-        self.scopes = cfg.scopes # this is redundant (scopes_supported is fetched from OIDC ep); but AWS requires to be checked
+        # OIDC config from swagger file (& envspec override):
+        self.oidc_ep = auth_cfg.get(f'authorizers.{cfg.auth_id}.url_override', cfg.endpoint_url)
+        self.audience = auth_cfg.get(f'authorizers.{cfg.auth_id}.audience')
 
-        # OIDC endpoint:
+        # remote OIDC endpoint information:
         self.initialized = False
         self.scopes_supported: list = None
         self.issuer = None
         self.jwks_client = None
 
     def authorize(self, event: dict):
-        jwt = self._initialize_oidc()
+        import jwt
+
+        # initialize OIDC endpoint
+        if not self.initialized:
+            oidc_cfg = self._fetch_oidc_endpoint()
+            self.jwks_client = jwt.PyJWKClient(oidc_cfg['jwks_uri'], cache_jwk_set=True, lifespan=900)
 
         if 'authorization' not in event['headers']:
             return None
         try:
             prefix, token_jwt = event['headers']['authorization'].split(" ")
             assert prefix.lower() in ('bearer', 'jwt')
 
@@ -55,43 +61,35 @@
         except (jwt.InvalidTokenError, AWSOIDCException) as e:
             raise e
             # invalidated claims -> authorizer refuses the token
             print("Auth error: ", e)
             return None
 
     def verify_claims(self, data: dict):
-        # TODO: ITT: what other stuff we need to check that JWT lib doesn't?
         _scope = data.get('scp', data.get('scope', None))
 
-        if self.scopes:
+        # validate: The token must include at least one of the scopes in the route's authorizationScopes
+        #self.scope, self.scopes_supported
+
+        if self.scopes_supported:
             if not _scope:
                 raise AWSOIDCException("no scope provided in JWT")
-            elif _scope not in self.scopes:
+            elif _scope not in self.scopes_supported:
                 raise AWSOIDCException("scope validation error")
 
         return _scope
 
-    def _initialize_oidc(self):
-        import jwt
-        if self.initialized:
-            return False
-
-        # fetch OIDC endpoint and find JWKS
+    def _fetch_oidc_endpoint(self):
         headers = {'Accept': 'application/json'}
         try:
             r = requests.get(self.oidc_ep, headers=headers)
         except requests.exceptions.ConnectionError:
             raise AWSOIDCException()
 
-        # TODO: ITT: how to refer to localhost instead of pythonanywhere?
         if r.status_code != 200:
             raise AWSOIDCException()
         oidc = r.json()
 
         self.issuer = oidc['issuer']
         self.scopes_supported = oidc['scopes_supported']
-        # validate: The token must include at least one of the scopes in the route's authorizationScopes
-        #self.scope, self.scopes_supported
-
-        self.jwks_client = jwt.PyJWKClient(oidc['jwks_uri'], cache_jwk_set=True, lifespan=900)
 
-        return jwt
+        return oidc
```

### Comparing `tomcru-0.2.5/tomcru/services/aws/hosted/apigw/api_shared/integration/TomcruApiGWHttpIntegration.py` & `tomcru-0.2.6/tomcru/services/aws/hosted/apigw/api_shared/integration/TomcruApiGWHttpIntegration.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/services/aws/hosted/apigw/flask_b/ApiGWFlaskBuilder.py` & `tomcru-0.2.6/tomcru/services/aws/hosted/apigw/flask_b/ApiGWFlaskBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/services/aws/hosted/apigw/flask_b/controllers/EmeProxyController.py` & `tomcru-0.2.6/tomcru/services/aws/hosted/apigw/flask_b/controllers/EmeProxyController.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/services/aws/hosted/apigw/flask_b/integration/LambdaIntegration.py` & `tomcru-0.2.6/tomcru/services/aws/hosted/apigw/flask_b/integration/LambdaIntegration.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/services/aws/hosted/apigw/flask_b/integration/MockedIntegration.py` & `tomcru-0.2.6/tomcru/services/aws/hosted/apigw/flask_b/integration/MockedIntegration.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/services/aws/hosted/apigw/flask_b/integration/SwaggerIntegration.py` & `tomcru-0.2.6/tomcru/services/aws/hosted/apigw/flask_b/integration/SwaggerIntegration.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/WsAppBuilder.py` & `tomcru-0.2.6/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/WsAppBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/_jank.py` & `tomcru-0.2.6/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/_jank.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/apps/EmeWsApp.py` & `tomcru-0.2.6/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/apps/EmeWsApp.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/LambdaIntegration.py` & `tomcru-0.2.6/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/LambdaIntegration.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/WsEnRouteCachedAuthorizer.py` & `tomcru-0.2.6/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/WsEnRouteCachedAuthorizer.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/services/aws/hosted/apigw_manager_b/ApiGWMgr.py` & `tomcru-0.2.6/tomcru/services/aws/hosted/apigw_manager_b/ApiGWMgr.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/services/aws/hosted/boto3_b/Boto3Builder.py` & `tomcru-0.2.6/tomcru/services/aws/hosted/boto3_b/Boto3Builder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/services/aws/hosted/boto3_b/boto3.py` & `tomcru-0.2.6/tomcru/services/aws/hosted/boto3_b/boto3.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/services/aws/hosted/cloudfront/flask_b/CloudfrontFlaskBuilder.py` & `tomcru-0.2.6/tomcru/services/aws/hosted/cloudfront/flask_b/CloudfrontFlaskBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/services/aws/hosted/ddb/proxy.py` & `tomcru-0.2.6/tomcru/services/aws/hosted/ddb/proxy.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/services/aws/hosted/ddb/sqlalchemy_b/DDBSqlAlchemyTable.py` & `tomcru-0.2.6/tomcru/services/aws/hosted/ddb/sqlalchemy_b/DDBSqlAlchemyTable.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/services/aws/hosted/ddb/sqlalchemy_b/DynamoDBBuilder.py` & `tomcru-0.2.6/tomcru/services/aws/hosted/ddb/sqlalchemy_b/DynamoDBBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/services/aws/hosted/ddb/sqlalchemy_b/SqlAlchemyJSONType.py` & `tomcru-0.2.6/tomcru/services/aws/hosted/ddb/sqlalchemy_b/SqlAlchemyJSONType.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/services/aws/hosted/ddb/sqlalchemy_b/dal_ddb.py` & `tomcru-0.2.6/tomcru/services/aws/hosted/ddb/sqlalchemy_b/dal_ddb.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/services/aws/hosted/lambda_b/LambdaBuilder.py` & `tomcru-0.2.6/tomcru/services/aws/hosted/lambda_b/LambdaBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/services/aws/hosted/lambda_b/LambdaHostedPyContext.py` & `tomcru-0.2.6/tomcru/services/aws/hosted/lambda_b/LambdaHostedPyContext.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/services/aws/hosted/lambda_b/proxy/Py2NodeLambdaProxy.py` & `tomcru-0.2.6/tomcru/services/aws/hosted/lambda_b/proxy/Py2NodeLambdaProxy.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/services/aws/hosted/s3_b/S3AdapterLocal.py` & `tomcru-0.2.6/tomcru/services/aws/hosted/s3_b/S3AdapterLocal.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/services/aws/hosted/s3_b/S3Service.py` & `tomcru-0.2.6/tomcru/services/aws/hosted/s3_b/S3Service.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/services/aws/onpremise/model_checker/SwaggerResponseModelValidator.py` & `tomcru-0.2.6/tomcru/services/aws/onpremise/model_checker/SwaggerResponseModelValidator.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/services/aws/onpremise/s3_static/S3StaticBuilder.py` & `tomcru-0.2.6/tomcru/services/aws/onpremise/s3_static/S3StaticBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/services/aws/sam/_junk/SamTplBuilder.py` & `tomcru-0.2.6/tomcru/services/aws/sam/_junk/SamTplBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/services/aws/sam/_junk/core.yaml` & `tomcru-0.2.6/tomcru/services/aws/sam/_junk/core.yaml`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/services/aws/sam/_junk/httpapi.yaml` & `tomcru-0.2.6/tomcru/services/aws/sam/_junk/httpapi.yaml`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/services/aws/sam/_junk/integ_ws.yaml` & `tomcru-0.2.6/tomcru/services/aws/sam/_junk/integ_ws.yaml`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/services/aws/sam/_junk/template.yaml` & `tomcru-0.2.6/tomcru/services/aws/sam/_junk/template.yaml`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/services/aws/sam/_junk/wsapi.yaml` & `tomcru-0.2.6/tomcru/services/aws/sam/_junk/wsapi.yaml`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/services/aws/sam/lambda_b/LambdaBuilder.py` & `tomcru-0.2.6/tomcru/services/aws/sam/lambda_b/LambdaBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/services/aws/sam/params_b/ParametersBuilder.py` & `tomcru-0.2.6/tomcru/services/aws/sam/params_b/ParametersBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/services/aws/sam/spec_api_b/SwaggerApiTemplater.py` & `tomcru-0.2.6/tomcru/services/aws/sam/spec_api_b/SwaggerApiTemplater.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/services/aws/sam/spec_api_b/authorizers/SAMLambdaAuthBuilder.py` & `tomcru-0.2.6/tomcru/services/aws/sam/spec_api_b/authorizers/SAMLambdaAuthBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/services/aws/sam/spec_api_b/authorizers/SAMOIDCAuthBuilder.py` & `tomcru-0.2.6/tomcru/services/aws/sam/spec_api_b/authorizers/SAMOIDCAuthBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/services/aws/sam/spec_api_b/integrations/SAMLambdaBuilder.py` & `tomcru-0.2.6/tomcru/services/aws/sam/spec_api_b/integrations/SAMLambdaBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/tomcru/services/general/eme2swagger/Eme2Swagger.py` & `tomcru-0.2.6/tomcru/services/general/eme2swagger/Eme2Swagger.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.5/PKG-INFO` & `tomcru-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomcru
-Version: 0.2.5
+Version: 0.2.6
 Summary: Serverless app framework
 Author: Rajmund Csombordi
 Author-email: rajmund.csombordi@hotmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

