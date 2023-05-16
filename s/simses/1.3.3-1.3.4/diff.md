# Comparing `tmp/simses-1.3.3.tar.gz` & `tmp/simses-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simses-1.3.3.tar", last modified: Tue May 16 14:07:41 2023, max compression
+gzip compressed data, was "simses-1.3.4.tar", last modified: Tue May 16 15:07:23 2023, max compression
```

## Comparing `simses-1.3.3.tar` & `simses-1.3.4.tar`

### file list

```diff
@@ -1,785 +1,790 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:41.472790 simses-1.3.3/
--rw-rw-rw-   0        0        0     1647 2023-02-10 09:26:04.000000 simses-1.3.3/LICENSE.txt
--rw-rw-rw-   0        0        0      158 2023-02-08 12:59:18.000000 simses-1.3.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1790 2023-05-16 14:07:41.470634 simses-1.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     1184 2023-05-16 10:48:41.000000 simses-1.3.3/README.md
--rw-rw-rw-   0        0        0     1099 2023-05-16 14:06:41.000000 simses-1.3.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-16 14:07:41.472790 simses-1.3.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.290157 simses-1.3.3/simses/
--rw-rw-rw-   0        0        0        5 2023-05-16 12:07:02.000000 simses-1.3.3/simses/VERSION
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.306386 simses-1.3.3/simses/analysis/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.345914 simses-1.3.3/simses/analysis/data/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/data/__init__.py
--rw-rw-rw-   0        0        0    10671 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/data/abstract_data.py
--rw-rw-rw-   0        0        0     6060 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/data/electrolyzer.py
--rw-rw-rw-   0        0        0     1980 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/data/energy_management.py
--rw-rw-rw-   0        0        0     2543 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/data/fuel_cell.py
--rw-rw-rw-   0        0        0     6598 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/data/hydrogen.py
--rw-rw-rw-   0        0        0     3563 2023-03-06 13:30:03.000000 simses-1.3.3/simses/analysis/data/lithium_ion.py
--rw-rw-rw-   0        0        0     3679 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/data/redox_flow.py
--rw-rw-rw-   0        0        0     6714 2023-03-06 13:30:03.000000 simses-1.3.3/simses/analysis/data/system.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.363385 simses-1.3.3/simses/analysis/evaluation/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/__init__.py
--rw-rw-rw-   0        0        0     5937 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/abstract_evaluation.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.369392 simses-1.3.3/simses/analysis/evaluation/economic/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/economic/__init__.py
--rw-rw-rw-   0        0        0     7935 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/economic/economic_evaluation.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.413443 simses-1.3.3/simses/analysis/evaluation/economic/revenue_stream/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/economic/revenue_stream/__init__.py
--rw-rw-rw-   0        0        0     3611 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/economic/revenue_stream/abstract_revenue_stream.py
--rw-rw-rw-   0        0        0    10705 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/economic/revenue_stream/demand_charge_reduction.py
--rw-rw-rw-   0        0        0     4503 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/economic/revenue_stream/electricity_consumption.py
--rw-rw-rw-   0        0        0     3452 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/economic/revenue_stream/energy_cost_reduction.py
--rw-rw-rw-   0        0        0     4318 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/economic/revenue_stream/fcr_revenue_stream.py
--rw-rw-rw-   0        0        0     4453 2023-03-06 13:30:03.000000 simses-1.3.3/simses/analysis/evaluation/economic/revenue_stream/intraday_recharge.py
--rw-rw-rw-   0        0        0     2742 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/economic/revenue_stream/operation_and_maintenance.py
--rw-rw-rw-   0        0        0     5668 2023-03-06 13:30:03.000000 simses-1.3.3/simses/analysis/evaluation/merger.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.454442 simses-1.3.3/simses/analysis/evaluation/plotting/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/plotting/__init__.py
--rw-rw-rw-   0        0        0      514 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/plotting/axis.py
--rw-rw-rw-   0        0        0     5130 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/plotting/energy_plotting.py
--rw-rw-rw-   0        0        0     3256 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/plotting/matplot_plotting.py
--rw-rw-rw-   0        0        0     7441 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/plotting/plotly_plotting.py
--rw-rw-rw-   0        0        0     4506 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/plotting/plotter.py
--rw-rw-rw-   0        0        0     7765 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/plotting/sankey_diagram.py
--rw-rw-rw-   0        0        0     5695 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/plotting/sunburst_diagram.py
--rw-rw-rw-   0        0        0    11357 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/plotting/system_parameters.py
--rw-rw-rw-   0        0        0     7539 2023-03-06 13:30:03.000000 simses-1.3.3/simses/analysis/evaluation/result.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.497442 simses-1.3.3/simses/analysis/evaluation/technical/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/technical/__init__.py
--rw-rw-rw-   0        0        0    16301 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/technical/electrolyzer.py
--rw-rw-rw-   0        0        0     4496 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/technical/fuel_cell.py
--rw-rw-rw-   0        0        0    16450 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/technical/hydrogen.py
--rw-rw-rw-   0        0        0     7977 2023-03-06 13:30:03.000000 simses-1.3.3/simses/analysis/evaluation/technical/lithium_ion.py
--rw-rw-rw-   0        0        0     5943 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/technical/redox_flow.py
--rw-rw-rw-   0        0        0     9681 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/technical/site_level.py
--rw-rw-rw-   0        0        0    18811 2023-03-06 13:30:03.000000 simses-1.3.3/simses/analysis/evaluation/technical/system.py
--rw-rw-rw-   0        0        0    11829 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/evaluation/technical/technical_evaluation.py
--rw-rw-rw-   0        0        0    11807 2023-05-16 11:18:59.000000 simses-1.3.3/simses/analysis/factory.py
--rw-rw-rw-   0        0        0     3346 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/storage.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.521447 simses-1.3.3/simses/analysis/test/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/test/__init__.py
--rw-rw-rw-   0        0        0     4929 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/test/test_demand_charge_reduction.py
--rw-rw-rw-   0        0        0     3723 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/test/test_energy_cost_reduction.py
--rw-rw-rw-   0        0        0     3268 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/test/test_fcr_revenue_stream.py
--rw-rw-rw-   0        0        0     3356 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/test/test_intraday_recharge_revenue_stream.py
--rw-rw-rw-   0        0        0    16978 2023-03-06 13:30:03.000000 simses-1.3.3/simses/analysis/test/test_technical_evaluation.py
--rw-rw-rw-   0        0        0     1066 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis/utils.py
--rw-rw-rw-   0        0        0     1609 2023-02-20 12:50:46.000000 simses-1.3.3/simses/analysis.defaults.ini
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.543444 simses-1.3.3/simses/commons/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.551443 simses-1.3.3/simses/commons/config/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/__init__.py
--rw-rw-rw-   0        0        0     4909 2023-03-06 13:30:03.000000 simses-1.3.3/simses/commons/config/abstract_config.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.569445 simses-1.3.3/simses/commons/config/analysis/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/analysis/__init__.py
--rw-rw-rw-   0        0        0      549 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/analysis/analysis_config.py
--rw-rw-rw-   0        0        0     5265 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/analysis/economic.py
--rw-rw-rw-   0        0        0     4645 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/analysis/general.py
--rw-rw-rw-   0        0        0     1138 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/analysis/market.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.606329 simses-1.3.3/simses/commons/config/data/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/data/__init__.py
--rw-rw-rw-   0        0        0      742 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/data/auxiliary.py
--rw-rw-rw-   0        0        0     7429 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/data/battery.py
--rw-rw-rw-   0        0        0      571 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/data/data_config.py
--rw-rw-rw-   0        0        0     2057 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/data/electrolyzer.py
--rw-rw-rw-   0        0        0     1900 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/data/energy_management.py
--rw-rw-rw-   0        0        0     1478 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/data/fuel_cell.py
--rw-rw-rw-   0        0        0     1481 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/data/power_electronics.py
--rw-rw-rw-   0        0        0     4119 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/data/redox_flow.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.622492 simses-1.3.3/simses/commons/config/generation/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/generation/__init__.py
--rw-rw-rw-   0        0        0     6251 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/generation/analysis.py
--rw-rw-rw-   0        0        0     2220 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/generation/generator.py
--rw-rw-rw-   0        0        0    34101 2023-05-15 14:47:15.000000 simses-1.3.3/simses/commons/config/generation/simulation.py
--rw-rw-rw-   0        0        0     1522 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/log.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.658491 simses-1.3.3/simses/commons/config/simulation/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/simulation/__init__.py
--rw-rw-rw-   0        0        0     5452 2023-03-06 13:30:03.000000 simses-1.3.3/simses/commons/config/simulation/battery.py
--rw-rw-rw-   0        0        0     1175 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/simulation/electrolyzer.py
--rw-rw-rw-   0        0        0     5372 2023-05-15 14:47:15.000000 simses-1.3.3/simses/commons/config/simulation/energy_management.py
--rw-rw-rw-   0        0        0     1144 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/simulation/fuel_cell.py
--rw-rw-rw-   0        0        0     2203 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/simulation/general.py
--rw-rw-rw-   0        0        0     4116 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/simulation/hydrogen.py
--rw-rw-rw-   0        0        0     7818 2023-03-06 13:30:03.000000 simses-1.3.3/simses/commons/config/simulation/profile.py
--rw-rw-rw-   0        0        0     1129 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/simulation/redox_flow.py
--rw-rw-rw-   0        0        0     1388 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/simulation/simulation_config.py
--rw-rw-rw-   0        0        0     6105 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/config/simulation/system.py
--rw-rw-rw-   0        0        0     5887 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/console_printer.py
--rw-rw-rw-   0        0        0     1775 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/constants.py
--rw-rw-rw-   0        0        0     7169 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/csv_standard.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.674491 simses-1.3.3/simses/commons/cycle_detection/
--rw-rw-rw-   0        0        0        2 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/cycle_detection/__init__.py
--rw-rw-rw-   0        0        0     2347 2023-03-06 13:30:03.000000 simses-1.3.3/simses/commons/cycle_detection/cycle_detector.py
--rw-rw-rw-   0        0        0     3294 2023-03-06 13:30:03.000000 simses-1.3.3/simses/commons/cycle_detection/half_cycle_detector.py
--rw-rw-rw-   0        0        0      695 2023-03-06 13:30:03.000000 simses-1.3.3/simses/commons/cycle_detection/no_cycle_detector.py
--rw-rw-rw-   0        0        0     6987 2023-03-06 13:30:03.000000 simses-1.3.3/simses/commons/cycle_detection/rainflow_cycle_detector.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.687548 simses-1.3.3/simses/commons/data/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/data/__init__.py
--rw-rw-rw-   0        0        0     6798 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/data/csv_data_handler.py
--rw-rw-rw-   0        0        0     1443 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/data/data_handler.py
--rw-rw-rw-   0        0        0     1183 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/data/no_data_handler.py
--rw-rw-rw-   0        0        0     1654 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/error.py
--rw-rw-rw-   0        0        0     1820 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/log.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.696582 simses-1.3.3/simses/commons/profile/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/profile/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.714488 simses-1.3.3/simses/commons/profile/economic/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/profile/economic/__init__.py
--rw-rw-rw-   0        0        0      493 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/profile/economic/constant.py
--rw-rw-rw-   0        0        0      905 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/profile/economic/fcr.py
--rw-rw-rw-   0        0        0      912 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/profile/economic/intraday.py
--rw-rw-rw-   0        0        0      784 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/profile/economic/market.py
--rw-rw-rw-   0        0        0    20695 2023-05-16 13:19:22.000000 simses-1.3.3/simses/commons/profile/file.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.761521 simses-1.3.3/simses/commons/profile/power/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/profile/power/__init__.py
--rw-rw-rw-   0        0        0     1927 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/profile/power/alternating.py
--rw-rw-rw-   0        0        0      808 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/profile/power/constant.py
--rw-rw-rw-   0        0        0     1729 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/profile/power/file.py
--rw-rw-rw-   0        0        0      966 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/profile/power/generation.py
--rw-rw-rw-   0        0        0      953 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/profile/power/load.py
--rw-rw-rw-   0        0        0      826 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/profile/power/power_profile.py
--rw-rw-rw-   0        0        0     1974 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/profile/power/random.py
--rw-rw-rw-   0        0        0      950 2023-03-06 13:30:03.000000 simses-1.3.3/simses/commons/profile/power/v2g_profile.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.784723 simses-1.3.3/simses/commons/profile/technical/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/profile/technical/__init__.py
--rw-rw-rw-   0        0        0     1769 2023-03-06 13:30:03.000000 simses-1.3.3/simses/commons/profile/technical/binary.py
--rw-rw-rw-   0        0        0     2367 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/profile/technical/frequency.py
--rw-rw-rw-   0        0        0      756 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/profile/technical/soc.py
--rw-rw-rw-   0        0        0      735 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/profile/technical/technical.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.817481 simses-1.3.3/simses/commons/state/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/state/__init__.py
--rw-rw-rw-   0        0        0     6761 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/state/abstract_state.py
--rw-rw-rw-   0        0        0     2777 2023-03-06 13:30:03.000000 simses-1.3.3/simses/commons/state/energy_management.py
--rw-rw-rw-   0        0        0     2476 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/state/parameters.py
--rw-rw-rw-   0        0        0    11708 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/state/parameters_reader.py
--rw-rw-rw-   0        0        0     9283 2023-03-06 13:30:03.000000 simses-1.3.3/simses/commons/state/system.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.850246 simses-1.3.3/simses/commons/state/technology/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/state/technology/__init__.py
--rw-rw-rw-   0        0        0    12642 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/state/technology/electrolyzer.py
--rw-rw-rw-   0        0        0     6008 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/state/technology/fuel_cell.py
--rw-rw-rw-   0        0        0     3675 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/state/technology/hydrogen.py
--rw-rw-rw-   0        0        0    10784 2023-03-06 13:30:03.000000 simses-1.3.3/simses/commons/state/technology/lithium_ion.py
--rw-rw-rw-   0        0        0     7185 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/state/technology/redox_flow.py
--rw-rw-rw-   0        0        0     2550 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/state/technology/storage.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.882531 simses-1.3.3/simses/commons/test/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/test/__init__.py
--rw-rw-rw-   0        0        0      702 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/test/test_constant_power_profile.py
--rw-rw-rw-   0        0        0     2361 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/test/test_file_power_profile.py
--rw-rw-rw-   0        0        0      849 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/test/test_linear_interpolation.py
--rw-rw-rw-   0        0        0      814 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/test/test_mean_average.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.896212 simses-1.3.3/simses/commons/timeseries/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/timeseries/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.908110 simses-1.3.3/simses/commons/timeseries/average/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/timeseries/average/__init__.py
--rw-rw-rw-   0        0        0      622 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/timeseries/average/average.py
--rw-rw-rw-   0        0        0      507 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/timeseries/average/mean_average.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:35.942784 simses-1.3.3/simses/commons/timeseries/interpolation/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/timeseries/interpolation/__init__.py
--rw-rw-rw-   0        0        0     1311 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/timeseries/interpolation/interpolation.py
--rw-rw-rw-   0        0        0      782 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/timeseries/interpolation/last_value.py
--rw-rw-rw-   0        0        0      565 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/timeseries/interpolation/linear_interpolation.py
--rw-rw-rw-   0        0        0     1418 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/timeseries/timevalue.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:36.070312 simses-1.3.3/simses/commons/utils/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/utils/__init__.py
--rw-rw-rw-   0        0        0     7923 2023-05-15 14:47:15.000000 simses-1.3.3/simses/commons/utils/cell_reader.py
--rw-rw-rw-   0        0        0     2227 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/utils/converter_comparison.py
--rw-rw-rw-   0        0        0     2092 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/utils/count_lines_of_code.py
--rw-rw-rw-   0        0        0     5380 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/utils/fitting.py
--rw-rw-rw-   0        0        0     5155 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/utils/heatmap.py
--rw-rw-rw-   0        0        0     5198 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/utils/max_peak_shaving_limit.py
--rw-rw-rw-   0        0        0     9471 2023-02-20 12:50:46.000000 simses-1.3.3/simses/commons/utils/utilities.py
--rw-rw-rw-   0        0        0     4300 2023-05-15 14:47:15.000000 simses-1.3.3/simses/commons/utils/xml_reader.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:36.077321 simses-1.3.3/simses/data/
--rw-rw-rw-   0        0        0       97 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:36.081391 simses-1.3.3/simses/data/electrolyzer/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:36.380889 simses-1.3.3/simses/data/electrolyzer/evaluation/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/evaluation/__init__.py
--rw-rw-rw-   0        0        0     3394 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/evaluation/comparison_lut_ana_new_with_afterfitting.py
--rw-rw-rw-   0        0        0     3816 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/evaluation/comparison_lut_ana_new_without_afterfitting.py
--rw-rw-rw-   0        0        0     3471 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/evaluation/comparison_lut_no_current_influence_ana_new.py
--rw-rw-rw-   0        0        0     6008 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/evaluation/multi_dim_regression_current_dens_3rd_best_fit.py
--rw-rw-rw-   0        0        0      336 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/evaluation/parameters_multi_dim_current_dens_fit_3rd_bestfit.csv
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:36.671082 simses-1.3.3/simses/data/electrolyzer/lookuptable/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/__init__.py
--rw-rw-rw-   0        0        0     7662 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/activation_overpotential_lookup_alkaline.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:36.842972 simses-1.3.3/simses/data/electrolyzer/lookuptable/archive/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/archive/__init__.py
--rw-rw-rw-   0        0        0  2333800 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/archive/activation_overpotential_lookup_alkaline.csv.gz
--rw-rw-rw-   0        0        0   367371 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/archive/cell_currentdensity_lookup.csv.gz
--rw-rw-rw-   0        0        0   347857 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/archive/cell_voltage_lookup.csv.gz
--rw-rw-rw-   0        0        0  1520365 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/archive/cell_voltage_lookup_alkaline.csv.gz
--rw-rw-rw-   0        0        0    29206 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/archive/polarizationcurve_alkaline.py
--rw-rw-rw-   0        0        0  1693681 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/cell_current_lookup_alkaline.gz
--rw-rw-rw-   0        0        0     5835 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/multi_dim_polarizationcurve.py
--rw-rw-rw-   0        0        0     5857 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/multi_dim_polarizationcurve_no_current_influence_on_part_pressure.py
--rw-rw-rw-   0        0        0    19149 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/polarizationcurve1bar.csv
--rw-rw-rw-   0        0        0     3910 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/polarizationcurve_e_master.py
--rw-rw-rw-   0        0        0    18991 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/powercurve1bar.csv
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:36.846970 simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:36.882717 simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/activation_overpotential_alkaline/
--rw-rw-rw-   0        0        0      909 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/activation_overpotential_alkaline/25°C.csv
--rw-rw-rw-   0        0        0      919 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/activation_overpotential_alkaline/90°C.csv
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/activation_overpotential_alkaline/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:36.912922 simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/general_alkaline/
--rw-rw-rw-   0        0        0     1084 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/general_alkaline/GHW 130°C at 30bar.csv
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/general_alkaline/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:37.066222 simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/
--rw-rw-rw-   0        0        0     1324 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/23°C.csv
--rw-rw-rw-   0        0        0     1365 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/35°C.csv
--rw-rw-rw-   0        0        0     1416 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/40°C.csv
--rw-rw-rw-   0        0        0     1479 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/45°C.csv
--rw-rw-rw-   0        0        0     1530 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/53,5°C.csv
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:37.142303 simses-1.3.3/simses/data/electrolyzer/parameters/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/parameters/__init__.py
--rw-rw-rw-   0        0        0      221 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/parameters/parameters_alkaline_overvoltage_fit.csv
--rw-rw-rw-   0        0        0      299 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/parameters/parameters_multi_dim_current_dens_fit.csv
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:37.191954 simses-1.3.3/simses/data/electrolyzer/regression/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/regression/__init__.py
--rw-rw-rw-   0        0        0  1943227 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/regression/cell_currentdensity_lookup.csv
--rw-rw-rw-   0        0        0     5615 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/electrolyzer/regression/multi_dim_regression_current_dens.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:37.195001 simses-1.3.3/simses/data/energy_management/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/energy_management/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:37.329134 simses-1.3.3/simses/data/fuel_cell/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/fuel_cell/__init__.py
--rw-rw-rw-   0        0        0    19570 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/fuel_cell/polarizationcurve1bar.csv
--rw-rw-rw-   0        0        0     9977 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/fuel_cell/polarizationcurve_fc_jupiter.py
--rw-rw-rw-   0        0        0     3857 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/fuel_cell/polarizationcurve_fc_master.py
--rw-rw-rw-   0        0        0    35785 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/fuel_cell/polarizationcurve_jupiter.csv
--rw-rw-rw-   0        0        0    19746 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/fuel_cell/powercurve1bar.csv
--rw-rw-rw-   0        0        0    36366 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/fuel_cell/powercurve_jupiter.csv
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:37.333220 simses-1.3.3/simses/data/lithium_ion/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data/lithium_ion/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.097781 simses-1.3.3/simses/data/lithium_ion/cell/
--rw-rw-rw-   0        0        0   338005 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/CLFP_Sony_US26650_OCV.csv
--rw-rw-rw-   0        0        0     1482 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/CLFP_Sony_US26650_Rint.csv
--rw-rw-rw-   0        0        0      581 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/CLFP_Sony_US26650_capacity_decrease_param.csv
--rw-rw-rw-   0        0        0      605 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/CLFP_Sony_US26650_resistance_increase_param.csv
--rw-rw-rw-   0        0        0     2487 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/LG_INR18560MJ1_OCV.csv
--rw-rw-rw-   0        0        0    16185 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/LG_INR18650MJ1_closs_calendar_aging.csv
--rw-rw-rw-   0        0        0    14576 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/LG_INR18650MJ1_closs_cycling_aging.csv
--rw-rw-rw-   0        0        0     7990 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/LG_INR18650MJ1_rint_cycling_aging.csv
--rw-rw-rw-   0        0        0     2919 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/LTO_LMO_closs_cycling_aging.csv
--rw-rw-rw-   0        0        0     2963 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/LTO_LMO_rint_cycling_aging.csv
--rw-rw-rw-   0        0        0     1126 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/LTO_NMC_closs_calendar_aging.csv
--rw-rw-rw-   0        0        0     2144 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/LTO_NMC_closs_cycling_aging.csv
--rw-rw-rw-   0        0        0     2284 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/LTO_NMC_rint_calendar_aging.csv
--rw-rw-rw-   0        0        0     1288 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/LTO_NMC_rint_cycling_aging.csv
--rw-rw-rw-   0        0        0     4849 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/NCA_PanasonicNCR_OCV.csv
--rw-rw-rw-   0        0        0    12237 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/NCA_PanasonicNCR_Rint.csv
--rw-rw-rw-   0        0        0     1068 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/NMC_Akasol_OEM_Rint.csv
--rw-rw-rw-   0        0        0     2384 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/NMC_Molicel_OCV.csv
--rw-rw-rw-   0        0        0    12168 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/NMC_Molicel_Rint.csv
--rw-rw-rw-   0        0        0    92642 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/NMC_Molicel_capacity_cal.csv
--rw-rw-rw-   0        0        0    24959 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/NMC_Molicel_capacity_cyc.csv
--rw-rw-rw-   0        0        0    80843 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/NMC_Molicel_ri_cal.csv
--rw-rw-rw-   0        0        0    25392 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/NMC_Molicel_ri_cyc.csv
--rw-rw-rw-   0        0        0    49004 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/NMC_Samsung_LabTest_cell_00_OCV.csv
--rw-rw-rw-   0        0        0    15435 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/NMC_Samsung_LabTest_cell_00_Ri.csv
--rw-rw-rw-   0        0        0      604 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/NMC_Sanyo_OCV.csv
--rw-rw-rw-   0        0        0    12168 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/NMC_Sanyo_Rint.csv
--rw-rw-rw-   0        0        0     2979 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/Sodium_Ion_OCV_Green_Rock.csv
--rw-rw-rw-   0        0        0     4940 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/Sodium_Ion_Rint_Green_Rock.csv
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/cell/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.100786 simses-1.3.3/simses/data/lithium_ion/isea/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/lithium_ion/isea/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.112775 simses-1.3.3/simses/data/logo/
--rw-rw-rw-   0        0        0    36954 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/logo/SimSES.png
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/logo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.141831 simses-1.3.3/simses/data/power_electronics/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/power_electronics/__init__.py
--rw-rw-rw-   0        0        0    29262 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/power_electronics/sinamics_S120_efficiency.csv
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.145777 simses-1.3.3/simses/data/profile/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/profile/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.149776 simses-1.3.3/simses/data/profile/economic/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/profile/economic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.173903 simses-1.3.3/simses/data/profile/power/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/profile/power/__init__.py
--rw-rw-rw-   0        0        0       41 2023-05-16 11:42:41.000000 simses-1.3.3/simses/data/profile/power/mockup_power_load_profile.csv
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.219061 simses-1.3.3/simses/data/profile/technical/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/profile/technical/__init__.py
--rw-rw-rw-   0        0        0       46 2023-05-16 11:43:00.000000 simses-1.3.3/simses/data/profile/technical/mockup_power_home_profile.csv
--rw-rw-rw-   0        0        0       58 2023-05-16 11:43:00.000000 simses-1.3.3/simses/data/profile/technical/mockup_power_soc_profile.csv
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.223259 simses-1.3.3/simses/data/profile/thermal/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/profile/thermal/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.252975 simses-1.3.3/simses/data/pump/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/pump/__init__.py
--rw-rw-rw-   0        0        0      369 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/pump/pump_efficiency_renner_RM1_5_35.csv
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.260984 simses-1.3.3/simses/data/redox_flow/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/redox_flow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.358977 simses-1.3.3/simses/data/redox_flow/degradation/
--rw-rw-rw-   0        0        0      560 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/redox_flow/degradation/H2_Current_F1_Schweiss.csv
--rw-rw-rw-   0        0        0      290 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/redox_flow/degradation/H2_Current_F2_Schweiss.csv
--rw-rw-rw-   0        0        0      560 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/redox_flow/degradation/H2_Current_F3_Schweiss.csv
--rw-rw-rw-   0        0        0      243 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/redox_flow/degradation/H2_Current_F4_Schweiss.csv
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/redox_flow/degradation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.597946 simses-1.3.3/simses/data/redox_flow/stack/
--rw-rw-rw-   0        0        0      509 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/redox_flow/stack/RFB_cell_data_R.csv
--rw-rw-rw-   0        0        0      343 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/redox_flow/stack/RFB_highperformance_stack_R.csv
--rw-rw-rw-   0        0        0       80 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/redox_flow/stack/SD_HP_Stack.csv
--rw-rw-rw-   0        0        0     2731 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/redox_flow/stack/SHUNT_CellStack_2250_40.csv
--rw-rw-rw-   0        0        0    28277 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/redox_flow/stack/SHUNT_FILE_INDUSTRIAL_STACK_1500W.csv
--rw-rw-rw-   0        0        0    28360 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/redox_flow/stack/SHUNT_FILE_INDUSTRIAL_STACK_9000W.csv
--rw-rw-rw-   0        0        0     5079 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/redox_flow/stack/SHUNT_HP_Stack.csv
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/data/redox_flow/stack/__init__.py
--rw-rw-rw-   0        0        0     4214 2023-02-20 12:50:46.000000 simses-1.3.3/simses/data.defaults.ini
--rw-rw-rw-   0        0        0      571 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logger.defaults.ini
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.604777 simses-1.3.3/simses/logic/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.627335 simses-1.3.3/simses/logic/energy_management/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/energy_management/__init__.py
--rw-rw-rw-   0        0        0    10719 2023-05-16 12:36:02.000000 simses-1.3.3/simses/logic/energy_management/energy_management_factory.py
--rw-rw-rw-   0        0        0     2470 2023-03-06 13:30:03.000000 simses-1.3.3/simses/logic/energy_management/energy_management_system.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.641450 simses-1.3.3/simses/logic/energy_management/strategy/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/energy_management/strategy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.720165 simses-1.3.3/simses/logic/energy_management/strategy/basic/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/energy_management/strategy/basic/__init__.py
--rw-rw-rw-   0        0        0     9246 2023-05-15 14:47:15.000000 simses-1.3.3/simses/logic/energy_management/strategy/basic/electric_vehicle.py
--rw-rw-rw-   0        0        0    13078 2023-05-15 14:47:15.000000 simses-1.3.3/simses/logic/energy_management/strategy/basic/electric_vehicle_soc.py
--rw-rw-rw-   0        0        0     9891 2023-03-06 13:30:03.000000 simses-1.3.3/simses/logic/energy_management/strategy/basic/electric_vehicle_v2g.py
--rw-rw-rw-   0        0        0     2234 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/energy_management/strategy/basic/ev_charger_with_buffer.py
--rw-rw-rw-   0        0        0     5761 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/energy_management/strategy/basic/frequency_containment_reserve.py
--rw-rw-rw-   0        0        0     4102 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/energy_management/strategy/basic/intraday_market_recharge.py
--rw-rw-rw-   0        0        0     7724 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/energy_management/strategy/basic/peak_shaving_perfect_foresight.py
--rw-rw-rw-   0        0        0     2541 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/energy_management/strategy/basic/peak_shaving_simple.py
--rw-rw-rw-   0        0        0     1310 2023-05-15 14:47:15.000000 simses-1.3.3/simses/logic/energy_management/strategy/basic/power_follower.py
--rw-rw-rw-   0        0        0     5407 2023-05-15 14:47:15.000000 simses-1.3.3/simses/logic/energy_management/strategy/basic/residential_pv_feed_in_damp.py
--rw-rw-rw-   0        0        0     1807 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/energy_management/strategy/basic/residential_pv_greedy.py
--rw-rw-rw-   0        0        0     1489 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/energy_management/strategy/basic/soc_follower.py
--rw-rw-rw-   0        0        0     1501 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/energy_management/strategy/basic/use_all_renewable_energy.py
--rw-rw-rw-   0        0        0      281 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/energy_management/strategy/operation_priority.py
--rw-rw-rw-   0        0        0     2041 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/energy_management/strategy/operation_strategy.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.727285 simses-1.3.3/simses/logic/energy_management/strategy/optimization/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/energy_management/strategy/optimization/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.765014 simses-1.3.3/simses/logic/energy_management/strategy/optimization/forecast_utils/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/energy_management/strategy/optimization/forecast_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.800306 simses-1.3.3/simses/logic/energy_management/strategy/optimization/linearized_models/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/energy_management/strategy/optimization/linearized_models/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.807397 simses-1.3.3/simses/logic/energy_management/strategy/serial/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/energy_management/strategy/serial/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.853000 simses-1.3.3/simses/logic/energy_management/strategy/stacked/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/energy_management/strategy/stacked/__init__.py
--rw-rw-rw-   0        0        0     1132 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/energy_management/strategy/stacked/fcr_idm_recharge_stacked.py
--rw-rw-rw-   0        0        0    44499 2023-03-06 13:30:03.000000 simses-1.3.3/simses/logic/energy_management/strategy/stacked/parallel_multi_use_with_stealing.py
--rw-rw-rw-   0        0        0     1198 2023-03-06 13:30:03.000000 simses-1.3.3/simses/logic/energy_management/strategy/stacked/stacked_operation_strategy.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.901427 simses-1.3.3/simses/logic/power_distribution/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/power_distribution/__init__.py
--rw-rw-rw-   0        0        0     3038 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/power_distribution/efficient.py
--rw-rw-rw-   0        0        0      626 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/power_distribution/equal.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.905450 simses-1.3.3/simses/logic/power_distribution/optimization_utils/
--rw-rw-rw-   0        0        0       46 2023-03-06 13:30:03.000000 simses-1.3.3/simses/logic/power_distribution/optimization_utils/__init__.py
--rw-rw-rw-   0        0        0     1475 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/power_distribution/power_distributor.py
--rw-rw-rw-   0        0        0     1500 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/power_distribution/soc.py
--rw-rw-rw-   0        0        0     4106 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/power_distribution/state.py
--rw-rw-rw-   0        0        0     9364 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/power_distribution/technology.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:38.976313 simses-1.3.3/simses/logic/test/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/test/__init__.py
--rw-rw-rw-   0        0        0     5066 2023-05-16 11:40:09.000000 simses-1.3.3/simses/logic/test/test_electric_vehicle_SOC_meanpower.py
--rw-rw-rw-   0        0        0     4951 2023-05-16 11:42:11.000000 simses-1.3.3/simses/logic/test/test_electric_vehicle_SOC_original.py
--rw-rw-rw-   0        0        0     5032 2023-05-16 11:41:52.000000 simses-1.3.3/simses/logic/test/test_electric_vehicle_SOC_paused.py
--rw-rw-rw-   0        0        0     4815 2023-05-16 11:41:31.000000 simses-1.3.3/simses/logic/test/test_electric_vehicle_SOC_uncontrolled.py
--rw-rw-rw-   0        0        0     5481 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/test/test_electric_vehicle_all_strategies.py
--rw-rw-rw-   0        0        0     4726 2023-05-16 11:42:40.000000 simses-1.3.3/simses/logic/test/test_electric_vehicle_uncontrolled.py
--rw-rw-rw-   0        0        0     1181 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/test/test_equal_power_distributor.py
--rw-rw-rw-   0        0        0    21492 2023-03-06 13:30:03.000000 simses-1.3.3/simses/logic/test/test_multi_use.py
--rw-rw-rw-   0        0        0     3169 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/test/test_peak_shaving.py
--rw-rw-rw-   0        0        0     3061 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/test/test_residential_pv_greedy.py
--rw-rw-rw-   0        0        0     1188 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/test/test_soc_based_power_distributor.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.000819 simses-1.3.3/simses/logic/thermal_management/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/thermal_management/__init__.py
--rw-rw-rw-   0        0        0     4285 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/thermal_management/on_off_controller.py
--rw-rw-rw-   0        0        0     6005 2023-03-06 13:30:03.000000 simses-1.3.3/simses/logic/thermal_management/pid_controller.py
--rw-rw-rw-   0        0        0       77 2023-02-20 12:50:47.000000 simses-1.3.3/simses/logic/thermal_management/thermal_management.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.052293 simses-1.3.3/simses/simses.egg-info/
--rw-rw-rw-   0        0        0     1790 2023-05-16 14:07:34.000000 simses-1.3.3/simses/simses.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    34826 2023-05-16 14:07:34.000000 simses-1.3.3/simses/simses.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 14:07:34.000000 simses-1.3.3/simses/simses.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2023-05-16 14:07:34.000000 simses-1.3.3/simses/simses.egg-info/requires.txt
--rw-rw-rw-   0        0        0       57 2023-05-16 14:07:34.000000 simses-1.3.3/simses/simses.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.074368 simses-1.3.3/simses/simulation/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/simulation/__init__.py
--rw-rw-rw-   0        0        0     4368 2023-02-20 12:50:47.000000 simses-1.3.3/simses/simulation/batch_processing.py
--rw-rw-rw-   0        0        0     2937 2023-02-20 12:50:47.000000 simses-1.3.3/simses/simulation/batch_simulation.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.087235 simses-1.3.3/simses/simulation/case_studies/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/simulation/case_studies/__init__.py
--rw-rw-rw-   0        0        0     1419 2023-02-20 12:50:47.000000 simses-1.3.3/simses/simulation/case_studies/case_study_1_peak_shaving.py
--rw-rw-rw-   0        0        0     1930 2023-02-20 12:50:47.000000 simses-1.3.3/simses/simulation/case_studies/case_study_2_fcr.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.092647 simses-1.3.3/simses/simulation/case_studies/configs/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/simulation/case_studies/configs/__init__.py
--rw-rw-rw-   0        0        0     4090 2023-02-20 12:50:47.000000 simses-1.3.3/simses/simulation/example.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.103074 simses-1.3.3/simses/simulation/simbas/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/simulation/simbas/__init__.py
--rw-rw-rw-   0        0        0     2534 2023-05-15 14:47:15.000000 simses-1.3.3/simses/simulation/simbas/room_tool_reader.py
--rw-rw-rw-   0        0        0     5577 2023-05-15 14:47:15.000000 simses-1.3.3/simses/simulation/simbas/simbas.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.107736 simses-1.3.3/simses/simulation/simulation_examples/
--rw-rw-rw-   0        0        0        0 2023-03-06 13:30:03.000000 simses-1.3.3/simses/simulation/simulation_examples/__init__.py
--rw-rw-rw-   0        0        0    10046 2023-05-15 14:47:15.000000 simses-1.3.3/simses/simulation/simulator.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.114803 simses-1.3.3/simses/simulation/system_tests/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/simulation/system_tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.118620 simses-1.3.3/simses/simulation/system_tests/configs/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/simulation/system_tests/configs/__init__.py
--rw-rw-rw-   0        0        0     4971 2023-02-20 12:50:47.000000 simses-1.3.3/simses/simulation/system_tests/system_test.py
--rw-rw-rw-   0        0        0    14759 2023-05-15 14:47:15.000000 simses-1.3.3/simses/simulation.defaults.ini
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.207852 simses-1.3.3/simses/system/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.214056 simses-1.3.3/simses/system/auxiliary/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/auxiliary/__init__.py
--rw-rw-rw-   0        0        0      889 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/auxiliary/auxiliary.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.274920 simses-1.3.3/simses/system/auxiliary/compression/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/auxiliary/compression/__init__.py
--rw-rw-rw-   0        0        0     1088 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/auxiliary/compression/compressor.py
--rw-rw-rw-   0        0        0     1080 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/auxiliary/compression/hydrogen_isentrop.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.286586 simses-1.3.3/simses/system/auxiliary/gas_drying/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/auxiliary/gas_drying/__init__.py
--rw-rw-rw-   0        0        0      749 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/auxiliary/gas_drying/gas_dryer.py
--rw-rw-rw-   0        0        0      946 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/auxiliary/gas_drying/hydrogen.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.307474 simses-1.3.3/simses/system/auxiliary/heating_ventilation_air_conditioning/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/auxiliary/heating_ventilation_air_conditioning/__init__.py
--rw-rw-rw-   0        0        0     1530 2023-03-06 13:30:03.000000 simses-1.3.3/simses/system/auxiliary/heating_ventilation_air_conditioning/fan.py
--rw-rw-rw-   0        0        0     4567 2023-03-06 13:30:03.000000 simses-1.3.3/simses/system/auxiliary/heating_ventilation_air_conditioning/fix_cop_hvac.py
--rw-rw-rw-   0        0        0     1662 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/auxiliary/heating_ventilation_air_conditioning/hvac.py
--rw-rw-rw-   0        0        0     1243 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/auxiliary/heating_ventilation_air_conditioning/no_hvac.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.346623 simses-1.3.3/simses/system/auxiliary/pump/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/auxiliary/pump/__init__.py
--rw-rw-rw-   0        0        0     1810 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/auxiliary/pump/abstract_pump.py
--rw-rw-rw-   0        0        0     1144 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/auxiliary/pump/fixeta_centrifugal.py
--rw-rw-rw-   0        0        0     2178 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/auxiliary/pump/scalable_variable_eta_centrifugal.py
--rw-rw-rw-   0        0        0     2300 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/auxiliary/pump/variable_eta_centrifugal.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.354167 simses-1.3.3/simses/system/auxiliary/water_heating/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/auxiliary/water_heating/__init__.py
--rw-rw-rw-   0        0        0      924 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/auxiliary/water_heating/water_heater.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.399513 simses-1.3.3/simses/system/dc_coupling/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/dc_coupling/__init__.py
--rw-rw-rw-   0        0        0      448 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/dc_coupling/bus_charging_dc_coupling.py
--rw-rw-rw-   0        0        0      551 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/dc_coupling/bus_charging_profile.py
--rw-rw-rw-   0        0        0     1643 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/dc_coupling/dc_coupler.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.436697 simses-1.3.3/simses/system/dc_coupling/generation/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/dc_coupling/generation/__init__.py
--rw-rw-rw-   0        0        0      752 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/dc_coupling/generation/dc_generation.py
--rw-rw-rw-   0        0        0      466 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/dc_coupling/generation/no_dc_generation.py
--rw-rw-rw-   0        0        0     1330 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/dc_coupling/generation/pv_dc_generation.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.480867 simses-1.3.3/simses/system/dc_coupling/load/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/dc_coupling/load/__init__.py
--rw-rw-rw-   0        0        0      980 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/dc_coupling/load/dc_bus_charging_fixed.py
--rw-rw-rw-   0        0        0     1372 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/dc_coupling/load/dc_bus_charging_profile.py
--rw-rw-rw-   0        0        0     2875 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/dc_coupling/load/dc_bus_charging_random.py
--rw-rw-rw-   0        0        0      812 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/dc_coupling/load/dc_load.py
--rw-rw-rw-   0        0        0     1058 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/dc_coupling/load/dc_radio_ups_load.py
--rw-rw-rw-   0        0        0      444 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/dc_coupling/load/no_dc_load.py
--rw-rw-rw-   0        0        0      327 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/dc_coupling/no_dc_coupling.py
--rw-rw-rw-   0        0        0      747 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/dc_coupling/usp_dc_coupling.py
--rw-rw-rw-   0        0        0    36968 2023-05-16 12:59:52.000000 simses-1.3.3/simses/system/factory.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.513195 simses-1.3.3/simses/system/housing/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/housing/__init__.py
--rw-rw-rw-   0        0        0     2954 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/housing/abstract_housing.py
--rw-rw-rw-   0        0        0     7225 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/housing/forty_ft_container.py
--rw-rw-rw-   0        0        0     3281 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/housing/layer.py
--rw-rw-rw-   0        0        0      453 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/housing/no_housing.py
--rw-rw-rw-   0        0        0     7218 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/housing/twenty_ft_container.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.525795 simses-1.3.3/simses/system/power_electronics/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/power_electronics/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.629219 simses-1.3.3/simses/system/power_electronics/acdc_converter/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/power_electronics/acdc_converter/__init__.py
--rw-rw-rw-   0        0        0     3531 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/power_electronics/acdc_converter/abstract_acdc_converter.py
--rw-rw-rw-   0        0        0     4152 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/power_electronics/acdc_converter/bonfiglioli.py
--rw-rw-rw-   0        0        0     2296 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/power_electronics/acdc_converter/fix_efficiency.py
--rw-rw-rw-   0        0        0      407 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/power_electronics/acdc_converter/no_loss.py
--rw-rw-rw-   0        0        0     3446 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/power_electronics/acdc_converter/notton.py
--rw-rw-rw-   0        0        0     2821 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/power_electronics/acdc_converter/notton_loss.py
--rw-rw-rw-   0        0        0     2459 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/power_electronics/acdc_converter/rampinelli_fit.py
--rw-rw-rw-   0        0        0     3879 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/power_electronics/acdc_converter/sinamics.py
--rw-rw-rw-   0        0        0     4198 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/power_electronics/acdc_converter/stable.py
--rw-rw-rw-   0        0        0     4895 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/power_electronics/acdc_converter/stacked.py
--rw-rw-rw-   0        0        0     8150 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/power_electronics/acdc_converter/sungrow.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.669113 simses-1.3.3/simses/system/power_electronics/dcdc_converter/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/power_electronics/dcdc_converter/__init__.py
--rw-rw-rw-   0        0        0     2423 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/power_electronics/dcdc_converter/abstract_dcdc_converter.py
--rw-rw-rw-   0        0        0     2775 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/power_electronics/dcdc_converter/fix_efficiency.py
--rw-rw-rw-   0        0        0     2299 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/power_electronics/dcdc_converter/no_dcdc.py
--rw-rw-rw-   0        0        0     1847 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/power_electronics/dcdc_converter/no_loss.py
--rw-rw-rw-   0        0        0     6350 2023-03-06 13:30:03.000000 simses-1.3.3/simses/system/power_electronics/electronics.py
--rw-rw-rw-   0        0        0     3725 2023-05-15 14:47:15.000000 simses-1.3.3/simses/system/storage_circuit.py
--rw-rw-rw-   0        0        0    10030 2023-05-15 14:47:15.000000 simses-1.3.3/simses/system/storage_system_ac.py
--rw-rw-rw-   0        0        0     5713 2023-03-06 13:30:03.000000 simses-1.3.3/simses/system/storage_system_dc.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.757091 simses-1.3.3/simses/system/test/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/test/__init__.py
--rw-rw-rw-   0        0        0     7277 2023-05-16 11:19:36.000000 simses-1.3.3/simses/system/test/test_acdc_converter.py
--rw-rw-rw-   0        0        0     1387 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/test/test_constant_ambient_temperature.py
--rw-rw-rw-   0        0        0     3571 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/test/test_fix_cop_hvac.py
--rw-rw-rw-   0        0        0      423 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/test/test_fixeta_centrifugal_pump.py
--rw-rw-rw-   0        0        0     3846 2023-03-06 13:30:03.000000 simses-1.3.3/simses/system/test/test_location_ambient_temperature.py
--rw-rw-rw-   0        0        0     1976 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/test/test_location_ambient_temperature_profile_check.py
--rw-rw-rw-   0        0        0     4318 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/test/test_location_solar_irradiation_model.py
--rw-rw-rw-   0        0        0     2801 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/test/test_location_solar_irradiation_model_profile_check.py
--rw-rw-rw-   0        0        0     2274 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/test/test_notton_acdc_converter.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.771303 simses-1.3.3/simses/system/thermal/
--rw-rw-rw-   0        0        0        2 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/thermal/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.836635 simses-1.3.3/simses/system/thermal/ambient/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/thermal/ambient/__init__.py
--rw-rw-rw-   0        0        0     1325 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/thermal/ambient/ambient_thermal_model.py
--rw-rw-rw-   0        0        0     1064 2023-05-15 14:47:15.000000 simses-1.3.3/simses/system/thermal/ambient/constant_temperature.py
--rw-rw-rw-   0        0        0     1654 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/thermal/ambient/location_temperature.py
--rw-rw-rw-   0        0        0     1585 2023-03-06 13:30:03.000000 simses-1.3.3/simses/system/thermal/ambient/user_battery_temperature.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.861538 simses-1.3.3/simses/system/thermal/model/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/thermal/model/__init__.py
--rw-rw-rw-   0        0        0     3667 2023-03-06 13:30:03.000000 simses-1.3.3/simses/system/thermal/model/no_system_thermal_model.py
--rw-rw-rw-   0        0        0     3095 2023-03-06 13:30:03.000000 simses-1.3.3/simses/system/thermal/model/system_thermal_model.py
--rw-rw-rw-   0        0        0    15883 2023-03-06 13:30:03.000000 simses-1.3.3/simses/system/thermal/model/zero_d_room_thermal_model.py
--rw-rw-rw-   0        0        0    24072 2023-03-06 13:30:03.000000 simses-1.3.3/simses/system/thermal/model/zero_d_system_thermal_model.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.932068 simses-1.3.3/simses/system/thermal/solar_irradiation/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/thermal/solar_irradiation/__init__.py
--rw-rw-rw-   0        0        0    18001 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/thermal/solar_irradiation/location.py
--rw-rw-rw-   0        0        0      795 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/thermal/solar_irradiation/no_solar_irradiation.py
--rw-rw-rw-   0        0        0     1464 2023-02-20 12:50:47.000000 simses-1.3.3/simses/system/thermal/solar_irradiation/solar_irradiation_model.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.940977 simses-1.3.3/simses/technology/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.951245 simses-1.3.3/simses/technology/hydrogen/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:39.960254 simses-1.3.3/simses/technology/hydrogen/control/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/control/__init__.py
--rw-rw-rw-   0        0        0     3315 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/control/management.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.035765 simses-1.3.3/simses/technology/hydrogen/control/pressure/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/control/pressure/__init__.py
--rw-rw-rw-   0        0        0     3335 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/control/pressure/ideal_var_cathode.py
--rw-rw-rw-   0        0        0      723 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/control/pressure/no_pressure_controller.py
--rw-rw-rw-   0        0        0      791 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/control/pressure/pressure_controller.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.062705 simses-1.3.3/simses/technology/hydrogen/control/thermal/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/control/thermal/__init__.py
--rw-rw-rw-   0        0        0     3633 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/control/thermal/ideal_var_flow.py
--rw-rw-rw-   0        0        0      531 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/control/thermal/no_thermal_controller.py
--rw-rw-rw-   0        0        0      795 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/control/thermal/thermal_controller.py
--rw-rw-rw-   0        0        0     2522 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/control/thermal/var_flow.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.081794 simses-1.3.3/simses/technology/hydrogen/electrolyzer/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.108296 simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.142316 simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/calendar/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/calendar/__init__.py
--rw-rw-rw-   0        0        0     2105 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/calendar/calendar_degradation.py
--rw-rw-rw-   0        0        0      785 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/calendar/no_calendar_degradation.py
--rw-rw-rw-   0        0        0     3071 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/calendar/pem_analytic.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.184191 simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/cyclic/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/cyclic/__init__.py
--rw-rw-rw-   0        0        0     2123 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/cyclic/cyclic_degradation.py
--rw-rw-rw-   0        0        0      796 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/cyclic/no_cyclic_degradation.py
--rw-rw-rw-   0        0        0     4542 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/cyclic/pem_analytic.py
--rw-rw-rw-   0        0        0     1437 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/cyclic/pem_analytic_ptl_coating.py
--rw-rw-rw-   0        0        0     4502 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/degradation_model.py
--rw-rw-rw-   0        0        0      728 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/no_degradation.py
--rw-rw-rw-   0        0        0     1517 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/pem_analytic.py
--rw-rw-rw-   0        0        0     1575 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/pem_analytic_ptl_coating.py
--rw-rw-rw-   0        0        0     9672 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/factory.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.215616 simses-1.3.3/simses/technology/hydrogen/electrolyzer/pressure/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/pressure/__init__.py
--rw-rw-rw-   0        0        0     1794 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/pressure/abstract_model.py
--rw-rw-rw-   0        0        0     2448 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/pressure/alkaline.py
--rw-rw-rw-   0        0        0     1802 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/pressure/no_pressure_model.py
--rw-rw-rw-   0        0        0     3656 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/pressure/var_cathode.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.239198 simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.275572 simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/alkaline/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/alkaline/__init__.py
--rw-rw-rw-   0        0        0    13091 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/alkaline/electrical_model.py
--rw-rw-rw-   0        0        0     8273 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/alkaline/electrolyzer_model.py
--rw-rw-rw-   0        0        0     1593 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/alkaline/fluid_model.py
--rw-rw-rw-   0        0        0     1697 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/alkaline/parameters.py
--rw-rw-rw-   0        0        0     1502 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/alkaline/pressure_model.py
--rw-rw-rw-   0        0        0     1474 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/no_electrolyzer.py
--rw-rw-rw-   0        0        0     4632 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/pem.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.353443 simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/__init__.py
--rw-rw-rw-   0        0        0     5244 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/efficiency_curves.py
--rw-rw-rw-   0        0        0     5765 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/electrical_model.py
--rw-rw-rw-   0        0        0     8627 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/electrolyzer_model.py
--rw-rw-rw-   0        0        0      603 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/electrolyzer_model_ptl_coating.py
--rw-rw-rw-   0        0        0     2461 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/fluid_model.py
--rw-rw-rw-   0        0        0     3649 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/membrane_model.py
--rw-rw-rw-   0        0        0     2077 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/parameters.py
--rw-rw-rw-   0        0        0     3318 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/pressure_model.py
--rw-rw-rw-   0        0        0     5098 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/stack_model.py
--rw-rw-rw-   0        0        0     5538 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/system.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.384462 simses-1.3.3/simses/technology/hydrogen/electrolyzer/thermal/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/thermal/__init__.py
--rw-rw-rw-   0        0        0     1691 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/thermal/abstract_model.py
--rw-rw-rw-   0        0        0     8252 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/thermal/alkaline.py
--rw-rw-rw-   0        0        0     1352 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/thermal/no_thermal_model.py
--rw-rw-rw-   0        0        0    12898 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/electrolyzer/thermal/pem.py
--rw-rw-rw-   0        0        0     2594 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/factory.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.400566 simses-1.3.3/simses/technology/hydrogen/fuel_cell/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/fuel_cell/__init__.py
--rw-rw-rw-   0        0        0     5007 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/fuel_cell/factory.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.424309 simses-1.3.3/simses/technology/hydrogen/fuel_cell/pressure/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/fuel_cell/pressure/__init__.py
--rw-rw-rw-   0        0        0     1527 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/fuel_cell/pressure/no_pressure.py
--rw-rw-rw-   0        0        0     1766 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/fuel_cell/pressure/pressure_model.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.460298 simses-1.3.3/simses/technology/hydrogen/fuel_cell/stack/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/fuel_cell/stack/__init__.py
--rw-rw-rw-   0        0        0     3734 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/fuel_cell/stack/jupiter.py
--rw-rw-rw-   0        0        0     1208 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/fuel_cell/stack/no_fuel_cell.py
--rw-rw-rw-   0        0        0     3141 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/fuel_cell/stack/pem.py
--rw-rw-rw-   0        0        0     2232 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/fuel_cell/stack/stack_model.py
--rw-rw-rw-   0        0        0     3181 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/fuel_cell/system.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.485387 simses-1.3.3/simses/technology/hydrogen/fuel_cell/thermal/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/fuel_cell/thermal/__init__.py
--rw-rw-rw-   0        0        0      913 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/fuel_cell/thermal/no_thermal_model.py
--rw-rw-rw-   0        0        0      963 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/fuel_cell/thermal/simple.py
--rw-rw-rw-   0        0        0     1015 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/fuel_cell/thermal/thermal_model.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.496183 simses-1.3.3/simses/technology/hydrogen/hydrogen_storage/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/hydrogen_storage/__init__.py
--rw-rw-rw-   0        0        0     1703 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/hydrogen_storage/hydrogen_storage.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.512071 simses-1.3.3/simses/technology/hydrogen/hydrogen_storage/pipeline/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/hydrogen_storage/pipeline/__init__.py
--rw-rw-rw-   0        0        0      500 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/hydrogen_storage/pipeline/pipeline.py
--rw-rw-rw-   0        0        0     1062 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/hydrogen_storage/pipeline/simple_pipeline.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.526746 simses-1.3.3/simses/technology/hydrogen/hydrogen_storage/pressuretank/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/hydrogen_storage/pressuretank/__init__.py
--rw-rw-rw-   0        0        0     3899 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/hydrogen_storage/pressuretank/pressuretank.py
--rw-rw-rw-   0        0        0     6240 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/system.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.534517 simses-1.3.3/simses/technology/hydrogen/test/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/test/__init__.py
--rw-rw-rw-   0        0        0     8265 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/hydrogen/test/test_pem_electrolyzer.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.561623 simses-1.3.3/simses/technology/lithium_ion/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/__init__.py
--rw-rw-rw-   0        0        0     6994 2023-03-06 13:30:03.000000 simses-1.3.3/simses/technology/lithium_ion/battery.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.573643 simses-1.3.3/simses/technology/lithium_ion/battery_management_system/
--rw-rw-rw-   0        0        0        2 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/battery_management_system/__init__.py
--rw-rw-rw-   0        0        0     7748 2023-03-06 13:30:03.000000 simses-1.3.3/simses/technology/lithium_ion/battery_management_system/management_system.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.699709 simses-1.3.3/simses/technology/lithium_ion/cell/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.718725 simses-1.3.3/simses/technology/lithium_ion/cell/electric/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/electric/__init__.py
--rw-rw-rw-   0        0        0     1006 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/electric/default.py
--rw-rw-rw-   0        0        0     3550 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/electric/properties.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.757435 simses-1.3.3/simses/technology/lithium_ion/cell/format/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/format/__init__.py
--rw-rw-rw-   0        0        0      829 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/format/abstract.py
--rw-rw-rw-   0        0        0      523 2023-03-06 13:30:03.000000 simses-1.3.3/simses/technology/lithium_ion/cell/format/pouch.py
--rw-rw-rw-   0        0        0      555 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/format/prismatic.py
--rw-rw-rw-   0        0        0      593 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/format/round.py
--rw-rw-rw-   0        0        0      298 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/format/round_18650.py
--rw-rw-rw-   0        0        0      298 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/format/round_26650.py
--rw-rw-rw-   0        0        0     1952 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/generic.py
--rw-rw-rw-   0        0        0     4224 2023-05-15 14:47:15.000000 simses-1.3.3/simses/technology/lithium_ion/cell/isea.py
--rw-rw-rw-   0        0        0     5009 2023-03-06 13:30:03.000000 simses-1.3.3/simses/technology/lithium_ion/cell/lfp_sony.py
--rw-rw-rw-   0        0        0      503 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/lfp_sony_generic.py
--rw-rw-rw-   0        0        0     8685 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/lmo_daimler.py
--rw-rw-rw-   0        0        0     5224 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/lto_lmo.py
--rw-rw-rw-   0        0        0     5352 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/lto_nmc.py
--rw-rw-rw-   0        0        0      532 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/nca_panasonic_generic.py
--rw-rw-rw-   0        0        0     5469 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/nca_panasonic_ncr.py
--rw-rw-rw-   0        0        0     4958 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/nmc_lgmj1.py
--rw-rw-rw-   0        0        0     4514 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/nmc_molicel.py
--rw-rw-rw-   0        0        0      518 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/nmc_molicel_generic.py
--rw-rw-rw-   0        0        0     4931 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/nmc_samsung78Ah.py
--rw-rw-rw-   0        0        0     7991 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/nmc_samsung94Ah.py
--rw-rw-rw-   0        0        0     8558 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/nmc_samsung94Ah_hybrid.py
--rw-rw-rw-   0        0        0     5481 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/nmc_sanyo_ur18650e.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.770758 simses-1.3.3/simses/technology/lithium_ion/cell/sodium_ion/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/sodium_ion/__init__.py
--rw-rw-rw-   0        0        0     5578 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/sodium_ion/sodium_ion_green_rock.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.790108 simses-1.3.3/simses/technology/lithium_ion/cell/thermal/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/thermal/__init__.py
--rw-rw-rw-   0        0        0      639 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/thermal/default.py
--rw-rw-rw-   0        0        0     2131 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/cell/thermal/properties.py
--rw-rw-rw-   0        0        0    16261 2023-03-06 13:30:03.000000 simses-1.3.3/simses/technology/lithium_ion/cell/type.py
--rw-rw-rw-   0        0        0    15101 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/circuit.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.881842 simses-1.3.3/simses/technology/lithium_ion/degradation/
--rw-rw-rw-   0        0        0        2 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:40.983318 simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/
--rw-rw-rw-   0        0        0        2 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/__init__.py
--rw-rw-rw-   0        0        0     3104 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/calendar_degradation.py
--rw-rw-rw-   0        0        0     2364 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/generic_cell.py
--rw-rw-rw-   0        0        0     2993 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/lfp_generic.py
--rw-rw-rw-   0        0        0     5050 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/lfp_sony.py
--rw-rw-rw-   0        0        0     3736 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/lto_lmo.py
--rw-rw-rw-   0        0        0     3698 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/lto_nmc.py
--rw-rw-rw-   0        0        0     2923 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/nca_generic.py
--rw-rw-rw-   0        0        0     4689 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/nca_panasonicNCR.py
--rw-rw-rw-   0        0        0     3063 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/nmc_generic.py
--rw-rw-rw-   0        0        0     3077 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/nmc_lgmj1.py
--rw-rw-rw-   0        0        0     4451 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/nmc_molicel.py
--rw-rw-rw-   0        0        0     2914 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/nmc_sanyo_ur18650e.py
--rw-rw-rw-   0        0        0      790 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/no_calendar_dedradation.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:41.075428 simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/
--rw-rw-rw-   0        0        0        2 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/__init__.py
--rw-rw-rw-   0        0        0     3202 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/cyclic_degradation.py
--rw-rw-rw-   0        0        0     2316 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/generic_cell.py
--rw-rw-rw-   0        0        0     4820 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/lfp_generic.py
--rw-rw-rw-   0        0        0     5993 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/lfp_sony.py
--rw-rw-rw-   0        0        0     4560 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/lto_lmo.py
--rw-rw-rw-   0        0        0     4568 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/lto_nmc.py
--rw-rw-rw-   0        0        0     4173 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/nca_generic.py
--rw-rw-rw-   0        0        0     6795 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/nca_panasonicNCR.py
--rw-rw-rw-   0        0        0     4784 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/nmc_generic.py
--rw-rw-rw-   0        0        0     4700 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/nmc_lgmj1.py
--rw-rw-rw-   0        0        0     6373 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/nmc_molicel.py
--rw-rw-rw-   0        0        0     3885 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/nmc_sanyo_ur18650e.py
--rw-rw-rw-   0        0        0      764 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/no_cyclic_degradation.py
--rw-rw-rw-   0        0        0     8719 2023-03-06 13:30:03.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/degradation_model.py
--rw-rw-rw-   0        0        0      958 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/generic_cell.py
--rw-rw-rw-   0        0        0      933 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/lfp_generic.py
--rw-rw-rw-   0        0        0     1159 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/lfp_sony.py
--rw-rw-rw-   0        0        0     1251 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/lmo_daimler.py
--rw-rw-rw-   0        0        0      853 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/lto_lmo.py
--rw-rw-rw-   0        0        0      853 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/lto_nmc.py
--rw-rw-rw-   0        0        0      933 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/nca_generic.py
--rw-rw-rw-   0        0        0      974 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/nca_panasonicNCR.py
--rw-rw-rw-   0        0        0      933 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/nmc_generic.py
--rw-rw-rw-   0        0        0      872 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/nmc_lgmj1.py
--rw-rw-rw-   0        0        0     1103 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/nmc_molicel.py
--rw-rw-rw-   0        0        0     1146 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/nmc_samsung94Ah.py
--rw-rw-rw-   0        0        0      921 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/nmc_sanyo_ur18650e.py
--rw-rw-rw-   0        0        0      804 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/degradation/no_degradation.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:41.093480 simses-1.3.3/simses/technology/lithium_ion/equivalent_circuit_model/
--rw-rw-rw-   0        0        0        4 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/equivalent_circuit_model/__init__.py
--rw-rw-rw-   0        0        0      527 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/equivalent_circuit_model/equivalent_circuit.py
--rw-rw-rw-   0        0        0     1861 2023-03-06 13:30:03.000000 simses-1.3.3/simses/technology/lithium_ion/equivalent_circuit_model/rint_model.py
--rw-rw-rw-   0        0        0    16756 2023-05-16 11:37:56.000000 simses-1.3.3/simses/technology/lithium_ion/factory.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:41.109333 simses-1.3.3/simses/technology/lithium_ion/test/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/test/__init__.py
--rw-rw-rw-   0        0        0     2384 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/lithium_ion/test/test_battery.py
--rw-rw-rw-   0        0        0     5158 2023-03-06 13:30:03.000000 simses-1.3.3/simses/technology/lithium_ion/test/test_bms.py
--rw-rw-rw-   0        0        0     2797 2023-05-16 11:18:19.000000 simses-1.3.3/simses/technology/lithium_ion/test/test_type.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:41.153758 simses-1.3.3/simses/technology/redox_flow/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:41.224759 simses-1.3.3/simses/technology/redox_flow/degradation/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/degradation/__init__.py
--rw-rw-rw-   0        0        0     1657 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/degradation/capacity_degradation.py
--rw-rw-rw-   0        0        0     2873 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/degradation/const_hydrogen_current.py
--rw-rw-rw-   0        0        0      541 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/degradation/no_degradation.py
--rw-rw-rw-   0        0        0     4209 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/degradation/variable_hydrogen_current.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:41.240005 simses-1.3.3/simses/technology/redox_flow/electrochemical/
--rw-rw-rw-   0        0        0        4 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/electrochemical/__init__.py
--rw-rw-rw-   0        0        0     1017 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/electrochemical/abstract_electrochemical.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:41.260662 simses-1.3.3/simses/technology/redox_flow/electrochemical/control/
--rw-rw-rw-   0        0        0        2 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/electrochemical/control/__init__.py
--rw-rw-rw-   0        0        0    10697 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/electrochemical/control/redox_control_system.py
--rw-rw-rw-   0        0        0     8509 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/electrochemical/rint_model.py
--rw-rw-rw-   0        0        0    17184 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/factory.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:41.292461 simses-1.3.3/simses/technology/redox_flow/pump_algorithm/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/pump_algorithm/__init__.py
--rw-rw-rw-   0        0        0     4905 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/pump_algorithm/abstract_pump_algorithm.py
--rw-rw-rw-   0        0        0     4324 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/pump_algorithm/constant_pressure_pulsed.py
--rw-rw-rw-   0        0        0     3741 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/pump_algorithm/fix_flow_rate_start_stop.py
--rw-rw-rw-   0        0        0     5153 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/pump_algorithm/stoich_flow_rate.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:41.330826 simses-1.3.3/simses/technology/redox_flow/stack/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/stack/__init__.py
--rw-rw-rw-   0        0        0    10504 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/stack/abstract_stack.py
--rw-rw-rw-   0        0        0     8549 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/stack/cell_data_stack_5500w.py
--rw-rw-rw-   0        0        0     4627 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/stack/dummy_stack_3000w.py
--rw-rw-rw-   0        0        0     4554 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/stack/dummy_stack_5500W.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:41.433772 simses-1.3.3/simses/technology/redox_flow/stack/electrolyte/
--rw-rw-rw-   0        0        0        4 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/stack/electrolyte/__init__.py
--rw-rw-rw-   0        0        0     3675 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/stack/electrolyte/abstract_electrolyte.py
--rw-rw-rw-   0        0        0     4086 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/stack/electrolyte/vanadium.py
--rw-rw-rw-   0        0        0     7211 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/stack/high_performance_stack_5700W.py
--rw-rw-rw-   0        0        0     5787 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/stack/industrial_stack_1500w.py
--rw-rw-rw-   0        0        0     5663 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/stack/industrial_stack_9000w.py
--rw-rw-rw-   0        0        0    13481 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/system.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:07:41.462998 simses-1.3.3/simses/technology/redox_flow/test/
--rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/test/__init__.py
--rw-rw-rw-   0        0        0     3013 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/redox_flow/test/test_stack_module.py
--rw-rw-rw-   0        0        0     2749 2023-02-20 12:50:47.000000 simses-1.3.3/simses/technology/storage.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:23.499349 simses-1.3.4/
+-rw-rw-rw-   0        0        0     1647 2023-02-10 09:26:04.000000 simses-1.3.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      158 2023-02-08 12:59:18.000000 simses-1.3.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1790 2023-05-16 15:07:23.495342 simses-1.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1184 2023-05-16 10:48:41.000000 simses-1.3.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:19.201272 simses-1.3.4/doc/
+-rw-rw-rw-   0        0        0        0 2023-02-07 13:10:46.000000 simses-1.3.4/doc/__init__.py
+-rw-rw-rw-   0        0        0     2915 2023-02-07 13:10:47.000000 simses-1.3.4/doc/conf.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:19.224264 simses-1.3.4/doc/graph/
+-rw-rw-rw-   0        0        0        0 2023-02-07 13:10:47.000000 simses-1.3.4/doc/graph/__init__.py
+-rw-rw-rw-   0        0        0     4830 2023-02-07 13:10:47.000000 simses-1.3.4/doc/graph/graph.py
+-rw-rw-rw-   0        0        0     1067 2023-05-16 15:06:28.000000 simses-1.3.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-16 15:07:23.499349 simses-1.3.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:19.270266 simses-1.3.4/simses/
+-rw-rw-rw-   0        0        0        5 2023-05-16 15:05:40.000000 simses-1.3.4/simses/VERSION
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.4/simses/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:19.361265 simses-1.3.4/simses/analysis/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.4/simses/analysis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:19.403266 simses-1.3.4/simses/analysis/data/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.4/simses/analysis/data/__init__.py
+-rw-rw-rw-   0        0        0    10671 2023-02-20 12:50:46.000000 simses-1.3.4/simses/analysis/data/abstract_data.py
+-rw-rw-rw-   0        0        0     6060 2023-02-20 12:50:46.000000 simses-1.3.4/simses/analysis/data/electrolyzer.py
+-rw-rw-rw-   0        0        0     1980 2023-02-20 12:50:46.000000 simses-1.3.4/simses/analysis/data/energy_management.py
+-rw-rw-rw-   0        0        0     2543 2023-02-20 12:50:46.000000 simses-1.3.4/simses/analysis/data/fuel_cell.py
+-rw-rw-rw-   0        0        0     6598 2023-02-20 12:50:46.000000 simses-1.3.4/simses/analysis/data/hydrogen.py
+-rw-rw-rw-   0        0        0     3563 2023-03-06 13:30:03.000000 simses-1.3.4/simses/analysis/data/lithium_ion.py
+-rw-rw-rw-   0        0        0     3679 2023-02-20 12:50:46.000000 simses-1.3.4/simses/analysis/data/redox_flow.py
+-rw-rw-rw-   0        0        0     6714 2023-03-06 13:30:03.000000 simses-1.3.4/simses/analysis/data/system.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:19.420271 simses-1.3.4/simses/analysis/evaluation/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.4/simses/analysis/evaluation/__init__.py
+-rw-rw-rw-   0        0        0     5937 2023-02-20 12:50:46.000000 simses-1.3.4/simses/analysis/evaluation/abstract_evaluation.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:19.427269 simses-1.3.4/simses/analysis/evaluation/economic/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.4/simses/analysis/evaluation/economic/__init__.py
+-rw-rw-rw-   0        0        0     7935 2023-02-20 12:50:46.000000 simses-1.3.4/simses/analysis/evaluation/economic/economic_evaluation.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:19.469275 simses-1.3.4/simses/analysis/evaluation/economic/revenue_stream/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.4/simses/analysis/evaluation/economic/revenue_stream/__init__.py
+-rw-rw-rw-   0        0        0     3611 2023-02-20 12:50:46.000000 simses-1.3.4/simses/analysis/evaluation/economic/revenue_stream/abstract_revenue_stream.py
+-rw-rw-rw-   0        0        0    10705 2023-02-20 12:50:46.000000 simses-1.3.4/simses/analysis/evaluation/economic/revenue_stream/demand_charge_reduction.py
+-rw-rw-rw-   0        0        0     4503 2023-02-20 12:50:46.000000 simses-1.3.4/simses/analysis/evaluation/economic/revenue_stream/electricity_consumption.py
+-rw-rw-rw-   0        0        0     3452 2023-02-20 12:50:46.000000 simses-1.3.4/simses/analysis/evaluation/economic/revenue_stream/energy_cost_reduction.py
+-rw-rw-rw-   0        0        0     4318 2023-02-20 12:50:46.000000 simses-1.3.4/simses/analysis/evaluation/economic/revenue_stream/fcr_revenue_stream.py
+-rw-rw-rw-   0        0        0     4453 2023-03-06 13:30:03.000000 simses-1.3.4/simses/analysis/evaluation/economic/revenue_stream/intraday_recharge.py
+-rw-rw-rw-   0        0        0     2742 2023-02-20 12:50:46.000000 simses-1.3.4/simses/analysis/evaluation/economic/revenue_stream/operation_and_maintenance.py
+-rw-rw-rw-   0        0        0     5668 2023-03-06 13:30:03.000000 simses-1.3.4/simses/analysis/evaluation/merger.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:19.505268 simses-1.3.4/simses/analysis/evaluation/plotting/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.4/simses/analysis/evaluation/plotting/__init__.py
+-rw-rw-rw-   0        0        0      514 2023-02-20 12:50:46.000000 simses-1.3.4/simses/analysis/evaluation/plotting/axis.py
+-rw-rw-rw-   0        0        0     5130 2023-02-20 12:50:46.000000 simses-1.3.4/simses/analysis/evaluation/plotting/energy_plotting.py
+-rw-rw-rw-   0        0        0     3256 2023-02-20 12:50:46.000000 simses-1.3.4/simses/analysis/evaluation/plotting/matplot_plotting.py
+-rw-rw-rw-   0        0        0     7441 2023-02-20 12:50:46.000000 simses-1.3.4/simses/analysis/evaluation/plotting/plotly_plotting.py
+-rw-rw-rw-   0        0        0     4506 2023-02-20 12:50:46.000000 simses-1.3.4/simses/analysis/evaluation/plotting/plotter.py
+-rw-rw-rw-   0        0        0     7765 2023-02-20 12:50:46.000000 simses-1.3.4/simses/analysis/evaluation/plotting/sankey_diagram.py
+-rw-rw-rw-   0        0        0     5695 2023-02-20 12:50:46.000000 simses-1.3.4/simses/analysis/evaluation/plotting/sunburst_diagram.py
+-rw-rw-rw-   0        0        0    11357 2023-02-20 12:50:46.000000 simses-1.3.4/simses/analysis/evaluation/plotting/system_parameters.py
+-rw-rw-rw-   0        0        0     7539 2023-03-06 13:30:03.000000 simses-1.3.4/simses/analysis/evaluation/result.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:19.558267 simses-1.3.4/simses/analysis/evaluation/technical/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.4/simses/analysis/evaluation/technical/__init__.py
+-rw-rw-rw-   0        0        0    16301 2023-02-20 12:50:46.000000 simses-1.3.4/simses/analysis/evaluation/technical/electrolyzer.py
+-rw-rw-rw-   0        0        0     4496 2023-02-20 12:50:46.000000 simses-1.3.4/simses/analysis/evaluation/technical/fuel_cell.py
+-rw-rw-rw-   0        0        0    16450 2023-02-20 12:50:46.000000 simses-1.3.4/simses/analysis/evaluation/technical/hydrogen.py
+-rw-rw-rw-   0        0        0     7977 2023-03-06 13:30:03.000000 simses-1.3.4/simses/analysis/evaluation/technical/lithium_ion.py
+-rw-rw-rw-   0        0        0     5943 2023-02-20 12:50:46.000000 simses-1.3.4/simses/analysis/evaluation/technical/redox_flow.py
+-rw-rw-rw-   0        0        0     9681 2023-02-20 12:50:46.000000 simses-1.3.4/simses/analysis/evaluation/technical/site_level.py
+-rw-rw-rw-   0        0        0    18811 2023-03-06 13:30:03.000000 simses-1.3.4/simses/analysis/evaluation/technical/system.py
+-rw-rw-rw-   0        0        0    11829 2023-02-20 12:50:46.000000 simses-1.3.4/simses/analysis/evaluation/technical/technical_evaluation.py
+-rw-rw-rw-   0        0        0    11807 2023-05-16 11:18:59.000000 simses-1.3.4/simses/analysis/factory.py
+-rw-rw-rw-   0        0        0     3346 2023-02-20 12:50:46.000000 simses-1.3.4/simses/analysis/storage.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:19.622766 simses-1.3.4/simses/analysis/test/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.4/simses/analysis/test/__init__.py
+-rw-rw-rw-   0        0        0     4929 2023-02-20 12:50:46.000000 simses-1.3.4/simses/analysis/test/test_demand_charge_reduction.py
+-rw-rw-rw-   0        0        0     3723 2023-02-20 12:50:46.000000 simses-1.3.4/simses/analysis/test/test_energy_cost_reduction.py
+-rw-rw-rw-   0        0        0     3268 2023-02-20 12:50:46.000000 simses-1.3.4/simses/analysis/test/test_fcr_revenue_stream.py
+-rw-rw-rw-   0        0        0     3356 2023-02-20 12:50:46.000000 simses-1.3.4/simses/analysis/test/test_intraday_recharge_revenue_stream.py
+-rw-rw-rw-   0        0        0    16978 2023-03-06 13:30:03.000000 simses-1.3.4/simses/analysis/test/test_technical_evaluation.py
+-rw-rw-rw-   0        0        0     1066 2023-02-20 12:50:46.000000 simses-1.3.4/simses/analysis/utils.py
+-rw-rw-rw-   0        0        0     1609 2023-02-20 12:50:46.000000 simses-1.3.4/simses/analysis.defaults.ini
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:19.643276 simses-1.3.4/simses/commons/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:19.655267 simses-1.3.4/simses/commons/config/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/config/__init__.py
+-rw-rw-rw-   0        0        0     4909 2023-03-06 13:30:03.000000 simses-1.3.4/simses/commons/config/abstract_config.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:19.674270 simses-1.3.4/simses/commons/config/analysis/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/config/analysis/__init__.py
+-rw-rw-rw-   0        0        0      549 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/config/analysis/analysis_config.py
+-rw-rw-rw-   0        0        0     5265 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/config/analysis/economic.py
+-rw-rw-rw-   0        0        0     4645 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/config/analysis/general.py
+-rw-rw-rw-   0        0        0     1138 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/config/analysis/market.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:19.705266 simses-1.3.4/simses/commons/config/data/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/config/data/__init__.py
+-rw-rw-rw-   0        0        0      742 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/config/data/auxiliary.py
+-rw-rw-rw-   0        0        0     7429 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/config/data/battery.py
+-rw-rw-rw-   0        0        0      571 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/config/data/data_config.py
+-rw-rw-rw-   0        0        0     2057 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/config/data/electrolyzer.py
+-rw-rw-rw-   0        0        0     1900 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/config/data/energy_management.py
+-rw-rw-rw-   0        0        0     1478 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/config/data/fuel_cell.py
+-rw-rw-rw-   0        0        0     1481 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/config/data/power_electronics.py
+-rw-rw-rw-   0        0        0     4119 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/config/data/redox_flow.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:19.717314 simses-1.3.4/simses/commons/config/generation/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/config/generation/__init__.py
+-rw-rw-rw-   0        0        0     6251 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/config/generation/analysis.py
+-rw-rw-rw-   0        0        0     2220 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/config/generation/generator.py
+-rw-rw-rw-   0        0        0    34101 2023-05-15 14:47:15.000000 simses-1.3.4/simses/commons/config/generation/simulation.py
+-rw-rw-rw-   0        0        0     1522 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/config/log.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:19.769822 simses-1.3.4/simses/commons/config/simulation/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/config/simulation/__init__.py
+-rw-rw-rw-   0        0        0     5452 2023-03-06 13:30:03.000000 simses-1.3.4/simses/commons/config/simulation/battery.py
+-rw-rw-rw-   0        0        0     1175 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/config/simulation/electrolyzer.py
+-rw-rw-rw-   0        0        0     5372 2023-05-15 14:47:15.000000 simses-1.3.4/simses/commons/config/simulation/energy_management.py
+-rw-rw-rw-   0        0        0     1144 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/config/simulation/fuel_cell.py
+-rw-rw-rw-   0        0        0     2203 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/config/simulation/general.py
+-rw-rw-rw-   0        0        0     4116 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/config/simulation/hydrogen.py
+-rw-rw-rw-   0        0        0     7818 2023-03-06 13:30:03.000000 simses-1.3.4/simses/commons/config/simulation/profile.py
+-rw-rw-rw-   0        0        0     1129 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/config/simulation/redox_flow.py
+-rw-rw-rw-   0        0        0     1388 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/config/simulation/simulation_config.py
+-rw-rw-rw-   0        0        0     6105 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/config/simulation/system.py
+-rw-rw-rw-   0        0        0     5887 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/console_printer.py
+-rw-rw-rw-   0        0        0     1775 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/constants.py
+-rw-rw-rw-   0        0        0     7169 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/csv_standard.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:19.804640 simses-1.3.4/simses/commons/cycle_detection/
+-rw-rw-rw-   0        0        0        2 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/cycle_detection/__init__.py
+-rw-rw-rw-   0        0        0     2347 2023-03-06 13:30:03.000000 simses-1.3.4/simses/commons/cycle_detection/cycle_detector.py
+-rw-rw-rw-   0        0        0     3294 2023-03-06 13:30:03.000000 simses-1.3.4/simses/commons/cycle_detection/half_cycle_detector.py
+-rw-rw-rw-   0        0        0      695 2023-03-06 13:30:03.000000 simses-1.3.4/simses/commons/cycle_detection/no_cycle_detector.py
+-rw-rw-rw-   0        0        0     6987 2023-03-06 13:30:03.000000 simses-1.3.4/simses/commons/cycle_detection/rainflow_cycle_detector.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:19.827443 simses-1.3.4/simses/commons/data/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/data/__init__.py
+-rw-rw-rw-   0        0        0     6798 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/data/csv_data_handler.py
+-rw-rw-rw-   0        0        0     1443 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/data/data_handler.py
+-rw-rw-rw-   0        0        0     1183 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/data/no_data_handler.py
+-rw-rw-rw-   0        0        0     1654 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/error.py
+-rw-rw-rw-   0        0        0     1820 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/log.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:19.843443 simses-1.3.4/simses/commons/profile/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/profile/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:19.873443 simses-1.3.4/simses/commons/profile/economic/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/profile/economic/__init__.py
+-rw-rw-rw-   0        0        0      493 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/profile/economic/constant.py
+-rw-rw-rw-   0        0        0      905 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/profile/economic/fcr.py
+-rw-rw-rw-   0        0        0      912 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/profile/economic/intraday.py
+-rw-rw-rw-   0        0        0      784 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/profile/economic/market.py
+-rw-rw-rw-   0        0        0    20695 2023-05-16 13:19:22.000000 simses-1.3.4/simses/commons/profile/file.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:19.938530 simses-1.3.4/simses/commons/profile/power/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/profile/power/__init__.py
+-rw-rw-rw-   0        0        0     1927 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/profile/power/alternating.py
+-rw-rw-rw-   0        0        0      808 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/profile/power/constant.py
+-rw-rw-rw-   0        0        0     1729 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/profile/power/file.py
+-rw-rw-rw-   0        0        0      966 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/profile/power/generation.py
+-rw-rw-rw-   0        0        0      953 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/profile/power/load.py
+-rw-rw-rw-   0        0        0      826 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/profile/power/power_profile.py
+-rw-rw-rw-   0        0        0     1974 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/profile/power/random.py
+-rw-rw-rw-   0        0        0      950 2023-03-06 13:30:03.000000 simses-1.3.4/simses/commons/profile/power/v2g_profile.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:19.978317 simses-1.3.4/simses/commons/profile/technical/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/profile/technical/__init__.py
+-rw-rw-rw-   0        0        0     1769 2023-03-06 13:30:03.000000 simses-1.3.4/simses/commons/profile/technical/binary.py
+-rw-rw-rw-   0        0        0     2367 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/profile/technical/frequency.py
+-rw-rw-rw-   0        0        0      756 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/profile/technical/soc.py
+-rw-rw-rw-   0        0        0      735 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/profile/technical/technical.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:20.011315 simses-1.3.4/simses/commons/state/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/state/__init__.py
+-rw-rw-rw-   0        0        0     6761 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/state/abstract_state.py
+-rw-rw-rw-   0        0        0     2777 2023-03-06 13:30:03.000000 simses-1.3.4/simses/commons/state/energy_management.py
+-rw-rw-rw-   0        0        0     2476 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/state/parameters.py
+-rw-rw-rw-   0        0        0    11708 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/state/parameters_reader.py
+-rw-rw-rw-   0        0        0     9283 2023-03-06 13:30:03.000000 simses-1.3.4/simses/commons/state/system.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:20.051513 simses-1.3.4/simses/commons/state/technology/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/state/technology/__init__.py
+-rw-rw-rw-   0        0        0    12642 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/state/technology/electrolyzer.py
+-rw-rw-rw-   0        0        0     6008 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/state/technology/fuel_cell.py
+-rw-rw-rw-   0        0        0     3675 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/state/technology/hydrogen.py
+-rw-rw-rw-   0        0        0    10784 2023-03-06 13:30:03.000000 simses-1.3.4/simses/commons/state/technology/lithium_ion.py
+-rw-rw-rw-   0        0        0     7185 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/state/technology/redox_flow.py
+-rw-rw-rw-   0        0        0     2550 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/state/technology/storage.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:20.073429 simses-1.3.4/simses/commons/test/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/test/__init__.py
+-rw-rw-rw-   0        0        0      702 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/test/test_constant_power_profile.py
+-rw-rw-rw-   0        0        0     2361 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/test/test_file_power_profile.py
+-rw-rw-rw-   0        0        0      849 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/test/test_linear_interpolation.py
+-rw-rw-rw-   0        0        0      814 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/test/test_mean_average.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:20.081770 simses-1.3.4/simses/commons/timeseries/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/timeseries/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:20.093737 simses-1.3.4/simses/commons/timeseries/average/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/timeseries/average/__init__.py
+-rw-rw-rw-   0        0        0      622 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/timeseries/average/average.py
+-rw-rw-rw-   0        0        0      507 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/timeseries/average/mean_average.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:20.125083 simses-1.3.4/simses/commons/timeseries/interpolation/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/timeseries/interpolation/__init__.py
+-rw-rw-rw-   0        0        0     1311 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/timeseries/interpolation/interpolation.py
+-rw-rw-rw-   0        0        0      782 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/timeseries/interpolation/last_value.py
+-rw-rw-rw-   0        0        0      565 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/timeseries/interpolation/linear_interpolation.py
+-rw-rw-rw-   0        0        0     1418 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/timeseries/timevalue.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:20.170051 simses-1.3.4/simses/commons/utils/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/utils/__init__.py
+-rw-rw-rw-   0        0        0     7923 2023-05-15 14:47:15.000000 simses-1.3.4/simses/commons/utils/cell_reader.py
+-rw-rw-rw-   0        0        0     2227 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/utils/converter_comparison.py
+-rw-rw-rw-   0        0        0     2092 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/utils/count_lines_of_code.py
+-rw-rw-rw-   0        0        0     5380 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/utils/fitting.py
+-rw-rw-rw-   0        0        0     5155 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/utils/heatmap.py
+-rw-rw-rw-   0        0        0     5198 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/utils/max_peak_shaving_limit.py
+-rw-rw-rw-   0        0        0     9471 2023-02-20 12:50:46.000000 simses-1.3.4/simses/commons/utils/utilities.py
+-rw-rw-rw-   0        0        0     4300 2023-05-15 14:47:15.000000 simses-1.3.4/simses/commons/utils/xml_reader.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:20.182368 simses-1.3.4/simses/data/
+-rw-rw-rw-   0        0        0       97 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:20.186367 simses-1.3.4/simses/data/electrolyzer/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/electrolyzer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:20.223869 simses-1.3.4/simses/data/electrolyzer/evaluation/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/electrolyzer/evaluation/__init__.py
+-rw-rw-rw-   0        0        0     3394 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/electrolyzer/evaluation/comparison_lut_ana_new_with_afterfitting.py
+-rw-rw-rw-   0        0        0     3816 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/electrolyzer/evaluation/comparison_lut_ana_new_without_afterfitting.py
+-rw-rw-rw-   0        0        0     3471 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/electrolyzer/evaluation/comparison_lut_no_current_influence_ana_new.py
+-rw-rw-rw-   0        0        0     6008 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/electrolyzer/evaluation/multi_dim_regression_current_dens_3rd_best_fit.py
+-rw-rw-rw-   0        0        0      336 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/electrolyzer/evaluation/parameters_multi_dim_current_dens_fit_3rd_bestfit.csv
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:20.284732 simses-1.3.4/simses/data/electrolyzer/lookuptable/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/electrolyzer/lookuptable/__init__.py
+-rw-rw-rw-   0        0        0     7662 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/electrolyzer/lookuptable/activation_overpotential_lookup_alkaline.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:20.344188 simses-1.3.4/simses/data/electrolyzer/lookuptable/archive/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/electrolyzer/lookuptable/archive/__init__.py
+-rw-rw-rw-   0        0        0  2333800 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/electrolyzer/lookuptable/archive/activation_overpotential_lookup_alkaline.csv.gz
+-rw-rw-rw-   0        0        0   367371 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/electrolyzer/lookuptable/archive/cell_currentdensity_lookup.csv.gz
+-rw-rw-rw-   0        0        0   347857 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/electrolyzer/lookuptable/archive/cell_voltage_lookup.csv.gz
+-rw-rw-rw-   0        0        0  1520365 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/electrolyzer/lookuptable/archive/cell_voltage_lookup_alkaline.csv.gz
+-rw-rw-rw-   0        0        0    29206 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/electrolyzer/lookuptable/archive/polarizationcurve_alkaline.py
+-rw-rw-rw-   0        0        0  1693681 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/electrolyzer/lookuptable/cell_current_lookup_alkaline.gz
+-rw-rw-rw-   0        0        0     5835 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/electrolyzer/lookuptable/multi_dim_polarizationcurve.py
+-rw-rw-rw-   0        0        0     5857 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/electrolyzer/lookuptable/multi_dim_polarizationcurve_no_current_influence_on_part_pressure.py
+-rw-rw-rw-   0        0        0    19149 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/electrolyzer/lookuptable/polarizationcurve1bar.csv
+-rw-rw-rw-   0        0        0     3910 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/electrolyzer/lookuptable/polarizationcurve_e_master.py
+-rw-rw-rw-   0        0        0    18991 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/electrolyzer/lookuptable/powercurve1bar.csv
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:20.352366 simses-1.3.4/simses/data/electrolyzer/lookuptable/ui_curves/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/electrolyzer/lookuptable/ui_curves/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:20.374984 simses-1.3.4/simses/data/electrolyzer/lookuptable/ui_curves/activation_overpotential_alkaline/
+-rw-rw-rw-   0        0        0      909 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/electrolyzer/lookuptable/ui_curves/activation_overpotential_alkaline/25°C.csv
+-rw-rw-rw-   0        0        0      919 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/electrolyzer/lookuptable/ui_curves/activation_overpotential_alkaline/90°C.csv
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/electrolyzer/lookuptable/ui_curves/activation_overpotential_alkaline/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:20.389036 simses-1.3.4/simses/data/electrolyzer/lookuptable/ui_curves/general_alkaline/
+-rw-rw-rw-   0        0        0     1084 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/electrolyzer/lookuptable/ui_curves/general_alkaline/GHW 130°C at 30bar.csv
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/electrolyzer/lookuptable/ui_curves/general_alkaline/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:20.426320 simses-1.3.4/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/
+-rw-rw-rw-   0        0        0     1324 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/23°C.csv
+-rw-rw-rw-   0        0        0     1365 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/35°C.csv
+-rw-rw-rw-   0        0        0     1416 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/40°C.csv
+-rw-rw-rw-   0        0        0     1479 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/45°C.csv
+-rw-rw-rw-   0        0        0     1530 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/53,5°C.csv
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:20.441483 simses-1.3.4/simses/data/electrolyzer/parameters/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/electrolyzer/parameters/__init__.py
+-rw-rw-rw-   0        0        0      221 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/electrolyzer/parameters/parameters_alkaline_overvoltage_fit.csv
+-rw-rw-rw-   0        0        0      299 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/electrolyzer/parameters/parameters_multi_dim_current_dens_fit.csv
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:20.471844 simses-1.3.4/simses/data/electrolyzer/regression/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/electrolyzer/regression/__init__.py
+-rw-rw-rw-   0        0        0  1943227 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/electrolyzer/regression/cell_currentdensity_lookup.csv
+-rw-rw-rw-   0        0        0     5615 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/electrolyzer/regression/multi_dim_regression_current_dens.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:20.475449 simses-1.3.4/simses/data/energy_management/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/energy_management/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:20.527160 simses-1.3.4/simses/data/fuel_cell/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/fuel_cell/__init__.py
+-rw-rw-rw-   0        0        0    19570 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/fuel_cell/polarizationcurve1bar.csv
+-rw-rw-rw-   0        0        0     9977 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/fuel_cell/polarizationcurve_fc_jupiter.py
+-rw-rw-rw-   0        0        0     3857 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/fuel_cell/polarizationcurve_fc_master.py
+-rw-rw-rw-   0        0        0    35785 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/fuel_cell/polarizationcurve_jupiter.csv
+-rw-rw-rw-   0        0        0    19746 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/fuel_cell/powercurve1bar.csv
+-rw-rw-rw-   0        0        0    36366 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/fuel_cell/powercurve_jupiter.csv
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:20.542729 simses-1.3.4/simses/data/lithium_ion/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data/lithium_ion/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:20.754383 simses-1.3.4/simses/data/lithium_ion/cell/
+-rw-rw-rw-   0        0        0   338005 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/lithium_ion/cell/CLFP_Sony_US26650_OCV.csv
+-rw-rw-rw-   0        0        0     1482 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/lithium_ion/cell/CLFP_Sony_US26650_Rint.csv
+-rw-rw-rw-   0        0        0      581 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/lithium_ion/cell/CLFP_Sony_US26650_capacity_decrease_param.csv
+-rw-rw-rw-   0        0        0      605 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/lithium_ion/cell/CLFP_Sony_US26650_resistance_increase_param.csv
+-rw-rw-rw-   0        0        0     2487 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/lithium_ion/cell/LG_INR18560MJ1_OCV.csv
+-rw-rw-rw-   0        0        0    16185 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/lithium_ion/cell/LG_INR18650MJ1_closs_calendar_aging.csv
+-rw-rw-rw-   0        0        0    14576 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/lithium_ion/cell/LG_INR18650MJ1_closs_cycling_aging.csv
+-rw-rw-rw-   0        0        0     7990 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/lithium_ion/cell/LG_INR18650MJ1_rint_cycling_aging.csv
+-rw-rw-rw-   0        0        0     2919 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/lithium_ion/cell/LTO_LMO_closs_cycling_aging.csv
+-rw-rw-rw-   0        0        0     2963 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/lithium_ion/cell/LTO_LMO_rint_cycling_aging.csv
+-rw-rw-rw-   0        0        0     1126 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/lithium_ion/cell/LTO_NMC_closs_calendar_aging.csv
+-rw-rw-rw-   0        0        0     2144 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/lithium_ion/cell/LTO_NMC_closs_cycling_aging.csv
+-rw-rw-rw-   0        0        0     2284 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/lithium_ion/cell/LTO_NMC_rint_calendar_aging.csv
+-rw-rw-rw-   0        0        0     1288 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/lithium_ion/cell/LTO_NMC_rint_cycling_aging.csv
+-rw-rw-rw-   0        0        0     4849 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/lithium_ion/cell/NCA_PanasonicNCR_OCV.csv
+-rw-rw-rw-   0        0        0    12237 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/lithium_ion/cell/NCA_PanasonicNCR_Rint.csv
+-rw-rw-rw-   0        0        0     1068 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/lithium_ion/cell/NMC_Akasol_OEM_Rint.csv
+-rw-rw-rw-   0        0        0     2384 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/lithium_ion/cell/NMC_Molicel_OCV.csv
+-rw-rw-rw-   0        0        0    12168 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/lithium_ion/cell/NMC_Molicel_Rint.csv
+-rw-rw-rw-   0        0        0    92642 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/lithium_ion/cell/NMC_Molicel_capacity_cal.csv
+-rw-rw-rw-   0        0        0    24959 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/lithium_ion/cell/NMC_Molicel_capacity_cyc.csv
+-rw-rw-rw-   0        0        0    80843 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/lithium_ion/cell/NMC_Molicel_ri_cal.csv
+-rw-rw-rw-   0        0        0    25392 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/lithium_ion/cell/NMC_Molicel_ri_cyc.csv
+-rw-rw-rw-   0        0        0    49004 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/lithium_ion/cell/NMC_Samsung_LabTest_cell_00_OCV.csv
+-rw-rw-rw-   0        0        0    15435 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/lithium_ion/cell/NMC_Samsung_LabTest_cell_00_Ri.csv
+-rw-rw-rw-   0        0        0      604 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/lithium_ion/cell/NMC_Sanyo_OCV.csv
+-rw-rw-rw-   0        0        0    12168 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/lithium_ion/cell/NMC_Sanyo_Rint.csv
+-rw-rw-rw-   0        0        0     2979 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/lithium_ion/cell/Sodium_Ion_OCV_Green_Rock.csv
+-rw-rw-rw-   0        0        0     4940 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/lithium_ion/cell/Sodium_Ion_Rint_Green_Rock.csv
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/lithium_ion/cell/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:20.757681 simses-1.3.4/simses/data/lithium_ion/isea/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/lithium_ion/isea/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:20.770361 simses-1.3.4/simses/data/logo/
+-rw-rw-rw-   0        0        0    36954 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/logo/SimSES.png
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/logo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:20.777353 simses-1.3.4/simses/data/power_electronics/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/power_electronics/__init__.py
+-rw-rw-rw-   0        0        0    29262 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/power_electronics/sinamics_S120_efficiency.csv
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:20.783287 simses-1.3.4/simses/data/profile/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/profile/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:20.789164 simses-1.3.4/simses/data/profile/economic/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/profile/economic/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:20.799567 simses-1.3.4/simses/data/profile/power/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/profile/power/__init__.py
+-rw-rw-rw-   0        0        0       41 2023-05-16 11:42:41.000000 simses-1.3.4/simses/data/profile/power/mockup_power_load_profile.csv
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:20.870873 simses-1.3.4/simses/data/profile/technical/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/profile/technical/__init__.py
+-rw-rw-rw-   0        0        0       46 2023-05-16 11:43:00.000000 simses-1.3.4/simses/data/profile/technical/mockup_power_home_profile.csv
+-rw-rw-rw-   0        0        0       58 2023-05-16 11:43:00.000000 simses-1.3.4/simses/data/profile/technical/mockup_power_soc_profile.csv
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:20.874787 simses-1.3.4/simses/data/profile/thermal/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/profile/thermal/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:20.883940 simses-1.3.4/simses/data/pump/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/pump/__init__.py
+-rw-rw-rw-   0        0        0      369 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/pump/pump_efficiency_renner_RM1_5_35.csv
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:20.888206 simses-1.3.4/simses/data/redox_flow/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/redox_flow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:21.005495 simses-1.3.4/simses/data/redox_flow/degradation/
+-rw-rw-rw-   0        0        0      560 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/redox_flow/degradation/H2_Current_F1_Schweiss.csv
+-rw-rw-rw-   0        0        0      290 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/redox_flow/degradation/H2_Current_F2_Schweiss.csv
+-rw-rw-rw-   0        0        0      560 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/redox_flow/degradation/H2_Current_F3_Schweiss.csv
+-rw-rw-rw-   0        0        0      243 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/redox_flow/degradation/H2_Current_F4_Schweiss.csv
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/redox_flow/degradation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:21.076178 simses-1.3.4/simses/data/redox_flow/stack/
+-rw-rw-rw-   0        0        0      509 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/redox_flow/stack/RFB_cell_data_R.csv
+-rw-rw-rw-   0        0        0      343 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/redox_flow/stack/RFB_highperformance_stack_R.csv
+-rw-rw-rw-   0        0        0       80 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/redox_flow/stack/SD_HP_Stack.csv
+-rw-rw-rw-   0        0        0     2731 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/redox_flow/stack/SHUNT_CellStack_2250_40.csv
+-rw-rw-rw-   0        0        0    28277 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/redox_flow/stack/SHUNT_FILE_INDUSTRIAL_STACK_1500W.csv
+-rw-rw-rw-   0        0        0    28360 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/redox_flow/stack/SHUNT_FILE_INDUSTRIAL_STACK_9000W.csv
+-rw-rw-rw-   0        0        0     5079 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/redox_flow/stack/SHUNT_HP_Stack.csv
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/data/redox_flow/stack/__init__.py
+-rw-rw-rw-   0        0        0     4214 2023-02-20 12:50:46.000000 simses-1.3.4/simses/data.defaults.ini
+-rw-rw-rw-   0        0        0      571 2023-02-20 12:50:47.000000 simses-1.3.4/simses/logger.defaults.ini
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:21.083571 simses-1.3.4/simses/logic/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/logic/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:21.105559 simses-1.3.4/simses/logic/energy_management/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/logic/energy_management/__init__.py
+-rw-rw-rw-   0        0        0    10719 2023-05-16 12:36:02.000000 simses-1.3.4/simses/logic/energy_management/energy_management_factory.py
+-rw-rw-rw-   0        0        0     2470 2023-03-06 13:30:03.000000 simses-1.3.4/simses/logic/energy_management/energy_management_system.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:21.120412 simses-1.3.4/simses/logic/energy_management/strategy/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/logic/energy_management/strategy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:21.206303 simses-1.3.4/simses/logic/energy_management/strategy/basic/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/logic/energy_management/strategy/basic/__init__.py
+-rw-rw-rw-   0        0        0     9246 2023-05-15 14:47:15.000000 simses-1.3.4/simses/logic/energy_management/strategy/basic/electric_vehicle.py
+-rw-rw-rw-   0        0        0    13078 2023-05-15 14:47:15.000000 simses-1.3.4/simses/logic/energy_management/strategy/basic/electric_vehicle_soc.py
+-rw-rw-rw-   0        0        0     9891 2023-03-06 13:30:03.000000 simses-1.3.4/simses/logic/energy_management/strategy/basic/electric_vehicle_v2g.py
+-rw-rw-rw-   0        0        0     2234 2023-02-20 12:50:47.000000 simses-1.3.4/simses/logic/energy_management/strategy/basic/ev_charger_with_buffer.py
+-rw-rw-rw-   0        0        0     5761 2023-02-20 12:50:47.000000 simses-1.3.4/simses/logic/energy_management/strategy/basic/frequency_containment_reserve.py
+-rw-rw-rw-   0        0        0     4102 2023-02-20 12:50:47.000000 simses-1.3.4/simses/logic/energy_management/strategy/basic/intraday_market_recharge.py
+-rw-rw-rw-   0        0        0     7724 2023-02-20 12:50:47.000000 simses-1.3.4/simses/logic/energy_management/strategy/basic/peak_shaving_perfect_foresight.py
+-rw-rw-rw-   0        0        0     2541 2023-02-20 12:50:47.000000 simses-1.3.4/simses/logic/energy_management/strategy/basic/peak_shaving_simple.py
+-rw-rw-rw-   0        0        0     1310 2023-05-15 14:47:15.000000 simses-1.3.4/simses/logic/energy_management/strategy/basic/power_follower.py
+-rw-rw-rw-   0        0        0     5407 2023-05-15 14:47:15.000000 simses-1.3.4/simses/logic/energy_management/strategy/basic/residential_pv_feed_in_damp.py
+-rw-rw-rw-   0        0        0     1807 2023-02-20 12:50:47.000000 simses-1.3.4/simses/logic/energy_management/strategy/basic/residential_pv_greedy.py
+-rw-rw-rw-   0        0        0     1489 2023-02-20 12:50:47.000000 simses-1.3.4/simses/logic/energy_management/strategy/basic/soc_follower.py
+-rw-rw-rw-   0        0        0     1501 2023-02-20 12:50:47.000000 simses-1.3.4/simses/logic/energy_management/strategy/basic/use_all_renewable_energy.py
+-rw-rw-rw-   0        0        0      281 2023-02-20 12:50:47.000000 simses-1.3.4/simses/logic/energy_management/strategy/operation_priority.py
+-rw-rw-rw-   0        0        0     2041 2023-02-20 12:50:47.000000 simses-1.3.4/simses/logic/energy_management/strategy/operation_strategy.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:21.212180 simses-1.3.4/simses/logic/energy_management/strategy/optimization/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/logic/energy_management/strategy/optimization/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:21.216524 simses-1.3.4/simses/logic/energy_management/strategy/optimization/forecast_utils/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/logic/energy_management/strategy/optimization/forecast_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:21.226501 simses-1.3.4/simses/logic/energy_management/strategy/optimization/linearized_models/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/logic/energy_management/strategy/optimization/linearized_models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:21.232144 simses-1.3.4/simses/logic/energy_management/strategy/serial/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/logic/energy_management/strategy/serial/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:21.244324 simses-1.3.4/simses/logic/energy_management/strategy/stacked/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/logic/energy_management/strategy/stacked/__init__.py
+-rw-rw-rw-   0        0        0     1132 2023-02-20 12:50:47.000000 simses-1.3.4/simses/logic/energy_management/strategy/stacked/fcr_idm_recharge_stacked.py
+-rw-rw-rw-   0        0        0     1198 2023-03-06 13:30:03.000000 simses-1.3.4/simses/logic/energy_management/strategy/stacked/stacked_operation_strategy.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:21.291125 simses-1.3.4/simses/logic/power_distribution/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/logic/power_distribution/__init__.py
+-rw-rw-rw-   0        0        0     3038 2023-02-20 12:50:47.000000 simses-1.3.4/simses/logic/power_distribution/efficient.py
+-rw-rw-rw-   0        0        0      626 2023-02-20 12:50:47.000000 simses-1.3.4/simses/logic/power_distribution/equal.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:21.295135 simses-1.3.4/simses/logic/power_distribution/optimization_utils/
+-rw-rw-rw-   0        0        0       46 2023-03-06 13:30:03.000000 simses-1.3.4/simses/logic/power_distribution/optimization_utils/__init__.py
+-rw-rw-rw-   0        0        0     1475 2023-02-20 12:50:47.000000 simses-1.3.4/simses/logic/power_distribution/power_distributor.py
+-rw-rw-rw-   0        0        0     1500 2023-02-20 12:50:47.000000 simses-1.3.4/simses/logic/power_distribution/soc.py
+-rw-rw-rw-   0        0        0     4106 2023-02-20 12:50:47.000000 simses-1.3.4/simses/logic/power_distribution/state.py
+-rw-rw-rw-   0        0        0     9364 2023-02-20 12:50:47.000000 simses-1.3.4/simses/logic/power_distribution/technology.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:21.364977 simses-1.3.4/simses/logic/test/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/logic/test/__init__.py
+-rw-rw-rw-   0        0        0     5066 2023-05-16 11:40:09.000000 simses-1.3.4/simses/logic/test/test_electric_vehicle_SOC_meanpower.py
+-rw-rw-rw-   0        0        0     4951 2023-05-16 11:42:11.000000 simses-1.3.4/simses/logic/test/test_electric_vehicle_SOC_original.py
+-rw-rw-rw-   0        0        0     5032 2023-05-16 11:41:52.000000 simses-1.3.4/simses/logic/test/test_electric_vehicle_SOC_paused.py
+-rw-rw-rw-   0        0        0     4815 2023-05-16 11:41:31.000000 simses-1.3.4/simses/logic/test/test_electric_vehicle_SOC_uncontrolled.py
+-rw-rw-rw-   0        0        0     5481 2023-02-20 12:50:47.000000 simses-1.3.4/simses/logic/test/test_electric_vehicle_all_strategies.py
+-rw-rw-rw-   0        0        0     4726 2023-05-16 11:42:40.000000 simses-1.3.4/simses/logic/test/test_electric_vehicle_uncontrolled.py
+-rw-rw-rw-   0        0        0     1181 2023-02-20 12:50:47.000000 simses-1.3.4/simses/logic/test/test_equal_power_distributor.py
+-rw-rw-rw-   0        0        0    21492 2023-03-06 13:30:03.000000 simses-1.3.4/simses/logic/test/test_multi_use.py
+-rw-rw-rw-   0        0        0     3169 2023-02-20 12:50:47.000000 simses-1.3.4/simses/logic/test/test_peak_shaving.py
+-rw-rw-rw-   0        0        0     3061 2023-02-20 12:50:47.000000 simses-1.3.4/simses/logic/test/test_residential_pv_greedy.py
+-rw-rw-rw-   0        0        0     1188 2023-02-20 12:50:47.000000 simses-1.3.4/simses/logic/test/test_soc_based_power_distributor.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:21.453386 simses-1.3.4/simses/logic/thermal_management/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/logic/thermal_management/__init__.py
+-rw-rw-rw-   0        0        0     4285 2023-02-20 12:50:47.000000 simses-1.3.4/simses/logic/thermal_management/on_off_controller.py
+-rw-rw-rw-   0        0        0     6005 2023-03-06 13:30:03.000000 simses-1.3.4/simses/logic/thermal_management/pid_controller.py
+-rw-rw-rw-   0        0        0       77 2023-02-20 12:50:47.000000 simses-1.3.4/simses/logic/thermal_management/thermal_management.py
+-rw-rw-rw-   0        0        0    10214 2023-05-15 14:47:15.000000 simses-1.3.4/simses/main.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:21.478011 simses-1.3.4/simses/simulation/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/simulation/__init__.py
+-rw-rw-rw-   0        0        0     4368 2023-02-20 12:50:47.000000 simses-1.3.4/simses/simulation/batch_processing.py
+-rw-rw-rw-   0        0        0     2937 2023-02-20 12:50:47.000000 simses-1.3.4/simses/simulation/batch_simulation.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:21.496103 simses-1.3.4/simses/simulation/case_studies/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/simulation/case_studies/__init__.py
+-rw-rw-rw-   0        0        0     1419 2023-02-20 12:50:47.000000 simses-1.3.4/simses/simulation/case_studies/case_study_1_peak_shaving.py
+-rw-rw-rw-   0        0        0     1930 2023-02-20 12:50:47.000000 simses-1.3.4/simses/simulation/case_studies/case_study_2_fcr.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:21.499689 simses-1.3.4/simses/simulation/case_studies/configs/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/simulation/case_studies/configs/__init__.py
+-rw-rw-rw-   0        0        0     4090 2023-02-20 12:50:47.000000 simses-1.3.4/simses/simulation/example.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:21.518259 simses-1.3.4/simses/simulation/simbas/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/simulation/simbas/__init__.py
+-rw-rw-rw-   0        0        0     2534 2023-05-15 14:47:15.000000 simses-1.3.4/simses/simulation/simbas/room_tool_reader.py
+-rw-rw-rw-   0        0        0     5577 2023-05-15 14:47:15.000000 simses-1.3.4/simses/simulation/simbas/simbas.py
+-rw-rw-rw-   0        0        0    10046 2023-05-15 14:47:15.000000 simses-1.3.4/simses/simulation/simulator.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:21.526170 simses-1.3.4/simses/simulation/system_tests/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/simulation/system_tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:21.535562 simses-1.3.4/simses/simulation/system_tests/configs/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/simulation/system_tests/configs/__init__.py
+-rw-rw-rw-   0        0        0     4971 2023-02-20 12:50:47.000000 simses-1.3.4/simses/simulation/system_tests/system_test.py
+-rw-rw-rw-   0        0        0    14759 2023-05-15 14:47:15.000000 simses-1.3.4/simses/simulation.defaults.ini
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:21.561409 simses-1.3.4/simses/system/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:21.569832 simses-1.3.4/simses/system/auxiliary/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/auxiliary/__init__.py
+-rw-rw-rw-   0        0        0      889 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/auxiliary/auxiliary.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:21.587455 simses-1.3.4/simses/system/auxiliary/compression/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/auxiliary/compression/__init__.py
+-rw-rw-rw-   0        0        0     1088 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/auxiliary/compression/compressor.py
+-rw-rw-rw-   0        0        0     1080 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/auxiliary/compression/hydrogen_isentrop.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:21.600177 simses-1.3.4/simses/system/auxiliary/gas_drying/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/auxiliary/gas_drying/__init__.py
+-rw-rw-rw-   0        0        0      749 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/auxiliary/gas_drying/gas_dryer.py
+-rw-rw-rw-   0        0        0      946 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/auxiliary/gas_drying/hydrogen.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:21.626965 simses-1.3.4/simses/system/auxiliary/heating_ventilation_air_conditioning/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/auxiliary/heating_ventilation_air_conditioning/__init__.py
+-rw-rw-rw-   0        0        0     1530 2023-03-06 13:30:03.000000 simses-1.3.4/simses/system/auxiliary/heating_ventilation_air_conditioning/fan.py
+-rw-rw-rw-   0        0        0     4567 2023-03-06 13:30:03.000000 simses-1.3.4/simses/system/auxiliary/heating_ventilation_air_conditioning/fix_cop_hvac.py
+-rw-rw-rw-   0        0        0     1662 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/auxiliary/heating_ventilation_air_conditioning/hvac.py
+-rw-rw-rw-   0        0        0     1243 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/auxiliary/heating_ventilation_air_conditioning/no_hvac.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:21.651178 simses-1.3.4/simses/system/auxiliary/pump/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/auxiliary/pump/__init__.py
+-rw-rw-rw-   0        0        0     1810 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/auxiliary/pump/abstract_pump.py
+-rw-rw-rw-   0        0        0     1144 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/auxiliary/pump/fixeta_centrifugal.py
+-rw-rw-rw-   0        0        0     2178 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/auxiliary/pump/scalable_variable_eta_centrifugal.py
+-rw-rw-rw-   0        0        0     2300 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/auxiliary/pump/variable_eta_centrifugal.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:21.661405 simses-1.3.4/simses/system/auxiliary/water_heating/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/auxiliary/water_heating/__init__.py
+-rw-rw-rw-   0        0        0      924 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/auxiliary/water_heating/water_heater.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:21.693818 simses-1.3.4/simses/system/dc_coupling/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/dc_coupling/__init__.py
+-rw-rw-rw-   0        0        0      448 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/dc_coupling/bus_charging_dc_coupling.py
+-rw-rw-rw-   0        0        0      551 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/dc_coupling/bus_charging_profile.py
+-rw-rw-rw-   0        0        0     1643 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/dc_coupling/dc_coupler.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:21.715294 simses-1.3.4/simses/system/dc_coupling/generation/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/dc_coupling/generation/__init__.py
+-rw-rw-rw-   0        0        0      752 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/dc_coupling/generation/dc_generation.py
+-rw-rw-rw-   0        0        0      466 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/dc_coupling/generation/no_dc_generation.py
+-rw-rw-rw-   0        0        0     1330 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/dc_coupling/generation/pv_dc_generation.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:21.751673 simses-1.3.4/simses/system/dc_coupling/load/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/dc_coupling/load/__init__.py
+-rw-rw-rw-   0        0        0      980 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/dc_coupling/load/dc_bus_charging_fixed.py
+-rw-rw-rw-   0        0        0     1372 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/dc_coupling/load/dc_bus_charging_profile.py
+-rw-rw-rw-   0        0        0     2875 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/dc_coupling/load/dc_bus_charging_random.py
+-rw-rw-rw-   0        0        0      812 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/dc_coupling/load/dc_load.py
+-rw-rw-rw-   0        0        0     1058 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/dc_coupling/load/dc_radio_ups_load.py
+-rw-rw-rw-   0        0        0      444 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/dc_coupling/load/no_dc_load.py
+-rw-rw-rw-   0        0        0      327 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/dc_coupling/no_dc_coupling.py
+-rw-rw-rw-   0        0        0      747 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/dc_coupling/usp_dc_coupling.py
+-rw-rw-rw-   0        0        0    36968 2023-05-16 12:59:52.000000 simses-1.3.4/simses/system/factory.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:21.779008 simses-1.3.4/simses/system/housing/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/housing/__init__.py
+-rw-rw-rw-   0        0        0     2954 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/housing/abstract_housing.py
+-rw-rw-rw-   0        0        0     7225 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/housing/forty_ft_container.py
+-rw-rw-rw-   0        0        0     3281 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/housing/layer.py
+-rw-rw-rw-   0        0        0      453 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/housing/no_housing.py
+-rw-rw-rw-   0        0        0     7218 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/housing/twenty_ft_container.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:21.788927 simses-1.3.4/simses/system/power_electronics/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/power_electronics/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:21.853860 simses-1.3.4/simses/system/power_electronics/acdc_converter/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/power_electronics/acdc_converter/__init__.py
+-rw-rw-rw-   0        0        0     3531 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/power_electronics/acdc_converter/abstract_acdc_converter.py
+-rw-rw-rw-   0        0        0     4152 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/power_electronics/acdc_converter/bonfiglioli.py
+-rw-rw-rw-   0        0        0     2296 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/power_electronics/acdc_converter/fix_efficiency.py
+-rw-rw-rw-   0        0        0      407 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/power_electronics/acdc_converter/no_loss.py
+-rw-rw-rw-   0        0        0     3446 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/power_electronics/acdc_converter/notton.py
+-rw-rw-rw-   0        0        0     2821 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/power_electronics/acdc_converter/notton_loss.py
+-rw-rw-rw-   0        0        0     2459 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/power_electronics/acdc_converter/rampinelli_fit.py
+-rw-rw-rw-   0        0        0     3879 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/power_electronics/acdc_converter/sinamics.py
+-rw-rw-rw-   0        0        0     4198 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/power_electronics/acdc_converter/stable.py
+-rw-rw-rw-   0        0        0     4895 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/power_electronics/acdc_converter/stacked.py
+-rw-rw-rw-   0        0        0     8150 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/power_electronics/acdc_converter/sungrow.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:21.878370 simses-1.3.4/simses/system/power_electronics/dcdc_converter/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/power_electronics/dcdc_converter/__init__.py
+-rw-rw-rw-   0        0        0     2423 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/power_electronics/dcdc_converter/abstract_dcdc_converter.py
+-rw-rw-rw-   0        0        0     2775 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/power_electronics/dcdc_converter/fix_efficiency.py
+-rw-rw-rw-   0        0        0     2299 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/power_electronics/dcdc_converter/no_dcdc.py
+-rw-rw-rw-   0        0        0     1847 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/power_electronics/dcdc_converter/no_loss.py
+-rw-rw-rw-   0        0        0     6350 2023-03-06 13:30:03.000000 simses-1.3.4/simses/system/power_electronics/electronics.py
+-rw-rw-rw-   0        0        0     3725 2023-05-15 14:47:15.000000 simses-1.3.4/simses/system/storage_circuit.py
+-rw-rw-rw-   0        0        0    10030 2023-05-15 14:47:15.000000 simses-1.3.4/simses/system/storage_system_ac.py
+-rw-rw-rw-   0        0        0     5713 2023-03-06 13:30:03.000000 simses-1.3.4/simses/system/storage_system_dc.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:21.933259 simses-1.3.4/simses/system/test/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/test/__init__.py
+-rw-rw-rw-   0        0        0     7277 2023-05-16 11:19:36.000000 simses-1.3.4/simses/system/test/test_acdc_converter.py
+-rw-rw-rw-   0        0        0     1387 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/test/test_constant_ambient_temperature.py
+-rw-rw-rw-   0        0        0     3571 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/test/test_fix_cop_hvac.py
+-rw-rw-rw-   0        0        0      423 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/test/test_fixeta_centrifugal_pump.py
+-rw-rw-rw-   0        0        0     3846 2023-03-06 13:30:03.000000 simses-1.3.4/simses/system/test/test_location_ambient_temperature.py
+-rw-rw-rw-   0        0        0     1976 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/test/test_location_ambient_temperature_profile_check.py
+-rw-rw-rw-   0        0        0     4318 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/test/test_location_solar_irradiation_model.py
+-rw-rw-rw-   0        0        0     2801 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/test/test_location_solar_irradiation_model_profile_check.py
+-rw-rw-rw-   0        0        0     2274 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/test/test_notton_acdc_converter.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:21.941039 simses-1.3.4/simses/system/thermal/
+-rw-rw-rw-   0        0        0        2 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/thermal/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:21.969251 simses-1.3.4/simses/system/thermal/ambient/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/thermal/ambient/__init__.py
+-rw-rw-rw-   0        0        0     1325 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/thermal/ambient/ambient_thermal_model.py
+-rw-rw-rw-   0        0        0     1064 2023-05-15 14:47:15.000000 simses-1.3.4/simses/system/thermal/ambient/constant_temperature.py
+-rw-rw-rw-   0        0        0     1654 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/thermal/ambient/location_temperature.py
+-rw-rw-rw-   0        0        0     1585 2023-03-06 13:30:03.000000 simses-1.3.4/simses/system/thermal/ambient/user_battery_temperature.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:22.000665 simses-1.3.4/simses/system/thermal/model/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/thermal/model/__init__.py
+-rw-rw-rw-   0        0        0     3667 2023-03-06 13:30:03.000000 simses-1.3.4/simses/system/thermal/model/no_system_thermal_model.py
+-rw-rw-rw-   0        0        0     3095 2023-03-06 13:30:03.000000 simses-1.3.4/simses/system/thermal/model/system_thermal_model.py
+-rw-rw-rw-   0        0        0    15883 2023-03-06 13:30:03.000000 simses-1.3.4/simses/system/thermal/model/zero_d_room_thermal_model.py
+-rw-rw-rw-   0        0        0    24072 2023-03-06 13:30:03.000000 simses-1.3.4/simses/system/thermal/model/zero_d_system_thermal_model.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:22.056704 simses-1.3.4/simses/system/thermal/solar_irradiation/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/thermal/solar_irradiation/__init__.py
+-rw-rw-rw-   0        0        0    18001 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/thermal/solar_irradiation/location.py
+-rw-rw-rw-   0        0        0      795 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/thermal/solar_irradiation/no_solar_irradiation.py
+-rw-rw-rw-   0        0        0     1464 2023-02-20 12:50:47.000000 simses-1.3.4/simses/system/thermal/solar_irradiation/solar_irradiation_model.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:22.064839 simses-1.3.4/simses/technology/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:22.076903 simses-1.3.4/simses/technology/hydrogen/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:22.083399 simses-1.3.4/simses/technology/hydrogen/control/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/control/__init__.py
+-rw-rw-rw-   0        0        0     3315 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/control/management.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:22.124373 simses-1.3.4/simses/technology/hydrogen/control/pressure/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/control/pressure/__init__.py
+-rw-rw-rw-   0        0        0     3335 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/control/pressure/ideal_var_cathode.py
+-rw-rw-rw-   0        0        0      723 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/control/pressure/no_pressure_controller.py
+-rw-rw-rw-   0        0        0      791 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/control/pressure/pressure_controller.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:22.155715 simses-1.3.4/simses/technology/hydrogen/control/thermal/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/control/thermal/__init__.py
+-rw-rw-rw-   0        0        0     3633 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/control/thermal/ideal_var_flow.py
+-rw-rw-rw-   0        0        0      531 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/control/thermal/no_thermal_controller.py
+-rw-rw-rw-   0        0        0      795 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/control/thermal/thermal_controller.py
+-rw-rw-rw-   0        0        0     2522 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/control/thermal/var_flow.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:22.176487 simses-1.3.4/simses/technology/hydrogen/electrolyzer/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/electrolyzer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:22.211648 simses-1.3.4/simses/technology/hydrogen/electrolyzer/degradation/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/electrolyzer/degradation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:22.244159 simses-1.3.4/simses/technology/hydrogen/electrolyzer/degradation/calendar/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/electrolyzer/degradation/calendar/__init__.py
+-rw-rw-rw-   0        0        0     2105 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/electrolyzer/degradation/calendar/calendar_degradation.py
+-rw-rw-rw-   0        0        0      785 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/electrolyzer/degradation/calendar/no_calendar_degradation.py
+-rw-rw-rw-   0        0        0     3071 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/electrolyzer/degradation/calendar/pem_analytic.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:22.271525 simses-1.3.4/simses/technology/hydrogen/electrolyzer/degradation/cyclic/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/electrolyzer/degradation/cyclic/__init__.py
+-rw-rw-rw-   0        0        0     2123 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/electrolyzer/degradation/cyclic/cyclic_degradation.py
+-rw-rw-rw-   0        0        0      796 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/electrolyzer/degradation/cyclic/no_cyclic_degradation.py
+-rw-rw-rw-   0        0        0     4542 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/electrolyzer/degradation/cyclic/pem_analytic.py
+-rw-rw-rw-   0        0        0     1437 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/electrolyzer/degradation/cyclic/pem_analytic_ptl_coating.py
+-rw-rw-rw-   0        0        0     4502 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/electrolyzer/degradation/degradation_model.py
+-rw-rw-rw-   0        0        0      728 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/electrolyzer/degradation/no_degradation.py
+-rw-rw-rw-   0        0        0     1517 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/electrolyzer/degradation/pem_analytic.py
+-rw-rw-rw-   0        0        0     1575 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/electrolyzer/degradation/pem_analytic_ptl_coating.py
+-rw-rw-rw-   0        0        0     9672 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/electrolyzer/factory.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:22.295405 simses-1.3.4/simses/technology/hydrogen/electrolyzer/pressure/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/electrolyzer/pressure/__init__.py
+-rw-rw-rw-   0        0        0     1794 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/electrolyzer/pressure/abstract_model.py
+-rw-rw-rw-   0        0        0     2448 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/electrolyzer/pressure/alkaline.py
+-rw-rw-rw-   0        0        0     1802 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/electrolyzer/pressure/no_pressure_model.py
+-rw-rw-rw-   0        0        0     3656 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/electrolyzer/pressure/var_cathode.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:22.339576 simses-1.3.4/simses/technology/hydrogen/electrolyzer/stack/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/electrolyzer/stack/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:22.386652 simses-1.3.4/simses/technology/hydrogen/electrolyzer/stack/alkaline/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/electrolyzer/stack/alkaline/__init__.py
+-rw-rw-rw-   0        0        0    13091 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/electrolyzer/stack/alkaline/electrical_model.py
+-rw-rw-rw-   0        0        0     8273 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/electrolyzer/stack/alkaline/electrolyzer_model.py
+-rw-rw-rw-   0        0        0     1593 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/electrolyzer/stack/alkaline/fluid_model.py
+-rw-rw-rw-   0        0        0     1697 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/electrolyzer/stack/alkaline/parameters.py
+-rw-rw-rw-   0        0        0     1502 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/electrolyzer/stack/alkaline/pressure_model.py
+-rw-rw-rw-   0        0        0     1474 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/electrolyzer/stack/no_electrolyzer.py
+-rw-rw-rw-   0        0        0     4632 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/electrolyzer/stack/pem.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:22.477629 simses-1.3.4/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/__init__.py
+-rw-rw-rw-   0        0        0     5244 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/efficiency_curves.py
+-rw-rw-rw-   0        0        0     5765 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/electrical_model.py
+-rw-rw-rw-   0        0        0     8627 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/electrolyzer_model.py
+-rw-rw-rw-   0        0        0      603 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/electrolyzer_model_ptl_coating.py
+-rw-rw-rw-   0        0        0     2461 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/fluid_model.py
+-rw-rw-rw-   0        0        0     3649 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/membrane_model.py
+-rw-rw-rw-   0        0        0     2077 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/parameters.py
+-rw-rw-rw-   0        0        0     3318 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/pressure_model.py
+-rw-rw-rw-   0        0        0     5098 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/electrolyzer/stack/stack_model.py
+-rw-rw-rw-   0        0        0     5538 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/electrolyzer/system.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:22.504216 simses-1.3.4/simses/technology/hydrogen/electrolyzer/thermal/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/electrolyzer/thermal/__init__.py
+-rw-rw-rw-   0        0        0     1691 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/electrolyzer/thermal/abstract_model.py
+-rw-rw-rw-   0        0        0     8252 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/electrolyzer/thermal/alkaline.py
+-rw-rw-rw-   0        0        0     1352 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/electrolyzer/thermal/no_thermal_model.py
+-rw-rw-rw-   0        0        0    12898 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/electrolyzer/thermal/pem.py
+-rw-rw-rw-   0        0        0     2594 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/factory.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:22.525330 simses-1.3.4/simses/technology/hydrogen/fuel_cell/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/fuel_cell/__init__.py
+-rw-rw-rw-   0        0        0     5007 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/fuel_cell/factory.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:22.540349 simses-1.3.4/simses/technology/hydrogen/fuel_cell/pressure/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/fuel_cell/pressure/__init__.py
+-rw-rw-rw-   0        0        0     1527 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/fuel_cell/pressure/no_pressure.py
+-rw-rw-rw-   0        0        0     1766 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/fuel_cell/pressure/pressure_model.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:22.569481 simses-1.3.4/simses/technology/hydrogen/fuel_cell/stack/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/fuel_cell/stack/__init__.py
+-rw-rw-rw-   0        0        0     3734 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/fuel_cell/stack/jupiter.py
+-rw-rw-rw-   0        0        0     1208 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/fuel_cell/stack/no_fuel_cell.py
+-rw-rw-rw-   0        0        0     3141 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/fuel_cell/stack/pem.py
+-rw-rw-rw-   0        0        0     2232 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/fuel_cell/stack/stack_model.py
+-rw-rw-rw-   0        0        0     3181 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/fuel_cell/system.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:22.585598 simses-1.3.4/simses/technology/hydrogen/fuel_cell/thermal/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/fuel_cell/thermal/__init__.py
+-rw-rw-rw-   0        0        0      913 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/fuel_cell/thermal/no_thermal_model.py
+-rw-rw-rw-   0        0        0      963 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/fuel_cell/thermal/simple.py
+-rw-rw-rw-   0        0        0     1015 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/fuel_cell/thermal/thermal_model.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:22.601067 simses-1.3.4/simses/technology/hydrogen/hydrogen_storage/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/hydrogen_storage/__init__.py
+-rw-rw-rw-   0        0        0     1703 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/hydrogen_storage/hydrogen_storage.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:22.616323 simses-1.3.4/simses/technology/hydrogen/hydrogen_storage/pipeline/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/hydrogen_storage/pipeline/__init__.py
+-rw-rw-rw-   0        0        0      500 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/hydrogen_storage/pipeline/pipeline.py
+-rw-rw-rw-   0        0        0     1062 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/hydrogen_storage/pipeline/simple_pipeline.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:22.629059 simses-1.3.4/simses/technology/hydrogen/hydrogen_storage/pressuretank/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/hydrogen_storage/pressuretank/__init__.py
+-rw-rw-rw-   0        0        0     3899 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/hydrogen_storage/pressuretank/pressuretank.py
+-rw-rw-rw-   0        0        0     6240 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/system.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:22.639487 simses-1.3.4/simses/technology/hydrogen/test/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/test/__init__.py
+-rw-rw-rw-   0        0        0     8265 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/hydrogen/test/test_pem_electrolyzer.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:22.666477 simses-1.3.4/simses/technology/lithium_ion/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/__init__.py
+-rw-rw-rw-   0        0        0     6994 2023-03-06 13:30:03.000000 simses-1.3.4/simses/technology/lithium_ion/battery.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:22.676615 simses-1.3.4/simses/technology/lithium_ion/battery_management_system/
+-rw-rw-rw-   0        0        0        2 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/battery_management_system/__init__.py
+-rw-rw-rw-   0        0        0     7748 2023-03-06 13:30:03.000000 simses-1.3.4/simses/technology/lithium_ion/battery_management_system/management_system.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:22.791851 simses-1.3.4/simses/technology/lithium_ion/cell/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/cell/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:22.811238 simses-1.3.4/simses/technology/lithium_ion/cell/electric/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/cell/electric/__init__.py
+-rw-rw-rw-   0        0        0     1006 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/cell/electric/default.py
+-rw-rw-rw-   0        0        0     3550 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/cell/electric/properties.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:22.854078 simses-1.3.4/simses/technology/lithium_ion/cell/format/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/cell/format/__init__.py
+-rw-rw-rw-   0        0        0      829 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/cell/format/abstract.py
+-rw-rw-rw-   0        0        0      523 2023-03-06 13:30:03.000000 simses-1.3.4/simses/technology/lithium_ion/cell/format/pouch.py
+-rw-rw-rw-   0        0        0      555 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/cell/format/prismatic.py
+-rw-rw-rw-   0        0        0      593 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/cell/format/round.py
+-rw-rw-rw-   0        0        0      298 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/cell/format/round_18650.py
+-rw-rw-rw-   0        0        0      298 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/cell/format/round_26650.py
+-rw-rw-rw-   0        0        0     1952 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/cell/generic.py
+-rw-rw-rw-   0        0        0     4224 2023-05-15 14:47:15.000000 simses-1.3.4/simses/technology/lithium_ion/cell/isea.py
+-rw-rw-rw-   0        0        0     5009 2023-03-06 13:30:03.000000 simses-1.3.4/simses/technology/lithium_ion/cell/lfp_sony.py
+-rw-rw-rw-   0        0        0      503 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/cell/lfp_sony_generic.py
+-rw-rw-rw-   0        0        0     8685 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/cell/lmo_daimler.py
+-rw-rw-rw-   0        0        0     5224 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/cell/lto_lmo.py
+-rw-rw-rw-   0        0        0     5352 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/cell/lto_nmc.py
+-rw-rw-rw-   0        0        0      532 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/cell/nca_panasonic_generic.py
+-rw-rw-rw-   0        0        0     5469 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/cell/nca_panasonic_ncr.py
+-rw-rw-rw-   0        0        0     4958 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/cell/nmc_lgmj1.py
+-rw-rw-rw-   0        0        0     4514 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/cell/nmc_molicel.py
+-rw-rw-rw-   0        0        0      518 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/cell/nmc_molicel_generic.py
+-rw-rw-rw-   0        0        0     4931 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/cell/nmc_samsung78Ah.py
+-rw-rw-rw-   0        0        0     7991 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/cell/nmc_samsung94Ah.py
+-rw-rw-rw-   0        0        0     8558 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/cell/nmc_samsung94Ah_hybrid.py
+-rw-rw-rw-   0        0        0     5481 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/cell/nmc_sanyo_ur18650e.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:22.861200 simses-1.3.4/simses/technology/lithium_ion/cell/sodium_ion/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/cell/sodium_ion/__init__.py
+-rw-rw-rw-   0        0        0     5578 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/cell/sodium_ion/sodium_ion_green_rock.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:22.872137 simses-1.3.4/simses/technology/lithium_ion/cell/thermal/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/cell/thermal/__init__.py
+-rw-rw-rw-   0        0        0      639 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/cell/thermal/default.py
+-rw-rw-rw-   0        0        0     2131 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/cell/thermal/properties.py
+-rw-rw-rw-   0        0        0    16261 2023-03-06 13:30:03.000000 simses-1.3.4/simses/technology/lithium_ion/cell/type.py
+-rw-rw-rw-   0        0        0    15101 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/circuit.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:22.960690 simses-1.3.4/simses/technology/lithium_ion/degradation/
+-rw-rw-rw-   0        0        0        2 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/degradation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:23.041066 simses-1.3.4/simses/technology/lithium_ion/degradation/calendar/
+-rw-rw-rw-   0        0        0        2 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/degradation/calendar/__init__.py
+-rw-rw-rw-   0        0        0     3104 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/degradation/calendar/calendar_degradation.py
+-rw-rw-rw-   0        0        0     2364 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/degradation/calendar/generic_cell.py
+-rw-rw-rw-   0        0        0     2993 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/degradation/calendar/lfp_generic.py
+-rw-rw-rw-   0        0        0     5050 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/degradation/calendar/lfp_sony.py
+-rw-rw-rw-   0        0        0     3736 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/degradation/calendar/lto_lmo.py
+-rw-rw-rw-   0        0        0     3698 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/degradation/calendar/lto_nmc.py
+-rw-rw-rw-   0        0        0     2923 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/degradation/calendar/nca_generic.py
+-rw-rw-rw-   0        0        0     4689 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/degradation/calendar/nca_panasonicNCR.py
+-rw-rw-rw-   0        0        0     3063 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/degradation/calendar/nmc_generic.py
+-rw-rw-rw-   0        0        0     3077 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/degradation/calendar/nmc_lgmj1.py
+-rw-rw-rw-   0        0        0     4451 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/degradation/calendar/nmc_molicel.py
+-rw-rw-rw-   0        0        0     2914 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/degradation/calendar/nmc_sanyo_ur18650e.py
+-rw-rw-rw-   0        0        0      790 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/degradation/calendar/no_calendar_dedradation.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:23.169327 simses-1.3.4/simses/technology/lithium_ion/degradation/cyclic/
+-rw-rw-rw-   0        0        0        2 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/degradation/cyclic/__init__.py
+-rw-rw-rw-   0        0        0     3202 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/degradation/cyclic/cyclic_degradation.py
+-rw-rw-rw-   0        0        0     2316 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/degradation/cyclic/generic_cell.py
+-rw-rw-rw-   0        0        0     4820 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/degradation/cyclic/lfp_generic.py
+-rw-rw-rw-   0        0        0     5993 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/degradation/cyclic/lfp_sony.py
+-rw-rw-rw-   0        0        0     4560 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/degradation/cyclic/lto_lmo.py
+-rw-rw-rw-   0        0        0     4568 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/degradation/cyclic/lto_nmc.py
+-rw-rw-rw-   0        0        0     4173 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/degradation/cyclic/nca_generic.py
+-rw-rw-rw-   0        0        0     6795 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/degradation/cyclic/nca_panasonicNCR.py
+-rw-rw-rw-   0        0        0     4784 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/degradation/cyclic/nmc_generic.py
+-rw-rw-rw-   0        0        0     4700 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/degradation/cyclic/nmc_lgmj1.py
+-rw-rw-rw-   0        0        0     6373 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/degradation/cyclic/nmc_molicel.py
+-rw-rw-rw-   0        0        0     3885 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/degradation/cyclic/nmc_sanyo_ur18650e.py
+-rw-rw-rw-   0        0        0      764 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/degradation/cyclic/no_cyclic_degradation.py
+-rw-rw-rw-   0        0        0     8719 2023-03-06 13:30:03.000000 simses-1.3.4/simses/technology/lithium_ion/degradation/degradation_model.py
+-rw-rw-rw-   0        0        0      958 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/degradation/generic_cell.py
+-rw-rw-rw-   0        0        0      933 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/degradation/lfp_generic.py
+-rw-rw-rw-   0        0        0     1159 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/degradation/lfp_sony.py
+-rw-rw-rw-   0        0        0     1251 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/degradation/lmo_daimler.py
+-rw-rw-rw-   0        0        0      853 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/degradation/lto_lmo.py
+-rw-rw-rw-   0        0        0      853 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/degradation/lto_nmc.py
+-rw-rw-rw-   0        0        0      933 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/degradation/nca_generic.py
+-rw-rw-rw-   0        0        0      974 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/degradation/nca_panasonicNCR.py
+-rw-rw-rw-   0        0        0      933 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/degradation/nmc_generic.py
+-rw-rw-rw-   0        0        0      872 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/degradation/nmc_lgmj1.py
+-rw-rw-rw-   0        0        0     1103 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/degradation/nmc_molicel.py
+-rw-rw-rw-   0        0        0     1146 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/degradation/nmc_samsung94Ah.py
+-rw-rw-rw-   0        0        0      921 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/degradation/nmc_sanyo_ur18650e.py
+-rw-rw-rw-   0        0        0      804 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/degradation/no_degradation.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:23.198207 simses-1.3.4/simses/technology/lithium_ion/equivalent_circuit_model/
+-rw-rw-rw-   0        0        0        4 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/equivalent_circuit_model/__init__.py
+-rw-rw-rw-   0        0        0      527 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/equivalent_circuit_model/equivalent_circuit.py
+-rw-rw-rw-   0        0        0     1861 2023-03-06 13:30:03.000000 simses-1.3.4/simses/technology/lithium_ion/equivalent_circuit_model/rint_model.py
+-rw-rw-rw-   0        0        0    16756 2023-05-16 11:37:56.000000 simses-1.3.4/simses/technology/lithium_ion/factory.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:23.222082 simses-1.3.4/simses/technology/lithium_ion/test/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/test/__init__.py
+-rw-rw-rw-   0        0        0     2384 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/lithium_ion/test/test_battery.py
+-rw-rw-rw-   0        0        0     5158 2023-03-06 13:30:03.000000 simses-1.3.4/simses/technology/lithium_ion/test/test_bms.py
+-rw-rw-rw-   0        0        0     2797 2023-05-16 11:18:19.000000 simses-1.3.4/simses/technology/lithium_ion/test/test_type.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:23.240510 simses-1.3.4/simses/technology/redox_flow/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/redox_flow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:23.302137 simses-1.3.4/simses/technology/redox_flow/degradation/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/redox_flow/degradation/__init__.py
+-rw-rw-rw-   0        0        0     1657 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/redox_flow/degradation/capacity_degradation.py
+-rw-rw-rw-   0        0        0     2873 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/redox_flow/degradation/const_hydrogen_current.py
+-rw-rw-rw-   0        0        0      541 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/redox_flow/degradation/no_degradation.py
+-rw-rw-rw-   0        0        0     4209 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/redox_flow/degradation/variable_hydrogen_current.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:23.314074 simses-1.3.4/simses/technology/redox_flow/electrochemical/
+-rw-rw-rw-   0        0        0        4 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/redox_flow/electrochemical/__init__.py
+-rw-rw-rw-   0        0        0     1017 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/redox_flow/electrochemical/abstract_electrochemical.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:23.322605 simses-1.3.4/simses/technology/redox_flow/electrochemical/control/
+-rw-rw-rw-   0        0        0        2 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/redox_flow/electrochemical/control/__init__.py
+-rw-rw-rw-   0        0        0    10697 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/redox_flow/electrochemical/control/redox_control_system.py
+-rw-rw-rw-   0        0        0     8509 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/redox_flow/electrochemical/rint_model.py
+-rw-rw-rw-   0        0        0    17184 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/redox_flow/factory.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:23.387026 simses-1.3.4/simses/technology/redox_flow/pump_algorithm/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/redox_flow/pump_algorithm/__init__.py
+-rw-rw-rw-   0        0        0     4905 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/redox_flow/pump_algorithm/abstract_pump_algorithm.py
+-rw-rw-rw-   0        0        0     4324 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/redox_flow/pump_algorithm/constant_pressure_pulsed.py
+-rw-rw-rw-   0        0        0     3741 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/redox_flow/pump_algorithm/fix_flow_rate_start_stop.py
+-rw-rw-rw-   0        0        0     5153 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/redox_flow/pump_algorithm/stoich_flow_rate.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:23.448088 simses-1.3.4/simses/technology/redox_flow/stack/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/redox_flow/stack/__init__.py
+-rw-rw-rw-   0        0        0    10504 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/redox_flow/stack/abstract_stack.py
+-rw-rw-rw-   0        0        0     8549 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/redox_flow/stack/cell_data_stack_5500w.py
+-rw-rw-rw-   0        0        0     4627 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/redox_flow/stack/dummy_stack_3000w.py
+-rw-rw-rw-   0        0        0     4554 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/redox_flow/stack/dummy_stack_5500W.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:23.477579 simses-1.3.4/simses/technology/redox_flow/stack/electrolyte/
+-rw-rw-rw-   0        0        0        4 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/redox_flow/stack/electrolyte/__init__.py
+-rw-rw-rw-   0        0        0     3675 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/redox_flow/stack/electrolyte/abstract_electrolyte.py
+-rw-rw-rw-   0        0        0     4086 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/redox_flow/stack/electrolyte/vanadium.py
+-rw-rw-rw-   0        0        0     7211 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/redox_flow/stack/high_performance_stack_5700W.py
+-rw-rw-rw-   0        0        0     5787 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/redox_flow/stack/industrial_stack_1500w.py
+-rw-rw-rw-   0        0        0     5663 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/redox_flow/stack/industrial_stack_9000w.py
+-rw-rw-rw-   0        0        0    13481 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/redox_flow/system.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:23.490364 simses-1.3.4/simses/technology/redox_flow/test/
+-rw-rw-rw-   0        0        0        0 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/redox_flow/test/__init__.py
+-rw-rw-rw-   0        0        0     3013 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/redox_flow/test/test_stack_module.py
+-rw-rw-rw-   0        0        0     2749 2023-02-20 12:50:47.000000 simses-1.3.4/simses/technology/storage.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:07:19.341268 simses-1.3.4/simses.egg-info/
+-rw-rw-rw-   0        0        0     1790 2023-05-16 15:07:18.000000 simses-1.3.4/simses.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    34760 2023-05-16 15:07:18.000000 simses-1.3.4/simses.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 15:07:18.000000 simses-1.3.4/simses.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2023-05-16 15:07:18.000000 simses-1.3.4/simses.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-16 15:07:18.000000 simses-1.3.4/simses.egg-info/top_level.txt
```

### Comparing `simses-1.3.3/LICENSE.txt` & `simses-1.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/PKG-INFO` & `simses-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simses
-Version: 1.3.3
+Version: 1.3.4
 Summary: Simulation for Stationary Storage Systems (SimSES)
 Author-email: simses.ees@ed.tum.de
 License: BSD-3-Clause
 Project-URL: source, https://gitlab.lrz.de/open-ees-ses/simses
 Keywords: simulation,battery,energy,storage
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `simses-1.3.3/README.md` & `simses-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/pyproject.toml` & `simses-1.3.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -23,21 +23,19 @@
     "pandas",
     "plotly",
     "matplotlib",
     "pytz",
 ]
 dynamic = ["version"]
 
+[project.optional-dependencies]
+tests = ["pytest"]
+
 [project.urls]
 source = "https://gitlab.lrz.de/open-ees-ses/simses"
 
 [tool.setuptools]
+packages = ["simses"]
 include-package-data = true
 
 [tool.setuptools.dynamic]
 version = { file = "simses/VERSION" }
-
-[tool.setuptools.packages.find]
-where = ["simses"]
-
-[project.optional-dependencies]
-tests = ["pytest"]
```

### Comparing `simses-1.3.3/simses/analysis/data/abstract_data.py` & `simses-1.3.4/simses/analysis/data/abstract_data.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/analysis/data/electrolyzer.py` & `simses-1.3.4/simses/analysis/data/electrolyzer.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/analysis/data/energy_management.py` & `simses-1.3.4/simses/analysis/data/energy_management.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/analysis/data/fuel_cell.py` & `simses-1.3.4/simses/analysis/data/fuel_cell.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/analysis/data/hydrogen.py` & `simses-1.3.4/simses/analysis/data/hydrogen.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/analysis/data/lithium_ion.py` & `simses-1.3.4/simses/analysis/data/lithium_ion.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/analysis/data/redox_flow.py` & `simses-1.3.4/simses/analysis/data/redox_flow.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/analysis/data/system.py` & `simses-1.3.4/simses/analysis/data/system.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/analysis/evaluation/abstract_evaluation.py` & `simses-1.3.4/simses/analysis/evaluation/abstract_evaluation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/analysis/evaluation/economic/economic_evaluation.py` & `simses-1.3.4/simses/analysis/evaluation/economic/economic_evaluation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/analysis/evaluation/economic/revenue_stream/abstract_revenue_stream.py` & `simses-1.3.4/simses/analysis/evaluation/economic/revenue_stream/abstract_revenue_stream.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/analysis/evaluation/economic/revenue_stream/demand_charge_reduction.py` & `simses-1.3.4/simses/analysis/evaluation/economic/revenue_stream/demand_charge_reduction.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/analysis/evaluation/economic/revenue_stream/electricity_consumption.py` & `simses-1.3.4/simses/analysis/evaluation/economic/revenue_stream/electricity_consumption.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/analysis/evaluation/economic/revenue_stream/energy_cost_reduction.py` & `simses-1.3.4/simses/analysis/evaluation/economic/revenue_stream/energy_cost_reduction.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/analysis/evaluation/economic/revenue_stream/fcr_revenue_stream.py` & `simses-1.3.4/simses/analysis/evaluation/economic/revenue_stream/fcr_revenue_stream.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/analysis/evaluation/economic/revenue_stream/intraday_recharge.py` & `simses-1.3.4/simses/analysis/evaluation/economic/revenue_stream/intraday_recharge.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/analysis/evaluation/economic/revenue_stream/operation_and_maintenance.py` & `simses-1.3.4/simses/analysis/evaluation/economic/revenue_stream/operation_and_maintenance.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/analysis/evaluation/merger.py` & `simses-1.3.4/simses/analysis/evaluation/merger.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/analysis/evaluation/plotting/axis.py` & `simses-1.3.4/simses/analysis/evaluation/plotting/axis.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/analysis/evaluation/plotting/energy_plotting.py` & `simses-1.3.4/simses/analysis/evaluation/plotting/energy_plotting.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/analysis/evaluation/plotting/matplot_plotting.py` & `simses-1.3.4/simses/analysis/evaluation/plotting/matplot_plotting.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/analysis/evaluation/plotting/plotly_plotting.py` & `simses-1.3.4/simses/analysis/evaluation/plotting/plotly_plotting.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/analysis/evaluation/plotting/plotter.py` & `simses-1.3.4/simses/analysis/evaluation/plotting/plotter.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/analysis/evaluation/plotting/sankey_diagram.py` & `simses-1.3.4/simses/analysis/evaluation/plotting/sankey_diagram.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/analysis/evaluation/plotting/sunburst_diagram.py` & `simses-1.3.4/simses/analysis/evaluation/plotting/sunburst_diagram.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/analysis/evaluation/plotting/system_parameters.py` & `simses-1.3.4/simses/analysis/evaluation/plotting/system_parameters.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/analysis/evaluation/result.py` & `simses-1.3.4/simses/analysis/evaluation/result.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/analysis/evaluation/technical/electrolyzer.py` & `simses-1.3.4/simses/analysis/evaluation/technical/electrolyzer.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/analysis/evaluation/technical/fuel_cell.py` & `simses-1.3.4/simses/analysis/evaluation/technical/fuel_cell.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/analysis/evaluation/technical/hydrogen.py` & `simses-1.3.4/simses/analysis/evaluation/technical/hydrogen.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/analysis/evaluation/technical/lithium_ion.py` & `simses-1.3.4/simses/analysis/evaluation/technical/lithium_ion.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/analysis/evaluation/technical/redox_flow.py` & `simses-1.3.4/simses/analysis/evaluation/technical/redox_flow.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/analysis/evaluation/technical/site_level.py` & `simses-1.3.4/simses/analysis/evaluation/technical/site_level.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/analysis/evaluation/technical/system.py` & `simses-1.3.4/simses/analysis/evaluation/technical/system.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/analysis/evaluation/technical/technical_evaluation.py` & `simses-1.3.4/simses/analysis/evaluation/technical/technical_evaluation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/analysis/factory.py` & `simses-1.3.4/simses/analysis/factory.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/analysis/storage.py` & `simses-1.3.4/simses/analysis/storage.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/analysis/test/test_demand_charge_reduction.py` & `simses-1.3.4/simses/analysis/test/test_demand_charge_reduction.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/analysis/test/test_energy_cost_reduction.py` & `simses-1.3.4/simses/analysis/test/test_energy_cost_reduction.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/analysis/test/test_fcr_revenue_stream.py` & `simses-1.3.4/simses/analysis/test/test_fcr_revenue_stream.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/analysis/test/test_intraday_recharge_revenue_stream.py` & `simses-1.3.4/simses/analysis/test/test_intraday_recharge_revenue_stream.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/analysis/test/test_technical_evaluation.py` & `simses-1.3.4/simses/analysis/test/test_technical_evaluation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/analysis/utils.py` & `simses-1.3.4/simses/analysis/utils.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/analysis.defaults.ini` & `simses-1.3.4/simses/analysis.defaults.ini`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/config/abstract_config.py` & `simses-1.3.4/simses/commons/config/abstract_config.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/config/analysis/analysis_config.py` & `simses-1.3.4/simses/commons/config/analysis/analysis_config.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/config/analysis/economic.py` & `simses-1.3.4/simses/commons/config/analysis/economic.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/config/analysis/general.py` & `simses-1.3.4/simses/commons/config/analysis/general.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/config/analysis/market.py` & `simses-1.3.4/simses/commons/config/analysis/market.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/config/data/auxiliary.py` & `simses-1.3.4/simses/commons/config/data/auxiliary.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/config/data/battery.py` & `simses-1.3.4/simses/commons/config/data/battery.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/config/data/data_config.py` & `simses-1.3.4/simses/commons/config/data/data_config.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/config/data/electrolyzer.py` & `simses-1.3.4/simses/commons/config/data/electrolyzer.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/config/data/energy_management.py` & `simses-1.3.4/simses/commons/config/data/energy_management.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/config/data/fuel_cell.py` & `simses-1.3.4/simses/commons/config/data/fuel_cell.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/config/data/power_electronics.py` & `simses-1.3.4/simses/commons/config/data/power_electronics.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/config/data/redox_flow.py` & `simses-1.3.4/simses/commons/config/data/redox_flow.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/config/generation/analysis.py` & `simses-1.3.4/simses/commons/config/generation/analysis.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/config/generation/generator.py` & `simses-1.3.4/simses/commons/config/generation/generator.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/config/generation/simulation.py` & `simses-1.3.4/simses/commons/config/generation/simulation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/config/log.py` & `simses-1.3.4/simses/commons/config/log.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/config/simulation/battery.py` & `simses-1.3.4/simses/commons/config/simulation/battery.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/config/simulation/electrolyzer.py` & `simses-1.3.4/simses/commons/config/simulation/electrolyzer.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/config/simulation/energy_management.py` & `simses-1.3.4/simses/commons/config/simulation/energy_management.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/config/simulation/fuel_cell.py` & `simses-1.3.4/simses/commons/config/simulation/fuel_cell.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/config/simulation/general.py` & `simses-1.3.4/simses/commons/config/simulation/general.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/config/simulation/hydrogen.py` & `simses-1.3.4/simses/commons/config/simulation/hydrogen.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/config/simulation/profile.py` & `simses-1.3.4/simses/commons/config/simulation/profile.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/config/simulation/redox_flow.py` & `simses-1.3.4/simses/commons/config/simulation/redox_flow.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/config/simulation/simulation_config.py` & `simses-1.3.4/simses/commons/config/simulation/simulation_config.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/config/simulation/system.py` & `simses-1.3.4/simses/commons/config/simulation/system.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/console_printer.py` & `simses-1.3.4/simses/commons/console_printer.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/constants.py` & `simses-1.3.4/simses/commons/constants.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/csv_standard.py` & `simses-1.3.4/simses/commons/csv_standard.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/cycle_detection/cycle_detector.py` & `simses-1.3.4/simses/commons/cycle_detection/cycle_detector.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/cycle_detection/half_cycle_detector.py` & `simses-1.3.4/simses/commons/cycle_detection/half_cycle_detector.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/cycle_detection/no_cycle_detector.py` & `simses-1.3.4/simses/commons/cycle_detection/no_cycle_detector.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/cycle_detection/rainflow_cycle_detector.py` & `simses-1.3.4/simses/commons/cycle_detection/rainflow_cycle_detector.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/data/csv_data_handler.py` & `simses-1.3.4/simses/commons/data/csv_data_handler.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/data/data_handler.py` & `simses-1.3.4/simses/commons/data/data_handler.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/data/no_data_handler.py` & `simses-1.3.4/simses/commons/data/no_data_handler.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/error.py` & `simses-1.3.4/simses/commons/error.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/log.py` & `simses-1.3.4/simses/commons/log.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/profile/economic/fcr.py` & `simses-1.3.4/simses/commons/profile/economic/fcr.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/profile/economic/intraday.py` & `simses-1.3.4/simses/commons/profile/economic/intraday.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/profile/economic/market.py` & `simses-1.3.4/simses/commons/profile/economic/market.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/profile/file.py` & `simses-1.3.4/simses/commons/profile/file.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/profile/power/alternating.py` & `simses-1.3.4/simses/commons/profile/power/alternating.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/profile/power/constant.py` & `simses-1.3.4/simses/commons/profile/power/constant.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/profile/power/file.py` & `simses-1.3.4/simses/commons/profile/power/file.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/profile/power/generation.py` & `simses-1.3.4/simses/commons/profile/power/generation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/profile/power/load.py` & `simses-1.3.4/simses/commons/profile/power/load.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/profile/power/power_profile.py` & `simses-1.3.4/simses/commons/profile/power/power_profile.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/profile/power/random.py` & `simses-1.3.4/simses/commons/profile/power/random.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/profile/power/v2g_profile.py` & `simses-1.3.4/simses/commons/profile/power/v2g_profile.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/profile/technical/binary.py` & `simses-1.3.4/simses/commons/profile/technical/binary.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/profile/technical/frequency.py` & `simses-1.3.4/simses/commons/profile/technical/frequency.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/profile/technical/soc.py` & `simses-1.3.4/simses/commons/profile/technical/soc.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/profile/technical/technical.py` & `simses-1.3.4/simses/commons/profile/technical/technical.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/state/abstract_state.py` & `simses-1.3.4/simses/commons/state/abstract_state.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/state/energy_management.py` & `simses-1.3.4/simses/commons/state/energy_management.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/state/parameters.py` & `simses-1.3.4/simses/commons/state/parameters.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/state/parameters_reader.py` & `simses-1.3.4/simses/commons/state/parameters_reader.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/state/system.py` & `simses-1.3.4/simses/commons/state/system.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/state/technology/electrolyzer.py` & `simses-1.3.4/simses/commons/state/technology/electrolyzer.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/state/technology/fuel_cell.py` & `simses-1.3.4/simses/commons/state/technology/fuel_cell.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/state/technology/hydrogen.py` & `simses-1.3.4/simses/commons/state/technology/hydrogen.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/state/technology/lithium_ion.py` & `simses-1.3.4/simses/commons/state/technology/lithium_ion.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/state/technology/redox_flow.py` & `simses-1.3.4/simses/commons/state/technology/redox_flow.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/state/technology/storage.py` & `simses-1.3.4/simses/commons/state/technology/storage.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/test/test_constant_power_profile.py` & `simses-1.3.4/simses/commons/test/test_constant_power_profile.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/test/test_file_power_profile.py` & `simses-1.3.4/simses/commons/test/test_file_power_profile.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/test/test_linear_interpolation.py` & `simses-1.3.4/simses/commons/test/test_linear_interpolation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/test/test_mean_average.py` & `simses-1.3.4/simses/commons/test/test_mean_average.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/timeseries/average/average.py` & `simses-1.3.4/simses/commons/timeseries/average/average.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/timeseries/interpolation/interpolation.py` & `simses-1.3.4/simses/commons/timeseries/interpolation/interpolation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/timeseries/interpolation/last_value.py` & `simses-1.3.4/simses/commons/timeseries/interpolation/last_value.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/timeseries/interpolation/linear_interpolation.py` & `simses-1.3.4/simses/commons/timeseries/interpolation/linear_interpolation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/timeseries/timevalue.py` & `simses-1.3.4/simses/commons/timeseries/timevalue.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/utils/cell_reader.py` & `simses-1.3.4/simses/commons/utils/cell_reader.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/utils/converter_comparison.py` & `simses-1.3.4/simses/commons/utils/converter_comparison.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/utils/count_lines_of_code.py` & `simses-1.3.4/simses/commons/utils/count_lines_of_code.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/utils/fitting.py` & `simses-1.3.4/simses/commons/utils/fitting.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/utils/heatmap.py` & `simses-1.3.4/simses/commons/utils/heatmap.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/utils/max_peak_shaving_limit.py` & `simses-1.3.4/simses/commons/utils/max_peak_shaving_limit.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/utils/utilities.py` & `simses-1.3.4/simses/commons/utils/utilities.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/commons/utils/xml_reader.py` & `simses-1.3.4/simses/commons/utils/xml_reader.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/electrolyzer/evaluation/comparison_lut_ana_new_with_afterfitting.py` & `simses-1.3.4/simses/data/electrolyzer/evaluation/comparison_lut_ana_new_with_afterfitting.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/electrolyzer/evaluation/comparison_lut_ana_new_without_afterfitting.py` & `simses-1.3.4/simses/data/electrolyzer/evaluation/comparison_lut_ana_new_without_afterfitting.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/electrolyzer/evaluation/comparison_lut_no_current_influence_ana_new.py` & `simses-1.3.4/simses/data/electrolyzer/evaluation/comparison_lut_no_current_influence_ana_new.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/electrolyzer/evaluation/multi_dim_regression_current_dens_3rd_best_fit.py` & `simses-1.3.4/simses/data/electrolyzer/evaluation/multi_dim_regression_current_dens_3rd_best_fit.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/electrolyzer/lookuptable/activation_overpotential_lookup_alkaline.py` & `simses-1.3.4/simses/data/electrolyzer/lookuptable/activation_overpotential_lookup_alkaline.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/electrolyzer/lookuptable/archive/activation_overpotential_lookup_alkaline.csv.gz` & `simses-1.3.4/simses/data/electrolyzer/lookuptable/archive/activation_overpotential_lookup_alkaline.csv.gz`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/electrolyzer/lookuptable/archive/cell_currentdensity_lookup.csv.gz` & `simses-1.3.4/simses/data/electrolyzer/lookuptable/archive/cell_currentdensity_lookup.csv.gz`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/electrolyzer/lookuptable/archive/cell_voltage_lookup.csv.gz` & `simses-1.3.4/simses/data/electrolyzer/lookuptable/archive/cell_voltage_lookup.csv.gz`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/electrolyzer/lookuptable/archive/cell_voltage_lookup_alkaline.csv.gz` & `simses-1.3.4/simses/data/electrolyzer/lookuptable/archive/cell_voltage_lookup_alkaline.csv.gz`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/electrolyzer/lookuptable/archive/polarizationcurve_alkaline.py` & `simses-1.3.4/simses/data/electrolyzer/lookuptable/archive/polarizationcurve_alkaline.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/electrolyzer/lookuptable/cell_current_lookup_alkaline.gz` & `simses-1.3.4/simses/data/electrolyzer/lookuptable/cell_current_lookup_alkaline.gz`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/electrolyzer/lookuptable/multi_dim_polarizationcurve.py` & `simses-1.3.4/simses/data/electrolyzer/lookuptable/multi_dim_polarizationcurve.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/electrolyzer/lookuptable/multi_dim_polarizationcurve_no_current_influence_on_part_pressure.py` & `simses-1.3.4/simses/data/electrolyzer/lookuptable/multi_dim_polarizationcurve_no_current_influence_on_part_pressure.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/electrolyzer/lookuptable/polarizationcurve1bar.csv` & `simses-1.3.4/simses/data/electrolyzer/lookuptable/polarizationcurve1bar.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/electrolyzer/lookuptable/polarizationcurve_e_master.py` & `simses-1.3.4/simses/data/electrolyzer/lookuptable/polarizationcurve_e_master.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/electrolyzer/lookuptable/powercurve1bar.csv` & `simses-1.3.4/simses/data/electrolyzer/lookuptable/powercurve1bar.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/activation_overpotential_alkaline/25°C.csv` & `simses-1.3.4/simses/data/electrolyzer/lookuptable/ui_curves/activation_overpotential_alkaline/25°C.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/activation_overpotential_alkaline/90°C.csv` & `simses-1.3.4/simses/data/electrolyzer/lookuptable/ui_curves/activation_overpotential_alkaline/90°C.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/general_alkaline/GHW 130°C at 30bar.csv` & `simses-1.3.4/simses/data/electrolyzer/lookuptable/ui_curves/general_alkaline/GHW 130°C at 30bar.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/23°C.csv` & `simses-1.3.4/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/23°C.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/35°C.csv` & `simses-1.3.4/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/35°C.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/40°C.csv` & `simses-1.3.4/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/40°C.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/45°C.csv` & `simses-1.3.4/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/45°C.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/53,5°C.csv` & `simses-1.3.4/simses/data/electrolyzer/lookuptable/ui_curves/stuart_hri/53,5°C.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/electrolyzer/regression/cell_currentdensity_lookup.csv` & `simses-1.3.4/simses/data/electrolyzer/regression/cell_currentdensity_lookup.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/electrolyzer/regression/multi_dim_regression_current_dens.py` & `simses-1.3.4/simses/data/electrolyzer/regression/multi_dim_regression_current_dens.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/fuel_cell/polarizationcurve1bar.csv` & `simses-1.3.4/simses/data/fuel_cell/polarizationcurve1bar.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/fuel_cell/polarizationcurve_fc_jupiter.py` & `simses-1.3.4/simses/data/fuel_cell/polarizationcurve_fc_jupiter.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/fuel_cell/polarizationcurve_fc_master.py` & `simses-1.3.4/simses/data/fuel_cell/polarizationcurve_fc_master.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/fuel_cell/polarizationcurve_jupiter.csv` & `simses-1.3.4/simses/data/fuel_cell/polarizationcurve_jupiter.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/fuel_cell/powercurve1bar.csv` & `simses-1.3.4/simses/data/fuel_cell/powercurve1bar.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/fuel_cell/powercurve_jupiter.csv` & `simses-1.3.4/simses/data/fuel_cell/powercurve_jupiter.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/lithium_ion/cell/CLFP_Sony_US26650_OCV.csv` & `simses-1.3.4/simses/data/lithium_ion/cell/CLFP_Sony_US26650_OCV.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/lithium_ion/cell/CLFP_Sony_US26650_Rint.csv` & `simses-1.3.4/simses/data/lithium_ion/cell/CLFP_Sony_US26650_Rint.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/lithium_ion/cell/CLFP_Sony_US26650_capacity_decrease_param.csv` & `simses-1.3.4/simses/data/lithium_ion/cell/CLFP_Sony_US26650_capacity_decrease_param.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/lithium_ion/cell/CLFP_Sony_US26650_resistance_increase_param.csv` & `simses-1.3.4/simses/data/lithium_ion/cell/CLFP_Sony_US26650_resistance_increase_param.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/lithium_ion/cell/LG_INR18560MJ1_OCV.csv` & `simses-1.3.4/simses/data/lithium_ion/cell/LG_INR18560MJ1_OCV.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/lithium_ion/cell/LG_INR18650MJ1_closs_calendar_aging.csv` & `simses-1.3.4/simses/data/lithium_ion/cell/LG_INR18650MJ1_closs_calendar_aging.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/lithium_ion/cell/LG_INR18650MJ1_closs_cycling_aging.csv` & `simses-1.3.4/simses/data/lithium_ion/cell/LG_INR18650MJ1_closs_cycling_aging.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/lithium_ion/cell/LG_INR18650MJ1_rint_cycling_aging.csv` & `simses-1.3.4/simses/data/lithium_ion/cell/LG_INR18650MJ1_rint_cycling_aging.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/lithium_ion/cell/LTO_LMO_closs_cycling_aging.csv` & `simses-1.3.4/simses/data/lithium_ion/cell/LTO_LMO_closs_cycling_aging.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/lithium_ion/cell/LTO_LMO_rint_cycling_aging.csv` & `simses-1.3.4/simses/data/lithium_ion/cell/LTO_LMO_rint_cycling_aging.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/lithium_ion/cell/LTO_NMC_closs_calendar_aging.csv` & `simses-1.3.4/simses/data/lithium_ion/cell/LTO_NMC_closs_calendar_aging.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/lithium_ion/cell/LTO_NMC_closs_cycling_aging.csv` & `simses-1.3.4/simses/data/lithium_ion/cell/LTO_NMC_closs_cycling_aging.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/lithium_ion/cell/LTO_NMC_rint_calendar_aging.csv` & `simses-1.3.4/simses/data/lithium_ion/cell/LTO_NMC_rint_calendar_aging.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/lithium_ion/cell/LTO_NMC_rint_cycling_aging.csv` & `simses-1.3.4/simses/data/lithium_ion/cell/LTO_NMC_rint_cycling_aging.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/lithium_ion/cell/NCA_PanasonicNCR_OCV.csv` & `simses-1.3.4/simses/data/lithium_ion/cell/NCA_PanasonicNCR_OCV.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/lithium_ion/cell/NCA_PanasonicNCR_Rint.csv` & `simses-1.3.4/simses/data/lithium_ion/cell/NCA_PanasonicNCR_Rint.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/lithium_ion/cell/NMC_Akasol_OEM_Rint.csv` & `simses-1.3.4/simses/data/lithium_ion/cell/NMC_Akasol_OEM_Rint.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/lithium_ion/cell/NMC_Molicel_OCV.csv` & `simses-1.3.4/simses/data/lithium_ion/cell/NMC_Molicel_OCV.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/lithium_ion/cell/NMC_Molicel_Rint.csv` & `simses-1.3.4/simses/data/lithium_ion/cell/NMC_Molicel_Rint.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/lithium_ion/cell/NMC_Molicel_capacity_cal.csv` & `simses-1.3.4/simses/data/lithium_ion/cell/NMC_Molicel_capacity_cal.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/lithium_ion/cell/NMC_Molicel_capacity_cyc.csv` & `simses-1.3.4/simses/data/lithium_ion/cell/NMC_Molicel_capacity_cyc.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/lithium_ion/cell/NMC_Molicel_ri_cal.csv` & `simses-1.3.4/simses/data/lithium_ion/cell/NMC_Molicel_ri_cal.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/lithium_ion/cell/NMC_Molicel_ri_cyc.csv` & `simses-1.3.4/simses/data/lithium_ion/cell/NMC_Molicel_ri_cyc.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/lithium_ion/cell/NMC_Samsung_LabTest_cell_00_OCV.csv` & `simses-1.3.4/simses/data/lithium_ion/cell/NMC_Samsung_LabTest_cell_00_OCV.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/lithium_ion/cell/NMC_Samsung_LabTest_cell_00_Ri.csv` & `simses-1.3.4/simses/data/lithium_ion/cell/NMC_Samsung_LabTest_cell_00_Ri.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/lithium_ion/cell/NMC_Sanyo_OCV.csv` & `simses-1.3.4/simses/data/lithium_ion/cell/NMC_Sanyo_OCV.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/lithium_ion/cell/NMC_Sanyo_Rint.csv` & `simses-1.3.4/simses/data/lithium_ion/cell/NMC_Sanyo_Rint.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/lithium_ion/cell/Sodium_Ion_OCV_Green_Rock.csv` & `simses-1.3.4/simses/data/lithium_ion/cell/Sodium_Ion_OCV_Green_Rock.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/lithium_ion/cell/Sodium_Ion_Rint_Green_Rock.csv` & `simses-1.3.4/simses/data/lithium_ion/cell/Sodium_Ion_Rint_Green_Rock.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/logo/SimSES.png` & `simses-1.3.4/simses/data/logo/SimSES.png`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/power_electronics/sinamics_S120_efficiency.csv` & `simses-1.3.4/simses/data/power_electronics/sinamics_S120_efficiency.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/redox_flow/degradation/H2_Current_F1_Schweiss.csv` & `simses-1.3.4/simses/data/redox_flow/degradation/H2_Current_F1_Schweiss.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/redox_flow/degradation/H2_Current_F3_Schweiss.csv` & `simses-1.3.4/simses/data/redox_flow/degradation/H2_Current_F3_Schweiss.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/redox_flow/stack/SHUNT_CellStack_2250_40.csv` & `simses-1.3.4/simses/data/redox_flow/stack/SHUNT_CellStack_2250_40.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/redox_flow/stack/SHUNT_FILE_INDUSTRIAL_STACK_1500W.csv` & `simses-1.3.4/simses/data/redox_flow/stack/SHUNT_FILE_INDUSTRIAL_STACK_1500W.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/redox_flow/stack/SHUNT_FILE_INDUSTRIAL_STACK_9000W.csv` & `simses-1.3.4/simses/data/redox_flow/stack/SHUNT_FILE_INDUSTRIAL_STACK_9000W.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data/redox_flow/stack/SHUNT_HP_Stack.csv` & `simses-1.3.4/simses/data/redox_flow/stack/SHUNT_HP_Stack.csv`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/data.defaults.ini` & `simses-1.3.4/simses/data.defaults.ini`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/logger.defaults.ini` & `simses-1.3.4/simses/logger.defaults.ini`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/logic/energy_management/energy_management_factory.py` & `simses-1.3.4/simses/logic/energy_management/energy_management_factory.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/logic/energy_management/energy_management_system.py` & `simses-1.3.4/simses/logic/energy_management/energy_management_system.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/logic/energy_management/strategy/basic/electric_vehicle.py` & `simses-1.3.4/simses/logic/energy_management/strategy/basic/electric_vehicle.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/logic/energy_management/strategy/basic/electric_vehicle_soc.py` & `simses-1.3.4/simses/logic/energy_management/strategy/basic/electric_vehicle_soc.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/logic/energy_management/strategy/basic/electric_vehicle_v2g.py` & `simses-1.3.4/simses/logic/energy_management/strategy/basic/electric_vehicle_v2g.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/logic/energy_management/strategy/basic/ev_charger_with_buffer.py` & `simses-1.3.4/simses/logic/energy_management/strategy/basic/ev_charger_with_buffer.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/logic/energy_management/strategy/basic/frequency_containment_reserve.py` & `simses-1.3.4/simses/logic/energy_management/strategy/basic/frequency_containment_reserve.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/logic/energy_management/strategy/basic/intraday_market_recharge.py` & `simses-1.3.4/simses/logic/energy_management/strategy/basic/intraday_market_recharge.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/logic/energy_management/strategy/basic/peak_shaving_perfect_foresight.py` & `simses-1.3.4/simses/logic/energy_management/strategy/basic/peak_shaving_perfect_foresight.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/logic/energy_management/strategy/basic/peak_shaving_simple.py` & `simses-1.3.4/simses/logic/energy_management/strategy/basic/peak_shaving_simple.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/logic/energy_management/strategy/basic/power_follower.py` & `simses-1.3.4/simses/logic/energy_management/strategy/basic/power_follower.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/logic/energy_management/strategy/basic/residential_pv_feed_in_damp.py` & `simses-1.3.4/simses/logic/energy_management/strategy/basic/residential_pv_feed_in_damp.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/logic/energy_management/strategy/basic/residential_pv_greedy.py` & `simses-1.3.4/simses/logic/energy_management/strategy/basic/residential_pv_greedy.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/logic/energy_management/strategy/basic/soc_follower.py` & `simses-1.3.4/simses/logic/energy_management/strategy/basic/soc_follower.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/logic/energy_management/strategy/basic/use_all_renewable_energy.py` & `simses-1.3.4/simses/logic/energy_management/strategy/basic/use_all_renewable_energy.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/logic/energy_management/strategy/operation_strategy.py` & `simses-1.3.4/simses/logic/energy_management/strategy/operation_strategy.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/logic/energy_management/strategy/stacked/fcr_idm_recharge_stacked.py` & `simses-1.3.4/simses/logic/energy_management/strategy/stacked/fcr_idm_recharge_stacked.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/logic/energy_management/strategy/stacked/stacked_operation_strategy.py` & `simses-1.3.4/simses/logic/energy_management/strategy/stacked/stacked_operation_strategy.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/logic/power_distribution/efficient.py` & `simses-1.3.4/simses/logic/power_distribution/efficient.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/logic/power_distribution/equal.py` & `simses-1.3.4/simses/logic/power_distribution/equal.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/logic/power_distribution/power_distributor.py` & `simses-1.3.4/simses/logic/power_distribution/power_distributor.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/logic/power_distribution/soc.py` & `simses-1.3.4/simses/logic/power_distribution/soc.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/logic/power_distribution/state.py` & `simses-1.3.4/simses/logic/power_distribution/state.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/logic/power_distribution/technology.py` & `simses-1.3.4/simses/logic/power_distribution/technology.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/logic/test/test_electric_vehicle_SOC_meanpower.py` & `simses-1.3.4/simses/logic/test/test_electric_vehicle_SOC_meanpower.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/logic/test/test_electric_vehicle_SOC_original.py` & `simses-1.3.4/simses/logic/test/test_electric_vehicle_SOC_original.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/logic/test/test_electric_vehicle_SOC_paused.py` & `simses-1.3.4/simses/logic/test/test_electric_vehicle_SOC_paused.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/logic/test/test_electric_vehicle_SOC_uncontrolled.py` & `simses-1.3.4/simses/logic/test/test_electric_vehicle_SOC_uncontrolled.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/logic/test/test_electric_vehicle_all_strategies.py` & `simses-1.3.4/simses/logic/test/test_electric_vehicle_all_strategies.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/logic/test/test_electric_vehicle_uncontrolled.py` & `simses-1.3.4/simses/logic/test/test_electric_vehicle_uncontrolled.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/logic/test/test_equal_power_distributor.py` & `simses-1.3.4/simses/logic/test/test_equal_power_distributor.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/logic/test/test_multi_use.py` & `simses-1.3.4/simses/logic/test/test_multi_use.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/logic/test/test_peak_shaving.py` & `simses-1.3.4/simses/logic/test/test_peak_shaving.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/logic/test/test_residential_pv_greedy.py` & `simses-1.3.4/simses/logic/test/test_residential_pv_greedy.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/logic/test/test_soc_based_power_distributor.py` & `simses-1.3.4/simses/logic/test/test_soc_based_power_distributor.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/logic/thermal_management/on_off_controller.py` & `simses-1.3.4/simses/logic/thermal_management/on_off_controller.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/logic/thermal_management/pid_controller.py` & `simses-1.3.4/simses/logic/thermal_management/pid_controller.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/simses.egg-info/PKG-INFO` & `simses-1.3.4/simses.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simses
-Version: 1.3.3
+Version: 1.3.4
 Summary: Simulation for Stationary Storage Systems (SimSES)
 Author-email: simses.ees@ed.tum.de
 License: BSD-3-Clause
 Project-URL: source, https://gitlab.lrz.de/open-ees-ses/simses
 Keywords: simulation,battery,energy,storage
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `simses-1.3.3/simses/simses.egg-info/SOURCES.txt` & `simses-1.3.4/simses.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,27 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 pyproject.toml
+doc/__init__.py
+doc/conf.py
+doc/graph/__init__.py
+doc/graph/graph.py
 simses/VERSION
+simses/__init__.py
 simses/analysis.defaults.ini
 simses/data.defaults.ini
 simses/logger.defaults.ini
+simses/main.py
 simses/simulation.defaults.ini
+simses.egg-info/PKG-INFO
+simses.egg-info/SOURCES.txt
+simses.egg-info/dependency_links.txt
+simses.egg-info/requires.txt
+simses.egg-info/top_level.txt
 simses/analysis/__init__.py
 simses/analysis/factory.py
 simses/analysis/storage.py
 simses/analysis/utils.py
 simses/analysis/data/__init__.py
 simses/analysis/data/abstract_data.py
 simses/analysis/data/electrolyzer.py
@@ -293,15 +304,14 @@
 simses/logic/energy_management/strategy/basic/use_all_renewable_energy.py
 simses/logic/energy_management/strategy/optimization/__init__.py
 simses/logic/energy_management/strategy/optimization/forecast_utils/__init__.py
 simses/logic/energy_management/strategy/optimization/linearized_models/__init__.py
 simses/logic/energy_management/strategy/serial/__init__.py
 simses/logic/energy_management/strategy/stacked/__init__.py
 simses/logic/energy_management/strategy/stacked/fcr_idm_recharge_stacked.py
-simses/logic/energy_management/strategy/stacked/parallel_multi_use_with_stealing.py
 simses/logic/energy_management/strategy/stacked/stacked_operation_strategy.py
 simses/logic/power_distribution/__init__.py
 simses/logic/power_distribution/efficient.py
 simses/logic/power_distribution/equal.py
 simses/logic/power_distribution/power_distributor.py
 simses/logic/power_distribution/soc.py
 simses/logic/power_distribution/state.py
@@ -319,32 +329,26 @@
 simses/logic/test/test_peak_shaving.py
 simses/logic/test/test_residential_pv_greedy.py
 simses/logic/test/test_soc_based_power_distributor.py
 simses/logic/thermal_management/__init__.py
 simses/logic/thermal_management/on_off_controller.py
 simses/logic/thermal_management/pid_controller.py
 simses/logic/thermal_management/thermal_management.py
-simses/simses.egg-info/PKG-INFO
-simses/simses.egg-info/SOURCES.txt
-simses/simses.egg-info/dependency_links.txt
-simses/simses.egg-info/requires.txt
-simses/simses.egg-info/top_level.txt
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
 simses/simulation/simbas/room_tool_reader.py
 simses/simulation/simbas/simbas.py
-simses/simulation/simulation_examples/__init__.py
 simses/simulation/system_tests/__init__.py
 simses/simulation/system_tests/system_test.py
 simses/simulation/system_tests/configs/__init__.py
 simses/system/__init__.py
 simses/system/factory.py
 simses/system/storage_circuit.py
 simses/system/storage_system_ac.py
```

### Comparing `simses-1.3.3/simses/simulation/batch_processing.py` & `simses-1.3.4/simses/simulation/batch_processing.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/simulation/batch_simulation.py` & `simses-1.3.4/simses/simulation/batch_simulation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/simulation/case_studies/case_study_1_peak_shaving.py` & `simses-1.3.4/simses/simulation/case_studies/case_study_1_peak_shaving.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/simulation/case_studies/case_study_2_fcr.py` & `simses-1.3.4/simses/simulation/case_studies/case_study_2_fcr.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/simulation/example.py` & `simses-1.3.4/simses/simulation/example.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/simulation/simbas/room_tool_reader.py` & `simses-1.3.4/simses/simulation/simbas/room_tool_reader.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/simulation/simbas/simbas.py` & `simses-1.3.4/simses/simulation/simbas/simbas.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/simulation/simulator.py` & `simses-1.3.4/simses/simulation/simulator.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/simulation/system_tests/system_test.py` & `simses-1.3.4/simses/simulation/system_tests/system_test.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/simulation.defaults.ini` & `simses-1.3.4/simses/simulation.defaults.ini`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/auxiliary/auxiliary.py` & `simses-1.3.4/simses/system/auxiliary/auxiliary.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/auxiliary/compression/compressor.py` & `simses-1.3.4/simses/system/auxiliary/compression/compressor.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/auxiliary/compression/hydrogen_isentrop.py` & `simses-1.3.4/simses/system/auxiliary/compression/hydrogen_isentrop.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/auxiliary/gas_drying/gas_dryer.py` & `simses-1.3.4/simses/system/auxiliary/gas_drying/gas_dryer.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/auxiliary/gas_drying/hydrogen.py` & `simses-1.3.4/simses/system/auxiliary/gas_drying/hydrogen.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/auxiliary/heating_ventilation_air_conditioning/fan.py` & `simses-1.3.4/simses/system/auxiliary/heating_ventilation_air_conditioning/fan.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/auxiliary/heating_ventilation_air_conditioning/fix_cop_hvac.py` & `simses-1.3.4/simses/system/auxiliary/heating_ventilation_air_conditioning/fix_cop_hvac.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/auxiliary/heating_ventilation_air_conditioning/hvac.py` & `simses-1.3.4/simses/system/auxiliary/heating_ventilation_air_conditioning/hvac.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/auxiliary/heating_ventilation_air_conditioning/no_hvac.py` & `simses-1.3.4/simses/system/auxiliary/heating_ventilation_air_conditioning/no_hvac.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/auxiliary/pump/abstract_pump.py` & `simses-1.3.4/simses/system/auxiliary/pump/abstract_pump.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/auxiliary/pump/fixeta_centrifugal.py` & `simses-1.3.4/simses/system/auxiliary/pump/fixeta_centrifugal.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/auxiliary/pump/scalable_variable_eta_centrifugal.py` & `simses-1.3.4/simses/system/auxiliary/pump/scalable_variable_eta_centrifugal.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/auxiliary/pump/variable_eta_centrifugal.py` & `simses-1.3.4/simses/system/auxiliary/pump/variable_eta_centrifugal.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/auxiliary/water_heating/water_heater.py` & `simses-1.3.4/simses/system/auxiliary/water_heating/water_heater.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/dc_coupling/bus_charging_profile.py` & `simses-1.3.4/simses/system/dc_coupling/bus_charging_profile.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/dc_coupling/dc_coupler.py` & `simses-1.3.4/simses/system/dc_coupling/dc_coupler.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/dc_coupling/generation/dc_generation.py` & `simses-1.3.4/simses/system/dc_coupling/generation/dc_generation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/dc_coupling/generation/pv_dc_generation.py` & `simses-1.3.4/simses/system/dc_coupling/generation/pv_dc_generation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/dc_coupling/load/dc_bus_charging_fixed.py` & `simses-1.3.4/simses/system/dc_coupling/load/dc_bus_charging_fixed.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/dc_coupling/load/dc_bus_charging_profile.py` & `simses-1.3.4/simses/system/dc_coupling/load/dc_bus_charging_profile.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/dc_coupling/load/dc_bus_charging_random.py` & `simses-1.3.4/simses/system/dc_coupling/load/dc_bus_charging_random.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/dc_coupling/load/dc_load.py` & `simses-1.3.4/simses/system/dc_coupling/load/dc_load.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/dc_coupling/load/dc_radio_ups_load.py` & `simses-1.3.4/simses/system/dc_coupling/load/dc_radio_ups_load.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/dc_coupling/usp_dc_coupling.py` & `simses-1.3.4/simses/system/dc_coupling/usp_dc_coupling.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/factory.py` & `simses-1.3.4/simses/system/factory.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/housing/abstract_housing.py` & `simses-1.3.4/simses/system/housing/abstract_housing.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/housing/forty_ft_container.py` & `simses-1.3.4/simses/system/housing/forty_ft_container.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/housing/layer.py` & `simses-1.3.4/simses/system/housing/layer.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/housing/twenty_ft_container.py` & `simses-1.3.4/simses/system/housing/twenty_ft_container.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/power_electronics/acdc_converter/abstract_acdc_converter.py` & `simses-1.3.4/simses/system/power_electronics/acdc_converter/abstract_acdc_converter.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/power_electronics/acdc_converter/bonfiglioli.py` & `simses-1.3.4/simses/system/power_electronics/acdc_converter/bonfiglioli.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/power_electronics/acdc_converter/fix_efficiency.py` & `simses-1.3.4/simses/system/power_electronics/acdc_converter/fix_efficiency.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/power_electronics/acdc_converter/notton.py` & `simses-1.3.4/simses/system/power_electronics/acdc_converter/notton.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/power_electronics/acdc_converter/notton_loss.py` & `simses-1.3.4/simses/system/power_electronics/acdc_converter/notton_loss.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/power_electronics/acdc_converter/rampinelli_fit.py` & `simses-1.3.4/simses/system/power_electronics/acdc_converter/rampinelli_fit.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/power_electronics/acdc_converter/sinamics.py` & `simses-1.3.4/simses/system/power_electronics/acdc_converter/sinamics.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/power_electronics/acdc_converter/stable.py` & `simses-1.3.4/simses/system/power_electronics/acdc_converter/stable.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/power_electronics/acdc_converter/stacked.py` & `simses-1.3.4/simses/system/power_electronics/acdc_converter/stacked.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/power_electronics/acdc_converter/sungrow.py` & `simses-1.3.4/simses/system/power_electronics/acdc_converter/sungrow.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/power_electronics/dcdc_converter/abstract_dcdc_converter.py` & `simses-1.3.4/simses/system/power_electronics/dcdc_converter/abstract_dcdc_converter.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/power_electronics/dcdc_converter/fix_efficiency.py` & `simses-1.3.4/simses/system/power_electronics/dcdc_converter/fix_efficiency.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/power_electronics/dcdc_converter/no_dcdc.py` & `simses-1.3.4/simses/system/power_electronics/dcdc_converter/no_dcdc.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/power_electronics/dcdc_converter/no_loss.py` & `simses-1.3.4/simses/system/power_electronics/dcdc_converter/no_loss.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/power_electronics/electronics.py` & `simses-1.3.4/simses/system/power_electronics/electronics.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/storage_circuit.py` & `simses-1.3.4/simses/system/storage_circuit.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/storage_system_ac.py` & `simses-1.3.4/simses/system/storage_system_ac.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/storage_system_dc.py` & `simses-1.3.4/simses/system/storage_system_dc.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/test/test_acdc_converter.py` & `simses-1.3.4/simses/system/test/test_acdc_converter.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/test/test_constant_ambient_temperature.py` & `simses-1.3.4/simses/system/test/test_constant_ambient_temperature.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/test/test_fix_cop_hvac.py` & `simses-1.3.4/simses/system/test/test_fix_cop_hvac.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/test/test_location_ambient_temperature.py` & `simses-1.3.4/simses/system/test/test_location_ambient_temperature.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/test/test_location_ambient_temperature_profile_check.py` & `simses-1.3.4/simses/system/test/test_location_ambient_temperature_profile_check.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/test/test_location_solar_irradiation_model.py` & `simses-1.3.4/simses/system/test/test_location_solar_irradiation_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/test/test_location_solar_irradiation_model_profile_check.py` & `simses-1.3.4/simses/system/test/test_location_solar_irradiation_model_profile_check.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/test/test_notton_acdc_converter.py` & `simses-1.3.4/simses/system/test/test_notton_acdc_converter.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/thermal/ambient/ambient_thermal_model.py` & `simses-1.3.4/simses/system/thermal/ambient/ambient_thermal_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/thermal/ambient/constant_temperature.py` & `simses-1.3.4/simses/system/thermal/ambient/constant_temperature.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/thermal/ambient/location_temperature.py` & `simses-1.3.4/simses/system/thermal/ambient/location_temperature.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/thermal/ambient/user_battery_temperature.py` & `simses-1.3.4/simses/system/thermal/ambient/user_battery_temperature.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/thermal/model/no_system_thermal_model.py` & `simses-1.3.4/simses/system/thermal/model/no_system_thermal_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/thermal/model/system_thermal_model.py` & `simses-1.3.4/simses/system/thermal/model/system_thermal_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/thermal/model/zero_d_room_thermal_model.py` & `simses-1.3.4/simses/system/thermal/model/zero_d_room_thermal_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/thermal/model/zero_d_system_thermal_model.py` & `simses-1.3.4/simses/system/thermal/model/zero_d_system_thermal_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/thermal/solar_irradiation/location.py` & `simses-1.3.4/simses/system/thermal/solar_irradiation/location.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/thermal/solar_irradiation/no_solar_irradiation.py` & `simses-1.3.4/simses/system/thermal/solar_irradiation/no_solar_irradiation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/system/thermal/solar_irradiation/solar_irradiation_model.py` & `simses-1.3.4/simses/system/thermal/solar_irradiation/solar_irradiation_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/control/management.py` & `simses-1.3.4/simses/technology/hydrogen/control/management.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/control/pressure/ideal_var_cathode.py` & `simses-1.3.4/simses/technology/hydrogen/control/pressure/ideal_var_cathode.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/control/pressure/no_pressure_controller.py` & `simses-1.3.4/simses/technology/hydrogen/control/pressure/no_pressure_controller.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/control/pressure/pressure_controller.py` & `simses-1.3.4/simses/technology/hydrogen/control/pressure/pressure_controller.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/control/thermal/ideal_var_flow.py` & `simses-1.3.4/simses/technology/hydrogen/control/thermal/ideal_var_flow.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/control/thermal/no_thermal_controller.py` & `simses-1.3.4/simses/technology/hydrogen/control/thermal/no_thermal_controller.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/control/thermal/thermal_controller.py` & `simses-1.3.4/simses/technology/hydrogen/control/thermal/thermal_controller.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/control/thermal/var_flow.py` & `simses-1.3.4/simses/technology/hydrogen/control/thermal/var_flow.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/calendar/calendar_degradation.py` & `simses-1.3.4/simses/technology/hydrogen/electrolyzer/degradation/calendar/calendar_degradation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/calendar/no_calendar_degradation.py` & `simses-1.3.4/simses/technology/hydrogen/electrolyzer/degradation/calendar/no_calendar_degradation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/calendar/pem_analytic.py` & `simses-1.3.4/simses/technology/hydrogen/electrolyzer/degradation/calendar/pem_analytic.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/cyclic/cyclic_degradation.py` & `simses-1.3.4/simses/technology/hydrogen/electrolyzer/degradation/cyclic/cyclic_degradation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/cyclic/no_cyclic_degradation.py` & `simses-1.3.4/simses/technology/hydrogen/electrolyzer/degradation/cyclic/no_cyclic_degradation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/cyclic/pem_analytic.py` & `simses-1.3.4/simses/technology/hydrogen/electrolyzer/degradation/cyclic/pem_analytic.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/cyclic/pem_analytic_ptl_coating.py` & `simses-1.3.4/simses/technology/hydrogen/electrolyzer/degradation/cyclic/pem_analytic_ptl_coating.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/degradation_model.py` & `simses-1.3.4/simses/technology/hydrogen/electrolyzer/degradation/degradation_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/no_degradation.py` & `simses-1.3.4/simses/technology/hydrogen/electrolyzer/degradation/no_degradation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/pem_analytic.py` & `simses-1.3.4/simses/technology/hydrogen/electrolyzer/degradation/pem_analytic.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/electrolyzer/degradation/pem_analytic_ptl_coating.py` & `simses-1.3.4/simses/technology/hydrogen/electrolyzer/degradation/pem_analytic_ptl_coating.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/electrolyzer/factory.py` & `simses-1.3.4/simses/technology/hydrogen/electrolyzer/factory.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/electrolyzer/pressure/abstract_model.py` & `simses-1.3.4/simses/technology/hydrogen/electrolyzer/pressure/abstract_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/electrolyzer/pressure/alkaline.py` & `simses-1.3.4/simses/technology/hydrogen/electrolyzer/pressure/alkaline.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/electrolyzer/pressure/no_pressure_model.py` & `simses-1.3.4/simses/technology/hydrogen/electrolyzer/pressure/no_pressure_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/electrolyzer/pressure/var_cathode.py` & `simses-1.3.4/simses/technology/hydrogen/electrolyzer/pressure/var_cathode.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/alkaline/electrical_model.py` & `simses-1.3.4/simses/technology/hydrogen/electrolyzer/stack/alkaline/electrical_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/alkaline/electrolyzer_model.py` & `simses-1.3.4/simses/technology/hydrogen/electrolyzer/stack/alkaline/electrolyzer_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/alkaline/fluid_model.py` & `simses-1.3.4/simses/technology/hydrogen/electrolyzer/stack/alkaline/fluid_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/alkaline/parameters.py` & `simses-1.3.4/simses/technology/hydrogen/electrolyzer/stack/alkaline/parameters.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/alkaline/pressure_model.py` & `simses-1.3.4/simses/technology/hydrogen/electrolyzer/stack/alkaline/pressure_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/no_electrolyzer.py` & `simses-1.3.4/simses/technology/hydrogen/electrolyzer/stack/no_electrolyzer.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/pem.py` & `simses-1.3.4/simses/technology/hydrogen/electrolyzer/stack/pem.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/efficiency_curves.py` & `simses-1.3.4/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/efficiency_curves.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/electrical_model.py` & `simses-1.3.4/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/electrical_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/electrolyzer_model.py` & `simses-1.3.4/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/electrolyzer_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/electrolyzer_model_ptl_coating.py` & `simses-1.3.4/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/electrolyzer_model_ptl_coating.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/fluid_model.py` & `simses-1.3.4/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/fluid_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/membrane_model.py` & `simses-1.3.4/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/membrane_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/parameters.py` & `simses-1.3.4/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/parameters.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/pressure_model.py` & `simses-1.3.4/simses/technology/hydrogen/electrolyzer/stack/pem_analytic/pressure_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/electrolyzer/stack/stack_model.py` & `simses-1.3.4/simses/technology/hydrogen/electrolyzer/stack/stack_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/electrolyzer/system.py` & `simses-1.3.4/simses/technology/hydrogen/electrolyzer/system.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/electrolyzer/thermal/abstract_model.py` & `simses-1.3.4/simses/technology/hydrogen/electrolyzer/thermal/abstract_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/electrolyzer/thermal/alkaline.py` & `simses-1.3.4/simses/technology/hydrogen/electrolyzer/thermal/alkaline.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/electrolyzer/thermal/no_thermal_model.py` & `simses-1.3.4/simses/technology/hydrogen/electrolyzer/thermal/no_thermal_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/electrolyzer/thermal/pem.py` & `simses-1.3.4/simses/technology/hydrogen/electrolyzer/thermal/pem.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/factory.py` & `simses-1.3.4/simses/technology/hydrogen/factory.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/fuel_cell/factory.py` & `simses-1.3.4/simses/technology/hydrogen/fuel_cell/factory.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/fuel_cell/pressure/no_pressure.py` & `simses-1.3.4/simses/technology/hydrogen/fuel_cell/pressure/no_pressure.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/fuel_cell/pressure/pressure_model.py` & `simses-1.3.4/simses/technology/hydrogen/fuel_cell/pressure/pressure_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/fuel_cell/stack/jupiter.py` & `simses-1.3.4/simses/technology/hydrogen/fuel_cell/stack/jupiter.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/fuel_cell/stack/no_fuel_cell.py` & `simses-1.3.4/simses/technology/hydrogen/fuel_cell/stack/no_fuel_cell.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/fuel_cell/stack/pem.py` & `simses-1.3.4/simses/technology/hydrogen/fuel_cell/stack/pem.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/fuel_cell/stack/stack_model.py` & `simses-1.3.4/simses/technology/hydrogen/fuel_cell/stack/stack_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/fuel_cell/system.py` & `simses-1.3.4/simses/technology/hydrogen/fuel_cell/system.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/fuel_cell/thermal/no_thermal_model.py` & `simses-1.3.4/simses/technology/hydrogen/fuel_cell/thermal/no_thermal_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/fuel_cell/thermal/simple.py` & `simses-1.3.4/simses/technology/hydrogen/fuel_cell/thermal/simple.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/fuel_cell/thermal/thermal_model.py` & `simses-1.3.4/simses/technology/hydrogen/fuel_cell/thermal/thermal_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/hydrogen_storage/hydrogen_storage.py` & `simses-1.3.4/simses/technology/hydrogen/hydrogen_storage/hydrogen_storage.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/hydrogen_storage/pipeline/simple_pipeline.py` & `simses-1.3.4/simses/technology/hydrogen/hydrogen_storage/pipeline/simple_pipeline.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/hydrogen_storage/pressuretank/pressuretank.py` & `simses-1.3.4/simses/technology/hydrogen/hydrogen_storage/pressuretank/pressuretank.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/system.py` & `simses-1.3.4/simses/technology/hydrogen/system.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/hydrogen/test/test_pem_electrolyzer.py` & `simses-1.3.4/simses/technology/hydrogen/test/test_pem_electrolyzer.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/battery.py` & `simses-1.3.4/simses/technology/lithium_ion/battery.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/battery_management_system/management_system.py` & `simses-1.3.4/simses/technology/lithium_ion/battery_management_system/management_system.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/cell/electric/default.py` & `simses-1.3.4/simses/technology/lithium_ion/cell/electric/default.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/cell/electric/properties.py` & `simses-1.3.4/simses/technology/lithium_ion/cell/electric/properties.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/cell/format/abstract.py` & `simses-1.3.4/simses/technology/lithium_ion/cell/format/abstract.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/cell/format/pouch.py` & `simses-1.3.4/simses/technology/lithium_ion/cell/format/pouch.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/cell/format/prismatic.py` & `simses-1.3.4/simses/technology/lithium_ion/cell/format/prismatic.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/cell/format/round.py` & `simses-1.3.4/simses/technology/lithium_ion/cell/format/round.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/cell/generic.py` & `simses-1.3.4/simses/technology/lithium_ion/cell/generic.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/cell/isea.py` & `simses-1.3.4/simses/technology/lithium_ion/cell/isea.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/cell/lfp_sony.py` & `simses-1.3.4/simses/technology/lithium_ion/cell/lfp_sony.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/cell/lmo_daimler.py` & `simses-1.3.4/simses/technology/lithium_ion/cell/lmo_daimler.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/cell/lto_lmo.py` & `simses-1.3.4/simses/technology/lithium_ion/cell/lto_lmo.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/cell/lto_nmc.py` & `simses-1.3.4/simses/technology/lithium_ion/cell/lto_nmc.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/cell/nca_panasonic_generic.py` & `simses-1.3.4/simses/technology/lithium_ion/cell/nca_panasonic_generic.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/cell/nca_panasonic_ncr.py` & `simses-1.3.4/simses/technology/lithium_ion/cell/nca_panasonic_ncr.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/cell/nmc_lgmj1.py` & `simses-1.3.4/simses/technology/lithium_ion/cell/nmc_lgmj1.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/cell/nmc_molicel.py` & `simses-1.3.4/simses/technology/lithium_ion/cell/nmc_molicel.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/cell/nmc_molicel_generic.py` & `simses-1.3.4/simses/technology/lithium_ion/cell/nmc_molicel_generic.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/cell/nmc_samsung78Ah.py` & `simses-1.3.4/simses/technology/lithium_ion/cell/nmc_samsung78Ah.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/cell/nmc_samsung94Ah.py` & `simses-1.3.4/simses/technology/lithium_ion/cell/nmc_samsung94Ah.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/cell/nmc_samsung94Ah_hybrid.py` & `simses-1.3.4/simses/technology/lithium_ion/cell/nmc_samsung94Ah_hybrid.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/cell/nmc_sanyo_ur18650e.py` & `simses-1.3.4/simses/technology/lithium_ion/cell/nmc_sanyo_ur18650e.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/cell/sodium_ion/sodium_ion_green_rock.py` & `simses-1.3.4/simses/technology/lithium_ion/cell/sodium_ion/sodium_ion_green_rock.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/cell/thermal/default.py` & `simses-1.3.4/simses/technology/lithium_ion/cell/thermal/default.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/cell/thermal/properties.py` & `simses-1.3.4/simses/technology/lithium_ion/cell/thermal/properties.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/cell/type.py` & `simses-1.3.4/simses/technology/lithium_ion/cell/type.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/circuit.py` & `simses-1.3.4/simses/technology/lithium_ion/circuit.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/calendar_degradation.py` & `simses-1.3.4/simses/technology/lithium_ion/degradation/calendar/calendar_degradation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/generic_cell.py` & `simses-1.3.4/simses/technology/lithium_ion/degradation/calendar/generic_cell.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/lfp_generic.py` & `simses-1.3.4/simses/technology/lithium_ion/degradation/calendar/lfp_generic.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/lfp_sony.py` & `simses-1.3.4/simses/technology/lithium_ion/degradation/calendar/lfp_sony.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/lto_lmo.py` & `simses-1.3.4/simses/technology/lithium_ion/degradation/calendar/lto_lmo.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/lto_nmc.py` & `simses-1.3.4/simses/technology/lithium_ion/degradation/calendar/lto_nmc.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/nca_generic.py` & `simses-1.3.4/simses/technology/lithium_ion/degradation/calendar/nca_generic.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/nca_panasonicNCR.py` & `simses-1.3.4/simses/technology/lithium_ion/degradation/calendar/nca_panasonicNCR.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/nmc_generic.py` & `simses-1.3.4/simses/technology/lithium_ion/degradation/calendar/nmc_generic.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/nmc_lgmj1.py` & `simses-1.3.4/simses/technology/lithium_ion/degradation/calendar/nmc_lgmj1.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/nmc_molicel.py` & `simses-1.3.4/simses/technology/lithium_ion/degradation/calendar/nmc_molicel.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/nmc_sanyo_ur18650e.py` & `simses-1.3.4/simses/technology/lithium_ion/degradation/calendar/nmc_sanyo_ur18650e.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/degradation/calendar/no_calendar_dedradation.py` & `simses-1.3.4/simses/technology/lithium_ion/degradation/calendar/no_calendar_dedradation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/cyclic_degradation.py` & `simses-1.3.4/simses/technology/lithium_ion/degradation/cyclic/cyclic_degradation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/generic_cell.py` & `simses-1.3.4/simses/technology/lithium_ion/degradation/cyclic/generic_cell.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/lfp_generic.py` & `simses-1.3.4/simses/technology/lithium_ion/degradation/cyclic/lfp_generic.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/lfp_sony.py` & `simses-1.3.4/simses/technology/lithium_ion/degradation/cyclic/lfp_sony.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/lto_lmo.py` & `simses-1.3.4/simses/technology/lithium_ion/degradation/cyclic/lto_lmo.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/lto_nmc.py` & `simses-1.3.4/simses/technology/lithium_ion/degradation/cyclic/lto_nmc.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/nca_generic.py` & `simses-1.3.4/simses/technology/lithium_ion/degradation/cyclic/nca_generic.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/nca_panasonicNCR.py` & `simses-1.3.4/simses/technology/lithium_ion/degradation/cyclic/nca_panasonicNCR.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/nmc_generic.py` & `simses-1.3.4/simses/technology/lithium_ion/degradation/cyclic/nmc_generic.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/nmc_lgmj1.py` & `simses-1.3.4/simses/technology/lithium_ion/degradation/cyclic/nmc_lgmj1.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/nmc_molicel.py` & `simses-1.3.4/simses/technology/lithium_ion/degradation/cyclic/nmc_molicel.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/nmc_sanyo_ur18650e.py` & `simses-1.3.4/simses/technology/lithium_ion/degradation/cyclic/nmc_sanyo_ur18650e.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/degradation/cyclic/no_cyclic_degradation.py` & `simses-1.3.4/simses/technology/lithium_ion/degradation/cyclic/no_cyclic_degradation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/degradation/degradation_model.py` & `simses-1.3.4/simses/technology/lithium_ion/degradation/degradation_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/degradation/generic_cell.py` & `simses-1.3.4/simses/technology/lithium_ion/degradation/generic_cell.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/degradation/lfp_generic.py` & `simses-1.3.4/simses/technology/lithium_ion/degradation/lfp_generic.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/degradation/lfp_sony.py` & `simses-1.3.4/simses/technology/lithium_ion/degradation/lfp_sony.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/degradation/lmo_daimler.py` & `simses-1.3.4/simses/technology/lithium_ion/degradation/lmo_daimler.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/degradation/lto_lmo.py` & `simses-1.3.4/simses/technology/lithium_ion/degradation/lto_lmo.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/degradation/lto_nmc.py` & `simses-1.3.4/simses/technology/lithium_ion/degradation/lto_nmc.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/degradation/nca_generic.py` & `simses-1.3.4/simses/technology/lithium_ion/degradation/nca_generic.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/degradation/nca_panasonicNCR.py` & `simses-1.3.4/simses/technology/lithium_ion/degradation/nca_panasonicNCR.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/degradation/nmc_generic.py` & `simses-1.3.4/simses/technology/lithium_ion/degradation/nmc_generic.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/degradation/nmc_lgmj1.py` & `simses-1.3.4/simses/technology/lithium_ion/degradation/nmc_lgmj1.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/degradation/nmc_molicel.py` & `simses-1.3.4/simses/technology/lithium_ion/degradation/nmc_molicel.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/degradation/nmc_samsung94Ah.py` & `simses-1.3.4/simses/technology/lithium_ion/degradation/nmc_samsung94Ah.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/degradation/nmc_sanyo_ur18650e.py` & `simses-1.3.4/simses/technology/lithium_ion/degradation/nmc_sanyo_ur18650e.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/degradation/no_degradation.py` & `simses-1.3.4/simses/technology/lithium_ion/degradation/no_degradation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/equivalent_circuit_model/equivalent_circuit.py` & `simses-1.3.4/simses/technology/lithium_ion/equivalent_circuit_model/equivalent_circuit.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/equivalent_circuit_model/rint_model.py` & `simses-1.3.4/simses/technology/lithium_ion/equivalent_circuit_model/rint_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/factory.py` & `simses-1.3.4/simses/technology/lithium_ion/factory.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/test/test_battery.py` & `simses-1.3.4/simses/technology/lithium_ion/test/test_battery.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/test/test_bms.py` & `simses-1.3.4/simses/technology/lithium_ion/test/test_bms.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/lithium_ion/test/test_type.py` & `simses-1.3.4/simses/technology/lithium_ion/test/test_type.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/redox_flow/degradation/capacity_degradation.py` & `simses-1.3.4/simses/technology/redox_flow/degradation/capacity_degradation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/redox_flow/degradation/const_hydrogen_current.py` & `simses-1.3.4/simses/technology/redox_flow/degradation/const_hydrogen_current.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/redox_flow/degradation/no_degradation.py` & `simses-1.3.4/simses/technology/redox_flow/degradation/no_degradation.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/redox_flow/degradation/variable_hydrogen_current.py` & `simses-1.3.4/simses/technology/redox_flow/degradation/variable_hydrogen_current.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/redox_flow/electrochemical/abstract_electrochemical.py` & `simses-1.3.4/simses/technology/redox_flow/electrochemical/abstract_electrochemical.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/redox_flow/electrochemical/control/redox_control_system.py` & `simses-1.3.4/simses/technology/redox_flow/electrochemical/control/redox_control_system.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/redox_flow/electrochemical/rint_model.py` & `simses-1.3.4/simses/technology/redox_flow/electrochemical/rint_model.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/redox_flow/factory.py` & `simses-1.3.4/simses/technology/redox_flow/factory.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/redox_flow/pump_algorithm/abstract_pump_algorithm.py` & `simses-1.3.4/simses/technology/redox_flow/pump_algorithm/abstract_pump_algorithm.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/redox_flow/pump_algorithm/constant_pressure_pulsed.py` & `simses-1.3.4/simses/technology/redox_flow/pump_algorithm/constant_pressure_pulsed.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/redox_flow/pump_algorithm/fix_flow_rate_start_stop.py` & `simses-1.3.4/simses/technology/redox_flow/pump_algorithm/fix_flow_rate_start_stop.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/redox_flow/pump_algorithm/stoich_flow_rate.py` & `simses-1.3.4/simses/technology/redox_flow/pump_algorithm/stoich_flow_rate.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/redox_flow/stack/abstract_stack.py` & `simses-1.3.4/simses/technology/redox_flow/stack/abstract_stack.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/redox_flow/stack/cell_data_stack_5500w.py` & `simses-1.3.4/simses/technology/redox_flow/stack/cell_data_stack_5500w.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/redox_flow/stack/dummy_stack_3000w.py` & `simses-1.3.4/simses/technology/redox_flow/stack/dummy_stack_3000w.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/redox_flow/stack/dummy_stack_5500W.py` & `simses-1.3.4/simses/technology/redox_flow/stack/dummy_stack_5500W.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/redox_flow/stack/electrolyte/abstract_electrolyte.py` & `simses-1.3.4/simses/technology/redox_flow/stack/electrolyte/abstract_electrolyte.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/redox_flow/stack/electrolyte/vanadium.py` & `simses-1.3.4/simses/technology/redox_flow/stack/electrolyte/vanadium.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/redox_flow/stack/high_performance_stack_5700W.py` & `simses-1.3.4/simses/technology/redox_flow/stack/high_performance_stack_5700W.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/redox_flow/stack/industrial_stack_1500w.py` & `simses-1.3.4/simses/technology/redox_flow/stack/industrial_stack_1500w.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/redox_flow/stack/industrial_stack_9000w.py` & `simses-1.3.4/simses/technology/redox_flow/stack/industrial_stack_9000w.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/redox_flow/system.py` & `simses-1.3.4/simses/technology/redox_flow/system.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/redox_flow/test/test_stack_module.py` & `simses-1.3.4/simses/technology/redox_flow/test/test_stack_module.py`

 * *Files identical despite different names*

### Comparing `simses-1.3.3/simses/technology/storage.py` & `simses-1.3.4/simses/technology/storage.py`

 * *Files identical despite different names*

