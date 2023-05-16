# Comparing `tmp/gridworks_atn-0.3.4.tar.gz` & `tmp/gridworks_atn-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridworks_atn-0.3.4.tar", max compression
+gzip compressed data, was "gridworks_atn-0.3.5.tar", max compression
```

## Comparing `gridworks_atn-0.3.4.tar` & `gridworks_atn-0.3.5.tar`

### file list

```diff
@@ -1,91 +1,231 @@
--rw-r--r--   0        0        0     1065 2023-05-13 12:50:21.758958 gridworks_atn-0.3.4/LICENSE
--rw-r--r--   0        0        0     3002 2023-05-13 12:50:21.758958 gridworks_atn-0.3.4/README.md
--rw-r--r--   0        0        0     2193 2023-05-13 12:50:40.230938 gridworks_atn-0.3.4/pyproject.toml
--rw-r--r--   0        0        0      681 2023-05-13 12:50:21.766958 gridworks_atn-0.3.4/src/gwatn/__init__.py
--rw-r--r--   0        0        0      226 2023-05-13 12:50:21.766958 gridworks_atn-0.3.4/src/gwatn/__main__.py
--rw-r--r--   0        0        0    13411 2023-05-13 12:50:21.766958 gridworks_atn-0.3.4/src/gwatn/api_types.py
--rw-r--r--   0        0        0    21728 2023-05-13 12:50:21.766958 gridworks_atn-0.3.4/src/gwatn/atn_actor_base.py
--rw-r--r--   0        0        0     3114 2023-05-13 12:50:40.230938 gridworks_atn-0.3.4/src/gwatn/atn_utils.py
--rw-r--r--   0        0        0    19478 2023-05-13 12:50:21.766958 gridworks_atn-0.3.4/src/gwatn/brick_storage_heater/atn.py
--rw-r--r--   0        0        0       98 2023-05-13 12:50:21.766958 gridworks_atn-0.3.4/src/gwatn/brick_storage_heater/dev_atn_params_data.csv
--rw-r--r--   0        0        0      867 2023-05-13 12:50:21.766958 gridworks_atn-0.3.4/src/gwatn/brick_storage_heater/edge.py
--rw-r--r--   0        0        0     7536 2023-05-13 12:50:21.766958 gridworks_atn-0.3.4/src/gwatn/brick_storage_heater/flo.py
--rw-r--r--   0        0        0    18484 2023-05-13 12:50:21.766958 gridworks_atn-0.3.4/src/gwatn/brick_storage_heater/flo_output.py
--rw-r--r--   0        0        0     2014 2023-05-13 12:50:21.766958 gridworks_atn-0.3.4/src/gwatn/brick_storage_heater/make_dev_input_data.py
--rw-r--r--   0        0        0      841 2023-05-13 12:50:21.766958 gridworks_atn-0.3.4/src/gwatn/brick_storage_heater/node.py
--rw-r--r--   0        0        0     6963 2023-05-13 12:50:21.766958 gridworks_atn-0.3.4/src/gwatn/brick_storage_heater/simple_scada_sim.py
--rw-r--r--   0        0        0     2472 2023-05-13 12:50:21.766958 gridworks_atn-0.3.4/src/gwatn/brick_storage_heater/strategy_utils.py
--rw-r--r--   0        0        0     4575 2023-05-13 12:50:21.766958 gridworks_atn-0.3.4/src/gwatn/config.py
--rw-r--r--   0        0        0       43 2023-05-13 12:50:21.766958 gridworks_atn-0.3.4/src/gwatn/conversion_factors.py
--rw-r--r--   0        0        0     6148 2023-05-13 12:50:21.766958 gridworks_atn-0.3.4/src/gwatn/data_classes/.DS_Store
--rw-r--r--   0        0        0      677 2023-05-13 12:50:21.766958 gridworks_atn-0.3.4/src/gwatn/data_classes/__init__.py
--rw-r--r--   0        0        0      577 2023-05-13 12:50:21.766958 gridworks_atn-0.3.4/src/gwatn/data_classes/d_edge.py
--rw-r--r--   0        0        0     7812 2023-05-13 12:50:21.766958 gridworks_atn-0.3.4/src/gwatn/data_classes/d_graph.py
--rw-r--r--   0        0        0     1508 2023-05-13 12:50:21.766958 gridworks_atn-0.3.4/src/gwatn/data_classes/d_node.py
--rw-r--r--   0        0        0    14466 2023-05-13 12:50:21.766958 gridworks_atn-0.3.4/src/gwatn/demo_methods.py
--rw-r--r--   0        0        0      276 2023-05-13 12:50:21.766958 gridworks_atn-0.3.4/src/gwatn/dev_utils/__init__.py
--rw-r--r--   0        0        0     1792 2023-05-13 12:50:21.766958 gridworks_atn-0.3.4/src/gwatn/dev_utils/dev_discoverer.py
--rw-r--r--   0        0        0    11883 2023-05-13 12:50:21.766958 gridworks_atn-0.3.4/src/gwatn/dev_utils/dev_ta_owner.py
--rw-r--r--   0        0        0    10994 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/dev_utils/dev_validator.py
--rw-r--r--   0        0        0     1171 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/dev_utils/make_plants.py
--rw-r--r--   0        0        0    11409 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/dispatch_contract.py
--rw-r--r--   0        0        0    12463 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/dispatch_contract_artifacts/application.json
--rw-r--r--   0        0        0     5229 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/dispatch_contract_artifacts/approval.teal
--rw-r--r--   0        0        0       40 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/dispatch_contract_artifacts/clear.teal
--rw-r--r--   0        0        0     3937 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/dispatch_contract_artifacts/contract.json
--rw-r--r--   0        0        0     2069 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/enums/__init__.py
--rw-r--r--   0        0        0      700 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/enums/distribution_tariff.py
--rw-r--r--   0        0        0      614 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/enums/energy_supply_type.py
--rw-r--r--   0        0        0      947 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/enums/recognized_irradiance_type.py
--rw-r--r--   0        0        0      570 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/enums/recognized_temperature_unit.py
--rw-r--r--   0        0        0      122 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/errors.py
--rw-r--r--   0        0        0        0 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/py.typed
--rw-r--r--   0        0        0     7945 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/python_ta_daemon.json
--rw-r--r--   0        0        0    12518 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/python_ta_daemon.py
--rw-r--r--   0        0        0      834 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/scada_codec.py
--rw-r--r--   0        0        0     4870 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/simple_atn_actor.py
--rw-r--r--   0        0        0    26139 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/simple_scada_sim_actor_base.py
--rw-r--r--   0        0        0     3169 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/ta_daemon_rest_api.py
--rw-r--r--   0        0        0      460 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/ta_validator_rest_api.py
--rw-r--r--   0        0        0    47761 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/two_channel_actor_base.py
--rw-r--r--   0        0        0    13145 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/types/__init__.py
--rw-r--r--   0        0        0     7868 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/types/accepted_bid.py
--rw-r--r--   0        0        0    20222 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/types/atn_bid.py
--rw-r--r--   0        0        0     4288 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/types/atn_params.py
--rw-r--r--   0        0        0    22335 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/types/atn_params_brickstorageheater.py
--rw-r--r--   0        0        0     8144 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/types/atn_params_report.py
--rw-r--r--   0        0        0     8321 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/types/basegnode_scada_create.py
--rw-r--r--   0        0        0    11106 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/types/csv_distp_sync.py
--rw-r--r--   0        0        0    11354 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/types/csv_eprt_sync.py
--rw-r--r--   0        0        0    21761 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/types/csv_weather_forecast_sync.py
--rw-r--r--   0        0        0     1067 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/types/data_channel.py
--rw-r--r--   0        0        0     9885 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/types/discoverycert_algo_create.py
--rw-r--r--   0        0        0     8092 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/types/dispatch_contract_confirmed.py
--rw-r--r--   0        0        0     7648 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/types/flo_params.py
--rw-r--r--   0        0        0    22826 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/types/flo_params_brickstorageheater.py
--rw-r--r--   0        0        0     8827 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/types/flo_params_report.py
--rw-r--r--   0        0        0     8206 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/types/gt_dispatch_boolean.py
--rw-r--r--   0        0        0     9155 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/types/heartbeat_b.py
--rw-r--r--   0        0        0     6154 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/types/initial_tadeed_algo_create.py
--rw-r--r--   0        0        0     7610 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/types/initial_tadeed_algo_optin.py
--rw-r--r--   0        0        0     8932 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/types/initial_tadeed_algo_transfer.py
--rw-r--r--   0        0        0     7959 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/types/join_dispatch_contract.py
--rw-r--r--   0        0        0    12429 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/types/latest_price.py
--rw-r--r--   0        0        0     5028 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/types/market_slot.py
--rw-r--r--   0        0        0    17161 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/types/market_type_gt.py
--rw-r--r--   0        0        0     5294 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/types/new_tadeed_algo_optin.py
--rw-r--r--   0        0        0     5196 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/types/new_tadeed_send.py
--rw-r--r--   0        0        0     5024 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/types/old_tadeed_algo_return.py
--rw-r--r--   0        0        0     8461 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/types/price_quantity.py
--rw-r--r--   0        0        0     2492 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/types/price_quantity_unitless.py
--rw-r--r--   0        0        0     5004 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/types/scada_cert_transfer.py
--rw-r--r--   0        0        0     3682 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/types/simplesim_driver_data.py
--rw-r--r--   0        0        0     4166 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/types/simplesim_driver_data_bsh.py
--rw-r--r--   0        0        0     6534 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/types/simplesim_driver_report.py
--rw-r--r--   0        0        0     6774 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/types/simplesim_snapshot_brickstorageheater.py
--rw-r--r--   0        0        0     3220 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/types/sla_enter.py
--rw-r--r--   0        0        0     4101 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/types/tadeed_specs_hack.py
--rw-r--r--   0        0        0     5734 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/types/tavalidatorcert_algo_create.py
--rw-r--r--   0        0        0     6371 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/types/tavalidatorcert_algo_transfer.py
--rw-r--r--   0        0        0     5242 2023-05-13 12:50:21.770959 gridworks_atn-0.3.4/src/gwatn/types/terminalasset_certify_hack.py
--rw-r--r--   0        0        0     3949 1970-01-01 00:00:00.000000 gridworks_atn-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-16 14:09:47.334500 gridworks_atn-0.3.5/LICENSE
+-rw-r--r--   0        0        0     3002 2023-05-16 14:09:47.334500 gridworks_atn-0.3.5/README.md
+-rw-r--r--   0        0        0     2193 2023-05-16 14:10:07.150559 gridworks_atn-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      681 2023-05-16 14:09:47.346500 gridworks_atn-0.3.5/src/gwatn/__init__.py
+-rw-r--r--   0        0        0      226 2023-05-16 14:09:47.346500 gridworks_atn-0.3.5/src/gwatn/__main__.py
+-rw-r--r--   0        0        0    13411 2023-05-16 14:09:47.346500 gridworks_atn-0.3.5/src/gwatn/api_types.py
+-rw-r--r--   0        0        0    21728 2023-05-16 14:10:07.150559 gridworks_atn-0.3.5/src/gwatn/atn_actor_base.py
+-rw-r--r--   0        0        0     3114 2023-05-16 14:09:47.346500 gridworks_atn-0.3.5/src/gwatn/atn_utils.py
+-rw-r--r--   0        0        0    19983 2023-05-16 14:10:07.150559 gridworks_atn-0.3.5/src/gwatn/brick_storage_heater/atn.py
+-rw-r--r--   0        0        0       98 2023-05-16 14:09:47.346500 gridworks_atn-0.3.5/src/gwatn/brick_storage_heater/dev_atn_params_data.csv
+-rw-r--r--   0        0        0     7196 2023-05-16 14:10:07.150559 gridworks_atn-0.3.5/src/gwatn/brick_storage_heater/dev_io.py
+-rw-r--r--   0        0        0      867 2023-05-16 14:09:47.346500 gridworks_atn-0.3.5/src/gwatn/brick_storage_heater/edge.py
+-rw-r--r--   0        0        0     7536 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/brick_storage_heater/flo.py
+-rw-r--r--   0        0        0    18355 2023-05-16 14:10:07.150559 gridworks_atn-0.3.5/src/gwatn/brick_storage_heater/flo_output.py
+-rw-r--r--   0        0        0     2014 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/brick_storage_heater/make_dev_input_data.py
+-rw-r--r--   0        0        0      841 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/brick_storage_heater/node.py
+-rw-r--r--   0        0        0     6963 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/brick_storage_heater/simple_scada_sim.py
+-rw-r--r--   0        0        0     2671 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/brick_storage_heater/strategy_utils.py
+-rw-r--r--   0        0        0     4575 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/config.py
+-rw-r--r--   0        0        0       43 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/conversion_factors.py
+-rw-r--r--   0        0        0     6148 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/data_classes/.DS_Store
+-rw-r--r--   0        0        0      935 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/data_classes/__init__.py
+-rw-r--r--   0        0        0      577 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/data_classes/d_edge.py
+-rw-r--r--   0        0        0     7812 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/data_classes/d_graph.py
+-rw-r--r--   0        0        0     1508 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/data_classes/d_node.py
+-rw-r--r--   0        0        0     8684 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/data_classes/hack_price_method.py
+-rw-r--r--   0        0        0     4082 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/data_classes/hack_weather_location.py
+-rw-r--r--   0        0        0     2104 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/data_classes/hack_weather_source.py
+-rw-r--r--   0        0        0    14466 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/demo_methods.py
+-rw-r--r--   0        0        0      276 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/dev_utils/__init__.py
+-rw-r--r--   0        0        0     1792 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/dev_utils/dev_discoverer.py
+-rw-r--r--   0        0        0    11883 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/dev_utils/dev_ta_owner.py
+-rw-r--r--   0        0        0    10994 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/dev_utils/dev_validator.py
+-rw-r--r--   0        0        0     1171 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/dev_utils/make_plants.py
+-rw-r--r--   0        0        0    11409 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/dispatch_contract.py
+-rw-r--r--   0        0        0    12463 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/dispatch_contract_artifacts/application.json
+-rw-r--r--   0        0        0     5229 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/dispatch_contract_artifacts/approval.teal
+-rw-r--r--   0        0        0       40 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/dispatch_contract_artifacts/clear.teal
+-rw-r--r--   0        0        0     3937 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/dispatch_contract_artifacts/contract.json
+-rw-r--r--   0        0        0     2402 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/enums/__init__.py
+-rw-r--r--   0        0        0      700 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/enums/distribution_tariff.py
+-rw-r--r--   0        0        0      614 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/enums/energy_supply_type.py
+-rw-r--r--   0        0        0     1308 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/enums/hack_price_method.py
+-rw-r--r--   0        0        0      415 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/enums/hack_recognized_p_node_alias.py
+-rw-r--r--   0        0        0      552 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/enums/hack_weather_method.py
+-rw-r--r--   0        0        0      132 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/enums/hack_weather_source.py
+-rw-r--r--   0        0        0      947 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/enums/recognized_irradiance_type.py
+-rw-r--r--   0        0        0      570 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/enums/recognized_temperature_unit.py
+-rw-r--r--   0        0        0      122 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/errors.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/py.typed
+-rw-r--r--   0        0        0     7945 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/python_ta_daemon.json
+-rw-r--r--   0        0        0    12518 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/python_ta_daemon.py
+-rw-r--r--   0        0        0      834 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/scada_codec.py
+-rw-r--r--   0        0        0     4870 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/simple_atn_actor.py
+-rw-r--r--   0        0        0    26139 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/simple_scada_sim_actor_base.py
+-rw-r--r--   0        0        0     3169 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/ta_daemon_rest_api.py
+-rw-r--r--   0        0        0      460 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/ta_validator_rest_api.py
+-rw-r--r--   0        0        0    47761 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/two_channel_actor_base.py
+-rw-r--r--   0        0        0    13145 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/types/__init__.py
+-rw-r--r--   0        0        0     7868 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/types/accepted_bid.py
+-rw-r--r--   0        0        0    20222 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/types/atn_bid.py
+-rw-r--r--   0        0        0     4288 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/types/atn_params.py
+-rw-r--r--   0        0        0    22335 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/types/atn_params_brickstorageheater.py
+-rw-r--r--   0        0        0     8144 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/types/atn_params_report.py
+-rw-r--r--   0        0        0     8321 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/types/basegnode_scada_create.py
+-rw-r--r--   0        0        0    11106 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/types/csv_distp_sync.py
+-rw-r--r--   0        0        0    11354 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/types/csv_eprt_sync.py
+-rw-r--r--   0        0        0    21761 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/types/csv_weather_forecast_sync.py
+-rw-r--r--   0        0        0     1067 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/types/data_channel.py
+-rw-r--r--   0        0        0     9885 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/types/discoverycert_algo_create.py
+-rw-r--r--   0        0        0     8092 2023-05-16 14:09:47.350500 gridworks_atn-0.3.5/src/gwatn/types/dispatch_contract_confirmed.py
+-rw-r--r--   0        0        0     3235 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/epda/gt_epda_actual_1_0_0.py
+-rw-r--r--   0        0        0      555 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/epda/gt_epda_actual_1_0_0_payload.py
+-rw-r--r--   0        0        0     3959 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/epda/gt_epda_actual_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     3338 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/eprt/gt_eprt_actual_1_0_0.py
+-rw-r--r--   0        0        0      555 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/eprt/gt_eprt_actual_1_0_0_payload.py
+-rw-r--r--   0        0        0     3959 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/eprt/gt_eprt_actual_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     3658 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/eprt/gt_eprt_forecast_sync_1_0_0.py
+-rw-r--r--   0        0        0     1690 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/eprt/gt_eprt_forecast_sync_1_0_0_payload.py
+-rw-r--r--   0        0        0     4905 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/eprt/gt_eprt_forecast_sync_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     7648 2023-05-16 14:09:47.354500 gridworks_atn-0.3.5/src/gwatn/types/flo_params.py
+-rw-r--r--   0        0        0    22826 2023-05-16 14:09:47.354500 gridworks_atn-0.3.5/src/gwatn/types/flo_params_brickstorageheater.py
+-rw-r--r--   0        0        0     8827 2023-05-16 14:09:47.354500 gridworks_atn-0.3.5/src/gwatn/types/flo_params_report.py
+-rw-r--r--   0        0        0     3885 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_req/r_gnode_distp_req_1_0_0.py
+-rw-r--r--   0        0        0      600 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_req/r_gnode_distp_req_1_0_0_payload.py
+-rw-r--r--   0        0        0     4184 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_req/r_gnode_distp_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5457 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_sync_req/r_gnode_distp_sync_req_1_0_0.py
+-rw-r--r--   0        0        0      620 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_sync_req/r_gnode_distp_sync_req_1_0_0_payload.py
+-rw-r--r--   0        0        0     7905 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_sync_req/r_gnode_distp_sync_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5419 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/gnode_eprequest_ps/r_get_eprt_forecast_sync/r_get_eprt_forecast_sync_1_0_0.py
+-rw-r--r--   0        0        0      625 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/gnode_eprequest_ps/r_get_eprt_forecast_sync/r_get_eprt_forecast_sync_1_0_0_payload.py
+-rw-r--r--   0        0        0     7913 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/gnode_eprequest_ps/r_get_eprt_forecast_sync/r_get_eprt_forecast_sync_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5176 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_forecast_cron_req/r_gnode_eprt_forecast_cron_req_1_0_0.py
+-rw-r--r--   0        0        0      649 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_forecast_cron_req/r_gnode_eprt_forecast_cron_req_1_0_0_payload.py
+-rw-r--r--   0        0        0     8053 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_forecast_cron_req/r_gnode_eprt_forecast_cron_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     3885 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_req/r_gnode_eprt_req_1_0_0.py
+-rw-r--r--   0        0        0      593 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_req/r_gnode_eprt_req_1_0_0_payload.py
+-rw-r--r--   0        0        0     4203 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_req/r_gnode_eprt_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5392 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_sync_req/r_gnode_eprt_sync_req_1_0_0.py
+-rw-r--r--   0        0        0      613 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_sync_req/r_gnode_eprt_sync_req_1_0_0_payload.py
+-rw-r--r--   0        0        0     7891 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_sync_req/r_gnode_eprt_sync_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     3909 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_uid_req/r_gnode_eprt_uid_req_1_0_0.py
+-rw-r--r--   0        0        0      609 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_uid_req/r_gnode_eprt_uid_req_1_0_0_payload.py
+-rw-r--r--   0        0        0     4212 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_uid_req/r_gnode_eprt_uid_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     7507 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_cron_req/r_gnode_weather_forecast_cron_req_1_0_0.py
+-rw-r--r--   0        0        0     1453 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_cron_req/r_gnode_weather_forecast_cron_req_1_0_0_payload.py
+-rw-r--r--   0        0        0    12856 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_cron_req/r_gnode_weather_forecast_cron_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     7530 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_sync_req/r_gnode_weather_forecast_sync_req_1_0_0.py
+-rw-r--r--   0        0        0     1453 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_sync_req/r_gnode_weather_forecast_sync_req_1_0_0_payload.py
+-rw-r--r--   0        0        0    11873 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_sync_req/r_gnode_weather_forecast_sync_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     3980 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_req/r_gnode_weather_req_1_0_0.py
+-rw-r--r--   0        0        0      611 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_req/r_gnode_weather_req_1_0_0_payload.py
+-rw-r--r--   0        0        0     4060 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_req/r_gnode_weather_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     4083 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_uid_req/r_gnode_weather_uid_req_1_0_0.py
+-rw-r--r--   0        0        0      627 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_uid_req/r_gnode_weather_uid_req_1_0_0_payload.py
+-rw-r--r--   0        0        0     4430 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_uid_req/r_gnode_weather_uid_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     3879 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_req/r_gnode_regp_req_1_0_0.py
+-rw-r--r--   0        0        0      595 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_req/r_gnode_regp_req_1_0_0_payload.py
+-rw-r--r--   0        0        0     4196 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_req/r_gnode_regp_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5398 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_sync_req/r_gnode_regp_sync_req_1_0_0.py
+-rw-r--r--   0        0        0      615 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_sync_req/r_gnode_regp_sync_req_1_0_0_payload.py
+-rw-r--r--   0        0        0     7901 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_sync_req/r_gnode_regp_sync_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     8206 2023-05-16 14:09:47.354500 gridworks_atn-0.3.5/src/gwatn/types/gt_dispatch_boolean.py
+-rw-r--r--   0        0        0    14769 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/hack_property_format.py
+-rw-r--r--   0        0        0      194 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/hack_test_dummy.py
+-rw-r--r--   0        0        0      781 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/hack_type_base.py
+-rw-r--r--   0        0        0      990 2023-05-16 14:10:07.154559 gridworks_atn-0.3.5/src/gwatn/types/hack_utils.py
+-rw-r--r--   0        0        0     9155 2023-05-16 14:09:47.354500 gridworks_atn-0.3.5/src/gwatn/types/heartbeat_b.py
+-rw-r--r--   0        0        0     6154 2023-05-16 14:09:47.354500 gridworks_atn-0.3.5/src/gwatn/types/initial_tadeed_algo_create.py
+-rw-r--r--   0        0        0     7610 2023-05-16 14:09:47.354500 gridworks_atn-0.3.5/src/gwatn/types/initial_tadeed_algo_optin.py
+-rw-r--r--   0        0        0     8932 2023-05-16 14:09:47.354500 gridworks_atn-0.3.5/src/gwatn/types/initial_tadeed_algo_transfer.py
+-rw-r--r--   0        0        0     7959 2023-05-16 14:09:47.354500 gridworks_atn-0.3.5/src/gwatn/types/join_dispatch_contract.py
+-rw-r--r--   0        0        0    12429 2023-05-16 14:09:47.354500 gridworks_atn-0.3.5/src/gwatn/types/latest_price.py
+-rw-r--r--   0        0        0     5028 2023-05-16 14:09:47.354500 gridworks_atn-0.3.5/src/gwatn/types/market_slot.py
+-rw-r--r--   0        0        0    17161 2023-05-16 14:09:47.358500 gridworks_atn-0.3.5/src/gwatn/types/market_type_gt.py
+-rw-r--r--   0        0        0     5294 2023-05-16 14:09:47.358500 gridworks_atn-0.3.5/src/gwatn/types/new_tadeed_algo_optin.py
+-rw-r--r--   0        0        0     5196 2023-05-16 14:09:47.358500 gridworks_atn-0.3.5/src/gwatn/types/new_tadeed_send.py
+-rw-r--r--   0        0        0     5024 2023-05-16 14:09:47.358500 gridworks_atn-0.3.5/src/gwatn/types/old_tadeed_algo_return.py
+-rw-r--r--   0        0        0     8461 2023-05-16 14:09:47.358500 gridworks_atn-0.3.5/src/gwatn/types/price_quantity.py
+-rw-r--r--   0        0        0     2492 2023-05-16 14:09:47.358500 gridworks_atn-0.3.5/src/gwatn/types/price_quantity_unitless.py
+-rw-r--r--   0        0        0    13837 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_distprices_gnode/csv_distp/csv_distp_1_0_0.py
+-rw-r--r--   0        0        0    13162 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_distprices_gnode/csv_distp_oneprice/csv_distp_oneprice_1_0_0.py
+-rw-r--r--   0        0        0    14105 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_distprices_gnode/csv_distp_sync/csv_distp_sync_1_0_0.py
+-rw-r--r--   0        0        0     5624 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_distprices_gnode/r_distp/r_distp_1_0_0.py
+-rw-r--r--   0        0        0      558 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_distprices_gnode/r_distp/r_distp_1_0_0_payload.py
+-rw-r--r--   0        0        0     8026 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_distprices_gnode/r_distp/r_distp_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5026 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_distprices_gnode/r_distp_oneprice/r_distp_oneprice_1_0_0.py
+-rw-r--r--   0        0        0      594 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_distprices_gnode/r_distp_oneprice/r_distp_oneprice_1_0_0_payload.py
+-rw-r--r--   0        0        0     7236 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_distprices_gnode/r_distp_oneprice/r_distp_oneprice_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5890 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_distprices_gnode/r_distp_sync/r_distp_sync_1_0_0.py
+-rw-r--r--   0        0        0      578 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_distprices_gnode/r_distp_sync/r_distp_sync_1_0_0_payload.py
+-rw-r--r--   0        0        0     7750 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_distprices_gnode/r_distp_sync/r_distp_sync_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     7618 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_electricityprices_gnode/csv_epda_actual/csv_epda_actual_1_0_0.py
+-rw-r--r--   0        0        0    13827 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_electricityprices_gnode/csv_eprt/csv_eprt_1_0_0.py
+-rw-r--r--   0        0        0     7319 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_actual/csv_eprt_actual_1_0_0.py
+-rw-r--r--   0        0        0    12667 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_forecast/csv_eprt_forecast_1_0_0.py
+-rw-r--r--   0        0        0     8872 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_forecast_sync/csv_eprt_forecast_sync_1_0_0.py
+-rw-r--r--   0        0        0    10345 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_forecast_sync_table/csv_eprt_forecast_sync_table_1_0_0.py
+-rw-r--r--   0        0        0    14435 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_sync/csv_eprt_sync_1_0_0.py
+-rw-r--r--   0        0        0     4044 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_electricityprices_gnode/r_epda_actual/r_epda_actual_1_0_0.py
+-rw-r--r--   0        0        0      589 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_electricityprices_gnode/r_epda_actual/r_epda_actual_1_0_0_payload.py
+-rw-r--r--   0        0        0     3804 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_electricityprices_gnode/r_epda_actual/r_epda_actual_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5402 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_electricityprices_gnode/r_eprt/r_eprt_1_0_0.py
+-rw-r--r--   0        0        0      561 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_electricityprices_gnode/r_eprt/r_eprt_1_0_0_payload.py
+-rw-r--r--   0        0        0     7263 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_electricityprices_gnode/r_eprt/r_eprt_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     4044 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_electricityprices_gnode/r_eprt_actual/r_eprt_actual_1_0_0.py
+-rw-r--r--   0        0        0      589 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_electricityprices_gnode/r_eprt_actual/r_eprt_actual_1_0_0_payload.py
+-rw-r--r--   0        0        0     3804 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_electricityprices_gnode/r_eprt_actual/r_eprt_actual_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5661 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast/r_eprt_forecast_1_0_0.py
+-rw-r--r--   0        0        0      597 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast/r_eprt_forecast_1_0_0_payload.py
+-rw-r--r--   0        0        0     7829 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast/r_eprt_forecast_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     3535 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_cron_response/r_eprt_forecast_cron_response_1_0_0.py
+-rw-r--r--   0        0        0      653 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_cron_response/r_eprt_forecast_cron_response_1_0_0_payload.py
+-rw-r--r--   0        0        0     3064 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_cron_response/r_eprt_forecast_cron_response_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     4184 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_sync/r_eprt_forecast_sync_1_0_0.py
+-rw-r--r--   0        0        0      586 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_sync/r_eprt_forecast_sync_1_0_0_payload.py
+-rw-r--r--   0        0        0     3863 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_sync/r_eprt_forecast_sync_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5892 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_electricityprices_gnode/r_eprt_sync/r_eprt_sync_1_0_0.py
+-rw-r--r--   0        0        0      581 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_electricityprices_gnode/r_eprt_sync/r_eprt_sync_1_0_0_payload.py
+-rw-r--r--   0        0        0     7746 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_electricityprices_gnode/r_eprt_sync/r_eprt_sync_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     3707 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_electricityprices_gnode/r_ps_penpal/r_ps_penpal_1_0_0.py
+-rw-r--r--   0        0        0      581 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_electricityprices_gnode/r_ps_penpal/r_ps_penpal_1_0_0_payload.py
+-rw-r--r--   0        0        0     3547 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_electricityprices_gnode/r_ps_penpal/r_ps_penpal_1_0_0_payload_base.py
+-rw-r--r--   0        0        0    13926 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_regprices_gnode/csv_regp/csv_regp_1_0_0.py
+-rw-r--r--   0        0        0    14182 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_regprices_gnode/csv_regp_sync/csv_regp_sync_1_0_0.py
+-rw-r--r--   0        0        0     5617 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_regprices_gnode/r_regp/r_regp_1_0_0.py
+-rw-r--r--   0        0        0      544 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_regprices_gnode/r_regp/r_regp_1_0_0_payload.py
+-rw-r--r--   0        0        0     8022 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_regprices_gnode/r_regp/r_regp_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5864 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_regprices_gnode/r_regp_sync/r_regp_sync_1_0_0.py
+-rw-r--r--   0        0        0      573 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_regprices_gnode/r_regp_sync/r_regp_sync_1_0_0_payload.py
+-rw-r--r--   0        0        0     7746 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ps_regprices_gnode/r_regp_sync/r_regp_sync_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5004 2023-05-16 14:09:47.362500 gridworks_atn-0.3.5/src/gwatn/types/scada_cert_transfer.py
+-rw-r--r--   0        0        0     3682 2023-05-16 14:09:47.362500 gridworks_atn-0.3.5/src/gwatn/types/simplesim_driver_data.py
+-rw-r--r--   0        0        0     4166 2023-05-16 14:09:47.362500 gridworks_atn-0.3.5/src/gwatn/types/simplesim_driver_data_bsh.py
+-rw-r--r--   0        0        0     6534 2023-05-16 14:09:47.362500 gridworks_atn-0.3.5/src/gwatn/types/simplesim_driver_report.py
+-rw-r--r--   0        0        0     6774 2023-05-16 14:09:47.362500 gridworks_atn-0.3.5/src/gwatn/types/simplesim_snapshot_brickstorageheater.py
+-rw-r--r--   0        0        0     3220 2023-05-16 14:09:47.362500 gridworks_atn-0.3.5/src/gwatn/types/sla_enter.py
+-rw-r--r--   0        0        0     4101 2023-05-16 14:09:47.362500 gridworks_atn-0.3.5/src/gwatn/types/tadeed_specs_hack.py
+-rw-r--r--   0        0        0     5734 2023-05-16 14:09:47.362500 gridworks_atn-0.3.5/src/gwatn/types/tavalidatorcert_algo_create.py
+-rw-r--r--   0        0        0     6371 2023-05-16 14:09:47.362500 gridworks_atn-0.3.5/src/gwatn/types/tavalidatorcert_algo_transfer.py
+-rw-r--r--   0        0        0     5242 2023-05-16 14:09:47.362500 gridworks_atn-0.3.5/src/gwatn/types/terminalasset_certify_hack.py
+-rw-r--r--   0        0        0    30475 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ws_forecast_gnode/csv_weather_forecast_raw/csv_weather_forecast_raw_1_0_0.py
+-rw-r--r--   0        0        0    29247 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ws_forecast_gnode/csv_weather_forecast_sync/csv_weather_forecast_sync_1_0_0.py
+-rw-r--r--   0        0        0     8474 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ws_forecast_gnode/r_weather_forecast/r_weather_forecast_1_0_0.py
+-rw-r--r--   0        0        0     1920 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ws_forecast_gnode/r_weather_forecast/r_weather_forecast_1_0_0_payload.py
+-rw-r--r--   0        0        0    13416 2023-05-16 14:10:07.158559 gridworks_atn-0.3.5/src/gwatn/types/ws_forecast_gnode/r_weather_forecast/r_weather_forecast_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     3535 2023-05-16 14:10:07.162559 gridworks_atn-0.3.5/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_cron_response/r_weather_forecast_cron_response_1_0_0.py
+-rw-r--r--   0        0        0      686 2023-05-16 14:10:07.162559 gridworks_atn-0.3.5/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_cron_response/r_weather_forecast_cron_response_1_0_0_payload.py
+-rw-r--r--   0        0        0     3076 2023-05-16 14:10:07.162559 gridworks_atn-0.3.5/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_cron_response/r_weather_forecast_cron_response_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     7834 2023-05-16 14:10:07.162559 gridworks_atn-0.3.5/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_raw/r_weather_forecast_raw_1_0_0.py
+-rw-r--r--   0        0        0      829 2023-05-16 14:10:07.162559 gridworks_atn-0.3.5/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_raw/r_weather_forecast_raw_1_0_0_payload.py
+-rw-r--r--   0        0        0    12801 2023-05-16 14:10:07.162559 gridworks_atn-0.3.5/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_raw/r_weather_forecast_raw_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     8628 2023-05-16 14:10:07.162559 gridworks_atn-0.3.5/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_sync/r_weather_forecast_sync_1_0_0.py
+-rw-r--r--   0        0        0     1153 2023-05-16 14:10:07.162559 gridworks_atn-0.3.5/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_sync/r_weather_forecast_sync_1_0_0_payload.py
+-rw-r--r--   0        0        0    12807 2023-05-16 14:10:07.162559 gridworks_atn-0.3.5/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_sync/r_weather_forecast_sync_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     3671 2023-05-16 14:10:07.162559 gridworks_atn-0.3.5/src/gwatn/types/ws_forecast_gnode/r_ws_penpal/r_ws_penpal_1_0_0.py
+-rw-r--r--   0        0        0      572 2023-05-16 14:10:07.162559 gridworks_atn-0.3.5/src/gwatn/types/ws_forecast_gnode/r_ws_penpal/r_ws_penpal_1_0_0_payload.py
+-rw-r--r--   0        0        0     3547 2023-05-16 14:10:07.162559 gridworks_atn-0.3.5/src/gwatn/types/ws_forecast_gnode/r_ws_penpal/r_ws_penpal_1_0_0_payload_base.py
+-rw-r--r--   0        0        0    14909 2023-05-16 14:10:07.162559 gridworks_atn-0.3.5/src/gwatn/types/ws_irradiances_gnode/csv_irradiance_poa_sync/csv_irradiance_poa_sync_1_0_0.py
+-rw-r--r--   0        0        0    11616 2023-05-16 14:10:07.162559 gridworks_atn-0.3.5/src/gwatn/types/ws_irradiances_gnode/csv_irradiance_poa_template/csv_irradiance_poa_template_1_0_0.py
+-rw-r--r--   0        0        0     4544 2023-05-16 14:10:07.162559 gridworks_atn-0.3.5/src/gwatn/types/ws_irradiances_gnode/r_irradiance_poa_template/r_irradiance_poa_template_1_0_0.py
+-rw-r--r--   0        0        0      631 2023-05-16 14:10:07.162559 gridworks_atn-0.3.5/src/gwatn/types/ws_irradiances_gnode/r_irradiance_poa_template/r_irradiance_poa_template_1_0_0_payload.py
+-rw-r--r--   0        0        0     6001 2023-05-16 14:10:07.162559 gridworks_atn-0.3.5/src/gwatn/types/ws_irradiances_gnode/r_irradiance_poa_template/r_irradiance_poa_template_1_0_0_payload_base.py
+-rw-r--r--   0        0        0    12321 2023-05-16 14:10:07.162559 gridworks_atn-0.3.5/src/gwatn/types/ws_typicalmodeledyear_gnode/csv_weather_tmy_temp/csv_weather_tmy_temp_1_0_0.py
+-rw-r--r--   0        0        0     6939 2023-05-16 14:10:07.162559 gridworks_atn-0.3.5/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_solarandtemp/r_weather_tmy_solarandtemp_1_0_0.py
+-rw-r--r--   0        0        0      642 2023-05-16 14:10:07.162559 gridworks_atn-0.3.5/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_solarandtemp/r_weather_tmy_solarandtemp_1_0_0_payload.py
+-rw-r--r--   0        0        0    10751 2023-05-16 14:10:07.162559 gridworks_atn-0.3.5/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_solarandtemp/r_weather_tmy_solarandtemp_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     4677 2023-05-16 14:10:07.162559 gridworks_atn-0.3.5/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_temp/r_weather_tmy_temp_1_0_0.py
+-rw-r--r--   0        0        0      610 2023-05-16 14:10:07.162559 gridworks_atn-0.3.5/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_temp/r_weather_tmy_temp_1_0_0_payload.py
+-rw-r--r--   0        0        0     6741 2023-05-16 14:10:07.162559 gridworks_atn-0.3.5/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_temp/r_weather_tmy_temp_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     3949 1970-01-01 00:00:00.000000 gridworks_atn-0.3.5/PKG-INFO
```

### Comparing `gridworks_atn-0.3.4/LICENSE` & `gridworks_atn-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/README.md` & `gridworks_atn-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/pyproject.toml` & `gridworks_atn-0.3.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gridworks-atn"
-version = "0.3.4"
+version = "0.3.5"
 description = "Gridworks Atn Spaceheat"
 authors = ["Jessica Millar <jmillar@gridworks-consulting.com>"]
 license = "None"
 readme = "README.md"
 homepage = "https://github.com/thegridelectric/gridworks-atn"
 repository = "https://github.com/thegridelectric/gridworks-atn"
 documentation = "https://gridworks-atn.readthedocs.io"
```

### Comparing `gridworks_atn-0.3.4/src/gwatn/__init__.py` & `gridworks_atn-0.3.5/src/gwatn/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/api_types.py` & `gridworks_atn-0.3.5/src/gwatn/api_types.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/atn_actor_base.py` & `gridworks_atn-0.3.5/src/gwatn/atn_actor_base.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -227,36 +227,36 @@
         raise NotImplementedError
 
     def _process_gt_sh_status_event_from_scada(self, payload: GtShStatusEvent) -> None:
         """Atn has received gridworks.event.gt.sh.status message from its SCADA"""
         gt_sh_status = payload.status
         self._process_gt_sh_status_from_scada(payload=gt_sh_status)
 
+    @abstractmethod
+    def _process_gt_sh_status_from_scada(self, payload: GtShStatus) -> None:
+        """Atn has received gt.sh.status message from its SCADA"""
+        raise NotImplementedError
+
     def _process_snapshot_spaceheat_event_from_scada(
         self, payload: SnapshotSpaceheatEvent
     ) -> None:
         """Atn has received  gridworks.event.snapshot.spaceheat message from its SCADA"""
         snapshot_spaceheat = payload.snap
         self._process_snapshot_spaceheat_from_scada(payload=snapshot_spaceheat)
 
     @abstractmethod
-    def _process_gt_sh_status_from_scada(self, payload: GtShStatus) -> None:
-        """Atn has received gt.sh.status message from its SCADA"""
+    def _process_snapshot_spaceheat_from_scada(self, payload: SnapshotSpaceheat):
+        """Atn has received a snapshot.sspaceheat message from the SCADA"""
         raise NotImplementedError
 
     @abstractmethod
     def _process_power_watts_from_scada(self, payload: PowerWatts) -> None:
         """Atn has received power.watts message from its SCADA"""
         raise NotImplementedError
 
-    @abstractmethod
-    def _process_snapshot_spaceheat_from_scada(self, payload: SnapshotSpaceheat):
-        """Atn has received a snapshot.sspaceheat message from the SCADA"""
-        raise NotImplementedError
-
     def route_message(
         self, from_alias: str, from_role: GNodeRole, payload: HeartbeatA
     ) -> None:
         self.payload = payload
         if payload.TypeName == HeartbeatA_Maker.type_name:
             if from_role != GNodeRole.Supervisor:
                 LOGGER.info(
```

### Comparing `gridworks_atn-0.3.4/src/gwatn/atn_utils.py` & `gridworks_atn-0.3.5/src/gwatn/atn_utils.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/brick_storage_heater/atn.py` & `gridworks_atn-0.3.5/src/gwatn/brick_storage_heater/atn.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,38 +10,36 @@
  """
 import functools
 import logging
 import math
 import random
 import time
 import uuid
+from typing import Optional
 from typing import no_type_check
 
 import dotenv
 import gridworks.algo_utils as algo_utils
 import pendulum
 import requests
-import satn.strategies.heatpumpwithbooststore.atn_utils as atn_utils
-import satn.strategies.heatpumpwithbooststore.dev_io as dev_io
 from algosdk import encoding
 from algosdk.future import transaction
 from algosdk.v2client.algod import AlgodClient
 from gridworks.algo_utils import BasicAccount
+from gridworks.data_classes.market_type import Rt60Gate30B
 from gridworks.utils import RestfulResponse
-from satn.strategies.heatpumpwithbooststore.atn_utils import SlotStuff
-from satn.strategies.heatpumpwithbooststore.edge import (
-    Edge__SpaceHeat__Water_HeatPumpAndBoost__Alpha as Edge,
-)
-from satn.strategies.heatpumpwithbooststore.flo import (
-    HeatPumpWithBoostStore__Flo as Flo,
-)
 
+import gwatn.atn_utils as atn_utils
+import gwatn.brick_storage_heater.dev_io as dev_io
+import gwatn.brick_storage_heater.strategy_utils as strategy_utils
 import gwatn.config as config
 from gwatn.atn_actor_base import AtnActorBase
-from gwatn.data_classes.market_type import Rt60Gate30B
+from gwatn.brick_storage_heater.edge import Edge__BrickStorageHeater as Edge
+from gwatn.brick_storage_heater.flo import Flo__BrickStorageHeater as Flo
+from gwatn.brick_storage_heater.strategy_utils import SlotStuff
 from gwatn.enums import GNodeRole
 from gwatn.enums import MessageCategory
 from gwatn.enums import MessageCategorySymbol
 from gwatn.enums import UniverseType
 from gwatn.types import AcceptedBid_Maker
 from gwatn.types import AtnParamsBrickstorageheater as AtnParams
 from gwatn.types import AtnParamsReport_Maker
@@ -79,26 +77,27 @@
         super().__init__(settings)
         LOGGER.info("Initializing HeatPumpWithBoostStore Atn")
         self.algo_acct: BasicAccount = BasicAccount(settings.sk.get_secret_value())
         self.algo_client: AlgodClient = AlgodClient(
             settings.algo_api_secrets.algod_token.get_secret_value(),
             settings.public.algod_address,
         )
-        self.atn_params: AtnParams = atn_utils.dummy_atn_params()
+        if self.universe_type == UniverseType.Dev:
+            self.atn_params: AtnParams = strategy_utils.dummy_atn_params()
+        else:
+            self.get_initial_params()
         self.market_type: MarketTypeGt = MarketTypeGt_Maker.dc_to_tuple(Rt60Gate30B)
-        self.active_run: SlotStuff = atn_utils.dummy_slot_stuff(
+        self.active_run: SlotStuff = strategy_utils.dummy_slot_stuff(
             slot=self.active_slot(self.market_type)
         )
-        self.next_run: SlotStuff = atn_utils.dummy_slot_stuff(
+        self.next_run: SlotStuff = strategy_utils.dummy_slot_stuff(
             slot=self.next_slot(self.market_type)
         )
         self.store_kwh: float = 0
-        self.heatpump_kw: float = 0
-        self.boost_kw: float = 0
-        self.cop: float = 2.5
+        self._power_watts: Optional[int] = None
         self.store_update_time: float = self.time()
         self.latest_price_received_time: float = 0
         self.latest_price_dollars_per_mwh: float = 10**6
         self._first_start_finished: bool = False
 
     @no_type_check
     def strategy_rabbit_startup(self) -> None:
@@ -118,14 +117,15 @@
             to_role=GNodeRole.Supervisor,
             to_g_node_alias=self.settings.my_super_alias,
         )
         d = pendulum.from_timestamp(time.time())
         LOGGER.warning(
             f"[{self.short_alias}] Sent first heartbeat to super: {d.minute}:{d.second}.{d.microsecond}"
         )
+        self._first_start_finished = True
 
     @no_type_check
     def on_marketprice_bindok(self, _unused_frame, binding) -> None:
         LOGGER.info(f"Queue {self.queue_name} bound with {binding}")
 
     def heartbeat_received(self, from_alias: str, ping: HeartbeatA):
         pong = HeartbeatA_Maker(
@@ -144,24 +144,25 @@
 
     def new_timestep(self, payload: SimTimestep) -> None:
         # LOGGER.info("----------------------------------------------------")
         # LOGGER.info(f"[{self.time_str()}: {self.short_alias}] NEW TIMESTEP")
         # LOGGER.info("----------------------------------------------------")
 
         # This gets called on the first timestep
-        if atn_utils.is_dummy_atn_params(self.atn_params):
+        if strategy_utils.is_dummy_atn_params(self.atn_params):
             self.get_initial_params()
             LOGGER.info("Correcting runs on initial timestep")
-            self.active_run = atn_utils.dummy_slot_stuff(
+            self.active_run = strategy_utils.dummy_slot_stuff(
                 slot=self.last_slot(self.market_type),
             )
             try:
                 self.next_run = dev_io.initialize_slot_stuff(
                     slot=self.active_slot(self.market_type),
                     atn_params=self.atn_params,
+                    atn_gni_id=self.g_node_instance_id,
                 )
             except Exception as e:
                 LOGGER.warning(
                     f"Failed to initialize FloParams! Not creating a next_run {e}"
                 )
                 return
 
@@ -178,14 +179,15 @@
             try:
                 self.get_bid()
             except Exception:
                 LOGGER.exception("Error in get_bid")
             self.next_run = dev_io.initialize_slot_stuff(
                 slot=self.next_slot(self.market_type),
                 atn_params=self.atn_params,
+                atn_gni_id=self.g_node_instance_id,
             )
             try:
                 self.submit_bid(self.active_run)
             except Exception:
                 LOGGER.exception("Error in submit_bid")
         if self.active_run.Price is not None:
             self.respond_to_price()
@@ -234,19 +236,23 @@
         try:
             self.update_power_levels()
         except Exception:
             LOGGER.exception("Error in update_power_levels")
         payload = Snapshot_Maker(
             from_g_node_alias=self.alias,
             from_g_node_instance_id=self.g_node_instance_id,
-            boost_power_kw_times1000=int(self.boost_kw * 1000),
-            heatpump_power_kw_times1000=int(self.heatpump_kw * 1000),
-            cop_times10=int(self.cop * 10),
+            power_watts=self._power_watts,
             store_kwh=int(self.store_kwh),
-            max_store_kwh=int(atn_utils.get_max_store_kwh_th(self.atn_params)),
+            max_store_kwh=int(
+                strategy_utils.get_max_store_kwh_th(
+                    max_brick_temp_c=self.atn_params.MaxBrickTempC,
+                    c=self.atn_params.C,
+                    room_temp_f=self.atn_params.RoomTempF,
+                )
+            ),
             about_terminal_asset_alias=self.alias + ".ta",
         ).tuple
         # pprint(payload)
         self.send_message(
             payload=payload, message_category=MessageCategory.RabbitJsonBroadcast
         )
 
@@ -272,23 +278,22 @@
         node = self.active_run.Flo.node[0][self.active_run.Flo.starting_store_idx]
         edge: Edge = list(
             filter(
                 lambda x: x.end_idx == node.best_next_idx,
                 self.active_run.Flo.edges[node],
             )
         )[0]
-        self.heatpump_kw = edge.hp_electricity_avg_kw
-        self.boost_kw = edge.boost_electricity_used_avg_kw
-        self.cop = self.active_run.Flo.cop[0]
+        self._power_watts = edge.avg_kw * 1000
+
         # LOGGER.info(
         #     f"[{self.time_str()}: {self.short_alias}] Updating state: heatpump {round(self.heatpump_kw,2)}"
         # )
 
     def update_store_level(self) -> None:
-        if atn_utils.is_dummy_slot_stuff(self.active_run):
+        if strategy_utils.is_dummy_slot_stuff(self.active_run):
             LOGGER.info(f"Not updating storage - active run is a dummy")
             self.store_update_time = self.time()
             return
         duration_minutes = int((self.time() - self.store_update_time) / 60)
         if duration_minutes != self.market_type.DurationMinutes:
             raise Exception(
                 f"In update_store_level: Expected {self.market_type.DurationMinutes} minutes, got {duration_minutes} minutes."
@@ -306,15 +311,19 @@
         try:
             store_idx = flo.node[0][flo.starting_store_idx].best_next_idx
         except:
             raise Exception(f"Flo node did not have best_node_idx!")
         # self.store_kwh = ...
         self.store_kwh = (
             store_idx
-            * atn_utils.get_max_store_kwh_th(self.atn_params)
+            * strategy_utils.get_max_store_kwh_th(
+                max_brick_temp_c=self.atn_params.MaxBrickTempC,
+                c=self.atn_params.C,
+                room_temp_f=self.atn_params.RoomTempF,
+            )
             / self.atn_params.StorageSteps
         )
         # LOGGER.info(
         #     f"[{self.time_str()}: {self.short_alias}] Storage level {round(self.store_kwh,2)} kWh, "
         #     f"StoreIdx {self.active_run.BidParams.StartingStoreIdx}"
         # )
         self.store_update_time = self.time()
@@ -335,15 +344,15 @@
         node = self.active_run.Flo.node[0][self.active_run.Flo.starting_store_idx]
         edge: Edge = list(
             filter(
                 lambda x: x.end_idx == node.best_next_idx,
                 self.active_run.Flo.edges[node],
             )
         )[0]
-        q = edge.hp_electricity_avg_kw + edge.boost_electricity_used_avg_kw
+        q = edge.avg_kw
         pq = PriceQuantityUnitless(
             PriceTimes1000=int(
                 self.active_run.Flo.params.RealtimeElectricityPrice[0] * 1000
             ),
             QuantityTimes1000=int(q * 1000),
         )
         bid_list = [pq]
@@ -409,28 +418,29 @@
             return rr
 
     ########################
     # Initialization
     ########################
 
     def dev_get_initial_params(self) -> None:
-        if not atn_utils.is_dummy_atn_params(self.atn_params):
+        if not strategy_utils.is_dummy_atn_params(self.atn_params):
             LOGGER.warning("Tried to get initial params but already have them")
 
         now_ms = int(self.time()) * 1000
         self.atn_params = dev_io.atn_params_from_alias(alias=self.alias, now_ms=now_ms)
         self.atn_params.GNodeInstanceId = self.g_node_instance_id
-        if atn_utils.is_dummy_atn_params(self.atn_params):
+        if strategy_utils.is_dummy_atn_params(self.atn_params):
             LOGGER.warning(f"No atn_params for {self.alias} before {self.time_str()}")
             return
         payload = AtnParamsReport_Maker(
             g_node_alias=self.alias,
             g_node_instance_id=self.g_node_instance_id,
+            atn_params_type_name=self.atn_params.TypeName,
             time_unix_s=int(self.time()),
-            atn_params=self.atn_params,
+            params=self.atn_params,
             irl_time_unix_s=int(time.time()),
         ).tuple
 
         self.send_message(
             payload=payload, message_category=MessageCategory.RabbitJsonBroadcast
         )
         # LOGGER.info(f"[{self.time_str()}: {self.short_alias}] Initial params loaded")
@@ -486,9 +496,13 @@
     # TerminalAsset properties
     #################
 
     def store_idx(self) -> int:
         return round(
             self.atn_params.StorageSteps
             * self.store_kwh
-            / atn_utils.get_max_store_kwh_th(self.atn_params)
+            / strategy_utils.get_max_store_kwh_th(
+                max_brick_temp_c=self.atn_params.MaxBrickTempC,
+                c=self.atn_params.C,
+                room_temp_f=self.atn_params.RoomTempF,
+            )
         )
```

### Comparing `gridworks_atn-0.3.4/src/gwatn/brick_storage_heater/edge.py` & `gridworks_atn-0.3.5/src/gwatn/brick_storage_heater/edge.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/brick_storage_heater/flo.py` & `gridworks_atn-0.3.5/src/gwatn/brick_storage_heater/flo.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/brick_storage_heater/flo_output.py` & `gridworks_atn-0.3.5/src/gwatn/brick_storage_heater/flo_output.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 import time
 
 import gridworks.conversion_factors as cf
 import pendulum
 import xlsxwriter
-from satn.strategies.heatpumpwithbooststore.flo import HeatPumpWithBoostStore__Flo
-from satn.strategies.heatpumpwithbooststore.node import (
-    Node_SpaceHeat__WaterStore as Node,
-)
 
 import gwatn.brick_storage_heater.strategy_utils as strategy_utils
 from gwatn.brick_storage_heater.edge import Edge__BrickStorageHeater as Edge
+from gwatn.brick_storage_heater.flo import Flo__BrickStorageHeater as Flo
+from gwatn.brick_storage_heater.node import Node_BrickStorageHeater as Node
 from gwatn.enums import RecognizedCurrencyUnit
 from gwatn.types import AtnParamsBrickstorageheater as AtnParams
 
 
 OUTPUT_FOLDER = "output_data"
 
 ON_PEAK_DIST_PRICE_PER_MWH_CUTOFF = 100
 SHOULDER_PEAK_DIST_PRICE_PER_MWH_CUTOFF = 50
 
 
-def export_xlsx(alias: str, flo: HeatPumpWithBoostStore__Flo, atn_params: AtnParams):
+def export_xlsx(alias: str, flo: Flo, atn_params: AtnParams):
     local_start = pendulum.timezone(flo.timezone_string).convert(flo.flo_start_utc)
     date_str = local_start.strftime("%Y%m%d")
     hour_str = local_start.strftime("%H")
     file = (
         OUTPUT_FOLDER + f"/result_{alias}_{date_str}_{hour_str}_{int(time.time())}.xlsx"
     )
     # flo.graph_strategy_alias,
@@ -51,15 +49,15 @@
 
     export_params_xlsx(flo=flo, atn_params=atn_params, workbook=workbook)
     workbook.close()
 
 
 def export_best_path_info(
     alias: str,
-    flo: HeatPumpWithBoostStore__Flo,
+    flo: Flo,
     workbook: xlsxwriter.workbook.Workbook,
     starting_store_idx: int,
 ):
     w = workbook.add_worksheet(
         f"start {100 * starting_store_idx / flo.params.StorageSteps}%"
     )
     w.freeze_panes(0, 2)
@@ -292,15 +290,15 @@
     w.write("K2", total_cost / gallons_oil, currency_bold_format)
     # w.write("H3", "Flat rate comparison")
 
     return w
 
 
 def export_flo_graph(
-    flo: HeatPumpWithBoostStore__Flo,
+    flo: Flo,
     workbook: xlsxwriter.workbook.Workbook,
     worksheet: xlsxwriter.workbook.Worksheet,
     starting_store_idx: int,
     graph_start_row: int,
 ):
     # worksheet.freeze_panes(graph_start_row - 1, 2)
     header_format = workbook.add_format({"bold": True, "text_wrap": True})
@@ -336,15 +334,15 @@
                     )
                 except:
                     print(f"failed for {jj},{kk}")
         best_idx = flo.best_edge[best_node].end_idx
 
 
 def export_params_xlsx(
-    flo: HeatPumpWithBoostStore__Flo,
+    flo: Flo,
     atn_params: AtnParams,
     workbook: xlsxwriter.workbook.Workbook,
 ):
     bold = workbook.add_format({"bold": True})
     w = workbook.add_worksheet("Params")
     derived_format_bold = workbook.add_format({"bold": True, "font_color": "green"})
     derived_format = workbook.add_format({"font_color": "green"})
```

### Comparing `gridworks_atn-0.3.4/src/gwatn/brick_storage_heater/make_dev_input_data.py` & `gridworks_atn-0.3.5/src/gwatn/brick_storage_heater/make_dev_input_data.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/brick_storage_heater/node.py` & `gridworks_atn-0.3.5/src/gwatn/brick_storage_heater/node.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/brick_storage_heater/simple_scada_sim.py` & `gridworks_atn-0.3.5/src/gwatn/brick_storage_heater/simple_scada_sim.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/brick_storage_heater/strategy_utils.py` & `gridworks_atn-0.3.5/src/gwatn/brick_storage_heater/strategy_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import List
 from typing import Optional
 
 from pydantic import BaseModel
 
 from gwatn.brick_storage_heater.flo import Flo__BrickStorageHeater as Flo
 from gwatn.types import AtnBid
 from gwatn.types import AtnParamsBrickstorageheater as AtnParams
@@ -61,22 +62,28 @@
 def dummy_flo_params() -> FloParams:
     return FloParams(
         RtElecPriceUid="00000000-0000-0000-0000-000000000000",
         WeatherUid="00000000-0000-0000-0000-000000000000",
     )
 
 
-def get_max_store_kwh_th(params: FloParams) -> float:
+def get_max_store_kwh_th(max_brick_temp_c: int, c: float, room_temp_f: int) -> float:
     """Use max store temp, room temp, and CF to get max store energy in kWh_th"""
-    room_temp_c = (params.RoomTempF - 32) * 5 / 9
-    return (params.MaxBrickTempC - room_temp_c) * params.C
+    room_temp_c = (room_temp_f - 32) * 5 / 9
+    return (max_brick_temp_c - room_temp_c) * c
 
 
-def get_house_worst_case_heat_output_avg_kw(params: FloParams) -> float:
-    design_t = params.HouseWorstCaseTempF
-    this_run_t = min(params.OutsideTempF)
-    room_t = params.RoomTempF
-    p = params.PowerRequiredByHouseFromSystemAvgKwList
+def get_house_worst_case_heat_output_avg_kw(
+    house_worst_case_temp_f: int,
+    room_temp_f: int,
+    ambient_power_in_kw: float,
+    outside_temp_f_list: List[int],
+    power_required_by_house_from_system_avg_kw_list: List[float],
+) -> float:
+    design_t = house_worst_case_temp_f
+    this_run_t = min(outside_temp_f_list)
+    room_t = room_temp_f
+    p = power_required_by_house_from_system_avg_kw_list
     this_run_max_system_kw = max(p)
-    this_run_max_kw_in = this_run_max_system_kw + params.AmbientPowerInKw
+    this_run_max_kw_in = this_run_max_system_kw + ambient_power_in_kw
     dd_max_kw_in = this_run_max_kw_in * (room_t - design_t) / (room_t - this_run_t)
-    return dd_max_kw_in - params.AmbientPowerInKw
+    return dd_max_kw_in - ambient_power_in_kw
```

### Comparing `gridworks_atn-0.3.4/src/gwatn/config.py` & `gridworks_atn-0.3.5/src/gwatn/config.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/data_classes/.DS_Store` & `gridworks_atn-0.3.5/src/gwatn/data_classes/.DS_Store`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/data_classes/__init__.py` & `gridworks_atn-0.3.5/src/gwatn/data_classes/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,20 +4,26 @@
 from gridworks.data_classes.g_node_instance import GNodeInstance
 from gridworks.data_classes.gps_point import GpsPoint
 from gridworks.data_classes.market_type import MarketType
 from gridworks.data_classes.supervisor_container import SupervisorContainer
 
 from gwatn.data_classes.d_edge import DEdge
 from gwatn.data_classes.d_node import DNode
+from gwatn.data_classes.hack_price_method import PriceMethod
+from gwatn.data_classes.hack_weather_location import WeatherLocation
+from gwatn.data_classes.hack_weather_source import WeatherSource
 
 
 __all__ = [
     "market_type",
     "BaseGNode",
     "DEdge",
     "DNode",
     "GNode",
     "GNodeInstance",
     "GpsPoint",
     "MarketType",
+    "PriceMethod",
     "SupervisorContainer",
+    "WeatherLocation",
+    "WeatherSource",
 ]
```

### Comparing `gridworks_atn-0.3.4/src/gwatn/data_classes/d_edge.py` & `gridworks_atn-0.3.5/src/gwatn/data_classes/d_edge.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/data_classes/d_graph.py` & `gridworks_atn-0.3.5/src/gwatn/data_classes/d_graph.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/data_classes/d_node.py` & `gridworks_atn-0.3.5/src/gwatn/data_classes/d_node.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/demo_methods.py` & `gridworks_atn-0.3.5/src/gwatn/demo_methods.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/dev_utils/dev_discoverer.py` & `gridworks_atn-0.3.5/src/gwatn/dev_utils/dev_discoverer.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/dev_utils/dev_ta_owner.py` & `gridworks_atn-0.3.5/src/gwatn/dev_utils/dev_ta_owner.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/dev_utils/dev_validator.py` & `gridworks_atn-0.3.5/src/gwatn/dev_utils/dev_validator.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/dev_utils/make_plants.py` & `gridworks_atn-0.3.5/src/gwatn/dev_utils/make_plants.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/dispatch_contract.py` & `gridworks_atn-0.3.5/src/gwatn/dispatch_contract.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/dispatch_contract_artifacts/application.json` & `gridworks_atn-0.3.5/src/gwatn/dispatch_contract_artifacts/application.json`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/dispatch_contract_artifacts/approval.teal` & `gridworks_atn-0.3.5/src/gwatn/dispatch_contract_artifacts/approval.teal`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/dispatch_contract_artifacts/contract.json` & `gridworks_atn-0.3.5/src/gwatn/dispatch_contract_artifacts/contract.json`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/enums/__init__.py` & `gridworks_atn-0.3.5/src/gwatn/enums/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -23,14 +23,18 @@
 from gwproto.enums.role import Role
 from gwproto.enums.telemetry_name import TelemetryName
 from gwproto.enums.unit import Unit
 
 # From gwatn
 from gwatn.enums.distribution_tariff import DistributionTariff
 from gwatn.enums.energy_supply_type import EnergySupplyType
+from gwatn.enums.hack_price_method import PriceMethod
+from gwatn.enums.hack_recognized_p_node_alias import RecognizedPNodeAlias
+from gwatn.enums.hack_weather_method import WeatherMethod
+from gwatn.enums.hack_weather_source import WeatherSource
 from gwatn.enums.recognized_irradiance_type import RecognizedIrradianceType
 from gwatn.enums.recognized_temperature_unit import RecognizedTemperatureUnit
 
 
 __all__ = [
     "ActorClass",
     "AlgoCertType",
@@ -43,17 +47,21 @@
     "LocalCommInterface",
     "MakeModel",
     "MarketPriceUnit",
     "MarketQuantityUnit",
     "MarketTypeName",
     "MessageCategory",
     "MessageCategorySymbol",
+    "PriceMethod",
     "RecognizedCurrencyUnit",
     "RecognizedIrradianceType",
+    "RecognizedPNodeAlias",
     "RecognizedTemperatureUnit",
     "Role",
     "StrategyName",
     "SupervisorContainerStatus",
     "TelemetryName",
     "Unit",
     "UniverseType",
+    "WeatherMethod",
+    "WeatherSource",
 ]
```

### Comparing `gridworks_atn-0.3.4/src/gwatn/enums/distribution_tariff.py` & `gridworks_atn-0.3.5/src/gwatn/enums/distribution_tariff.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/enums/energy_supply_type.py` & `gridworks_atn-0.3.5/src/gwatn/enums/energy_supply_type.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/enums/recognized_irradiance_type.py` & `gridworks_atn-0.3.5/src/gwatn/enums/recognized_irradiance_type.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/enums/recognized_temperature_unit.py` & `gridworks_atn-0.3.5/src/gwatn/enums/recognized_temperature_unit.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/python_ta_daemon.json` & `gridworks_atn-0.3.5/src/gwatn/python_ta_daemon.json`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/python_ta_daemon.py` & `gridworks_atn-0.3.5/src/gwatn/python_ta_daemon.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/scada_codec.py` & `gridworks_atn-0.3.5/src/gwatn/scada_codec.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/simple_atn_actor.py` & `gridworks_atn-0.3.5/src/gwatn/simple_atn_actor.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/simple_scada_sim_actor_base.py` & `gridworks_atn-0.3.5/src/gwatn/simple_scada_sim_actor_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/ta_daemon_rest_api.py` & `gridworks_atn-0.3.5/src/gwatn/ta_daemon_rest_api.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/two_channel_actor_base.py` & `gridworks_atn-0.3.5/src/gwatn/two_channel_actor_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/types/__init__.py` & `gridworks_atn-0.3.5/src/gwatn/types/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/types/accepted_bid.py` & `gridworks_atn-0.3.5/src/gwatn/types/accepted_bid.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/types/atn_bid.py` & `gridworks_atn-0.3.5/src/gwatn/types/atn_bid.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/types/atn_params.py` & `gridworks_atn-0.3.5/src/gwatn/types/atn_params.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/types/atn_params_brickstorageheater.py` & `gridworks_atn-0.3.5/src/gwatn/types/atn_params_brickstorageheater.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/types/atn_params_report.py` & `gridworks_atn-0.3.5/src/gwatn/types/atn_params_report.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/types/basegnode_scada_create.py` & `gridworks_atn-0.3.5/src/gwatn/types/basegnode_scada_create.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/types/csv_distp_sync.py` & `gridworks_atn-0.3.5/src/gwatn/types/csv_distp_sync.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/types/csv_eprt_sync.py` & `gridworks_atn-0.3.5/src/gwatn/types/csv_eprt_sync.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/types/csv_weather_forecast_sync.py` & `gridworks_atn-0.3.5/src/gwatn/types/csv_weather_forecast_sync.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/types/data_channel.py` & `gridworks_atn-0.3.5/src/gwatn/types/data_channel.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/types/discoverycert_algo_create.py` & `gridworks_atn-0.3.5/src/gwatn/types/discoverycert_algo_create.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/types/dispatch_contract_confirmed.py` & `gridworks_atn-0.3.5/src/gwatn/types/dispatch_contract_confirmed.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/types/flo_params.py` & `gridworks_atn-0.3.5/src/gwatn/types/flo_params.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/types/flo_params_brickstorageheater.py` & `gridworks_atn-0.3.5/src/gwatn/types/flo_params_brickstorageheater.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/types/flo_params_report.py` & `gridworks_atn-0.3.5/src/gwatn/types/flo_params_report.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/types/gt_dispatch_boolean.py` & `gridworks_atn-0.3.5/src/gwatn/types/gt_dispatch_boolean.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/types/heartbeat_b.py` & `gridworks_atn-0.3.5/src/gwatn/types/heartbeat_b.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/types/initial_tadeed_algo_create.py` & `gridworks_atn-0.3.5/src/gwatn/types/initial_tadeed_algo_create.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/types/initial_tadeed_algo_optin.py` & `gridworks_atn-0.3.5/src/gwatn/types/initial_tadeed_algo_optin.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/types/initial_tadeed_algo_transfer.py` & `gridworks_atn-0.3.5/src/gwatn/types/initial_tadeed_algo_transfer.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/types/join_dispatch_contract.py` & `gridworks_atn-0.3.5/src/gwatn/types/join_dispatch_contract.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/types/latest_price.py` & `gridworks_atn-0.3.5/src/gwatn/types/latest_price.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/types/market_slot.py` & `gridworks_atn-0.3.5/src/gwatn/types/market_slot.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/types/market_type_gt.py` & `gridworks_atn-0.3.5/src/gwatn/types/market_type_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/types/new_tadeed_algo_optin.py` & `gridworks_atn-0.3.5/src/gwatn/types/new_tadeed_algo_optin.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/types/new_tadeed_send.py` & `gridworks_atn-0.3.5/src/gwatn/types/new_tadeed_send.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/types/old_tadeed_algo_return.py` & `gridworks_atn-0.3.5/src/gwatn/types/old_tadeed_algo_return.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/types/price_quantity.py` & `gridworks_atn-0.3.5/src/gwatn/types/price_quantity.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/types/price_quantity_unitless.py` & `gridworks_atn-0.3.5/src/gwatn/types/price_quantity_unitless.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/types/scada_cert_transfer.py` & `gridworks_atn-0.3.5/src/gwatn/types/scada_cert_transfer.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/types/simplesim_driver_data.py` & `gridworks_atn-0.3.5/src/gwatn/types/simplesim_driver_data.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/types/simplesim_driver_data_bsh.py` & `gridworks_atn-0.3.5/src/gwatn/types/simplesim_driver_data_bsh.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/types/simplesim_driver_report.py` & `gridworks_atn-0.3.5/src/gwatn/types/simplesim_driver_report.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/types/simplesim_snapshot_brickstorageheater.py` & `gridworks_atn-0.3.5/src/gwatn/types/simplesim_snapshot_brickstorageheater.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/types/sla_enter.py` & `gridworks_atn-0.3.5/src/gwatn/types/sla_enter.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/types/tadeed_specs_hack.py` & `gridworks_atn-0.3.5/src/gwatn/types/tadeed_specs_hack.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/types/tavalidatorcert_algo_create.py` & `gridworks_atn-0.3.5/src/gwatn/types/tavalidatorcert_algo_create.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/types/tavalidatorcert_algo_transfer.py` & `gridworks_atn-0.3.5/src/gwatn/types/tavalidatorcert_algo_transfer.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/src/gwatn/types/terminalasset_certify_hack.py` & `gridworks_atn-0.3.5/src/gwatn/types/terminalasset_certify_hack.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.4/PKG-INFO` & `gridworks_atn-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridworks-atn
-Version: 0.3.4
+Version: 0.3.5
 Summary: Gridworks Atn Spaceheat
 Home-page: https://github.com/thegridelectric/gridworks-atn
 License: None
 Author: Jessica Millar
 Author-email: jmillar@gridworks-consulting.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

