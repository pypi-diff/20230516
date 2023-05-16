# Comparing `tmp/IntuneCD-1.4.5b1.tar.gz` & `tmp/IntuneCD-1.4.5b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IntuneCD-1.4.5b1.tar", last modified: Wed Apr 26 11:12:03 2023, max compression
+gzip compressed data, was "IntuneCD-1.4.5b2.tar", last modified: Thu Apr 27 08:51:02 2023, max compression
```

## Comparing `IntuneCD-1.4.5b1.tar` & `IntuneCD-1.4.5b2.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 tobias     (501) staff       (20)        0 2023-04-26 11:12:03.188841 IntuneCD-1.4.5b1/
--rw-r--r--   0 tobias     (501) staff       (20)     1059 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b1/LICENSE
--rw-r--r--   0 tobias     (501) staff       (20)     3230 2023-04-26 11:12:03.188928 IntuneCD-1.4.5b1/PKG-INFO
--rw-r--r--   0 tobias     (501) staff       (20)     2697 2023-01-24 09:42:37.000000 IntuneCD-1.4.5b1/README.md
--rw-r--r--   0 tobias     (501) staff       (20)      103 2022-05-03 19:33:01.000000 IntuneCD-1.4.5b1/pyproject.toml
--rw-r--r--   0 tobias     (501) staff       (20)      999 2023-04-26 11:12:03.189267 IntuneCD-1.4.5b1/setup.cfg
-drwxr-xr-x   0 tobias     (501) staff       (20)        0 2023-04-26 11:12:03.158575 IntuneCD-1.4.5b1/src/
-drwxr-xr-x   0 tobias     (501) staff       (20)        0 2023-04-26 11:12:03.183579 IntuneCD-1.4.5b1/src/IntuneCD/
--rw-r--r--   0 tobias     (501) staff       (20)        0 2022-05-03 19:33:01.000000 IntuneCD-1.4.5b1/src/IntuneCD/__init__.py
--rw-r--r--   0 tobias     (501) staff       (20)     2344 2023-04-26 08:18:13.000000 IntuneCD-1.4.5b1/src/IntuneCD/archive.py
--rw-r--r--   0 tobias     (501) staff       (20)     3938 2023-03-20 07:54:18.000000 IntuneCD-1.4.5b1/src/IntuneCD/assignment_report.py
--rw-r--r--   0 tobias     (501) staff       (20)     2241 2023-04-24 14:54:23.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_AppProtection.py
--rw-r--r--   0 tobias     (501) staff       (20)     1327 2023-04-24 14:55:45.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_apns.py
--rw-r--r--   0 tobias     (501) staff       (20)     2665 2023-04-24 14:48:58.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_appConfiguration.py
--rw-r--r--   0 tobias     (501) staff       (20)     1865 2023-04-24 15:05:44.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_appleEnrollmentProfile.py
--rw-r--r--   0 tobias     (501) staff       (20)     4651 2023-04-24 14:59:21.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_applications.py
--rw-r--r--   0 tobias     (501) staff       (20)     1370 2023-04-24 15:09:16.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_assignmentFilters.py
--rw-r--r--   0 tobias     (501) staff       (20)     1090 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_autopilotDevices.py
--rw-r--r--   0 tobias     (501) staff       (20)     2473 2023-04-24 15:00:03.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_compliance.py
--rw-r--r--   0 tobias     (501) staff       (20)     1454 2023-04-24 15:11:10.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_compliancePartner.py
--rw-r--r--   0 tobias     (501) staff       (20)     1655 2023-04-24 15:17:25.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_conditionalAccess.py
--rw-r--r--   0 tobias     (501) staff       (20)     2386 2023-04-24 15:16:50.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_configurationPolicies.py
--rw-r--r--   0 tobias     (501) staff       (20)     2718 2023-04-24 15:16:10.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_customAttributeShellScript.py
--rw-r--r--   0 tobias     (501) staff       (20)     1245 2023-04-24 15:01:01.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_deviceManagementSettings.py
--rw-r--r--   0 tobias     (501) staff       (20)     2359 2023-04-24 15:08:23.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_enrollmentConfigurations.py
--rw-r--r--   0 tobias     (501) staff       (20)     2926 2023-04-24 15:07:34.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_enrollmentStatusPage.py
--rw-r--r--   0 tobias     (501) staff       (20)     2508 2023-04-24 15:04:54.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_groupPolicyConfiguration.py
--rw-r--r--   0 tobias     (501) staff       (20)     1378 2023-04-24 15:09:54.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_managedGPlay.py
--rw-r--r--   0 tobias     (501) staff       (20)     2467 2023-04-24 15:10:36.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_managementIntents.py
--rw-r--r--   0 tobias     (501) staff       (20)     1445 2023-04-24 15:11:43.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_managementPartner.py
--rw-r--r--   0 tobias     (501) staff       (20)     1754 2023-04-24 15:02:06.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_notificationTemplate.py
--rw-r--r--   0 tobias     (501) staff       (20)     2710 2023-04-24 15:14:33.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_powershellScripts.py
--rw-r--r--   0 tobias     (501) staff       (20)     3289 2023-04-24 15:13:25.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_proactiveRemediation.py
--rw-r--r--   0 tobias     (501) staff       (20)     4962 2023-04-26 06:18:13.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_profiles.py
--rw-r--r--   0 tobias     (501) staff       (20)     1486 2023-04-24 15:12:12.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_remoteAssistancePartner.py
--rw-r--r--   0 tobias     (501) staff       (20)     2589 2023-04-24 15:15:17.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_shellScripts.py
--rw-r--r--   0 tobias     (501) staff       (20)     1312 2023-04-24 14:57:10.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_vppTokens.py
--rw-r--r--   0 tobias     (501) staff       (20)     1961 2023-04-24 15:06:47.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_windowsEnrollmentProfile.py
--rw-r--r--   0 tobias     (501) staff       (20)      548 2022-08-09 15:09:09.000000 IntuneCD-1.4.5b1/src/IntuneCD/check_file.py
--rw-r--r--   0 tobias     (501) staff       (20)      515 2022-08-09 15:09:09.000000 IntuneCD-1.4.5b1/src/IntuneCD/clean_filename.py
--rw-r--r--   0 tobias     (501) staff       (20)     1933 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b1/src/IntuneCD/diff_summary.py
--rw-r--r--   0 tobias     (501) staff       (20)    15819 2023-04-04 06:15:28.000000 IntuneCD-1.4.5b1/src/IntuneCD/documentation_functions.py
--rw-r--r--   0 tobias     (501) staff       (20)     3701 2023-03-08 08:59:36.000000 IntuneCD-1.4.5b1/src/IntuneCD/get_accesstoken.py
--rw-r--r--   0 tobias     (501) staff       (20)     3198 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b1/src/IntuneCD/get_authparams.py
--rw-r--r--   0 tobias     (501) staff       (20)    10342 2023-04-03 08:56:31.000000 IntuneCD-1.4.5b1/src/IntuneCD/graph_batch.py
--rw-r--r--   0 tobias     (501) staff       (20)     7753 2023-04-26 06:19:45.000000 IntuneCD-1.4.5b1/src/IntuneCD/graph_request.py
--rw-r--r--   0 tobias     (501) staff       (20)      622 2022-08-09 15:09:09.000000 IntuneCD-1.4.5b1/src/IntuneCD/load_file.py
--rw-r--r--   0 tobias     (501) staff       (20)      987 2023-04-25 09:24:15.000000 IntuneCD-1.4.5b1/src/IntuneCD/remove_keys.py
--rw-r--r--   0 tobias     (501) staff       (20)    12362 2023-04-26 06:16:38.000000 IntuneCD-1.4.5b1/src/IntuneCD/run_backup.py
--rw-r--r--   0 tobias     (501) staff       (20)    12356 2023-03-20 12:09:40.000000 IntuneCD-1.4.5b1/src/IntuneCD/run_documentation.py
--rw-r--r--   0 tobias     (501) staff       (20)    10507 2023-04-03 08:56:13.000000 IntuneCD-1.4.5b1/src/IntuneCD/run_update.py
--rw-r--r--   0 tobias     (501) staff       (20)      934 2023-03-06 07:57:06.000000 IntuneCD-1.4.5b1/src/IntuneCD/save_output.py
--rw-r--r--   0 tobias     (501) staff       (20)     8139 2023-04-26 06:20:45.000000 IntuneCD-1.4.5b1/src/IntuneCD/update_appConfiguration.py
--rw-r--r--   0 tobias     (501) staff       (20)     7924 2023-04-26 06:20:55.000000 IntuneCD-1.4.5b1/src/IntuneCD/update_appProtection.py
--rw-r--r--   0 tobias     (501) staff       (20)     3524 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b1/src/IntuneCD/update_appleEnrollmentProfile.py
--rw-r--r--   0 tobias     (501) staff       (20)     7443 2023-03-06 09:55:38.000000 IntuneCD-1.4.5b1/src/IntuneCD/update_assignment.py
--rw-r--r--   0 tobias     (501) staff       (20)     3741 2023-04-25 08:44:13.000000 IntuneCD-1.4.5b1/src/IntuneCD/update_assignmentFilter.py
--rw-r--r--   0 tobias     (501) staff       (20)     9333 2023-04-26 06:21:22.000000 IntuneCD-1.4.5b1/src/IntuneCD/update_compliance.py
--rw-r--r--   0 tobias     (501) staff       (20)     7166 2023-04-26 06:22:17.000000 IntuneCD-1.4.5b1/src/IntuneCD/update_conditionalAccess.py
--rw-r--r--   0 tobias     (501) staff       (20)     7662 2023-04-26 06:22:59.000000 IntuneCD-1.4.5b1/src/IntuneCD/update_configurationPolicies.py
--rw-r--r--   0 tobias     (501) staff       (20)     8890 2023-04-26 06:23:40.000000 IntuneCD-1.4.5b1/src/IntuneCD/update_customAttributeShellScript.py
--rw-r--r--   0 tobias     (501) staff       (20)     2630 2023-03-20 12:09:40.000000 IntuneCD-1.4.5b1/src/IntuneCD/update_deviceManagementSettings.py
--rw-r--r--   0 tobias     (501) staff       (20)    11609 2023-04-26 06:24:16.000000 IntuneCD-1.4.5b1/src/IntuneCD/update_enrollmentConfigurations.py
--rw-r--r--   0 tobias     (501) staff       (20)     8676 2023-04-26 06:25:08.000000 IntuneCD-1.4.5b1/src/IntuneCD/update_enrollmentStatusPage.py
--rw-r--r--   0 tobias     (501) staff       (20)      749 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b1/src/IntuneCD/update_frontend.py
--rw-r--r--   0 tobias     (501) staff       (20)    24247 2023-04-26 06:25:49.000000 IntuneCD-1.4.5b1/src/IntuneCD/update_groupPolicyConfiguration.py
--rw-r--r--   0 tobias     (501) staff       (20)     9030 2023-04-26 06:27:25.000000 IntuneCD-1.4.5b1/src/IntuneCD/update_managementIntents.py
--rw-r--r--   0 tobias     (501) staff       (20)     8039 2023-04-26 06:28:00.000000 IntuneCD-1.4.5b1/src/IntuneCD/update_notificationTemplate.py
--rw-r--r--   0 tobias     (501) staff       (20)     8389 2023-04-26 06:28:30.000000 IntuneCD-1.4.5b1/src/IntuneCD/update_powershellScripts.py
--rw-r--r--   0 tobias     (501) staff       (20)    10573 2023-04-26 06:29:03.000000 IntuneCD-1.4.5b1/src/IntuneCD/update_proactiveRemediation.py
--rw-r--r--   0 tobias     (501) staff       (20)    16073 2023-04-26 06:29:38.000000 IntuneCD-1.4.5b1/src/IntuneCD/update_profiles.py
--rw-r--r--   0 tobias     (501) staff       (20)     8346 2023-04-26 06:30:03.000000 IntuneCD-1.4.5b1/src/IntuneCD/update_shellScripts.py
--rw-r--r--   0 tobias     (501) staff       (20)     7158 2023-04-26 06:30:40.000000 IntuneCD-1.4.5b1/src/IntuneCD/update_windowsEnrollmentProfile.py
-drwxr-xr-x   0 tobias     (501) staff       (20)        0 2023-04-26 11:12:03.184508 IntuneCD-1.4.5b1/src/IntuneCD.egg-info/
--rw-r--r--   0 tobias     (501) staff       (20)     3230 2023-04-26 11:12:03.000000 IntuneCD-1.4.5b1/src/IntuneCD.egg-info/PKG-INFO
--rw-r--r--   0 tobias     (501) staff       (20)     3153 2023-04-26 11:12:03.000000 IntuneCD-1.4.5b1/src/IntuneCD.egg-info/SOURCES.txt
--rw-r--r--   0 tobias     (501) staff       (20)        1 2023-04-26 11:12:03.000000 IntuneCD-1.4.5b1/src/IntuneCD.egg-info/dependency_links.txt
--rw-r--r--   0 tobias     (501) staff       (20)      179 2023-04-26 11:12:03.000000 IntuneCD-1.4.5b1/src/IntuneCD.egg-info/entry_points.txt
--rw-r--r--   0 tobias     (501) staff       (20)      102 2023-04-26 11:12:03.000000 IntuneCD-1.4.5b1/src/IntuneCD.egg-info/requires.txt
--rw-r--r--   0 tobias     (501) staff       (20)        9 2023-04-26 11:12:03.000000 IntuneCD-1.4.5b1/src/IntuneCD.egg-info/top_level.txt
-drwxr-xr-x   0 tobias     (501) staff       (20)        0 2023-04-26 11:12:03.188651 IntuneCD-1.4.5b1/tests/
--rw-r--r--   0 tobias     (501) staff       (20)     2042 2023-04-26 06:14:42.000000 IntuneCD-1.4.5b1/tests/test_archive.py
--rw-r--r--   0 tobias     (501) staff       (20)     2005 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b1/tests/test_check_file.py
--rw-r--r--   0 tobias     (501) staff       (20)      848 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b1/tests/test_clean_filename.py
--rw-r--r--   0 tobias     (501) staff       (20)     2096 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b1/tests/test_diff_summary.py
--rw-r--r--   0 tobias     (501) staff       (20)     7233 2023-04-04 06:15:28.000000 IntuneCD-1.4.5b1/tests/test_documentation_functions.py
--rw-r--r--   0 tobias     (501) staff       (20)      953 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b1/tests/test_get_added_removed.py
--rw-r--r--   0 tobias     (501) staff       (20)     9753 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b1/tests/test_get_authparams.py
--rw-r--r--   0 tobias     (501) staff       (20)    12241 2023-03-08 09:16:49.000000 IntuneCD-1.4.5b1/tests/test_graph_batch.py
--rw-r--r--   0 tobias     (501) staff       (20)    14412 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b1/tests/test_graph_request.py
--rw-r--r--   0 tobias     (501) staff       (20)     2980 2023-03-08 10:43:23.000000 IntuneCD-1.4.5b1/tests/test_group_report.py
--rw-r--r--   0 tobias     (501) staff       (20)     1279 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b1/tests/test_load_file.py
--rw-r--r--   0 tobias     (501) staff       (20)     1622 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b1/tests/test_match.py
--rw-r--r--   0 tobias     (501) staff       (20)      559 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b1/tests/test_remove_keys.py
--rw-r--r--   0 tobias     (501) staff       (20)     1888 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b1/tests/test_save_output.py
--rw-r--r--   0 tobias     (501) staff       (20)     2292 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b1/tests/test_update_frontend.py
+drwxr-xr-x   0 tobias     (501) staff       (20)        0 2023-04-27 08:51:02.989494 IntuneCD-1.4.5b2/
+-rw-r--r--   0 tobias     (501) staff       (20)     1059 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b2/LICENSE
+-rw-r--r--   0 tobias     (501) staff       (20)     3230 2023-04-27 08:51:02.989621 IntuneCD-1.4.5b2/PKG-INFO
+-rw-r--r--   0 tobias     (501) staff       (20)     2697 2023-01-24 09:42:37.000000 IntuneCD-1.4.5b2/README.md
+-rw-r--r--   0 tobias     (501) staff       (20)      103 2022-05-03 19:33:01.000000 IntuneCD-1.4.5b2/pyproject.toml
+-rw-r--r--   0 tobias     (501) staff       (20)      999 2023-04-27 08:51:02.989988 IntuneCD-1.4.5b2/setup.cfg
+drwxr-xr-x   0 tobias     (501) staff       (20)        0 2023-04-27 08:51:02.959068 IntuneCD-1.4.5b2/src/
+drwxr-xr-x   0 tobias     (501) staff       (20)        0 2023-04-27 08:51:02.983938 IntuneCD-1.4.5b2/src/IntuneCD/
+-rw-r--r--   0 tobias     (501) staff       (20)        0 2022-05-03 19:33:01.000000 IntuneCD-1.4.5b2/src/IntuneCD/__init__.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2344 2023-04-26 08:18:13.000000 IntuneCD-1.4.5b2/src/IntuneCD/archive.py
+-rw-r--r--   0 tobias     (501) staff       (20)     3938 2023-03-20 07:54:18.000000 IntuneCD-1.4.5b2/src/IntuneCD/assignment_report.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2241 2023-04-24 14:54:23.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_AppProtection.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1327 2023-04-24 14:55:45.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_apns.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2665 2023-04-24 14:48:58.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_appConfiguration.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1865 2023-04-24 15:05:44.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_appleEnrollmentProfile.py
+-rw-r--r--   0 tobias     (501) staff       (20)     4651 2023-04-24 14:59:21.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_applications.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1370 2023-04-24 15:09:16.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_assignmentFilters.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1090 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_autopilotDevices.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2473 2023-04-24 15:00:03.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_compliance.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1454 2023-04-24 15:11:10.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_compliancePartner.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1655 2023-04-24 15:17:25.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_conditionalAccess.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2386 2023-04-24 15:16:50.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_configurationPolicies.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2718 2023-04-24 15:16:10.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_customAttributeShellScript.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1245 2023-04-24 15:01:01.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_deviceManagementSettings.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2359 2023-04-24 15:08:23.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_enrollmentConfigurations.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2926 2023-04-24 15:07:34.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_enrollmentStatusPage.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2508 2023-04-24 15:04:54.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_groupPolicyConfiguration.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1378 2023-04-24 15:09:54.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_managedGPlay.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2467 2023-04-24 15:10:36.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_managementIntents.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1445 2023-04-24 15:11:43.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_managementPartner.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1754 2023-04-24 15:02:06.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_notificationTemplate.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2710 2023-04-24 15:14:33.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_powershellScripts.py
+-rw-r--r--   0 tobias     (501) staff       (20)     3289 2023-04-24 15:13:25.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_proactiveRemediation.py
+-rw-r--r--   0 tobias     (501) staff       (20)     4962 2023-04-26 06:18:13.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_profiles.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1486 2023-04-24 15:12:12.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_remoteAssistancePartner.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2589 2023-04-24 15:15:17.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_shellScripts.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1312 2023-04-24 14:57:10.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_vppTokens.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1961 2023-04-24 15:06:47.000000 IntuneCD-1.4.5b2/src/IntuneCD/backup_windowsEnrollmentProfile.py
+-rw-r--r--   0 tobias     (501) staff       (20)      548 2022-08-09 15:09:09.000000 IntuneCD-1.4.5b2/src/IntuneCD/check_file.py
+-rw-r--r--   0 tobias     (501) staff       (20)      515 2022-08-09 15:09:09.000000 IntuneCD-1.4.5b2/src/IntuneCD/clean_filename.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1933 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b2/src/IntuneCD/diff_summary.py
+-rw-r--r--   0 tobias     (501) staff       (20)    15819 2023-04-04 06:15:28.000000 IntuneCD-1.4.5b2/src/IntuneCD/documentation_functions.py
+-rw-r--r--   0 tobias     (501) staff       (20)     3701 2023-03-08 08:59:36.000000 IntuneCD-1.4.5b2/src/IntuneCD/get_accesstoken.py
+-rw-r--r--   0 tobias     (501) staff       (20)     3198 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b2/src/IntuneCD/get_authparams.py
+-rw-r--r--   0 tobias     (501) staff       (20)    10342 2023-04-03 08:56:31.000000 IntuneCD-1.4.5b2/src/IntuneCD/graph_batch.py
+-rw-r--r--   0 tobias     (501) staff       (20)     7753 2023-04-26 06:19:45.000000 IntuneCD-1.4.5b2/src/IntuneCD/graph_request.py
+-rw-r--r--   0 tobias     (501) staff       (20)      622 2022-08-09 15:09:09.000000 IntuneCD-1.4.5b2/src/IntuneCD/load_file.py
+-rw-r--r--   0 tobias     (501) staff       (20)      987 2023-04-25 09:24:15.000000 IntuneCD-1.4.5b2/src/IntuneCD/remove_keys.py
+-rw-r--r--   0 tobias     (501) staff       (20)    12362 2023-04-26 06:16:38.000000 IntuneCD-1.4.5b2/src/IntuneCD/run_backup.py
+-rw-r--r--   0 tobias     (501) staff       (20)    12356 2023-03-20 12:09:40.000000 IntuneCD-1.4.5b2/src/IntuneCD/run_documentation.py
+-rw-r--r--   0 tobias     (501) staff       (20)    11471 2023-04-26 11:47:47.000000 IntuneCD-1.4.5b2/src/IntuneCD/run_update.py
+-rw-r--r--   0 tobias     (501) staff       (20)      934 2023-03-06 07:57:06.000000 IntuneCD-1.4.5b2/src/IntuneCD/save_output.py
+-rw-r--r--   0 tobias     (501) staff       (20)     8178 2023-04-26 11:50:38.000000 IntuneCD-1.4.5b2/src/IntuneCD/update_appConfiguration.py
+-rw-r--r--   0 tobias     (501) staff       (20)     7963 2023-04-26 11:50:51.000000 IntuneCD-1.4.5b2/src/IntuneCD/update_appProtection.py
+-rw-r--r--   0 tobias     (501) staff       (20)     3524 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b2/src/IntuneCD/update_appleEnrollmentProfile.py
+-rw-r--r--   0 tobias     (501) staff       (20)     7443 2023-03-06 09:55:38.000000 IntuneCD-1.4.5b2/src/IntuneCD/update_assignment.py
+-rw-r--r--   0 tobias     (501) staff       (20)     3741 2023-04-25 08:44:13.000000 IntuneCD-1.4.5b2/src/IntuneCD/update_assignmentFilter.py
+-rw-r--r--   0 tobias     (501) staff       (20)     9372 2023-04-26 11:51:00.000000 IntuneCD-1.4.5b2/src/IntuneCD/update_compliance.py
+-rw-r--r--   0 tobias     (501) staff       (20)     7193 2023-04-26 11:51:09.000000 IntuneCD-1.4.5b2/src/IntuneCD/update_conditionalAccess.py
+-rw-r--r--   0 tobias     (501) staff       (20)     7703 2023-04-26 11:51:17.000000 IntuneCD-1.4.5b2/src/IntuneCD/update_configurationPolicies.py
+-rw-r--r--   0 tobias     (501) staff       (20)     8929 2023-04-26 11:51:24.000000 IntuneCD-1.4.5b2/src/IntuneCD/update_customAttributeShellScript.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2630 2023-03-20 12:09:40.000000 IntuneCD-1.4.5b2/src/IntuneCD/update_deviceManagementSettings.py
+-rw-r--r--   0 tobias     (501) staff       (20)    11648 2023-04-26 11:51:36.000000 IntuneCD-1.4.5b2/src/IntuneCD/update_enrollmentConfigurations.py
+-rw-r--r--   0 tobias     (501) staff       (20)     8715 2023-04-26 11:51:43.000000 IntuneCD-1.4.5b2/src/IntuneCD/update_enrollmentStatusPage.py
+-rw-r--r--   0 tobias     (501) staff       (20)      749 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b2/src/IntuneCD/update_frontend.py
+-rw-r--r--   0 tobias     (501) staff       (20)    24286 2023-04-26 11:51:50.000000 IntuneCD-1.4.5b2/src/IntuneCD/update_groupPolicyConfiguration.py
+-rw-r--r--   0 tobias     (501) staff       (20)     9069 2023-04-26 11:51:58.000000 IntuneCD-1.4.5b2/src/IntuneCD/update_managementIntents.py
+-rw-r--r--   0 tobias     (501) staff       (20)     8066 2023-04-26 11:52:05.000000 IntuneCD-1.4.5b2/src/IntuneCD/update_notificationTemplate.py
+-rw-r--r--   0 tobias     (501) staff       (20)     8428 2023-04-26 11:52:12.000000 IntuneCD-1.4.5b2/src/IntuneCD/update_powershellScripts.py
+-rw-r--r--   0 tobias     (501) staff       (20)    10612 2023-04-26 11:52:18.000000 IntuneCD-1.4.5b2/src/IntuneCD/update_proactiveRemediation.py
+-rw-r--r--   0 tobias     (501) staff       (20)    16112 2023-04-26 11:52:24.000000 IntuneCD-1.4.5b2/src/IntuneCD/update_profiles.py
+-rw-r--r--   0 tobias     (501) staff       (20)     8385 2023-04-26 11:52:32.000000 IntuneCD-1.4.5b2/src/IntuneCD/update_shellScripts.py
+-rw-r--r--   0 tobias     (501) staff       (20)     7197 2023-04-26 11:52:39.000000 IntuneCD-1.4.5b2/src/IntuneCD/update_windowsEnrollmentProfile.py
+drwxr-xr-x   0 tobias     (501) staff       (20)        0 2023-04-27 08:51:02.985094 IntuneCD-1.4.5b2/src/IntuneCD.egg-info/
+-rw-r--r--   0 tobias     (501) staff       (20)     3230 2023-04-27 08:51:02.000000 IntuneCD-1.4.5b2/src/IntuneCD.egg-info/PKG-INFO
+-rw-r--r--   0 tobias     (501) staff       (20)     3153 2023-04-27 08:51:02.000000 IntuneCD-1.4.5b2/src/IntuneCD.egg-info/SOURCES.txt
+-rw-r--r--   0 tobias     (501) staff       (20)        1 2023-04-27 08:51:02.000000 IntuneCD-1.4.5b2/src/IntuneCD.egg-info/dependency_links.txt
+-rw-r--r--   0 tobias     (501) staff       (20)      179 2023-04-27 08:51:02.000000 IntuneCD-1.4.5b2/src/IntuneCD.egg-info/entry_points.txt
+-rw-r--r--   0 tobias     (501) staff       (20)      102 2023-04-27 08:51:02.000000 IntuneCD-1.4.5b2/src/IntuneCD.egg-info/requires.txt
+-rw-r--r--   0 tobias     (501) staff       (20)        9 2023-04-27 08:51:02.000000 IntuneCD-1.4.5b2/src/IntuneCD.egg-info/top_level.txt
+drwxr-xr-x   0 tobias     (501) staff       (20)        0 2023-04-27 08:51:02.989311 IntuneCD-1.4.5b2/tests/
+-rw-r--r--   0 tobias     (501) staff       (20)     2042 2023-04-26 06:14:42.000000 IntuneCD-1.4.5b2/tests/test_archive.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2005 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b2/tests/test_check_file.py
+-rw-r--r--   0 tobias     (501) staff       (20)      848 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b2/tests/test_clean_filename.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2096 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b2/tests/test_diff_summary.py
+-rw-r--r--   0 tobias     (501) staff       (20)     7233 2023-04-04 06:15:28.000000 IntuneCD-1.4.5b2/tests/test_documentation_functions.py
+-rw-r--r--   0 tobias     (501) staff       (20)      953 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b2/tests/test_get_added_removed.py
+-rw-r--r--   0 tobias     (501) staff       (20)     9753 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b2/tests/test_get_authparams.py
+-rw-r--r--   0 tobias     (501) staff       (20)    12241 2023-03-08 09:16:49.000000 IntuneCD-1.4.5b2/tests/test_graph_batch.py
+-rw-r--r--   0 tobias     (501) staff       (20)    17428 2023-04-27 08:46:23.000000 IntuneCD-1.4.5b2/tests/test_graph_request.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2980 2023-03-08 10:43:23.000000 IntuneCD-1.4.5b2/tests/test_group_report.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1279 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b2/tests/test_load_file.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1622 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b2/tests/test_match.py
+-rw-r--r--   0 tobias     (501) staff       (20)      559 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b2/tests/test_remove_keys.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1888 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b2/tests/test_save_output.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2292 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b2/tests/test_update_frontend.py
```

### Comparing `IntuneCD-1.4.5b1/LICENSE` & `IntuneCD-1.4.5b2/LICENSE`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/PKG-INFO` & `IntuneCD-1.4.5b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IntuneCD
-Version: 1.4.5b1
+Version: 1.4.5b2
 Summary: Tool to backup and update configurations in Intune
 Home-page: https://github.com/almenscorner/IntuneCD
 Author: Tobias Almén
 Author-email: almenscorner@outlook.com
 Project-URL: Bug Tracker, https://github.com/almenscorner/IntuneCD/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `IntuneCD-1.4.5b1/README.md` & `IntuneCD-1.4.5b2/README.md`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/setup.cfg` & `IntuneCD-1.4.5b2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = IntuneCD
-version = 1.4.5.beta1
+version = 1.4.5.beta2
 author = Tobias Almén
 author_email = almenscorner@outlook.com
 description = Tool to backup and update configurations in Intune
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/almenscorner/IntuneCD
 project_urls =
```

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/archive.py` & `IntuneCD-1.4.5b2/src/IntuneCD/archive.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/assignment_report.py` & `IntuneCD-1.4.5b2/src/IntuneCD/assignment_report.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/backup_AppProtection.py` & `IntuneCD-1.4.5b2/src/IntuneCD/backup_AppProtection.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/backup_apns.py` & `IntuneCD-1.4.5b2/src/IntuneCD/backup_apns.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/backup_appConfiguration.py` & `IntuneCD-1.4.5b2/src/IntuneCD/backup_appConfiguration.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/backup_appleEnrollmentProfile.py` & `IntuneCD-1.4.5b2/src/IntuneCD/backup_appleEnrollmentProfile.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/backup_applications.py` & `IntuneCD-1.4.5b2/src/IntuneCD/backup_applications.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/backup_assignmentFilters.py` & `IntuneCD-1.4.5b2/src/IntuneCD/backup_assignmentFilters.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/backup_autopilotDevices.py` & `IntuneCD-1.4.5b2/src/IntuneCD/backup_autopilotDevices.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/backup_compliance.py` & `IntuneCD-1.4.5b2/src/IntuneCD/backup_compliance.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/backup_compliancePartner.py` & `IntuneCD-1.4.5b2/src/IntuneCD/backup_compliancePartner.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/backup_conditionalAccess.py` & `IntuneCD-1.4.5b2/src/IntuneCD/backup_conditionalAccess.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/backup_configurationPolicies.py` & `IntuneCD-1.4.5b2/src/IntuneCD/backup_configurationPolicies.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/backup_customAttributeShellScript.py` & `IntuneCD-1.4.5b2/src/IntuneCD/backup_customAttributeShellScript.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/backup_deviceManagementSettings.py` & `IntuneCD-1.4.5b2/src/IntuneCD/backup_deviceManagementSettings.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/backup_enrollmentConfigurations.py` & `IntuneCD-1.4.5b2/src/IntuneCD/backup_enrollmentConfigurations.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/backup_enrollmentStatusPage.py` & `IntuneCD-1.4.5b2/src/IntuneCD/backup_enrollmentStatusPage.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/backup_groupPolicyConfiguration.py` & `IntuneCD-1.4.5b2/src/IntuneCD/backup_groupPolicyConfiguration.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/backup_managedGPlay.py` & `IntuneCD-1.4.5b2/src/IntuneCD/backup_managedGPlay.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/backup_managementIntents.py` & `IntuneCD-1.4.5b2/src/IntuneCD/backup_managementIntents.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/backup_managementPartner.py` & `IntuneCD-1.4.5b2/src/IntuneCD/backup_managementPartner.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/backup_notificationTemplate.py` & `IntuneCD-1.4.5b2/src/IntuneCD/backup_notificationTemplate.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/backup_powershellScripts.py` & `IntuneCD-1.4.5b2/src/IntuneCD/backup_powershellScripts.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/backup_proactiveRemediation.py` & `IntuneCD-1.4.5b2/src/IntuneCD/backup_proactiveRemediation.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/backup_profiles.py` & `IntuneCD-1.4.5b2/src/IntuneCD/backup_profiles.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/backup_remoteAssistancePartner.py` & `IntuneCD-1.4.5b2/src/IntuneCD/backup_remoteAssistancePartner.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/backup_shellScripts.py` & `IntuneCD-1.4.5b2/src/IntuneCD/backup_shellScripts.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/backup_vppTokens.py` & `IntuneCD-1.4.5b2/src/IntuneCD/backup_vppTokens.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/backup_windowsEnrollmentProfile.py` & `IntuneCD-1.4.5b2/src/IntuneCD/backup_windowsEnrollmentProfile.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/check_file.py` & `IntuneCD-1.4.5b2/src/IntuneCD/check_file.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/clean_filename.py` & `IntuneCD-1.4.5b2/src/IntuneCD/clean_filename.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/diff_summary.py` & `IntuneCD-1.4.5b2/src/IntuneCD/diff_summary.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/documentation_functions.py` & `IntuneCD-1.4.5b2/src/IntuneCD/documentation_functions.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/get_accesstoken.py` & `IntuneCD-1.4.5b2/src/IntuneCD/get_accesstoken.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/get_authparams.py` & `IntuneCD-1.4.5b2/src/IntuneCD/get_authparams.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/graph_batch.py` & `IntuneCD-1.4.5b2/src/IntuneCD/graph_batch.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/graph_request.py` & `IntuneCD-1.4.5b2/src/IntuneCD/graph_request.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/load_file.py` & `IntuneCD-1.4.5b2/src/IntuneCD/load_file.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/remove_keys.py` & `IntuneCD-1.4.5b2/src/IntuneCD/remove_keys.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/run_backup.py` & `IntuneCD-1.4.5b2/src/IntuneCD/run_backup.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/run_documentation.py` & `IntuneCD-1.4.5b2/src/IntuneCD/run_documentation.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/run_update.py` & `IntuneCD-1.4.5b2/src/IntuneCD/run_update.py`

 * *Files 8% similar despite different names*

```diff
@@ -120,14 +120,19 @@
     )
     parser.add_argument(
         "-g",
         "--create-groups",
         help="When this parameter is set, groups are created if they do not exist",
         action="store_true",
     )
+    parser.add_argument(
+        "--remove",
+        help="When this parameter is set, configurations in Intune that are not in the backup are removed",
+        action="store_true",
+    )
 
     args = parser.parse_args()
 
     def devtoprod():
         return "devtoprod"
 
     def standalone():
@@ -148,117 +153,145 @@
         args.mode,
         args.localauth,
         args.certauth,
         args.interactiveauth,
         tenant="PROD",
     )
 
-    def run_update(path, token, assignment, exclude, report, create_groups):
+    def run_update(path, token, assignment, exclude, report, create_groups, remove):
         diff_count = 0
         diff_summary = []
 
         if "AppConfigurations" not in exclude:
             from .update_appConfiguration import update
 
-            diff_summary.append(update(path, token, assignment, report, create_groups))
+            diff_summary.append(
+                update(path, token, assignment, report, create_groups, remove)
+            )
 
         if "AppProtection" not in exclude:
             from .update_appProtection import update
 
-            diff_summary.append(update(path, token, assignment, report, create_groups))
+            diff_summary.append(
+                update(path, token, assignment, report, create_groups, remove)
+            )
 
         if "Compliance" not in exclude:
             from .update_compliance import update
 
-            diff_summary.append(update(path, token, assignment, report, create_groups))
+            diff_summary.append(
+                update(path, token, assignment, report, create_groups, remove)
+            )
 
         if "DeviceManagementSettings" not in exclude and args.interactiveauth is True:
             from .update_deviceManagementSettings import update
 
             diff_summary.append(update(path, token, report))
         else:
             print("-" * 90)
             print(
                 "***Device Management Settings is only available with interactive auth***"
             )
 
         if "NotificationTemplate" not in exclude:
             from .update_notificationTemplate import update
 
-            diff_summary.append(update(path, token, report))
+            diff_summary.append(update(path, token, report, remove))
 
         if "Profiles" not in exclude:
             from .update_profiles import update
 
-            diff_summary.append(update(path, token, assignment, report, create_groups))
+            diff_summary.append(
+                update(path, token, assignment, report, create_groups, remove)
+            )
 
         if "GPOConfigurations" not in exclude:
             from .update_groupPolicyConfiguration import update
 
-            diff_summary.append(update(path, token, assignment, report, create_groups))
+            diff_summary.append(
+                update(path, token, assignment, report, create_groups, remove)
+            )
 
         if "AppleEnrollmentProfile" not in exclude:
             from .update_appleEnrollmentProfile import update
 
             diff_summary.append(update(path, token, report))
 
         if "WindowsEnrollmentProfile" not in exclude:
             from .update_windowsEnrollmentProfile import update
 
-            diff_summary.append(update(path, token, assignment, report, create_groups))
+            diff_summary.append(
+                update(path, token, assignment, report, create_groups, remove)
+            )
 
         if "EnrollmentStatusPage" not in exclude:
             from .update_enrollmentStatusPage import update
 
-            diff_summary.append(update(path, token, assignment, report, create_groups))
+            diff_summary.append(
+                update(path, token, assignment, report, create_groups, remove)
+            )
 
         if "EnrollmentConfigurations" not in exclude:
             from .update_enrollmentConfigurations import update
 
-            diff_summary.append(update(path, token, assignment, report, create_groups))
+            diff_summary.append(
+                update(path, token, assignment, report, create_groups, remove)
+            )
 
         if "Filters" not in exclude:
             from .update_assignmentFilter import update
 
             diff_summary.append(update(path, token, report))
 
         if "Intents" not in exclude:
             from .update_managementIntents import update
 
-            diff_summary.append(update(path, token, assignment, report, create_groups))
+            diff_summary.append(
+                update(path, token, assignment, report, create_groups, remove)
+            )
 
         if "ProactiveRemediation" not in exclude:
             from .update_proactiveRemediation import update
 
-            diff_summary.append(update(path, token, assignment, report, create_groups))
+            diff_summary.append(
+                update(path, token, assignment, report, create_groups, remove)
+            )
 
         if "PowershellScripts" not in exclude:
             from .update_powershellScripts import update
 
-            diff_summary.append(update(path, token, assignment, report, create_groups))
+            diff_summary.append(
+                update(path, token, assignment, report, create_groups, remove)
+            )
 
         if "ShellScripts" not in exclude:
             from .update_shellScripts import update
 
-            diff_summary.append(update(path, token, assignment, report, create_groups))
+            diff_summary.append(
+                update(path, token, assignment, report, create_groups, remove)
+            )
 
         if "CustomAttribute" not in exclude:
             from .update_customAttributeShellScript import update
 
-            diff_summary.append(update(path, token, assignment, report, create_groups))
+            diff_summary.append(
+                update(path, token, assignment, report, create_groups, remove)
+            )
 
         if "ConfigurationPolicies" not in exclude:
             from .update_configurationPolicies import update
 
-            diff_summary.append(update(path, token, assignment, report, create_groups))
+            diff_summary.append(
+                update(path, token, assignment, report, create_groups, remove)
+            )
 
         if "ConditionalAccess" not in exclude:
             from .update_conditionalAccess import update
 
-            diff_count += update(path, token, report)
+            diff_count += update(path, token, report, remove)
 
         for sum in diff_summary:
             for config in sum:
                 diff_count += config.count
 
         return diff_count, diff_summary
 
@@ -273,15 +306,21 @@
         if args.report:
             print("***Running in report mode, no updates will be pushed to Intune***")
 
         if args.frontend:
             old_stdout = sys.stdout
             sys.stdout = feedstdout = StringIO()
             summary = run_update(
-                args.path, token, args.u, exclude, args.report, args.create_groups
+                args.path,
+                token,
+                args.u,
+                exclude,
+                args.report,
+                args.create_groups,
+                args.remove,
             )
             sys.stdout = old_stdout
             feed_bytes = feedstdout.getvalue().encode("utf-8")
             out = base64.b64encode(feed_bytes).decode("utf-8")
 
             body = {"type": "diff_count", "diff_count": summary[0]}
             update_frontend(f"{args.frontend}/api/overview/summary", body)
@@ -302,13 +341,19 @@
                         )
 
             if len(body) > 0:
                 update_frontend(f"{args.frontend}/api/changes/summary", body)
 
         else:
             run_update(
-                args.path, token, args.u, exclude, args.report, args.create_groups
+                args.path,
+                token,
+                args.u,
+                exclude,
+                args.report,
+                args.create_groups,
+                args.remove,
             )
 
 
 if __name__ == "__main__":
     start()
```

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/save_output.py` & `IntuneCD-1.4.5b2/src/IntuneCD/save_output.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/update_appConfiguration.py` & `IntuneCD-1.4.5b2/src/IntuneCD/update_appConfiguration.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,17 @@
 # Set MS Graph endpoint
 ENDPOINT = (
     "https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations"
 )
 APP_ENDPOINT = "https://graph.microsoft.com/beta/deviceAppManagement/mobileApps"
 
 
-def update(path, token, assignment=False, report=False, create_groups=False):
+def update(
+    path, token, assignment=False, report=False, create_groups=False, remove=False
+):
     """
     This function updates all App Configuration Polices in Intune,
     if the configuration in Intune differs from the JSON/YAML file.
 
     :param path: Path to where the backup is saved
     :param token: Token to use for authenticating the request
     :param assignment: Boolean to determine if assignments should be updated
@@ -179,15 +181,15 @@
                         )
                     else:
                         print(
                             "App configured in App Configuration profile could not be found, skipping creation"
                         )
 
         # If any App Configurations are left in mem_data, remove them from Intune as they are not in the repo
-        if mem_data.get("value", None) is not None:
+        if mem_data.get("value", None) is not None and remove is True:
             for val in mem_data["value"]:
                 print("-" * 90)
                 print("Removing App Configuration from Intune: " + val["displayName"])
                 if report is False:
                     makeapirequestDelete(
                         f"{ENDPOINT}/{val['id']}", token, status_code=200
                     )
```

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/update_appProtection.py` & `IntuneCD-1.4.5b2/src/IntuneCD/update_appProtection.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,17 @@
 from .check_file import check_file
 from .load_file import load_file
 
 # Set MS Graph endpoint
 ENDPOINT = "https://graph.microsoft.com/beta/deviceAppManagement/"
 
 
-def update(path, token, assignment=False, report=False, create_groups=False):
+def update(
+    path, token, assignment=False, report=False, create_groups=False, remove=False
+):
     """
     This function updates all App Protection Polices in Intune,
     if the configuration in Intune differs from the JSON/YAML file.
 
     :param path: Path to where the backup is saved
     :param token: Token to use for authenticating the request
     :param assignment: Boolean to determine if assignments should be updated
@@ -172,15 +174,15 @@
                                 "assign",
                                 token,
                                 status_code=204,
                             )
                         print("App Protection created with id: " + post_request["id"])
 
         # If any App Protections are left in mem_data, remove them from Intune as they are not in the repo
-        if mem_data.get("value", None) is not None:
+        if mem_data.get("value", None) is not None and remove is True:
             for val in mem_data["value"]:
                 print("-" * 90)
                 print("Removing App Protection from Intune: " + val["displayName"])
                 if report is False:
                     makeapirequestDelete(
                         f"{ENDPOINT}managedAppPolicies/{val['id']}",
                         token,
```

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/update_appleEnrollmentProfile.py` & `IntuneCD-1.4.5b2/src/IntuneCD/update_appleEnrollmentProfile.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/update_assignment.py` & `IntuneCD-1.4.5b2/src/IntuneCD/update_assignment.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/update_assignmentFilter.py` & `IntuneCD-1.4.5b2/src/IntuneCD/update_assignmentFilter.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/update_compliance.py` & `IntuneCD-1.4.5b2/src/IntuneCD/update_compliance.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,17 @@
 from .diff_summary import DiffSummary
 
 
 # Set MS Graph endpoint
 ENDPOINT = "https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies"
 
 
-def update(path, token, assignment=False, report=False, create_groups=False):
+def update(
+    path, token, assignment=False, report=False, create_groups=False, remove=False
+):
     """
     This function updates all Compliance Polices in Intune,
     if the configuration in Intune differs from the JSON/YAML file.
 
     :param path: Path to where the backup is saved
     :param token: Token to use for authenticating the request
     :param assignment: Boolean to determine if assignments should be updated
@@ -207,15 +209,15 @@
                                 token,
                             )
                         print(
                             "Compliance Policy created with id: " + post_request["id"]
                         )
 
         # If any Compliance Policies are left in mem_data, remove them from Intune as they are not in the repo
-        if mem_data.get("value", None) is not None:
+        if mem_data.get("value", None) is not None and remove is True:
             for val in mem_data["value"]:
                 print("-" * 90)
                 print("Removing Compliance Policy from Intune: " + val["displayName"])
                 if report is False:
                     makeapirequestDelete(
                         f"{ENDPOINT}/{val['id']}", token, status_code=200
                     )
```

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/update_conditionalAccess.py` & `IntuneCD-1.4.5b2/src/IntuneCD/update_conditionalAccess.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from .load_file import load_file
 from .remove_keys import remove_keys
 
 # Set MS Graph endpoint
 ENDPOINT = "https://graph.microsoft.com/beta/identity/conditionalAccess/policies"
 
 
-def update(path, token, report):
+def update(path, token, report, remove):
     """
     This function updates all Conditional Access Profiles in Intune,
     if the configuration in Intune differs from the JSON/YAML file.
 
     :param path: Path to where the backup is saved
     :param token: Token to use for authenticating the request
     """
@@ -152,15 +152,15 @@
                         if post_request:
                             print(
                                 "Conditional Access policy created with id: "
                                 + post_request["id"]
                             )
 
         # If any Conditional Access policy are left in mem_data, remove them from Intune as they are not in the repo
-        if mem_data.get("value", None) is not None:
+        if mem_data.get("value", None) is not None and remove is True:
             for val in mem_data["value"]:
                 print("-" * 90)
                 print(
                     "Removing Conditional Access Policy from Intune: "
                     + val["displayName"]
                 )
                 if report is False:
```

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/update_configurationPolicies.py` & `IntuneCD-1.4.5b2/src/IntuneCD/update_configurationPolicies.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,17 @@
 from .load_file import load_file
 from .diff_summary import DiffSummary
 
 # Set MS Graph endpoint
 ENDPOINT = "https://graph.microsoft.com/beta/deviceManagement/configurationPolicies"
 
 
-def update(path, token, assignment=False, report=False, create_groups=False):
+def update(
+    path, token, assignment=False, report=False, create_groups=False, remove=False
+):
     """
     This function updates all Settings Catalog configurations in Intune,
     if the configuration in Intune differs from the JSON/YAML file.
 
     :param path: Path to where the backup is saved
     :param token: Token to use for authenticating the request
     :param assignment: Boolean to determine if assignments should be updated
@@ -168,15 +170,15 @@
                             )
                         print(
                             "Configuration Policy created with id: "
                             + post_request["id"]
                         )
 
         # If any Configuration Policies are left in mem_data, remove them from Intune as they are not in the repo
-        if mem_data.get("value", None) is not None:
+        if mem_data.get("value", None) is not None and remove is True:
             for val in mem_data["value"]:
                 print("-" * 90)
                 print("Removing Configuration Policy from Intune: " + val["name"])
                 if report is False:
                     makeapirequestDelete(
                         f"{ENDPOINT}/{val['id']}", token, status_code=200
                     )
```

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/update_customAttributeShellScript.py` & `IntuneCD-1.4.5b2/src/IntuneCD/update_customAttributeShellScript.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,17 @@
 # Set MS Graph endpoint
 ENDPOINT = "https://graph.microsoft.com/beta/deviceManagement/deviceCustomAttributeShellScripts"
 ASSIGNMENT_ENDPOINT = (
     "https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts"
 )
 
 
-def update(path, token, assignment=False, report=False, create_groups=False):
+def update(
+    path, token, assignment=False, report=False, create_groups=False, remove=False
+):
     """
     This function updates all Custom Attribute Shell scripts in Intune if the configuration in Intune differs from the JSON/YAML file.
 
     :param path: Path to where the backup is saved
     :param token: Token to use for authenticating the request
     :param assignment: Boolean to determine if assignments should be updated
     """
@@ -195,15 +197,15 @@
                                 "deviceManagement/deviceManagementScripts",
                                 "assign",
                                 token,
                             )
                         print("Custom Attribute created with id: " + post_request["id"])
 
         # If any Custom Attribute scripts are left in mem_shellScript, remove them from Intune as they are not in the repo
-        if mem_shellScript.get("value", None) is not None:
+        if mem_shellScript.get("value", None) is not None and remove is True:
             for val in mem_shellScript["value"]:
                 print("-" * 90)
                 print("Removing Custom Attribute from Intune: " + val["displayName"])
                 if report is False:
                     makeapirequestDelete(
                         f"{ENDPOINT}/{val['id']}", token, status_code=200
                     )
```

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/update_deviceManagementSettings.py` & `IntuneCD-1.4.5b2/src/IntuneCD/update_deviceManagementSettings.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/update_enrollmentConfigurations.py` & `IntuneCD-1.4.5b2/src/IntuneCD/update_enrollmentConfigurations.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,17 @@
 
 # Set MS Graph endpoint
 ENDPOINT = (
     "https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations"
 )
 
 
-def update(path, token, assignment=False, report=False, create_groups=False):
+def update(
+    path, token, assignment=False, report=False, create_groups=False, remove=False
+):
     """_summary_
 
     Args:
         path (str): Path to where the backup is saved
         token (str): Token to use for authenticating the request
         assignment (bool, optional): Decides if assignment should be updated. Defaults to False.
         report (bool, optional): If true, runs in report mode only. Defaults to False.
@@ -239,15 +241,15 @@
                             )
                         print(
                             f"Enrollment Config {config_type} created with id: "
                             + post_request["id"]
                         )
 
         # If any Enrollment Configurations are left in intune_data, remove them from Intune as they are not in the repo
-        if intune_data.get("value", None) is not None:
+        if intune_data.get("value", None) is not None and remove is True:
             for val in intune_data["value"]:
                 if (
                     val["@odata.type"]
                     == "#microsoft.graph.windows10EnrollmentCompletionPageConfiguration"
                 ):
                     continue
                 print("-" * 90)
```

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/update_enrollmentStatusPage.py` & `IntuneCD-1.4.5b2/src/IntuneCD/update_enrollmentStatusPage.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,17 @@
 # Set MS Graph endpoint
 ENDPOINT = (
     "https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations"
 )
 APP_ENDPOINT = "https://graph.microsoft.com/beta/deviceAppManagement/mobileApps"
 
 
-def update(path, token, assignment=False, report=False, create_groups=False):
+def update(
+    path, token, assignment=False, report=False, create_groups=False, remove=False
+):
     """
     This function updates all Windows Enrollment Status Page Profiles in Intune,
     if the configuration in Intune differs from the JSON/YAML file.
 
     :param path: Path to where the backup is saved
     :param token: Token to use for authenticating the request
     :param assignment: Boolean to determine if assignments should be updated
@@ -183,15 +185,15 @@
                             )
                         print(
                             "Enrollment Status Page profile created with id: "
                             + post_request["id"]
                         )
 
         # If any ESP are left in mem_data, remove them from Intune as they are not in the repo
-        if mem_data.get("value", None) is not None:
+        if mem_data.get("value", None) is not None and remove is True:
             for val in mem_data["value"]:
                 if val["displayName"] == "All users and all devices":
                     continue
                 if (
                     val["@odata.type"]
                     == "#microsoft.graph.windowsEnrollmentStatusPageConfiguration"
                 ):
```

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/update_frontend.py` & `IntuneCD-1.4.5b2/src/IntuneCD/update_frontend.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/update_groupPolicyConfiguration.py` & `IntuneCD-1.4.5b2/src/IntuneCD/update_groupPolicyConfiguration.py`

 * *Files 0% similar despite different names*

```diff
@@ -345,15 +345,17 @@
                                     None,
                                     token,
                                 )
 
     return diff_summary
 
 
-def update(path, token, assignment=False, report=False, create_groups=False):
+def update(
+    path, token, assignment=False, report=False, create_groups=False, remove=False
+):
     """
     This function updates all Group Policy configurations in Intune,
     if the configuration in Intune differs from the JSON/YAML file.
 
     :param path: Path to where the backup is saved
     :param token: Token to use for authenticating the request
     :param assignment: Boolean to determine if assignments should be updated
@@ -567,15 +569,15 @@
                         )
                     print(
                         "Group Policy Configuration created with id: "
                         + post_request["id"]
                     )
 
         # If any Group Policy Configuration are left in mem_configs, remove them from Intune as they are not in the repo
-        if mem_configs is not None:
+        if mem_configs is not None and remove is True:
             for val in mem_configs:
                 print("-" * 90)
                 print(
                     "Removing Group Policy Configuration from Intune: "
                     + val["displayName"]
                 )
                 if report is False:
```

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/update_managementIntents.py` & `IntuneCD-1.4.5b2/src/IntuneCD/update_managementIntents.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 from .load_file import load_file
 from .diff_summary import DiffSummary
 
 # Set MS Graph base endpoint
 BASE_ENDPOINT = "https://graph.microsoft.com/beta/deviceManagement"
 
 
-def update(path, token, assignment=False, report=False, create_groups=False):
+def update(
+    path, token, assignment=False, report=False, create_groups=False, remove=False
+):
     """
     This function updates all Endpoint Security configurations (intents) in Intune,
     if the configuration in Intune differs from the JSON/YAML file.
 
     :param path: Path to where the backup is saved
     :param token: Token to use for authenticating the request
     :param assignment: Boolean to determine if assignments should be updated
@@ -195,15 +197,15 @@
                                 "assign",
                                 token,
                                 status_code=204,
                             )
                         print("Intent created with id: " + post_request["id"])
 
         # If any Intents are left in intent_responses, remove them from Intune as they are not in the repo
-        if intent_responses.get("value", None) is not None:
+        if intent_responses.get("value", None) is not None and remove is True:
             for val in intent_responses["value"]:
                 print("-" * 90)
                 print("Removing Management Intent from Intune: " + val["displayName"])
                 if report is False:
                     makeapirequestDelete(
                         f"{BASE_ENDPOINT}/intents/{val['id']}", token, status_code=200
                     )
```

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/update_notificationTemplate.py` & `IntuneCD-1.4.5b2/src/IntuneCD/update_notificationTemplate.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 # Set MS Graph endpoint
 ENDPOINT = (
     "https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates"
 )
 
 
-def update(path, token, report):
+def update(path, token, report, remove):
     """
     This function updates all Notification Templates in Intune,
     if the configuration in Intune differs from the JSON/YAML file.
 
     :param path: Path to where the backup is saved
     :param token: Token to use for authenticating the request
     """
@@ -174,15 +174,15 @@
                             )
                         print(
                             "Notification template created with id: "
                             + template_post_request["id"]
                         )
 
         # If any Notification Template are left in mem_data, remove them from Intune as they are not in the repo
-        if mem_data.get("value", None) is not None:
+        if mem_data.get("value", None) is not None and remove is True:
             for val in mem_data["value"]:
                 if val["displayName"] == "EnrollmentNotificationInternalMEO":
                     continue
                 print("-" * 90)
                 print(
                     "Removing Notification template from Intune: " + val["displayName"]
                 )
```

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/update_powershellScripts.py` & `IntuneCD-1.4.5b2/src/IntuneCD/update_powershellScripts.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,17 @@
 from .remove_keys import remove_keys
 from .diff_summary import DiffSummary
 
 # Set MS Graph endpoint
 ENDPOINT = "https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts"
 
 
-def update(path, token, assignment=False, report=False, create_groups=False):
+def update(
+    path, token, assignment=False, report=False, create_groups=False, remove=False
+):
     """
     This function updates all Powershell scripts in Intune if,
     the configuration in Intune differs from the JSON/YAML file.
 
     :param path: Path to where the backup is saved
     :param token: Token to use for authenticating the request
     :param assignment: Boolean to determine if assignments should be updated
@@ -185,15 +187,15 @@
                                 token,
                             )
                         print(
                             "Powershell script created with id: " + post_request["id"]
                         )
 
         # If any Powershell Scripts are left in mem_powershellScript, remove them from Intune as they are not in the repo
-        if mem_powershellScript.get("value", None) is not None:
+        if mem_powershellScript.get("value", None) is not None and remove is True:
             for val in mem_powershellScript["value"]:
                 print("-" * 90)
                 print("Removing Powershell Script from Intune: " + val["displayName"])
                 if report is False:
                     makeapirequestDelete(
                         f"{ENDPOINT}/{val['id']}", token, status_code=200
                     )
```

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/update_proactiveRemediation.py` & `IntuneCD-1.4.5b2/src/IntuneCD/update_proactiveRemediation.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 from .diff_summary import DiffSummary
 from .clean_filename import clean_filename
 
 # Set MS Graph endpoint
 ENDPOINT = "https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts"
 
 
-def update(path, token, assignment=False, report=False, create_groups=False):
+def update(
+    path, token, assignment=False, report=False, create_groups=False, remove=False
+):
     """
     This function updates all Proactive Remediation in Intune if,
     the configuration in Intune differs from the JSON/YAML file.
 
     :param path: Path to where the backup is saved
     :param token: Token to use for authenticating the request
     :param assignment: Boolean to determine if assignments should be updated
@@ -223,15 +225,15 @@
                             )
                         print(
                             "Proactive Remediation created with id: "
                             + post_request["id"]
                         )
 
         # If any Proactive Remediations are left in mem_proactiveRemediation, remove them from Intune as they are not in the repo
-        if mem_proactiveRemediation.get("value", None) is not None:
+        if mem_proactiveRemediation.get("value", None) is not None and remove is True:
             for val in mem_proactiveRemediation["value"]:
                 if val.get("publisher", None) != "Microsoft":
                     print("-" * 90)
                     print(
                         "Removing Proactive Remediation from Intune: "
                         + val["displayName"]
                     )
```

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/update_profiles.py` & `IntuneCD-1.4.5b2/src/IntuneCD/update_profiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 from .remove_keys import remove_keys
 from .diff_summary import DiffSummary
 
 # Set MS Graph endpoint
 ENDPOINT = "https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations"
 
 
-def update(path, token, assignment=False, report=False, create_groups=False):
+def update(
+    path, token, assignment=False, report=False, create_groups=False, remove=False
+):
     """
     This function updates all Device Configurations in Intune,
     if the configuration in Intune differs from the JSON/YAML file.
 
     :param path: Path to where the backup is saved
     :param token: Token to use for authenticating the request
     :param assignment: Boolean to determine if assignments should be updated
@@ -342,15 +344,15 @@
                                 post_request["id"],
                                 "deviceManagement/deviceConfigurations",
                                 "assign",
                                 token,
                             )
 
         # If any Profiles are left in mem_data, remove them from Intune as they are not in the repo
-        if mem_data.get("value", None) is not None:
+        if mem_data.get("value", None) is not None and remove is True:
             for val in mem_data["value"]:
                 print("-" * 90)
                 print("Removing Profile from Intune: " + val["displayName"])
                 if report is False:
                     makeapirequestDelete(
                         f"{ENDPOINT}/{val['id']}", token, status_code=200
                     )
```

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/update_shellScripts.py` & `IntuneCD-1.4.5b2/src/IntuneCD/update_shellScripts.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,17 @@
 # Set MS Graph endpoint
 ENDPOINT = "https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts"
 ASSIGNMENT_ENDPOINT = (
     "https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts"
 )
 
 
-def update(path, token, assignment=False, report=False, create_groups=False):
+def update(
+    path, token, assignment=False, report=False, create_groups=False, remove=False
+):
     """
     This function updates all Shell scripts in Intune if the configuration in Intune differs from the JSON/YAML file.
 
     :param path: Path to where the backup is saved
     :param token: Token to use for authenticating the request
     :param assignment: Boolean to determine if assignments should be updated
     """
@@ -186,15 +188,15 @@
                                 "deviceManagement/deviceManagementScripts",
                                 "assign",
                                 token,
                             )
                         print("Shell script created with id: " + post_request["id"])
 
         # If any Shell Scripts are left in mem_shellScript, remove them from Intune as they are not in the repo
-        if mem_shellScript.get("value", None) is not None:
+        if mem_shellScript.get("value", None) is not None and remove is True:
             for val in mem_shellScript["value"]:
                 print("-" * 90)
                 print("Removing Shell Script from Intune: " + val["displayName"])
                 if report is False:
                     makeapirequestDelete(
                         f"{ENDPOINT}/{val['id']}", token, status_code=200
                     )
```

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD/update_windowsEnrollmentProfile.py` & `IntuneCD-1.4.5b2/src/IntuneCD/update_windowsEnrollmentProfile.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,17 @@
 from .remove_keys import remove_keys
 from .diff_summary import DiffSummary
 
 # Set MS Graph endpoint
 ENDPOINT = "https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles"
 
 
-def update(path, token, assignment=False, report=False, create_groups=False):
+def update(
+    path, token, assignment=False, report=False, create_groups=False, remove=False
+):
     """
     This function updates all Windows Enrollment Profiles in Intune,
     if the configuration in Intune differs from the JSON/YAML file.
 
     :param path: Path to where the backup is saved
     :param token: Token to use for authenticating the request
     :param assignment: Boolean to determine if assignments should be updated
@@ -152,15 +154,15 @@
                                     status_code=201,
                                 )
                         print(
                             "Autopilot profile created with id: " + post_request["id"]
                         )
 
         # If any Windows Enrollment Profile are left in mem_data, remove them from Intune as they are not in the repo
-        if mem_data.get("value", None) is not None:
+        if mem_data.get("value", None) is not None and remove is True:
             for val in mem_data["value"]:
                 print("-" * 90)
                 print("Removing Autopilot Profile from Intune: " + val["displayName"])
                 if report is False:
                     # Remove assignments so we can delete the profile
                     makeapirequestDelete(
                         f"{ENDPOINT}/{val['id']}/assignments", token, status_code=200
```

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD.egg-info/PKG-INFO` & `IntuneCD-1.4.5b2/src/IntuneCD.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IntuneCD
-Version: 1.4.5b1
+Version: 1.4.5b2
 Summary: Tool to backup and update configurations in Intune
 Home-page: https://github.com/almenscorner/IntuneCD
 Author: Tobias Almén
 Author-email: almenscorner@outlook.com
 Project-URL: Bug Tracker, https://github.com/almenscorner/IntuneCD/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `IntuneCD-1.4.5b1/src/IntuneCD.egg-info/SOURCES.txt` & `IntuneCD-1.4.5b2/src/IntuneCD.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/tests/test_archive.py` & `IntuneCD-1.4.5b2/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/tests/test_check_file.py` & `IntuneCD-1.4.5b2/tests/test_check_file.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/tests/test_clean_filename.py` & `IntuneCD-1.4.5b2/tests/test_clean_filename.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/tests/test_diff_summary.py` & `IntuneCD-1.4.5b2/tests/test_diff_summary.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/tests/test_documentation_functions.py` & `IntuneCD-1.4.5b2/tests/test_documentation_functions.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/tests/test_get_added_removed.py` & `IntuneCD-1.4.5b2/tests/test_get_added_removed.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/tests/test_get_authparams.py` & `IntuneCD-1.4.5b2/tests/test_get_authparams.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/tests/test_graph_batch.py` & `IntuneCD-1.4.5b2/tests/test_graph_batch.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/tests/test_graph_request.py` & `IntuneCD-1.4.5b2/tests/test_graph_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,18 +4,31 @@
 This module tests the graph_request module.
 """
 
 import unittest
 
 from unittest import mock
 from unittest.mock import patch
-from src.IntuneCD.graph_request import makeapirequest, makeapirequestPost, makeapirequestPut, makeapirequestPatch
-
-
-def _mock_response(self, status=200, content="CONTENT", json_data=None, raise_for_status=None, headers={}):
+from src.IntuneCD.graph_request import (
+    makeapirequest,
+    makeapirequestPost,
+    makeapirequestPut,
+    makeapirequestPatch,
+    makeapirequestDelete,
+)
+
+
+def _mock_response(
+    self,
+    status=200,
+    content="CONTENT",
+    json_data=None,
+    raise_for_status=None,
+    headers={},
+):
     """Mock the response from the requests library."""
 
     mock_resp = mock.Mock()
     # mock raise_for_status call w/optional error
     mock_resp.raise_for_status = mock.Mock()
     if raise_for_status:
         mock_resp.raise_for_status.side_effect = raise_for_status
@@ -32,134 +45,178 @@
 @patch("time.sleep", return_value=None)
 class TestGraphRequestGet(unittest.TestCase):
     """Test class for graph_request."""
 
     def setUp(self):
         self.token = {"access_token": "token"}
 
-    def test_makeapirequest_status_429_no_q_param(self, mock_sleep, mock_get, mock_makeapirequest):
+    def test_makeapirequest_status_429_no_q_param(
+        self, mock_sleep, mock_get, mock_makeapirequest
+    ):
         """The request should be made once and exception should be raised."""
         with self.assertRaises(Exception):
-            self.mock_resp = _mock_response(self, status=429, content="Too Many equests", headers={"Retry-After": "10"})
+            self.mock_resp = _mock_response(
+                self,
+                status=429,
+                content="Too Many equests",
+                headers={"Retry-After": "10"},
+            )
             self.mock_resp2 = _mock_response(self, status=200, content="Success")
             mock_get.side_effect = self.mock_resp, self.mock_resp2
             makeapirequest("https://endpoint", self.token)
 
         self.assertEqual(2, mock_get.call_count)
 
-    def test_makeapirequest_status_429_with_q_param(self, mock_sleep, mock_get, mock_makeapirequest):
+    def test_makeapirequest_status_429_with_q_param(
+        self, mock_sleep, mock_get, mock_makeapirequest
+    ):
         """The request should be made once and exception should be raised."""
         with self.assertRaises(Exception):
-            self.mock_resp = _mock_response(self, status=429, content="Too Many Requests", headers={"Retry-After": "10"})
+            self.mock_resp = _mock_response(
+                self,
+                status=429,
+                content="Too Many Requests",
+                headers={"Retry-After": "10"},
+            )
             self.mock_resp2 = _mock_response(self, status=200, content="Success")
             mock_get.side_effect = self.mock_resp, self.mock_resp2
             makeapirequest("https://endpoint", self.token, q_param="$filter=id eq '0'")
 
         self.assertEqual(2, mock_get.call_count)
 
     def test_makeapirequest_no_q_param(self, mock_sleep, mock_get, mock_makeapirequest):
         """The request should be made once and the response should be returned."""
-        self.mock_resp = _mock_response(self, status=200, content='{"value": [{"id": "0"}]}')
+        self.mock_resp = _mock_response(
+            self, status=200, content='{"value": [{"id": "0"}]}'
+        )
         mock_get.return_value = self.mock_resp
         self.result = makeapirequest("https://endpoint", self.token)
         self.assertEqual(self.result, {"value": [{"id": "0"}]})
 
-    def test_makeapirequest_status_502_no_q_param(self, mock_sleep, mock_get, mock_makeapirequest):
+    def test_makeapirequest_status_502_no_q_param(
+        self, mock_sleep, mock_get, mock_makeapirequest
+    ):
         """The request should be made twice and exception should be raised."""
         with self.assertRaises(Exception):
             self.mock_resp = _mock_response(self, status=502, content="request timeout")
             mock_get.return_value = self.mock_resp
             makeapirequest("https://endpoint", self.token)
 
         self.assertEqual(2, mock_get.call_count)
 
-    def test_makeapirequest_status_503_no_q_param(self, mock_sleep, mock_get, mock_makeapirequest):
+    def test_makeapirequest_status_503_no_q_param(
+        self, mock_sleep, mock_get, mock_makeapirequest
+    ):
         """The request should be made twice and exception should be raised."""
         with self.assertRaises(Exception):
             self.mock_resp = _mock_response(self, status=503, content="request timeout")
             mock_get.return_value = self.mock_resp
             makeapirequest("https://endpoint", self.token)
 
         self.assertEqual(2, mock_get.call_count)
 
-    def test_makeapirequest_status_504_no_q_param(self, mock_sleep, mock_get, mock_makeapirequest):
+    def test_makeapirequest_status_504_no_q_param(
+        self, mock_sleep, mock_get, mock_makeapirequest
+    ):
         """The request should be made twice and exception should be raised."""
         with self.assertRaises(Exception):
             self.mock_resp = _mock_response(self, status=504, content="request timeout")
             mock_get.return_value = self.mock_resp
             makeapirequest("https://endpoint", self.token)
 
         self.assertEqual(2, mock_get.call_count)
 
-    def test_makeapirequest_with_q_param(self, mock_sleep, mock_get, mock_makeapirequest):
+    def test_makeapirequest_with_q_param(
+        self, mock_sleep, mock_get, mock_makeapirequest
+    ):
         """The request should be made once and the response should be returned."""
-        self.mock_resp = _mock_response(self, status=200, content='{"value": [{"id": "0"}]}')
+        self.mock_resp = _mock_response(
+            self, status=200, content='{"value": [{"id": "0"}]}'
+        )
         mock_get.return_value = self.mock_resp
-        self.result = makeapirequest("https://endpoint", self.token, q_param="$filter=id eq '0'")
+        self.result = makeapirequest(
+            "https://endpoint", self.token, q_param="$filter=id eq '0'"
+        )
         self.assertEqual(self.result, {"value": [{"id": "0"}]})
 
-    def test_makeapirequest_status_502_with_q_param(self, mock_sleep, mock_get, mock_makeapirequest):
+    def test_makeapirequest_status_502_with_q_param(
+        self, mock_sleep, mock_get, mock_makeapirequest
+    ):
         """The request should be made twice and exception should be raised."""
         with self.assertRaises(Exception):
             self.mock_resp = _mock_response(self, status=502, content="request timeout")
             mock_get.return_value = self.mock_resp
             makeapirequest("https://endpoint", self.token, q_param="$filter=id eq '0'")
 
         self.assertEqual(2, mock_get.call_count)
 
-    def test_makeapirequest_status_503_with_q_param(self, mock_sleep, mock_get, mock_makeapirequest):
+    def test_makeapirequest_status_503_with_q_param(
+        self, mock_sleep, mock_get, mock_makeapirequest
+    ):
         """The request should be made twice and exception should be raised."""
         with self.assertRaises(Exception):
             self.mock_resp = _mock_response(self, status=503, content="request timeout")
             mock_get.return_value = self.mock_resp
             makeapirequest("https://endpoint", self.token, q_param="$filter=id eq '0'")
 
         self.assertEqual(2, mock_get.call_count)
 
-    def test_makeapirequest_status_504_with_q_param(self, mock_sleep, mock_get, mock_makeapirequest):
+    def test_makeapirequest_status_504_with_q_param(
+        self, mock_sleep, mock_get, mock_makeapirequest
+    ):
         """The request should be made twice and exception should be raised."""
         with self.assertRaises(Exception):
             self.mock_resp = _mock_response(self, status=504, content="request timeout")
             mock_get.return_value = self.mock_resp
             makeapirequest("https://endpoint", self.token, q_param="$filter=id eq '0'")
 
         self.assertEqual(2, mock_get.call_count)
 
-    def test_makeapirequest_odata_nextlink(self, mock_sleep, mock_get, mock_makeapirequest):
+    def test_makeapirequest_odata_nextlink(
+        self, mock_sleep, mock_get, mock_makeapirequest
+    ):
         """The request should be made and the response should contain next link values."""
         self.NEXT_LINK_VALUE = {"value": [{"id": "1"}]}
         mock_makeapirequest.return_value = self.NEXT_LINK_VALUE
         self.mock_resp = _mock_response(
-            self, status=200, content='{"value": [{"id": "0"}], "@odata.nextLink": "https://endpoint"}'
+            self,
+            status=200,
+            content='{"value": [{"id": "0"}], "@odata.nextLink": "https://endpoint"}',
         )
         mock_get.return_value = self.mock_resp
         self.result = makeapirequest("https://endpoint", self.token)
 
         self.assertEqual(self.result["value"], [{"id": "0"}, {"id": "1"}])
 
     def test_makeapirequest_status_404(self, mock_sleep, mock_get, mock_makeapirequest):
         """The request should be made and the response should be returned."""
         self.mock_resp = _mock_response(self, status=404, content="not found")
         mock_get.return_value = self.mock_resp
         makeapirequest("https://endpoint", self.token)
 
         self.assertEqual(1, mock_get.call_count)
 
-    def test_makeapirequest_assignmentfilter_not_enabled(self, mock_sleep, mock_get, mock_makeapirequest):
+    def test_makeapirequest_assignmentfilter_not_enabled(
+        self, mock_sleep, mock_get, mock_makeapirequest
+    ):
         """The request should be made and assignment filters should be skipped."""
-        self.mock_resp = _mock_response(self, status=500, content='{"FeatureNotEnabled": []}')
+        self.mock_resp = _mock_response(
+            self, status=500, content='{"FeatureNotEnabled": []}'
+        )
         mock_get.return_value = self.mock_resp
         makeapirequest("https://endpoint/assignmentFilters", self.token)
 
         self.assertEqual(1, mock_get.call_count)
 
     def test_makeapirequest_exception(self, mock_sleep, mock_get, mock_makeapirequest):
         """The request should be made and exception should be raised."""
         with self.assertRaises(Exception):
-            self.mock_resp = _mock_response(self, status=500, content="Internal Server Error")
+            self.mock_resp = _mock_response(
+                self, status=500, content="Internal Server Error"
+            )
             mock_get.return_value = self.mock_resp
             makeapirequest("https://endpoint/", self.token)
 
         self.assertEqual(1, mock_get.call_count)
 
 
 @patch("src.IntuneCD.graph_request.makeapirequestPatch")
@@ -168,33 +225,48 @@
     def setUp(self):
         self.token = {"access_token": "token"}
 
     def test_makeapirequestPatch_no_q_param(self, mock_patch, mock_makeapirequestPatch):
         """The request should be made and the response should be returned."""
         self.mock_resp = _mock_response(self, status=200, content="")
         mock_patch.return_value = self.mock_resp
-        result = makeapirequestPatch("https://endpoint", self.token, q_param=None, jdata='{"id": "0"}')
+        result = makeapirequestPatch(
+            "https://endpoint", self.token, q_param=None, jdata='{"id": "0"}'
+        )
 
         self.assertEqual(result, None)
 
-    def test_makeapirequestPatch_with_q_param(self, mock_patch, mock_makeapirequestPatch):
+    def test_makeapirequestPatch_with_q_param(
+        self, mock_patch, mock_makeapirequestPatch
+    ):
         """The request should be made and the response should be returned."""
         self.mock_resp = _mock_response(self, status=200, content="")
         mock_patch.return_value = self.mock_resp
-        self.result = makeapirequestPatch("https://endpoint", self.token, q_param="$filter=id eq '0'", jdata='{"id": "0"}')
+        self.result = makeapirequestPatch(
+            "https://endpoint",
+            self.token,
+            q_param="$filter=id eq '0'",
+            jdata='{"id": "0"}',
+        )
 
         self.assertEqual(self.result, None)
 
-    def test_makeapirequestPatch_not_matching_status_code(self, mock_patch, mock_makeapirequestPatch):
+    def test_makeapirequestPatch_not_matching_status_code(
+        self, mock_patch, mock_makeapirequestPatch
+    ):
         """The request should be made and the response should be returned."""
         with self.assertRaises(Exception):
             self.mock_resp = _mock_response(self, status=204, content="")
             mock_patch.return_value = self.mock_resp
             makeapirequestPatch(
-                "https://endpoint", self.token, q_param="$filter=id eq '0'", jdata='{"id": "0"}', status_code=200
+                "https://endpoint",
+                self.token,
+                q_param="$filter=id eq '0'",
+                jdata='{"id": "0"}',
+                status_code=200,
             )
 
         self.assertEqual(1, mock_patch.call_count)
 
 
 @patch("src.IntuneCD.graph_request.makeapirequestPost")
 @patch("requests.post")
@@ -202,88 +274,178 @@
 class TestGraphRequestPost(unittest.TestCase):
     def setUp(self):
         self.token = {"access_token": "token"}
         self.jdata = {"id": "0"}
         self.content = '{"id": "0"}'
         self.expected_result = {"id": "0"}
 
-
-    def test_makeapirequestPost_status_429_no_q_param(self, mock_sleep, mock_patch, mock_makeapirequestPost):
+    def test_makeapirequestPost_status_429_no_q_param(
+        self, mock_sleep, mock_patch, mock_makeapirequestPost
+    ):
         """The request should be made twice."""
-        self.mock_resp = _mock_response(self, status=429, content="Too Many equests", headers={"Retry-After": "10"})
+        self.mock_resp = _mock_response(
+            self, status=429, content="Too Many equests", headers={"Retry-After": "10"}
+        )
         self.mock_resp2 = _mock_response(self, status=200, content="Success")
         mock_patch.side_effect = self.mock_resp, self.mock_resp2
         makeapirequestPost("https://endpoint", self.token)
 
         self.assertEqual(2, mock_patch.call_count)
 
-    def test_makeapirequestPost_status_429_with_q_param(self, mock_sleep, mock_patch, mock_makeapirequestPost):
+    def test_makeapirequestPost_status_429_with_q_param(
+        self, mock_sleep, mock_patch, mock_makeapirequestPost
+    ):
         """The request should be made twice."""
-        self.mock_resp = _mock_response(self, status=429, content="Too Many Requests", headers={"Retry-After": "10"})
+        self.mock_resp = _mock_response(
+            self, status=429, content="Too Many Requests", headers={"Retry-After": "10"}
+        )
         self.mock_resp2 = _mock_response(self, status=200, content="Success")
         mock_patch.side_effect = self.mock_resp, self.mock_resp2
         makeapirequestPost("https://endpoint", self.token, q_param="$filter=id eq '0'")
 
         self.assertEqual(2, mock_patch.call_count)
 
-    def test_makeapirequestPost_no_q_param(self, mock_sleep, mock_patch, mock_makeapirequestPost):
+    def test_makeapirequestPost_no_q_param(
+        self, mock_sleep, mock_patch, mock_makeapirequestPost
+    ):
         """The request should be made and the response should be returned."""
         self.mock_resp = _mock_response(self, status=200, content=self.content)
         mock_patch.return_value = self.mock_resp
-        self.result = makeapirequestPost("https://endpoint", self.token, q_param=None, jdata=self.jdata)
+        self.result = makeapirequestPost(
+            "https://endpoint", self.token, q_param=None, jdata=self.jdata
+        )
 
         self.assertEqual(self.result, self.expected_result)
 
-    def test_makeapirequestPost_with_q_param(self, mock_sleep, mock_patch, mock_makeapirequestPost):
+    def test_makeapirequestPost_with_q_param(
+        self, mock_sleep, mock_patch, mock_makeapirequestPost
+    ):
         """The request should be made and the response should be returned."""
         self.mock_resp = _mock_response(self, status=200, content=self.content)
         mock_patch.return_value = self.mock_resp
-        self.result = makeapirequestPost("https://endpoint", self.token, q_param="$filter=id eq '0'", jdata=self.jdata)
+        self.result = makeapirequestPost(
+            "https://endpoint",
+            self.token,
+            q_param="$filter=id eq '0'",
+            jdata=self.jdata,
+        )
 
         self.assertEqual(self.result, self.expected_result)
 
-    def test_makeapirequestPost_not_matching_status_code(self, mock_sleep, mock_patch, mock_makeapirequestPost):
+    def test_makeapirequestPost_not_matching_status_code(
+        self, mock_sleep, mock_patch, mock_makeapirequestPost
+    ):
         """The request should be made and the response should be returned."""
         with self.assertRaises(Exception):
             self.mock_resp = _mock_response(self, status=204, content="")
             mock_patch.return_value = self.mock_resp
-            makeapirequestPost("https://endpoint", self.token, q_param="$filter=id eq '0'", jdata=self.jdata, status_code=200)
+            makeapirequestPost(
+                "https://endpoint",
+                self.token,
+                q_param="$filter=id eq '0'",
+                jdata=self.jdata,
+                status_code=200,
+            )
 
         self.assertEqual(1, mock_patch.call_count)
 
 
 @patch("src.IntuneCD.graph_request.makeapirequestPut")
 @patch("requests.put")
 class TestGraphRequestPut(unittest.TestCase):
     def setUp(self):
         self.token = {"access_token": "token"}
 
     def test_makeapirequestPut_no_q_param(self, mock_patch, mock_makeapirequestPut):
         """The request should be made and the response should be returned."""
         self.mock_resp = _mock_response(self, status=200, content="")
         mock_patch.return_value = self.mock_resp
-        self.result = makeapirequestPut("https://endpoint", self.token, q_param=None, jdata='{"id": "0"}')
+        self.result = makeapirequestPut(
+            "https://endpoint", self.token, q_param=None, jdata='{"id": "0"}'
+        )
 
         self.assertEqual(self.result, None)
 
     def test_makeapirequestPut_with_q_param(self, mock_patch, mock_makeapirequestPut):
         """The request should be made and the response should be returned."""
         self.mock_resp = _mock_response(self, status=200, content="")
         mock_patch.return_value = self.mock_resp
-        self.result = makeapirequestPut("https://endpoint", self.token, q_param="$filter=id eq '0'", jdata='{"id": "0"}')
+        self.result = makeapirequestPut(
+            "https://endpoint",
+            self.token,
+            q_param="$filter=id eq '0'",
+            jdata='{"id": "0"}',
+        )
 
         self.assertEqual(self.result, None)
 
-    def test_makeapirequestPut_not_matching_status_code(self, mock_patch, mock_makeapirequestPut):
+    def test_makeapirequestPut_not_matching_status_code(
+        self, mock_patch, mock_makeapirequestPut
+    ):
         """The request should be made and the response should be returned."""
         with self.assertRaises(Exception):
             self.mock_resp = _mock_response(self, status=204, content="")
             mock_patch.return_value = self.mock_resp
             makeapirequestPut(
-                "https://endpoint", self.token, q_param="$filter=id eq '0'", jdata='{"id": "0"}', status_code=200
+                "https://endpoint",
+                self.token,
+                q_param="$filter=id eq '0'",
+                jdata='{"id": "0"}',
+                status_code=200,
+            )
+
+        self.assertEqual(1, mock_patch.call_count)
+
+
+@patch("src.IntuneCD.graph_request.makeapirequestDelete")
+@patch("requests.delete")
+class TestGraphRequestDelete(unittest.TestCase):
+    def setUp(self):
+        self.token = {"access_token": "token"}
+
+    def test_makeapirequestDelete_no_q_param(
+        self, mock_patch, mock_makeapirequestDelete
+    ):
+        """The request should be made and the response should be returned."""
+        self.mock_resp = _mock_response(self, status=200, content="")
+        mock_patch.return_value = self.mock_resp
+        self.result = makeapirequestDelete(
+            "https://endpoint", self.token, q_param=None, jdata='{"id": "0"}'
+        )
+
+        self.assertEqual(self.result, None)
+
+    def test_makeapirequestDelete_with_q_param(
+        self, mock_patch, mock_makeapirequestDelete
+    ):
+        """The request should be made and the response should be returned."""
+        self.mock_resp = _mock_response(self, status=200, content="")
+        mock_patch.return_value = self.mock_resp
+        self.result = makeapirequestDelete(
+            "https://endpoint",
+            self.token,
+            q_param="$filter=id eq '0'",
+            jdata='{"id": "0"}',
+        )
+
+        self.assertEqual(self.result, None)
+
+    def test_makeapirequestDelete_not_matching_status_code(
+        self, mock_patch, mock_makeapirequestDelete
+    ):
+        """The request should be made and the response should be returned."""
+        with self.assertRaises(Exception):
+            self.mock_resp = _mock_response(self, status=204, content="")
+            mock_patch.return_value = self.mock_resp
+            makeapirequestDelete(
+                "https://endpoint",
+                self.token,
+                q_param="$filter=id eq '0'",
+                jdata='{"id": "0"}',
+                status_code=200,
             )
 
         self.assertEqual(1, mock_patch.call_count)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `IntuneCD-1.4.5b1/tests/test_group_report.py` & `IntuneCD-1.4.5b2/tests/test_group_report.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/tests/test_load_file.py` & `IntuneCD-1.4.5b2/tests/test_load_file.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/tests/test_match.py` & `IntuneCD-1.4.5b2/tests/test_match.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/tests/test_remove_keys.py` & `IntuneCD-1.4.5b2/tests/test_remove_keys.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/tests/test_save_output.py` & `IntuneCD-1.4.5b2/tests/test_save_output.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.5b1/tests/test_update_frontend.py` & `IntuneCD-1.4.5b2/tests/test_update_frontend.py`

 * *Files identical despite different names*

