# Comparing `tmp/asana-preview-1.0.4.tar.gz` & `tmp/asana-preview-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/python-asana-preview/python-asana-preview/dist/.tmp-4t7kh5ro/asana-preview-1.0.4.tar", last modified: Wed Apr 19 21:25:02 2023, max compression
+gzip compressed data, was "/home/runner/work/python-asana-preview/python-asana-preview/dist/.tmp-2nwnoom3/asana-preview-1.0.5.tar", last modified: Mon May 15 23:03:36 2023, max compression
```

## Comparing `asana-preview-1.0.4.tar` & `asana-preview-1.0.5.tar`

### file list

```diff
@@ -1,228 +1,906 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:25:02.000000 asana-preview-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-19 21:24:53.000000 asana-preview-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-04-19 21:25:02.000000 asana-preview-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-04-19 21:24:53.000000 asana-preview-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:25:02.000000 asana-preview-1.0.4/asana_preview/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:25:02.000000 asana-preview-1.0.4/asana_preview/api/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/api/events_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    15631 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/api/projects_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8796 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/api/sections_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/api/stories_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    32576 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/api/tasks_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/api/users_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    39420 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:25:02.000000 asana-preview-1.0.4/asana_preview/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16486 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:25:02.000000 asana-preview-1.0.4/asana_preview/model/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14450 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/asana_named_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    11458 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/asana_named_resource_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    11846 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/asana_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    23974 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/custom_field_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15390 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/custom_field_base_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    19803 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/custom_field_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)    17203 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/custom_field_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/custom_field_compact_all_of_date_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    32959 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/custom_field_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    20265 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/custom_field_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    14345 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/custom_field_setting_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)    11645 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/custom_field_setting_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    16084 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/custom_field_setting_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12923 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/custom_field_setting_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    15102 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/enum_option.py
--rw-r--r--   0 runner    (1001) docker     (123)    12479 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/enum_option_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    11679 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/error_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    13998 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/error_response5_xx.py
--rw-r--r--   0 runner    (1001) docker     (123)    11726 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/error_response5_xx_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/error_response5_xx_all_of_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    12041 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/error_response_errors_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    14117 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/event_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    15698 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/event_response_change.py
--rw-r--r--   0 runner    (1001) docker     (123)    14285 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/event_response_parent.py
--rw-r--r--   0 runner    (1001) docker     (123)    14291 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/event_response_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    14395 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/event_response_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    12228 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/get_events200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    14094 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/get_events401_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/get_events401_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    11633 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/get_events401_response_all_of_errors_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    14094 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/get_events403_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/get_events403_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    11633 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/get_events403_response_all_of_errors_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    14094 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/get_events404_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/get_events404_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    11633 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/get_events404_response_all_of_errors_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    14416 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/get_events412_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12124 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/get_events412_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    11633 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/get_events412_response_all_of_errors_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    14110 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/get_events500_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/get_events500_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    11633 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/get_events500_response_all_of_errors_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/get_project200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11624 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/get_projects200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11964 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/get_sections_for_project200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11938 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/get_stories_for_task200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/get_task200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11934 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/get_tasks_for_project200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/get_user200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11857 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/like.py
--rw-r--r--   0 runner    (1001) docker     (123)    11723 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/next_page.py
--rw-r--r--   0 runner    (1001) docker     (123)    23004 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/project_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    19567 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/project_base_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    14296 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/project_brief_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)    11627 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/project_brief_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    14729 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/project_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)    12086 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/project_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    28963 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    17331 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/project_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    15562 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/project_status_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12762 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/project_status_base_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    14569 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/project_status_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)    11895 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/project_status_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/project_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12889 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/project_status_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    14560 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/project_template_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)    11876 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/project_template_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    14581 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/section_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)    11938 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/section_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    15589 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/status_update_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)    12920 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/status_update_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    16666 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/story_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)    14097 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/story_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    14689 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/tag_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/tag_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    22243 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/task_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    18242 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/task_base_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    11575 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/task_base_all_of_external.py
--rw-r--r--   0 runner    (1001) docker     (123)    15523 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/task_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)    12895 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/task_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    36129 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/task_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    25145 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/task_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/task_response_all_of_memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/team_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/team_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    15264 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/user_base_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/user_base_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    12546 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/user_base_response_all_of_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)    14545 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/user_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)    11917 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/user_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    15982 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/user_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12001 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/user_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    14505 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/workspace_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)    11852 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model/workspace_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    82577 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:25:02.000000 asana-preview-1.0.4/asana_preview/models/
--rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14254 2023-04-19 21:24:53.000000 asana-preview-1.0.4/asana_preview/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:25:02.000000 asana-preview-1.0.4/asana_preview.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-04-19 21:25:02.000000 asana-preview-1.0.4/asana_preview.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8742 2023-04-19 21:25:02.000000 asana-preview-1.0.4/asana_preview.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 21:25:02.000000 asana-preview-1.0.4/asana_preview.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-19 21:25:02.000000 asana-preview-1.0.4/asana_preview.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-19 21:25:02.000000 asana-preview-1.0.4/asana_preview.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-19 21:25:02.000000 asana-preview-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-19 21:24:53.000000 asana-preview-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:25:02.000000 asana-preview-1.0.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_asana_named_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_asana_named_resource_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_asana_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_custom_field_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_custom_field_base_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_custom_field_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_custom_field_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_custom_field_compact_all_of_date_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_custom_field_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_custom_field_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_custom_field_setting_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_custom_field_setting_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_custom_field_setting_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_custom_field_setting_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_enum_option.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_enum_option_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_error_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_error_response5_xx.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_error_response5_xx_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_error_response5_xx_all_of_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_error_response_errors_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_event_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_event_response_change.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_event_response_parent.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_event_response_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_event_response_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_events_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_get_events200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_get_events401_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_get_events401_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_get_events401_response_all_of_errors_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_get_events403_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_get_events403_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_get_events403_response_all_of_errors_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_get_events404_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_get_events404_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_get_events404_response_all_of_errors_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_get_events412_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_get_events412_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_get_events412_response_all_of_errors_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_get_events500_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_get_events500_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_get_events500_response_all_of_errors_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_get_project200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_get_projects200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_get_sections_for_project200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_get_stories_for_task200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_get_task200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_get_tasks_for_project200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_get_user200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_like.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_next_page.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_project_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_project_base_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_project_brief_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_project_brief_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_project_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_project_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_project_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_project_status_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_project_status_base_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_project_status_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_project_status_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_project_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_project_status_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_project_template_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_project_template_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_projects_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_section_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_section_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_sections_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_status_update_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_status_update_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_stories_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_story_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_story_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_tag_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_tag_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_task_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_task_base_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_task_base_all_of_external.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_task_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_task_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_task_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_task_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_task_response_all_of_memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_tasks_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_team_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_team_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_user_base_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_user_base_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_user_base_response_all_of_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_user_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_user_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_user_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_user_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_users_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_workspace_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-19 21:24:53.000000 asana-preview-1.0.4/test/test_workspace_compact_all_of.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:03:36.000000 asana-preview-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-15 23:03:26.000000 asana-preview-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    30444 2023-05-15 23:03:36.000000 asana-preview-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    30154 2023-05-15 23:03:26.000000 asana-preview-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:03:36.000000 asana-preview-1.0.5/asana_preview/
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:03:36.000000 asana-preview-1.0.5/asana_preview/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31911 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/api/attachments_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/api/audit_log_api_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/api/batch_api_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16480 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/api/custom_field_settings_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64460 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/api/custom_fields_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8889 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/api/events_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36487 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/api/goal_relationships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61188 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/api/goals_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/api/jobs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27006 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/api/memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15627 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/api/organization_exports_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23167 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/api/portfolio_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89798 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/api/portfolios_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28064 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/api/project_briefs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15563 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/api/project_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29330 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/api/project_statuses_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31284 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/api/project_templates_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   156596 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/api/projects_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/api/rules_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48377 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/api/sections_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30345 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/api/status_updates_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45780 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/api/stories_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59040 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/api/tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   220597 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/api/tasks_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30781 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/api/team_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55806 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/api/teams_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15449 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/api/time_periods_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36606 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/api/time_tracking_entries_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11880 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/api/typeahead_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14401 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/api/user_task_lists_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36885 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/api/users_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37505 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/api/webhooks_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23801 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/api/workspace_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35868 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/api/workspaces_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39661 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:03:36.000000 asana-preview-1.0.5/asana_preview/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16637 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:03:36.000000 asana-preview-1.0.5/asana_preview/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11934 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/add_custom_field_setting_for_portfolio200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11937 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/add_custom_field_setting_for_portfolio_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13487 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/add_custom_field_setting_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/add_dependencies_for_task_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/add_dependents_for_task_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11839 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/add_followers_for_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/add_followers_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11859 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/add_item_for_portfolio_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/add_members_for_portfolio_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11849 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/add_members_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11839 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/add_project_for_task_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11969 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/add_supporting_relationship_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11799 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/add_tag_for_task_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11860 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/add_task_for_section_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11809 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/add_user_for_team_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11821 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/add_user_for_workspace200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11859 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/add_user_for_workspace_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14614 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/asana_named_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11622 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/asana_named_resource_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12010 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/asana_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/attachment_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15125 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/attachment_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12139 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/attachment_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19389 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/attachment_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15630 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/attachment_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14293 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/audit_log_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12869 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/audit_log_event_actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14166 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/audit_log_event_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12791 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/audit_log_event_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/batch_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13965 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/batch_request_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12187 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/batch_request_action_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12964 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/batch_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/create_batch_request200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/create_batch_request_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11836 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/create_custom_field201_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11817 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/create_custom_field_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11811 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/create_enum_option_for_custom_field201_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11849 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/create_enum_option_for_custom_field_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11786 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/create_goal_metric_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/create_membership200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11632 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/create_membership_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/create_membership_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11899 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/create_organization_export201_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11887 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/create_organization_export_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11815 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/create_portfolio201_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/create_portfolio_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11795 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/create_project201_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/create_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11846 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/create_project_status_for_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11836 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/create_status_for_object_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11755 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/create_tag201_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11736 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/create_tag_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/create_task201_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11746 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/create_task_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11869 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/create_time_tracking_entry201_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11674 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/create_time_tracking_entry_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11795 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/create_webhook201_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/create_webhook_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32380 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/custom_field_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24296 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/custom_field_base_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20384 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/custom_field_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17456 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/custom_field_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12156 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/custom_field_compact_all_of_date_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34131 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/custom_field_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13258 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/custom_field_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33863 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/custom_field_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13340 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/custom_field_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/custom_field_setting_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14213 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/custom_field_setting_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11645 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/custom_field_setting_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16182 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/custom_field_setting_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13087 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/custom_field_setting_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12600 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/date_variable_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12374 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/date_variable_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12082 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/delete_attachment200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11849 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/duplicate_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11819 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/duplicate_task_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15200 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/enum_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12249 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/enum_option_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11846 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/enum_option_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12882 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/enum_option_insert_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16303 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/enum_option_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12452 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/enum_option_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12700 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11707 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13998 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/error_response5_xx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11726 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/error_response5_xx_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/error_response5_xx_all_of_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12041 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/error_response_errors_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14281 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/event_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15862 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/event_response_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14449 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/event_response_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/event_response_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14493 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/event_response_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11816 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_attachment200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11845 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_attachments_for_object200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11800 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_audit_log_events200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11937 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_custom_field_settings_for_project200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11872 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_custom_fields_for_workspace200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12392 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_events200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14094 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_events401_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_events401_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11633 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_events401_response_all_of_errors_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14094 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_events403_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_events403_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11633 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_events403_response_all_of_errors_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14094 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_events404_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_events404_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11633 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_events404_response_all_of_errors_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14416 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_events412_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12124 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_events412_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11633 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_events412_response_all_of_errors_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14110 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_events500_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_events500_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11633 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_events500_response_all_of_errors_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_favorites_for_user200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_goal200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_goal_relationship200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11879 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_goal_relationships200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11758 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_goals200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11815 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_items_for_portfolio200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11739 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_job200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_memberships200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_portfolio_membership200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11909 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_portfolio_memberships200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11808 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_portfolios200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_project200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11837 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_project_brief200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11887 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_project_membership200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11919 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_project_memberships_for_project200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11847 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_project_status200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11882 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_project_statuses_for_project200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11867 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_project_template200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11869 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_project_templates200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11624 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_projects200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11786 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_section200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_sections_for_project200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11819 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_status200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_statuses_for_object200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_stories_for_task200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11766 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_story200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11748 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_tags200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_task200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11840 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_task_counts_for_project200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11758 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_tasks200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11934 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_tasks_for_project200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_team_membership200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11859 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_team_memberships200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11794 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_teams_for_workspace200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11817 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_time_period200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11819 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_time_periods200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11914 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_time_tracking_entries_for_task200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_user200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11831 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_user_task_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11758 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_users200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11795 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_webhooks200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_workspace200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11907 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_workspace_membership200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_workspace_memberships_for_user200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11808 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/get_workspaces200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12872 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/goal_add_subgoal_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13882 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/goal_add_supporting_relationship_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11876 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/goal_add_supporting_work_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18234 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/goal_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15293 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/goal_base_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/goal_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11951 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/goal_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/goal_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15661 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/goal_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12718 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/goal_membership_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11925 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/goal_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19970 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/goal_metric_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16998 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/goal_metric_base_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14904 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/goal_metric_current_value_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11855 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/goal_metric_current_value_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/goal_metric_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16563 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/goal_relationship_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11799 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/goal_relationship_base_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16137 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/goal_relationship_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13120 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/goal_relationship_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16353 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/goal_relationship_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16356 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/goal_relationship_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11760 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/goal_remove_subgoal_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12061 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/goal_remove_supporting_relationship_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19666 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/goal_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/goal_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21948 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/goal_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15147 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/goal_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/insert_enum_option_for_custom_field_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11899 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/insert_section_for_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/instantiate_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/job_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16755 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/job_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13868 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/job_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11837 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/job_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12021 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/like.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14544 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/member_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11906 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/member_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12452 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/membership_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21316 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11718 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/modify_dependencies_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11732 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/modify_dependents_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11723 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/next_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/organization_export_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16696 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/organization_export_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13733 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/organization_export_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11744 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/organization_export_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11957 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/organization_export_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12789 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/portfolio_add_item_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15602 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/portfolio_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12387 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/portfolio_base_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14603 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/portfolio_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11622 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/portfolio_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11953 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/portfolio_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15122 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/portfolio_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12154 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/portfolio_membership_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/portfolio_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11701 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/portfolio_remove_item_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16615 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/portfolio_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12392 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/portfolio_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21309 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/portfolio_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17145 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/portfolio_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13529 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23128 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/project_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19757 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/project_base_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14941 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/project_brief_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11928 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/project_brief_base_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14195 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/project_brief_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11627 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/project_brief_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15414 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/project_brief_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/project_brief_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16024 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/project_brief_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12466 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/project_brief_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14827 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/project_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/project_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13608 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/project_duplicate_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13034 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/project_duplicate_request_schedule_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11937 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/project_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14740 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/project_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11782 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/project_membership_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16011 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/project_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/project_membership_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24697 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12942 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/project_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28730 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17138 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/project_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11662 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/project_save_as_template_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12825 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/project_section_insert_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15662 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/project_status_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12534 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/project_status_base_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14667 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/project_status_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11665 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/project_status_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11899 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/project_status_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17251 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/project_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13039 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/project_status_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19025 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/project_template_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15806 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/project_template_base_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14658 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/project_template_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11646 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/project_template_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14539 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/project_template_instantiate_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18823 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/project_template_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11967 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/remove_custom_field_setting_for_portfolio_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11822 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/remove_custom_field_setting_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11886 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/remove_follower_for_task_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11869 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/remove_followers_for_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11886 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/remove_followers_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/remove_item_for_portfolio_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11855 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/remove_members_for_portfolio_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11858 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/remove_members_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11869 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/remove_project_for_task_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11999 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/remove_supporting_relationship_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11829 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/remove_tag_for_task_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11839 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/remove_user_for_team_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/remove_user_for_workspace_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12007 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/requested_role_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/rule_trigger_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11671 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/rule_trigger_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11857 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/section_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14679 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/section_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11708 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/section_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12740 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/section_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15742 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/section_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12499 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/section_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12656 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/section_task_insert_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11829 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/set_parent_for_task_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17043 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/status_update_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12933 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/status_update_base_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15687 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/status_update_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12690 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/status_update_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17361 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/status_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11810 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/status_update_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21331 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/status_update_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15735 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/status_update_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17423 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/story_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14477 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/story_base_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16772 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/story_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13875 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/story_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11835 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/story_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33456 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/story_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27464 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/story_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12948 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/story_response_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16144 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/tag_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12757 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/tag_base_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14787 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/tag_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11836 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/tag_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16825 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/tag_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12042 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/tag_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17696 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/tag_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13038 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/task_add_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11641 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/task_add_tag_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31593 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/task_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27660 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/task_base_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11739 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/task_base_all_of_external.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12145 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/task_base_all_of_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15619 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/task_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12663 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/task_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13413 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/task_count_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12303 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/task_duplicate_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11904 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/task_remove_followers_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11724 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/task_remove_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11660 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/task_remove_tag_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35592 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/task_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15363 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/task_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36852 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/task_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16786 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/task_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/task_response_all_of_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/task_set_parent_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11757 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/team_add_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11833 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/team_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14553 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/team_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11597 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/team_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/team_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15954 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/team_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13011 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/team_membership_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11925 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/team_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11766 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/team_remove_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19970 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/team_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16800 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/team_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20415 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/team_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17240 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/team_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14571 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/template_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11610 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/template_role_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16211 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/time_period_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/time_period_base_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15984 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/time_period_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12997 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/time_period_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16163 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/time_period_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16066 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/time_tracking_entry_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12124 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/time_tracking_entry_base_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15376 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/time_tracking_entry_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12417 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/time_tracking_entry_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/trigger_rule200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11799 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/trigger_rule_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11847 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/typeahead_for_workspace200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11893 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/update_goal_metric_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11867 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/update_goal_relationship_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11746 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/update_goal_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/update_membership_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/update_project_brief_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/update_section_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11735 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/update_story_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/update_team200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11746 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/update_team_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11674 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/update_time_tracking_entry_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11819 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/update_webhook_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/update_workspace_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11833 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/user_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15362 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/user_base_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12140 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/user_base_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12710 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/user_base_response_all_of_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14643 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/user_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11687 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/user_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11842 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16080 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/user_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12165 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/user_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/user_task_list_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15739 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/user_task_list_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12741 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/user_task_list_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11906 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/user_task_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11909 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/user_task_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15454 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/webhook_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12547 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/webhook_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13925 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/webhook_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13475 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/webhook_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16131 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/webhook_request_filters_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18014 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/webhook_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13932 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/webhook_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12359 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/webhook_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/workspace_add_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11873 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/workspace_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14603 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/workspace_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11622 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/workspace_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11953 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/workspace_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15122 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/workspace_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12154 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/workspace_membership_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11962 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/workspace_membership_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17593 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/workspace_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13882 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/workspace_membership_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12360 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/workspace_membership_response_all_of_vacation_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11781 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/workspace_remove_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11882 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/workspace_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15301 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model/workspace_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82741 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:03:36.000000 asana-preview-1.0.5/asana_preview/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    30734 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14418 2023-05-15 23:03:26.000000 asana-preview-1.0.5/asana_preview/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:03:36.000000 asana-preview-1.0.5/asana_preview.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    30444 2023-05-15 23:03:36.000000 asana-preview-1.0.5/asana_preview.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    38268 2023-05-15 23:03:36.000000 asana-preview-1.0.5/asana_preview.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 23:03:36.000000 asana-preview-1.0.5/asana_preview.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-15 23:03:36.000000 asana-preview-1.0.5/asana_preview.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-15 23:03:36.000000 asana-preview-1.0.5/asana_preview.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-15 23:03:36.000000 asana-preview-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-15 23:03:26.000000 asana-preview-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:03:36.000000 asana-preview-1.0.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_add_custom_field_setting_for_portfolio200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_add_custom_field_setting_for_portfolio_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_add_custom_field_setting_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_add_dependencies_for_task_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_add_dependents_for_task_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_add_followers_for_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_add_followers_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_add_item_for_portfolio_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_add_members_for_portfolio_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_add_members_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_add_project_for_task_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_add_supporting_relationship_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_add_tag_for_task_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_add_task_for_section_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_add_user_for_team_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_add_user_for_workspace200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_add_user_for_workspace_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_asana_named_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_asana_named_resource_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_asana_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_attachment_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_attachment_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_attachment_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_attachment_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_attachment_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_attachments_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_audit_log_api_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_audit_log_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_audit_log_event_actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_audit_log_event_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_audit_log_event_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_batch_api_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_batch_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_batch_request_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_batch_request_action_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_batch_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_create_batch_request200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_create_batch_request_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_create_custom_field201_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_create_custom_field_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_create_enum_option_for_custom_field201_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_create_enum_option_for_custom_field_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_create_goal_metric_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_create_membership200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_create_membership_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_create_membership_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_create_organization_export201_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_create_organization_export_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_create_portfolio201_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_create_portfolio_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_create_project201_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_create_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_create_project_status_for_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_create_status_for_object_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_create_tag201_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_create_tag_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_create_task201_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_create_task_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_create_time_tracking_entry201_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_create_time_tracking_entry_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_create_webhook201_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_create_webhook_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_custom_field_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_custom_field_base_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_custom_field_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_custom_field_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_custom_field_compact_all_of_date_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_custom_field_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_custom_field_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_custom_field_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_custom_field_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_custom_field_setting_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_custom_field_setting_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_custom_field_setting_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_custom_field_setting_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_custom_field_setting_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_custom_field_settings_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_custom_fields_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_date_variable_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_date_variable_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_delete_attachment200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_duplicate_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_duplicate_task_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_enum_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_enum_option_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_enum_option_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_enum_option_insert_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_enum_option_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_enum_option_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_error_response5_xx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_error_response5_xx_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_error_response5_xx_all_of_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_error_response_errors_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_event_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_event_response_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_event_response_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_event_response_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_event_response_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_events_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_attachment200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_attachments_for_object200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_audit_log_events200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_custom_field_settings_for_project200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_custom_fields_for_workspace200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_events200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_events401_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_events401_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_events401_response_all_of_errors_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_events403_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_events403_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_events403_response_all_of_errors_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_events404_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_events404_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_events404_response_all_of_errors_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_events412_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_events412_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_events412_response_all_of_errors_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_events500_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_events500_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_events500_response_all_of_errors_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_favorites_for_user200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_goal200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_goal_relationship200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_goal_relationships200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_goals200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_items_for_portfolio200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_job200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_memberships200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_portfolio_membership200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_portfolio_memberships200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_portfolios200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_project200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_project_brief200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_project_membership200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_project_memberships_for_project200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_project_status200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_project_statuses_for_project200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_project_template200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_project_templates200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_projects200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_section200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_sections_for_project200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_status200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_statuses_for_object200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_stories_for_task200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_story200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_tags200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_task200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_task_counts_for_project200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_tasks200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_tasks_for_project200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_team_membership200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_team_memberships200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_teams_for_workspace200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_time_period200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_time_periods200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_time_tracking_entries_for_task200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_user200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_user_task_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_users200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_webhooks200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_workspace200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_workspace_membership200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_workspace_memberships_for_user200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_get_workspaces200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_goal_add_subgoal_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_goal_add_supporting_relationship_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_goal_add_supporting_work_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_goal_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_goal_base_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_goal_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_goal_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_goal_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_goal_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_goal_membership_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_goal_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_goal_metric_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_goal_metric_base_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_goal_metric_current_value_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_goal_metric_current_value_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_goal_metric_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_goal_relationship_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_goal_relationship_base_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_goal_relationship_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_goal_relationship_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_goal_relationship_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_goal_relationship_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_goal_relationships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_goal_remove_subgoal_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_goal_remove_supporting_relationship_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_goal_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_goal_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_goal_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_goal_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_goals_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_insert_enum_option_for_custom_field_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_insert_section_for_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_instantiate_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_job_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_job_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_job_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_job_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_jobs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_like.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_member_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_member_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_membership_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_modify_dependencies_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_modify_dependents_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_next_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_organization_export_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_organization_export_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_organization_export_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_organization_export_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_organization_export_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_organization_exports_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_portfolio_add_item_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_portfolio_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_portfolio_base_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_portfolio_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_portfolio_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_portfolio_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_portfolio_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_portfolio_membership_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_portfolio_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_portfolio_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_portfolio_remove_item_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_portfolio_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_portfolio_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_portfolio_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_portfolio_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_portfolios_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_project_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_project_base_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_project_brief_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_project_brief_base_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_project_brief_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_project_brief_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_project_brief_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_project_brief_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_project_brief_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_project_brief_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_project_briefs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_project_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_project_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_project_duplicate_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_project_duplicate_request_schedule_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_project_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_project_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_project_membership_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_project_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_project_membership_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_project_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_project_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_project_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_project_save_as_template_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_project_section_insert_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_project_status_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_project_status_base_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_project_status_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_project_status_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_project_status_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_project_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_project_status_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_project_statuses_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_project_template_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_project_template_base_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_project_template_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_project_template_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_project_template_instantiate_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_project_template_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_project_templates_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_projects_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_remove_custom_field_setting_for_portfolio_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_remove_custom_field_setting_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_remove_follower_for_task_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_remove_followers_for_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_remove_followers_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_remove_item_for_portfolio_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_remove_members_for_portfolio_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_remove_members_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_remove_project_for_task_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_remove_supporting_relationship_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_remove_tag_for_task_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_remove_user_for_team_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_remove_user_for_workspace_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_requested_role_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_rule_trigger_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_rule_trigger_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_rules_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_section_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_section_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_section_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_section_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_section_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_section_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_section_task_insert_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_sections_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_set_parent_for_task_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_status_update_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_status_update_base_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_status_update_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_status_update_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_status_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_status_update_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_status_update_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_status_update_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_status_updates_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_stories_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_story_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_story_base_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_story_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_story_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_story_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_story_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_story_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_story_response_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_tag_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_tag_base_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_tag_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_tag_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_tag_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_tag_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_tag_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_task_add_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_task_add_tag_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_task_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_task_base_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_task_base_all_of_external.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_task_base_all_of_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_task_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_task_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_task_count_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_task_duplicate_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_task_remove_followers_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_task_remove_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_task_remove_tag_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_task_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_task_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_task_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_task_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_task_response_all_of_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_task_set_parent_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_tasks_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_team_add_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_team_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_team_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_team_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_team_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_team_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_team_membership_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_team_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_team_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_team_remove_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_team_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_team_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_team_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_team_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_teams_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_template_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_template_role_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_time_period_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_time_period_base_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_time_period_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_time_period_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_time_period_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_time_periods_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_time_tracking_entries_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_time_tracking_entry_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_time_tracking_entry_base_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_time_tracking_entry_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_time_tracking_entry_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_trigger_rule200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_trigger_rule_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_typeahead_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_typeahead_for_workspace200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_update_goal_metric_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_update_goal_relationship_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_update_goal_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_update_membership_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_update_project_brief_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_update_section_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_update_story_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_update_team200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_update_team_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_update_time_tracking_entry_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_update_webhook_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_update_workspace_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_user_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_user_base_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_user_base_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_user_base_response_all_of_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_user_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_user_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_user_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_user_task_list_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_user_task_list_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_user_task_list_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_user_task_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_user_task_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_user_task_lists_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_users_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_webhook_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_webhook_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_webhook_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_webhook_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_webhook_request_filters_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_webhook_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_webhook_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_webhook_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_webhooks_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_workspace_add_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_workspace_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_workspace_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_workspace_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_workspace_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_workspace_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_workspace_membership_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_workspace_membership_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_workspace_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_workspace_membership_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_workspace_membership_response_all_of_vacation_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_workspace_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_workspace_remove_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_workspace_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_workspace_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-15 23:03:26.000000 asana-preview-1.0.5/test/test_workspaces_api.py
```

### Comparing `asana-preview-1.0.4/LICENSE` & `asana-preview-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/asana_preview/__init__.py` & `asana-preview-1.0.5/asana_preview/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # flake8: noqa
 
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "1.0.4"
+__version__ = "1.0.5"
 
 # import ApiClient
 from asana_preview.api_client import ApiClient
 
 # import Configuration
 from asana_preview.configuration import Configuration
```

### Comparing `asana-preview-1.0.4/asana_preview/api/events_api.py` & `asana-preview-1.0.5/asana_preview/api/events_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -19,19 +19,14 @@
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
 from asana_preview.model.error_response import ErrorResponse
 from asana_preview.model.get_events200_response import GetEvents200Response
-from asana_preview.model.get_events401_response import GetEvents401Response
-from asana_preview.model.get_events403_response import GetEvents403Response
-from asana_preview.model.get_events404_response import GetEvents404Response
-from asana_preview.model.get_events412_response import GetEvents412Response
-from asana_preview.model.get_events500_response import GetEvents500Response
 
 
 class EventsApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -41,64 +36,75 @@
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
         self.get_events_endpoint = _Endpoint(
             settings={
                 'response_type': (GetEvents200Response,),
                 'auth': [
-                    'personal_access_token'
+                    'personalAccessToken'
                 ],
                 'endpoint_path': '/events',
                 'operation_id': 'get_events',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'resource',
                     'sync',
-                    'opt_fields',
                     'opt_pretty',
+                    'opt_fields',
                 ],
                 'required': [
                     'resource',
                 ],
                 'nullable': [
                 ],
                 'enum': [
+                    'opt_fields',
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
+                    ('opt_fields',): {
+
+                        "PARENT": "parent",
+                        "CREATED_AT": "created_at",
+                        "TYPE": "type",
+                        "RESOURCE": "resource",
+                        "ACTION": "action",
+                        "CHANGE": "change",
+                        "USER": "user"
+                    },
                 },
                 'openapi_types': {
                     'resource':
                         (str,),
                     'sync':
                         (str,),
-                    'opt_fields':
-                        ([str],),
                     'opt_pretty':
                         (bool,),
+                    'opt_fields':
+                        ([str],),
                 },
                 'attribute_map': {
                     'resource': 'resource',
                     'sync': 'sync',
-                    'opt_fields': 'opt_fields',
                     'opt_pretty': 'opt_pretty',
+                    'opt_fields': 'opt_fields',
                 },
                 'location_map': {
                     'resource': 'query',
                     'sync': 'query',
-                    'opt_fields': 'query',
                     'opt_pretty': 'query',
+                    'opt_fields': 'query',
                 },
                 'collection_format_map': {
                     'opt_fields': 'csv',
                 }
             },
             headers_map={
                 'accept': [
@@ -123,17 +129,17 @@
         >>> thread = api.get_events(resource, async_req=True)
         >>> result = thread.get()
 
         Args:
             resource (str): A resource ID to subscribe to. The resource can be a task or project.
 
         Keyword Args:
-            sync (str): A sync token received from the last request, or none on first sync. Events will be returned from the point in time that the sync token was generated.  *Note: On your first request, omit the sync token. The response will be the same as for an expired sync token, and will include a new valid sync token.If the sync token is too old (which may happen from time to time) the API will return a `412 Precondition Failed` error, and include a fresh sync token in the response.*. [optional]
-            opt_fields ([str]): Defines fields to return.  Some requests return *compact* representations of objects in order to conserve resources and complete the request more efficiently. Other times requests return more information than you may need. This option allows you to list the exact set of fields that the API should be sure to return for the objects. The field names should be provided as paths, described below.  The gid of included objects will always be returned, regardless of the field options.. [optional]
+            sync (str): A sync token received from the last request, or none on first sync. Events will be returned from the point in time that the sync token was generated. *Note: On your first request, omit the sync token. The response will be the same as for an expired sync token, and will include a new valid sync token.If the sync token is too old (which may happen from time to time) the API will return a `412 Precondition Failed` error, and include a fresh sync token in the response.*. [optional]
             opt_pretty (bool): Provides “pretty” output. Provides the response in a “pretty” format. In the case of JSON this means doing proper line breaking and indentation to make it readable. This will take extra time and increase the response size so it is advisable only to use this during debugging.. [optional]
+            opt_fields ([str]): This endpoint returns a compact resource, which excludes some properties by default. To include those optional properties, set this query parameter to a comma-separated list of the properties you wish to include.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `asana-preview-1.0.4/asana_preview/api/projects_api.py` & `asana-preview-1.0.5/asana_preview/api/project_memberships_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -18,202 +18,205 @@
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
 from asana_preview.model.error_response import ErrorResponse
-from asana_preview.model.get_events401_response import GetEvents401Response
-from asana_preview.model.get_events403_response import GetEvents403Response
-from asana_preview.model.get_events404_response import GetEvents404Response
-from asana_preview.model.get_events500_response import GetEvents500Response
-from asana_preview.model.get_project200_response import GetProject200Response
-from asana_preview.model.get_projects200_response import GetProjects200Response
+from asana_preview.model.get_project_membership200_response import GetProjectMembership200Response
+from asana_preview.model.get_project_memberships_for_project200_response import GetProjectMembershipsForProject200Response
 
 
-class ProjectsApi(object):
+class ProjectMembershipsApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
-        self.get_project_endpoint = _Endpoint(
+        self.get_project_membership_endpoint = _Endpoint(
             settings={
-                'response_type': (GetProject200Response,),
+                'response_type': (GetProjectMembership200Response,),
                 'auth': [
-                    'personal_access_token'
+                    'personalAccessToken'
                 ],
-                'endpoint_path': '/projects/{project_gid}',
-                'operation_id': 'get_project',
+                'endpoint_path': '/project_memberships/{project_membership_gid}',
+                'operation_id': 'get_project_membership',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'project_gid',
-                    'opt_fields',
+                    'project_membership_gid',
                     'opt_pretty',
+                    'opt_fields',
                 ],
                 'required': [
-                    'project_gid',
+                    'project_membership_gid',
                 ],
                 'nullable': [
                 ],
                 'enum': [
+                    'opt_fields',
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
+                    ('opt_fields',): {
+
+                        "WRITE_ACCESS": "write_access",
+                        "PROJECT": "project",
+                        "USER": "user",
+                        "MEMBER": "member"
+                    },
                 },
                 'openapi_types': {
-                    'project_gid':
+                    'project_membership_gid':
                         (str,),
-                    'opt_fields':
-                        ([str],),
                     'opt_pretty':
                         (bool,),
+                    'opt_fields':
+                        ([str],),
                 },
                 'attribute_map': {
-                    'project_gid': 'project_gid',
-                    'opt_fields': 'opt_fields',
+                    'project_membership_gid': 'project_membership_gid',
                     'opt_pretty': 'opt_pretty',
+                    'opt_fields': 'opt_fields',
                 },
                 'location_map': {
-                    'project_gid': 'path',
-                    'opt_fields': 'query',
+                    'project_membership_gid': 'path',
                     'opt_pretty': 'query',
+                    'opt_fields': 'query',
                 },
                 'collection_format_map': {
                     'opt_fields': 'csv',
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.get_projects_endpoint = _Endpoint(
+        self.get_project_memberships_for_project_endpoint = _Endpoint(
             settings={
-                'response_type': (GetProjects200Response,),
+                'response_type': (GetProjectMembershipsForProject200Response,),
                 'auth': [
-                    'personal_access_token'
+                    'personalAccessToken'
                 ],
-                'endpoint_path': '/projects',
-                'operation_id': 'get_projects',
+                'endpoint_path': '/projects/{project_gid}/project_memberships',
+                'operation_id': 'get_project_memberships_for_project',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'opt_fields',
+                    'project_gid',
+                    'user',
                     'opt_pretty',
                     'limit',
                     'offset',
-                    'archived',
-                    'team',
-                    'workspace',
+                    'opt_fields',
+                ],
+                'required': [
+                    'project_gid',
                 ],
-                'required': [],
                 'nullable': [
                 ],
                 'enum': [
+                    'opt_fields',
                 ],
                 'validation': [
-                    'limit',
                 ]
             },
             root_map={
                 'validations': {
-                    ('limit',): {
-
-                        'inclusive_maximum': 100,
-                        'inclusive_minimum': 0,
-                    },
                 },
                 'allowed_values': {
+                    ('opt_fields',): {
+
+                        "WRITE_ACCESS": "write_access",
+                        "PROJECT": "project",
+                        "USER": "user",
+                        "MEMBER": "member"
+                    },
                 },
                 'openapi_types': {
-                    'opt_fields':
-                        ([str],),
+                    'project_gid':
+                        (str,),
+                    'user':
+                        (str,),
                     'opt_pretty':
                         (bool,),
                     'limit':
                         (int,),
                     'offset':
                         (str,),
-                    'archived':
-                        (bool,),
-                    'team':
-                        (str,),
-                    'workspace':
-                        (str,),
+                    'opt_fields':
+                        ([str],),
                 },
                 'attribute_map': {
-                    'opt_fields': 'opt_fields',
+                    'project_gid': 'project_gid',
+                    'user': 'user',
                     'opt_pretty': 'opt_pretty',
                     'limit': 'limit',
                     'offset': 'offset',
-                    'archived': 'archived',
-                    'team': 'team',
-                    'workspace': 'workspace',
+                    'opt_fields': 'opt_fields',
                 },
                 'location_map': {
-                    'opt_fields': 'query',
+                    'project_gid': 'path',
+                    'user': 'query',
                     'opt_pretty': 'query',
                     'limit': 'query',
                     'offset': 'query',
-                    'archived': 'query',
-                    'team': 'query',
-                    'workspace': 'query',
+                    'opt_fields': 'query',
                 },
                 'collection_format_map': {
                     'opt_fields': 'csv',
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
 
-    def get_project(
+    def get_project_membership(
         self,
-        project_gid,
+        project_membership_gid,
         **kwargs
     ):
-        """Get a project  # noqa: E501
+        """Get a project membership  # noqa: E501
 
-        Returns the complete project record for a single project.  # noqa: E501
+        Returns the complete project record for a single project membership.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_project(project_gid, async_req=True)
+        >>> thread = api.get_project_membership(project_membership_gid, async_req=True)
         >>> result = thread.get()
 
         Args:
-            project_gid (str): Globally unique identifier for the project.
+            project_membership_gid (str):
 
         Keyword Args:
-            opt_fields ([str]): Defines fields to return.  Some requests return *compact* representations of objects in order to conserve resources and complete the request more efficiently. Other times requests return more information than you may need. This option allows you to list the exact set of fields that the API should be sure to return for the objects. The field names should be provided as paths, described below.  The gid of included objects will always be returned, regardless of the field options.. [optional]
             opt_pretty (bool): Provides “pretty” output. Provides the response in a “pretty” format. In the case of JSON this means doing proper line breaking and indentation to make it readable. This will take extra time and increase the response size so it is advisable only to use this during debugging.. [optional]
+            opt_fields ([str]): This endpoint returns a compact resource, which excludes some properties by default. To include those optional properties, set this query parameter to a comma-separated list of the properties you wish to include.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -238,15 +241,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            GetProject200Response
+            GetProjectMembership200Response
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -267,40 +270,41 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['project_gid'] = \
-            project_gid
-        return self.get_project_endpoint.call_with_http_info(**kwargs)
+        kwargs['project_membership_gid'] = \
+            project_membership_gid
+        return self.get_project_membership_endpoint.call_with_http_info(**kwargs)
 
-    def get_projects(
+    def get_project_memberships_for_project(
         self,
+        project_gid,
         **kwargs
     ):
-        """Get multiple projects  # noqa: E501
+        """Get memberships from a project  # noqa: E501
 
-        Returns the compact project records for some filtered set of projects. Use one or more of the parameters provided to filter the projects returned.  *Note: This endpoint may timeout for large domains. Try filtering by team!*  # noqa: E501
+        Returns the compact project membership records for the project.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_projects(async_req=True)
+        >>> thread = api.get_project_memberships_for_project(project_gid, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            project_gid (str): Globally unique identifier for the project.
 
         Keyword Args:
-            opt_fields ([str]): Defines fields to return.  Some requests return *compact* representations of objects in order to conserve resources and complete the request more efficiently. Other times requests return more information than you may need. This option allows you to list the exact set of fields that the API should be sure to return for the objects. The field names should be provided as paths, described below.  The gid of included objects will always be returned, regardless of the field options.. [optional]
+            user (str): A string identifying a user. This can either be the string \"me\", an email, or the gid of a user.. [optional]
             opt_pretty (bool): Provides “pretty” output. Provides the response in a “pretty” format. In the case of JSON this means doing proper line breaking and indentation to make it readable. This will take extra time and increase the response size so it is advisable only to use this during debugging.. [optional]
-            limit (int): The number of objects to return per page. The value must be between 1 and 100.. [optional]
-            offset (str): Offset token.  An offset to the next page returned by the API. A pagination request will return an offset token, which can be used as an input parameter to the next request. If an offset is not passed in, the API will return the first page of results.  'Note: You can only pass in an offset that was returned to you via a previously paginated request.. [optional]
-            archived (bool): Only return projects whose `archived` field takes on the value of this parameter.. [optional]
-            team (str): The team to filter projects on.. [optional]
-            workspace (str): The workspace or organization to filter projects on.. [optional]
+            limit (int): Results per page. The number of objects to return per page. The value must be between 1 and 100.. [optional]
+            offset (str): Offset token. An offset to the next page returned by the API. A pagination request will return an offset token, which can be used as an input parameter to the next request. If an offset is not passed in, the API will return the first page of results. 'Note: You can only pass in an offset that was returned to you via a previously paginated request.'. [optional]
+            opt_fields ([str]): This endpoint returns a compact resource, which excludes some properties by default. To include those optional properties, set this query parameter to a comma-separated list of the properties you wish to include.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -325,15 +329,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            GetProjects200Response
+            GetProjectMembershipsForProject200Response
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -354,9 +358,11 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        return self.get_projects_endpoint.call_with_http_info(**kwargs)
+        kwargs['project_gid'] = \
+            project_gid
+        return self.get_project_memberships_for_project_endpoint.call_with_http_info(**kwargs)
```

### Comparing `asana-preview-1.0.4/asana_preview/api/sections_api.py` & `asana-preview-1.0.5/asana_preview/api/jobs_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -18,133 +18,121 @@
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
 from asana_preview.model.error_response import ErrorResponse
-from asana_preview.model.get_events401_response import GetEvents401Response
-from asana_preview.model.get_events403_response import GetEvents403Response
-from asana_preview.model.get_events404_response import GetEvents404Response
-from asana_preview.model.get_events500_response import GetEvents500Response
-from asana_preview.model.get_sections_for_project200_response import GetSectionsForProject200Response
+from asana_preview.model.get_job200_response import GetJob200Response
 
 
-class SectionsApi(object):
+class JobsApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
-        self.get_sections_for_project_endpoint = _Endpoint(
+        self.get_job_endpoint = _Endpoint(
             settings={
-                'response_type': (GetSectionsForProject200Response,),
+                'response_type': (GetJob200Response,),
                 'auth': [
-                    'personal_access_token'
+                    'personalAccessToken'
                 ],
-                'endpoint_path': '/projects/{project_gid}/sections',
-                'operation_id': 'get_sections_for_project',
+                'endpoint_path': '/jobs/{job_gid}',
+                'operation_id': 'get_job',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'project_gid',
-                    'opt_fields',
+                    'job_gid',
                     'opt_pretty',
-                    'limit',
-                    'offset',
+                    'opt_fields',
                 ],
                 'required': [
-                    'project_gid',
+                    'job_gid',
                 ],
                 'nullable': [
                 ],
                 'enum': [
+                    'opt_fields',
                 ],
                 'validation': [
-                    'limit',
                 ]
             },
             root_map={
                 'validations': {
-                    ('limit',): {
-
-                        'inclusive_maximum': 100,
-                        'inclusive_minimum': 0,
-                    },
                 },
                 'allowed_values': {
+                    ('opt_fields',): {
+
+                        "STATUS": "status",
+                        "RESOURCE_SUBTYPE": "resource_subtype",
+                        "NEW_PROJECT_TEMPLATE": "new_project_template",
+                        "NEW_TASK": "new_task",
+                        "NEW_TASK_TEMPLATE": "new_task_template",
+                        "NEW_PROJECT": "new_project"
+                    },
                 },
                 'openapi_types': {
-                    'project_gid':
+                    'job_gid':
                         (str,),
-                    'opt_fields':
-                        ([str],),
                     'opt_pretty':
                         (bool,),
-                    'limit':
-                        (int,),
-                    'offset':
-                        (str,),
+                    'opt_fields':
+                        ([str],),
                 },
                 'attribute_map': {
-                    'project_gid': 'project_gid',
-                    'opt_fields': 'opt_fields',
+                    'job_gid': 'job_gid',
                     'opt_pretty': 'opt_pretty',
-                    'limit': 'limit',
-                    'offset': 'offset',
+                    'opt_fields': 'opt_fields',
                 },
                 'location_map': {
-                    'project_gid': 'path',
-                    'opt_fields': 'query',
+                    'job_gid': 'path',
                     'opt_pretty': 'query',
-                    'limit': 'query',
-                    'offset': 'query',
+                    'opt_fields': 'query',
                 },
                 'collection_format_map': {
                     'opt_fields': 'csv',
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
 
-    def get_sections_for_project(
+    def get_job(
         self,
-        project_gid,
+        job_gid,
         **kwargs
     ):
-        """Get sections in a project  # noqa: E501
+        """Get a job by id  # noqa: E501
 
-        Returns the compact records for all sections in the specified project.  # noqa: E501
+        Returns the full record for a job.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_sections_for_project(project_gid, async_req=True)
+        >>> thread = api.get_job(job_gid, async_req=True)
         >>> result = thread.get()
 
         Args:
-            project_gid (str): Globally unique identifier for the project.
+            job_gid (str): Globally unique identifier for the job.
 
         Keyword Args:
-            opt_fields ([str]): Defines fields to return.  Some requests return *compact* representations of objects in order to conserve resources and complete the request more efficiently. Other times requests return more information than you may need. This option allows you to list the exact set of fields that the API should be sure to return for the objects. The field names should be provided as paths, described below.  The gid of included objects will always be returned, regardless of the field options.. [optional]
             opt_pretty (bool): Provides “pretty” output. Provides the response in a “pretty” format. In the case of JSON this means doing proper line breaking and indentation to make it readable. This will take extra time and increase the response size so it is advisable only to use this during debugging.. [optional]
-            limit (int): The number of objects to return per page. The value must be between 1 and 100.. [optional]
-            offset (str): Offset token.  An offset to the next page returned by the API. A pagination request will return an offset token, which can be used as an input parameter to the next request. If an offset is not passed in, the API will return the first page of results.  'Note: You can only pass in an offset that was returned to you via a previously paginated request.. [optional]
+            opt_fields ([str]): This endpoint returns a compact resource, which excludes some properties by default. To include those optional properties, set this query parameter to a comma-separated list of the properties you wish to include.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -169,15 +157,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            GetSectionsForProject200Response
+            GetJob200Response
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -198,11 +186,11 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['project_gid'] = \
-            project_gid
-        return self.get_sections_for_project_endpoint.call_with_http_info(**kwargs)
+        kwargs['job_gid'] = \
+            job_gid
+        return self.get_job_endpoint.call_with_http_info(**kwargs)
```

### Comparing `asana-preview-1.0.4/asana_preview/api/stories_api.py` & `asana-preview-1.0.5/asana_preview/api/audit_log_api_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -18,133 +18,173 @@
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
 from asana_preview.model.error_response import ErrorResponse
-from asana_preview.model.get_events401_response import GetEvents401Response
-from asana_preview.model.get_events403_response import GetEvents403Response
-from asana_preview.model.get_events404_response import GetEvents404Response
-from asana_preview.model.get_events500_response import GetEvents500Response
-from asana_preview.model.get_stories_for_task200_response import GetStoriesForTask200Response
+from asana_preview.model.get_audit_log_events200_response import GetAuditLogEvents200Response
 
 
-class StoriesApi(object):
+class AuditLogAPIApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
-        self.get_stories_for_task_endpoint = _Endpoint(
+        self.get_audit_log_events_endpoint = _Endpoint(
             settings={
-                'response_type': (GetStoriesForTask200Response,),
+                'response_type': (GetAuditLogEvents200Response,),
                 'auth': [
-                    'personal_access_token'
+                    'personalAccessToken'
                 ],
-                'endpoint_path': '/tasks/{task_gid}/stories',
-                'operation_id': 'get_stories_for_task',
+                'endpoint_path': '/workspaces/{workspace_gid}/audit_log_events',
+                'operation_id': 'get_audit_log_events',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'task_gid',
-                    'opt_fields',
-                    'opt_pretty',
+                    'workspace_gid',
+                    'start_at',
+                    'end_at',
+                    'event_type',
+                    'actor_type',
+                    'actor_gid',
+                    'resource_gid',
                     'limit',
                     'offset',
+                    'opt_fields',
                 ],
                 'required': [
-                    'task_gid',
+                    'workspace_gid',
                 ],
                 'nullable': [
                 ],
                 'enum': [
+                    'actor_type',
+                    'opt_fields',
                 ],
                 'validation': [
-                    'limit',
                 ]
             },
             root_map={
                 'validations': {
-                    ('limit',): {
-
-                        'inclusive_maximum': 100,
-                        'inclusive_minimum': 0,
-                    },
                 },
                 'allowed_values': {
+                    ('actor_type',): {
+
+                        "USER": "user",
+                        "ASANA": "asana",
+                        "ASANA_SUPPORT": "asana_support",
+                        "ANONYMOUS": "anonymous",
+                        "EXTERNAL_ADMINISTRATOR": "external_administrator"
+                    },
+                    ('opt_fields',): {
+
+                        "EVENT_CATEGORY": "event_category",
+                        "CREATED_AT": "created_at",
+                        "RESOURCE": "resource",
+                        "EVENT_TYPE": "event_type",
+                        "DETAILS": "details",
+                        "ACTOR": "actor",
+                        "CONTEXT": "context"
+                    },
                 },
                 'openapi_types': {
-                    'task_gid':
+                    'workspace_gid':
+                        (str,),
+                    'start_at':
+                        (datetime,),
+                    'end_at':
+                        (datetime,),
+                    'event_type':
+                        (str,),
+                    'actor_type':
+                        (str,),
+                    'actor_gid':
+                        (str,),
+                    'resource_gid':
                         (str,),
-                    'opt_fields':
-                        ([str],),
-                    'opt_pretty':
-                        (bool,),
                     'limit':
                         (int,),
                     'offset':
                         (str,),
+                    'opt_fields':
+                        ([str],),
                 },
                 'attribute_map': {
-                    'task_gid': 'task_gid',
-                    'opt_fields': 'opt_fields',
-                    'opt_pretty': 'opt_pretty',
+                    'workspace_gid': 'workspace_gid',
+                    'start_at': 'start_at',
+                    'end_at': 'end_at',
+                    'event_type': 'event_type',
+                    'actor_type': 'actor_type',
+                    'actor_gid': 'actor_gid',
+                    'resource_gid': 'resource_gid',
                     'limit': 'limit',
                     'offset': 'offset',
+                    'opt_fields': 'opt_fields',
                 },
                 'location_map': {
-                    'task_gid': 'path',
-                    'opt_fields': 'query',
-                    'opt_pretty': 'query',
+                    'workspace_gid': 'path',
+                    'start_at': 'query',
+                    'end_at': 'query',
+                    'event_type': 'query',
+                    'actor_type': 'query',
+                    'actor_gid': 'query',
+                    'resource_gid': 'query',
                     'limit': 'query',
                     'offset': 'query',
+                    'opt_fields': 'query',
                 },
                 'collection_format_map': {
                     'opt_fields': 'csv',
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
 
-    def get_stories_for_task(
+    def get_audit_log_events(
         self,
-        task_gid,
+        workspace_gid,
         **kwargs
     ):
-        """Get stories from a task  # noqa: E501
+        """Get audit log events  # noqa: E501
 
-        Returns the compact records for all stories on the task.  # noqa: E501
+        Retrieve the audit log events that have been captured in your domain.  This endpoint will return a list of [AuditLogEvent](/reference/audit-log-api) objects, sorted by creation time in ascending order. Note that the Audit Log API captures events from October 8th, 2021 and later. Queries for events before this date will not return results.  There are a number of query parameters (below) that can be used to filter the set of [AuditLogEvent](/reference/audit-log-api) objects that are returned in the response. Any combination of query parameters is valid. When no filters are provided, all of the events that have been captured in your domain will match.  The list of events will always be [paginated](/docs/pagination). The default limit is 1000 events. The next set of events can be retrieved using the `offset` from the previous response. If there are no events that match the provided filters in your domain, the endpoint will return `null` for the `next_page` field. Querying again with the same filters may return new events if they were captured after the last request. Once a response includes a `next_page` with an `offset`, subsequent requests can be made with the latest `offset` to poll for new events that match the provided filters.  *Note: If the filters you provided match events in your domain and `next_page` is present in the response, we will continue to send `next_page` on subsequent requests even when there are no more events that match the filters. This was put in place so that you can implement an audit log stream that will return future events that match these filters. If you are not interested in future events that match the filters you have defined, you can rely on checking empty `data` response for the end of current events that match your filters.*  When no `offset` is provided, the response will begin with the oldest events that match the provided filters. It is important to note that [AuditLogEvent](/reference/audit-log-api) objects will be permanently deleted from our systems after 90 days. If you wish to keep a permanent record of these events, we recommend using a SIEM tool to ingest and store these logs.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_stories_for_task(task_gid, async_req=True)
+        >>> thread = api.get_audit_log_events(workspace_gid, async_req=True)
         >>> result = thread.get()
 
         Args:
-            task_gid (str): The task to operate on.
+            workspace_gid (str): Globally unique identifier for the workspace or organization.
 
         Keyword Args:
-            opt_fields ([str]): Defines fields to return.  Some requests return *compact* representations of objects in order to conserve resources and complete the request more efficiently. Other times requests return more information than you may need. This option allows you to list the exact set of fields that the API should be sure to return for the objects. The field names should be provided as paths, described below.  The gid of included objects will always be returned, regardless of the field options.. [optional]
-            opt_pretty (bool): Provides “pretty” output. Provides the response in a “pretty” format. In the case of JSON this means doing proper line breaking and indentation to make it readable. This will take extra time and increase the response size so it is advisable only to use this during debugging.. [optional]
-            limit (int): The number of objects to return per page. The value must be between 1 and 100.. [optional]
-            offset (str): Offset token.  An offset to the next page returned by the API. A pagination request will return an offset token, which can be used as an input parameter to the next request. If an offset is not passed in, the API will return the first page of results.  'Note: You can only pass in an offset that was returned to you via a previously paginated request.. [optional]
+            start_at (datetime): Filter to events created after this time (inclusive).. [optional]
+            end_at (datetime): Filter to events created before this time (exclusive).. [optional]
+            event_type (str): Filter to events of this type. Refer to the [supported audit log events](/docs/audit-log-events#supported-audit-log-events) for a full list of values.. [optional]
+            actor_type (str): Filter to events with an actor of this type. This only needs to be included if querying for actor types without an ID. If `actor_gid` is included, this should be excluded.. [optional]
+            actor_gid (str): Filter to events triggered by the actor with this ID.. [optional]
+            resource_gid (str): Filter to events with this resource ID.. [optional]
+            limit (int): Results per page. The number of objects to return per page. The value must be between 1 and 100.. [optional]
+            offset (str): Offset token. An offset to the next page returned by the API. A pagination request will return an offset token, which can be used as an input parameter to the next request. If an offset is not passed in, the API will return the first page of results. 'Note: You can only pass in an offset that was returned to you via a previously paginated request.'. [optional]
+            opt_fields ([str]): This endpoint returns a compact resource, which excludes some properties by default. To include those optional properties, set this query parameter to a comma-separated list of the properties you wish to include.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -169,15 +209,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            GetStoriesForTask200Response
+            GetAuditLogEvents200Response
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -198,11 +238,11 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['task_gid'] = \
-            task_gid
-        return self.get_stories_for_task_endpoint.call_with_http_info(**kwargs)
+        kwargs['workspace_gid'] = \
+            workspace_gid
+        return self.get_audit_log_events_endpoint.call_with_http_info(**kwargs)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `asana-preview-1.0.4/asana_preview/api/tasks_api.py` & `asana-preview-1.0.5/asana_preview/api/users_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -18,380 +18,447 @@
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
 from asana_preview.model.error_response import ErrorResponse
-from asana_preview.model.get_events401_response import GetEvents401Response
-from asana_preview.model.get_events403_response import GetEvents403Response
-from asana_preview.model.get_events404_response import GetEvents404Response
-from asana_preview.model.get_events500_response import GetEvents500Response
-from asana_preview.model.get_task200_response import GetTask200Response
-from asana_preview.model.get_tasks_for_project200_response import GetTasksForProject200Response
+from asana_preview.model.get_favorites_for_user200_response import GetFavoritesForUser200Response
+from asana_preview.model.get_user200_response import GetUser200Response
+from asana_preview.model.get_users200_response import GetUsers200Response
 
 
-class TasksApi(object):
+class UsersApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
-        self.get_subtasks_for_task_endpoint = _Endpoint(
+        self.get_favorites_for_user_endpoint = _Endpoint(
             settings={
-                'response_type': (GetTasksForProject200Response,),
+                'response_type': (GetFavoritesForUser200Response,),
                 'auth': [
-                    'personal_access_token'
+                    'personalAccessToken'
                 ],
-                'endpoint_path': '/tasks/{task_gid}/subtasks',
-                'operation_id': 'get_subtasks_for_task',
+                'endpoint_path': '/users/{user_gid}/favorites',
+                'operation_id': 'get_favorites_for_user',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'task_gid',
-                    'opt_fields',
+                    'user_gid',
+                    'resource_type',
+                    'workspace',
                     'opt_pretty',
-                    'limit',
-                    'offset',
+                    'opt_fields',
                 ],
                 'required': [
-                    'task_gid',
+                    'user_gid',
+                    'resource_type',
+                    'workspace',
                 ],
                 'nullable': [
                 ],
                 'enum': [
+                    'resource_type',
+                    'opt_fields',
                 ],
                 'validation': [
-                    'limit',
                 ]
             },
             root_map={
                 'validations': {
-                    ('limit',): {
-
-                        'inclusive_maximum': 100,
-                        'inclusive_minimum': 0,
-                    },
                 },
                 'allowed_values': {
+                    ('resource_type',): {
+
+                        "PORTFOLIO": "portfolio",
+                        "PROJECT": "project",
+                        "TAG": "tag",
+                        "TASK": "task",
+                        "USER": "user",
+                        "PROJECT_TEMPLATE": "project_template"
+                    },
+                    ('opt_fields',): {
+
+                        "NAME": "name"
+                    },
                 },
                 'openapi_types': {
-                    'task_gid':
+                    'user_gid':
+                        (str,),
+                    'resource_type':
+                        (str,),
+                    'workspace':
                         (str,),
-                    'opt_fields':
-                        ([str],),
                     'opt_pretty':
                         (bool,),
-                    'limit':
-                        (int,),
-                    'offset':
-                        (str,),
+                    'opt_fields':
+                        ([str],),
                 },
                 'attribute_map': {
-                    'task_gid': 'task_gid',
-                    'opt_fields': 'opt_fields',
+                    'user_gid': 'user_gid',
+                    'resource_type': 'resource_type',
+                    'workspace': 'workspace',
                     'opt_pretty': 'opt_pretty',
-                    'limit': 'limit',
-                    'offset': 'offset',
+                    'opt_fields': 'opt_fields',
                 },
                 'location_map': {
-                    'task_gid': 'path',
-                    'opt_fields': 'query',
+                    'user_gid': 'path',
+                    'resource_type': 'query',
+                    'workspace': 'query',
                     'opt_pretty': 'query',
-                    'limit': 'query',
-                    'offset': 'query',
+                    'opt_fields': 'query',
                 },
                 'collection_format_map': {
                     'opt_fields': 'csv',
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.get_task_endpoint = _Endpoint(
+        self.get_user_endpoint = _Endpoint(
             settings={
-                'response_type': (GetTask200Response,),
+                'response_type': (GetUser200Response,),
                 'auth': [
-                    'personal_access_token'
+                    'personalAccessToken'
                 ],
-                'endpoint_path': '/tasks/{task_gid}',
-                'operation_id': 'get_task',
+                'endpoint_path': '/users/{user_gid}',
+                'operation_id': 'get_user',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'task_gid',
-                    'opt_fields',
+                    'user_gid',
                     'opt_pretty',
+                    'opt_fields',
                 ],
                 'required': [
-                    'task_gid',
+                    'user_gid',
                 ],
                 'nullable': [
                 ],
                 'enum': [
+                    'opt_fields',
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
+                    ('opt_fields',): {
+
+                        "EMAIL": "email",
+                        "NAME": "name",
+                        "WORKSPACES": "workspaces",
+                        "PHOTO": "photo"
+                    },
                 },
                 'openapi_types': {
-                    'task_gid':
+                    'user_gid':
                         (str,),
-                    'opt_fields':
-                        ([str],),
                     'opt_pretty':
                         (bool,),
+                    'opt_fields':
+                        ([str],),
                 },
                 'attribute_map': {
-                    'task_gid': 'task_gid',
-                    'opt_fields': 'opt_fields',
+                    'user_gid': 'user_gid',
                     'opt_pretty': 'opt_pretty',
+                    'opt_fields': 'opt_fields',
                 },
                 'location_map': {
-                    'task_gid': 'path',
-                    'opt_fields': 'query',
+                    'user_gid': 'path',
                     'opt_pretty': 'query',
+                    'opt_fields': 'query',
                 },
                 'collection_format_map': {
                     'opt_fields': 'csv',
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.get_tasks_endpoint = _Endpoint(
+        self.get_users_endpoint = _Endpoint(
             settings={
-                'response_type': (GetTasksForProject200Response,),
+                'response_type': (GetUsers200Response,),
                 'auth': [
-                    'personal_access_token'
+                    'personalAccessToken'
                 ],
-                'endpoint_path': '/tasks',
-                'operation_id': 'get_tasks',
+                'endpoint_path': '/users',
+                'operation_id': 'get_users',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'opt_fields',
+                    'workspace',
+                    'team',
                     'opt_pretty',
                     'limit',
                     'offset',
-                    'assignee',
-                    'project',
-                    'section',
-                    'workspace',
-                    'completed_since',
-                    'modified_since',
+                    'opt_fields',
                 ],
                 'required': [],
                 'nullable': [
                 ],
                 'enum': [
+                    'opt_fields',
                 ],
                 'validation': [
-                    'limit',
                 ]
             },
             root_map={
                 'validations': {
-                    ('limit',): {
-
-                        'inclusive_maximum': 100,
-                        'inclusive_minimum': 0,
-                    },
                 },
                 'allowed_values': {
+                    ('opt_fields',): {
+
+                        "EMAIL": "email",
+                        "NAME": "name",
+                        "WORKSPACES": "workspaces",
+                        "PHOTO": "photo"
+                    },
                 },
                 'openapi_types': {
-                    'opt_fields':
-                        ([str],),
+                    'workspace':
+                        (str,),
+                    'team':
+                        (str,),
                     'opt_pretty':
                         (bool,),
                     'limit':
                         (int,),
                     'offset':
                         (str,),
-                    'assignee':
-                        (str,),
-                    'project':
-                        (str,),
-                    'section':
-                        (str,),
-                    'workspace':
-                        (str,),
-                    'completed_since':
-                        (datetime,),
-                    'modified_since':
-                        (datetime,),
+                    'opt_fields':
+                        ([str],),
                 },
                 'attribute_map': {
-                    'opt_fields': 'opt_fields',
+                    'workspace': 'workspace',
+                    'team': 'team',
                     'opt_pretty': 'opt_pretty',
                     'limit': 'limit',
                     'offset': 'offset',
-                    'assignee': 'assignee',
-                    'project': 'project',
-                    'section': 'section',
-                    'workspace': 'workspace',
-                    'completed_since': 'completed_since',
-                    'modified_since': 'modified_since',
+                    'opt_fields': 'opt_fields',
                 },
                 'location_map': {
-                    'opt_fields': 'query',
+                    'workspace': 'query',
+                    'team': 'query',
                     'opt_pretty': 'query',
                     'limit': 'query',
                     'offset': 'query',
-                    'assignee': 'query',
-                    'project': 'query',
-                    'section': 'query',
-                    'workspace': 'query',
-                    'completed_since': 'query',
-                    'modified_since': 'query',
+                    'opt_fields': 'query',
                 },
                 'collection_format_map': {
                     'opt_fields': 'csv',
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.get_tasks_for_project_endpoint = _Endpoint(
+        self.get_users_for_team_endpoint = _Endpoint(
             settings={
-                'response_type': (GetTasksForProject200Response,),
+                'response_type': (GetUsers200Response,),
                 'auth': [
-                    'personal_access_token'
+                    'personalAccessToken'
                 ],
-                'endpoint_path': '/projects/{project_gid}/tasks',
-                'operation_id': 'get_tasks_for_project',
+                'endpoint_path': '/teams/{team_gid}/users',
+                'operation_id': 'get_users_for_team',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'project_gid',
-                    'completed_since',
-                    'opt_fields',
+                    'team_gid',
                     'opt_pretty',
-                    'limit',
                     'offset',
+                    'opt_fields',
                 ],
                 'required': [
-                    'project_gid',
+                    'team_gid',
                 ],
                 'nullable': [
                 ],
                 'enum': [
+                    'opt_fields',
                 ],
                 'validation': [
-                    'limit',
                 ]
             },
             root_map={
                 'validations': {
-                    ('limit',): {
-
-                        'inclusive_maximum': 100,
-                        'inclusive_minimum': 0,
-                    },
                 },
                 'allowed_values': {
+                    ('opt_fields',): {
+
+                        "EMAIL": "email",
+                        "NAME": "name",
+                        "WORKSPACES": "workspaces",
+                        "PHOTO": "photo"
+                    },
                 },
                 'openapi_types': {
-                    'project_gid':
+                    'team_gid':
                         (str,),
-                    'completed_since':
+                    'opt_pretty':
+                        (bool,),
+                    'offset':
                         (str,),
                     'opt_fields':
                         ([str],),
+                },
+                'attribute_map': {
+                    'team_gid': 'team_gid',
+                    'opt_pretty': 'opt_pretty',
+                    'offset': 'offset',
+                    'opt_fields': 'opt_fields',
+                },
+                'location_map': {
+                    'team_gid': 'path',
+                    'opt_pretty': 'query',
+                    'offset': 'query',
+                    'opt_fields': 'query',
+                },
+                'collection_format_map': {
+                    'opt_fields': 'csv',
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.get_users_for_workspace_endpoint = _Endpoint(
+            settings={
+                'response_type': (GetUsers200Response,),
+                'auth': [
+                    'personalAccessToken'
+                ],
+                'endpoint_path': '/workspaces/{workspace_gid}/users',
+                'operation_id': 'get_users_for_workspace',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'workspace_gid',
+                    'opt_pretty',
+                    'offset',
+                    'opt_fields',
+                ],
+                'required': [
+                    'workspace_gid',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                    'opt_fields',
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                    ('opt_fields',): {
+
+                        "EMAIL": "email",
+                        "NAME": "name",
+                        "WORKSPACES": "workspaces",
+                        "PHOTO": "photo"
+                    },
+                },
+                'openapi_types': {
+                    'workspace_gid':
+                        (str,),
                     'opt_pretty':
                         (bool,),
-                    'limit':
-                        (int,),
                     'offset':
                         (str,),
+                    'opt_fields':
+                        ([str],),
                 },
                 'attribute_map': {
-                    'project_gid': 'project_gid',
-                    'completed_since': 'completed_since',
-                    'opt_fields': 'opt_fields',
+                    'workspace_gid': 'workspace_gid',
                     'opt_pretty': 'opt_pretty',
-                    'limit': 'limit',
                     'offset': 'offset',
+                    'opt_fields': 'opt_fields',
                 },
                 'location_map': {
-                    'project_gid': 'path',
-                    'completed_since': 'query',
-                    'opt_fields': 'query',
+                    'workspace_gid': 'path',
                     'opt_pretty': 'query',
-                    'limit': 'query',
                     'offset': 'query',
+                    'opt_fields': 'query',
                 },
                 'collection_format_map': {
                     'opt_fields': 'csv',
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
 
-    def get_subtasks_for_task(
+    def get_favorites_for_user(
         self,
-        task_gid,
+        user_gid,
+        workspace,
+        resource_type="project",
         **kwargs
     ):
-        """Get subtasks from a task  # noqa: E501
+        """Get a user's favorites  # noqa: E501
 
-        Returns a compact representation of all of the subtasks of a task.  # noqa: E501
+        Returns all of a user's favorites in the given workspace, of the given type. Results are given in order (The same order as Asana's sidebar).  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_subtasks_for_task(task_gid, async_req=True)
+        >>> thread = api.get_favorites_for_user(user_gid, workspace, resource_type="project", async_req=True)
         >>> result = thread.get()
 
         Args:
-            task_gid (str): The task to operate on.
+            user_gid (str): A string identifying a user. This can either be the string \"me\", an email, or the gid of a user.
+            workspace (str): The workspace in which to get favorites.
+            resource_type (str): The resource type of favorites to be returned.. defaults to "project", must be one of ["project"]
 
         Keyword Args:
-            opt_fields ([str]): Defines fields to return.  Some requests return *compact* representations of objects in order to conserve resources and complete the request more efficiently. Other times requests return more information than you may need. This option allows you to list the exact set of fields that the API should be sure to return for the objects. The field names should be provided as paths, described below.  The gid of included objects will always be returned, regardless of the field options.. [optional]
             opt_pretty (bool): Provides “pretty” output. Provides the response in a “pretty” format. In the case of JSON this means doing proper line breaking and indentation to make it readable. This will take extra time and increase the response size so it is advisable only to use this during debugging.. [optional]
-            limit (int): The number of objects to return per page. The value must be between 1 and 100.. [optional]
-            offset (str): Offset token.  An offset to the next page returned by the API. A pagination request will return an offset token, which can be used as an input parameter to the next request. If an offset is not passed in, the API will return the first page of results.  'Note: You can only pass in an offset that was returned to you via a previously paginated request.. [optional]
+            opt_fields ([str]): This endpoint returns a compact resource, which excludes some properties by default. To include those optional properties, set this query parameter to a comma-separated list of the properties you wish to include.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -416,15 +483,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            GetTasksForProject200Response
+            GetFavoritesForUser200Response
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -445,38 +512,128 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['task_gid'] = \
-            task_gid
-        return self.get_subtasks_for_task_endpoint.call_with_http_info(**kwargs)
+        kwargs['user_gid'] = \
+            user_gid
+        kwargs['resource_type'] = \
+            resource_type
+        kwargs['workspace'] = \
+            workspace
+        return self.get_favorites_for_user_endpoint.call_with_http_info(**kwargs)
 
-    def get_task(
+    def get_user(
         self,
-        task_gid,
+        user_gid,
         **kwargs
     ):
-        """Get a task  # noqa: E501
+        """Get a user  # noqa: E501
 
-        Returns the complete task record for a single task.  # noqa: E501
+        Returns the full user record for the single user with the provided ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_task(task_gid, async_req=True)
+        >>> thread = api.get_user(user_gid, async_req=True)
         >>> result = thread.get()
 
         Args:
-            task_gid (str): The task to operate on.
+            user_gid (str): A string identifying a user. This can either be the string \"me\", an email, or the gid of a user.
+
+        Keyword Args:
+            opt_pretty (bool): Provides “pretty” output. Provides the response in a “pretty” format. In the case of JSON this means doing proper line breaking and indentation to make it readable. This will take extra time and increase the response size so it is advisable only to use this during debugging.. [optional]
+            opt_fields ([str]): This endpoint returns a compact resource, which excludes some properties by default. To include those optional properties, set this query parameter to a comma-separated list of the properties you wish to include.. [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            GetUser200Response
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['user_gid'] = \
+            user_gid
+        return self.get_user_endpoint.call_with_http_info(**kwargs)
+
+    def get_users(
+        self,
+        **kwargs
+    ):
+        """Get multiple users  # noqa: E501
+
+        Returns the user records for all users in all workspaces and organizations accessible to the authenticated user. Accepts an optional workspace ID parameter. Results are sorted by user ID.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_users(async_req=True)
+        >>> result = thread.get()
+
 
         Keyword Args:
-            opt_fields ([str]): Defines fields to return.  Some requests return *compact* representations of objects in order to conserve resources and complete the request more efficiently. Other times requests return more information than you may need. This option allows you to list the exact set of fields that the API should be sure to return for the objects. The field names should be provided as paths, described below.  The gid of included objects will always be returned, regardless of the field options.. [optional]
+            workspace (str): The workspace or organization ID to filter users on.. [optional]
+            team (str): The team ID to filter users on.. [optional]
             opt_pretty (bool): Provides “pretty” output. Provides the response in a “pretty” format. In the case of JSON this means doing proper line breaking and indentation to make it readable. This will take extra time and increase the response size so it is advisable only to use this during debugging.. [optional]
+            limit (int): Results per page. The number of objects to return per page. The value must be between 1 and 100.. [optional]
+            offset (str): Offset token. An offset to the next page returned by the API. A pagination request will return an offset token, which can be used as an input parameter to the next request. If an offset is not passed in, the API will return the first page of results. 'Note: You can only pass in an offset that was returned to you via a previously paginated request.'. [optional]
+            opt_fields ([str]): This endpoint returns a compact resource, which excludes some properties by default. To include those optional properties, set this query parameter to a comma-separated list of the properties you wish to include.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -501,15 +658,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            GetTask200Response
+            GetUsers200Response
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -530,43 +687,37 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['task_gid'] = \
-            task_gid
-        return self.get_task_endpoint.call_with_http_info(**kwargs)
+        return self.get_users_endpoint.call_with_http_info(**kwargs)
 
-    def get_tasks(
+    def get_users_for_team(
         self,
+        team_gid,
         **kwargs
     ):
-        """Get multiple tasks  # noqa: E501
+        """Get users in a team  # noqa: E501
 
-        Returns the compact task records for some filtered set of tasks. Use one or more of the parameters provided to filter the tasks returned. You must specify a `project` or `tag` if you do not specify `assignee` and `workspace`.  For more complex task retrieval, use [workspaces/{workspace_gid}/tasks/search](/reference/searchtasksforworkspace).  # noqa: E501
+        Returns the compact records for all users that are members of the team. Results are sorted alphabetically and limited to 2000. For more results use the `/users` endpoint.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_tasks(async_req=True)
+        >>> thread = api.get_users_for_team(team_gid, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            team_gid (str): Globally unique identifier for the team.
 
         Keyword Args:
-            opt_fields ([str]): Defines fields to return.  Some requests return *compact* representations of objects in order to conserve resources and complete the request more efficiently. Other times requests return more information than you may need. This option allows you to list the exact set of fields that the API should be sure to return for the objects. The field names should be provided as paths, described below.  The gid of included objects will always be returned, regardless of the field options.. [optional]
             opt_pretty (bool): Provides “pretty” output. Provides the response in a “pretty” format. In the case of JSON this means doing proper line breaking and indentation to make it readable. This will take extra time and increase the response size so it is advisable only to use this during debugging.. [optional]
-            limit (int): The number of objects to return per page. The value must be between 1 and 100.. [optional]
-            offset (str): Offset token.  An offset to the next page returned by the API. A pagination request will return an offset token, which can be used as an input parameter to the next request. If an offset is not passed in, the API will return the first page of results.  'Note: You can only pass in an offset that was returned to you via a previously paginated request.. [optional]
-            assignee (str): The assignee to filter tasks on. If searching for unassigned tasks, assignee.any = null can be specified.  *Note: If you specify `assignee`, you must also specify the `workspace` to filter on.*. [optional]
-            project (str): The project to filter tasks on.. [optional]
-            section (str): The section to filter tasks on.. [optional]
-            workspace (str): The workspace to filter tasks on.  *Note: If you specify `workspace`, you must also specify the `assignee` to filter on.*. [optional]
-            completed_since (datetime): Only return tasks that are either incomplete or that have been completed since this time.. [optional]
-            modified_since (datetime): Only return tasks that have been modified since the given time.  *Note: A task is considered “modified” if any of its properties change, or associations between it and other objects are modified (e.g.  a task being added to a project). A task is not considered modified just because another object it is associated with (e.g. a subtask) is modified. Actions that count as modifying the task include assigning, renaming, completing, and adding stories.*. [optional]
+            offset (str): Offset token. An offset to the next page returned by the API. A pagination request will return an offset token, which can be used as an input parameter to the next request. If an offset is not passed in, the API will return the first page of results. 'Note: You can only pass in an offset that was returned to you via a previously paginated request.'. [optional]
+            opt_fields ([str]): This endpoint returns a compact resource, which excludes some properties by default. To include those optional properties, set this query parameter to a comma-separated list of the properties you wish to include.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -591,15 +742,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            GetTasksForProject200Response
+            GetUsers200Response
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -620,39 +771,39 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        return self.get_tasks_endpoint.call_with_http_info(**kwargs)
+        kwargs['team_gid'] = \
+            team_gid
+        return self.get_users_for_team_endpoint.call_with_http_info(**kwargs)
 
-    def get_tasks_for_project(
+    def get_users_for_workspace(
         self,
-        project_gid,
+        workspace_gid,
         **kwargs
     ):
-        """Get tasks from a project  # noqa: E501
+        """Get users in a workspace or organization  # noqa: E501
 
-        Returns the compact task records for all tasks within the given project, ordered by their priority within the project. Tasks can exist in more than one project at a time.  # noqa: E501
+        Returns the compact records for all users in the specified workspace or organization. Results are sorted alphabetically and limited to 2000. For more results use the `/users` endpoint.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_tasks_for_project(project_gid, async_req=True)
+        >>> thread = api.get_users_for_workspace(workspace_gid, async_req=True)
         >>> result = thread.get()
 
         Args:
-            project_gid (str): Globally unique identifier for the project.
+            workspace_gid (str): Globally unique identifier for the workspace or organization.
 
         Keyword Args:
-            completed_since (str): Only return tasks that are either incomplete or that have been completed since this time. Accepts a date-time string or the keyword *now*.. [optional]
-            opt_fields ([str]): Defines fields to return.  Some requests return *compact* representations of objects in order to conserve resources and complete the request more efficiently. Other times requests return more information than you may need. This option allows you to list the exact set of fields that the API should be sure to return for the objects. The field names should be provided as paths, described below.  The gid of included objects will always be returned, regardless of the field options.. [optional]
             opt_pretty (bool): Provides “pretty” output. Provides the response in a “pretty” format. In the case of JSON this means doing proper line breaking and indentation to make it readable. This will take extra time and increase the response size so it is advisable only to use this during debugging.. [optional]
-            limit (int): The number of objects to return per page. The value must be between 1 and 100.. [optional]
-            offset (str): Offset token.  An offset to the next page returned by the API. A pagination request will return an offset token, which can be used as an input parameter to the next request. If an offset is not passed in, the API will return the first page of results.  'Note: You can only pass in an offset that was returned to you via a previously paginated request.. [optional]
+            offset (str): Offset token. An offset to the next page returned by the API. A pagination request will return an offset token, which can be used as an input parameter to the next request. If an offset is not passed in, the API will return the first page of results. 'Note: You can only pass in an offset that was returned to you via a previously paginated request.'. [optional]
+            opt_fields ([str]): This endpoint returns a compact resource, which excludes some properties by default. To include those optional properties, set this query parameter to a comma-separated list of the properties you wish to include.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -677,15 +828,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            GetTasksForProject200Response
+            GetUsers200Response
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -706,11 +857,11 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['project_gid'] = \
-            project_gid
-        return self.get_tasks_for_project_endpoint.call_with_http_info(**kwargs)
+        kwargs['workspace_gid'] = \
+            workspace_gid
+        return self.get_users_for_workspace_endpoint.call_with_http_info(**kwargs)
```

### Comparing `asana-preview-1.0.4/asana_preview/api/users_api.py` & `asana-preview-1.0.5/asana_preview/api/rules_api.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -18,115 +18,120 @@
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
 from asana_preview.model.error_response import ErrorResponse
-from asana_preview.model.get_events401_response import GetEvents401Response
-from asana_preview.model.get_events403_response import GetEvents403Response
-from asana_preview.model.get_events404_response import GetEvents404Response
-from asana_preview.model.get_events500_response import GetEvents500Response
-from asana_preview.model.get_user200_response import GetUser200Response
+from asana_preview.model.trigger_rule200_response import TriggerRule200Response
+from asana_preview.model.trigger_rule_request import TriggerRuleRequest
 
 
-class UsersApi(object):
+class RulesApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
-        self.get_user_endpoint = _Endpoint(
+        self.trigger_rule_endpoint = _Endpoint(
             settings={
-                'response_type': (GetUser200Response,),
+                'response_type': (TriggerRule200Response,),
                 'auth': [
-                    'personal_access_token'
+                    'personalAccessToken'
                 ],
-                'endpoint_path': '/users/{user_gid}',
-                'operation_id': 'get_user',
-                'http_method': 'GET',
+                'endpoint_path': '/rule_triggers/{rule_trigger_gid}/run',
+                'operation_id': 'trigger_rule',
+                'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'user_gid',
+                    'rule_trigger_gid',
+                    'trigger_rule_request',
                     'opt_fields',
-                    'opt_pretty',
                 ],
                 'required': [
-                    'user_gid',
+                    'rule_trigger_gid',
+                    'trigger_rule_request',
                 ],
                 'nullable': [
                 ],
                 'enum': [
+                    'opt_fields',
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
+                    ('opt_fields',): {
+
+                        "MESSAGE": "message"
+                    },
                 },
                 'openapi_types': {
-                    'user_gid':
+                    'rule_trigger_gid':
                         (str,),
+                    'trigger_rule_request':
+                        (TriggerRuleRequest,),
                     'opt_fields':
                         ([str],),
-                    'opt_pretty':
-                        (bool,),
                 },
                 'attribute_map': {
-                    'user_gid': 'user_gid',
+                    'rule_trigger_gid': 'rule_trigger_gid',
                     'opt_fields': 'opt_fields',
-                    'opt_pretty': 'opt_pretty',
                 },
                 'location_map': {
-                    'user_gid': 'path',
+                    'rule_trigger_gid': 'path',
+                    'trigger_rule_request': 'body',
                     'opt_fields': 'query',
-                    'opt_pretty': 'query',
                 },
                 'collection_format_map': {
                     'opt_fields': 'csv',
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
-                'content_type': [],
+                'content_type': [
+                    'application/json'
+                ]
             },
             api_client=api_client
         )
 
-    def get_user(
+    def trigger_rule(
         self,
-        user_gid,
+        rule_trigger_gid,
+        trigger_rule_request,
         **kwargs
     ):
-        """Get a user  # noqa: E501
+        """Trigger a rule  # noqa: E501
 
-        Returns the full user record for the single user with the provided ID.  # noqa: E501
+        Trigger a rule which uses an [\"incoming web request\"](/docs/incoming-web-requests) trigger.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_user(user_gid, async_req=True)
+        >>> thread = api.trigger_rule(rule_trigger_gid, trigger_rule_request, async_req=True)
         >>> result = thread.get()
 
         Args:
-            user_gid (str): A string identifying a user. This can either be the string \"me\", an email, or the gid of a user.
+            rule_trigger_gid (str): The ID of the incoming web request trigger. This value is a path parameter that is automatically generated for the API endpoint.
+            trigger_rule_request (TriggerRuleRequest): A dictionary of variables accessible from within the rule.
 
         Keyword Args:
-            opt_fields ([str]): Defines fields to return.  Some requests return *compact* representations of objects in order to conserve resources and complete the request more efficiently. Other times requests return more information than you may need. This option allows you to list the exact set of fields that the API should be sure to return for the objects. The field names should be provided as paths, described below.  The gid of included objects will always be returned, regardless of the field options.. [optional]
-            opt_pretty (bool): Provides “pretty” output. Provides the response in a “pretty” format. In the case of JSON this means doing proper line breaking and indentation to make it readable. This will take extra time and increase the response size so it is advisable only to use this during debugging.. [optional]
+            opt_fields ([str]): This endpoint returns a compact resource, which excludes some properties by default. To include those optional properties, set this query parameter to a comma-separated list of the properties you wish to include.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -151,15 +156,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            GetUser200Response
+            TriggerRule200Response
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -180,11 +185,13 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['user_gid'] = \
-            user_gid
-        return self.get_user_endpoint.call_with_http_info(**kwargs)
+        kwargs['rule_trigger_gid'] = \
+            rule_trigger_gid
+        kwargs['trigger_rule_request'] = \
+            trigger_rule_request
+        return self.trigger_rule_endpoint.call_with_http_info(**kwargs)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `asana-preview-1.0.4/asana_preview/api_client.py` & `asana-preview-1.0.5/asana_preview/api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import json
 import atexit
 import mimetypes
@@ -73,20 +73,20 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.0.4/python'
+        self.user_agent = 'OpenAPI-Generator/1.0.5/python'
         # Add custom header
         self.default_headers['X-Asana-Client-Lib'] = urlencode(
             {
                 'language': 'PythonPreview',
-                'version': "1.0.4",
+                'version': "1.0.5",
                 'language_version': platform.python_version(),
                 'os': platform.system(),
                 'os_version': platform.release()
             }
         )
 
     def __enter__(self):
@@ -808,19 +808,19 @@
 
         return params
 
     def __call__(self, *args, **kwargs):
         """ This method is invoked when endpoints are called
         Example:
 
-        api_instance = EventsApi()
-        api_instance.get_events  # this is an instance of the class Endpoint
-        api_instance.get_events()  # this invokes api_instance.get_events.__call__()
+        api_instance = AttachmentsApi()
+        api_instance.create_attachment_for_object  # this is an instance of the class Endpoint
+        api_instance.create_attachment_for_object()  # this invokes api_instance.create_attachment_for_object.__call__()
         which then invokes the callable functions stored in that endpoint at
-        api_instance.get_events.callable or self.callable in this class
+        api_instance.create_attachment_for_object.callable or self.callable in this class
 
         """
         return self.callable(self, *args, **kwargs)
 
     def call_with_http_info(self, **kwargs):
 
         try:
```

### Comparing `asana-preview-1.0.4/asana_preview/configuration.py` & `asana-preview-1.0.5/asana_preview/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import copy
 import logging
 import multiprocessing
@@ -367,15 +367,15 @@
     def auth_settings(self):
         """Gets Auth Settings dict for api client.
 
         :return: The Auth Settings information dict.
         """
         auth = {}
         if self.access_token is not None:
-            auth['personal_access_token'] = {
+            auth['personalAccessToken'] = {
                 'type': 'bearer',
                 'in': 'header',
                 'key': 'Authorization',
                 'value': 'Bearer ' + self.access_token
             }
         return auth
 
@@ -383,27 +383,27 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.0.0\n"\
-               "SDK Package Version: 1.0.4".\
+               "Version of the API: 1.0\n"\
+               "SDK Package Version: 1.0.5".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
         return [
             {
                 'url': "https://app.asana.com/api/1.0",
-                'description': "No description provided",
+                'description': "Main endpoint.",
             }
         ]
 
     def get_host_from_settings(self, index, variables=None, servers=None):
         """Gets host URL based on the index and variables
         :param index: array index of the host settings
         :param variables: hash of variable and the corresponding value
```

### Comparing `asana-preview-1.0.4/asana_preview/exceptions.py` & `asana-preview-1.0.5/asana_preview/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
```

### Comparing `asana-preview-1.0.4/asana_preview/model/asana_named_resource.py` & `asana-preview-1.0.5/asana_preview/model/asana_named_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `asana-preview-1.0.4/asana_preview/model/asana_named_resource_all_of.py` & `asana-preview-1.0.5/asana_preview/model/user_compact_all_of.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from asana_preview.exceptions import ApiAttributeError
 
 
 
-class AsanaNamedResourceAllOf(ModelNormal):
+class UserCompactAllOf(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -97,15 +97,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """AsanaNamedResourceAllOf - a model defined in OpenAPI
+        """UserCompactAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -130,15 +130,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): The name of the object.. [optional]  # noqa: E501
+            name (str): *Read-only except when same user as requester*. The user’s name.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -183,15 +183,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """AsanaNamedResourceAllOf - a model defined in OpenAPI
+        """UserCompactAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -216,15 +216,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): The name of the object.. [optional]  # noqa: E501
+            name (str): *Read-only except when same user as requester*. The user’s name.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `asana-preview-1.0.4/asana_preview/model/asana_resource.py` & `asana-preview-1.0.5/asana_preview/model/asana_resource.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `asana-preview-1.0.4/asana_preview/model/custom_field_base.py` & `asana-preview-1.0.5/asana_preview/model/custom_field_compact.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,25 +26,25 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from asana_preview.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from asana_preview.model.custom_field_base_all_of import CustomFieldBaseAllOf
-    from asana_preview.model.custom_field_compact import CustomFieldCompact
+    from asana_preview.model.asana_resource import AsanaResource
+    from asana_preview.model.custom_field_compact_all_of import CustomFieldCompactAllOf
     from asana_preview.model.custom_field_compact_all_of_date_value import CustomFieldCompactAllOfDateValue
     from asana_preview.model.enum_option import EnumOption
-    globals()['CustomFieldBaseAllOf'] = CustomFieldBaseAllOf
-    globals()['CustomFieldCompact'] = CustomFieldCompact
+    globals()['AsanaResource'] = AsanaResource
+    globals()['CustomFieldCompactAllOf'] = CustomFieldCompactAllOf
     globals()['CustomFieldCompactAllOfDateValue'] = CustomFieldCompactAllOfDateValue
     globals()['EnumOption'] = EnumOption
 
 
-class CustomFieldBase(ModelComposed):
+class CustomFieldCompact(ModelComposed):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -75,25 +75,14 @@
         },
         ('type',): {
             'TEXT': "text",
             'ENUM': "enum",
             'MULTI_ENUM': "multi_enum",
             'NUMBER': "number",
         },
-        ('format',): {
-            'CURRENCY': "currency",
-            'IDENTIFIER': "identifier",
-            'PERCENTAGE': "percentage",
-            'CUSTOM': "custom",
-            'NONE': "none",
-        },
-        ('custom_label_position',): {
-            'PREFIX': "prefix",
-            'SUFFIX': "suffix",
-        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
@@ -115,33 +104,27 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'gid': (str,),  # noqa: E501
-            'resource_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'resource_type': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'resource_subtype': (str,),  # noqa: E501
             'type': (str,),  # noqa: E501
             'enum_options': ([EnumOption],),  # noqa: E501
             'enabled': (bool,),  # noqa: E501
+            'is_formula_field': (bool,),  # noqa: E501
             'date_value': (CustomFieldCompactAllOfDateValue,),  # noqa: E501
             'enum_value': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'multi_enum_values': ([EnumOption],),  # noqa: E501
-            'number_value': (float,),  # noqa: E501
-            'text_value': (str,),  # noqa: E501
+            'number_value': (float, none_type,),  # noqa: E501
+            'text_value': (str, none_type,),  # noqa: E501
             'display_value': (str, none_type,),  # noqa: E501
-            'description': (str,),  # noqa: E501
-            'precision': (int,),  # noqa: E501
-            'format': (str,),  # noqa: E501
-            'currency_code': (str, none_type,),  # noqa: E501
-            'custom_label': (str, none_type,),  # noqa: E501
-            'custom_label_position': (str,),  # noqa: E501
-            'has_notifications_enabled': (bool,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -149,39 +132,34 @@
         'gid': 'gid',  # noqa: E501
         'resource_type': 'resource_type',  # noqa: E501
         'name': 'name',  # noqa: E501
         'resource_subtype': 'resource_subtype',  # noqa: E501
         'type': 'type',  # noqa: E501
         'enum_options': 'enum_options',  # noqa: E501
         'enabled': 'enabled',  # noqa: E501
+        'is_formula_field': 'is_formula_field',  # noqa: E501
         'date_value': 'date_value',  # noqa: E501
         'enum_value': 'enum_value',  # noqa: E501
         'multi_enum_values': 'multi_enum_values',  # noqa: E501
         'number_value': 'number_value',  # noqa: E501
         'text_value': 'text_value',  # noqa: E501
         'display_value': 'display_value',  # noqa: E501
-        'description': 'description',  # noqa: E501
-        'precision': 'precision',  # noqa: E501
-        'format': 'format',  # noqa: E501
-        'currency_code': 'currency_code',  # noqa: E501
-        'custom_label': 'custom_label',  # noqa: E501
-        'custom_label_position': 'custom_label_position',  # noqa: E501
-        'has_notifications_enabled': 'has_notifications_enabled',  # noqa: E501
     }
 
     read_only_vars = {
         'gid',  # noqa: E501
+        'resource_type',  # noqa: E501
         'type',  # noqa: E501
         'display_value',  # noqa: E501
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """CustomFieldBase - a model defined in OpenAPI
+        """CustomFieldCompact - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -207,33 +185,27 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
             name (str): The name of the custom field.. [optional]  # noqa: E501
-            resource_subtype (str): The type of the custom field. Must be one of the given values.. [optional]  # noqa: E501
-            type (str): *Deprecated: new integrations should prefer the resource_subtype field.* The type of the custom field. Must be one of the given values.. [optional]  # noqa: E501
+            resource_subtype (str): The type of the custom field. Must be one of the given values. . [optional]  # noqa: E501
+            type (str): *Deprecated: new integrations should prefer the resource_subtype field.* The type of the custom field. Must be one of the given values. . [optional]  # noqa: E501
             enum_options ([EnumOption]): *Conditional*. Only relevant for custom fields of type `enum`. This array specifies the possible values which an `enum` custom field can adopt. To modify the enum options, refer to [working with enum options](/reference/createenumoptionforcustomfield).. [optional]  # noqa: E501
             enabled (bool): *Conditional*. Determines if the custom field is enabled or not.. [optional]  # noqa: E501
+            is_formula_field (bool): *Conditional*. This flag describes whether a custom field is a formula custom field.. [optional]  # noqa: E501
             date_value (CustomFieldCompactAllOfDateValue): [optional]  # noqa: E501
             enum_value (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             multi_enum_values ([EnumOption]): *Conditional*. Only relevant for custom fields of type `multi_enum`. This object is the chosen values of a `multi_enum` custom field.. [optional]  # noqa: E501
-            number_value (float): *Conditional*. This number is the value of a `number` custom field.. [optional]  # noqa: E501
-            text_value (str): *Conditional*. This string is the value of a `text` custom field.. [optional]  # noqa: E501
+            number_value (float, none_type): *Conditional*. This number is the value of a `number` custom field.. [optional]  # noqa: E501
+            text_value (str, none_type): *Conditional*. This string is the value of a `text` custom field.. [optional]  # noqa: E501
             display_value (str, none_type): A string representation for the value of the custom field. Integrations that don't require the underlying type should use this field to read values. Using this field will future-proof an app against new custom field types.. [optional]  # noqa: E501
-            description (str): [Opt In](/docs/inputoutput-options). The description of the custom field.. [optional]  # noqa: E501
-            precision (int): Only relevant for custom fields of type ‘Number’. This field dictates the number of places after the decimal to round to, i.e. 0 is integer values, 1 rounds to the nearest tenth, and so on. Must be between 0 and 6, inclusive. For percentage format, this may be unintuitive, as a value of 0.25 has a precision of 0, while a value of 0.251 has a precision of 1. This is due to 0.25 being displayed as 25%. The identifier format will always have a precision of 0.. [optional]  # noqa: E501
-            format (str): The format of this custom field.. [optional]  # noqa: E501
-            currency_code (str, none_type): ISO 4217 currency code to format this custom field. This will be null if the `format` is not `currency`.. [optional]  # noqa: E501
-            custom_label (str, none_type): This is the string that appears next to the custom field value. This will be null if the `format` is not `custom`.. [optional]  # noqa: E501
-            custom_label_position (str): Only relevant for custom fields with `custom` format. This depicts where to place the custom label. This will be null if the `format` is not `custom`.. [optional]  # noqa: E501
-            has_notifications_enabled (bool): *Conditional*. This flag describes whether a follower of a task with this field should receive inbox notifications from changes to this field.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -296,15 +268,15 @@
         '_composed_instances',
         '_var_name_to_model_instances',
         '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """CustomFieldBase - a model defined in OpenAPI
+        """CustomFieldCompact - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -330,33 +302,27 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
             name (str): The name of the custom field.. [optional]  # noqa: E501
-            resource_subtype (str): The type of the custom field. Must be one of the given values.. [optional]  # noqa: E501
-            type (str): *Deprecated: new integrations should prefer the resource_subtype field.* The type of the custom field. Must be one of the given values.. [optional]  # noqa: E501
+            resource_subtype (str): The type of the custom field. Must be one of the given values. . [optional]  # noqa: E501
+            type (str): *Deprecated: new integrations should prefer the resource_subtype field.* The type of the custom field. Must be one of the given values. . [optional]  # noqa: E501
             enum_options ([EnumOption]): *Conditional*. Only relevant for custom fields of type `enum`. This array specifies the possible values which an `enum` custom field can adopt. To modify the enum options, refer to [working with enum options](/reference/createenumoptionforcustomfield).. [optional]  # noqa: E501
             enabled (bool): *Conditional*. Determines if the custom field is enabled or not.. [optional]  # noqa: E501
+            is_formula_field (bool): *Conditional*. This flag describes whether a custom field is a formula custom field.. [optional]  # noqa: E501
             date_value (CustomFieldCompactAllOfDateValue): [optional]  # noqa: E501
             enum_value (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             multi_enum_values ([EnumOption]): *Conditional*. Only relevant for custom fields of type `multi_enum`. This object is the chosen values of a `multi_enum` custom field.. [optional]  # noqa: E501
-            number_value (float): *Conditional*. This number is the value of a `number` custom field.. [optional]  # noqa: E501
-            text_value (str): *Conditional*. This string is the value of a `text` custom field.. [optional]  # noqa: E501
+            number_value (float, none_type): *Conditional*. This number is the value of a `number` custom field.. [optional]  # noqa: E501
+            text_value (str, none_type): *Conditional*. This string is the value of a `text` custom field.. [optional]  # noqa: E501
             display_value (str, none_type): A string representation for the value of the custom field. Integrations that don't require the underlying type should use this field to read values. Using this field will future-proof an app against new custom field types.. [optional]  # noqa: E501
-            description (str): [Opt In](/docs/inputoutput-options). The description of the custom field.. [optional]  # noqa: E501
-            precision (int): Only relevant for custom fields of type ‘Number’. This field dictates the number of places after the decimal to round to, i.e. 0 is integer values, 1 rounds to the nearest tenth, and so on. Must be between 0 and 6, inclusive. For percentage format, this may be unintuitive, as a value of 0.25 has a precision of 0, while a value of 0.251 has a precision of 1. This is due to 0.25 being displayed as 25%. The identifier format will always have a precision of 0.. [optional]  # noqa: E501
-            format (str): The format of this custom field.. [optional]  # noqa: E501
-            currency_code (str, none_type): ISO 4217 currency code to format this custom field. This will be null if the `format` is not `currency`.. [optional]  # noqa: E501
-            custom_label (str, none_type): This is the string that appears next to the custom field value. This will be null if the `format` is not `custom`.. [optional]  # noqa: E501
-            custom_label_position (str): Only relevant for custom fields with `custom` format. This depicts where to place the custom label. This will be null if the `format` is not `custom`.. [optional]  # noqa: E501
-            has_notifications_enabled (bool): *Conditional*. This flag describes whether a follower of a task with this field should receive inbox notifications from changes to this field.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -418,13 +384,13 @@
         # classes don't exist yet because their module has not finished
         # loading
         lazy_import()
         return {
           'anyOf': [
           ],
           'allOf': [
-              CustomFieldBaseAllOf,
-              CustomFieldCompact,
+              AsanaResource,
+              CustomFieldCompactAllOf,
           ],
           'oneOf': [
           ],
         }
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `asana-preview-1.0.4/asana_preview/model/custom_field_base_all_of.py` & `asana-preview-1.0.5/asana_preview/model/story_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -25,16 +25,22 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from asana_preview.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from asana_preview.model.asana_resource import AsanaResource
+    from asana_preview.model.story_base_all_of import StoryBaseAllOf
+    globals()['AsanaResource'] = AsanaResource
+    globals()['StoryBaseAllOf'] = StoryBaseAllOf
 
-class CustomFieldBaseAllOf(ModelNormal):
+
+class StoryBase(ModelComposed):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -51,84 +57,93 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('format',): {
-            'CURRENCY': "currency",
-            'IDENTIFIER': "identifier",
-            'PERCENTAGE': "percentage",
-            'CUSTOM': "custom",
-            'NONE': "none",
-        },
-        ('custom_label_position',): {
-            'PREFIX': "prefix",
-            'SUFFIX': "suffix",
+        ('sticker_name',): {
+            'GREEN_CHECKMARK': "green_checkmark",
+            'PEOPLE_DANCING': "people_dancing",
+            'DANCING_UNICORN': "dancing_unicorn",
+            'HEART': "heart",
+            'PARTY_POPPER': "party_popper",
+            'PEOPLE_WAVING_FLAGS': "people_waving_flags",
+            'SPLASHING_NARWHAL': "splashing_narwhal",
+            'TROPHY': "trophy",
+            'YETI_RIDING_UNICORN': "yeti_riding_unicorn",
+            'CELEBRATING_PEOPLE': "celebrating_people",
+            'DETERMINED_CLIMBERS': "determined_climbers",
+            'PHOENIX_SPREADING_LOVE': "phoenix_spreading_love",
         },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'description': (str,),  # noqa: E501
-            'precision': (int,),  # noqa: E501
-            'format': (str,),  # noqa: E501
-            'currency_code': (str, none_type,),  # noqa: E501
-            'custom_label': (str, none_type,),  # noqa: E501
-            'custom_label_position': (str,),  # noqa: E501
-            'has_notifications_enabled': (bool,),  # noqa: E501
+            'gid': (str,),  # noqa: E501
+            'resource_type': (str,),  # noqa: E501
+            'created_at': (datetime,),  # noqa: E501
+            'resource_subtype': (str,),  # noqa: E501
+            'text': (str,),  # noqa: E501
+            'html_text': (str,),  # noqa: E501
+            'is_pinned': (bool,),  # noqa: E501
+            'sticker_name': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'description': 'description',  # noqa: E501
-        'precision': 'precision',  # noqa: E501
-        'format': 'format',  # noqa: E501
-        'currency_code': 'currency_code',  # noqa: E501
-        'custom_label': 'custom_label',  # noqa: E501
-        'custom_label_position': 'custom_label_position',  # noqa: E501
-        'has_notifications_enabled': 'has_notifications_enabled',  # noqa: E501
+        'gid': 'gid',  # noqa: E501
+        'resource_type': 'resource_type',  # noqa: E501
+        'created_at': 'created_at',  # noqa: E501
+        'resource_subtype': 'resource_subtype',  # noqa: E501
+        'text': 'text',  # noqa: E501
+        'html_text': 'html_text',  # noqa: E501
+        'is_pinned': 'is_pinned',  # noqa: E501
+        'sticker_name': 'sticker_name',  # noqa: E501
     }
 
     read_only_vars = {
+        'gid',  # noqa: E501
+        'resource_type',  # noqa: E501
+        'created_at',  # noqa: E501
+        'resource_subtype',  # noqa: E501
     }
 
-    _composed_schemas = {}
-
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """CustomFieldBaseAllOf - a model defined in OpenAPI
+        """StoryBase - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -153,25 +168,26 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            description (str): [Opt In](/docs/inputoutput-options). The description of the custom field.. [optional]  # noqa: E501
-            precision (int): Only relevant for custom fields of type ‘Number’. This field dictates the number of places after the decimal to round to, i.e. 0 is integer values, 1 rounds to the nearest tenth, and so on. Must be between 0 and 6, inclusive. For percentage format, this may be unintuitive, as a value of 0.25 has a precision of 0, while a value of 0.251 has a precision of 1. This is due to 0.25 being displayed as 25%. The identifier format will always have a precision of 0.. [optional]  # noqa: E501
-            format (str): The format of this custom field.. [optional]  # noqa: E501
-            currency_code (str, none_type): ISO 4217 currency code to format this custom field. This will be null if the `format` is not `currency`.. [optional]  # noqa: E501
-            custom_label (str, none_type): This is the string that appears next to the custom field value. This will be null if the `format` is not `custom`.. [optional]  # noqa: E501
-            custom_label_position (str): Only relevant for custom fields with `custom` format. This depicts where to place the custom label. This will be null if the `format` is not `custom`.. [optional]  # noqa: E501
-            has_notifications_enabled (bool): *Conditional*. This flag describes whether a follower of a task with this field should receive inbox notifications from changes to this field.. [optional]  # noqa: E501
+            gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
+            created_at (datetime): The time at which this resource was created.. [optional]  # noqa: E501
+            resource_subtype (str): The subtype of this resource. Different subtypes retain many of the same fields and behavior, but may render differently in Asana or represent resources with different semantic meaning.. [optional]  # noqa: E501
+            text (str): The plain text of the comment to add. Cannot be used with html_text.. [optional]  # noqa: E501
+            html_text (str): [Opt In](/docs/inputoutput-options). HTML formatted text for a comment. This will not include the name of the creator.. [optional]  # noqa: E501
+            is_pinned (bool): *Conditional*. Whether the story should be pinned on the resource.. [optional]  # noqa: E501
+            sticker_name (str): The name of the sticker in this story. `null` if there is no sticker.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         self = super(OpenApiModel, cls).__new__(cls)
 
         if args:
@@ -191,36 +207,54 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        constant_args = {
+            '_check_type': _check_type,
+            '_path_to_item': _path_to_item,
+            '_spec_property_naming': _spec_property_naming,
+            '_configuration': _configuration,
+            '_visited_composed_classes': self._visited_composed_classes,
+        }
+        composed_info = validate_get_composed_info(
+            constant_args, kwargs, self)
+        self._composed_instances = composed_info[0]
+        self._var_name_to_model_instances = composed_info[1]
+        self._additional_properties_model_instances = composed_info[2]
+        discarded_args = composed_info[3]
+
         for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
+            if var_name in discarded_args and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
+                        self._additional_properties_model_instances:
                 # discard variable.
                 continue
             setattr(self, var_name, var_value)
+
         return self
 
     required_properties = set([
         '_data_store',
         '_check_type',
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
+        '_composed_instances',
+        '_var_name_to_model_instances',
+        '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """CustomFieldBaseAllOf - a model defined in OpenAPI
+        """StoryBase - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -245,21 +279,22 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            description (str): [Opt In](/docs/inputoutput-options). The description of the custom field.. [optional]  # noqa: E501
-            precision (int): Only relevant for custom fields of type ‘Number’. This field dictates the number of places after the decimal to round to, i.e. 0 is integer values, 1 rounds to the nearest tenth, and so on. Must be between 0 and 6, inclusive. For percentage format, this may be unintuitive, as a value of 0.25 has a precision of 0, while a value of 0.251 has a precision of 1. This is due to 0.25 being displayed as 25%. The identifier format will always have a precision of 0.. [optional]  # noqa: E501
-            format (str): The format of this custom field.. [optional]  # noqa: E501
-            currency_code (str, none_type): ISO 4217 currency code to format this custom field. This will be null if the `format` is not `currency`.. [optional]  # noqa: E501
-            custom_label (str, none_type): This is the string that appears next to the custom field value. This will be null if the `format` is not `custom`.. [optional]  # noqa: E501
-            custom_label_position (str): Only relevant for custom fields with `custom` format. This depicts where to place the custom label. This will be null if the `format` is not `custom`.. [optional]  # noqa: E501
-            has_notifications_enabled (bool): *Conditional*. This flag describes whether a follower of a task with this field should receive inbox notifications from changes to this field.. [optional]  # noqa: E501
+            gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
+            created_at (datetime): The time at which this resource was created.. [optional]  # noqa: E501
+            resource_subtype (str): The subtype of this resource. Different subtypes retain many of the same fields and behavior, but may render differently in Asana or represent resources with different semantic meaning.. [optional]  # noqa: E501
+            text (str): The plain text of the comment to add. Cannot be used with html_text.. [optional]  # noqa: E501
+            html_text (str): [Opt In](/docs/inputoutput-options). HTML formatted text for a comment. This will not include the name of the creator.. [optional]  # noqa: E501
+            is_pinned (bool): *Conditional*. Whether the story should be pinned on the resource.. [optional]  # noqa: E501
+            sticker_name (str): The name of the sticker in this story. `null` if there is no sticker.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -281,18 +316,53 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        constant_args = {
+            '_check_type': _check_type,
+            '_path_to_item': _path_to_item,
+            '_spec_property_naming': _spec_property_naming,
+            '_configuration': _configuration,
+            '_visited_composed_classes': self._visited_composed_classes,
+        }
+        composed_info = validate_get_composed_info(
+            constant_args, kwargs, self)
+        self._composed_instances = composed_info[0]
+        self._var_name_to_model_instances = composed_info[1]
+        self._additional_properties_model_instances = composed_info[2]
+        discarded_args = composed_info[3]
+
         for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
+            if var_name in discarded_args and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
+                        self._additional_properties_model_instances:
                 # discard variable.
                 continue
             setattr(self, var_name, var_value)
             if var_name in self.read_only_vars:
                 raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
                                      f"class with read only attributes.")
+
+    @cached_property
+    def _composed_schemas():
+        # we need this here to make our import statements work
+        # we must store _composed_schemas in here so the code is only run
+        # when we invoke this method. If we kept this at the class
+        # level we would get an error because the class level
+        # code would be run when this module is imported, and these composed
+        # classes don't exist yet because their module has not finished
+        # loading
+        lazy_import()
+        return {
+          'anyOf': [
+          ],
+          'allOf': [
+              AsanaResource,
+              StoryBaseAllOf,
+          ],
+          'oneOf': [
+          ],
+        }
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `asana-preview-1.0.4/asana_preview/model/custom_field_compact.py` & `asana-preview-1.0.5/asana_preview/model/goal_request.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,25 +26,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from asana_preview.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from asana_preview.model.asana_resource import AsanaResource
-    from asana_preview.model.custom_field_compact_all_of import CustomFieldCompactAllOf
-    from asana_preview.model.custom_field_compact_all_of_date_value import CustomFieldCompactAllOfDateValue
-    from asana_preview.model.enum_option import EnumOption
-    globals()['AsanaResource'] = AsanaResource
-    globals()['CustomFieldCompactAllOf'] = CustomFieldCompactAllOf
-    globals()['CustomFieldCompactAllOfDateValue'] = CustomFieldCompactAllOfDateValue
-    globals()['EnumOption'] = EnumOption
+    from asana_preview.model.goal_base import GoalBase
+    from asana_preview.model.goal_request_all_of import GoalRequestAllOf
+    globals()['GoalBase'] = GoalBase
+    globals()['GoalRequestAllOf'] = GoalRequestAllOf
 
 
-class CustomFieldCompact(ModelComposed):
+class GoalRequest(ModelComposed):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -61,28 +57,14 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('resource_subtype',): {
-            'TEXT': "text",
-            'ENUM': "enum",
-            'MULTI_ENUM': "multi_enum",
-            'NUMBER': "number",
-            'DATE': "date",
-            'PEOPLE': "people",
-        },
-        ('type',): {
-            'TEXT': "text",
-            'ENUM': "enum",
-            'MULTI_ENUM': "multi_enum",
-            'NUMBER': "number",
-        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
@@ -104,59 +86,62 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'gid': (str,),  # noqa: E501
-            'resource_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'resource_type': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
-            'resource_subtype': (str,),  # noqa: E501
-            'type': (str,),  # noqa: E501
-            'enum_options': ([EnumOption],),  # noqa: E501
-            'enabled': (bool,),  # noqa: E501
-            'date_value': (CustomFieldCompactAllOfDateValue,),  # noqa: E501
-            'enum_value': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
-            'multi_enum_values': ([EnumOption],),  # noqa: E501
-            'number_value': (float,),  # noqa: E501
-            'text_value': (str,),  # noqa: E501
-            'display_value': (str, none_type,),  # noqa: E501
+            'html_notes': (str,),  # noqa: E501
+            'notes': (str,),  # noqa: E501
+            'due_on': (str, none_type,),  # noqa: E501
+            'start_on': (str, none_type,),  # noqa: E501
+            'status': (str, none_type,),  # noqa: E501
+            'is_workspace_level': (bool,),  # noqa: E501
+            'liked': (bool,),  # noqa: E501
+            'team': (str, none_type,),  # noqa: E501
+            'workspace': (str,),  # noqa: E501
+            'followers': ([str],),  # noqa: E501
+            'time_period': (str, none_type,),  # noqa: E501
+            'owner': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'gid': 'gid',  # noqa: E501
         'resource_type': 'resource_type',  # noqa: E501
         'name': 'name',  # noqa: E501
-        'resource_subtype': 'resource_subtype',  # noqa: E501
-        'type': 'type',  # noqa: E501
-        'enum_options': 'enum_options',  # noqa: E501
-        'enabled': 'enabled',  # noqa: E501
-        'date_value': 'date_value',  # noqa: E501
-        'enum_value': 'enum_value',  # noqa: E501
-        'multi_enum_values': 'multi_enum_values',  # noqa: E501
-        'number_value': 'number_value',  # noqa: E501
-        'text_value': 'text_value',  # noqa: E501
-        'display_value': 'display_value',  # noqa: E501
+        'html_notes': 'html_notes',  # noqa: E501
+        'notes': 'notes',  # noqa: E501
+        'due_on': 'due_on',  # noqa: E501
+        'start_on': 'start_on',  # noqa: E501
+        'status': 'status',  # noqa: E501
+        'is_workspace_level': 'is_workspace_level',  # noqa: E501
+        'liked': 'liked',  # noqa: E501
+        'team': 'team',  # noqa: E501
+        'workspace': 'workspace',  # noqa: E501
+        'followers': 'followers',  # noqa: E501
+        'time_period': 'time_period',  # noqa: E501
+        'owner': 'owner',  # noqa: E501
     }
 
     read_only_vars = {
         'gid',  # noqa: E501
-        'type',  # noqa: E501
-        'display_value',  # noqa: E501
+        'resource_type',  # noqa: E501
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """CustomFieldCompact - a model defined in OpenAPI
+        """GoalRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -182,26 +167,28 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            name (str): The name of the custom field.. [optional]  # noqa: E501
-            resource_subtype (str): The type of the custom field. Must be one of the given values.. [optional]  # noqa: E501
-            type (str): *Deprecated: new integrations should prefer the resource_subtype field.* The type of the custom field. Must be one of the given values.. [optional]  # noqa: E501
-            enum_options ([EnumOption]): *Conditional*. Only relevant for custom fields of type `enum`. This array specifies the possible values which an `enum` custom field can adopt. To modify the enum options, refer to [working with enum options](/reference/createenumoptionforcustomfield).. [optional]  # noqa: E501
-            enabled (bool): *Conditional*. Determines if the custom field is enabled or not.. [optional]  # noqa: E501
-            date_value (CustomFieldCompactAllOfDateValue): [optional]  # noqa: E501
-            enum_value (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            multi_enum_values ([EnumOption]): *Conditional*. Only relevant for custom fields of type `multi_enum`. This object is the chosen values of a `multi_enum` custom field.. [optional]  # noqa: E501
-            number_value (float): *Conditional*. This number is the value of a `number` custom field.. [optional]  # noqa: E501
-            text_value (str): *Conditional*. This string is the value of a `text` custom field.. [optional]  # noqa: E501
-            display_value (str, none_type): A string representation for the value of the custom field. Integrations that don't require the underlying type should use this field to read values. Using this field will future-proof an app against new custom field types.. [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
+            name (str): The name of the goal.. [optional]  # noqa: E501
+            html_notes (str): The notes of the goal with formatting as HTML.. [optional]  # noqa: E501
+            notes (str): Free-form textual information associated with the goal (i.e. its description).. [optional]  # noqa: E501
+            due_on (str, none_type): The localized day on which this goal is due. This takes a date with format `YYYY-MM-DD`.. [optional]  # noqa: E501
+            start_on (str, none_type): The day on which work for this goal begins, or null if the goal has no start date. This takes a date with `YYYY-MM-DD` format, and cannot be set unless there is an accompanying due date.. [optional]  # noqa: E501
+            status (str, none_type): The current status of this goal. When the goal is open, its status can be `green`, `yellow`, and `red` to reflect \"On Track\", \"At Risk\", and \"Off Track\", respectively. When the goal is closed, the value can be `missed`, `achieved`, `partial`, or `dropped`. *Note* you can only write to this property if `metric` is set.. [optional]  # noqa: E501
+            is_workspace_level (bool): *Conditional*. This property is only present when the `workspace` provided is an organization. Whether the goal belongs to the `workspace` (and is listed as part of the workspace’s goals) or not. If it isn’t a workspace-level goal, it is a team-level goal, and is associated with the goal’s team.. [optional]  # noqa: E501
+            liked (bool): True if the goal is liked by the authorized user, false if not.. [optional]  # noqa: E501
+            team (str, none_type): *Conditional*. This property is only present when the `workspace` provided is an organization.. [optional]  # noqa: E501
+            workspace (str): The `gid` of a workspace.. [optional]  # noqa: E501
+            followers ([str]): [optional]  # noqa: E501
+            time_period (str, none_type): The `gid` of a time period.. [optional]  # noqa: E501
+            owner (str, none_type): The `gid` of a user.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -264,15 +251,15 @@
         '_composed_instances',
         '_var_name_to_model_instances',
         '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """CustomFieldCompact - a model defined in OpenAPI
+        """GoalRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -298,26 +285,28 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            name (str): The name of the custom field.. [optional]  # noqa: E501
-            resource_subtype (str): The type of the custom field. Must be one of the given values.. [optional]  # noqa: E501
-            type (str): *Deprecated: new integrations should prefer the resource_subtype field.* The type of the custom field. Must be one of the given values.. [optional]  # noqa: E501
-            enum_options ([EnumOption]): *Conditional*. Only relevant for custom fields of type `enum`. This array specifies the possible values which an `enum` custom field can adopt. To modify the enum options, refer to [working with enum options](/reference/createenumoptionforcustomfield).. [optional]  # noqa: E501
-            enabled (bool): *Conditional*. Determines if the custom field is enabled or not.. [optional]  # noqa: E501
-            date_value (CustomFieldCompactAllOfDateValue): [optional]  # noqa: E501
-            enum_value (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            multi_enum_values ([EnumOption]): *Conditional*. Only relevant for custom fields of type `multi_enum`. This object is the chosen values of a `multi_enum` custom field.. [optional]  # noqa: E501
-            number_value (float): *Conditional*. This number is the value of a `number` custom field.. [optional]  # noqa: E501
-            text_value (str): *Conditional*. This string is the value of a `text` custom field.. [optional]  # noqa: E501
-            display_value (str, none_type): A string representation for the value of the custom field. Integrations that don't require the underlying type should use this field to read values. Using this field will future-proof an app against new custom field types.. [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
+            name (str): The name of the goal.. [optional]  # noqa: E501
+            html_notes (str): The notes of the goal with formatting as HTML.. [optional]  # noqa: E501
+            notes (str): Free-form textual information associated with the goal (i.e. its description).. [optional]  # noqa: E501
+            due_on (str, none_type): The localized day on which this goal is due. This takes a date with format `YYYY-MM-DD`.. [optional]  # noqa: E501
+            start_on (str, none_type): The day on which work for this goal begins, or null if the goal has no start date. This takes a date with `YYYY-MM-DD` format, and cannot be set unless there is an accompanying due date.. [optional]  # noqa: E501
+            status (str, none_type): The current status of this goal. When the goal is open, its status can be `green`, `yellow`, and `red` to reflect \"On Track\", \"At Risk\", and \"Off Track\", respectively. When the goal is closed, the value can be `missed`, `achieved`, `partial`, or `dropped`. *Note* you can only write to this property if `metric` is set.. [optional]  # noqa: E501
+            is_workspace_level (bool): *Conditional*. This property is only present when the `workspace` provided is an organization. Whether the goal belongs to the `workspace` (and is listed as part of the workspace’s goals) or not. If it isn’t a workspace-level goal, it is a team-level goal, and is associated with the goal’s team.. [optional]  # noqa: E501
+            liked (bool): True if the goal is liked by the authorized user, false if not.. [optional]  # noqa: E501
+            team (str, none_type): *Conditional*. This property is only present when the `workspace` provided is an organization.. [optional]  # noqa: E501
+            workspace (str): The `gid` of a workspace.. [optional]  # noqa: E501
+            followers ([str]): [optional]  # noqa: E501
+            time_period (str, none_type): The `gid` of a time period.. [optional]  # noqa: E501
+            owner (str, none_type): The `gid` of a user.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -379,13 +368,13 @@
         # classes don't exist yet because their module has not finished
         # loading
         lazy_import()
         return {
           'anyOf': [
           ],
           'allOf': [
-              AsanaResource,
-              CustomFieldCompactAllOf,
+              GoalBase,
+              GoalRequestAllOf,
           ],
           'oneOf': [
           ],
         }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `asana-preview-1.0.4/asana_preview/model/custom_field_compact_all_of.py` & `asana-preview-1.0.5/asana_preview/model/custom_field_compact_all_of.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -99,40 +99,40 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'resource_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'resource_subtype': (str,),  # noqa: E501
             'type': (str,),  # noqa: E501
             'enum_options': ([EnumOption],),  # noqa: E501
             'enabled': (bool,),  # noqa: E501
+            'is_formula_field': (bool,),  # noqa: E501
             'date_value': (CustomFieldCompactAllOfDateValue,),  # noqa: E501
             'enum_value': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'multi_enum_values': ([EnumOption],),  # noqa: E501
-            'number_value': (float,),  # noqa: E501
-            'text_value': (str,),  # noqa: E501
+            'number_value': (float, none_type,),  # noqa: E501
+            'text_value': (str, none_type,),  # noqa: E501
             'display_value': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'resource_type': 'resource_type',  # noqa: E501
         'name': 'name',  # noqa: E501
         'resource_subtype': 'resource_subtype',  # noqa: E501
         'type': 'type',  # noqa: E501
         'enum_options': 'enum_options',  # noqa: E501
         'enabled': 'enabled',  # noqa: E501
+        'is_formula_field': 'is_formula_field',  # noqa: E501
         'date_value': 'date_value',  # noqa: E501
         'enum_value': 'enum_value',  # noqa: E501
         'multi_enum_values': 'multi_enum_values',  # noqa: E501
         'number_value': 'number_value',  # noqa: E501
         'text_value': 'text_value',  # noqa: E501
         'display_value': 'display_value',  # noqa: E501
     }
@@ -176,25 +176,25 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             name (str): The name of the custom field.. [optional]  # noqa: E501
-            resource_subtype (str): The type of the custom field. Must be one of the given values.. [optional]  # noqa: E501
-            type (str): *Deprecated: new integrations should prefer the resource_subtype field.* The type of the custom field. Must be one of the given values.. [optional]  # noqa: E501
+            resource_subtype (str): The type of the custom field. Must be one of the given values. . [optional]  # noqa: E501
+            type (str): *Deprecated: new integrations should prefer the resource_subtype field.* The type of the custom field. Must be one of the given values. . [optional]  # noqa: E501
             enum_options ([EnumOption]): *Conditional*. Only relevant for custom fields of type `enum`. This array specifies the possible values which an `enum` custom field can adopt. To modify the enum options, refer to [working with enum options](/reference/createenumoptionforcustomfield).. [optional]  # noqa: E501
             enabled (bool): *Conditional*. Determines if the custom field is enabled or not.. [optional]  # noqa: E501
+            is_formula_field (bool): *Conditional*. This flag describes whether a custom field is a formula custom field.. [optional]  # noqa: E501
             date_value (CustomFieldCompactAllOfDateValue): [optional]  # noqa: E501
             enum_value (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             multi_enum_values ([EnumOption]): *Conditional*. Only relevant for custom fields of type `multi_enum`. This object is the chosen values of a `multi_enum` custom field.. [optional]  # noqa: E501
-            number_value (float): *Conditional*. This number is the value of a `number` custom field.. [optional]  # noqa: E501
-            text_value (str): *Conditional*. This string is the value of a `text` custom field.. [optional]  # noqa: E501
+            number_value (float, none_type): *Conditional*. This number is the value of a `number` custom field.. [optional]  # noqa: E501
+            text_value (str, none_type): *Conditional*. This string is the value of a `text` custom field.. [optional]  # noqa: E501
             display_value (str, none_type): A string representation for the value of the custom field. Integrations that don't require the underlying type should use this field to read values. Using this field will future-proof an app against new custom field types.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -273,25 +273,25 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             name (str): The name of the custom field.. [optional]  # noqa: E501
-            resource_subtype (str): The type of the custom field. Must be one of the given values.. [optional]  # noqa: E501
-            type (str): *Deprecated: new integrations should prefer the resource_subtype field.* The type of the custom field. Must be one of the given values.. [optional]  # noqa: E501
+            resource_subtype (str): The type of the custom field. Must be one of the given values. . [optional]  # noqa: E501
+            type (str): *Deprecated: new integrations should prefer the resource_subtype field.* The type of the custom field. Must be one of the given values. . [optional]  # noqa: E501
             enum_options ([EnumOption]): *Conditional*. Only relevant for custom fields of type `enum`. This array specifies the possible values which an `enum` custom field can adopt. To modify the enum options, refer to [working with enum options](/reference/createenumoptionforcustomfield).. [optional]  # noqa: E501
             enabled (bool): *Conditional*. Determines if the custom field is enabled or not.. [optional]  # noqa: E501
+            is_formula_field (bool): *Conditional*. This flag describes whether a custom field is a formula custom field.. [optional]  # noqa: E501
             date_value (CustomFieldCompactAllOfDateValue): [optional]  # noqa: E501
             enum_value (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             multi_enum_values ([EnumOption]): *Conditional*. Only relevant for custom fields of type `multi_enum`. This object is the chosen values of a `multi_enum` custom field.. [optional]  # noqa: E501
-            number_value (float): *Conditional*. This number is the value of a `number` custom field.. [optional]  # noqa: E501
-            text_value (str): *Conditional*. This string is the value of a `text` custom field.. [optional]  # noqa: E501
+            number_value (float, none_type): *Conditional*. This number is the value of a `number` custom field.. [optional]  # noqa: E501
+            text_value (str, none_type): *Conditional*. This string is the value of a `text` custom field.. [optional]  # noqa: E501
             display_value (str, none_type): A string representation for the value of the custom field. Integrations that don't require the underlying type should use this field to read values. Using this field will future-proof an app against new custom field types.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `asana-preview-1.0.4/asana_preview/model/custom_field_compact_all_of_date_value.py` & `asana-preview-1.0.5/asana_preview/model/goal_metric_current_value_request_all_of.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from asana_preview.exceptions import ApiAttributeError
 
 
 
-class CustomFieldCompactAllOfDateValue(ModelNormal):
+class GoalMetricCurrentValueRequestAllOf(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -77,37 +77,35 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'date': (str,),  # noqa: E501
-            'date_time': (str,),  # noqa: E501
+            'current_number_value': (float,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'date': 'date',  # noqa: E501
-        'date_time': 'date_time',  # noqa: E501
+        'current_number_value': 'current_number_value',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """CustomFieldCompactAllOfDateValue - a model defined in OpenAPI
+        """GoalMetricCurrentValueRequestAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -132,16 +130,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            date (str): A string representing the date in YYYY-MM-DD format.. [optional]  # noqa: E501
-            date_time (str): A string representing the date in ISO 8601 format. If no time value is selected, the value of `date-time` will be `null`.. [optional]  # noqa: E501
+            current_number_value (float): *Conditional*. This number is the current value of a goal metric of type number.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -186,15 +183,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """CustomFieldCompactAllOfDateValue - a model defined in OpenAPI
+        """GoalMetricCurrentValueRequestAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -219,16 +216,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            date (str): A string representing the date in YYYY-MM-DD format.. [optional]  # noqa: E501
-            date_time (str): A string representing the date in ISO 8601 format. If no time value is selected, the value of `date-time` will be `null`.. [optional]  # noqa: E501
+            current_number_value (float): *Conditional*. This number is the current value of a goal metric of type number.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `asana-preview-1.0.4/asana_preview/model/custom_field_response.py` & `asana-preview-1.0.5/asana_preview/model/custom_field_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -256,37 +256,39 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'gid': (str,),  # noqa: E501
-            'resource_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'resource_type': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'resource_subtype': (str,),  # noqa: E501
             'type': (str,),  # noqa: E501
             'enum_options': ([EnumOption],),  # noqa: E501
             'enabled': (bool,),  # noqa: E501
+            'is_formula_field': (bool,),  # noqa: E501
             'date_value': (CustomFieldCompactAllOfDateValue,),  # noqa: E501
             'enum_value': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'multi_enum_values': ([EnumOption],),  # noqa: E501
-            'number_value': (float,),  # noqa: E501
-            'text_value': (str,),  # noqa: E501
+            'number_value': (float, none_type,),  # noqa: E501
+            'text_value': (str, none_type,),  # noqa: E501
             'display_value': (str, none_type,),  # noqa: E501
             'description': (str,),  # noqa: E501
             'precision': (int,),  # noqa: E501
             'format': (str,),  # noqa: E501
             'currency_code': (str, none_type,),  # noqa: E501
             'custom_label': (str, none_type,),  # noqa: E501
             'custom_label_position': (str,),  # noqa: E501
+            'is_global_to_workspace': (bool,),  # noqa: E501
             'has_notifications_enabled': (bool,),  # noqa: E501
+            'asana_created_field': (str, none_type,),  # noqa: E501
+            'is_value_read_only': (bool,),  # noqa: E501
             'created_by': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'people_value': ([UserCompact],),  # noqa: E501
-            'is_global_to_workspace': (bool,),  # noqa: E501
-            'asana_created_field': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -294,39 +296,40 @@
         'gid': 'gid',  # noqa: E501
         'resource_type': 'resource_type',  # noqa: E501
         'name': 'name',  # noqa: E501
         'resource_subtype': 'resource_subtype',  # noqa: E501
         'type': 'type',  # noqa: E501
         'enum_options': 'enum_options',  # noqa: E501
         'enabled': 'enabled',  # noqa: E501
+        'is_formula_field': 'is_formula_field',  # noqa: E501
         'date_value': 'date_value',  # noqa: E501
         'enum_value': 'enum_value',  # noqa: E501
         'multi_enum_values': 'multi_enum_values',  # noqa: E501
         'number_value': 'number_value',  # noqa: E501
         'text_value': 'text_value',  # noqa: E501
         'display_value': 'display_value',  # noqa: E501
         'description': 'description',  # noqa: E501
         'precision': 'precision',  # noqa: E501
         'format': 'format',  # noqa: E501
         'currency_code': 'currency_code',  # noqa: E501
         'custom_label': 'custom_label',  # noqa: E501
         'custom_label_position': 'custom_label_position',  # noqa: E501
+        'is_global_to_workspace': 'is_global_to_workspace',  # noqa: E501
         'has_notifications_enabled': 'has_notifications_enabled',  # noqa: E501
+        'asana_created_field': 'asana_created_field',  # noqa: E501
+        'is_value_read_only': 'is_value_read_only',  # noqa: E501
         'created_by': 'created_by',  # noqa: E501
         'people_value': 'people_value',  # noqa: E501
-        'is_global_to_workspace': 'is_global_to_workspace',  # noqa: E501
-        'asana_created_field': 'asana_created_field',  # noqa: E501
     }
 
     read_only_vars = {
         'gid',  # noqa: E501
+        'resource_type',  # noqa: E501
         'type',  # noqa: E501
         'display_value',  # noqa: E501
-        'created_by',  # noqa: E501
-        'people_value',  # noqa: E501
         'is_global_to_workspace',  # noqa: E501
         'asana_created_field',  # noqa: E501
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
@@ -360,37 +363,39 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
             name (str): The name of the custom field.. [optional]  # noqa: E501
-            resource_subtype (str): The type of the custom field. Must be one of the given values.. [optional]  # noqa: E501
-            type (str): *Deprecated: new integrations should prefer the resource_subtype field.* The type of the custom field. Must be one of the given values.. [optional]  # noqa: E501
+            resource_subtype (str): The type of the custom field. Must be one of the given values. . [optional]  # noqa: E501
+            type (str): *Deprecated: new integrations should prefer the resource_subtype field.* The type of the custom field. Must be one of the given values. . [optional]  # noqa: E501
             enum_options ([EnumOption]): *Conditional*. Only relevant for custom fields of type `enum`. This array specifies the possible values which an `enum` custom field can adopt. To modify the enum options, refer to [working with enum options](/reference/createenumoptionforcustomfield).. [optional]  # noqa: E501
             enabled (bool): *Conditional*. Determines if the custom field is enabled or not.. [optional]  # noqa: E501
+            is_formula_field (bool): *Conditional*. This flag describes whether a custom field is a formula custom field.. [optional]  # noqa: E501
             date_value (CustomFieldCompactAllOfDateValue): [optional]  # noqa: E501
             enum_value (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             multi_enum_values ([EnumOption]): *Conditional*. Only relevant for custom fields of type `multi_enum`. This object is the chosen values of a `multi_enum` custom field.. [optional]  # noqa: E501
-            number_value (float): *Conditional*. This number is the value of a `number` custom field.. [optional]  # noqa: E501
-            text_value (str): *Conditional*. This string is the value of a `text` custom field.. [optional]  # noqa: E501
+            number_value (float, none_type): *Conditional*. This number is the value of a `number` custom field.. [optional]  # noqa: E501
+            text_value (str, none_type): *Conditional*. This string is the value of a `text` custom field.. [optional]  # noqa: E501
             display_value (str, none_type): A string representation for the value of the custom field. Integrations that don't require the underlying type should use this field to read values. Using this field will future-proof an app against new custom field types.. [optional]  # noqa: E501
             description (str): [Opt In](/docs/inputoutput-options). The description of the custom field.. [optional]  # noqa: E501
             precision (int): Only relevant for custom fields of type ‘Number’. This field dictates the number of places after the decimal to round to, i.e. 0 is integer values, 1 rounds to the nearest tenth, and so on. Must be between 0 and 6, inclusive. For percentage format, this may be unintuitive, as a value of 0.25 has a precision of 0, while a value of 0.251 has a precision of 1. This is due to 0.25 being displayed as 25%. The identifier format will always have a precision of 0.. [optional]  # noqa: E501
             format (str): The format of this custom field.. [optional]  # noqa: E501
             currency_code (str, none_type): ISO 4217 currency code to format this custom field. This will be null if the `format` is not `currency`.. [optional]  # noqa: E501
             custom_label (str, none_type): This is the string that appears next to the custom field value. This will be null if the `format` is not `custom`.. [optional]  # noqa: E501
             custom_label_position (str): Only relevant for custom fields with `custom` format. This depicts where to place the custom label. This will be null if the `format` is not `custom`.. [optional]  # noqa: E501
+            is_global_to_workspace (bool): This flag describes whether this custom field is available to every container in the workspace. Before project-specific custom fields, this field was always true.. [optional]  # noqa: E501
             has_notifications_enabled (bool): *Conditional*. This flag describes whether a follower of a task with this field should receive inbox notifications from changes to this field.. [optional]  # noqa: E501
+            asana_created_field (str, none_type): *Conditional*. A unique identifier to associate this field with the template source of truth.. [optional]  # noqa: E501
+            is_value_read_only (bool): *Conditional*. This flag describes whether a custom field is read only.. [optional]  # noqa: E501
             created_by (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             people_value ([UserCompact]): *Conditional*. Only relevant for custom fields of type `people`. This array of [compact user](/reference/users) objects reflects the values of a `people` custom field.. [optional]  # noqa: E501
-            is_global_to_workspace (bool): This flag describes whether this custom field is available to every container in the workspace. Before project-specific custom fields, this field was always true.. [optional]  # noqa: E501
-            asana_created_field (str, none_type): *Conditional*. A unique identifier to associate this field with the template source of truth.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -487,37 +492,39 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
             name (str): The name of the custom field.. [optional]  # noqa: E501
-            resource_subtype (str): The type of the custom field. Must be one of the given values.. [optional]  # noqa: E501
-            type (str): *Deprecated: new integrations should prefer the resource_subtype field.* The type of the custom field. Must be one of the given values.. [optional]  # noqa: E501
+            resource_subtype (str): The type of the custom field. Must be one of the given values. . [optional]  # noqa: E501
+            type (str): *Deprecated: new integrations should prefer the resource_subtype field.* The type of the custom field. Must be one of the given values. . [optional]  # noqa: E501
             enum_options ([EnumOption]): *Conditional*. Only relevant for custom fields of type `enum`. This array specifies the possible values which an `enum` custom field can adopt. To modify the enum options, refer to [working with enum options](/reference/createenumoptionforcustomfield).. [optional]  # noqa: E501
             enabled (bool): *Conditional*. Determines if the custom field is enabled or not.. [optional]  # noqa: E501
+            is_formula_field (bool): *Conditional*. This flag describes whether a custom field is a formula custom field.. [optional]  # noqa: E501
             date_value (CustomFieldCompactAllOfDateValue): [optional]  # noqa: E501
             enum_value (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             multi_enum_values ([EnumOption]): *Conditional*. Only relevant for custom fields of type `multi_enum`. This object is the chosen values of a `multi_enum` custom field.. [optional]  # noqa: E501
-            number_value (float): *Conditional*. This number is the value of a `number` custom field.. [optional]  # noqa: E501
-            text_value (str): *Conditional*. This string is the value of a `text` custom field.. [optional]  # noqa: E501
+            number_value (float, none_type): *Conditional*. This number is the value of a `number` custom field.. [optional]  # noqa: E501
+            text_value (str, none_type): *Conditional*. This string is the value of a `text` custom field.. [optional]  # noqa: E501
             display_value (str, none_type): A string representation for the value of the custom field. Integrations that don't require the underlying type should use this field to read values. Using this field will future-proof an app against new custom field types.. [optional]  # noqa: E501
             description (str): [Opt In](/docs/inputoutput-options). The description of the custom field.. [optional]  # noqa: E501
             precision (int): Only relevant for custom fields of type ‘Number’. This field dictates the number of places after the decimal to round to, i.e. 0 is integer values, 1 rounds to the nearest tenth, and so on. Must be between 0 and 6, inclusive. For percentage format, this may be unintuitive, as a value of 0.25 has a precision of 0, while a value of 0.251 has a precision of 1. This is due to 0.25 being displayed as 25%. The identifier format will always have a precision of 0.. [optional]  # noqa: E501
             format (str): The format of this custom field.. [optional]  # noqa: E501
             currency_code (str, none_type): ISO 4217 currency code to format this custom field. This will be null if the `format` is not `currency`.. [optional]  # noqa: E501
             custom_label (str, none_type): This is the string that appears next to the custom field value. This will be null if the `format` is not `custom`.. [optional]  # noqa: E501
             custom_label_position (str): Only relevant for custom fields with `custom` format. This depicts where to place the custom label. This will be null if the `format` is not `custom`.. [optional]  # noqa: E501
+            is_global_to_workspace (bool): This flag describes whether this custom field is available to every container in the workspace. Before project-specific custom fields, this field was always true.. [optional]  # noqa: E501
             has_notifications_enabled (bool): *Conditional*. This flag describes whether a follower of a task with this field should receive inbox notifications from changes to this field.. [optional]  # noqa: E501
+            asana_created_field (str, none_type): *Conditional*. A unique identifier to associate this field with the template source of truth.. [optional]  # noqa: E501
+            is_value_read_only (bool): *Conditional*. This flag describes whether a custom field is read only.. [optional]  # noqa: E501
             created_by (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             people_value ([UserCompact]): *Conditional*. Only relevant for custom fields of type `people`. This array of [compact user](/reference/users) objects reflects the values of a `people` custom field.. [optional]  # noqa: E501
-            is_global_to_workspace (bool): This flag describes whether this custom field is available to every container in the workspace. Before project-specific custom fields, this field was always true.. [optional]  # noqa: E501
-            asana_created_field (str, none_type): *Conditional*. A unique identifier to associate this field with the template source of truth.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `asana-preview-1.0.4/asana_preview/model/custom_field_response_all_of.py` & `asana-preview-1.0.5/asana_preview/model/project_base_all_of.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,19 +26,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from asana_preview.exceptions import ApiAttributeError
 
 
 def lazy_import():
+    from asana_preview.model.custom_field_setting_response import CustomFieldSettingResponse
     from asana_preview.model.user_compact import UserCompact
+    globals()['CustomFieldSettingResponse'] = CustomFieldSettingResponse
     globals()['UserCompact'] = UserCompact
 
 
-class CustomFieldResponseAllOf(ModelNormal):
+class ProjectBaseAllOf(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -55,152 +57,40 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('asana_created_field',): {
+        ('color',): {
             'None': None,
-            'A_V_REQUIREMENTS': "a_v_requirements",
-            'ACCOUNT_NAME': "account_name",
-            'ACTIONABLE': "actionable",
-            'ALIGN_SHIPPING_LINK': "align_shipping_link",
-            'ALIGN_STATUS': "align_status",
-            'ALLOTTED_TIME': "allotted_time",
-            'APPOINTMENT': "appointment",
-            'APPROVAL_STAGE': "approval_stage",
-            'APPROVED': "approved",
-            'ARTICLE_SERIES': "article_series",
-            'BOARD_COMMITTEE': "board_committee",
-            'BROWSER': "browser",
-            'CAMPAIGN_AUDIENCE': "campaign_audience",
-            'CAMPAIGN_PROJECT_STATUS': "campaign_project_status",
-            'CAMPAIGN_REGIONS': "campaign_regions",
-            'CHANNEL_PRIMARY': "channel_primary",
-            'CLIENT_TOPIC_TYPE': "client_topic_type",
-            'COMPLETE_BY': "complete_by",
-            'CONTACT': "contact",
-            'CONTACT_EMAIL_ADDRESS': "contact_email_address",
-            'CONTENT_CHANNELS': "content_channels",
-            'CONTENT_CHANNELS_NEEDED': "content_channels_needed",
-            'CONTENT_STAGE': "content_stage",
-            'CONTENT_TYPE': "content_type",
-            'CONTRACT': "contract",
-            'CONTRACT_STATUS': "contract_status",
-            'COST': "cost",
-            'CREATION_STAGE': "creation_stage",
-            'CREATIVE_CHANNEL': "creative_channel",
-            'CREATIVE_NEEDED': "creative_needed",
-            'CREATIVE_NEEDS': "creative_needs",
-            'DATA_SENSITIVITY': "data_sensitivity",
-            'DEAL_SIZE': "deal_size",
-            'DELIVERY_APPT': "delivery_appt",
-            'DELIVERY_APPT_DATE': "delivery_appt_date",
-            'DEPARTMENT': "department",
-            'DEPARTMENT_RESPONSIBLE': "department_responsible",
-            'DESIGN_REQUEST_NEEDED': "design_request_needed",
-            'DESIGN_REQUEST_TYPE': "design_request_type",
-            'DISCUSSION_CATEGORY': "discussion_category",
-            'DO_THIS_TASK': "do_this_task",
-            'EDITORIAL_CONTENT_STATUS': "editorial_content_status",
-            'EDITORIAL_CONTENT_TAG': "editorial_content_tag",
-            'EDITORIAL_CONTENT_TYPE': "editorial_content_type",
-            'EFFORT': "effort",
-            'EFFORT_LEVEL': "effort_level",
-            'EST_COMPLETION_DATE': "est_completion_date",
-            'ESTIMATED_TIME': "estimated_time",
-            'ESTIMATED_VALUE': "estimated_value",
-            'EXPECTED_COST': "expected_cost",
-            'EXTERNAL_STEPS_NEEDED': "external_steps_needed",
-            'FAVORITE_IDEA': "favorite_idea",
-            'FEEDBACK_TYPE': "feedback_type",
-            'FINANCIAL': "financial",
-            'FUNDING_AMOUNT': "funding_amount",
-            'GRANT_APPLICATION_PROCESS': "grant_application_process",
-            'HIRING_CANDIDATE_STATUS': "hiring_candidate_status",
-            'IDEA_STATUS': "idea_status",
-            'IDS_LINK': "ids_link",
-            'IDS_PATIENT_LINK': "ids_patient_link",
-            'IMPLEMENTATION_STAGE': "implementation_stage",
-            'INSURANCE': "insurance",
-            'INTERVIEW_AREA': "interview_area",
-            'INTERVIEW_QUESTION_SCORE': "interview_question_score",
-            'ITERO_SCAN_LINK': "itero_scan_link",
-            'JOB_S_APPLIED_TO': "job_s_applied_to",
-            'LAB': "lab",
-            'LAUNCH_STATUS': "launch_status",
-            'LEAD_STATUS': "lead_status",
-            'LOCALIZATION_LANGUAGE': "localization_language",
-            'LOCALIZATION_MARKET_TEAM': "localization_market_team",
-            'LOCALIZATION_STATUS': "localization_status",
-            'MEETING_MINUTES': "meeting_minutes",
-            'MEETING_NEEDED': "meeting_needed",
-            'MINUTES': "minutes",
-            'MRR': "mrr",
-            'MUST_LOCALIZE': "must_localize",
-            'NAME_OF_FOUNDATION': "name_of_foundation",
-            'NEED_TO_FOLLOW_UP': "need_to_follow_up",
-            'NEXT_APPOINTMENT': "next_appointment",
-            'NEXT_STEPS_SALES': "next_steps_sales",
-            'NUM_PEOPLE': "num_people",
-            'NUMBER_OF_USER_REPORTS': "number_of_user_reports",
-            'OFFICE_LOCATION': "office_location",
-            'ONBOARDING_ACTIVITY': "onboarding_activity",
-            'OWNER': "owner",
-            'PARTICIPANTS_NEEDED': "participants_needed",
-            'PATIENT_DATE_OF_BIRTH': "patient_date_of_birth",
-            'PATIENT_EMAIL': "patient_email",
-            'PATIENT_PHONE': "patient_phone",
-            'PATIENT_STATUS': "patient_status",
-            'PHONE_NUMBER': "phone_number",
-            'PLANNING_CATEGORY': "planning_category",
-            'POINT_OF_CONTACT': "point_of_contact",
-            'POSITION': "position",
-            'POST_FORMAT': "post_format",
-            'PRESCRIPTION': "prescription",
-            'PRIORITY': "priority",
-            'PRIORITY_LEVEL': "priority_level",
-            'PRODUCT': "product",
-            'PRODUCT_STAGE': "product_stage",
-            'PROGRESS': "progress",
-            'PROJECT_SIZE': "project_size",
-            'PROJECT_STATUS': "project_status",
-            'PROPOSED_BUDGET': "proposed_budget",
-            'PUBLISH_STATUS': "publish_status",
-            'REASON_FOR_SCAN': "reason_for_scan",
-            'REFERRAL': "referral",
-            'REQUEST_TYPE': "request_type",
-            'RESEARCH_STATUS': "research_status",
-            'RESPONSIBLE_DEPARTMENT': "responsible_department",
-            'RESPONSIBLE_TEAM': "responsible_team",
-            'RISK_ASSESSMENT_STATUS': "risk_assessment_status",
-            'ROOM_NAME': "room_name",
-            'SALES_COUNTERPART': "sales_counterpart",
-            'SENTIMENT': "sentiment",
-            'SHIPPING_LINK': "shipping_link",
-            'SOCIAL_CHANNELS': "social_channels",
-            'STAGE': "stage",
-            'STATUS': "status",
-            'STATUS_DESIGN': "status_design",
-            'STATUS_OF_INITIATIVE': "status_of_initiative",
-            'SYSTEM_SETUP': "system_setup",
-            'TASK_PROGRESS': "task_progress",
-            'TEAM': "team",
-            'TEAM_MARKETING': "team_marketing",
-            'TEAM_RESPONSIBLE': "team_responsible",
-            'TIME_IT_TAKES_TO_COMPLETE_TASKS': "time_it_takes_to_complete_tasks",
-            'TIMEFRAME': "timeframe",
-            'TREATMENT_TYPE': "treatment_type",
-            'TYPE_WORK_REQUESTS_IT': "type_work_requests_it",
-            'USE_AGENCY': "use_agency",
-            'USER_NAME': "user_name",
-            'VENDOR_CATEGORY': "vendor_category",
-            'VENDOR_TYPE': "vendor_type",
-            'WORD_COUNT': "word_count",
+            'DARK-PINK': "dark-pink",
+            'DARK-GREEN': "dark-green",
+            'DARK-BLUE': "dark-blue",
+            'DARK-RED': "dark-red",
+            'DARK-TEAL': "dark-teal",
+            'DARK-BROWN': "dark-brown",
+            'DARK-ORANGE': "dark-orange",
+            'DARK-PURPLE': "dark-purple",
+            'DARK-WARM-GRAY': "dark-warm-gray",
+            'LIGHT-PINK': "light-pink",
+            'LIGHT-GREEN': "light-green",
+            'LIGHT-BLUE': "light-blue",
+            'LIGHT-RED': "light-red",
+            'LIGHT-TEAL': "light-teal",
+            'LIGHT-BROWN': "light-brown",
+            'LIGHT-ORANGE': "light-orange",
+            'LIGHT-PURPLE': "light-purple",
+            'LIGHT-WARM-GRAY': "light-warm-gray",
+        },
+        ('default_view',): {
+            'LIST': "list",
+            'BOARD': "board",
+            'CALENDAR': "calendar",
+            'TIMELINE': "timeline",
         },
     }
 
     validations = {
     }
 
     @cached_property
@@ -222,45 +112,69 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'created_by': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
-            'people_value': ([UserCompact],),  # noqa: E501
-            'is_global_to_workspace': (bool,),  # noqa: E501
-            'asana_created_field': (str, none_type,),  # noqa: E501
+            'archived': (bool,),  # noqa: E501
+            'color': (str, none_type,),  # noqa: E501
+            'created_at': (datetime,),  # noqa: E501
+            'current_status': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'current_status_update': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'custom_field_settings': ([CustomFieldSettingResponse],),  # noqa: E501
+            'default_view': (str,),  # noqa: E501
+            'due_date': (datetime, none_type,),  # noqa: E501
+            'due_on': (datetime, none_type,),  # noqa: E501
+            'html_notes': (str,),  # noqa: E501
+            'members': ([UserCompact],),  # noqa: E501
+            'modified_at': (datetime,),  # noqa: E501
+            'notes': (str,),  # noqa: E501
+            'public': (bool,),  # noqa: E501
+            'start_on': (date, none_type,),  # noqa: E501
+            'workspace': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'created_by': 'created_by',  # noqa: E501
-        'people_value': 'people_value',  # noqa: E501
-        'is_global_to_workspace': 'is_global_to_workspace',  # noqa: E501
-        'asana_created_field': 'asana_created_field',  # noqa: E501
+        'archived': 'archived',  # noqa: E501
+        'color': 'color',  # noqa: E501
+        'created_at': 'created_at',  # noqa: E501
+        'current_status': 'current_status',  # noqa: E501
+        'current_status_update': 'current_status_update',  # noqa: E501
+        'custom_field_settings': 'custom_field_settings',  # noqa: E501
+        'default_view': 'default_view',  # noqa: E501
+        'due_date': 'due_date',  # noqa: E501
+        'due_on': 'due_on',  # noqa: E501
+        'html_notes': 'html_notes',  # noqa: E501
+        'members': 'members',  # noqa: E501
+        'modified_at': 'modified_at',  # noqa: E501
+        'notes': 'notes',  # noqa: E501
+        'public': 'public',  # noqa: E501
+        'start_on': 'start_on',  # noqa: E501
+        'workspace': 'workspace',  # noqa: E501
     }
 
     read_only_vars = {
-        'created_by',  # noqa: E501
-        'people_value',  # noqa: E501
-        'is_global_to_workspace',  # noqa: E501
-        'asana_created_field',  # noqa: E501
+        'created_at',  # noqa: E501
+        'custom_field_settings',  # noqa: E501
+        'members',  # noqa: E501
+        'modified_at',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """CustomFieldResponseAllOf - a model defined in OpenAPI
+        """ProjectBaseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -285,18 +199,30 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            created_by (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            people_value ([UserCompact]): *Conditional*. Only relevant for custom fields of type `people`. This array of [compact user](/reference/users) objects reflects the values of a `people` custom field.. [optional]  # noqa: E501
-            is_global_to_workspace (bool): This flag describes whether this custom field is available to every container in the workspace. Before project-specific custom fields, this field was always true.. [optional]  # noqa: E501
-            asana_created_field (str, none_type): *Conditional*. A unique identifier to associate this field with the template source of truth.. [optional]  # noqa: E501
+            archived (bool): True if the project is archived, false if not. Archived projects do not show in the UI by default and may be treated differently for queries.. [optional]  # noqa: E501
+            color (str, none_type): Color of the project.. [optional]  # noqa: E501
+            created_at (datetime): The time at which this resource was created.. [optional]  # noqa: E501
+            current_status (bool, date, datetime, dict, float, int, list, str, none_type): *Deprecated: new integrations should prefer the `current_status_update` resource.*. [optional]  # noqa: E501
+            current_status_update (bool, date, datetime, dict, float, int, list, str, none_type): The latest `status_update` posted to this project.. [optional]  # noqa: E501
+            custom_field_settings ([CustomFieldSettingResponse]): Array of Custom Field Settings (in compact form).. [optional]  # noqa: E501
+            default_view (str): The default view (list, board, calendar, or timeline) of a project.. [optional]  # noqa: E501
+            due_date (datetime, none_type): *Deprecated: new integrations should prefer the `due_on` field.*. [optional]  # noqa: E501
+            due_on (datetime, none_type): The day on which this project is due. This takes a date with format YYYY-MM-DD.. [optional]  # noqa: E501
+            html_notes (str): [Opt In](/docs/inputoutput-options). The notes of the project with formatting as HTML.. [optional]  # noqa: E501
+            members ([UserCompact]): Array of users who are members of this project.. [optional]  # noqa: E501
+            modified_at (datetime): The time at which this project was last modified. *Note: This does not currently reflect any changes in associations such as tasks or comments that may have been added or removed from the project.*. [optional]  # noqa: E501
+            notes (str): Free-form textual information associated with the project (ie., its description).. [optional]  # noqa: E501
+            public (bool): True if the project is public to its team.. [optional]  # noqa: E501
+            start_on (date, none_type): The day on which work for this project begins, or null if the project has no start date. This takes a date with `YYYY-MM-DD` format. *Note: `due_on` or `due_at` must be present in the request when setting or unsetting the `start_on` parameter. Additionally, `start_on` and `due_on` cannot be the same date.*. [optional]  # noqa: E501
+            workspace (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -341,15 +267,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """CustomFieldResponseAllOf - a model defined in OpenAPI
+        """ProjectBaseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -374,18 +300,30 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            created_by (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            people_value ([UserCompact]): *Conditional*. Only relevant for custom fields of type `people`. This array of [compact user](/reference/users) objects reflects the values of a `people` custom field.. [optional]  # noqa: E501
-            is_global_to_workspace (bool): This flag describes whether this custom field is available to every container in the workspace. Before project-specific custom fields, this field was always true.. [optional]  # noqa: E501
-            asana_created_field (str, none_type): *Conditional*. A unique identifier to associate this field with the template source of truth.. [optional]  # noqa: E501
+            archived (bool): True if the project is archived, false if not. Archived projects do not show in the UI by default and may be treated differently for queries.. [optional]  # noqa: E501
+            color (str, none_type): Color of the project.. [optional]  # noqa: E501
+            created_at (datetime): The time at which this resource was created.. [optional]  # noqa: E501
+            current_status (bool, date, datetime, dict, float, int, list, str, none_type): *Deprecated: new integrations should prefer the `current_status_update` resource.*. [optional]  # noqa: E501
+            current_status_update (bool, date, datetime, dict, float, int, list, str, none_type): The latest `status_update` posted to this project.. [optional]  # noqa: E501
+            custom_field_settings ([CustomFieldSettingResponse]): Array of Custom Field Settings (in compact form).. [optional]  # noqa: E501
+            default_view (str): The default view (list, board, calendar, or timeline) of a project.. [optional]  # noqa: E501
+            due_date (datetime, none_type): *Deprecated: new integrations should prefer the `due_on` field.*. [optional]  # noqa: E501
+            due_on (datetime, none_type): The day on which this project is due. This takes a date with format YYYY-MM-DD.. [optional]  # noqa: E501
+            html_notes (str): [Opt In](/docs/inputoutput-options). The notes of the project with formatting as HTML.. [optional]  # noqa: E501
+            members ([UserCompact]): Array of users who are members of this project.. [optional]  # noqa: E501
+            modified_at (datetime): The time at which this project was last modified. *Note: This does not currently reflect any changes in associations such as tasks or comments that may have been added or removed from the project.*. [optional]  # noqa: E501
+            notes (str): Free-form textual information associated with the project (ie., its description).. [optional]  # noqa: E501
+            public (bool): True if the project is public to its team.. [optional]  # noqa: E501
+            start_on (date, none_type): The day on which work for this project begins, or null if the project has no start date. This takes a date with `YYYY-MM-DD` format. *Note: `due_on` or `due_at` must be present in the request when setting or unsetting the `start_on` parameter. Additionally, `start_on` and `due_on` cannot be the same date.*. [optional]  # noqa: E501
+            workspace (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `asana-preview-1.0.4/asana_preview/model/custom_field_setting_compact.py` & `asana-preview-1.0.5/asana_preview/model/project_brief_compact.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -27,20 +27,18 @@
     OpenApiModel
 )
 from asana_preview.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from asana_preview.model.asana_resource import AsanaResource
-    from asana_preview.model.custom_field_setting_compact_all_of import CustomFieldSettingCompactAllOf
     globals()['AsanaResource'] = AsanaResource
-    globals()['CustomFieldSettingCompactAllOf'] = CustomFieldSettingCompactAllOf
 
 
-class CustomFieldSettingCompact(ModelComposed):
+class ProjectBriefCompact(ModelComposed):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -86,35 +84,36 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'gid': (str,),  # noqa: E501
-            'resource_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'resource_type': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'gid': 'gid',  # noqa: E501
         'resource_type': 'resource_type',  # noqa: E501
     }
 
     read_only_vars = {
         'gid',  # noqa: E501
+        'resource_type',  # noqa: E501
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """CustomFieldSettingCompact - a model defined in OpenAPI
+        """ProjectBriefCompact - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -140,15 +139,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -211,15 +210,15 @@
         '_composed_instances',
         '_var_name_to_model_instances',
         '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """CustomFieldSettingCompact - a model defined in OpenAPI
+        """ProjectBriefCompact - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -245,15 +244,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -316,12 +315,11 @@
         # loading
         lazy_import()
         return {
           'anyOf': [
           ],
           'allOf': [
               AsanaResource,
-              CustomFieldSettingCompactAllOf,
           ],
           'oneOf': [
           ],
         }
```

### Comparing `asana-preview-1.0.4/asana_preview/model/custom_field_setting_compact_all_of.py` & `asana-preview-1.0.5/asana_preview/model/custom_field_setting_compact_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/asana_preview/model/custom_field_setting_response.py` & `asana-preview-1.0.5/asana_preview/model/custom_field_setting_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -86,15 +86,15 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'gid': (str,),  # noqa: E501
-            'resource_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'resource_type': (str,),  # noqa: E501
             'project': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'is_important': (bool,),  # noqa: E501
             'parent': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'custom_field': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
         }
 
     @cached_property
@@ -109,14 +109,15 @@
         'is_important': 'is_important',  # noqa: E501
         'parent': 'parent',  # noqa: E501
         'custom_field': 'custom_field',  # noqa: E501
     }
 
     read_only_vars = {
         'gid',  # noqa: E501
+        'resource_type',  # noqa: E501
         'is_important',  # noqa: E501
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
         """CustomFieldSettingResponse - a model defined in OpenAPI
@@ -149,15 +150,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
             project (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             is_important (bool): `is_important` is used in the Asana web application to determine if this custom field is displayed in the list/grid view of a project or portfolio.. [optional]  # noqa: E501
             parent (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             custom_field (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
@@ -258,15 +259,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
             project (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             is_important (bool): `is_important` is used in the Asana web application to determine if this custom field is displayed in the list/grid view of a project or portfolio.. [optional]  # noqa: E501
             parent (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             custom_field (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
```

### Comparing `asana-preview-1.0.4/asana_preview/model/custom_field_setting_response_all_of.py` & `asana-preview-1.0.5/asana_preview/model/custom_field_setting_response_all_of.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `asana-preview-1.0.4/asana_preview/model/enum_option.py` & `asana-preview-1.0.5/asana_preview/model/enum_option.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -86,15 +86,15 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'gid': (str,),  # noqa: E501
-            'resource_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'resource_type': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'enabled': (bool,),  # noqa: E501
             'color': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
@@ -107,14 +107,15 @@
         'name': 'name',  # noqa: E501
         'enabled': 'enabled',  # noqa: E501
         'color': 'color',  # noqa: E501
     }
 
     read_only_vars = {
         'gid',  # noqa: E501
+        'resource_type',  # noqa: E501
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
         """EnumOption - a model defined in OpenAPI
 
@@ -146,15 +147,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
             name (str): The name of the enum option.. [optional]  # noqa: E501
             enabled (bool): Whether or not the enum option is a selectable value for the custom field.. [optional]  # noqa: E501
             color (str): The color of the enum option. Defaults to ‘none’.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
@@ -254,15 +255,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
             name (str): The name of the enum option.. [optional]  # noqa: E501
             enabled (bool): Whether or not the enum option is a selectable value for the custom field.. [optional]  # noqa: E501
             color (str): The color of the enum option. Defaults to ‘none’.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
```

### Comparing `asana-preview-1.0.4/asana_preview/model/enum_option_all_of.py` & `asana-preview-1.0.5/asana_preview/model/enum_option_all_of.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -77,27 +77,25 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'resource_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'enabled': (bool,),  # noqa: E501
             'color': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'resource_type': 'resource_type',  # noqa: E501
         'name': 'name',  # noqa: E501
         'enabled': 'enabled',  # noqa: E501
         'color': 'color',  # noqa: E501
     }
 
     read_only_vars = {
     }
@@ -136,15 +134,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             name (str): The name of the enum option.. [optional]  # noqa: E501
             enabled (bool): Whether or not the enum option is a selectable value for the custom field.. [optional]  # noqa: E501
             color (str): The color of the enum option. Defaults to ‘none’.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
@@ -225,15 +222,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             name (str): The name of the enum option.. [optional]  # noqa: E501
             enabled (bool): Whether or not the enum option is a selectable value for the custom field.. [optional]  # noqa: E501
             color (str): The color of the enum option. Defaults to ‘none’.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
```

### Comparing `asana-preview-1.0.4/asana_preview/model/error_response.py` & `asana-preview-1.0.5/asana_preview/model/error_response5_xx_all_of.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,19 +26,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from asana_preview.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from asana_preview.model.error_response_errors_inner import ErrorResponseErrorsInner
-    globals()['ErrorResponseErrorsInner'] = ErrorResponseErrorsInner
+    from asana_preview.model.error_response5_xx_all_of_errors import ErrorResponse5XXAllOfErrors
+    globals()['ErrorResponse5XXAllOfErrors'] = ErrorResponse5XXAllOfErrors
 
 
-class ErrorResponse(ModelNormal):
+class ErrorResponse5XXAllOf(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -83,15 +83,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'errors': ([ErrorResponseErrorsInner],),  # noqa: E501
+            'errors': ([ErrorResponse5XXAllOfErrors],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -103,15 +103,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ErrorResponse - a model defined in OpenAPI
+        """ErrorResponse5XXAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -136,15 +136,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            errors ([ErrorResponseErrorsInner]): [optional]  # noqa: E501
+            errors ([ErrorResponse5XXAllOfErrors]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -189,15 +189,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ErrorResponse - a model defined in OpenAPI
+        """ErrorResponse5XXAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -222,15 +222,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            errors ([ErrorResponseErrorsInner]): [optional]  # noqa: E501
+            errors ([ErrorResponse5XXAllOfErrors]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `asana-preview-1.0.4/asana_preview/model/error_response5_xx.py` & `asana-preview-1.0.5/asana_preview/model/error_response5_xx.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/asana_preview/model/error_response5_xx_all_of.py` & `asana-preview-1.0.5/asana_preview/model/error_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,19 +26,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from asana_preview.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from asana_preview.model.error_response5_xx_all_of_errors import ErrorResponse5XXAllOfErrors
-    globals()['ErrorResponse5XXAllOfErrors'] = ErrorResponse5XXAllOfErrors
+    from asana_preview.model.error import Error
+    globals()['Error'] = Error
 
 
-class ErrorResponse5XXAllOf(ModelNormal):
+class ErrorResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -83,15 +83,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'errors': ([ErrorResponse5XXAllOfErrors],),  # noqa: E501
+            'errors': ([Error],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -103,15 +103,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ErrorResponse5XXAllOf - a model defined in OpenAPI
+        """ErrorResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -136,15 +136,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            errors ([ErrorResponse5XXAllOfErrors]): [optional]  # noqa: E501
+            errors ([Error]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -189,15 +189,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ErrorResponse5XXAllOf - a model defined in OpenAPI
+        """ErrorResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -222,15 +222,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            errors ([ErrorResponse5XXAllOfErrors]): [optional]  # noqa: E501
+            errors ([Error]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `asana-preview-1.0.4/asana_preview/model/error_response5_xx_all_of_errors.py` & `asana-preview-1.0.5/asana_preview/model/error_response5_xx_all_of_errors.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/asana_preview/model/error_response_errors_inner.py` & `asana-preview-1.0.5/asana_preview/model/error_response_errors_inner.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/asana_preview/model/event_response.py` & `asana-preview-1.0.5/asana_preview/model/event_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `asana-preview-1.0.4/asana_preview/model/event_response_change.py` & `asana-preview-1.0.5/asana_preview/model/event_response_change.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `asana-preview-1.0.4/asana_preview/model/event_response_parent.py` & `asana-preview-1.0.5/asana_preview/model/custom_field_setting_compact.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,19 +26,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from asana_preview.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from asana_preview.model.asana_named_resource import AsanaNamedResource
-    globals()['AsanaNamedResource'] = AsanaNamedResource
+    from asana_preview.model.asana_resource import AsanaResource
+    globals()['AsanaResource'] = AsanaResource
 
 
-class EventResponseParent(ModelComposed):
+class CustomFieldSettingCompact(ModelComposed):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -85,37 +85,35 @@
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'gid': (str,),  # noqa: E501
             'resource_type': (str,),  # noqa: E501
-            'name': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'gid': 'gid',  # noqa: E501
         'resource_type': 'resource_type',  # noqa: E501
-        'name': 'name',  # noqa: E501
     }
 
     read_only_vars = {
         'gid',  # noqa: E501
         'resource_type',  # noqa: E501
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """EventResponseParent - a model defined in OpenAPI
+        """CustomFieldSettingCompact - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -142,15 +140,14 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
             resource_type (str): The base type of this resource.. [optional]  # noqa: E501
-            name (str): The name of the object.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -213,15 +210,15 @@
         '_composed_instances',
         '_var_name_to_model_instances',
         '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """EventResponseParent - a model defined in OpenAPI
+        """CustomFieldSettingCompact - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -248,15 +245,14 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
             resource_type (str): The base type of this resource.. [optional]  # noqa: E501
-            name (str): The name of the object.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -318,12 +314,12 @@
         # classes don't exist yet because their module has not finished
         # loading
         lazy_import()
         return {
           'anyOf': [
           ],
           'allOf': [
-              AsanaNamedResource,
+              AsanaResource,
           ],
           'oneOf': [
           ],
         }
```

### Comparing `asana-preview-1.0.4/asana_preview/model/event_response_resource.py` & `asana-preview-1.0.5/asana_preview/model/event_response_parent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -30,15 +30,15 @@
 
 
 def lazy_import():
     from asana_preview.model.asana_named_resource import AsanaNamedResource
     globals()['AsanaNamedResource'] = AsanaNamedResource
 
 
-class EventResponseResource(ModelComposed):
+class EventResponseParent(ModelComposed):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -107,15 +107,15 @@
         'gid',  # noqa: E501
         'resource_type',  # noqa: E501
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """EventResponseResource - a model defined in OpenAPI
+        """EventResponseParent - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -213,15 +213,15 @@
         '_composed_instances',
         '_var_name_to_model_instances',
         '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """EventResponseResource - a model defined in OpenAPI
+        """EventResponseParent - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `asana-preview-1.0.4/asana_preview/model/event_response_user.py` & `asana-preview-1.0.5/asana_preview/model/event_response_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -84,15 +84,15 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'gid': (str,),  # noqa: E501
-            'resource_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'resource_type': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
@@ -101,14 +101,15 @@
         'gid': 'gid',  # noqa: E501
         'resource_type': 'resource_type',  # noqa: E501
         'name': 'name',  # noqa: E501
     }
 
     read_only_vars = {
         'gid',  # noqa: E501
+        'resource_type',  # noqa: E501
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
         """EventResponseUser - a model defined in OpenAPI
 
@@ -140,15 +141,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
             name (str): *Read-only except when same user as requester*. The user’s name.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -246,15 +247,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
             name (str): *Read-only except when same user as requester*. The user’s name.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `asana-preview-1.0.4/asana_preview/model/get_events200_response.py` & `asana-preview-1.0.5/asana_preview/model/get_events200_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `asana-preview-1.0.4/asana_preview/model/get_events401_response.py` & `asana-preview-1.0.5/asana_preview/model/get_events401_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/asana_preview/model/get_events401_response_all_of.py` & `asana-preview-1.0.5/asana_preview/model/get_events401_response_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/asana_preview/model/get_events401_response_all_of_errors_inner.py` & `asana-preview-1.0.5/asana_preview/model/get_events401_response_all_of_errors_inner.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/asana_preview/model/get_events403_response.py` & `asana-preview-1.0.5/asana_preview/model/get_events403_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/asana_preview/model/get_events403_response_all_of.py` & `asana-preview-1.0.5/asana_preview/model/get_events403_response_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/asana_preview/model/get_events403_response_all_of_errors_inner.py` & `asana-preview-1.0.5/asana_preview/model/get_events403_response_all_of_errors_inner.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/asana_preview/model/get_events404_response.py` & `asana-preview-1.0.5/asana_preview/model/get_events404_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/asana_preview/model/get_events404_response_all_of.py` & `asana-preview-1.0.5/asana_preview/model/get_events404_response_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/asana_preview/model/get_events404_response_all_of_errors_inner.py` & `asana-preview-1.0.5/asana_preview/model/get_events404_response_all_of_errors_inner.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/asana_preview/model/get_events412_response.py` & `asana-preview-1.0.5/asana_preview/model/get_events412_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/asana_preview/model/get_events412_response_all_of.py` & `asana-preview-1.0.5/asana_preview/model/get_events412_response_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/asana_preview/model/get_events412_response_all_of_errors_inner.py` & `asana-preview-1.0.5/asana_preview/model/get_events412_response_all_of_errors_inner.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/asana_preview/model/get_events500_response.py` & `asana-preview-1.0.5/asana_preview/model/get_events500_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/asana_preview/model/get_events500_response_all_of.py` & `asana-preview-1.0.5/asana_preview/model/get_events500_response_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/asana_preview/model/get_events500_response_all_of_errors_inner.py` & `asana-preview-1.0.5/asana_preview/model/get_events500_response_all_of_errors_inner.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/asana_preview/model/get_project200_response.py` & `asana-preview-1.0.5/asana_preview/model/get_project200_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/asana_preview/model/get_projects200_response.py` & `asana-preview-1.0.5/asana_preview/model/get_projects200_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/asana_preview/model/get_sections_for_project200_response.py` & `asana-preview-1.0.5/asana_preview/model/get_tasks_for_project200_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,20 +27,20 @@
     OpenApiModel
 )
 from asana_preview.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from asana_preview.model.next_page import NextPage
-    from asana_preview.model.section_compact import SectionCompact
+    from asana_preview.model.task_compact import TaskCompact
     globals()['NextPage'] = NextPage
-    globals()['SectionCompact'] = SectionCompact
+    globals()['TaskCompact'] = TaskCompact
 
 
-class GetSectionsForProject200Response(ModelNormal):
+class GetTasksForProject200Response(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -85,15 +85,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': ([SectionCompact],),  # noqa: E501
+            'data': ([TaskCompact],),  # noqa: E501
             'next_page': (NextPage,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
@@ -107,15 +107,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """GetSectionsForProject200Response - a model defined in OpenAPI
+        """GetTasksForProject200Response - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -140,15 +140,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data ([SectionCompact]): [optional]  # noqa: E501
+            data ([TaskCompact]): [optional]  # noqa: E501
             next_page (NextPage): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -194,15 +194,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """GetSectionsForProject200Response - a model defined in OpenAPI
+        """GetTasksForProject200Response - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -227,15 +227,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data ([SectionCompact]): [optional]  # noqa: E501
+            data ([TaskCompact]): [optional]  # noqa: E501
             next_page (NextPage): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `asana-preview-1.0.4/asana_preview/model/get_stories_for_task200_response.py` & `asana-preview-1.0.5/asana_preview/model/update_team_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,21 +26,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from asana_preview.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from asana_preview.model.next_page import NextPage
-    from asana_preview.model.story_compact import StoryCompact
-    globals()['NextPage'] = NextPage
-    globals()['StoryCompact'] = StoryCompact
+    from asana_preview.model.team_request import TeamRequest
+    globals()['TeamRequest'] = TeamRequest
 
 
-class GetStoriesForTask200Response(ModelNormal):
+class UpdateTeamRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -85,37 +83,35 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': ([StoryCompact],),  # noqa: E501
-            'next_page': (NextPage,),  # noqa: E501
+            'data': (TeamRequest,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'data': 'data',  # noqa: E501
-        'next_page': 'next_page',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """GetStoriesForTask200Response - a model defined in OpenAPI
+        """UpdateTeamRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -140,16 +136,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data ([StoryCompact]): [optional]  # noqa: E501
-            next_page (NextPage): [optional]  # noqa: E501
+            data (TeamRequest): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -194,15 +189,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """GetStoriesForTask200Response - a model defined in OpenAPI
+        """UpdateTeamRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -227,16 +222,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data ([StoryCompact]): [optional]  # noqa: E501
-            next_page (NextPage): [optional]  # noqa: E501
+            data (TeamRequest): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `asana-preview-1.0.4/asana_preview/model/get_task200_response.py` & `asana-preview-1.0.5/asana_preview/model/get_task200_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/asana_preview/model/get_tasks_for_project200_response.py` & `asana-preview-1.0.5/asana_preview/model/create_batch_request200_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,21 +26,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from asana_preview.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from asana_preview.model.next_page import NextPage
-    from asana_preview.model.task_compact import TaskCompact
-    globals()['NextPage'] = NextPage
-    globals()['TaskCompact'] = TaskCompact
+    from asana_preview.model.batch_response import BatchResponse
+    globals()['BatchResponse'] = BatchResponse
 
 
-class GetTasksForProject200Response(ModelNormal):
+class CreateBatchRequest200Response(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -85,37 +83,35 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': ([TaskCompact],),  # noqa: E501
-            'next_page': (NextPage,),  # noqa: E501
+            'data': ([BatchResponse],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'data': 'data',  # noqa: E501
-        'next_page': 'next_page',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """GetTasksForProject200Response - a model defined in OpenAPI
+        """CreateBatchRequest200Response - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -140,16 +136,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data ([TaskCompact]): [optional]  # noqa: E501
-            next_page (NextPage): [optional]  # noqa: E501
+            data ([BatchResponse]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -194,15 +189,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """GetTasksForProject200Response - a model defined in OpenAPI
+        """CreateBatchRequest200Response - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -227,16 +222,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data ([TaskCompact]): [optional]  # noqa: E501
-            next_page (NextPage): [optional]  # noqa: E501
+            data ([BatchResponse]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `asana-preview-1.0.4/asana_preview/model/get_user200_response.py` & `asana-preview-1.0.5/asana_preview/model/get_user200_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `asana-preview-1.0.4/asana_preview/model/like.py` & `asana-preview-1.0.5/asana_preview/model/like.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `asana-preview-1.0.4/asana_preview/model/next_page.py` & `asana-preview-1.0.5/asana_preview/model/next_page.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/asana_preview/model/project_base.py` & `asana-preview-1.0.5/asana_preview/model/project_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -117,25 +117,25 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'gid': (str,),  # noqa: E501
-            'resource_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'resource_type': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'archived': (bool,),  # noqa: E501
             'color': (str, none_type,),  # noqa: E501
             'created_at': (datetime,),  # noqa: E501
             'current_status': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'current_status_update': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'custom_field_settings': ([CustomFieldSettingResponse],),  # noqa: E501
             'default_view': (str,),  # noqa: E501
-            'due_date': (date, none_type,),  # noqa: E501
-            'due_on': (date, none_type,),  # noqa: E501
+            'due_date': (datetime, none_type,),  # noqa: E501
+            'due_on': (datetime, none_type,),  # noqa: E501
             'html_notes': (str,),  # noqa: E501
             'members': ([UserCompact],),  # noqa: E501
             'modified_at': (datetime,),  # noqa: E501
             'notes': (str,),  # noqa: E501
             'public': (bool,),  # noqa: E501
             'start_on': (date, none_type,),  # noqa: E501
             'workspace': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
@@ -166,14 +166,15 @@
         'public': 'public',  # noqa: E501
         'start_on': 'start_on',  # noqa: E501
         'workspace': 'workspace',  # noqa: E501
     }
 
     read_only_vars = {
         'gid',  # noqa: E501
+        'resource_type',  # noqa: E501
         'created_at',  # noqa: E501
         'custom_field_settings',  # noqa: E501
         'members',  # noqa: E501
         'modified_at',  # noqa: E501
     }
 
     @classmethod
@@ -209,25 +210,25 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
             name (str): Name of the project. This is generally a short sentence fragment that fits on a line in the UI for maximum readability. However, it can be longer.. [optional]  # noqa: E501
             archived (bool): True if the project is archived, false if not. Archived projects do not show in the UI by default and may be treated differently for queries.. [optional]  # noqa: E501
             color (str, none_type): Color of the project.. [optional]  # noqa: E501
-            created_at (datetime): The time at which this project was created.. [optional]  # noqa: E501
+            created_at (datetime): The time at which this resource was created.. [optional]  # noqa: E501
             current_status (bool, date, datetime, dict, float, int, list, str, none_type): *Deprecated: new integrations should prefer the `current_status_update` resource.*. [optional]  # noqa: E501
             current_status_update (bool, date, datetime, dict, float, int, list, str, none_type): The latest `status_update` posted to this project.. [optional]  # noqa: E501
             custom_field_settings ([CustomFieldSettingResponse]): Array of Custom Field Settings (in compact form).. [optional]  # noqa: E501
             default_view (str): The default view (list, board, calendar, or timeline) of a project.. [optional]  # noqa: E501
-            due_date (date, none_type): *Deprecated: new integrations should prefer the `due_on` field.*. [optional]  # noqa: E501
-            due_on (date, none_type): The day on which this project is due. This takes a date with format YYYY-MM-DD.. [optional]  # noqa: E501
+            due_date (datetime, none_type): *Deprecated: new integrations should prefer the `due_on` field.*. [optional]  # noqa: E501
+            due_on (datetime, none_type): The day on which this project is due. This takes a date with format YYYY-MM-DD.. [optional]  # noqa: E501
             html_notes (str): [Opt In](/docs/inputoutput-options). The notes of the project with formatting as HTML.. [optional]  # noqa: E501
             members ([UserCompact]): Array of users who are members of this project.. [optional]  # noqa: E501
             modified_at (datetime): The time at which this project was last modified. *Note: This does not currently reflect any changes in associations such as tasks or comments that may have been added or removed from the project.*. [optional]  # noqa: E501
             notes (str): Free-form textual information associated with the project (ie., its description).. [optional]  # noqa: E501
             public (bool): True if the project is public to its team.. [optional]  # noqa: E501
             start_on (date, none_type): The day on which work for this project begins, or null if the project has no start date. This takes a date with `YYYY-MM-DD` format. *Note: `due_on` or `due_at` must be present in the request when setting or unsetting the `start_on` parameter. Additionally, `start_on` and `due_on` cannot be the same date.*. [optional]  # noqa: E501
             workspace (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
@@ -331,25 +332,25 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
             name (str): Name of the project. This is generally a short sentence fragment that fits on a line in the UI for maximum readability. However, it can be longer.. [optional]  # noqa: E501
             archived (bool): True if the project is archived, false if not. Archived projects do not show in the UI by default and may be treated differently for queries.. [optional]  # noqa: E501
             color (str, none_type): Color of the project.. [optional]  # noqa: E501
-            created_at (datetime): The time at which this project was created.. [optional]  # noqa: E501
+            created_at (datetime): The time at which this resource was created.. [optional]  # noqa: E501
             current_status (bool, date, datetime, dict, float, int, list, str, none_type): *Deprecated: new integrations should prefer the `current_status_update` resource.*. [optional]  # noqa: E501
             current_status_update (bool, date, datetime, dict, float, int, list, str, none_type): The latest `status_update` posted to this project.. [optional]  # noqa: E501
             custom_field_settings ([CustomFieldSettingResponse]): Array of Custom Field Settings (in compact form).. [optional]  # noqa: E501
             default_view (str): The default view (list, board, calendar, or timeline) of a project.. [optional]  # noqa: E501
-            due_date (date, none_type): *Deprecated: new integrations should prefer the `due_on` field.*. [optional]  # noqa: E501
-            due_on (date, none_type): The day on which this project is due. This takes a date with format YYYY-MM-DD.. [optional]  # noqa: E501
+            due_date (datetime, none_type): *Deprecated: new integrations should prefer the `due_on` field.*. [optional]  # noqa: E501
+            due_on (datetime, none_type): The day on which this project is due. This takes a date with format YYYY-MM-DD.. [optional]  # noqa: E501
             html_notes (str): [Opt In](/docs/inputoutput-options). The notes of the project with formatting as HTML.. [optional]  # noqa: E501
             members ([UserCompact]): Array of users who are members of this project.. [optional]  # noqa: E501
             modified_at (datetime): The time at which this project was last modified. *Note: This does not currently reflect any changes in associations such as tasks or comments that may have been added or removed from the project.*. [optional]  # noqa: E501
             notes (str): Free-form textual information associated with the project (ie., its description).. [optional]  # noqa: E501
             public (bool): True if the project is public to its team.. [optional]  # noqa: E501
             start_on (date, none_type): The day on which work for this project begins, or null if the project has no start date. This takes a date with `YYYY-MM-DD` format. *Note: `due_on` or `due_at` must be present in the request when setting or unsetting the `start_on` parameter. Additionally, `start_on` and `due_on` cannot be the same date.*. [optional]  # noqa: E501
             workspace (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
```

### Comparing `asana-preview-1.0.4/asana_preview/model/project_base_all_of.py` & `asana-preview-1.0.5/asana_preview/model/project_template_base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,21 +26,25 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from asana_preview.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from asana_preview.model.custom_field_setting_response import CustomFieldSettingResponse
-    from asana_preview.model.user_compact import UserCompact
-    globals()['CustomFieldSettingResponse'] = CustomFieldSettingResponse
-    globals()['UserCompact'] = UserCompact
+    from asana_preview.model.date_variable_compact import DateVariableCompact
+    from asana_preview.model.project_template_base_all_of import ProjectTemplateBaseAllOf
+    from asana_preview.model.project_template_compact import ProjectTemplateCompact
+    from asana_preview.model.template_role import TemplateRole
+    globals()['DateVariableCompact'] = DateVariableCompact
+    globals()['ProjectTemplateBaseAllOf'] = ProjectTemplateBaseAllOf
+    globals()['ProjectTemplateCompact'] = ProjectTemplateCompact
+    globals()['TemplateRole'] = TemplateRole
 
 
-class ProjectBaseAllOf(ModelNormal):
+class ProjectTemplateBase(ModelComposed):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,20 +82,14 @@
             'LIGHT-RED': "light-red",
             'LIGHT-TEAL': "light-teal",
             'LIGHT-BROWN': "light-brown",
             'LIGHT-ORANGE': "light-orange",
             'LIGHT-PURPLE': "light-purple",
             'LIGHT-WARM-GRAY': "light-warm-gray",
         },
-        ('default_view',): {
-            'LIST': "list",
-            'BOARD': "board",
-            'CALENDAR': "calendar",
-            'TIMELINE': "timeline",
-        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
@@ -112,69 +110,56 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'archived': (bool,),  # noqa: E501
-            'color': (str, none_type,),  # noqa: E501
-            'created_at': (datetime,),  # noqa: E501
-            'current_status': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
-            'current_status_update': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
-            'custom_field_settings': ([CustomFieldSettingResponse],),  # noqa: E501
-            'default_view': (str,),  # noqa: E501
-            'due_date': (date, none_type,),  # noqa: E501
-            'due_on': (date, none_type,),  # noqa: E501
-            'html_notes': (str,),  # noqa: E501
-            'members': ([UserCompact],),  # noqa: E501
-            'modified_at': (datetime,),  # noqa: E501
-            'notes': (str,),  # noqa: E501
+            'gid': (str,),  # noqa: E501
+            'resource_type': (str,),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'description': (str,),  # noqa: E501
+            'html_description': (str,),  # noqa: E501
             'public': (bool,),  # noqa: E501
-            'start_on': (date, none_type,),  # noqa: E501
-            'workspace': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'owner': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'team': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'requested_dates': ([DateVariableCompact],),  # noqa: E501
+            'color': (str, none_type,),  # noqa: E501
+            'requested_roles': ([TemplateRole],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'archived': 'archived',  # noqa: E501
-        'color': 'color',  # noqa: E501
-        'created_at': 'created_at',  # noqa: E501
-        'current_status': 'current_status',  # noqa: E501
-        'current_status_update': 'current_status_update',  # noqa: E501
-        'custom_field_settings': 'custom_field_settings',  # noqa: E501
-        'default_view': 'default_view',  # noqa: E501
-        'due_date': 'due_date',  # noqa: E501
-        'due_on': 'due_on',  # noqa: E501
-        'html_notes': 'html_notes',  # noqa: E501
-        'members': 'members',  # noqa: E501
-        'modified_at': 'modified_at',  # noqa: E501
-        'notes': 'notes',  # noqa: E501
+        'gid': 'gid',  # noqa: E501
+        'resource_type': 'resource_type',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'description': 'description',  # noqa: E501
+        'html_description': 'html_description',  # noqa: E501
         'public': 'public',  # noqa: E501
-        'start_on': 'start_on',  # noqa: E501
-        'workspace': 'workspace',  # noqa: E501
+        'owner': 'owner',  # noqa: E501
+        'team': 'team',  # noqa: E501
+        'requested_dates': 'requested_dates',  # noqa: E501
+        'color': 'color',  # noqa: E501
+        'requested_roles': 'requested_roles',  # noqa: E501
     }
 
     read_only_vars = {
-        'created_at',  # noqa: E501
-        'custom_field_settings',  # noqa: E501
-        'members',  # noqa: E501
-        'modified_at',  # noqa: E501
+        'gid',  # noqa: E501
+        'resource_type',  # noqa: E501
+        'requested_dates',  # noqa: E501
     }
 
-    _composed_schemas = {}
-
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ProjectBaseAllOf - a model defined in OpenAPI
+        """ProjectTemplateBase - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -199,34 +184,29 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            archived (bool): True if the project is archived, false if not. Archived projects do not show in the UI by default and may be treated differently for queries.. [optional]  # noqa: E501
-            color (str, none_type): Color of the project.. [optional]  # noqa: E501
-            created_at (datetime): The time at which this project was created.. [optional]  # noqa: E501
-            current_status (bool, date, datetime, dict, float, int, list, str, none_type): *Deprecated: new integrations should prefer the `current_status_update` resource.*. [optional]  # noqa: E501
-            current_status_update (bool, date, datetime, dict, float, int, list, str, none_type): The latest `status_update` posted to this project.. [optional]  # noqa: E501
-            custom_field_settings ([CustomFieldSettingResponse]): Array of Custom Field Settings (in compact form).. [optional]  # noqa: E501
-            default_view (str): The default view (list, board, calendar, or timeline) of a project.. [optional]  # noqa: E501
-            due_date (date, none_type): *Deprecated: new integrations should prefer the `due_on` field.*. [optional]  # noqa: E501
-            due_on (date, none_type): The day on which this project is due. This takes a date with format YYYY-MM-DD.. [optional]  # noqa: E501
-            html_notes (str): [Opt In](/docs/inputoutput-options). The notes of the project with formatting as HTML.. [optional]  # noqa: E501
-            members ([UserCompact]): Array of users who are members of this project.. [optional]  # noqa: E501
-            modified_at (datetime): The time at which this project was last modified. *Note: This does not currently reflect any changes in associations such as tasks or comments that may have been added or removed from the project.*. [optional]  # noqa: E501
-            notes (str): Free-form textual information associated with the project (ie., its description).. [optional]  # noqa: E501
-            public (bool): True if the project is public to its team.. [optional]  # noqa: E501
-            start_on (date, none_type): The day on which work for this project begins, or null if the project has no start date. This takes a date with `YYYY-MM-DD` format. *Note: `due_on` or `due_at` must be present in the request when setting or unsetting the `start_on` parameter. Additionally, `start_on` and `due_on` cannot be the same date.*. [optional]  # noqa: E501
-            workspace (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
+            name (str): Name of the project template.. [optional]  # noqa: E501
+            description (str): Free-form textual information associated with the project template. [optional]  # noqa: E501
+            html_description (str): The description of the project template with formatting as HTML.. [optional]  # noqa: E501
+            public (bool): True if the project template is public to its team.. [optional]  # noqa: E501
+            owner (bool, date, datetime, dict, float, int, list, str, none_type): The current owner of the project template, may be null.. [optional]  # noqa: E501
+            team (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            requested_dates ([DateVariableCompact]): Array of date variables in this project template. Calendar dates must be provided for these variables when instantiating a project.. [optional]  # noqa: E501
+            color (str, none_type): Color of the project template.. [optional]  # noqa: E501
+            requested_roles ([TemplateRole]): Array of template roles in this project template. User Ids can be provided for these variables when instantiating a project to assign template tasks to the user.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         self = super(OpenApiModel, cls).__new__(cls)
 
         if args:
@@ -246,36 +226,54 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        constant_args = {
+            '_check_type': _check_type,
+            '_path_to_item': _path_to_item,
+            '_spec_property_naming': _spec_property_naming,
+            '_configuration': _configuration,
+            '_visited_composed_classes': self._visited_composed_classes,
+        }
+        composed_info = validate_get_composed_info(
+            constant_args, kwargs, self)
+        self._composed_instances = composed_info[0]
+        self._var_name_to_model_instances = composed_info[1]
+        self._additional_properties_model_instances = composed_info[2]
+        discarded_args = composed_info[3]
+
         for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
+            if var_name in discarded_args and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
+                        self._additional_properties_model_instances:
                 # discard variable.
                 continue
             setattr(self, var_name, var_value)
+
         return self
 
     required_properties = set([
         '_data_store',
         '_check_type',
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
+        '_composed_instances',
+        '_var_name_to_model_instances',
+        '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ProjectBaseAllOf - a model defined in OpenAPI
+        """ProjectTemplateBase - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -300,30 +298,25 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            archived (bool): True if the project is archived, false if not. Archived projects do not show in the UI by default and may be treated differently for queries.. [optional]  # noqa: E501
-            color (str, none_type): Color of the project.. [optional]  # noqa: E501
-            created_at (datetime): The time at which this project was created.. [optional]  # noqa: E501
-            current_status (bool, date, datetime, dict, float, int, list, str, none_type): *Deprecated: new integrations should prefer the `current_status_update` resource.*. [optional]  # noqa: E501
-            current_status_update (bool, date, datetime, dict, float, int, list, str, none_type): The latest `status_update` posted to this project.. [optional]  # noqa: E501
-            custom_field_settings ([CustomFieldSettingResponse]): Array of Custom Field Settings (in compact form).. [optional]  # noqa: E501
-            default_view (str): The default view (list, board, calendar, or timeline) of a project.. [optional]  # noqa: E501
-            due_date (date, none_type): *Deprecated: new integrations should prefer the `due_on` field.*. [optional]  # noqa: E501
-            due_on (date, none_type): The day on which this project is due. This takes a date with format YYYY-MM-DD.. [optional]  # noqa: E501
-            html_notes (str): [Opt In](/docs/inputoutput-options). The notes of the project with formatting as HTML.. [optional]  # noqa: E501
-            members ([UserCompact]): Array of users who are members of this project.. [optional]  # noqa: E501
-            modified_at (datetime): The time at which this project was last modified. *Note: This does not currently reflect any changes in associations such as tasks or comments that may have been added or removed from the project.*. [optional]  # noqa: E501
-            notes (str): Free-form textual information associated with the project (ie., its description).. [optional]  # noqa: E501
-            public (bool): True if the project is public to its team.. [optional]  # noqa: E501
-            start_on (date, none_type): The day on which work for this project begins, or null if the project has no start date. This takes a date with `YYYY-MM-DD` format. *Note: `due_on` or `due_at` must be present in the request when setting or unsetting the `start_on` parameter. Additionally, `start_on` and `due_on` cannot be the same date.*. [optional]  # noqa: E501
-            workspace (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
+            name (str): Name of the project template.. [optional]  # noqa: E501
+            description (str): Free-form textual information associated with the project template. [optional]  # noqa: E501
+            html_description (str): The description of the project template with formatting as HTML.. [optional]  # noqa: E501
+            public (bool): True if the project template is public to its team.. [optional]  # noqa: E501
+            owner (bool, date, datetime, dict, float, int, list, str, none_type): The current owner of the project template, may be null.. [optional]  # noqa: E501
+            team (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            requested_dates ([DateVariableCompact]): Array of date variables in this project template. Calendar dates must be provided for these variables when instantiating a project.. [optional]  # noqa: E501
+            color (str, none_type): Color of the project template.. [optional]  # noqa: E501
+            requested_roles ([TemplateRole]): Array of template roles in this project template. User Ids can be provided for these variables when instantiating a project to assign template tasks to the user.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -345,18 +338,53 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        constant_args = {
+            '_check_type': _check_type,
+            '_path_to_item': _path_to_item,
+            '_spec_property_naming': _spec_property_naming,
+            '_configuration': _configuration,
+            '_visited_composed_classes': self._visited_composed_classes,
+        }
+        composed_info = validate_get_composed_info(
+            constant_args, kwargs, self)
+        self._composed_instances = composed_info[0]
+        self._var_name_to_model_instances = composed_info[1]
+        self._additional_properties_model_instances = composed_info[2]
+        discarded_args = composed_info[3]
+
         for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
+            if var_name in discarded_args and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
+                        self._additional_properties_model_instances:
                 # discard variable.
                 continue
             setattr(self, var_name, var_value)
             if var_name in self.read_only_vars:
                 raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
                                      f"class with read only attributes.")
+
+    @cached_property
+    def _composed_schemas():
+        # we need this here to make our import statements work
+        # we must store _composed_schemas in here so the code is only run
+        # when we invoke this method. If we kept this at the class
+        # level we would get an error because the class level
+        # code would be run when this module is imported, and these composed
+        # classes don't exist yet because their module has not finished
+        # loading
+        lazy_import()
+        return {
+          'anyOf': [
+          ],
+          'allOf': [
+              ProjectTemplateBaseAllOf,
+              ProjectTemplateCompact,
+          ],
+          'oneOf': [
+          ],
+        }
```

### Comparing `asana-preview-1.0.4/asana_preview/model/project_brief_compact.py` & `asana-preview-1.0.5/asana_preview/model/project_membership_compact.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -27,20 +27,22 @@
     OpenApiModel
 )
 from asana_preview.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from asana_preview.model.asana_resource import AsanaResource
-    from asana_preview.model.project_brief_compact_all_of import ProjectBriefCompactAllOf
+    from asana_preview.model.project_membership_compact_all_of import ProjectMembershipCompactAllOf
+    from asana_preview.model.user_compact import UserCompact
     globals()['AsanaResource'] = AsanaResource
-    globals()['ProjectBriefCompactAllOf'] = ProjectBriefCompactAllOf
+    globals()['ProjectMembershipCompactAllOf'] = ProjectMembershipCompactAllOf
+    globals()['UserCompact'] = UserCompact
 
 
-class ProjectBriefCompact(ModelComposed):
+class ProjectMembershipCompact(ModelComposed):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -86,35 +88,38 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'gid': (str,),  # noqa: E501
-            'resource_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'resource_type': (str,),  # noqa: E501
+            'user': (UserCompact,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'gid': 'gid',  # noqa: E501
         'resource_type': 'resource_type',  # noqa: E501
+        'user': 'user',  # noqa: E501
     }
 
     read_only_vars = {
         'gid',  # noqa: E501
+        'resource_type',  # noqa: E501
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ProjectBriefCompact - a model defined in OpenAPI
+        """ProjectMembershipCompact - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -140,15 +145,16 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
+            user (UserCompact): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -211,15 +217,15 @@
         '_composed_instances',
         '_var_name_to_model_instances',
         '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ProjectBriefCompact - a model defined in OpenAPI
+        """ProjectMembershipCompact - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -245,15 +251,16 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
+            user (UserCompact): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -316,12 +323,12 @@
         # loading
         lazy_import()
         return {
           'anyOf': [
           ],
           'allOf': [
               AsanaResource,
-              ProjectBriefCompactAllOf,
+              ProjectMembershipCompactAllOf,
           ],
           'oneOf': [
           ],
         }
```

### Comparing `asana-preview-1.0.4/asana_preview/model/project_brief_compact_all_of.py` & `asana-preview-1.0.5/asana_preview/model/project_brief_compact_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/asana_preview/model/project_compact.py` & `asana-preview-1.0.5/asana_preview/model/project_compact.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -86,15 +86,15 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'gid': (str,),  # noqa: E501
-            'resource_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'resource_type': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
@@ -103,14 +103,15 @@
         'gid': 'gid',  # noqa: E501
         'resource_type': 'resource_type',  # noqa: E501
         'name': 'name',  # noqa: E501
     }
 
     read_only_vars = {
         'gid',  # noqa: E501
+        'resource_type',  # noqa: E501
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
         """ProjectCompact - a model defined in OpenAPI
 
@@ -142,15 +143,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
             name (str): Name of the project. This is generally a short sentence fragment that fits on a line in the UI for maximum readability. However, it can be longer.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -248,15 +249,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
             name (str): Name of the project. This is generally a short sentence fragment that fits on a line in the UI for maximum readability. However, it can be longer.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `asana-preview-1.0.4/asana_preview/model/project_compact_all_of.py` & `asana-preview-1.0.5/asana_preview/model/user_base_response_all_of.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -25,16 +25,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from asana_preview.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from asana_preview.model.user_base_response_all_of_photo import UserBaseResponseAllOfPhoto
+    globals()['UserBaseResponseAllOfPhoto'] = UserBaseResponseAllOfPhoto
 
-class ProjectCompactAllOf(ModelNormal):
+
+class UserBaseResponseAllOf(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -62,52 +66,55 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'resource_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
-            'name': (str,),  # noqa: E501
+            'email': (str,),  # noqa: E501
+            'photo': (UserBaseResponseAllOfPhoto,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'resource_type': 'resource_type',  # noqa: E501
-        'name': 'name',  # noqa: E501
+        'email': 'email',  # noqa: E501
+        'photo': 'photo',  # noqa: E501
     }
 
     read_only_vars = {
+        'email',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ProjectCompactAllOf - a model defined in OpenAPI
+        """UserBaseResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -132,16 +139,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            name (str): Name of the project. This is generally a short sentence fragment that fits on a line in the UI for maximum readability. However, it can be longer.. [optional]  # noqa: E501
+            email (str): The user's email address.. [optional]  # noqa: E501
+            photo (UserBaseResponseAllOfPhoto): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -186,15 +193,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ProjectCompactAllOf - a model defined in OpenAPI
+        """UserBaseResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -219,16 +226,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            name (str): Name of the project. This is generally a short sentence fragment that fits on a line in the UI for maximum readability. However, it can be longer.. [optional]  # noqa: E501
+            email (str): The user's email address.. [optional]  # noqa: E501
+            photo (UserBaseResponseAllOfPhoto): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `asana-preview-1.0.4/asana_preview/model/project_response.py` & `asana-preview-1.0.5/asana_preview/model/project_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -154,36 +154,36 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'gid': (str,),  # noqa: E501
-            'resource_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'resource_type': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'archived': (bool,),  # noqa: E501
             'color': (str, none_type,),  # noqa: E501
             'created_at': (datetime,),  # noqa: E501
             'current_status': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'current_status_update': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'custom_field_settings': ([CustomFieldSettingResponse],),  # noqa: E501
             'default_view': (str,),  # noqa: E501
-            'due_date': (date, none_type,),  # noqa: E501
-            'due_on': (date, none_type,),  # noqa: E501
+            'due_date': (datetime, none_type,),  # noqa: E501
+            'due_on': (datetime, none_type,),  # noqa: E501
             'html_notes': (str,),  # noqa: E501
             'members': ([UserCompact],),  # noqa: E501
             'modified_at': (datetime,),  # noqa: E501
             'notes': (str,),  # noqa: E501
             'public': (bool,),  # noqa: E501
             'start_on': (date, none_type,),  # noqa: E501
             'workspace': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'custom_fields': ([CustomFieldCompact],),  # noqa: E501
             'completed': (bool,),  # noqa: E501
             'completed_at': (datetime, none_type,),  # noqa: E501
-            'completed_by': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'completed_by': (UserCompact,),  # noqa: E501
             'followers': ([UserCompact],),  # noqa: E501
             'owner': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'team': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'icon': (str, none_type,),  # noqa: E501
             'permalink_url': (str,),  # noqa: E501
             'project_brief': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'created_from_template': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
@@ -225,22 +225,22 @@
         'permalink_url': 'permalink_url',  # noqa: E501
         'project_brief': 'project_brief',  # noqa: E501
         'created_from_template': 'created_from_template',  # noqa: E501
     }
 
     read_only_vars = {
         'gid',  # noqa: E501
+        'resource_type',  # noqa: E501
         'created_at',  # noqa: E501
         'custom_field_settings',  # noqa: E501
         'members',  # noqa: E501
         'modified_at',  # noqa: E501
         'custom_fields',  # noqa: E501
         'completed',  # noqa: E501
         'completed_at',  # noqa: E501
-        'completed_by',  # noqa: E501
         'followers',  # noqa: E501
         'permalink_url',  # noqa: E501
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
@@ -274,36 +274,36 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
             name (str): Name of the project. This is generally a short sentence fragment that fits on a line in the UI for maximum readability. However, it can be longer.. [optional]  # noqa: E501
             archived (bool): True if the project is archived, false if not. Archived projects do not show in the UI by default and may be treated differently for queries.. [optional]  # noqa: E501
             color (str, none_type): Color of the project.. [optional]  # noqa: E501
-            created_at (datetime): The time at which this project was created.. [optional]  # noqa: E501
+            created_at (datetime): The time at which this resource was created.. [optional]  # noqa: E501
             current_status (bool, date, datetime, dict, float, int, list, str, none_type): *Deprecated: new integrations should prefer the `current_status_update` resource.*. [optional]  # noqa: E501
             current_status_update (bool, date, datetime, dict, float, int, list, str, none_type): The latest `status_update` posted to this project.. [optional]  # noqa: E501
             custom_field_settings ([CustomFieldSettingResponse]): Array of Custom Field Settings (in compact form).. [optional]  # noqa: E501
             default_view (str): The default view (list, board, calendar, or timeline) of a project.. [optional]  # noqa: E501
-            due_date (date, none_type): *Deprecated: new integrations should prefer the `due_on` field.*. [optional]  # noqa: E501
-            due_on (date, none_type): The day on which this project is due. This takes a date with format YYYY-MM-DD.. [optional]  # noqa: E501
+            due_date (datetime, none_type): *Deprecated: new integrations should prefer the `due_on` field.*. [optional]  # noqa: E501
+            due_on (datetime, none_type): The day on which this project is due. This takes a date with format YYYY-MM-DD.. [optional]  # noqa: E501
             html_notes (str): [Opt In](/docs/inputoutput-options). The notes of the project with formatting as HTML.. [optional]  # noqa: E501
             members ([UserCompact]): Array of users who are members of this project.. [optional]  # noqa: E501
             modified_at (datetime): The time at which this project was last modified. *Note: This does not currently reflect any changes in associations such as tasks or comments that may have been added or removed from the project.*. [optional]  # noqa: E501
             notes (str): Free-form textual information associated with the project (ie., its description).. [optional]  # noqa: E501
             public (bool): True if the project is public to its team.. [optional]  # noqa: E501
             start_on (date, none_type): The day on which work for this project begins, or null if the project has no start date. This takes a date with `YYYY-MM-DD` format. *Note: `due_on` or `due_at` must be present in the request when setting or unsetting the `start_on` parameter. Additionally, `start_on` and `due_on` cannot be the same date.*. [optional]  # noqa: E501
             workspace (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             custom_fields ([CustomFieldCompact]): Array of Custom Fields.. [optional]  # noqa: E501
             completed (bool): True if the project is currently marked complete, false if not.. [optional]  # noqa: E501
             completed_at (datetime, none_type): The time at which this project was completed, or null if the project is not completed.. [optional]  # noqa: E501
-            completed_by (bool, date, datetime, dict, float, int, list, str, none_type): The user that marked this project complete, or null if the project is not completed.. [optional]  # noqa: E501
+            completed_by (UserCompact): [optional]  # noqa: E501
             followers ([UserCompact]): Array of users following this project. Followers are a subset of members who have opted in to receive \"tasks added\" notifications for a project.. [optional]  # noqa: E501
             owner (bool, date, datetime, dict, float, int, list, str, none_type): The current owner of the project, may be null.. [optional]  # noqa: E501
             team (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             icon (str, none_type): The icon for a project.. [optional]  # noqa: E501
             permalink_url (str): A url that points directly to the object within Asana.. [optional]  # noqa: E501
             project_brief (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             created_from_template (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
@@ -407,36 +407,36 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
             name (str): Name of the project. This is generally a short sentence fragment that fits on a line in the UI for maximum readability. However, it can be longer.. [optional]  # noqa: E501
             archived (bool): True if the project is archived, false if not. Archived projects do not show in the UI by default and may be treated differently for queries.. [optional]  # noqa: E501
             color (str, none_type): Color of the project.. [optional]  # noqa: E501
-            created_at (datetime): The time at which this project was created.. [optional]  # noqa: E501
+            created_at (datetime): The time at which this resource was created.. [optional]  # noqa: E501
             current_status (bool, date, datetime, dict, float, int, list, str, none_type): *Deprecated: new integrations should prefer the `current_status_update` resource.*. [optional]  # noqa: E501
             current_status_update (bool, date, datetime, dict, float, int, list, str, none_type): The latest `status_update` posted to this project.. [optional]  # noqa: E501
             custom_field_settings ([CustomFieldSettingResponse]): Array of Custom Field Settings (in compact form).. [optional]  # noqa: E501
             default_view (str): The default view (list, board, calendar, or timeline) of a project.. [optional]  # noqa: E501
-            due_date (date, none_type): *Deprecated: new integrations should prefer the `due_on` field.*. [optional]  # noqa: E501
-            due_on (date, none_type): The day on which this project is due. This takes a date with format YYYY-MM-DD.. [optional]  # noqa: E501
+            due_date (datetime, none_type): *Deprecated: new integrations should prefer the `due_on` field.*. [optional]  # noqa: E501
+            due_on (datetime, none_type): The day on which this project is due. This takes a date with format YYYY-MM-DD.. [optional]  # noqa: E501
             html_notes (str): [Opt In](/docs/inputoutput-options). The notes of the project with formatting as HTML.. [optional]  # noqa: E501
             members ([UserCompact]): Array of users who are members of this project.. [optional]  # noqa: E501
             modified_at (datetime): The time at which this project was last modified. *Note: This does not currently reflect any changes in associations such as tasks or comments that may have been added or removed from the project.*. [optional]  # noqa: E501
             notes (str): Free-form textual information associated with the project (ie., its description).. [optional]  # noqa: E501
             public (bool): True if the project is public to its team.. [optional]  # noqa: E501
             start_on (date, none_type): The day on which work for this project begins, or null if the project has no start date. This takes a date with `YYYY-MM-DD` format. *Note: `due_on` or `due_at` must be present in the request when setting or unsetting the `start_on` parameter. Additionally, `start_on` and `due_on` cannot be the same date.*. [optional]  # noqa: E501
             workspace (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             custom_fields ([CustomFieldCompact]): Array of Custom Fields.. [optional]  # noqa: E501
             completed (bool): True if the project is currently marked complete, false if not.. [optional]  # noqa: E501
             completed_at (datetime, none_type): The time at which this project was completed, or null if the project is not completed.. [optional]  # noqa: E501
-            completed_by (bool, date, datetime, dict, float, int, list, str, none_type): The user that marked this project complete, or null if the project is not completed.. [optional]  # noqa: E501
+            completed_by (UserCompact): [optional]  # noqa: E501
             followers ([UserCompact]): Array of users following this project. Followers are a subset of members who have opted in to receive \"tasks added\" notifications for a project.. [optional]  # noqa: E501
             owner (bool, date, datetime, dict, float, int, list, str, none_type): The current owner of the project, may be null.. [optional]  # noqa: E501
             team (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             icon (str, none_type): The icon for a project.. [optional]  # noqa: E501
             permalink_url (str): A url that points directly to the object within Asana.. [optional]  # noqa: E501
             project_brief (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             created_from_template (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
```

### Comparing `asana-preview-1.0.4/asana_preview/model/project_response_all_of.py` & `asana-preview-1.0.5/asana_preview/model/project_response_all_of.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -123,15 +123,15 @@
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'custom_fields': ([CustomFieldCompact],),  # noqa: E501
             'completed': (bool,),  # noqa: E501
             'completed_at': (datetime, none_type,),  # noqa: E501
-            'completed_by': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'completed_by': (UserCompact,),  # noqa: E501
             'followers': ([UserCompact],),  # noqa: E501
             'owner': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'team': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'icon': (str, none_type,),  # noqa: E501
             'permalink_url': (str,),  # noqa: E501
             'project_brief': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'created_from_template': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
@@ -156,15 +156,14 @@
         'created_from_template': 'created_from_template',  # noqa: E501
     }
 
     read_only_vars = {
         'custom_fields',  # noqa: E501
         'completed',  # noqa: E501
         'completed_at',  # noqa: E501
-        'completed_by',  # noqa: E501
         'followers',  # noqa: E501
         'permalink_url',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
@@ -202,15 +201,15 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             custom_fields ([CustomFieldCompact]): Array of Custom Fields.. [optional]  # noqa: E501
             completed (bool): True if the project is currently marked complete, false if not.. [optional]  # noqa: E501
             completed_at (datetime, none_type): The time at which this project was completed, or null if the project is not completed.. [optional]  # noqa: E501
-            completed_by (bool, date, datetime, dict, float, int, list, str, none_type): The user that marked this project complete, or null if the project is not completed.. [optional]  # noqa: E501
+            completed_by (UserCompact): [optional]  # noqa: E501
             followers ([UserCompact]): Array of users following this project. Followers are a subset of members who have opted in to receive \"tasks added\" notifications for a project.. [optional]  # noqa: E501
             owner (bool, date, datetime, dict, float, int, list, str, none_type): The current owner of the project, may be null.. [optional]  # noqa: E501
             team (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             icon (str, none_type): The icon for a project.. [optional]  # noqa: E501
             permalink_url (str): A url that points directly to the object within Asana.. [optional]  # noqa: E501
             project_brief (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             created_from_template (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
@@ -298,15 +297,15 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             custom_fields ([CustomFieldCompact]): Array of Custom Fields.. [optional]  # noqa: E501
             completed (bool): True if the project is currently marked complete, false if not.. [optional]  # noqa: E501
             completed_at (datetime, none_type): The time at which this project was completed, or null if the project is not completed.. [optional]  # noqa: E501
-            completed_by (bool, date, datetime, dict, float, int, list, str, none_type): The user that marked this project complete, or null if the project is not completed.. [optional]  # noqa: E501
+            completed_by (UserCompact): [optional]  # noqa: E501
             followers ([UserCompact]): Array of users following this project. Followers are a subset of members who have opted in to receive \"tasks added\" notifications for a project.. [optional]  # noqa: E501
             owner (bool, date, datetime, dict, float, int, list, str, none_type): The current owner of the project, may be null.. [optional]  # noqa: E501
             team (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             icon (str, none_type): The icon for a project.. [optional]  # noqa: E501
             permalink_url (str): A url that points directly to the object within Asana.. [optional]  # noqa: E501
             project_brief (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             created_from_template (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
```

### Comparing `asana-preview-1.0.4/asana_preview/model/project_status_base.py` & `asana-preview-1.0.5/asana_preview/model/project_status_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -94,15 +94,15 @@
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'text': (str,),  # noqa: E501
             'color': (str,),  # noqa: E501
             'gid': (str,),  # noqa: E501
-            'resource_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'resource_type': (str,),  # noqa: E501
             'title': (str,),  # noqa: E501
             'html_text': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
@@ -115,14 +115,15 @@
         'resource_type': 'resource_type',  # noqa: E501
         'title': 'title',  # noqa: E501
         'html_text': 'html_text',  # noqa: E501
     }
 
     read_only_vars = {
         'gid',  # noqa: E501
+        'resource_type',  # noqa: E501
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
         """ProjectStatusBase - a model defined in OpenAPI
 
@@ -156,17 +157,17 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
             title (str): The title of the project status update.. [optional]  # noqa: E501
-            html_text (str): [OptIn](/docs/inputoutput-options). The text content of the status update with formatting as HTML.. [optional]  # noqa: E501
+            html_text (str): [Opt In](/docs/inputoutput-options). The text content of the status update with formatting as HTML.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -265,17 +266,17 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
             title (str): The title of the project status update.. [optional]  # noqa: E501
-            html_text (str): [OptIn](/docs/inputoutput-options). The text content of the status update with formatting as HTML.. [optional]  # noqa: E501
+            html_text (str): [Opt In](/docs/inputoutput-options). The text content of the status update with formatting as HTML.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `asana-preview-1.0.4/asana_preview/model/project_status_base_all_of.py` & `asana-preview-1.0.5/asana_preview/model/project_status_base_all_of.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -85,27 +85,25 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'text': (str,),  # noqa: E501
             'color': (str,),  # noqa: E501
-            'resource_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'html_text': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'text': 'text',  # noqa: E501
         'color': 'color',  # noqa: E501
-        'resource_type': 'resource_type',  # noqa: E501
         'html_text': 'html_text',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
@@ -146,16 +144,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            html_text (str): [OptIn](/docs/inputoutput-options). The text content of the status update with formatting as HTML.. [optional]  # noqa: E501
+            html_text (str): [Opt In](/docs/inputoutput-options). The text content of the status update with formatting as HTML.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -239,16 +236,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            html_text (str): [OptIn](/docs/inputoutput-options). The text content of the status update with formatting as HTML.. [optional]  # noqa: E501
+            html_text (str): [Opt In](/docs/inputoutput-options). The text content of the status update with formatting as HTML.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `asana-preview-1.0.4/asana_preview/model/project_status_compact.py` & `asana-preview-1.0.5/asana_preview/model/project_status_compact.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -86,15 +86,15 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'gid': (str,),  # noqa: E501
-            'resource_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'resource_type': (str,),  # noqa: E501
             'title': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
@@ -103,14 +103,15 @@
         'gid': 'gid',  # noqa: E501
         'resource_type': 'resource_type',  # noqa: E501
         'title': 'title',  # noqa: E501
     }
 
     read_only_vars = {
         'gid',  # noqa: E501
+        'resource_type',  # noqa: E501
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
         """ProjectStatusCompact - a model defined in OpenAPI
 
@@ -142,15 +143,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
             title (str): The title of the project status update.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -248,15 +249,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
             title (str): The title of the project status update.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `asana-preview-1.0.4/asana_preview/model/project_status_compact_all_of.py` & `asana-preview-1.0.5/asana_preview/model/goal_relationship_base_all_of.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from asana_preview.exceptions import ApiAttributeError
 
 
 
-class ProjectStatusCompactAllOf(ModelNormal):
+class GoalRelationshipBaseAllOf(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -77,37 +77,35 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'resource_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
-            'title': (str,),  # noqa: E501
+            'supported_goal': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'resource_type': 'resource_type',  # noqa: E501
-        'title': 'title',  # noqa: E501
+        'supported_goal': 'supported_goal',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ProjectStatusCompactAllOf - a model defined in OpenAPI
+        """GoalRelationshipBaseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -132,16 +130,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            title (str): The title of the project status update.. [optional]  # noqa: E501
+            supported_goal (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -186,15 +183,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ProjectStatusCompactAllOf - a model defined in OpenAPI
+        """GoalRelationshipBaseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -219,16 +216,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            title (str): The title of the project status update.. [optional]  # noqa: E501
+            supported_goal (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `asana-preview-1.0.4/asana_preview/model/project_status_response.py` & `asana-preview-1.0.5/asana_preview/model/project_status_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -96,15 +96,15 @@
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'text': (str,),  # noqa: E501
             'color': (str,),  # noqa: E501
             'gid': (str,),  # noqa: E501
-            'resource_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'resource_type': (str,),  # noqa: E501
             'title': (str,),  # noqa: E501
             'html_text': (str,),  # noqa: E501
             'author': (UserCompact,),  # noqa: E501
             'created_at': (datetime,),  # noqa: E501
             'created_by': (UserCompact,),  # noqa: E501
             'modified_at': (datetime,),  # noqa: E501
         }
@@ -125,14 +125,15 @@
         'created_at': 'created_at',  # noqa: E501
         'created_by': 'created_by',  # noqa: E501
         'modified_at': 'modified_at',  # noqa: E501
     }
 
     read_only_vars = {
         'gid',  # noqa: E501
+        'resource_type',  # noqa: E501
         'created_at',  # noqa: E501
         'modified_at',  # noqa: E501
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
@@ -168,21 +169,21 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
             title (str): The title of the project status update.. [optional]  # noqa: E501
-            html_text (str): [OptIn](/docs/inputoutput-options). The text content of the status update with formatting as HTML.. [optional]  # noqa: E501
+            html_text (str): [Opt In](/docs/inputoutput-options). The text content of the status update with formatting as HTML.. [optional]  # noqa: E501
             author (UserCompact): [optional]  # noqa: E501
-            created_at (datetime): The time at which this project status was created.. [optional]  # noqa: E501
+            created_at (datetime): The time at which this resource was created.. [optional]  # noqa: E501
             created_by (UserCompact): [optional]  # noqa: E501
-            modified_at (datetime): The time at which this project status was last modified.  *Note: This does not currently reflect any changes in associations such as comments that may have been added or removed from the project status.*. [optional]  # noqa: E501
+            modified_at (datetime): The time at which this project status was last modified. *Note: This does not currently reflect any changes in associations such as comments that may have been added or removed from the project status.*. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -281,21 +282,21 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
             title (str): The title of the project status update.. [optional]  # noqa: E501
-            html_text (str): [OptIn](/docs/inputoutput-options). The text content of the status update with formatting as HTML.. [optional]  # noqa: E501
+            html_text (str): [Opt In](/docs/inputoutput-options). The text content of the status update with formatting as HTML.. [optional]  # noqa: E501
             author (UserCompact): [optional]  # noqa: E501
-            created_at (datetime): The time at which this project status was created.. [optional]  # noqa: E501
+            created_at (datetime): The time at which this resource was created.. [optional]  # noqa: E501
             created_by (UserCompact): [optional]  # noqa: E501
-            modified_at (datetime): The time at which this project status was last modified.  *Note: This does not currently reflect any changes in associations such as comments that may have been added or removed from the project status.*. [optional]  # noqa: E501
+            modified_at (datetime): The time at which this project status was last modified. *Note: This does not currently reflect any changes in associations such as comments that may have been added or removed from the project status.*. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `asana-preview-1.0.4/asana_preview/model/project_status_response_all_of.py` & `asana-preview-1.0.5/asana_preview/model/project_status_response_all_of.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -145,17 +145,17 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             author (UserCompact): [optional]  # noqa: E501
-            created_at (datetime): The time at which this project status was created.. [optional]  # noqa: E501
+            created_at (datetime): The time at which this resource was created.. [optional]  # noqa: E501
             created_by (UserCompact): [optional]  # noqa: E501
-            modified_at (datetime): The time at which this project status was last modified.  *Note: This does not currently reflect any changes in associations such as comments that may have been added or removed from the project status.*. [optional]  # noqa: E501
+            modified_at (datetime): The time at which this project status was last modified. *Note: This does not currently reflect any changes in associations such as comments that may have been added or removed from the project status.*. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -234,17 +234,17 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             author (UserCompact): [optional]  # noqa: E501
-            created_at (datetime): The time at which this project status was created.. [optional]  # noqa: E501
+            created_at (datetime): The time at which this resource was created.. [optional]  # noqa: E501
             created_by (UserCompact): [optional]  # noqa: E501
-            modified_at (datetime): The time at which this project status was last modified.  *Note: This does not currently reflect any changes in associations such as comments that may have been added or removed from the project status.*. [optional]  # noqa: E501
+            modified_at (datetime): The time at which this project status was last modified. *Note: This does not currently reflect any changes in associations such as comments that may have been added or removed from the project status.*. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `asana-preview-1.0.4/asana_preview/model/project_template_compact.py` & `asana-preview-1.0.5/asana_preview/model/project_template_compact.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -86,15 +86,15 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'gid': (str,),  # noqa: E501
-            'resource_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'resource_type': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
@@ -103,14 +103,15 @@
         'gid': 'gid',  # noqa: E501
         'resource_type': 'resource_type',  # noqa: E501
         'name': 'name',  # noqa: E501
     }
 
     read_only_vars = {
         'gid',  # noqa: E501
+        'resource_type',  # noqa: E501
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
         """ProjectTemplateCompact - a model defined in OpenAPI
 
@@ -142,15 +143,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
             name (str): Name of the project template.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -248,15 +249,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
             name (str): Name of the project template.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `asana-preview-1.0.4/asana_preview/model/project_template_compact_all_of.py` & `asana-preview-1.0.5/asana_preview/model/goal_compact_all_of.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from asana_preview.exceptions import ApiAttributeError
 
 
 
-class ProjectTemplateCompactAllOf(ModelNormal):
+class GoalCompactAllOf(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -77,37 +77,37 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'resource_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'name': (str,),  # noqa: E501
+            'owner': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'resource_type': 'resource_type',  # noqa: E501
         'name': 'name',  # noqa: E501
+        'owner': 'owner',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ProjectTemplateCompactAllOf - a model defined in OpenAPI
+        """GoalCompactAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -132,16 +132,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            name (str): Name of the project template.. [optional]  # noqa: E501
+            name (str): The name of the goal.. [optional]  # noqa: E501
+            owner (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -186,15 +186,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ProjectTemplateCompactAllOf - a model defined in OpenAPI
+        """GoalCompactAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -219,16 +219,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            name (str): Name of the project template.. [optional]  # noqa: E501
+            name (str): The name of the goal.. [optional]  # noqa: E501
+            owner (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `asana-preview-1.0.4/asana_preview/model/section_compact.py` & `asana-preview-1.0.5/asana_preview/model/tag_compact.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -27,20 +27,20 @@
     OpenApiModel
 )
 from asana_preview.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from asana_preview.model.asana_resource import AsanaResource
-    from asana_preview.model.section_compact_all_of import SectionCompactAllOf
+    from asana_preview.model.tag_compact_all_of import TagCompactAllOf
     globals()['AsanaResource'] = AsanaResource
-    globals()['SectionCompactAllOf'] = SectionCompactAllOf
+    globals()['TagCompactAllOf'] = TagCompactAllOf
 
 
-class SectionCompact(ModelComposed):
+class TagCompact(ModelComposed):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -86,15 +86,15 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'gid': (str,),  # noqa: E501
-            'resource_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'resource_type': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
@@ -103,20 +103,21 @@
         'gid': 'gid',  # noqa: E501
         'resource_type': 'resource_type',  # noqa: E501
         'name': 'name',  # noqa: E501
     }
 
     read_only_vars = {
         'gid',  # noqa: E501
+        'resource_type',  # noqa: E501
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """SectionCompact - a model defined in OpenAPI
+        """TagCompact - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -142,16 +143,16 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            name (str): The name of the section (i.e. the text displayed as the section header).. [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
+            name (str): Name of the tag. This is generally a short sentence fragment that fits on a line in the UI for maximum readability. However, it can be longer.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -214,15 +215,15 @@
         '_composed_instances',
         '_var_name_to_model_instances',
         '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """SectionCompact - a model defined in OpenAPI
+        """TagCompact - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -248,16 +249,16 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            name (str): The name of the section (i.e. the text displayed as the section header).. [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
+            name (str): Name of the tag. This is generally a short sentence fragment that fits on a line in the UI for maximum readability. However, it can be longer.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -320,12 +321,12 @@
         # loading
         lazy_import()
         return {
           'anyOf': [
           ],
           'allOf': [
               AsanaResource,
-              SectionCompactAllOf,
+              TagCompactAllOf,
           ],
           'oneOf': [
           ],
         }
```

### Comparing `asana-preview-1.0.4/asana_preview/model/section_compact_all_of.py` & `asana-preview-1.0.5/asana_preview/model/create_membership_request_all_of.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from asana_preview.exceptions import ApiAttributeError
 
 
 
-class SectionCompactAllOf(ModelNormal):
+class CreateMembershipRequestAllOf(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -77,37 +77,37 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'resource_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
-            'name': (str,),  # noqa: E501
+            'member': (str,),  # noqa: E501
+            'parent': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'resource_type': 'resource_type',  # noqa: E501
-        'name': 'name',  # noqa: E501
+        'member': 'member',  # noqa: E501
+        'parent': 'parent',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """SectionCompactAllOf - a model defined in OpenAPI
+        """CreateMembershipRequestAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -132,16 +132,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            name (str): The name of the section (i.e. the text displayed as the section header).. [optional]  # noqa: E501
+            member (str): The gid of the user or team. [optional]  # noqa: E501
+            parent (str): The gid of the `portfolio`, `team`, `project`, or `goal`. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -186,15 +186,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """SectionCompactAllOf - a model defined in OpenAPI
+        """CreateMembershipRequestAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -219,16 +219,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            name (str): The name of the section (i.e. the text displayed as the section header).. [optional]  # noqa: E501
+            member (str): The gid of the user or team. [optional]  # noqa: E501
+            parent (str): The gid of the `portfolio`, `team`, `project`, or `goal`. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `asana-preview-1.0.4/asana_preview/model/status_update_compact.py` & `asana-preview-1.0.5/asana_preview/model/status_update_compact.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -91,15 +91,15 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'gid': (str,),  # noqa: E501
-            'resource_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'resource_type': (str,),  # noqa: E501
             'title': (str,),  # noqa: E501
             'resource_subtype': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
@@ -110,14 +110,15 @@
         'resource_type': 'resource_type',  # noqa: E501
         'title': 'title',  # noqa: E501
         'resource_subtype': 'resource_subtype',  # noqa: E501
     }
 
     read_only_vars = {
         'gid',  # noqa: E501
+        'resource_type',  # noqa: E501
         'resource_subtype',  # noqa: E501
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
         """StatusUpdateCompact - a model defined in OpenAPI
@@ -150,15 +151,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
             title (str): The title of the status update.. [optional]  # noqa: E501
             resource_subtype (str): The subtype of this resource. Different subtypes retain many of the same fields and behavior, but may render differently in Asana or represent resources with different semantic meaning. The `resource_subtype`s for `status` objects represent the type of their parent.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
@@ -257,15 +258,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
             title (str): The title of the status update.. [optional]  # noqa: E501
             resource_subtype (str): The subtype of this resource. Different subtypes retain many of the same fields and behavior, but may render differently in Asana or represent resources with different semantic meaning. The `resource_subtype`s for `status` objects represent the type of their parent.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
```

### Comparing `asana-preview-1.0.4/asana_preview/model/status_update_compact_all_of.py` & `asana-preview-1.0.5/asana_preview/model/goal_relationship_compact_all_of.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from asana_preview.exceptions import ApiAttributeError
 
 
 
-class StatusUpdateCompactAllOf(ModelNormal):
+class GoalRelationshipCompactAllOf(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -52,17 +52,16 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('resource_subtype',): {
-            'PROJECT_STATUS_UPDATE': "project_status_update",
-            'PORTFOLIO_STATUS_UPDATE': "portfolio_status_update",
-            'GOAL_STATUS_UPDATE': "goal_status_update",
+            'SUBGOAL': "subgoal",
+            'SUPPORTING_WORK': "supporting_work",
         },
     }
 
     validations = {
     }
 
     @cached_property
@@ -82,40 +81,40 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'resource_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
-            'title': (str,),  # noqa: E501
             'resource_subtype': (str,),  # noqa: E501
+            'supporting_resource': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'contribution_weight': (float,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'resource_type': 'resource_type',  # noqa: E501
-        'title': 'title',  # noqa: E501
         'resource_subtype': 'resource_subtype',  # noqa: E501
+        'supporting_resource': 'supporting_resource',  # noqa: E501
+        'contribution_weight': 'contribution_weight',  # noqa: E501
     }
 
     read_only_vars = {
         'resource_subtype',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """StatusUpdateCompactAllOf - a model defined in OpenAPI
+        """GoalRelationshipCompactAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -140,17 +139,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            title (str): The title of the status update.. [optional]  # noqa: E501
-            resource_subtype (str): The subtype of this resource. Different subtypes retain many of the same fields and behavior, but may render differently in Asana or represent resources with different semantic meaning. The `resource_subtype`s for `status` objects represent the type of their parent.. [optional]  # noqa: E501
+            resource_subtype (str): The subtype of this resource. Different subtypes retain many of the same fields and behavior, but may render differently in Asana or represent resources with different semantic meaning.. [optional]  # noqa: E501
+            supporting_resource (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            contribution_weight (float): The weight that the supporting resource's progress contributes to the supported goal's progress. This can only be 0 or 1.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -195,15 +194,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """StatusUpdateCompactAllOf - a model defined in OpenAPI
+        """GoalRelationshipCompactAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -228,17 +227,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            title (str): The title of the status update.. [optional]  # noqa: E501
-            resource_subtype (str): The subtype of this resource. Different subtypes retain many of the same fields and behavior, but may render differently in Asana or represent resources with different semantic meaning. The `resource_subtype`s for `status` objects represent the type of their parent.. [optional]  # noqa: E501
+            resource_subtype (str): The subtype of this resource. Different subtypes retain many of the same fields and behavior, but may render differently in Asana or represent resources with different semantic meaning.. [optional]  # noqa: E501
+            supporting_resource (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            contribution_weight (float): The weight that the supporting resource's progress contributes to the supported goal's progress. This can only be 0 or 1.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `asana-preview-1.0.4/asana_preview/model/story_compact.py` & `asana-preview-1.0.5/asana_preview/model/story_compact.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -88,15 +88,15 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'gid': (str,),  # noqa: E501
-            'resource_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'resource_type': (str,),  # noqa: E501
             'created_at': (datetime,),  # noqa: E501
             'created_by': (UserCompact,),  # noqa: E501
             'resource_subtype': (str,),  # noqa: E501
             'text': (str,),  # noqa: E501
         }
 
     @cached_property
@@ -111,14 +111,15 @@
         'created_by': 'created_by',  # noqa: E501
         'resource_subtype': 'resource_subtype',  # noqa: E501
         'text': 'text',  # noqa: E501
     }
 
     read_only_vars = {
         'gid',  # noqa: E501
+        'resource_type',  # noqa: E501
         'created_at',  # noqa: E501
         'resource_subtype',  # noqa: E501
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
@@ -152,16 +153,16 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            created_at (datetime): The time at which the story was created.. [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
+            created_at (datetime): The time at which this resource was created.. [optional]  # noqa: E501
             created_by (UserCompact): [optional]  # noqa: E501
             resource_subtype (str): The subtype of this resource. Different subtypes retain many of the same fields and behavior, but may render differently in Asana or represent resources with different semantic meaning.. [optional]  # noqa: E501
             text (str): *Create-only*. Human-readable text for the story or comment. This will not include the name of the creator. *Note: This is not guaranteed to be stable for a given type of story. For example, text for a reassignment may not always say “assigned to …” as the text for a story can both be edited and change based on the language settings of the user making the request.* Use the `resource_subtype` property to discover the action that created the story.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
@@ -261,16 +262,16 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            created_at (datetime): The time at which the story was created.. [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
+            created_at (datetime): The time at which this resource was created.. [optional]  # noqa: E501
             created_by (UserCompact): [optional]  # noqa: E501
             resource_subtype (str): The subtype of this resource. Different subtypes retain many of the same fields and behavior, but may render differently in Asana or represent resources with different semantic meaning.. [optional]  # noqa: E501
             text (str): *Create-only*. Human-readable text for the story or comment. This will not include the name of the creator. *Note: This is not guaranteed to be stable for a given type of story. For example, text for a reassignment may not always say “assigned to …” as the text for a story can both be edited and change based on the language settings of the user making the request.* Use the `resource_subtype` property to discover the action that created the story.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
```

### Comparing `asana-preview-1.0.4/asana_preview/model/story_compact_all_of.py` & `asana-preview-1.0.5/asana_preview/model/story_compact_all_of.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -83,28 +83,26 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'resource_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'created_at': (datetime,),  # noqa: E501
             'created_by': (UserCompact,),  # noqa: E501
             'resource_subtype': (str,),  # noqa: E501
             'text': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'resource_type': 'resource_type',  # noqa: E501
         'created_at': 'created_at',  # noqa: E501
         'created_by': 'created_by',  # noqa: E501
         'resource_subtype': 'resource_subtype',  # noqa: E501
         'text': 'text',  # noqa: E501
     }
 
     read_only_vars = {
@@ -146,16 +144,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            created_at (datetime): The time at which the story was created.. [optional]  # noqa: E501
+            created_at (datetime): The time at which this resource was created.. [optional]  # noqa: E501
             created_by (UserCompact): [optional]  # noqa: E501
             resource_subtype (str): The subtype of this resource. Different subtypes retain many of the same fields and behavior, but may render differently in Asana or represent resources with different semantic meaning.. [optional]  # noqa: E501
             text (str): *Create-only*. Human-readable text for the story or comment. This will not include the name of the creator. *Note: This is not guaranteed to be stable for a given type of story. For example, text for a reassignment may not always say “assigned to …” as the text for a story can both be edited and change based on the language settings of the user making the request.* Use the `resource_subtype` property to discover the action that created the story.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
@@ -236,16 +233,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            created_at (datetime): The time at which the story was created.. [optional]  # noqa: E501
+            created_at (datetime): The time at which this resource was created.. [optional]  # noqa: E501
             created_by (UserCompact): [optional]  # noqa: E501
             resource_subtype (str): The subtype of this resource. Different subtypes retain many of the same fields and behavior, but may render differently in Asana or represent resources with different semantic meaning.. [optional]  # noqa: E501
             text (str): *Create-only*. Human-readable text for the story or comment. This will not include the name of the creator. *Note: This is not guaranteed to be stable for a given type of story. For example, text for a reassignment may not always say “assigned to …” as the text for a story can both be edited and change based on the language settings of the user making the request.* Use the `resource_subtype` property to discover the action that created the story.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
```

### Comparing `asana-preview-1.0.4/asana_preview/model/tag_compact.py` & `asana-preview-1.0.5/asana_preview/model/goal_compact.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -27,20 +27,20 @@
     OpenApiModel
 )
 from asana_preview.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from asana_preview.model.asana_resource import AsanaResource
-    from asana_preview.model.tag_compact_all_of import TagCompactAllOf
+    from asana_preview.model.goal_compact_all_of import GoalCompactAllOf
     globals()['AsanaResource'] = AsanaResource
-    globals()['TagCompactAllOf'] = TagCompactAllOf
+    globals()['GoalCompactAllOf'] = GoalCompactAllOf
 
 
-class TagCompact(ModelComposed):
+class GoalCompact(ModelComposed):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -86,37 +86,40 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'gid': (str,),  # noqa: E501
-            'resource_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'resource_type': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
+            'owner': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'gid': 'gid',  # noqa: E501
         'resource_type': 'resource_type',  # noqa: E501
         'name': 'name',  # noqa: E501
+        'owner': 'owner',  # noqa: E501
     }
 
     read_only_vars = {
         'gid',  # noqa: E501
+        'resource_type',  # noqa: E501
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TagCompact - a model defined in OpenAPI
+        """GoalCompact - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -142,16 +145,17 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            name (str): Name of the tag. This is generally a short sentence fragment that fits on a line in the UI for maximum readability. However, it can be longer.. [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
+            name (str): The name of the goal.. [optional]  # noqa: E501
+            owner (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -214,15 +218,15 @@
         '_composed_instances',
         '_var_name_to_model_instances',
         '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TagCompact - a model defined in OpenAPI
+        """GoalCompact - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -248,16 +252,17 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            name (str): Name of the tag. This is generally a short sentence fragment that fits on a line in the UI for maximum readability. However, it can be longer.. [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
+            name (str): The name of the goal.. [optional]  # noqa: E501
+            owner (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -320,12 +325,12 @@
         # loading
         lazy_import()
         return {
           'anyOf': [
           ],
           'allOf': [
               AsanaResource,
-              TagCompactAllOf,
+              GoalCompactAllOf,
           ],
           'oneOf': [
           ],
         }
```

### Comparing `asana-preview-1.0.4/asana_preview/model/tag_compact_all_of.py` & `asana-preview-1.0.5/asana_preview/model/get_project_memberships_for_project200_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -25,16 +25,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from asana_preview.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from asana_preview.model.project_membership_compact import ProjectMembershipCompact
+    globals()['ProjectMembershipCompact'] = ProjectMembershipCompact
 
-class TagCompactAllOf(ModelNormal):
+
+class GetProjectMembershipsForProject200Response(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -62,52 +66,52 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'resource_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
-            'name': (str,),  # noqa: E501
+            'data': ([ProjectMembershipCompact],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'resource_type': 'resource_type',  # noqa: E501
-        'name': 'name',  # noqa: E501
+        'data': 'data',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TagCompactAllOf - a model defined in OpenAPI
+        """GetProjectMembershipsForProject200Response - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -132,16 +136,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            name (str): Name of the tag. This is generally a short sentence fragment that fits on a line in the UI for maximum readability. However, it can be longer.. [optional]  # noqa: E501
+            data ([ProjectMembershipCompact]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -186,15 +189,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TagCompactAllOf - a model defined in OpenAPI
+        """GetProjectMembershipsForProject200Response - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -219,16 +222,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            name (str): Name of the tag. This is generally a short sentence fragment that fits on a line in the UI for maximum readability. However, it can be longer.. [optional]  # noqa: E501
+            data ([ProjectMembershipCompact]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `asana-preview-1.0.4/asana_preview/model/task_base.py` & `asana-preview-1.0.5/asana_preview/model/goal_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,23 +26,25 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from asana_preview.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from asana_preview.model.task_base_all_of import TaskBaseAllOf
-    from asana_preview.model.task_base_all_of_external import TaskBaseAllOfExternal
-    from asana_preview.model.task_compact import TaskCompact
-    globals()['TaskBaseAllOf'] = TaskBaseAllOf
-    globals()['TaskBaseAllOfExternal'] = TaskBaseAllOfExternal
-    globals()['TaskCompact'] = TaskCompact
+    from asana_preview.model.goal_base import GoalBase
+    from asana_preview.model.goal_response_all_of import GoalResponseAllOf
+    from asana_preview.model.like import Like
+    from asana_preview.model.user_compact import UserCompact
+    globals()['GoalBase'] = GoalBase
+    globals()['GoalResponseAllOf'] = GoalResponseAllOf
+    globals()['Like'] = Like
+    globals()['UserCompact'] = UserCompact
 
 
-class TaskBase(ModelComposed):
+class GoalResponse(ModelComposed):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -59,33 +61,14 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('resource_subtype',): {
-            'DEFAULT_TASK': "default_task",
-            'MILESTONE': "milestone",
-            'SECTION': "section",
-            'APPROVAL': "approval",
-        },
-        ('approval_status',): {
-            'PENDING': "pending",
-            'APPROVED': "approved",
-            'REJECTED': "rejected",
-            'CHANGES_REQUESTED': "changes_requested",
-        },
-        ('assignee_status',): {
-            'TODAY': "today",
-            'UPCOMING': "upcoming",
-            'LATER': "later",
-            'NEW': "new",
-            'INBOX': "inbox",
-        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
@@ -107,61 +90,72 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'gid': (str,),  # noqa: E501
-            'resource_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'resource_type': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
-            'resource_subtype': (str,),  # noqa: E501
-            'approval_status': (str,),  # noqa: E501
-            'assignee_status': (str,),  # noqa: E501
-            'completed': (bool,),  # noqa: E501
-            'due_at': (datetime, none_type,),  # noqa: E501
-            'due_on': (date, none_type,),  # noqa: E501
-            'external': (TaskBaseAllOfExternal,),  # noqa: E501
             'html_notes': (str,),  # noqa: E501
-            'liked': (bool,),  # noqa: E501
             'notes': (str,),  # noqa: E501
-            'start_at': (datetime, none_type,),  # noqa: E501
-            'start_on': (date, none_type,),  # noqa: E501
+            'due_on': (str, none_type,),  # noqa: E501
+            'start_on': (str, none_type,),  # noqa: E501
+            'status': (str, none_type,),  # noqa: E501
+            'is_workspace_level': (bool,),  # noqa: E501
+            'liked': (bool,),  # noqa: E501
+            'likes': ([Like],),  # noqa: E501
+            'num_likes': (int,),  # noqa: E501
+            'team': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'workspace': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'followers': ([UserCompact],),  # noqa: E501
+            'time_period': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'metric': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'owner': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'current_status_update': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'gid': 'gid',  # noqa: E501
         'resource_type': 'resource_type',  # noqa: E501
         'name': 'name',  # noqa: E501
-        'resource_subtype': 'resource_subtype',  # noqa: E501
-        'approval_status': 'approval_status',  # noqa: E501
-        'assignee_status': 'assignee_status',  # noqa: E501
-        'completed': 'completed',  # noqa: E501
-        'due_at': 'due_at',  # noqa: E501
-        'due_on': 'due_on',  # noqa: E501
-        'external': 'external',  # noqa: E501
         'html_notes': 'html_notes',  # noqa: E501
-        'liked': 'liked',  # noqa: E501
         'notes': 'notes',  # noqa: E501
-        'start_at': 'start_at',  # noqa: E501
+        'due_on': 'due_on',  # noqa: E501
         'start_on': 'start_on',  # noqa: E501
+        'status': 'status',  # noqa: E501
+        'is_workspace_level': 'is_workspace_level',  # noqa: E501
+        'liked': 'liked',  # noqa: E501
+        'likes': 'likes',  # noqa: E501
+        'num_likes': 'num_likes',  # noqa: E501
+        'team': 'team',  # noqa: E501
+        'workspace': 'workspace',  # noqa: E501
+        'followers': 'followers',  # noqa: E501
+        'time_period': 'time_period',  # noqa: E501
+        'metric': 'metric',  # noqa: E501
+        'owner': 'owner',  # noqa: E501
+        'current_status_update': 'current_status_update',  # noqa: E501
     }
 
     read_only_vars = {
         'gid',  # noqa: E501
+        'resource_type',  # noqa: E501
+        'likes',  # noqa: E501
+        'num_likes',  # noqa: E501
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TaskBase - a model defined in OpenAPI
+        """GoalResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -187,28 +181,32 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            name (str): Name of the task. This is generally a short sentence fragment that fits on a line in the UI for maximum readability. However, it can be longer.. [optional]  # noqa: E501
-            resource_subtype (str): The subtype of this resource. Different subtypes retain many of the same fields and behavior, but may render differently in Asana or represent resources with different semantic meaning.  The resource_subtype `milestone` represent a single moment in time. This means tasks with this subtype cannot have a start_date.. [optional]  # noqa: E501
-            approval_status (str): *Conditional* Reflects the approval status of this task. This field is kept in sync with `completed`, meaning `pending` translates to false while `approved`, `rejected`, and `changes_requested` translate to true. If you set completed to true, this field will be set to `approved`.. [optional]  # noqa: E501
-            assignee_status (str): *Deprecated* Scheduling status of this task for the user it is assigned to. This field can only be set if the assignee is non-null. Setting this field to \"inbox\" or \"upcoming\" inserts it at the top of the section, while the other options will insert at the bottom.. [optional]  # noqa: E501
-            completed (bool): True if the task is currently marked complete, false if not.. [optional]  # noqa: E501
-            due_at (datetime, none_type): The UTC date and time on which this task is due, or null if the task has no due time. This takes an ISO 8601 date string in UTC and should not be used together with `due_on`.. [optional]  # noqa: E501
-            due_on (date, none_type): The localized date on which this task is due, or null if the task has no due date. This takes a date with `YYYY-MM-DD` format and should not be used together with `due_at`.. [optional]  # noqa: E501
-            external (TaskBaseAllOfExternal): [optional]  # noqa: E501
-            html_notes (str): [Opt In](/docs/inputoutput-options). The notes of the text with formatting as HTML.. [optional]  # noqa: E501
-            liked (bool): True if the task is liked by the authorized user, false if not.. [optional]  # noqa: E501
-            notes (str): Free-form textual information associated with the task (i.e. its description).. [optional]  # noqa: E501
-            start_at (datetime, none_type): Date and time on which work begins for the task, or null if the task has no start time. This takes an ISO 8601 date string in UTC and should not be used together with `start_on`. *Note: `due_at` must be present in the request when setting or unsetting the `start_at` parameter.*. [optional]  # noqa: E501
-            start_on (date, none_type): The day on which work begins for the task , or null if the task has no start date. This takes a date with `YYYY-MM-DD` format and should not be used together with `start_at`. *Note: `due_on` or `due_at` must be present in the request when setting or unsetting the `start_on` parameter.*. [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
+            name (str): The name of the goal.. [optional]  # noqa: E501
+            html_notes (str): The notes of the goal with formatting as HTML.. [optional]  # noqa: E501
+            notes (str): Free-form textual information associated with the goal (i.e. its description).. [optional]  # noqa: E501
+            due_on (str, none_type): The localized day on which this goal is due. This takes a date with format `YYYY-MM-DD`.. [optional]  # noqa: E501
+            start_on (str, none_type): The day on which work for this goal begins, or null if the goal has no start date. This takes a date with `YYYY-MM-DD` format, and cannot be set unless there is an accompanying due date.. [optional]  # noqa: E501
+            status (str, none_type): The current status of this goal. When the goal is open, its status can be `green`, `yellow`, and `red` to reflect \"On Track\", \"At Risk\", and \"Off Track\", respectively. When the goal is closed, the value can be `missed`, `achieved`, `partial`, or `dropped`. *Note* you can only write to this property if `metric` is set.. [optional]  # noqa: E501
+            is_workspace_level (bool): *Conditional*. This property is only present when the `workspace` provided is an organization. Whether the goal belongs to the `workspace` (and is listed as part of the workspace’s goals) or not. If it isn’t a workspace-level goal, it is a team-level goal, and is associated with the goal’s team.. [optional]  # noqa: E501
+            liked (bool): True if the goal is liked by the authorized user, false if not.. [optional]  # noqa: E501
+            likes ([Like]): Array of likes for users who have liked this goal.. [optional]  # noqa: E501
+            num_likes (int): The number of users who have liked this goal.. [optional]  # noqa: E501
+            team (bool, date, datetime, dict, float, int, list, str, none_type): *Conditional*. This property is only present when the `workspace` provided is an organization.. [optional]  # noqa: E501
+            workspace (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            followers ([UserCompact]): Array of users who are members of this goal.. [optional]  # noqa: E501
+            time_period (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            metric (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            owner (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            current_status_update (bool, date, datetime, dict, float, int, list, str, none_type): The latest `status_update` posted to this goal.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -271,15 +269,15 @@
         '_composed_instances',
         '_var_name_to_model_instances',
         '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TaskBase - a model defined in OpenAPI
+        """GoalResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -305,28 +303,32 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            name (str): Name of the task. This is generally a short sentence fragment that fits on a line in the UI for maximum readability. However, it can be longer.. [optional]  # noqa: E501
-            resource_subtype (str): The subtype of this resource. Different subtypes retain many of the same fields and behavior, but may render differently in Asana or represent resources with different semantic meaning.  The resource_subtype `milestone` represent a single moment in time. This means tasks with this subtype cannot have a start_date.. [optional]  # noqa: E501
-            approval_status (str): *Conditional* Reflects the approval status of this task. This field is kept in sync with `completed`, meaning `pending` translates to false while `approved`, `rejected`, and `changes_requested` translate to true. If you set completed to true, this field will be set to `approved`.. [optional]  # noqa: E501
-            assignee_status (str): *Deprecated* Scheduling status of this task for the user it is assigned to. This field can only be set if the assignee is non-null. Setting this field to \"inbox\" or \"upcoming\" inserts it at the top of the section, while the other options will insert at the bottom.. [optional]  # noqa: E501
-            completed (bool): True if the task is currently marked complete, false if not.. [optional]  # noqa: E501
-            due_at (datetime, none_type): The UTC date and time on which this task is due, or null if the task has no due time. This takes an ISO 8601 date string in UTC and should not be used together with `due_on`.. [optional]  # noqa: E501
-            due_on (date, none_type): The localized date on which this task is due, or null if the task has no due date. This takes a date with `YYYY-MM-DD` format and should not be used together with `due_at`.. [optional]  # noqa: E501
-            external (TaskBaseAllOfExternal): [optional]  # noqa: E501
-            html_notes (str): [Opt In](/docs/inputoutput-options). The notes of the text with formatting as HTML.. [optional]  # noqa: E501
-            liked (bool): True if the task is liked by the authorized user, false if not.. [optional]  # noqa: E501
-            notes (str): Free-form textual information associated with the task (i.e. its description).. [optional]  # noqa: E501
-            start_at (datetime, none_type): Date and time on which work begins for the task, or null if the task has no start time. This takes an ISO 8601 date string in UTC and should not be used together with `start_on`. *Note: `due_at` must be present in the request when setting or unsetting the `start_at` parameter.*. [optional]  # noqa: E501
-            start_on (date, none_type): The day on which work begins for the task , or null if the task has no start date. This takes a date with `YYYY-MM-DD` format and should not be used together with `start_at`. *Note: `due_on` or `due_at` must be present in the request when setting or unsetting the `start_on` parameter.*. [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
+            name (str): The name of the goal.. [optional]  # noqa: E501
+            html_notes (str): The notes of the goal with formatting as HTML.. [optional]  # noqa: E501
+            notes (str): Free-form textual information associated with the goal (i.e. its description).. [optional]  # noqa: E501
+            due_on (str, none_type): The localized day on which this goal is due. This takes a date with format `YYYY-MM-DD`.. [optional]  # noqa: E501
+            start_on (str, none_type): The day on which work for this goal begins, or null if the goal has no start date. This takes a date with `YYYY-MM-DD` format, and cannot be set unless there is an accompanying due date.. [optional]  # noqa: E501
+            status (str, none_type): The current status of this goal. When the goal is open, its status can be `green`, `yellow`, and `red` to reflect \"On Track\", \"At Risk\", and \"Off Track\", respectively. When the goal is closed, the value can be `missed`, `achieved`, `partial`, or `dropped`. *Note* you can only write to this property if `metric` is set.. [optional]  # noqa: E501
+            is_workspace_level (bool): *Conditional*. This property is only present when the `workspace` provided is an organization. Whether the goal belongs to the `workspace` (and is listed as part of the workspace’s goals) or not. If it isn’t a workspace-level goal, it is a team-level goal, and is associated with the goal’s team.. [optional]  # noqa: E501
+            liked (bool): True if the goal is liked by the authorized user, false if not.. [optional]  # noqa: E501
+            likes ([Like]): Array of likes for users who have liked this goal.. [optional]  # noqa: E501
+            num_likes (int): The number of users who have liked this goal.. [optional]  # noqa: E501
+            team (bool, date, datetime, dict, float, int, list, str, none_type): *Conditional*. This property is only present when the `workspace` provided is an organization.. [optional]  # noqa: E501
+            workspace (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            followers ([UserCompact]): Array of users who are members of this goal.. [optional]  # noqa: E501
+            time_period (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            metric (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            owner (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            current_status_update (bool, date, datetime, dict, float, int, list, str, none_type): The latest `status_update` posted to this goal.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -388,13 +390,13 @@
         # classes don't exist yet because their module has not finished
         # loading
         lazy_import()
         return {
           'anyOf': [
           ],
           'allOf': [
-              TaskBaseAllOf,
-              TaskCompact,
+              GoalBase,
+              GoalResponseAllOf,
           ],
           'oneOf': [
           ],
         }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `asana-preview-1.0.4/asana_preview/model/task_base_all_of.py` & `asana-preview-1.0.5/asana_preview/model/goal_base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,19 +26,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from asana_preview.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from asana_preview.model.task_base_all_of_external import TaskBaseAllOfExternal
-    globals()['TaskBaseAllOfExternal'] = TaskBaseAllOfExternal
+    from asana_preview.model.asana_resource import AsanaResource
+    from asana_preview.model.goal_base_all_of import GoalBaseAllOf
+    globals()['AsanaResource'] = AsanaResource
+    globals()['GoalBaseAllOf'] = GoalBaseAllOf
 
 
-class TaskBaseAllOf(ModelNormal):
+class GoalBase(ModelComposed):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -55,27 +57,14 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('approval_status',): {
-            'PENDING': "pending",
-            'APPROVED': "approved",
-            'REJECTED': "rejected",
-            'CHANGES_REQUESTED': "changes_requested",
-        },
-        ('assignee_status',): {
-            'TODAY': "today",
-            'UPCOMING': "upcoming",
-            'LATER': "later",
-            'NEW': "new",
-            'INBOX': "inbox",
-        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
@@ -96,57 +85,53 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'approval_status': (str,),  # noqa: E501
-            'assignee_status': (str,),  # noqa: E501
-            'completed': (bool,),  # noqa: E501
-            'due_at': (datetime, none_type,),  # noqa: E501
-            'due_on': (date, none_type,),  # noqa: E501
-            'external': (TaskBaseAllOfExternal,),  # noqa: E501
-            'html_notes': (str,),  # noqa: E501
-            'liked': (bool,),  # noqa: E501
+            'gid': (str,),  # noqa: E501
+            'resource_type': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
+            'html_notes': (str,),  # noqa: E501
             'notes': (str,),  # noqa: E501
-            'start_at': (datetime, none_type,),  # noqa: E501
-            'start_on': (date, none_type,),  # noqa: E501
+            'due_on': (str, none_type,),  # noqa: E501
+            'start_on': (str, none_type,),  # noqa: E501
+            'status': (str, none_type,),  # noqa: E501
+            'is_workspace_level': (bool,),  # noqa: E501
+            'liked': (bool,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'approval_status': 'approval_status',  # noqa: E501
-        'assignee_status': 'assignee_status',  # noqa: E501
-        'completed': 'completed',  # noqa: E501
-        'due_at': 'due_at',  # noqa: E501
-        'due_on': 'due_on',  # noqa: E501
-        'external': 'external',  # noqa: E501
-        'html_notes': 'html_notes',  # noqa: E501
-        'liked': 'liked',  # noqa: E501
+        'gid': 'gid',  # noqa: E501
+        'resource_type': 'resource_type',  # noqa: E501
         'name': 'name',  # noqa: E501
+        'html_notes': 'html_notes',  # noqa: E501
         'notes': 'notes',  # noqa: E501
-        'start_at': 'start_at',  # noqa: E501
+        'due_on': 'due_on',  # noqa: E501
         'start_on': 'start_on',  # noqa: E501
+        'status': 'status',  # noqa: E501
+        'is_workspace_level': 'is_workspace_level',  # noqa: E501
+        'liked': 'liked',  # noqa: E501
     }
 
     read_only_vars = {
+        'gid',  # noqa: E501
+        'resource_type',  # noqa: E501
     }
 
-    _composed_schemas = {}
-
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TaskBaseAllOf - a model defined in OpenAPI
+        """GoalBase - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -171,30 +156,28 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            approval_status (str): *Conditional* Reflects the approval status of this task. This field is kept in sync with `completed`, meaning `pending` translates to false while `approved`, `rejected`, and `changes_requested` translate to true. If you set completed to true, this field will be set to `approved`.. [optional]  # noqa: E501
-            assignee_status (str): *Deprecated* Scheduling status of this task for the user it is assigned to. This field can only be set if the assignee is non-null. Setting this field to \"inbox\" or \"upcoming\" inserts it at the top of the section, while the other options will insert at the bottom.. [optional]  # noqa: E501
-            completed (bool): True if the task is currently marked complete, false if not.. [optional]  # noqa: E501
-            due_at (datetime, none_type): The UTC date and time on which this task is due, or null if the task has no due time. This takes an ISO 8601 date string in UTC and should not be used together with `due_on`.. [optional]  # noqa: E501
-            due_on (date, none_type): The localized date on which this task is due, or null if the task has no due date. This takes a date with `YYYY-MM-DD` format and should not be used together with `due_at`.. [optional]  # noqa: E501
-            external (TaskBaseAllOfExternal): [optional]  # noqa: E501
-            html_notes (str): [Opt In](/docs/inputoutput-options). The notes of the text with formatting as HTML.. [optional]  # noqa: E501
-            liked (bool): True if the task is liked by the authorized user, false if not.. [optional]  # noqa: E501
-            name (str): Name of the task. This is generally a short sentence fragment that fits on a line in the UI for maximum readability. However, it can be longer.. [optional]  # noqa: E501
-            notes (str): Free-form textual information associated with the task (i.e. its description).. [optional]  # noqa: E501
-            start_at (datetime, none_type): Date and time on which work begins for the task, or null if the task has no start time. This takes an ISO 8601 date string in UTC and should not be used together with `start_on`. *Note: `due_at` must be present in the request when setting or unsetting the `start_at` parameter.*. [optional]  # noqa: E501
-            start_on (date, none_type): The day on which work begins for the task , or null if the task has no start date. This takes a date with `YYYY-MM-DD` format and should not be used together with `start_at`. *Note: `due_on` or `due_at` must be present in the request when setting or unsetting the `start_on` parameter.*. [optional]  # noqa: E501
+            gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
+            name (str): The name of the goal.. [optional]  # noqa: E501
+            html_notes (str): The notes of the goal with formatting as HTML.. [optional]  # noqa: E501
+            notes (str): Free-form textual information associated with the goal (i.e. its description).. [optional]  # noqa: E501
+            due_on (str, none_type): The localized day on which this goal is due. This takes a date with format `YYYY-MM-DD`.. [optional]  # noqa: E501
+            start_on (str, none_type): The day on which work for this goal begins, or null if the goal has no start date. This takes a date with `YYYY-MM-DD` format, and cannot be set unless there is an accompanying due date.. [optional]  # noqa: E501
+            status (str, none_type): The current status of this goal. When the goal is open, its status can be `green`, `yellow`, and `red` to reflect \"On Track\", \"At Risk\", and \"Off Track\", respectively. When the goal is closed, the value can be `missed`, `achieved`, `partial`, or `dropped`. *Note* you can only write to this property if `metric` is set.. [optional]  # noqa: E501
+            is_workspace_level (bool): *Conditional*. This property is only present when the `workspace` provided is an organization. Whether the goal belongs to the `workspace` (and is listed as part of the workspace’s goals) or not. If it isn’t a workspace-level goal, it is a team-level goal, and is associated with the goal’s team.. [optional]  # noqa: E501
+            liked (bool): True if the goal is liked by the authorized user, false if not.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         self = super(OpenApiModel, cls).__new__(cls)
 
         if args:
@@ -214,36 +197,54 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        constant_args = {
+            '_check_type': _check_type,
+            '_path_to_item': _path_to_item,
+            '_spec_property_naming': _spec_property_naming,
+            '_configuration': _configuration,
+            '_visited_composed_classes': self._visited_composed_classes,
+        }
+        composed_info = validate_get_composed_info(
+            constant_args, kwargs, self)
+        self._composed_instances = composed_info[0]
+        self._var_name_to_model_instances = composed_info[1]
+        self._additional_properties_model_instances = composed_info[2]
+        discarded_args = composed_info[3]
+
         for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
+            if var_name in discarded_args and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
+                        self._additional_properties_model_instances:
                 # discard variable.
                 continue
             setattr(self, var_name, var_value)
+
         return self
 
     required_properties = set([
         '_data_store',
         '_check_type',
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
+        '_composed_instances',
+        '_var_name_to_model_instances',
+        '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TaskBaseAllOf - a model defined in OpenAPI
+        """GoalBase - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -268,26 +269,24 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            approval_status (str): *Conditional* Reflects the approval status of this task. This field is kept in sync with `completed`, meaning `pending` translates to false while `approved`, `rejected`, and `changes_requested` translate to true. If you set completed to true, this field will be set to `approved`.. [optional]  # noqa: E501
-            assignee_status (str): *Deprecated* Scheduling status of this task for the user it is assigned to. This field can only be set if the assignee is non-null. Setting this field to \"inbox\" or \"upcoming\" inserts it at the top of the section, while the other options will insert at the bottom.. [optional]  # noqa: E501
-            completed (bool): True if the task is currently marked complete, false if not.. [optional]  # noqa: E501
-            due_at (datetime, none_type): The UTC date and time on which this task is due, or null if the task has no due time. This takes an ISO 8601 date string in UTC and should not be used together with `due_on`.. [optional]  # noqa: E501
-            due_on (date, none_type): The localized date on which this task is due, or null if the task has no due date. This takes a date with `YYYY-MM-DD` format and should not be used together with `due_at`.. [optional]  # noqa: E501
-            external (TaskBaseAllOfExternal): [optional]  # noqa: E501
-            html_notes (str): [Opt In](/docs/inputoutput-options). The notes of the text with formatting as HTML.. [optional]  # noqa: E501
-            liked (bool): True if the task is liked by the authorized user, false if not.. [optional]  # noqa: E501
-            name (str): Name of the task. This is generally a short sentence fragment that fits on a line in the UI for maximum readability. However, it can be longer.. [optional]  # noqa: E501
-            notes (str): Free-form textual information associated with the task (i.e. its description).. [optional]  # noqa: E501
-            start_at (datetime, none_type): Date and time on which work begins for the task, or null if the task has no start time. This takes an ISO 8601 date string in UTC and should not be used together with `start_on`. *Note: `due_at` must be present in the request when setting or unsetting the `start_at` parameter.*. [optional]  # noqa: E501
-            start_on (date, none_type): The day on which work begins for the task , or null if the task has no start date. This takes a date with `YYYY-MM-DD` format and should not be used together with `start_at`. *Note: `due_on` or `due_at` must be present in the request when setting or unsetting the `start_on` parameter.*. [optional]  # noqa: E501
+            gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
+            name (str): The name of the goal.. [optional]  # noqa: E501
+            html_notes (str): The notes of the goal with formatting as HTML.. [optional]  # noqa: E501
+            notes (str): Free-form textual information associated with the goal (i.e. its description).. [optional]  # noqa: E501
+            due_on (str, none_type): The localized day on which this goal is due. This takes a date with format `YYYY-MM-DD`.. [optional]  # noqa: E501
+            start_on (str, none_type): The day on which work for this goal begins, or null if the goal has no start date. This takes a date with `YYYY-MM-DD` format, and cannot be set unless there is an accompanying due date.. [optional]  # noqa: E501
+            status (str, none_type): The current status of this goal. When the goal is open, its status can be `green`, `yellow`, and `red` to reflect \"On Track\", \"At Risk\", and \"Off Track\", respectively. When the goal is closed, the value can be `missed`, `achieved`, `partial`, or `dropped`. *Note* you can only write to this property if `metric` is set.. [optional]  # noqa: E501
+            is_workspace_level (bool): *Conditional*. This property is only present when the `workspace` provided is an organization. Whether the goal belongs to the `workspace` (and is listed as part of the workspace’s goals) or not. If it isn’t a workspace-level goal, it is a team-level goal, and is associated with the goal’s team.. [optional]  # noqa: E501
+            liked (bool): True if the goal is liked by the authorized user, false if not.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -309,18 +308,53 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        constant_args = {
+            '_check_type': _check_type,
+            '_path_to_item': _path_to_item,
+            '_spec_property_naming': _spec_property_naming,
+            '_configuration': _configuration,
+            '_visited_composed_classes': self._visited_composed_classes,
+        }
+        composed_info = validate_get_composed_info(
+            constant_args, kwargs, self)
+        self._composed_instances = composed_info[0]
+        self._var_name_to_model_instances = composed_info[1]
+        self._additional_properties_model_instances = composed_info[2]
+        discarded_args = composed_info[3]
+
         for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
+            if var_name in discarded_args and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
+                        self._additional_properties_model_instances:
                 # discard variable.
                 continue
             setattr(self, var_name, var_value)
             if var_name in self.read_only_vars:
                 raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
                                      f"class with read only attributes.")
+
+    @cached_property
+    def _composed_schemas():
+        # we need this here to make our import statements work
+        # we must store _composed_schemas in here so the code is only run
+        # when we invoke this method. If we kept this at the class
+        # level we would get an error because the class level
+        # code would be run when this module is imported, and these composed
+        # classes don't exist yet because their module has not finished
+        # loading
+        lazy_import()
+        return {
+          'anyOf': [
+          ],
+          'allOf': [
+              AsanaResource,
+              GoalBaseAllOf,
+          ],
+          'oneOf': [
+          ],
+        }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `asana-preview-1.0.4/asana_preview/model/task_base_all_of_external.py` & `asana-preview-1.0.5/asana_preview/model/task_base_all_of_external.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `asana-preview-1.0.4/asana_preview/model/task_compact.py` & `asana-preview-1.0.5/asana_preview/model/task_compact.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -92,15 +92,15 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'gid': (str,),  # noqa: E501
-            'resource_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'resource_type': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'resource_subtype': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
@@ -111,14 +111,15 @@
         'resource_type': 'resource_type',  # noqa: E501
         'name': 'name',  # noqa: E501
         'resource_subtype': 'resource_subtype',  # noqa: E501
     }
 
     read_only_vars = {
         'gid',  # noqa: E501
+        'resource_type',  # noqa: E501
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
         """TaskCompact - a model defined in OpenAPI
 
@@ -150,17 +151,17 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
             name (str): The name of the task.. [optional]  # noqa: E501
-            resource_subtype (str): The subtype of this resource. Different subtypes retain many of the same fields and behavior, but may render differently in Asana or represent resources with different semantic meaning.  The resource_subtype `milestone` represent a single moment in time. This means tasks with this subtype cannot have a start_date.. [optional]  # noqa: E501
+            resource_subtype (str): The subtype of this resource. Different subtypes retain many of the same fields and behavior, but may render differently in Asana or represent resources with different semantic meaning. The resource_subtype `milestone` represent a single moment in time. This means tasks with this subtype cannot have a start_date.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -257,17 +258,17 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
             name (str): The name of the task.. [optional]  # noqa: E501
-            resource_subtype (str): The subtype of this resource. Different subtypes retain many of the same fields and behavior, but may render differently in Asana or represent resources with different semantic meaning.  The resource_subtype `milestone` represent a single moment in time. This means tasks with this subtype cannot have a start_date.. [optional]  # noqa: E501
+            resource_subtype (str): The subtype of this resource. Different subtypes retain many of the same fields and behavior, but may render differently in Asana or represent resources with different semantic meaning. The resource_subtype `milestone` represent a single moment in time. This means tasks with this subtype cannot have a start_date.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `asana-preview-1.0.4/asana_preview/model/task_compact_all_of.py` & `asana-preview-1.0.5/asana_preview/model/workspace_membership_response_all_of_vacation_dates.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from asana_preview.exceptions import ApiAttributeError
 
 
 
-class TaskCompactAllOf(ModelNormal):
+class WorkspaceMembershipResponseAllOfVacationDates(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -51,71 +51,63 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('resource_subtype',): {
-            'DEFAULT_TASK': "default_task",
-            'MILESTONE': "milestone",
-            'SECTION': "section",
-            'APPROVAL': "approval",
-        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
-    _nullable = False
+    _nullable = True
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'resource_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
-            'name': (str,),  # noqa: E501
-            'resource_subtype': (str,),  # noqa: E501
+            'start_on': (str,),  # noqa: E501
+            'end_on': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'resource_type': 'resource_type',  # noqa: E501
-        'name': 'name',  # noqa: E501
-        'resource_subtype': 'resource_subtype',  # noqa: E501
+        'start_on': 'start_on',  # noqa: E501
+        'end_on': 'end_on',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TaskCompactAllOf - a model defined in OpenAPI
+        """WorkspaceMembershipResponseAllOfVacationDates - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -140,17 +132,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            name (str): The name of the task.. [optional]  # noqa: E501
-            resource_subtype (str): The subtype of this resource. Different subtypes retain many of the same fields and behavior, but may render differently in Asana or represent resources with different semantic meaning.  The resource_subtype `milestone` represent a single moment in time. This means tasks with this subtype cannot have a start_date.. [optional]  # noqa: E501
+            start_on (str): The day on which the user's vacation in this workspace starts. This is a date with `YYYY-MM-DD` format.. [optional]  # noqa: E501
+            end_on (str, none_type): The day on which the user's vacation in this workspace ends, or null if there is no end date. This is a date with `YYYY-MM-DD` format.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -195,15 +186,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TaskCompactAllOf - a model defined in OpenAPI
+        """WorkspaceMembershipResponseAllOfVacationDates - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -228,17 +219,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            name (str): The name of the task.. [optional]  # noqa: E501
-            resource_subtype (str): The subtype of this resource. Different subtypes retain many of the same fields and behavior, but may render differently in Asana or represent resources with different semantic meaning.  The resource_subtype `milestone` represent a single moment in time. This means tasks with this subtype cannot have a start_date.. [optional]  # noqa: E501
+            start_on (str): The day on which the user's vacation in this workspace starts. This is a date with `YYYY-MM-DD` format.. [optional]  # noqa: E501
+            end_on (str, none_type): The day on which the user's vacation in this workspace ends, or null if there is no end date. This is a date with `YYYY-MM-DD` format.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `asana-preview-1.0.4/asana_preview/model/task_response.py` & `asana-preview-1.0.5/asana_preview/model/task_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -33,26 +33,26 @@
     from asana_preview.model.asana_resource import AsanaResource
     from asana_preview.model.custom_field_response import CustomFieldResponse
     from asana_preview.model.like import Like
     from asana_preview.model.project_compact import ProjectCompact
     from asana_preview.model.tag_compact import TagCompact
     from asana_preview.model.task_base import TaskBase
     from asana_preview.model.task_base_all_of_external import TaskBaseAllOfExternal
+    from asana_preview.model.task_base_all_of_memberships import TaskBaseAllOfMemberships
     from asana_preview.model.task_response_all_of import TaskResponseAllOf
-    from asana_preview.model.task_response_all_of_memberships import TaskResponseAllOfMemberships
     from asana_preview.model.user_compact import UserCompact
     globals()['AsanaResource'] = AsanaResource
     globals()['CustomFieldResponse'] = CustomFieldResponse
     globals()['Like'] = Like
     globals()['ProjectCompact'] = ProjectCompact
     globals()['TagCompact'] = TagCompact
     globals()['TaskBase'] = TaskBase
     globals()['TaskBaseAllOfExternal'] = TaskBaseAllOfExternal
+    globals()['TaskBaseAllOfMemberships'] = TaskBaseAllOfMemberships
     globals()['TaskResponseAllOf'] = TaskResponseAllOf
-    globals()['TaskResponseAllOfMemberships'] = TaskResponseAllOfMemberships
     globals()['UserCompact'] = UserCompact
 
 
 class TaskResponse(ModelComposed):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
@@ -121,52 +121,52 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'gid': (str,),  # noqa: E501
-            'resource_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'resource_type': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'resource_subtype': (str,),  # noqa: E501
             'approval_status': (str,),  # noqa: E501
             'assignee_status': (str,),  # noqa: E501
             'completed': (bool,),  # noqa: E501
-            'due_at': (datetime, none_type,),  # noqa: E501
-            'due_on': (date, none_type,),  # noqa: E501
-            'external': (TaskBaseAllOfExternal,),  # noqa: E501
-            'html_notes': (str,),  # noqa: E501
-            'liked': (bool,),  # noqa: E501
-            'notes': (str,),  # noqa: E501
-            'start_at': (datetime, none_type,),  # noqa: E501
-            'start_on': (date, none_type,),  # noqa: E501
-            'actual_time_minutes': (float, none_type,),  # noqa: E501
-            'assignee': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
-            'assignee_section': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'completed_at': (datetime, none_type,),  # noqa: E501
+            'completed_by': (UserCompact,),  # noqa: E501
             'created_at': (datetime,),  # noqa: E501
-            'completed_by': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
-            'custom_fields': ([CustomFieldResponse],),  # noqa: E501
             'dependencies': ([AsanaResource],),  # noqa: E501
             'dependents': ([AsanaResource],),  # noqa: E501
-            'followers': ([UserCompact],),  # noqa: E501
+            'due_at': (date, none_type,),  # noqa: E501
+            'due_on': (date, none_type,),  # noqa: E501
+            'external': (TaskBaseAllOfExternal,),  # noqa: E501
+            'html_notes': (str,),  # noqa: E501
             'hearted': (bool,),  # noqa: E501
             'hearts': ([Like],),  # noqa: E501
             'is_rendered_as_separator': (bool,),  # noqa: E501
+            'liked': (bool,),  # noqa: E501
             'likes': ([Like],),  # noqa: E501
-            'memberships': ([TaskResponseAllOfMemberships],),  # noqa: E501
+            'memberships': ([TaskBaseAllOfMemberships],),  # noqa: E501
             'modified_at': (datetime,),  # noqa: E501
+            'notes': (str,),  # noqa: E501
             'num_hearts': (int,),  # noqa: E501
             'num_likes': (int,),  # noqa: E501
             'num_subtasks': (int,),  # noqa: E501
+            'start_at': (date, none_type,),  # noqa: E501
+            'start_on': (date, none_type,),  # noqa: E501
+            'actual_time_minutes': (float, none_type,),  # noqa: E501
+            'assignee': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'assignee_section': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'custom_fields': ([CustomFieldResponse],),  # noqa: E501
+            'followers': ([UserCompact],),  # noqa: E501
             'parent': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
-            'permalink_url': (str,),  # noqa: E501
             'projects': ([ProjectCompact],),  # noqa: E501
             'tags': ([TagCompact],),  # noqa: E501
             'workspace': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'permalink_url': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -174,71 +174,70 @@
         'gid': 'gid',  # noqa: E501
         'resource_type': 'resource_type',  # noqa: E501
         'name': 'name',  # noqa: E501
         'resource_subtype': 'resource_subtype',  # noqa: E501
         'approval_status': 'approval_status',  # noqa: E501
         'assignee_status': 'assignee_status',  # noqa: E501
         'completed': 'completed',  # noqa: E501
-        'due_at': 'due_at',  # noqa: E501
-        'due_on': 'due_on',  # noqa: E501
-        'external': 'external',  # noqa: E501
-        'html_notes': 'html_notes',  # noqa: E501
-        'liked': 'liked',  # noqa: E501
-        'notes': 'notes',  # noqa: E501
-        'start_at': 'start_at',  # noqa: E501
-        'start_on': 'start_on',  # noqa: E501
-        'actual_time_minutes': 'actual_time_minutes',  # noqa: E501
-        'assignee': 'assignee',  # noqa: E501
-        'assignee_section': 'assignee_section',  # noqa: E501
         'completed_at': 'completed_at',  # noqa: E501
-        'created_at': 'created_at',  # noqa: E501
         'completed_by': 'completed_by',  # noqa: E501
-        'custom_fields': 'custom_fields',  # noqa: E501
+        'created_at': 'created_at',  # noqa: E501
         'dependencies': 'dependencies',  # noqa: E501
         'dependents': 'dependents',  # noqa: E501
-        'followers': 'followers',  # noqa: E501
+        'due_at': 'due_at',  # noqa: E501
+        'due_on': 'due_on',  # noqa: E501
+        'external': 'external',  # noqa: E501
+        'html_notes': 'html_notes',  # noqa: E501
         'hearted': 'hearted',  # noqa: E501
         'hearts': 'hearts',  # noqa: E501
         'is_rendered_as_separator': 'is_rendered_as_separator',  # noqa: E501
+        'liked': 'liked',  # noqa: E501
         'likes': 'likes',  # noqa: E501
         'memberships': 'memberships',  # noqa: E501
         'modified_at': 'modified_at',  # noqa: E501
+        'notes': 'notes',  # noqa: E501
         'num_hearts': 'num_hearts',  # noqa: E501
         'num_likes': 'num_likes',  # noqa: E501
         'num_subtasks': 'num_subtasks',  # noqa: E501
+        'start_at': 'start_at',  # noqa: E501
+        'start_on': 'start_on',  # noqa: E501
+        'actual_time_minutes': 'actual_time_minutes',  # noqa: E501
+        'assignee': 'assignee',  # noqa: E501
+        'assignee_section': 'assignee_section',  # noqa: E501
+        'custom_fields': 'custom_fields',  # noqa: E501
+        'followers': 'followers',  # noqa: E501
         'parent': 'parent',  # noqa: E501
-        'permalink_url': 'permalink_url',  # noqa: E501
         'projects': 'projects',  # noqa: E501
         'tags': 'tags',  # noqa: E501
         'workspace': 'workspace',  # noqa: E501
+        'permalink_url': 'permalink_url',  # noqa: E501
     }
 
     read_only_vars = {
         'gid',  # noqa: E501
-        'actual_time_minutes',  # noqa: E501
-        'assignee_section',  # noqa: E501
+        'resource_type',  # noqa: E501
         'completed_at',  # noqa: E501
         'created_at',  # noqa: E501
-        'completed_by',  # noqa: E501
-        'custom_fields',  # noqa: E501
         'dependencies',  # noqa: E501
         'dependents',  # noqa: E501
-        'followers',  # noqa: E501
         'hearted',  # noqa: E501
         'hearts',  # noqa: E501
         'is_rendered_as_separator',  # noqa: E501
         'likes',  # noqa: E501
         'memberships',  # noqa: E501
         'modified_at',  # noqa: E501
         'num_hearts',  # noqa: E501
         'num_likes',  # noqa: E501
         'num_subtasks',  # noqa: E501
-        'permalink_url',  # noqa: E501
+        'actual_time_minutes',  # noqa: E501
+        'custom_fields',  # noqa: E501
+        'followers',  # noqa: E501
         'projects',  # noqa: E501
         'tags',  # noqa: E501
+        'permalink_url',  # noqa: E501
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
         """TaskResponse - a model defined in OpenAPI
 
@@ -270,52 +269,52 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
             name (str): Name of the task. This is generally a short sentence fragment that fits on a line in the UI for maximum readability. However, it can be longer.. [optional]  # noqa: E501
-            resource_subtype (str): The subtype of this resource. Different subtypes retain many of the same fields and behavior, but may render differently in Asana or represent resources with different semantic meaning.  The resource_subtype `milestone` represent a single moment in time. This means tasks with this subtype cannot have a start_date.. [optional]  # noqa: E501
+            resource_subtype (str): The subtype of this resource. Different subtypes retain many of the same fields and behavior, but may render differently in Asana or represent resources with different semantic meaning. The resource_subtype `milestone` represent a single moment in time. This means tasks with this subtype cannot have a start_date.. [optional]  # noqa: E501
             approval_status (str): *Conditional* Reflects the approval status of this task. This field is kept in sync with `completed`, meaning `pending` translates to false while `approved`, `rejected`, and `changes_requested` translate to true. If you set completed to true, this field will be set to `approved`.. [optional]  # noqa: E501
             assignee_status (str): *Deprecated* Scheduling status of this task for the user it is assigned to. This field can only be set if the assignee is non-null. Setting this field to \"inbox\" or \"upcoming\" inserts it at the top of the section, while the other options will insert at the bottom.. [optional]  # noqa: E501
             completed (bool): True if the task is currently marked complete, false if not.. [optional]  # noqa: E501
-            due_at (datetime, none_type): The UTC date and time on which this task is due, or null if the task has no due time. This takes an ISO 8601 date string in UTC and should not be used together with `due_on`.. [optional]  # noqa: E501
+            completed_at (datetime, none_type): The time at which this task was completed, or null if the task is incomplete.. [optional]  # noqa: E501
+            completed_by (UserCompact): [optional]  # noqa: E501
+            created_at (datetime): The time at which this resource was created.. [optional]  # noqa: E501
+            dependencies ([AsanaResource]): [Opt In](/docs/inputoutput-options). Array of resources referencing tasks that this task depends on. The objects contain only the gid of the dependency.. [optional]  # noqa: E501
+            dependents ([AsanaResource]): [Opt In](/docs/inputoutput-options). Array of resources referencing tasks that depend on this task. The objects contain only the ID of the dependent.. [optional]  # noqa: E501
+            due_at (date, none_type): The UTC date and time on which this task is due, or null if the task has no due time. This takes an ISO 8601 date string in UTC and should not be used together with `due_on`.. [optional]  # noqa: E501
             due_on (date, none_type): The localized date on which this task is due, or null if the task has no due date. This takes a date with `YYYY-MM-DD` format and should not be used together with `due_at`.. [optional]  # noqa: E501
             external (TaskBaseAllOfExternal): [optional]  # noqa: E501
             html_notes (str): [Opt In](/docs/inputoutput-options). The notes of the text with formatting as HTML.. [optional]  # noqa: E501
+            hearted (bool): *Deprecated - please use liked instead* True if the task is hearted by the authorized user, false if not.. [optional]  # noqa: E501
+            hearts ([Like]): *Deprecated - please use likes instead* Array of likes for users who have hearted this task.. [optional]  # noqa: E501
+            is_rendered_as_separator (bool): [Opt In](/docs/inputoutput-options). In some contexts tasks can be rendered as a visual separator; for instance, subtasks can appear similar to [sections](/reference/sections) without being true `section` objects. If a `task` object is rendered this way in any context it will have the property `is_rendered_as_separator` set to `true`.. [optional]  # noqa: E501
             liked (bool): True if the task is liked by the authorized user, false if not.. [optional]  # noqa: E501
+            likes ([Like]): Array of likes for users who have liked this task.. [optional]  # noqa: E501
+            memberships ([TaskBaseAllOfMemberships]): *Create-only*. Array of projects this task is associated with and the section it is in. At task creation time, this array can be used to add the task to specific sections. After task creation, these associations can be modified using the `addProject` and `removeProject` endpoints. Note that over time, more types of memberships may be added to this property.. [optional]  # noqa: E501
+            modified_at (datetime): The time at which this task was last modified.  The following conditions will change `modified_at`:  - story is created on a task - story is trashed on a task - attachment is trashed on a task - task is assigned or unassigned - custom field value is changed - the task itself is trashed - Or if any of the following fields are updated:   - completed   - name   - due_date   - description   - attachments   - items   - schedule_status  The following conditions will _not_ change `modified_at`:  - moving to a new container (project, portfolio, etc) - comments being added to the task (but the stories they generate   _will_ affect `modified_at`). [optional]  # noqa: E501
             notes (str): Free-form textual information associated with the task (i.e. its description).. [optional]  # noqa: E501
-            start_at (datetime, none_type): Date and time on which work begins for the task, or null if the task has no start time. This takes an ISO 8601 date string in UTC and should not be used together with `start_on`. *Note: `due_at` must be present in the request when setting or unsetting the `start_at` parameter.*. [optional]  # noqa: E501
+            num_hearts (int): *Deprecated - please use likes instead* The number of users who have hearted this task.. [optional]  # noqa: E501
+            num_likes (int): The number of users who have liked this task.. [optional]  # noqa: E501
+            num_subtasks (int): [Opt In](/docs/inputoutput-options). The number of subtasks on this task. . [optional]  # noqa: E501
+            start_at (date, none_type): Date and time on which work begins for the task, or null if the task has no start time. This takes an ISO 8601 date string in UTC and should not be used together with `start_on`. *Note: `due_at` must be present in the request when setting or unsetting the `start_at` parameter.*. [optional]  # noqa: E501
             start_on (date, none_type): The day on which work begins for the task , or null if the task has no start date. This takes a date with `YYYY-MM-DD` format and should not be used together with `start_at`. *Note: `due_on` or `due_at` must be present in the request when setting or unsetting the `start_on` parameter.*. [optional]  # noqa: E501
             actual_time_minutes (float, none_type): This value represents the sum of all the Time Tracking entries in the Actual Time field on a given Task. It is represented as a nullable long value.. [optional]  # noqa: E501
             assignee (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             assignee_section (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            completed_at (datetime, none_type): The time at which this task was completed, or null if the task is incomplete.. [optional]  # noqa: E501
-            created_at (datetime): The time at which this task was created.. [optional]  # noqa: E501
-            completed_by (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             custom_fields ([CustomFieldResponse]): Array of custom field values applied to the task. These represent the custom field values recorded on this project for a particular custom field. For example, these custom field values will contain an `enum_value` property for custom fields of type `enum`, a `text_value` property for custom fields of type `text`, and so on. Please note that the `gid` returned on each custom field value *is identical* to the `gid` of the custom field, which allows referencing the custom field metadata through the `/custom_fields/custom_field-gid` endpoint.. [optional]  # noqa: E501
-            dependencies ([AsanaResource]): [Opt In](/docs/inputoutput-options). Array of resources referencing tasks that this task depends on. The objects contain only the gid of the dependency.. [optional]  # noqa: E501
-            dependents ([AsanaResource]): [Opt In](/docs/inputoutput-options). Array of resources referencing tasks that depend on this task. The objects contain only the ID of the dependent.. [optional]  # noqa: E501
             followers ([UserCompact]): Array of users following this task.. [optional]  # noqa: E501
-            hearted (bool): *Deprecated - please use liked instead* True if the task is hearted by the authorized user, false if not.. [optional]  # noqa: E501
-            hearts ([Like]): *Deprecated - please use likes instead* Array of likes for users who have hearted this task.. [optional]  # noqa: E501
-            is_rendered_as_separator (bool): [Opt In](/docs/inputoutput-options). In some contexts tasks can be rendered as a visual separator; for instance, subtasks can appear similar to [sections](/reference/sections) without being true `section` objects. If a `task` object is rendered this way in any context it will have the property `is_rendered_as_separator` set to `true`.. [optional]  # noqa: E501
-            likes ([Like]): Array of likes for users who have liked this task.. [optional]  # noqa: E501
-            memberships ([TaskResponseAllOfMemberships]): *Create-only*. Array of projects this task is associated with and the section it is in. At task creation time, this array can be used to add the task to specific sections. After task creation, these associations can be modified using the `addProject` and `removeProject` endpoints. Note that over time, more types of memberships may be added to this property.. [optional]  # noqa: E501
-            modified_at (datetime): The time at which this task was last modified.  *Note: This does not currently reflect any changes in associations such as projects or comments that may have been added or removed from the task.*. [optional]  # noqa: E501
-            num_hearts (int): *Deprecated - please use likes instead* The number of users who have hearted this task.. [optional]  # noqa: E501
-            num_likes (int): The number of users who have liked this task.. [optional]  # noqa: E501
-            num_subtasks (int): [Opt In](/docs/inputoutput-options). The number of subtasks on this task. . [optional]  # noqa: E501
             parent (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            permalink_url (str): A url that points directly to the object within Asana.. [optional]  # noqa: E501
             projects ([ProjectCompact]): *Create-only.* Array of projects this task is associated with. At task creation time, this array can be used to add the task to many projects at once. After task creation, these associations can be modified using the addProject and removeProject endpoints.. [optional]  # noqa: E501
             tags ([TagCompact]): Array of tags associated with this task. In order to change tags on an existing task use `addTag` and `removeTag`.. [optional]  # noqa: E501
             workspace (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            permalink_url (str): A url that points directly to the object within Asana.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -412,52 +411,52 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
             name (str): Name of the task. This is generally a short sentence fragment that fits on a line in the UI for maximum readability. However, it can be longer.. [optional]  # noqa: E501
-            resource_subtype (str): The subtype of this resource. Different subtypes retain many of the same fields and behavior, but may render differently in Asana or represent resources with different semantic meaning.  The resource_subtype `milestone` represent a single moment in time. This means tasks with this subtype cannot have a start_date.. [optional]  # noqa: E501
+            resource_subtype (str): The subtype of this resource. Different subtypes retain many of the same fields and behavior, but may render differently in Asana or represent resources with different semantic meaning. The resource_subtype `milestone` represent a single moment in time. This means tasks with this subtype cannot have a start_date.. [optional]  # noqa: E501
             approval_status (str): *Conditional* Reflects the approval status of this task. This field is kept in sync with `completed`, meaning `pending` translates to false while `approved`, `rejected`, and `changes_requested` translate to true. If you set completed to true, this field will be set to `approved`.. [optional]  # noqa: E501
             assignee_status (str): *Deprecated* Scheduling status of this task for the user it is assigned to. This field can only be set if the assignee is non-null. Setting this field to \"inbox\" or \"upcoming\" inserts it at the top of the section, while the other options will insert at the bottom.. [optional]  # noqa: E501
             completed (bool): True if the task is currently marked complete, false if not.. [optional]  # noqa: E501
-            due_at (datetime, none_type): The UTC date and time on which this task is due, or null if the task has no due time. This takes an ISO 8601 date string in UTC and should not be used together with `due_on`.. [optional]  # noqa: E501
+            completed_at (datetime, none_type): The time at which this task was completed, or null if the task is incomplete.. [optional]  # noqa: E501
+            completed_by (UserCompact): [optional]  # noqa: E501
+            created_at (datetime): The time at which this resource was created.. [optional]  # noqa: E501
+            dependencies ([AsanaResource]): [Opt In](/docs/inputoutput-options). Array of resources referencing tasks that this task depends on. The objects contain only the gid of the dependency.. [optional]  # noqa: E501
+            dependents ([AsanaResource]): [Opt In](/docs/inputoutput-options). Array of resources referencing tasks that depend on this task. The objects contain only the ID of the dependent.. [optional]  # noqa: E501
+            due_at (date, none_type): The UTC date and time on which this task is due, or null if the task has no due time. This takes an ISO 8601 date string in UTC and should not be used together with `due_on`.. [optional]  # noqa: E501
             due_on (date, none_type): The localized date on which this task is due, or null if the task has no due date. This takes a date with `YYYY-MM-DD` format and should not be used together with `due_at`.. [optional]  # noqa: E501
             external (TaskBaseAllOfExternal): [optional]  # noqa: E501
             html_notes (str): [Opt In](/docs/inputoutput-options). The notes of the text with formatting as HTML.. [optional]  # noqa: E501
+            hearted (bool): *Deprecated - please use liked instead* True if the task is hearted by the authorized user, false if not.. [optional]  # noqa: E501
+            hearts ([Like]): *Deprecated - please use likes instead* Array of likes for users who have hearted this task.. [optional]  # noqa: E501
+            is_rendered_as_separator (bool): [Opt In](/docs/inputoutput-options). In some contexts tasks can be rendered as a visual separator; for instance, subtasks can appear similar to [sections](/reference/sections) without being true `section` objects. If a `task` object is rendered this way in any context it will have the property `is_rendered_as_separator` set to `true`.. [optional]  # noqa: E501
             liked (bool): True if the task is liked by the authorized user, false if not.. [optional]  # noqa: E501
+            likes ([Like]): Array of likes for users who have liked this task.. [optional]  # noqa: E501
+            memberships ([TaskBaseAllOfMemberships]): *Create-only*. Array of projects this task is associated with and the section it is in. At task creation time, this array can be used to add the task to specific sections. After task creation, these associations can be modified using the `addProject` and `removeProject` endpoints. Note that over time, more types of memberships may be added to this property.. [optional]  # noqa: E501
+            modified_at (datetime): The time at which this task was last modified.  The following conditions will change `modified_at`:  - story is created on a task - story is trashed on a task - attachment is trashed on a task - task is assigned or unassigned - custom field value is changed - the task itself is trashed - Or if any of the following fields are updated:   - completed   - name   - due_date   - description   - attachments   - items   - schedule_status  The following conditions will _not_ change `modified_at`:  - moving to a new container (project, portfolio, etc) - comments being added to the task (but the stories they generate   _will_ affect `modified_at`). [optional]  # noqa: E501
             notes (str): Free-form textual information associated with the task (i.e. its description).. [optional]  # noqa: E501
-            start_at (datetime, none_type): Date and time on which work begins for the task, or null if the task has no start time. This takes an ISO 8601 date string in UTC and should not be used together with `start_on`. *Note: `due_at` must be present in the request when setting or unsetting the `start_at` parameter.*. [optional]  # noqa: E501
+            num_hearts (int): *Deprecated - please use likes instead* The number of users who have hearted this task.. [optional]  # noqa: E501
+            num_likes (int): The number of users who have liked this task.. [optional]  # noqa: E501
+            num_subtasks (int): [Opt In](/docs/inputoutput-options). The number of subtasks on this task. . [optional]  # noqa: E501
+            start_at (date, none_type): Date and time on which work begins for the task, or null if the task has no start time. This takes an ISO 8601 date string in UTC and should not be used together with `start_on`. *Note: `due_at` must be present in the request when setting or unsetting the `start_at` parameter.*. [optional]  # noqa: E501
             start_on (date, none_type): The day on which work begins for the task , or null if the task has no start date. This takes a date with `YYYY-MM-DD` format and should not be used together with `start_at`. *Note: `due_on` or `due_at` must be present in the request when setting or unsetting the `start_on` parameter.*. [optional]  # noqa: E501
             actual_time_minutes (float, none_type): This value represents the sum of all the Time Tracking entries in the Actual Time field on a given Task. It is represented as a nullable long value.. [optional]  # noqa: E501
             assignee (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             assignee_section (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            completed_at (datetime, none_type): The time at which this task was completed, or null if the task is incomplete.. [optional]  # noqa: E501
-            created_at (datetime): The time at which this task was created.. [optional]  # noqa: E501
-            completed_by (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             custom_fields ([CustomFieldResponse]): Array of custom field values applied to the task. These represent the custom field values recorded on this project for a particular custom field. For example, these custom field values will contain an `enum_value` property for custom fields of type `enum`, a `text_value` property for custom fields of type `text`, and so on. Please note that the `gid` returned on each custom field value *is identical* to the `gid` of the custom field, which allows referencing the custom field metadata through the `/custom_fields/custom_field-gid` endpoint.. [optional]  # noqa: E501
-            dependencies ([AsanaResource]): [Opt In](/docs/inputoutput-options). Array of resources referencing tasks that this task depends on. The objects contain only the gid of the dependency.. [optional]  # noqa: E501
-            dependents ([AsanaResource]): [Opt In](/docs/inputoutput-options). Array of resources referencing tasks that depend on this task. The objects contain only the ID of the dependent.. [optional]  # noqa: E501
             followers ([UserCompact]): Array of users following this task.. [optional]  # noqa: E501
-            hearted (bool): *Deprecated - please use liked instead* True if the task is hearted by the authorized user, false if not.. [optional]  # noqa: E501
-            hearts ([Like]): *Deprecated - please use likes instead* Array of likes for users who have hearted this task.. [optional]  # noqa: E501
-            is_rendered_as_separator (bool): [Opt In](/docs/inputoutput-options). In some contexts tasks can be rendered as a visual separator; for instance, subtasks can appear similar to [sections](/reference/sections) without being true `section` objects. If a `task` object is rendered this way in any context it will have the property `is_rendered_as_separator` set to `true`.. [optional]  # noqa: E501
-            likes ([Like]): Array of likes for users who have liked this task.. [optional]  # noqa: E501
-            memberships ([TaskResponseAllOfMemberships]): *Create-only*. Array of projects this task is associated with and the section it is in. At task creation time, this array can be used to add the task to specific sections. After task creation, these associations can be modified using the `addProject` and `removeProject` endpoints. Note that over time, more types of memberships may be added to this property.. [optional]  # noqa: E501
-            modified_at (datetime): The time at which this task was last modified.  *Note: This does not currently reflect any changes in associations such as projects or comments that may have been added or removed from the task.*. [optional]  # noqa: E501
-            num_hearts (int): *Deprecated - please use likes instead* The number of users who have hearted this task.. [optional]  # noqa: E501
-            num_likes (int): The number of users who have liked this task.. [optional]  # noqa: E501
-            num_subtasks (int): [Opt In](/docs/inputoutput-options). The number of subtasks on this task. . [optional]  # noqa: E501
             parent (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            permalink_url (str): A url that points directly to the object within Asana.. [optional]  # noqa: E501
             projects ([ProjectCompact]): *Create-only.* Array of projects this task is associated with. At task creation time, this array can be used to add the task to many projects at once. After task creation, these associations can be modified using the addProject and removeProject endpoints.. [optional]  # noqa: E501
             tags ([TagCompact]): Array of tags associated with this task. In order to change tags on an existing task use `addTag` and `removeTag`.. [optional]  # noqa: E501
             workspace (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            permalink_url (str): A url that points directly to the object within Asana.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `asana-preview-1.0.4/asana_preview/model/task_response_all_of.py` & `asana-preview-1.0.5/asana_preview/model/task_base_all_of.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -27,30 +27,26 @@
     OpenApiModel
 )
 from asana_preview.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from asana_preview.model.asana_resource import AsanaResource
-    from asana_preview.model.custom_field_response import CustomFieldResponse
     from asana_preview.model.like import Like
-    from asana_preview.model.project_compact import ProjectCompact
-    from asana_preview.model.tag_compact import TagCompact
-    from asana_preview.model.task_response_all_of_memberships import TaskResponseAllOfMemberships
+    from asana_preview.model.task_base_all_of_external import TaskBaseAllOfExternal
+    from asana_preview.model.task_base_all_of_memberships import TaskBaseAllOfMemberships
     from asana_preview.model.user_compact import UserCompact
     globals()['AsanaResource'] = AsanaResource
-    globals()['CustomFieldResponse'] = CustomFieldResponse
     globals()['Like'] = Like
-    globals()['ProjectCompact'] = ProjectCompact
-    globals()['TagCompact'] = TagCompact
-    globals()['TaskResponseAllOfMemberships'] = TaskResponseAllOfMemberships
+    globals()['TaskBaseAllOfExternal'] = TaskBaseAllOfExternal
+    globals()['TaskBaseAllOfMemberships'] = TaskBaseAllOfMemberships
     globals()['UserCompact'] = UserCompact
 
 
-class TaskResponseAllOf(ModelNormal):
+class TaskBaseAllOf(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -67,14 +63,27 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
+        ('approval_status',): {
+            'PENDING': "pending",
+            'APPROVED': "approved",
+            'REJECTED': "rejected",
+            'CHANGES_REQUESTED': "changes_requested",
+        },
+        ('assignee_status',): {
+            'TODAY': "today",
+            'UPCOMING': "upcoming",
+            'LATER': "later",
+            'NEW': "new",
+            'INBOX': "inbox",
+        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
@@ -95,102 +104,101 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'actual_time_minutes': (float, none_type,),  # noqa: E501
-            'assignee': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
-            'assignee_section': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'approval_status': (str,),  # noqa: E501
+            'assignee_status': (str,),  # noqa: E501
+            'completed': (bool,),  # noqa: E501
             'completed_at': (datetime, none_type,),  # noqa: E501
+            'completed_by': (UserCompact,),  # noqa: E501
             'created_at': (datetime,),  # noqa: E501
-            'completed_by': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
-            'custom_fields': ([CustomFieldResponse],),  # noqa: E501
             'dependencies': ([AsanaResource],),  # noqa: E501
             'dependents': ([AsanaResource],),  # noqa: E501
-            'followers': ([UserCompact],),  # noqa: E501
+            'due_at': (date, none_type,),  # noqa: E501
+            'due_on': (date, none_type,),  # noqa: E501
+            'external': (TaskBaseAllOfExternal,),  # noqa: E501
+            'html_notes': (str,),  # noqa: E501
             'hearted': (bool,),  # noqa: E501
             'hearts': ([Like],),  # noqa: E501
             'is_rendered_as_separator': (bool,),  # noqa: E501
+            'liked': (bool,),  # noqa: E501
             'likes': ([Like],),  # noqa: E501
-            'memberships': ([TaskResponseAllOfMemberships],),  # noqa: E501
+            'memberships': ([TaskBaseAllOfMemberships],),  # noqa: E501
             'modified_at': (datetime,),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'notes': (str,),  # noqa: E501
             'num_hearts': (int,),  # noqa: E501
             'num_likes': (int,),  # noqa: E501
             'num_subtasks': (int,),  # noqa: E501
-            'parent': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
-            'permalink_url': (str,),  # noqa: E501
-            'projects': ([ProjectCompact],),  # noqa: E501
-            'tags': ([TagCompact],),  # noqa: E501
-            'workspace': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'start_at': (date, none_type,),  # noqa: E501
+            'start_on': (date, none_type,),  # noqa: E501
+            'actual_time_minutes': (float, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'actual_time_minutes': 'actual_time_minutes',  # noqa: E501
-        'assignee': 'assignee',  # noqa: E501
-        'assignee_section': 'assignee_section',  # noqa: E501
+        'approval_status': 'approval_status',  # noqa: E501
+        'assignee_status': 'assignee_status',  # noqa: E501
+        'completed': 'completed',  # noqa: E501
         'completed_at': 'completed_at',  # noqa: E501
-        'created_at': 'created_at',  # noqa: E501
         'completed_by': 'completed_by',  # noqa: E501
-        'custom_fields': 'custom_fields',  # noqa: E501
+        'created_at': 'created_at',  # noqa: E501
         'dependencies': 'dependencies',  # noqa: E501
         'dependents': 'dependents',  # noqa: E501
-        'followers': 'followers',  # noqa: E501
+        'due_at': 'due_at',  # noqa: E501
+        'due_on': 'due_on',  # noqa: E501
+        'external': 'external',  # noqa: E501
+        'html_notes': 'html_notes',  # noqa: E501
         'hearted': 'hearted',  # noqa: E501
         'hearts': 'hearts',  # noqa: E501
         'is_rendered_as_separator': 'is_rendered_as_separator',  # noqa: E501
+        'liked': 'liked',  # noqa: E501
         'likes': 'likes',  # noqa: E501
         'memberships': 'memberships',  # noqa: E501
         'modified_at': 'modified_at',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'notes': 'notes',  # noqa: E501
         'num_hearts': 'num_hearts',  # noqa: E501
         'num_likes': 'num_likes',  # noqa: E501
         'num_subtasks': 'num_subtasks',  # noqa: E501
-        'parent': 'parent',  # noqa: E501
-        'permalink_url': 'permalink_url',  # noqa: E501
-        'projects': 'projects',  # noqa: E501
-        'tags': 'tags',  # noqa: E501
-        'workspace': 'workspace',  # noqa: E501
+        'start_at': 'start_at',  # noqa: E501
+        'start_on': 'start_on',  # noqa: E501
+        'actual_time_minutes': 'actual_time_minutes',  # noqa: E501
     }
 
     read_only_vars = {
-        'actual_time_minutes',  # noqa: E501
-        'assignee_section',  # noqa: E501
         'completed_at',  # noqa: E501
         'created_at',  # noqa: E501
-        'completed_by',  # noqa: E501
-        'custom_fields',  # noqa: E501
         'dependencies',  # noqa: E501
         'dependents',  # noqa: E501
-        'followers',  # noqa: E501
         'hearted',  # noqa: E501
         'hearts',  # noqa: E501
         'is_rendered_as_separator',  # noqa: E501
         'likes',  # noqa: E501
         'memberships',  # noqa: E501
         'modified_at',  # noqa: E501
         'num_hearts',  # noqa: E501
         'num_likes',  # noqa: E501
         'num_subtasks',  # noqa: E501
-        'permalink_url',  # noqa: E501
-        'projects',  # noqa: E501
-        'tags',  # noqa: E501
+        'actual_time_minutes',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TaskResponseAllOf - a model defined in OpenAPI
+        """TaskBaseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -215,38 +223,41 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            actual_time_minutes (float, none_type): This value represents the sum of all the Time Tracking entries in the Actual Time field on a given Task. It is represented as a nullable long value.. [optional]  # noqa: E501
-            assignee (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            assignee_section (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            approval_status (str): *Conditional* Reflects the approval status of this task. This field is kept in sync with `completed`, meaning `pending` translates to false while `approved`, `rejected`, and `changes_requested` translate to true. If you set completed to true, this field will be set to `approved`.. [optional]  # noqa: E501
+            assignee_status (str): *Deprecated* Scheduling status of this task for the user it is assigned to. This field can only be set if the assignee is non-null. Setting this field to \"inbox\" or \"upcoming\" inserts it at the top of the section, while the other options will insert at the bottom.. [optional]  # noqa: E501
+            completed (bool): True if the task is currently marked complete, false if not.. [optional]  # noqa: E501
             completed_at (datetime, none_type): The time at which this task was completed, or null if the task is incomplete.. [optional]  # noqa: E501
-            created_at (datetime): The time at which this task was created.. [optional]  # noqa: E501
-            completed_by (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            custom_fields ([CustomFieldResponse]): Array of custom field values applied to the task. These represent the custom field values recorded on this project for a particular custom field. For example, these custom field values will contain an `enum_value` property for custom fields of type `enum`, a `text_value` property for custom fields of type `text`, and so on. Please note that the `gid` returned on each custom field value *is identical* to the `gid` of the custom field, which allows referencing the custom field metadata through the `/custom_fields/custom_field-gid` endpoint.. [optional]  # noqa: E501
+            completed_by (UserCompact): [optional]  # noqa: E501
+            created_at (datetime): The time at which this resource was created.. [optional]  # noqa: E501
             dependencies ([AsanaResource]): [Opt In](/docs/inputoutput-options). Array of resources referencing tasks that this task depends on. The objects contain only the gid of the dependency.. [optional]  # noqa: E501
             dependents ([AsanaResource]): [Opt In](/docs/inputoutput-options). Array of resources referencing tasks that depend on this task. The objects contain only the ID of the dependent.. [optional]  # noqa: E501
-            followers ([UserCompact]): Array of users following this task.. [optional]  # noqa: E501
+            due_at (date, none_type): The UTC date and time on which this task is due, or null if the task has no due time. This takes an ISO 8601 date string in UTC and should not be used together with `due_on`.. [optional]  # noqa: E501
+            due_on (date, none_type): The localized date on which this task is due, or null if the task has no due date. This takes a date with `YYYY-MM-DD` format and should not be used together with `due_at`.. [optional]  # noqa: E501
+            external (TaskBaseAllOfExternal): [optional]  # noqa: E501
+            html_notes (str): [Opt In](/docs/inputoutput-options). The notes of the text with formatting as HTML.. [optional]  # noqa: E501
             hearted (bool): *Deprecated - please use liked instead* True if the task is hearted by the authorized user, false if not.. [optional]  # noqa: E501
             hearts ([Like]): *Deprecated - please use likes instead* Array of likes for users who have hearted this task.. [optional]  # noqa: E501
             is_rendered_as_separator (bool): [Opt In](/docs/inputoutput-options). In some contexts tasks can be rendered as a visual separator; for instance, subtasks can appear similar to [sections](/reference/sections) without being true `section` objects. If a `task` object is rendered this way in any context it will have the property `is_rendered_as_separator` set to `true`.. [optional]  # noqa: E501
+            liked (bool): True if the task is liked by the authorized user, false if not.. [optional]  # noqa: E501
             likes ([Like]): Array of likes for users who have liked this task.. [optional]  # noqa: E501
-            memberships ([TaskResponseAllOfMemberships]): *Create-only*. Array of projects this task is associated with and the section it is in. At task creation time, this array can be used to add the task to specific sections. After task creation, these associations can be modified using the `addProject` and `removeProject` endpoints. Note that over time, more types of memberships may be added to this property.. [optional]  # noqa: E501
-            modified_at (datetime): The time at which this task was last modified.  *Note: This does not currently reflect any changes in associations such as projects or comments that may have been added or removed from the task.*. [optional]  # noqa: E501
+            memberships ([TaskBaseAllOfMemberships]): *Create-only*. Array of projects this task is associated with and the section it is in. At task creation time, this array can be used to add the task to specific sections. After task creation, these associations can be modified using the `addProject` and `removeProject` endpoints. Note that over time, more types of memberships may be added to this property.. [optional]  # noqa: E501
+            modified_at (datetime): The time at which this task was last modified.  The following conditions will change `modified_at`:  - story is created on a task - story is trashed on a task - attachment is trashed on a task - task is assigned or unassigned - custom field value is changed - the task itself is trashed - Or if any of the following fields are updated:   - completed   - name   - due_date   - description   - attachments   - items   - schedule_status  The following conditions will _not_ change `modified_at`:  - moving to a new container (project, portfolio, etc) - comments being added to the task (but the stories they generate   _will_ affect `modified_at`). [optional]  # noqa: E501
+            name (str): Name of the task. This is generally a short sentence fragment that fits on a line in the UI for maximum readability. However, it can be longer.. [optional]  # noqa: E501
+            notes (str): Free-form textual information associated with the task (i.e. its description).. [optional]  # noqa: E501
             num_hearts (int): *Deprecated - please use likes instead* The number of users who have hearted this task.. [optional]  # noqa: E501
             num_likes (int): The number of users who have liked this task.. [optional]  # noqa: E501
             num_subtasks (int): [Opt In](/docs/inputoutput-options). The number of subtasks on this task. . [optional]  # noqa: E501
-            parent (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            permalink_url (str): A url that points directly to the object within Asana.. [optional]  # noqa: E501
-            projects ([ProjectCompact]): *Create-only.* Array of projects this task is associated with. At task creation time, this array can be used to add the task to many projects at once. After task creation, these associations can be modified using the addProject and removeProject endpoints.. [optional]  # noqa: E501
-            tags ([TagCompact]): Array of tags associated with this task. In order to change tags on an existing task use `addTag` and `removeTag`.. [optional]  # noqa: E501
-            workspace (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            start_at (date, none_type): Date and time on which work begins for the task, or null if the task has no start time. This takes an ISO 8601 date string in UTC and should not be used together with `start_on`. *Note: `due_at` must be present in the request when setting or unsetting the `start_at` parameter.*. [optional]  # noqa: E501
+            start_on (date, none_type): The day on which work begins for the task , or null if the task has no start date. This takes a date with `YYYY-MM-DD` format and should not be used together with `start_at`. *Note: `due_on` or `due_at` must be present in the request when setting or unsetting the `start_on` parameter.*. [optional]  # noqa: E501
+            actual_time_minutes (float, none_type): This value represents the sum of all the Time Tracking entries in the Actual Time field on a given Task. It is represented as a nullable long value.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -291,15 +302,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TaskResponseAllOf - a model defined in OpenAPI
+        """TaskBaseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -324,38 +335,41 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            actual_time_minutes (float, none_type): This value represents the sum of all the Time Tracking entries in the Actual Time field on a given Task. It is represented as a nullable long value.. [optional]  # noqa: E501
-            assignee (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            assignee_section (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            approval_status (str): *Conditional* Reflects the approval status of this task. This field is kept in sync with `completed`, meaning `pending` translates to false while `approved`, `rejected`, and `changes_requested` translate to true. If you set completed to true, this field will be set to `approved`.. [optional]  # noqa: E501
+            assignee_status (str): *Deprecated* Scheduling status of this task for the user it is assigned to. This field can only be set if the assignee is non-null. Setting this field to \"inbox\" or \"upcoming\" inserts it at the top of the section, while the other options will insert at the bottom.. [optional]  # noqa: E501
+            completed (bool): True if the task is currently marked complete, false if not.. [optional]  # noqa: E501
             completed_at (datetime, none_type): The time at which this task was completed, or null if the task is incomplete.. [optional]  # noqa: E501
-            created_at (datetime): The time at which this task was created.. [optional]  # noqa: E501
-            completed_by (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            custom_fields ([CustomFieldResponse]): Array of custom field values applied to the task. These represent the custom field values recorded on this project for a particular custom field. For example, these custom field values will contain an `enum_value` property for custom fields of type `enum`, a `text_value` property for custom fields of type `text`, and so on. Please note that the `gid` returned on each custom field value *is identical* to the `gid` of the custom field, which allows referencing the custom field metadata through the `/custom_fields/custom_field-gid` endpoint.. [optional]  # noqa: E501
+            completed_by (UserCompact): [optional]  # noqa: E501
+            created_at (datetime): The time at which this resource was created.. [optional]  # noqa: E501
             dependencies ([AsanaResource]): [Opt In](/docs/inputoutput-options). Array of resources referencing tasks that this task depends on. The objects contain only the gid of the dependency.. [optional]  # noqa: E501
             dependents ([AsanaResource]): [Opt In](/docs/inputoutput-options). Array of resources referencing tasks that depend on this task. The objects contain only the ID of the dependent.. [optional]  # noqa: E501
-            followers ([UserCompact]): Array of users following this task.. [optional]  # noqa: E501
+            due_at (date, none_type): The UTC date and time on which this task is due, or null if the task has no due time. This takes an ISO 8601 date string in UTC and should not be used together with `due_on`.. [optional]  # noqa: E501
+            due_on (date, none_type): The localized date on which this task is due, or null if the task has no due date. This takes a date with `YYYY-MM-DD` format and should not be used together with `due_at`.. [optional]  # noqa: E501
+            external (TaskBaseAllOfExternal): [optional]  # noqa: E501
+            html_notes (str): [Opt In](/docs/inputoutput-options). The notes of the text with formatting as HTML.. [optional]  # noqa: E501
             hearted (bool): *Deprecated - please use liked instead* True if the task is hearted by the authorized user, false if not.. [optional]  # noqa: E501
             hearts ([Like]): *Deprecated - please use likes instead* Array of likes for users who have hearted this task.. [optional]  # noqa: E501
             is_rendered_as_separator (bool): [Opt In](/docs/inputoutput-options). In some contexts tasks can be rendered as a visual separator; for instance, subtasks can appear similar to [sections](/reference/sections) without being true `section` objects. If a `task` object is rendered this way in any context it will have the property `is_rendered_as_separator` set to `true`.. [optional]  # noqa: E501
+            liked (bool): True if the task is liked by the authorized user, false if not.. [optional]  # noqa: E501
             likes ([Like]): Array of likes for users who have liked this task.. [optional]  # noqa: E501
-            memberships ([TaskResponseAllOfMemberships]): *Create-only*. Array of projects this task is associated with and the section it is in. At task creation time, this array can be used to add the task to specific sections. After task creation, these associations can be modified using the `addProject` and `removeProject` endpoints. Note that over time, more types of memberships may be added to this property.. [optional]  # noqa: E501
-            modified_at (datetime): The time at which this task was last modified.  *Note: This does not currently reflect any changes in associations such as projects or comments that may have been added or removed from the task.*. [optional]  # noqa: E501
+            memberships ([TaskBaseAllOfMemberships]): *Create-only*. Array of projects this task is associated with and the section it is in. At task creation time, this array can be used to add the task to specific sections. After task creation, these associations can be modified using the `addProject` and `removeProject` endpoints. Note that over time, more types of memberships may be added to this property.. [optional]  # noqa: E501
+            modified_at (datetime): The time at which this task was last modified.  The following conditions will change `modified_at`:  - story is created on a task - story is trashed on a task - attachment is trashed on a task - task is assigned or unassigned - custom field value is changed - the task itself is trashed - Or if any of the following fields are updated:   - completed   - name   - due_date   - description   - attachments   - items   - schedule_status  The following conditions will _not_ change `modified_at`:  - moving to a new container (project, portfolio, etc) - comments being added to the task (but the stories they generate   _will_ affect `modified_at`). [optional]  # noqa: E501
+            name (str): Name of the task. This is generally a short sentence fragment that fits on a line in the UI for maximum readability. However, it can be longer.. [optional]  # noqa: E501
+            notes (str): Free-form textual information associated with the task (i.e. its description).. [optional]  # noqa: E501
             num_hearts (int): *Deprecated - please use likes instead* The number of users who have hearted this task.. [optional]  # noqa: E501
             num_likes (int): The number of users who have liked this task.. [optional]  # noqa: E501
             num_subtasks (int): [Opt In](/docs/inputoutput-options). The number of subtasks on this task. . [optional]  # noqa: E501
-            parent (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            permalink_url (str): A url that points directly to the object within Asana.. [optional]  # noqa: E501
-            projects ([ProjectCompact]): *Create-only.* Array of projects this task is associated with. At task creation time, this array can be used to add the task to many projects at once. After task creation, these associations can be modified using the addProject and removeProject endpoints.. [optional]  # noqa: E501
-            tags ([TagCompact]): Array of tags associated with this task. In order to change tags on an existing task use `addTag` and `removeTag`.. [optional]  # noqa: E501
-            workspace (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            start_at (date, none_type): Date and time on which work begins for the task, or null if the task has no start time. This takes an ISO 8601 date string in UTC and should not be used together with `start_on`. *Note: `due_at` must be present in the request when setting or unsetting the `start_at` parameter.*. [optional]  # noqa: E501
+            start_on (date, none_type): The day on which work begins for the task , or null if the task has no start date. This takes a date with `YYYY-MM-DD` format and should not be used together with `start_at`. *Note: `due_on` or `due_at` must be present in the request when setting or unsetting the `start_on` parameter.*. [optional]  # noqa: E501
+            actual_time_minutes (float, none_type): This value represents the sum of all the Time Tracking entries in the Actual Time field on a given Task. It is represented as a nullable long value.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `asana-preview-1.0.4/asana_preview/model/task_response_all_of_memberships.py` & `asana-preview-1.0.5/asana_preview/model/task_response_all_of_memberships.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/asana_preview/model/team_compact.py` & `asana-preview-1.0.5/asana_preview/model/member_compact.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -27,20 +27,20 @@
     OpenApiModel
 )
 from asana_preview.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from asana_preview.model.asana_resource import AsanaResource
-    from asana_preview.model.team_compact_all_of import TeamCompactAllOf
+    from asana_preview.model.member_compact_all_of import MemberCompactAllOf
     globals()['AsanaResource'] = AsanaResource
-    globals()['TeamCompactAllOf'] = TeamCompactAllOf
+    globals()['MemberCompactAllOf'] = MemberCompactAllOf
 
 
-class TeamCompact(ModelComposed):
+class MemberCompact(ModelComposed):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -86,15 +86,15 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'gid': (str,),  # noqa: E501
-            'resource_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'resource_type': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
@@ -108,15 +108,15 @@
     read_only_vars = {
         'gid',  # noqa: E501
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TeamCompact - a model defined in OpenAPI
+        """MemberCompact - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -142,16 +142,16 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            name (str): The name of the team.. [optional]  # noqa: E501
+            resource_type (str): The type of the member (team or user). [optional]  # noqa: E501
+            name (str): The name of the member. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -214,15 +214,15 @@
         '_composed_instances',
         '_var_name_to_model_instances',
         '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TeamCompact - a model defined in OpenAPI
+        """MemberCompact - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -248,16 +248,16 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            name (str): The name of the team.. [optional]  # noqa: E501
+            resource_type (str): The type of the member (team or user). [optional]  # noqa: E501
+            name (str): The name of the member. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -320,12 +320,12 @@
         # loading
         lazy_import()
         return {
           'anyOf': [
           ],
           'allOf': [
               AsanaResource,
-              TeamCompactAllOf,
+              MemberCompactAllOf,
           ],
           'oneOf': [
           ],
         }
```

### Comparing `asana-preview-1.0.4/asana_preview/model/team_compact_all_of.py` & `asana-preview-1.0.5/asana_preview/model/team_compact_all_of.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -77,25 +77,23 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'resource_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'name': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'resource_type': 'resource_type',  # noqa: E501
         'name': 'name',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
@@ -132,15 +130,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             name (str): The name of the team.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -219,15 +216,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             name (str): The name of the team.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `asana-preview-1.0.4/asana_preview/model/user_base_response.py` & `asana-preview-1.0.5/asana_preview/model/goal_relationship_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,23 +26,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from asana_preview.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from asana_preview.model.user_base_response_all_of import UserBaseResponseAllOf
-    from asana_preview.model.user_base_response_all_of_photo import UserBaseResponseAllOfPhoto
-    from asana_preview.model.user_compact import UserCompact
-    globals()['UserBaseResponseAllOf'] = UserBaseResponseAllOf
-    globals()['UserBaseResponseAllOfPhoto'] = UserBaseResponseAllOfPhoto
-    globals()['UserCompact'] = UserCompact
+    from asana_preview.model.goal_relationship_base_all_of import GoalRelationshipBaseAllOf
+    from asana_preview.model.goal_relationship_compact import GoalRelationshipCompact
+    globals()['GoalRelationshipBaseAllOf'] = GoalRelationshipBaseAllOf
+    globals()['GoalRelationshipCompact'] = GoalRelationshipCompact
 
 
-class UserBaseResponse(ModelComposed):
+class GoalRelationshipBase(ModelComposed):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -59,14 +57,18 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
+        ('resource_subtype',): {
+            'SUBGOAL': "subgoal",
+            'SUPPORTING_WORK': "supporting_work",
+        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
@@ -88,42 +90,45 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'gid': (str,),  # noqa: E501
-            'resource_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
-            'name': (str,),  # noqa: E501
-            'email': (str,),  # noqa: E501
-            'photo': (UserBaseResponseAllOfPhoto,),  # noqa: E501
+            'resource_type': (str,),  # noqa: E501
+            'resource_subtype': (str,),  # noqa: E501
+            'supporting_resource': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'contribution_weight': (float,),  # noqa: E501
+            'supported_goal': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'gid': 'gid',  # noqa: E501
         'resource_type': 'resource_type',  # noqa: E501
-        'name': 'name',  # noqa: E501
-        'email': 'email',  # noqa: E501
-        'photo': 'photo',  # noqa: E501
+        'resource_subtype': 'resource_subtype',  # noqa: E501
+        'supporting_resource': 'supporting_resource',  # noqa: E501
+        'contribution_weight': 'contribution_weight',  # noqa: E501
+        'supported_goal': 'supported_goal',  # noqa: E501
     }
 
     read_only_vars = {
         'gid',  # noqa: E501
-        'email',  # noqa: E501
+        'resource_type',  # noqa: E501
+        'resource_subtype',  # noqa: E501
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """UserBaseResponse - a model defined in OpenAPI
+        """GoalRelationshipBase - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -149,18 +154,19 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            name (str): *Read-only except when same user as requester*. The user’s name.. [optional]  # noqa: E501
-            email (str): The user's email address.. [optional]  # noqa: E501
-            photo (UserBaseResponseAllOfPhoto): [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
+            resource_subtype (str): The subtype of this resource. Different subtypes retain many of the same fields and behavior, but may render differently in Asana or represent resources with different semantic meaning.. [optional]  # noqa: E501
+            supporting_resource (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            contribution_weight (float): The weight that the supporting resource's progress contributes to the supported goal's progress. This can only be 0 or 1.. [optional]  # noqa: E501
+            supported_goal (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -223,15 +229,15 @@
         '_composed_instances',
         '_var_name_to_model_instances',
         '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """UserBaseResponse - a model defined in OpenAPI
+        """GoalRelationshipBase - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -257,18 +263,19 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            name (str): *Read-only except when same user as requester*. The user’s name.. [optional]  # noqa: E501
-            email (str): The user's email address.. [optional]  # noqa: E501
-            photo (UserBaseResponseAllOfPhoto): [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
+            resource_subtype (str): The subtype of this resource. Different subtypes retain many of the same fields and behavior, but may render differently in Asana or represent resources with different semantic meaning.. [optional]  # noqa: E501
+            supporting_resource (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            contribution_weight (float): The weight that the supporting resource's progress contributes to the supported goal's progress. This can only be 0 or 1.. [optional]  # noqa: E501
+            supported_goal (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -330,13 +337,13 @@
         # classes don't exist yet because their module has not finished
         # loading
         lazy_import()
         return {
           'anyOf': [
           ],
           'allOf': [
-              UserBaseResponseAllOf,
-              UserCompact,
+              GoalRelationshipBaseAllOf,
+              GoalRelationshipCompact,
           ],
           'oneOf': [
           ],
         }
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `asana-preview-1.0.4/asana_preview/model/user_base_response_all_of.py` & `asana-preview-1.0.5/asana_preview/model/requested_role_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -25,20 +25,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from asana_preview.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from asana_preview.model.user_base_response_all_of_photo import UserBaseResponseAllOfPhoto
-    globals()['UserBaseResponseAllOfPhoto'] = UserBaseResponseAllOfPhoto
 
-
-class UserBaseResponseAllOf(ModelNormal):
+class RequestedRoleRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -66,55 +62,52 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'email': (str,),  # noqa: E501
-            'photo': (UserBaseResponseAllOfPhoto,),  # noqa: E501
+            'gid': (str,),  # noqa: E501
+            'value': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'email': 'email',  # noqa: E501
-        'photo': 'photo',  # noqa: E501
+        'gid': 'gid',  # noqa: E501
+        'value': 'value',  # noqa: E501
     }
 
     read_only_vars = {
-        'email',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """UserBaseResponseAllOf - a model defined in OpenAPI
+        """RequestedRoleRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -139,16 +132,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            email (str): The user's email address.. [optional]  # noqa: E501
-            photo (UserBaseResponseAllOfPhoto): [optional]  # noqa: E501
+            gid (str): Globally unique identifier of the template role in the project template.. [optional]  # noqa: E501
+            value (str): The user id that should be assigned to the template role.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -193,15 +186,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """UserBaseResponseAllOf - a model defined in OpenAPI
+        """RequestedRoleRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -226,16 +219,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            email (str): The user's email address.. [optional]  # noqa: E501
-            photo (UserBaseResponseAllOfPhoto): [optional]  # noqa: E501
+            gid (str): Globally unique identifier of the template role in the project template.. [optional]  # noqa: E501
+            value (str): The user id that should be assigned to the template role.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `asana-preview-1.0.4/asana_preview/model/user_base_response_all_of_photo.py` & `asana-preview-1.0.5/asana_preview/model/user_base_response_all_of_photo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `asana-preview-1.0.4/asana_preview/model/user_compact.py` & `asana-preview-1.0.5/asana_preview/model/workspace_compact.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -27,20 +27,20 @@
     OpenApiModel
 )
 from asana_preview.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from asana_preview.model.asana_resource import AsanaResource
-    from asana_preview.model.user_compact_all_of import UserCompactAllOf
+    from asana_preview.model.workspace_compact_all_of import WorkspaceCompactAllOf
     globals()['AsanaResource'] = AsanaResource
-    globals()['UserCompactAllOf'] = UserCompactAllOf
+    globals()['WorkspaceCompactAllOf'] = WorkspaceCompactAllOf
 
 
-class UserCompact(ModelComposed):
+class WorkspaceCompact(ModelComposed):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -86,15 +86,15 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'gid': (str,),  # noqa: E501
-            'resource_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'resource_type': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
@@ -103,20 +103,21 @@
         'gid': 'gid',  # noqa: E501
         'resource_type': 'resource_type',  # noqa: E501
         'name': 'name',  # noqa: E501
     }
 
     read_only_vars = {
         'gid',  # noqa: E501
+        'resource_type',  # noqa: E501
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """UserCompact - a model defined in OpenAPI
+        """WorkspaceCompact - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -142,16 +143,16 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            name (str): *Read-only except when same user as requester*. The user’s name.. [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
+            name (str): The name of the workspace.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -214,15 +215,15 @@
         '_composed_instances',
         '_var_name_to_model_instances',
         '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """UserCompact - a model defined in OpenAPI
+        """WorkspaceCompact - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -248,16 +249,16 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            name (str): *Read-only except when same user as requester*. The user’s name.. [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
+            name (str): The name of the workspace.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -320,12 +321,12 @@
         # loading
         lazy_import()
         return {
           'anyOf': [
           ],
           'allOf': [
               AsanaResource,
-              UserCompactAllOf,
+              WorkspaceCompactAllOf,
           ],
           'oneOf': [
           ],
         }
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `asana-preview-1.0.4/asana_preview/model/user_compact_all_of.py` & `asana-preview-1.0.5/asana_preview/model/add_project_for_task_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -25,16 +25,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from asana_preview.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from asana_preview.model.task_add_project_request import TaskAddProjectRequest
+    globals()['TaskAddProjectRequest'] = TaskAddProjectRequest
 
-class UserCompactAllOf(ModelNormal):
+
+class AddProjectForTaskRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -62,52 +66,52 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'resource_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
-            'name': (str,),  # noqa: E501
+            'data': (TaskAddProjectRequest,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'resource_type': 'resource_type',  # noqa: E501
-        'name': 'name',  # noqa: E501
+        'data': 'data',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """UserCompactAllOf - a model defined in OpenAPI
+        """AddProjectForTaskRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -132,16 +136,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            name (str): *Read-only except when same user as requester*. The user’s name.. [optional]  # noqa: E501
+            data (TaskAddProjectRequest): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -186,15 +189,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """UserCompactAllOf - a model defined in OpenAPI
+        """AddProjectForTaskRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -219,16 +222,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            name (str): *Read-only except when same user as requester*. The user’s name.. [optional]  # noqa: E501
+            data (TaskAddProjectRequest): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `asana-preview-1.0.4/asana_preview/model/user_response.py` & `asana-preview-1.0.5/asana_preview/model/user_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -90,15 +90,15 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'gid': (str,),  # noqa: E501
-            'resource_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'resource_type': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'email': (str,),  # noqa: E501
             'photo': (UserBaseResponseAllOfPhoto,),  # noqa: E501
             'workspaces': ([WorkspaceCompact],),  # noqa: E501
         }
 
     @cached_property
@@ -113,14 +113,15 @@
         'email': 'email',  # noqa: E501
         'photo': 'photo',  # noqa: E501
         'workspaces': 'workspaces',  # noqa: E501
     }
 
     read_only_vars = {
         'gid',  # noqa: E501
+        'resource_type',  # noqa: E501
         'email',  # noqa: E501
         'workspaces',  # noqa: E501
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
@@ -154,15 +155,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
             name (str): *Read-only except when same user as requester*. The user’s name.. [optional]  # noqa: E501
             email (str): The user's email address.. [optional]  # noqa: E501
             photo (UserBaseResponseAllOfPhoto): [optional]  # noqa: E501
             workspaces ([WorkspaceCompact]): Workspaces and organizations this user may access. Note\\: The API will only return workspaces and organizations that also contain the authenticated user.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
@@ -263,15 +264,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
             name (str): *Read-only except when same user as requester*. The user’s name.. [optional]  # noqa: E501
             email (str): The user's email address.. [optional]  # noqa: E501
             photo (UserBaseResponseAllOfPhoto): [optional]  # noqa: E501
             workspaces ([WorkspaceCompact]): Workspaces and organizations this user may access. Note\\: The API will only return workspaces and organizations that also contain the authenticated user.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
```

### Comparing `asana-preview-1.0.4/asana_preview/model/user_response_all_of.py` & `asana-preview-1.0.5/asana_preview/model/user_response_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `asana-preview-1.0.4/asana_preview/model/workspace_compact.py` & `asana-preview-1.0.5/asana_preview/model/user_compact.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -27,20 +27,20 @@
     OpenApiModel
 )
 from asana_preview.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from asana_preview.model.asana_resource import AsanaResource
-    from asana_preview.model.workspace_compact_all_of import WorkspaceCompactAllOf
+    from asana_preview.model.user_compact_all_of import UserCompactAllOf
     globals()['AsanaResource'] = AsanaResource
-    globals()['WorkspaceCompactAllOf'] = WorkspaceCompactAllOf
+    globals()['UserCompactAllOf'] = UserCompactAllOf
 
 
-class WorkspaceCompact(ModelComposed):
+class UserCompact(ModelComposed):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -86,15 +86,15 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'gid': (str,),  # noqa: E501
-            'resource_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'resource_type': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
@@ -103,20 +103,21 @@
         'gid': 'gid',  # noqa: E501
         'resource_type': 'resource_type',  # noqa: E501
         'name': 'name',  # noqa: E501
     }
 
     read_only_vars = {
         'gid',  # noqa: E501
+        'resource_type',  # noqa: E501
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WorkspaceCompact - a model defined in OpenAPI
+        """UserCompact - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -142,16 +143,16 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            name (str): The name of the workspace.. [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
+            name (str): *Read-only except when same user as requester*. The user’s name.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -214,15 +215,15 @@
         '_composed_instances',
         '_var_name_to_model_instances',
         '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """WorkspaceCompact - a model defined in OpenAPI
+        """UserCompact - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -248,16 +249,16 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gid (str): Globally unique identifier of the resource, as a string.. [optional]  # noqa: E501
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            name (str): The name of the workspace.. [optional]  # noqa: E501
+            resource_type (str): The base type of this resource.. [optional]  # noqa: E501
+            name (str): *Read-only except when same user as requester*. The user’s name.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -320,12 +321,12 @@
         # loading
         lazy_import()
         return {
           'anyOf': [
           ],
           'allOf': [
               AsanaResource,
-              WorkspaceCompactAllOf,
+              UserCompactAllOf,
           ],
           'oneOf': [
           ],
         }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `asana-preview-1.0.4/asana_preview/model/workspace_compact_all_of.py` & `asana-preview-1.0.5/asana_preview/model/portfolio_compact_all_of.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from asana_preview.exceptions import ApiAttributeError
 
 
 
-class WorkspaceCompactAllOf(ModelNormal):
+class PortfolioCompactAllOf(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -77,37 +77,35 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'resource_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'name': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'resource_type': 'resource_type',  # noqa: E501
         'name': 'name',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WorkspaceCompactAllOf - a model defined in OpenAPI
+        """PortfolioCompactAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -132,16 +130,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            name (str): The name of the workspace.. [optional]  # noqa: E501
+            name (str): The name of the portfolio.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -186,15 +183,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """WorkspaceCompactAllOf - a model defined in OpenAPI
+        """PortfolioCompactAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -219,16 +216,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            resource_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            name (str): The name of the workspace.. [optional]  # noqa: E501
+            name (str): The name of the portfolio.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `asana-preview-1.0.4/asana_preview/model_utils.py` & `asana-preview-1.0.5/asana_preview/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
 import inspect
```

### Comparing `asana-preview-1.0.4/asana_preview/rest.py` & `asana-preview-1.0.5/asana_preview/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Asana
 
-    This is the interface for interacting with the Asana platform  # noqa: E501
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import io
 import json
 import logging
```

### Comparing `asana-preview-1.0.4/test/test_asana_named_resource.py` & `asana-preview-1.0.5/test/test_asana_named_resource.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_asana_named_resource_all_of.py` & `asana-preview-1.0.5/test/test_asana_named_resource_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_asana_resource.py` & `asana-preview-1.0.5/test/test_asana_resource.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_custom_field_base.py` & `asana-preview-1.0.5/test/test_custom_field_base.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_custom_field_base_all_of.py` & `asana-preview-1.0.5/test/test_custom_field_base_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_custom_field_compact.py` & `asana-preview-1.0.5/test/test_custom_field_compact.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_custom_field_compact_all_of.py` & `asana-preview-1.0.5/test/test_custom_field_compact_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_custom_field_compact_all_of_date_value.py` & `asana-preview-1.0.5/test/test_custom_field_compact_all_of_date_value.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_custom_field_response.py` & `asana-preview-1.0.5/test/test_custom_field_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_custom_field_response_all_of.py` & `asana-preview-1.0.5/test/test_custom_field_response_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_custom_field_setting_compact.py` & `asana-preview-1.0.5/test/test_custom_field_setting_compact.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_custom_field_setting_compact_all_of.py` & `asana-preview-1.0.5/test/test_custom_field_setting_compact_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_custom_field_setting_response.py` & `asana-preview-1.0.5/test/test_custom_field_setting_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_custom_field_setting_response_all_of.py` & `asana-preview-1.0.5/test/test_custom_field_setting_response_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_enum_option.py` & `asana-preview-1.0.5/test/test_enum_option.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_enum_option_all_of.py` & `asana-preview-1.0.5/test/test_enum_option_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_error_response.py` & `asana-preview-1.0.5/test/test_error_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_error_response5_xx.py` & `asana-preview-1.0.5/test/test_error_response5_xx.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_error_response5_xx_all_of.py` & `asana-preview-1.0.5/test/test_error_response5_xx_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_error_response5_xx_all_of_errors.py` & `asana-preview-1.0.5/test/test_error_response5_xx_all_of_errors.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_error_response_errors_inner.py` & `asana-preview-1.0.5/test/test_error_response_errors_inner.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_event_response.py` & `asana-preview-1.0.5/test/test_event_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_event_response_change.py` & `asana-preview-1.0.5/test/test_event_response_change.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_event_response_parent.py` & `asana-preview-1.0.5/test/test_event_response_parent.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_event_response_resource.py` & `asana-preview-1.0.5/test/test_event_response_resource.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_event_response_user.py` & `asana-preview-1.0.5/test/test_event_response_user.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_events_api.py` & `asana-preview-1.0.5/test/test_events_api.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_get_events200_response.py` & `asana-preview-1.0.5/test/test_get_events200_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_get_events401_response.py` & `asana-preview-1.0.5/test/test_get_events401_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_get_events401_response_all_of.py` & `asana-preview-1.0.5/test/test_get_events401_response_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_get_events401_response_all_of_errors_inner.py` & `asana-preview-1.0.5/test/test_get_events401_response_all_of_errors_inner.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_get_events403_response.py` & `asana-preview-1.0.5/test/test_get_events403_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_get_events403_response_all_of.py` & `asana-preview-1.0.5/test/test_get_events403_response_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_get_events403_response_all_of_errors_inner.py` & `asana-preview-1.0.5/test/test_get_events403_response_all_of_errors_inner.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_get_events404_response.py` & `asana-preview-1.0.5/test/test_get_events404_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_get_events404_response_all_of.py` & `asana-preview-1.0.5/test/test_get_events404_response_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_get_events404_response_all_of_errors_inner.py` & `asana-preview-1.0.5/test/test_get_events404_response_all_of_errors_inner.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_get_events412_response.py` & `asana-preview-1.0.5/test/test_get_events412_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_get_events412_response_all_of.py` & `asana-preview-1.0.5/test/test_get_events412_response_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_get_events412_response_all_of_errors_inner.py` & `asana-preview-1.0.5/test/test_get_events412_response_all_of_errors_inner.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_get_events500_response.py` & `asana-preview-1.0.5/test/test_get_events500_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_get_events500_response_all_of.py` & `asana-preview-1.0.5/test/test_get_events500_response_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_get_events500_response_all_of_errors_inner.py` & `asana-preview-1.0.5/test/test_get_events500_response_all_of_errors_inner.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_get_project200_response.py` & `asana-preview-1.0.5/test/test_get_project200_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_get_projects200_response.py` & `asana-preview-1.0.5/test/test_get_projects200_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_get_sections_for_project200_response.py` & `asana-preview-1.0.5/test/test_get_sections_for_project200_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_get_stories_for_task200_response.py` & `asana-preview-1.0.5/test/test_get_stories_for_task200_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_get_task200_response.py` & `asana-preview-1.0.5/test/test_get_task200_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_get_tasks_for_project200_response.py` & `asana-preview-1.0.5/test/test_get_tasks_for_project200_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_get_user200_response.py` & `asana-preview-1.0.5/test/test_get_user200_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_like.py` & `asana-preview-1.0.5/test/test_like.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_next_page.py` & `asana-preview-1.0.5/test/test_next_page.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_project_base.py` & `asana-preview-1.0.5/test/test_project_base.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_project_base_all_of.py` & `asana-preview-1.0.5/test/test_project_base_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_project_brief_compact.py` & `asana-preview-1.0.5/test/test_project_brief_compact.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_project_brief_compact_all_of.py` & `asana-preview-1.0.5/test/test_project_brief_compact_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_project_compact.py` & `asana-preview-1.0.5/test/test_project_compact.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_project_compact_all_of.py` & `asana-preview-1.0.5/test/test_project_compact_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_project_response.py` & `asana-preview-1.0.5/test/test_project_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_project_response_all_of.py` & `asana-preview-1.0.5/test/test_project_response_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_project_status_base.py` & `asana-preview-1.0.5/test/test_project_status_base.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_project_status_base_all_of.py` & `asana-preview-1.0.5/test/test_project_status_base_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_project_status_compact.py` & `asana-preview-1.0.5/test/test_project_status_compact.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_project_status_compact_all_of.py` & `asana-preview-1.0.5/test/test_project_status_compact_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_project_status_response.py` & `asana-preview-1.0.5/test/test_project_status_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_project_status_response_all_of.py` & `asana-preview-1.0.5/test/test_project_status_response_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_project_template_compact.py` & `asana-preview-1.0.5/test/test_project_template_compact.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_project_template_compact_all_of.py` & `asana-preview-1.0.5/test/test_project_template_compact_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_projects_api.py` & `asana-preview-1.0.5/test/test_projects_api.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_section_compact.py` & `asana-preview-1.0.5/test/test_section_compact.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_section_compact_all_of.py` & `asana-preview-1.0.5/test/test_section_compact_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_sections_api.py` & `asana-preview-1.0.5/test/test_sections_api.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_status_update_compact.py` & `asana-preview-1.0.5/test/test_status_update_compact.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_status_update_compact_all_of.py` & `asana-preview-1.0.5/test/test_status_update_compact_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_stories_api.py` & `asana-preview-1.0.5/test/test_stories_api.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_story_compact.py` & `asana-preview-1.0.5/test/test_story_compact.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_story_compact_all_of.py` & `asana-preview-1.0.5/test/test_story_compact_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_tag_compact.py` & `asana-preview-1.0.5/test/test_tag_compact.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_tag_compact_all_of.py` & `asana-preview-1.0.5/test/test_tag_compact_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_task_base.py` & `asana-preview-1.0.5/test/test_task_base.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_task_base_all_of.py` & `asana-preview-1.0.5/test/test_task_base_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_task_base_all_of_external.py` & `asana-preview-1.0.5/test/test_task_base_all_of_external.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_task_compact.py` & `asana-preview-1.0.5/test/test_task_compact.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_task_compact_all_of.py` & `asana-preview-1.0.5/test/test_task_compact_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_task_response.py` & `asana-preview-1.0.5/test/test_task_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_task_response_all_of.py` & `asana-preview-1.0.5/test/test_task_response_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_task_response_all_of_memberships.py` & `asana-preview-1.0.5/test/test_task_response_all_of_memberships.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_tasks_api.py` & `asana-preview-1.0.5/test/test_tasks_api.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_team_compact.py` & `asana-preview-1.0.5/test/test_team_compact.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_team_compact_all_of.py` & `asana-preview-1.0.5/test/test_team_compact_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_user_base_response.py` & `asana-preview-1.0.5/test/test_user_base_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_user_base_response_all_of.py` & `asana-preview-1.0.5/test/test_user_base_response_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_user_base_response_all_of_photo.py` & `asana-preview-1.0.5/test/test_user_base_response_all_of_photo.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_user_compact.py` & `asana-preview-1.0.5/test/test_user_compact.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_user_compact_all_of.py` & `asana-preview-1.0.5/test/test_user_compact_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_user_response.py` & `asana-preview-1.0.5/test/test_user_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_user_response_all_of.py` & `asana-preview-1.0.5/test/test_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_users_api.py` & `asana-preview-1.0.5/test/test_users_api.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_workspace_compact.py` & `asana-preview-1.0.5/test/test_workspace_compact.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.4/test/test_workspace_compact_all_of.py` & `asana-preview-1.0.5/test/test_workspace_compact_all_of.py`

 * *Files identical despite different names*

