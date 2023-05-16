# Comparing `tmp/simses-1.3.2.tar.gz` & `tmp/simses-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simses-1.3.2.tar", last modified: Fri Feb 10 10:09:29 2023, max compression
+gzip compressed data, was "simses-1.3.3.tar", last modified: Tue May 16 14:07:41 2023, max compression
```

## Comparing `simses-1.3.2.tar` & `simses-1.3.3.tar`

### file list

```diff
@@ -1,790 +1,785 @@
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:29.633844 simses-1.3.2/
--rw-rw-rw-   0        0        0     1647 2023-02-10 09:26:04.000000 simses-1.3.2/LICENSE.txt
--rw-rw-rw-   0        0        0      158 2023-02-08 12:59:18.000000 simses-1.3.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1067 2023-02-10 10:09:29.632248 simses-1.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     1442 2022-01-26 22:48:49.000000 simses-1.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:26.716010 simses-1.3.2/doc/
--rw-rw-rw-   0        0        0        0 2023-02-07 13:10:46.000000 simses-1.3.2/doc/__init__.py
--rw-rw-rw-   0        0        0     2915 2023-02-07 13:10:47.000000 simses-1.3.2/doc/conf.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:26.720013 simses-1.3.2/doc/graph/
--rw-rw-rw-   0        0        0        0 2023-02-07 13:10:47.000000 simses-1.3.2/doc/graph/__init__.py
--rw-rw-rw-   0        0        0     4830 2023-02-07 13:10:47.000000 simses-1.3.2/doc/graph/graph.py
--rw-rw-rw-   0        0        0       42 2023-02-10 10:09:29.633844 simses-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1854 2023-02-10 10:05:23.000000 simses-1.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:26.736531 simses-1.3.2/simses/
--rw-rw-rw-   0        0        0        5 2023-02-10 10:05:31.000000 simses-1.3.2/simses/VERSION
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:21.000000 simses-1.3.2/simses/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:26.775268 simses-1.3.2/simses/analysis/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:21.000000 simses-1.3.2/simses/analysis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:26.851113 simses-1.3.2/simses/analysis/data/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:21.000000 simses-1.3.2/simses/analysis/data/__init__.py
--rw-rw-rw-   0        0        0    10671 2023-01-16 13:10:28.000000 simses-1.3.2/simses/analysis/data/abstract_data.py
--rw-rw-rw-   0        0        0     6060 2021-03-15 08:25:21.000000 simses-1.3.2/simses/analysis/data/electrolyzer.py
--rw-rw-rw-   0        0        0     1980 2021-03-15 08:25:21.000000 simses-1.3.2/simses/analysis/data/energy_management.py
--rw-rw-rw-   0        0        0     2543 2021-03-15 08:25:21.000000 simses-1.3.2/simses/analysis/data/fuel_cell.py
--rw-rw-rw-   0        0        0     6598 2021-03-15 08:25:21.000000 simses-1.3.2/simses/analysis/data/hydrogen.py
--rw-rw-rw-   0        0        0     3563 2023-02-07 14:36:41.000000 simses-1.3.2/simses/analysis/data/lithium_ion.py
--rw-rw-rw-   0        0        0     3679 2021-03-15 08:25:21.000000 simses-1.3.2/simses/analysis/data/redox_flow.py
--rw-rw-rw-   0        0        0     6500 2023-02-07 11:51:11.000000 simses-1.3.2/simses/analysis/data/system.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:26.860112 simses-1.3.2/simses/analysis/evaluation/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:21.000000 simses-1.3.2/simses/analysis/evaluation/__init__.py
--rw-rw-rw-   0        0        0     5937 2021-05-03 10:46:34.000000 simses-1.3.2/simses/analysis/evaluation/abstract_evaluation.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:26.864113 simses-1.3.2/simses/analysis/evaluation/economic/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:21.000000 simses-1.3.2/simses/analysis/evaluation/economic/__init__.py
--rw-rw-rw-   0        0        0     7935 2022-11-25 13:12:01.000000 simses-1.3.2/simses/analysis/evaluation/economic/economic_evaluation.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:26.921114 simses-1.3.2/simses/analysis/evaluation/economic/revenue_stream/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:21.000000 simses-1.3.2/simses/analysis/evaluation/economic/revenue_stream/__init__.py
--rw-rw-rw-   0        0        0     3611 2022-11-25 13:12:01.000000 simses-1.3.2/simses/analysis/evaluation/economic/revenue_stream/abstract_revenue_stream.py
--rw-rw-rw-   0        0        0    10705 2022-11-25 13:12:14.000000 simses-1.3.2/simses/analysis/evaluation/economic/revenue_stream/demand_charge_reduction.py
--rw-rw-rw-   0        0        0     4503 2022-11-25 13:12:14.000000 simses-1.3.2/simses/analysis/evaluation/economic/revenue_stream/electricity_consumption.py
--rw-rw-rw-   0        0        0     3452 2022-11-25 13:12:01.000000 simses-1.3.2/simses/analysis/evaluation/economic/revenue_stream/energy_cost_reduction.py
--rw-rw-rw-   0        0        0     4318 2022-11-25 13:12:14.000000 simses-1.3.2/simses/analysis/evaluation/economic/revenue_stream/fcr_revenue_stream.py
--rw-rw-rw-   0        0        0     4453 2023-02-07 16:11:10.000000 simses-1.3.2/simses/analysis/evaluation/economic/revenue_stream/intraday_recharge.py
--rw-rw-rw-   0        0        0     2742 2022-11-25 13:12:01.000000 simses-1.3.2/simses/analysis/evaluation/economic/revenue_stream/operation_and_maintenance.py
--rw-rw-rw-   0        0        0     5668 2023-02-07 14:40:48.000000 simses-1.3.2/simses/analysis/evaluation/merger.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:26.951123 simses-1.3.2/simses/analysis/evaluation/plotting/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:21.000000 simses-1.3.2/simses/analysis/evaluation/plotting/__init__.py
--rw-rw-rw-   0        0        0      514 2021-03-15 08:25:21.000000 simses-1.3.2/simses/analysis/evaluation/plotting/axis.py
--rw-rw-rw-   0        0        0     5130 2021-05-03 10:46:34.000000 simses-1.3.2/simses/analysis/evaluation/plotting/energy_plotting.py
--rw-rw-rw-   0        0        0     3256 2021-04-22 11:53:26.000000 simses-1.3.2/simses/analysis/evaluation/plotting/matplot_plotting.py
--rw-rw-rw-   0        0        0     7441 2022-11-25 13:12:14.000000 simses-1.3.2/simses/analysis/evaluation/plotting/plotly_plotting.py
--rw-rw-rw-   0        0        0     4506 2021-05-03 10:46:34.000000 simses-1.3.2/simses/analysis/evaluation/plotting/plotter.py
--rw-rw-rw-   0        0        0     7765 2021-05-03 10:46:34.000000 simses-1.3.2/simses/analysis/evaluation/plotting/sankey_diagram.py
--rw-rw-rw-   0        0        0     5695 2022-11-25 13:12:14.000000 simses-1.3.2/simses/analysis/evaluation/plotting/sunburst_diagram.py
--rw-rw-rw-   0        0        0    11357 2021-04-22 11:53:26.000000 simses-1.3.2/simses/analysis/evaluation/plotting/system_parameters.py
--rw-rw-rw-   0        0        0     7539 2023-02-07 11:51:11.000000 simses-1.3.2/simses/analysis/evaluation/result.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:26.978201 simses-1.3.2/simses/analysis/evaluation/technical/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:21.000000 simses-1.3.2/simses/analysis/evaluation/technical/__init__.py
--rw-rw-rw-   0        0        0    16301 2021-05-03 10:46:34.000000 simses-1.3.2/simses/analysis/evaluation/technical/electrolyzer.py
--rw-rw-rw-   0        0        0     4496 2021-03-15 08:25:21.000000 simses-1.3.2/simses/analysis/evaluation/technical/fuel_cell.py
--rw-rw-rw-   0        0        0    16450 2021-05-03 10:46:34.000000 simses-1.3.2/simses/analysis/evaluation/technical/hydrogen.py
--rw-rw-rw-   0        0        0     7977 2023-02-07 14:31:15.000000 simses-1.3.2/simses/analysis/evaluation/technical/lithium_ion.py
--rw-rw-rw-   0        0        0     5943 2021-04-13 08:36:54.000000 simses-1.3.2/simses/analysis/evaluation/technical/redox_flow.py
--rw-rw-rw-   0        0        0     9681 2022-11-25 13:12:01.000000 simses-1.3.2/simses/analysis/evaluation/technical/site_level.py
--rw-rw-rw-   0        0        0    17403 2023-02-07 11:51:11.000000 simses-1.3.2/simses/analysis/evaluation/technical/system.py
--rw-rw-rw-   0        0        0    11829 2022-11-25 13:12:01.000000 simses-1.3.2/simses/analysis/evaluation/technical/technical_evaluation.py
--rw-rw-rw-   0        0        0    11807 2023-02-08 12:20:50.000000 simses-1.3.2/simses/analysis/factory.py
--rw-rw-rw-   0        0        0     3346 2021-07-05 16:13:34.000000 simses-1.3.2/simses/analysis/storage.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:26.994125 simses-1.3.2/simses/analysis/test/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:21.000000 simses-1.3.2/simses/analysis/test/__init__.py
--rw-rw-rw-   0        0        0     4929 2022-11-25 13:12:01.000000 simses-1.3.2/simses/analysis/test/test_demand_charge_reduction.py
--rw-rw-rw-   0        0        0     3723 2022-11-25 13:12:01.000000 simses-1.3.2/simses/analysis/test/test_energy_cost_reduction.py
--rw-rw-rw-   0        0        0     3268 2021-03-15 08:25:21.000000 simses-1.3.2/simses/analysis/test/test_fcr_revenue_stream.py
--rw-rw-rw-   0        0        0     3356 2021-03-15 08:25:21.000000 simses-1.3.2/simses/analysis/test/test_intraday_recharge_revenue_stream.py
--rw-rw-rw-   0        0        0    16978 2023-02-07 11:51:11.000000 simses-1.3.2/simses/analysis/test/test_technical_evaluation.py
--rw-rw-rw-   0        0        0     1066 2021-03-15 08:25:21.000000 simses-1.3.2/simses/analysis/utils.py
--rw-rw-rw-   0        0        0     1609 2021-03-15 08:25:21.000000 simses-1.3.2/simses/analysis.defaults.ini
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.008117 simses-1.3.2/simses/commons/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.016114 simses-1.3.2/simses/commons/config/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/config/__init__.py
--rw-rw-rw-   0        0        0     4909 2022-11-25 13:12:14.000000 simses-1.3.2/simses/commons/config/abstract_config.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.063115 simses-1.3.2/simses/commons/config/analysis/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/config/analysis/__init__.py
--rw-rw-rw-   0        0        0      549 2021-04-13 08:36:54.000000 simses-1.3.2/simses/commons/config/analysis/analysis_config.py
--rw-rw-rw-   0        0        0     5265 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/config/analysis/economic.py
--rw-rw-rw-   0        0        0     4645 2021-04-13 08:36:54.000000 simses-1.3.2/simses/commons/config/analysis/general.py
--rw-rw-rw-   0        0        0     1138 2021-04-13 08:36:54.000000 simses-1.3.2/simses/commons/config/analysis/market.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.096120 simses-1.3.2/simses/commons/config/data/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/config/data/__init__.py
--rw-rw-rw-   0        0        0      742 2021-04-13 08:36:54.000000 simses-1.3.2/simses/commons/config/data/auxiliary.py
--rw-rw-rw-   0        0        0     7429 2021-08-20 08:21:35.000000 simses-1.3.2/simses/commons/config/data/battery.py
--rw-rw-rw-   0        0        0      571 2021-04-13 08:36:54.000000 simses-1.3.2/simses/commons/config/data/data_config.py
--rw-rw-rw-   0        0        0     2057 2021-04-13 08:36:54.000000 simses-1.3.2/simses/commons/config/data/electrolyzer.py
--rw-rw-rw-   0        0        0     1900 2021-06-28 14:45:15.000000 simses-1.3.2/simses/commons/config/data/energy_management.py
--rw-rw-rw-   0        0        0     1478 2021-04-13 08:36:54.000000 simses-1.3.2/simses/commons/config/data/fuel_cell.py
--rw-rw-rw-   0        0        0     1481 2021-04-13 08:36:54.000000 simses-1.3.2/simses/commons/config/data/power_electronics.py
--rw-rw-rw-   0        0        0     4119 2021-04-13 08:36:54.000000 simses-1.3.2/simses/commons/config/data/redox_flow.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.108145 simses-1.3.2/simses/commons/config/generation/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/config/generation/__init__.py
--rw-rw-rw-   0        0        0     6251 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/config/generation/analysis.py
--rw-rw-rw-   0        0        0     2220 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/config/generation/generator.py
--rw-rw-rw-   0        0        0    31025 2023-02-07 14:31:15.000000 simses-1.3.2/simses/commons/config/generation/simulation.py
--rw-rw-rw-   0        0        0     1522 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/config/log.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.139408 simses-1.3.2/simses/commons/config/simulation/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/config/simulation/__init__.py
--rw-rw-rw-   0        0        0     5452 2022-11-25 13:12:14.000000 simses-1.3.2/simses/commons/config/simulation/battery.py
--rw-rw-rw-   0        0        0     1175 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/config/simulation/electrolyzer.py
--rw-rw-rw-   0        0        0     4842 2022-11-25 13:12:14.000000 simses-1.3.2/simses/commons/config/simulation/energy_management.py
--rw-rw-rw-   0        0        0     1144 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/config/simulation/fuel_cell.py
--rw-rw-rw-   0        0        0     2203 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/config/simulation/general.py
--rw-rw-rw-   0        0        0     4116 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/config/simulation/hydrogen.py
--rw-rw-rw-   0        0        0     7818 2023-02-07 11:51:11.000000 simses-1.3.2/simses/commons/config/simulation/profile.py
--rw-rw-rw-   0        0        0     1129 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/config/simulation/redox_flow.py
--rw-rw-rw-   0        0        0     1388 2021-06-22 08:13:58.000000 simses-1.3.2/simses/commons/config/simulation/simulation_config.py
--rw-rw-rw-   0        0        0     6105 2021-12-03 10:12:00.000000 simses-1.3.2/simses/commons/config/simulation/system.py
--rw-rw-rw-   0        0        0     5887 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/console_printer.py
--rw-rw-rw-   0        0        0     1775 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/constants.py
--rw-rw-rw-   0        0        0     7169 2021-05-03 10:46:34.000000 simses-1.3.2/simses/commons/csv_standard.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.153216 simses-1.3.2/simses/commons/cycle_detection/
--rw-rw-rw-   0        0        0        2 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/cycle_detection/__init__.py
--rw-rw-rw-   0        0        0     2347 2023-02-07 11:51:11.000000 simses-1.3.2/simses/commons/cycle_detection/cycle_detector.py
--rw-rw-rw-   0        0        0     3294 2023-02-07 11:51:11.000000 simses-1.3.2/simses/commons/cycle_detection/half_cycle_detector.py
--rw-rw-rw-   0        0        0      695 2023-02-07 11:51:11.000000 simses-1.3.2/simses/commons/cycle_detection/no_cycle_detector.py
--rw-rw-rw-   0        0        0     6987 2023-02-07 11:51:11.000000 simses-1.3.2/simses/commons/cycle_detection/rainflow_cycle_detector.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.164166 simses-1.3.2/simses/commons/data/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/data/__init__.py
--rw-rw-rw-   0        0        0     6798 2022-11-25 13:12:14.000000 simses-1.3.2/simses/commons/data/csv_data_handler.py
--rw-rw-rw-   0        0        0     1443 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/data/data_handler.py
--rw-rw-rw-   0        0        0     1183 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/data/no_data_handler.py
--rw-rw-rw-   0        0        0     1654 2021-05-03 10:46:34.000000 simses-1.3.2/simses/commons/error.py
--rw-rw-rw-   0        0        0     1820 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/log.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.168165 simses-1.3.2/simses/commons/profile/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/profile/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.183168 simses-1.3.2/simses/commons/profile/economic/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/profile/economic/__init__.py
--rw-rw-rw-   0        0        0      493 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/profile/economic/constant.py
--rw-rw-rw-   0        0        0      905 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/profile/economic/fcr.py
--rw-rw-rw-   0        0        0      912 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/profile/economic/intraday.py
--rw-rw-rw-   0        0        0      784 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/profile/economic/market.py
--rw-rw-rw-   0        0        0    20696 2023-02-07 11:51:11.000000 simses-1.3.2/simses/commons/profile/file.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.217523 simses-1.3.2/simses/commons/profile/power/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/profile/power/__init__.py
--rw-rw-rw-   0        0        0     1927 2021-04-13 08:36:54.000000 simses-1.3.2/simses/commons/profile/power/alternating.py
--rw-rw-rw-   0        0        0      808 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/profile/power/constant.py
--rw-rw-rw-   0        0        0     1729 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/profile/power/file.py
--rw-rw-rw-   0        0        0      966 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/profile/power/generation.py
--rw-rw-rw-   0        0        0      953 2022-11-25 13:12:01.000000 simses-1.3.2/simses/commons/profile/power/load.py
--rw-rw-rw-   0        0        0      826 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/profile/power/power_profile.py
--rw-rw-rw-   0        0        0     1974 2021-03-19 16:32:54.000000 simses-1.3.2/simses/commons/profile/power/random.py
--rw-rw-rw-   0        0        0      950 2023-02-07 11:51:11.000000 simses-1.3.2/simses/commons/profile/power/v2g_profile.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.233332 simses-1.3.2/simses/commons/profile/technical/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/profile/technical/__init__.py
--rw-rw-rw-   0        0        0     1822 2023-02-07 14:31:15.000000 simses-1.3.2/simses/commons/profile/technical/binary.py
--rw-rw-rw-   0        0        0     2367 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/profile/technical/frequency.py
--rw-rw-rw-   0        0        0      756 2021-11-10 16:36:56.000000 simses-1.3.2/simses/commons/profile/technical/soc.py
--rw-rw-rw-   0        0        0      735 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/profile/technical/technical.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.250205 simses-1.3.2/simses/commons/state/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/state/__init__.py
--rw-rw-rw-   0        0        0     6761 2021-11-10 16:36:56.000000 simses-1.3.2/simses/commons/state/abstract_state.py
--rw-rw-rw-   0        0        0     2243 2022-11-25 13:12:14.000000 simses-1.3.2/simses/commons/state/energy_management.py
--rw-rw-rw-   0        0        0     2476 2021-04-13 08:36:54.000000 simses-1.3.2/simses/commons/state/parameters.py
--rw-rw-rw-   0        0        0    11708 2021-04-13 08:36:54.000000 simses-1.3.2/simses/commons/state/parameters_reader.py
--rw-rw-rw-   0        0        0     8645 2023-02-07 11:51:11.000000 simses-1.3.2/simses/commons/state/system.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.269168 simses-1.3.2/simses/commons/state/technology/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/state/technology/__init__.py
--rw-rw-rw-   0        0        0    12642 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/state/technology/electrolyzer.py
--rw-rw-rw-   0        0        0     6008 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/state/technology/fuel_cell.py
--rw-rw-rw-   0        0        0     3675 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/state/technology/hydrogen.py
--rw-rw-rw-   0        0        0    10784 2023-02-07 14:36:41.000000 simses-1.3.2/simses/commons/state/technology/lithium_ion.py
--rw-rw-rw-   0        0        0     7185 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/state/technology/redox_flow.py
--rw-rw-rw-   0        0        0     2550 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/state/technology/storage.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.283454 simses-1.3.2/simses/commons/test/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/test/__init__.py
--rw-rw-rw-   0        0        0      702 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/test/test_constant_power_profile.py
--rw-rw-rw-   0        0        0     2361 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/test/test_file_power_profile.py
--rw-rw-rw-   0        0        0      849 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/test/test_linear_interpolation.py
--rw-rw-rw-   0        0        0      814 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/test/test_mean_average.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.289169 simses-1.3.2/simses/commons/timeseries/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/timeseries/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.297302 simses-1.3.2/simses/commons/timeseries/average/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/timeseries/average/__init__.py
--rw-rw-rw-   0        0        0      622 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/timeseries/average/average.py
--rw-rw-rw-   0        0        0      507 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/timeseries/average/mean_average.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.307171 simses-1.3.2/simses/commons/timeseries/interpolation/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/timeseries/interpolation/__init__.py
--rw-rw-rw-   0        0        0     1311 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/timeseries/interpolation/interpolation.py
--rw-rw-rw-   0        0        0      782 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/timeseries/interpolation/last_value.py
--rw-rw-rw-   0        0        0      565 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/timeseries/interpolation/linear_interpolation.py
--rw-rw-rw-   0        0        0     1418 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/timeseries/timevalue.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.330166 simses-1.3.2/simses/commons/utils/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/utils/__init__.py
--rw-rw-rw-   0        0        0     7699 2023-02-07 11:51:11.000000 simses-1.3.2/simses/commons/utils/cell_reader.py
--rw-rw-rw-   0        0        0     2227 2021-08-20 08:21:35.000000 simses-1.3.2/simses/commons/utils/converter_comparison.py
--rw-rw-rw-   0        0        0     2092 2021-11-10 16:36:56.000000 simses-1.3.2/simses/commons/utils/count_lines_of_code.py
--rw-rw-rw-   0        0        0     5380 2021-08-20 08:21:35.000000 simses-1.3.2/simses/commons/utils/fitting.py
--rw-rw-rw-   0        0        0     5155 2021-03-15 08:25:21.000000 simses-1.3.2/simses/commons/utils/heatmap.py
--rw-rw-rw-   0        0        0     5198 2021-05-03 10:46:34.000000 simses-1.3.2/simses/commons/utils/max_peak_shaving_limit.py
--rw-rw-rw-   0        0        0     9471 2021-05-03 10:46:34.000000 simses-1.3.2/simses/commons/utils/utilities.py
--rw-rw-rw-   0        0        0     4216 2021-03-15 16:21:05.000000 simses-1.3.2/simses/commons/utils/xml_reader.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.332165 simses-1.3.2/simses/data/
--rw-rw-rw-   0        0        0       97 2021-03-15 08:25:21.000000 simses-1.3.2/simses/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.334169 simses-1.3.2/simses/data/electrolyzer/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:21.000000 simses-1.3.2/simses/data/electrolyzer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.350228 simses-1.3.2/simses/data/electrolyzer/evaluation/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:21.000000 simses-1.3.2/simses/data/electrolyzer/evaluation/__init__.py
--rw-rw-rw-   0        0        0     3394 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/electrolyzer/evaluation/comparison_lut_ana_new_with_afterfitting.py
--rw-rw-rw-   0        0        0     3816 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/electrolyzer/evaluation/comparison_lut_ana_new_without_afterfitting.py
--rw-rw-rw-   0        0        0     3471 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/electrolyzer/evaluation/comparison_lut_no_current_influence_ana_new.py
--rw-rw-rw-   0        0        0     6008 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/electrolyzer/evaluation/multi_dim_regression_current_dens_3rd_best_fit.py
--rw-rw-rw-   0        0        0      336 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/electrolyzer/evaluation/parameters_multi_dim_current_dens_fit_3rd_bestfit.csv
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.376248 simses-1.3.2/simses/data/electrolyzer/lookuptable/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:21.000000 simses-1.3.2/simses/data/electrolyzer/lookuptable/__init__.py
--rw-rw-rw-   0        0        0     7662 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/electrolyzer/lookuptable/activation_overpotential_lookup_alkaline.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.401269 simses-1.3.2/simses/data/electrolyzer/lookuptable/archive/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:21.000000 simses-1.3.2/simses/data/electrolyzer/lookuptable/archive/__init__.py
--rw-rw-rw-   0        0        0  2333800 2021-03-15 08:25:21.000000 simses-1.3.2/simses/data/electrolyzer/lookuptable/archive/activation_overpotential_lookup_alkaline.csv.gz
--rw-rw-rw-   0        0        0   367371 2021-03-15 08:25:22.000000 simses-1.3.2/simses/data/electrolyzer/lookuptable/archive/cell_currentdensity_lookup.csv.gz
--rw-rw-rw-   0        0        0   347857 2021-03-15 08:25:22.000000 simses-1.3.2/simses/data/electrolyzer/lookuptable/archive/cell_voltage_lookup.csv.gz
--rw-rw-rw-   0        0        0  1520365 2021-03-15 08:25:22.000000 simses-1.3.2/simses/data/electrolyzer/lookuptable/archive/cell_voltage_lookup_alkaline.csv.gz
--rw-rw-rw-   0        0        0    29206 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/electrolyzer/lookuptable/archive/polarizationcurve_alkaline.py
--rw-rw-rw-   0        0        0  1693681 2021-03-15 08:25:22.000000 simses-1.3.2/simses/data/electrolyzer/lookuptable/cell_current_lookup_alkaline.gz
--rw-rw-rw-   0        0        0     5835 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/electrolyzer/lookuptable/multi_dim_polarizationcurve.py
--rw-rw-rw-   0        0        0     5857 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/electrolyzer/lookuptable/multi_dim_polarizationcurve_no_current_influence_on_part_pressure.py
--rw-rw-rw-   0        0        0    19149 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/electrolyzer/lookuptable/polarizationcurve1bar.csv
--rw-rw-rw-   0        0        0     3910 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/electrolyzer/lookuptable/polarizationcurve_e_master.py
--rw-rw-rw-   0        0        0    18991 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/electrolyzer/lookuptable/powercurve1bar.csv
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.403247 simses-1.3.2/simses/data/electrolyzer/lookuptable/ui_curves/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/data/electrolyzer/lookuptable/ui_curves/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.414616 simses-1.3.2/simses/data/electrolyzer/lookuptable/ui_curves/activation_overpotential_alkaline/
--rw-rw-rw-   0        0        0      909 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/electrolyzer/lookuptable/ui_curves/activation_overpotential_alkaline/25°C.csv
--rw-rw-rw-   0        0        0      919 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/electrolyzer/lookuptable/ui_curves/activation_overpotential_alkaline/90°C.csv
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/data/electrolyzer/lookuptable/ui_curves/activation_overpotential_alkaline/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.419145 simses-1.3.2/simses/data/electrolyzer/lookuptable/ui_curves/general_alkaline/
--rw-rw-rw-   0        0        0     1084 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/electrolyzer/lookuptable/ui_curves/general_alkaline/GHW 130°C at 30bar.csv
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/data/electrolyzer/lookuptable/ui_curves/general_alkaline/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.435679 simses-1.3.2/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/
--rw-rw-rw-   0        0        0     1324 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/23°C.csv
--rw-rw-rw-   0        0        0     1365 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/35°C.csv
--rw-rw-rw-   0        0        0     1416 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/40°C.csv
--rw-rw-rw-   0        0        0     1479 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/45°C.csv
--rw-rw-rw-   0        0        0     1530 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/53,5°C.csv
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.447621 simses-1.3.2/simses/data/electrolyzer/parameters/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/data/electrolyzer/parameters/__init__.py
--rw-rw-rw-   0        0        0      221 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/electrolyzer/parameters/parameters_alkaline_overvoltage_fit.csv
--rw-rw-rw-   0        0        0      299 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/electrolyzer/parameters/parameters_multi_dim_current_dens_fit.csv
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.463625 simses-1.3.2/simses/data/electrolyzer/regression/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/data/electrolyzer/regression/__init__.py
--rw-rw-rw-   0        0        0  1943227 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/electrolyzer/regression/cell_currentdensity_lookup.csv
--rw-rw-rw-   0        0        0     5615 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/electrolyzer/regression/multi_dim_regression_current_dens.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.466617 simses-1.3.2/simses/data/energy_management/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/data/energy_management/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.498620 simses-1.3.2/simses/data/fuel_cell/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/data/fuel_cell/__init__.py
--rw-rw-rw-   0        0        0    19570 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/fuel_cell/polarizationcurve1bar.csv
--rw-rw-rw-   0        0        0     9977 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/fuel_cell/polarizationcurve_fc_jupiter.py
--rw-rw-rw-   0        0        0     3857 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/fuel_cell/polarizationcurve_fc_master.py
--rw-rw-rw-   0        0        0    35785 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/fuel_cell/polarizationcurve_jupiter.csv
--rw-rw-rw-   0        0        0    19746 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/fuel_cell/powercurve1bar.csv
--rw-rw-rw-   0        0        0    36366 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/fuel_cell/powercurve_jupiter.csv
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.500731 simses-1.3.2/simses/data/lithium_ion/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/data/lithium_ion/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.614479 simses-1.3.2/simses/data/lithium_ion/cell/
--rw-rw-rw-   0        0        0   338005 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/lithium_ion/cell/CLFP_Sony_US26650_OCV.csv
--rw-rw-rw-   0        0        0     1482 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/lithium_ion/cell/CLFP_Sony_US26650_Rint.csv
--rw-rw-rw-   0        0        0      581 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/lithium_ion/cell/CLFP_Sony_US26650_capacity_decrease_param.csv
--rw-rw-rw-   0        0        0      605 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/lithium_ion/cell/CLFP_Sony_US26650_resistance_increase_param.csv
--rw-rw-rw-   0        0        0     2487 2021-12-14 11:12:34.000000 simses-1.3.2/simses/data/lithium_ion/cell/LG_INR18560MJ1_OCV.csv
--rw-rw-rw-   0        0        0    16185 2022-11-25 13:12:01.000000 simses-1.3.2/simses/data/lithium_ion/cell/LG_INR18650MJ1_closs_calendar_aging.csv
--rw-rw-rw-   0        0        0    14576 2022-11-25 13:12:01.000000 simses-1.3.2/simses/data/lithium_ion/cell/LG_INR18650MJ1_closs_cycling_aging.csv
--rw-rw-rw-   0        0        0     7990 2022-11-25 13:12:01.000000 simses-1.3.2/simses/data/lithium_ion/cell/LG_INR18650MJ1_rint_cycling_aging.csv
--rw-rw-rw-   0        0        0     2919 2022-11-25 13:12:01.000000 simses-1.3.2/simses/data/lithium_ion/cell/LTO_LMO_closs_cycling_aging.csv
--rw-rw-rw-   0        0        0     2963 2022-11-25 13:12:01.000000 simses-1.3.2/simses/data/lithium_ion/cell/LTO_LMO_rint_cycling_aging.csv
--rw-rw-rw-   0        0        0     1126 2022-11-25 13:12:01.000000 simses-1.3.2/simses/data/lithium_ion/cell/LTO_NMC_closs_calendar_aging.csv
--rw-rw-rw-   0        0        0     2144 2022-11-25 13:12:01.000000 simses-1.3.2/simses/data/lithium_ion/cell/LTO_NMC_closs_cycling_aging.csv
--rw-rw-rw-   0        0        0     2284 2022-11-25 13:12:01.000000 simses-1.3.2/simses/data/lithium_ion/cell/LTO_NMC_rint_calendar_aging.csv
--rw-rw-rw-   0        0        0     1288 2022-11-25 13:12:01.000000 simses-1.3.2/simses/data/lithium_ion/cell/LTO_NMC_rint_cycling_aging.csv
--rw-rw-rw-   0        0        0     4849 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/lithium_ion/cell/NCA_PanasonicNCR_OCV.csv
--rw-rw-rw-   0        0        0    12237 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/lithium_ion/cell/NCA_PanasonicNCR_Rint.csv
--rw-rw-rw-   0        0        0     1068 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/lithium_ion/cell/NMC_Akasol_OEM_Rint.csv
--rw-rw-rw-   0        0        0     2384 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/lithium_ion/cell/NMC_Molicel_OCV.csv
--rw-rw-rw-   0        0        0    12168 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/lithium_ion/cell/NMC_Molicel_Rint.csv
--rw-rw-rw-   0        0        0    92642 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/lithium_ion/cell/NMC_Molicel_capacity_cal.csv
--rw-rw-rw-   0        0        0    24959 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/lithium_ion/cell/NMC_Molicel_capacity_cyc.csv
--rw-rw-rw-   0        0        0    80843 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/lithium_ion/cell/NMC_Molicel_ri_cal.csv
--rw-rw-rw-   0        0        0    25392 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/lithium_ion/cell/NMC_Molicel_ri_cyc.csv
--rw-rw-rw-   0        0        0    49004 2021-06-22 08:13:58.000000 simses-1.3.2/simses/data/lithium_ion/cell/NMC_Samsung_LabTest_cell_00_OCV.csv
--rw-rw-rw-   0        0        0    15435 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/lithium_ion/cell/NMC_Samsung_LabTest_cell_00_Ri.csv
--rw-rw-rw-   0        0        0      604 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/lithium_ion/cell/NMC_Sanyo_OCV.csv
--rw-rw-rw-   0        0        0    12168 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/lithium_ion/cell/NMC_Sanyo_Rint.csv
--rw-rw-rw-   0        0        0     2979 2021-07-01 15:40:50.000000 simses-1.3.2/simses/data/lithium_ion/cell/Sodium_Ion_OCV_Green_Rock.csv
--rw-rw-rw-   0        0        0     4940 2021-07-30 10:25:33.000000 simses-1.3.2/simses/data/lithium_ion/cell/Sodium_Ion_Rint_Green_Rock.csv
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/data/lithium_ion/cell/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.616397 simses-1.3.2/simses/data/lithium_ion/isea/
--rw-rw-rw-   0        0        0        0 2021-03-15 16:21:05.000000 simses-1.3.2/simses/data/lithium_ion/isea/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.621397 simses-1.3.2/simses/data/logo/
--rw-rw-rw-   0        0        0    36954 2021-03-15 08:25:22.000000 simses-1.3.2/simses/data/logo/SimSES.png
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/data/logo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.630766 simses-1.3.2/simses/data/power_electronics/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/data/power_electronics/__init__.py
--rw-rw-rw-   0        0        0    29262 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/power_electronics/sinamics_S120_efficiency.csv
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.633399 simses-1.3.2/simses/data/profile/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/data/profile/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.635397 simses-1.3.2/simses/data/profile/economic/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/data/profile/economic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.637812 simses-1.3.2/simses/data/profile/power/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/data/profile/power/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.642412 simses-1.3.2/simses/data/profile/technical/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/data/profile/technical/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.645631 simses-1.3.2/simses/data/profile/thermal/
--rw-rw-rw-   0        0        0        0 2021-04-13 08:36:54.000000 simses-1.3.2/simses/data/profile/thermal/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.650632 simses-1.3.2/simses/data/pump/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/data/pump/__init__.py
--rw-rw-rw-   0        0        0      369 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/pump/pump_efficiency_renner_RM1_5_35.csv
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.652632 simses-1.3.2/simses/data/redox_flow/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/data/redox_flow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.674633 simses-1.3.2/simses/data/redox_flow/degradation/
--rw-rw-rw-   0        0        0      560 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/redox_flow/degradation/H2_Current_F1_Schweiss.csv
--rw-rw-rw-   0        0        0      290 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/redox_flow/degradation/H2_Current_F2_Schweiss.csv
--rw-rw-rw-   0        0        0      560 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/redox_flow/degradation/H2_Current_F3_Schweiss.csv
--rw-rw-rw-   0        0        0      243 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/redox_flow/degradation/H2_Current_F4_Schweiss.csv
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/data/redox_flow/degradation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.705631 simses-1.3.2/simses/data/redox_flow/stack/
--rw-rw-rw-   0        0        0      509 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/redox_flow/stack/RFB_cell_data_R.csv
--rw-rw-rw-   0        0        0      343 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/redox_flow/stack/RFB_highperformance_stack_R.csv
--rw-rw-rw-   0        0        0       80 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/redox_flow/stack/SD_HP_Stack.csv
--rw-rw-rw-   0        0        0     2731 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/redox_flow/stack/SHUNT_CellStack_2250_40.csv
--rw-rw-rw-   0        0        0    28277 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/redox_flow/stack/SHUNT_FILE_INDUSTRIAL_STACK_1500W.csv
--rw-rw-rw-   0        0        0    28360 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/redox_flow/stack/SHUNT_FILE_INDUSTRIAL_STACK_9000W.csv
--rw-rw-rw-   0        0        0     5079 2021-05-03 10:46:34.000000 simses-1.3.2/simses/data/redox_flow/stack/SHUNT_HP_Stack.csv
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/data/redox_flow/stack/__init__.py
--rw-rw-rw-   0        0        0     4214 2021-08-20 08:21:35.000000 simses-1.3.2/simses/data.defaults.ini
--rw-rw-rw-   0        0        0      571 2021-07-12 08:01:43.000000 simses-1.3.2/simses/logger.defaults.ini
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.709631 simses-1.3.2/simses/logic/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/logic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.715891 simses-1.3.2/simses/logic/energy_management/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/logic/energy_management/__init__.py
--rw-rw-rw-   0        0        0    10718 2023-02-08 12:36:08.000000 simses-1.3.2/simses/logic/energy_management/energy_management_factory.py
--rw-rw-rw-   0        0        0     2470 2022-11-25 13:12:14.000000 simses-1.3.2/simses/logic/energy_management/energy_management_system.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.725765 simses-1.3.2/simses/logic/energy_management/strategy/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/logic/energy_management/strategy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.771473 simses-1.3.2/simses/logic/energy_management/strategy/basic/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/logic/energy_management/strategy/basic/__init__.py
--rw-rw-rw-   0        0        0     6823 2023-02-07 11:51:11.000000 simses-1.3.2/simses/logic/energy_management/strategy/basic/electric_vehicle.py
--rw-rw-rw-   0        0        0    11070 2023-02-07 16:15:13.000000 simses-1.3.2/simses/logic/energy_management/strategy/basic/electric_vehicle_soc.py
--rw-rw-rw-   0        0        0     6853 2023-02-07 11:51:11.000000 simses-1.3.2/simses/logic/energy_management/strategy/basic/electric_vehicle_v2g.py
--rw-rw-rw-   0        0        0     2234 2022-11-25 13:12:01.000000 simses-1.3.2/simses/logic/energy_management/strategy/basic/ev_charger_with_buffer.py
--rw-rw-rw-   0        0        0     5761 2021-06-22 08:13:58.000000 simses-1.3.2/simses/logic/energy_management/strategy/basic/frequency_containment_reserve.py
--rw-rw-rw-   0        0        0     4102 2021-03-15 08:25:22.000000 simses-1.3.2/simses/logic/energy_management/strategy/basic/intraday_market_recharge.py
--rw-rw-rw-   0        0        0     7724 2021-06-22 08:13:58.000000 simses-1.3.2/simses/logic/energy_management/strategy/basic/peak_shaving_perfect_foresight.py
--rw-rw-rw-   0        0        0     2541 2022-11-25 13:12:01.000000 simses-1.3.2/simses/logic/energy_management/strategy/basic/peak_shaving_simple.py
--rw-rw-rw-   0        0        0     1210 2021-03-15 08:25:22.000000 simses-1.3.2/simses/logic/energy_management/strategy/basic/power_follower.py
--rw-rw-rw-   0        0        0     5228 2022-11-25 13:12:14.000000 simses-1.3.2/simses/logic/energy_management/strategy/basic/residential_pv_feed_in_damp.py
--rw-rw-rw-   0        0        0     1807 2021-08-20 08:33:32.000000 simses-1.3.2/simses/logic/energy_management/strategy/basic/residential_pv_greedy.py
--rw-rw-rw-   0        0        0     1489 2021-03-15 08:25:22.000000 simses-1.3.2/simses/logic/energy_management/strategy/basic/soc_follower.py
--rw-rw-rw-   0        0        0     1501 2021-03-15 08:25:22.000000 simses-1.3.2/simses/logic/energy_management/strategy/basic/use_all_renewable_energy.py
--rw-rw-rw-   0        0        0      281 2021-03-15 08:25:22.000000 simses-1.3.2/simses/logic/energy_management/strategy/operation_priority.py
--rw-rw-rw-   0        0        0     2041 2021-03-15 08:25:22.000000 simses-1.3.2/simses/logic/energy_management/strategy/operation_strategy.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.777498 simses-1.3.2/simses/logic/energy_management/strategy/optimization/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/logic/energy_management/strategy/optimization/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.779727 simses-1.3.2/simses/logic/energy_management/strategy/optimization/forecast_utils/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/logic/energy_management/strategy/optimization/forecast_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.782474 simses-1.3.2/simses/logic/energy_management/strategy/optimization/linearized_models/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/logic/energy_management/strategy/optimization/linearized_models/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.784479 simses-1.3.2/simses/logic/energy_management/strategy/serial/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/logic/energy_management/strategy/serial/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.800209 simses-1.3.2/simses/logic/energy_management/strategy/stacked/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/logic/energy_management/strategy/stacked/__init__.py
--rw-rw-rw-   0        0        0    44067 2023-02-07 14:31:15.000000 simses-1.3.2/simses/logic/energy_management/strategy/stacked/dynamic_multi_use.py
--rw-rw-rw-   0        0        0     1132 2021-03-15 08:25:22.000000 simses-1.3.2/simses/logic/energy_management/strategy/stacked/fcr_idm_recharge_stacked.py
--rw-rw-rw-   0        0        0     1198 2023-02-07 11:51:11.000000 simses-1.3.2/simses/logic/energy_management/strategy/stacked/stacked_operation_strategy.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.849531 simses-1.3.2/simses/logic/power_distribution/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/logic/power_distribution/__init__.py
--rw-rw-rw-   0        0        0     3038 2021-06-22 08:13:58.000000 simses-1.3.2/simses/logic/power_distribution/efficient.py
--rw-rw-rw-   0        0        0      626 2021-06-22 08:13:58.000000 simses-1.3.2/simses/logic/power_distribution/equal.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.853237 simses-1.3.2/simses/logic/power_distribution/optimization_utils/
--rw-rw-rw-   0        0        0       46 2022-11-25 13:12:14.000000 simses-1.3.2/simses/logic/power_distribution/optimization_utils/__init__.py
--rw-rw-rw-   0        0        0     1475 2021-06-22 08:13:58.000000 simses-1.3.2/simses/logic/power_distribution/power_distributor.py
--rw-rw-rw-   0        0        0     1500 2021-06-22 08:13:58.000000 simses-1.3.2/simses/logic/power_distribution/soc.py
--rw-rw-rw-   0        0        0     4106 2021-03-15 08:25:22.000000 simses-1.3.2/simses/logic/power_distribution/state.py
--rw-rw-rw-   0        0        0     9364 2021-06-22 08:13:58.000000 simses-1.3.2/simses/logic/power_distribution/technology.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.902165 simses-1.3.2/simses/logic/test/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/logic/test/__init__.py
--rw-rw-rw-   0        0        0     5066 2023-02-07 16:13:52.000000 simses-1.3.2/simses/logic/test/test_electric_vehicle_SOC_meanpower.py
--rw-rw-rw-   0        0        0     4951 2023-02-07 17:10:28.000000 simses-1.3.2/simses/logic/test/test_electric_vehicle_SOC_original.py
--rw-rw-rw-   0        0        0     5032 2023-02-07 17:10:09.000000 simses-1.3.2/simses/logic/test/test_electric_vehicle_SOC_paused.py
--rw-rw-rw-   0        0        0     4815 2023-02-07 16:49:24.000000 simses-1.3.2/simses/logic/test/test_electric_vehicle_SOC_uncontrolled.py
--rw-rw-rw-   0        0        0     5481 2022-11-25 13:12:01.000000 simses-1.3.2/simses/logic/test/test_electric_vehicle_all_strategies.py
--rw-rw-rw-   0        0        0     4726 2023-02-07 16:49:33.000000 simses-1.3.2/simses/logic/test/test_electric_vehicle_uncontrolled.py
--rw-rw-rw-   0        0        0     1181 2021-10-22 09:09:54.000000 simses-1.3.2/simses/logic/test/test_equal_power_distributor.py
--rw-rw-rw-   0        0        0    22618 2023-02-07 11:51:11.000000 simses-1.3.2/simses/logic/test/test_multi_use.py
--rw-rw-rw-   0        0        0     3169 2021-03-15 08:25:22.000000 simses-1.3.2/simses/logic/test/test_peak_shaving.py
--rw-rw-rw-   0        0        0     3061 2021-03-15 08:25:22.000000 simses-1.3.2/simses/logic/test/test_residential_pv_greedy.py
--rw-rw-rw-   0        0        0     1188 2021-10-22 09:09:54.000000 simses-1.3.2/simses/logic/test/test_soc_based_power_distributor.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.918411 simses-1.3.2/simses/logic/thermal_management/
--rw-rw-rw-   0        0        0        0 2021-08-20 08:21:35.000000 simses-1.3.2/simses/logic/thermal_management/__init__.py
--rw-rw-rw-   0        0        0     4285 2021-12-03 10:12:00.000000 simses-1.3.2/simses/logic/thermal_management/on_off_controller.py
--rw-rw-rw-   0        0        0     5876 2022-11-25 13:12:14.000000 simses-1.3.2/simses/logic/thermal_management/pid_controller.py
--rw-rw-rw-   0        0        0       77 2021-09-03 07:53:22.000000 simses-1.3.2/simses/logic/thermal_management/thermal_management.py
--rw-rw-rw-   0        0        0     9943 2023-01-16 13:10:28.000000 simses-1.3.2/simses/main.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.935767 simses-1.3.2/simses/simulation/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/simulation/__init__.py
--rw-rw-rw-   0        0        0     4368 2021-05-03 10:46:34.000000 simses-1.3.2/simses/simulation/batch_processing.py
--rw-rw-rw-   0        0        0     2937 2021-05-03 10:46:34.000000 simses-1.3.2/simses/simulation/batch_simulation.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.950152 simses-1.3.2/simses/simulation/case_studies/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/simulation/case_studies/__init__.py
--rw-rw-rw-   0        0        0     1419 2021-03-15 08:25:22.000000 simses-1.3.2/simses/simulation/case_studies/case_study_1_peak_shaving.py
--rw-rw-rw-   0        0        0     1930 2021-03-15 08:25:22.000000 simses-1.3.2/simses/simulation/case_studies/case_study_2_fcr.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.951720 simses-1.3.2/simses/simulation/case_studies/configs/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/simulation/case_studies/configs/__init__.py
--rw-rw-rw-   0        0        0     4090 2021-03-15 08:25:22.000000 simses-1.3.2/simses/simulation/example.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.966726 simses-1.3.2/simses/simulation/simbas/
--rw-rw-rw-   0        0        0        0 2021-04-13 08:36:54.000000 simses-1.3.2/simses/simulation/simbas/__init__.py
--rw-rw-rw-   0        0        0       35 2022-11-25 13:12:14.000000 simses-1.3.2/simses/simulation/simbas/cell_config.csv
--rw-rw-rw-   0        0        0     2087 2022-11-25 13:12:14.000000 simses-1.3.2/simses/simulation/simbas/room_tool_reader.py
--rw-rw-rw-   0        0        0     4642 2022-11-25 13:12:14.000000 simses-1.3.2/simses/simulation/simbas/simbas.py
--rw-rw-rw-   0        0        0    10013 2022-11-25 13:12:01.000000 simses-1.3.2/simses/simulation/simulator.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.971861 simses-1.3.2/simses/simulation/system_tests/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/simulation/system_tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.977635 simses-1.3.2/simses/simulation/system_tests/configs/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/simulation/system_tests/configs/__init__.py
--rw-rw-rw-   0        0        0     4971 2021-03-15 08:25:22.000000 simses-1.3.2/simses/simulation/system_tests/system_test.py
--rw-rw-rw-   0        0        0    15019 2023-02-07 16:52:14.000000 simses-1.3.2/simses/simulation.defaults.ini
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:27.996800 simses-1.3.2/simses/system/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:28.003923 simses-1.3.2/simses/system/auxiliary/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/auxiliary/__init__.py
--rw-rw-rw-   0        0        0      889 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/auxiliary/auxiliary.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:28.020877 simses-1.3.2/simses/system/auxiliary/compression/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/auxiliary/compression/__init__.py
--rw-rw-rw-   0        0        0     1088 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/auxiliary/compression/compressor.py
--rw-rw-rw-   0        0        0     1080 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/auxiliary/compression/hydrogen_isentrop.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:28.035802 simses-1.3.2/simses/system/auxiliary/gas_drying/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/auxiliary/gas_drying/__init__.py
--rw-rw-rw-   0        0        0      749 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/auxiliary/gas_drying/gas_dryer.py
--rw-rw-rw-   0        0        0      946 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/auxiliary/gas_drying/hydrogen.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:28.067084 simses-1.3.2/simses/system/auxiliary/heating_ventilation_air_conditioning/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/auxiliary/heating_ventilation_air_conditioning/__init__.py
--rw-rw-rw-   0        0        0      953 2021-11-10 16:36:56.000000 simses-1.3.2/simses/system/auxiliary/heating_ventilation_air_conditioning/fan.py
--rw-rw-rw-   0        0        0     4620 2022-11-25 13:12:01.000000 simses-1.3.2/simses/system/auxiliary/heating_ventilation_air_conditioning/fix_cop_hvac.py
--rw-rw-rw-   0        0        0     8071 2022-11-25 13:12:01.000000 simses-1.3.2/simses/system/auxiliary/heating_ventilation_air_conditioning/fix_cop_hvac_pid_control.py
--rw-rw-rw-   0        0        0     1662 2022-11-25 13:12:01.000000 simses-1.3.2/simses/system/auxiliary/heating_ventilation_air_conditioning/hvac.py
--rw-rw-rw-   0        0        0     1243 2022-11-25 13:12:01.000000 simses-1.3.2/simses/system/auxiliary/heating_ventilation_air_conditioning/no_hvac.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:28.087377 simses-1.3.2/simses/system/auxiliary/pump/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/auxiliary/pump/__init__.py
--rw-rw-rw-   0        0        0     1810 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/auxiliary/pump/abstract_pump.py
--rw-rw-rw-   0        0        0     1144 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/auxiliary/pump/fixeta_centrifugal.py
--rw-rw-rw-   0        0        0     2178 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/auxiliary/pump/scalable_variable_eta_centrifugal.py
--rw-rw-rw-   0        0        0     2300 2021-05-03 10:46:34.000000 simses-1.3.2/simses/system/auxiliary/pump/variable_eta_centrifugal.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:28.098961 simses-1.3.2/simses/system/auxiliary/water_heating/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/auxiliary/water_heating/__init__.py
--rw-rw-rw-   0        0        0      924 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/auxiliary/water_heating/water_heater.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:28.120529 simses-1.3.2/simses/system/dc_coupling/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/dc_coupling/__init__.py
--rw-rw-rw-   0        0        0      448 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/dc_coupling/bus_charging_dc_coupling.py
--rw-rw-rw-   0        0        0      551 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/dc_coupling/bus_charging_profile.py
--rw-rw-rw-   0        0        0     1643 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/dc_coupling/dc_coupler.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:28.134215 simses-1.3.2/simses/system/dc_coupling/generation/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/dc_coupling/generation/__init__.py
--rw-rw-rw-   0        0        0      752 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/dc_coupling/generation/dc_generation.py
--rw-rw-rw-   0        0        0      466 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/dc_coupling/generation/no_dc_generation.py
--rw-rw-rw-   0        0        0     1330 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/dc_coupling/generation/pv_dc_generation.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:28.161136 simses-1.3.2/simses/system/dc_coupling/load/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/dc_coupling/load/__init__.py
--rw-rw-rw-   0        0        0      980 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/dc_coupling/load/dc_bus_charging_fixed.py
--rw-rw-rw-   0        0        0     1372 2021-05-03 10:46:34.000000 simses-1.3.2/simses/system/dc_coupling/load/dc_bus_charging_profile.py
--rw-rw-rw-   0        0        0     2875 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/dc_coupling/load/dc_bus_charging_random.py
--rw-rw-rw-   0        0        0      812 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/dc_coupling/load/dc_load.py
--rw-rw-rw-   0        0        0     1058 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/dc_coupling/load/dc_radio_ups_load.py
--rw-rw-rw-   0        0        0      444 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/dc_coupling/load/no_dc_load.py
--rw-rw-rw-   0        0        0      327 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/dc_coupling/no_dc_coupling.py
--rw-rw-rw-   0        0        0      747 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/dc_coupling/usp_dc_coupling.py
--rw-rw-rw-   0        0        0    37686 2023-02-08 12:17:16.000000 simses-1.3.2/simses/system/factory.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:28.237314 simses-1.3.2/simses/system/housing/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/housing/__init__.py
--rw-rw-rw-   0        0        0     2954 2022-11-25 13:12:14.000000 simses-1.3.2/simses/system/housing/abstract_housing.py
--rw-rw-rw-   0        0        0     7225 2022-11-25 13:12:14.000000 simses-1.3.2/simses/system/housing/forty_ft_container.py
--rw-rw-rw-   0        0        0     3281 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/housing/layer.py
--rw-rw-rw-   0        0        0      453 2021-12-03 10:12:00.000000 simses-1.3.2/simses/system/housing/no_housing.py
--rw-rw-rw-   0        0        0     7218 2022-11-25 13:12:14.000000 simses-1.3.2/simses/system/housing/twenty_ft_container.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:28.247819 simses-1.3.2/simses/system/power_electronics/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/power_electronics/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:28.297211 simses-1.3.2/simses/system/power_electronics/acdc_converter/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/power_electronics/acdc_converter/__init__.py
--rw-rw-rw-   0        0        0     3531 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/power_electronics/acdc_converter/abstract_acdc_converter.py
--rw-rw-rw-   0        0        0     4152 2021-05-03 10:46:35.000000 simses-1.3.2/simses/system/power_electronics/acdc_converter/bonfiglioli.py
--rw-rw-rw-   0        0        0     2296 2021-06-22 08:13:58.000000 simses-1.3.2/simses/system/power_electronics/acdc_converter/fix_efficiency.py
--rw-rw-rw-   0        0        0      407 2021-05-03 10:46:35.000000 simses-1.3.2/simses/system/power_electronics/acdc_converter/no_loss.py
--rw-rw-rw-   0        0        0     3446 2021-05-03 10:46:35.000000 simses-1.3.2/simses/system/power_electronics/acdc_converter/notton.py
--rw-rw-rw-   0        0        0     2821 2021-05-03 10:46:35.000000 simses-1.3.2/simses/system/power_electronics/acdc_converter/notton_loss.py
--rw-rw-rw-   0        0        0     2459 2021-08-20 08:21:35.000000 simses-1.3.2/simses/system/power_electronics/acdc_converter/rampinelli_fit.py
--rw-rw-rw-   0        0        0     3879 2021-05-03 10:46:35.000000 simses-1.3.2/simses/system/power_electronics/acdc_converter/sinamics.py
--rw-rw-rw-   0        0        0     4198 2021-10-06 13:33:06.000000 simses-1.3.2/simses/system/power_electronics/acdc_converter/stable.py
--rw-rw-rw-   0        0        0     4895 2022-11-25 13:12:01.000000 simses-1.3.2/simses/system/power_electronics/acdc_converter/stacked.py
--rw-rw-rw-   0        0        0     8150 2021-05-03 10:46:35.000000 simses-1.3.2/simses/system/power_electronics/acdc_converter/sungrow.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:28.320425 simses-1.3.2/simses/system/power_electronics/dcdc_converter/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/power_electronics/dcdc_converter/__init__.py
--rw-rw-rw-   0        0        0     2423 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/power_electronics/dcdc_converter/abstract_dcdc_converter.py
--rw-rw-rw-   0        0        0     2775 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/power_electronics/dcdc_converter/fix_efficiency.py
--rw-rw-rw-   0        0        0     2299 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/power_electronics/dcdc_converter/no_dcdc.py
--rw-rw-rw-   0        0        0     1847 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/power_electronics/dcdc_converter/no_loss.py
--rw-rw-rw-   0        0        0     6350 2023-02-07 11:51:11.000000 simses-1.3.2/simses/system/power_electronics/electronics.py
--rw-rw-rw-   0        0        0     3575 2022-11-25 13:12:01.000000 simses-1.3.2/simses/system/storage_circuit.py
--rw-rw-rw-   0        0        0     9362 2023-02-07 11:51:11.000000 simses-1.3.2/simses/system/storage_system_ac.py
--rw-rw-rw-   0        0        0     5713 2023-02-07 11:51:11.000000 simses-1.3.2/simses/system/storage_system_dc.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:28.361606 simses-1.3.2/simses/system/test/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/test/__init__.py
--rw-rw-rw-   0        0        0     7277 2023-02-08 12:34:33.000000 simses-1.3.2/simses/system/test/test_acdc_converter.py
--rw-rw-rw-   0        0        0     1387 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/test/test_constant_ambient_temperature.py
--rw-rw-rw-   0        0        0     3571 2022-11-25 13:12:01.000000 simses-1.3.2/simses/system/test/test_fix_cop_hvac.py
--rw-rw-rw-   0        0        0      423 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/test/test_fixeta_centrifugal_pump.py
--rw-rw-rw-   0        0        0     3846 2023-02-07 11:51:11.000000 simses-1.3.2/simses/system/test/test_location_ambient_temperature.py
--rw-rw-rw-   0        0        0     1976 2021-04-13 08:36:54.000000 simses-1.3.2/simses/system/test/test_location_ambient_temperature_profile_check.py
--rw-rw-rw-   0        0        0     4318 2021-04-13 08:36:54.000000 simses-1.3.2/simses/system/test/test_location_solar_irradiation_model.py
--rw-rw-rw-   0        0        0     2801 2021-04-13 08:36:54.000000 simses-1.3.2/simses/system/test/test_location_solar_irradiation_model_profile_check.py
--rw-rw-rw-   0        0        0     2274 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/test/test_notton_acdc_converter.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:28.366252 simses-1.3.2/simses/system/thermal/
--rw-rw-rw-   0        0        0        2 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/thermal/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:28.382724 simses-1.3.2/simses/system/thermal/ambient/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/thermal/ambient/__init__.py
--rw-rw-rw-   0        0        0     1325 2021-11-10 16:36:56.000000 simses-1.3.2/simses/system/thermal/ambient/ambient_thermal_model.py
--rw-rw-rw-   0        0        0     1015 2021-11-10 16:36:56.000000 simses-1.3.2/simses/system/thermal/ambient/constant_temperature.py
--rw-rw-rw-   0        0        0     1654 2021-11-10 16:36:56.000000 simses-1.3.2/simses/system/thermal/ambient/location_temperature.py
--rw-rw-rw-   0        0        0     1585 2023-02-07 11:51:11.000000 simses-1.3.2/simses/system/thermal/ambient/user_battery_temperature.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:28.401655 simses-1.3.2/simses/system/thermal/model/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/thermal/model/__init__.py
--rw-rw-rw-   0        0        0     3545 2023-02-07 11:51:11.000000 simses-1.3.2/simses/system/thermal/model/no_system_thermal_model.py
--rw-rw-rw-   0        0        0     2481 2021-11-10 16:36:56.000000 simses-1.3.2/simses/system/thermal/model/system_thermal_model.py
--rw-rw-rw-   0        0        0    15692 2021-12-03 10:12:00.000000 simses-1.3.2/simses/system/thermal/model/zero_d_room_thermal_model.py
--rw-rw-rw-   0        0        0    23564 2021-12-03 10:12:00.000000 simses-1.3.2/simses/system/thermal/model/zero_d_system_thermal_model.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:28.418829 simses-1.3.2/simses/system/thermal/solar_irradiation/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/system/thermal/solar_irradiation/__init__.py
--rw-rw-rw-   0        0        0    18001 2021-11-10 16:36:56.000000 simses-1.3.2/simses/system/thermal/solar_irradiation/location.py
--rw-rw-rw-   0        0        0      795 2021-11-10 16:36:56.000000 simses-1.3.2/simses/system/thermal/solar_irradiation/no_solar_irradiation.py
--rw-rw-rw-   0        0        0     1464 2021-11-10 16:36:56.000000 simses-1.3.2/simses/system/thermal/solar_irradiation/solar_irradiation_model.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:28.428521 simses-1.3.2/simses/technology/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:28.439053 simses-1.3.2/simses/technology/hydrogen/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:28.454542 simses-1.3.2/simses/technology/hydrogen/control/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/control/__init__.py
--rw-rw-rw-   0        0        0     3315 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/control/management.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:28.481168 simses-1.3.2/simses/technology/hydrogen/control/pressure/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/control/pressure/__init__.py
--rw-rw-rw-   0        0        0     3335 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/control/pressure/ideal_var_cathode.py
--rw-rw-rw-   0        0        0      723 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/control/pressure/no_pressure_controller.py
--rw-rw-rw-   0        0        0      791 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/control/pressure/pressure_controller.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:28.509042 simses-1.3.2/simses/technology/hydrogen/control/thermal/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/control/thermal/__init__.py
--rw-rw-rw-   0        0        0     3633 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/control/thermal/ideal_var_flow.py
--rw-rw-rw-   0        0        0      531 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/control/thermal/no_thermal_controller.py
--rw-rw-rw-   0        0        0      795 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/control/thermal/thermal_controller.py
--rw-rw-rw-   0        0        0     2522 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/control/thermal/var_flow.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:28.519989 simses-1.3.2/simses/technology/hydrogen/electrolyzer/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/electrolyzer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:28.550642 simses-1.3.2/simses/technology/hydrogen/electrolyzer/degradation/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/electrolyzer/degradation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:28.572255 simses-1.3.2/simses/technology/hydrogen/electrolyzer/degradation/calendar/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/electrolyzer/degradation/calendar/__init__.py
--rw-rw-rw-   0        0        0     2105 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/electrolyzer/degradation/calendar/calendar_degradation.py
--rw-rw-rw-   0        0        0      785 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/electrolyzer/degradation/calendar/no_calendar_degradation.py
--rw-rw-rw-   0        0        0     3071 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/electrolyzer/degradation/calendar/pem_analytic.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:28.598159 simses-1.3.2/simses/technology/hydrogen/electrolyzer/degradation/cyclic/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/electrolyzer/degradation/cyclic/__init__.py
--rw-rw-rw-   0        0        0     2123 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/electrolyzer/degradation/cyclic/cyclic_degradation.py
--rw-rw-rw-   0        0        0      796 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/electrolyzer/degradation/cyclic/no_cyclic_degradation.py
--rw-rw-rw-   0        0        0     4542 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/electrolyzer/degradation/cyclic/pem_analytic.py
--rw-rw-rw-   0        0        0     1437 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/electrolyzer/degradation/cyclic/pem_analytic_ptl_coating.py
--rw-rw-rw-   0        0        0     4502 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/electrolyzer/degradation/degradation_model.py
--rw-rw-rw-   0        0        0      728 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/electrolyzer/degradation/no_degradation.py
--rw-rw-rw-   0        0        0     1517 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/electrolyzer/degradation/pem_analytic.py
--rw-rw-rw-   0        0        0     1575 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/electrolyzer/degradation/pem_analytic_ptl_coating.py
--rw-rw-rw-   0        0        0     9672 2022-02-04 16:57:13.000000 simses-1.3.2/simses/technology/hydrogen/electrolyzer/factory.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:28.688424 simses-1.3.2/simses/technology/hydrogen/electrolyzer/pressure/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/electrolyzer/pressure/__init__.py
--rw-rw-rw-   0        0        0     1794 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/electrolyzer/pressure/abstract_model.py
--rw-rw-rw-   0        0        0     2448 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/electrolyzer/pressure/alkaline.py
--rw-rw-rw-   0        0        0     1802 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/electrolyzer/pressure/no_pressure_model.py
--rw-rw-rw-   0        0        0     3656 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/electrolyzer/pressure/var_cathode.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:28.709963 simses-1.3.2/simses/technology/hydrogen/electrolyzer/stack/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/electrolyzer/stack/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:28.736696 simses-1.3.2/simses/technology/hydrogen/electrolyzer/stack/alkaline/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/electrolyzer/stack/alkaline/__init__.py
--rw-rw-rw-   0        0        0    13091 2021-05-03 10:46:35.000000 simses-1.3.2/simses/technology/hydrogen/electrolyzer/stack/alkaline/electrical_model.py
--rw-rw-rw-   0        0        0     8273 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/electrolyzer/stack/alkaline/electrolyzer_model.py
--rw-rw-rw-   0        0        0     1593 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/electrolyzer/stack/alkaline/fluid_model.py
--rw-rw-rw-   0        0        0     1697 2021-05-03 10:46:35.000000 simses-1.3.2/simses/technology/hydrogen/electrolyzer/stack/alkaline/parameters.py
--rw-rw-rw-   0        0        0     1502 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/electrolyzer/stack/alkaline/pressure_model.py
--rw-rw-rw-   0        0        0     1474 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/electrolyzer/stack/no_electrolyzer.py
--rw-rw-rw-   0        0        0     4632 2021-05-03 10:46:35.000000 simses-1.3.2/simses/technology/hydrogen/electrolyzer/stack/pem.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:28.788313 simses-1.3.2/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/__init__.py
--rw-rw-rw-   0        0        0     5244 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/efficiency_curves.py
--rw-rw-rw-   0        0        0     5765 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/electrical_model.py
--rw-rw-rw-   0        0        0     8627 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/electrolyzer_model.py
--rw-rw-rw-   0        0        0      603 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/electrolyzer_model_ptl_coating.py
--rw-rw-rw-   0        0        0     2461 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/fluid_model.py
--rw-rw-rw-   0        0        0     3649 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/membrane_model.py
--rw-rw-rw-   0        0        0     2077 2021-05-03 10:46:35.000000 simses-1.3.2/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/parameters.py
--rw-rw-rw-   0        0        0     3318 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/pressure_model.py
--rw-rw-rw-   0        0        0     5098 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/electrolyzer/stack/stack_model.py
--rw-rw-rw-   0        0        0     5538 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/electrolyzer/system.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:28.819888 simses-1.3.2/simses/technology/hydrogen/electrolyzer/thermal/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/electrolyzer/thermal/__init__.py
--rw-rw-rw-   0        0        0     1691 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/electrolyzer/thermal/abstract_model.py
--rw-rw-rw-   0        0        0     8252 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/electrolyzer/thermal/alkaline.py
--rw-rw-rw-   0        0        0     1352 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/electrolyzer/thermal/no_thermal_model.py
--rw-rw-rw-   0        0        0    12898 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/electrolyzer/thermal/pem.py
--rw-rw-rw-   0        0        0     2594 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/factory.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:28.835898 simses-1.3.2/simses/technology/hydrogen/fuel_cell/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/fuel_cell/__init__.py
--rw-rw-rw-   0        0        0     5007 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/fuel_cell/factory.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:28.863090 simses-1.3.2/simses/technology/hydrogen/fuel_cell/pressure/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/fuel_cell/pressure/__init__.py
--rw-rw-rw-   0        0        0     1527 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/fuel_cell/pressure/no_pressure.py
--rw-rw-rw-   0        0        0     1766 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/fuel_cell/pressure/pressure_model.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:28.882834 simses-1.3.2/simses/technology/hydrogen/fuel_cell/stack/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/fuel_cell/stack/__init__.py
--rw-rw-rw-   0        0        0     3734 2021-05-03 10:46:35.000000 simses-1.3.2/simses/technology/hydrogen/fuel_cell/stack/jupiter.py
--rw-rw-rw-   0        0        0     1208 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/fuel_cell/stack/no_fuel_cell.py
--rw-rw-rw-   0        0        0     3141 2021-05-03 10:46:35.000000 simses-1.3.2/simses/technology/hydrogen/fuel_cell/stack/pem.py
--rw-rw-rw-   0        0        0     2232 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/fuel_cell/stack/stack_model.py
--rw-rw-rw-   0        0        0     3181 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/fuel_cell/system.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:28.911600 simses-1.3.2/simses/technology/hydrogen/fuel_cell/thermal/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/fuel_cell/thermal/__init__.py
--rw-rw-rw-   0        0        0      913 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/fuel_cell/thermal/no_thermal_model.py
--rw-rw-rw-   0        0        0      963 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/fuel_cell/thermal/simple.py
--rw-rw-rw-   0        0        0     1015 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/fuel_cell/thermal/thermal_model.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:28.918493 simses-1.3.2/simses/technology/hydrogen/hydrogen_storage/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/hydrogen_storage/__init__.py
--rw-rw-rw-   0        0        0     1703 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/hydrogen_storage/hydrogen_storage.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:28.929090 simses-1.3.2/simses/technology/hydrogen/hydrogen_storage/pipeline/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/hydrogen_storage/pipeline/__init__.py
--rw-rw-rw-   0        0        0      500 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/hydrogen_storage/pipeline/pipeline.py
--rw-rw-rw-   0        0        0     1062 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/hydrogen_storage/pipeline/simple_pipeline.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:28.937101 simses-1.3.2/simses/technology/hydrogen/hydrogen_storage/pressuretank/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/hydrogen_storage/pressuretank/__init__.py
--rw-rw-rw-   0        0        0     3899 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/hydrogen_storage/pressuretank/pressuretank.py
--rw-rw-rw-   0        0        0     6240 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/system.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:28.954361 simses-1.3.2/simses/technology/hydrogen/test/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/test/__init__.py
--rw-rw-rw-   0        0        0     8265 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/hydrogen/test/test_pem_electrolyzer.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:28.970563 simses-1.3.2/simses/technology/lithium_ion/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/lithium_ion/__init__.py
--rw-rw-rw-   0        0        0     6994 2023-02-07 11:51:11.000000 simses-1.3.2/simses/technology/lithium_ion/battery.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:28.984565 simses-1.3.2/simses/technology/lithium_ion/battery_management_system/
--rw-rw-rw-   0        0        0        2 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/lithium_ion/battery_management_system/__init__.py
--rw-rw-rw-   0        0        0     7748 2023-02-07 14:36:41.000000 simses-1.3.2/simses/technology/lithium_ion/battery_management_system/management_system.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:29.097760 simses-1.3.2/simses/technology/lithium_ion/cell/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/lithium_ion/cell/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:29.117315 simses-1.3.2/simses/technology/lithium_ion/cell/electric/
--rw-rw-rw-   0        0        0        0 2021-03-15 16:21:05.000000 simses-1.3.2/simses/technology/lithium_ion/cell/electric/__init__.py
--rw-rw-rw-   0        0        0     1006 2021-04-13 08:36:54.000000 simses-1.3.2/simses/technology/lithium_ion/cell/electric/default.py
--rw-rw-rw-   0        0        0     3550 2023-02-07 14:36:41.000000 simses-1.3.2/simses/technology/lithium_ion/cell/electric/properties.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:29.170671 simses-1.3.2/simses/technology/lithium_ion/cell/format/
--rw-rw-rw-   0        0        0        0 2021-03-15 16:21:05.000000 simses-1.3.2/simses/technology/lithium_ion/cell/format/__init__.py
--rw-rw-rw-   0        0        0      829 2022-11-25 13:12:01.000000 simses-1.3.2/simses/technology/lithium_ion/cell/format/abstract.py
--rw-rw-rw-   0        0        0      523 2023-02-07 11:51:11.000000 simses-1.3.2/simses/technology/lithium_ion/cell/format/pouch.py
--rw-rw-rw-   0        0        0      555 2022-11-25 13:12:01.000000 simses-1.3.2/simses/technology/lithium_ion/cell/format/prismatic.py
--rw-rw-rw-   0        0        0      593 2022-11-25 13:12:01.000000 simses-1.3.2/simses/technology/lithium_ion/cell/format/round.py
--rw-rw-rw-   0        0        0      298 2022-11-25 13:12:01.000000 simses-1.3.2/simses/technology/lithium_ion/cell/format/round_18650.py
--rw-rw-rw-   0        0        0      298 2022-11-25 13:12:01.000000 simses-1.3.2/simses/technology/lithium_ion/cell/format/round_26650.py
--rw-rw-rw-   0        0        0     1952 2022-11-25 13:12:01.000000 simses-1.3.2/simses/technology/lithium_ion/cell/generic.py
--rw-rw-rw-   0        0        0     3474 2022-11-25 13:12:14.000000 simses-1.3.2/simses/technology/lithium_ion/cell/isea.py
--rw-rw-rw-   0        0        0     5009 2023-02-07 11:51:11.000000 simses-1.3.2/simses/technology/lithium_ion/cell/lfp_sony.py
--rw-rw-rw-   0        0        0      503 2021-07-30 10:25:33.000000 simses-1.3.2/simses/technology/lithium_ion/cell/lfp_sony_generic.py
--rw-rw-rw-   0        0        0     8685 2021-05-03 10:46:35.000000 simses-1.3.2/simses/technology/lithium_ion/cell/lmo_daimler.py
--rw-rw-rw-   0        0        0     5224 2022-11-25 13:12:01.000000 simses-1.3.2/simses/technology/lithium_ion/cell/lto_lmo.py
--rw-rw-rw-   0        0        0     5352 2022-11-25 13:12:01.000000 simses-1.3.2/simses/technology/lithium_ion/cell/lto_nmc.py
--rw-rw-rw-   0        0        0      532 2021-07-30 10:25:33.000000 simses-1.3.2/simses/technology/lithium_ion/cell/nca_panasonic_generic.py
--rw-rw-rw-   0        0        0     5469 2022-11-25 13:12:01.000000 simses-1.3.2/simses/technology/lithium_ion/cell/nca_panasonic_ncr.py
--rw-rw-rw-   0        0        0     4958 2022-11-25 13:12:01.000000 simses-1.3.2/simses/technology/lithium_ion/cell/nmc_lgmj1.py
--rw-rw-rw-   0        0        0     4514 2022-11-25 13:12:01.000000 simses-1.3.2/simses/technology/lithium_ion/cell/nmc_molicel.py
--rw-rw-rw-   0        0        0      518 2021-07-30 10:25:33.000000 simses-1.3.2/simses/technology/lithium_ion/cell/nmc_molicel_generic.py
--rw-rw-rw-   0        0        0     4931 2021-03-16 10:01:15.000000 simses-1.3.2/simses/technology/lithium_ion/cell/nmc_samsung78Ah.py
--rw-rw-rw-   0        0        0     7991 2021-05-03 10:46:35.000000 simses-1.3.2/simses/technology/lithium_ion/cell/nmc_samsung94Ah.py
--rw-rw-rw-   0        0        0     8558 2021-10-22 09:09:54.000000 simses-1.3.2/simses/technology/lithium_ion/cell/nmc_samsung94Ah_hybrid.py
--rw-rw-rw-   0        0        0     5481 2022-11-25 13:12:01.000000 simses-1.3.2/simses/technology/lithium_ion/cell/nmc_sanyo_ur18650e.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:29.181167 simses-1.3.2/simses/technology/lithium_ion/cell/sodium_ion/
--rw-rw-rw-   0        0        0        0 2021-07-01 15:40:50.000000 simses-1.3.2/simses/technology/lithium_ion/cell/sodium_ion/__init__.py
--rw-rw-rw-   0        0        0     5578 2022-11-25 13:12:01.000000 simses-1.3.2/simses/technology/lithium_ion/cell/sodium_ion/sodium_ion_green_rock.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:29.201356 simses-1.3.2/simses/technology/lithium_ion/cell/thermal/
--rw-rw-rw-   0        0        0        0 2021-03-15 16:21:05.000000 simses-1.3.2/simses/technology/lithium_ion/cell/thermal/__init__.py
--rw-rw-rw-   0        0        0      639 2021-03-15 16:21:05.000000 simses-1.3.2/simses/technology/lithium_ion/cell/thermal/default.py
--rw-rw-rw-   0        0        0     2131 2021-03-15 16:21:05.000000 simses-1.3.2/simses/technology/lithium_ion/cell/thermal/properties.py
--rw-rw-rw-   0        0        0    16261 2023-01-16 13:10:28.000000 simses-1.3.2/simses/technology/lithium_ion/cell/type.py
--rw-rw-rw-   0        0        0    15101 2021-12-14 11:12:34.000000 simses-1.3.2/simses/technology/lithium_ion/circuit.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:29.282202 simses-1.3.2/simses/technology/lithium_ion/degradation/
--rw-rw-rw-   0        0        0        2 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/lithium_ion/degradation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:29.387457 simses-1.3.2/simses/technology/lithium_ion/degradation/calendar/
--rw-rw-rw-   0        0        0        2 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/lithium_ion/degradation/calendar/__init__.py
--rw-rw-rw-   0        0        0     3104 2022-11-25 13:12:01.000000 simses-1.3.2/simses/technology/lithium_ion/degradation/calendar/calendar_degradation.py
--rw-rw-rw-   0        0        0     2364 2021-06-22 08:13:58.000000 simses-1.3.2/simses/technology/lithium_ion/degradation/calendar/generic_cell.py
--rw-rw-rw-   0        0        0     2993 2021-07-30 10:25:33.000000 simses-1.3.2/simses/technology/lithium_ion/degradation/calendar/lfp_generic.py
--rw-rw-rw-   0        0        0     5050 2022-11-25 13:12:01.000000 simses-1.3.2/simses/technology/lithium_ion/degradation/calendar/lfp_sony.py
--rw-rw-rw-   0        0        0     3736 2021-06-28 14:45:15.000000 simses-1.3.2/simses/technology/lithium_ion/degradation/calendar/lto_lmo.py
--rw-rw-rw-   0        0        0     3698 2021-06-28 14:45:15.000000 simses-1.3.2/simses/technology/lithium_ion/degradation/calendar/lto_nmc.py
--rw-rw-rw-   0        0        0     2923 2021-07-30 10:25:33.000000 simses-1.3.2/simses/technology/lithium_ion/degradation/calendar/nca_generic.py
--rw-rw-rw-   0        0        0     4689 2021-08-20 08:21:35.000000 simses-1.3.2/simses/technology/lithium_ion/degradation/calendar/nca_panasonicNCR.py
--rw-rw-rw-   0        0        0     3063 2021-07-30 10:25:33.000000 simses-1.3.2/simses/technology/lithium_ion/degradation/calendar/nmc_generic.py
--rw-rw-rw-   0        0        0     3077 2022-01-02 14:18:23.000000 simses-1.3.2/simses/technology/lithium_ion/degradation/calendar/nmc_lgmj1.py
--rw-rw-rw-   0        0        0     4451 2021-08-20 08:21:35.000000 simses-1.3.2/simses/technology/lithium_ion/degradation/calendar/nmc_molicel.py
--rw-rw-rw-   0        0        0     2914 2021-08-20 08:21:35.000000 simses-1.3.2/simses/technology/lithium_ion/degradation/calendar/nmc_sanyo_ur18650e.py
--rw-rw-rw-   0        0        0      790 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/lithium_ion/degradation/calendar/no_calendar_dedradation.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:29.481837 simses-1.3.2/simses/technology/lithium_ion/degradation/cyclic/
--rw-rw-rw-   0        0        0        2 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/lithium_ion/degradation/cyclic/__init__.py
--rw-rw-rw-   0        0        0     3202 2023-01-16 13:10:28.000000 simses-1.3.2/simses/technology/lithium_ion/degradation/cyclic/cyclic_degradation.py
--rw-rw-rw-   0        0        0     2316 2021-06-22 08:13:58.000000 simses-1.3.2/simses/technology/lithium_ion/degradation/cyclic/generic_cell.py
--rw-rw-rw-   0        0        0     4820 2021-07-30 10:25:33.000000 simses-1.3.2/simses/technology/lithium_ion/degradation/cyclic/lfp_generic.py
--rw-rw-rw-   0        0        0     5993 2023-02-07 14:36:41.000000 simses-1.3.2/simses/technology/lithium_ion/degradation/cyclic/lfp_sony.py
--rw-rw-rw-   0        0        0     4560 2022-11-25 13:12:01.000000 simses-1.3.2/simses/technology/lithium_ion/degradation/cyclic/lto_lmo.py
--rw-rw-rw-   0        0        0     4568 2021-06-28 14:45:15.000000 simses-1.3.2/simses/technology/lithium_ion/degradation/cyclic/lto_nmc.py
--rw-rw-rw-   0        0        0     4173 2021-07-30 10:25:33.000000 simses-1.3.2/simses/technology/lithium_ion/degradation/cyclic/nca_generic.py
--rw-rw-rw-   0        0        0     6795 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/lithium_ion/degradation/cyclic/nca_panasonicNCR.py
--rw-rw-rw-   0        0        0     4784 2021-07-30 10:25:33.000000 simses-1.3.2/simses/technology/lithium_ion/degradation/cyclic/nmc_generic.py
--rw-rw-rw-   0        0        0     4700 2022-01-02 14:18:23.000000 simses-1.3.2/simses/technology/lithium_ion/degradation/cyclic/nmc_lgmj1.py
--rw-rw-rw-   0        0        0     6373 2023-01-16 13:10:28.000000 simses-1.3.2/simses/technology/lithium_ion/degradation/cyclic/nmc_molicel.py
--rw-rw-rw-   0        0        0     3885 2023-01-16 13:10:28.000000 simses-1.3.2/simses/technology/lithium_ion/degradation/cyclic/nmc_sanyo_ur18650e.py
--rw-rw-rw-   0        0        0      764 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/lithium_ion/degradation/cyclic/no_cyclic_degradation.py
--rw-rw-rw-   0        0        0     8719 2023-02-07 14:36:41.000000 simses-1.3.2/simses/technology/lithium_ion/degradation/degradation_model.py
--rw-rw-rw-   0        0        0      958 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/lithium_ion/degradation/generic_cell.py
--rw-rw-rw-   0        0        0      933 2021-07-30 10:25:33.000000 simses-1.3.2/simses/technology/lithium_ion/degradation/lfp_generic.py
--rw-rw-rw-   0        0        0     1159 2022-11-25 13:12:01.000000 simses-1.3.2/simses/technology/lithium_ion/degradation/lfp_sony.py
--rw-rw-rw-   0        0        0     1251 2022-11-25 13:12:01.000000 simses-1.3.2/simses/technology/lithium_ion/degradation/lmo_daimler.py
--rw-rw-rw-   0        0        0      853 2021-04-22 11:53:26.000000 simses-1.3.2/simses/technology/lithium_ion/degradation/lto_lmo.py
--rw-rw-rw-   0        0        0      853 2021-04-22 11:53:26.000000 simses-1.3.2/simses/technology/lithium_ion/degradation/lto_nmc.py
--rw-rw-rw-   0        0        0      933 2021-07-30 10:25:33.000000 simses-1.3.2/simses/technology/lithium_ion/degradation/nca_generic.py
--rw-rw-rw-   0        0        0      974 2021-10-22 09:09:54.000000 simses-1.3.2/simses/technology/lithium_ion/degradation/nca_panasonicNCR.py
--rw-rw-rw-   0        0        0      933 2021-07-30 10:25:33.000000 simses-1.3.2/simses/technology/lithium_ion/degradation/nmc_generic.py
--rw-rw-rw-   0        0        0      872 2022-01-02 14:18:23.000000 simses-1.3.2/simses/technology/lithium_ion/degradation/nmc_lgmj1.py
--rw-rw-rw-   0        0        0     1103 2021-10-22 09:09:54.000000 simses-1.3.2/simses/technology/lithium_ion/degradation/nmc_molicel.py
--rw-rw-rw-   0        0        0     1146 2021-10-22 09:09:54.000000 simses-1.3.2/simses/technology/lithium_ion/degradation/nmc_samsung94Ah.py
--rw-rw-rw-   0        0        0      921 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/lithium_ion/degradation/nmc_sanyo_ur18650e.py
--rw-rw-rw-   0        0        0      804 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/lithium_ion/degradation/no_degradation.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:29.499469 simses-1.3.2/simses/technology/lithium_ion/equivalent_circuit_model/
--rw-rw-rw-   0        0        0        4 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/lithium_ion/equivalent_circuit_model/__init__.py
--rw-rw-rw-   0        0        0      527 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/lithium_ion/equivalent_circuit_model/equivalent_circuit.py
--rw-rw-rw-   0        0        0     1861 2023-02-07 14:36:41.000000 simses-1.3.2/simses/technology/lithium_ion/equivalent_circuit_model/rint_model.py
--rw-rw-rw-   0        0        0    16756 2023-02-08 12:28:39.000000 simses-1.3.2/simses/technology/lithium_ion/factory.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:29.514253 simses-1.3.2/simses/technology/lithium_ion/test/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/lithium_ion/test/__init__.py
--rw-rw-rw-   0        0        0     2384 2021-04-13 08:36:54.000000 simses-1.3.2/simses/technology/lithium_ion/test/test_battery.py
--rw-rw-rw-   0        0        0     5158 2023-02-07 16:02:45.000000 simses-1.3.2/simses/technology/lithium_ion/test/test_bms.py
--rw-rw-rw-   0        0        0     2771 2023-02-08 12:28:12.000000 simses-1.3.2/simses/technology/lithium_ion/test/test_type.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:29.521932 simses-1.3.2/simses/technology/redox_flow/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/redox_flow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:29.541874 simses-1.3.2/simses/technology/redox_flow/degradation/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/redox_flow/degradation/__init__.py
--rw-rw-rw-   0        0        0     1657 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/redox_flow/degradation/capacity_degradation.py
--rw-rw-rw-   0        0        0     2873 2021-04-13 08:36:54.000000 simses-1.3.2/simses/technology/redox_flow/degradation/const_hydrogen_current.py
--rw-rw-rw-   0        0        0      541 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/redox_flow/degradation/no_degradation.py
--rw-rw-rw-   0        0        0     4209 2021-05-03 10:46:35.000000 simses-1.3.2/simses/technology/redox_flow/degradation/variable_hydrogen_current.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:29.552280 simses-1.3.2/simses/technology/redox_flow/electrochemical/
--rw-rw-rw-   0        0        0        4 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/redox_flow/electrochemical/__init__.py
--rw-rw-rw-   0        0        0     1017 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/redox_flow/electrochemical/abstract_electrochemical.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:29.561465 simses-1.3.2/simses/technology/redox_flow/electrochemical/control/
--rw-rw-rw-   0        0        0        2 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/redox_flow/electrochemical/control/__init__.py
--rw-rw-rw-   0        0        0    10697 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/redox_flow/electrochemical/control/redox_control_system.py
--rw-rw-rw-   0        0        0     8509 2021-04-13 08:36:54.000000 simses-1.3.2/simses/technology/redox_flow/electrochemical/rint_model.py
--rw-rw-rw-   0        0        0    17184 2021-04-27 11:37:49.000000 simses-1.3.2/simses/technology/redox_flow/factory.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:29.580449 simses-1.3.2/simses/technology/redox_flow/pump_algorithm/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/redox_flow/pump_algorithm/__init__.py
--rw-rw-rw-   0        0        0     4905 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/redox_flow/pump_algorithm/abstract_pump_algorithm.py
--rw-rw-rw-   0        0        0     4324 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/redox_flow/pump_algorithm/constant_pressure_pulsed.py
--rw-rw-rw-   0        0        0     3741 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/redox_flow/pump_algorithm/fix_flow_rate_start_stop.py
--rw-rw-rw-   0        0        0     5153 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/redox_flow/pump_algorithm/stoich_flow_rate.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:29.615091 simses-1.3.2/simses/technology/redox_flow/stack/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/redox_flow/stack/__init__.py
--rw-rw-rw-   0        0        0    10504 2021-04-13 08:36:54.000000 simses-1.3.2/simses/technology/redox_flow/stack/abstract_stack.py
--rw-rw-rw-   0        0        0     8549 2022-11-25 13:12:01.000000 simses-1.3.2/simses/technology/redox_flow/stack/cell_data_stack_5500w.py
--rw-rw-rw-   0        0        0     4627 2021-04-13 08:36:54.000000 simses-1.3.2/simses/technology/redox_flow/stack/dummy_stack_3000w.py
--rw-rw-rw-   0        0        0     4554 2021-04-13 08:36:54.000000 simses-1.3.2/simses/technology/redox_flow/stack/dummy_stack_5500W.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:29.621282 simses-1.3.2/simses/technology/redox_flow/stack/electrolyte/
--rw-rw-rw-   0        0        0        4 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/redox_flow/stack/electrolyte/__init__.py
--rw-rw-rw-   0        0        0     3675 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/redox_flow/stack/electrolyte/abstract_electrolyte.py
--rw-rw-rw-   0        0        0     4086 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/redox_flow/stack/electrolyte/vanadium.py
--rw-rw-rw-   0        0        0     7211 2022-11-25 13:12:01.000000 simses-1.3.2/simses/technology/redox_flow/stack/high_performance_stack_5700W.py
--rw-rw-rw-   0        0        0     5787 2021-05-03 10:46:35.000000 simses-1.3.2/simses/technology/redox_flow/stack/industrial_stack_1500w.py
--rw-rw-rw-   0        0        0     5663 2021-05-03 10:46:35.000000 simses-1.3.2/simses/technology/redox_flow/stack/industrial_stack_9000w.py
--rw-rw-rw-   0        0        0    13481 2021-11-10 16:36:56.000000 simses-1.3.2/simses/technology/redox_flow/system.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:29.629783 simses-1.3.2/simses/technology/redox_flow/test/
--rw-rw-rw-   0        0        0        0 2021-03-15 08:25:22.000000 simses-1.3.2/simses/technology/redox_flow/test/__init__.py
--rw-rw-rw-   0        0        0     3013 2021-04-27 11:37:49.000000 simses-1.3.2/simses/technology/redox_flow/test/test_stack_module.py
--rw-rw-rw-   0        0        0     2749 2022-11-25 13:12:01.000000 simses-1.3.2/simses/technology/storage.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:09:26.765114 simses-1.3.2/simses.egg-info/
--rw-rw-rw-   0        0        0     1067 2023-02-10 10:09:25.000000 simses-1.3.2/simses.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    34778 2023-02-10 10:09:26.000000 simses-1.3.2/simses.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-10 10:09:25.000000 simses-1.3.2/simses.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-02-10 10:09:25.000000 simses-1.3.2/simses.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-02-10 10:09:25.000000 simses-1.3.2/simses.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:41.472790 simses-1.3.3/
+-rw-rw-rw-   0        0        0     1647 2023-02-10 09:26:04.000000 simses-1.3.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      158 2023-02-08 12:59:18.000000 simses-1.3.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1790 2023-05-16 14:07:41.470634 simses-1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1184 2023-05-16 10:48:41.000000 simses-1.3.3/README.md
+-rw-rw-rw-   0        0        0     1099 2023-05-16 14:06:41.000000 simses-1.3.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-16 14:07:41.472790 simses-1.3.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.290157 simses-1.3.3/simses/
+-rw-rw-rw-   0        0        0        5 2023-05-16 12:07:02.000000 simses-1.3.3/simses/VERSION
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.306386 simses-1.3.3/simses/analysis/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.345914 simses-1.3.3/simses/analysis/data/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/data/__init__.py
+-rw-rw-rw-   0        0        0    10671 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/data/abstract_data.py
+-rw-rw-rw-   0        0        0     6060 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/data/electrolyzer.py
+-rw-rw-rw-   0        0        0     1980 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/data/energy_management.py
+-rw-rw-rw-   0        0        0     2543 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/data/fuel_cell.py
+-rw-rw-rw-   0        0        0     6598 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/data/hydrogen.py
+-rw-rw-rw-   0        0        0     3563 2023-03-06 13:30:03.000000 simses-1.3.3/simses/analysis/data/lithium_ion.py
+-rw-rw-rw-   0        0        0     3679 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/data/redox_flow.py
+-rw-rw-rw-   0        0        0     6714 2023-03-06 13:30:03.000000 simses-1.3.3/simses/analysis/data/system.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.363385 simses-1.3.3/simses/analysis/evaluation/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/__init__.py
+-rw-rw-rw-   0        0        0     5937 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/abstract_evaluation.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.369392 simses-1.3.3/simses/analysis/evaluation/economic/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/economic/__init__.py
+-rw-rw-rw-   0        0        0     7935 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/economic/economic_evaluation.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.413443 simses-1.3.3/simses/analysis/evaluation/economic/revenue_stream/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/economic/revenue_stream/__init__.py
+-rw-rw-rw-   0        0        0     3611 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/economic/revenue_stream/abstract_revenue_stream.py
+-rw-rw-rw-   0        0        0    10705 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/economic/revenue_stream/demand_charge_reduction.py
+-rw-rw-rw-   0        0        0     4503 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/economic/revenue_stream/electricity_consumption.py
+-rw-rw-rw-   0        0        0     3452 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/economic/revenue_stream/energy_cost_reduction.py
+-rw-rw-rw-   0        0        0     4318 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/economic/revenue_stream/fcr_revenue_stream.py
+-rw-rw-rw-   0        0        0     4453 2023-03-06 13:30:03.000000 simses-1.3.3/simses/analysis/evaluation/economic/revenue_stream/intraday_recharge.py
+-rw-rw-rw-   0        0        0     2742 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/economic/revenue_stream/operation_and_maintenance.py
+-rw-rw-rw-   0        0        0     5668 2023-03-06 13:30:03.000000 simses-1.3.3/simses/analysis/evaluation/merger.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.454442 simses-1.3.3/simses/analysis/evaluation/plotting/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/plotting/__init__.py
+-rw-rw-rw-   0        0        0      514 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/plotting/axis.py
+-rw-rw-rw-   0        0        0     5130 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/plotting/energy_plotting.py
+-rw-rw-rw-   0        0        0     3256 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/plotting/matplot_plotting.py
+-rw-rw-rw-   0        0        0     7441 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/plotting/plotly_plotting.py
+-rw-rw-rw-   0        0        0     4506 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/plotting/plotter.py
+-rw-rw-rw-   0        0        0     7765 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/plotting/sankey_diagram.py
+-rw-rw-rw-   0        0        0     5695 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/plotting/sunburst_diagram.py
+-rw-rw-rw-   0        0        0    11357 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/plotting/system_parameters.py
+-rw-rw-rw-   0        0        0     7539 2023-03-06 13:30:03.000000 simses-1.3.3/simses/analysis/evaluation/result.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.497442 simses-1.3.3/simses/analysis/evaluation/technical/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/technical/__init__.py
+-rw-rw-rw-   0        0        0    16301 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/technical/electrolyzer.py
+-rw-rw-rw-   0        0        0     4496 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/technical/fuel_cell.py
+-rw-rw-rw-   0        0        0    16450 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/technical/hydrogen.py
+-rw-rw-rw-   0        0        0     7977 2023-03-06 13:30:03.000000 simses-1.3.3/simses/analysis/evaluation/technical/lithium_ion.py
+-rw-rw-rw-   0        0        0     5943 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/technical/redox_flow.py
+-rw-rw-rw-   0        0        0     9681 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/technical/site_level.py
+-rw-rw-rw-   0        0        0    18811 2023-03-06 13:30:03.000000 simses-1.3.3/simses/analysis/evaluation/technical/system.py
+-rw-rw-rw-   0        0        0    11829 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/technical/technical_evaluation.py
+-rw-rw-rw-   0        0        0    11807 2023-05-16 11:18:59.000000 simses-1.3.3/simses/analysis/factory.py
+-rw-rw-rw-   0        0        0     3346 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/storage.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.521447 simses-1.3.3/simses/analysis/test/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/test/__init__.py
+-rw-rw-rw-   0        0        0     4929 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/test/test_demand_charge_reduction.py
+-rw-rw-rw-   0        0        0     3723 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/test/test_energy_cost_reduction.py
+-rw-rw-rw-   0        0        0     3268 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/test/test_fcr_revenue_stream.py
+-rw-rw-rw-   0        0        0     3356 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/test/test_intraday_recharge_revenue_stream.py
+-rw-rw-rw-   0        0        0    16978 2023-03-06 13:30:03.000000 simses-1.3.3/simses/analysis/test/test_technical_evaluation.py
+-rw-rw-rw-   0        0        0     1066 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/utils.py
+-rw-rw-rw-   0        0        0     1609 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis.defaults.ini
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.543444 simses-1.3.3/simses/commons/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.551443 simses-1.3.3/simses/commons/config/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/__init__.py
+-rw-rw-rw-   0        0        0     4909 2023-03-06 13:30:03.000000 simses-1.3.3/simses/commons/config/abstract_config.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.569445 simses-1.3.3/simses/commons/config/analysis/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/analysis/__init__.py
+-rw-rw-rw-   0        0        0      549 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/analysis/analysis_config.py
+-rw-rw-rw-   0        0        0     5265 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/analysis/economic.py
+-rw-rw-rw-   0        0        0     4645 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/analysis/general.py
+-rw-rw-rw-   0        0        0     1138 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/analysis/market.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.606329 simses-1.3.3/simses/commons/config/data/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/data/__init__.py
+-rw-rw-rw-   0        0        0      742 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/data/auxiliary.py
+-rw-rw-rw-   0        0        0     7429 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/data/battery.py
+-rw-rw-rw-   0        0        0      571 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/data/data_config.py
+-rw-rw-rw-   0        0        0     2057 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/data/electrolyzer.py
+-rw-rw-rw-   0        0        0     1900 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/data/energy_management.py
+-rw-rw-rw-   0        0        0     1478 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/data/fuel_cell.py
+-rw-rw-rw-   0        0        0     1481 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/data/power_electronics.py
+-rw-rw-rw-   0        0        0     4119 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/data/redox_flow.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.622492 simses-1.3.3/simses/commons/config/generation/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/generation/__init__.py
+-rw-rw-rw-   0        0        0     6251 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/generation/analysis.py
+-rw-rw-rw-   0        0        0     2220 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/generation/generator.py
+-rw-rw-rw-   0        0        0    34101 2023-05-15 14:47:15.000000 simses-1.3.3/simses/commons/config/generation/simulation.py
+-rw-rw-rw-   0        0        0     1522 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/log.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.658491 simses-1.3.3/simses/commons/config/simulation/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/simulation/__init__.py
+-rw-rw-rw-   0        0        0     5452 2023-03-06 13:30:03.000000 simses-1.3.3/simses/commons/config/simulation/battery.py
+-rw-rw-rw-   0        0        0     1175 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/simulation/electrolyzer.py
+-rw-rw-rw-   0        0        0     5372 2023-05-15 14:47:15.000000 simses-1.3.3/simses/commons/config/simulation/energy_management.py
+-rw-rw-rw-   0        0        0     1144 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/simulation/fuel_cell.py
+-rw-rw-rw-   0        0        0     2203 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/simulation/general.py
+-rw-rw-rw-   0        0        0     4116 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/simulation/hydrogen.py
+-rw-rw-rw-   0        0        0     7818 2023-03-06 13:30:03.000000 simses-1.3.3/simses/commons/config/simulation/profile.py
+-rw-rw-rw-   0        0        0     1129 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/simulation/redox_flow.py
+-rw-rw-rw-   0        0        0     1388 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/simulation/simulation_config.py
+-rw-rw-rw-   0        0        0     6105 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/simulation/system.py
+-rw-rw-rw-   0        0        0     5887 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/console_printer.py
+-rw-rw-rw-   0        0        0     1775 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/constants.py
+-rw-rw-rw-   0        0        0     7169 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/csv_standard.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.674491 simses-1.3.3/simses/commons/cycle_detection/
+-rw-rw-rw-   0        0        0        2 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/cycle_detection/__init__.py
+-rw-rw-rw-   0        0        0     2347 2023-03-06 13:30:03.000000 simses-1.3.3/simses/commons/cycle_detection/cycle_detector.py
+-rw-rw-rw-   0        0        0     3294 2023-03-06 13:30:03.000000 simses-1.3.3/simses/commons/cycle_detection/half_cycle_detector.py
+-rw-rw-rw-   0        0        0      695 2023-03-06 13:30:03.000000 simses-1.3.3/simses/commons/cycle_detection/no_cycle_detector.py
+-rw-rw-rw-   0        0        0     6987 2023-03-06 13:30:03.000000 simses-1.3.3/simses/commons/cycle_detection/rainflow_cycle_detector.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.687548 simses-1.3.3/simses/commons/data/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/data/__init__.py
+-rw-rw-rw-   0        0        0     6798 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/data/csv_data_handler.py
+-rw-rw-rw-   0        0        0     1443 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/data/data_handler.py
+-rw-rw-rw-   0        0        0     1183 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/data/no_data_handler.py
+-rw-rw-rw-   0        0        0     1654 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/error.py
+-rw-rw-rw-   0        0        0     1820 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/log.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.696582 simses-1.3.3/simses/commons/profile/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/profile/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.714488 simses-1.3.3/simses/commons/profile/economic/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/profile/economic/__init__.py
+-rw-rw-rw-   0        0        0      493 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/profile/economic/constant.py
+-rw-rw-rw-   0        0        0      905 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/profile/economic/fcr.py
+-rw-rw-rw-   0        0        0      912 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/profile/economic/intraday.py
+-rw-rw-rw-   0        0        0      784 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/profile/economic/market.py
+-rw-rw-rw-   0        0        0    20695 2023-05-16 13:19:22.000000 simses-1.3.3/simses/commons/profile/file.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.761521 simses-1.3.3/simses/commons/profile/power/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/profile/power/__init__.py
+-rw-rw-rw-   0        0        0     1927 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/profile/power/alternating.py
+-rw-rw-rw-   0        0        0      808 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/profile/power/constant.py
+-rw-rw-rw-   0        0        0     1729 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/profile/power/file.py
+-rw-rw-rw-   0        0        0      966 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/profile/power/generation.py
+-rw-rw-rw-   0        0        0      953 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/profile/power/load.py
+-rw-rw-rw-   0        0        0      826 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/profile/power/power_profile.py
+-rw-rw-rw-   0        0        0     1974 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/profile/power/random.py
+-rw-rw-rw-   0        0        0      950 2023-03-06 13:30:03.000000 simses-1.3.3/simses/commons/profile/power/v2g_profile.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.784723 simses-1.3.3/simses/commons/profile/technical/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/profile/technical/__init__.py
+-rw-rw-rw-   0        0        0     1769 2023-03-06 13:30:03.000000 simses-1.3.3/simses/commons/profile/technical/binary.py
+-rw-rw-rw-   0        0        0     2367 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/profile/technical/frequency.py
+-rw-rw-rw-   0        0        0      756 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/profile/technical/soc.py
+-rw-rw-rw-   0        0        0      735 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/profile/technical/technical.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.817481 simses-1.3.3/simses/commons/state/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/state/__init__.py
+-rw-rw-rw-   0        0        0     6761 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/state/abstract_state.py
+-rw-rw-rw-   0        0        0     2777 2023-03-06 13:30:03.000000 simses-1.3.3/simses/commons/state/energy_management.py
+-rw-rw-rw-   0        0        0     2476 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/state/parameters.py
+-rw-rw-rw-   0        0        0    11708 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/state/parameters_reader.py
+-rw-rw-rw-   0        0        0     9283 2023-03-06 13:30:03.000000 simses-1.3.3/simses/commons/state/system.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.850246 simses-1.3.3/simses/commons/state/technology/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/state/technology/__init__.py
+-rw-rw-rw-   0        0        0    12642 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/state/technology/electrolyzer.py
+-rw-rw-rw-   0        0        0     6008 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/state/technology/fuel_cell.py
+-rw-rw-rw-   0        0        0     3675 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/state/technology/hydrogen.py
+-rw-rw-rw-   0        0        0    10784 2023-03-06 13:30:03.000000 simses-1.3.3/simses/commons/state/technology/lithium_ion.py
+-rw-rw-rw-   0        0        0     7185 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/state/technology/redox_flow.py
+-rw-rw-rw-   0        0        0     2550 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/state/technology/storage.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.882531 simses-1.3.3/simses/commons/test/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/test/__init__.py
+-rw-rw-rw-   0        0        0      702 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/test/test_constant_power_profile.py
+-rw-rw-rw-   0        0        0     2361 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/test/test_file_power_profile.py
+-rw-rw-rw-   0        0        0      849 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/test/test_linear_interpolation.py
+-rw-rw-rw-   0        0        0      814 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/test/test_mean_average.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.896212 simses-1.3.3/simses/commons/timeseries/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/timeseries/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.908110 simses-1.3.3/simses/commons/timeseries/average/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/timeseries/average/__init__.py
+-rw-rw-rw-   0        0        0      622 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/timeseries/average/average.py
+-rw-rw-rw-   0        0        0      507 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/timeseries/average/mean_average.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.942784 simses-1.3.3/simses/commons/timeseries/interpolation/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/timeseries/interpolation/__init__.py
+-rw-rw-rw-   0        0        0     1311 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/timeseries/interpolation/interpolation.py
+-rw-rw-rw-   0        0        0      782 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/timeseries/interpolation/last_value.py
+-rw-rw-rw-   0        0        0      565 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/timeseries/interpolation/linear_interpolation.py
+-rw-rw-rw-   0        0        0     1418 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/timeseries/timevalue.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:36.070312 simses-1.3.3/simses/commons/utils/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/utils/__init__.py
+-rw-rw-rw-   0        0        0     7923 2023-05-15 14:47:15.000000 simses-1.3.3/simses/commons/utils/cell_reader.py
+-rw-rw-rw-   0        0        0     2227 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/utils/converter_comparison.py
+-rw-rw-rw-   0        0        0     2092 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/utils/count_lines_of_code.py
+-rw-rw-rw-   0        0        0     5380 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/utils/fitting.py
+-rw-rw-rw-   0        0        0     5155 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/utils/heatmap.py
+-rw-rw-rw-   0        0        0     5198 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/utils/max_peak_shaving_limit.py
+-rw-rw-rw-   0        0        0     9471 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/utils/utilities.py
+-rw-rw-rw-   0        0        0     4300 2023-05-15 14:47:15.000000 simses-1.3.3/simses/commons/utils/xml_reader.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:36.077321 simses-1.3.3/simses/data/
+-rw-rw-rw-   0        0        0       97 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:36.081391 simses-1.3.3/simses/data/electrolyzer/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:36.380889 simses-1.3.3/simses/data/electrolyzer/evaluation/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/evaluation/__init__.py
+-rw-rw-rw-   0        0        0     3394 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/evaluation/comparison_lut_ana_new_with_afterfitting.py
+-rw-rw-rw-   0        0        0     3816 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/evaluation/comparison_lut_ana_new_without_afterfitting.py
+-rw-rw-rw-   0        0        0     3471 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/evaluation/comparison_lut_no_current_influence_ana_new.py
+-rw-rw-rw-   0        0        0     6008 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/evaluation/multi_dim_regression_current_dens_3rd_best_fit.py
+-rw-rw-rw-   0        0        0      336 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/evaluation/parameters_multi_dim_current_dens_fit_3rd_bestfit.csv
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:36.671082 simses-1.3.3/simses/data/electrolyzer/lookuptable/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/__init__.py
+-rw-rw-rw-   0        0        0     7662 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/activation_overpotential_lookup_alkaline.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:36.842972 simses-1.3.3/simses/data/electrolyzer/lookuptable/archive/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/archive/__init__.py
+-rw-rw-rw-   0        0        0  2333800 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/archive/activation_overpotential_lookup_alkaline.csv.gz
+-rw-rw-rw-   0        0        0   367371 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/archive/cell_currentdensity_lookup.csv.gz
+-rw-rw-rw-   0        0        0   347857 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/archive/cell_voltage_lookup.csv.gz
+-rw-rw-rw-   0        0        0  1520365 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/archive/cell_voltage_lookup_alkaline.csv.gz
+-rw-rw-rw-   0        0        0    29206 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/archive/polarizationcurve_alkaline.py
+-rw-rw-rw-   0        0        0  1693681 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/cell_current_lookup_alkaline.gz
+-rw-rw-rw-   0        0        0     5835 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/multi_dim_polarizationcurve.py
+-rw-rw-rw-   0        0        0     5857 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/multi_dim_polarizationcurve_no_current_influence_on_part_pressure.py
+-rw-rw-rw-   0        0        0    19149 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/polarizationcurve1bar.csv
+-rw-rw-rw-   0        0        0     3910 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/polarizationcurve_e_master.py
+-rw-rw-rw-   0        0        0    18991 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/powercurve1bar.csv
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:36.846970 simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:36.882717 simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/activation_overpotential_alkaline/
+-rw-rw-rw-   0        0        0      909 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/activation_overpotential_alkaline/25°C.csv
+-rw-rw-rw-   0        0        0      919 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/activation_overpotential_alkaline/90°C.csv
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/activation_overpotential_alkaline/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:36.912922 simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/general_alkaline/
+-rw-rw-rw-   0        0        0     1084 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/general_alkaline/GHW 130°C at 30bar.csv
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/general_alkaline/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:37.066222 simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/
+-rw-rw-rw-   0        0        0     1324 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/23°C.csv
+-rw-rw-rw-   0        0        0     1365 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/35°C.csv
+-rw-rw-rw-   0        0        0     1416 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/40°C.csv
+-rw-rw-rw-   0        0        0     1479 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/45°C.csv
+-rw-rw-rw-   0        0        0     1530 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/53,5°C.csv
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:37.142303 simses-1.3.3/simses/data/electrolyzer/parameters/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/parameters/__init__.py
+-rw-rw-rw-   0        0        0      221 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/parameters/parameters_alkaline_overvoltage_fit.csv
+-rw-rw-rw-   0        0        0      299 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/parameters/parameters_multi_dim_current_dens_fit.csv
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:37.191954 simses-1.3.3/simses/data/electrolyzer/regression/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/regression/__init__.py
+-rw-rw-rw-   0        0        0  1943227 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/regression/cell_currentdensity_lookup.csv
+-rw-rw-rw-   0        0        0     5615 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/regression/multi_dim_regression_current_dens.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:37.195001 simses-1.3.3/simses/data/energy_management/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/energy_management/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:37.329134 simses-1.3.3/simses/data/fuel_cell/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/fuel_cell/__init__.py
+-rw-rw-rw-   0        0        0    19570 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/fuel_cell/polarizationcurve1bar.csv
+-rw-rw-rw-   0        0        0     9977 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/fuel_cell/polarizationcurve_fc_jupiter.py
+-rw-rw-rw-   0        0        0     3857 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/fuel_cell/polarizationcurve_fc_master.py
+-rw-rw-rw-   0        0        0    35785 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/fuel_cell/polarizationcurve_jupiter.csv
+-rw-rw-rw-   0        0        0    19746 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/fuel_cell/powercurve1bar.csv
+-rw-rw-rw-   0        0        0    36366 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/fuel_cell/powercurve_jupiter.csv
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:37.333220 simses-1.3.3/simses/data/lithium_ion/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/lithium_ion/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.097781 simses-1.3.3/simses/data/lithium_ion/cell/
+-rw-rw-rw-   0        0        0   338005 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/CLFP_Sony_US26650_OCV.csv
+-rw-rw-rw-   0        0        0     1482 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/CLFP_Sony_US26650_Rint.csv
+-rw-rw-rw-   0        0        0      581 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/CLFP_Sony_US26650_capacity_decrease_param.csv
+-rw-rw-rw-   0        0        0      605 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/CLFP_Sony_US26650_resistance_increase_param.csv
+-rw-rw-rw-   0        0        0     2487 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/LG_INR18560MJ1_OCV.csv
+-rw-rw-rw-   0        0        0    16185 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/LG_INR18650MJ1_closs_calendar_aging.csv
+-rw-rw-rw-   0        0        0    14576 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/LG_INR18650MJ1_closs_cycling_aging.csv
+-rw-rw-rw-   0        0        0     7990 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/LG_INR18650MJ1_rint_cycling_aging.csv
+-rw-rw-rw-   0        0        0     2919 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/LTO_LMO_closs_cycling_aging.csv
+-rw-rw-rw-   0        0        0     2963 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/LTO_LMO_rint_cycling_aging.csv
+-rw-rw-rw-   0        0        0     1126 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/LTO_NMC_closs_calendar_aging.csv
+-rw-rw-rw-   0        0        0     2144 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/LTO_NMC_closs_cycling_aging.csv
+-rw-rw-rw-   0        0        0     2284 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/LTO_NMC_rint_calendar_aging.csv
+-rw-rw-rw-   0        0        0     1288 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/LTO_NMC_rint_cycling_aging.csv
+-rw-rw-rw-   0        0        0     4849 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/NCA_PanasonicNCR_OCV.csv
+-rw-rw-rw-   0        0        0    12237 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/NCA_PanasonicNCR_Rint.csv
+-rw-rw-rw-   0        0        0     1068 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/NMC_Akasol_OEM_Rint.csv
+-rw-rw-rw-   0        0        0     2384 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/NMC_Molicel_OCV.csv
+-rw-rw-rw-   0        0        0    12168 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/NMC_Molicel_Rint.csv
+-rw-rw-rw-   0        0        0    92642 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/NMC_Molicel_capacity_cal.csv
+-rw-rw-rw-   0        0        0    24959 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/NMC_Molicel_capacity_cyc.csv
+-rw-rw-rw-   0        0        0    80843 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/NMC_Molicel_ri_cal.csv
+-rw-rw-rw-   0        0        0    25392 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/NMC_Molicel_ri_cyc.csv
+-rw-rw-rw-   0        0        0    49004 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/NMC_Samsung_LabTest_cell_00_OCV.csv
+-rw-rw-rw-   0        0        0    15435 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/NMC_Samsung_LabTest_cell_00_Ri.csv
+-rw-rw-rw-   0        0        0      604 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/NMC_Sanyo_OCV.csv
+-rw-rw-rw-   0        0        0    12168 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/NMC_Sanyo_Rint.csv
+-rw-rw-rw-   0        0        0     2979 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/Sodium_Ion_OCV_Green_Rock.csv
+-rw-rw-rw-   0        0        0     4940 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/Sodium_Ion_Rint_Green_Rock.csv
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.100786 simses-1.3.3/simses/data/lithium_ion/isea/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/isea/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.112775 simses-1.3.3/simses/data/logo/
+-rw-rw-rw-   0        0        0    36954 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/logo/SimSES.png
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/logo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.141831 simses-1.3.3/simses/data/power_electronics/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/power_electronics/__init__.py
+-rw-rw-rw-   0        0        0    29262 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/power_electronics/sinamics_S120_efficiency.csv
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.145777 simses-1.3.3/simses/data/profile/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/profile/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.149776 simses-1.3.3/simses/data/profile/economic/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/profile/economic/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.173903 simses-1.3.3/simses/data/profile/power/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/profile/power/__init__.py
+-rw-rw-rw-   0        0        0       41 2023-05-16 11:42:41.000000 simses-1.3.3/simses/data/profile/power/mockup_power_load_profile.csv
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.219061 simses-1.3.3/simses/data/profile/technical/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/profile/technical/__init__.py
+-rw-rw-rw-   0        0        0       46 2023-05-16 11:43:00.000000 simses-1.3.3/simses/data/profile/technical/mockup_power_home_profile.csv
+-rw-rw-rw-   0        0        0       58 2023-05-16 11:43:00.000000 simses-1.3.3/simses/data/profile/technical/mockup_power_soc_profile.csv
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.223259 simses-1.3.3/simses/data/profile/thermal/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/profile/thermal/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.252975 simses-1.3.3/simses/data/pump/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/pump/__init__.py
+-rw-rw-rw-   0        0        0      369 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/pump/pump_efficiency_renner_RM1_5_35.csv
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.260984 simses-1.3.3/simses/data/redox_flow/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/redox_flow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.358977 simses-1.3.3/simses/data/redox_flow/degradation/
+-rw-rw-rw-   0        0        0      560 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/redox_flow/degradation/H2_Current_F1_Schweiss.csv
+-rw-rw-rw-   0        0        0      290 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/redox_flow/degradation/H2_Current_F2_Schweiss.csv
+-rw-rw-rw-   0        0        0      560 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/redox_flow/degradation/H2_Current_F3_Schweiss.csv
+-rw-rw-rw-   0        0        0      243 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/redox_flow/degradation/H2_Current_F4_Schweiss.csv
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/redox_flow/degradation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.597946 simses-1.3.3/simses/data/redox_flow/stack/
+-rw-rw-rw-   0        0        0      509 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/redox_flow/stack/RFB_cell_data_R.csv
+-rw-rw-rw-   0        0        0      343 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/redox_flow/stack/RFB_highperformance_stack_R.csv
+-rw-rw-rw-   0        0        0       80 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/redox_flow/stack/SD_HP_Stack.csv
+-rw-rw-rw-   0        0        0     2731 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/redox_flow/stack/SHUNT_CellStack_2250_40.csv
+-rw-rw-rw-   0        0        0    28277 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/redox_flow/stack/SHUNT_FILE_INDUSTRIAL_STACK_1500W.csv
+-rw-rw-rw-   0        0        0    28360 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/redox_flow/stack/SHUNT_FILE_INDUSTRIAL_STACK_9000W.csv
+-rw-rw-rw-   0        0        0     5079 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/redox_flow/stack/SHUNT_HP_Stack.csv
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/redox_flow/stack/__init__.py
+-rw-rw-rw-   0        0        0     4214 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data.defaults.ini
+-rw-rw-rw-   0        0        0      571 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logger.defaults.ini
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.604777 simses-1.3.3/simses/logic/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.627335 simses-1.3.3/simses/logic/energy_management/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/energy_management/__init__.py
+-rw-rw-rw-   0        0        0    10719 2023-05-16 12:36:02.000000 simses-1.3.3/simses/logic/energy_management/energy_management_factory.py
+-rw-rw-rw-   0        0        0     2470 2023-03-06 13:30:03.000000 simses-1.3.3/simses/logic/energy_management/energy_management_system.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.641450 simses-1.3.3/simses/logic/energy_management/strategy/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/energy_management/strategy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.720165 simses-1.3.3/simses/logic/energy_management/strategy/basic/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/energy_management/strategy/basic/__init__.py
+-rw-rw-rw-   0        0        0     9246 2023-05-15 14:47:15.000000 simses-1.3.3/simses/logic/energy_management/strategy/basic/electric_vehicle.py
+-rw-rw-rw-   0        0        0    13078 2023-05-15 14:47:15.000000 simses-1.3.3/simses/logic/energy_management/strategy/basic/electric_vehicle_soc.py
+-rw-rw-rw-   0        0        0     9891 2023-03-06 13:30:03.000000 simses-1.3.3/simses/logic/energy_management/strategy/basic/electric_vehicle_v2g.py
+-rw-rw-rw-   0        0        0     2234 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/energy_management/strategy/basic/ev_charger_with_buffer.py
+-rw-rw-rw-   0        0        0     5761 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/energy_management/strategy/basic/frequency_containment_reserve.py
+-rw-rw-rw-   0        0        0     4102 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/energy_management/strategy/basic/intraday_market_recharge.py
+-rw-rw-rw-   0        0        0     7724 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/energy_management/strategy/basic/peak_shaving_perfect_foresight.py
+-rw-rw-rw-   0        0        0     2541 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/energy_management/strategy/basic/peak_shaving_simple.py
+-rw-rw-rw-   0        0        0     1310 2023-05-15 14:47:15.000000 simses-1.3.3/simses/logic/energy_management/strategy/basic/power_follower.py
+-rw-rw-rw-   0        0        0     5407 2023-05-15 14:47:15.000000 simses-1.3.3/simses/logic/energy_management/strategy/basic/residential_pv_feed_in_damp.py
+-rw-rw-rw-   0        0        0     1807 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/energy_management/strategy/basic/residential_pv_greedy.py
+-rw-rw-rw-   0        0        0     1489 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/energy_management/strategy/basic/soc_follower.py
+-rw-rw-rw-   0        0        0     1501 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/energy_management/strategy/basic/use_all_renewable_energy.py
+-rw-rw-rw-   0        0        0      281 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/energy_management/strategy/operation_priority.py
+-rw-rw-rw-   0        0        0     2041 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/energy_management/strategy/operation_strategy.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.727285 simses-1.3.3/simses/logic/energy_management/strategy/optimization/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/energy_management/strategy/optimization/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.765014 simses-1.3.3/simses/logic/energy_management/strategy/optimization/forecast_utils/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/energy_management/strategy/optimization/forecast_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.800306 simses-1.3.3/simses/logic/energy_management/strategy/optimization/linearized_models/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/energy_management/strategy/optimization/linearized_models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.807397 simses-1.3.3/simses/logic/energy_management/strategy/serial/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/energy_management/strategy/serial/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.853000 simses-1.3.3/simses/logic/energy_management/strategy/stacked/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/energy_management/strategy/stacked/__init__.py
+-rw-rw-rw-   0        0        0     1132 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/energy_management/strategy/stacked/fcr_idm_recharge_stacked.py
+-rw-rw-rw-   0        0        0    44499 2023-03-06 13:30:03.000000 simses-1.3.3/simses/logic/energy_management/strategy/stacked/parallel_multi_use_with_stealing.py
+-rw-rw-rw-   0        0        0     1198 2023-03-06 13:30:03.000000 simses-1.3.3/simses/logic/energy_management/strategy/stacked/stacked_operation_strategy.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.901427 simses-1.3.3/simses/logic/power_distribution/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/power_distribution/__init__.py
+-rw-rw-rw-   0        0        0     3038 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/power_distribution/efficient.py
+-rw-rw-rw-   0        0        0      626 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/power_distribution/equal.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.905450 simses-1.3.3/simses/logic/power_distribution/optimization_utils/
+-rw-rw-rw-   0        0        0       46 2023-03-06 13:30:03.000000 simses-1.3.3/simses/logic/power_distribution/optimization_utils/__init__.py
+-rw-rw-rw-   0        0        0     1475 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/power_distribution/power_distributor.py
+-rw-rw-rw-   0        0        0     1500 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/power_distribution/soc.py
+-rw-rw-rw-   0        0        0     4106 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/power_distribution/state.py
+-rw-rw-rw-   0        0        0     9364 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/power_distribution/technology.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.976313 simses-1.3.3/simses/logic/test/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/test/__init__.py
+-rw-rw-rw-   0        0        0     5066 2023-05-16 11:40:09.000000 simses-1.3.3/simses/logic/test/test_electric_vehicle_SOC_meanpower.py
+-rw-rw-rw-   0        0        0     4951 2023-05-16 11:42:11.000000 simses-1.3.3/simses/logic/test/test_electric_vehicle_SOC_original.py
+-rw-rw-rw-   0        0        0     5032 2023-05-16 11:41:52.000000 simses-1.3.3/simses/logic/test/test_electric_vehicle_SOC_paused.py
+-rw-rw-rw-   0        0        0     4815 2023-05-16 11:41:31.000000 simses-1.3.3/simses/logic/test/test_electric_vehicle_SOC_uncontrolled.py
+-rw-rw-rw-   0        0        0     5481 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/test/test_electric_vehicle_all_strategies.py
+-rw-rw-rw-   0        0        0     4726 2023-05-16 11:42:40.000000 simses-1.3.3/simses/logic/test/test_electric_vehicle_uncontrolled.py
+-rw-rw-rw-   0        0        0     1181 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/test/test_equal_power_distributor.py
+-rw-rw-rw-   0        0        0    21492 2023-03-06 13:30:03.000000 simses-1.3.3/simses/logic/test/test_multi_use.py
+-rw-rw-rw-   0        0        0     3169 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/test/test_peak_shaving.py
+-rw-rw-rw-   0        0        0     3061 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/test/test_residential_pv_greedy.py
+-rw-rw-rw-   0        0        0     1188 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/test/test_soc_based_power_distributor.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.000819 simses-1.3.3/simses/logic/thermal_management/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/thermal_management/__init__.py
+-rw-rw-rw-   0        0        0     4285 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/thermal_management/on_off_controller.py
+-rw-rw-rw-   0        0        0     6005 2023-03-06 13:30:03.000000 simses-1.3.3/simses/logic/thermal_management/pid_controller.py
+-rw-rw-rw-   0        0        0       77 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/thermal_management/thermal_management.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.052293 simses-1.3.3/simses/simses.egg-info/
+-rw-rw-rw-   0        0        0     1790 2023-05-16 14:07:34.000000 simses-1.3.3/simses/simses.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    34826 2023-05-16 14:07:34.000000 simses-1.3.3/simses/simses.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 14:07:34.000000 simses-1.3.3/simses/simses.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2023-05-16 14:07:34.000000 simses-1.3.3/simses/simses.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       57 2023-05-16 14:07:34.000000 simses-1.3.3/simses/simses.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.074368 simses-1.3.3/simses/simulation/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/simulation/__init__.py
+-rw-rw-rw-   0        0        0     4368 2023-02-20 12:50:47.000000 simses-1.3.3/simses/simulation/batch_processing.py
+-rw-rw-rw-   0        0        0     2937 2023-02-20 12:50:47.000000 simses-1.3.3/simses/simulation/batch_simulation.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.087235 simses-1.3.3/simses/simulation/case_studies/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/simulation/case_studies/__init__.py
+-rw-rw-rw-   0        0        0     1419 2023-02-20 12:50:47.000000 simses-1.3.3/simses/simulation/case_studies/case_study_1_peak_shaving.py
+-rw-rw-rw-   0        0        0     1930 2023-02-20 12:50:47.000000 simses-1.3.3/simses/simulation/case_studies/case_study_2_fcr.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.092647 simses-1.3.3/simses/simulation/case_studies/configs/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/simulation/case_studies/configs/__init__.py
+-rw-rw-rw-   0        0        0     4090 2023-02-20 12:50:47.000000 simses-1.3.3/simses/simulation/example.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.103074 simses-1.3.3/simses/simulation/simbas/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/simulation/simbas/__init__.py
+-rw-rw-rw-   0        0        0     2534 2023-05-15 14:47:15.000000 simses-1.3.3/simses/simulation/simbas/room_tool_reader.py
+-rw-rw-rw-   0        0        0     5577 2023-05-15 14:47:15.000000 simses-1.3.3/simses/simulation/simbas/simbas.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.107736 simses-1.3.3/simses/simulation/simulation_examples/
+-rw-rw-rw-   0        0        0        0 2023-03-06 13:30:03.000000 simses-1.3.3/simses/simulation/simulation_examples/__init__.py
+-rw-rw-rw-   0        0        0    10046 2023-05-15 14:47:15.000000 simses-1.3.3/simses/simulation/simulator.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.114803 simses-1.3.3/simses/simulation/system_tests/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/simulation/system_tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.118620 simses-1.3.3/simses/simulation/system_tests/configs/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/simulation/system_tests/configs/__init__.py
+-rw-rw-rw-   0        0        0     4971 2023-02-20 12:50:47.000000 simses-1.3.3/simses/simulation/system_tests/system_test.py
+-rw-rw-rw-   0        0        0    14759 2023-05-15 14:47:15.000000 simses-1.3.3/simses/simulation.defaults.ini
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.207852 simses-1.3.3/simses/system/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.214056 simses-1.3.3/simses/system/auxiliary/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/auxiliary/__init__.py
+-rw-rw-rw-   0        0        0      889 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/auxiliary/auxiliary.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.274920 simses-1.3.3/simses/system/auxiliary/compression/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/auxiliary/compression/__init__.py
+-rw-rw-rw-   0        0        0     1088 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/auxiliary/compression/compressor.py
+-rw-rw-rw-   0        0        0     1080 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/auxiliary/compression/hydrogen_isentrop.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.286586 simses-1.3.3/simses/system/auxiliary/gas_drying/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/auxiliary/gas_drying/__init__.py
+-rw-rw-rw-   0        0        0      749 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/auxiliary/gas_drying/gas_dryer.py
+-rw-rw-rw-   0        0        0      946 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/auxiliary/gas_drying/hydrogen.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.307474 simses-1.3.3/simses/system/auxiliary/heating_ventilation_air_conditioning/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/auxiliary/heating_ventilation_air_conditioning/__init__.py
+-rw-rw-rw-   0        0        0     1530 2023-03-06 13:30:03.000000 simses-1.3.3/simses/system/auxiliary/heating_ventilation_air_conditioning/fan.py
+-rw-rw-rw-   0        0        0     4567 2023-03-06 13:30:03.000000 simses-1.3.3/simses/system/auxiliary/heating_ventilation_air_conditioning/fix_cop_hvac.py
+-rw-rw-rw-   0        0        0     1662 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/auxiliary/heating_ventilation_air_conditioning/hvac.py
+-rw-rw-rw-   0        0        0     1243 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/auxiliary/heating_ventilation_air_conditioning/no_hvac.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.346623 simses-1.3.3/simses/system/auxiliary/pump/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/auxiliary/pump/__init__.py
+-rw-rw-rw-   0        0        0     1810 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/auxiliary/pump/abstract_pump.py
+-rw-rw-rw-   0        0        0     1144 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/auxiliary/pump/fixeta_centrifugal.py
+-rw-rw-rw-   0        0        0     2178 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/auxiliary/pump/scalable_variable_eta_centrifugal.py
+-rw-rw-rw-   0        0        0     2300 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/auxiliary/pump/variable_eta_centrifugal.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.354167 simses-1.3.3/simses/system/auxiliary/water_heating/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/auxiliary/water_heating/__init__.py
+-rw-rw-rw-   0        0        0      924 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/auxiliary/water_heating/water_heater.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.399513 simses-1.3.3/simses/system/dc_coupling/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/dc_coupling/__init__.py
+-rw-rw-rw-   0        0        0      448 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/dc_coupling/bus_charging_dc_coupling.py
+-rw-rw-rw-   0        0        0      551 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/dc_coupling/bus_charging_profile.py
+-rw-rw-rw-   0        0        0     1643 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/dc_coupling/dc_coupler.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.436697 simses-1.3.3/simses/system/dc_coupling/generation/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/dc_coupling/generation/__init__.py
+-rw-rw-rw-   0        0        0      752 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/dc_coupling/generation/dc_generation.py
+-rw-rw-rw-   0        0        0      466 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/dc_coupling/generation/no_dc_generation.py
+-rw-rw-rw-   0        0        0     1330 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/dc_coupling/generation/pv_dc_generation.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.480867 simses-1.3.3/simses/system/dc_coupling/load/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/dc_coupling/load/__init__.py
+-rw-rw-rw-   0        0        0      980 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/dc_coupling/load/dc_bus_charging_fixed.py
+-rw-rw-rw-   0        0        0     1372 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/dc_coupling/load/dc_bus_charging_profile.py
+-rw-rw-rw-   0        0        0     2875 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/dc_coupling/load/dc_bus_charging_random.py
+-rw-rw-rw-   0        0        0      812 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/dc_coupling/load/dc_load.py
+-rw-rw-rw-   0        0        0     1058 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/dc_coupling/load/dc_radio_ups_load.py
+-rw-rw-rw-   0        0        0      444 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/dc_coupling/load/no_dc_load.py
+-rw-rw-rw-   0        0        0      327 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/dc_coupling/no_dc_coupling.py
+-rw-rw-rw-   0        0        0      747 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/dc_coupling/usp_dc_coupling.py
+-rw-rw-rw-   0        0        0    36968 2023-05-16 12:59:52.000000 simses-1.3.3/simses/system/factory.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.513195 simses-1.3.3/simses/system/housing/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/housing/__init__.py
+-rw-rw-rw-   0        0        0     2954 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/housing/abstract_housing.py
+-rw-rw-rw-   0        0        0     7225 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/housing/forty_ft_container.py
+-rw-rw-rw-   0        0        0     3281 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/housing/layer.py
+-rw-rw-rw-   0        0        0      453 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/housing/no_housing.py
+-rw-rw-rw-   0        0        0     7218 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/housing/twenty_ft_container.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.525795 simses-1.3.3/simses/system/power_electronics/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/power_electronics/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.629219 simses-1.3.3/simses/system/power_electronics/acdc_converter/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/power_electronics/acdc_converter/__init__.py
+-rw-rw-rw-   0        0        0     3531 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/power_electronics/acdc_converter/abstract_acdc_converter.py
+-rw-rw-rw-   0        0        0     4152 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/power_electronics/acdc_converter/bonfiglioli.py
+-rw-rw-rw-   0        0        0     2296 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/power_electronics/acdc_converter/fix_efficiency.py
+-rw-rw-rw-   0        0        0      407 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/power_electronics/acdc_converter/no_loss.py
+-rw-rw-rw-   0        0        0     3446 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/power_electronics/acdc_converter/notton.py
+-rw-rw-rw-   0        0        0     2821 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/power_electronics/acdc_converter/notton_loss.py
+-rw-rw-rw-   0        0        0     2459 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/power_electronics/acdc_converter/rampinelli_fit.py
+-rw-rw-rw-   0        0        0     3879 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/power_electronics/acdc_converter/sinamics.py
+-rw-rw-rw-   0        0        0     4198 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/power_electronics/acdc_converter/stable.py
+-rw-rw-rw-   0        0        0     4895 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/power_electronics/acdc_converter/stacked.py
+-rw-rw-rw-   0        0        0     8150 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/power_electronics/acdc_converter/sungrow.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.669113 simses-1.3.3/simses/system/power_electronics/dcdc_converter/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/power_electronics/dcdc_converter/__init__.py
+-rw-rw-rw-   0        0        0     2423 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/power_electronics/dcdc_converter/abstract_dcdc_converter.py
+-rw-rw-rw-   0        0        0     2775 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/power_electronics/dcdc_converter/fix_efficiency.py
+-rw-rw-rw-   0        0        0     2299 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/power_electronics/dcdc_converter/no_dcdc.py
+-rw-rw-rw-   0        0        0     1847 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/power_electronics/dcdc_converter/no_loss.py
+-rw-rw-rw-   0        0        0     6350 2023-03-06 13:30:03.000000 simses-1.3.3/simses/system/power_electronics/electronics.py
+-rw-rw-rw-   0        0        0     3725 2023-05-15 14:47:15.000000 simses-1.3.3/simses/system/storage_circuit.py
+-rw-rw-rw-   0        0        0    10030 2023-05-15 14:47:15.000000 simses-1.3.3/simses/system/storage_system_ac.py
+-rw-rw-rw-   0        0        0     5713 2023-03-06 13:30:03.000000 simses-1.3.3/simses/system/storage_system_dc.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.757091 simses-1.3.3/simses/system/test/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/test/__init__.py
+-rw-rw-rw-   0        0        0     7277 2023-05-16 11:19:36.000000 simses-1.3.3/simses/system/test/test_acdc_converter.py
+-rw-rw-rw-   0        0        0     1387 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/test/test_constant_ambient_temperature.py
+-rw-rw-rw-   0        0        0     3571 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/test/test_fix_cop_hvac.py
+-rw-rw-rw-   0        0        0      423 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/test/test_fixeta_centrifugal_pump.py
+-rw-rw-rw-   0        0        0     3846 2023-03-06 13:30:03.000000 simses-1.3.3/simses/system/test/test_location_ambient_temperature.py
+-rw-rw-rw-   0        0        0     1976 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/test/test_location_ambient_temperature_profile_check.py
+-rw-rw-rw-   0        0        0     4318 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/test/test_location_solar_irradiation_model.py
+-rw-rw-rw-   0        0        0     2801 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/test/test_location_solar_irradiation_model_profile_check.py
+-rw-rw-rw-   0        0        0     2274 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/test/test_notton_acdc_converter.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.771303 simses-1.3.3/simses/system/thermal/
+-rw-rw-rw-   0        0        0        2 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/thermal/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.836635 simses-1.3.3/simses/system/thermal/ambient/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/thermal/ambient/__init__.py
+-rw-rw-rw-   0        0        0     1325 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/thermal/ambient/ambient_thermal_model.py
+-rw-rw-rw-   0        0        0     1064 2023-05-15 14:47:15.000000 simses-1.3.3/simses/system/thermal/ambient/constant_temperature.py
+-rw-rw-rw-   0        0        0     1654 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/thermal/ambient/location_temperature.py
+-rw-rw-rw-   0        0        0     1585 2023-03-06 13:30:03.000000 simses-1.3.3/simses/system/thermal/ambient/user_battery_temperature.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.861538 simses-1.3.3/simses/system/thermal/model/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/thermal/model/__init__.py
+-rw-rw-rw-   0        0        0     3667 2023-03-06 13:30:03.000000 simses-1.3.3/simses/system/thermal/model/no_system_thermal_model.py
+-rw-rw-rw-   0        0        0     3095 2023-03-06 13:30:03.000000 simses-1.3.3/simses/system/thermal/model/system_thermal_model.py
+-rw-rw-rw-   0        0        0    15883 2023-03-06 13:30:03.000000 simses-1.3.3/simses/system/thermal/model/zero_d_room_thermal_model.py
+-rw-rw-rw-   0        0        0    24072 2023-03-06 13:30:03.000000 simses-1.3.3/simses/system/thermal/model/zero_d_system_thermal_model.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.932068 simses-1.3.3/simses/system/thermal/solar_irradiation/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/thermal/solar_irradiation/__init__.py
+-rw-rw-rw-   0        0        0    18001 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/thermal/solar_irradiation/location.py
+-rw-rw-rw-   0        0        0      795 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/thermal/solar_irradiation/no_solar_irradiation.py
+-rw-rw-rw-   0        0        0     1464 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/thermal/solar_irradiation/solar_irradiation_model.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.940977 simses-1.3.3/simses/technology/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.951245 simses-1.3.3/simses/technology/hydrogen/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.960254 simses-1.3.3/simses/technology/hydrogen/control/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/control/__init__.py
+-rw-rw-rw-   0        0        0     3315 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/control/management.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.035765 simses-1.3.3/simses/technology/hydrogen/control/pressure/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/control/pressure/__init__.py
+-rw-rw-rw-   0        0        0     3335 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/control/pressure/ideal_var_cathode.py
+-rw-rw-rw-   0        0        0      723 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/control/pressure/no_pressure_controller.py
+-rw-rw-rw-   0        0        0      791 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/control/pressure/pressure_controller.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.062705 simses-1.3.3/simses/technology/hydrogen/control/thermal/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/control/thermal/__init__.py
+-rw-rw-rw-   0        0        0     3633 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/control/thermal/ideal_var_flow.py
+-rw-rw-rw-   0        0        0      531 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/control/thermal/no_thermal_controller.py
+-rw-rw-rw-   0        0        0      795 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/control/thermal/thermal_controller.py
+-rw-rw-rw-   0        0        0     2522 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/control/thermal/var_flow.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.081794 simses-1.3.3/simses/technology/hydrogen/electrolyzer/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.108296 simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.142316 simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/calendar/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/calendar/__init__.py
+-rw-rw-rw-   0        0        0     2105 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/calendar/calendar_degradation.py
+-rw-rw-rw-   0        0        0      785 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/calendar/no_calendar_degradation.py
+-rw-rw-rw-   0        0        0     3071 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/calendar/pem_analytic.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.184191 simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/cyclic/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/cyclic/__init__.py
+-rw-rw-rw-   0        0        0     2123 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/cyclic/cyclic_degradation.py
+-rw-rw-rw-   0        0        0      796 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/cyclic/no_cyclic_degradation.py
+-rw-rw-rw-   0        0        0     4542 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/cyclic/pem_analytic.py
+-rw-rw-rw-   0        0        0     1437 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/cyclic/pem_analytic_ptl_coating.py
+-rw-rw-rw-   0        0        0     4502 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/degradation_model.py
+-rw-rw-rw-   0        0        0      728 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/no_degradation.py
+-rw-rw-rw-   0        0        0     1517 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/pem_analytic.py
+-rw-rw-rw-   0        0        0     1575 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/pem_analytic_ptl_coating.py
+-rw-rw-rw-   0        0        0     9672 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/factory.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.215616 simses-1.3.3/simses/technology/hydrogen/electrolyzer/pressure/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/pressure/__init__.py
+-rw-rw-rw-   0        0        0     1794 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/pressure/abstract_model.py
+-rw-rw-rw-   0        0        0     2448 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/pressure/alkaline.py
+-rw-rw-rw-   0        0        0     1802 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/pressure/no_pressure_model.py
+-rw-rw-rw-   0        0        0     3656 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/pressure/var_cathode.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.239198 simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.275572 simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/alkaline/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/alkaline/__init__.py
+-rw-rw-rw-   0        0        0    13091 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/alkaline/electrical_model.py
+-rw-rw-rw-   0        0        0     8273 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/alkaline/electrolyzer_model.py
+-rw-rw-rw-   0        0        0     1593 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/alkaline/fluid_model.py
+-rw-rw-rw-   0        0        0     1697 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/alkaline/parameters.py
+-rw-rw-rw-   0        0        0     1502 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/alkaline/pressure_model.py
+-rw-rw-rw-   0        0        0     1474 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/no_electrolyzer.py
+-rw-rw-rw-   0        0        0     4632 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/pem.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.353443 simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/__init__.py
+-rw-rw-rw-   0        0        0     5244 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/efficiency_curves.py
+-rw-rw-rw-   0        0        0     5765 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/electrical_model.py
+-rw-rw-rw-   0        0        0     8627 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/electrolyzer_model.py
+-rw-rw-rw-   0        0        0      603 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/electrolyzer_model_ptl_coating.py
+-rw-rw-rw-   0        0        0     2461 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/fluid_model.py
+-rw-rw-rw-   0        0        0     3649 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/membrane_model.py
+-rw-rw-rw-   0        0        0     2077 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/parameters.py
+-rw-rw-rw-   0        0        0     3318 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/pressure_model.py
+-rw-rw-rw-   0        0        0     5098 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/stack_model.py
+-rw-rw-rw-   0        0        0     5538 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/system.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.384462 simses-1.3.3/simses/technology/hydrogen/electrolyzer/thermal/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/thermal/__init__.py
+-rw-rw-rw-   0        0        0     1691 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/thermal/abstract_model.py
+-rw-rw-rw-   0        0        0     8252 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/thermal/alkaline.py
+-rw-rw-rw-   0        0        0     1352 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/thermal/no_thermal_model.py
+-rw-rw-rw-   0        0        0    12898 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/thermal/pem.py
+-rw-rw-rw-   0        0        0     2594 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/factory.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.400566 simses-1.3.3/simses/technology/hydrogen/fuel_cell/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/fuel_cell/__init__.py
+-rw-rw-rw-   0        0        0     5007 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/fuel_cell/factory.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.424309 simses-1.3.3/simses/technology/hydrogen/fuel_cell/pressure/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/fuel_cell/pressure/__init__.py
+-rw-rw-rw-   0        0        0     1527 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/fuel_cell/pressure/no_pressure.py
+-rw-rw-rw-   0        0        0     1766 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/fuel_cell/pressure/pressure_model.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.460298 simses-1.3.3/simses/technology/hydrogen/fuel_cell/stack/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/fuel_cell/stack/__init__.py
+-rw-rw-rw-   0        0        0     3734 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/fuel_cell/stack/jupiter.py
+-rw-rw-rw-   0        0        0     1208 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/fuel_cell/stack/no_fuel_cell.py
+-rw-rw-rw-   0        0        0     3141 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/fuel_cell/stack/pem.py
+-rw-rw-rw-   0        0        0     2232 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/fuel_cell/stack/stack_model.py
+-rw-rw-rw-   0        0        0     3181 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/fuel_cell/system.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.485387 simses-1.3.3/simses/technology/hydrogen/fuel_cell/thermal/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/fuel_cell/thermal/__init__.py
+-rw-rw-rw-   0        0        0      913 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/fuel_cell/thermal/no_thermal_model.py
+-rw-rw-rw-   0        0        0      963 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/fuel_cell/thermal/simple.py
+-rw-rw-rw-   0        0        0     1015 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/fuel_cell/thermal/thermal_model.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.496183 simses-1.3.3/simses/technology/hydrogen/hydrogen_storage/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/hydrogen_storage/__init__.py
+-rw-rw-rw-   0        0        0     1703 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/hydrogen_storage/hydrogen_storage.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.512071 simses-1.3.3/simses/technology/hydrogen/hydrogen_storage/pipeline/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/hydrogen_storage/pipeline/__init__.py
+-rw-rw-rw-   0        0        0      500 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/hydrogen_storage/pipeline/pipeline.py
+-rw-rw-rw-   0        0        0     1062 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/hydrogen_storage/pipeline/simple_pipeline.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.526746 simses-1.3.3/simses/technology/hydrogen/hydrogen_storage/pressuretank/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/hydrogen_storage/pressuretank/__init__.py
+-rw-rw-rw-   0        0        0     3899 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/hydrogen_storage/pressuretank/pressuretank.py
+-rw-rw-rw-   0        0        0     6240 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/system.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.534517 simses-1.3.3/simses/technology/hydrogen/test/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/test/__init__.py
+-rw-rw-rw-   0        0        0     8265 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/test/test_pem_electrolyzer.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.561623 simses-1.3.3/simses/technology/lithium_ion/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/__init__.py
+-rw-rw-rw-   0        0        0     6994 2023-03-06 13:30:03.000000 simses-1.3.3/simses/technology/lithium_ion/battery.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.573643 simses-1.3.3/simses/technology/lithium_ion/battery_management_system/
+-rw-rw-rw-   0        0        0        2 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/battery_management_system/__init__.py
+-rw-rw-rw-   0        0        0     7748 2023-03-06 13:30:03.000000 simses-1.3.3/simses/technology/lithium_ion/battery_management_system/management_system.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.699709 simses-1.3.3/simses/technology/lithium_ion/cell/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.718725 simses-1.3.3/simses/technology/lithium_ion/cell/electric/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/electric/__init__.py
+-rw-rw-rw-   0        0        0     1006 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/electric/default.py
+-rw-rw-rw-   0        0        0     3550 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/electric/properties.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.757435 simses-1.3.3/simses/technology/lithium_ion/cell/format/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/format/__init__.py
+-rw-rw-rw-   0        0        0      829 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/format/abstract.py
+-rw-rw-rw-   0        0        0      523 2023-03-06 13:30:03.000000 simses-1.3.3/simses/technology/lithium_ion/cell/format/pouch.py
+-rw-rw-rw-   0        0        0      555 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/format/prismatic.py
+-rw-rw-rw-   0        0        0      593 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/format/round.py
+-rw-rw-rw-   0        0        0      298 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/format/round_18650.py
+-rw-rw-rw-   0        0        0      298 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/format/round_26650.py
+-rw-rw-rw-   0        0        0     1952 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/generic.py
+-rw-rw-rw-   0        0        0     4224 2023-05-15 14:47:15.000000 simses-1.3.3/simses/technology/lithium_ion/cell/isea.py
+-rw-rw-rw-   0        0        0     5009 2023-03-06 13:30:03.000000 simses-1.3.3/simses/technology/lithium_ion/cell/lfp_sony.py
+-rw-rw-rw-   0        0        0      503 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/lfp_sony_generic.py
+-rw-rw-rw-   0        0        0     8685 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/lmo_daimler.py
+-rw-rw-rw-   0        0        0     5224 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/lto_lmo.py
+-rw-rw-rw-   0        0        0     5352 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/lto_nmc.py
+-rw-rw-rw-   0        0        0      532 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/nca_panasonic_generic.py
+-rw-rw-rw-   0        0        0     5469 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/nca_panasonic_ncr.py
+-rw-rw-rw-   0        0        0     4958 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/nmc_lgmj1.py
+-rw-rw-rw-   0        0        0     4514 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/nmc_molicel.py
+-rw-rw-rw-   0        0        0      518 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/nmc_molicel_generic.py
+-rw-rw-rw-   0        0        0     4931 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/nmc_samsung78Ah.py
+-rw-rw-rw-   0        0        0     7991 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/nmc_samsung94Ah.py
+-rw-rw-rw-   0        0        0     8558 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/nmc_samsung94Ah_hybrid.py
+-rw-rw-rw-   0        0        0     5481 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/nmc_sanyo_ur18650e.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.770758 simses-1.3.3/simses/technology/lithium_ion/cell/sodium_ion/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/sodium_ion/__init__.py
+-rw-rw-rw-   0        0        0     5578 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/sodium_ion/sodium_ion_green_rock.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.790108 simses-1.3.3/simses/technology/lithium_ion/cell/thermal/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/thermal/__init__.py
+-rw-rw-rw-   0        0        0      639 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/thermal/default.py
+-rw-rw-rw-   0        0        0     2131 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/thermal/properties.py
+-rw-rw-rw-   0        0        0    16261 2023-03-06 13:30:03.000000 simses-1.3.3/simses/technology/lithium_ion/cell/type.py
+-rw-rw-rw-   0        0        0    15101 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/circuit.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.881842 simses-1.3.3/simses/technology/lithium_ion/degradation/
+-rw-rw-rw-   0        0        0        2 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.983318 simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/
+-rw-rw-rw-   0        0        0        2 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/__init__.py
+-rw-rw-rw-   0        0        0     3104 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/calendar_degradation.py
+-rw-rw-rw-   0        0        0     2364 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/generic_cell.py
+-rw-rw-rw-   0        0        0     2993 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/lfp_generic.py
+-rw-rw-rw-   0        0        0     5050 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/lfp_sony.py
+-rw-rw-rw-   0        0        0     3736 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/lto_lmo.py
+-rw-rw-rw-   0        0        0     3698 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/lto_nmc.py
+-rw-rw-rw-   0        0        0     2923 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/nca_generic.py
+-rw-rw-rw-   0        0        0     4689 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/nca_panasonicNCR.py
+-rw-rw-rw-   0        0        0     3063 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/nmc_generic.py
+-rw-rw-rw-   0        0        0     3077 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/nmc_lgmj1.py
+-rw-rw-rw-   0        0        0     4451 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/nmc_molicel.py
+-rw-rw-rw-   0        0        0     2914 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/nmc_sanyo_ur18650e.py
+-rw-rw-rw-   0        0        0      790 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/no_calendar_dedradation.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:41.075428 simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/
+-rw-rw-rw-   0        0        0        2 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/__init__.py
+-rw-rw-rw-   0        0        0     3202 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/cyclic_degradation.py
+-rw-rw-rw-   0        0        0     2316 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/generic_cell.py
+-rw-rw-rw-   0        0        0     4820 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/lfp_generic.py
+-rw-rw-rw-   0        0        0     5993 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/lfp_sony.py
+-rw-rw-rw-   0        0        0     4560 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/lto_lmo.py
+-rw-rw-rw-   0        0        0     4568 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/lto_nmc.py
+-rw-rw-rw-   0        0        0     4173 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/nca_generic.py
+-rw-rw-rw-   0        0        0     6795 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/nca_panasonicNCR.py
+-rw-rw-rw-   0        0        0     4784 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/nmc_generic.py
+-rw-rw-rw-   0        0        0     4700 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/nmc_lgmj1.py
+-rw-rw-rw-   0        0        0     6373 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/nmc_molicel.py
+-rw-rw-rw-   0        0        0     3885 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/nmc_sanyo_ur18650e.py
+-rw-rw-rw-   0        0        0      764 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/no_cyclic_degradation.py
+-rw-rw-rw-   0        0        0     8719 2023-03-06 13:30:03.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/degradation_model.py
+-rw-rw-rw-   0        0        0      958 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/generic_cell.py
+-rw-rw-rw-   0        0        0      933 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/lfp_generic.py
+-rw-rw-rw-   0        0        0     1159 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/lfp_sony.py
+-rw-rw-rw-   0        0        0     1251 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/lmo_daimler.py
+-rw-rw-rw-   0        0        0      853 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/lto_lmo.py
+-rw-rw-rw-   0        0        0      853 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/lto_nmc.py
+-rw-rw-rw-   0        0        0      933 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/nca_generic.py
+-rw-rw-rw-   0        0        0      974 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/nca_panasonicNCR.py
+-rw-rw-rw-   0        0        0      933 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/nmc_generic.py
+-rw-rw-rw-   0        0        0      872 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/nmc_lgmj1.py
+-rw-rw-rw-   0        0        0     1103 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/nmc_molicel.py
+-rw-rw-rw-   0        0        0     1146 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/nmc_samsung94Ah.py
+-rw-rw-rw-   0        0        0      921 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/nmc_sanyo_ur18650e.py
+-rw-rw-rw-   0        0        0      804 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/no_degradation.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:41.093480 simses-1.3.3/simses/technology/lithium_ion/equivalent_circuit_model/
+-rw-rw-rw-   0        0        0        4 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/equivalent_circuit_model/__init__.py
+-rw-rw-rw-   0        0        0      527 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/equivalent_circuit_model/equivalent_circuit.py
+-rw-rw-rw-   0        0        0     1861 2023-03-06 13:30:03.000000 simses-1.3.3/simses/technology/lithium_ion/equivalent_circuit_model/rint_model.py
+-rw-rw-rw-   0        0        0    16756 2023-05-16 11:37:56.000000 simses-1.3.3/simses/technology/lithium_ion/factory.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:41.109333 simses-1.3.3/simses/technology/lithium_ion/test/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/test/__init__.py
+-rw-rw-rw-   0        0        0     2384 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/test/test_battery.py
+-rw-rw-rw-   0        0        0     5158 2023-03-06 13:30:03.000000 simses-1.3.3/simses/technology/lithium_ion/test/test_bms.py
+-rw-rw-rw-   0        0        0     2797 2023-05-16 11:18:19.000000 simses-1.3.3/simses/technology/lithium_ion/test/test_type.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:41.153758 simses-1.3.3/simses/technology/redox_flow/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:41.224759 simses-1.3.3/simses/technology/redox_flow/degradation/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/degradation/__init__.py
+-rw-rw-rw-   0        0        0     1657 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/degradation/capacity_degradation.py
+-rw-rw-rw-   0        0        0     2873 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/degradation/const_hydrogen_current.py
+-rw-rw-rw-   0        0        0      541 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/degradation/no_degradation.py
+-rw-rw-rw-   0        0        0     4209 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/degradation/variable_hydrogen_current.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:41.240005 simses-1.3.3/simses/technology/redox_flow/electrochemical/
+-rw-rw-rw-   0        0        0        4 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/electrochemical/__init__.py
+-rw-rw-rw-   0        0        0     1017 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/electrochemical/abstract_electrochemical.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:41.260662 simses-1.3.3/simses/technology/redox_flow/electrochemical/control/
+-rw-rw-rw-   0        0        0        2 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/electrochemical/control/__init__.py
+-rw-rw-rw-   0        0        0    10697 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/electrochemical/control/redox_control_system.py
+-rw-rw-rw-   0        0        0     8509 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/electrochemical/rint_model.py
+-rw-rw-rw-   0        0        0    17184 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/factory.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:41.292461 simses-1.3.3/simses/technology/redox_flow/pump_algorithm/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/pump_algorithm/__init__.py
+-rw-rw-rw-   0        0        0     4905 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/pump_algorithm/abstract_pump_algorithm.py
+-rw-rw-rw-   0        0        0     4324 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/pump_algorithm/constant_pressure_pulsed.py
+-rw-rw-rw-   0        0        0     3741 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/pump_algorithm/fix_flow_rate_start_stop.py
+-rw-rw-rw-   0        0        0     5153 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/pump_algorithm/stoich_flow_rate.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:41.330826 simses-1.3.3/simses/technology/redox_flow/stack/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/stack/__init__.py
+-rw-rw-rw-   0        0        0    10504 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/stack/abstract_stack.py
+-rw-rw-rw-   0        0        0     8549 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/stack/cell_data_stack_5500w.py
+-rw-rw-rw-   0        0        0     4627 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/stack/dummy_stack_3000w.py
+-rw-rw-rw-   0        0        0     4554 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/stack/dummy_stack_5500W.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:41.433772 simses-1.3.3/simses/technology/redox_flow/stack/electrolyte/
+-rw-rw-rw-   0        0        0        4 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/stack/electrolyte/__init__.py
+-rw-rw-rw-   0        0        0     3675 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/stack/electrolyte/abstract_electrolyte.py
+-rw-rw-rw-   0        0        0     4086 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/stack/electrolyte/vanadium.py
+-rw-rw-rw-   0        0        0     7211 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/stack/high_performance_stack_5700W.py
+-rw-rw-rw-   0        0        0     5787 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/stack/industrial_stack_1500w.py
+-rw-rw-rw-   0        0        0     5663 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/stack/industrial_stack_9000w.py
+-rw-rw-rw-   0        0        0    13481 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/system.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:07:41.462998 simses-1.3.3/simses/technology/redox_flow/test/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/test/__init__.py
+-rw-rw-rw-   0        0        0     3013 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/test/test_stack_module.py
+-rw-rw-rw-   0        0        0     2749 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/storage.py
```

### Comparing `simses-1.3.2/LICENSE.txt` & `simses-1.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/analysis/data/abstract_data.py` & `simses-1.3.3/simses/analysis/data/abstract_data.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/analysis/data/electrolyzer.py` & `simses-1.3.3/simses/analysis/data/electrolyzer.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/analysis/data/energy_management.py` & `simses-1.3.3/simses/analysis/data/energy_management.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/analysis/data/fuel_cell.py` & `simses-1.3.3/simses/analysis/data/fuel_cell.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/analysis/data/hydrogen.py` & `simses-1.3.3/simses/analysis/data/hydrogen.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/analysis/data/lithium_ion.py` & `simses-1.3.3/simses/analysis/data/lithium_ion.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/analysis/data/redox_flow.py` & `simses-1.3.3/simses/analysis/data/redox_flow.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/analysis/data/system.py` & `simses-1.3.3/simses/analysis/data/system.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,22 @@
         return self._get_data(SystemState.SOH)
 
     @property
     def temperature(self):
         return self._get_data(SystemState.TEMPERATURE)
 
     @property
+    def ol_temperature(self):
+        return self._get_data(SystemState.OL_TEMPERATURE)
+
+    @property
+    def il_temperature(self):
+        return self._get_data(SystemState.IL_TEMPERATURE)
+
+    @property
     def ambient_temperature(self):
         return self._get_data(SystemState.AMBIENT_TEMPERATURE)
 
     @property
     def storage_fulfillment(self):
         return self._get_data(SystemState.AC_FULFILLMENT)
```

### Comparing `simses-1.3.2/simses/analysis/evaluation/abstract_evaluation.py` & `simses-1.3.3/simses/analysis/evaluation/abstract_evaluation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/analysis/evaluation/economic/economic_evaluation.py` & `simses-1.3.3/simses/analysis/evaluation/economic/economic_evaluation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/analysis/evaluation/economic/revenue_stream/abstract_revenue_stream.py` & `simses-1.3.3/simses/analysis/evaluation/economic/revenue_stream/abstract_revenue_stream.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/analysis/evaluation/economic/revenue_stream/demand_charge_reduction.py` & `simses-1.3.3/simses/analysis/evaluation/economic/revenue_stream/demand_charge_reduction.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/analysis/evaluation/economic/revenue_stream/electricity_consumption.py` & `simses-1.3.3/simses/analysis/evaluation/economic/revenue_stream/electricity_consumption.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/analysis/evaluation/economic/revenue_stream/energy_cost_reduction.py` & `simses-1.3.3/simses/analysis/evaluation/economic/revenue_stream/energy_cost_reduction.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/analysis/evaluation/economic/revenue_stream/fcr_revenue_stream.py` & `simses-1.3.3/simses/analysis/evaluation/economic/revenue_stream/fcr_revenue_stream.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/analysis/evaluation/economic/revenue_stream/intraday_recharge.py` & `simses-1.3.3/simses/analysis/evaluation/economic/revenue_stream/intraday_recharge.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/analysis/evaluation/economic/revenue_stream/operation_and_maintenance.py` & `simses-1.3.3/simses/analysis/evaluation/economic/revenue_stream/operation_and_maintenance.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/analysis/evaluation/merger.py` & `simses-1.3.3/simses/analysis/evaluation/merger.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/analysis/evaluation/plotting/axis.py` & `simses-1.3.3/simses/analysis/evaluation/plotting/axis.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/analysis/evaluation/plotting/energy_plotting.py` & `simses-1.3.3/simses/analysis/evaluation/plotting/energy_plotting.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/analysis/evaluation/plotting/matplot_plotting.py` & `simses-1.3.3/simses/analysis/evaluation/plotting/matplot_plotting.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/analysis/evaluation/plotting/plotly_plotting.py` & `simses-1.3.3/simses/analysis/evaluation/plotting/plotly_plotting.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/analysis/evaluation/plotting/plotter.py` & `simses-1.3.3/simses/analysis/evaluation/plotting/plotter.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/analysis/evaluation/plotting/sankey_diagram.py` & `simses-1.3.3/simses/analysis/evaluation/plotting/sankey_diagram.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/analysis/evaluation/plotting/sunburst_diagram.py` & `simses-1.3.3/simses/analysis/evaluation/plotting/sunburst_diagram.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/analysis/evaluation/plotting/system_parameters.py` & `simses-1.3.3/simses/analysis/evaluation/plotting/system_parameters.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/analysis/evaluation/result.py` & `simses-1.3.3/simses/analysis/evaluation/result.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/analysis/evaluation/technical/electrolyzer.py` & `simses-1.3.3/simses/analysis/evaluation/technical/electrolyzer.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/analysis/evaluation/technical/fuel_cell.py` & `simses-1.3.3/simses/analysis/evaluation/technical/fuel_cell.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/analysis/evaluation/technical/hydrogen.py` & `simses-1.3.3/simses/analysis/evaluation/technical/hydrogen.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/analysis/evaluation/technical/lithium_ion.py` & `simses-1.3.3/simses/analysis/evaluation/technical/lithium_ion.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/analysis/evaluation/technical/redox_flow.py` & `simses-1.3.3/simses/analysis/evaluation/technical/redox_flow.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/analysis/evaluation/technical/site_level.py` & `simses-1.3.3/simses/analysis/evaluation/technical/site_level.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/analysis/evaluation/technical/system.py` & `simses-1.3.3/simses/analysis/evaluation/technical/system.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,25 +16,26 @@
 
 class SystemTechnicalEvaluation(TechnicalEvaluation):
 
     __power_title = 'System power'
     __soc_title = 'System SOC'
     __system_thermal_title = 'System thermal parameters'
     __additional_title = 'Additional DC power'
-    __dc_power_loss_title = 'Loss through power electronics'
+    __power_loss_title = 'Power losses'
     __voltage_title = 'Intermediate circuit voltage'
     __energy_flows_title = 'Energy flows'
     __loss_distribution_title = 'Losses distribution'
 
     def __init__(self, data: SystemData, config: GeneralAnalysisConfig, path: str):
         super().__init__(data, config)
         self.__log: Logger = Logger(type(self).__name__)
         title_extension: str = ' for system ' + self.get_data().id
         self.__power_title += title_extension
         self.__soc_title += title_extension
+        self.__power_loss_title += title_extension
         self.__system_thermal_title += title_extension
         self.__energy_flows_title += title_extension
         self.__additional_title += title_extension
         self.__loss_distribution_title += title_extension
         self.__result_path = path
         self._set_numpy_err_handling()
 
@@ -81,28 +82,26 @@
         self.append_result(EvaluationResult(Description.Technical.ACDC_EFFICIENCY_CHARGE, Unit.PERCENTAGE, total_acdc_charge_efficiency))
         self.append_result(EvaluationResult(Description.Technical.ACDC_EFFICIENCY_DISCHARGE, Unit.PERCENTAGE, total_acdc_discharge_efficiency))
         self.append_result(EvaluationResult(Description.Technical.ACDC_EFFICIENCY, Unit.PERCENTAGE, total_acdc_efficiency))
         self.append_result(EvaluationResult(Description.Technical.PE_EFFICIENCY, Unit.PERCENTAGE, total_pe_efficiency))
         self.append_result(EvaluationResult(Description.Technical.MAX_LOAD_DC_POWER_ADDITIONAL, Unit.WATT, self.max_load_dc_power_additional))
         self.append_result(EvaluationResult(Description.Technical.MAX_GENERATION_DC_POWER_ADDITIONAL, Unit.WATT, self.max_generation_dc_power_additional))
         self.append_result(EvaluationResult(Description.Technical.SYSTEM_TEMPORAL_UTILIZATION, Unit.NONE, self.system_temporal_utilization()))
-
-
         # self.append_time_series(SystemState.DC_POWER_ADDITIONAL, data.dc_power_additional)
         # self.append_time_series(SystemState.DC_POWER_STORAGE, data.dc_power_storage)
         # self.append_time_series(SystemState.SOC, data.soc)
         self.print_results()
 
     def plot(self) -> None:
         self.__power_plotting()
         self.__soc_plotting()
+        self.__power_loss_plotting()
         self.__system_thermal_plotting()
         # self.__voltage_plotting()
         self.__additional_dc_power_plotting()
-        self.__dc_power_loss_plotting()
         self.__energy_flows_plotting()
         self.__loss_distribution_plotting()
 
     def __soc_plotting(self):
         data: SystemData = self.get_data()
         plot: Plotting = PlotlyPlotting(title=self.__soc_title, path=self.__result_path)
         xaxis: Axis = Axis(data=Plotting.format_time(data.time), label=SystemState.TIME)
@@ -116,22 +115,29 @@
         plot: Plotting = PlotlyPlotting(title=self.__voltage_title, path=self.__result_path)
         xaxis: Axis = Axis(data=Plotting.format_time(data.time), label=SystemState.TIME)
         yaxis: [Axis] = [Axis(data.dc_voltage, label=SystemState.DC_VOLTAGE_CIRCUIT, color=PlotlyPlotting.Color.SOC_BLUE)]
         plot.lines(xaxis, yaxis)
         plot.histogram(xaxis=xaxis, yaxis=yaxis)
         self.extend_figures(plot.get_figures())
 
-    def __dc_power_loss_plotting(self):
+    def __power_loss_plotting(self):
         data: SystemData = self.get_data()
-        if sum(abs(data.dc_power_loss)) > 0.0:
-            plot: Plotting = PlotlyPlotting(title=self.__dc_power_loss_title, path=self.__result_path)
-            xaxis: Axis = Axis(data=Plotting.format_time(data.time), label=SystemState.TIME)
-            yaxis: [Axis] = [Axis(data.dc_power_loss, label=SystemState.DC_POWER_LOSS)]
-            plot.lines(xaxis, yaxis)
-            self.extend_figures(plot.get_figures())
+        plot: Plotting = PlotlyPlotting(title=self.__power_loss_title, path=self.__result_path)
+        xaxis: Axis = Axis(data=Plotting.format_time(data.time), label=SystemState.TIME)
+        yaxis: [Axis] = list()
+        yaxis.append(Axis(data=data.pe_losses, label=SystemState.PE_LOSSES, color=PlotlyPlotting.Color.RED,
+                          linestyle=PlotlyPlotting.Linestyle.SOLID))
+        yaxis.append(Axis(data=data.dc_power_loss, label=SystemState.DC_POWER_LOSS, color=PlotlyPlotting.Color.HEAT_ORANGE,
+                          linestyle=PlotlyPlotting.Linestyle.SOLID))
+        yaxis.append(Axis(data=data.storage_technology_loss_power, label=SystemState.STORAGE_POWER_LOSS, color=PlotlyPlotting.Color.BLACK,
+                          linestyle=PlotlyPlotting.Linestyle.SOLID))
+        yaxis.append(Axis(data=data.aux_power, label=SystemState.AUX_LOSSES,
+                          color=PlotlyPlotting.Color.BLUE, linestyle=PlotlyPlotting.Linestyle.SOLID))
+        plot.lines(xaxis=xaxis, yaxis=yaxis)
+        self.extend_figures(plot.get_figures())
 
     def __additional_dc_power_plotting(self):
         data: SystemData = self.get_data()
         if sum(abs(data.dc_power_additional)) > 0.0:
             plot: Plotting = PlotlyPlotting(title=self.__additional_title, path=self.__result_path)
             xaxis: Axis = Axis(data=Plotting.format_time(data.time), label=SystemState.TIME)
             yaxis: [Axis] = [Axis(data.dc_power_additional, label=SystemState.DC_POWER_ADDITIONAL)]
@@ -158,29 +164,40 @@
         plot.lines(xaxis=xaxis, yaxis=yaxis)
         plot.histogram(xaxis=xaxis, yaxis=yaxis)
         self.extend_figures(plot.get_figures())
 
     def __system_thermal_plotting(self):
 
         data: SystemData = self.get_data()
-        plot: Plotting = PlotlyPlotting(title=self.__system_thermal_title, path=self.__result_path)
+        if abs(sum(data.hvac_thermal_power)) > 1:  # HVAC power only present in scenarios with housing and solar irradiation
+            plot: Plotting = PlotlyPlotting(title=self.__system_thermal_title, path=self.__result_path)
+            xaxis: Axis = Axis(data=Plotting.format_time(data.time), label=SystemState.TIME)
+            yaxis: [Axis] = list()
+
+            yaxis.append(Axis(data=data.solar_thermal_load, label=SystemState.SOLAR_THERMAL_LOAD,
+                              color=PlotlyPlotting.Color.POWER_YELLOW, linestyle=PlotlyPlotting.Linestyle.SOLID))
+            yaxis.append(Axis(data=-1*data.hvac_thermal_power, label=SystemState.HVAC_THERMAL_POWER, color=PlotlyPlotting.Color.BRIGHT_BLUE,
+                              linestyle=PlotlyPlotting.Linestyle.SOLID))
+            plot.subplots(xaxis=xaxis, yaxis=yaxis)
+            self.extend_figures(plot.get_figures())
+
+        plot3: Plotting = PlotlyPlotting(title=self.__system_thermal_title, path=self.__result_path)
         xaxis: Axis = Axis(data=Plotting.format_time(data.time), label=SystemState.TIME)
         yaxis: [Axis] = list()
         yaxis.append(Axis(data=data.ambient_temperature, label=SystemState.AMBIENT_TEMPERATURE,
                           color=PlotlyPlotting.Color.BRIGHT_GREEN, linestyle=PlotlyPlotting.Linestyle.SOLID))
-        yaxis.append(Axis(data=data.solar_thermal_load, label=SystemState.SOLAR_THERMAL_LOAD,
-                          color=PlotlyPlotting.Color.POWER_YELLOW, linestyle=PlotlyPlotting.Linestyle.SOLID))
-        yaxis.append(Axis(data=data.hvac_thermal_power, label=SystemState.HVAC_THERMAL_POWER, color=PlotlyPlotting.Color.BRIGHT_BLUE,
-                          linestyle=PlotlyPlotting.Linestyle.SOLID))
+        if sum(data.ol_temperature) > 1:
+            yaxis.append(Axis(data=data.ol_temperature, label=SystemState.OL_TEMPERATURE, color=PlotlyPlotting.Color.YELLOW,
+                              linestyle=PlotlyPlotting.Linestyle.SOLID))
+            yaxis.append(Axis(data=data.il_temperature, label=SystemState.IL_TEMPERATURE, color=PlotlyPlotting.Color.GREY,
+                              linestyle=PlotlyPlotting.Linestyle.SOLID))
         yaxis.append(Axis(data=data.temperature, label=SystemState.TEMPERATURE, color=PlotlyPlotting.Color.TEMPERATURE_RED,
                           linestyle=PlotlyPlotting.Linestyle.SOLID))
-        # yaxis.append(Axis(data=data.aux_power, label=SystemState.AUX_LOSSES,
-        #                   color=PlotlyPlotting.Color.RED, linestyle=PlotlyPlotting.Linestyle.SOLID))
-        plot.subplots(xaxis=xaxis, yaxis=yaxis)
-        self.extend_figures(plot.get_figures())
+        plot3.lines(xaxis=xaxis, yaxis=yaxis)
+        self.extend_figures(plot3.get_figures())
 
     def __energy_flows_plotting(self):
         data: SystemData = self.get_data()
         sankey_diagram: SankeyDiagram = SankeyDiagram(data, title=self.__energy_flows_title, path=self.__result_path)
         node_links: dict = sankey_diagram.create_node_links()
         plot: Plotting = PlotlyPlotting(self.__energy_flows_title, self.__result_path)
         plot.sankey_diagram(node_links)
@@ -250,24 +267,24 @@
         total_power_out = power_out[power_out < 0].sum()
         return 100.0 * (total_power_out / total_power_in)
 
     def total_dcdc_efficiency_charge(self) -> float:
         data: SystemData = self.get_data()
         dc_power_intermediate_circuit = data.dc_power + data.dc_power_additional
         return self.__total_charge_efficiency(dc_power_intermediate_circuit, data.dc_power_storage)
-    
+
     def total_dcdc_efficiency_discharge(self) -> float:
         data: SystemData = self.get_data()
         dc_power_intermediate_circuit = data.dc_power + data.dc_power_additional
         return self.__total_discharge_efficiency(data.dc_power_storage, dc_power_intermediate_circuit)
-    
+
     def total_acdc_efficiency_charge(self) -> float:
         data: SystemData = self.get_data()
         return self.__total_charge_efficiency(data.ac_pe_power, data.dc_power)
-    
+
     def total_acdc_efficiency_discharge(self) -> float:
         data: SystemData = self.get_data()
         return self.__total_discharge_efficiency(data.dc_power, data.ac_pe_power)
 
     def system_temporal_utilization(self) -> float:
         """
         calculates and returns system temporal utilization in p.u.
```

### Comparing `simses-1.3.2/simses/analysis/evaluation/technical/technical_evaluation.py` & `simses-1.3.3/simses/analysis/evaluation/technical/technical_evaluation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/analysis/factory.py` & `simses-1.3.3/simses/analysis/factory.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/analysis/storage.py` & `simses-1.3.3/simses/analysis/storage.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/analysis/test/test_demand_charge_reduction.py` & `simses-1.3.3/simses/analysis/test/test_demand_charge_reduction.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/analysis/test/test_energy_cost_reduction.py` & `simses-1.3.3/simses/analysis/test/test_energy_cost_reduction.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/analysis/test/test_fcr_revenue_stream.py` & `simses-1.3.3/simses/analysis/test/test_fcr_revenue_stream.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/analysis/test/test_intraday_recharge_revenue_stream.py` & `simses-1.3.3/simses/analysis/test/test_intraday_recharge_revenue_stream.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/analysis/test/test_technical_evaluation.py` & `simses-1.3.3/simses/analysis/test/test_technical_evaluation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/analysis/utils.py` & `simses-1.3.3/simses/analysis/utils.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/analysis.defaults.ini` & `simses-1.3.3/simses/analysis.defaults.ini`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/config/abstract_config.py` & `simses-1.3.3/simses/commons/config/abstract_config.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/config/analysis/analysis_config.py` & `simses-1.3.3/simses/commons/config/analysis/analysis_config.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/config/analysis/economic.py` & `simses-1.3.3/simses/commons/config/analysis/economic.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/config/analysis/general.py` & `simses-1.3.3/simses/commons/config/analysis/general.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/config/analysis/market.py` & `simses-1.3.3/simses/commons/config/analysis/market.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/config/data/auxiliary.py` & `simses-1.3.3/simses/commons/config/data/auxiliary.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/config/data/battery.py` & `simses-1.3.3/simses/commons/config/data/battery.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/config/data/data_config.py` & `simses-1.3.3/simses/commons/config/data/data_config.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/config/data/electrolyzer.py` & `simses-1.3.3/simses/commons/config/data/electrolyzer.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/config/data/energy_management.py` & `simses-1.3.3/simses/commons/config/data/energy_management.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/config/data/fuel_cell.py` & `simses-1.3.3/simses/commons/config/data/fuel_cell.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/config/data/power_electronics.py` & `simses-1.3.3/simses/commons/config/data/power_electronics.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/config/data/redox_flow.py` & `simses-1.3.3/simses/commons/config/data/redox_flow.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/config/generation/analysis.py` & `simses-1.3.3/simses/commons/config/generation/analysis.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/config/generation/generator.py` & `simses-1.3.3/simses/commons/config/generation/generator.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/config/generation/simulation.py` & `simses-1.3.3/simses/commons/config/generation/simulation.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,14 +61,28 @@
 
         """
         path: str = SimulationConfig.CONFIG_PATH
         path += SimulationConfig.CONFIG_NAME
         path += SimulationConfig.LOCAL
         self.load_config_from(path)
 
+    def load_specific_config(self, config_name: str) -> None:
+        """
+        Loads specific config given by config-name without ".local.ini" at the end
+
+        Returns
+        -------
+
+        """
+        path: str = SimulationConfig.CONFIG_PATH
+        path += config_name
+        path += SimulationConfig.LOCAL
+        self.load_config_from(path)
+
+
     def __check_time_format(self, time: str) -> None:
         if time is None:
             return
         try:
             datetime.strptime(time, GeneralSimulationConfig.TIME_FORMAT)
         except ValueError:
             raise ValueError('Incorrect time format. Expected time format: ' + GeneralSimulationConfig.TIME_FORMAT)
@@ -807,28 +821,89 @@
         """
         Set the filename for the load profile
         :param load_profile: name of specified file as str
         :return: None
         """
         self._set(ProfileConfig.SECTION, ProfileConfig.LOAD_PROFILE, load_profile)
 
-    def set_total_profile_config(self, all_profile_direction, soc_profile, binary_profile) -> None:
+    def set_profile_direction(self, all_profile_direction: str) -> None:
+        """
+        Sets the parameters for the load profile: Direction
+        Parameters
+        ----------
+
+        Returns
+        -------
+
+        """
+        self._set(ProfileConfig.SECTION, ProfileConfig.POWER_PROFILE_DIR, all_profile_direction)
+        self._set(ProfileConfig.SECTION, ProfileConfig.TECHNICAL_PROFILE_DIR, all_profile_direction)
+
+
+    def set_total_profile_config(self, all_profile_direction, soc_profile, binary_profile, v2gprofile: str = None) -> None:
         """
         Sets parameters for the profile section of the simulation.ini
         :param technical_profile_direction: name of the profile direction as str
         :param soc_profile: name of specified soc profile as str
         :param binary_profile: name of specified binary profile as str
 
         :return:
         """
         self._set(ProfileConfig.SECTION, ProfileConfig.TECHNICAL_PROFILE_DIR, all_profile_direction)
         self._set(ProfileConfig.SECTION, ProfileConfig.POWER_PROFILE_DIR, all_profile_direction)
         self._set(ProfileConfig.SECTION, ProfileConfig.SOC_PROFILE, soc_profile)
         self._set(ProfileConfig.SECTION, ProfileConfig.BINARY_PROFILE, binary_profile)
+        self._set(ProfileConfig.SECTION, ProfileConfig.V2G_PROFILE, v2gprofile)
 
     def set_generation_profile_config(self, generation_profile: str = None) -> None:
         """
         Set the filename for the generation profile
         :param generation_profile: name of specified file as str
         :return: None
         """
         self._set(ProfileConfig.SECTION, ProfileConfig.GENERATION_PROFILE, generation_profile)
+
+    def set_generation_profile_parameters(self, generation_profile: str, generation_scaling_type: str,
+                                          generation_scaling_factor: str) -> None:
+        """
+       Sets the parameters for the generation profile: Direction, name of profile, generation scaling type (energy/power),
+        generation scaling factor
+        Parameters
+        ----------
+        load_generation_scaling_factor : desired load scaling factor as str
+            examples: 5e6, 5e7, etc.
+
+        Returns
+        -------
+
+        """
+        self._set(ProfileConfig.SECTION, ProfileConfig.GENERATION_PROFILE, generation_profile)
+        self._set(ProfileConfig.SECTION, ProfileConfig.GENERATION_PROFILE_SCALING, generation_scaling_type)
+        self._set(ProfileConfig.SECTION, ProfileConfig.GENERATION_SCALING_FACTOR, generation_scaling_factor)
+
+    def set_load_profile_parameters(self, all_profile_direction: str, load_profile: str, load_scaling_type: str,
+                                    load_scaling_factor: str) -> None:
+        """
+        Sets the parameters for the load profile: Direction, name of profile, load scaling type (energy/power),
+        load scaling factor
+        Parameters
+        ----------
+        load_generation_scaling_factor : desired load scaling factor as str
+            examples: 5e6, 5e7, etc.
+
+        Returns
+        -------
+
+        """
+        self._set(ProfileConfig.SECTION, ProfileConfig.POWER_PROFILE_DIR, all_profile_direction)
+        self._set(ProfileConfig.SECTION, ProfileConfig.LOAD_PROFILE, load_profile)
+        self._set(ProfileConfig.SECTION, ProfileConfig.LOAD_PROFILE_SCALING, load_scaling_type)
+        self._set(ProfileConfig.SECTION, ProfileConfig.LOAD_SCALING_FACTOR, load_scaling_factor)
+
+
+    def set_frequency_profile_config(self, frequency_profile: str = None) -> None:
+        """
+        Set the filename for the frequency profile
+        :param frequency_profile: name of specified file as str
+        :return: None
+        """
+        self._set(ProfileConfig.SECTION, ProfileConfig.FREQUENCY_PROFILE, frequency_profile)
```

### Comparing `simses-1.3.2/simses/commons/config/log.py` & `simses-1.3.3/simses/commons/config/log.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/config/simulation/battery.py` & `simses-1.3.3/simses/commons/config/simulation/battery.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/config/simulation/electrolyzer.py` & `simses-1.3.3/simses/commons/config/simulation/electrolyzer.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/config/simulation/energy_management.py` & `simses-1.3.3/simses/commons/config/simulation/energy_management.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,16 @@
     MAX_POWER_MONTHLY_MODE: str = 'MAX_POWER_MONTHLY_MODE'
     EV_CHARGING_STRATEGY: str = 'EV_CHARGING_STRATEGY'
 
     MULTI_USE_STRATEGIES: str = 'MULTI_USE_STRATEGIES'
     ENERGY_ALLOCATION: str = 'ENERGY_ALLOCATION'
     POWER_ALLOCATION: str = 'POWER_ALLOCATION'
     RANKING: str = 'RANKING'
+    OPTIMIZED_POWER_DIST_CASE: str = 'OPTIMIZED_POWER_DIST_CASE'
+    OPTIMIZED_POWER_DIST_CASE_LIM: str = 'OPTIMIZED_POWER_DIST_CASE_LIM'
 
     def __init__(self, config: ConfigParser, path: str = None):
         super().__init__(path, config)
 
     @property
     def operation_strategy(self) -> str:
         """Returns operation strategy from __analysis_config file_name"""
@@ -119,7 +121,17 @@
         return props
 
     @property
     def multi_use_rank(self) -> [int]:
         """Returns the different priorities of different strategies"""
         props: [int] = clean_split(self.get_property(self.SECTION, self.RANKING), ',')
         return props
+
+    @property
+    def optimized_power_dist_case(self) -> str:
+        """Returns case for PSO Algorithm"""
+        return self.get_property(self.SECTION, self.OPTIMIZED_POWER_DIST_CASE)
+
+    @property
+    def optimized_power_dist_case_lim(self) -> str:
+        """Returns case for PSO Algorithm"""
+        return self.get_property(self.SECTION, self.OPTIMIZED_POWER_DIST_CASE_LIM)
```

### Comparing `simses-1.3.2/simses/commons/config/simulation/fuel_cell.py` & `simses-1.3.3/simses/commons/config/simulation/fuel_cell.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/config/simulation/general.py` & `simses-1.3.3/simses/commons/config/simulation/general.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/config/simulation/hydrogen.py` & `simses-1.3.3/simses/commons/config/simulation/hydrogen.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/config/simulation/profile.py` & `simses-1.3.3/simses/commons/config/simulation/profile.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/config/simulation/redox_flow.py` & `simses-1.3.3/simses/commons/config/simulation/redox_flow.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/config/simulation/simulation_config.py` & `simses-1.3.3/simses/commons/config/simulation/simulation_config.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/config/simulation/system.py` & `simses-1.3.3/simses/commons/config/simulation/system.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/console_printer.py` & `simses-1.3.3/simses/commons/console_printer.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/constants.py` & `simses-1.3.3/simses/commons/constants.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/csv_standard.py` & `simses-1.3.3/simses/commons/csv_standard.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/cycle_detection/cycle_detector.py` & `simses-1.3.3/simses/commons/cycle_detection/cycle_detector.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/cycle_detection/half_cycle_detector.py` & `simses-1.3.3/simses/commons/cycle_detection/half_cycle_detector.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/cycle_detection/no_cycle_detector.py` & `simses-1.3.3/simses/commons/cycle_detection/no_cycle_detector.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/cycle_detection/rainflow_cycle_detector.py` & `simses-1.3.3/simses/commons/cycle_detection/rainflow_cycle_detector.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/data/csv_data_handler.py` & `simses-1.3.3/simses/commons/data/csv_data_handler.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/data/data_handler.py` & `simses-1.3.3/simses/commons/data/data_handler.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/data/no_data_handler.py` & `simses-1.3.3/simses/commons/data/no_data_handler.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/error.py` & `simses-1.3.3/simses/commons/error.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/log.py` & `simses-1.3.3/simses/commons/log.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/profile/economic/fcr.py` & `simses-1.3.3/simses/commons/profile/economic/fcr.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/profile/economic/intraday.py` & `simses-1.3.3/simses/commons/profile/economic/intraday.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/profile/economic/market.py` & `simses-1.3.3/simses/commons/profile/economic/market.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/profile/file.py` & `simses-1.3.3/simses/commons/profile/file.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     __SUPPORTED_EXTENSIONS: [str] = list()
     __SUPPORTED_EXTENSIONS.append(__EXT_CSV + __EXT_GZIP)
     __SUPPORTED_EXTENSIONS.append(__EXT_GZIP)
     __SUPPORTED_EXTENSIONS.append(__EXT_CSV)
 
     __ERROR = None
 
-    __URL: str = 'https://syncandshare.lrz.de/dl/fiDZgUQ5uygrVfHTwa7BxiEZ/Profile/'
+    __URL: str = 'https://syncandshare.lrz.de/dl/fiACpACzuTyoENQE2qwqrG/profiles/'
     """URL to folder of profiles to download"""
 
     def __init__(self, config: GeneralSimulationConfig, filename: str, delimiter: str = ',', scaling_factor: float = 1,
                  value_index: int = 1, interpolation: Interpolation = LinearInterpolation(),
                  average: Average = MeanAverage()):
         """
         Constructor of FileProfile
```

### Comparing `simses-1.3.2/simses/commons/profile/power/alternating.py` & `simses-1.3.3/simses/commons/profile/power/alternating.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/profile/power/constant.py` & `simses-1.3.3/simses/commons/profile/power/constant.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/profile/power/file.py` & `simses-1.3.3/simses/commons/profile/power/file.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/profile/power/generation.py` & `simses-1.3.3/simses/commons/profile/power/generation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/profile/power/load.py` & `simses-1.3.3/simses/commons/profile/power/load.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/profile/power/power_profile.py` & `simses-1.3.3/simses/commons/profile/power/power_profile.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/profile/power/random.py` & `simses-1.3.3/simses/commons/profile/power/random.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/profile/power/v2g_profile.py` & `simses-1.3.3/simses/commons/profile/power/v2g_profile.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/profile/technical/binary.py` & `simses-1.3.3/simses/commons/profile/technical/binary.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,16 +23,15 @@
         return self.__file.next(time)
 
 
     def next_change_in_binary(self, time: float, current_binary: bool) -> float:
 
         self.__file_copy = copy(self.__file) # Copy of file because the last value is saved in next-function
         time_copy = copy(time)
-        start_value = self.__file_copy.next(time_copy)
-        current_value = start_value
+        current_value = current_binary
         while bool(np.ceil(current_value)) == current_binary and time_copy <= self.__file_copy._FileProfile__end:
             # maximum until end of file
             time_copy += 1
             current_value = self.__file_copy.next(time_copy)
 
         self.__file_copy = None
```

### Comparing `simses-1.3.2/simses/commons/profile/technical/frequency.py` & `simses-1.3.3/simses/commons/profile/technical/frequency.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/profile/technical/soc.py` & `simses-1.3.3/simses/commons/profile/technical/soc.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/profile/technical/technical.py` & `simses-1.3.3/simses/commons/profile/technical/technical.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/state/abstract_state.py` & `simses-1.3.3/simses/commons/state/abstract_state.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/state/energy_management.py` & `simses-1.3.3/simses/commons/state/energy_management.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
     AC_POWER_REQUESTED = 'Power requested from EMS in W'
     LOAD_POWER = 'Load in W'
     PV_POWER = 'PV Generation in W'
     FCR_MAX_POWER = 'Power reserved for FCR in W'
     IDM_POWER = 'Power delivered for IDM in W'
     PEAKSHAVING_LIMIT = 'Peak Shaving Limit in W'
+    BINARY_VALUE = 'Binary value for EVs (1 available, 0 on the road)'
+    V2G_POWER = 'Power provided in V2G operation'
 
     def __init__(self):
         super().__init__()
         self._initialize()
 
     @property
     def ac_power_requested(self) -> float:
@@ -38,14 +40,30 @@
         return self.get(self.PV_POWER)
 
     @pv_power.setter
     def pv_power(self, value: float) -> None:
         self.set(self.PV_POWER, value)
 
     @property
+    def binary(self) -> float:
+        return self.get(self.BINARY_VALUE)
+
+    @binary.setter
+    def binary(self, value: float) -> None:
+        self.set(self.BINARY_VALUE, value)
+
+    @property
+    def v2g_power(self) -> float:
+        return self.get(self.V2G_POWER)
+
+    @v2g_power.setter
+    def v2g_power(self, value: float) -> None:
+        self.set(self.V2G_POWER, value)
+
+    @property
     def fcr_max_power(self) -> float:
         return self.get(self.FCR_MAX_POWER)
 
     @fcr_max_power.setter
     def fcr_max_power(self, value: float) -> None:
         self.set(self.FCR_MAX_POWER, value)
```

### Comparing `simses-1.3.2/simses/commons/state/parameters.py` & `simses-1.3.3/simses/commons/state/parameters.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/state/parameters_reader.py` & `simses-1.3.3/simses/commons/state/parameters_reader.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/state/system.py` & `simses-1.3.3/simses/commons/state/system.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,17 +5,17 @@
     """
     Current physical state of the system with the main electrical parameters.
     """
 
     SYSTEM_AC_ID = 'StorageSystemAC'
     SYSTEM_DC_ID = 'StorageSystemDC'
     AC_POWER = 'AC power in W'
-    PE_LOSSES = 'PE_losses in W'
+    PE_LOSSES = 'PE losses in W'
     AC_FULFILLMENT = 'AC Fulfillment in p.u.'
-    AC_POWER_DELIVERED = 'AC_P_delivered in W'
+    AC_POWER_DELIVERED = 'AC power delivered in W'
     # DC_VOLTAGE_INPUT = 'DC voltage input in V'
     # DC_VOLTAGE = 'DC voltage in V'
     DC_CURRENT = 'DC current in A'
     AUX_LOSSES = 'Aux losses in W'
     DC_POWER_INTERMEDIATE_CIRCUIT = 'DC power of intermediate circuit in W'
     DC_POWER_STORAGE = 'DC power of storage in W'
     DC_POWER_LOSS = 'DC power loss in W'
@@ -30,21 +30,42 @@
     MAX_DISCHARGE_POWER = 'Maximum discharging power in W'
 
     TEMPERATURE = 'Internal air temperature in K'
     AMBIENT_TEMPERATURE = 'Ambient temperature in K'
     HVAC_THERMAL_POWER = 'HVAC thermal power in W'
     SOLAR_THERMAL_LOAD = 'Solar irradiation thermal load in W'
 
+    # ACDC_TEMPERATURE = 'ACDC converter temperature in K'
+
+    OL_TEMPERATURE = 'Outer layer temperature in K'
+    IL_TEMPERATURE = 'Inner layer temperature in K'
+
     def __init__(self, system_id: int, storage_id: int):
         super().__init__()
         self._initialize()
         self.set(self.SYSTEM_AC_ID, system_id)
         self.set(self.SYSTEM_DC_ID, storage_id)
 
     @property
+    def ol_temperature(self) -> float:
+        return self.get(self.OL_TEMPERATURE)
+
+    @ol_temperature.setter
+    def ol_temperature(self, value: float) -> None:
+        self.set(self.OL_TEMPERATURE, value)
+
+    @property
+    def il_temperature(self) -> float:
+        return self.get(self.IL_TEMPERATURE)
+
+    @il_temperature.setter
+    def il_temperature(self, value: float) -> None:
+        self.set(self.IL_TEMPERATURE, value)
+
+    @property
     def ac_power(self) -> float:
         return self.get(self.AC_POWER)
 
     @ac_power.setter
     def ac_power(self, value: float) -> None:
         self.set(self.AC_POWER, value)
```

### Comparing `simses-1.3.2/simses/commons/state/technology/electrolyzer.py` & `simses-1.3.3/simses/commons/state/technology/electrolyzer.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/state/technology/fuel_cell.py` & `simses-1.3.3/simses/commons/state/technology/fuel_cell.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/state/technology/hydrogen.py` & `simses-1.3.3/simses/commons/state/technology/hydrogen.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/state/technology/lithium_ion.py` & `simses-1.3.3/simses/commons/state/technology/lithium_ion.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/state/technology/redox_flow.py` & `simses-1.3.3/simses/commons/state/technology/redox_flow.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/state/technology/storage.py` & `simses-1.3.3/simses/commons/state/technology/storage.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/test/test_constant_power_profile.py` & `simses-1.3.3/simses/commons/test/test_constant_power_profile.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/test/test_file_power_profile.py` & `simses-1.3.3/simses/commons/test/test_file_power_profile.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/test/test_linear_interpolation.py` & `simses-1.3.3/simses/commons/test/test_linear_interpolation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/test/test_mean_average.py` & `simses-1.3.3/simses/commons/test/test_mean_average.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/timeseries/average/average.py` & `simses-1.3.3/simses/commons/timeseries/average/average.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/timeseries/interpolation/interpolation.py` & `simses-1.3.3/simses/commons/timeseries/interpolation/interpolation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/timeseries/interpolation/last_value.py` & `simses-1.3.3/simses/commons/timeseries/interpolation/last_value.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/timeseries/interpolation/linear_interpolation.py` & `simses-1.3.3/simses/commons/timeseries/interpolation/linear_interpolation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/timeseries/timevalue.py` & `simses-1.3.3/simses/commons/timeseries/timevalue.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/utils/cell_reader.py` & `simses-1.3.3/simses/commons/utils/cell_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     __MAX_CHARGE_CURRENT: str = 'MaxChargeCurrentCont'
     __MAX_DISCHARGE_CURRENT: str = 'MaxDischargeCurrentCont'
     __MAX_VOLTAGE: str = 'EndOfChargeVoltage'
     __MIN_VOLTAGE: str = 'EndOfDischargeVoltage'
 
     __MODEL_LEVEL: str = 'ModelLevel'
     __ELECTRICAL_MODEL: str = 'ElectricalModel'
-    __ISEA_R2RC_DATA: str = 'ISEA_R2RC'
+    __ISEA_R2RC_DATA: str = 'ISEA_R_OCV'
     __CONFIGURATION: str = 'Configuration'
     __CUSTOM_DEFINITION: str = 'CustomDefinitions'
     # Kokam Cell End
 
     __OPEN_CIRCUIT_VOLTAGE: str = 'MyOCV'
     __OPEN_CIRCUIT_VOLTAGE_OBJECT: str = 'Object'
     __OCV_DATA: str = 'LookupData'
@@ -72,21 +72,28 @@
 
         nom_voltage: Element = self.__data_cell.get_element(self.__NOMINAL_VOLTAGE, electrical_param)
         nom_voltage_value: Element = self.__data_cell.get_element(self.__VALUE, nom_voltage)
         cell_voltage = self.__data_cell.parse(nom_voltage_value).item()  # V
 
         max_charge: Element = self.__data_cell.get_element(self.__MAX_CHARGE_CURRENT, electrical_param)
         max_charge_value: Element = self.__data_cell.get_element(self.__VALUE, max_charge)
-        max_charge_current = self.__data_cell.parse(max_charge_value).item()  # A
-        max_charge_rate = max_charge_current / cell_capacity  # 1/h
+        try:
+            max_charge_current = self.__data_cell.parse(max_charge_value).item()  # A
+            max_charge_rate = max_charge_current / cell_capacity  # 1/h
+        except ValueError: # if no value available
+            max_charge_rate = 0.5
 
         max_discharge: Element = self.__data_cell.get_element(self.__MAX_DISCHARGE_CURRENT, electrical_param)
         max_discharge_value: Element = self.__data_cell.get_element(self.__VALUE, max_discharge)
-        max_discharge_current = self.__data_cell.parse(max_discharge_value).item()  # A
-        max_discharge_rate = max_discharge_current / cell_capacity  # 1/h
+        try:
+            max_discharge_current = self.__data_cell.parse(max_discharge_value).item()  # A
+            max_discharge_rate = max_discharge_current / cell_capacity  # 1/h
+        except ValueError: # if no value available
+            max_discharge_rate = 0.5
+
 
         max_voltage_data: Element = self.__data_cell.get_element(self.__MAX_VOLTAGE, electrical_param)
         max_voltage_value: Element = self.__data_cell.get_element(self.__VALUE, max_voltage_data)
         max_voltage = self.__data_cell.parse(max_voltage_value).item()  # V
 
         min_voltage_data: Element = self.__data_cell.get_element(self.__MIN_VOLTAGE, electrical_param)
         min_voltage_value: Element = self.__data_cell.get_element(self.__VALUE, min_voltage_data)
```

### Comparing `simses-1.3.2/simses/commons/utils/converter_comparison.py` & `simses-1.3.3/simses/commons/utils/converter_comparison.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/utils/count_lines_of_code.py` & `simses-1.3.3/simses/commons/utils/count_lines_of_code.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/utils/fitting.py` & `simses-1.3.3/simses/commons/utils/fitting.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/utils/heatmap.py` & `simses-1.3.3/simses/commons/utils/heatmap.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/utils/max_peak_shaving_limit.py` & `simses-1.3.3/simses/commons/utils/max_peak_shaving_limit.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/utils/utilities.py` & `simses-1.3.3/simses/commons/utils/utilities.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/commons/utils/xml_reader.py` & `simses-1.3.3/simses/commons/utils/xml_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,17 @@
             for val in row.split(column_delimiter):
                 values.append(float(val))
             matrix.append(values)
         return numpy.array(matrix)
 
     def parse(self, element: Element, row_delimiter: str = ';', column_delimiter: str = ',') -> numpy.ndarray:
         value: str = self.get_value_from(element)
+        value = value.replace('\n', '')
+        value = value.replace('\t', '')
+
         if row_delimiter in value:
             return self.__parse_to_matrix(value, row_delimiter, column_delimiter)
         else:
             return self.__parse_to_array(value, column_delimiter)
 
     # # find the first 'item' object
     # for elem in root:
```

### Comparing `simses-1.3.2/simses/data/electrolyzer/evaluation/comparison_lut_ana_new_with_afterfitting.py` & `simses-1.3.3/simses/data/electrolyzer/evaluation/comparison_lut_ana_new_with_afterfitting.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/electrolyzer/evaluation/comparison_lut_ana_new_without_afterfitting.py` & `simses-1.3.3/simses/data/electrolyzer/evaluation/comparison_lut_ana_new_without_afterfitting.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/electrolyzer/evaluation/comparison_lut_no_current_influence_ana_new.py` & `simses-1.3.3/simses/data/electrolyzer/evaluation/comparison_lut_no_current_influence_ana_new.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/electrolyzer/evaluation/multi_dim_regression_current_dens_3rd_best_fit.py` & `simses-1.3.3/simses/data/electrolyzer/evaluation/multi_dim_regression_current_dens_3rd_best_fit.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/electrolyzer/lookuptable/activation_overpotential_lookup_alkaline.py` & `simses-1.3.3/simses/data/electrolyzer/lookuptable/activation_overpotential_lookup_alkaline.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/electrolyzer/lookuptable/archive/activation_overpotential_lookup_alkaline.csv.gz` & `simses-1.3.3/simses/data/electrolyzer/lookuptable/archive/activation_overpotential_lookup_alkaline.csv.gz`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/electrolyzer/lookuptable/archive/cell_currentdensity_lookup.csv.gz` & `simses-1.3.3/simses/data/electrolyzer/lookuptable/archive/cell_currentdensity_lookup.csv.gz`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/electrolyzer/lookuptable/archive/cell_voltage_lookup.csv.gz` & `simses-1.3.3/simses/data/electrolyzer/lookuptable/archive/cell_voltage_lookup.csv.gz`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/electrolyzer/lookuptable/archive/cell_voltage_lookup_alkaline.csv.gz` & `simses-1.3.3/simses/data/electrolyzer/lookuptable/archive/cell_voltage_lookup_alkaline.csv.gz`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/electrolyzer/lookuptable/archive/polarizationcurve_alkaline.py` & `simses-1.3.3/simses/data/electrolyzer/lookuptable/archive/polarizationcurve_alkaline.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/electrolyzer/lookuptable/cell_current_lookup_alkaline.gz` & `simses-1.3.3/simses/data/electrolyzer/lookuptable/cell_current_lookup_alkaline.gz`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/electrolyzer/lookuptable/multi_dim_polarizationcurve.py` & `simses-1.3.3/simses/data/electrolyzer/lookuptable/multi_dim_polarizationcurve.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/electrolyzer/lookuptable/multi_dim_polarizationcurve_no_current_influence_on_part_pressure.py` & `simses-1.3.3/simses/data/electrolyzer/lookuptable/multi_dim_polarizationcurve_no_current_influence_on_part_pressure.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/electrolyzer/lookuptable/polarizationcurve1bar.csv` & `simses-1.3.3/simses/data/electrolyzer/lookuptable/polarizationcurve1bar.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/electrolyzer/lookuptable/polarizationcurve_e_master.py` & `simses-1.3.3/simses/data/electrolyzer/lookuptable/polarizationcurve_e_master.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/electrolyzer/lookuptable/powercurve1bar.csv` & `simses-1.3.3/simses/data/electrolyzer/lookuptable/powercurve1bar.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/electrolyzer/lookuptable/ui_curves/activation_overpotential_alkaline/25°C.csv` & `simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/activation_overpotential_alkaline/25°C.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/electrolyzer/lookuptable/ui_curves/activation_overpotential_alkaline/90°C.csv` & `simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/activation_overpotential_alkaline/90°C.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/electrolyzer/lookuptable/ui_curves/general_alkaline/GHW 130°C at 30bar.csv` & `simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/general_alkaline/GHW 130°C at 30bar.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/23°C.csv` & `simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/23°C.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/35°C.csv` & `simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/35°C.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/40°C.csv` & `simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/40°C.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/45°C.csv` & `simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/45°C.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/53,5°C.csv` & `simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/53,5°C.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/electrolyzer/regression/cell_currentdensity_lookup.csv` & `simses-1.3.3/simses/data/electrolyzer/regression/cell_currentdensity_lookup.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/electrolyzer/regression/multi_dim_regression_current_dens.py` & `simses-1.3.3/simses/data/electrolyzer/regression/multi_dim_regression_current_dens.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/fuel_cell/polarizationcurve1bar.csv` & `simses-1.3.3/simses/data/fuel_cell/polarizationcurve1bar.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/fuel_cell/polarizationcurve_fc_jupiter.py` & `simses-1.3.3/simses/data/fuel_cell/polarizationcurve_fc_jupiter.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/fuel_cell/polarizationcurve_fc_master.py` & `simses-1.3.3/simses/data/fuel_cell/polarizationcurve_fc_master.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/fuel_cell/polarizationcurve_jupiter.csv` & `simses-1.3.3/simses/data/fuel_cell/polarizationcurve_jupiter.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/fuel_cell/powercurve1bar.csv` & `simses-1.3.3/simses/data/fuel_cell/powercurve1bar.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/fuel_cell/powercurve_jupiter.csv` & `simses-1.3.3/simses/data/fuel_cell/powercurve_jupiter.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/lithium_ion/cell/CLFP_Sony_US26650_OCV.csv` & `simses-1.3.3/simses/data/lithium_ion/cell/CLFP_Sony_US26650_OCV.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/lithium_ion/cell/CLFP_Sony_US26650_Rint.csv` & `simses-1.3.3/simses/data/lithium_ion/cell/CLFP_Sony_US26650_Rint.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/lithium_ion/cell/CLFP_Sony_US26650_capacity_decrease_param.csv` & `simses-1.3.3/simses/data/lithium_ion/cell/CLFP_Sony_US26650_capacity_decrease_param.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/lithium_ion/cell/CLFP_Sony_US26650_resistance_increase_param.csv` & `simses-1.3.3/simses/data/lithium_ion/cell/CLFP_Sony_US26650_resistance_increase_param.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/lithium_ion/cell/LG_INR18560MJ1_OCV.csv` & `simses-1.3.3/simses/data/lithium_ion/cell/LG_INR18560MJ1_OCV.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/lithium_ion/cell/LG_INR18650MJ1_closs_calendar_aging.csv` & `simses-1.3.3/simses/data/lithium_ion/cell/LG_INR18650MJ1_closs_calendar_aging.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/lithium_ion/cell/LG_INR18650MJ1_closs_cycling_aging.csv` & `simses-1.3.3/simses/data/lithium_ion/cell/LG_INR18650MJ1_closs_cycling_aging.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/lithium_ion/cell/LG_INR18650MJ1_rint_cycling_aging.csv` & `simses-1.3.3/simses/data/lithium_ion/cell/LG_INR18650MJ1_rint_cycling_aging.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/lithium_ion/cell/LTO_LMO_closs_cycling_aging.csv` & `simses-1.3.3/simses/data/lithium_ion/cell/LTO_LMO_closs_cycling_aging.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/lithium_ion/cell/LTO_LMO_rint_cycling_aging.csv` & `simses-1.3.3/simses/data/lithium_ion/cell/LTO_LMO_rint_cycling_aging.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/lithium_ion/cell/LTO_NMC_closs_calendar_aging.csv` & `simses-1.3.3/simses/data/lithium_ion/cell/LTO_NMC_closs_calendar_aging.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/lithium_ion/cell/LTO_NMC_closs_cycling_aging.csv` & `simses-1.3.3/simses/data/lithium_ion/cell/LTO_NMC_closs_cycling_aging.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/lithium_ion/cell/LTO_NMC_rint_calendar_aging.csv` & `simses-1.3.3/simses/data/lithium_ion/cell/LTO_NMC_rint_calendar_aging.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/lithium_ion/cell/LTO_NMC_rint_cycling_aging.csv` & `simses-1.3.3/simses/data/lithium_ion/cell/LTO_NMC_rint_cycling_aging.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/lithium_ion/cell/NCA_PanasonicNCR_OCV.csv` & `simses-1.3.3/simses/data/lithium_ion/cell/NCA_PanasonicNCR_OCV.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/lithium_ion/cell/NCA_PanasonicNCR_Rint.csv` & `simses-1.3.3/simses/data/lithium_ion/cell/NCA_PanasonicNCR_Rint.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/lithium_ion/cell/NMC_Akasol_OEM_Rint.csv` & `simses-1.3.3/simses/data/lithium_ion/cell/NMC_Akasol_OEM_Rint.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/lithium_ion/cell/NMC_Molicel_OCV.csv` & `simses-1.3.3/simses/data/lithium_ion/cell/NMC_Molicel_OCV.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/lithium_ion/cell/NMC_Molicel_Rint.csv` & `simses-1.3.3/simses/data/lithium_ion/cell/NMC_Molicel_Rint.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/lithium_ion/cell/NMC_Molicel_capacity_cal.csv` & `simses-1.3.3/simses/data/lithium_ion/cell/NMC_Molicel_capacity_cal.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/lithium_ion/cell/NMC_Molicel_capacity_cyc.csv` & `simses-1.3.3/simses/data/lithium_ion/cell/NMC_Molicel_capacity_cyc.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/lithium_ion/cell/NMC_Molicel_ri_cal.csv` & `simses-1.3.3/simses/data/lithium_ion/cell/NMC_Molicel_ri_cal.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/lithium_ion/cell/NMC_Molicel_ri_cyc.csv` & `simses-1.3.3/simses/data/lithium_ion/cell/NMC_Molicel_ri_cyc.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/lithium_ion/cell/NMC_Samsung_LabTest_cell_00_OCV.csv` & `simses-1.3.3/simses/data/lithium_ion/cell/NMC_Samsung_LabTest_cell_00_OCV.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/lithium_ion/cell/NMC_Samsung_LabTest_cell_00_Ri.csv` & `simses-1.3.3/simses/data/lithium_ion/cell/NMC_Samsung_LabTest_cell_00_Ri.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/lithium_ion/cell/NMC_Sanyo_OCV.csv` & `simses-1.3.3/simses/data/lithium_ion/cell/NMC_Sanyo_OCV.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/lithium_ion/cell/NMC_Sanyo_Rint.csv` & `simses-1.3.3/simses/data/lithium_ion/cell/NMC_Sanyo_Rint.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/lithium_ion/cell/Sodium_Ion_OCV_Green_Rock.csv` & `simses-1.3.3/simses/data/lithium_ion/cell/Sodium_Ion_OCV_Green_Rock.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/lithium_ion/cell/Sodium_Ion_Rint_Green_Rock.csv` & `simses-1.3.3/simses/data/lithium_ion/cell/Sodium_Ion_Rint_Green_Rock.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/logo/SimSES.png` & `simses-1.3.3/simses/data/logo/SimSES.png`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/power_electronics/sinamics_S120_efficiency.csv` & `simses-1.3.3/simses/data/power_electronics/sinamics_S120_efficiency.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/redox_flow/degradation/H2_Current_F1_Schweiss.csv` & `simses-1.3.3/simses/data/redox_flow/degradation/H2_Current_F1_Schweiss.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/redox_flow/degradation/H2_Current_F3_Schweiss.csv` & `simses-1.3.3/simses/data/redox_flow/degradation/H2_Current_F3_Schweiss.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/redox_flow/stack/SHUNT_CellStack_2250_40.csv` & `simses-1.3.3/simses/data/redox_flow/stack/SHUNT_CellStack_2250_40.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/redox_flow/stack/SHUNT_FILE_INDUSTRIAL_STACK_1500W.csv` & `simses-1.3.3/simses/data/redox_flow/stack/SHUNT_FILE_INDUSTRIAL_STACK_1500W.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/redox_flow/stack/SHUNT_FILE_INDUSTRIAL_STACK_9000W.csv` & `simses-1.3.3/simses/data/redox_flow/stack/SHUNT_FILE_INDUSTRIAL_STACK_9000W.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data/redox_flow/stack/SHUNT_HP_Stack.csv` & `simses-1.3.3/simses/data/redox_flow/stack/SHUNT_HP_Stack.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/data.defaults.ini` & `simses-1.3.3/simses/data.defaults.ini`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/logger.defaults.ini` & `simses-1.3.3/simses/logger.defaults.ini`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/logic/energy_management/energy_management_factory.py` & `simses-1.3.3/simses/logic/energy_management/energy_management_factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from simses.logic.energy_management.strategy.basic.residential_pv_feed_in_damp import ResidentialPvFeedInDamp
 from simses.logic.energy_management.strategy.basic.residential_pv_greedy import ResidentialPvGreedy
 from simses.logic.energy_management.strategy.basic.soc_follower import SocFollower
 from simses.logic.energy_management.strategy.basic.electric_vehicle_soc import ElectricVehicleSOC
 from simses.logic.energy_management.strategy.basic.electric_vehicle_v2g import ElectricVehicleV2G
 from simses.logic.energy_management.strategy.basic.use_all_renewable_energy import UseAllRenewableEnergy
 from simses.logic.energy_management.strategy.stacked.fcr_idm_recharge_stacked import FcrIdmRechargeStacked
-from simses.logic.energy_management.strategy.stacked.dynamic_multi_use import DynamicMultiUse
+from simses.logic.energy_management.strategy.stacked.parallel_multi_use_with_stealing import ParallelMultiUseWithStealing
 
 class EnergyManagementFactory:
     """
     Energy Management Factory to create the operation strategy of the ESS.
     """
 
     def __init__(self, config: ConfigParser, path: str = None):
@@ -85,15 +85,15 @@
 
         elif os == ResidentialPvGreedy.__name__:
             self.__log.debug('Creating operation strategy as ' + os)
             return ResidentialPvGreedy(self.load_profile(), self.generation_profile())
 
         elif os == ResidentialPvFeedInDamp.__name__:
             self.__log.debug('Creating operation strategy as ' + os)
-            return ResidentialPvFeedInDamp(self.load_profile(), self.__config_general, self.generation_profile())
+            return ResidentialPvFeedInDamp(self.load_profile(), self.__config_general, self.__config_profile)
 
         elif os == UseAllRenewableEnergy.__name__:
             self.__log.debug('Creating operation strategy as ' + os)
             return UseAllRenewableEnergy(self.generation_profile())
 
         elif os == EvChargerWithBuffer.__name__:
             self.__log.debug('Creating operation strategy as ' + os)
@@ -108,36 +108,35 @@
             return ElectricVehicleSOC(self.__config_general, self.__config_profile, self.__config_ems)
 
         elif os == ElectricVehicleV2G.__name__:
             self.__log.debug('Creating operation strategy as ' + os)
             return ElectricVehicleV2G(self.__config_general, self.__config_profile, self.__config_ems, self.load_profile(),
                                       self.v2g_profile())
 
-        elif os == DynamicMultiUse.__name__:
+        elif os == ParallelMultiUseWithStealing.__name__:
             self.__log.debug('Creating operation strategy as ' + os)
-            return DynamicMultiUse(self.__config_general, self.__config_profile, self.__config_ems, self.load_profile(),
+            return ParallelMultiUseWithStealing(self.__config_general, self.__config_profile, self.__config_ems, self.load_profile(),
                                    self.__config_battery, self.generation_profile(), self.__config_system)
 
         else:
             options: [str] = list()
             options.append(FrequencyContainmentReserve.__name__)
             options.append(IntradayMarketRecharge.__name__)
             options.append(SimplePeakShaving.__name__)
             options.append(PeakShavingPerfectForesight.__name__)
             options.append(PowerFollower.__name__)
             options.append(SocFollower.__name__)
             options.append(FcrIdmRechargeStacked.__name__)
             options.append(ResidentialPvGreedy.__name__)
             options.append(ResidentialPvFeedInDamp.__name__)
-            options.append(FcrIdmPeakShavingSerial.__name__)
             options.append(EvChargerWithBuffer.__name__)
             options.append(ElectricVehicle.__name__)
             options.append(ElectricVehicleSOC.__name__)
             options.append(ElectricVehicleV2G.__name__)
-            options.append(DynamicMultiUse.__name__)
+            options.append(ParallelMultiUseWithStealing.__name__)
             raise Exception('Operation strategy ' + os + ' is unknown. '
                                                          'Following options are available: ' + str(options))
 
     def generation_profile(self) -> GenerationProfile:
         return GenerationProfile(self.__config_profile, self.__config_general)
 
     def binary_profile(self) -> BinaryProfile:
```

### Comparing `simses-1.3.2/simses/logic/energy_management/energy_management_system.py` & `simses-1.3.3/simses/logic/energy_management/energy_management_system.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/logic/energy_management/strategy/basic/electric_vehicle.py` & `simses-1.3.3/simses/logic/energy_management/strategy/basic/electric_vehicle_v2g.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from simses.commons.config.simulation.general import GeneralSimulationConfig
 from simses.commons.profile.power.power_profile import PowerProfile
+from simses.commons.profile.power.v2g_profile import V2GProfile
 from simses.commons.profile.technical.binary import BinaryProfile
 from simses.commons.config.simulation.profile import ProfileConfig
 from simses.commons.config.simulation.energy_management import EnergyManagementConfig
 from simses.commons.state.energy_management import EnergyManagementState
 from simses.commons.state.system import SystemState
 from simses.logic.energy_management.strategy.operation_priority import OperationPriority
 from simses.logic.energy_management.strategy.operation_strategy import OperationStrategy
 import numpy as np
 
 
-class ElectricVehicle(OperationStrategy):
+class ElectricVehicleV2G(OperationStrategy):
 
     """
     ElectricVehicle is a basic operation strategy which simulates an EV during trips and recharge. The algorithm
     requires the following profiles and parameters:
     - A load profile that contains the required (and recuperated) power while driving
     - A binary profile that contains ones when the EV is parked & can be charged and zeros if not
     - A string for the parameter 'EV_CHARGING_STRATEGY' which can be:
@@ -29,40 +30,47 @@
     - Using load and binary profile from emobpy, the LOAD_SCALING_FACTOR in [PROFILE] section should be set to 1
 
     Whenever the EV is not parked & ready to charge (binary=0), the EMS just follows the load profile.
     If the car is parked & ready to charge (binary=1), it is recharged depending on 'EV_CHARGING_STRATEGY'.
     """
 
     def __init__(self, config: GeneralSimulationConfig, profile_config: ProfileConfig, ems_config: EnergyManagementConfig,
-                 power_profile: PowerProfile):
+                 power_profile: PowerProfile, v2g_profile: V2GProfile):
 
         super().__init__(OperationPriority.MEDIUM)
 
         self.__load_profile_driving: PowerProfile = power_profile
         self.__binary_profile = BinaryProfile(config, profile_config)
+        self.__v2g_profile: V2GProfile = v2g_profile
 
         self.__power: float = 0.0
         self.__binary: bool = False
         self.__soc_to_charge: float = 0.0
         self.__charging_strategy = ems_config.ev_charging_strategy
         self.__max_ac_grid_power = ems_config.max_power
         self.__fast_charging_event = 0
         self.__time_counter_postponed_trip = 0
         self.__postponed_trip = []
         self.__Wh_to_Ws = 3600
         self.__next_time_zero = None
         self.__timestep = config.timestep
+        self.__flag_reload_in_action = False
+        self.__helper_class = HelperClassForProfileCopies(config, profile_config, ems_config)
+        if self.__charging_strategy[0:6] == 'Paused':
+            self.__threshold = float(self.__charging_strategy[-3:])
+        if self.__charging_strategy[0:3] == 'V2G':
+            temp = self.__charging_strategy.split(', ')
+            self.__ev_pool_size = float(temp[2])
+            self.__threshold_minimum_for_mobility = float(temp[1])
 
+        self.__ev_v2g_power_applied = 0
 
     def next(self, time: float, system_state: SystemState, power: float = 0) -> float:
         self.__power = self.__load_profile_driving.next(time)
-        temp_binary = np.round(self.__binary_profile.next(time))
-        if temp_binary!=0 and temp_binary!=1:
-            raise ValueError("The binary profile contains values different from 0 or 1!")
-        self.__binary = bool(temp_binary)
+        self.__binary = bool(np.round(self.__binary_profile.next(time)))
 
         if self.__binary != False and self.__binary != True:
             raise ValueError("The binary profile contains values different from 0 or 1!")
 
         if not self.__binary:                      # if EV is not at home: use load profile value
             # Possibly binary profile must also be shifted if fast charging is required on a long trip!
             # Right now, the break for fast charging is neglected (trip becomes shorter)
@@ -72,63 +80,107 @@
                 self.__fast_charging_event = 0
 
             if self.__fast_charging_event == 1:
                 self.__postponed_trip.append(-1.0 * self.__power)
 
                 power = 150000
             else:
-                # if len(self.__postponed_trip):
+                #if len(self.__postponed_trip):
                 #    power = self.__postponed_trip.pop(0)
                 #    self.__postponed_trip.append(-1.0 * self.__power)
-                # else:
+                #else:
                 power = 1.0 * self.__power
         elif system_state.soc == 1:                 # if EV is at home and SOC=100%: do nothing
             power = 0
         elif self.__charging_strategy == 'Uncontrolled':   # if EV is at home and SOC!=100%: Recharge with charging strategy
             power = self.__max_ac_grid_power
 
         elif self.__charging_strategy == 'Mean_power':  # Charge with mean power to be fully charged at departure time
 
-            if self.__next_time_zero == None:
-                self.__next_time_zero = self.__binary_profile.next_zero(time)
+            if self.__next_time_zero is None:
+                self.__next_time_zero = self.__helper_class.binary_change_function(time, self.__binary)
 
             charging_duration = self.__next_time_zero - time
             capacity_to_charge = (1 - system_state.soc) * system_state.capacity * self.__Wh_to_Ws
             if charging_duration > 0:
                 power = capacity_to_charge / charging_duration
             else:
-                power=0
+                power = self.__max_ac_grid_power
+                self.__next_time_zero = None
 
-            if charging_duration == self.__timestep:
+            if charging_duration <= self.__timestep:
                 self.__next_time_zero = None
 
 
         elif self.__charging_strategy[0:6] == 'Paused':
-            threshold = float(self.__charging_strategy[-3:])
-            if system_state.soc < threshold:
+            if system_state.soc < self.__threshold:
                 power = self.__max_ac_grid_power
             else:
-                if self.__next_time_zero == None:
-                    self.__next_time_zero = self.__binary_profile.next_zero(time)
+                if self.__next_time_zero is None:
+                    self.__next_time_zero = self.__helper_class.binary_change_function(time, self.__binary)
                 else:
                     charging_duration = (1-system_state.soc)*system_state.capacity*self.__Wh_to_Ws/self.__max_ac_grid_power
                     charging_restart_time = self.__next_time_zero - charging_duration - 1800
                     # start recharging after the pause, buffer of 30 minutes (1800s)
                     if time < charging_restart_time:
                         power = 0
                     else:
                         power = self.__max_ac_grid_power
                         if self.__next_time_zero - time < self.__timestep:
                             self.__next_time_zero = None
 
+        elif self.__charging_strategy[0:3] == 'V2G':
+            self.__v2g_power = self.__v2g_profile.next(time)
+            self.__ev_v2g_power_applied = 0
+            threshold_charge_to_when_under_minimum = 0.7
+
+            if system_state.soc < self.__threshold_minimum_for_mobility:
+                power = self.__max_ac_grid_power
+                self.__flag_reload_in_action = True
+            elif system_state.soc < threshold_charge_to_when_under_minimum and self.__flag_reload_in_action is True:
+                power = self.__max_ac_grid_power
+            else:
+                self.__flag_reload_in_action = False
+                if self.__next_time_zero is None:
+                    self.__next_time_zero = self.__helper_class.binary_change_function(time, self.__binary)
+                else:
+                    charging_duration = (1 - system_state.soc) * system_state.capacity * self.__Wh_to_Ws / self.__max_ac_grid_power
+                    charging_restart_time = self.__next_time_zero - charging_duration - 1800
+                    # start recharging after the pause, buffer of 30 minutes (1800s)
+                    if time < charging_restart_time:
+                        power = self.__v2g_power / self.__ev_pool_size
+                        self.__ev_v2g_power_applied = power
+                    else:
+                        power = self.__max_ac_grid_power
+                        if self.__next_time_zero - time < self.__timestep:
+                            self.__next_time_zero = None
 
         return power
 
     def update(self, energy_management_state: EnergyManagementState) -> None:
         energy_management_state.load_power = self.__power
+        energy_management_state.binary = int(self.__binary)
+        energy_management_state.v2g_power = self.__ev_v2g_power_applied
 
     def clear(self) -> None:
         self.__power = 0.0
 
     def close(self) -> None:
         self.__binary_profile.close()
         self.__load_profile_driving.close()
+
+
+class HelperClassForProfileCopies:
+
+    def __init__(self, config: GeneralSimulationConfig, profile_config: ProfileConfig, ems_config: EnergyManagementConfig):
+
+        # open second soc and binary profile for forecasts
+        # This is necessary, as next function of profiles of instance of ElectricVehicleSOC-class saves previous values
+        # Thus, those profiles cannot be used for forecasting SOC or binary values
+        self.__binary_profile_copy = BinaryProfile(config, profile_config)
+        self.__timestep = config.timestep
+
+    def binary_change_function(self, time, current_binary):
+        # This function returns the time when the binary profile changes its value
+        # from 0 to 1 or 1 to 0
+
+        return self.__binary_profile_copy.next_change_in_binary(time, current_binary)
```

### Comparing `simses-1.3.2/simses/logic/energy_management/strategy/basic/electric_vehicle_soc.py` & `simses-1.3.3/simses/logic/energy_management/strategy/basic/electric_vehicle.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,220 +1,174 @@
-import datetime
-
 from simses.commons.config.simulation.general import GeneralSimulationConfig
+from simses.commons.profile.power.power_profile import PowerProfile
+from simses.commons.profile.technical.binary import BinaryProfile
 from simses.commons.config.simulation.profile import ProfileConfig
-from simses.commons.profile.technical.soc import SocProfile
+from simses.commons.config.simulation.energy_management import EnergyManagementConfig
 from simses.commons.state.energy_management import EnergyManagementState
 from simses.commons.state.system import SystemState
 from simses.logic.energy_management.strategy.operation_priority import OperationPriority
 from simses.logic.energy_management.strategy.operation_strategy import OperationStrategy
-from simses.commons.profile.technical.binary import BinaryProfile
-from simses.commons.config.simulation.energy_management import EnergyManagementConfig
 import numpy as np
-from copy import copy
 
-class ElectricVehicleSOC(OperationStrategy):
+class ElectricVehicle(OperationStrategy):
 
     """
-    ElectricVehicleSOC is a basic operation strategy which simulates an EV during trips and recharge. The algorithm
+    ElectricVehicle is a basic operation strategy which simulates an EV during trips and recharge. The algorithm
     requires the following profiles and parameters:
-    - An SOC profile that contains the SOC of the vehicle. The charging of the vehicle can be changed but also the
-    original charging SOC-change can be used
-    - A binary profile that contains ones when the EV is parked at home and zeros if not
+    - A load profile that contains the required (and recuperated) power while driving
+    - A binary profile that contains ones when the EV is parked & can be charged and zeros if not
     - A string for the parameter 'EV_CHARGING_STRATEGY' which can be:
-        - "Original": Uses the original SOC-values for the charging
         - "Uncontrolled": Always recharge, if SOC<100% and parked at "home"
         - "Mean_Power": This strategy checks the next departure time (perfect foresight) and chooses the charging power
             to reach 100% SOC exactly at departure time.
         - "Paused, integer threshold value": This strategy charges immediately after arrival until a threshold value
             (e.g. 0.8 -> 80% SOC). Then the charging is paused. The charging continues with maximal grid power at the
             time (t = Delta_E/P) that allows 100% SOC to be reached at the next departure time (with 30 minutes buffer).
+
     - The maximal grid power is set in the 'ENERGY_MANAGEMENT' section as 'MAX_POWER'
+    - Using load and binary profile from emobpy, the LOAD_SCALING_FACTOR in [PROFILE] section should be set to 1
 
-    Whenever the EV is not at home, the EMS just follows the load profile. If the car is parked at home, it is
-    recharged depending on 'EV_CHARGING_STRATEGY'. The algorithm can also be used for electric buses.
+    Whenever the EV is not parked & ready to charge (binary=0), the EMS just follows the load profile.
+    If the car is parked & ready to charge (binary=1), it is recharged depending on 'EV_CHARGING_STRATEGY'.
     """
 
-    def __init__(self, config: GeneralSimulationConfig, profile_config: ProfileConfig, ems_config: EnergyManagementConfig):
+    def __init__(self, config: GeneralSimulationConfig, profile_config: ProfileConfig, ems_config: EnergyManagementConfig,
+                 power_profile: PowerProfile):
+
         super().__init__(OperationPriority.MEDIUM)
 
-        self.__soc_profile = SocProfile(config, profile_config) # SOC profile is used in this strategy
+        self.__load_profile_driving: PowerProfile = power_profile
         self.__binary_profile = BinaryProfile(config, profile_config)
-        self.__soc: float = 0.0
+
+        self.__power: float = 0.0
         self.__binary: bool = False
+        self.__soc_to_charge: float = 0.0
         self.__charging_strategy = ems_config.ev_charging_strategy
-        self.__max_ac_grid_power = ems_config.max_power  # Here maximal grid power
-
-        self.__timestep = config.timestep
+        self.__max_ac_grid_power = ems_config.max_power
+        self.__fast_charging_event = 0
+        self.__time_counter_postponed_trip = 0
+        self.__postponed_trip_power = []
+        self.__postponed_trip_binary = []
+        self.__postponed_time = 0
         self.__Wh_to_Ws = 3600
         self.__next_time_zero = None
-        self.__soc_at_nextzero = None
-        self.__target_soc = None
+        self.__timestep = config.timestep
 
         self.__helper_class = HelperClassForProfileCopies(config, profile_config, ems_config)
+        if self.__charging_strategy[0:6] == 'Paused':
+            self.__threshold = float(self.__charging_strategy[-3:])
 
     def next(self, time: float, system_state: SystemState, power: float = 0) -> float:
-
-        self.__soc = self.__soc_profile.next(time) # SOC
-        if self.__soc < 0:
-            print("Error: Desired SOC < 0")
-
+        self.__power = self.__load_profile_driving.next(time)
         temp_binary = np.ceil(self.__binary_profile.next(time))
-        # rounds binary upwards. If interpolation/no data available and next existing value is 1 all values inbetween
-        # are denoted as 1. Thus, charging is possible.
         if temp_binary!=0 and temp_binary!=1:
             raise ValueError("The binary profile contains values different from 0 or 1!")
         self.__binary = bool(temp_binary)
 
-        if not self.__binary: # EV is driving
-
-            soc_dif = self.__soc - system_state.soc
-            capacity_dif = soc_dif * system_state.capacity * self.__Wh_to_Ws
-            power = capacity_dif / self.__timestep
-            # E-Bus profile contained weired changes of SOC (Delta >0) while driving (not recuperation!?)
-            # which is why a student differentiated here: if soc_dif > 0 => power=0
-
-        else: # EV is parked
-            if np.round(system_state.soc,5)==1: # if already fully charged
-                power = 0
-            elif self.__charging_strategy == 'Original': # just follow SOC
-                soc_dif = self.__soc - system_state.soc
-                capacity_dif = soc_dif * system_state.capacity * self.__Wh_to_Ws
-                power = capacity_dif / self.__timestep
-
-            elif self.__charging_strategy == 'Uncontrolled_to_target_SOC': # Charge with full power to reach a target SOC
-
-                if self.__next_time_zero == None:
-                    self.__next_time_zero = self.__helper_class.binary_change_function(time, self.__binary)
-                    if self.__next_time_zero >= time + self.__timestep:
-                        self.__target_soc = self.__helper_class.specific_time_soc(time, self.__next_time_zero)
-                    else:
-                        self.__target_soc = self.__soc
-
-                if system_state.soc < self.__target_soc:
-                    power = self.__max_ac_grid_power    # charge with max power
-                else:
-                    power = 0
-
-                if self.__next_time_zero - time <= self.__timestep:
-                    self.__next_time_zero = None
-
-
-            elif self.__charging_strategy == 'Mean_to_target_SOC': # Charge with mean power to be at target soc at departure time
-
-                if self.__next_time_zero == None:
-                    self.__next_time_zero = self.__binary_profile.next_change_in_binary(time, self.__binary)
-
-                charging_duration = self.__next_time_zero - time
-                self.__soc_profile_copy = copy(self.__soc_profile)
-                target_soc = self.__soc_profile_copy.next(self.__next_time_zero)
-                self.__soc_profile_copy = None
-                capacity_to_charge = (target_soc - system_state.soc) * system_state.capacity * self.__Wh_to_Ws
-                if charging_duration > 0:
-                    power = capacity_to_charge / charging_duration
-                else:
-                    power = self.__max_ac_grid_power
-                    self.__next_time_zero = None
-
-                if charging_duration <= self.__timestep:
-                    self.__next_time_zero = None
-
-
-            elif self.__charging_strategy == 'Paused_to_target_SOC': # Charge with mean power to be at target soc at departure time
-
-                if self.__next_time_zero == None:
-                    self.__next_time_zero = self.__binary_profile.next_change_in_binary(time, self.__binary)
-
-                    self.__soc_profile_copy = copy(self.__soc_profile)
-                    self.__target_soc = self.__soc_profile_copy.next(self.__next_time_zero)
-                    self.__soc_profile_copy = None
+        if self.__binary != False and self.__binary != True:
+            raise ValueError("The binary profile contains values different from 0 or 1!")
 
-                if system_state.soc < self.__target_soc:
-                    power = self.__max_ac_grid_power    # charge with max power
+        if not self.__binary or self.__fast_charging_event > 0: # if EV is not at home: use load profile value
+            # Possibly binary profile must also be shifted if fast charging is required on a long trip!
+            # Right now, the break for fast charging is neglected (trip becomes shorter)
+            if system_state.soc < 0.02:
+                self.__fast_charging_event = 1  # if fast_charging has to start
+                if self.__binary == 0:
+                    self.__next_time_binary_one = self.__helper_class.binary_change_function(time, self.__binary)
+
+            elif system_state.soc > 0.80 and self.__fast_charging_event == 1:
+                self.__fast_charging_event = 2  # if fast_charging has happened and postponed period starts
+                self.__postponed_time = len(self.__postponed_trip_power) * self.__timestep
+                # Find next time when binary==1
+                if self.__binary == 0:
+                    self.__next_time_binary_one = self.__helper_class.binary_change_function(time, self.__binary)
+
+            if self.__fast_charging_event == 0:
+                power = self.__power    # normal case
+
+            elif self.__fast_charging_event == 1:
+                # 1st phase of fast-charging: charging with 150 kW (if possible by car) and save old power_values
+                self.__postponed_trip_power.append(self.__power)
+                self.__binary = True
+                power = 150000
+
+            elif self.__fast_charging_event == 2:
+                # 2nd phase of fast-charging: apply old power_values and save current value from profile
+                if time < self.__next_time_binary_one + self.__postponed_time:
+                   power = self.__postponed_trip_power.pop(0)
+                   self.__postponed_trip_power.append(self.__power)
                 else:
-                    power = 0
-
-                if self.__next_time_zero - time <= self.__timestep:
-                    self.__next_time_zero = None
-
-
-
-            elif self.__charging_strategy == 'Uncontrolled': # Recharge with max AC power when parked
+                    self.__fast_charging_event = 0
+                    power = self.__power
+                    self.__postponed_trip_power = []
+                self.__binary = False
+
+        elif system_state.soc == 1:                 # if EV is at home and SOC=100%: do nothing
+            power = 0
+        elif self.__charging_strategy == 'Uncontrolled':   # if EV is at home and SOC!=100%: Recharge with charging strategy
+            power = self.__max_ac_grid_power
+
+        elif self.__charging_strategy == 'Mean_power':  # Charge with mean power to be fully charged at departure time
+
+            if self.__next_time_zero is None:
+                self.__next_time_zero = self.__helper_class.binary_change_function(time, self.__binary)
+
+            charging_duration = self.__next_time_zero - time
+            capacity_to_charge = (1 - system_state.soc) * system_state.capacity * self.__Wh_to_Ws
+            if charging_duration > 0:
+                power = capacity_to_charge / charging_duration
+            else:
                 power = self.__max_ac_grid_power
+                self.__next_time_zero = None
 
-            elif self.__charging_strategy == 'Mean_power': # Charge with mean power to be fully charged at departure time
+            if charging_duration <= self.__timestep:
+                self.__next_time_zero = None
 
-                if self.__next_time_zero == None:
-                    self.__next_time_zero = self.__binary_profile.next_change_in_binary(time, self.__binary)
 
-                charging_duration = self.__next_time_zero - time
-                capacity_to_charge = (1 - system_state.soc) * system_state.capacity * self.__Wh_to_Ws
-                if charging_duration > 0:
-                    power = capacity_to_charge / charging_duration
-                else:
-                    power = self.__max_ac_grid_power
+        elif self.__charging_strategy[0:6] == 'Paused':
 
-                if charging_duration == self.__timestep:
-                    self.__next_time_zero = None
-
-            elif self.__charging_strategy[0:6] == 'Paused':
-                threshold = float(self.__charging_strategy[-3:])
-                if system_state.soc < threshold:
-                    power = self.__max_ac_grid_power
+            if system_state.soc < self.__threshold:
+                power = self.__max_ac_grid_power
+            else:
+                if self.__next_time_zero is None:
+                    self.__next_time_zero = self.__helper_class.binary_change_function(time, self.__binary)
                 else:
-                    if self.__next_time_zero == None:
-                        self.__next_time_zero = self.__binary_profile.next_change_in_binary(time, self.__binary)
+                    charging_duration = (1-system_state.soc)*system_state.capacity*self.__Wh_to_Ws/self.__max_ac_grid_power
+                    charging_restart_time = self.__next_time_zero - charging_duration - 1800
+                    # start recharging after the pause, buffer of 30 minutes (1800s)
+                    if time < charging_restart_time:
+                        power = 0
                     else:
-                        charging_duration = (1-threshold)*system_state.capacity*self.__Wh_to_Ws/self.__max_ac_grid_power
-                        charging_restart_time = self.__next_time_zero - charging_duration - 1800
-                        # start recharging after the pause, buffer of 30 minutes (1800s)
-                        if time < charging_restart_time:
-                            power = 0
-                        else:
-                            power = self.__max_ac_grid_power
-                            if self.__next_time_zero - time < self.__timestep:
-                                self.__next_time_zero = None
-        return power
+                        power = self.__max_ac_grid_power
+                        if self.__next_time_zero - time < self.__timestep:
+                            self.__next_time_zero = None
 
+        return power
 
     def update(self, energy_management_state: EnergyManagementState) -> None:
-        pass
+        energy_management_state.load_power = self.__power
+        energy_management_state.binary = int(self.__binary)
 
     def clear(self) -> None:
-        pass
+        self.__power = 0.0
 
     def close(self) -> None:
-        self.__soc_profile.close()
         self.__binary_profile.close()
+        self.__load_profile_driving.close()
+
 
 
 class HelperClassForProfileCopies:
 
     def __init__(self, config: GeneralSimulationConfig, profile_config: ProfileConfig, ems_config: EnergyManagementConfig):
 
         # open second soc and binary profile for forecasts
         # This is necessary, as next function of profiles of instance of ElectricVehicleSOC-class saves previous values
         # Thus, those profiles cannot be used for forecasting SOC or binary values
-        self.__soc_profile_copy = SocProfile(config, profile_config)
         self.__binary_profile_copy = BinaryProfile(config, profile_config)
         self.__timestep = config.timestep
 
     def binary_change_function(self, time, current_binary):
         # This function returns the time when the binary profile changes its value
         # from 0 to 1 or 1 to 0
 
         return self.__binary_profile_copy.next_change_in_binary(time, current_binary)
-
-    def specific_time_soc(self, current_time, target_time) -> float:
-        # This function returns the soc value of a specific point in time
-
-        for time_counter in range(int(current_time), int(target_time),int(self.__timestep)):
-            soc = self.__soc_profile_copy.next(time_counter)
-
-        if 'soc' not in locals():
-            soc = 1
-            print('Error in specific_time_soc of HelperClassForProfileCopies of ElectricVehicleSOC. '
-                  'Is target time > current time?')
-
-        return soc
-
-
```

### Comparing `simses-1.3.2/simses/logic/energy_management/strategy/basic/electric_vehicle_v2g.py` & `simses-1.3.3/simses/logic/energy_management/strategy/basic/peak_shaving_perfect_foresight.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,134 +1,154 @@
+import numpy as np
+
+from simses.commons.config.simulation.energy_management import EnergyManagementConfig
 from simses.commons.config.simulation.general import GeneralSimulationConfig
-from simses.commons.profile.power.power_profile import PowerProfile
-from simses.commons.profile.power.v2g_profile import V2GProfile
-from simses.commons.profile.technical.binary import BinaryProfile
 from simses.commons.config.simulation.profile import ProfileConfig
-from simses.commons.config.simulation.energy_management import EnergyManagementConfig
+from simses.commons.config.simulation.system import StorageSystemConfig
+from simses.commons.profile.power.power_profile import PowerProfile
 from simses.commons.state.energy_management import EnergyManagementState
 from simses.commons.state.system import SystemState
 from simses.logic.energy_management.strategy.operation_priority import OperationPriority
 from simses.logic.energy_management.strategy.operation_strategy import OperationStrategy
-import numpy as np
 
 
-class ElectricVehicleV2G(OperationStrategy):
-
+class PeakShavingPerfectForesight(OperationStrategy):
     """
-    ElectricVehicle is a basic operation strategy which simulates an EV during trips and recharge. The algorithm
-    requires the following profiles and parameters:
-    - A load profile that contains the required (and recuperated) power while driving
-    - A binary profile that contains ones when the EV is parked & can be charged and zeros if not
-    - A string for the parameter 'EV_CHARGING_STRATEGY' which can be:
-        - "Uncontrolled": Always recharge, if SOC<100% and parked at "home"
-        - "Mean_Power": This strategy checks the next departure time (perfect foresight) and chooses the charging power
-            to reach 100% SOC exactly at departure time.
-        - "Paused, integer threshold value": This strategy charges immediately after arrival until a threshold value
-            (e.g. 0.8 -> 80% SOC). Then the charging is paused. The charging continues with maximal grid power at the
-            time (t = Delta_E/P) that allows 100% SOC to be reached at the next departure time (with 30 minutes buffer).
-
-    - The maximal grid power is set in the 'ENERGY_MANAGEMENT' section as 'MAX_POWER'
-    - Using load and binary profile from emobpy, the LOAD_SCALING_FACTOR in [PROFILE] section should be set to 1
-
-    Whenever the EV is not parked & ready to charge (binary=0), the EMS just follows the load profile.
-    If the car is parked & ready to charge (binary=1), it is recharged depending on 'EV_CHARGING_STRATEGY'.
+        Peak Shaving under the assumption of perfect foresight for the load profile in order to reduce calendar
+        degradation.
+        The BESS will only charge up to the energy that is needed for the next load peak, right before the load peak
+        occurs.
     """
-
-    def __init__(self, config: GeneralSimulationConfig, profile_config: ProfileConfig, ems_config: EnergyManagementConfig,
-                 power_profile: PowerProfile, v2g_profile: V2GProfile):
-
-        super().__init__(OperationPriority.MEDIUM)
-
-        self.__load_profile_driving: PowerProfile = power_profile
-        self.__binary_profile = BinaryProfile(config, profile_config)
-        self.__v2g_profile: V2GProfile = v2g_profile
-
-        self.__power: float = 0.0
-        self.__binary: bool = False
-        self.__soc_to_charge: float = 0.0
-        self.__charging_strategy = ems_config.ev_charging_strategy
-        self.__max_ac_grid_power = ems_config.max_power
-        self.__fast_charging_event = 0
-        self.__time_counter_postponed_trip = 0
-        self.__postponed_trip = []
-        self.__Wh_to_Ws = 3600
-        self.__next_time_zero = None
-        self.__timestep = config.timestep
-
+    def __init__(self, general_config: GeneralSimulationConfig, power_profile: PowerProfile, forecast_profile: PowerProfile,
+                 energy_management_config: EnergyManagementConfig, system_config: StorageSystemConfig,
+                 profile_config: ProfileConfig):
+        super().__init__(OperationPriority.VERY_HIGH)
+
+        # configurable
+        self.__efficiency = 0.9
+        self.__soc_margin = 0.1  # to prevent missing peaks due to non-accurate efficiency
+        forecasting_time_hours = 72  # select forecast time for data horizon in the future that is considered
+        forecasting_steps = int(round(forecasting_time_hours*60*60 / general_config.timestep))
+
+        self.__load_profile = power_profile
+        self.__delta_t = general_config.timestep
+        self.__ps_limit: float = energy_management_config.max_power
+        nameplate_power = 0
+        for system in system_config.storage_systems_ac:
+            nameplate_power += float(system[1])
+        self.__peak_energy_forecaster = PeakEnergyForecaster(forecast_profile, forecasting_steps, self.__ps_limit, nameplate_power,
+                                                             self.__efficiency, general_config, profile_config)
+        self.__power = 0
 
     def next(self, time: float, system_state: SystemState, power: float = 0) -> float:
-        self.__power = self.__load_profile_driving.next(time)
-        self.__binary = bool(np.round(self.__binary_profile.next(time)))
-        self.__v2g_power = self.__v2g_profile.next(time)
-
-        if self.__binary != False and self.__binary != True:
-            raise ValueError("The binary profile contains values different from 0 or 1!")
-
-        if not self.__binary:                      # if EV is not at home: use load profile value
-            # Possibly binary profile must also be shifted if fast charging is required on a long trip!
-            # Right now, the break for fast charging is neglected (trip becomes shorter)
-            if system_state.soc < 0.02:
-                self.__fast_charging_event = 1
-            if system_state.soc > 0.80:
-                self.__fast_charging_event = 0
-
-            if self.__fast_charging_event == 1:
-                self.__postponed_trip.append(-1.0 * self.__power)
-
-                power = 150000
-            else:
-                #if len(self.__postponed_trip):
-                #    power = self.__postponed_trip.pop(0)
-                #    self.__postponed_trip.append(-1.0 * self.__power)
-                #else:
-                power = 1.0 * self.__power
-        elif system_state.soc == 1:                 # if EV is at home and SOC=100%: do nothing
-            power = 0
-        elif self.__charging_strategy == 'Uncontrolled':   # if EV is at home and SOC!=100%: Recharge with charging strategy
-            power = self.__max_ac_grid_power
-
-        elif self.__charging_strategy == 'Mean_power':  # Charge with mean power to be fully charged at departure time
-
-            if self.__next_time_zero == None:
-                self.__next_time_zero = self.__binary_profile.next_zero(time)
-
-            charging_duration = self.__next_time_zero - time
-            capacity_to_charge = (1 - system_state.soc) * system_state.capacity * self.__Wh_to_Ws
-            if charging_duration > 0:
-                power = capacity_to_charge / charging_duration
-            else:
-                power=0
-
-            if charging_duration == self.__timestep:
-                self.__next_time_zero = None
-
-
-        elif self.__charging_strategy[0:6] == 'Paused':
-            threshold = float(self.__charging_strategy[-3:])
-            if system_state.soc < threshold:
-                power = self.__max_ac_grid_power
+        # Only charge BESS to PeakShavingEnergy that is required during the next forecast cycle for reduced ageing.
+        # If forecasting horizon is chosen too short, the BESS may not be able to charge up before the peak.
+        self.__power = self.__load_profile.next(time) + power
+
+        peak_shaving_energy_delta = -1 * self.__peak_energy_forecaster.next(time, self.__power) * 1/3600
+
+        net_load = self.__power - self.__ps_limit
+        if net_load >= 0:
+            target_power = -1 * net_load
+        else:
+            if (system_state.soc - self.__soc_margin) * system_state.capacity < peak_shaving_energy_delta:
+                # adapt power for long simulation steps to prevent overshoot
+                # otherwise: target_power = -1 * net_load
+                missing_wh = peak_shaving_energy_delta - (system_state.soc - self.__soc_margin) * system_state.capacity
+                missing_wh *= 1 / self.__efficiency
+                target_power = missing_wh * 3600 / self.__delta_t
+                if target_power > -1 * net_load:
+                    target_power = -1 * net_load
+            elif self.__soc_margin > system_state.soc:
+                missing_wh = (self.__soc_margin - system_state.soc) * system_state.capacity
+                target_power = missing_wh * 3600 / self.__delta_t
+                if target_power > -1 * net_load:
+                    target_power = -1 * net_load
             else:
-                if self.__next_time_zero == None:
-                    self.__next_time_zero = self.__binary_profile.next_zero(time)
-                else:
-                    charging_duration = (1-system_state.soc)*system_state.capacity*self.__Wh_to_Ws/self.__max_ac_grid_power
-                    charging_restart_time = self.__next_time_zero - charging_duration - 1800
-                    # start recharging after the pause, buffer of 30 minutes (1800s)
-                    if time < charging_restart_time:
-                        power = 0
-                    else:
-                        power = self.__max_ac_grid_power
-                        if self.__next_time_zero - time < self.__timestep:
-                            self.__next_time_zero = None
+                target_power = 0
 
-
-        return power
+        return target_power
 
     def update(self, energy_management_state: EnergyManagementState) -> None:
         energy_management_state.load_power = self.__power
+        energy_management_state.peakshaving_limit = self.__ps_limit
 
     def clear(self) -> None:
         self.__power = 0.0
 
     def close(self) -> None:
-        self.__binary_profile.close()
-        self.__load_profile_driving.close()
+        pass
+
+
+class PeakEnergyForecaster:
+
+    def __init__(self, profile: PowerProfile, forecasting_steps: int, ps_limit: float, p_max: float,
+                 efficiency: float, general_config: GeneralSimulationConfig, profile_config: ProfileConfig):
+
+        # open second load profile for forecasts
+        # self.__load_profile: LoadProfile = LoadProfile(profile_config, general_config)
+        self.__load_profile: PowerProfile = profile
+
+        # needed for algorithm
+        self.__efficiency = efficiency
+        self.__delta_t = general_config.timestep
+        self.__forecasting_steps = forecasting_steps
+        self.__start_t = general_config.start
+        self.__nameplate_power = p_max
+        self.__ps_limit = ps_limit
+        power_values = list()
+        # for i in range(forecasting_steps):
+        for i in range(1, forecasting_steps+1):
+            power_values.append(self.__load_profile.next(self.__start_t+i*self.__delta_t))
+
+        # calculate initial energy surplus for every future peak within the load forecast timeframe in Ws
+        self.__energy_surpluses = [0]
+        self.__time_peak_end = []  # time at which the respective peak ends
+        self.__sign = np.sign(ps_limit - power_values[0])
+        for i in range(len(power_values)):
+            delta_p = self.limit(ps_limit - power_values[i], self.__nameplate_power)
+            if delta_p > 0:
+                delta_p *= self.__efficiency
+            if np.sign(delta_p) <= self.__sign:
+                self.__energy_surpluses[-1] += delta_p * self.__delta_t
+            else:
+                self.__energy_surpluses.append(self.__energy_surpluses[-1])
+                self.__time_peak_end.append(self.__start_t + (i+1) * self.__delta_t)
+                self.__energy_surpluses[-1] += delta_p * self.__delta_t
+            self.__sign = np.sign(delta_p)
+
+    @staticmethod
+    def limit(delta: float, max_abs: float) -> float:
+        if delta < - max_abs:
+            return -max_abs
+        elif delta > max_abs:
+            return max_abs
+        else:
+            return delta
+
+    def next(self, time, current_load) -> float:
+        # check if a peak has passed
+        if self.__time_peak_end:
+            if self.__time_peak_end[0] <= time:
+                self.__time_peak_end.pop(0)
+                self.__energy_surpluses.pop(0)
+
+        # subtract current peak energy from energy of future peaks
+        delta_p_now = self.limit(self.__ps_limit - current_load, self.__nameplate_power)
+        if delta_p_now > 0:
+            delta_p_now *= self.__efficiency
+        self.__energy_surpluses = [e - delta_p_now * self.__delta_t for e in self.__energy_surpluses]
+
+        # look for new peaks
+        delta_p_future = self.limit(
+            self.__ps_limit - self.__load_profile.next(time + self.__forecasting_steps * self.__delta_t),
+            self.__nameplate_power)
+        if delta_p_future > 0:
+            delta_p_future *= self.__efficiency
+        if np.sign(delta_p_future) <= self.__sign:
+            self.__energy_surpluses[-1] += delta_p_future * self.__delta_t
+        else:
+            self.__energy_surpluses.append(self.__energy_surpluses[-1])
+            self.__time_peak_end.append(time + self.__forecasting_steps * self.__delta_t)
+            self.__energy_surpluses[-1] += delta_p_future * self.__delta_t
+        self.__sign = np.sign(delta_p_future)
+        return min(self.__energy_surpluses)
```

### Comparing `simses-1.3.2/simses/logic/energy_management/strategy/basic/ev_charger_with_buffer.py` & `simses-1.3.3/simses/logic/energy_management/strategy/basic/ev_charger_with_buffer.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/logic/energy_management/strategy/basic/frequency_containment_reserve.py` & `simses-1.3.3/simses/logic/energy_management/strategy/basic/frequency_containment_reserve.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/logic/energy_management/strategy/basic/intraday_market_recharge.py` & `simses-1.3.3/simses/logic/energy_management/strategy/basic/intraday_market_recharge.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/logic/energy_management/strategy/basic/peak_shaving_perfect_foresight.py` & `simses-1.3.3/simses/logic/energy_management/strategy/basic/residential_pv_feed_in_damp.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,154 +1,111 @@
-import numpy as np
-
-from simses.commons.config.simulation.energy_management import EnergyManagementConfig
+import math
+from simses.commons.log import Logger
 from simses.commons.config.simulation.general import GeneralSimulationConfig
 from simses.commons.config.simulation.profile import ProfileConfig
-from simses.commons.config.simulation.system import StorageSystemConfig
-from simses.commons.profile.power.power_profile import PowerProfile
+from simses.commons.profile.power.generation import GenerationProfile
 from simses.commons.state.energy_management import EnergyManagementState
 from simses.commons.state.system import SystemState
 from simses.logic.energy_management.strategy.operation_priority import OperationPriority
 from simses.logic.energy_management.strategy.operation_strategy import OperationStrategy
 
 
-class PeakShavingPerfectForesight(OperationStrategy):
+class ResidentialPvFeedInDamp(OperationStrategy):
     """
-        Peak Shaving under the assumption of perfect foresight for the load profile in order to reduce calendar
-        degradation.
-        The BESS will only charge up to the energy that is needed for the next load peak, right before the load peak
-        occurs.
+    Operation Strategy for a residential home storage system in combination with PV generation.
+    The algorithm plans the charging of the lithium_ion according to a PV prediction. It tries to provide a fully charged
+    BESS at sundown.
     """
-    def __init__(self, general_config: GeneralSimulationConfig, power_profile: PowerProfile, forecast_profile: PowerProfile,
-                 energy_management_config: EnergyManagementConfig, system_config: StorageSystemConfig,
-                 profile_config: ProfileConfig):
-        super().__init__(OperationPriority.VERY_HIGH)
-
-        # configurable
-        self.__efficiency = 0.9
-        self.__soc_margin = 0.1  # to prevent missing peaks due to non-accurate efficiency
-        forecasting_time_hours = 72  # select forecast time for data horizon in the future that is considered
-        forecasting_steps = int(round(forecasting_time_hours*60*60 / general_config.timestep))
 
+    def __init__(self, power_profile, general_config: GeneralSimulationConfig, profile_config: ProfileConfig):
+        super().__init__(OperationPriority.MEDIUM)
+        self.__log: Logger = Logger(type(self).__name__)
+        self.__start = general_config.start
+        self.__end = general_config.end
+        self.__timestep = general_config.timestep
         self.__load_profile = power_profile
-        self.__delta_t = general_config.timestep
-        self.__ps_limit: float = energy_management_config.max_power
-        nameplate_power = 0
-        for system in system_config.storage_systems_ac:
-            nameplate_power += float(system[1])
-        self.__peak_energy_forecaster = PeakEnergyForecaster(forecast_profile, forecasting_steps, self.__ps_limit, nameplate_power,
-                                                             self.__efficiency, general_config, profile_config)
-        self.__power = 0
+        self.__pv_profile = GenerationProfile(profile_config, general_config)
+        self.__p_pv_peak = 1
+        self.__Wh_to_Ws = 3600
+        self.__s_per_day = 86400
+        self.__steps_per_day = int(self.__s_per_day / self.__timestep)
+        self.__pv_profile_copy_for_prediction = GenerationProfile(profile_config, general_config)
+        self.__last_pv_generation: list = self.pv_prediction(self.__pv_profile_copy_for_prediction)
+        self.__pv_power = 0
+        self.__load_power = 0
+
+        self.__eta = 0.95
 
     def next(self, time: float, system_state: SystemState, power: float = 0) -> float:
-        # Only charge BESS to PeakShavingEnergy that is required during the next forecast cycle for reduced ageing.
-        # If forecasting horizon is chosen too short, the BESS may not be able to charge up before the peak.
-        self.__power = self.__load_profile.next(time) + power
-
-        peak_shaving_energy_delta = -1 * self.__peak_energy_forecaster.next(time, self.__power) * 1/3600
-
-        net_load = self.__power - self.__ps_limit
-        if net_load >= 0:
-            target_power = -1 * net_load
-        else:
-            if (system_state.soc - self.__soc_margin) * system_state.capacity < peak_shaving_energy_delta:
-                # adapt power for long simulation steps to prevent overshoot
-                # otherwise: target_power = -1 * net_load
-                missing_wh = peak_shaving_energy_delta - (system_state.soc - self.__soc_margin) * system_state.capacity
-                missing_wh *= 1 / self.__efficiency
-                target_power = missing_wh * 3600 / self.__delta_t
-                if target_power > -1 * net_load:
-                    target_power = -1 * net_load
-            elif self.__soc_margin > system_state.soc:
-                missing_wh = (self.__soc_margin - system_state.soc) * system_state.capacity
-                target_power = missing_wh * 3600 / self.__delta_t
-                if target_power > -1 * net_load:
-                    target_power = -1 * net_load
+        self.__pv_power = self.__pv_profile.next(time)
+        self.__load_power = self.__load_profile.next(time)
+
+        residual_load = self.__pv_power - self.__load_power
+        if residual_load > 0 and self.__pv_power > 0:
+            day = math.floor(
+                (time - self.__start) / self.__s_per_day)
+            capacity_remaining = system_state.capacity * (1 - system_state.soc)
+
+            energy_remaining = capacity_remaining * self.__Wh_to_Ws
+            remaining_time = self.__last_pv_generation[
+                                   day] - time - 3600  # An hour before last pv production the storage should be filled
+            if remaining_time > 0:  # Preventing division by 0
+                power_ref = energy_remaining / (remaining_time * self.__eta)  # Ws
             else:
-                target_power = 0
+                power_ref = energy_remaining / (1 * self.__eta)  # Ws
+            battery_power = min(power_ref, residual_load)
+        else:
+            battery_power = residual_load
+        return battery_power
 
-        return target_power
+    def pv_prediction(self, pv_generation_profile) -> list:
+        """
+        Function to determine the last pv production of every day of the simulation
+        and storing the timestamps into a list.
+
+        Returns
+        -------
+        list:
+            timestamps of the last pv production of every day of the simulation.
+        """
+        self.__log.info('PV Prediction is performed this may take some time.')
+        pv_profile: list = pv_generation_profile.profile_data_to_list()
+        pv = pv_profile.copy()
+
+        timesteps = (self.__end - self.__start) / self.__timestep
+        days = int(timesteps / self.__steps_per_day) + 1
+
+        last_pv_generation = []
+        for day in range(days):
+            if day == days - 1:  # Last day special consideration (not full day)
+                beginning_of_day = day * self.__steps_per_day * self.__timestep
+                remaining_steps = int(
+                    (self.__end - self.__start - beginning_of_day) / self.__timestep)
+                for step in range(remaining_steps):
+                    current_step = day * self.__steps_per_day + remaining_steps - step
+                    if pv[current_step - 1] > 0:
+                        last_pv_generation.append(self.__start + current_step * self.__timestep)
+                        break
+                    if step == remaining_steps - 1:  # No Generation on this day
+                        last_pv_generation.append(None)
+            else:
+                for step in range(self.__steps_per_day):
+                    current_step = (day + 1) * self.__steps_per_day - step
+                    if pv[current_step] > 0:
+                        last_pv_generation.append(self.__start + current_step * self.__timestep)
+                        break
+                    if step == self.__steps_per_day - 1:  # No Generation on this day
+                        last_pv_generation.append(None)
+        self.__log.info('PV Prediction done.')
+        return last_pv_generation
 
     def update(self, energy_management_state: EnergyManagementState) -> None:
-        energy_management_state.load_power = self.__power
-        energy_management_state.peakshaving_limit = self.__ps_limit
+        energy_management_state.pv_power = self.__pv_power
+        energy_management_state.load_power = self.__load_power
 
     def clear(self) -> None:
-        self.__power = 0.0
+        self.__pv_power = 0.0
+        self.__load_power = 0.0
 
     def close(self) -> None:
-        pass
-
-
-class PeakEnergyForecaster:
-
-    def __init__(self, profile: PowerProfile, forecasting_steps: int, ps_limit: float, p_max: float,
-                 efficiency: float, general_config: GeneralSimulationConfig, profile_config: ProfileConfig):
-
-        # open second load profile for forecasts
-        # self.__load_profile: LoadProfile = LoadProfile(profile_config, general_config)
-        self.__load_profile: PowerProfile = profile
-
-        # needed for algorithm
-        self.__efficiency = efficiency
-        self.__delta_t = general_config.timestep
-        self.__forecasting_steps = forecasting_steps
-        self.__start_t = general_config.start
-        self.__nameplate_power = p_max
-        self.__ps_limit = ps_limit
-        power_values = list()
-        # for i in range(forecasting_steps):
-        for i in range(1, forecasting_steps+1):
-            power_values.append(self.__load_profile.next(self.__start_t+i*self.__delta_t))
-
-        # calculate initial energy surplus for every future peak within the load forecast timeframe in Ws
-        self.__energy_surpluses = [0]
-        self.__time_peak_end = []  # time at which the respective peak ends
-        self.__sign = np.sign(ps_limit - power_values[0])
-        for i in range(len(power_values)):
-            delta_p = self.limit(ps_limit - power_values[i], self.__nameplate_power)
-            if delta_p > 0:
-                delta_p *= self.__efficiency
-            if np.sign(delta_p) <= self.__sign:
-                self.__energy_surpluses[-1] += delta_p * self.__delta_t
-            else:
-                self.__energy_surpluses.append(self.__energy_surpluses[-1])
-                self.__time_peak_end.append(self.__start_t + (i+1) * self.__delta_t)
-                self.__energy_surpluses[-1] += delta_p * self.__delta_t
-            self.__sign = np.sign(delta_p)
-
-    @staticmethod
-    def limit(delta: float, max_abs: float) -> float:
-        if delta < - max_abs:
-            return -max_abs
-        elif delta > max_abs:
-            return max_abs
-        else:
-            return delta
-
-    def next(self, time, current_load) -> float:
-        # check if a peak has passed
-        if self.__time_peak_end:
-            if self.__time_peak_end[0] <= time:
-                self.__time_peak_end.pop(0)
-                self.__energy_surpluses.pop(0)
-
-        # subtract current peak energy from energy of future peaks
-        delta_p_now = self.limit(self.__ps_limit - current_load, self.__nameplate_power)
-        if delta_p_now > 0:
-            delta_p_now *= self.__efficiency
-        self.__energy_surpluses = [e - delta_p_now * self.__delta_t for e in self.__energy_surpluses]
-
-        # look for new peaks
-        delta_p_future = self.limit(
-            self.__ps_limit - self.__load_profile.next(time + self.__forecasting_steps * self.__delta_t),
-            self.__nameplate_power)
-        if delta_p_future > 0:
-            delta_p_future *= self.__efficiency
-        if np.sign(delta_p_future) <= self.__sign:
-            self.__energy_surpluses[-1] += delta_p_future * self.__delta_t
-        else:
-            self.__energy_surpluses.append(self.__energy_surpluses[-1])
-            self.__time_peak_end.append(time + self.__forecasting_steps * self.__delta_t)
-            self.__energy_surpluses[-1] += delta_p_future * self.__delta_t
-        self.__sign = np.sign(delta_p_future)
-        return min(self.__energy_surpluses)
+        self.__load_profile.close()
+        self.__pv_profile.close()
```

### Comparing `simses-1.3.2/simses/logic/energy_management/strategy/basic/peak_shaving_simple.py` & `simses-1.3.3/simses/logic/energy_management/strategy/basic/peak_shaving_simple.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/logic/energy_management/strategy/basic/power_follower.py` & `simses-1.3.3/simses/logic/energy_management/strategy/basic/power_follower.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,24 +5,25 @@
 from simses.logic.energy_management.strategy.operation_strategy import OperationStrategy
 
 
 class PowerFollower(OperationStrategy):
 
     """
     PowerFollower is a basic operation strategy which just forwards a given power profile to the storage system.
+    Here, SimSES interprets positive values as charging and negative as discharging of the storage.
     """
 
     def __init__(self, power_profile: PowerProfile):
         super().__init__(OperationPriority.MEDIUM)
         self.__power_profile: PowerProfile = power_profile
         self.__power: float = 0.0
 
     def next(self, time: float, system_state: SystemState, power: float = 0) -> float:
         self.__power = self.__power_profile.next(time)
-        return -1.0 * self.__power
+        return 1.0 * self.__power
 
     def update(self, energy_management_state: EnergyManagementState) -> None:
         energy_management_state.load_power = self.__power
 
     def clear(self) -> None:
         self.__power = 0.0
```

### Comparing `simses-1.3.2/simses/logic/energy_management/strategy/basic/residential_pv_feed_in_damp.py` & `simses-1.3.3/simses/simulation/system_tests/system_test.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,110 +1,118 @@
-import math
-from simses.commons.log import Logger
-from simses.commons.config.simulation.general import GeneralSimulationConfig
-from simses.commons.profile.power.generation import GenerationProfile
-from simses.commons.state.energy_management import EnergyManagementState
-from simses.commons.state.system import SystemState
-from simses.logic.energy_management.strategy.operation_priority import OperationPriority
-from simses.logic.energy_management.strategy.operation_strategy import OperationStrategy
+import os
+import shutil
+import time
+from configparser import ConfigParser
+from simses.commons.config.abstract_config import Config
+from simses.commons.config.generation.analysis import AnalysisConfigGenerator
+from simses.commons.config.simulation.simulation_config import SimulationConfig
+from simses.commons.utils.utilities import remove_file
+from simses.simulation.batch_processing import BatchProcessing
 
 
-class ResidentialPvFeedInDamp(OperationStrategy):
+class SystemTest(BatchProcessing):
+
     """
-    Operation Strategy for a residential home storage system in combination with PV generation.
-    The algorithm plans the charging of the lithium_ion according to a PV prediction. It tries to provide a fully charged
-    BESS at sundown.
+    TestBatchProcessing execute system tests for various system configurations.
     """
 
-    def __init__(self, power_profile, general_config: GeneralSimulationConfig, pv_generation_profile: GenerationProfile):
-        super().__init__(OperationPriority.MEDIUM)
-        self.__log: Logger = Logger(type(self).__name__)
-        self.__start = general_config.start
-        self.__end = general_config.end
-        self.__timestep = general_config.timestep
-        self.__load_profile = power_profile
-        self.__pv_profile = pv_generation_profile
-        self.__p_pv_peak = 1
-        self.__Wh_to_Ws = 3600
-        self.__s_per_day = 86400
-        self.__steps_per_day = int(self.__s_per_day / self.__timestep)
-        self.__last_pv_generation: list = self.pv_prediction(pv_generation_profile)
-        self.__pv_power = 0
-        self.__load_power = 0
-
-        self.__eta = 0.95
-
-    def next(self, time: float, system_state: SystemState, power: float = 0) -> float:
-        self.__pv_power = self.__pv_profile.next(time)
-        self.__load_power = self.__load_profile.next(time)
-
-        residual_load = self.__pv_power - self.__load_power
-        if residual_load > 0 and self.__pv_power > 0:
-            day = math.floor(
-                (time - self.__start) / self.__s_per_day)
-            capacity_remaining = system_state.capacity * (1 - system_state.soc)
-
-            energy_remaining = capacity_remaining * self.__Wh_to_Ws
-            remaining_time = self.__last_pv_generation[
-                                   day] - time - 3600  # An hour before last pv production the storage should be filled
-            if remaining_time > 0:  # Preventing division by 0
-                power_ref = energy_remaining / (remaining_time * self.__eta)  # Ws
-            else:
-                power_ref = energy_remaining / (1 * self.__eta)  # Ws
-            battery_power = min(power_ref, residual_load)
-        else:
-            battery_power = residual_load
-
-        return battery_power
-
-    def pv_prediction(self, pv_generation_profile: GenerationProfile) -> list:
-        """
-        Function do determine the last pv production of every day of the simulation
-        and storing the timestamps into a list.
-
-        Returns
-        -------
-        list:
-            timestamps of the last pv production of every day of the simulation.
-        """
-        self.__log.info('PV Prediction is performed this may take some time.')
-        pv_profile: list = pv_generation_profile.profile_data_to_list()
-        pv = pv_profile.copy()
-
-        timesteps = (self.__end - self.__start) / self.__timestep
-        days = int(timesteps / self.__steps_per_day) + 1
-
-        last_pv_generation = []
-        for day in range(days):
-            if day == days - 1:  # Last day special consideration (not full day)
-                beginning_of_day = day * self.__steps_per_day * self.__timestep
-                remaining_steps = int(
-                    (self.__end - self.__start - beginning_of_day) / self.__timestep)
-                for step in range(remaining_steps):
-                    current_step = day * self.__steps_per_day + remaining_steps - step
-                    if pv[current_step - 1] > 0:
-                        last_pv_generation.append(self.__start + current_step * self.__timestep)
-                        break
-                    if step == remaining_steps - 1:  # No Generation on this day
-                        last_pv_generation.append(None)
-            else:
-                for step in range(self.__steps_per_day):
-                    current_step = (day + 1) * self.__steps_per_day - step
-                    if pv[current_step] > 0:
-                        last_pv_generation.append(self.__start + current_step * self.__timestep)
-                        break
-                    if step == self.__steps_per_day - 1:  # No Generation on this day
-                        last_pv_generation.append(None)
-        self.__log.info('PV Prediction done.')
-        return last_pv_generation
-
-    def update(self, energy_management_state: EnergyManagementState) -> None:
-        energy_management_state.pv_power = self.__pv_power
-        energy_management_state.load_power = self.__load_power
-
-    def clear(self) -> None:
-        self.__pv_power = 0.0
-        self.__load_power = 0.0
-
-    def close(self) -> None:
-        self.__load_profile.close()
-        self.__pv_profile.close()
+    __TEST_NAME: str = 'test_'
+    __TEMP_FILE_ENDING: str = '.test.tmp'
+    __CONFIG_EXT: str = Config.CONFIG_EXT
+    __LOCAL_CONFIG_EXT: str = Config.LOCAL
+    __CONFIG_PATH: str = SimulationConfig.CONFIG_PATH
+    __SIMULATION_CONFIG: str = SimulationConfig.CONFIG_NAME
+    __DATA_DIR: str = os.path.join(os.path.dirname(__file__), 'configs')
+
+    __SELECTED_TESTS: [str] = list()
+    """List with names of selected tests to run. If list is empty, all tests will be executed."""
+    # __SELECTED_TESTS.append('test_16')
+    # __SELECTED_TESTS.append('test_14')
+
+    def __init__(self):
+        super().__init__(do_simulation=True, do_analysis=True)
+        # self.__id_generator = self.__get_id_generator()
+        self.__tests: [str] = list()
+
+    def _setup_config(self) -> dict:
+        # test set for config setup
+        self.__rename_local_config()
+        configs: dict = dict()
+        if not self.__SELECTED_TESTS:
+            self.__add('test_0', ConfigParser(), configs)
+        for file in os.listdir(self.__DATA_DIR):
+            if file.endswith(self.__CONFIG_EXT):
+                config: ConfigParser = ConfigParser()
+                config.read(os.path.join(self.__DATA_DIR, file))
+                test_id: str = file.split('.')[-2]
+                if self.__SELECTED_TESTS:
+                    if test_id not in self.__SELECTED_TESTS:
+                        continue
+                self.__add(test_id, config, configs)
+        return configs
+
+    def _analysis_config(self) -> ConfigParser:
+        config_generator: AnalysisConfigGenerator = AnalysisConfigGenerator()
+        config_generator.print_results(False)
+        config_generator.do_plotting(False)
+        config_generator.merge_analysis(False)
+        return config_generator.get_config()
+
+    def __add(self, test_id: str, config: ConfigParser, configs: dict) -> None:
+        # if test_id is None:
+        #     test_id: str = next(self.__id_generator)
+        self.__tests.append(test_id)
+        configs[test_id] = config
+
+    def __get_id_generator(self) -> str:
+        test_id: int = 1
+        while True:
+            yield self.__TEST_NAME + str(test_id)
+            test_id += 1
+
+    def __rename_local_config(self):
+        self.__rename_local_simulation_config(self.__LOCAL_CONFIG_EXT, self.__TEMP_FILE_ENDING)
+
+    def __reverse_local_config(self):
+        self.__rename_local_simulation_config(self.__TEMP_FILE_ENDING, self.__LOCAL_CONFIG_EXT)
+
+    def __rename_local_simulation_config(self, src_ext: str, dest_ext: str) -> None:
+        # 1) Only the simulation.local.ini needs to be renamed.
+        # 2) It is safer to copy a file instead of moving or renaming it.
+        # 3) Only one place for logic.
+        file: str = os.path.join(self.__CONFIG_PATH, self.__SIMULATION_CONFIG + src_ext)
+        new_file: str = file.replace(src_ext, dest_ext)
+        if os.path.exists(file):
+            shutil.copy(file, new_file)
+            remove_file(file)
+        # for file in os.listdir(self.__CONFIG_PATH):
+        #     if file.endswith(self.__LOCAL_CONFIG_EXT):
+        #         new_file = file.replace(self.__LOCAL_CONFIG_EXT, self.__TEMP_FILE_ENDING)
+        #         os.rename(os.path.join(self.__CONFIG_PATH, file), os.path.join(self.__CONFIG_PATH, new_file))
+
+    # def __rename_local_configs_reverse(self) -> None:
+    #     for file in os.listdir(self.__CONFIG_PATH):
+    #         if file.endswith(self.__TEMP_FILE_ENDING):
+    #             new_file = file.replace(self.__TEMP_FILE_ENDING, self.__LOCAL_CONFIG_EXT)
+    #             os.rename(os.path.join(self.__CONFIG_PATH, file), os.path.join(self.__CONFIG_PATH, new_file))
+
+    def clean_up(self) -> None:
+        self.__reverse_local_config()
+        for test in self.__tests:
+            while True:
+                try:
+                    shutil.rmtree(os.path.join(self.get_results_path(), test))
+                    break
+                except FileNotFoundError:
+                    break
+                except PermissionError:
+                    print('Waiting for simulation to finish...')
+                    time.sleep(1)
+
+
+if __name__ == "__main__":
+    batch_processing: BatchProcessing = SystemTest()
+    try:
+        batch_processing.run()
+    finally:
+        batch_processing.clean_up()
+        print('System tests Finished')
```

### Comparing `simses-1.3.2/simses/logic/energy_management/strategy/basic/residential_pv_greedy.py` & `simses-1.3.3/simses/logic/energy_management/strategy/basic/residential_pv_greedy.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/logic/energy_management/strategy/basic/soc_follower.py` & `simses-1.3.3/simses/logic/energy_management/strategy/basic/soc_follower.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/logic/energy_management/strategy/basic/use_all_renewable_energy.py` & `simses-1.3.3/simses/logic/energy_management/strategy/basic/use_all_renewable_energy.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/logic/energy_management/strategy/operation_strategy.py` & `simses-1.3.3/simses/logic/energy_management/strategy/operation_strategy.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/logic/energy_management/strategy/stacked/dynamic_multi_use.py` & `simses-1.3.3/simses/logic/energy_management/strategy/stacked/parallel_multi_use_with_stealing.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from simses.logic.energy_management.strategy.basic.soc_follower import SocFollower
 from simses.logic.energy_management.strategy.basic.intraday_market_recharge import IntradayMarketRecharge
 from simses.logic.energy_management.strategy.basic.residential_pv_greedy import ResidentialPvGreedy
 from simses.logic.energy_management.strategy.basic.residential_pv_feed_in_damp import ResidentialPvFeedInDamp
 import numpy as np
 
 
-class DynamicMultiUse(StackedOperationStrategy):
+class ParallelMultiUseWithStealing(StackedOperationStrategy):
     # 0. Section: Initialize variables and strategies
     def __init__(self, general_config: GeneralSimulationConfig, profile_config: ProfileConfig,
                  ems_config: EnergyManagementConfig, power_profile: PowerProfile, battery_config: BatteryConfig,
                  pv_generation_profile: GenerationProfile, system_config: StorageSystemConfig):
 
         self.__log: Logger = Logger(type(self).__name__)
         self.__strategies_names: [] = ems_config.multi_use_strategies
@@ -147,16 +147,16 @@
         self.__borrowed_capacity = np.zeros(len(self.__strategies)).tolist()
 
         self.__indices_btm = [i for i, x in enumerate(self.__btm_ftm) if x == 0]  # Get indices of BTM strategy
         self.__indices_ftm = [i for i, x in enumerate(self.__btm_ftm) if x == 1]  # Get indices of FTM strategy
 
     def next(self, time: float, system_state: SystemState, power: float = 0) -> float:
         self.__counter = self.__counter + 1
-        if self.__counter == 859:
-            print('Halt')
+        # if self.__counter == 859:
+            # print('Halt')
 
         self.__total_power = 0
         self.__power_requested = []
 
         # 1. Section: Calculate Sub-System-SOC
         if system_state.ac_power != 0:
             self.__a = system_state.ac_power_delivered / system_state.ac_power  # Ratio A: Delivered power divided by requested power
@@ -232,63 +232,77 @@
 
         # Correct total_power:
         self.__total_power = sum(power_allocated)
         # Save system state SOC and capacity for the next time step:
         self.__previous_system_state_soc = system_state.soc
         self.__previous_system_state_capacity = system_state.capacity
 
-        # Save subsystem_SOC here to CSV:
-        soc1 = self.__sub_system_states[0].soc
-        soc2 = self.__sub_system_states[1].soc
-        soc3 = self.__sub_system_states[2].soc
-        cap1 = self.__sub_system_states[0].capacity
-        cap2 = self.__sub_system_states[1].capacity
-        cap3 = self.__sub_system_states[2].capacity
-        power_requested_copy1 = power_requested[0]
-        power_requested_copy2 = power_requested[1]
-        power_requested_copy3 = power_requested[2]
-        power_allocated_copy1 = power_allocated[0]
-        power_allocated_copy2 = power_allocated[1]
-        power_allocated_copy3 = power_allocated[2]
-
+        # # Save subsystem_SOC here to CSV:
+        # soc1 = self.__sub_system_states[0].soc
+        # soc2 = self.__sub_system_states[1].soc
+        # #soc3 = self.__sub_system_states[2].soc
+        # cap1 = self.__sub_system_states[0].capacity
+        # cap2 = self.__sub_system_states[1].capacity
+        # #cap3 = self.__sub_system_states[2].capacity
+        # power_requested_copy1 = power_requested[0]
+        # power_requested_copy2 = power_requested[1]
+        # #power_requested_copy3 = power_requested[2]
+        # power_allocated_copy1 = power_allocated[0]
+        # power_allocated_copy2 = power_allocated[1]
+        # #power_allocated_copy3 = power_allocated[2]
+        #
         # df = pd.DataFrame([soc1, soc2, cap1, cap2,
         #                    power_requested_copy1, power_requested_copy2,
         #                    power_allocated_copy1, power_allocated_copy2]).transpose()
-
-        df = pd.DataFrame([soc1, soc2, soc3, cap1, cap2, cap3,
-                           power_requested_copy1, power_requested_copy2, power_requested_copy3,
-                           power_allocated_copy1, power_allocated_copy2, power_allocated_copy3]).transpose()
-        temp_name = 'multi_use_sub_soc.csv'
-
-        try:
-           f = open(temp_name)
-           df.to_csv(temp_name, mode='a', index=False, header=False)
-
-           f.close()
-        except IOError:
-           df.to_csv(temp_name, header=False)  # Create CSV
+        #
+        # # df = pd.DataFrame([soc1, soc2, soc3, cap1, cap2, cap3,
+        # #                    power_requested_copy1, power_requested_copy2, power_requested_copy3,
+        # #                    power_allocated_copy1, power_allocated_copy2, power_allocated_copy3]).transpose()
+        # temp_name = 'multi_use_sub_soc.csv'
+        #
+        # try:
+        #    f = open(temp_name)
+        #    df.to_csv(temp_name, mode='a', index=False, header=False)
+        #
+        #    f.close()
+        # except IOError:
+        #    df.to_csv(temp_name, header=False)  # Create CSV
 
         return self.__total_power
 
     def correct_subsystem_soc(self, sub_system_states, subsystem_counter, btm_ftm, indices_btm, indices_ftm, system_state):
         # Correction of Sub-System-State-SoF if System-State-SoC is 1 or 0
         if system_state.soc == 1:  # Set all subsystem-socs to one to prevent increasing deviation over time
             sub_system_states[subsystem_counter].soc = 1
         elif system_state.soc == 0:  # Set all subsystem-socs to zero to prevent increasing deviation over tim
             sub_system_states[subsystem_counter].soc = 0
 
         # Check if it possible for all BTM or FTM applications to borrow energy
         soc_sum_btm = sum(sub_system_states[j].soc for j in indices_btm)
         soc_sum_ftm = sum(sub_system_states[j].soc for j in indices_ftm)
-        if soc_sum_btm > len(indices_btm) or soc_sum_btm < 0 or soc_sum_ftm > len(indices_ftm) or soc_sum_ftm < 0:
+        if soc_sum_btm < 0:
             print('Warning! Sub-System-SoC is bigger/smaller then 1/0! Sub-System-SoC;', sub_system_states[subsystem_counter].soc)
-            if sub_system_states[subsystem_counter].soc > 1:
-                sub_system_states[subsystem_counter].soc = 1
-            elif sub_system_states[subsystem_counter].soc < 0:
-                sub_system_states[subsystem_counter].soc = 0
+            for btm_systems in indices_btm:
+                sub_system_states[btm_systems].soc = 0
+
+        elif soc_sum_btm > len(indices_btm):
+            print('Warning! Sub-System-SoC is bigger/smaller then 1/0! Sub-System-SoC;', sub_system_states[subsystem_counter].soc)
+            for btm_systems in indices_btm:
+                sub_system_states[btm_systems].soc = 1
+
+        elif soc_sum_ftm < 0:
+            print('Warning! Sub-System-SoC is bigger/smaller then 1/0! Sub-System-SoC;', sub_system_states[subsystem_counter].soc)
+            for ftm_systems in indices_ftm:
+                sub_system_states[ftm_systems].soc = 0
+
+        elif soc_sum_ftm > len(indices_ftm):
+            print('Warning! Sub-System-SoC is bigger/smaller then 1/0! Sub-System-SoC;', sub_system_states[subsystem_counter].soc)
+            for ftm_systems in indices_ftm:
+                sub_system_states[ftm_systems].soc = 1
+
         # If it is possible
         else:
             if sub_system_states[subsystem_counter].soc < 0:
                 temp_delta = sub_system_states[subsystem_counter].soc * sub_system_states[subsystem_counter].capacity
                 sub_system_states[subsystem_counter].soc = 0  # Set SOC to 0
 
                 if btm_ftm[subsystem_counter] == 0:  # BTM
@@ -527,21 +541,14 @@
                             surplus_of_capacity = surplus_of_capacity - ftm_free_space_capacity_current
 
                     # After loop
                     if surplus_of_capacity > 0:
                         real_capacity_change = np.round(desired_capacity_change - surplus_of_capacity, 6)
                         power_requested[subsystem_counter] = real_capacity_change / self.__ts * 3600
 
-
-        # for i in range(len(power_requested)):
-        #     if power_requested[i] < 0:
-        #         power_requested[i] = power_requested[i] * 0.95
-        #     elif power_requested[i] > 0:
-        #         power_requested[i] = power_requested[i] * 1.05
-
         return power_requested, borrowed_capacity
 
     def calculate_power_considering_ranking(self, power_requested_list, max_power_allocated, btm_ftm):
         power_left = max_power_allocated  # charge and discharge power together
 
         indices_btm = [i for i, x in enumerate(btm_ftm) if x == 0]
         btm_power_requested = [power_requested_list[i] for i in indices_btm]
```

### Comparing `simses-1.3.2/simses/logic/energy_management/strategy/stacked/fcr_idm_recharge_stacked.py` & `simses-1.3.3/simses/logic/energy_management/strategy/stacked/fcr_idm_recharge_stacked.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/logic/energy_management/strategy/stacked/stacked_operation_strategy.py` & `simses-1.3.3/simses/logic/energy_management/strategy/stacked/stacked_operation_strategy.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/logic/power_distribution/efficient.py` & `simses-1.3.3/simses/logic/power_distribution/efficient.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/logic/power_distribution/equal.py` & `simses-1.3.3/simses/logic/power_distribution/equal.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/logic/power_distribution/power_distributor.py` & `simses-1.3.3/simses/logic/power_distribution/power_distributor.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/logic/power_distribution/soc.py` & `simses-1.3.3/simses/logic/power_distribution/soc.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/logic/power_distribution/state.py` & `simses-1.3.3/simses/logic/power_distribution/state.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/logic/power_distribution/technology.py` & `simses-1.3.3/simses/logic/power_distribution/technology.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/logic/test/test_electric_vehicle_SOC_meanpower.py` & `simses-1.3.3/simses/logic/test/test_electric_vehicle_SOC_meanpower.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/logic/test/test_electric_vehicle_SOC_original.py` & `simses-1.3.3/simses/logic/test/test_electric_vehicle_SOC_original.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/logic/test/test_electric_vehicle_SOC_paused.py` & `simses-1.3.3/simses/logic/test/test_electric_vehicle_SOC_paused.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/logic/test/test_electric_vehicle_SOC_uncontrolled.py` & `simses-1.3.3/simses/logic/test/test_electric_vehicle_SOC_uncontrolled.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/logic/test/test_electric_vehicle_all_strategies.py` & `simses-1.3.3/simses/logic/test/test_electric_vehicle_all_strategies.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/logic/test/test_electric_vehicle_uncontrolled.py` & `simses-1.3.3/simses/logic/test/test_electric_vehicle_uncontrolled.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/logic/test/test_equal_power_distributor.py` & `simses-1.3.3/simses/logic/test/test_equal_power_distributor.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/logic/test/test_multi_use.py` & `simses-1.3.3/simses/logic/test/test_multi_use.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 from simses.commons.config.simulation.battery import BatteryConfig
 from simses.commons.config.simulation.profile import ProfileConfig
 from simses.commons.config.simulation.general import GeneralSimulationConfig
 from simses.commons.config.simulation.system import StorageSystemConfig
 from simses.commons.profile.power.file import FilePowerProfile
 from simses.commons.state.system import SystemState
 from simses.commons.utils.utilities import remove_file
-from simses.logic.energy_management.strategy.stacked.dynamic_multi_use import DynamicMultiUse
+from simses.logic.energy_management.strategy.stacked.parallel_multi_use_with_stealing import ParallelMultiUseWithStealing
 from simses.commons.config.simulation.simulation_config import SimulationConfig, create_dict_from, create_list_from, \
     clean_split
 
-
+# Important: Creation of the CSV file in the ParallelMultiUseWithStealing class must be commented out!
 
 DELIMITER: str = ','
 HEADER: str = '# Unit: W'
 system_state: SystemState = SystemState(0,0)
 START: int = 0
 END: int = 5
 TIME_STEP: int = 3600
@@ -29,86 +29,79 @@
 MAX_POWER: int = 3
 START_SOC: float = 0.5
 MULTI_USE_STRATEGIES: str = 'ResidentialPvGreedy, SimplePeakShaving'
 ENERGY_ALLOCATION: str = '0.5, 0.5'
 POWER_ALLOCATION: str = '0.5, 0.5'
 RANKING: str = '2, 1'
 STORAGE_SYSTEM_AC: str = 'system_1, 10, 600,fix,no_housing,no_hvac'  # Installed power
-#STORAGE_TECHNOLOGIES: str = 'storage_1, 10, lithium_ion, SonyLFP'  # Installed capacity
-# TEST: list = []
-# TEST.append(str(10))
-# TEST.append('lithium_ion')
-# TEST.append('SonyLFP')
 STORAGE_TECHNOLOGIES: dict = create_dict_from(['storage_1,10,lithium_ion,SonyLFP'])
 
-#STORAGE_TECHNOLOGIES = {}
-#STORAGE_TECHNOLOGIES['storage_1'] = ['10', 'lithium_ion', 'SonyLFP']
-
 FILE_NAME_LOAD: str = os.path.join(os.path.dirname(__file__), 'mockup_power_load_profile.csv')
 FILE_NAME_PV: str = os.path.join(os.path.dirname(__file__), 'mockup_power_pv_profile.csv')
 
+
 def create_general_config():
     conf: ConfigParser = ConfigParser()
     conf.add_section('GENERAL')
     date = datetime.fromtimestamp(START, timezone.utc)
     conf.set('GENERAL', 'START', date.strftime("%Y-%m-%d %H:%M:%S"))
     date = datetime.fromtimestamp(END, timezone.utc)
     conf.set('GENERAL', 'END', date.strftime("%Y-%m-%d %H:%M:%S"))
     conf.set('GENERAL', 'TIME_STEP', str(TIME_STEP))
     return GeneralSimulationConfig(config=conf)
 
+
 def create_ems_config():
     conf: ConfigParser = ConfigParser()
     conf.add_section('ENERGY_MANAGEMENT')
     conf.set('ENERGY_MANAGEMENT', 'STRATEGY', 'DynamicMultiUse')
     conf.set('ENERGY_MANAGEMENT', 'MULTI_USE_STRATEGIES', MULTI_USE_STRATEGIES)
     conf.set('ENERGY_MANAGEMENT', 'ENERGY_ALLOCATION', ENERGY_ALLOCATION)
     conf.set('ENERGY_MANAGEMENT', 'POWER_ALLOCATION', POWER_ALLOCATION)
     conf.set('ENERGY_MANAGEMENT', 'RANKING', RANKING)
     conf.set('ENERGY_MANAGEMENT', 'MAX_POWER', str(MAX_POWER))
     return EnergyManagementConfig(config=conf)
 
+
 def create_battery_config():
     conf: ConfigParser = ConfigParser()
     conf.add_section('BATTERY')
     conf.set('BATTERY', 'START_SOC', str(START_SOC))
     return BatteryConfig(config=conf)
 
+
 def create_profile_config():
     conf: ConfigParser = ConfigParser()
     conf.add_section('PROFILE')
     return ProfileConfig(config=conf)
 
+
 def create_storage_system_config():
     conf: ConfigParser = ConfigParser()
     conf.add_section('STORAGE_SYSTEM')
     conf.set('STORAGE_SYSTEM', 'STORAGE_SYSTEM_AC', STORAGE_SYSTEM_AC)
-    #conf.set('STORAGE_SYSTEM', 'STORAGE_TECHNOLOGIES', STORAGE_TECHNOLOGIES)
-    #conf.set('STORAGE_SYSTEM', 'STORAGE_TECHNOLOGIES', STORAGE_TECHNOLOGIES)
-    #conf.read_dict(STORAGE_TECHNOLOGIES)
-    # conf['STORAGE_SYSTEM'] = {
-    #     'STORAGE_SYSTEM_AC': 'system_1, 1000'
-    # }
 
     return StorageSystemConfig(config=conf)
 
+
 def create_load_file():
     with open(FILE_NAME_LOAD, mode='w') as file:
         file.write(HEADER + '\n')
         value = START
         tstmp = START
         while tstmp <= END:
             file.write(str(tstmp) + DELIMITER + str(value) + '\n')
             tstmp += STEP
             value += 1
 
     power_load_profile = FilePowerProfile(config=create_general_config(), filename=FILE_NAME_LOAD,
                                           delimiter=DELIMITER, scaling_factor=1)
     return power_load_profile
 
+
 def create_pv_file():
     with open(FILE_NAME_PV, mode='w') as file:
         file.write(HEADER + '\n')
         value = END
         tstmp = START
         while tstmp <= END:
             file.write(str(tstmp) + DELIMITER + str(value) + '\n')
@@ -118,125 +111,102 @@
     power_pv_profile = FilePowerProfile(config=create_general_config(), filename=FILE_NAME_PV,
                                           delimiter=DELIMITER, scaling_factor=1)
     return power_pv_profile
 
 
 @pytest.fixture(scope='module')
 def uut():
-   # print(STORAGE_TECHNOLOGIES)
-    #print(create_dict_from(['storage_1,10,lithium_ion,SonyLFP']))
-    system_config = create_storage_system_config()
-    #print(float(system_config.storage_technologies['storage_1'][system_config.STORAGE_CAPACITY]))
-    #print(float(system_config.storage_systems_ac[0][system_config.AC_SYSTEM_POWER]))
-    ems_config = create_ems_config()
-    uut = DynamicMultiUse(general_config = create_general_config(),
-                           profile_config = create_profile_config(),
-                           ems_config = ems_config,
-                           power_profile = create_load_file(),
-                           battery_config = create_battery_config(),
-                           pv_generation_profile = create_pv_file(),
-                           system_config = system_config)
+    uut = ParallelMultiUseWithStealing(general_config = create_general_config(),
+                                       profile_config = create_profile_config(),
+                                       ems_config =  create_ems_config(),
+                                       power_profile = create_load_file(),
+                                       battery_config = create_battery_config(),
+                                       pv_generation_profile = create_pv_file(),
+                                       system_config = create_storage_system_config())
     yield uut
     uut.close()
-    #remove_file(FILE_NAME_LOAD)
-    #remove_file(FILE_NAME_PV)
-#
-# @pytest.mark.parametrize('soc, capacity, subsystem_counter, btm_ftm, indices_btm, indices_ftm, result',
-#                          [
-#                           # ([0.5, 0.5], [10, 10], 0, [0, 0], [0, 1],  [], [0.5, 0.5]),
-#                           # ([0.5, 0.5], [10, 10], 1, [0, 0], [0, 1], [], [0.5, 0.5]),
-#                           # ([0.34, 0.23], [10, 10], 0, [0, 0], [0, 1], [], [0.34, 0.23]),
-#                           # ([0.34, 0.23], [10, 10], 1, [0, 0], [0, 1], [], [0.34, 0.23]),
-#                           # ([0.5, 0.5], [10, 10], 0, [1, 1], [],  [0, 1], [0.5, 0.5]),
-#                           # ([0.5, 0.5], [10, 10], 1, [1, 1], [], [0, 1], [0.5, 0.5]),
-#                           # ([0.34, 0.23], [10, 10], 0, [1, 1], [], [0, 1], [0.34, 0.23]),
-#                           # ([0.34, 0.23], [10, 10], 1, [1, 1], [], [0, 1], [0.34, 0.23]),
-#                           #
-#                           # ([-0.1, 0.5], [10, 10], 0, [0, 0], [0, 1], [], [0, 0.4]),
-#                           # ([1.1, 0.5], [10, 10], 0, [0, 0], [0, 1], [], [1, 0.6]),
-#                           # ([-0.1, 1.2], [10, 10], 0, [0, 0], [0, 1], [], [0, 1.1]),
-#                           #
-#                           # ([-0.1, 0.5], [10, 10], 0, [1, 1], [], [0, 1], [0, 0.4]),
-#                           # ([1.1, 0.5], [10, 10], 0, [1, 1], [], [0, 1], [1, 0.6]),
-#                           #
-#                           # ([0.5, 1.1], [10, 10], 0, [0, 0], [0, 1], [], [0.5, 1.1]),
-#                           # ([0.5, 1.1], [10, 10], 1, [0, 0], [0, 1], [], [0.6, 1]),
-#                           # ([0.5, -0.1], [10, 10], 0, [0, 0], [0, 1], [], [0.5, -0.1]),
-#                           # ([0.5, -0.1], [10, 10], 1, [0, 0], [0, 1], [], [0.4, 0]),
-#                           # ([0.5, 1.1], [10, 10], 0, [1, 1], [], [0, 1], [0.5, 1.1]),
-#                           # ([0.5, 1.1], [10, 10], 1, [1, 1], [], [0, 1], [0.6, 1]),
-#                           # ([0.5, -0.1], [10, 10], 0, [1, 1], [], [0, 1], [0.5, -0.1]),
-#                           # ([0.5, -0.1], [10, 10], 1, [1, 1], [], [0, 1], [0.4, 0]),
-#                           #
-#                           # ([0, 1.1], [10, 10], 1, [0, 0], [0, 1], [], [0.1, 1]),
-#                           # ([-0.1, -0.1, 0.5], [10, 10, 10], 0, [0, 0, 0], [0, 1, 2], [], [0, 0, 0]),
-#                           #
-#                           # ([1.2, 0.2, 0.5], [10, 10, 10], 0, [0, 1, 0], [0, 2], [1], [1, 0.2, 0.7]),
-#                           # ([1.2, 0.2, 0.5], [10, 10, 10], 0, [0, 1, 0], [0, 2], [1], [1, 0.2, 0.7]),
-#                           # ([1.2, 0.2, 0.5], [10, 10, 10], 0, [1, 1, 0], [0, 2], [1], [1, 0.4, 0.5]),
-#                           #
-#                           # ([0.2, 0.2, 1.1], [10, 10, 10], 2, [0, 1, 0], [0, 2], [1], [0.3, 0.2, 1]),
-#                           # ([0.2, 0.2, 1.1], [10, 10, 10], 2, [1, 0, 1], [1], [0, 2], [0.3, 0.2, 1])
-#
-#                          ]
-#                          )
-#
-# def test_correct_subsystem_soc(soc, capacity, subsystem_counter, btm_ftm, indices_btm, indices_ftm, result, uut):
-#     sub_system_states = []
-#     for i in range(len(soc)):
-#         sub_system_states.append(SystemState(0, 0))
-#         sub_system_states[i].soc = soc[i]
-#         sub_system_states[i].capacity = capacity[i]
-#     result_sub_system_states = uut.correct_subsystem_soc(sub_system_states, subsystem_counter, btm_ftm, indices_btm, indices_ftm)
-#
-#     result_soc = []
-#     for j in range(len(soc)):
-#         #result_soc.append(result_sub_system_states[j].soc,6)  #TODO: Runden?
-#         result_soc.append(np.round(result_sub_system_states[j].soc, 6))
-#
-#     assert result_soc == result
-
-# @pytest.mark.parametrize('soc, capacity, subsystem_counter, btm_ftm, indices_btm, indices_ftm',
-#                          [
-#                           ([-0.1, -0.1], [10, 10], 0, [0, 0], [0, 1], []),
-#                           ([1.1, 1.1], [10, 10], 0, [0, 0], [0, 1], []),
-#                           ([-0.1, -0.1], [10, 10], 1, [0, 0], [0, 1], []),
-#                           ([1.1, 1.1], [10, 10], 1, [0, 0], [0, 1], []),
-#                           ([-0.1, -0.1], [10, 10], 0, [1, 1], [], [0, 1]),
-#                           ([1.1, 1.1], [10, 10], 0, [1, 1], [], [0, 1]),
-#                           ([-0.1, -0.1], [10, 10], 1, [1, 1], [], [0, 1]),
-#                           ([1.1, 1.1], [10, 10], 1, [1, 1], [], [0, 1]),
-#                          ]
-#                          )
-#
-# def test_correct_subsystem_soc_error(soc, capacity, subsystem_counter, btm_ftm, indices_btm, indices_ftm, uut):
-#     sub_system_states = []
-#     for i in range(len(soc)):
-#         sub_system_states.append(SystemState(0, 0))
-#         sub_system_states[i].soc = soc[i]
-#         sub_system_states[i].capacity = capacity[i]
-#
-#     with pytest.raises(ValueError):
-#         uut.correct_subsystem_soc(sub_system_states, subsystem_counter, btm_ftm, indices_btm, indices_ftm)
+    remove_file(FILE_NAME_LOAD)
+    remove_file(FILE_NAME_PV)
+
+@pytest.mark.parametrize('soc, capacity, subsystem_counter, btm_ftm, indices_btm, indices_ftm, system_state_soc, result',
+                         [
+                          ([0.5, 0.5], [10, 10], 0, [0, 0], [0, 1],  [], [0.5], [0.5, 0.5]),
+                          ([0.5, 0.5], [10, 10], 1, [0, 0], [0, 1], [], [0.5], [0.5, 0.5]),
+                          ([0.34, 0.23], [10, 10], 0, [0, 0], [0, 1], [], [0.285], [0.34, 0.23]),
+                          ([0.34, 0.23], [10, 10], 1, [0, 0], [0, 1], [], [0.285], [0.34, 0.23]),
+                          ([0.5, 0.5], [10, 10], 0, [1, 1], [],  [0, 1], [0.5], [0.5, 0.5]),
+                          ([0.5, 0.5], [10, 10], 1, [1, 1], [], [0, 1], [0.5], [0.5, 0.5]),
+                          ([0.34, 0.23], [10, 10], 0, [1, 1], [], [0, 1], [0.285], [0.34, 0.23]),
+                          ([0.34, 0.23], [10, 10], 1, [1, 1], [], [0, 1], [0.285], [0.34, 0.23]),
+
+                          ([-0.1, 0.5], [10, 10], 0, [0, 0], [0, 1], [], [0.4], [0, 0.4]),
+                          ([1.1, 0.5], [10, 10], 0, [0, 0], [0, 1], [], [0.6], [1, 0.6]),
+                          #([-0.1, 1.2], [10, 10], 0, [0, 0], [0, 1], [], [0.4], [0, 1.1]),
+
+                          ([-0.1, 0.5], [10, 10], 0, [1, 1], [], [0, 1], [0.4], [0, 0.4]),
+                          ([1.1, 0.5], [10, 10], 0, [1, 1], [], [0, 1], [0.6], [1, 0.6]),
+
+                          ([0.5, 1.1], [10, 10], 0, [0, 0], [0, 1], [], [0.6], [0.5, 1.1]),
+                          ([0.5, 1.1], [10, 10], 1, [0, 0], [0, 1], [], [0.6], [0.6, 1]),
+                          ([0.5, -0.1], [10, 10], 0, [0, 0], [0, 1], [], [0.4], [0.5, -0.1]),
+                          ([0.5, -0.1], [10, 10], 1, [0, 0], [0, 1], [], [0.4], [0.4, 0]),
+                          ([0.5, 1.1], [10, 10], 0, [1, 1], [], [0, 1], [0.6], [0.5, 1.1]),
+                          ([0.5, 1.1], [10, 10], 1, [1, 1], [], [0, 1], [0.6], [0.6, 1]),
+                          ([0.5, -0.1], [10, 10], 0, [1, 1], [], [0, 1], [0.4], [0.5, -0.1]),
+                          ([0.5, -0.1], [10, 10], 1, [1, 1], [], [0, 1], [0.4], [0.4, 0]),
+
+                          ([0, 1.1], [10, 10], 1, [0, 0], [0, 1], [], [0.55], [0.1, 1]),
+                          ([-0.1, -0.1, 0.5], [10, 10, 10], 0, [0, 0, 0], [0, 1, 2], [], [0.3], [0, -0.1, 0.4]),
+                          ([0, -0.1, 0.4], [10, 10, 10], 1, [0, 0, 0], [0, 1, 2], [], [0.3], [0, 0, 0.3]),
+
+                          ([1.2, 0.2, 0.5], [10, 10, 10], 0, [0, 1, 0], [0, 2], [1], [0.6], [1, 0.2, 0.7]),
+                          ([1.2, 0.2, 0.5], [10, 10, 10], 0, [0, 1, 0], [0, 2], [1], [0.6], [1, 0.2, 0.7]),
+                          ([1.2, 0.2, 0.5], [10, 10, 10], 0, [1, 1, 0], [0, 2], [1], [0.6], [1, 0.4, 0.5]),
+
+                          ([0.2, 0.2, 1.1], [10, 10, 10], 2, [0, 1, 0], [0, 2], [1], [0.5], [0.3, 0.2, 1]),
+                          ([0.2, 0.2, 1.1], [10, 10, 10], 2, [1, 0, 1], [1], [0, 2], [0.5], [0.3, 0.2, 1]),
+                          ([1.3, -0.2], [10, 10], 0, [0, 0], [0, 1], [], [0.55], [1, 0.1]),
+                          ([1, -0.2], [10, 10], 1, [0, 0], [0, 1], [], [0.8], [0.8, 0]),
+                          ([1.3, 0.9, -0.2, 1], [10, 10, 10, 10], 0, [0, 1, 0, 1], [0, 2], [1, 3], [0.75], [1, 0.9, 0.1, 1])
+                         ]
+                         )
+
+def test_correct_subsystem_soc(soc, capacity, subsystem_counter, btm_ftm, indices_btm, indices_ftm,
+                               system_state_soc, result, uut):
+    sub_system_states = []
+    system_state = SystemState(0, 0)
+    system_state.soc = system_state_soc
+    for i in range(len(soc)):
+        sub_system_states.append(SystemState(0, 0))
+        sub_system_states[i].soc = soc[i]
+        sub_system_states[i].capacity = capacity[i]
+    result_sub_system_states = uut.correct_subsystem_soc(sub_system_states, subsystem_counter, btm_ftm,
+                                                         indices_btm, indices_ftm, system_state)
+
+    result_soc = []
+    for j in range(len(soc)):
+        result_soc.append(np.round(result_sub_system_states[j].soc, 6))
+
+    assert result_soc == result
 
 @pytest.mark.parametrize('soc, capacity, power_requested, indices_btm, indices_ftm, btm_ftm, result',
                          [
                              #  nur von unteren leihen
-
                              ([0.5, 0.5], [10, 10], [3, 3], [0, 1], [], [0, 0], [3, 3]),
                              ([0.5, 0.5], [10, 10], [3, 3], [], [0, 1], [1, 1], [3, 3]),
                              ([0.5, 0.5], [10, 10], [20, 5], [0, 1], [], [0, 0], [10, 0]),
                              ([0.5, 0.5], [10, 10], [20, 5], [], [0, 1], [1, 1], [10, 0]),
 
-                             ([0.5, 0.5], [10, 10], [6, 5], [0, 1], [], [0, 0], [6, 4]), # TODO: Was soll das Result sein?
+                             ([0.5, 0.5], [10, 10], [6, 5], [0, 1], [], [0, 0], [6, 4]),
                              ([1, 1], [10, 10], [-6, -5], [0, 1], [], [0, 0], [-6, -5]),
                              ([1, 1], [10, 10], [-11, -10], [0, 1], [], [0, 0], [-11, -9]),
                              ([0.5, 0.5], [10, 10], [6, 5], [], [0, 1], [1, 1], [6, 4]),
                              ([1, 1], [10, 10], [-6, -5], [], [0, 1], [1, 1], [-6, -5]),
                              ([1, 1], [10, 10], [-11, -10], [], [0, 1], [1, 1], [-11, -9]),
+                             ([0, 0.5], [10, 10], [-5, 0], [0, 1], [], [0, 0], [-5, 0]),
 
                              ([0.5, 0.5], [10, 10], [8, 0], [0, 1], [], [0, 0], [8, 0]),
                              ([0.5, 0.5], [10, 10], [8, 0], [], [0, 1], [1, 1], [8, 0]),
                              ([0.5, 0.5], [10, 10], [15, 0], [0, 1], [], [0, 0], [10, 0]),
                              ([0.5, 0.5], [10, 10], [15, 0], [], [0, 1], [1, 1], [10, 0]),
 
                              ([0.8, 0.1], [10, 10], [-10, 0], [0, 1], [], [0, 0], [-9, 0]),
@@ -270,150 +240,165 @@
         sub_system_states.append(SystemState(0, 0))
         sub_system_states[i].soc = soc[i]
         sub_system_states[i].capacity = capacity[i]
     power_requested, borrowed_capacity = uut.check_subsystem_soc_allows_power(indices_btm, indices_ftm, btm_ftm, power_requested,
                                                                         sub_system_states, borrowed_capacity)
     assert power_requested == result
 
-# @pytest.mark.parametrize('power_requested_list, max_power_allocated, btm_ftm, result',
-#                          [
-#                              ([1, 1], 10, [0, 0], [1, 1]),
-#                              ([-1, -1], 10, [0, 0], [-1, -1]),
-#                              ([1, -5], 10, [0, 0], [1, -5]),
-#                              ([-5, 5], 10, [0, 0], [-5, 5]),
-#                              ([1, 1], 10, [1, 1], [1, 1]),
-#                              ([-1, -1], 10, [1, 1], [-1, -1]),
-#                              ([1, -5], 10, [1, 1], [1, -5]),
-#                              ([-5, 5], 10, [1, 1], [-5, 5]),
-#
-#                              ([1, 1], 10, [0, 1], [1, 1]),
-#                              ([-1, -1], 10, [0, 1], [-1, -1]),
-#                              ([1, -5], 10, [0, 1], [1, -5]),
-#                              ([-5, 5], 10, [0, 1], [-5, 5]),
-#                              ([1, 1], 10, [1, 0], [1, 1]),
-#                              ([-1, -1], 10, [1, 0], [-1, -1]),
-#                              ([1, -5], 10, [1, 0], [1, -5]),
-#                              ([-5, 5], 10, [1, 0], [-5, 5]),
-#
-#                              ([10, 1], 10, [0, 0], [10, 0]),
-#                              ([1, 10], 10, [0, 0], [1, 9]),
-#                              ([-10, 5], 10, [0, 0], [-10, 5]),
-#                              ([-5, 25], 10, [0, 0], [-5, 15]),
-#                              ([15, -5], 10, [0, 0], [15, -5]),
-#                              ([-5, 25], 10, [0, 0], [-5, 15]),
-#                              ([-10, -1], 10, [0, 0], [-10, 0]),
-#                              ([-1, -10], 10, [0, 0], [-1, -9]),
-#
-#                              ([10, 1], 10, [1, 1], [10, 0]),
-#                              ([1, 10], 10, [1, 1], [1, 9]),
-#                              ([-10, 5], 10, [1, 1], [-10, 5]),
-#                              ([-5, 25], 10, [1, 1], [-5, 15]),
-#                              ([15, -5], 10, [1, 1], [15, -5]),
-#                              ([-5, 25], 10, [1, 1], [-5, 15]),
-#                              ([-10, -1], 10, [1, 1], [-10, 0]),
-#                              ([-1, -10], 10, [1, 1], [-1, -9]),
-#
-#                              ([10, 1], 10, [0, 1], [10, 0]),
-#                              ([1, 10], 10, [0, 1], [1, 9]),
-#                              ([-10, 5], 10, [0, 1], [-10, 0]),
-#                              ([-5, 25], 10, [0, 1], [-5, 5]),
-#                              ([15, -5], 10, [0, 1], [10, 0]),
-#                              ([-5, 25], 10, [0, 1], [-5, 5]),
-#                              ([-10, -1], 10, [0, 1], [-10, 0]),
-#                              ([-1, -10], 10, [0, 1], [-1, -9]),
-#
-#                              ([10, 1], 10, [1, 0], [10, 0]),
-#                              ([1, 10], 10, [1, 0], [1, 9]),
-#                              ([-10, 5], 10, [1, 0], [-10, 0]),
-#                              ([-5, 25], 10, [1, 0], [-5, 5]),
-#                              ([15, -5], 10, [1, 0], [10, 0]),
-#                              ([-5, 25], 10, [1, 0], [-5, 5]),
-#                              ([-10, -1], 10, [1, 0], [-10, 0]),
-#                              ([-1, -10], 10, [1, 0], [-1, -9]),
-#
-#                              ([1, 1, 1], 10, [0, 0, 0], [1, 1, 1]),
-#                              ([10, 1, 1], 10, [0, 0, 0], [10, 0, 0]),
-#                              ([10, -5, 6], 10, [0, 0, 0], [10, -5, 5]),
-#                              ([1, 1, 1], 10, [0, 0, 1], [1, 1, 1]),
-#
-#                              ([5, 5, 3], 10, [0, 0, 1], [5, 5, 0]),
-#                              ([1, 1, 5], 10, [0, 0, 1], [1, 1, 5]),
-#                              ([10, 1, 1], 10, [0, 0, 1], [10, 0, 0]),
-#
-#                              ([5, 5, -3], 10, [0, 0, 1], [5, 5, 0]),
-#                              ([3, 2, -6], 10, [0, 0, 1], [3, 2, -5]),
-#
-#                              ([5, -1, 10], 10, [0, 0, 1], [5, -1, 6]),
-#                              ([1, -11, 10], 10, [0, 0, 1], [1, -11, 0]),
-#                              ([10, -5, 5], 10, [0, 0, 1], [10, -5, 5]),
-#
-#                              ([-10, 5, 20], 10, [0, 0, 1], [-10, 5, 5]),
-#                              ([-1, 20, 5], 10, [0, 0, 1], [-1, 11, 0]),
-#
-#                              ([10, -5, -20], 10, [0, 0, 1], [10, -5, -5]),
-#                              ([1, -20, -5], 10, [0, 0, 1], [1, -11, 0]),
-#
-#                              ([-1, -5, -20], 10, [0, 0, 1], [-1, -5, -4]),
-#                              ([-1, -20, -5], 10, [0, 0, 1], [-1, -9, 0]),
-#
-#                              ([-10, 5, -20], 10, [0, 0, 1], [-10, 5, -5]),
-#                              ([-1, 20, -5], 10, [0, 0, 1], [-1, 11, 0]),
-#
-#                              ([-10, -5, 20], 10, [0, 0, 1], [-10, 0, 0]),
-#                              ([-5, -5, 20], 10, [0, 0, 1], [-5, -5, 0]),
-#                              ([-2, -2, 10], 10, [0, 0, 1], [-2, -2, 6]),
-#
-#
-#                              ([1, 1, 1], 10, [1, 1, 0], [1, 1, 1]),
-#                              ([10, -5, 5], 10, [1, 1, 0], [10, -5, 5]),
-#                              ([1, 10, 1], 10, [1, 1, 0], [1, 9, 0]),
-#                              ([-5, -5, 20], 10, [1, 1, 0], [-5, -5, 0]),
-#
-#                              ([1, -1, -1, 1], 10, [1, 0, 1, 0], [1, -1, -1, 1]),
-#                              ([10, 10, -10, 10], 10, [1, 0, 1, 0], [10, 10, -10, 0]),
-#                              ([10, 20, -13, -5], 10, [1, 0, 1, 0], [10, 15, -10, -5])
-#                          ]
-#                          )
-#
-# def test_calculate_power_considering_ranking(power_requested_list, max_power_allocated, btm_ftm, result, uut):
-#     assert uut.calculate_power_considering_ranking(power_requested_list, max_power_allocated, btm_ftm) == result
-
-
-# @pytest.mark.parametrize('time, soc, capacity, result',
-#                          [
-#                              # (0, 0, 10, 8),  # TODO: Frage 2, und nochmal checken
-#                              # (0, 0.1, 10, 7.5),
-#                              # (0, 0.2, 10, 7),
-#                              # (0, 0.3, 10, 6.5),
-#                              # (0, 0.4, 10, 6),
-#                              # (0, 0.5, 10, 5),
-#                              # (0, 0.6, 10, 4),
-#                              # (0, 0.7, 10, 3),
-#                              # (0, 0.8, 10, 2),
-#                              # (0, 0.9, 10, 1),
-#                              # (0, 1, 10, 0),
-#                              #
-#                              # (1, 0.5, 10, 4.5),
-#                              # (1, 0.0, 10, 5),
-#                              # (1, 1.0, 10, 0),
-#                              #
-#                              # (2, 0.0, 10, 4),
-#                              # (2, 1.0, 10, 0),
-#                              #
-#                              # (3, 0.0, 10, 0),
-#                              # (3, 1.0, 10, 0),
-#                              #
-#                              # (2, 0.5, 10, 1),
-#                              # (3, 0.5, 10, 1),
-#                              # (4, 0.5, 10, 1),
-#                              #
-#                              # (5, 0.5, 10, 1),  # TODO: ????
-#                              # (5, 0.5, 10, -2),  # TODO: Frage 1
-#                              # (5, 0.5, 10, -2),
-#                          ]
-#                          )
-#
-# def test_next(time, soc, capacity, result, uut):
-#     system_state = SystemState(0, 0)
-#     system_state.soc = soc
-#     system_state.capacity = capacity
-#     assert uut.next(time, system_state) == result
+@pytest.mark.parametrize('power_requested_list, max_power_allocated, btm_ftm, result',
+                         [
+                             ([100, 100], 50, [0, 0], [50, 0]),
+
+                             ([1, 1], 10, [0, 0], [1, 1]),
+                             ([-1, -1], 10, [0, 0], [-1, -1]),
+                             ([1, -5], 10, [0, 0], [1, -5]),
+                             ([-5, 5], 10, [0, 0], [-5, 5]),
+                             ([1, 1], 10, [1, 1], [1, 1]),
+                             ([-1, -1], 10, [1, 1], [-1, -1]),
+                             ([1, -5], 10, [1, 1], [1, -5]),
+                             ([-5, 5], 10, [1, 1], [-5, 5]),
+
+                             ([1, 1], 10, [0, 1], [1, 1]),
+                             ([-1, -1], 10, [0, 1], [-1, -1]),
+                             ([1, -5], 10, [0, 1], [1, -5]),
+                             ([-5, 5], 10, [0, 1], [-5, 5]),
+                             ([1, 1], 10, [1, 0], [1, 1]),
+                             ([-1, -1], 10, [1, 0], [-1, -1]),
+                             ([1, -5], 10, [1, 0], [1, -5]),
+                             ([-5, 5], 10, [1, 0], [-5, 5]),
+
+                             ([10, 1], 10, [0, 0], [10, 0]),
+                             ([1, 10], 10, [0, 0], [1, 9]),
+                             ([-10, 5], 10, [0, 0], [-10, 5]),
+                             ([-5, 25], 10, [0, 0], [-5, 15]),
+                             ([15, -5], 10, [0, 0], [15, -5]),
+                             ([-5, 25], 10, [0, 0], [-5, 15]),
+                             ([-10, -1], 10, [0, 0], [-10, 0]),
+                             ([-1, -10], 10, [0, 0], [-1, -9]),
+
+                             ([10, 1], 10, [1, 1], [10, 0]),
+                             ([1, 10], 10, [1, 1], [1, 9]),
+                             ([-10, 5], 10, [1, 1], [-10, 5]),
+                             ([-5, 25], 10, [1, 1], [-5, 15]),
+                             ([15, -5], 10, [1, 1], [15, -5]),
+                             ([-5, 25], 10, [1, 1], [-5, 15]),
+                             ([-10, -1], 10, [1, 1], [-10, 0]),
+                             ([-1, -10], 10, [1, 1], [-1, -9]),
+
+                             ([10, 1], 10, [0, 1], [10, 0]),
+                             ([1, 10], 10, [0, 1], [1, 9]),
+                             ([-10, 5], 10, [0, 1], [-10, 0]),
+                             ([-5, 25], 10, [0, 1], [-5, 5]),
+                             ([15, -5], 10, [0, 1], [10, 0]),
+                             ([-5, 25], 10, [0, 1], [-5, 5]),
+                             ([-10, -1], 10, [0, 1], [-10, 0]),
+                             ([-1, -10], 10, [0, 1], [-1, -9]),
+
+                             ([10, 1], 10, [1, 0], [10, 0]),
+                             ([1, 10], 10, [1, 0], [1, 9]),
+                             ([-10, 5], 10, [1, 0], [-10, 0]),
+                             ([-5, 25], 10, [1, 0], [-5, 5]),
+                             ([15, -5], 10, [1, 0], [10, 0]),
+                             ([-5, 25], 10, [1, 0], [-5, 5]),
+                             ([-10, -1], 10, [1, 0], [-10, 0]),
+                             ([-1, -10], 10, [1, 0], [-1, -9]),
+
+                             ([1, 1, 1], 10, [0, 0, 0], [1, 1, 1]),
+                             ([10, 1, 1], 10, [0, 0, 0], [10, 0, 0]),
+                             ([10, -5, 6], 10, [0, 0, 0], [10, -5, 5]),
+                             ([1, 1, 1], 10, [0, 0, 1], [1, 1, 1]),
+
+                             ([5, 5, 3], 10, [0, 0, 1], [5, 5, 0]),
+                             ([1, 1, 5], 10, [0, 0, 1], [1, 1, 5]),
+                             ([10, 1, 1], 10, [0, 0, 1], [10, 0, 0]),
+
+                             ([5, 5, -3], 10, [0, 0, 1], [5, 5, 0]),
+                             ([3, 2, -6], 10, [0, 0, 1], [3, 2, -5]),
+
+                             ([5, -1, 10], 10, [0, 0, 1], [5, -1, 6]),
+                             ([1, -11, 10], 10, [0, 0, 1], [1, -11, 0]),
+                             ([10, -5, 5], 10, [0, 0, 1], [10, -5, 5]),
+
+                             ([-10, 5, 20], 10, [0, 0, 1], [-10, 5, 5]),
+                             ([-1, 20, 5], 10, [0, 0, 1], [-1, 11, 0]),
+
+                             ([10, -5, -20], 10, [0, 0, 1], [10, -5, -5]),
+                             ([1, -20, -5], 10, [0, 0, 1], [1, -11, 0]),
+
+                             ([-1, -5, -20], 10, [0, 0, 1], [-1, -5, -4]),
+                             ([-1, -20, -5], 10, [0, 0, 1], [-1, -9, 0]),
+
+                             ([-10, 5, -20], 10, [0, 0, 1], [-10, 5, -5]),
+                             ([-1, 20, -5], 10, [0, 0, 1], [-1, 11, 0]),
+
+                             ([-10, -5, 20], 10, [0, 0, 1], [-10, 0, 0]),
+                             ([-5, -5, 20], 10, [0, 0, 1], [-5, -5, 0]),
+                             ([-2, -2, 10], 10, [0, 0, 1], [-2, -2, 6]),
+
+
+                             ([1, 1, 1], 10, [1, 1, 0], [1, 1, 1]),
+                             ([10, -5, 5], 10, [1, 1, 0], [10, -5, 5]),
+                             ([1, 10, 1], 10, [1, 1, 0], [1, 9, 0]),
+                             ([-5, -5, 20], 10, [1, 1, 0], [-5, -5, 0]),
+
+                             ([1, -1, -1, 1], 10, [1, 0, 1, 0], [1, -1, -1, 1]),
+                             ([10, 10, -10, 10], 10, [1, 0, 1, 0], [10, 10, -10, 0]),
+                             ([10, 20, -13, -5], 10, [1, 0, 1, 0], [10, 15, -10, -5])
+                         ]
+                         )
+
+def test_calculate_power_considering_ranking(power_requested_list, max_power_allocated, btm_ftm, result, uut):
+    assert uut.calculate_power_considering_ranking(power_requested_list, max_power_allocated, btm_ftm) == result
+
+
+@pytest.mark.parametrize('time, start_soc, capacity, result',
+                         [
+
+                             (0, 0, 10, 8),  # Time = 0, Power PS = 3, Power SCI = 5
+                             (0, 0.1, 10, 7.5),
+                             (0, 0.2, 10, 7),
+                             (0, 0.3, 10, 6.5),
+                             (0, 0.4, 10, 6),
+                             (0, 0.5, 10, 5),
+                             (0, 0.6, 10, 4),
+                             (0, 0.7, 10, 3),
+                             (0, 0.8, 10, 2),
+                             (0, 0.9, 10, 1),
+                             (0, 1, 10, 0),
+
+                             (1, 0.0, 10, 5),  # Time = 1, Power PS = 2, Power SCI = 3
+                             (1, 0.1, 10, 5),
+                             (1, 0.2, 10, 5),
+                             (1, 0.3, 10, 5),
+                             (1, 0.4, 10, 5),
+                             (1, 0.5, 10, 4.5),
+                             (1, 0.6, 10, 4),
+                             (1, 0.7, 10, 3),
+                             (1, 0.8, 10, 2),
+                             (1, 0.9, 10, 1),
+                             (1, 1.0, 10, 0),
+
+                             (2, 0.0, 10, 2),  # Time: 2, Power PS = 1, Power SCI = 1
+                             (2, 0.1, 10, 2),
+                             (2, 0.9, 10, 1),
+                             (2, 1.0, 10, 0),
+
+                             (3, 0.0, 10, 0),  # Time = 3, Power PS = 0, Power SCI = -1
+                             (3, 0.1, 10, -0.5),
+                             (3, 0.2, 10, -1),
+                             (3, 1.0, 10, -1),
+
+                             (4, 0.0, 10, 0),  # Time = 4, Power PS = -1, Power SCI = -3
+                             (4, 0.5, 10, -3.5),
+                             (4, 1.0, 10, -4),
+
+                             (5, 0.0, 10, 0),  # Time = 5, Power PS = -2, Power SCI = -5
+                             (5, 0.5, 10, -4.5),
+                             (5, 1, 10, -7)
+                         ]
+                         )
+
+def test_next(time, start_soc, capacity, result, uut):
+    system_state = SystemState(0, 0)
+    system_state.soc = start_soc
+    system_state.capacity = capacity
+    assert uut.next(time, system_state) == result
```

### Comparing `simses-1.3.2/simses/logic/test/test_peak_shaving.py` & `simses-1.3.3/simses/logic/test/test_peak_shaving.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/logic/test/test_residential_pv_greedy.py` & `simses-1.3.3/simses/logic/test/test_residential_pv_greedy.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/logic/test/test_soc_based_power_distributor.py` & `simses-1.3.3/simses/logic/test/test_soc_based_power_distributor.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/logic/thermal_management/on_off_controller.py` & `simses-1.3.3/simses/logic/thermal_management/on_off_controller.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/logic/thermal_management/pid_controller.py` & `simses-1.3.3/simses/logic/thermal_management/pid_controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,80 +5,93 @@
 import pandas as pd
 import os
 import time
 
 
 class PIDController(ThermalManagement):
 
-    TEMPERATURE_DEAD_BAND: float = 2.0  # K
+    TEMPERATURE_DEAD_BAND: float = 2  # K
 
     def __init__(self, set_point: float, hvac_max_thermal_power: float):
         super().__init__()
+        self.__export_running_data = False
         self.__set_temperature = set_point  # K
         self.__hvac_rated_thermal_power = hvac_max_thermal_power  # W
-        self.__kp_coefficient = 10000
-        self.__ki_coefficient = 100
+        self.__kp_coefficient = 8000
+        self.__ki_coefficient = 200
         self.__kd_coefficient = 1800
         self.__thermal_power_scaling_factor = 1
         self.__temperature_difference_memory = [0]
         self.__i_temperature_difference = 0
+
         # Export running data
-        # self.__file_name = os.getcwd() + '\\controller_running_data\\Results' + str(time.time()) + '.csv'
-        # df = pd.DataFrame(['Ti', 'Ta', 'Total Thermal Power', 'HVAC Thermal Power', 'Fan Power', 'Required thermal power', 'P_Difference', 'I_Difference', 'D_Difference', 'HVAC Limit']).T
-        # df.to_csv(self.__file_name, header=None, index=None)
+        if self.__export_running_data:
+            self.__file_name = os.getcwd() + '\\controller_running_data\\Results' + str(time.time()) + '.csv'
+            df = pd.DataFrame(['Ti', 'Ta', 'Total Thermal Power', 'HVAC Thermal Power', 'Fan Power', 'Required thermal power', 'P_Difference', 'I_Difference', 'D_Difference', 'HVAC Limit']).T
+            df.to_csv(self.__file_name, header=None, index=None)
 
     def compute(self, internal_air_temperature: float, ambient_air_temperature: float, air_mass: float,
                 air_density: float, time_step: float, fan: Fan) -> list:
         p_temperature_difference = float(internal_air_temperature - self.__set_temperature)
         self.__i_temperature_difference += p_temperature_difference
         self.__temperature_difference_memory.append(p_temperature_difference)
         d_temperature_difference = (self.__temperature_difference_memory[-1] - self.__temperature_difference_memory[-2])
 
         required_thermal_power = self.__thermal_power_scaling_factor * \
                                  (self.__kp_coefficient * p_temperature_difference +
                                   self.__ki_coefficient * self.__i_temperature_difference +
-                                  self.__kd_coefficient * d_temperature_difference)
+                                  self.__kd_coefficient * d_temperature_difference)  # W
 
-        if sign(required_thermal_power) == sign(p_temperature_difference) and abs(p_temperature_difference) > self.TEMPERATURE_DEAD_BAND:  # Filter with deadband to prevent overcooling / overheating
+        if sign(required_thermal_power) == sign(p_temperature_difference) and abs(p_temperature_difference) > self.TEMPERATURE_DEAD_BAND:
+            # -ve thermal power: heating, +ve thermal power: cooling
+            # Filter with deadband to prevent overcooling / overheating
 
             rated_supply_temperature = float(self.__set_temperature - sign(required_thermal_power) * 10)  # K
-            rated_fresh_air_thermal_power = fan.rated_airflow * air_density * (internal_air_temperature - ambient_air_temperature) * ZeroDSystemThermalModel.AIR_SPECIFIC_HEAT  # W
-            max_physical_fresh_air_thermal_power = air_mass * (internal_air_temperature - ambient_air_temperature) * ZeroDSystemThermalModel.AIR_SPECIFIC_HEAT / time_step  # W
-
-            if sign(required_thermal_power) == sign(max_physical_fresh_air_thermal_power):
-                # if the fresh air thermal power is usable
-                fresh_air_thermal_power = min(max(abs(max_physical_fresh_air_thermal_power), abs(rated_fresh_air_thermal_power)), abs(required_thermal_power)) * float(sign(required_thermal_power))  # W
-                hvac_thermal_power_limit = fan.rated_airflow * air_density * (ambient_air_temperature - rated_supply_temperature) * ZeroDSystemThermalModel.AIR_SPECIFIC_HEAT  # W
+            delta_temperature_internal_ambient = float(internal_air_temperature - ambient_air_temperature)  # K
+            rated_fresh_air_thermal_power = float(fan.rated_airflow * air_density * delta_temperature_internal_ambient * ZeroDSystemThermalModel.AIR_SPECIFIC_HEAT)  # W
+            max_physical_fresh_air_thermal_power = float(air_mass * delta_temperature_internal_ambient * ZeroDSystemThermalModel.AIR_SPECIFIC_HEAT / time_step)  # W
+
+            if sign(required_thermal_power) == sign(delta_temperature_internal_ambient):
+                # checks if the fresh air thermal power is usable
+                # -ve delta_temperature_internal_ambient: outside hotter, +ve: outside cooler
+                fresh_air_thermal_power = min(min(abs(max_physical_fresh_air_thermal_power), abs(rated_fresh_air_thermal_power)), abs(required_thermal_power)) * float(sign(required_thermal_power))  # W
                 if fresh_air_thermal_power / required_thermal_power >= 0.999:
                     # first case: the requirement can be met only with fresh air
                     hvac_thermal_power = 0.0  # W
+                else:
+                    # second case: fresh air thermal power is not enough, use HVAC
+                    if abs(rated_supply_temperature) - abs(ambient_air_temperature) > 0.1:
+                        hvac_thermal_power = float(min(abs(self.__hvac_rated_thermal_power),
+                                                       abs(required_thermal_power) - abs(fresh_air_thermal_power)) * sign(required_thermal_power))  # W
+                    else:
+                        hvac_thermal_power = 0.0
+
+                airflow_ratio = (fresh_air_thermal_power / rated_fresh_air_thermal_power)  # m3/s
+                if airflow_ratio <= 1:
                     airflow = fan.rated_airflow * (fresh_air_thermal_power / rated_fresh_air_thermal_power)  # m3/s
                 else:
-                    # second case: fresh air thermal power is not enough, the rest is from HVAC
-                    hvac_thermal_power = float(min(abs(self.__hvac_rated_thermal_power),
-                                                    abs(required_thermal_power - fresh_air_thermal_power),
-                                                    abs(hvac_thermal_power_limit)) * sign(required_thermal_power))  # W
-                    airflow = fan.rated_airflow  # m3/s
+                    airflow = fan.rated_airflow
             else:
-                # third case: fresh air cannot be used. HVAC only
+                # third case: fresh air can not be used. HVAC only.
                 fresh_air_thermal_power = 0.0  # W
-                hvac_thermal_power_limit = fan.rated_airflow * air_density * (internal_air_temperature - rated_supply_temperature) * ZeroDSystemThermalModel.AIR_SPECIFIC_HEAT  # W
-                hvac_thermal_power = float(min(abs(self.__hvac_rated_thermal_power), abs(required_thermal_power - fresh_air_thermal_power), abs(hvac_thermal_power_limit)) * sign(required_thermal_power))  # W
-                if internal_air_temperature != rated_supply_temperature:
-                    airflow = hvac_thermal_power / ((internal_air_temperature - rated_supply_temperature) * ZeroDSystemThermalModel.AIR_SPECIFIC_HEAT * air_density)  # m3/s
+                if abs(rated_supply_temperature) - abs(ambient_air_temperature) > 0.1:
+                    hvac_thermal_power = float(min(abs(self.__hvac_rated_thermal_power), abs(required_thermal_power)) * sign(required_thermal_power))  # W
                 else:
-                    airflow = 0.0  # m3/s
+                    hvac_thermal_power = 0.0
+                airflow = 0.0  # m3/s
         else:
             hvac_thermal_power = 0.0  # W
             fresh_air_thermal_power = 0.0  # W
             airflow = 0.0  # m3/s
         total_thermal_power = float(hvac_thermal_power + fresh_air_thermal_power)  # W
         fan.run(airflow)
 
         # Export running data
-        # data_list = [float(internal_air_temperature), ambient_air_temperature, total_thermal_power, hvac_thermal_power,
-        #             fan.electricity_consumption, required_thermal_power, p_temperature_difference,
-        #             self.__i_temperature_difference, d_temperature_difference, self.__hvac_rated_thermal_power]
-        # df = pd.DataFrame(data_list).T
-        # df.to_csv(self.__file_name, mode='a', header=None, index=None)
+        if self.__export_running_data:
+            data_list = [float(internal_air_temperature), ambient_air_temperature, total_thermal_power, hvac_thermal_power,
+                        fan.electricity_consumption, required_thermal_power, p_temperature_difference,
+                        self.__i_temperature_difference, d_temperature_difference, self.__hvac_rated_thermal_power]
+            df = pd.DataFrame(data_list).T
+            df.to_csv(self.__file_name, mode='a', header=None, index=None)
+
         return [float(total_thermal_power), float(hvac_thermal_power)]
```

### Comparing `simses-1.3.2/simses/main.py` & `simses-1.3.3/simses/simulation/simulator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,261 +1,249 @@
 import os
-import threading
+import sys
+import time
 from configparser import ConfigParser
+from math import floor
 from multiprocessing import Queue
-from os.path import dirname
-from simses.analysis.storage import StorageAnalysis
-from simses.commons.config.log import LogConfig
+from queue import Full
+
+from simses.commons.config.abstract_config import Config
+from simses.commons.config.data.data_config import DataConfig
+from simses.commons.config.simulation.general import GeneralSimulationConfig
+from simses.commons.console_printer import ConsolePrinter
+from simses.commons.data.csv_data_handler import CSVDataHandler
+from simses.commons.data.no_data_handler import NoDataHandler
+from simses.commons.error import EndOfLifeError
+from simses.commons.log import Logger
+from simses.commons.state.parameters import SystemParameters
 from simses.commons.state.system import SystemState
-from simses.commons.utils.utilities import create_directory_for
-from simses.simulation.simulator import StorageSimulation
+from simses.commons.utils.utilities import format_float
+from simses.logic.energy_management.energy_management_system import EnergyManagement
+from simses.system.storage_circuit import StorageCircuit
 
 
-class SimSES(threading.Thread):
+class StorageSimulation:
 
     """
-    SimSES is a simulation and analysis tool for complex energy storage systems. The tool can be used via the run method
-    (or alternatively as a Thread with its start method). The simulation and analysis can be run separately, the
-    analysis takes the results of the last run from the configured simulation.
-
-    SimSES can be configured via the INI files in config. DEFAULT configs (*.defaults.ini) can be overwritten by
-    LOCAL configs (*.local.ini). Furthermore, the configs can be overwritten by a ConfigParser passed to the SimSES
-    constructor. This is especially useful for sensitivity analysis.
-
-    The processing package provides a functionality for multiple simulations and analysis by using all available cores.
-    For this purpose, python's multiprocessing package is used. An example as well as a readme is provided in the
-    processing package how to use and configure it.
-
-    SimSES can also be used directly in other tools by providing the run_one_simulation_step and
-    evaluate_multiple_simulation_steps methods. With these methods SimSES can be integrated in other simulation
-    frameworks acting as a storage system. SimSES needs to be closed manually after the simulation from outer scope is
-    completed.
+    StorageSimulation constructs the the storage systems and energy management system in order to execute the simulation.
+    In the run() method the timestamp for the simulation is advanced as configured. Alternatively, simulation is included
+    in another framework advancing timestamps itself, e.g. run_one_step() or evaluate_multiple_steps(). StorageSimulation
+    also provided information of the current status of the simulation to the user.
     """
 
-    __DIR: str = dirname(__file__)
-    __VERSION_FILE: str = __DIR + '/VERSION'
-    __GIT_FILE: str = __DIR + '/../.git/FETCH_HEAD'
-
-    def __init__(self, path: str, name: str, do_simulation: bool = True, do_analysis: bool = True,
-                 simulation_config: ConfigParser = None, analysis_config: ConfigParser = None, queue: Queue = None,
-                 batch_dir: str = 'batch/'):
+    def __init__(self, path: str, config: ConfigParser, printer_queue: Queue):
         """
-        Constructor of SimSES
+        Constructor of StorageSimulation
 
         Parameters
         ----------
         path :
-            absolute path where to store results
-        name :
-            simulation name (will be concatenated with path to a unique path)
-        do_simulation :
-            flag for allowing or prohibiting execution of the simulation
-        do_analysis :
-            flag for allowing or prohibiting execution of the analysis
-        simulation_config :
-            ConfigParser overwriting configuration provided by INI files for simulation
-        analysis_config :
-            ConfigParser overwriting configuration provided by INI files for analysis
-        queue :
-            PrinterQueue provides progess information for the user in case of using the processing package
-        batch_dir :
-            Relative path of directory for comparison of results from multiple simulations using the processing package
-        """
-        super().__init__()
-        self.__do_simulation = do_simulation
-        self.__do_analysis = do_analysis
-        self.__name: str = name
-        batch_dir = path + batch_dir
-        self.__path = path + name + '/'
-        if self.__do_simulation:
-            create_directory_for(path)
-            self.__storage_simulation: StorageSimulation = StorageSimulation(self.__path, simulation_config, queue)
-        if self.__do_analysis:
-            self.__storage_analysis: StorageAnalysis = StorageAnalysis(self.__path, analysis_config, batch_dir, self.version)
+            path to result folder
+        config :
+            Optional configs taken into account overwriting values from provided config file
+        printer_queue :
+            Optional queue for concurrent simulation process for providing progress status of simulations
+        """
+        self.__path = path
+        self.__log = Logger(type(self).__name__)
+        # Only instantiated in order write data config to results folder, maybe this way should be improved
+        self.__data_config: Config = DataConfig(None, None)
+        self.__config = GeneralSimulationConfig(config)
+        if self.__config.export_data:
+            self.__data_export = CSVDataHandler(path, self.__config)
+        else:
+            self.__data_export = NoDataHandler()
+        self.__energy_management: EnergyManagement = EnergyManagement(self.__data_export, config)
+        self.__storage_system = StorageCircuit(self.__data_export, config)
+        self.__name: str = os.path.basename(os.path.dirname(self.__path))
+        self.__printer_queue: Queue = printer_queue
+        self.__send_register_signal()
+        self.__max_loop = self.__config.loop
+        self.__start = self.__config.start
+        self.__end = self.__config.end
+        self.__timestep = self.__config.timestep  # sec
+        # duration to the last executed time step
+        self.__duration = floor((self.__end - self.__start) / self.__timestep) * self.__timestep
+        self.__timesteps_per_hour = 3600 / self.__timestep
+        system_parameters: SystemParameters = SystemParameters()
+        system_parameters.set_all(self.__storage_system.get_system_parameters())
+        system_parameters.write_parameters_to(path)
 
-    @property
-    def name(self) -> str:
-        """
-        Returns
-        -------
-        str:
-            string representation of the simulation name
+    def run(self) -> None:
         """
-        return self.__name
+        Executes simulation
 
-    @property
-    def version(self) -> str:
-        """
         Returns
         -------
-        str:
-            current version of simses including, if available, git commit hash (short version) from last fetch
-        """
-        version = self.__get_version_simses()
-        version += self.__get_version_git()
-        return version
-
-    def __get_version_git(self):
-        version: str = ''
-        try:
-            with open(self.__GIT_FILE, 'r') as file:
-                version += '-' + file.readline().split('\t')[0].rstrip()[:8]
-        except FileNotFoundError:
-            pass
-        return version
 
-    def __get_version_simses(self):
-        version: str = ''
+        """
+        self.__log.info('start')
+        sim_start = time.time()
+        ts_performance = []
         try:
-            with open(self.__VERSION_FILE, 'r') as file:
-                version += file.readline().rstrip()
-        except FileNotFoundError:
-            version = 'unknown'
-        return version
+            loop = 0
+            ts = self.__start
+            while loop < self.__max_loop:
+                self.__log.info('Loop: ' + str(loop))
+                ts_adapted = loop * self.__duration
+                while ts <= (ts_adapted + self.__end) - self.__timestep:
+                    ts_before = time.time()
+                    ts += self.__timestep
+                    self.run_one_step(ts, ts_adapted)
+                    ts_performance.append(time.time() - ts_before)
+                    self.__print_progress(ts)
+                loop += 1
+                if loop < self.__max_loop:
+                    ts_adapted = loop * self.__duration
+                    self.reset_profiles(ts_adapted)
+        except EndOfLifeError as err:
+            self.__log.error(err)
+        finally:
+            self.close()
+            self.__print_end(ts_performance, sim_start)
+
+    def __print_progress(self, tstmp: float) -> None:
+        progress = (tstmp - self.__start) / (self.__duration * self.__max_loop) * 100
+        line: str = '|%-20s| ' % ('#' * round(progress / 5)) + format_float(progress, 1) + '%'
+        output: dict = {self.__name: line}
+        if self.__printer_queue is None:
+            sys.stdout.write('\r' + str(output))
+            sys.stdout.flush()
+        self.__put_to_queue(output)
+
+    def __put_to_queue(self, output: dict, blocking: bool = False) -> None:
+        if self.__printer_queue is not None:
+            try:
+                if blocking:
+                    self.__printer_queue.put(output)
+                else:
+                    self.__printer_queue.put_nowait(output)
+            except Full:
+                return
 
-    def run(self) -> None:
-        """
-        Runs the configured simulation and analysis and closes afterwards
-        """
-        self.run_simulation()
-        self.run_analysis()
-        self.close()
+    def __send_stop_signal(self) -> None:
+        self.__put_to_queue({self.__name: ConsolePrinter.STOP_SIGNAL}, blocking=True)
 
-    def run_one_simulation_step(self, time: float, power: float = None, power_dist: [float] = None) -> None:
-        """
-        Runs only one step of the simulation with the given time and power. The system is configured as mentioned
-        in the class description.
+    def __send_register_signal(self) -> None:
+        self.__put_to_queue({self.__name: ConsolePrinter.REGISTER_SIGNAL}, blocking=True)
 
-        If no power value is provided, the configured energy management system will provide a power value for
-        the given time.
+    def __print_end(self, ts_performance: list, sim_start: float) -> None:
+        try:
+            sim_end = time.time()
+            duration: str = format_float(sim_end - sim_start)
+            duration_per_step: str = format_float(sum(ts_performance) * 1000 / len(ts_performance))
+            self.__log.info('100.0% done. Duration in sec: ' + duration)
+            self.__log.info('Duration per step in ms:      ' + duration_per_step)
+            if self.__printer_queue is None:
+                print('\r[' + self.__name + ': |%-20s| ' % ('#' * 20) + '100.0%]')
+                print('          Duration in s: ' + duration)
+                print('Duration per step in ms: ' + duration_per_step)
+        except ZeroDivisionError:
+            self.__log.warn('No performance indicators could be calculated.')
 
-        Calculated values can be received via the state property. It provides information about the whole
-        storage system, e.g. SOC.
+    def run_one_step(self, ts: float, ts_adapted: float = 0, power: float = None, power_dist: [float] = None) -> None:
+        """
+        Advances simulation for one step. Results can be obtained via state property.
 
         Parameters
         ----------
-        time :
-            epoch timestamp in s
+        ts :
+            next timestamp in s
+        ts_adapted :
+            timestamp adaption for looping simulations multiple times (should only be used with stand alone SimSES)
         power :
-            power value in W
-        power_dist:
-            power value in W for every AC system (optional external power distribution logic)
-        """
-        self.__storage_simulation.run_one_step(ts=time, power=power, power_dist=power_dist)
+            next power transfered to storage system in W, if None power is taken from configured energy management
+        power_dist :
+            next power distribution in W for every AC system as a list. If None, power is taken from power distributor classes.
+        Returns
+        -------
 
-    def evaluate_multiple_simulation_steps(self, start: float, timestep: float, power: list) -> [SystemState]:
         """
-        Runs multiple steps of the simulation with the given start time, timestep and power list. The system is
-        configured as mentioned in the class description.
+        if power_dist is None:
+            power_dist = []
+        state = self.__storage_system.state
+        if not self.__data_export.is_alive():
+            self.__data_export.start()
+        self.__data_export.transfer_data(state.to_export())
+        if power is None:
+            power = self.__energy_management.next(ts - ts_adapted, state)
+        try:
+            self.__storage_system.update(ts, power, power_dist)
+        finally:
+            self.__energy_management.export(ts)
 
+    def evaluate_multiple_steps(self, start: float, timestep: float, power: list) -> [SystemState]:
+        """
+        Runs multiple steps of the simulation with the given start time, timestep and power list.
         If no power list is provided, the simulation will not be advanced.
 
-        Calculated values will be returned. They provide information about the whole storage system, e.g. SOC,
-        for each timestep.
-
         Parameters
         ----------
         start :
             start time in s
         timestep :
             timestep in s
         power :
             list of power for each timestep in W
 
         Returns
         ----------
         list:
             Returns a list of system states for each timestep
-        """
-        return self.__storage_simulation.evaluate_multiple_steps(start, timestep, power)
 
-    def run_simulation(self) -> None:
         """
-        Runs only the simulation as configured, if allowed
-        """
-        if self.__do_simulation:
-            self.__storage_simulation.run()
-
-    def run_analysis(self) -> None:
-        """
-        Runs only the analysis as configured, if allowed
-        """
-        if self.__do_analysis:
-            self.__storage_analysis.run()
+        res: [SystemState] = list()
+        ts = start
+        for pow in power:
+            self.run_one_step(ts=ts, power=pow)
+            res.append(self.state)
+            ts += timestep
+        return res
 
     @property
     def state(self) -> SystemState:
         """
-        Usage only supported in combination with run_one_simulation_step
 
         Returns
         -------
         SystemState:
-            current state of the system providing information of calculated results
+            current state of top level system
         """
-        return self.__storage_simulation.state
+        return self.__storage_system.state
 
     @property
     def ac_system_states(self) -> [SystemState]:
         """
-        Usage only supported in combination with run_one_simulation_step
 
         Returns
         -------
-        [SystemState]:
-            current states of all AC systems providing information of calculated results
+        SystemState:
+            list of current states for all AC systems
         """
-        return self.__storage_simulation.ac_system_states
+        return self.__storage_system.ac_system_states
 
     def reset_profiles(self, ts_adapted: float) -> None:
         """
-        Enables looping of the simulation beyond the original length of the time series for the AmbientThermalModel and
-        SolarIrradiationModel
+        Enables looping of the simulation beyond the original length of the time series for all profile-based modules
+        such as the EnergyManagement, the AmbientThermalModel, and SolarIrradiationModel
         """
-        self.__storage_simulation.reset_profiles(ts_adapted)
+        self.__energy_management.close()
+        self.__energy_management: EnergyManagement = self.__energy_management.create_instance()
+        self.__storage_system.reset_profiles(ts_adapted)
 
     def close(self) -> None:
         """
-        Closes all resources of simulation and analysis
-        """
-        self.close_simulation()
-        self.close_analysis()
-
-    def close_simulation(self) -> None:
-        """
-        Closes all resources of simulation
-        """
-        if self.__do_simulation:
-            self.__storage_simulation.close()
-
-    def close_analysis(self) -> None:
-        """
-        Closes all resources of analysis
-        """
-        if self.__do_analysis:
-            self.__storage_analysis.close()
+        Closing all resources of simulation
 
-    @classmethod
-    def set_log_config(cls, configuration: ConfigParser) -> None:
-        """
-        Class method for setting the global log configuration
+        Returns
+        -------
 
-        Parameters
-        ----------
-        configuration :
-            ConfigParser will overwrite global log configuration
         """
-        LogConfig.set_config(configuration)
-
-
-if __name__ == "__main__":
-    # minimum working example
-    # config_generator: SimulationConfigGenerator = SimulationConfigGenerator()
-    # config_generator.set_simulation_time('2014-01-01 00:00:00', '2014-02-01 00:00:00')
-    # config: ConfigParser = config_generator.get_config()
-    path: str = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
-    result_path: str = os.path.join(path, 'results').replace('\\','/') + '/'
-    simulation_name: str = 'simses_1'
-    simses: SimSES = SimSES(result_path, simulation_name, do_simulation=True, do_analysis=True)
-    # simses: SimSES = SimSES(result_path, simulation_name, do_simulation=True, do_analysis=True, simulation_config=config)
-    simses.start()
-    simses.join()
+        self.__log.info('closing')
+        self.__data_export.transfer_data(self.__storage_system.state.to_export())
+        self.__send_stop_signal()
+        self.__config.write_config_to(self.__path)
+        self.__data_config.write_config_to(self.__path)
+        self.__log.close()
+        self.__data_export.close()
+        self.__energy_management.close()
+        self.__storage_system.close()
```

### Comparing `simses-1.3.2/simses/simulation/batch_processing.py` & `simses-1.3.3/simses/simulation/batch_processing.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/simulation/batch_simulation.py` & `simses-1.3.3/simses/simulation/batch_simulation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/simulation/case_studies/case_study_1_peak_shaving.py` & `simses-1.3.3/simses/simulation/case_studies/case_study_1_peak_shaving.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/simulation/case_studies/case_study_2_fcr.py` & `simses-1.3.3/simses/simulation/case_studies/case_study_2_fcr.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/simulation/example.py` & `simses-1.3.3/simses/simulation/example.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/simulation/simbas/room_tool_reader.py` & `simses-1.3.3/simses/simulation/simbas/room_tool_reader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,61 @@
 from pandas import DataFrame, read_csv
 
 
 class RoomToolReader:
 
-    __ROOM_TOOL_REPORT_FILE: str = 'report.csv'
+    # __ROOM_TOOL_REPORT_FILE: str = 'report.csv'
 
     __MANUFACTURER: str = "Manufacturer"
     __MODEL: str = "Model"
     __FORMAT: str = "Format"
     __CONFIGURATION: str = "Configuration"
     __VOLTAGE_MAX: str = "Voltage_max (V)"
     __VOLTAGE_MIN: str = "Voltage_min (V)"
-    __VOLTAGE_NOM: str = "Voltage_nom (V)"
+    __VOLTAGE_NOM_MODULE: str = "Nom. module voltage (V)"
     __WEIGHT: str = "Weight (kg)"
     __VOLUME: str = "Volume (m^3)"
     __COOLING_TYPE: str = "Cooling type"
     __ENERGY: str = "Energy (Wh)"
 
-    def __init__(self, cell: str):
+    def __init__(self, room_tool_file: str):
         # * We need a matching between selected cell and room tool
         # * we need to adapt not only serial / parallel but also voltage and capacity -> overwriting config
         # * How could we scale such a solution?
         # -> maybe we should not try to solve the interface on this low level but maybe on a high level e.g. batch
         #    processing
-        self.__data: DataFrame = self.__read_room_tool_report(cell)
+        self.__ROOM_TOOL_REPORT_FILE = room_tool_file
+        self.__data_room_tool_report: DataFrame = read_csv(self.__ROOM_TOOL_REPORT_FILE, header=0)
+        # self.__data: DataFrame = self.__read_room_tool_report(cell)
+
+    def get_data_report(self):
+        return self.__data_room_tool_report
 
     def __read_room_tool_report(self, cell: str):
         data: DataFrame = read_csv(self.__ROOM_TOOL_REPORT_FILE, header=0)
+
+        # Select cell from dataset:
+        cell_data: DataFrame = data.loc[(data[self.__MODEL] == cell[:-10])]
+
+
         # Workaround for selecting multiple reports from room tool
-        first_row: DataFrame = data.iloc[0]
-        print("RoomToolReader: Only first row is considered")
-        print("RoomToolReader: Cell matching is not available")
+        # first_row: DataFrame = data.iloc[0]
+        # print("RoomToolReader: Only first row is considered")
+        # print("RoomToolReader: Cell matching is not available")
         # Note: Please consider a name matching of cell names between SimSES and room tool
-        cell_data: DataFrame = data.loc[(data[self.__MODEL] == cell)]
-        return first_row
+        return cell_data
 
     def get_battery_scale(self) -> (int, int):
-        first_values_serial_parallel: str = self.__data[self.__CONFIGURATION]
-        serial: int = int(first_values_serial_parallel.partition("s")[0])
-        parallel: int = int(first_values_serial_parallel.partition("s")[2][0:-1])
+        # first_values_serial_parallel: str = self.__data[self.__CONFIGURATION]
+        # serial: int = int(first_values_serial_parallel.partition("s")[0])
+        # parallel: int = int(first_values_serial_parallel.partition("s")[2][0:-1])
+        serial = int(self.__data["Cells in series"])
+        parallel = int(self.__data["Cells in parallel"])
+
         return serial, parallel
 
+
     def get_energy(self) -> float:
         return float(self.__data[self.__ENERGY])
 
     def get_nominal_voltage(self) -> float:
-        return float(self.__data[self.__VOLTAGE_NOM])
+        return float(self.__data[self.__VOLTAGE_NOM_MODULE])
```

### Comparing `simses-1.3.2/simses/simulation/simbas/simbas.py` & `simses-1.3.3/simses/simulation/simbas/simbas.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,70 +1,99 @@
 from configparser import ConfigParser
 
 from simses.commons.config.generation.analysis import AnalysisConfigGenerator
 from simses.commons.config.generation.simulation import SimulationConfigGenerator
 from simses.commons.config.simulation.battery import BatteryConfig
 from simses.simulation.batch_processing import BatchProcessing
 from simses.simulation.simbas.room_tool_reader import RoomToolReader
+import os
+import copy
 
 
 class SimBAS(BatchProcessing):
 
     """
     This is the SimBAS example for BatchProcessing.
     """
 
-    __CELL_CONFIG_FILE: str = 'cell_config.csv'
     __CELL_EXT: str = '.xml'
 
     def __init__(self, use_room_tool: bool = True):
         super().__init__(do_simulation=True, do_analysis=True)
         self.__use_room_tool: bool = use_room_tool
 
     def _setup_config(self) -> dict:
-        # Example for config setup
+
+        # Use case:
+        #use_case = 'ecar'
+        # use_case = 'eboat'
+        use_case = 'hpc+bess'
+
+        if use_case == 'ecar':
+            config_file_name = 'simulation_SimBAS_Ecar'
+            room_tool_file = 'report_auto.csv'
+            ac_power: float = 105e3
+        elif use_case == 'eboat':
+            config_file_name = 'simulation_SimBAS_Eboot'
+            room_tool_file = 'report_boot.csv'
+            ac_power: float = 320000.0
+        elif use_case == 'hpc+bess':
+            config_file_name = 'simulation_SimBAS_HPC+BSS'
+            room_tool_file = 'report_ladesäule.csv'
+            ac_power: float = 320000.0
+
+
+        profile_path = os.getcwd() + '\Profiles'
+
         config_generator: SimulationConfigGenerator = SimulationConfigGenerator()
-        # example: loading default config as base (not necessary)
         config_generator.load_default_config()
-        config_generator.load_local_config()
-        # defining parameters
-        capacity: float = 22000.0
-        ac_power: float = 105000.0
-        voltage_ic: float = 300.0
+        config_generator.load_specific_config(config_file_name)
+
+        # Set profile direction
+        config_generator.set_profile_direction(profile_path)
+
         # generating config options
         config_generator.clear_storage_technology()
-        dcdc_1: str = config_generator.add_fix_efficiency_dcdc(efficiency=0.98)
-        acdc_1: str = config_generator.add_fix_efficiency_acdc()
+        dcdc_1: str = config_generator.add_fix_efficiency_dcdc(1.0)
+        acdc_1: str = config_generator.add_no_loss_acdc()
         housing_1: str = config_generator.add_no_housing()
         hvac_1: str = config_generator.add_no_hvac()
         # generating storage systems
         config_generator.clear_storage_system_ac()
         config_generator.clear_storage_system_dc()
         # setting up multiple configurations with manual naming of simulations
-        cell_config: [[str]] = self.__read_cell_config(self.__CELL_CONFIG_FILE)
+
         config_set: dict = dict()
         count: int = 0
-        for cells in cell_config:
+
+        room_tool_reader: RoomToolReader = RoomToolReader(room_tool_file)
+        room_tool_entries = room_tool_reader.get_data_report()
+        for current_number in range(len(room_tool_entries)):
+
+            cell = room_tool_entries["Model"][current_number]
             serial, parallel = 1, 1
-            config_generator.clear_storage_system_dc()
-            config_generator.clear_storage_technology()
-            for cell in cells:
-                cell_type: str = 'IseaCellType;' + cell #+ self.__CELL_EXT
-                if self.__use_room_tool:
-                    room_tool_reader: RoomToolReader = RoomToolReader(cell=cell)
-                    serial, parallel = room_tool_reader.get_battery_scale()
-                    # print(serial, parallel)
-                    capacity = room_tool_reader.get_energy()
-                    voltage_ic = room_tool_reader.get_nominal_voltage()
-                storage = config_generator.add_lithium_ion_battery(capacity=capacity, cell_type=cell_type)
-                ac_system_1: str = config_generator.add_storage_system_ac(ac_power, voltage_ic, acdc_1, housing_1,
+            current_config_generator = copy.deepcopy(config_generator)
+
+            cell_type: str = 'IseaCellType;' + cell + '_00001'# + self.__CELL_EXT
+            # serial, parallel = room_tool_reader.get_battery_scale()
+            serial = int(room_tool_entries["Cells in series"][current_number])
+            parallel = int(room_tool_entries["Cells in parallel"][current_number])
+            energy = int(room_tool_entries["Energy (Wh)"][current_number])
+            voltage_ic = int(room_tool_entries["Nom. module voltage (V)"][current_number])
+
+            # room_tool_reader: RoomToolReader = RoomToolReader(room_tool_file, cell=cell)
+            # print(serial, parallel)
+            # capacity = room_tool_reader.get_energy()
+            # voltage_ic = room_tool_reader.get_nominal_voltage()
+            storage = current_config_generator.add_lithium_ion_battery(capacity=energy, cell_type=cell_type)
+            ac_system_1: str = current_config_generator.add_storage_system_ac(ac_power, voltage_ic, acdc_1, housing_1,
                                                                           hvac_1)
-                config_generator.add_storage_system_dc(ac_system_1, dcdc_1, storage)
+            current_config_generator.add_storage_system_dc(ac_system_1, dcdc_1, storage)
             count += 1
-            config: ConfigParser = config_generator.get_config()
+            config: ConfigParser = current_config_generator.get_config()
             # Attention: SimSES can only handle ONE serial/parallel config for ALL batteries
             # config.add_section('BATTERY')
             config.set(BatteryConfig.SECTION, BatteryConfig.CELL_SERIAL_SCALE, str(serial))
             config.set(BatteryConfig.SECTION, BatteryConfig.CELL_PARALLEL_SCALE, str(parallel))
             config_set['storage_' + str(count)] = config
             # for section in config.sections():
             #     print(section)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `simses-1.3.2/simses/simulation/simulator.py` & `simses-1.3.3/simses/system/storage_system_ac.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,249 +1,207 @@
-import os
-import sys
-import time
-from configparser import ConfigParser
-from math import floor
-from multiprocessing import Queue
-from queue import Full
-
-from simses.commons.config.abstract_config import Config
-from simses.commons.config.data.data_config import DataConfig
-from simses.commons.config.simulation.general import GeneralSimulationConfig
-from simses.commons.console_printer import ConsolePrinter
-from simses.commons.data.csv_data_handler import CSVDataHandler
-from simses.commons.data.no_data_handler import NoDataHandler
+from simses.system.housing.forty_ft_container import FortyFtContainer
+from simses.system.housing.twenty_ft_container import TwentyFtContainer
+from simses.commons.data.data_handler import DataHandler
 from simses.commons.error import EndOfLifeError
-from simses.commons.log import Logger
+from simses.commons.state.abstract_state import State
 from simses.commons.state.parameters import SystemParameters
 from simses.commons.state.system import SystemState
-from simses.commons.utils.utilities import format_float
-from simses.logic.energy_management.energy_management_system import EnergyManagement
-from simses.system.storage_circuit import StorageCircuit
+from simses.logic.power_distribution.power_distributor import PowerDistributor
+from simses.system.auxiliary.auxiliary import Auxiliary
+from simses.system.dc_coupling.dc_coupler import DcCoupling
+from simses.system.housing.abstract_housing import Housing
+from simses.system.power_electronics.electronics import PowerElectronics
+from simses.system.storage_system_dc import StorageSystemDC
+from simses.system.thermal.model.system_thermal_model import SystemThermalModel
 
 
-class StorageSimulation:
-
+class StorageSystemAC:
     """
-    StorageSimulation constructs the the storage systems and energy management system in order to execute the simulation.
-    In the run() method the timestamp for the simulation is advanced as configured. Alternatively, simulation is included
-    in another framework advancing timestamps itself, e.g. run_one_step() or evaluate_multiple_steps(). StorageSimulation
-    also provided information of the current status of the simulation to the user.
+    AC storage system class manages all connections within the AC storage system. Connections are power electronics,
+    further DC couplings (load/generation), housing, thermal model, auxiliaries, DC storage systems and its power
+    distribution logic. DC couplings are handled as an interference and tried to be primarily fed by storage system
+    power.
     """
 
-    def __init__(self, path: str, config: ConfigParser, printer_queue: Queue):
+    def __init__(self, state: SystemState, data_export: DataHandler, system_thermal_model: SystemThermalModel,
+                 power_electronics: PowerElectronics, storage_systems: [StorageSystemDC], dc_couplings: [DcCoupling]
+                 , housing: Housing, power_distributor: PowerDistributor):
+        self.__data_export = data_export
+        self.__system_state: SystemState = state
+        self.__system_id: int = int(self.__system_state.get(SystemState.SYSTEM_AC_ID))
+        self.__power_electronics: PowerElectronics = power_electronics
+        self.__acdc_converter: str = self.__power_electronics.acdc_converter_type
+        self.__system_thermal_model: SystemThermalModel = system_thermal_model
+        self.__storage_systems: [StorageSystemDC] = storage_systems
+        self.__dc_couplings: [DcCoupling] = dc_couplings
+        self.__auxiliaries: [Auxiliary] = list()
+        self.__auxiliaries.extend(self.__system_thermal_model.get_auxiliaries())
+        self.__auxiliaries.extend(self.__power_electronics.get_auxiliaries())
+        self.__housing = housing
+        for storage_system in self.__storage_systems:
+            self.__auxiliaries.extend(storage_system.get_auxiliaries())
+            self.__housing.add_component_volume(storage_system.volume)
+        for dc_coupling in self.__dc_couplings:
+            self.__auxiliaries.extend(dc_coupling.get_auxiliaries())
+        self.__system_state = self.__get_current_state()
+        self.__data_export.transfer_data(self.__system_state.to_export())  # initial timestep
+        self.__power_distributor: PowerDistributor = power_distributor
+        self.__housing.add_component_volume(self.__power_electronics.volume)
+        self.__system_thermal_model.update_air_parameters()
+
+    def update(self, power: float, time: float) -> None:
         """
-        Constructor of StorageSimulation
+        Function to update the states of an AC storage system
 
         Parameters
         ----------
-        path :
-            path to result folder
-        config :
-            Optional configs taken into account overwriting values from provided config file
-        printer_queue :
-            Optional queue for concurrent simulation process for providing progress status of simulations
-        """
-        self.__path = path
-        self.__log = Logger(type(self).__name__)
-        # Only instantiated in order write data config to results folder, maybe this way should be improved
-        self.__data_config: Config = DataConfig(None, None)
-        self.__config = GeneralSimulationConfig(config)
-        if self.__config.export_data:
-            self.__data_export = CSVDataHandler(path, self.__config)
-        else:
-            self.__data_export = NoDataHandler()
-        self.__energy_management: EnergyManagement = EnergyManagement(self.__data_export, config)
-        self.__storage_system = StorageCircuit(self.__data_export, config)
-        self.__name: str = os.path.basename(os.path.dirname(self.__path))
-        self.__printer_queue: Queue = printer_queue
-        self.__send_register_signal()
-        self.__max_loop = self.__config.loop
-        self.__start = self.__config.start
-        self.__end = self.__config.end
-        self.__timestep = self.__config.timestep  # sec
-        # duration to the last executed time step
-        self.__duration = floor((self.__end - self.__start) / self.__timestep) * self.__timestep
-        self.__timesteps_per_hour = 3600 / self.__timestep
-        system_parameters: SystemParameters = SystemParameters()
-        system_parameters.set_all(self.__storage_system.get_system_parameters())
-        system_parameters.write_parameters_to(path)
-
-    def run(self) -> None:
-        """
-        Executes simulation
+        power : ac target power (from energy management system)
+        time : current simulation time
 
         Returns
         -------
 
         """
-        self.__log.info('start')
-        sim_start = time.time()
-        ts_performance = []
-        try:
-            loop = 0
-            ts = self.__start
-            while loop < self.__max_loop:
-                self.__log.info('Loop: ' + str(loop))
-                ts_adapted = loop * self.__duration
-                while ts <= (ts_adapted + self.__end) - self.__timestep:
-                    ts_before = time.time()
-                    ts += self.__timestep
-                    self.run_one_step(ts, ts_adapted)
-                    ts_performance.append(time.time() - ts_before)
-                    self.__print_progress(ts)
-                loop += 1
-                if loop < self.__max_loop:
-                    ts_adapted = loop * self.__duration
-                    self.__energy_management.close()
-                    self.__energy_management: EnergyManagement = self.__energy_management.create_instance()
-                    self.reset_profiles(ts_adapted)
-        except EndOfLifeError as err:
-            self.__log.error(err)
-        finally:
-            self.close()
-            self.__print_end(ts_performance, sim_start)
-
-    def __print_progress(self, tstmp: float) -> None:
-        progress = (tstmp - self.__start) / (self.__duration * self.__max_loop) * 100
-        line: str = '|%-20s| ' % ('#' * round(progress / 5)) + format_float(progress, 1) + '%'
-        output: dict = {self.__name: line}
-        if self.__printer_queue is None:
-            sys.stdout.write('\r' + str(output))
-            sys.stdout.flush()
-        self.__put_to_queue(output)
-
-    def __put_to_queue(self, output: dict, blocking: bool = False) -> None:
-        if self.__printer_queue is not None:
+        state = self.__system_state
+        state.ac_power = power
+        # TODO Aux losses are calculated from last timestep. How to implement aux losses for current timestep?
+        state.aux_losses = 0
+        state.dc_power_additional = 0
+        for aux in self.__auxiliaries:  # type: Auxiliary
+            aux.update(time, state)
+        for dc in self.__dc_couplings:  # type: DcCoupling
+            dc.update(time, state)
+        self.__power_electronics.update(time, state)
+
+        states: [State] = list()
+        for system in self.__storage_systems:  # type: StorageSystemDC
+            states.append(system.state)
+
+        # self.__system_thermal_model.calculate_temperature(time, state, states)
+
+        self.__power_distributor.set(time, states, power)
+
+        total_dc_power: float = state.dc_power_intermediate_circuit + state.dc_power_additional
+        all_systems_ok: bool = True
+        err_msg: str = ''
+        for system in self.__storage_systems:  # type: StorageSystemDC
+            # TODO how to decide whether to store additional dc load or generation? (MM)
+            local_power: float = self.__power_distributor.get_power_for(total_dc_power, system.state)
             try:
-                if blocking:
-                    self.__printer_queue.put(output)
-                else:
-                    self.__printer_queue.put_nowait(output)
-            except Full:
-                return
-
-    def __send_stop_signal(self) -> None:
-        self.__put_to_queue({self.__name: ConsolePrinter.STOP_SIGNAL}, blocking=True)
-
-    def __send_register_signal(self) -> None:
-        self.__put_to_queue({self.__name: ConsolePrinter.REGISTER_SIGNAL}, blocking=True)
-
-    def __print_end(self, ts_performance: list, sim_start: float) -> None:
-        try:
-            sim_end = time.time()
-            duration: str = format_float(sim_end - sim_start)
-            duration_per_step: str = format_float(sum(ts_performance) * 1000 / len(ts_performance))
-            self.__log.info('100.0% done. Duration in sec: ' + duration)
-            self.__log.info('Duration per step in ms:      ' + duration_per_step)
-            if self.__printer_queue is None:
-                print('\r[' + self.__name + ': |%-20s| ' % ('#' * 20) + '100.0%]')
-                print('          Duration in s: ' + duration)
-                print('Duration per step in ms: ' + duration_per_step)
-        except ZeroDivisionError:
-            self.__log.warn('No performance indicators could be calculated.')
+                system.update(time, local_power)
+            except EndOfLifeError as err:
+                all_systems_ok = False
+                err_msg = str(err)
+        for system in self.__storage_systems:  # type: StorageSystemDC
+            system.wait()
+        state.time = time
+        self.__system_state = self.__get_current_state()
+        # Make sure to run the temperature model after running the DC System to represent ACDC losses for corner cases
+        # of SOC=0 and SOC=1 correctly
+        self.__system_thermal_model.calculate_temperature(time, self.__system_state, states)
+        self.__data_export.transfer_data(self.__system_state.to_export())
+        if not all_systems_ok:
+            raise EndOfLifeError(err_msg)
 
-    def run_one_step(self, ts: float, ts_adapted: float = 0, power: float = None, power_dist: [float] = None) -> None:
+    def __get_current_state(self) -> SystemState:
         """
-        Advances simulation for one step. Results can be obtained via state property.
+        Calculation of current system state
 
-        Parameters
-        ----------
-        ts :
-            next timestamp in s
-        ts_adapted :
-            timestamp adaption for looping simulations multiple times (should only be used with stand alone SimSES)
-        power :
-            next power transfered to storage system in W, if None power is taken from configured energy management
-        power_dist :
-            next power distribution in W for every AC system as a list. If None, power is taken from power distributor classes.
         Returns
         -------
-
-        """
-        if power_dist is None:
-            power_dist = []
-        state = self.__storage_system.state
-        if not self.__data_export.is_alive():
-            self.__data_export.start()
-        self.__data_export.transfer_data(state.to_export())
-        if power is None:
-            power = self.__energy_management.next(ts - ts_adapted, state)
-        try:
-            self.__storage_system.update(ts, power, power_dist)
-        finally:
-            self.__energy_management.export(ts)
-
-    def evaluate_multiple_steps(self, start: float, timestep: float, power: list) -> [SystemState]:
+        SystemState:
+            Current state of system
         """
-        Runs multiple steps of the simulation with the given start time, timestep and power list.
-        If no power list is provided, the simulation will not be advanced.
-
-        Parameters
-        ----------
-        start :
-            start time in s
-        timestep :
-            timestep in s
-        power :
-            list of power for each timestep in W
-
-        Returns
-        ----------
-        list:
-            Returns a list of system states for each timestep
+        states = list()
+        for system in self.__storage_systems:  # type: StorageSystemDC
+            states.append(system.state)
+        system_state: SystemState = SystemState.sum_parallel(states)
+        system_state.set(SystemState.SYSTEM_AC_ID, self.__system_id)
+        system_state.set(SystemState.SYSTEM_DC_ID, 0)
+        system_state.time = self.__system_state.time
+        system_state.temperature = self.__system_thermal_model.get_temperature()
+        if isinstance(self.__housing, (TwentyFtContainer, FortyFtContainer)):
+            system_state.ol_temperature = self.__system_thermal_model.get_ol_temperature()
+            system_state.il_temperature = self.__system_thermal_model.get_il_temperature()
+        system_state.ambient_temperature = self.__system_thermal_model.get_ambient_temperature()
+        system_state.solar_thermal_load = self.__system_thermal_model.get_solar_irradiation_thermal_load()
+        system_state.hvac_thermal_power = self.__system_thermal_model.get_hvac_thermal_power()
+        system_state.ac_power = self.__system_state.ac_power
+        system_state.pe_losses = self.__system_state.pe_losses
+        system_state.aux_losses = self.__system_state.aux_losses
+        system_state.dc_power_additional = self.__system_state.dc_power_additional
+        system_state.max_charge_power = min(system_state.max_charge_power, self.__power_electronics.max_power)
+        system_state.max_discharge_power = min(system_state.max_discharge_power, self.__power_electronics.max_power)
+        self.__power_electronics.update_ac_power_from(system_state)
+        # Include power electronic fulfillment after reverse power calculation
+        if abs(system_state.ac_power) < max(system_state.max_charge_power, system_state.max_discharge_power) * 0.01:
+            system_state.ac_fulfillment = 1
+        else:
+            system_state.ac_fulfillment = system_state.ac_power_delivered / system_state.ac_power
+        return system_state
 
-        """
-        res: [SystemState] = list()
-        ts = start
-        for pow in power:
-            self.run_one_step(ts=ts, power=pow)
-            res.append(self.state)
-            ts += timestep
-        return res
+    def get_system_parameters(self) -> dict:
+        parameters: dict = dict()
+        parameters[SystemParameters.SYSTEM] = type(self).__name__
+        parameters[SystemParameters.ID] = str(self.__system_id)
+        parameters[SystemParameters.POWER_DISTRIBUTION] = type(self.__power_distributor).__name__
+        parameters[SystemParameters.CONTAINER_NUMBER] = self.__housing.get_number_of_containers()
+        parameters[SystemParameters.CONTAINER_TYPE] = type(self.__housing).__name__
+        parameters[SystemParameters.ACDC_CONVERTER] = self.__acdc_converter
+        auxiliaries: list = list()
+        for aux in self.__auxiliaries:  # type: Auxiliary
+            auxiliaries.append(type(aux).__name__)
+        subsystems: list = list()
+        for system in self.__storage_systems:  # type: StorageSystemDC
+            subsystems.append(system.get_system_parameters())
+        parameters[SystemParameters.AUXILIARIES] = auxiliaries
+        parameters[SystemParameters.SUBSYSTEM] = subsystems
+        return parameters
 
     @property
     def state(self) -> SystemState:
         """
+        Returns current system state
 
         Returns
         -------
         SystemState:
-            current state of top level system
+            State of the ac system
+
         """
-        return self.__storage_system.state
+        return self.__system_state
 
     @property
-    def ac_system_states(self) -> [SystemState]:
-        """
+    def max_power(self) -> float:
+        return self.__power_electronics.max_power
 
-        Returns
-        -------
-        SystemState:
-            list of current states for all AC systems
-        """
-        return self.__storage_system.ac_system_states
+    @property
+    def system_id(self) -> int:
+        return self.__system_id
 
     def reset_profiles(self, ts_adapted: float) -> None:
         """
         Enables looping of the simulation beyond the original length of the time series for the AmbientThermalModel and
         SolarIrradiationModel
         """
-        self.__storage_system.reset_profiles(ts_adapted)
+        self.__system_thermal_model.reset_profiles(ts_adapted)
 
     def close(self) -> None:
         """
-        Closing all resources of simulation
+        Closing all open resources in AC storage system
+
+        Parameters
+        ----------
 
         Returns
         -------
 
         """
-        self.__log.info('closing')
-        self.__data_export.transfer_data(self.__storage_system.state.to_export())
-        self.__send_stop_signal()
-        self.__config.write_config_to(self.__path)
-        self.__data_config.write_config_to(self.__path)
-        self.__log.close()
-        self.__data_export.close()
-        self.__energy_management.close()
-        self.__storage_system.close()
+        self.__power_electronics.close()
+        self.__system_thermal_model.close()
+        self.__power_distributor.close()
+        for storage_system in self.__storage_systems:  # type: StorageSystemDC
+            storage_system.close()
+        for aux in self.__auxiliaries:  # type: Auxiliary
+            aux.close()
+        for dc_coupling in self.__dc_couplings:  # type: DcCoupling
+            dc_coupling.close()
```

### Comparing `simses-1.3.2/simses/simulation.defaults.ini` & `simses-1.3.3/simses/simulation.defaults.ini`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 ;           and keeps SOC as low as possible in order to reduce calendar aging.
 ;           MAX_POWER: This value determines the peak-shaving limit for the whole year in W
 ;       FrequencyContainmentReserve: A strategy to participate in the FCR market (German regulations) without recharge
 ;           POWER_FCR: How much power should be offered to the FCR market in W?
 ;           SOC_SET: Target SOC for FCR simulations in p.u.
 ;           FCR_RESERVE: Full power reserve for alert state in h, default: 0.25 (15 minute criterion)
 ;       FcrIdmRechargeStacked: A multi-use to participate in the FCR market (German regulations) with IDM recharge
+;           POWER_IDM: How much power can be used to participate in the Intraday market in W?
 ;       ElectricVehicle: A strategy to simulate the load on EV batteries while driving and recharge using a power
 ;                        profile and a binary profile.
 ;           EV_CHARGING_STRATEGY: Decide on the charging strategy. Currently available: Uncontrolled
 ;           MAX_POWER: This value determines the maximal AC charging power in W
 ;       ElectricVehicleSOC: A strategy to simulate the load on EV batteries while driving and recharge using an SOC
 ;                           profile and a binary profile.
 ;           EV_CHARGING_STRATEGY: Decide on the charging strategy. Currently available: Original, Uncontrolled,
@@ -156,20 +157,16 @@
 HOUSING =
     no_housing,NoHousing
     small_container,TwentyFtContainer,False,0,0.15,0.2
 
 ; Configuration of the HVAC system:
 ; Format: HVAC system name, HVAC system type,
 ; optional: heating/cooling power in W, set-point temperature (in °C),
-; (Required for FixCOPHeatingVentilationAirConditioning and FixCOPHeatingVentilationAirConditioningPIDControl)
-; optional: Kp_coefficient, Ki_coefficient, Kd_coefficient
-; (Required for FixCOPHeatingVentilationAirConditioningPIDControl)
 ;    no_hvac,NoHeatingVentilationAirConditioning
 ;    constant_hvac,FixCOPHeatingVentilationAirConditioning,3000,25
-;    constant_hvac,FixCOPHeatingVentilationAirConditioningPIDControl,80000,21,600,1,0
 HVAC =
     no_hvac,NoHeatingVentilationAirConditioning
     constant_hvac,FixCOPHeatingVentilationAirConditioning,3000,25
 
 ; Configuration of the DC storage system. Every AC system must have at least 1 DC system
 ; Format: AC-system name, DCDC converter name, storage technology name
 ; Some examples are provided here:
@@ -217,15 +214,15 @@
 ; Configuration of power distributor logic between AC systems as well as between DC systems
 ; Options: EqualPowerDistributor, SocBasedPowerDistributor
 POWER_DISTRIBUTOR_AC = EqualPowerDistributor
 POWER_DISTRIBUTOR_DC = EqualPowerDistributor
 
 ; Configuration of ambient temperature for the simulation
 ;   ConstantAmbientTemperature,UserDefinedTemperatureValue (in °C): default value 25 °C, if unspecified
-;   LocationAmbientTemperature (Standard = Berlin) Change Location in data.ini
+;   LocationAmbientTemperature (Standard = Berlin)
 ;   Specify profile filename in field AMBIENT_TEMPERATURE_PROFILE, values in °C (no timestamps, profiles start from January)
 ;   UserBatteryTemperatureProfile, allows users to input their own temperature test data to calculate battery degradation
 ;   Specify profile filename in field BATTERY_TEMPERATURE_PROFILE, values in °C (no timestamps, profiles start from January)
 AMBIENT_TEMPERATURE_MODEL = ConstantAmbientTemperature,25
 
 ; Configuration of solar irradiation model for the simulation
 ;   NoSolarIrradiationModel
```

### Comparing `simses-1.3.2/simses/system/auxiliary/auxiliary.py` & `simses-1.3.3/simses/system/auxiliary/auxiliary.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/auxiliary/compression/compressor.py` & `simses-1.3.3/simses/system/auxiliary/compression/compressor.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/auxiliary/compression/hydrogen_isentrop.py` & `simses-1.3.3/simses/system/auxiliary/compression/hydrogen_isentrop.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/auxiliary/gas_drying/gas_dryer.py` & `simses-1.3.3/simses/system/auxiliary/gas_drying/gas_dryer.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/auxiliary/gas_drying/hydrogen.py` & `simses-1.3.3/simses/system/auxiliary/gas_drying/hydrogen.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/auxiliary/heating_ventilation_air_conditioning/fix_cop_hvac.py` & `simses-1.3.3/simses/system/auxiliary/heating_ventilation_air_conditioning/fix_cop_hvac.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,14 @@
         self.__seer: float = 6.31
 
         # Initialize variables
         self.__electric_power: float = 0  # W
         self.__thermal_power: float = 0  # W
         self.__air_mass: float = 0  # kg
         self.__air_specific_heat: float = 0  # J/kgK
-        self.__supply_air_temperature = 288.15  # K
 
         # Create the Fan
         self.__fan = Fan()
 
         # Create Thermal Management
         # self.__thermal_management = OnOffController(self.__set_point_temperature, self.__max_thermal_power)
         self.__thermal_management = PIDController(self.__set_point_temperature, self.__max_thermal_power)
```

### Comparing `simses-1.3.2/simses/system/auxiliary/heating_ventilation_air_conditioning/hvac.py` & `simses-1.3.3/simses/system/auxiliary/heating_ventilation_air_conditioning/hvac.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/auxiliary/heating_ventilation_air_conditioning/no_hvac.py` & `simses-1.3.3/simses/system/auxiliary/heating_ventilation_air_conditioning/no_hvac.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/auxiliary/pump/abstract_pump.py` & `simses-1.3.3/simses/system/auxiliary/pump/abstract_pump.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/auxiliary/pump/fixeta_centrifugal.py` & `simses-1.3.3/simses/system/auxiliary/pump/fixeta_centrifugal.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/auxiliary/pump/scalable_variable_eta_centrifugal.py` & `simses-1.3.3/simses/system/auxiliary/pump/scalable_variable_eta_centrifugal.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/auxiliary/pump/variable_eta_centrifugal.py` & `simses-1.3.3/simses/system/auxiliary/pump/variable_eta_centrifugal.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/auxiliary/water_heating/water_heater.py` & `simses-1.3.3/simses/system/auxiliary/water_heating/water_heater.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/dc_coupling/bus_charging_profile.py` & `simses-1.3.3/simses/system/dc_coupling/bus_charging_profile.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/dc_coupling/dc_coupler.py` & `simses-1.3.3/simses/system/dc_coupling/dc_coupler.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/dc_coupling/generation/dc_generation.py` & `simses-1.3.3/simses/system/dc_coupling/generation/dc_generation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/dc_coupling/generation/pv_dc_generation.py` & `simses-1.3.3/simses/system/dc_coupling/generation/pv_dc_generation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/dc_coupling/load/dc_bus_charging_fixed.py` & `simses-1.3.3/simses/system/dc_coupling/load/dc_bus_charging_fixed.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/dc_coupling/load/dc_bus_charging_profile.py` & `simses-1.3.3/simses/system/dc_coupling/load/dc_bus_charging_profile.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/dc_coupling/load/dc_bus_charging_random.py` & `simses-1.3.3/simses/system/dc_coupling/load/dc_bus_charging_random.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/dc_coupling/load/dc_load.py` & `simses-1.3.3/simses/system/dc_coupling/load/dc_load.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/dc_coupling/load/dc_radio_ups_load.py` & `simses-1.3.3/simses/system/dc_coupling/load/dc_radio_ups_load.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/dc_coupling/usp_dc_coupling.py` & `simses-1.3.3/simses/system/dc_coupling/usp_dc_coupling.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/factory.py` & `simses-1.3.3/simses/system/factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,14 @@
 from simses.logic.power_distribution.efficient import EfficientPowerDistributor
 from simses.logic.power_distribution.equal import EqualPowerDistributor
 from simses.logic.power_distribution.power_distributor import PowerDistributor
 from simses.logic.power_distribution.soc import SocBasedPowerDistributor
 from simses.logic.power_distribution.technology import TechnologyBasedPowerDistributor
 from simses.system.auxiliary.heating_ventilation_air_conditioning.fix_cop_hvac import \
     FixCOPHeatingVentilationAirConditioning
-from simses.system.auxiliary.heating_ventilation_air_conditioning.fix_cop_hvac_pid_control import \
-    FixCOPHeatingVentilationAirConditioningPIDControl
 from simses.system.auxiliary.heating_ventilation_air_conditioning.hvac import HeatingVentilationAirConditioning
 from simses.system.auxiliary.heating_ventilation_air_conditioning.no_hvac import NoHeatingVentilationAirConditioning
 from simses.system.dc_coupling.bus_charging_dc_coupling import BusChargingDcCoupling
 from simses.system.dc_coupling.bus_charging_profile import BusChargingProfileDcCoupling
 from simses.system.dc_coupling.dc_coupler import DcCoupling
 from simses.system.dc_coupling.no_dc_coupling import NoDcCoupling
 from simses.system.dc_coupling.usp_dc_coupling import USPDCCoupling
@@ -61,15 +59,15 @@
 from simses.technology import hydrogen
 from simses.technology import lithium_ion, redox_flow
 from simses.technology.hydrogen.system import Hydrogen
 from simses.technology.lithium_ion.battery import LithiumIonBattery
 from simses.technology.lithium_ion.circuit import BatteryCircuit
 from simses.technology.redox_flow.system import RedoxFlow
 from simses.technology.storage import StorageTechnology
-
+from simses.commons.config.simulation.energy_management import EnergyManagementConfig
 
 class StorageSystemFactory:
     """
     The StorageSystemFactory instantiates all necessary and configured objects for AC and DC storage systems.
     """
 
     __lithium_ion_name: str = lithium_ion.__name__.split('.')[-1]
@@ -81,14 +79,15 @@
         self.__simulation_config: ConfigParser = config
         self.__system_config: StorageSystemConfig = StorageSystemConfig(config)
         self.__general_config: GeneralSimulationConfig = GeneralSimulationConfig(config)
         self.__power_electronics_data_config: PowerElectronicsConfig = PowerElectronicsConfig()
         self.__profile_config: ProfileConfig = ProfileConfig(config)
         self.__config_battery: BatteryConfig = BatteryConfig(config)
         self.__energy_management_data_config = EnergyManagementDataConfig()
+        self.__energy_management_config = EnergyManagementConfig(config)
 
     def create_acdc_converter(self, converter: str, max_power: float,
                               intermediate_cicuit_voltage: float) -> AcDcConverter:
         converter_configuration: dict = self.__system_config.acdc_converter
         converter_type = converter_configuration[converter][StorageSystemConfig.ACDC_CONVERTER_TYPE]
         acdc_converter: AcDcConverter = None
         if converter_type == NoLossAcDcConverter.__name__:
@@ -291,21 +290,14 @@
             elif hvac_type == FixCOPHeatingVentilationAirConditioning.__name__:
                 if not isinstance(housing, supported_housing):
                     raise Exception('HVAC model ' + hvac_type + ' is incompatible with ' + housing.__class__.__name__
                                     + '. Please select ' + NoHeatingVentilationAirConditioning.__name__
                                     + ', or select a supported housing model: ' + str(supported_housing_names))
                 self.__log.debug('Creating HVAC model ' + FixCOPHeatingVentilationAirConditioning.__class__.__name__)
                 return FixCOPHeatingVentilationAirConditioning(hvac_configuration[hvac])
-            elif hvac_type == FixCOPHeatingVentilationAirConditioningPIDControl.__name__:
-                if not isinstance(housing, supported_housing):
-                    raise Exception('HVAC model ' + hvac_type + ' is incompatible with ' + housing.__class__.__name__
-                                    + '. Please select ' + NoHeatingVentilationAirConditioning.__name__
-                                    + ', or select a supported housing model: ' + str(supported_housing_names))
-                self.__log.debug('Creating HVAC model ' + FixCOPHeatingVentilationAirConditioningPIDControl.__class__.__name__)
-                return FixCOPHeatingVentilationAirConditioningPIDControl(hvac_configuration[hvac])
             else:
                 options: [str] = list()
                 options.append(NoHeatingVentilationAirConditioning.__name__)
                 options.append(FixCOPHeatingVentilationAirConditioning.__name__)
                 raise Exception('HVAC model ' + hvac_type + ' is unknown. '
                                                             'Following options are available: ' + str(options))
         else:
```

### Comparing `simses-1.3.2/simses/system/housing/abstract_housing.py` & `simses-1.3.3/simses/system/housing/abstract_housing.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/housing/forty_ft_container.py` & `simses-1.3.3/simses/system/housing/forty_ft_container.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/housing/layer.py` & `simses-1.3.3/simses/system/housing/layer.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/housing/twenty_ft_container.py` & `simses-1.3.3/simses/system/housing/twenty_ft_container.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/power_electronics/acdc_converter/abstract_acdc_converter.py` & `simses-1.3.3/simses/system/power_electronics/acdc_converter/abstract_acdc_converter.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/power_electronics/acdc_converter/bonfiglioli.py` & `simses-1.3.3/simses/system/power_electronics/acdc_converter/bonfiglioli.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/power_electronics/acdc_converter/fix_efficiency.py` & `simses-1.3.3/simses/system/power_electronics/acdc_converter/fix_efficiency.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/power_electronics/acdc_converter/notton.py` & `simses-1.3.3/simses/system/power_electronics/acdc_converter/notton.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/power_electronics/acdc_converter/notton_loss.py` & `simses-1.3.3/simses/system/power_electronics/acdc_converter/notton_loss.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/power_electronics/acdc_converter/rampinelli_fit.py` & `simses-1.3.3/simses/system/power_electronics/acdc_converter/rampinelli_fit.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/power_electronics/acdc_converter/sinamics.py` & `simses-1.3.3/simses/system/power_electronics/acdc_converter/sinamics.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/power_electronics/acdc_converter/stable.py` & `simses-1.3.3/simses/system/power_electronics/acdc_converter/stable.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/power_electronics/acdc_converter/stacked.py` & `simses-1.3.3/simses/system/power_electronics/acdc_converter/stacked.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/power_electronics/acdc_converter/sungrow.py` & `simses-1.3.3/simses/system/power_electronics/acdc_converter/sungrow.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/power_electronics/dcdc_converter/abstract_dcdc_converter.py` & `simses-1.3.3/simses/system/power_electronics/dcdc_converter/abstract_dcdc_converter.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/power_electronics/dcdc_converter/fix_efficiency.py` & `simses-1.3.3/simses/system/power_electronics/dcdc_converter/fix_efficiency.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/power_electronics/dcdc_converter/no_dcdc.py` & `simses-1.3.3/simses/system/power_electronics/dcdc_converter/no_dcdc.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/power_electronics/dcdc_converter/no_loss.py` & `simses-1.3.3/simses/system/power_electronics/dcdc_converter/no_loss.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/power_electronics/electronics.py` & `simses-1.3.3/simses/system/power_electronics/electronics.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/storage_circuit.py` & `simses-1.3.3/simses/system/storage_circuit.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         self.__power_distributor: PowerDistributor = factory.create_power_distributor_ac()
         factory.close()
 
     def update(self, time: float, power: float, power_dist: [float] = None) -> None:
         if power_dist is None:
             power_dist = []
         states: [State] = list()
-        for system in self.__storage_systems:
+        for system in self.__storage_systems:  # type: StorageSystemAC
             states.append(system.state)
         self.__power_distributor.set(time, states, power)
         end_of_life_reached: bool = False
         for i in range(0, len(self.__storage_systems)):
             if not power_dist:
                 local_power: float = self.__power_distributor.get_power_for(power, self.__storage_systems[i].state)
             else:
@@ -41,43 +41,43 @@
                 end_of_life_reached = True
         if end_of_life_reached:
             raise EndOfLifeError()
 
     @property
     def state(self) -> SystemState:
         system_states = list()
-        for storage in self.__storage_systems:
+        for storage in self.__storage_systems:  # type: StorageSystemAC
             system_states.append(storage.state)
         system_state: SystemState = SystemState.sum_parallel(system_states)
         system_state.set(SystemState.SYSTEM_AC_ID, 0)
         system_state.set(SystemState.SYSTEM_DC_ID, 0)
         return system_state
 
     @property
     def ac_system_states(self) -> [SystemState]:
         system_states = list()
-        for storage in self.__storage_systems:
+        for storage in self.__storage_systems:  # type: StorageSystemAC
             system_states.append(storage.state)
         return system_states
 
     def get_system_parameters(self) -> dict:
         parameters: dict = dict()
         subsystems: list = list()
-        for system in self.__storage_systems:
+        for system in self.__storage_systems:  # type: StorageSystemAC
             subsystems.append(system.get_system_parameters())
         parameters[SystemParameters.POWER_DISTRIBUTION] = type(self.__power_distributor).__name__
         parameters[SystemParameters.SUBSYSTEM] = subsystems
         return {SystemParameters.PARAMETERS: parameters}
 
     def reset_profiles(self, ts_adapted: float) -> None:
         """
         Enables looping of the simulation beyond the original length of the time series for the AmbientThermalModel and
         SolarIrradiationModel
         """
-        for system in self.__storage_systems:
+        for system in self.__storage_systems:  # type: StorageSystemAC
             system.reset_profiles(ts_adapted)
 
     def close(self) -> None:
         """Closing all resources in storage systems"""
         self.__power_distributor.close()
-        for storage in self.__storage_systems:
+        for storage in self.__storage_systems:  # type: StorageSystemAC
             storage.close()
```

### Comparing `simses-1.3.2/simses/system/storage_system_dc.py` & `simses-1.3.3/simses/system/storage_system_dc.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/test/test_acdc_converter.py` & `simses-1.3.3/simses/system/test/test_acdc_converter.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/test/test_constant_ambient_temperature.py` & `simses-1.3.3/simses/system/test/test_constant_ambient_temperature.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/test/test_fix_cop_hvac.py` & `simses-1.3.3/simses/system/test/test_fix_cop_hvac.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/test/test_location_ambient_temperature.py` & `simses-1.3.3/simses/system/test/test_location_ambient_temperature.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/test/test_location_ambient_temperature_profile_check.py` & `simses-1.3.3/simses/system/test/test_location_ambient_temperature_profile_check.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/test/test_location_solar_irradiation_model.py` & `simses-1.3.3/simses/system/test/test_location_solar_irradiation_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/test/test_location_solar_irradiation_model_profile_check.py` & `simses-1.3.3/simses/system/test/test_location_solar_irradiation_model_profile_check.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/test/test_notton_acdc_converter.py` & `simses-1.3.3/simses/system/test/test_notton_acdc_converter.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/thermal/ambient/ambient_thermal_model.py` & `simses-1.3.3/simses/system/thermal/ambient/ambient_thermal_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/thermal/ambient/constant_temperature.py` & `simses-1.3.3/simses/system/thermal/ambient/constant_temperature.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     def __init__(self, temperature: float = 25):
         """
         Constructor of ConstantAmbientTemperature
 
         Parameters
         ----------
         temperature :
-            temperature in centigrades, default: 25 °C
+            temperature in in °C, default: 25 °C
         """
         super().__init__()
         self.__temperature = 273.15 + temperature  # K
 
     def get_temperature(self, time) -> float:
         return self.__temperature
 
@@ -26,11 +26,12 @@
         return self.__temperature
 
     def create_instance(self) -> AmbientThermalModel:
         """
         reinstantiates the AmbientThermalModel
         :return: AmbientThermalModel
         """
-        return ConstantAmbientTemperature(self.__temperature)
+        temperature = self.__temperature - 273.15  # in °C
+        return ConstantAmbientTemperature(temperature)
 
     def close(self):
         pass
```

### Comparing `simses-1.3.2/simses/system/thermal/ambient/location_temperature.py` & `simses-1.3.3/simses/system/thermal/ambient/location_temperature.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/thermal/ambient/user_battery_temperature.py` & `simses-1.3.3/simses/system/thermal/ambient/user_battery_temperature.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/thermal/model/no_system_thermal_model.py` & `simses-1.3.3/simses/system/thermal/model/no_system_thermal_model.py`

 * *Files 17% similar despite different names*

```diff
@@ -63,7 +63,14 @@
         Enables looping of the simulation beyond the original length of the time series for the AmbientThermalModel and
         SolarIrradiationModel
         """
         pass
 
     def update_air_parameters(self):
         pass
+
+    def get_ol_temperature(self) -> float:
+        pass
+
+    def get_il_temperature(self) -> float:
+        pass
+
```

### Comparing `simses-1.3.2/simses/system/thermal/model/system_thermal_model.py` & `simses-1.3.3/simses/system/thermal/model/system_thermal_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,46 @@
         float
             system temperature in Kelvin
         """
 
         pass
 
     @abstractmethod
+    def get_ol_temperature(self) -> float:
+        """
+        Returns the current temperature of the outer layer of container
+
+        Parameters
+        -------
+
+        Returns
+        -------
+        float
+            temperature in Kelvin
+        """
+
+        pass
+
+    @abstractmethod
+    def get_il_temperature(self) -> float:
+        """
+        Returns the current temperature of the inner layer of container
+
+        Parameters
+        -------
+
+        Returns
+        -------
+        float
+            temperature in Kelvin
+        """
+
+        pass
+
+    @abstractmethod
     def get_ambient_temperature(self) -> float:
         """
         Returns the ambient temperature at the location
         """
 
         pass
```

### Comparing `simses-1.3.2/simses/system/thermal/model/zero_d_room_thermal_model.py` & `simses-1.3.3/simses/system/thermal/model/zero_d_room_thermal_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,16 +193,15 @@
 
                 # Differential equation for change in inner air temperature
                 d_by_dt_inner_air_temperature = 0.0
 
                 # Differential equation for change in converter temperature
                 d_by_dt_converter_temperature_ac_dc = (state.pe_losses - (
                         (variable_array[number_storage_technologies + 1] - variable_array[0])
-                        / self.__converter_ia_thermal_resistance)) / \
-                                                      self.__converter_thermal_capacity
+                        / self.__converter_ia_thermal_resistance)) / self.__converter_thermal_capacity
 
                 equation_rhs_array = [d_by_dt_inner_air_temperature] + d_by_dt_storage_technology_temperature + \
                                      [d_by_dt_converter_temperature_ac_dc]
                 return equation_rhs_array
 
             # time_interval is an array of times at which the equation get evaluated
             time_interval = [i for i in range(self.__t_eval_step, self.__calculation_time_step + self.__t_eval_step,
@@ -280,7 +279,19 @@
         self.__ambient_thermal_model: AmbientThermalModel = self.__ambient_thermal_model.create_instance()
 
     def close(self) -> None:
         """
         closes specified open resources
         """
         self.__ambient_thermal_model.close()
+
+    def get_ol_temperature(self) -> float:
+        """
+        Not applicable to this class
+        """
+        pass
+
+    def get_il_temperature(self) -> float:
+        """
+        Not applicable to this class
+        """
+        pass
```

### Comparing `simses-1.3.2/simses/system/thermal/model/zero_d_system_thermal_model.py` & `simses-1.3.3/simses/system/thermal/model/zero_d_system_thermal_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,17 +42,17 @@
         self.__ambient_thermal_model: AmbientThermalModel = ambient_thermal_model
         self.__solar_irradiation_model: SolarIrradiationModel = solar_irradiation_model
         self.__housing: Housing = housing
         self.__heating_cooling: HeatingVentilationAirConditioning = hvac
 
         # Auto-adjust thermal model calculation timestep
         if general_config.end - general_config.start >= 86400:  # Choose a larger calculation_time_step for faster performance
-            self.__calculation_time_step = 300
+            self.__calculation_time_step = 180
         else:
-            self.__calculation_time_step = 60
+            self.__calculation_time_step = 15
         if self.__calculation_time_step >= self.__sample_time:
             self.__calculation_time_step = int(self.__sample_time)
 
         if self.__sample_time % self.__calculation_time_step != 0:
             raise Exception(self.__name__ +
                             ': For simulations longer than a day, please set a simulation timestep '
                             'in multiples of 5 minutes, for shorter simulations, use a timestep in multiples of 1 minute.')
@@ -198,14 +198,18 @@
 
         calculated_time = 0
         radiation_power = self.__solar_irradiation_model.get_heat_load(time - self.__ts_adapted)
         self.__solar_irradiation_thermal_load = radiation_power
         hvac_electric_consumption = []
         thermal_power_hvac = []
 
+        pe_loss = state.pe_losses
+        dcdcloss = storage_system_dc_states[0].dc_power_loss
+        st_loss = storage_system_dc_states[0].storage_power_loss
+
         while calculated_time < self.__sample_time:
             calculated_time += self.__calculation_time_step
             thermal_power = self.__heating_cooling.get_thermal_power()
             thermal_power_hvac.append(thermal_power)
 
             def equation_rhs(t, variable_array):
                 """
@@ -230,19 +234,16 @@
                     d_by_dt_storage_technology_temperature.append(
                         ((storage_system_dc_state.storage_power_loss + storage_system_dc_state.dc_power_loss) -
                          (variable_array[index + 1] - variable_array[0]) /
                          self.__storage_technology_ia_thermal_resistance[index]) / \
                         self.__storage_technology_thermal_capacity[index])
 
                 # Differential equation for change in inner air temperature
-                d_by_dt_inner_air_temperature = (((variable_array[number_storage_technologies + 4] - variable_array[
-                    0]) / self.__inner_layer_air_thermal_resistance) +
-                                                 (sum(heat_flow_storage_technology_ia)) +
-                                                 ((variable_array[number_storage_technologies + 1] - variable_array[
-                                                     0]) / self.__converter_ia_thermal_resistance) - thermal_power) / self.__internal_air_thermal_capacity
+                d_by_dt_inner_air_temperature = (((variable_array[number_storage_technologies + 4] - variable_array[0]) / self.__inner_layer_air_thermal_resistance) + (sum(heat_flow_storage_technology_ia)) +
+                                                 ((variable_array[number_storage_technologies + 1] - variable_array[0]) / self.__converter_ia_thermal_resistance) - thermal_power) / self.__internal_air_thermal_capacity
 
                 # Differential equation for change in converter temperature
                 d_by_dt_converter_temperature_ac_dc = (state.pe_losses - (
                         (variable_array[number_storage_technologies + 1] - variable_array[0])
                         / self.__converter_ia_thermal_resistance)) / \
                                                       self.__converter_thermal_capacity
 
@@ -334,14 +335,28 @@
     def get_temperature(self) -> float:
         """
         returns internal air temperature in the container in K
         :return: __internal_air_temperature as float
         """
         return self.__internal_air_temperature
 
+    def get_ol_temperature(self) -> float:
+        """
+        returns outer layer temperature of the container in K
+        :return: __outer_layer_temperature as float
+        """
+        return self.__outer_layer_temperature
+
+    def get_il_temperature(self) -> float:
+        """
+        returns inner layer temperature of the container in K
+        :return: __inner_layer_temperature as float
+        """
+        return self.__inner_layer_temperature
+
     def get_ambient_temperature(self) -> float:
         """
         returns the ambient temperature at the location in K
         :return: __ambient_air_temperature as float
         """
         return self.__ambient_air_temperature
```

### Comparing `simses-1.3.2/simses/system/thermal/solar_irradiation/location.py` & `simses-1.3.3/simses/system/thermal/solar_irradiation/location.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/thermal/solar_irradiation/no_solar_irradiation.py` & `simses-1.3.3/simses/system/thermal/solar_irradiation/no_solar_irradiation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/system/thermal/solar_irradiation/solar_irradiation_model.py` & `simses-1.3.3/simses/system/thermal/solar_irradiation/solar_irradiation_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/control/management.py` & `simses-1.3.3/simses/technology/hydrogen/control/management.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/control/pressure/ideal_var_cathode.py` & `simses-1.3.3/simses/technology/hydrogen/control/pressure/ideal_var_cathode.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/control/pressure/no_pressure_controller.py` & `simses-1.3.3/simses/technology/hydrogen/control/pressure/no_pressure_controller.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/control/pressure/pressure_controller.py` & `simses-1.3.3/simses/technology/hydrogen/control/pressure/pressure_controller.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/control/thermal/ideal_var_flow.py` & `simses-1.3.3/simses/technology/hydrogen/control/thermal/ideal_var_flow.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/control/thermal/no_thermal_controller.py` & `simses-1.3.3/simses/technology/hydrogen/control/thermal/no_thermal_controller.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/control/thermal/thermal_controller.py` & `simses-1.3.3/simses/technology/hydrogen/control/thermal/thermal_controller.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/control/thermal/var_flow.py` & `simses-1.3.3/simses/technology/hydrogen/control/thermal/var_flow.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/electrolyzer/degradation/calendar/calendar_degradation.py` & `simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/calendar/calendar_degradation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/electrolyzer/degradation/calendar/no_calendar_degradation.py` & `simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/calendar/no_calendar_degradation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/electrolyzer/degradation/calendar/pem_analytic.py` & `simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/calendar/pem_analytic.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/electrolyzer/degradation/cyclic/cyclic_degradation.py` & `simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/cyclic/cyclic_degradation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/electrolyzer/degradation/cyclic/no_cyclic_degradation.py` & `simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/cyclic/no_cyclic_degradation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/electrolyzer/degradation/cyclic/pem_analytic.py` & `simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/cyclic/pem_analytic.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/electrolyzer/degradation/cyclic/pem_analytic_ptl_coating.py` & `simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/cyclic/pem_analytic_ptl_coating.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/electrolyzer/degradation/degradation_model.py` & `simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/degradation_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/electrolyzer/degradation/no_degradation.py` & `simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/no_degradation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/electrolyzer/degradation/pem_analytic.py` & `simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/pem_analytic.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/electrolyzer/degradation/pem_analytic_ptl_coating.py` & `simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/pem_analytic_ptl_coating.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/electrolyzer/factory.py` & `simses-1.3.3/simses/technology/hydrogen/electrolyzer/factory.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/electrolyzer/pressure/abstract_model.py` & `simses-1.3.3/simses/technology/hydrogen/electrolyzer/pressure/abstract_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/electrolyzer/pressure/alkaline.py` & `simses-1.3.3/simses/technology/hydrogen/electrolyzer/pressure/alkaline.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/electrolyzer/pressure/no_pressure_model.py` & `simses-1.3.3/simses/technology/hydrogen/electrolyzer/pressure/no_pressure_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/electrolyzer/pressure/var_cathode.py` & `simses-1.3.3/simses/technology/hydrogen/electrolyzer/pressure/var_cathode.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/electrolyzer/stack/alkaline/electrical_model.py` & `simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/alkaline/electrical_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/electrolyzer/stack/alkaline/electrolyzer_model.py` & `simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/alkaline/electrolyzer_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/electrolyzer/stack/alkaline/fluid_model.py` & `simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/alkaline/fluid_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/electrolyzer/stack/alkaline/parameters.py` & `simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/alkaline/parameters.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/electrolyzer/stack/alkaline/pressure_model.py` & `simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/alkaline/pressure_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/electrolyzer/stack/no_electrolyzer.py` & `simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/no_electrolyzer.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/electrolyzer/stack/pem.py` & `simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/pem.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/efficiency_curves.py` & `simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/efficiency_curves.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/electrical_model.py` & `simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/electrical_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/electrolyzer_model.py` & `simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/electrolyzer_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/electrolyzer_model_ptl_coating.py` & `simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/electrolyzer_model_ptl_coating.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/fluid_model.py` & `simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/fluid_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/membrane_model.py` & `simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/membrane_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/parameters.py` & `simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/parameters.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/pressure_model.py` & `simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/pressure_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/electrolyzer/stack/stack_model.py` & `simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/stack_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/electrolyzer/system.py` & `simses-1.3.3/simses/technology/hydrogen/electrolyzer/system.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/electrolyzer/thermal/abstract_model.py` & `simses-1.3.3/simses/technology/hydrogen/electrolyzer/thermal/abstract_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/electrolyzer/thermal/alkaline.py` & `simses-1.3.3/simses/technology/hydrogen/electrolyzer/thermal/alkaline.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/electrolyzer/thermal/no_thermal_model.py` & `simses-1.3.3/simses/technology/hydrogen/electrolyzer/thermal/no_thermal_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/electrolyzer/thermal/pem.py` & `simses-1.3.3/simses/technology/hydrogen/electrolyzer/thermal/pem.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/factory.py` & `simses-1.3.3/simses/technology/hydrogen/factory.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/fuel_cell/factory.py` & `simses-1.3.3/simses/technology/hydrogen/fuel_cell/factory.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/fuel_cell/pressure/no_pressure.py` & `simses-1.3.3/simses/technology/hydrogen/fuel_cell/pressure/no_pressure.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/fuel_cell/pressure/pressure_model.py` & `simses-1.3.3/simses/technology/hydrogen/fuel_cell/pressure/pressure_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/fuel_cell/stack/jupiter.py` & `simses-1.3.3/simses/technology/hydrogen/fuel_cell/stack/jupiter.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/fuel_cell/stack/no_fuel_cell.py` & `simses-1.3.3/simses/technology/hydrogen/fuel_cell/stack/no_fuel_cell.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/fuel_cell/stack/pem.py` & `simses-1.3.3/simses/technology/hydrogen/fuel_cell/stack/pem.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/fuel_cell/stack/stack_model.py` & `simses-1.3.3/simses/technology/hydrogen/fuel_cell/stack/stack_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/fuel_cell/system.py` & `simses-1.3.3/simses/technology/hydrogen/fuel_cell/system.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/fuel_cell/thermal/no_thermal_model.py` & `simses-1.3.3/simses/technology/hydrogen/fuel_cell/thermal/no_thermal_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/fuel_cell/thermal/simple.py` & `simses-1.3.3/simses/technology/hydrogen/fuel_cell/thermal/simple.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/fuel_cell/thermal/thermal_model.py` & `simses-1.3.3/simses/technology/hydrogen/fuel_cell/thermal/thermal_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/hydrogen_storage/hydrogen_storage.py` & `simses-1.3.3/simses/technology/hydrogen/hydrogen_storage/hydrogen_storage.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/hydrogen_storage/pipeline/simple_pipeline.py` & `simses-1.3.3/simses/technology/hydrogen/hydrogen_storage/pipeline/simple_pipeline.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/hydrogen_storage/pressuretank/pressuretank.py` & `simses-1.3.3/simses/technology/hydrogen/hydrogen_storage/pressuretank/pressuretank.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/system.py` & `simses-1.3.3/simses/technology/hydrogen/system.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/hydrogen/test/test_pem_electrolyzer.py` & `simses-1.3.3/simses/technology/hydrogen/test/test_pem_electrolyzer.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/battery.py` & `simses-1.3.3/simses/technology/lithium_ion/battery.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/battery_management_system/management_system.py` & `simses-1.3.3/simses/technology/lithium_ion/battery_management_system/management_system.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/cell/electric/default.py` & `simses-1.3.3/simses/technology/lithium_ion/cell/electric/default.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/cell/electric/properties.py` & `simses-1.3.3/simses/technology/lithium_ion/cell/electric/properties.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/cell/format/abstract.py` & `simses-1.3.3/simses/technology/lithium_ion/cell/format/abstract.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/cell/format/pouch.py` & `simses-1.3.3/simses/technology/lithium_ion/cell/format/pouch.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/cell/format/prismatic.py` & `simses-1.3.3/simses/technology/lithium_ion/cell/format/prismatic.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/cell/format/round.py` & `simses-1.3.3/simses/technology/lithium_ion/cell/format/round.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/cell/generic.py` & `simses-1.3.3/simses/technology/lithium_ion/cell/generic.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/cell/isea.py` & `simses-1.3.3/simses/technology/lithium_ion/cell/isea.py`

 * *Files 24% similar despite different names*

```diff
@@ -30,33 +30,49 @@
         isea_cell_properties = cell.get_cell_properties()
         super().__init__(voltage, capacity, soh, isea_cell_properties, DefaultThermalCellProperties(),
                          RoundCell18650(), battery_config)
 
         ocv_mat: numpy.ndarray = cell.get_open_cicuit_voltage()
         ocv_soc_arr: numpy.ndarray = cell.get_open_cicuit_voltage_soc()
         ocv_temp_arr: numpy.ndarray = cell.get_open_cicuit_voltage_temperature()
-        self.__open_circuit_voltage_interpolation = scipy.interpolate.interp2d(ocv_soc_arr, ocv_temp_arr.T, ocv_mat,
-                                                                               kind='linear')
+
+        if len(ocv_temp_arr.T) == 1:
+            self.__open_circuit_voltage_interpolation = scipy.interpolate.interp1d(ocv_soc_arr, ocv_mat,kind='linear')
+            self.__temperature_dependency = False
+        else:
+            self.__temperature_dependency = True
+            self.__open_circuit_voltage_interpolation = scipy.interpolate.interp2d(ocv_soc_arr, ocv_temp_arr.T, ocv_mat,
+                                                                                   kind='linear')
         rint_mat: numpy.ndarray = cell.get_internal_resistance()
         rint_soc_arr: numpy.ndarray = cell.get_internal_resistance_soc()
         rint_temp_arr: numpy.ndarray = cell.get_internal_resistance_temperature()
-        self.__internal_resistance_interpolation = scipy.interpolate.interp2d(rint_soc_arr, rint_temp_arr.T, rint_mat,
-                                                                              kind='linear')
+        if len(ocv_temp_arr.T) == 1:
+            self.__internal_resistance_interpolation = scipy.interpolate.interp1d(rint_soc_arr, rint_mat,kind='linear')
+        else:
+            self.__internal_resistance_interpolation = scipy.interpolate.interp2d(rint_soc_arr, rint_temp_arr.T,
+                                                                                  rint_mat,kind='linear')
 
     def get_open_circuit_voltage(self, battery_state: LithiumIonState) -> float:
         soc: float = battery_state.soc * 100.0
         temp: float = battery_state.temperature - 273.15
-        res: float = float(self.__open_circuit_voltage_interpolation(soc, temp))
+        if self.__temperature_dependency:
+            res: float = float(self.__open_circuit_voltage_interpolation(soc, temp))
+        else:
+            res: float = float(self.__open_circuit_voltage_interpolation(soc))
+
         # print(soc, temp, res)
         return res * self.get_serial_scale()
 
     def get_internal_resistance(self, battery_state: LithiumIonState) -> float:
         soc: float = battery_state.soc * 100.0
         temp: float = battery_state.temperature - 273.15
-        res: float = float(self.__internal_resistance_interpolation(soc, temp))
+        if self.__temperature_dependency:
+            res: float = float(self.__internal_resistance_interpolation(soc, temp))
+        else:
+            res: float = float(self.__internal_resistance_interpolation(soc))
         # print(soc, temp, res)
         return res / self.get_parallel_scale() * self.get_serial_scale()
 
     def get_name(self) -> str:
         return self.__name
 
     def close(self):
```

### Comparing `simses-1.3.2/simses/technology/lithium_ion/cell/lfp_sony.py` & `simses-1.3.3/simses/technology/lithium_ion/cell/lfp_sony.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/cell/lmo_daimler.py` & `simses-1.3.3/simses/technology/lithium_ion/cell/lmo_daimler.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/cell/lto_lmo.py` & `simses-1.3.3/simses/technology/lithium_ion/cell/lto_lmo.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/cell/lto_nmc.py` & `simses-1.3.3/simses/technology/lithium_ion/cell/lto_nmc.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/cell/nca_panasonic_generic.py` & `simses-1.3.3/simses/technology/lithium_ion/cell/nca_panasonic_generic.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/cell/nca_panasonic_ncr.py` & `simses-1.3.3/simses/technology/lithium_ion/cell/nca_panasonic_ncr.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/cell/nmc_lgmj1.py` & `simses-1.3.3/simses/technology/lithium_ion/cell/nmc_lgmj1.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/cell/nmc_molicel.py` & `simses-1.3.3/simses/technology/lithium_ion/cell/nmc_molicel.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/cell/nmc_molicel_generic.py` & `simses-1.3.3/simses/technology/lithium_ion/cell/nmc_molicel_generic.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/cell/nmc_samsung78Ah.py` & `simses-1.3.3/simses/technology/lithium_ion/cell/nmc_samsung78Ah.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/cell/nmc_samsung94Ah.py` & `simses-1.3.3/simses/technology/lithium_ion/cell/nmc_samsung94Ah.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/cell/nmc_samsung94Ah_hybrid.py` & `simses-1.3.3/simses/technology/lithium_ion/cell/nmc_samsung94Ah_hybrid.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/cell/nmc_sanyo_ur18650e.py` & `simses-1.3.3/simses/technology/lithium_ion/cell/nmc_sanyo_ur18650e.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/cell/sodium_ion/sodium_ion_green_rock.py` & `simses-1.3.3/simses/technology/lithium_ion/cell/sodium_ion/sodium_ion_green_rock.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/cell/thermal/default.py` & `simses-1.3.3/simses/technology/lithium_ion/cell/thermal/default.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/cell/thermal/properties.py` & `simses-1.3.3/simses/technology/lithium_ion/cell/thermal/properties.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/cell/type.py` & `simses-1.3.3/simses/technology/lithium_ion/cell/type.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/circuit.py` & `simses-1.3.3/simses/technology/lithium_ion/circuit.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/degradation/calendar/calendar_degradation.py` & `simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/calendar_degradation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/degradation/calendar/generic_cell.py` & `simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/generic_cell.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/degradation/calendar/lfp_generic.py` & `simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/lfp_generic.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/degradation/calendar/lfp_sony.py` & `simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/lfp_sony.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/degradation/calendar/lto_lmo.py` & `simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/lto_lmo.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/degradation/calendar/lto_nmc.py` & `simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/lto_nmc.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/degradation/calendar/nca_generic.py` & `simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/nca_generic.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/degradation/calendar/nca_panasonicNCR.py` & `simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/nca_panasonicNCR.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/degradation/calendar/nmc_generic.py` & `simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/nmc_generic.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/degradation/calendar/nmc_lgmj1.py` & `simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/nmc_lgmj1.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/degradation/calendar/nmc_molicel.py` & `simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/nmc_molicel.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/degradation/calendar/nmc_sanyo_ur18650e.py` & `simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/nmc_sanyo_ur18650e.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/degradation/calendar/no_calendar_dedradation.py` & `simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/no_calendar_dedradation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/degradation/cyclic/cyclic_degradation.py` & `simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/cyclic_degradation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/degradation/cyclic/generic_cell.py` & `simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/generic_cell.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/degradation/cyclic/lfp_generic.py` & `simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/lfp_generic.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/degradation/cyclic/lfp_sony.py` & `simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/lfp_sony.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/degradation/cyclic/lto_lmo.py` & `simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/lto_lmo.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/degradation/cyclic/lto_nmc.py` & `simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/lto_nmc.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/degradation/cyclic/nca_generic.py` & `simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/nca_generic.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/degradation/cyclic/nca_panasonicNCR.py` & `simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/nca_panasonicNCR.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/degradation/cyclic/nmc_generic.py` & `simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/nmc_generic.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/degradation/cyclic/nmc_lgmj1.py` & `simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/nmc_lgmj1.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/degradation/cyclic/nmc_molicel.py` & `simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/nmc_molicel.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/degradation/cyclic/nmc_sanyo_ur18650e.py` & `simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/nmc_sanyo_ur18650e.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/degradation/cyclic/no_cyclic_degradation.py` & `simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/no_cyclic_degradation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/degradation/degradation_model.py` & `simses-1.3.3/simses/technology/lithium_ion/degradation/degradation_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/degradation/generic_cell.py` & `simses-1.3.3/simses/technology/lithium_ion/degradation/generic_cell.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/degradation/lfp_generic.py` & `simses-1.3.3/simses/technology/lithium_ion/degradation/lfp_generic.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/degradation/lfp_sony.py` & `simses-1.3.3/simses/technology/lithium_ion/degradation/lfp_sony.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/degradation/lmo_daimler.py` & `simses-1.3.3/simses/technology/lithium_ion/degradation/lmo_daimler.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/degradation/lto_lmo.py` & `simses-1.3.3/simses/technology/lithium_ion/degradation/lto_lmo.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/degradation/lto_nmc.py` & `simses-1.3.3/simses/technology/lithium_ion/degradation/lto_nmc.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/degradation/nca_generic.py` & `simses-1.3.3/simses/technology/lithium_ion/degradation/nca_generic.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/degradation/nca_panasonicNCR.py` & `simses-1.3.3/simses/technology/lithium_ion/degradation/nca_panasonicNCR.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/degradation/nmc_generic.py` & `simses-1.3.3/simses/technology/lithium_ion/degradation/nmc_generic.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/degradation/nmc_lgmj1.py` & `simses-1.3.3/simses/technology/lithium_ion/degradation/nmc_lgmj1.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/degradation/nmc_molicel.py` & `simses-1.3.3/simses/technology/lithium_ion/degradation/nmc_molicel.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/degradation/nmc_samsung94Ah.py` & `simses-1.3.3/simses/technology/lithium_ion/degradation/nmc_samsung94Ah.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/degradation/nmc_sanyo_ur18650e.py` & `simses-1.3.3/simses/technology/lithium_ion/degradation/nmc_sanyo_ur18650e.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/degradation/no_degradation.py` & `simses-1.3.3/simses/technology/lithium_ion/degradation/no_degradation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/equivalent_circuit_model/equivalent_circuit.py` & `simses-1.3.3/simses/technology/lithium_ion/equivalent_circuit_model/equivalent_circuit.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/equivalent_circuit_model/rint_model.py` & `simses-1.3.3/simses/technology/lithium_ion/equivalent_circuit_model/rint_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/factory.py` & `simses-1.3.3/simses/technology/lithium_ion/factory.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/test/test_battery.py` & `simses-1.3.3/simses/technology/lithium_ion/test/test_battery.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/test/test_bms.py` & `simses-1.3.3/simses/technology/lithium_ion/test/test_bms.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/lithium_ion/test/test_type.py` & `simses-1.3.3/simses/technology/lithium_ion/test/test_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,10 +45,9 @@
     def test_ocv(self, soc, lithium_ion_subclass_list):
         for lithium_ion_subclass in lithium_ion_subclass_list:
             if lithium_ion_subclass.__name__ == IseaCellType.__name__:
                 continue
             uut = self.make_lithium_ion_cell(lithium_ion_subclass)
             self.lithium_ion_state.soc = soc
             # all ocv values must be between the cell minimal voltage and maximum voltage
-            ocv = uut.get_open_circuit_voltage(self.lithium_ion_state)
-            assert ocv >= uut.get_min_voltage()
-            assert ocv <= uut.get_max_voltage()
+            assert uut.get_open_circuit_voltage(self.lithium_ion_state) >= uut.get_min_voltage()
+            assert uut.get_open_circuit_voltage(self.lithium_ion_state) <= uut.get_max_voltage()
```

### Comparing `simses-1.3.2/simses/technology/redox_flow/degradation/capacity_degradation.py` & `simses-1.3.3/simses/technology/redox_flow/degradation/capacity_degradation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/redox_flow/degradation/const_hydrogen_current.py` & `simses-1.3.3/simses/technology/redox_flow/degradation/const_hydrogen_current.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/redox_flow/degradation/no_degradation.py` & `simses-1.3.3/simses/technology/redox_flow/degradation/no_degradation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/redox_flow/degradation/variable_hydrogen_current.py` & `simses-1.3.3/simses/technology/redox_flow/degradation/variable_hydrogen_current.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/redox_flow/electrochemical/abstract_electrochemical.py` & `simses-1.3.3/simses/technology/redox_flow/electrochemical/abstract_electrochemical.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/redox_flow/electrochemical/control/redox_control_system.py` & `simses-1.3.3/simses/technology/redox_flow/electrochemical/control/redox_control_system.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/redox_flow/electrochemical/rint_model.py` & `simses-1.3.3/simses/technology/redox_flow/electrochemical/rint_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/redox_flow/factory.py` & `simses-1.3.3/simses/technology/redox_flow/factory.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/redox_flow/pump_algorithm/abstract_pump_algorithm.py` & `simses-1.3.3/simses/technology/redox_flow/pump_algorithm/abstract_pump_algorithm.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/redox_flow/pump_algorithm/constant_pressure_pulsed.py` & `simses-1.3.3/simses/technology/redox_flow/pump_algorithm/constant_pressure_pulsed.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/redox_flow/pump_algorithm/fix_flow_rate_start_stop.py` & `simses-1.3.3/simses/technology/redox_flow/pump_algorithm/fix_flow_rate_start_stop.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/redox_flow/pump_algorithm/stoich_flow_rate.py` & `simses-1.3.3/simses/technology/redox_flow/pump_algorithm/stoich_flow_rate.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/redox_flow/stack/abstract_stack.py` & `simses-1.3.3/simses/technology/redox_flow/stack/abstract_stack.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/redox_flow/stack/cell_data_stack_5500w.py` & `simses-1.3.3/simses/technology/redox_flow/stack/cell_data_stack_5500w.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/redox_flow/stack/dummy_stack_3000w.py` & `simses-1.3.3/simses/technology/redox_flow/stack/dummy_stack_3000w.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/redox_flow/stack/dummy_stack_5500W.py` & `simses-1.3.3/simses/technology/redox_flow/stack/dummy_stack_5500W.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/redox_flow/stack/electrolyte/abstract_electrolyte.py` & `simses-1.3.3/simses/technology/redox_flow/stack/electrolyte/abstract_electrolyte.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/redox_flow/stack/electrolyte/vanadium.py` & `simses-1.3.3/simses/technology/redox_flow/stack/electrolyte/vanadium.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/redox_flow/stack/high_performance_stack_5700W.py` & `simses-1.3.3/simses/technology/redox_flow/stack/high_performance_stack_5700W.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/redox_flow/stack/industrial_stack_1500w.py` & `simses-1.3.3/simses/technology/redox_flow/stack/industrial_stack_1500w.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/redox_flow/stack/industrial_stack_9000w.py` & `simses-1.3.3/simses/technology/redox_flow/stack/industrial_stack_9000w.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/redox_flow/system.py` & `simses-1.3.3/simses/technology/redox_flow/system.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/redox_flow/test/test_stack_module.py` & `simses-1.3.3/simses/technology/redox_flow/test/test_stack_module.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses/technology/storage.py` & `simses-1.3.3/simses/technology/storage.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.2/simses.egg-info/SOURCES.txt` & `simses-1.3.3/simses/simses.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,16 @@
 LICENSE.txt
 MANIFEST.in
 README.md
-setup.py
-doc/__init__.py
-doc/conf.py
-doc/graph/__init__.py
-doc/graph/graph.py
+pyproject.toml
 simses/VERSION
-simses/__init__.py
 simses/analysis.defaults.ini
 simses/data.defaults.ini
 simses/logger.defaults.ini
-simses/main.py
 simses/simulation.defaults.ini
-simses.egg-info/PKG-INFO
-simses.egg-info/SOURCES.txt
-simses.egg-info/dependency_links.txt
-simses.egg-info/requires.txt
-simses.egg-info/top_level.txt
 simses/analysis/__init__.py
 simses/analysis/factory.py
 simses/analysis/storage.py
 simses/analysis/utils.py
 simses/analysis/data/__init__.py
 simses/analysis/data/abstract_data.py
 simses/analysis/data/electrolyzer.py
@@ -256,15 +245,18 @@
 simses/data/logo/SimSES.png
 simses/data/logo/__init__.py
 simses/data/power_electronics/__init__.py
 simses/data/power_electronics/sinamics_S120_efficiency.csv
 simses/data/profile/__init__.py
 simses/data/profile/economic/__init__.py
 simses/data/profile/power/__init__.py
+simses/data/profile/power/mockup_power_load_profile.csv
 simses/data/profile/technical/__init__.py
+simses/data/profile/technical/mockup_power_home_profile.csv
+simses/data/profile/technical/mockup_power_soc_profile.csv
 simses/data/profile/thermal/__init__.py
 simses/data/pump/__init__.py
 simses/data/pump/pump_efficiency_renner_RM1_5_35.csv
 simses/data/redox_flow/__init__.py
 simses/data/redox_flow/degradation/H2_Current_F1_Schweiss.csv
 simses/data/redox_flow/degradation/H2_Current_F2_Schweiss.csv
 simses/data/redox_flow/degradation/H2_Current_F3_Schweiss.csv
@@ -300,16 +292,16 @@
 simses/logic/energy_management/strategy/basic/soc_follower.py
 simses/logic/energy_management/strategy/basic/use_all_renewable_energy.py
 simses/logic/energy_management/strategy/optimization/__init__.py
 simses/logic/energy_management/strategy/optimization/forecast_utils/__init__.py
 simses/logic/energy_management/strategy/optimization/linearized_models/__init__.py
 simses/logic/energy_management/strategy/serial/__init__.py
 simses/logic/energy_management/strategy/stacked/__init__.py
-simses/logic/energy_management/strategy/stacked/dynamic_multi_use.py
 simses/logic/energy_management/strategy/stacked/fcr_idm_recharge_stacked.py
+simses/logic/energy_management/strategy/stacked/parallel_multi_use_with_stealing.py
 simses/logic/energy_management/strategy/stacked/stacked_operation_strategy.py
 simses/logic/power_distribution/__init__.py
 simses/logic/power_distribution/efficient.py
 simses/logic/power_distribution/equal.py
 simses/logic/power_distribution/power_distributor.py
 simses/logic/power_distribution/soc.py
 simses/logic/power_distribution/state.py
@@ -327,27 +319,32 @@
 simses/logic/test/test_peak_shaving.py
 simses/logic/test/test_residential_pv_greedy.py
 simses/logic/test/test_soc_based_power_distributor.py
 simses/logic/thermal_management/__init__.py
 simses/logic/thermal_management/on_off_controller.py
 simses/logic/thermal_management/pid_controller.py
 simses/logic/thermal_management/thermal_management.py
+simses/simses.egg-info/PKG-INFO
+simses/simses.egg-info/SOURCES.txt
+simses/simses.egg-info/dependency_links.txt
+simses/simses.egg-info/requires.txt
+simses/simses.egg-info/top_level.txt
 simses/simulation/__init__.py
 simses/simulation/batch_processing.py
 simses/simulation/batch_simulation.py
 simses/simulation/example.py
 simses/simulation/simulator.py
 simses/simulation/case_studies/__init__.py
 simses/simulation/case_studies/case_study_1_peak_shaving.py
 simses/simulation/case_studies/case_study_2_fcr.py
 simses/simulation/case_studies/configs/__init__.py
 simses/simulation/simbas/__init__.py
-simses/simulation/simbas/cell_config.csv
 simses/simulation/simbas/room_tool_reader.py
 simses/simulation/simbas/simbas.py
+simses/simulation/simulation_examples/__init__.py
 simses/simulation/system_tests/__init__.py
 simses/simulation/system_tests/system_test.py
 simses/simulation/system_tests/configs/__init__.py
 simses/system/__init__.py
 simses/system/factory.py
 simses/system/storage_circuit.py
 simses/system/storage_system_ac.py
@@ -359,15 +356,14 @@
 simses/system/auxiliary/compression/hydrogen_isentrop.py
 simses/system/auxiliary/gas_drying/__init__.py
 simses/system/auxiliary/gas_drying/gas_dryer.py
 simses/system/auxiliary/gas_drying/hydrogen.py
 simses/system/auxiliary/heating_ventilation_air_conditioning/__init__.py
 simses/system/auxiliary/heating_ventilation_air_conditioning/fan.py
 simses/system/auxiliary/heating_ventilation_air_conditioning/fix_cop_hvac.py
-simses/system/auxiliary/heating_ventilation_air_conditioning/fix_cop_hvac_pid_control.py
 simses/system/auxiliary/heating_ventilation_air_conditioning/hvac.py
 simses/system/auxiliary/heating_ventilation_air_conditioning/no_hvac.py
 simses/system/auxiliary/pump/__init__.py
 simses/system/auxiliary/pump/abstract_pump.py
 simses/system/auxiliary/pump/fixeta_centrifugal.py
 simses/system/auxiliary/pump/scalable_variable_eta_centrifugal.py
 simses/system/auxiliary/pump/variable_eta_centrifugal.py
```

