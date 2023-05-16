# Comparing `tmp/Accuinsight-3.4.230426rc0.tar.gz` & `tmp/Accuinsight-3.4.230516rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Accuinsight-3.4.230426rc0.tar", last modified: Wed Apr 26 04:11:20 2023, max compression
+gzip compressed data, was "Accuinsight-3.4.230516rc1.tar", last modified: Tue May 16 00:46:37 2023, max compression
```

## Comparing `Accuinsight-3.4.230426rc0.tar` & `Accuinsight-3.4.230516rc1.tar`

### file list

```diff
@@ -1,129 +1,132 @@
-drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-04-26 04:11:20.548590 Accuinsight-3.4.230426rc0/
-drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-04-26 04:11:20.352481 Accuinsight-3.4.230426rc0/Accuinsight/
-drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-04-26 04:11:20.364723 Accuinsight-3.4.230426rc0/Accuinsight/Lifecycle/
--rw-r--r--   0 a10894     (501) staff       (20)    16026 2023-04-06 06:12:04.000000 Accuinsight-3.4.230426rc0/Accuinsight/Lifecycle/ML.py
--rw-r--r--   0 a10894     (501) staff       (20)        0 2023-03-14 00:39:55.000000 Accuinsight-3.4.230426rc0/Accuinsight/Lifecycle/__init__.py
--rw-r--r--   0 a10894     (501) staff       (20)    17408 2023-03-22 07:26:18.000000 Accuinsight-3.4.230426rc0/Accuinsight/Lifecycle/common.py
--rw-r--r--   0 a10894     (501) staff       (20)    19673 2023-04-06 06:12:04.000000 Accuinsight-3.4.230426rc0/Accuinsight/Lifecycle/keras.py
--rw-r--r--   0 a10894     (501) staff       (20)      983 2023-03-14 00:39:55.000000 Accuinsight-3.4.230426rc0/Accuinsight/Lifecycle/settings.py
--rw-r--r--   0 a10894     (501) staff       (20)    26272 2023-04-26 02:59:58.000000 Accuinsight-3.4.230426rc0/Accuinsight/Lifecycle/tensorflow.py
--rw-r--r--   0 a10894     (501) staff       (20)     2511 2023-04-20 04:49:40.000000 Accuinsight-3.4.230426rc0/Accuinsight/Lifecycle/utils.py
-drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-04-26 04:11:20.365904 Accuinsight-3.4.230426rc0/Accuinsight/Monitoring/
--rw-r--r--   0 a10894     (501) staff       (20)       20 2023-03-14 00:39:55.000000 Accuinsight-3.4.230426rc0/Accuinsight/Monitoring/__init__.py
-drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-04-26 04:11:20.369285 Accuinsight-3.4.230426rc0/Accuinsight/Monitoring/deploy/
--rw-r--r--   0 a10894     (501) staff       (20)      101 2023-03-14 00:39:55.000000 Accuinsight-3.4.230426rc0/Accuinsight/Monitoring/deploy/__init__.py
--rw-r--r--   0 a10894     (501) staff       (20)     3987 2023-03-14 00:39:55.000000 Accuinsight-3.4.230426rc0/Accuinsight/Monitoring/deploy/monitoring_deploy.py
-drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-04-26 04:11:20.374100 Accuinsight-3.4.230426rc0/Accuinsight/WorkspaceRun/
--rw-r--r--   0 a10894     (501) staff       (20)       92 2023-03-14 00:39:55.000000 Accuinsight-3.4.230426rc0/Accuinsight/WorkspaceRun/__init__.py
--rw-r--r--   0 a10894     (501) staff       (20)     3657 2023-04-13 04:31:54.000000 Accuinsight-3.4.230426rc0/Accuinsight/WorkspaceRun/workspace_run.py
--rw-r--r--   0 a10894     (501) staff       (20)      178 2023-04-26 04:11:05.000000 Accuinsight-3.4.230426rc0/Accuinsight/__about__.py
--rw-r--r--   0 a10894     (501) staff       (20)      353 2023-03-14 00:39:55.000000 Accuinsight-3.4.230426rc0/Accuinsight/__init__.py
--rw-r--r--   0 a10894     (501) staff       (20)     3042 2023-03-14 00:39:55.000000 Accuinsight-3.4.230426rc0/Accuinsight/exceptions.py
--rw-r--r--   0 a10894     (501) staff       (20)      205 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/info.py
-drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-04-26 04:11:20.378753 Accuinsight-3.4.230426rc0/Accuinsight/modeler/
--rw-r--r--   0 a10894     (501) staff       (20)        0 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/__init__.py
-drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-04-26 04:11:20.382163 Accuinsight-3.4.230426rc0/Accuinsight/modeler/clients/
--rw-r--r--   0 a10894     (501) staff       (20)        0 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/clients/__init__.py
--rw-r--r--   0 a10894     (501) staff       (20)     2053 2023-04-17 02:18:35.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/clients/modeler_api.py
-drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-04-26 04:11:20.405693 Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/
-drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-04-26 04:11:20.408902 Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/LcConst/
--rw-r--r--   0 a10894     (501) staff       (20)     2564 2023-04-18 05:13:02.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/LcConst/LcConst.py
--rw-r--r--   0 a10894     (501) staff       (20)       27 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/LcConst/__init__.py
--rw-r--r--   0 a10894     (501) staff       (20)      460 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/Lifecycle.py
--rw-r--r--   0 a10894     (501) staff       (20)      730 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/ModelType.py
-drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-04-26 04:11:20.410180 Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/MonitoringConst/
--rw-r--r--   0 a10894     (501) staff       (20)        0 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/MonitoringConst/__init__.py
-drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-04-26 04:11:20.412362 Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/MonitoringConst/deploy/
--rw-r--r--   0 a10894     (501) staff       (20)      219 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/MonitoringConst/deploy/DeployConst.py
--rw-r--r--   0 a10894     (501) staff       (20)       31 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/MonitoringConst/deploy/__init__.py
-drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-04-26 04:11:20.414529 Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/Run/
-drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-04-26 04:11:20.446550 Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/Run/ParseRun/
--rw-r--r--   0 a10894     (501) staff       (20)     2894 2023-04-18 05:20:36.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/Run/ParseRun/BaseParser.py
--rw-r--r--   0 a10894     (501) staff       (20)     2387 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/Run/ParseRun/ParseExperiment.py
--rw-r--r--   0 a10894     (501) staff       (20)     3556 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/Run/ParseRun/ParseKeras.py
--rw-r--r--   0 a10894     (501) staff       (20)     6127 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/Run/ParseRun/Parse_DLClassification.py
--rw-r--r--   0 a10894     (501) staff       (20)     6000 2023-04-18 07:30:03.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/Run/ParseRun/Parse_DLClassification_evl.py
--rw-r--r--   0 a10894     (501) staff       (20)     6899 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/Run/ParseRun/Parse_DLRegression.py
--rw-r--r--   0 a10894     (501) staff       (20)      381 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/Run/ParseRun/Parse_Helper.py
--rw-r--r--   0 a10894     (501) staff       (20)     4071 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/Run/ParseRun/Parse_MLClassifier.py
--rw-r--r--   0 a10894     (501) staff       (20)     6902 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/Run/ParseRun/Parse_MLRegression.py
--rw-r--r--   0 a10894     (501) staff       (20)     4642 2023-04-25 08:27:25.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/Run/ParseRun/ParserVisualJaon.py
--rw-r--r--   0 a10894     (501) staff       (20)       30 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/Run/ParseRun/__init__.py
-drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-04-26 04:11:20.458101 Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/Run/RunInfo/
--rw-r--r--   0 a10894     (501) staff       (20)    12016 2023-04-25 08:27:25.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/Run/RunInfo/RunInfo.py
--rw-r--r--   0 a10894     (501) staff       (20)       26 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/Run/RunInfo/__init__.py
--rw-r--r--   0 a10894     (501) staff       (20)     1615 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/Run/RunOjbject.py
--rw-r--r--   0 a10894     (501) staff       (20)        0 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/Run/__init__.py
--rw-r--r--   0 a10894     (501) staff       (20)        0 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/__init__.py
--rw-r--r--   0 a10894     (501) staff       (20)     1878 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/feature_contribution.py
--rw-r--r--   0 a10894     (501) staff       (20)      311 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/func.py
--rw-r--r--   0 a10894     (501) staff       (20)     6753 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/func_for_visual.py
--rw-r--r--   0 a10894     (501) staff       (20)     5931 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/get.py
--rw-r--r--   0 a10894     (501) staff       (20)     7545 2023-04-20 06:14:10.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/get_for_visual.py
--rw-r--r--   0 a10894     (501) staff       (20)      823 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/lossFuncInfo.py
--rw-r--r--   0 a10894     (501) staff       (20)     1144 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/metricsLightgbm.py
--rw-r--r--   0 a10894     (501) staff       (20)     1566 2023-04-20 06:00:29.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/modelEvaluation.py
--rw-r--r--   0 a10894     (501) staff       (20)     8299 2023-04-11 06:50:31.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/path.py
--rw-r--r--   0 a10894     (501) staff       (20)      361 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/sklearnModelType.py
-drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-04-26 04:11:20.501379 Accuinsight-3.4.230426rc0/Accuinsight/modeler/entities/
--rw-r--r--   0 a10894     (501) staff       (20)      500 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/entities/__init__.py
--rw-r--r--   0 a10894     (501) staff       (20)     1491 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/entities/_modeler_object.py
--rw-r--r--   0 a10894     (501) staff       (20)     1278 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/entities/alarm.py
--rw-r--r--   0 a10894     (501) staff       (20)      803 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/entities/lc_artifact.py
--rw-r--r--   0 a10894     (501) staff       (20)     1204 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/entities/lc_metric.py
--rw-r--r--   0 a10894     (501) staff       (20)      970 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/entities/lc_param.py
--rw-r--r--   0 a10894     (501) staff       (20)      624 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/entities/lc_run.py
--rw-r--r--   0 a10894     (501) staff       (20)     5712 2023-04-17 02:35:03.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/entities/lc_run_info.py
--rw-r--r--   0 a10894     (501) staff       (20)     1506 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/entities/lc_run_status.py
--rw-r--r--   0 a10894     (501) staff       (20)      918 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/entities/lc_run_tag.py
--rw-r--r--   0 a10894     (501) staff       (20)     1287 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/entities/lc_stage.py
--rw-r--r--   0 a10894     (501) staff       (20)     1836 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/entities/lc_view_type.py
--rw-r--r--   0 a10894     (501) staff       (20)     3638 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/entities/monitoring_deploy_log.py
--rw-r--r--   0 a10894     (501) staff       (20)     1286 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/entities/workspace_run_log.py
--rw-r--r--   0 a10894     (501) staff       (20)     3050 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/exceptions.py
--rw-r--r--   0 a10894     (501) staff       (20)      205 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/info.py
-drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-04-26 04:11:20.509055 Accuinsight-3.4.230426rc0/Accuinsight/modeler/protos/
--rw-r--r--   0 a10894     (501) staff       (20)        0 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/protos/__init__.py
--rw-r--r--   0 a10894     (501) staff       (20)    37721 2023-04-25 08:22:55.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/protos/life_cycle_pb2.py
--rw-r--r--   0 a10894     (501) staff       (20)   107276 2023-04-25 08:22:55.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/protos/service_pb2.py
--rw-r--r--   0 a10894     (501) staff       (20)    27025 2023-04-25 08:22:55.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/protos/skapi_pb2.py
-drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-04-26 04:11:20.515873 Accuinsight-3.4.230426rc0/Accuinsight/modeler/protos_bak/
--rw-r--r--   0 a10894     (501) staff       (20)        0 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/protos_bak/__init__.py
--rw-r--r--   0 a10894     (501) staff       (20)    36510 2023-03-16 01:29:02.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/protos_bak/life_cycle_pb2.py
--rw-r--r--   0 a10894     (501) staff       (20)   107276 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/protos_bak/service_pb2.py
--rw-r--r--   0 a10894     (501) staff       (20)    27025 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/protos_bak/skapi_pb2.py
-drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-04-26 04:11:20.518031 Accuinsight-3.4.230426rc0/Accuinsight/modeler/store/
--rw-r--r--   0 a10894     (501) staff       (20)        0 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/store/__init__.py
-drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-04-26 04:11:20.527634 Accuinsight-3.4.230426rc0/Accuinsight/modeler/store/tracking/
--rw-r--r--   0 a10894     (501) staff       (20)      315 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/store/tracking/__init__.py
--rw-r--r--   0 a10894     (501) staff       (20)      957 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/store/tracking/lc_abstract_store.py
--rw-r--r--   0 a10894     (501) staff       (20)     6982 2023-04-25 08:29:18.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/store/tracking/life_cycle_store.py
--rw-r--r--   0 a10894     (501) staff       (20)     1789 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/store/tracking/monitoring_deploy_store.py
--rw-r--r--   0 a10894     (501) staff       (20)     1416 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/store/tracking/workspace_store.py
-drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-04-26 04:11:20.542470 Accuinsight-3.4.230426rc0/Accuinsight/modeler/utils/
--rw-r--r--   0 a10894     (501) staff       (20)     1619 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/utils/__init__.py
--rw-r--r--   0 a10894     (501) staff       (20)      365 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/utils/annotations.py
-drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-04-26 04:11:20.547516 Accuinsight-3.4.230426rc0/Accuinsight/modeler/utils/dependency/
--rw-r--r--   0 a10894     (501) staff       (20)        0 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/utils/dependency/__init__.py
--rw-r--r--   0 a10894     (501) staff       (20)    19325 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/utils/dependency/dependencies.py
--rw-r--r--   0 a10894     (501) staff       (20)     2209 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/utils/dependency/settings.py
--rw-r--r--   0 a10894     (501) staff       (20)     1202 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/utils/dl_utils.py
--rwxr-xr-x   0 a10894     (501) staff       (20)     4122 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/utils/os_getenv.py
--rw-r--r--   0 a10894     (501) staff       (20)     1175 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/utils/proto_json_utils.py
--rwxr-xr-x   0 a10894     (501) staff       (20)    11063 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/utils/rest_utils.py
--rw-r--r--   0 a10894     (501) staff       (20)     2433 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/utils/runs_utils.py
--rw-r--r--   0 a10894     (501) staff       (20)      367 2023-03-22 07:23:16.000000 Accuinsight-3.4.230426rc0/Accuinsight/modeler/utils/string_utils.py
-drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-04-26 04:11:20.357022 Accuinsight-3.4.230426rc0/Accuinsight.egg-info/
--rw-r--r--   0 a10894     (501) staff       (20)     2269 2023-04-26 04:11:20.000000 Accuinsight-3.4.230426rc0/Accuinsight.egg-info/PKG-INFO
--rw-r--r--   0 a10894     (501) staff       (20)     4336 2023-04-26 04:11:20.000000 Accuinsight-3.4.230426rc0/Accuinsight.egg-info/SOURCES.txt
--rw-r--r--   0 a10894     (501) staff       (20)        1 2023-04-26 04:11:20.000000 Accuinsight-3.4.230426rc0/Accuinsight.egg-info/dependency_links.txt
--rw-r--r--   0 a10894     (501) staff       (20)        1 2023-04-26 04:11:20.000000 Accuinsight-3.4.230426rc0/Accuinsight.egg-info/not-zip-safe
--rw-r--r--   0 a10894     (501) staff       (20)      281 2023-04-26 04:11:20.000000 Accuinsight-3.4.230426rc0/Accuinsight.egg-info/requires.txt
--rw-r--r--   0 a10894     (501) staff       (20)       12 2023-04-26 04:11:20.000000 Accuinsight-3.4.230426rc0/Accuinsight.egg-info/top_level.txt
--rw-r--r--   0 a10894     (501) staff       (20)       21 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/LICENSE.txt
--rw-r--r--   0 a10894     (501) staff       (20)       63 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/MANIFEST.in
--rw-r--r--   0 a10894     (501) staff       (20)     2269 2023-04-26 04:11:20.548826 Accuinsight-3.4.230426rc0/PKG-INFO
--rw-r--r--   0 a10894     (501) staff       (20)     1487 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/README.rst
--rw-r--r--   0 a10894     (501) staff       (20)      280 2023-03-14 00:39:56.000000 Accuinsight-3.4.230426rc0/requirements.txt
--rw-r--r--   0 a10894     (501) staff       (20)      256 2023-04-26 04:11:20.549953 Accuinsight-3.4.230426rc0/setup.cfg
--rw-r--r--   0 a10894     (501) staff       (20)     1294 2023-03-14 00:40:01.000000 Accuinsight-3.4.230426rc0/setup.py
+drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-16 00:46:37.602403 Accuinsight-3.4.230516rc1/
+drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-16 00:46:37.155850 Accuinsight-3.4.230516rc1/Accuinsight/
+drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-16 00:46:37.201678 Accuinsight-3.4.230516rc1/Accuinsight/Lifecycle/
+-rw-r--r--   0 a10894     (501) staff       (20)    23813 2023-05-10 02:33:36.000000 Accuinsight-3.4.230516rc1/Accuinsight/Lifecycle/ML.py
+-rw-r--r--   0 a10894     (501) staff       (20)        0 2023-03-14 00:39:55.000000 Accuinsight-3.4.230516rc1/Accuinsight/Lifecycle/__init__.py
+-rw-r--r--   0 a10894     (501) staff       (20)    17408 2023-03-22 07:26:18.000000 Accuinsight-3.4.230516rc1/Accuinsight/Lifecycle/common.py
+-rw-r--r--   0 a10894     (501) staff       (20)    26875 2023-05-10 05:06:10.000000 Accuinsight-3.4.230516rc1/Accuinsight/Lifecycle/keras.py
+-rw-r--r--   0 a10894     (501) staff       (20)      983 2023-03-14 00:39:55.000000 Accuinsight-3.4.230516rc1/Accuinsight/Lifecycle/settings.py
+-rw-r--r--   0 a10894     (501) staff       (20)    26656 2023-05-10 05:06:10.000000 Accuinsight-3.4.230516rc1/Accuinsight/Lifecycle/tensorflow.py
+-rw-r--r--   0 a10894     (501) staff       (20)     2795 2023-05-10 05:06:10.000000 Accuinsight-3.4.230516rc1/Accuinsight/Lifecycle/utils.py
+drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-16 00:46:37.203496 Accuinsight-3.4.230516rc1/Accuinsight/Monitoring/
+-rw-r--r--   0 a10894     (501) staff       (20)       20 2023-03-14 00:39:55.000000 Accuinsight-3.4.230516rc1/Accuinsight/Monitoring/__init__.py
+drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-16 00:46:37.207076 Accuinsight-3.4.230516rc1/Accuinsight/Monitoring/deploy/
+-rw-r--r--   0 a10894     (501) staff       (20)      101 2023-03-14 00:39:55.000000 Accuinsight-3.4.230516rc1/Accuinsight/Monitoring/deploy/__init__.py
+-rw-r--r--   0 a10894     (501) staff       (20)     3987 2023-03-14 00:39:55.000000 Accuinsight-3.4.230516rc1/Accuinsight/Monitoring/deploy/monitoring_deploy.py
+drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-16 00:46:37.211449 Accuinsight-3.4.230516rc1/Accuinsight/WorkspaceRun/
+-rw-r--r--   0 a10894     (501) staff       (20)       92 2023-03-14 00:39:55.000000 Accuinsight-3.4.230516rc1/Accuinsight/WorkspaceRun/__init__.py
+-rw-r--r--   0 a10894     (501) staff       (20)     3763 2023-05-08 04:59:50.000000 Accuinsight-3.4.230516rc1/Accuinsight/WorkspaceRun/workspace_run.py
+-rw-r--r--   0 a10894     (501) staff       (20)      178 2023-05-16 00:45:44.000000 Accuinsight-3.4.230516rc1/Accuinsight/__about__.py
+-rw-r--r--   0 a10894     (501) staff       (20)      353 2023-03-14 00:39:55.000000 Accuinsight-3.4.230516rc1/Accuinsight/__init__.py
+-rw-r--r--   0 a10894     (501) staff       (20)     3042 2023-03-14 00:39:55.000000 Accuinsight-3.4.230516rc1/Accuinsight/exceptions.py
+-rw-r--r--   0 a10894     (501) staff       (20)      205 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/info.py
+drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-16 00:46:37.243920 Accuinsight-3.4.230516rc1/Accuinsight/modeler/
+-rw-r--r--   0 a10894     (501) staff       (20)        0 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/__init__.py
+drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-16 00:46:37.250584 Accuinsight-3.4.230516rc1/Accuinsight/modeler/clients/
+-rw-r--r--   0 a10894     (501) staff       (20)        0 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/clients/__init__.py
+-rw-r--r--   0 a10894     (501) staff       (20)     2053 2023-04-17 02:18:35.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/clients/modeler_api.py
+drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-16 00:46:37.301913 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/
+drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-16 00:46:37.306946 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/LcConst/
+-rw-r--r--   0 a10894     (501) staff       (20)     2786 2023-05-10 01:48:37.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/LcConst/LcConst.py
+-rw-r--r--   0 a10894     (501) staff       (20)       27 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/LcConst/__init__.py
+-rw-r--r--   0 a10894     (501) staff       (20)      460 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Lifecycle.py
+-rw-r--r--   0 a10894     (501) staff       (20)      730 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/ModelType.py
+drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-16 00:46:37.309011 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/MonitoringConst/
+-rw-r--r--   0 a10894     (501) staff       (20)        0 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/MonitoringConst/__init__.py
+drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-16 00:46:37.313821 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/MonitoringConst/deploy/
+-rw-r--r--   0 a10894     (501) staff       (20)      219 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/MonitoringConst/deploy/DeployConst.py
+-rw-r--r--   0 a10894     (501) staff       (20)       31 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/MonitoringConst/deploy/__init__.py
+drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-16 00:46:37.336373 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/
+drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-16 00:46:37.405994 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/
+-rw-r--r--   0 a10894     (501) staff       (20)     4185 2023-05-08 05:02:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/BaseParser.py
+-rw-r--r--   0 a10894     (501) staff       (20)     2387 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/ParseExperiment.py
+-rw-r--r--   0 a10894     (501) staff       (20)     3556 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/ParseKeras.py
+-rw-r--r--   0 a10894     (501) staff       (20)     6127 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/Parse_DLClassification.py
+-rw-r--r--   0 a10894     (501) staff       (20)     3877 2023-05-10 05:06:10.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/Parse_DLClassification_evl.py
+-rw-r--r--   0 a10894     (501) staff       (20)     6899 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/Parse_DLRegression.py
+-rw-r--r--   0 a10894     (501) staff       (20)     4901 2023-05-10 05:06:10.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/Parse_DLRegression_evl.py
+-rw-r--r--   0 a10894     (501) staff       (20)      381 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/Parse_Helper.py
+-rw-r--r--   0 a10894     (501) staff       (20)     4069 2023-05-08 05:02:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/Parse_MLClassifier.py
+-rw-r--r--   0 a10894     (501) staff       (20)     2506 2023-05-10 05:06:10.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/Parse_MLClassifier_evl.py
+-rw-r--r--   0 a10894     (501) staff       (20)     6902 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/Parse_MLRegression.py
+-rw-r--r--   0 a10894     (501) staff       (20)     5146 2023-05-10 05:06:10.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/Parse_MLRegression_evl.py
+-rw-r--r--   0 a10894     (501) staff       (20)     4641 2023-04-27 02:41:11.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/ParserVisualJaon.py
+-rw-r--r--   0 a10894     (501) staff       (20)       30 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/__init__.py
+drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-16 00:46:37.410831 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/RunInfo/
+-rw-r--r--   0 a10894     (501) staff       (20)    13570 2023-05-10 05:06:10.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/RunInfo/RunInfo.py
+-rw-r--r--   0 a10894     (501) staff       (20)       26 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/RunInfo/__init__.py
+-rw-r--r--   0 a10894     (501) staff       (20)     1615 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/RunOjbject.py
+-rw-r--r--   0 a10894     (501) staff       (20)        0 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/__init__.py
+-rw-r--r--   0 a10894     (501) staff       (20)        0 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/__init__.py
+-rw-r--r--   0 a10894     (501) staff       (20)     1878 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/feature_contribution.py
+-rw-r--r--   0 a10894     (501) staff       (20)      311 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/func.py
+-rw-r--r--   0 a10894     (501) staff       (20)     6753 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/func_for_visual.py
+-rw-r--r--   0 a10894     (501) staff       (20)     5931 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/get.py
+-rw-r--r--   0 a10894     (501) staff       (20)     7618 2023-05-10 05:06:10.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/get_for_visual.py
+-rw-r--r--   0 a10894     (501) staff       (20)      823 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/lossFuncInfo.py
+-rw-r--r--   0 a10894     (501) staff       (20)     1144 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/metricsLightgbm.py
+-rw-r--r--   0 a10894     (501) staff       (20)     1884 2023-05-10 05:06:10.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/modelEvaluation.py
+-rw-r--r--   0 a10894     (501) staff       (20)     8437 2023-04-27 06:49:04.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/path.py
+-rw-r--r--   0 a10894     (501) staff       (20)      361 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/sklearnModelType.py
+drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-16 00:46:37.468671 Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/
+-rw-r--r--   0 a10894     (501) staff       (20)      500 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/__init__.py
+-rw-r--r--   0 a10894     (501) staff       (20)     1491 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/_modeler_object.py
+-rw-r--r--   0 a10894     (501) staff       (20)     1278 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/alarm.py
+-rw-r--r--   0 a10894     (501) staff       (20)      803 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/lc_artifact.py
+-rw-r--r--   0 a10894     (501) staff       (20)     1204 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/lc_metric.py
+-rw-r--r--   0 a10894     (501) staff       (20)      970 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/lc_param.py
+-rw-r--r--   0 a10894     (501) staff       (20)      624 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/lc_run.py
+-rw-r--r--   0 a10894     (501) staff       (20)     5712 2023-04-17 02:35:03.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/lc_run_info.py
+-rw-r--r--   0 a10894     (501) staff       (20)     1506 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/lc_run_status.py
+-rw-r--r--   0 a10894     (501) staff       (20)      918 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/lc_run_tag.py
+-rw-r--r--   0 a10894     (501) staff       (20)     1287 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/lc_stage.py
+-rw-r--r--   0 a10894     (501) staff       (20)     1836 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/lc_view_type.py
+-rw-r--r--   0 a10894     (501) staff       (20)     3638 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/monitoring_deploy_log.py
+-rw-r--r--   0 a10894     (501) staff       (20)     1286 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/workspace_run_log.py
+-rw-r--r--   0 a10894     (501) staff       (20)     3050 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/exceptions.py
+-rw-r--r--   0 a10894     (501) staff       (20)      205 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/info.py
+drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-16 00:46:37.505642 Accuinsight-3.4.230516rc1/Accuinsight/modeler/protos/
+-rw-r--r--   0 a10894     (501) staff       (20)        0 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/protos/__init__.py
+-rw-r--r--   0 a10894     (501) staff       (20)    37721 2023-04-25 08:22:55.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/protos/life_cycle_pb2.py
+-rw-r--r--   0 a10894     (501) staff       (20)   107276 2023-04-25 08:22:55.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/protos/service_pb2.py
+-rw-r--r--   0 a10894     (501) staff       (20)    27025 2023-04-25 08:22:55.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/protos/skapi_pb2.py
+drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-16 00:46:37.540087 Accuinsight-3.4.230516rc1/Accuinsight/modeler/protos_bak/
+-rw-r--r--   0 a10894     (501) staff       (20)        0 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/protos_bak/__init__.py
+-rw-r--r--   0 a10894     (501) staff       (20)    36510 2023-03-16 01:29:02.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/protos_bak/life_cycle_pb2.py
+-rw-r--r--   0 a10894     (501) staff       (20)   107276 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/protos_bak/service_pb2.py
+-rw-r--r--   0 a10894     (501) staff       (20)    27025 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/protos_bak/skapi_pb2.py
+drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-16 00:46:37.542016 Accuinsight-3.4.230516rc1/Accuinsight/modeler/store/
+-rw-r--r--   0 a10894     (501) staff       (20)        0 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/store/__init__.py
+drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-16 00:46:37.555128 Accuinsight-3.4.230516rc1/Accuinsight/modeler/store/tracking/
+-rw-r--r--   0 a10894     (501) staff       (20)      315 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/store/tracking/__init__.py
+-rw-r--r--   0 a10894     (501) staff       (20)      957 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/store/tracking/lc_abstract_store.py
+-rw-r--r--   0 a10894     (501) staff       (20)     6918 2023-04-27 02:45:39.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/store/tracking/life_cycle_store.py
+-rw-r--r--   0 a10894     (501) staff       (20)     1789 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/store/tracking/monitoring_deploy_store.py
+-rw-r--r--   0 a10894     (501) staff       (20)     1416 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/store/tracking/workspace_store.py
+drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-16 00:46:37.594904 Accuinsight-3.4.230516rc1/Accuinsight/modeler/utils/
+-rw-r--r--   0 a10894     (501) staff       (20)     1619 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/utils/__init__.py
+-rw-r--r--   0 a10894     (501) staff       (20)      365 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/utils/annotations.py
+drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-16 00:46:37.601029 Accuinsight-3.4.230516rc1/Accuinsight/modeler/utils/dependency/
+-rw-r--r--   0 a10894     (501) staff       (20)        0 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/utils/dependency/__init__.py
+-rw-r--r--   0 a10894     (501) staff       (20)    19325 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/utils/dependency/dependencies.py
+-rw-r--r--   0 a10894     (501) staff       (20)     2209 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/utils/dependency/settings.py
+-rw-r--r--   0 a10894     (501) staff       (20)     1202 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/utils/dl_utils.py
+-rwxr-xr-x   0 a10894     (501) staff       (20)     4122 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/utils/os_getenv.py
+-rw-r--r--   0 a10894     (501) staff       (20)     1175 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/utils/proto_json_utils.py
+-rwxr-xr-x   0 a10894     (501) staff       (20)    11063 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/utils/rest_utils.py
+-rw-r--r--   0 a10894     (501) staff       (20)     2433 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/utils/runs_utils.py
+-rw-r--r--   0 a10894     (501) staff       (20)      367 2023-03-22 07:23:16.000000 Accuinsight-3.4.230516rc1/Accuinsight/modeler/utils/string_utils.py
+drwxr-xr-x   0 a10894     (501) staff       (20)        0 2023-05-16 00:46:37.169055 Accuinsight-3.4.230516rc1/Accuinsight.egg-info/
+-rw-r--r--   0 a10894     (501) staff       (20)     2269 2023-05-16 00:46:36.000000 Accuinsight-3.4.230516rc1/Accuinsight.egg-info/PKG-INFO
+-rw-r--r--   0 a10894     (501) staff       (20)     4528 2023-05-16 00:46:36.000000 Accuinsight-3.4.230516rc1/Accuinsight.egg-info/SOURCES.txt
+-rw-r--r--   0 a10894     (501) staff       (20)        1 2023-05-16 00:46:36.000000 Accuinsight-3.4.230516rc1/Accuinsight.egg-info/dependency_links.txt
+-rw-r--r--   0 a10894     (501) staff       (20)        1 2023-05-16 00:46:36.000000 Accuinsight-3.4.230516rc1/Accuinsight.egg-info/not-zip-safe
+-rw-r--r--   0 a10894     (501) staff       (20)      281 2023-05-16 00:46:36.000000 Accuinsight-3.4.230516rc1/Accuinsight.egg-info/requires.txt
+-rw-r--r--   0 a10894     (501) staff       (20)       12 2023-05-16 00:46:36.000000 Accuinsight-3.4.230516rc1/Accuinsight.egg-info/top_level.txt
+-rw-r--r--   0 a10894     (501) staff       (20)       21 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/LICENSE.txt
+-rw-r--r--   0 a10894     (501) staff       (20)       63 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/MANIFEST.in
+-rw-r--r--   0 a10894     (501) staff       (20)     2269 2023-05-16 00:46:37.602673 Accuinsight-3.4.230516rc1/PKG-INFO
+-rw-r--r--   0 a10894     (501) staff       (20)     1487 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/README.rst
+-rw-r--r--   0 a10894     (501) staff       (20)      280 2023-03-14 00:39:56.000000 Accuinsight-3.4.230516rc1/requirements.txt
+-rw-r--r--   0 a10894     (501) staff       (20)      256 2023-05-16 00:46:37.604569 Accuinsight-3.4.230516rc1/setup.cfg
+-rw-r--r--   0 a10894     (501) staff       (20)     1294 2023-03-14 00:40:01.000000 Accuinsight-3.4.230516rc1/setup.py
```

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/Lifecycle/ML.py` & `Accuinsight-3.4.230516rc1/Accuinsight/Lifecycle/common.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,360 +1,411 @@
-import inspect
+import os
+import shutil
+import sys
 import json
-from collections import OrderedDict
-import warnings
 import logging
-from joblib import dump
-from sklearn import pipeline
+import time
+import datetime
+from collections import OrderedDict
+from pathlib import Path
 
-from Accuinsight.modeler.core import func, path, get
-from Accuinsight.modeler.core.func import get_time
-from Accuinsight.modeler.core.get_for_visual import roc_pr_curve, get_true_y, get_visual_info_regressor
-from Accuinsight.modeler.core.sklearnModelType import REGRESSION, CLASSIFICATION
-from Accuinsight.modeler.core.LcConst.LcConst import ALL_MODEL_PARAMS, SELECTED_PARAMS, SELECTED_METRICS, VALUE_ERROR, \
-    LOGGING_TIME, LOGGING_RUN_ID, FITTED_MODEL, USER_ID, RUN_OBJ_NAME, RUN_MODEL_JSON_PATH, RUN_MODEL_VISUAL_JSON_PATH, \
-    RUN_MODEL_SHAP_JSON_PATH, RUN_MODEL_JOBLIB_PATH
-from Accuinsight.modeler.core.Run.RunInfo.RunInfo import set_current_runs, clear_runs, \
-    set_git_meta, set_python_dependencies, set_run_name, set_model_json_path, set_visual_json_path, set_model_file_path, \
-    set_prefix_path, set_best_model_joblib_path, _set_result_path, set_shap_json_path
-from Accuinsight.modeler.utils.dependency.dependencies import gather_sources_and_dependencies
+import boto3
+import joblib
+from hdfs3 import HDFileSystem
+
+from Accuinsight.Lifecycle.utils import load_model
 from Accuinsight.modeler.core.LcConst import LcConst
-from Accuinsight.modeler.utils.os_getenv import is_in_ipython, get_current_notebook, get_os_env
-from Accuinsight.modeler.clients.modeler_api import LifecycleRestApi
+from Accuinsight.modeler.core.LcConst.LcConst import ENV_JUPYTER_HOME_DIR
+from Accuinsight.modeler.utils.runs_utils import ProgressPercentage
+from Accuinsight.modeler.clients.modeler_api import WorkspaceRestApi
+from Accuinsight.modeler.utils.os_getenv import get_os_env, get_current_notebook
+from Accuinsight.modeler.entities.alarm import Alarm
 
-from Accuinsight.modeler.core.feature_contribution import shap_value
-from Accuinsight.modeler.core import metricsLightgbm
-from Accuinsight.Lifecycle.common import Common
+class Common(object):
+    def __init__(self):
+        env_value = get_os_env('ENV')
 
-logging.basicConfig(level=logging.INFO,
-                    format='%(message)s')
+        self.StorageInfo = None
+        self.target_name = None
+        self.save_path = None
+        self.endpoint = None
+        self.thresholds = None
+        self.hook_url = None
+        self.message = None
+        self.feature_name = None
+        self.data = None
+        self.user_id = None
+        self.storage_info_from_set = OrderedDict()
+        self.workspace_alarm_api = WorkspaceRestApi(env_value[LcConst.BACK_END_API_URL],
+                                                    env_value[LcConst.BACK_END_API_PORT],
+                                                    env_value[LcConst.BACK_END_API_URI])
+        self.workspace_alarm = Alarm()
+
+        self.notebook_info = get_current_notebook()
+        self.default_run_nick_name = Path(self.notebook_info).stem
+    def set_storage(self,
+                    access_key=None,  # aws-s3
+                    secret_key=None,  # aws-s3
+                    region=None,  # aws-s3
+                    bucket_name=None,  # aws-s3
+                    endpoint_url=None,  # none aws-s3
+                    hdfs_uri=None,  # pipeline-hdfs
+                    file_path=None,  # common
+                    target=None,  # common
+                    save_json=False,  # common - if it is TRUE, saving a storage information as a json file.
+                    save_path=None  # common - if save_path is not None, the json file is saved in this path.
+                    ):
+
+        if target is None:
+            raise ValueError('target을 입력해주시기 바랍니다.')
+
+        ## make a directory for saving json file
+        save_prefix = None
+        if save_json:
+            save_prefix_run = os.path.join(ENV_JUPYTER_HOME_DIR, 'runs')
+            if not os.path.isdir(save_prefix_run):
+                try:
+                    os.mkdir(save_prefix_run)
+                except:
+                    pass
+            save_prefix = os.path.join(save_prefix_run, 'storage-info-json')
+            if not os.path.isdir(save_prefix):
+                try:
+                    os.mkdir(save_prefix)
+                except:
+                    pass
+
+        ### HDFS
+        if hdfs_uri is not None:
+            storage_type = 'hdfs'
+
+            split_1 = hdfs_uri.split('//')[1].split('/')
+            split_2 = [i.split(':') for i in split_1 if ':' in i][0]
+
+            self.storage_info_from_set['host'] = split_2[0]
+            self.storage_info_from_set['port'] = split_2[1]
+            self.storage_info_from_set['filePath'] = os.path.join('/', *split_1[1:])
+            self.storage_info_from_set['target'] = target
+
+        ### S3
+        elif bucket_name is not None:
+            ### AWS - S3
+            if endpoint_url is None:
+                storage_type = 's3'
+                self.storage_info_from_set['myAccessKey'] = access_key
+                self.storage_info_from_set['mySecretKey'] = secret_key
+                self.storage_info_from_set['endpoint'] = 's3.' + region + '.amazonaws.com'
+                self.storage_info_from_set['region'] = region
+                self.storage_info_from_set['bucketType'] = 's3'
+                self.storage_info_from_set['bucketName'] = bucket_name
+                self.storage_info_from_set['filePath'] = file_path
+                self.storage_info_from_set['fileName'] = file_path.split('/')[-1]
+                self.storage_info_from_set['target'] = target
 
-warnings.filterwarnings("ignore")
+            ### other - S3
+            else:
+                storage_type = 's3'
+                self.storage_info_from_set['myAccessKey'] = access_key
+                self.storage_info_from_set['mySecretKey'] = secret_key
+                self.storage_info_from_set['endpointUrl'] = endpoint_url
+                self.storage_info_from_set['region'] = region
+                self.storage_info_from_set['bucketType'] = 's3'
+                self.storage_info_from_set['bucketName'] = bucket_name
+                self.storage_info_from_set['filePath'] = file_path
+                self.storage_info_from_set['fileName'] = file_path.split('/')[-1]
+                self.storage_info_from_set['target'] = target
 
+        ### Local
+        else:
+            storage_type = 'local'
+            self.storage_info_from_set['filePath'] = file_path
+            self.storage_info_from_set['fileName'] = file_path.split('/')[-1]
+            self.storage_info_from_set['target'] = target
+
+            self.save_path = file_path
+            self.StorageInfo = self.storage_info_from_set
+            self.target_name = target
+
+        # save_json 만 True로 하고 사용자가 파라미터로 save_path를 입력하지 않을 경우
+        if save_json:
+            if save_path is None:
+                timestamp = str(datetime.datetime.now().date()).replace('-', '')
+                dir_list = os.listdir(save_prefix)
+                num = len([True for i in dir_list if timestamp in i])
+                save_path = timestamp + '-' + str(num + 1).zfill(2) + '-' + storage_type + '-connection-info' + '.json'
 
-class accuinsight(Common):
-    def __init__(self):
-        global feature_name, alarm, alarm_api, message_param, user_id, notebook_info, run_meta, run_nick_name
-        super().__init__()
+            else:  # save_path is not None
+                pass
 
-        feature_name = None
-        user_id = None
-        message_param = ''
-
-        alarm = self.workspace_alarm
-        alarm_api = self.workspace_alarm_api
-        notebook_info = self.notebook_info
-        run_nick_name = self.default_run_nick_name
+            storage_info_full_path = os.path.join(save_prefix, save_path)
+            with open(storage_info_full_path, 'w', encoding='utf-8') as save_file:
+                json.dump(self.storage_info_from_set, save_file, indent='\t')
 
-        run_meta = None
+        if not save_json and save_path is not None:
+            raise ValueError("'save_json=True'로 설정하시기 바랍니다.")
 
     def get_file(self, storage_json_file_name=None):
-        global save_path, StorageInfo, target_name
-        save_path, StorageInfo, target_name = super().get_file(storage_json_file_name)
+        if storage_json_file_name is not None:
 
-    def set_features(self, feature_names):
-        global feature_name
-        feature_name = super().set_features(feature_names)
+            # meta file 저장하는 폴더 만들면, 이 경로는 수정돼야 함.
+            storage_info_json_path = os.path.join(ENV_JUPYTER_HOME_DIR, storage_json_file_name)
+
+            with open(storage_info_json_path) as jsonFile:
+                self.StorageInfo = json.load(jsonFile)
+
+        else:  # storage_json_file_name == None, when using set_storage() method.
+            self.StorageInfo = self.storage_info_from_set
+
+        ## define the target name
+        self.target_name = self.StorageInfo['target']
+
+        ### HDFS
+        if 'host' in self.StorageInfo.keys():
+
+            ## path for saving data
+            save_dir = os.path.join(ENV_JUPYTER_HOME_DIR, 'data_from_hdfs')
+            if not os.path.exists(save_dir):
+                os.mkdir(save_dir)
+            else:
+                pass
+
+            split_list = list(filter(None, self.StorageInfo['filePath'].split('/')))
+
+            HOST = self.StorageInfo['host']
+            PORT = int(self.StorageInfo['port'])
+            FILE_PATH = self.StorageInfo['filePath']
+            FILE_DIR = '/'
+            for i in split_list[:len(split_list) - 1]:
+                FILE_DIR = os.path.join(FILE_DIR, i)
+            FILE_NAME = split_list[-1]
+
+            save_file_name = FILE_NAME.split('.')[0] + '_' + str(datetime.datetime.now().date()).replace('-', '') + '.'\
+                             + FILE_NAME.split('.')[1]
+            self.save_path = os.path.join(save_dir, save_file_name)
+            self.endpoint = os.path.join('hdfs://', HOST, self.StorageInfo['port']) + FILE_PATH
+
+            hdfs = HDFileSystem(host=HOST, port=PORT)
+            hdfs.ls(FILE_DIR)
+
+            sys.stdout.write('%s %s %s' % ('Downloading file...', FILE_NAME, '\n'))
+            time.sleep(1)
+            hdfs.get(FILE_PATH, self.save_path)
+            logging.info(self.save_path)
+
+        ### AWS-S3
+        elif 'bucketName' in self.StorageInfo.keys():
+            if not 'endpointUrl' in self.StorageInfo.keys():
+                BUCKET_TYPE = self.StorageInfo['bucketType']
+                BUCKET_NAME = self.StorageInfo['bucketName']
+                FILE_PATH = self.StorageInfo['filePath']
+                FILE_NAME = self.StorageInfo['fileName']
+                # FILE_TYPE = self.StorageInfo['fileType']
+                # FILE_DELIM = self.StorageInfo['fileDelim']
+                ACCESS_KEY = self.StorageInfo['myAccessKey']
+                SECRET_KEY = self.StorageInfo['mySecretKey']
+                REGION = self.StorageInfo['region']
+                URL = self.StorageInfo['endpoint']
+                ## path for saving data
+                save_dir = os.path.join(ENV_JUPYTER_HOME_DIR, 'data_from_aws')
+                if not os.path.exists(save_dir):
+                    os.mkdir(save_dir)
+                else:
+                    pass
+
+                save_file_name = FILE_NAME.split('.')[0] + '_' + str(datetime.datetime.now().date()).replace('-', '') \
+                                 + '.' + FILE_NAME.split('.')[1]
+                self.save_path = os.path.join(save_dir, save_file_name)
+
+                # endpoint
+                pre_url = 'https://' + BUCKET_NAME + '.' + URL
+                self.endpoint = os.path.join(pre_url, FILE_PATH)
+
+                client = boto3.client(BUCKET_TYPE,
+                                      aws_access_key_id=ACCESS_KEY,
+                                      aws_secret_access_key=SECRET_KEY,
+                                      region_name=REGION)
+
+                transfer = boto3.s3.transfer.S3Transfer(client)
+
+                progress = ProgressPercentage(client, BUCKET_NAME, FILE_PATH)
+
+                sys.stdout.write('%s %s %s' % ('Downloading file...', FILE_NAME, '\n'))
+                transfer.download_file(BUCKET_NAME, FILE_PATH, self.save_path, callback=progress)
+                logging.info(self.save_path)
+
+            else:
+                BUCKET_TYPE = self.StorageInfo['bucketType']
+                BUCKET_NAME = self.StorageInfo['bucketName']
+                FILE_PATH = self.StorageInfo['filePath']
+                FILE_NAME = self.StorageInfo['fileName']
+                ACCESS_KEY = self.StorageInfo['myAccessKey']
+                SECRET_KEY = self.StorageInfo['mySecretKey']
+                REGION = self.StorageInfo['region']
+                ENDPOINT_URL = self.StorageInfo['endpointUrl']
+                ## path for saving data
+                save_dir = os.path.join(ENV_JUPYTER_HOME_DIR, 'data_from_other')
+                if not os.path.exists(save_dir):
+                    os.mkdir(save_dir)
+                else:
+                    pass
+
+                save_file_name = FILE_NAME.split('.')[0] + '_' + str(datetime.datetime.now().date()).replace('-', '')\
+                                      + '.' + FILE_NAME.split('.')[1]
+                self.save_path = os.path.join(save_dir, save_file_name)
+
+                # endpoint
+                client = boto3.client(BUCKET_TYPE,
+                                      aws_access_key_id=ACCESS_KEY,
+                                      aws_secret_access_key=SECRET_KEY,
+                                      region_name=REGION,
+                                      endpoint_url=ENDPOINT_URL)
+
+                transfer = boto3.s3.transfer.S3Transfer(client)
+
+                progress = ProgressPercentage(client, BUCKET_NAME, FILE_PATH)
+
+                sys.stdout.write('%s %s %s' % ('Downloading file...', FILE_NAME, '\n'))
+                transfer.download_file(BUCKET_NAME, FILE_PATH, self.save_path, callback=progress)
+                logging.info(self.save_path)
+
+        ### Local
+        else:
+            self.save_path = self.StorageInfo['filePath']
+
+        return self.save_path, self.StorageInfo, self.target_name
+
+    def set_data(self, data=None):
+        if data is not None:
+            self.data = data
+
+    def unset_data(self):
+        self.data = None
+
+    @staticmethod
+    def _send_message(metric=None, current_value=None, message=None, thresholds=None, alarm_object=None, alarm_api=None):
+        if alarm_object:
+            messages = list()
+
+            if thresholds:
+                if current_value >= thresholds:
+                    messages.append('[모델 학습 완료] ' + metric + '이 설정하신 thresolds: ' + str(thresholds) + '를 초과하였습니다.')
+
+            if message:
+                if isinstance(message, str):
+                    messages.append(message)
+                elif isinstance(message, list):
+                    messages.extend(message)
+                else:
+                    raise ValueError("Wrong message input detected. Available type is 'str' and 'list'")
+
+            if messages:
+                for message in messages:
+                    alarm_object.message = message
+                    alarm_object.type = "Workspace"
+                    alarm_api.call_rest_api(alarm_object.get_alarm_param(), "alarm")
 
     def set_slack(self, hook_url=None):
-        alarm.notifiers['slack'] = hook_url
+        if hook_url:
+            self.workspace_alarm.notifiers['slack'] = hook_url
 
     def unset_slack(self):
-        if 'slack' in alarm.notifiers.keys():
-            del alarm.notifiers['slack']
+        if 'slack' in self.workspace_alarm.notifiers.keys():
+            del self.workspace_alarm.notifiers['slack']
 
     def set_mail(self, address=None):
-        alarm.notifiers['mail'] = address
+        if address:
+            self.workspace_alarm.notifiers['mail'] = address
 
     def unset_mail(self):
-        if 'mail' in alarm.notifiers.keys():
-            del alarm.notifiers['mail']
+        if 'mail' in self.workspace_alarm.notifiers.keys():
+            del self.workspace_alarm.notifiers['mail']
 
     def send_message(self, message=None, thresholds=None):
-        global message_param
-
-        if thresholds:
-            raise ValueError("ML 모델의 경우 'thresholds'를 사용한 alarm 기능을 사용할 수 없습니다. message 인수를 사용해 주세요.")
+        if message and thresholds:
+            raise ValueError("'message'와 'thresholds' 두 개의 arguments를 동시에 입력할 수 없습니다.")
         else:
-            message_param = message
+            self.message = message
+            self.thresholds = thresholds
 
     def unset_message(self):
-        global message_param
-        message_param = ''
+        self.message = None
+        self.thresholds = None
 
-    def set_user_id(self, uid):
-        global user_id
-        user_id = uid
+    def set_user_id(self, user_id):
+        self.user_id = user_id
 
     def unset_user_id(self):
-        global user_id
-        user_id = None
+        self.user_id = None
 
-    def set_current_notebook(self):
-        global notebook_info
-        notebook_info = get_current_notebook()
+    def set_features(self, feature_names):
+        if str(type(feature_names)) == "<class 'list'>":
+            self.feature_name = feature_names
+        else:
+            try:
+                self.feature_name = feature_names.tolist()
+            except:
+                pass
 
-    @staticmethod
-    def get_current_run_meta():
-        global run_meta
-        return run_meta
-
-    def get_current_run_id(self):
-        try:
-            return self.get_current_run_meta()[RUN_OBJ_NAME]
-        except TypeError or KeyError:
-            return None
-
-    class add_experiment(object):
-        def __init__(self, model_name, *args, model_monitor=False, runtime=False, f1_average_in='weighted', recall_average_in='weighted'):
-            self.shap_on = model_monitor
-            self.runtime = runtime
-            logging.info('Using add_experiment(model_monitor={})'.format(model_monitor))
-            if f1_average_in not in ['micro', 'macro', 'weighted']:
-                raise ValueError("f1_average_in set micro|macro|weighted")
-            if recall_average_in not in ['micro', 'macro', 'weighted']:
-                raise ValueError("recall_average_in set micro|macro|weighted")
+            try:
+                self.feature_name = list(feature_names)
+            except AttributeError:
+                raise ValueError('입력값으로 list 또는 pandas.core.indexes.base.Index를 사용하시기 바랍니다.')
 
-            if type(model_name) == pipeline.Pipeline:
-                self.model_name = model_name.steps[-1][1]
-            else:
-                self.model_name = model_name
-        
-            # if in notebook
-            if is_in_ipython():
-                self.var_model_file_path = notebook_info
-                _caller_globals = inspect.stack()[1][0].f_globals
-                (
-                    self.mainfile,
-                    self.sources,
-                    self.dependencies
-                ) = gather_sources_and_dependencies(
-                    globs=_caller_globals,
-                    save_git_info=False
-                )
-            else:
-                _caller_globals = inspect.stack()[1][0].f_globals
-                (
-                    self.mainfile,
-                    self.sources,
-                    self.dependencies
-                ) = gather_sources_and_dependencies(
-                    globs=_caller_globals,
-                    save_git_info=True
-                )
-                self.var_model_file_path = self.mainfile['filename']
-
-            self.fitted_model = get.model_type(self.model_name)          # fitted model type
-            self.json_path = OrderedDict()                               # path
-            self.selected_params = []                                    # log params
-            self.selected_metrics = OrderedDict()                        # log metrics
-            self.summary_info = OrderedDict()                            # final results
-            self.error_log = []                                          # error log
-            self.vis_info = None                                         # visualization info - classifier
-            self.dict_path = path.get_file_path(self.model_name)
-
-            set_current_runs(get.model_type(self.model_name))
-            _set_result_path(self.dict_path)
-
-            # data for visualization function
-            if len(args) == 3:
-                self.xval = args[1]
-                self.yval = args[2]
-                self.summary_info['run_nick_name'] = args[0]
-
-            elif len(args) == 5:
-                self.xtrain = args[1]
-                self.ytrain = args[2]
-                self.xval = args[3]
-                self.yval = args[4]
-                self.summary_info['run_nick_name'] = args[0]
-
-            # 사용자가 run_nick_name 파라미터 입력 안했을 경우
-            # ex1) with accu.add_experiment(model, X_train_scaled, y_train_num, X_test_scaled, y_test_num, model_monitor=True, runtime=True) as exp:
-            # ex2) with accu.add_experiment(model, X_test_scaled, y_test_num, model_monitor=True, runtime=True) as exp:
-            elif len(args) == 2:
-                self.xval = args[0]
-                self.yval = args[1]
-                self.summary_info['run_nick_name'] = run_nick_name
-
-            elif len(args) == 4:
-                self.xtrain = args[0]
-                self.ytrain = args[1]
-                self.xval = args[2]
-                self.yval = args[3]
-                self.summary_info['run_nick_name'] = run_nick_name
+        return feature_names
 
-            else:
-                raise ValueError('Check the arguments of function - add_experiment(model_name, run_nick_name, X_val, y_val) or add_experiment(model_name, run_nick_name, X_train, y_train, X_val, y_val)',
-                                 '\n and No assign run_nick_name, set default run_nick_name as File name.')
+    def set_current_notebook(self):
+        self.notebook_info = get_current_notebook()
 
-            # 사용자가 run_nick_name 파라미터를 지정했는데 '' 일 경우
-            if args[0] == '':
-                self.summary_info['run_nick_name'] = run_nick_name
-
-            # sklearn/xgboost/lightgbm
-            get_from_model = get.from_model(self.model_name)
-            self.all_model_params = get_from_model.all_params()
-
-            if 'metric' not in self.all_model_params.keys():
-                self.all_model_params['metric'] = ''
-
-            self.model_param_keys = get_from_model.param_keys()
-            
-            # classifier
-            if any(i in self.fitted_model for i in CLASSIFICATION):
-                self.vis_info = roc_pr_curve(self.model_name, self.xval, self.yval, f1_average=f1_average_in, recall_average=recall_average_in)
-
-            # regressor
-            elif any(i in self.fitted_model for i in REGRESSION):
-                self.ypred = get_visual_info_regressor(self.model_name, self.xval)
-            
-            # if user uses lightgbm package, verify the model for classification or regression.
-            if self.fitted_model == 'lightgbm':
-                
-                # classifier
-                if self.all_model_params['metric'] in metricsLightgbm.CLASSIFICATION:
-                    self.vis_info = roc_pr_curve(self.model_name, self.xval, self.yval, f1_average=f1_average_in, recall_average=recall_average_in)
-                
-                # regressor
-                elif self.all_model_params['metric'] in metricsLightgbm.REGRESSION:
-                    self.ypred = get_visual_info_regressor(self.model_name, self.xval)
-                
-                # None
-                elif self.all_model_params['metric'] in metricsLightgbm.no_metrics:
-                    raise ValueError('Please set any metric parameter in the lightGBM.')
-            
-            set_model_file_path(self.var_model_file_path)
-
-            if hasattr(self, 'mainfile'):
-                set_git_meta(fileinfo=self.mainfile)
-            if hasattr(self, 'dependencies'):
-                set_python_dependencies(py_depenpency=self.dependencies)
-
-        def __enter__(self):
-            self.start_time = get_time.now()
-            self.summary_info[LOGGING_TIME] = get_time.logging_time()
-            self.summary_info[LOGGING_RUN_ID] = func.get_run_id()
-            self.summary_info[FITTED_MODEL] = self.fitted_model
-
-            if user_id is not None:
-                self.summary_info[USER_ID] = user_id
-
-            set_prefix_path(self.dict_path[LcConst.RUN_PREFIX_PATH])
-            set_run_name(self.fitted_model, self.summary_info[LOGGING_RUN_ID], self.summary_info['run_nick_name'])
-
-            return self
-
-        def __exit__(self, a, b, c):
-            self.summary_info[ALL_MODEL_PARAMS] = self.all_model_params
-            self.summary_info[SELECTED_PARAMS] = self.selected_params
-            self.summary_info[SELECTED_METRICS] = self.selected_metrics
-            self.summary_info[VALUE_ERROR] = self.error_log
-
-            # model_monitor = True
-            self.run_id = self.summary_info[LOGGING_RUN_ID]
-            
-            if self.shap_on:
-                if not feature_name:
-                    try:
-                        if self.data is not None:
-                            self.feature_name = get.feature_name(save_path, StorageInfo, target_name, data=self.data)
-                            self.data = None
-                        else:
-                            self.feature_name = get.feature_name(save_path, StorageInfo, target_name)
-                    except:
-                        self.feature_name = None
-                else:
-                    self.feature_name = feature_name
+    def get_current_notebook(self):
+        return self.notebook_info
 
-                self.run_id = self.fitted_model + '-' + self.run_id
-                
-                # when user uses lightGBM fitted by lightGBM datasets, convert data type to lightGBM dataset.
-                if self.fitted_model == 'lightgbm':
-                    self.xtrain = lgb.Dataset(self.xtrain, label=self.ytrain, silent=True)
-                        
-                self.shap_value = shap_value(self.model_name, self.xtrain, self.feature_name)
-                
-                # path for shap.json
-                shap_json_full_path = self.dict_path[RUN_MODEL_SHAP_JSON_PATH]
-                set_shap_json_path(self.dict_path['shap_json'])
-                
-                with open(shap_json_full_path, 'w', encoding='utf-8') as save_file:
-                    json.dump(self.shap_value, save_file, indent='\t')
-                
-            # visualization
-            if any(i in self.fitted_model for i in CLASSIFICATION) or self.all_model_params['metric'] in metricsLightgbm.CLASSIFICATION:
-
-                # path for visual.json
-                visual_json_full_path = self.dict_path[RUN_MODEL_VISUAL_JSON_PATH]
-                set_visual_json_path(self.dict_path['visual_json'])
-
-                with open(visual_json_full_path, 'w', encoding='utf-8') as save_file1:
-                    json.dump(self.vis_info, save_file1, indent="\t")
-
-            elif any(i in self.fitted_model for i in REGRESSION) or self.all_model_params['metric'] in metricsLightgbm.REGRESSION:
-                temp_yval = get_true_y(self.yval)
-                if len(temp_yval) <= 5000:
-                    self.summary_info['True_y'] = temp_yval
-                    self.summary_info['Predicted_y'] = get_visual_info_regressor(self.model_name, self.xval)
-                else:
-                    self.summary_info['True_y'] = None
-                    self.summary_info['Predicted_y'] = None
+    @staticmethod
+    def set_runtime_model(framework, run_id=None):
+        if framework == 'sklearn':
+            if run_id:
+                export_path = ENV_JUPYTER_HOME_DIR + '/airuntime/' + framework + '/models'
+                shutil.rmtree(export_path)
+                os.mkdir(export_path)
+                joblib.dump(load_model(run_id), export_path + '/model.joblib')
+            else:
+                with open(ENV_JUPYTER_HOME_DIR + '/runs/run_info.json') as f:
+                    json_object = json.load(f)
 
-            self.summary_info[VALUE_ERROR] = self.error_log
+                try:
+                    shutil.copyfile(ENV_JUPYTER_HOME_DIR + '/' + json_object['save_best_model_joblib_path'],
+                                    ENV_JUPYTER_HOME_DIR + '/airuntime/' + framework + '/models/model.joblib')
+                except TypeError:
+                    raise ValueError('최근에 실행된 experiment가 ML 모델이 아닙니다.')
+
+        elif framework == 'tensorflow' or framework == 'keras':
+            if run_id:
+                if framework == 'keras':
+                    framework = 'tensorflow'
 
-            if not self.summary_info[VALUE_ERROR]:
-                # path for model_info.json
-                model_json_full_path = self.dict_path[RUN_MODEL_JSON_PATH]
-                set_model_json_path(self.dict_path['model_json'])
-
-                with open(model_json_full_path, 'w', encoding='utf-8') as save_file2:
-                    json.dump(self.summary_info, save_file2, indent="\t")
-                    
-            else:
-                pass
+                saved_model = load_model(run_id)
 
-            # model save
-            save_model_path = self.dict_path[RUN_MODEL_JOBLIB_PATH] + self.summary_info[FITTED_MODEL] + '-' + self.summary_info[LOGGING_RUN_ID] +'.joblib'
-            path_for_setting_model_joblib = self.dict_path['save_model_dir'] + '/' + self.summary_info[FITTED_MODEL] + '-' + self.summary_info[LOGGING_RUN_ID] +'.joblib'
-
-            set_best_model_joblib_path(path_for_setting_model_joblib)
-
-            dump(self.model_name, save_model_path)
-
-            start_time = int(self.start_time.timestamp()*1000)
-            end_time = int(get_time.now().timestamp()*1000)
-            delta_ts = end_time - start_time
-
-            global run_meta
-            run_meta = clear_runs(start_time, end_time, delta_ts)
-
-            accuinsight._send_message(metric=None,
-                                      current_value=None,
-                                      message=message_param,
-                                      thresholds=None,
-                                      alarm_object=alarm,
-                                      alarm_api=alarm_api)
-
-            env_value = get_os_env('ENV')
-            modeler_rest = LifecycleRestApi(env_value[LcConst.BACK_END_API_URL],
-                                            env_value[LcConst.BACK_END_API_PORT],
-                                            env_value[LcConst.BACK_END_API_URI])
-            modeler_rest.lc_create_run(run_meta)
-            if self.runtime:
-                accuinsight.set_runtime_model('sklearn')
-
-        def log_params(self, param=None):
-            # sklearn/xgboost/lightgbm
-            if param:
-                if param in self.model_param_keys:
-                    return self.selected_params.append(param)
+            else:
+                with open(ENV_JUPYTER_HOME_DIR + '/runs/run_info.json') as f:
+                    json_object = json.load(f)
 
+                try:
+                    with open(ENV_JUPYTER_HOME_DIR + '/' + json_object['save_best_model_json_path'], 'r') as f:
+                        saved_model_json = f.read()
+                except TypeError:
+                    raise ValueError('최근에 실행된 experiment가 DL 모델이 아닙니다.')
+
+                if framework == 'keras':
+                    from keras.models import model_from_json
+                    saved_model = model_from_json(saved_model_json)
+                    framework = 'tensorflow'
                 else:
-                    self.error_log.append(True)
-                    raise ValueError('"' + param + '"' + ' does not exist in the model.')
+                    from tensorflow.keras.models import model_from_json
+                    saved_model = model_from_json(saved_model_json)
 
-        def log_metrics(self, metric_name, defined_metric):
-            self.selected_metrics[metric_name] = defined_metric
+                # load weights into new model
+                saved_model.load_weights(ENV_JUPYTER_HOME_DIR + '/' + json_object['save_best_model_h5_path'])
 
-        def log_tag(self, description):
-            self.summary_info['tag'] = description
+            export_path = ENV_JUPYTER_HOME_DIR + '/airuntime/' + framework + '/models'
+            shutil.rmtree(export_path)
+            saved_model.save(export_path + '/1', save_format='tf')
+        else:
+            raise ValueError("잘못된 framework 값이 입력되었습니다. framework가 가질 수 있는 값은 sklearn/tensorflow/keras 입니다.")
```

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/Lifecycle/keras.py` & `Accuinsight-3.4.230516rc1/Accuinsight/Lifecycle/keras.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 import warnings
 from collections import OrderedDict
 import gorilla
 import logging
 import numpy as np
 import keras
 from keras.callbacks import CSVLogger
-from Accuinsight.modeler.core import func, path, get
+from Accuinsight.modeler.core import func, path, get, modelEvaluation, lossFuncInfo
 from Accuinsight.modeler.core.func import get_time
 from Accuinsight.modeler.core.LcConst import LcConst
 from Accuinsight.modeler.core.LcConst.LcConst import RUN_NAME_KERAS, RUN_OBJ_NAME, RUN_MODEL_JSON_PATH, \
-    RUN_MODEL_SHAP_JSON_PATH, RUN_MODEL_VISUAL_JSON_PATH, SELECTED_METRICS, USER_ID
-from Accuinsight.modeler.core.get_for_visual import roc_pr_curve, get_visual_info_regressor
+    RUN_MODEL_SHAP_JSON_PATH, RUN_MODEL_VISUAL_JSON_PATH, SELECTED_METRICS, USER_ID, RUN_MODEL_EVL_JSON_PATH
+from Accuinsight.modeler.core.get_for_visual import roc_pr_curve, get_visual_info_regressor, get_true_y
 from Accuinsight.modeler.core.Run.RunInfo.RunInfo import set_current_runs, clear_runs, set_model_json_path, \
     set_visual_csv_path, set_visual_json_path, set_best_model_h5_path, set_best_model_json_path, \
-    set_python_dependencies, set_run_name, set_model_file_path, set_prefix_path, set_shap_json_path
+    set_python_dependencies, set_run_name, set_model_file_path, set_prefix_path, set_shap_json_path, set_model_type, \
+    set_optimizer_info_path, set_evl_json_path, set_selected_metrics_path
 from Accuinsight.modeler.core.feature_contribution import shap_value
 from Accuinsight.modeler.utils.dl_utils import delete_files_except_best, get_best_model_path
 from Accuinsight.modeler.utils.dependency.dependencies import gather_sources_and_dependencies
 from Accuinsight.modeler.utils.os_getenv import is_in_ipython, get_os_env
 from Accuinsight.modeler.clients.modeler_api import LifecycleRestApi
 from Accuinsight.Lifecycle.common import Common
 
@@ -46,14 +47,136 @@
 
     def get_current_run_id(self):
         try:
             return self.get_current_run_meta()[RUN_OBJ_NAME]
         except TypeError or KeyError:
             return None
 
+    def model_evaluation(self, run_nickname_input=None, loaded_model=None, loaded_model_json=None, x_validation=None, y_validation=None):
+        start_evl = get_time.now()
+
+        # get_file_path 실행 시 experiment 생성 시 필요한 폴더들이 다 만들어짐.
+        # modeler backend 호출 시 파라미터로 경로 내 json 파일 내용을 protobuf 통해서 변환 후 gRPC로 전송을 위해 사용.
+        self.dict_path = path.get_file_path(loaded_model, usedFramework='tensorflow')
+
+        # dependencies를 가져오기 위한 작업
+        if is_in_ipython():
+            var_model_file_path = self.notebook_info
+            _caller_globals = inspect.stack()[1][0].f_globals
+            (
+                mainfile,
+                sources,
+                dependencies
+            ) = gather_sources_and_dependencies(
+                globs=_caller_globals,
+                save_git_info=False
+            )
+        else:
+            _caller_globals = inspect.stack()[1][0].f_globals
+            (
+                mainfile,
+                sources,
+                dependencies
+            ) = gather_sources_and_dependencies(
+                globs=_caller_globals,
+                save_git_info=True
+            )
+            var_model_file_path = mainfile['filename']
+
+        if run_nickname_input is None:
+            run_nick_name = self.default_run_nick_name
+        else:
+            run_nick_name = run_nickname_input
+
+
+        if loaded_model is None or x_validation is None or y_validation is None or loaded_model_json is None:
+            raise ValueError("Please set parameter -> model or validation data. ")
+        x_val = x_validation
+        y_val = y_validation
+
+        # set current run
+        set_current_runs(RUN_NAME_KERAS)
+
+        # path for for-evl-json
+        # visualCallback 참고 해서 actual data로 성능평가
+        path_for_setting_evl_json = self.dict_path['evl_json']
+        evl_json_full_path = self.dict_path[RUN_MODEL_EVL_JSON_PATH]
+        set_evl_json_path(path_for_setting_evl_json)
+
+        loaded_model_json_dict = json.loads(loaded_model_json)
+        loss_function = loaded_model_json_dict['loss_function']
+        run_id = loaded_model_json_dict['run_id']
+
+        '''
+        RunInfo.py 내 아래 데이터에 set
+        global _runData
+        run_obj = _runData[0]
+        '''
+        set_optimizer_info_path(loaded_model_json_dict['optimizer_info'])
+        set_model_file_path(loaded_model_json_dict['path'])
+        set_python_dependencies(py_depenpency=loaded_model_json_dict['model_dependencies'])
+        set_prefix_path(self.dict_path[LcConst.RUN_PREFIX_PATH])
+        set_run_name('tf.keras', run_id, run_nick_name)
+
+        set_best_model_json_path(loaded_model_json_dict['best_model_json'])
+        set_best_model_h5_path(loaded_model_json_dict['best_model_h5'])
+
+
+        # 모델 라이브러리 확인 (tf or keras)
+        if isinstance(loaded_model, keras.Model): #Sequential은 Model에서 상속 받아 같음.
+
+            # print(loss_function)
+            # print(self.dict_path[RUN_MODEL_EVL_JSON_PATH])
+
+            # classification
+            if loss_function in lossFuncInfo.CLASSIFICATION:
+                print("DL_CLASSIFICATION in model_evaluation method")
+                # visual_classification_json = roc_pr_curve(loaded_model, x_val, y_val, f1_average=f1_average_in,
+                #                                           recall_average=recall_average_in)
+                visual_classification_json = roc_pr_curve(loaded_model, x_val, y_val, f1_average="weighted",
+                                                          recall_average="weighted")
+                with open(evl_json_full_path, 'w', encoding='utf-8') as save_file:
+                    json.dump(visual_classification_json, save_file, indent="\t")
+
+                selected_metrics = modelEvaluation.calculate_classification_metrics(loaded_model, x_val, y_val, average='weighted')
+                set_model_type("DL_CLASSIFICATION")
+            # regression
+            elif loss_function in lossFuncInfo.REGRESSION:
+                print("DL_REGRESSION in model_evaluation method")
+                visual_regression_json = OrderedDict()
+                visual_regression_json['True_y'] = get_true_y(y_val)
+                visual_regression_json['Predicted_y'] = get_visual_info_regressor(loaded_model, x_val)
+
+                with open(evl_json_full_path, 'w', encoding='utf-8') as save_file:
+                    json.dump(visual_regression_json, save_file, indent="\t")
+
+                selected_metrics = modelEvaluation.calculate_regression_metrics(loaded_model, x_val, y_val)
+                set_model_type("DL_REGRESSION")
+
+            else:
+                raise ValueError('현재 설정한 loss는 지원되지 않습니다. 관리자에게 문의하십시오.')
+        else: # keras 만을 사용한 경우 없음. 추후 pytorch 대응용
+            pass
+        loaded_model_json_dict[SELECTED_METRICS] = selected_metrics
+        set_selected_metrics_path(loaded_model_json_dict[SELECTED_METRICS])
+
+        end_evl = get_time.now()
+
+        start_ts = int(start_evl.timestamp())
+        end_ts = int(end_evl.timestamp())
+        delta_ts = end_ts - start_ts
+
+        run_meta = clear_runs(start_ts, end_ts, delta_ts, isEvaluation="true")
+
+        env_value = get_os_env('ENV')
+        modeler_rest = LifecycleRestApi(env_value[LcConst.BACK_END_API_URL],
+                                        env_value[LcConst.BACK_END_API_PORT],
+                                        env_value[LcConst.BACK_END_API_URI])
+        modeler_rest.lc_create_run(run_meta)
+
     def autolog(self, run_nickname_input=None, tag=None, best_weights=False, model_monitor=False, runtime=False, f1_average_in='weighted', recall_average_in='weighted'):
         global description, endpoint, var_model_file_path, message, thresholds, best_weights_on, run_id, alarm, alarm_api, shap_on, feature_name, run_meta, run_nick_name
         description = tag
         endpoint = self.endpoint
         message = self.message # common.py send_message 호출을 통해 생성
         thresholds = self.thresholds
         alarm = self.workspace_alarm
@@ -226,21 +349,45 @@
                 # model save path
                 run_id = self.model_summary['model_type'] + '-' + self.model_summary['run_id']
                 common_path = self.dict_path['save_model_path'] + run_id + '-epoch-' + str(epoch + 1).zfill(5) \
                               + '-' + self.monitor + '-' + str(current).zfill(5)
                 save_model_path = common_path + '.json'
                 save_weights_path = common_path + '.h5'
 
+                # model evaluation path(in jupyter lab browser path)
+                browser_common_path = self.dict_path['save_model_dir'] + '/' + run_id + '-epoch-' + str(epoch + 1).zfill(
+                    5) + '-' + self.monitor + '-' + str(current).zfill(5)
+                save_model_path_browser = browser_common_path + '.json'
+                save_weights_path_browser = browser_common_path + '.h5'
+
                 # model to JSON
                 model_json = self.model.to_json()
+
+                # model 정보에 loss 추가
+                model_dict = json.loads(model_json)
+                model_dict['loss_function'] = self.model_summary['loss_function']
+                model_dict['run_id'] = self.model_summary['run_id']
+                model_dict['path'] = var_model_file_path
+                model_dict['model_dependencies'] = dependencies
+                model_dict['best_model_h5'] = save_weights_path_browser
+                model_dict['best_model_json'] = save_model_path_browser
+                model_dict['optimizer_info'] = self.model_summary['optimizer_info']
+                if best_weights_on:
+                    model_dict[SELECTED_METRICS] = {self.monitor: np.float64(self.best)}
+                else:
+                    model_dict[SELECTED_METRICS] = {self.monitor: np.float64(self.last_epoch_metric)}
+
+                updated_model_json = json.dumps(model_dict)
+
                 with open(save_model_path, "w") as json_file:
-                    json_file.write(model_json)
+                    json_file.write(updated_model_json)
 
                 # weights to H5
-                self.model.save_weights(save_weights_path)
+                # self.model.save_weights(save_weights_path)
+                self.model.save(save_weights_path)
 
             def on_train_end(self, logs={}):
                 '''[get best model] on_train_end '''
                 if self.verbose > 0:
                     print('Using epoch %05d with %s: %0.5f' % (self.best_epochs, self.monitor, self.best))
                 self.model.set_weights(self.best_weights)  # set best model's weights
```

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/Lifecycle/settings.py` & `Accuinsight-3.4.230516rc1/Accuinsight/Lifecycle/settings.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/Lifecycle/tensorflow.py` & `Accuinsight-3.4.230516rc1/Accuinsight/Lifecycle/tensorflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from Accuinsight.modeler.core.func import get_time
 from Accuinsight.modeler.core.LcConst import LcConst
 from Accuinsight.modeler.core.LcConst.LcConst import RUN_NAME_TENSORFLOW, RUN_OBJ_NAME, RUN_MODEL_JSON_PATH, \
     RUN_MODEL_VISUAL_JSON_PATH,RUN_MODEL_EVL_JSON_PATH, RUN_MODEL_VISUAL_CSV_PATH, SELECTED_METRICS, USER_ID
 from Accuinsight.modeler.core.Run.RunInfo.RunInfo import set_current_runs, clear_runs, set_model_json_path, \
     set_visual_csv_path, set_visual_json_path, set_best_model_json_path, set_best_model_h5_path, \
     set_python_dependencies, set_run_name, set_model_file_path, set_prefix_path, set_shap_json_path, set_evl_json_path, \
-    set_optimizer_info_path, set_selected_metrics_path
+    set_optimizer_info_path, set_selected_metrics_path, set_model_type, set_true_y, set_predict_y
 from Accuinsight.modeler.core.get_for_visual import roc_pr_curve, get_true_y, get_visual_info_regressor
 from Accuinsight.modeler.clients.modeler_api import LifecycleRestApi
 from Accuinsight.modeler.utils.dependency.dependencies import gather_sources_and_dependencies
 from Accuinsight.modeler.utils.dl_utils import delete_files_except_best, get_best_model_path
 from Accuinsight.modeler.utils.os_getenv import is_in_ipython, get_os_env
 from Accuinsight.modeler.core.feature_contribution import shap_value
 from Accuinsight.Lifecycle.common import Common
@@ -51,24 +51,21 @@
 
     def get_current_run_id(self):
         try:
             return self.get_current_run_meta()[RUN_OBJ_NAME]
         except TypeError or KeyError:
             return None
 
-    def model_evaluation(self, run_nickname_input=None, loaded_model=None, loaded_model_json=None, x_validation=None, y_validation=None):
+    def model_evaluation(self, run_nickname_input=None, loaded_model=None, loaded_model_json=None, x_validation=None, y_validation=None, f1_average_in='weighted', recall_average_in='weighted'):
         start_evl = get_time.now()
 
         # get_file_path 실행 시 experiment 생성 시 필요한 폴더들이 다 만들어짐.
         # modeler backend 호출 시 파라미터로 경로 내 json 파일 내용을 protobuf 통해서 변환 후 gRPC로 전송을 위해 사용.
         self.dict_path = path.get_file_path(loaded_model, usedFramework='tensorflow')
 
-        # set current run
-        set_current_runs(RUN_NAME_TENSORFLOW)
-
         # dependencies를 가져오기 위한 작업
         if is_in_ipython():
             var_model_file_path = self.notebook_info
             _caller_globals = inspect.stack()[1][0].f_globals
             (
                 mainfile,
                 sources,
@@ -96,65 +93,76 @@
 
 
         if loaded_model is None or x_validation is None or y_validation is None or loaded_model_json is None:
             raise ValueError("Please set parameter -> model or validation data. ")
         x_val = x_validation
         y_val = y_validation
 
+        # set current run
+        set_current_runs(RUN_NAME_TENSORFLOW)
+
         # path for for-evl-json
         # visualCallback 참고 해서 actual data로 성능평가
         path_for_setting_evl_json = self.dict_path['evl_json']
         evl_json_full_path = self.dict_path[RUN_MODEL_EVL_JSON_PATH]
         set_evl_json_path(path_for_setting_evl_json)
 
         loaded_model_json_dict = json.loads(loaded_model_json)
         loss_function = loaded_model_json_dict['loss_function']
         run_id = loaded_model_json_dict['run_id']
 
+        '''
+        RunInfo.py 내 아래 데이터에 set
+        global _runData
+        run_obj = _runData[0]
+        '''
         set_optimizer_info_path(loaded_model_json_dict['optimizer_info'])
         set_model_file_path(loaded_model_json_dict['path'])
         set_python_dependencies(py_depenpency=loaded_model_json_dict['model_dependencies'])
         set_prefix_path(self.dict_path[LcConst.RUN_PREFIX_PATH])
         set_run_name('tf.keras', run_id, run_nick_name)
 
         set_best_model_json_path(loaded_model_json_dict['best_model_json'])
         set_best_model_h5_path(loaded_model_json_dict['best_model_h5'])
 
 
         # 모델 라이브러리 확인 (tf or keras)
         if isinstance(loaded_model, tensorflow.keras.Model): #Sequential은 Model에서 상속 받아 같음.
 
-            print(loss_function)
-            print(self.dict_path[RUN_MODEL_EVL_JSON_PATH])
+            # print(loss_function)
+            # print(self.dict_path[RUN_MODEL_EVL_JSON_PATH])
 
             # classification
             if loss_function in lossFuncInfo.CLASSIFICATION:
-                print("나는야 분류")
-                # visual_classification_json = roc_pr_curve(loaded_model, x_val, y_val, f1_average=f1_average_in,
-                #                                           recall_average=recall_average_in)
-                visual_classification_json = roc_pr_curve(loaded_model, x_val, y_val, f1_average="weighted",
-                                                          recall_average="weighted")
+                print("DL_CLASSIFICATION in model_evaluation method")
+                visual_classification_json = roc_pr_curve(loaded_model, x_val, y_val, f1_average=f1_average_in,
+                                                          recall_average=recall_average_in)
                 with open(evl_json_full_path, 'w', encoding='utf-8') as save_file:
                     json.dump(visual_classification_json, save_file, indent="\t")
 
-                selected_metrics = modelEvaluation.calculate_classification_metrics(loaded_model, x_val, y_val, average='weighted')
-
+                selected_metrics = modelEvaluation.calculate_classification_metrics(loaded_model, x_val, y_val, average=f1_average_in)
+                set_model_type("DL_CLASSIFICATION")
             # regression
             elif loss_function in lossFuncInfo.REGRESSION:
+                print("DL_REGRESSION in model_evaluation method")
                 visual_regression_json = OrderedDict()
                 visual_regression_json['True_y'] = get_true_y(y_val)
                 visual_regression_json['Predicted_y'] = get_visual_info_regressor(loaded_model, x_val)
 
+                set_true_y(visual_regression_json['True_y'])
+                set_predict_y(visual_regression_json['Predicted_y'])
+
                 with open(evl_json_full_path, 'w', encoding='utf-8') as save_file:
                     json.dump(visual_regression_json, save_file, indent="\t")
 
                 selected_metrics = modelEvaluation.calculate_regression_metrics(loaded_model, x_val, y_val)
+                set_model_type("DL_REGRESSION")
 
             else:
-                raise ValueError('현재 설정한 loss는 지원되지 않습니다. 관리자에게 문의하십시오.')
+                raise ValueError('현재 설정한 모델은 지원되지 않습니다. 관리자에게 문의하십시오.')
         else: # keras 만을 사용한 경우 없음. 추후 pytorch 대응용
             pass
         loaded_model_json_dict[SELECTED_METRICS] = selected_metrics
         set_selected_metrics_path(loaded_model_json_dict[SELECTED_METRICS])
 
         end_evl = get_time.now()
 
@@ -343,15 +351,15 @@
 
                 # model save path
                 run_id = self.model_summary['model_type'] + '-' + self.model_summary['run_id']
                 common_path = self.dict_path['save_model_path'] + run_id + '-epoch-' + str(epoch + 1).zfill(5) + '-' + self.monitor + '-' + str(current).zfill(5)
                 save_model_path = common_path + '.json'
                 save_weights_path = common_path + '.h5'
 
-                # model evaluation path(in jupyter lab browser path)
+                # model evaluation path(in jupyter lab browser path - 상대경로 의미...)
                 browser_common_path = self.dict_path['save_model_dir'] + '/' + run_id + '-epoch-' + str(epoch + 1).zfill(
                     5) + '-' + self.monitor + '-' + str(current).zfill(5)
                 save_model_path_browser = browser_common_path + '.json'
                 save_weights_path_browser = browser_common_path + '.h5'
 
                 # model to JSON
                 model_json = self.model.to_json()
```

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/Lifecycle/utils.py` & `Accuinsight-3.4.230516rc1/Accuinsight/Lifecycle/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,37 +8,33 @@
 
 class AbcNotifier:
     def completed_message(self, **kwargs):
         pass
 
 
 def load_model(run_name):
-    k = []
     best_model_path_dict = dict()
 
     model_type = run_name.split('-')[0]
     t = run_name.split('-')[1].split('_')[0]
     filename = model_type + '-' + t[0:8] + '-' + t[8:12] + '-' + t[12:16] + '-' + t[16:20] + '-' +  t[20:]
     regex = re.compile(filename)
 
     common_path = '/home/work/runs/best-model'
 
     for subdir, dirs, files in os.walk(common_path):
+        dirs[:] = []  # 하위 디렉토리를 탐색하지 않도록 dirs 리스트를 비움
         for filename in files:
             if regex.search(filename):
-                k.append(os.path.join(common_path, filename))
-
-    if 'json' in k[0]:
-        best_model_path_dict['json'] = k[0]
-        best_model_path_dict['h5'] = k[1]
-    elif 'h5' in k[0]:
-        best_model_path_dict['json'] = k[1]
-        best_model_path_dict['h5'] = k[0]
-    else:
-        best_model_path_dict['joblib'] = k[0]
+                if filename.endswith(".joblib"):
+                    best_model_path_dict['joblib'] = os.path.join(common_path, filename)
+                elif filename.endswith(".json"):
+                    best_model_path_dict['json'] = os.path.join(common_path, filename)
+                elif filename.endswith(".h5"):
+                    best_model_path_dict['h5'] = os.path.join(common_path, filename)
 
     # load model trained using keras
     if model_type == 'keras':
         from keras.models import model_from_json
         # load json and create model
         json_file = open(best_model_path_dict['json'], 'r')
         loaded_model_json = json_file.read()
@@ -60,14 +56,17 @@
 
         # load weights into new model
         loaded_model.load_weights(best_model_path_dict['h5'])
         # loaded_model.load_model(best_model_path_dict['h5'])
 
     else:
         import joblib
+        json_file = open(best_model_path_dict['json'], 'r')
+        loaded_model_json = json_file.read()
+        json_file.close()
         loaded_model = joblib.load(best_model_path_dict['joblib'])
 
     # 파라미터 추가
     # 실제로 experiment 모델을 생성하는 것이 아니라 평가해서 모델러 백엔드로 동일 모델에 대한 평가를 식별하기 위해 추가.
     loaded_model_dict = json.loads(loaded_model_json)
 
     loaded_model_dict["run_name"] = run_name
```

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/Monitoring/deploy/monitoring_deploy.py` & `Accuinsight-3.4.230516rc1/Accuinsight/Monitoring/deploy/monitoring_deploy.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/WorkspaceRun/workspace_run.py` & `Accuinsight-3.4.230516rc1/Accuinsight/WorkspaceRun/workspace_run.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,15 @@
         self.custom_args = ''
 
     def exec_code(self):
         parser = argparse.ArgumentParser()
         parser.add_argument('--workspaceRunId', default=None)
         parser.add_argument('--codePath', default=None)
         parser.add_argument('--argument', default='')
+        parser.add_argument('--envPath', default='/opt/conda')
 
         args, unknown = parser.parse_known_args()
         args_dict = vars(args)
 
         # set custom arguments
         if not args_dict['argument'] == '':
             self.custom_args = ' ' + args_dict['argument']\
@@ -58,21 +59,22 @@
 
         self.code_path = args_dict['codePath']
         self.workspace_run_log.workspace_run_id = args_dict['workspaceRunId']
 
         if not self.code_path:
             raise Exception("codePath cannot be none")
 
+        env_path = args_dict['envPath']
         new_env = os.environ.copy()
-        new_env['PATH'] = '/opt/conda/bin:' + new_env['PATH']
+        new_env['PATH'] = env_path + '/bin:' + new_env['PATH']
 
         try:
             # python run with subprocess
-            subprocess.run("/opt/conda/bin/python -u '%s'%s > /tmp/output_%s.log 2>&1" %
-                           (self.code_path, self.custom_args, self.workspace_run_log.workspace_run_id),
+            subprocess.run("%s/bin/python -u '%s'%s > /tmp/output_%s.log 2>&1" %
+                           (env_path, self.code_path, self.custom_args, self.workspace_run_log.workspace_run_id),
                            shell=True, encoding='UTF-8', env=new_env).check_returncode()
             self.workspace_run_log.is_success = True
 
             # add success log
             with open("/tmp/output_%s.log" % self.workspace_run_log.workspace_run_id, 'a') as result_log:
                 result_log.write("\nWorkspace run with id=%s has been successfully finished.\n" %
                                  self.workspace_run_log.workspace_run_id)
```

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/exceptions.py` & `Accuinsight-3.4.230516rc1/Accuinsight/exceptions.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/clients/modeler_api.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/clients/modeler_api.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/LcConst/LcConst.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/LcConst/LcConst.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 FITTED_MODEL = 'fitted_model'
 ALL_MODEL_PARAMS = 'all_model_params'
 SELECTED_PARAMS = 'selected_params'
 SELECTED_METRICS = 'selected_metrics'
 VALUE_ERROR = 'ValueError'
 USER_ID = 'user_id'
 TAG = 'tag'
-
+RUN_ID = 'run_id'
 # using dl framework
 RUN_NAME_KERAS = 'keras'
 RUN_NAME_TENSORFLOW = 'tensorflow'
 
 # for run object
 RUN_BASE_PATH = 'base_path'
 RUN_ROOT_PATH = '/runs/'
 RUN_PREFIX_PATH = 'prefix_path'
 
 RUN_OBJ_NAME = 'run_name'
+RUN_OBJ_ID = 'run_id'
 RUN_OBJ_NICK_NAME = 'run_nick_name'
 RUN_OBJ_IS_EVALUATION = 'is_evaluation'
 RUN_OBJ_OPT_INFO = 'optimizer_info'
 
 RUN_OBJ_JSON_PATH = 'json_path'
 RUN_OBJ_CSV_PATH = 'csv_path'
 RUN_OBJ_VISUAL_PATH = 'visual_path'
@@ -34,14 +35,19 @@
 RUN_OBJ_VISUAL_JSON_PATH = 'visual_json_path'
 RUN_OBJ_EVL_JSON_PATH = 'evl_json_path'
 RUN_OBJ_SHAP_JSON_PATH = 'shap_json_path'
 RUN_OBJ_BEST_MODEL_H5_PATH = 'save_best_model_h5_path'
 RUN_OBJ_BEST_MODEL_JSON_PATH = 'save_best_model_json_path'
 RUN_OBJ_BEST_MODEL_JOBLIB_PATH = 'save_best_model_joblib_path'
 RUN_OBJ_DATA_VERSION = 'data_version'
+RUN_OBJ_MODELTYPE = 'model_type'
+RUN_OBJ_ALL_MODEL_PARAMS = 'all_model_params'
+RUN_OBJ_SELECTED_PARAMS = 'selected_params'
+RUN_OBJ_TRUE_Y = 'True_y'
+RUN_OBJ_PREDICT_Y = 'Predicted_y'
 
 # full path
 RUN_MODEL_JSON_PATH = 'model_json_full'
 RUN_MODEL_VISUAL_JSON_PATH = 'visual_json_full'
 RUN_MODEL_SHAP_JSON_PATH = 'shap_json_full'
 RUN_MODEL_VISUAL_CSV_PATH = 'visual_csv_full'
 RUN_MODEL_EVL_JSON_PATH = 'evl_json_full'
```

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/ModelType.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/ModelType.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/Run/ParseRun/BaseParser.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/BaseParser.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 import json
 from enum import Enum
 from Accuinsight.modeler.core.LcConst import LcConst
-from Accuinsight.modeler.core.Run.ParseRun import Parse_MLClassifier
+from Accuinsight.modeler.core.Run.ParseRun import Parse_MLClassifier, Parse_MLClassifier_evl, Parse_MLRegression_evl
 from Accuinsight.modeler.core.Run.ParseRun import Parse_DLRegression
 from Accuinsight.modeler.core.Run.ParseRun import Parse_DLClassification
 from Accuinsight.modeler.core.Run.ParseRun import Parse_MLRegression
 from Accuinsight.modeler.core.Run.ParseRun import Parse_DLClassification_evl
+from Accuinsight.modeler.core.Run.ParseRun import Parse_DLRegression_evl
 
 
 class ModelType(Enum):
     DL_REGRESSION = 1
     DL_CLASSIFICATION = 2
     ML_REGRESSION = 3
     ML_CLASSIFICATION = 4
     DL_REGRESSION_evl = 5
     DL_CLASSIFICATION_evl = 6
+    ML_REGRESSION_evl = 7
+    ML_CLASSIFICATION_evl = 8
 
 
 def run_parser(parser_type, run_info_json):
     if parser_type is ModelType.DL_REGRESSION:
         return Parse_DLRegression.parse_run_result(run_info_json)
 
     if parser_type is ModelType.DL_CLASSIFICATION:
@@ -30,14 +33,25 @@
     if parser_type is ModelType.ML_CLASSIFICATION:
         return Parse_MLClassifier.parse_run_result(run_info_json)
 
     #evaluation
     if parser_type is ModelType.DL_CLASSIFICATION_evl:
         return Parse_DLClassification_evl.parse_run_result(run_info_json)
 
+    if parser_type is ModelType.DL_REGRESSION_evl:
+        return Parse_DLRegression_evl.parse_run_result(run_info_json)
+
+    if parser_type is ModelType.ML_CLASSIFICATION_evl:
+        return Parse_MLClassifier_evl.parse_run_result(run_info_json)
+
+    if parser_type is ModelType.ML_REGRESSION_evl:
+        return Parse_MLRegression_evl.parse_run_result(run_info_json)
+    else:
+        print('Data parsing error for rest API (lc_create_run method)')
+        exit(1)
 
 def get_parser_type(run_info_json):
     parser_type = None
     run_result_path = run_info_json[LcConst.RUN_RESULT_PATH]
 
     # data_path = run_result_path[LcConst.RUN_MODEL_JSON_PATH]
     visual_json_path = None
@@ -70,14 +84,22 @@
     if visual_json_path is not None and visual_csv_path is None:
         parser_type = ModelType.ML_CLASSIFICATION
 
     # evaluation
     if LcConst.RUN_MODEL_EVL_JSON_PATH in run_result_path:
         evl_json_path = run_result_path[LcConst.RUN_MODEL_EVL_JSON_PATH]
 
-    if evl_json_path is not None:
+    if evl_json_path is not None and run_info_json[LcConst.RUN_OBJ_MODELTYPE] == "DL_CLASSIFICATION":
         parser_type = ModelType.DL_CLASSIFICATION_evl
-        print("이쪽으로 오니?")
-
+        print("DL_CLASSIFICATION 평가")
+    elif evl_json_path is not None and run_info_json[LcConst.RUN_OBJ_MODELTYPE] == "DL_REGRESSION":
+        parser_type = ModelType.DL_REGRESSION_evl
+        print("DL_REGRESSION 평가")
+    elif evl_json_path is not None and run_info_json[LcConst.RUN_OBJ_MODELTYPE] == "ML_CLASSIFICATION":
+        parser_type = ModelType.ML_CLASSIFICATION_evl
+        print("ML_CLASSIFICATION 평가")
+    elif evl_json_path is not None and run_info_json[LcConst.RUN_OBJ_MODELTYPE] == "ML_REGRESSION":
+        parser_type = ModelType.ML_REGRESSION_evl
+        print("ML_REGRESSION 평가")
     return parser_type
```

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/Run/ParseRun/ParseExperiment.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/ParseExperiment.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/Run/ParseRun/ParseKeras.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/ParseKeras.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/Run/ParseRun/Parse_DLClassification.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/Parse_DLClassification.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/Run/ParseRun/Parse_DLRegression.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/Parse_DLRegression.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/Run/ParseRun/Parse_MLClassifier.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/Parse_MLClassifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,9 +143,8 @@
         if grpc_params[i].key == 'data_version':
             result_dict['artifact'] = {}
             result_dict['artifact']['name'] = grpc_params[i].value
             result_dict['artifact']['version'] = ""
             del grpc_params[i]
             break
 
-    return result_dict
-
+    return result_dict
```

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/Run/ParseRun/Parse_MLRegression.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/Parse_MLRegression.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/Run/ParseRun/ParserVisualJaon.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/ParseRun/ParserVisualJaon.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 
 
 def parse_run_visual(run_mata):
     # parse 'for-visual-json/keras-visual-n.json'
     run_result_path = run_mata[RUN_RESULT_PATH]
     if run_mata[RUN_OBJ_IS_EVALUATION]=='true':
         visual_path = run_result_path[RUN_MODEL_EVL_JSON_PATH]
-        print("여기 보이니~~~~~", visual_path)
+        print("Set evaluation path.", visual_path)
     else:
         visual_path = run_result_path[RUN_MODEL_VISUAL_JSON_PATH]
 
     with open(visual_path) as visual_file:
         visual_data = json.load(visual_file)
 
     result_dict = {'metrics': []}
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/Run/RunInfo/RunInfo.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/RunInfo/RunInfo.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,14 @@
     run_obj[LcConst.RUN_OBJ_VISUAL_JSON_PATH] = None
     run_obj[LcConst.RUN_OBJ_EVL_JSON_PATH] = None
     run_obj[LcConst.RUN_OBJ_SHAP_JSON_PATH] = None
     run_obj[LcConst.RUN_OBJ_BEST_MODEL_H5_PATH] = None
     run_obj[LcConst.RUN_OBJ_BEST_MODEL_JSON_PATH] = None
     run_obj[LcConst.RUN_OBJ_BEST_MODEL_JOBLIB_PATH] = None
 
-
     _runData.append(run_obj)
 
     return _runData
 
 
 def clear_runs(start_time, end_time, delta_time, isEvaluation="false"):
     global _runData
@@ -61,17 +60,26 @@
     save_result_path[LcConst.RUN_PREFIX_PATH] = run_meta[LcConst.RUN_PREFIX_PATH]
     if isEvaluation == "false":
         save_result_path[LcConst.RUN_MODEL_JSON_PATH] = ''.join([save_result_path[LcConst.RUN_BASE_PATH],
                                                             save_result_path[LcConst.RUN_PREFIX_PATH],
                                                             run_meta[LcConst.RUN_OBJ_MODEL_JSON_PATH]
                                                             ])
     else:
-        run_meta[LcConst.RUN_OBJ_OPT_INFO] = run_obj[LcConst.RUN_OBJ_OPT_INFO]
         run_meta[LcConst.SELECTED_METRICS] = run_obj[LcConst.SELECTED_METRICS]
+        run_meta[LcConst.RUN_OBJ_MODELTYPE] = run_obj[LcConst.RUN_OBJ_MODELTYPE]
 
+        # optimazer info는 DL에만 있음.
+        if run_meta[LcConst.RUN_OBJ_MODELTYPE] == "DL_CLASSIFICATION" or run_meta[LcConst.RUN_OBJ_MODELTYPE] == "DL_REGRESSION":
+            run_meta[LcConst.RUN_OBJ_OPT_INFO] = run_obj[LcConst.RUN_OBJ_OPT_INFO]
+        elif run_meta[LcConst.RUN_OBJ_MODELTYPE] == "ML_CLASSIFICATION" or run_meta[LcConst.RUN_OBJ_MODELTYPE] == "ML_REGRESSION":
+            run_meta[LcConst.RUN_OBJ_ALL_MODEL_PARAMS] = run_obj[LcConst.RUN_OBJ_ALL_MODEL_PARAMS]
+            run_meta[LcConst.RUN_OBJ_SELECTED_PARAMS] = run_obj[LcConst.RUN_OBJ_SELECTED_PARAMS]
+        if run_meta[LcConst.RUN_OBJ_MODELTYPE] == "DL_REGRESSION" or run_meta[LcConst.RUN_OBJ_MODELTYPE] == "ML_REGRESSION":
+            run_meta[LcConst.RUN_OBJ_TRUE_Y] = run_obj[LcConst.RUN_OBJ_TRUE_Y]
+            run_meta[LcConst.RUN_OBJ_PREDICT_Y] = run_obj[LcConst.RUN_OBJ_PREDICT_Y]
 
     if run_meta[LcConst.RUN_OBJ_VISUAL_CSV_PATH] is not None:
         save_result_path[LcConst.RUN_MODEL_VISUAL_CSV_PATH] = ''.join([save_result_path[LcConst.RUN_BASE_PATH],
                                                                       save_result_path[LcConst.RUN_PREFIX_PATH],
                                                                       run_meta[LcConst.RUN_OBJ_VISUAL_CSV_PATH]
                                                                       ])
 
@@ -249,14 +257,44 @@
 
 def set_python_dependencies(py_depenpency):
     global _runData
 
     run_obj = _runData[0]
     run_obj[LcConst.PYTHON_DEPENDENCY] = py_depenpency
 
+def set_model_type(model_type):
+    global _runData
+
+    run_obj = _runData[0]
+    run_obj[LcConst.RUN_OBJ_MODELTYPE] = model_type
+
+def set_all_model_params(model_params):
+    global _runData
+
+    run_obj = _runData[0]
+    run_obj[LcConst.RUN_OBJ_ALL_MODEL_PARAMS] = model_params
+
+def set_selected_params(selected_params):
+    global _runData
+
+    run_obj = _runData[0]
+    run_obj[LcConst.RUN_OBJ_SELECTED_PARAMS] = selected_params
+
+def set_true_y(true_y):
+    global _runData
+
+    run_obj = _runData[0]
+    run_obj[LcConst.RUN_OBJ_TRUE_Y] = true_y
+
+def set_predict_y(predict_y):
+    global _runData
+
+    run_obj = _runData[0]
+    run_obj[LcConst.RUN_OBJ_PREDICT_Y] = predict_y
+
 
 def dict_to_list(dict_data):
     # "dependency": {
     #     "numpy": "1.18.2",
     #     "scikit-learn": "0.22.2.post1",
     #     "xgboost": "1.1.0rc1",
     #     "ModelLifeCycle": "0.1.0"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/Run/RunOjbject.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/Run/RunOjbject.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/feature_contribution.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/feature_contribution.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/func_for_visual.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/func_for_visual.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/get.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/get.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/get_for_visual.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/get_for_visual.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,29 +48,30 @@
         y_test_cat = y_test
 
     return y_test_cat
 
 
 def y_pred_reshape(model, X_test):
     prob = model.predict(X_test)
-
     if prob.ndim == 1:
+        print('y_pred_reshape: prob.ndim == 1')
         try:
-            y_pred = [1 if i >= 0.5 else 0 for i in prob]
+            y_pred = prob
         except TypeError:
             y_pred = list(prob)
 
     elif prob.ndim == 2:
+        print('y_pred_reshape: prob.ndim == 2')
         if prob.shape[1] == 1:
             y_prob = np.c_[1-prob, prob]
             y_pred = np.array([np.where(y_prob[i] == np.max(y_prob[i]))[0].tolist() for i in range(len(y_prob))]).flatten()
         else:
             y_prob = prob
             y_pred = np.array([np.where(y_prob[i]==np.max(y_prob[i]))[0].tolist() for i in range(len(y_prob))]).flatten()
-    return y_pred
+    return np.array(y_pred)
 
 
 def y_pred_to_categorical(model, X_test, y_test):
     try:
         n_classes = len(np.unique(y_test, axis = 0))
     except:
         n_classes = len(np.unique(y_test))
```

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/lossFuncInfo.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/lossFuncInfo.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/metricsLightgbm.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/metricsLightgbm.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/modelEvaluation.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/modelEvaluation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from sklearn.metrics import accuracy_score, precision_score, recall_score, f1_score
 from sklearn.metrics import mean_absolute_error, mean_squared_error, r2_score, mean_absolute_percentage_error
 import numpy as np
 
+from Accuinsight.modeler.core.get_for_visual import y_pred_reshape, y_test_reshape
+
 
 def calculate_regression_metrics(model, x_val, y_true):
     y_pred = model.predict(x_val)
 
     metrics = {
         'mae': mean_absolute_error(y_true, y_pred),
         'mse': mean_squared_error(y_true, y_pred),
@@ -14,31 +16,41 @@
         'mape': mean_absolute_percentage_error(y_true, y_pred),
     }
 
     return metrics
 
 
 def calculate_classification_metrics(model, x_val, y_true, average=None):
-    y_pred_prob = model.predict(x_val)
-    y_pred = np.argmax(y_pred_prob, axis=-1)
+    y_pred = y_pred_reshape(model, x_val)
+    y_true = y_test_reshape(y_true)
+
+    print("y_true shape:", y_true.shape)
+    print("y_pred shape:", y_pred.shape)
+    result = {
+        "y_true": y_true,
+        "y_pred": y_pred
+    }
 
+    print(result)
     if len(np.unique(y_true)) > 2:
         # 다중 클래스 분류
+        print("다중 클래스")
         accuracy = accuracy_score(y_true, y_pred)
         precision = precision_score(y_true, y_pred, average=average)
         recall = recall_score(y_true, y_pred, average=average)
         f1score = f1_score(y_true, y_pred, average=average)
     else:
         # 이진 분류
+        print("이진 클래스")
         accuracy = accuracy_score(y_true, y_pred)
         precision = precision_score(y_true, y_pred, average=average, pos_label=1)
         recall = recall_score(y_true, y_pred, average=average, pos_label=1)
         f1score = f1_score(y_true, y_pred, average=average, pos_label=1)
 
     metrics = {
         'accuracy': accuracy,
         'precision': precision,
         'recall': recall,
         'f1score': f1score
     }
 
-    return metrics
+    return metrics
```

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/core/path.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/core/path.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,17 @@
         merged_list = list(itertools.chain.from_iterable(trial_num_list))
         merged_list = list(map(int, merged_list))
         trial_num = str(max(merged_list))
 
     else:
         trial_num_list = [get.trial_number_all(i, 'json') for i in path_list if 'json' in i]
         trial_num = str(max(trial_num_list))
-    
+    ## 모델 평가시 trial_num 별도 생성
+    ## 모델 학습없이 평가만 진행할 경우 trial_num 안올라가는 경우 생김
+
     ## 최종 path
     if len(path_list) == 3:     # ML & Regression
         json_file_name_model = json_path_model + '/' + get.model_type(model_name) + '-' + trial_num + '.json'
         json_file_name_shap = json_path_shap + '/' + get.model_type(model_name) + '-shap-' + trial_num + '.json'
         evl_file_name_path = evl_path + '/' + get.model_type(model_name) + '-evl-' + trial_num + '.json'
 
         dir_dict = {'home_path': home,
```

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/entities/_modeler_object.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/_modeler_object.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/entities/alarm.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/alarm.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/entities/lc_artifact.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/lc_artifact.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/entities/lc_metric.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/lc_metric.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/entities/lc_param.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/lc_param.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/entities/lc_run.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/lc_run.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/entities/lc_run_info.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/lc_run_info.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/entities/lc_run_status.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/lc_run_status.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/entities/lc_run_tag.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/lc_run_tag.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/entities/lc_stage.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/lc_stage.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/entities/lc_view_type.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/lc_view_type.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/entities/monitoring_deploy_log.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/monitoring_deploy_log.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/entities/workspace_run_log.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/entities/workspace_run_log.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/exceptions.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/exceptions.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/protos/life_cycle_pb2.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/protos/life_cycle_pb2.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/protos/service_pb2.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/protos/service_pb2.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/protos/skapi_pb2.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/protos/skapi_pb2.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/protos_bak/life_cycle_pb2.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/protos_bak/life_cycle_pb2.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/protos_bak/service_pb2.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/protos_bak/service_pb2.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/protos_bak/skapi_pb2.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/protos_bak/skapi_pb2.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/store/tracking/lc_abstract_store.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/store/tracking/lc_abstract_store.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/store/tracking/life_cycle_store.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/store/tracking/life_cycle_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         env_value = get_os_env()
         project_id = str(env_value[LcConst.ENV_PROJECT_ID])
         workspace_id = str(env_value[LcConst.ENV_WORKSPACE_ID])
         experiment_id = str(env_value[LcConst.ENV_EXPERIMENT_ID])
         user_id = str(env_value[LcConst.ENV_USER_SSO_ID])  # owner id
 
         if current_run_meta[LcConst.RUN_OBJ_IS_EVALUATION]=="false":
-            print("여기로 오나요? 오지말아요~~~ 여긴 모델 생성이에요 두둠칫")
+            print("training model.")
             with open(current_run_meta[LcConst.RUN_RESULT_PATH][LcConst.RUN_MODEL_JSON_PATH]) as run_json_file:
                 json_data = json.load(run_json_file)
 
                 try:
                     user_id = json_data['user_id']
                 except KeyError:
                     pass
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/store/tracking/monitoring_deploy_store.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/store/tracking/monitoring_deploy_store.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/store/tracking/workspace_store.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/store/tracking/workspace_store.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/utils/__init__.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/utils/dependency/dependencies.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/utils/dependency/dependencies.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/utils/dependency/settings.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/utils/dependency/settings.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/utils/dl_utils.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/utils/dl_utils.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/utils/os_getenv.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/utils/os_getenv.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/utils/proto_json_utils.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/utils/proto_json_utils.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/utils/rest_utils.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/utils/rest_utils.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight/modeler/utils/runs_utils.py` & `Accuinsight-3.4.230516rc1/Accuinsight/modeler/utils/runs_utils.py`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight.egg-info/PKG-INFO` & `Accuinsight-3.4.230516rc1/Accuinsight.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Accuinsight
-Version: 3.4.230426rc0
+Version: 3.4.230516rc1
 Summary: Model life cycle and monitoring library in Accuinsight+
 Home-page: 
 Author: SK
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `Accuinsight-3.4.230426rc0/Accuinsight.egg-info/SOURCES.txt` & `Accuinsight-3.4.230516rc1/Accuinsight.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -53,17 +53,20 @@
 Accuinsight/modeler/core/Run/__init__.py
 Accuinsight/modeler/core/Run/ParseRun/BaseParser.py
 Accuinsight/modeler/core/Run/ParseRun/ParseExperiment.py
 Accuinsight/modeler/core/Run/ParseRun/ParseKeras.py
 Accuinsight/modeler/core/Run/ParseRun/Parse_DLClassification.py
 Accuinsight/modeler/core/Run/ParseRun/Parse_DLClassification_evl.py
 Accuinsight/modeler/core/Run/ParseRun/Parse_DLRegression.py
+Accuinsight/modeler/core/Run/ParseRun/Parse_DLRegression_evl.py
 Accuinsight/modeler/core/Run/ParseRun/Parse_Helper.py
 Accuinsight/modeler/core/Run/ParseRun/Parse_MLClassifier.py
+Accuinsight/modeler/core/Run/ParseRun/Parse_MLClassifier_evl.py
 Accuinsight/modeler/core/Run/ParseRun/Parse_MLRegression.py
+Accuinsight/modeler/core/Run/ParseRun/Parse_MLRegression_evl.py
 Accuinsight/modeler/core/Run/ParseRun/ParserVisualJaon.py
 Accuinsight/modeler/core/Run/ParseRun/__init__.py
 Accuinsight/modeler/core/Run/RunInfo/RunInfo.py
 Accuinsight/modeler/core/Run/RunInfo/__init__.py
 Accuinsight/modeler/entities/__init__.py
 Accuinsight/modeler/entities/_modeler_object.py
 Accuinsight/modeler/entities/alarm.py
```

### Comparing `Accuinsight-3.4.230426rc0/PKG-INFO` & `Accuinsight-3.4.230516rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Accuinsight
-Version: 3.4.230426rc0
+Version: 3.4.230516rc1
 Summary: Model life cycle and monitoring library in Accuinsight+
 Home-page: 
 Author: SK
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `Accuinsight-3.4.230426rc0/README.rst` & `Accuinsight-3.4.230516rc1/README.rst`

 * *Files identical despite different names*

### Comparing `Accuinsight-3.4.230426rc0/setup.py` & `Accuinsight-3.4.230516rc1/setup.py`

 * *Files identical despite different names*

