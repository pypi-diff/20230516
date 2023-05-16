# Comparing `tmp/zhmcclient-1.7.3.tar.gz` & `tmp/zhmcclient-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhmcclient-1.7.3.tar", last modified: Wed May 10 12:18:17 2023, max compression
+gzip compressed data, was "zhmcclient-1.8.0.tar", last modified: Tue May 16 07:25:52 2023, max compression
```

## Comparing `zhmcclient-1.7.3.tar` & `zhmcclient-1.8.0.tar`

### file list

```diff
@@ -1,70 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:18:17.681876 zhmcclient-1.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-10 12:18:12.000000 zhmcclient-1.7.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-05-10 12:18:17.681876 zhmcclient-1.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/extra-testutils-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 12:18:17.681876 zhmcclient-1.7.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     5408 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:18:17.677876 zhmcclient-1.7.3/zhmcclient/
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient/_activation_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    24998 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient/_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient/_capacity_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient/_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    30840 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient/_console.py
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    92008 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient/_cpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient/_debug_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    46440 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient/_hba.py
--rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient/_ldap_server_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient/_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    76387 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient/_lpar.py
--rw-r--r--   0 runner    (1001) docker     (123)    32451 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient/_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    36561 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient/_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    11907 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient/_nic.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15902 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient/_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)    49996 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient/_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient/_password_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     9171 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient/_port.py
--rw-r--r--   0 runner    (1001) docker     (123)    21760 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient/_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    11445 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient/_resource_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)    65630 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient/_session.py
--rw-r--r--   0 runner    (1001) docker     (123)    33564 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient/_storage_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    12919 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient/_storage_group_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    25230 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient/_storage_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    13631 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient/_storage_volume_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient/_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    10289 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient/_timestats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient/_unmanaged_cpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11520 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient/_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    11108 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient/_user_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)    16070 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient/_user_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    17515 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient/_virtual_function.py
--rw-r--r--   0 runner    (1001) docker     (123)    12325 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient/_virtual_storage_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient/_virtual_switch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:18:17.681876 zhmcclient-1.7.3/zhmcclient/testutils/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient/testutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient/testutils/_cpc_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient/testutils/_hmc_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient/testutils/_hmc_definition_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)    18720 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient/testutils/_hmc_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11162 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient/testutils/_hmc_inventory_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7628 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient/testutils/_hmc_vault_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:18:17.677876 zhmcclient-1.7.3/zhmcclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-05-10 12:18:17.000000 zhmcclient-1.7.3/zhmcclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-10 12:18:17.000000 zhmcclient-1.7.3/zhmcclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:18:17.000000 zhmcclient-1.7.3/zhmcclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-10 12:18:17.000000 zhmcclient-1.7.3/zhmcclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 12:18:17.000000 zhmcclient-1.7.3/zhmcclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:17:19.000000 zhmcclient-1.7.3/zhmcclient.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:18:17.681876 zhmcclient-1.7.3/zhmcclient_mock/
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient_mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   130816 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient_mock/_hmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient_mock/_idpool.py
--rw-r--r--   0 runner    (1001) docker     (123)    41808 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient_mock/_session.py
--rw-r--r--   0 runner    (1001) docker     (123)   196269 2023-05-10 12:17:05.000000 zhmcclient-1.7.3/zhmcclient_mock/_urihandler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:52.224789 zhmcclient-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-16 07:25:48.000000 zhmcclient-1.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-05-16 07:25:52.224789 zhmcclient-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/extra-testutils-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 07:25:52.224789 zhmcclient-1.8.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5458 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:52.220788 zhmcclient-1.8.0/zhmcclient/
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12561 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_activation_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27187 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_capacity_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12571 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32528 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94301 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_cpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_debug_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46440 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_hba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_ldap_server_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78470 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_lpar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33251 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36561 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11907 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_nic.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15902 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52098 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9863 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_password_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9171 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_port.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25139 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11445 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_resource_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65630 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33564 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_storage_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12919 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_storage_group_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25230 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_storage_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13631 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_storage_volume_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10289 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_timestats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_unmanaged_cpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_user_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16071 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_user_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18362 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_virtual_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12325 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_virtual_storage_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_virtual_switch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:52.220788 zhmcclient-1.8.0/zhmcclient/testutils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/testutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/testutils/_cpc_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/testutils/_hmc_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/testutils/_hmc_definition_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19125 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/testutils/_hmc_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11276 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/testutils/_hmc_inventory_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/testutils/_hmc_vault_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:52.220788 zhmcclient-1.8.0/zhmcclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-05-16 07:25:52.000000 zhmcclient-1.8.0/zhmcclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-16 07:25:52.000000 zhmcclient-1.8.0/zhmcclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 07:25:52.000000 zhmcclient-1.8.0/zhmcclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-16 07:25:52.000000 zhmcclient-1.8.0/zhmcclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-16 07:25:52.000000 zhmcclient-1.8.0/zhmcclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 07:25:12.000000 zhmcclient-1.8.0/zhmcclient.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:52.224789 zhmcclient-1.8.0/zhmcclient_mock/
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient_mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   134108 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient_mock/_hmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient_mock/_idpool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41808 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient_mock/_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)   201548 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient_mock/_urihandler.py
```

### Comparing `zhmcclient-1.7.3/LICENSE` & `zhmcclient-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.7.3/MANIFEST.in` & `zhmcclient-1.8.0/MANIFEST.in`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 include README.rst
 include requirements.txt
 include extra-testutils-requirements.txt
 include zhmcclient/__init__.py
 include zhmcclient/_activation_profile.py
 include zhmcclient/_adapter.py
 include zhmcclient/_capacity_group.py
+include zhmcclient/_certificates.py
 include zhmcclient/_client.py
 include zhmcclient/_console.py
 include zhmcclient/_constants.py
 include zhmcclient/_cpc.py
 include zhmcclient/_debug_info.py
 include zhmcclient/_exceptions.py
+include zhmcclient/_group.py
 include zhmcclient/_hba.py
 include zhmcclient/_ldap_server_definition.py
 include zhmcclient/_logging.py
 include zhmcclient/_lpar.py
 include zhmcclient/_manager.py
 include zhmcclient/_metrics.py
 include zhmcclient/_nic.py
```

### Comparing `zhmcclient-1.7.3/PKG-INFO` & `zhmcclient-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhmcclient
-Version: 1.7.3
+Version: 1.8.0
 Summary: A pure Python client library for the IBM Z HMC Web Services API.
 Home-page: https://github.com/zhmcclient/python-zhmcclient
 Author: Juergen Leopold, Andreas Maier
 Author-email: leopoldj@de.ibm.com, maiera@de.ibm.com
 Maintainer: Andreas Maier, Kathir Velusamy
 Maintainer-email: maiera@de.ibm.com, kathir.velu@in.ibm.com
 License: Apache License, Version 2.0
@@ -23,14 +23,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*
 Description-Content-Type: text/x-rst
 Provides-Extra: testutils
 License-File: LICENSE
 
 .. Copyright 2016-2021 IBM Corp. All Rights Reserved.
```

### Comparing `zhmcclient-1.7.3/README.rst` & `zhmcclient-1.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.7.3/extra-testutils-requirements.txt` & `zhmcclient-1.8.0/extra-testutils-requirements.txt`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.7.3/requirements.txt` & `zhmcclient-1.8.0/requirements.txt`

 * *Files 22% similar despite different names*

```diff
@@ -48,21 +48,26 @@
 # yamlloader pulled in by zhmcclient_mock and zhmcclient.testutils
 # yamlloader 1.0 removed support for py27,35
 yamlloader>=0.5.5
 
 # jsonschema pulled in by zhmcclient_mock and zhmcclient.testutils
 # jsonschema 4.0 removed support for py27,35,36
 # jsonschema 4.0.0 was yanked (and does not install), but older pip versions don't recognize that
-jsonschema>=2.6.0,!=4.0.0
+# jsonschema is also used by jupyter and requires >=3.0.1
+jsonschema>=3.0.1,!=4.0.0
 
 # Indirect dependencies (commented out, only listed to document their license):
 
 # Since we changed to use the allowed_methods attribute introduced in urllib3
 # 1.26.0, and our minimum version of requests (2.25.0) only requires
 # urllib3>=1.21.0, we need to require a minimum version of urllib3.
 urllib3>=1.26.5  # MIT
 
+# MIT, from jsonschema>=3.0
+# pyrsistent 0.15.0 started using the FileNotFoundError built-in exception that
+# was added only in Python 3. pyrsistent 0.15.1 fixed that by defining it locally for py27.
+pyrsistent>=0.15.1
+
 # certifi # ISC, from requests>=2.20
 # chardet # LGPL, from requests>=2.20
 # docopt # MIT, from stomp.py>=4.1
 # idna # BSD-like, from requests>=2.20
-# pyrsistent # MIT, from jsonschema>=3.0
```

### Comparing `zhmcclient-1.7.3/setup.py` & `zhmcclient-1.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,10 +138,11 @@
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ]
 )
```

### Comparing `zhmcclient-1.7.3/zhmcclient/__init__.py` & `zhmcclient-1.8.0/zhmcclient/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from ._resource import *      # noqa: F401
 from ._logging import *       # noqa: F401
 from ._session import *       # noqa: F401
 from ._resource_updater import *       # noqa: F401
 from ._timestats import *     # noqa: F401
 from ._client import *        # noqa: F401
 from ._cpc import *           # noqa: F401
+from ._group import *         # noqa: F401
 from ._lpar import *          # noqa: F401
 from ._partition import *     # noqa: F401
 from ._activation_profile import *     # noqa: F401
 from ._adapter import *       # noqa: F401
 from ._nic import *           # noqa: F401
 from ._hba import *           # noqa: F401
 from ._virtual_function import *       # noqa: F401
@@ -54,8 +55,9 @@
 from ._unmanaged_cpc import *          # noqa: F401
 from ._storage_group import *          # noqa: F401
 from ._storage_volume import *         # noqa: F401
 from ._virtual_storage_resource import *        # noqa: F401
 from ._storage_group_template import *          # noqa: F401
 from ._storage_volume_template import *         # noqa: F401
 from ._capacity_group import *         # noqa: F401
+from ._certificates import *         # noqa: F401
 from ._debug_info import *         # noqa: F401
```

### Comparing `zhmcclient-1.7.3/zhmcclient/_activation_profile.py` & `zhmcclient-1.8.0/zhmcclient/_activation_profile.py`

 * *Files 15% similar despite different names*

```diff
@@ -119,15 +119,16 @@
             class_name=activation_profile_class,
             session=cpc.manager.session,
             parent=cpc,
             base_uri='{}/{}-activation-profiles'.format(cpc.uri, profile_type),
             oid_prop='name',  # This is an exception!
             uri_prop='element-uri',
             name_prop='name',
-            query_props=query_props)
+            query_props=query_props,
+            supports_properties=True)
 
         self._profile_type = profile_type
 
     @property
     def cpc(self):
         """
         :class:`~zhmcclient.Cpc`: :term:`CPC` defining the scope for this
@@ -274,7 +275,71 @@
         """
         # pylint: disable=protected-access
         self.manager.session.post(self.uri, body=properties)
         # Attempts to change the 'name' property will be rejected by the HMC,
         # so we don't need to update the name-to-URI cache.
         assert self.manager._name_prop not in properties
         self.update_properties_local(copy.deepcopy(properties))
+
+    @logged_api_call
+    def assign_certificate(self, certificate):
+        """
+        Assigns a :term:`Certificate` to this Image Activation Profile.
+
+        :ref:`Feature enablement` requirements:
+
+        *  "secure-boot-with-certificates" must be available on HMC and CPC
+
+        Authorization requirements:
+
+        * Object-access permission to this Activation Profile.
+        * Object-access permission to the specified certificate.
+        * Task permission to the "Assign Secure Boot Certificates" task.
+
+        Parameters:
+
+          certificate (:class:`~zhmcclient.Certificate`):
+            Certificate to be assigned. The certificate must not currently
+            be assigned to this LPAR.
+
+        Raises:
+
+          :exc:`~zhmcclient.HTTPError`
+          :exc:`~zhmcclient.ParseError`
+          :exc:`~zhmcclient.AuthError`
+          :exc:`~zhmcclient.ConnectionError`
+        """
+        body = {'certificate-uri': certificate.uri}
+        self.manager.session.post(
+            self.uri + '/operations/assign-certificate', body)
+
+    @logged_api_call
+    def unassign_certificate(self, certificate):
+        """
+        Unassign a :term:`Certificate` from this Image Activation Profile.
+
+        :ref:`Feature enablement` requirements:
+
+        *  "secure-boot-with-certificates" must be available on HMC and CPC
+
+        Authorization requirements:
+
+        * Object-access permission to this Image Activation Profile.
+        * Object-access permission to the specified certificate.
+        * Task permission to the "Assign Secure Boot Certificates" task.
+
+        Parameters:
+
+          certificate (:class:`~zhmcclient.Certificate`):
+            Certificate to be unassigned. The certificate must currently be
+            assigned to this LPAR.
+
+        Raises:
+
+          :exc:`~zhmcclient.HTTPError`
+          :exc:`~zhmcclient.ParseError`
+          :exc:`~zhmcclient.AuthError`
+          :exc:`~zhmcclient.ConnectionError`
+        """
+        body = {'certificate-uri': certificate.uri}
+        self.manager.session.post(
+            self.uri + '/operations/unassign-certificate', body)
```

### Comparing `zhmcclient-1.7.3/zhmcclient/_adapter.py` & `zhmcclient-1.8.0/zhmcclient/_adapter.py`

 * *Files 4% similar despite different names*

```diff
@@ -675,7 +675,63 @@
 
             if matches_filters(resource_obj, client_filters):
                 resource_obj_list.append(resource_obj)
                 if full_properties:
                     resource_obj.pull_full_properties()
 
         return resource_obj_list
+
+    @logged_api_call
+    def list_sibling_adapters(self, full_properties=False):
+        """
+        List the other Adapters on the same adapter card as this Adapter.
+
+        Some adapter cards are represented as multiple Adapter objects
+        (for example, 2-port FICON Express cards, or 2-port CNA cards).
+        This method lists the other Adapter objects that are on the same
+        adapter card as this Adapter object.
+
+        This is useful for example to determine the affected Adapter objects
+        when replacing the adapter card, or when changing the type of a FICON
+        Express adepter (see :meth:`~zhmcclient.Adapter.change_adapter_type`).
+
+        Authorization requirements:
+
+        * Object-access permission to this CPC.
+        * Object-access permission to any Adapter to be included in the result.
+
+        Parameters:
+
+          full_properties (bool):
+            Controls whether the full set of resource properties should be
+            retrieved, vs. only the short set as returned by the list
+            operation.
+
+        Returns:
+
+          : A list of :class:`~zhmcclient.Adapter` objects.
+
+        Raises:
+
+          :exc:`~zhmcclient.HTTPError`
+          :exc:`~zhmcclient.ParseError`
+          :exc:`~zhmcclient.AuthError`
+          :exc:`~zhmcclient.ConnectionError`
+        """
+        # This algorithm is based on the fact that physical adapter cards
+        # have their PCHIDs always within a range of 4 adjacent PCHIDs that
+        # start at a multiple of 4.
+
+        self_pchid = int(self.prop('adapter-id'), 16)
+        if self_pchid >= int('7c0', 16):
+            # A virtual adapter with a single PCHID -> no siblings
+            return []
+
+        # A physical adapter with a total of 4 PCHIDs reserved for the slot
+        pchid_base = self_pchid // 4 * 4
+        sibling_pchids = list(range(pchid_base, pchid_base + 4))
+        sibling_pchids.remove(self_pchid)
+        sibling_adapter_ids = ['{:03x}'.format(p) for p in sibling_pchids]
+        filter_args = {'adapter-id': sibling_adapter_ids}
+        sibling_adapters = self.manager.cpc.adapters.list(
+            full_properties, filter_args)
+        return sibling_adapters
```

### Comparing `zhmcclient-1.7.3/zhmcclient/_capacity_group.py` & `zhmcclient-1.8.0/zhmcclient/_capacity_group.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.7.3/zhmcclient/_client.py` & `zhmcclient-1.8.0/zhmcclient/_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,14 +225,15 @@
                 self.query_api_version()
             except Error:
                 pass
             else:
                 break
             if operation_timeout > 0:
                 current_time = time.time()
+                # noinspection PyUnboundLocalVariable
                 if current_time > start_time + operation_timeout:
                     raise OperationTimeout(
                         "Waiting for Console at {} to become available timed "
                         "out (operation timeout: {} s)".
                         format(self.session.host, operation_timeout),
                         operation_timeout)
             time.sleep(10)  # Avoid hot spin loop
@@ -289,15 +290,15 @@
         as an HMC definition dictionary.
 
         This method can be used on clients for sessions to real HMCs and
         faked sessions.
 
         The returned dictionary has only items of type dict, list, string,
         int, float, bool or None. That makes it convertible to simple formats
-        such as JSON or YAML so it can be externalized (e.g. persisted).
+        such as JSON or YAML, so it can be externalized (e.g. persisted).
 
         The returned dictionary can be used to instantiate a faked session
         using :meth:`zhmcclient_mock.FakedSession.from_hmc_dict`.
 
         The returned HMC definition dictionary has the following format::
 
             {
```

### Comparing `zhmcclient-1.7.3/zhmcclient/_console.py` & `zhmcclient-1.8.0/zhmcclient/_console.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,17 @@
 from ._user import UserManager
 from ._user_role import UserRoleManager
 from ._user_pattern import UserPatternManager
 from ._password_rule import PasswordRuleManager
 from ._task import TaskManager
 from ._ldap_server_definition import LdapServerDefinitionManager
 from ._unmanaged_cpc import UnmanagedCpcManager
+from ._group import GroupManager
+from ._utils import get_features
+from ._certificates import CertificateManager
 
 __all__ = ['ConsoleManager', 'Console']
 
 
 class ConsoleManager(BaseManager):
     """
     Manager providing access to the :term:`Console` representing the HMC this
@@ -71,15 +74,16 @@
             session=client.session,
             parent=None,
             base_uri='/api/console',
             oid_prop='object-id',
             uri_prop='object-uri',
             name_prop='name',
             query_props=None,
-            list_has_name=False)
+            list_has_name=False,
+            supports_properties=True)
         self._client = client
         self._console = None
 
     @property
     def client(self):
         """
         :class:`~zhmcclient.Client`:
@@ -108,15 +112,15 @@
           retrieved.
         """
         if self._console is None:
             self._console = self.resource_object('/api/console')
         return self._console
 
     @logged_api_call
-    def list(self, full_properties=True, filter_args=None):
+    def list(self, full_properties=False, filter_args=None):
         """
         List the (one) :term:`Console` representing the HMC this client is
         connected to.
 
         Authorization requirements:
 
         * None
@@ -193,14 +197,16 @@
         self._users = None
         self._user_roles = None
         self._user_patterns = None
         self._password_rules = None
         self._tasks = None
         self._ldap_server_definitions = None
         self._unmanaged_cpcs = None
+        self._groups = None
+        self._certificates = None
 
     @property
     def storage_groups(self):
         """
         :class:`~zhmcclient.StorageGroupManager`:
           Manager object for the Storage Groups in scope of this Console.
         """
@@ -295,14 +301,25 @@
         :term:`CPCs <CPC>` in this Console.
         """
         # We do here some lazy loading.
         if not self._unmanaged_cpcs:
             self._unmanaged_cpcs = UnmanagedCpcManager(self)
         return self._unmanaged_cpcs
 
+    @property
+    def groups(self):
+        """
+        :class:`~zhmcclient.GroupManager`: Access to user-defined
+        :term:`Groups <Group>` in this Console.
+        """
+        # We do here some lazy loading.
+        if not self._groups:
+            self._groups = GroupManager(self)
+        return self._groups
+
     @logged_api_call
     def restart(self, force=False, wait_for_available=True,
                 operation_timeout=None):
         """
         Restart the HMC represented by this Console object.
 
         Once the HMC is online again, this Console object, as well as any other
@@ -799,14 +816,51 @@
                 if matches_filters(lpar_obj, client_filters):
                     lpar_objs.append(lpar_obj)
                     if full_properties:
                         lpar_obj.pull_full_properties()
 
         return lpar_objs
 
+    @logged_api_call
+    def list_api_features(self, name=None):
+        """
+        Returns information about the Web Services API features (introduced with
+        Web Services version 4.10) available on this console, see
+        :ref:`Feature enablement`.
+
+        Parameters:
+
+          name:
+            A regular expression used to limit returned objects to those that
+            have a matching name field.
+
+        Authorization requirements:
+
+        * None
+
+        Returns:
+
+          list of strings: The list of API features that are available on this
+          client. For API versions prior to 4.10, an empty list is returned.
+
+        """
+        # TODO: add reference to WSAPI book chapter regarding API features
+        return get_features(self.manager.session, '/api/console', name)
+
+    @property
+    def certificates(self):
+        """
+        :class:`~zhmcclient.CertificateManager`: Access to the
+        :term:`Certificates <Certificate>` in this HMC.
+        """
+        # We do here some lazy loading.
+        if not self._certificates:
+            self._certificates = CertificateManager(self)
+        return self._certificates
+
     def dump(self):
         """
         Dump this Console resource with its properties and child resources
         (recursively) as a resource definition.
 
         The returned resource definition has the following format::
```

### Comparing `zhmcclient-1.7.3/zhmcclient/_constants.py` & `zhmcclient-1.8.0/zhmcclient/_constants.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.7.3/zhmcclient/_cpc.py` & `zhmcclient-1.8.0/zhmcclient/_cpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,22 +61,22 @@
 from ._partition import PartitionManager, Partition
 from ._activation_profile import ActivationProfileManager
 from ._adapter import AdapterManager
 from ._virtual_switch import VirtualSwitchManager
 from ._capacity_group import CapacityGroupManager
 from ._logging import logged_api_call
 from ._exceptions import ParseError, ConsistencyError
-from ._utils import matches_filters, divide_filter_args, \
+from ._utils import get_features, matches_filters, divide_filter_args, \
     RC_CPC, RC_ADAPTER, RC_CAPACITY_GROUP, RC_HBA, RC_NIC, RC_PARTITION, \
     RC_NETWORK_PORT, RC_STORAGE_PORT, RC_STORAGE_TEMPLATE, RC_STORAGE_GROUP, \
     RC_STORAGE_TEMPLATE_VOLUME, RC_STORAGE_VOLUME, RC_VIRTUAL_FUNCTION, \
     RC_VIRTUAL_STORAGE_RESOURCE, RC_VIRTUAL_SWITCH, RC_STORAGE_SITE, \
     RC_STORAGE_FABRIC, RC_STORAGE_SWITCH, RC_STORAGE_SUBSYSTEM, \
     RC_STORAGE_PATH, RC_STORAGE_CONTROL_UNIT, RC_VIRTUAL_TAPE_RESOURCE, \
-    RC_TAPE_LINK, RC_TAPE_LIBRARY
+    RC_TAPE_LINK, RC_TAPE_LIBRARY, RC_CERTIFICATE
 
 __all__ = ['CpcManager', 'Cpc']
 
 
 class CpcManager(BaseManager):
     """
     Manager providing access to the managed :term:`CPCs <CPC>` exposed by the
@@ -109,15 +109,16 @@
             class_name=RC_CPC,
             session=client.session,
             parent=None,
             base_uri='/api/cpcs',
             oid_prop='object-id',
             uri_prop='object-uri',
             name_prop='name',
-            query_props=query_props)
+            query_props=query_props,
+            supports_properties=True)
         self._client = client
 
     @property
     def client(self):
         """
         :class:`~zhmcclient.Client`:
           The client defining the scope for this manager.
@@ -1118,15 +1119,15 @@
         crypto adapters in this CPC.
 
         A crypto domain is considered free for usage if it is not assigned to
         any defined partition of this CPC in access mode 'control-usage' on any
         of the specified crypto adapters.
 
         For this test, all currently defined partitions of this CPC are
-        checked, regardless of whether or not they are active. This ensures
+        checked, regardless of whether they are active. This ensures
         that a crypto domain that is found to be free for usage can be assigned
         to a partition for 'control-usage' access to the specified crypto
         adapters, without causing a crypto domain conflict when activating that
         partition.
 
         Note that a similar notion of free domains does not exist for access
         mode 'control', because a crypto domain on a crypto adapter can be
@@ -1334,15 +1335,15 @@
         return result
 
     @logged_api_call
     def set_power_capping(self, power_capping_state, power_cap=None,
                           wait_for_completion=True, operation_timeout=None):
         """
         Set the power capping settings of this CPC. The power capping settings
-        of a CPC define whether or not the power consumption of the CPC is
+        of a CPC define whether the power consumption of the CPC is
         limited and if so, what the limit is. Use this method to limit the
         peak power consumption of a CPC, or to remove a power consumption
         limit for a CPC.
 
         The current power capping settings in effect for a CPC are described in
         the "cpc-power-capping-state" and "cpc-power-cap-current" properties of
         the CPC.
@@ -1909,14 +1910,20 @@
         This method performs the "Import DPM Configuration" HMC operation.
 
         This method requires the CPC to be in DPM mode.
 
         Authorization requirements:
 
         * Object-access permission to this CPC.
+        * Object-access permission to Secure Boot Certificate objects (only
+          applies when the request body contains one or more secure boot
+          Certificate objects to be assigned to Partitions).
+        * Task permission for the "Import Secure Boot Certificates" task
+          (only applies when the request body contains one or more Certificate
+          objects).
         * Task permission to the "Import Dynamic Partition Manager
           Configuration" task.
 
         Parameters:
 
           dpm_configuration (dict): A DPM configuration, represented as a
             dictionary with the fields described for the
@@ -1967,27 +1974,30 @@
     def export_dpm_configuration(self, include_unused_adapters=False):
         """
         Export a DPM configuration from this CPC and return it.
 
         The DPM configuration includes settable CPC properties and all DPM
         specific objects of or associated with the CPC, such as adapters with
         their ports, virtual switches, partitions with their child objects,
-        capacity groups, and various storage and tape related resources.
+        capacity groups, various storage and tape related resources, and
+        certificate objects.
 
         By default, only those adapters of the CPC are exported that are
         referenced by other DPM specific objects.
 
         This method performs the "Get Inventory" HMC operation and extracts
         the relevant elements into the result.
 
         This method requires the CPC to be in DPM mode.
 
         Authorization requirements:
 
         * Object-access permission to this CPC.
+        * Object-access permission to all Certificate objects associated to
+          this CPC.
 
         Parameters:
 
           include_unused_adapters (bool):
             Controls whether the full set of adapters should be returned,
             vs. only those that are referenced by other DPM objects that
             are part of the return data.
@@ -2022,18 +2032,47 @@
           :exc:`~zhmcclient.ParseError`
           :exc:`~zhmcclient.AuthError`
           :exc:`~zhmcclient.ConnectionError`
           :exc:`~zhmcclient.ConsistencyError` - issues with inventory data
         """
         inventory_list = retrieveInventoryData(self.manager.client)
         cpc_uri = self.get_property('object-uri')
-        config_dict = convertToConfig(inventory_list, cpc_uri,
-                                      include_unused_adapters)
+        config_dict = convertToConfig(self.manager.console, inventory_list,
+                                      cpc_uri, include_unused_adapters)
+        features = self.list_api_features()
+        if len(features) > 0:
+            config_dict['available-api-features-list'] = features
         return config_dict
 
+    @logged_api_call
+    def list_api_features(self, name=None):
+        """
+        Returns information about the Web Services API features (introduced with
+        Web Services version 4.10) available on the CPC, see
+        :ref:`Feature enablement`.
+
+        Parameters:
+
+          name:
+            A regular expression used to limit returned objects to those that
+            have a matching name field.
+
+        Authorization requirements:
+
+        * None
+
+        Returns:
+
+          list of strings: The list of API features that are available on this
+          CPC. For API versions prior to 4.10, an empty list is returned.
+
+        """
+        # TODO: add reference to WSAPI book chapter regarding API features
+        return get_features(self.manager.session, self.uri, name)
+
 
 # Functions used by Cpc.export_dpm_configuration().
 # Some of these functions were adapted from code in the
 # exportDpmResourcesToFile.py script available at
 # https://www-01.ibm.com/servers/resourcelink/lib03020.nsf/0/2C88A77CEA71062E8525829500667BCD?OpenDocument
 
 def extractByParent(classname, parent_list, inventory_list):
@@ -2141,14 +2180,18 @@
 
 def retrieveInventoryData(client):
     """
     Retrieve inventory data from the HMC.
     Returns the inventory list from Client.get_inventory().
     """
     resource_classes = ['dpm-resources', 'cpc']
+    api_features = client.consoles.console.list_api_features()
+    if 'secure-boot-with-certificates' in api_features:
+        resource_classes.append('certificate-resources')
+
     inventory_list = client.get_inventory(resource_classes)
     error_msgs = []
     for item in inventory_list:
         if item.get('class') == 'inventory-error':
             msg = ("Inventory error {} for resource with URI {}: {}; "
                    "Details: {}".format(
                        item.get('inventory-error-code'),
@@ -2159,15 +2202,15 @@
     if error_msgs:
         raise ConsistencyError(
             "Some resources could not be fully inventoried:\n  {}".
             format('\n  '.join(error_msgs)))
     return inventory_list
 
 
-def convertToConfig(inventory_list, cpc_uri, include_unused_adapters):
+def convertToConfig(console, inventory_list, cpc_uri, include_unused_adapters):
     """
     Convert the inventory list to a DPM configuration dict.
 
     Important: In order to support export of DPM configs with zhmcclient
     versions that have support for newer features from older machines and
     import into older machines, any dictionary items for newly added features
     must be omitted if empty.
@@ -2316,23 +2359,40 @@
 
     classname_for_partition_links = 'partition-link'
     partition_links = extractByPropertyInListValue(
         classname_for_partition_links, 'cpc-uri', cpc_uris, inventory_list)
     if partition_links:
         config_dict['partition-links'] = partition_links
 
+    certificates = extractByPropertyInListValue(
+        RC_CERTIFICATE, 'parent', cpc_uris, inventory_list)
+    if certificates:
+        _add_encoded(console, certificates)
+        config_dict['certificates'] = certificates
+
     if not include_unused_adapters:
-        remove_unreferenced_adapters(config_dict)
+        _remove_unreferenced_adapters(config_dict)
 
     sort_lists(config_dict)
 
     return config_dict
 
 
-def remove_unreferenced_adapters(dpm_config):
+def _add_encoded(console, certificates):
+    """
+    Takes a list of dicts representing certificate objects and adds
+    the corresponding encoded certificate data to each dict.
+    """
+    for cert_dict in certificates:
+        cert = console.certificates.list(
+            filter_args={'name': cert_dict['name']})[0]
+        cert_dict.update(cert.get_encoded())
+
+
+def _remove_unreferenced_adapters(dpm_config):
     """
     Creates a string representation of the given config, EXCLUDING
     adapters AND network-ports. Then iterates the list of adapters,
     to collect those that are referenced by their object-id within that
     string representation. Updates dpm_config in place to use the refined
     adapter list.
     """
```

### Comparing `zhmcclient-1.7.3/zhmcclient/_debug_info.py` & `zhmcclient-1.8.0/zhmcclient/_debug_info.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.7.3/zhmcclient/_exceptions.py` & `zhmcclient-1.8.0/zhmcclient/_exceptions.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.7.3/zhmcclient/_hba.py` & `zhmcclient-1.8.0/zhmcclient/_hba.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.7.3/zhmcclient/_ldap_server_definition.py` & `zhmcclient-1.8.0/zhmcclient/_ldap_server_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         """
         :class:`~zhmcclient.Console`: :term:`Console` defining the scope for
         this manager.
         """
         return self._parent
 
     @logged_api_call
-    def list(self, full_properties=True, filter_args=None):
+    def list(self, full_properties=False, filter_args=None):
         """
         List the :term:`LDAP Server Definition` resources representing the
         definitions of LDAp servers in this HMC.
 
         Authorization requirements:
 
         * User-related-access permission to the LDAP Server Definition objects
```

### Comparing `zhmcclient-1.7.3/zhmcclient/_logging.py` & `zhmcclient-1.8.0/zhmcclient/_logging.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.7.3/zhmcclient/_lpar.py` & `zhmcclient-1.8.0/zhmcclient/_lpar.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,15 +73,16 @@
             class_name=RC_LOGICAL_PARTITION,
             session=cpc.manager.session,
             parent=cpc,
             base_uri='/api/logical-partitions',
             oid_prop='object-id',
             uri_prop='object-uri',
             name_prop='name',
-            query_props=query_props)
+            query_props=query_props,
+            supports_properties=True)
 
     @property
     def cpc(self):
         """
         :class:`~zhmcclient.Cpc`: :term:`CPC` defining the scope for this
         manager.
         """
@@ -1784,7 +1785,71 @@
                 raise StatusTimeout(
                     "Waiting for LPAR {} to reach status(es) '{}' timed out "
                     "after {} s - current status is '{}'".
                     format(self.name, statuses, status_timeout, actual_status),
                     actual_status, statuses, status_timeout)
 
             time.sleep(1)  # Avoid hot spin loop
+
+    @logged_api_call
+    def assign_certificate(self, certificate):
+        """
+        Assigns a :term:`Certificate` to this LPAR.
+
+        :ref:`Feature enablement` requirements:
+
+        *  "secure-boot-with-certificates" must be available on HMC and CPC
+
+        Authorization requirements:
+
+        * Object-access permission to this LPAR.
+        * Object-access permission to the specified certificate.
+        * Task permission to the "Assign Secure Boot Certificates" task.
+
+        Parameters:
+
+          certificate (:class:`~zhmcclient.Certificate`):
+            Certificate to be assigned. The certificate must not currently
+            be assigned to this LPAR.
+
+        Raises:
+
+          :exc:`~zhmcclient.HTTPError`
+          :exc:`~zhmcclient.ParseError`
+          :exc:`~zhmcclient.AuthError`
+          :exc:`~zhmcclient.ConnectionError`
+        """
+        body = {'certificate-uri': certificate.uri}
+        self.manager.session.post(
+            self.uri + '/operations/assign-certificate', body)
+
+    @logged_api_call
+    def unassign_certificate(self, certificate):
+        """
+        Unassign a :term:`Certificate` from this LPAR.
+
+        :ref:`Feature enablement` requirements:
+
+        *  "secure-boot-with-certificates" must be available on HMC and CPC
+
+        Authorization requirements:
+
+        * Object-access permission to this LPAR.
+        * Object-access permission to the specified certificate.
+        * Task permission to the "Assign Secure Boot Certificates" task.
+
+        Parameters:
+
+          certificate (:class:`~zhmcclient.Certificate`):
+            Certificate to be unassigned. The certificate must currently be
+            assigned to this LPAR.
+
+        Raises:
+
+          :exc:`~zhmcclient.HTTPError`
+          :exc:`~zhmcclient.ParseError`
+          :exc:`~zhmcclient.AuthError`
+          :exc:`~zhmcclient.ConnectionError`
+        """
+        body = {'certificate-uri': certificate.uri}
+        self.manager.session.post(
+            self.uri + '/operations/unassign-certificate', body)
```

### Comparing `zhmcclient-1.7.3/zhmcclient/_manager.py` & `zhmcclient-1.8.0/zhmcclient/_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,15 +188,16 @@
     reason, the `__init__()`  method of this class and of its derived manager
     classes are considered internal interfaces and their parameters are not
     documented and may change incompatibly.
     """
 
     def __init__(self, resource_class, class_name, session, parent, base_uri,
                  oid_prop, uri_prop, name_prop, query_props,
-                 list_has_name=True, case_insensitive_names=False):
+                 list_has_name=True, case_insensitive_names=False,
+                 supports_properties=False):
         # This method intentionally has no docstring, because it is internal.
         #
         # Parameters:
         #   resource_class (class):
         #     Python class for the resources of this manager.
         #     Must not be `None`.
         #   class_name (string):
@@ -239,14 +240,18 @@
         #   list_has_name (bool):
         #     Indicates whether the list() method for the resource populates
         #     the name property (i.e. name_prop). For example, for NICs the
         #     list() method returns minimalistic Nic objects without name.
         #   case_insensitive_names (bool):
         #     Indicates whether the name of the resource is treated case
         #     insensitively.
+        #   supports_properties (bool):
+        #     Indicates whether the Get Properties operation for this type of
+        #     resource supports the 'properties' query parameter in the latest
+        #     released version of the HMC.
 
         # We want to surface precondition violations as early as possible,
         # so we test those that are not surfaced through the init code:
         assert resource_class is not None
         assert class_name is not None
         assert session is not None
         assert base_uri is not None
@@ -261,14 +266,15 @@
         self._base_uri = base_uri
         self._oid_prop = oid_prop
         self._uri_prop = uri_prop
         self._name_prop = name_prop
         self._query_props = query_props
         self._list_has_name = list_has_name
         self._case_insensitive_names = case_insensitive_names
+        self._supports_properties = supports_properties
 
         self._name_uri_cache = _NameUriCache(
             self, session.retry_timeout_config.name_uri_cache_timetolive,
             case_insensitive_names)
 
     def __repr__(self):
         """
@@ -284,14 +290,15 @@
             "  _base_uri={_base_uri!r},\n"
             "  _oid_prop={_oid_prop!r},\n"
             "  _uri_prop={_uri_prop!r},\n"
             "  _name_prop={_name_prop!r},\n"
             "  _query_props={_query_props},\n"
             "  _list_has_name={_list_has_name!r},\n"
             "  _case_insensitive_names={_case_insensitive_names!r},\n"
+            "  _supports_properties={_supports_properties!r},\n"
             "  _name_uri_cache={_name_uri_cache!r}\n"
             ")".format(
                 classname=self.__class__.__name__,
                 id=id(self),
                 _resource_class=self._resource_class,
                 _class_name=self._class_name,
                 _session_classname=self._session.__class__.__name__,
@@ -301,14 +308,15 @@
                 _base_uri=self._base_uri,
                 _oid_prop=self._oid_prop,
                 _uri_prop=self._uri_prop,
                 _name_prop=self._name_prop,
                 _query_props=repr_list(self._query_props, indent=2),
                 _list_has_name=self._list_has_name,
                 _case_insensitive_names=self._case_insensitive_names,
+                _supports_properties=self._supports_properties,
                 _name_uri_cache=self._name_uri_cache,
             ))
         return ret
 
     def invalidate_cache(self):
         """
         Invalidate the Name-URI cache of this manager.
@@ -436,14 +444,24 @@
         """
         :class:`py:bool`:
           Indicates whether the names of the resources are treated case
           insensitively.
         """
         return self._case_insensitive_names
 
+    @property
+    def supports_properties(self):
+        """
+        :class:`py:bool`:
+          Indicates whether the "Get Properties" operation for this type of
+          resource supports the 'properties' query parameter in the latest
+          released version of the HMC.
+        """
+        return self._supports_properties
+
     def resource_object(self, uri_or_oid, props=None):
         """
         Return a minimalistic Python resource object for this resource class,
         that is scoped to this manager.
 
         This method is an internal helper function and is not normally called
         by users.
```

### Comparing `zhmcclient-1.7.3/zhmcclient/_metrics.py` & `zhmcclient-1.8.0/zhmcclient/_metrics.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.7.3/zhmcclient/_nic.py` & `zhmcclient-1.8.0/zhmcclient/_nic.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.7.3/zhmcclient/_notification.py` & `zhmcclient-1.8.0/zhmcclient/_notification.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.7.3/zhmcclient/_partition.py` & `zhmcclient-1.8.0/zhmcclient/_partition.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,15 +82,16 @@
             class_name=RC_PARTITION,
             session=cpc.manager.session,
             parent=cpc,
             base_uri='/api/partitions',
             oid_prop='object-id',
             uri_prop='object-uri',
             name_prop='name',
-            query_props=query_props)
+            query_props=query_props,
+            supports_properties=True)
 
     @property
     def cpc(self):
         """
         :class:`~zhmcclient.Cpc`: :term:`CPC` defining the scope for this
         manager.
         """
@@ -254,25 +255,22 @@
 
     @property
     def hbas(self):
         """
         :class:`~zhmcclient.HbaManager`: Access to the :term:`HBAs <HBA>` in
         this Partition.
 
-        If the "dpm-storage-management" feature is enabled, this property is
-        `None`.
+        If the "dpm-storage-management" feature is enabled (i.e. starting with
+        z14), the CPC will not have any HBA objects anymore (they are now
+        Virtual Storage Resources), but this property still provides a manager
+        object for consistency.
         """
         # We do here some lazy loading.
         if not self._hbas:
-            try:
-                dpm_sm = self.feature_enabled('dpm-storage-management')
-            except ValueError:
-                dpm_sm = False
-            if not dpm_sm:
-                self._hbas = HbaManager(self)
+            self._hbas = HbaManager(self)
         return self._hbas
 
     @property
     def virtual_functions(self):
         """
         :class:`~zhmcclient.VirtualFunctionManager`: Access to the
         :term:`Virtual Functions <Virtual Function>` in this Partition.
@@ -1312,14 +1310,78 @@
             for sg_uri in sg_uris:
                 sg = console.storage_groups.resource_object(sg_uri)
                 sg_list.append(sg)
                 if full_properties:
                     sg.pull_full_properties()
         return sg_list
 
+    @logged_api_call
+    def assign_certificate(self, certificate):
+        """
+        Assigns a :term:`Certificate` to this partition.
+
+        :ref:`Feature enablement` requirements:
+
+        *  "secure-boot-with-certificates" must be available on HMC and CPC
+
+        Authorization requirements:
+
+        * Object-access permission to this partition.
+        * Object-access permission to the specified certificate.
+        * Task permission to the "Assign Secure Boot Certificates" task.
+
+        Parameters:
+
+          certificate (:class:`~zhmcclient.Certificate`):
+            Certificate to be assigned. The certificate must not currently
+            be assigned to this partition.
+
+        Raises:
+
+          :exc:`~zhmcclient.HTTPError`
+          :exc:`~zhmcclient.ParseError`
+          :exc:`~zhmcclient.AuthError`
+          :exc:`~zhmcclient.ConnectionError`
+        """
+        body = {'certificate-uri': certificate.uri}
+        self.manager.session.post(
+            self.uri + '/operations/assign-certificate', body)
+
+    @logged_api_call
+    def unassign_certificate(self, certificate):
+        """
+        Unassign a :term:`Certificate` from this partition.
+
+        :ref:`Feature enablement` requirements:
+
+        *  "secure-boot-with-certificates" must be available on HMC and CPC
+
+        Authorization requirements:
+
+        * Object-access permission to this partition.
+        * Object-access permission to the specified certificate.
+        * Task permission to the "Assign Secure Boot Certificates" task.
+
+        Parameters:
+
+          certificate (:class:`~zhmcclient.Certificate`):
+            Certificate to be unassigned. The certificate must currently be
+            assigned to this partition.
+
+        Raises:
+
+          :exc:`~zhmcclient.HTTPError`
+          :exc:`~zhmcclient.ParseError`
+          :exc:`~zhmcclient.AuthError`
+          :exc:`~zhmcclient.ConnectionError`
+        """
+        body = {'certificate-uri': certificate.uri}
+        self.manager.session.post(
+            self.uri + '/operations/unassign-certificate', body)
+
     def dump(self):
         """
         Dump this Partition resource with its properties and child resources
         (recursively) as a resource definition.
 
         The returned resource definition has the following format::
```

### Comparing `zhmcclient-1.7.3/zhmcclient/_password_rule.py` & `zhmcclient-1.8.0/zhmcclient/_password_rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         """
         :class:`~zhmcclient.Console`: :term:`Console` defining the scope for
         this manager.
         """
         return self._parent
 
     @logged_api_call
-    def list(self, full_properties=True, filter_args=None):
+    def list(self, full_properties=False, filter_args=None):
         """
         List the :term:`Password Rule` resources representing the password
         rules defined in this HMC.
 
         Authorization requirements:
 
         * User-related-access permission to the Password Rule objects included
```

### Comparing `zhmcclient-1.7.3/zhmcclient/_port.py` & `zhmcclient-1.8.0/zhmcclient/_port.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.7.3/zhmcclient/_resource.py` & `zhmcclient-1.8.0/zhmcclient/_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from ordereddict import OrderedDict
 # import contextlib
 from immutable_views import DictView
 
 from ._logging import logged_api_call
 from ._utils import repr_dict, repr_timestamp
-from ._exceptions import CeasedExistence
+from ._exceptions import CeasedExistence, HTTPError
 
 __all__ = ['BaseResource']
 
 
 class BaseResource(object):
     """
     Abstract base class for resource classes (e.g. :class:`~zhmcclient.Cpc`)
@@ -260,14 +260,94 @@
         full_properties = self.manager.session.get(self._uri)
         with self._property_lock:
             self._properties = dict(full_properties)
             self._properties_timestamp = int(time.time())
             self._full_properties = True
 
     @logged_api_call
+    def pull_properties(self, properties):
+        """
+        Retrieve the specified set of resource properties and cache them in
+        this zhmcclient object.
+
+        The values of other properties that may already exist in this
+        zhmcclient object remain unchanged.
+
+        If the HMC does not yet support property filtering for this type of
+        resource, the full set of properties is retrieved, as in
+        :meth:`pull_full_properties`.
+
+        This method serializes with other methods that access or change
+        properties on the same Python object.
+
+        Authorization requirements:
+
+        * Object-access permission to this resource.
+
+        Parameters:
+
+          properties (iterable of :term:`string`):
+            The names of one or more properties to be retrieved, using the
+            names defined in the respective 'Data model' section in the
+            :term:`HMC API` book.
+
+        Raises:
+
+          :exc:`~zhmcclient.HTTPError`
+          :exc:`~zhmcclient.ParseError`
+          :exc:`~zhmcclient.AuthError`
+          :exc:`~zhmcclient.ConnectionError`
+          :exc:`~zhmcclient.CeasedExistence`
+        """
+        with self._property_lock:
+            if self._ceased_existence:
+                raise CeasedExistence(self._uri)
+
+        if self.manager.supports_properties:
+            # Note: Older HMC versions may simply ignore the query parameter
+            # and return the full list of properties. Newer HMC versions return
+            # HTTP 400,1 "unrecognized or unsupported query parameter" if it is
+            # not supported for the resource type.
+            uri = "{}?properties={}".format(self._uri, ','.join(properties))
+            try:
+                subset_properties = self.manager.session.get(uri)
+                # pylint: disable=simplifiable-if-statement
+                if len(subset_properties) > len(properties):
+                    # We have an older HMC that ignored the query parameter and
+                    # returned all properties.
+                    is_full = True
+                else:
+                    is_full = False
+            except HTTPError as exc:
+                if exc.http_status == 400 and exc.reason == 1:
+                    # HMC does not yet support the query parameter, get full set
+                    subset_properties = self.manager.session.get(self._uri)
+                    is_full = True
+                else:
+                    raise
+        else:
+            # Resource does not support the query parameter, get full set
+            subset_properties = self.manager.session.get(self._uri)
+            is_full = True
+
+        with self._property_lock:
+            if is_full:
+                self._properties = dict(subset_properties)
+                self._properties_timestamp = int(time.time())
+                self._full_properties = True
+            else:
+                self._properties.update(subset_properties)
+                # We leave the self._full_properties flag unchanged. If the
+                # local object already had full properties pulled earlier, it
+                # now still has all of them.
+                # We leave the self._properties_timestamp unchanged. The
+                # resource now has newer and older properties, and the timestamp
+                # indicates the oldest properties.
+
+    @logged_api_call
     def get_property(self, name):
         """
         Return the value of a resource property.
 
         If the resource property is not cached in this object yet, the full set
         of resource properties is retrieved and cached in this object, and the
         resource property is again attempted to be returned.
```

### Comparing `zhmcclient-1.7.3/zhmcclient/_resource_updater.py` & `zhmcclient-1.8.0/zhmcclient/_resource_updater.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.7.3/zhmcclient/_session.py` & `zhmcclient-1.8.0/zhmcclient/_session.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.7.3/zhmcclient/_storage_group.py` & `zhmcclient-1.8.0/zhmcclient/_storage_group.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.7.3/zhmcclient/_storage_group_template.py` & `zhmcclient-1.8.0/zhmcclient/_storage_group_template.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.7.3/zhmcclient/_storage_volume.py` & `zhmcclient-1.8.0/zhmcclient/_storage_volume.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.7.3/zhmcclient/_storage_volume_template.py` & `zhmcclient-1.8.0/zhmcclient/_storage_volume_template.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.7.3/zhmcclient/_task.py` & `zhmcclient-1.8.0/zhmcclient/_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         """
         :class:`~zhmcclient.Console`: :term:`Console` defining the scope for
         this manager.
         """
         return self._parent
 
     @logged_api_call
-    def list(self, full_properties=True, filter_args=None):
+    def list(self, full_properties=False, filter_args=None):
         """
         List the :term:`Task` resources representing the tasks defined in this
         HMC.
 
         Authorization requirements:
 
         * None
```

### Comparing `zhmcclient-1.7.3/zhmcclient/_timestats.py` & `zhmcclient-1.8.0/zhmcclient/_timestats.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.7.3/zhmcclient/_unmanaged_cpc.py` & `zhmcclient-1.8.0/zhmcclient/_unmanaged_cpc.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.7.3/zhmcclient/_user.py` & `zhmcclient-1.8.0/zhmcclient/_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         """
         :class:`~zhmcclient.Console`: :term:`Console` defining the scope for
         this manager.
         """
         return self._parent
 
     @logged_api_call
-    def list(self, full_properties=True, filter_args=None):
+    def list(self, full_properties=False, filter_args=None):
         """
         List the :term:`User` resources representing the users defined in this
         HMC.
 
         Authorization requirements:
 
         * User-related-access permission to the User object included in the
```

### Comparing `zhmcclient-1.7.3/zhmcclient/_user_pattern.py` & `zhmcclient-1.8.0/zhmcclient/_user_pattern.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         """
         :class:`~zhmcclient.Console`: :term:`Console` defining the scope for
         this manager.
         """
         return self._parent
 
     @logged_api_call
-    def list(self, full_properties=True, filter_args=None):
+    def list(self, full_properties=False, filter_args=None):
         """
         List the :term:`User Pattern` resources representing the user patterns
         defined in this HMC.
 
         Authorization requirements:
 
         * User-related-access permission to the User Pattern objects included
```

### Comparing `zhmcclient-1.7.3/zhmcclient/_user_role.py` & `zhmcclient-1.8.0/zhmcclient/_user_role.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         """
         :class:`~zhmcclient.Console`: :term:`Console` defining the scope for
         this manager.
         """
         return self._parent
 
     @logged_api_call
-    def list(self, full_properties=True, filter_args=None):
+    def list(self, full_properties=False, filter_args=None):
         """
         List the :term:`User Role` resources representing the user roles
         defined in this HMC.
 
         Authorization requirements:
 
         * User-related-access permission to the User Role objects included in
```

### Comparing `zhmcclient-1.7.3/zhmcclient/_utils.py` & `zhmcclient-1.8.0/zhmcclient/_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,25 +16,28 @@
 Utility functions.
 """
 
 from __future__ import absolute_import
 
 import re
 from collections import OrderedDict
+
 try:
     from collections.abc import Mapping, MutableSequence, Iterable
 except ImportError:
     # pylint: disable=deprecated-class
     from collections import Mapping, MutableSequence, Iterable
 from datetime import datetime
 from dateutil import parser
 import six
 import pytz
 from requests.utils import quote
 
+from ._exceptions import HTTPError
+
 __all__ = ['datetime_from_timestamp', 'timestamp_from_datetime']
 
 
 _EPOCH_DT = datetime(1970, 1, 1, 0, 0, 0, 0, pytz.utc)
 
 # Resource class names.
 # These are the values of the 'class' property on the resource objects.
@@ -59,15 +62,15 @@
 RC_STORAGE_SWITCH = 'storage-switch'
 RC_STORAGE_SUBSYSTEM = 'storage-subsystem'
 RC_STORAGE_PATH = 'storage-path'
 RC_STORAGE_CONTROL_UNIT = 'storage-control-unit'
 RC_VIRTUAL_TAPE_RESOURCE = 'virtual-tape-resource'
 RC_TAPE_LINK = 'tape-link'
 RC_TAPE_LIBRARY = 'tape-library'
-
+RC_CERTIFICATE = 'certificate'
 #
 # For CPCs in classic mode:
 RC_RESET_ACTIVATION_PROFILE = 'reset-activation-profile'
 RC_IMAGE_ACTIVATION_PROFILE = 'image-activation-profile'
 RC_LOAD_ACTIVATION_PROFILE = 'load-activation-profile'
 RC_LDAP_SERVER_DEFINITION = 'ldap-server-definition'
 RC_LOGICAL_PARTITION = 'logical-partition'
@@ -76,14 +79,15 @@
 RC_CONSOLE = 'console'
 RC_CPC = 'cpc'
 RC_PASSWORD_RULE = 'password-rule'
 RC_TASK = 'task'
 RC_USER_PATTERN = 'user-pattern'
 RC_USER_ROLE = 'user-role'
 RC_USER = 'user'
+RC_GROUP = 'group'
 
 # Valid resource class names
 #:
 VALID_RESOURCE_CLASSES = frozenset([
     RC_ADAPTER,
     RC_CAPACITY_GROUP,
     RC_HBA,
@@ -115,14 +119,15 @@
     RC_CONSOLE,
     RC_CPC,
     RC_PASSWORD_RULE,
     RC_TASK,
     RC_USER_PATTERN,
     RC_USER_ROLE,
     RC_USER,
+    RC_GROUP,
 ])
 
 
 def _indent(text, amount, ch=' '):
     """Return the indent text, where each line is indented by `amount`
     characters `ch`."""
     padding = amount * ch
@@ -528,7 +533,28 @@
         when the datetime microsecond value is 0.
       * shh:mm - is an optional part specifying the timezone offset with sign,
         hours hh and minutes mm. It is not created when the datetime is
         timezone-naive.
     """
     dt_str = dt.isoformat(sep=' ')
     return dt_str
+
+
+def get_features(session, base_uri, name):
+    """
+    Helper method that GETS the given uri via the given session, appending
+    '/operations/list-features' to the uri (and the query parameter if needed).
+
+    404/Not Found is caught and turned into an empty list result.
+    """
+    try:
+        uri = '{}/operations/list-features'.format(base_uri)
+        if name is not None:
+            uri = '{}?name={}'.format(uri, name)
+        return session.get(uri)
+    except HTTPError as e:
+        # API features are introduced with WS API version 4.10.
+        # Older HMCs will respond with 404/Not Found, which we simply
+        # turn into "no features available at all".
+        if e.http_status == 404:
+            return []
+        raise e
```

### Comparing `zhmcclient-1.7.3/zhmcclient/_version.py` & `zhmcclient-1.8.0/zhmcclient/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 #: The full version of this package including any development levels, as a
 #: :term:`string`.
 #:
 #: Possible formats for this version string are:
 #:
 #: * "M.N.P.dev1": A not yet released version M.N.P
 #: * "M.N.P": A released version M.N.P
-__version__ = '1.7.3'
+__version__ = '1.8.0'
 
 # Check supported Python versions
 # Keep these Python versions in sync with:
 # - python_requires and classifiers in setup.py
 # - Section "Supported environments" in docs/intro.rst
 _PYTHON_M = sys.version_info[0]
 _PYTHON_N = sys.version_info[1]
```

### Comparing `zhmcclient-1.7.3/zhmcclient/_virtual_function.py` & `zhmcclient-1.8.0/zhmcclient/_virtual_function.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.7.3/zhmcclient/_virtual_storage_resource.py` & `zhmcclient-1.8.0/zhmcclient/_virtual_storage_resource.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.7.3/zhmcclient/_virtual_switch.py` & `zhmcclient-1.8.0/zhmcclient/_virtual_switch.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.7.3/zhmcclient/testutils/__init__.py` & `zhmcclient-1.8.0/zhmcclient/testutils/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
-zhmcclient.testutils - Utilities for testing against (real or mocked) HMCs.
+zhmcclient.testutils - Utilities for testing against real or mocked HMCs.
 """
 
 from __future__ import absolute_import
 
 from ._hmc_inventory_file import *         # noqa: F401
 from ._hmc_vault_file import *             # noqa: F401
 from ._hmc_definition import *             # noqa: F401
```

### Comparing `zhmcclient-1.7.3/zhmcclient/testutils/_cpc_fixtures.py` & `zhmcclient-1.8.0/zhmcclient/testutils/_cpc_fixtures.py`

 * *Files 10% similar despite different names*

```diff
@@ -47,16 +47,19 @@
 @pytest.fixture(
     scope='module',
     ids=fixtureid_cpcs
 )
 def all_cpcs(request, hmc_session):  # noqa: F811
     # pylint: disable=redefined-outer-name,unused-argument
     """
-    Pytest fixture representing the set of all CPCs that are defined in the HMC
-    definition file for the selected HMC or HMC group.
+    Pytest fixture representing the set of all CPCs to test against, regardless
+    of their operational mode.
+
+    The CPCs to test against are defined in the ``cpcs`` variable for the
+    HMC entry in the :ref:`HMC inventory file`.
 
     A test function parameter using this fixture resolves to a list of
     :class:`zhmcclient.Cpc` objects representing that set of CPCs. These
     objects have the "short" set of properties from :meth:`zhmcclient.Cpc.list`.
 
     Because the `hmc_session` parameter of this fixture is again a fixture,
     the :func:`zhmcclient.testutils.hmc_session`
@@ -68,16 +71,19 @@
 @pytest.fixture(
     scope='module',
     ids=fixtureid_cpcs
 )
 def dpm_mode_cpcs(request, hmc_session):  # noqa: F811
     # pylint: disable=redefined-outer-name,unused-argument
     """
-    Pytest fixture representing the set of CPCs in DPM mode that are
-    defined in the HMC definition file for the selected HMC or HMC group.
+    Pytest fixture representing the set of CPCs in DPM mode to test against.
+
+    The CPCs to test against are defined in the ``cpcs`` variable in the
+    HMC entry in the :ref:`HMC inventory file` and have their ``dpm_enabled``
+    property set to ``true``.
 
     A test function parameter using this fixture resolves to a list of
     :class:`zhmcclient.Cpc` objects representing that set of CPCs. These
     objects have the "short" set of properties from :meth:`zhmcclient.Cpc.list`.
 
     Because the `hmc_session` parameter of this fixture is again a fixture,
     the :func:`zhmcclient.testutils.hmc_session`
@@ -89,16 +95,19 @@
 @pytest.fixture(
     scope='module',
     ids=fixtureid_cpcs
 )
 def classic_mode_cpcs(request, hmc_session):  # noqa: F811
     # pylint: disable=redefined-outer-name,unused-argument
     """
-    Pytest fixture representing the set of CPCs in classic mode that are
-    defined in the HMC definition file for the selected HMC or HMC group.
+    Pytest fixture representing the set of CPCs in classic mode to test against.
+
+    The CPCs to test against are defined in the ``cpcs`` variable in the
+    HMC entry in the :ref:`HMC inventory file` and have their ``dpm_enabled``
+    property set to ``false``.
 
     A test function parameter using this fixture resolves to a list of
     :class:`zhmcclient.Cpc` objects representing that set of CPCs. These
     objects have the "short" set of properties from :meth:`zhmcclient.Cpc.list`.
 
     Because the `hmc_session` parameter of this fixture is again a fixture,
     the :func:`zhmcclient.testutils.hmc_session`
```

### Comparing `zhmcclient-1.7.3/zhmcclient/testutils/_hmc_definition.py` & `zhmcclient-1.8.0/zhmcclient/testutils/_hmc_definition.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.7.3/zhmcclient/testutils/_hmc_definition_fixtures.py` & `zhmcclient-1.8.0/zhmcclient/testutils/_hmc_definition_fixtures.py`

 * *Files 10% similar despite different names*

```diff
@@ -66,58 +66,61 @@
 @pytest.fixture(
     params=hmc_definitions(load=None),
     scope='module',
     ids=fixtureid_hmc_definition
 )
 def hmc_definition(request):
     """
-    Fixture representing the set of HMC definitions to use for the end2end
-    tests.
+    Pytest fixture representing the set of HMC definitions to use for a test.
 
     A test function parameter using this fixture resolves to the
     :class:`~zhmcclient.testutils.HMCDefinition`
     object of each HMC to test against.
     """
     return request.param
 
 
 @pytest.fixture(
     scope='module'
 )
 def hmc_session(request, hmc_definition):
     # pylint: disable=redefined-outer-name,unused-argument
     """
-    Pytest fixture representing the set of HMC sessions to use for the
-    end2end tests.
-
-    Because the `hmc_definition` parameter of this fixture is again a fixture,
-    the :func:`zhmcclient.testutils.hmc_definition` function needs to be
-    imported as well when this fixture is used.
+    Pytest fixture representing the set of HMC sessions to run a test against.
 
     A test function parameter using this fixture resolves to the
     :class:`zhmcclient.Session` or :class:`zhmcclient_mock.FakedSession` object
-    for the HMC session to test against.
+    for each HMC to test against.
+
     The session is already logged on to the HMC.
 
+    The session object has an additional property named ``hmc_definition``
+    that is the :class:`~zhmcclient.testutils.HMCDefinition` object for the
+    corresponding HMC definition in the :ref:`HMC inventory file`.
+
+    Because the `hmc_definition` parameter of this fixture is again a fixture,
+    the :func:`zhmcclient.testutils.hmc_definition` function needs to be
+    imported as well when this fixture is used.
+
     Upon fixture teardown, the session is automatically logged off from the HMC.
     """
     session = setup_hmc_session(hmc_definition)
     yield session
     teardown_hmc_session(session)
 
 
 def setup_hmc_session(hd):
     """
-    Setup an HMC session and return a new zhmcclient.Session object for it.
+    Setup an HMC session and return a new session object for it.
 
     If the HMC definition represents a real HMC, log on to an HMC and return
-    a new zhmcclient.Session object.
+    a new :class:`zhmcclient.Session` object.
 
     If the HMC definition represents a mocked HMC, create a new mock environment
-    from that and return a zhmcclient_mock.FakedSession object.
+    from that and return a :class:`zhmcclient_mock.FakedSession` object.
     """
     # We use the cached skip reason from previous attempts
     skip_msg = getattr(hd, 'skip_msg', None)
     if skip_msg:
         pytest.skip("Skip reason from earlier attempt: {0}".format(skip_msg))
 
     if hd.mock_file:
```

### Comparing `zhmcclient-1.7.3/zhmcclient/testutils/_hmc_definitions.py` & `zhmcclient-1.8.0/zhmcclient/testutils/_hmc_definitions.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,17 @@
 
 def hmc_definitions(load=True):
     """
     Return the list of HMC definitions to be used for testing.
 
     Parameters:
 
-      load (bool): Load the HMC inventory and vault files.
+      load (bool): Load the HMC inventory and vault files. Otherwise, these
+        files are not loaded. This is used to avoid a dependency on these
+        files for normal zhmcclient users.
         If `None`, the 'TESTEND2END_LOAD' environment variable is used.
 
     Returns:
       list of :class:`zhmcclient.testutils.HMCDefinition`
     """
     hmcdefs = HMCDefinitions(load=load)
     hd_list = hmcdefs.list_hmcs(hmcdefs.testhmc)
@@ -94,50 +96,55 @@
         if vars_dict and key in vars_dict:
             return vars_dict[key]
     return default
 
 
 class HMCNoVaultError(Exception):
     """
-    The HMC vault file does not have a corresponding entry for the HMC.
+    The :ref:`HMC vault file` does not have a corresponding entry for the HMC.
     """
     pass
 
 
 class HMCNotFound(Exception):
     """
-    The HMC group was not found in the HMC inventory file.
+    The HMC group was not found in the :ref:`HMC inventory file`.
     """
     pass
 
 
 class HMCDefinitions(object):
     """
-    The HMC definitions in the HMC inventory and vault files.
+    The HMC definitions in the :ref:`HMC inventory file` and their credentials
+    in the :ref:`HMC vault file`.
     """
 
     def __init__(self, inventory_file=None, vault_file=None, testhmc=None,
                  load=None):
         """
         Parameters:
 
-          inventory_file (string): Path name of HMC inventory file.
+          inventory_file (string): Path name of HMC inventory file`.
             If `None`, the file specified in the 'TESTINVENTORY' environment
-            variable, or the default file in the user's home directory is used.
+            variable or if not set, the default file ``~/.zhmc_inventory.yaml``
+            is used.
 
           vault_file (string): Path name of HMC vault file.
             If `None`, the file specified in the 'TESTVAULT' environment
-            variable, or the default file in the user's home directory is used.
+            variable or if not set, the default file ``~/.zhmc_vault.yaml``
+            is used.
 
-          testhmc (string): Group name or HMC nickname in HMC inventory file
+          testhmc (string): Group nickname or HMC nickname in HMC inventory file
             to test against.
-            If `None`, the file specified in the 'TESTHMC' environment
-            variable, or the default name is used.
+            If `None`, the nickname specified in the 'TESTHMC' environment
+            variable or if not set, the nickname "default" is used.
 
-          load (bool): Load the HMC inventory and vault files.
+          load (bool): Load the HMC inventory and vault files. Otherwise, these
+            files are not loaded. This is used to avoid a dependency on these
+            files for normal zhmcclient users.
             If `None`, the 'TESTEND2END_LOAD' environment variable is used.
 
         Raises:
           zhmcclient.testutils.HMCInventoryFileError:
           zhmcclient.testutils.HMCVaultFileError:
           zhmcclient.testutils.HMCNoVaultError:
         """
```

### Comparing `zhmcclient-1.7.3/zhmcclient/testutils/_hmc_inventory_file.py` & `zhmcclient-1.8.0/zhmcclient/testutils/_hmc_inventory_file.py`

 * *Files 5% similar despite different names*

```diff
@@ -222,32 +222,32 @@
         },
     },
 }
 
 
 class HMCInventoryFileError(Exception):
     """
-    An error in the HMC inventory file.
+    An error in the :ref:`HMC inventory file`.
     """
     pass
 
 
 class HMCInventoryFile(object):
     """
-    Encapsulation of an HMC inventory file in YAML format.
+    Encapsulation of an :ref:`HMC inventory file` in YAML format.
     """
 
     def __init__(self, filepath):
         self._filepath = filepath
         self._data = OrderedDict()  # File content
         self._load_file()
 
     def _load_file(self):
         """
-        Load and validate the HMC inventory file in YAML format.
+        Load and validate the :ref:`HMC inventory file` in YAML format.
         """
         try:
             # pylint: disable=unspecified-encoding
             with open(self._filepath) as fp:
                 try:
                     data = yaml.load(fp, Loader=yamlloader.ordereddict.Loader)
                 except (yaml.parser.ParserError,
@@ -291,18 +291,20 @@
             "filepath={s.filepath!r}, " \
             "data={s.data!r})". \
             format(s=self)
 
     @property
     def filepath(self):
         """
-        string: Path name of the HMC inventory file.
+        string: Path name of the :ref:`HMC inventory file`.
         """
         return self._filepath
 
     @property
     def data(self):
         """
-        OrderedDict: Content of the HMC inventory file, as nested OrderedDict
-        and list objects.
+        :class:`~py:collections.OrderedDict`: Content of the
+        :ref:`HMC inventory file`, as nested
+        :class:`~py:collections.OrderedDict` and
+        :class:`~py:list` objects.
         """
         return self._data
```

### Comparing `zhmcclient-1.7.3/zhmcclient/testutils/_hmc_vault_file.py` & `zhmcclient-1.8.0/zhmcclient/testutils/_hmc_vault_file.py`

 * *Files 10% similar despite different names*

```diff
@@ -126,32 +126,32 @@
         },
     },
 }
 
 
 class HMCVaultFileError(Exception):
     """
-    An error in the HMC vault file.
+    An error in the :ref:`HMC vault file`.
     """
     pass
 
 
 class HMCVaultFile(object):
     """
-    Encapsulation of an HMC vault file in YAML format.
+    Encapsulation of an :ref:`HMC vault file` in YAML format.
     """
 
     def __init__(self, filepath):
         self._filepath = filepath
         self._data = OrderedDict()  # file content
         self._load_file()
 
     def _load_file(self):
         """
-        Load and validate the HMC vault file in YAML format.
+        Load and validate the :ref:`HMC vault file` in YAML format.
         """
         try:
             # pylint: disable=unspecified-encoding
             with open(self._filepath) as fp:
                 try:
                     data = yaml.load(fp, Loader=yamlloader.ordereddict.Loader)
                 except (yaml.parser.ParserError,
@@ -195,18 +195,20 @@
             "filepath={s.filepath!r}, " \
             "data={s.data!r})". \
             format(s=self)
 
     @property
     def filepath(self):
         """
-        string: Path name of the HMC vault file.
+        string: Path name of the :ref:`HMC vault file`.
         """
         return self._filepath
 
     @property
     def data(self):
         """
-        OrderedDict: Content of the HMC vault file, as nested OrderedDict
-        and list objects.
+        :class:`~py:collections.OrderedDict`: Content of the
+        :ref:`HMC vault file`, as nested
+        :class:`~py:collections.OrderedDict` and
+        :class:`~py:list` objects.
         """
         return self._data
```

### Comparing `zhmcclient-1.7.3/zhmcclient.egg-info/PKG-INFO` & `zhmcclient-1.8.0/zhmcclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhmcclient
-Version: 1.7.3
+Version: 1.8.0
 Summary: A pure Python client library for the IBM Z HMC Web Services API.
 Home-page: https://github.com/zhmcclient/python-zhmcclient
 Author: Juergen Leopold, Andreas Maier
 Author-email: leopoldj@de.ibm.com, maiera@de.ibm.com
 Maintainer: Andreas Maier, Kathir Velusamy
 Maintainer-email: maiera@de.ibm.com, kathir.velu@in.ibm.com
 License: Apache License, Version 2.0
@@ -23,14 +23,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*
 Description-Content-Type: text/x-rst
 Provides-Extra: testutils
 License-File: LICENSE
 
 .. Copyright 2016-2021 IBM Corp. All Rights Reserved.
```

### Comparing `zhmcclient-1.7.3/zhmcclient.egg-info/SOURCES.txt` & `zhmcclient-1.8.0/zhmcclient.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 extra-testutils-requirements.txt
 requirements.txt
 setup.py
 zhmcclient/__init__.py
 zhmcclient/_activation_profile.py
 zhmcclient/_adapter.py
 zhmcclient/_capacity_group.py
+zhmcclient/_certificates.py
 zhmcclient/_client.py
 zhmcclient/_console.py
 zhmcclient/_constants.py
 zhmcclient/_cpc.py
 zhmcclient/_debug_info.py
 zhmcclient/_exceptions.py
+zhmcclient/_group.py
 zhmcclient/_hba.py
 zhmcclient/_ldap_server_definition.py
 zhmcclient/_logging.py
 zhmcclient/_lpar.py
 zhmcclient/_manager.py
 zhmcclient/_metrics.py
 zhmcclient/_nic.py
```

### Comparing `zhmcclient-1.7.3/zhmcclient.egg-info/requires.txt` & `zhmcclient-1.8.0/zhmcclient.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 requests>=2.25.0
 python-dateutil>=2.8.2
 immutable-views>=0.6.0
 nocasedict>=1.0.2
 yamlloader>=0.5.5
-jsonschema!=4.0.0,>=2.6.0
+jsonschema!=4.0.0,>=3.0.1
 urllib3>=1.26.5
+pyrsistent>=0.15.1
 
 [:python_version <= "3.5"]
 stomp.py<5.0.0,>=4.1.23
 PyYAML>=5.3.1
 
 [:python_version <= "3.9"]
 pytz>=2016.10
```

### Comparing `zhmcclient-1.7.3/zhmcclient_mock/__init__.py` & `zhmcclient-1.8.0/zhmcclient_mock/__init__.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.7.3/zhmcclient_mock/_hmc.py` & `zhmcclient-1.8.0/zhmcclient_mock/_hmc.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
            'FakedPasswordRuleManager', 'FakedPasswordRule',
            'FakedTaskManager', 'FakedTask',
            'FakedLdapServerDefinitionManager', 'FakedLdapServerDefinition',
            'FakedActivationProfileManager', 'FakedActivationProfile',
            'FakedAdapterManager', 'FakedAdapter',
            'FakedCpcManager', 'FakedCpc',
            'FakedUnmanagedCpcManager', 'FakedUnmanagedCpc',
+           'FakedGroupManager', 'FakedGroup',
            'FakedHbaManager', 'FakedHba',
            'FakedLparManager', 'FakedLpar',
            'FakedNicManager', 'FakedNic',
            'FakedPartitionManager', 'FakedPartition',
            'FakedPortManager', 'FakedPort',
            'FakedVirtualFunctionManager', 'FakedVirtualFunction',
            'FakedVirtualSwitchManager', 'FakedVirtualSwitch',
@@ -1103,14 +1104,15 @@
         self._password_rules = FakedPasswordRuleManager(
             hmc=manager.hmc, console=self)
         self._tasks = FakedTaskManager(hmc=manager.hmc, console=self)
         self._ldap_server_definitions = FakedLdapServerDefinitionManager(
             hmc=manager.hmc, console=self)
         self._unmanaged_cpcs = FakedUnmanagedCpcManager(
             hmc=manager.hmc, console=self)
+        self._groups = FakedGroupManager(hmc=manager.hmc, console=self)
 
     def __repr__(self):
         """
         Return a string with the state of this faked Console resource, for
         debug purposes.
         """
         ret = (
@@ -1123,14 +1125,15 @@
             "  _users = {_users}\n"
             "  _user_roles = {_user_roles}\n"
             "  _user_patterns = {_user_patterns}\n"
             "  _password_rules = {_password_rules}\n"
             "  _tasks = {_tasks}\n"
             "  _ldap_server_definitions = {_ldap_server_definitions}\n"
             "  _unmanaged_cpcs = {_unmanaged_cpcs}\n"
+            "  _groups = {_groups}\n"
             ")".format(
                 classname=self.__class__.__name__,
                 id=id(self),
                 manager_classname=self._manager.__class__.__name__,
                 manager_id=id(self._manager),
                 parent_uri=self._manager.parent.uri,
                 _uri=self._uri,
@@ -1140,14 +1143,15 @@
                 _user_roles=repr_manager(self.user_roles, indent=2),
                 _user_patterns=repr_manager(self.user_patterns, indent=2),
                 _password_rules=repr_manager(self.password_rules, indent=2),
                 _tasks=repr_manager(self.tasks, indent=2),
                 _ldap_server_definitions=repr_manager(
                     self.ldap_server_definitions, indent=2),
                 _unmanaged_cpcs=repr_manager(self.unmanaged_cpcs, indent=2),
+                _groups=repr_manager(self.groups, indent=2),
             ))
         return ret
 
     @property
     def storage_groups(self):
         """
         :class:`~zhmcclient_mock.FakedStorageGroupManager`: Access to the faked
@@ -1207,14 +1211,22 @@
     def unmanaged_cpcs(self):
         """
         :class:`~zhmcclient_mock.FakedUnmanagedCpcManager`: Access to the faked
         unmanaged CPC resources of this Console.
         """
         return self._unmanaged_cpcs
 
+    @property
+    def groups(self):
+        """
+        :class:`~zhmcclient_mock.FakedGroupManager`: Access to the faked
+        group resources of this Console.
+        """
+        return self._groups
+
 
 class FakedUserManager(FakedBaseManager):
     """
     A manager for faked User resources within a faked HMC (see
     :class:`zhmcclient_mock.FakedHmc`).
 
     Derived from :class:`zhmcclient_mock.FakedBaseManager`, see there for
@@ -2139,14 +2151,102 @@
         """
         ret = (
             "{classname} at 0x{id:08x} (\n"
             "  _manager = {manager_classname} at 0x{manager_id:08x}\n"
             "  _manager._parent._uri = {parent_uri!r}\n"
             "  _uri = {_uri!r}\n"
             "  _properties = {_properties}\n"
+            ")".format(
+                classname=self.__class__.__name__,
+                id=id(self),
+                manager_classname=self._manager.__class__.__name__,
+                manager_id=id(self._manager),
+                parent_uri=self._manager.parent.uri,
+                _uri=self._uri,
+                _properties=repr_dict(self._properties, indent=2),
+            ))
+        return ret
+
+
+class FakedGroupManager(FakedBaseManager):
+    """
+    A manager for faked managed Group resources within a faked HMC (see
+    :class:`zhmcclient_mock.FakedHmc`).
+
+    Derived from :class:`zhmcclient_mock.FakedBaseManager`, see there for
+    common methods and attributes.
+    """
+
+    def __init__(self, hmc, console):
+        super(FakedGroupManager, self).__init__(
+            hmc=hmc,
+            parent=console,
+            resource_class=FakedGroup,
+            base_uri=self.api_root + '/groups',
+            oid_prop='object-id',
+            uri_prop='object-uri',
+            class_value='group',
+            name_prop='name')
+
+    def add(self, properties):
+        # pylint: disable=useless-super-delegation
+        """
+        Add a faked Group resource.
+
+        Parameters:
+
+          properties (dict):
+            Resource properties.
+
+            Special handling and requirements for certain properties:
+
+            * 'object-id' will be auto-generated with a unique value across
+              all instances of this resource type, if not specified.
+            * 'object-uri' will be auto-generated based upon the object ID,
+              if not specified.
+            * 'class' will be auto-generated to 'group',
+              if not specified.
+
+        Returns:
+          :class:`~zhmcclient_mock.FakedGroup`: The faked Group resource.
+        """
+        new_group = super(FakedGroupManager, self).add(properties)
+
+        # Set optional properties to their defaults
+        new_group.properties.setdefault('description', '')
+        new_group.properties.setdefault('match-info', None)
+
+        return new_group
+
+
+class FakedGroup(FakedBaseResource):
+    """
+    A faked managed Group resource within a faked HMC (see
+    :class:`zhmcclient_mock.FakedHmc`).
+
+    Derived from :class:`zhmcclient_mock.FakedBaseResource`, see there for
+    common methods and attributes.
+    """
+
+    def __init__(self, manager, properties):
+        super(FakedGroup, self).__init__(
+            manager=manager,
+            properties=properties)
+
+    def __repr__(self):
+        """
+        Return a string with the state of this faked Group resource, for debug
+        purposes.
+        """
+        ret = (
+            "{classname} at 0x{id:08x} (\n"
+            "  _manager = {manager_classname} at 0x{manager_id:08x}\n"
+            "  _manager._parent._uri = {parent_uri!r}\n"
+            "  _uri = {_uri!r}\n"
+            "  _properties = {_properties}\n"
             ")".format(
                 classname=self.__class__.__name__,
                 id=id(self),
                 manager_classname=self._manager.__class__.__name__,
                 manager_id=id(self._manager),
                 parent_uri=self._manager.parent.uri,
                 _uri=self._uri,
```

### Comparing `zhmcclient-1.7.3/zhmcclient_mock/_idpool.py` & `zhmcclient-1.8.0/zhmcclient_mock/_idpool.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.7.3/zhmcclient_mock/_session.py` & `zhmcclient-1.8.0/zhmcclient_mock/_session.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.7.3/zhmcclient_mock/_urihandler.py` & `zhmcclient-1.8.0/zhmcclient_mock/_urihandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -2061,14 +2061,160 @@
             raise new_exc  # zhmcclient_mock.InvalidResourceError
         check_required_fields(method, uri, body, ['auto-start-list'])
         auto_start_list = body['auto-start-list']
         # Store it in the CPC
         cpc.properties['auto-start-list'] = auto_start_list
 
 
+class GroupsHandler(object):
+    """
+    Handler class for HTTP methods on set of Group resources.
+    """
+
+    @staticmethod
+    def get(method, hmc, uri, uri_parms, logon_required):
+        # pylint: disable=unused-argument
+        """Operation: List Custom Groups."""
+        query_str = uri_parms[0]
+        try:
+            console = hmc.consoles.lookup_by_oid(None)
+        except KeyError:
+            new_exc = InvalidResourceError(method, uri)
+            new_exc.__cause__ = None
+            raise new_exc  # zhmcclient_mock.InvalidResourceError
+        result_groups = []
+        filter_args = parse_query_parms(method, uri, query_str)
+        for group in console.groups.list(filter_args):
+            result_group = {}
+            for prop in group.properties:
+                if prop in ('object-uri', 'name'):
+                    result_group[prop] = group.properties[prop]
+            result_groups.append(result_group)
+        return {'groups': result_groups}
+
+    @staticmethod
+    def post(method, hmc, uri, uri_parms, body, logon_required,
+             wait_for_completion):
+        # pylint: disable=unused-argument
+        """Operation: Create Custom Group."""
+
+        assert wait_for_completion is True  # async not supported yet
+        try:
+            console = hmc.consoles.lookup_by_oid(None)
+        except KeyError:
+            new_exc = InvalidResourceError(method, uri)
+            new_exc.__cause__ = None
+            raise new_exc  # zhmcclient_mock.InvalidResourceError
+        check_required_fields(method, uri, body, ['name'])
+
+        properties = copy.deepcopy(body)
+
+        # Set defaults for optional input properties
+        properties.setdefault('description', '')
+        properties.setdefault('match-info', None)
+
+        # Set non-input properties
+        properties['members'] = []
+
+        # Reflect the result of creating the partition
+        new_group = console.groups.add(properties)
+        return {'object-uri': new_group.uri}
+
+
+class GroupHandler(GenericGetPropertiesHandler):
+    """
+    Handler class for HTTP methods on single Group resource.
+    """
+
+    @staticmethod
+    def delete(method, hmc, uri, uri_parms, logon_required):
+        # pylint: disable=unused-argument
+        """Operation: Delete Custom Group."""
+        try:
+            group = hmc.lookup_by_uri(uri)
+        except KeyError:
+            new_exc = InvalidResourceError(method, uri)
+            new_exc.__cause__ = None
+            raise new_exc  # zhmcclient_mock.InvalidResourceError
+
+        # Reflect the result of deleting the group
+        group.manager.remove(group.oid)
+
+
+class GroupAddMemberHandler(object):
+    """
+    Handler class for operation: Add Member to Custom Group.
+    """
+
+    @staticmethod
+    def post(method, hmc, uri, uri_parms, body, logon_required,
+             wait_for_completion):
+        # pylint: disable=unused-argument
+        """Operation: Add Member to Custom Group."""
+        assert wait_for_completion is True  # async not supported yet
+        group_oid = uri_parms[0]
+        try:
+            group = hmc.groups.lookup_by_oid(group_oid)
+        except KeyError:
+            new_exc = InvalidResourceError(method, uri)
+            new_exc.__cause__ = None
+            raise new_exc  # zhmcclient_mock.InvalidResourceError
+        check_required_fields(method, uri, body, ['object-uri'])
+
+        object_uri = body['object-uri']
+
+        group.properties['members'].append(object_uri)
+
+
+class GroupRemoveMemberHandler(object):
+    """
+    Handler class for operation: Remove Member from Custom Group.
+    """
+
+    @staticmethod
+    def post(method, hmc, uri, uri_parms, body, logon_required,
+             wait_for_completion):
+        # pylint: disable=unused-argument
+        """Operation: Remove Member from Custom Group."""
+        assert wait_for_completion is True  # async not supported yet
+        group_oid = uri_parms[0]
+        try:
+            group = hmc.groups.lookup_by_oid(group_oid)
+        except KeyError:
+            new_exc = InvalidResourceError(method, uri)
+            new_exc.__cause__ = None
+            raise new_exc  # zhmcclient_mock.InvalidResourceError
+        check_required_fields(method, uri, body, ['object-uri'])
+
+        object_uri = body['object-uri']
+
+        group.properties['members'].remove(object_uri)
+
+
+class GroupMembersHandler(object):
+    """
+    Handler class for operation: List Custom Group Members.
+    """
+
+    @staticmethod
+    def get(method, hmc, uri, uri_parms, logon_required):
+        # pylint: disable=unused-argument
+        """Operation: List Custom Group Members."""
+        group_oid = uri_parms[0]
+        try:
+            group = hmc.groups.lookup_by_oid(group_oid)
+        except KeyError:
+            new_exc = InvalidResourceError(method, uri)
+            new_exc.__cause__ = None
+            raise new_exc  # zhmcclient_mock.InvalidResourceError
+
+        result = {'members': group.properties['members']}
+        return result
+
+
 class MetricsContextsHandler(object):
     """
     Handler class for HTTP methods on set of MetricsContext resources.
     """
 
     @staticmethod
     def post(method, hmc, uri, uri_parms, body, logon_required,
@@ -4761,14 +4907,20 @@
     (r'/api/cpcs/([^/]+)/operations/set-cpc-power-save',
      CpcSetPowerSaveHandler),
     (r'/api/cpcs/([^/]+)/operations/set-cpc-power-capping',
      CpcSetPowerCappingHandler),
     (r'/api/cpcs/([^/]+)/energy-management-data',
      CpcGetEnergyManagementDataHandler),
 
+    (r'/api/groups(?:\?(.*))?', GroupsHandler),
+    (r'/api/groups/([^/]+)', GroupHandler),
+    (r'/api/groups/([^/]+)/operations/add-member', GroupAddMemberHandler),
+    (r'/api/groups/([^/]+)/operations/remove-member', GroupRemoveMemberHandler),
+    (r'/api/groups/([^/]+)/members', GroupMembersHandler),
+
     (r'/api/services/metrics/context', MetricsContextsHandler),
     (r'/api/services/metrics/context/([^/]+)', MetricsContextHandler),
 
     # Only in DPM mode:
 
     (r'/api/cpcs/([^/]+)/operations/start', CpcStartHandler),
     (r'/api/cpcs/([^/]+)/operations/stop', CpcStopHandler),
```

