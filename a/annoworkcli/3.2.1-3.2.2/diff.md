# Comparing `tmp/annoworkcli-3.2.1.tar.gz` & `tmp/annoworkcli-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "annoworkcli-3.2.1.tar", max compression
+gzip compressed data, was "annoworkcli-3.2.2.tar", max compression
```

## Comparing `annoworkcli-3.2.1.tar` & `annoworkcli-3.2.2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0     2244 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/README.md
--rw-r--r--   0        0        0       71 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/__init__.py
--rw-r--r--   0        0        0     2496 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/__main__.py
--rw-r--r--   0        0        0       22 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/__version__.py
--rw-r--r--   0        0        0        0 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/account/__init__.py
--rw-r--r--   0        0        0     2901 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/account/list_external_linkage_info.py
--rw-r--r--   0        0        0     2398 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/account/put_external_linkage_info.py
--rw-r--r--   0        0        0      879 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/account/subcommand.py
--rw-r--r--   0        0        0        0 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/actual_working_time/__init__.py
--rw-r--r--   0        0        0     7614 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/actual_working_time/delete_actual_working_time.py
--rw-r--r--   0        0        0    14541 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/actual_working_time/list_actual_working_hours_daily.py
--rw-r--r--   0        0        0    13292 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/actual_working_time/list_actual_working_hours_daily_groupby_tag.py
--rw-r--r--   0        0        0    15229 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/actual_working_time/list_actual_working_time.py
--rw-r--r--   0        0        0     1408 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/actual_working_time/subcommand.py
--rw-r--r--   0        0        0        0 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/annofab/__init__.py
--rw-r--r--   0        0        0     8540 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/annofab/list_job_with_annofab_project.py
--rw-r--r--   0        0        0    22039 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/annofab/list_working_hours.py
--rw-r--r--   0        0        0     5210 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/annofab/put_account_external_linkage_info.py
--rw-r--r--   0        0        0     3953 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/annofab/put_job_from_annofab_project.py
--rw-r--r--   0        0        0    51720 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/annofab/reshape_working_hours.py
--rw-r--r--   0        0        0     1515 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/annofab/subcommand.py
--rw-r--r--   0        0        0    11287 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/annofab/visualize_statistics.py
--rw-r--r--   0        0        0        0 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/common/__init__.py
--rw-r--r--   0        0        0      846 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/common/annofab.py
--rw-r--r--   0        0        0     9053 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/common/cli.py
--rw-r--r--   0        0        0       92 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/common/exeptions.py
--rw-r--r--   0        0        0       78 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/common/job.py
--rw-r--r--   0        0        0     4364 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/common/utils.py
--rw-r--r--   0        0        0      923 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/common/workspace_tag.py
--rw-r--r--   0        0        0      829 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/data/logging.yaml
--rw-r--r--   0        0        0        0 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/expected_working_time/__init__.py
--rw-r--r--   0        0        0     3858 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/expected_working_time/delete_expected_working_time.py
--rw-r--r--   0        0        0     6739 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/expected_working_time/list_expected_working_time.py
--rw-r--r--   0        0        0     8777 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/expected_working_time/list_expected_working_time_groupby_tag.py
--rw-r--r--   0        0        0     5351 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/expected_working_time/list_expected_working_time_weekly.py
--rw-r--r--   0        0        0     1296 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/expected_working_time/subcommand.py
--rw-r--r--   0        0        0        0 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/job/__init__.py
--rw-r--r--   0        0        0     4038 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/job/change_job_properties.py
--rw-r--r--   0        0        0     3326 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/job/delete_job.py
--rw-r--r--   0        0        0     6284 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/job/list_job.py
--rw-r--r--   0        0        0      885 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/job/subcommand.py
--rw-r--r--   0        0        0        0 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/my/__init__.py
--rw-r--r--   0        0        0     1404 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/my/get_my_account.py
--rw-r--r--   0        0        0     2361 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/my/list_my_workspace_member.py
--rw-r--r--   0        0        0      816 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/my/subcommand.py
--rw-r--r--   0        0        0        0 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/schedule/__init__.py
--rw-r--r--   0        0        0     8172 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/schedule/list_assigned_hours_daily.py
--rw-r--r--   0        0        0     9204 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/schedule/list_assigned_hours_daily_groupby_tag.py
--rw-r--r--   0        0        0    11024 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/schedule/list_schedule.py
--rw-r--r--   0        0        0      995 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/schedule/subcommand.py
--rw-r--r--   0        0        0     3276 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/workspace/list_workspace.py
--rw-r--r--   0        0        0     2141 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/workspace/put_workspace.py
--rw-r--r--   0        0        0      847 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/workspace/subcommand.py
--rw-r--r--   0        0        0        0 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/workspace_member/__init__.py
--rw-r--r--   0        0        0     5048 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/workspace_member/append_tag_to_workspace_member.py
--rw-r--r--   0        0        0     4601 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/workspace_member/change_workspace_member_properties.py
--rw-r--r--   0        0        0     2897 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/workspace_member/delete_workspace_member.py
--rw-r--r--   0        0        0     6248 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/workspace_member/list_workspace_member.py
--rw-r--r--   0        0        0     4725 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/workspace_member/put_workspace_member.py
--rw-r--r--   0        0        0     5079 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/workspace_member/remove_tag_to_workspace_member.py
--rw-r--r--   0        0        0     1518 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/workspace_member/subcommand.py
--rw-r--r--   0        0        0        0 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/workspace_tag/__init__.py
--rw-r--r--   0        0        0     2645 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/workspace_tag/list_workspace_tag.py
--rw-r--r--   0        0        0     2576 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/workspace_tag/put_workspace_tag.py
--rw-r--r--   0        0        0      877 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/workspace_tag/subcommand.py
--rw-r--r--   0        0        0     1907 2023-05-01 06:29:38.436617 annoworkcli-3.2.1/pyproject.toml
--rw-r--r--   0        0        0     3332 1970-01-01 00:00:00.000000 annoworkcli-3.2.1/PKG-INFO
+-rw-r--r--   0        0        0     2107 2023-05-16 06:21:08.479328 annoworkcli-3.2.2/README.md
+-rw-r--r--   0        0        0       71 2023-05-16 06:21:08.479328 annoworkcli-3.2.2/annoworkcli/__init__.py
+-rw-r--r--   0        0        0     2496 2023-05-16 06:21:08.479328 annoworkcli-3.2.2/annoworkcli/__main__.py
+-rw-r--r--   0        0        0      131 2023-05-16 06:21:23.923590 annoworkcli-3.2.2/annoworkcli/__version__.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:21:08.479328 annoworkcli-3.2.2/annoworkcli/account/__init__.py
+-rw-r--r--   0        0        0     2901 2023-05-16 06:21:08.479328 annoworkcli-3.2.2/annoworkcli/account/list_external_linkage_info.py
+-rw-r--r--   0        0        0     2398 2023-05-16 06:21:08.479328 annoworkcli-3.2.2/annoworkcli/account/put_external_linkage_info.py
+-rw-r--r--   0        0        0      879 2023-05-16 06:21:08.479328 annoworkcli-3.2.2/annoworkcli/account/subcommand.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:21:08.479328 annoworkcli-3.2.2/annoworkcli/actual_working_time/__init__.py
+-rw-r--r--   0        0        0     7614 2023-05-16 06:21:08.479328 annoworkcli-3.2.2/annoworkcli/actual_working_time/delete_actual_working_time.py
+-rw-r--r--   0        0        0    14541 2023-05-16 06:21:08.479328 annoworkcli-3.2.2/annoworkcli/actual_working_time/list_actual_working_hours_daily.py
+-rw-r--r--   0        0        0    13292 2023-05-16 06:21:08.479328 annoworkcli-3.2.2/annoworkcli/actual_working_time/list_actual_working_hours_daily_groupby_tag.py
+-rw-r--r--   0        0        0    15229 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/actual_working_time/list_actual_working_time.py
+-rw-r--r--   0        0        0     1408 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/actual_working_time/subcommand.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/annofab/__init__.py
+-rw-r--r--   0        0        0     8540 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/annofab/list_job_with_annofab_project.py
+-rw-r--r--   0        0        0    22039 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/annofab/list_working_hours.py
+-rw-r--r--   0        0        0     5210 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/annofab/put_account_external_linkage_info.py
+-rw-r--r--   0        0        0     3953 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/annofab/put_job_from_annofab_project.py
+-rw-r--r--   0        0        0    51720 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/annofab/reshape_working_hours.py
+-rw-r--r--   0        0        0     1515 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/annofab/subcommand.py
+-rw-r--r--   0        0        0    11287 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/annofab/visualize_statistics.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/common/__init__.py
+-rw-r--r--   0        0        0      846 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/common/annofab.py
+-rw-r--r--   0        0        0     9053 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/common/cli.py
+-rw-r--r--   0        0        0       92 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/common/exeptions.py
+-rw-r--r--   0        0        0       78 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/common/job.py
+-rw-r--r--   0        0        0     4364 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/common/utils.py
+-rw-r--r--   0        0        0      923 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/common/workspace_tag.py
+-rw-r--r--   0        0        0      829 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/data/logging.yaml
+-rw-r--r--   0        0        0        0 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/expected_working_time/__init__.py
+-rw-r--r--   0        0        0     3858 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/expected_working_time/delete_expected_working_time.py
+-rw-r--r--   0        0        0     6739 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/expected_working_time/list_expected_working_time.py
+-rw-r--r--   0        0        0     8777 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/expected_working_time/list_expected_working_time_groupby_tag.py
+-rw-r--r--   0        0        0     5351 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/expected_working_time/list_expected_working_time_weekly.py
+-rw-r--r--   0        0        0     1296 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/expected_working_time/subcommand.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/job/__init__.py
+-rw-r--r--   0        0        0     4038 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/job/change_job_properties.py
+-rw-r--r--   0        0        0     3326 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/job/delete_job.py
+-rw-r--r--   0        0        0     6284 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/job/list_job.py
+-rw-r--r--   0        0        0      885 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/job/subcommand.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/my/__init__.py
+-rw-r--r--   0        0        0     1404 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/my/get_my_account.py
+-rw-r--r--   0        0        0     2361 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/my/list_my_workspace_member.py
+-rw-r--r--   0        0        0      816 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/my/subcommand.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/schedule/__init__.py
+-rw-r--r--   0        0        0     8172 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/schedule/list_assigned_hours_daily.py
+-rw-r--r--   0        0        0     9204 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/schedule/list_assigned_hours_daily_groupby_tag.py
+-rw-r--r--   0        0        0    11024 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/schedule/list_schedule.py
+-rw-r--r--   0        0        0      995 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/schedule/subcommand.py
+-rw-r--r--   0        0        0     3276 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/workspace/list_workspace.py
+-rw-r--r--   0        0        0     2141 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/workspace/put_workspace.py
+-rw-r--r--   0        0        0      847 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/workspace/subcommand.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/workspace_member/__init__.py
+-rw-r--r--   0        0        0     5048 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/workspace_member/append_tag_to_workspace_member.py
+-rw-r--r--   0        0        0     4601 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/workspace_member/change_workspace_member_properties.py
+-rw-r--r--   0        0        0     2897 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/workspace_member/delete_workspace_member.py
+-rw-r--r--   0        0        0     6248 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/workspace_member/list_workspace_member.py
+-rw-r--r--   0        0        0     4725 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/workspace_member/put_workspace_member.py
+-rw-r--r--   0        0        0     5079 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/workspace_member/remove_tag_to_workspace_member.py
+-rw-r--r--   0        0        0     1518 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/workspace_member/subcommand.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/workspace_tag/__init__.py
+-rw-r--r--   0        0        0     2645 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/workspace_tag/list_workspace_tag.py
+-rw-r--r--   0        0        0     2576 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/workspace_tag/put_workspace_tag.py
+-rw-r--r--   0        0        0      877 2023-05-16 06:21:08.483328 annoworkcli-3.2.2/annoworkcli/workspace_tag/subcommand.py
+-rw-r--r--   0        0        0     2043 2023-05-16 06:21:23.923590 annoworkcli-3.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3152 1970-01-01 00:00:00.000000 annoworkcli-3.2.2/PKG-INFO
```

### Comparing `annoworkcli-3.2.1/README.md` & `annoworkcli-3.2.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -70,19 +70,9 @@
 
 
 
 
 
 
 
-
-# VSCode Devcontainerを使って開発する方法
-1. 以下の環境変数を定義します。
-    * `ANNOFAB_USER_ID`
-    * `ANNOFAB_PASSWORD`
-    * `ANNOWORK_USER_ID`
-    * `ANNOWORK_PASSWORD`
-
-2. VSCodeのdevcontainerを起動します。
-
-
-
+# 開発者向けの情報
+https://github.com/kurusugawa-computer/annowork-cli/blob/main/README_for_developer.md
```

### Comparing `annoworkcli-3.2.1/annoworkcli/__main__.py` & `annoworkcli-3.2.2/annoworkcli/__main__.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/account/list_external_linkage_info.py` & `annoworkcli-3.2.2/annoworkcli/account/list_external_linkage_info.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/account/put_external_linkage_info.py` & `annoworkcli-3.2.2/annoworkcli/account/put_external_linkage_info.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/account/subcommand.py` & `annoworkcli-3.2.2/annoworkcli/account/subcommand.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/actual_working_time/delete_actual_working_time.py` & `annoworkcli-3.2.2/annoworkcli/actual_working_time/delete_actual_working_time.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/actual_working_time/list_actual_working_hours_daily.py` & `annoworkcli-3.2.2/annoworkcli/actual_working_time/list_actual_working_hours_daily.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/actual_working_time/list_actual_working_hours_daily_groupby_tag.py` & `annoworkcli-3.2.2/annoworkcli/actual_working_time/list_actual_working_hours_daily_groupby_tag.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/actual_working_time/list_actual_working_time.py` & `annoworkcli-3.2.2/annoworkcli/actual_working_time/list_actual_working_time.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/actual_working_time/subcommand.py` & `annoworkcli-3.2.2/annoworkcli/actual_working_time/subcommand.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/annofab/list_job_with_annofab_project.py` & `annoworkcli-3.2.2/annoworkcli/annofab/list_job_with_annofab_project.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/annofab/list_working_hours.py` & `annoworkcli-3.2.2/annoworkcli/annofab/list_working_hours.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/annofab/put_account_external_linkage_info.py` & `annoworkcli-3.2.2/annoworkcli/annofab/put_account_external_linkage_info.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/annofab/put_job_from_annofab_project.py` & `annoworkcli-3.2.2/annoworkcli/annofab/put_job_from_annofab_project.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/annofab/reshape_working_hours.py` & `annoworkcli-3.2.2/annoworkcli/annofab/reshape_working_hours.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/annofab/subcommand.py` & `annoworkcli-3.2.2/annoworkcli/annofab/subcommand.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/annofab/visualize_statistics.py` & `annoworkcli-3.2.2/annoworkcli/annofab/visualize_statistics.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/common/annofab.py` & `annoworkcli-3.2.2/annoworkcli/common/annofab.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/common/cli.py` & `annoworkcli-3.2.2/annoworkcli/common/cli.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/common/utils.py` & `annoworkcli-3.2.2/annoworkcli/common/utils.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/common/workspace_tag.py` & `annoworkcli-3.2.2/annoworkcli/common/workspace_tag.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/data/logging.yaml` & `annoworkcli-3.2.2/annoworkcli/data/logging.yaml`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/expected_working_time/delete_expected_working_time.py` & `annoworkcli-3.2.2/annoworkcli/expected_working_time/delete_expected_working_time.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/expected_working_time/list_expected_working_time.py` & `annoworkcli-3.2.2/annoworkcli/expected_working_time/list_expected_working_time.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/expected_working_time/list_expected_working_time_groupby_tag.py` & `annoworkcli-3.2.2/annoworkcli/expected_working_time/list_expected_working_time_groupby_tag.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/expected_working_time/list_expected_working_time_weekly.py` & `annoworkcli-3.2.2/annoworkcli/expected_working_time/list_expected_working_time_weekly.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/expected_working_time/subcommand.py` & `annoworkcli-3.2.2/annoworkcli/expected_working_time/subcommand.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/job/change_job_properties.py` & `annoworkcli-3.2.2/annoworkcli/job/change_job_properties.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/job/delete_job.py` & `annoworkcli-3.2.2/annoworkcli/job/delete_job.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/job/list_job.py` & `annoworkcli-3.2.2/annoworkcli/job/list_job.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/job/subcommand.py` & `annoworkcli-3.2.2/annoworkcli/job/subcommand.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/my/get_my_account.py` & `annoworkcli-3.2.2/annoworkcli/my/get_my_account.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/my/list_my_workspace_member.py` & `annoworkcli-3.2.2/annoworkcli/my/list_my_workspace_member.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/my/subcommand.py` & `annoworkcli-3.2.2/annoworkcli/my/subcommand.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/schedule/list_assigned_hours_daily.py` & `annoworkcli-3.2.2/annoworkcli/schedule/list_assigned_hours_daily.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/schedule/list_assigned_hours_daily_groupby_tag.py` & `annoworkcli-3.2.2/annoworkcli/schedule/list_assigned_hours_daily_groupby_tag.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/schedule/list_schedule.py` & `annoworkcli-3.2.2/annoworkcli/schedule/list_schedule.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/schedule/subcommand.py` & `annoworkcli-3.2.2/annoworkcli/schedule/subcommand.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/workspace/list_workspace.py` & `annoworkcli-3.2.2/annoworkcli/workspace/list_workspace.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/workspace/put_workspace.py` & `annoworkcli-3.2.2/annoworkcli/workspace/put_workspace.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/workspace/subcommand.py` & `annoworkcli-3.2.2/annoworkcli/workspace/subcommand.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/workspace_member/append_tag_to_workspace_member.py` & `annoworkcli-3.2.2/annoworkcli/workspace_member/append_tag_to_workspace_member.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/workspace_member/change_workspace_member_properties.py` & `annoworkcli-3.2.2/annoworkcli/workspace_member/change_workspace_member_properties.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/workspace_member/delete_workspace_member.py` & `annoworkcli-3.2.2/annoworkcli/workspace_member/delete_workspace_member.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/workspace_member/list_workspace_member.py` & `annoworkcli-3.2.2/annoworkcli/workspace_member/list_workspace_member.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/workspace_member/put_workspace_member.py` & `annoworkcli-3.2.2/annoworkcli/workspace_member/put_workspace_member.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/workspace_member/remove_tag_to_workspace_member.py` & `annoworkcli-3.2.2/annoworkcli/workspace_member/remove_tag_to_workspace_member.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/workspace_member/subcommand.py` & `annoworkcli-3.2.2/annoworkcli/workspace_member/subcommand.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/workspace_tag/list_workspace_tag.py` & `annoworkcli-3.2.2/annoworkcli/workspace_tag/list_workspace_tag.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/workspace_tag/put_workspace_tag.py` & `annoworkcli-3.2.2/annoworkcli/workspace_tag/put_workspace_tag.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/annoworkcli/workspace_tag/subcommand.py` & `annoworkcli-3.2.2/annoworkcli/workspace_tag/subcommand.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.1/pyproject.toml` & `annoworkcli-3.2.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 [tool.poetry]
 name = "annoworkcli"
-version = "3.2.1"
+version = "3.2.2"  # `poetry-dynamic-versioning`を使ってGitHubのバージョンタグを取得している。変更不要
 description = "AnnoworkのCLI(Command Line Interface)"
 authors = ["Kurusugawa Computer Inc."]
 license = "MIT"
 keywords=["annowork", "cli"]
 readme="README.md"
 repository="https://github.com/kurusugawa-computer/annowork-cli"
 classifiers = [
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
-        "License :: OSI Approved :: MIT License",
         "Environment :: Console",
-        "Programming Language :: Python",
         "Topic :: Utilities",
         "Operating System :: OS Independent",
 ]
 
 
 [tool.poetry.dependencies]
 # 3.8.1まで指定している理由: flake8 v6.0.0を利用するため、Python3.8.0のサポートを落とした
@@ -79,11 +77,17 @@
 
 [tool.mypy]
 ignore_missing_imports = true
 
 check_untyped_defs = true
 
 
+[tool.poetry-dynamic-versioning]
+enable = false
+format = "{base}"
+
 
 [build-system]
-requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
+build-backend = "poetry_dynamic_versioning.backend"
+
+
```

### Comparing `annoworkcli-3.2.1/PKG-INFO` & `annoworkcli-3.2.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: annoworkcli
-Version: 3.2.1
+Version: 3.2.2
 Summary: AnnoworkのCLI(Command Line Interface)
 Home-page: https://github.com/kurusugawa-computer/annowork-cli
 License: MIT
 Keywords: annowork,cli
 Author: Kurusugawa Computer Inc.
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Requires-Dist: annofabapi (>=0.52.4)
 Requires-Dist: annofabcli (>=1.61.2)
@@ -100,20 +99,9 @@
 
 
 
 
 
 
 
-
-# VSCode Devcontainerを使って開発する方法
-1. 以下の環境変数を定義します。
-    * `ANNOFAB_USER_ID`
-    * `ANNOFAB_PASSWORD`
-    * `ANNOWORK_USER_ID`
-    * `ANNOWORK_PASSWORD`
-
-2. VSCodeのdevcontainerを起動します。
-
-
-
-
+# 開発者向けの情報
+https://github.com/kurusugawa-computer/annowork-cli/blob/main/README_for_developer.md
```

