# Comparing `tmp/sageworks-0.1.5.1.tar.gz` & `tmp/sageworks-0.1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sageworks-0.1.5.1.tar", last modified: Sun May 14 18:57:19 2023, max compression
+gzip compressed data, was "sageworks-0.1.5.2.tar", last modified: Mon May 15 23:21:53 2023, max compression
```

## Comparing `sageworks-0.1.5.1.tar` & `sageworks-0.1.5.2.tar`

### file list

```diff
@@ -1,270 +1,273 @@
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.902579 sageworks-0.1.5.1/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.853512 sageworks-0.1.5.1/.github/
--rw-r--r--   0 briford    (501) staff       (20)      499 2023-04-03 17:04:32.000000 sageworks-0.1.5.1/.github/dependabot.yml
--rw-r--r--   0 briford    (501) staff       (20)     1899 2023-03-25 19:33:37.000000 sageworks-0.1.5.1/.gitignore
--rw-r--r--   0 briford    (501) staff       (20)      281 2023-03-28 23:51:00.000000 sageworks-0.1.5.1/CONTRIBUTING.md
--rw-r--r--   0 briford    (501) staff       (20)     1080 2023-02-17 22:10:33.000000 sageworks-0.1.5.1/LICENSE
--rw-r--r--   0 briford    (501) staff       (20)     1426 2023-04-30 02:31:13.000000 sageworks-0.1.5.1/Makefile
--rw-r--r--   0 briford    (501) staff       (20)     5964 2023-05-14 18:57:19.902666 sageworks-0.1.5.1/PKG-INFO
--rw-r--r--   0 briford    (501) staff       (20)     5231 2023-05-06 21:24:25.000000 sageworks-0.1.5.1/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)      463 2023-04-03 17:04:32.000000 sageworks-0.1.5.1/SECURITY.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.847615 sageworks-0.1.5.1/applications/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.853692 sageworks-0.1.5.1/applications/aws_dashboard/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.854181 sageworks-0.1.5.1/applications/aws_dashboard/assets/
--rw-r--r--   0 briford    (501) staff       (20)    12244 2023-04-30 02:31:13.000000 sageworks-0.1.5.1/applications/aws_dashboard/assets/custom.css
--rw-r--r--   0 briford    (501) staff       (20)      318 2023-03-21 14:30:06.000000 sageworks-0.1.5.1/applications/aws_dashboard/assets/favicon.ico
--rw-r--r--   0 briford    (501) staff       (20)     1081 2023-05-14 18:49:45.000000 sageworks-0.1.5.1/applications/aws_dashboard/aws_dashboard.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.855502 sageworks-0.1.5.1/applications/aws_dashboard/pages/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.856599 sageworks-0.1.5.1/applications/aws_dashboard/pages/callbacks/
--rw-r--r--   0 briford    (501) staff       (20)     4713 2023-05-14 18:51:03.000000 sageworks-0.1.5.1/applications/aws_dashboard/pages/callbacks/data_sources_callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)      928 2023-05-10 17:06:02.000000 sageworks-0.1.5.1/applications/aws_dashboard/pages/callbacks/endpoints_callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)      975 2023-05-10 17:06:02.000000 sageworks-0.1.5.1/applications/aws_dashboard/pages/callbacks/feature_sets_callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     1777 2023-05-14 18:41:54.000000 sageworks-0.1.5.1/applications/aws_dashboard/pages/callbacks/main_callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     4757 2023-05-10 17:06:02.000000 sageworks-0.1.5.1/applications/aws_dashboard/pages/callbacks/models_callbacks.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.857085 sageworks-0.1.5.1/applications/aws_dashboard/pages/data/
--rw-r--r--   0 briford    (501) staff       (20)     1867 2023-04-08 01:44:28.000000 sageworks-0.1.5.1/applications/aws_dashboard/pages/data/toy_data.csv
--rw-r--r--   0 briford    (501) staff       (20)      597 2023-04-05 23:27:13.000000 sageworks-0.1.5.1/applications/aws_dashboard/pages/data/toy_scores.json
--rw-r--r--   0 briford    (501) staff       (20)     2518 2023-05-14 18:45:34.000000 sageworks-0.1.5.1/applications/aws_dashboard/pages/data_sources.py
--rw-r--r--   0 briford    (501) staff       (20)     1425 2023-05-10 17:06:02.000000 sageworks-0.1.5.1/applications/aws_dashboard/pages/endpoints.py
--rw-r--r--   0 briford    (501) staff       (20)     1526 2023-05-10 17:06:02.000000 sageworks-0.1.5.1/applications/aws_dashboard/pages/feature_sets.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.858483 sageworks-0.1.5.1/applications/aws_dashboard/pages/layout/
--rw-r--r--   0 briford    (501) staff       (20)     2847 2023-05-14 18:51:03.000000 sageworks-0.1.5.1/applications/aws_dashboard/pages/layout/data_sources_layout.py
--rw-r--r--   0 briford    (501) staff       (20)     1143 2023-04-09 22:27:31.000000 sageworks-0.1.5.1/applications/aws_dashboard/pages/layout/endpoints_layout.py
--rw-r--r--   0 briford    (501) staff       (20)     1286 2023-04-09 21:27:30.000000 sageworks-0.1.5.1/applications/aws_dashboard/pages/layout/feature_sets_layout.py
--rw-r--r--   0 briford    (501) staff       (20)     1584 2023-04-07 15:53:06.000000 sageworks-0.1.5.1/applications/aws_dashboard/pages/layout/main_layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2436 2023-05-09 15:15:28.000000 sageworks-0.1.5.1/applications/aws_dashboard/pages/layout/models_layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2115 2023-05-11 20:29:48.000000 sageworks-0.1.5.1/applications/aws_dashboard/pages/main.py
--rw-r--r--   0 briford    (501) staff       (20)     2547 2023-05-10 17:06:02.000000 sageworks-0.1.5.1/applications/aws_dashboard/pages/models.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.859183 sageworks-0.1.5.1/applications/hello_world/
--rw-r--r--   0 briford    (501) staff       (20)     3870 2023-04-02 18:05:33.000000 sageworks-0.1.5.1/applications/hello_world/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2152 2023-05-10 22:36:25.000000 sageworks-0.1.5.1/applications/hello_world/hello_world.py
--rw-r--r--   0 briford    (501) staff       (20)     1060 2023-04-02 18:05:33.000000 sageworks-0.1.5.1/applications/hello_world/layout.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.859937 sageworks-0.1.5.1/applications/model_viewer/
--rw-r--r--   0 briford    (501) staff       (20)     3870 2023-04-02 18:05:33.000000 sageworks-0.1.5.1/applications/model_viewer/callbacks.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.860376 sageworks-0.1.5.1/applications/model_viewer/data/
--rw-r--r--   0 briford    (501) staff       (20)     1849 2023-03-12 02:23:08.000000 sageworks-0.1.5.1/applications/model_viewer/data/toy_data.csv
--rw-r--r--   0 briford    (501) staff       (20)      597 2023-03-12 02:23:08.000000 sageworks-0.1.5.1/applications/model_viewer/data/toy_scores.json
--rw-r--r--   0 briford    (501) staff       (20)     3069 2023-04-02 18:05:33.000000 sageworks-0.1.5.1/applications/model_viewer/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2525 2023-05-09 15:17:31.000000 sageworks-0.1.5.1/applications/model_viewer/model_viewer.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.861192 sageworks-0.1.5.1/applications/web_admin/
--rw-r--r--   0 briford    (501) staff       (20)      213 2023-04-02 18:05:33.000000 sageworks-0.1.5.1/applications/web_admin/flask_test.py
--rw-r--r--   0 briford    (501) staff       (20)      201 2023-03-03 22:18:34.000000 sageworks-0.1.5.1/applications/web_admin/hello-world-http-test.ini
--rw-r--r--   0 briford    (501) staff       (20)      235 2023-03-03 22:19:17.000000 sageworks-0.1.5.1/applications/web_admin/hello-world.ini
--rw-r--r--   0 briford    (501) staff       (20)      399 2023-03-03 22:20:51.000000 sageworks-0.1.5.1/applications/web_admin/hello-world.service
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.861425 sageworks-0.1.5.1/applications/web_admin/nginx_conf/
--rw-r--r--   0 briford    (501) staff       (20)      486 2023-03-03 22:17:39.000000 sageworks-0.1.5.1/applications/web_admin/nginx_conf/nginx.conf
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.861846 sageworks-0.1.5.1/aws_setup/
--rw-r--r--   0 briford    (501) staff       (20)     3315 2023-05-05 02:30:09.000000 sageworks-0.1.5.1/aws_setup/aws_account_check.py
--rw-r--r--   0 briford    (501) staff       (20)     4013 2023-05-05 02:30:09.000000 sageworks-0.1.5.1/aws_setup/build_ml_pipeline.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.863329 sageworks-0.1.5.1/aws_setup/sageworks_cdk/
--rw-r--r--   0 briford    (501) staff       (20)      119 2023-04-20 17:45:20.000000 sageworks-0.1.5.1/aws_setup/sageworks_cdk/.gitignore
--rw-r--r--   0 briford    (501) staff       (20)     1028 2023-04-30 02:31:15.000000 sageworks-0.1.5.1/aws_setup/sageworks_cdk/README.md
--rw-r--r--   0 briford    (501) staff       (20)     1291 2023-04-30 16:18:03.000000 sageworks-0.1.5.1/aws_setup/sageworks_cdk/app.py
--rw-r--r--   0 briford    (501) staff       (20)     1998 2023-04-20 17:45:20.000000 sageworks-0.1.5.1/aws_setup/sageworks_cdk/cdk.json
--rw-r--r--   0 briford    (501) staff       (20)       14 2023-04-20 17:45:20.000000 sageworks-0.1.5.1/aws_setup/sageworks_cdk/requirements-dev.txt
--rw-r--r--   0 briford    (501) staff       (20)       70 2023-04-30 17:09:37.000000 sageworks-0.1.5.1/aws_setup/sageworks_cdk/requirements.txt
--rw-r--r--   0 briford    (501) staff       (20)      437 2023-04-20 17:45:20.000000 sageworks-0.1.5.1/aws_setup/sageworks_cdk/source.bat
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.863569 sageworks-0.1.5.1/aws_setup/sageworks_cdk/stacks/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-04-20 17:45:20.000000 sageworks-0.1.5.1/aws_setup/sageworks_cdk/stacks/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     2304 2023-05-05 02:30:09.000000 sageworks-0.1.5.1/aws_setup/sageworks_cdk/stacks/sageworks_stack.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.863697 sageworks-0.1.5.1/aws_setup/sageworks_cdk/tests/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-04-20 17:45:20.000000 sageworks-0.1.5.1/aws_setup/sageworks_cdk/tests/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.863864 sageworks-0.1.5.1/aws_setup/sageworks_cdk/tests/unit/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-04-20 17:45:20.000000 sageworks-0.1.5.1/aws_setup/sageworks_cdk/tests/unit/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)      720 2023-04-30 02:31:15.000000 sageworks-0.1.5.1/aws_setup/sageworks_cdk/tests/unit/test_sageworks_sandbox_stack.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.864008 sageworks-0.1.5.1/config/
--rw-r--r--   0 briford    (501) staff       (20)      147 2023-04-30 02:43:00.000000 sageworks-0.1.5.1/config/sageworks_config.ini
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.865055 sageworks-0.1.5.1/data/
--rw-r--r--   0 briford    (501) staff       (20)   196156 2023-03-26 18:42:12.000000 sageworks-0.1.5.1/data/abalone.csv
--rw-r--r--   0 briford    (501) staff       (20)      829 2023-05-02 22:39:27.000000 sageworks-0.1.5.1/data/test_data.csv
--rw-r--r--   0 briford    (501) staff       (20)     2270 2023-04-19 19:55:29.000000 sageworks-0.1.5.1/data/test_data.json
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.865736 sageworks-0.1.5.1/docs/
--rw-r--r--   0 briford    (501) staff       (20)     1770 2023-05-09 15:36:49.000000 sageworks-0.1.5.1/docs/admin_notes.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.871221 sageworks-0.1.5.1/docs/images/
--rw-r--r--   0 briford    (501) staff       (20)   605827 2022-12-06 17:43:49.000000 sageworks-0.1.5.1/docs/images/big_spider.png
--rw-r--r--   0 briford    (501) staff       (20)    32320 2023-01-15 22:00:05.000000 sageworks-0.1.5.1/docs/images/graph_representation.png
--rw-r--r--   0 briford    (501) staff       (20)    15549 2023-03-06 20:35:02.000000 sageworks-0.1.5.1/docs/images/powered_aws_dark_blue.png
--rw-r--r--   0 briford    (501) staff       (20)    10003 2023-03-06 20:33:32.000000 sageworks-0.1.5.1/docs/images/powered_aws_transparent.png
--rw-r--r--   0 briford    (501) staff       (20)     6435 2023-03-06 20:31:13.000000 sageworks-0.1.5.1/docs/images/powered_aws_white.png
--rw-r--r--   0 briford    (501) staff       (20)    21174 2023-03-06 20:40:25.000000 sageworks-0.1.5.1/docs/images/powered_aws_with_tm_grey.png
--rw-r--r--   0 briford    (501) staff       (20)    51137 2023-01-15 21:19:16.000000 sageworks-0.1.5.1/docs/images/sageworks.png
--rw-r--r--   0 briford    (501) staff       (20)   489672 2023-03-10 19:48:12.000000 sageworks-0.1.5.1/docs/images/sageworks_concepts.png
--rw-r--r--   0 briford    (501) staff       (20)    30017 2023-01-15 21:23:57.000000 sageworks-0.1.5.1/docs/images/scp.png
--rw-r--r--   0 briford    (501) staff       (20)   139307 2023-01-12 16:00:43.000000 sageworks-0.1.5.1/docs/images/scp_labs.png
--rw-r--r--   0 briford    (501) staff       (20)   381209 2022-12-06 17:43:49.000000 sageworks-0.1.5.1/docs/images/small_spider.png
--rw-r--r--   0 briford    (501) staff       (20)      667 2023-03-15 14:00:32.000000 sageworks-0.1.5.1/docs/sageworks_classes_concepts.md
--rw-r--r--   0 briford    (501) staff       (20)     1873 2023-03-13 14:45:22.000000 sageworks-0.1.5.1/docs/scp_consulting.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.872066 sageworks-0.1.5.1/examples/
--rw-r--r--   0 briford    (501) staff       (20)     1240 2023-04-02 18:05:33.000000 sageworks-0.1.5.1/examples/data_to_data_example.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.872325 sageworks-0.1.5.1/notebooks/
--rw-r--r--   0 briford    (501) staff       (20)   236926 2023-05-06 21:30:24.000000 sageworks-0.1.5.1/notebooks/ML_Pipeline_with_SageWorks.ipynb
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.876646 sageworks-0.1.5.1/notebooks/images/
--rw-r--r--   0 briford    (501) staff       (20)   142099 2023-04-14 22:52:23.000000 sageworks-0.1.5.1/notebooks/images/athena_query_aqsol.png
--rw-r--r--   0 briford    (501) staff       (20)   191022 2023-04-14 22:50:14.000000 sageworks-0.1.5.1/notebooks/images/aws_dashboard_aqsol.png
--rw-r--r--   0 briford    (501) staff       (20)   222686 2023-04-14 23:47:56.000000 sageworks-0.1.5.1/notebooks/images/dashboard_aqsol_features.png
--rw-r--r--   0 briford    (501) staff       (20)   171441 2023-04-15 00:30:02.000000 sageworks-0.1.5.1/notebooks/images/model_screenshot.png
--rw-r--r--   0 briford    (501) staff       (20)   489672 2023-04-15 16:18:02.000000 sageworks-0.1.5.1/notebooks/images/sageworks_concepts.png
--rw-r--r--   0 briford    (501) staff       (20)   139307 2023-04-15 16:17:49.000000 sageworks-0.1.5.1/notebooks/images/scp_labs.png
--rw-r--r--   0 briford    (501) staff       (20)      211 2023-05-02 03:06:50.000000 sageworks-0.1.5.1/requirements.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.880700 sageworks-0.1.5.1/scripts/
--rw-r--r--   0 briford    (501) staff       (20)     1373 2023-04-09 21:27:30.000000 sageworks-0.1.5.1/scripts/data_source_tags.py
--rw-r--r--   0 briford    (501) staff       (20)     1717 2023-05-05 02:30:09.000000 sageworks-0.1.5.1/scripts/generate_jsonl_data.py
--rw-r--r--   0 briford    (501) staff       (20)     1306 2023-04-09 21:27:30.000000 sageworks-0.1.5.1/scripts/list_data_sources.py
--rw-r--r--   0 briford    (501) staff       (20)      527 2023-05-14 18:57:19.902952 sageworks-0.1.5.1/setup.cfg
--rw-r--r--   0 briford    (501) staff       (20)     1787 2023-05-14 18:53:19.000000 sageworks-0.1.5.1/setup.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.848594 sageworks-0.1.5.1/src/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.880872 sageworks-0.1.5.1/src/sageworks/
--rw-r--r--   0 briford    (501) staff       (20)      853 2023-04-22 21:03:48.000000 sageworks-0.1.5.1/src/sageworks/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.881646 sageworks-0.1.5.1/src/sageworks/algorithms/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.1/src/sageworks/algorithms/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.848808 sageworks-0.1.5.1/src/sageworks/algorithms/graph/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.881752 sageworks-0.1.5.1/src/sageworks/algorithms/graph/heavy/
--rw-r--r--   0 briford    (501) staff       (20)       96 2023-03-05 20:00:31.000000 sageworks-0.1.5.1/src/sageworks/algorithms/graph/heavy/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.882001 sageworks-0.1.5.1/src/sageworks/algorithms/graph/light/
--rw-r--r--   0 briford    (501) staff       (20)      122 2023-03-05 19:59:59.000000 sageworks-0.1.5.1/src/sageworks/algorithms/graph/light/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.849058 sageworks-0.1.5.1/src/sageworks/algorithms/table/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.882229 sageworks-0.1.5.1/src/sageworks/algorithms/table/heavy/
--rw-r--r--   0 briford    (501) staff       (20)      169 2023-03-05 20:04:10.000000 sageworks-0.1.5.1/src/sageworks/algorithms/table/heavy/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.883333 sageworks-0.1.5.1/src/sageworks/algorithms/table/light/
--rw-r--r--   0 briford    (501) staff       (20)       95 2023-03-05 20:05:08.000000 sageworks-0.1.5.1/src/sageworks/algorithms/table/light/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)     1751 2023-04-05 21:18:09.000000 sageworks-0.1.5.1/src/sageworks/algorithms/table/light/data_source_eda.py
--rw-r--r--   0 briford    (501) staff       (20)     9476 2023-04-09 21:27:30.000000 sageworks-0.1.5.1/src/sageworks/algorithms/table/light/feature_spider.py
--rw-r--r--   0 briford    (501) staff       (20)     4186 2023-04-09 21:27:30.000000 sageworks-0.1.5.1/src/sageworks/algorithms/table/light/row_tagger.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.883899 sageworks-0.1.5.1/src/sageworks/artifacts/
--rw-r--r--   0 briford    (501) staff       (20)      639 2023-03-05 21:06:58.000000 sageworks-0.1.5.1/src/sageworks/artifacts/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-04-01 03:28:03.000000 sageworks-0.1.5.1/src/sageworks/artifacts/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     5706 2023-05-14 17:23:33.000000 sageworks-0.1.5.1/src/sageworks/artifacts/artifact.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.884747 sageworks-0.1.5.1/src/sageworks/artifacts/data_sources/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.1/src/sageworks/artifacts/data_sources/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    15504 2023-05-14 17:23:53.000000 sageworks-0.1.5.1/src/sageworks/artifacts/data_sources/athena_source.py
--rw-r--r--   0 briford    (501) staff       (20)     3129 2023-05-14 17:27:17.000000 sageworks-0.1.5.1/src/sageworks/artifacts/data_sources/data_source.py
--rw-r--r--   0 briford    (501) staff       (20)     2891 2023-05-14 15:23:51.000000 sageworks-0.1.5.1/src/sageworks/artifacts/data_sources/data_source_abstract.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.885117 sageworks-0.1.5.1/src/sageworks/artifacts/endpoints/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.1/src/sageworks/artifacts/endpoints/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     9792 2023-05-14 17:29:06.000000 sageworks-0.1.5.1/src/sageworks/artifacts/endpoints/endpoint.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.885487 sageworks-0.1.5.1/src/sageworks/artifacts/feature_sets/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.1/src/sageworks/artifacts/feature_sets/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    13093 2023-05-14 17:29:06.000000 sageworks-0.1.5.1/src/sageworks/artifacts/feature_sets/feature_set.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.885860 sageworks-0.1.5.1/src/sageworks/artifacts/models/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.1/src/sageworks/artifacts/models/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     4419 2023-05-14 17:29:06.000000 sageworks-0.1.5.1/src/sageworks/artifacts/models/model.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.886367 sageworks-0.1.5.1/src/sageworks/aws_service_broker/
--rw-r--r--   0 briford    (501) staff       (20)     7633 2023-05-04 14:48:56.000000 sageworks-0.1.5.1/src/sageworks/aws_service_broker/aws_account_clamp.py
--rw-r--r--   0 briford    (501) staff       (20)     9590 2023-05-12 17:33:32.000000 sageworks-0.1.5.1/src/sageworks/aws_service_broker/aws_service_broker.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.887846 sageworks-0.1.5.1/src/sageworks/aws_service_broker/aws_service_connectors/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-14 19:44:44.000000 sageworks-0.1.5.1/src/sageworks/aws_service_broker/aws_service_connectors/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     2501 2023-05-11 17:16:49.000000 sageworks-0.1.5.1/src/sageworks/aws_service_broker/aws_service_connectors/connector.py
--rw-r--r--   0 briford    (501) staff       (20)     6066 2023-05-11 17:16:49.000000 sageworks-0.1.5.1/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py
--rw-r--r--   0 briford    (501) staff       (20)     3325 2023-05-11 18:41:08.000000 sageworks-0.1.5.1/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py
--rw-r--r--   0 briford    (501) staff       (20)     5772 2023-05-12 17:34:32.000000 sageworks-0.1.5.1/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py
--rw-r--r--   0 briford    (501) staff       (20)     4297 2023-05-11 18:40:16.000000 sageworks-0.1.5.1/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py
--rw-r--r--   0 briford    (501) staff       (20)     2949 2023-05-10 23:23:46.000000 sageworks-0.1.5.1/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.888448 sageworks-0.1.5.1/src/sageworks/transforms/
--rw-r--r--   0 briford    (501) staff       (20)     1432 2023-03-17 17:39:22.000000 sageworks-0.1.5.1/src/sageworks/transforms/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.1/src/sageworks/transforms/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.849778 sageworks-0.1.5.1/src/sageworks/transforms/data_loaders/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.888673 sageworks-0.1.5.1/src/sageworks/transforms/data_loaders/heavy/
--rw-r--r--   0 briford    (501) staff       (20)     7367 2023-05-05 02:30:09.000000 sageworks-0.1.5.1/src/sageworks/transforms/data_loaders/heavy/s3_heavy_to_data_source.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.889365 sageworks-0.1.5.1/src/sageworks/transforms/data_loaders/light/
--rw-r--r--   0 briford    (501) staff       (20)     2997 2023-04-14 22:16:23.000000 sageworks-0.1.5.1/src/sageworks/transforms/data_loaders/light/csv_to_data_source.py
--rw-r--r--   0 briford    (501) staff       (20)     2483 2023-04-19 22:41:04.000000 sageworks-0.1.5.1/src/sageworks/transforms/data_loaders/light/json_to_data_source.py
--rw-r--r--   0 briford    (501) staff       (20)     4155 2023-04-30 02:50:10.000000 sageworks-0.1.5.1/src/sageworks/transforms/data_loaders/light/s3_to_data_source_light.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.889576 sageworks-0.1.5.1/src/sageworks/transforms/data_to_data/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.1/src/sageworks/transforms/data_to_data/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.889663 sageworks-0.1.5.1/src/sageworks/transforms/data_to_data/heavy/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.1/src/sageworks/transforms/data_to_data/heavy/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.889751 sageworks-0.1.5.1/src/sageworks/transforms/data_to_data/heavy/emr/
--rw-r--r--   0 briford    (501) staff       (20)       68 2023-03-15 02:15:48.000000 sageworks-0.1.5.1/src/sageworks/transforms/data_to_data/heavy/emr/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.889936 sageworks-0.1.5.1/src/sageworks/transforms/data_to_data/heavy/glue/
--rw-r--r--   0 briford    (501) staff       (20)       48 2023-03-15 02:16:45.000000 sageworks-0.1.5.1/src/sageworks/transforms/data_to_data/heavy/glue/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.890458 sageworks-0.1.5.1/src/sageworks/transforms/data_to_data/light/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.1/src/sageworks/transforms/data_to_data/light/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     2231 2023-05-12 22:12:48.000000 sageworks-0.1.5.1/src/sageworks/transforms/data_to_data/light/clean_data.py
--rw-r--r--   0 briford    (501) staff       (20)     2298 2023-05-12 21:29:54.000000 sageworks-0.1.5.1/src/sageworks/transforms/data_to_data/light/data_to_data_light.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.890677 sageworks-0.1.5.1/src/sageworks/transforms/data_to_features/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.1/src/sageworks/transforms/data_to_features/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.890838 sageworks-0.1.5.1/src/sageworks/transforms/data_to_features/heavy/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.1/src/sageworks/transforms/data_to_features/heavy/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     5817 2023-05-12 17:46:07.000000 sageworks-0.1.5.1/src/sageworks/transforms/data_to_features/heavy/data_to_features_heavy.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.891046 sageworks-0.1.5.1/src/sageworks/transforms/data_to_features/heavy/emr/
--rw-r--r--   0 briford    (501) staff       (20)       68 2023-03-15 02:18:14.000000 sageworks-0.1.5.1/src/sageworks/transforms/data_to_features/heavy/emr/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.891282 sageworks-0.1.5.1/src/sageworks/transforms/data_to_features/heavy/glue/
--rw-r--r--   0 briford    (501) staff       (20)       48 2023-03-15 02:18:14.000000 sageworks-0.1.5.1/src/sageworks/transforms/data_to_features/heavy/glue/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.891824 sageworks-0.1.5.1/src/sageworks/transforms/data_to_features/light/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.1/src/sageworks/transforms/data_to_features/light/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     2538 2023-05-12 17:52:28.000000 sageworks-0.1.5.1/src/sageworks/transforms/data_to_features/light/data_to_features_light.py
--rw-r--r--   0 briford    (501) staff       (20)     2974 2023-05-12 17:46:07.000000 sageworks-0.1.5.1/src/sageworks/transforms/data_to_features/light/rdkit_descriptors.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.892070 sageworks-0.1.5.1/src/sageworks/transforms/features_to_features/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 18:06:15.000000 sageworks-0.1.5.1/src/sageworks/transforms/features_to_features/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.850562 sageworks-0.1.5.1/src/sageworks/transforms/features_to_features/heavy/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.892158 sageworks-0.1.5.1/src/sageworks/transforms/features_to_features/heavy/emr/
--rw-r--r--   0 briford    (501) staff       (20)       68 2023-03-15 02:18:46.000000 sageworks-0.1.5.1/src/sageworks/transforms/features_to_features/heavy/emr/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.892428 sageworks-0.1.5.1/src/sageworks/transforms/features_to_features/heavy/glue/
--rw-r--r--   0 briford    (501) staff       (20)       48 2023-03-15 02:18:46.000000 sageworks-0.1.5.1/src/sageworks/transforms/features_to_features/heavy/glue/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.892704 sageworks-0.1.5.1/src/sageworks/transforms/features_to_model/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.1/src/sageworks/transforms/features_to_model/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     7840 2023-05-12 17:53:53.000000 sageworks-0.1.5.1/src/sageworks/transforms/features_to_model/features_to_model.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.893192 sageworks-0.1.5.1/src/sageworks/transforms/features_to_model/light_model_harness/
--rw-r--r--   0 briford    (501) staff       (20)        8 2023-03-25 02:07:31.000000 sageworks-0.1.5.1/src/sageworks/transforms/features_to_model/light_model_harness/requirements.txt
--rw-r--r--   0 briford    (501) staff       (20)     5179 2023-04-18 16:01:35.000000 sageworks-0.1.5.1/src/sageworks/transforms/features_to_model/light_model_harness/xgb_model.template
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.893516 sageworks-0.1.5.1/src/sageworks/transforms/model_to_endpoint/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.1/src/sageworks/transforms/model_to_endpoint/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     2800 2023-05-12 17:54:23.000000 sageworks-0.1.5.1/src/sageworks/transforms/model_to_endpoint/model_to_endpoint.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.894522 sageworks-0.1.5.1/src/sageworks/transforms/pandas_transforms/
--rw-r--r--   0 briford    (501) staff       (20)     2745 2023-04-13 18:18:49.000000 sageworks-0.1.5.1/src/sageworks/transforms/pandas_transforms/data_to_pandas.py
--rw-r--r--   0 briford    (501) staff       (20)     3144 2023-04-13 18:18:49.000000 sageworks-0.1.5.1/src/sageworks/transforms/pandas_transforms/features_to_pandas.py
--rw-r--r--   0 briford    (501) staff       (20)     7003 2023-05-12 21:36:54.000000 sageworks-0.1.5.1/src/sageworks/transforms/pandas_transforms/pandas_to_data.py
--rw-r--r--   0 briford    (501) staff       (20)    10872 2023-05-12 17:52:28.000000 sageworks-0.1.5.1/src/sageworks/transforms/pandas_transforms/pandas_to_features.py
--rw-r--r--   0 briford    (501) staff       (20)     7517 2023-05-12 23:56:39.000000 sageworks-0.1.5.1/src/sageworks/transforms/pandas_transforms/pandas_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     6705 2023-05-14 17:33:24.000000 sageworks-0.1.5.1/src/sageworks/transforms/transform.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.896498 sageworks-0.1.5.1/src/sageworks/utils/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 02:34:19.000000 sageworks-0.1.5.1/src/sageworks/utils/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     3962 2023-04-30 02:31:13.000000 sageworks-0.1.5.1/src/sageworks/utils/cache.py
--rw-r--r--   0 briford    (501) staff       (20)     5113 2023-04-09 21:27:30.000000 sageworks-0.1.5.1/src/sageworks/utils/df_to_endpoint.py
--rw-r--r--   0 briford    (501) staff       (20)     2417 2023-05-14 17:23:33.000000 sageworks-0.1.5.1/src/sageworks/utils/iso_8601.py
--rw-r--r--   0 briford    (501) staff       (20)     6532 2023-05-05 02:30:09.000000 sageworks-0.1.5.1/src/sageworks/utils/redis_cache.py
--rw-r--r--   0 briford    (501) staff       (20)     3618 2023-04-17 19:53:54.000000 sageworks-0.1.5.1/src/sageworks/utils/sageworks_config.py
--rw-r--r--   0 briford    (501) staff       (20)     3558 2023-04-12 15:59:21.000000 sageworks-0.1.5.1/src/sageworks/utils/sageworks_event_bridge.py
--rw-r--r--   0 briford    (501) staff       (20)      531 2023-04-02 18:05:33.000000 sageworks-0.1.5.1/src/sageworks/utils/sageworks_logging.py
--rw-r--r--   0 briford    (501) staff       (20)     2209 2023-04-02 19:53:47.000000 sageworks-0.1.5.1/src/sageworks/utils/sageworks_sqs.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.897473 sageworks-0.1.5.1/src/sageworks/views/
--rw-r--r--   0 briford    (501) staff       (20)    11812 2023-05-12 17:36:11.000000 sageworks-0.1.5.1/src/sageworks/views/artifacts_text_view.py
--rw-r--r--   0 briford    (501) staff       (20)     3063 2023-05-12 17:33:32.000000 sageworks-0.1.5.1/src/sageworks/views/artifacts_web_view.py
--rw-r--r--   0 briford    (501) staff       (20)     4206 2023-05-14 18:51:25.000000 sageworks-0.1.5.1/src/sageworks/views/data_source_web_view.py
--rw-r--r--   0 briford    (501) staff       (20)     1296 2023-04-19 17:02:05.000000 sageworks-0.1.5.1/src/sageworks/views/view.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.900206 sageworks-0.1.5.1/src/sageworks/web_components/
--rw-r--r--   0 briford    (501) staff       (20)     1304 2023-05-05 02:30:09.000000 sageworks-0.1.5.1/src/sageworks/web_components/box_plot.py
--rw-r--r--   0 briford    (501) staff       (20)     1661 2023-04-08 01:37:21.000000 sageworks-0.1.5.1/src/sageworks/web_components/confusion_matrix.py
--rw-r--r--   0 briford    (501) staff       (20)     1015 2023-05-14 18:45:34.000000 sageworks-0.1.5.1/src/sageworks/web_components/data_source_details.py
--rw-r--r--   0 briford    (501) staff       (20)     1247 2023-04-09 21:27:30.000000 sageworks-0.1.5.1/src/sageworks/web_components/feature_details.py
--rw-r--r--   0 briford    (501) staff       (20)      815 2023-04-02 19:53:47.000000 sageworks-0.1.5.1/src/sageworks/web_components/feature_importance.py
--rw-r--r--   0 briford    (501) staff       (20)     1182 2023-04-07 23:04:10.000000 sageworks-0.1.5.1/src/sageworks/web_components/histogram.py
--rw-r--r--   0 briford    (501) staff       (20)      837 2023-04-09 21:27:30.000000 sageworks-0.1.5.1/src/sageworks/web_components/line_chart.py
--rw-r--r--   0 briford    (501) staff       (20)     1507 2023-04-09 21:30:08.000000 sageworks-0.1.5.1/src/sageworks/web_components/model_data.py
--rw-r--r--   0 briford    (501) staff       (20)     1703 2023-04-02 19:53:47.000000 sageworks-0.1.5.1/src/sageworks/web_components/model_details.py
--rw-r--r--   0 briford    (501) staff       (20)     1551 2023-04-09 21:27:30.000000 sageworks-0.1.5.1/src/sageworks/web_components/scatter_plot.py
--rw-r--r--   0 briford    (501) staff       (20)     2227 2023-05-11 20:41:25.000000 sageworks-0.1.5.1/src/sageworks/web_components/table.py
--rw-r--r--   0 briford    (501) staff       (20)     1944 2023-05-05 02:30:09.000000 sageworks-0.1.5.1/src/sageworks/web_components/violin_plot.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.881521 sageworks-0.1.5.1/src/sageworks.egg-info/
--rw-r--r--   0 briford    (501) staff       (20)     5964 2023-05-14 18:57:19.000000 sageworks-0.1.5.1/src/sageworks.egg-info/PKG-INFO
--rw-r--r--   0 briford    (501) staff       (20)     8753 2023-05-14 18:57:19.000000 sageworks-0.1.5.1/src/sageworks.egg-info/SOURCES.txt
--rw-r--r--   0 briford    (501) staff       (20)        1 2023-05-14 18:57:19.000000 sageworks-0.1.5.1/src/sageworks.egg-info/dependency_links.txt
--rw-r--r--   0 briford    (501) staff       (20)      134 2023-05-14 18:57:19.000000 sageworks-0.1.5.1/src/sageworks.egg-info/requires.txt
--rw-r--r--   0 briford    (501) staff       (20)       10 2023-05-14 18:57:19.000000 sageworks-0.1.5.1/src/sageworks.egg-info/top_level.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.900368 sageworks-0.1.5.1/tests/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.901219 sageworks-0.1.5.1/tests/artifacts/
--rw-r--r--   0 briford    (501) staff       (20)     1250 2023-05-14 17:27:17.000000 sageworks-0.1.5.1/tests/artifacts/data_source_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     1483 2023-04-11 20:37:15.000000 sageworks-0.1.5.1/tests/artifacts/endpoint_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     1155 2023-05-14 17:27:17.000000 sageworks-0.1.5.1/tests/artifacts/feature_set_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      799 2023-04-02 18:05:33.000000 sageworks-0.1.5.1/tests/artifacts/model_tests.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.901644 sageworks-0.1.5.1/tests/aws_account/
--rw-r--r--   0 briford    (501) staff       (20)     1105 2023-05-05 02:37:56.000000 sageworks-0.1.5.1/tests/aws_account/aws_account_clamp_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      642 2023-05-05 02:38:20.000000 sageworks-0.1.5.1/tests/aws_account/aws_service_broker_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     3341 2023-04-19 17:23:07.000000 sageworks-0.1.5.1/tests/create_sageworks_objs_for_tests.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.902432 sageworks-0.1.5.1/tests/transforms/
--rw-r--r--   0 briford    (501) staff       (20)      554 2023-05-12 17:46:18.000000 sageworks-0.1.5.1/tests/transforms/data_to_data_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      682 2023-05-12 18:00:39.000000 sageworks-0.1.5.1/tests/transforms/data_to_features_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      655 2023-05-12 18:01:20.000000 sageworks-0.1.5.1/tests/transforms/features_to_model_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      642 2023-05-12 17:46:18.000000 sageworks-0.1.5.1/tests/transforms/model_to_endpoint_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      628 2023-05-12 17:46:18.000000 sageworks-0.1.5.1/tests/transforms/pandas_to_data_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      729 2023-05-05 02:35:30.000000 sageworks-0.1.5.1/tox.ini
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.679161 sageworks-0.1.5.2/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.624478 sageworks-0.1.5.2/.github/
+-rw-r--r--   0 briford    (501) staff       (20)      499 2023-04-03 17:04:32.000000 sageworks-0.1.5.2/.github/dependabot.yml
+-rw-r--r--   0 briford    (501) staff       (20)     1899 2023-03-25 19:33:37.000000 sageworks-0.1.5.2/.gitignore
+-rw-r--r--   0 briford    (501) staff       (20)      281 2023-03-28 23:51:00.000000 sageworks-0.1.5.2/CONTRIBUTING.md
+-rw-r--r--   0 briford    (501) staff       (20)     1080 2023-02-17 22:10:33.000000 sageworks-0.1.5.2/LICENSE
+-rw-r--r--   0 briford    (501) staff       (20)     1426 2023-04-30 02:31:13.000000 sageworks-0.1.5.2/Makefile
+-rw-r--r--   0 briford    (501) staff       (20)     5964 2023-05-15 23:21:53.679250 sageworks-0.1.5.2/PKG-INFO
+-rw-r--r--   0 briford    (501) staff       (20)     5231 2023-05-06 21:24:25.000000 sageworks-0.1.5.2/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)      463 2023-04-03 17:04:32.000000 sageworks-0.1.5.2/SECURITY.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.618717 sageworks-0.1.5.2/applications/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.624690 sageworks-0.1.5.2/applications/aws_dashboard/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.625161 sageworks-0.1.5.2/applications/aws_dashboard/assets/
+-rw-r--r--   0 briford    (501) staff       (20)    12412 2023-05-15 21:52:25.000000 sageworks-0.1.5.2/applications/aws_dashboard/assets/custom.css
+-rw-r--r--   0 briford    (501) staff       (20)      318 2023-03-21 14:30:06.000000 sageworks-0.1.5.2/applications/aws_dashboard/assets/favicon.ico
+-rw-r--r--   0 briford    (501) staff       (20)     1081 2023-05-15 22:35:52.000000 sageworks-0.1.5.2/applications/aws_dashboard/aws_dashboard.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.626316 sageworks-0.1.5.2/applications/aws_dashboard/pages/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.627601 sageworks-0.1.5.2/applications/aws_dashboard/pages/callbacks/
+-rw-r--r--   0 briford    (501) staff       (20)     4725 2023-05-15 22:23:21.000000 sageworks-0.1.5.2/applications/aws_dashboard/pages/callbacks/data_sources_callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)      928 2023-05-10 17:06:02.000000 sageworks-0.1.5.2/applications/aws_dashboard/pages/callbacks/endpoints_callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     4748 2023-05-15 22:23:21.000000 sageworks-0.1.5.2/applications/aws_dashboard/pages/callbacks/feature_sets_callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     1777 2023-05-14 18:41:54.000000 sageworks-0.1.5.2/applications/aws_dashboard/pages/callbacks/main_callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     4757 2023-05-10 17:06:02.000000 sageworks-0.1.5.2/applications/aws_dashboard/pages/callbacks/models_callbacks.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.628087 sageworks-0.1.5.2/applications/aws_dashboard/pages/data/
+-rw-r--r--   0 briford    (501) staff       (20)     1867 2023-04-08 01:44:28.000000 sageworks-0.1.5.2/applications/aws_dashboard/pages/data/toy_data.csv
+-rw-r--r--   0 briford    (501) staff       (20)      597 2023-04-05 23:27:13.000000 sageworks-0.1.5.2/applications/aws_dashboard/pages/data/toy_scores.json
+-rw-r--r--   0 briford    (501) staff       (20)     2545 2023-05-15 23:15:00.000000 sageworks-0.1.5.2/applications/aws_dashboard/pages/data_sources.py
+-rw-r--r--   0 briford    (501) staff       (20)     1425 2023-05-10 17:06:02.000000 sageworks-0.1.5.2/applications/aws_dashboard/pages/endpoints.py
+-rw-r--r--   0 briford    (501) staff       (20)     2576 2023-05-15 23:15:00.000000 sageworks-0.1.5.2/applications/aws_dashboard/pages/feature_sets.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.629306 sageworks-0.1.5.2/applications/aws_dashboard/pages/layout/
+-rw-r--r--   0 briford    (501) staff       (20)     2696 2023-05-15 01:07:25.000000 sageworks-0.1.5.2/applications/aws_dashboard/pages/layout/data_sources_layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     1143 2023-04-09 22:27:31.000000 sageworks-0.1.5.2/applications/aws_dashboard/pages/layout/endpoints_layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2707 2023-05-15 22:17:03.000000 sageworks-0.1.5.2/applications/aws_dashboard/pages/layout/feature_sets_layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     1584 2023-04-07 15:53:06.000000 sageworks-0.1.5.2/applications/aws_dashboard/pages/layout/main_layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2436 2023-05-09 15:15:28.000000 sageworks-0.1.5.2/applications/aws_dashboard/pages/layout/models_layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2115 2023-05-11 20:29:48.000000 sageworks-0.1.5.2/applications/aws_dashboard/pages/main.py
+-rw-r--r--   0 briford    (501) staff       (20)     2547 2023-05-10 17:06:02.000000 sageworks-0.1.5.2/applications/aws_dashboard/pages/models.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.630101 sageworks-0.1.5.2/applications/hello_world/
+-rw-r--r--   0 briford    (501) staff       (20)     3870 2023-04-02 18:05:33.000000 sageworks-0.1.5.2/applications/hello_world/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2152 2023-05-10 22:36:25.000000 sageworks-0.1.5.2/applications/hello_world/hello_world.py
+-rw-r--r--   0 briford    (501) staff       (20)     1060 2023-04-02 18:05:33.000000 sageworks-0.1.5.2/applications/hello_world/layout.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.630776 sageworks-0.1.5.2/applications/model_viewer/
+-rw-r--r--   0 briford    (501) staff       (20)     3870 2023-04-02 18:05:33.000000 sageworks-0.1.5.2/applications/model_viewer/callbacks.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.631297 sageworks-0.1.5.2/applications/model_viewer/data/
+-rw-r--r--   0 briford    (501) staff       (20)     1849 2023-03-12 02:23:08.000000 sageworks-0.1.5.2/applications/model_viewer/data/toy_data.csv
+-rw-r--r--   0 briford    (501) staff       (20)      597 2023-03-12 02:23:08.000000 sageworks-0.1.5.2/applications/model_viewer/data/toy_scores.json
+-rw-r--r--   0 briford    (501) staff       (20)     3069 2023-04-02 18:05:33.000000 sageworks-0.1.5.2/applications/model_viewer/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2525 2023-05-09 15:17:31.000000 sageworks-0.1.5.2/applications/model_viewer/model_viewer.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.632048 sageworks-0.1.5.2/applications/web_admin/
+-rw-r--r--   0 briford    (501) staff       (20)      213 2023-04-02 18:05:33.000000 sageworks-0.1.5.2/applications/web_admin/flask_test.py
+-rw-r--r--   0 briford    (501) staff       (20)      201 2023-03-03 22:18:34.000000 sageworks-0.1.5.2/applications/web_admin/hello-world-http-test.ini
+-rw-r--r--   0 briford    (501) staff       (20)      235 2023-03-03 22:19:17.000000 sageworks-0.1.5.2/applications/web_admin/hello-world.ini
+-rw-r--r--   0 briford    (501) staff       (20)      399 2023-03-03 22:20:51.000000 sageworks-0.1.5.2/applications/web_admin/hello-world.service
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.632249 sageworks-0.1.5.2/applications/web_admin/nginx_conf/
+-rw-r--r--   0 briford    (501) staff       (20)      486 2023-03-03 22:17:39.000000 sageworks-0.1.5.2/applications/web_admin/nginx_conf/nginx.conf
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.632641 sageworks-0.1.5.2/aws_setup/
+-rw-r--r--   0 briford    (501) staff       (20)     3315 2023-05-05 02:30:09.000000 sageworks-0.1.5.2/aws_setup/aws_account_check.py
+-rw-r--r--   0 briford    (501) staff       (20)     4013 2023-05-05 02:30:09.000000 sageworks-0.1.5.2/aws_setup/build_ml_pipeline.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.634264 sageworks-0.1.5.2/aws_setup/sageworks_cdk/
+-rw-r--r--   0 briford    (501) staff       (20)      119 2023-04-20 17:45:20.000000 sageworks-0.1.5.2/aws_setup/sageworks_cdk/.gitignore
+-rw-r--r--   0 briford    (501) staff       (20)     1028 2023-04-30 02:31:15.000000 sageworks-0.1.5.2/aws_setup/sageworks_cdk/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     1291 2023-04-30 16:18:03.000000 sageworks-0.1.5.2/aws_setup/sageworks_cdk/app.py
+-rw-r--r--   0 briford    (501) staff       (20)     1998 2023-04-20 17:45:20.000000 sageworks-0.1.5.2/aws_setup/sageworks_cdk/cdk.json
+-rw-r--r--   0 briford    (501) staff       (20)       14 2023-04-20 17:45:20.000000 sageworks-0.1.5.2/aws_setup/sageworks_cdk/requirements-dev.txt
+-rw-r--r--   0 briford    (501) staff       (20)       70 2023-04-30 17:09:37.000000 sageworks-0.1.5.2/aws_setup/sageworks_cdk/requirements.txt
+-rw-r--r--   0 briford    (501) staff       (20)      437 2023-04-20 17:45:20.000000 sageworks-0.1.5.2/aws_setup/sageworks_cdk/source.bat
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.634508 sageworks-0.1.5.2/aws_setup/sageworks_cdk/stacks/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-04-20 17:45:20.000000 sageworks-0.1.5.2/aws_setup/sageworks_cdk/stacks/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     2304 2023-05-05 02:30:09.000000 sageworks-0.1.5.2/aws_setup/sageworks_cdk/stacks/sageworks_stack.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.634640 sageworks-0.1.5.2/aws_setup/sageworks_cdk/tests/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-04-20 17:45:20.000000 sageworks-0.1.5.2/aws_setup/sageworks_cdk/tests/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.634801 sageworks-0.1.5.2/aws_setup/sageworks_cdk/tests/unit/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-04-20 17:45:20.000000 sageworks-0.1.5.2/aws_setup/sageworks_cdk/tests/unit/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)      720 2023-04-30 02:31:15.000000 sageworks-0.1.5.2/aws_setup/sageworks_cdk/tests/unit/test_sageworks_sandbox_stack.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.634953 sageworks-0.1.5.2/config/
+-rw-r--r--   0 briford    (501) staff       (20)      147 2023-04-30 02:43:00.000000 sageworks-0.1.5.2/config/sageworks_config.ini
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.636236 sageworks-0.1.5.2/data/
+-rw-r--r--   0 briford    (501) staff       (20)   196156 2023-03-26 18:42:12.000000 sageworks-0.1.5.2/data/abalone.csv
+-rw-r--r--   0 briford    (501) staff       (20)      829 2023-05-02 22:39:27.000000 sageworks-0.1.5.2/data/test_data.csv
+-rw-r--r--   0 briford    (501) staff       (20)     2270 2023-04-19 19:55:29.000000 sageworks-0.1.5.2/data/test_data.json
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.637115 sageworks-0.1.5.2/docs/
+-rw-r--r--   0 briford    (501) staff       (20)     1770 2023-05-09 15:36:49.000000 sageworks-0.1.5.2/docs/admin_notes.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.643240 sageworks-0.1.5.2/docs/images/
+-rw-r--r--   0 briford    (501) staff       (20)   605827 2022-12-06 17:43:49.000000 sageworks-0.1.5.2/docs/images/big_spider.png
+-rw-r--r--   0 briford    (501) staff       (20)    32320 2023-01-15 22:00:05.000000 sageworks-0.1.5.2/docs/images/graph_representation.png
+-rw-r--r--   0 briford    (501) staff       (20)    15549 2023-03-06 20:35:02.000000 sageworks-0.1.5.2/docs/images/powered_aws_dark_blue.png
+-rw-r--r--   0 briford    (501) staff       (20)    10003 2023-03-06 20:33:32.000000 sageworks-0.1.5.2/docs/images/powered_aws_transparent.png
+-rw-r--r--   0 briford    (501) staff       (20)     6435 2023-03-06 20:31:13.000000 sageworks-0.1.5.2/docs/images/powered_aws_white.png
+-rw-r--r--   0 briford    (501) staff       (20)    21174 2023-03-06 20:40:25.000000 sageworks-0.1.5.2/docs/images/powered_aws_with_tm_grey.png
+-rw-r--r--   0 briford    (501) staff       (20)    51137 2023-01-15 21:19:16.000000 sageworks-0.1.5.2/docs/images/sageworks.png
+-rw-r--r--   0 briford    (501) staff       (20)   489672 2023-03-10 19:48:12.000000 sageworks-0.1.5.2/docs/images/sageworks_concepts.png
+-rw-r--r--   0 briford    (501) staff       (20)    30017 2023-01-15 21:23:57.000000 sageworks-0.1.5.2/docs/images/scp.png
+-rw-r--r--   0 briford    (501) staff       (20)   139307 2023-01-12 16:00:43.000000 sageworks-0.1.5.2/docs/images/scp_labs.png
+-rw-r--r--   0 briford    (501) staff       (20)   381209 2022-12-06 17:43:49.000000 sageworks-0.1.5.2/docs/images/small_spider.png
+-rw-r--r--   0 briford    (501) staff       (20)      667 2023-03-15 14:00:32.000000 sageworks-0.1.5.2/docs/sageworks_classes_concepts.md
+-rw-r--r--   0 briford    (501) staff       (20)     1873 2023-03-13 14:45:22.000000 sageworks-0.1.5.2/docs/scp_consulting.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.644056 sageworks-0.1.5.2/examples/
+-rw-r--r--   0 briford    (501) staff       (20)     1240 2023-04-02 18:05:33.000000 sageworks-0.1.5.2/examples/data_to_data_example.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.644403 sageworks-0.1.5.2/notebooks/
+-rw-r--r--   0 briford    (501) staff       (20)   236926 2023-05-06 21:30:24.000000 sageworks-0.1.5.2/notebooks/ML_Pipeline_with_SageWorks.ipynb
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.649126 sageworks-0.1.5.2/notebooks/images/
+-rw-r--r--   0 briford    (501) staff       (20)   142099 2023-04-14 22:52:23.000000 sageworks-0.1.5.2/notebooks/images/athena_query_aqsol.png
+-rw-r--r--   0 briford    (501) staff       (20)   191022 2023-04-14 22:50:14.000000 sageworks-0.1.5.2/notebooks/images/aws_dashboard_aqsol.png
+-rw-r--r--   0 briford    (501) staff       (20)   222686 2023-04-14 23:47:56.000000 sageworks-0.1.5.2/notebooks/images/dashboard_aqsol_features.png
+-rw-r--r--   0 briford    (501) staff       (20)   171441 2023-04-15 00:30:02.000000 sageworks-0.1.5.2/notebooks/images/model_screenshot.png
+-rw-r--r--   0 briford    (501) staff       (20)   489672 2023-04-15 16:18:02.000000 sageworks-0.1.5.2/notebooks/images/sageworks_concepts.png
+-rw-r--r--   0 briford    (501) staff       (20)   139307 2023-04-15 16:17:49.000000 sageworks-0.1.5.2/notebooks/images/scp_labs.png
+-rw-r--r--   0 briford    (501) staff       (20)      211 2023-05-02 03:06:50.000000 sageworks-0.1.5.2/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.653194 sageworks-0.1.5.2/scripts/
+-rw-r--r--   0 briford    (501) staff       (20)     1373 2023-04-09 21:27:30.000000 sageworks-0.1.5.2/scripts/data_source_tags.py
+-rw-r--r--   0 briford    (501) staff       (20)     1717 2023-05-05 02:30:09.000000 sageworks-0.1.5.2/scripts/generate_jsonl_data.py
+-rw-r--r--   0 briford    (501) staff       (20)     1306 2023-04-09 21:27:30.000000 sageworks-0.1.5.2/scripts/list_data_sources.py
+-rw-r--r--   0 briford    (501) staff       (20)      527 2023-05-15 23:21:53.679561 sageworks-0.1.5.2/setup.cfg
+-rw-r--r--   0 briford    (501) staff       (20)     1787 2023-05-15 23:21:38.000000 sageworks-0.1.5.2/setup.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.619652 sageworks-0.1.5.2/src/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.653481 sageworks-0.1.5.2/src/sageworks/
+-rw-r--r--   0 briford    (501) staff       (20)      853 2023-04-22 21:03:48.000000 sageworks-0.1.5.2/src/sageworks/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.654302 sageworks-0.1.5.2/src/sageworks/algorithms/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.2/src/sageworks/algorithms/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.619894 sageworks-0.1.5.2/src/sageworks/algorithms/graph/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.654389 sageworks-0.1.5.2/src/sageworks/algorithms/graph/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)       96 2023-03-05 20:00:31.000000 sageworks-0.1.5.2/src/sageworks/algorithms/graph/heavy/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.654625 sageworks-0.1.5.2/src/sageworks/algorithms/graph/light/
+-rw-r--r--   0 briford    (501) staff       (20)      122 2023-03-05 19:59:59.000000 sageworks-0.1.5.2/src/sageworks/algorithms/graph/light/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.620061 sageworks-0.1.5.2/src/sageworks/algorithms/table/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.654845 sageworks-0.1.5.2/src/sageworks/algorithms/table/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)      169 2023-03-05 20:04:10.000000 sageworks-0.1.5.2/src/sageworks/algorithms/table/heavy/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.655931 sageworks-0.1.5.2/src/sageworks/algorithms/table/light/
+-rw-r--r--   0 briford    (501) staff       (20)       95 2023-03-05 20:05:08.000000 sageworks-0.1.5.2/src/sageworks/algorithms/table/light/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)     1751 2023-04-05 21:18:09.000000 sageworks-0.1.5.2/src/sageworks/algorithms/table/light/data_source_eda.py
+-rw-r--r--   0 briford    (501) staff       (20)     9476 2023-04-09 21:27:30.000000 sageworks-0.1.5.2/src/sageworks/algorithms/table/light/feature_spider.py
+-rw-r--r--   0 briford    (501) staff       (20)     4186 2023-04-09 21:27:30.000000 sageworks-0.1.5.2/src/sageworks/algorithms/table/light/row_tagger.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.656622 sageworks-0.1.5.2/src/sageworks/artifacts/
+-rw-r--r--   0 briford    (501) staff       (20)      639 2023-03-05 21:06:58.000000 sageworks-0.1.5.2/src/sageworks/artifacts/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-04-01 03:28:03.000000 sageworks-0.1.5.2/src/sageworks/artifacts/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     5706 2023-05-14 17:23:33.000000 sageworks-0.1.5.2/src/sageworks/artifacts/artifact.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.657570 sageworks-0.1.5.2/src/sageworks/artifacts/data_sources/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.2/src/sageworks/artifacts/data_sources/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    15504 2023-05-15 19:02:40.000000 sageworks-0.1.5.2/src/sageworks/artifacts/data_sources/athena_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     3129 2023-05-14 17:27:17.000000 sageworks-0.1.5.2/src/sageworks/artifacts/data_sources/data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     2891 2023-05-14 15:23:51.000000 sageworks-0.1.5.2/src/sageworks/artifacts/data_sources/data_source_abstract.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.657913 sageworks-0.1.5.2/src/sageworks/artifacts/endpoints/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.2/src/sageworks/artifacts/endpoints/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     9792 2023-05-14 17:29:06.000000 sageworks-0.1.5.2/src/sageworks/artifacts/endpoints/endpoint.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.658365 sageworks-0.1.5.2/src/sageworks/artifacts/feature_sets/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.2/src/sageworks/artifacts/feature_sets/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    13915 2023-05-15 23:16:08.000000 sageworks-0.1.5.2/src/sageworks/artifacts/feature_sets/feature_set.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.658573 sageworks-0.1.5.2/src/sageworks/artifacts/models/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.2/src/sageworks/artifacts/models/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     4419 2023-05-14 17:29:06.000000 sageworks-0.1.5.2/src/sageworks/artifacts/models/model.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.659284 sageworks-0.1.5.2/src/sageworks/aws_service_broker/
+-rw-r--r--   0 briford    (501) staff       (20)     7633 2023-05-04 14:48:56.000000 sageworks-0.1.5.2/src/sageworks/aws_service_broker/aws_account_clamp.py
+-rw-r--r--   0 briford    (501) staff       (20)     9590 2023-05-12 17:33:32.000000 sageworks-0.1.5.2/src/sageworks/aws_service_broker/aws_service_broker.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.661256 sageworks-0.1.5.2/src/sageworks/aws_service_broker/aws_service_connectors/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-14 19:44:44.000000 sageworks-0.1.5.2/src/sageworks/aws_service_broker/aws_service_connectors/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     2501 2023-05-11 17:16:49.000000 sageworks-0.1.5.2/src/sageworks/aws_service_broker/aws_service_connectors/connector.py
+-rw-r--r--   0 briford    (501) staff       (20)     6066 2023-05-11 17:16:49.000000 sageworks-0.1.5.2/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py
+-rw-r--r--   0 briford    (501) staff       (20)     3325 2023-05-11 18:41:08.000000 sageworks-0.1.5.2/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py
+-rw-r--r--   0 briford    (501) staff       (20)     5772 2023-05-12 17:34:32.000000 sageworks-0.1.5.2/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py
+-rw-r--r--   0 briford    (501) staff       (20)     4297 2023-05-11 18:40:16.000000 sageworks-0.1.5.2/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py
+-rw-r--r--   0 briford    (501) staff       (20)     2949 2023-05-10 23:23:46.000000 sageworks-0.1.5.2/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.661936 sageworks-0.1.5.2/src/sageworks/transforms/
+-rw-r--r--   0 briford    (501) staff       (20)     1432 2023-03-17 17:39:22.000000 sageworks-0.1.5.2/src/sageworks/transforms/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.2/src/sageworks/transforms/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.620674 sageworks-0.1.5.2/src/sageworks/transforms/data_loaders/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.662307 sageworks-0.1.5.2/src/sageworks/transforms/data_loaders/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)     7367 2023-05-05 02:30:09.000000 sageworks-0.1.5.2/src/sageworks/transforms/data_loaders/heavy/s3_heavy_to_data_source.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.663122 sageworks-0.1.5.2/src/sageworks/transforms/data_loaders/light/
+-rw-r--r--   0 briford    (501) staff       (20)     2997 2023-04-14 22:16:23.000000 sageworks-0.1.5.2/src/sageworks/transforms/data_loaders/light/csv_to_data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     2483 2023-04-19 22:41:04.000000 sageworks-0.1.5.2/src/sageworks/transforms/data_loaders/light/json_to_data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     4155 2023-04-30 02:50:10.000000 sageworks-0.1.5.2/src/sageworks/transforms/data_loaders/light/s3_to_data_source_light.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.663428 sageworks-0.1.5.2/src/sageworks/transforms/data_to_data/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.2/src/sageworks/transforms/data_to_data/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.663517 sageworks-0.1.5.2/src/sageworks/transforms/data_to_data/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.2/src/sageworks/transforms/data_to_data/heavy/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.663598 sageworks-0.1.5.2/src/sageworks/transforms/data_to_data/heavy/emr/
+-rw-r--r--   0 briford    (501) staff       (20)       68 2023-03-15 02:15:48.000000 sageworks-0.1.5.2/src/sageworks/transforms/data_to_data/heavy/emr/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.663779 sageworks-0.1.5.2/src/sageworks/transforms/data_to_data/heavy/glue/
+-rw-r--r--   0 briford    (501) staff       (20)       48 2023-03-15 02:16:45.000000 sageworks-0.1.5.2/src/sageworks/transforms/data_to_data/heavy/glue/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.664404 sageworks-0.1.5.2/src/sageworks/transforms/data_to_data/light/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.2/src/sageworks/transforms/data_to_data/light/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     2231 2023-05-12 22:12:48.000000 sageworks-0.1.5.2/src/sageworks/transforms/data_to_data/light/clean_data.py
+-rw-r--r--   0 briford    (501) staff       (20)     2298 2023-05-12 21:29:54.000000 sageworks-0.1.5.2/src/sageworks/transforms/data_to_data/light/data_to_data_light.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.664784 sageworks-0.1.5.2/src/sageworks/transforms/data_to_features/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.2/src/sageworks/transforms/data_to_features/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.664998 sageworks-0.1.5.2/src/sageworks/transforms/data_to_features/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.2/src/sageworks/transforms/data_to_features/heavy/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     5817 2023-05-12 17:46:07.000000 sageworks-0.1.5.2/src/sageworks/transforms/data_to_features/heavy/data_to_features_heavy.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.665283 sageworks-0.1.5.2/src/sageworks/transforms/data_to_features/heavy/emr/
+-rw-r--r--   0 briford    (501) staff       (20)       68 2023-03-15 02:18:14.000000 sageworks-0.1.5.2/src/sageworks/transforms/data_to_features/heavy/emr/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.665568 sageworks-0.1.5.2/src/sageworks/transforms/data_to_features/heavy/glue/
+-rw-r--r--   0 briford    (501) staff       (20)       48 2023-03-15 02:18:14.000000 sageworks-0.1.5.2/src/sageworks/transforms/data_to_features/heavy/glue/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.666195 sageworks-0.1.5.2/src/sageworks/transforms/data_to_features/light/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.2/src/sageworks/transforms/data_to_features/light/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     2538 2023-05-12 17:52:28.000000 sageworks-0.1.5.2/src/sageworks/transforms/data_to_features/light/data_to_features_light.py
+-rw-r--r--   0 briford    (501) staff       (20)     2974 2023-05-12 17:46:07.000000 sageworks-0.1.5.2/src/sageworks/transforms/data_to_features/light/rdkit_descriptors.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.666440 sageworks-0.1.5.2/src/sageworks/transforms/features_to_features/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 18:06:15.000000 sageworks-0.1.5.2/src/sageworks/transforms/features_to_features/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.621544 sageworks-0.1.5.2/src/sageworks/transforms/features_to_features/heavy/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.666535 sageworks-0.1.5.2/src/sageworks/transforms/features_to_features/heavy/emr/
+-rw-r--r--   0 briford    (501) staff       (20)       68 2023-03-15 02:18:46.000000 sageworks-0.1.5.2/src/sageworks/transforms/features_to_features/heavy/emr/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.666783 sageworks-0.1.5.2/src/sageworks/transforms/features_to_features/heavy/glue/
+-rw-r--r--   0 briford    (501) staff       (20)       48 2023-03-15 02:18:46.000000 sageworks-0.1.5.2/src/sageworks/transforms/features_to_features/heavy/glue/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.667089 sageworks-0.1.5.2/src/sageworks/transforms/features_to_model/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.2/src/sageworks/transforms/features_to_model/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     7840 2023-05-12 17:53:53.000000 sageworks-0.1.5.2/src/sageworks/transforms/features_to_model/features_to_model.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.667683 sageworks-0.1.5.2/src/sageworks/transforms/features_to_model/light_model_harness/
+-rw-r--r--   0 briford    (501) staff       (20)        8 2023-03-25 02:07:31.000000 sageworks-0.1.5.2/src/sageworks/transforms/features_to_model/light_model_harness/requirements.txt
+-rw-r--r--   0 briford    (501) staff       (20)     5179 2023-04-18 16:01:35.000000 sageworks-0.1.5.2/src/sageworks/transforms/features_to_model/light_model_harness/xgb_model.template
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.668037 sageworks-0.1.5.2/src/sageworks/transforms/model_to_endpoint/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.2/src/sageworks/transforms/model_to_endpoint/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     2800 2023-05-12 17:54:23.000000 sageworks-0.1.5.2/src/sageworks/transforms/model_to_endpoint/model_to_endpoint.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.669273 sageworks-0.1.5.2/src/sageworks/transforms/pandas_transforms/
+-rw-r--r--   0 briford    (501) staff       (20)     2745 2023-04-13 18:18:49.000000 sageworks-0.1.5.2/src/sageworks/transforms/pandas_transforms/data_to_pandas.py
+-rw-r--r--   0 briford    (501) staff       (20)     3144 2023-04-13 18:18:49.000000 sageworks-0.1.5.2/src/sageworks/transforms/pandas_transforms/features_to_pandas.py
+-rw-r--r--   0 briford    (501) staff       (20)     7003 2023-05-12 21:36:54.000000 sageworks-0.1.5.2/src/sageworks/transforms/pandas_transforms/pandas_to_data.py
+-rw-r--r--   0 briford    (501) staff       (20)    10872 2023-05-12 17:52:28.000000 sageworks-0.1.5.2/src/sageworks/transforms/pandas_transforms/pandas_to_features.py
+-rw-r--r--   0 briford    (501) staff       (20)     7517 2023-05-12 23:56:39.000000 sageworks-0.1.5.2/src/sageworks/transforms/pandas_transforms/pandas_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     6705 2023-05-14 17:33:24.000000 sageworks-0.1.5.2/src/sageworks/transforms/transform.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.671659 sageworks-0.1.5.2/src/sageworks/utils/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 02:34:19.000000 sageworks-0.1.5.2/src/sageworks/utils/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     3962 2023-04-30 02:31:13.000000 sageworks-0.1.5.2/src/sageworks/utils/cache.py
+-rw-r--r--   0 briford    (501) staff       (20)     5113 2023-04-09 21:27:30.000000 sageworks-0.1.5.2/src/sageworks/utils/df_to_endpoint.py
+-rw-r--r--   0 briford    (501) staff       (20)     2417 2023-05-14 17:23:33.000000 sageworks-0.1.5.2/src/sageworks/utils/iso_8601.py
+-rw-r--r--   0 briford    (501) staff       (20)     6532 2023-05-05 02:30:09.000000 sageworks-0.1.5.2/src/sageworks/utils/redis_cache.py
+-rw-r--r--   0 briford    (501) staff       (20)     3618 2023-04-17 19:53:54.000000 sageworks-0.1.5.2/src/sageworks/utils/sageworks_config.py
+-rw-r--r--   0 briford    (501) staff       (20)     3558 2023-04-12 15:59:21.000000 sageworks-0.1.5.2/src/sageworks/utils/sageworks_event_bridge.py
+-rw-r--r--   0 briford    (501) staff       (20)      531 2023-04-02 18:05:33.000000 sageworks-0.1.5.2/src/sageworks/utils/sageworks_logging.py
+-rw-r--r--   0 briford    (501) staff       (20)     2209 2023-04-02 19:53:47.000000 sageworks-0.1.5.2/src/sageworks/utils/sageworks_sqs.py
+-rw-r--r--   0 briford    (501) staff       (20)     1469 2023-05-15 01:49:43.000000 sageworks-0.1.5.2/src/sageworks/utils/type_abbrev.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.672993 sageworks-0.1.5.2/src/sageworks/views/
+-rw-r--r--   0 briford    (501) staff       (20)    11812 2023-05-12 17:36:11.000000 sageworks-0.1.5.2/src/sageworks/views/artifacts_text_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     3063 2023-05-12 17:33:32.000000 sageworks-0.1.5.2/src/sageworks/views/artifacts_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     4307 2023-05-15 19:34:45.000000 sageworks-0.1.5.2/src/sageworks/views/data_source_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     4307 2023-05-15 22:08:31.000000 sageworks-0.1.5.2/src/sageworks/views/feature_set_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     1296 2023-04-19 17:02:05.000000 sageworks-0.1.5.2/src/sageworks/views/view.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.676103 sageworks-0.1.5.2/src/sageworks/web_components/
+-rw-r--r--   0 briford    (501) staff       (20)     1304 2023-05-05 02:30:09.000000 sageworks-0.1.5.2/src/sageworks/web_components/box_plot.py
+-rw-r--r--   0 briford    (501) staff       (20)     1661 2023-04-08 01:37:21.000000 sageworks-0.1.5.2/src/sageworks/web_components/confusion_matrix.py
+-rw-r--r--   0 briford    (501) staff       (20)     2316 2023-05-15 19:38:51.000000 sageworks-0.1.5.2/src/sageworks/web_components/data_source_details.py
+-rw-r--r--   0 briford    (501) staff       (20)     1247 2023-04-09 21:27:30.000000 sageworks-0.1.5.2/src/sageworks/web_components/feature_details.py
+-rw-r--r--   0 briford    (501) staff       (20)      815 2023-04-02 19:53:47.000000 sageworks-0.1.5.2/src/sageworks/web_components/feature_importance.py
+-rw-r--r--   0 briford    (501) staff       (20)     2316 2023-05-15 22:17:03.000000 sageworks-0.1.5.2/src/sageworks/web_components/feature_set_details.py
+-rw-r--r--   0 briford    (501) staff       (20)     1182 2023-04-07 23:04:10.000000 sageworks-0.1.5.2/src/sageworks/web_components/histogram.py
+-rw-r--r--   0 briford    (501) staff       (20)      837 2023-04-09 21:27:30.000000 sageworks-0.1.5.2/src/sageworks/web_components/line_chart.py
+-rw-r--r--   0 briford    (501) staff       (20)     1507 2023-04-09 21:30:08.000000 sageworks-0.1.5.2/src/sageworks/web_components/model_data.py
+-rw-r--r--   0 briford    (501) staff       (20)     1703 2023-04-02 19:53:47.000000 sageworks-0.1.5.2/src/sageworks/web_components/model_details.py
+-rw-r--r--   0 briford    (501) staff       (20)     1551 2023-04-09 21:27:30.000000 sageworks-0.1.5.2/src/sageworks/web_components/scatter_plot.py
+-rw-r--r--   0 briford    (501) staff       (20)     2227 2023-05-11 20:41:25.000000 sageworks-0.1.5.2/src/sageworks/web_components/table.py
+-rw-r--r--   0 briford    (501) staff       (20)     2134 2023-05-15 22:23:21.000000 sageworks-0.1.5.2/src/sageworks/web_components/violin_plot.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.654194 sageworks-0.1.5.2/src/sageworks.egg-info/
+-rw-r--r--   0 briford    (501) staff       (20)     5964 2023-05-15 23:21:53.000000 sageworks-0.1.5.2/src/sageworks.egg-info/PKG-INFO
+-rw-r--r--   0 briford    (501) staff       (20)     8884 2023-05-15 23:21:53.000000 sageworks-0.1.5.2/src/sageworks.egg-info/SOURCES.txt
+-rw-r--r--   0 briford    (501) staff       (20)        1 2023-05-15 23:21:53.000000 sageworks-0.1.5.2/src/sageworks.egg-info/dependency_links.txt
+-rw-r--r--   0 briford    (501) staff       (20)      134 2023-05-15 23:21:53.000000 sageworks-0.1.5.2/src/sageworks.egg-info/requires.txt
+-rw-r--r--   0 briford    (501) staff       (20)       10 2023-05-15 23:21:53.000000 sageworks-0.1.5.2/src/sageworks.egg-info/top_level.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.676340 sageworks-0.1.5.2/tests/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.677521 sageworks-0.1.5.2/tests/artifacts/
+-rw-r--r--   0 briford    (501) staff       (20)     1250 2023-05-14 17:27:17.000000 sageworks-0.1.5.2/tests/artifacts/data_source_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     1483 2023-04-11 20:37:15.000000 sageworks-0.1.5.2/tests/artifacts/endpoint_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     1155 2023-05-14 17:27:17.000000 sageworks-0.1.5.2/tests/artifacts/feature_set_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      799 2023-04-02 18:05:33.000000 sageworks-0.1.5.2/tests/artifacts/model_tests.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.677959 sageworks-0.1.5.2/tests/aws_account/
+-rw-r--r--   0 briford    (501) staff       (20)     1105 2023-05-05 02:37:56.000000 sageworks-0.1.5.2/tests/aws_account/aws_account_clamp_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      642 2023-05-05 02:38:20.000000 sageworks-0.1.5.2/tests/aws_account/aws_service_broker_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     3341 2023-04-19 17:23:07.000000 sageworks-0.1.5.2/tests/create_sageworks_objs_for_tests.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.678897 sageworks-0.1.5.2/tests/transforms/
+-rw-r--r--   0 briford    (501) staff       (20)      554 2023-05-12 17:46:18.000000 sageworks-0.1.5.2/tests/transforms/data_to_data_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      682 2023-05-12 18:00:39.000000 sageworks-0.1.5.2/tests/transforms/data_to_features_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      655 2023-05-12 18:01:20.000000 sageworks-0.1.5.2/tests/transforms/features_to_model_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      642 2023-05-12 17:46:18.000000 sageworks-0.1.5.2/tests/transforms/model_to_endpoint_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      628 2023-05-12 17:46:18.000000 sageworks-0.1.5.2/tests/transforms/pandas_to_data_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      729 2023-05-05 02:35:30.000000 sageworks-0.1.5.2/tox.ini
```

### Comparing `sageworks-0.1.5.1/.gitignore` & `sageworks-0.1.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/LICENSE` & `sageworks-0.1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/Makefile` & `sageworks-0.1.5.2/Makefile`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/PKG-INFO` & `sageworks-0.1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sageworks
-Version: 0.1.5.1
+Version: 0.1.5.2
 Summary: SageWorks: A Python WorkBench for creating and deploying SageMaker Models
 Home-page: https://github.com/SuperCowPowers/sageworks
 Author: SuperCowPowers LLC
 Author-email: support@supercowpowers.com
 License: MIT
 Keywords: SageMaker,Machine Learning,AWS,Python,Utilities
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `sageworks-0.1.5.1/Readme.md` & `sageworks-0.1.5.2/Readme.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/applications/aws_dashboard/assets/custom.css` & `sageworks-0.1.5.2/applications/aws_dashboard/assets/custom.css`

 * *Files 14% similar despite different names*

```diff
@@ -140,20 +140,26 @@
 
 /* Typography
 –––––––––––––––––––––––––––––––––––––––––––––––––– */
 h1, h2, h3, h4, h5, h6 {
   margin-top: 0;
   margin-bottom: 0;
   font-weight: 300; }
-h1 { font-size: 4.0rem; line-height: 1.2;  letter-spacing: -.1rem; margin-bottom: 0rem; }
-h2 { font-size: 3.3rem; line-height: 1.25; letter-spacing: -.1rem; margin-bottom: 0rem; margin-top: 1.8rem;}
-h3 { font-size: 2.7rem; line-height: 1.3;  letter-spacing: -.1rem; margin-bottom: 0rem; margin-top: 1.5rem;}
-h4 { font-size: 2.6rem; line-height: 1.35; letter-spacing: -.08rem; margin-bottom: 0rem; margin-top: 1.2rem;}
-h5 { font-size: 2.2rem; line-height: 1.5;  letter-spacing: -.05rem; margin-bottom: 0rem; margin-top: 0.6rem;}
-h6 { font-size: 2.0rem; line-height: 1.6;  letter-spacing: 0; margin-bottom: 0.75rem; margin-top: 0.75rem;}
+h1 { font-size: 4.0rem; line-height: 1.2;  letter-spacing: -.1rem;
+  margin-bottom: 0rem; color: rgb(200, 200, 200);}
+h2 { font-size: 3.3rem; line-height: 1.25; letter-spacing: -.1rem;
+  margin-bottom: 0rem; margin-top: 1.8rem; color: rgb(200, 200, 200);}
+h3 { font-size: 2.7rem; line-height: 1.3;  letter-spacing: -.1rem;
+  margin-bottom: 0rem; margin-top: 1.5rem; color: rgb(200, 200, 200);}
+h4 { font-size: 2.6rem; line-height: 1.35; letter-spacing: -.08rem;
+  margin-bottom: 0rem; margin-top: 1.2rem; color: rgb(200, 200, 200);}
+h5 { font-size: 2.2rem; line-height: 1.5;  letter-spacing: -.05rem;
+  margin-bottom: 0rem; margin-top: 0.6rem; color: rgb(200, 200, 200);}
+h6 { font-size: 2.0rem; line-height: 1.6;  letter-spacing: 0;
+  margin-bottom: 0.75rem; margin-top: 0.75rem; color: rgb(200, 200, 200);}
 
 p {
   margin-top: 0; }
 
 
 /* Links
 –––––––––––––––––––––––––––––––––––––––––––––––––– */
@@ -305,24 +311,24 @@
 /* Lists
 –––––––––––––––––––––––––––––––––––––––––––––––––– */
 ul {
   list-style: circle inside; }
 ol {
   list-style: decimal inside; }
 ol, ul {
-  padding-left: 0;
+  padding-left: 30;
   margin-top: 0; }
 ul ul,
 ul ol,
 ol ol,
 ol ul {
   margin: 1.5rem 0 1.5rem 3rem;
-  font-size: 90%; }
+  font-size: 100%; }
 li {
-  margin-bottom: 1rem; }
+  margin: -2px; }
 
 
 /* Tables
 –––––––––––––––––––––––––––––––––––––––––––––––––– */
 table {
   border: 4px solid #222222;
   border-collapse: collapse;
```

### Comparing `sageworks-0.1.5.1/applications/aws_dashboard/aws_dashboard.py` & `sageworks-0.1.5.2/applications/aws_dashboard/aws_dashboard.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/applications/aws_dashboard/pages/callbacks/data_sources_callbacks.py` & `sageworks-0.1.5.2/applications/aws_dashboard/pages/callbacks/data_sources_callbacks.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         return [header, column_setup, sample_rows.to_dict("records")]
 
 
 def update_violin_plots(app: Dash, data_source_web_view: DataSourceWebView):
     """Updates the Violin Plots when a new data source is selected"""
 
     @app.callback(
-        Output("violin_plot", "figure"),
+        Output("data_source_violin_plot", "figure"),
         Input("data_sources_table", "derived_viewport_selected_row_ids"),
         prevent_initial_call=True,
     )
     def generate_new_violin_plot(selected_rows):
         print(f"Selected Rows: {selected_rows}")
         if not selected_rows or selected_rows[0] is None:
             return dash.no_update
```

### Comparing `sageworks-0.1.5.1/applications/aws_dashboard/pages/callbacks/endpoints_callbacks.py` & `sageworks-0.1.5.2/applications/aws_dashboard/pages/callbacks/endpoints_callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/applications/aws_dashboard/pages/callbacks/main_callbacks.py` & `sageworks-0.1.5.2/applications/aws_dashboard/pages/callbacks/main_callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/applications/aws_dashboard/pages/callbacks/models_callbacks.py` & `sageworks-0.1.5.2/applications/aws_dashboard/pages/callbacks/models_callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/applications/aws_dashboard/pages/data/toy_data.csv` & `sageworks-0.1.5.2/applications/aws_dashboard/pages/data/toy_data.csv`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/applications/aws_dashboard/pages/data/toy_scores.json` & `sageworks-0.1.5.2/applications/aws_dashboard/pages/data/toy_scores.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/applications/aws_dashboard/pages/data_sources.py` & `sageworks-0.1.5.2/applications/aws_dashboard/pages/data_sources.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 # Data Source Details
 details = data_source_broker.data_source_details(0)
 data_details = data_source_details.create("data_source_details", details)
 
 # Create a box plot of all the numeric columns in the sample rows
 smart_sample_rows = data_source_broker.data_source_smart_sample(0)
-violin = violin_plot.create(smart_sample_rows)
+violin = violin_plot.create("data_source_violin_plot", smart_sample_rows)
 
 # Create our components
 components = {
     "data_sources_table": data_sources_table,
     "data_source_details": data_details,
     "data_source_sample_rows": data_source_sample_rows,
     "violin_plot": violin,
```

### Comparing `sageworks-0.1.5.1/applications/aws_dashboard/pages/endpoints.py` & `sageworks-0.1.5.2/applications/aws_dashboard/pages/endpoints.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/applications/aws_dashboard/pages/feature_sets.py` & `sageworks-0.1.5.2/applications/aws_dashboard/pages/main.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,49 +1,69 @@
-"""DataSources:  A SageWorks Web Interface to view, interact, and manage Data Sources"""
+"""Main: The main SageWorks Web Interface to view, interact, and manage SageWorks Artifacts"""
 from dash import register_page
 import dash
 
 # SageWorks Imports
-from sageworks.web_components import scatter_plot
 from sageworks.views.artifacts_web_view import ArtifactsWebView
 from sageworks.web_components import table
 
 # Local Imports
-from pages.layout.feature_sets_layout import feature_sets_layout
-import pages.callbacks.feature_sets_callbacks as callbacks
+from pages.layout.main_layout import main_layout
+import pages.callbacks.main_callbacks as callbacks
 
-register_page(__name__, path="/feature_sets")
+register_page(__name__, path="/")
 
 
 # Okay feels a bit weird but Dash pages just have a bunch of top level code (no classes/methods)
 
 # Grab a view that gives us a summary of all the artifacts currently in SageWorks
-sageworks_artifacts = ArtifactsWebView()
-feature_sets_summary = sageworks_artifacts.feature_sets_summary()
+web_artifacts_summary = ArtifactsWebView()
+sageworks_artifacts = web_artifacts_summary.view_data()
 
-# Create a table to display the feature sets
-feature_sets_table = table.create(
-    "FEATURE_SETS_DETAILS",
-    feature_sets_summary,
+# Grab the Artifact Information DataFrame for each AWS Service and pass it to the table creation
+tables = dict()
+tables["INCOMING_DATA"] = table.create(
+    "INCOMING_DATA",
+    sageworks_artifacts["INCOMING_DATA"],
+    header_color="rgb(60, 60, 100)",
+)
+tables["DATA_SOURCES"] = table.create(
+    "DATA_SOURCES",
+    sageworks_artifacts["DATA_SOURCES"],
+    header_color="rgb(100, 60, 60)",
+    markdown_columns=["Name"],
+)
+tables["FEATURE_SETS"] = table.create(
+    "FEATURE_SETS",
+    sageworks_artifacts["FEATURE_SETS"],
     header_color="rgb(100, 100, 60)",
-    row_select="single",
     markdown_columns=["Feature Group"],
 )
-
-# Create a fake scatter plot
-scatter1 = scatter_plot.create()
-scatter2 = scatter_plot.create(variant=2)
+tables["MODELS"] = table.create(
+    "MODELS",
+    sageworks_artifacts["MODELS"],
+    header_color="rgb(60, 100, 60)",
+    markdown_columns=["Model Group"],
+)
+tables["ENDPOINTS"] = table.create(
+    "ENDPOINTS",
+    sageworks_artifacts["ENDPOINTS"],
+    header_color="rgb(100, 60, 100)",
+    markdown_columns=["Name"],
+)
 
 # Create our components
 components = {
-    "feature_sets_details": feature_sets_table,
-    "scatter1": scatter1,
-    "scatter2": scatter2,
+    "incoming_data": tables["INCOMING_DATA"],
+    "data_sources": tables["DATA_SOURCES"],
+    "feature_sets": tables["FEATURE_SETS"],
+    "models": tables["MODELS"],
+    "endpoints": tables["ENDPOINTS"],
 }
 
 # Setup our callbacks/connections
 app = dash.get_app()
-callbacks.update_last_updated(app)
-callbacks.update_feature_sets_table(app, sageworks_artifacts)
+callbacks.update_last_updated(app, web_artifacts_summary)
+callbacks.update_artifact_tables(app)
 
 # Set up our layout (Dash looks for a var called layout)
-layout = feature_sets_layout(components)
+layout = main_layout(components)
```

### Comparing `sageworks-0.1.5.1/applications/aws_dashboard/pages/layout/data_sources_layout.py` & `sageworks-0.1.5.2/applications/aws_dashboard/pages/layout/data_sources_layout.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,44 +21,45 @@
                     ),
                     dbc.Row(style={"padding": "30px 0px 0px 0px"}),
                 ]
             ),
             # List out all the Data Sources
             dbc.Row(components["data_sources_table"]),
             # Data Source Details, Sample Rows, and Violin Plots
-            # Row [ Column 1                       Column 2 ]
-            #       (Row(Data Source Details))     Row(Sample Rows)
-            #                                      Row(Violin Plots)
+            # Row [ Sample Rows ]
+            # Row [ Column 1                      Column 2 ]
+            #       (Row(Data Source Details))    Row(Violin Plots)
+            #
+            dbc.Row(
+                html.H3("Sampled Rows", id="sample_rows_header"),
+                style={"padding": "30px 0px 10px 0px"},
+            ),
+            dbc.Row(
+                components["data_source_sample_rows"],
+                style={"padding": "0px 0px 30px 0px"},
+            ),
             dbc.Row(
                 [
                     # Column 1: Data Source Details
                     dbc.Col(
                         [
                             dbc.Row(
                                 html.H3("Details", id="data_details_header"),
-                                style={"padding": "30px 0px 10px 0px"},
+                                style={"padding": "0px 0px 10px 0px"},
                             ),
                             dbc.Row(
                                 components["data_source_details"],
                                 style={"padding": "0px 0px 30px 0px"},
                             ),
                         ],
                         width=4,
                     ),
                     # Column 2: Sample Rows and Violin Plots
                     dbc.Col(
                         [
-                            dbc.Row(
-                                html.H3("Sampled Rows", id="sample_rows_header"),
-                                style={"padding": "30px 0px 10px 0px"},
-                            ),
-                            dbc.Row(
-                                components["data_source_sample_rows"],
-                                style={"padding": "0px 0px 30px 0px"},
-                            ),
                             dbc.Row(components["violin_plot"]),
                         ],
                         width=8,
                     ),
                     # Just the auto updater
                     dcc.Interval(id="data-sources-updater", interval=5000, n_intervals=0),
                 ]
```

### Comparing `sageworks-0.1.5.1/applications/aws_dashboard/pages/layout/endpoints_layout.py` & `sageworks-0.1.5.2/applications/aws_dashboard/pages/layout/endpoints_layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/applications/aws_dashboard/pages/layout/main_layout.py` & `sageworks-0.1.5.2/applications/aws_dashboard/pages/layout/main_layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/applications/aws_dashboard/pages/layout/models_layout.py` & `sageworks-0.1.5.2/applications/aws_dashboard/pages/layout/models_layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/applications/aws_dashboard/pages/models.py` & `sageworks-0.1.5.2/applications/aws_dashboard/pages/models.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/applications/hello_world/callbacks.py` & `sageworks-0.1.5.2/applications/hello_world/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/applications/hello_world/hello_world.py` & `sageworks-0.1.5.2/applications/hello_world/hello_world.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/applications/hello_world/layout.py` & `sageworks-0.1.5.2/applications/hello_world/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/applications/model_viewer/callbacks.py` & `sageworks-0.1.5.2/applications/model_viewer/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/applications/model_viewer/data/toy_data.csv` & `sageworks-0.1.5.2/applications/model_viewer/data/toy_data.csv`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/applications/model_viewer/data/toy_scores.json` & `sageworks-0.1.5.2/applications/model_viewer/data/toy_scores.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/applications/model_viewer/layout.py` & `sageworks-0.1.5.2/applications/model_viewer/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/applications/model_viewer/model_viewer.py` & `sageworks-0.1.5.2/applications/model_viewer/model_viewer.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/aws_setup/aws_account_check.py` & `sageworks-0.1.5.2/aws_setup/aws_account_check.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/aws_setup/build_ml_pipeline.py` & `sageworks-0.1.5.2/aws_setup/build_ml_pipeline.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/aws_setup/sageworks_cdk/README.md` & `sageworks-0.1.5.2/aws_setup/sageworks_cdk/README.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/aws_setup/sageworks_cdk/app.py` & `sageworks-0.1.5.2/aws_setup/sageworks_cdk/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/aws_setup/sageworks_cdk/cdk.json` & `sageworks-0.1.5.2/aws_setup/sageworks_cdk/cdk.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/aws_setup/sageworks_cdk/stacks/sageworks_stack.py` & `sageworks-0.1.5.2/aws_setup/sageworks_cdk/stacks/sageworks_stack.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/aws_setup/sageworks_cdk/tests/unit/test_sageworks_sandbox_stack.py` & `sageworks-0.1.5.2/aws_setup/sageworks_cdk/tests/unit/test_sageworks_sandbox_stack.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/data/abalone.csv` & `sageworks-0.1.5.2/data/abalone.csv`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/data/test_data.csv` & `sageworks-0.1.5.2/data/test_data.csv`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/data/test_data.json` & `sageworks-0.1.5.2/data/test_data.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/docs/admin_notes.md` & `sageworks-0.1.5.2/docs/admin_notes.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/docs/images/big_spider.png` & `sageworks-0.1.5.2/docs/images/big_spider.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/docs/images/graph_representation.png` & `sageworks-0.1.5.2/docs/images/graph_representation.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/docs/images/powered_aws_dark_blue.png` & `sageworks-0.1.5.2/docs/images/powered_aws_dark_blue.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/docs/images/powered_aws_transparent.png` & `sageworks-0.1.5.2/docs/images/powered_aws_transparent.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/docs/images/powered_aws_white.png` & `sageworks-0.1.5.2/docs/images/powered_aws_white.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/docs/images/powered_aws_with_tm_grey.png` & `sageworks-0.1.5.2/docs/images/powered_aws_with_tm_grey.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/docs/images/sageworks.png` & `sageworks-0.1.5.2/docs/images/sageworks.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/docs/images/sageworks_concepts.png` & `sageworks-0.1.5.2/docs/images/sageworks_concepts.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/docs/images/scp.png` & `sageworks-0.1.5.2/docs/images/scp.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/docs/images/scp_labs.png` & `sageworks-0.1.5.2/docs/images/scp_labs.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/docs/images/small_spider.png` & `sageworks-0.1.5.2/docs/images/small_spider.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/docs/sageworks_classes_concepts.md` & `sageworks-0.1.5.2/docs/sageworks_classes_concepts.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/docs/scp_consulting.md` & `sageworks-0.1.5.2/docs/scp_consulting.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/examples/data_to_data_example.py` & `sageworks-0.1.5.2/examples/data_to_data_example.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/notebooks/ML_Pipeline_with_SageWorks.ipynb` & `sageworks-0.1.5.2/notebooks/ML_Pipeline_with_SageWorks.ipynb`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/notebooks/images/athena_query_aqsol.png` & `sageworks-0.1.5.2/notebooks/images/athena_query_aqsol.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/notebooks/images/aws_dashboard_aqsol.png` & `sageworks-0.1.5.2/notebooks/images/aws_dashboard_aqsol.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/notebooks/images/dashboard_aqsol_features.png` & `sageworks-0.1.5.2/notebooks/images/dashboard_aqsol_features.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/notebooks/images/model_screenshot.png` & `sageworks-0.1.5.2/notebooks/images/model_screenshot.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/notebooks/images/sageworks_concepts.png` & `sageworks-0.1.5.2/notebooks/images/sageworks_concepts.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/notebooks/images/scp_labs.png` & `sageworks-0.1.5.2/notebooks/images/scp_labs.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/scripts/data_source_tags.py` & `sageworks-0.1.5.2/scripts/data_source_tags.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/scripts/generate_jsonl_data.py` & `sageworks-0.1.5.2/scripts/generate_jsonl_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/scripts/list_data_sources.py` & `sageworks-0.1.5.2/scripts/list_data_sources.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/setup.cfg` & `sageworks-0.1.5.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/setup.py` & `sageworks-0.1.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     """Simple directory walker"""
     return [(os.path.join(".", d), [os.path.join(d, f) for f in files]) for d, _, files in os.walk(dir_name)]
 
 
 setup(
     name="sageworks",
     # use_scm_version=True,
-    version="0.1.5.1",
+    version="0.1.5.2",
     description="SageWorks: A Python WorkBench for creating and deploying SageMaker Models",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="SuperCowPowers LLC",
     author_email="support@supercowpowers.com",
     url="https://github.com/SuperCowPowers/sageworks",
     packages=find_packages("src"),
```

### Comparing `sageworks-0.1.5.1/src/sageworks/__init__.py` & `sageworks-0.1.5.2/src/sageworks/__init__.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/algorithms/table/light/data_source_eda.py` & `sageworks-0.1.5.2/src/sageworks/algorithms/table/light/data_source_eda.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/algorithms/table/light/feature_spider.py` & `sageworks-0.1.5.2/src/sageworks/algorithms/table/light/feature_spider.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/algorithms/table/light/row_tagger.py` & `sageworks-0.1.5.2/src/sageworks/algorithms/table/light/row_tagger.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/artifacts/Readme.md` & `sageworks-0.1.5.2/src/sageworks/artifacts/Readme.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/artifacts/artifact.py` & `sageworks-0.1.5.2/src/sageworks/artifacts/artifact.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/artifacts/data_sources/athena_source.py` & `sageworks-0.1.5.2/src/sageworks/artifacts/data_sources/athena_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/artifacts/data_sources/data_source.py` & `sageworks-0.1.5.2/src/sageworks/artifacts/data_sources/data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/artifacts/data_sources/data_source_abstract.py` & `sageworks-0.1.5.2/src/sageworks/artifacts/data_sources/data_source_abstract.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/artifacts/endpoints/endpoint.py` & `sageworks-0.1.5.2/src/sageworks/artifacts/endpoints/endpoint.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/artifacts/feature_sets/feature_set.py` & `sageworks-0.1.5.2/src/sageworks/artifacts/feature_sets/feature_set.py`

 * *Files 5% similar despite different names*

```diff
@@ -180,15 +180,15 @@
             f"    FROM (SELECT *, row_number() OVER (PARTITION BY {self.record_id} "
             f"        ORDER BY {self.event_time} desc, api_invocation_time DESC, write_time DESC) AS row_num "
             f'        FROM "{self.athena_table}") '
             "    WHERE row_num = 1 and  NOT is_deleted;"
         )
         return query
 
-    def details(self) -> dict:
+    def details_sav(self) -> dict:
         """Additional Details about this FeatureSet
         Returns:
             dict: A dictionary of details about this FeatureSet
         Notes:
             - num_columns
             - num_rows
             - column_details
@@ -214,14 +214,23 @@
         # Underlying Storage Details
         fs_details["storage_type"] = "athena"  # TODO: Add RDS support
         fs_details["storage_uuid"] = self.data_source.uuid
 
         # Return the details
         return fs_details
 
+    def details(self, recompute: bool = False) -> dict[dict]:
+        """Additional Details about this AthenaSource Artifact
+        Args:
+            recompute(bool): Recompute the details (default: False)
+        Returns:
+            dict(dict): A dictionary of details about this AthenaSource
+        """
+        return self.data_source.details(recompute)
+
     def delete(self):
         """Delete the Feature Set: Feature Group, Catalog Table, and S3 Storage Objects"""
 
         # Delete the Feature Group and ensure that it gets deleted
         remove_fg = FeatureGroup(name=self.feature_set_name, sagemaker_session=self.sm_session)
         remove_fg.delete()
         self.ensure_feature_group_deleted(remove_fg)
@@ -245,31 +254,40 @@
                 if error.response["Error"]["Code"] == "ResourceNotFound":
                     break
                 else:
                     raise error
             time.sleep(1)
         self.log.info(f"FeatureSet {feature_group.name} successfully deleted")
 
-    def quartiles(self) -> dict:
+    def quartiles(self, recompute: bool = False) -> dict:
         """Get the quartiles for the numeric columns of the underlying DataSource
+        Args:
+            recompute (bool): Recompute the quartiles (default=False)
         Returns:
             dict: A dictionary of quartiles for the numeric columns
         """
-        return self.data_source.quartiles()
+        return self.data_source.quartiles(recompute)
 
-    def sample_df(self) -> pd.DataFrame:
-        """Get a sample of the data from the underlying DataSource"""
-        return self.data_source.sample_df()
+    def sample_df(self, recompute: bool = False) -> pd.DataFrame:
+        """Get a sample of the data from the underlying DataSource
+        Args:
+            recompute (bool): Recompute the sample (default=False)
+        Returns:
+            pd.DataFrame: A sample of the data from the underlying DataSource
+        """
+        return self.data_source.sample_df(recompute)
 
-    def value_counts(self) -> dict:
+    def value_counts(self, recompute: bool = False) -> dict:
         """Get the quartiles for the string columns of the underlying DataSource
+        Args:
+            recompute (bool): Recompute the value counts (default=False)
         Returns:
             dict: A dictionary of value counts for the string columns
         """
-        return self.data_source.value_counts()
+        return self.data_source.value_counts(recompute)
 
 
 if __name__ == "__main__":
     """Exercise for FeatureSet Class"""
     from pprint import pprint
 
     # Setup Pandas output options
```

### Comparing `sageworks-0.1.5.1/src/sageworks/artifacts/models/model.py` & `sageworks-0.1.5.2/src/sageworks/artifacts/models/model.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/aws_service_broker/aws_account_clamp.py` & `sageworks-0.1.5.2/src/sageworks/aws_service_broker/aws_account_clamp.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/aws_service_broker/aws_service_broker.py` & `sageworks-0.1.5.2/src/sageworks/aws_service_broker/aws_service_broker.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/aws_service_broker/aws_service_connectors/connector.py` & `sageworks-0.1.5.2/src/sageworks/aws_service_broker/aws_service_connectors/connector.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py` & `sageworks-0.1.5.2/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py` & `sageworks-0.1.5.2/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py` & `sageworks-0.1.5.2/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py` & `sageworks-0.1.5.2/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py` & `sageworks-0.1.5.2/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/transforms/Readme.md` & `sageworks-0.1.5.2/src/sageworks/transforms/Readme.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/transforms/data_loaders/heavy/s3_heavy_to_data_source.py` & `sageworks-0.1.5.2/src/sageworks/transforms/data_loaders/heavy/s3_heavy_to_data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/transforms/data_loaders/light/csv_to_data_source.py` & `sageworks-0.1.5.2/src/sageworks/transforms/data_loaders/light/csv_to_data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/transforms/data_loaders/light/json_to_data_source.py` & `sageworks-0.1.5.2/src/sageworks/transforms/data_loaders/light/json_to_data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/transforms/data_loaders/light/s3_to_data_source_light.py` & `sageworks-0.1.5.2/src/sageworks/transforms/data_loaders/light/s3_to_data_source_light.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/transforms/data_to_data/light/clean_data.py` & `sageworks-0.1.5.2/src/sageworks/transforms/data_to_data/light/clean_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/transforms/data_to_data/light/data_to_data_light.py` & `sageworks-0.1.5.2/src/sageworks/transforms/data_to_data/light/data_to_data_light.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/transforms/data_to_features/heavy/data_to_features_heavy.py` & `sageworks-0.1.5.2/src/sageworks/transforms/data_to_features/heavy/data_to_features_heavy.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/transforms/data_to_features/light/data_to_features_light.py` & `sageworks-0.1.5.2/src/sageworks/transforms/data_to_features/light/data_to_features_light.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/transforms/data_to_features/light/rdkit_descriptors.py` & `sageworks-0.1.5.2/src/sageworks/transforms/data_to_features/light/rdkit_descriptors.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/transforms/features_to_model/features_to_model.py` & `sageworks-0.1.5.2/src/sageworks/transforms/features_to_model/features_to_model.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/transforms/features_to_model/light_model_harness/xgb_model.template` & `sageworks-0.1.5.2/src/sageworks/transforms/features_to_model/light_model_harness/xgb_model.template`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/transforms/model_to_endpoint/model_to_endpoint.py` & `sageworks-0.1.5.2/src/sageworks/transforms/model_to_endpoint/model_to_endpoint.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/transforms/pandas_transforms/data_to_pandas.py` & `sageworks-0.1.5.2/src/sageworks/transforms/pandas_transforms/data_to_pandas.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/transforms/pandas_transforms/features_to_pandas.py` & `sageworks-0.1.5.2/src/sageworks/transforms/pandas_transforms/features_to_pandas.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/transforms/pandas_transforms/pandas_to_data.py` & `sageworks-0.1.5.2/src/sageworks/transforms/pandas_transforms/pandas_to_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/transforms/pandas_transforms/pandas_to_features.py` & `sageworks-0.1.5.2/src/sageworks/transforms/pandas_transforms/pandas_to_features.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/transforms/pandas_transforms/pandas_utils.py` & `sageworks-0.1.5.2/src/sageworks/transforms/pandas_transforms/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/transforms/transform.py` & `sageworks-0.1.5.2/src/sageworks/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/utils/cache.py` & `sageworks-0.1.5.2/src/sageworks/utils/cache.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/utils/df_to_endpoint.py` & `sageworks-0.1.5.2/src/sageworks/utils/df_to_endpoint.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/utils/iso_8601.py` & `sageworks-0.1.5.2/src/sageworks/utils/iso_8601.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/utils/redis_cache.py` & `sageworks-0.1.5.2/src/sageworks/utils/redis_cache.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/utils/sageworks_config.py` & `sageworks-0.1.5.2/src/sageworks/utils/sageworks_config.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/utils/sageworks_event_bridge.py` & `sageworks-0.1.5.2/src/sageworks/utils/sageworks_event_bridge.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/utils/sageworks_logging.py` & `sageworks-0.1.5.2/src/sageworks/utils/sageworks_logging.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/utils/sageworks_sqs.py` & `sageworks-0.1.5.2/src/sageworks/utils/sageworks_sqs.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/views/artifacts_text_view.py` & `sageworks-0.1.5.2/src/sageworks/views/artifacts_text_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/views/artifacts_web_view.py` & `sageworks-0.1.5.2/src/sageworks/views/artifacts_web_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/views/data_source_web_view.py` & `sageworks-0.1.5.2/src/sageworks/views/data_source_web_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,16 @@
         """
         return {"DATA_SOURCES": self.data_sources_df}  # Just the DataSources Summary Dataframe
 
     def data_source_sample(self, data_source_index: int) -> pd.DataFrame:
         """Get a sample dataframe for the given DataSource Index"""
         data_uuid = self.data_source_name(data_source_index)
         if data_uuid is not None:
-            sample_rows = DataSource(data_uuid).sample_df()
+            ds = DataSource(data_uuid)
+            sample_rows = ds.sample_df()
         else:
             sample_rows = pd.DataFrame()
         return sample_rows
 
     def data_source_quartiles(self, data_source_index: int) -> (dict, None):
         """Get all columns quartiles for the given DataSource Index"""
         data_uuid = self.data_source_name(data_source_index)
@@ -67,15 +68,17 @@
         # Combine the sample rows with the quartiles data
         return pd.concat([sample_rows, quartiles_df]).reset_index(drop=True)
 
     def data_source_details(self, data_source_index: int) -> (dict, None):
         """Get all of the details for the given DataSource Index"""
         data_uuid = self.data_source_name(data_source_index)
         if data_uuid is not None:
-            details_data = DataSource(data_uuid).details()
+            ds = DataSource(data_uuid)
+            details_data = ds.details()
+            details_data["value_counts"] = ds.value_counts()
             return details_data
         else:
             return None
 
     def data_source_name(self, data_source_index: int) -> (str, None):
         """Helper method for getting the data source name for the given DataSource Index"""
         if not self.data_sources_df.empty and data_source_index < len(self.data_sources_df):
```

### Comparing `sageworks-0.1.5.1/src/sageworks/views/view.py` & `sageworks-0.1.5.2/src/sageworks/views/view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/web_components/box_plot.py` & `sageworks-0.1.5.2/src/sageworks/web_components/box_plot.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/web_components/confusion_matrix.py` & `sageworks-0.1.5.2/src/sageworks/web_components/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/web_components/feature_details.py` & `sageworks-0.1.5.2/src/sageworks/web_components/feature_details.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/web_components/feature_importance.py` & `sageworks-0.1.5.2/src/sageworks/web_components/feature_importance.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/web_components/histogram.py` & `sageworks-0.1.5.2/src/sageworks/web_components/histogram.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/web_components/line_chart.py` & `sageworks-0.1.5.2/src/sageworks/web_components/line_chart.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/web_components/model_data.py` & `sageworks-0.1.5.2/src/sageworks/web_components/model_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/web_components/model_details.py` & `sageworks-0.1.5.2/src/sageworks/web_components/model_details.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/web_components/scatter_plot.py` & `sageworks-0.1.5.2/src/sageworks/web_components/scatter_plot.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/web_components/table.py` & `sageworks-0.1.5.2/src/sageworks/web_components/table.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/src/sageworks/web_components/violin_plot.py` & `sageworks-0.1.5.2/src/sageworks/web_components/violin_plot.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,12 +35,18 @@
             row=i // num_columns + 1,
             col=i % num_columns + 1,
         )
     fig.update_layout(margin=dict(l=20, r=20, t=20, b=20))
     return fig
 
 
-def create(df: pd.DataFrame) -> dcc.Graph:
-    """Create a Violin Plot Graph Component"""
+def create(component_id: str, df: pd.DataFrame) -> dcc.Graph:
+    """Create a Violin Plot Graph Component
+    Args:
+        component_id (str): The ID of the UI component
+        df (pd.DataFrame): A dataframe of data
+    Returns:
+        dcc.Graph: A Dash Graph Component
+    """
 
     # Generate a figure and wrap it in a Dash Graph Component
-    return dcc.Graph(id="violin_plot", figure=create_figure(df))
+    return dcc.Graph(id=component_id, figure=create_figure(df))
```

### Comparing `sageworks-0.1.5.1/src/sageworks.egg-info/PKG-INFO` & `sageworks-0.1.5.2/src/sageworks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sageworks
-Version: 0.1.5.1
+Version: 0.1.5.2
 Summary: SageWorks: A Python WorkBench for creating and deploying SageMaker Models
 Home-page: https://github.com/SuperCowPowers/sageworks
 Author: SuperCowPowers LLC
 Author-email: support@supercowpowers.com
 License: MIT
 Keywords: SageMaker,Machine Learning,AWS,Python,Utilities
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `sageworks-0.1.5.1/src/sageworks.egg-info/SOURCES.txt` & `sageworks-0.1.5.2/src/sageworks.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -162,23 +162,26 @@
 src/sageworks/utils/df_to_endpoint.py
 src/sageworks/utils/iso_8601.py
 src/sageworks/utils/redis_cache.py
 src/sageworks/utils/sageworks_config.py
 src/sageworks/utils/sageworks_event_bridge.py
 src/sageworks/utils/sageworks_logging.py
 src/sageworks/utils/sageworks_sqs.py
+src/sageworks/utils/type_abbrev.py
 src/sageworks/views/artifacts_text_view.py
 src/sageworks/views/artifacts_web_view.py
 src/sageworks/views/data_source_web_view.py
+src/sageworks/views/feature_set_web_view.py
 src/sageworks/views/view.py
 src/sageworks/web_components/box_plot.py
 src/sageworks/web_components/confusion_matrix.py
 src/sageworks/web_components/data_source_details.py
 src/sageworks/web_components/feature_details.py
 src/sageworks/web_components/feature_importance.py
+src/sageworks/web_components/feature_set_details.py
 src/sageworks/web_components/histogram.py
 src/sageworks/web_components/line_chart.py
 src/sageworks/web_components/model_data.py
 src/sageworks/web_components/model_details.py
 src/sageworks/web_components/scatter_plot.py
 src/sageworks/web_components/table.py
 src/sageworks/web_components/violin_plot.py
```

### Comparing `sageworks-0.1.5.1/tests/artifacts/data_source_tests.py` & `sageworks-0.1.5.2/tests/artifacts/data_source_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/tests/artifacts/endpoint_tests.py` & `sageworks-0.1.5.2/tests/artifacts/endpoint_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/tests/artifacts/feature_set_tests.py` & `sageworks-0.1.5.2/tests/artifacts/feature_set_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/tests/artifacts/model_tests.py` & `sageworks-0.1.5.2/tests/artifacts/model_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/tests/aws_account/aws_account_clamp_tests.py` & `sageworks-0.1.5.2/tests/aws_account/aws_account_clamp_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/tests/aws_account/aws_service_broker_tests.py` & `sageworks-0.1.5.2/tests/aws_account/aws_service_broker_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/tests/create_sageworks_objs_for_tests.py` & `sageworks-0.1.5.2/tests/create_sageworks_objs_for_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/tests/transforms/data_to_data_tests.py` & `sageworks-0.1.5.2/tests/transforms/data_to_data_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/tests/transforms/data_to_features_tests.py` & `sageworks-0.1.5.2/tests/transforms/data_to_features_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/tests/transforms/features_to_model_tests.py` & `sageworks-0.1.5.2/tests/transforms/features_to_model_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/tests/transforms/model_to_endpoint_tests.py` & `sageworks-0.1.5.2/tests/transforms/model_to_endpoint_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/tests/transforms/pandas_to_data_tests.py` & `sageworks-0.1.5.2/tests/transforms/pandas_to_data_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.1/tox.ini` & `sageworks-0.1.5.2/tox.ini`

 * *Files identical despite different names*

