# Comparing `tmp/netbox-validity-1.1.0.tar.gz` & `tmp/netbox-validity-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-validity-1.1.0.tar", last modified: Wed May  3 23:20:04 2023, max compression
+gzip compressed data, was "netbox-validity-1.2.0.tar", last modified: Tue May 16 00:03:00 2023, max compression
```

## Comparing `netbox-validity-1.1.0.tar` & `netbox-validity-1.2.0.tar`

### file list

```diff
@@ -1,130 +1,136 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.958199 netbox-validity-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-05-03 23:20:04.958199 netbox-validity-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.946199 netbox-validity-1.1.0/netbox_validity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-05-03 23:20:04.000000 netbox-validity-1.1.0/netbox_validity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-05-03 23:20:04.000000 netbox-validity-1.1.0/netbox_validity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 23:20:04.000000 netbox-validity-1.1.0/netbox_validity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-03 23:20:04.000000 netbox-validity-1.1.0/netbox_validity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-03 23:20:04.000000 netbox-validity-1.1.0/netbox_validity.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.946199 netbox-validity-1.1.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 23:20:04.958199 netbox-validity-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.946199 netbox-validity-1.1.0/validity/
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.946199 netbox-validity-1.1.0/validity/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/api/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/choices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.946199 netbox-validity-1.1.0/validity/config_compliance/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.946199 netbox-validity-1.1.0/validity/config_compliance/device_config/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/config_compliance/device_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/config_compliance/device_config/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/config_compliance/device_config/routeros.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/config_compliance/device_config/ttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/config_compliance/device_config/yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/config_compliance/dynamic_pairs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.946199 netbox-validity-1.1.0/validity/config_compliance/eval/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/config_compliance/eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/config_compliance/eval/default_nameset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/config_compliance/eval/eval.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/config_compliance/eval/eval_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/config_compliance/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/filtersets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.950199 netbox-validity-1.1.0/validity/forms/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/forms/filterset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/forms/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/forms/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.950199 netbox-validity-1.1.0/validity/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.950199 netbox-validity-1.1.0/validity/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/management/commands/linkscripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.950199 netbox-validity-1.1.0/validity/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    12486 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/migrations/0002_custom_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.950199 netbox-validity-1.1.0/validity/models/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/models/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/models/nameset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/models/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/models/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/models/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/models/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/models/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/models/test_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/navigation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.950199 netbox-validity-1.1.0/validity/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/scripts/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/scripts/run_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.942199 netbox-validity-1.1.0/validity/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.954199 netbox-validity-1.1.0/validity/templates/validity/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/templates/validity/compliance_results.html
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/templates/validity/compliancereport.html
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/templates/validity/complianceselector.html
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/templates/validity/compliancetest.html
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/templates/validity/compliancetestresult.html
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/templates/validity/configserializer.html
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/templates/validity/device_config.html
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/templates/validity/gitrepo.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.954199 netbox-validity-1.1.0/validity/templates/validity/inc/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/templates/validity/inc/git_link.html
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/templates/validity/inc/path_with_link.html
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/templates/validity/inc/report_stats_row.html
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/templates/validity/nameset.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.954199 netbox-validity-1.1.0/validity/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/templatetags/validity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.954199 netbox-validity-1.1.0/validity/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/tests/test_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.954199 netbox-validity-1.1.0/validity/tests/test_config_compliance/
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/tests/test_config_compliance/test_device_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/tests/test_config_compliance/test_dynamic_pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/tests/test_config_compliance/test_eval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.954199 netbox-validity-1.1.0/validity/tests/test_models/
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/tests/test_models/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/tests/test_models/test_git_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/tests/test_models/test_git_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/tests/test_models/test_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/tests/test_models/test_vdevice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.954199 netbox-validity-1.1.0/validity/tests/test_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/tests/test_scripts/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6793 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/tests/test_scripts/test_run_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.954199 netbox-validity-1.1.0/validity/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/tests/test_utils/test_git.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/tests/test_utils/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.954199 netbox-validity-1.1.0/validity/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/utils/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/utils/password.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:20:04.958199 netbox-validity-1.1.0/validity/views/
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/views/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/views/git_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/views/nameset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/views/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/views/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/views/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/views/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-05-03 23:19:51.000000 netbox-validity-1.1.0/validity/views/test_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.109245 netbox-validity-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-05-16 00:03:00.109245 netbox-validity-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.097245 netbox-validity-1.2.0/netbox_validity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-05-16 00:03:00.000000 netbox-validity-1.2.0/netbox_validity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-05-16 00:03:00.000000 netbox-validity-1.2.0/netbox_validity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 00:03:00.000000 netbox-validity-1.2.0/netbox_validity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-16 00:03:00.000000 netbox-validity-1.2.0/netbox_validity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-16 00:03:00.000000 netbox-validity-1.2.0/netbox_validity.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.097245 netbox-validity-1.2.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 00:03:00.113245 netbox-validity-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.101245 netbox-validity-1.2.0/validity/
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.101245 netbox-validity-1.2.0/validity/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/api/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/choices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.101245 netbox-validity-1.2.0/validity/config_compliance/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.101245 netbox-validity-1.2.0/validity/config_compliance/device_config/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/config_compliance/device_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/config_compliance/device_config/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/config_compliance/device_config/routeros.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/config_compliance/device_config/ttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/config_compliance/device_config/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/config_compliance/dynamic_pairs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.101245 netbox-validity-1.2.0/validity/config_compliance/eval/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/config_compliance/eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/config_compliance/eval/default_nameset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/config_compliance/eval/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/config_compliance/eval/eval_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/config_compliance/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/filtersets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.101245 netbox-validity-1.2.0/validity/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/forms/filterset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/forms/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/forms/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/graphql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.101245 netbox-validity-1.2.0/validity/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.101245 netbox-validity-1.2.0/validity/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/management/commands/linkscripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.101245 netbox-validity-1.2.0/validity/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    12486 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/migrations/0002_custom_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/migrations/0003_complianceselector_dp_tag_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.105245 netbox-validity-1.2.0/validity/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/models/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/models/nameset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/models/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/models/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/models/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/models/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/models/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/models/test_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/navigation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.105245 netbox-validity-1.2.0/validity/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/scripts/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/scripts/run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.097245 netbox-validity-1.2.0/validity/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.105245 netbox-validity-1.2.0/validity/templates/validity/
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/templates/validity/compliance_results.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/templates/validity/compliancereport.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/templates/validity/complianceselector.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/templates/validity/compliancetest.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/templates/validity/compliancetestresult.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/templates/validity/configserializer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/templates/validity/device_config.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/templates/validity/gitrepo.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.105245 netbox-validity-1.2.0/validity/templates/validity/inc/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/templates/validity/inc/git_link.html
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/templates/validity/inc/path_with_link.html
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/templates/validity/inc/report_stats_row.html
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/templates/validity/inc/search_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/templates/validity/nameset.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.105245 netbox-validity-1.2.0/validity/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/templatetags/validity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.109245 netbox-validity-1.2.0/validity/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.109245 netbox-validity-1.2.0/validity/tests/test_config_compliance/
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/tests/test_config_compliance/test_device_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/tests/test_config_compliance/test_dynamic_pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/tests/test_config_compliance/test_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/tests/test_graphql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.109245 netbox-validity-1.2.0/validity/tests/test_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/tests/test_models/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/tests/test_models/test_git_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/tests/test_models/test_git_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/tests/test_models/test_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/tests/test_models/test_vdevice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.109245 netbox-validity-1.2.0/validity/tests/test_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/tests/test_scripts/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/tests/test_scripts/test_run_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.109245 netbox-validity-1.2.0/validity/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/tests/test_utils/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/tests/test_utils/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.109245 netbox-validity-1.2.0/validity/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/utils/password.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.109245 netbox-validity-1.2.0/validity/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/views/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/views/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/views/git_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/views/nameset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/views/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/views/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/views/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/views/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/views/test_result.py
```

### Comparing `netbox-validity-1.1.0/LICENSE` & `netbox-validity-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.1.0/PKG-INFO` & `netbox-validity-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-validity
-Version: 1.1.0
+Version: 1.2.0
 Summary: NetBox plugin for vendor-agnostic configuration compliance
 Author-email: Anton Miasnikov <anton2008m@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Anton Miasnikov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -92,7 +92,11 @@
 
 
 ## Quick Start
 
 The short video about first steps with Validity:
 
 [![Watch the video](https://img.youtube.com/vi/Hs2IUE6rKC4/0.jpg)](https://youtu.be/Hs2IUE6rKC4)
+
+## Contributing
+
+Feel free to ask a [Question](https://github.com/amyasnikov/validity/discussions), report an [Issue](https://github.com/amyasnikov/validity/issues) or even make a [PR](CONTRIBUTING.md). Read more about contribution in the [CONTRIBUTING](CONTRIBUTING.md) guide.
```

### Comparing `netbox-validity-1.1.0/README.md` & `netbox-validity-1.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -44,7 +44,11 @@
 
 
 ## Quick Start
 
 The short video about first steps with Validity:
 
 [![Watch the video](https://img.youtube.com/vi/Hs2IUE6rKC4/0.jpg)](https://youtu.be/Hs2IUE6rKC4)
+
+## Contributing
+
+Feel free to ask a [Question](https://github.com/amyasnikov/validity/discussions), report an [Issue](https://github.com/amyasnikov/validity/issues) or even make a [PR](CONTRIBUTING.md). Read more about contribution in the [CONTRIBUTING](CONTRIBUTING.md) guide.
```

### Comparing `netbox-validity-1.1.0/netbox_validity.egg-info/PKG-INFO` & `netbox-validity-1.2.0/netbox_validity.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-validity
-Version: 1.1.0
+Version: 1.2.0
 Summary: NetBox plugin for vendor-agnostic configuration compliance
 Author-email: Anton Miasnikov <anton2008m@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Anton Miasnikov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -92,7 +92,11 @@
 
 
 ## Quick Start
 
 The short video about first steps with Validity:
 
 [![Watch the video](https://img.youtube.com/vi/Hs2IUE6rKC4/0.jpg)](https://youtu.be/Hs2IUE6rKC4)
+
+## Contributing
+
+Feel free to ask a [Question](https://github.com/amyasnikov/validity/discussions), report an [Issue](https://github.com/amyasnikov/validity/issues) or even make a [PR](CONTRIBUTING.md). Read more about contribution in the [CONTRIBUTING](CONTRIBUTING.md) guide.
```

### Comparing `netbox-validity-1.1.0/netbox_validity.egg-info/SOURCES.txt` & `netbox-validity-1.2.0/netbox_validity.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -9,16 +9,18 @@
 netbox_validity.egg-info/top_level.txt
 requirements/base.txt
 requirements/dev.txt
 requirements/docs.txt
 validity/__init__.py
 validity/choices.py
 validity/filtersets.py
+validity/graphql.py
 validity/managers.py
 validity/navigation.py
+validity/search.py
 validity/tables.py
 validity/urls.py
 validity/api/__init__.py
 validity/api/helpers.py
 validity/api/serializers.py
 validity/api/urls.py
 validity/api/views.py
@@ -38,14 +40,15 @@
 validity/forms/general.py
 validity/forms/helpers.py
 validity/management/__init__.py
 validity/management/commands/__init__.py
 validity/management/commands/linkscripts.py
 validity/migrations/0001_initial.py
 validity/migrations/0002_custom_fields.py
+validity/migrations/0003_complianceselector_dp_tag_prefix.py
 validity/migrations/__init__.py
 validity/models/__init__.py
 validity/models/base.py
 validity/models/device.py
 validity/models/nameset.py
 validity/models/repo.py
 validity/models/report.py
@@ -64,20 +67,22 @@
 validity/templates/validity/configserializer.html
 validity/templates/validity/device_config.html
 validity/templates/validity/gitrepo.html
 validity/templates/validity/nameset.html
 validity/templates/validity/inc/git_link.html
 validity/templates/validity/inc/path_with_link.html
 validity/templates/validity/inc/report_stats_row.html
+validity/templates/validity/inc/search_form.html
 validity/templatetags/__init__.py
 validity/templatetags/validity.py
 validity/tests/base.py
 validity/tests/conftest.py
 validity/tests/factories.py
 validity/tests/test_api.py
+validity/tests/test_graphql.py
 validity/tests/test_version.py
 validity/tests/test_views.py
 validity/tests/test_config_compliance/test_device_config.py
 validity/tests/test_config_compliance/test_dynamic_pairs.py
 validity/tests/test_config_compliance/test_eval.py
 validity/tests/test_models/test_clean.py
 validity/tests/test_models/test_git_link.py
@@ -89,14 +94,15 @@
 validity/tests/test_utils/test_git.py
 validity/tests/test_utils/test_misc.py
 validity/utils/config.py
 validity/utils/git.py
 validity/utils/misc.py
 validity/utils/password.py
 validity/views/__init__.py
+validity/views/base.py
 validity/views/device.py
 validity/views/git_repo.py
 validity/views/nameset.py
 validity/views/report.py
 validity/views/selector.py
 validity/views/serializer.py
 validity/views/test.py
```

### Comparing `netbox-validity-1.1.0/pyproject.toml` & `netbox-validity-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "netbox-validity"
-version = "1.1.0"
+version = "1.2.0"
 description = "NetBox plugin for vendor-agnostic configuration compliance"
 authors = [
     {name = "Anton Miasnikov", email = "anton2008m@gmail.com"},
 ]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `netbox-validity-1.1.0/validity/__init__.py` & `netbox-validity-1.2.0/validity/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,17 +12,18 @@
 
 class NetBoxValidityConfig(PluginConfig):
     name = "validity"
     verbose_name = "Validity: Configuration Compliance"
     description = "Vendor-agnostic framework to build your own configuration compliance rule set"
     author = "Anton Miasnikov"
     author_email = "anton2008m@gmail.com"
-    version = "1.1.0"
+    version = "1.2.0"
     base_url = "validity"
     django_apps = ["bootstrap5"]
+    min_version = "3.4.0"
 
     def ready(self):
         try:
             os.makedirs(settings.git_folder, exist_ok=True)
         except OSError as e:
             if not settings.git_folder.is_dir():
                 logger.error("Cannot create git_folder (%s), %s: %s", settings.git_folder, type(e).__name__, e)
```

### Comparing `netbox-validity-1.1.0/validity/api/helpers.py` & `netbox-validity-1.2.0/validity/api/helpers.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.1.0/validity/api/serializers.py` & `netbox-validity-1.2.0/validity/api/serializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,15 @@
             "type_filter",
             "platform_filter",
             "status_filter",
             "location_filter",
             "site_filter",
             "tenant_filter",
             "dynamic_pairs",
+            "dp_tag_prefix",
             "tags",
             "custom_fields",
             "created",
             "last_updated",
         )
```

### Comparing `netbox-validity-1.1.0/validity/api/urls.py` & `netbox-validity-1.2.0/validity/api/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.1.0/validity/api/views.py` & `netbox-validity-1.2.0/validity/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.1.0/validity/choices.py` & `netbox-validity-1.2.0/validity/choices.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     OR = "OR", _("OR"), "purple"
     AND = "AND", _("AND"), "blue"
 
 
 class DynamicPairsChoices(TextChoices, metaclass=ColoredChoiceMeta):
     NO = "NO", _("NO"), "red"
     NAME = "NAME", _("By name"), "blue"
+    TAG = "TAG", _("By tag"), "purple"
 
 
 class SeverityChoices(TextChoices, metaclass=ColoredChoiceMeta):
     LOW = "LOW", _("LOW"), "green"
     MIDDLE = "MIDDLE", _("MIDDLE"), "yellow"
     HIGH = "HIGH", _("HIGH"), "red"
```

### Comparing `netbox-validity-1.1.0/validity/config_compliance/device_config/base.py` & `netbox-validity-1.2.0/validity/config_compliance/device_config/base.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.1.0/validity/config_compliance/device_config/routeros.py` & `netbox-validity-1.2.0/validity/config_compliance/device_config/routeros.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.1.0/validity/config_compliance/device_config/ttp.py` & `netbox-validity-1.2.0/validity/config_compliance/device_config/ttp.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.1.0/validity/config_compliance/device_config/yaml.py` & `netbox-validity-1.2.0/validity/config_compliance/device_config/yaml.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.1.0/validity/config_compliance/dynamic_pairs.py` & `netbox-validity-1.2.0/validity/config_compliance/dynamic_pairs.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 
 class NoneFilter(DynamicPairFilter):
     @property
     def filter(self) -> None:
         return
 
 
-@dataclass
-class DynamicNamePairFilter(DynamicPairFilter):
+class DynamicPairNameFilter(DynamicPairFilter):
     @staticmethod
     def extract_first_group(regex: str) -> str | None:
         open_bracket_index = -1
         open_square_brackets = 0
         for i, char in enumerate(regex):
             if char in "[]" and (i == 0 or regex[i - 1] != "\\"):
                 open_square_brackets += 1 if char == "[" else -1
@@ -63,13 +62,23 @@
         if not (name_match := re.search(self.selector.name_filter, self.device.name)):
             return
         start, end = name_match.start(1), name_match.end(1)
         filter_string = self.device.name[:start] + group1 + self.device.name[end:]
         return Q(name__regex=filter_string)
 
 
-dynamic_pair_filters = {DynamicPairsChoices.NAME: DynamicNamePairFilter}
+class DynamicPairTagFilter(DynamicPairFilter):
+    @property
+    def filter(self) -> Q | None:
+        tags = self.device.tags.filter(slug__startswith=self.selector.dp_tag_prefix)
+        return Q(tags__in=tags)
+
+
+dynamic_pair_filters = {
+    DynamicPairsChoices.NAME: DynamicPairNameFilter,
+    DynamicPairsChoices.TAG: DynamicPairTagFilter,
+}
 
 
 def dpf_factory(selector: "ComplianceSelector", device: Device) -> DynamicPairFilter:
     filter_cls = dynamic_pair_filters.get(selector.dynamic_pairs, NoneFilter)
     return filter_cls(selector, device)
```

### Comparing `netbox-validity-1.1.0/validity/config_compliance/eval/default_nameset.py` & `netbox-validity-1.2.0/validity/config_compliance/eval/default_nameset.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.1.0/validity/config_compliance/eval/eval.py` & `netbox-validity-1.2.0/validity/config_compliance/eval/eval.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.1.0/validity/config_compliance/eval/eval_defaults.py` & `netbox-validity-1.2.0/validity/config_compliance/eval/eval_defaults.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.1.0/validity/filtersets.py` & `netbox-validity-1.2.0/validity/filtersets.py`

 * *Files 3% similar despite different names*

```diff
@@ -100,7 +100,13 @@
 class NameSetFilterSet(SearchMixin, NetBoxModelFilterSet):
     repo_id = ModelMultipleChoiceFilter(field_name="repo", queryset=models.GitRepo.objects.all())
 
     class Meta:
         model = models.NameSet
         fields = ("id", "name", "_global", "repo_id", "file_path")
         search_fields = ("name", "description", "definitions")
+
+    @classmethod
+    def get_filters(cls):
+        filters = super().get_filters()
+        filters["global"] = filters.pop("_global")
+        return filters
```

### Comparing `netbox-validity-1.1.0/validity/forms/filterset.py` & `netbox-validity-1.2.0/validity/forms/filterset.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.1.0/validity/forms/general.py` & `netbox-validity-1.2.0/validity/forms/general.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,36 +32,58 @@
         queryset=DeviceType.objects.all(), required=False, label=_("Device Type Filter")
     )
     platform_filter = DynamicModelMultipleChoiceField(queryset=Platform.objects.all(), required=False)
     location_filter = DynamicModelMultipleChoiceField(queryset=Location.objects.all(), required=False)
     site_filter = DynamicModelMultipleChoiceField(queryset=Site.objects.all(), required=False)
     tenant_filter = DynamicModelMultipleChoiceField(queryset=Tenant.objects.all(), required=False)
 
+    fieldsets = (
+        (_("Common"), ("name", "tags")),
+        (_("Dynamic Pairs"), ("dynamic_pairs", "dp_tag_prefix")),
+        (
+            _("Filters"),
+            (
+                "filter_operation",
+                "name_filter",
+                "type_filter",
+                "location_filter",
+                "manufacturer_filter",
+                "platform_filter",
+                "site_filter",
+                "status_filter",
+                "tag_filter",
+                "tenant_filter",
+            ),
+        ),
+    )
+
     class Meta:
         model = models.ComplianceSelector
         fields = (
             "name",
             "filter_operation",
             "dynamic_pairs",
+            "dp_tag_prefix",
             "name_filter",
             "tag_filter",
             "manufacturer_filter",
             "type_filter",
             "platform_filter",
             "status_filter",
             "location_filter",
             "site_filter",
             "tenant_filter",
             "tags",
         )
 
     def clean(self):
-        super().clean()
+        result = super().clean()
         if not self.cleaned_data.keys() & models.ComplianceSelector.filters.keys():
             raise ValidationError(_("You must specify at least one filter"))
+        return result
 
 
 class GitRepoForm(NetBoxModelForm):
     password = CharField(widget=PasswordInput(), required=False)
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
```

### Comparing `netbox-validity-1.1.0/validity/forms/helpers.py` & `netbox-validity-1.2.0/validity/forms/helpers.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.1.0/validity/management/commands/linkscripts.py` & `netbox-validity-1.2.0/validity/management/commands/linkscripts.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.1.0/validity/managers.py` & `netbox-validity-1.2.0/validity/managers.py`

 * *Files 11% similar despite different names*

```diff
@@ -119,14 +119,34 @@
 
 
 def annotate_json(qs: _QS, field: str, annotate_model: type["BaseModel"]) -> _QS:
     return qs.annotate(**{f"json_{field}": annotate_model.objects.filter(pk=OuterRef(f"{field}_id")).as_json()})
 
 
 class VDeviceQS(RestrictedQuerySet):
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
+        self.selector = None
+
+    def _clone(self, *args, **kwargs):
+        c = super()._clone(*args, **kwargs)
+        c.selector = self.selector
+        return c
+
+    def set_selector(self, selector):
+        self.selector = selector
+        return self
+
+    def _fetch_all(self):
+        super()._fetch_all()
+        if self.selector:
+            for item in self._result_cache:
+                if isinstance(item, self.model):
+                    item.selector = self.selector
+
     def annotate_git_repo_id(self: _QS) -> _QS:
         from validity.models import GitRepo
 
         return self.annotate(
             bound_repo=Cast(KeyTextTransform("repo", "tenant__custom_field_data"), BigIntegerField())
         ).annotate(
             repo_id=Case(
```

### Comparing `netbox-validity-1.1.0/validity/migrations/0001_initial.py` & `netbox-validity-1.2.0/validity/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.1.0/validity/migrations/0002_custom_fields.py` & `netbox-validity-1.2.0/validity/migrations/0002_custom_fields.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.1.0/validity/models/base.py` & `netbox-validity-1.2.0/validity/models/base.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.1.0/validity/models/device.py` & `netbox-validity-1.2.0/validity/models/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,8 +79,8 @@
         You have to set .selector before calling this method
         """
         if self.selector is None:
             return
         filter_ = self.selector.dynamic_pair_filter(self)
         if filter_ is None:
             return
-        return type(self).objects.filter(filter_).exclude(pk=self.pk).first()
+        return type(self).objects.filter(filter_).first()
```

### Comparing `netbox-validity-1.1.0/validity/models/nameset.py` & `netbox-validity-1.2.0/validity/models/nameset.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.1.0/validity/models/repo.py` & `netbox-validity-1.2.0/validity/models/repo.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,15 @@
                 raise ValidationError({"default": _("Default Repository already exists")})
 
     def save(self, **kwargs) -> None:
         if not self.name:
             self.name = self.git_url.split("://")[-1]
         return super().save(**kwargs)
 
+    @property
     def bound_devices(self) -> models.QuerySet[Device]:
         from .device import VDevice
 
         return (
             VDevice.objects.annotate_git_repo_id()
             .filter(repo_id=self.pk)
             .select_related("site", "device_role", "device_type__manufacturer")
```

### Comparing `netbox-validity-1.1.0/validity/models/selector.py` & `netbox-validity-1.2.0/validity/models/selector.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 from django.core.exceptions import ValidationError
 from django.db import models
 from django.utils.translation import gettext_lazy as _
 from extras.models import Tag
 from tenancy.models import Tenant
 
 from validity.choices import BoolOperationChoices, DynamicPairsChoices
-from validity.config_compliance.dynamic_pairs import DynamicNamePairFilter, dpf_factory
+from validity.config_compliance.dynamic_pairs import DynamicPairNameFilter, dpf_factory
+from validity.utils.misc import reraise
 from .base import BaseModel
 from .device import VDevice
 
 
 class ComplianceSelector(BaseModel):
     name = models.CharField(_("Selector Name"), max_length=255, unique=True)
     filter_operation = models.CharField(
@@ -35,14 +36,15 @@
     status_filter = models.CharField(max_length=50, choices=DeviceStatusChoices, blank=True)
     location_filter = models.ManyToManyField(Location, verbose_name=_("Location Filter"), blank=True, related_name="+")
     site_filter = models.ManyToManyField(Site, verbose_name=_("Site Filter"), blank=True, related_name="+")
     tenant_filter = models.ManyToManyField(Tenant, verbose_name=_("Tenant Filter"), blank=True, related_name="+")
     dynamic_pairs = models.CharField(
         _("Dynamic Pairs"), max_length=20, choices=DynamicPairsChoices.choices, default="NO"
     )
+    dp_tag_prefix = models.CharField(_("Dynamic Pair Tag Prefix"), max_length=255, blank=True)
 
     clone_fields = (
         "filter_operation",
         "name_filter",
         "tag_filter",
         "manufacturer_filter",
         "type_filter",
@@ -69,21 +71,25 @@
     class Meta:
         ordering = ("name",)
 
     def __str__(self) -> str:
         return self.name
 
     def clean(self):
-        try:
+        with reraise(re.error, ValidationError, {"name_filter": _("Invalid regular expression")}):
             re.compile(self.name_filter)
-        except re.error:
-            raise ValidationError({"name_filter": "Invalid regular expression"})
         if self.dynamic_pairs == DynamicPairsChoices.NAME:
-            if not DynamicNamePairFilter.extract_first_group(self.name_filter):
-                raise ValidationError({"name_filter": "You must define regexp group if dynamic_pairs is set to NAME"})
+            if not DynamicPairNameFilter.extract_first_group(self.name_filter):
+                raise ValidationError(
+                    {"name_filter": _("You must define regexp group if dynamic_pairs is set to NAME")}
+                )
+        elif self.dynamic_pairs == DynamicPairsChoices.TAG and not self.dp_tag_prefix:
+            raise ValidationError({"dp_tag_prefix": _("You must define Tag Prefix if dynamic_pairs is set to TAG")})
+        if self.dp_tag_prefix and self.dynamic_pairs != DynamicPairsChoices.TAG:
+            raise ValidationError({"dp_tag_prefix": _("This field may be used only if dynamic_pairs is set to TAG")})
 
     def get_filter_operation_color(self):
         return BoolOperationChoices.colors.get(self.filter_operation)
 
     def get_status_filter_color(self):
         return DeviceStatusChoices.colors.get(self.status_filter)
 
@@ -103,12 +109,12 @@
     @property
     def filter(self) -> models.Q:
         op = operator.or_ if self.filter_operation == BoolOperationChoices.OR else operator.and_
         return reduce(op, self.q_objects(), models.Q())
 
     @property
     def devices(self) -> models.QuerySet:
-        return VDevice.objects.filter(self.filter)
+        return VDevice.objects.filter(self.filter).set_selector(self)
 
     def dynamic_pair_filter(self, device: Device) -> models.Q | None:
         if dp_filter := dpf_factory(self, device).filter:
-            return self.filter & dp_filter & ~models.Q(pk=device.pk)
+            return dp_filter & ~models.Q(pk=device.pk)
```

### Comparing `netbox-validity-1.1.0/validity/models/serializer.py` & `netbox-validity-1.2.0/validity/models/serializer.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         if self.extraction_method != "TTP" and self.ttp_template:
             raise ValidationError({"ttp_template": _("TTP Template must be empty if extraction method is not TTP")})
         if self.extraction_method != "TTP" and (self.repo or self.file_path):
             raise ValidationError(_("Git properties may be set only if extraction method is TTP"))
         if self.extraction_method == "TTP" and not (self.ttp_template or self.repo):
             raise ValidationError(_("TTP Template must be defined if extraction method is TTP"))
 
+    @property
     def bound_devices(self) -> models.QuerySet[Device]:
         from .device import VDevice
 
         return (
             VDevice.objects.annotate_serializer_id()
             .filter(serializer_id=self.pk)
             .select_related("site", "device_role", "device_type__manufacturer")
```

### Comparing `netbox-validity-1.1.0/validity/models/test.py` & `netbox-validity-1.2.0/validity/models/test.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.1.0/validity/models/test_result.py` & `netbox-validity-1.2.0/validity/models/test_result.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.1.0/validity/navigation.py` & `netbox-validity-1.2.0/validity/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.1.0/validity/scripts/git.py` & `netbox-validity-1.2.0/validity/scripts/git.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.1.0/validity/scripts/run_tests.py` & `netbox-validity-1.2.0/validity/scripts/run_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,14 @@
         device_ids: list[int],
     ) -> Generator[ComplianceTestResult, None, None]:
         qs = selector.devices.select_related().annotate_json_serializer().annotate_json_repo()
         if device_ids:
             qs = qs.filter(pk__in=device_ids)
         for device in qs:
             try:
-                device.selector = selector
                 yield from self.run_tests_for_device(selector.tests.all(), device, report)
             except DeviceConfigError as e:
                 self.log_failure(f"`{e}`, ignoring all tests for *{device}*")
                 continue
 
     def fire_report_webhook(self, report_id: int) -> None:
         report = ComplianceReport.objects.filter(pk=report_id).annotate_result_stats().count_devices_and_tests().first()
```

### Comparing `netbox-validity-1.1.0/validity/tables.py` & `netbox-validity-1.2.0/validity/tables.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,19 @@
+from functools import partial
+
+from dcim.models import Device
+from dcim.tables import DeviceTable
 from django.urls import reverse
 from django.utils.html import format_html
 from django.utils.safestring import mark_safe
 from django.utils.translation import gettext_lazy as _
-from django_tables2 import Column, Table
+from django_tables2 import Column, RequestConfig, Table
 from netbox.tables import BooleanColumn as BooleanColumn
 from netbox.tables import ChoiceFieldColumn, ManyToManyColumn, NetBoxTable
+from utilities.paginator import EnhancedPaginator
 
 from validity import models
 from validity.utils.misc import colorful_percentage
 
 
 class SelectorTable(NetBoxTable):
     name = Column(linkify=True)
@@ -172,7 +177,37 @@
         return self._render_stats("low", record)
 
     def render_middle_stats(self, record):
         return self._render_stats("middle", record)
 
     def render_high_stats(self, record):
         return self._render_stats("high", record)
+
+
+class DynamicPairsTable(DeviceTable):
+    dynamic_pair = Column(verbose_name="Dynamic Pair", linkify=True)
+
+    class Meta(DeviceTable.Meta):
+        model = Device
+        fields = DeviceTable.Meta.fields + ("dynamic_pair",)
+        default_columns = DeviceTable.Meta.default_columns + ("dynamic_pair",)
+
+    def get_paginate_by(self, request, max_paginate_by) -> int:
+        try:
+            per_page = int(request.GET["per_page"])
+            if per_page > max_paginate_by:
+                per_page = max_paginate_by
+            return per_page
+        except (KeyError, ValueError):
+            return max_paginate_by // 2
+
+    def configure(self, request, max_paginate_by=None, orphans=None):
+        def get_page_lengths(self):
+            return (max_paginate_by // 2, max_paginate_by)
+
+        super().configure(request)
+        if max_paginate_by and orphans:
+            paginator_class = type("CustomPaginator", (EnhancedPaginator,), {"get_page_lengths": get_page_lengths})
+            paginator_class = partial(paginator_class, orphans=orphans)
+            paginate_by = self.get_paginate_by(request, max_paginate_by)
+            paginate = {"paginator_class": paginator_class, "per_page": paginate_by}
+            RequestConfig(request, paginate).configure(self)
```

### Comparing `netbox-validity-1.1.0/validity/templates/validity/compliance_results.html` & `netbox-validity-1.2.0/validity/templates/validity/compliance_results.html`

 * *Files 8% similar despite different names*

```diff
@@ -33,12 +33,12 @@
     </form>
   </div>
 </div>
 <div class="card mb-3">
   <div class="card-body">
     <h5 class="card-title mb-2">All Results related to {{ object }}</h5>
     <div class="table-responsive">
-      {% render_table table %}
+      {% render_table table 'inc/table.html' %}
     </div>
     {%include 'inc/paginator.html' with paginator=table.paginator page=table.page%}
   </div>
   {% endblock %}
```

### Comparing `netbox-validity-1.1.0/validity/templates/validity/compliancereport.html` & `netbox-validity-1.2.0/validity/templates/validity/compliancereport.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.1.0/validity/templates/validity/complianceselector.html` & `netbox-validity-1.2.0/validity/templates/validity/complianceselector.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,81 +1,95 @@
 {% extends 'generic/object.html' %}
 {% load helpers %}
 {% load validity %}
 {% load render_table from django_tables2 %}
 {% block content %}
   <div class="row mb-3">
-    <div class="col col-md-6">
+    <div class="col col-md-5">
       <div class="card">
         <h5 class="card-header">Compliance Selector</h5>
         <div class="card-body">
           <table class="table table-hover attr-table">
             <tr>
               <th scope="row">Name</th>
               <td>{{ object.name }}</td>
             </tr>
             <tr>
+              <th scope="row">Dynamic Pairs</th>
+              <td><code>{{ object | colored_choice:"dynamic_pairs" }}</code></td>
+            </tr>
+            <tr>
+              <th scope="row">Dynamic Pair Tag Prefix</th>
+              <td><code>{{ object.dp_tag_prefix | placeholder }}</code></td>
+            </tr>
+          </table>
+        </div>
+      </div>
+      {% include 'inc/panels/tags.html' %}
+    </div>
+    <div class="col col-md-7">
+      <div class="card">
+        <h5 class="card-header">Filters</h5>
+        <div class="card-body">
+          <table class="table table-hover attr-table">
+            <tr>
               <th scope="row">Multi-filter operation</th>
               <td>{{ object | colored_choice:"filter_operation" }}</td>
             </tr>
             <tr>
               <th scope="row">Device Name Filter</th>
               <td><code>{{ object.name_filter | placeholder }}</code></td>
             </tr>
             <tr>
-              <th scope="row">Tag Filter</th>
-              <td><code>{{ object.tag_filter.all | linkify_list }}</code></td>
+              <th scope="row">Device Type Filter</th>
+              <td><code>{{ object.type_filter.all | linkify_list }}</code></td>
             </tr>
             <tr>
-              <th scope="row">Manufacturer Filter</th>
-              <td><code>{{ object.manufacturer_filter.all | linkify_list }}</code></td>
+              <th scope="row">Location Filter</th>
+              <td><code>{{ object.location_filter.all | linkify_list }}</code></td>
             </tr>
             <tr>
-              <th scope="row">Device Type Filter</th>
-              <td><code>{{ object.type_filter.all | linkify_list }}</code></td>
+              <th scope="row">Manufacturer Filter</th>
+              <td><code>{{ object.manufacturer_filter.all | linkify_list }}</code></td>
             </tr>
             <tr>
               <th scope="row">Platform Filter</th>
               <td><code>{{ object.platform_filter.all | linkify_list }}</code></td>
             </tr>
             <tr>
-              <th scope="row">Status Filter</th>
-              <td><code>{{ object | colored_choice:"status_filter" | placeholder }}</code></td>
+              <th scope="row">Site Filter</th>
+              <td><code>{{ object.site_filter.all | linkify_list }}</code></td>
             </tr>
             <tr>
-              <th scope="row">Location Filter</th>
-              <td><code>{{ object.location_filter.all | linkify_list }}</code></td>
+              <th scope="row">Status Filter</th>
+              <td><code>{{ object | colored_choice:"status_filter" | placeholder }}</code></td>
             </tr>
             <tr>
-              <th scope="row">Site Filter</th>
-              <td><code>{{ object.site_filter.all | linkify_list }}</code></td>
+              <th scope="row">Tag Filter</th>
+              <td><code>{{ object.tag_filter.all | linkify_list }}</code></td>
             </tr>
             <tr>
               <th scope="row">Tenant Filter</th>
               <td><code>{{ object.tenant_filter.all | linkify_list }}</code></td>
             </tr>
-            <tr>
-              <th scope="row">Dynamic Pairs</th>
-              <td><code>{{ object | colored_choice:"dynamic_pairs" }}</code></td>
-            </tr>
           </table>
         </div>
       </div>
     </div>
-    <div class="col col-md-6">
-      {% include 'inc/panels/tags.html' %}
-    </div>
   </div>
   <div class="row">
     <div class="col col-md-12">
       <div class="card">
         <h5 class="card-header">Selected Devices</h5>
         <div class="card-body">
+          <div class="pt-0 mb-3 col col-md-3">
+            {% include 'validity/inc/search_form.html' with model='Device' %}
+          </div>
           <div class="table-responsive">
-            {% render_table device_table %}
+            {% render_table table 'inc/table.html' %}
           </div>
-          {%include 'inc/paginator.html' with paginator=device_table.paginator page=device_table.page%}
+          {%include 'inc/paginator.html' with paginator=table.paginator page=table.page%}
         </div>
       </div>
     </div>
   </div>
 {% endblock content %}
```

#### html2text {}

```diff
@@ -1,22 +1,24 @@
 {% extends 'generic/object.html' %} {% load helpers %} {% load validity %} {%
 load render_table from django_tables2 %} {% block content %}
 ** Compliance Selector **
-Name                   {{ object.name }}
+Name                    {{ object.name }}
+Dynamic Pairs           {{ object | colored_choice:"dynamic_pairs" }}
+Dynamic Pair Tag Prefix {{ object.dp_tag_prefix | placeholder }}
+{% include 'inc/panels/tags.html' %}
+** Filters **
 Multi-filter operation {{ object | colored_choice:"filter_operation" }}
 Device Name Filter     {{ object.name_filter | placeholder }}
-Tag Filter             {{ object.tag_filter.all | linkify_list }}
-Manufacturer Filter    {{ object.manufacturer_filter.all | linkify_list }}
 Device Type Filter     {{ object.type_filter.all | linkify_list }}
+Location Filter        {{ object.location_filter.all | linkify_list }}
+Manufacturer Filter    {{ object.manufacturer_filter.all | linkify_list }}
 Platform Filter        {{ object.platform_filter.all | linkify_list }}
+Site Filter            {{ object.site_filter.all | linkify_list }}
 Status Filter          {{ object | colored_choice:"status_filter" | placeholder
                        }}
-Location Filter        {{ object.location_filter.all | linkify_list }}
-Site Filter            {{ object.site_filter.all | linkify_list }}
+Tag Filter             {{ object.tag_filter.all | linkify_list }}
 Tenant Filter          {{ object.tenant_filter.all | linkify_list }}
-Dynamic Pairs          {{ object | colored_choice:"dynamic_pairs" }}
-{% include 'inc/panels/tags.html' %}
 ** Selected Devices **
-{% render_table device_table %}
-{%include 'inc/paginator.html' with paginator=device_table.paginator
-page=device_table.page%}
+{% include 'validity/inc/search_form.html' with model='Device' %}
+{% render_table table 'inc/table.html' %}
+{%include 'inc/paginator.html' with paginator=table.paginator page=table.page%}
 {% endblock content %}
```

### Comparing `netbox-validity-1.1.0/validity/templates/validity/compliancetest.html` & `netbox-validity-1.2.0/validity/templates/validity/compliancetest.html`

 * *Files 20% similar despite different names*

```diff
@@ -40,16 +40,19 @@
     </div>
   </div>
   <div class="row">
     <div class="col col-md-12">
       <div class="card">
         <h5 class="card-header">Bound Namesets</h5>
         <div class="card-body">
+          <div class="pt-0 mb-3 col col-md-3">
+            {% include 'validity/inc/search_form.html' with model='NameSet' %}
+          </div>
           <div class="table-responsive">
-            {% render_table nameset_table %}
+            {% render_table table 'inc/table.html' %}
           </div>
-          {%include 'inc/paginator.html' with paginator=nameset_table.paginator page=nameset_table.page%}
+          {%include 'inc/paginator.html' with paginator=table.paginator page=table.page%}
         </div>
       </div>
     </div>
   </div>
 {% endblock content %}
```

#### html2text {}

```diff
@@ -5,11 +5,11 @@
 Severity    {{ object | colored_choice:"severity" }}
 Selectors   {{ object.selectors.all | linkify_list }}
 Description {{ object.description }}
 {% include 'inc/panels/tags.html' %}
 ** Expression [source: {{ object | data_source }}] **
 {{ object.effective_expression }}
 ** Bound Namesets **
-{% render_table nameset_table %}
-{%include 'inc/paginator.html' with paginator=nameset_table.paginator
-page=nameset_table.page%}
+{% include 'validity/inc/search_form.html' with model='NameSet' %}
+{% render_table table 'inc/table.html' %}
+{%include 'inc/paginator.html' with paginator=table.paginator page=table.page%}
 {% endblock content %}
```

### Comparing `netbox-validity-1.1.0/validity/templates/validity/compliancetestresult.html` & `netbox-validity-1.2.0/validity/templates/validity/compliancetestresult.html`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
           <h5 class="card-header">Explanation</h5>
         </div>
         <div class="col d-flex align-items-center mb-0 pb-0 justify-content-end me-5">
           <a class="btn btn-sm btn-primary" href="?verbose=true">Verbose</a>
         </div>
       </div>
       <div class="card-body pt-0">
-        <div class="table-responsive">{% render_table explanation_table %}</div>
+        <div class="table-responsive">{% render_table explanation_table 'inc/table.html' %}</div>
       </div>
     </div>
   </div>
 </div>
 <div class="row">
   <div class="col col-md-12">
     <div class="card">
```

#### html2text {}

```diff
@@ -7,13 +7,13 @@
 Test Severity {{ object.test | colored_choice:"severity" }}
 Device        {{ object.device | linkify }}
 Dynamic Pair  {{ object.dynamic_pair | linkify | placeholder }}
 Result        {% if object.passed %} PASSED {% else %} FAILED {% endif %}
 Created       {{ object.created | date:"Y-m-d G:i:s" }}
 ** Explanation **
 Verbose
-{% render_table explanation_table %}
+{% render_table explanation_table 'inc/table.html' %}
 ** Other results for the same test and device **
 {% render_table result_table %}
 {%include 'inc/paginator.html' with paginator=result_table.paginator
 page=result_table.page%}
 {% endblock content %}
```

### Comparing `netbox-validity-1.1.0/validity/templates/validity/configserializer.html` & `netbox-validity-1.2.0/validity/templates/validity/configserializer.html`

 * *Files 21% similar despite different names*

```diff
@@ -36,16 +36,19 @@
     </div>
   </div>
   <div class="row">
     <div class="col col-md-12">
       <div class="card">
         <h5 class="card-header">Bound Devices</h5>
         <div class="card-body">
+          <div class="pt-0 mb-3 col col-md-3">
+            {% include 'validity/inc/search_form.html' with model='Device' %}
+          </div>
           <div class="table-responsive">
-            {% render_table device_table %}
+            {% render_table table 'inc/table.html' %}
           </div>
-          {%include 'inc/paginator.html' with paginator=device_table.paginator page=device_table.page%}
+          {%include 'inc/paginator.html' with paginator=table.paginator page=table.page%}
         </div>
       </div>
     </div>
   </div>
 {% endblock content %}
```

#### html2text {}

```diff
@@ -3,11 +3,11 @@
 ** Config Serializer **
 Name                     {{ object.name }}
 Config Extraction Method {{ object | colored_choice:"extraction_method" }}
 {% include 'inc/panels/tags.html' %}
 ** TTP Template [Source: {{ object | data_source }}] **
 {{ object.effective_template }}
 ** Bound Devices **
-{% render_table device_table %}
-{%include 'inc/paginator.html' with paginator=device_table.paginator
-page=device_table.page%}
+{% include 'validity/inc/search_form.html' with model='Device' %}
+{% render_table table 'inc/table.html' %}
+{%include 'inc/paginator.html' with paginator=table.paginator page=table.page%}
 {% endblock content %}
```

### Comparing `netbox-validity-1.1.0/validity/templates/validity/device_config.html` & `netbox-validity-1.2.0/validity/templates/validity/device_config.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.1.0/validity/templates/validity/gitrepo.html` & `netbox-validity-1.2.0/validity/templates/validity/gitrepo.html`

 * *Files 19% similar despite different names*

```diff
@@ -62,16 +62,19 @@
     </div>
   </div>
   <div class="row">
     <div class="col col-md-12">
       <div class="card">
         <h5 class="card-header">Bound Devices</h5>
         <div class="card-body">
+          <div class="pt-0 mb-3 col col-md-3">
+            {% include 'validity/inc/search_form.html' with model='Device' %}
+          </div>
           <div class="table-responsive">
-            {% render_table device_table %}
+            {% render_table table 'inc/table.html' %}
           </div>
-          {%include 'inc/paginator.html' with paginator=device_table.paginator page=device_table.page%}
+          {%include 'inc/paginator.html' with paginator=table.paginator page=table.page%}
         </div>
       </div>
     </div>
   </div>
 {% endblock content %}
```

#### html2text {}

```diff
@@ -11,11 +11,11 @@
 Web URL            {{ object.web_url | placeholder }}
 Username           {{ object.username | placeholder }}
 Password           {% if object.encrypted_password %}$encrypted{% else %}{{ ''
                    | placeholder }}{% endif %}
 Branch             {{ object.branch | placeholder }}
 {% include 'inc/panels/tags.html' %}
 ** Bound Devices **
-{% render_table device_table %}
-{%include 'inc/paginator.html' with paginator=device_table.paginator
-page=device_table.page%}
+{% include 'validity/inc/search_form.html' with model='Device' %}
+{% render_table table 'inc/table.html' %}
+{%include 'inc/paginator.html' with paginator=table.paginator page=table.page%}
 {% endblock content %}
```

### Comparing `netbox-validity-1.1.0/validity/templates/validity/nameset.html` & `netbox-validity-1.2.0/validity/templates/validity/nameset.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 {% extends 'generic/object.html' %}
 {% load validity %}
 {% load helpers %}
-{% load render_table from django_tables2 %}
 {% block content %}
   <div class="row">
     <div class="col col-md-4">
       <div class="card mb-3">
         <h5 class="card-header">Compliance Test</h5>
         <div class="card-body">
           <table class="table table-hover attr-table">
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 {% extends 'generic/object.html' %} {% load validity %} {% load helpers %} {%
-load render_table from django_tables2 %} {% block content %}
+block content %}
 ** Compliance Test **
 Name        {{ object.name }}
 Description {{ object.description | placeholder}}
 Global      {{ global | checkmark }}
 Bound Tests {{ object.tests.all | linkify_list }}
 {% include 'inc/panels/tags.html' %}
 ** Definitions [source: {{ object | data_source }}] **
```

### Comparing `netbox-validity-1.1.0/validity/templatetags/validity.py` & `netbox-validity-1.2.0/validity/templatetags/validity.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.1.0/validity/tests/base.py` & `netbox-validity-1.2.0/validity/tests/base.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.1.0/validity/tests/conftest.py` & `netbox-validity-1.2.0/validity/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import shutil
 from pathlib import Path
 
 import pytest
 from dcim.models import Device, DeviceType, Manufacturer
 from django.contrib.contenttypes.models import ContentType
 from extras.models import CustomField
+from graphene_django.utils.testing import graphql_query
 from tenancy.models import Tenant
 
 import validity
 from validity.models import ConfigSerializer, GitRepo
 
 
 pytest.register_assert_rewrite("base")
@@ -78,7 +79,15 @@
         [
             ContentType.objects.get_for_model(Device),
             ContentType.objects.get_for_model(DeviceType),
             ContentType.objects.get_for_model(Manufacturer),
         ]
     )
     cfs[1].content_types.set([ContentType.objects.get_for_model(Tenant)])
+
+
+@pytest.fixture
+def gql_query(admin_client):
+    def func(*args, **kwargs):
+        return graphql_query(*args, **kwargs, client=admin_client, graphql_url="/graphql/")
+
+    return func
```

### Comparing `netbox-validity-1.1.0/validity/tests/factories.py` & `netbox-validity-1.2.0/validity/tests/factories.py`

 * *Files 12% similar despite different names*

```diff
@@ -85,14 +85,28 @@
         model = models.ComplianceTest
 
 
 class ReportFactory(DjangoModelFactory):
     class Meta:
         model = models.ComplianceReport
 
+    @factory.post_generation
+    def passed_results(self, create, extracted, **kwargs):
+        if not create or not extracted:
+            return
+        for _ in range(extracted):
+            CompTestResultFactory(report=self, passed=True)
+
+    @factory.post_generation
+    def failed_results(self, create, extracted, **kwargs):
+        if not create or not extracted:
+            return
+        for _ in range(extracted):
+            CompTestResultFactory(report=self, passed=False)
+
 
 class ManufacturerFactory(DjangoModelFactory):
     name = factory.Sequence(lambda n: f"manufacturer-{n}")
     slug = factory.Sequence(lambda n: f"manufacturer-{n}")
 
     class Meta:
         model = Manufacturer
```

### Comparing `netbox-validity-1.1.0/validity/tests/test_api.py` & `netbox-validity-1.2.0/validity/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.1.0/validity/tests/test_config_compliance/test_device_config.py` & `netbox-validity-1.2.0/validity/tests/test_config_compliance/test_device_config.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.1.0/validity/tests/test_config_compliance/test_dynamic_pairs.py` & `netbox-validity-1.2.0/validity/tests/test_config_compliance/test_dynamic_pairs.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,30 @@
 from unittest.mock import Mock
 
 import pytest
 from django.db.models import Q
-from factories import DeviceFactory, SelectorFactory
+from extras.models import Tag
+from factories import DeviceFactory, SelectorFactory, TagFactory
 
-from validity.config_compliance.dynamic_pairs import DynamicNamePairFilter, NoneFilter, dpf_factory
+from validity.config_compliance.dynamic_pairs import (
+    DynamicPairNameFilter,
+    DynamicPairTagFilter,
+    NoneFilter,
+    dpf_factory,
+)
 
 
-@pytest.mark.parametrize("dynamic_pairs, filter_cls", [("NAME", DynamicNamePairFilter), ("NO", NoneFilter)])
+@pytest.mark.parametrize(
+    "dynamic_pairs, filter_cls",
+    [
+        ("NAME", DynamicPairNameFilter),
+        ("NO", NoneFilter),
+        ("TAG", DynamicPairTagFilter),
+    ],
+)
 def test_dpf_factory(dynamic_pairs, filter_cls):
     selector = Mock(dynamic_pairs=dynamic_pairs)
     obj = dpf_factory(selector=selector, device=Mock())
     assert type(obj) == filter_cls
 
 
 @pytest.mark.parametrize(
@@ -26,12 +39,26 @@
         pytest.param("sw[0-9]+-([12])-([a-z]+)", "sw01-1-paris", "sw01-([12])-paris", id="sw01-([12])-paris"),
     ],
 )
 @pytest.mark.django_db
 def test_name_filter(name_filter, device_name, dp_filter):
     device = DeviceFactory(name=device_name)
     selector = SelectorFactory(name_filter=name_filter)
-    filter_ = DynamicNamePairFilter(selector, device)
+    filter_ = DynamicPairNameFilter(selector, device)
     if dp_filter:
         assert filter_.filter == Q(name__regex=dp_filter)
     else:
         assert filter_.filter is None
+
+
+@pytest.mark.django_db
+def test_tag_filter():
+    tags = [
+        TagFactory(name="tag-1_", slug="tag-1"),
+        TagFactory(name="tag-2_", slug="tag-2"),
+        TagFactory(name="sometag_", slug="sometag"),
+    ]
+    selector = SelectorFactory(dp_tag_prefix="tag-", name_filter=".*")
+    device = DeviceFactory()
+    device.tags.set([tags[0], tags[2]])
+    filter_ = DynamicPairTagFilter(selector, device).filter
+    assert repr(filter_) == repr(Q(tags__in=Tag.objects.filter(slug="tag-1")))
```

### Comparing `netbox-validity-1.1.0/validity/tests/test_config_compliance/test_eval.py` & `netbox-validity-1.2.0/validity/tests/test_config_compliance/test_eval.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.1.0/validity/tests/test_models/test_clean.py` & `netbox-validity-1.2.0/validity/tests/test_models/test_clean.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.1.0/validity/tests/test_models/test_git_link.py` & `netbox-validity-1.2.0/validity/tests/test_models/test_git_link.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.1.0/validity/tests/test_models/test_git_repo.py` & `netbox-validity-1.2.0/validity/tests/test_models/test_git_repo.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.1.0/validity/tests/test_models/test_selector.py` & `netbox-validity-1.2.0/validity/tests/test_models/test_selector.py`

 * *Files 15% similar despite different names*

```diff
@@ -57,23 +57,22 @@
         str(model.filter)
         == "(AND: ('name__regex', 'some_name'), (OR: ('site', <Site: site-0>), ('site', <Site: site-1>)))"
     )
 
 
 @pytest.mark.django_db
 def test_devices(monkeypatch):
-    monkeypatch.setattr(VDevice.objects, "filter", device_mock := Mock())
+    monkeypatch.setattr(VDevice.objects, "filter", filter_mock := Mock(name="filter"))
     monkeypatch.setattr(selector.ComplianceSelector, "filter", "filter_value")
     model = SelectorFactory()
-    model.devices
-    device_mock.assert_called_once_with("filter_value")
+    assert model.devices._extract_mock_name() == "filter().set_selector()"
+    filter_mock.assert_called_once_with("filter_value")
 
 
 @pytest.mark.django_db
 def test_dynamic_pairs(monkeypatch):
     monkeypatch.setattr(selector, "dpf_factory", dpf_mock := Mock(return_value=Mock(filter=Q(dpf_filter=True))))
-    monkeypatch.setattr(selector.ComplianceSelector, "filter", Q(s_filter=True))
     selector_instance = SelectorFactory()
     device = DeviceFactory()
     dp_filter = selector_instance.dynamic_pair_filter(device)
     dpf_mock.assert_called_once_with(selector_instance, device)
-    assert dp_filter == Q(s_filter=True) & Q(dpf_filter=True) & ~Q(pk=device.pk)
+    assert dp_filter == Q(dpf_filter=True) & ~Q(pk=device.pk)
```

### Comparing `netbox-validity-1.1.0/validity/tests/test_models/test_vdevice.py` & `netbox-validity-1.2.0/validity/tests/test_models/test_vdevice.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 from django.db import connection
-from factories import DeviceFactory, GitRepoFactory, SerializerDBFactory, TenantFactory
+from factories import DeviceFactory, GitRepoFactory, SelectorFactory, SerializerDBFactory, TenantFactory
 
 from validity.models import VDevice
 
 
 @pytest.fixture
 def setup_device_and_serializer(create_custom_fields):
     serializer = SerializerDBFactory()
@@ -67,7 +67,22 @@
 @pytest.mark.django_db
 def test_annotated_serializer(setup_device_and_serializer):
     device, serializer = setup_device_and_serializer
     vdevice = VDevice.objects.annotate_json_serializer().get(pk=device.pk)
     queries_count = len(connection.queries)
     assert vdevice.serializer == serializer
     assert len(connection.queries) == queries_count
+
+
+@pytest.mark.parametrize("qs", [VDevice.objects.all(), VDevice.objects.filter(name__in=["d1", "d2"])])
+@pytest.mark.django_db
+def test_set_selector(qs, subtests):
+    for name in ["d1", "d2", "d3"]:
+        DeviceFactory(name=name)
+    selector = SelectorFactory()
+    some_model = qs.first()
+    assert some_model.selector is None
+    qs = qs.set_selector(selector)
+    for i, queryset in enumerate([qs, qs.select_related(), qs.filter(name="d1")]):
+        with subtests.test(id=f"qs-{i}"):
+            for model in queryset:
+                assert model.selector == selector
```

### Comparing `netbox-validity-1.1.0/validity/tests/test_scripts/test_run_tests.py` & `netbox-validity-1.2.0/validity/tests/test_scripts/test_run_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,14 @@
         }
     )
     report = Mock()
     list(script.run_tests_for_selector(selector, report, []))
     assert script.run_tests_for_device.call_count == len(devices)
     script.run_tests_for_device.assert_any_call(selector.tests.all(), devices[0], report)
     script.run_tests_for_device.assert_any_call(selector.tests.all(), devices[1], report)
-    assert devices[0].selector == selector
 
 
 @pytest.mark.django_db
 def test_webhook_without_ctx_is_not_fired(monkeypatch):
     enq_obj = Mock()
     monkeypatch.setattr(run_tests, "enqueue_object", enq_obj)
     with null_request():
```

### Comparing `netbox-validity-1.1.0/validity/tests/test_utils/test_git.py` & `netbox-validity-1.2.0/validity/tests/test_utils/test_git.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.1.0/validity/tests/test_utils/test_misc.py` & `netbox-validity-1.2.0/validity/tests/test_utils/test_misc.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.1.0/validity/tests/test_views.py` & `netbox-validity-1.2.0/validity/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.1.0/validity/urls.py` & `netbox-validity-1.2.0/validity/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.1.0/validity/utils/git.py` & `netbox-validity-1.2.0/validity/utils/git.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.1.0/validity/utils/misc.py` & `netbox-validity-1.2.0/validity/utils/misc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from contextlib import contextmanager
+from typing import Any
 
 from django.utils.html import format_html
 from netbox.context import current_request
 
 
 def colorful_percentage(percent: float) -> str:
     levels = {75: "warning", 50: "orange", 25: "danger"}
@@ -22,18 +23,18 @@
     try:
         yield
     finally:
         current_request.set(ctx)
 
 
 @contextmanager
-def reraise(catch: type[Exception] | tuple[type[Exception], ...], raise_: type[Exception], msg: str | None = None):
+def reraise(catch: type[Exception] | tuple[type[Exception], ...], raise_: type[Exception], msg: Any = None):
     try:
         yield
     except raise_:
         raise
     except catch as e:
-        if msg:
+        if msg and isinstance(msg, str):
             msg = msg.format(str(e))
-        else:
+        if not msg:
             msg = str(e)
         raise raise_(msg) from e
```

### Comparing `netbox-validity-1.1.0/validity/utils/password.py` & `netbox-validity-1.2.0/validity/utils/password.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.1.0/validity/views/__init__.py` & `netbox-validity-1.2.0/validity/views/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.1.0/validity/views/device.py` & `netbox-validity-1.2.0/validity/views/device.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from dcim.models import Device
 from netbox.views import generic
 from utilities.views import ViewTab, register_model_view
 
 from validity.config_compliance.exceptions import DeviceConfigError
 from validity.models import VDevice
-from .test_result import TestResultBaseView
+from .base import TestResultBaseView
 
 
 logger = logging.getLogger(__name__)
 
 
 @register_model_view(Device, "results")
 class TestResultView(TestResultBaseView):
```

### Comparing `netbox-validity-1.1.0/validity/views/git_repo.py` & `netbox-validity-1.2.0/validity/views/git_repo.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,29 @@
+from dcim.filtersets import DeviceFilterSet
 from dcim.tables import DeviceTable
 from netbox.views import generic
 from utilities.views import register_model_view
 
 from validity import filtersets, forms, models, tables
+from .base import TableMixin
 
 
 class GitRepoListView(generic.ObjectListView):
     queryset = models.GitRepo.objects.all()
     table = tables.GitRepoTable
     filterset = filtersets.GitRepoFilterSet
     filterset_form = forms.GitRepoFilterForm
 
 
 @register_model_view(models.GitRepo)
-class GitRepoView(generic.ObjectView):
+class GitRepoView(TableMixin, generic.ObjectView):
     queryset = models.GitRepo.objects.prefetch_related("tags")
-
-    def get_extra_context(self, request, instance):
-        table = DeviceTable(instance.bound_devices())
-        table.configure(request)
-        return {"device_table": table}
+    table = DeviceTable
+    filterset = DeviceFilterSet
+    object_table_field = "bound_devices"
 
 
 @register_model_view(models.GitRepo, "delete")
 class GitRepoDeleteView(generic.ObjectDeleteView):
     queryset = models.GitRepo.objects.all()
```

### Comparing `netbox-validity-1.1.0/validity/views/nameset.py` & `netbox-validity-1.2.0/validity/views/nameset.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.1.0/validity/views/report.py` & `netbox-validity-1.2.0/validity/views/report.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, Iterable, Iterator
 
 from netbox.views import generic
 from utilities.views import register_model_view
 
 from validity import forms, models, tables
 from validity.choices import DeviceGroupByChoices
-from .test_result import TestResultBaseView
+from .base import TestResultBaseView
 
 
 class ComplianceReportListView(generic.ObjectListView):
     queryset = models.ComplianceReport.objects.annotate_result_stats().count_devices_and_tests().order_by("-created")
     table = tables.ComplianceReportTable
 
     def get_table(self, data, request, bulk_actions=True):
```

### Comparing `netbox-validity-1.1.0/validity/views/selector.py` & `netbox-validity-1.2.0/validity/views/selector.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,44 @@
-from dcim.tables import DeviceTable
+from dcim.filtersets import DeviceFilterSet
 from netbox.views import generic
 from utilities.views import register_model_view
 
 from validity import filtersets, forms, models, tables
+from .base import TableMixin
 
 
 class ComplianceSelectorListView(generic.ObjectListView):
     queryset = models.ComplianceSelector.objects.all()
     table = tables.SelectorTable
     filterset = filtersets.ComplianceSelectorFilterSet
     filterset_form = forms.ComplianceSelectorFilterForm
 
 
 @register_model_view(models.ComplianceSelector)
-class ComplianceSelectorView(generic.ObjectView):
+class ComplianceSelectorView(TableMixin, generic.ObjectView):
     queryset = models.ComplianceSelector.objects.prefetch_related(
         "tag_filter",
         "manufacturer_filter",
         "type_filter",
         "platform_filter",
         "location_filter",
         "site_filter",
         "tenant_filter",
         "tags",
     )
-
-    def get_extra_context(self, request, instance):
-        table = DeviceTable(instance.devices.all())
-        table.configure(request)
-        return {"device_table": table}
+    filterset = DeviceFilterSet
+    object_table_field = "devices"
+    table = tables.DynamicPairsTable
+    max_paginate_by = 10
+    page_orphans = 1
+
+    def configure_table(self, request, table, instance):
+        if instance.dynamic_pairs == "NO":
+            table.exclude += ("dynamic_pair",)
+        table.configure(request, max_paginate_by=self.max_paginate_by, orphans=self.page_orphans)
 
 
 @register_model_view(models.ComplianceSelector, "delete")
 class ComplianceSelectorDeleteView(generic.ObjectDeleteView):
     queryset = models.ComplianceSelector.objects.all()
```

### Comparing `netbox-validity-1.1.0/validity/views/serializer.py` & `netbox-validity-1.2.0/validity/views/serializer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,29 @@
+from dcim.filtersets import DeviceFilterSet
 from dcim.tables import DeviceTable
 from netbox.views import generic
 from utilities.views import register_model_view
 
 from validity import filtersets, forms, models, tables
+from .base import TableMixin
 
 
 class ConfigSerializerListView(generic.ObjectListView):
     queryset = models.ConfigSerializer.objects.all()
     table = tables.ConfigSerializerTable
     filterset = filtersets.ConfigSerializerFilterSet
     filterset_form = forms.ConfigSerializerFilterForm
 
 
 @register_model_view(models.ConfigSerializer)
-class ConfigSerializerView(generic.ObjectView):
+class ConfigSerializerView(TableMixin, generic.ObjectView):
     queryset = models.ConfigSerializer.objects.all()
-
-    def get_extra_context(self, request, instance):
-        table = DeviceTable(instance.bound_devices())
-        table.configure(request)
-        return {"device_table": table}
+    object_table_field = "bound_devices"
+    table = DeviceTable
+    filterset = DeviceFilterSet
 
 
 @register_model_view(models.ConfigSerializer, "delete")
 class ConfigSerializerDeleteView(generic.ObjectDeleteView):
     queryset = models.ConfigSerializer.objects.all()
```

### Comparing `netbox-validity-1.1.0/validity/views/test.py` & `netbox-validity-1.2.0/validity/views/test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 from django.db.models import Count, Q
 from netbox.views import generic
 from utilities.views import register_model_view
 
 from validity import filtersets, forms, models, tables
-from .test_result import TestResultBaseView
+from .base import TableMixin, TestResultBaseView
 
 
 class ComplianceTestListView(generic.ObjectListView):
     queryset = models.ComplianceTest.objects.annotate_latest_count()
     table = tables.ComplianceTestTable
     filterset = filtersets.ComplianceTestFilterSet
     filterset_form = forms.ComplianceTestFilterForm
 
 
 @register_model_view(models.ComplianceTest)
-class ComplianceTestView(generic.ObjectView):
+class ComplianceTestView(TableMixin, generic.ObjectView):
     queryset = models.ComplianceTest.objects.prefetch_related("namesets")
+    table = tables.NameSetTable
+    filterset = filtersets.NameSetFilterSet
 
-    def get_extra_context(self, request, instance):
-        global_namesets = models.NameSet.objects.filter(_global=True)
-        table = tables.NameSetTable(instance.namesets.all() | global_namesets)
-        table.configure(request)
-        return {"nameset_table": table}
+    def get_table_qs(self, request, instance):
+        return models.NameSet.objects.filter(Q(_global=True) | Q(tests__pk=instance.pk))
 
 
 @register_model_view(models.ComplianceTest, "results")
 class TestResultView(TestResultBaseView):
     parent_model = models.ComplianceTest
     result_relation = "test"
     exclude_form_fields = ("platform_id", "tenant_id", "device_role_id", "manufacturer_id", "report_id", "selector_id")
```

### Comparing `netbox-validity-1.1.0/validity/views/test_result.py` & `netbox-validity-1.2.0/validity/views/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,68 +1,53 @@
-from collections import namedtuple
-from typing import Callable
-
 from django.db.models import Model
 from django.shortcuts import get_object_or_404
+from django_filters import FilterSet
 from django_filters.views import FilterView
-from django_tables2 import SingleTableMixin
-from netbox.views import generic
-from utilities.views import ViewTab, register_model_view
+from django_tables2 import SingleTableMixin, Table
+from utilities.views import ViewTab
 
 from validity import filtersets, forms, models, tables
-from validity.config_compliance.eval import repr_
 
 
-class ComplianceResultListView(generic.ObjectListView):
-    queryset = models.ComplianceTestResult.objects.select_related("test", "device")
-    table = tables.ComplianceResultTable
-    filterset = filtersets.ComplianceTestResultFilterSet
-    filterset_form = forms.ComplianceTestResultFilterForm
-
-
-@register_model_view(models.ComplianceTestResult)
-class ComplianceResultView(generic.ObjectView):
-    queryset = models.ComplianceTestResult.objects.select_related("test", "device")
-
-    def get_result_table(self, request, instance):
-        table = tables.ComplianceResultTable(
-            models.ComplianceTestResult.objects.filter(test=instance.test, device=instance.device).exclude(
-                pk=instance.pk
-            )
-        )
-        table.exclude += ("test", "device")
-        table.order_by = "last_updated"
-        table.configure(request)
-        return table
+class TableMixin:
+    """
+    Mixin to filter aux table in DetailView
+    """
+
+    object_table_field: str
+    filterset: type[FilterSet]
+    table: type[Table]
+
+    def get_table_qs(self, request, instance):
+        return getattr(instance, self.object_table_field).all()
+
+    def get_table_data(self, request, instance):
+        qs = self.get_table_qs(request, instance)
+        return self.filterset(request.GET, qs, request=request).qs
 
-    @staticmethod
-    def repr_func(verbose: bool) -> Callable:
-        func = repr if verbose else repr_
-        return lambda item: item if isinstance(item, str) else func(item)
-
-    def get_explanation_table(self, request, instance):
-        verbose = request.GET.get("verbose", "") == "true"
-        repr_func = self.repr_func(verbose)
-        Explanation = namedtuple("Explanation", "left right")
-        explanations = (Explanation(*map(repr_func, item)) for item in instance.explanation)
-        return tables.ExplanationTable(explanations)
+    def get_table(self, request, instance):
+        return self.table(self.get_table_data(request, instance))
+
+    def configure_table(self, request, table, instance):
+        table.configure(request)
 
     def get_extra_context(self, request, instance):
-        result_table = self.get_result_table(request, instance)
-        explanation_table = self.get_explanation_table(request, instance)
-        return {"result_table": result_table, "explanation_table": explanation_table}
+        table = self.get_table(request, instance)
+        self.configure_table(request, table, instance)
+        return {"table": table, "search_value": request.GET.get("q", "")}
 
 
 class TestResultBaseView(SingleTableMixin, FilterView):
     template_name = "validity/compliance_results.html"
     tab = ViewTab("Test Results", badge=lambda obj: obj.results.count())
     model = models.ComplianceTestResult
     filterset_class = filtersets.ComplianceTestResultFilterSet
     filter_form_class = forms.TestResultFilterForm
     table_class = tables.ComplianceResultTable
+    permission_required = "validity.view_compliancetestresult."
 
     parent_model: type[Model]
     result_relation: str
     read_only: bool = False
     exclude_form_fields: tuple[str, ...] = ()
 
     def get_table(self, **kwargs):
```

