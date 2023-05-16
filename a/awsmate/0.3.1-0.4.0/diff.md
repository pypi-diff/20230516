# Comparing `tmp/awsmate-0.3.1.tar.gz` & `tmp/awsmate-0.4.0.tar.gz`

## Comparing `awsmate-0.3.1.tar` & `awsmate-0.4.0.tar`

### file list

```diff
@@ -1,65 +1,71 @@
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 awsmate-0.3.1/.readthedocs.yaml
--rw-r--r--   0        0        0     6137 2020-02-02 00:00:00.000000 awsmate-0.3.1/CHANGELOG.md
--rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 awsmate-0.3.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 awsmate-0.3.1/CONTRIBUTING.md
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 awsmate-0.3.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 awsmate-0.3.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 awsmate-0.3.1/.github/workflows/tests.yaml
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 awsmate-0.3.1/docs/requirements.txt
--rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 awsmate-0.3.1/docs/source/apigateway.rst
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 awsmate-0.3.1/docs/source/awsmate.rst
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 awsmate-0.3.1/docs/source/changelog.rst
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 awsmate-0.3.1/docs/source/code_of_conduct.rst
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 awsmate-0.3.1/docs/source/conf.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 awsmate-0.3.1/docs/source/contributing.rst
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 awsmate-0.3.1/docs/source/eventbridge.rst
--rw-r--r--   0        0        0    12611 2020-02-02 00:00:00.000000 awsmate-0.3.1/docs/source/example_application.rst
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 awsmate-0.3.1/docs/source/genindex.rst
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 awsmate-0.3.1/docs/source/index.rst
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 awsmate-0.3.1/docs/source/lambdafunction.rst
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 awsmate-0.3.1/docs/source/logger.rst
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 awsmate-0.3.1/docs/source/readme.rst
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 awsmate-0.3.1/docs/source/release_process.rst
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 awsmate-0.3.1/docs/source/s3.rst
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 awsmate-0.3.1/docs/source/testing.rst
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 awsmate-0.3.1/docs/source/_static/flyout.js
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 awsmate-0.3.1/docs/source/_static/theme.css
--rwxr-xr-x   0        0        0     1607 2020-02-02 00:00:00.000000 awsmate-0.3.1/docs/source/_templates/layout.html
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 awsmate-0.3.1/example/check_terraform
--rwxr-xr-x   0        0        0      183 2020-02-02 00:00:00.000000 awsmate-0.3.1/example/deploy.sh
--rwxr-xr-x   0        0        0      185 2020-02-02 00:00:00.000000 awsmate-0.3.1/example/undeploy.sh
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 awsmate-0.3.1/example/variables.tfvars
--rwxr-xr-x   0        0        0     1102 2020-02-02 00:00:00.000000 awsmate-0.3.1/example/src/lambda_apigateway_returns_403.py
--rwxr-xr-x   0        0        0     1808 2020-02-02 00:00:00.000000 awsmate-0.3.1/example/src/lambda_apigateway_returns_500.py
--rwxr-xr-x   0        0        0     3738 2020-02-02 00:00:00.000000 awsmate-0.3.1/example/src/lambda_apigateway_returns_okay.py
--rwxr-xr-x   0        0        0      465 2020-02-02 00:00:00.000000 awsmate-0.3.1/example/src/lambda_eventbridge_scheduler.py
--rwxr-xr-x   0        0        0      394 2020-02-02 00:00:00.000000 awsmate-0.3.1/example/src/lambda_logger.py
--rwxr-xr-x   0        0        0      742 2020-02-02 00:00:00.000000 awsmate-0.3.1/example/src/lambda_s3_notification.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 awsmate-0.3.1/example/tf/00-provider.tf
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 awsmate-0.3.1/example/tf/00-variables.tf
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 awsmate-0.3.1/example/tf/01-lambda-iam-role.tf
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 awsmate-0.3.1/example/tf/02-awsmate-lambda-layer.tf
--rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 awsmate-0.3.1/example/tf/03-apigateway-lambda-functions.tf
--rw-r--r--   0        0        0     6745 2020-02-02 00:00:00.000000 awsmate-0.3.1/example/tf/04-apigateway.tf
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 awsmate-0.3.1/example/tf/05-eventbridge-lambda-functions.tf
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 awsmate-0.3.1/example/tf/06-eventbridge-iam-role.tf
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 awsmate-0.3.1/example/tf/07-eventbridge-scheduler.tf
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 awsmate-0.3.1/example/tf/08-s3-bucket.tf
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 awsmate-0.3.1/example/tf/09-s3-lambda-functions.tf
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 awsmate-0.3.1/example/tf/10-logger-lambda-functions.tf
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 awsmate-0.3.1/src/awsmate/__init__.py
--rw-r--r--   0        0        0    52826 2020-02-02 00:00:00.000000 awsmate-0.3.1/src/awsmate/apigateway.py
--rw-r--r--   0        0        0     4242 2020-02-02 00:00:00.000000 awsmate-0.3.1/src/awsmate/eventbridge.py
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 awsmate-0.3.1/src/awsmate/lambdafunction.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 awsmate-0.3.1/src/awsmate/logger.py
--rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 awsmate-0.3.1/src/awsmate/s3.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 awsmate-0.3.1/tests/conftest.py
--rw-r--r--   0        0        0    34262 2020-02-02 00:00:00.000000 awsmate-0.3.1/tests/unit/test_apigateway.py
--rw-r--r--   0        0        0     3158 2020-02-02 00:00:00.000000 awsmate-0.3.1/tests/unit/test_eventbridge.py
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 awsmate-0.3.1/tests/unit/test_lambdafunction.py
--rw-r--r--   0        0        0    15684 2020-02-02 00:00:00.000000 awsmate-0.3.1/tests/unit/test_s3.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 awsmate-0.3.1/.gitignore
--rw-r--r--   0        0        0    13827 2020-02-02 00:00:00.000000 awsmate-0.3.1/LICENSE.txt
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 awsmate-0.3.1/README.md
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 awsmate-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 awsmate-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 awsmate-0.4.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     6933 2020-02-02 00:00:00.000000 awsmate-0.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 awsmate-0.4.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 awsmate-0.4.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 awsmate-0.4.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 awsmate-0.4.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 awsmate-0.4.0/.github/workflows/tests.yaml
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 awsmate-0.4.0/docs/requirements.txt
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 awsmate-0.4.0/docs/source/apigateway.rst
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 awsmate-0.4.0/docs/source/awsmate.rst
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 awsmate-0.4.0/docs/source/changelog.rst
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 awsmate-0.4.0/docs/source/code_of_conduct.rst
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 awsmate-0.4.0/docs/source/conf.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 awsmate-0.4.0/docs/source/contributing.rst
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 awsmate-0.4.0/docs/source/eventbridge.rst
+-rw-r--r--   0        0        0    13773 2020-02-02 00:00:00.000000 awsmate-0.4.0/docs/source/example_application.rst
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 awsmate-0.4.0/docs/source/genindex.rst
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 awsmate-0.4.0/docs/source/index.rst
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 awsmate-0.4.0/docs/source/lambdafunction.rst
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 awsmate-0.4.0/docs/source/logger.rst
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 awsmate-0.4.0/docs/source/readme.rst
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 awsmate-0.4.0/docs/source/release_process.rst
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 awsmate-0.4.0/docs/source/s3.rst
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 awsmate-0.4.0/docs/source/sns.rst
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 awsmate-0.4.0/docs/source/testing.rst
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 awsmate-0.4.0/docs/source/_static/flyout.js
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 awsmate-0.4.0/docs/source/_static/theme.css
+-rwxr-xr-x   0        0        0     1607 2020-02-02 00:00:00.000000 awsmate-0.4.0/docs/source/_templates/layout.html
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 awsmate-0.4.0/example/check_terraform
+-rwxr-xr-x   0        0        0      183 2020-02-02 00:00:00.000000 awsmate-0.4.0/example/deploy.sh
+-rwxr-xr-x   0        0        0      185 2020-02-02 00:00:00.000000 awsmate-0.4.0/example/undeploy.sh
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 awsmate-0.4.0/example/variables.tfvars
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 awsmate-0.4.0/example/src/lambda_apigateway_returns_403.py
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 awsmate-0.4.0/example/src/lambda_apigateway_returns_500.py
+-rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 awsmate-0.4.0/example/src/lambda_apigateway_returns_okay.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 awsmate-0.4.0/example/src/lambda_eventbridge_scheduler.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 awsmate-0.4.0/example/src/lambda_logger.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 awsmate-0.4.0/example/src/lambda_s3_notification.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 awsmate-0.4.0/example/src/lambda_sns_message.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 awsmate-0.4.0/example/tf/00-provider.tf
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 awsmate-0.4.0/example/tf/00-variables.tf
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 awsmate-0.4.0/example/tf/01-lambda-iam-role.tf
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 awsmate-0.4.0/example/tf/02-awsmate-lambda-layer.tf
+-rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 awsmate-0.4.0/example/tf/03-apigateway-lambda-functions.tf
+-rw-r--r--   0        0        0     6745 2020-02-02 00:00:00.000000 awsmate-0.4.0/example/tf/04-apigateway.tf
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 awsmate-0.4.0/example/tf/05-eventbridge-lambda-functions.tf
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 awsmate-0.4.0/example/tf/06-eventbridge-iam-role.tf
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 awsmate-0.4.0/example/tf/07-eventbridge-scheduler.tf
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 awsmate-0.4.0/example/tf/08-s3-bucket.tf
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 awsmate-0.4.0/example/tf/09-s3-lambda-functions.tf
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 awsmate-0.4.0/example/tf/10-sns-topic.tf
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 awsmate-0.4.0/example/tf/11-sns-lambda-functions.tf
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 awsmate-0.4.0/example/tf/12-logger-lambda-functions.tf
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 awsmate-0.4.0/src/awsmate/__init__.py
+-rw-r--r--   0        0        0    52834 2020-02-02 00:00:00.000000 awsmate-0.4.0/src/awsmate/apigateway.py
+-rw-r--r--   0        0        0     4242 2020-02-02 00:00:00.000000 awsmate-0.4.0/src/awsmate/eventbridge.py
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 awsmate-0.4.0/src/awsmate/lambdafunction.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 awsmate-0.4.0/src/awsmate/logger.py
+-rw-r--r--   0        0        0     6313 2020-02-02 00:00:00.000000 awsmate-0.4.0/src/awsmate/s3.py
+-rw-r--r--   0        0        0    10713 2020-02-02 00:00:00.000000 awsmate-0.4.0/src/awsmate/sns.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 awsmate-0.4.0/tests/conftest.py
+-rw-r--r--   0        0        0    34262 2020-02-02 00:00:00.000000 awsmate-0.4.0/tests/unit/test_apigateway.py
+-rw-r--r--   0        0        0     3158 2020-02-02 00:00:00.000000 awsmate-0.4.0/tests/unit/test_eventbridge.py
+-rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 awsmate-0.4.0/tests/unit/test_lambdafunction.py
+-rw-r--r--   0        0        0    13880 2020-02-02 00:00:00.000000 awsmate-0.4.0/tests/unit/test_s3.py
+-rw-r--r--   0        0        0    30158 2020-02-02 00:00:00.000000 awsmate-0.4.0/tests/unit/test_sns.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 awsmate-0.4.0/.gitignore
+-rw-r--r--   0        0        0    13827 2020-02-02 00:00:00.000000 awsmate-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 awsmate-0.4.0/README.md
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 awsmate-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 awsmate-0.4.0/PKG-INFO
```

### Comparing `awsmate-0.3.1/CHANGELOG.md` & `awsmate-0.4.0/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,48 @@
 All notable changes to this project are documented in this file.
 
+## [0.4.0] - 2023-05-16
+
+### Added
+
+- Code
+    - initiated ``awsmate.sns`` module with ``awsmate.sns.LambdaMessageEvent``
+
+- Example application
+    - Python and Terraform source code to demonstrate `awsmate.sns`
+
+### Changed
+
+- Code
+    - transparently moved code from class ``awsmate.s3.LambdaNotificationEvent`` to ``awsmate.lambdafunction.LambdaEvent`` for mutualization
+
+- Example application
+    - Terraform version upgrade
+    
+### Deprecated
+
+*nothing*
+
+### Removed
+
+*nothing*
+
+### Fixed
+
+- Code
+    - ``awsmate.apigateway.LambdaProxyEvent.__init__()``: fixed return type hint
+    - ``awsmate.s3.LambdaNotificationEvent.__init__()``: fixed return type hint
+
+- Example application
+    - Fixed erroneous S3 bucket ACL in Terraform code that is now rejected by AWS
+
+### Security
+
+*nothing*
+
 ## [0.3.1] - 2023-04-28
 
 ### Added
 
 *nothing*
 
 ### Changed
```

### Comparing `awsmate-0.3.1/CODE_OF_CONDUCT.md` & `awsmate-0.4.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.1/CONTRIBUTING.md` & `awsmate-0.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.1/.github/ISSUE_TEMPLATE/feature_request.md` & `awsmate-0.4.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.1/.github/workflows/tests.yaml` & `awsmate-0.4.0/.github/workflows/tests.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: Automated tests
+name: automated tests
 
 on: [push]
 
 jobs:
   test:
     runs-on: ubuntu-latest
     strategy:
```

### Comparing `awsmate-0.3.1/docs/source/apigateway.rst` & `awsmate-0.4.0/docs/source/apigateway.rst`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.1/docs/source/conf.py` & `awsmate-0.4.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.1/docs/source/example_application.rst` & `awsmate-0.4.0/docs/source/example_application.rst`

 * *Files 3% similar despite different names*

```diff
@@ -205,27 +205,57 @@
                 |___src
                      |
                      |___lambda_s3_notification.py
 
 
 * Use
     * Step by step instructions
-        * Go to the S3 service page
+        * Go to the S3 service page of the AWS Console
         * Open the page of the S3 bucket ``awsmate-drop-files-here-<your AWS account number>``
         * Upload a file into this bucket
         * Go to the Cloudwatch service page of the AWS Console
         * Follow the "Logs/Log group" link of the left navigation panel
         * Search for the ``/aws/lambda/awsmate_s3_notification`` log group and open it
         * Open the most recent log stream
         * This show a log that contains the result of all methods of :class:`awsmate.s3.LambdaNotificationEvent` plus the raw event received from the AWS S3 service.
     * This demonstrates
         * the use of all methods of :class:`awsmate.s3.LambdaNotificationEvent`
     * Tip: try to delete a file from the S3 bucket and see the corresponding log, try to drop or delete several files in a single action
 
 
+SNS features: :doc:`sns <sns>` module
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+* Relevant source files
+
+::
+
+    awsmate
+        |___example
+                |
+                |___src
+                     |
+                     |___lambda_sns_message.py
+
+
+* Use
+    * Step by step instructions
+        * Go to the SNS service page of the AWS Console
+        * Follow the "Topics" link of the left navigation panel
+        * Open the page of the topic ``awsmate_demo``
+        * Click on the "Publish message" button located at the top-right corner of the screen
+        * Fill the form with the content you decide 
+        * Go to the Cloudwatch service page of the AWS Console
+        * Follow the "Logs/Log group" link of the left navigation panel
+        * Search for the ``/aws/lambda/awsmate_sns_message`` log group and open it
+        * Open the most recent log stream
+        * This show a log that contains the result of all methods of :class:`awsmate.sns.LambdaMessageEvent` plus the raw event received from the AWS SNS service.        
+    * This demonstrates
+        * the use of all methods of :class:`awsmate.sns.LambdaMessageEvent`
+
 .. _LoggerFeatures:
 
 Logger features: :doc:`logger <logger>` module
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 * Relevant source files
```

### Comparing `awsmate-0.3.1/docs/source/release_process.rst` & `awsmate-0.4.0/docs/source/release_process.rst`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.1/docs/source/_static/flyout.js` & `awsmate-0.4.0/docs/source/_static/flyout.js`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.1/docs/source/_templates/layout.html` & `awsmate-0.4.0/docs/source/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.1/example/check_terraform` & `awsmate-0.4.0/example/check_terraform`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 }
 
 notSupportedArch () {
   echo >&1 "Sorry, Terraform $TERRAFORM_VERSION is unlikely to be available for this architecture."
   exit 1
 }
 
-TERRAFORM_VERSION='1.4.5'
+TERRAFORM_VERSION='1.4.6'
 
 BUILD_DIR='.build'
 
 EXE_EXT=''
 OS_PART=''
 ARCH_PART=''
```

### Comparing `awsmate-0.3.1/example/src/lambda_apigateway_returns_403.py` & `awsmate-0.4.0/example/src/lambda_apigateway_returns_403.py`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.1/example/src/lambda_apigateway_returns_500.py` & `awsmate-0.4.0/example/src/lambda_apigateway_returns_500.py`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.1/example/src/lambda_apigateway_returns_okay.py` & `awsmate-0.4.0/example/src/lambda_apigateway_returns_okay.py`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.1/example/src/lambda_s3_notification.py` & `awsmate-0.4.0/example/src/lambda_s3_notification.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import site
 site.addsitedir('/opt')
 
 import json 
 
-from awsmate.logger import logger, log_internal_error
+from awsmate.logger import logger
 from awsmate.s3 import LambdaNotificationEvent
 
 
 def lambda_handler(raw_event, context):
     event = LambdaNotificationEvent(raw_event)
 
     logger.info(f'event.event_name(): {event.event_name()}')
```

### Comparing `awsmate-0.3.1/example/tf/01-lambda-iam-role.tf` & `awsmate-0.4.0/example/tf/01-lambda-iam-role.tf`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.1/example/tf/03-apigateway-lambda-functions.tf` & `awsmate-0.4.0/example/tf/03-apigateway-lambda-functions.tf`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.1/example/tf/04-apigateway.tf` & `awsmate-0.4.0/example/tf/04-apigateway.tf`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.1/example/tf/05-eventbridge-lambda-functions.tf` & `awsmate-0.4.0/example/tf/05-eventbridge-lambda-functions.tf`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.1/example/tf/06-eventbridge-iam-role.tf` & `awsmate-0.4.0/example/tf/06-eventbridge-iam-role.tf`

 * *Files 14% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     description = "Invoke policy"
 
     policy = <<EOF
 {
     "Version": "2012-10-17",
     "Statement": [
         {
-            "Sid": "InvokeDataprovidersLambdaFunctions",
+            "Sid": "InvokeSchedulerTargetLambdaFunctions",
             "Effect": "Allow",
             "Action": [
                 "lambda:InvokeFunction"
             ],
             "Resource": [
                 "${aws_lambda_function.eventbridge_scheduler.arn}"
             ]
```

### Comparing `awsmate-0.3.1/example/tf/08-s3-bucket.tf` & `awsmate-0.4.0/example/tf/08-s3-bucket.tf`

 * *Files 4% similar despite different names*

```diff
@@ -2,20 +2,14 @@
 
 resource "aws_s3_bucket" "demo_notifications" {
     bucket = "awsmate-drop-files-here-${data.aws_caller_identity.current.account_id}" // bucket names must be unique across all AWS accounts
 
     force_destroy = true
 }
 
-resource "aws_s3_bucket_acl" "demo_notifications" {
-    bucket = aws_s3_bucket.demo_notifications.bucket
-
-    acl    = "private"
-}
-
 resource "aws_s3_bucket_public_access_block" "demo_notifications" {
     bucket = aws_s3_bucket.demo_notifications.bucket
 
     block_public_acls       = true
     block_public_policy     = true
     ignore_public_acls      = true
     restrict_public_buckets = true
```

### Comparing `awsmate-0.3.1/example/tf/09-s3-lambda-functions.tf` & `awsmate-0.4.0/example/tf/09-s3-lambda-functions.tf`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.1/example/tf/10-logger-lambda-functions.tf` & `awsmate-0.4.0/example/tf/12-logger-lambda-functions.tf`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.1/src/awsmate/apigateway.py` & `awsmate-0.4.0/src/awsmate/apigateway.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 class LambdaProxyEvent(LambdaEvent):
     """
     Mapping of the input event received by an AWS Lambda function triggered by AWS API Gateway and integrated 
     in `AWS_PROXY <https://docs.aws.amazon.com/apigateway/latest/developerguide/api-gateway-set-up-simple-proxy.html>`_ mode.
     """
 
-    def __init__(self, event_object: dict):
+    def __init__(self, event_object: dict) -> None:
         """
         Parameters
         ----------
         event_object : dict
             The parameter ``event`` received by the AWS Lambda function handler.
 
         Raises
```

### Comparing `awsmate-0.3.1/src/awsmate/eventbridge.py` & `awsmate-0.4.0/src/awsmate/eventbridge.py`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.1/src/awsmate/lambdafunction.py` & `awsmate-0.4.0/src/awsmate/lambdafunction.py`

 * *Files 20% similar despite different names*

```diff
@@ -51,7 +51,26 @@
         """
         
         if not isinstance(event_object, dict):
             raise TypeError(f"event_object should be a dict. Here: {str(type(event_object))}.")
 
         self._event = event_object
 
+
+    def _records_structure(self) -> dict:
+        KEY_RECORDS = "Records"
+
+        try:
+            ret = self._event[KEY_RECORDS][0]
+
+        except KeyError as err:
+            LambdaEvent._raiseCannotReachError(str(err))
+        
+        except IndexError:
+            LambdaEvent._raiseEventStructureError(f"'{KEY_RECORDS}' is empty")
+
+        if len(self._event[KEY_RECORDS]) != 1:
+            LambdaEvent._raiseEventStructureError(
+                f"event contains {str(len(self._event[KEY_RECORDS]))} {KEY_RECORDS} where 1 is expected"
+            )
+        
+        return ret
```

### Comparing `awsmate-0.3.1/src/awsmate/logger.py` & `awsmate-0.4.0/src/awsmate/logger.py`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.1/src/awsmate/s3.py` & `awsmate-0.4.0/src/awsmate/s3.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 class LambdaNotificationEvent(LambdaEvent):
     """
     Mapping of the input event received by an AWS Lambda function triggered by AWS S3 Notification.
     """
 
-    def __init__(self, event_object: dict):
+    def __init__(self, event_object: dict) -> None:
         """
         Parameters
         ----------
         event_object : dict
             The parameter ``event`` received by the AWS Lambda function handler.
 
         Raises
@@ -27,34 +27,14 @@
         >>>     from awsmate.s3 import LambdaNotificationEvent
         >>>     event = LambdaNotificationEvent(raw_event)                
         """
 
         super().__init__(event_object)
 
 
-    def _records_structure(self) -> dict:
-        KEY_RECORDS = "Records"
-
-        try:
-            ret = self._event[KEY_RECORDS][0]
-
-        except KeyError as err:
-            LambdaEvent._raiseCannotReachError(str(err))
-        
-        except IndexError:
-            LambdaEvent._raiseEventStructureError(f"'{KEY_RECORDS}' is empty")
-
-        if len(self._event[KEY_RECORDS]) != 1:
-            LambdaEvent._raiseEventStructureError(
-                f"event contains {str(len(self._event[KEY_RECORDS]))} {KEY_RECORDS} where 1 is expected"
-            )
-        
-        return ret
-        
-        
     def _s3_structure(self) -> dict:
         try:
             ret = self._records_structure()["s3"]
 
         except KeyError as err:
             LambdaEvent._raiseCannotReachError(str(err))
```

### Comparing `awsmate-0.3.1/tests/unit/test_apigateway.py` & `awsmate-0.4.0/tests/unit/test_apigateway.py`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.1/tests/unit/test_eventbridge.py` & `awsmate-0.4.0/tests/unit/test_eventbridge.py`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.1/tests/unit/test_s3.py` & `awsmate-0.4.0/tests/unit/test_s3.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,71 +11,14 @@
     event = {}
 
     test = s3.LambdaNotificationEvent(event)
 
     assert test._event is event
 
 
-def LambdaNotificationEvent__records_structure_returnsTheProperStructure():
-    event = {
-        "Records": [
-            {
-                "anything": {}
-            }
-        ]
-    }    
-
-    test = s3.LambdaNotificationEvent(event)
-
-    assert test._records_structure() == event['Records']
-
-
-def LambdaNotificationEvent__records_structure_raisesIfEventHasNoRecordKey():
-    event = {}    
-
-    test = s3.LambdaNotificationEvent(event)
-
-    with pytest.raises(AwsEventSpecificationError) as exceptionInfo:
-        with patch.object(s3.LambdaEvent, '_raiseCannotReachError', side_effect=s3.LambdaEvent._raiseCannotReachError) as mcre:
-            test._records_structure()
-
-    mcre.assert_called_once_with("'Records'")
-
-
-def test_LambdaNotificationEvent__records_structure_raisesIfRecordsIsEmpty():
-    event = {
-        "Records": []
-    }
-
-    test = s3.LambdaNotificationEvent(event)
-
-    with pytest.raises(AwsEventSpecificationError) as exceptionInfo:
-        with patch.object(s3.LambdaEvent, '_raiseEventStructureError', side_effect=s3.LambdaEvent._raiseEventStructureError) as mcre:
-            test._records_structure()
-
-    mcre.assert_called_once_with("'Records' is empty")     
-
-
-def test_LambdaNotificationEvent_records_structure_raisesIfRecordsContainsMoreThanOneElement():
-    event = {
-        "Records": [
-            {},
-            {}
-        ]
-    }
-
-    test = s3.LambdaNotificationEvent(event)
-
-    with pytest.raises(AwsEventSpecificationError) as exceptionInfo:
-        with patch.object(s3.LambdaEvent, '_raiseEventStructureError', side_effect=s3.LambdaEvent._raiseEventStructureError) as mcre:
-            test._records_structure()
-
-    mcre.assert_called_once_with("event contains 2 Records where 1 is expected")       
-
-
 def test_LambdaNotificationEvent__s3_structure_returnsTheProperStructure():
     event = {
         "Records": [
             {
                 "s3": {
                     "anything": {}
                 }
@@ -84,15 +27,15 @@
     }
 
     test = s3.LambdaNotificationEvent(event)
 
     assert test._s3_structure() == test._records_structure()['s3']
     
     
-def LambdaNotificationEvent__s3_structure_raisesIfEventHasNoS3UnderRecords():
+def test_LambdaNotificationEvent__s3_structure_raisesIfEventHasNoS3UnderRecords():
     event = {
         "Records": [
             {}
         ]
     }    
 
     test = s3.LambdaNotificationEvent(event)
```

### Comparing `awsmate-0.3.1/LICENSE.txt` & `awsmate-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.1/README.md` & `awsmate-0.4.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -48,77 +48,120 @@
 000002f0: 2064 6576 656c 6f70 6d65 6e74 7320 696e   developments in
 00000300: 2050 7974 686f 6e2e 0a49 7420 7072 6f76   Python..It prov
 00000310: 6964 6573 2079 6f75 2077 6974 6820 6865  ides you with he
 00000320: 6c70 6572 2063 6f64 6520 7468 6174 2066  lper code that f
 00000330: 6163 696c 6974 6174 6573 2074 6865 2075  acilitates the u
 00000340: 7365 206f 6620 7661 7269 6f75 7320 4157  se of various AW
 00000350: 5320 7365 7276 6963 6573 2e0a 0a23 2320  S services...## 
-00000360: 496e 7374 616c 6c61 7469 6f6e 0a0a 2a20  Installation..* 
-00000370: 436f 6d6d 616e 6420 6c69 6e65 3a20 6070  Command line: `p
-00000380: 6970 3320 696e 7374 616c 6c20 6177 736d  ip3 install awsm
-00000390: 6174 6560 0a2a 205b 5079 5049 2070 6167  ate`.* [PyPI pag
-000003a0: 655d 2868 7474 7073 3a2f 2f70 7970 692e  e](https://pypi.
-000003b0: 6f72 672f 7072 6f6a 6563 742f 6177 736d  org/project/awsm
-000003c0: 6174 652f 2022 5079 5049 2070 6167 6522  ate/ "PyPI page"
-000003d0: 290a 0a23 2320 446f 6375 6d65 6e74 6174  )..## Documentat
-000003e0: 696f 6e0a 0a54 6865 2063 6f6d 706c 6574  ion..The complet
-000003f0: 6520 646f 6375 6d65 6e74 6174 696f 6e20  e documentation 
-00000400: 6973 2061 7661 696c 6162 6c65 2061 7420  is available at 
-00000410: 5b52 6561 6454 6865 446f 6373 5d28 6874  [ReadTheDocs](ht
-00000420: 7470 733a 2f2f 6177 736d 6174 652e 7265  tps://awsmate.re
-00000430: 6164 7468 6564 6f63 732e 696f 2f20 2244  adthedocs.io/ "D
-00000440: 6f63 756d 656e 7461 7469 6f6e 202d 2052  ocumentation - R
-00000450: 6561 6454 6865 446f 6373 2e69 6f22 292e  eadTheDocs.io").
-00000460: 0a0a 2323 2045 7861 6d70 6c65 2061 7070  ..## Example app
-00000470: 6c69 6361 7469 6f6e 0a0a 416e 2065 7861  lication..An exa
-00000480: 6d70 6c65 2061 7070 6c69 6361 7469 6f6e  mple application
-00000490: 2069 7320 6176 6169 6c61 626c 6520 746f   is available to
-000004a0: 2064 656d 6f6e 7374 7261 7465 2074 6865   demonstrate the
-000004b0: 206d 6169 6e20 6665 6174 7572 6573 206f   main features o
-000004c0: 6620 7468 6973 206c 6962 7261 7279 2e20  f this library. 
-000004d0: 4974 2069 7320 646f 6375 6d65 6e74 6564  It is documented
-000004e0: 205b 696e 2074 6869 7320 6368 6170 7465   [in this chapte
-000004f0: 725d 2868 7474 7073 3a2f 2f61 7773 6d61  r](https://awsma
-00000500: 7465 2e72 6561 6474 6865 646f 6373 2e69  te.readthedocs.i
-00000510: 6f2f 656e 2f6c 6174 6573 742f 6578 616d  o/en/latest/exam
-00000520: 706c 655f 6170 706c 6963 6174 696f 6e2e  ple_application.
-00000530: 6874 6d6c 292e 0a0a 2323 2049 7373 7565  html)...## Issue
-00000540: 730a 0a53 686f 756c 6420 796f 7520 656e  s..Should you en
-00000550: 636f 756e 7465 7220 616e 7920 6275 6720  counter any bug 
-00000560: 6f72 2070 726f 626c 656d 206f 6620 616e  or problem of an
-00000570: 7920 6b69 6e64 2c20 706c 6561 7365 2066  y kind, please f
-00000580: 6565 6c20 6672 6565 2074 6f20 6f70 656e  eel free to open
-00000590: 2061 6e20 6973 7375 6520 6163 636f 7264   an issue accord
-000005a0: 696e 6720 746f 206f 7572 205b 636f 6e74  ing to our [cont
-000005b0: 7269 6275 7469 6f6e 2067 7569 6465 6c69  ribution guideli
-000005c0: 6e65 735d 2868 7474 7073 3a2f 2f61 7773  nes](https://aws
-000005d0: 6d61 7465 2e72 6561 6474 6865 646f 6373  mate.readthedocs
-000005e0: 2e69 6f2f 656e 2f6c 6174 6573 742f 636f  .io/en/latest/co
-000005f0: 6e74 7269 6275 7469 6e67 2e68 746d 6c29  ntributing.html)
-00000600: 2e0a 0a23 2320 4c69 6365 6e73 650a 0a54  ...## License..T
-00000610: 6869 7320 7072 6f6a 6563 7420 6973 206c  his project is l
-00000620: 6963 656e 7365 6420 756e 6465 7220 7468  icensed under th
-00000630: 6520 4555 524f 5045 414e 2055 4e49 4f4e  e EUROPEAN UNION
-00000640: 2050 5542 4c49 4320 4c49 4345 4e43 4520   PUBLIC LICENCE 
-00000650: 2845 5550 4c29 2076 2e20 312e 322c 2077  (EUPL) v. 1.2, w
-00000660: 6869 6368 2069 7320 636f 6d70 6174 6962  hich is compatib
-00000670: 6c65 2077 6974 6820 7468 6520 6d61 6a6f  le with the majo
-00000680: 7269 7479 206f 6620 6f70 656e 2073 6f75  rity of open sou
-00000690: 7263 6520 6c69 6365 6e63 6573 2e0a 0a2a  rce licences...*
-000006a0: 205b 5669 6577 2061 6c6c 2074 7261 6e73   [View all trans
-000006b0: 6c61 7469 6f6e 735d 2868 7474 7073 3a2f  lations](https:/
-000006c0: 2f6a 6f69 6e75 702e 6563 2e65 7572 6f70  /joinup.ec.europ
-000006d0: 612e 6575 2f63 6f6c 6c65 6374 696f 6e2f  a.eu/collection/
-000006e0: 6575 706c 2f65 7570 6c2d 7465 7874 2d65  eupl/eupl-text-e
-000006f0: 7570 6c2d 3132 2022 5472 616e 736c 6174  upl-12 "Translat
-00000700: 696f 6e73 206f 6620 7468 6520 4555 504c  ions of the EUPL
-00000710: 2d31 2e32 2229 0a2a 205b 4f53 4920 436f  -1.2").* [OSI Co
-00000720: 6d70 6174 6962 696c 6974 7920 6d61 7472  mpatibility matr
-00000730: 6978 5d28 6874 7470 733a 2f2f 6a6f 696e  ix](https://join
-00000740: 7570 2e65 632e 6575 726f 7061 2e65 752f  up.ec.europa.eu/
-00000750: 636f 6c6c 6563 7469 6f6e 2f65 7570 6c2f  collection/eupl/
-00000760: 6d61 7472 6978 2d65 7570 6c2d 636f 6d70  matrix-eupl-comp
-00000770: 6174 6962 6c65 2d6f 7065 6e2d 736f 7572  atible-open-sour
-00000780: 6365 2d6c 6963 656e 6365 7320 2243 6f6d  ce-licences "Com
-00000790: 7061 7469 6269 6c69 7479 206d 6174 7269  patibility matri
-000007a0: 7820 6f66 2074 6865 2045 5550 4c2d 312e  x of the EUPL-1.
-000007b0: 3222 290a                                2").
+00000360: 5768 6174 2069 7420 6973 2c20 7768 6174  What it is, what
+00000370: 2069 7420 646f 6573 0a0a 6061 7773 6d61   it does..`awsma
+00000380: 7465 6020 706f 6f6c 7320 4157 5320 7370  te` pools AWS sp
+00000390: 6563 6966 6963 2063 6f64 6520 7468 6174  ecific code that
+000003a0: 2069 7320 7265 7772 6974 656e 2061 6e64   is rewriten and
+000003b0: 2072 6574 6573 7465 6420 666f 7220 6561   retested for ea
+000003c0: 6368 206e 6577 2070 726f 6a65 6374 3a0a  ch new project:.
+000003d0: 2a20 6974 2073 696d 706c 6966 6965 7320  * it simplifies 
+000003e0: 7468 6520 7573 6520 6f66 2073 6f6d 6520  the use of some 
+000003f0: 4157 5320 7365 7276 6963 6573 0a2a 2069  AWS services.* i
+00000400: 7420 7369 6d70 6c69 6669 6573 2074 6865  t simplifies the
+00000410: 2065 7272 6f72 2068 616e 646c 696e 6720   error handling 
+00000420: 7265 6c61 7465 6420 746f 2074 6865 2075  related to the u
+00000430: 7365 206f 6620 7468 6573 6520 7365 7276  se of these serv
+00000440: 6963 6573 0a0a 6061 7773 6d61 7465 6020  ices..`awsmate` 
+00000450: 646f 6573 206e 6f74 2064 6f20 7768 6174  does not do what
+00000460: 206f 7468 6572 7320 6861 7665 2061 6c72   others have alr
+00000470: 6561 6479 2064 6f6e 6520 616e 6420 7374  eady done and st
+00000480: 6963 6b73 2074 6f20 7369 6d70 6c69 6679  icks to simplify
+00000490: 696e 6720 7468 6520 7573 6520 6f66 2041  ing the use of A
+000004a0: 5753 3a0a 2a20 6974 2064 6f65 7320 6e6f  WS:.* it does no
+000004b0: 7420 7265 706c 6163 6520 6578 6973 7469  t replace existi
+000004c0: 6e67 206d 616a 6f72 206c 6962 7261 7269  ng major librari
+000004d0: 6573 2073 7563 6820 6173 205b 7333 6673  es such as [s3fs
+000004e0: 5d28 6874 7470 733a 2f2f 7333 6673 2e72  ](https://s3fs.r
+000004f0: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
+00000500: 2f6c 6174 6573 742f 292c 205b 7079 6e61  /latest/), [pyna
+00000510: 6d6f 6462 5d28 6874 7470 733a 2f2f 7079  modb](https://py
+00000520: 6e61 6d6f 6462 2e72 6561 6474 6865 646f  namodb.readthedo
+00000530: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
+00000540: 292c 205b 6177 732d 6c61 6d62 6461 2d70  ), [aws-lambda-p
+00000550: 6f77 6572 746f 6f6c 735d 2868 7474 7073  owertools](https
+00000560: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
+00000570: 6563 742f 6177 732d 6c61 6d62 6461 2d70  ect/aws-lambda-p
+00000580: 6f77 6572 746f 6f6c 732f 2920 6f72 205b  owertools/) or [
+00000590: 626f 746f 335d 2868 7474 7073 3a2f 2f62  boto3](https://b
+000005a0: 6f74 6f33 2e61 6d61 7a6f 6e61 7773 2e63  oto3.amazonaws.c
+000005b0: 6f6d 2f76 312f 646f 6375 6d65 6e74 6174  om/v1/documentat
+000005c0: 696f 6e2f 6170 692f 6c61 7465 7374 2f69  ion/api/latest/i
+000005d0: 6e64 6578 2e68 746d 6c29 0a2a 2069 7420  ndex.html).* it 
+000005e0: 646f 6573 206e 6f74 2069 6d70 6c65 6d65  does not impleme
+000005f0: 6e74 2066 756e 6374 696f 6e61 6c20 7573  nt functional us
+00000600: 6520 6361 7365 7320 6f72 2061 6c67 6f72  e cases or algor
+00000610: 6974 686d 730a 0a23 2320 496e 7374 616c  ithms..## Instal
+00000620: 6c61 7469 6f6e 0a0a 2a20 436f 6d6d 616e  lation..* Comman
+00000630: 6420 6c69 6e65 3a20 6070 6970 3320 696e  d line: `pip3 in
+00000640: 7374 616c 6c20 6177 736d 6174 6560 0a2a  stall awsmate`.*
+00000650: 205b 5079 5049 2070 6167 655d 2868 7474   [PyPI page](htt
+00000660: 7073 3a2f 2f70 7970 692e 6f72 672f 7072  ps://pypi.org/pr
+00000670: 6f6a 6563 742f 6177 736d 6174 652f 2022  oject/awsmate/ "
+00000680: 5079 5049 2070 6167 6522 290a 0a23 2320  PyPI page")..## 
+00000690: 446f 6375 6d65 6e74 6174 696f 6e0a 0a54  Documentation..T
+000006a0: 6865 2063 6f6d 706c 6574 6520 646f 6375  he complete docu
+000006b0: 6d65 6e74 6174 696f 6e20 6973 2061 7661  mentation is ava
+000006c0: 696c 6162 6c65 2061 7420 5b52 6561 6454  ilable at [ReadT
+000006d0: 6865 446f 6373 5d28 6874 7470 733a 2f2f  heDocs](https://
+000006e0: 6177 736d 6174 652e 7265 6164 7468 6564  awsmate.readthed
+000006f0: 6f63 732e 696f 2f20 2244 6f63 756d 656e  ocs.io/ "Documen
+00000700: 7461 7469 6f6e 202d 2052 6561 6454 6865  tation - ReadThe
+00000710: 446f 6373 2e69 6f22 292e 0a0a 2323 2045  Docs.io")...## E
+00000720: 7861 6d70 6c65 2061 7070 6c69 6361 7469  xample applicati
+00000730: 6f6e 0a0a 416e 2065 7861 6d70 6c65 2061  on..An example a
+00000740: 7070 6c69 6361 7469 6f6e 2069 7320 6176  pplication is av
+00000750: 6169 6c61 626c 6520 746f 2064 656d 6f6e  ailable to demon
+00000760: 7374 7261 7465 2074 6865 206d 6169 6e20  strate the main 
+00000770: 6665 6174 7572 6573 206f 6620 7468 6973  features of this
+00000780: 206c 6962 7261 7279 2e20 4974 2069 7320   library. It is 
+00000790: 646f 6375 6d65 6e74 6564 205b 696e 2074  documented [in t
+000007a0: 6869 7320 6368 6170 7465 725d 2868 7474  his chapter](htt
+000007b0: 7073 3a2f 2f61 7773 6d61 7465 2e72 6561  ps://awsmate.rea
+000007c0: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
+000007d0: 6174 6573 742f 6578 616d 706c 655f 6170  atest/example_ap
+000007e0: 706c 6963 6174 696f 6e2e 6874 6d6c 292e  plication.html).
+000007f0: 0a0a 2323 2049 7373 7565 730a 0a53 686f  ..## Issues..Sho
+00000800: 756c 6420 796f 7520 656e 636f 756e 7465  uld you encounte
+00000810: 7220 616e 7920 6275 6720 6f72 2070 726f  r any bug or pro
+00000820: 626c 656d 206f 6620 616e 7920 6b69 6e64  blem of any kind
+00000830: 2c20 706c 6561 7365 2066 6565 6c20 6672  , please feel fr
+00000840: 6565 2074 6f20 6f70 656e 2061 6e20 6973  ee to open an is
+00000850: 7375 6520 6163 636f 7264 696e 6720 746f  sue according to
+00000860: 206f 7572 205b 636f 6e74 7269 6275 7469   our [contributi
+00000870: 6f6e 2067 7569 6465 6c69 6e65 735d 2868  on guidelines](h
+00000880: 7474 7073 3a2f 2f61 7773 6d61 7465 2e72  ttps://awsmate.r
+00000890: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
+000008a0: 2f6c 6174 6573 742f 636f 6e74 7269 6275  /latest/contribu
+000008b0: 7469 6e67 2e68 746d 6c29 2e0a 0a23 2320  ting.html)...## 
+000008c0: 4c69 6365 6e73 650a 0a54 6869 7320 7072  License..This pr
+000008d0: 6f6a 6563 7420 6973 206c 6963 656e 7365  oject is license
+000008e0: 6420 756e 6465 7220 7468 6520 4555 524f  d under the EURO
+000008f0: 5045 414e 2055 4e49 4f4e 2050 5542 4c49  PEAN UNION PUBLI
+00000900: 4320 4c49 4345 4e43 4520 2845 5550 4c29  C LICENCE (EUPL)
+00000910: 2076 2e20 312e 322c 2077 6869 6368 2069   v. 1.2, which i
+00000920: 7320 636f 6d70 6174 6962 6c65 2077 6974  s compatible wit
+00000930: 6820 7468 6520 6d61 6a6f 7269 7479 206f  h the majority o
+00000940: 6620 6f70 656e 2073 6f75 7263 6520 6c69  f open source li
+00000950: 6365 6e63 6573 2e0a 0a2a 205b 5669 6577  cences...* [View
+00000960: 2061 6c6c 2074 7261 6e73 6c61 7469 6f6e   all translation
+00000970: 735d 2868 7474 7073 3a2f 2f6a 6f69 6e75  s](https://joinu
+00000980: 702e 6563 2e65 7572 6f70 612e 6575 2f63  p.ec.europa.eu/c
+00000990: 6f6c 6c65 6374 696f 6e2f 6575 706c 2f65  ollection/eupl/e
+000009a0: 7570 6c2d 7465 7874 2d65 7570 6c2d 3132  upl-text-eupl-12
+000009b0: 2022 5472 616e 736c 6174 696f 6e73 206f   "Translations o
+000009c0: 6620 7468 6520 4555 504c 2d31 2e32 2229  f the EUPL-1.2")
+000009d0: 0a2a 205b 4f53 4920 436f 6d70 6174 6962  .* [OSI Compatib
+000009e0: 696c 6974 7920 6d61 7472 6978 5d28 6874  ility matrix](ht
+000009f0: 7470 733a 2f2f 6a6f 696e 7570 2e65 632e  tps://joinup.ec.
+00000a00: 6575 726f 7061 2e65 752f 636f 6c6c 6563  europa.eu/collec
+00000a10: 7469 6f6e 2f65 7570 6c2f 6d61 7472 6978  tion/eupl/matrix
+00000a20: 2d65 7570 6c2d 636f 6d70 6174 6962 6c65  -eupl-compatible
+00000a30: 2d6f 7065 6e2d 736f 7572 6365 2d6c 6963  -open-source-lic
+00000a40: 656e 6365 7320 2243 6f6d 7061 7469 6269  ences "Compatibi
+00000a50: 6c69 7479 206d 6174 7269 7820 6f66 2074  lity matrix of t
+00000a60: 6865 2045 5550 4c2d 312e 3222 290a       he EUPL-1.2").
```

### Comparing `awsmate-0.3.1/pyproject.toml` & `awsmate-0.4.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build" 
 
 [project]
 name = "awsmate"
-version = "0.3.1"
+version = "0.4.0"
 authors = [
     { name="Vincent Poulain (Shlublu)", email="shlublu@yahoo.fr" },
 ]
 description = "A companion for your AWS Python developments."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Intended Audience :: Developers",
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)"
```

### Comparing `awsmate-0.3.1/PKG-INFO` & `awsmate-0.4.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: awsmate
-Version: 0.3.1
+Version: 0.4.0
 Summary: A companion for your AWS Python developments.
 Project-URL: Repository, https://github.com/shlublu/awsmate
 Project-URL: Documentation, https://awsmate.readthedocs.io/
 Project-URL: Bug Tracker, https://github.com/shlublu/awsmate/issues
 Project-URL: Changelog, https://github.com/shlublu/awsmate/blob/master/CHANGELOG.md
 Author-email: "Vincent Poulain (Shlublu)" <shlublu@yahoo.fr>
 License-File: LICENSE.txt
 Keywords: aws,aws-apigateway,aws-eventbridge,aws-lambda,aws-s3,python
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -28,14 +28,24 @@
 [![Tests](https://github.com/shlublu/awsmate/actions/workflows/tests.yaml/badge.svg?branch=master)](https://github.com/shlublu/awsmate/actions "Workflows - Github")
 [![Documentation](https://readthedocs.org/projects/awsmate/badge/?version=latest)](https://awsmate.readthedocs.io/ "Documentation - ReadTheDocs.io")
 
 
 `awsmate` is a companion for your AWS developments in Python.
 It provides you with helper code that facilitates the use of various AWS services.
 
+## What it is, what it does
+
+`awsmate` pools AWS specific code that is rewriten and retested for each new project:
+* it simplifies the use of some AWS services
+* it simplifies the error handling related to the use of these services
+
+`awsmate` does not do what others have already done and sticks to simplifying the use of AWS:
+* it does not replace existing major libraries such as [s3fs](https://s3fs.readthedocs.io/en/latest/), [pynamodb](https://pynamodb.readthedocs.io/en/latest/), [aws-lambda-powertools](https://pypi.org/project/aws-lambda-powertools/) or [boto3](https://boto3.amazonaws.com/v1/documentation/api/latest/index.html)
+* it does not implement functional use cases or algorithms
+
 ## Installation
 
 * Command line: `pip3 install awsmate`
 * [PyPI page](https://pypi.org/project/awsmate/ "PyPI page")
 
 ## Documentation
```

